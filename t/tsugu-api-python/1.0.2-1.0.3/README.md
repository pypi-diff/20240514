# Comparing `tmp/tsugu-api-python-1.0.2.tar.gz` & `tmp/tsugu-api-python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-1.0.2.tar", last modified: Mon May 13 09:10:12 2024, max compression
+gzip compressed data, was "tsugu-api-python-1.0.3.tar", last modified: Tue May 14 08:29:34 2024, max compression
```

## Comparing `tsugu-api-python-1.0.2.tar` & `tsugu-api-python-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:10:12.508735 tsugu-api-python-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-13 09:10:12.508735 tsugu-api-python-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:10:12.508735 tsugu-api-python-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:10:12.508735 tsugu-api-python-1.0.2/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:10:12.508735 tsugu-api-python-1.0.2/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-13 09:10:04.000000 tsugu-api-python-1.0.2/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:10:12.508735 tsugu-api-python-1.0.2/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-13 09:10:12.000000 tsugu-api-python-1.0.2/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-13 09:10:12.000000 tsugu-api-python-1.0.2/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:10:12.000000 tsugu-api-python-1.0.2/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 09:10:12.000000 tsugu-api-python-1.0.2/tsugu_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 09:10:12.000000 tsugu-api-python-1.0.2/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:29:34.480145 tsugu-api-python-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-14 08:29:34.480145 tsugu-api-python-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:29:34.480145 tsugu-api-python-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:29:34.476145 tsugu-api-python-1.0.3/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:29:34.476145 tsugu-api-python-1.0.3/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api_async/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api_async/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api_async/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api_async/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-14 08:29:24.000000 tsugu-api-python-1.0.3/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:29:34.480145 tsugu-api-python-1.0.3/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-14 08:29:34.000000 tsugu-api-python-1.0.3/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-14 08:29:34.000000 tsugu-api-python-1.0.3/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:29:34.000000 tsugu-api-python-1.0.3/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 08:29:34.000000 tsugu-api-python-1.0.3/tsugu_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 08:29:34.000000 tsugu-api-python-1.0.3/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-1.0.2/LICENSE` & `tsugu-api-python-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/PKG-INFO` & `tsugu-api-python-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.2 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.3 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.0.2/README.md` & `tsugu-api-python-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/setup.py` & `tsugu-api-python-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='1.0.2',
+    version='1.0.3',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-1.0.2/tsugu_api/__init__.py` & `tsugu-api-python-1.0.3/tsugu_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api/_bandoristation.py` & `tsugu-api-python-1.0.3/tsugu_api/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api/_network.py` & `tsugu-api-python-1.0.3/tsugu_api/_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         request = Request(
             method,
             self.url,
             params=params,
             data=cast(dict, dumps(data)) if data is not None else data,
             headers=headers
         )
-        print(data)
+        
         # 构建代理服务器字典
         if self.proxy:
             proxies = settings._get_proxy()
         else:
             proxies = None
         
         # 发送请求并获取响应
```

### Comparing `tsugu-api-python-1.0.2/tsugu_api/_station.py` & `tsugu-api-python-1.0.3/tsugu_api/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api/_tsugu.py` & `tsugu-api-python-1.0.3/tsugu_api/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api/_typing.py` & `tsugu-api-python-1.0.3/tsugu_api/_typing.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api/_user.py` & `tsugu-api-python-1.0.3/tsugu_api/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api/settings.py` & `tsugu-api-python-1.0.3/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api/utils.py` & `tsugu-api-python-1.0.3/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api_async/__init__.py` & `tsugu-api-python-1.0.3/tsugu_api_async/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api_async/_bandoristation.py` & `tsugu-api-python-1.0.3/tsugu_api_async/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api_async/_network.py` & `tsugu-api-python-1.0.3/tsugu_api_async/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api_async/_station.py` & `tsugu-api-python-1.0.3/tsugu_api_async/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api_async/_tsugu.py` & `tsugu-api-python-1.0.3/tsugu_api_async/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api_async/_typing.py` & `tsugu-api-python-1.0.3/tsugu_api_async/_typing.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api_async/_user.py` & `tsugu-api-python-1.0.3/tsugu_api_async/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api_async/settings.py` & `tsugu-api-python-1.0.3/tsugu_api_async/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api_async/utils.py` & `tsugu-api-python-1.0.3/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.2/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-1.0.3/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.2 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.3 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.0.2/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-1.0.3/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

