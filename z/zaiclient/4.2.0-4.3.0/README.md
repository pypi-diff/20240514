# Comparing `tmp/zaiclient-4.2.0-py3-none-any.whl.zip` & `tmp/zaiclient-4.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 24793 bytes, number of entries: 45
+Zip file size: 24839 bytes, number of entries: 45
 -rw-r--r--  2.0 unx      350 b- defN 80-Jan-01 00:00 zaiclient/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 zaiclient/__main__.py
 -rw-r--r--  2.0 unx     1371 b- defN 80-Jan-01 00:00 zaiclient/auth.py
 -rw-r--r--  2.0 unx     6714 b- defN 80-Jan-01 00:00 zaiclient/client.py
 -rw-r--r--  2.0 unx      799 b- defN 80-Jan-01 00:00 zaiclient/config.py
 -rw-r--r--  2.0 unx      150 b- defN 80-Jan-01 00:00 zaiclient/exceptions/BatchSizeLimitExceededException.py
 -rw-r--r--  2.0 unx      114 b- defN 80-Jan-01 00:00 zaiclient/exceptions/EmptyBatchException.py
@@ -33,15 +33,15 @@
 -rw-r--r--  2.0 unx     1303 b- defN 80-Jan-01 00:00 zaiclient/request/Recommendations/GetRerankingRecommendation.py
 -rw-r--r--  2.0 unx     1041 b- defN 80-Jan-01 00:00 zaiclient/request/Recommendations/GetUserRecommendation.py
 -rw-r--r--  2.0 unx      724 b- defN 80-Jan-01 00:00 zaiclient/request/Recommendations/Recommendation.py
 -rw-r--r--  2.0 unx     1042 b- defN 80-Jan-01 00:00 zaiclient/request/Recommendations/RecommendationRequest.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 zaiclient/request/Recommendations/__init__.py
 -rw-r--r--  2.0 unx      439 b- defN 80-Jan-01 00:00 zaiclient/request/Request.py
 -rw-r--r--  2.0 unx     1613 b- defN 80-Jan-01 00:00 zaiclient/request/__init__.py
--rw-r--r--  2.0 unx      499 b- defN 80-Jan-01 00:00 zaiclient/response/EventLoggerResponse.py
+-rw-r--r--  2.0 unx      500 b- defN 80-Jan-01 00:00 zaiclient/response/EventLoggerResponse.py
 -rw-r--r--  2.0 unx      261 b- defN 80-Jan-01 00:00 zaiclient/response/ItemResponse.py
--rw-r--r--  2.0 unx      533 b- defN 80-Jan-01 00:00 zaiclient/response/RecommendationResponse.py
+-rw-r--r--  2.0 unx      644 b- defN 80-Jan-01 00:00 zaiclient/response/RecommendationResponse.py
 -rw-r--r--  2.0 unx      224 b- defN 80-Jan-01 00:00 zaiclient/response/__init__.py
--rw-r--r--  2.0 unx     1853 b- defN 80-Jan-01 00:00 zaiclient-4.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 zaiclient-4.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     4239 b- defN 16-Jan-01 00:00 zaiclient-4.2.0.dist-info/RECORD
-45 files, 51921 bytes uncompressed, 17829 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx     1853 b- defN 80-Jan-01 00:00 zaiclient-4.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 zaiclient-4.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     4239 b- defN 16-Jan-01 00:00 zaiclient-4.3.0.dist-info/RECORD
+45 files, 52033 bytes uncompressed, 17875 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -120,17 +120,17 @@
 
 Filename: zaiclient/response/RecommendationResponse.py
 Comment: 
 
 Filename: zaiclient/response/__init__.py
 Comment: 
 
-Filename: zaiclient-4.2.0.dist-info/METADATA
+Filename: zaiclient-4.3.0.dist-info/METADATA
 Comment: 
 
-Filename: zaiclient-4.2.0.dist-info/WHEEL
+Filename: zaiclient-4.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: zaiclient-4.2.0.dist-info/RECORD
+Filename: zaiclient-4.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zaiclient/__init__.py

```diff
@@ -1,13 +1,13 @@
 """Copyright (c) 2022 Z.Ai Inc. ALL RIGHTS RESERVED
 
 Z.Ai official client SDK.
 Z.Ai's clients can utilize this SDK to easily connect to the provided API endpoints.
 """
 # ruff: noqa: F401
 
-__version__ = "4.2.0"
+__version__ = "4.3.0"
 
 from zaiclient.client import ZaiClient
 from zaiclient.exceptions import *
 from zaiclient.request import *
 from zaiclient.response import *
```

## zaiclient/response/EventLoggerResponse.py

```diff
@@ -6,11 +6,11 @@
     failure_count: conint(ge=0, le=10000)
     timestamp: confloat(ge=1_648_871_097.0, le=2_147_483_647.0)
 
     class Config:
         schema_extra = {
             "example": {
                 "message": "The given event was handled successfully.",
-                "failed_count": 0,
+                "failure_count": 0,
                 "timestamp": 1_648_871_097.0,
             }
         }
```

## zaiclient/response/RecommendationResponse.py

