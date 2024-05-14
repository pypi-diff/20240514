# Comparing `tmp/rov_db_access-0.1.6.tar.gz` & `tmp/rov_db_access-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rov_db_access-0.1.6.tar", max compression
+gzip compressed data, was "rov_db_access-0.1.7.tar", max compression
```

## Comparing `rov_db_access-0.1.6.tar` & `rov_db_access-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      453 2024-05-08 20:09:03.117867 rov_db_access-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-28 21:38:40.450138 rov_db_access-0.1.6/README.md
--rw-r--r--   0        0        0      359 2024-05-07 17:08:16.858586 rov_db_access-0.1.6/rov_db_access/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 20:09:14.778226 rov_db_access-0.1.6/rov_db_access/authentication/__init__.py
--rw-r--r--   0        0        0     2324 2024-05-07 15:18:49.279026 rov_db_access-0.1.6/rov_db_access/authentication/models.py
--rw-r--r--   0        0        0     1756 2024-05-07 16:22:22.222344 rov_db_access-0.1.6/rov_db_access/authentication/worker.py
--rw-r--r--   0        0        0      675 2024-05-07 16:39:33.493938 rov_db_access-0.1.6/rov_db_access/config/db_utils.py
--rw-r--r--   0        0        0     1122 2024-05-08 20:09:03.118984 rov_db_access-0.1.6/rov_db_access/config/settings.py
--rw-r--r--   0        0        0        0 2024-04-19 20:09:14.782941 rov_db_access-0.1.6/rov_db_access/gis/__init__.py
--rw-r--r--   0        0        0     7207 2024-05-08 20:09:03.119358 rov_db_access-0.1.6/rov_db_access/gis/models.py
--rw-r--r--   0        0        0    24897 2024-05-08 20:09:03.119358 rov_db_access-0.1.6/rov_db_access/gis/worker.py
--rw-r--r--   0        0        0        0 2024-04-19 20:09:14.791048 rov_db_access-0.1.6/rov_db_access/sentinel/__init__.py
--rw-r--r--   0        0        0      427 2024-04-19 20:09:14.792050 rov_db_access-0.1.6/rov_db_access/sentinel/models.py
--rw-r--r--   0        0        0     2984 2024-05-07 16:21:41.802152 rov_db_access-0.1.6/rov_db_access/sentinel/worker.py
--rw-r--r--   0        0        0     1531 2024-05-08 20:09:03.120864 rov_db_access-0.1.6/rov_db_access/utils/s3_utils.py
--rw-r--r--   0        0        0     1155 2024-05-08 20:09:03.120864 rov_db_access-0.1.6/rov_db_access/utils/utils.py
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 rov_db_access-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      453 2024-05-14 15:53:52.686829 rov_db_access-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-28 21:38:40.450138 rov_db_access-0.1.7/README.md
+-rw-r--r--   0        0        0      359 2024-05-07 17:08:16.858586 rov_db_access-0.1.7/rov_db_access/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.778226 rov_db_access-0.1.7/rov_db_access/authentication/__init__.py
+-rw-r--r--   0        0        0     2324 2024-05-07 15:18:49.279026 rov_db_access-0.1.7/rov_db_access/authentication/models.py
+-rw-r--r--   0        0        0     1756 2024-05-07 16:22:22.222344 rov_db_access-0.1.7/rov_db_access/authentication/worker.py
+-rw-r--r--   0        0        0     2133 2024-05-14 15:53:52.686829 rov_db_access-0.1.7/rov_db_access/config/db_utils.py
+-rw-r--r--   0        0        0     1122 2024-05-08 20:09:03.118984 rov_db_access-0.1.7/rov_db_access/config/settings.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.782941 rov_db_access-0.1.7/rov_db_access/gis/__init__.py
+-rw-r--r--   0        0        0     7207 2024-05-08 20:09:03.119358 rov_db_access-0.1.7/rov_db_access/gis/models.py
+-rw-r--r--   0        0        0    25083 2024-05-14 15:53:52.686829 rov_db_access-0.1.7/rov_db_access/gis/worker.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.791048 rov_db_access-0.1.7/rov_db_access/sentinel/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-19 20:09:14.792050 rov_db_access-0.1.7/rov_db_access/sentinel/models.py
+-rw-r--r--   0        0        0     2984 2024-05-07 16:21:41.802152 rov_db_access-0.1.7/rov_db_access/sentinel/worker.py
+-rw-r--r--   0        0        0     1531 2024-05-08 20:09:03.120864 rov_db_access-0.1.7/rov_db_access/utils/s3_utils.py
+-rw-r--r--   0        0        0     1155 2024-05-08 20:09:03.120864 rov_db_access-0.1.7/rov_db_access/utils/utils.py
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 rov_db_access-0.1.7/PKG-INFO
```

### Comparing `rov_db_access-0.1.6/rov_db_access/authentication/models.py` & `rov_db_access-0.1.7/rov_db_access/authentication/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.6/rov_db_access/authentication/worker.py` & `rov_db_access-0.1.7/rov_db_access/authentication/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.6/rov_db_access/config/settings.py` & `rov_db_access-0.1.7/rov_db_access/config/settings.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.6/rov_db_access/gis/models.py` & `rov_db_access-0.1.7/rov_db_access/gis/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.6/rov_db_access/gis/worker.py` & `rov_db_access-0.1.7/rov_db_access/gis/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
-from typing import TypedDict, List, Optional
+from typing import Literal, TypedDict, List, Optional
 
 import boto3
 import hashlib
 from botocore.client import Config
 from botocore.exceptions import ClientError
 
 from rov_db_access.authentication.models import User
 from rov_db_access.utils.s3_utils import S3Client
 from rov_db_access.utils.utils import wkbelement_to_wkt
