# Comparing `tmp/easy_notion_api-0.1.4-py3-none-any.whl.zip` & `tmp/easy_notion_api-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7055 bytes, number of entries: 12
+Zip file size: 7084 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       27 b- defN 23-Nov-29 08:24 notion/__init__.py
 -rw-r--r--  2.0 unx      440 b- defN 23-Nov-30 09:22 notion/core.py
 -rw-r--r--  2.0 unx      778 b- defN 24-Mar-27 05:17 notion/database.py
 -rw-r--r--  2.0 unx      406 b- defN 23-Nov-30 05:04 notion/exceptions.py
--rw-r--r--  2.0 unx     5103 b- defN 24-Mar-27 05:17 notion/notion.py
+-rw-r--r--  2.0 unx     5286 b- defN 24-May-14 06:19 notion/notion.py
 -rw-r--r--  2.0 unx      648 b- defN 24-Mar-27 05:17 notion/page.py
 -rw-r--r--  2.0 unx     1080 b- defN 24-Mar-27 05:17 notion/user.py
--rw-r--r--  2.0 unx     1061 b- defN 24-May-01 07:39 easy_notion_api-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2910 b- defN 24-May-01 07:39 easy_notion_api-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-01 07:39 easy_notion_api-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-May-01 07:39 easy_notion_api-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      932 b- defN 24-May-01 07:39 easy_notion_api-0.1.4.dist-info/RECORD
-12 files, 13484 bytes uncompressed, 5495 bytes compressed:  59.2%
+-rw-r--r--  2.0 unx     1061 b- defN 24-May-14 07:21 easy_notion_api-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2910 b- defN 24-May-14 07:21 easy_notion_api-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 07:21 easy_notion_api-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-14 07:21 easy_notion_api-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      932 b- defN 24-May-14 07:21 easy_notion_api-0.1.5.dist-info/RECORD
+12 files, 13667 bytes uncompressed, 5524 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: notion/page.py
 Comment: 
 
 Filename: notion/user.py
 Comment: 
 
-Filename: easy_notion_api-0.1.4.dist-info/LICENSE
+Filename: easy_notion_api-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: easy_notion_api-0.1.4.dist-info/METADATA
+Filename: easy_notion_api-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: easy_notion_api-0.1.4.dist-info/WHEEL
+Filename: easy_notion_api-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: easy_notion_api-0.1.4.dist-info/top_level.txt
+Filename: easy_notion_api-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: easy_notion_api-0.1.4.dist-info/RECORD
+Filename: easy_notion_api-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## notion/notion.py

```diff
@@ -150,10 +150,15 @@
                 data_form[data_key] = {col_type: users}
 
             elif col_type == "checkbox":
                 if not isinstance(value, bool):
                     raise InvalidData(f"The Key {data_key} must be boolean")
                 data_form[data_key] = {col_type: value}
             elif col_type == "date":
-                data_form[data_key] = {col_type: {"start": value[0], "end": value[1]}}
+                if type(value) == list:
+                    data_form[data_key] = {
+                        col_type: {"start": value[0], "end": value[1]}
+                    }
+                else:
+                    data_form[data_key] = {col_type: {"start": value}}
 
         return data_form
```

## Comparing `easy_notion_api-0.1.4.dist-info/LICENSE` & `easy_notion_api-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `easy_notion_api-0.1.4.dist-info/METADATA` & `easy_notion_api-0.1.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-notion-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: Unofficial Python API client for Notion
 Home-page: https://github.com/Hans97a/easy-notion-api
 Author: Hans97a
 Author-email: byby8992@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `easy_notion_api-0.1.4.dist-info/RECORD` & `easy_notion_api-0.1.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 notion/__init__.py,sha256=Qw14aNtCniBye1SQ5gD9xRahyrtl3DaXXXiTzhZlLNc,27
 notion/core.py,sha256=vMfYywTHLDmpbjG-fMkFewit1y9o6kuIieUAnFXvGts,440
 notion/database.py,sha256=vZSvfLRa_LBsNkKEIQT6qttpgK6Mbk4XtNcFMUhdyik,778
 notion/exceptions.py,sha256=DPxBTAqTHkPW2s2nxY-H6pC7g4sPJFyROuGli_cMj8o,406
-notion/notion.py,sha256=IMfIfiD4TH0lIlXyUTK33_-fBDFpLBrNK7A_eMF9iMc,5103
+notion/notion.py,sha256=EWSqcHW6VcvPuK18nR4dh-SDJu3QWfSUI8LP9tT41Iw,5286
 notion/page.py,sha256=PI-jzEJCYWsRW3POjiDJH-_GSokhdxnaqpRGHBJmX3M,648
 notion/user.py,sha256=arHbrLeIHWxHNaD3xWj7lfD9NNbqI4LoVIrHVgvx4MA,1080
-easy_notion_api-0.1.4.dist-info/LICENSE,sha256=8whQTDFStEXIG4xEpl-vWuXr6Tevalqfw1w9vhIe5Vw,1061
-easy_notion_api-0.1.4.dist-info/METADATA,sha256=VyiH-alJ-qzXcXkPfk4ZXcduPrYiTur9x6V47T9THq4,2910
-easy_notion_api-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-easy_notion_api-0.1.4.dist-info/top_level.txt,sha256=r_d1o60I-zSgTmqPuoFA0HpSmOydrIqu_Gz_zhtPkgc,7
-easy_notion_api-0.1.4.dist-info/RECORD,,
+easy_notion_api-0.1.5.dist-info/LICENSE,sha256=8whQTDFStEXIG4xEpl-vWuXr6Tevalqfw1w9vhIe5Vw,1061
+easy_notion_api-0.1.5.dist-info/METADATA,sha256=_VbtvFHT_qU2_KamD5uZJGFqN2i9KIqSal3GoqNKmi4,2910
+easy_notion_api-0.1.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+easy_notion_api-0.1.5.dist-info/top_level.txt,sha256=r_d1o60I-zSgTmqPuoFA0HpSmOydrIqu_Gz_zhtPkgc,7
+easy_notion_api-0.1.5.dist-info/RECORD,,
```

