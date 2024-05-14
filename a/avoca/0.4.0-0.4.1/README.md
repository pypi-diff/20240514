# Comparing `tmp/avoca-0.4.0.tar.gz` & `tmp/avoca-0.4.1.tar.gz`

## Comparing `avoca-0.4.0.tar` & `avoca-0.4.1.tar`

### file list

```diff
@@ -1,46 +1,50 @@
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 avoca-0.4.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 avoca-0.4.0/.readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/export_nas.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/flags.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/io.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/logging.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/manager.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/requirements.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/bindings/__init__.py
--rw-r--r--   0        0        0    15939 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/bindings/ebas.py
--rw-r--r--   0        0        0    10120 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/bindings/gcwerks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/__init__.py
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/abstract.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/concs.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/generate_classes_doc.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/rt.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/test.py
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/zscore.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/testing/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/testing/df.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/utils/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/utils/torch_models.py
--rw-r--r--   0        0        0   152471 2020-02-02 00:00:00.000000 avoca-0.4.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas
--rw-r--r--   0        0        0   499755 2020-02-02 00:00:00.000000 avoca-0.4.0/data/voc_jan2jun_2023.csv
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 avoca-0.4.0/data/.avoca/config.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/make.bat
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/source/conf.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/source/index.rst
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/source/quickstart.ipynb
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/source/bindings/ebas.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/source/bindings/gcwerks.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/source/bindings/index.rst
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 avoca-0.4.0/examples/config.yaml
--rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 avoca-0.4.0/examples/data_qa.ipynb
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 avoca-0.4.0/examples/read_nas.ipynb
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 avoca-0.4.0/tests/test_io.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 avoca-0.4.0/tests/bindings/gcwerks.dat
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 avoca-0.4.0/tests/bindings/test_gcwerks.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 avoca-0.4.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 avoca-0.4.0/LICENCE.txt
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 avoca-0.4.0/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 avoca-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 avoca-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 avoca-0.4.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 avoca-0.4.1/.readthedocs.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/export_nas.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/flags.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/io.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/logging.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/manager.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/requirements.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/bindings/__init__.py
+-rw-r--r--   0        0        0    16458 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/bindings/ebas.py
+-rw-r--r--   0        0        0    11022 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/bindings/gcwerks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/__init__.py
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/abstract.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/concs.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/generate_classes_doc.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/rt.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/test.py
+-rw-r--r--   0        0        0    15855 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/zscore.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/testing/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/testing/df.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/utils/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/utils/torch_models.py
+-rw-r--r--   0        0        0   152471 2020-02-02 00:00:00.000000 avoca-0.4.1/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas
+-rw-r--r--   0        0        0   499755 2020-02-02 00:00:00.000000 avoca-0.4.1/data/voc_jan2jun_2023.csv
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 avoca-0.4.1/data/.avoca/config.yaml
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 avoca-0.4.1/data/tests/missing_area_cols.csv
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/make.bat
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/source/conf.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/source/index.rst
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/source/quickstart.ipynb
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/source/bindings/ebas.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/source/bindings/gcwerks.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/source/bindings/index.rst
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 avoca-0.4.1/examples/config.yaml
+-rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 avoca-0.4.1/examples/data_qa.ipynb
+-rw-r--r--   0        0        0   199025 2020-02-02 00:00:00.000000 avoca-0.4.1/examples/data_qa_gcwerks.ipynb
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 avoca-0.4.1/examples/export_gc_werks.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 avoca-0.4.1/examples/export_gc_werks_secondary_peaks.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 avoca-0.4.1/examples/read_nas.ipynb
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 avoca-0.4.1/tests/test_io.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 avoca-0.4.1/tests/bindings/gcwerks.dat
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 avoca-0.4.1/tests/bindings/test_gcwerks.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 avoca-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 avoca-0.4.1/LICENCE.txt
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 avoca-0.4.1/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 avoca-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 avoca-0.4.1/PKG-INFO
```

### Comparing `avoca-0.4.0/.gitlab-ci.yml` & `avoca-0.4.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/.readthedocs.yaml` & `avoca-0.4.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/avoca/flags.py` & `avoca-0.4.1/avoca/flags.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/avoca/manager.py` & `avoca-0.4.1/avoca/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,31 +79,42 @@
         )
 
     @staticmethod
     def train(assigner: AbstractQA_Assigner, df: pd.DataFrame):
         # Check that the compounds are okay
         compounds_of_df = compounds_from_df(df)
         if not assigner.compounds:
