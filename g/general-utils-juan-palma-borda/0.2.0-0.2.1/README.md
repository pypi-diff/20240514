# Comparing `tmp/general-utils-juan-palma-borda-0.2.0.tar.gz` & `tmp/general_utils_juan_palma_borda-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general-utils-juan-palma-borda-0.2.0.tar", last modified: Tue Oct 10 08:45:17 2023, max compression
+gzip compressed data, was "general_utils_juan_palma_borda-0.2.1.tar", last modified: Tue May 14 08:58:40 2024, max compression
```

## Comparing `general-utils-juan-palma-borda-0.2.0.tar` & `general_utils_juan_palma_borda-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 08:45:17.040118 general-utils-juan-palma-borda-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-10-10 08:45:17.040118 general-utils-juan-palma-borda-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-10-10 08:45:17.040118 general-utils-juan-palma-borda-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 08:45:17.036118 general-utils-juan-palma-borda-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 08:45:17.036118 general-utils-juan-palma-borda-0.2.0/src/general_utils_j/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/src/general_utils_j/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 08:45:17.036118 general-utils-juan-palma-borda-0.2.0/src/general_utils_j/clases_auxiliares/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/src/general_utils_j/clases_auxiliares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/src/general_utils_j/clases_auxiliares/punto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/src/general_utils_j/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 08:45:17.040118 general-utils-juan-palma-borda-0.2.0/src/general_utils_j/patrones/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/src/general_utils_j/patrones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/src/general_utils_j/patrones/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/src/general_utils_j/prints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2023-10-10 08:45:03.000000 general-utils-juan-palma-borda-0.2.0/src/general_utils_j/umaths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 08:45:17.040118 general-utils-juan-palma-borda-0.2.0/src/general_utils_juan_palma_borda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-10-10 08:45:17.000000 general-utils-juan-palma-borda-0.2.0/src/general_utils_juan_palma_borda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-10-10 08:45:17.000000 general-utils-juan-palma-borda-0.2.0/src/general_utils_juan_palma_borda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 08:45:17.000000 general-utils-juan-palma-borda-0.2.0/src/general_utils_juan_palma_borda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-10 08:45:17.000000 general-utils-juan-palma-borda-0.2.0/src/general_utils_juan_palma_borda.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:58:40.234824 general_utils_juan_palma_borda-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-14 08:58:40.230824 general_utils_juan_palma_borda-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-14 08:58:40.234824 general_utils_juan_palma_borda-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:58:40.230824 general_utils_juan_palma_borda-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:58:40.230824 general_utils_juan_palma_borda-0.2.1/src/general_utils_j/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/src/general_utils_j/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:58:40.230824 general_utils_juan_palma_borda-0.2.1/src/general_utils_j/clases_auxiliares/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/src/general_utils_j/clases_auxiliares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/src/general_utils_j/clases_auxiliares/punto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/src/general_utils_j/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:58:40.230824 general_utils_juan_palma_borda-0.2.1/src/general_utils_j/patrones/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/src/general_utils_j/patrones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/src/general_utils_j/patrones/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/src/general_utils_j/prints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-14 08:58:35.000000 general_utils_juan_palma_borda-0.2.1/src/general_utils_j/umaths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:58:40.230824 general_utils_juan_palma_borda-0.2.1/src/general_utils_juan_palma_borda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-14 08:58:40.000000 general_utils_juan_palma_borda-0.2.1/src/general_utils_juan_palma_borda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-14 08:58:40.000000 general_utils_juan_palma_borda-0.2.1/src/general_utils_juan_palma_borda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:58:40.000000 general_utils_juan_palma_borda-0.2.1/src/general_utils_juan_palma_borda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 08:58:40.000000 general_utils_juan_palma_borda-0.2.1/src/general_utils_juan_palma_borda.egg-info/top_level.txt
```

### Comparing `general-utils-juan-palma-borda-0.2.0/LICENSE` & `general_utils_juan_palma_borda-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `general-utils-juan-palma-borda-0.2.0/LICENSE.txt` & `general_utils_juan_palma_borda-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `general-utils-juan-palma-borda-0.2.0/PKG-INFO` & `general_utils_juan_palma_borda-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: general-utils-juan-palma-borda
-Version: 0.2.0
-Summary: Group of general utils from different projects
+Version: 0.2.1
+Summary: Group of general utils from different projects.
 Home-page: https://github.com/muerterauda/general-utils
 Author: Juan Palma Borda
