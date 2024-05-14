# Comparing `tmp/anaouder-0.9.1.tar.gz` & `tmp/anaouder-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anaouder-0.9.1.tar", last modified: Mon May 13 11:55:17 2024, max compression
+gzip compressed data, was "anaouder-0.9.2.tar", last modified: Tue May 14 16:51:19 2024, max compression
```

## Comparing `anaouder-0.9.1.tar` & `anaouder-0.9.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.480837 anaouder-0.9.1/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2018 2024-05-13 11:38:08.000000 anaouder-0.9.1/CHANGELOG.md
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     6754 2024-05-13 11:55:17.480837 anaouder-0.9.1/PKG-INFO
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5609 2024-05-13 11:51:35.000000 anaouder-0.9.1/README-fr.md
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5083 2024-05-13 11:52:12.000000 anaouder-0.9.1/README.md
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.476836 anaouder-0.9.1/anaouder/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      180 2023-10-21 14:25:36.000000 anaouder-0.9.1/anaouder/__init__.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11650 2024-05-13 11:54:43.000000 anaouder-0.9.1/anaouder/adskrivan.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.480837 anaouder-0.9.1/anaouder/asr/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        0 2023-05-20 06:43:27.000000 anaouder-0.9.1/anaouder/asr/__init__.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       74 2023-05-20 06:43:27.000000 anaouder-0.9.1/anaouder/asr/inorm_units.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3698 2024-03-09 16:05:14.000000 anaouder-0.9.1/anaouder/asr/models.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     6255 2024-05-13 10:09:57.000000 anaouder-0.9.1/anaouder/asr/post_processing.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2797 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/asr/postproc_sub.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4993 2024-05-13 10:13:05.000000 anaouder-0.9.1/anaouder/asr/recognizer.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.480837 anaouder-0.9.1/anaouder/audio/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5482 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/audio/__init__.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.480837 anaouder-0.9.1/anaouder/dicts/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2769 2023-10-21 14:25:36.000000 anaouder-0.9.1/anaouder/dicts/__init__.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3263 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/dicts/acronyms.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5601 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/dicts/corrected_tokens.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3328 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/dicts/noun_f.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4439 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/dicts/noun_m.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18304 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/dicts/proper_nouns_phon.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3415 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/dicts/standard_tokens.tsv
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)      206 2023-11-30 08:14:18.000000 anaouder-0.9.1/anaouder/istitlan.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11135 2024-03-09 15:05:10.000000 anaouder-0.9.1/anaouder/linennan.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     3688 2024-03-09 16:46:02.000000 anaouder-0.9.1/anaouder/mikro.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     1185 2023-11-10 20:39:34.000000 anaouder-0.9.1/anaouder/normalizan.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.480837 anaouder-0.9.1/anaouder/text/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3446 2023-11-10 20:39:34.000000 anaouder-0.9.1/anaouder/text/__init__.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4275 2023-05-23 13:01:08.000000 anaouder-0.9.1/anaouder/text/definitions.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    13824 2023-11-10 20:39:34.000000 anaouder-0.9.1/anaouder/text/inverse_normalizer.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    10825 2023-10-21 14:25:37.000000 anaouder-0.9.1/anaouder/text/normalizer.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18371 2023-10-21 14:25:37.000000 anaouder-0.9.1/anaouder/text/tokenizer.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3687 2023-10-21 14:25:37.000000 anaouder-0.9.1/anaouder/text/utils.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5396 2024-05-13 08:15:45.000000 anaouder-0.9.1/anaouder/utils.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       17 2024-05-13 09:34:17.000000 anaouder-0.9.1/anaouder/version.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.480837 anaouder-0.9.1/anaouder.egg-info/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     6754 2024-05-13 11:55:17.000000 anaouder-0.9.1/anaouder.egg-info/PKG-INFO
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      979 2024-05-13 11:55:17.000000 anaouder-0.9.1/anaouder.egg-info/SOURCES.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        1 2024-05-13 11:55:17.000000 anaouder-0.9.1/anaouder.egg-info/dependency_links.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      189 2024-05-13 11:55:17.000000 anaouder-0.9.1/anaouder.egg-info/entry_points.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       73 2024-05-13 11:55:17.000000 anaouder-0.9.1/anaouder.egg-info/requires.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        9 2024-05-13 11:55:17.000000 anaouder-0.9.1/anaouder.egg-info/top_level.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       38 2024-05-13 11:55:17.480837 anaouder-0.9.1/setup.cfg
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2080 2024-03-09 17:01:43.000000 anaouder-0.9.1/setup.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.330364 anaouder-0.9.2/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2018 2024-05-14 16:50:44.000000 anaouder-0.9.2/CHANGELOG.md
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     7264 2024-05-14 16:51:19.330364 anaouder-0.9.2/PKG-INFO
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5609 2024-05-13 11:51:35.000000 anaouder-0.9.2/README-fr.md
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5083 2024-05-13 11:52:12.000000 anaouder-0.9.2/README.md
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.326364 anaouder-0.9.2/anaouder/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      180 2023-10-21 14:25:36.000000 anaouder-0.9.2/anaouder/__init__.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11650 2024-05-13 11:54:43.000000 anaouder-0.9.2/anaouder/adskrivan.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.326364 anaouder-0.9.2/anaouder/asr/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        0 2023-05-20 06:43:27.000000 anaouder-0.9.2/anaouder/asr/__init__.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       74 2023-05-20 06:43:27.000000 anaouder-0.9.2/anaouder/asr/inorm_units.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3698 2024-03-09 16:05:14.000000 anaouder-0.9.2/anaouder/asr/models.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     6255 2024-05-13 10:09:57.000000 anaouder-0.9.2/anaouder/asr/post_processing.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2797 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/asr/postproc_sub.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4870 2024-05-14 16:45:26.000000 anaouder-0.9.2/anaouder/asr/recognizer.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.326364 anaouder-0.9.2/anaouder/audio/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5482 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/audio/__init__.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.330364 anaouder-0.9.2/anaouder/dicts/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2769 2023-10-21 14:25:36.000000 anaouder-0.9.2/anaouder/dicts/__init__.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3263 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/dicts/acronyms.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5601 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/dicts/corrected_tokens.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3328 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/dicts/noun_f.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4439 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/dicts/noun_m.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18304 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/dicts/proper_nouns_phon.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3415 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/dicts/standard_tokens.tsv
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)      206 2023-11-30 08:14:18.000000 anaouder-0.9.2/anaouder/istitlan.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11135 2024-03-09 15:05:10.000000 anaouder-0.9.2/anaouder/linennan.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     3688 2024-03-09 16:46:02.000000 anaouder-0.9.2/anaouder/mikro.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     1185 2023-11-10 20:39:34.000000 anaouder-0.9.2/anaouder/normalizan.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.330364 anaouder-0.9.2/anaouder/text/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3446 2023-11-10 20:39:34.000000 anaouder-0.9.2/anaouder/text/__init__.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4275 2023-05-23 13:01:08.000000 anaouder-0.9.2/anaouder/text/definitions.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    13824 2023-11-10 20:39:34.000000 anaouder-0.9.2/anaouder/text/inverse_normalizer.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    10825 2023-10-21 14:25:37.000000 anaouder-0.9.2/anaouder/text/normalizer.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18371 2023-10-21 14:25:37.000000 anaouder-0.9.2/anaouder/text/tokenizer.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3687 2023-10-21 14:25:37.000000 anaouder-0.9.2/anaouder/text/utils.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5396 2024-05-13 08:15:45.000000 anaouder-0.9.2/anaouder/utils.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       17 2024-05-14 16:50:31.000000 anaouder-0.9.2/anaouder/version.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.326364 anaouder-0.9.2/anaouder.egg-info/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     7264 2024-05-14 16:51:19.000000 anaouder-0.9.2/anaouder.egg-info/PKG-INFO
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      979 2024-05-14 16:51:19.000000 anaouder-0.9.2/anaouder.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        1 2024-05-14 16:51:19.000000 anaouder-0.9.2/anaouder.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      189 2024-05-14 16:51:19.000000 anaouder-0.9.2/anaouder.egg-info/entry_points.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       73 2024-05-14 16:51:19.000000 anaouder-0.9.2/anaouder.egg-info/requires.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        9 2024-05-14 16:51:19.000000 anaouder-0.9.2/anaouder.egg-info/top_level.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       38 2024-05-14 16:51:19.330364 anaouder-0.9.2/setup.cfg
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2083 2024-05-13 11:56:35.000000 anaouder-0.9.2/setup.py
```

### Comparing `anaouder-0.9.1/CHANGELOG.md` & `anaouder-0.9.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## [0.9.1] - 2024-05-13
+## [0.9.2] - 2024-05-14
 
 - Better segmentation when decoding to a text file with `-o/--output` option.
 - Shows a progress bar when decoding to a text file with `-o/--output` option.
 - Included Anaouder version in EAF headers.
 - Removed optional use of translation dictionaries.
 
 ## [0.9.0] - 2024-03-09
