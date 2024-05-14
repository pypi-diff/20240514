# Comparing `tmp/gen_wrappers-0.3.5.tar.gz` & `tmp/gen_wrappers-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.3.5.tar", last modified: Tue May 14 14:50:06 2024, max compression
+gzip compressed data, was "gen_wrappers-0.3.6.tar", last modified: Tue May 14 15:44:03 2024, max compression
```

## Comparing `gen_wrappers-0.3.5.tar` & `gen_wrappers-0.3.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.075251 gen_wrappers-0.3.5/
--rw-rw-rw-   0        0        0      847 2024-05-14 14:50:06.073248 gen_wrappers-0.3.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.030549 gen_wrappers-0.3.5/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.5/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.044510 gen_wrappers-0.3.5/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.5/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     6625 2024-05-11 17:01:23.000000 gen_wrappers-0.3.5/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.3.5/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.5/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.049759 gen_wrappers-0.3.5/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.5/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.3.5/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.5/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.5/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.5/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.053764 gen_wrappers-0.3.5/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.5/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9561 2024-05-11 17:02:29.000000 gen_wrappers-0.3.5/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0    10277 2024-05-14 14:43:03.000000 gen_wrappers-0.3.5/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.5/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.058765 gen_wrappers-0.3.5/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.5/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6345 2024-05-11 17:04:12.000000 gen_wrappers-0.3.5/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.5/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.5/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.059765 gen_wrappers-0.3.5/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.5/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.3.5/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.072250 gen_wrappers-0.3.5/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-14 14:50:05.000000 gen_wrappers-0.3.5/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-14 14:50:05.000000 gen_wrappers-0.3.5/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 14:50:05.000000 gen_wrappers-0.3.5/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-14 14:50:05.000000 gen_wrappers-0.3.5/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 14:50:05.000000 gen_wrappers-0.3.5/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 14:50:06.075251 gen_wrappers-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-14 14:47:27.000000 gen_wrappers-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.468173 gen_wrappers-0.3.6/
+-rw-rw-rw-   0        0        0      847 2024-05-14 15:44:03.467173 gen_wrappers-0.3.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.361285 gen_wrappers-0.3.6/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.6/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.370824 gen_wrappers-0.3.6/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.6/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     5302 2024-05-14 15:42:23.000000 gen_wrappers-0.3.6/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     3971 2024-05-14 15:19:49.000000 gen_wrappers-0.3.6/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.6/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.391447 gen_wrappers-0.3.6/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.6/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1491 2024-05-14 15:42:23.000000 gen_wrappers-0.3.6/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.6/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.6/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.6/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.410594 gen_wrappers-0.3.6/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.6/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9489 2024-05-14 15:42:23.000000 gen_wrappers-0.3.6/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    10277 2024-05-14 14:43:03.000000 gen_wrappers-0.3.6/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.6/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.430593 gen_wrappers-0.3.6/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.6/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6273 2024-05-14 15:42:23.000000 gen_wrappers-0.3.6/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.6/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.6/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.439618 gen_wrappers-0.3.6/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.6/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.3.6/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.466172 gen_wrappers-0.3.6/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-14 15:44:03.000000 gen_wrappers-0.3.6/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-14 15:44:03.000000 gen_wrappers-0.3.6/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 15:44:03.000000 gen_wrappers-0.3.6/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-14 15:44:03.000000 gen_wrappers-0.3.6/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 15:44:03.000000 gen_wrappers-0.3.6/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 15:44:03.469173 gen_wrappers-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-14 15:43:58.000000 gen_wrappers-0.3.6/setup.py
```

### Comparing `gen_wrappers-0.3.5/PKG-INFO` & `gen_wrappers-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.3.5
+Version: 0.3.6
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.5/creator/auto/creator_auto.py` & `gen_wrappers-0.3.6/creator/fcus_api/creator_fcus_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,137 @@
 import asyncio
+import json
 import logging
 import os
-import random
-import traceback
-from typing import Any, List, Union
+from typing import Any, Union, List
 
 import httpx
+import requests
 
-from creator.auto.request_auto import AutoTxt2Img, AutoModelLoad, AutoImg2Img, AutoSchedTxt2Img
-from creator.auto.response_auto import ResponseAuto
 from creator.base.base_app import BaseApp
