# Comparing `tmp/asknews-0.6.1-py3-none-any.whl.zip` & `tmp/asknews-0.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -15,12 +15,12 @@
 -rw-r--r--  2.0 unx      588 b- defN 80-Jan-01 00:00 asknews_sdk/dto/sentiment.py
 -rw-r--r--  2.0 unx     6643 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
 -rw-r--r--  2.0 unx     1451 b- defN 80-Jan-01 00:00 asknews_sdk/errors.py
 -rw-r--r--  2.0 unx     6339 b- defN 80-Jan-01 00:00 asknews_sdk/sdk.py
 -rw-r--r--  2.0 unx     5396 b- defN 80-Jan-01 00:00 asknews_sdk/security.py
 -rw-r--r--  2.0 unx     1614 b- defN 80-Jan-01 00:00 asknews_sdk/utils.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 asknews_sdk/version.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3233 b- defN 80-Jan-01 00:00 asknews-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.6.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.6.1.dist-info/RECORD
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.6.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3233 b- defN 80-Jan-01 00:00 asknews-0.6.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.6.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.6.2.dist-info/RECORD
 24 files, 93825 bytes uncompressed, 20501 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: asknews_sdk/utils.py
 Comment: 
 
 Filename: asknews_sdk/version.py
 Comment: 
 
-Filename: asknews-0.6.1.dist-info/LICENSE
+Filename: asknews-0.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: asknews-0.6.1.dist-info/METADATA
+Filename: asknews-0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: asknews-0.6.1.dist-info/WHEEL
+Filename: asknews-0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: asknews-0.6.1.dist-info/RECORD
+Filename: asknews-0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `asknews-0.6.1.dist-info/LICENSE` & `asknews-0.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `asknews-0.6.1.dist-info/METADATA` & `asknews-0.6.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: asknews
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python SDK for AskNews
 Home-page: https://github.com/emergentmethods/asknews-python-sdk
 License: MIT
 Author: Emergent Methods
 Author-email: contact@emergentmethods.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asgiref (>=3.7.2,<4.0.0)
 Requires-Dist: authlib (>=1.3.0,<2.0.0)
-Requires-Dist: httpx (>=0.25.2,<0.26.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: orjson (>=3.9.10,<4.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Project-URL: Repository, https://github.com/emergentmethods/asknews-python-sdk
 Description-Content-Type: text/markdown
 
 # AskNews Python SDk
```

## Comparing `asknews-0.6.1.dist-info/RECORD` & `asknews-0.6.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 asknews_sdk/dto/sentiment.py,sha256=ZK0ArKptbbu7WScZWxavZrONDb5l2o9jlPdrCBF5epg,588
 asknews_sdk/dto/stories.py,sha256=H0TTy1t52NOkTP4mLB1bcDgibPh76_bDhOWV7UCtVw8,6643
 asknews_sdk/errors.py,sha256=2J6fihHeAL1ny7bdGAoEOazaRibosU3N4IFDBlO9vHk,1451
 asknews_sdk/sdk.py,sha256=EMQeZLuPeAWlV8yLbiefY_C7UuG-1pFDp7GwKJ0rsn4,6339
 asknews_sdk/security.py,sha256=mXVyc4_5KE2j-t5fS3IKewUfmCJZLCPbfcXMJJpLzIk,5396
 asknews_sdk/utils.py,sha256=tM7ga0MZGDA4YheH4dyZ6xxVVexMkzTMz0f6ttP6pwU,1614
 asknews_sdk/version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-asknews-0.6.1.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
-asknews-0.6.1.dist-info/METADATA,sha256=Cr61PEtDMQCVtd3QJNmc7wOeJ8y3LMJoJ4mfk4Hgzdk,3233
-asknews-0.6.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-asknews-0.6.1.dist-info/RECORD,,
+asknews-0.6.2.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
+asknews-0.6.2.dist-info/METADATA,sha256=jx-ASxXi2jtlvWiTSqrr35bui93SfayAfkbrNXnfZ3Y,3233
+asknews-0.6.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+asknews-0.6.2.dist-info/RECORD,,
```

