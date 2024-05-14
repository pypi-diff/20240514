# Comparing `tmp/jccrypto-1.0.3-py3-none-any.whl.zip` & `tmp/jccrypto-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2203 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1199 b- defN 24-May-14 06:21 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     1254 b- defN 24-May-14 06:22 jccrypto-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 06:22 jccrypto-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 06:22 jccrypto-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-14 06:22 jccrypto-1.0.3.dist-info/RECORD
-5 files, 2932 bytes uncompressed, 1497 bytes compressed:  48.9%
+Zip file size: 2250 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1209 b- defN 24-May-14 09:35 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 24-May-14 09:35 jccrypto-1.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 09:35 jccrypto-1.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 09:35 jccrypto-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-14 09:35 jccrypto-1.0.4.dist-info/RECORD
+5 files, 3033 bytes uncompressed, 1544 bytes compressed:  49.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.0.3.dist-info/METADATA
+Filename: jccrypto-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.0.3.dist-info/WHEEL
+Filename: jccrypto-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.0.3.dist-info/top_level.txt
+Filename: jccrypto-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.0.3.dist-info/RECORD
+Filename: jccrypto-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jccrypto/__init__.py

```diff
@@ -1,30 +1,30 @@
 # pip install PyCryptoDome
 from Crypto.Cipher import AES
 import base64
 
 __package_name__ = 'pycrypto'
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.0.3'
+__version__      = '1.0.4'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
 __all__ = ['JcCrypto']
 
 class JcCrypto:
     def __init__(self, key, iv):
         self.cipher = AES.new(key, AES.MODE_CBC, iv)
         self.decipher = AES.new(key, AES.MODE_CBC, iv)
-    def encode(self, plain_text):
+    def encode_text(self, plain_text):
         data = plain_text.encode()
         block_size = AES.block_size
         padding_size = block_size - (len(data) % block_size)
         padded_data = data + bytes([padding_size]) * padding_size
         encrypted_data = self.cipher.encrypt(padded_data)
         return base64.b64encode(encrypted_data).decode()
-    def decode(self, base64_text):
+    def decode_text(self, base64_text):
         encrypted_data = base64.b64decode(base64_text.encode())
         decrypted_data = self.decipher.decrypt(encrypted_data)
         padding_size = decrypted_data[-1]
         unpadded_data = decrypted_data[:-padding_size]
         return unpadded_data.decode()
```

## Comparing `jccrypto-1.0.3.dist-info/METADATA` & `jccrypto-1.0.4.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jccrypto
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple crypto library
 Home-page: https://github.com/lang-library/py-jccrypto
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -36,35 +36,39 @@
 
 
 
 text = "Pythonの暗号化ライブラリとそれらの概要を表にまとめました。非常にたくさんのライブラリがあることがわかりました。それぞれのライブラリが得手不得手を持っているためユースケースに応じて適切なライブラリを使用する必要があります。"
 
 
 
-key = 'abcdefghijklmnop'.encode()
+# 鍵の生成
 
+key = 'abcdefghijklmnop'.encode() # get_random_bytes(16)
 
 
-iv = '1234567890123456'.encode()
+
+# IVの生成
+
+iv = '1234567890123456'.encode() # get_random_bytes(16)
 
 
 
 cr = JcCrypto(key, iv)
 
 
 
-encoded = cr.encode(text)
+encoded = cr.encode_text(text)
 
 
 
 print(encoded)
 
 
 
-decoded = cr.decode(encoded)
+decoded = cr.decode_text(encoded)
 
 
 
 print(decoded)
 
 ```
```

