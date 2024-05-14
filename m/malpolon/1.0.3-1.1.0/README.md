# Comparing `tmp/malpolon-1.0.3.tar.gz` & `tmp/malpolon-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malpolon-1.0.3.tar", last modified: Mon Mar  4 11:04:41 2024, max compression
+gzip compressed data, was "malpolon-1.1.0.tar", last modified: Tue May 14 13:12:57 2024, max compression
```

## Comparing `malpolon-1.0.3.tar` & `malpolon-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-03-04 11:04:41.450792 malpolon-1.0.3/
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     1073 2023-09-29 15:18:12.000000 malpolon-1.0.3/LICENSE.md
--rw-r--r--   0 tlarcher  (1001) tlarcher  (1001)     2115 2024-03-04 11:04:41.450792 malpolon-1.0.3/PKG-INFO
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    12877 2024-02-29 16:36:20.000000 malpolon-1.0.3/README.md
-drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-03-04 11:04:41.450792 malpolon-1.0.3/malpolon/
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      153 2024-02-28 19:29:31.000000 malpolon-1.0.3/malpolon/__init__.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      749 2024-02-26 11:45:26.000000 malpolon-1.0.3/malpolon/check_install.py
-drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-03-04 11:04:41.450792 malpolon-1.0.3/malpolon/data/
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      472 2024-02-28 19:29:31.000000 malpolon-1.0.3/malpolon/data/__init__.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    11741 2024-02-26 11:45:26.000000 malpolon-1.0.3/malpolon/data/data_module.py
-drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-03-04 11:04:41.450792 malpolon-1.0.3/malpolon/data/datasets/
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      437 2024-02-28 19:29:31.000000 malpolon-1.0.3/malpolon/data/datasets/__init__.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)       45 2023-09-29 15:18:12.000000 malpolon-1.0.3/malpolon/data/datasets/_base.py
-drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-03-04 11:04:41.450792 malpolon-1.0.3/malpolon/data/datasets/_data/
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)        0 2023-09-29 15:18:12.000000 malpolon-1.0.3/malpolon/data/datasets/_data/__init__.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)   169004 2023-09-29 15:18:12.000000 malpolon-1.0.3/malpolon/data/datasets/_data/minigeolifeclef2022_species_details.csv
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    23522 2024-02-28 19:29:31.000000 malpolon-1.0.3/malpolon/data/datasets/geolifeclef2022.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    47290 2024-02-23 13:28:06.000000 malpolon-1.0.3/malpolon/data/datasets/geolifeclef2023.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    20712 2024-02-28 19:29:31.000000 malpolon-1.0.3/malpolon/data/datasets/torchgeo_datasets.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    14151 2024-03-01 10:36:03.000000 malpolon-1.0.3/malpolon/data/datasets/torchgeo_sentinel2.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    12758 2024-02-28 17:52:27.000000 malpolon-1.0.3/malpolon/data/environmental_raster.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     4827 2024-02-26 11:45:26.000000 malpolon-1.0.3/malpolon/data/get_jpeg_patches_stats.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     5045 2024-02-28 19:29:31.000000 malpolon-1.0.3/malpolon/data/utils.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     3559 2024-02-26 17:06:46.000000 malpolon-1.0.3/malpolon/logging.py
-drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-03-04 11:04:41.450792 malpolon-1.0.3/malpolon/models/
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      156 2023-09-29 15:18:12.000000 malpolon-1.0.3/malpolon/models/__init__.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     9202 2024-02-26 11:45:26.000000 malpolon-1.0.3/malpolon/models/model_builder.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     5418 2024-02-26 11:45:26.000000 malpolon-1.0.3/malpolon/models/multi_modal.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    10938 2024-02-26 11:45:26.000000 malpolon-1.0.3/malpolon/models/standard_prediction_systems.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     5014 2024-02-26 11:45:26.000000 malpolon-1.0.3/malpolon/models/utils.py
-drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-03-04 11:04:41.450792 malpolon-1.0.3/malpolon/plot/
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)        0 2023-09-29 15:18:12.000000 malpolon-1.0.3/malpolon/plot/__init__.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     4042 2024-02-26 11:45:26.000000 malpolon-1.0.3/malpolon/plot/history.py
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     1959 2024-02-26 11:45:26.000000 malpolon-1.0.3/malpolon/plot/map.py
-drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-03-04 11:04:41.450792 malpolon-1.0.3/malpolon.egg-info/
--rw-r--r--   0 tlarcher  (1001) tlarcher  (1001)     2115 2024-03-04 11:04:41.000000 malpolon-1.0.3/malpolon.egg-info/PKG-INFO
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      997 2024-03-04 11:04:41.000000 malpolon-1.0.3/malpolon.egg-info/SOURCES.txt
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)        1 2024-03-04 11:04:41.000000 malpolon-1.0.3/malpolon.egg-info/dependency_links.txt
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      389 2024-03-04 11:04:41.000000 malpolon-1.0.3/malpolon.egg-info/requires.txt
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)        9 2024-03-04 11:04:41.000000 malpolon-1.0.3/malpolon.egg-info/top_level.txt
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)       38 2024-03-04 11:04:41.450792 malpolon-1.0.3/setup.cfg
--rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     2362 2024-03-04 10:54:05.000000 malpolon-1.0.3/setup.py
+drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-05-14 13:12:57.013908 malpolon-1.1.0/
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     1073 2023-09-29 15:18:12.000000 malpolon-1.1.0/LICENSE.md
+-rw-r--r--   0 tlarcher  (1001) tlarcher  (1001)     2085 2024-05-14 13:12:57.013908 malpolon-1.1.0/PKG-INFO
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    13109 2024-05-14 09:58:48.000000 malpolon-1.1.0/README.md
+drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-05-14 13:12:57.013908 malpolon-1.1.0/malpolon/
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      153 2024-02-28 19:29:31.000000 malpolon-1.1.0/malpolon/__init__.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      749 2024-02-26 11:45:26.000000 malpolon-1.1.0/malpolon/check_install.py
+drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-05-14 13:12:57.013908 malpolon-1.1.0/malpolon/data/
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      472 2024-04-12 17:29:12.000000 malpolon-1.1.0/malpolon/data/__init__.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    15504 2024-05-14 09:58:48.000000 malpolon-1.1.0/malpolon/data/data_module.py
+drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-05-14 13:12:57.013908 malpolon-1.1.0/malpolon/data/datasets/
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      523 2024-05-14 09:58:48.000000 malpolon-1.1.0/malpolon/data/datasets/__init__.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)       45 2023-09-29 15:18:12.000000 malpolon-1.1.0/malpolon/data/datasets/_base.py
+drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-05-14 13:12:57.013908 malpolon-1.1.0/malpolon/data/datasets/_data/
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)        0 2023-09-29 15:18:12.000000 malpolon-1.1.0/malpolon/data/datasets/_data/__init__.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)   169004 2023-09-29 15:18:12.000000 malpolon-1.1.0/malpolon/data/datasets/_data/minigeolifeclef2022_species_details.csv
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    23588 2024-05-14 09:58:48.000000 malpolon-1.1.0/malpolon/data/datasets/geolifeclef2022.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    47290 2024-04-01 13:21:01.000000 malpolon-1.1.0/malpolon/data/datasets/geolifeclef2023.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    48002 2024-05-14 09:58:48.000000 malpolon-1.1.0/malpolon/data/datasets/geolifeclef2024.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     8275 2024-05-14 09:58:48.000000 malpolon-1.1.0/malpolon/data/datasets/torchgeo_concat.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    26380 2024-05-14 09:58:48.000000 malpolon-1.1.0/malpolon/data/datasets/torchgeo_datasets.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    13162 2024-05-14 09:58:48.000000 malpolon-1.1.0/malpolon/data/datasets/torchgeo_sentinel2.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    12758 2024-02-28 17:52:27.000000 malpolon-1.1.0/malpolon/data/environmental_raster.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     4827 2024-02-26 11:45:26.000000 malpolon-1.1.0/malpolon/data/get_jpeg_patches_stats.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     5104 2024-05-14 09:58:48.000000 malpolon-1.1.0/malpolon/data/utils.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     3559 2024-02-26 17:06:46.000000 malpolon-1.1.0/malpolon/logging.py
+drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-05-14 13:12:57.013908 malpolon-1.1.0/malpolon/models/
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      156 2023-09-29 15:18:12.000000 malpolon-1.1.0/malpolon/models/__init__.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     9202 2024-02-26 11:45:26.000000 malpolon-1.1.0/malpolon/models/model_builder.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     5418 2024-02-26 11:45:26.000000 malpolon-1.1.0/malpolon/models/multi_modal.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)    10995 2024-05-14 09:58:48.000000 malpolon-1.1.0/malpolon/models/standard_prediction_systems.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     5028 2024-05-14 09:58:48.000000 malpolon-1.1.0/malpolon/models/utils.py
+drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-05-14 13:12:57.013908 malpolon-1.1.0/malpolon/plot/
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)        0 2023-09-29 15:18:12.000000 malpolon-1.1.0/malpolon/plot/__init__.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     4042 2024-02-26 11:45:26.000000 malpolon-1.1.0/malpolon/plot/history.py
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     4696 2024-05-14 09:58:48.000000 malpolon-1.1.0/malpolon/plot/map.py
+drwxrwxr-x   0 tlarcher  (1001) tlarcher  (1001)        0 2024-05-14 13:12:57.013908 malpolon-1.1.0/malpolon.egg-info/
+-rw-r--r--   0 tlarcher  (1001) tlarcher  (1001)     2085 2024-05-14 13:12:57.000000 malpolon-1.1.0/malpolon.egg-info/PKG-INFO
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     1081 2024-05-14 13:12:57.000000 malpolon-1.1.0/malpolon.egg-info/SOURCES.txt
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)        1 2024-05-14 13:12:57.000000 malpolon-1.1.0/malpolon.egg-info/dependency_links.txt
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)      374 2024-05-14 13:12:57.000000 malpolon-1.1.0/malpolon.egg-info/requires.txt
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)        9 2024-05-14 13:12:57.000000 malpolon-1.1.0/malpolon.egg-info/top_level.txt
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)       38 2024-05-14 13:12:57.013908 malpolon-1.1.0/setup.cfg
+-rw-rw-r--   0 tlarcher  (1001) tlarcher  (1001)     2336 2024-05-14 13:07:17.000000 malpolon-1.1.0/setup.py
```

### Comparing `malpolon-1.0.3/LICENSE.md` & `malpolon-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `malpolon-1.0.3/PKG-INFO` & `malpolon-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: malpolon
-Version: 1.0.3
-Summary: Malpolon v1.0.3
+Version: 1.1.0
+Summary: Malpolon v1.1.0
 Home-page: https://github.com/plantnet/malpolon
 Author: Theo Larcher, Titouan Lorieul
 Author-email: theo.larcher@inria.fr, titouan.lorieul@gmail.com
 Project-URL: Bug Reports, https://github.com/plantnet/malpolon/issues/new?assignees=aerodynamic-sauce-pan&labels=bug&projects=&template=bug_report.md&title=%5BBUG%5D
 Project-URL: Feature request, https://github.com/plantnet/malpolon/issues/new?assignees=aerodynamic-sauce-pan&labels=enhancement&projects=&template=enhancement.md&title=%5BEnhancement%5D
 Project-URL: Host organizer, https://plantnet.org/
 Project-URL: Source, https://github.com/plantnet/malpolon
@@ -26,24 +26,23 @@
 License-File: LICENSE.md
 Requires-Dist: Cartopy>=0.21.1
 Requires-Dist: kaggle>=1.5.16
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: omegaconf>=2.3.0
 Requires-Dist: pandas>=2.2.1
-Requires-Dist: Pillow>=10.0.1
-Requires-Dist: Pillow>=10.2.0
+Requires-Dist: Pillow>=10.3.0
 Requires-Dist: planetary_computer>=0.4.9
 Requires-Dist: pyproj>=3.6.1
 Requires-Dist: pystac>=1.6.1
 Requires-Dist: pytest>=7.2.2
 Requires-Dist: pytorch_lightning>=2.1.0
 Requires-Dist: rasterio>=1.3.8.post1
 Requires-Dist: scikit_learn>=1.1.3
 Requires-Dist: Shapely>=2.0.3
 Requires-Dist: tifffile>=2022.10.10
 Requires-Dist: timm>=0.9.2
 Requires-Dist: torch>=2.1.0
 Requires-Dist: torchgeo>=0.5.0
 Requires-Dist: torchmetrics>=1.2.0
 Requires-Dist: torchvision>=0.16.0
-Requires-Dist: tqdm>=4.66.1
+Requires-Dist: tqdm>=4.66.3
```

