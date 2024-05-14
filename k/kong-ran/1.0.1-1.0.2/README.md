# Comparing `tmp/kong_ran-1.0.1.tar.gz` & `tmp/kong_ran-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kong_ran-1.0.1.tar", last modified: Tue May 14 09:49:05 2024, max compression
+gzip compressed data, was "kong_ran-1.0.2.tar", last modified: Tue May 14 09:53:45 2024, max compression
```

## Comparing `kong_ran-1.0.1.tar` & `kong_ran-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-14 09:49:05.185820 kong_ran-1.0.1/
--rw-r--r--   0 a08030320   (501) staff       (20)     1073 2024-01-09 12:07:09.000000 kong_ran-1.0.1/LICENSE
--rw-r--r--   0 a08030320   (501) staff       (20)      534 2024-05-14 09:49:05.185398 kong_ran-1.0.1/PKG-INFO
--rw-r--r--   0 a08030320   (501) staff       (20)       75 2024-05-14 09:31:19.000000 kong_ran-1.0.1/README.md
-drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-14 09:49:05.184777 kong_ran-1.0.1/kong_ran.egg-info/
--rw-r--r--   0 a08030320   (501) staff       (20)      534 2024-05-14 09:49:05.000000 kong_ran-1.0.1/kong_ran.egg-info/PKG-INFO
--rw-r--r--   0 a08030320   (501) staff       (20)      206 2024-05-14 09:49:05.000000 kong_ran-1.0.1/kong_ran.egg-info/SOURCES.txt
--rw-r--r--   0 a08030320   (501) staff       (20)        1 2024-05-14 09:49:05.000000 kong_ran-1.0.1/kong_ran.egg-info/dependency_links.txt
--rw-r--r--   0 a08030320   (501) staff       (20)       46 2024-05-14 09:49:05.000000 kong_ran-1.0.1/kong_ran.egg-info/requires.txt
--rw-r--r--   0 a08030320   (501) staff       (20)        9 2024-05-14 09:49:05.000000 kong_ran-1.0.1/kong_ran.egg-info/top_level.txt
-drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-14 09:49:05.184131 kong_ran-1.0.1/kongcore/
--rw-r--r--   0 a08030320   (501) staff       (20)     3989 2024-05-14 06:34:36.000000 kong_ran-1.0.1/kongcore/__init__.py
--rw-r--r--   0 a08030320   (501) staff       (20)       38 2024-05-14 09:49:05.185927 kong_ran-1.0.1/setup.cfg
--rw-r--r--   0 a08030320   (501) staff       (20)     1292 2024-05-14 09:49:04.000000 kong_ran-1.0.1/setup.py
+drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-14 09:53:45.437199 kong_ran-1.0.2/
+-rw-r--r--   0 a08030320   (501) staff       (20)     1073 2024-01-09 12:07:09.000000 kong_ran-1.0.2/LICENSE
+-rw-r--r--   0 a08030320   (501) staff       (20)      534 2024-05-14 09:53:45.436869 kong_ran-1.0.2/PKG-INFO
+-rw-r--r--   0 a08030320   (501) staff       (20)       75 2024-05-14 09:31:19.000000 kong_ran-1.0.2/README.md
+drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-14 09:53:45.436521 kong_ran-1.0.2/kong_ran.egg-info/
+-rw-r--r--   0 a08030320   (501) staff       (20)      534 2024-05-14 09:53:45.000000 kong_ran-1.0.2/kong_ran.egg-info/PKG-INFO
+-rw-r--r--   0 a08030320   (501) staff       (20)      206 2024-05-14 09:53:45.000000 kong_ran-1.0.2/kong_ran.egg-info/SOURCES.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)        1 2024-05-14 09:53:45.000000 kong_ran-1.0.2/kong_ran.egg-info/dependency_links.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)       46 2024-05-14 09:53:45.000000 kong_ran-1.0.2/kong_ran.egg-info/requires.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)        9 2024-05-14 09:53:45.000000 kong_ran-1.0.2/kong_ran.egg-info/top_level.txt
+drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-14 09:53:45.436221 kong_ran-1.0.2/kongcore/
+-rw-r--r--   0 a08030320   (501) staff       (20)     3989 2024-05-14 06:34:36.000000 kong_ran-1.0.2/kongcore/__init__.py
+-rw-r--r--   0 a08030320   (501) staff       (20)       38 2024-05-14 09:53:45.437260 kong_ran-1.0.2/setup.cfg
+-rw-r--r--   0 a08030320   (501) staff       (20)     1292 2024-05-14 09:53:28.000000 kong_ran-1.0.2/setup.py
```

### Comparing `kong_ran-1.0.1/LICENSE` & `kong_ran-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kong_ran-1.0.1/PKG-INFO` & `kong_ran-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: kong_ran
-Version: 1.0.1
+Version: 1.0.2
 Summary: Libraries for encryption and alignment
 Home-page: 
 Author: ranyu
 Author-email: wy176404@163.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx~=0.27.0
+Requires-Dist: httpx~=0.13.3
 Requires-Dist: pyjwt~=1.7.1
 Requires-Dist: sentry-sdk~=1.5.12
 
 # How to use it?
 **description**
 > use kong with your project
```

### Comparing `kong_ran-1.0.1/kong_ran.egg-info/PKG-INFO` & `kong_ran-1.0.2/kong_ran.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: kong_ran
-Version: 1.0.1
+Version: 1.0.2
 Summary: Libraries for encryption and alignment
 Home-page: 
 Author: ranyu
 Author-email: wy176404@163.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx~=0.27.0
+Requires-Dist: httpx~=0.13.3
 Requires-Dist: pyjwt~=1.7.1
 Requires-Dist: sentry-sdk~=1.5.12
 
 # How to use it?
 **description**
 > use kong with your project
```

### Comparing `kong_ran-1.0.1/kongcore/__init__.py` & `kong_ran-1.0.2/kongcore/__init__.py`

 * *Files identical despite different names*

### Comparing `kong_ran-1.0.1/setup.py` & `kong_ran-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="kong_ran",
-    version="1.0.1",
+    version="1.0.2",
     # 作者名
     author="ranyu",
     # 作者邮箱
     author_email="wy176404@163.com",
     # 包的简介描述
     description="Libraries for encryption and alignment",
     # 包的详细介绍(一般通过加载README.md)
@@ -27,12 +27,12 @@
         "Programming Language :: Python :: 3.8",
         # 根据MIT许可证开源
         "License :: OSI Approved :: MIT License",
         # 与操作系统无关
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'httpx~=0.27.0',
+        'httpx~=0.13.3',
         'pyjwt~=1.7.1',
         'sentry-sdk~=1.5.12'
     ]
 )
```