```

### Comparing `anaouder-0.9.1/README-fr.md` & `anaouder-0.9.2/README-fr.md`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/README.md` & `anaouder-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/adskrivan.py` & `anaouder-0.9.2/anaouder/adskrivan.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/asr/models.py` & `anaouder-0.9.2/anaouder/asr/models.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/asr/post_processing.py` & `anaouder-0.9.2/anaouder/asr/post_processing.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/asr/postproc_sub.tsv` & `anaouder-0.9.2/anaouder/asr/postproc_sub.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/asr/recognizer.py` & `anaouder-0.9.2/anaouder/asr/recognizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,20 +112,17 @@
         The resulting transcription is a list of Vosk tokens
         Each Vosk token is a dictionary of the form:
             {'word': str, 'start': float, 'end': float, 'conf': float}
         'start' and 'end' keys are in seconds
         'conf' is a normalized confidence score
     """
 
-    def format_output(result, normalize=False) -> List[dict]:
+    def format_output(result) -> List[dict]:
         jres = json.loads(result)
         return jres.get("result", [])
-        if not "result" in jres:
-            return []
-        return jres["result"]
 
     model = load_model()
     recognizer = KaldiRecognizer(model, 16000)
     recognizer.SetWords(True)
     
     total_duration = get_audiofile_length(filepath)
     progress_bar = tqdm(total=ceil(total_duration))
@@ -138,17 +135,17 @@
                                 "-ar", "16000" , "-ac", "1", "-f", "s16le", "-"],
                                 stdout=subprocess.PIPE) as process:
         while True:
             data = process.stdout.read(4000)
             if len(data) == 0:
                 break
             if recognizer.AcceptWaveform(data):
-                tokens.extend(format_output(recognizer.Result(), normalize))
+                tokens.extend(format_output(recognizer.Result()))
             cumul_frames += len(data) // 2
             if i%10 == 0:
                 progress_bar.update(cumul_frames / 16000)
                 cumul_frames = 0
             i += 1
-        tokens.extend(format_output(recognizer.FinalResult(), normalize))
+        tokens.extend(format_output(recognizer.FinalResult()))
     progress_bar.close()
     
-    return tokens
+    return tokens
```

