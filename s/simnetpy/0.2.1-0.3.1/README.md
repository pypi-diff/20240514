# Comparing `tmp/simnetpy-0.2.1.tar.gz` & `tmp/simnetpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simnetpy-0.2.1.tar", last modified: Thu Nov  2 13:37:49 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `simnetpy-0.2.1.tar` & `simnetpy-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,32 @@
-drwxr-xr-x   0 amarnane  (1000) amarnane  (1000)        0 2023-11-02 13:37:49.374759 simnetpy-0.2.1/
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     1500 2023-07-10 15:55:26.000000 simnetpy-0.2.1/LICENSE
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     3281 2023-11-02 13:37:49.374759 simnetpy-0.2.1/PKG-INFO
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     2512 2023-11-02 13:36:25.000000 simnetpy-0.2.1/README.md
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     1274 2023-11-02 13:37:49.374759 simnetpy-0.2.1/setup.cfg
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)      158 2023-07-10 15:55:52.000000 simnetpy-0.2.1/setup.py
-drwxr-xr-x   0 amarnane  (1000) amarnane  (1000)        0 2023-11-02 13:37:49.354759 simnetpy-0.2.1/src/
-drwxr-xr-x   0 amarnane  (1000) amarnane  (1000)        0 2023-11-02 13:37:49.354759 simnetpy-0.2.1/src/simnet/
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)      601 2023-11-02 12:34:27.000000 simnetpy-0.2.1/src/simnet/__init__.py
-drwxr-xr-x   0 amarnane  (1000) amarnane  (1000)        0 2023-11-02 13:37:49.354759 simnetpy-0.2.1/src/simnet/clustering/
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)      549 2023-10-19 13:36:09.000000 simnetpy-0.2.1/src/simnet/clustering/__init__.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)    11063 2023-10-19 13:36:48.000000 simnetpy-0.2.1/src/simnet/clustering/clustering.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     8195 2023-10-19 13:36:09.000000 simnetpy-0.2.1/src/simnet/clustering/event_sampling.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     5936 2023-10-19 13:36:09.000000 simnetpy-0.2.1/src/simnet/clustering/quality.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     5490 2023-10-19 13:36:09.000000 simnetpy-0.2.1/src/simnet/clustering/spectral.py
-drwxr-xr-x   0 amarnane  (1000) amarnane  (1000)        0 2023-11-02 13:37:49.364759 simnetpy-0.2.1/src/simnet/datasets/
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)      470 2023-10-19 13:34:17.000000 simnetpy-0.2.1/src/simnet/datasets/__init__.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)    18456 2023-10-19 13:32:33.000000 simnetpy-0.2.1/src/simnet/datasets/generator.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     5416 2023-10-19 13:35:09.000000 simnetpy-0.2.1/src/simnet/datasets/multi_mod.py
-drwxr-xr-x   0 amarnane  (1000) amarnane  (1000)        0 2023-11-02 13:37:49.364759 simnetpy-0.2.1/src/simnet/graph/
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)      345 2023-10-19 13:26:07.000000 simnetpy-0.2.1/src/simnet/graph/__init__.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     9114 2023-11-02 12:25:23.000000 simnetpy-0.2.1/src/simnet/graph/igraphf.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     7106 2023-10-19 13:27:18.000000 simnetpy-0.2.1/src/simnet/graph/plotting.py
-drwxr-xr-x   0 amarnane  (1000) amarnane  (1000)        0 2023-11-02 13:37:49.374759 simnetpy-0.2.1/src/simnet/plotting/
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)      294 2023-11-02 12:33:27.000000 simnetpy-0.2.1/src/simnet/plotting/__init__.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     9504 2023-11-02 12:33:11.000000 simnetpy-0.2.1/src/simnet/plotting/graph_plot.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     5597 2023-11-02 12:29:55.000000 simnetpy-0.2.1/src/simnet/plotting/igraph_vis.py
-drwxr-xr-x   0 amarnane  (1000) amarnane  (1000)        0 2023-11-02 13:37:49.374759 simnetpy-0.2.1/src/simnet/similarity/
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)      464 2023-10-19 13:15:38.000000 simnetpy-0.2.1/src/simnet/similarity/__init__.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     4254 2023-10-19 13:15:38.000000 simnetpy-0.2.1/src/simnet/similarity/merging.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     6325 2023-10-19 13:20:56.000000 simnetpy-0.2.1/src/simnet/similarity/similarity.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     9096 2023-10-19 13:15:38.000000 simnetpy-0.2.1/src/simnet/similarity/threshold.py
-drwxr-xr-x   0 amarnane  (1000) amarnane  (1000)        0 2023-11-02 13:37:49.374759 simnetpy-0.2.1/src/simnet/utils/
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)      498 2023-10-19 13:38:55.000000 simnetpy-0.2.1/src/simnet/utils/__init__.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     5295 2023-10-19 13:37:28.000000 simnetpy-0.2.1/src/simnet/utils/filesys.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     6376 2023-10-19 13:38:26.000000 simnetpy-0.2.1/src/simnet/utils/plotting.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     2008 2023-10-19 13:37:56.000000 simnetpy-0.2.1/src/simnet/utils/sci_funcs.py
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)       67 2023-11-02 13:36:53.000000 simnetpy-0.2.1/src/simnet/version.py
-drwxr-xr-x   0 amarnane  (1000) amarnane  (1000)        0 2023-11-02 13:37:49.374759 simnetpy-0.2.1/src/simnetpy.egg-info/
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     3281 2023-11-02 13:37:49.000000 simnetpy-0.2.1/src/simnetpy.egg-info/PKG-INFO
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)     1010 2023-11-02 13:37:49.000000 simnetpy-0.2.1/src/simnetpy.egg-info/SOURCES.txt
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)        1 2023-11-02 13:37:49.000000 simnetpy-0.2.1/src/simnetpy.egg-info/dependency_links.txt
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)        1 2023-11-02 13:11:01.000000 simnetpy-0.2.1/src/simnetpy.egg-info/not-zip-safe
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)      122 2023-11-02 13:37:49.000000 simnetpy-0.2.1/src/simnetpy.egg-info/requires.txt
--rw-r--r--   0 amarnane  (1000) amarnane  (1000)        7 2023-11-02 13:37:49.000000 simnetpy-0.2.1/src/simnetpy.egg-info/top_level.txt
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 simnetpy-0.3.1/_version.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/version.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/clustering/__init__.py
+-rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/clustering/clustering.py
+-rw-r--r--   0        0        0     8195 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/clustering/event_sampling.py
+-rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/clustering/quality.py
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/clustering/spectral.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/datasets/__init__.py
+-rw-r--r--   0        0        0    17114 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/datasets/distributions.py
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/datasets/multi_mod.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/datasets/single_mod.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/graph/__init__.py
+-rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/graph/igraphf.py
+-rw-r--r--   0        0        0     8318 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/graph/plotting.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/plotting/__init__.py
+-rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/plotting/graph_plot.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/plotting/igraph_vis.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/similarity/__init__.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/similarity/merging.py
+-rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/similarity/similarity.py
+-rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/similarity/threshold.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/utils/__init__.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/utils/filesys.py
+-rw-r--r--   0        0        0     6376 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/utils/plotting.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 simnetpy-0.3.1/src/simnetpy/utils/sci_funcs.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 simnetpy-0.3.1/.gitignore
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 simnetpy-0.3.1/AUTHORS.md
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 simnetpy-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 simnetpy-0.3.1/README.md
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 simnetpy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 simnetpy-0.3.1/PKG-INFO
```

### Comparing `simnetpy-0.2.1/LICENSE` & `simnetpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simnetpy-0.2.1/PKG-INFO` & `simnetpy-0.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,41 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: simnetpy
-Version: 0.2.1
+Version: 0.3.1
 Summary: Python package for the Construction and Clustering of Similarity Networks
-Home-page: https://github.com/amarnane/simnetpy
-Download-URL: https://github.com/amarnane/simnetpy
-Author: Aidan Marnane
-Author-email: aidan.marnane@gmail.com
-License: BSD
-Keywords: similarity-network network-construction networks graphs clustering graph-clustering community-detection
+Project-URL: Download, https://github.com/amarnane/simnetpy
+Project-URL: Homepage, https://github.com/amarnane/simnetpy
+Project-URL: Documentation, https://amarnane.github.io/simnetpy/
+Author-email: Aidan Marnane <aidan.marnane@gmail.com>
+License-Expression: BSD-3-Clause
+License-File: AUTHORS.md
+License-File: LICENSE
+Keywords: clustering,community-detection,graph-clustering,graphs,network-construction,networks,similarity-network
 Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Requires-Dist: click
+Requires-Dist: igraph==0.10.4
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: palettable
+Requires-Dist: pandas
+Requires-Dist: pyyaml
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: seaborn
+Requires-Dist: snfpy
+Requires-Dist: spectralcluster
+Requires-Dist: tqdm
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: twine; extra == 'dev'
+Description-Content-Type: text/markdown
 
 # simnetpy
 
 Python Package for the creation and analysis of similarity networks.
 
 <!-- Project Organization
 --------------------
@@ -61,18 +76,14 @@
 ```
 
 ### Developer Mode
 To install in developer mode (have changes in source code update without reinstallation) add `-e` flag
 ```
 pip install -e .
 ```
-Note: removing the package is slightly more complicated and a different command is needed to uninstall 
-```
-python setup.py develop -u
-```
 
 ### Graph Tool
 There is one dependency that cannot be installed through pip - `Graph-Tool`. This is a result of it's underlying `c++` dependencies.
 The simplest method for python users is to make use of a conda environment, install this package using the commands above and install `graph-tool` using `conda-forge`
 ```
 conda install -c conda-forge graph-tool
 ```
```