-from creator.base.base_response import BaseResponse
+from creator.base.base_request import BaseRequest
+from creator.base.base_response import BaseResponse, ResponseDataType, ResponseData
+from creator.fcus_api.request_fcus_api import FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint
+from creator.fcus_api.response_fcus_api import ResponseFcusApi
 
 logger = logging.getLogger(__name__)
 
 
-class AppAuto(BaseApp):
-    param_classes = [AutoTxt2Img, AutoImg2Img, AutoSchedTxt2Img]
+class AppFcusApi(BaseApp):
+    param_classes = [FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint]
     output = {}
-    jobs = {}
-    sched_jobs = {}
 
     def __init__(self):
         super().__init__()
-        auto_port = os.environ.get("PORT_AUTO", 8081)
-        if isinstance(auto_port, str):
-            auto_port = int(auto_port)
-        self.jobs = {}
-        self.output = {}
-        self.api_base_url = f"http://0.0.0.0:{auto_port}/sdapi"
-
-    async def create(self, params: Union[AutoTxt2Img, AutoImg2Img, AutoSchedTxt2Img], job_id=None) -> BaseResponse:
-        print(f"Creating job with params: {params}")
-        endpoint_name = "txt2img" if isinstance(params, AutoTxt2Img) else "img2img"
-        url = f"{self.api_base_url}/sdapi/v1/{endpoint_name}"
-        get_task_id = False
-        if isinstance(params, AutoSchedTxt2Img):
-            url = f"{self.api_base_url}/agent-scheduler/v1/queue/tx2img"
-            get_task_id = True
-        data = params.__dict__
-        headers = {'Content-Type': 'application/json'}
-        async with httpx.AsyncClient() as client:
-            response = await client.post(url, data=data, headers=headers)
-            response.raise_for_status()
-        output = response.json()
-        print(f"Response received: {output}")
-        if job_id:
-            self.output[job_id] = output
-        self.jobs[job_id] = output
-        return ResponseAuto.parse_response(output, job_id)
-
-    async def create_async(self, params: Union[AutoTxt2Img, AutoImg2Img, AutoSchedTxt2Img]) -> BaseResponse:
-        job_id = str(random.randint(0, 100000))
-        print(f"Creating job with ID {job_id}")
+        focus_port = os.environ.get("PORT_FCUS_API", 8888)
+        if isinstance(focus_port, str):
+            focus_port = int(focus_port)
+        self.api_base_url = f"http://0.0.0.0:{focus_port}"
+
+    async def create(self, params: Union[FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint]) -> BaseResponse:
+        if isinstance(params, FcusTxt2Img):
+            url = f"{self.api_base_url}/v1/generation/text-to-image"
+        elif isinstance(params, FcusUpscaleOrVary):
+            url = f"{self.api_base_url}/v1/generation/image-upscale-vary"
+        elif isinstance(params, FcusInpaintOrOutpaint):
+            url = f"{self.api_base_url}/v1/generation/image-inpaint-outpaint"
+        else:
+            raise ValueError("Invalid parameters for creation")
 
-        # Store the job_id immediately with a placeholder to indicate it's pending
-        self.output[job_id] = {"status": "pending"}
-
-        # Fire off the job without waiting for it to complete
-        asyncio.create_task(self._create_job(params, job_id, self.output))
+        data = json.dumps(params.__dict__)
+        headers = {'Content-Type': 'application/json'}
+        response = requests.post(url, data=data, headers=headers)
+        # If we have a 422 here, print what the unprocessable entity is
+        if response.status_code == 422:
+            logger.warning(f"Unprocessable entity: {response.text}")
+        response.raise_for_status()
+
+        self.output = response.json()
+        logger.debug(f"Response: {self.output}")
+        job_id = self.output.get('job_id', None)
+        output = None
+        if job_id is not None:
+            job_count = 0
+            while output is None and job_count < 60:
+                logger.debug(f"Job count: {job_count}")
+                output = await self._get_output(job_id)
+                job_count += 1
+                if output is None:
+                    await asyncio.sleep(1)
+            response_data = ResponseData(data=output, data_type=ResponseDataType.IMAGE, total_count=len(output))
+            return ResponseFcusApi(status="Job Finished", output=response_data, job_id=job_id)
+
+    async def create_async(self, params: Union[FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint]) -> BaseResponse:
+        if isinstance(params, FcusTxt2Img):
+            model = params.base_model_name
+            url = f"{self.api_base_url}/v1/generation/text-to-image"
+        elif isinstance(params, FcusUpscaleOrVary):
+            model = params.base_model_name
+            url = f"{self.api_base_url}/v1/generation/image-upscale-vary"
+        elif isinstance(params, FcusInpaintOrOutpaint):
+            model = params.base_model_name
+            url = f"{self.api_base_url}/v1/generation/image-inpaint-outpaint"
+        else:
+            raise ValueError("Invalid parameters for creation")
+        if model is not None and model not in self.loaded_models:
+            self.loaded_models.append(model)
+        max_cached_models = os.environ.get("MAX_CACHED_MODELS", 3)
+        if len(self.loaded_models) > max_cached_models:
+            self.loaded_models = self.loaded_models[-max_cached_models:]
 
