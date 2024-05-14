# Comparing `tmp/semantic_link-0.7.1-py3-none-any.whl.zip` & `tmp/semantic_link-0.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
 Zip file size: 8235 bytes, number of entries: 5
--rw-rw-r--  2.0 unx    12690 b- defN 24-Mar-18 18:39 semantic_link-0.7.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     5068 b- defN 24-Mar-18 18:39 semantic_link-0.7.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-18 18:39 semantic_link-0.7.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 24-Mar-18 18:39 semantic_link-0.7.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      420 b- defN 24-Mar-18 18:39 semantic_link-0.7.1.dist-info/RECORD
+-rw-rw-r--  2.0 unx    12690 b- defN 24-Mar-21 23:48 semantic_link-0.7.2.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     5068 b- defN 24-Mar-21 23:48 semantic_link-0.7.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Mar-21 23:48 semantic_link-0.7.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 24-Mar-21 23:48 semantic_link-0.7.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      420 b- defN 24-Mar-21 23:48 semantic_link-0.7.2.dist-info/RECORD
 5 files, 18271 bytes uncompressed, 7447 bytes compressed:  59.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: semantic_link-0.7.1.dist-info/LICENSE.txt
+Filename: semantic_link-0.7.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: semantic_link-0.7.1.dist-info/METADATA
+Filename: semantic_link-0.7.2.dist-info/METADATA
 Comment: 
 
-Filename: semantic_link-0.7.1.dist-info/WHEEL
+Filename: semantic_link-0.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: semantic_link-0.7.1.dist-info/top_level.txt
+Filename: semantic_link-0.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: semantic_link-0.7.1.dist-info/RECORD
+Filename: semantic_link-0.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `semantic_link-0.7.1.dist-info/LICENSE.txt` & `semantic_link-0.7.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `semantic_link-0.7.1.dist-info/METADATA` & `semantic_link-0.7.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: semantic-link
-Version: 0.7.1
+Version: 0.7.2
 Summary: Semantic link for Microsoft Fabric
 Home-page: https://learn.microsoft.com/en-us/fabric/data-science/semantic-link-overview
 Author: Microsoft
 Author-email: semanticdatascience@service.microsoft.com
 License: proprietary and confidential
 Platform: Microsoft Fabric
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: ../LICENSE.txt
-Requires-Dist: semantic-link-sempy ==0.7.1
-Requires-Dist: semantic-link-functions-geopandas ==0.7.1
-Requires-Dist: semantic-link-functions-holidays ==0.7.1
-Requires-Dist: semantic-link-functions-meteostat ==0.7.1
-Requires-Dist: semantic-link-functions-phonenumbers ==0.7.1
-Requires-Dist: semantic-link-functions-validators ==0.7.1
+Requires-Dist: semantic-link-sempy ==0.7.2
+Requires-Dist: semantic-link-functions-geopandas ==0.7.2
+Requires-Dist: semantic-link-functions-holidays ==0.7.2
+Requires-Dist: semantic-link-functions-meteostat ==0.7.2
+Requires-Dist: semantic-link-functions-phonenumbers ==0.7.2
+Requires-Dist: semantic-link-functions-validators ==0.7.2
 
 Semantic link is a feature that allows you to establish a connection between [Power BI datasets](https://learn.microsoft.com/en-us/power-bi/connect-data/service-datasets-understand) and [Synapse Data Science in Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/data-science/data-science-overview).  
 
 The primary goals of semantic link are to facilitate data connectivity, enable the propagation of semantic information, and seamlessly integrate with established tools used by data scientists, such as notebooks.  
 
 Semantic link helps you to preserve domain knowledge about data semantics in a standardized way that can speed up data analysis and reduce errors.
```

