# Comparing `tmp/nbp_sdk-0.1.4.tar.gz` & `tmp/nbp_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbp_sdk-0.1.4.tar", last modified: Wed May  1 16:18:17 2024, max compression
+gzip compressed data, was "nbp_sdk-0.1.5.tar", last modified: Tue May 14 12:00:42 2024, max compression
```

## Comparing `nbp_sdk-0.1.4.tar` & `nbp_sdk-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2024-05-01 16:18:17.386484 nbp_sdk-0.1.4/
--rw-r--r--   0 lukas      (501) staff       (20)     1071 2024-03-19 10:02:52.000000 nbp_sdk-0.1.4/LICENSE
--rw-r--r--   0 lukas      (501) staff       (20)     3764 2024-05-01 16:18:17.386291 nbp_sdk-0.1.4/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)     3251 2024-03-19 10:22:43.000000 nbp_sdk-0.1.4/README.md
--rw-r--r--   0 lukas      (501) staff       (20)      544 2024-05-01 16:17:22.000000 nbp_sdk-0.1.4/pyproject.toml
--rw-r--r--   0 lukas      (501) staff       (20)       38 2024-05-01 16:18:17.386522 nbp_sdk-0.1.4/setup.cfg
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2024-05-01 16:18:17.381518 nbp_sdk-0.1.4/src/
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2024-05-01 16:18:17.384895 nbp_sdk-0.1.4/src/nbp_sdk/
--rw-r--r--   0 lukas      (501) staff       (20)       79 2024-03-19 10:02:52.000000 nbp_sdk-0.1.4/src/nbp_sdk/_exceptions.py
--rw-r--r--   0 lukas      (501) staff       (20)      549 2024-03-19 10:02:52.000000 nbp_sdk-0.1.4/src/nbp_sdk/_request.py
--rw-r--r--   0 lukas      (501) staff       (20)       25 2024-03-19 10:02:52.000000 nbp_sdk-0.1.4/src/nbp_sdk/_settings.py
--rw-r--r--   0 lukas      (501) staff       (20)      842 2024-03-19 10:03:56.000000 nbp_sdk-0.1.4/src/nbp_sdk/_urls.py
--rw-r--r--   0 lukas      (501) staff       (20)      713 2024-03-19 10:02:52.000000 nbp_sdk-0.1.4/src/nbp_sdk/_utils.py
--rw-r--r--   0 lukas      (501) staff       (20)     7340 2024-03-19 10:20:13.000000 nbp_sdk-0.1.4/src/nbp_sdk/client.py
--rw-r--r--   0 lukas      (501) staff       (20)      999 2024-03-19 10:18:16.000000 nbp_sdk-0.1.4/src/nbp_sdk/models.py
--rw-r--r--   0 lukas      (501) staff       (20)      394 2024-03-19 10:02:52.000000 nbp_sdk-0.1.4/src/nbp_sdk/types.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2024-05-01 16:18:17.386079 nbp_sdk-0.1.4/src/nbp_sdk.egg-info/
--rw-r--r--   0 lukas      (501) staff       (20)     3764 2024-05-01 16:18:17.000000 nbp_sdk-0.1.4/src/nbp_sdk.egg-info/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)      411 2024-05-01 16:18:17.000000 nbp_sdk-0.1.4/src/nbp_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 lukas      (501) staff       (20)        1 2024-05-01 16:18:17.000000 nbp_sdk-0.1.4/src/nbp_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 lukas      (501) staff       (20)       17 2024-05-01 16:18:17.000000 nbp_sdk-0.1.4/src/nbp_sdk.egg-info/requires.txt
--rw-r--r--   0 lukas      (501) staff       (20)        8 2024-05-01 16:18:17.000000 nbp_sdk-0.1.4/src/nbp_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2024-05-01 16:18:17.385872 nbp_sdk-0.1.4/tests/
--rw-r--r--   0 lukas      (501) staff       (20)     3376 2024-03-19 10:21:22.000000 nbp_sdk-0.1.4/tests/test_client.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2024-05-14 12:00:42.486587 nbp_sdk-0.1.5/
+-rw-r--r--   0 lukas      (501) staff       (20)     1071 2024-03-19 10:02:52.000000 nbp_sdk-0.1.5/LICENSE
+-rw-r--r--   0 lukas      (501) staff       (20)     3917 2024-05-14 12:00:42.486405 nbp_sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)     3251 2024-03-19 10:22:43.000000 nbp_sdk-0.1.5/README.md
+-rw-r--r--   0 lukas      (501) staff       (20)      682 2024-05-14 11:58:05.000000 nbp_sdk-0.1.5/pyproject.toml
+-rw-r--r--   0 lukas      (501) staff       (20)       38 2024-05-14 12:00:42.486622 nbp_sdk-0.1.5/setup.cfg
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2024-05-14 12:00:42.484047 nbp_sdk-0.1.5/src/
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2024-05-14 12:00:42.485404 nbp_sdk-0.1.5/src/nbp_sdk/
+-rw-r--r--   0 lukas      (501) staff       (20)       79 2024-03-19 10:02:52.000000 nbp_sdk-0.1.5/src/nbp_sdk/_exceptions.py
+-rw-r--r--   0 lukas      (501) staff       (20)      549 2024-03-19 10:02:52.000000 nbp_sdk-0.1.5/src/nbp_sdk/_request.py
+-rw-r--r--   0 lukas      (501) staff       (20)       25 2024-03-19 10:02:52.000000 nbp_sdk-0.1.5/src/nbp_sdk/_settings.py
+-rw-r--r--   0 lukas      (501) staff       (20)      842 2024-03-19 10:03:56.000000 nbp_sdk-0.1.5/src/nbp_sdk/_urls.py
+-rw-r--r--   0 lukas      (501) staff       (20)      713 2024-03-19 10:02:52.000000 nbp_sdk-0.1.5/src/nbp_sdk/_utils.py
+-rw-r--r--   0 lukas      (501) staff       (20)     7340 2024-03-19 10:20:13.000000 nbp_sdk-0.1.5/src/nbp_sdk/client.py
+-rw-r--r--   0 lukas      (501) staff       (20)      999 2024-03-19 10:18:16.000000 nbp_sdk-0.1.5/src/nbp_sdk/models.py
+-rw-r--r--   0 lukas      (501) staff       (20)      394 2024-03-19 10:02:52.000000 nbp_sdk-0.1.5/src/nbp_sdk/types.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2024-05-14 12:00:42.486225 nbp_sdk-0.1.5/src/nbp_sdk.egg-info/
+-rw-r--r--   0 lukas      (501) staff       (20)     3917 2024-05-14 12:00:42.000000 nbp_sdk-0.1.5/src/nbp_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)      411 2024-05-14 12:00:42.000000 nbp_sdk-0.1.5/src/nbp_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas      (501) staff       (20)        1 2024-05-14 12:00:42.000000 nbp_sdk-0.1.5/src/nbp_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas      (501) staff       (20)       17 2024-05-14 12:00:42.000000 nbp_sdk-0.1.5/src/nbp_sdk.egg-info/requires.txt
+-rw-r--r--   0 lukas      (501) staff       (20)        8 2024-05-14 12:00:42.000000 nbp_sdk-0.1.5/src/nbp_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2024-05-14 12:00:42.486066 nbp_sdk-0.1.5/tests/
+-rw-r--r--   0 lukas      (501) staff       (20)     3376 2024-03-19 10:21:22.000000 nbp_sdk-0.1.5/tests/test_client.py
```

### Comparing `nbp_sdk-0.1.4/LICENSE` & `nbp_sdk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nbp_sdk-0.1.4/PKG-INFO` & `nbp_sdk-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: nbp-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Plain simple SDK for Polish National Bank (NBP) currency rate
 Author-email: Łukasz Klim <lukasz.klim92@gmail.com>
 Project-URL: Homepage, https://github.com/lukas346/nbp_sdk
 Project-URL: Issues, https://github.com/lukas346/nbp_sdk/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
 # NBP SDK
