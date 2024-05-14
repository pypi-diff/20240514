# Comparing `tmp/WaveFormer-0.1.1.tar.gz` & `tmp/WaveFormer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaveFormer-0.1.1.tar", last modified: Sun May 12 11:44:20 2024, max compression
+gzip compressed data, was "WaveFormer-0.1.2.tar", last modified: Tue May 14 06:57:02 2024, max compression
```

## Comparing `WaveFormer-0.1.1.tar` & `WaveFormer-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 11:44:20.389449 WaveFormer-0.1.1/
--rw-rw-rw-   0        0        0    15659 2024-05-12 11:44:20.389449 WaveFormer-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    13348 2024-05-12 11:33:27.000000 WaveFormer-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 11:44:20.360934 WaveFormer-0.1.1/WaveFormer.egg-info/
--rw-rw-rw-   0        0        0    15659 2024-05-12 11:44:20.000000 WaveFormer-0.1.1/WaveFormer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1151 2024-05-12 11:44:20.000000 WaveFormer-0.1.1/WaveFormer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 11:44:20.000000 WaveFormer-0.1.1/WaveFormer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      362 2024-05-12 11:44:20.000000 WaveFormer-0.1.1/WaveFormer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       43 2024-05-12 11:44:20.000000 WaveFormer-0.1.1/WaveFormer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-12 11:44:20.363932 WaveFormer-0.1.1/audio_modules/
--rw-rw-rw-   0        0        0        0 2023-03-30 08:05:32.000000 WaveFormer-0.1.1/audio_modules/__init__.py
--rw-rw-rw-   0        0        0    33218 2024-05-12 08:58:22.000000 WaveFormer-0.1.1/audio_modules/air.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:44:20.366933 WaveFormer-0.1.1/audio_modules/core/
--rw-rw-rw-   0        0        0        0 2023-06-07 06:27:05.000000 WaveFormer-0.1.1/audio_modules/core/__init__.py
--rw-rw-rw-   0        0        0     9745 2024-05-12 08:58:45.000000 WaveFormer-0.1.1/audio_modules/core/configs.py
--rw-rw-rw-   0        0        0        0 2023-06-07 06:21:56.000000 WaveFormer-0.1.1/audio_modules/core/forms.py
--rw-rw-rw-   0        0        0    28704 2024-05-05 10:27:34.000000 WaveFormer-0.1.1/audio_modules/core/informers.py
--rw-rw-rw-   0        0        0        0 2023-06-07 06:21:45.000000 WaveFormer-0.1.1/audio_modules/core/reformers.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:44:20.371939 WaveFormer-0.1.1/audio_modules/extraction/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:17:07.000000 WaveFormer-0.1.1/audio_modules/extraction/__init__.py
--rw-rw-rw-   0        0        0    23908 2024-05-05 11:09:15.000000 WaveFormer-0.1.1/audio_modules/extraction/commands.py
--rw-rw-rw-   0        0        0    15143 2024-05-05 11:09:15.000000 WaveFormer-0.1.1/audio_modules/extraction/core.py
--rw-rw-rw-   0        0        0    28479 2024-05-05 11:09:15.000000 WaveFormer-0.1.1/audio_modules/extraction/extract_configs.py
--rw-rw-rw-   0        0        0     2097 2024-05-05 11:09:15.000000 WaveFormer-0.1.1/audio_modules/extraction/xtgraph.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:44:20.374938 WaveFormer-0.1.1/audio_modules/nvision/
--rw-rw-rw-   0        0        0        0 2024-05-05 11:53:17.000000 WaveFormer-0.1.1/audio_modules/nvision/__init__.py
--rw-rw-rw-   0        0        0     5696 2024-05-12 08:59:01.000000 WaveFormer-0.1.1/audio_modules/nvision/configs.py
--rw-rw-rw-   0        0        0     6100 2024-05-05 11:09:15.000000 WaveFormer-0.1.1/audio_modules/nvision/core.py
--rw-rw-rw-   0        0        0     3709 2024-05-05 11:09:15.000000 WaveFormer-0.1.1/audio_modules/nvision/ngraph.py
--rw-rw-rw-   0        0        0   110049 2024-05-05 11:09:15.000000 WaveFormer-0.1.1/audio_modules/nvision/plotly_mappings.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:44:20.382939 WaveFormer-0.1.1/audio_modules/praat/
--rw-rw-rw-   0        0        0        0 2023-06-14 09:13:20.000000 WaveFormer-0.1.1/audio_modules/praat/__init__.py
--rw-rw-rw-   0        0        0     5979 2024-05-12 08:59:21.000000 WaveFormer-0.1.1/audio_modules/praat/configs.py
--rw-rw-rw-   0        0        0     1615 2024-05-12 09:00:03.000000 WaveFormer-0.1.1/audio_modules/praat/core.py
--rw-rw-rw-   0        0        0     1252 2024-05-05 11:09:15.000000 WaveFormer-0.1.1/audio_modules/praat/filters.py
--rw-rw-rw-   0        0        0     9908 2024-05-12 09:00:13.000000 WaveFormer-0.1.1/audio_modules/praat/formant.py
--rw-rw-rw-   0        0        0     1832 2024-05-12 09:00:23.000000 WaveFormer-0.1.1/audio_modules/praat/handlers.py
--rw-rw-rw-   0        0        0     1833 2023-06-14 12:11:37.000000 WaveFormer-0.1.1/audio_modules/praat/processor.py
--rw-rw-rw-   0        0        0     1765 2023-06-14 08:39:57.000000 WaveFormer-0.1.1/audio_modules/praat/spectrogram.py
--rw-rw-rw-   0        0        0     4456 2024-05-05 11:09:15.000000 WaveFormer-0.1.1/audio_modules/types.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:44:20.386451 WaveFormer-0.1.1/rubberband/
--rw-rw-rw-   0        0        0       64 2023-06-02 09:36:21.000000 WaveFormer-0.1.1/rubberband/__init__.py
--rw-rw-rw-   0        0        0     4910 2024-05-05 12:10:35.000000 WaveFormer-0.1.1/rubberband/options.py
--rw-rw-rw-   0        0        0    12814 2023-06-06 13:00:27.000000 WaveFormer-0.1.1/rubberband/rubberbandstretcher.py
--rw-rw-rw-   0        0        0      394 2024-05-12 08:07:29.000000 WaveFormer-0.1.1/rubberband/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:44:20.387450 WaveFormer-0.1.1/rubberband_builds/
--rw-rw-rw-   0        0        0        0 2023-05-06 11:06:20.000000 WaveFormer-0.1.1/rubberband_builds/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-12 11:44:20.389449 WaveFormer-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      804 2024-05-12 11:38:22.000000 WaveFormer-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.252564 WaveFormer-0.1.2/
+-rw-rw-rw-   0        0        0    15659 2024-05-14 06:57:02.251535 WaveFormer-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13348 2024-05-12 11:33:27.000000 WaveFormer-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.228532 WaveFormer-0.1.2/WaveFormer.egg-info/
+-rw-rw-rw-   0        0        0    15659 2024-05-14 06:57:02.000000 WaveFormer-0.1.2/WaveFormer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1151 2024-05-14 06:57:02.000000 WaveFormer-0.1.2/WaveFormer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 06:57:02.000000 WaveFormer-0.1.2/WaveFormer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      362 2024-05-14 06:57:02.000000 WaveFormer-0.1.2/WaveFormer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       43 2024-05-14 06:57:02.000000 WaveFormer-0.1.2/WaveFormer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.230037 WaveFormer-0.1.2/audio_modules/
+-rw-rw-rw-   0        0        0        0 2023-03-30 08:05:32.000000 WaveFormer-0.1.2/audio_modules/__init__.py
+-rw-rw-rw-   0        0        0    33218 2024-05-12 08:58:22.000000 WaveFormer-0.1.2/audio_modules/air.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.234548 WaveFormer-0.1.2/audio_modules/core/
+-rw-rw-rw-   0        0        0        0 2023-06-07 06:27:05.000000 WaveFormer-0.1.2/audio_modules/core/__init__.py
+-rw-rw-rw-   0        0        0     9745 2024-05-12 08:58:45.000000 WaveFormer-0.1.2/audio_modules/core/configs.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 06:21:56.000000 WaveFormer-0.1.2/audio_modules/core/forms.py
+-rw-rw-rw-   0        0        0    28704 2024-05-05 10:27:34.000000 WaveFormer-0.1.2/audio_modules/core/informers.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 06:21:45.000000 WaveFormer-0.1.2/audio_modules/core/reformers.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.237550 WaveFormer-0.1.2/audio_modules/extraction/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:17:07.000000 WaveFormer-0.1.2/audio_modules/extraction/__init__.py
+-rw-rw-rw-   0        0        0    23908 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/extraction/commands.py
+-rw-rw-rw-   0        0        0    15143 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/extraction/core.py
+-rw-rw-rw-   0        0        0    28479 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/extraction/extract_configs.py
+-rw-rw-rw-   0        0        0     2097 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/extraction/xtgraph.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.241484 WaveFormer-0.1.2/audio_modules/nvision/
+-rw-rw-rw-   0        0        0        0 2024-05-05 11:53:17.000000 WaveFormer-0.1.2/audio_modules/nvision/__init__.py
+-rw-rw-rw-   0        0        0     5696 2024-05-12 08:59:01.000000 WaveFormer-0.1.2/audio_modules/nvision/configs.py
+-rw-rw-rw-   0        0        0     6100 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/nvision/core.py
+-rw-rw-rw-   0        0        0     3709 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/nvision/ngraph.py
+-rw-rw-rw-   0        0        0   110049 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/nvision/plotly_mappings.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.247490 WaveFormer-0.1.2/audio_modules/praat/
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:13:20.000000 WaveFormer-0.1.2/audio_modules/praat/__init__.py
+-rw-rw-rw-   0        0        0     5979 2024-05-12 08:59:21.000000 WaveFormer-0.1.2/audio_modules/praat/configs.py
+-rw-rw-rw-   0        0        0     1615 2024-05-12 09:00:03.000000 WaveFormer-0.1.2/audio_modules/praat/core.py
+-rw-rw-rw-   0        0        0     1252 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/praat/filters.py
+-rw-rw-rw-   0        0        0     9908 2024-05-12 09:00:13.000000 WaveFormer-0.1.2/audio_modules/praat/formant.py
+-rw-rw-rw-   0        0        0     1832 2024-05-12 09:00:23.000000 WaveFormer-0.1.2/audio_modules/praat/handlers.py
+-rw-rw-rw-   0        0        0     1833 2023-06-14 12:11:37.000000 WaveFormer-0.1.2/audio_modules/praat/processor.py
+-rw-rw-rw-   0        0        0     1765 2023-06-14 08:39:57.000000 WaveFormer-0.1.2/audio_modules/praat/spectrogram.py
+-rw-rw-rw-   0        0        0     4456 2024-05-05 11:09:15.000000 WaveFormer-0.1.2/audio_modules/types.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.250538 WaveFormer-0.1.2/rubberband/
+-rw-rw-rw-   0        0        0       64 2023-06-02 09:36:21.000000 WaveFormer-0.1.2/rubberband/__init__.py
+-rw-rw-rw-   0        0        0     4910 2024-05-05 12:10:35.000000 WaveFormer-0.1.2/rubberband/options.py
+-rw-rw-rw-   0        0        0    12814 2023-06-06 13:00:27.000000 WaveFormer-0.1.2/rubberband/rubberbandstretcher.py
+-rw-rw-rw-   0        0        0      272 2024-05-14 06:00:37.000000 WaveFormer-0.1.2/rubberband/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:57:02.250538 WaveFormer-0.1.2/rubberband_builds/
+-rw-rw-rw-   0        0        0        0 2023-05-06 11:06:20.000000 WaveFormer-0.1.2/rubberband_builds/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-14 06:57:02.252564 WaveFormer-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      804 2024-05-14 06:53:34.000000 WaveFormer-0.1.2/setup.py
```

### Comparing `WaveFormer-0.1.1/PKG-INFO` & `WaveFormer-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaveFormer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A single unified Advanced Audio Processing toolkit, that provides both High-Level and Low-Level approaches to its extensive collection of tools.
 Home-page: UNKNOWN
 Author: Bloom Research
 Author-email: rosebloomresearch@gmail.com
 License: CC BY 4.0
 Description: ## WaveForm
