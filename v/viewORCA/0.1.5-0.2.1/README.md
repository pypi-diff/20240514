# Comparing `tmp/vieworca-0.1.5.tar.gz` & `tmp/vieworca-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vieworca-0.1.5.tar", last modified: Wed May  1 13:38:30 2024, max compression
+gzip compressed data, was "vieworca-0.2.1.tar", last modified: Tue May 14 13:13:49 2024, max compression
```

## Comparing `vieworca-0.1.5.tar` & `vieworca-0.2.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.358605 vieworca-0.1.5/
--rwxr-xr-x   0 runner    (1001) docker     (127)    35129 2024-05-01 13:38:26.000000 vieworca-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-01 13:38:30.358605 vieworca-0.1.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2354 2024-05-01 13:38:26.000000 vieworca-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.350604 vieworca-0.1.5/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-05-01 13:38:26.000000 vieworca-0.1.5/bin/viewORCA
--rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-05-01 13:38:26.000000 vieworca-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:38:30.358605 vieworca-0.1.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3078 2024-05-01 13:38:26.000000 vieworca-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.354604 vieworca-0.1.5/viewORCA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.354604 vieworca-0.1.5/viewORCA/Programs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6148 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewIRC.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.354604 vieworca-0.1.5/viewORCA/Programs/viewIRC_methods/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1982 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewIRC_methods/get_ORCA_IRC_images.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2050 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewIRC_methods/get_trajectory_filename.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6018 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewNEB.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.354604 vieworca-0.1.5/viewORCA/Programs/viewNEB_methods/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2057 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewNEB_methods/get_MEP_trajectory_filename.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2176 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewNEB_methods/get_ORCA_NEB_images.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6078 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewNEB_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.354604 vieworca-0.1.5/viewORCA/Programs/viewNEB_snapshot_methods/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2141 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewNEB_snapshot_methods/get_interpolation_filename.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2955 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewNEB_snapshot_methods/plot_neb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5394 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewNEB_snapshot_methods/read_orca_interpolation_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6056 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.354604 vieworca-0.1.5/viewORCA/Programs/viewOPT_methods/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2179 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewOPT_methods/get_ORCA_OPT_images.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1987 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewOPT_methods/get_trajectory_filename.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5006 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewSCAN.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.354604 vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4165 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3510 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_from_SCAN_folders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.358605 vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3652 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/assign_energies_to_SCAN_images.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1962 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/get_ORCA_SCAN_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.358605 vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/utility_methods/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4038 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_files.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2563 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_folders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2029 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/utility_methods/get_trajectory_filename.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      617 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9059 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/check_prerequisites.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.358605 vieworca-0.1.5/viewORCA/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4132 2024-05-01 13:38:26.000000 vieworca-0.1.5/viewORCA/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:38:30.358605 vieworca-0.1.5/viewORCA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-01 13:38:30.000000 vieworca-0.1.5/viewORCA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-01 13:38:30.000000 vieworca-0.1.5/viewORCA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:38:30.000000 vieworca-0.1.5/viewORCA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:38:30.000000 vieworca-0.1.5/viewORCA.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 13:38:30.000000 vieworca-0.1.5/viewORCA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-01 13:38:30.000000 vieworca-0.1.5/viewORCA.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35129 2024-05-14 13:13:45.000000 vieworca-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-14 13:13:49.562180 vieworca-0.2.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2354 2024-05-14 13:13:45.000000 vieworca-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.558180 vieworca-0.2.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-05-14 13:13:45.000000 vieworca-0.2.1/bin/viewORCA
+-rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-05-14 13:13:45.000000 vieworca-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:13:49.562180 vieworca-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3078 2024-05-14 13:13:45.000000 vieworca-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.558180 vieworca-0.2.1/viewORCA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.558180 vieworca-0.2.1/viewORCA/Programs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/get_multiplicity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6148 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewIRC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.558180 vieworca-0.2.1/viewORCA/Programs/viewIRC_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1982 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewIRC_methods/get_ORCA_IRC_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2050 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewIRC_methods/get_trajectory_filename.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6018 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/Programs/viewNEB_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2057 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB_methods/get_MEP_trajectory_filename.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2176 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB_methods/get_ORCA_NEB_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6078 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2141 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/get_interpolation_filename.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2955 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/plot_neb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5394 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/read_orca_interpolation_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6056 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/Programs/viewOPT_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2179 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewOPT_methods/get_ORCA_OPT_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1987 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewOPT_methods/get_trajectory_filename.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5006 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4165 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3510 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_from_SCAN_folders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3652 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/assign_energies_to_SCAN_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1962 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/get_ORCA_SCAN_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4038 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2563 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_folders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2029 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/get_trajectory_filename.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      617 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9059 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/check_prerequisites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4189 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-14 13:13:49.000000 vieworca-0.2.1/viewORCA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-14 13:13:49.000000 vieworca-0.2.1/viewORCA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:13:49.000000 vieworca-0.2.1/viewORCA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:13:49.000000 vieworca-0.2.1/viewORCA.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 13:13:49.000000 vieworca-0.2.1/viewORCA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 13:13:49.000000 vieworca-0.2.1/viewORCA.egg-info/top_level.txt
```

### Comparing `vieworca-0.1.5/LICENSE` & `vieworca-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/PKG-INFO` & `vieworca-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: viewORCA
-Version: 0.1.5
+Version: 0.2.1
 Summary: This program is designed to allow the user to inspect calculations from ORCA. This is to be used along side the ORCA Reaction Mechanism Tutorial.
 Home-page: https://geoffreyweal.github.io/ORCA_Mechanism_Procedure/
