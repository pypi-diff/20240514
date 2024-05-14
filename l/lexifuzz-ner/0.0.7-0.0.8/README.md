# Comparing `tmp/lexifuzz_ner-0.0.7.tar.gz` & `tmp/lexifuzz_ner-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexifuzz_ner-0.0.7.tar", max compression
+gzip compressed data, was "lexifuzz_ner-0.0.8.tar", max compression
```

## Comparing `lexifuzz_ner-0.0.7.tar` & `lexifuzz_ner-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1097 2023-09-12 04:08:59.142483 lexifuzz_ner-0.0.7/LICENSE
--rwxr-xr-x   0        0        0     2993 2024-04-17 10:22:18.366558 lexifuzz_ner-0.0.7/README.md
--rwxr-xr-x   0        0        0      640 2024-04-17 12:17:26.305562 lexifuzz_ner-0.0.7/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-09-12 04:29:12.919915 lexifuzz_ner-0.0.7/src/lexifuzz_ner/__init__.py
--rwxr-xr-x   0        0        0     6799 2024-04-17 12:16:55.949064 lexifuzz_ner-0.0.7/src/lexifuzz_ner/ner.py
--rw-r--r--   0        0        0     3718 1970-01-01 00:00:00.000000 lexifuzz_ner-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1097 2023-09-12 04:08:59.142483 lexifuzz_ner-0.0.8/LICENSE
+-rwxr-xr-x   0        0        0     2993 2024-04-17 10:22:18.366558 lexifuzz_ner-0.0.8/README.md
+-rwxr-xr-x   0        0        0      775 2024-05-14 06:51:42.793350 lexifuzz_ner-0.0.8/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-09-12 04:29:12.919915 lexifuzz_ner-0.0.8/src/lexifuzz_ner/__init__.py
+-rwxr-xr-x   0        0        0     6799 2024-04-17 12:16:55.949064 lexifuzz_ner-0.0.8/src/lexifuzz_ner/ner.py
+-rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 lexifuzz_ner-0.0.8/PKG-INFO
```

### Comparing `lexifuzz_ner-0.0.7/LICENSE` & `lexifuzz_ner-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lexifuzz_ner-0.0.7/README.md` & `lexifuzz_ner-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lexifuzz_ner-0.0.7/pyproject.toml` & `lexifuzz_ner-0.0.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "lexifuzz-ner"
-version = "0.0.7"
+version = "0.0.8"
 authors = ["Hanif Yuli Abdillah P <hanifabd23@gmail.com>"]
+repository = "https://github.com/hanifabd/lexifuzz-ner"
+keywords = ["ktp", "segmentation", "segmentasi", "id-card", "identity-card"]
 description = "Python package for detecting entities in text based on a dictionary and fuzzy similarity"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `lexifuzz_ner-0.0.7/src/lexifuzz_ner/ner.py` & `lexifuzz_ner-0.0.8/src/lexifuzz_ner/ner.py`

 * *Files identical despite different names*

### Comparing `lexifuzz_ner-0.0.7/PKG-INFO` & `lexifuzz_ner-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: lexifuzz-ner
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python package for detecting entities in text based on a dictionary and fuzzy similarity
+Home-page: https://github.com/hanifabd/lexifuzz-ner
+Keywords: ktp,segmentation,segmentasi,id-card,identity-card
 Author: Hanif Yuli Abdillah P
 Author-email: hanifabd23@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: nltk (==3.8.1)
 Requires-Dist: thefuzz (==0.20.0)
+Project-URL: Repository, https://github.com/hanifabd/lexifuzz-ner
 Description-Content-Type: text/markdown
 
 # **LexiFuzz NER: Named Entity Recognition Based on Dictionary and Fuzzy Matching**
 
 ![Image](https://github.com/hanifabd/lexifuzz-ner/blob/master/assets/lexifuzz-mascot.png)
 
 ## **About**
```

