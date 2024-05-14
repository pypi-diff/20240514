# Comparing `tmp/pyutilkit-0.2.0.tar.gz` & `tmp/pyutilkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutilkit-0.2.0.tar", max compression
+gzip compressed data, was "pyutilkit-0.3.0.tar", max compression
```

## Comparing `pyutilkit-0.2.0.tar` & `pyutilkit-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7696 2024-05-12 17:26:27.967790 pyutilkit-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     1477 2024-05-12 17:26:27.967790 pyutilkit-0.2.0/docs/README.md
--rw-r--r--   0        0        0     2994 2024-05-13 16:52:54.889471 pyutilkit-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-13 16:53:00.422686 pyutilkit-0.2.0/src/pyutilkit/__init__.py
--rw-r--r--   0        0        0      462 2024-05-12 17:26:28.511050 pyutilkit-0.2.0/src/pyutilkit/classes.py
--rw-r--r--   0        0        0        0 2024-05-12 17:26:28.644365 pyutilkit-0.2.0/src/pyutilkit/data/__init__.py
--rw-r--r--   0        0        0     3866 2024-05-12 17:26:28.644365 pyutilkit-0.2.0/src/pyutilkit/data/timezones.py
--rw-r--r--   0        0        0     1821 2024-05-12 17:26:28.644365 pyutilkit-0.2.0/src/pyutilkit/date_utils.py
--rw-r--r--   0        0        0     1523 2024-05-13 16:50:53.492051 pyutilkit-0.2.0/src/pyutilkit/files.py
--rw-r--r--   0        0        0        0 2024-05-12 17:26:27.967790 pyutilkit-0.2.0/src/pyutilkit/py.typed
--rw-r--r--   0        0        0     2895 2024-05-13 16:50:11.949600 pyutilkit-0.2.0/src/pyutilkit/term.py
--rw-r--r--   0        0        0     1073 2024-05-12 17:26:28.377734 pyutilkit-0.2.0/src/pyutilkit/timing.py
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 pyutilkit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7696 2024-05-12 17:26:27.967790 pyutilkit-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     1836 2024-05-13 21:39:43.972463 pyutilkit-0.3.0/docs/README.md
+-rw-r--r--   0        0        0     2994 2024-05-14 09:13:56.737771 pyutilkit-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 09:14:05.144163 pyutilkit-0.3.0/src/pyutilkit/__init__.py
+-rw-r--r--   0        0        0      462 2024-05-12 17:26:28.511050 pyutilkit-0.3.0/src/pyutilkit/classes.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:26:28.644365 pyutilkit-0.3.0/src/pyutilkit/data/__init__.py
+-rw-r--r--   0        0        0     3866 2024-05-12 17:26:28.644365 pyutilkit-0.3.0/src/pyutilkit/data/timezones.py
+-rw-r--r--   0        0        0     1820 2024-05-13 21:39:32.392717 pyutilkit-0.3.0/src/pyutilkit/date_utils.py
+-rw-r--r--   0        0        0     1523 2024-05-13 16:50:53.492051 pyutilkit-0.3.0/src/pyutilkit/files.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:26:27.967790 pyutilkit-0.3.0/src/pyutilkit/py.typed
+-rw-r--r--   0        0        0     2895 2024-05-13 16:50:11.949600 pyutilkit-0.3.0/src/pyutilkit/term.py
+-rw-r--r--   0        0        0     1838 2024-05-13 21:39:48.282369 pyutilkit-0.3.0/src/pyutilkit/timing.py
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 pyutilkit-0.3.0/PKG-INFO
```

### Comparing `pyutilkit-0.2.0/LICENSE.md` & `pyutilkit-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.2.0/pyproject.toml` & `pyutilkit-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "poetry_core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 target-version = [
-    "py38",
+    "py39",
 ]
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
@@ -28,15 +28,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 
 [tool.ruff]
 src = [
     "src",
 ]
-target-version = "py38"
+target-version = "py39"
 
 [tool.ruff.lint]
 select = [
     "A",
     "ARG",
     "ASYNC",
     "B",
@@ -122,15 +122,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "pyutilkit"
-version = "0.2.0"
+version = "0.3.0"
 description = "python's missing batteries"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "docs/README.md"
@@ -145,15 +145,15 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 # python version
-python = "^3.8"
+python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = { version = "^0.13", python = "^3.10" }
 ipython = { version = "^8.21", python = "^3.10" }
 pickleshare = { version = "^0.7", python = "^3.10" }
 pipdeptree = "^2.13"
```

### Comparing `pyutilkit-0.2.0/src/pyutilkit/data/timezones.py` & `pyutilkit-0.3.0/src/pyutilkit/data/timezones.py`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.2.0/src/pyutilkit/date_utils.py` & `pyutilkit-0.3.0/src/pyutilkit/date_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from datetime import datetime, tzinfo
-
 from zoneinfo import ZoneInfo, available_timezones
 
 from pyutilkit.data.timezones import UNAVAILABLE_TIMEZONES
 
 UTC = ZoneInfo("UTC")
```

### Comparing `pyutilkit-0.2.0/src/pyutilkit/files.py` & `pyutilkit-0.3.0/src/pyutilkit/files.py`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.2.0/src/pyutilkit/term.py` & `pyutilkit-0.3.0/src/pyutilkit/term.py`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.2.0/PKG-INFO` & `pyutilkit-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pyutilkit
-Version: 0.2.0
+Version: 0.3.0
 Summary: python's missing batteries
 Home-page: https://pyutilkit.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: utils
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Documentation, https://pyutilkit.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/spapanik/pyutilkit
 Description-Content-Type: text/markdown
@@ -27,15 +26,19 @@
 [![license][licence_badge]][licence_url]
 [![pypi][pypi_badge]][pypi_url]
 [![downloads][pepy_badge]][pepy_url]
 [![code style: black][black_badge]][black_url]
 [![build automation: yam][yam_badge]][yam_url]
 [![Lint: ruff][ruff_badge]][ruff_url]
 
-Long project description and tldr goes here
+The Python has long maintained the philosophy of "batteries included", giving the user
+a rich standard library, avoiding the need for third party tools for most work. Some packages
+are so common, that the have a similar status to the standard library. Still, some code seems
+to be written time and again, with every project. This small library, with minimal requirements,
+hopes to stop this repetition.
 
 ## Links
 
 -   [Documentation]
 -   [Changelog]
 
 [test_badge]: https://github.com/spapanik/pyutilkit/actions/workflows/tests.yml/badge.svg
```

