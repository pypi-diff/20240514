# Comparing `tmp/superb-ai-apps-0.0.8.tar.gz` & `tmp/superb-ai-apps-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superb-ai-apps-0.0.8.tar", last modified: Fri May  3 07:19:40 2024, max compression
+gzip compressed data, was "superb-ai-apps-0.0.9.tar", last modified: Tue May 14 05:41:16 2024, max compression
```

## Comparing `superb-ai-apps-0.0.8.tar` & `superb-ai-apps-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:19:40.072488 superb-ai-apps-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-03 07:19:40.072488 superb-ai-apps-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 07:19:26.000000 superb-ai-apps-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 07:19:40.072488 superb-ai-apps-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-03 07:19:26.000000 superb-ai-apps-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:19:40.068488 superb-ai-apps-0.0.8/spb_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:19:26.000000 superb-ai-apps-0.0.8/spb_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-03 07:19:26.000000 superb-ai-apps-0.0.8/spb_apps/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:19:40.072488 superb-ai-apps-0.0.8/spb_apps/curate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:19:26.000000 superb-ai-apps-0.0.8/spb_apps/curate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:19:26.000000 superb-ai-apps-0.0.8/spb_apps/curate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:19:40.072488 superb-ai-apps-0.0.8/spb_apps/label/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:19:26.000000 superb-ai-apps-0.0.8/spb_apps/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11965 2024-05-03 07:19:26.000000 superb-ai-apps-0.0.8/spb_apps/superb_curate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-05-03 07:19:26.000000 superb-ai-apps-0.0.8/spb_apps/superb_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:19:40.072488 superb-ai-apps-0.0.8/spb_apps/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:19:26.000000 superb-ai-apps-0.0.8/spb_apps/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-03 07:19:26.000000 superb-ai-apps-0.0.8/spb_apps/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-05-03 07:19:26.000000 superb-ai-apps-0.0.8/spb_apps/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:19:40.072488 superb-ai-apps-0.0.8/superb_ai_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-03 07:19:40.000000 superb-ai-apps-0.0.8/superb_ai_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-03 07:19:40.000000 superb-ai-apps-0.0.8/superb_ai_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:19:40.000000 superb-ai-apps-0.0.8/superb_ai_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-03 07:19:40.000000 superb-ai-apps-0.0.8/superb_ai_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 07:19:40.000000 superb-ai-apps-0.0.8/superb_ai_apps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:41:16.346781 superb-ai-apps-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-14 05:41:16.346781 superb-ai-apps-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 05:41:05.000000 superb-ai-apps-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 05:41:16.346781 superb-ai-apps-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-14 05:41:05.000000 superb-ai-apps-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:41:16.346781 superb-ai-apps-0.0.9/spb_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:41:05.000000 superb-ai-apps-0.0.9/spb_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-14 05:41:05.000000 superb-ai-apps-0.0.9/spb_apps/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:41:16.346781 superb-ai-apps-0.0.9/spb_apps/curate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:41:05.000000 superb-ai-apps-0.0.9/spb_apps/curate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:41:05.000000 superb-ai-apps-0.0.9/spb_apps/curate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:41:16.346781 superb-ai-apps-0.0.9/spb_apps/label/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:41:05.000000 superb-ai-apps-0.0.9/spb_apps/label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11965 2024-05-14 05:41:05.000000 superb-ai-apps-0.0.9/spb_apps/superb_curate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23623 2024-05-14 05:41:05.000000 superb-ai-apps-0.0.9/spb_apps/superb_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:41:16.346781 superb-ai-apps-0.0.9/spb_apps/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:41:05.000000 superb-ai-apps-0.0.9/spb_apps/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-14 05:41:05.000000 superb-ai-apps-0.0.9/spb_apps/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-05-14 05:41:05.000000 superb-ai-apps-0.0.9/spb_apps/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:41:16.346781 superb-ai-apps-0.0.9/superb_ai_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-14 05:41:16.000000 superb-ai-apps-0.0.9/superb_ai_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-14 05:41:16.000000 superb-ai-apps-0.0.9/superb_ai_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 05:41:16.000000 superb-ai-apps-0.0.9/superb_ai_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-14 05:41:16.000000 superb-ai-apps-0.0.9/superb_ai_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 05:41:16.000000 superb-ai-apps-0.0.9/superb_ai_apps.egg-info/top_level.txt
```

### Comparing `superb-ai-apps-0.0.8/setup.py` & `superb-ai-apps-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="superb-ai-apps",
-    version="0.0.8",
+    version="0.0.9",
     description="Python Package for Superb-AI Apps",
     install_requires=[
         "asttokens==2.4.1",
         "attrs==23.2.0",
         "backcall==0.2.0",
         "beautifulsoup4==4.12.3",
         "bleach==6.1.0",
@@ -70,10 +70,12 @@
         "traitlets==5.14.2",
         "typing_extensions==4.10.0",
         "urllib3==2.2.1",
         "wcwidth==0.2.13",
         "webencodings==0.5.1",
         "yarg==0.1.9",
         "zipp==3.18.1",
+        "natsort==8.4.0",
+        "tqdm==4.66.4",
     ],
     packages=find_packages(exclude=("tests*", "testing*")),
 )
```

### Comparing `superb-ai-apps-0.0.8/spb_apps/apps.py` & `superb-ai-apps-0.0.9/spb_apps/apps.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.8/spb_apps/superb_curate.py` & `superb-ai-apps-0.0.9/spb_apps/superb_curate.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.8/spb_apps/utils/converter.py` & `superb-ai-apps-0.0.9/spb_apps/utils/converter.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.8/spb_apps/utils/utils.py` & `superb-ai-apps-0.0.9/spb_apps/utils/utils.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.8/superb_ai_apps.egg-info/requires.txt` & `superb-ai-apps-0.0.9/superb_ai_apps.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -63,7 +63,9 @@
 traitlets==5.14.2
 typing_extensions==4.10.0
 urllib3==2.2.1
 wcwidth==0.2.13
 webencodings==0.5.1
 yarg==0.1.9
 zipp==3.18.1
+natsort==8.4.0
+tqdm==4.66.4
```

