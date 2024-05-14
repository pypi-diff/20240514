# Comparing `tmp/g3visu-0.1.7.tar.gz` & `tmp/g3visu-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3visu-0.1.7.tar", last modified: Fri May 10 10:14:57 2024, max compression
+gzip compressed data, was "g3visu-0.1.8.tar", last modified: Tue May 14 08:26:20 2024, max compression
```

## Comparing `g3visu-0.1.7.tar` & `g3visu-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 10:14:57.408045 g3visu-0.1.7/
--rw-rw-rw-   0        0        0     1091 2024-04-29 14:15:00.000000 g3visu-0.1.7/LICENCE
--rw-rw-rw-   0        0        0     1759 2024-05-10 10:14:57.404134 g3visu-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-04-30 08:21:52.000000 g3visu-0.1.7/README.md
--rw-rw-rw-   0        0        0     1516 2024-05-10 10:08:48.000000 g3visu-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 10:14:57.408045 g3visu-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 10:14:57.292979 g3visu-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 10:14:57.318101 g3visu-0.1.7/src/g3visu/
--rw-rw-rw-   0        0        0      289 2024-04-29 14:15:00.000000 g3visu-0.1.7/src/g3visu/__init__.py
--rw-rw-rw-   0        0        0     5593 2024-04-30 12:55:51.000000 g3visu-0.1.7/src/g3visu/_cli.py
-drwxrwxrwx   0        0        0        0 2024-05-10 10:14:57.350985 g3visu-0.1.7/src/g3visu/meta/
--rw-rw-rw-   0        0        0       99 2024-04-29 14:15:00.000000 g3visu-0.1.7/src/g3visu/meta/__init__.py
--rw-rw-rw-   0        0        0     3591 2024-04-29 14:15:00.000000 g3visu-0.1.7/src/g3visu/meta/_meta.py
-drwxrwxrwx   0        0        0        0 2024-05-10 10:14:57.371949 g3visu-0.1.7/src/g3visu/site/
--rw-rw-rw-   0        0        0      120 2024-04-29 14:15:00.000000 g3visu-0.1.7/src/g3visu/site/__init__.py
--rw-rw-rw-   0        0        0    22979 2024-05-10 08:59:38.000000 g3visu-0.1.7/src/g3visu/site/_site_svg.py
--rw-rw-rw-   0        0        0    11402 2024-04-29 14:15:00.000000 g3visu-0.1.7/src/g3visu/site/_table.py
--rw-rw-rw-   0        0        0     5645 2024-05-06 18:57:40.000000 g3visu-0.1.7/src/g3visu/site/site.svg
-drwxrwxrwx   0        0        0        0 2024-05-10 10:14:57.387673 g3visu-0.1.7/src/g3visu/typeinfo/
--rw-rw-rw-   0        0        0      411 2024-04-29 14:15:00.000000 g3visu-0.1.7/src/g3visu/typeinfo/__init__.py
--rw-rw-rw-   0        0        0     1310 2024-04-30 12:56:03.000000 g3visu-0.1.7/src/g3visu/typeinfo/_list_operations.py
--rw-rw-rw-   0        0        0    19489 2024-04-30 12:56:11.000000 g3visu-0.1.7/src/g3visu/typeinfo/_typeinfo.py
--rw-rw-rw-   0        0        0        0 2024-04-29 14:15:00.000000 g3visu-0.1.7/src/g3visu/typeinfo/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-10 10:14:57.394615 g3visu-0.1.7/src/g3visu/utils/
--rw-rw-rw-   0        0        0      308 2024-04-29 14:15:00.000000 g3visu-0.1.7/src/g3visu/utils/__init__.py
--rw-rw-rw-   0        0        0     7709 2024-04-30 08:21:52.000000 g3visu-0.1.7/src/g3visu/utils/_download_from_sites.py
-drwxrwxrwx   0        0        0        0 2024-05-10 10:14:57.399773 g3visu-0.1.7/src/g3visu.egg-info/
--rw-rw-rw-   0        0        0     1759 2024-05-10 10:14:57.000000 g3visu-0.1.7/src/g3visu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2024-05-10 10:14:57.000000 g3visu-0.1.7/src/g3visu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 10:14:57.000000 g3visu-0.1.7/src/g3visu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-10 10:14:57.000000 g3visu-0.1.7/src/g3visu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      143 2024-05-10 10:14:57.000000 g3visu-0.1.7/src/g3visu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-10 10:14:57.000000 g3visu-0.1.7/src/g3visu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 08:26:20.171510 g3visu-0.1.8/
+-rw-rw-rw-   0        0        0     1091 2024-04-29 14:15:00.000000 g3visu-0.1.8/LICENCE
+-rw-rw-rw-   0        0        0     1759 2024-05-14 08:26:20.155883 g3visu-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-04-30 08:21:52.000000 g3visu-0.1.8/README.md
+-rw-rw-rw-   0        0        0     1516 2024-05-14 07:42:27.000000 g3visu-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 08:26:20.171510 g3visu-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 08:26:20.117725 g3visu-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 08:26:20.134739 g3visu-0.1.8/src/g3visu/
+-rw-rw-rw-   0        0        0      289 2024-04-29 14:15:00.000000 g3visu-0.1.8/src/g3visu/__init__.py
+-rw-rw-rw-   0        0        0     5593 2024-04-30 12:55:51.000000 g3visu-0.1.8/src/g3visu/_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:26:20.140246 g3visu-0.1.8/src/g3visu/meta/
+-rw-rw-rw-   0        0        0       99 2024-04-29 14:15:00.000000 g3visu-0.1.8/src/g3visu/meta/__init__.py
+-rw-rw-rw-   0        0        0     3585 2024-05-14 07:40:50.000000 g3visu-0.1.8/src/g3visu/meta/_meta.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:26:20.155883 g3visu-0.1.8/src/g3visu/site/
+-rw-rw-rw-   0        0        0      120 2024-04-29 14:15:00.000000 g3visu-0.1.8/src/g3visu/site/__init__.py
+-rw-rw-rw-   0        0        0    22979 2024-05-10 08:59:38.000000 g3visu-0.1.8/src/g3visu/site/_site_svg.py
+-rw-rw-rw-   0        0        0    11402 2024-04-29 14:15:00.000000 g3visu-0.1.8/src/g3visu/site/_table.py
+-rw-rw-rw-   0        0        0     5645 2024-05-06 18:57:40.000000 g3visu-0.1.8/src/g3visu/site/site.svg
+drwxrwxrwx   0        0        0        0 2024-05-14 08:26:20.155883 g3visu-0.1.8/src/g3visu/typeinfo/
+-rw-rw-rw-   0        0        0      411 2024-04-29 14:15:00.000000 g3visu-0.1.8/src/g3visu/typeinfo/__init__.py
+-rw-rw-rw-   0        0        0     1310 2024-04-30 12:56:03.000000 g3visu-0.1.8/src/g3visu/typeinfo/_list_operations.py
+-rw-rw-rw-   0        0        0    19489 2024-04-30 12:56:11.000000 g3visu-0.1.8/src/g3visu/typeinfo/_typeinfo.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:15:00.000000 g3visu-0.1.8/src/g3visu/typeinfo/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-14 08:26:20.155883 g3visu-0.1.8/src/g3visu/utils/
+-rw-rw-rw-   0        0        0      308 2024-04-29 14:15:00.000000 g3visu-0.1.8/src/g3visu/utils/__init__.py
+-rw-rw-rw-   0        0        0     7709 2024-04-30 08:21:52.000000 g3visu-0.1.8/src/g3visu/utils/_download_from_sites.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:26:20.155883 g3visu-0.1.8/src/g3visu.egg-info/
+-rw-rw-rw-   0        0        0     1759 2024-05-14 08:26:20.000000 g3visu-0.1.8/src/g3visu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2024-05-14 08:26:20.000000 g3visu-0.1.8/src/g3visu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:26:20.000000 g3visu-0.1.8/src/g3visu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-14 08:26:20.000000 g3visu-0.1.8/src/g3visu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      143 2024-05-14 08:26:20.000000 g3visu-0.1.8/src/g3visu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-14 08:26:20.000000 g3visu-0.1.8/src/g3visu.egg-info/top_level.txt
```

### Comparing `g3visu-0.1.7/LICENCE` & `g3visu-0.1.8/LICENCE`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.7/PKG-INFO` & `g3visu-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3visu
-Version: 0.1.7
+Version: 0.1.8
 Summary: System G3 Visualization files' parsers and generators
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Visu.git
 Keywords: Elektroline,System G3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3visu-0.1.7/pyproject.toml` & `g3visu-0.1.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "g3visu"
-version = "0.1.7"
+version = "0.1.8"
 description = "System G3 Visualization files' parsers and generators"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
   { name = "Elektroline a.s." },
 ]
 classifiers = [
```

