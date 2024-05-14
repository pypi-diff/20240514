# Comparing `tmp/derivative-0.6.0.tar.gz` & `tmp/derivative-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "derivative-0.6.0.tar", max compression
+gzip compressed data, was "derivative-0.6.1.tar", max compression
```

## Comparing `derivative-0.6.0.tar` & `derivative-0.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1229 2023-05-06 17:44:02.681192 derivative-0.6.0/LICENSE.rst
--rw-r--r--   0        0        0     5447 2023-05-06 17:44:02.681192 derivative-0.6.0/README.rst
--rw-r--r--   0        0        0      212 2023-05-06 17:44:02.681192 derivative-0.6.0/derivative/__init__.py
--rw-r--r--   0        0        0       27 2023-05-06 17:44:02.681192 derivative-0.6.0/derivative/__version__.py
--rw-r--r--   0        0        0    11189 2023-05-06 17:44:02.681192 derivative-0.6.0/derivative/dglobal.py
--rw-r--r--   0        0        0     9399 2023-05-06 17:44:02.681192 derivative-0.6.0/derivative/differentiation.py
--rw-r--r--   0        0        0     5657 2023-05-06 17:44:02.681192 derivative-0.6.0/derivative/dlocal.py
--rw-r--r--   0        0        0     4230 2023-05-06 17:44:02.681192 derivative-0.6.0/derivative/utils.py
--rw-r--r--   0        0        0     1206 2023-05-06 17:44:02.685191 derivative-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 derivative-0.6.0/setup.py
--rw-r--r--   0        0        0     6666 1970-01-01 00:00:00.000000 derivative-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1229 2024-05-14 04:41:02.924659 derivative-0.6.1/LICENSE.rst
+-rw-r--r--   0        0        0     5490 2024-05-14 04:41:02.924659 derivative-0.6.1/README.rst
+-rw-r--r--   0        0        0      212 2024-05-14 04:41:02.924659 derivative-0.6.1/derivative/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-14 04:41:02.924659 derivative-0.6.1/derivative/__version__.py
+-rw-r--r--   0        0        0    11363 2024-05-14 04:41:02.924659 derivative-0.6.1/derivative/dglobal.py
+-rw-r--r--   0        0        0     9806 2024-05-14 04:41:02.924659 derivative-0.6.1/derivative/differentiation.py
+-rw-r--r--   0        0        0     5657 2024-05-14 04:41:02.924659 derivative-0.6.1/derivative/dlocal.py
+-rw-r--r--   0        0        0     4858 2024-05-14 04:41:02.924659 derivative-0.6.1/derivative/utils.py
+-rw-r--r--   0        0        0     1236 2024-05-14 04:41:02.928659 derivative-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6668 1970-01-01 00:00:00.000000 derivative-0.6.1/setup.py
+-rw-r--r--   0        0        0     6547 1970-01-01 00:00:00.000000 derivative-0.6.1/PKG-INFO
```

### Comparing `derivative-0.6.0/LICENSE.rst` & `derivative-0.6.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `derivative-0.6.0/README.rst` & `derivative-0.6.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -53,18 +53,18 @@
     # 7. Kernel derivative with smoothing set to 1
     result7 = dxdt(x, t, kind="kernel", sigma=1, lmbd=.1, kernel="rbf")
 
 Contributors:
 -------------
 Thanks to the members of the community who have contributed!
 
-+-----------------------------------------------------------------+----------------------------------------------------------------------------------+
-|  `Jacob Stevens-Haas <https://github.com/Jacob-Stevens-Haas>`_  | Kalman derivatives `#12 <https://github.com/andgoldschmidt/derivative/pull/12>`_,|
-|								  | Kernel derivatives `#30 <https://github.com/andgoldschmidt/derivative/pull/30>`_ |  
-+-----------------------------------------------------------------+----------------------------------------------------------------------------------+
++-----------------------------------------------------------------+-----------------------------------------------------------------------------------+
+|`Jacob Stevens-Haas <https://github.com/Jacob-Stevens-Haas>`_    | Kalman derivatives `#12 <https://github.com/andgoldschmidt/derivative/pull/12>`_, |
+|                                                                 | and more!                                                                         |
++-----------------------------------------------------------------+-----------------------------------------------------------------------------------+
 
 
 References:
 -----------
 
 [1] Numerical differentiation of experimental data: local versus global methods- K. Ahnert and M. Abel
 
