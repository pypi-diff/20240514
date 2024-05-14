# Comparing `tmp/evomap-0.3.0.tar.gz` & `tmp/evomap-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evomap-0.3.0.tar", max compression
+gzip compressed data, was "evomap-0.3.1.tar", max compression
```

## Comparing `evomap-0.3.0.tar` & `evomap-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1233 2022-06-15 16:03:22.000000 evomap-0.3.0/LICENSE
--rw-r--r--   0        0        0     4986 2024-05-09 18:44:32.642415 evomap-0.3.0/README.md
--rw-r--r--   0        0        0     1252 2023-03-03 10:26:02.000000 evomap-0.3.0/build.py
--rw-r--r--   0        0        0      922 2024-05-09 20:54:56.957283 evomap-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      293 2022-06-01 11:43:21.000000 evomap-0.3.0/src/evomap/__init__.py
--rw-r--r--   0        0        0        0 2022-04-19 13:16:47.000000 evomap-0.3.0/src/evomap/data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 07:28:01.000000 evomap-0.3.0/src/evomap/data/cars/__init__.py
--rw-r--r--   0        0        0     1840 2023-06-16 07:28:02.000000 evomap-0.3.0/src/evomap/data/cars/customer_preference_ratings.csv
--rw-r--r--   0        0        0      857 2023-06-16 07:28:01.000000 evomap-0.3.0/src/evomap/data/cars/perceptual_attribute_ratings.csv
--rw-r--r--   0        0        0     9267 2023-06-16 07:28:02.000000 evomap-0.3.0/src/evomap/data/cars/perceptual_attribute_ratings.xlsx
--rw-r--r--   0        0        0        0 2023-06-16 07:28:01.000000 evomap-0.3.0/src/evomap/data/tnic_sample_small/__init__.py
--rw-r--r--   0        0        0 13835652 2023-06-16 07:28:08.000000 evomap-0.3.0/src/evomap/data/tnic_sample_small/tnic_sample_small.csv
--rw-r--r--   0        0        0 13090689 2023-06-16 07:28:08.000000 evomap-0.3.0/src/evomap/data/tnic_sample_small/tnic_sample_small_old.csv
--rw-r--r--   0        0        0        0 2023-07-28 13:51:10.007285 evomap-0.3.0/src/evomap/data/tnic_sample_tech/__init__.py
--rw-r--r--   0        0        0    41133 2023-07-28 13:48:28.634183 evomap-0.3.0/src/evomap/data/tnic_sample_tech/tnic_sample_technology.csv
--rw-r--r--   0        0        0    34789 2023-07-28 13:48:28.630408 evomap-0.3.0/src/evomap/data/tnic_sample_tech/tnic_sample_technology_with_netflix.csv
--rw-r--r--   0        0        0        0 2023-06-16 07:28:01.000000 evomap-0.3.0/src/evomap/data/tnic_snapshot/__init__.py
--rw-r--r--   0        0        0     8864 2023-06-16 07:28:02.000000 evomap-0.3.0/src/evomap/data/tnic_snapshot/cluster.npy
--rw-r--r--   0        0        0   122432 2023-06-16 07:28:02.000000 evomap-0.3.0/src/evomap/data/tnic_snapshot/label.npy
--rw-r--r--   0        0        0  9539840 2023-06-16 07:28:07.000000 evomap-0.3.0/src/evomap/data/tnic_snapshot/sim_mat.npy
--rw-r--r--   0        0        0     8864 2023-06-16 07:28:02.000000 evomap-0.3.0/src/evomap/data/tnic_snapshot/size.npy
--rw-r--r--   0        0        0        0 2023-06-16 07:28:01.000000 evomap-0.3.0/src/evomap/data/tnic_snapshot_small/__init__.py
--rw-r--r--   0        0        0      168 2023-06-16 07:28:02.000000 evomap-0.3.0/src/evomap/data/tnic_snapshot_small/cluster.npy
--rw-r--r--   0        0        0      928 2023-06-16 07:28:02.000000 evomap-0.3.0/src/evomap/data/tnic_snapshot_small/labels.npy
--rw-r--r--   0        0        0      928 2023-06-16 07:28:02.000000 evomap-0.3.0/src/evomap/data/tnic_snapshot_small/sim_mat.npy
--rw-r--r--   0        0        0     3906 2023-07-28 13:52:44.656953 evomap-0.3.0/src/evomap/datasets.py
--rw-r--r--   0        0        0      224 2023-07-28 18:51:46.904816 evomap-0.3.0/src/evomap/mapping/__init__.py
--rw-r--r--   0        0        0     3563 2024-04-19 18:48:48.128748 evomap-0.3.0/src/evomap/mapping/_cmds.py
--rw-r--r--   0        0        0     7859 2024-04-19 19:03:31.317495 evomap-0.3.0/src/evomap/mapping/_mds.py
--rw-r--r--   0        0        0     8084 2024-04-19 18:49:31.177814 evomap-0.3.0/src/evomap/mapping/_optim.py
--rw-r--r--   0        0        0     4933 2024-04-19 19:11:05.208294 evomap-0.3.0/src/evomap/mapping/_sammon.py
--rw-r--r--   0        0        0     8515 2024-04-19 19:11:08.621728 evomap-0.3.0/src/evomap/mapping/_tsne.py
--rw-r--r--   0        0        0      137 2023-06-16 07:28:01.000000 evomap-0.3.0/src/evomap/mapping/evomap/__init__.py
--rw-r--r--   0        0        0    20705 2024-05-09 17:50:30.489285 evomap-0.3.0/src/evomap/mapping/evomap/_core.py
--rw-r--r--   0        0        0     4589 2023-08-03 21:25:59.633061 evomap-0.3.0/src/evomap/mapping/evomap/_evomds.py
--rw-r--r--   0        0        0     4299 2024-05-09 15:32:21.370904 evomap-0.3.0/src/evomap/mapping/evomap/_evosammon.py
--rw-r--r--   0        0        0     5549 2024-05-09 15:31:51.167197 evomap-0.3.0/src/evomap/mapping/evomap/_evotsne.py
--rw-r--r--   0        0        0   295041 2024-05-09 15:18:56.838354 evomap-0.3.0/src/evomap/mapping/evomap/_utils.c
--rw-r--r--   0        0        0     4176 2024-05-09 15:18:52.321159 evomap-0.3.0/src/evomap/mapping/evomap/_utils.pyx
--rw-r--r--   0        0        0      313 2024-05-09 15:04:34.538487 evomap-0.3.0/src/evomap/mapping/evomap/setup.py
--rw-r--r--   0        0        0    14138 2024-05-09 17:48:00.046970 evomap-0.3.0/src/evomap/metrics.py
--rw-r--r--   0        0        0    12812 2024-05-08 00:44:51.574871 evomap-0.3.0/src/evomap/preprocessing.py
--rw-r--r--   0        0        0    25829 2024-05-09 18:39:19.898198 evomap-0.3.0/src/evomap/printer.py
--rw-r--r--   0        0        0     4132 2024-04-17 21:40:12.475814 evomap-0.3.0/src/evomap/transform.py
--rw-r--r--   0        0        0     6243 1970-01-01 00:00:00.000000 evomap-0.3.0/setup.py
--rw-r--r--   0        0        0     5857 1970-01-01 00:00:00.000000 evomap-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1233 2022-06-15 16:03:22.000000 evomap-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4871 2024-05-13 14:38:16.794716 evomap-0.3.1/README.md
+-rw-r--r--   0        0        0     1252 2023-03-03 10:26:02.000000 evomap-0.3.1/build.py
+-rw-r--r--   0        0        0      922 2024-05-14 01:23:37.315407 evomap-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      293 2022-06-01 11:43:21.000000 evomap-0.3.1/src/evomap/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:16:47.000000 evomap-0.3.1/src/evomap/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 07:28:01.000000 evomap-0.3.1/src/evomap/data/cars/__init__.py
+-rw-r--r--   0        0        0     1840 2023-06-16 07:28:02.000000 evomap-0.3.1/src/evomap/data/cars/customer_preference_ratings.csv
+-rw-r--r--   0        0        0      857 2023-06-16 07:28:01.000000 evomap-0.3.1/src/evomap/data/cars/perceptual_attribute_ratings.csv
+-rw-r--r--   0        0        0     9267 2023-06-16 07:28:02.000000 evomap-0.3.1/src/evomap/data/cars/perceptual_attribute_ratings.xlsx
+-rw-r--r--   0        0        0        0 2023-06-16 07:28:01.000000 evomap-0.3.1/src/evomap/data/tnic_sample_small/__init__.py
+-rw-r--r--   0        0        0 13835652 2023-06-16 07:28:08.000000 evomap-0.3.1/src/evomap/data/tnic_sample_small/tnic_sample_small.csv
+-rw-r--r--   0        0        0 13090689 2023-06-16 07:28:08.000000 evomap-0.3.1/src/evomap/data/tnic_sample_small/tnic_sample_small_old.csv
+-rw-r--r--   0        0        0        0 2023-07-28 13:51:10.007285 evomap-0.3.1/src/evomap/data/tnic_sample_tech/__init__.py
+-rw-r--r--   0        0        0    41133 2023-07-28 13:48:28.634183 evomap-0.3.1/src/evomap/data/tnic_sample_tech/tnic_sample_technology.csv
+-rw-r--r--   0        0        0    34789 2023-07-28 13:48:28.630408 evomap-0.3.1/src/evomap/data/tnic_sample_tech/tnic_sample_technology_with_netflix.csv
+-rw-r--r--   0        0        0        0 2023-06-16 07:28:01.000000 evomap-0.3.1/src/evomap/data/tnic_snapshot/__init__.py
+-rw-r--r--   0        0        0     8864 2023-06-16 07:28:02.000000 evomap-0.3.1/src/evomap/data/tnic_snapshot/cluster.npy
+-rw-r--r--   0        0        0   122432 2023-06-16 07:28:02.000000 evomap-0.3.1/src/evomap/data/tnic_snapshot/label.npy
+-rw-r--r--   0        0        0  9539840 2023-06-16 07:28:07.000000 evomap-0.3.1/src/evomap/data/tnic_snapshot/sim_mat.npy
+-rw-r--r--   0        0        0     8864 2023-06-16 07:28:02.000000 evomap-0.3.1/src/evomap/data/tnic_snapshot/size.npy
+-rw-r--r--   0        0        0        0 2023-06-16 07:28:01.000000 evomap-0.3.1/src/evomap/data/tnic_snapshot_small/__init__.py
+-rw-r--r--   0        0        0      168 2023-06-16 07:28:02.000000 evomap-0.3.1/src/evomap/data/tnic_snapshot_small/cluster.npy
+-rw-r--r--   0        0        0      928 2023-06-16 07:28:02.000000 evomap-0.3.1/src/evomap/data/tnic_snapshot_small/labels.npy
+-rw-r--r--   0        0        0      928 2023-06-16 07:28:02.000000 evomap-0.3.1/src/evomap/data/tnic_snapshot_small/sim_mat.npy
+-rw-r--r--   0        0        0     3906 2023-07-28 13:52:44.656953 evomap-0.3.1/src/evomap/datasets.py
+-rw-r--r--   0        0        0      224 2023-07-28 18:51:46.904816 evomap-0.3.1/src/evomap/mapping/__init__.py
+-rw-r--r--   0        0        0     3563 2024-04-19 18:48:48.128748 evomap-0.3.1/src/evomap/mapping/_cmds.py
+-rw-r--r--   0        0        0     7859 2024-04-19 19:03:31.317495 evomap-0.3.1/src/evomap/mapping/_mds.py
+-rw-r--r--   0        0        0     8084 2024-04-19 18:49:31.177814 evomap-0.3.1/src/evomap/mapping/_optim.py
+-rw-r--r--   0        0        0     4933 2024-04-19 19:11:05.208294 evomap-0.3.1/src/evomap/mapping/_sammon.py
+-rw-r--r--   0        0        0     8515 2024-04-19 19:11:08.621728 evomap-0.3.1/src/evomap/mapping/_tsne.py
+-rw-r--r--   0        0        0      137 2023-06-16 07:28:01.000000 evomap-0.3.1/src/evomap/mapping/evomap/__init__.py
+-rw-r--r--   0        0        0    20705 2024-05-09 17:50:30.489285 evomap-0.3.1/src/evomap/mapping/evomap/_core.py
+-rw-r--r--   0        0        0     4589 2023-08-03 21:25:59.633061 evomap-0.3.1/src/evomap/mapping/evomap/_evomds.py
+-rw-r--r--   0        0        0     4299 2024-05-09 15:32:21.370904 evomap-0.3.1/src/evomap/mapping/evomap/_evosammon.py
+-rw-r--r--   0        0        0     5549 2024-05-09 15:31:51.167197 evomap-0.3.1/src/evomap/mapping/evomap/_evotsne.py
+-rw-r--r--   0        0        0   334022 2024-05-09 23:46:05.328308 evomap-0.3.1/src/evomap/mapping/evomap/_utils.c
+-rw-r--r--   0        0        0     4176 2024-05-09 15:18:52.321159 evomap-0.3.1/src/evomap/mapping/evomap/_utils.pyx
+-rw-r--r--   0        0        0      313 2024-05-09 15:04:34.538487 evomap-0.3.1/src/evomap/mapping/evomap/setup.py
+-rw-r--r--   0        0        0    14138 2024-05-09 17:48:00.046970 evomap-0.3.1/src/evomap/metrics.py
+-rw-r--r--   0        0        0    12812 2024-05-08 00:44:51.574871 evomap-0.3.1/src/evomap/preprocessing.py
+-rw-r--r--   0        0        0    25603 2024-05-13 14:37:45.761746 evomap-0.3.1/src/evomap/printer.py
+-rw-r--r--   0        0        0     4132 2024-04-17 21:40:12.475814 evomap-0.3.1/src/evomap/transform.py
+-rw-r--r--   0        0        0     6128 1970-01-01 00:00:00.000000 evomap-0.3.1/setup.py
+-rw-r--r--   0        0        0     5742 1970-01-01 00:00:00.000000 evomap-0.3.1/PKG-INFO
```

### Comparing `evomap-0.3.0/LICENSE` & `evomap-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/README.md` & `evomap-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 - evaluation
 - plotting
 
 Note: As of now, `evomap` is available as a ***pre-release version*** and parts of `evomap` are still under active development. For any bug reports or feature requests, <a href = 'mailto:mpmatthe@iu.edu'>please get in touch</a>.
 
 ## Installation
 
