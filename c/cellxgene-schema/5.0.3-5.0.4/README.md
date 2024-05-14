# Comparing `tmp/cellxgene-schema-5.0.3.tar.gz` & `tmp/cellxgene-schema-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene-schema-5.0.3.tar", last modified: Thu May  9 20:24:20 2024, max compression
+gzip compressed data, was "cellxgene-schema-5.0.4.tar", last modified: Tue May 14 18:08:21 2024, max compression
```

## Comparing `cellxgene-schema-5.0.3.tar` & `cellxgene-schema-5.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-09 20:24:20.833459 cellxgene-schema-5.0.3/
--rw-r--r--   0 trentsmith   (502) staff       (20)     1098 2022-06-01 19:47:22.000000 cellxgene-schema-5.0.3/LICENSE.txt
--rw-r--r--   0 trentsmith   (502) staff       (20)      120 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/MANIFEST.in
--rw-r--r--   0 trentsmith   (502) staff       (20)      701 2024-05-09 20:24:20.833561 cellxgene-schema-5.0.3/PKG-INFO
-drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-09 20:24:20.828253 cellxgene-schema-5.0.3/cellxgene_schema/
--rw-r--r--   0 trentsmith   (502) staff       (20)       22 2024-05-09 20:23:37.000000 cellxgene-schema-5.0.3/cellxgene_schema/__init__.py
--rw-r--r--   0 trentsmith   (502) staff       (20)     3902 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/cli.py
--rw-r--r--   0 trentsmith   (502) staff       (20)      493 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/env.py
--rw-r--r--   0 trentsmith   (502) staff       (20)     3304 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/gencode.py
-drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-09 20:24:20.832880 cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/
--rw-r--r--   0 trentsmith   (502) staff       (20)      714 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/genes_ercc.csv.gz
--rw-r--r--   0 trentsmith   (502) staff       (20)   673926 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/genes_homo_sapiens.csv.gz
--rw-r--r--   0 trentsmith   (502) staff       (20)   599259 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/genes_mus_musculus.csv.gz
--rw-r--r--   0 trentsmith   (502) staff       (20)      171 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/genes_sars_cov_2.csv.gz
--rw-r--r--   0 trentsmith   (502) staff       (20)    14201 2024-05-09 19:20:45.000000 cellxgene-schema-5.0.3/cellxgene_schema/migrate.py
--rw-r--r--   0 trentsmith   (502) staff       (20)     2774 2023-09-18 18:32:37.000000 cellxgene-schema-5.0.3/cellxgene_schema/remove_labels.py
--rw-r--r--   0 trentsmith   (502) staff       (20)      522 2023-09-18 18:32:37.000000 cellxgene-schema-5.0.3/cellxgene_schema/schema.py
-drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-09 20:24:20.833089 cellxgene-schema-5.0.3/cellxgene_schema/schema_definitions/
--rw-r--r--   0 trentsmith   (502) staff       (20)    28970 2024-04-29 23:23:16.000000 cellxgene-schema-5.0.3/cellxgene_schema/schema_definitions/schema_definition.yaml
--rw-r--r--   0 trentsmith   (502) staff       (20)     6738 2024-03-08 00:33:50.000000 cellxgene-schema-5.0.3/cellxgene_schema/utils.py
--rw-r--r--   0 trentsmith   (502) staff       (20)    90667 2024-05-09 20:23:37.000000 cellxgene-schema-5.0.3/cellxgene_schema/validate.py
--rw-r--r--   0 trentsmith   (502) staff       (20)    15528 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/write_labels.py
-drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-09 20:24:20.829627 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/
--rw-r--r--   0 trentsmith   (502) staff       (20)      701 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/PKG-INFO
--rw-r--r--   0 trentsmith   (502) staff       (20)      899 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/SOURCES.txt
--rw-r--r--   0 trentsmith   (502) staff       (20)        1 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/dependency_links.txt
--rw-r--r--   0 trentsmith   (502) staff       (20)       69 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/entry_points.txt
--rw-r--r--   0 trentsmith   (502) staff       (20)        1 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/not-zip-safe
--rw-r--r--   0 trentsmith   (502) staff       (20)      189 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/requires.txt
--rw-r--r--   0 trentsmith   (502) staff       (20)       17 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/top_level.txt
--rw-r--r--   0 trentsmith   (502) staff       (20)      276 2024-05-09 19:20:45.000000 cellxgene-schema-5.0.3/requirements.txt
--rw-r--r--   0 trentsmith   (502) staff       (20)       70 2024-05-09 20:24:20.833822 cellxgene-schema-5.0.3/setup.cfg
--rw-r--r--   0 trentsmith   (502) staff       (20)     1224 2024-05-09 20:23:37.000000 cellxgene-schema-5.0.3/setup.py
+drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-14 18:08:21.898356 cellxgene-schema-5.0.4/
+-rw-r--r--   0 trentsmith   (502) staff       (20)     1098 2022-06-01 19:47:22.000000 cellxgene-schema-5.0.4/LICENSE.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)      120 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.4/MANIFEST.in
+-rw-r--r--   0 trentsmith   (502) staff       (20)      701 2024-05-14 18:08:21.898431 cellxgene-schema-5.0.4/PKG-INFO
+drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-14 18:08:21.895821 cellxgene-schema-5.0.4/cellxgene_schema/
+-rw-r--r--   0 trentsmith   (502) staff       (20)       22 2024-05-14 18:07:58.000000 cellxgene-schema-5.0.4/cellxgene_schema/__init__.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)     3902 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.4/cellxgene_schema/cli.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)      493 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.4/cellxgene_schema/env.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)     3304 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.4/cellxgene_schema/gencode.py
+drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-14 18:08:21.898055 cellxgene-schema-5.0.4/cellxgene_schema/gencode_files/
+-rw-r--r--   0 trentsmith   (502) staff       (20)      714 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.4/cellxgene_schema/gencode_files/genes_ercc.csv.gz
+-rw-r--r--   0 trentsmith   (502) staff       (20)   673926 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.4/cellxgene_schema/gencode_files/genes_homo_sapiens.csv.gz
+-rw-r--r--   0 trentsmith   (502) staff       (20)   599259 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.4/cellxgene_schema/gencode_files/genes_mus_musculus.csv.gz
+-rw-r--r--   0 trentsmith   (502) staff       (20)      171 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.4/cellxgene_schema/gencode_files/genes_sars_cov_2.csv.gz
+-rw-r--r--   0 trentsmith   (502) staff       (20)    14201 2024-05-10 19:09:46.000000 cellxgene-schema-5.0.4/cellxgene_schema/migrate.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)     2774 2023-09-18 18:32:37.000000 cellxgene-schema-5.0.4/cellxgene_schema/remove_labels.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)      522 2023-09-18 18:32:37.000000 cellxgene-schema-5.0.4/cellxgene_schema/schema.py
+drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-14 18:08:21.898207 cellxgene-schema-5.0.4/cellxgene_schema/schema_definitions/
+-rw-r--r--   0 trentsmith   (502) staff       (20)    28970 2024-04-29 23:23:16.000000 cellxgene-schema-5.0.4/cellxgene_schema/schema_definitions/schema_definition.yaml
+-rw-r--r--   0 trentsmith   (502) staff       (20)     6738 2024-05-10 21:23:53.000000 cellxgene-schema-5.0.4/cellxgene_schema/utils.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)    90822 2024-05-14 17:41:37.000000 cellxgene-schema-5.0.4/cellxgene_schema/validate.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)    15528 2024-05-10 19:09:46.000000 cellxgene-schema-5.0.4/cellxgene_schema/write_labels.py
+drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-14 18:08:21.896843 cellxgene-schema-5.0.4/cellxgene_schema.egg-info/
+-rw-r--r--   0 trentsmith   (502) staff       (20)      701 2024-05-14 18:08:21.000000 cellxgene-schema-5.0.4/cellxgene_schema.egg-info/PKG-INFO
+-rw-r--r--   0 trentsmith   (502) staff       (20)      899 2024-05-14 18:08:21.000000 cellxgene-schema-5.0.4/cellxgene_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)        1 2024-05-14 18:08:21.000000 cellxgene-schema-5.0.4/cellxgene_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)       69 2024-05-14 18:08:21.000000 cellxgene-schema-5.0.4/cellxgene_schema.egg-info/entry_points.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)        1 2024-05-14 18:08:21.000000 cellxgene-schema-5.0.4/cellxgene_schema.egg-info/not-zip-safe
+-rw-r--r--   0 trentsmith   (502) staff       (20)      189 2024-05-14 18:08:21.000000 cellxgene-schema-5.0.4/cellxgene_schema.egg-info/requires.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)       17 2024-05-14 18:08:21.000000 cellxgene-schema-5.0.4/cellxgene_schema.egg-info/top_level.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)      276 2024-05-09 22:30:30.000000 cellxgene-schema-5.0.4/requirements.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)       70 2024-05-14 18:08:21.898670 cellxgene-schema-5.0.4/setup.cfg
+-rw-r--r--   0 trentsmith   (502) staff       (20)     1224 2024-05-14 18:07:58.000000 cellxgene-schema-5.0.4/setup.py
```

### Comparing `cellxgene-schema-5.0.3/LICENSE.txt` & `cellxgene-schema-5.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/PKG-INFO` & `cellxgene-schema-5.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-schema
-Version: 5.0.3
+Version: 5.0.4
 Summary: Tool for applying and validating cellxgene integration schema to single cell datasets
 Home-page: https://github.com/chanzuckerberg/single-cell-curation
 Author: Chan Zuckerberg Initiative
 Author-email: cellxgene@chanzuckerberg.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema/cli.py` & `cellxgene-schema-5.0.4/cellxgene_schema/cli.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema/gencode.py` & `cellxgene-schema-5.0.4/cellxgene_schema/gencode.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/genes_ercc.csv.gz` & `cellxgene-schema-5.0.4/cellxgene_schema/gencode_files/genes_ercc.csv.gz`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/genes_homo_sapiens.csv.gz` & `cellxgene-schema-5.0.4/cellxgene_schema/gencode_files/genes_homo_sapiens.csv.gz`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/genes_mus_musculus.csv.gz` & `cellxgene-schema-5.0.4/cellxgene_schema/gencode_files/genes_mus_musculus.csv.gz`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema/migrate.py` & `cellxgene-schema-5.0.4/cellxgene_schema/migrate.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema/remove_labels.py` & `cellxgene-schema-5.0.4/cellxgene_schema/remove_labels.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema/schema.py` & `cellxgene-schema-5.0.4/cellxgene_schema/schema.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema/schema_definitions/schema_definition.yaml` & `cellxgene-schema-5.0.4/cellxgene_schema/schema_definitions/schema_definition.yaml`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema/utils.py` & `cellxgene-schema-5.0.4/cellxgene_schema/utils.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema/validate.py` & `cellxgene-schema-5.0.4/cellxgene_schema/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Dict, List, Mapping, Optional, Union
 
 import anndata
 import matplotlib.colors as mcolors
 import numpy as np
 import pandas as pd
 import scipy
