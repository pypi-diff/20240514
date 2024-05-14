# Comparing `tmp/nornir_arista-0.0.1.tar.gz` & `tmp/nornir_arista-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_arista-0.0.1.tar", last modified: Wed May  1 01:33:53 2024, max compression
+gzip compressed data, was "nornir_arista-0.0.2.tar", last modified: Tue May 14 05:39:17 2024, max compression
```

## Comparing `nornir_arista-0.0.1.tar` & `nornir_arista-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vicc     (12511) operations  (6003)        0 2024-05-01 01:33:53.219163 nornir_arista-0.0.1/
--rw-r--r--   0 vicc     (12511) operations  (6003)      637 2024-05-01 01:33:53.219163 nornir_arista-0.0.1/PKG-INFO
--rw-r--r--   0 vicc     (12511) operations  (6003)       46 2024-04-24 02:48:06.000000 nornir_arista-0.0.1/README.md
-drwxr-xr-x   0 vicc     (12511) operations  (6003)        0 2024-05-01 01:33:53.219163 nornir_arista-0.0.1/nornir_arista/
--rw-r--r--   0 vicc     (12511) operations  (6003)       21 2024-04-24 02:40:25.000000 nornir_arista-0.0.1/nornir_arista/__init__.py
-drwxr-xr-x   0 vicc     (12511) operations  (6003)        0 2024-05-01 01:33:53.219163 nornir_arista-0.0.1/nornir_arista/connections/
--rw-r--r--   0 vicc     (12511) operations  (6003)      879 2024-04-25 21:33:22.000000 nornir_arista-0.0.1/nornir_arista/connections/__init__.py
-drwxr-xr-x   0 vicc     (12511) operations  (6003)        0 2024-05-01 01:33:53.219163 nornir_arista-0.0.1/nornir_arista/tasks/
--rw-r--r--   0 vicc     (12511) operations  (6003)      130 2024-04-30 22:21:54.000000 nornir_arista-0.0.1/nornir_arista/tasks/__init__.py
--rw-r--r--   0 vicc     (12511) operations  (6003)     3151 2024-05-01 01:25:47.000000 nornir_arista-0.0.1/nornir_arista/tasks/arista_config.py
--rw-r--r--   0 vicc     (12511) operations  (6003)     1463 2024-04-30 23:19:55.000000 nornir_arista-0.0.1/nornir_arista/tasks/arista_get.py
--rw-r--r--   0 vicc     (12511) operations  (6003)      278 2024-04-30 22:22:39.000000 nornir_arista-0.0.1/nornir_arista/tasks/report.py
-drwxr-xr-x   0 vicc     (12511) operations  (6003)        0 2024-05-01 01:33:53.219163 nornir_arista-0.0.1/nornir_arista.egg-info/
--rw-r--r--   0 vicc     (12511) operations  (6003)      637 2024-05-01 01:33:53.000000 nornir_arista-0.0.1/nornir_arista.egg-info/PKG-INFO
--rw-r--r--   0 vicc     (12511) operations  (6003)      399 2024-05-01 01:33:53.000000 nornir_arista-0.0.1/nornir_arista.egg-info/SOURCES.txt
--rw-r--r--   0 vicc     (12511) operations  (6003)        1 2024-05-01 01:33:53.000000 nornir_arista-0.0.1/nornir_arista.egg-info/dependency_links.txt
--rw-r--r--   0 vicc     (12511) operations  (6003)       14 2024-05-01 01:33:53.000000 nornir_arista-0.0.1/nornir_arista.egg-info/requires.txt
--rw-r--r--   0 vicc     (12511) operations  (6003)       14 2024-05-01 01:33:53.000000 nornir_arista-0.0.1/nornir_arista.egg-info/top_level.txt
--rw-r--r--   0 vicc     (12511) operations  (6003)       38 2024-05-01 01:33:53.219163 nornir_arista-0.0.1/setup.cfg
--rw-r--r--   0 vicc     (12511) operations  (6003)     1600 2024-05-01 01:33:40.000000 nornir_arista-0.0.1/setup.py
+drwxr-xr-x   0 vicc     (12511) operations  (6003)        0 2024-05-14 05:39:17.070590 nornir_arista-0.0.2/
+-rw-r--r--   0 vicc     (12511) operations  (6003)      638 2024-05-14 05:39:17.070590 nornir_arista-0.0.2/PKG-INFO
+-rw-r--r--   0 vicc     (12511) operations  (6003)       47 2024-05-01 01:51:08.000000 nornir_arista-0.0.2/README.md
+drwxr-xr-x   0 vicc     (12511) operations  (6003)        0 2024-05-14 05:39:17.070590 nornir_arista-0.0.2/nornir_arista/
+-rw-r--r--   0 vicc     (12511) operations  (6003)       21 2024-05-14 05:39:13.000000 nornir_arista-0.0.2/nornir_arista/__init__.py
+drwxr-xr-x   0 vicc     (12511) operations  (6003)        0 2024-05-14 05:39:17.070590 nornir_arista-0.0.2/nornir_arista/connections/
+-rw-r--r--   0 vicc     (12511) operations  (6003)     1307 2024-05-14 05:35:41.000000 nornir_arista-0.0.2/nornir_arista/connections/__init__.py
+drwxr-xr-x   0 vicc     (12511) operations  (6003)        0 2024-05-14 05:39:17.070590 nornir_arista-0.0.2/nornir_arista/tasks/
+-rw-r--r--   0 vicc     (12511) operations  (6003)      130 2024-05-01 01:51:08.000000 nornir_arista-0.0.2/nornir_arista/tasks/__init__.py
+-rw-r--r--   0 vicc     (12511) operations  (6003)     3151 2024-05-01 01:51:08.000000 nornir_arista-0.0.2/nornir_arista/tasks/arista_config.py
+-rw-r--r--   0 vicc     (12511) operations  (6003)     1463 2024-05-01 01:51:08.000000 nornir_arista-0.0.2/nornir_arista/tasks/arista_get.py
+-rw-r--r--   0 vicc     (12511) operations  (6003)      278 2024-05-01 01:51:08.000000 nornir_arista-0.0.2/nornir_arista/tasks/report.py
+drwxr-xr-x   0 vicc     (12511) operations  (6003)        0 2024-05-14 05:39:17.070590 nornir_arista-0.0.2/nornir_arista.egg-info/
+-rw-r--r--   0 vicc     (12511) operations  (6003)      638 2024-05-14 05:39:16.000000 nornir_arista-0.0.2/nornir_arista.egg-info/PKG-INFO
+-rw-r--r--   0 vicc     (12511) operations  (6003)      399 2024-05-14 05:39:17.000000 nornir_arista-0.0.2/nornir_arista.egg-info/SOURCES.txt
+-rw-r--r--   0 vicc     (12511) operations  (6003)        1 2024-05-14 05:39:16.000000 nornir_arista-0.0.2/nornir_arista.egg-info/dependency_links.txt
+-rw-r--r--   0 vicc     (12511) operations  (6003)       14 2024-05-14 05:39:16.000000 nornir_arista-0.0.2/nornir_arista.egg-info/requires.txt
+-rw-r--r--   0 vicc     (12511) operations  (6003)       14 2024-05-14 05:39:16.000000 nornir_arista-0.0.2/nornir_arista.egg-info/top_level.txt
+-rw-r--r--   0 vicc     (12511) operations  (6003)       38 2024-05-14 05:39:17.070590 nornir_arista-0.0.2/setup.cfg
+-rw-r--r--   0 vicc     (12511) operations  (6003)     1600 2024-05-01 01:51:08.000000 nornir_arista-0.0.2/setup.py
```

### Comparing `nornir_arista-0.0.1/PKG-INFO` & `nornir_arista-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nornir_arista
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library to interact with Arista devices. Based on Arista EAPI
 Home-page: https://github.com/Vicnz03/nornir_arista
 Author: Vic Chen
 Author-email: vicnz03@hotmail.com
 License: MIT
-Description: # nornir_junos
+Description: # nornir_arista
         Arista EAPI Plugins for Nornir
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nornir_arista-0.0.1/nornir_arista/tasks/arista_config.py` & `nornir_arista-0.0.2/nornir_arista/tasks/arista_config.py`

 * *Files identical despite different names*

### Comparing `nornir_arista-0.0.1/nornir_arista/tasks/arista_get.py` & `nornir_arista-0.0.2/nornir_arista/tasks/arista_get.py`

 * *Files identical despite different names*

### Comparing `nornir_arista-0.0.1/nornir_arista.egg-info/PKG-INFO` & `nornir_arista-0.0.2/nornir_arista.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nornir-arista
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library to interact with Arista devices. Based on Arista EAPI
 Home-page: https://github.com/Vicnz03/nornir_arista
 Author: Vic Chen
 Author-email: vicnz03@hotmail.com
 License: MIT
-Description: # nornir_junos
+Description: # nornir_arista
         Arista EAPI Plugins for Nornir
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nornir_arista-0.0.1/setup.py` & `nornir_arista-0.0.2/setup.py`

 * *Files identical despite different names*

