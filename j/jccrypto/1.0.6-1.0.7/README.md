# Comparing `tmp/jccrypto-1.0.6-py3-none-any.whl.zip` & `tmp/jccrypto-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2326 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1815 b- defN 24-May-14 10:17 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     1604 b- defN 24-May-14 10:17 jccrypto-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 10:17 jccrypto-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 10:17 jccrypto-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-14 10:17 jccrypto-1.0.6.dist-info/RECORD
-5 files, 3898 bytes uncompressed, 1620 bytes compressed:  58.4%
+Zip file size: 2411 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     2479 b- defN 24-May-14 12:31 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     1746 b- defN 24-May-14 12:31 jccrypto-1.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 12:31 jccrypto-1.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 12:31 jccrypto-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-14 12:31 jccrypto-1.0.7.dist-info/RECORD
+5 files, 4704 bytes uncompressed, 1705 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.0.6.dist-info/METADATA
+Filename: jccrypto-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.0.6.dist-info/WHEEL
+Filename: jccrypto-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.0.6.dist-info/top_level.txt
+Filename: jccrypto-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.0.6.dist-info/RECORD
+Filename: jccrypto-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jccrypto/__init__.py

```diff
@@ -1,14 +1,15 @@
 # pip install PyCryptoDome
 from Crypto.Cipher import AES
 import base64
+import pickle
 
 __package_name__ = 'pycrypto'
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.0.6'
+__version__      = '1.0.7'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
 __all__ = ['JcCrypto']
 
 class JcCrypto:
@@ -36,7 +37,20 @@
         return base64.b64encode(encrypted_data).decode()
     def decode_bytes(self, base64_text):
         encrypted_data = base64.b64decode(base64_text.encode())
         decrypted_data = self.decipher.decrypt(encrypted_data)
         padding_size = decrypted_data[-1]
         unpadded_data = decrypted_data[:-padding_size]
         return unpadded_data
+    def encode_pickle(self, x):
+        data = pickle.dumps(x)
+        block_size = AES.block_size
+        padding_size = block_size - (len(data) % block_size)
+        padded_data = data + bytes([padding_size]) * padding_size
+        encrypted_data = self.cipher.encrypt(padded_data)
+        return base64.b64encode(encrypted_data).decode()
+    def decode_pickle(self, base64_text):
+        encrypted_data = base64.b64decode(base64_text.encode())
+        decrypted_data = self.decipher.decrypt(encrypted_data)
+        padding_size = decrypted_data[-1]
+        unpadded_data = decrypted_data[:-padding_size]
+        return pickle.loads(unpadded_data)
```

## Comparing `jccrypto-1.0.6.dist-info/METADATA` & `jccrypto-1.0.7.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jccrypto
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple crypto library
 Home-page: https://github.com/lang-library/py-jccrypto
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -49,8 +49,14 @@
 print("encoded={}".format(encoded))
 decoded = cr.decode_bytes(encoded)
 print("decoded={}".format(decoded))
 
 print("")
 text2 = decoded.decode()
 print("text2={}".format(text2))
+
+print("")
+list = [11, 22, 33]
+encoded = cr.encode_pickle(list)
+decoded = cr.decode_pickle(encoded)
+print("decoded={}".format(decoded))
 ```
```

