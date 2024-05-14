# Comparing `tmp/wrongbutusefulsbi-0.0.3.tar.gz` & `tmp/wrongbutusefulsbi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrongbutusefulsbi-0.0.3.tar", last modified: Tue May 14 02:40:12 2024, max compression
+gzip compressed data, was "wrongbutusefulsbi-0.0.4.tar", last modified: Tue May 14 03:02:38 2024, max compression
```

## Comparing `wrongbutusefulsbi-0.0.3.tar` & `wrongbutusefulsbi-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:12.149342 wrongbutusefulsbi-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 02:40:08.000000 wrongbutusefulsbi-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 02:40:12.149342 wrongbutusefulsbi-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-14 02:40:08.000000 wrongbutusefulsbi-0.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 02:40:12.149342 wrongbutusefulsbi-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-14 02:40:08.000000 wrongbutusefulsbi-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:12.149342 wrongbutusefulsbi-0.0.3/wrongbutusefulsbi/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 02:40:08.000000 wrongbutusefulsbi-0.0.3/wrongbutusefulsbi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:40:12.149342 wrongbutusefulsbi-0.0.3/wrongbutusefulsbi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 02:40:12.000000 wrongbutusefulsbi-0.0.3/wrongbutusefulsbi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-14 02:40:12.000000 wrongbutusefulsbi-0.0.3/wrongbutusefulsbi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 02:40:12.000000 wrongbutusefulsbi-0.0.3/wrongbutusefulsbi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 02:40:12.000000 wrongbutusefulsbi-0.0.3/wrongbutusefulsbi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 02:40:12.000000 wrongbutusefulsbi-0.0.3/wrongbutusefulsbi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:02:38.388204 wrongbutusefulsbi-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 03:02:34.000000 wrongbutusefulsbi-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 03:02:38.388204 wrongbutusefulsbi-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-14 03:02:34.000000 wrongbutusefulsbi-0.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 03:02:38.388204 wrongbutusefulsbi-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-14 03:02:34.000000 wrongbutusefulsbi-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:02:38.384204 wrongbutusefulsbi-0.0.4/wrongbutusefulsbi/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-14 03:02:34.000000 wrongbutusefulsbi-0.0.4/wrongbutusefulsbi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:02:38.388204 wrongbutusefulsbi-0.0.4/wrongbutusefulsbi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 03:02:38.000000 wrongbutusefulsbi-0.0.4/wrongbutusefulsbi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-14 03:02:38.000000 wrongbutusefulsbi-0.0.4/wrongbutusefulsbi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 03:02:38.000000 wrongbutusefulsbi-0.0.4/wrongbutusefulsbi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 03:02:38.000000 wrongbutusefulsbi-0.0.4/wrongbutusefulsbi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 03:02:38.000000 wrongbutusefulsbi-0.0.4/wrongbutusefulsbi.egg-info/top_level.txt
```

### Comparing `wrongbutusefulsbi-0.0.3/LICENSE` & `wrongbutusefulsbi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wrongbutusefulsbi-0.0.3/PKG-INFO` & `wrongbutusefulsbi-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrongbutusefulsbi
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/RyanJafefKelly/wrongbutusefulsbi
 Author: Ryan Kelly
 Author-email: ryan@kiiii.com
 License: GPLv3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `wrongbutusefulsbi-0.0.3/README.rst` & `wrongbutusefulsbi-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `wrongbutusefulsbi-0.0.3/setup.py` & `wrongbutusefulsbi-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name='wrongbutusefulsbi',
-    version='0.0.3',
+    version='0.0.4',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author='Ryan Kelly',
     author_email='ryan@kiiii.com',
     url='https://github.com/RyanJafefKelly/wrongbutusefulsbi',
     install_requires=requirements,
     license='GPLv3',
```

### Comparing `wrongbutusefulsbi-0.0.3/wrongbutusefulsbi.egg-info/PKG-INFO` & `wrongbutusefulsbi-0.0.4/wrongbutusefulsbi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrongbutusefulsbi
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/RyanJafefKelly/wrongbutusefulsbi
 Author: Ryan Kelly
 Author-email: ryan@kiiii.com
 License: GPLv3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