### Comparing `simnetpy-0.2.1/README.md` & `simnetpy-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,14 @@
 ```
 
 ### Developer Mode
 To install in developer mode (have changes in source code update without reinstallation) add `-e` flag
 ```
 pip install -e .
 ```
-Note: removing the package is slightly more complicated and a different command is needed to uninstall 
-```
-python setup.py develop -u
-```
 
 ### Graph Tool
 There is one dependency that cannot be installed through pip - `Graph-Tool`. This is a result of it's underlying `c++` dependencies.
 The simplest method for python users is to make use of a conda environment, install this package using the commands above and install `graph-tool` using `conda-forge`
 ```
 conda install -c conda-forge graph-tool
 ```
```

### Comparing `simnetpy-0.2.1/src/simnet/clustering/__init__.py` & `simnetpy-0.3.1/src/simnetpy/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `simnetpy-0.2.1/src/simnet/clustering/clustering.py` & `simnetpy-0.3.1/src/simnetpy/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `simnetpy-0.2.1/src/simnet/clustering/event_sampling.py` & `simnetpy-0.3.1/src/simnetpy/clustering/event_sampling.py`

 * *Files identical despite different names*

### Comparing `simnetpy-0.2.1/src/simnet/clustering/quality.py` & `simnetpy-0.3.1/src/simnetpy/clustering/quality.py`

 * *Files identical despite different names*

### Comparing `simnetpy-0.2.1/src/simnet/clustering/spectral.py` & `simnetpy-0.3.1/src/simnetpy/clustering/spectral.py`

 * *Files identical despite different names*

### Comparing `simnetpy-0.2.1/src/simnet/datasets/generator.py` & `simnetpy-0.3.1/src/simnetpy/datasets/distributions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,278 +1,329 @@
 import numpy as np
-import matplotlib.pyplot as plt
-import sklearn.decomposition as decomp 
-import igraph as ig
-
-
-from sklearn.utils import Bunch
 from scipy import stats
+from sklearn.utils import Bunch
+
 
 def uniform_sampler(d, std=1, rng=None):
-    """sample random location in d dimensional box with 
+    """sample random location in d dimensional box with
     max value of std and min value -std on any axis
 
     Args:
         d (int): number of dimensions
         std (float, optional): max abs value on any axis. Defaults to 1.
-        rng (np.random.default_rng, optional): user seeded random number generator. Defaults to None. 
+        rng (np.random.default_rng, optional): user seeded random number generator. Defaults to None.
 
     Returns:
         np.ndarray: random point in d dimensional space with max abs value of std on any dimension
     """
     if rng is None:
         rng = np.random.default_rng()
-    
-    a = [1,-1]
+
+    a = [1, -1]
 
     direction = rng.choice(a, size=d)
     r = rng.uniform(0, std, size=d)
-    return direction*r
+    return direction * r
+
 
 def multivariate_guassian(N, center, std=1, rng=None):
-    """Sample N point from a multivariate guassian with mean at center and 
+    """Sample N point from a multivariate guassian with mean at center and
     Covariance of std*Identity (i.e. circular guassian). Dimensions of guassian inferred
     from user passed center.
 
     Args:
         N (int): number of points to sample
-        center (np.ndarray): d-dimensional point 
+        center (np.ndarray): d-dimensional point
         std (float, optional): Standard deviation along any axis. Covariance is `std`*Identity Matrix. Defaults to 1.
-        rng (np.random.default_rng, optional): user seeded random number generator. Defaults to None. 
+        rng (np.random.default_rng, optional): user seeded random number generator. Defaults to None.
 
     Returns:
         np.ndarray: N samples from multi-dimensional guassian centered at `center`. (N x d) matrix
     """
     if rng is None:
         rng = np.random.default_rng()
-    
-    if not isinstance(std,np.ndarray):
+
+    if not isinstance(std, np.ndarray):
         d = center.shape[0]
-        COV = std*np.eye(d)
+        COV = std * np.eye(d)
     else:
         COV = std
 
     X = rng.multivariate_normal(center, COV, size=N)
     return X
 
+
 def multivariate_t(N, center, std=1, df=1, rng=None):
-    """Sample N point from a multivariate guassian with mean at center and 
+    """Sample N point from a multivariate guassian with mean at center and
     Covariance of std*Identity (i.e. circular guassian). Dimensions of guassian inferred
     from user passed center.
 
     Args:
         N (int): number of points to sample
-        center (np.ndarray): d-dimensional point 
+        center (np.ndarray): d-dimensional point
         std (float, optional): Standard deviation along any axis. Covariance is `std`*Identity Matrix. Defaults to 1.
                                 Also accepts numpy covariance matrix
         df (float, optional): Degrees of freedom of the distribution. Defaults to 1. If np.inf results are multivariate normal.
-        rng (np.random.default_rng, optional): user seeded random number generator. Defaults to None. 
+        rng (np.random.default_rng, optional): user seeded random number generator. Defaults to None.
 
     Returns:
         np.ndarray: N samples from multi-dimensional guassian centered at `center`. (N x d) matrix
     """
     if rng is None:
         rng = np.random.default_rng()
-    
-    if not isinstance(std,np.ndarray):
+
+    if not isinstance(std, np.ndarray):
         d = center.shape[0]
-        COV = std*np.eye(d)
+        COV = std * np.eye(d)
     else:
         COV = std
 
     # X = rng.multivariate_normal(center, COV, size=N)
     # dist = stats.multivariate_t(center, shape=COV, df=df, seed=rng)
     # X = dist.rvs(size=size)
     X = stats.multivariate_t.rvs(loc=center, shape=COV, df=df, size=N, random_state=rng)
-    
+
     return X
 
+
 def cluster_centers(n, d, lower=1, higher=2, rng=None, init=None):
-    """Sample n point in d-dimensional space. Points will be between 
+    """Sample n point in d-dimensional space. Points will be between
     (lower, ~2*higher) distance from all other points. Initial center will be (0,0, ..,0)
-    unless otherwise specified. Sampling done sequentially with next center proposed, 
+    unless otherwise specified. Sampling done sequentially with next center proposed,
     rejected if too close to all others and resampled until accepted.
     If sampling large number of points & time taken is large increase size of higher.
 
-    Note: 2*higher is not actual distance upper bound. higher controls size of box around previous center 
-    that we sample a proposal point. Each center sampled from box with sides of size 2*higher. 
+    Note: 2*higher is not actual distance upper bound. higher controls size of box around previous center
+    that we sample a proposal point. Each center sampled from box with sides of size 2*higher.
     Args:
         n (int): number of points to generate
         d (int): number of dimensions
-        lower (float, optional): Lower bound of distances to accept. All points will be 
+        lower (float, optional): Lower bound of distances to accept. All points will be
                             at least lower away from each other. Defaults to 1.
         higher (float, optional): Size of box around previous center to sample from. Defaults to 2.
-        rng (np.random.default_rng, optional): user seeded random number generator. Defaults to None. 
-        init (np.ndarray, optional): Location of first sample. Defaults to None. Note points are shuffled 
+        rng (np.random.default_rng, optional): user seeded random number generator. Defaults to None.
+        init (np.ndarray, optional): Location of first sample. Defaults to None. Note points are shuffled
         but if none at least one will be the origin (0,0,...,0).
 
     Returns:
         list: n randomly sampled points in d-dimensional space all at least lower away from each other.
     """
     if rng is None:
         rng = np.random.default_rng()
 
     if init is None:
         init = np.zeros(d)
-    centers=[]
+    centers = []
     x = init + uniform_sampler(d, std=higher, rng=rng)
     centers.append(x)
 
     while len(centers) < n:
         # sample point in random direction
         x = uniform_sampler(d, std=higher, rng=rng)
-        
+
         # find random center and move away in direction x
         i = rng.integers(0, len(centers))
         x = centers[i] + x
 
-        carray = np.array(centers)    
+        carray = np.array(centers)
         dist = np.linalg.norm(carray - x, axis=1, ord=2)
 
-        if np.all(dist>lower):
+        if np.all(dist > lower):
             centers.append(x)
-    rng.shuffle(centers) # shuffle so first cluster is not necessarily close to init
+    rng.shuffle(centers)  # shuffle so first cluster is not necessarily close to init
     return centers
 
 
-def mixed_multi_guassian(nclusters, d, N=100, std=1, lower=2, upper=5, sizes=None, distype=None, scale_ul_with_d=False, df=2, rng=None):
-    if isinstance(sizes,str):
-        assert sizes.lower() in ['equal', 'random', 'roughly_equal'], "if specifying method sizes must be one of [equal, random, roughly_equal]"
-        sizes = split_data_into_clusters(N,nclusters,method=sizes)
+def mixed_multi_numeric(
+    nclusters,
+    d,
+    N=100,
+    std=1,
+    lower=2,
+    upper=5,
+    sizes=None,
+    distype=None,
+    scale_ul_with_d=False,
+    df=2,
+    rng=None,
+):
+    if isinstance(sizes, str):
+        assert sizes.lower() in [
+            "equal",
+            "random",
+            "roughly_equal",
+        ], "if specifying method sizes must be one of [equal, random, roughly_equal]"
+        sizes = split_data_into_clusters(N, nclusters, method=sizes)
     elif sizes is None:
-        sizes = split_data_into_clusters(N,nclusters,method='equal')
-        
+        sizes = split_data_into_clusters(N, nclusters, method="equal")
+
     if scale_ul_with_d:
-        lower = lower/np.sqrt(d)
-        upper = upper/np.sqrt(d)
+        lower = lower / np.sqrt(d)
+        upper = upper / np.sqrt(d)
 
     centers = cluster_centers(n=nclusters, d=d, lower=lower, higher=upper, rng=rng)
 
     X = []
     y = []
