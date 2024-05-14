# Comparing `tmp/BL_Python.AWS-0.1.0.tar.gz` & `tmp/bl_python_aws-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BL_Python.AWS-0.1.0.tar", last modified: Wed Feb  7 18:58:01 2024, max compression
+gzip compressed data, was "bl_python_aws-0.2.0.tar", last modified: Tue May 14 21:28:31 2024, max compression
```

## Comparing `BL_Python.AWS-0.1.0.tar` & `bl_python_aws-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:01.849300 BL_Python.AWS-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:01.845301 BL_Python.AWS-0.1.0/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:01.849300 BL_Python.AWS-0.1.0/BL_Python/AWS/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-07 18:57:52.000000 BL_Python.AWS-0.1.0/BL_Python/AWS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:01.849300 BL_Python.AWS-0.1.0/BL_Python.AWS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-07 18:58:01.000000 BL_Python.AWS-0.1.0/BL_Python.AWS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-07 18:58:01.000000 BL_Python.AWS-0.1.0/BL_Python.AWS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 18:58:01.000000 BL_Python.AWS-0.1.0/BL_Python.AWS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-07 18:58:01.000000 BL_Python.AWS-0.1.0/BL_Python.AWS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-07 18:58:01.000000 BL_Python.AWS-0.1.0/BL_Python.AWS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-07 18:57:52.000000 BL_Python.AWS-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-07 18:57:52.000000 BL_Python.AWS-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-07 18:58:01.849300 BL_Python.AWS-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-07 18:57:52.000000 BL_Python.AWS-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:57:52.000000 BL_Python.AWS-0.1.0/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-02-07 18:57:52.000000 BL_Python.AWS-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 18:58:01.849300 BL_Python.AWS-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:28:31.675739 bl_python_aws-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:28:31.675739 bl_python_aws-0.2.0/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:28:31.675739 bl_python_aws-0.2.0/BL_Python/AWS/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:28:27.000000 bl_python_aws-0.2.0/BL_Python/AWS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-14 21:28:27.000000 bl_python_aws-0.2.0/BL_Python/AWS/aws-ssm.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-14 21:28:27.000000 bl_python_aws-0.2.0/BL_Python/AWS/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:28:31.675739 bl_python_aws-0.2.0/BL_Python.AWS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-14 21:28:31.000000 bl_python_aws-0.2.0/BL_Python.AWS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 21:28:31.000000 bl_python_aws-0.2.0/BL_Python.AWS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:28:31.000000 bl_python_aws-0.2.0/BL_Python.AWS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 21:28:31.000000 bl_python_aws-0.2.0/BL_Python.AWS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 21:28:31.000000 bl_python_aws-0.2.0/BL_Python.AWS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 21:28:27.000000 bl_python_aws-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 21:28:27.000000 bl_python_aws-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-14 21:28:31.675739 bl_python_aws-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 21:28:27.000000 bl_python_aws-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:28:27.000000 bl_python_aws-0.2.0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-14 21:28:27.000000 bl_python_aws-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:28:31.675739 bl_python_aws-0.2.0/setup.cfg
```

### Comparing `BL_Python.AWS-0.1.0/BL_Python.AWS.egg-info/PKG-INFO` & `bl_python_aws-0.2.0/BL_Python.AWS.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.AWS
-Version: 0.1.0
+Version: 0.2.0
 Summary: Libraries for working with AWS services in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
@@ -16,12 +16,13 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: boto3
+Requires-Dist: boto3~=1.34
+Requires-Dist: boto3-stubs~=1.34
 
 # `BL_Python.AWS`
 
 Libraries for working with AWS services in Boutros Lab.
```

### Comparing `BL_Python.AWS-0.1.0/LICENSE.md` & `bl_python_aws-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `BL_Python.AWS-0.1.0/PKG-INFO` & `bl_python_aws-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.AWS
-Version: 0.1.0
+Version: 0.2.0
 Summary: Libraries for working with AWS services in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
@@ -16,12 +16,13 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: boto3
+Requires-Dist: boto3~=1.34
+Requires-Dist: boto3-stubs~=1.34
 
 # `BL_Python.AWS`
 
 Libraries for working with AWS services in Boutros Lab.
```

### Comparing `BL_Python.AWS-0.1.0/pyproject.toml` & `bl_python_aws-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "Development Status :: 4 - Beta",
     "Natural Language :: English"
 ]
 
 dependencies = [
-    "boto3"
+    "boto3 ~= 1.34",
+    "boto3-stubs ~= 1.34"
 ]
 
 dynamic = ["version", "readme"]
 [tool.setuptools.dynamic]
 version = {attr = "BL_Python.AWS.__version__"}
 readme = {file = ["README.md"], content-type = "text/markdown"}
 
@@ -45,8 +46,8 @@
 [tool.setuptools.package-dir]
 "BL_Python.AWS" = "BL_Python/AWS"
 
 [tool.setuptools.packages.find]
 exclude = ["build*"]
 
 [tool.setuptools.package-data]
-"BL_Python.AWS" = ["py.typed"]
+"BL_Python.AWS" = ["py.typed", "aws-ssm.ini"]
```

