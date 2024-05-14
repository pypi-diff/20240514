# Comparing `tmp/xmask-0.3.8.tar.gz` & `tmp/xmask-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmask-0.3.8.tar", last modified: Sat Feb 10 07:01:00 2024, max compression
+gzip compressed data, was "xmask-0.3.9.tar", last modified: Tue May 14 07:52:53 2024, max compression
```

## Comparing `xmask-0.3.8.tar` & `xmask-0.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-02-10 07:01:00.858286 xmask-0.3.8/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:05:06.000000 xmask-0.3.8/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      237 2023-03-23 11:05:06.000000 xmask-0.3.8/MANIFEST.in
--rw-r--r--   0 giadarol   (503) staff       (20)      671 2024-02-10 07:01:00.858028 xmask-0.3.8/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      115 2023-10-03 14:12:25.000000 xmask-0.3.8/pyproject.toml
--rw-r--r--   0 giadarol   (503) staff       (20)       38 2024-02-10 07:01:00.858347 xmask-0.3.8/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1433 2023-10-03 14:12:25.000000 xmask-0.3.8/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-02-10 07:01:00.824076 xmask-0.3.8/tests/
--rw-r--r--   0 giadarol   (503) staff       (20)    71921 2024-02-05 10:39:56.000000 xmask-0.3.8/tests/test_hllhc14.py
--rw-r--r--   0 giadarol   (503) staff       (20)    21539 2024-02-10 06:42:53.000000 xmask-0.3.8/tests/test_hllhc14_b1_only.py
--rw-r--r--   0 giadarol   (503) staff       (20)    29761 2023-11-29 05:23:47.000000 xmask-0.3.8/tests/test_lhc_ion.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-02-10 07:01:00.840145 xmask-0.3.8/xmask/
--rw-r--r--   0 giadarol   (503) staff       (20)      233 2023-10-03 14:12:25.000000 xmask-0.3.8/xmask/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2024-02-10 06:43:16.000000 xmask-0.3.8/xmask/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)      225 2023-03-23 11:05:06.000000 xmask-0.3.8/xmask/env_and_links.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-02-10 07:01:00.857115 xmask-0.3.8/xmask/lhc/
--rw-r--r--   0 giadarol   (503) staff       (20)      432 2023-05-07 06:53:44.000000 xmask-0.3.8/xmask/lhc/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)     5652 2023-10-03 14:12:25.000000 xmask-0.3.8/xmask/lhc/build_madx_and_xsuite_models.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3553 2023-10-03 14:12:25.000000 xmask-0.3.8/xmask/lhc/errors.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2423 2023-05-30 19:22:48.000000 xmask-0.3.8/xmask/lhc/knob_manipulations.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3572 2024-01-22 16:26:06.000000 xmask-0.3.8/xmask/lhc/leveling.py
--rw-r--r--   0 giadarol   (503) staff       (20)    12388 2023-07-21 09:09:07.000000 xmask-0.3.8/xmask/madx_model.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2883 2023-10-03 14:12:25.000000 xmask-0.3.8/xmask/tuning.py
--rw-r--r--   0 giadarol   (503) staff       (20)      728 2023-03-23 11:05:06.000000 xmask-0.3.8/xmask/yaml.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-02-10 07:01:00.857483 xmask-0.3.8/xmask.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      671 2024-02-10 07:01:00.000000 xmask-0.3.8/xmask.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      508 2024-02-10 07:01:00.000000 xmask-0.3.8/xmask.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2024-02-10 07:01:00.000000 xmask-0.3.8/xmask.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       49 2024-02-10 07:01:00.000000 xmask-0.3.8/xmask.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        6 2024-02-10 07:01:00.000000 xmask-0.3.8/xmask.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-05-14 07:52:53.563268 xmask-0.3.9/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:05:06.000000 xmask-0.3.9/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      237 2023-03-23 11:05:06.000000 xmask-0.3.9/MANIFEST.in
+-rw-r--r--   0 giadarol   (503) staff       (20)      671 2024-05-14 07:52:53.563037 xmask-0.3.9/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      115 2023-10-03 14:12:25.000000 xmask-0.3.9/pyproject.toml
+-rw-r--r--   0 giadarol   (503) staff       (20)       38 2024-05-14 07:52:53.563311 xmask-0.3.9/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1433 2023-10-03 14:12:25.000000 xmask-0.3.9/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-05-14 07:52:53.548597 xmask-0.3.9/tests/
+-rw-r--r--   0 giadarol   (503) staff       (20)    71921 2024-02-05 10:39:56.000000 xmask-0.3.9/tests/test_hllhc14.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    21539 2024-02-10 06:42:53.000000 xmask-0.3.9/tests/test_hllhc14_b1_only.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    29761 2023-11-29 05:23:47.000000 xmask-0.3.9/tests/test_lhc_ion.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-05-14 07:52:53.558271 xmask-0.3.9/xmask/
+-rw-r--r--   0 giadarol   (503) staff       (20)      233 2023-10-03 14:12:25.000000 xmask-0.3.9/xmask/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2024-05-14 07:52:23.000000 xmask-0.3.9/xmask/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      225 2023-03-23 11:05:06.000000 xmask-0.3.9/xmask/env_and_links.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-05-14 07:52:53.562252 xmask-0.3.9/xmask/lhc/
+-rw-r--r--   0 giadarol   (503) staff       (20)      432 2023-05-07 06:53:44.000000 xmask-0.3.9/xmask/lhc/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     5652 2023-10-03 14:12:25.000000 xmask-0.3.9/xmask/lhc/build_madx_and_xsuite_models.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3553 2023-10-03 14:12:25.000000 xmask-0.3.9/xmask/lhc/errors.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2423 2023-05-30 19:22:48.000000 xmask-0.3.9/xmask/lhc/knob_manipulations.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3572 2024-01-22 16:26:06.000000 xmask-0.3.9/xmask/lhc/leveling.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    12388 2023-07-21 09:09:07.000000 xmask-0.3.9/xmask/madx_model.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2890 2024-05-14 07:50:28.000000 xmask-0.3.9/xmask/tuning.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      728 2023-03-23 11:05:06.000000 xmask-0.3.9/xmask/yaml.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-05-14 07:52:53.562612 xmask-0.3.9/xmask.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      671 2024-05-14 07:52:53.000000 xmask-0.3.9/xmask.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      508 2024-05-14 07:52:53.000000 xmask-0.3.9/xmask.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2024-05-14 07:52:53.000000 xmask-0.3.9/xmask.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       49 2024-05-14 07:52:53.000000 xmask-0.3.9/xmask.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        6 2024-05-14 07:52:53.000000 xmask-0.3.9/xmask.egg-info/top_level.txt
```

### Comparing `xmask-0.3.8/LICENSE` & `xmask-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xmask-0.3.8/PKG-INFO` & `xmask-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmask
-Version: 0.3.8
+Version: 0.3.9
 Summary: Configuration of tracking simulations for the LHC and other accelerators
 Home-page: https://github.com/xsuite/xsuite/issues
 Download-URL: https://pypi.python.org/pypi/xmask
 Author: G. Iadarola et al.
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Source Code, https://github.com/xsuite/xmask/
```

### Comparing `xmask-0.3.8/setup.py` & `xmask-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.8/tests/test_hllhc14.py` & `xmask-0.3.9/tests/test_hllhc14.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.8/tests/test_hllhc14_b1_only.py` & `xmask-0.3.9/tests/test_hllhc14_b1_only.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.8/tests/test_lhc_ion.py` & `xmask-0.3.9/tests/test_lhc_ion.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.8/xmask/lhc/build_madx_and_xsuite_models.py` & `xmask-0.3.9/xmask/lhc/build_madx_and_xsuite_models.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.8/xmask/lhc/errors.py` & `xmask-0.3.9/xmask/lhc/errors.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.8/xmask/lhc/knob_manipulations.py` & `xmask-0.3.9/xmask/lhc/knob_manipulations.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.8/xmask/lhc/leveling.py` & `xmask-0.3.9/xmask/lhc/leveling.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.8/xmask/madx_model.py` & `xmask-0.3.9/xmask/madx_model.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.8/xmask/tuning.py` & `xmask-0.3.9/xmask/tuning.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         print(f'Correcting closed orbit')
         assert line_co_ref is not None
         assert co_corr_config is not None
         if isinstance(co_corr_config, (str, Path)):
             with open(co_corr_config, 'r') as fid:
                 co_corr_config = json.load(fid)
 
-        line.correct_closed_orbit(
+        line._xmask_correct_closed_orbit(
                                 reference=line_co_ref,
                                 correction_config=co_corr_config)
 
     if enable_linear_coupling_correction:
         assert knob_names is not None
         assert 'c_minus_knob_1' in knob_names
         assert 'c_minus_knob_2' in knob_names
```

### Comparing `xmask-0.3.8/xmask/yaml.py` & `xmask-0.3.9/xmask/yaml.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.8/xmask.egg-info/PKG-INFO` & `xmask-0.3.9/xmask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmask
-Version: 0.3.8
+Version: 0.3.9
 Summary: Configuration of tracking simulations for the LHC and other accelerators
 Home-page: https://github.com/xsuite/xsuite/issues
 Download-URL: https://pypi.python.org/pypi/xmask
 Author: G. Iadarola et al.
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Source Code, https://github.com/xsuite/xmask/
```

