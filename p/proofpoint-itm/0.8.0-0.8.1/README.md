# Comparing `tmp/proofpoint_itm-0.8.0.tar.gz` & `tmp/proofpoint_itm-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proofpoint_itm-0.8.0.tar", last modified: Fri Oct 20 03:12:06 2023, max compression
+gzip compressed data, was "proofpoint_itm-0.8.1.tar", last modified: Mon May 13 22:45:45 2024, max compression
```

## Comparing `proofpoint_itm-0.8.0.tar` & `proofpoint_itm-0.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-10-20 03:12:06.483391 proofpoint_itm-0.8.0/
--rw-r--r--   0 molden     (501) staff       (20)    11357 2021-11-16 02:23:49.000000 proofpoint_itm-0.8.0/LICENSE
--rw-r--r--   0 molden     (501) staff       (20)     1703 2023-10-20 03:12:06.483329 proofpoint_itm-0.8.0/PKG-INFO
--rw-r--r--   0 molden     (501) staff       (20)     1084 2023-10-20 03:11:09.000000 proofpoint_itm-0.8.0/README.md
--rw-r--r--   0 molden     (501) staff       (20)       74 2023-10-20 03:12:06.483590 proofpoint_itm-0.8.0/setup.cfg
--rw-r--r--   0 molden     (501) staff       (20)      925 2023-10-20 03:09:54.000000 proofpoint_itm-0.8.0/setup.py
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-10-20 03:12:06.480143 proofpoint_itm-0.8.0/src/
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-10-20 03:12:06.482481 proofpoint_itm-0.8.0/src/proofpoint_itm/
--rw-r--r--   0 molden     (501) staff       (20)       43 2022-10-14 21:09:35.000000 proofpoint_itm-0.8.0/src/proofpoint_itm/__init__.py
--rw-r--r--   0 molden     (501) staff       (20)     1686 2023-07-12 23:28:29.000000 proofpoint_itm-0.8.0/src/proofpoint_itm/auth.py
--rw-r--r--   0 molden     (501) staff       (20)    10810 2022-12-13 03:20:50.000000 proofpoint_itm-0.8.0/src/proofpoint_itm/classes.py
--rw-r--r--   0 molden     (501) staff       (20)    59443 2023-10-20 03:07:20.000000 proofpoint_itm-0.8.0/src/proofpoint_itm/client.py
--rw-r--r--   0 molden     (501) staff       (20)     4980 2023-09-13 01:57:32.000000 proofpoint_itm-0.8.0/src/proofpoint_itm/webclient.py
-drwxr-xr-x   0 molden     (501) staff       (20)        0 2023-10-20 03:12:06.483136 proofpoint_itm-0.8.0/src/proofpoint_itm.egg-info/
--rw-r--r--   0 molden     (501) staff       (20)     1703 2023-10-20 03:12:06.000000 proofpoint_itm-0.8.0/src/proofpoint_itm.egg-info/PKG-INFO
--rw-r--r--   0 molden     (501) staff       (20)      353 2023-10-20 03:12:06.000000 proofpoint_itm-0.8.0/src/proofpoint_itm.egg-info/SOURCES.txt
--rw-r--r--   0 molden     (501) staff       (20)        1 2023-10-20 03:12:06.000000 proofpoint_itm-0.8.0/src/proofpoint_itm.egg-info/dependency_links.txt
--rw-r--r--   0 molden     (501) staff       (20)       15 2023-10-20 03:12:06.000000 proofpoint_itm-0.8.0/src/proofpoint_itm.egg-info/top_level.txt
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2024-05-13 22:45:45.048968 proofpoint_itm-0.8.1/
+-rw-r--r--   0 molden     (501) staff       (20)    11357 2021-11-16 02:23:49.000000 proofpoint_itm-0.8.1/LICENSE
+-rw-r--r--   0 molden     (501) staff       (20)     1703 2024-05-13 22:45:45.048911 proofpoint_itm-0.8.1/PKG-INFO
+-rw-r--r--   0 molden     (501) staff       (20)     1084 2024-05-07 04:09:24.000000 proofpoint_itm-0.8.1/README.md
+-rw-r--r--   0 molden     (501) staff       (20)       74 2024-05-13 22:45:45.049175 proofpoint_itm-0.8.1/setup.cfg
+-rw-r--r--   0 molden     (501) staff       (20)      925 2024-05-13 22:44:24.000000 proofpoint_itm-0.8.1/setup.py
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2024-05-13 22:45:45.046363 proofpoint_itm-0.8.1/src/
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2024-05-13 22:45:45.047998 proofpoint_itm-0.8.1/src/proofpoint_itm/
+-rw-r--r--   0 molden     (501) staff       (20)       43 2022-10-14 21:09:35.000000 proofpoint_itm-0.8.1/src/proofpoint_itm/__init__.py
+-rw-r--r--   0 molden     (501) staff       (20)     1686 2023-07-12 23:28:29.000000 proofpoint_itm-0.8.1/src/proofpoint_itm/auth.py
+-rw-r--r--   0 molden     (501) staff       (20)    10810 2022-12-13 03:20:50.000000 proofpoint_itm-0.8.1/src/proofpoint_itm/classes.py
+-rw-r--r--   0 molden     (501) staff       (20)    59443 2024-05-13 22:11:20.000000 proofpoint_itm-0.8.1/src/proofpoint_itm/client.py
+-rw-r--r--   0 molden     (501) staff       (20)     4992 2024-05-13 22:44:24.000000 proofpoint_itm-0.8.1/src/proofpoint_itm/webclient.py
+drwxr-xr-x   0 molden     (501) staff       (20)        0 2024-05-13 22:45:45.048722 proofpoint_itm-0.8.1/src/proofpoint_itm.egg-info/
+-rw-r--r--   0 molden     (501) staff       (20)     1703 2024-05-13 22:45:45.000000 proofpoint_itm-0.8.1/src/proofpoint_itm.egg-info/PKG-INFO
+-rw-r--r--   0 molden     (501) staff       (20)      353 2024-05-13 22:45:45.000000 proofpoint_itm-0.8.1/src/proofpoint_itm.egg-info/SOURCES.txt
+-rw-r--r--   0 molden     (501) staff       (20)        1 2024-05-13 22:45:45.000000 proofpoint_itm-0.8.1/src/proofpoint_itm.egg-info/dependency_links.txt
+-rw-r--r--   0 molden     (501) staff       (20)       15 2024-05-13 22:45:45.000000 proofpoint_itm-0.8.1/src/proofpoint_itm.egg-info/top_level.txt
```

### Comparing `proofpoint_itm-0.8.0/LICENSE` & `proofpoint_itm-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.8.0/PKG-INFO` & `proofpoint_itm-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proofpoint_itm
-Version: 0.8.0
+Version: 0.8.1
 Summary: Proofpoint ITM API client library
 Home-page: https://github.com/drizzo-tech/proofpoint_itm
 Author: Mike Olden
 Author-email: michael.olden@oldendigital.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/drizzo-tech/proofpoint_itm/issues
 Keywords: Proofpoint ITM,Proofpoint,ITM,ObserveIT
