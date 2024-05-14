# Comparing `tmp/megaxdl-0.0.7.tar.gz` & `tmp/megaxdl-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megaxdl-0.0.7.tar", last modified: Tue May 14 15:37:10 2024, max compression
+gzip compressed data, was "megaxdl-0.0.8.tar", last modified: Tue May 14 15:45:25 2024, max compression
```

## Comparing `megaxdl-0.0.7.tar` & `megaxdl-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:37:10.838658 megaxdl-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 15:37:06.000000 megaxdl-0.0.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:37:10.838658 megaxdl-0.0.7/Megaxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 15:37:06.000000 megaxdl-0.0.7/Megaxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 15:37:06.000000 megaxdl-0.0.7/Megaxdl/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 15:37:06.000000 megaxdl-0.0.7/Megaxdl/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-14 15:37:06.000000 megaxdl-0.0.7/Megaxdl/mega.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 15:37:10.838658 megaxdl-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 15:37:06.000000 megaxdl-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:37:10.838658 megaxdl-0.0.7/megaxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 15:37:10.000000 megaxdl-0.0.7/megaxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 15:37:10.000000 megaxdl-0.0.7/megaxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:37:10.000000 megaxdl-0.0.7/megaxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 15:37:10.000000 megaxdl-0.0.7/megaxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 15:37:10.000000 megaxdl-0.0.7/megaxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:37:10.838658 megaxdl-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-14 15:37:06.000000 megaxdl-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:45:25.890443 megaxdl-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 15:45:17.000000 megaxdl-0.0.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:45:25.890443 megaxdl-0.0.8/Megaxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 15:45:17.000000 megaxdl-0.0.8/Megaxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 15:45:17.000000 megaxdl-0.0.8/Megaxdl/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 15:45:17.000000 megaxdl-0.0.8/Megaxdl/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16291 2024-05-14 15:45:17.000000 megaxdl-0.0.8/Megaxdl/mega.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 15:45:25.890443 megaxdl-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 15:45:17.000000 megaxdl-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:45:25.890443 megaxdl-0.0.8/megaxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 15:45:25.000000 megaxdl-0.0.8/megaxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 15:45:25.000000 megaxdl-0.0.8/megaxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:45:25.000000 megaxdl-0.0.8/megaxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 15:45:25.000000 megaxdl-0.0.8/megaxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 15:45:25.000000 megaxdl-0.0.8/megaxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:45:25.890443 megaxdl-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-14 15:45:17.000000 megaxdl-0.0.8/setup.py
```

### Comparing `megaxdl-0.0.7/LICENSE` & `megaxdl-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.7/Megaxdl/crypto.py` & `megaxdl-0.0.8/Megaxdl/crypto.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.7/Megaxdl/errors.py` & `megaxdl-0.0.8/Megaxdl/errors.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.7/Megaxdl/mega.py` & `megaxdl-0.0.8/Megaxdl/mega.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             if s_item['h'] in ok_dict:
                 shared_keys[s_item['u']][s_item['h']] = ok_dict[s_item['h']]
     
         self.shared_keys = shared_keys
 
 #===================================================================================================================================
 
-   def get_files(self):
+    def get_files(self):
         files = self.api_request({'a': 'f', 'c': 1, 'r': 1})
         files_dict = {}
         shared_keys = {}
         self._init_shared_keys(files, shared_keys)
         for file in files['f']:
             processed_file = self.process_file(file, shared_keys)
             if processed_file['a']:
```

### Comparing `megaxdl-0.0.7/PKG-INFO` & `megaxdl-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.7
+Version: 0.0.8
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
```

### Comparing `megaxdl-0.0.7/README.md` & `megaxdl-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.7/megaxdl.egg-info/PKG-INFO` & `megaxdl-0.0.8/megaxdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.7
+Version: 0.0.8
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
```

