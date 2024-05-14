# Comparing `tmp/docprompt-0.4.6.tar.gz` & `tmp/docprompt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.4.6.tar", last modified: Sun May 12 22:46:44 2024, max compression
+gzip compressed data, was "docprompt-0.5.0.tar", last modified: Tue May 14 06:54:24 2024, max compression
```

## Comparing `docprompt-0.4.6.tar` & `docprompt-0.5.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.4.6/LICENSE
--rw-r--r--   0        0        0     5174 2024-05-10 05:55:50.188361 docprompt-0.4.6/README.md
--rw-r--r--   0        0        0      752 2024-05-12 22:46:23.635955 docprompt-0.4.6/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.4.6/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.4.6/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0     1545 2024-05-12 22:42:37.149558 docprompt-0.4.6/docprompt/_pdfium.py
--rw-r--r--   0        0        0      107 2024-05-06 05:10:23.648879 docprompt-0.4.6/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9861 2024-05-10 22:04:25.589467 docprompt-0.4.6/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1425 2024-05-10 22:19:31.977780 docprompt-0.4.6/docprompt/provenance/source.py
--rw-r--r--   0        0        0     5771 2024-05-10 22:19:31.977780 docprompt-0.4.6/docprompt/provenance/util.py
--rw-r--r--   0        0        0     7097 2024-05-07 00:41:50.085452 docprompt-0.4.6/docprompt/rasterize.py
--rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.4.6/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     9548 2024-05-12 22:44:37.214627 docprompt-0.4.6/docprompt/schema/document.py
--rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.4.6/docprompt/schema/layout.py
--rw-r--r--   0        0        0    12026 2024-05-07 01:27:16.164027 docprompt-0.4.6/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.4.6/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.4.6/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.4.6/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.4.6/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.4.6/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.4.6/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.4.6/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.4.6/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.4.6/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.4.6/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.4.6/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.4.6/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      375 2024-05-04 01:28:27.264357 docprompt-0.4.6/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.4.6/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.4.6/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-04-16 21:31:16.273985 docprompt-0.4.6/docprompt/utils/masking/__init__.py
--rw-r--r--   0        0        0      707 2024-04-17 06:27:28.658476 docprompt-0.4.6/docprompt/utils/masking/image.py
--rw-r--r--   0        0        0     3577 2024-05-06 23:51:36.501689 docprompt-0.4.6/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     4088 2024-05-06 23:51:36.485689 docprompt-0.4.6/docprompt/utils/util.py
--rw-r--r--   0        0        0     2717 2024-05-12 22:46:44.480225 docprompt-0.4.6/pyproject.toml
--rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.4.6/tests/__init__.py
--rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.4.6/tests/fixtures.py
--rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.4.6/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.4.6/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.4.6/tests/test_date_extraction.py
--rw-r--r--   0        0        0     5545 2024-05-12 22:45:37.195345 docprompt-0.4.6/tests/test_document.py
--rw-r--r--   0        0        0     1813 2024-05-07 01:14:14.543427 docprompt-0.4.6/tests/test_documentnode.py
--rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.4.6/tests/test_layout_models.py
--rw-r--r--   0        0        0     2868 2024-05-10 22:19:31.977780 docprompt-0.4.6/tests/test_search.py
--rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.4.6/tests/test_threadpool.py
--rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.4.6/tests/util.py
--rw-r--r--   0        0        0     6689 1970-01-01 00:00:00.000000 docprompt-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5174 2024-05-10 05:55:50.188361 docprompt-0.5.0/README.md
+-rw-r--r--   0        0        0      752 2024-05-14 06:54:02.321496 docprompt-0.5.0/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.5.0/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.5.0/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0     1545 2024-05-12 22:42:37.149558 docprompt-0.5.0/docprompt/_pdfium.py
+-rw-r--r--   0        0        0        0 2024-05-14 05:11:38.652722 docprompt-0.5.0/docprompt/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 05:15:17.130391 docprompt-0.5.0/docprompt/contrib/parser_bot/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-06 05:10:23.648879 docprompt-0.5.0/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9861 2024-05-10 22:04:25.589467 docprompt-0.5.0/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1425 2024-05-10 22:19:31.977780 docprompt-0.5.0/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     5771 2024-05-10 22:19:31.977780 docprompt-0.5.0/docprompt/provenance/util.py
+-rw-r--r--   0        0        0     7097 2024-05-07 00:41:50.085452 docprompt-0.5.0/docprompt/rasterize.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.5.0/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0     9524 2024-05-14 06:52:55.136274 docprompt-0.5.0/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6649 2024-05-14 01:50:59.692646 docprompt-0.5.0/docprompt/schema/layout.py
+-rw-r--r--   0        0        0    12176 2024-05-14 06:53:16.252663 docprompt-0.5.0/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.5.0/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.5.0/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.5.0/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.5.0/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.5.0/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18558 2024-05-14 01:51:01.492661 docprompt-0.5.0/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.5.0/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.5.0/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      737 2024-05-14 06:53:16.252663 docprompt-0.5.0/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.5.0/docprompt/tasks/table_extraction/schema.py
+-rw-r--r--   0        0        0      375 2024-05-04 01:28:27.264357 docprompt-0.5.0/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.5.0/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.5.0/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-04-16 21:31:16.273985 docprompt-0.5.0/docprompt/utils/masking/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-17 06:27:28.658476 docprompt-0.5.0/docprompt/utils/masking/image.py
+-rw-r--r--   0        0        0     3577 2024-05-06 23:51:36.501689 docprompt-0.5.0/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     4073 2024-05-14 06:53:04.120440 docprompt-0.5.0/docprompt/utils/util.py
+-rw-r--r--   0        0        0     2735 2024-05-14 06:54:24.057881 docprompt-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.5.0/tests/fixtures.py
+-rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.5.0/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.5.0/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.5.0/tests/test_date_extraction.py
+-rw-r--r--   0        0        0     5545 2024-05-12 22:45:37.195345 docprompt-0.5.0/tests/test_document.py
+-rw-r--r--   0        0        0     1813 2024-05-07 01:14:14.543427 docprompt-0.5.0/tests/test_documentnode.py
+-rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.5.0/tests/test_layout_models.py
+-rw-r--r--   0        0        0     2868 2024-05-10 22:19:31.977780 docprompt-0.5.0/tests/test_search.py
+-rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.5.0/tests/test_threadpool.py
+-rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.5.0/tests/util.py
+-rw-r--r--   0        0        0     6684 1970-01-01 00:00:00.000000 docprompt-0.5.0/PKG-INFO
```

### Comparing `docprompt-0.4.6/LICENSE` & `docprompt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/README.md` & `docprompt-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/__init__.py` & `docprompt-0.5.0/docprompt/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Docprompt."""
 
 __author__ = """Frankie Colson"""
 __email__ = "frank@pageleaf.io"
-__version__ = "0.4.6"
+__version__ = "0.5.0"
 
 from docprompt.schema.document import Document, PdfDocument  # noqa
 from docprompt.schema.layout import NormBBox, TextBlock  # noqa
 from docprompt.schema.pipeline import DocumentCollection, DocumentNode, PageNode  # noqa
 from docprompt.utils import load_document, load_documents, hash_from_bytes  # noqa
 from docprompt.rasterize import ProviderResizeRatios
```

### Comparing `docprompt-0.4.6/docprompt/_exec/ghostscript.py` & `docprompt-0.5.0/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/_pdfium.py` & `docprompt-0.5.0/docprompt/_pdfium.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/provenance/search.py` & `docprompt-0.5.0/docprompt/provenance/search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/provenance/source.py` & `docprompt-0.5.0/docprompt/provenance/source.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/provenance/util.py` & `docprompt-0.5.0/docprompt/provenance/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/rasterize.py` & `docprompt-0.5.0/docprompt/rasterize.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/schema/document.py` & `docprompt-0.5.0/docprompt/schema/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from datetime import datetime
 from functools import cached_property
 from io import BytesIO
 from os import PathLike
 from pathlib import Path
 from typing import Dict, Generator, Optional, Tuple, Union, Iterable
 from pydantic import Field
+import filetype
 
-import magic
 from pydantic import (
     BaseModel,
     PositiveInt,
     computed_field,
     field_serializer,
     field_validator,
 )
@@ -103,21 +103,21 @@
     def validate_file_bytes(cls, v: bytes):
         if not isinstance(v, bytes):
             raise ValueError("File bytes must be bytes")
 
         if len(v) == 0:
             raise ValueError("File bytes must not be empty")
 
-        if magic.from_buffer(v, mime=True) == "text/plain":
+        if filetype.guess_mime(v) == "text/plain":
             v = base64.b64decode(v, validate=True)
 
-        if magic.from_buffer(v, mime=True) == "application/gzip":
+        if filetype.guess_mime(v) == "application/gzip":
             v = gzip.decompress(v)
 
-        if magic.from_buffer(v, mime=True) != "application/pdf":
+        if filetype.guess_mime(v) != "application/pdf":
             raise ValueError("File bytes must be a PDF")
 
         return v
 
     @classmethod
     def from_path(cls, file_path: Union[PathLike, str]):
         file_path = Path(file_path)
```

### Comparing `docprompt-0.4.6/docprompt/schema/layout.py` & `docprompt-0.5.0/docprompt/schema/layout.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/schema/pipeline.py` & `docprompt-0.5.0/docprompt/schema/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 from io import BytesIO
 import multiprocessing
 from typing import (
+    Any,
     Dict,
     Generic,
     Iterable,
     List,
     Literal,
     Optional,
     Tuple,
@@ -252,14 +253,18 @@
     """
 
     document: "DocumentNode" = Field(exclude=True, repr=False)
     page_number: PositiveInt = Field(description="The page number")
     metadata: Optional[PageNodeMetadata] = Field(
         description="Application-specific metadata for the page", default=None
     )