-        print(f"Job {job_id} is running.")
-        return ResponseAuto.running(job_id)
+        data = json.dumps(params.model_dump())
+        headers = {'Content-Type': 'application/json'}
+        response = requests.post(url, data=data, headers=headers)
+        # If we have a 422 here, print what the unprocessable entity is
+        if response.status_code == 422:
+            logger.warning(f"Unprocessable entity: {response.text}")
+        response.raise_for_status()
+
+        self.output = response.json()
+        logger.debug(f"Response: {self.output}")
+        job_id = self.output.get('job_id', None)
+        if job_id is not None:
+            return ResponseFcusApi.running(job_id)
+        return ResponseFcusApi.error("Job ID not found", job_id)
 
     async def get_status(self, job_id: str) -> BaseResponse:
-        try:
-            output = self.output.get(job_id)
-            if output:
-                task_id = output.get("task_id")
-                if task_id:
-                    url = f"{self.api_base_url}/agent-scheduler/v1/queue/tx2img/{task_id}"
-                    async with httpx.AsyncClient() as client:
-                        response = await client.get(url)
-                        response.raise_for_status()
-                    output = response.json()
-                    return ResponseAuto.parse_response(output, job_id)
-            else:
-                # Check if the job resulted in an error
-                if "error" in output:
-                    print(f"Error found for job ID {job_id}")
-                    return ResponseAuto.error(output["error"], job_id)
-                print(f"Output found for job ID {job_id}")
-                return ResponseAuto.parse_response(output, job_id)
-
-            # If job_id is not in the jobs dictionary and no output is found, assume the job does not exist
-            if job_id not in self.jobs:
-                logger.warning(f"Job ID {job_id} not found")
-                return ResponseAuto.error(f"Job ID {job_id} not found", job_id)
-
-            # If the job is still in jobs but no output has been generated yet
-            print(f"Job {job_id} is still running.")
-            return ResponseAuto.running(job_id)
-
-        except Exception as e:
-            logger.error(f"Error getting job status for job ID {job_id}: {e}")
-            traceback.print_exc()
-            return ResponseAuto.error(f"Error getting job status: {e}", job_id)
-
-    async def get_models(self) -> List[Any]:
-        url = f"{self.api_base_url}/sdapi/v1/sd-models"
-        async with httpx.AsyncClient() as client:
-            response = await client.get(url)
-            response.raise_for_status()
-            response_json = response.json()
-        models = [model.get("title") for model in response_json if model.get("title")]
-        return models
+        output = await self._get_output(job_id)
+        if output is None:
+            return BaseResponse.error("Error getting job status")
+        if not output:
+            print(f"Job {job_id} is still running (or can't get output)")
+            return BaseResponse.running(job_id)
+        return BaseResponse.success(
+            ResponseData(data=output, data_type=ResponseDataType.IMAGE, total_count=len(output)))
 
-    # Assuming you will provide more detail or use this method later
     async def upload_image(self, image_data: Any) -> str:
         pass
 
