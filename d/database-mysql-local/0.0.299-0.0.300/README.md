# Comparing `tmp/database_mysql_local-0.0.299.tar.gz` & `tmp/database_mysql_local-0.0.300.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.299.tar", last modified: Sun May 12 21:27:20 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.300.tar", last modified: Mon May 13 17:08:41 2024, max compression
```

## Comparing `database_mysql_local-0.0.299.tar` & `database_mysql_local-0.0.300.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:27:20.243113 database_mysql_local-0.0.299/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 21:27:20.243113 database_mysql_local-0.0.299/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:27:20.235113 database_mysql_local-0.0.299/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:27:20.243113 database_mysql_local-0.0.299/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    51458 2024-05-12 21:26:50.000000 database_mysql_local-0.0.299/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-12 21:26:48.000000 database_mysql_local-0.0.299/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-12 21:26:25.000000 database_mysql_local-0.0.299/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:27:20.243113 database_mysql_local-0.0.299/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 21:27:20.000000 database_mysql_local-0.0.299/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 21:27:20.000000 database_mysql_local-0.0.299/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 21:27:20.000000 database_mysql_local-0.0.299/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 21:27:20.000000 database_mysql_local-0.0.299/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 21:27:20.000000 database_mysql_local-0.0.299/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-12 21:26:50.000000 database_mysql_local-0.0.299/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 21:27:20.243113 database_mysql_local-0.0.299/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 21:26:50.000000 database_mysql_local-0.0.299/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:08:41.804278 database_mysql_local-0.0.300/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-13 17:08:41.804278 database_mysql_local-0.0.300/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:08:41.796278 database_mysql_local-0.0.300/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:08:41.800278 database_mysql_local-0.0.300/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51458 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31008 2024-05-13 17:08:11.000000 database_mysql_local-0.0.300/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-13 17:08:08.000000 database_mysql_local-0.0.300/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-13 17:07:44.000000 database_mysql_local-0.0.300/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:08:41.800278 database_mysql_local-0.0.300/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-13 17:08:41.000000 database_mysql_local-0.0.300/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-13 17:08:41.000000 database_mysql_local-0.0.300/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:08:41.000000 database_mysql_local-0.0.300/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-13 17:08:41.000000 database_mysql_local-0.0.300/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 17:08:41.000000 database_mysql_local-0.0.300/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 17:08:11.000000 database_mysql_local-0.0.300/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:08:41.804278 database_mysql_local-0.0.300/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-13 17:08:11.000000 database_mysql_local-0.0.300/setup.py
```

### Comparing `database_mysql_local-0.0.299/PKG-INFO` & `database_mysql_local-0.0.300/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.299
+Version: 0.0.300
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.299/README.md` & `database_mysql_local-0.0.300/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.300/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.300/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.300/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.300/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.300/database_mysql_local/src/generic_crud_ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,20 +107,23 @@
         finally:
             self.cursor = old_cursor
             self.default_schema_name = old_schema_name
             if cursor:
                 cursor.close()
         return table_id, ml_table_id
 
-    def add_value_if_not_exist(self, *, data_dict: dict = None, data_ml_dict: dict,
+    def add_value_if_not_exist(self, *, data_dict: dict = None, data_ml_dict: dict = None,
                                data_json: dict = None, data_ml_json: dict = None,
                                table_id: int = None, lang_code: LangCode = None,
                                is_main: int = 0, table_name: str = None,
                                ml_table_name: str = None, schema_name: str = None,
                                order_by: str = None) -> tuple:
+        # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
+        if not data_ml_dict and not data_ml_json:
+            raise ValueError("data_ml_dict or data_ml_json is required for add_value_if_not_exist")
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         self.default_schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
         column_name = GenericCRUD.generate_column_name(table_name)
         ml_column_name = GenericCRUD.generate_column_name(ml_table_name)
@@ -135,21 +138,24 @@
                                              column_name=ml_column_name, order_by=order_by)
         if not table_id:
             return self.add_value(data_ml_dict=data_ml_dict, table_id=table_id, lang_code=lang_code, is_main=is_main,
                                   data_dict=data_dict, table_name=table_name, ml_table_name=ml_table_name)
         else:
             return table_id, ml_table_id
 
-    def update_value_by_id(self, *, data_dict: dict = None, data_ml_dict: dict,
+    def update_value_by_id(self, *, data_dict: dict = None, data_ml_dict: dict = None,
                            data_json: dict = None, data_ml_json: dict = None,
                            ml_table_id: int, table_id: int,
                            lang_code: LangCode = None, is_main: int = 0,
                            table_name: str = None, ml_table_name: str = None,
                            schema_name: str = None, limit: int = DEFAULT_SQL_SELECT_LIMIT,
                            order_by: str = None) -> tuple:
+        # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
+        if not data_ml_dict and not data_ml_json:
+            raise ValueError("data_ml_dict or data_ml_json is required for update_value")
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         old_schema_name = self.default_schema_name
         self.default_schema_name = schema_name or self.default_schema_name
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, data_ml_dict=data_ml_dict)
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
@@ -187,21 +193,24 @@
         finally:
             self.cursor = old_cursor
             self.default_schema_name = old_schema_name
             if cursor:
                 cursor.close()
         return table_id, ml_table_id
 
-    def upsert_value(self, *, data_dict: dict = None, data_ml_dict: dict,
+    def upsert_value(self, *, data_dict: dict = None, data_ml_dict: dict = None,
                      data_json: dict = None, data_ml_json: dict = None,
                      table_id: int = None, data_dict_compare: dict = None, lang_code: LangCode = None,
                      is_main: int = 0, table_name: str = None,
                      ml_table_name: str = None, schema_name: str = None,
                      compare_view_name: str = None,
                      limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> tuple:
+        # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
+        if not data_ml_dict and not data_ml_json:
+            raise ValueError("data_ml_dict or data_ml_json is required for upsert_value")
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         self.default_schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
         column_name = GenericCRUD.generate_column_name(table_name)
         ml_column_name = GenericCRUD.generate_column_name(ml_table_name)
@@ -235,14 +244,17 @@
                                         data_json: dict = None, data_ml_json: dict = None,
                                         data_dict_compare: dict = None,
                                         table_id: int = None, lang_code: LangCode = None,
                                         table_name: str = None,
                                         ml_table_name: str = None, schema_name: str = None,
                                         compare_view_name: str = None,
                                         limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> tuple:
+        # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
+        if not data_ml_dict and not data_ml_json:
+            raise ValueError("data_ml_dict or data_ml_json is required for upsert_value")
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         self.default_schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
         column_name = GenericCRUD.generate_column_name(table_name)
         ml_column_name = GenericCRUD.generate_column_name(ml_table_name)
```

### Comparing `database_mysql_local-0.0.299/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.300/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/database_mysql_local/src/point.py` & `database_mysql_local-0.0.300/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.300/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.300/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.300/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.300/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.300/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.300/database_mysql_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.299
+Version: 0.0.300
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.299/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.300/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.299/pyproject.toml` & `database_mysql_local-0.0.300/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.299" # https://pypi.org/project/database-mysql-local
+version = "0.0.300" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.299/setup.py` & `database_mysql_local-0.0.300/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.299',
+    version='0.0.300',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