-            if not set(assigner.compounds).issubset(compounds_of_df):
-                raise ValueError(
-                    f"{assigner=} has {assigner.compounds=} which are not in the"
-                    f" dataframe compounds: {compounds_of_df}"
-                )
-        else:
             # Set all the compounds if not specified
             assigner.compounds = compounds_of_df
+        if not set(assigner.compounds).issubset(compounds_of_df):
+            raise ValueError(
+                f"{assigner=} has {assigner.compounds=} which are not in the"
+                f" dataframe compounds: {compounds_of_df}"
+            )
 
         if not hasattr(assigner, "runtypes") or assigner.runtypes is None:
             # Set all the runtypes if not specified
             assigner.runtypes = runtypes_from_df(df)
 
         # Get the rows that the assigner should use
-        rows = df[("-", "type")].isin(assigner.runtypes)
+        rows = (
+            # Correct types
+            df[("-", "type")].isin(assigner.runtypes)
+            # Correct times
+            & df[("-", "datetime")].between(assigner.start, assigner.stopp)
+        )
+
+        # Check consistency of the df
+        if not rows.any():
+            raise ValueError(
+                f"No rows in the dataframe with {assigner.runtypes=} and between"
+                f" {assigner.start=} and {assigner.stopp=}"
+            )
 
-        assigner.fit(df.loc[rows].loc[assigner.start : assigner.stopp])
+        assigner.fit(df.loc[rows])
 
     @staticmethod
     def apply(assigner: AbstractQA_Assigner, df: pd.DataFrame):
         """Apply a QA assigner to a dataframe.
 
         Args:
             assigner: The QA assigner to apply.
```

### Comparing `avoca-0.4.0/avoca/requirements.py` & `avoca-0.4.1/avoca/requirements.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/avoca/settings.py` & `avoca-0.4.1/avoca/settings.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/avoca/bindings/ebas.py` & `avoca-0.4.1/avoca/bindings/ebas.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,29 @@
     ebas_compname_of_var = {
         "rt": "retention_time",
         "w": "peak_width",
         "area": "peak_area",
     }
 
     metadatas = {}
+
+        
+    # Export calibration status if given by the user
+    status_col = ("-", "status")
+    if status_col in df_export.columns:
+        metadata = DataObject()
+        metadata.comp_name = "status"
+        metadata.title = "cal"
+        metadata.unit = "no unit"
+        values = [val for val in df_export[status_col]]
+        flags = [[] for _ in df_export[status_col]]
+        nas.variables.append(
+            DataObject(values_=values,flags=flags, flagcol=True, metadata=metadata)
+        )
+
     for sub in compounds:
         flags = [
             sorted(flag_all + [flags_to_ebas[f] for f in QA_Flag if f in QA_Flag(flag)])
             for flag in df_export[(sub, "flag")]
         ]
         nan_flag = df_export[(sub, "flag")] & QA_Flag.MISSING.value
         for var in vars_to_export[data_level]:
```

### Comparing `avoca-0.4.0/avoca/bindings/gcwerks.py` & `avoca-0.4.1/avoca/bindings/gcwerks.py`

 * *Files 5% similar despite different names*

```diff
@@ -289,15 +289,38 @@
     variables_str = " ".join([f"{sub}.{var}" for sub in compounds for var in variables])
 
     command = (
         f"{gc_bin_dir}/gcexport "
         f"-gcdir {gcdir} "
         # f"-format {report_conf} "
         f"-mindate {date_start.strftime('%y%m%d')} "
-        f"time type {variables_str} "
+        f"time type sample {variables_str} "
         f"> {out_file}"
     )
     # command = f"gcnetcdf-export -gcdir {gcdir}  -mindate {date_start.strftime('%y%m%d')} time type {variables_str} -exportdir {out_file.parent}"
 
     # Run the command
     print("Running: ", command)
     subprocess.run(command, shell=True, check=True)
+
+
+
+def read_quats_log(gcdir: PathLike) -> pd.DataFrame:
+    """Read the quat.log file from gcwerks."""
+
+    # Find where the quat log file is located
+    quat_log_filepath = Path(gcdir) /"results" / "log" / "quat.log"
+
+    if not quat_log_filepath.exists():
+        raise FileNotFoundError(f"File {quat_log_filepath} not found.")
+
+    df = pd.read_csv(quat_log_filepath, sep="\s+", skiprows=1, header=None, names=["dt1", "dt2", "gas", "mean", "mean_s", "blank", "blank_s", "fit_n", "fit_a", "fit_b", "fit_c", "#", "tanks"])
+    # Convert datetime from unix timestamp to datetime
+    for col in ["dt1", "dt2"]:
+        df[col] = pd.to_datetime(df[col], unit="s")
+
+    # Split the tank column inot the two tanks they contain 
+    splitted = df["tanks"].str.split("/", expand=True)
+    df["sampleQuaternary"] = splitted[0]
+    df["sampleTertiary"] = splitted[1]
+
+    return df
```

### Comparing `avoca-0.4.0/avoca/qa_class/abstract.py` & `avoca-0.4.1/avoca/qa_class/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,16 +81,22 @@
 
         if args:
             raise ValueError(
                 f"{AbstractQA_Assigner} does not take any positional arguments."
             )
         if not compounds:
             raise ValueError(f"{self} must have at least one compound.")
+        self.logger.debug(f"Creating {self} with {compounds=}")
         self.compounds = compounds
 
+        # Check the types
+        if not isinstance(start, pd.Timestamp):
+            raise ValueError(f"{start=} is not a pd.Timestamp.")
+        if not isinstance(stopp, pd.Timestamp):
+            raise ValueError(f"{stopp=} is not a pd.Timestamp.")
         self.start = start
         self.stopp = stopp
 
         if self.required_packages is not None:
             for package in self.required_packages:
                 if not package.check():
                     raise ImportError(
```

### Comparing `avoca-0.4.0/avoca/qa_class/concs.py` & `avoca-0.4.1/avoca/qa_class/concs.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/avoca/qa_class/generate_classes_doc.py` & `avoca-0.4.1/avoca/qa_class/generate_classes_doc.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/avoca/qa_class/rt.py` & `avoca-0.4.1/avoca/qa_class/rt.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/avoca/qa_class/test.py` & `avoca-0.4.1/avoca/qa_class/test.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/avoca/qa_class/zscore.py` & `avoca-0.4.1/avoca/qa_class/zscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     The method is based on the z-score, which is calculated as follows:
 
     .. math::
 
         z = \\frac{x - \\mu}{\\sigma}
 
-    where :math:`x` is the value, :math:`\\mu` is the mean of the values 
+    where :math:`x` is the value, :math:`\\mu` is the mean of the values
     and :math:`\\sigma` is the standard deviation of the values.
 
     If the z-score is greater than a threshold, the value is flagged.
 
     :param variable: The variable to check for extreme values.
     :param threshold: The threshold for the z-score. To flag values.
     :param use_log_normal: If True, the log of the values will be used to calculate the z-score.
```

### Comparing `avoca-0.4.0/avoca/utils/__init__.py` & `avoca-0.4.1/avoca/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from contextlib import contextmanager
 
 import pandas as pd
 
 
 def compounds_from_df(df: pd.DataFrame) -> list[str]:
     """Get the compounds from a dataframe.
