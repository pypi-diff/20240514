# Comparing `tmp/megaxdl-0.0.1.tar.gz` & `tmp/megaxdl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megaxdl-0.0.1.tar", last modified: Tue May 14 07:31:05 2024, max compression
+gzip compressed data, was "megaxdl-0.0.2.tar", last modified: Tue May 14 10:42:26 2024, max compression
```

## Comparing `megaxdl-0.0.1.tar` & `megaxdl-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:31:05.129821 megaxdl-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 07:31:00.000000 megaxdl-0.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:31:05.125821 megaxdl-0.0.1/Megaxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 07:31:00.000000 megaxdl-0.0.1/Megaxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 07:31:00.000000 megaxdl-0.0.1/Megaxdl/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 07:31:00.000000 megaxdl-0.0.1/Megaxdl/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    40138 2024-05-14 07:31:00.000000 megaxdl-0.0.1/Megaxdl/mega.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-14 07:31:05.129821 megaxdl-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-14 07:31:00.000000 megaxdl-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:31:05.129821 megaxdl-0.0.1/megaxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-14 07:31:05.000000 megaxdl-0.0.1/megaxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 07:31:05.000000 megaxdl-0.0.1/megaxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:31:05.000000 megaxdl-0.0.1/megaxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 07:31:05.000000 megaxdl-0.0.1/megaxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 07:31:05.000000 megaxdl-0.0.1/megaxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:31:05.129821 megaxdl-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 07:31:00.000000 megaxdl-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:42:26.084700 megaxdl-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 10:42:19.000000 megaxdl-0.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:42:26.080700 megaxdl-0.0.2/Megaxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 10:42:19.000000 megaxdl-0.0.2/Megaxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 10:42:19.000000 megaxdl-0.0.2/Megaxdl/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 10:42:19.000000 megaxdl-0.0.2/Megaxdl/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38446 2024-05-14 10:42:19.000000 megaxdl-0.0.2/Megaxdl/mega.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 10:42:26.084700 megaxdl-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 10:42:19.000000 megaxdl-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:42:26.084700 megaxdl-0.0.2/megaxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-14 10:42:26.000000 megaxdl-0.0.2/megaxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 10:42:26.000000 megaxdl-0.0.2/megaxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:42:26.000000 megaxdl-0.0.2/megaxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 10:42:26.000000 megaxdl-0.0.2/megaxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 10:42:26.000000 megaxdl-0.0.2/megaxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:42:26.084700 megaxdl-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 10:42:19.000000 megaxdl-0.0.2/setup.py
```

### Comparing `megaxdl-0.0.1/LICENSE` & `megaxdl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.1/Megaxdl/crypto.py` & `megaxdl-0.0.2/Megaxdl/crypto.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.1/Megaxdl/errors.py` & `megaxdl-0.0.2/Megaxdl/errors.py`

 * *Files identical despite different names*

### Comparing `megaxdl-0.0.1/Megaxdl/mega.py` & `megaxdl-0.0.2/Megaxdl/mega.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,36 @@
 from .crypto import encrypt_attr, base64_to_a32, base64_url_decode
 from .crypto import decrypt_attr, a32_to_str, get_chunks, str_to_a32
 from tenacity import retry, wait_exponential, retry_if_exception_type
 
 logger = logging.getLogger(__name__)
 
 class Mega:
+
     def __init__(self, options=None):
+        self.sid = None
+        self.timeout = 160
         self.schema = 'https'
         self.domain = 'mega.nz'
-        self.api_domain = 'mega.co.nz'  # g.api.mega.nz doesn't exist, have to use the old domain name for api access
-        self.timeout = 160  # max secs to wait for resp from api requests
-        self.sid = None
-        self.sequence_num = random.randint(0, 0xFFFFFFFF)
         self.request_id = make_id(10)
+        self.api_domain = 'mega.co.nz'
         self._trash_folder_node_id = None
