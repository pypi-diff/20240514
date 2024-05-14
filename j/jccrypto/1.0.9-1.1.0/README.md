# Comparing `tmp/jccrypto-1.0.9-py3-none-any.whl.zip` & `tmp/jccrypto-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2960 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     2686 b- defN 24-May-14 13:39 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     2797 b- defN 24-May-14 13:41 jccrypto-1.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 13:41 jccrypto-1.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 13:41 jccrypto-1.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-14 13:41 jccrypto-1.0.9.dist-info/RECORD
-5 files, 5962 bytes uncompressed, 2254 bytes compressed:  62.2%
+Zip file size: 3727 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     2686 b- defN 24-May-14 14:41 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     4387 b- defN 24-May-14 14:41 jccrypto-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 14:41 jccrypto-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 14:41 jccrypto-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-14 14:41 jccrypto-1.1.0.dist-info/RECORD
+5 files, 7552 bytes uncompressed, 3021 bytes compressed:  60.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.0.9.dist-info/METADATA
+Filename: jccrypto-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.0.9.dist-info/WHEEL
+Filename: jccrypto-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.0.9.dist-info/top_level.txt
+Filename: jccrypto-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.0.9.dist-info/RECORD
+Filename: jccrypto-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jccrypto/__init__.py

```diff
@@ -2,15 +2,15 @@
 from Crypto.Cipher import AES
 import base64
 import hashlib
 import pickle
 
 __package_name__ = 'pycrypto'
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.0.9'
+__version__      = '1.1.0'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
 __all__ = ['JcCrypto']
 
 def JcCryptoFromString(str):
```

