# Comparing `tmp/sniffs-0.5.4.tar.gz` & `tmp/sniffs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffs-0.5.4.tar", max compression
+gzip compressed data, was "sniffs-0.6.0.tar", max compression
```

## Comparing `sniffs-0.5.4.tar` & `sniffs-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-05-06 16:08:40.397256 sniffs-0.5.4/LICENSE
--rw-r--r--   0        0        0     3452 2024-05-06 16:08:40.397256 sniffs-0.5.4/README.md
--rw-r--r--   0        0        0      368 2024-05-06 16:58:06.987597 sniffs-0.5.4/pyproject.toml
--rw-r--r--   0        0        0       66 2024-05-06 16:08:40.397256 sniffs-0.5.4/sniffs/__init__.py
--rw-r--r--   0        0        0     4729 2024-05-06 16:08:40.397256 sniffs-0.5.4/sniffs/router.py
--rw-r--r--   0        0        0     1306 2024-05-06 16:08:40.397256 sniffs-0.5.4/sniffs/sniffs.py
--rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 sniffs-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-06 16:08:40.397256 sniffs-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3452 2024-05-06 16:08:40.397256 sniffs-0.6.0/README.md
+-rw-r--r--   0        0        0      367 2024-05-14 16:13:06.634552 sniffs-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2024-05-06 16:08:40.397256 sniffs-0.6.0/sniffs/__init__.py
+-rw-r--r--   0        0        0     4729 2024-05-06 16:08:40.397256 sniffs-0.6.0/sniffs/router.py
+-rw-r--r--   0        0        0     1306 2024-05-06 16:08:40.397256 sniffs-0.6.0/sniffs/sniffs.py
+-rw-r--r--   0        0        0     3867 1970-01-01 00:00:00.000000 sniffs-0.6.0/PKG-INFO
```

### Comparing `sniffs-0.5.4/LICENSE` & `sniffs-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sniffs-0.5.4/README.md` & `sniffs-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sniffs-0.5.4/sniffs/router.py` & `sniffs-0.6.0/sniffs/router.py`

 * *Files identical despite different names*

### Comparing `sniffs-0.5.4/sniffs/sniffs.py` & `sniffs-0.6.0/sniffs/sniffs.py`

 * *Files identical despite different names*

### Comparing `sniffs-0.5.4/PKG-INFO` & `sniffs-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sniffs
-Version: 0.5.4
+Version: 0.6.0
 Summary: 
 Author: surdouski
 Author-email: michael.surdouski@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: paho-mqtt (>=2.0.0,<3.0.0)
+Requires-Dist: paho-mqtt (==1.6.1)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Description-Content-Type: text/markdown
 
 # Sniffs - Python MQTT Router
 
 Sniffs is a lightweight Python package for routing MQTT messages using flexible topic patterns. It provides an easy-to-use interface for defining routes and handling incoming messages efficiently.
```

