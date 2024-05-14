# Comparing `tmp/dq_check-0.3.0.tar.gz` & `tmp/dq_check-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dq_check-0.3.0.tar", last modified: Sun May 12 21:43:43 2024, max compression
+gzip compressed data, was "dq_check-0.3.1.tar", last modified: Tue May 14 04:21:11 2024, max compression
```

## Comparing `dq_check-0.3.0.tar` & `dq_check-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-12 21:43:43.257844 dq_check-0.3.0/
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-12 21:43:43.257516 dq_check-0.3.0/PKG-INFO
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2440 2024-05-12 21:16:29.000000 dq_check-0.3.0/README.md
--rw-r--r--   0 rohan.goel   (502) staff       (20)      327 2024-05-12 21:28:43.000000 dq_check-0.3.0/pyproject.toml
--rw-r--r--   0 rohan.goel   (502) staff       (20)      131 2024-05-12 21:43:43.258822 dq_check-0.3.0/setup.cfg
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-12 21:43:43.248422 dq_check-0.3.0/src/
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-12 21:43:43.251700 dq_check-0.3.0/src/dq_check/
--rw-r--r--   0 rohan.goel   (502) staff       (20)       29 2024-05-05 04:45:50.000000 dq_check-0.3.0/src/dq_check/__init__.py
--rw-r--r--   0 rohan.goel   (502) staff       (20)    15105 2024-05-12 21:16:57.000000 dq_check-0.3.0/src/dq_check/dq_check.py
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-12 21:43:43.256485 dq_check-0.3.0/src/dq_check.egg-info/
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-12 21:43:43.000000 dq_check-0.3.0/src/dq_check.egg-info/PKG-INFO
--rw-r--r--   0 rohan.goel   (502) staff       (20)      263 2024-05-12 21:43:43.000000 dq_check-0.3.0/src/dq_check.egg-info/SOURCES.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)        1 2024-05-12 21:43:43.000000 dq_check-0.3.0/src/dq_check.egg-info/dependency_links.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)       15 2024-05-12 21:43:43.000000 dq_check-0.3.0/src/dq_check.egg-info/requires.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)        9 2024-05-12 21:43:43.000000 dq_check-0.3.0/src/dq_check.egg-info/top_level.txt
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-14 04:21:11.802461 dq_check-0.3.1/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-14 04:21:11.802191 dq_check-0.3.1/PKG-INFO
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2440 2024-05-12 21:16:29.000000 dq_check-0.3.1/README.md
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      327 2024-05-14 04:20:39.000000 dq_check-0.3.1/pyproject.toml
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      131 2024-05-14 04:21:11.803377 dq_check-0.3.1/setup.cfg
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-14 04:21:11.793110 dq_check-0.3.1/src/
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-14 04:21:11.796614 dq_check-0.3.1/src/dq_check/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)       29 2024-05-05 04:45:50.000000 dq_check-0.3.1/src/dq_check/__init__.py
+-rw-r--r--   0 rohan.goel   (502) staff       (20)    15934 2024-05-14 04:19:45.000000 dq_check-0.3.1/src/dq_check/dq_check.py
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-14 04:21:11.801270 dq_check-0.3.1/src/dq_check.egg-info/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-14 04:21:11.000000 dq_check-0.3.1/src/dq_check.egg-info/PKG-INFO
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      263 2024-05-14 04:21:11.000000 dq_check-0.3.1/src/dq_check.egg-info/SOURCES.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)        1 2024-05-14 04:21:11.000000 dq_check-0.3.1/src/dq_check.egg-info/dependency_links.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)       15 2024-05-14 04:21:11.000000 dq_check-0.3.1/src/dq_check.egg-info/requires.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)        9 2024-05-14 04:21:11.000000 dq_check-0.3.1/src/dq_check.egg-info/top_level.txt
```

### Comparing `dq_check-0.3.0/PKG-INFO` & `dq_check-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_check
-Version: 0.3.0
+Version: 0.3.1
 Summary: A data quality check module for Spark
 Author-email: rohan goel <rohan.goel@databricks.com>
 Description-Content-Type: text/markdown
 Requires-Dist: pyspark
 Requires-Dist: pandas
 
 ## dq_check
```

### Comparing `dq_check-0.3.0/README.md` & `dq_check-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dq_check-0.3.0/src/dq_check/dq_check.py` & `dq_check-0.3.1/src/dq_check/dq_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -161,28 +161,38 @@
         
         if where_clause is not None and not isinstance(where_clause, str):
             raise ValueError("Invalid input: 'where_clause' must be a string if provided.")
         
         if not isinstance(quality_threshold_percentage, int) or quality_threshold_percentage < 0 or quality_threshold_percentage > 100:
             raise ValueError("Invalid input: 'quality_threshold_percentage' must be an integer between 0 and 100.")
 
