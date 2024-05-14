# Comparing `tmp/megaxdl-0.0.8.tar.gz` & `tmp/megaxdl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megaxdl-0.0.8.tar", last modified: Tue May 14 15:45:25 2024, max compression
+gzip compressed data, was "megaxdl-0.0.9.tar", last modified: Tue May 14 15:56:10 2024, max compression
```

## Comparing `megaxdl-0.0.8.tar` & `megaxdl-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:45:25.890443 megaxdl-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 15:45:17.000000 megaxdl-0.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:45:25.890443 megaxdl-0.0.8/Megaxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 15:45:17.000000 megaxdl-0.0.8/Megaxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 15:45:17.000000 megaxdl-0.0.8/Megaxdl/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 15:45:17.000000 megaxdl-0.0.8/Megaxdl/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    16291 2024-05-14 15:45:17.000000 megaxdl-0.0.8/Megaxdl/mega.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 15:45:25.890443 megaxdl-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 15:45:17.000000 megaxdl-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:45:25.890443 megaxdl-0.0.8/megaxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 15:45:25.000000 megaxdl-0.0.8/megaxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 15:45:25.000000 megaxdl-0.0.8/megaxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:45:25.000000 megaxdl-0.0.8/megaxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 15:45:25.000000 megaxdl-0.0.8/megaxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 15:45:25.000000 megaxdl-0.0.8/megaxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:45:25.890443 megaxdl-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-14 15:45:17.000000 megaxdl-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:56:10.254344 megaxdl-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 15:56:02.000000 megaxdl-0.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:56:10.250344 megaxdl-0.0.9/Megaxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 15:56:02.000000 megaxdl-0.0.9/Megaxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 15:56:02.000000 megaxdl-0.0.9/Megaxdl/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 15:56:02.000000 megaxdl-0.0.9/Megaxdl/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16291 2024-05-14 15:56:02.000000 megaxdl-0.0.9/Megaxdl/mega.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 15:56:10.254344 megaxdl-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 15:56:02.000000 megaxdl-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:56:10.254344 megaxdl-0.0.9/megaxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-14 15:56:10.000000 megaxdl-0.0.9/megaxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 15:56:10.000000 megaxdl-0.0.9/megaxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:56:10.000000 megaxdl-0.0.9/megaxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 15:56:10.000000 megaxdl-0.0.9/megaxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 15:56:10.000000 megaxdl-0.0.9/megaxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:56:10.254344 megaxdl-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-14 15:56:02.000000 megaxdl-0.0.9/setup.py
```

### Comparing `megaxdl-0.0.8/LICENSE` & `megaxdl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.8/Megaxdl/crypto.py` & `megaxdl-0.0.9/Megaxdl/crypto.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.8/Megaxdl/errors.py` & `megaxdl-0.0.9/Megaxdl/errors.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.8/Megaxdl/mega.py` & `megaxdl-0.0.9/Megaxdl/mega.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,26 +242,26 @@
     async def parse_uri(self, url: str):
         url = await self.follow_redirects(url)
         if '/file/' in url:
             url = url.replace(' ', '')
             file_id = re.findall(r'\W\w\w\w\w\w\w\w\w\W', url)[0][1:-1]
             id_index = re.search(file_id, url).end()
             key = url[id_index + 1:]
-            return f'{file_id}!{key}'
+            return f'{file_id}!{key}'.split('!')
         elif '!' in url:
             match = re.findall(r'/#!(.*)', url)
             path = match[0]
-            return path
+            return path.split('!')
         else:
             raise RequestError('Url key missing')
 
 #===================================================================================================================================
 
     async def download(self, url, message=None, progress=None, dest_path=None, dest_filename=None):
-        path_mid = await self.parse_uri(url).split('!')
+        path_mid = await self.parse_uri(url)
         file_uid = path_mid[0]
         file_key = path_mid[1]
         return await self.downloadR(file_uid, file_key, message=message, progress=progress,
                                is_public=True, dest_path=dest_path, dest_filename=dest_filename)
 
 #===================================================================================================================================
     
@@ -323,15 +323,15 @@
             tlocation.close()
             shutil.move(output_name, output_path)
             return output_path
 
 #===================================================================================================================================
     
     async def getinfo(self, url):
-        fileuid, filekey = await self.parse_uri(url).split('!')
+        fileuid, filekey = await self.parse_uri(url)
         return await self.exeinfo(fileuid, filekey)
 
 #===================================================================================================================================
 
     async def exeinfo(self, file_uid, file_key):
         data = self.api_request({'a': 'g', 'p': file_uid, 'ssm': 1})
         if isinstance(data, int):
```

### Comparing `megaxdl-0.0.8/PKG-INFO` & `megaxdl-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.8
+Version: 0.0.9
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
```

### Comparing `megaxdl-0.0.8/README.md` & `megaxdl-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.8/megaxdl.egg-info/PKG-INFO` & `megaxdl-0.0.9/megaxdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.8
+Version: 0.0.9
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
```