### Comparing `malpolon-1.0.3/README.md` & `malpolon-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 - [**Kaggle**](examples/kaggle/) : I am a potential kaggle participant on the GeoLifeClef challenge. I want to train a model on the provided datasets without having to worry about the data loading, starting from a plug-and-play example.
   - [<u>GeoLifeClef2022</u>](examples/kaggle/geolifeclef2022/) : contains a fully functionnal example of a model training on the GeoLifeClef2022 dataset, from data download, to training and prediction.
   - [<u>GeoLifeClef2023</u>](examples/kaggle/geolifeclef2023/) : contains dataloaders for the GeoLifeClef2023 dataset (different from the GLC2022 dataloaders). The training and prediction scripts are not provided.
 - [**Ecologists**](examples/ecologists/) : I have a dataset of my own and I want to train a model on it. I want to be able to easily customize the training process and the model architecture.
   - <u>Drop and play</u> : I have an observations file (.csv) and I want to train a model on different environmental variables (rasters, satellite imagery) without having to worry about the data loading.
   - <u>Custom dataset</u> : I have my own dataset consisting of pre-extracted image patches and/or rasters and I want to train a model on it.
 - [**Inference**](examples/inference/) : I have an observations file (.csv) and I want to predict the presence of species on a given area using a model I trained previously and a selected dataset or a shapefile I would provide.
+- [**Benchmark**](examples/benchmark/) : I want to compare the performance of different models on a given known dataset, or validate the framework's backbone (every module apart from the datasets and datamodule) on a specific hardware.
 
 ## 🔧 Installation
 
 To install malpolon, you will first need to install **Python ≥ 3.10**, and several python packages. To do so, it is best practice to create a virtual environment containing all these packages locally.
 
 ⚠️ **macOS** installation does not yet include instructions on how to properly set up GPU usage for GPU-enabled mac. For training purposes we recommend sticking to Linux for the time being. ⚠️
 
@@ -85,15 +86,15 @@
 ```
 
 ---
 
 #### 2. Create your virtual environment
 
 - **Via `virtualenv`**
-  
+
 We recommend handling your virtual environment using [`virtualenv`](https://virtualenv.pypa.io/en/stable/) (or similar) and installing the packages via `pip`.
 
 First create your virtual environment using the proper python version, and activate it _(note that in this example, the virtual environment "malpolon_env" will be installed in the current directory)_.
 
 ```script
 virtualenv -p /usr/bin/python3.10 ./malpolon_3.10
 source ./malpolon_3.10/bin/activate
@@ -202,17 +203,17 @@
   - [ ] Allow dataset intersections and unions
 - [ ] Allow data parallel training
   - [x] Multithreading
   - [ ] Multiprocessing
     - Issues may arise depending on hardware
 
 </details>
- 
+
 ## Libraries
