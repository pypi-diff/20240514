# Comparing `tmp/translate_util-1.1.3.tar.gz` & `tmp/translate_util-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/translate_util-1.1.3.tar", last modified: Sat May 11 03:08:36 2024, max compression
+gzip compressed data, was "dist/translate_util-1.1.4.tar", last modified: Tue May 14 12:02:28 2024, max compression
```

## Comparing `translate_util-1.1.3.tar` & `translate_util-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-11 03:08:36.000000 translate_util-1.1.3/
--rw-r--r--   0 admin      (501) staff       (20)     1796 2024-05-11 03:08:36.000000 translate_util-1.1.3/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      791 2024-05-11 03:02:15.000000 translate_util-1.1.3/README.md
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-05-11 03:08:36.000000 translate_util-1.1.3/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1158 2024-05-11 03:08:25.000000 translate_util-1.1.3/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-11 03:08:36.000000 translate_util-1.1.3/translate_util/
--rw-r--r--   0 admin      (501) staff       (20)       60 2020-06-12 15:15:27.000000 translate_util-1.1.3/translate_util/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      713 2024-05-06 03:30:42.000000 translate_util-1.1.3/translate_util/base_translate.py
--rw-r--r--   0 admin      (501) staff       (20)      756 2020-06-13 13:57:02.000000 translate_util-1.1.3/translate_util/common_request.py
--rw-r--r--   0 admin      (501) staff       (20)     5817 2022-08-24 03:09:35.000000 translate_util-1.1.3/translate_util/translate_baidu.py
--rw-r--r--   0 admin      (501) staff       (20)     2957 2024-05-11 03:08:25.000000 translate_util-1.1.3/translate_util/translate_google.py
--rw-r--r--   0 admin      (501) staff       (20)     1608 2022-08-24 03:14:57.000000 translate_util-1.1.3/translate_util/translate_iciba.py
--rw-r--r--   0 admin      (501) staff       (20)     4178 2024-05-06 03:55:52.000000 translate_util-1.1.3/translate_util/translate_tool.py
--rw-r--r--   0 admin      (501) staff       (20)     1801 2022-08-24 03:16:53.000000 translate_util-1.1.3/translate_util/translate_youdao.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-11 03:08:36.000000 translate_util-1.1.3/translate_util.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1796 2024-05-11 03:08:36.000000 translate_util-1.1.3/translate_util.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      471 2024-05-11 03:08:36.000000 translate_util-1.1.3/translate_util.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-05-11 03:08:36.000000 translate_util-1.1.3/translate_util.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       63 2024-05-11 03:08:36.000000 translate_util-1.1.3/translate_util.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       15 2024-05-11 03:08:36.000000 translate_util-1.1.3/translate_util.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-14 12:02:28.000000 translate_util-1.1.4/
+-rw-r--r--   0 admin      (501) staff       (20)     1796 2024-05-14 12:02:28.000000 translate_util-1.1.4/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      791 2024-05-11 03:02:15.000000 translate_util-1.1.4/README.md
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-05-14 12:02:28.000000 translate_util-1.1.4/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1158 2024-05-14 12:00:54.000000 translate_util-1.1.4/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-14 12:02:28.000000 translate_util-1.1.4/translate_util/
+-rw-r--r--   0 admin      (501) staff       (20)       60 2020-06-12 15:15:27.000000 translate_util-1.1.4/translate_util/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      713 2024-05-06 03:30:42.000000 translate_util-1.1.4/translate_util/base_translate.py
+-rw-r--r--   0 admin      (501) staff       (20)      756 2020-06-13 13:57:02.000000 translate_util-1.1.4/translate_util/common_request.py
+-rw-r--r--   0 admin      (501) staff       (20)     5817 2022-08-24 03:09:35.000000 translate_util-1.1.4/translate_util/translate_baidu.py
+-rw-r--r--   0 admin      (501) staff       (20)     2957 2024-05-11 03:08:25.000000 translate_util-1.1.4/translate_util/translate_google.py
+-rw-r--r--   0 admin      (501) staff       (20)     1608 2022-08-24 03:14:57.000000 translate_util-1.1.4/translate_util/translate_iciba.py
+-rw-r--r--   0 admin      (501) staff       (20)     4209 2024-05-14 12:00:54.000000 translate_util-1.1.4/translate_util/translate_tool.py
+-rw-r--r--   0 admin      (501) staff       (20)     1801 2022-08-24 03:16:53.000000 translate_util-1.1.4/translate_util/translate_youdao.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-14 12:02:28.000000 translate_util-1.1.4/translate_util.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1796 2024-05-14 12:02:28.000000 translate_util-1.1.4/translate_util.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      471 2024-05-14 12:02:28.000000 translate_util-1.1.4/translate_util.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-05-14 12:02:28.000000 translate_util-1.1.4/translate_util.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       63 2024-05-14 12:02:28.000000 translate_util-1.1.4/translate_util.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       15 2024-05-14 12:02:28.000000 translate_util-1.1.4/translate_util.egg-info/top_level.txt
```

### Comparing `translate_util-1.1.3/PKG-INFO` & `translate_util-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate_util
-Version: 1.1.3
+Version: 1.1.4
 Summary: translate tool support(google)
 Home-page: https://github.com/abo123456789/translate_util
 Author: cc
 Author-email: abcdef123456chen@sohu.com
 Maintainer: cc
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
```

### Comparing `translate_util-1.1.3/README.md` & `translate_util-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.3/setup.py` & `translate_util-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @TIME 2020/04/29 23:26
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='translate_util',
-    version='1.1.3',
+    version='1.1.4',
     description=(
         'translate tool support(google)'
     ),
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     author='cc',
     author_email='abcdef123456chen@sohu.com',
