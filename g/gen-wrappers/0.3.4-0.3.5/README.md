# Comparing `tmp/gen_wrappers-0.3.4.tar.gz` & `tmp/gen_wrappers-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.3.4.tar", last modified: Tue May 14 13:55:14 2024, max compression
+gzip compressed data, was "gen_wrappers-0.3.5.tar", last modified: Tue May 14 14:50:06 2024, max compression
```

## Comparing `gen_wrappers-0.3.4.tar` & `gen_wrappers-0.3.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.537770 gen_wrappers-0.3.4/
--rw-rw-rw-   0        0        0      847 2024-05-14 13:55:14.536771 gen_wrappers-0.3.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.496246 gen_wrappers-0.3.4/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.4/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.501279 gen_wrappers-0.3.4/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.4/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     6625 2024-05-11 17:01:23.000000 gen_wrappers-0.3.4/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.3.4/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.4/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.505252 gen_wrappers-0.3.4/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.4/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.3.4/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.4/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.4/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.4/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.509252 gen_wrappers-0.3.4/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.4/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9561 2024-05-11 17:02:29.000000 gen_wrappers-0.3.4/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     9193 2024-05-11 14:41:07.000000 gen_wrappers-0.3.4/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.4/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.513770 gen_wrappers-0.3.4/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.4/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6345 2024-05-11 17:04:12.000000 gen_wrappers-0.3.4/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.4/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.4/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.515772 gen_wrappers-0.3.4/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.4/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.3.4/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.534770 gen_wrappers-0.3.4/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-14 13:55:14.000000 gen_wrappers-0.3.4/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-14 13:55:14.000000 gen_wrappers-0.3.4/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 13:55:14.000000 gen_wrappers-0.3.4/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-14 13:55:14.000000 gen_wrappers-0.3.4/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 13:55:14.000000 gen_wrappers-0.3.4/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 13:55:14.537770 gen_wrappers-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-14 13:55:01.000000 gen_wrappers-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.075251 gen_wrappers-0.3.5/
+-rw-rw-rw-   0        0        0      847 2024-05-14 14:50:06.073248 gen_wrappers-0.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.030549 gen_wrappers-0.3.5/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.5/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.044510 gen_wrappers-0.3.5/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.5/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     6625 2024-05-11 17:01:23.000000 gen_wrappers-0.3.5/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.3.5/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.5/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.049759 gen_wrappers-0.3.5/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.5/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.3.5/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.5/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.5/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.5/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.053764 gen_wrappers-0.3.5/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.5/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9561 2024-05-11 17:02:29.000000 gen_wrappers-0.3.5/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    10277 2024-05-14 14:43:03.000000 gen_wrappers-0.3.5/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.5/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.058765 gen_wrappers-0.3.5/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.5/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6345 2024-05-11 17:04:12.000000 gen_wrappers-0.3.5/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.5/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.5/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.059765 gen_wrappers-0.3.5/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.5/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.3.5/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:50:06.072250 gen_wrappers-0.3.5/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-14 14:50:05.000000 gen_wrappers-0.3.5/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-14 14:50:05.000000 gen_wrappers-0.3.5/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 14:50:05.000000 gen_wrappers-0.3.5/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-14 14:50:05.000000 gen_wrappers-0.3.5/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 14:50:05.000000 gen_wrappers-0.3.5/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 14:50:06.075251 gen_wrappers-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-14 14:47:27.000000 gen_wrappers-0.3.5/setup.py
```

### Comparing `gen_wrappers-0.3.4/PKG-INFO` & `gen_wrappers-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.3.4
+Version: 0.3.5
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.4/creator/auto/creator_auto.py` & `gen_wrappers-0.3.5/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.4/creator/auto/request_auto.py` & `gen_wrappers-0.3.5/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.4/creator/auto/response_auto.py` & `gen_wrappers-0.3.5/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.4/creator/base/base_app.py` & `gen_wrappers-0.3.5/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.4/creator/base/base_request.py` & `gen_wrappers-0.3.5/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.4/creator/base/base_response.py` & `gen_wrappers-0.3.5/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.4/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.3.5/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.4/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.3.5/creator/cmfy/request_cmfy.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,19 +33,21 @@
         "class_type": "KSampler",
         "_meta": {
             "title": "KSampler"
         }
     },
     "4": {
         "inputs": {
-            "ckpt_name": "Juggernaut-XI-Prototype.safetensors"
+            "ckpt_name": "Juggernaut-XI-Prototype.safetensors",
+            "key_opt": "",
+            "mode": "Auto"
         },
-        "class_type": "CheckpointLoaderSimple",
+        "class_type": "CheckpointLoaderSimpleShared //Inspire",
         "_meta": {
-            "title": "Load Checkpoint"
+            "title": "Shared Checkpoint Loader (Inspire)"
         }
     },
     "5": {
         "inputs": {
             "width": 1024,
             "height": 768,
             "batch_size": 1
@@ -109,42 +111,33 @@
         "_meta": {
             "title": "Save Image"
         }
     }
 }
 
 default_workflow_json_2 = {
-  "4": {
-    "inputs": {
-      "ckpt_name": "Juggernaut-XI-Prototype.safetensors"
-    },
-    "class_type": "CheckpointLoaderSimple",
-    "_meta": {
-      "title": "Load Checkpoint"
-    }
-  },
   "21": {
     "inputs": {
-      "width": 2432,
-      "height": 1664,
+      "width": 1344,
+      "height": 768,
       "batch_size": 2
     },
     "class_type": "EmptyLatentImage",
     "_meta": {
       "title": "Image Size\n"
     }
   },
   "67": {
     "inputs": {
       "samples": [
         "132",
         0
       ],
       "vae": [
-        "4",
+        "135",
         2
       ]
     },
     "class_type": "VAEDecode",
     "_meta": {
       "title": "VAE Decode"
     }
@@ -159,51 +152,51 @@
     "class_type": "PreviewImage",
     "_meta": {
       "title": "Output"
     }
   },
   "99": {
     "inputs": {
-      "seed": 1042340763738557
+      "seed": 178120892921818
     },
     "class_type": "CR Seed",
     "_meta": {
       "title": "🌱 CR Seed"
     }
   },
   "100": {
     "inputs": {
       "text": [
         "114:0",
         0
       ],
-      "seed": 1116260329,
+      "seed": 1892035549,
       "log_prompt": "No"
     },
     "class_type": "PromptExpansion",
     "_meta": {
       "title": "Prompt Expansion"
     }
   },
   "101": {
     "inputs": {
       "text": [
-        "100",
+        "144",
         0
       ]
     },
     "class_type": "ShowText|pysssss",
     "_meta": {
       "title": "Final Positive Prompt"
     }
   },
   "102": {
     "inputs": {
       "text": [
-        "114:1",
+        "145",
         0
       ]
     },
     "class_type": "ShowText|pysssss",
     "_meta": {
       "title": "Final Negative Prompt"
     }
@@ -211,15 +204,15 @@
   "120": {
     "inputs": {
       "b1": 1.01,
       "b2": 1.02,
       "s1": 0.99,
       "s2": 0.9500000000000001,
       "model": [
-        "4",
+        "135",
         0
       ]
     },
     "class_type": "FreeU_V2",
     "_meta": {
       "title": "FreeU_V2"
     }
@@ -243,19 +236,19 @@
       "variation_seed": 0,
       "variation_strength": 0,
       "model": [
         "134",
         0
       ],
       "positive": [
-        "98:0",
+        "138:1",
         0
       ],
       "negative": [
-        "98:1",
+        "138:0",
         0
       ],
       "latent_image": [
         "21",
         0
       ]
     },
@@ -278,14 +271,75 @@
       ]
     },
     "class_type": "Hires",
     "_meta": {
       "title": "Apply Kohya's HiresFix"
     }
   },
