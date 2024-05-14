# Comparing `tmp/saiph-1.5.2.tar.gz` & `tmp/saiph-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saiph-1.5.2.tar", max compression
+gzip compressed data, was "saiph-1.5.3.tar", max compression
```

## Comparing `saiph-1.5.2.tar` & `saiph-1.5.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     9861 2024-04-26 09:34:44.539190 saiph-1.5.2/LICENSE
--rw-r--r--   0        0        0     2210 2024-04-26 09:34:44.543191 saiph-1.5.2/pyproject.toml
--rw-r--r--   0        0        0      286 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/__init__.py
--rw-r--r--   0        0        0     4439 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/conftest.py
--rw-r--r--   0        0        0     1195 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/contribution.py
--rw-r--r--   0        0        0     1384 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/contribution_test.py
--rw-r--r--   0        0        0      119 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/exception.py
--rw-r--r--   0        0        0     7031 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/inverse_transform.py
--rw-r--r--   0        0        0     9868 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/inverse_transform_test.py
--rw-r--r--   0        0        0      410 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/lib/size.py
--rw-r--r--   0        0        0     2511 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/models.py
--rw-r--r--   0        0        0     8738 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/projection.py
--rw-r--r--   0        0        0    13496 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/projection_test.py
--rw-r--r--   0        0        0       26 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/__init__.py
--rw-r--r--   0        0        0    15986 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/famd.py
--rw-r--r--   0        0        0     4911 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/famd_sparse.py
--rw-r--r--   0        0        0     4879 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/famd_sparse_test.py
--rw-r--r--   0        0        0     8509 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/famd_test.py
--rw-r--r--   0        0        0     9690 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/mca.py
--rw-r--r--   0        0        0     6868 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/mca_test.py
--rw-r--r--   0        0        0     4558 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/pca.py
--rw-r--r--   0        0        0     3829 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/pca_test.py
--rw-r--r--   0        0        0        0 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/utils/__init__.py
--rw-r--r--   0        0        0     3823 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/utils/common.py
--rw-r--r--   0        0        0     2455 2024-04-26 09:34:44.543191 saiph-1.5.2/saiph/reduction/utils/common_test.py
--rw-r--r--   0        0        0     4709 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/reduction/utils/svd.py
--rw-r--r--   0        0        0     5288 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/reduction/utils/svd_test.py
--rw-r--r--   0        0        0     5178 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/serializer.py
--rw-r--r--   0        0        0     2002 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/serializer_test.py
--rw-r--r--   0        0        0        0 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/tests/__init_.py
--rw-r--r--   0        0        0     1402 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/tests/benchmark_test.py
--rw-r--r--   0        0        0      521 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/tests/profile_cpu.py
--rw-r--r--   0        0        0      983 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/tests/profile_memory.py
--rw-r--r--   0        0        0     5405 2024-04-26 09:34:44.547191 saiph-1.5.2/saiph/visualization.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 saiph-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     9861 2024-05-14 15:31:45.874910 saiph-1.5.3/LICENSE
+-rw-r--r--   0        0        0     2210 2024-05-14 15:31:45.874910 saiph-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0      286 2024-05-14 15:31:45.874910 saiph-1.5.3/saiph/__init__.py
+-rw-r--r--   0        0        0     4439 2024-05-14 15:31:45.874910 saiph-1.5.3/saiph/conftest.py
+-rw-r--r--   0        0        0     1195 2024-05-14 15:31:45.874910 saiph-1.5.3/saiph/contribution.py
+-rw-r--r--   0        0        0     1384 2024-05-14 15:31:45.874910 saiph-1.5.3/saiph/contribution_test.py
+-rw-r--r--   0        0        0      119 2024-05-14 15:31:45.874910 saiph-1.5.3/saiph/exception.py
+-rw-r--r--   0        0        0     7031 2024-05-14 15:31:45.874910 saiph-1.5.3/saiph/inverse_transform.py
+-rw-r--r--   0        0        0     9868 2024-05-14 15:31:45.874910 saiph-1.5.3/saiph/inverse_transform_test.py
+-rw-r--r--   0        0        0      410 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/lib/size.py
+-rw-r--r--   0        0        0     2511 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/models.py
+-rw-r--r--   0        0        0     8738 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/projection.py
+-rw-r--r--   0        0        0    13496 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/projection_test.py
+-rw-r--r--   0        0        0       26 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/__init__.py
+-rw-r--r--   0        0        0    16087 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/famd.py
+-rw-r--r--   0        0        0     4911 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/famd_sparse.py
+-rw-r--r--   0        0        0     4879 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/famd_sparse_test.py
+-rw-r--r--   0        0        0     8509 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/famd_test.py
+-rw-r--r--   0        0        0     9690 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/mca.py
+-rw-r--r--   0        0        0     6868 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/mca_test.py
+-rw-r--r--   0        0        0     4558 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/pca.py
+-rw-r--r--   0        0        0     3829 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/pca_test.py
+-rw-r--r--   0        0        0        0 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/utils/__init__.py
+-rw-r--r--   0        0        0     3823 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/utils/common.py
+-rw-r--r--   0        0        0     2455 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/utils/common_test.py
+-rw-r--r--   0        0        0     4709 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/utils/svd.py
+-rw-r--r--   0        0        0     5288 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/reduction/utils/svd_test.py
+-rw-r--r--   0        0        0     5178 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/serializer.py
+-rw-r--r--   0        0        0     2002 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/serializer_test.py
+-rw-r--r--   0        0        0        0 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/tests/__init_.py
+-rw-r--r--   0        0        0     1402 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/tests/benchmark_test.py
+-rw-r--r--   0        0        0      521 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/tests/profile_cpu.py
+-rw-r--r--   0        0        0      983 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/tests/profile_memory.py
+-rw-r--r--   0        0        0     5405 2024-05-14 15:31:45.878910 saiph-1.5.3/saiph/visualization.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 saiph-1.5.3/PKG-INFO
```

### Comparing `saiph-1.5.2/LICENSE` & `saiph-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/pyproject.toml` & `saiph-1.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "saiph"
 # Also modify in saiph/__init__.py