### Comparing `g3visu-0.1.7/src/g3visu/_cli.py` & `g3visu-0.1.8/src/g3visu/_cli.py`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.7/src/g3visu/meta/_meta.py` & `g3visu-0.1.8/src/g3visu/meta/_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     @abstractmethod
     def model_validate_system_config(cls, system_config: dict) -> typing.Self:
         pass
 
 
 class MetaProjectSiteWare(BaseMeta):
     shv_user: str = Field(default="viewer")
-    shv_password: str = Field(default="42view")
+    shv_password: str = Field(default="")
     default_language: str
     language_array: list[str]
 
     @classmethod
     def model_validate_system_config(
         cls, system_config: dict, **kwargs
     ) -> typing.Self:
```

### Comparing `g3visu-0.1.7/src/g3visu/site/_site_svg.py` & `g3visu-0.1.8/src/g3visu/site/_site_svg.py`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.7/src/g3visu/site/_table.py` & `g3visu-0.1.8/src/g3visu/site/_table.py`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.7/src/g3visu/site/site.svg` & `g3visu-0.1.8/src/g3visu/site/site.svg`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.7/src/g3visu/typeinfo/_list_operations.py` & `g3visu-0.1.8/src/g3visu/typeinfo/_list_operations.py`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.7/src/g3visu/typeinfo/_typeinfo.py` & `g3visu-0.1.8/src/g3visu/typeinfo/_typeinfo.py`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.7/src/g3visu/utils/_download_from_sites.py` & `g3visu-0.1.8/src/g3visu/utils/_download_from_sites.py`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.7/src/g3visu.egg-info/PKG-INFO` & `g3visu-0.1.8/src/g3visu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3visu
-Version: 0.1.7
+Version: 0.1.8
 Summary: System G3 Visualization files' parsers and generators
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Visu.git
 Keywords: Elektroline,System G3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3visu-0.1.7/src/g3visu.egg-info/SOURCES.txt` & `g3visu-0.1.8/src/g3visu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