+from anndata._core.sparse_dataset import SparseDataset
 from cellxgene_ontology_guide.ontology_parser import OntologyParser
 from pandas.core.computation.ops import UndefinedVariableError
 from scipy import sparse
 
 from . import gencode, schema
 from .utils import SPARSE_MATRIX_TYPES, get_matrix_format, getattr_anndata, read_h5ad
 
@@ -1218,24 +1219,28 @@
         if has_row_of_zeros:
             self._raw_layer_exists = False
             self.errors.append("Each cell must have at least one non-zero value in its row in the raw matrix.")
         if has_invalid_nonzero_value:
             self._raw_layer_exists = False
             self.errors.append("All non-zero values in raw matrix must be positive integers of type numpy.float32.")
 
-    def _validate_raw_data_with_in_tissue_0(self, x: Union[np.ndarray, sparse.spmatrix], is_sparse_matrix: bool):
+    def _validate_raw_data_with_in_tissue_0(
+        self, x: Union[np.ndarray, sparse.spmatrix, SparseDataset], is_sparse_matrix: bool
+    ):
         """
         Special case validation checks for Visium data with is_single = True and in_tissue column in obs where in_tissue
         has at least one value 0. Static matrix size of 4992 rows, so chunking is not required.
 
         :param x: raw matrix
         :param is_sparse_matrix: bool indicating if the matrix is sparse {csc, csr, coo}
         """
         has_tissue_0_non_zero_row = False
         has_tissue_1_zero_row = False