+    extra: Dict[str, Any] = Field(
+        description="Extra data that can be stored on the page node",
+        default_factory=dict,
+    )
 
     ocr_results: ResultContainer[OcrPageResult] = Field(
         default_factory=lambda: ResultContainer(),
         description="The OCR results for the page",
         repr=False,
     )
```

### Comparing `docprompt-0.4.6/docprompt/tasks/base.py` & `docprompt-0.5.0/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/tasks/message.py` & `docprompt-0.5.0/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/tasks/ocr/gcp.py` & `docprompt-0.5.0/docprompt/tasks/ocr/gcp.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/tasks/ocr/result.py` & `docprompt-0.5.0/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/tasks/table_extraction/base.py` & `docprompt-0.5.0/docprompt/tasks/table_extraction/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Dict
 from docprompt.schema.pipeline import DocumentNode
 from docprompt.tasks.base import AbstractLanguageModelTaskProvider, CAPABILITIES
-from .result import TableExtractionPageResult
+from .schema import TableExtractionPageResult
 
 
 class BaseTableExtractionProvider(AbstractLanguageModelTaskProvider):
     capabilities = [
         CAPABILITIES.PAGE_TABLE_IDENTIFICATION.value,
         CAPABILITIES.PAGE_TABLE_EXTRACTION.value,
     ]
 
     def contribute_to_document_node(
         self, document_node: DocumentNode, results: Dict[int, TableExtractionPageResult]
     ) -> None:
         for page_number, page_result in results.items():
