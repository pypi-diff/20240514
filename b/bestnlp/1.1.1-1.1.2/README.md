# Comparing `tmp/bestnlp-1.1.1-py3-none-any.whl.zip` & `tmp/bestnlp-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 1913199 bytes, number of entries: 10
+Zip file size: 1913282 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      325 b- defN 24-Apr-22 10:55 bestnlp/__init__.py
 -rw-r--r--  2.0 unx  5071852 b- defN 24-Mar-29 09:38 bestnlp/dict.txt
 -rw-r--r--  2.0 unx     7610 b- defN 24-Apr-15 06:26 bestnlp/new_word_discovery.py
--rw-r--r--  2.0 unx    11004 b- defN 24-Apr-22 10:54 bestnlp/similar_word_discovery.py
+-rw-r--r--  2.0 unx    12085 b- defN 24-May-14 11:01 bestnlp/similar_word_discovery.py
 -rw-r--r--  2.0 unx     4004 b- defN 24-Mar-29 09:39 bestnlp/similar_word_discovery_embedding.py
 -rw-r--r--  2.0 unx      958 b- defN 24-Apr-09 10:58 bestnlp/utils.py
--rw-r--r--  2.0 unx      245 b- defN 24-Apr-22 10:57 bestnlp-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 10:57 bestnlp-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-22 10:57 bestnlp-1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      796 b- defN 24-Apr-22 10:57 bestnlp-1.1.1.dist-info/RECORD
-10 files, 5096894 bytes uncompressed, 1911849 bytes compressed:  62.5%
+-rw-r--r--  2.0 unx      245 b- defN 24-May-14 11:05 bestnlp-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 11:05 bestnlp-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-14 11:05 bestnlp-1.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      796 b- defN 24-May-14 11:05 bestnlp-1.1.2.dist-info/RECORD
+10 files, 5097975 bytes uncompressed, 1911932 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: bestnlp/similar_word_discovery_embedding.py
 Comment: 
 
 Filename: bestnlp/utils.py
 Comment: 
 
-Filename: bestnlp-1.1.1.dist-info/METADATA
+Filename: bestnlp-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: bestnlp-1.1.1.dist-info/WHEEL
+Filename: bestnlp-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: bestnlp-1.1.1.dist-info/top_level.txt
+Filename: bestnlp-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bestnlp-1.1.1.dist-info/RECORD
+Filename: bestnlp-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bestnlp/similar_word_discovery.py