```

### Comparing `proofpoint_itm-0.8.0/README.md` & `proofpoint_itm-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.8.0/setup.py` & `proofpoint_itm-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(name='proofpoint_itm',
-    version='0.8.0',
+    version='0.8.1',
     description='Proofpoint ITM API client library',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Mike Olden',
     author_email='michael.olden@oldendigital.com',
     url = 'https://github.com/drizzo-tech/proofpoint_itm',
     project_urls={
```

### Comparing `proofpoint_itm-0.8.0/src/proofpoint_itm/auth.py` & `proofpoint_itm-0.8.1/src/proofpoint_itm/auth.py`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.8.0/src/proofpoint_itm/classes.py` & `proofpoint_itm-0.8.1/src/proofpoint_itm/classes.py`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.8.0/src/proofpoint_itm/client.py` & `proofpoint_itm-0.8.1/src/proofpoint_itm/client.py`

 * *Files identical despite different names*

### Comparing `proofpoint_itm-0.8.0/src/proofpoint_itm/webclient.py` & `proofpoint_itm-0.8.1/src/proofpoint_itm/webclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     Returns:
         dict: Response from the request.
     """
     if params:
         url_params = urlencode(params)
         url = url + '?' + url_params
 
-    if json_data:
+    if json_data is not None:
         headers['Content-Type'] = 'application/json; charset=utf-8'
         data = json.dumps(json_data)
         data = data.encode('utf-8')
     elif data:
         data = urlencode(data)
         data = data.encode('utf-8')
```

### Comparing `proofpoint_itm-0.8.0/src/proofpoint_itm.egg-info/PKG-INFO` & `proofpoint_itm-0.8.1/src/proofpoint_itm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: proofpoint-itm
-Version: 0.8.0
+Name: proofpoint_itm
+Version: 0.8.1
 Summary: Proofpoint ITM API client library
 Home-page: https://github.com/drizzo-tech/proofpoint_itm
 Author: Mike Olden
 Author-email: michael.olden@oldendigital.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/drizzo-tech/proofpoint_itm/issues
 Keywords: Proofpoint ITM,Proofpoint,ITM,ObserveIT
```

