# Comparing `tmp/RunFeemsSim-0.2.3.tar.gz` & `tmp/runfeemssim-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RunFeemsSim-0.2.3.tar", last modified: Tue Apr  9 12:53:48 2024, max compression
+gzip compressed data, was "runfeemssim-0.2.4.tar", last modified: Tue May 14 10:59:21 2024, max compression
```

## Comparing `RunFeemsSim-0.2.3.tar` & `runfeemssim-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.267446 RunFeemsSim-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-09 12:53:48.267446 RunFeemsSim-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.267446 RunFeemsSim-0.2.3/RunFeemsSim/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/RunFeemsSim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/RunFeemsSim/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/RunFeemsSim/_nbdev.py
--rw-r--r--   0 runner    (1001) docker     (127)    14740 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/RunFeemsSim/machinery_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/RunFeemsSim/pms_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/RunFeemsSim/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.267446 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-09 12:53:48.000000 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-09 12:53:48.000000 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:53:48.000000 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:53:48.000000 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 12:53:48.000000 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 12:53:48.000000 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:53:48.267446 RunFeemsSim-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:59:21.869727 runfeemssim-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-14 10:59:17.000000 runfeemssim-0.2.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-14 10:59:17.000000 runfeemssim-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-14 10:59:17.000000 runfeemssim-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-14 10:59:21.869727 runfeemssim-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-14 10:59:17.000000 runfeemssim-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:59:21.865727 runfeemssim-0.2.4/RunFeemsSim/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 10:59:17.000000 runfeemssim-0.2.4/RunFeemsSim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-14 10:59:17.000000 runfeemssim-0.2.4/RunFeemsSim/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-14 10:59:17.000000 runfeemssim-0.2.4/RunFeemsSim/_nbdev.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14740 2024-05-14 10:59:17.000000 runfeemssim-0.2.4/RunFeemsSim/machinery_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-14 10:59:17.000000 runfeemssim-0.2.4/RunFeemsSim/pms_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:59:17.000000 runfeemssim-0.2.4/RunFeemsSim/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:59:21.869727 runfeemssim-0.2.4/RunFeemsSim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-14 10:59:21.000000 runfeemssim-0.2.4/RunFeemsSim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-14 10:59:21.000000 runfeemssim-0.2.4/RunFeemsSim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:59:21.000000 runfeemssim-0.2.4/RunFeemsSim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:59:21.000000 runfeemssim-0.2.4/RunFeemsSim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 10:59:21.000000 runfeemssim-0.2.4/RunFeemsSim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 10:59:21.000000 runfeemssim-0.2.4/RunFeemsSim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-14 10:59:17.000000 runfeemssim-0.2.4/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:59:21.869727 runfeemssim-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-14 10:59:17.000000 runfeemssim-0.2.4/setup.py
```

### Comparing `RunFeemsSim-0.2.3/CONTRIBUTING.md` & `runfeemssim-0.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.3/LICENSE` & `runfeemssim-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.3/PKG-INFO` & `runfeemssim-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RunFeemsSim
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library for running feems simulation
 Home-page: https://github.com/SINTEF/FEEMS
 Author: Kevin Koosup Yum
 Author-email: kevinkoosup.yum@sintef.no
 License: Apache Software License 2.0
 Keywords: FEEMS,machinery system,fuel,emissions
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `RunFeemsSim-0.2.3/README.md` & `runfeemssim-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.3/RunFeemsSim/_modidx.py` & `runfeemssim-0.2.4/RunFeemsSim/_modidx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Autogenerated by nbdev
 
 d = {
     "settings": {
         "branch": "master",
         "doc_baseurl": "/RunFeemsSim/",
         "doc_host": "https://kevinkoosup.yum@sintef.no.github.io",
-        "git_url": "https://SintefOceanEnergySystem@dev.azure.com/SintefOceanEnergySystem/FEEMSService/_git/RunFEEMSSim",
+        "git_url": "https://github.com/SINTEF/FEEMS",
         "lib_path": "RunFeemsSim",
     },
     "syms": {
         "RunFeemsSim.machinery_calculation": {
             "RunFeemsSim.machinery_calculation.MachineryCalculation": (
                 "machinery_calculation.html#machinerycalculation",
                 "RunFeemsSim/machinery_calculation.py",
```

### Comparing `RunFeemsSim-0.2.3/RunFeemsSim/_nbdev.py` & `runfeemssim-0.2.4/RunFeemsSim/_nbdev.py`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.3/RunFeemsSim/machinery_calculation.py` & `runfeemssim-0.2.4/RunFeemsSim/machinery_calculation.py`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.3/RunFeemsSim/pms_basic.py` & `runfeemssim-0.2.4/RunFeemsSim/pms_basic.py`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.3/RunFeemsSim.egg-info/PKG-INFO` & `runfeemssim-0.2.4/RunFeemsSim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RunFeemsSim
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library for running feems simulation
 Home-page: https://github.com/SINTEF/FEEMS
 Author: Kevin Koosup Yum
 Author-email: kevinkoosup.yum@sintef.no
 License: Apache Software License 2.0
 Keywords: FEEMS,machinery system,fuel,emissions
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `RunFeemsSim-0.2.3/settings.ini` & `runfeemssim-0.2.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = kevinkoosup.yum@sintef.no
 description = A library for running feems simulation
 keywords = FEEMS, machinery system, fuel, emissions
 author = Kevin Koosup Yum
 author_email = kevinkoosup.yum@sintef.no
 copyright = SINTEF
 branch = master
-version = 0.2.3
+version = 0.2.4
 min_python = 3.10
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = pandas numpy MachSysS
```

### Comparing `RunFeemsSim-0.2.3/setup.py` & `runfeemssim-0.2.4/setup.py`

 * *Files identical despite different names*

