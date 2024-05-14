# Comparing `tmp/jccrypto-1.0.5-py3-none-any.whl.zip` & `tmp/jccrypto-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2336 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1815 b- defN 24-May-14 10:14 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     1684 b- defN 24-May-14 10:15 jccrypto-1.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 10:15 jccrypto-1.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 10:15 jccrypto-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-14 10:15 jccrypto-1.0.5.dist-info/RECORD
-5 files, 3978 bytes uncompressed, 1630 bytes compressed:  59.0%
+Zip file size: 2326 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1815 b- defN 24-May-14 10:17 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     1604 b- defN 24-May-14 10:17 jccrypto-1.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 10:17 jccrypto-1.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 10:17 jccrypto-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-14 10:17 jccrypto-1.0.6.dist-info/RECORD
+5 files, 3898 bytes uncompressed, 1620 bytes compressed:  58.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.0.5.dist-info/METADATA
+Filename: jccrypto-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.0.5.dist-info/WHEEL
+Filename: jccrypto-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.0.5.dist-info/top_level.txt
+Filename: jccrypto-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.0.5.dist-info/RECORD
+Filename: jccrypto-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jccrypto/__init__.py

```diff
@@ -1,14 +1,14 @@
 # pip install PyCryptoDome
 from Crypto.Cipher import AES
 import base64
 
 __package_name__ = 'pycrypto'
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.0.5'
+__version__      = '1.0.6'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
 __all__ = ['JcCrypto']
 
 class JcCrypto:
```

## Comparing `jccrypto-1.0.5.dist-info/METADATA` & `jccrypto-1.0.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jccrypto
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simple crypto library
 Home-page: https://github.com/lang-library/py-jccrypto
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,85 +12,45 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 Requires-Dist: PyCryptoDome
 
 # py-jccrypto
 
-
-
 ## To install
 
-
-
 pip install jccrypto
 
-
-
 ## Sample code
 
-
-
 ```
-
 from jccrypto import JcCrypto
 
-
-
 text = "Pythonの暗号化ライブラリとそれらの概要を表にまとめました。非常にたくさんのライブラリがあることがわかりました。それぞれのライブラリが得手不得手を持っているためユースケースに応じて適切なライブラリを使用する必要があります。"
 
-
-
 # 鍵の生成
-
 key = 'abcdefghijklmnop'.encode()
-
 # IVの生成
-
 iv = '1234567890123456'.encode()
 
-
-
 cr = JcCrypto(key, iv)
 
-
-
 print("")
-
 encoded = cr.encode_text(text)
-
 print("encoded={}".format(encoded))
-
 decoded = cr.decode_text(encoded)
-
 print("decoded={}".format(decoded))
 
-
-
 print("")
-
 text_bytes = text.encode()
-
 print("text_bytes={}".format(text_bytes))
 
-
-
 print("")
-
 encoded = cr.encode_bytes(text_bytes)
-
 print("encoded={}".format(encoded))
-
 decoded = cr.decode_bytes(encoded)
-
 print("decoded={}".format(decoded))
 
-
-
 print("")
-
 text2 = decoded.decode()
-
 print("text2={}".format(text2))
-
 ```
-
```

