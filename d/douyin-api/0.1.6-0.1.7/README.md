# Comparing `tmp/douyin-api-0.1.6.tar.gz` & `tmp/douyin-api-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\douyin-api-0.1.6.tar", last modified: Tue Nov 28 06:26:44 2023, max compression
+gzip compressed data, was "dist\douyin-api-0.1.7.tar", last modified: Mon Mar 25 05:52:17 2024, max compression
```

## Comparing `douyin-api-0.1.6.tar` & `douyin-api-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-11-28 06:26:44.000000 douyin-api-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-11-28 06:26:44.000000 douyin-api-0.1.6/douyin_api/
--rw-rw-rw-   0        0        0    13776 2023-10-07 08:25:25.000000 douyin-api-0.1.6/douyin_api/api.py
--rw-rw-rw-   0        0        0      853 2023-08-22 10:24:45.000000 douyin-api-0.1.6/douyin_api/exception.py
--rw-rw-rw-   0        0        0     1876 2023-11-28 06:22:00.000000 douyin-api-0.1.6/douyin_api/tool.py
--rw-rw-rw-   0        0        0     9671 2023-08-23 11:13:46.000000 douyin-api-0.1.6/douyin_api/utils.py
--rw-rw-rw-   0        0        0       22 2023-11-28 06:25:44.000000 douyin-api-0.1.6/douyin_api/_version.py
--rw-rw-rw-   0        0        0       25 2023-08-09 08:37:56.000000 douyin-api-0.1.6/douyin_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-28 06:26:44.000000 douyin-api-0.1.6/douyin_api.egg-info/
--rw-rw-rw-   0        0        0        1 2023-11-28 06:26:44.000000 douyin-api-0.1.6/douyin_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3448 2023-11-28 06:26:44.000000 douyin-api-0.1.6/douyin_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-11-28 06:26:44.000000 douyin-api-0.1.6/douyin_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0      314 2023-11-28 06:26:44.000000 douyin-api-0.1.6/douyin_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2023-11-28 06:26:44.000000 douyin-api-0.1.6/douyin_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3448 2023-11-28 06:26:44.000000 douyin-api-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2260 2023-08-23 11:47:35.000000 douyin-api-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-11-28 06:26:44.000000 douyin-api-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     5166 2023-11-28 06:26:42.000000 douyin-api-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-25 05:52:17.000000 douyin-api-0.1.7/
+drwxrwxrwx   0        0        0        0 2024-03-25 05:52:17.000000 douyin-api-0.1.7/douyin_api/
+-rw-rw-rw-   0        0        0    13776 2023-10-07 08:25:25.000000 douyin-api-0.1.7/douyin_api/api.py
+-rw-rw-rw-   0        0        0      853 2023-08-22 10:24:45.000000 douyin-api-0.1.7/douyin_api/exception.py
+-rw-rw-rw-   0        0        0     2868 2024-03-25 03:58:45.000000 douyin-api-0.1.7/douyin_api/tool.py
+-rw-rw-rw-   0        0        0     9671 2023-08-23 11:13:46.000000 douyin-api-0.1.7/douyin_api/utils.py
+-rw-rw-rw-   0        0        0       22 2024-03-25 04:00:40.000000 douyin-api-0.1.7/douyin_api/_version.py
+-rw-rw-rw-   0        0        0       25 2023-08-09 08:37:56.000000 douyin-api-0.1.7/douyin_api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-25 05:52:17.000000 douyin-api-0.1.7/douyin_api.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-03-25 05:52:16.000000 douyin-api-0.1.7/douyin_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3448 2024-03-25 05:52:16.000000 douyin-api-0.1.7/douyin_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2024-03-25 05:52:16.000000 douyin-api-0.1.7/douyin_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      314 2024-03-25 05:52:16.000000 douyin-api-0.1.7/douyin_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2024-03-25 05:52:16.000000 douyin-api-0.1.7/douyin_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3448 2024-03-25 05:52:17.000000 douyin-api-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2260 2023-08-23 11:47:35.000000 douyin-api-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-25 05:52:17.000000 douyin-api-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     5246 2024-03-25 05:51:24.000000 douyin-api-0.1.7/setup.py
```

### Comparing `douyin-api-0.1.6/douyin_api/api.py` & `douyin-api-0.1.7/douyin_api/api.py`

 * *Files identical despite different names*

### Comparing `douyin-api-0.1.6/douyin_api/exception.py` & `douyin-api-0.1.7/douyin_api/exception.py`

 * *Files identical despite different names*

### Comparing `douyin-api-0.1.6/douyin_api/utils.py` & `douyin-api-0.1.7/douyin_api/utils.py`

 * *Files identical despite different names*

### Comparing `douyin-api-0.1.6/douyin_api.egg-info/PKG-INFO` & `douyin-api-0.1.7/douyin_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: douyin-api
-Version: 0.1.6
+Version: 0.1.7
 Summary: 抖音官方开放接口
 Home-page: https://github.com/ldsxp/douyin-api
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/douyin-api
 Description: # douyin-api
```

### Comparing `douyin-api-0.1.6/PKG-INFO` & `douyin-api-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: douyin-api
-Version: 0.1.6
+Version: 0.1.7
 Summary: 抖音官方开放接口
 Home-page: https://github.com/ldsxp/douyin-api
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/douyin-api
 Description: # douyin-api
```

### Comparing `douyin-api-0.1.6/README.md` & `douyin-api-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `douyin-api-0.1.6/setup.py` & `douyin-api-0.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 # 用这个命令升级：easy_install -U pip
 
 # 检查错误
 # twine check dist/*
 
 echo 使用 twine 上传到官方的pip服务器:
 echo 在系统添加 TWINE_USERNAME 和 TWINE_PASSWORD 变量，不用输入用户名和密码
+echo 例如 TWINE_USERNAME=__token__ TWINE_PASSWORD=pypi-AgEIcHlwaS5vcmcCJD...
 rmdir /S/Q build
 rmdir /S/Q dist
 python setup.py sdist bdist_wheel
 echo 上传到PyPI:
 twine upload dist/*
 """
```