+        self.sequence_num = random.randint(0, 0xFFFFFFFF)
 
         if options is None:
             options = {}
         self.options = options
 
+    def display(self, stime, tsize, dsize, message, progress):
+        if message and progress:
+            progress(stime, tsize, dsize, message)
+        elif progress:
+            progress(stime, tsize, dsize)
+        else: pass
+        
     def login(self, email=None, password=None):
         if email:
             self._login_user(email, password)
         else:
             self.login_anonymous()
         self._trash_folder_node_id = self.get_node_by_type(4)[0]
         logger.info('Login complete')
@@ -137,16 +145,15 @@
 
             encrypted_sid = mpi_to_int(base64_url_decode(resp['csid']))
 
             sid = '%x' % rsa_decrypter._decrypt(encrypted_sid)
             sid = binascii.unhexlify('0' + sid if len(sid) % 2 else sid)
             self.sid = base64_url_encode(sid[:43])
 
-    @retry(retry=retry_if_exception_type(RuntimeError),
-           wait=wait_exponential(multiplier=2, min=2, max=60))
+    @retry(retry=retry_if_exception_type(RuntimeError), wait=wait_exponential(multiplier=2, min=2, max=60))
     def _api_request(self, data):
         params = {'id': self.sequence_num}
         self.sequence_num += 1
 
         if self.sid:
             params.update({'sid': self.sid})
 
@@ -565,32 +572,17 @@
         # make a list of json
         if files != {}:
             post_list = []
             for file in files:
                 post_list.append({"a": "d", "n": file, "i": self.request_id})
             return self._api_request(post_list)
 
-    def download(self, file, dest_path=None, dest_filename=None):
-        """
-        Download a file by it's file object
-        """
-        return self._download_file(file_handle=None,
-                                   file_key=None,
-                                   file=file[1],
-                                   dest_path=dest_path,
-                                   dest_filename=dest_filename,
-                                   is_public=False)
-
     def _export_file(self, node):
         node_data = self._node_data(node)
-        self._api_request([{
-            'a': 'l',
-            'n': node_data['h'],
-            'i': self.request_id
-        }])
+        self._api_request( [ {'a': 'l', 'n': node_data['h'], 'i': self.request_id } ] )
         return self.get_link(node)
 
     def export(self, path=None, node_id=None):
         nodes = self.get_files()
         if node_id:
             node = nodes[node_id]
         else:
@@ -638,131 +630,92 @@
             ha,
             'cr': [[node_id], [node_id], [0, 0, encrypted_node_key]]
         }]
         self._api_request(request_body)
         nodes = self.get_files()
         return self.get_folder_link(nodes[node_id])
 
-    def download_url(self, url, dest_path=None, dest_filename=None, no_temp_file=False):
-        """
-        Download a file by it's public url
-        """
-        path = self._parse_url(url).split('!')
-        file_id = path[0]
-        file_key = path[1]
-        return self._download_file(
-            file_handle=file_id,
-            file_key=file_key,
-            dest_path=dest_path,
-            dest_filename=dest_filename,
-            is_public=True,
-            no_temp_file=no_temp_file
-        )
 
-    def _download_file(self,
-                       file_handle,
-                       file_key,
-                       dest_path=None,
-                       dest_filename=None,
-                       is_public=False,
-                       file=None,
-                       no_temp_file=False):
-        if file is None:
-            if is_public:
-                file_key = base64_to_a32(file_key)
-            file_data = self._api_request({
-                'a': 'g',
-                'g': 1,
-                'p' if is_public else 'n': file_handle
-            })
+    def download(self, file, dest_path=None, dest_filename=None):
+        return self.sdownload(file_uid=None, file_key=None, file=file[1], message=None, progress=None, is_public=False, dest_path=dest_path, dest_filename=dest_filename)
+
+
+    def download_url(self, url, message=None, progress=None, dest_path=None, dest_filename=None, no_temp_file=False):
+        path_mid = self._parse_url(url).split('!')
+        file_uid = path_mid[0]
+        file_key = path_mid[1]
+        return self.sdownload(file_uid, file_key, message=None, progress=None, is_public=True, dest_path=dest_path, dest_filename=dest_filename, no_temp_file=no_temp_file)
+
+
+    def sdownload(self, file_uid, file_key, file=None, message=None, progress=None, dest_path=None, dest_filename=None, is_public=False, no_temp_file=False):
 