-from rov_db_access.config.db_utils import init_db_engine
+from rov_db_access.config.db_utils import BaseWorker
 from rov_db_access.config.settings import Settings
 from rov_db_access.sentinel.worker import is_valid_uuid
-from sqlalchemy.orm import Session
 from rov_db_access.gis.models import Process, Image, InferenceModel, Input, ResultsRaster, Run, ResultsRaw
 from sqlalchemy import select, and_, func
 
 settings = Settings()
 
 CreateProcessDict = TypedDict("CreateProcessDict", {
     "name": str,
@@ -80,26 +79,24 @@
         return None
 
 
 def get_date(obj):
     return tuple(map(int, obj["date"].split("/")[::-1]))
 
 
-class GisWorker:
+class GisWorker(BaseWorker):
 
     def __init__(self) -> None:
-
-        self.engine = init_db_engine(
+        super().__init__(
             settings.db_rov_gis_user,
             settings.db_rov_gis_password,
             settings.db_rov_gis_host,
             settings.db_rov_gis_port,
             settings.db_rov_gis_database
         )
-        self.session = Session(self.engine)
 
     def create_process(self, data: CreateProcessDict, user: User):
         name = data["name"]
         inference_model_id = data["inference_model_id"]
         area = data["area"]
         cost_estimated = data["cost_estimated"]
         images = data["images"]
@@ -586,54 +583,36 @@
         self.session.add(new_image)
         self.session.commit()
         return new_image
 
     def upload_run_results(self, run_id: int, runtime: float, files_path: str, raster_name: str=None, file_names: list[str]=[], data: dict=None, bbox: str=None):
         """
         Uploads the files to the S3 bucket and updates the run status to finished
-        :param run_id: The id of the run
-        :param files_path: The path where the files are located
-        :param runtime: The runtime of the run
-        :param raster_name: The name of the raster file
-        :param file_names: Array with the names of additional files to upload
-        :param data: additional data to store in the results raster table
-        :param bbox: The bbox of the raster
+
+        Args:
+            run_id: The id of the run
+            files_path: The path where the files are located
+            runtime: The runtime of the run
+            raster_name: The name of the raster file
+            file_names: Array with the names of additional files to upload
+            data: additional data to store in the results raster table
+            bbox: The bbox of the raster
         """
-        #check data
-        if not isinstance(run_id, int):
-            print('Invalid run_id!')
-            return False
-        if isinstance(runtime, int):
-            try:
-                runtime = float(runtime)
-            except:
-                print('Invalid runtime!')
-                return False
-        if not isinstance(runtime, float):
-            print('Invalid runtime!')
-            return False
-        if not isinstance(files_path, str):
-            print('Invalid files_path!')
-            return False
-        if raster_name is not None and not isinstance(raster_name, str):
-            print('Invalid raster_name!')
-            return False
-        if not isinstance(file_names, list):
-            print('Invalid file_names!')
-            return False
-        if data is not None and not isinstance(data, dict):
-            print('Invalid data!')
-            return False
-        if bbox is not None and not isinstance(bbox, str):
-            print('Invalid bbox!')
-            return False
+        assert isinstance(run_id, int), 'Invalid run_id!'
+        assert isinstance(runtime, (int, float)), 'Invalid runtime!'
+        runtime = float(runtime)
+        assert isinstance(files_path, str), 'Invalid files_path!'
+        assert raster_name is None or isinstance(raster_name, str), 'Invalid raster_name!'
+        assert isinstance(file_names, list), 'Invalid file_names!'
+        assert data is None or isinstance(data, dict), 'Invalid data!'
+        assert bbox is None or isinstance(bbox, str), 'Invalid bbox!'
 
-        if raster_name is None and len(file_names) == 0:
-            print('No files to upload!')
-            return False
+        assert raster_name is not None or len(file_names) != 0, 'No files to upload!'
+
+        self.check_db_connection()
 
         # actual function
         query = (
             select(Run)
             .where(Run.id == run_id)
             .limit(1)
         )
@@ -655,22 +634,22 @@
 
         for file_name in file_names:
             if not isinstance(file_name, str):
                 print('Invalid file_name!')
                 return False
             print(f'Uploading file: {file_name}')
             object_key = bucket_base_directory + file_name
-            file_path = files_path + file_name
+            file_path = os.path.join(files_path, file_name)
             s3_client.upload_file(file_path, object_key)
             print(f'File uploaded to S3 with key: {object_key}')
 
         if raster_name is not None:
             print(f'Uploading raster file: {raster_name}')
             object_key = bucket_base_directory + raster_name
-            file_path = files_path + raster_name
+            file_path = os.path.join(files_path, raster_name)
             s3_client.upload_file(file_path, object_key)
             print(f'File uploaded to S3 with key: {object_key}')
             self.add_results_raster(run_id, object_key, data, bbox)
 
         # update run status
         run.status = 'finished'
         run.finished_at = func.now()
@@ -686,7 +665,31 @@
             data=data,
             bbox=bbox,
             run_id=run_id
         )
         self.session.add(new_result)
         self.session.commit()
         return new_result
+
+    def update_run_status(self, run_id: int, status: Literal['queued', 'running', 'finished']):
+        """
+        Updates the status of the run
+
+        Args:
+            run_id: The id of the run
+            status: The new status of the run
+        """
+        assert isinstance(run_id, int), 'Invalid run_id!'
+        assert status in ['queued', 'running', 'finished'], 'Invalid status!'
+
+        query = (
+            select(Run)
+            .where(Run.id == run_id)
+            .limit(1)
+        )
+        run = self.session.scalar(query)
+        if run is None:
+            print(f'No run with id ${run_id} found!')
+            return False
+        run.status = status
+        self.session.commit()
+        return True
```

### Comparing `rov_db_access-0.1.6/rov_db_access/sentinel/worker.py` & `rov_db_access-0.1.7/rov_db_access/sentinel/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.6/rov_db_access/utils/s3_utils.py` & `rov_db_access-0.1.7/rov_db_access/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.6/rov_db_access/utils/utils.py` & `rov_db_access-0.1.7/rov_db_access/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.6/PKG-INFO` & `rov_db_access-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rov-db-access
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Pablo Cano
 Author-email: pablo.cano@rovisen.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

