# Comparing `tmp/gen_wrappers-0.3.6.tar.gz` & `tmp/gen_wrappers-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.3.6.tar", last modified: Tue May 14 15:44:03 2024, max compression
+gzip compressed data, was "gen_wrappers-0.3.7.tar", last modified: Tue May 14 16:11:56 2024, max compression
```

## Comparing `gen_wrappers-0.3.6.tar` & `gen_wrappers-0.3.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.468173 gen_wrappers-0.3.6/
--rw-rw-rw-   0        0        0      847 2024-05-14 15:44:03.467173 gen_wrappers-0.3.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.361285 gen_wrappers-0.3.6/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.6/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.370824 gen_wrappers-0.3.6/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.6/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     5302 2024-05-14 15:42:23.000000 gen_wrappers-0.3.6/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     3971 2024-05-14 15:19:49.000000 gen_wrappers-0.3.6/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.6/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.391447 gen_wrappers-0.3.6/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.6/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1491 2024-05-14 15:42:23.000000 gen_wrappers-0.3.6/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.6/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.6/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.6/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.410594 gen_wrappers-0.3.6/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.6/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9489 2024-05-14 15:42:23.000000 gen_wrappers-0.3.6/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0    10277 2024-05-14 14:43:03.000000 gen_wrappers-0.3.6/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.6/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.430593 gen_wrappers-0.3.6/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.6/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6273 2024-05-14 15:42:23.000000 gen_wrappers-0.3.6/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.6/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.6/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.439618 gen_wrappers-0.3.6/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.6/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.3.6/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-14 15:44:03.466172 gen_wrappers-0.3.6/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-14 15:44:03.000000 gen_wrappers-0.3.6/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-14 15:44:03.000000 gen_wrappers-0.3.6/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 15:44:03.000000 gen_wrappers-0.3.6/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-14 15:44:03.000000 gen_wrappers-0.3.6/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 15:44:03.000000 gen_wrappers-0.3.6/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 15:44:03.469173 gen_wrappers-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-14 15:43:58.000000 gen_wrappers-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.045489 gen_wrappers-0.3.7/
+-rw-rw-rw-   0        0        0      847 2024-05-14 16:11:56.044481 gen_wrappers-0.3.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.009092 gen_wrappers-0.3.7/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.7/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.014658 gen_wrappers-0.3.7/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.7/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     5302 2024-05-14 15:42:23.000000 gen_wrappers-0.3.7/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.3.7/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.7/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.018658 gen_wrappers-0.3.7/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.7/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1491 2024-05-14 15:42:23.000000 gen_wrappers-0.3.7/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.7/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.7/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.7/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.022743 gen_wrappers-0.3.7/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.7/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9489 2024-05-14 15:42:23.000000 gen_wrappers-0.3.7/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    10277 2024-05-14 14:43:03.000000 gen_wrappers-0.3.7/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.7/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.026751 gen_wrappers-0.3.7/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.7/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6273 2024-05-14 15:42:23.000000 gen_wrappers-0.3.7/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.7/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.7/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.029750 gen_wrappers-0.3.7/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.7/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.3.7/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:11:56.043459 gen_wrappers-0.3.7/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-14 16:11:55.000000 gen_wrappers-0.3.7/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-14 16:11:55.000000 gen_wrappers-0.3.7/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 16:11:55.000000 gen_wrappers-0.3.7/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-14 16:11:55.000000 gen_wrappers-0.3.7/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 16:11:55.000000 gen_wrappers-0.3.7/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 16:11:56.045489 gen_wrappers-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-14 16:11:36.000000 gen_wrappers-0.3.7/setup.py
```

### Comparing `gen_wrappers-0.3.6/PKG-INFO` & `gen_wrappers-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.3.6
+Version: 0.3.7
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.6/creator/auto/creator_auto.py` & `gen_wrappers-0.3.7/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.6/creator/auto/request_auto.py` & `gen_wrappers-0.3.7/creator/auto/request_auto.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,40 +7,40 @@
 
 class AutoTxt2Img(BaseRequest):
     prompt: str = Field("", examples=["A beautiful sunset over a mountain lake."])
     negative_prompt: str = ""
     styles: List[str] = Field(default_factory=list, examples=[[]])
     seed: int = -1
     subseed: int = -1
