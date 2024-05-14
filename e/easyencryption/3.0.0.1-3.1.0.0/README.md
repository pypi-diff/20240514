# Comparing `tmp/easyencryption-3.0.0.1.tar.gz` & `tmp/easyencryption-3.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-3.0.0.1.tar", last modified: Tue May 14 01:07:09 2024, max compression
+gzip compressed data, was "easyencryption-3.1.0.0.tar", last modified: Tue May 14 01:41:33 2024, max compression
```

## Comparing `easyencryption-3.0.0.1.tar` & `easyencryption-3.1.0.0.tar`

### file list

```diff
@@ -1,11 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:07:09.029512 easyencryption-3.0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-14 01:07:09.025512 easyencryption-3.0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-14 01:06:55.000000 easyencryption-3.0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:07:09.025512 easyencryption-3.0.0.1/easyencryption.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-14 01:07:09.000000 easyencryption-3.0.0.1/easyencryption.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-14 01:07:09.000000 easyencryption-3.0.0.1/easyencryption.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 01:07:09.000000 easyencryption-3.0.0.1/easyencryption.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:07:09.000000 easyencryption-3.0.0.1/easyencryption.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 01:07:09.000000 easyencryption-3.0.0.1/easyencryption.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:07:09.029512 easyencryption-3.0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-14 01:06:55.000000 easyencryption-3.0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:41:33.577180 easyencryption-3.1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-14 01:41:33.577180 easyencryption-3.1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-14 01:41:29.000000 easyencryption-3.1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:41:33.577180 easyencryption-3.1.0.0/easyencryption/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 01:41:29.000000 easyencryption-3.1.0.0/easyencryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 01:41:29.000000 easyencryption-3.1.0.0/easyencryption/aes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-14 01:41:29.000000 easyencryption-3.1.0.0/easyencryption/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-14 01:41:29.000000 easyencryption-3.1.0.0/easyencryption/blake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-14 01:41:29.000000 easyencryption-3.1.0.0/easyencryption/fernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-14 01:41:29.000000 easyencryption-3.1.0.0/easyencryption/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-14 01:41:29.000000 easyencryption-3.1.0.0/easyencryption/sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-14 01:41:29.000000 easyencryption-3.1.0.0/easyencryption/shake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-14 01:41:29.000000 easyencryption-3.1.0.0/easyencryption/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-14 01:41:29.000000 easyencryption-3.1.0.0/easyencryption/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:41:33.577180 easyencryption-3.1.0.0/easyencryption.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-14 01:41:33.000000 easyencryption-3.1.0.0/easyencryption.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 01:41:33.000000 easyencryption-3.1.0.0/easyencryption.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 01:41:33.000000 easyencryption-3.1.0.0/easyencryption.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:41:33.000000 easyencryption-3.1.0.0/easyencryption.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:41:33.000000 easyencryption-3.1.0.0/easyencryption.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:41:33.577180 easyencryption-3.1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-14 01:41:29.000000 easyencryption-3.1.0.0/setup.py
```

### Comparing `easyencryption-3.0.0.1/PKG-INFO` & `easyencryption-3.1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 3.0.0.1
+Version: 3.1.0.0
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

### Comparing `easyencryption-3.0.0.1/README.md` & `easyencryption-3.1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `easyencryption-3.0.0.1/easyencryption.egg-info/PKG-INFO` & `easyencryption-3.1.0.0/easyencryption.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 3.0.0.1
+Version: 3.1.0.0
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

### Comparing `easyencryption-3.0.0.1/setup.py` & `easyencryption-3.1.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
-version = "3.0.0.1"
+version = "3.1.0.0"
+print(find_packages(include=['easyencryption']))
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

