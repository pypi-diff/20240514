# Comparing `tmp/jccrypto-1.1.0-py3-none-any.whl.zip` & `tmp/jccrypto-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3727 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     2686 b- defN 24-May-14 14:41 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     4387 b- defN 24-May-14 14:41 jccrypto-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 14:41 jccrypto-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 14:41 jccrypto-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-14 14:41 jccrypto-1.1.0.dist-info/RECORD
-5 files, 7552 bytes uncompressed, 3021 bytes compressed:  60.0%
+Zip file size: 4388 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     2686 b- defN 24-May-14 20:57 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     5965 b- defN 24-May-14 20:57 jccrypto-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 20:57 jccrypto-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 20:57 jccrypto-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-14 20:57 jccrypto-1.1.1.dist-info/RECORD
+5 files, 9130 bytes uncompressed, 3682 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.1.0.dist-info/METADATA
+Filename: jccrypto-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.1.0.dist-info/WHEEL
+Filename: jccrypto-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.1.0.dist-info/top_level.txt
+Filename: jccrypto-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.1.0.dist-info/RECORD
+Filename: jccrypto-1.1.1.dist-info/RECORD
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
-__version__      = '1.1.0'
+__version__      = '1.1.1'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
 __all__ = ['JcCrypto']
 
 def JcCryptoFromString(str):
```

## Comparing `jccrypto-1.1.0.dist-info/METADATA` & `jccrypto-1.1.1.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jccrypto
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simple crypto library
 Home-page: https://github.com/lang-library/py-jccrypto
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -43,14 +43,53 @@
     100 億人の人が、
     毎ナノ秒 1 兆個の数値を消費していく活動があり、
     その活動を、太陽系が属するこの銀河系の全ての星（～2,000 億くらい）でおこなうと、
 
 消費される数字の個数は、50 億年 × 100 億人 × 100000000 ナノ秒 × 60 秒 × 60 分 × 24 時間 × 365 日 × 1 兆個 × 2000 億個(星) で 59 桁の数字になります。こんなに頑張って消費しても、50 億年後 (太陽が赤色巨星になって太陽系が崩壊する頃) に消費し終わっているのは、(59 桁) / (78 桁) = 10^-19、つまり全体の 100 京分の 1 です。
 ```
 
+```
+----
+
+# 鍵の生成
+key = 'abcdefghijklmnop'.encode()
+# IVの生成
+iv = '1234567890123456'.encode()
+# 鍵とIVで暗号化クラスオオブジェクト生成
+cr = JcCrypto(key, iv)
+
+↑こんな適当な鍵とIVでは推測されてしまう可能性もありますが・・・
+
+----
+
+# 任意の文字列から暗号化クラスオブジェクトを作る方法
+cr2 = JcCryptoFromString("Python")
+
+①「Python」のSHA256(32bytes=256bit)を求める ⇒ 18885f27b5af9012df19e496460f9294d5ab76128824c6f993787004f6d9a7db
+②上下16bytes(16進数32桁)ずつに分割
+   upper = 18885f27b5af9012df19e496460f9294
+   lower = d5ab76128824c6f993787004f6d9a7db
+③ upper を鍵, lower をIVとして暗号化クラスオブジェクトを作成
+   return JcCrypto(upper, lower)
+
+----
+
+↑の「任意の文字列から暗号化クラスオブジェクトを作る方法」を使うととても強力です。(ただし「Python」を推測されたらアウト)
+
+そこで、パスワード生成 https://www.graviness.com/app/pwg/ で以下のようなランダムなパスワードを生成して
+5{$HtT<M)}<$&*_yEp[]-3>n*5e&)G<J
+
+cr2 = JcCryptoFromString("5{$HtT<M)}<$&*_yEp[]-3>n*5e&)G<J")
+としてしまえば、SHA256は、463cf456a504a0a1fb331981d799f5fb4e58af867977e246d7cbf54a97546d34 となり
+十進数では、31769596586757812275155959797078663488097707046160970084875920216559577230644 (10進77桁) となります。
+このような鍵、IVを総当たりで求めることは「もはや不可能」です。
+
+----
+```
+
 ## Sample code
 
 ```
 from jccrypto import JcCrypto, JcCryptoFromString
 
 text = "Pythonの暗号化ライブラリとそれらの概要を表にまとめました。非常にたくさんのライブラリがあることがわかりました。それぞれのライブラリが得手不得手を持っているためユースケースに応じて適切なライブラリを使用する必要があります。"
```

