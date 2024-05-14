# Comparing `tmp/oip_tracking_client-0.0.3-py3-none-any.whl.zip` & `tmp/oip_tracking_client-0.0.3.dev0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17515 bytes, number of entries: 9
+Zip file size: 17352 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-14 15:48 oip_tracking_client/__init__.py
 -rw-r--r--  2.0 unx     5256 b- defN 24-Mar-08 06:51 oip_tracking_client/lib.py
 -rw-r--r--  2.0 unx     5459 b- defN 24-Mar-08 06:06 oip_tracking_client/rest.py
--rw-r--r--  2.0 unx    10962 b- defN 24-May-11 15:33 oip_tracking_client/tracking.py
+-rw-r--r--  2.0 unx    10205 b- defN 24-Apr-15 06:42 oip_tracking_client/tracking.py
 -rw-r--r--  2.0 unx    21096 b- defN 24-Mar-08 06:06 oip_tracking_client/wavfile.py
--rw-r--r--  2.0 unx     5609 b- defN 24-May-14 09:42 oip_tracking_client-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 09:42 oip_tracking_client-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 24-May-14 09:42 oip_tracking_client-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      775 b- defN 24-May-14 09:42 oip_tracking_client-0.0.3.dist-info/RECORD
-9 files, 49269 bytes uncompressed, 16167 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx     5614 b- defN 24-Apr-15 06:50 oip_tracking_client-0.0.3.dev0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 06:50 oip_tracking_client-0.0.3.dev0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-15 06:50 oip_tracking_client-0.0.3.dev0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      795 b- defN 24-Apr-15 06:50 oip_tracking_client-0.0.3.dev0.dist-info/RECORD
+9 files, 48537 bytes uncompressed, 15964 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: oip_tracking_client/tracking.py
 Comment: 
 
 Filename: oip_tracking_client/wavfile.py
 Comment: 
 
-Filename: oip_tracking_client-0.0.3.dist-info/METADATA
+Filename: oip_tracking_client-0.0.3.dev0.dist-info/METADATA
 Comment: 
 
-Filename: oip_tracking_client-0.0.3.dist-info/WHEEL
+Filename: oip_tracking_client-0.0.3.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: oip_tracking_client-0.0.3.dist-info/top_level.txt
+Filename: oip_tracking_client-0.0.3.dev0.dist-info/top_level.txt
 Comment: 
 
-Filename: oip_tracking_client-0.0.3.dist-info/RECORD
+Filename: oip_tracking_client-0.0.3.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oip_tracking_client/tracking.py

```diff
@@ -1,9 +1,8 @@
 import mlflow
-from urllib.parse import urlparse
 import os
 from PIL.Image import Image
 import numpy as np
 from matplotlib.figure import Figure
 from plotly.graph_objects import Figure as FigureP
 import io
 import json
@@ -91,37 +90,16 @@
         # If the attribute is a module, wrap it using ModuleWrapper
         if type(mlflow_attr).__name__ == "module":
             return ModuleWrapper(mlflow_attr)
 
         return mlflow_attr
 
 
-from contextlib import contextmanager
-
-
 class TrackingClient(metaclass=TrackingClientMeta):
     @staticmethod
-    @contextmanager
-    def start_run():
-        with mlflow.start_run() as run:
-
-            parsed_host_url = urlparse(os.environ["OIP_API_HOST"])
-            platform_url = f"{parsed_host_url.scheme}://{parsed_host_url.hostname}"
-            workspace_id = os.environ["WORKSPACE_ID"]
-            exp_id = run.info.experiment_id
-            run_id = run.info.run_id
-            exp_url = f"{platform_url}/ws/{workspace_id}/tracking/experiments/{exp_id}/overview"
-            run_url = f"{platform_url}/ws/{workspace_id}/tracking/experiments/{exp_id}/run/{run_id}"
-
-            print(f"View experiment at: {exp_url}")
-            print(f"View run at: {run_url}")
-
-            yield run
-
-    @staticmethod
     def connect(api_host: str, api_key: str, workspace_name: str):
         """
         Connect to the remove MLOPS platform
         It will check if the workspace exists and get its id
         Then set the the api host, the workspace id, and the api key
         :param api_host: str: The API Host
         :param api_key: str: The API Key
@@ -274,15 +252,17 @@
         md5_hash: str = hashlib.md5(serialized_data).hexdigest()
         file_name: str = f"{md5_hash}.json"
         artifact_path: str = f"llm_predictions/step_{str(int(step))}/{file_name}"
         mlflow.log_dict(dictionary, artifact_path)
 
     @staticmethod
     def log_audio_at_step(
-        data: Union[np.ndarray],
+        data: Union[
+            np.ndarray,
+        ],
         file_name: str,
         step: int,
         rate: int = None,
         extra: Optional[Dict[str, Any]] = None,
     ) -> None:
 
         audio_formats = ("mp3", "wav", "flac")
```

## Comparing `oip_tracking_client-0.0.3.dist-info/METADATA` & `oip_tracking_client-0.0.3.dev0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oip-tracking-client
-Version: 0.0.3
+Version: 0.0.3.dev0
 Summary: This is the API client of Open Innovation Platform - Tracking
 Author: Rachid Belmeskine
 Author-email: rachid.belmeskine@gmail.com
 License: PRIVATE LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

## Comparing `oip_tracking_client-0.0.3.dist-info/RECORD` & `oip_tracking_client-0.0.3.dev0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 oip_tracking_client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oip_tracking_client/lib.py,sha256=ujU_bQ6ix7noiiXpje0ZKyhJpJKi4tM0ukYQVYlbUIw,5256
 oip_tracking_client/rest.py,sha256=IKs8uipUKPIW3VG8dbKIxkclxlVXpaBQElUpy0cQ5Hw,5459
-oip_tracking_client/tracking.py,sha256=Oo3qmNiFTWJo74bGknYGabaK3fOar03Nk97zqxJsPE4,10962
+oip_tracking_client/tracking.py,sha256=jh24V-c1sofJQbecaQSr4qq5CBO9FKWDYCu2oipLM2g,10205
 oip_tracking_client/wavfile.py,sha256=vAYY3NF0KZ-wP0VLCMcya0_99OtNGcoWP5XOeyZfF2g,21096
-oip_tracking_client-0.0.3.dist-info/METADATA,sha256=kVj0c4n15I-p8OTXPogB66M4mkZQ64D6OPlYK5iUOA4,5609
-oip_tracking_client-0.0.3.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-oip_tracking_client-0.0.3.dist-info/top_level.txt,sha256=TlX4Qx0OtAJefucshHIOZ2z8FR8BF-Us-9af0zLI3Uc,20
-oip_tracking_client-0.0.3.dist-info/RECORD,,
+oip_tracking_client-0.0.3.dev0.dist-info/METADATA,sha256=3kQPnTPDUhoZbNjlueT1S7ABJidWicrprxI7yweN3s8,5614
+oip_tracking_client-0.0.3.dev0.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+oip_tracking_client-0.0.3.dev0.dist-info/top_level.txt,sha256=TlX4Qx0OtAJefucshHIOZ2z8FR8BF-Us-9af0zLI3Uc,20
+oip_tracking_client-0.0.3.dev0.dist-info/RECORD,,
```