-            k = (file_key[0] ^ file_key[4], file_key[1] ^ file_key[5],
-                 file_key[2] ^ file_key[6], file_key[3] ^ file_key[7])
+        stime = time.time()
+        if file == None:
+            file_key = base64_to_a32(file_key) if is_public else file_key
+            file_data = self._api_request({'a': 'g', 'g': 1, 'p' if is_public else 'n': file_uid})
+            k = (file_key[0] ^ file_key[4], file_key[1] ^ file_key[5], file_key[2] ^ file_key[6], file_key[3] ^ file_key[7])
             iv = file_key[4:6] + (0, 0)
             meta_mac = file_key[6:8]
         else:
             file_data = self._api_request({'a': 'g', 'g': 1, 'n': file['h']})
             k = file['k']
             iv = file['iv']
             meta_mac = file['meta_mac']
 
-        # Seems to happens sometime... When this occurs, files are
-        # inaccessible also in the official web app.
-        # Strangely, files can come back later.
         if 'g' not in file_data:
             raise RequestError('File not accessible anymore')
+
+        tsize = file_data['s']
         file_url = file_data['g']
-        file_size = file_data['s']
         attribs = base64_url_decode(file_data['at'])
         attribs = decrypt_attr(attribs, k)
-
-        if dest_filename is not None:
-            file_name = dest_filename
-        else:
-            file_name = attribs['n']
-
+        file_name = dest_filename if dest_filename is not None else attribs['n']
         input_file = requests.get(file_url, stream=True).raw
+        dest_patho = '' if dest_path is None else dest_path + '/'
+        
+        output_path = Path(dest_patho + file_name)
+        with (tempfile.NamedTemporaryFile(mode='w+b', prefix='megapy_', delete=False) if not no_temp_file else open(output_path, 'xb')) as temp_output_file:
+            k_str = a32_to_str(k)
+            counter = Counter.new(128, initial_value=((iv[0] << 32) + iv[1]) << 64)
+            aes = AES.new(k_str, AES.MODE_CTR, counter=counter)
+            mac_bytes = b'\0' * 16
+            mac_encryptor = AES.new(k_str, AES.MODE_CBC, mac_bytes)
+            iv_str = a32_to_str([iv[0], iv[1], iv[0], iv[1]])
+            for chunk_start, chunk_size in get_chunks(tsize):
+                chunk = input_file.read(chunk_size)
+                chunk = aes.decrypt(chunk)
+                temp_output_file.write(chunk)
+                encryptor = AES.new(k_str, AES.MODE_CBC, iv_str)
+        
+                modchunk = len(chunk) % 16
+                if modchunk == 0:
+                    modchunk = 16
+                    last_block = chunk[-modchunk:]
+                else:
+                    last_block = chunk[-modchunk:] + (b'\0' * (16 - modchunk))
 
-        if dest_path is None:
-            dest_path = ''
-        else:
-            dest_path += '/'
-        output_path = Path(dest_path + file_name)
+                mv = memoryview(chunk)
+                rest_of_chunk = mv[:-modchunk]
+                encryptor.encrypt(rest_of_chunk)
+                input_to_mac = encryptor.encrypt(last_block)
+                mac_bytes = mac_encryptor.encrypt(input_to_mac)
+                dsize = os.stat(temp_output_file.name).st_size
+                self.display(stime, tsize, dsize, message, progress)
+
+            file_mac = str_to_a32(mac_bytes)
+            if (file_mac[0] ^ file_mac[1], file_mac[2] ^ file_mac[3]) != meta_mac:
+                raise ValueError('Mismatched mac')
+        
+            output_name = temp_output_file.name
+            temp_output_file.close()
+            if not no_temp_file:
+                print('Moving temporary file to destination path')
+                shutil.move(output_name, output_path)
 
