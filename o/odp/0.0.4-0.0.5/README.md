# Comparing `tmp/odp-0.0.4.tar.gz` & `tmp/odp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odp-0.0.4.tar", max compression
+gzip compressed data, was "odp-0.0.5.tar", max compression
```

## Comparing `odp-0.0.4.tar` & `odp-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      582 2024-05-14 17:57:09.247221 odp-0.0.4/LICENSE
--rw-r--r--   0        0        0     2002 2024-05-14 17:57:09.841762 odp-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-05-13 16:35:32.352855 odp-0.0.4/odp/__init__.py
--rw-r--r--   0        0        0       67 2024-05-14 17:57:09.253889 odp-0.0.4/odp/__main__.py
--rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353425 odp-0.0.4/odp/cli/__init__.py
--rw-r--r--   0        0        0     4049 2024-05-14 18:09:06.165941 odp-0.0.4/odp/cli/main.py
--rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353850 odp-0.0.4/odp/core/__init__.py
--rw-r--r--   0        0        0     5525 2024-05-14 17:57:09.692111 odp-0.0.4/odp/core/detect_unused.py
--rw-r--r--   0        0        0     2770 2024-05-14 17:57:09.691865 odp-0.0.4/odp/core/snowflake.py
--rw-r--r--   0        0        0      994 2024-05-14 18:10:28.564415 odp-0.0.4/odp/core/types.py
--rw-r--r--   0        0        0     2042 2024-05-14 18:15:24.511245 odp-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2906 1970-01-01 00:00:00.000000 odp-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      582 2024-05-14 17:57:09.247221 odp-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2002 2024-05-14 17:57:09.841762 odp-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 16:35:32.352855 odp-0.0.5/odp/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-14 17:57:09.253889 odp-0.0.5/odp/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353425 odp-0.0.5/odp/cli/__init__.py
+-rw-r--r--   0        0        0     4049 2024-05-14 18:09:06.165941 odp-0.0.5/odp/cli/main.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353850 odp-0.0.5/odp/core/__init__.py
+-rw-r--r--   0        0        0     5525 2024-05-14 17:57:09.692111 odp-0.0.5/odp/core/detect_unused.py
+-rw-r--r--   0        0        0     2770 2024-05-14 17:57:09.691865 odp-0.0.5/odp/core/snowflake.py
+-rw-r--r--   0        0        0      994 2024-05-14 18:10:28.564415 odp-0.0.5/odp/core/types.py
+-rw-r--r--   0        0        0     2046 2024-05-14 18:19:32.316378 odp-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2906 1970-01-01 00:00:00.000000 odp-0.0.5/PKG-INFO
```

### Comparing `odp-0.0.4/LICENSE` & `odp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `odp-0.0.4/README.md` & `odp-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `odp-0.0.4/odp/cli/main.py` & `odp-0.0.5/odp/cli/main.py`

 * *Files identical despite different names*

### Comparing `odp-0.0.4/odp/core/detect_unused.py` & `odp-0.0.5/odp/core/detect_unused.py`

 * *Files identical despite different names*

### Comparing `odp-0.0.4/odp/core/snowflake.py` & `odp-0.0.5/odp/core/snowflake.py`

 * *Files identical despite different names*

### Comparing `odp-0.0.4/odp/core/types.py` & `odp-0.0.5/odp/core/types.py`

 * *Files identical despite different names*

### Comparing `odp-0.0.4/pyproject.toml` & `odp-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odp"
-version = "0.0.4"
+version = "0.0.5"
 description = "odp"
 authors = ["odp Authors <fdexter@metalytics.dev>"]
 repository = "https://github.com/open-data-products/odp"
 documentation = "https://open-data-products.github.io/odp/"
 readme = "README.md"
 packages = [
   {include = "odp"}
@@ -15,15 +15,15 @@
 sqlglot = "^23.0.5"
 click = "^8.1.7"
 snowflake-connector-python = "^3.7.1"
 python-dotenv = "^1.0.1"
 pydantic = "^2.7.1"
 
 [tool.poetry.scripts]
-odp = "odp.cli:main"
+odp = "odp.cli.main:cli"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.12.0"
 mypy = "^1.5.1"
 pre-commit = "^3.4.0"
```

### Comparing `odp-0.0.4/PKG-INFO` & `odp-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odp
-Version: 0.0.4
+Version: 0.0.5
 Summary: odp
 Home-page: https://github.com/open-data-products/odp
 Author: odp Authors
 Author-email: fdexter@metalytics.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

