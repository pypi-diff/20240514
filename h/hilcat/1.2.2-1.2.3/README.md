# Comparing `tmp/hilcat-1.2.2.tar.gz` & `tmp/hilcat-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilcat-1.2.2.tar", last modified: Sun May 12 06:14:47 2024, max compression
+gzip compressed data, was "hilcat-1.2.3.tar", last modified: Tue May 14 09:54:42 2024, max compression
```

## Comparing `hilcat-1.2.2.tar` & `hilcat-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:47.194262 hilcat-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-12 06:14:47.194262 hilcat-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-12 06:14:34.000000 hilcat-1.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:47.190262 hilcat-1.2.2/hilcat/
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-12 06:14:47.000000 hilcat-1.2.2/hilcat/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:47.194262 hilcat-1.2.2/hilcat/db/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/db/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/db/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    38320 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/db/relational.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/db/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/es.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:47.194262 hilcat-1.2.2/hilcat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-12 06:14:47.000000 hilcat-1.2.2/hilcat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-12 06:14:47.000000 hilcat-1.2.2/hilcat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:14:47.000000 hilcat-1.2.2/hilcat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-12 06:14:34.000000 hilcat-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 06:14:47.194262 hilcat-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:54:42.458405 hilcat-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-14 09:54:42.458405 hilcat-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-14 09:54:34.000000 hilcat-1.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:54:42.458405 hilcat-1.2.3/hilcat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-14 09:54:34.000000 hilcat-1.2.3/hilcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-14 09:54:42.000000 hilcat-1.2.3/hilcat/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-05-14 09:54:34.000000 hilcat-1.2.3/hilcat/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:54:42.458405 hilcat-1.2.3/hilcat/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-14 09:54:34.000000 hilcat-1.2.3/hilcat/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-14 09:54:34.000000 hilcat-1.2.3/hilcat/db/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-14 09:54:34.000000 hilcat-1.2.3/hilcat/db/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39496 2024-05-14 09:54:34.000000 hilcat-1.2.3/hilcat/db/relational.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-14 09:54:34.000000 hilcat-1.2.3/hilcat/db/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-14 09:54:34.000000 hilcat-1.2.3/hilcat/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-14 09:54:34.000000 hilcat-1.2.3/hilcat/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-14 09:54:34.000000 hilcat-1.2.3/hilcat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:54:42.458405 hilcat-1.2.3/hilcat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-14 09:54:42.000000 hilcat-1.2.3/hilcat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-14 09:54:42.000000 hilcat-1.2.3/hilcat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:54:42.000000 hilcat-1.2.3/hilcat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-14 09:54:34.000000 hilcat-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:54:42.458405 hilcat-1.2.3/setup.cfg
```

### Comparing `hilcat-1.2.2/PKG-INFO` & `hilcat-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilcat
-Version: 1.2.2
+Version: 1.2.3
 Summary: High Level Cache Tool.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/hilcat
 Description-Content-Type: text/x-rst
 
 ==========
 HiLCaT
```

### Comparing `hilcat-1.2.2/README.rst` & `hilcat-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.2/hilcat/__init__.py` & `hilcat-1.2.3/hilcat/__init__.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.2/hilcat/core.py` & `hilcat-1.2.3/hilcat/core.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.2/hilcat/db/__init__.py` & `hilcat-1.2.3/hilcat/db/__init__.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.2/hilcat/db/mysql.py` & `hilcat-1.2.3/hilcat/db/mysql.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.2/hilcat/db/postgresql.py` & `hilcat-1.2.3/hilcat/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.2/hilcat/db/relational.py` & `hilcat-1.2.3/hilcat/db/relational.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
 Relational database can be used as a cache or a persistence storage.
 Actually, implement a cache is enough.
 """
 
+import json
 import collections
 from typing import (
     Any, Iterable, Dict,
     List, Type, Optional,
     Sequence, Callable,
     Literal, Union,
     Tuple, Hashable,
@@ -67,14 +68,45 @@
 
     def build_column_values(self, value: Any) -> Dict[str, Any]:
         return {self.col: value}
 
     def parse_column_values(self, value: Dict[str, Any]) -> Any:
         return value[self.col]
 
+class SingleJsonValueAdapter(SingleAdapter):
+    """
+    Cache value is stored in one column, and can be a complex type
+      such as dict or list, type in db is text in json format.
+    """
+    def __init__(self, col: str, ensure_ascii=True):
+        super().__init__(col)
+        self.ensure_ascii = ensure_ascii
+
+    def build_column_values(self, value: Dict[str, Any]) -> Dict[str, Any]:
+        value = json.dumps(value, ensure_ascii=self.ensure_ascii)
+        return super().build_column_values(value)
+
+    def parse_column_values(self, value: Dict[str, Any]) -> Any:
+        s = super().parse_column_values(value)
+        return json.loads(s)
+
+class JsonValueAdapter(ValueAdapter):
+    """
+    All value type in db should be text.
+    """
+    def __init__(self, ensure_ascii=True):
+        super().__init__()
+        self.ensure_ascii = ensure_ascii
+
+    def build_column_values(self, value: Dict[str, Any]) -> Dict[str, Any]:
+        return {k: json.dumps(v, ensure_ascii=self.ensure_ascii) for k, v in value.items()}
+
+    def parse_column_values(self, value: Dict[str, Any]) -> Dict[str, Any]:
+        return {k: json.loads(v) for k, v in value.items()}
+
 class SequenceAdapter(ValueAdapter):
     """
     Cache value is a list or tuple, corresponding to some columns.
     """
 
     def __init__(self, cols: Sequence[str], return_type: Type[Union[list, tuple]] = tuple):
         self.cols = cols
```

### Comparing `hilcat-1.2.2/hilcat/db/sqlite.py` & `hilcat-1.2.3/hilcat/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.2/hilcat/es.py` & `hilcat-1.2.3/hilcat/es.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.2/hilcat/redis.py` & `hilcat-1.2.3/hilcat/redis.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.2/hilcat.egg-info/PKG-INFO` & `hilcat-1.2.3/hilcat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilcat
-Version: 1.2.2
+Version: 1.2.3
 Summary: High Level Cache Tool.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/hilcat
 Description-Content-Type: text/x-rst
 
 ==========
 HiLCaT
```

### Comparing `hilcat-1.2.2/pyproject.toml` & `hilcat-1.2.3/pyproject.toml`

 * *Files identical despite different names*

