# Comparing `tmp/metatensor_torch-0.5.0.tar.gz` & `tmp/metatensor_torch-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metatensor_torch-0.5.0.tar", last modified: Fri May  3 12:06:49 2024, max compression
+gzip compressed data, was "metatensor_torch-0.5.1.tar", last modified: Tue May 14 16:52:06 2024, max compression
```

## Comparing `metatensor_torch-0.5.0.tar` & `metatensor_torch-0.5.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:49.658967 metatensor_torch-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-03 12:06:49.658967 metatensor_torch-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:49.654967 metatensor_torch-0.5.0/build-backend/
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/build-backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:49.650967 metatensor_torch-0.5.0/metatensor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:49.654967 metatensor_torch-0.5.0/metatensor/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/_c_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:49.654967 metatensor_torch-0.5.0/metatensor/torch/atomistic/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18054 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/ase_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    27073 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/systems_to_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    48268 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/learn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    61377 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor-torch-cxx-0.5.0.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:49.658967 metatensor_torch-0.5.0/metatensor_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor_torch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/n_commits_since_last_tag
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:06:49.658967 metatensor_torch-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12132 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:06.172803 metatensor_torch-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-14 16:52:06.172803 metatensor_torch-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:06.168803 metatensor_torch-0.5.1/build-backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/build-backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:06.168803 metatensor_torch-0.5.1/metatensor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:06.172803 metatensor_torch-0.5.1/metatensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/_c_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:06.172803 metatensor_torch-0.5.1/metatensor/torch/atomistic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/atomistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/atomistic/_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18054 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/atomistic/ase_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/atomistic/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27073 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/atomistic/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/atomistic/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/atomistic/systems_to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48268 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/metatensor/torch/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61648 2024-05-14 16:52:06.000000 metatensor_torch-0.5.1/metatensor-torch-cxx-0.5.1.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:52:06.172803 metatensor_torch-0.5.1/metatensor_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-14 16:52:06.000000 metatensor_torch-0.5.1/metatensor_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-14 16:52:06.000000 metatensor_torch-0.5.1/metatensor_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:52:06.000000 metatensor_torch-0.5.1/metatensor_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:52:05.000000 metatensor_torch-0.5.1/metatensor_torch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 16:52:06.000000 metatensor_torch-0.5.1/metatensor_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 16:52:06.000000 metatensor_torch-0.5.1/metatensor_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:52:06.000000 metatensor_torch-0.5.1/n_commits_since_last_tag
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:52:06.172803 metatensor_torch-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-05-14 16:51:40.000000 metatensor_torch-0.5.1/setup.py
```

### Comparing `metatensor_torch-0.5.0/LICENSE` & `metatensor_torch-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/PKG-INFO` & `metatensor_torch-0.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: metatensor-torch
-Version: 0.5.0
+Version: 0.5.1
 Summary: TorchScript bindings for metatensor
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
-Project-URL: homepage, https://lab-cosmo.github.io/metatensor/latest/
-Project-URL: documentation, https://lab-cosmo.github.io/metatensor/latest/
+Project-URL: homepage, https://docs.metatensor.org/latest/
+Project-URL: documentation, https://docs.metatensor.org/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
-Project-URL: changelog, https://lab-cosmo.github.io/metatensor/latest/torch/CHANGELOG.html
+Project-URL: changelog, https://docs.metatensor.org/latest/torch/CHANGELOG.html
 Keywords: machine learning,molecular modeling,torch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `metatensor_torch-0.5.0/build-backend/backend.py` & `metatensor_torch-0.5.1/build-backend/backend.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor/torch/__init__.py` & `metatensor_torch-0.5.1/metatensor/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor/torch/_c_lib.py` & `metatensor_torch-0.5.1/metatensor/torch/_c_lib.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor/torch/atomistic/__init__.py` & `metatensor_torch-0.5.1/metatensor/torch/atomistic/__init__.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor/torch/atomistic/_extensions.py` & `metatensor_torch-0.5.1/metatensor/torch/atomistic/_extensions.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor/torch/atomistic/ase_calculator.py` & `metatensor_torch-0.5.1/metatensor/torch/atomistic/ase_calculator.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor/torch/atomistic/documentation.py` & `metatensor_torch-0.5.1/metatensor/torch/atomistic/documentation.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor/torch/atomistic/model.py` & `metatensor_torch-0.5.1/metatensor/torch/atomistic/model.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor/torch/atomistic/outputs.py` & `metatensor_torch-0.5.1/metatensor/torch/atomistic/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     expected_dtype: torch.dtype,
 ):
     """
     Check that the outputs of a model conform to the expected structure for metatensor
     atomistic models.
 
     This function checks conformance with the reference documentation in
-    https://lab-cosmo.github.io/metatensor/latest/atomistic/outputs.html
+    https://docs.metatensor.org/latest/atomistic/outputs.html
     """
 
     for name, output in outputs.items():
         if requested.get(name) is None:
             raise ValueError(
                 f"the model produced an output named '{name}', which was not requested"
             )
```

