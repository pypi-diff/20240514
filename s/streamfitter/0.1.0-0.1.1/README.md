# Comparing `tmp/streamfitter-0.1.0.tar.gz` & `tmp/streamfitter-0.1.1.tar.gz`

## Comparing `streamfitter-0.1.0.tar` & `streamfitter-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 streamfitter-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 streamfitter-0.1.0/.python-version
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 streamfitter-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 streamfitter-0.1.0/requirements.lock
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 streamfitter-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 streamfitter-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 streamfitter-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 streamfitter-0.1.0/.idea/streamfitter.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 streamfitter-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 streamfitter-0.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 streamfitter-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 streamfitter-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamfitter-0.1.0/src/streamfitter/__init__.py
--rw-r--r--   0        0        0    15773 2020-02-02 00:00:00.000000 streamfitter-0.1.0/src/streamfitter/fitter.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 streamfitter-0.1.0/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 streamfitter-0.1.0/LICENSE
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 streamfitter-0.1.0/README.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 streamfitter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 streamfitter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 streamfitter-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 streamfitter-0.1.1/.python-version
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 streamfitter-0.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 streamfitter-0.1.1/requirements.lock
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 streamfitter-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 streamfitter-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 streamfitter-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 streamfitter-0.1.1/.idea/streamfitter.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 streamfitter-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 streamfitter-0.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 streamfitter-0.1.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 streamfitter-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamfitter-0.1.1/src/streamfitter/__init__.py
+-rw-r--r--   0        0        0    17678 2020-02-02 00:00:00.000000 streamfitter-0.1.1/src/streamfitter/fitter.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 streamfitter-0.1.1/.gitignore
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 streamfitter-0.1.1/LICENSE
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 streamfitter-0.1.1/README.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 streamfitter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 streamfitter-0.1.1/PKG-INFO
```

### Comparing `streamfitter-0.1.0/.pre-commit-config.yaml` & `streamfitter-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `streamfitter-0.1.0/requirements-dev.lock` & `streamfitter-0.1.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `streamfitter-0.1.0/requirements.lock` & `streamfitter-0.1.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `streamfitter-0.1.0/.idea/workspace.xml` & `streamfitter-0.1.1/.idea/workspace.xml`

 * *Files 10% similar despite different names*

#### Comparing `streamfitter-0.1.0/.idea/workspace.xml` & `streamfitter-0.1.1/.idea/workspace.xml`

```diff
@@ -1,14 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="8dcca099-1c7c-441f-ba95-19933515925b" name="Changes" comment="following merge from github"/>
+    <list default="true" id="8dcca099-1c7c-441f-ba95-19933515925b" name="Changes" comment="following merge from github">
+      <change beforePath="$PROJECT_DIR$/src/streamfitter/fitter.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/streamfitter/fitter.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -29,28 +31,31 @@
   &quot;associatedIndex&quot;: 4
 }</component>
   <component name="ProjectId" id="2gMV0ZaxQRtTunz1xf57gVj0Irg"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent">{
-  &quot;keyToString&quot;: {
-    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
-    &quot;last_opened_file_path&quot;: &quot;/Users/garyt/Dropbox/git/streamfitter&quot;,
-    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
-    &quot;node.js.detected.package.tslint&quot;: &quot;true&quot;,
-    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
-    &quot;node.js.selected.package.tslint&quot;: &quot;(autodetect)&quot;,
-    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
-    &quot;settings.editor.selected.configurable&quot;: &quot;com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable&quot;,
-    &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
+  <component name="PropertiesComponent"><![CDATA[{
+  "keyToString": {
+    "RunOnceActivity.ShowReadmeOnStart": "true",
+    "last_opened_file_path": "/Users/garyt/Dropbox/git/streamfitter/.github/workflows",
+    "node.js.detected.package.eslint": "true",
+    "node.js.detected.package.tslint": "true",
+    "node.js.selected.package.eslint": "(autodetect)",
+    "node.js.selected.package.tslint": "(autodetect)",
+    "nodejs_package_manager_path": "npm",
+    "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable",
+    "vue.rearranger.settings.migration": "true"
   }
-}</component>
+}]]></component>
   <component name="RecentsManager">
+    <key name="CopyFile.RECENT_KEYS">
+      <recent name="$PROJECT_DIR$/.github/workflows"/>
+    </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/src/streamfitter"/>
     </key>
   </component>
   <component name="SharedIndexes">
     <attachedChunks>
       <set>
@@ -66,15 +71,15 @@
       <created>1715507210922</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1715507210922</updated>
       <workItem from="1715507214700" duration="766000"/>
       <workItem from="1715507991442" duration="4195000"/>
       <workItem from="1715512460538" duration="9000"/>
-      <workItem from="1715512656594" duration="11281000"/>
+      <workItem from="1715512656594" duration="18847000"/>
     </task>
     <task id="LOCAL-00001" summary="initial commit of streamfitter">
       <option name="closed" value="true"/>
       <created>1715529436697</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
```

