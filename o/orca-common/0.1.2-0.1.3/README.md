# Comparing `tmp/orca_common-0.1.2.tar.gz` & `tmp/orca_common-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orca_common-0.1.2.tar", max compression
+gzip compressed data, was "orca_common-0.1.3.tar", max compression
```

## Comparing `orca_common-0.1.2.tar` & `orca_common-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      309 2024-03-25 19:18:00.404798 orca_common-0.1.2/README.md
--rw-r--r--   0        0        0      247 2024-03-25 19:18:00.404798 orca_common-0.1.2/orca_common/__init__.py
--rw-r--r--   0        0        0     1034 2024-03-25 19:18:00.404798 orca_common-0.1.2/orca_common/api_types.py
--rw-r--r--   0        0        0      264 2024-03-25 19:18:00.404798 orca_common-0.1.2/orca_common/embedding_models.py
--rw-r--r--   0        0        0     2528 2024-03-25 19:18:00.404798 orca_common-0.1.2/orca_common/numeric_type.py
--rw-r--r--   0        0        0      595 2024-03-25 19:18:00.404798 orca_common-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 orca_common-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      309 2024-05-14 15:51:50.514790 orca_common-0.1.3/README.md
+-rw-r--r--   0        0        0      247 2024-05-14 15:51:50.514790 orca_common-0.1.3/orca_common/__init__.py
+-rw-r--r--   0        0        0     1310 2024-05-14 15:51:50.514790 orca_common-0.1.3/orca_common/api_types.py
+-rw-r--r--   0        0        0      264 2024-05-14 15:51:50.514790 orca_common-0.1.3/orca_common/embedding_models.py
+-rw-r--r--   0        0        0     2528 2024-05-14 15:51:50.514790 orca_common-0.1.3/orca_common/numeric_type.py
+-rw-r--r--   0        0        0      595 2024-05-14 15:51:50.514790 orca_common-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 orca_common-0.1.3/PKG-INFO
```

### Comparing `orca_common-0.1.2/orca_common/api_types.py` & `orca_common-0.1.3/orca_common/api_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,11 +27,25 @@
     JPEG = "JPEG"
     PNG = "PNG"
     TIFF = "TIFF"
     GIF = "GIF"
     BMP = "BMP"
 
 
+class OperationEnum(str, Enum):
+    NOT = "$!"
+    AND = "$&"
+    OR = "$|"
+    GREATER_THAN = "$GT"
+    LESS_THAN = "$LT"
+    GREATER_THAN_OR_EQUAL = "$GTE"
+    LESS_THAN_OR_EQUAL = "$LTE"
+    EQUAL = "$EQ"
+    NOT_EQUAL = "$NEQ"
+    LIKE = "$LIKE"
+    NOT_LIKE = "$NLIKE"
+
+
 ColumnName = str
 TableName = str
 RowDict = dict[ColumnName, Any]
 OrderByColumns = ColumnName | tuple[ColumnName, Order] | list[ColumnName | tuple[ColumnName, Order]]
```

### Comparing `orca_common-0.1.2/orca_common/numeric_type.py` & `orca_common-0.1.3/orca_common/numeric_type.py`

 * *Files identical despite different names*

### Comparing `orca_common-0.1.2/pyproject.toml` & `orca_common-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orca_common"
-version = "0.1.2"
+version = "0.1.3"
 description = "Shared objects for manifold and orcalib"
 authors = ["Orca DB Inc. <dev-rel@orcadb.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.24"
```

### Comparing `orca_common-0.1.2/PKG-INFO` & `orca_common-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orca_common
-Version: 0.1.2
+Version: 0.1.3
 Summary: Shared objects for manifold and orcalib
 Author: Orca DB Inc.
 Author-email: dev-rel@orcadb.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

