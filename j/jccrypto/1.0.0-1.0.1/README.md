# Comparing `tmp/jccrypto-1.0.0-py3-none-any.whl.zip` & `tmp/jccrypto-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1871 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1199 b- defN 24-May-14 05:21 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat      578 b- defN 24-May-14 05:23 jccrypto-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 05:23 jccrypto-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 05:23 jccrypto-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      377 b- defN 24-May-14 05:23 jccrypto-1.0.0.dist-info/RECORD
-5 files, 2255 bytes uncompressed, 1165 bytes compressed:  48.3%
+Zip file size: 2224 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1199 b- defN 24-May-14 05:51 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     1272 b- defN 24-May-14 05:51 jccrypto-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 05:51 jccrypto-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 05:51 jccrypto-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-14 05:51 jccrypto-1.0.1.dist-info/RECORD
+5 files, 2950 bytes uncompressed, 1518 bytes compressed:  48.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.0.0.dist-info/METADATA
+Filename: jccrypto-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.0.0.dist-info/WHEEL
+Filename: jccrypto-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.0.0.dist-info/top_level.txt
+Filename: jccrypto-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.0.0.dist-info/RECORD
+Filename: jccrypto-1.0.1.dist-info/RECORD
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
-__version__      = '1.0.0'
+__version__      = '1.0.1'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
 __all__ = ['JcCrypto']
 
 class JcCrypto:
```
