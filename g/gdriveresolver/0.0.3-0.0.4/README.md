# Comparing `tmp/gdriveresolver-0.0.3.tar.gz` & `tmp/gdriveresolver-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdriveresolver-0.0.3.tar", last modified: Tue May 14 21:07:59 2024, max compression
+gzip compressed data, was "gdriveresolver-0.0.4.tar", last modified: Tue May 14 21:09:11 2024, max compression
```

## Comparing `gdriveresolver-0.0.3.tar` & `gdriveresolver-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:07:59.416762 gdriveresolver-0.0.3/
--rw-r--r--   0 harman     (501) staff       (20)     1069 2024-05-14 18:58:35.000000 gdriveresolver-0.0.3/LICENSE
--rw-r--r--   0 harman     (501) staff       (20)     1603 2024-05-14 21:07:59.416607 gdriveresolver-0.0.3/PKG-INFO
--rw-r--r--   0 harman     (501) staff       (20)      992 2024-05-14 20:57:44.000000 gdriveresolver-0.0.3/README.md
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:07:59.415886 gdriveresolver-0.0.3/gdriveresolver/
--rw-r--r--   0 harman     (501) staff       (20)       42 2024-05-14 19:54:16.000000 gdriveresolver-0.0.3/gdriveresolver/__init__.py
--rw-r--r--   0 harman     (501) staff       (20)      105 2024-05-14 17:29:08.000000 gdriveresolver-0.0.3/gdriveresolver/exceptions.py
--rw-r--r--   0 harman     (501) staff       (20)     1053 2024-05-14 18:17:17.000000 gdriveresolver-0.0.3/gdriveresolver/model.py
--rw-r--r--   0 harman     (501) staff       (20)      850 2024-05-14 21:06:12.000000 gdriveresolver-0.0.3/gdriveresolver/resolver.py
--rw-r--r--   0 harman     (501) staff       (20)     2805 2024-05-14 19:26:42.000000 gdriveresolver-0.0.3/gdriveresolver/system_operations.py
-drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:07:59.416462 gdriveresolver-0.0.3/gdriveresolver.egg-info/
--rw-r--r--   0 harman     (501) staff       (20)     1603 2024-05-14 21:07:59.000000 gdriveresolver-0.0.3/gdriveresolver.egg-info/PKG-INFO
--rw-r--r--   0 harman     (501) staff       (20)      327 2024-05-14 21:07:59.000000 gdriveresolver-0.0.3/gdriveresolver.egg-info/SOURCES.txt
--rw-r--r--   0 harman     (501) staff       (20)        1 2024-05-14 21:07:59.000000 gdriveresolver-0.0.3/gdriveresolver.egg-info/dependency_links.txt
--rw-r--r--   0 harman     (501) staff       (20)       15 2024-05-14 21:07:59.000000 gdriveresolver-0.0.3/gdriveresolver.egg-info/top_level.txt
--rw-r--r--   0 harman     (501) staff       (20)      683 2024-05-14 21:04:50.000000 gdriveresolver-0.0.3/pyproject.toml
--rw-r--r--   0 harman     (501) staff       (20)       38 2024-05-14 21:07:59.416801 gdriveresolver-0.0.3/setup.cfg
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:09:11.527958 gdriveresolver-0.0.4/
+-rw-r--r--   0 harman     (501) staff       (20)     1069 2024-05-14 18:58:35.000000 gdriveresolver-0.0.4/LICENSE
+-rw-r--r--   0 harman     (501) staff       (20)     1603 2024-05-14 21:09:11.527799 gdriveresolver-0.0.4/PKG-INFO
+-rw-r--r--   0 harman     (501) staff       (20)      992 2024-05-14 20:57:44.000000 gdriveresolver-0.0.4/README.md
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:09:11.527071 gdriveresolver-0.0.4/gdriveresolver/
+-rw-r--r--   0 harman     (501) staff       (20)       42 2024-05-14 19:54:16.000000 gdriveresolver-0.0.4/gdriveresolver/__init__.py
+-rw-r--r--   0 harman     (501) staff       (20)      105 2024-05-14 17:29:08.000000 gdriveresolver-0.0.4/gdriveresolver/exceptions.py
+-rw-r--r--   0 harman     (501) staff       (20)     1053 2024-05-14 18:17:17.000000 gdriveresolver-0.0.4/gdriveresolver/model.py
+-rw-r--r--   0 harman     (501) staff       (20)      850 2024-05-14 21:06:12.000000 gdriveresolver-0.0.4/gdriveresolver/resolver.py
+-rw-r--r--   0 harman     (501) staff       (20)     2805 2024-05-14 19:26:42.000000 gdriveresolver-0.0.4/gdriveresolver/system_operations.py
+drwxr-xr-x   0 harman     (501) staff       (20)        0 2024-05-14 21:09:11.527575 gdriveresolver-0.0.4/gdriveresolver.egg-info/
+-rw-r--r--   0 harman     (501) staff       (20)     1603 2024-05-14 21:09:11.000000 gdriveresolver-0.0.4/gdriveresolver.egg-info/PKG-INFO
+-rw-r--r--   0 harman     (501) staff       (20)      327 2024-05-14 21:09:11.000000 gdriveresolver-0.0.4/gdriveresolver.egg-info/SOURCES.txt
+-rw-r--r--   0 harman     (501) staff       (20)        1 2024-05-14 21:09:11.000000 gdriveresolver-0.0.4/gdriveresolver.egg-info/dependency_links.txt
+-rw-r--r--   0 harman     (501) staff       (20)       15 2024-05-14 21:09:11.000000 gdriveresolver-0.0.4/gdriveresolver.egg-info/top_level.txt
+-rw-r--r--   0 harman     (501) staff       (20)      683 2024-05-14 21:09:04.000000 gdriveresolver-0.0.4/pyproject.toml
+-rw-r--r--   0 harman     (501) staff       (20)       38 2024-05-14 21:09:11.527994 gdriveresolver-0.0.4/setup.cfg
```

### Comparing `gdriveresolver-0.0.3/LICENSE` & `gdriveresolver-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.3/PKG-INFO` & `gdriveresolver-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdriveresolver
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location.
 Author-email: C Harman <charman@netrias.com>
 Project-URL: Homepage, https://github.com/netrias/gdrive_resolver
 Project-URL: Issues, https://github.com/netrias/gdrive_resolver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gdriveresolver-0.0.3/README.md` & `gdriveresolver-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.3/gdriveresolver/model.py` & `gdriveresolver-0.0.4/gdriveresolver/model.py`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.3/gdriveresolver/resolver.py` & `gdriveresolver-0.0.4/gdriveresolver/resolver.py`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.3/gdriveresolver/system_operations.py` & `gdriveresolver-0.0.4/gdriveresolver/system_operations.py`

 * *Files identical despite different names*

### Comparing `gdriveresolver-0.0.3/gdriveresolver.egg-info/PKG-INFO` & `gdriveresolver-0.0.4/gdriveresolver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdriveresolver
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location.
 Author-email: C Harman <charman@netrias.com>
 Project-URL: Homepage, https://github.com/netrias/gdrive_resolver
 Project-URL: Issues, https://github.com/netrias/gdrive_resolver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gdriveresolver-0.0.3/pyproject.toml` & `gdriveresolver-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gdriveresolver"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="C Harman", email="charman@netrias.com" },
 ]
 description = "A package that helps resolve relative Google Drive paths to absolute system paths that refer to the Google drive mount location."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

