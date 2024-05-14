# Comparing `tmp/acdh_baserow_pyutils-0.8.tar.gz` & `tmp/acdh_baserow_pyutils-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acdh_baserow_pyutils-0.8.tar", last modified: Mon Feb 19 11:55:40 2024, max compression
+gzip compressed data, was "acdh_baserow_pyutils-0.9.tar", last modified: Tue May 14 06:57:42 2024, max compression
```

## Comparing `acdh_baserow_pyutils-0.8.tar` & `acdh_baserow_pyutils-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:55:40.281241 acdh_baserow_pyutils-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-19 11:55:31.000000 acdh_baserow_pyutils-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-02-19 11:55:40.281241 acdh_baserow_pyutils-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-02-19 11:55:31.000000 acdh_baserow_pyutils-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:55:40.281241 acdh_baserow_pyutils-0.8/acdh_baserow_pyutils/
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-02-19 11:55:31.000000 acdh_baserow_pyutils-0.8/acdh_baserow_pyutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:55:40.281241 acdh_baserow_pyutils-0.8/acdh_baserow_pyutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-02-19 11:55:40.000000 acdh_baserow_pyutils-0.8/acdh_baserow_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-19 11:55:40.000000 acdh_baserow_pyutils-0.8/acdh_baserow_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 11:55:40.000000 acdh_baserow_pyutils-0.8/acdh_baserow_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 11:55:40.000000 acdh_baserow_pyutils-0.8/acdh_baserow_pyutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-19 11:55:40.000000 acdh_baserow_pyutils-0.8/acdh_baserow_pyutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-19 11:55:40.000000 acdh_baserow_pyutils-0.8/acdh_baserow_pyutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 11:55:40.281241 acdh_baserow_pyutils-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-19 11:55:31.000000 acdh_baserow_pyutils-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:57:42.742771 acdh_baserow_pyutils-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-14 06:57:33.000000 acdh_baserow_pyutils-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-14 06:57:42.742771 acdh_baserow_pyutils-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-14 06:57:33.000000 acdh_baserow_pyutils-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:57:42.742771 acdh_baserow_pyutils-0.9/acdh_baserow_pyutils/
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-14 06:57:33.000000 acdh_baserow_pyutils-0.9/acdh_baserow_pyutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:57:42.742771 acdh_baserow_pyutils-0.9/acdh_baserow_pyutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-14 06:57:42.000000 acdh_baserow_pyutils-0.9/acdh_baserow_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-14 06:57:42.000000 acdh_baserow_pyutils-0.9/acdh_baserow_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:57:42.000000 acdh_baserow_pyutils-0.9/acdh_baserow_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:57:42.000000 acdh_baserow_pyutils-0.9/acdh_baserow_pyutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 06:57:42.000000 acdh_baserow_pyutils-0.9/acdh_baserow_pyutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 06:57:42.000000 acdh_baserow_pyutils-0.9/acdh_baserow_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 06:57:42.742771 acdh_baserow_pyutils-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-14 06:57:34.000000 acdh_baserow_pyutils-0.9/setup.py
```

### Comparing `acdh_baserow_pyutils-0.8/LICENSE` & `acdh_baserow_pyutils-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `acdh_baserow_pyutils-0.8/PKG-INFO` & `acdh_baserow_pyutils-0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acdh_baserow_pyutils
-Version: 0.8
+Version: 0.9
 Summary: Utility functions to work with Baserow
 Home-page: https://github.com/acdh-oeaw/acdh-baserow-pyutils
 Author: Peter Andorfer
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT license
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `acdh_baserow_pyutils-0.8/README.md` & `acdh_baserow_pyutils-0.9/README.md`

 * *Files identical despite different names*

### Comparing `acdh_baserow_pyutils-0.8/acdh_baserow_pyutils/__init__.py` & `acdh_baserow_pyutils-0.9/acdh_baserow_pyutils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -271,14 +271,39 @@
                     valid = False
                     raise KeyError("link_row field missing 'link_row_table_id' key")
                 elif not isinstance(f["link_row_table_id"], int):
                     valid = False
                     raise ValueError("link_row_table_id field must be a integer")
         return br_table_fields, valid
 
+    def patch_row(self, table_id: str, row_id: str, payload: dict) -> dict:
+        """sends a PATCH request for the given row
+
+        Args:
+            table_id (str): The ID of the table
+            row_id (str): The ID of the row
+            payload (dict): The patch-data, see
+            https://api.baserow.io/api/redoc/#tag/Database-table-rows/operation/update_database_table_row
+
+        Returns:
+            dict: The JSON response of the updated row
+        """
+
+        url = f"{self.br_base_url}database/rows/table/{table_id}/{row_id}/?user_field_names=true"
+        print(url)
+        r = requests.patch(
+            url,
+            headers={
+                "Authorization": f"Token {self.br_token}",
+                "Content-Type": "application/json",
+            },
+            json=payload,
+        )
+        return r.json()
+
     def __init__(
         self,
         br_user,
         br_pw,
         br_token,
         br_base_url="https://api.baserow.io/api/",
         br_db_id=None,
```

### Comparing `acdh_baserow_pyutils-0.8/acdh_baserow_pyutils.egg-info/PKG-INFO` & `acdh_baserow_pyutils-0.9/acdh_baserow_pyutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acdh-baserow-pyutils
-Version: 0.8
+Version: 0.9
 Summary: Utility functions to work with Baserow
 Home-page: https://github.com/acdh-oeaw/acdh-baserow-pyutils
 Author: Peter Andorfer
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT license
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `acdh_baserow_pyutils-0.8/setup.py` & `acdh_baserow_pyutils-0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,10 +34,10 @@
     include_package_data=True,
     name="acdh_baserow_pyutils",
     packages=find_packages(include=["acdh_baserow_pyutils", "acdh_baserow_pyutils.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/acdh-oeaw/acdh-baserow-pyutils",
-    version="v0.8",
+    version="v0.9",
     zip_safe=False,
 )
```