-    async def select_model(self, params: AutoModelLoad):
-        model_to_load = params.sd_model_checkpoint
-        if model_to_load and model_to_load not in self.loaded_models:
-            self.loaded_models.append(model_to_load)
-        max_cached_models = os.environ.get("MAX_CACHED_MODELS", 3)
-        if len(self.loaded_models) > max_cached_models:
-            self.loaded_models = self.loaded_models[-max_cached_models:]
-        url = f"{self.api_base_url}/sdapi/v1/options"
-        headers = {'Content-Type': 'application/json'}
+    async def get_models(self) -> List[str]:
         async with httpx.AsyncClient() as client:
-            response = await client.post(url, data=params.__dict__, headers=headers)
+            response = await client.get(f"{self.api_base_url}/v1/engines/all-models")
             response.raise_for_status()
-            return response.json()
+            response_json = response.json()
+            return response_json.get("model_filenames", [])
 
     async def test(self):
-        auto_port = int(os.environ.get("PORT_AUTO", 8081))
-        url = f"http://0.0.0.0:{auto_port}/docs"
         async with httpx.AsyncClient() as client:
+            url = f"{self.api_base_url}/docs"
             response = await client.get(url)
             if response.status_code == 200:
                 return BaseResponse.active()
             else:
                 return BaseResponse.error("Error testing connection")
 
-    async def _create_job(self, params: AutoTxt2Img, job_id: str, output_store: dict):
-        url = f"{self.api_base_url}/v1/txt2img"  # Adjust URL as necessary
-        data = params.__dict__
-        headers = {'Content-Type': 'application/json'}
-        try:
-            async with httpx.AsyncClient() as client:
-                response = await client.post(url, data=data, headers=headers)
-                response.raise_for_status()
-            output = response.json()
-            print(f"Response received: {output}")
-            output_store[job_id] = output  # Storing output for future retrieval
-        except Exception as e:
-            print(f"Error in job {job_id}: {e}")
-            output_store[job_id] = {"error": str(e)}
+    async def _get_output(self, job_id: str) -> Union[None, List[str]]:
+        async with httpx.AsyncClient() as client:
+            response = await client.get(f"{self.api_base_url}/v1/generation/query-job", params={'job_id': job_id})
+            response.raise_for_status()
+            response_json = response.json()
+            status = response_json.get('job_status')
+            logger.debug(f"Status: {status}")
+            if status is None:
+                return None
+            if status != "Finished":
+                return []
+            outputs = [result.get('base64') for result in response_json.get('job_result', []) if result.get('finish_reason', "UNKNOWN") == "SUCCESS"]
+            return outputs
```

### Comparing `gen_wrappers-0.3.5/creator/auto/request_auto.py` & `gen_wrappers-0.3.6/creator/auto/request_auto.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,85 +7,87 @@
 
 class AutoTxt2Img(BaseRequest):
     prompt: str = Field("", examples=["A beautiful sunset over a mountain lake."])
     negative_prompt: str = ""
     styles: List[str] = Field(default_factory=list, examples=[[]])
     seed: int = -1
     subseed: int = -1
-    subseed_strength: float = 0.0
+    subseed_strength: int = 0
     seed_resize_from_h: int = -1
     seed_resize_from_w: int = -1
-    sampler_name: str = "Euler a"
+    sampler_name: str = "DPM++ 2M"
+    scheduler: str = ""
     batch_size: int = 1
     n_iter: int = 1
-    steps: int = 20
-    cfg_scale: float = 7.0
+    steps: int = 30
+    cfg_scale: int = 7.5
     width: int = 1024
     height: int = 768
     restore_faces: bool = False
     tiling: bool = False
     do_not_save_samples: bool = True
     do_not_save_grid: bool = True
-    eta: float = 0.0
-    denoising_strength: float = 0.7
-    s_min_uncond: float = 0.0
-    s_churn: float = 0.0
-    s_tmax: float = 0.0
-    s_tmin: float = 0.0
-    s_noise: float = 1.0
+    eta: int = 0
+    denoising_strength: int = 0
+    s_min_uncond: int = 0
+    s_churn: int = 0
+    s_tmax: int = 0
+    s_tmin: int = 0
+    s_noise: int = 0
     override_settings: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
     override_settings_restore_afterwards: bool = True
     refiner_checkpoint: str = ""
     refiner_switch_at: int = 0
     disable_extra_networks: bool = False
     firstpass_image: str = ""