-Author-email: juanpalmaborda@hotmail.com
-Project-URL: Bug Tracker, https://github.com/muerterauda/general-utils/issues
+Author-email: Juan Palma Borda <juanpalmaborda@hotmail.com>
+Keywords: utils,colors,prints,math_operations
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
-# General Utils (0.2.0)
+# General Utils (0.2.1)
 
 Group of general utils from different projects.
 
 Included classes:
 
 - Point class
 - Singleton pattern
```

### Comparing `general-utils-juan-palma-borda-0.2.0/setup.cfg` & `general_utils_juan_palma_borda-0.2.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = general-utils-juan-palma-borda
-version = 0.2.0
+version = 0.2.1
 author = Juan Palma Borda
 author_email = juanpalmaborda@hotmail.com
 description = Group of general utils from different projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/muerterauda/general-utils
 project_urls =
```

### Comparing `general-utils-juan-palma-borda-0.2.0/setup.py` & `general_utils_juan_palma_borda-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="general-utils-juan-palma-borda",
-    version="0.2.0",
+    version="0.2.1",
     author='Juan Palma Borda',
     author_email='juanpalmaborda@hotmail.com',
     description='Group of general utils from different projects',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/muerterauda/general-utils",
     project_urls={
```

### Comparing `general-utils-juan-palma-borda-0.2.0/src/general_utils_j/clases_auxiliares/punto.py` & `general_utils_juan_palma_borda-0.2.1/src/general_utils_j/clases_auxiliares/punto.py`

 * *Files identical despite different names*

### Comparing `general-utils-juan-palma-borda-0.2.0/src/general_utils_j/colors.py` & `general_utils_juan_palma_borda-0.2.1/src/general_utils_j/colors.py`

 * *Files identical despite different names*

### Comparing `general-utils-juan-palma-borda-0.2.0/src/general_utils_j/umaths.py` & `general_utils_juan_palma_borda-0.2.1/src/general_utils_j/umaths.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     if x > in_max:
         if not raise_error:
             return returned_no_error_max
         raise Exception('Valor no incluido')
     return (x - in_min) * (out_max - out_min) / (in_max - in_min) + out_min
 
 
+def map_value_no_bounds(x, in_min, in_max, out_min, out_max):
+    return (x - in_min) * (out_max - out_min) / (in_max - in_min) + out_min
+
+
 class Incremental_math_operations:
 
     @staticmethod
     def media_incremental_adicion(media_original, longitud_original, nuevo_valor):
         return (media_original * longitud_original + nuevo_valor) / (longitud_original + 1)
 
     @staticmethod
```

### Comparing `general-utils-juan-palma-borda-0.2.0/src/general_utils_juan_palma_borda.egg-info/PKG-INFO` & `general_utils_juan_palma_borda-0.2.1/src/general_utils_juan_palma_borda.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: general-utils-juan-palma-borda
-Version: 0.2.0
-Summary: Group of general utils from different projects
+Version: 0.2.1
+Summary: Group of general utils from different projects.
 Home-page: https://github.com/muerterauda/general-utils
 Author: Juan Palma Borda
-Author-email: juanpalmaborda@hotmail.com
-Project-URL: Bug Tracker, https://github.com/muerterauda/general-utils/issues
+Author-email: Juan Palma Borda <juanpalmaborda@hotmail.com>
+Keywords: utils,colors,prints,math_operations
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
-# General Utils (0.2.0)
+# General Utils (0.2.1)
 
 Group of general utils from different projects.
 
 Included classes:
 
 - Point class
 - Singleton pattern
```

### Comparing `general-utils-juan-palma-borda-0.2.0/src/general_utils_juan_palma_borda.egg-info/SOURCES.txt` & `general_utils_juan_palma_borda-0.2.1/src/general_utils_juan_palma_borda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