### Comparing `anaouder-0.9.1/anaouder/audio/__init__.py` & `anaouder-0.9.2/anaouder/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/dicts/__init__.py` & `anaouder-0.9.2/anaouder/dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/dicts/acronyms.tsv` & `anaouder-0.9.2/anaouder/dicts/acronyms.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/dicts/corrected_tokens.tsv` & `anaouder-0.9.2/anaouder/dicts/corrected_tokens.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/dicts/noun_f.tsv` & `anaouder-0.9.2/anaouder/dicts/noun_f.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/dicts/noun_m.tsv` & `anaouder-0.9.2/anaouder/dicts/noun_m.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/dicts/proper_nouns_phon.tsv` & `anaouder-0.9.2/anaouder/dicts/proper_nouns_phon.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/dicts/standard_tokens.tsv` & `anaouder-0.9.2/anaouder/dicts/standard_tokens.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/linennan.py` & `anaouder-0.9.2/anaouder/linennan.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/mikro.py` & `anaouder-0.9.2/anaouder/mikro.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/normalizan.py` & `anaouder-0.9.2/anaouder/normalizan.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/text/__init__.py` & `anaouder-0.9.2/anaouder/text/__init__.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/text/definitions.py` & `anaouder-0.9.2/anaouder/text/definitions.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/text/inverse_normalizer.py` & `anaouder-0.9.2/anaouder/text/inverse_normalizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/text/normalizer.py` & `anaouder-0.9.2/anaouder/text/normalizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/text/tokenizer.py` & `anaouder-0.9.2/anaouder/text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/text/utils.py` & `anaouder-0.9.2/anaouder/text/utils.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder/utils.py` & `anaouder-0.9.2/anaouder/utils.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/anaouder.egg-info/SOURCES.txt` & `anaouder-0.9.2/anaouder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.1/setup.py` & `anaouder-0.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     name=NAME,
     url=URL,
     version=VERSION,
     author=AUTHOR,
     licence="MIT",
     author_email=EMAIL,
     description=DESCRIPTION,
-    long_description=open("README.md", encoding="utf-8").read(),
+    long_description=open("README-fr.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     python_requires=REQUIRES_PYTHON,
     install_requires=REQUIREMENTS,
     classifiers=[
 		"Intended Audience :: Developers",
 		"License :: OSI Approved :: MIT License",
 		"Programming Language :: Python",
```

