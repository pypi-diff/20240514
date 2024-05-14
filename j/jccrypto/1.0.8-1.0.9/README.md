# Comparing `tmp/jccrypto-1.0.8-py3-none-any.whl.zip` & `tmp/jccrypto-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2826 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     2479 b- defN 24-May-14 13:14 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     2583 b- defN 24-May-14 13:14 jccrypto-1.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 13:14 jccrypto-1.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 13:14 jccrypto-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-14 13:14 jccrypto-1.0.8.dist-info/RECORD
-5 files, 5541 bytes uncompressed, 2120 bytes compressed:  61.7%
+Zip file size: 2960 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     2686 b- defN 24-May-14 13:39 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     2797 b- defN 24-May-14 13:41 jccrypto-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 13:41 jccrypto-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 13:41 jccrypto-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-14 13:41 jccrypto-1.0.9.dist-info/RECORD
+5 files, 5962 bytes uncompressed, 2254 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.0.8.dist-info/METADATA
+Filename: jccrypto-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.0.8.dist-info/WHEEL
+Filename: jccrypto-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.0.8.dist-info/top_level.txt
+Filename: jccrypto-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.0.8.dist-info/RECORD
+Filename: jccrypto-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jccrypto/__init__.py

```diff
@@ -1,21 +1,29 @@
 # pip install PyCryptoDome
 from Crypto.Cipher import AES
 import base64
+import hashlib
 import pickle
 
 __package_name__ = 'pycrypto'
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.0.8'
+__version__      = '1.0.9'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
 __all__ = ['JcCrypto']
 
+def JcCryptoFromString(str):
+    sha256 = hashlib.sha256(str.encode())
+    digets = sha256.digest()
+    upper16 = digets[0:16]
+    lower16 = digets[16:]
+    return JcCrypto(upper16, lower16)
+
 class JcCrypto:
     def __init__(self, key, iv):
         self.cipher = AES.new(key, AES.MODE_CBC, iv)
         self.decipher = AES.new(key, AES.MODE_CBC, iv)
     def encode_text(self, plain_text):
         data = plain_text.encode()
         block_size = AES.block_size
```

## Comparing `jccrypto-1.0.8.dist-info/METADATA` & `jccrypto-1.0.9.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jccrypto
-Version: 1.0.8
+Version: 1.0.9
 Summary: Simple crypto library
 Home-page: https://github.com/lang-library/py-jccrypto
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
    せめて、英文テキストとかいう条件がわかっていればある程度は可能ですけど、総当たりですからファイルサイズと計算速度次第ってことになります。
    これが公開鍵暗号なら、暗号化キーから数学的に（膨大なCPU時間をかければ）複合化キーを計算することができますけどね。
 ```
 
 ## Sample code
 
 ```
-from jccrypto import JcCrypto
+from jccrypto import JcCrypto, JcCryptoFromString
 
 text = "Pythonの暗号化ライブラリとそれらの概要を表にまとめました。非常にたくさんのライブラリがあることがわかりました。それぞれのライブラリが得手不得手を持っているためユースケースに応じて適切なライブラリを使用する必要があります。"
 
 # 鍵の生成
 key = 'abcdefghijklmnop'.encode()
 # IVの生成
 iv = '1234567890123456'.encode()
@@ -66,8 +66,15 @@
 print("text2={}".format(text2))
 
 print("")
 list = [11, 22, 33]
 encoded = cr.encode_pickle(list)
 decoded = cr.decode_pickle(encoded)
 print("decoded={}".format(decoded))
+
+print("")
+cr2 = JcCryptoFromString("this is password!")
+list = [111, 222, 333]
+encoded = cr2.encode_pickle(list)
+decoded = cr2.decode_pickle(encoded)
+print("decoded={}".format(decoded))
 ```
```