-    comments: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
+    comments: Dict[str, Any] = {}
     enable_hr: bool = False
     firstphase_width: int = 0
     firstphase_height: int = 0
     hr_scale: int = 2
-    hr_upscaler: str = "Latent"
+    hr_upscaler: str = ""
     hr_second_pass_steps: int = 0
     hr_resize_x: int = 0
     hr_resize_y: int = 0
     hr_checkpoint_name: str = ""
     hr_sampler_name: str = ""
+    hr_scheduler: str = ""
     hr_prompt: str = ""
     hr_negative_prompt: str = ""
     force_task_id: str = ""
-    sampler_index: str = "0"
     script_name: str = ""
-    script_args: List[Any] = Field(default_factory=list, examples=[[]])
-    send_images: bool = True
-    save_images: bool = False
-    alwayson_scripts: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
+    script_args: List[str] = []
+    alwayson_scripts: Dict[str, Any] = {}
     infotext: str = ""
+    checkpoint: str = "Juggernaut-XI-Prototype.safetensors"
+    vae: str = ""
+    callback_url: str = ""
 
 
 class AutoImg2Img(BaseRequest):
     prompt: str = ""
     negative_prompt: str = ""
     styles: List[str] = Field(default_factory=list, examples=[[]])
     seed: int = -1
     subseed: int = -1
     subseed_strength: float = 0.0
     seed_resize_from_h: int = -1
     seed_resize_from_w: int = -1
-    sampler_name: str = ""
+    sampler_name: str = "DPM++ 2M"
     scheduler: str = ""
     batch_size: int = 1
     n_iter: int = 1
-    steps: int = 50
-    cfg_scale: float = 7.0
-    width: int = 512
-    height: int = 512
-    restore_faces: bool = True
-    tiling: bool = True
-    do_not_save_samples: bool = False
-    do_not_save_grid: bool = False
+    steps: int = 30
+    cfg_scale: float = 7.5
+    width: int = 1024
+    height: int = 768
+    restore_faces: bool = False
+    tiling: bool = False
+    do_not_save_samples: bool = True
+    do_not_save_grid: bool = True
     eta: float = 0.0
     denoising_strength: float = 0.75
     s_min_uncond: float = 0.0
     s_churn: float = 0.0
     s_tmax: float = 0.0
     s_tmin: float = 0.0
     s_noise: float = 0.0
@@ -107,77 +109,15 @@
     inpainting_fill: int = 0
     inpaint_full_res: bool = True
     inpaint_full_res_padding: int = 0
     inpainting_mask_invert: int = 0
     initial_noise_multiplier: float = 0.0
     latent_mask: str = ""
     force_task_id: str = ""
-    sampler_index: str = "Euler"
     include_init_images: bool = False
     script_name: str = ""
     script_args: List[Any] = Field(default_factory=list, examples=[[]])
-    send_images: bool = True
-    save_images: bool = False
     alwayson_scripts: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
     infotext: str = ""
-
-
-class AutoSchedTxt2Img(BaseRequest):
-    prompt: str = Field("", examples=["A beautiful sunset over a mountain lake."])
-    negative_prompt: str = ""
-    styles: List[str] = Field(default_factory=list, examples=[[]])
-    seed: int = -1
-    subseed: int = -1
-    subseed_strength: int = 0
-    seed_resize_from_h: int = -1
-    seed_resize_from_w: int = -1
-    sampler_name: str = "DPM++ 2M"
-    scheduler: str = ""
-    batch_size: int = 1
-    n_iter: int = 1
-    steps: int = 50
-    cfg_scale: int = 7
-    width: int = 1024
-    height: int = 768
-    restore_faces: bool = True
-    tiling: bool = True
-    do_not_save_samples: bool = False
-    do_not_save_grid: bool = False
-    eta: int = 0
-    denoising_strength: int = 0
-    s_min_uncond: int = 0
-    s_churn: int = 0
-    s_tmax: int = 0
-    s_tmin: int = 0
-    s_noise: int = 0
-    override_settings: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
-    override_settings_restore_afterwards: bool = True
-    refiner_checkpoint: str = ""
-    refiner_switch_at: int = 0
-    disable_extra_networks: bool = False
-    firstpass_image: str = ""
-    comments: Dict[str, Any] = {}
-    enable_hr: bool = False
-    firstphase_width: int = 0
-    firstphase_height: int = 0
-    hr_scale: int = 2
-    hr_upscaler: str = ""
-    hr_second_pass_steps: int = 0
-    hr_resize_x: int = 0
-    hr_resize_y: int = 0
-    hr_checkpoint_name: str = ""
-    hr_sampler_name: str = ""
-    hr_scheduler: str = ""
-    hr_prompt: str = ""
-    hr_negative_prompt: str = ""
-    force_task_id: str = ""
-    script_name: str = ""
-    script_args: List[str] = []
-    alwayson_scripts: Dict[str, Any] = {}
-    infotext: str = ""
-    checkpoint: str = "sdxl/juggernautXL_v9Rundiffusionphoto2.safetensors"
+    checkpoint: str = "Juggernaut-XI-Prototype.safetensors"
     vae: str = ""
     callback_url: str = ""