-        with (tempfile.NamedTemporaryFile(mode='w+b',
-                                         prefix='megapy_',
-                                         delete=False) if not no_temp_file else open(output_path, 'xb')) as temp_output_file:
-            with tqdm.tqdm(total=file_size, unit='iB', unit_scale=True) as progress_bar:
-                k_str = a32_to_str(k)
-                counter = Counter.new(128,
-                                      initial_value=((iv[0] << 32) + iv[1]) << 64)
-                aes = AES.new(k_str, AES.MODE_CTR, counter=counter)
-
-                # mega.nz improperly uses CBC as a MAC mode, so after each chunk, the computed mac_bytes are used as IV for the next chunk MAC accumulation
-                mac_bytes = b'\0' * 16
-                mac_encryptor = AES.new(k_str, AES.MODE_CBC, mac_bytes)
-                iv_str = a32_to_str([iv[0], iv[1], iv[0], iv[1]])
-
-                for chunk_start, chunk_size in get_chunks(file_size):
-                    # print('Chunk size from generator: '+chunk_size)
-                    chunk = input_file.read(chunk_size)
-                    chunk = aes.decrypt(chunk)
-                    temp_output_file.write(chunk)
-                    progress_bar.update(len(chunk))
-
-                    encryptor = AES.new(k_str, AES.MODE_CBC, iv_str)
-
-                    # take last 16-N bytes from chunk (with N between 1 and 16, including extremes)
-                    mv = memoryview(chunk) # avoid copying memory for the entire chunk when slicing
-                    modchunk = len(chunk) % 16
-                    if modchunk == 0:
-                        # ensure we reserve the last 16 bytes anyway, we have to feed them into mac_encryptor
-                        modchunk = 16
-                        last_block = chunk[-modchunk:] # fine to copy bytes here, they're only a few bytes
-                    else:
-                        last_block = chunk[-modchunk:] + (b'\0' * (16 - modchunk)) # pad last block to 16 bytes
-                    rest_of_chunk = mv[:-modchunk]
-
-                    encryptor.encrypt(rest_of_chunk)
-                    input_to_mac = encryptor.encrypt(last_block)
-                    mac_bytes = mac_encryptor.encrypt(input_to_mac)
-
-                    # file_info = os.stat(temp_output_file.name)
-                    # logger.info('%s of %s downloaded', file_info.st_size,
-                    #             file_size)
-                file_mac = str_to_a32(mac_bytes)
-                # check mac integrity
-                if (file_mac[0] ^ file_mac[1],
-                        file_mac[2] ^ file_mac[3]) != meta_mac:
-                    raise ValueError('Mismatched mac')
-                output_name = temp_output_file.name
-        if not no_temp_file:
-            print('Moving temporary file to destination path')
-            shutil.move(output_name, output_path)
-        return output_path
+            return output_path
 
     def upload(self, filename, dest=None, dest_filename=None):
         # determine storage node
         if dest is None:
             # if none set, upload to cloud drive node
             if not hasattr(self, 'root_id'):
                 self.get_files()
```

### Comparing `megaxdl-0.0.1/PKG-INFO` & `megaxdl-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,53 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.1
+Version: 0.0.2
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
 
