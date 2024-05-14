# Comparing `tmp/glytrait-0.1.4.tar.gz` & `tmp/glytrait-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glytrait-0.1.4.tar", max compression
+gzip compressed data, was "glytrait-0.1.5.tar", max compression
```

## Comparing `glytrait-0.1.4.tar` & `glytrait-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1063 2023-06-01 11:46:23.327576 glytrait-0.1.4/LICENSE
--rw-r--r--   0        0        0    14358 2024-04-25 13:00:54.127735 glytrait-0.1.4/README.md
--rw-r--r--   0        0        0     1406 2024-04-28 07:04:03.629136 glytrait-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      118 2024-04-28 07:06:14.279101 glytrait-0.1.4/src/glytrait/__init__.py
--rw-r--r--   0        0        0    18661 2024-04-24 16:52:01.574358 glytrait-0.1.4/src/glytrait/api.py
--rw-r--r--   0        0        0     8032 2024-04-24 15:43:00.391548 glytrait-0.1.4/src/glytrait/cli.py
--rw-r--r--   0        0        0     2640 2024-04-20 16:02:21.883776 glytrait-0.1.4/src/glytrait/data_export.py
--rw-r--r--   0        0        0    12490 2024-04-24 12:35:20.623069 glytrait-0.1.4/src/glytrait/data_input.py
--rw-r--r--   0        0        0      923 2023-12-30 06:44:57.217908 glytrait-0.1.4/src/glytrait/data_type.py
--rw-r--r--   0        0        0      812 2024-04-14 11:59:08.463548 glytrait-0.1.4/src/glytrait/exception.py
--rw-r--r--   0        0        0    26284 2024-04-24 12:35:20.622266 glytrait-0.1.4/src/glytrait/formula.py
--rw-r--r--   0        0        0    13016 2024-04-24 12:35:20.622716 glytrait-0.1.4/src/glytrait/glycan.py
--rw-r--r--   0        0        0    18326 2024-04-24 12:35:20.623387 glytrait-0.1.4/src/glytrait/meta_property.py
--rw-r--r--   0        0        0     6664 2024-04-14 11:59:08.464921 glytrait-0.1.4/src/glytrait/post_filtering.py
--rw-r--r--   0        0        0     3687 2024-04-24 12:35:20.623765 glytrait-0.1.4/src/glytrait/preprocessing.py
--rw-r--r--   0        0        0     7931 2024-04-24 12:35:20.624129 glytrait-0.1.4/src/glytrait/resources/comp_formula.txt
--rw-r--r--   0        0        0    54374 2024-04-24 12:35:20.624453 glytrait-0.1.4/src/glytrait/resources/struc_formula.txt
--rw-r--r--   0        0        0     4834 2024-04-24 12:35:20.624749 glytrait-0.1.4/src/glytrait/stat.py
--rw-r--r--   0        0        0     1665 2023-12-30 06:44:57.220052 glytrait-0.1.4/src/glytrait/trait.py
--rw-r--r--   0        0        0    14991 1970-01-01 00:00:00.000000 glytrait-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-01 11:46:23.327576 glytrait-0.1.5/LICENSE
+-rw-r--r--   0        0        0    14774 2024-04-29 03:43:46.462080 glytrait-0.1.5/README.md
+-rw-r--r--   0        0        0     1406 2024-05-14 11:24:08.310318 glytrait-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-05-14 11:24:01.010739 glytrait-0.1.5/src/glytrait/__init__.py
+-rw-r--r--   0        0        0    20638 2024-05-14 11:15:11.560250 glytrait-0.1.5/src/glytrait/api.py
+-rw-r--r--   0        0        0     7998 2024-05-14 08:06:17.534042 glytrait-0.1.5/src/glytrait/cli.py
+-rw-r--r--   0        0        0     2640 2024-04-20 16:02:21.883776 glytrait-0.1.5/src/glytrait/data_export.py
+-rw-r--r--   0        0        0    12490 2024-04-24 12:35:20.623069 glytrait-0.1.5/src/glytrait/data_input.py
+-rw-r--r--   0        0        0      923 2023-12-30 06:44:57.217908 glytrait-0.1.5/src/glytrait/data_type.py
+-rw-r--r--   0        0        0      812 2024-04-14 11:59:08.463548 glytrait-0.1.5/src/glytrait/exception.py
+-rw-r--r--   0        0        0    26273 2024-05-14 08:33:00.448535 glytrait-0.1.5/src/glytrait/formula.py
+-rw-r--r--   0        0        0    13016 2024-04-24 12:35:20.622716 glytrait-0.1.5/src/glytrait/glycan.py
+-rw-r--r--   0        0        0    18326 2024-04-24 12:35:20.623387 glytrait-0.1.5/src/glytrait/meta_property.py
+-rw-r--r--   0        0        0     6664 2024-04-14 11:59:08.464921 glytrait-0.1.5/src/glytrait/post_filtering.py
+-rw-r--r--   0        0        0     3687 2024-04-24 12:35:20.623765 glytrait-0.1.5/src/glytrait/preprocessing.py
+-rw-r--r--   0        0        0     7931 2024-04-24 12:35:20.624129 glytrait-0.1.5/src/glytrait/resources/comp_formula.txt
+-rw-r--r--   0        0        0    54374 2024-04-24 12:35:20.624453 glytrait-0.1.5/src/glytrait/resources/struc_formula.txt
+-rw-r--r--   0        0        0     4834 2024-04-24 12:35:20.624749 glytrait-0.1.5/src/glytrait/stat.py
+-rw-r--r--   0        0        0     1665 2023-12-30 06:44:57.220052 glytrait-0.1.5/src/glytrait/trait.py
+-rw-r--r--   0        0        0    15396 1970-01-01 00:00:00.000000 glytrait-0.1.5/PKG-INFO
```

### Comparing `glytrait-0.1.4/LICENSE` & `glytrait-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/README.md` & `glytrait-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -238,14 +238,25 @@
 The "GlycanID" column should contain all glycan IDs in the abundance file.
 The "Structure" column should contain the structure strings of the glycans.
 For now, only the GlycoCT format is supported.
 In the "composition" mode, the second column should be "Composition" instead of "Structure",
 and the composition strings should be used instead of the structure strings.
 Condensed format ("H3N4F1S1") is supported.
 
