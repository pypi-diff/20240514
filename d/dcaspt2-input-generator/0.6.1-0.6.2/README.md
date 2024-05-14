# Comparing `tmp/dcaspt2_input_generator-0.6.1.tar.gz` & `tmp/dcaspt2_input_generator-0.6.2.tar.gz`

## Comparing `dcaspt2_input_generator-0.6.1.tar` & `dcaspt2_input_generator-0.6.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    18182 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/.pylintrc
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/.github/release-drafter.yml
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/.github/scripts/versionup.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/.github/workflows/release-pr.yml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/.vscode/extensions.json
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/data/.gitignore
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/__about__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/__main__.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/dcaspt2_input_generator.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/color_settings.py
--rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/data.py
--rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/main_window.py
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/menu_bar.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/multi_process_settings.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/table_summary.py
--rw-r--r--   0        0        0    12248 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/table_widget.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/controller/color_settings_controller.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/controller/multi_process_controller.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/controller/save_default_settings_controller.py
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/controller/widget_controller.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/utils/args.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/utils/dir_info.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/utils/settings.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/utils/utils.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/LICENSE
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/README.md
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    18182 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/.pylintrc
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/.github/release-drafter.yml
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/.github/scripts/versionup.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/.github/workflows/release-pr.yml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/.vscode/extensions.json
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/data/.gitignore
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/__about__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/__main__.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/dcaspt2_input_generator.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/color_settings.py
+-rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/data.py
+-rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/main_window.py
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/menu_bar.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/multi_process_settings.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/table_summary.py
+-rw-r--r--   0        0        0    12248 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/table_widget.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/controller/color_settings_controller.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/controller/multi_process_controller.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/controller/save_default_settings_controller.py
+-rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/controller/widget_controller.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/utils/args.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/utils/dir_info.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/utils/settings.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/utils/utils.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/LICENSE
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/README.md
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 dcaspt2_input_generator-0.6.2/PKG-INFO
```

### Comparing `dcaspt2_input_generator-0.6.1/.pylintrc` & `dcaspt2_input_generator-0.6.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/.github/release-drafter.yml` & `dcaspt2_input_generator-0.6.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/.github/scripts/versionup.py` & `dcaspt2_input_generator-0.6.2/.github/scripts/versionup.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/.github/workflows/publish.yml` & `dcaspt2_input_generator-0.6.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/.github/workflows/release-pr.yml` & `dcaspt2_input_generator-0.6.2/.github/workflows/release-pr.yml`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/dcaspt2_input_generator.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/dcaspt2_input_generator.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/color_settings.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/color_settings.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/data.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/data.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/main_window.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/main_window.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/menu_bar.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/menu_bar.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/multi_process_settings.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/multi_process_settings.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/table_summary.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/table_summary.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/components/table_widget.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/components/table_widget.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/controller/color_settings_controller.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/controller/color_settings_controller.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/controller/multi_process_controller.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/controller/multi_process_controller.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/controller/save_default_settings_controller.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/controller/save_default_settings_controller.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/controller/widget_controller.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/controller/widget_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,27 +34,27 @@
         row_count = self.table_widget.rowCount()
         for row in range(row_count):
             item = self.table_widget.item(row, 0)
             color = item.background()
             sym_str = item.text()
 
             # nocc, nvcut
-            if rem_electrons >= 0:
+            if rem_electrons > 0:
                 nocc[sym_str] += 1
             elif color != colors.not_used.color:
                 # Reset nvcut
                 for k in nvcut.keys():
                     nvcut[k] = 0
             else:
                 nvcut[sym_str] += 1
 
             # act, sec
             if color == colors.not_used.color:
                 pass
-            elif rem_electrons >= 0:
+            elif rem_electrons > 0:
                 act += 2
             else:
                 sec += 2
             rem_electrons -= 2
 
         # Create standard IVO input
         output = "ninact\n0\n"
```

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/utils/args.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/utils/args.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/utils/dir_info.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/utils/dir_info.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/utils/settings.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/utils/settings.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/src/dcaspt2_input_generator/utils/utils.py` & `dcaspt2_input_generator-0.6.2/src/dcaspt2_input_generator/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/.gitignore` & `dcaspt2_input_generator-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/LICENSE` & `dcaspt2_input_generator-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/pyproject.toml` & `dcaspt2_input_generator-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcaspt2_input_generator-0.6.1/PKG-INFO` & `dcaspt2_input_generator-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dcaspt2_input_generator
-Version: 0.6.1
+Version: 0.6.2
 Summary: This is a GUI tool for supporting the generation of input files for DIRAC_CASPT2 calculation.
 Project-URL: Documentation, https://github.com/RQC-HU/dcaspt2_input_generator#readme
 Project-URL: Issues, https://github.com/RQC-HU/dcaspt2_input_generator/issues
 Project-URL: Source, https://github.com/RQC-HU/dcaspt2_input_generator
 Author-email: Kohei Noda <kohei-noda@hiroshima-u.ac.jp>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

