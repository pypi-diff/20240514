# Comparing `tmp/pypomes_db-0.7.7.tar.gz` & `tmp/pypomes_db-0.7.8.tar.gz`

## Comparing `pypomes_db-0.7.7.tar` & `pypomes_db-0.7.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    17799 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    18535 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.8/PKG-INFO
```

### Comparing `pypomes_db-0.7.7/src/pypomes_db/__init__.py` & `pypomes_db-0.7.8/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.7/src/pypomes_db/db_common.py` & `pypomes_db-0.7.8/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.7/src/pypomes_db/db_pomes.py` & `pypomes_db-0.7.8/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.7/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.7.8/src/pypomes_db/migration_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,14 +158,21 @@
             result += len(rows)
             # read the next batch
             if batch_size:
                 rows = source_cursor.fetchmany(size=batch_size)
             else:
                 rows = source_cursor.fetchall()
 
+            # log partial result
+            _db_log(logger=logger,
+                    engine=source_engine,
+                    stmt=(f"Migrated {result} tuples, "
+                          f"from {source_engine}.{source_table} "
+                          f"to {target_engine}.{target_table}"))
+
         # close the cursors and commit the transactions
         source_cursor.close()
         curr_source_conn.commit()
         target_cursor.close()
         curr_target_conn.commit()
     except Exception as e:
         # rollback the transactions
@@ -352,14 +359,22 @@
                 offset += size
                 lob_data = lob.read(offset=offset,
                                     amount=chunk_size)
 
             # increment the LOB migration counter
             result += 1
 
+            # log partial result at each 100000 LOBs migrated
+            if result % 1000000 == 0:
+                _db_log(logger=logger,
+                        engine=source_engine,
+                        stmt=(f"Migrated {result} LOBs, "
+                              f"from {source_engine}.{source_table}.{source_lob_column} "
+                              f"to {target_engine}.{target_table}.{target_lob_column}"))
+
         # close the cursors and commit the transactions
         source_cursor.close()
         curr_source_conn.commit()
         target_cursor.close()
         curr_target_conn.commit()
     except Exception as e:
         # rollback the transactions
```

### Comparing `pypomes_db-0.7.7/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.7.8/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.7/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.7.8/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.7/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.7.8/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.7/LICENSE` & `pypomes_db-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.7/pyproject.toml` & `pypomes_db-0.7.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.7.7"
+version = "0.7.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.7.7/PKG-INFO` & `pypomes_db-0.7.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.7.7
+Version: 0.7.8
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

