# Comparing `tmp/lparchive2epub-1.0.1.tar.gz` & `tmp/lparchive2epub-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lparchive2epub-1.0.1.tar", max compression
+gzip compressed data, was "lparchive2epub-1.1.0.tar", max compression
```

## Comparing `lparchive2epub-1.0.1.tar` & `lparchive2epub-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-01-04 09:32:14.500465 lparchive2epub-1.0.1/lparchive2epub/__init__.py
--rw-r--r--   0        0        0     7247 2024-04-23 13:45:27.464182 lparchive2epub-1.0.1/lparchive2epub/lib.py
--rw-r--r--   0        0        0     1060 2024-04-23 12:56:08.358150 lparchive2epub-1.0.1/lparchive2epub/main.py
--rw-r--r--   0        0        0      727 2024-04-23 15:12:32.918569 lparchive2epub-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      921 2024-04-23 15:10:45.870943 lparchive2epub-1.0.1/README.md
--rw-r--r--   0        0        0     1475 1970-01-01 00:00:00.000000 lparchive2epub-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-04 09:32:14.500465 lparchive2epub-1.1.0/lparchive2epub/__init__.py
+-rw-r--r--   0        0        0     7657 2024-05-14 19:02:50.683162 lparchive2epub-1.1.0/lparchive2epub/lib.py
+-rw-r--r--   0        0        0      962 2024-05-09 15:59:26.997141 lparchive2epub-1.1.0/lparchive2epub/main.py
+-rw-r--r--   0        0        0      725 2024-05-14 19:02:50.685160 lparchive2epub-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      972 2024-05-14 19:02:50.679652 lparchive2epub-1.1.0/README.md
+-rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 lparchive2epub-1.1.0/PKG-INFO
```

### Comparing `lparchive2epub-1.0.1/lparchive2epub/lib.py` & `lparchive2epub-1.1.0/lparchive2epub/lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import functools
 from dataclasses import dataclass
-from multiprocessing import Pool
 from typing import List, Tuple
 
-import requests
+import aiohttp
 from bs4 import BeautifulSoup
 from ebooklib import epub
 from ebooklib.epub import EpubHtml, EpubImage, EpubBook
-from requests import Session
-import bisect
 import urllib.parse
 import os
+import asyncio
+
+from tqdm.asyncio import tqdm
+
+from contextlib import nullcontext
 
 
 @dataclass(order=True)
 class Chapters:
     num: int
     original_href: str
     txt: str
@@ -134,109 +136,125 @@
     chapter: EpubHtml
     images: List[IndexedEpubImage]
 
     def __post_init__(self):
         self.sort_index = self.num
 
 
-def _get_image(session: Session, url_root: str, img: Image) -> IndexedEpubImage:
-    r = session.get(f"{url_root}/{img.src}")
-    return IndexedEpubImage(img.num, EpubImage(uid=img.file_name, file_name=img.file_name, media_type=img.media_type,
-                                               content=r.content))
+async def _get_image(session: aiohttp.ClientSession, url_root: str, img: Image) -> IndexedEpubImage:
+    async with session.get(f"{url_root}/{img.src}") as r:
+        return IndexedEpubImage(img.num, EpubImage(
+            uid=img.file_name,
+            file_name=img.file_name,
+            media_type=img.media_type,
+            content=await r.content.read()))
 
 
-def build_intro(pool: Pool, session: Session, url_root: str, intro: Intro) -> Page:
+async def build_intro(session: aiohttp.ClientSession, url_root: str, intro: Intro) -> Page:
     intro_chapter = epub.EpubHtml(title="Introduction", file_name="introduction.xhtml", lang=intro.language)
     intro_chapter.content = intro.intro
-    images = []
 
-    builder = functools.partial(_get_image, session, url_root)
+    tasks = []
+    for image in intro.images:
+        task = asyncio.ensure_future(_get_image(session, url_root, image))
+        tasks.append(task)
 
-    for i in pool.imap_unordered(builder, intro.images):
-        bisect.insort(images, i)
+    images = await asyncio.gather(*tasks)
 
     return Page(0, intro_chapter, images)
 
 
