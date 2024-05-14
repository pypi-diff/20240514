# Comparing `tmp/fish_util-0.0.4.tar.gz` & `tmp/fish_util-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fish_util-0.0.4.tar", last modified: Tue May 14 11:42:10 2024, max compression
+gzip compressed data, was "fish_util-0.0.5.tar", last modified: Tue May 14 11:46:59 2024, max compression
```

## Comparing `fish_util-0.0.4.tar` & `fish_util-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 yutianran   (501) staff       (20)        0 2024-05-14 11:42:10.695910 fish_util-0.0.4/
--rw-r--r--   0 yutianran   (501) staff       (20)     1644 2024-05-14 11:42:10.695618 fish_util-0.0.4/PKG-INFO
--rw-r--r--   0 yutianran   (501) staff       (20)     1310 2024-05-14 09:54:29.000000 fish_util-0.0.4/README.md
-drwxr-xr-x   0 yutianran   (501) staff       (20)        0 2024-05-14 11:42:10.688478 fish_util-0.0.4/fish_util/
--rw-r--r--   0 yutianran   (501) staff       (20)        0 2024-05-13 05:44:49.000000 fish_util-0.0.4/fish_util/__init__.py
--rw-r--r--   0 yutianran   (501) staff       (20)      230 2024-05-14 04:52:03.000000 fish_util-0.0.4/fish_util/main.py
-drwxr-xr-x   0 yutianran   (501) staff       (20)        0 2024-05-14 11:42:10.693636 fish_util-0.0.4/fish_util/src/
--rw-r--r--   0 yutianran   (501) staff       (20)        0 2024-05-14 03:56:07.000000 fish_util-0.0.4/fish_util/src/__init__.py
--rw-r--r--   0 yutianran   (501) staff       (20)     1286 2024-05-14 11:24:47.000000 fish_util-0.0.4/fish_util/src/collections_util.py
--rw-r--r--   0 yutianran   (501) staff       (20)     9838 2024-05-13 16:00:11.000000 fish_util-0.0.4/fish_util/src/common_op.py
--rw-r--r--   0 yutianran   (501) staff       (20)     3951 2024-05-13 05:44:49.000000 fish_util-0.0.4/fish_util/src/content_format.py
--rw-r--r--   0 yutianran   (501) staff       (20)     3284 2024-05-14 04:56:40.000000 fish_util-0.0.4/fish_util/src/decorator_util.py
--rw-r--r--   0 yutianran   (501) staff       (20)     1850 2024-05-14 10:42:41.000000 fish_util-0.0.4/fish_util/src/file_util.py
--rw-r--r--   0 yutianran   (501) staff       (20)      515 2024-05-13 05:44:49.000000 fish_util-0.0.4/fish_util/src/internal_var.py
--rw-r--r--   0 yutianran   (501) staff       (20)     3865 2024-05-14 05:52:45.000000 fish_util-0.0.4/fish_util/src/log_util.py
--rw-r--r--   0 yutianran   (501) staff       (20)      372 2024-05-14 11:34:26.000000 fish_util-0.0.4/fish_util/src/read_config.py
--rw-r--r--   0 yutianran   (501) staff       (20)     1311 2024-05-14 11:29:11.000000 fish_util-0.0.4/fish_util/src/yaml_util.py
-drwxr-xr-x   0 yutianran   (501) staff       (20)        0 2024-05-14 11:42:10.695062 fish_util-0.0.4/fish_util/test/
--rw-r--r--   0 yutianran   (501) staff       (20)        0 2024-05-14 04:00:10.000000 fish_util-0.0.4/fish_util/test/__init__.py
--rw-r--r--   0 yutianran   (501) staff       (20)      712 2024-05-14 07:32:32.000000 fish_util-0.0.4/fish_util/test/test_allure.py
--rw-r--r--   0 yutianran   (501) staff       (20)     1222 2024-05-14 09:35:50.000000 fish_util-0.0.4/fish_util/test/test_decorator_util.py
--rw-r--r--   0 yutianran   (501) staff       (20)      524 2024-05-14 06:48:48.000000 fish_util-0.0.4/fish_util/test/test_log_util.py
-drwxr-xr-x   0 yutianran   (501) staff       (20)        0 2024-05-14 11:42:10.689830 fish_util-0.0.4/fish_util.egg-info/
--rw-r--r--   0 yutianran   (501) staff       (20)     1644 2024-05-14 11:42:10.000000 fish_util-0.0.4/fish_util.egg-info/PKG-INFO
--rw-r--r--   0 yutianran   (501) staff       (20)      607 2024-05-14 11:42:10.000000 fish_util-0.0.4/fish_util.egg-info/SOURCES.txt
--rw-r--r--   0 yutianran   (501) staff       (20)        1 2024-05-14 11:42:10.000000 fish_util-0.0.4/fish_util.egg-info/dependency_links.txt
--rw-r--r--   0 yutianran   (501) staff       (20)       10 2024-05-14 11:42:10.000000 fish_util-0.0.4/fish_util.egg-info/top_level.txt
--rw-r--r--   0 yutianran   (501) staff       (20)       38 2024-05-14 11:42:10.696018 fish_util-0.0.4/setup.cfg
--rw-r--r--   0 yutianran   (501) staff       (20)      680 2024-05-14 11:33:27.000000 fish_util-0.0.4/setup.py
+drwxr-xr-x   0 yutianran   (501) staff       (20)        0 2024-05-14 11:46:59.002033 fish_util-0.0.5/
+-rw-r--r--   0 yutianran   (501) staff       (20)     1644 2024-05-14 11:46:59.001572 fish_util-0.0.5/PKG-INFO
+-rw-r--r--   0 yutianran   (501) staff       (20)     1310 2024-05-14 09:54:29.000000 fish_util-0.0.5/README.md
+drwxr-xr-x   0 yutianran   (501) staff       (20)        0 2024-05-14 11:46:58.986975 fish_util-0.0.5/fish_util/
+-rw-r--r--   0 yutianran   (501) staff       (20)        0 2024-05-13 05:44:49.000000 fish_util-0.0.5/fish_util/__init__.py
+-rw-r--r--   0 yutianran   (501) staff       (20)      230 2024-05-14 04:52:03.000000 fish_util-0.0.5/fish_util/main.py
+drwxr-xr-x   0 yutianran   (501) staff       (20)        0 2024-05-14 11:46:58.997431 fish_util-0.0.5/fish_util/src/
+-rw-r--r--   0 yutianran   (501) staff       (20)        0 2024-05-14 03:56:07.000000 fish_util-0.0.5/fish_util/src/__init__.py
+-rw-r--r--   0 yutianran   (501) staff       (20)     1286 2024-05-14 11:24:47.000000 fish_util-0.0.5/fish_util/src/collections_util.py
+-rw-r--r--   0 yutianran   (501) staff       (20)     9838 2024-05-13 16:00:11.000000 fish_util-0.0.5/fish_util/src/common_op.py
+-rw-r--r--   0 yutianran   (501) staff       (20)     3951 2024-05-13 05:44:49.000000 fish_util-0.0.5/fish_util/src/content_format.py
+-rw-r--r--   0 yutianran   (501) staff       (20)     3284 2024-05-14 04:56:40.000000 fish_util-0.0.5/fish_util/src/decorator_util.py
+-rw-r--r--   0 yutianran   (501) staff       (20)     1850 2024-05-14 10:42:41.000000 fish_util-0.0.5/fish_util/src/file_util.py
+-rw-r--r--   0 yutianran   (501) staff       (20)      515 2024-05-13 05:44:49.000000 fish_util-0.0.5/fish_util/src/internal_var.py
+-rw-r--r--   0 yutianran   (501) staff       (20)     3865 2024-05-14 05:52:45.000000 fish_util-0.0.5/fish_util/src/log_util.py
+-rw-r--r--   0 yutianran   (501) staff       (20)      372 2024-05-14 11:34:26.000000 fish_util-0.0.5/fish_util/src/read_config.py
+-rw-r--r--   0 yutianran   (501) staff       (20)     1311 2024-05-14 11:29:11.000000 fish_util-0.0.5/fish_util/src/yaml_util.py
+drwxr-xr-x   0 yutianran   (501) staff       (20)        0 2024-05-14 11:46:59.000662 fish_util-0.0.5/fish_util/test/
+-rw-r--r--   0 yutianran   (501) staff       (20)        0 2024-05-14 04:00:10.000000 fish_util-0.0.5/fish_util/test/__init__.py
+-rw-r--r--   0 yutianran   (501) staff       (20)      712 2024-05-14 07:32:32.000000 fish_util-0.0.5/fish_util/test/test_allure.py
+-rw-r--r--   0 yutianran   (501) staff       (20)     1222 2024-05-14 09:35:50.000000 fish_util-0.0.5/fish_util/test/test_decorator_util.py
+-rw-r--r--   0 yutianran   (501) staff       (20)      524 2024-05-14 06:48:48.000000 fish_util-0.0.5/fish_util/test/test_log_util.py
+drwxr-xr-x   0 yutianran   (501) staff       (20)        0 2024-05-14 11:46:58.989177 fish_util-0.0.5/fish_util.egg-info/
+-rw-r--r--   0 yutianran   (501) staff       (20)     1644 2024-05-14 11:46:58.000000 fish_util-0.0.5/fish_util.egg-info/PKG-INFO
+-rw-r--r--   0 yutianran   (501) staff       (20)      607 2024-05-14 11:46:58.000000 fish_util-0.0.5/fish_util.egg-info/SOURCES.txt
+-rw-r--r--   0 yutianran   (501) staff       (20)        1 2024-05-14 11:46:58.000000 fish_util-0.0.5/fish_util.egg-info/dependency_links.txt
+-rw-r--r--   0 yutianran   (501) staff       (20)       10 2024-05-14 11:46:58.000000 fish_util-0.0.5/fish_util.egg-info/top_level.txt
+-rw-r--r--   0 yutianran   (501) staff       (20)       38 2024-05-14 11:46:59.002197 fish_util-0.0.5/setup.cfg
+-rw-r--r--   0 yutianran   (501) staff       (20)      680 2024-05-14 11:44:10.000000 fish_util-0.0.5/setup.py
```

### Comparing `fish_util-0.0.4/PKG-INFO` & `fish_util-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fish_util
-Version: 0.0.4
+Version: 0.0.5
 Summary: Fishyer's Python Util Library
 Home-page: https://github.com/fishyer/fish_util
 Author: Fishyer
 Author-email: yutianran666@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `fish_util-0.0.4/README.md` & `fish_util-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/fish_util/src/collections_util.py` & `fish_util-0.0.5/fish_util/src/collections_util.py`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/fish_util/src/common_op.py` & `fish_util-0.0.5/fish_util/src/common_op.py`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/fish_util/src/content_format.py` & `fish_util-0.0.5/fish_util/src/content_format.py`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/fish_util/src/decorator_util.py` & `fish_util-0.0.5/fish_util/src/decorator_util.py`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/fish_util/src/file_util.py` & `fish_util-0.0.5/fish_util/src/file_util.py`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/fish_util/src/internal_var.py` & `fish_util-0.0.5/fish_util/src/internal_var.py`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/fish_util/src/log_util.py` & `fish_util-0.0.5/fish_util/src/log_util.py`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/fish_util/src/yaml_util.py` & `fish_util-0.0.5/fish_util/src/yaml_util.py`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/fish_util/test/test_allure.py` & `fish_util-0.0.5/fish_util/test/test_allure.py`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/fish_util/test/test_decorator_util.py` & `fish_util-0.0.5/fish_util/test/test_decorator_util.py`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/fish_util/test/test_log_util.py` & `fish_util-0.0.5/fish_util/test/test_log_util.py`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/fish_util.egg-info/PKG-INFO` & `fish_util-0.0.5/fish_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fish-util
-Version: 0.0.4
+Version: 0.0.5
 Summary: Fishyer's Python Util Library
 Home-page: https://github.com/fishyer/fish_util
 Author: Fishyer
 Author-email: yutianran666@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `fish_util-0.0.4/fish_util.egg-info/SOURCES.txt` & `fish_util-0.0.5/fish_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fish_util-0.0.4/setup.py` & `fish_util-0.0.5/setup.py`

 * *Files identical despite different names*