### Comparing `metatensor_torch-0.5.0/metatensor/torch/atomistic/systems_to_torch.py` & `metatensor_torch-0.5.1/metatensor/torch/atomistic/systems_to_torch.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor/torch/documentation.py` & `metatensor_torch-0.5.1/metatensor/torch/documentation.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor/torch/learn.py` & `metatensor_torch-0.5.1/metatensor/torch/learn.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor/torch/operations.py` & `metatensor_torch-0.5.1/metatensor/torch/operations.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor/torch/utils.py` & `metatensor_torch-0.5.1/metatensor/torch/utils.py`

 * *Files identical despite different names*

### Comparing `metatensor_torch-0.5.0/metatensor_torch.egg-info/PKG-INFO` & `metatensor_torch-0.5.1/metatensor_torch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: metatensor-torch
-Version: 0.5.0
+Version: 0.5.1
 Summary: TorchScript bindings for metatensor
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
-Project-URL: homepage, https://lab-cosmo.github.io/metatensor/latest/
-Project-URL: documentation, https://lab-cosmo.github.io/metatensor/latest/
+Project-URL: homepage, https://docs.metatensor.org/latest/
+Project-URL: documentation, https://docs.metatensor.org/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
-Project-URL: changelog, https://lab-cosmo.github.io/metatensor/latest/torch/CHANGELOG.html
+Project-URL: changelog, https://docs.metatensor.org/latest/torch/CHANGELOG.html
 Keywords: machine learning,molecular modeling,torch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `metatensor_torch-0.5.0/metatensor_torch.egg-info/SOURCES.txt` & `metatensor_torch-0.5.1/metatensor_torch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.rst
-metatensor-torch-cxx-0.5.0.tar.gz
+metatensor-torch-cxx-0.5.1.tar.gz
 n_commits_since_last_tag
 pyproject.toml
 setup.py
 build-backend/backend.py
 metatensor/torch/__init__.py
 metatensor/torch/_c_lib.py
 metatensor/torch/documentation.py
```

### Comparing `metatensor_torch-0.5.0/pyproject.toml` & `metatensor_torch-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [project.urls]
-homepage = "https://lab-cosmo.github.io/metatensor/latest/"
-documentation = "https://lab-cosmo.github.io/metatensor/latest/"
+homepage = "https://docs.metatensor.org/latest/"
+documentation = "https://docs.metatensor.org/latest/"
 repository = "https://github.com/lab-cosmo/metatensor"
-changelog = "https://lab-cosmo.github.io/metatensor/latest/torch/CHANGELOG.html"
+changelog = "https://docs.metatensor.org/latest/torch/CHANGELOG.html"
 
 ### ======================================================================== ###
 [build-system]
 requires = [
     "setuptools >=68",
     "packaging >=23",
     "wheel >=0.41",
```

### Comparing `metatensor_torch-0.5.0/setup.py` & `metatensor_torch-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         cmake_install_prefix = os.path.join(
             install_dir, f"torch-{torch_major}.{torch_minor}"
         )
 
         cmake_options = [
             "-DCMAKE_BUILD_TYPE=Release",
             f"-DCMAKE_INSTALL_PREFIX={cmake_install_prefix}",
+            "-DCMAKE_INSTALL_LIBDIR=lib",
             f"-DCMAKE_PREFIX_PATH={';'.join(cmake_prefix_path)}",
         ]
 
         # ==================================================================== #
         # HACK: Torch cmake build system has a hard time finding CuDNN, so we
         # help it by pointing it to the right files
```

