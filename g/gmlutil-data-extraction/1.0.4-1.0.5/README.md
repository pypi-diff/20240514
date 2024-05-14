# Comparing `tmp/gmlutil-data-extraction-1.0.4.tar.gz` & `tmp/gmlutil-data-extraction-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmlutil-data-extraction-1.0.4.tar", last modified: Mon May 13 20:59:23 2024, max compression
+gzip compressed data, was "gmlutil-data-extraction-1.0.5.tar", last modified: Tue May 14 21:22:13 2024, max compression
```

## Comparing `gmlutil-data-extraction-1.0.4.tar` & `gmlutil-data-extraction-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        0 2024-05-13 20:59:23.125176 gmlutil-data-extraction-1.0.4/
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      767 2024-05-13 20:59:23.124941 gmlutil-data-extraction-1.0.4/PKG-INFO
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)     6303 2024-02-22 22:08:31.000000 gmlutil-data-extraction-1.0.4/README.md
-drwxr-xr-x   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        0 2024-05-13 20:59:23.108708 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction/
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      162 2024-02-13 01:11:59.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction/config.py
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)    19450 2024-05-13 20:50:24.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction/data_extraction.py
-drwxr-xr-x   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        0 2024-05-13 20:59:23.124626 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      767 2024-05-13 20:59:23.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/PKG-INFO
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      329 2024-05-13 20:59:23.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/SOURCES.txt
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        1 2024-05-13 20:59:23.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/dependency_links.txt
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      315 2024-05-13 20:59:23.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/requires.txt
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)       24 2024-05-13 20:59:23.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/top_level.txt
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)       38 2024-05-13 20:59:23.125224 gmlutil-data-extraction-1.0.4/setup.cfg
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)     1387 2024-05-13 20:59:12.000000 gmlutil-data-extraction-1.0.4/setup.py
+drwxr-xr-x   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        0 2024-05-14 21:22:13.097026 gmlutil-data-extraction-1.0.5/
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      767 2024-05-14 21:22:13.096678 gmlutil-data-extraction-1.0.5/PKG-INFO
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)     6303 2024-02-22 22:08:31.000000 gmlutil-data-extraction-1.0.5/README.md
+drwxr-xr-x   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        0 2024-05-14 21:22:13.093208 gmlutil-data-extraction-1.0.5/gmlutil_data_extraction/
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      162 2024-02-13 01:11:59.000000 gmlutil-data-extraction-1.0.5/gmlutil_data_extraction/config.py
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)    19567 2024-05-14 21:18:38.000000 gmlutil-data-extraction-1.0.5/gmlutil_data_extraction/data_extraction.py
+drwxr-xr-x   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        0 2024-05-14 21:22:13.096063 gmlutil-data-extraction-1.0.5/gmlutil_data_extraction.egg-info/
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      767 2024-05-14 21:22:12.000000 gmlutil-data-extraction-1.0.5/gmlutil_data_extraction.egg-info/PKG-INFO
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      329 2024-05-14 21:22:12.000000 gmlutil-data-extraction-1.0.5/gmlutil_data_extraction.egg-info/SOURCES.txt
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        1 2024-05-14 21:22:12.000000 gmlutil-data-extraction-1.0.5/gmlutil_data_extraction.egg-info/dependency_links.txt
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      315 2024-05-14 21:22:12.000000 gmlutil-data-extraction-1.0.5/gmlutil_data_extraction.egg-info/requires.txt
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)       24 2024-05-14 21:22:12.000000 gmlutil-data-extraction-1.0.5/gmlutil_data_extraction.egg-info/top_level.txt
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)       38 2024-05-14 21:22:13.097129 gmlutil-data-extraction-1.0.5/setup.cfg
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)     1387 2024-05-14 21:17:03.000000 gmlutil-data-extraction-1.0.5/setup.py
```

### Comparing `gmlutil-data-extraction-1.0.4/PKG-INFO` & `gmlutil-data-extraction-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmlutil-data-extraction
-Version: 1.0.4
+Version: 1.0.5
 Summary: General Machine Learning Utility Package for Data Extraction
 Home-page: https://github.com/Phillip1982/gmlutil_data_extraction
 Author: Phillip Kim
 Author-email: phillip.kim@ejgallo.com
 License: BSD 2-clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `gmlutil-data-extraction-1.0.4/README.md` & `gmlutil-data-extraction-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gmlutil-data-extraction-1.0.4/gmlutil_data_extraction/data_extraction.py` & `gmlutil-data-extraction-1.0.5/gmlutil_data_extraction/data_extraction.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,16 +77,16 @@
                             user=cred.GCO_USERNAME, 
                             password = cred.GCO_PASSWORD, 
                             database = cred.GCO_DATABASE, # 'IRIGCO', 
                             port = cred.GCO_PORT) # 61433)
         return conn
 
 
-    def rs_connection(self):
-        engine_string = 'redshift+psycopg2://{}:{}@{}'.format(credr.username, credr.password, credr.host + ":" + credr.port + "/" + credr.dbName)
+    def rs_connection(self, username=credr.username, password=credr.password, host=credr.host, port=credr.port, dbName=credr.dbName):
+        engine_string = 'redshift+psycopg2://{}:{}@{}'.format(username, password, host + ":" + port + "/" + dbName)
         conn = create_engine(engine_string)
         return conn
 
     
     def get_category(self, sub, cat):
         if self.dsrc == 'sgws':
             if sub in ['SPARKLING WINE']:
@@ -345,16 +345,16 @@
         """
         upc_df = self.read_from_s3(bucket_name, file_name)
         # Add leading zeros to UPC to match Gallo data
         upc_df['UPC'] = upc_df['UPC'].astype(int).astype(str).str.rjust(12, "0")
         return upc_df
 
 
-    def upload_to_rs(self, bucket_name, file_name, table_name=credr.winegrowing_table, host = credr.winegrowing_host, database = credr.winegrowing_database, user = credr.winegrowing_user, password = credr.winegrowing_password): # prophet/Deployment/DS_Collab/winegrowing_research/GQI/model_outputs/gqi_calc.csv
-        rs_push_query = """call """ + table_name + """.copy_gqi_calc('s3://"""+ bucket_name + """/""" + file_name + """')"""
+    def upload_to_rs(self, bucket_name, file_name, copy_function='copy_gqi_calc', table_name=credr.winegrowing_table, host = credr.winegrowing_host, database = credr.winegrowing_database, user = credr.winegrowing_user, password = credr.winegrowing_password): # prophet/Deployment/DS_Collab/winegrowing_research/GQI/model_outputs/gqi_calc.csv
+        rs_push_query = """call """ + table_name + """.{}('s3://""".format(copy_function)+ bucket_name + """/""" + file_name + """')"""
         conn_redshift = redshift_connector.connect(
             host = host,
             database = database,
             user = user,
             password = password
         )
         cursor = conn_redshift.cursor()
```

### Comparing `gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/PKG-INFO` & `gmlutil-data-extraction-1.0.5/gmlutil_data_extraction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmlutil-data-extraction
-Version: 1.0.4
+Version: 1.0.5
 Summary: General Machine Learning Utility Package for Data Extraction
 Home-page: https://github.com/Phillip1982/gmlutil_data_extraction
 Author: Phillip Kim
 Author-email: phillip.kim@ejgallo.com
 License: BSD 2-clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `gmlutil-data-extraction-1.0.4/setup.py` & `gmlutil-data-extraction-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='gmlutil-data-extraction',
-    version='1.0.4',    
+    version='1.0.5',    
     description='General Machine Learning Utility Package for Data Extraction',
     url='https://github.com/Phillip1982/gmlutil_data_extraction',
     author='Phillip Kim',
     author_email='phillip.kim@ejgallo.com',
     license='BSD 2-clause', ## Change this
     packages=['gmlutil_data_extraction'],
     install_requires=[ # package>=0.2,<0.3
```

