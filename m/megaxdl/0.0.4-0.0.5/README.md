# Comparing `tmp/megaxdl-0.0.4.tar.gz` & `tmp/megaxdl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megaxdl-0.0.4.tar", last modified: Tue May 14 10:57:51 2024, max compression
+gzip compressed data, was "megaxdl-0.0.5.tar", last modified: Tue May 14 11:10:22 2024, max compression
```

## Comparing `megaxdl-0.0.4.tar` & `megaxdl-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:57:51.242373 megaxdl-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 10:57:43.000000 megaxdl-0.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:57:51.238373 megaxdl-0.0.4/Megaxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 10:57:43.000000 megaxdl-0.0.4/Megaxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 10:57:43.000000 megaxdl-0.0.4/Megaxdl/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 10:57:43.000000 megaxdl-0.0.4/Megaxdl/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    38491 2024-05-14 10:57:43.000000 megaxdl-0.0.4/Megaxdl/mega.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 10:57:51.242373 megaxdl-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 10:57:43.000000 megaxdl-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:57:51.242373 megaxdl-0.0.4/megaxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 10:57:51.000000 megaxdl-0.0.4/megaxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 10:57:51.000000 megaxdl-0.0.4/megaxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:57:51.000000 megaxdl-0.0.4/megaxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 10:57:51.000000 megaxdl-0.0.4/megaxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 10:57:51.000000 megaxdl-0.0.4/megaxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:57:51.242373 megaxdl-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 10:57:43.000000 megaxdl-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:10:22.978809 megaxdl-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 11:10:17.000000 megaxdl-0.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:10:22.974810 megaxdl-0.0.5/Megaxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 11:10:17.000000 megaxdl-0.0.5/Megaxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 11:10:17.000000 megaxdl-0.0.5/Megaxdl/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 11:10:17.000000 megaxdl-0.0.5/Megaxdl/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38433 2024-05-14 11:10:17.000000 megaxdl-0.0.5/Megaxdl/mega.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 11:10:22.978809 megaxdl-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 11:10:17.000000 megaxdl-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:10:22.978809 megaxdl-0.0.5/megaxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 11:10:22.000000 megaxdl-0.0.5/megaxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 11:10:22.000000 megaxdl-0.0.5/megaxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:10:22.000000 megaxdl-0.0.5/megaxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 11:10:22.000000 megaxdl-0.0.5/megaxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 11:10:22.000000 megaxdl-0.0.5/megaxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:10:22.978809 megaxdl-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 11:10:17.000000 megaxdl-0.0.5/setup.py
```

### Comparing `megaxdl-0.0.4/LICENSE` & `megaxdl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.4/Megaxdl/crypto.py` & `megaxdl-0.0.5/Megaxdl/crypto.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.4/Megaxdl/errors.py` & `megaxdl-0.0.5/Megaxdl/errors.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.4/Megaxdl/mega.py` & `megaxdl-0.0.5/Megaxdl/mega.py`

 * *Files 1% similar despite different names*

```diff
@@ -681,30 +681,29 @@
             mac_bytes = b'\0' * 16
             mac_encryptor = AES.new(k_str, AES.MODE_CBC, mac_bytes)
             iv_str = a32_to_str([iv[0], iv[1], iv[0], iv[1]])
             for chunk_start, chunk_size in get_chunks(tsize):
                 chunk = input_file.read(chunk_size)
                 chunk = aes.decrypt(chunk)
                 temp_output_file.write(chunk)
+                self.display(stime, tsize, len(chunk), message, progress)
                 encryptor = AES.new(k_str, AES.MODE_CBC, iv_str)
         
                 modchunk = len(chunk) % 16
                 if modchunk == 0:
                     modchunk = 16
                     last_block = chunk[-modchunk:]
                 else:
                     last_block = chunk[-modchunk:] + (b'\0' * (16 - modchunk))
 
                 mv = memoryview(chunk)
                 rest_of_chunk = mv[:-modchunk]
                 encryptor.encrypt(rest_of_chunk)
                 input_to_mac = encryptor.encrypt(last_block)
                 mac_bytes = mac_encryptor.encrypt(input_to_mac)
-                dsize = os.stat(temp_output_file.name).st_size
-                self.display(stime, tsize, dsize, message, progress)
 
             file_mac = str_to_a32(mac_bytes)
             if (file_mac[0] ^ file_mac[1], file_mac[2] ^ file_mac[3]) != meta_mac:
                 raise ValueError('Mismatched mac')
         
             output_name = temp_output_file.name
             temp_output_file.close()
```

### Comparing `megaxdl-0.0.4/PKG-INFO` & `megaxdl-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.4
+Version: 0.0.5
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
```

### Comparing `megaxdl-0.0.4/README.md` & `megaxdl-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.4/megaxdl.egg-info/PKG-INFO` & `megaxdl-0.0.5/megaxdl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.4
+Version: 0.0.5
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
```

### Comparing `megaxdl-0.0.4/setup.py` & `megaxdl-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 
 install = ["tqdm>=4.64.1",
            "tenacity>=8.2.2",
            "requests>=2.27.1",
            "pycryptodome>=3.20.0,<4.0.0"]
 
 setup(name='megaxdl',
-      version='0.0.4',
+      version='0.0.5',
       python_requires='~=3.10',
       packages=find_packages(),
       long_description=readme,
       install_requires=install,
       include_package_data=True,
       long_description_content_type='text/markdown')
```

