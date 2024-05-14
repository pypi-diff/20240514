# Comparing `tmp/celltypegenomics-0.0.5.tar.gz` & `tmp/celltypegenomics-0.0.6.tar.gz`

## Comparing `celltypegenomics-0.0.5.tar` & `celltypegenomics-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/README.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/requirements.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/__init__.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/celltypegenomics.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/test_celltypegenomics.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/test_integration.py
--rw-r--r--   0        0        0    23364 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/data/heca_cell_type_to_ensembl.json
--rw-r--r--   0        0        0  1136374 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/data/hpa_cell_types_to_ensembl.json
--rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/data/hpa_marker_genes_cell_types_to_ensembl.json
--rw-r--r--   0        0        0   332831 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/data/hpa_tissue__to_ensembl.json
--rw-r--r--   0        0        0   383078 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/data/protein_atlas_ensembl_ids.json
--rw-r--r--   0        0        0  1469205 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/src/celltypegenomics/data/tissue_and_cell_types_to_ensembl.json
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/LICENSE
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/README.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 celltypegenomics-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/README.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/requirements.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/__init__.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/celltypegenomics.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/test_celltypegenomics.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/test_integration.py
+-rw-r--r--   0        0        0    23364 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/data/heca_cell_type_to_ensembl.json
+-rw-r--r--   0        0        0  1136374 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/data/hpa_cell_types_to_ensembl.json
+-rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/data/hpa_marker_genes_cell_types_to_ensembl.json
+-rw-r--r--   0        0        0   332831 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/data/hpa_tissue__to_ensembl.json
+-rw-r--r--   0        0        0   383078 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/data/protein_atlas_ensembl_ids.json
+-rw-r--r--   0        0        0  1469205 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/src/celltypegenomics/data/tissue_and_cell_types_to_ensembl.json
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 celltypegenomics-0.0.6/PKG-INFO
```

### Comparing `celltypegenomics-0.0.5/src/celltypegenomics/celltypegenomics.py` & `celltypegenomics-0.0.6/src/celltypegenomics/celltypegenomics.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,17 +59,19 @@
     for cell_type, adj_p_value in zip(fisher_test_results.keys(), pvals_corrected):
         fisher_test_results[cell_type]["adjusted_p_value"] = adj_p_value
     
     # Convert the results to a pandas DataFrame and return
     df = pd.DataFrame.from_dict(fisher_test_results, orient='index')
 
     # Sort the DataFrame by p-value in ascending order
-    df_sorted = df.sort_values(by='p_value', ascending=True)
+    df_sorted = df.sort_values(by='adjusted_p_value', ascending=True)
 
-    return df_sorted
+    df_filtered = df_sorted[df_sorted['adjusted_p_value'] <= alpha]
+
+    return df_filtered
 
 if __name__ == "__main__":
     # Test the function (this part will not be executed when the module is imported)
     test_ensembl_ids = ['ENSG00000182389', 'ENSG00000078081', 'ENSG00000084073', 'ENSG00000119632', 'ENSG00000161267']  # Example Ensembl IDs
     # Alpha used for adjusted p-value
     alpha = 0.05
     print(celltypefishertest(test_ensembl_ids, alpha)) # use the default cell type list from HPA (from proteinatlas.tsv)
```

### Comparing `celltypegenomics-0.0.5/src/celltypegenomics/test_celltypegenomics.py` & `celltypegenomics-0.0.6/src/celltypegenomics/test_celltypegenomics.py`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.5/src/celltypegenomics/test_integration.py` & `celltypegenomics-0.0.6/src/celltypegenomics/test_integration.py`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.5/src/celltypegenomics/data/heca_cell_type_to_ensembl.json` & `celltypegenomics-0.0.6/src/celltypegenomics/data/heca_cell_type_to_ensembl.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.5/src/celltypegenomics/data/hpa_cell_types_to_ensembl.json` & `celltypegenomics-0.0.6/src/celltypegenomics/data/hpa_cell_types_to_ensembl.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.5/src/celltypegenomics/data/hpa_marker_genes_cell_types_to_ensembl.json` & `celltypegenomics-0.0.6/src/celltypegenomics/data/hpa_marker_genes_cell_types_to_ensembl.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.5/src/celltypegenomics/data/hpa_tissue__to_ensembl.json` & `celltypegenomics-0.0.6/src/celltypegenomics/data/hpa_tissue__to_ensembl.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.5/src/celltypegenomics/data/protein_atlas_ensembl_ids.json` & `celltypegenomics-0.0.6/src/celltypegenomics/data/protein_atlas_ensembl_ids.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.5/src/celltypegenomics/data/tissue_and_cell_types_to_ensembl.json` & `celltypegenomics-0.0.6/src/celltypegenomics/data/tissue_and_cell_types_to_ensembl.json`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.5/LICENSE` & `celltypegenomics-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.5/README.md` & `celltypegenomics-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `celltypegenomics-0.0.5/pyproject.toml` & `celltypegenomics-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "celltypegenomics"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Lars Føleide", email="larsfole@stud.ntnu.no" },
 ]
 description = "Package for cell type genomics"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `celltypegenomics-0.0.5/PKG-INFO` & `celltypegenomics-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: celltypegenomics
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package for cell type genomics
 Project-URL: Homepage, https://github.com/Zyron/CellTypeGenomics
 Project-URL: Bug Tracker, https://github.com/Zyron/CellTypeGenomics/issues
 Author-email: Lars Føleide <larsfole@stud.ntnu.no>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

