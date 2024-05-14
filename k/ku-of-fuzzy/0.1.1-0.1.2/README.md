# Comparing `tmp/ku_of_fuzzy-0.1.1-py3-none-any.whl.zip` & `tmp/ku_of_fuzzy-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 12682 bytes, number of entries: 7
+Zip file size: 12893 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        2 b- defN 24-May-13 01:06 ku_of_fuzzy/__init__.py
--rw-rw-rw-  2.0 fat    31589 b- defN 24-May-14 00:51 ku_of_fuzzy/fuzzy_calculate.py
--rw-rw-rw-  2.0 fat     1089 b- defN 24-May-14 01:21 ku_of_fuzzy-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    14873 b- defN 24-May-14 01:21 ku_of_fuzzy-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 01:21 ku_of_fuzzy-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-May-14 01:21 ku_of_fuzzy-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      572 b- defN 24-May-14 01:21 ku_of_fuzzy-0.1.1.dist-info/RECORD
-7 files, 48229 bytes uncompressed, 11664 bytes compressed:  75.8%
+-rw-rw-rw-  2.0 fat    31944 b- defN 24-May-14 06:44 ku_of_fuzzy/fuzzy_calculate.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 24-May-14 06:58 ku_of_fuzzy-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    15028 b- defN 24-May-14 06:58 ku_of_fuzzy-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 06:58 ku_of_fuzzy-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-May-14 06:58 ku_of_fuzzy-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      572 b- defN 24-May-14 06:58 ku_of_fuzzy-0.1.2.dist-info/RECORD
+7 files, 48739 bytes uncompressed, 11875 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: ku_of_fuzzy/__init__.py
 Comment: 
 
 Filename: ku_of_fuzzy/fuzzy_calculate.py
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.1.dist-info/LICENSE
+Filename: ku_of_fuzzy-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.1.dist-info/METADATA
+Filename: ku_of_fuzzy-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.1.dist-info/WHEEL
+Filename: ku_of_fuzzy-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.1.dist-info/top_level.txt
+Filename: ku_of_fuzzy-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ku_of_fuzzy-0.1.1.dist-info/RECORD
+Filename: ku_of_fuzzy-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ku_of_fuzzy/fuzzy_calculate.py

```diff
@@ -546,22 +546,31 @@
 augmented_dendrogram(Z)
 plt.show()'''
 
 
 # 根据模糊等价矩阵生成动态聚类图
 
 
-def draw(df):
-    """这里是提供一个我个人常用的聚类图的类型
-    如果想要个性化的化可以直接用augmented_dendrogram()和matplotlib
-    参数同dendrogram()一样的
-    加强版额外标出了λ的值
-    别忘了plt.show()哦
+def draw(df,width=6.4,height=4.8):
+    """
+    绘制基于模糊链接矩阵的动态聚类树状图。
+
+    参数:
+    df (DataFrame): 用于聚类的数据框。
+    width (float): 图形的宽度，默认为6.4英寸。
+    height (float): 图形的高度，默认为4.8英寸。
+
+    返回:
+    None: 该函数不返回任何值，但会显示一个树状图。
+    注意:
+    - 如果想要个性化定制图形，可以直接使用augmented_dendrogram()和matplotlib库的其他功能。
+    - 别忘了在函数调用后使用plt.show()来显示图形。
     """
     Z = fuzzy_linkage(df)
+    plt.figure(figsize=(width, height))
     augmented_dendrogram(Z, labels=df.columns)
     plt.rcParams['font.sans-serif'] = ['SimHei']
     ax = plt.gca()
     ax.spines['top'].set_visible(False)
     ax.spines['right'].set_visible(False)
     ax.spines['bottom'].set_visible(False)
     ax.spines['left'].set_visible(False)
```

## Comparing `ku_of_fuzzy-0.1.1.dist-info/LICENSE` & `ku_of_fuzzy-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ku_of_fuzzy-0.1.1.dist-info/METADATA` & `ku_of_fuzzy-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ku_of_fuzzy
-Version: 0.1.1
+Version: 0.1.2
 Summary: 用于模糊数学计算的Python库
 Home-page: https://github.com/YueorLekai/ku_of_fuzzy
 Author: Yuekai
 Author-email: 1977269004@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -230,14 +230,16 @@
 - **描述**: 绘制加强型动态聚类图，额外标出了λ的值。
 
 ### 动态聚类图绘制
 - **函数**: `draw(df)`
 - **描述**: 提供一个常用的聚类图绘制方法，额外标出了λ的值。如果需要个性化定制，可以使用`augmented_dendrogram()`和`matplotlib`库。
 - **参数**:
   - `df` (DataFrame): 输入的模糊等价矩阵。
+  - `width` (float): 图形的宽度，以英寸为单位，默认为6.4。
+  - `height` (float): 图形的高度，以英寸为单位，默认为4.8。
 - **注意**: 在绘制完聚类图后，使用`plt.show()`来显示图像。
 
 ### 模糊统计量F的求解
 - **函数**: `fuzzy_statistic(df0, df1, lambda_level)`
 - **描述**: 输入原始元素-属性矩阵和归一化、相似后的矩阵，返回对应λ的F值。
 
 ### 最优分类λ值求解
```

## Comparing `ku_of_fuzzy-0.1.1.dist-info/RECORD` & `ku_of_fuzzy-0.1.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 ku_of_fuzzy/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-ku_of_fuzzy/fuzzy_calculate.py,sha256=54Z5PpFAGJnBG5TRky8-Q6cPFmPayYfdLd2g0bTIKJ4,31589
-ku_of_fuzzy-0.1.1.dist-info/LICENSE,sha256=fDZm28u_emvGIctHAbLP5bx1dgcjHwCGo61aK7b1Cg8,1089
-ku_of_fuzzy-0.1.1.dist-info/METADATA,sha256=c7ozPLC0V4jk24uYwzoqxsRqg6zOiT6AT9y7FcmEtJ8,14873
-ku_of_fuzzy-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ku_of_fuzzy-0.1.1.dist-info/top_level.txt,sha256=oaitTqS9nBZcV-nvMY-vUcjP_wLKTtrlNSNMeb3bUy4,12
-ku_of_fuzzy-0.1.1.dist-info/RECORD,,
+ku_of_fuzzy/fuzzy_calculate.py,sha256=1btTyArxGCexFbOkMU-NLU9rXIL9mATY0WxcwWECzyg,31944
+ku_of_fuzzy-0.1.2.dist-info/LICENSE,sha256=fDZm28u_emvGIctHAbLP5bx1dgcjHwCGo61aK7b1Cg8,1089
+ku_of_fuzzy-0.1.2.dist-info/METADATA,sha256=4NnSaYOF_JgvjPQ4U-QVll_qVAw7u8A8pjQZBMpKdvU,15028
+ku_of_fuzzy-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ku_of_fuzzy-0.1.2.dist-info/top_level.txt,sha256=oaitTqS9nBZcV-nvMY-vUcjP_wLKTtrlNSNMeb3bUy4,12
+ku_of_fuzzy-0.1.2.dist-info/RECORD,,
```

