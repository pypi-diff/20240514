# Comparing `tmp/group_local-0.0.24.tar.gz` & `tmp/group_local-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "group_local-0.0.24.tar", last modified: Mon May 13 18:20:59 2024, max compression
+gzip compressed data, was "group_local-0.0.25.tar", last modified: Tue May 14 08:28:31 2024, max compression
```

## Comparing `group_local-0.0.24.tar` & `group_local-0.0.25.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:20:59.394767 group_local-0.0.24/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-13 18:20:59.394767 group_local-0.0.24/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:20:59.394767 group_local-0.0.24/group_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:20:59.394767 group_local-0.0.24/group_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:20:44.000000 group_local-0.0.24/group_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-05-13 18:20:44.000000 group_local-0.0.24/group_local/src/group_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-13 18:20:44.000000 group_local-0.0.24/group_local/src/group_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:20:59.394767 group_local-0.0.24/group_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-13 18:20:59.000000 group_local-0.0.24/group_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-13 18:20:59.000000 group_local-0.0.24/group_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:20:59.000000 group_local-0.0.24/group_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 18:20:59.000000 group_local-0.0.24/group_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 18:20:59.000000 group_local-0.0.24/group_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-13 18:20:44.000000 group_local-0.0.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:20:59.394767 group_local-0.0.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-13 18:20:44.000000 group_local-0.0.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:28:31.980318 group_local-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 08:28:31.980318 group_local-0.0.25/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:28:31.976318 group_local-0.0.25/group_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:28:31.980318 group_local-0.0.25/group_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:28:12.000000 group_local-0.0.25/group_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13301 2024-05-14 08:28:12.000000 group_local-0.0.25/group_local/src/group_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-14 08:28:12.000000 group_local-0.0.25/group_local/src/group_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:28:31.980318 group_local-0.0.25/group_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 08:28:31.000000 group_local-0.0.25/group_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 08:28:31.000000 group_local-0.0.25/group_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:28:31.000000 group_local-0.0.25/group_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 08:28:31.000000 group_local-0.0.25/group_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 08:28:31.000000 group_local-0.0.25/group_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 08:28:12.000000 group_local-0.0.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:28:31.980318 group_local-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-14 08:28:12.000000 group_local-0.0.25/setup.py
```

### Comparing `group_local-0.0.24/PKG-INFO` & `group_local-0.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.24
+Version: 0.0.25
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `group_local-0.0.24/group_local/src/group_local.py` & `group_local-0.0.25/group_local/src/group_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             "updated_effective_user_id": user_context.get_effective_user_id(),
             "updated_effective_profile_id": user_context.get_effective_profile_id(),
             "is_title_approved": group_dict.get('is_title_approved', None),
             "is_description_approved": group_dict.get('is_description_approved', None)
         }
         if "(" and ")" in group_dict.get('title'):
             group_id, group_ml_ids_list = GenericCRUDML.upsert_value_with_abbreviations(
-                self, table_name="group_table", data_dict=group_ml_data_dict,
+                self, table_name="group_table", data_dict=group_data_dict,
                 data_ml_dict=group_ml_data_dict,
                 ml_table_name="group_ml_table",
                 lang_code=lang_code,
                 data_dict_compare=data_dict_compare,
                 compare_view_name="group_ml_also_not_approved_view",
                 order_by=order_by
             )
```

### Comparing `group_local-0.0.24/group_local/src/group_local_constants.py` & `group_local-0.0.25/group_local/src/group_local_constants.py`

 * *Files identical despite different names*

### Comparing `group_local-0.0.24/group_local.egg-info/PKG-INFO` & `group_local-0.0.25/group_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.24
+Version: 0.0.25
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `group_local-0.0.24/setup.py` & `group_local-0.0.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "group-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/group-local
-    version='0.0.24',
+    version='0.0.25',
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles group-local Python",
     long_description="PyPI Package for Circles group-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/group-main-local-python-package",
     packages=[package_dir],
```