-Here is an overview of the main Python librairies used in this project. 
+Here is an overview of the main Python librairies used in this project.
 
 * [![PyTorch](https://img.shields.io/badge/PyTorch-%23ee4c2c.svg?logo=pytorch&logoColor=white)](https://pytorch.org/) - To handle deep learning loops and dataloaders
 * [![PyTorch Lightning](https://img.shields.io/badge/PyTorch%20Lightning-%23792EE5.svg?logo=lightning&logoColor=white)](https://lightning.ai/docs/pytorch/stable/) - Deep learning framework which simplifies the usage of PyTorch elements
 * [![Numpy](https://img.shields.io/badge/Numpy-%234D77CF.svg?logo=numpy&logoColor=white)](https://numpy.org/) - For common computational operations
 * [![Torchgeo](https://img.shields.io/badge/Torchgeo-%23EE4C2C.svg?logo=torchgeo&logoColor=white)](https://torchgeo.readthedocs.io/en/stable/) - To handle data rasters
 * [![Matplotlib](https://img.shields.io/badge/Matplotlib-%2311557C.svg?logo=matplotlib&logoColor=white)](https://matplotlib.org/) - For displaying purposes
 * [![Hydra](https://img.shields.io/badge/Hydra-%23729DB1.svg?logo=hydra&logoColor=white)](https://hydra.cc/docs/intro/) - To handle models' hyperparameters
```

#### html2text {}

```diff
@@ -28,23 +28,26 @@
 architecture. - _D_r_o_p_ _a_n_d_ _p_l_a_y : I have an observations file (.csv) and I want
 to train a model on different environmental variables (rasters, satellite
 imagery) without having to worry about the data loading. - _C_u_s_t_o_m_ _d_a_t_a_s_e_t : I
 have my own dataset consisting of pre-extracted image patches and/or rasters
 and I want to train a model on it. - [**Inference**](examples/inference/) : I
 have an observations file (.csv) and I want to predict the presence of species
 on a given area using a model I trained previously and a selected dataset or a
-shapefile I would provide. ## ð§ Installation To install malpolon, you will
-first need to install **Python â¥ 3.10**, and several python packages. To do
-so, it is best practice to create a virtual environment containing all these
-packages locally. â ï¸ **macOS** installation does not yet include
-instructions on how to properly set up GPU usage for GPU-enabled mac. For
-training purposes we recommend sticking to Linux for the time being. â ï¸
-_C_l_i_c_k_ _h_e_r_e_ _t_o_ _e_x_p_a_n_d_ _i_n_s_t_r_u_c_t_i_o_n_s ### Requirements Before proceeding, please
-make sure the following packages are installed on your system: - [Python â¥
-3.10](https://www.python.org/downloads/) - [`pip`](https://pip.pypa.io/en/
+shapefile I would provide. - [**Benchmark**](examples/benchmark/) : I want to
+compare the performance of different models on a given known dataset, or
+validate the framework's backbone (every module apart from the datasets and
+datamodule) on a specific hardware. ## ð§ Installation To install malpolon,
+you will first need to install **Python â¥ 3.10**, and several python
+packages. To do so, it is best practice to create a virtual environment
+containing all these packages locally. â ï¸ **macOS** installation does not
+yet include instructions on how to properly set up GPU usage for GPU-enabled
+mac. For training purposes we recommend sticking to Linux for the time being.
+â ï¸ _C_l_i_c_k_ _h_e_r_e_ _t_o_ _e_x_p_a_n_d_ _i_n_s_t_r_u_c_t_i_o_n_s ### Requirements Before proceeding,
+please make sure the following packages are installed on your system: - [Python
+â¥ 3.10](https://www.python.org/downloads/) - [`pip`](https://pip.pypa.io/en/
 stable/installation/) - [`git`](https://git-scm.com/downloads) - `libgeos-dev`
 (dependency of Python library `Cartopy`) - On Linux (Ubuntu): `sudo apt install
 libgeos-dev` - On MacOS: `brew install geos` - `cmake` - On Linux (Ubuntu):
 `sudo apt install cmake` - On MacOS: `brew install cmake` - `cuda` (if you
 intend to run your models on GPU) - [`CUDA Installation guide`](https://
 docs.nvidia.com/cuda/index.html) - [`CuDNN Installation guide`](https://
 docs.nvidia.com/deeplearning/cudnn/install-guide/index.html) The following
```

### Comparing `malpolon-1.0.3/malpolon/check_install.py` & `malpolon-1.1.0/malpolon/check_install.py`

 * *Files identical despite different names*

### Comparing `malpolon-1.0.3/malpolon/data/data_module.py` & `malpolon-1.1.0/malpolon/data/data_module.py`

 * *Files 27% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         self.pin_memory = True
 
         self.dataset_train = None
         self.dataset_val = None
         self.dataset_test = None
         self.dataset_predict = None
         self.sampler = None
+        self.task = None
 
     @property
     @abstractmethod
     def train_transform(self) -> Callable:
         """Return train data transforms.
 
         Returns
@@ -256,29 +257,88 @@
         -------
         tuple[np.ndarray, np.ndarray]
             class labels and corresponding probabilities
         """
         device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
         classes = torch.tensor(classes).to(device)
         probas = activation_fn(predictions)
-        probas, indices = torch.sort(probas, descending=True)
-        probas, indices = probas.to(device), indices.to(device)
-        class_preds = torch.zeros(probas.shape[0], len(classes), device=device)
-        for batch_i in range(predictions.shape[0]):
-            class_preds[batch_i] = classes[indices[batch_i]]
+        if 'binary' in self.task:
+            class_preds = probas.round()
+        else:
+            probas, indices = torch.sort(probas, descending=True)
+            probas, indices = probas.to(device), indices.to(device)
+            class_preds = torch.zeros_like(probas, device=device)
+            for batch_i in range(predictions.shape[0]):  # useful if classes don't span from 0 to n_classes-1
+                class_preds[batch_i] = classes[indices[batch_i]]
+            if 'multiclass' in self.task:
+                class_preds, probas = class_preds[:, :1], probas[:, :1]
         return class_preds.to('cpu').numpy().astype(int), probas.to('cpu').numpy()
 
+    def export_predict_csv_basic(self,
+                                 predictions: Union[Tensor, np.ndarray],
+                                 targets: Union[np.ndarray, list],
+                                 probas: Union[Tensor, np.ndarray] = None,
+                                 ids: Union[np.ndarray, list] = None,
+                                 out_name: str = "predictions",
+                                 out_dir: str = './',
+                                 return_csv: bool = False,
+                                 top_k: int = None,
+                                 **kwargs: Any):
+        """Export predictions to csv file.
+
+        Exports predictions, probabilities and ids to a csv file.
+
+        Parameters
+        ----------
+        predictions : Union[Tensor, np.ndarray]
+            model's predictions.
+        targets : Union[np.ndarray, list], optional
+            target species ids, by default None
+        probas : Union[Tensor, np.ndarray], optional
+            predictions' raw logits or logits passed through an
+            activation function, by default None
+        ids : Union[np.ndarray, list], optional
+            ids of the observations, by default None
+        out_name : str, optional
+            output CSV file name, by default "predictions"
+        out_dir : str, optional
+            output directory name, by default "./"
+        return_csv : bool, optional
+            if true, the method returns the CSV as a pandas DataFrame,
+            by default False
+        top_k : int, optional
+            number of top predictions to return, by default None (max
+            number of predictions)
+
+        Returns
+        -------
+        pandas.DataFrame
+            CSV content as a pandas DataFrame if `return_csv` is True
+        """
+        predictions = [None] * len(predictions) if predictions is None else predictions
+        probas = [None] * len(probas) if probas is None else probas
+        ids = np.arange(len(predictions)) if ids is None else ids
+        df = pd.DataFrame({'ids': ids,
+                           'predictions': tuple(predictions[:, :top_k].astype(str)),
+                           'targets': targets,
+                           'probas': tuple(probas[:, :top_k].astype(str))})
+        for key in ['probas', 'predictions']:
+            df[key] = df[key].apply(' '.join)
+        df.to_csv(Path(out_dir) / Path(out_name + ".csv"), index=False, sep=',', **kwargs)
+        if return_csv:
+            return df
+
     def export_predict_csv(self,
                            predictions: Union[Tensor, np.ndarray],
                            probas: Union[Tensor, np.ndarray] = None,
                            single_point_query: dict = None,
                            out_name: str = "predictions",
                            out_dir: str = './',
                            return_csv: bool = False,
-                           top_k: int = 1,
+                           top_k: int = None,
                            **kwargs: Any) -> Any:
         """Export predictions to csv file.
 
         This method is used to export predictions to a csv file.
         It can be used with a single point query or with the whole
         test dataset.
         This method is adapted for a classification task with an
@@ -292,50 +352,62 @@
         ----------
         predictions : Union[Tensor, np.ndarray]
             model's predictions.
         probas : Union[Tensor, np.ndarray], optional
             predictions' raw logits or logits passed through an
             activation function, by default None
         single_point_query : dict, optional
-            query dictionnary of the single-point prediction, by default
-            None
+            query dictionnary of the single-point prediction.
+            'target_species_id' key is mandatory expects a list of
+            numpy arrays of species ids.
+            'predictions' and 'probas' keys expect numpy arrays of
+            predictions and probabilities.
+            By default None (whole test dataset predictions)
         out_name : str, optional
             output CSV file name, by default "predictions"
         out_dir : str, optional
             output directory name, by default "./"
         return_csv : bool, optional
             if true, the method returns the CSV as a pandas DataFrame,
             by default False
         top_k : int, optional
-            number of top predictions to return, by default 1
+            number of top predictions to return, by default None (max
+            number of predictions)
 
         Returns
         -------
         pandas.DataFrame
             CSV content as a pandas DataFrame if `return_csv` is True
         """
         out_name = out_name + ".csv" if not out_name.endswith(".csv") else out_name
         fp = Path(out_dir) / Path(out_name)
+        top_k = top_k if top_k is not None else predictions.shape[1]
         if single_point_query:
             df = pd.DataFrame({'observation_id': [single_point_query['observation_id'] if 'observation_id' in single_point_query else None],
                                'lon': [single_point_query['lon']],
                                'lat': [single_point_query['lat']],
                                'crs': [single_point_query['crs']],
-                               'target_species_id': [single_point_query['species_id'] if 'species_id' in single_point_query else None],
+                               'target_species_id': tuple(np.array(single_point_query['species_id']).astype(str) if 'species_id' in single_point_query else None),
                                'predictions': tuple(predictions[:, :top_k].astype(str)),
                                'probas': tuple(probas[:, :top_k].astype(str))})
         else:
             test_ds = self.get_test_dataset()
+            targets = test_ds.targets
             df = pd.DataFrame({'observation_id': test_ds.observation_ids,
                                'lon': [None] * len(test_ds) if not hasattr(test_ds, 'coordinates') else test_ds.coordinates[:, 0],
                                'lat': [None] * len(test_ds) if not hasattr(test_ds, 'coordinates') else test_ds.coordinates[:, 1],
-                               'target_species_id': test_ds.targets,
+                               'target_species_id': tuple(np.array(targets).astype(int).astype(str)),
                                'predictions': tuple(predictions[:, :top_k].astype(str)),
                                'probas': [None] * len(predictions)})
+            if 'multilabel' in self.task:
+                predictions_multilabel = []
+                for obs_id in df['observation_id']:
+                    predictions_multilabel.append(' '.join(targets[df.index[df['observation_id'] == obs_id].values].astype(str)))
+                df['target_species_id'] = predictions_multilabel  # values must already be strings since the number of targets may vary per obs_id, however pd.DataFrame expects arrays of same lengths
         if probas is not None:
             df['probas'] = tuple(probas[:, :top_k].astype(str))
-        df['predictions'] = df['predictions'].apply(' '.join)
-        df['probas'] = df['probas'].apply(' '.join)
+        for key in ['probas', 'predictions', 'target_species_id']:
+            if not isinstance(df.loc[0, key], str) and len(df.loc[0, key]) >= 1:
+                df[key] = df[key].apply(' '.join)
         df.to_csv(fp, index=False, sep=';', **kwargs)
         if return_csv:
             return df
-        return None
```

### Comparing `malpolon-1.0.3/malpolon/data/datasets/_data/minigeolifeclef2022_species_details.csv` & `malpolon-1.1.0/malpolon/data/datasets/_data/minigeolifeclef2022_species_details.csv`

 * *Files identical despite different names*

### Comparing `malpolon-1.0.3/malpolon/data/datasets/geolifeclef2022.py` & `malpolon-1.1.0/malpolon/data/datasets/geolifeclef2022.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,14 +287,15 @@
         patch_data: str = "all",
         use_rasters: bool = True,
         patch_extractor: Optional[PatchExtractor] = None,
         use_localisation: bool = False,
         transform: Optional[Callable] = None,
         target_transform: Optional[Callable] = None,
         download: bool = False,
+        **kwargs,
     ):
         root = Path(root)
 
         possible_subsets = ["train", "val", "train+val", "test"]
         if subset not in possible_subsets:
             raise ValueError(f"Possible values for 'subset' are:"
                              f" {possible_subsets} (given {subset})")
@@ -483,14 +484,15 @@
         patch_data: str = "all",
         use_rasters: bool = True,
         patch_extractor: Optional[PatchExtractor] = None,
         use_localisation: bool = False,
         transform: Optional[Callable] = None,
         target_transform: Optional[Callable] = None,
         download: bool = False,
+        **kwargs,
     ):
         super().__init__(
             root,
             subset,
             region="fr",
             patch_data=patch_data,
             use_rasters=use_rasters,
@@ -514,23 +516,23 @@
         else:
             subset_file_suffix = "train"
 
         df = pd.read_csv(
             root / "observations" / f"observations_fr_{subset_file_suffix}.csv",
             sep=";",
             index_col="observation_id",
-        )
+        )[:600]
 
         file_name = "minigeolifeclef2022_species_details.csv"
         with resources.path(DATA_MODULE, file_name) as species_file_path:
             df_species = pd.read_csv(
                 species_file_path,
                 sep=";",
                 index_col="species_id",
-            )
+            )[:600]
 
         df = df[np.isin(df["species_id"], df_species.index)]
         value_counts = df.species_id.value_counts()
         species_id = value_counts.iloc[:100].index
         df_species = df_species.loc[species_id]
         df = df[np.isin(df["species_id"], df_species.index)]
 
@@ -583,14 +585,15 @@
         patch_data="all",
         use_rasters=True,
         patch_extractor=None,
         use_localisation=False,
         transform=None,
         target_transform=None,
         download=False,
+        **kwargs,
     ):
         root = Path(root)
 
         self.root = root
         self.subset = subset
         self.patch_data = patch_data
         self.use_localisation = use_localisation
```

### Comparing `malpolon-1.0.3/malpolon/data/datasets/geolifeclef2023.py` & `malpolon-1.1.0/malpolon/data/datasets/geolifeclef2023.py`

 * *Files identical despite different names*

### Comparing `malpolon-1.0.3/malpolon/data/datasets/torchgeo_datasets.py` & `malpolon-1.1.0/malpolon/data/datasets/torchgeo_datasets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """This module provides raster related classes based on torchgeo.
 
 Author: Theo Larcher <theo.larcher@inria.fr>
 """
-
 from __future__ import annotations
 
+import math
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Dict, Sequence, Union
 
 import numpy as np
 import pandas as pd
 import pyproj
+from matplotlib import pyplot as plt
 from pyproj import CRS, Transformer
 from torchgeo.datasets import BoundingBox, RasterDataset
 from torchgeo.samplers import Units
 
 from malpolon.data.utils import is_point_in_bbox, to_one_hot_encoding
 
 if TYPE_CHECKING:
     import numpy.typing as npt
-
     Patches = npt.NDArray
     Targets = npt.NDArray[np.int64]
 
 ALL_NORTHERN_EPSG_CODES = list(range(32601, 32662))
 EUROPE_EPSG_CODE = [3035]
 
-
 class RasterTorchGeoDataset(RasterDataset):
     """Generic torchgeo based raster datasets.
 
     Datasets based on this class return patches from raster files and
     can be queried by either a torchgeo BoundingBox object, a tuple of
     coordinates in the dataset's CRS or a dictionary specifying
     coordinates and the wanted CRS. Additionally one can specify the
@@ -38,85 +37,131 @@
     dataset's.
 
     RasterTorchGeoDataset inherits torchgeo's RasterDataset class.
     """
     def __init__(
         self,
         root: str = "data",
-        split: str = None,  # 'train', 'test', 'val', 'all'
         labels_name: str = None,
-        crs: Any | None = None,
-        res: float | None = None,
-        bands: Sequence[str] | None = None,
-        transforms_data: Callable[[Dict[str, Any]], Dict[str, Any]] | None = None,
-        cache: bool = True,
+        split: str = None,  # 'train', 'test', 'val', 'all'
+        crs: Any = None,
+        res: float = None,
+        bands: Sequence[str] = None,
+        transform: Callable = None,
+        transform_target: Callable = None,
         patch_size: Union[int, float, tuple] = 256,
+        query_units: str = 'pixel',
+        query_crs: Union[int, str, CRS] = 'self',
+        obs_data_columns: dict = {'x': 'lon',
+                                  'y': 'lat',
+                                  'index': 'surveyId',
+                                  'species_id': 'speciesId',
+                                  'split': 'subset'},
         task: str = 'multiclass',  # ['binary', 'multiclass', 'multilabel']
-        binary_positive_classes: list = []
+        binary_positive_classes: list = [],
+        cache: bool = True,
     ) -> None:
         """Class constructor.
 
         Parameters
         ----------
         root : str, optional
             path to the directory containing the data and labels, by default "data"
-        split : str, optional
-            dataset subset desired for labels selection, by default None
         labels_name : str, optional
             labels file name, by default None
+        split : str, optional
+            dataset subset desired for labels selection, by default None
         crs : Any | None, optional
             `coordinate reference system (CRS)` to warp to
             (defaults to the CRS of the first file found), by default None
         res : float | None, optional
             resolution of the dataset in units of CRS
             (defaults to the resolution of the first file found), by default None
         bands : Sequence[str] | None, optional
             bands to return (defaults to all bands), by default None
-        transforms_data : Callable[[Dict[str, Any]], Dict[str, Any]] | None, optional
-            a function/transform that takes an input sample and returns
+        transform : Callable | None, optional
+            a callable function that takes an input sample and returns
+            a transformed version, by default None
+        transform_target : Callable | None, optional
+            a callable function that takes an input target and returns
             a transformed version, by default None
-        cache : bool, optional
-            if True, cache file handle to speed up repeated sampling, by default True
         patch_size : int, optional
             size of the 2D extracted patches. Patches can either be
             square (int/float value) or rectangular (tuple of int/float).
             Defaults to a square of size 256, by default 256
+        query_units : str, optional
+            unit system of the dataset's queries, by default 'pixel'
+        query_crs: Union[int, str, CRS], optional
+            CRS of the dataset's queries, by default 'self' (same as dataset's CRS)
+        obs_data_columns: dict, optional
+            this dictionary allows users to match the dataset attributes
+            with custom column names of their obs data file,
+            by default::
+
+              {'x': 'lon',
+               'y': 'lat',
+               'index': 'surveyId',
+               'species_id': 'speciesId',
+               'split': 'subset'}
+
+            Here's a description of the keys:
+
+            - 'x', 'y': coordinates of the obs points (by default 'lon', 'lat' as per the WGS84 system)
+            - 'index': obs ID over which to iterate during the training loop
+            - 'species_id': species ID (label) associated with the obs points
+            - 'split': dataset split column name
+
         task : str, optional
             machine learning task (used to format labels accordingly), by default 'multiclass'
         binary_positive_classes : list, optional
             labels' classes to consider valid in the case of binary
             classification with multi-class labels (defaults to all 0),
             by default []
+        cache : bool, optional
+            if True, cache file handle to speed up repeated sampling, by default True
         """
         super().__init__(root, crs, res, bands, None, cache)
         self.patch_size = patch_size
         self.crs_pyproj = CRS(self.crs.data['init']) if self.crs.is_epsg_code else self.crs
         self.units = self.crs_pyproj.axis_info[0].unit_name if self.crs.is_epsg_code else self.crs.data['units']
         self.training = split != "test"
         self.task = task
         self.binary_positive_classes = set(binary_positive_classes)
-        self.transforms_data = transforms_data
+        self.transform = transform
+        self.transform_target = transform_target
+        self._query_units = query_units
+        self._query_crs = query_crs
+        self._load_observation_data(Path(root), labels_name, split, obs_data_columns)
+        # df = self._load_observation_data(Path(root), labels_name, split)
+        # self.observation_ids = df.index
+        # self.coordinates = df[["lon", "lat"]].values
+        # self.targets = df["speciesId"].values
+        # self._query_units = query_units
+        # self._query_crs = query_crs
 
-        df = self._load_observation_data(Path(root), labels_name, split)
-        self.observation_ids = df.index
-        self.coordinates = df[["longitude", "latitude"]].values
-        self.targets = df["species_id"].values
+    def __len__(self) -> int:
+        return len(self.observation_ids)
 
     def _load_observation_data(
         self,
         root: Path = None,
         obs_fn: str = None,
         subsets: str = ['train', 'test', 'val'],
+        keys: dict = {'x': 'lon',
+                      'y': 'lat',
+                      'index': 'surveyId',
+                      'species_id': 'speciesId',
+                      'split': 'subset'}
     ) -> pd.DataFrame:
         """Load observation data from a CSV file.
 
         Reads values from a CSV file containing lon/lat coordinates,
         species id (labels) and dataset subset info (train/test/val).
         The associated columns must have the following values:
-        ['longitude', 'latitude', 'species_id', 'subset']
+        ['longitude', 'latitude', 'speciesId', 'subset']
 
         If no value is given to root or obs_fn, the method returns an
         empty labels DataFrame.
 
         Parameters
         ----------
         root : Path
@@ -128,32 +173,44 @@
             ["train", "test", "val"] (no restriction).
 
         Returns
         -------
         pd.DataFrame
             labels DataFrame
         """
+        x_key, y_key = keys['x'], keys['y']
+        index_key = keys['index']
+        species_id_key = keys['species_id']
+        split_key = keys['split']
+
         if any([root is None, obs_fn is None]):
-            return pd.DataFrame(columns=['longitude', 'latitude', 'species_id', 'subset'])
+            df = pd.DataFrame(columns=[x_key, y_key, species_id_key, split_key])
+            self.observation_ids = df.index
+            self.coordinates = df[["lon", "lat"]].values
+            self.targets = df["speciesId"].values
+            return df
         labels_fp = obs_fn if len(obs_fn.split('.csv')) >= 2 else f'{obs_fn}.csv'
         labels_fp = root / labels_fp
         df = pd.read_csv(
             labels_fp,
             sep=",",
-            index_col="observation_id",
+            index_col=index_key,
         )
-        self.unique_labels = np.sort(np.unique(df['species_id']))
+        self.unique_labels = np.sort(np.unique(df[species_id_key]))
         try:
             subsets = [subsets] if isinstance(subsets, str) else subsets
-            ind = df.index[df["subset"].isin(subsets)]
+            ind = np.unique(df.index[df[split_key].isin(subsets)])
             df = df.loc[ind]
         except ValueError as e:
             print('Unrecognized subset name.\n'
                   'Please use one or several amongst: ["train", "test", "val"], as a string or list of strings.\n',
                   {e})
+        self.observation_ids = df.index
+        self.coordinates = df[[x_key, y_key]].values
+        self.targets = df[species_id_key].values
         return df
 
     def coords_transform(
         self,
         lon: Union[int, float],
         lat: Union[int, float],
         input_crs: Union[str, int, CRS] = "4326",
@@ -297,33 +354,34 @@
         if query['crs'] != epsg4326:
             transformer = Transformer.from_crs(query['crs'], epsg4326)
             coords_4326 = transformer.transform(query['lon'], query['lat'])
             coords_4326 = coords_4326[1], coords_4326[0]
         if self.crs_pyproj != epsg4326:
             transformer = Transformer.from_crs(self.crs_pyproj, epsg4326)
             bounds_4326 = transformer.transform_bounds(self.bounds.minx, self.bounds.miny, self.bounds.maxx, self.bounds.maxy)
-            bounds_4326 = (bounds_4326[1], bounds_4326[0], bounds_4326[3], bounds_4326[2])
+            bounds_4326 = (bounds_4326[1], bounds_4326[3], bounds_4326[0], bounds_4326[2])
         return is_point_in_bbox(coords_4326, bounds_4326)
 
     def _format_label_to_task(
         self,
         label: np.ndarray
     ) -> Union[np.ndarray, int]:
         """Format label(s) returned to match the task type.
 
         Depending on the classification task (binary, multiclass or
         multilabel), labels have to be formatted accordingly.
+
         - **Binary**: label is an `int` equal to 1 if potential labels,
         i.e. input label values, contain an elligible value (i.e. in
         self.binary_positive_classes); 0 otherwise.
         - **Multiclass**: label is an `int` which value can be any
-        class index (i.e. 'species_id'). If several label match a
+        class index (i.e. 'speciesId'). If several label match a
         coordinate set, the 1st one of the lsit is choosen.
         - **Multilabel**: label is a list of class index, containing all
-        species_id observed to a coordinate set.
+        speciesId observed to a coordinate set.
 
         Parameters
         ----------
         label : np.ndarray
             Potential labels matching a coordinate set.
 
         Returns
@@ -373,32 +431,45 @@
         Union[np.ndarray, int]
             target label(s).
         """
         if obs_id is None:
             return self.targets[df.index[(df['lon'] == query_lon) & (df['lat'] == query_lat)].values]
         return self.targets[df.index[df['observation_id'] == obs_id].values]
 
+    def _default_sample_to_getitem(
+        self,
+        idx: int,
+    ) -> Dict[str, Any]:
+        coords = tuple(self.coordinates[idx])
+        obs_id = self.observation_ids[idx]
+        return {'lon': coords[0], 'lat': coords[1],
+                'crs': self._query_crs,
+                'size': self.patch_size,
+                'units': self._query_units,
+                'obs_id': obs_id}
+
     def __getitem__(
         self,
-        query: Union[dict, tuple, list, set, BoundingBox]
+        query: Union[int, dict, tuple, list, set, BoundingBox]
     ) -> Dict[str, Any]:
         """Query an item from the dataset.
 
         Supports querying the dataset with coordinates in the dataset's CRS
         or in another CRS.
         The dataset is always queried with a torchgeo BoundingBox because it is
         itself a torchgeo dataset, but the query in this getter method can be
         passed as a tuple, list, set, dict or BoundingBox.
+
         - Use case 1: query is a [list, tuple, set] of 2 elements : lon, lat.
-        Here the CRS and Units system are by default those of the dataset's.
+          Here the CRS and Units system are by default those of the dataset's.
         - Use case 2: query is a torchgeo BoundingBox.
-        Here the CRS and Units system are by default those of the dataset's.
+          Here the CRS and Units system are by default those of the dataset's.
         - Use case 3: query is a dict containing the following necessary keys: {'lon', 'lat'},
-        and optional keys: {'crs', 'units', 'size'} which values default to those of
-        the dataset's.
+          and optional keys: {'crs', 'units', 'size'} which values default to those of
+          the dataset's.
 
         In Use case 3, if the 'crs' key is registered and it is different from
         the dataset's CRS, the coordinates of the point are projected into the
         dataset's CRS and the value of the key is overwritten by said CRS.
 
         Use cases 1 and 3 give the possibility to easily query the dataset using
         only a point and a bounding box (bbox) size, using the desired input CRS.
@@ -413,17 +484,21 @@
         ----------
         query : Union[dict, tuple, BoundingBox]
             item query containing geographical coordinates. It can be of
             different types for different use.
             One can query a patch by providing a BoundingBox using
             `torchgeo.datasets.BoundingBox` constructor; or by given a center
             and a size.
+
             --- BoundingBox strategy ---
+
             Must follow : BoundingBox(minx, maxx, miny, maxy, mint, maxt)
+
             --- Point strategy ---
+
             If tuple, must follow : (lon, lat) and the CRS of the coordinates
             will be assumed to be the dataset's.
             If dict, must follow : {'lon': lon, 'lat': lat, <'crs': crs>} and
             the coordinates CRS can be specified. If not, it will be assumed
             that it is equal to the dataset's.
             In both cases, a BoundingBox is generated to pursue the query.
 
@@ -462,14 +537,77 @@
             patch = super().__getitem__(query)
             df = pd.DataFrame(self.coordinates, columns=['lon', 'lat'])
             df['observation_id'] = self.observation_ids
 
             label = self.get_label(df, query_lon, query_lat, query_obs_id)
             label = self._format_label_to_task(label)
             sample = patch['image']
-            if self.transforms_data is not None:
-                sample = self.transforms_data(sample)
+            if self.transform:
+                sample = self.transform(sample)
+            if self.transform_target:
+                label = self.transform_target(label)
             return sample, label
         sample = super().__getitem__(query)
-        if self.transforms_data is not None:
-            sample = self.transforms_data(sample)
+        if self.transform is not None:
+            sample = self.transform(sample)
         return sample
+
+class RasterBioclim(RasterTorchGeoDataset):
+    """Raster dataset adapted for Sentinel-2 data.
+
+    Inherits RasterTorchGeoDataset.
+    """
+    filename_glob = "bio_*.tif"
+    filename_regex = r"(?P<band>bio_[\d])"
+    date_format = "%Y%m%dT%H%M%S"
+    is_image = True
+    separate_files = True
+    all_bands = ["bio_1", "bio_2", "bio_3", "bio_4"]
+    plot_bands = 'all_bands'
+
+    def __init__(self, root: str = "data", labels_name: str = None, split: str = None, crs: Any = None, res: float = None, bands: Sequence[str] = None, transform: Callable[..., Any] = None, transform_target: Callable[..., Any] = None, patch_size: int | float | tuple = 256, query_units: str = 'pixel', query_crs: int | str | CRS = 'self', obs_data_columns: Dict = { 'x': 'lon','y': 'lat','index': 'surveyId','species_id': 'speciesId','split': 'subset' }, task: str = 'multiclass', binary_positive_classes: list = [], cache: TYPE_CHECKING = True, **kwargs) -> None:
+        super().__init__(root, labels_name, split, crs, res, bands, transform, transform_target, patch_size, query_units, query_crs, obs_data_columns, task, binary_positive_classes, cache)
+        self.__dict__.update(kwargs)
+        if self.plot_bands == 'plot_bands':
+            self.plot_bands = self.all_bands
+
+    def plot(self, sample: Patches):
+        """Plot all layers of a given patch.
+
+        A patch is selected based on a key matching the associated
+        provider's __get__() method.
+
+        Args:
+            item (dict): provider's get index.
+        """
+        nb_layers = len(self.plot_bands)
+        patch = self[sample]
+        if nb_layers == 1:
+            plt.figure(figsize=(10, 10))
+            plt.imshow(patch[0])
+        else:
+            # calculate the number of rows and columns for the subplots grid
+            rows = int(math.ceil(math.sqrt(nb_layers)))
+            cols = int(math.ceil(nb_layers / rows))
+
+            # create a figure with a grid of subplots
+            fig, axs = plt.subplots(rows, cols, figsize=(10, 10))
+
+            # flatten the subplots array to easily access the subplots
+            axs = axs.flatten()
+
+            # loop through the layers of patch data
+            for i, band_name in enumerate(self.plot_bands):
+                # display the layer on the corresponding subplot
+                axs[i].imshow(patch[i])
+                axs[i].set_title(f'layer_{i}: {band_name}')
+                axs[i].axis('off')
+
+            # remove empty subplots
+            for i in range(nb_layers, rows * cols):
+                fig.delaxes(axs[i])
+
+        plt.suptitle('Tensor for sample: ' + str(sample), fontsize=16)
+
+        # show the plot
+        plt.tight_layout(rect=[0, 0.03, 1, 0.95])
+        plt.show()
```

### Comparing `malpolon-1.0.3/malpolon/data/datasets/torchgeo_sentinel2.py` & `malpolon-1.1.0/malpolon/data/datasets/torchgeo_sentinel2.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pystac
 import torch
 from matplotlib import pyplot as plt
 from matplotlib.figure import Figure
 from torch.utils.data import DataLoader
 from torchgeo.datasets import BoundingBox, GeoDataset
 from torchgeo.datasets.utils import download_url
-from torchgeo.samplers import GeoSampler, Units
+from torchgeo.samplers import GeoSampler
 from torchvision import transforms
 
 from malpolon.data.data_module import BaseDataModule
 from malpolon.data.datasets.torchgeo_datasets import RasterTorchGeoDataset
 
 if TYPE_CHECKING:
     import numpy.typing as npt
@@ -40,19 +40,21 @@
         self,
         dataset_path: str,
         labels_name: str = 'labels.csv',
         train_batch_size: int = 32,
         inference_batch_size: int = 256,
         num_workers: int = 8,
         size: int = 200,
-        units: Units = Units.CRS,
+        units: str = 'pixel',
         crs: int = 4326,
         binary_positive_classes: list = [],
         task: str = 'classification_multiclass',  # ['classification_binary', 'classification_multiclass', 'classification_multilabel']
-        download_data_sample: bool = False
+        dataset_kwargs: dict = {},
+        download_data_sample: bool = False,
+        **kwargs,
     ):
         """Class constructor.
 
         Parameters
         ----------
         dataset_path : str
             path to the directory containing the data
@@ -83,24 +85,29 @@
         binary_positive_classes : list, optional
             labels' classes to consider valid in the case of binary
             classification with multi-class labels (defaults to all 0),
             by default []
         task : str, optional
             machine learning task (used to format labels accordingly),
             by default 'classification_multiclass'
+        dataset_kwargs : dict, optional
+            additional keyword arguments for the dataset, by default {}
+        download_data_sample: bool, optional
+            whether to download a sample of Sentinel-2 data, by default False
         """
         super().__init__(train_batch_size, inference_batch_size, num_workers)
         self.dataset_path = dataset_path
         self.labels_name = labels_name
         self.size = size
         self.units = units
         self.crs = crs
         self.sampler = Sentinel2GeoSampler
         self.task = task
         self.binary_positive_classes = binary_positive_classes
+        self.dataset_kwargs = dataset_kwargs
         if download_data_sample:
             self.download_data_sample()
 
     def download_data_sample(self):
         """Download 4 Sentinel-2A tiles from MPC.
 
         This method is useful to quickly download a sample of
@@ -117,22 +124,22 @@
             signed_item = planetary_computer.sign(item)
             for band in ["B08", "B03", "B02", "B04"]:
                 asset_href = signed_item.assets[band].href
                 filename = urlparse(asset_href).path.split("/")[-1]
                 download_url(asset_href, self.dataset_path, filename)
 
     def get_dataset(self, split, transform, **kwargs):
-        dataset = RasterBio(
+        dataset = RasterSentinel2(
             self.dataset_path,
             labels_name=self.labels_name,
             split=split,
             task=self.task,
             binary_positive_classes=self.binary_positive_classes,
-            transforms_data=transform,
-            **kwargs
+            transform=transform,
+            **self.dataset_kwargs
         )
         return dataset
 
     def train_dataloader(self) -> DataLoader:
         dataloader = DataLoader(
             self.dataset_train,
             sampler=self.sampler(self.dataset_train, size=self.size, units=self.units, crs=self.crs),
@@ -199,67 +206,14 @@
                 transforms.Normalize(
                     mean=[0.485, 0.456, 0.406, 0.2],
                     std=[0.229, 0.224, 0.225, 0.2]
                 ),
             ]
         )
 
-# Chantier
-
-class RasterBio(RasterTorchGeoDataset):
-    """Raster dataset adapted for Sentinel-2 data.
-
-    Inherits RasterTorchGeoDataset.
-    """
-    filename_glob = "bio*.tif"
-    filename_regex = r"bio_[\d]"
-    date_format = "%Y%m%dT%H%M%S"
-    is_image = True
-    separate_files = True
-    all_bands = ["1", "2", "3", "4"]
-    plot_bands = ["1", "2", "3", "4"]
-
-    def plot(
-        self,
-        sample: Patches
-    ) -> Figure:
-        """Plot a 3-bands dataset patch (sample).
-
-        Plots a dataset sample by selecting the 3 bands indicated in
-        the `plot_bands` variable (in the same order).
-        By default, the method plots the RGB bands.
-
-        Parameters
-        ----------
-        sample : Patches
-            dataset's patch to plot
-
-        Returns
-        -------
-        Figure
-            matplotlib figure containing the plot
-        """
-        # Find the correct band index order
-        plot_indices = []
-        for band in self.plot_bands:
-            plot_indices.append(self.all_bands.index(band))
-
-        # Reorder and rescale the image
-        image = sample[plot_indices].permute(1, 2, 0)
-        image = torch.clamp(image / 10000, min=0, max=1).numpy()
-
-        # Plot the image
-        fig, ax = plt.subplots()
-        ax.imshow(image)
-
-        return fig
-
-# Fin chantier
-
-
 
 class RasterSentinel2(RasterTorchGeoDataset):
     """Raster dataset adapted for Sentinel-2 data.
 
     Inherits RasterTorchGeoDataset.
     """
     filename_glob = "T*_B0*_10m.tif"
@@ -366,15 +320,15 @@
 
     def __init__(
         self,
         dataset: GeoDataset,
         size: Union[Tuple[float, float], float],
         length: Optional[int] = None,
         roi: Optional[BoundingBox] = None,
-        units: Units = 'pixel',
+        units: str = 'pixel',
         crs: str = 'crs',
     ) -> None:
         super().__init__(dataset, roi)
         self.units = units
         self.crs = crs
         self.size = (size, size) if isinstance(size, (int, float)) else size
         self.coordinates = dataset.coordinates
```

### Comparing `malpolon-1.0.3/malpolon/data/environmental_raster.py` & `malpolon-1.1.0/malpolon/data/environmental_raster.py`

 * *Files identical despite different names*

### Comparing `malpolon-1.0.3/malpolon/data/get_jpeg_patches_stats.py` & `malpolon-1.1.0/malpolon/data/get_jpeg_patches_stats.py`

 * *Files identical despite different names*

### Comparing `malpolon-1.0.3/malpolon/data/utils.py` & `malpolon-1.1.0/malpolon/data/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,22 +65,22 @@
     method: str = 'shapely'
 ) -> bool:
     """Determine if a 2D point in included inside of a 2D bounding box.
 
     Returns a boolean answering the question "Is point contained inside
     bbox ?".
     Point must follow the format: [x, y]
-    Bounding boxe must follow the format: [xmin, ymin, xmax, ymax]
+    Bounding box must follow the format: [xmin, ymin, xmax, ymax]
 
     Parameters
     ----------
     point : Iterable
-        Point.
+        Point in the format [x, y].
     bbox : Iterable
-        Bounding box.
+        Bounding box in the format [xmin, xmax, ymin, ymax].
     method : str
         Method to use for comparison. Can take any value in
         ['shapely', 'manual'], by default 'shapely'.
 
     Returns
     -------
     boolean
```

### Comparing `malpolon-1.0.3/malpolon/logging.py` & `malpolon-1.1.0/malpolon/logging.py`

 * *Files identical despite different names*

### Comparing `malpolon-1.0.3/malpolon/models/model_builder.py` & `malpolon-1.1.0/malpolon/models/model_builder.py`

 * *Files identical despite different names*

### Comparing `malpolon-1.0.3/malpolon/models/multi_modal.py` & `malpolon-1.1.0/malpolon/models/multi_modal.py`

 * *Files identical despite different names*

### Comparing `malpolon-1.0.3/malpolon/models/standard_prediction_systems.py` & `malpolon-1.1.0/malpolon/models/standard_prediction_systems.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,30 +70,30 @@
             y = y.to(torch.float32)
         return y
 
     def _step(
         self, split: str, batch: tuple[Any, Any], batch_idx: int
     ) -> Union[Tensor, dict[str, Any]]:
         if split == "train":
-            log_kwargs = {"on_step": False, "on_epoch": True, "sync_dist": True}
+            log_kwargs = {"on_step": True, "on_epoch": True, "sync_dist": True}
         else:
-            log_kwargs = {}
+            log_kwargs = {"on_step": True, "on_epoch": True, "sync_dist": True}
 
         x, y = batch
         y_hat = self(x)
 
         loss = self.loss(y_hat, self._cast_type_to_loss(y))  # Shape mismatch for binary: need to 'y = y.unsqueeze(1)' (or use .reshape(2)) to cast from [2] to [2,1] and cast y to float with .float()
-        self.log(f"{split}_loss", loss, **log_kwargs)
+        self.log(f"loss/{split}", loss, **log_kwargs)
 
         for metric_name, metric_func in self.metrics.items():
             if isinstance(metric_func, dict):
                 score = metric_func['callable'](y_hat, y, **metric_func['kwargs'])
             else:
                 score = metric_func(y_hat, y)
-            self.log(f"{split}_{metric_name}", score, **log_kwargs)
+            self.log(f"{metric_name}/{split}", score, **log_kwargs)
 
         return loss
 
     def training_step(
         self, batch: tuple[Any, Any], batch_idx: int
     ) -> Union[Tensor, dict[str, Any]]:
         return self._step("train", batch, batch_idx)
@@ -298,15 +298,15 @@
         optimizer = torch.optim.SGD(
             model.parameters(),
             lr=self.lr,
             weight_decay=self.weight_decay,
             momentum=self.momentum,
             nesterov=self.nesterov,
         )
-        if ('binary' or 'multilabel') in task:
+        if 'binary' in task or 'multilabel' in task:
             loss = torch.nn.BCEWithLogitsLoss()
         else:
             loss = torch.nn.CrossEntropyLoss()
 
         if metrics is None:
             metrics = {
                 "accuracy": {'callable': Fmetrics.classification.binary_accuracy,
```

### Comparing `malpolon-1.0.3/malpolon/models/utils.py` & `malpolon-1.1.0/malpolon/models/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     Returns
     -------
     OmegaConf
         user's metrics with their corresponding callable function
     """
     try:
-        metrics = OmegaConf.to_container(metrics)
+        metrics = OmegaConf.to_container(metrics, resolve=True)
         for k, v in metrics.items():
             if 'callable' in v:
                 metrics[k]['callable'] = eval(v['callable'])
             else:
                 metrics[k]['callable'] = FMETRICS_CALLABLES[k]
     except ValueError as e:
         print('\n[WARNING]: Please make sure you have registered'
```

### Comparing `malpolon-1.0.3/malpolon/plot/history.py` & `malpolon-1.1.0/malpolon/plot/history.py`

 * *Files identical despite different names*

### Comparing `malpolon-1.0.3/malpolon.egg-info/PKG-INFO` & `malpolon-1.1.0/malpolon.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: malpolon
-Version: 1.0.3
-Summary: Malpolon v1.0.3
+Version: 1.1.0
+Summary: Malpolon v1.1.0
 Home-page: https://github.com/plantnet/malpolon
 Author: Theo Larcher, Titouan Lorieul
 Author-email: theo.larcher@inria.fr, titouan.lorieul@gmail.com
 Project-URL: Bug Reports, https://github.com/plantnet/malpolon/issues/new?assignees=aerodynamic-sauce-pan&labels=bug&projects=&template=bug_report.md&title=%5BBUG%5D
 Project-URL: Feature request, https://github.com/plantnet/malpolon/issues/new?assignees=aerodynamic-sauce-pan&labels=enhancement&projects=&template=enhancement.md&title=%5BEnhancement%5D
 Project-URL: Host organizer, https://plantnet.org/
 Project-URL: Source, https://github.com/plantnet/malpolon
@@ -26,24 +26,23 @@
 License-File: LICENSE.md
 Requires-Dist: Cartopy>=0.21.1
 Requires-Dist: kaggle>=1.5.16
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: omegaconf>=2.3.0
 Requires-Dist: pandas>=2.2.1
-Requires-Dist: Pillow>=10.0.1
-Requires-Dist: Pillow>=10.2.0
+Requires-Dist: Pillow>=10.3.0
 Requires-Dist: planetary_computer>=0.4.9
 Requires-Dist: pyproj>=3.6.1
 Requires-Dist: pystac>=1.6.1
 Requires-Dist: pytest>=7.2.2
 Requires-Dist: pytorch_lightning>=2.1.0
 Requires-Dist: rasterio>=1.3.8.post1
 Requires-Dist: scikit_learn>=1.1.3
 Requires-Dist: Shapely>=2.0.3
 Requires-Dist: tifffile>=2022.10.10
 Requires-Dist: timm>=0.9.2
 Requires-Dist: torch>=2.1.0
 Requires-Dist: torchgeo>=0.5.0
 Requires-Dist: torchmetrics>=1.2.0
 Requires-Dist: torchvision>=0.16.0
-Requires-Dist: tqdm>=4.66.1
+Requires-Dist: tqdm>=4.66.3
```

### Comparing `malpolon-1.0.3/malpolon.egg-info/SOURCES.txt` & `malpolon-1.1.0/malpolon.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 malpolon/data/environmental_raster.py
 malpolon/data/get_jpeg_patches_stats.py
 malpolon/data/utils.py
 malpolon/data/datasets/__init__.py
 malpolon/data/datasets/_base.py
 malpolon/data/datasets/geolifeclef2022.py
 malpolon/data/datasets/geolifeclef2023.py
+malpolon/data/datasets/geolifeclef2024.py
+malpolon/data/datasets/torchgeo_concat.py
 malpolon/data/datasets/torchgeo_datasets.py
 malpolon/data/datasets/torchgeo_sentinel2.py
 malpolon/data/datasets/_data/__init__.py
 malpolon/data/datasets/_data/minigeolifeclef2022_species_details.csv
 malpolon/models/__init__.py
 malpolon/models/model_builder.py
 malpolon/models/multi_modal.py
```

### Comparing `malpolon-1.0.3/setup.py` & `malpolon-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(name="malpolon",
-      version="1.0.3",
-      description="Malpolon v1.0.3",
+      version="1.1.0",
+      description="Malpolon v1.1.0",
       author="Theo Larcher, Titouan Lorieul",
       author_email="theo.larcher@inria.fr, titouan.lorieul@gmail.com",
       url="https://github.com/plantnet/malpolon",
       classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
@@ -30,31 +30,30 @@
       install_requires=[
         "Cartopy>=0.21.1",
         "kaggle>=1.5.16",
         "matplotlib>=3.8.0",
         "numpy>=1.26.4",
         "omegaconf>=2.3.0",
         "pandas>=2.2.1",
-        "Pillow>=10.0.1",
-        "Pillow>=10.2.0",
+        "Pillow>=10.3.0",
         "planetary_computer>=0.4.9",
         "pyproj>=3.6.1",
         "pystac>=1.6.1",
         "pytest>=7.2.2",
         "pytorch_lightning>=2.1.0",
         "rasterio>=1.3.8.post1",
         "scikit_learn>=1.1.3",
         "Shapely>=2.0.3",
         "tifffile>=2022.10.10",
         "timm>=0.9.2",
         "torch>=2.1.0",
         "torchgeo>=0.5.0",
         "torchmetrics>=1.2.0",
         "torchvision>=0.16.0",
-        "tqdm>=4.66.1"
+        "tqdm>=4.66.3"
       ],
       project_urls={
         "Bug Reports": "https://github.com/plantnet/malpolon/issues/new?assignees=aerodynamic-sauce-pan&labels=bug&projects=&template=bug_report.md&title=%5BBUG%5D",
         "Feature request": "https://github.com/plantnet/malpolon/issues/new?assignees=aerodynamic-sauce-pan&labels=enhancement&projects=&template=enhancement.md&title=%5BEnhancement%5D",
         "Host organizer": "https://plantnet.org/",
         "Source": "https://github.com/plantnet/malpolon",
     },
```