-            document_node.page_nodes[page_number - 1].table_extraction_results.results[
-                self.name
-            ] = page_result
+            document_node.page_nodes[page_number - 1].extra["extracted_tables"] = (
+                page_result.tables
+            )
```

### Comparing `docprompt-0.4.6/docprompt/tasks/table_extraction/result.py` & `docprompt-0.5.0/docprompt/tasks/table_extraction/schema.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/utils/date_extraction.py` & `docprompt-0.5.0/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/utils/masking/image.py` & `docprompt-0.5.0/docprompt/utils/masking/image.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/utils/splitter.py` & `docprompt-0.5.0/docprompt/utils/splitter.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/docprompt/utils/util.py` & `docprompt-0.5.0/docprompt/utils/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from os import PathLike
 from pathlib import Path
 from typing import List, Optional, Union
 from urllib.parse import unquote, urlparse
 import warnings
 
 import fsspec
-import magic
+import filetype
 
 from docprompt.schema.document import PdfDocument
 from docprompt._pdfium import get_pdfium_document
 
 
 def is_pdf(fd: Union[Path, PathLike, bytes]) -> bool:
     """
     Determines if a file is a PDF
     """
     if isinstance(fd, (bytes, str)):
-        mime = magic.from_buffer(fd, mime=True)
+        mime = filetype.guess_mime(fd)
     else:
         with open(fd, "rb") as f:
             # We only need the first 1024 bytes to determine if it's a PDF