-    subseed_strength: int = 0
+    subseed_strength: float = 0
     seed_resize_from_h: int = -1
     seed_resize_from_w: int = -1
     sampler_name: str = "DPM++ 2M"
     scheduler: str = ""
     batch_size: int = 1
     n_iter: int = 1
     steps: int = 30
-    cfg_scale: int = 7.5
+    cfg_scale: float = 7.5
     width: int = 1024
     height: int = 768
     restore_faces: bool = False
     tiling: bool = False
     do_not_save_samples: bool = True
     do_not_save_grid: bool = True
-    eta: int = 0
-    denoising_strength: int = 0
-    s_min_uncond: int = 0
-    s_churn: int = 0
-    s_tmax: int = 0
-    s_tmin: int = 0
-    s_noise: int = 0
+    eta: float = 0
+    denoising_strength: float = 0
+    s_min_uncond: float = 0
+    s_churn: float = 0
+    s_tmax: float = 0
+    s_tmin: float = 0
+    s_noise: float = 0
     override_settings: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
     override_settings_restore_afterwards: bool = True
     refiner_checkpoint: str = ""
-    refiner_switch_at: int = 0
+    refiner_switch_at: float = 0
     disable_extra_networks: bool = False
     firstpass_image: str = ""
     comments: Dict[str, Any] = {}
     enable_hr: bool = False
     firstphase_width: int = 0
     firstphase_height: int = 0
     hr_scale: int = 2
@@ -60,15 +60,15 @@
     infotext: str = ""
     checkpoint: str = "Juggernaut-XI-Prototype.safetensors"
     vae: str = ""
     callback_url: str = ""
 
 
 class AutoImg2Img(BaseRequest):
-    prompt: str = ""
+    prompt: str = Field("", examples=["A beautiful sunset over a mountain lake."])
     negative_prompt: str = ""
     styles: List[str] = Field(default_factory=list, examples=[[]])
     seed: int = -1
     subseed: int = -1
     subseed_strength: float = 0.0
     seed_resize_from_h: int = -1
     seed_resize_from_w: int = -1
@@ -90,15 +90,15 @@
     s_churn: float = 0.0
     s_tmax: float = 0.0
     s_tmin: float = 0.0
     s_noise: float = 0.0
     override_settings: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
     override_settings_restore_afterwards: bool = True
     refiner_checkpoint: str = ""
-    refiner_switch_at: int = 0
+    refiner_switch_at: float = 0
     disable_extra_networks: bool = False
     firstpass_image: str = ""
     comments: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
     init_images: List[str] = Field(default_factory=list, examples=[[]])
     resize_mode: int = 0
     image_cfg_scale: float = 0.0
     mask: str = ""
```

### Comparing `gen_wrappers-0.3.6/creator/auto/response_auto.py` & `gen_wrappers-0.3.7/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.6/creator/base/base_app.py` & `gen_wrappers-0.3.7/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.6/creator/base/base_request.py` & `gen_wrappers-0.3.7/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.6/creator/base/base_response.py` & `gen_wrappers-0.3.7/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.6/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.3.7/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.6/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.3.7/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.6/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.3.7/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.6/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.3.7/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.6/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.3.7/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.6/creator/util/helper.py` & `gen_wrappers-0.3.7/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.6/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.3.7/gen_wrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.3.6
+Version: 0.3.7
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.6/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.3.7/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.6/setup.py` & `gen_wrappers-0.3.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.3.6',
+    version='0.3.7',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