-version = "1.5.2"
+version = "1.5.3"
 description = "A projection package"
 authors = ["Octopize <help@octopize.io>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 pandas = "^1.3"
```

### Comparing `saiph-1.5.2/saiph/conftest.py` & `saiph-1.5.3/saiph/conftest.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/contribution.py` & `saiph-1.5.3/saiph/contribution.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/contribution_test.py` & `saiph-1.5.3/saiph/contribution_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/inverse_transform.py` & `saiph-1.5.3/saiph/inverse_transform.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/inverse_transform_test.py` & `saiph-1.5.3/saiph/inverse_transform_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/models.py` & `saiph-1.5.3/saiph/models.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/projection.py` & `saiph-1.5.3/saiph/projection.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/projection_test.py` & `saiph-1.5.3/saiph/projection_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/reduction/famd.py` & `saiph-1.5.3/saiph/reduction/famd.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,23 +479,29 @@
     coords :
         projections of the data used to created the axes
 
     Returns
     -------
         cos2 of the single category
     """
+    _, n_cols = single_category_df.shape
     cos2 = []
+
     for coord_col in coords.columns:
-        # for each modality of the qualitative column
-        p = 0
-        for col in single_category_df.columns:
-            weighted_coords = coords[coord_col] * model.row_weights
+        weighted_coord = coords[coord_col].values * model.row_weights
+        p_values = np.zeros(n_cols)
+
+        for i, col in enumerate(single_category_df.columns):
             dummy_values = single_category_df[col].values
             if model.prop is not None:
-                p += (dummy_values * weighted_coords).sum() ** 2 / model.prop[col]
+                p_values[i] = (dummy_values * weighted_coord).sum() ** 2 / model.prop[
+                    col
+                ]
 
+        p = p_values.sum()
         cos2.append(p)
+
     all_weighted_coords = (coords.values**2).T * model.row_weights
     summed_weights = all_weighted_coords.sum(axis=1)
 
     single_category_cos2: NDArray[np.float_] = np.array(cos2) / summed_weights
     return single_category_cos2
```

### Comparing `saiph-1.5.2/saiph/reduction/famd_sparse.py` & `saiph-1.5.3/saiph/reduction/famd_sparse.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/reduction/famd_sparse_test.py` & `saiph-1.5.3/saiph/reduction/famd_sparse_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/reduction/famd_test.py` & `saiph-1.5.3/saiph/reduction/famd_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/reduction/mca.py` & `saiph-1.5.3/saiph/reduction/mca.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/reduction/mca_test.py` & `saiph-1.5.3/saiph/reduction/mca_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/reduction/pca.py` & `saiph-1.5.3/saiph/reduction/pca.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/reduction/pca_test.py` & `saiph-1.5.3/saiph/reduction/pca_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/reduction/utils/common.py` & `saiph-1.5.3/saiph/reduction/utils/common.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/reduction/utils/common_test.py` & `saiph-1.5.3/saiph/reduction/utils/common_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/reduction/utils/svd.py` & `saiph-1.5.3/saiph/reduction/utils/svd.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/reduction/utils/svd_test.py` & `saiph-1.5.3/saiph/reduction/utils/svd_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/serializer.py` & `saiph-1.5.3/saiph/serializer.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/serializer_test.py` & `saiph-1.5.3/saiph/serializer_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/tests/benchmark_test.py` & `saiph-1.5.3/saiph/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/tests/profile_cpu.py` & `saiph-1.5.3/saiph/tests/profile_cpu.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/tests/profile_memory.py` & `saiph-1.5.3/saiph/tests/profile_memory.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/saiph/visualization.py` & `saiph-1.5.3/saiph/visualization.py`

 * *Files identical despite different names*

### Comparing `saiph-1.5.2/PKG-INFO` & `saiph-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saiph
-Version: 1.5.2
+Version: 1.5.3
 Summary: A projection package
 License: Apache-2.0
 Author: Octopize
 Author-email: help@octopize.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

