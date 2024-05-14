# Comparing `tmp/mulankit-1.0.0.tar.gz` & `tmp/mulankit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mulankit-1.0.0.tar", last modified: Tue May 14 05:27:10 2024, max compression
+gzip compressed data, was "mulankit-1.0.1.tar", last modified: Tue May 14 05:41:46 2024, max compression
```

## Comparing `mulankit-1.0.0.tar` & `mulankit-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:27:10.000000 mulankit-1.0.0/
--rw-r--r--   0 huangzhenhang (100000384) huangzhenhang (100000384)      248 2024-05-14 05:27:10.000000 mulankit-1.0.0/PKG-INFO
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     3565 2024-05-14 05:12:32.000000 mulankit-1.0.0/README.md
-drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:27:09.000000 mulankit-1.0.0/mulankit/
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)       51 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/__init__.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     4863 2024-05-14 05:12:57.000000 mulankit-1.0.0/mulankit/api.py
-drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:27:09.000000 mulankit-1.0.0/mulankit/app/
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 04:25:40.000000 mulankit-1.0.0/mulankit/app/__init__.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     2430 2024-05-14 04:55:34.000000 mulankit-1.0.0/mulankit/app/meta.json
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    13555 2024-05-14 05:05:58.000000 mulankit-1.0.0/mulankit/app/samples.txt
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)       50 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/app/style.css
-drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:27:09.000000 mulankit-1.0.0/mulankit/app/viscpm/
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 04:25:50.000000 mulankit-1.0.0/mulankit/app/viscpm/__init__.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     6074 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/app/viscpm/configuration_cpmbee.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    40684 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/app/viscpm/modeling_cpmbee.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    32675 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/app/viscpm/pipeline_viscpm_paint.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    40229 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/app/viscpm/tokenization_viscpmbee.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    26949 2024-05-14 05:21:14.000000 mulankit-1.0.0/mulankit/app/webui.py
-drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:27:10.000000 mulankit-1.0.0/mulankit/internvl/
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     3596 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/internvl/__init__.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     5478 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/internvl/configuration_intern_vit.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     4802 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/internvl/configuration_internvl.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     3459 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/internvl/flash_attention.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     3277 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/internvl/modeling_intern_text.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     1673 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/internvl/modeling_intern_vision.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    13993 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/internvl/modeling_intern_vit.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    21083 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/internvl/modeling_internvl.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    48012 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/internvl/modeling_qllama.py
-drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:27:10.000000 mulankit-1.0.0/mulankit/models/
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 04:25:35.000000 mulankit-1.0.0/mulankit/models/__init__.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     4988 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/models/adapter.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     1132 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/models/unet.py
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    24266 2024-05-12 07:23:03.000000 mulankit-1.0.0/mulankit/patch.py
-drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:27:09.000000 mulankit-1.0.0/mulankit.egg-info/
--rw-r--r--   0 huangzhenhang (100000384) huangzhenhang (100000384)      248 2024-05-14 05:27:09.000000 mulankit-1.0.0/mulankit.egg-info/PKG-INFO
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)      995 2024-05-14 05:27:09.000000 mulankit-1.0.0/mulankit.egg-info/SOURCES.txt
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)        1 2024-05-14 05:27:09.000000 mulankit-1.0.0/mulankit.egg-info/dependency_links.txt
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)        5 2024-05-14 05:27:09.000000 mulankit-1.0.0/mulankit.egg-info/requires.txt
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)        9 2024-05-14 05:27:09.000000 mulankit-1.0.0/mulankit.egg-info/top_level.txt
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)       38 2024-05-14 05:27:10.000000 mulankit-1.0.0/setup.cfg
--rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)      554 2024-05-14 05:23:15.000000 mulankit-1.0.0/setup.py
+drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:41:46.000000 mulankit-1.0.1/
+-rw-r--r--   0 huangzhenhang (100000384) huangzhenhang (100000384)      395 2024-05-14 05:41:46.000000 mulankit-1.0.1/PKG-INFO
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     3565 2024-05-14 05:12:32.000000 mulankit-1.0.1/README.md
+drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:41:45.000000 mulankit-1.0.1/mulankit/
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)       51 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/__init__.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     4863 2024-05-14 05:12:57.000000 mulankit-1.0.1/mulankit/api.py
+drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:41:46.000000 mulankit-1.0.1/mulankit/app/
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 04:25:40.000000 mulankit-1.0.1/mulankit/app/__init__.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     2430 2024-05-14 04:55:34.000000 mulankit-1.0.1/mulankit/app/meta.json
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    13555 2024-05-14 05:05:58.000000 mulankit-1.0.1/mulankit/app/samples.txt
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)       50 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/app/style.css
+drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:41:46.000000 mulankit-1.0.1/mulankit/app/viscpm/
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 04:25:50.000000 mulankit-1.0.1/mulankit/app/viscpm/__init__.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     6074 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/app/viscpm/configuration_cpmbee.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    40684 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/app/viscpm/modeling_cpmbee.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    32675 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/app/viscpm/pipeline_viscpm_paint.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    40229 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/app/viscpm/tokenization_viscpmbee.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    26779 2024-05-14 05:40:02.000000 mulankit-1.0.1/mulankit/app/webui.py
+drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:41:46.000000 mulankit-1.0.1/mulankit/internvl/
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     3596 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/internvl/__init__.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     5478 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/internvl/configuration_intern_vit.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     4802 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/internvl/configuration_internvl.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     3459 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/internvl/flash_attention.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     3277 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/internvl/modeling_intern_text.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     1673 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/internvl/modeling_intern_vision.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    13993 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/internvl/modeling_intern_vit.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    21083 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/internvl/modeling_internvl.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    48012 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/internvl/modeling_qllama.py
+drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:41:46.000000 mulankit-1.0.1/mulankit/models/
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 04:25:35.000000 mulankit-1.0.1/mulankit/models/__init__.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     4988 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/models/adapter.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)     1132 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/models/unet.py
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)    24266 2024-05-12 07:23:03.000000 mulankit-1.0.1/mulankit/patch.py
+drwxrwxr-x   0 huangzhenhang (100000384) huangzhenhang (100000384)        0 2024-05-14 05:41:46.000000 mulankit-1.0.1/mulankit.egg-info/
+-rw-r--r--   0 huangzhenhang (100000384) huangzhenhang (100000384)      395 2024-05-14 05:41:45.000000 mulankit-1.0.1/mulankit.egg-info/PKG-INFO
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)      995 2024-05-14 05:41:45.000000 mulankit-1.0.1/mulankit.egg-info/SOURCES.txt
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)        1 2024-05-14 05:41:45.000000 mulankit-1.0.1/mulankit.egg-info/dependency_links.txt
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)       62 2024-05-14 05:41:45.000000 mulankit-1.0.1/mulankit.egg-info/requires.txt
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)        9 2024-05-14 05:41:45.000000 mulankit-1.0.1/mulankit.egg-info/top_level.txt
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)       38 2024-05-14 05:41:46.000000 mulankit-1.0.1/setup.cfg
+-rw-rw-r--   0 huangzhenhang (100000384) huangzhenhang (100000384)      658 2024-05-14 05:40:49.000000 mulankit-1.0.1/setup.py
```

### Comparing `mulankit-1.0.0/README.md` & `mulankit-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/api.py` & `mulankit-1.0.1/mulankit/api.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/app/meta.json` & `mulankit-1.0.1/mulankit/app/meta.json`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/app/samples.txt` & `mulankit-1.0.1/mulankit/app/samples.txt`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/app/viscpm/configuration_cpmbee.py` & `mulankit-1.0.1/mulankit/app/viscpm/configuration_cpmbee.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/app/viscpm/modeling_cpmbee.py` & `mulankit-1.0.1/mulankit/app/viscpm/modeling_cpmbee.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/app/viscpm/pipeline_viscpm_paint.py` & `mulankit-1.0.1/mulankit/app/viscpm/pipeline_viscpm_paint.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/app/viscpm/tokenization_viscpmbee.py` & `mulankit-1.0.1/mulankit/app/viscpm/tokenization_viscpmbee.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/app/webui.py` & `mulankit-1.0.1/mulankit/app/webui.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,20 +344,14 @@
     share=False,
 ):
     print('launching demo', flush=True)
 
     DESCRIPTION = """
     # 🌻 MuLan: Adapting Multilingual Diffusion Models for 110 + Languages
     [[Technical Report (coming soon)]](#) [[Code]](https://github.com/mulanai/MuLan) [[Model]](https://huggingface.co/mulanai)
-    
-    Note:
-    - dreamshaperXL-lightning should use SDXL-Lightning Scheduler
-    - LCM should use LCM Scheduler
-    - SD-Turbo is trained on 512x512 resolution.
-    
     """
     if not torch.cuda.is_available():
         DESCRIPTION += "\n<p>Running on CPU 🥶 This demo does not work on CPU.</p>"
 
     COPY_RIGHT = """
     <div align="center">
     Feel free to steal this gradio's source code. Templated by [MuLan]().
```

### Comparing `mulankit-1.0.0/mulankit/internvl/__init__.py` & `mulankit-1.0.1/mulankit/internvl/__init__.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/internvl/configuration_intern_vit.py` & `mulankit-1.0.1/mulankit/internvl/configuration_intern_vit.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/internvl/configuration_internvl.py` & `mulankit-1.0.1/mulankit/internvl/configuration_internvl.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/internvl/flash_attention.py` & `mulankit-1.0.1/mulankit/internvl/flash_attention.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/internvl/modeling_intern_text.py` & `mulankit-1.0.1/mulankit/internvl/modeling_intern_text.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/internvl/modeling_intern_vision.py` & `mulankit-1.0.1/mulankit/internvl/modeling_intern_vision.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/internvl/modeling_intern_vit.py` & `mulankit-1.0.1/mulankit/internvl/modeling_intern_vit.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/internvl/modeling_internvl.py` & `mulankit-1.0.1/mulankit/internvl/modeling_internvl.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/internvl/modeling_qllama.py` & `mulankit-1.0.1/mulankit/internvl/modeling_qllama.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/models/adapter.py` & `mulankit-1.0.1/mulankit/models/adapter.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/models/unet.py` & `mulankit-1.0.1/mulankit/models/unet.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit/patch.py` & `mulankit-1.0.1/mulankit/patch.py`

 * *Files identical despite different names*

### Comparing `mulankit-1.0.0/mulankit.egg-info/SOURCES.txt` & `mulankit-1.0.1/mulankit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

