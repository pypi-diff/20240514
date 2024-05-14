# Comparing `tmp/fastapi_storage_helper-0.0.6.tar.gz` & `tmp/fastapi_storage_helper-0.0.7.tar.gz`

## Comparing `fastapi_storage_helper-0.0.6.tar` & `fastapi_storage_helper-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/build_and_publish.sh
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/build_and_test.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/pytest.ini
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/readme.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/requirements.txt
--rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/startup.sh
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/tox.ini
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/.github/workflows/publish.yaml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/fastapi_storage_helper/__init__.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/fastapi_storage_helper/storage.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/.gitignore
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/README.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/build_and_publish.sh
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/build_and_test.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/pytest.ini
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/readme.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/requirements.txt
+-rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/startup.sh
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/tox.ini
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/fastapi_storage_helper/__init__.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/fastapi_storage_helper/storage.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/.gitignore
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/README.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.7/PKG-INFO
```

### Comparing `fastapi_storage_helper-0.0.6/.github/workflows/publish.yaml` & `fastapi_storage_helper-0.0.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_storage_helper-0.0.6/fastapi_storage_helper/storage.py` & `fastapi_storage_helper-0.0.7/fastapi_storage_helper/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         )
 
     # Use boto2 to resolve performance issue
     def create_read_presign_url(self, key: str):
         return self.s3_v2.generate_url(7 * 24 * 60 * 60, 'GET', bucket=self.bucket, key=key, query_auth=True)
 
     def create_read_nerver_expired_presign_url(self, key: str):
-        expiration = 100 * 365 * 7 * 24 * 60 * 60
+        expiration = 1 * 365 * 7 * 24 * 60 * 60
         return self.s3_v2.generate_url(expiration, 'GET', bucket=self.bucket, key=key, query_auth=True)
 
     def get_metadata(self, path: str):
         return self.s3.head_object(Bucket=self.bucket, Key=path).get('Metadata')
 
     def upload_file_to_s3(self, file_path: str, s3_path: str):
         try:
```

### Comparing `fastapi_storage_helper-0.0.6/.gitignore` & `fastapi_storage_helper-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_storage_helper-0.0.6/pyproject.toml` & `fastapi_storage_helper-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_storage_helper"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Dzung Nguyen", email="dung@megatron-solutions.com" },
 ]
 description = "FastAPI Storage Helper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `fastapi_storage_helper-0.0.6/PKG-INFO` & `fastapi_storage_helper-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fastapi_storage_helper
-Version: 0.0.6
+Version: 0.0.7
 Summary: FastAPI Storage Helper
 Project-URL: Homepage, https://github.com/megatron-global/fastapi-queue
 Project-URL: Bug Tracker, https://github.com/megatron-global/fastapi-queue/issues
 Author-email: Dzung Nguyen <dung@megatron-solutions.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

