# Comparing `tmp/encorsa_e_factura-0.2.8.tar.gz` & `tmp/encorsa_e_factura-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encorsa_e_factura-0.2.8.tar", last modified: Thu May  9 16:58:26 2024, max compression
+gzip compressed data, was "encorsa_e_factura-0.2.9.tar", last modified: Tue May 14 21:55:43 2024, max compression
```

## Comparing `encorsa_e_factura-0.2.8.tar` & `encorsa_e_factura-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:58:26.646337 encorsa_e_factura-0.2.8/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-09 16:58:26.646337 encorsa_e_factura-0.2.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-05-09 16:58:23.000000 encorsa_e_factura-0.2.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)      679 2024-05-09 16:58:26.646337 encorsa_e_factura-0.2.8/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:58:26.646337 encorsa_e_factura-0.2.8/src/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:58:26.646337 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/
--rw-r--r--   0 vsts      (1001) docker     (127)     8253 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/WebConRequestUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15963 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/XMLUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      624 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/runLocaly.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24808 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/sincronizare.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:58:26.646337 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-09 16:58:26.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-09 16:58:26.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 16:58:26.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-05-09 16:58:26.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-05-09 16:58:26.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-09 16:58:26.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 21:55:43.577598 encorsa_e_factura-0.2.9/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-14 21:55:43.577598 encorsa_e_factura-0.2.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-05-14 21:55:40.000000 encorsa_e_factura-0.2.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)      679 2024-05-14 21:55:43.577598 encorsa_e_factura-0.2.9/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 21:55:43.577598 encorsa_e_factura-0.2.9/src/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 21:55:43.577598 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8253 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/WebConRequestUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15963 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/XMLUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      624 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/runLocaly.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25044 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/sincronizare.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 21:55:43.577598 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-14 21:55:43.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-14 21:55:43.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-14 21:55:43.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-05-14 21:55:43.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-05-14 21:55:43.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-14 21:55:43.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/top_level.txt
```

### Comparing `encorsa_e_factura-0.2.8/LICENCE` & `encorsa_e_factura-0.2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.8/PKG-INFO` & `encorsa_e_factura-0.2.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Encorsa_e_Factura
-Version: 0.2.8
+Version: 0.2.9
 Summary: A small example package
 Home-page: https://encorsa.ro
 Author: Dan Popescu, Razvan Ogrezeanu
 Author-email: dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `encorsa_e_factura-0.2.8/README.md` & `encorsa_e_factura-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.8/setup.cfg` & `encorsa_e_factura-0.2.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Encorsa_e_Factura
-version = 0.2.8
+version = 0.2.9
 author = Dan Popescu, Razvan Ogrezeanu
 author_email = dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 description = A small example package
 long_description = file: README.md
 url = https://encorsa.ro
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/WebConRequestUtils.py` & `encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/WebConRequestUtils.py`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/XMLUtils.py` & `encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/XMLUtils.py`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/runLocaly.py` & `encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/runLocaly.py`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/sincronizare.py` & `encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/sincronizare.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from datetime import datetime
 import requests
 import zipfile
 from requests.auth import HTTPBasicAuth
 import argparse
 from datetime import datetime
 import re
+import time
 
 try:
     from .XMLUtils import *
 except:
     from XMLUtils import *
 
 try:
@@ -227,26 +228,31 @@
     if "proxi_pt_anaf_http" in parameters and parameters["proxi_pt_anaf_http"]:
         proxies["http"] = parameters["proxi_pt_anaf_http"]
 
     # Retry logic
     max_retries = 5
     attempts = 0
 
+    # Encode the XML data to UTF-8 bytes to ensure compatibility
+    xml_data = xml_data.encode('utf-8')
+
     while attempts < max_retries:
         try:
             response = requests.post(
                 url, headers=headers, data=xml_data, proxies=proxies)
             if response.status_code != 200:
                 response.raise_for_status()
 
             # Directly check if the response is JSON
             if "application/json" in response.headers.get('Content-Type', ''):
-                print("JSON response received, retrying..." +
-                      str(response.content))
+                print("JSON response received, retrying..." + str(response.content))
+                # Print the whole response for debugging
                 attempts += 1
+                # Sleep for 1 second before retrying
+                time.sleep(1)
                 continue
             else:
                 # Assume the response is the binary content of the PDF
                 pdf_content = response.content
                 # Encode the PDF content to Base64
                 base64_encoded_pdf = base64.b64encode(pdf_content)
                 return base64_encoded_pdf.decode('utf-8')
```

### Comparing `encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/PKG-INFO` & `encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Encorsa_e_Factura
-Version: 0.2.8
+Version: 0.2.9
 Summary: A small example package
 Home-page: https://encorsa.ro
 Author: Dan Popescu, Razvan Ogrezeanu
 Author-email: dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

