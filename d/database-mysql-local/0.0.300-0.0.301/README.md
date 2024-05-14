# Comparing `tmp/database_mysql_local-0.0.300.tar.gz` & `tmp/database_mysql_local-0.0.301.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.300.tar", last modified: Mon May 13 17:08:41 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.301.tar", last modified: Tue May 14 08:54:05 2024, max compression
```

## Comparing `database_mysql_local-0.0.300.tar` & `database_mysql_local-0.0.301.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:08:41.804278 database_mysql_local-0.0.300/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-13 17:08:41.804278 database_mysql_local-0.0.300/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:08:41.796278 database_mysql_local-0.0.300/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:08:41.800278 database_mysql_local-0.0.300/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    51458 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31008 2024-05-13 17:08:11.000000 database_mysql_local-0.0.300/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-13 17:08:08.000000 database_mysql_local-0.0.300/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:08:41.800278 database_mysql_local-0.0.300/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-13 17:08:41.000000 database_mysql_local-0.0.300/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-13 17:08:41.000000 database_mysql_local-0.0.300/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:08:41.000000 database_mysql_local-0.0.300/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-13 17:08:41.000000 database_mysql_local-0.0.300/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 17:08:41.000000 database_mysql_local-0.0.300/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 17:08:11.000000 database_mysql_local-0.0.300/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:08:41.804278 database_mysql_local-0.0.300/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-13 17:08:11.000000 database_mysql_local-0.0.300/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:54:05.737757 database_mysql_local-0.0.301/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 08:54:05.737757 database_mysql_local-0.0.301/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:54:05.733756 database_mysql_local-0.0.301/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:54:05.737757 database_mysql_local-0.0.301/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51545 2024-05-14 08:53:30.000000 database_mysql_local-0.0.301/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31008 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-14 08:53:26.000000 database_mysql_local-0.0.301/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-14 08:53:00.000000 database_mysql_local-0.0.301/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:54:05.737757 database_mysql_local-0.0.301/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 08:54:05.000000 database_mysql_local-0.0.301/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-14 08:54:05.000000 database_mysql_local-0.0.301/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:54:05.000000 database_mysql_local-0.0.301/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-14 08:54:05.000000 database_mysql_local-0.0.301/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 08:54:05.000000 database_mysql_local-0.0.301/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 08:53:30.000000 database_mysql_local-0.0.301/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:54:05.737757 database_mysql_local-0.0.301/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-14 08:53:30.000000 database_mysql_local-0.0.301/setup.py
```

### Comparing `database_mysql_local-0.0.300/PKG-INFO` & `database_mysql_local-0.0.301/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.300
+Version: 0.0.301
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.300/README.md` & `database_mysql_local-0.0.301/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.301/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.301/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.301/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.301/database_mysql_local/src/generic_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -841,15 +841,16 @@
             else:
                 test_entity_id = insert_function(**insert_kwargs)
         self.logger.debug(object=locals())
         return test_entity_id
 
     def __get_where_params(self, column_name: str, column_value: Any) -> tuple:
         column_name = column_name or self.default_column_name
-        if column_value:
+        # If we use "if column_value:" it will not work for 0, False, etc.
+        if column_value is not None:
             where = f"`{column_name}`=%s"
             params = (column_value,)
         else:
             where = f"`{column_name}` IS NULL"
             params = None
         return where, params
```

### Comparing `database_mysql_local-0.0.300/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.301/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.301/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/database_mysql_local/src/point.py` & `database_mysql_local-0.0.301/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.301/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.301/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.301/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.301/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.301/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.301/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.300
+Version: 0.0.301
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.300/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.301/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.300/pyproject.toml` & `database_mysql_local-0.0.301/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.300" # https://pypi.org/project/database-mysql-local
+version = "0.0.301" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.300/setup.py` & `database_mysql_local-0.0.301/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.300',
+    version='0.0.301',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