-
-
-class AutoModelLoad(BaseRequest):
-    sd_model_checkpoint: str = Field("", examples=["sdxl/juggernautXL_v9Rundiffusionphoto2.safetensors"])
```

### Comparing `gen_wrappers-0.3.5/creator/auto/response_auto.py` & `gen_wrappers-0.3.6/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.5/creator/base/base_app.py` & `gen_wrappers-0.3.6/creator/base/base_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,13 +39,9 @@
         return base_response
 
     @abstractmethod
     def upload_image(self, image_data: Any) -> str:
         pass
 
     @abstractmethod
-    async def select_model(self, params: BaseRequest):
-        pass
-
-    @abstractmethod
     async def test(self):
         pass
```

### Comparing `gen_wrappers-0.3.5/creator/base/base_request.py` & `gen_wrappers-0.3.6/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.5/creator/base/base_response.py` & `gen_wrappers-0.3.6/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.5/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.3.6/creator/cmfy/creator_cmfy.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,17 +154,14 @@
                         if model_name:
                             models.append(model_name)
         return models
 
     async def upload_image(self, image_data: Any) -> str:
         pass
 
-    async def select_model(self, params: BaseRequest):
-        pass
-
     async def test(self):
         url = f"http://localhost:{os.environ.get('PORT_CMFY', 8889)}/history"
         async with httpx.AsyncClient() as client:
             response = await client.get(url)
             if response.status_code == 200:
                 return BaseResponse.active()
             else:
```

### Comparing `gen_wrappers-0.3.5/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.3.6/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.5/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.3.6/creator/auto/creator_auto.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,140 +1,126 @@
 import asyncio
-import json
 import logging
 import os
-from typing import Any, Union, List
+import traceback
+from typing import Any, List, Union
 
 import httpx
-import requests
 
+from creator.auto.request_auto import AutoTxt2Img, AutoImg2Img
+from creator.auto.response_auto import ResponseAuto
 from creator.base.base_app import BaseApp
-from creator.base.base_request import BaseRequest
-from creator.base.base_response import BaseResponse, ResponseDataType, ResponseData
-from creator.fcus_api.request_fcus_api import FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint
-from creator.fcus_api.response_fcus_api import ResponseFcusApi
+from creator.base.base_response import BaseResponse, ResponseData, ResponseDataType
+from creator.base.job_status import JobStatus
 
 logger = logging.getLogger(__name__)
 
 
-class AppFcusApi(BaseApp):
-    param_classes = [FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint]
+class AppAuto(BaseApp):
+    param_classes = [AutoTxt2Img, AutoImg2Img]
     output = {}
+    jobs = {}
+    sched_jobs = {}
 
     def __init__(self):
         super().__init__()
