# Comparing `tmp/mathbib-0.7.8.tar.gz` & `tmp/mathbib-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.7.8.tar", max compression
+gzip compressed data, was "mathbib-0.7.9.tar", max compression
```

## Comparing `mathbib-0.7.8.tar` & `mathbib-0.7.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.7.8/LICENSE
--rw-r--r--   0        0        0     6085 2023-08-30 21:46:36.307290 mathbib-0.7.8/README.md
--rw-r--r--   0        0        0      143 2023-07-22 11:31:07.945040 mathbib-0.7.8/mathbib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.7.8/mathbib/__main__.py
--rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.7.8/mathbib/bibtex.py
--rw-r--r--   0        0        0     3326 2023-07-13 10:48:13.319332 mathbib-0.7.8/mathbib/citegen.py
--rw-r--r--   0        0        0    12333 2023-09-11 14:10:38.499381 mathbib-0.7.8/mathbib/command.py
--rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.7.8/mathbib/partition.py
--rw-r--r--   0        0        0    10779 2023-09-11 14:43:23.350824 mathbib-0.7.8/mathbib/record.py
--rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.7.8/mathbib/remote/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.7.8/mathbib/remote/arxiv.py
--rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.7.8/mathbib/remote/doi.py
--rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.7.8/mathbib/remote/error.py
--rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.7.8/mathbib/remote/isbn.py
--rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.7.8/mathbib/remote/ol.py
--rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.7.8/mathbib/remote/utils.py
--rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.7.8/mathbib/remote/zbl.py
--rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.7.8/mathbib/remote/zbmath.py
--rw-r--r--   0        0        0     6688 2023-06-04 07:43:41.660653 mathbib-0.7.8/mathbib/request.py
--rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.7.8/mathbib/resources/__init__.py
--rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.7.8/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0        0        0     3269 2023-08-24 16:43:32.574977 mathbib-0.7.8/mathbib/session.py
--rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.7.8/mathbib/term.py
--rw-r--r--   0        0        0      953 2023-09-11 14:44:51.212410 mathbib-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     6974 1970-01-01 00:00:00.000000 mathbib-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.7.9/LICENSE
+-rw-r--r--   0        0        0     6091 2023-09-11 22:05:12.203070 mathbib-0.7.9/README.md
+-rw-r--r--   0        0        0      143 2023-07-22 11:31:07.945040 mathbib-0.7.9/mathbib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.7.9/mathbib/__main__.py
+-rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.7.9/mathbib/bibtex.py
+-rw-r--r--   0        0        0     3326 2023-07-13 10:48:13.319332 mathbib-0.7.9/mathbib/citegen.py
+-rw-r--r--   0        0        0    12333 2023-09-11 14:10:38.499381 mathbib-0.7.9/mathbib/command.py
+-rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.7.9/mathbib/partition.py
+-rw-r--r--   0        0        0    10779 2023-09-11 14:43:23.350824 mathbib-0.7.9/mathbib/record.py
+-rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.7.9/mathbib/remote/__init__.py
+-rw-r--r--   0        0        0     3095 2023-10-08 11:59:01.891690 mathbib-0.7.9/mathbib/remote/arxiv.py
+-rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.7.9/mathbib/remote/doi.py
+-rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.7.9/mathbib/remote/error.py
+-rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.7.9/mathbib/remote/isbn.py
+-rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.7.9/mathbib/remote/ol.py
+-rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.7.9/mathbib/remote/utils.py
+-rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.7.9/mathbib/remote/zbl.py
+-rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.7.9/mathbib/remote/zbmath.py
+-rw-r--r--   0        0        0     6688 2023-06-04 07:43:41.660653 mathbib-0.7.9/mathbib/request.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.7.9/mathbib/resources/__init__.py
+-rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.7.9/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0        0        0     3269 2023-08-24 16:43:32.574977 mathbib-0.7.9/mathbib/session.py
+-rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.7.9/mathbib/term.py
+-rw-r--r--   0        0        0      953 2023-10-08 11:59:30.840261 mathbib-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     6980 1970-01-01 00:00:00.000000 mathbib-0.7.9/PKG-INFO
```

### Comparing `mathbib-0.7.8/LICENSE` & `mathbib-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/README.md` & `mathbib-0.7.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 \addbibresource{doc.bib}
 \begin{document}
 This document references an article \cite{Hoc2014}.
 It also contains more references \cite{HocShm2012, Shm2019}.
 \printbibliography
 \end{document}
 ```
-Remember to regenerate the `doc.bib` file with `mbib generate doc.tex > doc.bib` (the citation keys need to be updated), and the file will compile!
+Remember to regenerate the `doc.bib` file with `mbib generate doc.tex --out doc.bib` (the citation keys need to be updated), and the file will compile!
 Aliases also work as command line arguments anywhere a `key:id` is expected.
 
 Suppose you have been working on the above TEX document for a while, and now you want to cite a specific theorem from the paper `Hoc2014`.
 Simply run
 ```sh
 mbib file open Hoc2014
 ```
@@ -86,15 +86,15 @@
 Of course, if `mbib` cannot find a resource for your file, you can also add one yourself.
 ```sh
 mbib file add Hoc2014 path/to/file.pdf
 ```
 
 Finally, if you have loaded a record but there are mistakes (for instance, improperly formatted LaTeX), you can apply local modifications which will always be applied when requesting the record.
 Edit the local record with, for example,
-```
+```sh
 mbib file open zbl:1251.28008
 ```
 There are also other features implemented: either read more below, or run `mbib --help` and `mbib <subcommand> --help` for more information.
 
 
 ## Remote and local records
 Internally, whenever you request a new record, MathBib searches a few online data repositories for the information associated with the record.