-Download-URL: https://github.com/geoffreyweal/viewORCA/archive/v0.1.5.tar.gz
+Download-URL: https://github.com/geoffreyweal/viewORCA/archive/v0.2.1.tar.gz
 Author: Dr. Geoffrey R. Weal
 Author-email: geoffrey.weal@gmail.ac.nz
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Keywords: computational-chemistry,DFT,atomic-simulation-environment,ORCA
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
@@ -45,16 +45,16 @@
 * Intrinsic Reaction Coordinate (IRC) Calculations: View the last NEB profile, along with the energy profile of the NEB calculation.
 
 
 ## ORCA
 
 I have written this procedure for: 
 
-* ORCA 5.0.3
 * ORCA 5.0.4
+* ORCA 5.0.3
 
 This method should be valid for future versions of ORCA, but just in case any problems occur it may be due to ORCA version issues. 
 
 
 ## Installing the ``viewORCA`` Program
 
 See [Installation: Setting Up the ``viewORCA`` Program and Pre-Requisites Packages](https://geoffreyweal.github.io/viewORCA/Installation.html) for more information.
```

### Comparing `vieworca-0.1.5/README.md` & `vieworca-0.2.1/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 * Intrinsic Reaction Coordinate (IRC) Calculations: View the last NEB profile, along with the energy profile of the NEB calculation.
 
 
 ## ORCA
 
 I have written this procedure for: 
 
-* ORCA 5.0.3
 * ORCA 5.0.4
+* ORCA 5.0.3
 
 This method should be valid for future versions of ORCA, but just in case any problems occur it may be due to ORCA version issues. 
 
 
 ## Installing the ``viewORCA`` Program
 
 See [Installation: Setting Up the ``viewORCA`` Program and Pre-Requisites Packages](https://geoffreyweal.github.io/viewORCA/Installation.html) for more information.
```

### Comparing `vieworca-0.1.5/setup.py` & `vieworca-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewIRC.py` & `vieworca-0.2.1/viewORCA/Programs/viewIRC.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewIRC_methods/get_ORCA_IRC_images.py` & `vieworca-0.2.1/viewORCA/Programs/viewIRC_methods/get_ORCA_IRC_images.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewIRC_methods/get_trajectory_filename.py` & `vieworca-0.2.1/viewORCA/Programs/viewIRC_methods/get_trajectory_filename.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewNEB.py` & `vieworca-0.2.1/viewORCA/Programs/viewNEB.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewNEB_methods/get_MEP_trajectory_filename.py` & `vieworca-0.2.1/viewORCA/Programs/viewNEB_methods/get_MEP_trajectory_filename.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewNEB_methods/get_ORCA_NEB_images.py` & `vieworca-0.2.1/viewORCA/Programs/viewNEB_methods/get_ORCA_NEB_images.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewNEB_snapshot.py` & `vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewNEB_snapshot_methods/get_interpolation_filename.py` & `vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/get_interpolation_filename.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewNEB_snapshot_methods/plot_neb.py` & `vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/plot_neb.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewNEB_snapshot_methods/read_orca_interpolation_file.py` & `vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/read_orca_interpolation_file.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewOPT.py` & `vieworca-0.2.1/viewORCA/Programs/viewOPT.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewOPT_methods/get_ORCA_OPT_images.py` & `vieworca-0.2.1/viewORCA/Programs/viewOPT_methods/get_ORCA_OPT_images.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewOPT_methods/get_trajectory_filename.py` & `vieworca-0.2.1/viewORCA/Programs/viewOPT_methods/get_trajectory_filename.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewSCAN.py` & `vieworca-0.2.1/viewORCA/Programs/viewSCAN.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information.py` & `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_from_SCAN_folders.py` & `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_from_SCAN_folders.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/assign_energies_to_SCAN_images.py` & `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/assign_energies_to_SCAN_images.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/get_ORCA_SCAN_images.py` & `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/get_ORCA_SCAN_images.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_files.py` & `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_files.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_folders.py` & `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_folders.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/Programs/viewSCAN_methods/utility_methods/get_trajectory_filename.py` & `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/get_trajectory_filename.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/__init__.py` & `vieworca-0.2.1/viewORCA/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # The information about the viewORCA program
 from viewORCA.check_prerequisites import check_prerequisites
 
 __name__    = 'viewORCA'
-__version__ = '0.1.5'
+__version__ = '0.2.1'
 __author__  = 'Dr. Geoffrey Weal'
 check_prerequisites(__version__)
 __author_email__ = 'geoffrey.weal@vuw.ac.nz'
 __license__ = 'GNU AFFERO GENERAL PUBLIC LICENSE'
 __url__ = 'https://github.com/geoffreyweal/viewORCA'
 __doc__ = 'See https://geoffreyweal.github.io/ORCA_Mechanism_Procedure for the documentation on this program'
```

### Comparing `vieworca-0.1.5/viewORCA/check_prerequisites.py` & `vieworca-0.2.1/viewORCA/check_prerequisites.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.1.5/viewORCA/cli/main.py` & `vieworca-0.2.1/viewORCA/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,20 @@
     A subcommand may raise this.  The message will be forwarded to
     the error() method of the argument parser."""
 
 
 # Important: Following any change to command-line parameters, use
 # python3 -m ase.cli.completion to update autocompletion.
 commands = [
+    ('multi',    'viewORCA.Programs.get_multiplicity'),
     ('opt',      'viewORCA.Programs.viewOPT'),
     ('scan',     'viewORCA.Programs.viewSCAN'),
     ('neb',      'viewORCA.Programs.viewNEB'),
     ('neb_snap', 'viewORCA.Programs.viewNEB_snapshot'),
-    ('irc',      'viewORCA.Programs.viewIRC')
+    ('irc',      'viewORCA.Programs.viewIRC'),
 ]
 
 def main(prog='viewORCA', description='Program for viewing jobs from ORCA', commands=commands, hook=None, args=None):
     """
     This method is designed to allow the user to view jobs performed by ORCA to study organic mechanisms. 
     """
     #check_prerequisites(__version__)
```

### Comparing `vieworca-0.1.5/viewORCA.egg-info/PKG-INFO` & `vieworca-0.2.1/viewORCA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: viewORCA
-Version: 0.1.5
+Version: 0.2.1
 Summary: This program is designed to allow the user to inspect calculations from ORCA. This is to be used along side the ORCA Reaction Mechanism Tutorial.
 Home-page: https://geoffreyweal.github.io/ORCA_Mechanism_Procedure/
-Download-URL: https://github.com/geoffreyweal/viewORCA/archive/v0.1.5.tar.gz
+Download-URL: https://github.com/geoffreyweal/viewORCA/archive/v0.2.1.tar.gz
 Author: Dr. Geoffrey R. Weal
 Author-email: geoffrey.weal@gmail.ac.nz
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Keywords: computational-chemistry,DFT,atomic-simulation-environment,ORCA
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
@@ -45,16 +45,16 @@
 * Intrinsic Reaction Coordinate (IRC) Calculations: View the last NEB profile, along with the energy profile of the NEB calculation.
 
 
 ## ORCA
 
 I have written this procedure for: 
 
-* ORCA 5.0.3
 * ORCA 5.0.4
+* ORCA 5.0.3
 
 This method should be valid for future versions of ORCA, but just in case any problems occur it may be due to ORCA version issues. 
 
 
 ## Installing the ``viewORCA`` Program
 
 See [Installation: Setting Up the ``viewORCA`` Program and Pre-Requisites Packages](https://geoffreyweal.github.io/viewORCA/Installation.html) for more information.
```

### Comparing `vieworca-0.1.5/viewORCA.egg-info/SOURCES.txt` & `vieworca-0.2.1/viewORCA.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 viewORCA/check_prerequisites.py
 viewORCA.egg-info/PKG-INFO
 viewORCA.egg-info/SOURCES.txt
 viewORCA.egg-info/dependency_links.txt
 viewORCA.egg-info/not-zip-safe
 viewORCA.egg-info/requires.txt
 viewORCA.egg-info/top_level.txt
+viewORCA/Programs/get_multiplicity.py
 viewORCA/Programs/viewIRC.py
 viewORCA/Programs/viewNEB.py
 viewORCA/Programs/viewNEB_snapshot.py
 viewORCA/Programs/viewOPT.py
 viewORCA/Programs/viewSCAN.py
 viewORCA/Programs/viewIRC_methods/get_ORCA_IRC_images.py
 viewORCA/Programs/viewIRC_methods/get_trajectory_filename.py
```