+        if isinstance(x, SparseDataset):
+            x = x.to_memory()
         if is_sparse_matrix:
             nonzero_row_indices, _ = x.nonzero()
         else:  # must be dense matrix
             nonzero_row_indices = np.where(np.any(x != 0, axis=1))[0]
         for i in range(x.shape[0]):
             if not has_tissue_0_non_zero_row and i in nonzero_row_indices and self.adata.obs["in_tissue"][i] == 0:
                 has_tissue_0_non_zero_row = True
```

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema/write_labels.py` & `cellxgene-schema-5.0.4/cellxgene_schema/write_labels.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema.egg-info/PKG-INFO` & `cellxgene-schema-5.0.4/cellxgene_schema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-schema
-Version: 5.0.3
+Version: 5.0.4
 Summary: Tool for applying and validating cellxgene integration schema to single cell datasets
 Home-page: https://github.com/chanzuckerberg/single-cell-curation
 Author: Chan Zuckerberg Initiative
 Author-email: cellxgene@chanzuckerberg.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cellxgene-schema-5.0.3/cellxgene_schema.egg-info/SOURCES.txt` & `cellxgene-schema-5.0.4/cellxgene_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.3/setup.py` & `cellxgene-schema-5.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("requirements.txt") as fh:
     requirements = fh.read().splitlines()
 
 setup(
     name="cellxgene-schema",
-    version="5.0.3",
+    version="5.0.4",
     url="https://github.com/chanzuckerberg/single-cell-curation",
     license="MIT",
     author="Chan Zuckerberg Initiative",
     author_email="cellxgene@chanzuckerberg.com",
     description="Tool for applying and validating cellxgene integration schema to single cell datasets",
     long_description="Tool for applying and validating cellxgene integration schema to single cell datasets",
     install_requires=requirements,
```