```diff
@@ -37,15 +37,15 @@
                     di[keyword[i]][keyword[i + 1]] = di[keyword[i]].get(keyword[i + 1], 0) + 1
         res = dict()
         for key, value in di.items():
             sum_num = sum(value.values())
             res[key] = dict()
             for key2 in value:
                 ratio = value[key2]/sum_num
-                if value[key2] > threshold:
+                if value[key2] > threshold and ratio > 0.1:
                     res[key][key2] = value[key2]
         for key, value in res.items():
             for key2 in value:
                 print(key, key2, value[key2])
         final_res = dict()
         for key, value in res.items():
             for key2 in value:
@@ -94,21 +94,21 @@
                 if key2 in res and key in res[key2]:
                     final_res[frozenset([key, key2])] = res[key][key2] + res[key2][key]
         return final_res
 
 
     def find_similar(self, search_df, click_df, search_weight=1, click_weight=1, both=False, search_threshod=None, click_threshold=None, threshold=None, max_num=1000, time_name="time", user_id_name="user_id", keyword_name="keyword", item_id_name="item_id"):
         search_df = search_df[~((search_df[keyword_name].isnull()) | (search_df[keyword_name] == ""))]
-        search_df[keyword_name] = search_df[keyword_name].apply(lambda x: x.strip().lower())
+        search_df[keyword_name] = search_df[keyword_name].apply(lambda x: str(x).strip().lower())
         if search_threshod is None:
             search_threshod = max([5, math.pow(len(set(search_df[keyword_name])), 1 / 4),
                              math.pow(len(search_df[keyword_name]) / 2, 1 / 4)])
             print("default search threshold: ", search_threshod)
         click_df = click_df[~((click_df[keyword_name].isnull()) | (click_df[keyword_name] == ""))]
-        click_df[keyword_name] = click_df[keyword_name].apply(lambda x: x.strip().lower())
+        click_df[keyword_name] = click_df[keyword_name].apply(lambda x: str(x).strip().lower())
         if click_threshold is None:
             click_threshold = max(
                 [10, math.pow(len(set(click_df[keyword_name])), 1 / 4), math.pow(len(click_df[keyword_name]) / 2, 1 / 4)])
             print("default click threshold: ", click_threshold)
 
         search_res = self.process_search(search_df, search_threshod, time_name=time_name, user_id_name=user_id_name, keyword_name=keyword_name) if search_df is not None else dict()
         click_res = self.process_click(click_df, click_threshold, time_name=time_name, user_id_name=user_id_name, keyword_name=keyword_name, item_id_name=item_id_name) if click_df is not None else dict()
@@ -127,15 +127,16 @@
         res = list(sorted(res.items(), key=lambda x: x[1], reverse=True))
         res = res[:max_num if len(res) > max_num else len(res)]
         return res
 
 
     def get_search_similar(self, search_df, threshold=None, time_name="time", user_id_name="user_id", keyword_name="keyword"):
         #搜索行为
-        search_df[keyword_name] = search_df[keyword_name].apply(lambda x: x.strip().lower())
+        search_df = search_df[~((search_df[keyword_name].isnull()) | (search_df[keyword_name] == ""))]
+        search_df[keyword_name] = search_df[keyword_name].apply(lambda x: str(x).strip().lower())
         search_df = search_df[~((search_df[keyword_name].isnull()) | (search_df[keyword_name]==""))]
         if threshold is None:
             threshold = 5
         print("default search threshold: ", threshold)
         df = search_df.sort_values(time_name)
         df = df.groupby(user_id_name)[keyword_name].agg(list).reset_index()
         di = dict()
@@ -156,15 +157,16 @@
                     res[key][key2] = (value[key2], ratio)
         return res
 
 
     def get_click_similar(self, click_df, threshold=None, time_name="time", user_id_name="user_id", keyword_name="keyword", item_id_name="item_id"):
         #点击行为
         #同一个商品点击等行为对应的搜索词
-        click_df[keyword_name] = click_df[keyword_name].apply(lambda x: x.strip().lower())
+        click_df = click_df[~((click_df[keyword_name].isnull()) | (click_df[keyword_name] == ""))]
+        click_df[keyword_name] = click_df[keyword_name].apply(lambda x: str(x).strip().lower())
         click_df = click_df[~((click_df[keyword_name].isnull()) | (click_df[keyword_name]==""))]
         if threshold is None:
             threshold = 5
         print("default click threshold: ", threshold)
         act_df = click_df.sort_values(time_name).drop_duplicates([user_id_name, keyword_name, item_id_name])
         df = act_df.groupby(item_id_name)[keyword_name].agg(list).reset_index()
         di = dict()
@@ -182,14 +184,32 @@
             for key2 in value:
                 ratio = value[key2] / sum_num
                 if value[key2] > threshold:
                     res[key][key2] = (value[key2], ratio)
         return res
 
 
+    # def get_search_embedding_similar(self, search_df, threshold=None, time_name="time", user_id_name="user_id", keyword_name="keyword"):
+    #     # 搜索行为
+    #     search_df[keyword_name] = search_df[keyword_name].apply(lambda x: str(x).strip().lower())
+    #     search_df = search_df[~((search_df[keyword_name].isnull()) | (search_df[keyword_name] == ""))]
+    #     if threshold is None:
+    #         threshold = 5
+    #     print("default search threshold: ", threshold)
+    #     df = search_df.sort_values(time_name)
+    #     df = df.groupby(user_id_name)[keyword_name].agg(list).reset_index()
+    #     li = []
+    #
+    #     for keyword in df[keyword_name].tolist():
+    #         if len(keyword) >= 2:
+    #             for i in range(len(keyword) - 1):
+    #                 if keyword[i] == keyword[i + 1]: continue
+
+
+
 # import pandas as pd
 # df = pd.read_excel("df_details.xlsx")
 # search_df = df[df["action_type"]=="search"][["timestamp", "query", "userid"]]
 # search_df.rename(columns={"timestamp":"time", "query":"keyword", "userid":"user_id"}, inplace=True)
 # click_df = df[df["action_type"]=="click"][["timestamp", "query", "userid", "itemid"]]
 # click_df.rename(columns={"timestamp":"time", "query":"keyword", "userid":"user_id", "itemid":"item_id"}, inplace=True)
 # swd = SimilarWordDiscovery()
```

## Comparing `bestnlp-1.1.1.dist-info/RECORD` & `bestnlp-1.1.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 bestnlp/__init__.py,sha256=0XWpNdmxPa2JZgo6L9_HmWwpegVn5A2r3ycUA69XwN0,325
 bestnlp/dict.txt,sha256=cZfDIR3dmJYrA2zfQDJNHqK_qhK9Ao5o-qcBEaiOEqg,5071852
 bestnlp/new_word_discovery.py,sha256=zea2PJVBJJBqQkiW8HlARIp6JJRZXtmbIanHfmQzrS4,7610
-bestnlp/similar_word_discovery.py,sha256=qgiZ5FzRTPx4P3cOLcCQKdhENjxjahbNHWZZ0oFoAs4,11004
+bestnlp/similar_word_discovery.py,sha256=2MVMpRhbUFcjUJAq48NGi8cz6xJL695WWyqrrE4wwTU,12085
 bestnlp/similar_word_discovery_embedding.py,sha256=HsoxJomebHNlB9JyNfGghGSPJ6FJ4X0eAvRnbTUUmf8,4004
 bestnlp/utils.py,sha256=c8bSHGOjGJXOxFADZ9uKPKL6PClG2_XQGOsse3LJfNA,958
-bestnlp-1.1.1.dist-info/METADATA,sha256=EF1zKKODB3Pj1jYrNE_G5HhhIlkKTrGqh_9DPJQyM3c,245
-bestnlp-1.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-bestnlp-1.1.1.dist-info/top_level.txt,sha256=gEejasanGTcCsrx7FMvnDNjB5jb-Xf07bqn5DqRKxg8,8
-bestnlp-1.1.1.dist-info/RECORD,,
+bestnlp-1.1.2.dist-info/METADATA,sha256=L94d5z6uWE23HZW2E-6TGCcZvsDrGZyzEWMXj5_y7gA,245
+bestnlp-1.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+bestnlp-1.1.2.dist-info/top_level.txt,sha256=gEejasanGTcCsrx7FMvnDNjB5jb-Xf07bqn5DqRKxg8,8
+bestnlp-1.1.2.dist-info/RECORD,,
```

