# Comparing `tmp/eip712-clearsign-1.1.2.tar.gz` & `tmp/eip712_clearsign-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eip712-clearsign-1.1.2.tar", last modified: Thu Nov 24 15:42:26 2022, max compression
+gzip compressed data, was "eip712_clearsign-1.1.3.tar", last modified: Tue May 14 18:57:21 2024, max compression
```

## Comparing `eip712-clearsign-1.1.2.tar` & `eip712_clearsign-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 15:42:26.143401 eip712-clearsign-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2022-11-24 15:41:33.000000 eip712-clearsign-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2405 2022-11-24 15:42:26.143401 eip712-clearsign-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2022-11-24 15:41:33.000000 eip712-clearsign-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 15:42:26.139401 eip712-clearsign-1.1.2/eip712/
--rw-r--r--   0 runner    (1001) docker     (122)     6134 2022-11-24 15:41:33.000000 eip712-clearsign-1.1.2/eip712/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 15:42:26.143401 eip712-clearsign-1.1.2/eip712_clearsign.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2405 2022-11-24 15:42:26.000000 eip712-clearsign-1.1.2/eip712_clearsign.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      244 2022-11-24 15:42:26.000000 eip712-clearsign-1.1.2/eip712_clearsign.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 15:42:26.000000 eip712-clearsign-1.1.2/eip712_clearsign.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-24 15:42:26.000000 eip712-clearsign-1.1.2/eip712_clearsign.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2022-11-24 15:42:26.000000 eip712-clearsign-1.1.2/eip712_clearsign.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 15:42:26.143401 eip712-clearsign-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      717 2022-11-24 15:41:33.000000 eip712-clearsign-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-14 18:57:21.323648 eip712_clearsign-1.1.3/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1063 2024-05-14 18:55:59.000000 eip712_clearsign-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)     2429 2024-05-14 18:57:21.323648 eip712_clearsign-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2024-05-14 18:55:59.000000 eip712_clearsign-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-14 18:57:21.323648 eip712_clearsign-1.1.3/eip712/
+-rw-r--r--   0 runner    (1001) runner    (1001)     6134 2024-05-14 18:55:59.000000 eip712_clearsign-1.1.3/eip712/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-14 18:57:21.323648 eip712_clearsign-1.1.3/eip712_clearsign.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2429 2024-05-14 18:57:21.000000 eip712_clearsign-1.1.3/eip712_clearsign.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      265 2024-05-14 18:57:21.000000 eip712_clearsign-1.1.3/eip712_clearsign.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-14 18:57:21.000000 eip712_clearsign-1.1.3/eip712_clearsign.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-05-14 18:57:21.000000 eip712_clearsign-1.1.3/eip712_clearsign.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        7 2024-05-14 18:57:21.000000 eip712_clearsign-1.1.3/eip712_clearsign.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-05-14 18:57:21.323648 eip712_clearsign-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)      717 2024-05-14 18:55:59.000000 eip712_clearsign-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-14 18:57:21.323648 eip712_clearsign-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) runner    (1001)    10587 2024-05-14 18:55:59.000000 eip712_clearsign-1.1.3/tests/test_eip712.py
```

### Comparing `eip712-clearsign-1.1.2/LICENSE` & `eip712_clearsign-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eip712-clearsign-1.1.2/PKG-INFO` & `eip712_clearsign-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: eip712-clearsign
-Version: 1.1.2
+Version: 1.1.3
 Summary: Parse eip712 clear sign descriptors
 Home-page: https://github.com/LedgerHQ/python-eip712
 Author: Ledger
 Author-email: hello@ledger.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydantic
 
 # python-eip712
 
 Parse eip712 clear sign descriptors.
 
 ## Install
```

### Comparing `eip712-clearsign-1.1.2/README.md` & `eip712_clearsign-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `eip712-clearsign-1.1.2/eip712/__init__.py` & `eip712_clearsign-1.1.3/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `eip712-clearsign-1.1.2/eip712_clearsign.egg-info/PKG-INFO` & `eip712_clearsign-1.1.3/eip712_clearsign.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: eip712-clearsign
-Version: 1.1.2
+Version: 1.1.3
 Summary: Parse eip712 clear sign descriptors
 Home-page: https://github.com/LedgerHQ/python-eip712
 Author: Ledger
 Author-email: hello@ledger.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydantic
 
 # python-eip712
 
 Parse eip712 clear sign descriptors.
 
 ## Install
```

### Comparing `eip712-clearsign-1.1.2/setup.py` & `eip712_clearsign-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="eip712-clearsign",
-    version="1.1.2",
+    version="1.1.3",
     url="https://github.com/LedgerHQ/python-eip712",
     author="Ledger",
     author_email="hello@ledger.com",
     description="Parse eip712 clear sign descriptors",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["pydantic"],
```

