# Comparing `tmp/aistrings-0.1.0.tar.gz` & `tmp/aistrings-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aistrings-0.1.0.tar", max compression
+gzip compressed data, was "aistrings-0.1.1.tar", max compression
```

## Comparing `aistrings-0.1.0.tar` & `aistrings-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1075 2024-05-14 12:02:20.808856 aistrings-0.1.0/LICENSE
--rw-r--r--   0        0        0     4122 2024-05-14 16:46:08.409320 aistrings-0.1.0/README.md
--rw-r--r--   0        0        0       19 2024-05-14 08:52:15.123778 aistrings-0.1.0/aistrings/__init__.py
--rw-r--r--   0        0        0     4098 2024-05-14 16:46:30.723006 aistrings-0.1.0/aistrings/main.py
--rw-r--r--   0        0        0        0 2024-05-14 08:32:15.520265 aistrings-0.1.0/aistrings/models/__init__.py
--rw-r--r--   0        0        0      249 2024-05-14 16:46:08.412076 aistrings-0.1.0/aistrings/models/base.py
--rw-r--r--   0        0        0     1584 2024-05-14 13:09:36.359742 aistrings-0.1.0/aistrings/models/openai.py
--rw-r--r--   0        0        0      386 2024-05-14 08:31:06.894823 aistrings-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4769 1970-01-01 00:00:00.000000 aistrings-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-14 12:02:20.808856 aistrings-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4122 2024-05-14 16:46:08.409320 aistrings-0.1.1/README.md
+-rw-r--r--   0        0        0       27 2024-05-14 19:46:37.063145 aistrings-0.1.1/aistrings/__init__.py
+-rw-r--r--   0        0        0     4098 2024-05-14 16:46:30.723006 aistrings-0.1.1/aistrings/main.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:32:15.520265 aistrings-0.1.1/aistrings/models/__init__.py
+-rw-r--r--   0        0        0      249 2024-05-14 16:46:08.412076 aistrings-0.1.1/aistrings/models/base.py
+-rw-r--r--   0        0        0     1584 2024-05-14 13:09:36.359742 aistrings-0.1.1/aistrings/models/openai.py
+-rw-r--r--   0        0        0      386 2024-05-14 19:46:55.569591 aistrings-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4769 1970-01-01 00:00:00.000000 aistrings-0.1.1/PKG-INFO
```

### Comparing `aistrings-0.1.0/LICENSE` & `aistrings-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aistrings-0.1.0/README.md` & `aistrings-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aistrings-0.1.0/aistrings/main.py` & `aistrings-0.1.1/aistrings/main.py`

 * *Files identical despite different names*

### Comparing `aistrings-0.1.0/aistrings/models/openai.py` & `aistrings-0.1.1/aistrings/models/openai.py`

 * *Files identical despite different names*

### Comparing `aistrings-0.1.0/PKG-INFO` & `aistrings-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistrings
-Version: 0.1.0
+Version: 0.1.1
 Summary: An API to manipulate strings semantically.
 License: MIT
 Author: roncaglionidaniele
 Author-email: roncaglionidaniele@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

