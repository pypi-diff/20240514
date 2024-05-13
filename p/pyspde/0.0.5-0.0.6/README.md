# Comparing `tmp/pyspde-0.0.5.tar.gz` & `tmp/pyspde-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspde-0.0.5.tar", last modified: Wed Apr 24 06:42:15 2024, max compression
+gzip compressed data, was "pyspde-0.0.6.tar", last modified: Mon May 13 23:13:32 2024, max compression
```

## Comparing `pyspde-0.0.5.tar` & `pyspde-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 06:42:15.868251 pyspde-0.0.5/
--rw-rw-rw-   0        0        0     1085 2024-04-09 03:25:05.000000 pyspde-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1732 2024-04-24 06:42:15.867251 pyspde-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      927 2024-04-24 00:22:13.000000 pyspde-0.0.5/README.md
--rw-rw-rw-   0        0        0     1198 2024-04-24 06:42:10.000000 pyspde-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-24 06:42:15.868251 pyspde-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-24 06:42:15.852122 pyspde-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 06:42:15.858248 pyspde-0.0.5/src/pyspde/
--rw-rw-rw-   0        0        0       91 2024-04-24 00:34:35.000000 pyspde-0.0.5/src/pyspde/__init__.py
--rw-rw-rw-   0        0        0    10145 2024-04-24 05:12:51.000000 pyspde-0.0.5/src/pyspde/anisotropy.py
--rw-rw-rw-   0        0        0     4826 2024-04-24 06:29:51.000000 pyspde-0.0.5/src/pyspde/grid.py
--rw-rw-rw-   0        0        0     3606 2024-04-23 06:08:32.000000 pyspde-0.0.5/src/pyspde/neighbours.py
--rw-rw-rw-   0        0        0    10608 2024-04-23 06:10:05.000000 pyspde-0.0.5/src/pyspde/spde.py
--rw-rw-rw-   0        0        0     4908 2024-04-24 01:17:48.000000 pyspde-0.0.5/src/pyspde/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 06:42:15.867251 pyspde-0.0.5/src/pyspde.egg-info/
--rw-rw-rw-   0        0        0     1732 2024-04-24 06:42:15.000000 pyspde-0.0.5/src/pyspde.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-04-24 06:42:15.000000 pyspde-0.0.5/src/pyspde.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 06:42:15.000000 pyspde-0.0.5/src/pyspde.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-24 06:42:15.000000 pyspde-0.0.5/src/pyspde.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 06:42:15.000000 pyspde-0.0.5/src/pyspde.egg-info/top_level.txt
+drwxr-xr-x   0 wslubuntu  (1000) wslubuntu  (1000)        0 2024-05-13 23:13:32.313711 pyspde-0.0.6/
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)     1064 2024-04-26 01:12:21.000000 pyspde-0.0.6/LICENSE
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)     1818 2024-05-13 23:13:32.313711 pyspde-0.0.6/PKG-INFO
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)     1031 2024-04-26 08:58:36.000000 pyspde-0.0.6/README.md
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)     1162 2024-05-13 22:52:47.000000 pyspde-0.0.6/pyproject.toml
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)       38 2024-05-13 23:13:32.313711 pyspde-0.0.6/setup.cfg
+drwxr-xr-x   0 wslubuntu  (1000) wslubuntu  (1000)        0 2024-05-13 23:13:32.313711 pyspde-0.0.6/src/
+drwxr-xr-x   0 wslubuntu  (1000) wslubuntu  (1000)        0 2024-05-13 23:13:32.313711 pyspde-0.0.6/src/pyspde/
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)       87 2024-04-26 08:55:51.000000 pyspde-0.0.6/src/pyspde/__init__.py
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)     9807 2024-04-26 08:55:51.000000 pyspde-0.0.6/src/pyspde/anisotropy.py
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)     4665 2024-04-26 08:55:51.000000 pyspde-0.0.6/src/pyspde/grid.py
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)     3487 2024-04-26 01:12:21.000000 pyspde-0.0.6/src/pyspde/neighbours.py
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)    10342 2024-05-02 00:53:15.000000 pyspde-0.0.6/src/pyspde/spde.py
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)     4708 2024-04-26 08:55:51.000000 pyspde-0.0.6/src/pyspde/utils.py
+drwxr-xr-x   0 wslubuntu  (1000) wslubuntu  (1000)        0 2024-05-13 23:13:32.313711 pyspde-0.0.6/src/pyspde.egg-info/
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)     1818 2024-05-13 23:13:32.000000 pyspde-0.0.6/src/pyspde.egg-info/PKG-INFO
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)      332 2024-05-13 23:13:32.000000 pyspde-0.0.6/src/pyspde.egg-info/SOURCES.txt
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)        1 2024-05-13 23:13:32.000000 pyspde-0.0.6/src/pyspde.egg-info/dependency_links.txt
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)       45 2024-05-13 23:13:32.000000 pyspde-0.0.6/src/pyspde.egg-info/requires.txt
+-rw-r--r--   0 wslubuntu  (1000) wslubuntu  (1000)        7 2024-05-13 23:13:32.000000 pyspde-0.0.6/src/pyspde.egg-info/top_level.txt
```

### Comparing `pyspde-0.0.5/LICENSE` & `pyspde-0.0.6/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 M1nerAI
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 M1nerAI
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pyspde-0.0.5/PKG-INFO` & `pyspde-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-Metadata-Version: 2.1
-Name: pyspde
-Version: 0.0.5
-Summary: PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs)
-Author-email: Esteban Jimenez <ejimenez@minerai.com.au>
-Project-URL: Homepage, https://github.com/M1nerAI/pyspde
-Project-URL: Issues, https://github.com/M1nerAI/pyspde/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: scipy
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: scikit-sparse==0.4.12
-
-# PySPDE
-
-PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs):
-
-$$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}W(x) \quad x \in \mathbb{R}^2
-$$
-
-The theory is proposed in Fuglstad (2014).
-
-## Instalation
-
-On Debian/Ubuntu systems:
-```
-sudo apt-get install libsuitesparse-dev
-pip install pyspde
-```
-
-On Windows systems:
-```
-conda install -c conda-forge suitesparse
-pip install pyspde
-```
-
-## Basic Usage
-
-Imports:
-```
-from pyspde import anisotropy, Grid, Spde
-```
-
-Define the anisotropy and the grid:
-```
-atpy = anisotropy_from_svg(r'assets/anicline.svg', beta=10, gamma=0.1)
-grid = Grid(nx=200, ny=100, anisotropy=atpy)
-```
-
-Define SPDE and Simulate:
-```
-sp = Spde(grid, sigma=1, a=25)
-Z = sp.simulate()
-```
+Metadata-Version: 2.1
+Name: pyspde
+Version: 0.0.6
+Summary: PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs)
+Author-email: Esteban Jimenez <ejimenez@minerai.com.au>
+Project-URL: Homepage, https://github.com/M1nerAI/pyspde
+Project-URL: Issues, https://github.com/M1nerAI/pyspde/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: scipy
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: scikit-sparse==0.4.12
+
+# PySPDE
+
+PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs):
+
+$$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}(x)W(x) \quad x \in \mathbb{R}^2
+$$
+
+The theory is proposed in Fuglstad (2014).
+
+## Instalation
+
+On Debian/Ubuntu systems:
+```
+sudo apt-get install libsuitesparse-dev
+pip install pyspde
+```
+
+On Windows systems:
+```
+conda install -c conda-forge suitesparse
+pip install pyspde
+```
+
+## Basic Usage
+
+Imports:
+```
+from pyspde import anisotropy, Grid, Spde, anisotropy_from_svg
+```
+
+Define the anisotropy and the grid:
+```
+atpy = anisotropy_from_svg(r'assets/anticline.svg', beta=50, gamma=0.5)
+grid = Grid(nx=400, ny=200, anisotropy=atpy)
+```
+
+Define SPDE and Simulate:
+```
+sp = Spde(grid, sigma=1, a=50)
+Z = sp.simulate(seed=0)
+```
+
+![alt text](https://onedrive.live.com/embed?resid=a94fce3415a299a1%2117697&authkey=%21AMG50D19mGNfdyY&width=660)
```

### Comparing `pyspde-0.0.5/pyproject.toml` & `pyspde-0.0.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "pyspde"
-version = "0.0.5"
-authors = [
-  { name="Esteban Jimenez", email="ejimenez@minerai.com.au" },
-]
-description = "PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs)"
-readme = "README.md"
-requires-python = ">=3.11"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = ["scipy", "numpy", "matplotlib", "scikit-sparse==0.4.12"]
-
-[project.urls]
-Homepage = "https://github.com/M1nerAI/pyspde"
-Issues = "https://github.com/M1nerAI/pyspde/issues"
-
-
-[tool.ruff.lint]
-select = ["ALL"]
-#I001 unsorted-imports
-#ANN101 missing-type-self
-#Q000 Double quotes instead of single quotes
-#PLR0913 toomany arguments
-#RET505 unnecesary return after else
-#N806 non-lowercase-variable-in-function 
-extend-ignore = ["I001", "ANN101", "Q000", "PLR0913", "RET505", "N806"]
-
-[tool.ruff]
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "pyspde"
+version = "0.0.6"
+authors = [
+  { name="Esteban Jimenez", email="ejimenez@minerai.com.au" },
+]
+description = "PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs)"
+readme = "README.md"
+requires-python = ">=3.11"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = ["scipy", "numpy", "matplotlib", "scikit-sparse==0.4.12"]
+
+[project.urls]
+Homepage = "https://github.com/M1nerAI/pyspde"
+Issues = "https://github.com/M1nerAI/pyspde/issues"
+
+
+[tool.ruff.lint]
+select = ["ALL"]
+#I001 unsorted-imports
+#ANN101 missing-type-self
+#Q000 Double quotes instead of single quotes
+#PLR0913 toomany arguments
+#RET505 unnecesary return after else
+#N806 non-lowercase-variable-in-function 
+extend-ignore = ["I001", "ANN101", "Q000", "PLR0913", "RET505", "N806"]
+
+[tool.ruff]
 line-length = 79
```

### Comparing `pyspde-0.0.5/src/pyspde/anisotropy.py` & `pyspde-0.0.6/src/pyspde/anisotropy.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,338 +1,338 @@
-import re
-
-import numpy as np
-import matplotlib.pyplot as plt
-from matplotlib.axes import Axes
-import xml.etree.ElementTree as Et
-from matplotlib.figure import Figure
-
-from .utils import get_inkscape_namespace, get_inkscape_transform
-
-__all__ = ['Anisotropy', 'anisotropy_from_svg', 'anisotropy_stationary']
-
-class Anisotropy:
-    """Represents an anisotropy object.
-
-    Attributes
-    ----------
-        _x (np.ndarray): X-coordinates of vectors.
-        _y (np.ndarray): Y-coordinates of vectors.
-        _u (np.ndarray): Horizontal components of vectors.
-        _v (np.ndarray): Vertical components of vectors.
-        width (float): Width extent of the anisotropy.
-        height (float): Height extent of the anisotropy.
-        H (np.ndarray): Anisotropy tensor.
-        V (np.ndarray): Vector field tensor.
-        beta (float): Anisotropic local effect coefficient.
-        gamma (float): Isotropic baseline effect coeficient.
-        dtype (type): Data type for the fields tensors.
-
-    """
-
-    def __init__(self, x_u: np.ndarray, beta: float, gamma: float,
-                 width: float = None, height: float = None, k: int = 3,
-                 dtype: type = np.float64, *, scale: bool = True) -> None:
-        """Initialize an Anisotropy object.
-
-        Args:
-        ----
-            x_u (np.ndarray): Anisotropy data points of shape (p, 4). Each row
-            is composed by  (x, y, u, v) where (x, y) coordinates with (u, v)
-            directions.
-            beta (float): Anisotropic local effect coefficient.
-            gamma (float): Isotropic baseline effect coeficient.
-            width (float): Width extent of the anisotropy.
-            height (float): Height extent of the anisotropy.
-            k (int): No of neighbours to consider during interpolation.
-            dtype (type): Data type for the fields tensors.
-            Defaults to np.float32.
-            scale (bool, optional): Whether to scale the anisotropy field to
-            match grid dimensions. Defaults to True.
-
-        """
-        # No Interpolation
-        self._x = x_u[:,0].astype(dtype)
-        self._y = x_u[:,1].astype(dtype)
-        self._u = x_u[:,2].astype(dtype)
-        self._v = x_u[:,3].astype(dtype)
-
-        self.width = x_u[:, 0].max() - x_u[:, 0].min() if width is None \
-                     else width
-
-        self.height = x_u[:, 1].max() - x_u[:, 1].min() if height is None \
-                     else height
-
-        # Interpolated
-        self.H = None
-        self.V = None
-
-        # Params
-        self.beta = beta
-        self.gamma = gamma
-        self.dtype = dtype
-        self.scale = scale
-        self.k = k
-
-    @property
-    def x(self) -> np.ndarray:
-        """Get the X-coordinates of vectors, considering interpolation.
-
-        Returns
-        -------
-            np.ndarray: X-coordinates.
-
-        """
-        if self.V is None:
-            return self._x
-        else:
-            j = np.indices(self.V.shape)[1,:,:,0]
-            return j.reshape(-1)
-
-    @property
-    def y(self) -> np.ndarray:
-        """Get the Y-coordinates of vectors, considering interpolation.
-
-        Returns
-        -------
-            np.ndarray: Y-coordinates.
-
-        """
-        if self.V is None:
-            return self._y
-        else:
-            i = np.indices(self.V.shape)[0,:,:,0]
-            return i.reshape(-1)
-
-    @property
-    def u(self) -> np.ndarray:
-        """Get the horizontal components of vectors, considering interpolation.
-
-        Returns
-        -------
-            np.ndarray: Horizontal components.
-
-        """
-        if self.V is None:
-            return self._u
-        else:
-            return self.V[:,:,1].reshape(-1)
-
-    @property
-    def v(self) -> np.ndarray:
-        """Get the vertical components of vectors, considering interpolation.
-
-        Returns
-        -------
-            np.ndarray: Vertical components.
-
-        """
-        if self.V is None:
-            return self._v
-        else:
-            return self.V[:,:,0].reshape(-1)
-
-
-    def plot(self, fig: Figure = None, ax: Axes = None, *, show: bool = True,
-             ) -> Figure:
-        """Plot the vectors.
-
-        Args:
-        ----
-            fig (Figure, optional): Matplotlib Figure object to use for
-            plotting. Defaults to None.
-            ax (Axes, optional): Matplotlib Axes object to use for plotting.
-            Defaults to None.
-            show (bool, optional): Whether to display the plot. Defaults to
-            True.
-
-        Returns:
-        -------
-            Figure: Matplotlib Figure object.
-
-        """
-        if (fig is None) & (ax is None):
-            fig, ax = plt.subplots()
-            ax.set_aspect('equal')
-            ax.invert_yaxis()
-
-        ax.quiver(self.x, self.y, self.u, self.v, angles='xy')
-
-        if show:
-            fig.show()
-
-        return fig
-
-    def check_positiveness(self) -> np.ndarray:
-        """Check if all the matrices in the `H` attribute are positive definite.
-
-        Returns:
-        -------
-            positiveness (ndarray):
-                A boolean array of shape `(ny_, nx_)` where `ny_` and `nx_`
-                are the number of rows and columns in the `H` attribute
-                respectively.
-                It indicates whether each matrix in `H` is positive definite
-                or not.
-
-        """
-        nx_ = self.H.shape[1]
-        ny_ = self.H.shape[0]
-
-        positiveness = np.zeros((ny_, nx_),dtype=bool)
-
-        for j in range(nx_):
-            for i in range(ny_):
-                x = self.H[i, j, :, :]
-                positiveness[i, j] = np.all(np.linalg.eigvals(x) > 0)
-
-        return positiveness
-
-    def check_differenciable(self, dx: int, dy: int) -> np.ndarray:
-        """Check if H is differenciable.
-
-        Parameters
-        ----------
-        dx : int
-            The increment in the x-direction.
-        dy : int
-            The increment in the y-direction.
-
-        Returns
-        -------
-        ndarray
-            A 4D array representing the partial derivatives of H with respect
-            to x and y.
-
-        """
-        nx_ = self.H.shape[1]
-        ny_ = self.H.shape[0]
-
-        differenciable = np.zeros((ny_, nx_, 2, 2))
-
-        for j in range(1,nx_-1):
-            for i in range(1, ny_ - 1):
-
-                dh_dy = (self.H[i + 1, j, :, :] - self.H[i - 1, j, :, :]
-                         ) / (2 * dy)
-                dh_dx = (self.H[i, j + 1, :, :] - self.H[i , j - 1, :, :]
-                         ) / (2 * dx)
-
-                dh00_dy = dh_dy[0, 0]
-                dh01_dy = dh_dy[0, 1]
-                dh11_dx = dh_dx[1, 1]
-                dh10_dx = dh_dx[1, 0]
-
-
-                differenciable[i, j, 0, 0] = dh00_dy
-                differenciable[i, j, 0, 1] = dh01_dy
-                differenciable[i, j, 1, 1] = dh11_dx
-                differenciable[i, j, 1, 0] = dh10_dx
-
-        return differenciable
-
-def anisotropy_from_svg(path: str, beta: float, gamma: float,
-                        norm_type: str = 'norm', k: int = 3) -> Anisotropy:
-    """Create an Anisotropy object from an SVG file.
-
-    Args:
-    ----
-        path (str): Path to the SVG file.
-        beta (float): Beta parameter.
-        gamma (float): Gamma parameter.
-        norm_type (str, optional): Type of normalization. Defaults to 'norm'.
-        k (int, optional): No of neighbours to consider when interpolating.
-        Defaults to 3.
-
-    Returns:
-    -------
-        Anisotropy: An Anisotropy object.
-
-    """
-    tree = Et.parse(path)
-    root = tree.getroot()
-
-    xmlns = get_inkscape_namespace(root)
-    tfm = get_inkscape_transform(root, xmlns)
-
-    view_box = root.attrib['viewBox']
-    view_box = re.findall(r'(-?[\d]+[\.]?[\d]*)', view_box)
-    _, _, width, height = (float(i) for i in view_box)
-
-    P = []
-
-    # Remove defitinions to skip style 'path' elements, like arrows heads.
-    defs = next(root.iter(f'{xmlns}defs'))
-    root.remove(defs)
-
-    for child in root.iter(f'{xmlns}path'):
-
-        values = child.attrib['d'][2:]
-        style = child.attrib['d'][0]
-
-        p0, p1 = values.split(' ')
-
-        p0 = p0.split(',')
-        p1 = p1.split(',')
-
-        p0 = [float(p0[0]), float(p0[1])]
-        p1 = [float(p1[0]) , float(p1[1])]
-
-        # m style is incremental / M style is absolute
-        if style == 'M':
-            p1 = [p1[0] - p0[0], p1[1] - p0[1]]
-
-        # Flip anchor point (p0) and incremental point (p1)
-        p0[1] =  p0[1]
-        p1[1] = p1[1]
-
-        P.append([p0[0], p0[1], p1[0], p1[1]])
-
-    P = np.asarray(P)
-
-    x = P[:,:2] +  tfm
-    u = P[:,2:]
-
-    norm = (u**2).sum(axis=1)**0.5
-    if norm_type == 'min':
-        min_norm = (norm).min()
-        u = u/(min_norm)
-    elif norm_type == 'max':
-        max_norm = (norm).max()
-        u = u/(max_norm)
-    elif norm_type == 'norm':
-        u = u/norm[:, np.newaxis]
-    else:
-        msg = f'Unknown norm_type = "{norm_type}"'
-        raise ValueError(msg)
-
-    x_u = np.column_stack((x,u))
-
-    return Anisotropy(x_u, beta, gamma, width,
-                      height, k)
-
-
-def anisotropy_stationary(theta: float, gamma: float, beta: float,
-                          ) -> Anisotropy:
-    """Create an Anisotropy stationary anisotrpy from an angle.
-
-    Parameters
-    ----------
-    theta : float
-        The angle in degrees at which the anisotropy pattern is oriented.
-    gamma : float
-        The isotropic baseline effect coefficient.
-    beta : float
-        The anisotropic local effect coefficient.
-
-    Returns
-    -------
-    Anisotropy
-        An Anisotropy object representing the stationary anisotropy pattern.
-
-    """
-    theta = np.radians(theta)
-
-    v =  np.asarray([- np.sin(theta),  np.cos(theta)])
-    x_u  = np.asarray([[0,0,v[0],v[1]]])
-
-    return Anisotropy(x_u, beta, gamma, scale=False)
+import re
+
+import numpy as np
+import matplotlib.pyplot as plt
+from matplotlib.axes import Axes
+import xml.etree.ElementTree as Et
+from matplotlib.figure import Figure
+
+from .utils import get_inkscape_namespace, get_inkscape_transform
+
+__all__ = ['Anisotropy', 'anisotropy_from_svg', 'anisotropy_stationary']
+
+class Anisotropy:
+    """Represents an anisotropy object.
+
+    Attributes
+    ----------
+        _x (np.ndarray): X-coordinates of vectors.
+        _y (np.ndarray): Y-coordinates of vectors.
+        _u (np.ndarray): Horizontal components of vectors.
+        _v (np.ndarray): Vertical components of vectors.
+        width (float): Width extent of the anisotropy.
+        height (float): Height extent of the anisotropy.
+        H (np.ndarray): Anisotropy tensor.
+        V (np.ndarray): Vector field tensor.
+        beta (float): Anisotropic local effect coefficient.
+        gamma (float): Isotropic baseline effect coeficient.
+        dtype (type): Data type for the fields tensors.
+
+    """
+
+    def __init__(self, x_u: np.ndarray, beta: float, gamma: float,
+                 width: float = None, height: float = None, k: int = 3,
+                 dtype: type = np.float64, *, scale: bool = True) -> None:
+        """Initialize an Anisotropy object.
+
+        Args:
+        ----
+            x_u (np.ndarray): Anisotropy data points of shape (p, 4). Each row
+            is composed by  (x, y, u, v) where (x, y) coordinates with (u, v)
+            directions.
+            beta (float): Anisotropic local effect coefficient.
+            gamma (float): Isotropic baseline effect coeficient.
+            width (float): Width extent of the anisotropy.
+            height (float): Height extent of the anisotropy.
+            k (int): No of neighbours to consider during interpolation.
+            dtype (type): Data type for the fields tensors.
+            Defaults to np.float32.
+            scale (bool, optional): Whether to scale the anisotropy field to
+            match grid dimensions. Defaults to True.
+
+        """
+        # No Interpolation
+        self._x = x_u[:,0].astype(dtype)
+        self._y = x_u[:,1].astype(dtype)
+        self._u = x_u[:,2].astype(dtype)
+        self._v = x_u[:,3].astype(dtype)
+
+        self.width = x_u[:, 0].max() - x_u[:, 0].min() if width is None \
+                     else width
+
+        self.height = x_u[:, 1].max() - x_u[:, 1].min() if height is None \
+                     else height
+
+        # Interpolated
+        self.H = None
+        self.V = None
+
+        # Params
+        self.beta = beta
+        self.gamma = gamma
+        self.dtype = dtype
+        self.scale = scale
+        self.k = k
+
+    @property
+    def x(self) -> np.ndarray:
+        """Get the X-coordinates of vectors, considering interpolation.
+
+        Returns
+        -------
+            np.ndarray: X-coordinates.
+
+        """
+        if self.V is None:
+            return self._x
+        else:
+            j = np.indices(self.V.shape)[1,:,:,0]
+            return j.reshape(-1)
+
+    @property
+    def y(self) -> np.ndarray:
+        """Get the Y-coordinates of vectors, considering interpolation.
+
+        Returns
+        -------
+            np.ndarray: Y-coordinates.
+
+        """
+        if self.V is None:
+            return self._y
+        else:
+            i = np.indices(self.V.shape)[0,:,:,0]
+            return i.reshape(-1)
+
+    @property
+    def u(self) -> np.ndarray:
+        """Get the horizontal components of vectors, considering interpolation.
+
+        Returns
+        -------
+            np.ndarray: Horizontal components.
+
+        """
+        if self.V is None:
+            return self._u
+        else:
+            return self.V[:,:,1].reshape(-1)
+
+    @property
+    def v(self) -> np.ndarray:
+        """Get the vertical components of vectors, considering interpolation.
+
+        Returns
+        -------
+            np.ndarray: Vertical components.
+
+        """
+        if self.V is None:
+            return self._v
+        else:
+            return self.V[:,:,0].reshape(-1)
+
+
+    def plot(self, fig: Figure = None, ax: Axes = None, *, show: bool = True,
+             ) -> Figure:
+        """Plot the vectors.
+
+        Args:
+        ----
+            fig (Figure, optional): Matplotlib Figure object to use for
+            plotting. Defaults to None.
+            ax (Axes, optional): Matplotlib Axes object to use for plotting.
+            Defaults to None.
+            show (bool, optional): Whether to display the plot. Defaults to
+            True.
+
+        Returns:
+        -------
+            Figure: Matplotlib Figure object.
+
+        """
+        if (fig is None) & (ax is None):
+            fig, ax = plt.subplots()
+            ax.set_aspect('equal')
+            ax.invert_yaxis()
+
+        ax.quiver(self.x, self.y, self.u, self.v, angles='xy')
+
+        if show:
+            fig.show()
+
+        return fig
+
+    def check_positiveness(self) -> np.ndarray:
+        """Check if all the matrices in the `H` attribute are positive definite.
+
+        Returns:
+        -------
+            positiveness (ndarray):
+                A boolean array of shape `(ny_, nx_)` where `ny_` and `nx_`
+                are the number of rows and columns in the `H` attribute
+                respectively.
+                It indicates whether each matrix in `H` is positive definite
+                or not.
+
+        """
+        nx_ = self.H.shape[1]
+        ny_ = self.H.shape[0]
+
+        positiveness = np.zeros((ny_, nx_),dtype=bool)
+
+        for j in range(nx_):
+            for i in range(ny_):
+                x = self.H[i, j, :, :]
+                positiveness[i, j] = np.all(np.linalg.eigvals(x) > 0)
+
+        return positiveness
+
+    def check_differenciable(self, dx: int, dy: int) -> np.ndarray:
+        """Check if H is differenciable.
+
+        Parameters
+        ----------
+        dx : int
+            The increment in the x-direction.
+        dy : int
+            The increment in the y-direction.
+
+        Returns
+        -------
+        ndarray
+            A 4D array representing the partial derivatives of H with respect
+            to x and y.
+
+        """
+        nx_ = self.H.shape[1]
+        ny_ = self.H.shape[0]
+
+        differenciable = np.zeros((ny_, nx_, 2, 2))
+
+        for j in range(1,nx_-1):
+            for i in range(1, ny_ - 1):
+
+                dh_dy = (self.H[i + 1, j, :, :] - self.H[i - 1, j, :, :]
+                         ) / (2 * dy)
+                dh_dx = (self.H[i, j + 1, :, :] - self.H[i , j - 1, :, :]
+                         ) / (2 * dx)
+
+                dh00_dy = dh_dy[0, 0]
+                dh01_dy = dh_dy[0, 1]
+                dh11_dx = dh_dx[1, 1]
+                dh10_dx = dh_dx[1, 0]
+
+
+                differenciable[i, j, 0, 0] = dh00_dy
+                differenciable[i, j, 0, 1] = dh01_dy
+                differenciable[i, j, 1, 1] = dh11_dx
+                differenciable[i, j, 1, 0] = dh10_dx
+
+        return differenciable
+
+def anisotropy_from_svg(path: str, beta: float, gamma: float,
+                        norm_type: str = 'norm', k: int = 3) -> Anisotropy:
+    """Create an Anisotropy object from an SVG file.
+
+    Args:
+    ----
+        path (str): Path to the SVG file.
+        beta (float): Beta parameter.
+        gamma (float): Gamma parameter.
+        norm_type (str, optional): Type of normalization. Defaults to 'norm'.
+        k (int, optional): No of neighbours to consider when interpolating.
+        Defaults to 3.
+
+    Returns:
+    -------
+        Anisotropy: An Anisotropy object.
+
+    """
+    tree = Et.parse(path)
+    root = tree.getroot()
+
+    xmlns = get_inkscape_namespace(root)
+    tfm = get_inkscape_transform(root, xmlns)
+
+    view_box = root.attrib['viewBox']
+    view_box = re.findall(r'(-?[\d]+[\.]?[\d]*)', view_box)
+    _, _, width, height = (float(i) for i in view_box)
+
+    P = []
+
+    # Remove defitinions to skip style 'path' elements, like arrows heads.
+    defs = next(root.iter(f'{xmlns}defs'))
+    root.remove(defs)
+
+    for child in root.iter(f'{xmlns}path'):
+
+        values = child.attrib['d'][2:]
+        style = child.attrib['d'][0]
+
+        p0, p1 = values.split(' ')
+
+        p0 = p0.split(',')
+        p1 = p1.split(',')
+
+        p0 = [float(p0[0]), float(p0[1])]
+        p1 = [float(p1[0]) , float(p1[1])]
+
+        # m style is incremental / M style is absolute
+        if style == 'M':
+            p1 = [p1[0] - p0[0], p1[1] - p0[1]]
+
+        # Flip anchor point (p0) and incremental point (p1)
+        p0[1] =  p0[1]
+        p1[1] = p1[1]
+
+        P.append([p0[0], p0[1], p1[0], p1[1]])
+
+    P = np.asarray(P)
+
+    x = P[:,:2] +  tfm
+    u = P[:,2:]
+
+    norm = (u**2).sum(axis=1)**0.5
+    if norm_type == 'min':
+        min_norm = (norm).min()
+        u = u/(min_norm)
+    elif norm_type == 'max':
+        max_norm = (norm).max()
+        u = u/(max_norm)
+    elif norm_type == 'norm':
+        u = u/norm[:, np.newaxis]
+    else:
+        msg = f'Unknown norm_type = "{norm_type}"'
+        raise ValueError(msg)
+
+    x_u = np.column_stack((x,u))
+
+    return Anisotropy(x_u, beta, gamma, width,
+                      height, k)
+
+
+def anisotropy_stationary(theta: float, gamma: float, beta: float,
+                          ) -> Anisotropy:
+    """Create an Anisotropy stationary anisotrpy from an angle.
+
+    Parameters
+    ----------
+    theta : float
+        The angle in degrees at which the anisotropy pattern is oriented.
+    gamma : float
+        The isotropic baseline effect coefficient.
+    beta : float
+        The anisotropic local effect coefficient.
+
+    Returns
+    -------
+    Anisotropy
+        An Anisotropy object representing the stationary anisotropy pattern.
+
+    """
+    theta = np.radians(theta)
+
+    v =  np.asarray([- np.sin(theta),  np.cos(theta)])
+    x_u  = np.asarray([[0,0,v[0],v[1]]])
+
+    return Anisotropy(x_u, beta, gamma, scale=False)
```

### Comparing `pyspde-0.0.5/src/pyspde/grid.py` & `pyspde-0.0.6/src/pyspde/grid.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-
-from __future__ import annotations
-from typing import TYPE_CHECKING
-import warnings
-
-import numpy as np
-from  scipy.spatial import  KDTree
-
-if TYPE_CHECKING:
-    from .anisotropy import Anisotropy
-
-__all__ = ['Grid']
-
-class Grid:
-    """Grid class representing a computational grid for anisotropic simulations.
-
-    Attributes
-    ----------
-        nx (int): Number of grid points in the x-direction.
-        ny (int): Number of grid points in the y-direction.
-        dx (float): Spacing between grid points in the x-direction.
-        dy (float): Spacing between grid points in the y-direction.
-        anisotropy (Anisotropy): An Anisotropy object representing the
-        anisotropy field.
-        padx (int): Padding in the x-direction.
-        pady (int): Padding in the y-direction.
-        _nx (int): Total number of grid points including padding in the
-        x-direction.
-        _ny (int): Total number of grid points including padding in the
-        y-direction.
-
-    """
-
-    _padx_pct = 15
-    _pady_pct = 15
-
-    def __init__(self, nx: int, ny: int, anisotropy: Anisotropy, dx: float=1,
-                 dy: float=1, padx: None | int = None, pady: None | int = None,
-                 ) -> None:
-        """Initialize a Grid object.
-
-        Args:
-        ----
-            nx (int): Number of grid points in the x-direction.
-            ny (int): Number of grid points in the y-direction.
-            dx (float): Spacing between grid points in the x-direction.
-            dy (float): Spacing between grid points in the y-direction.
-            anisotropy (Anisotropy): An Anisotropy object representing the
-            anisotropy field.
-            padx (None | int, optional): Padding in the x-direction. Defaults
-            to None.
-            pady (None | int, optional): Padding in the y-direction. Defaults
-            to None.
-
-        """
-        self.nx = nx
-        self.ny = ny
-        self.dx = dx
-        self.dy = dy
-        self.anisotropy = anisotropy
-
-        # Add Padding
-        if padx is None:
-            self.padx = int(np.ceil(self._padx_pct / 100 * nx))
-        else:
-            self.padx = padx
-
-        if pady is None:
-            self.pady = int(np.ceil(self._pady_pct / 100 * ny))
-        else:
-            self.pady = pady
-
-        self._nx = nx + 2 * self.padx
-        self._ny = ny + 2 * self.pady
-
-        self.intrp_anisotropy()
-
-
-    def intrp_anisotropy(self) ->  None:
-        """Interpolate the anisotropy field onto the grid.
-
-        Args:
-        ----
-            k (int, optional): Number of nearest neighbors to consider in
-            interpolation. Defaults to 3.
-
-
-        """
-        anis = self.anisotropy
-        k = min(anis.k,  len(anis.x))
-
-
-        if anis.scale:
-            scale_x = self.nx * self.dx / anis.width
-            scale_y = self.ny * self.dy / anis.height
-
-            # TODO(ejimenez): scale u,v
-        else:
-            scale_x = 1
-            scale_y = 1
-
-        x = (anis.x * scale_x) + self.padx
-        y = (anis.y * scale_y) + self.pady
-
-       #import matplotlib.pyplot as plt
-       #plt.imshow(np.random.rand(self._ny, self._nx))
-       #plt.scatter(x, y, c=anis.u, cmap='jet')
-
-       #plt.show()
-       #breakpoint()
-
-        X = np.column_stack((x, y))
-        U = np.column_stack((anis.u, anis.v))
-
-        # 1D
-        grid = np.meshgrid(np.arange(self._nx) * self.dx,
-                           np.arange(self._ny) * self.dy)
-
-        # 2D
-        grid = np.column_stack((grid[0].reshape(-1), grid[1].reshape(-1)))
-
-        V = np.zeros(grid.shape, dtype=anis.dtype)
-        tree = KDTree(X)
-
-        dists, idxs = tree.query(grid, k=k)
-
-        if k == 1:
-            dists = dists[:, np.newaxis]
-            idxs = idxs[:, np.newaxis]
-
-        warnings.filterwarnings("error")
-
-        for i,(dist, idx) in enumerate(zip(dists, idxs)):
-
-            try:
-                inv_dist = dist**(-0.25)
-                inv_dist = inv_dist/inv_dist.sum()
-            except RuntimeWarning:
-
-                inv_dist = np.zeros(k, dtype=anis.dtype)
-                inv_dist[np.argmin(dist)] = 1 
-
-
-            V[i, :] = (U[idx, :] * inv_dist[:, np.newaxis]).sum(axis=0)
-
-        warnings.resetwarnings()
-
-        V = V.reshape(self._ny, self._nx , 2)[:,:,::-1]
-        H = np.zeros((self._ny,self._nx, 2, 2), dtype=anis.dtype)
-        I = np.eye(2, dtype=anis.dtype)
-
-        for i in range(self._ny):
-            for j in range(self._nx):
-                H[i, j, :, :] = anis.gamma*I +\
-                                anis.beta*(V[i, j][:,np.newaxis] @ \
-                                           V[i, j][np.newaxis,:] )
-
-        anis.H = H
-        anis.V = V
-
-
+
+from __future__ import annotations
+from typing import TYPE_CHECKING
+import warnings
+
+import numpy as np
+from  scipy.spatial import  KDTree
+
+if TYPE_CHECKING:
+    from .anisotropy import Anisotropy
+
+__all__ = ['Grid']
+
+class Grid:
+    """Grid class representing a computational grid for anisotropic simulations.
+
+    Attributes
+    ----------
+        nx (int): Number of grid points in the x-direction.
+        ny (int): Number of grid points in the y-direction.
+        dx (float): Spacing between grid points in the x-direction.
+        dy (float): Spacing between grid points in the y-direction.
+        anisotropy (Anisotropy): An Anisotropy object representing the
+        anisotropy field.
+        padx (int): Padding in the x-direction.
+        pady (int): Padding in the y-direction.
+        _nx (int): Total number of grid points including padding in the
+        x-direction.
+        _ny (int): Total number of grid points including padding in the
+        y-direction.
+
+    """
+
+    _padx_pct = 15
+    _pady_pct = 15
+
+    def __init__(self, nx: int, ny: int, anisotropy: Anisotropy, dx: float=1,
+                 dy: float=1, padx: None | int = None, pady: None | int = None,
+                 ) -> None:
+        """Initialize a Grid object.
+
+        Args:
+        ----
+            nx (int): Number of grid points in the x-direction.
+            ny (int): Number of grid points in the y-direction.
+            dx (float): Spacing between grid points in the x-direction.
+            dy (float): Spacing between grid points in the y-direction.
+            anisotropy (Anisotropy): An Anisotropy object representing the
+            anisotropy field.
+            padx (None | int, optional): Padding in the x-direction. Defaults
+            to None.
+            pady (None | int, optional): Padding in the y-direction. Defaults
+            to None.
+
+        """
+        self.nx = nx
+        self.ny = ny
+        self.dx = dx
+        self.dy = dy
+        self.anisotropy = anisotropy
+
+        # Add Padding
+        if padx is None:
+            self.padx = int(np.ceil(self._padx_pct / 100 * nx))
+        else:
+            self.padx = padx
+
+        if pady is None:
+            self.pady = int(np.ceil(self._pady_pct / 100 * ny))
+        else:
+            self.pady = pady
+
+        self._nx = nx + 2 * self.padx
+        self._ny = ny + 2 * self.pady
+
+        self.intrp_anisotropy()
+
+
+    def intrp_anisotropy(self) ->  None:
+        """Interpolate the anisotropy field onto the grid.
+
+        Args:
+        ----
+            k (int, optional): Number of nearest neighbors to consider in
+            interpolation. Defaults to 3.
+
+
+        """
+        anis = self.anisotropy
+        k = min(anis.k,  len(anis.x))
+
+
+        if anis.scale:
+            scale_x = self.nx * self.dx / anis.width
+            scale_y = self.ny * self.dy / anis.height
+
+            # TODO(ejimenez): scale u,v
+        else:
+            scale_x = 1
+            scale_y = 1
+
+        x = (anis.x * scale_x) + self.padx
+        y = (anis.y * scale_y) + self.pady
+
+       #import matplotlib.pyplot as plt
+       #plt.imshow(np.random.rand(self._ny, self._nx))
+       #plt.scatter(x, y, c=anis.u, cmap='jet')
+
+       #plt.show()
+       #breakpoint()
+
+        X = np.column_stack((x, y))
+        U = np.column_stack((anis.u, anis.v))
+
+        # 1D
+        grid = np.meshgrid(np.arange(self._nx) * self.dx,
+                           np.arange(self._ny) * self.dy)
+
+        # 2D
+        grid = np.column_stack((grid[0].reshape(-1), grid[1].reshape(-1)))
+
+        V = np.zeros(grid.shape, dtype=anis.dtype)
+        tree = KDTree(X)
+
+        dists, idxs = tree.query(grid, k=k)
+
+        if k == 1:
+            dists = dists[:, np.newaxis]
+            idxs = idxs[:, np.newaxis]
+
+        warnings.filterwarnings("error")
+
+        for i,(dist, idx) in enumerate(zip(dists, idxs)):
+
+            try:
+                inv_dist = dist**(-0.25)
+                inv_dist = inv_dist/inv_dist.sum()
+            except RuntimeWarning:
+
+                inv_dist = np.zeros(k, dtype=anis.dtype)
+                inv_dist[np.argmin(dist)] = 1 
+
+
+            V[i, :] = (U[idx, :] * inv_dist[:, np.newaxis]).sum(axis=0)
+
+        warnings.resetwarnings()
+
+        V = V.reshape(self._ny, self._nx , 2)[:,:,::-1]
+        H = np.zeros((self._ny,self._nx, 2, 2), dtype=anis.dtype)
+        I = np.eye(2, dtype=anis.dtype)
+
+        for i in range(self._ny):
+            for j in range(self._nx):
+                H[i, j, :, :] = anis.gamma*I +\
+                                anis.beta*(V[i, j][:,np.newaxis] @ \
+                                           V[i, j][np.newaxis,:] )
+
+        anis.H = H
+        anis.V = V
+
+
```

### Comparing `pyspde-0.0.5/src/pyspde/utils.py` & `pyspde-0.0.6/src/pyspde/utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,200 +1,200 @@
-from __future__ import annotations
-import re
-
-import numpy as np
-
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    import xml.etree.ElementTree as Et
-
-__all__ = ['sample_grid']
-
-class imdict(dict):
-    def __hash__(self) -> None:
-        """Return the unique id of the object as its hash value."""
-        return id(self)
-
-    def _immutable(self, *args, **kws) -> None:
-        """Raise TypeError for methods that attempt mutability."""
-        msg = 'Object is immutable'
-        raise TypeError(msg)
-
-    __setitem__ = _immutable
-    __delitem__ = _immutable
-    clear       = _immutable
-    update      = _immutable
-    setdefault  = _immutable
-    pop         = _immutable
-    popitem     = _immutable
-
-
-def map_2d_1d_nx_ny(i: int, j: int, nx: int, ny: int) -> int | None:
-    """Map a 2D index to a 1D index given the dimensions of the 2D array.
-
-    Parameters
-    ----------
-    i : int
-        The row index.
-    j : int
-        The column index.
-    nx : int
-        The total width of the 2D array.
-    ny : int
-        The total height of the 2D array.
-
-    Returns
-    -------
-    int or None
-        The mapped 1D index if the input indices are within bounds, otherwise
-        None.
-
-    """
-    if (i < 0) or (j < 0) or (j >= nx) or (i >= ny):
-        return None
-
-    return int(nx*i + j)
-
-
-def map_1d_2d_nx(idx: int, nx: int) -> tuple[int, int]:
-    """Map a 1D index to a 2D index given the total width of the 2D array.
-
-    Parameters
-    ----------
-    idx : int
-        The 1D index to be mapped.
-    nx : int
-        The total width of the 2D array.
-
-    Returns
-    -------
-    Tuple[int, int]
-        A tuple containing the mapped 2D indices (i, j).
-
-    """
-    j = int(idx % nx)
-    i = int((idx - j) / nx)
-
-    return i, j
-
-
-def get_inkscape_transform(root: Et.Element, xmlns: str,
-                           ) -> tuple[float, float]:
-    """Get the inkscape transform from the root element.
-
-    Parameters
-    ----------
-    root : Et.Element
-        The root element.
-    xmlns : str
-        The namespace string.
-
-    Returns
-    -------
-    Tuple[float, float]
-        A tuple containing the x and y shift values.
-
-    """
-    try:
-        translate = next(root.iter(f'{xmlns}g')).attrib['transform']
-
-        translate = re.search(r'translate\((-?\d+\.\d+),(-?\d+\.\d+)\)',translate)
-        if translate is None:
-            translate = (0, 0)
-        else:
-            shift_x = float(translate.group(1))
-            shift_y = float(translate.group(2))
-
-            translate = (shift_x, shift_y)
-
-    except Exception as e:
-        print('Unknown error while getting inkscape transform: ', e)
-        translate = (0, 0)
-
-    return translate
-
-
-def get_inkscape_namespace(root: Et.Element) -> str:
-    """Extract the XML namespace from the root element tag.
-
-    Parameters
-    ----------
-    root : ElementTree.Element
-        The root element of the XML document.
-
-    Returns
-    -------
-    str
-        The XML namespace extracted from the root element tag. If no namespace 
-        is found, an empty string is returned.
-
-    """
-    xmlns = re.search(r'({.*})',root.tag)
-    xmlns = xmlns.group(1) if xmlns is not None else ''
-
-    return xmlns
-
-
-def sample_grid(Z: np.ndarray, dx: float, dy: float,
-             ) -> np.ndarray:
-    """Regular sampling from a 2D grid.
-
-    Parameters
-    ----------
-    Z : np.ndarray
-        The input array from which to sample points.
-    dx : float
-        The spacing between sample points in the x-direction.
-    dy : float
-        The spacing between sample points in the y-direction.
-
-    Returns
-    -------
-    np.ndarray
-        An array of sample points with shape (n, 3), where n is the number of
-        sample points.
-
-    """
-    ny, nx, * _ = Z.shape
-
-    sx = np.arange(0, nx, dx, dtype=int)
-    sy = np.arange(0, ny, dy, dtype=int)
-
-    xv, yv = np.meshgrid(sx, sy, indexing='xy')
-
-    xv = xv.reshape(-1)
-    yv = yv.reshape(-1)
-    samps = Z[yv, xv]
-
-    X = np.column_stack((xv, yv, samps))
-
-    return X
-
-
-def append_element(vals: list, rows: list, cols: list, val: float, row: int,
-                   col: int) -> None:
-    """Append an element for cosntructiong the sparse matrix.
-
-    Parameters
-    ----------
-    vals : list
-        The list to append the value to.
-    rows : list
-        The list to append the row index to.
-    cols : list
-        The list to append the column index to.
-    val : float
-        The value to append to the `vals` list.
-    row : int
-        The row index to append to the `rows` list.
-    col : int
-        The column index to append to the `cols` list.
-
-    Returns
-    -------
-    None
-
-    """
-    vals.append(val)
-    rows.append(row)
-    cols.append(col)
+from __future__ import annotations
+import re
+
+import numpy as np
+
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    import xml.etree.ElementTree as Et
+
+__all__ = ['sample_grid']
+
+class imdict(dict):
+    def __hash__(self) -> None:
+        """Return the unique id of the object as its hash value."""
+        return id(self)
+
+    def _immutable(self, *args, **kws) -> None:
+        """Raise TypeError for methods that attempt mutability."""
+        msg = 'Object is immutable'
+        raise TypeError(msg)
+
+    __setitem__ = _immutable
+    __delitem__ = _immutable
+    clear       = _immutable
+    update      = _immutable
+    setdefault  = _immutable
+    pop         = _immutable
+    popitem     = _immutable
+
+
+def map_2d_1d_nx_ny(i: int, j: int, nx: int, ny: int) -> int | None:
+    """Map a 2D index to a 1D index given the dimensions of the 2D array.
+
+    Parameters
+    ----------
+    i : int
+        The row index.
+    j : int
+        The column index.
+    nx : int
+        The total width of the 2D array.
+    ny : int
+        The total height of the 2D array.
+
+    Returns
+    -------
+    int or None
+        The mapped 1D index if the input indices are within bounds, otherwise
+        None.
+
+    """
+    if (i < 0) or (j < 0) or (j >= nx) or (i >= ny):
+        return None
+
+    return int(nx*i + j)
+
+
+def map_1d_2d_nx(idx: int, nx: int) -> tuple[int, int]:
+    """Map a 1D index to a 2D index given the total width of the 2D array.
+
+    Parameters
+    ----------
+    idx : int
+        The 1D index to be mapped.
+    nx : int
+        The total width of the 2D array.
+
+    Returns
+    -------
+    Tuple[int, int]
+        A tuple containing the mapped 2D indices (i, j).
+
+    """
+    j = int(idx % nx)
+    i = int((idx - j) / nx)
+
+    return i, j
+
+
+def get_inkscape_transform(root: Et.Element, xmlns: str,
+                           ) -> tuple[float, float]:
+    """Get the inkscape transform from the root element.
+
+    Parameters
+    ----------
+    root : Et.Element
+        The root element.
+    xmlns : str
+        The namespace string.
+
+    Returns
+    -------
+    Tuple[float, float]
+        A tuple containing the x and y shift values.
+
+    """
+    try:
+        translate = next(root.iter(f'{xmlns}g')).attrib['transform']
+
+        translate = re.search(r'translate\((-?\d+\.\d+),(-?\d+\.\d+)\)',translate)
+        if translate is None:
+            translate = (0, 0)
+        else:
+            shift_x = float(translate.group(1))
+            shift_y = float(translate.group(2))
+
+            translate = (shift_x, shift_y)
+
+    except Exception as e:
+        print('Unknown error while getting inkscape transform: ', e)
+        translate = (0, 0)
+
+    return translate
+
+
+def get_inkscape_namespace(root: Et.Element) -> str:
+    """Extract the XML namespace from the root element tag.
+
+    Parameters
+    ----------
+    root : ElementTree.Element
+        The root element of the XML document.
+
+    Returns
+    -------
+    str
+        The XML namespace extracted from the root element tag. If no namespace 
+        is found, an empty string is returned.
+
+    """
+    xmlns = re.search(r'({.*})',root.tag)
+    xmlns = xmlns.group(1) if xmlns is not None else ''
+
+    return xmlns
+
+
+def sample_grid(Z: np.ndarray, dx: float, dy: float,
+             ) -> np.ndarray:
+    """Regular sampling from a 2D grid.
+
+    Parameters
+    ----------
+    Z : np.ndarray
+        The input array from which to sample points.
+    dx : float
+        The spacing between sample points in the x-direction.
+    dy : float
+        The spacing between sample points in the y-direction.
+
+    Returns
+    -------
+    np.ndarray
+        An array of sample points with shape (n, 3), where n is the number of
+        sample points.
+
+    """
+    ny, nx, * _ = Z.shape
+
+    sx = np.arange(0, nx, dx, dtype=int)
+    sy = np.arange(0, ny, dy, dtype=int)
+
+    xv, yv = np.meshgrid(sx, sy, indexing='xy')
+
+    xv = xv.reshape(-1)
+    yv = yv.reshape(-1)
+    samps = Z[yv, xv]
+
+    X = np.column_stack((xv, yv, samps))
+
+    return X
+
+
+def append_element(vals: list, rows: list, cols: list, val: float, row: int,
+                   col: int) -> None:
+    """Append an element for cosntructiong the sparse matrix.
+
+    Parameters
+    ----------
+    vals : list
+        The list to append the value to.
+    rows : list
+        The list to append the row index to.
+    cols : list
+        The list to append the column index to.
+    val : float
+        The value to append to the `vals` list.
+    row : int
+        The row index to append to the `rows` list.
+    col : int
+        The column index to append to the `cols` list.
+
+    Returns
+    -------
+    None
+
+    """
+    vals.append(val)
+    rows.append(row)
+    cols.append(col)
```

### Comparing `pyspde-0.0.5/src/pyspde.egg-info/PKG-INFO` & `pyspde-0.0.6/src/pyspde.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-Metadata-Version: 2.1
-Name: pyspde
-Version: 0.0.5
-Summary: PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs)
-Author-email: Esteban Jimenez <ejimenez@minerai.com.au>
-Project-URL: Homepage, https://github.com/M1nerAI/pyspde
-Project-URL: Issues, https://github.com/M1nerAI/pyspde/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: scipy
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: scikit-sparse==0.4.12
-
-# PySPDE
-
-PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs):
-
-$$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}W(x) \quad x \in \mathbb{R}^2
-$$
-
-The theory is proposed in Fuglstad (2014).
-
-## Instalation
-
-On Debian/Ubuntu systems:
-```
-sudo apt-get install libsuitesparse-dev
-pip install pyspde
-```
-
-On Windows systems:
-```
-conda install -c conda-forge suitesparse
-pip install pyspde
-```
-
-## Basic Usage
-
-Imports:
-```
-from pyspde import anisotropy, Grid, Spde
-```
-
-Define the anisotropy and the grid:
-```
-atpy = anisotropy_from_svg(r'assets/anicline.svg', beta=10, gamma=0.1)
-grid = Grid(nx=200, ny=100, anisotropy=atpy)
-```
-
-Define SPDE and Simulate:
-```
-sp = Spde(grid, sigma=1, a=25)
-Z = sp.simulate()
-```
+Metadata-Version: 2.1
+Name: pyspde
+Version: 0.0.6
+Summary: PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs)
+Author-email: Esteban Jimenez <ejimenez@minerai.com.au>
+Project-URL: Homepage, https://github.com/M1nerAI/pyspde
+Project-URL: Issues, https://github.com/M1nerAI/pyspde/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: scipy
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: scikit-sparse==0.4.12
+
+# PySPDE
+
+PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs):
+
+$$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}(x)W(x) \quad x \in \mathbb{R}^2
+$$
+
+The theory is proposed in Fuglstad (2014).
+
+## Instalation
+
+On Debian/Ubuntu systems:
+```
+sudo apt-get install libsuitesparse-dev
+pip install pyspde
+```
+
+On Windows systems:
+```
+conda install -c conda-forge suitesparse
+pip install pyspde
+```
+
+## Basic Usage
+
+Imports:
+```
+from pyspde import anisotropy, Grid, Spde, anisotropy_from_svg
+```
+
+Define the anisotropy and the grid:
+```
+atpy = anisotropy_from_svg(r'assets/anticline.svg', beta=50, gamma=0.5)
+grid = Grid(nx=400, ny=200, anisotropy=atpy)
+```
+
+Define SPDE and Simulate:
+```
+sp = Spde(grid, sigma=1, a=50)
+Z = sp.simulate(seed=0)
+```
+
+![alt text](https://onedrive.live.com/embed?resid=a94fce3415a299a1%2117697&authkey=%21AMG50D19mGNfdyY&width=660)
```

