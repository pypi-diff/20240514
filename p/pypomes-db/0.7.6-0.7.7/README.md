# Comparing `tmp/pypomes_db-0.7.6.tar.gz` & `tmp/pypomes_db-0.7.7.tar.gz`

## Comparing `pypomes_db-0.7.6.tar` & `pypomes_db-0.7.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    17279 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    17799 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/PKG-INFO
```

### Comparing `pypomes_db-0.7.6/src/pypomes_db/__init__.py` & `pypomes_db-0.7.7/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.6/src/pypomes_db/db_common.py` & `pypomes_db-0.7.7/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.6/src/pypomes_db/db_pomes.py` & `pypomes_db-0.7.7/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.6/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.7.7/src/pypomes_db/migration_pomes.py`

 * *Files 8% similar despite different names*

```diff
@@ -192,41 +192,43 @@
                   f"to {target_engine}.{target_table}"))
 
     return result
 
 def db_migrate_lobs(errors: list[str],
                     source_engine: str,
                     source_table: str,
-                    source_column: str,
-                    pk_columns: list[str],
+                    source_lob_column: str,
+                    source_pk_columns: list[str],
                     target_engine: str,
                     target_table: str = None,
-                    target_column: str = None,
+                    target_lob_column: str = None,
+                    target_pk_columns: list[str] = None,
                     source_conn: Any = None,
                     target_conn: Any = None,
                     where_clause: tuple = None,
                     chunk_size: int = None,
                     logger: Logger = None) -> int:
     """
     Migrate large binary objects (LOBs) from one database to another database.
 
     The origin and destination databases must be in the list of databases configured and
     supported by this package. One or more columns making up a primary key, or a unique row identifier,
     must exist on *source_table* and *target_table*, and be provided in *pk_columns*.
-    It is assumed that the primary key columns have the same name, and are of equivalent types,
-    in both the origin and the destination database.
+    It is assumed that the primary key columns have the same cardinality, and are of equivalent types,
+    respectively, in both the origin and the destination databases.
 
     :param errors: incidental error messages
     :param source_engine: the source database engine type
     :param source_table: the table holding the LOBs
-    :param source_column: the column holding the LOB
-    :param pk_columns: columns making up a primary key, or a unique identifier for a tuple
+    :param source_lob_column: the column holding the LOB
+    :param source_pk_columns: columns making up a primary key, or a unique identifier for a tuple, in source database
     :param target_engine: the destination database engine type
     :param target_table: the table to write the lob to (defaults to the source table)
-    :param target_column: the column to write the lob to (defaults to the source column)
+    :param target_lob_column: the column to write the lob to (defaults to the source column)
+    :param target_pk_columns: columns making up a primary key, or a unique identifier for a tuple, in target database
     :param source_conn: the connection to the source database (obtains a new one, if not specified)
     :param target_conn: the connection to the destination database (obtains a new one, if not specified)
     :param where_clause: the criteria for tuple selection
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param logger: optional logger
     :return: number of LOBs effectively migrated
     """
@@ -242,53 +244,57 @@
                                                       logger=logger)
 
     # make sure to have a target table
     if not target_table:
         target_table = source_table
 
     # make sure to have a target column
-    if not target_column:
-        target_column = source_column
+    if not target_lob_column:
+        target_lob_column = source_lob_column
+
+    # make sure to have target PK columns
+    if not target_pk_columns:
+        target_pk_columns = source_pk_columns
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
 
     # buid the SELECT query
-    pks: str = ", ".join(pk_columns)
-    sel_stmt: str = f"SELECT {pks}, {source_column} FROM {source_table}"
+    source_pks: str = ", ".join(source_pk_columns)
+    sel_stmt: str = f"SELECT {source_pks}, {source_lob_column} FROM {source_table}"
     if where_clause:
         sel_stmt += f" WHERE {where_clause}"
-    blob_index: int = len(pk_columns)
+    blob_index: int = len(source_pk_columns)
 
     # build the UPDATE query
-    where_columns: str = _db_bind_columns(engine=target_engine,
-                                          columns=pk_columns,
-                                          concat=" AND ",
-                                          start_index=2)
+    target_where_columns: str = _db_bind_columns(engine=target_engine,
+                                                 columns=target_pk_columns,
+                                                 concat=" AND ",
+                                                 start_index=2)
     if target_engine == "oracle":
         update_stmt: str = (f"UPDATE {target_table} "
-                            f"SET {target_column} = empty_blob() "
-                            f"WHERE {where_columns} "
-                            f"RETURNING {target_column} INTO :{len(where_columns)+2}")
+                            f"SET {target_lob_column} = empty_blob() "
+                            f"WHERE {target_where_columns} "
+                            f"RETURNING {target_lob_column} INTO :{len(target_where_columns) + 2}")
     else:
         lob_bind: str = _db_bind_columns(engine=target_engine,
-                                         columns=[target_column],
+                                         columns=[target_lob_column],
                                          concat=", ",
                                          start_index=1)
         update_stmt: str = (f"UPDATE {target_table} "
-                            f"SET {target_column} = {target_column} || {lob_bind[len(target_column)+3:]} "
-                            f"WHERE {where_columns}")
+                            f"SET {target_lob_column} = {target_lob_column} || {lob_bind[len(target_lob_column) + 3:]} "
+                            f"WHERE {target_where_columns}")
 
     # log the migration start
     _db_log(logger=logger,
             engine=source_engine,
             stmt=(f"Started migrating LOBs, "
-                  f"from {source_engine}.{source_table}.{source_column} "
-                  f"to {target_engine}.{target_table}.{target_column}"))
+                  f"from {source_engine}.{source_table}.{source_lob_column} "
+                  f"to {target_engine}.{target_table}.{target_lob_column}"))
 
     # migrate the LOBs
     err_msg: str | None = None
     try:
         source_cursor: Any = curr_source_conn.cursor()
         target_cursor: Any = curr_target_conn.cursor()
 
@@ -325,15 +331,15 @@
                     case "oracle":
                         ora_lob.write(data=lob_data,
                                       offset=offset)
                     case "postgres":
                         from psycopg2 import Binary
                         # remove append indication on first update
                         if offset == 1:
-                            update_pg: str = update_stmt.replace(f"{target_column} || ", "")
+                            update_pg: str = update_stmt.replace(f"{target_lob_column} || ", "")
                         else:
                             update_pg: str = update_stmt
                         # string data may come from LOB (Oracle's NCLOB is a good example)
                         col_data: str | Binary = Binary(lob_data) if isinstance(lob_data, bytes) else lob_data
                         target_cursor.execute(query=update_pg,
                                               vars=(col_data, *pk_vals))
                     case "sqlserver":
@@ -372,11 +378,11 @@
 
     # log the migration finish
     _db_log(logger=logger,
             engine=source_engine,
             err_msg=err_msg,
             errors=errors,
             stmt=(f"Migrated {result} LOBs, "
-                  f"from {source_engine}.{source_table}.{source_column} "
-                  f"to {target_engine}.{target_table}.{target_column}"))
+                  f"from {source_engine}.{source_table}.{source_lob_column} "
+                  f"to {target_engine}.{target_table}.{target_lob_column}"))
 
     return result
```

### Comparing `pypomes_db-0.7.6/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.7.7/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.6/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.7.7/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.6/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.7.7/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.6/LICENSE` & `pypomes_db-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.6/pyproject.toml` & `pypomes_db-0.7.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.7.6"
+version = "0.7.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.7.6/PKG-INFO` & `pypomes_db-0.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.7.6
+Version: 0.7.7
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