-        focus_port = os.environ.get("PORT_FCUS_API", 8888)
-        if isinstance(focus_port, str):
-            focus_port = int(focus_port)
-        self.api_base_url = f"http://0.0.0.0:{focus_port}"
-
-    async def select_model(self, params: BaseRequest):
-        pass
-
-    async def create(self, params: Union[FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint]) -> BaseResponse:
-        if isinstance(params, FcusTxt2Img):
-            url = f"{self.api_base_url}/v1/generation/text-to-image"
-        elif isinstance(params, FcusUpscaleOrVary):
-            url = f"{self.api_base_url}/v1/generation/image-upscale-vary"
-        elif isinstance(params, FcusInpaintOrOutpaint):
-            url = f"{self.api_base_url}/v1/generation/image-inpaint-outpaint"
-        else:
-            raise ValueError("Invalid parameters for creation")
-
-        data = json.dumps(params.__dict__)
+        auto_port = os.environ.get("PORT_AUTO", 8081)
+        if isinstance(auto_port, str):
+            auto_port = int(auto_port)
+        self.jobs = {}
+        self.output = {}
+        self.api_base_url = f"http://0.0.0.0:{auto_port}/sdapi"
+
+    async def create(self, params: Union[AutoTxt2Img, AutoImg2Img], job_id=None) -> BaseResponse:
+        print(f"Creating job with params: {params}")
+        endpoint_name = "txt2img" if isinstance(params, AutoTxt2Img) else "img2img"
+        url = f"{self.api_base_url}/agent-scheduler/v1/{endpoint_name}"
+        data = params.model_dump()
         headers = {'Content-Type': 'application/json'}
-        response = requests.post(url, data=data, headers=headers)
-        # If we have a 422 here, print what the unprocessable entity is
-        if response.status_code == 422:
-            logger.warning(f"Unprocessable entity: {response.text}")
-        response.raise_for_status()
-
-        self.output = response.json()
-        logger.debug(f"Response: {self.output}")
-        job_id = self.output.get('job_id', None)
-        output = None
-        if job_id is not None:
-            job_count = 0
-            while output is None and job_count < 60:
-                logger.debug(f"Job count: {job_count}")
-                output = await self._get_output(job_id)
-                job_count += 1
-                if output is None:
-                    await asyncio.sleep(1)
-            response_data = ResponseData(data=output, data_type=ResponseDataType.IMAGE, total_count=len(output))
-            return ResponseFcusApi(status="Job Finished", output=response_data, job_id=job_id)
-
-    async def create_async(self, params: Union[FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint]) -> BaseResponse:
-        if isinstance(params, FcusTxt2Img):
-            model = params.base_model_name
-            url = f"{self.api_base_url}/v1/generation/text-to-image"
-        elif isinstance(params, FcusUpscaleOrVary):
-            model = params.base_model_name
-            url = f"{self.api_base_url}/v1/generation/image-upscale-vary"
-        elif isinstance(params, FcusInpaintOrOutpaint):
-            model = params.base_model_name
-            url = f"{self.api_base_url}/v1/generation/image-inpaint-outpaint"
-        else:
-            raise ValueError("Invalid parameters for creation")
-        if model is not None and model not in self.loaded_models:
-            self.loaded_models.append(model)
-        max_cached_models = os.environ.get("MAX_CACHED_MODELS", 3)
-        if len(self.loaded_models) > max_cached_models:
-            self.loaded_models = self.loaded_models[-max_cached_models:]
-
-        data = json.dumps(params.model_dump())
+        async with httpx.AsyncClient() as client:
+            response = await client.post(url, data=data, headers=headers)
+            response.raise_for_status()
+        output = response.json()
+        task_id = output.get("task_id", None)
+        print(f"Response received: {output}")
+        if task_id:
+            self.jobs[task_id] = endpoint_name
+            result = await self.get_status(task_id)
+            while result.status == JobStatus.RUNNING:
+                await asyncio.sleep(5)
+            return result
+
+    async def create_async(self, params: Union[AutoTxt2Img, AutoImg2Img]) -> BaseResponse:
+        endpoint_name = "txt2img" if isinstance(params, AutoTxt2Img) else "img2img"
+        url = f"{self.api_base_url}/agent-scheduler/v1/queue/{endpoint_name}"
+        data = params.model_dump()
         headers = {'Content-Type': 'application/json'}