### Comparing `streamfitter-0.1.0/src/streamfitter/fitter.py` & `streamfitter-0.1.1/src/streamfitter/fitter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import math
 import multiprocessing
 import time
+from collections import Counter
 from dataclasses import dataclass
 from datetime import timedelta
 from enum import StrEnum, auto
 from itertools import combinations
 from typing import List, Dict
 
+from nef_pipelines.lib.shift_lib import IntensityMeasurementType
 from nef_pipelines.lib.util import exit_error
 from numpy.random import normal
 
 
 from statistics import stdev
 
 from pynmrstar import Entry, Saveframe
@@ -28,19 +30,14 @@
 
 class ErrorPropogation(StrEnum):
     PROPOGATION = auto()
     JACKNIFE = auto()
     BOOTSTRAP = auto()
 
 
-class DataType(StrEnum):
-    HEIGHT = auto()
-    VOLUME = auto()
-
-
 @dataclass
 class PointAndValue:
     point: float
     value: float
     spectrum_name: str
 
 
@@ -93,44 +90,79 @@
         if self.m_n != 0:
             result = self.stdev() / math.sqrt(self.m_n)
         else:
             result = 0.0
         return result
 
 
-def _calculate_monte_carlo_error(fitter, xs, fits, error_method, noise_level, num_cycles):
+def _calculate_monte_carlo_error(fitter, xs, fits, error_method, noise_level, num_cycles, validate_mc=False):
+    xs_as_floats = [float(x) for x in xs]
+    if validate_mc:
+        replicate_xs = [value for value, count in Counter(xs_as_floats).items() if count > 1]
+        replicate_averages = RunningStats()
+
     mc_fitted_params = {}
+    mc_value_stats = {}
+    mc_fitted_param_values = {}
     for row_count, (atom_key, fit) in enumerate(fits.items()):
+        value_stats = {(i, value): RunningStats() for i, value in enumerate(xs_as_floats)}
+        mc_value_stats[atom_key] = value_stats
+        mc_fitted_param_list = []
+        mc_fitted_param_values[atom_key] = mc_fitted_param_list
+
         fitted_params = [value.value for value in fit.params.values()]
 
         back_calculated = fitter.function(*fitted_params, xs)
 
         mc_keys_and_values = {}
         for i in range(num_cycles):
-            key = atom_key, i
+            fit_key = atom_key, i
             mc_data = back_calculated + normal(0, noise_level, len(xs))
 
-            mc_keys_and_values[key] = xs, mc_data
+            if validate_mc:
+                replicate_values = {}
+                for point, data in zip(xs_as_floats, mc_data):
+                    if point in replicate_xs:
+                        replicate_values.setdefault(point, []).append(float(data))
+                for replicate in replicate_values.values():
+                    for combination in combinations(replicate, 2):
+                        replicate_averages.add(combination[0] - combination[1])
+
+            mc_keys_and_values[fit_key] = xs, mc_data
 
         fits = _fit_series(mc_keys_and_values, fitter)
+
         averagers = {name: RunningStats() for name in fitter.params}
         mc_calculations = 0
-        for key, fit in fits.items():
+        for fit_key, fit in fits.items():
             if fit.success:
                 mc_calculations += 1
+
+                mc_fitted_param_list.append(fit.params)
+
                 for name, value in fit.params.items():
                     averagers[name].add(value.value)
 
+                mc_fitted_params_for_backcalc = [value.value for value in fit.params.values()]
+                mc_back_calculated = fitter.function(*mc_fitted_params_for_backcalc, xs)
+                for back_calculated, averager in zip(mc_back_calculated, value_stats.values()):
+                    averager.add(back_calculated)
+
         errors = {f'{name}_mc_error': averager.sterr() for name, averager in averagers.items()}
         mc_fitted_params[atom_key] = {
             **errors,
             '%mc_failures': (num_cycles - mc_calculations) / num_cycles * 100,
         }
 