-Mega.py
+Megaxdl
 =======
 
 Python library for the [Mega.nz](https://mega.nz)
 API, currently supporting:
 
 -   login
--   uploading
--   downloading
--   deleting
--   searching
 -   sharing
 -   renaming
+-   deleting
+-   searching
+-   uploading
+-   downloading
 -   moving files
 
-This is a work in progress, further functionality coming shortly.
-
-For more detailed information see API\_INFO.md
-
 How To Use
 ----------
 
 ### Create a Mega account
 
 For downloading links, no account is needed. To use upload capabilities, [create an account with Mega](https://mega.nz) .
 
-### Install mega.py package
-
-Clone the repository, and then run:
+### Install megaxdl package
 
 ```sh
-cd mega.py
-pip install .
+pip install megaxdl
 ```
 
-### Import mega.py
+### Import Mega
 
 ```python
-from mega import Mega
+from Megaxdl import Mega
 ```
 
-### Create an instance of Mega.py
+### Create an instance of Mega
 
 ```python
 mega = Mega()
 ```
 
 ### Login to Mega
```

### Comparing `megaxdl-0.0.1/README.md` & `megaxdl-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,42 @@
-Mega.py
+Megaxdl
 =======
 
 Python library for the [Mega.nz](https://mega.nz)
 API, currently supporting:
 
 -   login
--   uploading
--   downloading
--   deleting
--   searching
 -   sharing
 -   renaming
+-   deleting
+-   searching
+-   uploading
+-   downloading
 -   moving files
 
-This is a work in progress, further functionality coming shortly.
-
-For more detailed information see API\_INFO.md
-
 How To Use
 ----------
 
 ### Create a Mega account
 
 For downloading links, no account is needed. To use upload capabilities, [create an account with Mega](https://mega.nz) .
 
-### Install mega.py package
-
-Clone the repository, and then run:
+### Install megaxdl package
 
 ```sh
-cd mega.py
-pip install .
+pip install megaxdl
 ```
 
-### Import mega.py
+### Import Mega
 
 ```python
-from mega import Mega
+from Megaxdl import Mega
 ```
 
-### Create an instance of Mega.py
+### Create an instance of Mega
 
 ```python
 mega = Mega()
 ```
 
 ### Login to Mega
```

### Comparing `megaxdl-0.0.1/megaxdl.egg-info/PKG-INFO` & `megaxdl-0.0.2/megaxdl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,53 @@
 Metadata-Version: 2.1
 Name: megaxdl
-Version: 0.0.1
+Version: 0.0.2
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: pycryptodome<4.0.0,>=3.20.0
 
-Mega.py
+Megaxdl
 =======
 
 Python library for the [Mega.nz](https://mega.nz)
 API, currently supporting:
 
 -   login
--   uploading
--   downloading
--   deleting
--   searching
 -   sharing
 -   renaming
+-   deleting
+-   searching
+-   uploading
+-   downloading
 -   moving files
 
-This is a work in progress, further functionality coming shortly.
-
-For more detailed information see API\_INFO.md
-
 How To Use
 ----------
 
 ### Create a Mega account
 
 For downloading links, no account is needed. To use upload capabilities, [create an account with Mega](https://mega.nz) .
 
-### Install mega.py package
-
-Clone the repository, and then run:
+### Install megaxdl package
 
 ```sh
-cd mega.py
-pip install .
+pip install megaxdl
 ```
 
-### Import mega.py
+### Import Mega
 
 ```python
-from mega import Mega
+from Megaxdl import Mega
 ```
 
-### Create an instance of Mega.py
+### Create an instance of Mega
 
 ```python
 mega = Mega()
 ```
 
 ### Login to Mega
```

### Comparing `megaxdl-0.0.1/setup.py` & `megaxdl-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 
 install = ["tqdm>=4.64.1",
            "tenacity>=8.2.2",
            "requests>=2.27.1",
            "pycryptodome>=3.20.0,<4.0.0"]
 
 setup(name='megaxdl',
-      version='0.0.1',
+      version='0.0.2',
       python_requires='~=3.10',
       packages=find_packages(),
       long_description=readme,
       install_requires=install,
       include_package_data=True,
       long_description_content_type='text/markdown')
```