-        response = requests.post(url, data=data, headers=headers)
-        # If we have a 422 here, print what the unprocessable entity is
-        if response.status_code == 422:
-            logger.warning(f"Unprocessable entity: {response.text}")
-        response.raise_for_status()
-
-        self.output = response.json()
-        logger.debug(f"Response: {self.output}")
-        job_id = self.output.get('job_id', None)
-        if job_id is not None:
-            return ResponseFcusApi.running(job_id)
-        return ResponseFcusApi.error("Job ID not found", job_id)
+        try:
+            async with httpx.AsyncClient() as client:
+                response = await client.post(url, data=data, headers=headers)
+                response.raise_for_status()
+            output = response.json()
+            task_id = output.get("task_id", None)
+            if task_id:
+                return ResponseAuto.running(task_id)
+        except Exception as e:
+            logger.error(f"Error creating job: {e}")
+            traceback.print_exc()
+            return ResponseAuto.error(f"Error creating job: {e}")
 
     async def get_status(self, job_id: str) -> BaseResponse:
-        output = await self._get_output(job_id)
-        if output is None:
-            return BaseResponse.error("Error getting job status")
-        if not output:
-            print(f"Job {job_id} is still running (or can't get output)")
-            return BaseResponse.running(job_id)
-        return BaseResponse.success(
-            ResponseData(data=output, data_type=ResponseDataType.IMAGE, total_count=len(output)))
-
-    async def upload_image(self, image_data: Any) -> str:
-        pass
+        try:
+            url = f"{self.api_base_url}/agent-scheduler/v1/task/{job_id}/results"
+            async with httpx.AsyncClient() as client:
+                response = await client.get(url)
+                response.raise_for_status()
+            output = response.json()
+
+            job_success = output.get("success", False)
+            if not job_success:
+                message = output.get("message", "Unknown status")
+                if message == "Task is pending":
+                    return ResponseAuto.running(job_id)
+                else:
+                    return ResponseAuto.error(f"Error getting job status: {message}", job_id)
+            else:
+                images = []
+                data = output.get("data", [])
+                if data and isinstance(data, list):
+                    for output in data:
+                        image = output.get("image", None)
+                        if image:
+                            # Remove the data:image/png;base64, prefix
+                            image = image.split(",")[-1]
+                            images.append(image)
+                response_data = ResponseData(data=images, data_type=ResponseDataType.IMAGE, total_count=len(images))
+                return ResponseAuto.success(response_data, job_id)
+
+        except Exception as e:
+            logger.error(f"Error getting job status for job ID {job_id}: {e}")
+            traceback.print_exc()
+            return ResponseAuto.error(f"Error getting job status: {e}", job_id)
 
-    async def get_models(self) -> List[str]:
+    async def get_models(self) -> List[Any]:
+        url = f"{self.api_base_url}/sdapi/v1/sd-models"
         async with httpx.AsyncClient() as client:
-            response = await client.get(f"{self.api_base_url}/v1/engines/all-models")
+            response = await client.get(url)
             response.raise_for_status()
             response_json = response.json()
-            return response_json.get("model_filenames", [])
+        models = [model.get("title") for model in response_json if model.get("title")]
+        return models
+
+    # Assuming you will provide more detail or use this method later
+    async def upload_image(self, image_data: Any) -> str:
+        pass
 
     async def test(self):
+        auto_port = int(os.environ.get("PORT_AUTO", 8081))
+        url = f"http://0.0.0.0:{auto_port}/docs"
         async with httpx.AsyncClient() as client:
-            url = f"{self.api_base_url}/docs"
             response = await client.get(url)
             if response.status_code == 200:
                 return BaseResponse.active()
             else:
                 return BaseResponse.error("Error testing connection")
 
-    async def _get_output(self, job_id: str) -> Union[None, List[str]]:
-        async with httpx.AsyncClient() as client:
-            response = await client.get(f"{self.api_base_url}/v1/generation/query-job", params={'job_id': job_id})
-            response.raise_for_status()
-            response_json = response.json()
-            status = response_json.get('job_status')
-            logger.debug(f"Status: {status}")
-            if status is None:
-                return None
-            if status != "Finished":
-                return []
-            outputs = [result.get('base64') for result in response_json.get('job_result', []) if result.get('finish_reason', "UNKNOWN") == "SUCCESS"]
-            return outputs
+
```

### Comparing `gen_wrappers-0.3.5/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.3.6/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.5/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.3.6/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.5/creator/util/helper.py` & `gen_wrappers-0.3.6/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.5/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.3.6/gen_wrappers.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.3.5
+Version: 0.3.6
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.5/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.3.6/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.5/setup.py` & `gen_wrappers-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.3.5',
+    version='0.3.6',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

