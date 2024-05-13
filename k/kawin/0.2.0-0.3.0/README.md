# Comparing `tmp/kawin-0.2.0.tar.gz` & `tmp/kawin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kawin-0.2.0.tar", last modified: Fri May 12 03:08:57 2023, max compression
+gzip compressed data, was "kawin-0.3.0.tar", last modified: Mon May 13 22:47:31 2024, max compression
```

## Comparing `kawin-0.2.0.tar` & `kawin-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 03:08:57.980107 kawin-0.2.0/
--rw-rw-rw-   0        0        0     1251 2022-08-31 21:05:28.000000 kawin-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       52 2022-08-31 21:05:28.000000 kawin-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1325 2023-05-12 03:08:57.979106 kawin-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      501 2022-08-31 21:05:28.000000 kawin-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 03:08:57.937760 kawin-0.2.0/kawin/
--rw-rw-rw-   0        0        0    35058 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/Diffusion.py
--rw-rw-rw-   0        0        0     4924 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/EffectiveDiffusion.py
--rw-rw-rw-   0        0        0    35769 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/ElasticFactors.py
--rw-rw-rw-   0        0        0     7543 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/FreeEnergyHessian.py
--rw-rw-rw-   0        0        0     6858 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/GrainBoundaries.py
--rw-rw-rw-   0        0        0    75858 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/KWNBase.py
--rw-rw-rw-   0        0        0    52739 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/KWNEuler.py
--rw-rw-rw-   0        0        0    37701 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/LebedevNodes.py
--rw-rw-rw-   0        0        0     2644 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/LocalEquilibrium.py
--rw-rw-rw-   0        0        0    17421 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/Mobility.py
--rw-rw-rw-   0        0        0    25704 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/PopulationBalance.py
--rw-rw-rw-   0        0        0    13586 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/ShapeFactors.py
--rw-rw-rw-   0        0        0    39544 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/Strength.py
--rw-rw-rw-   0        0        0    67348 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/Surrogate.py
--rw-rw-rw-   0        0        0    78335 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/Thermodynamics.py
--rw-rw-rw-   0        0        0        0 2023-05-05 03:15:13.000000 kawin-0.2.0/kawin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 03:08:57.978107 kawin-0.2.0/kawin/tests/
--rw-rw-rw-   0        0        0    71718 2022-11-02 19:07:56.000000 kawin-0.2.0/kawin/tests/datasets.py
--rw-rw-rw-   0        0        0     4217 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/tests/test_PBM.py
--rw-rw-rw-   0        0        0     9266 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/tests/test_diffusion.py
--rw-rw-rw-   0        0        0     7503 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/tests/test_extraFactors.py
--rw-rw-rw-   0        0        0     8101 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/tests/test_strength.py
--rw-rw-rw-   0        0        0    11110 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/tests/test_surrogate.py
--rw-rw-rw-   0        0        0    14488 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/tests/test_thermodynamics.py
-drwxrwxrwx   0        0        0        0 2023-05-12 03:08:57.967637 kawin-0.2.0/kawin.egg-info/
--rw-rw-rw-   0        0        0     1325 2023-05-12 03:08:57.000000 kawin-0.2.0/kawin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2023-05-12 03:08:57.000000 kawin-0.2.0/kawin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 03:08:57.000000 kawin-0.2.0/kawin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-12 03:08:57.000000 kawin-0.2.0/kawin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-12 03:08:57.000000 kawin-0.2.0/kawin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2022-08-31 21:05:28.000000 kawin-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 03:08:57.980107 kawin-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1602 2022-11-02 19:07:56.000000 kawin-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:47:31.632185 kawin-0.3.0/
+-rw-rw-rw-   0        0        0     1251 2023-10-04 19:40:10.000000 kawin-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       52 2023-10-04 19:40:10.000000 kawin-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1600 2024-05-13 22:47:31.630185 kawin-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2024-05-13 18:14:04.000000 kawin-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 22:47:31.492960 kawin-0.3.0/kawin/
+-rw-rw-rw-   0        0        0    18212 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/GenericModel.py
+-rw-rw-rw-   0        0        0        0 2023-10-04 19:40:10.000000 kawin-0.3.0/kawin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:47:31.513010 kawin-0.3.0/kawin/diffusion/
+-rw-rw-rw-   0        0        0    18962 2024-05-13 17:45:57.000000 kawin-0.3.0/kawin/diffusion/Diffusion.py
+-rw-rw-rw-   0        0        0    14074 2024-05-13 17:45:57.000000 kawin-0.3.0/kawin/diffusion/Homogenization.py
+-rw-rw-rw-   0        0        0     5147 2024-05-13 17:45:57.000000 kawin-0.3.0/kawin/diffusion/Plot.py
+-rw-rw-rw-   0        0        0     3635 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/diffusion/SinglePhase.py
+-rw-rw-rw-   0        0        0       90 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/diffusion/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:47:31.533257 kawin-0.3.0/kawin/precipitation/
+-rw-rw-rw-   0        0        0    52409 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/KWNBase.py
+-rw-rw-rw-   0        0        0    39836 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/KWNEuler.py
+-rw-rw-rw-   0        0        0    21071 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/Plot.py
+-rw-rw-rw-   0        0        0    39831 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/PopulationBalance.py
+-rw-rw-rw-   0        0        0     4763 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/StoppingConditions.py
+-rw-rw-rw-   0        0        0     4093 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/TimeTemperaturePrecipitation.py
+-rw-rw-rw-   0        0        0      306 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:47:31.543427 kawin-0.3.0/kawin/precipitation/coupling/
+-rw-rw-rw-   0        0        0    13394 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/coupling/GrainGrowth.py
+-rw-rw-rw-   0        0        0    42976 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/coupling/Strength.py
+-rw-rw-rw-   0        0        0       78 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/coupling/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:47:31.561666 kawin-0.3.0/kawin/precipitation/non_ideal/
+-rw-rw-rw-   0        0        0     4924 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/non_ideal/EffectiveDiffusion.py
+-rw-rw-rw-   0        0        0    38378 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/non_ideal/ElasticFactors.py
+-rw-rw-rw-   0        0        0     6858 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/non_ideal/GrainBoundaries.py
+-rw-rw-rw-   0        0        0    37701 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/non_ideal/LebedevNodes.py
+-rw-rw-rw-   0        0        0    14077 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/non_ideal/ShapeFactors.py
+-rw-rw-rw-   0        0        0        0 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/precipitation/non_ideal/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:47:31.561666 kawin-0.3.0/kawin/solver/
+-rw-rw-rw-   0        0        0     2047 2024-04-04 00:09:00.000000 kawin-0.3.0/kawin/solver/Iterators.py
+-rw-rw-rw-   0        0        0     7766 2024-04-03 22:57:35.000000 kawin-0.3.0/kawin/solver/Solver.py
+-rw-rw-rw-   0        0        0       40 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/solver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:47:31.598918 kawin-0.3.0/kawin/tests/
+-rw-rw-rw-   0        0        0        0 2024-01-24 21:11:17.000000 kawin-0.3.0/kawin/tests/__init__.py
+-rw-rw-rw-   0        0        0    98150 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/tests/datasets.py
+-rw-rw-rw-   0        0        0     3492 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/tests/test_PBM.py
+-rw-rw-rw-   0        0        0    13576 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/tests/test_diffusion.py
+-rw-rw-rw-   0        0        0    10567 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/tests/test_extraFactors.py
+-rw-rw-rw-   0        0        0     4525 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/tests/test_plotting.py
+-rw-rw-rw-   0        0        0     7814 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/tests/test_precipitation.py
+-rw-rw-rw-   0        0        0     4573 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/tests/test_solver.py
+-rw-rw-rw-   0        0        0     8115 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/tests/test_strength.py
+-rw-rw-rw-   0        0        0    11074 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/tests/test_surrogate.py
+-rw-rw-rw-   0        0        0    15300 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/tests/test_thermodynamics.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:47:31.623920 kawin-0.3.0/kawin/thermo/
+-rw-rw-rw-   0        0        0    15438 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/thermo/BinTherm.py
+-rw-rw-rw-   0        0        0     8979 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/thermo/FreeEnergyHessian.py
+-rw-rw-rw-   0        0        0     2793 2024-05-13 17:45:57.000000 kawin-0.3.0/kawin/thermo/LocalEquilibrium.py
+-rw-rw-rw-   0        0        0    30492 2024-05-13 17:45:57.000000 kawin-0.3.0/kawin/thermo/Mobility.py
+-rw-rw-rw-   0        0        0    24264 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/thermo/MultiTherm.py
+-rw-rw-rw-   0        0        0    67756 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/thermo/Surrogate.py
+-rw-rw-rw-   0        0        0    60293 2024-05-13 17:45:57.000000 kawin-0.3.0/kawin/thermo/Thermodynamics.py
+-rw-rw-rw-   0        0        0      236 2024-01-24 20:28:13.000000 kawin-0.3.0/kawin/thermo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:47:31.627919 kawin-0.3.0/kawin.egg-info/
+-rw-rw-rw-   0        0        0     1600 2024-05-13 22:47:31.000000 kawin-0.3.0/kawin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1673 2024-05-13 22:47:31.000000 kawin-0.3.0/kawin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 22:47:31.000000 kawin-0.3.0/kawin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-13 22:47:31.000000 kawin-0.3.0/kawin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 22:47:31.000000 kawin-0.3.0/kawin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      590 2024-01-24 21:05:12.000000 kawin-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 22:47:31.632185 kawin-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1741 2024-05-13 18:13:40.000000 kawin-0.3.0/setup.py
```

### Comparing `kawin-0.2.0/LICENSE.txt` & `kawin-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kawin-0.2.0/PKG-INFO` & `kawin-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kawin
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tool for simulating precipitation using the KWN model coupled with Calphad.
 Home-page: https://kawin.org/
 Author: Nicholas Ury
 Author-email: nury12n@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -14,19 +14,28 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: matplotlib>=3.3
+Requires-Dist: numpy>=1.13
+Requires-Dist: pycalphad>=0.10.1
+Requires-Dist: scipy
+Requires-Dist: setuptools_scm[toml]>=6.0
 
 # kawin
 
 Python implementation of the Kampmann-Wagner Numerical (KWN) model to predict precipitate nucleation and growth behavior. This package couples with pycalphad to perform thermodynamic and kinetic calculations.
 
+Notes
+-----
+There are some API changes between kawin 0.3.0 and 0.2.0. Please see the examples for more details.
+
 Installation
 ------------
 `pip install kawin`
 
 Examples
 --------
 Examples on Jupyter notebooks can be found on [NBViewer](https://nbviewer.org/github/materialsgenomefoundation/kawin/tree/main/examples/).
```

### Comparing `kawin-0.2.0/kawin/Diffusion.py` & `kawin-0.3.0/kawin/precipitation/non_ideal/ElasticFactors.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,971 +1,1023 @@
 import numpy as np
+import itertools
 import matplotlib.pyplot as plt
-from kawin.Mobility import mobility_from_composition_set
-import time
-import csv
+from kawin.precipitation.non_ideal.LebedevNodes import loadPoints
 import copy
-from itertools import zip_longest
 
-class DiffusionModel:
-    #Boundary conditions
-    FLUX = 0
-    COMPOSITION = 1
-
-    def __init__(self, zlim, N, elements = ['A', 'B'], phases = ['alpha']):
-        '''
-        Class for defining a 1-dimensional mesh
+class StrainEnergy:
+    '''
+    Defines class for calculating strain energy of a precipitate
+
+    Ellipsoidal precipitates will use the Eshelby's tensor
+    Spherical and Cuboidal precipitates will use the Khachaturyan's approximation
+    '''
+
+    SPHERE = 0
+    ELLIPSE = 1
+    CUBE = 2
+    CONSTANT = 3
+
+    def __init__(self):
+        self.c = None
+        self._c4 = np.zeros((3,3,3,3))
+        self.cPrec = None
+        self._c4Prec = np.zeros((3,3,3,3))
+        self.eigstrain = np.zeros((3,3))
+        self.appstress = np.zeros((3,3))
+        self.appstrain = np.zeros((3,3))
+        self.rotation = None
+        self.rotationPrec = None
+
+        self.lebedevIntegration('high')
+
+        self._strainEnergyGeneric = self._strainEnergyConstant
+        self.type = self.CONSTANT
+        self.r = np.zeros(3)
+        self.oldr = np.zeros(3)
+        self._prevEnergy = 0
+
+        self._gElasticConstant = 0
+
+        #Cached values for calculating equilibrium aspect ratio
+        self.ifmethod = 1
+        self._aspectRatios = None
+        self._normEnergies = None
+        self._cachedRange = 5
+        self._cachedIntervals = 100
+
+        self._ohm_inverse = self._ohm_quickInverse
+
+    def setOhmInverseFunction(self, method = 'quick'):
+        '''
+        Sets method to invert the ohm term in calculating eshelby's tensor
 
         Parameters
         ----------
-        zlim : tuple
-            Z-bounds of mesh (lower, upper)
-        N : int
-            Number of nodes
-        elements : list of str
-            Elements in system (first element will be assumed as the reference element)
-        phases : list of str
-            Number of phases in the system
+        method : str
+            'numpy' - uses np.linalg.inv, which can be slower for batch, but runs through
+                        multiple checks for whether values are real/complex or if inverse exists
+            'quick' - quick inverse using Cramer's rule assuming that values are real and inverse exists - recommended method
         '''
-        if isinstance(phases, str):
-            phases = [phases]
-        self.zlim, self.N = zlim, N
-        self.allElements, self.elements = elements, elements[1:]
-        self.phases = phases
-        self.therm = None
-
-        self.z = np.linspace(zlim[0], zlim[1], N)
-        self.dz = self.z[1] - self.z[0]
-
-        self.reset()
-
-        self.LBC, self.RBC = self.FLUX*np.ones(len(self.elements)), self.FLUX*np.ones(len(self.elements))
-        self.LBCvalue, self.RBCvalue = np.zeros(len(self.elements)), np.zeros(len(self.elements))
-
-        self.cache = True
-        self.setHashSensitivity(4)
-        self.minComposition = 1e-8
-
-        self.maxCompositionChange = 0.002
+        if method == 'numpy':
+            self._ohm_inverse = self._ohm_npinv
+        else:
+            self._ohm_inverse = self._ohm_quickInverse
 
-    def reset(self):
+    def setAspectRatioResolution(self, resolution = 0.01, cachedRange = 5):
         '''
-        Resets model
+        Sets resolution to which equilibrium aspect ratios are calculated
 
-        This involves clearing any caches in the Thermodynamics object and this model
-        as well as resetting the composition and phase profiles
-        '''
-        if self.therm is not None:
-            self.therm.clearCache()
-        
-        self.x = np.zeros((len(self.elements), self.N))
-        self.p = np.ones((1,self.N)) if len(self.phases) == 1 else np.zeros((len(self.phases), self.N))
-        self.hashTable = {}
-        self.isSetup = False
+        Equilibrium aspect ratios are found by calculated strain energy for a range of aspect ratios
+        and finding the aspect ratio giving the minimum energy (strain + interfacial energy)
 
-    def setThermodynamics(self, thermodynamics):
-        '''
-        Defines thermodynamics object for the diffusion model
+        If aspect ratio does not vary much in a given system, then the default parameters may lead to poor
+        prediction of the aspect ratios
 
         Parameters
         ----------
-        thermodynamics : Thermodynamics object
-            Requires the elements in the Thermodynamics and DiffusionModel objects to have the same order
+        resolution : float (optional)
+            Minimum distance between aspect ratios when calculating cache (default at 0.01)
+        cachedRange : float (optional)
+            Range of aspect ratio to calculate strain energy when updated cache (default at 5)
         '''
-        self.therm = thermodynamics
+        self._cachedRange = cachedRange
+        self._cachedIntervals = int(1 / resolution)
 
-    def setTemperature(self, T):
+    def setInterfacialEnergyMethod(self, method):
         '''
-        Sets iso-thermal temperature
+        Sets method for calculating interfacial energy as a function of aspect ratio
 
         Parameters
         ----------
-        T : float
-            Temperature in Kelvin
+        method : str
+            'eqradius' - interfacial energy is determined using the equivalent spherical radius
+            'thermo' - interfacial energy is determined using dG/dSA (default)
         '''
-        self.T = T
+        if method == 'eqradius':
+            self.ifmethod = 0
+        else:
+            self.ifmethod = 1
 
-    def save(self, filename, compressed = False, toCSV = False):
+    def setSpherical(self):
         '''
-        Saves mesh, composition and phases
-
-        Parameters
-        ----------
-        filename : str
-            File to save to
-        compressed : bool
-            Whether to compress data if saving to numpy binary format (toCSV = False)
-        toCSV : bool
-            Whether to output data to a .CSV file format
+        Assumes spherical geometry for strain energy calculation
+        Uses Khachaturyan's approximation
         '''
-        if toCSV:
-            headers = ['Distance(m)']
-            arrays = [self.z]
-            for i in range(len(self.allElements)):
-                headers.append('x(' + self.allElements[i] + ')')
-                if i == 0:
-                    arrays.append(1 - np.sum(self.x, axis=0))
-                else:
-                    arrays.append(self.x[i-1,:])
-            for i in range(len(self.phases)):
-                headers.append('f(' + self.phases[i] + ')')
-                arrays.append(self.p[i,:])
-            rows = zip_longest(*arrays, fillvalue='')
-            if '.csv' not in filename.lower():
-                filename = filename + '.csv'
-            with open(filename, 'w', newline='') as f:
-                csv.writer(f).writerow(headers)
-                csv.writer(f).writerows(rows)
-        else:
-            variables = ['zlim', 'N', 'allElements', 'phases', 'z', 'x', 'p']
-            vDict = {v: getattr(self, v) for v in variables}
-            if compressed:
-                np.savez_compressed(filename, **vDict, allow_pickle=True)
-            else:
-                np.savez(filename, **vDict, allow_pickle=True)
-
-    def load(filename):
+        self._strainEnergyGeneric = self._strainEnergySphere
+        self.type = self.SPHERE
+    
+    def setCuboidal(self):
         '''
-        Loads a previously saved model
-
-        filename : str
-            File name to load model from, must include file extension
+        Assumes cuboidal geometry for strain energy calculation
+        Uses Khachaturyan's approximation
         '''
-        if '.np' in filename.lower():
-            data = np.load(filename, allow_pickle=True)
-            model = DiffusionModel(data['zlim'], data['N'], data['allElements'], data['phases'])
-            model.z = data['z']
-            model.x = data['x']
-            model.p = data['p']
-        else:
-            with open(filename, 'r') as csvFile:
-                data = csv.reader(csvFile, delimiter=',')
-                i = 0
-                headers = []
-                columns = {}
-                for row in data:
-                    if i == 0:
-                        headers = row
-                        columns = {h: [] for h in headers}
-                    else:
-                        for j in range(len(row)):
-                            if row[j] != '':
-                                columns[headers[j]].append(float(row[j]))
-                    i += 1
-            
-            elements, phases = [], []
-            x, p = [], []
-            for h in headers:
-                if 'Distance' in h:
-                    z = columns[h]
-                elif 'x' in h:
-                    elements.append(h[2:-1])
-                    x.append(columns[h])
-                elif 'f' in h:
-                    phases.append(h[2:-1])
-                    p.append(columns[h])
-            model = DiffusionModel([z[0], z[-1]], len(z), elements, phases)
-            model.z = np.array(z)
-            model.x = np.array(x)[1:,:]
-            model.p = np.array(p)
-        return model   
+        self._strainEnergyGeneric = self._strainEnergyCube
+        self.type = self.CUBE
 
-    def setHashSensitivity(self, s):
+    def setEllipsoidal(self):
         '''
-        Sets sensitivity of the hash table by significant digits
-
-        For example, if a composition set is (0.5693, 0.2937) and s = 3, then
-        the hash will be stored as (0.569, 0.294)
+        Assumes ellipsoidal geometry for strain energy calculation
+        Uses Eshelby's tensor
+        '''
+        self._strainEnergyGeneric = self._strainEnergyEllipsoid
+        self._strainEnergyGeneric = self._strainEnergyBohm
+        self.type = self.ELLIPSE
 
-        Lower s values will give faster simulation times at the expense of accuracy
+    def setConstantElasticEnergy(self, energy):
+        '''
+        If elastic strain energy is known to be a constant, this can be use to greatly
+        simplify calculations
 
         Parameters
         ----------
-        s : int
-            Number of significant digits to keep for the hash table
+        energy - strain energy in J/m3
         '''
-        self.hashSensitivity = np.power(10, int(s))
+        self._gElasticConstant = energy
+        self._strainEnergyGeneric = self._strainEnergyConstant
+        self.type = self.CONSTANT
 
-    def _getHash(self, x):
+    def setElasticTensor(self, tensor):
         '''
-        Gets hash value for a composition set
+        Sets elastic tensor of matrix using 2nd rank tensor
 
         Parameters
         ----------
-        x : list of floats
-            Composition set to create hash
+        tensor : 6x6 array
+            2nd rank elastic tensor
         '''
-        return hash(tuple((x*self.hashSensitivity).astype(np.int32)))
-        #return int(np.sum(np.power(self.hashSensitivity, 1+np.arange(len(x))) * x))
+        self.c = self._setElasticTensor(tensor)
+        self._c4 = self._convert2To4rankTensor(self.c)
 
-    def useCache(self, use):
+    def setElasticConstants(self, c11, c12, c44):
         '''
-        Whether to use the hash table
+        Sets elastic tensor of matrix by elastic constants, assuming cubic symmetry
 
         Parameters
         ----------
-        use : bool
-            If True, then the hash table will be used
-        '''
-        self.cache = use
-
-    def clearCache(self):
-        '''
-        Clears hash table
+        c11 : float
+            Modulus for compression
+            c11 = E(1-nu) / (1+nu)(1-2nu)
+        c12 : float
+            Modulus for dilation (accounts for compression and Poisson's ratio)
+            c12 = E nu / (1+nu)(1-2nu)
+        c44 : float
+            Modulus for shear
+            c44 = (c11-c12)/2
         '''
-        self.hashTable = {}
+        self.c = self._setElasticConstants(c11, c12, c44)
+        self._c4 = self._convert2To4rankTensor(self.c)
 
-    def _getElementIndex(self, element = None):
+    def setModuli(self, E = None, nu = None, G = None, lam = None, K = None, M = None):
         '''
-        Gets index of element in self.elements
+        Sets elastic tensor of matrix by 2 moduli
 
-        Parameters
+        Parameters (only 2 has to be defined)
         ----------
-        element : str
-            Specified element, will return first element if None
+        E : float
+            Elastic modulus
+        nu : float
+            Poisson's ratio
+        G : float
+            Shear modulus
+        lam : float
+            Lame's first parameter
+        K : float
+            Bulk modulus
+        M : float
+            P-wave modulus
         '''
-        if element is None:
-            return 0
-        else:
-            return self.elements.index(element)
+        self.c = self._setModuli(E, nu, G, lam, K, M)
+        self._c4 = self._convert2To4rankTensor(self.c)
 
-    def _getPhaseIndex(self, phase = None):
+    def setElasticTensorPrecipitate(self, tensor):
         '''
-        Gets index of phase in self.phases
+        Sets elastic tensor of precipitate using 2nd rank tensor
 
         Parameters
         ----------
-        phase : str
-            Specified phase, will return first phase if None
+        tensor : 6x6 array
+            2nd rank elastic tensor
         '''
-        if phase is None:
-            return 0
-        else:
-            return self.phases.index(phase)
+        self.cPrec = self._setElasticTensor(tensor)
+        self._c4Prec = self._convert2To4rankTensor(self.cPrec)
 
-    def setBC(self, LBCtype = 0, LBCvalue = 0, RBCtype = 0, RBCvalue = 0, element = None):
+    def setElasticConsantsPrecipitate(self, c11, c12, c44):
         '''
-        Set boundary conditions
+        Sets elastic tensor of precipitate by elastic constants, assuming cubic symmetry
 
         Parameters
         ----------
-        LBCtype : int
-            Left boundary condition type
-                Mesh1D.FLUX - constant flux
-                Mesh1D.COMPOSITION - constant composition
-        LBCvalue : float
-            Value of left boundary condition
-        RBCtype : int
-            Right boundary condition type
-                Mesh1D.FLUX - constant flux
-                Mesh1D.COMPOSITION - constant composition
-        RBCvalue : float
-            Value of right boundary condition
-        element : str
-            Specified element to apply boundary conditions on
+        c11 : float
+            Modulus for compression
+            c11 = E(1-nu) / (1+nu)(1-2nu)
+        c12 : float
+            Modulus for dilation (accounts for compression and Poisson's ratio)
+            c12 = E nu / (1+nu)(1-2nu)
+        c44 : float
+            Modulus for shear
+            c44 = (c11-c12)/2
         '''
-        eIndex = self._getElementIndex(element)
-        self.LBC[eIndex] = LBCtype
-        self.LBCvalue[eIndex] = LBCvalue
-        if LBCtype == self.COMPOSITION:
-            self.x[eIndex,0] = LBCvalue
-
-        self.RBC[eIndex] = RBCtype
-        self.RBCvalue[eIndex] = RBCvalue
-        if RBCtype == self.COMPOSITION:
-            self.x[eIndex,-1] = RBCvalue
-
-    def setCompositionLinear(self, Lvalue, Rvalue, element = None):
+        self.cPrec = self._setElasticConstants(c11, c12, c44)
+        self._c4Prec = self._convert2To4rankTensor(self.cPrec)
+    
+    def setModuliPrecipitate(self, E = None, nu = None, G = None, lam = None, K = None, M = None):
         '''
-        Sets composition as a linear function between ends of the mesh
+        Sets elastic tensor of precipitate by 2 moduli
 
-        Parameters
+        Parameters (only 2 has to be defined)
         ----------
-        Lvalue : float
-            Value at left boundary
-        Rvalue : float
-            Value at right boundary
-        element : str
-            Element to apply composition profile to
+        E : float
+            Elastic modulus
+        nu : float
+            Poisson's ratio
+        G : float
+            Shear modulus
+        lam : float
+            Lame's first parameter
+        K : float
+            Bulk modulus
+        M : float
+            P-wave modulus
         '''
-        eIndex = self._getElementIndex(element)
-        self.x[eIndex] = np.linspace(Lvalue, Rvalue, self.N)
+        self.cPrec = self._setModuli(E, nu, G, lam, K, M)
+        self._c4Prec = self._convert2To4rankTensor(self.cPrec)
 
-    def setCompositionStep(self, Lvalue, Rvalue, z, element = None):
+    def _setElasticTensor(self, tensor):
         '''
-        Sets composition as a step-wise function
+        Inputs 6x6 elastic matrix
 
         Parameters
         ----------
-        Lvalue : float
-            Value on left side of mesh
-        Rvalue : float
-            Value on right side of mesh
-        z : float
-            Position on mesh where composition switches from Lvalue to Rvalue
-        element : str
-            Element to apply composition profile to
+        tensor : matrix of floats
+            Must be 6x6
         '''
-        eIndex = self._getElementIndex(element)
-        Lindices = self.z <= z
-        self.x[eIndex,Lindices] = Lvalue
-        self.x[eIndex,~Lindices] = Rvalue
+        return np.array(tensor)
 
-    def setCompositionSingle(self, value, z, element = None):
+    def _setElasticConstants(self, c11, c12, c44):
         '''
-        Sets single node to specified composition
+        Creates elastic tensor from c11, c12 and c44 constants assuming isotropic system
 
         Parameters
         ----------
-        value : float
-            Composition
-        z : float
-            Position to set value to (will use closest node to z)
-        element : str
-            Element to apply composition profile to
+        c11 : float
+        c12 : float
+        c44 : float
         '''
-        eIndex = self._getElementIndex(element)
-        zIndex = np.argmin(np.abs(self.z-z))
-        self.x[eIndex,zIndex] = value
+        c = np.zeros((6, 6))
+        c[0,0], c[1,1], c[2,2] = c11, c11, c11
+        c[0,1], c[0,2], c[1,0], c[1,2], c[2,0], c[2,1] = c12, c12, c12, c12, c12, c12
+        c[3,3], c[4,4], c[5,5] = c44, c44, c44
+        return c
 
-    def setCompositionInBounds(self, value, Lbound, Rbound, element = None):
+    def _setModuli(self, E = None, nu = None, G = None, lam = None, K = None, M = None):
         '''
-        Sets single node to specified composition
+        Set elastic tensor by defining at least two of the moduli
+        Everything will be converted to E, nu and G
+        If more than two parameters are defined, then the following priority will be used:
+        E - Youngs modulus
+        nu - Poisson's ratio
+        G - shear modulus
+        lam - Lame's first parameter
+        K - bulk modulus
+        M - P-wave modulus
 
-        Parameters
-        ----------
-        value : float
-            Composition
-        Lbound : float
-            Position of left bound
-        Rbound : float
-            Position of right bound
-        element : str
-            Element to apply composition profile to
+        NOTE: There's gotta be a better way to implement the conversions
         '''
-        eIndex = self._getElementIndex(element)
-        indices = (self.z >= Lbound) & (self.z <= Rbound)
-        self.x[eIndex,indices] = value
+        if E:
+            if nu:
+                G = E / (2 * (1 + nu))
+            elif G:
+                nu = E / (2 * G) - 1
+            elif lam:
+                R = np.sqrt(E**2 + 9*lam**2 + 2*E*lam)
+                nu = 2*lam / (E + lam + R)
+                G = (E - 3*lam + R) / 4
+            elif K:
+                nu = (3*K - E) / (6*K)
+                G = 3*K*E / (9*K - E)
+            elif M:
+                S = np.sqrt(E**2 + 9*M**2 - 10*E*M)
+                nu = (E - M + S) / (4*M)
+                G = (3*M + E - S) / 8
+        elif nu:
+            if G:
+                E = 2*G*(1 + nu)
+            elif lam:
+                E = lam * (1 + nu) * (1 - 2*nu) / nu
+                G = lam * (1 - 2*nu) / (2*nu)
+            elif K:
+                E = 3*K*(1 - 2*nu)
+                G = 3*K*(1 - 2*nu) / (2*(1 + nu))
+            elif M:
+                E = M * (1 + nu) * (1 - 2*nu) / (1 - nu)
+                G = M * (1 - 2*nu) / (2 * (1 - nu))
+        elif G:
+            if lam:
+                E = G * (3*lam + 2*G) / (lam + G)
+                nu = lam / (2*(lam + G))
+            elif K:
+                E = 9*K*G / (3*K + G)
+                nu = (3*K - 2*G) / (2*(3*K + G))
+            elif M:
+                E = G * (3*M - 4*G) / (M - G)
+                nu = (M - 2*G) / (2*M - 2*G)
+        elif lam:
+            if K:
+                E = 9*K*(K - lam) / (3*K - lam)
+                G = 3*(K - lam) / 2
+                nu = lam / (3*K - lam)
+            elif M:
+                E = (M - lam) * (M + 2*lam) / (M + lam)
+                G = (M - lam) / 2
+                nu = lam / (M + lam)
+        elif K:
+            if M:
+                E = 9*K*(M - K) / (3*K + M)
+                G = 3*(M - K) / 4
+                nu = (3*K - M) / (3*K + M)
 
-    def setCompositionFunction(self, func, element = None):
+        s = np.zeros((6,6))
+        s[0,0], s[1,1], s[2,2] = 1/E, 1/E, 1/E
+        s[3,3], s[4,4], s[5,5] = 1/G, 1/G, 1/G
+        s[0,1], s[0,2], s[1,0], s[1,2], s[2,0], s[2,1] = -nu/E, -nu/E, -nu/E, -nu/E, -nu/E, -nu/E
+        return np.linalg.inv(s)
+
+    def setRotationMatrix(self, rot):
         '''
-        Sets composition as a function of z
+        Sets rotation matrix to be applied to the matrix
+
+        This is for cases where the axes of the precipitate does not align with the axes of the matrix
+        (e.g., the long/short axes of the precipitate is not parallel to the <100> directions of the matrix)
 
         Parameters
         ----------
-        func : function
-            Function taking in z and returning composition
-        element : str
-            Element to apply composition profile to
+        rot : matrix
+            3x3 rotation matrix
         '''
-        eIndex = self._getElementIndex(element)
-        self.x[eIndex,:] = func(self.z)
+        self.rotation = np.array(rot)
+
+    def setRotationPrecipitate(self, rot):
+        self.rotationPrec = np.array(rot)
 
-    def setCompositionProfile(self, z, x, element = None):
+    def setEigenstrain(self, strain):
         '''
-        Sets composition profile by linear interpolation
+        Sets eigenstrain of precipitate
 
         Parameters
         ----------
-        z : array
-            z-coords of composition profile
-        x : array
-            Composition profile
-        element : str
-            Element to apply composition profile to
+        strain : float, array or matrix
+            float - assume strain is the same along all 3 axis
+            array - each index corresponds to strain in a given axis
+            matrix - full 2nd rank strain tensor
+
+        NOTE: when using in conjunction with ShapeFactors, the axis are order specific
+            For needle-like precipitates, x1, x2 and x3 correspond to (short axis, short axis, long axis)
+            For plate-like precipitates, x1, x2 and x3 correspond to (long axis, long axis, short axis)
         '''
-        eIndex = self._getElementIndex(element)
-        z = np.array(z)
-        x = np.array(x)
-        sortIndices = np.argsort(z)
-        z = z[sortIndices]
-        x = x[sortIndices]
-        self.x[eIndex,:] = np.interp(self.z, z, x)
+        strain = np.array(strain)
+        #If scalar, then apply to all 3 axis
+        if (type(strain) == np.ndarray and strain.ndim == 0):
+            self.eigstrain = strain * np.identity(3)
+        #If array of length 3, then apply strain along each index to corresponding axis
+        elif strain.ndim == 1:
+            self.eigstrain = np.array([[strain[0], 0, 0], [0, strain[1], 0], [0, 0, strain[2]]])
+        #Else, assume it's a tensor
+        else:
+            self.eigstrain = strain
 
-    def setup(self):
+    def setAppliedStress(self, stress):
         '''
-        General setup function for all diffusio models
+        Sets applied stress tensor
+        Axes of stress tensor should be the same as the matrix
 
-        This will clear any cached values in the thermodynamics function and check if all compositions add up to 1
+        Parameters
+        ----------
+        stress : float, array or matrix
+            float - assume stress is the same along all 3 axis
+            array - each index corresponds to stress in a given axis
+            matrix - full 2nd rank stress tensor
 
-        This will also make sure that all compositions are not 0 or 1 to speed up equilibrium calculations
-        '''
-        if self.therm is not None:
-            self.therm.clearCache()
-        xsum = np.sum(self.x, axis=0)
-        if any(xsum > 1):
-            print('Compositions add up to above 1 between z = [{:.3e}, {:.3e}]'.format(np.amin(self.z[xsum>1]), np.amax(self.z[xsum>1])))
-            raise Exception('Some compositions sum up to above 1')
-        self.x[self.x > self.minComposition] = self.x[self.x > self.minComposition] - len(self.allElements) * self.minComposition
-        self.x[self.x < self.minComposition] = self.minComposition
-        self.isSetup = True
+        NOTE: The applied stress is in reference to the coordinate axes of the precipitates
+        Thus, this is only valid if the following conditions are met:
+            The matrix phase has a single orientation (either as a single crystal or highly textured)
+            Precipitates will form only in a single orientation with respect to the matrix
 
-    def getFluxes(self):
-        '''
-        "Virtual" function to be implemented by child objects
+        TODO: It will be nice to expand on this.
+            For polycrystalline matrix and randomly oriented precipitates, it should be possible
+            to average the strain energy contributions over all matrix/precipitate orientations
         '''
-        return [], []
+        stress = np.array(stress)
+        #If scalar, then apply to all 3 axis
+        if (type(stress) == np.ndarray and stress.ndim == 0):
+            self.appstress = stress * np.identity(3)
+        #If array of length 3, then apply stress along each index to corresponding axis
+        elif stress.ndim == 1:
+            self.appstress = np.array([[stress[0], 0, 0], [0, stress[1], 0], [0, 0, stress[2]]])
+        #Else, assume it's a tensor
+        else:
+            self.appstress = stress
 
-    def updateMesh(self):
+    def getAppliedStrain(self):
         '''
-        "Virtual" function to be implemented by child objects
+        Calculates applied strain tensor from applied stress tensor and elastic tensor
         '''
-        pass
+        flatStress = self._convert2rankToVec(self.appstress)
+        flatStrain = np.matmul(np.linalg.inv(self.c), flatStress)
+        self.appstrain = self._convertVecTo2rankTensor(flatStrain)
 
-    def update(self):
+    def setup(self):
         '''
-        Updates the mesh by a given dt that is calculated for numerical stability
+        Sets up elastic constants
         '''
-        #Get fluxes
-        fluxes, dt = self.getFluxes()
+        #If no elastic tensor is given, then elastic energy will be constant at 0
+        if self.c is not None:
+            #Apply rotation on matrix phase if there is one
+            #Since applied stress tensor is aligned with matrix, rotate it too since calculations will be in reference to precipitate axes
+            if self.rotation is not None:
+                self._c4 = self._rotateRank4Tensor(self.rotation, self._c4)
+                self.c = self._convert4To2rankTensor(self._c4)
+                self.appstress = self._rotateRank2Tensor(self.rotation, self.appstress)
 
-        if self.t + dt > self.tf:
-            dt = self.tf - self.t
+            #If elastic constants for precipitate are not given, then assume they're the same as the matrix
+            #This will give the elastic energy equation from Wu et al, Journal of Phase Equilibria and Diffusion, 39, 2018
+            #Using a different elastic tensor for the precipitate will give energy from Bohm et al, Mechanics of Materials, 155, 2021
+            if self.cPrec is None:
+                self.cPrec = copy.copy(self.c)
+                self._c4Prec = copy.copy(self._c4)
 
-        #Update mesh
-        self.updateMesh(fluxes, dt)
-        self.x[self.x < self.minComposition] = self.minComposition
-        self.t += dt
+            if self.rotationPrec is not None:
+                self._c4Prec = self._rotateRank4Tensor(self.rotationPrec, self._c4Prec)
+                self.cPrec = self._convert4To2rankTensor(self._c4Prec)
 
-    def solve(self, simTime, verbose=False, vIt=10):
-        '''
-        Solves the model by updated the mesh until the final simulation time is met
-        '''
-        self.setup()
+            self.getAppliedStrain()
 
-        self.t = 0
-        self.tf = simTime
-        i = 0
-        t0 = time.time()
-        if verbose:
-            print('Iteration\tSim Time (h)\tRun time (s)')
-        while self.t < self.tf:
-            if verbose and i % vIt == 0:
-                tf = time.time()
-                print(str(i) + '\t\t{:.3f}\t\t{:.3f}'.format(self.t/3600, tf-t0))
-            self.update()
-            i += 1
+            #Set type to something other than CONSTANT
+            #Since CONSTANT is the only method not requiring the elastic tensor,
+            #    we assume that the user is intending to calculate strain energy when inputting the tensor
+            if self.type == self.CONSTANT:
+                self.type = self.SPHERE
 
-        tf = time.time()
-        print(str(i) + '\t\t{:.3f}\t\t{:.3f}'.format(self.t/3600, tf-t0))
-
-    def getX(self, element):
+    #Utility functions for tensors
+    def _convert2To4rankTensor(self, c):
         '''
-        Gets composition profile of element
-        
+        Converts 2nd rank elastic tensor to 4th rank
+
         Parameters
         ----------
-        element : str
-            Element to get profile of
+        c : ndarray
+            2nd rank elastic tensor
+
+        Returns
+        -------
+        c4 : ndarray
+            4th rank elastic tensor
         '''
-        if element in self.allElements and element not in self.elements:
-            return 1 - np.sum(self.x, axis=0)
-        else:
-            e = self._getElementIndex(element)
-            return self.x[e]
+        vMap = {frozenset({0}): 0, frozenset({1}): 1, frozenset({2}): 2,
+                frozenset({1,2}): 3, frozenset({0,2}): 4, frozenset({0,1}): 5}
+
+        c4 = np.zeros((3,3,3,3))
+        for i, j, k, l in itertools.product(range(3), range(3), range(3), range(3)):
+            c4[i,j,k,l] = c[vMap[frozenset({i,j})], vMap[frozenset({k,l})]]
+        return c4
 
-    def getP(self, phase):
+    def _convert4To2rankTensor(self, c4):
         '''
-        Gets phase profile
+        Converts 4th rank elastic tensor to 4nd rank
 
         Parameters
         ----------
-        phase : str
-            Phase to get profile of
+        c4 : ndarray
+            4th rank elastic tensor
+
+        Returns
+        -------
+        c : ndarray
+            2nd rank elastic tensor
         '''
-        p = self._getPhaseIndex(phase)
-        return self.p[p]
+        vMap = [[0,0], [1,1], [2,2], [1,2], [0,2], [0,1]]
+        c = np.zeros((6,6))
+        for i, j in itertools.product(range(6), range(6)):
+            c[i,j] = c4[vMap[i][0], vMap[i][1], vMap[j][0], vMap[j][1]]
+        return c
 
-    def plot(self, ax, plotReference = True, plotElement = None, zScale = 1, *args, **kwargs):
+    def _invert4rankTensor(self, c4):
         '''
-        Plots composition profile
+        Inverts 4th rank tensor to give stiffness tensor
 
-        Parameters
-        ----------
-        ax : matplotlib Axes object
-            Axis to plot on
-        plotReference : bool
-            Whether to plot reference element (composition = 1 - sum(composition of rest of elements))
-        plotElement : None or str
-            Plots single element if it is defined, otherwise, all elements are plotted
-        zScale : float
-            Scale factor for z-coordinates
+        This is done by converting to 2nd rank, inverting, then converting back to 4th rank
         '''
-        if not self.isSetup:
-            self.setup()
+        c = self._convert4To2rankTensor(c4)
+        return self._convert2To4rankTensor(np.linalg.inv(c))
 
-        if plotElement is not None:
-            if plotElement not in self.elements and plotElement in self.allElements:
-                x = 1 - np.sum(self.x, axis=0)
-            else:
-                e = self._getElementIndex(plotElement)
-                x = self.x[e]
-            ax.plot(self.z/zScale, x, *args, **kwargs)
-        else:
-            if plotReference:
-                refE = 1 - np.sum(self.x, axis=0)
-                ax.plot(self.z/zScale, refE, label=self.allElements[0], *args, **kwargs)
-            for e in range(len(self.elements)):
-                ax.plot(self.z/zScale, self.x[e], label=self.elements[e], *args, **kwargs)
-            
-        ax.set_xlim([self.zlim[0]/zScale, self.zlim[1]/zScale])
-        ax.legend()
-        ax.set_xlabel('Distance (m)')
-        ax.set_ylabel('Composition (at.%)')
-
-    def plotTwoAxis(self, axL, Lelements, Relements, zScale = 1, *args, **kwargs):
-        '''
-        Plots composition profile with two y-axes
+    def _convertVecTo2rankTensor(self, v):
+        '''
+        Converts strain/stress vector to 2nd rank tensor
 
         Parameters
         ----------
-        axL : matplotlib Axes object
-            Left axis to plot on
-        Lelements : list of str
-            Elements to plot on left axis
-        Relements : list of str
-            Elements to plot on right axis
-        zScale : float
-            Scale factor for z-coordinates
-        '''
-        if not self.isSetup:
-            self.setup()
-
-        if type(Lelements) is str:
-            Lelements = [Lelements]
-        if type(Relements) is str:
-            Relements = [Relements]
-
-        ci = 0
-        refE = 1 - np.sum(self.x, axis=0)
-        axR = axL.twinx()
-        for e in range(len(Lelements)):
-            if Lelements[e] in self.elements:
-                eIndex = self._getElementIndex(Lelements[e])
-                axL.plot(self.z/zScale, self.x[eIndex], label=self.elements[eIndex], color = 'C' + str(ci), *args, **kwargs)
-                ci = ci+1 if ci <= 9 else 0
-            elif Lelements[e] in self.allElements:
-                axL.plot(self.z/zScale, refE, label=self.allElements[0], color = 'C' + str(ci), *args, **kwargs)
-                ci = ci+1 if ci <= 9 else 0
-        for e in range(len(Relements)):
-            if Relements[e] in self.elements:
-                eIndex = self._getElementIndex(Relements[e])
-                axR.plot(self.z/zScale, self.x[eIndex], label=self.elements[eIndex], color = 'C' + str(ci), *args, **kwargs)
-                ci = ci+1 if ci <= 9 else 0
-            elif Relements[e] in self.allElements:
-                axR.plot(self.z/zScale, refE, label=self.allElements[0], color = 'C' + str(ci), *args, **kwargs)
-                ci = ci+1 if ci <= 9 else 0
+        v : 1d array
+            Strain/stress vector
 
-        
-        axL.set_xlim([self.zlim[0]/zScale, self.zlim[1]/zScale])
-        axL.set_xlabel('Distance (m)')
-        axL.set_ylabel('Composition (at.%) ' + str(Lelements))
-        axR.set_ylabel('Composition (at.%) ' + str(Relements))
-        
-        lines, labels = axL.get_legend_handles_labels()
-        lines2, labels2 = axR.get_legend_handles_labels()
-        axR.legend(lines+lines2, labels+labels2, framealpha=1)
-
-        return axL, axR
-
-    def plotPhases(self, ax, plotPhase = None, zScale = 1, *args, **kwargs):
+        Returns
+        -------
+        e : ndarray
+            2nd rank elastic tensor
         '''
-        Plots phase fractions over z
+        return np.array([[v[0], v[5], v[4]], \
+                        [v[5], v[1], v[3]], \
+                        [v[3], v[4], v[2]]])
 
-        Parameters
-        ----------
-        ax : matplotlib Axes object
-            Axis to plot on
-        plotPhase : None or str
-            Plots single phase if it is defined, otherwise, all phases are plotted
-        zScale : float
-            Scale factor for z-coordinates
+    def _convert2rankToVec(self, c):
         '''
-        if not self.isSetup:
-            self.setup()
+        Converts 2nd rank tensor to vector
 
-        if plotPhase is not None:
-            p = self._getPhaseIndex(plotPhase)
-            ax.plot(self.z/zScale, self.p[p], *args, **kwargs)
-        else:
-            for p in range(len(self.phases)):
-                ax.plot(self.z/zScale, self.p[p], label=self.phases[p], *args, **kwargs)
-        ax.set_xlim([self.zlim[0]/zScale, self.zlim[1]/zScale])
-        ax.set_ylim([0, 1])
-        ax.set_xlabel('Distance (m)')
-        ax.set_ylabel('Phase Fraction')
-        ax.legend()
-
-class SinglePhaseModel(DiffusionModel):
-    def getFluxes(self):
-        '''
-        Gets fluxes at the boundary of each nodes
+        Parameter
+        ---------
+        c : ndarray
+            3x3 tensor
 
         Returns
         -------
-        fluxes : (e-1, n+1) array of floats
-            e - number of elements including reference element
-            n - number of nodes
-        dt : float
-            Maximum calculated time interval for numerical stability
+        v : 1darray
+            Strain/stress vector
         '''
-        xMid = (self.x[:,1:] + self.x[:,:-1]) / 2
+        return np.array([c[0,0], c[1,1], c[2,2], c[1,2], c[0,2], c[0,1]])
 
-        if len(self.elements) == 1:
-            d = np.zeros(self.N-1)
-        else:
-            d = np.zeros((self.N-1, len(self.elements), len(self.elements)))
-        if self.cache:
-            for i in range(self.N-1):
-                hashValue = self._getHash(xMid[:,i])
-                if hashValue not in self.hashTable:
-                    self.hashTable[hashValue] = self.therm.getInterdiffusivity(xMid[:,i], self.T, phase=self.phases[0])
-                d[i] = self.hashTable[hashValue]
-        else:
-            d = self.therm.getInterdiffusivity(xMid.T, self.T*np.ones(self.N-1), phase=self.phases[0])
-
-        dxdz = (self.x[:,1:] - self.x[:,:-1]) / self.dz
-        fluxes = np.zeros((len(self.elements), self.N+1))
-        if len(self.elements) == 1:
-            fluxes[0,1:-1] = -d * dxdz
-        else:
-            dxdz = np.expand_dims(dxdz, axis=0)
-            fluxes[:,1:-1] = -np.matmul(d, np.transpose(dxdz, (2,1,0)))[:,:,0].T
-        for e in range(len(self.elements)):
-            fluxes[e,0] = self.LBCvalue[e] if self.LBC[e] == self.FLUX else fluxes[e,1]
-            fluxes[e,-1] = self.RBCvalue[e] if self.RBC[e] == self.FLUX else fluxes[e,-2]
-
-        dt = 0.4 * self.dz**2 / np.amax(np.abs(d))
+    def _rotateRank2Tensor(self, rot, tensor):
+        '''
+        Rotates a 2nd rank tensor
+        T_ij = r_il * r_jk * T_lk
 
-        return fluxes, dt
+        Parameters
+        ----------
+        tensor : ndarray
+            2nd rank tensor to rotate (3x3 array)
+        '''
+        return np.tensordot(rot,
+                np.tensordot(rot, tensor, axes=(1,1)), axes=(1,1))
 
-    def updateMesh(self, fluxes, dt):
+    def _rotateRank4Tensor(self, rot, tensor):
         '''
-        Updates mesh using fluxes by time increment dt
+        Rotates a 4th rank tensor
+        T_ijkl = r_im * r_jn * r_ok * r_lp * T_mnop
 
         Parameters
         ----------
-        fluxes : 2D array
-            Fluxes for each element between each node. Size must be (E, N-1)
-                E - number of elements (NOT including reference element)
-                N - number of nodes
-            Boundary conditions will automatically be applied
-        dt : float
-            Time increment
+        tensor : ndarray
+            4th rank tensor to rotate (3x3x3x3 array)
         '''
-        for e in range(len(self.elements)):
-            self.x[e] += -(fluxes[e,1:] - fluxes[e,:-1]) * dt / self.dz
+        return np.tensordot(rot, 
+                np.tensordot(rot, 
+                np.tensordot(rot, 
+                np.tensordot(rot, tensor, axes=(1,3)), axes=(1,3)), axes=(1,3)), axes=(1,3))
 
-class HomogenizationModel(DiffusionModel):
-    def __init__(self, zlim, N, elements = ['A', 'B'], phases = ['alpha']):
-        super().__init__(zlim, N, elements, phases)
+    def setIntegrationIntervals(self, phiInt, thetaInt, assumeSymmetric=True):
+        '''
+        Number of intervals to split domain along phi and theta for integration
 
-        self.mobilityFunction = self.wienerUpper
-        self.defaultMob = 0
-        self.eps = 0.05
+        Parameters
+        ----------
+        phiInt : int
+            Number of intervals to divide along phi
+        thetaInt : int
+            Number of intervals to divide along theta
+        assumeSymmetric : bool (optional)
+            If True (default), will only integrate Eshelby's tensor on a single quadrant and
+            multiply the results by 8
+        '''
+        #If assume symmetric, then only a single quadrant will be integrated over
+        phiRange = np.pi/2 if assumeSymmetric else 2*np.pi
+        thetaRange = np.pi/2 if assumeSymmetric else np.pi
+        dphi = phiRange / phiInt
+        dtheta = thetaRange / thetaInt
+        midPhi = np.linspace(dphi/2, phiRange - dphi/2, phiInt)
+        midTheta = np.linspace(dtheta/2, thetaRange - dtheta/2, thetaInt)
+        self.dA = dtheta*dphi if assumeSymmetric else 1/8 * dtheta*dphi
 
-        self.sortIndices = np.argsort(self.allElements)
-        self.unsortIndices = np.argsort(self.sortIndices)
-        self.labFactor = 1
+        #Cartesian product of phi and theta intervals
+        self.midPhiGrid, self.midThetaGrid = np.meshgrid(midPhi, midTheta)
+        self.midPhiGrid = self.midPhiGrid.ravel()
+        self.midThetaGrid = self.midThetaGrid.ravel()
+        self.midWeights = np.sin(self.midThetaGrid)
 
-    def reset(self):
+    def lebedevIntegration(self, order = 'high'):
         '''
-        Resets model
+        Creates Lebedev quadrature points and nodes for integrating Eshebly's tensor
+        This is preferred over discretizing phi and theta
 
-        This also includes chemical potential and pycalphad CompositionSets for each node
+        Parameters
+        ----------
+        order : str
+            'low' - uses quadrature order or 53 (974 points)
+            'mid' - uses quadrature order or 83 (2354 points)
+            'high' (default) - uses quadrature order or 131 (5810 points)
         '''
-        super().reset()
-        self.mu = np.zeros((len(self.elements)+1, self.N))
-        self.compSets = [None for _ in range(self.N)]
+        if order == 'low':
+            order = 53
+        elif order == 'mid':
+            order = 83
+        else:
+            order = 131
 
-    def setMobilityFunction(self, function):
-        '''
-        Sets averaging function to use for mobility
+        self.midPhiGrid, self.midThetaGrid, self.midWeights = loadPoints(order)
+        self.dA = np.pi/2
 
-        Default mobility value should be that a phase of unknown mobility will be ignored for average mobility calcs
+    def _n(self, phi, theta):
+        '''
+        Unit normal vector of sphere
 
         Parameters
         ----------
-        function : str
-            Options - 'upper wiener', 'lower wiener', 'upper hashin-shtrikman', 'lower hashin-strikman', 'labyrinth'
+        phi - azimuthal angle
+        theta - polar angle
         '''
-        #np.finfo(dtype).max - largest representable value
-        #np.finfo(dtype).tiny - smallest positive usable value
-        if 'upper' in function and 'wiener' in function:
-            self.mobilityFunction = self.wienerUpper
-            self.defaultMob = np.finfo(np.float64).tiny
-        elif 'lower' in function and 'wiener' in function:
-            self.mobilityFunction = self.wienerLower
-            self.defaultMob = np.finfo(np.float64).max
-        elif 'upper' in function and 'hashin' in function:
-            self.mobilityFunction = self.hashin_shtrikmanUpper
-            self.defaultMob = np.finfo(np.float64).tiny
-        elif 'lower' in function and 'hashin' in function:
-            self.mobilityFunction = self.hashin_shtrikmanLower
-            self.defaultMob = np.finfo(np.float64).max
-        elif 'lab' in function:
-            self.mobilityFunction = self.labyrinth
-            self.defaultMob = np.finfo(np.float64).tiny
-
-    def setLabyrinthFactor(self, n):
+        return np.array([np.sin(theta)*np.cos(phi), np.sin(theta)*np.sin(phi), np.cos(theta)])
+    
+    def _beta(self, a, b, c, phi, theta):
         '''
-        Labyrinth factor
+        Distance from center to surface of ellipsoid
 
         Parameters
         ----------
-        n : int
-            Either 1 or 2
-            Note: n = 1 will the same as the weiner upper bounds
+        a, b, c - radii of ellipsoid along x,y,z axes
+        phi, theta - azimuthal, polar angle
         '''
-        if n < 1:
-            n = 1
-        if n > 2:
-            n = 2
-        self.labFactor = n
+        return np.sqrt(((a*np.cos(phi))**2 + (b*np.sin(phi))**2)*np.sin(theta)**2 + (c*np.cos(theta))**2)
 
-    def setup(self):
+    def _OhmGeneral(self, n):
         '''
-        Sets up model
+        Ohm term for general system
 
-        This also includes getting the CompositionSets for each node
+        Ohm_ij = inverse(C_iklj * n_k * n_l)
         '''
-        super().setup()
-        #self.midX = 0.5 * (self.x[:,1:] + self.x[:,:-1])
-        self.p = self.updateCompSets(self.x)
+        invOhm = np.tensordot(self._c4, np.tensordot(n, n, axes=0), axes=[[1,2], [0,1]])
+        return np.linalg.inv(invOhm)
+    
+    def _ohm_quickInverse(self, m):
+        '''
+        Hard coded inverse of m which is of shape (3,3,n)
+
+        numpy inv is more optimized for larger matrices, but can be slower for small
+        matrices such as a 2x2 or 3x3. We can take advantage of 3x3 matrices having a computable
+        inverse to make it faster
 
-    def _newEqCalc(self, x):
+        NOTE: this only works since we know that m has a shape of (3,3,n) and is only composed of real numbers
+
+        This function can probably be a bit more efficient, but quick 
+        profiling on sphInt gives around a 35x speedup compared to doing 
+        np.transpose(np.linalg.inv(np.transpose(m, (2,0,1))), (1,2,0)) 
+        where the slowdown was in np.linalg.inv
+
+        For matrix:
+            |  a  b  c  |
+            |  d  e  f  |
+            |  g  h  i  |
+
+        Inverse is defined as:
+            |  ei-fh  fg-di  dh-eg  |          |  A  B  C  |
+            |  ch-bi  ai-cg  bg-ah  | / det -> |  D  E  F  | / det
+            |  bf-ce  cd-af  ae-bd  |          |  G  H  I  |
+            Where det = aA + bB + cC
         '''
-        Calculates equilibrium and returns a CompositionSet
+        a, b, c, d, e, f, g, h, i = m[0,0], m[0,1], m[0,2], m[1,0], m[1,1], m[1,2], m[2,0], m[2,1], m[2,2]
+        A = e*i - f*h
+        B = f*g - d*i
+        C = d*h - e*g
+        D = c*h - b*i
+        E = a*i - c*g
+        F = b*g - a*h
+        G = b*f - c*e
+        H = c*d - a*f
+        I = a*e - b*d
+        det = a*A + b*B + c*C
+        return np.array([[A, B, C], [D, E, F], [G, H, I]]) / det
+    
+    def _ohm_npinv(self, m):
         '''
-        eq = self.therm.getEq(x, self.T, 0, self.phases)
-        state_variables = np.array([0, 1, 101325, self.T], dtype=np.float64)
-        stable_phases = eq.Phase.values.ravel()
-        phase_amounts = eq.NP.values.ravel()
-        comp = []
-        for p in stable_phases:
-            if p != '':
-                idx = np.where(stable_phases == p)[0]
-                cs, misc = self.therm._createCompositionSet(eq, state_variables, p, phase_amounts, idx)
-                comp.append(cs)
+        Inverts ohm term using np.linalg.inv
 
-        if len(comp) == 0:
-            comp = None
-
-        return self.therm.getLocalEq(x, self.T, 0, self.phases, comp)
+        numpy inverse function takes in an array of shape (m,n,n) and inverts each nxn matrix
+            So we have to transpose m from (3,3,n) -> (n,3,3), then invert, then transpose (n,3,3) ->(3,3,n)
+        '''
+        return np.transpose(np.linalg.inv(np.transpose(m, (2,0,1))), (1,2,0))
 
-    def updateCompSets(self, xarray):
+    def sphInt(self):
+        '''
+        Faster version of calculating the Dijkl, which avoids
+        using a for loop to iterate across phi and theta
         '''
-        Updates the array of CompositionSets
+        #Normal vector (1 x 3 x n) where n is number of integration points
+        n = self._n(self.midPhiGrid, self.midThetaGrid)
+        nexp = np.expand_dims(n, axis=0)
 
-        If an equilibrium calculation is already done for a given composition, 
-        the CompositionSet will be taken out of the hash table
+        #n_i*n_j for each grid point (n x 3 x 1) x (n x 1 x 3) = (n x 3 x 3) -> (3 x 3 x n)
+        nProd = np.matmul(np.transpose(nexp, (2,1,0)), np.transpose(nexp, (2,0,1))).transpose((1,2,0))
 
-        Otherwise, a new equilibrium calculation will be performed
+        #End term inside integral = sin(theta) / beta**3
+        #endTerm = np.sin(self.midThetaGrid) / self._beta(self.r[0], self.r[1], self.r[2], self.midPhiGrid, self.midThetaGrid)**3
+        endTerm = 1 / self._beta(self.r[0], self.r[1], self.r[2], self.midPhiGrid, self.midThetaGrid)**3
 
-        Parameters
-        ----------
-        xarray : (e-1, N) array
-            Composition for each node
-            e is number of elements
-            N is number of nodes
+        #Ohm term (Ohm_ij = inverse(C_iklj * n_k * n_l))
+        #For all grid points (Ohm_ijn = inverse(C_iklj) * nProd_kln)
+        invOhm = np.tensordot(self._c4, nProd, axes=[[1,2], [0,1]])
 
-        Returns
-        -------
-        parray : (p, N) array
-            Phase fractions for each node
-            p is number of phases
-        '''
-        parray = np.zeros((len(self.phases), xarray.shape[1]))
-        for i in range(parray.shape[1]):
-            if self.cache:
-                hashValue = self._getHash(xarray[:,i])
-                if hashValue not in self.hashTable:
-                    result, comp = self._newEqCalc(xarray[:,i])
-                    #result, comp = self.therm.getLocalEq(xarray[:,i], self.T, 0, self.phases, self.compSets[i])
-                    self.hashTable[hashValue] = (result, comp, None)
-                else:
-                    result, comp, _ = self.hashTable[hashValue]
-                results, self.compSets[i] = copy.copy(result), copy.copy(comp)
-            else:
-                if self.compSets[i] is None:
-                    results, self.compSets[i] = self._newEqCalc(xarray[:,i])
-                else:
-                    results, self.compSets[i] = self.therm.getLocalEq(xarray[:,i], self.T, 0, self.phases, self.compSets[i])
-            self.mu[:,i] = results.chemical_potentials[self.unsortIndices]
-            cs_phases = [cs.phase_record.phase_name for cs in self.compSets[i]]
-            for p in range(len(cs_phases)):
-                parray[self._getPhaseIndex(cs_phases[p]), i] = self.compSets[i][p].NP
-        
-        return parray
+        ohm = self._ohm_inverse(invOhm)
 
-    def getMobility(self, xarray):
-        '''
-        Gets mobility of all phases
+        #Tensor product (D_ijkl = intergral(ohm_ij * n_k * n_l * endTerm))
+        #For summing over grid points (D_ijkl = ohm_ij * nProd_kln * endTerm_n)
+        d = np.tensordot(ohm, np.multiply(nProd, endTerm * self.midWeights), axes=[[2], [2]])
 
-        Returns
-        -------
-        (p, e+1, N) array - p is number of phases, e is number of elements, N is number of nodes
+        #Multiply by differential area and across the 8 quadrants
+        return 8*d*self.dA
+
+    def Dijkl(self):
         '''
-        mob = self.defaultMob * np.ones((len(self.phases), len(self.elements)+1, xarray.shape[1]))
-        for i in range(xarray.shape[1]):
-            if self.cache:
-                hashValue = self._getHash(xarray[:,i])
-                _, _, mTemp = self.hashTable[hashValue]
-            else:
-                mTemp = None
-            if mTemp is None or not self.cache:
-                maxPhaseAmount = 0
-                maxPhaseIndex = 0
-                for p in range(len(self.phases)):
-                    if self.p[p,i] > 0:
-                        if self.p[p,i] > maxPhaseAmount:
-                            maxPhaseAmount = self.p[p,i]
-                            maxPhaseIndex = p
-                        if self.phases[p] in self.therm.mobCallables and self.therm.mobCallables[self.phases[p]] is not None:
-                            #print(self.phases, self.phases[p], xarray[:,i], self.p[:,i], i, self.compSets[i])
-                            compset = [cs for cs in self.compSets[i] if cs.phase_record.phase_name == self.phases[p]][0]
-                            mob[p,:,i] = mobility_from_composition_set(compset, self.therm.mobCallables[self.phases[p]], self.therm.mobility_correction)[self.unsortIndices]
-                            mob[p,:,i] *= np.concatenate(([1-np.sum(xarray[:,i])], xarray[:,i]))
-                        else:
-                            mob[p,:,i] = -1
-                for p in range(len(self.phases)):
-                    if any(mob[p,:,i] == -1) and not all(mob[p,:,i] == -1):
-                        mob[p,:,i] = mob[maxPhaseIndex,:,i]
-                    if all(mob[p,:,i] == -1):
-                        mob[p,:,i] = self.defaultMob
-                if self.cache:
-                    self.hashTable[hashValue] = (self.hashTable[hashValue][0], self.hashTable[hashValue][1], copy.copy(mob[:,:,i]))
-            else:
-                mob[:,:,i] = mTemp
+        Dijkl term for Eshelby's theory
+        '''
+        #return -np.prod(self.r)/(4*np.pi) * self.sphericalIntegral(self.Dfunc)
+        return -np.prod(self.r)/(4*np.pi) * self.sphInt()
 
-        return mob
+    def Sijmn(self, D):
+        '''
+        S_ijmn = -0.5 * C_lkmn * (D_iklj + D_jkli)
+        '''
+        S = -0.5 * np.tensordot(self._c4, D + np.transpose(D, (3,1,2,0)), axes=[[0,1],[2,1]])
+        #The tensor product gives S_mnij so we'll need to transpose it
+        return np.transpose(S, (2,3,0,1))
 
-    def wienerUpper(self, xarray):
+    def _multiply(self, a, b):
+        '''
+        Multiplies 2 tensors
+        4th x 2nd -> c_ij = a_ijkl * b_kl
+        4th x 4th -> c_ijkl = a_ijmn * b_mnkl
         '''
-        Upper wiener bounds for average mobility
+        return np.tensordot(a, b, axes=[[2,3], [0,1]])
 
-        Returns
-        -------
-        (e+1, N) mobility array - e is number of elements, N is number of nodes
+    def _strainEnergy(self, stress, strain, V):
+        '''
+        u = -0.5 * V * sigma_ij * strain_ij
         '''
-        mob = self.getMobility(xarray)
-        avgMob = np.sum(np.multiply(self.p[:,np.newaxis], mob), axis=0)
-        return avgMob
+        return -0.5 * V * np.sum(stress * strain)
 
-    def wienerLower(self, xarray):
+    def _strainEnergyEllipsoidWithStress(self):
+        '''
+        Strain energy of ellipsoidal particle with applied stress
         '''
-        Lower wiener bounds for average mobility
+        V = 4*np.pi/3 * np.prod(self.r)
+        S = self.Sijmn(self.Dijkl())
+        stress = self._multiply(self._c4, self._multiply(S, self.eigstrain) - self.eigstrain)
+        stress0 = self._multiply(self._c4, self._multiply(S, self.appstrain) - self.appstrain)
+        return self._strainEnergy(stress - stress0, self.eigstrain - self.appstrain, V)
 
-        Returns
-        -------
-        (e+1, N) mobility array - e is number of elements, N is number of nodes
+    def _strainEnergyEllipsoid(self):
+        '''
+        Strain energy of ellipsoidal particle
         '''
-        #(p, e, N)
-        mob = self.getMobility(xarray)
-        avgMob = 1/np.sum(np.multiply(self.p[:,np.newaxis], 1/mob), axis=0)
-        return avgMob
+        V = 4*np.pi/3 * np.prod(self.r)
+        S = self.Sijmn(self.Dijkl())
+        stress = self._multiply(self._c4, self._multiply(S, self.eigstrain) - self.eigstrain)
+        return self._strainEnergy(stress, self.eigstrain, V)
 
-    def labyrinth(self, xarray):
+    def _strainEnergyEllipsoid2(self):
         '''
-        Labyrinth mobility
+        Alternative method of strain energy on ellipsoidal particle using 2nd rank tensors
+        '''
+        V = 4*np.pi/3 * np.prod(self.r)
+        S = self._convert4To2rankTensor(self.Sijmn(self.Dijkl()))
+        eigFlat = self._convert2rankToVec(self.eigstrain)
+        multTerm = np.matmul(self.c, S - np.eye(6))
+        return -0.5 * V * np.matmul(eigFlat, np.matmul(multTerm, eigFlat))
 
-        Returns
-        -------
-        (e+1, N) mobility array - e is number of elements, N is number of nodes
+    def _strainEnergyBohm(self):
+        '''
+        Strain energy of particle for when matrix and precipitate phases have different elastic tensors
         '''
-        mob = self.getMobility(xarray)
-        avgMob = np.sum(np.multiply(np.power(self.p[:,np.newaxis], self.labFactor), mob), axis=0)
-        return avgMob
+        V = 4*np.pi/3 * np.prod(self.r)
+        S = self.Sijmn(self.Dijkl())
+        #invTerm = np.linalg.tensorinv(self._multiply(self._c4Prec - self._c4, S) + self._c4)
+        invTerm = self._invert4rankTensor(self._multiply(self._c4Prec - self._c4, S) + self._c4)
+        multTerm = self._multiply(invTerm, self._c4Prec)
+        stressC = self._multiply(self._c4, self._multiply(self._multiply(S, multTerm), self.eigstrain))
+        stress0 = self._multiply(self._c4, self._multiply(multTerm, self.eigstrain))
+        return self._strainEnergy(stressC-stress0, self.eigstrain, V)
 
-    def hashin_shtrikmanUpper(self, xarray):
+    def _strainEnergyBohm2(self):
+        '''
+        Strain energy of particle for when matrix and precipitate phases have different elastic tensors using 2nd rank tensors
         '''
-        Upper hashin shtrikman bounds for average mobility
+        V = 4*np.pi/3 * np.prod(self.r)
+        S = self._convert4To2rankTensor(self.Sijmn(self.Dijkl()))
+        eigFlat = self._convert2rankToVec(self.eigstrain)
+        invTerm = np.linalg.inv(np.matmul(self.cPrec - self.c, S) + self.c)
+        multTerm = np.matmul(invTerm, self.cPrec)
+        stressC = np.matmul(self.c, np.matmul(np.matmul(S, multTerm), eigFlat))
+        stress0 = np.matmul(self.c, np.matmul(multTerm, eigFlat))
+        return -0.5 * V * np.matmul(eigFlat, stressC - stress0)
 
-        Returns
-        -------
-        (e+1, N) mobility array - e is number of elements, N is number of nodes
+    def _Khachaturyan(self, I1, I2):
+        '''
+        Khachaturyan's approximation for strain energy of spherical and cuboidal precipitates
         '''
-        #self.p                                 #(p,N)
-        mob = self.getMobility(xarray)          #(p,e+1,N)
-        maxMob = np.amax(mob, axis=0)           #(e+1,N)
-
-        # 1 / ((1 / mPhi - mAlpha) + 1 / (3mAlpha)) = 3mAlpha * (mPhi - mAlpha) / (2mAlpha + mPhi)
-        Ak = 3 * maxMob * (mob - maxMob) / (2*maxMob + mob)
-        Ak = Ak * self.p[:,np.newaxis]
-        Ak = np.sum(Ak, axis=0)
-        avgMob = maxMob + Ak / (1 - Ak / (3*maxMob))
-        return avgMob
+        V = 4*np.pi/3 * np.prod(self.r)
+        A1 = 2 * (self.c[0,0] - self.c[0,1]) / self.c[0,0]
+        A1 -= 12 * (self.c[0,0] + 2 * self.c[0,1]) * (self.c[0,0] - self.c[0,1] - 2 * self.c[3,3]) / (self.c[0,0] * (self.c[0,0] + self.c[0,1] + 2*self.c[3,3])) * I1
+        A2 = -54 * (self.c[0,0] + 2 * self.c[0,1]) * (self.c[0,0] - self.c[0,1] - 2 * self.c[3,3])**2 / (self.c[0,0] * (self.c[0,0] + self.c[0,1] + 2 * self.c[3,3]) * (self.c[0,0] + 2 * self.c[0,1] + 4 * self.c[3,3])) * I2
+        return 0.5 * (self.c[0,0] + 2 * self.c[0,1]) * (A1 + A2) * self.eigstrain[0,0]**2 * V
 
-    def hashin_shtrikmanLower(self, xarray):
+    def _strainEnergyCube(self):
         '''
-        Lower hashin shtrikman bounds for average mobility
+        Strain energy of perfect cube (cubic factor = sqrt(2))
+        '''
+        return self._Khachaturyan(0.006931, 0.000959)
+    
+    def _strainEnergySphere(self):
+        '''
+        Strain energy of perfect sphere (cubic factor = 1)
+        '''
+        return self._Khachaturyan(1/15, 1/105)
 
-        Returns
-        -------
-        (e, N) mobility array - e is number of elements, N is number of nodes
+    def _strainEnergyCuboidal(self, eta = 1):
         '''
-        #self.p                                 #(p,N)
-        mob = self.getMobility(xarray)          #(p,e+1,N)
-        minMob = np.amin(mob, axis=0)           #(e+1,N)
+        For cuboidal preciptitates, strain energy can be approximated
+        as a linear interpolation between a perfect cube and sphere
+        '''
+        sC = self.strainEnergyCube()
+        sS = self.strainEnergySphere()
+        return (sC - sS) * (eta - 1) / (np.sqrt(2) - 1) + sS
 
-        #This prevents an infinite mobility which could cause the time interval to be 0
-        minMob[minMob == np.inf] = 0
+    def _strainEnergyConstant(self):
+        return 4 * np.pi / 3 * np.prod(self.r) * self._gElasticConstant
 
-        # 1 / ((1 / mPhi - mAlpha) + 1 / (3mAlpha)) = 3mAlpha * (mPhi - mAlpha) / (2mAlpha + mPhi)
-        Ak = 3 * minMob * (mob - minMob) / (2*minMob + mob)
+    def _strainEnergySingle(self, rsingle):
+        '''
+        Generic strain energy function
+        '''
+        self.r = rsingle
+        self._prevEnergy = self._prevEnergy if np.array_equal(self.r, self.oldr) else self._strainEnergyGeneric()
+        self.oldr = self.r
+        return self._prevEnergy
 
-        Ak = Ak * self.p[:,np.newaxis]
-        Ak = np.sum(Ak, axis=0)
-        avgMob = minMob + Ak / (1 - Ak / (3*minMob))
-        return avgMob
+    def strainEnergy(self, r):
+        r = np.array(r)
+        #If single set of radii
+        if r.ndim == 1:
+            return self._strainEnergySingle(r)
+        else:
+            eng = np.zeros(len(r))
+            for i in range(len(r)):
+                eng[i] = self._strainEnergySingle(r[i])
+            return eng
+
+    #Additional methods for verifying that the general methods reduce to these
+    #specific cases for cubic crystal symmetry
+    def _OhmCubic(self, n):
+        '''
+        Ohm term for cubic crystal symmetry
+        '''
+        ohm = np.zeros((3,3))
+        jk = [(1,2), (0,2), (0,1)]
+        for i in range(3):
+            for j in range(3):
+                if i == j:
+                    jn, k = jk[i]
+                    ohm[i,i] = (self.c[3,3] + (self.c[0,0]-self.c[3,3])*(n[jn]**2 + n[k]**2) + self._xi*(self.c[0,0]+self.c[0,1])*(n[jn]*n[k])**2) / (self.c[3,3]*self._D(n))
+                else:
+                    k = 3 - (i + j)
+                    ohm[i,j] = -(self.c[0,1] + self.c[3,3])*(1 + self._xi*n[k]**2)*n[i]*n[j] / (self.c[3,3]*self._D(n))
+        
+        return ohm
 
-    def getFluxes(self):
+    def _D(self, n):
         '''
-        Return fluxes and time interval for the current iteration
+        Needed for the Ohm term with cubic crystal symmetry
+        '''
+        d = self.c[0,0]
+        d += self._xi*(self.c[0,0] + self.c[0,1])*((n[0]*n[1])**2 + (n[0]*n[2])**2 + (n[1]*n[2])**2)
+        d += self._xi**2 * (self.c[0,0] + 2*self.c[0,1] + self.c[3,3])*(n[0]*n[1]*n[2])**2
+        return d
+
+    @property
+    def _xi(self):
+        '''
+        Needed for the Ohm term with cubic crystal symmetry
+        '''
+        return (self.c[0,0] - self.c[0,1] - 2*self.c[3,3]) / self.c[3,3]
+
+    #Equilibrium aspect ratios
+    #Determined by minimum of strain energy + interfacial energy
+    def eqAR_byGR(self, Rsph, gamma, shpFactor, a=1.001, b=100):
         '''
-        self.p = self.updateCompSets(self.x)
+        Equilibrium aspect ratio using golden ratio search
 
-        #Get average mobility between nodes
-        avgMob = self.mobilityFunction(self.x)
-        avgMob = 0.5 * (avgMob[:,1:] + avgMob[:,:-1])
+        Parameters
+        ----------
+        Rsph : float or array
+            Equivalent spherical radius
+        gamma : float
+            Interfacial energy
+        shpFactor : ShapeFactor object
+        a, b : float
+            Min and max bounds
+            Default is 1.001 and 100
+        '''
+        normR = shpFactor._normalRadiiEquation
+        interfacial = shpFactor._thermoEquation if self.ifmethod == 1 else shpFactor._eqRadiusEquation
+        if hasattr(Rsph, '__len__'):
+            eqAR = np.ones(len(Rsph))
+            for i in range(len(Rsph)):
+                eqAR[i] = self._GRsearch(Rsph[i], gamma, interfacial, normR, a, b)
+        else:
+            eqAR = self._GRsearch(Rsph, gamma, interfacial, normR, a, b)
 
-        #Composition between nodes
-        avgX = 0.5 * (self.x[:,1:] + self.x[:,:-1])
-        avgX = np.concatenate(([1-np.sum(avgX, axis=0)], avgX), axis=0)
+        return eqAR
 
-        #Chemical potential gradient
-        dmudz = (self.mu[:,1:] - self.mu[:,:-1]) / self.dz
+    def _GRsearch(self, Rsph, gamma, interfacial, normR, a, b):
+        '''
+        Golden ratio search for a single radius
+        '''
+        f = lambda ar: self.strainEnergy(normR(ar))*(4/3)*np.pi*Rsph**3 + gamma*interfacial(ar)*4*np.pi*Rsph**2
+    
+        tol = 1e-3
+        invphi = (np.sqrt(5) - 1) / 2
+        invphi2 = (3 - np.sqrt(5)) / 2
+        h = b - a
+        c, d = a+invphi2*h, a+invphi*h
+        fc, fd = f(c), f(d)
+
+        while abs(h) > tol:
+            if fc < fd:
+                b, d, fd = d, c, fc
+                h *= invphi
+                c = a + invphi2 * h
+                fc = f(c)  
+            else:
+                a, c, fc = c, d, fd
+                h *= invphi
+                d = a + invphi * h
+                fd = f(d)
 
-        #Composition gradient (we need to calculate gradient for reference element)
-        dxdz = (self.x[:,1:] - self.x[:,:-1]) / self.dz
-        dxdz = np.concatenate(([0-np.sum(dxdz, axis=0)], dxdz), axis=0)
+        return (c+d)/2
 
-        # J = -M * dmu/dz
-        # Ideal contribution: J_id = -eps * M*R*T / x * dx/dz
-        fluxes = np.zeros((len(self.elements)+1, self.N-1))
-        fluxes = -avgMob * dmudz
-        nonzeroComp = avgX != 0
-        fluxes[nonzeroComp] += -self.eps * avgMob[nonzeroComp] * 8.314 * self.T * dxdz[nonzeroComp] / avgX[nonzeroComp]
+    def updateCache(self, normR):
+        '''
+        Update cached calculations
+        '''
+        if self._aspectRatios is None:
+            self._aspectRatios = np.linspace(1 + 1/self._cachedIntervals, 1+self._cachedRange, int(self._cachedRange*self._cachedIntervals))
+            self._normEnergies = self.strainEnergy(normR(self._aspectRatios))
+        else:
+            addedAspectRatios = np.linspace(self._aspectRatios[-1] + 1/self._cachedIntervals, self._aspectRatios[-1] + self._cachedRange, int(self._cachedRange*self._cachedIntervals))
+            addedNormEnergies = self.strainEnergy(normR(addedAspectRatios))
+            self._aspectRatios = np.concatenate((self._aspectRatios, addedAspectRatios))
+            self._normEnergies = np.concatenate((self._normEnergies, addedNormEnergies))
 
-        #Flux in a volume fixed frame: J_vi = J_i - x_i * sum(J_j)
-        vfluxes = np.zeros((len(self.elements), self.N+1))
-        vfluxes[:,1:-1] = fluxes[1:,:] - avgX[1:,:] * np.sum(fluxes, axis=0)
+    def clearCache(self):
+        '''
+        Clear cached calculations
+        '''
+        self._aspectRatios = None
+        self._normEnergies = None
 
-        #Boundary conditions
-        for e in range(len(self.elements)):
-            vfluxes[e,0] = self.LBCvalue[e] if self.LBC[e] == self.FLUX else vfluxes[e,1]
-            vfluxes[e,-1] = self.RBCvalue[e] if self.RBC[e] == self.FLUX else vfluxes[e,-2]
+    def eqAR_bySearch(self, Rsph, gamma, shpFactor):
+        '''
+        Equilibrium aspect ratio by cached search
 
-        #Time increment
-        #This is done by finding the time interval such that the composition
-        # change caused by the fluxes will be lower than self.maxCompositionChange
-        dJ = np.abs(vfluxes[:,1:] - vfluxes[:,:-1]) / self.dz
-        dt = self.maxCompositionChange / np.amax(dJ[dJ!=0])
+        Parameters
+        ----------
+        Rsph : float or array
+            Equivalent spherical radius
+        gamma : float
+            Interfacial energy
+        shpFactor : ShapeFactor object
+        '''
+        normR = shpFactor._normalRadiiEquation
+        interfacial = shpFactor._thermoEquation if self.ifmethod == 1 else shpFactor._eqRadiusEquation
+        if hasattr(Rsph, '__len__'):
+            eqAR = np.ones(len(Rsph))
+            for i in range(len(Rsph)):
+                eqAR[i] = self._cachedSearch(Rsph[i], gamma, interfacial, normR)
+        else:
+            eqAR = self._cachedSearch(Rsph, gamma, interfacial, normR)
+        return eqAR
 
-        return vfluxes, dt
-        
-    def updateMesh(self, fluxes, dt):
+    def _cachedSearch(self, Rsph, gamma, interfacial, normR):
         '''
-        Updates the mesh based off the fluxes and time interval
+        Cached search for a single radius
         '''
-        for e in range(len(self.elements)):
-            self.x[e] += -(fluxes[e,1:] - fluxes[e,:-1]) * dt / self.dz
+        if self._aspectRatios is None:
+            self.updateCache(normR)
+        
+        Vsph = 4/3*np.pi*Rsph**3
+        Asph = 4*np.pi*Rsph**2
+        eInter = Asph*interfacial(self._aspectRatios)*gamma
+        eqAR = self._aspectRatios[np.argmin(self._normEnergies*Vsph+eInter)]
+
+        #If eqAR is on the upper end (3/4) of the cached aspect ratios, then
+        #added to the cached arrays until it's not
+        while eqAR > self._aspectRatios[int(-self._cachedIntervals/4)] and self._aspectRatios[-1] < 100:
+            self.updateCache(normR)
+            eInter = Asph*interfacial(self._aspectRatios)*gamma
+            eqAR = self._aspectRatios[np.argmin(self._normEnergies*Vsph+eInter)]
+
+        return eqAR
+
```

### Comparing `kawin-0.2.0/kawin/EffectiveDiffusion.py` & `kawin-0.3.0/kawin/precipitation/non_ideal/EffectiveDiffusion.py`

 * *Files identical despite different names*

### Comparing `kawin-0.2.0/kawin/FreeEnergyHessian.py` & `kawin-0.3.0/kawin/thermo/FreeEnergyHessian.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,62 +4,90 @@
 
 setattr(v, 'GE', v.StateVariable('GE'))
 
 def hessian(chemical_potentials, composition_set):
     '''
     Returns the hessian of the objective function for a single phase
 
+    For the Lagrangian function
+        L = N * G + sum(mu_A * (N_A - N * dM_A/dy_i)) + sum(lambda_s * (1 - sum(y_i)))
+    We have 5 derivatives
+    d2L/dyi2 = N * d2G/dyi2
+    d2L/dyidlambda_s = -1 if y_i in s else 0
+    d2L/dyidN = dG/dy - sum(mu_A * dM_A/dy_i)
+    d2L/dyidmu_A = -N dM_A/dy_i
+    d2L/dmu_AdN = -M_A
+
+    Everything is per mole of formula unit, so N has to be corrected for phases where the 
+    total moles of atoms could be off from 1
+
     Parameters
     ----------
     chemical_potentials : 1-D ndarray
     composition_set : pycalphad.core.composition_set.CompositionSet
     
     Returns
     -------
     Matrix of floats for each second derivative
     Derivatives along each axis will be in order of:
         site fractions, phase amount, lagrangian multipliers, chemical potential
     '''
     elements = list(composition_set.phase_record.nonvacant_elements)
-    x = np.array(composition_set.X)
     mu = np.asarray(chemical_potentials)
+
+    #dM_A / dy_i
     dxdy = np.zeros((len(elements), len(composition_set.dof)))
+    #M_A
+    moleA = np.zeros((len(elements),1))
     for comp_idx in range(len(elements)):
         composition_set.phase_record.formulamole_grad(dxdy[comp_idx, :], composition_set.dof, comp_idx)
+        composition_set.phase_record.formulamole_obj(moleA[comp_idx,:], composition_set.dof, comp_idx)
+
+    #Moles of phase per formula unit
+    #We assume 1 mole of phase, but this is per mole of atoms
+    #This is generally okay, but for interstitials or vacancies in the main sublattice
+    #We need to use moles of formula units when constructing the hessian
+    formulaPhAmt = 1 / np.sum(moleA)
+
+    #dG/dy_i and d2G/dy2
     dg = np.zeros(len(composition_set.dof))
     composition_set.phase_record.formulagrad(dg, composition_set.dof)
     d2g = np.zeros((len(composition_set.dof), len(composition_set.dof)))
     composition_set.phase_record.formulahess(d2g, composition_set.dof)
 
     phase_dof = composition_set.phase_record.phase_dof
     num_internal_cons = composition_set.phase_record.num_internal_cons
     num_statevars = composition_set.phase_record.num_statevars
     #Create hessian matrix
     hess = np.zeros((phase_dof + num_internal_cons + len(elements) + 1,
                      phase_dof + num_internal_cons + len(elements) + 1))
-    # wrt phase dof
+    # wrt phase dof - d2L / dyi dyj
     hess[:phase_dof, :phase_dof] = d2g[composition_set.phase_record.num_statevars:,
-                                       composition_set.phase_record.num_statevars:]
-    cons_jac_tmp = np.zeros((num_internal_cons, len(composition_set.dof)))
-    composition_set.phase_record.internal_cons_jac(cons_jac_tmp, composition_set.dof)
-
-    # wrt phase amount
+                                       composition_set.phase_record.num_statevars:] * formulaPhAmt
+    
+    # wrt phase amount - d2L / dyi dN
     for i in range(phase_dof):
         hess[i, phase_dof] = dg[num_statevars + i] - np.sum(mu * dxdy[:, num_statevars+i])
         hess[phase_dof, i] = hess[i, phase_dof]
 
+    # d2L / dyi dlambda
+    cons_jac_tmp = np.zeros((num_internal_cons, len(composition_set.dof)))
+    composition_set.phase_record.internal_cons_jac(cons_jac_tmp, composition_set.dof)
     hess[:phase_dof, phase_dof+1:phase_dof+1+num_internal_cons] = -cons_jac_tmp[:, num_statevars:].T
     hess[phase_dof+1:phase_dof+1+num_internal_cons, :phase_dof] = hess[:phase_dof, phase_dof+1:phase_dof+1+num_internal_cons].T
+
+    # d2L / dyi dmuA
     index = phase_dof + num_internal_cons + 1
-    hess[:phase_dof, index:] = -1 * dxdy[:, num_statevars:].T
-    hess[index:, :phase_dof] = -1 * dxdy[:, num_statevars:]
+    hess[:phase_dof, index:] = -1 * dxdy[:, num_statevars:].T * formulaPhAmt
+    hess[index:, :phase_dof] = -1 * dxdy[:, num_statevars:] * formulaPhAmt
 
+    # d2L / dmuA dN
     for A in range(len(elements)):
-        hess[phase_dof, index + A] = -x[A]
-        hess[index + A, phase_dof] = -x[A]
+        hess[phase_dof, index + A] = -moleA[A,0]
+        hess[index + A, phase_dof] = -moleA[A,0]
     return hess
 
 
 def totalddx(chemical_potentials, composition_set, refElement):
     '''
     Total derivative of site fractions, phase amount, lagrangian multipliers 
     and chemical potential with respect to system composition
@@ -135,14 +163,18 @@
     '''
     Total derivative of chemical potential with respect to system composition
     dmuA/dxB = (partial dmuA/dxB - partial dmuA/dxR) - (partial dmuR/dxB - partial dmuR/dxR) 
     where R is reference
 
     This more or less represents the curvature of the free energy surface with reference element R
 
+    Rows correspond to mu_A and columns correspond to X_A so for ternary system with (A,B,R), its
+    |   dmu_A/dX_A   dmu_A/dX_B   |
+    |   dmu_B/dX_A   dmu_B/dX_B   |
+
     Parameters
     ----------
     chemical_potentials : 1-D ndarray
     composition_set : pycalphad.core.composition_set.CompositionSet
     refElement : str
         Reference element
     
@@ -168,14 +200,18 @@
 
     return dmudx
 
 def partialdMudX(chemical_potentials, composition_set):
     '''
     Partial derivative of chemical potential with respect to system composition
 
+    Rows correspond to mu_A and columns correspond to X_A so for binary system, its
+    |   dmu_A/dX_A   dmu_A/dX_B   |
+    |   dmu_B/dX_A   dmu_B/dX_B   |
+
     Parameters
     ----------
     composition_set : pycalphad.core.composition_set.CompositionSet
     
     Returns
     -------
     Array of floats for each derivative, (n x n) matrix
```

### Comparing `kawin-0.2.0/kawin/GrainBoundaries.py` & `kawin-0.3.0/kawin/precipitation/non_ideal/GrainBoundaries.py`

 * *Files identical despite different names*

### Comparing `kawin-0.2.0/kawin/KWNBase.py` & `kawin-0.3.0/kawin/thermo/Surrogate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,1689 +1,1581 @@
 import numpy as np
-import matplotlib.pyplot as plt
-from kawin.EffectiveDiffusion import EffectiveDiffusionFunctions
-from kawin.ShapeFactors import ShapeFactor
-from kawin.ElasticFactors import StrainEnergy
-from kawin.GrainBoundaries import GBFactors
-import copy
-import time
-import csv
-from itertools import zip_longest
+import pickle
+from scipy.interpolate import Rbf
+import scipy.spatial.distance as spd
 
-class PrecipitateBase:
+def generateTrainingPoints(*arrays):
     '''
-    Base class for precipitation models
-    Note: currently only the Euler implementation is available, but
-        other implementations are planned to be added
-    
+    Creates all combinations of inputted arrays
+    Used for creating training points in composition space for
+    MulticomponentSurrogate
+
     Parameters
     ----------
-    t0 : float
-        Initial time in seconds
-    tf : float
-        Final time in seconds
-    steps : int
-        Number of time steps
-    phases : list (optional)
-        Precipitate phases (array of str)
-        If only one phase is considered, the default is ['beta']
-    linearTimeSpacing : bool (optional)
-        Whether to have time increment spaced linearly or logarithimically
-        Defaults to False
-    elements : list (optional)
-        Solute elements in system
-        Note: order of elements must correspond to order of elements set in Thermodynamics module
-        If binary system, then defualt is ['solute']
+    arrays - arrays along each dimension
+        Order of arrays should correspond to the order of elements when defining thermodynamic functions
     '''
-    def __init__(self, t0, tf, steps, phases = ['beta'], linearTimeSpacing = False, elements = ['solute']):
-        #Store input parameters
-        self.initialSteps = int(steps)      #Initial number of steps for when model is reset
-        self.steps = int(steps)             #This includes the number of steps added when adaptive time stepping is enabled
-        self.t0 = t0
-        self.tf = tf
-        self.phases = np.array(phases)
-        self.linearTimeSpacing = linearTimeSpacing
-
-        #Change t0 to finite value if logarithmic time spacing
-        #New t0 will be tf / 1e6
-        if self.t0 <= 0 and self.linearTimeSpacing == False:
-            self.t0 = self.tf / 1e6
-            print('Warning: Cannot use 0 as an initial time when using logarithmic time spacing')
-            print('\tSetting t0 to {:.3e}'.format(self.t0))
-        
-        #Time variables
-        self.adaptiveTimeStepping(True)
-
-        #Predefined constraints, these can be set if they make the simulation unstable
-        self._defaultConstraints()
-
-        #Stopping conditions
-        self.clearStoppingConditions()
-            
-        #Composition array
-        self.elements = elements
-        self.numberOfElements = len(elements)
-        
-        #All other arrays
-        self._resetArrays()
-        
-        #Constants
-        self.Rg = 8.314                 #J/mol-K
-        self.avo = 6.022e23             #/mol
-        self.kB = self.Rg / self.avo    #J/K
-        
-        #Default variables, these terms won't have to be set before simulation
-        self.strainEnergy = [StrainEnergy() for i in self.phases]
-        self.calculateAspectRatio = [False for i in self.phases]
-        self.RdrivingForceLimit = np.zeros(len(self.phases), dtype=np.float32)
-        self.shapeFactors = [ShapeFactor() for i in self.phases]
-        self.theta = 2 * np.ones(len(self.phases), dtype=np.float32)
-        self.effDiffFuncs = EffectiveDiffusionFunctions()
-        self.effDiffDistance = self.effDiffFuncs.effectiveDiffusionDistance
-        self.infinitePrecipitateDiffusion = [True for i in self.phases]
-        self.dTemp = 0
-        self.iterationSinceTempChange = 0
-        self.GBenergy = 0.3     #J/m2
-        self.parentPhases = [[] for i in self.phases]
-        self.GB = [GBFactors() for p in self.phases]
-        
-        #Set other variables to None to throw errors if not set
-        self.xInit = None
-        self.T = None
-        self.Tparameters = None
-
-        self._isNucleationSetup = False
-        self.GBareaN0 = None
-        self.GBedgeN0 = None
-        self.GBcornerN0 = None
-        self.dislocationN0 = None
-        self.bulkN0 = None
-        
-        #Unit cell parameters
-        self.aAlpha = None
-        self.VaAlpha = None
-        self.VmAlpha = None
-        self.atomsPerCellBeta = np.empty(len(self.phases), dtype=np.float32)
-        self.VaBeta = np.empty(len(self.phases), dtype=np.float32)
-        self.VmBeta = np.empty(len(self.phases), dtype=np.float32)
-        self.Rmin = np.empty(len(self.phases), dtype=np.float32)
-        
-        #Free energy parameters
-        self.gamma = np.empty(len(self.phases), dtype=np.float32)
-        self.dG = [None for i in self.phases]
-        self.interfacialComposition = [None for i in self.phases]
-
-        if self.numberOfElements == 1:
-            self._Beta = self._BetaBinary1
-        else:
-            self._Beta = self._BetaMulti
-            self._betaFuncs = [None for p in phases]
-            self._defaultBeta = 20
-        
-    def phaseIndex(self, phase = None):
-        '''
-        Returns index of phase in list
-
-        Parameters
-        ----------
-        phase : str (optional)
-            Precipitate phase (defaults to None, which will return 0)
-        '''
-        return 0 if phase is None else np.where(self.phases == phase)[0][0]
-        
-    def reset(self):
-        '''
-        Resets simulation results
-        This does not reset the model parameters, however, it will clear any stopping conditions
-        '''
-        self._resetArrays()
-        self.xComp[0] = self.xInit
-        self.dTemp = 0
-
-        #Reset temperature array
-        if np.isscalar(self.Tparameters):
-            self.setTemperature(self.Tparameters)
-        elif len(self.Tparameters) == 2:
-            self.setTemperatureArray(*self.Tparameters)
-        elif self.Tparameters is not None:
-            self.setNonIsothermalTemperature(self.Tparameters)
-        
-    def _resetArrays(self):
-        '''
-        Resets and initializes arrays for all variables
-            time
-            matrix composition, equilibrium composition
-            critial radius and nucleation barrier
-            average radius and aspect ratio
-            volume fraction
-            nucleation rate
-            precipitate density
-            driving force
-            beta
-            incubation time
-        '''
-        self.steps = self.initialSteps
-        self.time = np.linspace(self.t0, self.tf, self.steps) if self.linearTimeSpacing else np.logspace(np.log10(self.t0), np.log10(self.tf), self.steps)
-
-        if self.numberOfElements == 1:
-            self.xComp = np.zeros(self.steps)                                #Current composition of matrix phase
-            self.xEqAlpha = np.zeros((len(self.phases), self.steps))         #Equilibrium composition of matrix phase with respect to each precipitate phase
-            self.xEqBeta = np.zeros((len(self.phases), self.steps))          #Equilibrium composition of precipitate phases
-        else:
-            self.xComp = np.zeros((self.steps, self.numberOfElements))
-            self.xEqAlpha = np.zeros((len(self.phases), self.steps, self.numberOfElements))
-            self.xEqBeta = np.zeros((len(self.phases), self.steps, self.numberOfElements))
-            
-        self.Rcrit = np.zeros((len(self.phases), self.steps))                #Critical radius
-        self.Gcrit = np.zeros((len(self.phases), self.steps))                #Height of nucleation barrier
-        self.Rad = np.zeros((len(self.phases), self.steps))                  #Radius of particles formed at each time step
-        self.avgR = np.zeros((len(self.phases), self.steps))                 #Average radius
-        self.avgAR = np.zeros((len(self.phases), self.steps))                #Mean aspect ratio
-        self.betaFrac = np.zeros((len(self.phases), self.steps))             #Fraction of precipitate
-        
-        self.nucRate = np.zeros((len(self.phases), self.steps))              #Nucleation rate
-        self.precipitateDensity = np.zeros((len(self.phases), self.steps))   #Number of nucleates
-        
-        self.dGs = np.zeros((len(self.phases), self.steps))                  #Driving force
-        self.betas = np.zeros((len(self.phases), self.steps))                #Impingement rates (used for non-isothermal)
-        self.incubationOffset = np.zeros(len(self.phases))                   #Offset for incubation time (for non-isothermal precipitation)
-        self.incubationSum = np.zeros(len(self.phases))                      #Sum of incubation time
-
-        self.prevFConc = np.zeros((2, len(self.phases), self.numberOfElements))    #Sum of precipitate composition for mass balance
-
-    def save(self, filename, compressed = False, toCSV = False):
-        '''
-        Save results into a numpy .npz or .csv format
-
-        Parameters
-        ----------
-        filename : str
-        compressed : bool
-            If true, will save compressed .npz format
-        toCSV : bool
-            If true, will save to .csv
-        '''
-        variables = ['t0', 'tf', 'steps', 'phases', 'linearTimeSpacing', 'elements', \
-            'time', 'xComp', 'Rcrit', 'Gcrit', 'Rad', 'avgR', 'avgAR', 'betaFrac', 'nucRate', 'precipitateDensity', 'dGs', 'xEqAlpha', 'xEqBeta']
-        vDict = {v: getattr(self, v) for v in variables}
-        
-        if toCSV:
-            vDict['t0'] = np.array([vDict['t0']])
-            vDict['tf'] = np.array([vDict['tf']])
-            vDict['steps'] = np.array([vDict['steps']])
-            vDict['linearTimeSpacing'] = np.array([vDict['linearTimeSpacing']])
-            if self.numberOfElements == 2:
-                vDict['xComp'] = vDict['xComp'].T
-            arrays = []
-            headers = []
-            for v in vDict:
-                vDict[v] = np.array(vDict[v])
-                if len(vDict[v].shape) == 2:
-                    for i in range(len(vDict[v])):
-                        arrays.append(vDict[v][i])
-                        headers.append(v + str(i))
-                        if v == 'xComp':
-                            headers.append(v + '_' + self.elements[i])
-                        else:
-                            headers.append(v + '_' + self.phases[i])
-                elif v == 'xEqAlpha' or v == 'xEqBeta':
-                    for i in range(len(self.phases)):
-                        for j in range(self.numberOfElements):
-                            arrays.append(vDict[v][i,:,j])
-                            headers.append(v + '_' + self.phases[i] + '_' + self.elements[j])
-                else:
-                    arrays.append(vDict[v])
-                    headers.append(v)
-            rows = zip_longest(*arrays, fillvalue='')
-            if '.csv' not in filename.lower():
-                filename = filename + '.csv'
-            with open(filename, 'w', newline='') as f:
-                csv.writer(f).writerow(headers)
-                csv.writer(f).writerows(rows)
-        else:
-            if compressed:
-                np.savez_compressed(filename, **vDict)
-                #np.savez_compressed(filename, **vDict, allow_pickle=True)
-            else:
-                np.savez(filename, **vDict)
-                #np.savez(filename, **vDict, allow_pickle=True)
-
-    def load(filename):
-        '''
-        Loads data
+    return np.array(np.meshgrid(*arrays)).T.reshape(-1, len(arrays))
 
-        Parameters
-        ----------
-        filename : str
-
-        Returns
-        -------
-        PrecipitateBase object
-            Note: this will only contain model outputs which can be used for plotting
-        '''
-        setupVars = ['t0', 'tf', 'steps', 'phases', 'linearTimeSpacing', 'elements']
-        if '.np' in filename.lower():
-            data = np.load(filename, allow_pickle=True)
-            model = PrecipitateBase(data['t0'], data['tf'], data['steps'], data['phases'], data['linearTimeSpacing'], data['elements'])
-            for d in data:
-                if d not in setupVars:
-                    setattr(model, d, data[d])
-        elif '.csv' in filename.lower():
-            with open(filename, 'r') as csvFile:
-                data = csv.reader(csvFile, delimiter=',')
-                i = 0
-                headers = []
-                columns = {}
-                #Grab all columns
-                for row in data:
-                    if i == 0:
-                        headers = row
-                        columns = {h: [] for h in headers}
-                    else:
-                        for j in range(len(row)):
-                            if row[j] != '':
-                                columns[headers[j]].append(row[j])
-                    i += 1
+def _filter_points(inputs, outputs, tol = 1e-3):
+    '''
+    Filter set of input points such that the closest distance is above tolerance
+    This is to avoid non-positive definite training matrices when creating surrogate models
 
-                t0, tf, steps, phases, elements = float(columns['t0'][0]), float(columns['tf'][0]), int(columns['steps'][0]), columns['phases'], columns['elements']
-                linearTimeSpacing = True if columns['linearTimeSpacing'][0] == 'True' else False
-                model = PrecipitateBase(t0, tf, steps, phases, linearTimeSpacing, elements)
+    Parameters
+    ----------
+    inputs : m x n matrix of floats
+        Input points of m observations in n-dimensional space
+    outputs : list of array of floats
+        Output points, each array must be m x n where
+            m is number of observations and n is dimensions of output
+    tol : float
+        Tolerance for distance between two input points
+
+    Outputs
+    -------
+    (filtered inputs, filtered outputs)
+    filtered inputs - array of input points
+    filtered outputs - array of output points
+    '''
+    #Make distance matrix
+    distance = spd.squareform(spd.pdist(inputs))
 
-                restOfVariables = ['time', 'xComp', 'Rcrit', 'Gcrit', 'Rad', 'avgR', 'avgAR', 'betaFrac', 'nucRate', 'precipitateDensity', 'dGs', 'xEqAlpha', 'xEqBeta']
-                restOfColumns = {v: [] for v in restOfVariables}
-                for d in columns:
-                    if d not in setupVars:
-                        if d == 'time':
-                            restOfColumns[d] = np.array(columns[d], dtype='float')
-                        elif d == 'xComp':
-                            if model.numberOfElements == 1:
-                                restOfColumns[d] = np.array(columns[d], dtype='float')
-                            else:
-                                restOfColumns['xComp'].append(columns[d], dtype='float')
-                        else:
-                            selectedVar = ''
-                            for r in restOfVariables:
-                                if r in d:
-                                    selectedVar = r
-                            restOfColumns[selectedVar].append(np.array(columns[d], dtype='float'))
-                for d in restOfColumns:
-                    restOfColumns[d] = np.array(restOfColumns[d])
-                    setattr(model, d, restOfColumns[d])
+    #Indices to remove
+    indices = np.where((distance > 0) & (distance <= tol))
+    indices = np.unique(indices[0][indices[0] < indices[1]])
 
-                #For multicomponent systems, adjust as necessary such that number of elements will be the last axis
-                if model.numberOfElements > 1:
-                    model.xComp = model.xComp.T
-                    if len(model.phases) == 1:
-                        model.xEqAlpha = np.expand_dims(model.xEqAlpha, 0)
-                        model.xEqBeta = np.expand_dims(model.xEqBeta, 0)
-                    else:
-                        model.xEqAlpha = np.reshape(model.xEqAlpha, ((len(model.phases), model.numberOfElements, len(model.time))))
-                        model.xEqBeta = np.reshape(model.xEqBeta, ((len(model.phases), model.numberOfElements, len(model.time))))
-                    model.xEqAlpha = np.transpose(model.xEqAlpha, (0, 2, 1))
-                    model.xEqBeta = np.transpose(model.xEqBeta, (0, 2, 1))
-        return model
-        
-    def _divideTimestep(self, i, dt):
-        '''
-        Adds a new time step between t_i-1 and t_i, with new time being t_i-1 + dt
+    newInputs = np.delete(inputs, indices, axis=0)
+    newOutputs = []
+    for i in range(len(outputs)):
+        newOutputs.append(np.delete(outputs[i], indices, axis=0))
 
-        Parameters
-        ----------
-        i : int
-        dt : float
-            Note: this must be smaller than t_i - t_i-1
-        '''
-        self.steps += 1
-
-        if self.numberOfElements == 1:
-            self.xComp = np.append(self.xComp, 0)
-            self.xEqAlpha = np.append(self.xEqAlpha, np.zeros((len(self.phases), 1)), axis=1)
-            self.xEqBeta = np.append(self.xEqBeta, np.zeros((len(self.phases), 1)), axis=1)
-        else:
-            self.xComp = np.append(self.xComp, np.zeros((1, self.numberOfElements)), axis=0)
-            self.xEqAlpha = np.append(self.xEqAlpha, np.zeros((len(self.phases), 1, self.numberOfElements)), axis=1)
-            self.xEqBeta = np.append(self.xEqBeta, np.zeros((len(self.phases), 1, self.numberOfElements)), axis=1)
+    return newInputs, newOutputs
 
-        #Add new element to each variable
-        self.Rcrit = np.append(self.Rcrit, np.zeros((len(self.phases), 1)), axis=1)
-        self.Gcrit = np.append(self.Gcrit, np.zeros((len(self.phases), 1)), axis=1)
-        self.Rad = np.append(self.Rad, np.zeros((len(self.phases), 1)), axis=1)
-        self.avgR = np.append(self.avgR, np.zeros((len(self.phases), 1)), axis=1)
-        self.avgAR = np.append(self.avgAR, np.zeros((len(self.phases), 1)), axis=1)
-        self.betaFrac = np.append(self.betaFrac, np.zeros((len(self.phases), 1)), axis=1)
-        self.nucRate = np.append(self.nucRate, np.zeros((len(self.phases), 1)), axis=1)
-        self.precipitateDensity = np.append(self.precipitateDensity, np.zeros((len(self.phases), 1)), axis=1)
-        self.dGs = np.append(self.dGs, np.zeros((len(self.phases), 1)), axis=1)
-        self.betas = np.append(self.betas, np.zeros((len(self.phases), 1)), axis=1)
+class BinarySurrogate:
+    '''
+    Handles surrogate models for driving force, interfacial composition and
+    diffusivity in a binary system
+    
+    Parameters
+    ----------
+    binaryThermodynamics - BinaryThermodynamics (optional)
+        Driving force and interfacial composition will be taken from this if not explicitly defined
+        If None, then drivingForce and interfacialComposition must be defined
+        
+    drivingForce - function (optional)
+        Function will take in (composition, temperature) and return driving force,
+            where a positive value means that precipitation is favorable
+        
+    interfacialComposition - function (optional)
+        Function will take in (temperature, excess gibbs free energy) and
+            return tuple (parent composition, precipitate composition) or (None, None) if precipitate is unstable
 
-        prevDT = self.time[i] - self.time[i-1]
-        self.time = np.insert(self.time, i, self.time[i-1] + dt)
+    diffusivity - function (optional)
+        Function will take in (composition, temperature) and return diffusivity
 
-        ratio = dt / prevDT
-        self.T = np.insert(self.T, i, ratio * self.T[i-1] + (1-ratio) * self.T[i])
+    precPhase : str (optional)
+        Precipitate phase to consider if binaryThermodynamics is defined
 
-    def adaptiveTimeStepping(self, adaptive = True):
-        '''
-        Sets if adaptive time stepping is used
+    Note: if binaryThermodynamics is not defined, then drivingForce and
+        interfacial composition needs to be defined
+    '''
+    def __init__(self, binaryThermodynamics = None, drivingForce = None, interfacialComposition = None, diffusivity = None, precPhase = None):
+        self.binTherm = binaryThermodynamics
+        self.precPhase = precPhase
+        
+        #If no driving force or interfacial composition function is supplied, then use function from thermodynamics class
+        if drivingForce is None:
+            self.drivingForceFunction = lambda x, T, returnComp=False, training = True: self.binTherm.getDrivingForce(x, T, self.precPhase, returnComp, training)
+        else:
+            self.drivingForceFunction = drivingForce
+        
+        if interfacialComposition is None:
+            self.interfacialCompositionFunction = lambda T, ge: self.binTherm.getInterfacialComposition(T, ge, self.precPhase)
+        else:
+            self.interfacialCompositionFunction = interfacialComposition
+
+        if binaryThermodynamics is not None:
+            self.diffusivityFunction = self.binTherm.getInterdiffusivity
+        elif diffusivity is not None:
+            self.diffusivityFunction = diffusivity
+
+        self.eps = 1e-3
+
+        #Driving force variables -----------------------------------------
+        #Training data points
+        self.drivingForce = []
+        self.precComp = []
+        self.dGcoords = []
+        self.precCompIndices = []
+        self.precCompCoords = []
+
+        #Scaling factor to normalize distance
+        self.XDGscale = None
+        self.TDGscale = None
+
+        #Surrogates
+        self.DGfunction = 'linear'
+        self.DGepsilon = 1
+        self.DGsmooth = 0
+        self.linearDG = True
+        self.LogSurrDG = None
+        self.LogSurrPrecComp = None
+        self.SurrogateDrivingForce = None
+        self.SurrogatePrecComp = None
+
+        #Interfacial composition -----------------------------------------
+        #Training data
+        self.xParent = []
+        self.xPrec = []
+        self.ICcoords = []
+        self.uniqueXPrec = []
+        self.Gcoords = []
+        self.G = []
+        
+        #Scaling factor to normalize distance
+        self.TICscale = None
+        self.GICscale = None
+        self.XGscale = None
+        
+        #Surrogates
+        self.ICfunction = 'linear'
+        self.ICepsilon = 1
+        self.ICsmooth = 0
+        self.linearIC = True
+        self.SurrogateParent = None
+        self.SurrogatePrec = None
+        self.SurrogateG = None
+        self.LogSurrParent = None
+        self.LogSurrPrec = None
+
+        #Diffusivity -----------------------------------------------------
+        #Training data
+        self.Diffcoords = []
+        self.Diff = []
+
+        #Scaling factor
+        #Scale temperature and free energy range is proportional to amount of data along given axis
+        self.XDiffscale = None
+        self.singleXDiff = False
+        self.TDiffscale = None
+
+        #Surrogates
+        self.linearDiff = False
+        self.Difffunction = 'linear'
+        self.Diffepsilon = 1
+        self.Diffsmooth = 0
+        self.SurrogateDiff = None
+        self.LogSurrDiff = None
+        
+        
+    def trainDrivingForce(self, comps, temperature, function='linear', epsilon=1, smooth=0, scale='linear'):
+        '''
+        Creates training points and sets up surrogate models for driving force calculations
+        
+        Parameters
+        ----------
+        comps : array of floats
+            Range of compositions for training points
+        temperature : float or array
+            Temperature or range of temperatures for training points
+        function : str (optional)
+            Radial basis function to use (defaults to 'linear')
+            Other functions are 'multiquadric', 'inverse_multiquadric',
+                'gaussian', 'cubic', 'quintic' and 'thin_plate'
+        epsilon : float
+            Scale for radial basis function (defaults to 1)
+            Training data will be scaled automatically
+                such that optimal scale is around 1
+        smooth : float
+            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
+        scale : float
+            Whether the composition training data should be in log or linear scale
+            Note: 'log' is recommended for dilute solutions
+        '''
+        #Convert temperature to array if not so
+        if not hasattr(temperature, '__len__'):
+            temperature = [temperature]
+        
+        #Ensure that composition are defined values if in log scale
+        if scale == 'log':
+            comps[comps == 0] = 1e-9
+        
+        self.drivingForce = []
+        self.precComp = []
+        self.dGcoords = []
+        self.precCompIndices = []
+        
+        #Create training data
+        n = 0   #Index for precCompIndices (needs to correspond to indices self.drivingForce array)
+        for t in temperature:
+            for x in comps:
+                dG, xP = self.drivingForceFunction(x, t, returnComp = True)
+
+                #If driving force can be obtained (generally True)
+                if dG is not None:
+                    self.drivingForce.append(dG)
+                    self.dGcoords.append([x, t])
+                    
+                    #If driving force is positive, then store nucleate composition
+                    if xP is not None:
+                        self.precComp.append(xP)
+                        self.precCompIndices.append(n)
+                    
+                    n += 1
 
-        Parameters
-        ----------
-        adaptive : bool (optional)
-            Defaults to True
-        '''
-        if adaptive:
-            self._timeIncrementCheck = self._checkDT
-            #self._postTimeIncrementCheck = self._postCheckDT
-            self._postTimeIncrementCheck = self._noPostCheckDT
+        self.dGcoords = np.array(self.dGcoords)   
+        self.drivingForce = np.array(self.drivingForce)
+        self.precComp = np.array(self.precComp)
+        self.precCompIndices = np.array(self.precCompIndices)
+        
+        #Log scale
+        if scale == 'log':
+            self.dGcoords[:,0] = np.log10(self.dGcoords[:,0])
+        
+        #Scale data so that it the range is proportional to the amount of data points along the given axis
+        if len(comps) == 1:
+            self.XDGscale = 1
         else:
-            self._timeIncrementCheck = self._noCheckDT
-            self._postTimeIncrementCheck = self._noPostCheckDT
-
-    def _calculateDT(self, i, fraction):
-        '''
-        Calculates DT as a fraction of the total simulation time
-        '''
-        if self.linearTimeSpacing:
-            dt = fraction*(self.tf - self.t0)
+            self.XDGscale = (np.amax(self.dGcoords[:,0]) - np.amin(self.dGcoords[:,0])) / len(comps)
+            self.dGcoords[:,0] /= self.XDGscale
+            
+        if len(temperature) == 1:
+            self.TDGscale = 1
         else:
-            dt = self.time[i] * (np.exp(fraction*np.log(self.tf / self.t0)) - 1)
-        return dt
-
-    def _defaultConstraints(self):
-        '''
-        Default values for contraints
-        '''
-        self.minRadius = 3e-10
-        self.maxTempChange = 1
-
-        self.maxDTFraction = 1e-2
-        self.minDTFraction = 1e-5
-
-        self.checkTemperature = True
-        self.maxNonIsothermalDT = 1
-
-        self.checkPSD = True
-        self.maxDissolution = 0.01
-
-        self.checkRcrit = True
-        self.maxRcritChange = 0.01
+            self.TDGscale = (np.amax(self.dGcoords[:,1]) - np.amin(self.dGcoords[:,1])) / len(temperature)
+            self.dGcoords[:,1] /= self.TDGscale
 
-        self.checkNucleation = True
-        self.maxNucleationRateChange = 0.5
-        self.minNucleationRate = 1e-5
+        #Create new array of coordinates for precipitate composition (this is to allow for filtering)
+        self.precCompCoords = self.dGcoords[self.precCompIndices]
 
-        self.checkVolumePre = True
-        self.checkVolumePost = False
-        self.maxVolumeChange = 0.001
+        #Filter points such that all points are separated by a distance by at least self.eps
+        self.dGcoords, outputs = _filter_points(self.dGcoords, [self.drivingForce], self.eps)
+        self.drivingForce = outputs[0]
         
-        self.checkComposition = False
-        self.checkCompositionPre = False
-        self.maxCompositionChange = 0.001
-        self.minComposition = 0
+        self.precCompCoords, outputs = _filter_points(self.precCompCoords, [self.precComp], self.eps)
+        self.precComp = outputs[0]
 
-        self.minNucleateDensity = 1e-5
-
-    def setConstraints(self, **kwargs):
-        '''
-        Sets constraints
-
-        TODO: the following constraints are not implemented
-            maxDTFraction
-            maxRcritChange - this is somewhat implemented but disabled by default
-
-        Possible constraints:
-        ---------------------
-        minRadius - minimum radius to be considered a precipitate (1e-10 m)
-        maxTempChange - maximum temperature change before lookup table is updated (only for Euler in binary case) (1 K)
-
-        maxDTFraction - maximum time increment allowed as a fraction of total simulation time (0.1)
-        minDTFraction - minimum time increment allowed as a fraction of total simulation time (1e-5)
-
-        checkTemperature - checks max temperature change (True)
-        maxNonIsothermalDT - maximum time step when temperature is changing (1 second)
-
-        checkPSD - checks maximum growth rate for particle size distribution (True)
-        maxDissolution - maximum relative volume fraction of precipitates allowed to dissolve in a single time step (0.01)
-
-        checkRcrit - checks maximum change in critical radius (False)
-        maxRcritChange - maximum change in critical radius (as a fraction) per single time step (0.01)
-
-        checkNucleation - checks maximum change in nucleation rate (True)
-        maxNucleationRateChange - maximum change in nucleation rate (on log scale) per single time step (0.5)
-        minNucleationRate - minimum nucleation rate to be considered for checking time intervals (1e-5)
-
-        checkVolumePre - estimates maximum volume change (True)
-        checkVolumePost - checks maximum calculated volume change (True)
-        maxVolumeChange - maximum absolute value that volume fraction can change per single time step (0.001)
-
-        checkComposition - checks maximum change in composition (True)
-        chekcCompositionPre - estimates maximum change in composition (False)
-        maxCompositionChange - maximum change in composition in single time step (0.01)
+        if scale == 'log':
+            self.linearDG = False
+        else:
+            self.linearDG = True
+        self.DGfunction = function
+        self.DGepsilon = epsilon
+        self.DGsmooth = np.amax([smooth, self.eps])
+        
+        self._createDGSurrogate()
 
-        minNucleateDensity - minimum nucleate density to consider nucleation to have occurred (1e-5)
+    def _createDGSurrogate(self):
         '''
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-        
-    def setBetaBinary(self, functionType = 1):
+        Build surrogates for driving force
         '''
-        Sets function for beta calculation in binary systems
+        if self.linearDG:
+            self.SurrogateDrivingForce = Rbf(self.dGcoords[:,0], self.dGcoords[:,1], self.drivingForce, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
+            self.SurrogatePrecComp = Rbf(self.precCompCoords[:,0], self.precCompCoords[:,1], self.precComp, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
+        else:
+            self.linearDG = False
+            self.LogSurrDG = Rbf(self.dGcoords[:,0], self.dGcoords[:,1], self.drivingForce, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
+            self.LogSurrPrecComp = Rbf(self.precCompCoords[:,0], self.precCompCoords[:,1], self.precComp, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
+            self.SurrogateDrivingForce = lambda x, T: self.LogSurrDG(np.log10(x) / self.XDGscale, T)
+            self.SurrogatePrecComp = lambda x, T: self.LogSurrPrecComp(np.log10(x) / self.XDGscale, T)
 
-        If using a multicomponent system, this function will not do anything
+    def changeDrivingForceHyperparameters(self, function = 'linear', epsilon = 1, smooth = 0):
+        '''
+        Re-create surrogate model for driving force with updated hyperparameters
 
         Parameters
         ----------
-        functionType : int
-            ID for function
-                1 for implementation seen in Perez et al, 2008 (default)
-                2 for implementation similar to multicomponent systems
+        function : str (optional)
+            Radial basis function to use (defaults to 'linear')
+            Other functions are 'multiquadric', 'inverse_multiquadric',
+                'gaussian', 'cubic', 'quintic' and 'thin_plate'
+        epsilon : float
+            Scale for radial basis function (defaults to 1)
+            Training data will be scaled automatically
+                such that optimal scale is around 1
+        smooth : float
+            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
         '''
-        if self.numberOfElements == 1:
-            if functionType == 2:
-                self.beta = self._BetaBinary2
-            else:
-                self.beta = self._BetaBinary1
+        if self.TDGscale is None:
+            raise Exception("Driving force has not been trained.")
 
-    def setInitialComposition(self, xInit):
-        '''
-        Parameters
+        self.DGfunction = function
+        self.DGepsilon = epsilon
+        self.DGsmooth = np.amax([smooth, self.eps])
         
-        xInit : float or array
-            Initial composition of parent matrix phase in atomic fraction
-            Use float for binary system and array of solutes for multicomponent systems
-        '''
-        self.xInit = xInit
-        self.xComp[0] = xInit
+        self._createDGSurrogate()            
         
-    def setInterfacialEnergy(self, gamma, phase = None):
+    def getDrivingForce(self, x, T, returnComp = False):
         '''
+        Gets driving force from surrogate models
+        
         Parameters
         ----------
-        gamma : float
-            Interfacial energy between precipitate and matrix in J/m2
-        phase : str (optional)
-            Phase to input interfacial energy (defaults to first precipitate in list)
-        '''
-        index = self.phaseIndex(phase)
-        self.gamma[index] = gamma
+        x : float or array of floats
+            Composition
+        T : float or array of floats
+            Temperature, must be same length as x
+        returnComp : bool (optional)
+            Returns precipitate composition if True (defaults to False)
         
-    def resetAspectRatio(self, phase = None):
-        '''
-        Resets aspect ratio variables of defined phase to default
+        Returns
+        -------
+        (driving force, precipitate composition)
+        Both will be same shape as x and T
+        Positive driving force means that precipitate will form
+        precipitate composition will be None if returnComp is False
+        '''
+        if self.TDGscale is None:
+            raise Exception("Driving force has not been trained.")
+
+        #Convert arrays to Numpy arrays for math operations
+        if hasattr(x, '__len__'):
+            x = np.array(x)
+        if hasattr(T, '__len__'):
+            T = np.array(T)
 
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
-        '''
-        index = self.phaseIndex(phase)
-        self.shapeFactors[index].setSpherical()
+        if self.linearDG:
+            dG = self.SurrogateDrivingForce(x / self.XDGscale, T / self.TDGscale)
+            
+            if returnComp:
+                xP = self.SurrogatePrecComp(x / self.XDGscale, T / self.TDGscale)
+                return dG, xP
+            else:
+                if hasattr(dG, '__len__'):
+                    return dG, np.full(dG.shape, None)
+                else:
+                    return dG, None
+                
+        else:
+            dG = self.SurrogateDrivingForce(x, T / self.TDGscale)
+            
+            if returnComp:
+                xP = self.SurrogatePrecComp(x, T / self.TDGscale)
 
-    def setSpherical(self, phase = None):
+                return dG, xP
+            else:
+                if hasattr(dG, '__len__'):
+                    return dG, np.full(dG.shape, None)
+                else:
+                    return dG, None
+        
+    def trainInterfacialComposition(self, temperature, freeEnergy, function='linear', epsilon=1, smooth=0, scale = 'linear'):
         '''
-        Sets precipitate shape to spherical for defined phase
+        Creates training points and sets up surrogate models for interfacial composition
 
         Parameters
         ----------
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
-        '''
-        index = self.phaseIndex(phase)
-        self.shapeFactors[index].setSpherical()
+        temperature : float or array
+            Temperature or range of temperatures for training points
+        freeEnergy : array of floats
+            range of free energy values from Gibbs-Thomson contribution
+        function : str (optional)
+            Radial basis function to use (defaults to 'linear')
+            Other functions are 'multiquadric', 'inverse_multiquadric',
+                'gaussian', 'cubic', 'quintic' and 'thin_plate'
+        epsilon : float
+            Scale for radial basis function (defaults to 1)
+            Training data will be scaled automatically
+                such that optimal scale is around 1
+        smooth : float
+            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
+        scale : float
+            Whether the matrix composition output should be in log or linear scale
+            Note: 'log' is recommended for dilute solutions
+        '''
+        #Make temperature an array if not so
+        if not hasattr(temperature, '__len__'):
+            temperature = [temperature]
+        
+        self.xParent = []
+        self.xPrec = []
+        self.ICcoords = []
+        
+        #Create training data
+        for t in temperature:
+            for g in freeEnergy:
+                xM, xP = self.interfacialCompositionFunction(t, g)
+                
+                #If precipitate can be form at T,G, then add to training array
+                if xM is not None and xM > 0:
+                    self.xParent.append(xM)
+                    self.xPrec.append(xP)
+                    
+                    self.ICcoords.append([t, g])
+                    
+        self._buildInterfacialCompositionModels(temperature, freeEnergy, function, epsilon, smooth, scale)
         
-    def setAspectRatioNeedle(self, ratio=1, phase = None):
+    def trainInterfacialCompositionFromDrivingForceData(self, function='linear', epsilon=1, smooth=0, scale='linear'):
         '''
-        Consider specified precipitate phase as needle-shaped
-        with specified aspect ratio
+        Converts driving force data ([x, T] -> G) to interfacial composition data ([T, G] -> x)
+        This may lead to inaccuracies in the precipitate composition since driving force calculations are done by sampling the free energy curve
 
         Parameters
         ----------
-        ratio : float or function
-            Aspect ratio of needle-shaped precipitate
-            If float, must be greater than 1
-            If function, must take in radius as input and output float greater than 1
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
+        function : str (optional)
+            Radial basis function to use (defaults to 'linear')
+            Other functions are 'multiquadric', 'inverse_multiquadric',
+                'gaussian', 'cubic', 'quintic' and 'thin_plate'
+        epsilon : float
+            Scale for radial basis function (defaults to 1)
+            Training data will be scaled automatically
+                such that optimal scale is around 1
+        smooth : float
+            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
+        scale : float
+            Whether the matrix composition output should be in log or linear scale
+            Note: 'log' is recommended for dilute solutions
         '''
-        index = self.phaseIndex(phase)
-        self.shapeFactors[index].setNeedleShape(ratio)
+        self.xPrec = [x for x in self.precComp]
         
-    def setAspectRatioPlate(self, ratio=1, phase = None):
+        #Take driving force training data and convert to interfacial composition training data
+        if self.linearDG:
+            self.xParent = [self.dGcoords[i, 0] * self.XDGscale for i in self.precCompIndices]
+        else:
+            self.xParent = [10**self.dGcoords[i, 0] * self.XDGscale for i in self.precCompIndices]
+            
+        self.ICcoords = []
+        for i in self.precCompIndices:
+            self.ICcoords.append([self.dGcoords[i, 1] * self.TDGscale, self.drivingForce[i]])
+        
+        self._buildInterfacialCompositionModels(np.unique(self.dGcoords[:, 1]) * self.TDGscale, self.drivingForce, function, epsilon, smooth, scale)
+                    
+    def _buildInterfacialCompositionModels(self, temperature, freeEnergy, function, epsilon, smooth, scale):
         '''
-        Consider specified precipitate phase as plate-shaped
-        with specified aspect ratio
+        Builds interfacial composition model (this is separate to allow for both training from new data or driving force data)
 
         Parameters
         ----------
-        ratio : float or function
-            Aspect ratio of needle-shaped precipitate
-            If float, must be greater than 1
-            If function, must take in radius as input and output float greater than 1
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
-        '''
-        index = self.phaseIndex(phase)
-        self.shapeFactors[index].setPlateShape(ratio)
+        temperature - range of temperatures
+        freeEnergy - range of free energies
+        function - radial basis function
+        epsilon - scale factor
+        smooth - smoothing factor
+        scale - linear or log scale
+        '''
+        #Create new training points finding the driving force for precipitation at the precipitate composition
+        self.uniqueXPrec = np.unique(self.xPrec)
+        if np.amax(self.uniqueXPrec) - np.amin(self.uniqueXPrec) < 1e-4:
+            self.uniqueXPrec = np.array([self.uniqueXPrec[0]])
+        self.Gcoords = []
+        self.G = []
+        
+        for t in temperature:
+            for x in self.uniqueXPrec:
+                #Driving force calcs can be interpreted as the maximum free energy that can be contributed by the Gibbs-Thomson effect
+                dG, _ = self.drivingForceFunction(x, t, returnComp = False)
+
+                #if driving force can be obtained (generally True)
+                if dG is not None:
+                    self.G.append(dG)
+                    self.Gcoords.append([x, t])
+                    
+                    #Add these points to the composition surrogate training data as an endpoint (these are for the minimum particle radius)
+                    self.ICcoords.append([t, dG])
+                    self.xParent.append(x)
+                    self.xPrec.append(x)
+        
+        self.G = np.array(self.G)
+        self.Gcoords = np.array(self.Gcoords)
+        
+        self.xParent = np.array(self.xParent)
+        self.xPrec = np.array(self.xPrec)
+        self.ICcoords = np.array(self.ICcoords)
+        
+        #Invert free energy coordinates - this will make the spacing more consistent
+        self.ICcoords[:,1] =  1 / self.ICcoords[:,1]
+        
+        #Scale temperature and free energy range is proportional to amount of data along given axis
+        if len(temperature) == 1:
+            self.TICscale = 1
+        else:
+            self.TICscale = (np.amax(self.ICcoords[:,0]) - np.amin(self.ICcoords[:,0])) / len(temperature)
+            self.ICcoords[:,0] /= self.TICscale
+            
+        if len(freeEnergy) == 1:
+            self.GICscale = 1
+        else:
+            self.GICscale = (np.amax(self.ICcoords[:,1]) - np.amin(self.ICcoords[:,1])) / len(freeEnergy)
+            self.ICcoords[:,1] /= self.GICscale
+            
+        if len(self.uniqueXPrec) == 1:
+            self.XGscale = 1
+        else:
+            self.XGscale = (np.amax(self.Gcoords[:,0]) - np.amin(self.Gcoords[:,0])) / len(self.uniqueXPrec)
+            self.Gcoords[:,0] /= self.XGscale
+            
+        self.Gcoords[:,1] /= self.TICscale
+
+        #Filter points such that all points are separated by a distance by at least self.eps
+        self.ICcoords, outputs = _filter_points(self.ICcoords, [self.xParent, self.xPrec], self.eps)
+        self.xParent = outputs[0]
+        self.xPrec = outputs[1]
         
-    def setAspectRatioCuboidal(self, ratio=1, phase = None):
-        '''
-        Consider specified precipitate phase as cuboidal-shaped
-        with specified aspect ratio
+        self.Gcoords, outputs = _filter_points(self.Gcoords, [self.G], self.eps)
+        self.G = outputs[0]
 
-        TODO: add cuboidal factor
-            Currently, I think this considers that the cuboidal factor is 1
+        if scale == 'log':
+            self.linearIC = False
+        else:
+            self.linearIC = True
+        self.ICfunction = function
+        self.ICepsilon = epsilon
+        self.ICsmooth = np.amax([smooth, self.eps])
 
-        Parameters
-        ----------
-        ratio : float or function
-            Aspect ratio of needle-shaped precipitate
-            If float, must be greater than 1
-            If function, must take in radius as input and output float greater than 1
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
-        '''
-        index = self.phaseIndex(phase)
-        self.shapeFactors[index].setCuboidalShape(ratio)
-    
-    def setVmAlpha(self, Vm, atomsPerCell):
-        '''
-        Molar volume for parent phase
-        
-        Parameters
-        ----------
-        Vm : float
-            Molar volume (m3 / mol)
-        atomsPerCell : int
-            Number of atoms in a unit cell
-        '''
-        self.VmAlpha = Vm
-        self.VaAlpha = atomsPerCell * self.VmAlpha / self.avo
-        self.aAlpha = np.cbrt(self.VaAlpha)
-        self.atomsPerCellAlpha = atomsPerCell
-        
-    def setVaAlpha(self, Va, atomsPerCell):
+        self._createICSurrogate()
+
+    def _createICSurrogate(self):
         '''
-        Unit cell volume for parent phase
-        
-        Parameters
-        ----------
-        Va : float
-            Unit cell volume (m3 / unit cell)
-        atomsPerCell : int
-            Number of atoms in a unit cell
+        Build surrogates for interfacial composition
         '''
-        self.VaAlpha = Va
-        self.VmAlpha = self.VaAlpha * self.avo / atomsPerCell
-        self.aAlpha = np.cbrt(Va)
-        self.atomsPerCellAlpha = atomsPerCell
-        
-    def setUnitCellAlpha(self, a, atomsPerCell):
+        if self.linearIC:
+            self.SurrogateParent = Rbf(self.ICcoords[:,0], self.ICcoords[:,1], self.xParent, function = self.ICfunction, epsilon = self.ICepsilon, smooth=self.ICsmooth)
+            self.SurrogatePrec = Rbf(self.ICcoords[:,0], self.ICcoords[:,1], self.xPrec, function = self.ICfunction, epsilon = self.ICepsilon, smooth=self.ICsmooth)  
+        else:
+            self.LogSurrParent = Rbf(self.ICcoords[:,0], self.ICcoords[:,1], np.log10(self.xParent), function = self.ICfunction, epsilon = self.ICepsilon, smooth=self.ICsmooth)
+            self.LogSurrPrec = Rbf(self.ICcoords[:,0], self.ICcoords[:,1], np.log10(self.xPrec), function = self.ICfunction, epsilon = self.ICepsilon, smooth=self.ICsmooth) 
+            
+            self.SurrogateParent = lambda T, gExtraInverse: 10**(self.LogSurrParent(T, gExtraInverse))
+            self.SurrogatePrec = lambda T, gExtraInverse: 10**(self.LogSurrPrec(T, gExtraInverse))
+           
+        if len(self.G) == 1:
+            self.SurrogateG = lambda x, T: self.G[0]
+        else:
+            self.SurrogateG = Rbf(self.Gcoords[:,0], self.Gcoords[:,1], self.G, function = 'linear', epsilon = 1)
+
+    def changeInterfacialCompositionHyperparameters(self, function = 'linear', epsilon = 1, smooth = 0):
         '''
-        Lattice parameter for parent phase (assuming cubic unit cell)
-        
+        Re-create surrogate model for interfacial composition with updated hyperparameters
+
         Parameters
         ----------
-        a : float
-            Lattice constant (m)
-        atomsPerCell : int
-            Number of atoms in a unit cell
+        function : str (optional)
+            Radial basis function to use (defaults to 'linear')
+            Other functions are 'multiquadric', 'inverse_multiquadric',
+                'gaussian', 'cubic', 'quintic' and 'thin_plate'
+        epsilon : float
+            Scale for radial basis function (defaults to 1)
+            Training data will be scaled automatically
+                such that optimal scale is around 1
+        smooth : float
+            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
         '''
-        self.aAlpha = a
-        self.VaAlpha = a**3
-        self.VmAlpha = self.VaAlpha * self.avo / atomsPerCell
-        self.atomsPerCellAlpha = atomsPerCell
-        
-    def setVmBeta(self, Vm, atomsPerCell, phase = None):
+        if self.TICscale is None:
+            raise Exception("Interfacial composition has not been trained.")
+
+        self.ICfunction = function
+        self.ICepsilon = epsilon
+        self.ICsmooth = np.amax([smooth, self.eps])
+
+        self._createICSurrogate()
+            
+    def getInterfacialComposition(self, T, gExtra = 0):
         '''
-        Molar volume for precipitate phase
+        Gets Interfacial composition from surrogate models
         
         Parameters
         ----------
-        Vm : float
-            Molar volume (m3 / mol)
-        atomsPerCell : int
-            Number of atoms in a unit cell
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
-        '''
-        index = self.phaseIndex(phase)
-        self.VmBeta[index] = Vm
-        self.VaBeta[index] = atomsPerCell * self.VmBeta[index] / self.avo
-        self.atomsPerCellBeta[index] = atomsPerCell
+        T : float or array of floats
+            Temperature
+        gExtra : float or array of floats
+            Free energy from Gibbs-Thomson contribution (must be same length as T)
         
-    def setVaBeta(self, Va, atomsPerCell, phase = None):
+        Returns
+        -------
+        (composition of parent phase, composition of precipitate phase)
+        Composition will be in same shape as T and gExtra
+        Will return (None, None) if gExtra is large enough that 
+            precipitate becomes unstable
+        '''
+        if self.TICscale is None:
+            raise Exception("Interfacial composition has not been trained.")
+
+        #Convert arrays to Numpy arrays for math operations
+        #Also raise gExtra to lowest training value to avoid erroneous values
+        #   NOTE: Do not use this as a way to minimize the amount of training points!!
+        #   While this is a safegaurd to avoid weird results, this creates a constant growth rate
+        #   for any values of gExtra less than the lowest training point, which can lead to non-realistic
+        #   values in the precipitate simulation (i.e. precipitates growing in an unsaturated matrix).
+        #   Just train more points at lower gExtra values (larger radius sizes)
+        if hasattr(gExtra, '__len__'):
+            gExtra = np.array(gExtra)
+            gExtra[1 / (gExtra * self.GICscale) > np.amax(self.ICcoords[:,1])] = 1 / (np.amax(self.ICcoords[:,1]) * self.GICscale)
+        else:
+            if gExtra == 0 or (1 / (gExtra * self.GICscale)) > np.amax(self.ICcoords[:,1]):
+                gExtra = 1 / (np.amax(self.ICcoords[:,1]) * self.GICscale)
+        if hasattr(T, '__len__'):
+            T = np.array(T)
+
+        #If gExtra is array and T isn't, then convert T to array
+        #This is to keep consistent with Thermodynamics counterpart
+        if hasattr(gExtra, '__len__') and not hasattr(T, '__len__'):
+            T = T * np.ones(len(gExtra))
+
+        xM, xP = self.SurrogateParent(T / self.TICscale, 1 / (gExtra * self.GICscale)), self.SurrogatePrec(T / self.TICscale, 1 / (gExtra * self.GICscale))
+        
+        dG = self.SurrogateG(xP / self.XGscale, T / self.TICscale)
+        if hasattr(xM, '__len__'):
+            noneVals = (dG < gExtra)
+            xM[noneVals] = -1
+            xP[noneVals] = -1
+        else:
+            if dG < gExtra:
+                xM = -1
+                xP = -1
+                    
+        return xM, xP
+
+    def trainInterdiffusivity(self, comps, temperature, function='linear', epsilon=1, smooth=0, scale='linear'):
         '''
-        Unit cell volume for precipitate phase
-        
+        Trains interdiffusivity from mobility parameters
+
         Parameters
         ----------
-        Va : float
-            Unit cell volume (m3 / unit cell)
-        atomsPerCell : int
-            Number of atoms in a unit cell
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
+        comps : array of floats
+            Range of compositions for training points
+        temperature : float or array
+            Temperature or range of temperatures for training points
+        function : str (optional)
+            Radial basis function to use (defaults to 'linear')
+            Other functions are 'multiquadric', 'inverse_multiquadric',
+                'gaussian', 'cubic', 'quintic' and 'thin_plate'
+        epsilon : float
+            Scale for radial basis function (defaults to 1)
+            Training data will be scaled automatically
+                such that optimal scale is around 1
+        smooth : float
+            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
+        scale : float
+            Whether the diffusivity output should be in log or linear scale
         '''
-        index = self.phaseIndex(phase)
-        self.VaBeta[index] = Va
-        self.VmBeta[index] = self.VaBeta[index] * self.avo / atomsPerCell
-        self.atomsPerCellBeta[index] = atomsPerCell
-        
-    def setUnitCellBeta(self, a, atomsPerCell, phase = None):
+        #Convert composition and temperature to array if not so
+        if not hasattr(comps, '__len__'):
+            comps = [comps]
+
+        if not hasattr(temperature, '__len__'):
+            temperature = [temperature]
+
+        self.Diffcoords = []
+        self.Diff = []
+
+        for x in comps:
+            for t in temperature:
+                self.Diff.append(self.diffusivityFunction(x, t))
+                self.Diffcoords.append([x, t])
+
+        self.Diffcoords = np.array(self.Diffcoords)
+        self.Diff = np.array(self.Diff)
+
+        #Scale temperature and free energy range is proportional to amount of data along given axis
+        if len(comps) == 1:
+            self.XDiffscale = 1
+            self.singleXDiff = True
+        else:
+            self.XDiffscale = (np.amax(self.Diffcoords[:,0]) - np.amin(self.Diffcoords[:,0])) / len(comps)
+            self.Diffcoords[:,0] /= self.XDiffscale
+            self.singleXDiff = False
+
+        if len(temperature) == 1:
+            self.TDiffscale = 1
+        else:
+            self.TDiffscale = (np.amax(self.Diffcoords[:,1]) - np.amin(self.Diffcoords[:,1])) / len(temperature)
+            self.Diffcoords[:,1] /= self.TDiffscale
+
+        #Filter diffusivity points
+        self.Diffcoords, outputs = _filter_points(self.Diffcoords, [self.Diff], self.eps)
+        self.Diff = outputs[0]
+
+        if scale == 'log':
+            self.linearDiff = False
+        else:
+            self.linearDiff = True
+        self.Difffunction = function
+        self.Diffepsilon = epsilon
+        self.Diffsmooth = np.amax([smooth, self.eps])
+
+        self._createDiffSurrogate()
+
+    def _createDiffSurrogate(self):
         '''
-        Lattice parameter for precipitate phase (assuming cubic unit cell)
-        
-        Parameters
-        ----------
-        a : float
-            Latice parameter (m)
-        atomsPerCell : int
-            Number of atoms in a unit cell
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
+        Builds surrogate for diffusivity
         '''
-        index = self.phaseIndex(phase)
-        self.VaBeta[index] = a**3
-        self.VmBeta[index] = self.VaBeta[index] * self.avo / atomsPerCell
-        self.atomsPerCellBeta[index] = atomsPerCell
+        #If only 1 data point, then create constant function
+        if len(self.Diff) == 1:
+            self.SurrogateDiff = lambda x, T: self.Diff[0]
+            return
 
-    def setNucleationDensity(self, grainSize = 100, aspectRatio = 1, dislocationDensity = 5e12, bulkN0 = None):
+        #Build surrogates
+        if self.linearDiff:
+            if self.singleXDiff:
+                self.SurrogateDiff = Rbf(self.Diffcoords[:,1], self.Diff, function = self.Difffunction, epsilon = self.Diffepsilon, smooth = self.Diffsmooth)
+            else:
+                self.SurrogateDiff = Rbf(self.Diffcoords[:,0], self.Diffcoords[:,1], self.Diff, function = self.Difffunction, epsilon = self.Diffepsilon, smooth = self.Diffsmooth) 
+        else:
+            if self.singleXDiff:
+                self.LogSurrDiff = Rbf(self.Diffcoords[:,1], np.log10(self.Diff), function = self.Difffunction, epsilon = self.Diffepsilon, smooth = self.Diffsmooth)
+                self.SurrogateDiff = lambda T: 10**(self.LogSurrDiff(T))
+            else:
+                self.LogSurrDiff = Rbf(self.Diffcoords[:,0], self.Diffcoords[:,1], np.log10(self.Diff), function = self.Difffunction, epsilon = self.Diffepsilon, smooth = self.Diffsmooth) 
+                self.SurrogateDiff = lambda x, T: 10**(self.LogSurrDiff(x, T))
+
+    def changeDiffusivityHyperparameters(self, function = 'linear', epsilon = 1, smooth = 0):
         '''
-        Sets grain size and dislocation density which determines the available nucleation sites
-        
+        Re-create surrogate model for diffusivity with updated hyperparameters
+
         Parameters
         ----------
-        grainSize : float (optional)
-            Average grain size in microns (default at 100um if this function is not called)
-        aspectRatio : float (optional)
-            Aspect ratio of grains (default at 1)
-        dislocationDensity : float (optional)
-            Dislocation density (m/m3) (default at 5e12)
-        bulkN0 : float (optional)
-            This allows for the use to override the nucleation site density for bulk precipitation
-            By default (None), this is calculated by the number of lattice sites containing a solute atom
-            However, for calibration purposes, it may be better to set the nucleation site density manually
+        function : str (optional)
+            Radial basis function to use (defaults to 'linear')
+            Other functions are 'multiquadric', 'inverse_multiquadric',
+                'gaussian', 'cubic', 'quintic' and 'thin_plate'
+        epsilon : float
+            Scale for radial basis function (defaults to 1)
+            Training data will be scaled automatically
+                such that optimal scale is around 1
+        smooth : float
+            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
         '''
-        self.grainSize = grainSize * 1e-6
-        self.grainAspectRatio = aspectRatio
-        self.dislocationDensity = dislocationDensity
+        if self.XDiffscale is None:
+            raise Exception("Diffusivity has not been trained.")
 
-        self.bulkN0 = bulkN0
-        self._isNucleationSetup = True
+        self.Difffunction = function
+        self.Diffepsilon = epsilon
+        self.Diffsmooth = np.amax([smooth, self.eps])
 
-    def _getNucleationDensity(self):
-        '''
-        Calculates nucleation density
-        This is separated from setting nucleation density to
-            allow it to be called right before the simulation starts
-        '''
-        #Set bulk nucleation site to the number of solutes per unit volume
-        #NOTE: some texts will state the bulk nucleation sites to just be the number
-        #       of lattice sites per unit volume. The justification for this would be 
-        #       the solutes can diffuse around to any lattice site and nucleate there
-        if self.bulkN0 is None:
-            if self.numberOfElements == 1:
-                self.bulkN0 = self.xComp[0] * (self.avo / self.VmAlpha)
-            else:
-                self.bulkN0 = np.amin(self.xComp[0,:]) * (self.avo / self.VmAlpha)
+        self._createDiffSurrogate()
 
-        self.dislocationN0 = self.dislocationDensity * (self.avo / self.VmAlpha)**(1/3)
-        
-        if self.grainSize != np.inf:
-            if self.GBareaN0 is None:
-                self.GBareaN0 = (6 * np.sqrt(1 + 2 * self.grainAspectRatio**2) + 1 + 2 * self.grainAspectRatio) / (4 * self.grainAspectRatio * self.grainSize)
-                self.GBareaN0 *= (self.avo / self.VmAlpha)**(2/3)
-            if self.GBedgeN0 is None:
-                self.GBedgeN0 = 2 * (np.sqrt(2) + 2 * np.sqrt(1 + self.grainAspectRatio**2)) / (self.grainAspectRatio * self.grainSize**2)
-                self.GBedgeN0 *= (self.avo / self.VmAlpha)**(1/3)
-            if self.GBcornerN0 is None:
-                self.GBcornerN0 = 12 / (self.grainAspectRatio * self.grainSize**3)
-        else:
-            self.GBareaN0 = 0
-            self.GBedgeN0 = 0
-            self.GBcornerN0 = 0
-        
-    def setNucleationSite(self, site, phase = None):
+    def getInterdiffusivity(self, x, T):
         '''
-        Sets nucleation site type for specified phase
-        If site type is grain boundaries, edges or corners, the phase morphology will be set to spherical and precipitate shape will depend on wetting angle
-        
+        Returns interdiffusivity
+
         Parameters
         ----------
-        site : str
-            Type of nucleation site
-            Options are 'bulk', 'dislocations', 'grain_boundaries', 'grain_edges' and 'grain_corners'
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
+        x : float or array of floats
+            Composition
+        T : float or array of floats
+            Temperature (must be same length as x)
+        
+        Returns
+        -------
+        diffusivity (same shape as x and T)
         '''
-        index = self.phaseIndex(phase)
+        #Convert arrays to numpy arrays for math operations
+        if hasattr(x, '__len__'):
+            x = np.array(x)
+        if hasattr(T, '__len__'):
+            T = np.array(T)
 
-        self.GB[index].setNucleationType(site)
+        if self.XDiffscale is None:
+            raise Exception("Diffusivity has not been trained.")
+
+        if self.singleXDiff:
+            return self.SurrogateDiff(T / self.TDiffscale)
+        else:
+            return self.SurrogateDiff(x / self.XDiffscale, T / self.TDiffscale)
         
-        if self.GB[index].nucleationSiteType != GBFactors.BULK and self.GB[index].nucleationSiteType != GBFactors.DISLOCATION:
-            self.shapeFactors[index].setSpherical()
-            
-    def _setGBfactors(self):
+    def drivingForceTrainingTemperature(self):
         '''
-        Calcualtes factors for bulk or grain boundary nucleation
-        This is separated from setting the nucleation sites to allow
-        it to be called right before simulation
+        Returns the temperature coordinates of driving force training points
         '''
-        for p in range(len(self.phases)):
-            self.GB[p].setFactors(self.GBenergy, self.gamma[p])
-                    
-    def _GBareaRemoval(self, p):
+        return self.dGcoords[:,1] * self.TDGscale
+        
+    def drivingForceTrainingComposition(self):
         '''
-        Returns factor to multiply radius by to give the equivalent radius of circles representing the area of grain boundary removal
-
-        Parameters
-        ----------
-        p : int
-            Index for phase
+        Returns the composition coordinates of driving force training points
         '''
-        if self.GB[p].nucleationSiteType == GBFactors.BULK or self.GB[p].nucleationSiteType == GBFactors.DISLOCATION:
-            return 1
+        if self.linearDG:
+            return self.dGcoords[:,0] * self.XDGscale
         else:
-            return np.sqrt(self.GB[p].gbRemoval / np.pi)
+            return 10**(self.dGcoords[:,0] * self.XDGscale)
             
-    def setParentPhases(self, phase, parentPhases):
+    def interfacialCompositionTrainingTemperature(self):
+        '''
+        Returns the temperature coordinates of interfacial composition training points
         '''
-        Sets parent precipitates at which a precipitate can nucleate on the surface of
+        return self.ICcoords[:,0] * self.TICscale
         
-        Parameters
-        ----------
-        phase : str
-            Precipitate phase of interest that will nucleate
-        parentPhases : list
-            Phases that the precipitate of interest can nucleate on the surface of
+    def interfacialCompositionTrainingGibbsThomson(self):
         '''
-        index = self.phaseIndex(phase)
-        for p in parentPhases:
-            self.parentPhases[index].append(self.phaseIndex(p))
-           
-    def setGrainBoundaryEnergy(self, energy):
+        Returns the Gibbs-Thomson contribution coordinates of interfacial composition training points
         '''
-        Grain boundary energy - this will decrease the critical radius as some grain boundaries will be removed upon nucleation
-
-        Parameters
-        ----------
-        energy : float
-            GB energy in J/m2
+        return 1 / (self.ICcoords[:,1] * self.GICscale)
 
-        Default upon initialization is 0.3
-        Note: GBenergy of 0 is equivalent to bulk precipitation
-        '''
-        self.GBenergy = energy
-        
-    def setTheta(self, theta, phase = None):
+    def save(self, fileName):
         '''
-        This is a scaling factor for the incubation time calculation, default is 2
-
-        Incubation time is defined as 1 / \theta * \beta * Z^2
-        \theta differs by derivation. By default, this is set to 2 following the
-        Feder derivation. In the Wakeshima derivation, \theta is 4pi
+        Pickles surrogate data
+        Note: this will remove the user-defined driving force and interfacial compositions
+            This is not a problem; however, a loaded surrogate will not be
+            able to be re-trained with different training points
 
         Parameters
         ----------
-        theta : float
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
-        '''
-        index = self.phaseIndex(phase)
-        self.theta[index] = theta
-        
-    def setTemperature(self, temperature):
+        fileName : str
         '''
-        Sets isothermal temperature
-        
-        Parameters
-        ----------
-        temperature : float
-            Temperature in Kelvin
-        ''' 
-        #Store parameter in case model is reset
-        self.Tparameters = temperature
+        self.binTherm = None
+        self.drivingForceFunction = None
+        self.interfacialCompositionFunction = None
+        self.diffusivityFunction = None
 
-        self.T = np.full(self.steps, temperature, dtype=np.float32)
-        self._incubation = self._incubationIsothermal
-        
-    def setNonIsothermalTemperature(self, temperatureFunction):
+        self.LogSurrDG = None
+        self.LogSurrPrecComp = None
+        self.SurrogateDrivingForce = None
+        self.SurrogatePrecComp = None
+
+        self.SurrogateParent = None
+        self.SurrogatePrec = None
+        self.SurrogateG = None
+        self.LogSurrParent = None
+        self.LogSurrPrec = None
+
+        self.SurrogateDiff = None
+        self.LogSurrDiff = None
+
+        with open(fileName, 'wb') as file:
+            pickle.dump(self, file)
+
+        #Re-create surrogates so that it could still be used after saving
+        if self.XDGscale is not None:
+            self._createDGSurrogate()
+        if self.TICscale is not None:
+            self._createICSurrogate()
+        if self.XDiffscale is not None:
+            self._createDiffSurrogate()
+
+    def load(fileName):
         '''
-        Sets temperature as a function of time
-        
+        Loads data from a pickled surrogate and builds driving force and interfacial composition functions
+
         Parameters
         ----------
-        temperatureFunction : function 
-            Takes in time and returns temperature in K
+        fileName : str
+
+        Returns
+        -------
+        BinarySurrogate object
         '''
-        #Store parameter in case model is reset
-        self.Tparameters = temperatureFunction
+        surr = None
+        with open(fileName, 'rb') as file:
+            surr = pickle.load(file)
+
+        #Re-create surrogates so that it could still be used after saving
+        if surr.XDGscale is not None:
+            surr._createDGSurrogate()
+        if surr.TICscale is not None:
+            surr._createICSurrogate()
+        if surr.XDiffscale is not None:
+            surr._createDiffSurrogate()
 
-        self.T = np.array([temperatureFunction(t) for t in self.time])
+        return surr
         
-        if len(np.unique(self.T)) == 1:
-            self._incubation = self._incubationIsothermal
+class MulticomponentSurrogate:
+    '''
+    Handles surrogate models for driving force, interfacial composition
+        and growth rate in a multicomponent system
+    
+    Parameters
+    ----------
+    thermodynamics - MulticomponentThermodynamics (optional)
+        Driving force, interfacial composition and 
+            curvature functions will be taken from this
+        If None, then drivingForce and curvature will need to be defined
+        
+    drivingForce - function (optional))
+        Function will take in (composition, temperature) and return driving force
+            where a positive value means that precipitation is favorable
+            composition is an array for each element, excluding the reference element
+        
+    interfacialComposition - function (optional)
+        Takes in (composition, temperature, gExtra) and returns matrix and precipitate composition
+            composition is an array for each element, excluding the reference element
+        Function should return (None, None) if precipitate is unstable
+
+    curvature - function (optional)
+        Function will take in (composition, temperature) and return the following:
+            {D-1 dCbar / dCbar^T M-1 dCbar} - for calculating interfacial composition of matrix
+            {1 / dCbar^T M-1 dCbar} - for calculating growth rate
+            {Gb^-1 Ga} - for calculating precipitate composition
+            Ca - interfacial composition of matrix phase
+            Cb - interfacial composition of precipitate phase
+        Function will return (None, None, None, None, None) if composition is outside two phase region
+    
+    precPhase : str (optional)
+        Precipitate phase to consider if binaryThermodynamics is defined
+
+    Note: if binaryThermodynamics is not defined, then drivingForce and
+        interfacial composition needs to be defined
+    '''
+    def __init__(self, thermodynamics = None, drivingForce = None, interfacialComposition = None, curvature = None, precPhase = None):
+        self.therm = thermodynamics
+        self.precPhase = precPhase
+        self.elements = self.therm.elements[1:-1]
+        
+        #Grab driving force and curvature function from thermodynamics class if not supplied
+        if drivingForce is None:
+            #self.drivingForceFunction = self.therm.getDrivingForce
+            self.drivingForceFunction = lambda x, T, returnComp=False, training = True: self.therm.getDrivingForce(x, T, self.precPhase, returnComp, training)
+            #self.drivingForceFunction = lambda x, T, returnComp=False: self.therm.drivingForceFromCurvature(x, T, self.precPhase, returnComp)
+        else:
+            self.drivingForceFunction = drivingForce
+
+        if interfacialComposition is None:
+            self.interfacialCompositionFunction = lambda x, T, gExtra: self.therm.getInterfacialComposition(x, T, gExtra, self.precPhase)
+        else:
+            self.interfacialCompositionFunction = interfacialComposition
+
+        #TODO: curvatureFactor should take in searchDir from drivingForceFunction
+        #    but this needs to be compatible with the same parameters
+        if curvature is None:
+            #self.curvature = self.therm.curvatureFactor
+            #self.curvature = lambda x, T, training = True: self.therm.curvatureFactor(x, T, self.precPhase, training)
+            self.curvature = lambda x, T, training = True: self.therm._curvatureWithSearch(x, T, self.precPhase, training)
+        else:
+            self.curvature = curvature
+
+        self.eps = 1e-3
+
+        #Driving force ---------------------------------------------------
+        #Training data
+        self.drivingForce = []
+        self.precComp = []
+        self.dGcoords = []
+        self.precCompIndices = []
+        self.precCompCoords = []
+
+        #Scaling factor
+        self.XDGscale = []
+        self.TDGscale = None
+        
+        #Surrogates
+        self.linearDG = True
+        self.DGfunction = 'linear'
+        self.DGepsilon = 1
+        self.DGsmooth = 0
+        self.SurrogateDrivingForce = None
+        self.SurrPrecComp = None
+        self.SurrogatePrecComp = None
+        self.LogSurrDG = None
+        self.LogSurrPrecComp = None
+
+        #Interfacial composition -----------------------------------------
+        #Training data
+        self.Dc = []
+        self.Mc = []
+        self.Gba = []
+        self.beta = []
+        self.Ca = []
+        self.Cb = []
+        self.ICcoords = []
+
+        #Scaling factors
+        self.XICscale = None
+        self.TICscale = None
+
+        #Interfacial composition surrogates
+        self.linearIC = True
+        self.ICfunction = 'linear'
+        self.ICepsilon = 1
+        self.ICsmooth = 0
+
+        self.SurrDc = None
+        self.SurrCa = None
+        self.SurrCb = None
+        self.SurrGba = None
+
+        self.LogSurrDc = None
+        self.LogSurrMc = None
+        self.LogSurrBeta = None
+        self.LogSurrCa = None
+        self.LogSurrCb = None
+        self.LogSurrGba = None
+        
+        self.SurrogateDc = None
+        self.SurrogateMc = None
+        self.SurrogateBeta = None
+        self.SurrogateCa = None
+        self.SurrogateCb = None
+        self.SurrogateGba = None
+
+        
+    def trainDrivingForce(self, comps, temperature, function='linear', epsilon=1, smooth=0, scale='linear'):
+        '''
+        Creates training points and sets up surrogate models for driving force calculations
+        
+        Parameters
+        ----------
+        comps : 2-D array
+            Range of compositions for training points
+            0th axis represents an individual training point
+            1st axis represents element composition
+        temperature : float or array
+            Range of temperatures for training points
+        function : str (optional)
+            Radial basis function to use (defaults to 'linear')
+            Other functions are 'multiquadric', 'inverse_multiquadric',
+                'gaussian', 'cubic', 'quintic' and 'thin_plate'
+        epsilon : float
+            Scale for radial basis function (defaults to 1)
+            Training data will be scaled automatically
+                such that optimal scale is around 1
+        smooth : float
+            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
+        scale : float
+            Whether the composition training data should be in log or linear scale
+            Note: 'log' is recommended for dilute solutions
+        '''
+        #Make temperature an array if not so
+        if not hasattr(temperature, '__len__'):
+            temperature = [temperature]
+
+        #Ensure that composition are defined values when using log scale
+        if scale == 'log':
+            for x in comps:
+                x[x == 0] = 1e-9
+        
+        #Create training data
+        self.drivingForce = []
+        self.precComp = []
+        self.dGcoords = []
+        self.precCompIndices = []
+        
+        n = 0   #Index for precCompIndices (needs to correspond to indices self.drivingForce array)
+        for t in temperature:
+            for x in comps:
+                dG, xP = self.drivingForceFunction(x, t, returnComp = True)
+                
+                #If driving force can be obtained (generally True)
+                if dG is not None:
+                    self.drivingForce.append(dG)
+                    self.dGcoords.append(np.concatenate((x, [t])))
+                    
+                    #If driving force is positive, then add nucleate composition
+                    #Also determine equilibrium matrix composition, then add training point where driving force is 0
+                    
+                    if xP is not None:
+                        self.precComp.append(xP)
+                        self.precCompIndices.append(n)
+                        
+                        xMeq, xPeq = self.interfacialCompositionFunction(x, t, 0)
+                        if xMeq is not None:
+                            self.drivingForce.append(0)
+                            self.dGcoords.append(np.concatenate((xMeq[1:], [t])))
+                            n += 1
+                            self.precComp.append(xPeq[1:])
+                            self.precCompIndices.append(n)
+                        
+                    n += 1
+                
+        self.drivingForce = np.array(self.drivingForce)
+        self.precComp = np.array(self.precComp)
+        self.dGcoords = np.array(self.dGcoords)
+        self.precCompIndices = np.array(self.precCompIndices)
+        
+        #Log scale on only composition (good for dilute solutions)
+        if scale == 'log':
+            self.dGcoords[:,:-1] = np.log10(self.dGcoords[:,:-1])
+        
+        #Scale data so range is proportional to amount of data along given axis
+        if len(comps) == 1:
+            self.XDGscale = np.ones(len(self.elements))
         else:
-            self._incubation = self._incubationNonIsothermal
-        
-    def setTemperatureArray(self, times, temperatures):
-        '''
-        Sets temperature as a function of time interpolating between the inputted times and temperatures
-        
-        Parameters
-        ----------
-        times : list
-            Time in hours for when the corresponding temperature is reached
-        temperatures : list
-            Temperatures in K to be reached at corresponding times
-        '''
-        #Store parameter in case model is reset
-        self.Tparameters = (times, temperatures)
+            self.XDGscale = (np.amax(self.dGcoords[:,:-1]) - np.amin(self.dGcoords[:,:-1])) / len(comps)
+            self.dGcoords[:,:-1] /= self.XDGscale
+            
+        if len(temperature) == 1:
+            self.TDGscale = 1
+        else:
+            self.TDGscale = (np.amax(self.dGcoords[:,-1]) - np.amin(self.dGcoords[:,-1])) / len(temperature)
+            self.dGcoords[:,-1] /= self.TDGscale
 
-        self.T = np.full(self.steps, temperatures[0])
-        for i in range(1, len(times)):
-            self.T[(self.time < 3600*times[i]) & (self.time >= 3600*times[i-1])] = (temperatures[i] - temperatures[i-1]) / (3600 * (times[i] - times[i-1])) * (self.time[(self.time < 3600*times[i]) & (self.time >= 3600*times[i-1])] - 3600 * times[i-1]) + temperatures[i-1]
-        self.T[self.time >= 3600*times[-1]] = temperatures[-1]
+        #Create new array of coordinates for precipitate composition (this is to allow for filtering)
+        self.precCompCoords = self.dGcoords[self.precCompIndices]
+
+        #Filter points such that all points are separated by a distance by at least self.eps
+        self.dGcoords, outputs = _filter_points(self.dGcoords, [self.drivingForce], self.eps)
+        self.drivingForce = outputs[0]
         
-        if len(np.unique(self.T)) == 1:
-            self._incubation = self._incubationIsothermal
+        self.precCompCoords, outputs = _filter_points(self.precCompCoords, [self.precComp], self.eps)
+        self.precComp = outputs[0]
+
+        if scale == 'log':
+            self.linearDG = False
         else:
-            self._incubation = self._incubationNonIsothermal
+            self.linearDG = True
+        self.DGfunction = function
+        self.DGepsilon = epsilon
+        self.DGsmooth = np.amax([smooth, self.eps])
 
-    def setStrainEnergy(self, strainEnergy, phase = None, calculateAspectRatio = False):
-        '''
-        Sets strain energy class to precipitate
-        '''
-        index = self.phaseIndex(phase)
-        self.strainEnergy[index] = strainEnergy
-        self.calculateAspectRatio[index] = calculateAspectRatio
+        self._createDGSurrogate()
 
-    def _setupStrainEnergyFactors(self):
-        #For each phase, the strain energy calculation will be set to assume
-        # a spherical, cubic or ellipsoidal shape depending on the defined shape factors
-        for i in range(len(self.phases)):
-            self.strainEnergy[i].setup()
-            if self.strainEnergy[i].type != StrainEnergy.CONSTANT:
-                if self.shapeFactors[i].particleType == ShapeFactor.SPHERE:
-                    self.strainEnergy[i].setSpherical()
-                elif self.shapeFactors[i].particleType == ShapeFactor.CUBIC:
-                    self.strainEnergy[i].setCuboidal()
-                else:
-                    self.strainEnergy[i].setEllipsoidal()
-            
-    def setDiffusivity(self, diffusivity):
+    def _createDGSurrogate(self):
         '''
-        Parameters
-        ----------
-        diffusivity : function taking 
-            Composition and temperature (K) and returning diffusivity (m2/s)
-            Function must have inputs in this order: f(x, T)
-                For multicomponent systems, x is an array
+        Builds surrogate for driving force
         '''
-        self.Diffusivity = diffusivity
+        if self.linearDG:
+            arguments = [self.dGcoords[:,i] for i in range(len(self.dGcoords[0]))]
+            self.SurrogateDrivingForce = Rbf(*arguments, self.drivingForce, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
+            
+            arguments = [self.precCompCoords[:,i] for i in range(len(self.dGcoords[0]))]
+            self.SurrPrecComp = [Rbf(*arguments, self.precComp[:,i], function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth) for i in range(len(self.elements))]
+            self.SurrogatePrecComp = lambda x, T: np.array([self.SurrPrecComp[i](*x, T) for i in range(len(self.elements))])
+        else:
+            arguments = [self.dGcoords[:,i] for i in range(len(self.dGcoords[0]))]
+            self.LogSurrDG = Rbf(*arguments, self.drivingForce, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
+            self.LogSurrPrecComp = [Rbf(*arguments, self.precComp[:,i], function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth) for i in range(len(self.elements))]
+            self.SurrogateDrivingForce = lambda x, T: self.LogSurrDG(*(np.log10(x) / self.XDGscale), T)
+            self.SurrogatePrecComp = lambda x, T: np.array([self.LogSurrPrecComp[i](*(np.log10(x) / self.XDGscale), T) for i in range(len(self.elements))])
 
-    def setInfinitePrecipitateDiffusivity(self, infinite, phase = None):
+    def changeDrivingForceHyperparameters(self, function = 'linear', epsilon = 1, smooth = 0):
         '''
-        Sets whether to assuming infinitely fast or no diffusion in phase
+        Re-create surrogate model for driving force with updated hyperparameters
 
         Parameters
         ----------
-        infinite : bool
-            True will assume infinitely fast diffusion
-            False will assume no diffusion
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
-            Use 'all' to apply to all phases
+        function : str (optional)
+            Radial basis function to use (defaults to 'linear')
+            Other functions are 'multiquadric', 'inverse_multiquadric',
+                'gaussian', 'cubic', 'quintic' and 'thin_plate'
+        epsilon : float
+            Scale for radial basis function (defaults to 1)
+            Training data will be scaled automatically
+                such that optimal scale is around 1
+        smooth : float
+            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
         '''
-        if phase == 'all':
-            self.infinitePrecipitateDiffusion = [infinite for i in range(len(self.phases))]
-        else:
-            index = self.phaseIndex(phase)
-            self.infinitePrecipitateDiffusion[index] = infinite
+        if self.TDGscale is None:
+            raise Exception("Driving force has not been trained.")
+
+        self.DGfunction = function
+        self.DGepsilon = epsilon
+        self.DGsmooth = np.amax([smooth, self.eps])
         
-    def setDrivingForce(self, drivingForce, phase = None):
-        '''
-        Parameters
-        ----------
-        drivingForce : function
-            Taking in composition (at. fraction) and temperature (K) and return driving force (J/mol)
-                f(x, T) = dg, where x is float for binary and array for multicomponent
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
-        '''
-        index = self.phaseIndex(phase)
-        self.dG[index] = drivingForce
+        self._createDGSurrogate()
         
-    def setInterfacialComposition(self, composition, phase = None):
+    def getDrivingForce(self, x, T, returnComp = False):
         '''
+        Gets driving force from surrogate models
+        
         Parameters
         ----------
-        composition : function
-            Takes in temperature (K) and excess free energy (J/mol) and 
-            returns a tuple of (matrix composition, precipitate composition)
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
-
-        The excess free energy term will be taken as the interfacial curvature and elastic energy contributions.
-        This will be a positive value, so the function should ensure that the excess free energy to reduce the driving force
+        x : array or 2D array
+            Composition (array of float for each minor element)
+            2D arrays will have 0th axis for each set and 1st axis for composition
+        T : float or array
+            Temperature (must be float or same length as 0th axis of x if array)
         
-        If equilibrium cannot be solved, then the function should return (None, None) or (-1, -1)
+        Returns
+        -------
+        driving force (positive value means that precipitate is stable)
         '''
-        index = self.phaseIndex(phase)
-        self.interfacialComposition[index] = composition
+        if self.TDGscale is None:
+            raise Exception("Driving force has not been trained.")
 
-    def setThermodynamics(self, therm, phase = None, removeCache = False, addDiffusivity = True):
-        '''
-        Parameters
-        ----------
-        therm : Thermodynamics class
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
-        removeCache : bool (optional)
-            Will not cache equilibrium results if True (defaults to False)
-        addDiffusivity : bool (optional)
-            For binary systems, will add diffusivity functions from the database if present
-            Defaults to True
-        '''
-        index = self.phaseIndex(phase)
-        self.dG[index] = lambda x, T, removeCache = removeCache: therm.getDrivingForce(x, T, precPhase=phase, training = removeCache)
-        
-        if self.numberOfElements == 1:
-            self.interfacialComposition[index] = lambda x, T: therm.getInterfacialComposition(x, T, precPhase=phase)
-            if (therm.mobCallables is not None or therm.diffCallables is not None) and addDiffusivity:
-                self.Diffusivity = lambda x, T, removeCache = removeCache: therm.getInterdiffusivity(x, T, removeCache = removeCache)
+        if hasattr(T, '__len__'):
+            T = np.array(T)
+        x = np.array(x)
+        if x.ndim == 2:
+            x = x.T
+
+        if self.linearDG:
+            dG = self.SurrogateDrivingForce(*(x / self.XDGscale), T / self.TDGscale)
+            
+            if returnComp:
+                return dG, self.SurrogatePrecComp(x / self.XDGscale, T / self.TDGscale).T
+            else:
+                if hasattr(dG, '__len__'):
+                    return dG, np.full(dG.shape, None)
+                else:
+                    return dG, None
+            
         else:
-            self.interfacialComposition[index] = lambda x, T, dG, R, gExtra, removeCache = removeCache: therm.getGrowthAndInterfacialComposition(x, T, dG, R, gExtra, precPhase=phase, training = False)
-            self._betaFuncs[index] = lambda x, T, removeCache = removeCache: therm.impingementFactor(x, T, precPhase=phase, training = False)
+            dG = self.SurrogateDrivingForce(x, T / self.TDGscale)
+            
+            if returnComp:
+                return dG, self.SurrogatePrecComp(x, T / self.TDGscale)
+            else:
+                if hasattr(dG, '__len__'):
+                    return dG, np.full(dG.shape, None)
+                else:
+                    return dG, None
 
-    def setSurrogate(self, surr, phase = None):
-        '''
-        Parameters
-        ----------
-        surr : Surrogate class
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
+    def trainCurvature(self, comps, temperature, function='linear', epsilon=1, smooth=0, scale='linear'):
         '''
-        index = self.phaseIndex(phase)
-        self.dG[index] = surr.getDrivingForce
-        
-        if self.numberOfElements == 1:
-            self.interfacialComposition[index] = surr.getInterfacialComposition
+        Trains for curvature factor (from Phillipes and Voorhees - 2013) as a function of composition and temperature
+
+        Creates 5 surrogates
+        {D-1 dCbar / dCbar^T M-1 dCbar} - for calculating interfacial composition of matrix
+        {1 / dCbar^T M-1 dCbar} - for calculating growth rate
+        {Gb^-1 Ga} - for calculating precipitate composition
+        Ca - interfacial composition of matrix phase
+        Cb - interfacial composition of precipitate phase
+
+
+        Parameters
+        ----------
+        comps : 2D array of floats
+            Range of compositions for training points
+            0th axis represents a training point
+            1st axis represents element compositions
+        temperature : float or array
+            Range of temperatures for training points
+        function : str (optional)
+            Radial basis function to use (defaults to 'linear')
+            Other functions are 'multiquadric', 'inverse_multiquadric',
+                'gaussian', 'cubic', 'quintic' and 'thin_plate'
+        epsilon : float
+            Scale for radial basis function (defaults to 1)
+            Training data will be scaled automatically
+                such that optimal scale is around 1
+        smooth : float
+            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
+        scale : float
+            Whether the matrix composition output should be in log or linear scale
+            Note: 'log' is recommended for dilute solutions
+        '''
+        #Make temperature an array if not so
+        if not hasattr(temperature, '__len__'):
+            temperature = [temperature]
+
+        #Ensure that composition are defined values when using log scale
+        if scale == 'log':
+            for x in comps:
+                x[x == 0] = 1e-9
+        
+        #Create training data
+        self.Dc = []
+        self.Mc = []
+        self.Gba = []
+        self.beta = []
+        self.Ca = []
+        self.Cb = []
+        self.ICcoords = []
+        
+        for t in temperature:
+            for x in comps:
+                results = self.curvature(x, t)
+                #dc, mc, gba, beta, ca, cb = self.curvature(x, t)
+
+                if results is not None:
+                    dc, mc, gba, beta, ca, cb = results
+                    #Since Dc, Mc and Gba is constant for a given tie-line, add 3 training data points (at bulk compostion and phase boundaries)
+                    #This should give more accurate values at very small or very large supersaturations without having to calculate a lot of training data
+                    compCoords = [x, ca, cb]
+                    for i in range(3):
+                        self.Dc.append(dc)
+                        self.Mc.append(mc)
+                        self.Gba.append(gba)
+                        self.beta.append(beta)
+                        self.Ca.append(ca)
+                        self.Cb.append(cb)
+                        self.ICcoords.append(np.concatenate((compCoords[i], [t])))
+
+        self.Dc = np.array(self.Dc)
+        self.Mc = np.array(self.Mc)
+        self.Gba = np.array(self.Gba)
+        self.beta = np.array(self.beta)
+        self.Ca = np.array(self.Ca)
+        self.Cb = np.array(self.Cb)
+        self.ICcoords = np.array(self.ICcoords)
+        
+        #Log scale only on compositions (good for low solubility)
+        if scale == 'log':
+            self.ICcoords[:,:-1] = np.log10(self.ICcoords[:,:-1])
+        
+        #Scale data so range is proportional to amount of data along given axis
+        if len(comps) == 1:
+            self.XICscale = np.ones(len(self.elements))
         else:
-            self.interfacialComposition[index] = surr.getGrowthAndInterfacialComposition
-            self._betaFuncs[index] = surr.impingementFactor
+            self.XICscale = (np.amax(self.ICcoords[:,:-1]) - np.amin(self.ICcoords[:,:-1])) / len(comps)
+            self.ICcoords[:,:-1] /= self.XICscale
+            
+        if len(temperature) == 1:
+            self.TICscale = 1
+        else:
+            self.TICscale = (np.amax(self.ICcoords[:,-1]) - np.amin(self.ICcoords[:,-1])) / len(temperature)
+            self.ICcoords[:,-1] /= self.TICscale
 
-    def particleGibbs(self, radius, phase = None):
+        #Filter points such that all points are separated by a distance by at least self.eps
+        self.ICcoords, outputs = _filter_points(self.ICcoords, [self.Dc, self.Mc, self.Gba, self.beta, self.Ca, self.Cb], self.eps)
+        self.Dc = outputs[0]
+        self.Mc = outputs[1]
+        self.Gba = outputs[2]
+        self.beta = outputs[3]
+        self.Ca = outputs[4]
+        self.Cb = outputs[5]
+
+        if scale == 'log':
+            self.linearIC = False
+        else:
+            self.linearIC = True
+        self.ICfunction = function
+        self.ICepsilon = epsilon
+        self.ICsmooth = np.amax([smooth, self.eps])
+
+        self._createICSurrogate()
+
+    def _createICSurrogate(self):
+        '''
+        Builds surrogate for interfacial composition and curvature
+        '''
+        if self.linearIC:
+            arguments = [self.ICcoords[:,i] for i in range(len(self.ICcoords[0]))]
+            self.SurrogateMc = Rbf(*arguments, self.Mc, function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth)
+            self.SurrogateBeta = Rbf(*arguments, self.beta, function=self.ICfunction, epislon=self.ICepsilon, smooth=self.ICsmooth)
+
+            self.SurrDc = [Rbf(*arguments, self.Dc[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
+            self.SurrCa = [Rbf(*arguments, self.Ca[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
+            self.SurrCb = [Rbf(*arguments, self.Cb[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
+            self.SurrGba = [[Rbf(*arguments, self.Gba[:,i,j], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for j in range(len(self.elements))] for i in range(len(self.elements))]
+            
+            self.SurrogateDc = lambda x, T: np.array([self.SurrDc[i](*x, T) for i in range(len(self.elements))])
+            self.SurrogateCa = lambda x, T: np.array([self.SurrCa[i](*x, T) for i in range(len(self.elements))])
+            self.SurrogateCb = lambda x, T: np.array([self.SurrCb[i](*x, T) for i in range(len(self.elements))])
+            self.SurrogateGba = lambda x, T: np.array([[self.SurrGba[i][j](*x, T) for j in range(len(self.elements))] for i in range(len(self.elements))])
+            
+        else:
+            arguments = [self.dGcoords[:,i] for i in range(len(self.dGcoords[0]))]
+            self.LogSurrDc = [Rbf(*arguments, self.Dc[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
+            self.LogSurrMc = Rbf(*arguments, self.Mc, function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth)
+            self.LogSurrBeta = Rbf(*arguments, self.beta, function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth)
+            self.LogSurrCa = [Rbf(*arguments, self.Ca[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
+            self.LogSurrCb = [Rbf(*arguments, self.Cb[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
+            self.LogSurrGba = [[Rbf(*arguments, self.Gba[:,i,j], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for j in range(len(self.elements))] for i in range(len(self.elements))]
+            
+            self.SurrogateDc = lambda x, T: np.array([self.LogSurrDc[i](*(np.log10(x) / self.XICscale), T) for i in range(len(self.elements))])
+            self.SurrogateMc = lambda x, T: self.LogSurrMc(*(np.log10(x) / self.XICscale), T)
+            self.SurrogateBeta = lambda x, T: self.LogSurrBeta(*(np.log10(x) / self.XICscale), T)
+            self.SurrogateCa = lambda x, T: np.array([self.LogSurrCa[i](*(np.log10(x) / self.XICscale), T) for i in range(len(self.elements))])
+            self.SurrogateCb = lambda x, T: np.array([self.LogSurrCb[i](*(np.log10(x) / self.XICscale), T) for i in range(len(self.elements))])
+            self.SurrogateGba = lambda x, T: np.array([[self.LogSurrGba[i][j](*(np.log10(x) / self.XICscale), T) for j in range(len(self.elements))] for i in range(len(self.elements))])
+
+    def changeCurvatureHyperparameters(self, function = 'linear', epsilon = 1, smooth = 0):
         '''
-        Returns Gibbs Thomson contribution of a particle given its radius
+        Re-create surrogate model for curvature factors with updated hyperparameters
 
         Parameters
         ----------
-        radius : float or array
-            Precipitate radius
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
+        function : str (optional)
+            Radial basis function to use (defaults to 'linear')
+            Other functions are 'multiquadric', 'inverse_multiquadric',
+                'gaussian', 'cubic', 'quintic' and 'thin_plate'
+        epsilon : float
+            Scale for radial basis function (defaults to 1)
+            Training data will be scaled automatically
+                such that optimal scale is around 1
+        smooth : float
+            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
+        scale : float
+            Whether the composition training data should be in log or linear scale
+            Note: 'log' is recommended for dilute solutions
         '''
-        index = self.phaseIndex(phase)
-        return self.VmBeta[index] * (self.strainEnergy[index].strainEnergy(self.shapeFactors[index].normalRadii(radius)) + 2 * self.shapeFactors[index].thermoFactor(radius) * self.gamma[index] / radius)
+        if self.TICscale is None:
+            raise Exception("Curvature has not been trained.")
 
-    def neglectEffectiveDiffusionDistance(self, neglect = True):
-        '''
-        Whether or not to account for effective diffusion distance dependency on the supersaturation
-        By default, effective diffusion distance is considered
-        
-        Parameters
-        ----------
-        neglect : bool (optional)
-            If True (default), will assume effective diffusion distance is particle radius
-            If False, will calculate correction factor from Chen, Jeppson and Agren (2008)
-        '''
-        if neglect:
-            self.effDiffDistance = self.effDiffFuncs.noDiffusionDistance
-        else:
-            self.effDiffDistance = self.effDiffFuncs.effectiveDiffusionDistance
-
-    def addStoppingCondition(self, variable, condition, value, phase = None, element = None, mode = 'or'):
-        '''
-        Adds condition to stop simulation when condition is met
-
-        Parameters
-        ----------
-        variable : str
-            Variable to set condition for, options are 
-                'Volume Fraction'
-                'Average Radius'
-                'Driving Force'
-                'Nucleation Rate'
-                'Precipitate Density'
-        condition : str
-            Operator for condition, options are
-                'greater than' or '>'
-                'less than' or '<'
-        value : float
-            Value for condition
-        phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
-        element : str (optional)
-            For 'Composition', element to consider for condition (defaults to first element in list)
-        mode : str (optional)
-            How the condition will be handled
-                'or' (default) - at least one condition in this mode needs to be met before stopping
-                'and' - all conditions in this mode need to be met before stopping
-                    This will also record the times each condition is met
-
-        Example
-        model.addStoppingCondition('Volume Fraction', '>', 0.002, 'beta')
-            will add a condition to stop simulation when the volume fraction of the 'beta'
-            phase becomes greater than 0.002
-        '''
-        index = self.phaseIndex(phase)
-
-        if self._stoppingConditions is None:
-            self._stoppingConditions = []
-            self.stopConditionTimes = []
-            self._stopConditionMode = []
-
-        standardLabels = {
-            'Volume Fraction': 'betaFrac',
-            'Average Radius': 'avgR',
-            'Driving Force': 'dGs',
-            'Nucleation Rate': 'nucRate',
-            'Precipitate Density': 'precipitateDensity',
-        }
-        otherLabels = ['Composition']
-
-        if variable in standardLabels:
-            if 'greater' in condition or '>' in condition:
-                cond = lambda self, i, p = index, var=standardLabels[variable] : getattr(self, var)[p,i] > value
-            elif 'less' in condition or '<' in condition:
-                cond = lambda self, i, p = index, var=standardLabels[variable] : getattr(self, var)[p,i] < value
-        else:
-            if variable == 'Composition':
-                eIndex = 0 if element is None else self.elements.index(element)
-                if 'greater' in condition or '>' in condition:
-                    if self.numberOfElements > 1:
-                        cond = lambda self, i, e = eIndex, var='xComp' : getattr(self, var)[i, e] > value
-                    else:
-                        cond = lambda self, i, var='xComp' : getattr(self, var)[i] > value
-                elif 'less' in condition or '<' in condition:
-                    if self.numberOfElements > 1:
-                        cond = lambda self, i, e = eIndex, var='xComp' : getattr(self, var)[i, e] < value
-                    else:
-                        cond = lambda self, i, var='xComp' : getattr(self, var)[i] < value
-
-        self._stoppingConditions.append(cond)
-        self.stopConditionTimes.append(-1)
-        if mode == 'and':
-            self._stopConditionMode.append(False)
-        else:
-            self._stopConditionMode.append(True)
-
-    def clearStoppingConditions(self):
-        '''
-        Clears all stopping conditions
-        '''
-        self._stoppingConditions = None
-        self.stopConditionTimes = None
-        self._stopConditionMode = None
-
-    def printModelParameters(self):
-        '''
-        Prints the model parameters
-        '''
-        print('Temperature (K):               {:.3f}'.format(self.T[0]))
-        print('Initial Composition (at%):     {:.3f}'.format(100*self.xInit))
-        print('Molar Volume (m3):             {:.3e}'.format(self.VmAlpha))
-
-        for p in range(len(self.phases)):
-            print('Phase: {}'.format(self.phases[p]))
-            print('\tMolar Volume (m3):             {:.3e}'.format(self.VmBeta[p]))
-            print('\tInterfacial Energy (J/m2):     {:.3f}'.format(self.gamma[p]))
-            print('\tMinimum Radius (m):            {:.3e}'.format(self.Rmin[p]))
-
-    def setup(self):
-        '''
-        Sets up hidden parameters before solving
-        Here it's just the nucleation density and the grain boundary nucleation factors
-        '''
-        if not self._isNucleationSetup:
-            #Set nucleation density assuming grain size of 100 um and dislocation density of 5e12 m/m3 (Thermocalc default)
-            print('Nucleation density not set.\nSetting nucleation density assuming grain size of {:.0f} um and dislocation density of {:.0e} #/m2'.format(100, 5e12))
-            self.setNucleationDensity(100, 1, 5e12)
-        for p in range(len(self.phases)):
-            self.Rmin[p] = self.minRadius
-        self._getNucleationDensity()
-        self._setGBfactors()
-        self._setupStrainEnergyFactors()
-
-    def _printOutput(self, i):
-        '''
-        Prints various terms at step i
-        '''
-        if self.numberOfElements == 1:
-            print('N\tTime (s)\tTemperature (K)\tMatrix Comp')
-            print('{:.0f}\t{:.1e}\t\t{:.0f}\t\t{:.4f}\n'.format(i, self.time[i], self.T[i], 100*self.xComp[i]))
-        else:
-            compStr = 'N\tTime (s)\tTemperature (K)\t'
-            compValStr = '{:.0f}\t{:.1e}\t\t{:.0f}\t\t'.format(i, self.time[i], self.T[i])
-            for a in range(self.numberOfElements):
-                compStr += self.elements[a] + '\t'
-                compValStr += '{:.4f}\t'.format(100*self.xComp[i,a])
-            compValStr += '\n'
-            print(compStr)
-            print(compValStr)
-        print('\tPhase\tPrec Density (#/m3)\tVolume Frac\tAvg Radius (m)\tDriving Force (J/mol)')
-        for p in range(len(self.phases)):
-            print('\t{}\t{:.3e}\t\t{:.4f}\t\t{:.4e}\t{:.4e}'.format(self.phases[p], self.precipitateDensity[p,i], 100*self.betaFrac[p,i], self.avgR[p,i], self.dGs[p,i]*self.VmBeta[p]))
-        print('')
-                
-    def solve(self, verbose = False, vIt = 1000):
+        self.ICfunction = function
+        self.ICepsilon = epsilon
+        self.ICsmooth = np.amax([smooth, self.eps])
+
+        self._createICSurrogate()
+
+    def getCurvature(self, x, T):
         '''
-        Solves the KWN model between initial and final time
+        Gets driving force from surrogate models
         
-        Note: _calculateNucleationRate, _calculatePSD and _printOutput will need to be implemented in the child classes
-
         Parameters
         ----------
-        verbose : bool (optional)
-            Whether to print current simulation terms every couple iterations
-            Defaults to False
-        vIt : int (optional)
-            If verbose is True, vIt is how many iterations will pass before printing an output
-            Defaults to 1000
-        '''
-        self.setup()
-
-        t0 = time.time()
+        x : array or 2D array
+            Composition (array of float for each minor element)
+            2D arrays will have 0th axis for each set and 1st axis for composition
+        T : float or array
+            Temperature (must be float or same length as 0th axis of x if array)
         
-        #While loop since number of steps may change with adaptive time stepping
-        i = 1
-        stopCondition = False
-        while i < self.steps and not stopCondition:
-            self._iterate(i)
-
-            #Apply stopping condition
-            if self._stoppingConditions is not None:
-                andConditions = True
-                numberOfAndConditions = 0
-                orConditions = False
-                for s in range(len(self._stoppingConditions)):
-                    #Record time if stopping condition is met
-                    conditionResult = self._stoppingConditions[s](self, i)
-                    if conditionResult and self.stopConditionTimes[s] == -1:
-                        self.stopConditionTimes[s] = self.time[i]
-
-                    #If condition mode is 'or'
-                    if self._stopConditionMode[s]:
-                        orConditions = orConditions or conditionResult
-                    #If condition mode is 'and'
-                    else:
-                        andConditions = andConditions and conditionResult
-                        numberOfAndConditions += 1
-
-                #If there are no 'and' conditions, andConditions will be True
-                #Set to False so andConditions will not stop the model unneccesarily
-                if numberOfAndConditions == 0:
-                    andConditions = False
-
-                stopCondition = andConditions or orConditions
-
-            #Print current variables
-            if i % vIt == 0 and verbose:
-                self._printOutput(i)
+        Returns
+        -------
+        Curvature factors
+            {D-1 dCbar / dCbar^T M-1 dCbar} - for calculating interfacial composition of matrix
+            {1 / dCbar^T M-1 dCbar} - for calculating growth rate
+            {Gb^-1 Ga} - for calculating precipitate composition
+            Ca - interfacial composition of matrix phase
+            Cb - interfacial composition of precipitate phase
+        Note: this function currently does not return (None, None, None, None, None)
+            if precipitate is unstable
+        '''
+        if self.TICscale is None:
+            raise Exception("Curvature has not been trained.")
+
+        if self.linearIC:
+            dc = self.SurrogateDc(x / self.XICscale, T / self.TICscale)
+            mc = self.SurrogateMc(*(x / self.XICscale), T / self.TICscale)
+            gba = self.SurrogateGba(x / self.XICscale, T / self.TICscale)
+            beta = self.SurrogateBeta(*(x / self.XICscale), T / self.TICscale)
+            #beta = self.SurrogateBeta(x, T / self.TICscale)
+            ca = self.SurrogateCa(x / self.XICscale, T / self.TICscale)
+            cb = self.SurrogateCb(x / self.XICscale, T / self.TICscale)
             
-            i += 1
-
-        t1 = time.time()
-        if verbose:
-            print('Finished in {:.3f} seconds.'.format(t1 - t0))
+            return dc, mc, gba, beta, ca, cb
+            
+        else:
+            dc = self.SurrogateDc(x, T / self.TICscale)
+            mc = self.SurrogateMc(x, T / self.TICscale)
+            gba = self.SurrogateGba(x, T / self.TICscale)
+            beta = self.SurrogateBeta(x, T / self.TICscale)
+            ca = self.SurrogateCa(x, T / self.TICscale)
+            cb = self.SurrogateCb(x, T / self.TICscale)
+            
+            return dc, mc, gba, beta, ca, cb
 
-    def _iterate(self, i):
-        '''
-        Blank iteration function to be implemented in other classes
+    def getGrowthAndInterfacialComposition(self, x, T, dG, R, gExtra, searchDir = None):
         '''
-        pass
+        Returns growth rate and interfacial compostion given Gibbs-Thomson contribution
 
-    def _nucleationRate(self, p, i):
-        '''
-        Calculates nucleation rate at current timestep (normalized to number of nucleation sites)
-        This step is general to all systems except for how self._Beta is defined
-        
         Parameters
         ----------
-        p : int
-            Phase index (int)
-        i : int
-            Current iteration
-        dt : float
-            Current time increment
+        x : array of floats
+            Matrix composition
+        T : float
+            Temperature
+        dG : float
+            Driving force
+        R : float or array
+            Precipitate radius
+        gExtra : float or array
+            Gibbs-Thomson contribution corresponding to R
+            Must be same shape as R
+        
+        Returns
+        -------
+        (growth rate, matrix composition, precipitate composition)
+        Growth rate will be float or array depending on R
+        matrix and precipitate composition will be 1D or 2D array depending on R
+            1D array will be length of composition
+            2D array will have 0th axis be length of R and 1st axis be length of composition
         '''
-        #Most equations in literature take the driving force to be positive
-        #Although this really only changes the calculation of Rcrit since Z and beta is dG^2
-        self.dGs[p, i], _ = self.dG[p](self.xComp[i-1], self.T[i])
-        self.dGs[p, i] /= self.VmBeta[p]
+        if self.TICscale is None:
+            raise Exception("Curvature needs to be trained to calculated interfacial composition.")
 
-        #Add strain energy for spherical shape, use previous critical radius
-        #This should still be correct even if the interfacial energy dominates at small radii since the aspect ratio may be near 1
-        self.dGs[p, i] -= self.strainEnergy[p].strainEnergy(self.shapeFactors[p].normalRadii(self.Rcrit[p, i-1]))
+        if hasattr(R, '__len__'):
+            R = np.array(R)
+        if hasattr(gExtra, '__len__'):
+            gExtra = np.array(gExtra)
 
-        if self.dGs[p, i] < 0:
-            return self._noDrivingForce(p, i)
+        dc, mc, gba, beta, ca, cb = self.getCurvature(x, T)
 
-        #Only do this if there is some parent phase left (brute force solution for to avoid numerical errors)
-        if self.betaFrac[p, i-1] < 1:
+        Rdiff = (dG - gExtra)
 
-            #Calculate critical radius
-            #For bulk or dislocation nucleation sites, use previous critical radius to get aspect ratio
-            if self.GB[p].nucleationSiteType == GBFactors.BULK or self.GB[p].nucleationSiteType == GBFactors.DISLOCATION:
-                self.Rcrit[p, i] = 2 * self.shapeFactors[p].thermoFactor(self.Rcrit[p, i-1]) * self.gamma[p] / self.dGs[p, i]
-                #self.Rcrit[p, i] = 2 * self.gamma[p] / self.dGs[p, i]
-                if self.Rcrit[p, i] < self.Rmin[p]:
-                    self.Rcrit[p, i] = self.Rmin[p]
-                
-                self.Gcrit[p, i] = (4 * np.pi / 3) * self.gamma[p] * self.Rcrit[p, i]**2
+        gr = (mc / R) * Rdiff
 
-            #If nucleation is on a grain boundary, then use the critical radius as defined by the grain boundary type    
-            else:
-                self.Rcrit[p, i] = self.GB[p].Rcrit(self.dGs[p, i])
-                if self.Rcrit[p, i] < self.Rmin[p]:
-                    self.Rcrit[p, i] = self.Rmin[p]
-                    
-                self.Gcrit[p, i] = self.GB[p].Gcrit(self.dGs[p, i], self.Rcrit[p, i])
+        if hasattr(Rdiff, '__len__'):
+            calpha = np.zeros((len(Rdiff), len(self.elements)))
+            dca = np.zeros((len(Rdiff), len(self.elements)))
+            cbeta = np.zeros((len(Rdiff), len(self.elements)))
+            for i in range(len(self.elements)):
+                calpha[:,i] = x[i] - dc[i] * Rdiff
+                dca[:,i] = calpha[:,i] - ca[i]
 
-            #Calculate nucleation rate
-            Z = self._Zeldovich(p, i)
-            self.betas[p,i] = self._Beta(p, i)
-            if self.betas[p,i] == 0:
-                return self._noDrivingForce(p, i)
+            dcb = np.matmul(gba, dca.T)
+            for i in range(len(self.elements)):
+                cbeta[:,i] = cb[i] + dcb[i,:]
 
-            #Incubation time, either isothermal or nonisothermal
-            self.incubationSum[p] = self._incubation(Z, p, i)
-            if self.incubationSum[p] > 1:
-                self.incubationSum[p] = 1
-
-            return Z * self.betas[p,i] * np.exp(-self.Gcrit[p, i] / (self.kB * self.T[i])) * self.incubationSum[p]
+            calpha[calpha < 0] = 0
+            cbeta[cbeta < 0] = 0
 
+            return gr, calpha, cbeta, ca, cb
         else:
-            return self._noDrivingForce(p, i)
-            
-    def _noCheckDT(self, i):
-        '''
-        Default for no adaptive time stepping
-        '''
-        pass
-
-    def _noPostCheckDT(self, i):
-        '''
-        Default for no adaptive time stepping
-        '''
-        pass
+            calpha = x - dc * Rdiff
+            cbeta = cb + np.matmul(gba, (calpha - ca)).flatten()
 
-    def _checkDT(self, i):
-        '''
-        Default time increment function if implement (which is no implementation)
-        '''
-        pass
+            calpha[calpha < 0] = 0
+            cbeta[cbeta < 0] = 0
 
-    def _postCheckDT(self, i):
-        '''
-        Default time increment function if implement (which is no implementation)
-        '''
-        pass
-
-    def _noDrivingForce(self, p, i):
-        '''
-        Set everything to 0 if there is no driving force for precipitation
-        '''
-        self.Rcrit[p, i] = 0
-        self.incubationOffset[p] = np.amax([i-1, 0])
-        return 0
-
-    def _nucleateFreeEnergy(self, Rsph, p, i):
-        '''
-        Free energy change for a nucleate with radius of Rsph
-        '''
-        volContribution = 4/3 * np.pi * Rsph**3 * (self.dGs[p,i] + self.strainEnergy[p].strainEnergy(self.shapeFactors[p].normalRadii(Rsph)))
-        areaContribution = 4 * np.pi * self.gamma[p] * Rsph**2 * self.shapeFactors[p].thermoFactor(Rsph)
-        return -volContribution + areaContribution
+            return gr, calpha, cbeta, ca, cb
 
-    def _Zeldovich(self, p, i):
-        '''
-        Zeldovich factor - probability that cluster at height of nucleation barrier will continue to grow
-        '''
-        return np.sqrt(3 * self.GB[p].volumeFactor / (4 * np.pi)) * self.VmBeta[p] * np.sqrt(self.gamma[p] / (self.kB * self.T[i])) / (2 * np.pi * self.avo * self.Rcrit[p,i]**2)
-        
-    def _BetaBinary1(self, p, i):
-        '''
-        Impingement rate for binary systems using Perez et al
+    def impingementFactor(self, x, T):
         '''
-        return self.GB[p].areaFactor * self.Rcrit[p,i]**2 * self.xComp[0] * self.Diffusivity(self.xComp[i-1], self.T[i]) / self.aAlpha**4
+        Calculates impingement factor for nucleation rate calculations
 
-    def _BetaBinary2(self, p, i):
-        '''
-        Impingement rate for binary systems taken from Thermocalc prisma documentation
-        This will follow the same equation as with _BetaMulti; however, some simplications can be made based off the summation contraint
-        '''
-        D = self.Diffusivity(self.xComp[i-1], self.T[i])
-        Dfactor = (self.xEqBeta[p,i-1] - self.xEqAlpha[p,i-1])**2 / (self.xEqAlpha[p,i-1]*D) + (self.xEqBeta[p,i-1] - self.xEqAlpha[p,i-1])**2 / ((1 - self.xEqAlpha[p,i-1])*D)
-        return self.GB[p].areaFactor * self.Rcrit[p,i]**2 * (1/Dfactor) / self.aAlpha**4
-            
-    def _BetaMulti(self, p, i):
-        '''
-        Impingement rate for multicomponent systems
+        Parameters
+        ----------
+        x : array of floats
+            Matrix composition
+        T : float
+            Temperature
         '''
-        if self._betaFuncs[p] is None:
-            return self._defaultBeta
+        if self.TICscale is None:
+            raise Exception("Curvature needs to be trained to calculated impingement factor.")
+        #return self.SurrogateBeta(x, T / self.TICscale)
+        if self.linearIC:
+            return self.SurrogateBeta(*(x / self.XICscale), T / self.TICscale)
         else:
-            beta = self._betaFuncs[p](self.xComp[i-1], self.T[i-1])
-            if beta is None:
-                return self.betas[p,i-1]
-            else:
-                return (self.GB[p].areaFactor * self.Rcrit[p, i]**2 / self.aAlpha**4) * beta
+            return self.SurrogateBeta(x, T / self.TICscale)
 
-    def _incubationIsothermal(self, Z, p, i):
-        '''
-        Incubation time for isothermal conditions
-        '''
-        tau = 1 / (self.theta[p] * (self.betas[p,i] * Z**2))
-        return np.exp(-tau / self.time[i])
-        
-    def _incubationNonIsothermal(self, Z, p, i):
+    def save(self, fileName):
         '''
-        Incubation time for non-isothermal conditions
-        This must match isothermal conditions if the temperature is constant
+        Pickles surrogate data
+        Note: this will remove the user-defined driving force and curvature functions
+            This is not a problem; however, a loaded surrogate will not be
+            able to be re-trained with different training points
 
-        Solve for integral(beta(t-t0)) from 0 to tau = 1/theta*Z(tau)^2
+        Parameters
+        ----------
+        fileName : str
         '''
-        LHS = 1 / (self.theta[p] * Z**2 * (self.T[i] / self.T[int(self.incubationOffset[p]):]))
+        self.therm = None
+        self.drivingForceFunction = None
+        self.interfacialCompositionFunction = None
+        self.curvature = None
 
-        RHS = np.cumsum(self.betas[p,int(self.incubationOffset[p])+1:i] * (self.time[int(self.incubationOffset[p])+1:i] - self.time[int(self.incubationOffset[p]):i-1]))
-        if len(RHS) == 0:
-            RHS = self.betas[p,i] * (self.time[int(self.incubationOffset[p]):] - self.time[int(self.incubationOffset[p])])
-        else:
-            RHS = np.concatenate((RHS, RHS[-1] + self.betas[p,i] * (self.time[i-1:] - self.time[int(self.incubationOffset[p])])))
+        self.SurrogateDrivingForce = None
+        self.SurrPrecComp = None
+        self.SurrogatePrecComp = None
+        self.LogSurrDG = None
+        self.LogSurrPrecComp = None
 
-        #Test for intersection
-        diff = RHS - LHS
-        signChange = np.sign(diff[:-1]) != np.sign(diff[1:])
+        self.SurrDc = None
+        self.SurrCa = None
+        self.SurrCb = None
+        self.SurrGba = None
 
-        #If no intersection
-        if not any(signChange):
-            #If RHS > LHS, then intersection is at t = 0
-            if diff[0] > 0:
-                tau = 0
-            #Else, RHS intersects LHS beyond simulation time
-            #Extrapolate integral of RHS from last point to intersect LHS
-            #integral(beta(t-t0)) from t0 to ti + beta_i * (tau - (ti - t0)) = 1 / theta * Z(tau+t0)^2
-            else:
-                tau = LHS[-1] / self.betas[p,i] - RHS[-1] / self.betas[p,i] + (self.time[i] - self.time[int(self.incubationOffset[p])])
-        else:
-            tau = self.time[int(self.incubationOffset[p]):-1][signChange][0] - self.time[int(self.incubationOffset[p])]
+        self.LogSurrDc = None
+        self.LogSurrMc = None
+        self.LogSurrBeta = None
+        self.LogSurrCa = None
+        self.LogSurrCb = None
+        self.LogSurrGba = None
+        
+        self.SurrogateDc = None
+        self.SurrogateMc = None
+        self.SurrogateBeta = None
+        self.SurrogateCa = None
+        self.SurrogateCb = None
+        self.SurrogateGba = None
 
-        return np.exp(-tau / (self.time[i] - self.time[int(self.incubationOffset[p])]))
+        with open(fileName, 'wb') as file:
+            pickle.dump(self, file)
 
-    def _setNucleateRadius(self, i):
-        '''
-        Adds 1/2 * sqrt(kb T / pi gamma) to critical radius to ensure they grow when growth rates are calculated
-        '''
-        for p in range(len(self.phases)):
-            #If nucleates form, then calculate radius of precipitate
-            #Radius is set slightly larger so precipitate 
-            if self.nucRate[p,i]*(self.time[i]-self.time[i-1]) >= self.minNucleateDensity and self.Rcrit[p, i] >= self.Rmin[p]:
-                self.Rad[p, i] = self.Rcrit[p, i] + 0.5 * np.sqrt(self.kB * self.T[i] / (np.pi * self.gamma[p]))
-            else:
-                self.Rad[p, i] = 0
+        if self.TDGscale is not None:
+            self._createDGSurrogate()
+        if self.TICscale is not None:
+            self._createICSurrogate()
 
-    def getTimeAxis(self, timeUnits='s', bounds=None):
+    def load(fileName):
         '''
-        Returns scaling factor, label and x-limits depending on units of time
+        Loads data from a pickled surrogate and builds driving force and curvature functions
 
         Parameters
         ----------
-        timeUnits : str
-            's' / 'sec' / 'seconds' - seconds
-            'min' / 'minutes' - minutes
-            'h' / 'hrs' / 'hours' - hours
-        '''
-        timeScale = 1
-        timeLabel = 'Time (s)'
-        if 'min' in timeUnits:
-            timeScale = 1/60
-            timeLabel = 'Time (min)'
-        if 'h' in timeUnits:
-            timeScale = 1/3600
-            timeLabel = 'Time (hrs)'
+        fileName : str
 
-        if bounds is None:
-            if self.t0 == 0:
-                bounds = [timeScale * 1e-5 * self.tf, timeScale * self.tf]
-            else:
-                bounds = [timeScale * self.t0, timeScale * self.tf]
-
-        return timeScale, timeLabel, bounds
-        
-    
-    def plot(self, axes, variable, bounds = None, timeUnits = 's', radius='spherical', *args, **kwargs):
+        Returns
+        -------
+        MulticomponentSurrogate object
         '''
-        Plots model outputs
-        
-        Parameters
-        ----------
-        axes : Axis
-        variable : str
-            Specified variable to plot
-            Options are 'Volume Fraction', 'Total Volume Fraction', 'Critical Radius',
-                'Average Radius', 'Volume Average Radius', 'Total Average Radius', 
-                'Total Volume Average Radius', 'Aspect Ratio', 'Total Aspect Ratio'
-                'Driving Force', 'Nucleation Rate', 'Total Nucleation Rate',
-                'Precipitate Density', 'Total Precipitate Density', 
-                'Temperature' and 'Composition'
+        surr = None
+        with open(fileName, 'rb') as file:
+            surr = pickle.load(file)
+
+        if surr.TDGscale is not None:
+            surr._createDGSurrogate()
+        if surr.TICscale is not None:
+            surr._createICSurrogate()
 
-                Note: for multi-phase simulations, adding the word 'Total' will
-                    sum the variable for all phases. Without the word 'Total', the variable
-                    for each phase will be plotted separately
-                    
-        bounds : tuple (optional)
-            Limits on the x-axis (float, float) or None (default, this will set bounds to (initial time, final time))
-        timeUnits : str (optional)
-            Plot time dependent variables per seconds ('s'), minutes ('min') or hours ('h')
-        radius : str (optional)
-            For non-spherical precipitates, plot the Average Radius by the -
-                Equivalent spherical radius ('spherical')
-                Short axis ('short')
-                Long axis ('long')
-            Note: Total Average Radius and Volume Average Radius will still use the equivalent spherical radius
-        *args, **kwargs - extra arguments for plotting
-        '''
-        timeScale, timeLabel, bounds = self.getTimeAxis(timeUnits, bounds)
-
-        axes.set_xlabel(timeLabel)
-        axes.set_xlim(bounds)
-
-        labels = {
-            'Volume Fraction': 'Volume Fraction',
-            'Total Volume Fraction': 'Volume Fraction',
-            'Critical Radius': 'Critical Radius (m)',
-            'Average Radius': 'Average Radius (m)',
-            'Volume Average Radius': 'Volume Average Radius (m)',
-            'Total Average Radius': 'Average Radius (m)',
-            'Total Volume Average Radius': 'Volume Average Radius (m)',
-            'Aspect Ratio': 'Mean Aspect Ratio',
-            'Total Aspect Ratio': 'Mean Aspect Ratio',
-            'Driving Force': 'Driving Force (J/m$^3$)',
-            'Nucleation Rate': 'Nucleation Rate (#/m$^3$-s)',
-            'Total Nucleation Rate': 'Nucleation Rate (#/m$^3$-s)',
-            'Precipitate Density': 'Precipitate Density (#/m$^3$)',
-            'Total Precipitate Density': 'Precipitate Density (#/m$^3$)',
-            'Temperature': 'Temperature (K)',
-            'Composition': 'Matrix Composition (at.%)',
-            'Eq Composition Alpha': 'Matrix Composition (at.%)',
-            'Eq Composition Beta': 'Matrix Composition (at.%)',
-            'Supersaturation': 'Supersaturation',
-            'Eq Volume Fraction': 'Volume Fraction'
-        }
-
-        totalVariables = ['Total Volume Fraction', 'Total Average Radius', 'Total Aspect Ratio', \
-                            'Total Nucleation Rate', 'Total Precipitate Density']
-        singleVariables = ['Volume Fraction', 'Critical Radius', 'Average Radius', 'Aspect Ratio', \
-                            'Driving Force', 'Nucleation Rate', 'Precipitate Density']
-        eqCompositions = ['Eq Composition Alpha', 'Eq Composition Beta']
-        saturations = ['Supersaturation', 'Eq Volume Fraction']
-
-        if variable == 'Temperature':
-            axes.semilogx(timeScale * self.time, self.T, *args, **kwargs)
-            axes.set_ylabel(labels[variable])
-
-        elif variable == 'Composition':
-            if self.numberOfElements == 1:
-                axes.semilogx(timeScale * self.time, self.xComp, *args, **kwargs)
-                axes.set_ylabel('Matrix Composition (at.% ' + self.elements[0] + ')')
-            else:
-                for i in range(self.numberOfElements):
-                    #Keep color consistent between Composition, Eq Composition Alpha and Eq Composition Beta if color isn't passed as an arguement
-                    if 'color' in kwargs:
-                        axes.semilogx(timeScale * self.time, self.xComp[:,i], label=self.elements[i], *args, **kwargs)
-                    else:
-                        axes.semilogx(timeScale * self.time, self.xComp[:,i], label=self.elements[i], color='C'+str(i), *args, **kwargs)
-                axes.legend(self.elements)
-                axes.set_ylabel(labels[variable])
-            yRange = [np.amin(self.xComp), np.amax(self.xComp)]
-            axes.set_ylim([yRange[0] - 0.1 * (yRange[1] - yRange[0]), yRange[1] + 0.1 * (yRange[1] - yRange[0])])
-
-        elif variable in eqCompositions:
-            if variable == 'Eq Composition Alpha':
-                plotVariable = self.xEqAlpha
-            elif variable == 'Eq Composition Beta':
-                plotVariable = self.xEqBeta
-
-            if len(self.phases) == 1:
-                if self.numberOfElements == 1:
-                    axes.semilogx(timeScale * self.time, plotVariable[0], *args, **kwargs)
-                    axes.set_ylabel('Matrix Composition (at.% ' + self.elements[0] + ')')
-                else:
-                    for i in range(self.numberOfElements):
-                        #Keep color consistent between Composition, Eq Composition Alpha and Eq Composition Beta if color isn't passed as an arguement
-                        if 'color' in kwargs:
-                            axes.semilogx(timeScale * self.time, plotVariable[0,:,i], label=self.elements[i]+'_Eq', *args, **kwargs)
-                        else:
-                            axes.semilogx(timeScale * self.time, plotVariable[0,:,i], label=self.elements[i]+'_Eq', color='C'+str(i), *args, **kwargs)
-                    axes.legend()
-                    axes.set_ylabel(labels[variable])
-            else:
-                if self.numberOfElements == 1:
-                    for p in range(len(self.phases)):
-                        #Keep color somewhat consistent between Composition, Eq Composition Alpha and Eq Composition Beta if color isn't passed as an arguement
-                        if 'color' in kwargs:
-                            axes.semilogx(timeScale * self.time, plotVariable[p], label=self.phases[p]+'_Eq', *args, **kwargs)
-                        else:
-                            axes.semilogx(timeScale * self.time, plotVariable[p], label=self.phases[p]+'_Eq', color='C'+str(p), *args, **kwargs)
-                    axes.legend()
-                    axes.set_ylabel('Matrix Composition (at.% ' + self.elements[0] + ')')
-                else:
-                    cIndex = 0
-                    for p in range(len(self.phases)):
-                        for i in range(self.numberOfElements):
-                            #Keep color somewhat consistent between Composition, Eq Composition Alpha and Eq Composition Beta if color isn't passed as an arguement
-                            if 'color' in kwargs:
-                                axes.semilogx(timeScale * self.time, plotVariable[p,:,i], label=self.phases[p]+'_'+self.elements[i]+'_Eq', *args, **kwargs)
-                            else:
-                                axes.semilogx(timeScale * self.time, plotVariable[p,:,i], label=self.phases[p]+'_'+self.elements[i]+'_Eq', color='C'+str(cIndex), *args, **kwargs)
-                            cIndex += 1
-                    axes.legend()
-                    axes.set_ylabel(labels[variable])
-
-        elif variable in saturations:
-            #Since supersaturation is calculated in respect to the tie-line, it is the same for each element
-            #Thus only a single element is needed
-            plotVariable = np.zeros(self.betaFrac.shape)
-            for p in range(len(self.phases)):
-                if self.numberOfElements == 1:
-                    if variable == 'Eq Volume Fraction':
-                        num = self.xComp[0] - self.xEqAlpha[p]
-                    else:
-                        num = self.xComp - self.xEqAlpha[p]
-                    den = self.xEqBeta[p] - self.xEqAlpha[p]
-                else:
-                    if variable == 'Eq Volume Fraction':
-                        num = self.xComp[0,0] - self.xEqAlpha[p,:,0]
-                    else:
-                        num = self.xComp[:,0] - self.xEqAlpha[p,:,0]
-                    den = self.xEqBeta[p,:,0] - self.xEqAlpha[p,:,0]
-                #If precipitate is unstable, both xEqAlpha and xEqBeta are set to 0
-                #For these cases, change the values of numerator and denominator so that supersaturation is 0 instead of undefined
-                num[den == 0] = 0
-                den[den == 0] = 1
-                plotVariable[p] = num / den
-            
-            if len(self.phases) == 1:
-                axes.semilogx(timeScale * self.time, plotVariable[0], *args, **kwargs)
-            else:
-                for p in range(len(self.phases)):
-                    if 'color' in kwargs:
-                        axes.semilogx(timeScale * self.time, plotVariable[p], label=self.phases[p], *args, **kwargs)
-                    else:
-                        axes.semilogx(timeScale * self.time, plotVariable[p], label=self.phases[p], color='C'+str(p), *args, **kwargs)
-                axes.legend()
-            axes.set_ylabel(labels[variable])
-
-        elif variable in singleVariables:
-            if variable == 'Volume Fraction':
-                plotVariable = self.betaFrac
-            elif variable == 'Critical Radius':
-                plotVariable = self.Rcrit
-            elif variable == 'Average Radius':
-                plotVariable = self.avgR
-                for p in range(len(self.phases)):
-                    if self.GB[p].nucleationSiteType == self.GB[p].BULK or self.GB[p].nucleationSiteType == self.GB[p].DISLOCATION:
-                        if radius != 'spherical':
-                            plotVariable[p] /= self.shapeFactors[p].eqRadiusFactor(self.avgR[p])
-                        if radius == 'long':
-                            plotVariable[p] *= self.avgAR[p]
-                    else:
-                        plotVariable[p] *= self._GBareaRemoval(p)
-
-            elif variable == 'Volume Average Radius':
-                plotVariable = np.cbrt(self.betaFrac / self.precipitateDensity / (4/3*np.pi))
-            elif variable == 'Aspect Ratio':
-                plotVariable = self.avgAR
-            elif variable == 'Driving Force':
-                plotVariable = self.dGs
-            elif variable == 'Nucleation Rate':
-                plotVariable = self.nucRate
-            elif variable == 'Precipitate Density':
-                plotVariable = self.precipitateDensity
-
-            if (len(self.phases)) == 1:
-                axes.semilogx(timeScale * self.time, plotVariable[0], *args, **kwargs)
-            else:
-                for p in range(len(self.phases)):
-                    axes.semilogx(timeScale * self.time, plotVariable[p], label=self.phases[p], color='C'+str(p), *args, **kwargs)
-                axes.legend()
-            axes.set_ylabel(labels[variable])
-            yb = 1 if variable == 'Aspect Ratio' else 0
-            axes.set_ylim([yb, 1.1 * np.amax(plotVariable)])
-
-        elif variable in totalVariables:
-            if variable == 'Total Volume Fraction':
-                plotVariable = np.sum(self.betaFrac, axis=0)
-            elif variable == 'Total Average Radius':
-                totalN = np.sum(self.precipitateDensity, axis=0)
-                totalN[totalN == 0] = 1
-                totalR = np.sum(self.avgR * self.precipitateDensity, axis=0)
-                plotVariable = totalR / totalN
-            elif variable == 'Total Volume Average Radius':
-                totalN = np.sum(self.precipitateDensity, axis=0)
-                totalN[totalN == 0] = 1
-                totalVol = np.sum(self.betaFrac, axis=0)
-                plotVariable = np.cbrt(totalVol / totalN)
-            elif variable == 'Total Aspect Ratio':
-                totalN = np.sum(self.precipitateDensity, axis=0)
-                totalN[totalN == 0] = 1
-                totalAR = np.sum(self.avgAR * self.precipitateDensity, axis=0)
-                plotVariable = totalAR / totalN
-            elif variable == 'Total Nucleation Rate':
-                plotVariable = np.sum(self.nucRate, axis=0)
-            elif variable == 'Total Precipitate Density':
-                plotVariable = np.sum(self.precipitateDensity, axis=0)
-
-            axes.semilogx(timeScale * self.time, plotVariable, *args, **kwargs)
-            axes.set_ylabel(labels[variable])
-            yb = 1 if variable == 'Total Aspect Ratio' else 0
-            axes.set_ylim(bottom=yb)
+        return surr
+
```

### Comparing `kawin-0.2.0/kawin/KWNEuler.py` & `kawin-0.3.0/kawin/precipitation/KWNEuler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,280 +1,87 @@
 import numpy as np
-from kawin.KWNBase import PrecipitateBase
-from kawin.PopulationBalance import PopulationBalanceModel
-from kawin.GrainBoundaries import GBFactors
-import copy
-import csv
-from itertools import zip_longest
-import time
+from kawin.precipitation.KWNBase import PrecipitateBase
+from kawin.precipitation.PopulationBalance import PopulationBalanceModel
+from kawin.precipitation.non_ideal.GrainBoundaries import GBFactors
+from kawin.precipitation.Plot import plotEuler
 
 class PrecipitateModel (PrecipitateBase):
     '''
-    Euler implementation of the KWN model designed for binary systems
+    Euler implementation of KWN model
 
     Parameters
     ----------
-    t0 : float
-        Initial time in seconds
-    tf : float
-        Final time in seconds
-    steps : int
-        Number of time steps
     phases : list (optional)
         Precipitate phases (array of str)
         If only one phase is considered, the default is ['beta']
-    linearTimeSpacing : bool (optional)
-        Whether to have time increment spaced linearly or logarithimically
-        Defaults to False
     elements : list (optional)
         Solute elements in system
         Note: order of elements must correspond to order of elements set in Thermodynamics module
         If binary system, then defualt is ['solute']
     '''
-    def __init__(self, t0, tf, steps, phases = ['beta'], linearTimeSpacing = False, elements = ['solute']):
-        #Initialize base class
-        super().__init__(t0, tf, steps, phases, linearTimeSpacing, elements)
+    def __init__(self, phases = ['beta'], elements = ['solute']):
+        super().__init__(phases, elements)
 
         if self.numberOfElements == 1:
             self._growthRate = self._growthRateBinary
             self._Beta = self._BetaBinary1
         else:
             self._growthRate = self._growthRateMulti
             self._Beta = self._BetaMulti
 
-        #Additional outputs
-        self.additionalFunctions = []
-        self.additionalFunctionNames = []
-        self.additionalOutputs = None
+        self.eqAspectRatio = [None for p in range(len(self.phases))]
 
     def _resetArrays(self):
         '''
         Resets and initializes arrays for all variables
 
         In addition to PrecipitateBase, the equilibrium aspect ratio area and population balance models are created here
         '''
         super()._resetArrays()
         self.PBM = [PopulationBalanceModel() for p in self.phases]
 
-        #Index of particle size classes which below, precipitates are unstable
         self.RdrivingForceIndex = np.zeros(len(self.phases), dtype=np.int32)
-
-        #Aspect ratio
-        self.eqAspectRatio = [[] for p in self.phases]
-
+        self.dissolutionIndex = np.zeros(len(self.phases), dtype=np.int32)
+        
     def reset(self):
         '''
         Resets model results
         '''
         super().reset()
 
-        #Bounds of the bins in PSD
         for i in range(len(self.phases)):
             self.PBM[i].reset()
+            self.PBM[i].resetRecordedData()
 
-        #Resets PSD outputs
-        self._setupAdditionalOutputs()
-
-    def save(self, filename, compressed = False, toCSV = False):
-        '''
-        Save results into a numpy .npz format
-
-        Parameters
-        ----------
-        filename : str
-        compressed : bool
-            If true, will save compressed .npz format
-        toCSV : bool
-            If true, wil save to .csv
-        '''
-        variables = ['t0', 'tf', 'steps', 'phases', 'linearTimeSpacing', 'elements', \
-            'time', 'xComp', 'Rcrit', 'Gcrit', 'Rad', 'avgR', 'avgAR', 'betaFrac', 'nucRate', 'precipitateDensity', 'dGs', 'xEqAlpha', 'xEqBeta']
-        vDict = {v: getattr(self, v) for v in variables}
-        if self.additionalOutputs is not None:
-            vDict['additionalOutputs'] = self.additionalOutputs
-            if not toCSV:
-                vDict['additionalFunctionNames'] = self.additionalFunctionNames
+    def _addExtraSaveVariables(self, saveDict):
         for p in range(len(self.phases)):
-            vDict['PSDdata_'+self.phases[p]] = [self.PBM[p].min, self.PBM[p].max, self.PBM[p].bins]
-            vDict['PSDsize_' + self.phases[p]] = self.PBM[p].PSDsize
-            vDict['PSD_' + self.phases[p]] = self.PBM[p].PSD
-            vDict['PSDbounds_' + self.phases[p]] = self.PBM[p].PSDbounds
-            vDict['eqAspectRatio_' + self.phases[p]] = self.eqAspectRatio[p]
-
-        if toCSV:
-            vDict['t0'] = np.array([vDict['t0']])
-            vDict['tf'] = np.array([vDict['tf']])
-            vDict['steps'] = np.array([vDict['steps']])
-            vDict['linearTimeSpacing'] = np.array([vDict['linearTimeSpacing']])
-            if self.numberOfElements == 2:
-                vDict['xComp'] = vDict['xComp'].T
-            arrays = []
-            headers = []
-            for v in vDict:
-                vDict[v] = np.array(vDict[v])
-                if len(vDict[v].shape) == 2:
-                    for i in range(len(vDict[v])):
-                        arrays.append(vDict[v][i])
-                        if v == 'xComp':
-                            headers.append(v + '_' + self.elements[i])
-                        else:
-                            headers.append(v + '_' + self.phases[i])
-                elif v == 'xEqAlpha' or v == 'xEqBeta':
-                    for i in range(len(self.phases)):
-                        for j in range(self.numberOfElements):
-                            arrays.append(vDict[v][i,:,j])
-                            headers.append(v + '_' + self.phases[i] + '_' + self.elements[j])
-                elif v == 'additionalOutputs':
-                    for i in range(len(self.phases)):
-                        for j in range(len(self.additionalFunctionNames)):
-                            arrays.append(vDict[v][i,:,j])
-                            headers.append(v + '_' + self.phases[i] + '_' + self.additionalFunctionNames[j])
-                else:
-                    arrays.append(vDict[v])
-                    headers.append(v)
-            rows = zip_longest(*arrays, fillvalue='')
-            if '.csv' not in filename.lower():
-                filename = filename + '.csv'
-            with open(filename, 'w', newline='') as f:
-                csv.writer(f).writerow(headers)
-                csv.writer(f).writerows(rows)
-        else:
-            if compressed:
-                np.savez_compressed(filename, **vDict)
-                #np.savez_compressed(filename, **vDict, allow_pickle=True)
-            else:
-                np.savez(filename, **vDict)
-                #np.savez(filename, **vDict, allow_pickle=True)
+            saveDict['PBM_data_' + self.phases[p]] = [self.PBM[p].min, self.PBM[p].max, self.PBM[p].bins]
+            saveDict['PBM_PSD_' + self.phases[p]] = self.PBM[p].PSD
+            saveDict['PBM_bounds_' + self.phases[p]] = self.PBM[p].PSDbounds
+            saveDict['PBM_size_' + self.phases[p]] = self.PBM[p].PSDsize
+            saveDict['eqAspectRatio_' + self.phases[p]] = self.eqAspectRatio[p]
 
     def load(filename):
-        '''
-        Loads data
-
-        Parameters
-        ----------
-        filename : str
-
-        Returns
-        -------
-        PrecipitateModel object
-            Note: this will only contain model outputs which can be used for plotting
-        '''
-        setupVars = ['t0', 'tf', 'steps', 'phases', 'linearTimeSpacing', 'elements']
-        if '.np' in filename.lower():
-            data = np.load(filename, allow_pickle=True)
-            
-            #Input arbitrary values for PSD parameters (rMin, rMax, bins) since this will be changed shortly after
-            model = PrecipitateModel(data['t0'], data['tf'], data['steps'], data['phases'], data['linearTimeSpacing'], data['elements'])
-            for p in range(len(model.phases)):
-                PSDvars = ['PSDdata_' + model.phases[p], 'PSD_' + model.phases[p], 'PSDsize_' + model.phases[p], 'eqAspectRatio_' + model.phases[p], 'PSDbounds_' + model.phases[p]]
-                #For back compatibility
-                if PSDvars[0] not in data:
-                    PSDvars = ['PSDdata' + str(p), 'PSD' + str(p), 'PSDsize' + str(p), 'eqAspectRatio' + str(p), 'PSDbounds' + str(p)]
-                setupVars = np.concatenate((setupVars, PSDvars))
-                model.PBM[p] = PopulationBalanceModel(data[PSDvars[0]][0], data[PSDvars[0]][1], int(data[PSDvars[0]][2]), True)
-                model.PBM[p].PSD = data[PSDvars[1]]
-                model.PBM[p].PSDsize = data[PSDvars[2]]
-                model.eqAspectRatio[p] = data[PSDvars[3]]
-                model.PBM[p].PSDbounds = data[PSDvars[4]]
-            for d in data:
-                if d not in setupVars:
-                    setattr(model, d, data[d])
-            if 'additionalOutputs' not in data:
-                model.additionalOutputs = None
-                model.additionalFunctions = []
-                model.additionalFunctionNames = []
-        elif '.csv' in filename.lower():
-            with open(filename, 'r') as csvFile:
-                data = csv.reader(csvFile, delimiter=',')
-                i = 0
-                headers = []
-                columns = {}
-                #Grab all columns
-                for row in data:
-                    if i == 0:
-                        headers = row
-                        columns = {h: [] for h in headers}
-                    else:
-                        for j in range(len(row)):
-                            if row[j] != '':
-                                columns[headers[j]].append(row[j])
-                    i += 1
-
-                t0, tf, steps, phases, elements = float(columns['t0'][0]), float(columns['tf'][0]), int(columns['steps'][0]), columns['phases'], columns['elements']
-                linearTimeSpacing = True if columns['linearTimeSpacing'][0] == 'True' else False
-                model = PrecipitateModel(t0, tf, steps, phases, linearTimeSpacing, elements)
-
-                for p in range(len(model.phases)):
-                    PSDvars = ['PSDdata_' + model.phases[p], 'PSD_' + model.phases[p], 'PSDsize_' + model.phases[p], 'eqAspectRatio_' + model.phases[p], 'PSDbounds_' + model.phases[p]]
-                    #For back compatibility
-                    if PSDvars[0] not in columns:
-                        PSDvars = ['PSDdata' + str(p), 'PSD' + str(p), 'PSDsize' + str(p), 'eqAspectRatio' + str(p), 'PSDbounds' + str(p)]
-                    setupVars = np.concatenate((setupVars, PSDvars))
-                    model.PBM[p] = PopulationBalanceModel(float(columns[PSDvars[0]][0]), float(columns[PSDvars[0]][1]), int(float(columns[PSDvars[0]][2])), True)
-                    model.PBM[p].PSD = np.array(columns[PSDvars[1]], dtype='float')
-                    model.PBM[p].PSDsize = np.array(columns[PSDvars[2]], dtype='float')
-                    model.eqAspectRatio[p] = np.array(columns[PSDvars[3]], dtype='float')
-                    model.PBM[p].PSDbounds = np.array(columns[PSDvars[4]], dtype='float')
-
-                restOfVariables = ['time', 'xComp', 'Rcrit', 'Gcrit', 'Rad', 'avgR', 'avgAR', 'betaFrac', 'nucRate', 'precipitateDensity', 'dGs', 'xEqAlpha', 'xEqBeta', 'additionalOutputs']
-                restOfColumns = {v: [] for v in restOfVariables}
-                additionalFunctionNames = []
-                for d in columns:
-                    if d not in setupVars:
-                        if d == 'time':
-                            restOfColumns[d] = np.array(columns[d], dtype='float')
-                        elif d == 'xComp':
-                            if model.numberOfElements == 1:
-                                restOfColumns[d] = np.array(columns[d], dtype='float')
-                            else:
-                                restOfColumns['xComp'].append(columns[d], dtype='float')
-                        else:
-                            selectedVar = ''
-                            for r in restOfVariables:
-                                if r in d:
-                                    selectedVar = r
-                            if selectedVar == 'additionalOutputs':
-                                additionalFunctionNames.append(d[18:])
-                            restOfColumns[selectedVar].append(np.array(columns[d], dtype='float'))
-                for d in restOfColumns:
-                    restOfColumns[d] = np.array(restOfColumns[d])
-                    setattr(model, d, restOfColumns[d])
-
-                #For multicomponent systems, adjust as necessary such that number of elements will be the last axis
-                if model.numberOfElements > 1:
-                    model.xComp = model.xComp.T
-                    if len(model.phases) == 1:
-                        model.xEqAlpha = np.expand_dims(model.xEqAlpha, 0)
-                        model.xEqBeta = np.expand_dims(model.xEqBeta, 0)
-                    else:
-                        model.xEqAlpha = np.reshape(model.xEqAlpha, ((len(model.phases), model.numberOfElements, len(model.time))))
-                        model.xEqBeta = np.reshape(model.xEqBeta, ((len(model.phases), model.numberOfElements, len(model.time))))
-                    model.xEqAlpha = np.transpose(model.xEqAlpha, (0, 2, 1))
-                    model.xEqBeta = np.transpose(model.xEqBeta, (0, 2, 1))
-
-                #If additional outputs exists, then reshape array to (phase, iterations, functions)
-                if len(additionalFunctionNames) > 0:
-                    numberOfFunctions = int(len(additionalFunctionNames) / len(model.phases))
-                    model.additionalOutputs = np.reshape(model.additionalOutputs, (len(model.phases), numberOfFunctions, len(model.time)))
-                    model.additionalOutputs = np.transpose(model.additionalOutputs, (0, 2, 1))
-                    model.additionalFunctionNames = []
-                    for i in range(numberOfFunctions):
-                        model.additionalFunctionNames.append(additionalFunctionNames[i][len(model.phases[0])+1:])
-                    model.additionalFunctionNames = np.array(model.additionalFunctionNames)
-
+        data = np.load(filename)
+        model = PrecipitateModel(data['phases'], data['elements'])
+        model._loadData(data)
         return model
 
-    def _divideTimestep(self, i, dt):
-        '''
-        Divides timestep at iteration i
-        '''
-        super()._divideTimestep(i, dt)
-
-        if len(self.additionalFunctions) > 0:
-            self.additionalOutputs = np.append(self.additionalOutputs, np.zeros((len(self.phases), 1, len(self.additionalFunctions))), axis=1)
+    def _loadExtraVariables(self, data):
+        for p in range(len(self.phases)):
+            PBMdata = data['PBM_data_' + self.phases[p]]
+            psd = data['PBM_PSD_' + self.phases[p]]
+            bounds = data['PBM_bounds_' + self.phases[p]]
+            size = data['PBM_size_' + self.phases[p]]
+            eqAR = data['eqAspectRatio_' + self.phases[p]]
+            self.PBM[p] = PopulationBalanceModel(PBMdata[0], PBMdata[1], int(PBMdata[2]))
+            self.PBM[p].PSD = psd
+            self.PBM[p].PSDsize = size
+            self.PBM[p].PSDbounds = bounds
+            self.eqAspectRatio[p] = eqAR
 
     def setPBMParameters(self, cMin = 1e-10, cMax = 1e-9, bins = 150, minBins = 100, maxBins = 200, adaptive = True, phase = None):
         '''
         Sets population balance model parameters for each phase
 
         Parameters
         ----------
@@ -298,83 +105,71 @@
                 self.PBM[p] = PopulationBalanceModel(cMin, cMax, bins, minBins, maxBins)
                 self.PBM[p].setAdaptiveBinSize(adaptive)
         else:
             index = self.phaseIndex(phase)
             self.PBM[index] = PopulationBalanceModel(cMin, cMax, bins, minBins, maxBins)
             self.PBM[index].setAdaptiveBinSize(adaptive)
 
-    def loadParticleSizeDistribution(self, data, phase = None):
+    def setPSDrecording(self, record = True, phase = 'all'):
         '''
-        Loads particle size distribution for specified phase
+        Sets recording parameters for PSD of specified phase
 
         Parameters
         ----------
-        data : array
-            Array of data containing precipitate sizes
+        record : bool (optional)
+            Whether to record PSD, defaults to True
         phase : str (optional)
-            Phase to consider (defaults to first precipitate in list)
+            Precipitate phase to record for
+            Defaults to 'all', which will apply to all precipitate phases
         '''
-        index = self.phaseIndex(phase)
-        self.PBM[index].LoadDistribution(data)
+        if phase is None or phase == 'all':
+            for p in self.phases:
+                index = self.phaseIndex(p)
+                self.PBM[index].setRecording(record)
+        else:
+            index = self.phaseIndex(phase)
+            self.PBM[index].setRecording(record)
 
-    def addAdditionalOutput(self, name, f):
+    def saveRecordedPSD(self, filename, compressed = True, phase = 'all'):
         '''
-        Creates output based off PSD
+        Saves recorded PSD in npz format
 
         Parameters
         ----------
-        name : str
-            Name of the function
-        f : function
-            Takes in model, phase index and iteration index and returns a value
-        '''
-        if name in self.additionalFunctionNames:
-            i = 1
-            name = name + '_{}'.format(i)
-            while name in self.additionalFunctionNames:
-                i += 1
-                name = name[:-2]
-                name = name + '_{}'.format(i)
-            print('Warning: Function \'{}\' has already been set, this function will be stored as \'{}\''.format(name[:-2], name))
-            
-        self.additionalFunctions.append(f)
-        self.additionalFunctionNames = np.append(self.additionalFunctionNames, name)
-
-    def _setupAdditionalOutputs(self):
-        '''
-        Function to setup PSD output arrays, will be used in setup and reset functions
-        '''
-        #Resets PSD outputs
-        if len(self.additionalFunctions) > 0:
-            self.additionalOutputs = np.zeros((len(self.phases), self.steps, len(self.additionalFunctions)))
-
-    def _calculateAdditionalOutputs(self, i):
-        '''
-        Calculates additional PSD functions
+        filename : str
+            File name to save to
+            Note: the phase name will be added to the filename if all phases are being saved
+        compressed : bool (optional)
+            Whether to save in compressed npz format
+            Defualts to True
+        phase : str (optional)
+            Phase to save PSD for
+            Defaults to 'all', which will save a file for each phase
         '''
-        for f in range(len(self.additionalFunctions)):
-            for p in range(len(self.phases)):
-                self.additionalOutputs[p, i, f] = self.additionalFunctions[f](self, p, i)
+        if phase is None or phase == 'all':
+            for p in self.phases:
+                index = self.phaseIndex(p)
+                self.PBM[index].saveRecordedPSD(filename + '_' + p, compressed)
+        else:
+            index = self.phaseIndex(phase)
+            self.PBM[index].saveRecordedPSD(filename, compressed)
 
-    def getAdditionalOutput(self, name):
+    def loadParticleSizeDistribution(self, data, phase = None):
         '''
-        Gets additional output by name
+        Loads particle size distribution for specified phase
 
         Parameters
         ----------
-        name : str
-            Name of function used for the additional output
-
-        Returns
-        -------
-        (p, N) array for the output for each phase
-        '''
-        if name in self.additionalFunctionNames:
-            index, = np.where(self.additionalFunctionNames == name)
-            return self.additionalOutputs[:, :, index[0]]
+        data : array
+            Array of data containing precipitate sizes
+        phase : str (optional)
+            Phase to consider (defaults to first precipitate in list)
+        '''
+        index = self.phaseIndex(phase)
+        self.PBM[index].LoadDistribution(data)
 
     def particleRadius(self, phase = None):
         '''
         Returns PSD bounds of given phase
 
         Parameters
         ----------
@@ -408,64 +203,73 @@
         Parameters
         ----------
         phase : str (optional)
             Phase to consider (defaults to first precipitate in list)
         '''
         index = self.phaseIndex(phase)
         return self.PBM[index].PSD
- 
-    def createLookup(self, i = 0):
+    
+    def createLookup(self):
         '''
         This creates a lookup table mapping the particle size classes to the interfacial composition
         '''
         #RdrivingForceIndex will find the index of the largest particle size class where the precipitate is unstable
         #This is determined by the interfacial composition function, where it should return -1 or None
         #All compositions from the PSD bounds will be set to the compositions just above RdrivingForceLimit
         #This is just to allow for particles to dissolve instead of pile up in the smallest bin
         self.RdrivingForceIndex = np.zeros(len(self.phases), dtype=np.int32)
 
         #Keep as separate arrays so that number of PSD classes can change within precipitate phases
         self.PSDXalpha = []
         self.PSDXbeta = []
         
+        xEqAlpha = np.zeros((1, len(self.phases), self.numberOfElements))
+        xEqBeta = np.zeros((1, len(self.phases), self.numberOfElements))
+        T = self._currY[self.TEMPERATURE][0]
         for p in range(len(self.phases)):
             #Interfacial compositions at equilibrium (planar interface)
-            self.xEqAlpha[p,i], self.xEqBeta[p,i] = self.interfacialComposition[p](self.T[i], 0)
-            if self.xEqAlpha[p,i] == -1 or self.xEqAlpha[p,i] is None:
-                self.xEqAlpha[p,i] = 0
-                self.xEqBeta[p,i] = 0
+            xAResult, xBResult = self.interfacialComposition[p](T, 0)
+            if xAResult == -1 or xAResult is None:
+                xEqAlpha[0,p,0] = 0
+                xEqBeta[0,p,0] = 0
+            else:
+                xEqAlpha[0,p,0] = xAResult
+                xEqBeta[0,p,0] = xBResult
 
             #Interfacial compositions at each size class in PSD
-            self.PSDXalpha.append(np.zeros(self.PBM[p].bins + 1))
-            self.PSDXbeta.append(np.zeros(self.PBM[p].bins + 1))
+            self.PSDXalpha.append(np.zeros((self.PBM[p].bins + 1, 1)))
+            self.PSDXbeta.append(np.zeros((self.PBM[p].bins + 1, 1)))
 
-            self.PSDXalpha[p], self.PSDXbeta[p] = self.interfacialComposition[p](self.T[i], self.particleGibbs(self.PBM[p].PSDbounds, self.phases[p]))
-            self.RdrivingForceIndex[p] = np.argmax(self.PSDXalpha[p] != -1)-1
+            self.PSDXalpha[p][:,0], self.PSDXbeta[p][:,0] = self.interfacialComposition[p](T, self.particleGibbs(self.PBM[p].PSDbounds, self.phases[p]))
+            self.RdrivingForceIndex[p] = np.argmax(self.PSDXalpha[p][:,0] != -1)-1
             self.RdrivingForceIndex[p] = 0 if self.RdrivingForceIndex[p] < 0 else self.RdrivingForceIndex[p]
             self.RdrivingForceLimit[p] = self.PBM[p].PSDbounds[self.RdrivingForceIndex[p]]
 
             #Sets particle radii smaller than driving force limit to driving force limit composition
             #If RdrivingForceIndex is at the end of the PSDX arrays, then no precipitate in the size classes of the PSD is stable
             #This can occur in non-isothermal situations where the temperature gets too high
-            if self.RdrivingForceIndex[p]+1 < len(self.PSDXalpha[p]):
-                self.PSDXalpha[p][:self.RdrivingForceIndex[p]+1] = self.PSDXalpha[p][self.RdrivingForceIndex[p]+1]
-                self.PSDXbeta[p][:self.RdrivingForceIndex[p]+1] = self.PSDXbeta[p][self.RdrivingForceIndex[p]+1]
+            if self.RdrivingForceIndex[p]+1 < len(self.PSDXalpha[p][:,0]):
+                self.PSDXalpha[p][:self.RdrivingForceIndex[p]+1,0] = self.PSDXalpha[p][self.RdrivingForceIndex[p]+1,0]
+                self.PSDXbeta[p][:self.RdrivingForceIndex[p]+1,0] = self.PSDXbeta[p][self.RdrivingForceIndex[p]+1,0]
             else:
-                self.PSDXalpha[p] = np.zeros(self.PBM[p].bins + 1)
-                self.PSDXbeta[p] = np.zeros(self.PBM[p].bins + 1)
+                self.PSDXalpha[p] = np.zeros((self.PBM[p].bins + 1,1))
+                self.PSDXbeta[p] = np.zeros((self.PBM[p].bins + 1,1))
+
+        return xEqAlpha, xEqBeta
             
     def setup(self):
         '''
         Sets up additional variables in addition to PrecipitateBase
 
         Sets up additional outputs, population balance models, equilibrium aspect ratio and equilibrium compositions
         '''
-        super().setup()
+        if self._isSetup:
+            return
 
-        self._setupAdditionalOutputs()
+        super().setup()
 
         #Equilibrium aspect ratio and PBM setup
         #If calculateAspectRatio is True, then use strain energy to calculate aspect ratio for each size class in PSD
         #Else, then use aspect ratio defined in shape factors
         self.eqAspectRatio = [None for p in range(len(self.phases))]
         for p in range(len(self.phases)):
             self.PBM[p].reset()
@@ -473,473 +277,457 @@
             if self.calculateAspectRatio[p]:
                 self.eqAspectRatio[p] = self.strainEnergy[p].eqAR_bySearch(self.PBM[p].PSDbounds, self.gamma[p], self.shapeFactors[p])
                 arFunc = lambda R, p1=p : self._interpolateAspectRatio(R, p1)
                 self.shapeFactors[p].setAspectRatio(arFunc)
             else:
                 self.eqAspectRatio[p] = self.shapeFactors[p].aspectRatio(self.PBM[p].PSDbounds)
 
-        #Only create lookup table for binary system
+        self._currY = [np.array([self.varList[i][self.n]]) for i in range(self.NUM_TERMS)]
+        self._currY[self.TIME] = np.array([self.time[self.n]])
+        self._currY[self.TEMPERATURE] = np.array([self.getTemperature(self.time[self.n])])
+        
+        #Setup interfacial composition
         if self.numberOfElements == 1:
-            self.createLookup(0)
+            self.xEqAlpha[self.n], self.xEqBeta[self.n] = self.createLookup()
         else:
             self.PSDXalpha = [None for p in range(len(self.phases))]
             self.PSDXbeta = [None for p in range(len(self.phases))]
 
             #Set first index of eq composition
             for p in range(len(self.phases)):
                 #Use arbitrary dg, R and gE since only the eq compositions are needed here
-                _, _, _, xEqAlpha, xEqBeta = self.interfacialComposition[p](self.xComp[0], self.T[0], 0, 1, 0)
+                _, _, _, xEqAlpha, xEqBeta = self.interfacialComposition[p](self.xComp[self.n], self.temperature[self.n], 0, 1, 0)
                 if xEqAlpha is not None:
-                    self.xEqAlpha[p,0] = xEqAlpha
-                    self.xEqBeta[p,0] = xEqBeta
-
+                    self.xEqAlpha[self.n,p] = xEqAlpha
+                    self.xEqBeta[self.n,p] = xEqBeta
+        
+        x = [self.PBM[p].PSD for p in range(len(self.phases))]
+        self._calcDrivingForce(self.time[self.n], x)
+        self._growthRate()
+        self._calcNucleationRate(self.time[self.n], x)
+        for i in range(self.NUM_TERMS):
+            self.varList[i][self.n] = self._currY[i][0]
+    
     def _interpolateAspectRatio(self, R, p):
         '''
         Linear interpolation between self.eqAspectRatio and self.PBM[p].PSDbounds
 
         Parameters
         ----------
         R : float
             Equivalent spherical radius
         p : int
             Phase index
         '''
         return np.interp(R, self.PBM[p].PSDbounds, self.eqAspectRatio[p])
 
-    def _iterate(self, i):
-        '''
-        Iteration function
-        '''
-        #Nucleation and growth rate are independent of time increment
-        #They can be calculated first and used to determine the time increment for numerical stability
-        self._nucleate(i)
-        self._setNucleateRadius(i)
-        self._growthRate(i)
-        self._timeIncrementCheck(i)
-
-        #Backup variables in case size classes on PSD changes
-        self.growthBackup = copy.copy(self.growth)
-        self.PSDXalphaBackup = copy.copy(self.PSDXalpha)
-        self.PSDXbetaBackup = copy.copy(self.PSDXbeta)
-        self.eqAspectRatioBackup = copy.copy(self.eqAspectRatio)
-        self.RdrivingForceIndexBackup = copy.copy(self.RdrivingForceIndex)
-        self.RdrivingForceLimitBackup = copy.copy(self.RdrivingForceLimit)
-
-        postDTCheck = False
-        while not postDTCheck:
-            dt = self.time[i] - self.time[i-1]
-            self._calculatePSD(i, dt)
-            self._massBalance(i)
-
-            if i < self.steps - 1:
-                postDTCheck = self._postTimeIncrementCheck(i)
-            else:
-                postDTCheck = True
-
-        #Calculate additional PSD function
-        self._calculateAdditionalOutputs(i)
-
-    def _noCheckDT(self, i):
+    def getDt(self, dXdt):
         '''
-        Function if adaptive time stepping is not used
-        Will calculated growth rate since it is done in the _checkDT function (not a good way of doing this, but works for now)
-        '''
-        return
-
-    def _checkDT(self, i):
-        '''
-        Checks max growth rate and updates dt correspondingly
-        '''
-        dt = self._calculateDT(i-1, self.maxDTFraction)
-        dtAll = [dt]
-
+        The following checks are made
+            1) change in number of particles moving between bins
+                This is controlled by the implementation in PopulationBalanceModel,
+                but essentially limits the number of particles moving between bins
+            2) change in nucleation rate
+                Time will be proportional to the 1/log(previous nuc rate / new nuc rate)
+            3) change in temperature
+                Limits how fast temperature can change
+            4) change in critical radius
+                Proportional to a percent change in critical radius
+            5) estimated change in volume fraction
+                Estimates the change in volume fraction from the nucleation rate and nucleation radius
+        '''
+        #Start test dt at 0.01 or previous dt
+        i = self.n
+        dtPrev = 0.01 if self.n == 0 else self.time[i] - self.time[i-1]
+        #Try to slowly increase the time step
+        #  Precipitation kinetics is more on a log scale than linear (unless temperature changes are involve)
+        #  Thus, we can get away with increasing the time step over time assuming that kinetics are slowing down
+        #  Plus, unlike the single phase diffusion module, there's no form way to define a good time step apart from the checks here
+        dtPropose = (1 + self.dtScale) * dtPrev
+        dtMax = self.finalTime - self.time[i]
+        
+        dtAll = [dtMax]
         if self.checkPSD:
-            if self.T[i] == self.T[i-1]:
-                dtPBM = [self.PBM[p].getDTEuler(dt, self.growth[p], self.maxDissolution, self.RdrivingForceIndex[p]) for p in range(len(self.phases))]
-            else:
-                dtPBM = [dt]
-            dt = np.amin(np.concatenate(([dt], dtPBM)))
-            dtAll.append(dt)
-
-        if i > 1:
-            dtPrev = self.time[i-1] - self.time[i-2]
-        else:
-            dtPrev = dt
-
-        #Nucleation rate constraint
+            dtPBM = [dtMax]
+            if i > 0 and self.temperature[i] == self.temperature[i-1]:
+                dtPBM += [self.PBM[p].getDTEuler(dtMax, self.growth[p], self.dissolutionIndex[p]) for p in range(len(self.phases))]
+            dtPBM = np.amin(dtPBM)
+            dtAll.append(dtPBM)
+        
         if self.checkNucleation:
-            dtNuc = dt * np.ones(len(self.phases)+1)
-            for p in range(len(self.phases)):
-                if self.nucRate[p,i] > self.minNucleationRate and self.nucRate[p,i-1] > self.minNucleationRate and self.nucRate[p,i-1] != self.nucRate[p,i]:
-                    dtNuc[p] = self.maxNucleationRateChange * dtPrev / np.abs(np.log10(self.nucRate[p,i-1] / self.nucRate[p,i]))
-            dt = np.amin(dtNuc)
-            dtAll.append(dt)
+            dtNuc = dtMax * np.ones(len(self.phases))
+            if i > 0:
+                nRateCurr = self.nucRate[i]
+                nRatePrev = self.nucRate[i-1]
+                for p in range(len(self.phases)):
+                    if nRateCurr[p] > self.minNucleationRate and nRatePrev[p] > self.minNucleationRate and nRatePrev[p] != nRateCurr[p]:
+                        dtNuc[p] = self.maxNucleationRateChange * dtPrev / np.abs(np.log10(nRatePrev[p] / nRateCurr[p]))
+            else:
+                for p in range(len(self.phases)):
+                    if self.nucRate[i,p] * dtPrev > 1e5:
+                        dtNuc[p] = 1e5 / self.nucRate[i,p]
+            dtNuc = np.amin(dtNuc)
+            dtAll.append(dtNuc)
 
         #Temperature change constraint
-        if self.checkTemperature:
-            Tchange = self.T[i] - self.T[i-1]
-            dtTemp = dt
+        if self.checkTemperature and i > 0:
+            Tchange = self.temperature[i] - self.temperature[i-1]
+            dtTemp = dtMax
             if Tchange > self.maxNonIsothermalDT:
-                dtTemp = self.maxNonIsothermalDT * (self.time[i] - self.time[i-1]) / Tchange
-                dt = np.amin([dt, dtTemp])
+                dtTemp = self.maxNonIsothermalDT * dtPrev / Tchange
+            dtAll.append(dtTemp)
 
-        if self.checkRcrit:
-            dtRad = dt * np.ones(len(self.phases)+1)
-            if not all((self.Rcrit[:,i-1] == 0) & (self.Rcrit[:,i] - self.Rcrit[:,i-1] == 0) & (self.dGs[:,i] <= 0)):
-                indices = (self.Rcrit[:,i-1] > 0) & (self.Rcrit[:,i] - self.Rcrit[:,i-1] != 0) & (self.dGs[:,i] > 0)
-                dtRad[:-1][indices] = self.maxRcritChange * dtPrev / np.abs((self.Rcrit[:,i][indices] - self.Rcrit[:,i-1][indices]) / self.Rcrit[:,i-1][indices])
-            dt = np.amin(dtRad)
-            dtAll.append(dt)
+        if self.checkRcrit and i > 0:
+            dtRad = dtMax * np.ones(len(self.phases))
+            if not all((self.Rcrit[i-1,:] == 0) & (self.Rcrit[i,:] - self.Rcrit[i-1,:] == 0) & (self.dGs[i,:] <= 0)):
+                indices = (self.Rcrit[i-1,:] > 0) & (self.Rcrit[i,:] - self.Rcrit[i-1,:] != 0) & (self.dGs[i,:] > 0)
+                dtRad[indices] = self.maxRcritChange * dtPrev / np.abs((self.Rcrit[i,:][indices] - self.Rcrit[i-1,:][indices]) / self.Rcrit[i-1,:][indices])
+            dtRad = np.amin(dtRad)
+            dtAll.append(dtRad)
 
-        if self.checkVolumePre or self.checkCompositionPre:
+        if self.checkVolumePre:
             dV = np.zeros(len(self.phases))
             for p in range(len(self.phases)):
                 #Calculate estimate volume change based off growth rate and nucleated particles
                 #TODO: account for non-spherical precipitates
                 dVi = self.PBM[p].PSD * self.PBM[p].PSDsize**2 * 0.5 * (self.growth[p][1:] + self.growth[p][:-1])
                 dVi[dVi < 0] = 0
-                dV = self.VmAlpha / self.VmBeta[p] * (self.GB[p].areaFactor * np.sum(dVi) + self.GB[p].volumeFactor * self.nucRate[p,i] * self.Rad[p,i]**3)
-
-            if self.checkVolumePre:
-                dtVol = dt * np.ones(len(self.phases) + 1)
-                for p in range(len(self.phases)):
-                    if dV != 0:
-                        dtVol[p] = self.maxVolumeChange / (2 * np.abs(dV))
-                #if not all((self.Rad[:,i]**3*self.nucRate[:,i] > 1e-30)):
-                #    indices = (self.Rad[:,i]**3*self.nucRate[:,i] > 1e-30)
-                #    dtVol[:-1][indices] = self.maxVolumeChange / (10 * (4*np.pi*self.Rad[:,i][indices]**3*self.nucRate[:,i][indices]/3))
-                dt = np.amin(dtVol)
-                dtAll.append(dt)
-
-            if self.checkCompositionPre:
-                dtComp = dt * np.ones(self.numberOfElements + 1)
-                fvsum = np.sum(self.betaFrac[:,i-1])
-                xbavg = np.zeros(self.numberOfElements)
-                if self.numberOfElements == 1:
-                    xbavg[0] = 0 if fvsum == 0 else (self.xComp[0] - self.xComp[i-1] * (1 - fvsum)) / fvsum
-                    dxadt = (self.xComp[i-1] - xbavg) * np.sum(dV) / (1 - fvsum)
-                else:
-                    for e in range(self.numberOfElements):
-                        xbavg[e] = 0 if fvsum == 0 else (self.xComp[0,e] - self.xComp[i-1,e] * (1 - fvsum)) / fvsum
-                    dxadt = (self.xComp[i-1,:] - xbavg) * np.sum(dV) / (1 - fvsum)
-                dxadt[dxadt == 0] = self.maxCompositionChange / (2 * dt)
-                dtComp[:self.numberOfElements] = self.maxCompositionChange / (2 * dxadt)
-                    
-                dt = np.amin(dtComp)
-                dtAll.append(dt)
+                dV = self.VmAlpha / self.VmBeta[p] * (self.GB[p].areaFactor * np.sum(dVi) + self.GB[p].volumeFactor * self.nucRate[i,p] * self.Rad[i,p]**3)
 
-        #Minimum dt is the lower of the minimum allowed time increment or the time to the next pre-defined increment
-        minDT = self._calculateDT(i-1, self.minDTFraction)
-        dt = np.amax([dt, minDT])
-
-        #Override time increment with the predefined time steps
-        #This prevents the next time increment from becoming 0 or negative
-        dt = np.amin([dt, self.time[i] - self.time[i-1]])
-        
-        if dt < self.time[i] - self.time[i-1]:
-            #print(dtAll)
-            self._divideTimestep(i, dt)
+            dtVol = dtMax * np.ones(len(self.phases))
+            for p in range(len(self.phases)):
+                if dV != 0:
+                    dtVol[p] = self.maxVolumeChange / (2 * np.abs(dV))
+            dtVol = np.amin(dtVol)
+            dtAll.append(dtVol)
+
+        dt = np.amin(dtAll)
+        #If all time checks pass, then go back to previous time step and increase it slowly
+        #   This is so we don't step at the maximum possible time
+        if dt == dtMax:
+            dt = dtPropose
 
-    def _noPostCheckDT(self, i):
-        '''
-        Function if no adaptive time stepping is used, no need to do anything in this function
+        return dt
+    
+    def _processX(self, x):
         '''
-        return True
-
-    def _postCheckDT(self, i):
+        Quick check to make sure particles below the thresholds are 0
+            RdrivingForceIndex - only for binary, where energy from the Gibbs-Thompson effect is high enough
+                that the free energy of the precipitate is above the free energy surface of the matrix phase
+                and equilibrium cannot be calculated
+            minRadius - minimum radius to be considered a precipitate
         '''
-        CURRENTLY UNUSED AND MAY BE REMOVED LATER
-
-        If adaptive time step is used, this checks new values at iteration i
-        and compares with simulation contraints
-
-        If contraints are not met, then remove current values and divide time step
+        for p in range(len(self.phases)):
+            x[p][:self.RdrivingForceIndex[p]+1] = 0
+            x[p][self.PBM[p].PSDsize < self.minRadius] = 0
+        return
+    
+    def _calcNucleationRate(self, t, x):
         '''
-        #Only perform checks in non-isothermal situations
-        if np.abs(self.T[i] - self.T[i-1]) > 1:
-            return True
-
-        #Composition and volume change are checks in absolute changes
-        #This prevents any unneccessary reduction in time increments for dilute solutions, or
-        #if there is a long incubation time until nucleations starts occuring
-
-        if self.checkVolumePost:
-            volChange = np.abs(self.betaFrac[:,i] - self.betaFrac[:,i-1])
-            #If current volume fraction is 0, then ignore (either precipitation has not occured or precipitates has dissolved)
-            volChange[self.betaFrac[:,i] == 0] = 0
-            volCheck = np.amax(volChange) < self.maxVolumeChange
-        else:
-            volCheck = True
-
-        if self.checkComposition:
-            if self.numberOfElements == 1:
-                compCheck = (np.abs(self.xComp[i] - self.xComp[i-1]) < self.maxCompositionChange) & (self.xComp[i] > 0)
-            else:
-                compCheck = (np.amax(np.abs(self.xComp[i,:] - self.xComp[i-1,:])) < self.maxCompositionChange) & (np.amin(self.xComp[i,:] > self.minComposition))
-        else:
-            compCheck = True
+        The _calcNucleationRate function in KWNBase calculates the nucleation rate as the
+            probability that a site can form a nucleate that will continue to grow
 
-        checks = [volCheck, compCheck]
+        To convert this probability to an actual nucleation rate, we multiply by the amount
+            of available nucleation sites
 
-        #If any test fails, then reset iteration and divide time increment
-        if not all(checks):
-            dt = (self.time[i] - self.time[i-1]) / 2
-            minDT = self._calculateDT(i-1, self.minDTFraction)
-
-            #If proposed time increment is smaller than the minimum allowed increment, then skip the checks
-            if dt < minDT:
-                return True
-
-            #Only revert changes to variables that aren't stored per iteration
-            #Variables related to nucleation are not dependent on the time increment
-            #Variables related to the particle size distribution (composition, volume fraction, etc)
-            # will be overridden if the time increment changes            
-            self.prevFConc[0] = copy.copy(self.prevFConc[1])
-
-            for p in range(len(self.phases)):
-                self.PBM[p].revert()
-            self.growth = copy.copy(self.growthBackup)
-            self.PSDXalpha = copy.copy(self.PSDXalphaBackup)
-            self.PSDXbeta = copy.copy(self.PSDXbetaBackup)
-            self.eqAspectRatio = copy.copy(self.eqAspectRatioBackup)
-            self.RdrivingForceIndex = copy.copy(self.RdrivingForceIndexBackup)
-            self.RdrivingForceLimit = copy.copy(self.RdrivingForceLimitBackup)
-
-            self._divideTimestep(i, dt)
-
-            return False
-        else:
-            return True
-    
-    def _nucleate(self, i):
-        '''
-        Calculates the nucleation rate at current timestep
-        This can be done before the initial time increment checks are performed
+        The number of available sites is determined by:
+            Available sites = All sites - used up sites + sites on parent precipitates
+            The used up sites depends on the type of nucleation
+                Bulk and grain corners - used sites = number of current precipitates
+                Dislocation and grain edges - number of sites filled along the edges (assumes average radius of precipitates)
+                Grain boundaries - number of sites filled along the faces (assumes average cross sectional area of precipitates)
         '''
+        super()._calcNucleationRate(t, x)
         for p in range(len(self.phases)):
             #If parent phases exists, then calculate the number of potential nucleation sites on the parent phase
             #This is the number of lattice sites on the total surface area of the parent precipitate
-            nucleationSites = np.sum([4 * np.pi * self.PBM[p2].SecondMoment() * (self.avo / self.VmBeta[p2])**(2/3) for p2 in self.parentPhases[p]])
+            nucleationSites = np.sum([4 * np.pi * self.PBM[p2].SecondMomentFromN(x[p2]) * (self.avo / self.VmBeta[p2])**(2/3) for p2 in self.parentPhases[p]])
 
             if self.GB[p].nucleationSiteType == GBFactors.BULK:
                 #bulkPrec = np.sum([self.GB[p2].volumeFactor * self.PBM[p2].ThirdMoment() for p2 in range(len(self.phases)) if self.GB[p2].nucleationSiteType == GBFactors.BULK])
                 #nucleationSites += self.bulkN0 - bulkPrec * (self.avo / self.VmAlpha)
-                bulkPrec = np.sum([self.PBM[p2].ZeroMoment() for p2 in range(len(self.phases)) if self.GB[p2].nucleationSiteType == GBFactors.BULK])
+                bulkPrec = np.sum([self.PBM[p2].ZeroMomentFromN(x[p2]) for p2 in range(len(self.phases)) if self.GB[p2].nucleationSiteType == GBFactors.BULK])
                 nucleationSites += self.bulkN0 - bulkPrec
             elif self.GB[p].nucleationSiteType == GBFactors.DISLOCATION:
-                bulkPrec = np.sum([self.PBM[p2].FirstMoment() for p2 in range(len(self.phases)) if self.GB[p2].nucleationSiteType == GBFactors.DISLOCATION])
+                bulkPrec = np.sum([self.PBM[p2].FirstMomentFromN(x[p2]) for p2 in range(len(self.phases)) if self.GB[p2].nucleationSiteType == GBFactors.DISLOCATION])
                 nucleationSites += self.dislocationN0 - bulkPrec * (self.avo / self.VmAlpha)**(1/3)
             elif self.GB[p].nucleationSiteType == GBFactors.GRAIN_BOUNDARIES:
-                boundPrec = np.sum([self.GB[p2].gbRemoval * self.PBM[p2].SecondMoment() for p2 in range(len(self.phases)) if self.GB[p2].nucleationSiteType == GBFactors.GRAIN_BOUNDARIES])
+                boundPrec = np.sum([self.GB[p2].gbRemoval * self.PBM[p2].SecondMomentFromN(x[p2]) for p2 in range(len(self.phases)) if self.GB[p2].nucleationSiteType == GBFactors.GRAIN_BOUNDARIES])
                 nucleationSites += self.GBareaN0 - boundPrec * (self.avo / self.VmAlpha)**(2/3)
             elif self.GB[p].nucleationSiteType == GBFactors.GRAIN_EDGES:
-                edgePrec = np.sum([np.sqrt(1 - self.GB[p2].GBk**2) * self.PBM[p2].FirstMoment() for p2 in range(len(self.phases)) if self.GB[p2].nucleationSiteType == GBFactors.GRAIN_EDGES])
+                edgePrec = np.sum([np.sqrt(1 - self.GB[p2].GBk**2) * self.PBM[p2].FirstMomentFromN(x[p2]) for p2 in range(len(self.phases)) if self.GB[p2].nucleationSiteType == GBFactors.GRAIN_EDGES])
                 nucleationSites += self.GBedgeN0 - edgePrec * (self.avo / self.VmAlpha)**(1/3)
             elif self.GB[p].nucleationSiteType == GBFactors.GRAIN_CORNERS:
-                cornerPrec = np.sum([self.PBM[p2].ZeroMoment() for p2 in range(len(self.phases)) if self.GB[p2].nucleationSiteType == GBFactors.GRAIN_CORNERS])
+                cornerPrec = np.sum([self.PBM[p2].ZeroMomentFromN(x[p2]) for p2 in range(len(self.phases)) if self.GB[p2].nucleationSiteType == GBFactors.GRAIN_CORNERS])
                 nucleationSites += self.GBcornerN0 - cornerPrec
                
             if nucleationSites < 0:
                 nucleationSites = 0
-            self.nucRate[p, i] = nucleationSites * self._nucleationRate(p, i)
-
-    def _calculatePSD(self, i, dt):
+            self._currY[self.NUC_RATE][0,p] *= nucleationSites
+    
+    def _calcMassBalance(self, t, x):
         '''
-        Updates the PSD using the population balance model from coarsening and nucleation rate
-        This also updates the fraction of precipitates, matrix composition and average radius
+        Mass balance to find matrix composition with new particle size distribution
+
+        This also includes: volume fraction, precipitate density, average radius, average aspect ratio and sum of precipitate composition
         '''
+        fBeta = np.zeros((1,len(self.phases)))
+        fConc = np.zeros((1, len(self.phases),self.numberOfElements))
+        precDens = np.zeros((1,len(self.phases)))
+        avgR = np.zeros((1,len(self.phases)))
+        avgAR = np.zeros((1,len(self.phases)))
+        xComp = np.zeros((1,self.numberOfElements))
+        
         for p in range(len(self.phases)):
-            #Backup PSD for time increment checks
-            #Also backup PSDXbeta for precipitate composition with no diffusion
-            self.PBM[p].createBackup()
-            self._prevPSDXbeta = copy.copy(self.PSDXbeta)
-
-            change1, newIndices = self.PBM[p].UpdateEuler(dt, self.growth[p])
-            change2 = self.PBM[p].Nucleate(self.nucRate[p, i] * dt, self.Rad[p, i])
-            if change1 or change2:
-                #Add aspect ratio, do this before growth rate and interfacial composition since those are dependent on this
-                if self.calculateAspectRatio[p]:
-                    self.eqAspectRatio[p] = self.strainEnergy[p].eqAR_bySearch(self.PBM[p].PSDbounds, self.gamma[p], self.shapeFactors[p])
-                else:
-                    self.eqAspectRatio[p] = self.shapeFactors[p].aspectRatio(self.PBM[p].PSDbounds)
-
-                self.growth[p] = np.zeros(len(self.PBM[p].PSDbounds))
-                if self.numberOfElements == 1:
-                    if newIndices is None:
-                        #This is very slow to do
-                        self.createLookup(i)
-                    else:
-                        self.PSDXalpha[p] = np.concatenate((self.PSDXalpha[p], np.zeros(self.PBM[p].bins+1 - len(self.PSDXalpha[p]))))
-                        self.PSDXbeta[p] = np.concatenate((self.PSDXbeta[p], np.zeros(self.PBM[p].bins+1 - len(self.PSDXbeta[p]))))
-                        self.PSDXalpha[p][newIndices:], self.PSDXbeta[p][newIndices:] = self.interfacialComposition[p](self.T[i-1], self.particleGibbs(self.PBM[p].PSDbounds[newIndices:], self.phases[p]))
-                    self.growth[p] = self._singleGrowthBinary(i, p)
-                else:
-                    self.growth[p] = self._singleGrowthMulti(i, p)
+            volRatio = self.VmAlpha / self.VmBeta[p]
+            Ntot = self.PBM[p].ZeroMomentFromN(x[p])
+            #If no precipitates, then avgR, avgAR, precDens, fConc and fBeta for phase p is all 0
+            if Ntot == 0:
+                continue
+            RadSum = self.PBM[p].MomentFromN(x[p], 1)
+            ARsum = self.PBM[p].WeightedMomentFromN(x[p], 0, self.shapeFactors[p].aspectRatio(self.PBM[p].PSDsize))
+            fBeta[0,p] = np.amin([volRatio * self.GB[p].volumeFactor * self.PBM[p].ThirdMomentFromN(x[p]), 1])
+
+            '''
+            Concentration of the precipitates - needed to get matrix composition
+
+            For a line compound with composition x^beta, this boils down to:
+            x_0 = (1-f_v) * x^inf + f_v * x^beta
+                Where x_0 is initial composition, f_v is volume fraction and x^inf is matrix composition
+
+            For non-stoichiometric compounds, we want to integrate the precipitate composition as a function of radius
+                We'll call this term f_conc (fraction + concentration of precipitates), so:
+                x_0 = (1-f_v) * x^inf + f_conc
             
-            #Set negative frequencies in PSD to 0
-            #Also set any less than the minimum possible radius to be 0
-            self.PBM[p].PSD[:self.RdrivingForceIndex[p]] = 0
-            self.PBM[p].PSD[self.PBM[p].PSDsize < self.minRadius] = 0
-
-    def _massBalance(self, i):
+            For infinite precipitate diffusion, the concentration of a single precipitate is assumed to be homogenous
+            f_conc = r_vol * vol_factor * sum(n_i * R_i^3 * x_i^beta)
+                Where r_vol is V^alpha / V^beta and vol_factor is a factor for converting R^3 to volume (for sphere, this is 4*pi/3)
+
+            For no diffusion in precipitate, the concentration depends on the history of the precipitate compositions and growth rate
+            We just have to convert the summation to an integral of the time derivative of the terms inside
+            f_conc = r_vol * vol_factor * sum(int(d(n_i * R_i^3 * x_i^beta)/dt, dt))
+            We'll assume x_i^beta is constant with time (for 3 or more components, this is not true, but assume it doesn't change significantly per iteration - it'll also be a lot harder to account for)
+            d(f_conc)/dt = r_vol * vol_factor * sum(d(n_i)/dt * R_i^3 * x_i^beta + 3 * R_i^3 * d(R_i)/dt * n_i * x_i^beta)
+                d(n_i)/dt is the change in precipitates, since we don't record this, this is just (x[p] - self.PBM[p].PSD) / dt - with x[p] being the new number density for phase p
+                d(R_i)/dt is the growth rate, however, since we use a eulerian solver, this corresponds to the growth rate of the bins themselves, which is 0
+                    If we were to use a langrangian solver, then d(n_i)/dt would be 0 (since the density in each bin would be constant) and d(R_i)/dt would be the growth rate at R_i
+            Then we can calculate f_conc per iteration as a time integration like we do with some of the other variables
+            '''
+            if self.infinitePrecipitateDiffusion[p]:
+                compAvg = 0.5 * (self.PSDXbeta[p][:-1] + self.PSDXbeta[p][1:])
+                for e in range(self.numberOfElements):
+                    fConc[0,p,e] = volRatio * self.GB[p].volumeFactor * self.PBM[p].WeightedMomentFromN(x[p], 3, compAvg[:,e])
+            else:
+                midX = (self.PSDXbeta[p][1:] + self.PSDXbeta[p][:-1]) / 2
+                for e in range(self.numberOfElements):
+                    #y = volRatio * self.GB[p].volumeFactor * np.sum((3*midG*self.PBM[p].PSDsize**2*self.PBM[p].PSD*dt + self.PBM[p].PSDsize**3*(x[p]-self.PBM[p].PSD))*midX[:,e])
+                    y = volRatio * self.GB[p].volumeFactor * np.sum((self.PBM[p].PSDsize**3*(x[p]-self.PBM[p].PSD))*midX[:,e])
+                    fConc[0,p,e] = self.fConc[self.n,p,e] + y
+
+            #Only record these terms if there are non-zero number of precipitates
+            #Otherwise we will be dividing by 0 for avgR and avgAR
+            #   Argueably, RadSum and ARsum would be 0 if Ntot is 0, so it should be fine to do this
+            if Ntot > self.minNucleateDensity:
+                avgR[0,p] = RadSum / Ntot
+                precDens[0,p] = Ntot
+                avgAR[0,p] = ARsum / Ntot
+            else:
+                avgR[0,p] = 0
+                precDens[0,p] = 0
+                avgAR[0,p] = 0
+
+            #Not sure if needed, but just in case
+            if self.betaFrac[self.n,p] == 1:
+                fBeta[0,p] = 1
+
+        if np.sum(fBeta[0]) < 1:
+            xComp[0] = (self.xComp[0] - np.sum(fConc[0], axis=0)) / (1 - np.sum(fBeta[0]))
+            xComp[0,xComp[0] < 0] = self.minComposition
+
+        self._currY[self.VOL_FRAC] = fBeta
+        self._currY[self.FCONC] = fConc
+        self._currY[self.PREC_DENS] = precDens
+        self._currY[self.R_AVG] = avgR
+        self._currY[self.AR_AVG] = avgAR
+        self._currY[self.COMPOSITION] = xComp
+
+    def getCurrentX(self):
+        '''
+        Returns current value of time and X
+        In this case, X is the particle size distribution for each phase
+        '''
+        return self.time[self.n], [self.PBM[p].PSD for p in range(len(self.phases))]
+
+    def _getdXdt(self, t, x):
         '''
-        Updates matrix composition and volume fraction of precipitates
+        Returns dn_i/dt for each PBM of each phase
         '''
-        fBeta = np.zeros(len(self.phases))
-        if self.numberOfElements == 1:
-            fConc = np.zeros(len(self.phases))
-        else:
-            fConc = np.zeros((len(self.phases), self.numberOfElements))
+        return [self.PBM[p].getdXdtEuler(self.growth[p], self._currY[self.NUC_RATE][0,p], self._currY[self.R_NUC][0,p], x[p]) for p in range(len(self.phases))]
 
+    def correctdXdt(self, dt, x, dXdt):
+        '''
+        Corrects dXdt with the newly found dt, this adjusts the fluxes at the ends of the PBM so that we don't get negative bins
+        '''
         for p in range(len(self.phases)):
-            #Sum up particles and average for particles
-            Ntot = self.PBM[p].ZeroMoment()
-            RadSum = self.PBM[p].Moment(order=1)
-            ARsum = self.PBM[p].WeightedMoment(0, self.shapeFactors[p].aspectRatio(self.PBM[p].PSDsize))
-            fBeta[p] = self.VmAlpha / self.VmBeta[p] * self.GB[p].volumeFactor * self.PBM[p].ThirdMoment()
-
-            if self.numberOfElements == 1:
-                if self.infinitePrecipitateDiffusion[p]:
-                    fConc[p] = self.VmAlpha / self.VmBeta[p] * self.GB[p].volumeFactor * self.PBM[p].WeightedMoment(3, 0.5 * (self.PSDXbeta[p][:-1] + self.PSDXbeta[p][1:]))
-                else:
-                    y = self.VmAlpha / self.VmBeta[p] * self.GB[p].areaFactor * np.sum(self.PBM[p]._prevPSDbounds[1:]**2 * self.PBM[p]._fv[1:] * self._prevPSDXbeta[p][1:] * (self.PBM[p]._prevPSDbounds[1:] - self.PBM[p]._prevPSDbounds[:-1]))
-                    fConc[p] = self.prevFConc[0,p,0] + y
-                self.prevFConc[1,p,0] = copy.copy(self.prevFConc[0,p,0])
-                self.prevFConc[0,p,0] = fConc[p]
-            else:
-                if self.infinitePrecipitateDiffusion[p]:
-                    for a in range(self.numberOfElements):
-                        fConc[p,a] = self.VmAlpha / self.VmBeta[p] * self.GB[p].volumeFactor * self.PBM[p].WeightedMoment(3, 0.5 * (self.PSDXbeta[p][:-1,a] + self.PSDXbeta[p][1:,a]))
-                else:
-                    for a in range(self.numberOfElements):
-                        y = self.VmAlpha / self.VmBeta[p] * self.GB[p].areaFactor * np.sum(self.PBM[p]._prevPSDbounds[1:]**2 * self.PBM[p]._fv[1:] * self._prevPSDXbeta[p][1:,a] * (self.PBM[p]._prevPSDbounds[1:] - self.PBM[p]._prevPSDbounds[:-1]))
-                        fConc[p,a] = self.prevFConc[0,p,a] + y
-                self.prevFConc[1,p] = copy.copy(self.prevFConc[0,p])
-                self.prevFConc[0,p] = fConc[p]
-
-            #Average radius and precipitate density
-            if Ntot > 0:
-                self.avgR[p, i] = RadSum / Ntot
-                self.precipitateDensity[p, i] = Ntot
-                self.avgAR[p, i] = ARsum / Ntot
-            else:
-                self.avgR[p, i] = 0
-                self.precipitateDensity[p, i] = 0
-                self.avgAR[p, i] = 0
-            
-            #Volume fraction (max at 1)
-            if fBeta[p] > 1:
-                fBeta[p] = 1
-            if self.betaFrac[p, i-1] == 1:
-                fBeta[p] = 1
-            
-            self.betaFrac[p, i] = fBeta[p]
-        
-        #Composition (min at 0)
-        if self.numberOfElements == 1:
-            if np.sum(fBeta) < 1:
-                self.xComp[i] = (self.xComp[0] - np.sum(fConc)) / (1 - np.sum(fBeta))
-            else:
-                self.xComp[i] = 0
-        else:
-            if np.sum(fBeta) < 1:
-                self.xComp[i] = (self.xComp[0] - np.sum(fConc, axis=0)) / (1 - np.sum(fBeta))
-                self.xComp[i][self.xComp[i] < 0] = self.minComposition
-            else:
-                self.xComp[i] = np.zeros(self.numberOfElements)
+            dXdt[p] = self.PBM[p].correctdXdtEuler(dt, self.growth[p], self._currY[self.NUC_RATE][0,p], self._currY[self.R_NUC][0,p], x[p])
 
-    def _singleGrowthBinary(self, i, p):
+    def _singleGrowthBinary(self, p):
         '''
         Calculates growth rate for a single phase
         This is separated from _growthRateBinary since it's used in _calculatePSD
 
         Matrix/precipitate composition are not calculated here since it's
         already calculated in createLookup
         '''
+        xComp = self._currY[self.COMPOSITION][0]
+        T = self._currY[self.TEMPERATURE][0]
         growthRate = np.zeros(self.PBM[p].bins + 1)
         #If no precipitates are stable, don't calculate growth rate and set PSD to 0
         #This should represent dissolution of the precipitates
-        if self.RdrivingForceIndex[p]+1 < len(self.PSDXalpha[p]):
-            superSaturation = (self.xComp[i-1] - self.PSDXalpha[p]) / (self.VmAlpha * self.PSDXbeta[p] / self.VmBeta[p] - self.PSDXalpha[p])
-            growthRate = self.shapeFactors[p].kineticFactor(self.PBM[p].PSDbounds) * self.Diffusivity(self.xComp[i-1], self.T[i]) * superSaturation / (self.effDiffDistance(superSaturation) * self.PBM[p].PSDbounds)
-        else:
-            self.PBM[p].PSD = np.zeros(self.PBM[p].bins)
+        if self.RdrivingForceIndex[p]+1 < len(self.PSDXalpha[p][:,0]):
+            superSaturation = (xComp[0] - self.PSDXalpha[p][:,0]) / (self.VmAlpha * self.PSDXbeta[p][:,0] / self.VmBeta[p] - self.PSDXalpha[p][:,0])
+            growthRate = self.shapeFactors[p].kineticFactor(self.PBM[p].PSDbounds) * self.Diffusivity(xComp[0], T) * superSaturation / (self.effDiffDistance(superSaturation) * self.PBM[p].PSDbounds)
 
         return growthRate
-
     
-    def _growthRateBinary(self, i):
+    def _growthRateBinary(self):
         '''
         Determines current growth rate of all particle size classes in a binary system
         '''
         #Update equilibrium interfacial compositions
         #This will be override if createLookup is called
-        self.xEqAlpha[:,i] = self.xEqAlpha[:,i-1]
-        self.xEqBeta[:,i] = self.xEqBeta[:,i-1]
-
-        #Update lookup table if temperature changes too much
-        self.dTemp += self.T[i] - self.T[i-1]
+        T = self._currY[self.TEMPERATURE]
+        self.dTemp += T - self.temperature[self.n]
         if np.abs(self.dTemp) > self.maxTempChange:
-            self.createLookup(i)
+            xEqAlpha, xEqBeta = self.createLookup()
+        else:
+            xEqAlpha, xEqBeta = np.array([self.xEqAlpha[self.n]]), np.array([self.xEqBeta[self.n]])
             self.dTemp = 0
+        self._currY[self.EQ_COMP_ALPHA] = xEqAlpha
+        self._currY[self.EQ_COMP_BETA] = xEqBeta
         
         #growthRate = np.zeros((len(self.phases), self.bins + 1))
         growthRate = []
         for p in range(len(self.phases)):
-            growthRate.append(self._singleGrowthBinary(i, p))
+            growthRate.append(self._singleGrowthBinary(p))
             
         self.growth = growthRate
 
-    def _singleGrowthMulti(self, i, p):
+    def _singleGrowthMulti(self, p):
         '''
         Calculates growth rate for a single phase
         This is separated from _growthRateMulti since it's used in _calculatePSD
 
         This will also calculate the matrix/precipitate composition 
         for the radius in the PSD as well as equilibrium (infinite radius)
         '''
-        growth, xAlpha, xBeta, xEqAlpha, xEqBeta = self.interfacialComposition[p](self.xComp[i-1], self.T[i], self.dGs[p,i-1] * self.VmBeta[p], self.PBM[p].PSDbounds, self.particleGibbs(phase=self.phases[p]))
+        xComp = self._currY[self.COMPOSITION][0]
+        dGs = self._currY[self.DRIVING_FORCE][0]
+        T = self._currY[self.TEMPERATURE][0]
+        precDens = self._currY[self.PREC_DENS][0]
+        if dGs[p] < 0 and precDens[p] <= 0:
+            xEqAlpha = np.zeros(self.numberOfElements)
+            xEqBeta = np.zeros(self.numberOfElements)
+            growthRate = np.zeros(self.PBM[p].bins + 1)
+            return growthRate, xEqAlpha, xEqBeta
+
+
+        growth, xAlpha, xBeta, xEqAlpha, xEqBeta = self.interfacialComposition[p](xComp, T, dGs[p] * self.VmBeta[p], self.PBM[p].PSDbounds, self.particleGibbs(phase=self.phases[p]), searchDir = self._precBetaTemp[p])
 
         #If two-phase equilibrium not found, two possibilities - precipitates are unstable or equilibrium calculations didn't converge
+        #We try to avoid this as much as possible to where if precipitates are unstable, then attempt to get a growth rate from the nearest composition on the phase boundary
+        #And if equilibrium calculations didn't converge, try to use the previous calculations assuming the new composition is close to the previous
         if growth is None:
             #If driving force is negative, then precipitates are unstable
-            if self.dGs[p,i] < 0:
+            if dGs[p] < 0:
                 #Completely reset the PBM, including bounds and number of bins
                 #In case nucleation occurs again, the PBM will be at a good length scale
-                self.PBM[p].reset()
                 self.PSDXalpha[p] = np.zeros((self.PBM[p].bins + 1, self.numberOfElements))
                 self.PSDXbeta[p] = np.zeros((self.PBM[p].bins + 1, self.numberOfElements))
-                self.xEqAlpha[p,i] = np.zeros(self.numberOfElements)
-                self.xEqBeta[p,i] = np.zeros(self.numberOfElements)
-                return np.zeros(self.PBM[p].bins + 1)
+                xEqAlpha = np.zeros(self.numberOfElements)
+                xEqBeta = np.zeros(self.numberOfElements)
+                growthRate = np.zeros(self.PBM[p].bins + 1)
             #Else, equilibrium did not converge and just use previous values
             #Only the growth rate needs to be updated, since all other terms are previous
             #Also revert the PSD in case this function was called to adjust for the new PSD bins
             else:
-                self.PBM[p].revert()
-                return self.growth[p]
+                growthRate = self.growth[p]
         else:
             #Update interfacial composition for each precipitate size
             self.PSDXalpha[p] = xAlpha
             self.PSDXbeta[p] = xBeta
-            self.xEqAlpha[p,i] = xEqAlpha
-            self.xEqBeta[p,i] = xEqBeta
 
             #Add shape factor to growth rate - will need to add effective diffusion distance as well
-            return self.shapeFactors[p].kineticFactor(self.PBM[p].PSDbounds) * growth
+            growthRate = self.shapeFactors[p].kineticFactor(self.PBM[p].PSDbounds) * growth
+
+        return growthRate, xEqAlpha, xEqBeta
     
-    def _growthRateMulti(self, i):
+    def _growthRateMulti(self):
         '''
         Determines current growth rate of all particle size classes in a multicomponent system
         '''
+        xEqAlpha = np.zeros((1,len(self.phases), self.numberOfElements))
+        xEqBeta = np.zeros((1,len(self.phases), self.numberOfElements))
         growthRate = []
         for p in range(len(self.phases)):
-            growthRate.append(self._singleGrowthMulti(i, p))
+            growthRate_p, xEqAlpha_p, xEqBeta_p = self._singleGrowthMulti(p)
+            growthRate.append(growthRate_p)
+            xEqAlpha[0,p] = xEqAlpha_p
+            xEqBeta[0,p] = xEqBeta_p
+        self._currY[self.EQ_COMP_ALPHA] = xEqAlpha
+        self._currY[self.EQ_COMP_BETA] = xEqBeta
         self.growth = growthRate
 
+    def _updateParticleSizeDistribution(self, t, x):
+        '''
+        Updates particle size distribution with new x
+
+        Steps:
+            1. Check if growth rate calculation failed with negative driving force
+                We'll reset the PBM since we can't do much from here, but the chances of this happening should be pretty low
+            2. Update the PBM with new x
+            3. Check if the PBM needs to adjust the size class
+                If so, then update the cached aspect ratio and precipitate composition with the new size classes
+            4. Remove precipitates below a certain threshold (RdrivingForceIndex and minRadius)
+            5. Calculate the dissolution index (index at which below are not considered when calculating dt)
+                This is to prevent very small dt as the growth rate increases rapidly when R->0
+        '''
+        for p in range(len(self.phases)):
+            if self.dGs[self.n,p] < 0 and np.all(self.xEqAlpha[self.n,p,:] == 0):
+                self.PBM[p].reset()
+                self.PSDXalpha[p] = np.zeros((self.PBM[p].bins + 1, self.numberOfElements))
+                self.PSDXbeta[p] = np.zeros((self.PBM[p].bins + 1, self.numberOfElements))
+                self.growth[p] = np.zeros(self.PBM[p].bins+1)
+                continue
+            self.PBM[p].UpdatePBMEuler(t, x[p])
+            change, addedIndices = self.PBM[p].adjustSizeClassesEuler(all(self.growth[p] < 0))
+            if change:
+                if self.calculateAspectRatio[p]:
+                    self.eqAspectRatio[p] = self.strainEnergy[p].eqAR_bySearch(self.PBM[p].PSDbounds, self.gamma[p], self.shapeFactors[p])
+                else:
+                    self.eqAspectRatio[p] = self.shapeFactors[p].aspectRatio(self.PBM[p].PSDbounds)
+
+                self.growth[p] = np.zeros(len(self.PBM[p].PSDbounds))
+                if self.numberOfElements == 1:
+                    if addedIndices is None:
+                        #This is very slow to do
+                        self.createLookup()
+                    else:
+                        self.PSDXalpha[p] = np.concatenate((self.PSDXalpha[p], np.zeros((self.PBM[p].bins+1 - len(self.PSDXalpha[p]),1))))
+                        self.PSDXbeta[p] = np.concatenate((self.PSDXbeta[p], np.zeros((self.PBM[p].bins+1 - len(self.PSDXbeta[p]),1))))
+                        self.PSDXalpha[p][addedIndices:,0], self.PSDXbeta[p][addedIndices:,0] = self.interfacialComposition[p](self.temperature[self.n], self.particleGibbs(self.PBM[p].PSDbounds[addedIndices:], self.phases[p]))
+                else:
+                    self.PSDXalpha[p] = np.zeros((self.PBM[p].bins + 1, self.numberOfElements))
+                    self.PSDXbeta[p] = np.zeros((self.PBM[p].bins + 1, self.numberOfElements))
+                self._growthRate()
+            self.PBM[p].PSD[:self.RdrivingForceIndex[p]+1] = 0
+            self.PBM[p].PSD[self.PBM[p].PSDsize < self.minRadius] = 0
+            self.dissolutionIndex[p] = self.PBM[p].getDissolutionIndex(self.maxDissolution, self.RdrivingForceIndex[p])
+            #self.PBM[p].PSD[:self.dissolutionIndex[p]] = 0
+
     def plot(self, axes, variable, bounds = None, timeUnits = 's', radius='spherical', *args, **kwargs):
         '''
         Plots model outputs
         
         Parameters
         ----------
         axes : Axis
@@ -968,94 +756,11 @@
             For non-spherical precipitates, plot the Average Radius by the -
                 Equivalent spherical radius ('spherical')
                 Short axis ('short')
                 Long axis ('long')
             Note: Total Average Radius and Volume Average Radius will still use the equivalent spherical radius
         *args, **kwargs - extra arguments for plotting
         '''
-        sizeDistributionVariables = ['Size Distribution', 'Size Distribution Curve', 'Size Distribution KDE', 'Size Distribution Density']
-        compositionVariables = ['Interfacial Composition Alpha', 'Interfacial Composition Beta']
-
-        scale = []
-        for p in range(len(self.phases)):
-            if self.GB[p].nucleationSiteType == self.GB[p].BULK or self.GB[p].nucleationSiteType == self.GB[p].DISLOCATION:
-                if radius == 'spherical':
-                    scale.append(self._GBareaRemoval(p) * np.ones(len(self.PBM[p].PSDbounds)))
-                else:
-                    scale.append(1/self.shapeFactors[p].eqRadiusFactor(self.PBM[p].PSDbounds))
-                    if radius == 'long':
-                        scale.append(self.shapeFactors[p].aspectRatio(self.PBM[p].PSDbounds) / self.shapeFactors[p].eqRadiusFactor(self.PBM[p].PSDbounds))
-            else:
-                scale.append(self._GBareaRemoval(p) * np.ones(len(self.PBM[p].PSDbounds)))
-
-        if variable in compositionVariables:
-            if variable == 'Interfacial Composition Alpha':
-                yVar = self.PSDXalpha
-                ylabel = 'Composition in Alpha phase'
-            else:
-                yVar = self.PSDXbeta
-                ylabel = 'Composition in Beta Phase'
-
-            if (len(self.phases)) == 1:
-                axes.semilogx(self.PBM[0].PSDbounds, yVar[0], *args, **kwargs)
-            else:
-                for p in range(len(self.phases)):
-                    axes.plot(self.PBM[p].PSDbounds, yVar[p], label=self.phases[p], *args, **kwargs)
-                axes.legend()
-            axes.set_xlim([self.PBM[0].PSDbounds[0], self.PBM[0].PSDbounds[-1]])
-            axes.set_xlabel('Radius (m)')
-            axes.set_ylabel(ylabel)
-
-        elif variable in sizeDistributionVariables:
-            ylabel = 'Frequency (#/$m^3$)'
-            if variable == 'Size Distribution':
-                functionName = 'PlotHistogram'
-            elif variable == 'Size Distribution KDE':
-                functionName = 'PlotKDE'
-            elif variable == 'Size Distribution Density':
-                functionName = 'PlotDistributionDensity'
-                ylabel = 'Distribution Density (#/$m^4$)'
-            else:
-                functionName = 'PlotCurve'
-
-            if len(self.phases) == 1:
-                getattr(self.PBM[0], functionName)(axes, scale=scale[0], *args, **kwargs)
-            else:
-                for p in range(len(self.phases)):
-                    getattr(self.PBM[p], functionName)(axes, label=self.phases[p], scale=scale[p], *args, **kwargs)
-                axes.legend()
-            axes.set_xlabel('Radius (m)')
-            axes.set_ylabel(ylabel)
-            axes.set_xlim([0, np.amax([pb.max for pb in self.PBM])])
-            if variable == 'Size Distribution Density':
-                axes.set_ylim([0, 1.1*np.amax(np.concatenate(([np.amax(pb.PSD/(pb.PSDbounds[1:] - pb.PSDbounds[:-1])) for pb in self.PBM], [1])))])
-            else:
-                axes.set_ylim([0, 1.1*np.amax(np.concatenate(([np.amax(pb.PSD) for pb in self.PBM], [1])))])
+        plotEuler(self, axes, variable, bounds, timeUnits, radius, *args, **kwargs)
 
-        elif variable == 'Cumulative Size Distribution':
-            ylabel = 'CDF'
-            if len(self.phases) == 1:
-                self.PBM[0].PlotCDF(axes, scale=scale[0], *args, **kwargs)
-            else:
-                for p in range(len(self.phases)):
-                    self.PBM[p].PlotCDF(axes, label=self.phases[p], scale=scale[p], *args, **kwargs)
-                axes.legend()
-            axes.set_xlabel('Radius (m)')
-            axes.set_ylabel(ylabel)
-            axes.set_xlim([0, np.amax([pb.max for pb in self.PBM])])
-
-        elif variable == 'Aspect Ratio Distribution':
-            if len(self.phases) == 1:
-                axes.plot(self.PBM[0].PSDbounds * np.interp(self.PBM[p].PSDbounds, self.PBM[0].PSDbounds, scale[0]), self.eqAspectRatio[0], *args, **kwargs)
-            else:
-                for p in range(len(self.phases)):
-                    axes.plot(self.PBM[p].PSDbounds * np.interp(self.PBM[p].PSDbounds, self.PBM[p].PSDbounds, scale[p]), self.eqAspectRatio[p], label=self.phases[p], *args, **kwargs)
-                axes.legend()
-            axes.set_xlim([0, np.amax(self.PBM[p].PSDbounds * np.interp(self.PBM[p].PSDbounds, self.PBM[p].PSDbounds, scale[p]))])
-            axes.set_ylim(bottom=1)
-            axes.set_xlabel('Radius (m)')
-            axes.set_ylabel('Aspect ratio distribution')
-            
-        else:
-            super().plot(axes, variable, bounds, timeUnits, radius, *args, **kwargs)
 
-        
+
```

### Comparing `kawin-0.2.0/kawin/LebedevNodes.py` & `kawin-0.3.0/kawin/precipitation/non_ideal/LebedevNodes.py`

 * *Files identical despite different names*

### Comparing `kawin-0.2.0/kawin/LocalEquilibrium.py` & `kawin-0.3.0/kawin/thermo/LocalEquilibrium.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,18 @@
 
     Returns
     -------
     Dataset containing free energy and chemical potential
     '''
     # Broadcasting conditions not supported
     cur_conds = {str(k): float(v) for k, v in conds.items()}
-    state_variables = np.array([cur_conds['GE'], cur_conds['N'], cur_conds['P'], cur_conds['T']], dtype=np.float64)
+    if 'GE' in cur_conds:
+        state_variables = np.array([cur_conds['GE'], cur_conds['N'], cur_conds['P'], cur_conds['T']], dtype=np.float64)
+    else:
+        state_variables = np.array([0, cur_conds['N'], cur_conds['P'], cur_conds['T']], dtype=np.float64)
     if composition_sets is None:
         # Note: filter_phases() not called, so all specified phases must be valid
         composition_sets = []
 
         # Choose a naive starting point for each phase
         # only one composition set per phase is chosen
         # here, we just choose the point with the minimum Gibbs energy
```

### Comparing `kawin-0.2.0/kawin/PopulationBalance.py` & `kawin-0.3.0/kawin/precipitation/PopulationBalance.py`

 * *Files 26% similar despite different names*

```diff
@@ -58,22 +58,237 @@
 
         self.originalBins = bins
         self.setBinConstraints(bins, minBins, maxBins)
         
         self.reset()
 
         self._adaptiveBinSize = True
+        
+        self._record = False
+        self._recordedBins = None
+        self._recordedPSD = None
+        self._recordedTime = None
+
+    def reset(self, resetBounds = True):
+        '''
+        Resets the PSD to 0 and resets bin size and number of bins to original values
+        This will remove any size classes that were added since initialization
+        '''
+        if resetBounds:
+            self.min = self.originalMin
+            self.max = self.originalMax
+            self.bins = self.originalBins
+        self.PSDbounds = np.linspace(self.min, self.max, self.bins+1)
+        self.PSDsize = 0.5 * (self.PSDbounds[:-1] + self.PSDbounds[1:])
+            
+        self.PSD = np.zeros(self.bins)
+
+        #Hidden variable for use in KWNEuler when adaptive time stepping is enabled
+        #This allows for PSD to revert to its previous value if a time constraint is not met
+        self._prevPSD = np.zeros(self.bins)
+        self._prevPSDbounds = np.zeros(self.bins+1)
+
+        #Temporary storage for net flux
+        #This is used to correct the fluxes once the time step is known
+        self._netFlux = None
+
+    def enableRecording(self):
+        '''
+        Enables recording of particle size distribution per iteration
+
+        The initial data in the recorded bin is t = 0, N_i = 0
+
+        The size of the recorded particle size distribution will be (n x max bins)
+            Where n in the number of iterations
+            max bins is the maximum number of bins, if the current number is smaller, the rest of the array will be 0
+        '''
+        self._record = True
+        self._recordedBins = np.zeros((1, self.maxBins + 1))
+        self._recordedPSD = np.zeros((1, self.maxBins))
+        self._recordedTime = np.zeros(1)
+
+    def resetRecordedData(self):
+        '''
+        If recording, then reset the recorded bins to the original size (starting with t = 0, N_i = 0)
+        If not recording, then clear the recorded data
+        '''
+        if self._record:
+            self._recordedBins = np.zeros((1, self.maxBins + 1))
+            self._recordedPSD = np.zeros((1, self.maxBins))
+            self._recordedTime = np.zeros(1)
+        else:
+            self._recordedBins = None
+            self._recordedPSD = None
+            self._recordedTime = None
+
+    def disableRecording(self):
+        '''
+        Disables recording
+
+        We won't clear the recorded bins here in case the user still wants to grab recorded data
+        '''
+        self._record = False
+
+    def setRecording(self, record = True):
+        '''
+        Wrapper around enable and disable recording
+        '''
+        if record:
+            self.enableRecording()
+        else:
+            self.disableRecording()
+
+    def removeRecordedData(self):
+        '''
+        Removes recorded data
+        '''
+        self._recordedBins = None
+        self._recordedPSD = None
+        self._recordedTime = None
+
+    def record(self, time):
+        '''
+        Adds current PSD data to recorded arrays
+
+        TODO: Make sure this works when adaptive bins is False
+        '''
+        if self._record:
+            maxBins = self.maxBins if self._adaptiveBinSize else self.bins
+            self._recordedBins = np.pad(self._recordedBins, ((0, 1), (0, maxBins+1 - self._recordedBins.shape[1])))
+            self._recordedPSD = np.pad(self._recordedPSD, ((0, 1), (0, maxBins - self._recordedPSD.shape[1])))
+            self._recordedTime = np.pad(self._recordedTime, (0,1))
+            self._recordedBins[-1][:self.PSDbounds.shape[0]] = self.PSDbounds
+            self._recordedPSD[-1][:self.PSD.shape[0]] = self.PSD
+            self._recordedTime[-1] = time
+
+    def saveRecordedPSD(self, filename, compressed = True):
+        '''
+        Saves recorded data into npz format
+
+        Note: If recording is disabled, then this function will do nothing since 
+              there is nothing to save anyways
+
+        Parameters
+        ----------
+        filename : str
+            File name to save to
+        compressed : bool (optional)
+            Whether to save as in compressed format (defaults to True)
+        '''
+        if self._record:
+            if compressed:
+                np.savez_compressed(filename, time = self._recordedTime, bins = self._recordedBins, PSD = self._recordedPSD)
+            else:
+                np.savez(filename, time = self._recordedTime, bins = self._recordedBins, PSD = self._recordedPSD)
+
+    def loadRecordedPSD(self, filename):
+        '''
+        Loads recorded PSD
+        '''
+        data = np.load(filename)
+        self._record = True
+        self._recordedTime = data['time']
+        self._recordedBins = data['bins']
+        self._recordedPSD = data['PSD']
+
+    def _grabPSDfromIndex(self, index):
+        '''
+        Returns PSD bounds, PSD bins and PSD from recorded data based off index
+
+        Since the number of bins is likely less than the max, we want to grab only the non-zero indices
+        TODO: two concerns
+            1) this may remove the last 1 bins (this may be okay since we add new bins once the
+                list bins has at least 1 particle), so the last bin would be 0 anyways
+        '''
+        nonzero = len(np.nonzero(self._recordedBins[index])[0])
+        if nonzero == 0:
+            PSDbounds = np.linspace(self.originalMin, self.originalMax, self.originalBins+1)
+            PSDsize = 0.5 * (PSDbounds[1:] + PSDbounds[:-1])
+            PSD = np.zeros(self.originalBins)
+        else:
+            PSDbounds = self._recordedBins[index,:nonzero]
+            PSD = self._recordedPSD[index,:nonzero-1]
+            PSDsize = 0.5 * (PSDbounds[1:] + PSDbounds[:-1])
+        bins = len(PSD)
+        minBound, maxBound = np.amin(PSDbounds), np.amax(PSDbounds)
+        return PSDbounds, PSD, PSDsize, bins, minBound, maxBound
+
+    def setPSDtoRecordedTime(self, time):
+        '''
+        Sets particle size distribution to specific time if recorded
+
+        Parameter
+        ---------
+        time : float
+            Time to load PSD from, will load to nearest time available
+        '''
+        if self._record:
+            if time <= self._recordedTime[0]:
+                print('Input time is lower than smallest recorded time, setting PSD to t = {:.3e}'.format(self._recordedTime[0]))
+                self.PSDbounds, self.PSD, self.PSDsize, self.bins, self.min, self.max = self._grabPSDfromIndex(0)
+            elif time >= self._recordedTime[-1]:
+                print('Input time is larger than longest recorded time, setting PSD to t = {:.3e}'.format(self._recordedTime[-1]))
+                self.PSDbounds, self.PSD, self.PSDsize, self.bins, self.min, self.max = self._grabPSDfromIndex(-1)
+            else:
+                #Upper and lower PSD
+                #Note: horrible naming convention here
+                #    Upper PSD refers to the PSD just after time
+                #    Lower PSD refers to the PSD just before time
+                #This does NOT refer to the PSD with the larger or smaller number of bins
+                uind = np.argmax(self._recordedTime > time)
+                lind = uind - 1
+
+                utime, ltime = self._recordedTime[uind], self._recordedTime[lind]
+                uPSDbounds, uPSD, uPSDsize, ubins, umin, umax = self._grabPSDfromIndex(uind)
+                lPSDbounds, lPSD, lPSDsize, lbins, lmin, lmax = self._grabPSDfromIndex(lind)
+
+                #Interpolate from lower PSD to upper PSD using bounds of larger PSD
+                #This will account for all possible cases if the PSD size classes change
+                #This is done by pretending we're calling changeSizeClasses
+                #    Where we resize the PSD with the smaller number of bins to have the same bins as the larger PSD
+                #    And correct for the possible change in number density
+                if ubins >= lbins:
+                    #Resize lower PSD to upper PSD
+                    oldV = np.sum(lPSD * lPSDsize**3)
+                    distDen = lPSD / (lPSDbounds[1:] - lPSDbounds[:-1])
+                    rOld = 0.5 * (lPSDbounds[1:] + lPSDbounds[:-1])
+                    lPSD = np.interp(uPSDsize, rOld, distDen, left=0, right=0) * (uPSDbounds[1:] - uPSDbounds[:-1])
+                    newV = np.sum(lPSD * uPSDsize**3)
+                    if newV != 0:
+                        lPSD *= oldV / newV
+                    else:
+                        lPSD = np.zeros(ubins)
+                    
+                else:
+                    #Resize upper PSD to lower PSD
+                    oldV = np.sum(uPSD * uPSDsize**3)
+                    distDen = uPSD / (uPSDbounds[1:] - uPSDbounds[:-1])
+                    rOld = 0.5 * (uPSDbounds[1:] + uPSDbounds[:-1])
+                    uPSD = np.interp(lPSDsize, rOld, distDen, left=0, right=0) * (lPSDbounds[1:] - lPSDbounds[:-1])
+                    uPSDbounds = lPSDbounds
+                    newV = np.sum(uPSD * lPSDsize**3)
+                    if newV != 0:
+                        uPSD *= oldV / newV
+                    else:
+                        uPSD = np.zeros(lbins)
+
+                #Now that the bin sizes are the same, we can just interpolate the PSD
+                self.PSDbounds = uPSDbounds
+                self.PSDsize = 0.5 * (self.PSDbounds[1:] + self.PSDbounds[:-1])
+                self.PSD = (uPSD - lPSD) * (time - ltime) / (utime - ltime) + lPSD
+                self.bins = len(self.PSDsize)
+                self.min, self.max = np.amin(self.PSDbounds), np.amax(self.PSDbounds)
 
     def setAdaptiveBinSize(self, adaptive):
         '''
         For Euler implementation, sets whether to change the bin size when 
         the number of filled bins > maxBins or < minBins
 
-        If False, the bins will still change if nucleated particles are greater than the max bin size
-        and bins will still be added when the last bins starts to fill (although this will not change the bin size)
+        If False, the bins will still be if nucleated particles are greater than the max bin size
+        and bins will still be added when the last bins starts to fill (but this will not change the bin size)
         '''
         self._adaptiveBinSize = adaptive
 
     def setBinConstraints(self, bins = 150, minBins = 100, maxBins = 200):
         '''
         Sets constraints for minimum and maxinum number of bins over an order of magnitude
 
@@ -114,48 +329,34 @@
         '''
         self._prevPSD = copy.copy(self.PSD)
         self._prevPSDbounds = copy.copy(self.PSDbounds)
 
     def revert(self):
         '''
         Reverts to previous PSD and PSDbounds
+
+        NOTE: this appears to be unused
+            (this was used in the previous KWNEuler implementation when the PSD could change within an iteration)
+            (now it changes between iterations, so we don't need to revert back if something goes wrong)
         '''
         self.PSD = copy.copy(self._prevPSD)
         self.PSDbounds = copy.copy(self._prevPSDbounds)
         self.PSDsize = 0.5 * (self.PSDbounds[1:] + self.PSDbounds[:-1])
         self.bins = len(self.PSD)
         self.min, self.max = self.PSDbounds[0], self.PSDbounds[-1]
 
-    def reset(self, resetBounds = True):
-        '''
-        Resets the PSD to 0
-        This will remove any size classes that were added since initialization
-        '''
-        if resetBounds:
-            self.min = self.originalMin
-            self.max = self.originalMax
-            self.bins = self.originalBins
-        self.PSDbounds = np.linspace(self.min, self.max, self.bins+1)
-        self.PSDsize = 0.5 * (self.PSDbounds[:-1] + self.PSDbounds[1:])
-            
-        self.PSD = np.zeros(self.bins)
-
-        #Hidden variable for use in KWNEuler when determining composition assuming no diffusion in precipitate
-        #Represents d(PSD)/dr * growth rate * dt
-        #I would like this variable to be in KWNEuler, but this way is much easier
-        self._fv = np.zeros(self.bins + 1)
-
-        #Hidden variable for use in KWNEuler when adaptive time stepping is enabled
-        #This allows for PSD to revert to its previous value if a time constraint is not met
-        self._prevPSD = np.zeros(self.bins)
-        self._prevPSDbounds = np.zeros(self.bins+1)
-
     def changeSizeClasses(self, cMin, cMax, bins = None, resetPSD = False):
         '''
         Changes the size classes and resets the PSD
+
+        This is done by linear interpolation of the previous bins and PSD
+        And interpolating to the new bins and PSD
+        Due to differences in bin size (thus resolution of the PSD), the number density
+            could be a little different. To correct for this, we get the 3rd moment of the
+            previous PSD and the new PSD, and correct the new PSD to have the same 3rd moment
         
         Parameters
         ----------
         cMin : float
             Lower bound of PSD
         cMax : float
             Upper bound of PSD
@@ -180,61 +381,49 @@
             if newV != 0:
                 self.PSD *= oldV / newV
             else:
                 self.PSD = np.zeros(self.bins)
 
     def addSizeClasses(self, bins = 1):
         '''
-        Adds an additional size class to end of distribution
+        Adds an additional number of size classes to end of distribution
 
         Parameters
         ----------
         bins : int
             Number of bins to add
         '''
         self.bins += bins
         self.PSD = np.append(self.PSD, np.zeros(bins))
 
         self.max += bins * (self.PSDbounds[1] - self.PSDbounds[0])
         self.PSDbounds = np.linspace(self.min, self.max, self.bins+1)
         self.PSDsize = 0.5 * (self.PSDbounds[:-1] + self.PSDbounds[1:])
 
-    def getDTEuler(self, currDT, growth, maxDissolution, startIndex):
+    def adjustSizeClassesEuler(self, checkDissolution = False):
         '''
-        Calculates time interval for Euler implementation
-            dt < dR / (2 * growth rate)
-        This ensures that at most, only half of particles in one size class can go to another
+        1) adds some bins to the end of the PSD if the last bin has at least 1 precipitate
+            Number of bins is 1/4 of the original number of bins
+        2) If adaptive bin size is enabled, then two checks
+            2a) if number of bins > max bins, then resize to have the number of bins be the minimum
+            2b) if checking dissolution and number of filled bins < 1/2 min bins,
+                then resize to last filled bin with the number of bins being the maximum
 
         Parameters
         ----------
-        currDT : float
-            Current time interval, will be returned if it's smaller than what's given by the contraint
-        growth : array of floats
-            Growth rate, must have lenth of bins+1 (or length of PSDbounds)
-        maxDissolution : float
-            Maximum volume allowed to dissolve
-        startIndex : int
-            First index to look at for growth rate, all indices below startIndex will be ignored
-        '''
-        dissFrac = maxDissolution * self.ThirdMoment()
-        dissIndex = np.amax([np.argmax(self.CumulativeMoment(3) > dissFrac), startIndex])
-        growthFilter = growth[dissIndex:-1][self.PSD[dissIndex:] > 0]
-        #if len(growthFilter) == 0 or np.amax(growthFilter) < 0:
-        if len(growthFilter) == 0:
-            return currDT
-        else:
-            if np.amax(np.abs(growthFilter)) == 0:
-                return currDT
-            else:
-                return np.amin([currDT, (self.PSDbounds[1] - self.PSDbounds[0]) / (2 * np.amax(np.abs(growthFilter)))])
-
-    def adjustSizeClassesEuler(self, checkDissolution = False):
-        '''
-        Adds a size class if last class in PBM is filled
-        Changes length of size classes based off number of allowed bins
+        checkDissolution : bool
+            Whether to check if the PSD is getting smaller and resize accordingly
+
+        Returns
+        -------
+        change : bool
+            When the number of bins changed
+        newIndices : int or None
+            The number of bins added to the PSD
+            If the size of the bins changed, then this is None to indicate that resizing occured
         '''
         change = False
         newIndices = None
         if self.PSD[-1] > 1:
             #print('adding bins')
             newIndices = self.bins
             self.addSizeClasses(int(self.originalBins/4))
@@ -270,153 +459,314 @@
         order : int (optional)
             Order of moment that PSD will be normalized to (defaults to 0)
             Using zeroth order will normalize the PSD so the sum of PSD will be 1
         '''
         total = self.Moment(order)
         self.PSD /= total
 
-    def Nucleate(self, amount, radius):
+    def getDissolutionIndex(self, maxDissolution, minIndex = 0):
         '''
-        Adds nucleated particles to PSD given radius and amount of particles
+        Finds indices when the volume fraction of particles below this index is 
+        within the maximum amount (fraction-wise) that the PSD is allowed to dissolve
+
+        So find R_max where int(0, R_max, R^3 * dr) < maxDissolution * int(0, infinity, R^3 * dr)
+        The index is the correspoinding index to R_max
 
         Parameters
         ----------
-        amount : float
-            Amount of nucleated particles
-        radius : float
-            Radius of nucleated particles
+        maxDissolution : float
+            Max fraction allowed to dissolve
+        minIndex : int
+            Minimum index which below, all particles are allowed to dissolve
+            Upper limit on dissolution index
+
+        Returns
+        -------
+        max of [dissolution index, minIndex]
         '''
-        if amount < 1:
-            return False
-            
-        change = False
-
-        #Find size class for nucleated particles
-        nRad = np.argmax(self.PSDbounds > radius) - 1
-
-        #If radius is larger than length scale of PBM, adjust PBM such that radius is towards the beginning
-        if nRad == -1 and radius > 0:
-            #print('adding nucleated bins')
-            self.changeSizeClasses(self.PSDbounds[0], 5 * radius, self.originalBins)
-            nRad = np.argmax(self.PSDbounds > radius)
-            change = True
-        self.PSD[nRad] += amount
-        return change
+        dissFrac = maxDissolution * self.ThirdMoment()
+        dissIndex = np.argmax(self.CumulativeMoment(3) > dissFrac) - 1
+        if dissIndex < 0:
+            dissIndex = 0
+        return np.amax([np.argmax(self.CumulativeMoment(3) > dissFrac), minIndex])
         
-    def UpdateEuler(self, dt, flux):
+
+    def getDTEuler(self, currDT, growth, dissolutionIndex, maxBinRatio = 0.4):
         '''
-        Updates PSD given the flux and any external contributions
+        Calculates time interval for Euler implementation
+            dt < dR / (2 * growth rate)
+        This ensures that at most, only half of particles in one size class can go to another
+
+        Also finds dt such that the max delta in growth rate is 0.4 dR
+            We could use 0.5 dR which is the upper limit
+                (for a given bin, the max change in density would remove all particles, with 0.5 getting smaller and 0.5 getting bigger)
+            But 0.4 dR should be slightly more stable
+
+        TODO: allow variable ratio - this will make it more flexible for testing different time step constraints
 
-        Change in the amount of particles in a given size class = d(G*n)/dx
-        Where G is flux of size class, n is number of particles in size class and dx is range of size class
-        
         Parameters
         ----------
-        dt : float
-            Time increment
-        flux : array
-            Growth rate of each particle size class
-            Array size must be (bins + 1) since this operates on bounds of size classes
+        currDT : float
+            Current time interval, will be returned if it's smaller than what's given by the contraint
+        growth : array of floats
+            Growth rate, must have lenth of bins+1 (or length of PSDbounds)
+        maxDissolution : float
+            Maximum volume allowed to dissolve
+        startIndex : int
+            First index to look at for growth rate, all indices below startIndex will be ignored
+        maxBinRatio : float (optional)
+            Max ratio of particles in bin allowed to move to a nearby bin
+            Default is 0.4
         '''
-        netFlux = np.zeros(self.bins + 1)
+        self.maxRatio = maxBinRatio
+        growthFilter = growth[dissolutionIndex:-1][self.PSD[dissolutionIndex:] > 0]
 
-        #Array of 0 (flux <= 0), 1 (flux > 0)
+        if len(growthFilter) == 0:
+            return currDT
+        else:
+            if np.amax(np.abs(growthFilter)) == 0:
+                return currDT
+            else:
+                return self.maxRatio * (self.PSDbounds[1] - self.PSDbounds[0]) / np.amax(np.abs(growthFilter))
+    
+    def getdXdtEuler(self, flux, nucRate, nucRadius, psd):
+        '''
+        dn_i/dt = d(G*n)/dr + nucRate
+
+        d(G*n)/dr is calculated from two conditions
+        For positive growth rates - d(G*n)/dr|_i = n_i * flux_i / dr
+        For negative growth rates - d(G*n)/dr|_i = n_(i-1) * flux_i / dr
+        TODO : check that the two equations above represent the implementation
+
+        Parameters
+        ----------
+        flux : numpy array (bins+1)
+            Growth rate of particles in m/s
+        nucRate : float
+            Nucleation rate in #/m^3/s
+        nucRadius : float
+            Nucleation radius in m
+        psd : numpy array (bins)
+            Particle size distribution with number density #/m3
+
+        Returns
+        -------
+        dXdt (bins) - corresponds to dn_i/dt
+        '''
+        self._netFlux = np.zeros(self.bins+1)
         fluxSign = np.sign(flux)
         fluxSign[fluxSign == -1] = 0
+        dR = self.PSDbounds[1:] - self.PSDbounds[:-1]
+        self._netFlux[:-1] += flux[:-1] * psd * (1-fluxSign[:-1]) / dR
+        self._netFlux[1:] += flux[1:] * psd * fluxSign[1:] / dR
 
-        #If flux is negative (from class n to n-1), then take from size class n
-        #If flux is positive, then take from size class n-1
-        netFlux[:-1] += dt * flux[:-1] * self.PSD * (1-fluxSign[:-1]) / (self.PSDbounds[1:] - self.PSDbounds[:-1])
-        netFlux[1:] += dt * flux[1:] * self.PSD * fluxSign[1:] / (self.PSDbounds[1:] - self.PSDbounds[:-1])
-
-        #Brute force stability so PSD is never negative
-        #If the time step is determined from getDTEuler, this should be unnecessary
-        netFlux[1:-1][netFlux[1:-1] < -self.PSD[1:]] = -self.PSD[1:][netFlux[1:-1] < -self.PSD[1:]]
-        netFlux[1:-1][netFlux[1:-1] > self.PSD[:-1]] = self.PSD[:-1][netFlux[1:-1] > self.PSD[:-1]]
+        dXdt = (self._netFlux[:-1] - self._netFlux[1:])
 
-        self._fv = netFlux
-        
-        self.PSD += (netFlux[:-1] - netFlux[1:])
-        
-        #Adjust size classes and return True if the size classes had changed
-        change, newIndices = self.adjustSizeClassesEuler(all(flux<0))
-            
-        #Set negative frequencies to 0
+        #Find size class for nucleated particles
+        nRad = np.argmax(self.PSDbounds > nucRadius) - 1
+        dXdt[nRad] += nucRate
+
+        return dXdt
+    
+    def correctdXdtEuler(self, dt, flux, nucRate, nucRadius, psd):
+        '''
+        Given dt, correct the net flux so PSD will not be negative
+            Essentially, the total number of particles leaving a bin should be less than or equal to the number of particles in the bin
+
+        Size of fluxes is bins+1 while for PSD, it is bins
+
+        For fluxes on the right (positive) side of the PSD
+            We limit fluxes so that J_i+1 * dt < PSD_i
+
+        For fluxes on the left (negative) side of the PSD
+            We limit fluxes so that -J_i * dt < PSD_i
+
+        Normally, this wouldn't be an issue since the time step from getDtEuler would limit J_i*dt to less than half the number of particles in a bin
+            But because we set a dissolution threshold to ignore (to prevent extremely small dt since growth rate scales by 1/r), the bins below
+            the dissolution threshold will not follow the constraint we apply in getDtEuler
+
+        Parameters
+        ----------
+        dt : float
+            time step
+        flux : numpy array (bins+1)
+            Growth rate of particles in m/s
+        nucRate : float
+            Nucleation rate in #/m^3/s
+        nucRadius : float
+            Nucleation radius in m
+        psd : numpy array (bins)
+            Particle size distribution with number density #/m3
+
+        Returns
+        -------
+        dXdt (bins) - corresponds to dn_i/dt corrected to avoid negative bins
+        '''
+        #indBelow = self._netFlux[1:-1]*dt < -psd[1:]
+        #self._netFlux[1:-1][indBelow] = -psd[1:][indBelow] / dt
+        #indAbove = self._netFlux[1:-1]*dt > psd[:-1]
+        #self._netFlux[1:-1][indAbove] = psd[:-1][indAbove] / dt
+
+        indBelow = self._netFlux[:-1]*dt < -psd
+        self._netFlux[:-1][indBelow] = -psd[indBelow] / dt
+        indAbove = self._netFlux[1:]*dt > psd
+        self._netFlux[1:][indAbove] = psd[indAbove] / dt
+
+        dXdt = (self._netFlux[:-1] - self._netFlux[1:])
+
+        #Find size class for nucleated particles
+        nRad = np.argmax(self.PSDbounds > nucRadius) - 1
+        dXdt[nRad] += nucRate
+
+        return dXdt
+    
+    def UpdatePBMEuler(self, time, newN):
+        '''
+        Updates PBM with new values
+
+        Parameters
+        ----------
+        time : float
+            New time
+        newN : numpy array
+            New number density
+        '''
+        self.PSD = newN
         self.PSD[self.PSD < 1] = 0
+        self.record(time)
 
-        return change, newIndices
+    def MomentFromN(self, N, order):
+        '''
+        Given arbtrary PSD, return moment
 
-    def UpdateLagrange(self, dt, flux):
+        Parameters
+        ----------
+        N : numpy array
+            PSD / number density
+        order : float
+            Moment order
+        '''
+        return np.sum(N * self.PSDsize**order)
+    
+    def CumulativeMomentFromN(self, N, order):
         '''
-        Updates bounds of size classes with given growth rate
-        Fluxes of particles between size classes is d(Gn)/dx,
-        however, keeping the number of particles in each size class the same,
-        the bounds of the size classes can be updated by r_i = v_i * dt
+        Given arbtrary PSD, return cumulative moment (from 0 to max)
 
         Parameters
         ----------
-        dt : float
-            Time increment
-        flux : array
-            Growth rate of each particle size class
-            Array size must be (bins + 1) since this operates on bounds of size classes
+        N : numpy array
+            PSD / number density
+        order : float
+            Moment order
         '''
-        self._prevPSDbounds = copy.copy(self.PSDbounds)
-        self.PSDbounds += flux * dt
-        self.PSDsize = 0.5 * (self.PSDbounds[1:] + self.PSDbounds[:-1])
+        return np.cumsum(N * self.PSDsize**order)
+    
+    def WeightedMomentFromN(self, N, order, weights):
+        '''
+        Given arbtrary PSD, return weighted moment
+
+        Parameters
+        ----------
+        N : numpy array
+            PSD / number density
+        order : float
+            Moment order
+        weights : numpy array
+            Weights for each bin
+        '''
+        return np.sum(N * self.PSDsize**order * weights)
+    
+    def CumulativeWeightedMomentFromN(self, N, order, weights):
+        '''
+        Given arbtrary PSD, return cumulative weighted moment (from 0 to max)
+
+        Parameters
+        ----------
+        N : numpy array
+            PSD / number density
+        order : float
+            Moment order
+        weights : numpy array
+            Weights for each bin
+        '''
+        return np.cumsum(self.PSD * self.PSDsize**order * weights)
+    
+    def ZeroMomentFromN(self, N):
+        '''
+        Sum of N
+        '''
+        return self.MomentFromN(N, 0)
+    
+    def FirstMomentFromN(self, N):
+        '''
+        Length weighted moment of N
+        '''
+        return self.MomentFromN(N, 1)
+        
+    def SecondMomentFromN(self, N):
+        '''
+        Area weighted moment of N
+        '''
+        return self.MomentFromN(N, 2)
+        
+    def ThirdMomentFromN(self, N):
+        '''
+        Volume weighted moment of N
+        '''
+        return self.MomentFromN(N, 3)
         
     def Moment(self, order):
         '''
         Moment of specified order
 
         Parameters
         ----------
         order : int
             Order of moment
         '''
-        return np.sum(self.PSD * self.PSDsize**order)
+        return self.MomentFromN(self.PSD, order)
 
     def CumulativeMoment(self, order):
         '''
         Cumulative distribution using moment of specified order
 
         Parameters
         ----------
         order : int
             Order of moment
         '''
-        return np.cumsum(self.PSD * self.PSDsize**order)
+        return self.CumulativeMomentFromN(self.PSD, order)
         
     def WeightedMoment(self, order, weights):
         '''
         Weighted moment of specified order
 
         Parameters
         ----------
         order : int
             Order of moment
         weights : array
             Weights to apply to each size class
             Array size of (bins)
         '''
-        return np.sum(self.PSD * self.PSDsize**order * weights)
+        return self.WeightedMomentFromN(self.PSD, order, weights)
 
     def CumulativeWeightedMoment(self, order, weights):
         '''
         Weighted moment of specified order
 
         Parameters
         ----------
         order : int
             Order of moment
         weights : array
             Weights to apply to each size class
             Array size of (bins)
         '''
-        return np.cumsum(self.PSD * self.PSDsize**order * weights)
+        return self.CumulativeWeightedMomentFromN(self.PSD, order, weights)
 
     def ZeroMoment(self):
         '''
         Sum of the PSD
         '''
         return self.Moment(0)
     
@@ -458,15 +808,15 @@
                 reported precipitate radius differs from the radius
                 determined by precipitate curvature
         *args, **kwargs - extra arguments for plotting
         '''
         if hasattr(scale, '__len__'):
             scale = np.interp(self.PSDsize, self.PSDbounds, scale)
         else:
-            scale = scale * np.ones(self.PSDsize)
+            scale = scale * np.ones(len(self.PSDsize))
 
         if fill:
             axes.fill_between(self.PSDsize * scale, self.PSD, np.zeros(len(self.PSD)), *args, **kwargs)
         else:
             axes.plot(self.PSDsize * scale, self.PSD, *args, **kwargs)
         self.setAxes(axes, scale, logX, logY) 
 
@@ -491,15 +841,15 @@
                 reported precipitate radius differs from the radius
                 determined by precipitate curvature
         *args, **kwargs - extra arguments for plotting
         '''
         if hasattr(scale, '__len__'):
             scale = np.interp(self.PSDsize, self.PSDbounds, scale)
         else:
-            scale = scale * np.ones(self.PSDsize)
+            scale = scale * np.ones(len(self.PSDsize))
 
         if fill:
             axes.fill_between(self.PSDsize * scale, self.PSD, np.zeros(len(self.PSD)), *args, **kwargs)
         else:
             axes.plot(self.PSDsize * scale, self.PSD / (self.PSDbounds[1:] - self.PSDbounds[:-1]), *args, **kwargs)
         
         #Set x-limits
@@ -539,22 +889,25 @@
         scale : float (optional)
             Scale factor for x-axis (defaults to 1)
             Note: this is for grain boundary nucleation where the
                 reported precipitate radius differs from the radius
                 determined by precipitate curvature
         *args, **kwargs - extra arguments for plotting
         '''
-        kernel = sts.gaussian_kde(self.PSDsize, bw_method = bw_method, weights = self.PSD)
-        x = np.linspace(self.min, self.max, 1000)   
-        y = kernel(x) * self.ZeroMoment() * (self.PSDbounds[1] - self.PSDbounds[0])
+        x = np.linspace(self.min, self.max, 1000) 
+        if np.all(self.PSD == 0):
+            y = np.zeros(x.shape)
+        else:
+            kernel = sts.gaussian_kde(self.PSDsize, bw_method = bw_method, weights = self.PSD)  
+            y = kernel(x) * self.ZeroMoment() * (self.PSDbounds[1] - self.PSDbounds[0])
 
         if hasattr(scale, '__len__'):
             scale = np.interp(x, self.PSDbounds, scale)
         else:
-            scale = scale * np.ones(x)
+            scale = scale * np.ones(len(x))
         
         if fill:
             axes.fill_between(x * scale, y, np.zeros(len(y)), *args, **kwargs)
         else:
             axes.plot(x * scale, y, *args, **kwargs)
         self.setAxes(axes, scale, logX, logY) 
             
@@ -590,15 +943,15 @@
             xCoord, yCoord = np.zeros(1 + 2 * self.bins), np.zeros(1 + 2 * self.bins)
             xCoord[0], xCoord[1::2], xCoord[2::2] = self.PSDbounds[0], self.PSDbounds[:-1], self.PSDbounds[1:]
             yCoord[1::2], yCoord[2::2] = self.PSD, self.PSD
 
         if hasattr(scale, '__len__'):
             scale = np.interp(xCoord, self.PSDbounds, scale)
         else:
-            scale = scale * np.ones(xCoord)
+            scale = scale * np.ones(len(xCoord))
 
         if outline != 'no outline':
             axes.plot(xCoord * scale, yCoord, *args, **kwargs)
             if fill:
                 axes.fill_between(xCoord * scale, yCoord, np.zeros(len(yCoord)), alpha=0.3, *args, **kwargs)
         else:
             axes.fill_between(xCoord * scale, yCoord, np.zeros(len(yCoord)), *args, **kwargs)
@@ -622,15 +975,15 @@
         order : int (optional)
             Moment of specified order
         *args, **kwargs - extra arguments for plotting
         '''
         if hasattr(scale, '__len__'):
             scale = np.interp(self.PSDsize, self.PSDbounds, scale)
         else:
-            scale = scale * np.ones(self.PSDsize)
+            scale = scale * np.ones(len(self.PSDsize))
 
         axes.plot(self.PSDsize * scale, self.CumulativeMoment(order) / self.Moment(order), *args, **kwargs)
         self.setAxes(axes, scale, logX, False) 
         axes.set_ylim([0, 1])
         
     def setAxes(self, axes, scale = 1, logX = False, logY = False): 
         '''
```

### Comparing `kawin-0.2.0/kawin/ShapeFactors.py` & `kawin-0.3.0/kawin/precipitation/non_ideal/ShapeFactors.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,29 @@
         '''
         Aspect ratio as a function of radius if the aspect ratio is set as a scalar
         '''
         if hasattr(R, '__len__'):
             return self._aspectRatioScalar * np.ones(len(R))
         else:
             return self._aspectRatioScalar
+        
+    def setPrecipitateShape(self, precipitateShape, ar = 1):
+        '''
+        General shape setting function
+
+        Defualts to spherical
+        '''
+        if precipitateShape == ShapeFactor.NEEDLE:
+            self.setNeedleShape(ar)
+        elif precipitateShape == ShapeFactor.PLATE:
+            self.setPlateShape(ar)
+        elif precipitateShape == ShapeFactor.CUBIC:
+            self.setCuboidalShape(ar)
+        else:
+            self.setSpherical(ar)
             
     def setSpherical(self, ar = 1):
         '''
         Sets factors for spherical precipitates
         '''
         self.particleType = self.SPHERE
         self._eqRadiusEquation = self._eqRadiusFactorSphere
```

### Comparing `kawin-0.2.0/kawin/Strength.py` & `kawin-0.3.0/kawin/precipitation/coupling/Strength.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import numpy as np
+from kawin.precipitation.Plot import getTimeAxis
 
 class StrengthModel:
     '''
     Defines strength model
 
+    Following implementation described in
+    M.R. Ahmadi, E. Povoden-Karadeni, K.I. Oksuz, A. Falahati and E. Kozeschnik
+        Computational Materials Science 91 (2014) 173-186
+
     6 contributions are accounted for
     For dislocation cutting, contributions are coherency, modulus, anti-phase boundary, stacking fault energy and interfacial energy
     For dislocation bowing, contribution is orowan
 
     Contributions can be added for all phases or for a single phase
     '''
     def __init__(self):
@@ -61,27 +66,77 @@
         #Multi-phase superposition exponents
         self.multiphaseSameExp = 1.8
         self.multiphaseMixedExp = 1.4
 
         #Superposition exponent for total strength
         self.totalStrengthExp = 1.8
 
-    def _getStrengthFunctions(self):
+        #Strength terms
+        self.rss = None
+        self.ls = None
+        self.solidStrength = None
+
+    def save(self, filename, compressed = True):
+        '''
+        Saves strength model data
+
+        Note, this only saves solid solution strength, the rss and ls terms
+        Parameters should be free so user can load model and evaluate different parameters
+        '''
+        if compressed:
+            np.savez_compressed(filename, ssStrength=self.solidStrength, rss = self.rss, ls = self.ls)
+        else:
+            np.savez(filename, ssStrength=self.solidStrength, rss = self.rss, ls = self.ls)
+
+    def load(self, filename):
+        data = np.load(filename)
+        self.solidStrength = data['ssStrength']
+        self.rss = data['rss']
+        self.ls = data['ls']
+
+    def _getStrengthFunctions(self, selectedContributions = None):
         '''
         Internal function that creates arrays for dislocation cutting mechanisms
 
         wfuncs, sfuncs - list of functions for each contribution for weak and strong effects
         contributions - each contribution has a dictionary of str : boolean to say whether a phase has that contribution
         labels - labels for plotting
+
+        Parameters
+        ----------
+        selectedContributions : None or List[str]
+            If None, will return weak/strong functions and labels for all contributions
+            If List[str], will return weak/strong functions and labels for only the contributions defined in list
+                Options are: Coherency, Modulus, APB, SFE and/or Interfacial
+        
+        Returns
+        -------
+        wfuncs - List of functions for weak contributions
+        sfuncs - List of functions for strong contributions
+        contributions - List of {phase str:boolean} for whether the contribution is enabled
+        labels - List of labels for plotting
         '''
         wfuncs = [self.coherencyWeak, self.modulusWeak, self.APBweak, self.SFEweak, self.interfacialWeak]
         sfuncs = [self.coherencyStrong, self.modulusStrong, self.APBstrong, self.SFEstrong, self.interfacialStrong]
         contributions = [self.coherencyEffect, self.modulusEffect, self.APBEffect, self.SFEffect, self.IFEffect]
         labels = ['Coherency', 'Modulus', 'APB', 'SFE', 'Interfacial']
-        return wfuncs, sfuncs, contributions, labels
+        if selectedContributions is None:
+            return wfuncs, sfuncs, contributions, labels
+        else:
+            wfuncsSub, sfuncsSub, contributionsSub, labelsSub = [], [], [], []
+            lowerLabels = [l.lower() for l in labels]
+            for c in selectedContributions:
+                if c.lower() in lowerLabels:
+                    index = lowerLabels.index(c.lower())
+                    wfuncsSub.append(wfuncs[index])
+                    sfuncsSub.append(sfuncs[index])
+                    contributionsSub.append(contributions[index])
+                    labelsSub.append(labels[index])
+            return wfuncsSub, sfuncsSub, contributionsSub, labelsSub 
+        
 
     def setBaseStrength(self, sigma0):
         '''
         Sets base strength of matrix
 
         Parameters
         ----------
@@ -430,39 +485,42 @@
 
     def orowan(self, r, Ls):
         '''
         Orowan strengthening for non-shearable particles
         '''
         return self.J * self.G * self.b / (2 * np.pi * np.sqrt(1 - self.nu) * Ls) * np.log(2 * r / self.ri)
 
-    def ssStrength(self, model):
+    def ssStrength(self, model, n):
         '''
         Solid solution strength model
-        \sigma_ss = \sum{k_i * c_i^n}
+        sigma_ss = sum(k_i * c_i^n)
 
         Parameters
         ----------
         model : KWNEuler object
             Model to take composition from
 
         Returns
         -------
         strength : array of floats
             Solid solution strength contribution over time
         '''
-        if len(model.xComp.shape) == 1:
-            return self.ssweights[model.elements[0]] * model.xComp**self.ssexp
-        else:
-            return np.sum([self.ssweights[model.elements[i]]*model.xComp[:,i]**self.ssexp for i in range(len(model.elements))], axis=0)
+        val = 0
+        for i in range(len(model.elements)):
+            if model.elements[i] in self.ssweights:
+                val += self.ssweights[model.elements[i]]*model.xComp[n,i]**self.ssexp
+        return val
 
-    def rssterm(self, model, p, i):
+    def rssterm(self, model, p):
         '''
         Mean projected radius of particles
 
-        This function is inserted into a PrecipitateModel object as an additional output
+        r1 = first ordered moment of particle size distribution
+        r2 = second ordered moment of particle size distribution
+        rss = sqrt(2/3) * r2 / r1
 
         Parameters
         ----------
         model : PrecipitateModel
         p : int
             Phase index
         i : int
@@ -472,19 +530,22 @@
         r2 = np.sum(model.PBM[p].PSD * model.PBM[p].PSDsize**2)
         if r1 == 0:
             rss = 0
         else:
             rss = np.sqrt(2/3) * r2 / r1
         return rss
 
-    def Lsterm(self, model, p, i):
+    def Lsterm(self, model, p):
         '''
         Mean surface to surface distance between particles
 
-        This function is inserted into a PrecipitateModel object as an additional output
+        r1 = first ordered moment of particle size distribution
+        r2 = second ordered moment of particle size distribution
+        rss = sqrt(2/3) * r2 / r1
+        ls = sqrt(ln(3)/(2*pi*r1) + (2*rss)^2) - 2*rss
 
         Parameters
         ----------
         model : PrecipitateModel
         p : int
             Phase index
         i : int
@@ -494,88 +555,87 @@
         r2 = np.sum(model.PBM[p].PSD * model.PBM[p].PSDsize**2)
         if r1 == 0:
             Ls = 0
         else:
             rss = np.sqrt(2/3) * r2 / r1
             Ls = np.sqrt(np.log(3) / (2*np.pi*r1) + (2*rss)**2) - 2*rss
         return Ls
-
-    def insertStrength(self, model):
+    
+    def updateCoupledModel(self, model):
         '''
-        Inserts Fterm into the KWNmodel to be solved for
+        Computes rss, ls and solid solution strengthening terms
+        from current state of the PrecipitateModel
 
         Parameters
         ----------
-        model : KWNEuler object
+        model : PrecpitateModel
         '''
-        model.addAdditionalOutput(self.rssName, self.rssterm)
-        model.addAdditionalOutput(self.LsName, self.Lsterm)
+        if self.rss is None:
+            self.rss = np.zeros((1, len(model.phases)))
+            self.ls = np.zeros((1, len(model.phases)))
+            self.solidStrength = np.zeros(1)
+            self.solidStrength[0] = self.ssStrength(model, 0)
 
-    def getParticleSpacing(self, model, phase = None):
-        '''
-        Grabs mean projected radius and surface to surface distance from a PrecipitateModel
-
-        Parameters
-        ----------
-        model : PrecipitateModel
-        phase : str (optional)
-            Phase name, will default to first phase in the model
-        '''
-        index = model.phaseIndex(phase)
-        rss = model.getAdditionalOutput(self.rssName)[index]
-        Ls = model.getAdditionalOutput(self.LsName)[index]
-        return rss, Ls
+        self.rss = np.append(self.rss, [[self.rssterm(model, p) for p in range(len(model.phases))]], axis=0)
+        self.ls = np.append(self.ls, [[self.Lsterm(model, p) for p in range(len(model.phases))]], axis=0)
+        self.solidStrength = np.append(self.solidStrength, [self.ssStrength(model, model.n)], axis=0)
 
     def precStrength(self, model):
         '''
         Gets strength as a function of time
 
         Parameters
         ----------
         model : PrecipitateModel
         '''
-        rss = model.getAdditionalOutput(self.rssName)
-        Ls = model.getAdditionalOutput(self.LsName)
+        #rss = model.getAdditionalOutput(self.rssName)
+        #Ls = model.getAdditionalOutput(self.LsName)
+        rss = self.rss
+        Ls = self.ls
 
         ps = []
-        totalCompare = np.zeros(len(rss[0]))
+        totalCompare = np.zeros(len(rss[:,0]))
         for i in range(len(model.phases)):
-            weakContributions, strongContributions, orowan, _ = self.getStrengthContributions(rss[i], Ls[i], model.phases[i])
-            strength, compare = self.combineStrengthContributions(weakContributions, strongContributions, orowan, returnComparison=True)
+            weakContributions, strongContributions, orowan, _ = self.getStrengthContributions(rss[:,i], Ls[:,i], model.phases[i])
+            strength, compare, _ = self.combineStrengthContributions(weakContributions, strongContributions, orowan, returnComparison=True)
             compare[~np.isfinite(strength)] = 0
             strength[~np.isfinite(strength)] = 0
             ps.append(strength)
             totalCompare += np.array(compare, dtype='int')
         ps = np.array(ps)
         totalStrength = np.zeros(len(ps[0]))
         indices = (totalCompare == 0) | (totalCompare == len(model.phases))
         totalStrength[indices] = np.power(np.sum(np.power(ps[:,indices], self.multiphaseSameExp), axis=0), 1/self.multiphaseSameExp)
         totalStrength[~indices] = np.power(np.sum(np.power(ps[:,~indices], self.multiphaseMixedExp), axis=0), 1/self.multiphaseMixedExp)
         return totalStrength
 
-    def getStrengthContributions(self, rss, Ls, phase = 'all'):
+    def getStrengthContributions(self, rss, Ls, phase = 'all', selectedContributions=None):
         '''
         Gets strength contributions from a model
 
         Parameters
         ----------
         rss : array
             Mean projected radius
         Ls : array
             Mean surface to surface particle spacing
         phase : str (optional)
             Phase name
             Defaults to 'all'
+        selectedContributions : None or List[str]
+            If None, will return weak/strong functions and labels for all contributions
+            If List[str], will return weak/strong functions and labels for only the contributions defined in list
+                Options are: Coherency, Modulus, APB, SFE and/or Interfacial
         '''
         r0Weak = Ls / np.sqrt(np.cos(self.psi / 2))
         r0Strong = Ls
         weakContributions = []
         strongContributions = []
         contributionsList = []
-        wfuncs, sfuncs, contributions, ylabel = self._getStrengthFunctions()
+        wfuncs, sfuncs, contributions, ylabel = self._getStrengthFunctions(selectedContributions)
         for i in range(len(wfuncs)):
             if contributions[i]['all'] or (phase in contributions[i] and contributions[i][phase]):
                 with np.errstate(divide='ignore', invalid='ignore'):
                     if (phase in contributions[i] and contributions[i][phase]):
                         weakContributions.append(wfuncs[i](rss, Ls, r0Weak, phase))
                         strongContributions.append(sfuncs[i](rss, Ls, r0Strong, phase))
                     else:
@@ -585,15 +645,15 @@
         weakContributions = np.array(weakContributions)
         weakContributions[(weakContributions < 0) | ~np.isfinite(weakContributions)] = 0
         strongContributions = np.array(strongContributions)
         strongContributions[(strongContributions < 0) | ~np.isfinite(strongContributions)] = 0
         tauowo = np.array(self.orowan(rss, Ls))
         tauowo[~np.isfinite(tauowo)] = 0
         return weakContributions, strongContributions, tauowo, contributionsList
-
+    
     def combineStrengthContributions(self, weakContributions, strongContributions, orowan, returnComparison = False):
         '''
         Combines weak, strong and orowan contributions
 
         Parameters
         ----------
         weakContributions : 2D array
@@ -610,15 +670,15 @@
         tausumweak = np.zeros(orowan.shape) if len(weakContributions) == 0 else np.array(np.power(np.sum(np.power(weakContributions, self.singlePhaseExp), axis=0), 1/self.singlePhaseExp))
         tausumstrong = np.zeros(orowan.shape) if len(strongContributions) == 0 else np.array(np.power(np.sum(np.power(strongContributions, self.singlePhaseExp), axis=0), 1/self.singlePhaseExp))
         tausumweak[~np.isfinite(tausumweak)] = 0
         tausumstrong[~np.isfinite(tausumstrong)] = 0
         orowan[~np.isfinite(orowan)] = 0
         taumin = np.amin(np.array([tausumweak, tausumstrong, orowan]), axis=0)
         if returnComparison:
-            return self.M * taumin, (tausumweak > tausumstrong) & (tausumweak > orowan)
+            return self.M * taumin, (tausumweak > tausumstrong) & (tausumweak > orowan), (self.M * tausumweak, self.M * tausumstrong, self.M * orowan)
         else:
             return self.M * taumin
 
     def totalStrength(self, ssStrength, precStrength):
         '''
         Combined base strength, solid solution strength and precipitate strength
 
@@ -645,114 +705,124 @@
             yscale = 1e6
             ylabel = 'Strength (MPa)'
         elif strengthUnits.lower() == 'gpa':
             yscale = 1e9
             ylabel = 'Strength (GPa)'
         return yscale, ylabel
 
-    def plotPrecipitateStrengthOverR(self, ax, r, Ls, phase=None, strengthUnits = 'MPa', plotContributions = False, *args, **kwargs):
+    def plotPrecipitateStrengthOverR(self, ax, r, Ls, phase=None, strengthUnits = 'MPa', contribution = None, *args, **kwargs):
         '''
         Plots precipitate strength contribution as a function of radius
 
         Parameters
         ----------
         ax : Axis
         r : list
             Equivalent radius
         Ls : list
             Surface to surface particle distance
         strengthUnits : str
             Units for strength, options are 'Pa', 'kPa', 'MPa' or 'GPa'
-        plotContributions : bool
-            Whether to plot all contributions
+        contribution : None or str
+            If None, will plot overall strength
+            If str, will plot selected contribution or all contributions
+                Options are: Coherency, Modulus, APB, SFE or Interfacial
         '''
         if phase is None:
             phase = 'all'
 
-        self.plotPrecipitateStrengthOverX(ax, r, r, Ls, phase, strengthUnits, plotContributions, *args, **kwargs)
+        self.plotPrecipitateStrengthOverX(ax, r, r, Ls, phase, strengthUnits, contribution, *args, **kwargs)
+        ax.set_xlabel('Radius (m)')
 
-    def plotPrecipitateStrengthOverTime(self, ax, model, phase = None, bounds = None, timeUnits = 's', strengthUnits = 'MPa', plotContributions = False, *args, **kwargs):
+    def plotPrecipitateStrengthOverTime(self, ax, model, phase = None, bounds = None, timeUnits = 's', strengthUnits = 'MPa', contribution = None, *args, **kwargs):
         '''
         Plots precipitate strength contribution as a function of time
 
         Parameters
         ----------
         ax : Axis
         r : list
             Equivalent radius
         Ls : list
             Surface to surface particle distance
         strengthUnits : str
             Units for strength, options are 'Pa', 'kPa', 'MPa' or 'GPa'
-        plotContributions : bool
-            Whether to plot all contributions
-        '''
-        r, Ls = self.getParticleSpacing(model, phase)
+        contribution : None or str
+            If None, will plot overall strength
+            If str, will plot selected contribution or all contributions
+                Options are: Coherency, Modulus, APB, SFE or Interfacial
+        '''
+        timeScale, timeLabel, bounds = getTimeAxis(model, timeUnits, bounds)
+
+        self.plotPrecipitateStrengthOverX(ax, model.time*timeScale, self.rss, self.ls, phase, strengthUnits, contribution, *args, **kwargs)
+        ax.set_xlabel(timeLabel)
+        ax.set_xscale('log')
+        ax.set_xlim(bounds)
 
-        timeScale, timeLabel, bounds = model.getTimeAxis(timeUnits, bounds)
-
-        self.plotPrecipitateStrengthOverX(ax, model.time*timeScale, r, Ls, phase, strengthUnits, plotContributions, *args, **kwargs)
-        if plotContributions:
-            row, col = [0, 0, 1, 1, 2, 2], [0, 1, 0, 1, 0, 1]
-            for i in range(len(row)):
-                ax[row[i], col[i]].set_xlabel(timeLabel)
-                ax[row[i], col[i]].set_xscale('log')
-        else:
-            ax.set_xlabel(timeLabel)
-            ax.set_xscale('log')
-
-    def plotPrecipitateStrengthOverX(self, ax, x, r, Ls, phase = None, strengthUnits = 'MPa', plotContributions = False, *args, **kwargs):
+    def plotPrecipitateStrengthOverX(self, ax, x, r, Ls, phase = None, strengthUnits = 'MPa', contribution = None, *args, **kwargs):
         '''
         Plots precipitate strength contribution as a function of x
 
+        TODO: make this a bit more generalized where you can set the contribution you want to plot
+            This should also remove the restriction that axes subplot must be 3x2
+
         Parameters
         ----------
         ax : Axis
         x : list
             X coordinates to plot against
         r : list
             Equivalent radius, must correspond to x
         Ls : list
             Surface to surface particle distance, must correspond to x
         strengthUnits : str
             Units for strength, options are 'Pa', 'kPa', 'MPa' or 'GPa'
-        plotContributions : bool
-            Whether to plot all contributions
+        contribution : None or str
+            If None, will plot overall strength
+            If str, will plot selected contribution or all contributions
+                Options are: Coherency, Modulus, APB, SFE, Interfacial, Orowan or All
         '''
         yscale, ylabel = self.getStrengthUnits(strengthUnits)
-        if plotContributions:
-            _, _, _, ylabel = self._getStrengthFunctions()
-            row, col = [0, 0, 1, 1, 2], [0, 1, 0, 1, 0]
-            weak, strong, oro, contributionList = self.getStrengthContributions(r, Ls, phase)
-            for i in range(len(row)):
-                if ylabel[i] in contributionList:
-                    index = contributionList.index(ylabel[i])
-                    ax[row[i], col[i]].plot(x, self.M * weak[index] / yscale, x, self.M * strong[index] / yscale, *args, **kwargs)
-                    ax[row[i], col[i]].legend(['Weak', 'Strong'])
-                    ax[row[i], col[i]].set_ylim(bottom=0)
+        if contribution is not None:
+            if contribution.lower() == 'orowan':
+                tauowo = np.array(self.orowan(r, Ls))
+                tauowo[~np.isfinite(tauowo)] = 0
+                ax.plot(x, self.M * tauowo / yscale, *args, **kwargs)
+                ax.set_ylabel(r'$\tau_{orowan}$ (' + strengthUnits + ')')
+                ax.set_ylim(bottom=0)
+                ax.set_xlim([x[0], x[-1]])
+
+            elif contribution.lower() != 'all':
+                _, _, _, ylabel = self._getStrengthFunctions([contribution])
+                weak, strong, oro, contributionList = self.getStrengthContributions(r, Ls, phase, [contribution])
+                if ylabel[0] in contributionList:
+                    ax.plot(x, self.M * weak[0] / yscale, x, self.M * strong[0] / yscale, *args, **kwargs)
+                    ax.set_ylim(bottom=0)
+                    ax.legend(['Weak', 'Strong'])
                 else:
-                    ax[row[i], col[i]].plot(x, np.zeros(len(x)), *args, **kwargs)
-                    ax[row[i], col[i]].set_ylim([-1, 1])
-                ax[row[i], col[i]].set_xlabel('Radius (m)')
-                ax[row[i], col[i]].set_ylabel(r'$\tau_{' + ylabel[i] + '}$ (' + strengthUnits + ')')
-                ax[row[i], col[i]].set_xlim([x[0], x[-1]])
-
-            #If no contributions exists for shearable precipitates, then wtot and stot is 0
-            wtot = np.zeros(len(x)) if len(weak) == 0 else np.array(np.power(np.sum(np.power(weak, self.singlePhaseExp), axis=0), 1/self.singlePhaseExp))
-            stot = np.zeros(len(x)) if len(strong) == 0 else np.array(np.power(np.sum(np.power(strong, self.singlePhaseExp), axis=0), 1/self.singlePhaseExp))
-            smin = np.amin([wtot, stot, oro], axis=0)
-            ax[2,1].plot(x, self.M * wtot/yscale, x, self.M * stot/yscale, x, self.M * oro/yscale, x, self.M * smin/yscale, *args, **kwargs)
-            ax[2,1].set_ylim(bottom=0)
-            ax[2,1].set_ylabel(r'$\tau$ (' + strengthUnits + ')')
-            ax[2,1].set_xlabel('Radius (m)')
-            ax[2,1].legend(['Weak', 'Strong', 'Orowan', 'Minimum'])
-            ax[2,1].set_xlim([x[0], x[-1]])
+                    ax.plot(x, np.zeros(len(x)), *args, **kwargs)
+                    ax.set_ylim([-1, 1])
+                ax.set_ylabel(r'$\tau_{' + ylabel[0] + '}$ (' + strengthUnits + ')')
+                ax.set_xlim([x[0], x[-1]])
+
+            else:
+                _, _, _, ylabel = self._getStrengthFunctions()
+                weak, strong, oro, contributionList = self.getStrengthContributions(r, Ls, phase)
+                strength, _, summedContributions = self.combineStrengthContributions(weak, strong, oro, returnComparison=True)
+                wtot, stot, oro = summedContributions
+
+                ax.plot(x, wtot/yscale, x, stot/yscale, x, oro/yscale, x, strength/yscale, *args, **kwargs)
+                ax.set_ylim(bottom=0)
+                ax.set_ylabel(r'$\tau$ (' + strengthUnits + ')')
+                ax.legend(['Weak', 'Strong', 'Orowan', 'Minimum'])
+                ax.set_xlim([x[0], x[-1]])
+            
 
         else:
-            weak, strong, oro, contributionList = self.getStrengthContributions(r, Ls, Leff, Ls, phase)
+            weak, strong, oro, contributionList = self.getStrengthContributions(r, Ls, phase)
             strength = self.combineStrengthContributions(weak, strong, oro)
             ax.plot(x, strength / yscale, *args, **kwargs)
             ax.set_ylabel('Yield ' + ylabel)
             ax.set_ylim(bottom=0)
             ax.set_xlim([x[0], x[-1]])
 
     def plotStrength(self, ax, model, plotContributions = False, bounds = None, timeUnits = 's', strengthUnits = 'MPa', *args, **kwargs):
@@ -768,19 +838,20 @@
         bounds : tuple or None
             Bounds on time axis (if None, the bounds will automatically be set)
         timeUnits : str
             Units of time to plot in, options are 's' for seconds, 'm' for minutes or 'h' for hours
         strengthUnits : str
             Units for strength, options are 'Pa', 'kPa', 'MPa' or 'GPa'
         '''
-        timeScale, timeLabel, bounds = model.getTimeAxis(timeUnits, bounds)
+        timeScale, timeLabel, bounds = getTimeAxis(model, timeUnits, bounds)
         yscale, ylabel = self.getStrengthUnits(strengthUnits)
 
         sigma0 = self.sigma0 * np.ones(len(model.time))
-        ssStrength = self.ssStrength(model) if len(self.ssweights) > 0 else np.zeros(len(model.time))
+        #ssStrength = self.ssStrength(model) if len(self.ssweights) > 0 else np.zeros(len(model.time))
+        ssStrength = self.solidStrength
         precStrength = self.precStrength(model)
 
         total = self.totalStrength(ssStrength, precStrength)
 
         ax.plot(model.time*timeScale, total / yscale, *args, **kwargs)
 
         if plotContributions:
```

### Comparing `kawin-0.2.0/kawin/Surrogate.py` & `kawin-0.3.0/kawin/thermo/Thermodynamics.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1576 +1,1334 @@
 import numpy as np
-import pickle
-from scipy.interpolate import Rbf
-import scipy.spatial.distance as spd
+from pycalphad import Model, Database, calculate, equilibrium, variables as v
+from pycalphad.codegen.callables import build_callables, build_phase_records
+from pycalphad.core.composition_set import CompositionSet
+from pycalphad.core.utils import extract_parameters
+from kawin.thermo.Mobility import MobilityModel, inverseMobility, inverseMobility_from_diffusivity, tracer_diffusivity, tracer_diffusivity_from_diff
+from kawin.thermo.FreeEnergyHessian import dMudX
+from kawin.thermo.LocalEquilibrium import local_equilibrium
+import matplotlib.pyplot as plt
+import copy
+from tinydb import where
 
-def generateTrainingPoints(*arrays):
-    '''
-    Creates all combinations of inputted arrays
-    Used for creating training points in composition space for
-    MulticomponentSurrogate
+setattr(v, 'GE', v.StateVariable('GE'))
 
-    Parameters
-    ----------
-    arrays - arrays along each dimension
-        Order of arrays should correspond to the order of elements when defining thermodynamic functions
+class ExtraGibbsModel(Model):
     '''
-    return np.array(np.meshgrid(*arrays)).T.reshape(-1, len(arrays))
+    Child of pycalphad Model with extra variable GE
+        GE represents any extra contribution to the Gibbs free energy
+        such as the Gibbs-Thomson contribution
+    '''
+    energy = GM = property(lambda self: self.ast + v.GE)
+    formulaenergy = G = property(lambda self: (self.ast + v.GE) * self._site_ratio_normalization)
+    orderingContribution = OCM = property(lambda self: self.models['ord'])
 
-def _filter_points(inputs, outputs, tol = 1e-3):
+class GeneralThermodynamics:
     '''
-    Filter set of input points such that the closest distance is above tolerance
-    This is to avoid non-positive definite training matrices when creating surrogate models
+    Class for defining driving force and essential functions for
+    binary and multicomponent systems using pycalphad for equilibrium
+    calculations
 
     Parameters
     ----------
-    inputs : m x n matrix of floats
-        Input points of m observations in n-dimensional space
-    outputs : list of array of floats
-        Output points, each array must be m x n where
-            m is number of observations and n is dimensions of output
-    tol : float
-        Tolerance for distance between two input points
-
-    Outputs
-    -------
-    (filtered inputs, filtered outputs)
-    filtered inputs - array of input points
-    filtered outputs - array of output points
+    database : Database or str
+        pycalphad Database or file name for database
+    elements : list
+        Elements to consider
+        Note: reference element must be the first index in the list
+    phases : list
+        Phases involved
+        Note: matrix phase must be first index in the list
+    drivingForceMethod : str (optional)
+        Method used to calculate driving force
+        Options are 'tangent' (default), 'approximate', 'sampling' and 'curvature' (not recommended)
+    parameters : list [str] or dict {str : float} or None
+        List of parameters to keep symbolic in the thermodynamic or mobility models
+        If None, then parameters are fixed
     '''
-    #Make distance matrix
-    distance = spd.squareform(spd.pdist(inputs))
-
-    #Indices to remove
-    indices = np.where((distance > 0) & (distance <= tol))
-    indices = np.unique(indices[0][indices[0] < indices[1]])
-
-    newInputs = np.delete(inputs, indices, axis=0)
-    newOutputs = []
-    for i in range(len(outputs)):
-        newOutputs.append(np.delete(outputs[i], indices, axis=0))
 
-    return newInputs, newOutputs
+    gOffset = 1      #Small value to add to precipitate phase for when order/disorder models are used
 
-class BinarySurrogate:
-    '''
-    Handles surrogate models for driving force, interfacial composition and
-    diffusivity in a binary system
-    
-    Parameters
-    ----------
-    binaryThermodynamics - BinaryThermodynamics (optional)
-        Driving force and interfacial composition will be taken from this if not explicitly defined
-        If None, then drivingForce and interfacialComposition must be defined
-        
-    drivingForce - function (optional)
-        Function will take in (composition, temperature) and return driving force,
-            where a positive value means that precipitation is favorable
-        
-    interfacialComposition - function (optional)
-        Function will take in (temperature, excess gibbs free energy) and
-            return tuple (parent composition, precipitate composition) or (None, None) if precipitate is unstable
+    def __init__(self, database, elements, phases, drivingForceMethod = 'tangent', parameters = None):
+        if isinstance(database, str):
+            database = Database(database)
+        self.db = database
+        self.elements = copy.copy(elements)
+        if parameters is None:
+            self._parameters = {}
+        else:
+            if isinstance(parameters, list):
+                self._parameters = {p: 0 for p in parameters}
+            else:
+                self._parameters = parameters
 
-    diffusivity - function (optional)
-        Function will take in (composition, temperature) and return diffusivity
+        if 'VA' not in self.elements:
+            self.elements.append('VA')
 
-    precPhase : str (optional)
-        Precipitate phase to consider if binaryThermodynamics is defined
+        if type(phases) == str:  # check if a single phase was passed as a string instead of a list of phases.
+            phases = [phases]
+        self.phases = phases
+
+        self._buildThermoModels()
+
+        #Amount of points to sample per degree of freedom
+        # sampling_pDens is for when using sampling method in driving force calculations
+        # pDens is for equilibrium calculations
+        self.sampling_pDens = 2000
+        self.pDens = 500
+
+        #Stored variables of last time the class was used
+        #This is so that these can be used again if the temperature has not changed since last usage
+        self._prevTemperature = None
+
+        #Pertains to parent phase (composition, sampled points, equilibrium calculations)
+        self._prevX = None
+        self._parentEq = None
+
+        #Pertains to precipitate phases (sampled points)
+        self._pointsPrec = {self.phases[i]: None for i in range(1, len(self.phases))}
+        self._orderingPoints = {self.phases[i]: None for i in range(1, len(self.phases))}
+
+        self.setDrivingForceMethod(drivingForceMethod)
+
+        self._buildMobilityModels()
+
+        #Cached results
+        self._compset_cache = {}
+        self._compset_cache_df = {}
+        self._matrix_cs = None
+
+    def _buildThermoModels(self):
+        '''
+        Builds thermodynamic models for each phase
+
+        This assumes that the first phase is the parent phase and the rest of the phases are precipitate phases
+            For usage in a diffusion model, this won't affect anything
+
+        For each precipitate phase, it checks whether the phase has an order/disorder contribution
+            If so, then it checks if the disorder contribution comes from the parent phase (ex. gamma and gamma prime in Ni alloys)
+            An ordering contribution phase record will be created to allow separated between the parent and the ordered phase
+        '''
+        self.orderedPhase = {self.phases[i]: False for i in range(1, len(self.phases))}
+        for i in range(1, len(self.phases)):
+            if 'disordered_phase' in self.db.phases[self.phases[i]].model_hints:
+                if self.db.phases[self.phases[i]].model_hints['disordered_phase'] == self.phases[0]:
+                    self.orderedPhase[self.phases[i]] = True
+                    self._forceDisorder(self.phases[0])
+
+        #Build phase models assuming first phase is parent phase and rest of precipitate phases
+        #If the same phase is used for matrix and precipitate phase, then force the matrix phase to remove the ordering contribution
+        #This may be unnecessary as already disordered phase models will not be affected, but I guess just in case the matrix phase happens to be an ordered solution
+        param_keys, _ = extract_parameters(self._parameters)
+        self.models = {self.phases[0]: Model(self.db, self.elements, self.phases[0], parameters=param_keys)}
+        self.models[self.phases[0]].state_variables = sorted([v.T, v.P, v.N, v.GE], key=str)
+
+        for i in range(1, len(self.phases)):
+            self.models[self.phases[i]] = ExtraGibbsModel(self.db, self.elements, self.phases[i], parameters=param_keys)
+            self.models[self.phases[i]].state_variables = sorted([v.T, v.P, v.N, v.GE], key=str)
+
+        self.phase_records = build_phase_records(self.db, self.elements, self.phases,
+                                                 self.models[self.phases[0]].state_variables,
+                                                 self.models, build_gradients=True, build_hessians=True,
+                                                 parameters=self._parameters)
+
+        self.OCMphase_records = {}
+        for i in range(1, len(self.phases)):
+            if self.orderedPhase[self.phases[i]]:
+                self.OCMphase_records[self.phases[i]] = build_phase_records(self.db, self.elements, [self.phases[i]],
+                                                                            self.models[self.phases[0]].state_variables,
+                                                                            {self.phases[i]: self.models[self.phases[i]]},
+                                                                            output='OCM', build_gradients=False, build_hessians=False, 
+                                                                            parameters=self._parameters)
+                
+    def _buildMobilityModels(self):
+        '''
+        Builds mobility models for phases that have model parameters
+        '''
+        self.mobModels = {p: None for p in self.phases}
+        self.mobCallables = {p: None for p in self.phases}
+        self.diffCallables = {p: None for p in self.phases}
+        param_keys, _ = extract_parameters(self._parameters)
+        for p in self.phases:
+            #Get mobility/diffusivity of phase p if exists
+            param_search = self.db.search
+            param_query_mob = (
+                (where('phase_name') == p) & \
+                (where('parameter_type') == 'MQ') | \
+                (where('parameter_type') == 'MF')
+            )
+
+            param_query_diff = (
+                (where('phase_name') == p) & \
+                (where('parameter_type') == 'DQ') | \
+                (where('parameter_type') == 'DF')
+            )
+
+            pMob = param_search(param_query_mob)
+            pDiff = param_search(param_query_diff)
+
+            if len(pMob) > 0 or len(pDiff) > 0:
+                self.mobModels[p] = MobilityModel(self.db, self.elements, p, parameters=param_keys)
+                if len(pMob) > 0:
+                    self.mobCallables[p] = {}
+                    for c in self.phase_records[p].nonvacant_elements:
+                        bcp = build_callables(self.db, self.elements, [p], {p: self.mobModels[p]},
+                                            parameter_symbols=self._parameters, output='MOB_'+c, build_gradients=False, build_hessians=False,
+                                            additional_statevars=[v.T, v.P, v.N, v.GE])
+                        self.mobCallables[p][c] = bcp['MOB_'+c]['callables'][p]
+                else:
+                    self.diffCallables[p] = {}
+                    for c in self.phase_records[p].nonvacant_elements:
+                        bcp = build_callables(self.db, self.elements, [p], {p: self.mobModels[p]},
+                                            parameter_symbols=self._parameters, output='DIFF_'+c, build_gradients=False, build_hessians=False,
+                                            additional_statevars=[v.T, v.P, v.N, v.GE])
+                        self.diffCallables[p][c] = bcp['DIFF_'+c]['callables'][p]
 
-    Note: if binaryThermodynamics is not defined, then drivingForce and
-        interfacial composition needs to be defined
-    '''
-    def __init__(self, binaryThermodynamics = None, drivingForce = None, interfacialComposition = None, diffusivity = None, precPhase = None):
-        self.binTherm = binaryThermodynamics
-        self.precPhase = precPhase
-        
-        #If no driving force or interfacial composition function is supplied, then use function from thermodynamics class
-        if drivingForce is None:
-            self.drivingForceFunction = lambda x, T, returnComp=False, training = True: self.binTherm.getDrivingForce(x, T, self.precPhase, returnComp, training)
-        else:
-            self.drivingForceFunction = drivingForce
-        
-        if interfacialComposition is None:
-            self.interfacialCompositionFunction = lambda T, ge: self.binTherm.getInterfacialComposition(T, ge, self.precPhase)
-        else:
-            self.interfacialCompositionFunction = interfacialComposition
+        #This applies to all phases since this is typically reflective of quenched-in vacancies
+        self.mobility_correction = {A: 1 for A in self.elements}
 
-        if binaryThermodynamics is not None:
-            self.diffusivityFunction = self.binTherm.getInterdiffusivity
-        elif diffusivity is not None:
-            self.diffusivityFunction = diffusivity
-
-        self.eps = 1e-3
-
-        #Driving force variables -----------------------------------------
-        #Training data points
-        self.drivingForce = []
-        self.precComp = []
-        self.dGcoords = []
-        self.precCompIndices = []
-        self.precCompCoords = []
-
-        #Scaling factor to normalize distance
-        self.XDGscale = None
-        self.TDGscale = None
-
-        #Surrogates
-        self.DGfunction = 'linear'
-        self.DGepsilon = 1
-        self.DGsmooth = 0
-        self.linearDG = True
-        self.LogSurrDG = None
-        self.LogSurrPrecComp = None
-        self.SurrogateDrivingForce = None
-        self.SurrogatePrecComp = None
-
-        #Interfacial composition -----------------------------------------
-        #Training data
-        self.xParent = []
-        self.xPrec = []
-        self.ICcoords = []
-        self.uniqueXPrec = []
-        self.Gcoords = []
-        self.G = []
-        
-        #Scaling factor to normalize distance
-        self.TICscale = None
-        self.GICscale = None
-        self.XGscale = None
-        
-        #Surrogates
-        self.ICfunction = 'linear'
-        self.ICepsilon = 1
-        self.ICsmooth = 0
-        self.linearIC = True
-        self.SurrogateParent = None
-        self.SurrogatePrec = None
-        self.SurrogateG = None
-        self.LogSurrParent = None
-        self.LogSurrPrec = None
-
-        #Diffusivity -----------------------------------------------------
-        #Training data
-        self.Diffcoords = []
-        self.Diff = []
-
-        #Scaling factor
-        #Scale temperature and free energy range is proportional to amount of data along given axis
-        self.XDiffscale = None
-        self.singleXDiff = False
-        self.TDiffscale = None
-
-        #Surrogates
-        self.linearDiff = False
-        self.Difffunction = 'linear'
-        self.Diffepsilon = 1
-        self.Diffsmooth = 0
-        self.SurrogateDiff = None
-        self.LogSurrDiff = None
-        
-        
-    def trainDrivingForce(self, comps, temperature, function='linear', epsilon=1, smooth=0, scale='linear'):
+    def updateParameters(self, parameters):
         '''
-        Creates training points and sets up surrogate models for driving force calculations
-        
+        Update parameter dictionary with new values
+
         Parameters
         ----------
-        comps : array of floats
-            Range of compositions for training points
-        temperature : float or array
-            Temperature or range of temperatures for training points
-        function : str (optional)
-            Radial basis function to use (defaults to 'linear')
-            Other functions are 'multiquadric', 'inverse_multiquadric',
-                'gaussian', 'cubic', 'quintic' and 'thin_plate'
-        epsilon : float
-            Scale for radial basis function (defaults to 1)
-            Training data will be scaled automatically
-                such that optimal scale is around 1
-        smooth : float
-            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
-        scale : float
-            Whether the composition training data should be in log or linear scale
-            Note: 'log' is recommended for dilute solutions
-        '''
-        #Convert temperature to array if not so
-        if not hasattr(temperature, '__len__'):
-            temperature = [temperature]
-        
-        #Ensure that composition are defined values if in log scale
-        if scale == 'log':
-            comps[comps == 0] = 1e-9
-        
-        self.drivingForce = []
-        self.precComp = []
-        self.dGcoords = []
-        self.precCompIndices = []
-        
-        #Create training data
-        n = 0   #Index for precCompIndices (needs to correspond to indices self.drivingForce array)
-        for t in temperature:
-            for x in comps:
-                dG, xP = self.drivingForceFunction(x, t, returnComp = True)
-
-                #If driving force can be obtained (generally True)
-                if dG is not None:
-                    self.drivingForce.append(dG)
-                    self.dGcoords.append([x, t])
-                    
-                    #If driving force is positive, then store nucleate composition
-                    if xP is not None:
-                        self.precComp.append(xP)
-                        self.precCompIndices.append(n)
-                    
-                    n += 1
-
-        self.dGcoords = np.array(self.dGcoords)   
-        self.drivingForce = np.array(self.drivingForce)
-        self.precComp = np.array(self.precComp)
-        self.precCompIndices = np.array(self.precCompIndices)
-        
-        #Log scale
-        if scale == 'log':
-            self.dGcoords[:,0] = np.log10(self.dGcoords[:,0])
-        
-        #Scale data so that it the range is proportional to the amount of data points along the given axis
-        if len(comps) == 1:
-            self.XDGscale = 1
-        else:
-            self.XDGscale = (np.amax(self.dGcoords[:,0]) - np.amin(self.dGcoords[:,0])) / len(comps)
-            self.dGcoords[:,0] /= self.XDGscale
-            
-        if len(temperature) == 1:
-            self.TDGscale = 1
-        else:
-            self.TDGscale = (np.amax(self.dGcoords[:,1]) - np.amin(self.dGcoords[:,1])) / len(temperature)
-            self.dGcoords[:,1] /= self.TDGscale
+        parameters : dict {str : float}
+            Dictionary of parameters
+            NOTE: this does not have to be the full list and can also have other parameters in it
+                Only the parameters that are stored upon initialization will be changed
+        '''
+        for pm in parameters:
+            if pm in self._parameters:
+                self._parameters[pm] = parameters[pm]
 
-        #Create new array of coordinates for precipitate composition (this is to allow for filtering)
-        self.precCompCoords = self.dGcoords[self.precCompIndices]
+        param_keys, param_values = extract_parameters(self._parameters)
+        for p in self.phases:
+            self.phase_records[p].parameters[:] = np.asarray(param_values, dtype=np.float_)
 
-        #Filter points such that all points are separated by a distance by at least self.eps
-        self.dGcoords, outputs = _filter_points(self.dGcoords, [self.drivingForce], self.eps)
-        self.drivingForce = outputs[0]
-        
-        self.precCompCoords, outputs = _filter_points(self.precCompCoords, [self.precComp], self.eps)
-        self.precComp = outputs[0]
+    def _forceDisorder(self, phase):
+        '''
+        For phases using an order/disorder model, pycalphad will neglect the disordered phase unless
+        it is the only phase set active, so the order and disordered portion of the phase will use the same model
 
-        if scale == 'log':
-            self.linearDG = False
-        else:
-            self.linearDG = True
-        self.DGfunction = function
-        self.DGepsilon = epsilon
-        self.DGsmooth = np.amax([smooth, self.eps])
-        
-        self._createDGSurrogate()
+        For the Gibbs-Thomson effect to be applied, the ordered and disordered parts of the model will need to be kept separate
+        As a fix, a new phase is added to the database that uses only the disordered part of the model
+        '''
+        newPhase = 'DIS_' + phase
+        self.phases[0] = newPhase
+        self.db.phases[newPhase] = copy.deepcopy(self.db.phases[phase])
+        self.db.phases[newPhase].name = newPhase
+        del self.db.phases[newPhase].model_hints['ordered_phase']
+        del self.db.phases[newPhase].model_hints['disordered_phase']
+
+        #Copy database parameters with new name
+        param_query = where('phase_name') == phase
+        params = self.db.search(param_query)
+        for p in params:
+            #We have to create a new dictionary since p is a TinyDB.Document
+            newP = {}
+            for entry in p:
+                newP[entry] = p[entry]
+            newP['phase_name'] = newPhase
+            self.db._parameters.insert(newP)
 
-    def _createDGSurrogate(self):
+    def clearCache(self):
         '''
-        Build surrogates for driving force
+        Removes any cached data
+        This is intended for surrogate training, where the cached data
+        will be removed incase
         '''
-        if self.linearDG:
-            self.SurrogateDrivingForce = Rbf(self.dGcoords[:,0], self.dGcoords[:,1], self.drivingForce, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
-            self.SurrogatePrecComp = Rbf(self.precCompCoords[:,0], self.precCompCoords[:,1], self.precComp, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
-        else:
-            self.linearDG = False
-            self.LogSurrDG = Rbf(self.dGcoords[:,0], self.dGcoords[:,1], self.drivingForce, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
-            self.LogSurrPrecComp = Rbf(self.precCompCoords[:,0], self.precCompCoords[:,1], self.precComp, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
-            self.SurrogateDrivingForce = lambda x, T: self.LogSurrDG(np.log10(x) / self.XDGscale, T)
-            self.SurrogatePrecComp = lambda x, T: self.LogSurrPrecComp(np.log10(x) / self.XDGscale, T)
-
-    def changeDrivingForceHyperparameters(self, function = 'linear', epsilon = 1, smooth = 0):
-        '''
-        Re-create surrogate model for driving force with updated hyperparameters
+        self._compset_cache = {}
+        self._compset_cache_df = {}
+        self._matrix_cs = None
 
-        Parameters
-        ----------
-        function : str (optional)
-            Radial basis function to use (defaults to 'linear')
-            Other functions are 'multiquadric', 'inverse_multiquadric',
-                'gaussian', 'cubic', 'quintic' and 'thin_plate'
-        epsilon : float
-            Scale for radial basis function (defaults to 1)
-            Training data will be scaled automatically
-                such that optimal scale is around 1
-        smooth : float
-            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
-        '''
-        if self.TDGscale is None:
-            raise Exception("Driving force has not been trained.")
-
-        self.DGfunction = function
-        self.DGepsilon = epsilon
-        self.DGsmooth = np.amax([smooth, self.eps])
-        
-        self._createDGSurrogate()            
-        
-    def getDrivingForce(self, x, T, returnComp = False):
+    def setDrivingForceMethod(self, drivingForceMethod):
         '''
-        Gets driving force from surrogate models
-        
+        Sets method for calculating driving force
+
         Parameters
         ----------
-        x : float or array of floats
-            Composition
-        T : float or array of floats
-            Temperature, must be same length as x
-        returnComp : bool (optional)
-            Returns precipitate composition if True (defaults to False)
-        
-        Returns
-        -------
-        (driving force, precipitate composition)
-        Both will be same shape as x and T
-        Positive driving force means that precipitate will form
-        precipitate composition will be None if returnComp is False
-        '''
-        if self.TDGscale is None:
-            raise Exception("Driving force has not been trained.")
-
-        #Convert arrays to Numpy arrays for math operations
-        if hasattr(x, '__len__'):
-            x = np.array(x)
-        if hasattr(T, '__len__'):
-            T = np.array(T)
-
-        if self.linearDG:
-            dG = self.SurrogateDrivingForce(x / self.XDGscale, T / self.TDGscale)
-            
-            if returnComp:
-                xP = self.SurrogatePrecComp(x / self.XDGscale, T / self.TDGscale)
-                return dG, xP
-            else:
-                if hasattr(dG, '__len__'):
-                    return dG, np.full(dG.shape, None)
-                else:
-                    return dG, None
-                
+        drivingForceMethod - str
+            Options are ['approximate', 'sampling', 'curvature']
+        '''
+        if drivingForceMethod == 'approximate':
+            self._drivingForce = self._getDrivingForceApprox
+        elif drivingForceMethod == 'sampling':
+            self._drivingForce = self._getDrivingForceSampling
+        elif drivingForceMethod == 'curvature':
+            self._drivingForce = self._getDrivingForceCurvature
+        elif drivingForceMethod == 'tangent':
+            self._drivingForce = self._getDrivingForceTangent
         else:
-            dG = self.SurrogateDrivingForce(x, T / self.TDGscale)
-            
-            if returnComp:
-                xP = self.SurrogatePrecComp(x, T / self.TDGscale)
+            raise Exception('Driving force method must be either \'approximate\', \'sampling\', \'tangent\' or \'curvature\'')
 
-                return dG, xP
-            else:
-                if hasattr(dG, '__len__'):
-                    return dG, np.full(dG.shape, None)
-                else:
-                    return dG, None
-        
-    def trainInterfacialComposition(self, temperature, freeEnergy, function='linear', epsilon=1, smooth=0, scale = 'linear'):
+    def setDFSamplingDensity(self, density):
         '''
-        Creates training points and sets up surrogate models for interfacial composition
+        Sets sampling density for sampling method in driving
+        force calculations
+
+        Default upon initialization is 2000
 
         Parameters
         ----------
-        temperature : float or array
-            Temperature or range of temperatures for training points
-        freeEnergy : array of floats
-            range of free energy values from Gibbs-Thomson contribution
-        function : str (optional)
-            Radial basis function to use (defaults to 'linear')
-            Other functions are 'multiquadric', 'inverse_multiquadric',
-                'gaussian', 'cubic', 'quintic' and 'thin_plate'
-        epsilon : float
-            Scale for radial basis function (defaults to 1)
-            Training data will be scaled automatically
-                such that optimal scale is around 1
-        smooth : float
-            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
-        scale : float
-            Whether the matrix composition output should be in log or linear scale
-            Note: 'log' is recommended for dilute solutions
-        '''
-        #Make temperature an array if not so
-        if not hasattr(temperature, '__len__'):
-            temperature = [temperature]
-        
-        self.xParent = []
-        self.xPrec = []
-        self.ICcoords = []
-        
-        #Create training data
-        for t in temperature:
-            for g in freeEnergy:
-                xM, xP = self.interfacialCompositionFunction(t, g)
-                
-                #If precipitate can be form at T,G, then add to training array
-                if xM is not None and xM > 0:
-                    self.xParent.append(xM)
-                    self.xPrec.append(xP)
-                    
-                    self.ICcoords.append([t, g])
-                    
-        self._buildInterfacialCompositionModels(temperature, freeEnergy, function, epsilon, smooth, scale)
-        
-    def trainInterfacialCompositionFromDrivingForceData(self, function='linear', epsilon=1, smooth=0, scale='linear'):
+        density : int
+            Number of samples to take per degree of freedom in the phase
         '''
-        Converts driving force data ([x, T] -> G) to interfacial composition data ([T, G] -> x)
-        This may lead to inaccuracies in the precipitate composition since driving force calculations are done by sampling the free energy curve
+        self._pointsPrec = {self.phases[i]: None for i in range(1, len(self.phases))}
+        self.sampling_pDens = density
 
-        Parameters
-        ----------
-        function : str (optional)
-            Radial basis function to use (defaults to 'linear')
-            Other functions are 'multiquadric', 'inverse_multiquadric',
-                'gaussian', 'cubic', 'quintic' and 'thin_plate'
-        epsilon : float
-            Scale for radial basis function (defaults to 1)
-            Training data will be scaled automatically
-                such that optimal scale is around 1
-        smooth : float
-            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
-        scale : float
-            Whether the matrix composition output should be in log or linear scale
-            Note: 'log' is recommended for dilute solutions
+    def setEQSamplingDensity(self, density):
         '''
-        self.xPrec = [x for x in self.precComp]
-        
-        #Take driving force training data and convert to interfacial composition training data
-        if self.linearDG:
-            self.xParent = [self.dGcoords[i, 0] * self.XDGscale for i in self.precCompIndices]
-        else:
-            self.xParent = [10**self.dGcoords[i, 0] * self.XDGscale for i in self.precCompIndices]
-            
-        self.ICcoords = []
-        for i in self.precCompIndices:
-            self.ICcoords.append([self.dGcoords[i, 1] * self.TDGscale, self.drivingForce[i]])
-        
-        self._buildInterfacialCompositionModels(np.unique(self.dGcoords[:, 1]) * self.TDGscale, self.drivingForce, function, epsilon, smooth, scale)
-                    
-    def _buildInterfacialCompositionModels(self, temperature, freeEnergy, function, epsilon, smooth, scale):
-        '''
-        Builds interfacial composition model (this is separate to allow for both training from new data or driving force data)
+        Sets sampling density for equilibrium calculations
+
+        Default upon initialization is 500
 
         Parameters
         ----------
-        temperature - range of temperatures
-        freeEnergy - range of free energies
-        function - radial basis function
-        epsilon - scale factor
-        smooth - smoothing factor
-        scale - linear or log scale
-        '''
-        #Create new training points finding the driving force for precipitation at the precipitate composition
-        self.uniqueXPrec = np.unique(self.xPrec)
-        if np.amax(self.uniqueXPrec) - np.amin(self.uniqueXPrec) < 1e-4:
-            self.uniqueXPrec = np.array([self.uniqueXPrec[0]])
-        self.Gcoords = []
-        self.G = []
-        
-        for t in temperature:
-            for x in self.uniqueXPrec:
-                #Driving force calcs can be interpreted as the maximum free energy that can be contributed by the Gibbs-Thomson effect
-                dG, _ = self.drivingForceFunction(x, t, returnComp = False)
-
-                #if driving force can be obtained (generally True)
-                if dG is not None:
-                    self.G.append(dG)
-                    self.Gcoords.append([x, t])
-                    
-                    #Add these points to the composition surrogate training data as an endpoint (these are for the minimum particle radius)
-                    self.ICcoords.append([t, dG])
-                    self.xParent.append(x)
-                    self.xPrec.append(x)
-        
-        self.G = np.array(self.G)
-        self.Gcoords = np.array(self.Gcoords)
-        
-        self.xParent = np.array(self.xParent)
-        self.xPrec = np.array(self.xPrec)
-        self.ICcoords = np.array(self.ICcoords)
-        
-        #Invert free energy coordinates - this will make the spacing more consistent
-        self.ICcoords[:,1] =  1 / self.ICcoords[:,1]
-        
-        #Scale temperature and free energy range is proportional to amount of data along given axis
-        if len(temperature) == 1:
-            self.TICscale = 1
-        else:
-            self.TICscale = (np.amax(self.ICcoords[:,0]) - np.amin(self.ICcoords[:,0])) / len(temperature)
-            self.ICcoords[:,0] /= self.TICscale
-            
-        if len(freeEnergy) == 1:
-            self.GICscale = 1
-        else:
-            self.GICscale = (np.amax(self.ICcoords[:,1]) - np.amin(self.ICcoords[:,1])) / len(freeEnergy)
-            self.ICcoords[:,1] /= self.GICscale
-            
-        if len(self.uniqueXPrec) == 1:
-            self.XGscale = 1
-        else:
-            self.XGscale = (np.amax(self.Gcoords[:,0]) - np.amin(self.Gcoords[:,0])) / len(self.uniqueXPrec)
-            self.Gcoords[:,0] /= self.XGscale
-            
-        self.Gcoords[:,1] /= self.TICscale
+        density : int
+            Number of samples to take per degree of freedom in the phase
+        '''
+        self.pDens = density
 
-        #Filter points such that all points are separated by a distance by at least self.eps
-        self.ICcoords, outputs = _filter_points(self.ICcoords, [self.xParent, self.xPrec], self.eps)
-        self.xParent = outputs[0]
-        self.xPrec = outputs[1]
-        
-        self.Gcoords, outputs = _filter_points(self.Gcoords, [self.G], self.eps)
-        self.G = outputs[0]
+    def setMobility(self, mobility):
+        '''
+        Allows user to define mobility functions
 
-        if scale == 'log':
-            self.linearIC = False
-        else:
-            self.linearIC = True
-        self.ICfunction = function
-        self.ICepsilon = epsilon
-        self.ICsmooth = np.amax([smooth, self.eps])
+        mobility : dict
+            Dictionary of functions for each element (including reference)
+            Each function takes in (v.T, v.P, v.N, v.GE, site fractions) and returns mobility
 
-        self._createICSurrogate()
+        Optional - only required for multicomponent systems where
+            mobility terms are not defined in the TDB database
+        '''
+        self.mobCallables = mobility
 
-    def _createICSurrogate(self):
+    def setDiffusivity(self, diffusivity):
         '''
-        Build surrogates for interfacial composition
+        Allows user to define diffusivity functions
+
+        diffusivity : dict
+            Dictionary of functions for each element (including reference)
+            Each function takes in (v.T, v.P, v.N, v.GE, site fractions) and returns diffusivity
+
+        Optional - only required for multicomponent systems where
+            diffusivity terms are not defined in the TDB database
+            and if mobility terms are not defined
         '''
-        if self.linearIC:
-            self.SurrogateParent = Rbf(self.ICcoords[:,0], self.ICcoords[:,1], self.xParent, function = self.ICfunction, epsilon = self.ICepsilon, smooth=self.ICsmooth)
-            self.SurrogatePrec = Rbf(self.ICcoords[:,0], self.ICcoords[:,1], self.xPrec, function = self.ICfunction, epsilon = self.ICepsilon, smooth=self.ICsmooth)  
-        else:
-            self.LogSurrParent = Rbf(self.ICcoords[:,0], self.ICcoords[:,1], np.log10(self.xParent), function = self.ICfunction, epsilon = self.ICepsilon, smooth=self.ICsmooth)
-            self.LogSurrPrec = Rbf(self.ICcoords[:,0], self.ICcoords[:,1], np.log10(self.xPrec), function = self.ICfunction, epsilon = self.ICepsilon, smooth=self.ICsmooth) 
-            
-            self.SurrogateParent = lambda T, gExtraInverse: 10**(self.LogSurrParent(T, gExtraInverse))
-            self.SurrogatePrec = lambda T, gExtraInverse: 10**(self.LogSurrPrec(T, gExtraInverse))
-           
-        if len(self.G) == 1:
-            self.SurrogateG = lambda x, T: self.G[0]
-        else:
-            self.SurrogateG = Rbf(self.Gcoords[:,0], self.Gcoords[:,1], self.G, function = 'linear', epsilon = 1)
+        self.diffCallables = diffusivity
 
-    def changeInterfacialCompositionHyperparameters(self, function = 'linear', epsilon = 1, smooth = 0):
+    def setMobilityCorrection(self, element, factor):
         '''
-        Re-create surrogate model for interfacial composition with updated hyperparameters
+        Factor to multiply mobility by for each element
 
         Parameters
         ----------
-        function : str (optional)
-            Radial basis function to use (defaults to 'linear')
-            Other functions are 'multiquadric', 'inverse_multiquadric',
-                'gaussian', 'cubic', 'quintic' and 'thin_plate'
-        epsilon : float
-            Scale for radial basis function (defaults to 1)
-            Training data will be scaled automatically
-                such that optimal scale is around 1
-        smooth : float
-            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
+        element : str
+            Element to set factor for
+            If 'all', factor will be set to all elements
+        factor : float
+            Scaling factor
         '''
-        if self.TICscale is None:
-            raise Exception("Interfacial composition has not been trained.")
-
-        self.ICfunction = function
-        self.ICepsilon = epsilon
-        self.ICsmooth = np.amax([smooth, self.eps])
+        if element == 'all':
+            for e in self.mobility_correction:
+                self.mobility_correction[e] = factor
+        else:
+            self.mobility_correction[element] = factor
 
-        self._createICSurrogate()
-            
-    def getInterfacialComposition(self, T, gExtra = 0):
+    def _getConditions(self, x, T, gExtra = 0):
         '''
-        Gets Interfacial composition from surrogate models
-        
+        Creates dictionary of conditions from composition, temperature and gExtra
+
         Parameters
         ----------
-        T : float or array of floats
+        x : list
+            Composition (excluding reference element)
+        T : float
             Temperature
-        gExtra : float or array of floats
-            Free energy from Gibbs-Thomson contribution (must be same length as T)
-        
-        Returns
-        -------
-        (composition of parent phase, composition of precipitate phase)
-        Composition will be in same shape as T and gExtra
-        Will return (None, None) if gExtra is large enough that 
-            precipitate becomes unstable
-        '''
-        if self.TICscale is None:
-            raise Exception("Interfacial composition has not been trained.")
-
-        #Convert arrays to Numpy arrays for math operations
-        #Also raise gExtra to lowest training value to avoid erroneous values
-        #   NOTE: Do not use this as a way to minimize the amount of training points!!
-        #   While this is a safegaurd to avoid weird results, this creates a constant growth rate
-        #   for any values of gExtra less than the lowest training point, which can lead to non-realistic
-        #   values in the precipitate simulation (i.e. precipitates growing in an unsaturated matrix).
-        #   Just train more points at lower gExtra values (larger radius sizes)
-        if hasattr(gExtra, '__len__'):
-            gExtra = np.array(gExtra)
-            gExtra[1 / (gExtra * self.GICscale) > np.amax(self.ICcoords[:,1])] = 1 / (np.amax(self.ICcoords[:,1]) * self.GICscale)
-        else:
-            if gExtra == 0 or (1 / (gExtra * self.GICscale)) > np.amax(self.ICcoords[:,1]):
-                gExtra = 1 / (np.amax(self.ICcoords[:,1]) * self.GICscale)
-        if hasattr(T, '__len__'):
-            T = np.array(T)
-
-        #If gExtra is array and T isn't, then convert T to array
-        #This is to keep consistent with Thermodynamics counterpart
-        if hasattr(gExtra, '__len__') and not hasattr(T, '__len__'):
-            T = T * np.ones(len(gExtra))
+        gExtra : float
+            Gibbs free energy to add to phase
+        '''
+        cond = {v.X(self.elements[i+1]): x[i] for i in range(len(x))}
+        cond[v.P] = 101325
+        cond[v.T] = T
+        cond[v.GE] = gExtra
+        cond[v.N] = 1
+        return cond
 
-        xM, xP = self.SurrogateParent(T / self.TICscale, 1 / (gExtra * self.GICscale)), self.SurrogatePrec(T / self.TICscale, 1 / (gExtra * self.GICscale))
-        
-        dG = self.SurrogateG(xP / self.XGscale, T / self.TICscale)
-        if hasattr(xM, '__len__'):
-            noneVals = (dG < gExtra)
-            xM[noneVals] = -1
-            xP[noneVals] = -1
-        else:
-            if dG < gExtra:
-                xM = -1
-                xP = -1
-                    
-        return xM, xP
-
-    def trainInterdiffusivity(self, comps, temperature, function='linear', epsilon=1, smooth=0, scale='linear'):
-        '''
-        Trains interdiffusivity from mobility parameters
+    def _createCompositionSet(self, eq, state_variables, phase, phase_amounts, idx):
+        '''
+        Creates a pycalphad CompositionSet from equilibrium results
 
         Parameters
         ----------
-        comps : array of floats
-            Range of compositions for training points
-        temperature : float or array
-            Temperature or range of temperatures for training points
-        function : str (optional)
-            Radial basis function to use (defaults to 'linear')
-            Other functions are 'multiquadric', 'inverse_multiquadric',
-                'gaussian', 'cubic', 'quintic' and 'thin_plate'
-        epsilon : float
-            Scale for radial basis function (defaults to 1)
-            Training data will be scaled automatically
-                such that optimal scale is around 1
-        smooth : float
-            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
-        scale : float
-            Whether the diffusivity output should be in log or linear scale
-        '''
-        #Convert composition and temperature to array if not so
-        if not hasattr(comps, '__len__'):
-            comps = [comps]
-
-        if not hasattr(temperature, '__len__'):
-            temperature = [temperature]
-
-        self.Diffcoords = []
-        self.Diff = []
-
-        for x in comps:
-            for t in temperature:
-                self.Diff.append(self.diffusivityFunction(x, t))
-                self.Diffcoords.append([x, t])
-
-        self.Diffcoords = np.array(self.Diffcoords)
-        self.Diff = np.array(self.Diff)
-
-        #Scale temperature and free energy range is proportional to amount of data along given axis
-        if len(comps) == 1:
-            self.XDiffscale = 1
-            self.singleXDiff = True
-        else:
-            self.XDiffscale = (np.amax(self.Diffcoords[:,0]) - np.amin(self.Diffcoords[:,0])) / len(comps)
-            self.Diffcoords[:,0] /= self.XDiffscale
-            self.singleXDiff = False
-
-        if len(temperature) == 1:
-            self.TDiffscale = 1
-        else:
-            self.TDiffscale = (np.amax(self.Diffcoords[:,1]) - np.amin(self.Diffcoords[:,1])) / len(temperature)
-            self.Diffcoords[:,1] /= self.TDiffscale
-
-        #Filter diffusivity points
-        self.Diffcoords, outputs = _filter_points(self.Diffcoords, [self.Diff], self.eps)
-        self.Diff = outputs[0]
+        eq : pycalphad equilibrium result
+        state_variables : list
+            List of state variables
+        phase : str
+            Phase to create CompositionSet for
+        phase_amounts : list
+            Array of floats for phase fraction of each phase
+        idx : ndarray
+            Index array for the index of phase
+        '''
+        miscibility = False
+        cs = CompositionSet(self.phase_records[phase])
+        #If there's a miscibility gap in the matrix phase, then take the largest value
+        if len(idx) > 1:
+            idx = [idx[np.argmax(phase_amounts[idx])]]
+            miscibility = True
+        cs.update(eq.Y.isel(vertex=idx[0]).values.ravel()[:cs.phase_record.phase_dof],
+                        phase_amounts[idx[0]], state_variables)
 
-        if scale == 'log':
-            self.linearDiff = False
-        else:
-            self.linearDiff = True
-        self.Difffunction = function
-        self.Diffepsilon = epsilon
-        self.Diffsmooth = np.amax([smooth, self.eps])
-
-        self._createDiffSurrogate()
-
-    def _createDiffSurrogate(self):
-        '''
-        Builds surrogate for diffusivity
-        '''
-        #If only 1 data point, then create constant function
-        if len(self.Diff) == 1:
-            self.SurrogateDiff = lambda x, T: self.Diff[0]
-            return
-
-        #Build surrogates
-        if self.linearDiff:
-            if self.singleXDiff:
-                self.SurrogateDiff = Rbf(self.Diffcoords[:,1], self.Diff, function = self.Difffunction, epsilon = self.Diffepsilon, smooth = self.Diffsmooth)
-            else:
-                self.SurrogateDiff = Rbf(self.Diffcoords[:,0], self.Diffcoords[:,1], self.Diff, function = self.Difffunction, epsilon = self.Diffepsilon, smooth = self.Diffsmooth) 
-        else:
-            if self.singleXDiff:
-                self.LogSurrDiff = Rbf(self.Diffcoords[:,1], np.log10(self.Diff), function = self.Difffunction, epsilon = self.Diffepsilon, smooth = self.Diffsmooth)
-                self.SurrogateDiff = lambda T: 10**(self.LogSurrDiff(T))
-            else:
-                self.LogSurrDiff = Rbf(self.Diffcoords[:,0], self.Diffcoords[:,1], np.log10(self.Diff), function = self.Difffunction, epsilon = self.Diffepsilon, smooth = self.Diffsmooth) 
-                self.SurrogateDiff = lambda x, T: 10**(self.LogSurrDiff(x, T))
+        return cs, miscibility
 
-    def changeDiffusivityHyperparameters(self, function = 'linear', epsilon = 1, smooth = 0):
+    def getEq(self, x, T, gExtra = 0, precPhase = None):
         '''
-        Re-create surrogate model for diffusivity with updated hyperparameters
+        Calculates equilibrium at specified x, T, gExtra
+
+        This is separated from the interfacial composition function so that this can be used for getting curvature for interfacial composition from mobility
 
         Parameters
         ----------
-        function : str (optional)
-            Radial basis function to use (defaults to 'linear')
-            Other functions are 'multiquadric', 'inverse_multiquadric',
-                'gaussian', 'cubic', 'quintic' and 'thin_plate'
-        epsilon : float
-            Scale for radial basis function (defaults to 1)
-            Training data will be scaled automatically
-                such that optimal scale is around 1
-        smooth : float
-            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
+        x : float or array
+            Composition
+            Needs to be array for multicomponent systems
+        T : float
+            Temperature
+        gExtra : float
+            Gibbs-Thomson contribution (if applicable)
+        precPhase : str, int, list or None
+            Precipitate phase (default is first precipitate)
+            Options:
+                None - first precipitate phase in phase list
+                str - specific precipitate phase by name
+                list - all phases by name in list
+                -1 - no precipitate phase
+
+        Returns
+        -------
+        Dataset from pycalphad equilibrium results
         '''
-        if self.XDiffscale is None:
-            raise Exception("Diffusivity has not been trained.")
+        phases = [self.phases[0]]
+        if precPhase != -1:
+            if precPhase is None:
+                precPhase = self.phases[1]
+            if isinstance(precPhase, str):
+                phases.append(precPhase)
+            else:
+                phases = [p for p in precPhase]
+        phaseRec = {p: self.phase_records[p] for p in phases}
 
-        self.Difffunction = function
-        self.Diffepsilon = epsilon
-        self.Diffsmooth = np.amax([smooth, self.eps])
+        if not hasattr(x, '__len__'):
+            x = [x]
 
-        self._createDiffSurrogate()
+        #Remove first element if x lists composition of all elements
+        if len(x) == len(self.elements) - 1:
+            x = x[1:]
 
-    def getInterdiffusivity(self, x, T):
+        cond = self._getConditions(x, T, gExtra+self.gOffset)
+
+        eq = equilibrium(self.db, self.elements, phases, cond, model=self.models, 
+                         phase_records=phaseRec, 
+                         calc_opts={'pdens': self.pDens})
+        return eq
+
+    def getLocalEq(self, x, T, gExtra = 0, precPhase = None, composition_sets = None):
         '''
-        Returns interdiffusivity
+        Calculates local equilibrium at specified x, T, gExtra
 
         Parameters
         ----------
-        x : float or array of floats
+        x : float or array
             Composition
-        T : float or array of floats
-            Temperature (must be same length as x)
-        
+            Needs to be array for multicomponent systems
+        T : float
+            Temperature
+        gExtra : float
+            Gibbs-Thomson contribution (if applicable)
+        precPhase : str, int, list or None
+            Precipitate phase (default is first precipitate)
+            Options:
+                None - first precipitate phase in phase list
+                str - specific precipitate phase by name
+                list - all phases by name in list
+                -1 - no precipitate phase
+
         Returns
         -------
-        diffusivity (same shape as x and T)
-        '''
-        #Convert arrays to numpy arrays for math operations
-        if hasattr(x, '__len__'):
-            x = np.array(x)
-        if hasattr(T, '__len__'):
-            T = np.array(T)
+        result - equilibrium convergence and chemical potentials
+        composition_sets - list of CompositionSet for phases in "equilibrium"
+            Note - "equilibrium" in terms of the matrix and singled out precipitate phase (or just matrix if precPhase is -1)
+        '''
+        phases = [self.phases[0]]
+        if precPhase != -1:
+            if precPhase is None:
+                precPhase = self.phases[1]
+            if isinstance(precPhase, str):
+                phases.append(precPhase)
+            else:
+                phases = [p for p in precPhase]
 
-        if self.XDiffscale is None:
-            raise Exception("Diffusivity has not been trained.")
+        if not hasattr(x, '__len__'):
+            x = [x]
 
-        if self.singleXDiff:
-            return self.SurrogateDiff(T / self.TDiffscale)
-        else:
-            return self.SurrogateDiff(x / self.XDiffscale, T / self.TDiffscale)
-        
-    def drivingForceTrainingTemperature(self):
-        '''
-        Returns the temperature coordinates of driving force training points
-        '''
-        return self.dGcoords[:,1] * self.TDGscale
-        
-    def drivingForceTrainingComposition(self):
+        #Remove first element if x lists composition of all elements
+        if len(x) == len(self.elements) - 1:
+            x = x[1:]
+
+        cond = self._getConditions(x, T, gExtra)
+        result, composition_sets = local_equilibrium(self.db, self.elements, phases, cond,
+                                                         self.models, self.phase_records,
+                                                         composition_sets=composition_sets)
+        return result, composition_sets
+
+    def getInterdiffusivity(self, x, T, removeCache = True, phase = None):
         '''
-        Returns the composition coordinates of driving force training points
+        Gets interdiffusivity at specified x and T
+        Requires TDB database to have mobility or diffusivity parameters
+
+        Parameters
+        ----------
+        x : float, array or 2D array
+            Composition
+            Float or array for binary systems
+            Array or 2D array for multicomponent systems
+        T : float or array
+            Temperature
+            If array, must be same length as x
+                For multicomponent systems, must be same length as 0th axis
+        removeCache : boolean
+            If True, recalculates equilibrium to get interdiffusivity (default)
+            If False, will use calculation from driving force calcs (if available) to compute diffusivity
+        phase : str
+            Phase to compute diffusivity for (defaults to first or matrix phase)
+            This only needs to be used for multiphase diffusion simulations
+
+        Returns
+        -------
+        interdiffusivity - will return array if T is an array
+            For binary case - float or array of floats
+            For multicomponent - matrix or array of matrices
         '''
-        if self.linearDG:
-            return self.dGcoords[:,0] * self.XDGscale
+        dnkj = []
+
+        if hasattr(T, '__len__'):
+            for i in range(len(T)):
+                dnkj.append(self._interdiffusivitySingle(x[i], T[i], removeCache, phase))
+            return np.array(dnkj)
         else:
-            return 10**(self.dGcoords[:,0] * self.XDGscale)
-            
-    def interfacialCompositionTrainingTemperature(self):
-        '''
-        Returns the temperature coordinates of interfacial composition training points
-        '''
-        return self.ICcoords[:,0] * self.TICscale
-        
-    def interfacialCompositionTrainingGibbsThomson(self):
-        '''
-        Returns the Gibbs-Thomson contribution coordinates of interfacial composition training points
-        '''
-        return 1 / (self.ICcoords[:,1] * self.GICscale)
+            return self._interdiffusivitySingle(x, T, removeCache, phase)
 
-    def save(self, fileName):
+    def _interdiffusivitySingle(self, x, T, removeCache = True, phase = None):
         '''
-        Pickles surrogate data
-        Note: this will remove the user-defined driving force and interfacial compositions
-            This is not a problem; however, a loaded surrogate will not be
-            able to be re-trained with different training points
+        Gets interdiffusivity at unique composition and temperature
 
         Parameters
         ----------
-        fileName : str
+        x : float or array
+            Composition
+        T : float
+            Temperature
+        removeCache : boolean
+        phase : str
+
+        Returns
+        -------
+        Interdiffusivity as a matrix (will return float in binary case)
         '''
-        self.binTherm = None
-        self.drivingForceFunction = None
-        self.interfacialCompositionFunction = None
-        self.diffusivityFunction = None
+        if phase is None:
+            phase = self.phases[0]
 
-        self.LogSurrDG = None
-        self.LogSurrPrecComp = None
-        self.SurrogateDrivingForce = None
-        self.SurrogatePrecComp = None
+        if not hasattr(x, '__len__'):
+            x = [x]
 
-        self.SurrogateParent = None
-        self.SurrogatePrec = None
-        self.SurrogateG = None
-        self.LogSurrParent = None
-        self.LogSurrPrec = None
+        #Remove first element if x lists composition of all elements
+        if len(x) == len(self.elements) - 1:
+            x = x[1:]
 
-        self.SurrogateDiff = None
-        self.LogSurrDiff = None
+        cond = self._getConditions(x, T, 0)
 
-        with open(fileName, 'wb') as file:
-            pickle.dump(self, file)
+        if removeCache:
+            self._matrix_cs = None
+            self._parentEq, self._matrix_cs = local_equilibrium(self.db, self.elements, [phase], cond,
+                                                        self.models, self.phase_records,
+                                                        composition_sets=self._matrix_cs)
 
-        #Re-create surrogates so that it could still be used after saving
-        if self.XDGscale is not None:
-            self._createDGSurrogate()
-        if self.TICscale is not None:
-            self._createICSurrogate()
-        if self.XDiffscale is not None:
-            self._createDiffSurrogate()
+        cs_matrix = [cs for cs in self._matrix_cs if cs.phase_record.phase_name == phase][0]
+        chemical_potentials = self._parentEq.chemical_potentials
 
-    def load(fileName):
+        if self.mobCallables[phase] is None:
+            Dnkj, _, _ = inverseMobility_from_diffusivity(chemical_potentials, cs_matrix,
+                                                                            self.elements[0], self.diffCallables[phase],
+                                                                            diffusivity_correction=self.mobility_correction,
+                                                                            parameters = self._parameters)
+        else:
+            Dnkj, _, _ = inverseMobility(chemical_potentials, cs_matrix, self.elements[0],
+                                                        self.mobCallables[phase],
+                                                        mobility_correction=self.mobility_correction,
+                                                        parameters=self._parameters)
+
+        if len(x) == 1:
+            return Dnkj.ravel()[0]
+        else:
+            sortIndices = np.argsort(self.elements[1:-1])
+            unsortIndices = np.argsort(sortIndices)
+            Dnkj = Dnkj[unsortIndices,:]
+            Dnkj = Dnkj[:,unsortIndices]
+            return Dnkj
+
+
+    def getTracerDiffusivity(self, x, T, removeCache = True, phase = None):
         '''
-        Loads data from a pickled surrogate and builds driving force and interfacial composition functions
+        Gets tracer diffusivity for element el at specified x and T
+        Requires TDB database to have mobility or diffusivity parameters
 
         Parameters
         ----------
-        fileName : str
+        x : float, array or 2D array
+            Composition
+            Float or array for binary systems
+            Array or 2D array for multicomponent systems
+        T : float or array
+            Temperature
+            If array, must be same length as x
+                For multicomponent systems, must be same length as 0th axis
+        removeCache : boolean
+        phase : str
 
         Returns
         -------
-        BinarySurrogate object
+        tracer diffusivity - will return array if T is an array
         '''
-        surr = None
-        with open(fileName, 'rb') as file:
-            surr = pickle.load(file)
-
-        #Re-create surrogates so that it could still be used after saving
-        if surr.XDGscale is not None:
-            surr._createDGSurrogate()
-        if surr.TICscale is not None:
-            surr._createICSurrogate()
-        if surr.XDiffscale is not None:
-            surr._createDiffSurrogate()
-
-        return surr
-        
-class MulticomponentSurrogate:
-    '''
-    Handles surrogate models for driving force, interfacial composition
-        and growth rate in a multicomponent system
-    
-    Parameters
-    ----------
-    thermodynamics - MulticomponentThermodynamics (optional)
-        Driving force, interfacial composition and 
-            curvature functions will be taken from this
-        If None, then drivingForce and curvature will need to be defined
-        
-    drivingForce - function (optional))
-        Function will take in (composition, temperature) and return driving force
-            where a positive value means that precipitation is favorable
-            composition is an array for each element, excluding the reference element
-        
-    interfacialComposition - function (optional)
-        Takes in (composition, temperature, gExtra) and returns matrix and precipitate composition
-            composition is an array for each element, excluding the reference element
-        Function should return (None, None) if precipitate is unstable
-
-    curvature - function (optional)
-        Function will take in (composition, temperature) and return the following:
-            {D-1 dCbar / dCbar^T M-1 dCbar} - for calculating interfacial composition of matrix
-            {1 / dCbar^T M-1 dCbar} - for calculating growth rate
-            {Gb^-1 Ga} - for calculating precipitate composition
-            Ca - interfacial composition of matrix phase
-            Cb - interfacial composition of precipitate phase
-        Function will return (None, None, None, None, None) if composition is outside two phase region
-    
-    precPhase : str (optional)
-        Precipitate phase to consider if binaryThermodynamics is defined
+        td = []
 
-    Note: if binaryThermodynamics is not defined, then drivingForce and
-        interfacial composition needs to be defined
-    '''
-    def __init__(self, thermodynamics = None, drivingForce = None, interfacialComposition = None, curvature = None, precPhase = None):
-        self.therm = thermodynamics
-        self.precPhase = precPhase
-        self.elements = self.therm.elements[1:-1]
-        
-        #Grab driving force and curvature function from thermodynamics class if not supplied
-        if drivingForce is None:
-            #self.drivingForceFunction = self.therm.getDrivingForce
-            self.drivingForceFunction = lambda x, T, returnComp=False, training = True: self.therm.getDrivingForce(x, T, self.precPhase, returnComp, training)
-            #self.drivingForceFunction = lambda x, T, returnComp=False: self.therm.drivingForceFromCurvature(x, T, self.precPhase, returnComp)
-        else:
-            self.drivingForceFunction = drivingForce
-
-        if interfacialComposition is None:
-            self.interfacialCompositionFunction = lambda x, T, gExtra: self.therm.getInterfacialComposition(x, T, gExtra, self.precPhase)
-        else:
-            self.interfacialCompositionFunction = interfacialComposition
-
-        if curvature is None:
-            #self.curvature = self.therm.curvatureFactor
-            self.curvature = lambda x, T, training = True: self.therm.curvatureFactor(x, T, self.precPhase, training)
+        if hasattr(T, '__len__'):
+            for i in range(len(T)):
+                td.append(self._tracerDiffusivitySingle(x[i], T[i], removeCache, phase))
+            return np.array(td)
         else:
-            self.curvature = curvature
+            return self._tracerDiffusivitySingle(x, T, removeCache, phase)
 
-        self.eps = 1e-3
-
-        #Driving force ---------------------------------------------------
-        #Training data
-        self.drivingForce = []
-        self.precComp = []
-        self.dGcoords = []
-        self.precCompIndices = []
-        self.precCompCoords = []
-
-        #Scaling factor
-        self.XDGscale = []
-        self.TDGscale = None
-        
-        #Surrogates
-        self.linearDG = True
-        self.DGfunction = 'linear'
-        self.DGepsilon = 1
-        self.DGsmooth = 0
-        self.SurrogateDrivingForce = None
-        self.SurrPrecComp = None
-        self.SurrogatePrecComp = None
-        self.LogSurrDG = None
-        self.LogSurrPrecComp = None
-
-        #Interfacial composition -----------------------------------------
-        #Training data
-        self.Dc = []
-        self.Mc = []
-        self.Gba = []
-        self.beta = []
-        self.Ca = []
-        self.Cb = []
-        self.ICcoords = []
-
-        #Scaling factors
-        self.XICscale = None
-        self.TICscale = None
-
-        #Interfacial composition surrogates
-        self.linearIC = True
-        self.ICfunction = 'linear'
-        self.ICepsilon = 1
-        self.ICsmooth = 0
-
-        self.SurrDc = None
-        self.SurrCa = None
-        self.SurrCb = None
-        self.SurrGba = None
-
-        self.LogSurrDc = None
-        self.LogSurrMc = None
-        self.LogSurrBeta = None
-        self.LogSurrCa = None
-        self.LogSurrCb = None
-        self.LogSurrGba = None
-        
-        self.SurrogateDc = None
-        self.SurrogateMc = None
-        self.SurrogateBeta = None
-        self.SurrogateCa = None
-        self.SurrogateCb = None
-        self.SurrogateGba = None
-
-        
-    def trainDrivingForce(self, comps, temperature, function='linear', epsilon=1, smooth=0, scale='linear'):
+    def _tracerDiffusivitySingle(self, x, T, removeCache = True, phase = None):
         '''
-        Creates training points and sets up surrogate models for driving force calculations
-        
+        Gets tracer diffusivity at unique composition and temperature
+
         Parameters
         ----------
-        comps : 2-D array
-            Range of compositions for training points
-            0th axis represents an individual training point
-            1st axis represents element composition
-        temperature : float or array
-            Range of temperatures for training points
-        function : str (optional)
-            Radial basis function to use (defaults to 'linear')
-            Other functions are 'multiquadric', 'inverse_multiquadric',
-                'gaussian', 'cubic', 'quintic' and 'thin_plate'
-        epsilon : float
-            Scale for radial basis function (defaults to 1)
-            Training data will be scaled automatically
-                such that optimal scale is around 1
-        smooth : float
-            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
-        scale : float
-            Whether the composition training data should be in log or linear scale
-            Note: 'log' is recommended for dilute solutions
-        '''
-        #Make temperature an array if not so
-        if not hasattr(temperature, '__len__'):
-            temperature = [temperature]
-
-        #Ensure that composition are defined values when using log scale
-        if scale == 'log':
-            for x in comps:
-                x[x == 0] = 1e-9
-        
-        #Create training data
-        self.drivingForce = []
-        self.precComp = []
-        self.dGcoords = []
-        self.precCompIndices = []
-        
-        n = 0   #Index for precCompIndices (needs to correspond to indices self.drivingForce array)
-        for t in temperature:
-            for x in comps:
-                dG, xP = self.drivingForceFunction(x, t, returnComp = True)
-                
-                #If driving force can be obtained (generally True)
-                if dG is not None:
-                    self.drivingForce.append(dG)
-                    self.dGcoords.append(np.concatenate((x, [t])))
-                    
-                    #If driving force is positive, then add nucleate composition
-                    #Also determine equilibrium matrix composition, then add training point where driving force is 0
-                    
-                    if xP is not None:
-                        self.precComp.append(xP)
-                        self.precCompIndices.append(n)
-                        
-                        xMeq, xPeq = self.interfacialCompositionFunction(x, t, 0)
-                        if xMeq is not None:
-                            self.drivingForce.append(0)
-                            self.dGcoords.append(np.concatenate((xMeq[1:], [t])))
-                            n += 1
-                            self.precComp.append(xPeq[1:])
-                            self.precCompIndices.append(n)
-                        
-                    n += 1
-                
-        self.drivingForce = np.array(self.drivingForce)
-        self.precComp = np.array(self.precComp)
-        self.dGcoords = np.array(self.dGcoords)
-        self.precCompIndices = np.array(self.precCompIndices)
-        
-        #Log scale on only composition (good for dilute solutions)
-        if scale == 'log':
-            self.dGcoords[:,:-1] = np.log10(self.dGcoords[:,:-1])
+        x : float or array
+            Composition
+        T : float
+            Temperature
+        el : str
+            Element to calculate diffusivity
         
-        #Scale data so range is proportional to amount of data along given axis
-        if len(comps) == 1:
-            self.XDGscale = np.ones(len(self.elements))
-        else:
-            self.XDGscale = (np.amax(self.dGcoords[:,:-1]) - np.amin(self.dGcoords[:,:-1])) / len(comps)
-            self.dGcoords[:,:-1] /= self.XDGscale
-            
-        if len(temperature) == 1:
-            self.TDGscale = 1
-        else:
-            self.TDGscale = (np.amax(self.dGcoords[:,-1]) - np.amin(self.dGcoords[:,-1])) / len(temperature)
-            self.dGcoords[:,-1] /= self.TDGscale
+        Returns
+        -------
+        Tracer diffusivity as a float
+        '''
+        if phase is None:
+            phase = self.phases[0]
 
-        #Create new array of coordinates for precipitate composition (this is to allow for filtering)
-        self.precCompCoords = self.dGcoords[self.precCompIndices]
+        if not hasattr(x, '__len__'):
+            x = [x]
 
-        #Filter points such that all points are separated by a distance by at least self.eps
-        self.dGcoords, outputs = _filter_points(self.dGcoords, [self.drivingForce], self.eps)
-        self.drivingForce = outputs[0]
-        
-        self.precCompCoords, outputs = _filter_points(self.precCompCoords, [self.precComp], self.eps)
-        self.precComp = outputs[0]
+        #Remove first element if x lists composition of all elements
+        if len(x) == len(self.elements) - 1:
+            x = x[1:]
+
+        cond = self._getConditions(x, T, 0)
 
-        if scale == 'log':
-            self.linearDG = False
+        if removeCache:
+            self._matrix_cs = None
+            self._parentEq, self._matrix_cs = local_equilibrium(self.db, self.elements, [phase], cond,
+                                                        self.models, self.phase_records,
+                                                        composition_sets=self._matrix_cs)
+
+        cs_matrix = [cs for cs in self._matrix_cs if cs.phase_record.phase_name == phase][0]
+
+        if self.mobCallables[phase] is None:
+            #NOTE: This is not tested yet
+            Dtrace = tracer_diffusivity_from_diff(cs_matrix, self.diffCallables[phase], diffusivity_correction=self.mobility_correction, parameters=self._parameters)
         else:
-            self.linearDG = True
-        self.DGfunction = function
-        self.DGepsilon = epsilon
-        self.DGsmooth = np.amax([smooth, self.eps])
+            Dtrace = tracer_diffusivity(cs_matrix, self.mobCallables[phase], mobility_correction=self.mobility_correction, parameters=self._parameters)
 
-        self._createDGSurrogate()
+        sortIndices = np.argsort(self.elements[:-1])
+        unsortIndices = np.argsort(sortIndices)
 
-    def _createDGSurrogate(self):
-        '''
-        Builds surrogate for driving force
+        Dtrace = Dtrace[unsortIndices]
+
+        return Dtrace
+
+    def getDrivingForce(self, x, T, precPhase = None, returnComp = False, training = False):
         '''
-        if self.linearDG:
-            arguments = [self.dGcoords[:,i] for i in range(len(self.dGcoords[0]))]
-            self.SurrogateDrivingForce = Rbf(*arguments, self.drivingForce, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
-            
-            arguments = [self.precCompCoords[:,i] for i in range(len(self.dGcoords[0]))]
-            self.SurrPrecComp = [Rbf(*arguments, self.precComp[:,i], function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth) for i in range(len(self.elements))]
-            self.SurrogatePrecComp = lambda x, T: np.array([self.SurrPrecComp[i](*x, T) for i in range(len(self.elements))])
-        else:
-            arguments = [self.dGcoords[:,i] for i in range(len(self.dGcoords[0]))]
-            self.LogSurrDG = Rbf(*arguments, self.drivingForce, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
-            self.LogSurrPrecComp = [Rbf(*arguments, self.precComp[:,i], function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth) for i in range(len(self.elements))]
-            self.SurrogateDrivingForce = lambda x, T: self.LogSurrDG(*(np.log10(x) / self.XDGscale), T)
-            self.SurrogatePrecComp = lambda x, T: np.array([self.LogSurrPrecComp[i](*(np.log10(x) / self.XDGscale), T) for i in range(len(self.elements))])
-
-    def changeDrivingForceHyperparameters(self, function = 'linear', epsilon = 1, smooth = 0):
-        '''
-        Re-create surrogate model for driving force with updated hyperparameters
+        Gets driving force using method defined upon initialization
 
         Parameters
         ----------
-        function : str (optional)
-            Radial basis function to use (defaults to 'linear')
-            Other functions are 'multiquadric', 'inverse_multiquadric',
-                'gaussian', 'cubic', 'quintic' and 'thin_plate'
-        epsilon : float
-            Scale for radial basis function (defaults to 1)
-            Training data will be scaled automatically
-                such that optimal scale is around 1
-        smooth : float
-            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
-        '''
-        if self.TDGscale is None:
-            raise Exception("Driving force has not been trained.")
-
-        self.DGfunction = function
-        self.DGepsilon = epsilon
-        self.DGsmooth = np.amax([smooth, self.eps])
-        
-        self._createDGSurrogate()
-        
-    def getDrivingForce(self, x, T, returnComp = False):
+        x : float, array or 2D array
+            Composition of minor element in bulk matrix phase
+            For binary system, use an array for multiple compositions
+            For multicomponent systems, use a 2D array for multiple compositions
+                Where 0th axis is for indices of each composition
+        T : float or array
+            Temperature in K
+            Must be same length as x if x is array or 2D array
+        precPhase : str (optional)
+            Precipitate phase to consider (default is first precipitate phase in list)
+        returnComp : bool (optional)
+            Whether to return composition of precipitate (defaults to False)
+        training : bool (optional)
+            If True, this will not cache any equilibrium
+            This is used for training since training points may not be near each other
+
+        Returns
+        -------
+        (driving force, precipitate composition)
+        Driving force is positive if precipitate can form
+        Precipitate composition will be None if driving force is negative or returnComp is False
         '''
-        Gets driving force from surrogate models
-        
+        if hasattr(T, '__len__'):
+            dgArray = []
+            compArray = []
+            for i in range(len(T)):
+                dg, comp = self._drivingForce(x[i], T[i], precPhase, returnComp, training)
+                dgArray.append(dg)
+                compArray.append(comp)
+            dgArray = np.array(dgArray)
+            compArray = np.array(compArray)
+            return dgArray, compArray
+        else:
+            return self._drivingForce(x, T, precPhase, returnComp, training)
+
+    def _getDrivingForceSampling(self, x, T, precPhase = None, returnComp = False, training = False):
+        '''
+        Gets driving force for nucleation by sampling
+
+        Steps
+            1. Compute local equilibrium at x and T of only the matrix phase
+            2. Sample precipitate phase
+                If ordered contribution to matrix phase, then sample ordering contribution
+                and remove points on the matrix free energy surface
+            3. Compute energy difference between precipitate samples and chemical potential hyperplane
+            4. Find sample that maximizes energy difference and return sample composition and driving force
+
         Parameters
         ----------
-        x : array or 2D array
-            Composition (array of float for each minor element)
-            2D arrays will have 0th axis for each set and 1st axis for composition
-        T : float or array
-            Temperature (must be float or same length as 0th axis of x if array)
-        
+        x : float or array
+            Composition of minor element in bulk matrix phase
+            Use float for binary systems
+            Use array for multicomponent systems
+        T : float
+            Temperature in K
+        precPhase : str (optional)
+            Precipitate phase to consider (default is first precipitate phase in list)
+        returnComp : bool (optional)
+            Whether to return composition of precipitate (defaults to False)
+        training : bool (optional)
+            If True, this will not cache any equilibrium
+            This is used for training since training points may not be near each other
+
         Returns
         -------
-        driving force (positive value means that precipitate is stable)
+        (driving force, precipitate composition)
+        Driving force is positive if precipitate can form
+        Precipitate composition will be None if driving force is negative or returnComp is False
         '''
-        if self.TDGscale is None:
-            raise Exception("Driving force has not been trained.")
-
-        if hasattr(T, '__len__'):
-            T = np.array(T)
-        x = np.array(x)
-        if x.ndim == 2:
-            x = x.T
+        precPhase = self.phases[1] if precPhase is None else precPhase
 
-        if self.linearDG:
-            dG = self.SurrogateDrivingForce(*(x / self.XDGscale), T / self.TDGscale)
-            
-            if returnComp:
-                return dG, self.SurrogatePrecComp(x / self.XDGscale, T / self.TDGscale).T
+        #Calculate equilibrium with only the parent phase -------------------------------------------------------------------------------------------
+        if not hasattr(x, '__len__'):
+            x = [x]
+        cond = self._getConditions(x, T, 0)
+        self._prevX = x
+
+        cs_results = self._getPrecCompositionSetSamplingDF(x, T, cond, precPhase, training)
+        if cs_results is None:
+            return None, None
+        
+        dg, prec_cs = cs_results
+
+        #Remove cache when training
+        if training:
+            self._matrix_cs = None
+
+        if returnComp:
+            sortIndices = np.argsort(self.elements[:-1])
+            unsortIndices = np.argsort(sortIndices)
+            beta_x = np.array(prec_cs.X)
+            beta_x = beta_x[unsortIndices]
+            if len(x) == 1:
+                return dg, beta_x[1:][0]
             else:
-                if hasattr(dG, '__len__'):
-                    return dG, np.full(dG.shape, None)
-                else:
-                    return dG, None
-            
+                return dg, beta_x[1:]
         else:
-            dG = self.SurrogateDrivingForce(x, T / self.TDGscale)
-            
-            if returnComp:
-                return dG, self.SurrogatePrecComp(x, T / self.TDGscale)
-            else:
-                if hasattr(dG, '__len__'):
-                    return dG, np.full(dG.shape, None)
-                else:
-                    return dG, None
+            return dg, None
 
-    def trainCurvature(self, comps, temperature, function='linear', epsilon=1, smooth=0, scale='linear'):
+    def _getDrivingForceApprox(self, x, T, precPhase = None, returnComp = False, training = False):
         '''
-        Trains for curvature factor (from Phillipes and Voorhees - 2013) as a function of composition and temperature
+        Approximate method of driving force calculation
+        Assumes equilibrium composition of precipitate phase
 
-        Creates 5 surrogates
-        {D-1 dCbar / dCbar^T M-1 dCbar} - for calculating interfacial composition of matrix
-        {1 / dCbar^T M-1 dCbar} - for calculating growth rate
-        {Gb^-1 Ga} - for calculating precipitate composition
-        Ca - interfacial composition of matrix phase
-        Cb - interfacial composition of precipitate phase
+        Sampling method is used if driving force is negative
 
+        Steps:
+            1. Compute equilibrium and get composition sets for matrix and precipitate phase
+            2. Check for 2 phases and that one phase is the matrix and other phase is precipitate
+                If not, then resort to sampling method
+            3. Compute equilibrium at matrix composition and get chemical potential hyperplane
+            4. Driving force is the difference between the free energy of the precipitate (from step 1)
+               and the free energy on the chemical potential hyperplane (from step 3) at the precipitate composition
 
         Parameters
         ----------
-        comps : 2D array of floats
-            Range of compositions for training points
-            0th axis represents a training point
-            1st axis represents element compositions
-        temperature : float or array
-            Range of temperatures for training points
-        function : str (optional)
-            Radial basis function to use (defaults to 'linear')
-            Other functions are 'multiquadric', 'inverse_multiquadric',
-                'gaussian', 'cubic', 'quintic' and 'thin_plate'
-        epsilon : float
-            Scale for radial basis function (defaults to 1)
-            Training data will be scaled automatically
-                such that optimal scale is around 1
-        smooth : float
-            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
-        scale : float
-            Whether the matrix composition output should be in log or linear scale
-            Note: 'log' is recommended for dilute solutions
-        '''
-        #Make temperature an array if not so
-        if not hasattr(temperature, '__len__'):
-            temperature = [temperature]
-
-        #Ensure that composition are defined values when using log scale
-        if scale == 'log':
-            for x in comps:
-                x[x == 0] = 1e-9
-        
-        #Create training data
-        self.Dc = []
-        self.Mc = []
-        self.Gba = []
-        self.beta = []
-        self.Ca = []
-        self.Cb = []
-        self.ICcoords = []
-        
-        for t in temperature:
-            for x in comps:
-                dc, mc, gba, beta, ca, cb = self.curvature(x, t)
-
-                if dc is not None:
-                    #Since Dc, Mc and Gba is constant for a given tie-line, add 3 training data points (at bulk compostion and phase boundaries)
-                    #This should give more accurate values at very small or very large supersaturations without having to calculate a lot of training data
-                    compCoords = [x, ca, cb]
-                    for i in range(3):
-                        self.Dc.append(dc)
-                        self.Mc.append(mc)
-                        self.Gba.append(gba)
-                        self.beta.append(beta)
-                        self.Ca.append(ca)
-                        self.Cb.append(cb)
-                        self.ICcoords.append(np.concatenate((compCoords[i], [t])))
-
-        self.Dc = np.array(self.Dc)
-        self.Mc = np.array(self.Mc)
-        self.Gba = np.array(self.Gba)
-        self.beta = np.array(self.beta)
-        self.Ca = np.array(self.Ca)
-        self.Cb = np.array(self.Cb)
-        self.ICcoords = np.array(self.ICcoords)
-        
-        #Log scale only on compositions (good for low solubility)
-        if scale == 'log':
-            self.ICcoords[:,:-1] = np.log10(self.ICcoords[:,:-1])
-        
-        #Scale data so range is proportional to amount of data along given axis
-        if len(comps) == 1:
-            self.XICscale = np.ones(len(self.elements))
-        else:
-            self.XICscale = (np.amax(self.ICcoords[:,:-1]) - np.amin(self.ICcoords[:,:-1])) / len(comps)
-            self.ICcoords[:,:-1] /= self.XICscale
-            
-        if len(temperature) == 1:
-            self.TICscale = 1
-        else:
-            self.TICscale = (np.amax(self.ICcoords[:,-1]) - np.amin(self.ICcoords[:,-1])) / len(temperature)
-            self.ICcoords[:,-1] /= self.TICscale
+        x : float or array
+            Composition of minor element in bulk matrix phase
+            Use float for binary systems
+            Use array for multicomponent systems
+        T : float
+            Temperature in K
+        precPhase : str (optional)
+            Precipitate phase to consider (default is first precipitate phase in list)
+        returnComp : bool (optional)
+            Whether to return composition of precipitate (defaults to False)
+        training : bool (optional)
+            If True, this will not cache any equilibrium
+            This is used for training since training points may not be near each other
 
-        #Filter points such that all points are separated by a distance by at least self.eps
-        self.ICcoords, outputs = _filter_points(self.ICcoords, [self.Dc, self.Mc, self.Gba, self.beta, self.Ca, self.Cb], self.eps)
-        self.Dc = outputs[0]
-        self.Mc = outputs[1]
-        self.Gba = outputs[2]
-        self.beta = outputs[3]
-        self.Ca = outputs[4]
-        self.Cb = outputs[5]
+        Returns
+        -------
+        (driving force, precipitate composition)
+        Driving force is positive if precipitate can form
+        Precipitate composition will be None if driving force is negative or returnComp is False
+        '''
+        if precPhase is None:
+            precPhase = self.phases[1]
 
-        if scale == 'log':
-            self.linearIC = False
-        else:
-            self.linearIC = True
-        self.ICfunction = function
-        self.ICepsilon = epsilon
-        self.ICsmooth = np.amax([smooth, self.eps])
-
-        self._createICSurrogate()
-
-    def _createICSurrogate(self):
-        '''
-        Builds surrogate for interfacial composition and curvature
-        '''
-        if self.linearIC:
-            arguments = [self.ICcoords[:,i] for i in range(len(self.ICcoords[0]))]
-            self.SurrogateMc = Rbf(*arguments, self.Mc, function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth)
-            self.SurrogateBeta = Rbf(*arguments, self.beta, function=self.ICfunction, epislon=self.ICepsilon, smooth=self.ICsmooth)
-
-            self.SurrDc = [Rbf(*arguments, self.Dc[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
-            self.SurrCa = [Rbf(*arguments, self.Ca[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
-            self.SurrCb = [Rbf(*arguments, self.Cb[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
-            self.SurrGba = [[Rbf(*arguments, self.Gba[:,i,j], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for j in range(len(self.elements))] for i in range(len(self.elements))]
-            
-            self.SurrogateDc = lambda x, T: np.array([self.SurrDc[i](*x, T) for i in range(len(self.elements))])
-            self.SurrogateCa = lambda x, T: np.array([self.SurrCa[i](*x, T) for i in range(len(self.elements))])
-            self.SurrogateCb = lambda x, T: np.array([self.SurrCb[i](*x, T) for i in range(len(self.elements))])
-            self.SurrogateGba = lambda x, T: np.array([[self.SurrGba[i][j](*x, T) for j in range(len(self.elements))] for i in range(len(self.elements))])
-            
+        if not hasattr(x, '__len__'):
+            x = [x]
+        cond = self._getConditions(x, T, 0)
+        self._prevX = x
+
+        cs_results = self._getCompositionSetsForDF(x, T, cond, precPhase, training=training)
+        if cs_results is None:
+            return self._getDrivingForceSampling(x, T, precPhase, returnComp, training=training)
         else:
-            arguments = [self.dGcoords[:,i] for i in range(len(self.dGcoords[0]))]
-            self.LogSurrDc = [Rbf(*arguments, self.Dc[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
-            self.LogSurrMc = Rbf(*arguments, self.Mc, function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth)
-            self.LogSurrBeta = Rbf(*arguments, self.beta, function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth)
-            self.LogSurrCa = [Rbf(*arguments, self.Ca[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
-            self.LogSurrCb = [Rbf(*arguments, self.Cb[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
-            self.LogSurrGba = [[Rbf(*arguments, self.Gba[:,i,j], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for j in range(len(self.elements))] for i in range(len(self.elements))]
-            
-            self.SurrogateDc = lambda x, T: np.array([self.LogSurrDc[i](*(np.log10(x) / self.XICscale), T) for i in range(len(self.elements))])
-            self.SurrogateMc = lambda x, T: self.LogSurrMc(*(np.log10(x) / self.XICscale), T)
-            self.SurrogateBeta = lambda x, T: self.LogSurrBeta(*(np.log10(x) / self.XICscale), T)
-            self.SurrogateCa = lambda x, T: np.array([self.LogSurrCa[i](*(np.log10(x) / self.XICscale), T) for i in range(len(self.elements))])
-            self.SurrogateCb = lambda x, T: np.array([self.LogSurrCb[i](*(np.log10(x) / self.XICscale), T) for i in range(len(self.elements))])
-            self.SurrogateGba = lambda x, T: np.array([[self.LogSurrGba[i][j](*(np.log10(x) / self.XICscale), T) for j in range(len(self.elements))] for i in range(len(self.elements))])
+            ph, ele, chemical_potentials, composition_sets, cs_matrix, x_matrix, cs_precip, x_precip = cs_results
 
-    def changeCurvatureHyperparameters(self, function = 'linear', epsilon = 1, smooth = 0):
-        '''
-        Re-create surrogate model for curvature factors with updated hyperparameters
+        #Check that equilibrium has converged
+        #If not, then return None, None since driving force can't be obtained
+        if any(np.isnan(chemical_potentials)):
+            return None, None
 
-        Parameters
-        ----------
-        function : str (optional)
-            Radial basis function to use (defaults to 'linear')
-            Other functions are 'multiquadric', 'inverse_multiquadric',
-                'gaussian', 'cubic', 'quintic' and 'thin_plate'
-        epsilon : float
-            Scale for radial basis function (defaults to 1)
-            Training data will be scaled automatically
-                such that optimal scale is around 1
-        smooth : float
-            Smoothness of interpolation, (defaults to 0, where interpolation will go through all points)
-        scale : float
-            Whether the composition training data should be in log or linear scale
-            Note: 'log' is recommended for dilute solutions
-        '''
-        if self.TICscale is None:
-            raise Exception("Curvature has not been trained.")
+        #If in two phase region, then calculate equilibrium using only parent phase and find free energy difference between chemical potential and free energy of preciptiate
+        if len(ph) == 2 and self.phases[0] in ph and precPhase in ph:
+            for i in range(len(ele)):
+                if ele[i] == self.elements[0]:
+                    refIndex = i
+                    break
+
+            #Equilibrium at matrix composition for only the parent phase
+            self._parentEq, self._matrix_cs = local_equilibrium(self.db, self.elements, [self.phases[0]], cond,
+                                                                self.models, self.phase_records,
+                                                                composition_sets=self._matrix_cs)
+
+
+            #Remove caching if training surrogate in case training points are far apart
+            if training:
+                self._matrix_cs = None
+
+            #Check if equilibrium has converged and chemical potential can be obtained
+            #If not, then return None for driving force
+            if any(np.isnan(self._parentEq.chemical_potentials)):
+                return None, None
+
+            sortIndices = np.argsort(self.elements[1:-1])
+            unsortIndices = np.argsort(sortIndices)
+
+            xP = x_precip
 
-        self.ICfunction = function
-        self.ICepsilon = epsilon
-        self.ICsmooth = np.amax([smooth, self.eps])
+            dg = np.sum(xP * self._parentEq.chemical_potentials) - np.sum(xP * chemical_potentials)
 
-        self._createICSurrogate()
+            #Remove reference element
+            xP = np.delete(xP, refIndex)
 
-    def getCurvature(self, x, T):
+            if returnComp:
+                if len(x) == 1:
+                    return dg.ravel()[0], xP[unsortIndices][0]
+                else:
+                    return dg.ravel()[0], xP[unsortIndices]
+            else:
+                return dg.ravel()[0], None
+        else:
+            #If driving force is negative, then use sampling method ---------------------------------------------------------------------------------
+            return self._getDrivingForceSampling(x, T, precPhase, returnComp, training=training)
+
+    def _getDrivingForceCurvature(self, x, T, precPhase = None, returnComp = False, training = False):
         '''
-        Gets driving force from surrogate models
-        
+        Gets driving force from curvature of free energy function
+        Assumes small saturation
+
+        Steps:
+            1. Compute equilibrium and get composition sets for matrix and precipitate phase
+            2. Check for 2 phases and that one phase is the matrix and other phase is precipitate
+                If not, then resort to sampling method
+            3. Get dmu/dx (free energy curvature)
+            4. Compute (x_infty - x_matrix) * dmu/dx * (x_prec - x_matrix)^T
+                This does a first (or second?) order approximation of the driving force based off the curvature at x_infty
+
+        Sampling method is used if driving force is negative
+
         Parameters
         ----------
-        x : array or 2D array
-            Composition (array of float for each minor element)
-            2D arrays will have 0th axis for each set and 1st axis for composition
-        T : float or array
-            Temperature (must be float or same length as 0th axis of x if array)
-        
+        x : float or array
+            Composition of minor element in bulk matrix phase
+            Use float for binary systems
+            Use array for multicomponent systems
+        T : float
+            Temperature in K
+        precPhase : str (optional)
+            Precipitate phase to consider (default is first precipitate phase in list)
+        returnComp : bool (optional)
+            Whether to return composition of precipitate (defaults to False)
+        training : bool (optional)
+            If True, this will not cache any equilibrium
+            This is used for training since training points may not be near each other
+
         Returns
         -------
-        Curvature factors
-            {D-1 dCbar / dCbar^T M-1 dCbar} - for calculating interfacial composition of matrix
-            {1 / dCbar^T M-1 dCbar} - for calculating growth rate
-            {Gb^-1 Ga} - for calculating precipitate composition
-            Ca - interfacial composition of matrix phase
-            Cb - interfacial composition of precipitate phase
-        Note: this function currently does not return (None, None, None, None, None)
-            if precipitate is unstable
-        '''
-        if self.TICscale is None:
-            raise Exception("Curvature has not been trained.")
-
-        if self.linearIC:
-            dc = self.SurrogateDc(x / self.XICscale, T / self.TICscale)
-            mc = self.SurrogateMc(*(x / self.XICscale), T / self.TICscale)
-            gba = self.SurrogateGba(x / self.XICscale, T / self.TICscale)
-            beta = self.SurrogateBeta(*(x / self.XICscale), T / self.TICscale)
-            #beta = self.SurrogateBeta(x, T / self.TICscale)
-            ca = self.SurrogateCa(x / self.XICscale, T / self.TICscale)
-            cb = self.SurrogateCb(x / self.XICscale, T / self.TICscale)
-            
-            return dc, mc, gba, beta, ca, cb
-            
+        (driving force, precipitate composition)
+        Driving force is positive if precipitate can form
+        Precipitate composition will be None if driving force is negative or returnComp is False
+        '''
+        if precPhase is None:
+            precPhase = self.phases[1]
+
+        if not hasattr(x, '__len__'):
+            x = [x]
+        cond = self._getConditions(x, T, 0)
+        self._prevX = x
+
+        cs_results = self._getCompositionSetsForDF(x, T, cond, precPhase, training=training)
+        if cs_results is None:
+            return self._getDrivingForceSampling(x, T, precPhase, returnComp, training=training)
         else:
-            dc = self.SurrogateDc(x, T / self.TICscale)
-            mc = self.SurrogateMc(x, T / self.TICscale)
-            gba = self.SurrogateGba(x, T / self.TICscale)
-            beta = self.SurrogateBeta(x, T / self.TICscale)
-            ca = self.SurrogateCa(x, T / self.TICscale)
-            cb = self.SurrogateCb(x, T / self.TICscale)
-            
-            return dc, mc, gba, beta, ca, cb
+            ph, ele, chemical_potentials, composition_sets, cs_matrix, x_matrix, cs_precip, x_precip = cs_results
+
+        #Check that equilibrium has converged
+        #If not, then return None, None since driving force can't be obtained
+        if any(np.isnan(chemical_potentials)):
+            return None, None
+
+        if not hasattr(x, '__len__'):
+            x = [x]
+
+        if len(ph) == 2 and self.phases[0] in ph and precPhase in ph:
+            for i in range(len(ele)):
+                if ele[i] == self.elements[0]:
+                    refIndex = i
+                    break
+
+            #If in two phase region, then get curvature of parent phase and use it to calculate driving force ---------------------------------------
+            sortIndices = np.argsort(self.elements[1:-1])
+            unsortIndices = np.argsort(sortIndices)
+
+            dMudxParent = dMudX(chemical_potentials, composition_sets[0], self.elements[0])
+            xM = np.delete(x_matrix, refIndex)
+
+            xP = np.delete(x_precip, refIndex)
+            xBar = np.array([xP - xM])
+
+            x = np.array(x)[sortIndices]
+            xD = np.array([x - xM])
+
+            dg = np.matmul(xD, np.matmul(dMudxParent, xBar.T))
+
+            if returnComp:
+                if len(x) == 1:
+                    return dg.ravel()[0], xP[unsortIndices][0]
+                else:
+                    return dg.ravel()[0], xP[unsortIndices]
+            else:
+                return dg.ravel()[0], None
+        else:
+            #If driving force is negative, then use sampling method ---------------------------------------------------------------------------------
+            return self._getDrivingForceSampling(x, T, precPhase, returnComp, training=training)
 
-    def getGrowthAndInterfacialComposition(self, x, T, dG, R, gExtra):
+    def _getDrivingForceTangent(self, x, T, precPhase = None, returnComp = False, training = False):
         '''
-        Returns growth rate and interfacial compostion given Gibbs-Thomson contribution
+        Gets driving force from parallel tangent calculation
+
+        Steps
+            1. Compute equilibrium to get composition sets (or used previous cached CS)
+            2. Compute equilibrium of matrix phase at matrix composition
+            3. Remove composition and extra free energy from conditions
+            4. Add chemical potential for each component to conditions
+            5. Compute equilibrium of precipitate phase with new conditions
+                The calculated v.GE is the driving force
+
+        This will work for positive and negative driving forces
 
         Parameters
         ----------
-        x : array of floats
-            Matrix composition
+        x : float or array
+            Composition of minor element in bulk matrix phase
+            Use float for binary systems
+            Use array for multicomponent systems
         T : float
-            Temperature
-        dG : float
-            Driving force
-        R : float or array
-            Precipitate radius
-        gExtra : float or array
-            Gibbs-Thomson contribution corresponding to R
-            Must be same shape as R
-        
+            Temperature in K
+        precPhase : str (optional)
+            Precipitate phase to consider (default is first precipitate phase in list)
+        returnComp : bool (optional)
+            Whether to return composition of precipitate (defaults to False)
+        training : bool (optional)
+            If True, this will not cache any equilibrium
+            This is used for training since training points may not be near each other
+            
         Returns
         -------
-        (growth rate, matrix composition, precipitate composition)
-        Growth rate will be float or array depending on R
-        matrix and precipitate composition will be 1D or 2D array depending on R
-            1D array will be length of composition
-            2D array will have 0th axis be length of R and 1st axis be length of composition
-        '''
-        if self.TICscale is None:
-            raise Exception("Curvature needs to be trained to calculated interfacial composition.")
-
-        if hasattr(R, '__len__'):
-            R = np.array(R)
-        if hasattr(gExtra, '__len__'):
-            gExtra = np.array(gExtra)
-
-        dc, mc, gba, beta, ca, cb = self.getCurvature(x, T)
-
-        Rdiff = (dG - gExtra)
-
-        gr = (mc / R) * Rdiff
-
-        if hasattr(Rdiff, '__len__'):
-            calpha = np.zeros((len(Rdiff), len(self.elements)))
-            dca = np.zeros((len(Rdiff), len(self.elements)))
-            cbeta = np.zeros((len(Rdiff), len(self.elements)))
-            for i in range(len(self.elements)):
-                calpha[:,i] = x[i] - dc[i] * Rdiff
-                dca[:,i] = calpha[:,i] - ca[i]
-
-            dcb = np.matmul(gba, dca.T)
-            for i in range(len(self.elements)):
-                cbeta[:,i] = cb[i] + dcb[i,:]
+        (driving force, precipitate composition)
+        Driving force is positive if precipitate can form
+        Precipitate composition will be None if driving force is negative or returnComp is False
+        '''
+        if precPhase is None:
+            precPhase = self.phases[1]
 
-            calpha[calpha < 0] = 0
-            cbeta[cbeta < 0] = 0
+        if not hasattr(x, '__len__'):
+            x = [x]
+        cond = self._getConditions(x, T, self.gOffset)
+        self._prevX = x
+
+        if self._compset_cache_df.get(precPhase, None) is None or training:
+            #This will calculate local equilibrium for the matrix phase and get the composition set for the precipitate phase
+            cs_results = self._getPrecCompositionSetSamplingDF(x, T, cond, precPhase, training=training)
+            if cs_results is None:
+                return None, None
+
+            dg, _prec_cs = cs_results
+            self._compset_cache_df[precPhase] = [_prec_cs]
+        else:
+            #If we already have a cache, then we just need equilibrium at the matrix phase
+            self._parentEq, self._matrix_cs = local_equilibrium(self.db, self.elements, [self.phases[0]], cond,
+                                                    self.models, self.phase_records, composition_sets=self._matrix_cs)
+        
+            #Check that equilibrium has converged
+            #If not, then return None, None since driving force can't be obtained
+            if any(np.isnan(self._parentEq.chemical_potentials)):
+                return None, None
+
+        #Remove element conditions and free extra Gibbs energy conditions
+        for e in self.elements:
+            if v.X(e) in cond:
+                cond.pop(v.X(e))
+        if v.GE in cond:
+            cond.pop(v.GE)
+
+        #Add chemical potential conditions
+        sortedEl = sorted(list(set(self.elements) - set(['VA'])))
+        for i in range(len(sortedEl)):
+            cond[v.MU(sortedEl[i])] = self._parentEq.chemical_potentials[i]
+
+        #Solving for local equilibrium on precipitate
+        #The fixed conditions are T, P and MU, so this should solve for precipitate composition and GE
+        #   Rather than solving for parallel tangent where the driving force is the difference between the chemical potentials of matrix and precipitate phase
+        #   This instead solves for the offset in the precipitate energy surface to make the precipitate lie on the chemical potential hyperplane of the matrix phase
+        prev_dof = np.array(self._compset_cache_df[precPhase][0].dof)
+        _precEq, _prec_cs = local_equilibrium(self.db, self.elements, [precPhase], cond,
+                                                self.models, self.phase_records, composition_sets=self._compset_cache_df[precPhase])
+
+        #Check if precipitate composition at equilibrium is the matrix composition
+        #This can occur in order/disordered models where the miscibility gap is small enough that the parallel tangent can only be found at the matrix composition
+        #In this case, switch to sampling for the driving force
+        #This still seems to be an improvement over approximate and curvature methods since this occurs after the driving force becomes negative
+        prec_comps = np.array(_prec_cs[0].X)
+        mat_comps = np.array(self._matrix_cs[0].X)
+        if np.allclose(prec_comps, mat_comps, 1e-6):
+            self._compset_cache_df[precPhase] = None
+            return self._getDrivingForceSampling(x, T, precPhase, returnComp, training=training)
+
+        self._compset_cache_df[precPhase] = _prec_cs
+
+        #Check that equilibrium has converged
+        #If not, then return None, None since driving force can't be obtained
+        if any(np.isnan(_precEq.chemical_potentials)):
+            return None, None
+        
+        dg = _precEq.x[0]
+        xb = np.array(_prec_cs[0].X)
+
+        sortIndices = np.argsort(self.elements[:-1])
+        unsortIndices = np.argsort(sortIndices)
+        xb = xb[unsortIndices]
 
-            return gr, calpha, cbeta, ca, cb
+        if len(x) == 1:
+            return dg, xb[1:][0]
         else:
-            calpha = x - dc * Rdiff
-            cbeta = cb + np.matmul(gba, (calpha - ca)).flatten()
-
-            calpha[calpha < 0] = 0
-            cbeta[cbeta < 0] = 0
+            return dg, xb[1:]
+    
+    def _getCompositionSetsForDF(self, x, T, cond, precPhase = None, training = False):
+        '''
+        Wrapper for getting composition set from x and T by either global equilibrium or local from a cached composition set
 
-            return gr, calpha, cbeta, ca, cb
+        Parameters
+        ----------
+        x : float or array
+            Composition of minor element in bulk matrix phase
+            Use float for binary systems
+            Use array for multicomponent systems
+        T : float
+            Temperature in K
+        precPhase : str (optional)
+            Precipitate phase to consider (default is first precipitate phase in list)
+        returnComp : bool (optional)
+            Whether to return composition of precipitate (defaults to False)
+        training : bool (optional)
+            If True, this will not cache any equilibrium
+            This is used for training since training points may not be near each other
 
-    def impingementFactor(self, x, T):
+        Returns
+        -------
+        phases - set of stable phases
+        elements - set of elements
+        chemical_potentials
+        composition_sets - all composition sets at equilibrium
+        cs_matrix - composition set of matrix phase
+        x_matrix - composition of matrix phase
+        cs_precip - composition set of precipitate phase
+        x_precip - composition of precipitate phase
         '''
-        Calculates impingement factor for nucleation rate calculations
+        if self._compset_cache_df.get(precPhase, None) is None or training:
+            return self._getCompositionSetsEq(x, T, cond, precPhase)
+        else:
+            return self._getCompositionSetsCache(x, T, cond, precPhase)
+    
+    def _getCompositionSetsEq(self, x, T, cond, precPhase = None):
+        '''
+        Gets composition set from x and T by global equilibrium
+
+        Steps
+            1. Compute equilibrium at x and T
+                If equilibrium did not converge or matrix phase is not stable, then return None
+            2. Get composition sets and add to cache
+                If precipitate is not stable, the return None
+            3. Resolve possible issues with miscibility gaps
+            4. Return values
 
         Parameters
         ----------
-        x : array of floats
-            Matrix composition
+        x : float or array
+            Composition of minor element in bulk matrix phase
+            Use float for binary systems
+            Use array for multicomponent systems
         T : float
-            Temperature
-        '''
-        if self.TICscale is None:
-            raise Exception("Curvature needs to be trained to calculated impingement factor.")
-        #return self.SurrogateBeta(x, T / self.TICscale)
-        if self.linearIC:
-            return self.SurrogateBeta(*(x / self.XICscale), T / self.TICscale)
+            Temperature in K
+        precPhase : str (optional)
+            Precipitate phase to consider (default is first precipitate phase in list)
+        returnComp : bool (optional)
+            Whether to return composition of precipitate (defaults to False)
+
+        Returns
+        -------
+        phases - set of stable phases
+        elements - set of elements
+        chemical_potentials
+        composition_sets - all composition sets at equilibrium
+        cs_matrix - composition set of matrix phase
+        x_matrix - composition of matrix phase
+        cs_precip - composition set of precipitate phase
+        x_precip - composition of precipitate phase
+        '''
+        #Create cache of composition set if not done so already or if training a surrogate
+        #Training points for surrogates may be far apart, so starting from a previous
+        #   composition set could give a bad starting position for the minimizer
+        #Calculate equilibrium ----------------------------------------------------------------------------------------------------------------------
+        eq = self.getEq(x, T, 0, precPhase)
+        #Cast values in state_variables to double for updating composition sets
+        state_variables = np.array([cond[v.GE], cond[v.N], cond[v.P], cond[v.T]], dtype=np.float64)
+        stable_phases = eq.Phase.values.ravel()
+        phase_amounts = eq.NP.values.ravel()
+        matrix_idx = np.where(stable_phases == self.phases[0])[0]
+        precip_idx = np.where(stable_phases == precPhase)[0]
+        chemical_potentials = eq.MU.values.ravel()
+        x_precip = eq.isel(vertex=precip_idx).X.values.ravel()
+        x_matrix = eq.isel(vertex=matrix_idx).X.values.ravel()
+
+        #If matrix phase is not stable, then use sampling method
+        #   This may occur during surrogate training of interfacial composition,
+        #   where we're trying to calculate the driving force at the precipitate composition
+        #   In this case, the conditions will be at th precipitate composition which can result in
+        #   only that phase being stable
+        if len(matrix_idx) == 0:
+            return None
+        
+        if any(np.isnan(chemical_potentials)):
+            return None
+
+        #Test that precipitate phase is stable and that we're not training a surrogate
+        #If not, then there's no composition set to cache
+        if len(precip_idx) > 0:
+            cs_matrix, miscMatrix = self._createCompositionSet(eq, state_variables, self.phases[0], phase_amounts, matrix_idx)
+            cs_precip, miscPrec = self._createCompositionSet(eq, state_variables, precPhase, phase_amounts, precip_idx)
+            x_matrix = np.array(cs_matrix.X)
+            x_precip = np.array(cs_precip.X)
+            
+            composition_sets = [cs_matrix, cs_precip]
+            self._compset_cache_df[precPhase] = composition_sets
+
+            #If there's a miscibility gap in the matrix or precipitate phase, then calculate local equilibrium with the singled out comp sets
+            if miscMatrix or miscPrec:
+                result, composition_sets = local_equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond,
+                                                        self.models, self.phase_records,
+                                                        composition_sets=self._compset_cache_df[precPhase])
+                self._compset_cache_df[precPhase] = composition_sets
+                chemical_potentials = result.chemical_potentials
+                cs_precip = [cs for cs in composition_sets if cs.phase_record.phase_name == precPhase][0]
+                x_precip = np.array(cs_precip.X)
+
+                cs_matrix = [cs for cs in composition_sets if cs.phase_record.phase_name == self.phases[0]][0]
+                x_matrix = np.array(cs_matrix.X)
         else:
-            return self.SurrogateBeta(x, T / self.TICscale)
+            return None
+
+        ph = np.unique(stable_phases[stable_phases != ''])
+        ele = eq.component.values.ravel()
 
-    def save(self, fileName):
+        return ph, ele, chemical_potentials, composition_sets, cs_matrix, x_matrix, cs_precip, x_precip
+    
+    def _getCompositionSetsCache(self, x, T, cond, precPhase = None):
         '''
-        Pickles surrogate data
-        Note: this will remove the user-defined driving force and curvature functions
-            This is not a problem; however, a loaded surrogate will not be
-            able to be re-trained with different training points
+        Gets composition set from x and T by global equilibrium
+
+        Steps
+            1. Compute local equilibrium at x and T using previous composition sets
+            2. Get composition sets and update cache
+                If equilibrium did not converge, then return None
+            3. Return values
 
         Parameters
         ----------
-        fileName : str
-        '''
-        self.therm = None
-        self.drivingForceFunction = None
-        self.interfacialCompositionFunction = None
-        self.curvature = None
+        x : float or array
+            Composition of minor element in bulk matrix phase
+            Use float for binary systems
+            Use array for multicomponent systems
+        T : float
+            Temperature in K
+        precPhase : str (optional)
+            Precipitate phase to consider (default is first precipitate phase in list)
+        returnComp : bool (optional)
+            Whether to return composition of precipitate (defaults to False)
 
-        self.SurrogateDrivingForce = None
-        self.SurrPrecComp = None
-        self.SurrogatePrecComp = None
-        self.LogSurrDG = None
-        self.LogSurrPrecComp = None
+        Returns
+        -------
+        phases - set of stable phases
+        elements - set of elements
+        chemical_potentials
+        composition_sets - all composition sets at equilibrium
+        cs_matrix - composition set of matrix phase
+        x_matrix - composition of matrix phase
+        cs_precip - composition set of precipitate phase
+        x_precip - composition of precipitate phase
+        '''
+        result, composition_sets = local_equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond,
+                                                         self.models, self.phase_records,
+                                                         composition_sets=self._compset_cache_df[precPhase])
+        self._compset_cache_df[precPhase] = composition_sets
+        chemical_potentials = result.chemical_potentials
+        if any(np.isnan(chemical_potentials)):
+            return None
+        
+        ph = [cs.phase_record.phase_name for cs in composition_sets if cs.NP > 0]
+        if len(ph) == 2 and self.phases[0] in ph and precPhase in ph:
+            cs_precip = [cs for cs in composition_sets if cs.phase_record.phase_name == precPhase][0]
+            x_precip = np.array(cs_precip.X)
 
-        self.SurrDc = None
-        self.SurrCa = None
-        self.SurrCb = None
-        self.SurrGba = None
+            cs_matrix = [cs for cs in composition_sets if cs.phase_record.phase_name == self.phases[0]][0]
+            x_matrix = np.array(cs_matrix.X)
 
-        self.LogSurrDc = None
-        self.LogSurrMc = None
-        self.LogSurrBeta = None
-        self.LogSurrCa = None
-        self.LogSurrCb = None
-        self.LogSurrGba = None
+            ele = list(cs_precip.phase_record.nonvacant_elements)
+        else:
+            return None
         
-        self.SurrogateDc = None
-        self.SurrogateMc = None
-        self.SurrogateBeta = None
-        self.SurrogateCa = None
-        self.SurrogateCb = None
-        self.SurrogateGba = None
+        return ph, ele, chemical_potentials, composition_sets, cs_matrix, x_matrix, cs_precip, x_precip
+    
+    def _getPrecCompositionSetSamplingDF(self, x, T, cond, precPhase = None, training = False):
+        '''
+        Gets samples for precipitate phase for use in sampling driving force method and returns driving force and precipitate composition
 
-        with open(fileName, 'wb') as file:
-            pickle.dump(self, file)
+        This is also use in tangent driving force method for when equilibrium is not (yet) cached
 
-        if self.TDGscale is not None:
-            self._createDGSurrogate()
-        if self.TICscale is not None:
-            self._createICSurrogate()
-
-    def load(fileName):
-        '''
-        Loads data from a pickled surrogate and builds driving force and curvature functions
+        Steps
+            1. Compute local equilibrium at x and T of only the matrix phase
+            2. Sample precipitate phase
+                If ordered contribution to matrix phase, then sample ordering contribution
+                and remove points on the matrix free energy surface
+            3. Compute energy difference between precipitate samples and chemical potential hyperplane
+            4. Find sample that maximizes energy difference and return sample composition and driving force
 
         Parameters
         ----------
-        fileName : str
+        x : float or array
+            Composition of minor element in bulk matrix phase
+            Use float for binary systems
+            Use array for multicomponent systems
+        T : float
+            Temperature in K
+        precPhase : str (optional)
+            Precipitate phase to consider (default is first precipitate phase in list)
+        returnComp : bool (optional)
+            Whether to return composition of precipitate (defaults to False)
+        training : bool (optional)
+            If True, this will not cache any equilibrium
+            This is used for training since training points may not be near each other
 
         Returns
         -------
-        MulticomponentSurrogate object
+        driving force - max free energy difference
+        precipitate composition - corresponds to max driving force
         '''
-        surr = None
-        with open(fileName, 'rb') as file:
-            surr = pickle.load(file)
-
-        if surr.TDGscale is not None:
-            surr._createDGSurrogate()
-        if surr.TICscale is not None:
-            surr._createICSurrogate()
+        orderTol = -1e-8
+
+        #Equilibrium at matrix composition for only the parent phase
+        self._parentEq, self._matrix_cs = local_equilibrium(self.db, self.elements, [self.phases[0]], cond,
+                                                            self.models, self.phase_records,
+                                                            composition_sets = self._matrix_cs)
+
+        if any(np.isnan(self._parentEq.chemical_potentials)):
+            return None
+        
+        #Sample precipitate phase and get driving force differences at all points -------------------------------------------------------------------
+        #Sample points of precipitate phase
+        if self._pointsPrec[precPhase] is None or self._prevTemperature != T:
+            self._pointsPrec[precPhase] = calculate(self.db, self.elements, precPhase, P = 101325, T = T, GE=self.gOffset, pdens = self.sampling_pDens, model=self.models, output='GM', phase_records=self.phase_records)
+            if self.orderedPhase[precPhase]:
+                self._orderingPoints[precPhase] = calculate(self.db, self.elements, precPhase, P = 101325, T = T, GE=self.gOffset, pdens = self.sampling_pDens, model=self.models, output='OCM', phase_records=self.OCMphase_records[precPhase])
+            self._prevTemperature = T
+
+        #Get value of chemical potential hyperplane at composition of sampled points
+        precComp = self._pointsPrec[precPhase].X.values.ravel()
+        precComp = precComp.reshape((int(len(precComp) / (len(self.elements) - 1)), len(self.elements) - 1))
+        mu = np.array([self._parentEq.chemical_potentials])
+        mult = precComp * mu
+
+        #Difference between the chemical potential hyperplane and the samples points
+        #The max driving force is the same as when the chemical potentials of the two phases are parallel
+        diff = np.sum(mult, axis=1) - self._pointsPrec[precPhase].GM.values.ravel()
+            
+        #Find maximum driving force and corresponding composition -----------------------------------------------------------------------------------
+        #For phases with order/disorder transition, a filter is applied such that it will only use points that are below the disordered energy surface
+        if self.orderedPhase[precPhase]:
+            indices = self._orderingPoints[precPhase].OCM.values.ravel() < orderTol
+            diff = diff[indices]
+
+        dg = np.amax(diff)
+        idx = np.argmax(diff)
+
+        prec_cs = CompositionSet(self.phase_records[precPhase])
+        state_variables = np.array([cond[v.GE], cond[v.N], cond[v.P], cond[v.T]], dtype=np.float64)
+        #state_variables = np.array([-dg, cond[v.N], cond[v.P], cond[v.T]], dtype=np.float64)
+        if self.orderedPhase[precPhase]:
+            y = np.squeeze(self._pointsPrec[precPhase].Y.values)
+            y = y[indices][idx]
+        else:
+            y = np.array(self._pointsPrec[precPhase].Y.isel(points=idx).values.ravel())
+        prec_cs.update(y, 1, state_variables)
 
-        return surr
-        
+        return dg, prec_cs
```

### Comparing `kawin-0.2.0/kawin/tests/test_PBM.py` & `kawin-0.3.0/kawin/tests/test_PBM.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from numpy.testing import assert_allclose
-from kawin.PopulationBalance import PopulationBalanceModel
+from kawin.precipitation import PopulationBalanceModel
 
 #Set parameters for pbm. Default bins are increased here so that added bins should be 50
 bins = 200
 qBins = int(200/4)
 minBins = 100
 maxBins = 300
 pbm = PopulationBalanceModel(1e-10, 1e-8, 200, 100, 300)
@@ -68,43 +68,21 @@
     assert_allclose(pbm.PSDbounds[-1], finalLength, rtol=1e-6)
     assert_allclose(pbm.max, finalLength, rtol=1e-6)
     assert(len(pbm.PSDbounds) == maxBins+1)
     assert(len(pbm.PSDsize) == maxBins)
     assert_allclose(pbm.PSDsize[0], 0.5*(pbm.PSDbounds[0] + pbm.PSDbounds[1]), atol=0, rtol=1e-6)
     pbm.reset()
 
-def test_nucleateSmall():
-    '''
-    If nucleate radius is smaller than PSD length, then no change
-    '''
-    pbm.Nucleate(10, 1e-9)
-    assert(len(pbm.PSD) == bins and pbm.bins == len(pbm.PSD))
-    assert(len(pbm.PSDbounds) == bins+1)
-    assert(len(pbm.PSDsize) == bins)
-    assert(pbm.Moment(0) == 10)
-    assert(pbm.PSDbounds[-1] == 1e-8)
-
-def test_nucleateBig():
-    '''
-    If nucleate radius is larger than PSD length, then increase bin size
-    such that number of bins is the same, but max if 5*radius
-    '''
-    r = 1e-7
-    pbm.Nucleate(10, r)
-    assert(len(pbm.PSD) == bins and pbm.bins == len(pbm.PSD))
-    assert(len(pbm.PSDbounds) == bins+1)
-    assert(len(pbm.PSDsize) == bins)
-    assert(pbm.Moment(0) == 10)
-    assert_allclose(pbm.PSDbounds[-1], 5*r, rtol=1e-6)
-    assert_allclose(pbm.PSDsize[0], 0.5*(pbm.PSDbounds[0] + pbm.PSDbounds[1]), atol=0, rtol=1e-6)
-    pbm.reset()
-
 def test_DT():
     '''
     Calculated DT with constant growth rate
-    DT = binSize / (2*max(growth rate))
+    DT = ratio * binSize / (max(growth rate))
+
+    Previous version had ratio of 0.5, but this was decreased slightly to 0.4 for numerical stability
     '''
     growth = 5*np.ones(pbm.bins+1)
     pbm.PSD = 2*np.ones(pbm.bins)
-    trueDT = (pbm.PSDbounds[1] - pbm.PSDbounds[0]) / (2*growth[0])
-    calcDT = pbm.getDTEuler(5, growth, 1e-3, 0)
+    ratio = 0.4
+    trueDT = ratio * (pbm.PSDbounds[1] - pbm.PSDbounds[0]) / (growth[0])
+    dissIndex = pbm.getDissolutionIndex(1e-3, 0)
+    calcDT = pbm.getDTEuler(5, growth, dissIndex, maxBinRatio=ratio)
     assert_allclose(trueDT, calcDT, rtol=1e-6)
```

### Comparing `kawin-0.2.0/kawin/tests/test_strength.py` & `kawin-0.3.0/kawin/tests/test_strength.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from kawin.Strength import StrengthModel
+from kawin.precipitation.coupling import StrengthModel
 import numpy as np
 
 sm = StrengthModel()
 G, b, nu = 79.3e9, 0.25e-9, 1/3
 bp, ri = b, 2*b
 eps, Gp = 0.001, 70e9
 yAPB, ySFM, ySFP, gamma = 0.04, 0.1, 0.05, 0.5
```

### Comparing `kawin-0.2.0/kawin/tests/test_surrogate.py` & `kawin-0.3.0/kawin/tests/test_surrogate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from numpy.testing import assert_allclose
 import numpy as np
 import os
-from kawin.Thermodynamics import BinaryThermodynamics, MulticomponentThermodynamics
-from kawin.Surrogate import BinarySurrogate, MulticomponentSurrogate
+from kawin.thermo import BinaryThermodynamics, MulticomponentThermodynamics, BinarySurrogate, MulticomponentSurrogate
 from kawin.tests.datasets import *
 
 AlZrTherm = BinaryThermodynamics(ALZR_TDB, ['AL', 'ZR'], ['FCC_A1', 'AL3ZR'], drivingForceMethod='approximate')
 NiCrAlTherm = MulticomponentThermodynamics(NICRAL_TDB, ['NI', 'CR', 'AL'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='approximate')
 
 #Set constant sampling densities for each Thermodynamics object
 #pycalphad equilibrium results may change based off sampling density, so this is to make sure
```

### Comparing `kawin-0.2.0/kawin/tests/test_thermodynamics.py` & `kawin-0.3.0/kawin/tests/test_thermodynamics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import numpy as np
 from numpy.testing import assert_allclose
-from kawin.Thermodynamics import BinaryThermodynamics, GeneralThermodynamics, MulticomponentThermodynamics
+from kawin.thermo import GeneralThermodynamics, BinaryThermodynamics, MulticomponentThermodynamics
 from kawin.tests.datasets import *
 from pycalphad import Database
 
-AlZrTherm = BinaryThermodynamics(ALZR_TDB, ['AL', 'ZR'], ['FCC_A1', 'AL3ZR'], drivingForceMethod='approximate')
-NiCrAlTherm = MulticomponentThermodynamics(NICRAL_TDB, ['NI', 'CR', 'AL'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='approximate')
-NiCrAlThermDiff = MulticomponentThermodynamics(NICRAL_TDB_DIFF, ['NI', 'CR', 'AL'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='approximate')
-NiAlCrTherm = MulticomponentThermodynamics(NICRAL_TDB, ['NI', 'AL', 'CR'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='approximate')
-NiAlCrThermDiff = MulticomponentThermodynamics(NICRAL_TDB_DIFF, ['NI', 'AL', 'CR'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='approximate')
-AlCrNiTherm = MulticomponentThermodynamics(NICRAL_TDB, ['AL', 'CR', 'NI'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='approximate')
+#Default driving force method will be 'tangent'
+AlZrTherm = BinaryThermodynamics(ALZR_TDB, ['AL', 'ZR'], ['FCC_A1', 'AL3ZR'], drivingForceMethod='tangent')
+NiCrAlTherm = MulticomponentThermodynamics(NICRAL_TDB, ['NI', 'CR', 'AL'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='tangent')
+NiCrAlThermDiff = MulticomponentThermodynamics(NICRAL_TDB_DIFF, ['NI', 'CR', 'AL'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='tangent')
+NiAlCrTherm = MulticomponentThermodynamics(NICRAL_TDB, ['NI', 'AL', 'CR'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='tangent')
+NiAlCrThermDiff = MulticomponentThermodynamics(NICRAL_TDB_DIFF, ['NI', 'AL', 'CR'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='tangent')
+AlCrNiTherm = MulticomponentThermodynamics(NICRAL_TDB, ['AL', 'CR', 'NI'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='tangent')
 
 #Set constant sampling densities for each Thermodynamics object
 #pycalphad equilibrium results may change based off sampling density, so this is to make sure
 #tests won't failed unneccesarily because the default sampling densities are modified
 AlZrTherm.setDFSamplingDensity(2000)
 AlZrTherm.setEQSamplingDensity(500)
 NiCrAlTherm.setDFSamplingDensity(2000)
@@ -26,53 +27,67 @@
 NiAlCrThermDiff.setEQSamplingDensity(500)
 AlCrNiTherm.setDFSamplingDensity(2000)
 AlCrNiTherm.setEQSamplingDensity(500)
 
 def test_DG_binary():
     '''
     Checks value of binary driving force calculation
+
+    Driving force value was updated due to switch from approximate to tangent method
     '''
     dg, _ = AlZrTherm.getDrivingForce(0.004, 673.15, training = True)
-    assert_allclose(dg, 6346.929428, atol=0, rtol=1e-3)
+    assert_allclose(dg, 6346.930428, atol=0, rtol=1e-3)
 
 def test_DG_binary_output():
     '''
     Checks that output of binary driving force calculation follows input
     Ex. for f(x, T) -> (dg, xP)
         (scalar, scalar) input -> scalar
         (array, array) input -> array
     '''
-    dg, xP = AlZrTherm.getDrivingForce(0.004, 673.15, returnComp=True, training = True)
-    dgarray, xParray = AlZrTherm.getDrivingForce([0.004, 0.005], [673.15, 683.15], returnComp=True, training = True)
+    methods = ['sampling', 'approximate', 'curvature', 'tangent']
+    for m in methods:
+        AlZrTherm.setDrivingForceMethod(m)
+        dg, xP = AlZrTherm.getDrivingForce(0.004, 673.15, returnComp=True, training = True)
+        dgarray, xParray = AlZrTherm.getDrivingForce([0.004, 0.005], [673.15, 683.15], returnComp=True, training = True)
+
+        assert np.isscalar(dg) or (type(dg) == np.ndarray and dg.ndim == 0)
+        assert np.isscalar(xP) or (type(xP) == np.ndarray and xP.ndim == 0)
+        assert hasattr(dgarray, '__len__') and len(dgarray) == 2
+        assert hasattr(xParray, '__len__') and len(xParray) == 2
 
-    assert np.isscalar(dg) or (type(dg) == np.ndarray and dg.ndim == 0)
-    assert np.isscalar(xP) or (type(xP) == np.ndarray and xP.ndim == 0)
-    assert hasattr(dgarray, '__len__') and len(dgarray) == 2
-    assert hasattr(xParray, '__len__') and len(xParray) == 2
+    AlZrTherm.setDrivingForceMethod('tangent')
 
 def test_DG_ternary():
     '''
     Checks value of ternary driving force calculation
+
+    Driving force value was updated due to switch from approximate to tangent method
     '''
     dg, _ = NiCrAlTherm.getDrivingForce([0.08, 0.1], 1073.15, training = True)
-    assert_allclose(dg, 244.012027, atol=0, rtol=1e-3)
+    assert_allclose(dg, 265.779087, atol=0, rtol=1e-3)
 
 def test_DG_ternary_output():
     '''
     Checks that output of ternary driving force calculations follow input
     Ex. for f(x, T) -> (dg, xP)
         (array, scalar) -> scalar
         (2D array, array) -> array
     '''
-    dg, xP = NiCrAlTherm.getDrivingForce([0.08, 0.1], 1073.15, returnComp=True, training = True)
-    dgarray, xParray = NiCrAlTherm.getDrivingForce([[0.08, 0.1], [0.085, 0.1], [0.09, 0.1]], [1073.15, 1078.15, 1083.15], returnComp=True, training = True)
-    assert np.isscalar(dg) or (type(dg) == np.ndarray and dg.ndim == 0)
-    assert xP.ndim == 1 and len(xP) == 2
-    assert hasattr(dgarray, '__len__')
-    assert xParray.shape == (3, 2)
+    methods = ['sampling', 'approximate', 'curvature', 'tangent']
+    for m in methods:
+        NiCrAlTherm.setDrivingForceMethod(m)
+        dg, xP = NiCrAlTherm.getDrivingForce([0.08, 0.1], 1073.15, returnComp=True, training = True)
+        dgarray, xParray = NiCrAlTherm.getDrivingForce([[0.08, 0.1], [0.085, 0.1], [0.09, 0.1]], [1073.15, 1078.15, 1083.15], returnComp=True, training = True)
+        assert np.isscalar(dg) or (type(dg) == np.ndarray and dg.ndim == 0)
+        assert xP.ndim == 1 and len(xP) == 2
+        assert hasattr(dgarray, '__len__')
+        assert xParray.shape == (3, 2)
+
+    NiCrAlTherm.setDrivingForceMethod('tangent')
 
 def test_DG_ternary_order():
     '''
     Check that driving force is the same given that the order of input elements and composition are the same
     Ex. Input elements as [Ni, Cr, Al] should require composition to be [Cr, Al]
         Input elements as [Ni, Al, Cr] should require composition to be [Al, Cr]
         Input elements as [Al, Cr, Ni] should require composition to be [Cr, Ni]
@@ -101,24 +116,29 @@
     '''
     Checks that output of interfacial composition follows input
     Ex. For f(T, g) -> (xM, xP)
         (scalar, scalar) -> (scalar, scalar)
         (array, array) -> (array, array)
         (scalar, array) -> (array, array)   Special case where T is scalar
     '''
-    xm, xp = AlZrTherm.getInterfacialComposition(673.15, 5000)
-    xmarray, xparray = AlZrTherm.getInterfacialComposition([673.15, 683.15], [5000, 50000])
-    xmarray2, xparray2 = AlZrTherm.getInterfacialComposition(673.15, [5000, 50000])
-
-    assert np.isscalar(xm) or (type(xm) == np.ndarray and xm.ndim == 0)
-    assert np.isscalar(xp) or (type(xp) == np.ndarray and xp.ndim == 0)
-    assert hasattr(xmarray, '__len__') and len(xmarray) == 2
-    assert hasattr(xparray, '__len__') and len(xparray) == 2
-    assert hasattr(xmarray2, '__len__') and len(xmarray2) == 2
-    assert hasattr(xparray2, '__len__') and len(xparray2) == 2
+    methods = ['curvature', 'equilibrium']
+    for m in methods:
+        AlZrTherm.setInterfacialMethod(m)
+        xm, xp = AlZrTherm.getInterfacialComposition(673.15, 5000)
+        xmarray, xparray = AlZrTherm.getInterfacialComposition([673.15, 683.15], [5000, 50000])
+        xmarray2, xparray2 = AlZrTherm.getInterfacialComposition(673.15, [5000, 50000])
+
+        assert np.isscalar(xm) or (type(xm) == np.ndarray and xm.ndim == 0)
+        assert np.isscalar(xp) or (type(xp) == np.ndarray and xp.ndim == 0)
+        assert hasattr(xmarray, '__len__') and len(xmarray) == 2
+        assert hasattr(xparray, '__len__') and len(xparray) == 2
+        assert hasattr(xmarray2, '__len__') and len(xmarray2) == 2
+        assert hasattr(xparray2, '__len__') and len(xparray2) == 2
+
+    AlZrTherm.setInterfacialMethod('equilibrium')
 
 def test_Mob_binary():
     '''
     Checks value of binary interdiffusvity calculation
     '''
     dnkj = AlZrTherm.getInterdiffusivity(0.004, 673.15)
     assert_allclose(dnkj, 1.280344e-20, atol=0, rtol=1e-3)
```

### Comparing `kawin-0.2.0/kawin.egg-info/PKG-INFO` & `kawin-0.3.0/kawin.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kawin
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tool for simulating precipitation using the KWN model coupled with Calphad.
 Home-page: https://kawin.org/
 Author: Nicholas Ury
 Author-email: nury12n@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -14,19 +14,28 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: matplotlib>=3.3
+Requires-Dist: numpy>=1.13
+Requires-Dist: pycalphad>=0.10.1
+Requires-Dist: scipy
+Requires-Dist: setuptools_scm[toml]>=6.0
 
 # kawin
 
 Python implementation of the Kampmann-Wagner Numerical (KWN) model to predict precipitate nucleation and growth behavior. This package couples with pycalphad to perform thermodynamic and kinetic calculations.
 
+Notes
+-----
+There are some API changes between kawin 0.3.0 and 0.2.0. Please see the examples for more details.
+
 Installation
 ------------
 `pip install kawin`
 
 Examples
 --------
 Examples on Jupyter notebooks can be found on [NBViewer](https://nbviewer.org/github/materialsgenomefoundation/kawin/tree/main/examples/).
```

### Comparing `kawin-0.2.0/setup.py` & `kawin-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='kawin',
     author='Nicholas Ury',
     author_email='nury12n@gmail.com',
     description='Tool for simulating precipitation using the KWN model coupled with Calphad.',
-    packages=['kawin', 'kawin.tests'],
+    packages=['kawin', 'kawin.tests', 'kawin.diffusion', 'kawin.precipitation', 'kawin.precipitation.coupling', 'kawin.precipitation.non_ideal', 'kawin.solver', 'kawin.thermo'],
     license='MIT',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     url='https://kawin.org/',
-    version='0.2.0',
+    version='0.3.0',
     install_requires=[
         'matplotlib>=3.3',
         'numpy>=1.13',
         'pycalphad>=0.10.1',
         'scipy',
         'setuptools_scm[toml]>=6.0',
     ],
```

