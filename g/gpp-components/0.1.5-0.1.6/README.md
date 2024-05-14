# Comparing `tmp/gpp_components-0.1.5.tar.gz` & `tmp/gpp_components-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpp_components-0.1.5.tar", last modified: Fri Apr 26 03:00:55 2024, max compression
+gzip compressed data, was "gpp_components-0.1.6.tar", last modified: Tue May 14 05:55:45 2024, max compression
```

## Comparing `gpp_components-0.1.5.tar` & `gpp_components-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 03:00:55.674511 gpp_components-0.1.5/
--rw-rw-rw-   0        0        0     1097 2024-01-24 04:54:41.000000 gpp_components-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      412 2024-04-26 03:00:55.674511 gpp_components-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       58 2024-01-24 04:54:41.000000 gpp_components-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 03:00:55.606733 gpp_components-0.1.5/gpp_components/
--rw-rw-rw-   0        0        0       19 2024-01-24 04:54:41.000000 gpp_components-0.1.5/gpp_components/__init__.py
--rw-rw-rw-   0        0        0     1076 2024-01-24 04:54:41.000000 gpp_components-0.1.5/gpp_components/aes.py
--rw-rw-rw-   0        0        0      239 2024-01-26 05:10:34.000000 gpp_components-0.1.5/gpp_components/constant.py
--rw-rw-rw-   0        0        0     4442 2024-01-24 04:54:41.000000 gpp_components-0.1.5/gpp_components/dbConfig.py
--rw-rw-rw-   0        0        0     2535 2024-04-02 12:30:35.000000 gpp_components-0.1.5/gpp_components/decorator.py
--rw-rw-rw-   0        0        0     9431 2024-04-26 02:59:51.000000 gpp_components-0.1.5/gpp_components/fileImporter.py
--rw-rw-rw-   0        0        0     7692 2024-04-17 06:42:48.000000 gpp_components-0.1.5/gpp_components/handleData.py
--rw-rw-rw-   0        0        0     1629 2024-01-24 04:54:41.000000 gpp_components-0.1.5/gpp_components/lazyImport.py
--rw-rw-rw-   0        0        0     1422 2024-03-04 01:22:22.000000 gpp_components-0.1.5/gpp_components/response.py
--rw-rw-rw-   0        0        0     5115 2024-04-17 06:41:00.000000 gpp_components-0.1.5/gpp_components/runOracle.py
--rw-rw-rw-   0        0        0     2880 2024-01-24 04:54:41.000000 gpp_components-0.1.5/gpp_components/sendMail.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:00:55.657780 gpp_components-0.1.5/gpp_components.egg-info/
--rw-rw-rw-   0        0        0      412 2024-04-26 03:00:54.000000 gpp_components-0.1.5/gpp_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2024-04-26 03:00:55.000000 gpp_components-0.1.5/gpp_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 03:00:55.000000 gpp_components-0.1.5/gpp_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-26 03:00:55.000000 gpp_components-0.1.5/gpp_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-26 03:00:55.000000 gpp_components-0.1.5/gpp_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 03:00:55.685507 gpp_components-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      876 2024-04-26 03:00:18.000000 gpp_components-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:55:45.832958 gpp_components-0.1.6/
+-rw-rw-rw-   0        0        0     1097 2024-01-24 04:54:41.000000 gpp_components-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      412 2024-05-14 05:55:45.832958 gpp_components-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       58 2024-01-24 04:54:41.000000 gpp_components-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 05:55:45.749453 gpp_components-0.1.6/gpp_components/
+-rw-rw-rw-   0        0        0       19 2024-01-24 04:54:41.000000 gpp_components-0.1.6/gpp_components/__init__.py
+-rw-rw-rw-   0        0        0     1076 2024-01-24 04:54:41.000000 gpp_components-0.1.6/gpp_components/aes.py
+-rw-rw-rw-   0        0        0      239 2024-01-26 05:10:34.000000 gpp_components-0.1.6/gpp_components/constant.py
+-rw-rw-rw-   0        0        0     4442 2024-01-24 04:54:41.000000 gpp_components-0.1.6/gpp_components/dbConfig.py
+-rw-rw-rw-   0        0        0     2535 2024-04-02 12:30:35.000000 gpp_components-0.1.6/gpp_components/decorator.py
+-rw-rw-rw-   0        0        0     9431 2024-04-26 03:21:24.000000 gpp_components-0.1.6/gpp_components/fileImporter.py
+-rw-rw-rw-   0        0        0     7696 2024-05-14 05:53:22.000000 gpp_components-0.1.6/gpp_components/handleData.py
+-rw-rw-rw-   0        0        0     1629 2024-01-24 04:54:41.000000 gpp_components-0.1.6/gpp_components/lazyImport.py
+-rw-rw-rw-   0        0        0     1422 2024-03-04 01:22:22.000000 gpp_components-0.1.6/gpp_components/response.py
+-rw-rw-rw-   0        0        0     5115 2024-04-17 06:41:00.000000 gpp_components-0.1.6/gpp_components/runOracle.py
+-rw-rw-rw-   0        0        0     2880 2024-01-24 04:54:41.000000 gpp_components-0.1.6/gpp_components/sendMail.py
+drwxrwxrwx   0        0        0        0 2024-05-14 05:55:45.816932 gpp_components-0.1.6/gpp_components.egg-info/
+-rw-rw-rw-   0        0        0      412 2024-05-14 05:55:44.000000 gpp_components-0.1.6/gpp_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2024-05-14 05:55:45.000000 gpp_components-0.1.6/gpp_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 05:55:45.000000 gpp_components-0.1.6/gpp_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-14 05:55:45.000000 gpp_components-0.1.6/gpp_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 05:55:45.000000 gpp_components-0.1.6/gpp_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 05:55:45.847349 gpp_components-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-05-14 05:55:34.000000 gpp_components-0.1.6/setup.py
```

### Comparing `gpp_components-0.1.5/LICENSE` & `gpp_components-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.5/gpp_components/aes.py` & `gpp_components-0.1.6/gpp_components/aes.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.5/gpp_components/dbConfig.py` & `gpp_components-0.1.6/gpp_components/dbConfig.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.5/gpp_components/decorator.py` & `gpp_components-0.1.6/gpp_components/decorator.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.5/gpp_components/fileImporter.py` & `gpp_components-0.1.6/gpp_components/fileImporter.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.5/gpp_components/handleData.py` & `gpp_components-0.1.6/gpp_components/handleData.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,16 +107,16 @@
 
         if exclude and f.name in exclude:
             continue
 
         if isinstance(f, ManyToManyField):
             value = [i.id for i in value] if self.pk else None
 
-        if isinstance(f, DateTimeField):
-            value = value.strftime("%Y-%m-%d %H:%M:%S") if value else None
+        # if isinstance(f, DateTimeField):
+        #     value = value.strftime("%Y-%m-%d %H:%M:%S") if value else None
 
         data[f.name] = value
 
     return data
 
 
 def addCreateModifyDate(obj, type="ymd"):
```

### Comparing `gpp_components-0.1.5/gpp_components/lazyImport.py` & `gpp_components-0.1.6/gpp_components/lazyImport.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.5/gpp_components/response.py` & `gpp_components-0.1.6/gpp_components/response.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.5/gpp_components/runOracle.py` & `gpp_components-0.1.6/gpp_components/runOracle.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.5/gpp_components/sendMail.py` & `gpp_components-0.1.6/gpp_components/sendMail.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.5/gpp_components.egg-info/SOURCES.txt` & `gpp_components-0.1.6/gpp_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.5/setup.py` & `gpp_components-0.1.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gpp_components",
-    version = '0.1.5',
+    version = '0.1.6',
     # version="0.0.36", # last version for Py310
     #
     author="L",
     description="for internal use",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT Licence",
```

