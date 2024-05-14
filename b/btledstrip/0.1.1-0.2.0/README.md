# Comparing `tmp/btledstrip-0.1.1.tar.gz` & `tmp/btledstrip-0.2.0.tar.gz`

## Comparing `btledstrip-0.1.1.tar` & `btledstrip-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 btledstrip-0.1.1/.editorconfig
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 btledstrip-0.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 btledstrip-0.1.1/.tool-versions
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 btledstrip-0.1.1/Makefile
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 btledstrip-0.1.1/Pipfile
--rw-r--r--   0        0        0    31069 2020-02-02 00:00:00.000000 btledstrip-0.1.1/Pipfile.lock
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 btledstrip-0.1.1/requirements.txt
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 btledstrip-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 btledstrip-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 btledstrip-0.1.1/btledstrip/__init__.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 btledstrip-0.1.1/btledstrip/controllers.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 btledstrip-0.1.1/btledstrip/dev.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 btledstrip-0.1.1/btledstrip/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 btledstrip-0.1.1/btledstrip/demonstrations/__init__.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 btledstrip-0.1.1/btledstrip/demonstrations/melk.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 btledstrip-0.1.1/docs/conf.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 btledstrip-0.1.1/docs/index.rst
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 btledstrip-0.1.1/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 btledstrip-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 btledstrip-0.1.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 btledstrip-0.1.1/LICENSE
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 btledstrip-0.1.1/README.md
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 btledstrip-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 btledstrip-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 btledstrip-0.2.0/.editorconfig
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 btledstrip-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 btledstrip-0.2.0/.tool-versions
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 btledstrip-0.2.0/Makefile
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 btledstrip-0.2.0/Pipfile
+-rw-r--r--   0        0        0    31069 2020-02-02 00:00:00.000000 btledstrip-0.2.0/Pipfile.lock
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 btledstrip-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 btledstrip-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 btledstrip-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 btledstrip-0.2.0/btledstrip/__init__.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 btledstrip-0.2.0/btledstrip/__init__.pyi
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 btledstrip-0.2.0/btledstrip/controllers.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 btledstrip-0.2.0/btledstrip/dev.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 btledstrip-0.2.0/btledstrip/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 btledstrip-0.2.0/btledstrip/demonstrations/__init__.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 btledstrip-0.2.0/btledstrip/demonstrations/melk.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 btledstrip-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 btledstrip-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 btledstrip-0.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 btledstrip-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 btledstrip-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 btledstrip-0.2.0/LICENSE
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 btledstrip-0.2.0/README.md
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 btledstrip-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 btledstrip-0.2.0/PKG-INFO
```

### Comparing `btledstrip-0.1.1/Makefile` & `btledstrip-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.1/Pipfile.lock` & `btledstrip-0.2.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.1/.github/workflows/python-publish.yml` & `btledstrip-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.1/btledstrip/__init__.py` & `btledstrip-0.2.0/btledstrip/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,8 +119,8 @@
 __all__ = [
     "BTLedStrip",
     "Controller",
     "MELKController",
     "Command",
 ]
 
-VERSION = "0.1.1"
+VERSION = "0.2.0"
```

### Comparing `btledstrip-0.1.1/btledstrip/controllers.py` & `btledstrip-0.2.0/btledstrip/controllers.py`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.1/btledstrip/dev.py` & `btledstrip-0.2.0/btledstrip/dev.py`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.1/btledstrip/demonstrations/melk.py` & `btledstrip-0.2.0/btledstrip/demonstrations/melk.py`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.1/docs/index.rst` & `btledstrip-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.1/.gitignore` & `btledstrip-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.1/LICENSE` & `btledstrip-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.1/pyproject.toml` & `btledstrip-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btledstrip"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
     { name="Douglas Paz", email="eu@douglaspaz.com" },
 ]
 description = "Python LED Strip Bluetooth Controller API"
 readme = "README.md"
 requires-python = ">=3.12"
 dependencies = [
```

### Comparing `btledstrip-0.1.1/PKG-INFO` & `btledstrip-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: btledstrip
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python LED Strip Bluetooth Controller API
 Project-URL: Homepage, https://github.com/dougppaz/python-bt-led-strip
 Project-URL: Documentation, https://python-bt-led-strip.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/dougppaz/python-bt-led-strip/issues
 Author-email: Douglas Paz <eu@douglaspaz.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