+The names of the abundance file and the structure (composition) file is not important, 
+i.e., it doesn't have to be "abundance.csv" and "structures.csv". 
+You could use any name you want, as long as the two files are passed in order,
+e.g.: 
+
+```shell
+glytrait experiment_1_15.csv serum_structures.csv
+#        ~~~~~~~~~~~~~~~~~~~ ~~~~~~~~~~~~~~~~~~~~
+#        the abundance file   the structure file
+```
+
 ### Specify the output path
 
 You might have noticed before that GlyTrait saves the output file to the same directory 
 as the abundance file with a "_glytrait" suffix.
 You can specify the output file path by using the "-o" or "--output-file" option:
 
 ```shell
```

### Comparing `glytrait-0.1.4/pyproject.toml` & `glytrait-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glytrait"
-version = "0.1.4"
+version = "0.1.5"
 description = "A tool for calculating derived traits for N-glycome"
 authors = ["fubin1999 <65430559+fubin1999@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/fubin1999/glytrait"
 keywords = ["bioinformatics", "glycomics", "biology"]
```

### Comparing `glytrait-0.1.4/src/glytrait/api.py` & `glytrait-0.1.5/src/glytrait/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from collections.abc import Iterable
 from functools import wraps
 from typing import cast, Literal, Optional, ClassVar, Any
 
 import pandas as pd
 from attrs import define, field
 
 from glytrait.data_type import (
     MetaPropertyTable,
     DerivedTraitTable,
     GroupSeries,
     AbundanceTable,
 )
 from glytrait.exception import GlyTraitError
-from glytrait.formula import load_default_formulas, TraitFormula
+from glytrait.formula import load_default_formulas, TraitFormula, parse_formulas
 from glytrait.data_input import GlyTraitInputData
 from glytrait.meta_property import build_meta_property_table
 from glytrait.post_filtering import post_filter
 from glytrait.preprocessing import preprocess
 from glytrait.trait import calcu_derived_trait
 from glytrait.stat import auto_test
 from glytrait.glycan import Structure, Composition
@@ -182,39 +183,43 @@
 GlycanDict = dict[str, Structure] | dict[str, Composition]
 
 
 @define
 class Experiment(_Workflow):
     """GlyTrait experiment.
 
-    Create an instance of this class with an abundance table and a structure series
+    Create an instance of this class with an GlyTraitInputData instance
     to perform all the steps in the GlyTrait workflow.
 
     Firstly, call the `preprocessed` method to filter glycans, impute missing values,
     and normalize the abundance.
-    Calling this method makes the `processed_abundance_table` attribute available.
+    Calling this method makes the `processed_abundance_table` and
+    `meta_property_table` attributes available.
+    The latter is a table of structural or compositional properties of glycans,
+    which is used to calculate derived traits.
 
-    Secondly, call the `extract_meta_properties` method.
-    This method generates a table of meta-properties for each glycan,
-    stored as the `meta_property_table` attribute.
-
-    Thirdly, call the `derive_traits` method to calculate all the derived traits.
+    Secondly, call the `derive_traits` method to calculate all the derived traits.
     The result table is stored as the `derived_trait_table` attribute.
 
-    Fourthly, call the `post_filter` method
+    Thirdly, call the `post_filter` method
     to remove invalid traits and highly correlated traits.
     The result table is stored as the `filtered_derived_trait_table` attribute.
 
     Finally, and optionally, call the `diff_analysis` method with a group series
     to perform differential analysis.
     The result is stored as the `diff_results` attribute.
 
+    Alternatively, you can call the `run_workflow` method to run the entire workflow.
+
+    If you want to try new formula expressions, use the `try_formulas` method.
+    Instead of saving the result as an attribute,
+    this method returns the result DataFrame or Series directly.
+
     Methods:
         preprocess: Preprocess the data.
-        extract_meta_properties: Extract meta properties.
         derive_traits: Calculate derived traits.
         post_filter: Post-filter the derived traits.
         diff_analysis: Perform differential analysis.
         derive_one_trait: Try a single trait formula.
         reset: Reset the workflow to the beginning (before `preprocess`).
         get_data: Get the data by name.
 
@@ -241,30 +246,27 @@
         ...    glycan_df=pd.read_csv("glycan_structure.csv"),
         ...    group_df=pd.read_csv("group.csv"),
         ...    mode="structure",
         )
         # `input_data` is a GlyTraitInputData instance.
         >>> experiment = Experiment(input_data)
         >>> experiment.preprocess(filter_max_na=0.5, impute_method="min")
-        >>> experiment.extract_meta_properties()
         >>> experiment.derive_traits()  # with default formulas
         >>> experiment.post_filter(corr_threshold=0.9)
         >>> experiment.diff_analysis()
     """
 
     _all_steps = [
         "preprocess",
-        "extract_meta_properties",
         "derive_traits",
         "post_filter",
         "diff_analysis",
     ]
     _data_dict = {
-        "preprocess": ["processed_abundance_table"],
-        "extract_meta_properties": ["meta_property_table"],
+        "preprocess": ["processed_abundance_table", "meta_property_table"],
         "derive_traits": ["derived_trait_table", "formulas"],
         "post_filter": ["filtered_derived_trait_table"],
         "diff_analysis": ["diff_results"],
     }
 
     input_data: GlyTraitInputData
     mode: Literal["structure", "composition"] = field(default="structure", kw_only=True)
@@ -329,15 +331,16 @@
     def preprocess(
         self,
         filter_max_na: float = 1.0,
         impute_method: Literal["zero", "min", "lod", "mean", "median"] = "zero",
     ) -> None:
         """Preprocess the data.
 
-        Calling this method will make the `processed_abundance_table` attribute available.
+        Calling this method will make the `processed_abundance_table` and
+        `meta_property_table` attributes available.
 
         Args:
             filter_max_na (float): The maximum ratio of missing values in a sample.
                 Range: [0, 1].
                 If the ratio of missing values in a sample is greater than this value,
                 the sample will be removed.
                 Setting to 1.0 means no filtering.
@@ -352,26 +355,31 @@
                 Default: "zero".
         """
         processed = preprocess(
             data=self.input_data.abundance_table,
             filter_max_na=filter_max_na,
             impute_method=impute_method,
         )
-        return {"processed_abundance_table": AbundanceTable(processed)}  # type: ignore
-
-    @_step
-    def extract_meta_properties(self) -> None:
+        mp_table = self._extract_meta_properties(processed)
+        return {  # type: ignore
+            "processed_abundance_table": AbundanceTable(processed),
+            "meta_property_table": mp_table,
+        }
+
+    def _extract_meta_properties(
+        self, processed_abund_df: AbundanceTable
+    ) -> MetaPropertyTable:
         """Extract meta-properties.
 
         Calling this method will make the `meta_property_table` attribute available.
         """
-        glycans: list[str] = self.processed_abundance_table.columns.tolist()
+        glycans: list[str] = processed_abund_df.columns.tolist()
         glycan_dict = cast(GlycanDict, {g: self.input_data.glycans[g] for g in glycans})
         mp_table = build_meta_property_table(glycan_dict, self.mode, self.sia_linkage)
-        return {"meta_property_table": mp_table}  # type: ignore
+        return mp_table
 
     @_step
     def derive_traits(self, formulas: Optional[list[TraitFormula]] = None) -> None:
         """Calculate derived traits.
 
         Calling this method will make the `derived_trait_table` attribute available.
 
@@ -437,17 +445,16 @@
         filter_max_na: float = 1.0,
         impute_method: Literal["zero", "min", "lod", "mean", "median"] = "zero",
         formulas: Optional[list[TraitFormula]] = None,
         corr_threshold: float = 1.0,
     ) -> None:
         """Run the entire workflow.
 
-        Call the `preprocess`, `extract_meta_properties`, `derive_traits`,
-        `post_filter`, and `diff_analysis` methods sequentially.
-        `diff_analysis` will be skipped if group information is not provided.
+        Call `preprocess`, `derive_traits`, and `post_filter` sequentially.
+        If group information is provided, call `diff_analysis` at the end.
 
         Args:
             filter_max_na: The maximum ratio of missing values in a sample.
                 Range: [0, 1].
                 If the ratio of missing values in a sample is greater than this value,
                 the sample will be removed.
                 Setting to 1.0 means no filtering.
@@ -466,12 +473,61 @@
             corr_threshold: The correlation threshold for post filtering.
                 If the correlation between two traits is greater than this value,
                 one of them will be removed.
                 Setting to -1.0 means no correlation filtering.
                 Default: 1.0.
         """
         self.preprocess(filter_max_na, impute_method)
-        self.extract_meta_properties()
         self.derive_traits(formulas)
         self.post_filter(corr_threshold)
         if self.input_data.groups is not None:
             self.diff_analysis()
+
+    def try_formulas(
+        self, __expr: Iterable[str] | str, /, squeeze: bool = True
+    ) -> pd.DataFrame | pd.Series:
+        """Calculate derived traits with the given formulas
+
+        Args:
+            __expr: The formulas to calculate the derived traits.
+                Could be a list of formula expressions (str)
+                or a single formula expression (str).
+            squeeze: Whether to squeeze the result if only one formula is provided.
+                Default: True.
+
+        Returns:
+            If `squeeze=True` and only one formula is provided, return a Series.
+            Otherwise, return a DataFrame with derived trait names as columns.
+            Index of the DataFrame or Series is the sample names
+            (same as the processed abundance table).
+
+        Raises:
+            FormulaParseError: If any formula expression is invalid.
+
+        Examples:
+            >>> exp = Experiment(input_data)
+            >>> exp.preprocess()
+            >>> exp.try_formulas("TC = [type == 'complex'] / [1]")
+            pd.Series(...)
+            >>> exp.try_formulas(["TC = [type == 'complex'] / [1]", "TS = [nS > 0] / [1]"])
+            pd.DataFrame(...)
+        """
+
+        if self._current_step == "__START__":
+            raise InvalidOperationOrderError("Call `preprocess` first.")
+
+        if isinstance(__expr, str):
+            exprs = [__expr]
+        else:
+            exprs = list(__expr)
+        formulas = parse_formulas(exprs)
+
+        trait_table = calcu_derived_trait(
+            abund_df=self.processed_abundance_table,
+            meta_prop_df=self.meta_property_table,
+            formulas=formulas,
+        )
+
+        if squeeze and len(formulas) == 1:
+            return trait_table.iloc[:, 0]
+        else:
+            return trait_table
```

### Comparing `glytrait-0.1.4/src/glytrait/cli.py` & `glytrait-0.1.5/src/glytrait/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,14 @@
 
 def _process_exp(
     exp: Experiment,
     formula_file: str | None,
     config: WorkflowConfig,
 ) -> None:
     exp.preprocess(config.filter_glycan_ratio, config.impute_method)
-    exp.extract_meta_properties()
 
     if formula_file:
         formulas = load_formulas_from_file(formula_file, config.sia_linkage)
         exp.derive_traits(formulas)
     else:
         exp.derive_traits()
```

### Comparing `glytrait-0.1.4/src/glytrait/data_export.py` & `glytrait-0.1.5/src/glytrait/data_export.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/src/glytrait/data_input.py` & `glytrait-0.1.5/src/glytrait/data_input.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/src/glytrait/data_type.py` & `glytrait-0.1.5/src/glytrait/data_type.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/src/glytrait/exception.py` & `glytrait-0.1.5/src/glytrait/exception.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/src/glytrait/formula.py` & `glytrait-0.1.5/src/glytrait/formula.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 The `TraitFormula` class is used to represent a trait formula.
 It is the core of calculating derived traits.
 
 Classes:
     TraitFormula: The trait formula.
 
 Functions:
-    load_formulas: Load all trait formulas from default formula files and custom formulas files.
-    save_trait_formulas_tepmlate: Save a template of trait formulas to a file.
+    parse_formulas: Parse formula expressions.
+    load_formulas_from_file: Load formulas from a formula file.
+    load_default_formulas: Load the default formulas.
     save_builtin_formula: Save a built-in trait formulas to a file.
 """
 
 from __future__ import annotations
 
 import functools
 import itertools
```

### Comparing `glytrait-0.1.4/src/glytrait/glycan.py` & `glytrait-0.1.5/src/glytrait/glycan.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/src/glytrait/meta_property.py` & `glytrait-0.1.5/src/glytrait/meta_property.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/src/glytrait/post_filtering.py` & `glytrait-0.1.5/src/glytrait/post_filtering.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/src/glytrait/preprocessing.py` & `glytrait-0.1.5/src/glytrait/preprocessing.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/src/glytrait/resources/comp_formula.txt` & `glytrait-0.1.5/src/glytrait/resources/comp_formula.txt`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/src/glytrait/resources/struc_formula.txt` & `glytrait-0.1.5/src/glytrait/resources/struc_formula.txt`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/src/glytrait/stat.py` & `glytrait-0.1.5/src/glytrait/stat.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/src/glytrait/trait.py` & `glytrait-0.1.5/src/glytrait/trait.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.4/PKG-INFO` & `glytrait-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glytrait
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool for calculating derived traits for N-glycome
 Home-page: https://github.com/fubin1999/glytrait
 License: MIT
 Keywords: bioinformatics,glycomics,biology
 Author: fubin1999
 Author-email: 65430559+fubin1999@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
@@ -264,14 +264,25 @@
 The "GlycanID" column should contain all glycan IDs in the abundance file.
 The "Structure" column should contain the structure strings of the glycans.
 For now, only the GlycoCT format is supported.
 In the "composition" mode, the second column should be "Composition" instead of "Structure",
 and the composition strings should be used instead of the structure strings.
 Condensed format ("H3N4F1S1") is supported.
 
+The names of the abundance file and the structure (composition) file is not important, 
+i.e., it doesn't have to be "abundance.csv" and "structures.csv". 
+You could use any name you want, as long as the two files are passed in order,
+e.g.: 
+
+```shell
+glytrait experiment_1_15.csv serum_structures.csv
+#        ~~~~~~~~~~~~~~~~~~~ ~~~~~~~~~~~~~~~~~~~~
+#        the abundance file   the structure file
+```
+
 ### Specify the output path
 
 You might have noticed before that GlyTrait saves the output file to the same directory 
 as the abundance file with a "_glytrait" suffix.
 You can specify the output file path by using the "-o" or "--output-file" option:
 
 ```shell
```