-    for i,(cc, m) in enumerate(zip(centers, sizes)):
-        if distype == 'studentt':
-            x = multivariate_t(m, cc, std=std, df=df, rng=rng)    
+    for i, (cc, m) in enumerate(zip(centers, sizes)):
+        if distype == "studentt":
+            x = multivariate_t(m, cc, std=std, df=df, rng=rng)
         else:
             x = multivariate_guassian(m, cc, std=std, rng=rng)
         X.append(x)
 
-        labels = [i]*m
+        labels = [i] * m
         y += labels
 
     return Bunch(y=np.array(y), X=np.vstack(X))
-    # return 
-
-def polygenerator(degree, upperb, rng=None):
-    if rng is None:
-        rng = np.random.default_rng()
 
-    coef = rng.uniform(low=-upperb, high=upperb, size=degree+1)
-    polyt = np.poly1d(coef)
-    return polyt
-
-    
-def polytransform(X, degree, upperb, rng=None, norm=False):
-    polyt = polygenerator(degree, upperb, rng)
-
-    X = polyt(X)
-    if norm:
-        X = (X - X.mean(axis=0))/X.std(axis=0)
-    return X
 
-def multi_modal_guassian(nmodality=3, nclusters=3, N=50, d=10, std=1, sizes=None, rng=None, normalise=True):
+# def polygenerator(degree, upperb, rng=None):
+#     if rng is None:
+#         rng = np.random.default_rng()
+
+#     coef = rng.uniform(low=-upperb, high=upperb, size=degree + 1)
+#     polyt = np.poly1d(coef)
+#     return polyt
+
+
+# def polytransform(X, degree, upperb, rng=None, norm=False):
+#     polyt = polygenerator(degree, upperb, rng)
+
+#     X = polyt(X)
+#     if norm:
+#         X = (X - X.mean(axis=0)) / X.std(axis=0)
+#     return X
+
+
+# def multi_modal_guassian(
+#     nmodality=3, nclusters=3, N=50, d=10, std=1, sizes=None, rng=None, normalise=True
+# ):
+#     if rng is None:
+#         rng = np.random.default_rng()
+
+#     if isinstance(sizes, str):
+#         assert sizes.lower() in [
+#             "equal",
+#             "random",
+#             "roughly_equal",
+#         ], "if specifying method sizes must be one of [equal, random, roughly_equal]"
+#         sizes = split_data_into_clusters(N, nclusters, method=sizes)
+#     elif sizes is None:
+#         sizes = split_data_into_clusters(N, nclusters, method="equal")
+
+#     # std = 1
+#     lower = 3 / np.sqrt(
+#         d
+#     )  # this value found to work nicely between 2-10 dimensions. completely arbitrary.
+#     upper = 7 / np.sqrt(d)  # similar to above.
+
+#     data = {}
+
+#     for i in range(nmodality):
+#         dataset = mixed_multi_guassian(
+#             nclusters, d, N=N, std=std, lower=lower, upper=upper, sizes=sizes, rng=rng
+#         )
+#         X = dataset.X
+#         y = dataset.y
+
+#         if normalise:
+#             X = (X - X.mean(axis=0)) / X.std(axis=0)
+
+#         data[f"X{i}"] = X
+#     # data['y'] = y
+
+#     return Bunch(data=data, y=y)
+
+
+# def multi_modal_data(
+#     nmodality=3,
+#     nclusters=3,
+#     N=300,
+#     d=10,
+#     std=1,
+#     rng=None,
+#     nonlinear=True,
+#     max_degree=8,
+#     coef_max_abs=2,
+#     norm=True,
+# ):
+
+#     dataset = multi_modal_guassian(nmodality, nclusters, N, d, std, rng)
+
+#     if nonlinear:
+#         y = dataset.y
+#         data = {}
+#         for k, X in dataset.data.items():
+#             degree = rng.integers(2, max_degree + 1)
+#             # print(degree)
+#             Xt = polytransform(X, degree, coef_max_abs, rng, norm=norm)
+#             data[k] = Xt
+
+#     return Bunch(data=data, y=y)
+
+
+############################# Categorial ###############################################
+
+
+def random_discrete_pmf(
+    nlevels=5,
+    min_largest_cat=0,
+    max_any_cat=None,
+    min_each_cat=0,
+    shuffle=True,
+    rng=None,
+):
     if rng is None:
         rng = np.random.default_rng()
 
-    if isinstance(sizes,str):
-        assert sizes.lower() in ['equal', 'random', 'roughly_equal'], "if specifying method sizes must be one of [equal, random, roughly_equal]"
-        sizes = split_data_into_clusters(N, nclusters, method=sizes)
-    elif sizes is None:
-        sizes = split_data_into_clusters(N, nclusters, method='equal')
-
-    # std = 1
-    lower = 3/np.sqrt(d) # this value found to work nicely between 2-10 dimensions. completely arbitrary. 
-    upper = 7/np.sqrt(d) # similar to above. 
-    
-    data = {}
-    
-    for i in range(nmodality):
-        dataset = mixed_multi_guassian(nclusters, d, N=N, std=std, lower=lower, upper=upper, sizes=sizes, rng=rng)
-        X = dataset.X
-        y = dataset.y
-
-        if normalise:
-            X = (X-X.mean(axis=0))/X.std(axis=0)
-
-        data[f'X{i}'] = X
-    # data['y'] = y
-
-    return Bunch(data=data, y=y)
-
-def multi_modal_data(nmodality=3, nclusters=3, N=300, d=10, std=1, rng=None, nonlinear=True, max_degree=8, coef_max_abs=2, norm=True):
-
-    dataset = multi_modal_guassian(nmodality, nclusters, N, d, std, rng)
-
-    if nonlinear:
-        y = dataset.y
-        data = {}
-        for k, X in dataset.data.items():
-            degree = rng.integers(2, max_degree+1)
-            # print(degree)
-            Xt = polytransform(X, degree, coef_max_abs, rng, norm=norm)
-            data[k] = Xt    
-
-    return Bunch(data=data, y=y)
-
-
-
-
-################################################################################
-
+    assert (
+        min_each_cat * nlevels < 1
+    ), f"error guaranteeing each cat has minimum {min_each_cat} prob mass results in sum(prob mass) > 1"
 
-
-
-
-def random_discrete_pmf(nlevels=5, min_largest_cat=0, max_any_cat=None, min_each_cat=0, shuffle=True, rng=None):
-    if rng is None:
-        rng = np.random.default_rng()
-
-    assert min_each_cat*nlevels < 1, f"error guaranteeing each cat has minimum {min_each_cat} prob mass results in sum(prob mass) > 1"
-    
-    total = 1 - min_each_cat*nlevels # total probability mass to distribute
+    total = 1 - min_each_cat * nlevels  # total probability mass to distribute
 
     if max_any_cat is None:
         max_any_cat = total
 
-    assert max_any_cat <= total and max_any_cat >= 1/nlevels, f"max_any_cat must be float between 1/nlevels and {total}."
-    assert min_largest_cat <= total and min_largest_cat >= 0, f"min_largest_cat must be float between 0 and {total}"
-    assert max_any_cat >= min_largest_cat, "allowable upper bound for any category must be larger than minimum value for largest"
+    assert (
+        max_any_cat <= total and max_any_cat >= 1 / nlevels
+    ), f"max_any_cat must be float between 1/nlevels and {total}."
+    assert (
+        min_largest_cat <= total and min_largest_cat >= 0
+    ), f"min_largest_cat must be float between 0 and {total}"
+    assert (
+        max_any_cat >= min_largest_cat
+    ), "allowable upper bound for any category must be larger than minimum value for largest"
 
     p = np.zeros(nlevels)
     # total = 1 # total probability mass to distribute
 
-    upper = max_any_cat # max in 
-    for i in range(nlevels-1):
+    upper = max_any_cat  # max in
+    for i in range(nlevels - 1):
         if not i:
-            lower = min_largest_cat  # if we want to skew the distribution we set a value 
-                                    # above 0.5 to that at prob of first element is > 0.5
+            lower = (
+                min_largest_cat  # if we want to skew the distribution we set a value
+            )
+            # above 0.5 to that at prob of first element is > 0.5
         else:
             lower = 0  # for all other elements we want to equally distriute the remaining prob mass
-        
-        if total < max_any_cat: # when remaining probability mass less than upper bound 
-            upper=total
-        
- 
+
+        if total < max_any_cat:  # when remaining probability mass less than upper bound
+            upper = total
+
         # when limiting maximum of any category with max_any_cat
         # the lower bound needs to be adjusted in case a sequence of too small values are sampled.
         # otherwise final value p_{n-1} will be greater than max_any_cat
         # lower is the minimum value possible assuming the remaining categories are assigned the max_any_cat value.
-        lower = total - (max_any_cat*(nlevels-i-1)) # i is number of categories sampled. nlevels -i -1 = number of categories remaining -1
+        lower = total - (
+            max_any_cat * (nlevels - i - 1)
+        )  # i is number of categories sampled. nlevels -i -1 = number of categories remaining -1
         lower = max(lower, 0)
-        
+
         x = rng.uniform(low=lower, high=upper, size=1)
         total = total - x
         p[i] = x
 
     # xn = 1 - sum(p)
     p[-1] = total
 
@@ -289,219 +340,205 @@
     # note could also change starting average cluster size
     # if [N*frac]*nclusters Then max_margin is max_margin=1/(ncluster-1) - frac
     # as e.g. if frac=1/(N+1) then immediate increase in possible margin sizes that can be used
     # note: assert frac < 1/ncluster otherwise total is too large
     if rng is None:
         rng = np.random.default_rng()
 
