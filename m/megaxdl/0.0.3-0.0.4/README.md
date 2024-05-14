# Comparing `tmp/megaxdl-0.0.3.tar.gz` & `tmp/megaxdl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megaxdl-0.0.3.tar", last modified: Tue May 14 10:47:34 2024, max compression
+gzip compressed data, was "megaxdl-0.0.4.tar", last modified: Tue May 14 10:57:51 2024, max compression
```

## Comparing `megaxdl-0.0.3.tar` & `megaxdl-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:34.335612 megaxdl-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 10:47:30.000000 megaxdl-0.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:34.335612 megaxdl-0.0.3/Megaxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 10:47:30.000000 megaxdl-0.0.3/Megaxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 10:47:30.000000 megaxdl-0.0.3/Megaxdl/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 10:47:30.000000 megaxdl-0.0.3/Megaxdl/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    38458 2024-05-14 10:47:30.000000 megaxdl-0.0.3/Megaxdl/mega.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 10:47:34.335612 megaxdl-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 10:47:30.000000 megaxdl-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:34.335612 megaxdl-0.0.3/megaxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 10:47:34.000000 megaxdl-0.0.3/megaxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 10:47:34.000000 megaxdl-0.0.3/megaxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:47:34.000000 megaxdl-0.0.3/megaxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 10:47:34.000000 megaxdl-0.0.3/megaxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 10:47:34.000000 megaxdl-0.0.3/megaxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:47:34.335612 megaxdl-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 10:47:30.000000 megaxdl-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:57:51.242373 megaxdl-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 10:57:43.000000 megaxdl-0.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:57:51.238373 megaxdl-0.0.4/Megaxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 10:57:43.000000 megaxdl-0.0.4/Megaxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 10:57:43.000000 megaxdl-0.0.4/Megaxdl/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 10:57:43.000000 megaxdl-0.0.4/Megaxdl/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38491 2024-05-14 10:57:43.000000 megaxdl-0.0.4/Megaxdl/mega.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 10:57:51.242373 megaxdl-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 10:57:43.000000 megaxdl-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:57:51.242373 megaxdl-0.0.4/megaxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 10:57:51.000000 megaxdl-0.0.4/megaxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 10:57:51.000000 megaxdl-0.0.4/megaxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:57:51.000000 megaxdl-0.0.4/megaxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 10:57:51.000000 megaxdl-0.0.4/megaxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 10:57:51.000000 megaxdl-0.0.4/megaxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:57:51.242373 megaxdl-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 10:57:43.000000 megaxdl-0.0.4/setup.py
```

### Comparing `megaxdl-0.0.3/LICENSE` & `megaxdl-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.3/Megaxdl/crypto.py` & `megaxdl-0.0.4/Megaxdl/crypto.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.3/Megaxdl/errors.py` & `megaxdl-0.0.4/Megaxdl/errors.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.3/Megaxdl/mega.py` & `megaxdl-0.0.4/Megaxdl/mega.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,26 +632,26 @@
             'cr': [[node_id], [node_id], [0, 0, encrypted_node_key]]
         }]
         self._api_request(request_body)
         nodes = self.get_files()
         return self.get_folder_link(nodes[node_id])
 
 
-    def download(self, file, dest_path=None, dest_filename=None):
-        return self.sdownload(file_uid=None, file_key=None, file=file[1], message=None, progress=None, is_public=False, dest_path=dest_path, dest_filename=dest_filename)
+    def download(self, file, dest_path=None, dest_filename=None, message=None, progress=None):
+        return self.sdownload(file_uid=None, file_key=None, file=file[1], is_public=False, message=message, progress=progress, dest_path=dest_path, dest_filename=dest_filename)
 
 
     def download_url(self, url, message=None, progress=None, dest_path=None, dest_filename=None, no_temp_file=False):
         path_mid = self._parse_url(url).split('!')
         file_uid = path_mid[0]
         file_key = path_mid[1]
-        return self.sdownload(file_uid, file_key, message=None, progress=None, is_public=True, dest_path=dest_path, dest_filename=dest_filename, no_temp_file=no_temp_file)
+        return self.sdownload(file_uid, file_key, message=message, progress=progress, is_public=True, dest_path=dest_path, dest_filename=dest_filename, no_temp_file=no_temp_file)
 
 
-    def sdownload(self, file_uid, file_key, file=None, message=None, progress=None, dest_path=None, dest_filename=None, is_public=False, no_temp_file=False):
+    def sdownload(self, file_uid, file_key, message, progress, file=None, dest_path=None, dest_filename=None, is_public=False, no_temp_file=False):
 
         stime = time.time()
         if file == None:
             file_key = base64_to_a32(file_key) if is_public else file_key
             file_data = self._api_request({'a': 'g', 'g': 1, 'p' if is_public else 'n': file_uid})
             k = (file_key[0] ^ file_key[4], file_key[1] ^ file_key[5], file_key[2] ^ file_key[6], file_key[3] ^ file_key[7])
             iv = file_key[4:6] + (0, 0)
```

### Comparing `megaxdl-0.0.3/PKG-INFO` & `megaxdl-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.3
+Version: 0.0.4
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
```

### Comparing `megaxdl-0.0.3/README.md` & `megaxdl-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.3/megaxdl.egg-info/PKG-INFO` & `megaxdl-0.0.4/megaxdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.3
+Version: 0.0.4
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
```

### Comparing `megaxdl-0.0.3/setup.py` & `megaxdl-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 
 install = ["tqdm>=4.64.1",
            "tenacity>=8.2.2",
            "requests>=2.27.1",
            "pycryptodome>=3.20.0,<4.0.0"]
 
 setup(name='megaxdl',
-      version='0.0.3',
+      version='0.0.4',
       python_requires='~=3.10',
       packages=find_packages(),
       long_description=readme,
       install_requires=install,
       include_package_data=True,
       long_description_content_type='text/markdown')
```

