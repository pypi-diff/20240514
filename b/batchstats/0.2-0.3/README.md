# Comparing `tmp/batchstats-0.2.tar.gz` & `tmp/batchstats-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchstats-0.2.tar", last modified: Sun May 12 13:20:32 2024, max compression
+gzip compressed data, was "batchstats-0.3.tar", last modified: Mon May 13 22:08:59 2024, max compression
```

## Comparing `batchstats-0.2.tar` & `batchstats-0.3.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:20:32.165073 batchstats-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-12 13:20:21.000000 batchstats-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-12 13:20:32.165073 batchstats-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-12 13:20:21.000000 batchstats-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:20:32.161073 batchstats-0.2/batchstats/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-12 13:20:21.000000 batchstats-0.2/batchstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13188 2024-05-12 13:20:21.000000 batchstats-0.2/batchstats/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:20:32.161073 batchstats-0.2/batchstats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-12 13:20:32.000000 batchstats-0.2/batchstats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-12 13:20:32.000000 batchstats-0.2/batchstats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:20:32.000000 batchstats-0.2/batchstats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 13:20:32.000000 batchstats-0.2/batchstats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-12 13:20:32.000000 batchstats-0.2/batchstats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 13:20:32.165073 batchstats-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-12 13:20:21.000000 batchstats-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:20:32.161073 batchstats-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-12 13:20:21.000000 batchstats-0.2/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:59.930142 batchstats-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 22:08:48.000000 batchstats-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-13 22:08:59.930142 batchstats-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-13 22:08:48.000000 batchstats-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:59.926142 batchstats-0.3/batchstats/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 22:08:48.000000 batchstats-0.3/batchstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-13 22:08:48.000000 batchstats-0.3/batchstats/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-13 22:08:48.000000 batchstats-0.3/batchstats/nanstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-05-13 22:08:48.000000 batchstats-0.3/batchstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:59.930142 batchstats-0.3/batchstats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-13 22:08:59.000000 batchstats-0.3/batchstats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-13 22:08:59.000000 batchstats-0.3/batchstats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:08:59.000000 batchstats-0.3/batchstats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 22:08:59.000000 batchstats-0.3/batchstats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 22:08:59.000000 batchstats-0.3/batchstats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 22:08:59.930142 batchstats-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-13 22:08:48.000000 batchstats-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:59.926142 batchstats-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-13 22:08:48.000000 batchstats-0.3/tests/test_nanstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-13 22:08:48.000000 batchstats-0.3/tests/test_stats.py
```

### Comparing `batchstats-0.2/LICENSE` & `batchstats-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `batchstats-0.2/PKG-INFO` & `batchstats-0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,10 @@
-Metadata-Version: 2.1
-Name: batchstats
-Version: 0.2
-Summary: Efficient batch statistics computation library for Python.
-Home-page: https://github.com/CyrilJl/BatchStats
-Author: Cyril Joly
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-
 [![PyPI Version](https://img.shields.io/pypi/v/batchstats.svg)](https://pypi.org/project/batchstats/)
 
-# BatchStats
+# <img src="https://raw.githubusercontent.com/CyrilJl/BatchStats/main/docs/source/_static/logo_batchstats.svg" alt="Logo BatchStats" width="56.5" height="35"> BatchStats: Efficient Batch Statistics Computation in Python
 
 `batchstats` is a Python package designed to compute various statistics of data that arrive batch by batch, making it suitable for streaming input or data too large to fit in memory.
 
 ## Installation
 
 You can install `batchstats` using pip:
 
@@ -132,12 +122,38 @@
 >>> True
 %timeit a = np.var(data, axis=0)
 %timeit b = BatchVar().update_batch(data)()
 >>> 510 ms ± 111 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 >>> 306 ms ± 5.09 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 ```
 
+## NaN handling possibility
+
+While the previous `Batch*` classes exclude every sample containing at least one NaN from the computations, the `BatchNan*` classes adopt a more flexible approach to handling NaN values, similar to `np.nansum`, `np.nanmean`, etc. Consequently, the outputted statistics can be computed from various numbers of samples for each feature:
+
+```python
+import numpy as np
+from batchstats import BatchNanSum
+
+m, n = 1_000_000, 50
+nan_ratio = 0.05
+n_batches = 17
+
+data = np.random.randn(m, n)
+num_nans = int(m * n * nan_ratio)
+nan_indices = np.random.choice(range(m * n), num_nans, replace=False)
+data.ravel()[nan_indices] = np.nan
+
+batchsum = BatchNanSum()
+for batch_data in np.array_split(data, n_batches):
+    batchsum.update_batch(batch=batch_data)
+np.allclose(np.nansum(data, axis=0), batchsum())
+>>> True
+```
+
+## Documentation
 