```

### Comparing `translate_util-1.1.3/translate_util/base_translate.py` & `translate_util-1.1.4/translate_util/base_translate.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.3/translate_util/common_request.py` & `translate_util-1.1.4/translate_util/common_request.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.3/translate_util/translate_baidu.py` & `translate_util-1.1.4/translate_util/translate_baidu.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.3/translate_util/translate_google.py` & `translate_util-1.1.4/translate_util/translate_google.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.3/translate_util/translate_iciba.py` & `translate_util-1.1.4/translate_util/translate_iciba.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.3/translate_util/translate_tool.py` & `translate_util-1.1.4/translate_util/translate_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         #    return YoudaoTranslate(content=content, proxies=proxies).trans_text_en2cn()
         else:
             return GoogleTranslate(content=content, proxies=proxies).trans_text_en2cn()
     except(Exception,):
         raise Exception(traceback.format_exc())
 
 @retry(stop_max_attempt_number=3)
-def translate_text(content: str, sl='auto', tl='zh-CN'):
+def translate_text(content: str, sl='auto', tl='zh-CN', proxies=None):
     try:
-        return GoogleTranslate(content=content).trans_text(content, sl, tl)
+        return GoogleTranslate(content=content, proxies=proxies).trans_text(content, sl, tl)
     except(Exception,):
         raise Exception(traceback.format_exc())
 
 
 @retry(stop_max_attempt_number=3)
 def translate_other2cn(content: str, platform='google', proxies: str = None):
     """
```

### Comparing `translate_util-1.1.3/translate_util/translate_youdao.py` & `translate_util-1.1.4/translate_util/translate_youdao.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.3/translate_util.egg-info/PKG-INFO` & `translate_util-1.1.4/translate_util.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate-util
-Version: 1.1.3
+Version: 1.1.4
 Summary: translate tool support(google)
 Home-page: https://github.com/abo123456789/translate_util
 Author: cc
 Author-email: abcdef123456chen@sohu.com
 Maintainer: cc
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
```

