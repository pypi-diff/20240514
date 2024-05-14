# Comparing `tmp/browsergym-0.2.1.tar.gz` & `tmp/browsergym-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browsergym-0.2.1.tar", last modified: Fri May 10 17:09:30 2024, max compression
+gzip compressed data, was "browsergym-0.2.2.tar", last modified: Tue May 14 19:58:34 2024, max compression
```

## Comparing `browsergym-0.2.1.tar` & `browsergym-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:09:30.780627 browsergym-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-10 17:09:17.000000 browsergym-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-10 17:09:30.780627 browsergym-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-10 17:09:17.000000 browsergym-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:09:30.780627 browsergym-0.2.1/browsergym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-10 17:09:30.000000 browsergym-0.2.1/browsergym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-10 17:09:30.000000 browsergym-0.2.1/browsergym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:09:30.000000 browsergym-0.2.1/browsergym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-10 17:09:30.000000 browsergym-0.2.1/browsergym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:09:30.000000 browsergym-0.2.1/browsergym.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-10 17:09:17.000000 browsergym-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:09:30.780627 browsergym-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:58:34.771437 browsergym-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-14 19:58:21.000000 browsergym-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-05-14 19:58:34.771437 browsergym-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-14 19:58:21.000000 browsergym-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:58:34.771437 browsergym-0.2.2/browsergym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-05-14 19:58:34.000000 browsergym-0.2.2/browsergym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-14 19:58:34.000000 browsergym-0.2.2/browsergym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:58:34.000000 browsergym-0.2.2/browsergym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 19:58:34.000000 browsergym-0.2.2/browsergym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:58:34.000000 browsergym-0.2.2/browsergym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-14 19:58:21.000000 browsergym-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:58:34.771437 browsergym-0.2.2/setup.cfg
```

### Comparing `browsergym-0.2.1/LICENSE` & `browsergym-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `browsergym-0.2.1/PKG-INFO` & `browsergym-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: browsergym
-Version: 0.2.1
+Version: 0.2.2
 Summary: BrowserGym: a gym environment for web task automation in the Chromium browser
 Author: Rim Assouel, Léo Boisvert, Massimo Caccia, Alex Drouin, Maxime Gasse, Alex Lacoste, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: browsergym-core==0.2.1
-Requires-Dist: browsergym-miniwob==0.2.1
-Requires-Dist: browsergym-webarena==0.2.1
-Requires-Dist: browsergym-workarena==0.2.1
+Requires-Dist: browsergym-core==0.2.2
+Requires-Dist: browsergym-miniwob==0.2.2
+Requires-Dist: browsergym-webarena==0.2.2
+Requires-Dist: browsergym-workarena
 
 # BrowserGym: a Gym Environment for Web Task Automation
 
 [[Setup]](#setup) ♦ [[Usage]](#usage) ♦ [[Demo]](#demo)
 
 This package provides `browsergym`, a gym environment for web task automation in the Chromium browser.
```

### Comparing `browsergym-0.2.1/README.md` & `browsergym-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `browsergym-0.2.1/browsergym.egg-info/PKG-INFO` & `browsergym-0.2.2/browsergym.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: browsergym
-Version: 0.2.1
+Version: 0.2.2
 Summary: BrowserGym: a gym environment for web task automation in the Chromium browser
 Author: Rim Assouel, Léo Boisvert, Massimo Caccia, Alex Drouin, Maxime Gasse, Alex Lacoste, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: browsergym-core==0.2.1
-Requires-Dist: browsergym-miniwob==0.2.1
-Requires-Dist: browsergym-webarena==0.2.1
-Requires-Dist: browsergym-workarena==0.2.1
+Requires-Dist: browsergym-core==0.2.2
+Requires-Dist: browsergym-miniwob==0.2.2
+Requires-Dist: browsergym-webarena==0.2.2
+Requires-Dist: browsergym-workarena
 
 # BrowserGym: a Gym Environment for Web Task Automation
 
 [[Setup]](#setup) ♦ [[Usage]](#usage) ♦ [[Demo]](#demo)
 
 This package provides `browsergym`, a gym environment for web task automation in the Chromium browser.
```

### Comparing `browsergym-0.2.1/pyproject.toml` & `browsergym-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: Apache Software License",
 ]
-version="0.2.1"
+version="0.2.2"
 dependencies = [
-    "browsergym-core==0.2.1",
-    "browsergym-miniwob==0.2.1",
-    "browsergym-webarena==0.2.1",
-    "browsergym-workarena==0.2.1",
+    "browsergym-core==0.2.2",
+    "browsergym-miniwob==0.2.2",
+    "browsergym-webarena==0.2.2",
+    "browsergym-workarena",
 ]
 
 [tool.setuptools]
 packages = []  # meta distribution, packages are included as dependencies
 
 [tool.black]
 line-length = 100
```