-            mime = magic.from_buffer(f.read(1024), mime=True)
+            mime = filetype.guess_mime(f.read(1024))
 
     return mime == "application/pdf"
 
 
 def get_page_count(fd: Union[Path, PathLike, bytes]) -> int:
     """
     Determines the number of pages in a PDF
```

### Comparing `docprompt-0.4.6/pyproject.toml` & `docprompt-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "docprompt"
-version = "0.4.6"
+version = "0.5.0"
 description = "Documents and large language models."
 authors = [
     { name = "Frank Colson", email = "frank@pageleaf.io" },
 ]
 dependencies = [
     "python-dateutil<3.0.0,>=2.8.2",
     "pillow>=9.0.1",
-    "python-magic>=0.4.24",
     "tqdm>=4.50.2",
     "fsspec>=2022.11.0",
     "pydantic>=2.1.0",
     "tenacity>=7.0.0",
     "pypdfium2<5.0.0,>=4.28.0",
     "rapidfuzz>=3.0.0",
+    "filetype>=1.2.0",
 ]
 requires-python = "<3.13,>=3.8.1"
 readme = "README.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
@@ -107,14 +107,15 @@
     "tox<4.0.0,>=3.20.1",
     "virtualenv<21.0.0,>=20.2.2",
     "pip<21.0.0,>=20.3.1",
     "twine<4.0.0,>=3.3.0",
     "pre-commit<3.0.0,>=2.12.0",
     "toml<1.0.0,>=0.10.2",
     "bump2version<2.0.0,>=1.0.1",
+    "ipython>=8.12.3",
 ]
 
 [tool.ruff]
 target-version = "py38"
 
 [tool.ruff.lint]
 select = [
```

### Comparing `docprompt-0.4.6/tests/fixtures/1.pdf` & `docprompt-0.5.0/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/tests/fixtures/1_ocr.json` & `docprompt-0.5.0/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/tests/test_date_extraction.py` & `docprompt-0.5.0/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/tests/test_document.py` & `docprompt-0.5.0/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/tests/test_documentnode.py` & `docprompt-0.5.0/tests/test_documentnode.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/tests/test_layout_models.py` & `docprompt-0.5.0/tests/test_layout_models.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/tests/test_search.py` & `docprompt-0.5.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/tests/test_threadpool.py` & `docprompt-0.5.0/tests/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/tests/util.py` & `docprompt-0.5.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.6/PKG-INFO` & `docprompt-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docprompt
-Version: 0.4.6
+Version: 0.5.0
 Summary: Documents and large language models.
 Home-page: https://github.com/Page-Leaf/docprompt
 Author-Email: Frank Colson <frank@pageleaf.io>
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,21 +15,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Homepage, https://github.com/Page-Leaf/docprompt
 Requires-Python: <3.13,>=3.8.1
 Requires-Dist: python-dateutil<3.0.0,>=2.8.2
 Requires-Dist: pillow>=9.0.1
-Requires-Dist: python-magic>=0.4.24
 Requires-Dist: tqdm>=4.50.2
 Requires-Dist: fsspec>=2022.11.0
 Requires-Dist: pydantic>=2.1.0
 Requires-Dist: tenacity>=7.0.0
 Requires-Dist: pypdfium2<5.0.0,>=4.28.0
 Requires-Dist: rapidfuzz>=3.0.0
+Requires-Dist: filetype>=1.2.0
 Requires-Dist: google-cloud-documentai>=2.20.0; extra == "google"
 Requires-Dist: azure-ai-formrecognizer>=3.3.0; extra == "azure"
 Requires-Dist: tantivy<1.0.0,>=0.21.0; extra == "search"
 Requires-Dist: rtree<2.0.0,>=1.2.0; extra == "search"
 Requires-Dist: networkx<3.2,>=2.8.8; extra == "search"
 Provides-Extra: google
 Provides-Extra: azure
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: docprompt Version: 0.4.6 Summary: Documents and
+Metadata-Version: 2.1 Name: docprompt Version: 0.5.0 Summary: Documents and
 large language models. Home-page: https://github.com/Page-Leaf/docprompt
 Author-Email: Frank Colson
 pageleaf.io> License: Apache-2.0 Classifier: Development Status :: 2 - Pre-
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Homepage, https://github.com/Page-Leaf/docprompt Requires-Python:
 <3.13,>=3.8.1 Requires-Dist: python-dateutil<3.0.0,>=2.8.2 Requires-Dist:
-pillow>=9.0.1 Requires-Dist: python-magic>=0.4.24 Requires-Dist: tqdm>=4.50.2
-Requires-Dist: fsspec>=2022.11.0 Requires-Dist: pydantic>=2.1.0 Requires-Dist:
-tenacity>=7.0.0 Requires-Dist: pypdfium2<5.0.0,>=4.28.0 Requires-Dist:
-rapidfuzz>=3.0.0 Requires-Dist: google-cloud-documentai>=2.20.0; extra ==
+pillow>=9.0.1 Requires-Dist: tqdm>=4.50.2 Requires-Dist: fsspec>=2022.11.0
+Requires-Dist: pydantic>=2.1.0 Requires-Dist: tenacity>=7.0.0 Requires-Dist:
+pypdfium2<5.0.0,>=4.28.0 Requires-Dist: rapidfuzz>=3.0.0 Requires-Dist:
+filetype>=1.2.0 Requires-Dist: google-cloud-documentai>=2.20.0; extra ==
 "google" Requires-Dist: azure-ai-formrecognizer>=3.3.0; extra == "azure"
 Requires-Dist: tantivy<1.0.0,>=0.21.0; extra == "search" Requires-Dist:
 rtree<2.0.0,>=1.2.0; extra == "search" Requires-Dist: networkx<3.2,>=2.8.8;
 extra == "search" Provides-Extra: google Provides-Extra: azure Provides-Extra:
 search Description-Content-Type: text/markdown [![pypi](https://img.shields.io/
 pypi/v/docprompt.svg)](https://pypi.org/project/docprompt/) [![python](https://
 img.shields.io/pypi/pyversions/docprompt.svg)](https://pypi.org/project/
```