-This pre-release is available via GitHub. Stay tuned for a release on PyPi, which is coming soon! 
+This pre-release is available via PyPi. 
 
 To install `evomap` run
 ```bash
-pip install git+https://github.com/mpmatthe/evomap
+pip install evomap
 ```
 
-`evomap` requires Python version 3.9. We recommend using Python within a virtual environment, for instance via conda:
+`evomap` works best with Python version 3.9. We recommend using Python within a virtual environment, for instance via conda:
 ```bash
 conda create -n evomap python=3.9
 conda activate evomap
-pip install git+https://github.com/mpmatthe/evomap
+pip install evomap
 ```
 
 **Note:** Currently, `evomap` builds its C extensions upon installation on the system. Thus, it requires a C compiler to be present. The right C compiler depends upon your system, e.g. GCC on Linux or MSVC on Windows. For details, see <a href = 'https://cython.readthedocs.io/en/latest/src/quickstart/install.html'>the Cython documentation</a>. In future versions, extensions will be pre-compiled.
 
 ## Usage
 
 The following tutorials provide a good starting point for using `evomap`.
```

### Comparing `evomap-0.3.0/build.py` & `evomap-0.3.1/build.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/pyproject.toml` & `evomap-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "numpy==1.21.6", "poetry-core>=1.4.0", "Cython==0.29.33"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "evomap"
-version = "0.3.0"
+version = "0.3.1"
 description = "A Python Toolbox for Mapping Evolving Relationship Data"
 authors = ["Maximilian Matthe <mpmatthe@iu.edu>, Daniel M. Ringel <>, and Bernd Skiera <>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.build]
 generate-setup-file = true
```

### Comparing `evomap-0.3.0/src/evomap/data/cars/customer_preference_ratings.csv` & `evomap-0.3.1/src/evomap/data/cars/customer_preference_ratings.csv`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/data/cars/perceptual_attribute_ratings.csv` & `evomap-0.3.1/src/evomap/data/cars/perceptual_attribute_ratings.csv`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/data/cars/perceptual_attribute_ratings.xlsx` & `evomap-0.3.1/src/evomap/data/cars/perceptual_attribute_ratings.xlsx`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/data/tnic_sample_small/tnic_sample_small.csv` & `evomap-0.3.1/src/evomap/data/tnic_sample_small/tnic_sample_small.csv`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/data/tnic_sample_small/tnic_sample_small_old.csv` & `evomap-0.3.1/src/evomap/data/tnic_sample_small/tnic_sample_small_old.csv`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/data/tnic_sample_tech/tnic_sample_technology.csv` & `evomap-0.3.1/src/evomap/data/tnic_sample_tech/tnic_sample_technology.csv`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/data/tnic_sample_tech/tnic_sample_technology_with_netflix.csv` & `evomap-0.3.1/src/evomap/data/tnic_sample_tech/tnic_sample_technology_with_netflix.csv`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/data/tnic_snapshot/cluster.npy` & `evomap-0.3.1/src/evomap/data/tnic_snapshot/cluster.npy`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/data/tnic_snapshot/label.npy` & `evomap-0.3.1/src/evomap/data/tnic_snapshot/label.npy`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/data/tnic_snapshot/sim_mat.npy` & `evomap-0.3.1/src/evomap/data/tnic_snapshot/sim_mat.npy`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/data/tnic_snapshot/size.npy` & `evomap-0.3.1/src/evomap/data/tnic_snapshot/size.npy`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/data/tnic_snapshot_small/labels.npy` & `evomap-0.3.1/src/evomap/data/tnic_snapshot_small/labels.npy`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/data/tnic_snapshot_small/sim_mat.npy` & `evomap-0.3.1/src/evomap/data/tnic_snapshot_small/sim_mat.npy`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/datasets.py` & `evomap-0.3.1/src/evomap/datasets.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/mapping/_cmds.py` & `evomap-0.3.1/src/evomap/mapping/_cmds.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/mapping/_mds.py` & `evomap-0.3.1/src/evomap/mapping/_mds.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/mapping/_optim.py` & `evomap-0.3.1/src/evomap/mapping/_optim.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/mapping/_sammon.py` & `evomap-0.3.1/src/evomap/mapping/_sammon.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/mapping/_tsne.py` & `evomap-0.3.1/src/evomap/mapping/_tsne.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/mapping/evomap/_core.py` & `evomap-0.3.1/src/evomap/mapping/evomap/_core.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/mapping/evomap/_evomds.py` & `evomap-0.3.1/src/evomap/mapping/evomap/_evomds.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/mapping/evomap/_evosammon.py` & `evomap-0.3.1/src/evomap/mapping/evomap/_evosammon.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/mapping/evomap/_evotsne.py` & `evomap-0.3.1/src/evomap/mapping/evomap/_evotsne.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/mapping/evomap/_utils.c` & `evomap-0.3.1/src/evomap/mapping/evomap/_utils.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 /* Generated by Cython 0.29.33 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/Users/mpmatthe/anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/Users/mpmatthe/anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/Users/mpmatthe/anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/Users/mpmatthe/anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/Users/mpmatthe/anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/core/include/numpy/npy_math.h",
-            "/Users/mpmatthe/anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/core/include/numpy/npy_math.h",
+            "/private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/Users/mpmatthe/anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/core/include"
+            "/private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/core/include"
         ],
-        "name": "_utils",
+        "name": "evomap.mapping.evomap._utils",
         "sources": [
-            "_utils.pyx"
+            "src/evomap/mapping/evomap/_utils.pyx"
         ]
     },
-    "module_name": "_utils"
+    "module_name": "evomap.mapping.evomap._utils"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
@@ -757,16 +757,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE___utils
-#define __PYX_HAVE_API___utils
+#define __PYX_HAVE__evomap__mapping__evomap___utils
+#define __PYX_HAVE_API__evomap__mapping__evomap___utils
 /* Early includes */
 #include <math.h>
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
 #include "numpy/ndarrayobject.h"
 #include "numpy/ndarraytypes.h"
@@ -1003,15 +1003,15 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "_utils.pyx",
+  "src/evomap/mapping/evomap/_utils.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 /* BufferFormatStructs.proto */
 #define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
@@ -1044,195 +1044,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":693
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":700
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":705
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":716
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":720
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":723
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":727
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1259,42 +1259,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":731
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":733
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1369,14 +1369,282 @@
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
+/* Profile.proto */
+#ifndef CYTHON_PROFILE
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
+  #define CYTHON_PROFILE 0
+#else
+  #define CYTHON_PROFILE 1
+#endif
+#endif
+#ifndef CYTHON_TRACE_NOGIL
+  #define CYTHON_TRACE_NOGIL 0
+#else
+  #if CYTHON_TRACE_NOGIL && !defined(CYTHON_TRACE)
+    #define CYTHON_TRACE 1
+  #endif
+#endif
+#ifndef CYTHON_TRACE
+  #define CYTHON_TRACE 0
+#endif
+#if CYTHON_TRACE
+  #undef CYTHON_PROFILE_REUSE_FRAME
+#endif
+#ifndef CYTHON_PROFILE_REUSE_FRAME
+  #define CYTHON_PROFILE_REUSE_FRAME 0
+#endif
+#if CYTHON_PROFILE || CYTHON_TRACE
+  #include "compile.h"
+  #include "frameobject.h"
+  #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #if CYTHON_PROFILE_REUSE_FRAME
+    #define CYTHON_FRAME_MODIFIER static
+    #define CYTHON_FRAME_DEL(frame)
+  #else
+    #define CYTHON_FRAME_MODIFIER
+    #define CYTHON_FRAME_DEL(frame) Py_CLEAR(frame)
+  #endif
+  #define __Pyx_TraceDeclarations\
+      static PyCodeObject *__pyx_frame_code = NULL;\
+      CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
+      int __Pyx_use_tracing = 0;
+  #define __Pyx_TraceFrameInit(codeobj)\
+      if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
+#if PY_VERSION_HEX >= 0x030b00a2
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     (unlikely((tstate)->cframe->use_tracing) &&\
+         (!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
+  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
+#elif PY_VERSION_HEX >= 0x030a00b1
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     (unlikely((tstate)->cframe->use_tracing) &&\
+         (!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #define __Pyx_EnterTracing(tstate)\
+      do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
+  #define __Pyx_LeaveTracing(tstate)\
+      do {\
+          tstate->tracing--;\
+          tstate->cframe->use_tracing = ((CYTHON_TRACE && tstate->c_tracefunc != NULL)\
+                                 || tstate->c_profilefunc != NULL);\
+      } while (0)
+#else
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     (unlikely((tstate)->use_tracing) &&\
+         (!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #define __Pyx_EnterTracing(tstate)\
+      do { tstate->tracing++; tstate->use_tracing = 0; } while (0)
+  #define __Pyx_LeaveTracing(tstate)\
+      do {\
+          tstate->tracing--;\
+          tstate->use_tracing = ((CYTHON_TRACE && tstate->c_tracefunc != NULL)\
+                                         || tstate->c_profilefunc != NULL);\
+      } while (0)
+#endif
+  #ifdef WITH_THREAD
+  #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)\
+  if (nogil) {\
+      if (CYTHON_TRACE_NOGIL) {\
+          PyThreadState *tstate;\
+          PyGILState_STATE state = PyGILState_Ensure();\
+          tstate = __Pyx_PyThreadState_Current;\
+          if (__Pyx_IsTracing(tstate, 1, 1)) {\
+              __Pyx_use_tracing = __Pyx_TraceSetupAndCall(&__pyx_frame_code, &__pyx_frame, tstate, funcname, srcfile, firstlineno);\
+          }\
+          PyGILState_Release(state);\
+          if (unlikely(__Pyx_use_tracing < 0)) goto_error;\
+      }\
+  } else {\
+      PyThreadState* tstate = PyThreadState_GET();\
+      if (__Pyx_IsTracing(tstate, 1, 1)) {\
+          __Pyx_use_tracing = __Pyx_TraceSetupAndCall(&__pyx_frame_code, &__pyx_frame, tstate, funcname, srcfile, firstlineno);\
+          if (unlikely(__Pyx_use_tracing < 0)) goto_error;\
+      }\
+  }
+  #else
+  #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)\
+  {   PyThreadState* tstate = PyThreadState_GET();\
+      if (__Pyx_IsTracing(tstate, 1, 1)) {\
+          __Pyx_use_tracing = __Pyx_TraceSetupAndCall(&__pyx_frame_code, &__pyx_frame, tstate, funcname, srcfile, firstlineno);\
+          if (unlikely(__Pyx_use_tracing < 0)) goto_error;\
+      }\
+  }
+  #endif
+  #define __Pyx_TraceException()\
+  if (likely(!__Pyx_use_tracing)); else {\
+      PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+      if (__Pyx_IsTracing(tstate, 0, 1)) {\
+          __Pyx_EnterTracing(tstate);\
+          PyObject *exc_info = __Pyx_GetExceptionTuple(tstate);\
+          if (exc_info) {\
+              if (CYTHON_TRACE && tstate->c_tracefunc)\
+                  tstate->c_tracefunc(\
+                      tstate->c_traceobj, __pyx_frame, PyTrace_EXCEPTION, exc_info);\
+              tstate->c_profilefunc(\
+                  tstate->c_profileobj, __pyx_frame, PyTrace_EXCEPTION, exc_info);\
+              Py_DECREF(exc_info);\
+          }\
+          __Pyx_LeaveTracing(tstate);\
+      }\
+  }
+  static void __Pyx_call_return_trace_func(PyThreadState *tstate, PyFrameObject *frame, PyObject *result) {
+      PyObject *type, *value, *traceback;
+      __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
+      __Pyx_EnterTracing(tstate);
+      if (CYTHON_TRACE && tstate->c_tracefunc)
+          tstate->c_tracefunc(tstate->c_traceobj, frame, PyTrace_RETURN, result);
+      if (tstate->c_profilefunc)
+          tstate->c_profilefunc(tstate->c_profileobj, frame, PyTrace_RETURN, result);
+      CYTHON_FRAME_DEL(frame);
+      __Pyx_LeaveTracing(tstate);
+      __Pyx_ErrRestoreInState(tstate, type, value, traceback);
+  }
+  #ifdef WITH_THREAD
+  #define __Pyx_TraceReturn(result, nogil)\
+  if (likely(!__Pyx_use_tracing)); else {\
+      if (nogil) {\
+          if (CYTHON_TRACE_NOGIL) {\
+              PyThreadState *tstate;\
+              PyGILState_STATE state = PyGILState_Ensure();\
+              tstate = __Pyx_PyThreadState_Current;\
+              if (__Pyx_IsTracing(tstate, 0, 0)) {\
+                  __Pyx_call_return_trace_func(tstate, __pyx_frame, (PyObject*)result);\
+              }\
+              PyGILState_Release(state);\
+          }\
+      } else {\
+          PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+          if (__Pyx_IsTracing(tstate, 0, 0)) {\
+              __Pyx_call_return_trace_func(tstate, __pyx_frame, (PyObject*)result);\
+          }\
+      }\
+  }
+  #else
+  #define __Pyx_TraceReturn(result, nogil)\
+  if (likely(!__Pyx_use_tracing)); else {\
+      PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+      if (__Pyx_IsTracing(tstate, 0, 0)) {\
+          __Pyx_call_return_trace_func(tstate, __pyx_frame, (PyObject*)result);\
+      }\
+  }
+  #endif
+  static PyCodeObject *__Pyx_createFrameCodeObject(const char *funcname, const char *srcfile, int firstlineno);
+  static int __Pyx_TraceSetupAndCall(PyCodeObject** code, PyFrameObject** frame, PyThreadState* tstate, const char *funcname, const char *srcfile, int firstlineno);
+#else
+  #define __Pyx_TraceDeclarations
+  #define __Pyx_TraceFrameInit(codeobj)
+  #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)   if ((1)); else goto_error;
+  #define __Pyx_TraceException()
+  #define __Pyx_TraceReturn(result, nogil)
+#endif
+#if CYTHON_TRACE
+  static int __Pyx_call_line_trace_func(PyThreadState *tstate, PyFrameObject *frame, int lineno) {
+      int ret;
+      PyObject *type, *value, *traceback;
+      __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
+      __Pyx_PyFrame_SetLineNumber(frame, lineno);
+      __Pyx_EnterTracing(tstate);
+      ret = tstate->c_tracefunc(tstate->c_traceobj, frame, PyTrace_LINE, NULL);
+      __Pyx_LeaveTracing(tstate);
+      if (likely(!ret)) {
+          __Pyx_ErrRestoreInState(tstate, type, value, traceback);
+      } else {
+          Py_XDECREF(type);
+          Py_XDECREF(value);
+          Py_XDECREF(traceback);
+      }
+      return ret;
+  }
+  #ifdef WITH_THREAD
+  #define __Pyx_TraceLine(lineno, nogil, goto_error)\
+  if (likely(!__Pyx_use_tracing)); else {\
+      if (nogil) {\
+          if (CYTHON_TRACE_NOGIL) {\
+              int ret = 0;\
+              PyThreadState *tstate;\
+              PyGILState_STATE state = PyGILState_Ensure();\
+              tstate = __Pyx_PyThreadState_Current;\
+              if (__Pyx_IsTracing(tstate, 0, 0) && tstate->c_tracefunc && __pyx_frame->f_trace) {\
+                  ret = __Pyx_call_line_trace_func(tstate, __pyx_frame, lineno);\
+              }\
+              PyGILState_Release(state);\
+              if (unlikely(ret)) goto_error;\
+          }\
+      } else {\
+          PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+          if (__Pyx_IsTracing(tstate, 0, 0) && tstate->c_tracefunc && __pyx_frame->f_trace) {\
+              int ret = __Pyx_call_line_trace_func(tstate, __pyx_frame, lineno);\
+              if (unlikely(ret)) goto_error;\
+          }\
+      }\
+  }
+  #else
+  #define __Pyx_TraceLine(lineno, nogil, goto_error)\
+  if (likely(!__Pyx_use_tracing)); else {\
+      PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+      if (__Pyx_IsTracing(tstate, 0, 0) && tstate->c_tracefunc && __pyx_frame->f_trace) {\
+          int ret = __Pyx_call_line_trace_func(tstate, __pyx_frame, lineno);\
+          if (unlikely(ret)) goto_error;\
+      }\
+  }
+  #endif
+#else
+  #define __Pyx_TraceLine(lineno, nogil, goto_error)   if ((1)); else goto_error;
+#endif
+
 /* IsLittleEndian.proto */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
 
 /* BufferFormatCheck.proto */
 static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts);
 static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
                               __Pyx_BufFmt_StackElem* stack,
@@ -1522,50 +1790,14 @@
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
-#endif
-
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
-#endif
-
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
@@ -1576,14 +1808,19 @@
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1849,25 +2086,25 @@
 static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
 static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 static CYTHON_INLINE int __pyx_f_5numpy_import_array(void); /*proto*/
 
-/* Module declarations from '_utils' */
-static float __pyx_v_6_utils_EPSILON_DBL;
-static float __pyx_v_6_utils_PERPLEXITY_TOLERANCE;
-static PyArrayObject *__pyx_f_6_utils__binary_search_perplexity(PyArrayObject *, float, int, int __pyx_skip_dispatch); /*proto*/
+/* Module declarations from 'evomap.mapping.evomap._utils' */
+static float __pyx_v_6evomap_7mapping_6evomap_6_utils_EPSILON_DBL;
+static float __pyx_v_6evomap_7mapping_6evomap_6_utils_PERPLEXITY_TOLERANCE;
+static PyArrayObject *__pyx_f_6evomap_7mapping_6evomap_6_utils__binary_search_perplexity(PyArrayObject *, float, int, int __pyx_skip_dispatch); /*proto*/
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_float32_t = { "float32_t", NULL, sizeof(__pyx_t_5numpy_float32_t), { 0 }, 0, 'R', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t = { "float64_t", NULL, sizeof(__pyx_t_5numpy_float64_t), { 0 }, 0, 'R', 0, 0 };
-#define __Pyx_MODULE_NAME "_utils"
-extern int __pyx_module_is_main__utils;
-int __pyx_module_is_main__utils = 0;
+#define __Pyx_MODULE_NAME "evomap.mapping.evomap._utils"
+extern int __pyx_module_is_main_evomap__mapping__evomap___utils;
+int __pyx_module_is_main_evomap__mapping__evomap___utils = 0;
 
-/* Implementation of '_utils' */
+/* Implementation of 'evomap.mapping.evomap._utils' */
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_print;
 static PyObject *__pyx_builtin_ImportError;
 static const char __pyx_k_[] = " / ";
 static const char __pyx_k_d[] = "d";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_main[] = "__main__";
@@ -1910,29 +2147,29 @@
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_sqdistances;
 static PyObject *__pyx_kp_u_t_SNE_Computed_conditional_prob;
 static PyObject *__pyx_kp_u_t_SNE_Mean_sigma_f;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_verbose;
 static PyObject *__pyx_n_s_zeros;
-static PyObject *__pyx_pf_6_utils__binary_search_perplexity(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_sqdistances, float __pyx_v_desired_perplexity, int __pyx_v_verbose); /* proto */
+static PyObject *__pyx_pf_6evomap_7mapping_6evomap_6_utils__binary_search_perplexity(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_sqdistances, float __pyx_v_desired_perplexity, int __pyx_v_verbose); /* proto */
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 /* Late includes */
 
-/* "_utils.pyx":23
+/* "evomap/mapping/evomap/_utils.pyx":23
  * cdef float PERPLEXITY_TOLERANCE = 1e-5
  * 
  * cpdef np.ndarray[np.float32_t, ndim=2] _binary_search_perplexity(             # <<<<<<<<<<<<<<
  *         np.ndarray[np.float32_t, ndim=2] sqdistances,
  *         float desired_perplexity,
  */
 
-static PyObject *__pyx_pw_6_utils_1_binary_search_perplexity(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyArrayObject *__pyx_f_6_utils__binary_search_perplexity(PyArrayObject *__pyx_v_sqdistances, float __pyx_v_desired_perplexity, int __pyx_v_verbose, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_6evomap_7mapping_6evomap_6_utils_1_binary_search_perplexity(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyArrayObject *__pyx_f_6evomap_7mapping_6evomap_6_utils__binary_search_perplexity(PyArrayObject *__pyx_v_sqdistances, float __pyx_v_desired_perplexity, int __pyx_v_verbose, CYTHON_UNUSED int __pyx_skip_dispatch) {
   long __pyx_v_n_steps;
   long __pyx_v_n_samples;
   long __pyx_v_n_neighbors;
   int __pyx_v_using_neighbors;
   double __pyx_v_beta;
   double __pyx_v_beta_min;
   double __pyx_v_beta_max;
@@ -1947,14 +2184,15 @@
   CYTHON_UNUSED long __pyx_v_l;
   PyArrayObject *__pyx_v_P = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_P;
   __Pyx_Buffer __pyx_pybuffer_P;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sqdistances;
   __Pyx_Buffer __pyx_pybuffer_sqdistances;
   PyArrayObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyArrayObject *__pyx_t_6 = NULL;
@@ -1976,152 +2214,164 @@
   Py_ssize_t __pyx_t_22;
   Py_ssize_t __pyx_t_23;
   Py_UCS4 __pyx_t_24;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_binary_search_perplexity", 0);
+  __Pyx_TraceCall("_binary_search_perplexity", __pyx_f[0], 23, 0, __PYX_ERR(0, 23, __pyx_L1_error));
   __pyx_pybuffer_P.pybuffer.buf = NULL;
   __pyx_pybuffer_P.refcount = 0;
   __pyx_pybuffernd_P.data = NULL;
   __pyx_pybuffernd_P.rcbuffer = &__pyx_pybuffer_P;
   __pyx_pybuffer_sqdistances.pybuffer.buf = NULL;
   __pyx_pybuffer_sqdistances.refcount = 0;
   __pyx_pybuffernd_sqdistances.data = NULL;
   __pyx_pybuffernd_sqdistances.rcbuffer = &__pyx_pybuffer_sqdistances;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_sqdistances.rcbuffer->pybuffer, (PyObject*)__pyx_v_sqdistances, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float32_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 23, __pyx_L1_error)
   }
   __pyx_pybuffernd_sqdistances.diminfo[0].strides = __pyx_pybuffernd_sqdistances.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_sqdistances.diminfo[0].shape = __pyx_pybuffernd_sqdistances.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_sqdistances.diminfo[1].strides = __pyx_pybuffernd_sqdistances.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_sqdistances.diminfo[1].shape = __pyx_pybuffernd_sqdistances.rcbuffer->pybuffer.shape[1];
 
-  /* "_utils.pyx":47
+  /* "evomap/mapping/evomap/_utils.pyx":47
  *     """
  *     # Maximum number of binary search steps
  *     cdef long n_steps = 100             # <<<<<<<<<<<<<<
  * 
  *     cdef long n_samples = sqdistances.shape[0]
  */
+  __Pyx_TraceLine(47,0,__PYX_ERR(0, 47, __pyx_L1_error))
   __pyx_v_n_steps = 0x64;
 
-  /* "_utils.pyx":49
+  /* "evomap/mapping/evomap/_utils.pyx":49
  *     cdef long n_steps = 100
  * 
  *     cdef long n_samples = sqdistances.shape[0]             # <<<<<<<<<<<<<<
  *     cdef long n_neighbors = sqdistances.shape[1]
  *     cdef int using_neighbors = n_neighbors < n_samples
  */
+  __Pyx_TraceLine(49,0,__PYX_ERR(0, 49, __pyx_L1_error))
   __pyx_v_n_samples = (__pyx_v_sqdistances->dimensions[0]);
 
-  /* "_utils.pyx":50
+  /* "evomap/mapping/evomap/_utils.pyx":50
  * 
  *     cdef long n_samples = sqdistances.shape[0]
  *     cdef long n_neighbors = sqdistances.shape[1]             # <<<<<<<<<<<<<<
  *     cdef int using_neighbors = n_neighbors < n_samples
  *     # Precisions of conditional Gaussian distributions
  */
+  __Pyx_TraceLine(50,0,__PYX_ERR(0, 50, __pyx_L1_error))
   __pyx_v_n_neighbors = (__pyx_v_sqdistances->dimensions[1]);
 
-  /* "_utils.pyx":51
+  /* "evomap/mapping/evomap/_utils.pyx":51
  *     cdef long n_samples = sqdistances.shape[0]
  *     cdef long n_neighbors = sqdistances.shape[1]
  *     cdef int using_neighbors = n_neighbors < n_samples             # <<<<<<<<<<<<<<
  *     # Precisions of conditional Gaussian distributions
  *     cdef double beta
  */
+  __Pyx_TraceLine(51,0,__PYX_ERR(0, 51, __pyx_L1_error))
   __pyx_v_using_neighbors = (__pyx_v_n_neighbors < __pyx_v_n_samples);
 
-  /* "_utils.pyx":56
+  /* "evomap/mapping/evomap/_utils.pyx":56
  *     cdef double beta_min
  *     cdef double beta_max
  *     cdef double beta_sum = 0.0             # <<<<<<<<<<<<<<
  * 
  *     # Use log scale
  */
+  __Pyx_TraceLine(56,0,__PYX_ERR(0, 56, __pyx_L1_error))
   __pyx_v_beta_sum = 0.0;
 
-  /* "_utils.pyx":59
+  /* "evomap/mapping/evomap/_utils.pyx":59
  * 
  *     # Use log scale
  *     cdef double desired_entropy = math.log(desired_perplexity)             # <<<<<<<<<<<<<<
  *     cdef double entropy_diff
  * 
  */
+  __Pyx_TraceLine(59,0,__PYX_ERR(0, 59, __pyx_L1_error))
   __pyx_v_desired_entropy = log(__pyx_v_desired_perplexity);
 
-  /* "_utils.pyx":69
+  /* "evomap/mapping/evomap/_utils.pyx":69
  *     # This array is later used as a 32bit array. It has multiple intermediate
  *     # floating point additions that benefit from the extra precision
  *     cdef np.ndarray[np.float64_t, ndim=2] P = np.zeros(             # <<<<<<<<<<<<<<
  *         (n_samples, n_neighbors), dtype=np.float64)
  * 
  */
+  __Pyx_TraceLine(69,0,__PYX_ERR(0, 69, __pyx_L1_error))
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_utils.pyx":70
+  /* "evomap/mapping/evomap/_utils.pyx":70
  *     # floating point additions that benefit from the extra precision
  *     cdef np.ndarray[np.float64_t, ndim=2] P = np.zeros(
  *         (n_samples, n_neighbors), dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(n_samples):
  */
+  __Pyx_TraceLine(70,0,__PYX_ERR(0, 70, __pyx_L1_error))
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_n_samples); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_n_neighbors); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
 
-  /* "_utils.pyx":69
+  /* "evomap/mapping/evomap/_utils.pyx":69
  *     # This array is later used as a 32bit array. It has multiple intermediate
  *     # floating point additions that benefit from the extra precision
  *     cdef np.ndarray[np.float64_t, ndim=2] P = np.zeros(             # <<<<<<<<<<<<<<
  *         (n_samples, n_neighbors), dtype=np.float64)
  * 
  */
+  __Pyx_TraceLine(69,0,__PYX_ERR(0, 69, __pyx_L1_error))
   __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "_utils.pyx":70
+  /* "evomap/mapping/evomap/_utils.pyx":70
  *     # floating point additions that benefit from the extra precision
  *     cdef np.ndarray[np.float64_t, ndim=2] P = np.zeros(
  *         (n_samples, n_neighbors), dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(n_samples):
  */
+  __Pyx_TraceLine(70,0,__PYX_ERR(0, 70, __pyx_L1_error))
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "_utils.pyx":69
+  /* "evomap/mapping/evomap/_utils.pyx":69
  *     # This array is later used as a 32bit array. It has multiple intermediate
  *     # floating point additions that benefit from the extra precision
  *     cdef np.ndarray[np.float64_t, ndim=2] P = np.zeros(             # <<<<<<<<<<<<<<
  *         (n_samples, n_neighbors), dtype=np.float64)
  * 
  */
+  __Pyx_TraceLine(69,0,__PYX_ERR(0, 69, __pyx_L1_error))
   __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 69, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
@@ -2133,111 +2383,120 @@
     } else {__pyx_pybuffernd_P.diminfo[0].strides = __pyx_pybuffernd_P.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_P.diminfo[0].shape = __pyx_pybuffernd_P.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_P.diminfo[1].strides = __pyx_pybuffernd_P.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_P.diminfo[1].shape = __pyx_pybuffernd_P.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_P = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "_utils.pyx":72
+  /* "evomap/mapping/evomap/_utils.pyx":72
  *         (n_samples, n_neighbors), dtype=np.float64)
  * 
  *     for i in range(n_samples):             # <<<<<<<<<<<<<<
  *         beta_min = -NPY_INFINITY
  *         beta_max = NPY_INFINITY
  */
+  __Pyx_TraceLine(72,0,__PYX_ERR(0, 72, __pyx_L1_error))
   __pyx_t_7 = __pyx_v_n_samples;
   __pyx_t_8 = __pyx_t_7;
   for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
     __pyx_v_i = __pyx_t_9;
 
-    /* "_utils.pyx":73
+    /* "evomap/mapping/evomap/_utils.pyx":73
  * 
  *     for i in range(n_samples):
  *         beta_min = -NPY_INFINITY             # <<<<<<<<<<<<<<
  *         beta_max = NPY_INFINITY
  *         beta = 1.0
  */
+    __Pyx_TraceLine(73,0,__PYX_ERR(0, 73, __pyx_L1_error))
     __pyx_v_beta_min = (-NPY_INFINITY);
 
-    /* "_utils.pyx":74
+    /* "evomap/mapping/evomap/_utils.pyx":74
  *     for i in range(n_samples):
  *         beta_min = -NPY_INFINITY
  *         beta_max = NPY_INFINITY             # <<<<<<<<<<<<<<
  *         beta = 1.0
  * 
  */
+    __Pyx_TraceLine(74,0,__PYX_ERR(0, 74, __pyx_L1_error))
     __pyx_v_beta_max = NPY_INFINITY;
 
-    /* "_utils.pyx":75
+    /* "evomap/mapping/evomap/_utils.pyx":75
  *         beta_min = -NPY_INFINITY
  *         beta_max = NPY_INFINITY
  *         beta = 1.0             # <<<<<<<<<<<<<<
  * 
  *         # Binary search of precision for i-th conditional distribution
  */
+    __Pyx_TraceLine(75,0,__PYX_ERR(0, 75, __pyx_L1_error))
     __pyx_v_beta = 1.0;
 
-    /* "_utils.pyx":78
+    /* "evomap/mapping/evomap/_utils.pyx":78
  * 
  *         # Binary search of precision for i-th conditional distribution
  *         for l in range(n_steps):             # <<<<<<<<<<<<<<
  *             # Compute current entropy and corresponding probabilities
  *             # computed just over the nearest neighbors or over all data
  */
+    __Pyx_TraceLine(78,0,__PYX_ERR(0, 78, __pyx_L1_error))
     __pyx_t_10 = __pyx_v_n_steps;
     __pyx_t_11 = __pyx_t_10;
     for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
       __pyx_v_l = __pyx_t_12;
 
-      /* "_utils.pyx":82
+      /* "evomap/mapping/evomap/_utils.pyx":82
  *             # computed just over the nearest neighbors or over all data
  *             # if we're not using neighbors
  *             sum_Pi = 0.0             # <<<<<<<<<<<<<<
  *             for j in range(n_neighbors):
  *                 if j != i or using_neighbors:
  */
+      __Pyx_TraceLine(82,0,__PYX_ERR(0, 82, __pyx_L1_error))
       __pyx_v_sum_Pi = 0.0;
 
-      /* "_utils.pyx":83
+      /* "evomap/mapping/evomap/_utils.pyx":83
  *             # if we're not using neighbors
  *             sum_Pi = 0.0
  *             for j in range(n_neighbors):             # <<<<<<<<<<<<<<
  *                 if j != i or using_neighbors:
  *                     P[i, j] = math.exp(-sqdistances[i, j] * beta)
  */
+      __Pyx_TraceLine(83,0,__PYX_ERR(0, 83, __pyx_L1_error))
       __pyx_t_13 = __pyx_v_n_neighbors;
       __pyx_t_14 = __pyx_t_13;
       for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
         __pyx_v_j = __pyx_t_15;
 
-        /* "_utils.pyx":84
+        /* "evomap/mapping/evomap/_utils.pyx":84
  *             sum_Pi = 0.0
  *             for j in range(n_neighbors):
  *                 if j != i or using_neighbors:             # <<<<<<<<<<<<<<
  *                     P[i, j] = math.exp(-sqdistances[i, j] * beta)
  *                     sum_Pi += P[i, j]
  */
+        __Pyx_TraceLine(84,0,__PYX_ERR(0, 84, __pyx_L1_error))
         __pyx_t_17 = ((__pyx_v_j != __pyx_v_i) != 0);
         if (!__pyx_t_17) {
         } else {
           __pyx_t_16 = __pyx_t_17;
           goto __pyx_L10_bool_binop_done;
         }
         __pyx_t_17 = (__pyx_v_using_neighbors != 0);
         __pyx_t_16 = __pyx_t_17;
         __pyx_L10_bool_binop_done:;
         if (__pyx_t_16) {
 
-          /* "_utils.pyx":85
+          /* "evomap/mapping/evomap/_utils.pyx":85
  *             for j in range(n_neighbors):
  *                 if j != i or using_neighbors:
  *                     P[i, j] = math.exp(-sqdistances[i, j] * beta)             # <<<<<<<<<<<<<<
  *                     sum_Pi += P[i, j]
  * 
  */
+          __Pyx_TraceLine(85,0,__PYX_ERR(0, 85, __pyx_L1_error))
           __pyx_t_18 = __pyx_v_i;
           __pyx_t_19 = __pyx_v_j;
           __pyx_t_20 = -1;
           if (__pyx_t_18 < 0) {
             __pyx_t_18 += __pyx_pybuffernd_sqdistances.diminfo[0].shape;
             if (unlikely(__pyx_t_18 < 0)) __pyx_t_20 = 0;
           } else if (unlikely(__pyx_t_18 >= __pyx_pybuffernd_sqdistances.diminfo[0].shape)) __pyx_t_20 = 0;
@@ -2262,21 +2521,22 @@
           } else if (unlikely(__pyx_t_22 >= __pyx_pybuffernd_P.diminfo[1].shape)) __pyx_t_20 = 1;
           if (unlikely(__pyx_t_20 != -1)) {
             __Pyx_RaiseBufferIndexError(__pyx_t_20);
             __PYX_ERR(0, 85, __pyx_L1_error)
           }
           *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_P.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_P.diminfo[0].strides, __pyx_t_22, __pyx_pybuffernd_P.diminfo[1].strides) = exp(((-(*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float32_t *, __pyx_pybuffernd_sqdistances.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_sqdistances.diminfo[0].strides, __pyx_t_19, __pyx_pybuffernd_sqdistances.diminfo[1].strides))) * __pyx_v_beta));
 
-          /* "_utils.pyx":86
+          /* "evomap/mapping/evomap/_utils.pyx":86
  *                 if j != i or using_neighbors:
  *                     P[i, j] = math.exp(-sqdistances[i, j] * beta)
  *                     sum_Pi += P[i, j]             # <<<<<<<<<<<<<<
  * 
  *             if sum_Pi == 0.0:
  */
+          __Pyx_TraceLine(86,0,__PYX_ERR(0, 86, __pyx_L1_error))
           __pyx_t_19 = __pyx_v_i;
           __pyx_t_18 = __pyx_v_j;
           __pyx_t_20 = -1;
           if (__pyx_t_19 < 0) {
             __pyx_t_19 += __pyx_pybuffernd_P.diminfo[0].shape;
             if (unlikely(__pyx_t_19 < 0)) __pyx_t_20 = 0;
           } else if (unlikely(__pyx_t_19 >= __pyx_pybuffernd_P.diminfo[0].shape)) __pyx_t_20 = 0;
@@ -2286,80 +2546,85 @@
           } else if (unlikely(__pyx_t_18 >= __pyx_pybuffernd_P.diminfo[1].shape)) __pyx_t_20 = 1;
           if (unlikely(__pyx_t_20 != -1)) {
             __Pyx_RaiseBufferIndexError(__pyx_t_20);
             __PYX_ERR(0, 86, __pyx_L1_error)
           }
           __pyx_v_sum_Pi = (__pyx_v_sum_Pi + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_P.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_P.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_P.diminfo[1].strides)));
 
-          /* "_utils.pyx":84
+          /* "evomap/mapping/evomap/_utils.pyx":84
  *             sum_Pi = 0.0
  *             for j in range(n_neighbors):
  *                 if j != i or using_neighbors:             # <<<<<<<<<<<<<<
  *                     P[i, j] = math.exp(-sqdistances[i, j] * beta)
  *                     sum_Pi += P[i, j]
  */
         }
       }
 
-      /* "_utils.pyx":88
+      /* "evomap/mapping/evomap/_utils.pyx":88
  *                     sum_Pi += P[i, j]
  * 
  *             if sum_Pi == 0.0:             # <<<<<<<<<<<<<<
  *                 sum_Pi = EPSILON_DBL
  *             sum_disti_Pi = 0.0
  */
+      __Pyx_TraceLine(88,0,__PYX_ERR(0, 88, __pyx_L1_error))
       __pyx_t_16 = ((__pyx_v_sum_Pi == 0.0) != 0);
       if (__pyx_t_16) {
 
-        /* "_utils.pyx":89
+        /* "evomap/mapping/evomap/_utils.pyx":89
  * 
  *             if sum_Pi == 0.0:
  *                 sum_Pi = EPSILON_DBL             # <<<<<<<<<<<<<<
  *             sum_disti_Pi = 0.0
  * 
  */
-        __pyx_v_sum_Pi = __pyx_v_6_utils_EPSILON_DBL;
+        __Pyx_TraceLine(89,0,__PYX_ERR(0, 89, __pyx_L1_error))
+        __pyx_v_sum_Pi = __pyx_v_6evomap_7mapping_6evomap_6_utils_EPSILON_DBL;
 
-        /* "_utils.pyx":88
+        /* "evomap/mapping/evomap/_utils.pyx":88
  *                     sum_Pi += P[i, j]
  * 
  *             if sum_Pi == 0.0:             # <<<<<<<<<<<<<<
  *                 sum_Pi = EPSILON_DBL
  *             sum_disti_Pi = 0.0
  */
       }
 
-      /* "_utils.pyx":90
+      /* "evomap/mapping/evomap/_utils.pyx":90
  *             if sum_Pi == 0.0:
  *                 sum_Pi = EPSILON_DBL
  *             sum_disti_Pi = 0.0             # <<<<<<<<<<<<<<
  * 
  *             for j in range(n_neighbors):
  */
+      __Pyx_TraceLine(90,0,__PYX_ERR(0, 90, __pyx_L1_error))
       __pyx_v_sum_disti_Pi = 0.0;
 
-      /* "_utils.pyx":92
+      /* "evomap/mapping/evomap/_utils.pyx":92
  *             sum_disti_Pi = 0.0
  * 
  *             for j in range(n_neighbors):             # <<<<<<<<<<<<<<
  *                 P[i, j] /= sum_Pi
  *                 sum_disti_Pi += sqdistances[i, j] * P[i, j]
  */
+      __Pyx_TraceLine(92,0,__PYX_ERR(0, 92, __pyx_L1_error))
       __pyx_t_13 = __pyx_v_n_neighbors;
       __pyx_t_14 = __pyx_t_13;
       for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
         __pyx_v_j = __pyx_t_15;
 
-        /* "_utils.pyx":93
+        /* "evomap/mapping/evomap/_utils.pyx":93
  * 
  *             for j in range(n_neighbors):
  *                 P[i, j] /= sum_Pi             # <<<<<<<<<<<<<<
  *                 sum_disti_Pi += sqdistances[i, j] * P[i, j]
  * 
  */
+        __Pyx_TraceLine(93,0,__PYX_ERR(0, 93, __pyx_L1_error))
         __pyx_t_18 = __pyx_v_i;
         __pyx_t_19 = __pyx_v_j;
         __pyx_t_20 = -1;
         if (__pyx_t_18 < 0) {
           __pyx_t_18 += __pyx_pybuffernd_P.diminfo[0].shape;
           if (unlikely(__pyx_t_18 < 0)) __pyx_t_20 = 0;
         } else if (unlikely(__pyx_t_18 >= __pyx_pybuffernd_P.diminfo[0].shape)) __pyx_t_20 = 0;
@@ -2369,21 +2634,22 @@
         } else if (unlikely(__pyx_t_19 >= __pyx_pybuffernd_P.diminfo[1].shape)) __pyx_t_20 = 1;
         if (unlikely(__pyx_t_20 != -1)) {
           __Pyx_RaiseBufferIndexError(__pyx_t_20);
           __PYX_ERR(0, 93, __pyx_L1_error)
         }
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_P.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_P.diminfo[0].strides, __pyx_t_19, __pyx_pybuffernd_P.diminfo[1].strides) /= __pyx_v_sum_Pi;
 
-        /* "_utils.pyx":94
+        /* "evomap/mapping/evomap/_utils.pyx":94
  *             for j in range(n_neighbors):
  *                 P[i, j] /= sum_Pi
  *                 sum_disti_Pi += sqdistances[i, j] * P[i, j]             # <<<<<<<<<<<<<<
  * 
  *             entropy = math.log(sum_Pi) + beta * sum_disti_Pi
  */
+        __Pyx_TraceLine(94,0,__PYX_ERR(0, 94, __pyx_L1_error))
         __pyx_t_19 = __pyx_v_i;
         __pyx_t_18 = __pyx_v_j;
         __pyx_t_20 = -1;
         if (__pyx_t_19 < 0) {
           __pyx_t_19 += __pyx_pybuffernd_sqdistances.diminfo[0].shape;
           if (unlikely(__pyx_t_19 < 0)) __pyx_t_20 = 0;
         } else if (unlikely(__pyx_t_19 >= __pyx_pybuffernd_sqdistances.diminfo[0].shape)) __pyx_t_20 = 0;
@@ -2409,201 +2675,216 @@
         if (unlikely(__pyx_t_20 != -1)) {
           __Pyx_RaiseBufferIndexError(__pyx_t_20);
           __PYX_ERR(0, 94, __pyx_L1_error)
         }
         __pyx_v_sum_disti_Pi = (__pyx_v_sum_disti_Pi + ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float32_t *, __pyx_pybuffernd_sqdistances.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_sqdistances.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_sqdistances.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_P.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_P.diminfo[0].strides, __pyx_t_21, __pyx_pybuffernd_P.diminfo[1].strides))));
       }
 
-      /* "_utils.pyx":96
+      /* "evomap/mapping/evomap/_utils.pyx":96
  *                 sum_disti_Pi += sqdistances[i, j] * P[i, j]
  * 
  *             entropy = math.log(sum_Pi) + beta * sum_disti_Pi             # <<<<<<<<<<<<<<
  *             entropy_diff = entropy - desired_entropy
  * 
  */
+      __Pyx_TraceLine(96,0,__PYX_ERR(0, 96, __pyx_L1_error))
       __pyx_v_entropy = (log(__pyx_v_sum_Pi) + (__pyx_v_beta * __pyx_v_sum_disti_Pi));
 
-      /* "_utils.pyx":97
+      /* "evomap/mapping/evomap/_utils.pyx":97
  * 
  *             entropy = math.log(sum_Pi) + beta * sum_disti_Pi
  *             entropy_diff = entropy - desired_entropy             # <<<<<<<<<<<<<<
  * 
  *             if math.fabs(entropy_diff) <= PERPLEXITY_TOLERANCE:
  */
+      __Pyx_TraceLine(97,0,__PYX_ERR(0, 97, __pyx_L1_error))
       __pyx_v_entropy_diff = (__pyx_v_entropy - __pyx_v_desired_entropy);
 
-      /* "_utils.pyx":99
+      /* "evomap/mapping/evomap/_utils.pyx":99
  *             entropy_diff = entropy - desired_entropy
  * 
  *             if math.fabs(entropy_diff) <= PERPLEXITY_TOLERANCE:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
-      __pyx_t_16 = ((fabs(__pyx_v_entropy_diff) <= __pyx_v_6_utils_PERPLEXITY_TOLERANCE) != 0);
+      __Pyx_TraceLine(99,0,__PYX_ERR(0, 99, __pyx_L1_error))
+      __pyx_t_16 = ((fabs(__pyx_v_entropy_diff) <= __pyx_v_6evomap_7mapping_6evomap_6_utils_PERPLEXITY_TOLERANCE) != 0);
       if (__pyx_t_16) {
 
-        /* "_utils.pyx":100
+        /* "evomap/mapping/evomap/_utils.pyx":100
  * 
  *             if math.fabs(entropy_diff) <= PERPLEXITY_TOLERANCE:
  *                 break             # <<<<<<<<<<<<<<
  * 
  *             if entropy_diff > 0.0:
  */
+        __Pyx_TraceLine(100,0,__PYX_ERR(0, 100, __pyx_L1_error))
         goto __pyx_L6_break;
 
-        /* "_utils.pyx":99
+        /* "evomap/mapping/evomap/_utils.pyx":99
  *             entropy_diff = entropy - desired_entropy
  * 
  *             if math.fabs(entropy_diff) <= PERPLEXITY_TOLERANCE:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
       }
 
-      /* "_utils.pyx":102
+      /* "evomap/mapping/evomap/_utils.pyx":102
  *                 break
  * 
  *             if entropy_diff > 0.0:             # <<<<<<<<<<<<<<
  *                 beta_min = beta
  *                 if beta_max == NPY_INFINITY:
  */
+      __Pyx_TraceLine(102,0,__PYX_ERR(0, 102, __pyx_L1_error))
       __pyx_t_16 = ((__pyx_v_entropy_diff > 0.0) != 0);
       if (__pyx_t_16) {
 
-        /* "_utils.pyx":103
+        /* "evomap/mapping/evomap/_utils.pyx":103
  * 
  *             if entropy_diff > 0.0:
  *                 beta_min = beta             # <<<<<<<<<<<<<<
  *                 if beta_max == NPY_INFINITY:
  *                     beta *= 2.0
  */
+        __Pyx_TraceLine(103,0,__PYX_ERR(0, 103, __pyx_L1_error))
         __pyx_v_beta_min = __pyx_v_beta;
 
-        /* "_utils.pyx":104
+        /* "evomap/mapping/evomap/_utils.pyx":104
  *             if entropy_diff > 0.0:
  *                 beta_min = beta
  *                 if beta_max == NPY_INFINITY:             # <<<<<<<<<<<<<<
  *                     beta *= 2.0
  *                 else:
  */
+        __Pyx_TraceLine(104,0,__PYX_ERR(0, 104, __pyx_L1_error))
         __pyx_t_16 = ((__pyx_v_beta_max == NPY_INFINITY) != 0);
         if (__pyx_t_16) {
 
-          /* "_utils.pyx":105
+          /* "evomap/mapping/evomap/_utils.pyx":105
  *                 beta_min = beta
  *                 if beta_max == NPY_INFINITY:
  *                     beta *= 2.0             # <<<<<<<<<<<<<<
  *                 else:
  *                     beta = (beta + beta_max) / 2.0
  */
+          __Pyx_TraceLine(105,0,__PYX_ERR(0, 105, __pyx_L1_error))
           __pyx_v_beta = (__pyx_v_beta * 2.0);
 
-          /* "_utils.pyx":104
+          /* "evomap/mapping/evomap/_utils.pyx":104
  *             if entropy_diff > 0.0:
  *                 beta_min = beta
  *                 if beta_max == NPY_INFINITY:             # <<<<<<<<<<<<<<
  *                     beta *= 2.0
  *                 else:
  */
           goto __pyx_L17;
         }
 
-        /* "_utils.pyx":107
+        /* "evomap/mapping/evomap/_utils.pyx":107
  *                     beta *= 2.0
  *                 else:
  *                     beta = (beta + beta_max) / 2.0             # <<<<<<<<<<<<<<
  *             else:
  *                 beta_max = beta
  */
+        __Pyx_TraceLine(107,0,__PYX_ERR(0, 107, __pyx_L1_error))
         /*else*/ {
           __pyx_v_beta = ((__pyx_v_beta + __pyx_v_beta_max) / 2.0);
         }
         __pyx_L17:;
 
-        /* "_utils.pyx":102
+        /* "evomap/mapping/evomap/_utils.pyx":102
  *                 break
  * 
  *             if entropy_diff > 0.0:             # <<<<<<<<<<<<<<
  *                 beta_min = beta
  *                 if beta_max == NPY_INFINITY:
  */
         goto __pyx_L16;
       }
 
-      /* "_utils.pyx":109
+      /* "evomap/mapping/evomap/_utils.pyx":109
  *                     beta = (beta + beta_max) / 2.0
  *             else:
  *                 beta_max = beta             # <<<<<<<<<<<<<<
  *                 if beta_min == -NPY_INFINITY:
  *                     beta /= 2.0
  */
+      __Pyx_TraceLine(109,0,__PYX_ERR(0, 109, __pyx_L1_error))
       /*else*/ {
         __pyx_v_beta_max = __pyx_v_beta;
 
-        /* "_utils.pyx":110
+        /* "evomap/mapping/evomap/_utils.pyx":110
  *             else:
  *                 beta_max = beta
  *                 if beta_min == -NPY_INFINITY:             # <<<<<<<<<<<<<<
  *                     beta /= 2.0
  *                 else:
  */
+        __Pyx_TraceLine(110,0,__PYX_ERR(0, 110, __pyx_L1_error))
         __pyx_t_16 = ((__pyx_v_beta_min == (-NPY_INFINITY)) != 0);
         if (__pyx_t_16) {
 
-          /* "_utils.pyx":111
+          /* "evomap/mapping/evomap/_utils.pyx":111
  *                 beta_max = beta
  *                 if beta_min == -NPY_INFINITY:
  *                     beta /= 2.0             # <<<<<<<<<<<<<<
  *                 else:
  *                     beta = (beta + beta_min) / 2.0
  */
+          __Pyx_TraceLine(111,0,__PYX_ERR(0, 111, __pyx_L1_error))
           __pyx_v_beta = (__pyx_v_beta / 2.0);
 
-          /* "_utils.pyx":110
+          /* "evomap/mapping/evomap/_utils.pyx":110
  *             else:
  *                 beta_max = beta
  *                 if beta_min == -NPY_INFINITY:             # <<<<<<<<<<<<<<
  *                     beta /= 2.0
  *                 else:
  */
           goto __pyx_L18;
         }
 
-        /* "_utils.pyx":113
+        /* "evomap/mapping/evomap/_utils.pyx":113
  *                     beta /= 2.0
  *                 else:
  *                     beta = (beta + beta_min) / 2.0             # <<<<<<<<<<<<<<
  * 
  *         beta_sum += beta
  */
+        __Pyx_TraceLine(113,0,__PYX_ERR(0, 113, __pyx_L1_error))
         /*else*/ {
           __pyx_v_beta = ((__pyx_v_beta + __pyx_v_beta_min) / 2.0);
         }
         __pyx_L18:;
       }
       __pyx_L16:;
     }
     __pyx_L6_break:;
 
-    /* "_utils.pyx":115
+    /* "evomap/mapping/evomap/_utils.pyx":115
  *                     beta = (beta + beta_min) / 2.0
  * 
  *         beta_sum += beta             # <<<<<<<<<<<<<<
  * 
  *         if verbose and ((i + 1) % 1000 == 0 or i + 1 == n_samples):
  */
+    __Pyx_TraceLine(115,0,__PYX_ERR(0, 115, __pyx_L1_error))
     __pyx_v_beta_sum = (__pyx_v_beta_sum + __pyx_v_beta);
 
-    /* "_utils.pyx":117
+    /* "evomap/mapping/evomap/_utils.pyx":117
  *         beta_sum += beta
  * 
  *         if verbose and ((i + 1) % 1000 == 0 or i + 1 == n_samples):             # <<<<<<<<<<<<<<
  *             print("[t-SNE] Computed conditional probabilities for sample "
  *                   "%d / %d" % (i + 1, n_samples))
  */
+    __Pyx_TraceLine(117,0,__PYX_ERR(0, 117, __pyx_L1_error))
     __pyx_t_17 = (__pyx_v_verbose != 0);
     if (__pyx_t_17) {
     } else {
       __pyx_t_16 = __pyx_t_17;
       goto __pyx_L20_bool_binop_done;
     }
     __pyx_t_17 = ((__Pyx_mod_long((__pyx_v_i + 1), 0x3E8) == 0) != 0);
@@ -2613,37 +2894,39 @@
       goto __pyx_L20_bool_binop_done;
     }
     __pyx_t_17 = (((__pyx_v_i + 1) == __pyx_v_n_samples) != 0);
     __pyx_t_16 = __pyx_t_17;
     __pyx_L20_bool_binop_done:;
     if (__pyx_t_16) {
 
-      /* "_utils.pyx":118
+      /* "evomap/mapping/evomap/_utils.pyx":118
  * 
  *         if verbose and ((i + 1) % 1000 == 0 or i + 1 == n_samples):
  *             print("[t-SNE] Computed conditional probabilities for sample "             # <<<<<<<<<<<<<<
  *                   "%d / %d" % (i + 1, n_samples))
  * 
  */
+      __Pyx_TraceLine(118,0,__PYX_ERR(0, 118, __pyx_L1_error))
       __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 118, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_23 = 0;
       __pyx_t_24 = 127;
       __Pyx_INCREF(__pyx_kp_u_t_SNE_Computed_conditional_prob);
       __pyx_t_23 += 54;
       __Pyx_GIVEREF(__pyx_kp_u_t_SNE_Computed_conditional_prob);
       PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_kp_u_t_SNE_Computed_conditional_prob);
 
-      /* "_utils.pyx":119
+      /* "evomap/mapping/evomap/_utils.pyx":119
  *         if verbose and ((i + 1) % 1000 == 0 or i + 1 == n_samples):
  *             print("[t-SNE] Computed conditional probabilities for sample "
  *                   "%d / %d" % (i + 1, n_samples))             # <<<<<<<<<<<<<<
  * 
  *     if verbose:
  */
+      __Pyx_TraceLine(119,0,__PYX_ERR(0, 119, __pyx_L1_error))
       __pyx_t_4 = __Pyx_PyUnicode_From_long((__pyx_v_i + 1), 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_23 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
       __pyx_t_4 = 0;
       __Pyx_INCREF(__pyx_kp_u_);
@@ -2653,55 +2936,58 @@
       __pyx_t_4 = __Pyx_PyUnicode_From_long(__pyx_v_n_samples, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_23 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 3, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "_utils.pyx":118
+      /* "evomap/mapping/evomap/_utils.pyx":118
  * 
  *         if verbose and ((i + 1) % 1000 == 0 or i + 1 == n_samples):
  *             print("[t-SNE] Computed conditional probabilities for sample "             # <<<<<<<<<<<<<<
  *                   "%d / %d" % (i + 1, n_samples))
  * 
  */
+      __Pyx_TraceLine(118,0,__PYX_ERR(0, 118, __pyx_L1_error))
       __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_5, 4, __pyx_t_23, __pyx_t_24); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 118, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "_utils.pyx":117
+      /* "evomap/mapping/evomap/_utils.pyx":117
  *         beta_sum += beta
  * 
  *         if verbose and ((i + 1) % 1000 == 0 or i + 1 == n_samples):             # <<<<<<<<<<<<<<
  *             print("[t-SNE] Computed conditional probabilities for sample "
  *                   "%d / %d" % (i + 1, n_samples))
  */
     }
   }
 
-  /* "_utils.pyx":121
+  /* "evomap/mapping/evomap/_utils.pyx":121
  *                   "%d / %d" % (i + 1, n_samples))
  * 
  *     if verbose:             # <<<<<<<<<<<<<<
  *         print("[t-SNE] Mean sigma: %f"
  *               % np.mean(math.sqrt(n_samples / beta_sum)))
  */
+  __Pyx_TraceLine(121,0,__PYX_ERR(0, 121, __pyx_L1_error))
   __pyx_t_16 = (__pyx_v_verbose != 0);
   if (__pyx_t_16) {
 
-    /* "_utils.pyx":123
+    /* "evomap/mapping/evomap/_utils.pyx":123
  *     if verbose:
  *         print("[t-SNE] Mean sigma: %f"
  *               % np.mean(math.sqrt(n_samples / beta_sum)))             # <<<<<<<<<<<<<<
  *     return P
  */
+    __Pyx_TraceLine(123,0,__PYX_ERR(0, 123, __pyx_L1_error))
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_mean); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(__pyx_v_beta_sum == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
@@ -2725,46 +3011,48 @@
     if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_t_SNE_Mean_sigma_f, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "_utils.pyx":122
+    /* "evomap/mapping/evomap/_utils.pyx":122
  * 
  *     if verbose:
  *         print("[t-SNE] Mean sigma: %f"             # <<<<<<<<<<<<<<
  *               % np.mean(math.sqrt(n_samples / beta_sum)))
  *     return P
  */
+    __Pyx_TraceLine(122,0,__PYX_ERR(0, 122, __pyx_L1_error))
     __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "_utils.pyx":121
+    /* "evomap/mapping/evomap/_utils.pyx":121
  *                   "%d / %d" % (i + 1, n_samples))
  * 
  *     if verbose:             # <<<<<<<<<<<<<<
  *         print("[t-SNE] Mean sigma: %f"
  *               % np.mean(math.sqrt(n_samples / beta_sum)))
  */
   }
 
-  /* "_utils.pyx":124
+  /* "evomap/mapping/evomap/_utils.pyx":124
  *         print("[t-SNE] Mean sigma: %f"
  *               % np.mean(math.sqrt(n_samples / beta_sum)))
  *     return P             # <<<<<<<<<<<<<<
  */
+  __Pyx_TraceLine(124,0,__PYX_ERR(0, 124, __pyx_L1_error))
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_P));
   __pyx_r = ((PyArrayObject *)__pyx_v_P);
   goto __pyx_L0;
 
-  /* "_utils.pyx":23
+  /* "evomap/mapping/evomap/_utils.pyx":23
  * cdef float PERPLEXITY_TOLERANCE = 1e-5
  * 
  * cpdef np.ndarray[np.float32_t, ndim=2] _binary_search_perplexity(             # <<<<<<<<<<<<<<
  *         np.ndarray[np.float32_t, ndim=2] sqdistances,
  *         float desired_perplexity,
  */
 
@@ -2778,31 +3066,32 @@
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_P.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_sqdistances.rcbuffer->pybuffer);
   __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
-  __Pyx_AddTraceback("_utils._binary_search_perplexity", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("evomap.mapping.evomap._utils._binary_search_perplexity", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   goto __pyx_L2;
   __pyx_L0:;
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_P.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_sqdistances.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_P);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6_utils_1_binary_search_perplexity(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6_utils__binary_search_perplexity[] = "Binary search for sigmas of conditional Gaussians.\n    This approximation reduces the computational complexity from O(N^2) to\n    O(uN).\n    Parameters\n    ----------\n    sqdistances : array-like, shape (n_samples, n_neighbors)\n        Distances between training samples and their k nearest neighbors.\n        When using the exact method, this is a square (n_samples, n_samples)\n        distance matrix. The TSNE default metric is \"euclidean\" which is\n        interpreted as squared euclidean distance.\n    desired_perplexity : float\n        Desired perplexity (2^entropy) of the conditional Gaussians.\n    verbose : int\n        Verbosity level.\n    Returns\n    -------\n    P : array, shape (n_samples, n_samples)\n        Probabilities of conditional Gaussian distributions p_i|j.\n    ";
-static PyObject *__pyx_pw_6_utils_1_binary_search_perplexity(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6evomap_7mapping_6evomap_6_utils_1_binary_search_perplexity(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6evomap_7mapping_6evomap_6_utils__binary_search_perplexity[] = "Binary search for sigmas of conditional Gaussians.\n    This approximation reduces the computational complexity from O(N^2) to\n    O(uN).\n    Parameters\n    ----------\n    sqdistances : array-like, shape (n_samples, n_neighbors)\n        Distances between training samples and their k nearest neighbors.\n        When using the exact method, this is a square (n_samples, n_samples)\n        distance matrix. The TSNE default metric is \"euclidean\" which is\n        interpreted as squared euclidean distance.\n    desired_perplexity : float\n        Desired perplexity (2^entropy) of the conditional Gaussians.\n    verbose : int\n        Verbosity level.\n    Returns\n    -------\n    P : array, shape (n_samples, n_samples)\n        Probabilities of conditional Gaussian distributions p_i|j.\n    ";
+static PyObject *__pyx_pw_6evomap_7mapping_6evomap_6_utils_1_binary_search_perplexity(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_sqdistances = 0;
   float __pyx_v_desired_perplexity;
   int __pyx_v_verbose;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -2856,633 +3145,699 @@
     __pyx_v_desired_perplexity = __pyx_PyFloat_AsFloat(values[1]); if (unlikely((__pyx_v_desired_perplexity == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 25, __pyx_L3_error)
     __pyx_v_verbose = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_verbose == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_binary_search_perplexity", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 23, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("_utils._binary_search_perplexity", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("evomap.mapping.evomap._utils._binary_search_perplexity", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sqdistances), __pyx_ptype_5numpy_ndarray, 1, "sqdistances", 0))) __PYX_ERR(0, 24, __pyx_L1_error)
-  __pyx_r = __pyx_pf_6_utils__binary_search_perplexity(__pyx_self, __pyx_v_sqdistances, __pyx_v_desired_perplexity, __pyx_v_verbose);
+  __pyx_r = __pyx_pf_6evomap_7mapping_6evomap_6_utils__binary_search_perplexity(__pyx_self, __pyx_v_sqdistances, __pyx_v_desired_perplexity, __pyx_v_verbose);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6_utils__binary_search_perplexity(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_sqdistances, float __pyx_v_desired_perplexity, int __pyx_v_verbose) {
+static PyObject *__pyx_pf_6evomap_7mapping_6evomap_6_utils__binary_search_perplexity(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_sqdistances, float __pyx_v_desired_perplexity, int __pyx_v_verbose) {
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sqdistances;
   __Pyx_Buffer __pyx_pybuffer_sqdistances;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_binary_search_perplexity", 0);
+  __Pyx_TraceCall("_binary_search_perplexity (wrapper)", __pyx_f[0], 23, 0, __PYX_ERR(0, 23, __pyx_L1_error));
   __pyx_pybuffer_sqdistances.pybuffer.buf = NULL;
   __pyx_pybuffer_sqdistances.refcount = 0;
   __pyx_pybuffernd_sqdistances.data = NULL;
   __pyx_pybuffernd_sqdistances.rcbuffer = &__pyx_pybuffer_sqdistances;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_sqdistances.rcbuffer->pybuffer, (PyObject*)__pyx_v_sqdistances, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float32_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 23, __pyx_L1_error)
   }
   __pyx_pybuffernd_sqdistances.diminfo[0].strides = __pyx_pybuffernd_sqdistances.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_sqdistances.diminfo[0].shape = __pyx_pybuffernd_sqdistances.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_sqdistances.diminfo[1].strides = __pyx_pybuffernd_sqdistances.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_sqdistances.diminfo[1].shape = __pyx_pybuffernd_sqdistances.rcbuffer->pybuffer.shape[1];
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_6_utils__binary_search_perplexity(__pyx_v_sqdistances, __pyx_v_desired_perplexity, __pyx_v_verbose, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_6evomap_7mapping_6evomap_6_utils__binary_search_perplexity(__pyx_v_sqdistances, __pyx_v_desired_perplexity, __pyx_v_verbose, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_sqdistances.rcbuffer->pybuffer);
   __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
-  __Pyx_AddTraceback("_utils._binary_search_perplexity", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("evomap.mapping.evomap._utils._binary_search_perplexity", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   goto __pyx_L2;
   __pyx_L0:;
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_sqdistances.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":735
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
+  __Pyx_TraceCall("PyArray_MultiIterNew1", __pyx_f[1], 735, 0, __PYX_ERR(1, 735, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
+  __Pyx_TraceLine(736,0,__PYX_ERR(1, 736, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("numpy.PyArray_MultiIterNew1", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":738
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
+  __Pyx_TraceCall("PyArray_MultiIterNew2", __pyx_f[1], 738, 0, __PYX_ERR(1, 738, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
+  __Pyx_TraceLine(739,0,__PYX_ERR(1, 739, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("numpy.PyArray_MultiIterNew2", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":741
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
+  __Pyx_TraceCall("PyArray_MultiIterNew3", __pyx_f[1], 741, 0, __PYX_ERR(1, 741, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
+  __Pyx_TraceLine(742,0,__PYX_ERR(1, 742, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("numpy.PyArray_MultiIterNew3", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":744
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
+  __Pyx_TraceCall("PyArray_MultiIterNew4", __pyx_f[1], 744, 0, __PYX_ERR(1, 744, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
+  __Pyx_TraceLine(745,0,__PYX_ERR(1, 745, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("numpy.PyArray_MultiIterNew4", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":747
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
+  __Pyx_TraceCall("PyArray_MultiIterNew5", __pyx_f[1], 747, 0, __PYX_ERR(1, 747, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
+  __Pyx_TraceLine(748,0,__PYX_ERR(1, 748, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("numpy.PyArray_MultiIterNew5", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":750
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
+  __Pyx_TraceCall("PyDataType_SHAPE", __pyx_f[1], 750, 0, __PYX_ERR(1, 750, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
+  __Pyx_TraceLine(751,0,__PYX_ERR(1, 751, __pyx_L1_error))
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
+    __Pyx_TraceLine(752,0,__PYX_ERR(1, 752, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
+  __Pyx_TraceLine(754,0,__PYX_ERR(1, 754, __pyx_L1_error))
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.PyDataType_SHAPE", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":929
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
+  __Pyx_TraceCall("set_array_base", __pyx_f[1], 929, 0, __PYX_ERR(1, 929, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
+  __Pyx_TraceLine(930,0,__PYX_ERR(1, 930, __pyx_L1_error))
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
+  __Pyx_TraceLine(931,0,__PYX_ERR(1, 931, __pyx_L1_error))
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":933
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_array_base", 0);
+  __Pyx_TraceCall("get_array_base", __pyx_f[1], 933, 0, __PYX_ERR(1, 933, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
+  __Pyx_TraceLine(934,0,__PYX_ERR(1, 934, __pyx_L1_error))
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
+  __Pyx_TraceLine(935,0,__PYX_ERR(1, 935, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
+    __Pyx_TraceLine(936,0,__PYX_ERR(1, 936, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
+  __Pyx_TraceLine(937,0,__PYX_ERR(1, 937, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.get_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":941
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
   int __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
+  __Pyx_TraceCall("import_array", __pyx_f[1], 941, 0, __PYX_ERR(1, 941, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
+  __Pyx_TraceLine(942,0,__PYX_ERR(1, 942, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
+      __Pyx_TraceLine(943,0,__PYX_ERR(1, 943, __pyx_L3_error))
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
+    __Pyx_TraceLine(944,0,__PYX_ERR(1, 944, __pyx_L5_except_error))
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
+      __Pyx_TraceLine(945,0,__PYX_ERR(1, 945, __pyx_L5_except_error))
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3493,128 +3848,135 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":947
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
   int __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
+  __Pyx_TraceCall("import_umath", __pyx_f[1], 947, 0, __PYX_ERR(1, 947, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
+  __Pyx_TraceLine(948,0,__PYX_ERR(1, 948, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
+      __Pyx_TraceLine(949,0,__PYX_ERR(1, 949, __pyx_L3_error))
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
+    __Pyx_TraceLine(950,0,__PYX_ERR(1, 950, __pyx_L5_except_error))
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
+      __Pyx_TraceLine(951,0,__PYX_ERR(1, 951, __pyx_L5_except_error))
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3625,128 +3987,135 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":953
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
   int __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
+  __Pyx_TraceCall("import_ufunc", __pyx_f[1], 953, 0, __PYX_ERR(1, 953, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
+  __Pyx_TraceLine(954,0,__PYX_ERR(1, 954, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
+      __Pyx_TraceLine(955,0,__PYX_ERR(1, 955, __pyx_L3_error))
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
+    __Pyx_TraceLine(956,0,__PYX_ERR(1, 956, __pyx_L5_except_error))
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
+      __Pyx_TraceLine(957,0,__PYX_ERR(1, 957, __pyx_L5_except_error))
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3757,194 +4126,245 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":967
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+  __Pyx_TraceCall("is_timedelta64_object", __pyx_f[1], 967, 0, __PYX_ERR(1, 967, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
+  __Pyx_TraceLine(979,0,__PYX_ERR(1, 979, __pyx_L1_error))
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.is_timedelta64_object", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_r = 0;
   __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":982
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+  __Pyx_TraceCall("is_datetime64_object", __pyx_f[1], 982, 0, __PYX_ERR(1, 982, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
+  __Pyx_TraceLine(994,0,__PYX_ERR(1, 994, __pyx_L1_error))
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.is_datetime64_object", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_r = 0;
   __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":997
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
+  __Pyx_TraceDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_TraceCall("get_datetime64_value", __pyx_f[1], 997, 1, __PYX_ERR(1, 997, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
+  __Pyx_TraceLine(1004,1,__PYX_ERR(1, 1004, __pyx_L1_error))
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.get_datetime64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
+  __pyx_r = 0;
   __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
+  __Pyx_TraceDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_TraceCall("get_timedelta64_value", __pyx_f[1], 1007, 1, __PYX_ERR(1, 1007, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
+  __Pyx_TraceLine(1011,1,__PYX_ERR(1, 1011, __pyx_L1_error))
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.get_timedelta64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
+  __pyx_r = 0;
   __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
+  __Pyx_TraceDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_TraceCall("get_datetime64_unit", __pyx_f[1], 1014, 1, __PYX_ERR(1, 1014, __pyx_L1_error));
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
+  __Pyx_TraceLine(1018,1,__PYX_ERR(1, 1018, __pyx_L1_error))
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.get_datetime64_unit", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
+  __pyx_r = (NPY_DATETIMEUNIT) 0;
   __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
 static PyMethodDef __pyx_methods[] = {
-  {"_binary_search_perplexity", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6_utils_1_binary_search_perplexity, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6_utils__binary_search_perplexity},
+  {"_binary_search_perplexity", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6evomap_7mapping_6evomap_6_utils_1_binary_search_perplexity, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6evomap_7mapping_6evomap_6_utils__binary_search_perplexity},
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
 static int __pyx_pymod_exec__utils(PyObject* module); /*proto*/
@@ -4020,26 +4440,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 951, __pyx_L1_error)
@@ -4265,14 +4685,15 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec__utils(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  __Pyx_TraceDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
@@ -4344,22 +4765,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main__utils) {
+  if (__pyx_module_is_main_evomap__mapping__evomap___utils) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "_utils")) {
-      if (unlikely(PyDict_SetItemString(modules, "_utils", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "evomap.mapping.evomap._utils")) {
+      if (unlikely(PyDict_SetItemString(modules, "evomap.mapping.evomap._utils", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -4371,84 +4792,253 @@
   if (unlikely(__Pyx_modinit_type_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
+  __Pyx_TraceCall("__Pyx_PyMODINIT_FUNC PyInit__utils(void)", __pyx_f[0], 1, 0, __PYX_ERR(0, 1, __pyx_L1_error));
 
-  /* "_utils.pyx":9
+  /* "evomap/mapping/evomap/_utils.pyx":9
  * from libc cimport math
  * cimport cython
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * from libc.stdio cimport printf
  */
+  __Pyx_TraceLine(9,0,__PYX_ERR(0, 9, __pyx_L1_error))
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_utils.pyx":13
+  /* "evomap/mapping/evomap/_utils.pyx":13
  * from libc.stdio cimport printf
  * 
  * np.import_array()             # <<<<<<<<<<<<<<
  * 
  * 
  */
+  __Pyx_TraceLine(13,0,__PYX_ERR(0, 13, __pyx_L1_error))
   __pyx_t_2 = __pyx_f_5numpy_import_array(); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 13, __pyx_L1_error)
 
-  /* "_utils.pyx":20
+  /* "evomap/mapping/evomap/_utils.pyx":20
  * 
  * 
  * cdef float EPSILON_DBL = 1e-8             # <<<<<<<<<<<<<<
  * cdef float PERPLEXITY_TOLERANCE = 1e-5
  * 
  */
-  __pyx_v_6_utils_EPSILON_DBL = 1e-8;
+  __Pyx_TraceLine(20,0,__PYX_ERR(0, 20, __pyx_L1_error))
+  __pyx_v_6evomap_7mapping_6evomap_6_utils_EPSILON_DBL = 1e-8;
 
-  /* "_utils.pyx":21
+  /* "evomap/mapping/evomap/_utils.pyx":21
  * 
  * cdef float EPSILON_DBL = 1e-8
  * cdef float PERPLEXITY_TOLERANCE = 1e-5             # <<<<<<<<<<<<<<
  * 
  * cpdef np.ndarray[np.float32_t, ndim=2] _binary_search_perplexity(
  */
-  __pyx_v_6_utils_PERPLEXITY_TOLERANCE = 1e-5;
+  __Pyx_TraceLine(21,0,__PYX_ERR(0, 21, __pyx_L1_error))
+  __pyx_v_6evomap_7mapping_6evomap_6_utils_PERPLEXITY_TOLERANCE = 1e-5;
+
+  /* "evomap/mapping/evomap/_utils.pyx":23
+ * cdef float PERPLEXITY_TOLERANCE = 1e-5
+ * 
+ * cpdef np.ndarray[np.float32_t, ndim=2] _binary_search_perplexity(             # <<<<<<<<<<<<<<
+ *         np.ndarray[np.float32_t, ndim=2] sqdistances,
+ *         float desired_perplexity,
+ */
+  __Pyx_TraceLine(23,0,__PYX_ERR(0, 23, __pyx_L1_error))
+
 
-  /* "_utils.pyx":1
+  /* "evomap/mapping/evomap/_utils.pyx":1
  * #define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION             # <<<<<<<<<<<<<<
  * # cython: language_level=3
  * 
  */
+  __Pyx_TraceLine(1,0,__PYX_ERR(0, 1, __pyx_L1_error))
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../../../../../../../anaconda3/envs/evomap-test/lib/python3.9/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":735
+ * ctypedef npy_cdouble     complex_t
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ */
+  __Pyx_TraceLine(735,0,__PYX_ERR(1, 735, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":738
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ */
+  __Pyx_TraceLine(738,0,__PYX_ERR(1, 738, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":741
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ */
+  __Pyx_TraceLine(741,0,__PYX_ERR(1, 741, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":744
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ */
+  __Pyx_TraceLine(744,0,__PYX_ERR(1, 744, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":747
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ */
+  __Pyx_TraceLine(747,0,__PYX_ERR(1, 747, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":750
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+  __Pyx_TraceLine(750,0,__PYX_ERR(1, 750, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":929
+ *     int _import_umath() except -1
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
+ */
+  __Pyx_TraceLine(929,0,__PYX_ERR(1, 929, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":933
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ */
+  __Pyx_TraceLine(933,0,__PYX_ERR(1, 933, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":941
+ * # Versions of the import_* functions which are more suitable for
+ * # Cython code.
+ * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         __pyx_import_array()
+ */
+  __Pyx_TraceLine(941,0,__PYX_ERR(1, 941, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":947
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+  __Pyx_TraceLine(947,0,__PYX_ERR(1, 947, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":953
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+  __Pyx_TraceLine(953,0,__PYX_ERR(1, 953, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+  __Pyx_TraceLine(967,0,__PYX_ERR(1, 967, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+  __Pyx_TraceLine(982,0,__PYX_ERR(1, 982, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+  __Pyx_TraceLine(997,0,__PYX_ERR(1, 997, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+  __Pyx_TraceLine(1007,0,__PYX_ERR(1, 1007, __pyx_L1_error))
+
+
+  /* "../../../../../../../../private/var/folders/1z/nx4x54q97jvgthsnm68bv48w0000gq/T/pip-build-env-r32tsx2d/overlay/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
+  __Pyx_TraceLine(1014,0,__PYX_ERR(1, 1014, __pyx_L1_error))
+
+  __Pyx_TraceReturn(Py_None, 0);
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init _utils", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init evomap.mapping.evomap._utils", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init _utils");
+    PyErr_SetString(PyExc_ImportError, "init evomap.mapping.evomap._utils");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -4499,14 +5089,128 @@
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+}
+#endif
+
+/* Profile */
+#if CYTHON_PROFILE
+static int __Pyx_TraceSetupAndCall(PyCodeObject** code,
+                                   PyFrameObject** frame,
+                                   PyThreadState* tstate,
+                                   const char *funcname,
+                                   const char *srcfile,
+                                   int firstlineno) {
+    PyObject *type, *value, *traceback;
+    int retval;
+    if (*frame == NULL || !CYTHON_PROFILE_REUSE_FRAME) {
+        if (*code == NULL) {
+            *code = __Pyx_createFrameCodeObject(funcname, srcfile, firstlineno);
+            if (*code == NULL) return 0;
+        }
+        *frame = PyFrame_New(
+            tstate,                          /*PyThreadState *tstate*/
+            *code,                           /*PyCodeObject *code*/
+            __pyx_d,                  /*PyObject *globals*/
+            0                                /*PyObject *locals*/
+        );
+        if (*frame == NULL) return 0;
+        if (CYTHON_TRACE && (*frame)->f_trace == NULL) {
+            Py_INCREF(Py_None);
+            (*frame)->f_trace = Py_None;
+        }
+#if PY_VERSION_HEX < 0x030400B1
+    } else {
+        (*frame)->f_tstate = tstate;
+#endif
+    }
+    __Pyx_PyFrame_SetLineNumber(*frame, firstlineno);
+    retval = 1;
+    __Pyx_EnterTracing(tstate);
+    __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
+    #if CYTHON_TRACE
+    if (tstate->c_tracefunc)
+        retval = tstate->c_tracefunc(tstate->c_traceobj, *frame, PyTrace_CALL, NULL) == 0;
+    if (retval && tstate->c_profilefunc)
+    #endif
+        retval = tstate->c_profilefunc(tstate->c_profileobj, *frame, PyTrace_CALL, NULL) == 0;
+    __Pyx_LeaveTracing(tstate);
+    if (retval) {
+        __Pyx_ErrRestoreInState(tstate, type, value, traceback);
+        return __Pyx_IsTracing(tstate, 0, 0) && retval;
+    } else {
+        Py_XDECREF(type);
+        Py_XDECREF(value);
+        Py_XDECREF(traceback);
+        return -1;
+    }
+}
+static PyCodeObject *__Pyx_createFrameCodeObject(const char *funcname, const char *srcfile, int firstlineno) {
+    PyCodeObject *py_code = 0;
+#if PY_MAJOR_VERSION >= 3
+    py_code = PyCode_NewEmpty(srcfile, funcname, firstlineno);
+    if (likely(py_code)) {
+        py_code->co_flags |= CO_OPTIMIZED | CO_NEWLOCALS;
+    }
+#else
+    PyObject *py_srcfile = 0;
+    PyObject *py_funcname = 0;
+    py_funcname = PyString_FromString(funcname);
+    if (unlikely(!py_funcname)) goto bad;
+    py_srcfile = PyString_FromString(srcfile);
+    if (unlikely(!py_srcfile)) goto bad;
+    py_code = PyCode_New(
+        0,
+        0,
+        0,
+        CO_OPTIMIZED | CO_NEWLOCALS,
+        __pyx_empty_bytes,     /*PyObject *code,*/
+        __pyx_empty_tuple,     /*PyObject *consts,*/
+        __pyx_empty_tuple,     /*PyObject *names,*/
+        __pyx_empty_tuple,     /*PyObject *varnames,*/
+        __pyx_empty_tuple,     /*PyObject *freevars,*/
+        __pyx_empty_tuple,     /*PyObject *cellvars,*/
+        py_srcfile,       /*PyObject *filename,*/
+        py_funcname,      /*PyObject *name,*/
+        firstlineno,
+        __pyx_empty_bytes      /*PyObject *lnotab*/
+    );
+bad:
+    Py_XDECREF(py_srcfile);
+    Py_XDECREF(py_funcname);
+#endif
+    return py_code;
+}
+#endif
+
 /* IsLittleEndian */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
 {
   union {
     uint32_t u32;
     uint8_t u8[4];
   } S;
@@ -5636,38 +6340,14 @@
     result = __Pyx_PyObject_Call(function, args, NULL);
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
-/* PyErrFetchRestore */
-  #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
 /* RaiseArgTupleInvalid */
   static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -5823,14 +6503,54 @@
     }
     PyErr_Format(PyExc_TypeError,
         "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
         name, type->tp_name, Py_TYPE(obj)->tp_name);
     return 0;
 }
 
+/* WriteUnraisableException */
+  static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* GetTopmostException */
   #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
```

### Comparing `evomap-0.3.0/src/evomap/mapping/evomap/_utils.pyx` & `evomap-0.3.1/src/evomap/mapping/evomap/_utils.pyx`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/metrics.py` & `evomap-0.3.1/src/evomap/metrics.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/preprocessing.py` & `evomap-0.3.1/src/evomap/preprocessing.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/src/evomap/printer.py` & `evomap-0.3.1/src/evomap/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,22 +403,22 @@
         scatter_args.update(scatter_kws)
 
         # Only plot points for the last period if show_last_positions_only is True
         if not show_last_positions_only or t == n_periods - 1:
             ax.scatter(X_t[t][valid_indices, 0], X_t[t][valid_indices, 1], alpha=transparency, s=sizes[valid_indices], 
                     c=colors[valid_indices], **scatter_args)
 
-            if show_arrows and t > 0:
-                for i in range(n_samples):
-                    if incl_t[t][i] and incl_t[t-1][i]:
-                        start_point = X_t[t-1][i]
-                        end_point = X_t[t][i]
-                        if not np.array_equal(start_point, end_point):
-                            ax.plot([start_point[0], end_point[0]], [start_point[1], end_point[1]],
-                                    color='gray', alpha=transparency_start, linewidth=1)
+        if show_arrows and t > 0:
+            for i in range(n_samples):
+                if incl_t[t][i] and incl_t[t-1][i]:
+                    start_point = X_t[t-1][i]
+                    end_point = X_t[t][i]
+                    if not np.array_equal(start_point, end_point):
+                        ax.plot([start_point[0], end_point[0]], [start_point[1], end_point[1]],
+                                color='gray', alpha=transparency, linewidth=1)
 
             if label is not None and t == n_periods - 1:  # Check explicitly if label is not None
                 for i, txt in enumerate(label):
                     if valid_indices[i]:
                         ax.text(X_t[t][i, 0], X_t[t][i, 1], txt, fontsize=DEFAULT_FONT_SIZE)
 
     style_axes(ax, show_axes, show_box, show_grid, axes_at_origin)
@@ -442,17 +442,17 @@
                alpha=transparency, s=sizes if sizes is not None else DEFAULT_BUBBLE_SIZE,
                color=colors[valid_indices])
     if period == n_periods - 1 and labels is not None:
         for i, txt in enumerate(labels):
             if valid_indices[i]:
                 ax.text(X[i, 0], X[i, 1], txt, fontsize=DEFAULT_FONT_SIZE)
 
