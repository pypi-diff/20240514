# Comparing `tmp/wrongbutusefulsbi-0.0.6.tar.gz` & `tmp/wrongbutusefulsbi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrongbutusefulsbi-0.0.6.tar", last modified: Tue May 14 03:30:45 2024, max compression
+gzip compressed data, was "wrongbutusefulsbi-0.0.7.tar", last modified: Tue May 14 03:42:13 2024, max compression
```

## Comparing `wrongbutusefulsbi-0.0.6.tar` & `wrongbutusefulsbi-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:30:45.919577 wrongbutusefulsbi-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 03:30:41.000000 wrongbutusefulsbi-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 03:30:45.919577 wrongbutusefulsbi-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-14 03:30:41.000000 wrongbutusefulsbi-0.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 03:30:45.919577 wrongbutusefulsbi-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-14 03:30:41.000000 wrongbutusefulsbi-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:30:45.919577 wrongbutusefulsbi-0.0.6/wrongbutusefulsbi/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-14 03:30:41.000000 wrongbutusefulsbi-0.0.6/wrongbutusefulsbi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:30:45.919577 wrongbutusefulsbi-0.0.6/wrongbutusefulsbi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 03:30:45.000000 wrongbutusefulsbi-0.0.6/wrongbutusefulsbi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-14 03:30:45.000000 wrongbutusefulsbi-0.0.6/wrongbutusefulsbi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 03:30:45.000000 wrongbutusefulsbi-0.0.6/wrongbutusefulsbi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 03:30:45.000000 wrongbutusefulsbi-0.0.6/wrongbutusefulsbi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 03:30:45.000000 wrongbutusefulsbi-0.0.6/wrongbutusefulsbi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:42:13.140455 wrongbutusefulsbi-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 03:42:13.140455 wrongbutusefulsbi-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 03:42:13.140455 wrongbutusefulsbi-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:42:13.140455 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:42:13.140455 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi/examples/bvcbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi/examples/contaminated_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi/examples/contaminated_slcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi/examples/gaussian_vs_laplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi/examples/misspec_ma1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi/examples/sir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi/examples/toad.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:42:08.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi/examples/wright_fisher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:42:13.140455 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 03:42:13.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-14 03:42:13.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 03:42:13.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 03:42:13.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 03:42:13.000000 wrongbutusefulsbi-0.0.7/wrongbutusefulsbi.egg-info/top_level.txt
```

### Comparing `wrongbutusefulsbi-0.0.6/LICENSE` & `wrongbutusefulsbi-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wrongbutusefulsbi-0.0.6/PKG-INFO` & `wrongbutusefulsbi-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrongbutusefulsbi
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/RyanJafefKelly/wrongbutusefulsbi
 Author: Ryan Kelly
 Author-email: ryan@kiiii.com
 License: GPLv3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `wrongbutusefulsbi-0.0.6/README.rst` & `wrongbutusefulsbi-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `wrongbutusefulsbi-0.0.6/setup.py` & `wrongbutusefulsbi-0.0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from setuptools import setup
+from setuptools import setup, find_packages
+
+packages = ['wrongbutusefulsbi'] + ['wrongbutusefulsbi.' + p for p in find_packages('wrongbutusefulsbi')]
 
 with open("README.rst", encoding='utf8') as fh:
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 # read version number
 __version__ = open('wrongbutusefulsbi/__init__.py').readlines()[-1].split(' ')[-1].strip().strip("'\"")
 
 setup(
     name='wrongbutusefulsbi',
     version=__version__,
+    packages=packages,
+    include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author='Ryan Kelly',
     author_email='ryan@kiiii.com',
     url='https://github.com/RyanJafefKelly/wrongbutusefulsbi',
     install_requires=requirements,
     license='GPLv3',
     python_requires='>=3.7',
-    packages=['wrongbutusefulsbi'],
 )
```

### Comparing `wrongbutusefulsbi-0.0.6/wrongbutusefulsbi.egg-info/PKG-INFO` & `wrongbutusefulsbi-0.0.7/wrongbutusefulsbi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrongbutusefulsbi
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/RyanJafefKelly/wrongbutusefulsbi
 Author: Ryan Kelly
 Author-email: ryan@kiiii.com
 License: GPLv3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