-def build_update(session: Session, chapter: Chapters, data: Update, intro: Intro) -> Page:
+async def build_update(session: aiohttp.ClientSession, chapter: Chapters, data: Update, intro: Intro) -> Page:
     update_chapter = epub.EpubHtml(title=chapter.txt, file_name=chapter.new_href,
                                    lang=intro.language)  # TODO: fix language
     update_chapter.content = data.content
 
     img_builder = functools.partial(_get_image, session, chapter.original_href)
 
-    images: List[IndexedEpubImage] = list(map(img_builder, data.images))
+    tasks = []
+    for image in data.images:
+        task = asyncio.ensure_future(img_builder(image))
+        tasks.append(task)
+
+    images = await asyncio.gather(*tasks)
 
     return Page(chapter.num, update_chapter, images)
 
 
 def add_page(book: EpubBook, toc: List, spine: List, page: Page):
     book.add_item(page.chapter)
     for img in page.images:
         book.add_item(img.data)
     toc.append(epub.Link(page.chapter.file_name, page.chapter.title, page.chapter.id))
     spine.append(page.chapter)
 
 
-def build_single_page(session: Session, intro: Intro, chapter: Chapters) -> Page:
-    chapter_page = session.get(chapter.original_href)
-    chapter_bs = BeautifulSoup(chapter_page.content, 'html.parser')
+async def build_single_page(session: aiohttp.ClientSession(), intro: Intro, chapter: Chapters) -> Page:
+    chapter_page = await session.get(chapter.original_href)
+    chapter_bs = BeautifulSoup(await chapter_page.text(), 'html.parser')
     update = Extractor.get_update(str(chapter.num), chapter_bs)
-    return build_update(session, chapter, update, intro)
+    return await build_update(session, chapter, update, intro)
 
 
 class DummyUpdater:
 
     def __init__(self, *args, **kwargs):
         pass
 
     #todo: everything
 
 
-def lparchive2epub(update_manager, session: Session, pool: Pool, url: str, file: str):
-    if update_manager is None:
-        update_manager = DummyUpdater
+async def lparchive2epub(url: str, file: str, root_session: [aiohttp.ClientSession | None] = None, with_pbar: bool = True):
+    if root_session is None:
+        root_session = aiohttp.ClientSession()
+    async with root_session as session:
+        await do(url, file, session, with_pbar)
+
+
+async def do(url: str, file: str, session: aiohttp.ClientSession, with_pbar: bool):
+    page = await session.get(url)
+    landing = BeautifulSoup(await page.text(), 'html.parser')
 
-    page = session.get(url)
-    landing = BeautifulSoup(page.content, 'html.parser')
     book = epub.EpubBook()
     intro = Extractor.intro(url, landing)
 
     book.add_author(intro.author)
     book.set_title(intro.title)
     book.set_language(intro.language)
     book.add_metadata("DC", "source", url)
     book.set_identifier(f"lparchive2epub-{hash(intro.title)}-{hash(intro.author)}-{hash(url)}")
 
     toc = []
     spine = ["nav"]
 
-    epub_intro = build_intro(pool, session, url, intro)
+    epub_intro = await build_intro(session, url, intro)
 
     add_page(book, toc, spine, epub_intro)
 
-    page_builder = functools.partial(build_single_page, session)
-    page_builder = functools.partial(page_builder, intro)
-
     # pages takes a vastly inequal times to get, so it's faster to imap_unordered and do a simple bisect.insort
     # gotta go fast, but also keep the page order.
-    pages_iterator = pool.imap_unordered(page_builder, intro.chapters)
-    pages = []
-    with update_manager(total=len(intro.chapters)) as pbar:
-        for p in pages_iterator:
-            bisect.insort(pages, p)
-            pbar.update()
+
+    tasks = []
+
+    for chapter in intro.chapters:
+        task = asyncio.ensure_future(build_single_page(session, intro, chapter))
+        tasks.append(task)
+
+    gatherer = tqdm.gather if with_pbar else asyncio.gather
+
+    pages = await gatherer(*tasks)
+    pages = sorted(pages)
 
     for p in pages:
         add_page(book, toc, spine, p)
 
     book.toc = toc
 
     book.add_item(epub.EpubNcx())
     book.add_item(epub.EpubNav())
 
     book.spine = spine
 
     epub.write_epub(file, book)
 
 # todo: check for links like in headshoots
