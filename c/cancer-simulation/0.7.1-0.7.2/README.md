# Comparing `tmp/cancer_simulation-0.7.1.tar.gz` & `tmp/cancer_simulation-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cancer_simulation-0.7.1.tar", last modified: Mon May 13 05:52:15 2024, max compression
+gzip compressed data, was "cancer_simulation-0.7.2.tar", last modified: Mon May 13 05:55:04 2024, max compression
```

## Comparing `cancer_simulation-0.7.1.tar` & `cancer_simulation-0.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-13 05:52:15.400377 cancer_simulation-0.7.1/
--rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      324 2024-05-13 05:52:15.396377 cancer_simulation-0.7.1/PKG-INFO
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     9885 2024-05-12 12:44:46.000000 cancer_simulation-0.7.1/README.md
-drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-13 05:52:15.396377 cancer_simulation-0.7.1/cancer_simulation.egg-info/
--rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      324 2024-05-13 05:52:15.000000 cancer_simulation-0.7.1/cancer_simulation.egg-info/PKG-INFO
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      390 2024-05-13 05:52:15.000000 cancer_simulation-0.7.1/cancer_simulation.egg-info/SOURCES.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        1 2024-05-13 05:52:15.000000 cancer_simulation-0.7.1/cancer_simulation.egg-info/dependency_links.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       34 2024-05-13 05:52:15.000000 cancer_simulation-0.7.1/cancer_simulation.egg-info/entry_points.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       62 2024-05-13 05:52:15.000000 cancer_simulation-0.7.1/cancer_simulation.egg-info/requires.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        4 2024-05-13 05:52:15.000000 cancer_simulation-0.7.1/cancer_simulation.egg-info/top_level.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       38 2024-05-13 05:52:15.400377 cancer_simulation-0.7.1/setup.cfg
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      754 2024-05-13 05:51:54.000000 cancer_simulation-0.7.1/setup.py
-drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-13 05:52:15.396377 cancer_simulation-0.7.1/src/
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       30 2024-05-12 18:56:52.000000 cancer_simulation-0.7.1/src/__init__.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2986 2024-05-12 19:00:27.000000 cancer_simulation-0.7.1/src/automaton.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     1625 2024-05-12 17:43:44.000000 cancer_simulation-0.7.1/src/cell.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      274 2024-05-11 21:25:41.000000 cancer_simulation-0.7.1/src/constants.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)    12362 2024-05-12 18:59:45.000000 cancer_simulation-0.7.1/src/csimulation.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     8346 2024-05-12 19:00:17.000000 cancer_simulation-0.7.1/src/entity.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2924 2024-05-12 19:00:03.000000 cancer_simulation-0.7.1/src/grid.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     4286 2024-05-12 11:57:53.000000 cancer_simulation-0.7.1/src/variables.py
+drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-13 05:55:04.554490 cancer_simulation-0.7.2/
+-rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      546 2024-05-13 05:55:04.554490 cancer_simulation-0.7.2/PKG-INFO
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     9885 2024-05-12 12:44:46.000000 cancer_simulation-0.7.2/README.md
+drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-13 05:55:04.554490 cancer_simulation-0.7.2/cancer_simulation.egg-info/
+-rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      546 2024-05-13 05:55:04.000000 cancer_simulation-0.7.2/cancer_simulation.egg-info/PKG-INFO
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      390 2024-05-13 05:55:04.000000 cancer_simulation-0.7.2/cancer_simulation.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        1 2024-05-13 05:55:04.000000 cancer_simulation-0.7.2/cancer_simulation.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       34 2024-05-13 05:55:04.000000 cancer_simulation-0.7.2/cancer_simulation.egg-info/entry_points.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       62 2024-05-13 05:55:04.000000 cancer_simulation-0.7.2/cancer_simulation.egg-info/requires.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        4 2024-05-13 05:55:04.000000 cancer_simulation-0.7.2/cancer_simulation.egg-info/top_level.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       38 2024-05-13 05:55:04.554490 cancer_simulation-0.7.2/setup.cfg
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      828 2024-05-13 05:54:35.000000 cancer_simulation-0.7.2/setup.py
+drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-13 05:55:04.550490 cancer_simulation-0.7.2/src/
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       30 2024-05-12 18:56:52.000000 cancer_simulation-0.7.2/src/__init__.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2986 2024-05-12 19:00:27.000000 cancer_simulation-0.7.2/src/automaton.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     1625 2024-05-12 17:43:44.000000 cancer_simulation-0.7.2/src/cell.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      274 2024-05-11 21:25:41.000000 cancer_simulation-0.7.2/src/constants.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)    12362 2024-05-12 18:59:45.000000 cancer_simulation-0.7.2/src/csimulation.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     8346 2024-05-12 19:00:17.000000 cancer_simulation-0.7.2/src/entity.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2924 2024-05-12 19:00:03.000000 cancer_simulation-0.7.2/src/grid.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     4286 2024-05-12 11:57:53.000000 cancer_simulation-0.7.2/src/variables.py
```

### Comparing `cancer_simulation-0.7.1/README.md` & `cancer_simulation-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.1/setup.py` & `cancer_simulation-0.7.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cancer_simulation",
-    version='0.7.1',
+    version='0.7.2',
     packages=find_packages(),
-    description="""We implemented cancer development and chemotherapy impact simulation using
+    short_description="A simple cancer and chemotherapy simulation",
+    long_description="""We implemented cancer development and chemotherapy impact simulation using
                    stochastic cellular automaton with Python. The main feature of implemented 
                    app is capability of simulating different treatment strategies under same-
                    type cancer behavior.""",
     url = "https://github.com/Zhukowych/CancerSimulation",
     install_requires = [
         'pygame==2.5.2',
         'pygame-chart==1.0.0',
```

### Comparing `cancer_simulation-0.7.1/src/automaton.py` & `cancer_simulation-0.7.2/src/automaton.py`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.1/src/cell.py` & `cancer_simulation-0.7.2/src/cell.py`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.1/src/csimulation.py` & `cancer_simulation-0.7.2/src/csimulation.py`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.1/src/entity.py` & `cancer_simulation-0.7.2/src/entity.py`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.1/src/grid.py` & `cancer_simulation-0.7.2/src/grid.py`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.1/src/variables.py` & `cancer_simulation-0.7.2/src/variables.py`

 * *Files identical despite different names*