```

### Comparing `mathbib-0.7.8/mathbib/bibtex.py` & `mathbib-0.7.9/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/citegen.py` & `mathbib-0.7.9/mathbib/citegen.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/command.py` & `mathbib-0.7.9/mathbib/command.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/partition.py` & `mathbib-0.7.9/mathbib/partition.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/record.py` & `mathbib-0.7.9/mathbib/record.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/remote/__init__.py` & `mathbib-0.7.9/mathbib/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/remote/arxiv.py` & `mathbib-0.7.9/mathbib/remote/arxiv.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 def show_url(arxiv: str) -> str:
     return f"https://arxiv.org/abs/{arxiv}"
 
 
 def download_url(arxiv: str) -> str:
-    return f"https://arxiv.org/pdf/{arxiv}.pdf"
+    return f"https://browse.arxiv.org/pdf/{arxiv}.pdf"
 
 
 def record_parser(result: str) -> ParsedRecord:
     # TODO: sometimes this returns the incorrect record, which needs to be checked
 
     related = [
         RelatedRecord(
```

### Comparing `mathbib-0.7.8/mathbib/remote/doi.py` & `mathbib-0.7.9/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/remote/error.py` & `mathbib-0.7.9/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/remote/isbn.py` & `mathbib-0.7.9/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/remote/ol.py` & `mathbib-0.7.9/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/remote/utils.py` & `mathbib-0.7.9/mathbib/remote/utils.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/remote/zbl.py` & `mathbib-0.7.9/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/remote/zbmath.py` & `mathbib-0.7.9/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/request.py` & `mathbib-0.7.9/mathbib/request.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/resources/journal_abbrevs.json` & `mathbib-0.7.9/mathbib/resources/journal_abbrevs.json`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/session.py` & `mathbib-0.7.9/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/mathbib/term.py` & `mathbib-0.7.9/mathbib/term.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.8/pyproject.toml` & `mathbib-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [virtualenv]
 in-project = true
 
 [tool.poetry]
 name = "mathbib"
-version = "0.7.8"
+version = "0.7.9"
 description = "A mathematics BibLaTeX bibliography manager."
 authors = ["Alex Rutar <alex@rutar.org>"]
 readme = "README.md"
 packages = [{include = "mathbib"}]
 license = "MIT"
 repository = "https://github.com/alexrutar/mathbib-py"
 include = ["mathbib/resources/journal_abbrevs.json"]
```

### Comparing `mathbib-0.7.8/PKG-INFO` & `mathbib-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.7.8
+Version: 0.7.9
 Summary: A mathematics BibLaTeX bibliography manager.
 Home-page: https://github.com/alexrutar/mathbib-py
 License: MIT
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -91,15 +91,15 @@
 \addbibresource{doc.bib}
 \begin{document}
 This document references an article \cite{Hoc2014}.
 It also contains more references \cite{HocShm2012, Shm2019}.
 \printbibliography
 \end{document}
 ```
-Remember to regenerate the `doc.bib` file with `mbib generate doc.tex > doc.bib` (the citation keys need to be updated), and the file will compile!
+Remember to regenerate the `doc.bib` file with `mbib generate doc.tex --out doc.bib` (the citation keys need to be updated), and the file will compile!
 Aliases also work as command line arguments anywhere a `key:id` is expected.
 
 Suppose you have been working on the above TEX document for a while, and now you want to cite a specific theorem from the paper `Hoc2014`.
 Simply run
 ```sh
 mbib file open Hoc2014
 ```
@@ -110,15 +110,15 @@
 Of course, if `mbib` cannot find a resource for your file, you can also add one yourself.
 ```sh
 mbib file add Hoc2014 path/to/file.pdf
 ```
 
 Finally, if you have loaded a record but there are mistakes (for instance, improperly formatted LaTeX), you can apply local modifications which will always be applied when requesting the record.
 Edit the local record with, for example,
-```
+```sh
 mbib file open zbl:1251.28008
 ```
 There are also other features implemented: either read more below, or run `mbib --help` and `mbib <subcommand> --help` for more information.
 
 
 ## Remote and local records
 Internally, whenever you request a new record, MathBib searches a few online data repositories for the information associated with the record.
```

