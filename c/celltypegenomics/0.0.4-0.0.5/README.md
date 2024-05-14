# Comparing `tmp/celltypegenomics-0.0.4.tar.gz` & `tmp/celltypegenomics-0.0.5.tar.gz`

## Comparing `celltypegenomics-0.0.4.tar` & `celltypegenomics-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 celltypegenomics-0.0.4/requirements.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 celltypegenomics-0.0.4/src/celltypegenomics/__init__.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 celltypegenomics-0.0.4/src/celltypegenomics/celltypegenomics.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 celltypegenomics-0.0.4/src/celltypegenomics/test_celltypegenomics.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 celltypegenomics-0.0.4/src/celltypegenomics/test_integration.py
--rw-r--r--   0        0        0  1469205 2020-02-02 00:00:00.000000 celltypegenomics-0.0.4/src/celltypegenomics/data/cell_types_to_ensembl.json
--rw-r--r--   0        0        0   383078 2020-02-02 00:00:00.000000 celltypegenomics-0.0.4/src/celltypegenomics/data/protein_atlas_ensembl_ids.json
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 celltypegenomics-0.0.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 celltypegenomics-0.0.4/LICENSE
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 celltypegenomics-0.0.4/README.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 celltypegenomics-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 celltypegenomics-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/README.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/requirements.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/__init__.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/celltypegenomics.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/test_celltypegenomics.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/test_integration.py
+-rw-r--r--   0        0        0    23364 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/data/heca_cell_type_to_ensembl.json
+-rw-r--r--   0        0        0  1136374 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/data/hpa_cell_types_to_ensembl.json
+-rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/data/hpa_marker_genes_cell_types_to_ensembl.json
+-rw-r--r--   0        0        0   332831 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/data/hpa_tissue__to_ensembl.json
+-rw-r--r--   0        0        0   383078 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/data/protein_atlas_ensembl_ids.json
+-rw-r--r--   0        0        0  1469205 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/data/tissue_and_cell_types_to_ensembl.json
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/PKG-INFO
```

### Comparing `celltypegenomics-0.0.4/src/celltypegenomics/celltypegenomics.py` & `celltypegenomics-0.0.5/src/celltypegenomics/celltypegenomics.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,22 +2,36 @@
 #pip install scipy statsmodels
 import json
 import pandas as pd
 import pkg_resources
 from scipy.stats import fisher_exact
 from statsmodels.stats.multitest import multipletests
 
-def celltypefishertest(ensembl_ids, alpha=0.05):
+def celltypefishertest(ensembl_ids, alpha=0.05, heca=None, hpa_marker_genes=None, tissue=None):
     # Get the correct path for the JSON files
-    cell_types_to_ensembl_path = pkg_resources.resource_filename('celltypegenomics', 'data/cell_types_to_ensembl.json')
+    hpa_cell_types_to_ensembl_path = pkg_resources.resource_filename('celltypegenomics', 'data/hpa_cell_types_to_ensembl.json')
+    heca_cell_types_to_ensembl_path = pkg_resources.resource_filename('celltypegenomics', 'data/heca_cell_types_to_ensembl.json')
+    hpa_marker_genes_cell_types_to_ensembl_path = pkg_resources.resource_filename('celltypegenomics', 'data/hpa_marker_genes_cell_types_to_ensembl.json')
+    tissue_cell_types_to_ensembl_path = pkg_resources.resource_filename('celltypegenomics', 'data/tissue_to_ensembl.json')
     protein_atlas_ensembl_ids_path = pkg_resources.resource_filename('celltypegenomics', 'data/protein_atlas_ensembl_ids.json')
     
     # Read necessary JSON files
-    with open(cell_types_to_ensembl_path, 'r') as f:
-        cell_types_to_ensembl = json.load(f)
+    if (heca):
+        with open(heca_cell_types_to_ensembl_path, 'r') as f:
+            cell_types_to_ensembl = json.load(f)
+    elif (hpa_marker_genes):
+        with open(hpa_marker_genes_cell_types_to_ensembl_path, 'r') as f:
+            cell_types_to_ensembl = json.load(f)
+    elif (tissue):
+        with open(tissue_cell_types_to_ensembl_path, 'r') as f:
+            cell_types_to_ensembl = json.load(f)
+    else:
+        with open(hpa_cell_types_to_ensembl_path, 'r') as f:
+            cell_types_to_ensembl = json.load(f)
+    
     with open(protein_atlas_ensembl_ids_path, 'r') as f:
         protein_atlas_ensembl_ids = json.load(f)
     
     fisher_test_results = {}
     
     for cell_type, genes in cell_types_to_ensembl.items():
         count_in_both = len(set(ensembl_ids) & set(genes))
@@ -54,8 +68,11 @@
     return df_sorted
 
 if __name__ == "__main__":
     # Test the function (this part will not be executed when the module is imported)
     test_ensembl_ids = ['ENSG00000182389', 'ENSG00000078081', 'ENSG00000084073', 'ENSG00000119632', 'ENSG00000161267']  # Example Ensembl IDs
     # Alpha used for adjusted p-value
     alpha = 0.05
-    print(celltypefishertest(test_ensembl_ids, alpha))
+    print(celltypefishertest(test_ensembl_ids, alpha)) # use the default cell type list from HPA (from proteinatlas.tsv)
+    print(celltypefishertest(test_ensembl_ids, alpha, heca=True)) # use the cell type list from hECA
+    print(celltypefishertest(test_ensembl_ids, alpha, hpa_marker_genes=True)) # use the cell type list from HPA marker genes
+    print(celltypefishertest(test_ensembl_ids, alpha, tissue=True)) # use the cell type list from tissue
```

### Comparing `celltypegenomics-0.0.4/src/celltypegenomics/test_celltypegenomics.py` & `celltypegenomics-0.0.5/src/celltypegenomics/test_celltypegenomics.py`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.4/src/celltypegenomics/test_integration.py` & `celltypegenomics-0.0.5/src/celltypegenomics/test_integration.py`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.4/src/celltypegenomics/data/cell_types_to_ensembl.json` & `celltypegenomics-0.0.5/src/celltypegenomics/data/tissue_and_cell_types_to_ensembl.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.4/src/celltypegenomics/data/protein_atlas_ensembl_ids.json` & `celltypegenomics-0.0.5/src/celltypegenomics/data/protein_atlas_ensembl_ids.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.4/LICENSE` & `celltypegenomics-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.4/pyproject.toml` & `celltypegenomics-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "celltypegenomics"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Lars Føleide", email="larsfole@stud.ntnu.no" },
 ]
 description = "Package for cell type genomics"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

