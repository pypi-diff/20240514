# Comparing `tmp/KudraCloudClient-0.0.8.tar.gz` & `tmp/KudraCloudClient-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KudraCloudClient-0.0.8.tar", last modified: Mon Dec 18 15:21:27 2023, max compression
+gzip compressed data, was "KudraCloudClient-0.0.9.tar", last modified: Mon Dec 18 15:24:56 2023, max compression
```

## Comparing `KudraCloudClient-0.0.8.tar` & `KudraCloudClient-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:21:27.877044 KudraCloudClient-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-18 15:21:11.000000 KudraCloudClient-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 15:21:11.000000 KudraCloudClient-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-12-18 15:21:27.877044 KudraCloudClient-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-12-18 15:21:11.000000 KudraCloudClient-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 15:21:11.000000 KudraCloudClient-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-18 15:21:27.877044 KudraCloudClient-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-18 15:21:25.000000 KudraCloudClient-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:21:27.873044 KudraCloudClient-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:21:27.877044 KudraCloudClient-0.0.8/src/KudraCloudClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-12-18 15:21:27.000000 KudraCloudClient-0.0.8/src/KudraCloudClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-18 15:21:27.000000 KudraCloudClient-0.0.8/src/KudraCloudClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 15:21:27.000000 KudraCloudClient-0.0.8/src/KudraCloudClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-18 15:21:27.000000 KudraCloudClient-0.0.8/src/KudraCloudClient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-18 15:21:27.000000 KudraCloudClient-0.0.8/src/KudraCloudClient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:21:27.877044 KudraCloudClient-0.0.8/src/kudra_cloud_client/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-18 15:21:11.000000 KudraCloudClient-0.0.8/src/kudra_cloud_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2023-12-18 15:21:11.000000 KudraCloudClient-0.0.8/src/kudra_cloud_client/kudra_cloud_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:24:56.647837 KudraCloudClient-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-18 15:24:40.000000 KudraCloudClient-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 15:24:40.000000 KudraCloudClient-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-12-18 15:24:56.647837 KudraCloudClient-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-12-18 15:24:40.000000 KudraCloudClient-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 15:24:40.000000 KudraCloudClient-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-18 15:24:56.647837 KudraCloudClient-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-18 15:24:54.000000 KudraCloudClient-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:24:56.647837 KudraCloudClient-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:24:56.647837 KudraCloudClient-0.0.9/src/KudraCloudClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-12-18 15:24:56.000000 KudraCloudClient-0.0.9/src/KudraCloudClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-18 15:24:56.000000 KudraCloudClient-0.0.9/src/KudraCloudClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 15:24:56.000000 KudraCloudClient-0.0.9/src/KudraCloudClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-18 15:24:56.000000 KudraCloudClient-0.0.9/src/KudraCloudClient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-18 15:24:56.000000 KudraCloudClient-0.0.9/src/KudraCloudClient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:24:56.647837 KudraCloudClient-0.0.9/src/kudra_cloud_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-18 15:24:40.000000 KudraCloudClient-0.0.9/src/kudra_cloud_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2023-12-18 15:24:40.000000 KudraCloudClient-0.0.9/src/kudra_cloud_client/kudra_cloud_client.py
```

### Comparing `KudraCloudClient-0.0.8/LICENSE.txt` & `KudraCloudClient-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KudraCloudClient-0.0.8/PKG-INFO` & `KudraCloudClient-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KudraCloudClient
-Version: 0.0.8
+Version: 0.0.9
 Summary: A client for Kudra Cloud
 Home-page: https://github.com/ubiai-incorporated/KudraCloudClient
 Author: UBUAI Inc
 Author-email: admin@ubiai.tools
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ubiai-incorporated/KudraCloudClient
 Description: # Kudra Cloud Client
```

### Comparing `KudraCloudClient-0.0.8/README.md` & `KudraCloudClient-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `KudraCloudClient-0.0.8/setup.cfg` & `KudraCloudClient-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.8
+current_version = 0.0.9
 
 [metadata]
 name = KudraCloudClient
 version = 0.0.3
 author = UBUAI Inc
 author_email = admin@ubiai.tools
 description = A client for Kudra Cloud
```

### Comparing `KudraCloudClient-0.0.8/setup.py` & `KudraCloudClient-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='KudraCloudClient',
-    version='0.0.8',
+    version='0.0.9',
     author='UBUAI Inc',
     author_email='admin@ubiai.tools',
     description='A client for Kudra Cloud',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/ubiai-incorporated/KudraCloudClient",
     project_urls = {
```

### Comparing `KudraCloudClient-0.0.8/src/KudraCloudClient.egg-info/PKG-INFO` & `KudraCloudClient-0.0.9/src/KudraCloudClient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KudraCloudClient
-Version: 0.0.8
+Version: 0.0.9
 Summary: A client for Kudra Cloud
 Home-page: https://github.com/ubiai-incorporated/KudraCloudClient
 Author: UBUAI Inc
 Author-email: admin@ubiai.tools
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ubiai-incorporated/KudraCloudClient
 Description: # Kudra Cloud Client
```

### Comparing `KudraCloudClient-0.0.8/src/kudra_cloud_client/kudra_cloud_client.py` & `KudraCloudClient-0.0.9/src/kudra_cloud_client/kudra_cloud_client.py`

 * *Files identical despite different names*