-def draw_trajectories(Y_ts, labels, selected_labels = None, title = None, 
+def draw_trajectories(Y_ts, labels, selected_labels = None, 
     show_axes = False, show_box = True, show_grid = False, axes_at_origin = False,
-    annotate_periods = True, period_labels = None, ax = None, fig_size = None):
+    annotate_periods = True, period_labels = None, fig_size = None, **kwargs):
     """ Draw the trajectories of selected objects.
 
     Parameters
     ----------
     Y_ts : list of ndarrays, each of shape (n_samples, d)
         Sequence of map coordinates.
     labels : ndarray of shape (n_samples,)
@@ -473,22 +473,21 @@
     """
 
     n_periods = len(Y_ts)
     n_firms = Y_ts[0].shape[0]
     if selected_labels == None:
         selected_labels = labels
 
-    # If not ax is provided, return the whole FIgure. Else, only draw the plot on the provided axes
+    ax = kwargs.get('ax')
     if ax is None:
+        fig, ax = plt.subplots(figsize=kwargs.get('fig_size', (6,6)))
         return_fig = True
-        if fig_size is None:
-            fig_size = (7,7)
-        fig, ax = plt.subplots(figsize = fig_size)
     else:
-        return_fig = False  
+        fig = ax.figure
+        return_fig = False
 
     annotations = []
 
     if period_labels is None and annotate_periods == True:
         period_labels = ["Period " + str(t+1) for t in range(n_periods)]
 
     for i in range(n_firms):