```diff
@@ -4,17 +4,19 @@
 
 
 class RecommendationResponse(BaseModel):
     items: List[str]
     count: conint(ge=0, le=10_000)
     metadata: dict
     timestamp: confloat(ge=1_648_871_097.0, le=2_147_483_647.0)
+    recommendation_id: str | None
 
     class Config:
         schema_extra = {
             "example": {
                 "items": ["1234", "1232"],
                 "count": 4,
                 "metadata": {"recommendation_type": "homepage"},
                 "timestamp": 1648835666.825221,
+                "recommendation_id": "e912f039-8717-46a2-9879-4eac1268dcaf",
             }
         }
```

## Comparing `zaiclient-4.2.0.dist-info/METADATA` & `zaiclient-4.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaiclient
-Version: 4.2.0
+Version: 4.3.0
 Summary: Z.Ai official client SDK.
 Home-page: https://github.com/zaikorea/zaiclient-python
 License: Proprietary
 Author: Z.Ai Inc.
 Author-email: tech@zaikorea.org
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
```

## Comparing `zaiclient-4.2.0.dist-info/RECORD` & `zaiclient-4.3.0.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-zaiclient/__init__.py,sha256=pVpRIwx-aCPLnUGSvahvCu7iD3gona97hQklZaAosDk,350
+zaiclient/__init__.py,sha256=MdaJfzpDFq_OQLBa8t7cPStOYD4gFFi5ZlQ-UfbiPhE,350
 zaiclient/__main__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 zaiclient/auth.py,sha256=ksfvxljshg3TK9u6LiynBpZo-M9I0xA6oYbKsWDSxe0,1371
 zaiclient/client.py,sha256=KL-Q4eL7duiN_1B7sTbha5eoelyeULP2PT-xVn9_sE0,6714
 zaiclient/config.py,sha256=9rgoJjHgmy1FzDb9D2n_PkcNC9oF8_voe-kG1lGcSL4,799
 zaiclient/exceptions/BatchSizeLimitExceededException.py,sha256=wn1nyw0WeXzaobipnOaau0vxNktbtbQT4nFXeBUGOkQ,150
 zaiclient/exceptions/EmptyBatchException.py,sha256=TIa9sba-FtlXKw0fYIjjhGpS12DEcPO4a6tU8GY7xiU,114
 zaiclient/exceptions/InputLengthNotEqualException.py,sha256=6R1qzAL_xYcJwOF-NQLtqwPg-xsyzXu-oOK2oftZdm0,145
@@ -32,14 +32,14 @@
 zaiclient/request/Recommendations/GetRerankingRecommendation.py,sha256=-3C1jbni9XHugJptb5WuSxIhugoh6OHVf_xiPcq_Ubc,1303
 zaiclient/request/Recommendations/GetUserRecommendation.py,sha256=sDdfr8CFVIgY_SCH5JxqgMUAox7ChEL8DTyR0-0kaUw,1041
 zaiclient/request/Recommendations/Recommendation.py,sha256=baWvZs1nHbEXd4ceg7RzZv4c2OYrT06hrDc6tfmd_0A,724
 zaiclient/request/Recommendations/RecommendationRequest.py,sha256=5XMnvyqBEKVrU6LjTs_87LmpZ_S43ur5Z9WGXV4nd44,1042
 zaiclient/request/Recommendations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 zaiclient/request/Request.py,sha256=DwKwnMFLC3SHZ9UzWCyeYcog_14ca40l9T7frP1QPDA,439
 zaiclient/request/__init__.py,sha256=3VVVEHb33hEs2pI3hpCsbeNhxGsoX48Q7q04DM_k2kE,1613
-zaiclient/response/EventLoggerResponse.py,sha256=m1gvvqhr2oDdIaiCfalfjd1GsBghU2W0M3VccIrv5cA,499
+zaiclient/response/EventLoggerResponse.py,sha256=-gNzv41gwvmYc2Hp6hVIt6tTLMsuN1hgGojwsFlYmww,500
 zaiclient/response/ItemResponse.py,sha256=VjqYZ3-lccsPKQRCd0FYfJVa5UH_aNTBZqiwA-Fkbao,261
-zaiclient/response/RecommendationResponse.py,sha256=rdA7RenvhLcz_0Dtkvzev2YSyq8EAcn9_FDh2OPacdU,533
+zaiclient/response/RecommendationResponse.py,sha256=yW3uPAEDzAPZrenEc3WrI2dA2tDV_H7WTWLHWedwRF0,644
 zaiclient/response/__init__.py,sha256=fX4BThAAu6jvXdsrO9Qlemrl6LjliJagY1WwpS0amjo,224
-zaiclient-4.2.0.dist-info/METADATA,sha256=tD27lctbS_mx7VOjqE18piGCz_ykodj9rQEW6SAXeFY,1853
-zaiclient-4.2.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-zaiclient-4.2.0.dist-info/RECORD,,
+zaiclient-4.3.0.dist-info/METADATA,sha256=jOBQL3kw0-u5WAup_GlJc0dCJ4dBI40-v2BfVotUv2Q,1853
+zaiclient-4.3.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+zaiclient-4.3.0.dist-info/RECORD,,
```