-    
-    max_margin = 1/(nclusters-1) - 1/nclusters
+    max_margin = 1 / (nclusters - 1) - 1 / nclusters
     if margin is None:
-        margin=max_margin
+        margin = max_margin
     assert margin <= max_margin, f"margin must be less than max possible: {max_margin}"
-    
-    shift = rng.uniform(-margin, margin, nclusters-1)
-    if np.all(shift==max_margin): # in very unlikely event that all are max_margin resample
-        shift = rng.uniform(-margin, margin, nclusters-1)
-
-    shift = np.round(shift*N)
-
-    equal = [N//nclusters]*nclusters
-    sizes = np.zeros(nclusters, dtype='int')
-    for i,size in enumerate(equal[:-1]):
+
+    shift = rng.uniform(-margin, margin, nclusters - 1)
+    if np.all(
+        shift == max_margin
+    ):  # in very unlikely event that all are max_margin resample
+        shift = rng.uniform(-margin, margin, nclusters - 1)
+
+    shift = np.round(shift * N)
+
+    equal = [N // nclusters] * nclusters
+    sizes = np.zeros(nclusters, dtype="int")
+    for i, size in enumerate(equal[:-1]):
         sizes[i] = size + shift[i]
     sizes[-1] = N - sizes[:-1].sum()
 
     return sizes
 
-def random_split(N, nclusters, max_any_cat=0.6, min_each_cat=0, min_largest_cat=0, shuffle=True, rng=None):
-    
-    sizes = random_discrete_pmf(nlevels=nclusters, max_any_cat=max_any_cat,min_largest_cat=min_largest_cat,
-                                 min_each_cat=min_each_cat, shuffle=shuffle, rng=rng)
-    sizes = np.round(N*sizes).astype('int')
+
+def random_split(
+    N,
+    nclusters,
+    max_any_cat=0.6,
+    min_each_cat=0,
+    min_largest_cat=0,
+    shuffle=True,
+    rng=None,
+):
+
+    sizes = random_discrete_pmf(
+        nlevels=nclusters,
+        max_any_cat=max_any_cat,
+        min_largest_cat=min_largest_cat,
+        min_each_cat=min_each_cat,
+        shuffle=shuffle,
+        rng=rng,
+    )
+    sizes = np.round(N * sizes).astype("int")
     # resample if empty
-    if np.any(sizes==0):
-        sizes = random_split(N,nclusters, max_any_cat=max_any_cat)
-    
+    if np.any(sizes == 0):
+        sizes = random_split(N, nclusters, max_any_cat=max_any_cat)
+
     # check for rounding errors
     rounderror = N - sizes.sum()
 
     for i in range(np.abs(rounderror)):
         if rounderror > 0:
-            sizes[i] +=1
+            sizes[i] += 1
         elif rounderror < 0:
-            sizes[i] -=1    
+            sizes[i] -= 1
     return sizes
 
+
 def equal_split(N, nclusters):
-    sizes = [N//nclusters]*nclusters # split equally
+    sizes = [N // nclusters] * nclusters  # split equally
     rounderror = N - sum(sizes)
     for i in range(rounderror):
-        sizes[i] +=1
+        sizes[i] += 1
     return np.array(sizes)
 
-def split_data_into_clusters(N,nclusters, method='equal', random_kwds={}, requal_kwds={}):
-    assert method in ['equal', 'random', 'roughly_equal'], 'Must be one of equal, random, roughly equal'
 
-    if method=='equal':
-        sizes = equal_split(N,nclusters)
-    elif method=='random':
-        sizes = random_split(N,nclusters, **random_kwds)
+def split_data_into_clusters(
+    N, nclusters, method="equal", random_kwds={}, requal_kwds={}
+):
+    assert method in [
+        "equal",
+        "random",
+        "roughly_equal",
+    ], "Must be one of equal, random, roughly equal"
+
+    if method == "equal":
+        sizes = equal_split(N, nclusters)
+    elif method == "random":
+        sizes = random_split(N, nclusters, **random_kwds)
     else:
-        sizes=roughly_equal_split(N,nclusters, **requal_kwds)
+        sizes = roughly_equal_split(N, nclusters, **requal_kwds)
     return np.array(sizes)
 
-def single_categorical_feature(N, nlevels, min_largest_cat=0.8, max_any_cat=1,shuffle=True, rng=None):
+
+def single_categorical_feature(
+    N, nlevels, min_largest_cat=0.8, max_any_cat=1, shuffle=True, rng=None
+):
     if rng is None:
-        rng=np.random.default_rng()
-    p = random_discrete_pmf(nlevels, min_largest_cat=min_largest_cat,
-                                max_any_cat=max_any_cat, shuffle=shuffle, rng=rng)
+        rng = np.random.default_rng()
+    p = random_discrete_pmf(
+        nlevels,
+        min_largest_cat=min_largest_cat,
+        max_any_cat=max_any_cat,
+        shuffle=shuffle,
+        rng=rng,
+    )
     x = rng.choice(nlevels, size=N, p=p)
     return x
 
-def mixed_categorical_cluster_feature(sizes, nlevels,min_largest_cat=0.8, max_any_cat=1,shuffle=True, rng=None):
+
+def mixed_categorical_cluster_feature(
+    sizes, nlevels, min_largest_cat=0.8, max_any_cat=1, shuffle=True, rng=None
+):
     if rng is None:
-        rng=np.random.default_rng()
+        rng = np.random.default_rng()
     # nlevels = 5
     X = []
     for size in sizes:
-        x = single_categorical_feature(size, nlevels=nlevels, min_largest_cat=min_largest_cat,
-                                max_any_cat=max_any_cat, shuffle=shuffle, rng=rng)
+        x = single_categorical_feature(
+            size,
+            nlevels=nlevels,
+            min_largest_cat=min_largest_cat,
+            max_any_cat=max_any_cat,
+            shuffle=shuffle,
+            rng=rng,
+        )
         # p = random_discrete_pmf(nlevels, min_largest_cat=min_largest_cat,
         #                         max_any_cat=max_any_cat, shuffle=shuffle, rng=rng)
         # # print(p.argmax(), p.max())
         # x = rng.choice(nlevels, size=size, p=p)
         X.append(x)
     return np.hstack(X)
-    
 
-def mixed_categorical_clusters(N, d, nclusters=3, sizes='equal', alpha=5, beta=1, nlevels=5, return_skew_factors=True, rng=None):
-    """ alpha and beta control shape of skew factor distribution
-    higher max(abs(a,b))>1 -> less flat more peaked distribution 
+
+def mixed_categorical_clusters(
+    N,
+    d,
+    nclusters=3,
+    sizes="equal",
+    alpha=5,
+    beta=1,
+    nlevels=5,
+    return_skew_factors=True,
+    rng=None,
+):
+    """alpha and beta control shape of skew factor distribution
+    higher max(abs(a,b))>1 -> less flat more peaked distribution
     a<b -> skewed below 0.5
     a>b -> skewed above 0.5
     so 5,1 means on average skew passed to ordinal feature generator will be centered on a/a+b~0.83
     and 1,5 means average skew will be ~0.16
     lower average skew means noisier data and harder clustering problem
-    
-    
+
     """
 
     if rng is None:
         rng = np.random.default_rng()
 
-    if isinstance(sizes,str):
-        assert sizes.lower() in ['equal', 'random', 'roughly_equal'], "if specifying method sizes must be one of [equal, random, roughly_equal]"
-        sizes = split_data_into_clusters(N,nclusters,method=sizes)
+    if isinstance(sizes, str):
+        assert sizes.lower() in [
+            "equal",
+            "random",
+            "roughly_equal",
+        ], "if specifying method sizes must be one of [equal, random, roughly_equal]"
+        sizes = split_data_into_clusters(N, nclusters, method=sizes)
     elif sizes is None:
-        sizes = split_data_into_clusters(N,nclusters,method='equal')
+        sizes = split_data_into_clusters(N, nclusters, method="equal")
 
     assert sizes.shape[0] == nclusters, "nclusters and sizes must match"
     assert sizes.sum() == N, f"sizes must add up to N {sizes.sum()} != {N}"
 
     # N = sizes.sum()
 
     # generate skew distribution & sample
-    rv = stats.beta(a=alpha,b=beta)
-    skew_factors = rv.rvs(size=d,random_state=rng)
-    
+    rv = stats.beta(a=alpha, b=beta)
+    skew_factors = rv.rvs(size=d, random_state=rng)
+
     # generate features
-    X = np.zeros((N,d))
+    X = np.zeros((N, d))
     for i in range(d):
         si = skew_factors[i]
-        if si >= 0.5 and si <=1:
-            skew = 2*((nlevels-1)/nlevels)*si + (2-nlevels)/nlevels # map skew factor from [0.5, 1] to [1/nlevels, 1] i.e. si=0.5, skew=1/nlevels
-            X[:,i] = mixed_categorical_cluster_feature(sizes, nlevels=nlevels, min_largest_cat=skew, rng=rng)
-        elif si >=0 and si < 0.5:
-            skew = 2*((1-nlevels)/nlevels)*si + 1 # map skew factor from [0.5, 0] to [1/nlevels, 1] i.e si=0 -> skew = 1.0
-            X[:,i] = single_categorical_feature(N, nlevels=nlevels, min_largest_cat=skew, rng=rng)
+        if si >= 0.5 and si <= 1:
+            skew = (
+                2 * ((nlevels - 1) / nlevels) * si + (2 - nlevels) / nlevels
+            )  # map skew factor from [0.5, 1] to [1/nlevels, 1] i.e. si=0.5, skew=1/nlevels
+            X[:, i] = mixed_categorical_cluster_feature(
+                sizes, nlevels=nlevels, min_largest_cat=skew, rng=rng
+            )
+        elif si >= 0 and si < 0.5:
+            skew = (
+                2 * ((1 - nlevels) / nlevels) * si + 1
+            )  # map skew factor from [0.5, 0] to [1/nlevels, 1] i.e si=0 -> skew = 1.0
+            X[:, i] = single_categorical_feature(
+                N, nlevels=nlevels, min_largest_cat=skew, rng=rng
+            )
         else:
             raise ValueError("Error beta distribution ill defined")
 
-    # generate labels        
+    # generate labels
     y = np.zeros(N)
     total = 0
     for i, size in enumerate(sizes):
-        y[total:total+size] = i
-        total +=size
-        
+        y[total : total + size] = i
+        total += size
+
     dataset = Bunch(y=y, X=X)
     if return_skew_factors:
-        dataset['skew_factors'] = skew_factors
+        dataset["skew_factors"] = skew_factors
 
     return dataset
-
-
-def cluster_plot(X, y=None, ax = None, PCA=True, print_variance=False, alpha=0.2, marker='o', linestyle='None', **kwds):
-    if y is None:
-        y = np.ones(X.shape[0])
-
-    if PCA:
-        pca = decomp.PCA(n_components=2)
-        Z = pca.fit_transform(X)
-        if print_variance:
-            print(pca.explained_variance_ratio_)
-    else:
-        Z = X[:,:2]
-
-    # create new figure if user ax not provided
-    if ax is None:
-        fig, ax = plt.subplots(dpi=100)
-    else:
-        fig = None
-    # ax.scatter(Z[:,0], Z[:,1], c=y, marker=marker, alpha=alpha, **kwds)
-    for i, c in enumerate(np.unique(y)):
-        idx = y==c
-        ax.plot(Z[idx,0], Z[idx,1], marker=marker, linestyle=linestyle, alpha=alpha, **kwds)
-
-    return fig, ax
-
-def network_plot(g, X, y, markersize=3, style_dict=None, PCA=False, ax=None, **scatterkwds):
-     # create new figure if user ax not provided
-    if ax is None:
-        fig, ax = plt.subplots(dpi=100)
-    else:
-        fig = None
-        
-    if PCA:
-        pca = decomp.PCA(n_components=2)
-        Z = pca.fit_transform(X)
-    else:
-        Z = X[:,:2]
-
-    dd = np.array(g.degree())+1 # +1 to ensure isolated nodes appear on plot
-    dd = dd/dd.max()
-    dd = (dd**2)*(markersize**2)
-
-    nclstr = len(np.unique(y))
-    for i, c in enumerate(np.unique(y)):
-        idx = y==c
-        ax.scatter(x=Z[idx,0], y=Z[idx,1], c=f'C{i}', s=dd[idx], zorder=10, **scatterkwds)
-
-    if style_dict is None:
-        style_dict = {
-            "edge_width": 0.5,
-            "edge_color": 'lightgrey',
-        }
-
-    if isinstance(Z, np.ndarray):
-        coords=Z.tolist()
-    else:
-        coords = Z
-    layout = ig.Layout(coords=coords)
-    style_dict['layout'] = layout
-    # edge_width=0.5, edge_color='lightgrey'
-    # visual_style = {
-    #     "edge_width": edge_width,
-    #     "edge_color": edge_color,
-    #     "layout": layout,
-    #     **igstylekwds,
-    # }
-    
-
-    ig.plot(g.plottable(), target=ax, **style_dict)
-    ax.set_aspect('auto')
-    N = g.vcount()
-    [vertex.remove() for vertex in ax.get_children()[nclstr:N+nclstr]]
-
-    return fig, ax
-
```

### Comparing `simnetpy-0.2.1/src/simnet/graph/igraphf.py` & `simnetpy-0.3.1/src/simnetpy/graph/igraphf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,206 +1,211 @@
-import time
-import pandas as pd
+import igraph as ig
 import numpy as np
+import pandas as pd
 import scipy.sparse as sp
-import igraph as ig
+
 from ..plotting import plot_degree_dist
-# from ..clustering import run_cluster_method
 
+# from ..clustering import run_cluster_method
 
 
 def convert_adj_2_igraph(A):
     A = sp.triu(A).tocoo()
     E = np.vstack((A.row, A.col)).T
-    E=list(map(tuple, E))
+    E = list(map(tuple, E))
 
     # X = {var: row for var, row in enumerate(g.x.T)}
     return ig.Graph(E)
 
+
 def find_second_cc(cc):
     # cc = np.array(g2.clusters().membership)
     C = np.vstack(np.unique(cc, return_counts=True))
-    assert C[1, :].max() == C[1,0], "LCC is not 0th component"
-    cc2 = C[:,(C[1, :] > 1) & (C[1,:] < C[1,0])] # find values lower than max but greater than 1 (might be empty?)
-    return tuple(cc2[:,cc2[1,:].argmax()]) # returns index and size
+    assert C[1, :].max() == C[1, 0], "LCC is not 0th component"
+    cc2 = C[
+        :, (C[1, :] > 1) & (C[1, :] < C[1, 0])
+    ]  # find values lower than max but greater than 1 (might be empty?)
+    return tuple(cc2[:, cc2[1, :].argmax()])  # returns index and size
+
 
 def find_first_second_largest_cc(cc):
     C = np.vstack(np.unique(cc, return_counts=True))
-    cmax = C[:,C[1,:].argmax()]
-    cc2 = C[:,(C[1, :] > 1) & (C[1,:] < cmax[1])] # find values lower than max but greater than 1 (might be empty?)
+    cmax = C[:, C[1, :].argmax()]
+    cc2 = C[
+        :, (C[1, :] > 1) & (C[1, :] < cmax[1])
+    ]  # find values lower than max but greater than 1 (might be empty?)
     try:
-        cc2 = cc2[:,cc2[1,:].argmax()]
+        cc2 = cc2[:, cc2[1, :].argmax()]
     except ValueError:
-        return cmax[0], None # if no second component return None.
+        return cmax[0], None  # if no second component return None.
+
+    return cmax[0], cc2[0]  # returns index for largest and 2nd largest components
 
-    return cmax[0], cc2[0] # returns index for largest and 2nd largest components
 
 def graph_stats(gg):
     ddict = {}
-    ddict['density'] = gg.density()
-    ddict['n'] = gg.vcount()
-    ddict['E'] = gg.ecount()
-    ddict['diameter'] = gg.diameter()
-    ddict['globalcc'] = gg.transitivity_undirected(mode='zero')
-    ddict['avglocalcc'] = gg.transitivity_avglocal_undirected(mode='zero')
-    ddict['assortivity'] = gg.assortativity_degree(directed=False)
-    ddict['avg_path_length'] = gg.average_path_length(directed=False)
+    ddict["density"] = gg.density()
+    ddict["n"] = gg.vcount()
+    ddict["E"] = gg.ecount()
+    ddict["diameter"] = gg.diameter()
+    ddict["globalcc"] = gg.transitivity_undirected(mode="zero")
+    ddict["avglocalcc"] = gg.transitivity_avglocal_undirected(mode="zero")
+    ddict["assortivity"] = gg.assortativity_degree(directed=False)
+    ddict["avg_path_length"] = gg.average_path_length(directed=False)
     dd = np.array(gg.degree())
-    ddict['avg_degree'] = dd.mean()
-    ddict['median_degree'] = np.median(dd)
-    ddict['max_degree'] = dd.max()
-
+    ddict["avg_degree"] = dd.mean()
+    ddict["median_degree"] = np.median(dd)
+    ddict["max_degree"] = dd.max()
 
     return ddict
 
+
 def component_info(gg):
     ddict = {}
-    ddict['E'] = gg.ecount()
-    
+    ddict["E"] = gg.ecount()
+
     cc = gg.clusters()
-    ddict['Nc'] = len(cc)
+    ddict["Nc"] = len(cc)
 
     idxmax, idx2 = find_first_second_largest_cc(cc.membership)
 
     gc = cc.subgraph(idx=idxmax)
-    ddict['cc_max'] = graph_stats(gc)
-    
+    ddict["cc_max"] = graph_stats(gc)
+
     ccmem = np.array(cc.membership)
-    ddict['cc_max_mem'] = (ccmem==idxmax)
+    ddict["cc_max_mem"] = ccmem == idxmax
 
     if idx2 is not None:
         gc2 = cc.subgraph(idx=idx2)
-        ddict['cc2'] = graph_stats(gc2)
+        ddict["cc2"] = graph_stats(gc2)
     else:
-        ddict['cc2'] = None
+        ddict["cc2"] = None
     return ddict
 
 
 def compare_clusters(c1, c2):
     ddict = {}
-    for metric in ['vi', 'nmi', 'split-join', 'rand', 'adjusted_rand']:
+    for metric in ["vi", "nmi", "split-join", "rand", "adjusted_rand"]:
         try:
             dist = ig.compare_communities(c1, c2, method=metric)
         except:
             dist = np.nan
         ddict[metric] = dist
     return ddict
-    
+
+
 def cluster_comparison(clist):
     ddict = {}
     for i, c1 in enumerate(clist):
-        for j, c2 in enumerate(clist[i+1:],i+1):
+        for j, c2 in enumerate(clist[i + 1 :], i + 1):
             # print(i,j)
-            ddict[(i,j)] = compare_clusters(c1, c2)
+            ddict[(i, j)] = compare_clusters(c1, c2)
     return ddict
 
 
-
 def ig_graphinfo(gg, community_funcs=None):
     ddict = {}
-    component_stats = component_info(gg)    
-    ddict['component_stats'] = component_stats
+    component_stats = component_info(gg)
+    ddict["component_stats"] = component_stats
 
-    ccmax = list(np.array(gg.vs.indices)[component_stats['cc_max_mem']])
+    ccmax = list(np.array(gg.vs.indices)[component_stats["cc_max_mem"]])
     gc = gg.induced_subgraph(ccmax)
 
     # communities = run_communities(gc, community_funcs=community_funcs)
     # ddict['community_stats'] = communities
 
-    clist = [ddict['clustering'] for k, ddict in communities.items()]
+    clist = [ddict["clustering"] for k, ddict in communities.items()]
     clustercomp = cluster_comparison(clist)
 
-    ddict['cluster_comp'] = clustercomp
+    ddict["cluster_comp"] = clustercomp
 
-    ddict['gg'] = gg
-    ddict['gc'] = gc
+    ddict["gg"] = gg
+    ddict["gc"] = gc
     return ddict
 
 
 def find_threshold_graph_stats(A):
     gg = convert_adj_2_igraph(A)
     stats = ig_graphinfo(gg)
     return stats
 
 
-
 class Igraph(ig.Graph):
-    def __init__(self, *args,**kwds):
-        X = kwds.pop('X', None) # check if X passed as argument
+    def __init__(self, *args, **kwds):
+        X = kwds.pop("X", None)  # check if X passed as argument
 
         if isinstance(X, pd.DataFrame):
-            X = X.to_dict(orient='list')
+            X = X.to_dict(orient="list")
 
-        super().__init__(*args,**kwds)
+        super().__init__(*args, **kwds)
 
     def graph_stats(self):
         ddict = {}
-        ddict['density'] = self.density()
-        ddict['n'] = self.vcount()
-        ddict['E'] = self.ecount()
+        ddict["density"] = self.density()
+        ddict["n"] = self.vcount()
+        ddict["E"] = self.ecount()
         C = self.component_sizes(pcent=False)
-        ddict['Nc'] = C.shape[1]
-        ddict['ncmax'] = C[1,0]
-        ddict['diameter'] = self.diameter()
-        ddict['globalcc'] = self.transitivity_undirected(mode='zero')
-        ddict['avglocalcc'] = self.transitivity_avglocal_undirected(mode='zero')
-        ddict['assortivity'] = self.assortativity_degree(directed=False)
-        ddict['avg_path_length'] = self.average_path_length(directed=False)
+        ddict["Nc"] = C.shape[1]
+        ddict["ncmax"] = C[1, 0]
+        ddict["diameter"] = self.diameter()
+        ddict["globalcc"] = self.transitivity_undirected(mode="zero")
+        ddict["avglocalcc"] = self.transitivity_avglocal_undirected(mode="zero")
+        ddict["assortativity"] = self.assortativity_degree(directed=False)
+        ddict["avg_path_length"] = self.average_path_length(directed=False)
         dd = np.array(self.degree())
-        ddict['avg_degree'] = dd.mean()
-        ddict['median_degree'] = np.median(dd)
-        ddict['max_degree'] = dd.max()
+        ddict["avg_degree"] = dd.mean()
+        ddict["median_degree"] = np.median(dd)
+        ddict["max_degree"] = dd.max()
 
         return ddict
 
-
     def component_stats(self):
         ddict = {}
-        ddict['E'] = self.ecount()
-        
+        ddict["E"] = self.ecount()
+
         cc = self.connected_components()
-        ddict['Nc'] = len(cc)
+        ddict["Nc"] = len(cc)
 
         idxmax, idx2 = self.find_first_second_largest_cc(cc.membership)
 
         gc = cc.subgraph(idx=idxmax)
         gc = self.from_igraph(gc)
-        ddict['cc_max'] = gc.graph_stats()
-        
+        ddict["cc_max"] = gc.graph_stats()
+
         ccmem = np.array(cc.membership)
-        ddict['cc_max_mem'] = (ccmem==idxmax)
+        ddict["cc_max_mem"] = ccmem == idxmax
 
         if idx2 is not None:
             gc2 = cc.subgraph(idx=idx2)
             gc2 = self.from_igraph(gc2)
-            ddict['cc2'] = gc2.graph_stats()
+            ddict["cc2"] = gc2.graph_stats()
         else:
-            ddict['cc2'] = None
+            ddict["cc2"] = None
         return ddict
-    
+
     def component_sizes(self, cc=None, pcent=True):
         if cc is None:
             cc = self.connected_components()
 
         C = np.vstack(np.unique(cc.membership, return_counts=True))
-        C = C[:,np.argsort(C[1,:])[::-1]] # sort so largest is first
+        C = C[:, np.argsort(C[1, :])[::-1]]  # sort so largest is first
         if pcent:
-            C = C.astype('float64')
-            C[1,:] = C[1,:]/len(cc.membership)
+            C = C.astype("float64")
+            C[1, :] = C[1, :] / len(cc.membership)
 
         return C
 
     def large_components(self, large_comp_cutoff=0.1, cc=None, return_idx=False):
         """Find components in network greater than large_comp_cutoff.
 
         Args:
-            large_comp_cutoff (float/int, optional): Cutoff to be considered a large component. 
-                        If int is number of nodes, if float is percentage of total nodes. 
+            large_comp_cutoff (float/int, optional): Cutoff to be considered a large component.
+                        If int is number of nodes, if float is percentage of total nodes.
                         note decimal percentage so 33% cutoff would be 0.33.Defaults to 0.1
-            cc (ig.VertexClustering, optional): precalculated components/clustering. 
+            cc (ig.VertexClustering, optional): precalculated components/clustering.
                         Typically output of g.connected_components. Defaults to None.
             return_idx (bool, optional): flag wether to return indexs of components/clusters. Defaults to False.
 
         Returns:
             list/tuple of lists: if return idx returns tuple containing list of large component subgraphs and list of indexes
                                 otherwise returns just list of component subgraphs
         """
@@ -208,72 +213,74 @@
             cc = self.connected_components()
 
         if isinstance(large_comp_cutoff, float):
             pcent = True
         elif isinstance(large_comp_cutoff, int):
             pcent = False
         else:
-            raise ValueError('large_comp_cutoff should be node number or decimal percentage (i.e. 33% cutoff should be 0.33)')
+            raise ValueError(
+                "large_comp_cutoff should be node number or decimal percentage (i.e. 33% cutoff should be 0.33)"
+            )
 
         C = self.component_sizes(cc, pcent=pcent)
 
-        large_comps = C[0,C[1,:] >= large_comp_cutoff]
+        large_comps = C[0, C[1, :] >= large_comp_cutoff]
         components = [cc.subgraph(idx) for idx in large_comps]
 
-        return (components, large_comps)  if return_idx else components
-
-
+        return (components, large_comps) if return_idx else components
 
     def find_first_second_largest_cc(self, cc=None):
         if cc is None:
             cc = self.connected_components()
             cc = cc.membership
-    
+
         C = np.vstack(np.unique(cc, return_counts=True))
-        cmax = C[:,C[1,:].argmax()]
-        cc2 = C[:,(C[1, :] > 1) & (C[1,:] < cmax[1])] # find values lower than max but greater than 1 (might be empty?)
+        cmax = C[:, C[1, :].argmax()]
+        cc2 = C[
+            :, (C[1, :] > 1) & (C[1, :] < cmax[1])
+        ]  # find values lower than max but greater than 1 (might be empty?)
         try:
-            cc2 = cc2[:,cc2[1,:].argmax()]
+            cc2 = cc2[:, cc2[1, :].argmax()]
         except ValueError:
-            return cmax[0], None # if no second component return None.
+            return cmax[0], None  # if no second component return None.
 
-        return cmax[0], cc2[0] # returns index for largest and 2nd largest components
+        return cmax[0], cc2[0]  # returns index for largest and 2nd largest components
 
     def get_comp(self, idx, cc=None):
         if cc is None:
             cc = self.connected_components()
-        
+
         gc = cc.subgraph(idx=idx)
 
         return self.from_igraph(gc)
 
     def max_component(self):
         cc = self.connected_components()
         idxmax, idx2 = self.find_first_second_largest_cc(cc.membership)
         return self.get_comp(idx=idxmax, cc=cc)
 
     def get_2ndmax_comp(self):
         cc = self.connected_components()
         idxmax, idx2 = self.find_first_second_largest_cc(cc.membership)
         if idx2 is None:
-            raise ValueError('No 2nd largest component')
+            raise ValueError("No 2nd largest component")
         return self.get_comp(idx=idx2, cc=cc)
 
     def get_X(self):
         X = []
         for k in self.vs.attributes():
             v = self.vs[k]
             X.append(v)
-        X = np.array(X).T # Transpose to have shape n x d
+        X = np.array(X).T  # Transpose to have shape n x d
         return X
 
     def plot_degree_dist(self, logbinsize=0.1, LOG_ONLY=False):
         degree = self.degree()
         plot_degree_dist(degree_dist=degree, logbinsize=logbinsize, LOG_ONLY=LOG_ONLY)
 
-    def plottable(self, mode='undirected'):
+    def plottable(self, mode="undirected"):
         A = self.get_adjacency_sparse()
         return ig.Graph().Adjacency(A, mode=mode)
 
     @classmethod
     def from_igraph(cls, gg, *args, **kwds):
-        return cls(*args, **kwds) + gg
+        return cls(*args, **kwds) + gg
```

### Comparing `simnetpy-0.2.1/src/simnet/graph/plotting.py` & `simnetpy-0.3.1/src/simnetpy/graph/plotting.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,205 +1,341 @@
-import numpy as np
-import matplotlib.pyplot as plt
 import igraph as ig
-import sklearn.decomposition as decomp 
+import matplotlib.pyplot as plt
+import numpy as np
+import sklearn.decomposition as decomp
 
 
 def check_community_order(y):
     mem = set()
     order = []
     for idx in y:
         if idx not in mem:
             order.append(idx)
             mem.add(idx)
     return order
 
+
 def gen_layout(g, method, scale_factor, center):
     l = g.layout(layout=method)
     # l.fit_into(bbox)
     l.scale(scale_factor)
     l.center(center)
     return l
 
-def cluster_graph_frame(g, attr, layout_alg='fr'):
+
+def cluster_graph_frame(g, attr, layout_alg="fr"):
     clstr = ig.VertexClustering.FromAttribute(g, attr)
     ggclst = clstr.cluster_graph(combine_edges=dict(weight="sum"))
     frame = ggclst.layout(layout_alg)
     return frame, clstr, ggclst
 
-def layout_per_cluster(clstr, ggclst, centers, N, nclstr_factor=0.5, clstr_size_factor=0.5, node_layout_alg='fr', vs_id_attr='name'):
+
+def layout_per_cluster(
+    clstr,
+    ggclst,
+    centers,
+    N,
+    nclstr_factor=0.5,
+    clstr_size_factor=0.5,
+    node_layout_alg="fr",
+    vs_id_attr="name",
+):
     layouts = []
 
     for i, gg in enumerate(clstr.subgraphs()):
-            # change scaling based on number nodes
-            # factor = gg.vcount()/ N
-            scale_factor = nclstr_factor*1/(ggclst.vcount()) + clstr_size_factor*gg.vcount()/N
-            # scale_factor = factor/(ggclst.vcount())
-    
-            ll = gen_layout(gg, node_layout_alg, scale_factor=scale_factor, center=centers[i])
-            layouts.append({v: coord for v, coord in zip(gg.vs[vs_id_attr],ll)})
+        # change scaling based on number nodes
+        # factor = gg.vcount()/ N
+        scale_factor = (
+            nclstr_factor * 1 / (ggclst.vcount()) + clstr_size_factor * gg.vcount() / N
+        )
+        # scale_factor = factor/(ggclst.vcount())
+
+        ll = gen_layout(
+            gg, node_layout_alg, scale_factor=scale_factor, center=centers[i]
+        )
+        layouts.append({v: coord for v, coord in zip(gg.vs[vs_id_attr], ll)})
 
     # unpack layouts
     layout_dict = {}
     for dd in layouts:
         layout_dict = {**layout_dict, **dd}
     layout = [layout_dict[x] for x in sorted(layout_dict.keys(), key=lambda x: int(x))]
     return layout
 
-def group_by_cluster_layout(g, y_group, nclstr_factor=0.1, clstr_size_factor=1, frame_layout_alg='fr', node_layout_alg='fr'):
+
+def group_by_cluster_layout(
+    g,
+    y_group,
+    nclstr_factor=0.1,
+    clstr_size_factor=1,
+    frame_layout_alg="fr",
+    node_layout_alg="fr",
+):
     N = g.vcount()
-    g.vs['name'] = list(np.arange(N))
-    g.vs['y_group'] = list(y_group)
+    g.vs["name"] = list(np.arange(N))
+    g.vs["y_group"] = list(y_group)
     # g.vs['y_color'] = list(y_color)
 
-    frame, clstr, ggclst = cluster_graph_frame(g, attr='y_group', layout_alg=frame_layout_alg)
-    layout = layout_per_cluster(clstr, ggclst, centers=frame.coords, N=N, nclstr_factor=nclstr_factor, clstr_size_factor=clstr_size_factor, node_layout_alg=node_layout_alg)
+    frame, clstr, ggclst = cluster_graph_frame(
+        g, attr="y_group", layout_alg=frame_layout_alg
+    )
+    layout = layout_per_cluster(
+        clstr,
+        ggclst,
+        centers=frame.coords,
+        N=N,
+        nclstr_factor=nclstr_factor,
+        clstr_size_factor=clstr_size_factor,
+        node_layout_alg=node_layout_alg,
+    )
 
     return layout
 
-def plot_by_cluster(g, y_color, y_group, nclstr_factor=0.1, clstr_size_factor=0.2, layout=None, markersize=5, scale_marker=False, edge_alpha=0.5, edge_width=0.5, node_alpha=0.3, ax=None, style_dict=None, **kwds):
+
+def plot_by_cluster(
+    g,
+    y_color,
+    y_group,
+    nclstr_factor=0.1,
+    clstr_size_factor=0.2,
+    layout=None,
+    markersize=5,
+    scale_marker=False,
+    edge_alpha=0.5,
+    edge_width=0.5,
+    node_alpha=0.3,
+    ax=None,
+    style_dict=None,
+    **kwds,
+):
     if layout is None:
-        layout = group_by_cluster_layout(g, y_group, nclstr_factor=nclstr_factor, clstr_size_factor=clstr_size_factor)
-    
+        layout = group_by_cluster_layout(
+            g, y_group, nclstr_factor=nclstr_factor, clstr_size_factor=clstr_size_factor
+        )
+
     L = np.array(layout)
 
     if ax is None:
-            fig, ax = plt.subplots(dpi=200)
+        fig, ax = plt.subplots(dpi=200)
     else:
         fig = None
 
-    dd = np.array(g.degree())+1 # +1 to ensure isolated nodes appear on plot
-    dd = dd/dd.max()
-    dd = (dd**2)*(10*markersize**2)
+    dd = np.array(g.degree()) + 1  # +1 to ensure isolated nodes appear on plot
+    dd = dd / dd.max()
+    dd = (dd**2) * (10 * markersize**2)
 
     nclstr = len(np.unique(y_group))
     for i, c in enumerate(np.unique(y_group)):
-        idx = y_group==c
-        c = [f'C{int(j)}' for j in y_color[idx]]
+        idx = y_group == c
+        c = [f"C{int(j)}" for j in y_color[idx]]
         if scale_marker:
-            ax.scatter(x=L[idx,0], y=L[idx,1], c=c, s=dd[idx], alpha=node_alpha, marker='.', linewidths=0, **kwds)
+            ax.scatter(
+                x=L[idx, 0],
+                y=L[idx, 1],
+                c=c,
+                s=dd[idx],
+                alpha=node_alpha,
+                marker=".",
+                linewidths=0,
+                **kwds,
+            )
         else:
-            ax.scatter(x=L[idx,0], y=L[idx,1], c=c, alpha=node_alpha, s=markersize**2, marker='.', linewidths=0, **kwds)
+            ax.scatter(
+                x=L[idx, 0],
+                y=L[idx, 1],
+                c=c,
+                alpha=node_alpha,
+                s=markersize**2,
+                marker=".",
+                linewidths=0,
+                **kwds,
+            )
 
     if style_dict is None:
         style_dict = {
             "edge_width": edge_width,
-            "edge_color": 'lightgrey',
+            "edge_color": "lightgrey",
         }
 
-
-    style_dict['layout'] = layout
+    style_dict["layout"] = layout
     ig.plot(g.plottable(), target=ax, **style_dict)
     # fix aspect ratio
-    ax.set_aspect('auto')
+    ax.set_aspect("auto")
 
     N = g.vcount()
     ecount = g.ecount()
-    #remove igraph circles (we use scatter instead)
-    [edge.set_alpha(edge_alpha) for edge in ax.get_children()[N+nclstr:N+nclstr+ecount]]
-    [vertex.remove() for vertex in ax.get_children()[nclstr:N+nclstr]]
+    # remove igraph circles (we use scatter instead)
+    [
+        edge.set_alpha(edge_alpha)
+        for edge in ax.get_children()[N + nclstr : N + nclstr + ecount]
+    ]
+    [vertex.remove() for vertex in ax.get_children()[nclstr : N + nclstr]]
     # change alpha of edges
     return fig, ax
 
 
-
-def network_plot_cmap(g, X, c, markersize=3, scale_marker=False, edge_alpha=0.5, edge_width=0.5, node_alpha=0.3,
-                      style_dict=None, PCA=False, ax=None, **scatterkwds):
-     # create new figure if user ax not provided
+def network_plot_cmap(
+    g,
+    X,
+    c,
+    markersize=3,
+    scale_marker=False,
+    edge_alpha=0.5,
+    edge_width=0.5,
+    node_alpha=0.3,
+    style_dict=None,
+    PCA=False,
+    ax=None,
+    **scatterkwds,
+):
+    # create new figure if user ax not provided
     if ax is None:
         fig, ax = plt.subplots(dpi=100)
     else:
         fig = None
-        
+
     if PCA:
         pca = decomp.PCA(n_components=2)
         Z = pca.fit_transform(X)
     else:
-        Z = X[:,:2]
+        Z = X[:, :2]
 
-    dd = np.array(g.degree())+1 # +1 to ensure isolated nodes appear on plot
-    dd = dd/dd.max()
-    dd = (dd**2)*(markersize**2)
+    dd = np.array(g.degree()) + 1  # +1 to ensure isolated nodes appear on plot
+    dd = dd / dd.max()
+    dd = (dd**2) * (markersize**2)
 
     # zorder adjusts plotting order so nodes cover edges.
     if scale_marker:
-        cbar = ax.scatter(x=Z[:,0], y=Z[:,1], c=c, s=dd, alpha=node_alpha, marker='.', linewidths=0, zorder=10, **scatterkwds)
+        cbar = ax.scatter(
+            x=Z[:, 0],
+            y=Z[:, 1],
+            c=c,
+            s=dd,
+            alpha=node_alpha,
+            marker=".",
+            linewidths=0,
+            zorder=10,
+            **scatterkwds,
+        )
     else:
-        cbar = ax.scatter(x=Z[:,0], y=Z[:,1], c=c, s=markersize**2, alpha=node_alpha, marker='.', linewidths=0, zorder=10, **scatterkwds)
+        cbar = ax.scatter(
+            x=Z[:, 0],
+            y=Z[:, 1],
+            c=c,
+            s=markersize**2,
+            alpha=node_alpha,
+            marker=".",
+            linewidths=0,
+            zorder=10,
+            **scatterkwds,
+        )
 
     if fig is not None:
         fig.subplots_adjust(right=0.8)
         cbar_ax = fig.add_axes([0.85, 0.15, 0.05, 0.7])
         fig.colorbar(cbar, cax=cbar_ax)
-    
+
     if style_dict is None:
         style_dict = {
             "edge_width": edge_width,
-            "edge_color": 'lightgrey',
+            "edge_color": "lightgrey",
         }
 
     if isinstance(Z, np.ndarray):
-        coords=Z.tolist()
+        coords = Z.tolist()
     else:
         coords = Z
     layout = ig.Layout(coords=coords)
-    style_dict['layout'] = layout
+    style_dict["layout"] = layout
 
     ig.plot(g.plottable(), target=ax, **style_dict)
-    ax.set_aspect('auto')
+    ax.set_aspect("auto")
     N = g.vcount()
     ecount = g.ecount()
-    [edge.set_alpha(edge_alpha) for edge in ax.get_children()[N+1:N+1+ecount]]
-    [vertex.remove() for vertex in ax.get_children()[1:N+1]]
+    [edge.set_alpha(edge_alpha) for edge in ax.get_children()[N + 1 : N + 1 + ecount]]
+    [vertex.remove() for vertex in ax.get_children()[1 : N + 1]]
 
     return fig, ax
 
 
-def network_plot_col_by_cluster(g, X, y, markersize=3, min_markersize=1.5, scale_marker=False, edge_alpha=0.5, edge_width=0.5, node_alpha=0.3,
-                      style_dict=None, PCA=False, ax=None, **scatterkwds):
-     # create new figure if user ax not provided
+def network_plot_col_by_cluster(
+    g,
+    X,
+    y,
+    markersize=3,
+    min_markersize=1.5,
+    scale_marker=False,
+    edge_alpha=0.5,
+    edge_width=0.5,
+    node_alpha=0.3,
+    style_dict=None,
+    PCA=False,
+    ax=None,
+    **scatterkwds,
+):
+    # create new figure if user ax not provided
     if ax is None:
         fig, ax = plt.subplots(dpi=100)
     else:
         fig = None
-        
+
     if PCA:
         pca = decomp.PCA(n_components=2)
         Z = pca.fit_transform(X)
     else:
-        Z = X[:,:2]
+        Z = X[:, :2]
 
-    dd = np.array(g.degree())+1 # +1 to ensure isolated nodes appear on plot
-    dd = dd/dd.max()
-    dd = (dd**2)*(markersize**2) + min_markersize**2
+    dd = np.array(g.degree()) + 1  # +1 to ensure isolated nodes appear on plot
+    dd = dd / dd.max()
+    dd = (dd**2) * (markersize**2) + min_markersize**2
 
     # zorder adjusts plotting order so nodes cover edges.
     nclstr = len(np.unique(y))
     for i, c in enumerate(np.unique(y)):
-        idx = y==c
+        idx = y == c
 
         if scale_marker:
-            ax.scatter(x=Z[idx,0], y=Z[idx,1], c=f'C{i}', s=dd[idx], alpha=node_alpha, marker='.', linewidths=0, zorder=10, **scatterkwds)
+            ax.scatter(
+                x=Z[idx, 0],
+                y=Z[idx, 1],
+                c=f"C{i}",
+                s=dd[idx],
+                alpha=node_alpha,
+                marker=".",
+                linewidths=0,
+                zorder=10,
+                **scatterkwds,
+            )
         else:
-            ax.scatter(x=Z[idx,0], y=Z[idx,1], c=f'C{i}', s=markersize**2, alpha=node_alpha, marker='.', linewidths=0, zorder=10, **scatterkwds)
-    
+            ax.scatter(
+                x=Z[idx, 0],
+                y=Z[idx, 1],
+                c=f"C{i}",
+                s=markersize**2,
+                alpha=node_alpha,
+                marker=".",
+                linewidths=0,
+                zorder=10,
+                **scatterkwds,
+            )
+
     if style_dict is None:
         style_dict = {
             "edge_width": edge_width,
-            "edge_color": 'lightgrey',
+            "edge_color": "lightgrey",
         }
 
     if isinstance(Z, np.ndarray):
-        coords=Z.tolist()
+        coords = Z.tolist()
     else:
         coords = Z
     layout = ig.Layout(coords=coords)
-    style_dict['layout'] = layout
+    style_dict["layout"] = layout
 
     ig.plot(g.plottable(), target=ax, **style_dict)
-    ax.set_aspect('auto')
+    ax.set_aspect("auto")
     N = g.vcount()
     ecount = g.ecount()
     [edge.set_alpha(edge_alpha) for edge in ax.get_children()[N+nclstr:N+nclstr+ecount]]
     [vertex.remove() for vertex in ax.get_children()[nclstr:N+nclstr]]
 
-    return fig, ax
+    return fig, ax
```

### Comparing `simnetpy-0.2.1/src/simnet/plotting/graph_plot.py` & `simnetpy-0.3.1/src/simnetpy/plotting/graph_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import math
 import igraph as ig
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.patches as ptc
 import seaborn as sns
+import sklearn.decomposition as decomp 
+
 
 
 
 # from ..graph import Igraph
 
 
 def log_bin_means(x, y, bins):
@@ -274,8 +276,85 @@
         g = g.plottable()
     except AttributeError:
         g = g
     
     ig.plot(g, target=ax, **vs)
     color_nodes(ax, g, y, alpha)
 
+    return fig, ax
+
+
+
+def plot_data_col_by_cluster(X, y=None, ax = None, PCA=True, print_variance=False, alpha=0.2, marker='o', linestyle='None', **kwds):
+    if y is None:
+        y = np.ones(X.shape[0])
+
+    if PCA:
+        pca = decomp.PCA(n_components=2)
+        Z = pca.fit_transform(X)
+        if print_variance:
+            print(pca.explained_variance_ratio_)
+    else:
+        Z = X[:,:2]
+
+    # create new figure if user ax not provided
+    if ax is None:
+        fig, ax = plt.subplots(dpi=100)
+    else:
+        fig = None
+        
+    for i, c in enumerate(np.unique(y)):
+        idx = y==c
+        ax.plot(Z[idx,0], Z[idx,1], marker=marker, linestyle=linestyle, alpha=alpha, **kwds)
+
+    return fig, ax
+
+
+def plot_network_in_dataspace(g, X, y, markersize=3, style_dict=None, PCA=False, ax=None, **scatterkwds):
+     # create new figure if user ax not provided
+    if ax is None:
+        fig, ax = plt.subplots(dpi=100)
+    else:
+        fig = None
+        
+    if PCA:
+        pca = decomp.PCA(n_components=2)
+        Z = pca.fit_transform(X)
+    else:
+        Z = X[:,:2]
+
+    dd = np.array(g.degree())+1 # +1 to ensure isolated nodes appear on plot
+    dd = dd/dd.max()
+    dd = (dd**2)*(markersize**2)
+
+    nclstr = len(np.unique(y))
+    for i, c in enumerate(np.unique(y)):
+        idx = y==c
+        ax.scatter(x=Z[idx,0], y=Z[idx,1], c=f'C{i}', s=dd[idx], zorder=10, **scatterkwds)
+
+    if style_dict is None:
+        style_dict = {
+            "edge_width": 0.5,
+            "edge_color": 'lightgrey',
+        }
+
+    if isinstance(Z, np.ndarray):
+        coords=Z.tolist()
+    else:
+        coords = Z
+    layout = ig.Layout(coords=coords)
+    style_dict['layout'] = layout
+    # edge_width=0.5, edge_color='lightgrey'
+    # visual_style = {
+    #     "edge_width": edge_width,
+    #     "edge_color": edge_color,
+    #     "layout": layout,
+    #     **igstylekwds,
+    # }
+    
+
+    ig.plot(g.plottable(), target=ax, **style_dict)
+    ax.set_aspect('auto')
+    N = g.vcount()
+    [vertex.remove() for vertex in ax.get_children()[nclstr:N+nclstr]]
+
     return fig, ax
```

### Comparing `simnetpy-0.2.1/src/simnet/plotting/igraph_vis.py` & `simnetpy-0.3.1/src/simnetpy/plotting/igraph_vis.py`

 * *Files identical despite different names*

### Comparing `simnetpy-0.2.1/src/simnet/similarity/merging.py` & `simnetpy-0.3.1/src/simnetpy/similarity/merging.py`

 * *Files identical despite different names*

### Comparing `simnetpy-0.2.1/src/simnet/similarity/similarity.py` & `simnetpy-0.3.1/src/simnetpy/similarity/similarity.py`

 * *Files identical despite different names*

### Comparing `simnetpy-0.2.1/src/simnet/similarity/threshold.py` & `simnetpy-0.3.1/src/simnetpy/similarity/threshold.py`

 * *Files identical despite different names*

### Comparing `simnetpy-0.2.1/src/simnet/utils/filesys.py` & `simnetpy-0.3.1/src/simnetpy/utils/filesys.py`

 * *Files identical despite different names*

### Comparing `simnetpy-0.2.1/src/simnet/utils/plotting.py` & `simnetpy-0.3.1/src/simnetpy/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `simnetpy-0.2.1/src/simnet/utils/sci_funcs.py` & `simnetpy-0.3.1/src/simnetpy/utils/sci_funcs.py`

 * *Files identical despite different names*

