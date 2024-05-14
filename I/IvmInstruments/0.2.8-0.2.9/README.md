# Comparing `tmp/ivminstruments-0.2.8.tar.gz` & `tmp/ivminstruments-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivminstruments-0.2.8.tar", last modified: Mon May 13 16:36:11 2024, max compression
+gzip compressed data, was "ivminstruments-0.2.9.tar", last modified: Tue May 14 08:28:45 2024, max compression
```

## Comparing `ivminstruments-0.2.8.tar` & `ivminstruments-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:36:11.905316 ivminstruments-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:36:11.905316 ivminstruments-0.2.8/Instruments/
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-13 16:35:56.000000 ivminstruments-0.2.8/Instruments/DigitalScope.py
--rw-r--r--   0 runner    (1001) docker     (127)    23077 2024-05-13 16:35:56.000000 ivminstruments-0.2.8/Instruments/KeySight_N670x.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-13 16:35:56.000000 ivminstruments-0.2.8/Instruments/KeySight_RP7954.py
--rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-05-13 16:35:56.000000 ivminstruments-0.2.8/Instruments/Keysight_34461.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-13 16:35:56.000000 ivminstruments-0.2.8/Instruments/Keysight_E362x.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 16:35:56.000000 ivminstruments-0.2.8/Instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-13 16:35:56.000000 ivminstruments-0.2.8/Instruments/multimeter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:36:11.905316 ivminstruments-0.2.8/IvmInstruments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 16:36:11.000000 ivminstruments-0.2.8/IvmInstruments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-13 16:36:11.000000 ivminstruments-0.2.8/IvmInstruments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:36:11.000000 ivminstruments-0.2.8/IvmInstruments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 16:36:11.000000 ivminstruments-0.2.8/IvmInstruments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-13 16:35:56.000000 ivminstruments-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 16:36:11.905316 ivminstruments-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 16:35:56.000000 ivminstruments-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:36:11.905316 ivminstruments-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-13 16:35:56.000000 ivminstruments-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:28:45.508434 ivminstruments-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:28:45.508434 ivminstruments-0.2.9/Instruments/
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-14 08:28:33.000000 ivminstruments-0.2.9/Instruments/DigitalScope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23077 2024-05-14 08:28:33.000000 ivminstruments-0.2.9/Instruments/KeySight_N670x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-14 08:28:33.000000 ivminstruments-0.2.9/Instruments/KeySight_RP7954.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-05-14 08:28:33.000000 ivminstruments-0.2.9/Instruments/Keysight_34461.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-14 08:28:33.000000 ivminstruments-0.2.9/Instruments/Keysight_E362x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-14 08:28:33.000000 ivminstruments-0.2.9/Instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-14 08:28:33.000000 ivminstruments-0.2.9/Instruments/multimeter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:28:45.508434 ivminstruments-0.2.9/IvmInstruments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-14 08:28:45.000000 ivminstruments-0.2.9/IvmInstruments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-14 08:28:45.000000 ivminstruments-0.2.9/IvmInstruments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:28:45.000000 ivminstruments-0.2.9/IvmInstruments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 08:28:45.000000 ivminstruments-0.2.9/IvmInstruments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-14 08:28:33.000000 ivminstruments-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-14 08:28:45.508434 ivminstruments-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 08:28:33.000000 ivminstruments-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:28:45.508434 ivminstruments-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-14 08:28:33.000000 ivminstruments-0.2.9/setup.py
```

### Comparing `ivminstruments-0.2.8/Instruments/DigitalScope.py` & `ivminstruments-0.2.9/Instruments/DigitalScope.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.8/Instruments/KeySight_N670x.py` & `ivminstruments-0.2.9/Instruments/KeySight_N670x.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.8/Instruments/KeySight_RP7954.py` & `ivminstruments-0.2.9/Instruments/KeySight_RP7954.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.8/Instruments/Keysight_34461.py` & `ivminstruments-0.2.9/Instruments/Keysight_34461.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.8/Instruments/Keysight_E362x.py` & `ivminstruments-0.2.9/Instruments/Keysight_E362x.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.8/Instruments/multimeter.py` & `ivminstruments-0.2.9/Instruments/multimeter.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.8/LICENSE` & `ivminstruments-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.8/setup.py` & `ivminstruments-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 AUTHOR_USER_NAME = 'HarishKumarSedu'
 AUTHOR_EMAIL = 'harishkumarsedu@gmail.com'
 REPO_NAME = 'Instruments'
 setup(
     name=f'Ivm{REPO_NAME}',
     author=AUTHOR_USER_NAME,
     author_email=AUTHOR_EMAIL,
-    version='0.2.8',
+    version='0.2.9',
     py_modules=['Instruments'],
     description=[ 'text/markdown','text/x-rst',],
     url=f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
     project_urls={
         "Bug Tracker": f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}/issues",
     },
     long_description=long_description,
```

