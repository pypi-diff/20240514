# Comparing `tmp/jccrypto-1.0.7-py3-none-any.whl.zip` & `tmp/jccrypto-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2411 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     2479 b- defN 24-May-14 12:31 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     1746 b- defN 24-May-14 12:31 jccrypto-1.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 12:31 jccrypto-1.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 12:31 jccrypto-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-14 12:31 jccrypto-1.0.7.dist-info/RECORD
-5 files, 4704 bytes uncompressed, 1705 bytes compressed:  63.8%
+Zip file size: 2826 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     2479 b- defN 24-May-14 13:14 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     2583 b- defN 24-May-14 13:14 jccrypto-1.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 13:14 jccrypto-1.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 13:14 jccrypto-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-14 13:14 jccrypto-1.0.8.dist-info/RECORD
+5 files, 5541 bytes uncompressed, 2120 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.0.7.dist-info/METADATA
+Filename: jccrypto-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.0.7.dist-info/WHEEL
+Filename: jccrypto-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.0.7.dist-info/top_level.txt
+Filename: jccrypto-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.0.7.dist-info/RECORD
+Filename: jccrypto-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jccrypto/__init__.py

```diff
@@ -1,15 +1,15 @@
 # pip install PyCryptoDome
 from Crypto.Cipher import AES
 import base64
 import pickle
 
 __package_name__ = 'pycrypto'
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.0.7'
+__version__      = '1.0.8'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
 __all__ = ['JcCrypto']
 
 class JcCrypto:
```

