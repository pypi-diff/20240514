# Comparing `tmp/jccrypto-1.0.2-py3-none-any.whl.zip` & `tmp/jccrypto-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2208 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1199 b- defN 24-May-14 06:19 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     1259 b- defN 24-May-14 06:20 jccrypto-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 06:20 jccrypto-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 06:20 jccrypto-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-14 06:20 jccrypto-1.0.2.dist-info/RECORD
-5 files, 2937 bytes uncompressed, 1502 bytes compressed:  48.9%
+Zip file size: 2203 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1199 b- defN 24-May-14 06:21 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     1254 b- defN 24-May-14 06:22 jccrypto-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 06:22 jccrypto-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 06:22 jccrypto-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-14 06:22 jccrypto-1.0.3.dist-info/RECORD
+5 files, 2932 bytes uncompressed, 1497 bytes compressed:  48.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.0.2.dist-info/METADATA
+Filename: jccrypto-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.0.2.dist-info/WHEEL
+Filename: jccrypto-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.0.2.dist-info/top_level.txt
+Filename: jccrypto-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.0.2.dist-info/RECORD
+Filename: jccrypto-1.0.3.dist-info/RECORD
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
-__version__      = '1.0.2'
+__version__      = '1.0.3'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
 __all__ = ['JcCrypto']
 
 class JcCrypto:
```

## Comparing `jccrypto-1.0.2.dist-info/METADATA` & `jccrypto-1.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jccrypto
-Version: 1.0.2
-Summary: ('Simple crypto library',)
+Version: 1.0.3
+Summary: Simple crypto library
 Home-page: https://github.com/lang-library/py-jccrypto
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