@@ -79,26 +79,26 @@
 ------------------
 The **derivative** package is a contribution to `PySINDy <https://github.com/dynamicslab/pysindy/>`_; this work has been published in the Journal of Open Source Software (JOSS). If you use **derivative** in your work, please cite it using the following reference:
 
 Kaptanoglu et al., (2022). PySINDy: A comprehensive Python package for robust sparse system identification. Journal of Open Source Software, 7(69), 3994, https://doi.org/10.21105/joss.03994
 
 .. code-block:: text
 
-      @article{kaptanoglu2022pysindy,
-  	doi = {10.21105/joss.03994},
-  	url = {https://doi.org/10.21105/joss.03994},
-  	year = {2022},
-  	publisher = {The Open Journal},
-  	volume = {7},
-  	number = {69},
-  	pages = {3994},
-  	author = {Alan A. Kaptanoglu and Brian M. de Silva and Urban Fasel and Kadierdan Kaheman and Andy J. Goldschmidt and Jared Callaham and Charles B. Delahunt and Zachary G. Nicolaou and Kathleen Champion and Jean-Christophe Loiseau and J. Nathan Kutz and Steven L. Brunton},
-  	title = {PySINDy: A comprehensive Python package for robust sparse system identification},
-  	journal = {Journal of Open Source Software}
-	}
+	@article{kaptanoglu2022pysindy,
+		doi = {10.21105/joss.03994},
+		url = {https://doi.org/10.21105/joss.03994},
+		year = {2022},
+		publisher = {The Open Journal},
+		volume = {7},
+		number = {69},
+		pages = {3994},
+		author = {Alan A. Kaptanoglu and Brian M. de Silva and Urban Fasel and Kadierdan Kaheman and Andy J. Goldschmidt and Jared Callaham and Charles B. Delahunt and Zachary G. Nicolaou and Kathleen Champion and Jean-Christophe Loiseau and J. Nathan Kutz and Steven L. Brunton},
+		title = {PySINDy: A comprehensive Python package for robust sparse system identification},
+		journal = {Journal of Open Source Software}
+		}
     
 
 .. |RTD| image:: https://readthedocs.org/projects/derivative/badge/?version=latest
    :target: https://derivative.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
   
 .. |LIC| image:: https://img.shields.io/badge/License-MIT-blue.svg
```

### Comparing `derivative-0.6.0/derivative/dglobal.py` & `derivative-0.6.1/derivative/dglobal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import partialmethod
 from .differentiation import Derivative, register
-from .utils import deriv, integ, _memoize_arrays
+from .utils import deriv, integ, _memoize_arrays, _load_hyperparam_func
 
 import numpy as np
 from numpy.linalg import inv
 from scipy import interpolate, sparse
 from scipy.special import legendre
 from sklearn.linear_model import Lasso
 
@@ -188,15 +188,15 @@
         x_hat = self._global(t, x)[0]
         for i in indices:
             yield x_hat[i]
 
 
 @register("kalman")
 class Kalman(Derivative):
-    def __init__(self, alpha = 1):
+    def __init__(self, alpha=None):
         """ Fit the derivative assuming that given data are noisy measurements
 
         The Kalman smoother is the maximum likelihood estimator (MLE) for a process whose derivative obeys a Brownian
         motion. Equivalently, it is the MLE for a process whose measurement errors are drawn from standard normal distributions. 
         Specifically, it minimizes the convex objective
 
         .. math ::
@@ -211,14 +211,18 @@
             alpha (float): Ratio of measurement error variance to assumed process variance.
         """
         self.alpha = alpha
 
 
     @_memoize_arrays(1)
     def _global(self, t, z, alpha):
+        if alpha is None:
+            alpha = 1
+        if isinstance(alpha, str):
+            alpha = _load_hyperparam_func(f"kalman.{alpha}")(t, z)
         delta_times = t[1:]-t[:-1]
         n = len(t)
         Qs = [np.array([[dt, dt**2/2], [dt**2/2, dt**3/3]]) for dt in delta_times]
         Qinv = alpha*sparse.block_diag([np.linalg.inv(Q) for Q in Qs])
         Qinv = (Qinv + Qinv.T)/2  # force to be symmetric
 
         G_left = sparse.block_diag([-np.array([[1, 0], [dt, 1]]) for dt in delta_times])
```

### Comparing `derivative-0.6.0/derivative/differentiation.py` & `derivative-0.6.1/derivative/differentiation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import numpy as np
+from numpy.typing import NDArray
 
 from .utils import _memoize_arrays
 
 methods = {}
 default = ["finite_difference", {"k": 1}]
 
 
@@ -212,45 +213,42 @@
             X  (:obj:`ndarray` of float): Ordered measurements values. Multiple measurements allowed.
             t (:obj:`ndarray` of float): Ordered measurement times.
             axis ({0,1}). axis of X along which to smooth. default 1.
 
         Returns:
             :obj:`ndarray` of float: Returns dX/dt along axis.
         """
-        X, flat = _align_axes(X, t, axis)
+        X, orig_shape = _align_axes(X, t, axis)
 
         if X.shape[1] == 1:
             dX = X
         else:
             dX = np.array([list(self.compute_x_for(t, x, np.arange(len(t)))) for x in X])
 
-        return _restore_axes(dX, axis, flat)
+        return _restore_axes(dX, axis, orig_shape)
 
 
-def _align_axes(X, t, axis):
-    # Cast
+def _align_axes(X, t, axis) -> tuple[NDArray, tuple[int, ...]]:
     X = np.array(X)
-    flat = False
-    # Check shape and axis
-    if len(X.shape) == 1:
+    orig_shape = X.shape
+    # By convention, differentiate axis 1
+    if len(orig_shape) == 1:
         X = X.reshape(1, -1)
-        flat = True
-    elif len(X.shape) == 2:
-        if axis == 0:
-            X = X.T
-        elif axis == 1:
-            pass
-        else:
-            raise ValueError("Invalid axis.")
     else:
-        raise ValueError("Invalid shape of X.")
-
+        ax_len = orig_shape[axis]
+        # order of operations coupled with _restore_axes.  Move differentiation axis to
+        # zero so reshape does not skew differentiation axis
+        X = np.moveaxis(X, axis, 0).reshape((ax_len, -1)).T
     if X.shape[1] != len(t):
         raise ValueError("Desired X axis size does not match t size.")
-    return X, flat
+    return X, orig_shape
 
 
-def _restore_axes(dX, axis, flat):
-    if flat:
+def _restore_axes(dX: NDArray, axis: int, orig_shape: tuple[int, ...]) -> NDArray:
+    if len(orig_shape) == 1:
         return dX.flatten()
     else:
-        return dX if axis == 1 else dX.T
+        # order of operations coupled with _align_axes
+        extra_dims = tuple(length for ax, length in enumerate(orig_shape) if ax != axis)
+        moved_shape = (orig_shape[axis],) + extra_dims
+        dX = np.moveaxis(dX.T.reshape((moved_shape)), 0, axis)
+        return dX
```

### Comparing `derivative-0.6.0/derivative/dlocal.py` & `derivative-0.6.1/derivative/dlocal.py`

 * *Files identical despite different names*

### Comparing `derivative-0.6.0/derivative/utils.py` & `derivative-0.6.1/derivative/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,37 @@
+import sys
+
 from functools import _CacheInfo as CacheInfo, wraps
 from collections import OrderedDict, Counter
 import numpy as np
 from scipy.special import binom
 
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points
+else:
+    from importlib.metadata import entry_points
+
+hyperparam_algorithms = entry_points(group="derivative.hyperparam_opt")
+
+
+def _load_hyperparam_func(func_key):
+    try:
+        func = hyperparam_algorithms[func_key].load()
+    except KeyError:
+        raise ValueError(
+            f"No reduction method named {func_key} is installed."
+            "Reduction methods need to be installed as an entry point to"
+            "the 'derivative.hyperparam_opt' group"
+        )
+    return func
+
+
+def _default_kalman(t, z):
+    return 1
+
 
 def deriv(n, dx, order):
     """ Matrix derivative. Equi-spaced derivative via forward finite differences, mapping R^n into R^(n-order).
 
     Args:
         n (int): Number of data points
         dx (float): Width of x[k+1] - x[k]
```

### Comparing `derivative-0.6.0/pyproject.toml` & `derivative-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 [tool.poetry]
 name = "derivative"
-version = "0.6.0"
+version = "0.6.1"
 description = "Numerical differentiation in python."
 repository = "https://github.com/andgoldschmidt/derivative"
 documentation = "https://derivative.readthedocs.io/"
 keywords = ["differentiation", "derivative", "gradient", "prime"]
 authors = [
     "Andy Goldschmidt <andygold@uchicago.edu>",
     "Markus Quade <info@markusqua.de>",
     "Jacob Stevens-Haas <jmsh@uw.edu>"
 ]
 license = "MIT"
 readme = "README.rst"
 
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.9"
 numpy = "^1.18.3"
 scipy = "^1.4.1"
 scikit-learn = "^1"
 
 # docs
-sphinx = {version = "^4.5", optional = true}
+sphinx = {version = "^5", optional = true}
 nbsphinx = {version = "^0.6.1", optional = true}
 ipykernel = {version = "^5.2.1", optional = true}
 jupyter_client = {version = "^6.1.3", optional = true}
-sphinx_rtd_theme = {version = "^1", optional = true}
 matplotlib = {version = "^3.2.1", optional = true}
 #pandoc = {version = "^2.2", optional = true}
 
 # dev
 pytest = {version = "^7", optional = true}
 
 [tool.poetry.extras]
-docs = ["sphinx", "nbsphinx", "ipykernel", "jupyter_client", "sphinx_rtd_theme", "matplotlib", "pandoc"]
+docs = ["sphinx", "nbsphinx", "ipykernel", "jupyter_client", "matplotlib", "pandoc"]
 dev = ["pytest"]
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.plugins.'derivative.hyperparam_opt']
+"kalman.default" = "derivative.utils:_default_kalman"
```

### Comparing `derivative-0.6.0/setup.py` & `derivative-0.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,33 +8,37 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.18.3,<2.0.0', 'scikit-learn>=1,<2', 'scipy>=1.4.1,<2.0.0']
 
 extras_require = \
 {'dev': ['pytest>=7,<8'],
- 'docs': ['sphinx>=4.5,<5.0',
+ 'docs': ['sphinx>=5,<6',
           'nbsphinx>=0.6.1,<0.7.0',
           'ipykernel>=5.2.1,<6.0.0',
           'jupyter_client>=6.1.3,<7.0.0',
-          'sphinx_rtd_theme>=1,<2',
           'matplotlib>=3.2.1,<4.0.0']}
 
+entry_points = \
+{'derivative.hyperparam_opt': ['kalman.default = '
+                               'derivative.utils:_default_kalman']}
+
 setup_kwargs = {
     'name': 'derivative',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'Numerical differentiation in python.',
-    'long_description': '|RTD| |PyPI| |Zenodo| |GithubCI| |LIC|\n\nNumerical differentiation of noisy time series data in python\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\n**derivative** is a Python package for differentiating noisy data. The package showcases a variety of improvements that can be made over finite differences when data is not clean.\n\nWant to see an example of how **derivative** can help? This package is part of **PySINDy** (`github.com/dynamicslab/pysindy <https://github.com/dynamicslab/pysindy/>`_), a sparse-regression framework for discovering nonlinear dynamical systems from data.\n\nThis package binds common differentiation methods to a single easily implemented differentiation interface to encourage user adaptation.\nNumerical differentiation methods for noisy time series data in python includes:\n\n1. Symmetric finite difference schemes using arbitrary window size.\n\n2. Savitzky-Galoy derivatives (aka polynomial-filtered derivatives) of any polynomial order with independent left and right window parameters.\n\n3. Spectral derivatives with optional filter.\n\n4. Spline derivatives of any order.\n\n5. Polynomial-trend-filtered derivatives generalizing methods like total variational derivatives.\n\n6. Kalman derivatives find the maximum likelihood estimator for a derivative described by a Brownian motion.\n\n7. Kernel derivatives smooth a random process defined by its kernel (covariance).\n\n.. code-block:: python\n\n    from derivative import dxdt\n    import numpy as np\n\n    t = np.linspace(0,2*np.pi,50)\n    x = np.sin(x)\n\n    # 1. Finite differences with central differencing using 3 points.\n    result1 = dxdt(x, t, kind="finite_difference", k=1)\n\n    # 2. Savitzky-Golay using cubic polynomials to fit in a centered window of length 1\n    result2 = dxdt(x, t, kind="savitzky_golay", left=.5, right=.5, order=3)\n\n    # 3. Spectral derivative\n    result3 = dxdt(x, t, kind="spectral")\n\n    # 4. Spline derivative with smoothing set to 0.01\n    result4 = dxdt(x, t, kind="spline", s=1e-2)\n\n    # 5. Total variational derivative with regularization set to 0.01\n    result5 = dxdt(x, t, kind="trend_filtered", order=0, alpha=1e-2)\n\n    # 6. Kalman derivative with smoothing set to 1\n    result6 = dxdt(x, t, kind="kalman", alpha=1)\n    \n    # 7. Kernel derivative with smoothing set to 1\n    result7 = dxdt(x, t, kind="kernel", sigma=1, lmbd=.1, kernel="rbf")\n\nContributors:\n-------------\nThanks to the members of the community who have contributed!\n\n+-----------------------------------------------------------------+----------------------------------------------------------------------------------+\n|  `Jacob Stevens-Haas <https://github.com/Jacob-Stevens-Haas>`_  | Kalman derivatives `#12 <https://github.com/andgoldschmidt/derivative/pull/12>`_,|\n|\t\t\t\t\t\t\t\t  | Kernel derivatives `#30 <https://github.com/andgoldschmidt/derivative/pull/30>`_ |  \n+-----------------------------------------------------------------+----------------------------------------------------------------------------------+\n\n\nReferences:\n-----------\n\n[1] Numerical differentiation of experimental data: local versus global methods- K. Ahnert and M. Abel\n\n[2] Numerical Differentiation of Noisy, Nonsmooth Data- Rick Chartrand\n\n[3] The Solution Path of the Generalized LASSO- R.J. Tibshirani and J. Taylor\n\n[4] A Kernel Approach for PDE Discovery and Operator Learning - D. Long et al.\n\n\nCiting derivative:\n------------------\nThe **derivative** package is a contribution to `PySINDy <https://github.com/dynamicslab/pysindy/>`_; this work has been published in the Journal of Open Source Software (JOSS). If you use **derivative** in your work, please cite it using the following reference:\n\nKaptanoglu et al., (2022). PySINDy: A comprehensive Python package for robust sparse system identification. Journal of Open Source Software, 7(69), 3994, https://doi.org/10.21105/joss.03994\n\n.. code-block:: text\n\n      @article{kaptanoglu2022pysindy,\n  \tdoi = {10.21105/joss.03994},\n  \turl = {https://doi.org/10.21105/joss.03994},\n  \tyear = {2022},\n  \tpublisher = {The Open Journal},\n  \tvolume = {7},\n  \tnumber = {69},\n  \tpages = {3994},\n  \tauthor = {Alan A. Kaptanoglu and Brian M. de Silva and Urban Fasel and Kadierdan Kaheman and Andy J. Goldschmidt and Jared Callaham and Charles B. Delahunt and Zachary G. Nicolaou and Kathleen Champion and Jean-Christophe Loiseau and J. Nathan Kutz and Steven L. Brunton},\n  \ttitle = {PySINDy: A comprehensive Python package for robust sparse system identification},\n  \tjournal = {Journal of Open Source Software}\n\t}\n    \n\n.. |RTD| image:: https://readthedocs.org/projects/derivative/badge/?version=latest\n   :target: https://derivative.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n  \n.. |LIC| image:: https://img.shields.io/badge/License-MIT-blue.svg\n   :target: https://derivative.readthedocs.io/en/latest/license.html\n   :alt: MIT License\n\n.. |PyPI| image:: https://badge.fury.io/py/derivative.svg\n    :target: https://pypi.org/project/derivative/\n\n.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6617446.svg\n   :target: https://doi.org/10.5281/zenodo.6617446\n\n.. |GithubCI| image:: https://github.com/andgoldschmidt/derivative/actions/workflows/push-test.yml/badge.svg\n    :target: https://github.com/andgoldschmidt/derivative/actions/workflows/push-test.yml\n\n',
+    'long_description': '|RTD| |PyPI| |Zenodo| |GithubCI| |LIC|\n\nNumerical differentiation of noisy time series data in python\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\n**derivative** is a Python package for differentiating noisy data. The package showcases a variety of improvements that can be made over finite differences when data is not clean.\n\nWant to see an example of how **derivative** can help? This package is part of **PySINDy** (`github.com/dynamicslab/pysindy <https://github.com/dynamicslab/pysindy/>`_), a sparse-regression framework for discovering nonlinear dynamical systems from data.\n\nThis package binds common differentiation methods to a single easily implemented differentiation interface to encourage user adaptation.\nNumerical differentiation methods for noisy time series data in python includes:\n\n1. Symmetric finite difference schemes using arbitrary window size.\n\n2. Savitzky-Galoy derivatives (aka polynomial-filtered derivatives) of any polynomial order with independent left and right window parameters.\n\n3. Spectral derivatives with optional filter.\n\n4. Spline derivatives of any order.\n\n5. Polynomial-trend-filtered derivatives generalizing methods like total variational derivatives.\n\n6. Kalman derivatives find the maximum likelihood estimator for a derivative described by a Brownian motion.\n\n7. Kernel derivatives smooth a random process defined by its kernel (covariance).\n\n.. code-block:: python\n\n    from derivative import dxdt\n    import numpy as np\n\n    t = np.linspace(0,2*np.pi,50)\n    x = np.sin(x)\n\n    # 1. Finite differences with central differencing using 3 points.\n    result1 = dxdt(x, t, kind="finite_difference", k=1)\n\n    # 2. Savitzky-Golay using cubic polynomials to fit in a centered window of length 1\n    result2 = dxdt(x, t, kind="savitzky_golay", left=.5, right=.5, order=3)\n\n    # 3. Spectral derivative\n    result3 = dxdt(x, t, kind="spectral")\n\n    # 4. Spline derivative with smoothing set to 0.01\n    result4 = dxdt(x, t, kind="spline", s=1e-2)\n\n    # 5. Total variational derivative with regularization set to 0.01\n    result5 = dxdt(x, t, kind="trend_filtered", order=0, alpha=1e-2)\n\n    # 6. Kalman derivative with smoothing set to 1\n    result6 = dxdt(x, t, kind="kalman", alpha=1)\n    \n    # 7. Kernel derivative with smoothing set to 1\n    result7 = dxdt(x, t, kind="kernel", sigma=1, lmbd=.1, kernel="rbf")\n\nContributors:\n-------------\nThanks to the members of the community who have contributed!\n\n+-----------------------------------------------------------------+-----------------------------------------------------------------------------------+\n|`Jacob Stevens-Haas <https://github.com/Jacob-Stevens-Haas>`_    | Kalman derivatives `#12 <https://github.com/andgoldschmidt/derivative/pull/12>`_, |\n|                                                                 | and more!                                                                         |\n+-----------------------------------------------------------------+-----------------------------------------------------------------------------------+\n\n\nReferences:\n-----------\n\n[1] Numerical differentiation of experimental data: local versus global methods- K. Ahnert and M. Abel\n\n[2] Numerical Differentiation of Noisy, Nonsmooth Data- Rick Chartrand\n\n[3] The Solution Path of the Generalized LASSO- R.J. Tibshirani and J. Taylor\n\n[4] A Kernel Approach for PDE Discovery and Operator Learning - D. Long et al.\n\n\nCiting derivative:\n------------------\nThe **derivative** package is a contribution to `PySINDy <https://github.com/dynamicslab/pysindy/>`_; this work has been published in the Journal of Open Source Software (JOSS). If you use **derivative** in your work, please cite it using the following reference:\n\nKaptanoglu et al., (2022). PySINDy: A comprehensive Python package for robust sparse system identification. Journal of Open Source Software, 7(69), 3994, https://doi.org/10.21105/joss.03994\n\n.. code-block:: text\n\n\t@article{kaptanoglu2022pysindy,\n\t\tdoi = {10.21105/joss.03994},\n\t\turl = {https://doi.org/10.21105/joss.03994},\n\t\tyear = {2022},\n\t\tpublisher = {The Open Journal},\n\t\tvolume = {7},\n\t\tnumber = {69},\n\t\tpages = {3994},\n\t\tauthor = {Alan A. Kaptanoglu and Brian M. de Silva and Urban Fasel and Kadierdan Kaheman and Andy J. Goldschmidt and Jared Callaham and Charles B. Delahunt and Zachary G. Nicolaou and Kathleen Champion and Jean-Christophe Loiseau and J. Nathan Kutz and Steven L. Brunton},\n\t\ttitle = {PySINDy: A comprehensive Python package for robust sparse system identification},\n\t\tjournal = {Journal of Open Source Software}\n\t\t}\n    \n\n.. |RTD| image:: https://readthedocs.org/projects/derivative/badge/?version=latest\n   :target: https://derivative.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n  \n.. |LIC| image:: https://img.shields.io/badge/License-MIT-blue.svg\n   :target: https://derivative.readthedocs.io/en/latest/license.html\n   :alt: MIT License\n\n.. |PyPI| image:: https://badge.fury.io/py/derivative.svg\n    :target: https://pypi.org/project/derivative/\n\n.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6617446.svg\n   :target: https://doi.org/10.5281/zenodo.6617446\n\n.. |GithubCI| image:: https://github.com/andgoldschmidt/derivative/actions/workflows/push-test.yml/badge.svg\n    :target: https://github.com/andgoldschmidt/derivative/actions/workflows/push-test.yml\n\n',
     'author': 'Andy Goldschmidt',
     'author_email': 'andygold@uchicago.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/andgoldschmidt/derivative',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
+    'entry_points': entry_points,
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `derivative-0.6.0/PKG-INFO` & `derivative-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: derivative
-Version: 0.6.0
+Version: 0.6.1
 Summary: Numerical differentiation in python.
 Home-page: https://github.com/andgoldschmidt/derivative
 License: MIT
 Keywords: differentiation,derivative,gradient,prime
 Author: Andy Goldschmidt
 Author-email: andygold@uchicago.edu
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: dev
 Provides-Extra: docs
 Requires-Dist: ipykernel (>=5.2.1,<6.0.0); extra == "docs"
 Requires-Dist: jupyter_client (>=6.1.3,<7.0.0); extra == "docs"
 Requires-Dist: matplotlib (>=3.2.1,<4.0.0); extra == "docs"
 Requires-Dist: nbsphinx (>=0.6.1,<0.7.0); extra == "docs"
 Requires-Dist: numpy (>=1.18.3,<2.0.0)
 Requires-Dist: pytest (>=7,<8); extra == "dev"
 Requires-Dist: scikit-learn (>=1,<2)
 Requires-Dist: scipy (>=1.4.1,<2.0.0)
-Requires-Dist: sphinx (>=4.5,<5.0); extra == "docs"
-Requires-Dist: sphinx_rtd_theme (>=1,<2); extra == "docs"
+Requires-Dist: sphinx (>=5,<6); extra == "docs"
 Project-URL: Documentation, https://derivative.readthedocs.io/
 Project-URL: Repository, https://github.com/andgoldschmidt/derivative
 Description-Content-Type: text/x-rst
 
 |RTD| |PyPI| |Zenodo| |GithubCI| |LIC|
 
 Numerical differentiation of noisy time series data in python
@@ -85,18 +82,18 @@
     # 7. Kernel derivative with smoothing set to 1
     result7 = dxdt(x, t, kind="kernel", sigma=1, lmbd=.1, kernel="rbf")
 
 Contributors:
 -------------
 Thanks to the members of the community who have contributed!
 
-+-----------------------------------------------------------------+----------------------------------------------------------------------------------+
-|  `Jacob Stevens-Haas <https://github.com/Jacob-Stevens-Haas>`_  | Kalman derivatives `#12 <https://github.com/andgoldschmidt/derivative/pull/12>`_,|
-|								  | Kernel derivatives `#30 <https://github.com/andgoldschmidt/derivative/pull/30>`_ |  
-+-----------------------------------------------------------------+----------------------------------------------------------------------------------+
++-----------------------------------------------------------------+-----------------------------------------------------------------------------------+
+|`Jacob Stevens-Haas <https://github.com/Jacob-Stevens-Haas>`_    | Kalman derivatives `#12 <https://github.com/andgoldschmidt/derivative/pull/12>`_, |
+|                                                                 | and more!                                                                         |
++-----------------------------------------------------------------+-----------------------------------------------------------------------------------+
 
 
 References:
 -----------
 
 [1] Numerical differentiation of experimental data: local versus global methods- K. Ahnert and M. Abel
 
@@ -111,26 +108,26 @@
 ------------------
 The **derivative** package is a contribution to `PySINDy <https://github.com/dynamicslab/pysindy/>`_; this work has been published in the Journal of Open Source Software (JOSS). If you use **derivative** in your work, please cite it using the following reference:
 
 Kaptanoglu et al., (2022). PySINDy: A comprehensive Python package for robust sparse system identification. Journal of Open Source Software, 7(69), 3994, https://doi.org/10.21105/joss.03994
 
 .. code-block:: text
 
-      @article{kaptanoglu2022pysindy,
-  	doi = {10.21105/joss.03994},
-  	url = {https://doi.org/10.21105/joss.03994},
-  	year = {2022},
-  	publisher = {The Open Journal},
-  	volume = {7},
-  	number = {69},
-  	pages = {3994},
-  	author = {Alan A. Kaptanoglu and Brian M. de Silva and Urban Fasel and Kadierdan Kaheman and Andy J. Goldschmidt and Jared Callaham and Charles B. Delahunt and Zachary G. Nicolaou and Kathleen Champion and Jean-Christophe Loiseau and J. Nathan Kutz and Steven L. Brunton},
-  	title = {PySINDy: A comprehensive Python package for robust sparse system identification},
-  	journal = {Journal of Open Source Software}
-	}
+	@article{kaptanoglu2022pysindy,
+		doi = {10.21105/joss.03994},
+		url = {https://doi.org/10.21105/joss.03994},
+		year = {2022},
+		publisher = {The Open Journal},
+		volume = {7},
+		number = {69},
+		pages = {3994},
+		author = {Alan A. Kaptanoglu and Brian M. de Silva and Urban Fasel and Kadierdan Kaheman and Andy J. Goldschmidt and Jared Callaham and Charles B. Delahunt and Zachary G. Nicolaou and Kathleen Champion and Jean-Christophe Loiseau and J. Nathan Kutz and Steven L. Brunton},
+		title = {PySINDy: A comprehensive Python package for robust sparse system identification},
+		journal = {Journal of Open Source Software}
+		}
     
 
 .. |RTD| image:: https://readthedocs.org/projects/derivative/badge/?version=latest
    :target: https://derivative.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
   
 .. |LIC| image:: https://img.shields.io/badge/License-MIT-blue.svg
```

