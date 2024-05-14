# Comparing `tmp/ca_vntl_helper-0.0.2.tar.gz` & `tmp/ca_vntl_helper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ca_vntl_helper-0.0.2.tar", last modified: Tue May 14 10:44:10 2024, max compression
+gzip compressed data, was "ca_vntl_helper-1.0.2.tar", last modified: Tue May 14 11:00:33 2024, max compression
```

## Comparing `ca_vntl_helper-0.0.2.tar` & `ca_vntl_helper-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-14 10:44:10.011330 ca_vntl_helper-0.0.2/
--rw-r--r--   0 s19404     (502) staff       (20)     1073 2024-05-10 16:06:44.000000 ca_vntl_helper-0.0.2/LICENSE
--rw-r--r--   0 s19404     (502) staff       (20)      746 2024-05-14 10:44:10.011038 ca_vntl_helper-0.0.2/PKG-INFO
--rw-r--r--   0 s19404     (502) staff       (20)      172 2024-05-12 10:16:24.000000 ca_vntl_helper-0.0.2/README.md
--rw-r--r--   0 s19404     (502) staff       (20)      643 2024-05-14 10:43:57.000000 ca_vntl_helper-0.0.2/pyproject.toml
--rw-r--r--   0 s19404     (502) staff       (20)       38 2024-05-14 10:44:10.011384 ca_vntl_helper-0.0.2/setup.cfg
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-14 10:44:10.008446 ca_vntl_helper-0.0.2/src/
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-14 10:44:10.009126 ca_vntl_helper-0.0.2/src/ca_vntl_helper/
--rw-r--r--   0 s19404     (502) staff       (20)       75 2024-05-14 09:42:20.000000 ca_vntl_helper-0.0.2/src/ca_vntl_helper/__init__.py
--rw-r--r--   0 s19404     (502) staff       (20)     3186 2024-05-14 09:41:02.000000 ca_vntl_helper-0.0.2/src/ca_vntl_helper/decorator.py
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-14 10:44:10.010688 ca_vntl_helper-0.0.2/src/ca_vntl_helper.egg-info/
--rw-r--r--   0 s19404     (502) staff       (20)      746 2024-05-14 10:44:10.000000 ca_vntl_helper-0.0.2/src/ca_vntl_helper.egg-info/PKG-INFO
--rw-r--r--   0 s19404     (502) staff       (20)      275 2024-05-14 10:44:10.000000 ca_vntl_helper-0.0.2/src/ca_vntl_helper.egg-info/SOURCES.txt
--rw-r--r--   0 s19404     (502) staff       (20)        1 2024-05-14 10:44:10.000000 ca_vntl_helper-0.0.2/src/ca_vntl_helper.egg-info/dependency_links.txt
--rw-r--r--   0 s19404     (502) staff       (20)       20 2024-05-14 10:44:10.000000 ca_vntl_helper-0.0.2/src/ca_vntl_helper.egg-info/top_level.txt
--rw-r--r--   0 s19404     (502) staff       (20)      218 2024-05-14 09:42:49.000000 ca_vntl_helper-0.0.2/src/test.py
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-14 11:00:33.587104 ca_vntl_helper-1.0.2/
+-rw-r--r--   0 s19404     (502) staff       (20)     1073 2024-05-10 16:06:44.000000 ca_vntl_helper-1.0.2/LICENSE
+-rw-r--r--   0 s19404     (502) staff       (20)      746 2024-05-14 11:00:33.586856 ca_vntl_helper-1.0.2/PKG-INFO
+-rw-r--r--   0 s19404     (502) staff       (20)      172 2024-05-12 10:16:24.000000 ca_vntl_helper-1.0.2/README.md
+-rw-r--r--   0 s19404     (502) staff       (20)      643 2024-05-14 11:00:28.000000 ca_vntl_helper-1.0.2/pyproject.toml
+-rw-r--r--   0 s19404     (502) staff       (20)       38 2024-05-14 11:00:33.587154 ca_vntl_helper-1.0.2/setup.cfg
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-14 11:00:33.584541 ca_vntl_helper-1.0.2/src/
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-14 11:00:33.585198 ca_vntl_helper-1.0.2/src/ca_vntl_helper/
+-rw-r--r--   0 s19404     (502) staff       (20)       75 2024-05-14 09:42:20.000000 ca_vntl_helper-1.0.2/src/ca_vntl_helper/__init__.py
+-rw-r--r--   0 s19404     (502) staff       (20)     3186 2024-05-14 09:41:02.000000 ca_vntl_helper-1.0.2/src/ca_vntl_helper/decorator.py
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-14 11:00:33.586556 ca_vntl_helper-1.0.2/src/ca_vntl_helper.egg-info/
+-rw-r--r--   0 s19404     (502) staff       (20)      746 2024-05-14 11:00:33.000000 ca_vntl_helper-1.0.2/src/ca_vntl_helper.egg-info/PKG-INFO
+-rw-r--r--   0 s19404     (502) staff       (20)      275 2024-05-14 11:00:33.000000 ca_vntl_helper-1.0.2/src/ca_vntl_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 s19404     (502) staff       (20)        1 2024-05-14 11:00:33.000000 ca_vntl_helper-1.0.2/src/ca_vntl_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 s19404     (502) staff       (20)       20 2024-05-14 11:00:33.000000 ca_vntl_helper-1.0.2/src/ca_vntl_helper.egg-info/top_level.txt
+-rw-r--r--   0 s19404     (502) staff       (20)      218 2024-05-14 09:42:49.000000 ca_vntl_helper-1.0.2/src/test.py
```

### Comparing `ca_vntl_helper-0.0.2/LICENSE` & `ca_vntl_helper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ca_vntl_helper-0.0.2/PKG-INFO` & `ca_vntl_helper-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ca-vntl-helper
-Version: 0.0.2
+Version: 1.0.2
 Summary: Some useful functions, classes to help work. Create by Van of Techlab CA team.
 Author-email: Bui Ngoc Huy Van <bui_ngoc_huy_van@ca-adv.co.jp>
 Project-URL: Homepage, https://github.com/vanbnh/ca-vntl-helper
 Project-URL: Issues, https://github.com/vanbnh/ca-vntl-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ca_vntl_helper-0.0.2/pyproject.toml` & `ca_vntl_helper-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ca-vntl-helper"
-version = "0.0.2"
+version = "1.0.2"
 authors = [
   { name="Bui Ngoc Huy Van", email="bui_ngoc_huy_van@ca-adv.co.jp" },
 ]
 description = "Some useful functions, classes to help work. Create by Van of Techlab CA team."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ca_vntl_helper-0.0.2/src/ca_vntl_helper/decorator.py` & `ca_vntl_helper-1.0.2/src/ca_vntl_helper/decorator.py`

 * *Files identical despite different names*

### Comparing `ca_vntl_helper-0.0.2/src/ca_vntl_helper.egg-info/PKG-INFO` & `ca_vntl_helper-1.0.2/src/ca_vntl_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ca-vntl-helper
-Version: 0.0.2
+Version: 1.0.2
 Summary: Some useful functions, classes to help work. Create by Van of Techlab CA team.
 Author-email: Bui Ngoc Huy Van <bui_ngoc_huy_van@ca-adv.co.jp>
 Project-URL: Homepage, https://github.com/vanbnh/ca-vntl-helper
 Project-URL: Issues, https://github.com/vanbnh/ca-vntl-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