```

### Comparing `avoca-0.4.0/avoca/utils/torch_models.py` & `avoca-0.4.1/avoca/utils/torch_models.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas` & `avoca-0.4.1/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/data/voc_jan2jun_2023.csv` & `avoca-0.4.1/data/voc_jan2jun_2023.csv`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/docs/Makefile` & `avoca-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/docs/make.bat` & `avoca-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/docs/source/conf.py` & `avoca-0.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/docs/source/index.rst` & `avoca-0.4.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/docs/source/quickstart.ipynb` & `avoca-0.4.1/docs/source/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/docs/source/bindings/ebas.md` & `avoca-0.4.1/docs/source/bindings/ebas.md`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/examples/data_qa.ipynb` & `avoca-0.4.1/examples/data_qa.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.8.10'}}"}*

```diff
@@ -358,14 +358,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.12.2"
+            "version": "3.8.10"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `avoca-0.4.0/examples/read_nas.ipynb` & `avoca-0.4.1/examples/read_nas.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/LICENCE.txt` & `avoca-0.4.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `avoca-0.4.0/pyproject.toml` & `avoca-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "avoca"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Lionel Constantin", email="lionel.constantin@empa.ch" },
 ]
 description = "@voc@: Quality assessement of measurement data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `avoca-0.4.0/PKG-INFO` & `avoca-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: avoca
-Version: 0.4.0
+Version: 0.4.1
 Summary: @voc@: Quality assessement of measurement data
 Project-URL: Homepage, https://gitlab.com/empa503/atmospheric-measurements/avoca
 Project-URL: Bug Tracker, https://gitlab.com/empa503/atmospheric-measurements/avoca/-/issues
 Project-URL: Documentation, http://avoca.readthedocs.io/
 Author-email: Lionel Constantin <lionel.constantin@empa.ch>
 License-File: LICENCE.txt
 Classifier: License :: OSI Approved :: MIT License
```