-# todo: deduplicate images when possible. 
+# todo: deduplicate images when possible.
```

### Comparing `lparchive2epub-1.0.1/lparchive2epub/main.py` & `lparchive2epub-1.1.0/lparchive2epub/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+import asyncio
 from argparse import ArgumentParser, ArgumentTypeError
-from multiprocessing import Pool
+
 from urllib.parse import urlparse
 
-from requests import Session
 
 from lparchive2epub.lib import lparchive2epub
-from tqdm import tqdm
+from tqdm import asyncio as tqdm
 
 def is_lparchive_url(arg):
     url = urlparse(arg)
     if not "lparchive.org" in url.geturl():
         raise ArgumentTypeError(f"{arg} is not an lparchive.org URL")
     if not url.path or url.path == "/":
         raise ArgumentTypeError(f"{arg} is not a let's play archive")
@@ -23,14 +23,12 @@
 
 arg_parser.add_argument("url", metavar="URL", nargs=1, type=is_lparchive_url)
 arg_parser.add_argument("output", metavar="OUTPUT_FILE", nargs=1, type=str)
 
 
 def main():
     args = arg_parser.parse_args()
-    session = Session()
-    with Pool() as pool:
-        lparchive2epub(tqdm, session, pool, args.url[0], args.output[0])
+    asyncio.run(lparchive2epub(args.url[0], args.output[0]))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `lparchive2epub-1.0.1/pyproject.toml` & `lparchive2epub-1.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "lparchive2epub"
-version = "1.0.1"
+version = "1.1.0"
 description = ""
 authors = ["Arwalk <siragentprovocateurarwalk@gmail.com>"]
 readme = "README.md"
 packages = [{include = "lparchive2epub"}]
 repository = "https://github.com/Arwalk/lparchive2epub"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 ebooklib = "^0.18"
-requests = "^2.31.0"
 beautifulsoup4 = "^4.12.2"
-tqdm = "^4.66.2"
+tqdm = "^4.66.4"
+aiohttp = "^3.9.5"
 
 [tool.poetry.scripts]
 lparchive2epub = 'lparchive2epub.main:main'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lparchive2epub-1.0.1/README.md` & `lparchive2epub-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -23,13 +23,17 @@
 
 Poetry, python 3.12
 
 ### Users
 
 python 3.12
 
+## Installation
+
+`pip install lparchive2epub`
+
 ## Known limitations
 
 - Similar images present in multiple pages in the let's play are duplicated, bloating the file. Though recurring images are usually smileys, so not too big.
 - Links to images are not properly saved.
 - LPs that are mostly link to YouTube videos are not very interesting to transform to epub
 - Some LPs completely fail to be downloaded.
```

### Comparing `lparchive2epub-1.0.1/PKG-INFO` & `lparchive2epub-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: lparchive2epub
-Version: 1.0.1
+Version: 1.1.0
 Summary: 
 Home-page: https://github.com/Arwalk/lparchive2epub
 Author: Arwalk
 Author-email: siragentprovocateurarwalk@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: ebooklib (>=0.18,<0.19)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Project-URL: Repository, https://github.com/Arwalk/lparchive2epub
 Description-Content-Type: text/markdown
 
 # lparchive2pub
 
 this tool (and library) aims at helping people extracting full epubs of Let's Plays from https://lparchive.org/
 
@@ -40,13 +40,17 @@
 
 Poetry, python 3.12
 
 ### Users
 
 python 3.12
 
+## Installation
+
+`pip install lparchive2epub`
+
 ## Known limitations
 
 - Similar images present in multiple pages in the let's play are duplicated, bloating the file. Though recurring images are usually smileys, so not too big.
 - Links to images are not properly saved.
 - LPs that are mostly link to YouTube videos are not very interesting to transform to epub
 - Some LPs completely fail to be downloaded.
```