+The documentation is available [here](https://batchstats.readthedocs.io/en/latest/).
 
 ## Requesting Additional Statistics
 
 If you require additional statistics that are not currently implemented in `batchstats`, feel free to open an issue on the GitHub repository or submit a pull request with your suggested feature. We welcome contributions and feedback from the community to improve `batchstats` and make it more versatile for various data analysis tasks.
```

### Comparing `batchstats-0.2/README.md` & `batchstats-0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,20 @@
+Metadata-Version: 2.1
+Name: batchstats
+Version: 0.3
+Summary: Efficient batch statistics computation library for Python.
+Home-page: https://github.com/CyrilJl/BatchStats
+Author: Cyril Joly
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+
 [![PyPI Version](https://img.shields.io/pypi/v/batchstats.svg)](https://pypi.org/project/batchstats/)
 
-# BatchStats
+# <img src="https://raw.githubusercontent.com/CyrilJl/BatchStats/main/docs/source/_static/logo_batchstats.svg" alt="Logo BatchStats" width="56.5" height="35"> BatchStats: Efficient Batch Statistics Computation in Python
 
 `batchstats` is a Python package designed to compute various statistics of data that arrive batch by batch, making it suitable for streaming input or data too large to fit in memory.
 
 ## Installation
 
 You can install `batchstats` using pip:
 
@@ -122,12 +132,38 @@
 >>> True
 %timeit a = np.var(data, axis=0)
 %timeit b = BatchVar().update_batch(data)()
 >>> 510 ms ± 111 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 >>> 306 ms ± 5.09 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 ```
 
+## NaN handling possibility
+
+While the previous `Batch*` classes exclude every sample containing at least one NaN from the computations, the `BatchNan*` classes adopt a more flexible approach to handling NaN values, similar to `np.nansum`, `np.nanmean`, etc. Consequently, the outputted statistics can be computed from various numbers of samples for each feature:
+
+```python
+import numpy as np
+from batchstats import BatchNanSum
+
+m, n = 1_000_000, 50
+nan_ratio = 0.05
+n_batches = 17
+
+data = np.random.randn(m, n)
+num_nans = int(m * n * nan_ratio)
+nan_indices = np.random.choice(range(m * n), num_nans, replace=False)
+data.ravel()[nan_indices] = np.nan
+
+batchsum = BatchNanSum()
+for batch_data in np.array_split(data, n_batches):
+    batchsum.update_batch(batch=batch_data)
+np.allclose(np.nansum(data, axis=0), batchsum())
+>>> True
+```
+
+## Documentation
 
+The documentation is available [here](https://batchstats.readthedocs.io/en/latest/).
 
 ## Requesting Additional Statistics
 
 If you require additional statistics that are not currently implemented in `batchstats`, feel free to open an issue on the GitHub repository or submit a pull request with your suggested feature. We welcome contributions and feedback from the community to improve `batchstats` and make it more versatile for various data analysis tasks.
```

### Comparing `batchstats-0.2/batchstats/core.py` & `batchstats-0.3/batchstats/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,12 @@
 import string
 
 import numpy as np
 
-
-class NoValidSamplesError(ValueError):
-    """
-    Error raised when there are no valid samples for calculation.
-    """
-    pass
-
-
-class UnequalSamplesNumber(ValueError):
-    """
-    Error raised when two batches have unequal lengths.
-    """
-    pass
-
-
-def any_nan(x, axis=None):
-    """
-    Check if there are any NaN values in the input array.
-
-    Args:
-        x (numpy.ndarray): Input array.
-        axis (int or tuple of ints, optional): Axis or axes along which to operate. Default is None.
-
-    Returns:
-        numpy.ndarray: Boolean array indicating NaN presence.
-
-    """
-    return np.isnan(np.add.reduce(array=x, axis=axis))
+from ._misc import NoValidSamplesError, UnequalSamplesNumber, any_nan, check_params
 
 
 class BatchStat:
     """
     Base class for calculating statistics over batches of data.
 
     Attributes:
@@ -266,21 +239,23 @@
             return self.mean.copy()
 
 
 class BatchVar(BatchMean):
     """
     Class for calculating the variance of batches of data.
 
+    Args:
+        ddof (int, optional): Means Delta Degrees of Freedom. The divisor used in calculations is N - ddof, where N represents the number of elements. By default ddof is zero.
     """
 
     def __init__(self, ddof=0):
         super().__init__()
         self.mean = BatchMean()
         self.var = None
-        self.ddof = ddof
+        self.ddof = check_params(param=ddof, types=int)
 
     @classmethod
     def init_var(cls, v, vm):
         """
         Initialize variance.
 
         Args:
@@ -295,14 +270,17 @@
         ret /= len(v)
         return ret
 
     @staticmethod
     def compute_incremental_variance(v, p, u):
         """
         Compute incremental variance.
+        For v 2D and p/u 1D, equivalent to ``((v-p).T@(v-u)).sum(axis=0)`` or
+        ``np.einsum('ji,ji->i', v - p, v - u)``. Faster and less memory consumer because
+        no intermediate 2D array are created.
 
         Args:
             v (numpy.ndarray): Input data.
             p (numpy.ndarray): Previous mean.
             u (numpy.ndarray): Updated mean.
 
         Returns:
@@ -361,30 +339,32 @@
         return (self.n_samples / (self.n_samples - self.ddof)) * self.var
 
 
 class BatchCov(BatchStat):
     """
     Class for calculating the covariance of batches of data.
 
+    Args:
+        ddof (int, optional): Means Delta Degrees of Freedom. The divisor used in calculations is N - ddof, where N represents the number of elements. By default ddof is zero.
     """
 
     def __init__(self, ddof=0):
         super().__init__()
         self.mean1 = BatchMean()
         self.mean2 = BatchMean()
         self.cov = None
-        self.ddof = ddof
+        self.ddof = check_params(param=ddof, types=int)
 
     def _process_batch(self, batch1, batch2=None, assume_valid=False):
         """
         Process the input batches, handling NaN values if necessary.
 
         Args:
             batch1 (numpy.ndarray): Input batch 1.
-            batch2 (numpy.ndarray): Input batch 2.
+            batch2 (numpy.ndarray, optional): Input batch 2. Default is None.
             assume_valid (bool, optional): If True, assumes all elements in the batches are valid. Default is False.
 
         Returns:
             Tuple[numpy.ndarray, numpy.ndarray]: Processed batches 1 and 2.
 
         Raises:
             UnequalSamplesNumber: If the batches have unequal lengths.
@@ -410,15 +390,15 @@
 
     def update_batch(self, batch1, batch2=None, assume_valid=False):
         """
         Update the covariance with new batches of data.
 
         Args:
             batch1 (numpy.ndarray): Input batch 1.
-            batch2 (numpy.ndarray): Input batch 2.
+            batch2 (numpy.ndarray, optional): Input batch 2. Default is None.
             assume_valid (bool, optional): If True, assumes all elements in the batches are valid. Default is False.
 
         Returns:
             BatchCov: Updated BatchCov object.
 
         """
         batch1, batch2 = self._process_batch(batch1, batch2, assume_valid=assume_valid)
```

### Comparing `batchstats-0.2/batchstats.egg-info/PKG-INFO` & `batchstats-0.3/batchstats.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: batchstats
-Version: 0.2
+Version: 0.3
 Summary: Efficient batch statistics computation library for Python.
 Home-page: https://github.com/CyrilJl/BatchStats
 Author: Cyril Joly
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 [![PyPI Version](https://img.shields.io/pypi/v/batchstats.svg)](https://pypi.org/project/batchstats/)
 
-# BatchStats
+# <img src="https://raw.githubusercontent.com/CyrilJl/BatchStats/main/docs/source/_static/logo_batchstats.svg" alt="Logo BatchStats" width="56.5" height="35"> BatchStats: Efficient Batch Statistics Computation in Python
 
 `batchstats` is a Python package designed to compute various statistics of data that arrive batch by batch, making it suitable for streaming input or data too large to fit in memory.
 
 ## Installation
 
 You can install `batchstats` using pip:
 
@@ -132,12 +132,38 @@
 >>> True
 %timeit a = np.var(data, axis=0)
 %timeit b = BatchVar().update_batch(data)()
 >>> 510 ms ± 111 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 >>> 306 ms ± 5.09 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 ```
 
+## NaN handling possibility
 
+While the previous `Batch*` classes exclude every sample containing at least one NaN from the computations, the `BatchNan*` classes adopt a more flexible approach to handling NaN values, similar to `np.nansum`, `np.nanmean`, etc. Consequently, the outputted statistics can be computed from various numbers of samples for each feature:
+
+```python
+import numpy as np
+from batchstats import BatchNanSum
+
+m, n = 1_000_000, 50
+nan_ratio = 0.05
+n_batches = 17
+
+data = np.random.randn(m, n)
+num_nans = int(m * n * nan_ratio)
+nan_indices = np.random.choice(range(m * n), num_nans, replace=False)
+data.ravel()[nan_indices] = np.nan
+
+batchsum = BatchNanSum()
+for batch_data in np.array_split(data, n_batches):
+    batchsum.update_batch(batch=batch_data)
+np.allclose(np.nansum(data, axis=0), batchsum())
+>>> True
+```
+
+## Documentation
+
+The documentation is available [here](https://batchstats.readthedocs.io/en/latest/).
 
 ## Requesting Additional Statistics
 
 If you require additional statistics that are not currently implemented in `batchstats`, feel free to open an issue on the GitHub repository or submit a pull request with your suggested feature. We welcome contributions and feedback from the community to improve `batchstats` and make it more versatile for various data analysis tasks.
```

### Comparing `batchstats-0.2/setup.py` & `batchstats-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `batchstats-0.2/tests/test_core.py` & `batchstats-0.3/tests/test_stats.py`

 * *Files identical despite different names*