-    return mc_fitted_params
+    if validate_mc:
+        print(
+            f'mc mean: {replicate_averages.mean()} mc stdev: {replicate_averages.stdev()}  [from {replicate_averages.num_values()} values]'
+        )
+
+    return mc_fitted_params, mc_value_stats, mc_fitted_param_values
 
 
 def td_format(td_object):
     seconds = int(td_object.total_seconds())
     periods = [
         ('year', 60 * 60 * 24 * 365),
         ('month', 60 * 60 * 24 * 30),
@@ -157,15 +189,15 @@
 
 def fitter(
     entry: Entry,
     series_frames: List[Saveframe],
     error_method: ErrorPropogation,
     cycles: int,
     noise_level,
-    data_type: DataType,
+    intensity_measurement_type: IntensityMeasurementType,
     seed: int,
 ) -> Dict:
     _import_nef_pipelines_or_raise()
 
     from nef_pipelines.lib.peak_lib import frame_to_peaks
 
     numpy_random.seed(seed)
@@ -179,18 +211,18 @@
 
         _exit_if_spectra_are_missing(spectra_by_times_and_indices, frame.name)
 
         peaks_by_times_and_indices = {
             key: frame_to_peaks(spectrum_frame) for key, spectrum_frame in spectra_by_times_and_indices.items()
         }
 
-        atoms_and_values = _get_atoms_and_values(peaks_by_times_and_indices, data_type)
+        atoms_and_values = _get_atoms_and_values(peaks_by_times_and_indices, intensity_measurement_type)
 
         replicate_noise_level, stderr, num_replicates = _get_noise_from_duplicated_values(
-            peaks_by_times_and_indices, data_type
+            peaks_by_times_and_indices, intensity_measurement_type
         )
 
         noise_source = 'cli' if noise_level else 'replicates'
         noise_level = noise_level or replicate_noise_level
 
         msg = [
             ['number of cpus', multiprocessing.cpu_count()],
@@ -203,20 +235,23 @@
             ['number of replicates', num_replicates],
         ]
         print(tabulate(msg, tablefmt='plain'))
         print()
 
         fitter = Relaxation2PointFitter()
 
+        # TODO: this could be a context manager
         start_time = time.time()
         fits = _fit_series(atoms_and_values, fitter)
 
         xs = _get_series_variables_array(series_experiment_loop)
 
-        monte_carlo_errors = _calculate_monte_carlo_error(fitter, xs, fits, error_method, noise_level, cycles)
+        monte_carlo_errors, monte_carlo_value_stats, monte_carlo_param_values = _calculate_monte_carlo_error(
+            fitter, xs, fits, error_method, noise_level, cycles
+        )
         end_time = time.time()
 
         time_delta = timedelta(seconds=end_time - start_time)
         print(f'fitting took {td_format(time_delta)}')
         print()
 
         table = []
@@ -397,29 +432,29 @@
         return amplitude * exp(-time_constant * xs)
 
     @classprop
     def params(cls):
         return list(signature(cls.function).parameters.keys())[:-1]
 
 
-def _get_atoms_and_values(peaks_by_times_and_indices, data_type: DataType) -> Dict:
+def _get_atoms_and_values(peaks_by_times_and_indices, data_type: IntensityMeasurementType) -> Dict:
     atoms_to_values = {}
     for (index, x_value, spectrum_name), peaks in peaks_by_times_and_indices.items():
         for peak in peaks:
             atoms = tuple(sorted([shift.atom for shift in peak.shifts]))
             x_and_y = atoms_to_values.setdefault(atoms, [[], []])
 
-            y_value = peak.height if data_type == DataType.HEIGHT else peak.volume
+            y_value = peak.height if data_type == IntensityMeasurementType.HEIGHT else peak.volume
             x_and_y[0].append(x_value)
             x_and_y[1].append(y_value)
 
     return atoms_to_values
 
 
-def _get_noise_from_duplicated_values(peaks_by_times_and_indices, data_type: DataType) -> float:
+def _get_noise_from_duplicated_values(peaks_by_times_and_indices, data_type: IntensityMeasurementType) -> float:
     peak_list_keys_by_times = {}
     for key, peak_list in peaks_by_times_and_indices.items():
         _, value, _ = key
         peak_list_keys_by_times.setdefault(value, []).append(key)
 
     duplicated_peak_list_keys = [
         peak_list_keys for peak_list_keys in peak_list_keys_by_times.values() if len(peak_list_keys) > 1
@@ -427,17 +462,17 @@
 
     differences = []
     for duplicated_peak_list_set in duplicated_peak_list_keys:
         for combination in combinations(duplicated_peak_list_set, 2):
             peak_pairs = {}
             for key in combination:
                 for peak in peaks_by_times_and_indices[key]:
-                    if data_type == DataType.HEIGHT:
+                    if data_type == IntensityMeasurementType.HEIGHT:
                         value = peak.height
-                    elif data_type == DataType.VOLUME:
+                    elif data_type == IntensityMeasurementType.VOLUME:
                         value = peak.volume
                     key = tuple(sorted([shift.atom for shift in peak.shifts]))
                     peak_pairs.setdefault(key, []).append(value)
 
             for value_pair in peak_pairs.values():
                 if len(value_pair) == 2:
                     differences.append(value_pair[0] - value_pair[1])
```

### Comparing `streamfitter-0.1.0/.gitignore` & `streamfitter-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `streamfitter-0.1.0/LICENSE` & `streamfitter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamfitter-0.1.0/pyproject.toml` & `streamfitter-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "streamfitter"
-version = "0.1.0"
+version = "0.1.1"
 description = "Add your description here"
 authors = [
     { name = "varioustoxins", email = "garyt.and.sarahb@gmail.com" }
 ]
 dependencies = [
     "numpy>=1.26.4",
     "jax>=0.4.28",
```

### Comparing `streamfitter-0.1.0/PKG-INFO` & `streamfitter-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: streamfitter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Add your description here
 Author-email: varioustoxins <garyt.and.sarahb@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: classprop>=0.1.1
 Requires-Dist: jax>=0.4.28
 Requires-Dist: lmfit>=1.3.1
```