+  "135": {
+    "inputs": {
+      "ckpt_name": "Juggernaut-XI-Prototype.safetensors",
+      "key_opt": "",
+      "mode": "Auto"
+    },
+    "class_type": "CheckpointLoaderSimpleShared //Inspire",
+    "_meta": {
+      "title": "Shared Checkpoint Loader (Inspire)"
+    }
+  },
+  "139": {
+    "inputs": {
+      "prompt": "a cat in a hat"
+    },
+    "class_type": "CR Prompt Text",
+    "_meta": {
+      "title": "Positive Prompt"
+    }
+  },
+  "140": {
+    "inputs": {
+      "prompt": "blurry, bad eyes, bad hands, deformed, low quality"
+    },
+    "class_type": "CR Prompt Text",
+    "_meta": {
+      "title": "Negative Prompt"
+    }
+  },
+  "144": {
+    "inputs": {
+      "action": "replace",
+      "tidy_tags": "yes",
+      "text_a": [
+        "100",
+        0
+      ],
+      "text_b": "",
+      "text_c": ""
+    },
+    "class_type": "StringFunction|pysssss",
+    "_meta": {
+      "title": "Tidy Positive Tags"
+    }
+  },
+  "145": {
+    "inputs": {
+      "action": "replace",
+      "tidy_tags": "yes",
+      "text_a": [
+        "114:1",
+        0
+      ],
+      "text_b": "",
+      "text_c": ""
+    },
+    "class_type": "StringFunction|pysssss",
+    "_meta": {
+      "title": "Tidy Negative Tags"
+    }
+  },
   "119:0": {
     "inputs": {
       "text_positive": "",
       "text_negative": "",
       "style": "Fooocus Photograph",
       "log_prompt": True,
       "style_positive": True,
@@ -296,15 +350,15 @@
       "title": "SDXL Prompt Styler"
     }
   },
   "119:1": {
     "inputs": {
       "text_positive": "",
       "text_negative": "",
-      "style": "Fooocus Enhance",
+      "style": "Fooocus Sharp",
       "log_prompt": True,
       "style_positive": True,
       "style_negative": True
     },
     "class_type": "SDXLPromptStyler",
     "_meta": {
       "title": "SDXL Prompt Styler"
@@ -322,29 +376,35 @@
     "class_type": "SDXLPromptStyler",
     "_meta": {
       "title": "SDXL Prompt Styler"
     }
   },
   "133:0": {
     "inputs": {
-      "text1": "a close-up shot of a soldier running on the battlefield, world war 2, gritty, dust, explosions",
+      "text1": [
+        "139",
+        0
+      ],
       "text2": [
         "119:0",
         0
       ],
       "separator": ", "
     },
     "class_type": "CR Text Concatenate",
     "_meta": {
       "title": "Concat Positive"
     }
   },
   "133:1": {
     "inputs": {
-      "text1": "blurry eyes, zombie eyes, bad face, too many fingers",
+      "text1": [
+        "140",
+        0
+      ],
       "text2": [
         "119:0",
         1
       ],
       "separator": ", "
     },
     "class_type": "CR Text Concatenate",
@@ -416,44 +476,44 @@
       "separator": ", "
     },
     "class_type": "CR Text Concatenate",
     "_meta": {
       "title": "Concat Negative"
     }
   },
-  "98:0": {
+  "138:0": {
     "inputs": {
       "text": [
-        "101",
+        "102",
         0
       ],
       "clip": [
-        "4",
+        "135",
         1
       ]
     },
     "class_type": "CLIPTextEncode",
     "_meta": {
-      "title": "Encode Positive"
+      "title": "Encode Negative"
     }
   },
-  "98:1": {
+  "138:1": {
     "inputs": {
       "text": [
-        "102",
+        "101",
         0
       ],
       "clip": [
-        "4",
+        "135",
         1
       ]
     },
     "class_type": "CLIPTextEncode",
     "_meta": {
-      "title": "Encode Negative"
+      "title": "Encode Positive"
     }
   }
 }
 
 
 class CmfyWorkflow(BaseRequest):
     workflow_json: str = Field("", examples=[json.dumps(default_workflow_json)])
```

### Comparing `gen_wrappers-0.3.4/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.3.5/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.4/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.3.5/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.4/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.3.5/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.4/creator/util/helper.py` & `gen_wrappers-0.3.5/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.4/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.3.5/gen_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.3.4
+Version: 0.3.5
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.4/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.3.5/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.4/setup.py` & `gen_wrappers-0.3.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.3.4',
+    version='0.3.5',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