```

### Comparing `nbp_sdk-0.1.4/README.md` & `nbp_sdk-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nbp_sdk-0.1.4/src/nbp_sdk/_request.py` & `nbp_sdk-0.1.5/src/nbp_sdk/_request.py`

 * *Files identical despite different names*

### Comparing `nbp_sdk-0.1.4/src/nbp_sdk/_urls.py` & `nbp_sdk-0.1.5/src/nbp_sdk/_urls.py`

 * *Files identical despite different names*

### Comparing `nbp_sdk-0.1.4/src/nbp_sdk/_utils.py` & `nbp_sdk-0.1.5/src/nbp_sdk/_utils.py`

 * *Files identical despite different names*

### Comparing `nbp_sdk-0.1.4/src/nbp_sdk/client.py` & `nbp_sdk-0.1.5/src/nbp_sdk/client.py`

 * *Files identical despite different names*

### Comparing `nbp_sdk-0.1.4/src/nbp_sdk/models.py` & `nbp_sdk-0.1.5/src/nbp_sdk/models.py`

 * *Files identical despite different names*

### Comparing `nbp_sdk-0.1.4/src/nbp_sdk.egg-info/PKG-INFO` & `nbp_sdk-0.1.5/src/nbp_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: nbp-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Plain simple SDK for Polish National Bank (NBP) currency rate
 Author-email: Łukasz Klim <lukasz.klim92@gmail.com>
 Project-URL: Homepage, https://github.com/lukas346/nbp_sdk
 Project-URL: Issues, https://github.com/lukas346/nbp_sdk/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
 # NBP SDK
```

### Comparing `nbp_sdk-0.1.4/tests/test_client.py` & `nbp_sdk-0.1.5/tests/test_client.py`

 * *Files identical despite different names*