```

### Comparing `WaveFormer-0.1.1/README.md` & `WaveFormer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/WaveFormer.egg-info/PKG-INFO` & `WaveFormer-0.1.2/WaveFormer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaveFormer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A single unified Advanced Audio Processing toolkit, that provides both High-Level and Low-Level approaches to its extensive collection of tools.
 Home-page: UNKNOWN
 Author: Bloom Research
 Author-email: rosebloomresearch@gmail.com
 License: CC BY 4.0
 Description: ## WaveForm
```

### Comparing `WaveFormer-0.1.1/WaveFormer.egg-info/SOURCES.txt` & `WaveFormer-0.1.2/WaveFormer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/air.py` & `WaveFormer-0.1.2/audio_modules/air.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/core/configs.py` & `WaveFormer-0.1.2/audio_modules/core/configs.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/core/informers.py` & `WaveFormer-0.1.2/audio_modules/core/informers.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/extraction/commands.py` & `WaveFormer-0.1.2/audio_modules/extraction/commands.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/extraction/core.py` & `WaveFormer-0.1.2/audio_modules/extraction/core.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/extraction/extract_configs.py` & `WaveFormer-0.1.2/audio_modules/extraction/extract_configs.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/extraction/xtgraph.py` & `WaveFormer-0.1.2/audio_modules/extraction/xtgraph.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/nvision/configs.py` & `WaveFormer-0.1.2/audio_modules/nvision/configs.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/nvision/core.py` & `WaveFormer-0.1.2/audio_modules/nvision/core.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/nvision/ngraph.py` & `WaveFormer-0.1.2/audio_modules/nvision/ngraph.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/nvision/plotly_mappings.py` & `WaveFormer-0.1.2/audio_modules/nvision/plotly_mappings.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/praat/configs.py` & `WaveFormer-0.1.2/audio_modules/praat/configs.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/praat/core.py` & `WaveFormer-0.1.2/audio_modules/praat/core.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/praat/filters.py` & `WaveFormer-0.1.2/audio_modules/praat/filters.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/praat/formant.py` & `WaveFormer-0.1.2/audio_modules/praat/formant.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/praat/handlers.py` & `WaveFormer-0.1.2/audio_modules/praat/handlers.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/praat/processor.py` & `WaveFormer-0.1.2/audio_modules/praat/processor.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/praat/spectrogram.py` & `WaveFormer-0.1.2/audio_modules/praat/spectrogram.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/audio_modules/types.py` & `WaveFormer-0.1.2/audio_modules/types.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/rubberband/options.py` & `WaveFormer-0.1.2/rubberband/options.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/rubberband/rubberbandstretcher.py` & `WaveFormer-0.1.2/rubberband/rubberbandstretcher.py`

 * *Files identical despite different names*

### Comparing `WaveFormer-0.1.1/setup.py` & `WaveFormer-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requirements = f.read().splitlines()
     
 with open('readme.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='WaveFormer',  
-    version='0.1.1', 
+    version='0.1.2', 
     description='A single unified Advanced Audio Processing toolkit, that provides both High-Level and Low-Level approaches to its extensive collection of tools.',
     long_description=long_description,
     author='Bloom Research',
     author_email='rosebloomresearch@gmail.com',
     packages=find_packages(),  
     package_data={'': ['rubberband_builds/*.dll']},
     install_requires=requirements,
```

