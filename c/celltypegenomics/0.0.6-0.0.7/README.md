# Comparing `tmp/celltypegenomics-0.0.6.tar.gz` & `tmp/celltypegenomics-0.0.7.tar.gz`

## Comparing `celltypegenomics-0.0.6.tar` & `celltypegenomics-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/README.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/requirements.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/__init__.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/celltypegenomics.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/test_celltypegenomics.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/test_integration.py
--rw-r--r--   0        0        0    23364 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/data/heca_cell_type_to_ensembl.json
--rw-r--r--   0        0        0  1136374 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/data/hpa_cell_types_to_ensembl.json
--rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/data/hpa_marker_genes_cell_types_to_ensembl.json
--rw-r--r--   0        0        0   332831 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/data/hpa_tissue__to_ensembl.json
--rw-r--r--   0        0        0   383078 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/data/protein_atlas_ensembl_ids.json
--rw-r--r--   0        0        0  1469205 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/data/tissue_and_cell_types_to_ensembl.json
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/LICENSE
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/README.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/README.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/requirements.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/src/celltypegenomics/__init__.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/src/celltypegenomics/celltypegenomics.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/src/celltypegenomics/test_celltypegenomics.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/src/celltypegenomics/test_integration.py
+-rw-r--r--   0        0        0    23364 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/src/celltypegenomics/data/heca_cell_types_to_ensembl.json
+-rw-r--r--   0        0        0  1136374 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/src/celltypegenomics/data/hpa_cell_types_to_ensembl.json
+-rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/src/celltypegenomics/data/hpa_marker_genes_cell_types_to_ensembl.json
+-rw-r--r--   0        0        0   332831 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/src/celltypegenomics/data/hpa_tissue_to_ensembl.json
+-rw-r--r--   0        0        0   383078 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/src/celltypegenomics/data/protein_atlas_ensembl_ids.json
+-rw-r--r--   0        0        0  1469205 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/src/celltypegenomics/data/tissue_and_cell_types_to_ensembl.json
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 celltypegenomics-0.0.7/PKG-INFO
```

### Comparing `celltypegenomics-0.0.6/src/celltypegenomics/celltypegenomics.py` & `celltypegenomics-0.0.7/src/celltypegenomics/celltypegenomics.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,22 +59,25 @@
     for cell_type, adj_p_value in zip(fisher_test_results.keys(), pvals_corrected):
         fisher_test_results[cell_type]["adjusted_p_value"] = adj_p_value
     
     # Convert the results to a pandas DataFrame and return
     df = pd.DataFrame.from_dict(fisher_test_results, orient='index')
 
     # Sort the DataFrame by p-value in ascending order
+    df_sorted = df.sort_values(by='p_value', ascending=True)
+
+    # Sort the DataFrame by p-value in ascending order
     df_sorted = df.sort_values(by='adjusted_p_value', ascending=True)
 
     df_filtered = df_sorted[df_sorted['adjusted_p_value'] <= alpha]
 
     return df_filtered
 
 if __name__ == "__main__":
     # Test the function (this part will not be executed when the module is imported)
     test_ensembl_ids = ['ENSG00000182389', 'ENSG00000078081', 'ENSG00000084073', 'ENSG00000119632', 'ENSG00000161267']  # Example Ensembl IDs
     # Alpha used for adjusted p-value
-    alpha = 0.05
+    alpha = 1.0
     print(celltypefishertest(test_ensembl_ids, alpha)) # use the default cell type list from HPA (from proteinatlas.tsv)
     print(celltypefishertest(test_ensembl_ids, alpha, heca=True)) # use the cell type list from hECA
     print(celltypefishertest(test_ensembl_ids, alpha, hpa_marker_genes=True)) # use the cell type list from HPA marker genes
     print(celltypefishertest(test_ensembl_ids, alpha, tissue=True)) # use the cell type list from tissue
```

### Comparing `celltypegenomics-0.0.6/src/celltypegenomics/test_celltypegenomics.py` & `celltypegenomics-0.0.7/src/celltypegenomics/test_celltypegenomics.py`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.6/src/celltypegenomics/test_integration.py` & `celltypegenomics-0.0.7/src/celltypegenomics/test_integration.py`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.6/src/celltypegenomics/data/heca_cell_type_to_ensembl.json` & `celltypegenomics-0.0.7/src/celltypegenomics/data/heca_cell_types_to_ensembl.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.6/src/celltypegenomics/data/hpa_cell_types_to_ensembl.json` & `celltypegenomics-0.0.7/src/celltypegenomics/data/hpa_cell_types_to_ensembl.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.6/src/celltypegenomics/data/hpa_marker_genes_cell_types_to_ensembl.json` & `celltypegenomics-0.0.7/src/celltypegenomics/data/hpa_marker_genes_cell_types_to_ensembl.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.6/src/celltypegenomics/data/hpa_tissue__to_ensembl.json` & `celltypegenomics-0.0.7/src/celltypegenomics/data/hpa_tissue_to_ensembl.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.6/src/celltypegenomics/data/protein_atlas_ensembl_ids.json` & `celltypegenomics-0.0.7/src/celltypegenomics/data/protein_atlas_ensembl_ids.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.6/src/celltypegenomics/data/tissue_and_cell_types_to_ensembl.json` & `celltypegenomics-0.0.7/src/celltypegenomics/data/tissue_and_cell_types_to_ensembl.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.6/LICENSE` & `celltypegenomics-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.6/README.md` & `celltypegenomics-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ## Key Functionality
 - **Gene Analysis:** Analyzes a list of gene Ensembl IDs and returns a sorted pandas DataFrame, highlighting genes that are potentially over- or under-represented in certain cell types.
 - **Data Source:** Leverages the comprehensive gene expression data available from the Human Protein Atlas (HPA) and the human Ensemble Cell Atlas (hECA).
 
 ## Installation
 To install CellTypeGenomics, run the following command in your terminal:
 ```bash
-pip install celltypegenomics
+pip install --upgrade celltypegenomics
 ```
 
 ## Usage
 Here's how to use the CellTypeGenomics package to analyze your gene list with numerical Human Protein Atlas (HPA) marker genes:
 
 ```python
 from celltypegenomics import celltypefishertest
```

### Comparing `celltypegenomics-0.0.6/pyproject.toml` & `celltypegenomics-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "celltypegenomics"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Lars Føleide", email="larsfole@stud.ntnu.no" },
 ]
 description = "Package for cell type genomics"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `celltypegenomics-0.0.6/PKG-INFO` & `celltypegenomics-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: celltypegenomics
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package for cell type genomics
 Project-URL: Homepage, https://github.com/Zyron/CellTypeGenomics
 Project-URL: Bug Tracker, https://github.com/Zyron/CellTypeGenomics/issues
 Author-email: Lars Føleide <larsfole@stud.ntnu.no>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,15 +25,15 @@
 ## Key Functionality
 - **Gene Analysis:** Analyzes a list of gene Ensembl IDs and returns a sorted pandas DataFrame, highlighting genes that are potentially over- or under-represented in certain cell types.
 - **Data Source:** Leverages the comprehensive gene expression data available from the Human Protein Atlas (HPA) and the human Ensemble Cell Atlas (hECA).
 
 ## Installation
 To install CellTypeGenomics, run the following command in your terminal:
 ```bash
-pip install celltypegenomics
+pip install --upgrade celltypegenomics
 ```
 
 ## Usage
 Here's how to use the CellTypeGenomics package to analyze your gene list with numerical Human Protein Atlas (HPA) marker genes:
 
 ```python
 from celltypegenomics import celltypefishertest
```

