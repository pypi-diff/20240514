# Comparing `tmp/kong_ran-1.0.2.tar.gz` & `tmp/kong_ran-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kong_ran-1.0.2.tar", last modified: Tue May 14 09:53:45 2024, max compression
+gzip compressed data, was "kong_ran-1.0.3.tar", last modified: Tue May 14 10:30:57 2024, max compression
```

## Comparing `kong_ran-1.0.2.tar` & `kong_ran-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-14 09:53:45.437199 kong_ran-1.0.2/
--rw-r--r--   0 a08030320   (501) staff       (20)     1073 2024-01-09 12:07:09.000000 kong_ran-1.0.2/LICENSE
--rw-r--r--   0 a08030320   (501) staff       (20)      534 2024-05-14 09:53:45.436869 kong_ran-1.0.2/PKG-INFO
--rw-r--r--   0 a08030320   (501) staff       (20)       75 2024-05-14 09:31:19.000000 kong_ran-1.0.2/README.md
-drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-14 09:53:45.436521 kong_ran-1.0.2/kong_ran.egg-info/
--rw-r--r--   0 a08030320   (501) staff       (20)      534 2024-05-14 09:53:45.000000 kong_ran-1.0.2/kong_ran.egg-info/PKG-INFO
--rw-r--r--   0 a08030320   (501) staff       (20)      206 2024-05-14 09:53:45.000000 kong_ran-1.0.2/kong_ran.egg-info/SOURCES.txt
--rw-r--r--   0 a08030320   (501) staff       (20)        1 2024-05-14 09:53:45.000000 kong_ran-1.0.2/kong_ran.egg-info/dependency_links.txt
--rw-r--r--   0 a08030320   (501) staff       (20)       46 2024-05-14 09:53:45.000000 kong_ran-1.0.2/kong_ran.egg-info/requires.txt
--rw-r--r--   0 a08030320   (501) staff       (20)        9 2024-05-14 09:53:45.000000 kong_ran-1.0.2/kong_ran.egg-info/top_level.txt
-drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-14 09:53:45.436221 kong_ran-1.0.2/kongcore/
--rw-r--r--   0 a08030320   (501) staff       (20)     3989 2024-05-14 06:34:36.000000 kong_ran-1.0.2/kongcore/__init__.py
--rw-r--r--   0 a08030320   (501) staff       (20)       38 2024-05-14 09:53:45.437260 kong_ran-1.0.2/setup.cfg
--rw-r--r--   0 a08030320   (501) staff       (20)     1292 2024-05-14 09:53:28.000000 kong_ran-1.0.2/setup.py
+drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-14 10:30:57.064165 kong_ran-1.0.3/
+-rw-r--r--   0 a08030320   (501) staff       (20)     1073 2024-01-09 12:07:09.000000 kong_ran-1.0.3/LICENSE
+-rw-r--r--   0 a08030320   (501) staff       (20)      534 2024-05-14 10:30:57.063863 kong_ran-1.0.3/PKG-INFO
+-rw-r--r--   0 a08030320   (501) staff       (20)       75 2024-05-14 09:31:19.000000 kong_ran-1.0.3/README.md
+drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-14 10:30:57.063567 kong_ran-1.0.3/kong_ran.egg-info/
+-rw-r--r--   0 a08030320   (501) staff       (20)      534 2024-05-14 10:30:57.000000 kong_ran-1.0.3/kong_ran.egg-info/PKG-INFO
+-rw-r--r--   0 a08030320   (501) staff       (20)      206 2024-05-14 10:30:57.000000 kong_ran-1.0.3/kong_ran.egg-info/SOURCES.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)        1 2024-05-14 10:30:57.000000 kong_ran-1.0.3/kong_ran.egg-info/dependency_links.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)       46 2024-05-14 10:30:57.000000 kong_ran-1.0.3/kong_ran.egg-info/requires.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)        9 2024-05-14 10:30:57.000000 kong_ran-1.0.3/kong_ran.egg-info/top_level.txt
+drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-14 10:30:57.063310 kong_ran-1.0.3/kongcore/
+-rw-r--r--   0 a08030320   (501) staff       (20)     3995 2024-05-14 10:30:53.000000 kong_ran-1.0.3/kongcore/__init__.py
+-rw-r--r--   0 a08030320   (501) staff       (20)       38 2024-05-14 10:30:57.064230 kong_ran-1.0.3/setup.cfg
+-rw-r--r--   0 a08030320   (501) staff       (20)     1292 2024-05-14 10:30:53.000000 kong_ran-1.0.3/setup.py
```

### Comparing `kong_ran-1.0.2/LICENSE` & `kong_ran-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kong_ran-1.0.2/PKG-INFO` & `kong_ran-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kong_ran
-Version: 1.0.2
+Version: 1.0.3
 Summary: Libraries for encryption and alignment
 Home-page: 
 Author: ranyu
 Author-email: wy176404@163.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kong_ran-1.0.2/kong_ran.egg-info/PKG-INFO` & `kong_ran-1.0.3/kong_ran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kong_ran
-Version: 1.0.2
+Version: 1.0.3
 Summary: Libraries for encryption and alignment
 Home-page: 
 Author: ranyu
 Author-email: wy176404@163.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kong_ran-1.0.2/kongcore/__init__.py` & `kong_ran-1.0.3/kongcore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
                 r = await client.request(method, url, json=json)
 
                 if r.status_code == 204:
                     return r.status_code, None
                 if r.status_code != 200 and r.status_code != 201:
                     return r.status_code, r.json()
                 return IError.Ok.value, r.json()
-        except httpx.ConnectError as e:
-            sentry_sdk.capture_exception(e)
-            return IError.Request_Kong_Error.value, None
+        # except httpx.ConnectError as e:
+        #     sentry_sdk.capture_exception(e)
+        #     return IError.Request_Kong_Error.value, None
         except Exception as e:
             sentry_sdk.capture_exception(e)
             return IError.Request_Kong_Error.value, None
 
     async def get_consumer(self, username) -> (int, ConsumerModel):
         path = f"/consumers/{username}"
         ret, j = await self.request("get", path)
```

### Comparing `kong_ran-1.0.2/setup.py` & `kong_ran-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="kong_ran",
-    version="1.0.2",
+    version="1.0.3",
     # 作者名
     author="ranyu",
     # 作者邮箱
     author_email="wy176404@163.com",
     # 包的简介描述
     description="Libraries for encryption and alignment",
     # 包的详细介绍(一般通过加载README.md)
```