@@ -519,17 +518,14 @@
         # Plot the trajectory
         ax.xaxis.set_ticklabels([])
         ax.yaxis.set_ticklabels([])
         ax.plot(xs, ys, c = c_line, alpha = .4)
 
     style_axes(ax = ax, show_axes= show_axes, show_box = show_box, show_grid = show_grid, axes_at_origin = axes_at_origin)
 
-    if not title is None:
-        ax.set_title(title, fontdict = title_fontdict)
-
     if not return_fig:
         plt.close(fig)
 
 def fit_attribute(coords, attribute_label, attribute_values, ax, coord_range):
     """Fit an attribute to the map and display the resultant vector."""
     # Store the current limits to restore them later
     x_lim = ax.get_xlim()
```

### Comparing `evomap-0.3.0/src/evomap/transform.py` & `evomap-0.3.1/src/evomap/transform.py`

 * *Files identical despite different names*

### Comparing `evomap-0.3.0/setup.py` & `evomap-0.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
  'setuptools==68.2.0',
  'sphinx-book-theme==1.1.2',
  'sphinx==7.3.7',
  'statsmodels==0.13.2']
 
 setup_kwargs = {
     'name': 'evomap',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'A Python Toolbox for Mapping Evolving Relationship Data',
-    'long_description': "# evomap - A Toolbox for Dynamic Mapping in Python\n\n`evomap` offers a comprehensive toolbox to create, explore and analyze spatial representations ('maps') from relationship data. Common applications include Marketing (market structure analysis), Network Analysis (e.g., social, economic, or biological networks), Political Science, or High-Dimensional Data Analysis in general. \n\nOften, relationship data is retrievable over time, as markets and networks tend to evolve. `evomap` provides all necessary tools to analyze such data in maps either in static snapshots at a single point in time, or in evolving maps across multiple periods. `evomap` provides an all-in-one solution and integrates many steps of the analysis into an easy-to-use API. Specifically, `evomap` includes modules for \n\n- preprocessing\n- mapping (static/dynamic)\n- evaluation\n- plotting\n\nNote: As of now, `evomap` is available as a ***pre-release version*** and parts of `evomap` are still under active development. For any bug reports or feature requests, <a href = 'mailto:mpmatthe@iu.edu'>please get in touch</a>.\n\n## Installation\n\nThis pre-release is available via GitHub. Stay tuned for a release on PyPi, which is coming soon! \n\nTo install `evomap` run\n```bash\npip install git+https://github.com/mpmatthe/evomap\n```\n\n`evomap` requires Python version 3.9. We recommend using Python within a virtual environment, for instance via conda:\n```bash\nconda create -n evomap python=3.9\nconda activate evomap\npip install git+https://github.com/mpmatthe/evomap\n```\n\n**Note:** Currently, `evomap` builds its C extensions upon installation on the system. Thus, it requires a C compiler to be present. The right C compiler depends upon your system, e.g. GCC on Linux or MSVC on Windows. For details, see <a href = 'https://cython.readthedocs.io/en/latest/src/quickstart/install.html'>the Cython documentation</a>. In future versions, extensions will be pre-compiled.\n\n## Usage\n\nThe following tutorials provide a good starting point for using `evomap`. \n\nFor a simple introduction to a typical market structure application, see <a href = 'https://evomap.readthedocs.io/en/latest/car%20application.html'>this example</a>.\n\nIf you want to dive deaper into what `evomap` has to offer, check out the following examples on\n\n1. <a href = 'https://evomap.readthedocs.io/en/latest/static%20mapping.html'>Static Mapping</a>\n2. <a href = 'https://evomap.readthedocs.io/en/latest/dynamic%20mapping.html'>Dynamic Mapping</a>\n\nUpdated versions of these examples will be available as new features are released. \n\n## Mapping Methods\n\nAs of now, `evomap` provides implementations of the following mapping methods:\n- MDS (Multidimensional Scaling)\n- Sammon Mapping (non-linear MDS)\n- t-SNE (t-distributed Stochastic Neighbor Embedding)\n\nYou can apply all methods statically and dynamically. Moreover, `evomap` follows the syntax conventions of `scikit-learn`, such that other \nmachine-learning techniques (such as LLE, Isomap, ... ) can easily be integrated. For more background, see <a href = 'https://scikit-learn.org/stable/modules/manifold.html'> here</a>.\n\n## References\n\nThis package is based on the authors' work in \n\n```\n[1] Matthe, M., Ringel, D. M., Skiera, B. (2023), Mapping Market Structure Evolution. Marketing Science, Vol. 42, Issue 3, 589-613.\n```\nRead the full paper here (open access): <a href = 'https://doi.org/10.1287/mksc.2022.1385'>https://doi.org/10.1287/mksc.2022.1385</a> \n\n<b><i>Please cite our paper if you use this package or part of its code</i></b>\n\n`evomap` also builds upon the work of others, including\n```\n[2] Ringel, D. M., & Skiera, B. (2016). Visualizing asymmetric competition among more than 1,000 products using big search data. Marketing Science, 35(3), 511-534.\n\n[3] Torgerson, W. S. (1952). Multidimensional Scaling: I. Theory and method. Psychometrika, 17(4), 401-419.\n\n[4] Van der Maaten, L., & Hinton, G. (2008). Visualizing data using t-SNE. Journal of Machine Learning Research, 9(11).\n\n[5] Sammon, J. W. (1969). A nonlinear mapping for data structure analysis. IEEE Transactions on computers, 100(5), 401-409.\n\n[6] Kruskal, J. B. (1964). Multidimensional scaling by optimizing goodness of fit to a nonmetric hypothesis. Psychometrika, 29(1), 1-27.\n```\n\nIf you use the respective methods implemented in `evomap`, consider also citing the original references.\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`evomap` is licensed under the terms of the MIT license. It is free to use, however, <i>please cite our work</i>.\n\n## Credits\n\n`evomap` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n",
+    'long_description': "# evomap - A Toolbox for Dynamic Mapping in Python\n\n`evomap` offers a comprehensive toolbox to create, explore and analyze spatial representations ('maps') from relationship data. Common applications include Marketing (market structure analysis), Network Analysis (e.g., social, economic, or biological networks), Political Science, or High-Dimensional Data Analysis in general. \n\nOften, relationship data is retrievable over time, as markets and networks tend to evolve. `evomap` provides all necessary tools to analyze such data in maps either in static snapshots at a single point in time, or in evolving maps across multiple periods. `evomap` provides an all-in-one solution and integrates many steps of the analysis into an easy-to-use API. Specifically, `evomap` includes modules for \n\n- preprocessing\n- mapping (static/dynamic)\n- evaluation\n- plotting\n\nNote: As of now, `evomap` is available as a ***pre-release version*** and parts of `evomap` are still under active development. For any bug reports or feature requests, <a href = 'mailto:mpmatthe@iu.edu'>please get in touch</a>.\n\n## Installation\n\nThis pre-release is available via PyPi. \n\nTo install `evomap` run\n```bash\npip install evomap\n```\n\n`evomap` works best with Python version 3.9. We recommend using Python within a virtual environment, for instance via conda:\n```bash\nconda create -n evomap python=3.9\nconda activate evomap\npip install evomap\n```\n\n**Note:** Currently, `evomap` builds its C extensions upon installation on the system. Thus, it requires a C compiler to be present. The right C compiler depends upon your system, e.g. GCC on Linux or MSVC on Windows. For details, see <a href = 'https://cython.readthedocs.io/en/latest/src/quickstart/install.html'>the Cython documentation</a>. In future versions, extensions will be pre-compiled.\n\n## Usage\n\nThe following tutorials provide a good starting point for using `evomap`. \n\nFor a simple introduction to a typical market structure application, see <a href = 'https://evomap.readthedocs.io/en/latest/car%20application.html'>this example</a>.\n\nIf you want to dive deaper into what `evomap` has to offer, check out the following examples on\n\n1. <a href = 'https://evomap.readthedocs.io/en/latest/static%20mapping.html'>Static Mapping</a>\n2. <a href = 'https://evomap.readthedocs.io/en/latest/dynamic%20mapping.html'>Dynamic Mapping</a>\n\nUpdated versions of these examples will be available as new features are released. \n\n## Mapping Methods\n\nAs of now, `evomap` provides implementations of the following mapping methods:\n- MDS (Multidimensional Scaling)\n- Sammon Mapping (non-linear MDS)\n- t-SNE (t-distributed Stochastic Neighbor Embedding)\n\nYou can apply all methods statically and dynamically. Moreover, `evomap` follows the syntax conventions of `scikit-learn`, such that other \nmachine-learning techniques (such as LLE, Isomap, ... ) can easily be integrated. For more background, see <a href = 'https://scikit-learn.org/stable/modules/manifold.html'> here</a>.\n\n## References\n\nThis package is based on the authors' work in \n\n```\n[1] Matthe, M., Ringel, D. M., Skiera, B. (2023), Mapping Market Structure Evolution. Marketing Science, Vol. 42, Issue 3, 589-613.\n```\nRead the full paper here (open access): <a href = 'https://doi.org/10.1287/mksc.2022.1385'>https://doi.org/10.1287/mksc.2022.1385</a> \n\n<b><i>Please cite our paper if you use this package or part of its code</i></b>\n\n`evomap` also builds upon the work of others, including\n```\n[2] Ringel, D. M., & Skiera, B. (2016). Visualizing asymmetric competition among more than 1,000 products using big search data. Marketing Science, 35(3), 511-534.\n\n[3] Torgerson, W. S. (1952). Multidimensional Scaling: I. Theory and method. Psychometrika, 17(4), 401-419.\n\n[4] Van der Maaten, L., & Hinton, G. (2008). Visualizing data using t-SNE. Journal of Machine Learning Research, 9(11).\n\n[5] Sammon, J. W. (1969). A nonlinear mapping for data structure analysis. IEEE Transactions on computers, 100(5), 401-409.\n\n[6] Kruskal, J. B. (1964). Multidimensional scaling by optimizing goodness of fit to a nonmetric hypothesis. Psychometrika, 29(1), 1-27.\n```\n\nIf you use the respective methods implemented in `evomap`, consider also citing the original references.\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`evomap` is licensed under the terms of the MIT license. It is free to use, however, <i>please cite our work</i>.\n\n## Credits\n\n`evomap` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n",
     'author': 'Maximilian Matthe',
     'author_email': 'mpmatthe@iu.edu>, Daniel M. Ringel <>, and Bernd Skiera <',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `evomap-0.3.0/PKG-INFO` & `evomap-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evomap
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python Toolbox for Mapping Evolving Relationship Data
 License: MIT
 Author: Maximilian Matthe
 Author-email: mpmatthe@iu.edu>, Daniel M. Ringel <>, and Bernd Skiera <
 Requires-Python: >=3.9.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -36,26 +36,26 @@
 - evaluation
 - plotting
 
 Note: As of now, `evomap` is available as a ***pre-release version*** and parts of `evomap` are still under active development. For any bug reports or feature requests, <a href = 'mailto:mpmatthe@iu.edu'>please get in touch</a>.
 
 ## Installation
 
-This pre-release is available via GitHub. Stay tuned for a release on PyPi, which is coming soon! 
+This pre-release is available via PyPi. 
 
 To install `evomap` run
 ```bash
-pip install git+https://github.com/mpmatthe/evomap
+pip install evomap
 ```
 
-`evomap` requires Python version 3.9. We recommend using Python within a virtual environment, for instance via conda:
+`evomap` works best with Python version 3.9. We recommend using Python within a virtual environment, for instance via conda:
 ```bash
 conda create -n evomap python=3.9
 conda activate evomap
-pip install git+https://github.com/mpmatthe/evomap
+pip install evomap
 ```
 
 **Note:** Currently, `evomap` builds its C extensions upon installation on the system. Thus, it requires a C compiler to be present. The right C compiler depends upon your system, e.g. GCC on Linux or MSVC on Windows. For details, see <a href = 'https://cython.readthedocs.io/en/latest/src/quickstart/install.html'>the Cython documentation</a>. In future versions, extensions will be pre-compiled.
 
 ## Usage
 
 The following tutorials provide a good starting point for using `evomap`.
```

