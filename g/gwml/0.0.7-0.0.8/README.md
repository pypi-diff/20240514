# Comparing `tmp/gwml-0.0.7-py3-none-any.whl.zip` & `tmp/gwml-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1860 bytes, number of entries: 7
--rw-r--r--  2.0 unx       22 b- defN 24-May-14 09:17 gwml/__init__.py
+Zip file size: 1858 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       22 b- defN 24-May-14 09:26 gwml/__init__.py
 -rw-r--r--  2.0 unx      125 b- defN 24-May-08 00:38 gwml/example.py
--rw-r--r--  2.0 unx       28 b- defN 24-May-14 09:17 gwml-0.0.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      645 b- defN 24-May-14 09:17 gwml-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 09:17 gwml-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-May-14 09:17 gwml-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      513 b- defN 24-May-14 09:17 gwml-0.0.7.dist-info/RECORD
-7 files, 1430 bytes uncompressed, 948 bytes compressed:  33.7%
+-rw-r--r--  2.0 unx       28 b- defN 24-May-14 09:26 gwml-0.0.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      645 b- defN 24-May-14 09:26 gwml-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 09:26 gwml-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-May-14 09:26 gwml-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      513 b- defN 24-May-14 09:26 gwml-0.0.8.dist-info/RECORD
+7 files, 1430 bytes uncompressed, 946 bytes compressed:  33.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: gwml/__init__.py
 Comment: 
 
 Filename: gwml/example.py
 Comment: 
 
-Filename: gwml-0.0.7.dist-info/LICENSE.txt
+Filename: gwml-0.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: gwml-0.0.7.dist-info/METADATA
+Filename: gwml-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: gwml-0.0.7.dist-info/WHEEL
+Filename: gwml-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: gwml-0.0.7.dist-info/top_level.txt
+Filename: gwml-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: gwml-0.0.7.dist-info/RECORD
+Filename: gwml-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gwml/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.7"
+__version__ = "0.0.8"
```

## Comparing `gwml-0.0.7.dist-info/METADATA` & `gwml-0.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwml
-Version: 0.0.7
+Version: 0.0.8
 Summary: PYPI tutorial package creation written by TeddyNote
 Home-page: https://weda.kr
 Author: weda
 Author-email: dmshin@weda.kr
 Keywords: gw,weda,greenwhales,ml,dl,automl
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `gwml-0.0.7.dist-info/RECORD` & `gwml-0.0.8.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-gwml/__init__.py,sha256=R9xOYoYrWKcfO5zvTeGC3m_eDNOvxMd8CocQs2tLufo,22
+gwml/__init__.py,sha256=wOJN3HxAgnSon5vWYU3Txm2UZ_7tBHDKXUKZIH-mXX8,22
 gwml/example.py,sha256=ihdQ7-XAqAfecNvWbi7-kC1CEQHHz8rYRRG4NqQnSTQ,125
-gwml-0.0.7.dist-info/LICENSE.txt,sha256=sMb1CD5yWhcP_5FiSdNEtgqQEXKD6UPiro-JzEAQa-A,28
-gwml-0.0.7.dist-info/METADATA,sha256=L-Ou5XMBUaYomCUVSVsRNPT_oKn1qwy_FquIP7HrbHA,645
-gwml-0.0.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-gwml-0.0.7.dist-info/top_level.txt,sha256=-Ib3RiOMqlhiZ_idfsP2Unxpw70_Lzk5xN0I7vWHuAQ,5
-gwml-0.0.7.dist-info/RECORD,,
+gwml-0.0.8.dist-info/LICENSE.txt,sha256=sMb1CD5yWhcP_5FiSdNEtgqQEXKD6UPiro-JzEAQa-A,28
+gwml-0.0.8.dist-info/METADATA,sha256=Wzap_zRV-5PYbdU_4KozCtFrkCwYzAmKagzazwawECk,645
+gwml-0.0.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+gwml-0.0.8.dist-info/top_level.txt,sha256=-Ib3RiOMqlhiZ_idfsP2Unxpw70_Lzk5xN0I7vWHuAQ,5
+gwml-0.0.8.dist-info/RECORD,,
```