-        if not isinstance(self.audit_table_name, str) or not self.audit_table_name or not self.audit_table_name.count('.') == 2 :
+        audit_dot_cnt = self.audit_table_name.count(".")
+        if not isinstance(self.audit_table_name, str) or not self.audit_table_name or not audit_dot_cnt == 2 :
             raise ValueError("Invalid input: 'audit_table_name' must be a non-empty string and with catalog and schema name.")
         
         #remove colon at end if present
         sql_query = sql_query.replace(';','')
         # Check if the query contains aggregation functions
         aggregates = ['min', 'max', 'avg', 'sum', 'count', 'group by']
         agg_ind = next(('y' for i in aggregates if i in sql_query.lower()), None)
-        #get catalog,schema,table
+        
+        #get catalog,schema,table for DQ table
         table_dtls = table_name.split(".")
         catalog = table_dtls[0] if table_dot_cnt == 2 else None
         schema = table_dtls[-2]
         table_name_only = table_dtls[-1]
-        print(F"Audit table catalog,schema,table_name_only: {catalog},{schema},{table_name_only}")
+        
+
+
+        #get catalog,schema,table for Audit table table
+        audit_table_dtls = self.audit_table_name.split(".")
+        audit_catalog = audit_table_dtls[0] if audit_dot_cnt == 2 else None
+        audit_schema = audit_table_dtls[-2]
+        audit_table_name_only = audit_table_dtls[-1]
+        print(F"Audit table catalog,schema,table_name_only: {audit_catalog},{audit_schema},{audit_table_name_only}")
 
         # Determine the SQL query for data extraction
         if where_clause is None:
                 sql_stmt = f"SELECT * FROM {table_name}"
         else:
                 sql_stmt = f"SELECT * FROM {table_name} {where_clause}"
                 
@@ -192,22 +202,24 @@
             # Create an instance of SparkSQLClient
             client = _SparkSQLClient(self.spark)
         elif (table_type).lower() == 'asql':
             client = self.azure_sql_client
         else:
             print(F"Invalid table type. It should either be delta or asql")
 
-        #create schema if not exists
+        #create audit schema if not exists
         try:
-            if catalog:
-                client.read_sql(F'CREATE SCHEMA IF NOT EXISTS {catalog}.{schema}')
+            if audit_catalog:
+                client.read_sql(F'CREATE SCHEMA IF NOT EXISTS {audit_catalog}.{audit_schema}')
             else:
-                client.read_sql(F'CREATE SCHEMA IF NOT EXISTS {schema}')
+                client.read_sql(F'CREATE SCHEMA IF NOT EXISTS {audit_schema}')
         except Exception as e:
-            print("User does not have create schema permission. Please check error below {e}")
+            raise Exception(F"User does not have create schema permission for audit table."
+                            F"Please make sure audit table schema is available or user has permission to create it."
+                            F"Please check error below {e}")
 
         
         #validate sql
 
         table_cols,sql_tables = self.parse_sql_query(sql_query)
 
         # table validation
@@ -263,23 +275,31 @@
         # Collect primary keys of failed records
         failed_primary_keys = {}
         #failed_primary_keys_sample = {}
         sort_col = primary_keys[0]
         if agg_without_pk_ind == 'n':
             try:
                 df_failed_primary_keys = client.read_sql(dq_primary_key_sql)
-                #failed_primary_keys = df_failed_primary_keys.select(primary_keys).toPandas().to_dict(orient='list')
-                #failed_primary_keys_sample = df_failed_primary_keys.select(primary_keys).limit(150).toPandas().to_dict(orient='list')
+
                 #below will be met incase of when there are no failed records.
+
                 if df_failed_primary_keys.count() == 0:
                    df_failed_primary_keys = client.read_sql(F'select "" as {sort_col}') 
+                # add all pk cols to df_failed_primary_keys df
+                   for pk in primary_keys:
+                       if pk != sort_col:
+                            df_failed_primary_keys = df_failed_primary_keys.withColumn(pk,lit(''))
             except Exception as e:
-                print(F"primary keys are not found in table {table_name}. Please see error below \n {e}")
+                raise KeyError(F"primary keys {primary_keys} are not found in table {table_name}. Please see error below \n {e}")
         else:
             df_failed_primary_keys = client.read_sql(F'select "" as {sort_col}')
+                # add all pk cols to df_failed_primary_keys df
+            for pk in primary_keys:
+                if pk != sort_col:
+                    df_failed_primary_keys = df_failed_primary_keys.withColumn(pk,lit(''))
 
         df_failed_primary_keys = df_failed_primary_keys.withColumn("constant",lit(1))
         window_spec = Window.orderBy("constant")
 
         df_with_row_number = df_failed_primary_keys.withColumn("Seq",row_number().over(window_spec))
         df_with_chunk = df_with_row_number.withColumn("ChunkNo",((col("Seq")/chunk_size) - 0.05).cast('int') + 1)
```

### Comparing `dq_check-0.3.0/src/dq_check.egg-info/PKG-INFO` & `dq_check-0.3.1/src/dq_check.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_check
-Version: 0.3.0
+Version: 0.3.1
 Summary: A data quality check module for Spark
 Author-email: rohan goel <rohan.goel@databricks.com>
 Description-Content-Type: text/markdown
 Requires-Dist: pyspark
 Requires-Dist: pandas
 
 ## dq_check
```

