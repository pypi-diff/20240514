# Comparing `tmp/pinjected_openai-0.4.6.tar.gz` & `tmp/pinjected_openai-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected_openai-0.4.6.tar", max compression
+gzip compressed data, was "pinjected_openai-0.4.7.tar", max compression
```

## Comparing `pinjected_openai-0.4.6.tar` & `pinjected_openai-0.4.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-01-25 04:47:59.248948 pinjected_openai-0.4.6/README.md
--rw-r--r--   0        0        0      380 2024-04-12 06:08:48.671473 pinjected_openai-0.4.6/pinjected_openai/__init__.py
--rw-r--r--   0        0        0      631 2024-04-15 03:17:41.134925 pinjected_openai-0.4.6/pinjected_openai/clients.py
--rw-r--r--   0        0        0     6794 2024-04-12 06:08:48.682761 pinjected_openai-0.4.6/pinjected_openai/vision_llm.py
--rw-r--r--   0        0        0     1358 2024-04-12 06:13:50.042530 pinjected_openai-0.4.6/pinjected_openai/whisper.py
--rw-r--r--   0        0        0      453 2024-04-15 03:18:52.861961 pinjected_openai-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pinjected_openai-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-25 04:47:59.248948 pinjected_openai-0.4.7/README.md
+-rw-r--r--   0        0        0      380 2024-04-12 06:08:48.671473 pinjected_openai-0.4.7/pinjected_openai/__init__.py
+-rw-r--r--   0        0        0      631 2024-04-15 03:17:41.134925 pinjected_openai-0.4.7/pinjected_openai/clients.py
+-rw-r--r--   0        0        0     6794 2024-04-16 09:31:59.739199 pinjected_openai-0.4.7/pinjected_openai/vision_llm.py
+-rw-r--r--   0        0        0     1358 2024-04-12 06:13:50.042530 pinjected_openai-0.4.7/pinjected_openai/whisper.py
+-rw-r--r--   0        0        0      453 2024-05-14 13:11:47.655415 pinjected_openai-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 pinjected_openai-0.4.7/PKG-INFO
```

### Comparing `pinjected_openai-0.4.6/pinjected_openai/clients.py` & `pinjected_openai-0.4.7/pinjected_openai/clients.py`

 * *Files identical despite different names*

### Comparing `pinjected_openai-0.4.6/pinjected_openai/vision_llm.py` & `pinjected_openai-0.4.7/pinjected_openai/vision_llm.py`

 * *Files identical despite different names*

### Comparing `pinjected_openai-0.4.6/pinjected_openai/whisper.py` & `pinjected_openai-0.4.7/pinjected_openai/whisper.py`

 * *Files identical despite different names*

### Comparing `pinjected_openai-0.4.6/PKG-INFO` & `pinjected_openai-0.4.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pinjected-openai
-Version: 0.4.6
+Version: 0.4.7
 Summary: 
 Author: proboscis
 Author-email: nameissoap@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: injected-utils (>=0.1.5,<0.2.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: openai (>=1.9.0,<2.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: pinjected
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
```

