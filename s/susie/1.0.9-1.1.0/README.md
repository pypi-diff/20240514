# Comparing `tmp/susie-1.0.9.tar.gz` & `tmp/susie-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "susie-1.0.9.tar", last modified: Mon Apr 15 19:27:02 2024, max compression
+gzip compressed data, was "susie-1.1.0.tar", last modified: Tue May 14 18:50:06 2024, max compression
```

## Comparing `susie-1.0.9.tar` & `susie-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-04-15 19:27:02.952117 susie-1.0.9/
--rw-r--r--   0 maliabarker   (501) staff       (20)     1065 2023-09-18 19:40:07.000000 susie-1.0.9/LICENSE.txt
--rw-r--r--   0 maliabarker   (501) staff       (20)    12234 2024-04-15 19:27:02.952013 susie-1.0.9/PKG-INFO
--rw-r--r--   0 maliabarker   (501) staff       (20)    10299 2024-03-27 19:16:09.000000 susie-1.0.9/README.md
--rw-r--r--   0 maliabarker   (501) staff       (20)       84 2023-10-09 21:44:27.000000 susie-1.0.9/pyproject.toml
--rw-r--r--   0 maliabarker   (501) staff       (20)      949 2024-04-15 19:27:02.952616 susie-1.0.9/setup.cfg
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-04-15 19:27:02.947420 susie-1.0.9/src/
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-04-15 19:27:02.949382 susie-1.0.9/src/susie/
--rw-r--r--   0 maliabarker   (501) staff       (20)       36 2023-08-31 20:39:34.000000 susie-1.0.9/src/susie/__init__.py
--rw-r--r--   0 maliabarker   (501) staff       (20)    37916 2024-04-15 19:23:11.000000 susie-1.0.9/src/susie/ephemeris.py
--rw-r--r--   0 maliabarker   (501) staff       (20)    14811 2024-04-15 18:59:39.000000 susie-1.0.9/src/susie/transit_times.py
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-04-15 19:27:02.951569 susie-1.0.9/src/susie.egg-info/
--rw-r--r--   0 maliabarker   (501) staff       (20)    12234 2024-04-15 19:27:02.000000 susie-1.0.9/src/susie.egg-info/PKG-INFO
--rw-r--r--   0 maliabarker   (501) staff       (20)      334 2024-04-15 19:27:02.000000 susie-1.0.9/src/susie.egg-info/SOURCES.txt
--rw-r--r--   0 maliabarker   (501) staff       (20)        1 2024-04-15 19:27:02.000000 susie-1.0.9/src/susie.egg-info/dependency_links.txt
--rw-r--r--   0 maliabarker   (501) staff       (20)       31 2024-04-15 19:27:02.000000 susie-1.0.9/src/susie.egg-info/requires.txt
--rw-r--r--   0 maliabarker   (501) staff       (20)        6 2024-04-15 19:27:02.000000 susie-1.0.9/src/susie.egg-info/top_level.txt
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-04-15 19:27:02.950975 susie-1.0.9/tests/
--rw-r--r--   0 maliabarker   (501) staff       (20)     7689 2024-04-01 20:05:34.000000 susie-1.0.9/tests/test_ephemeris.py
--rw-r--r--   0 maliabarker   (501) staff       (20)    20366 2024-03-25 19:15:32.000000 susie-1.0.9/tests/test_transit_times.py
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-14 18:50:06.212435 susie-1.1.0/
+-rw-r--r--   0 maliabarker   (501) staff       (20)     1065 2023-09-18 19:40:07.000000 susie-1.1.0/LICENSE.txt
+-rw-r--r--   0 maliabarker   (501) staff       (20)    12234 2024-05-14 18:50:06.212073 susie-1.1.0/PKG-INFO
+-rw-r--r--   0 maliabarker   (501) staff       (20)    10299 2024-03-27 19:16:09.000000 susie-1.1.0/README.md
+-rw-r--r--   0 maliabarker   (501) staff       (20)       84 2023-10-09 21:44:27.000000 susie-1.1.0/pyproject.toml
+-rw-r--r--   0 maliabarker   (501) staff       (20)      949 2024-05-14 18:50:06.212913 susie-1.1.0/setup.cfg
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-14 18:50:06.203427 susie-1.1.0/src/
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-14 18:50:06.207176 susie-1.1.0/src/susie/
+-rw-r--r--   0 maliabarker   (501) staff       (20)       36 2023-08-31 20:39:34.000000 susie-1.1.0/src/susie/__init__.py
+-rw-r--r--   0 maliabarker   (501) staff       (20)    43305 2024-05-14 18:44:33.000000 susie-1.1.0/src/susie/ephemeris.py
+-rw-r--r--   0 maliabarker   (501) staff       (20)    22474 2024-05-13 21:14:53.000000 susie-1.1.0/src/susie/timing_data.py
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-14 18:50:06.211629 susie-1.1.0/src/susie.egg-info/
+-rw-r--r--   0 maliabarker   (501) staff       (20)    12234 2024-05-14 18:50:06.000000 susie-1.1.0/src/susie.egg-info/PKG-INFO
+-rw-r--r--   0 maliabarker   (501) staff       (20)      332 2024-05-14 18:50:06.000000 susie-1.1.0/src/susie.egg-info/SOURCES.txt
+-rw-r--r--   0 maliabarker   (501) staff       (20)        1 2024-05-14 18:50:06.000000 susie-1.1.0/src/susie.egg-info/dependency_links.txt
+-rw-r--r--   0 maliabarker   (501) staff       (20)       31 2024-05-14 18:50:06.000000 susie-1.1.0/src/susie.egg-info/requires.txt
+-rw-r--r--   0 maliabarker   (501) staff       (20)        6 2024-05-14 18:50:06.000000 susie-1.1.0/src/susie.egg-info/top_level.txt
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-05-14 18:50:06.210902 susie-1.1.0/tests/
+-rw-r--r--   0 maliabarker   (501) staff       (20)    22468 2024-05-14 18:44:23.000000 susie-1.1.0/tests/test_ephemeris.py
+-rw-r--r--   0 maliabarker   (501) staff       (20)    27292 2024-05-14 18:44:11.000000 susie-1.1.0/tests/test_transit_times.py
```

### Comparing `susie-1.0.9/LICENSE.txt` & `susie-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `susie-1.0.9/PKG-INFO` & `susie-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: susie
-Version: 1.0.9
+Version: 1.1.0
 Summary: Susie allows users to input exoplanet transit data and return information detailing possible tidal decay.
 Author: Malia Barker, Holly VanLooy, Adrienne Kirk
 Author-email: maliabarker@icloud.com, hollyvanlooy@u.boisestate.edu, adriennekirk@u.boisestate.edu
 Project-URL: Bug Tracker, https://github.com/BoiseStatePlanetary/susie/issues
 Project-URL: Repository, https://github.com/BoiseStatePlanetary/susie/
 Project-URL: Documentation, https://susie.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
-Requires-Dist: scipy
+Requires-Dist: lmfit
 Requires-Dist: matplotlib
 Requires-Dist: astropy
 
 # The Susie Python Package
 A package for exoplanet transit decay calculations and visualizations.
 
 https://susie.readthedocs.io/en/latest/
```

### Comparing `susie-1.0.9/README.md` & `susie-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `susie-1.0.9/setup.cfg` & `susie-1.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = susie
-version = 1.0.9
+version = 1.1.0
 author = Malia Barker, Holly VanLooy, Adrienne Kirk
 author_email = maliabarker@icloud.com, hollyvanlooy@u.boisestate.edu, adriennekirk@u.boisestate.edu
 description = Susie allows users to input exoplanet transit data and return information detailing possible tidal decay.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 project_urls = 
 	Bug Tracker = https://github.com/BoiseStatePlanetary/susie/issues
@@ -18,15 +18,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy
-	scipy
+	lmfit
 	matplotlib
 	astropy
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `susie-1.0.9/src/susie/ephemeris.py` & `susie-1.1.0/src/susie/ephemeris.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from abc import ABC, abstractmethod
-from scipy.optimize import curve_fit
 import numpy as np
 import matplotlib.pyplot as plt
-# from transit_times import TransitTimes
-from susie.transit_times import TransitTimes
+from lmfit import Model
+from susie.timing_data import TimingData # REMEMBER TO COMMENT THIS OUT BEFORE GIT PUSHES
+# from susie.transit_times import TransitTimes
 
 class BaseModelEphemeris(ABC):
     """Abstract class that defines the structure of different model ephemeris classes."""
     @abstractmethod
-    def fit_model(self, x, y, yerr, **kwargs):
+    def fit_model(self, x, y, yerr, tra_or_occ, **kwargs):
         """Fits a model ephemeris to transit data.
 
+        TODO: Update docstring
         Defines the structure for fitting a model (linear or quadratic) to transit data. 
         All subclasses must implement this method.
 
         Parameters
         ----------
             x : numpy.ndarray[int]
                 The epoch data as recieved from the TransitTimes object.
@@ -29,40 +30,51 @@
 
         """
         pass
 
 
 class LinearModelEphemeris(BaseModelEphemeris):
     """Subclass of BaseModelEphemeris that implements a linear fit."""
-    def lin_fit(self, x, P, T0):
+    def lin_fit(self, E, P, T0, tra_or_occ):
         """Calculates a linear function with given data.
-
-        Uses the equation (Period * mid transit times + initial epoch) as a linear function for SciPy's 
+        TODO: Update docstring
+        Uses the equation (Period * epochs + initial mid time) as a linear function for SciPy's 
         curve_fit method.
         
         Parameters
         ----------
 
-            x: numpy.ndarray[float]
-                The mid-transit times.
-            P : float
+            E: numpy.ndarray[float]
+                The epochs.
+            P: float
                 The exoplanet transit period.
-            T0 : float
-                The initial epoch associated with a mid-transit time.
+            T0: float
+                The initial mid time.
         
         Returns
         -------
-            P*x + T0 : numpy.ndarray[float]
-                A linear function calculated with TransitTimes object data to be used with curve_fit.
-        """
-        return P*x + T0
+            result: numpy.ndarray[float]
+                A linear function calculated with the TimingData object, returned as:
+                    P*E + T0 if the data point is an observed transit (denoted by 0)
+                    P*E + (T0 + 0.5*P) if the data point is an observed occultation (denoted by 1)
+        """
+        result = np.zeros_like(E)
+        for i, t_type in enumerate(tra_or_occ):
+            if t_type == 0:
+                # transit data
+                result[i] = P*E[i] + T0
+            elif t_type == 1:
+                # occultation data
+                result[i] = P*E[i] + (T0 + 0.5*P)
+        return result
     
-    def fit_model(self, x, y, yerr, **kwargs):
+    def fit_model(self, x, y, yerr, tra_or_occ, **kwargs):
         """Fits a linear model to ephemeris data.
 
+        TODO: Update docstring
         Compares the model ephemieris data to the linear fit created by data in TransitTimes object calculated 
         with lin_fit method. Then creates a curve fit which minimizes the difference between the two sets of data.
         Curve fit then returns the parameters of the linear function corresponding to period, conjunction time, 
         and their respective errors. These parameters are returned in a dictionary to the user for further use.
 
         Parameters
         ----------
@@ -82,32 +94,33 @@
             
             Example:
                 * 'period': An array of exoplanet periods over time corresponding to epochs (in units of days),
                 * 'period_err': The uncertainities associated with period (in units of days),
                 * 'conjunction_time': The time of conjunction of exoplanet transit over time corresponding to epochs,
                 * 'conjunction_time_err': The uncertainties associated with conjunction_time
         """
-        # Will come back in units of y/x (so will be in days), period is days per orbit (but rly this is days bc orbit is unitless)
-        popt, pcov = curve_fit(self.lin_fit, x, y, sigma=yerr, absolute_sigma=True, **kwargs)
-        unc = np.sqrt(np.diag(pcov))
+        tra_or_occ_enum = [0 if i == 'tra' else 1 for i in tra_or_occ]
+        model = Model(self.lin_fit, independent_vars=['E', 'tra_or_occ'])
+        # TODO: Should we set this as the base estimate for T0 and P or should we try to find a good estimate to start with?
+        params = model.make_params(T0=0., P=1.091423, tra_or_occ=tra_or_occ_enum)
+        result = model.fit(y, params, weights=1.0/yerr, E=x, tra_or_occ=tra_or_occ_enum)
         return_data = {
-            'period': popt[0],
-            'period_err': unc[0],
-            'conjunction_time': popt[1],
-            'conjunction_time_err': unc[1]
+            'period': result.params['P'].value,
+            'period_err': result.params['P'].stderr,
+            'conjunction_time': result.params['T0'].value,
+            'conjunction_time_err': result.params['T0'].stderr
         }
         return(return_data)
 
-# TODO: Check the units for each thing in here (are times given in days, seconds?)
-
 class QuadraticModelEphemeris(BaseModelEphemeris):
     """Subclass of BaseModelEphemeris that implements a quadratic fit."""
-    def quad_fit(self, x, dPdE, P, T0):
+    def quad_fit(self, E, dPdE, P, T0, tra_or_occ):
         """Calculates a quadratic function with given data.
 
+        TODO: Update docstring
         Uses the equation (0.5 * change in period over epoch * mid transit times^2 + Period * mid transit times + initial epoch) 
         as a quadratic function for SciPy's curve_fit method.
         
         Parameters
         ----------
             x: numpy.ndarray[int]
                 The mid-transit times.
@@ -120,19 +133,28 @@
         
         Returns
         -------
             0.5*dPdE*x*x + P*x + T0: numpy.ndarray[float]
                 A list of quadratic function values calculated with TransitTimes object data to be 
                 used with curve_fit.
         """
-        return 0.5*dPdE*x*x + P*x + T0
+        result = np.zeros_like(E)
+        for i, t_type in enumerate(tra_or_occ):
+            if t_type == 0:
+                # transit data
+                result[i] = T0 + P*E[i] + 0.5*dPdE*E[i]*E[i] 
+            elif t_type == 1:
+                # occultation data
+                result[i] = (T0 + 0.5*P) + P*E[i] + 0.5*dPdE*E[i]*E[i] 
+        return result
     
-    def fit_model(self, x, y, yerr, **kwargs):
+    def fit_model(self, x, y, yerr, tra_or_occ, **kwargs):
         """Fits a quadratic model to ephemeris data.
 
+        TODO: Update docstring
         Compares the model ephemeris data to the quadratic fit calculated with quad_fit method. Then creates a 
         curve fit which minimizes the difference between the two sets of data. Curve fit then returns the 
         parameters of the quadratic function corresponding to period, conjunction time, period change by epoch, 
         and their respective errors. These parameters are returned in a dictionary to the user for further use.
 
         Parameters
         ----------
@@ -152,32 +174,36 @@
                 * 'period': An array of exoplanet periods over time corresponding to epochs (in units of days),
                 * 'period_err': The uncertainities associated with period (in units of days),
                 * 'conjunction_time': The time of conjunction of exoplanet transit over time corresponding to epochs,
                 * 'conjunction_time_err': The uncertainties associated with conjunction_time,
                 * 'period_change_by_epoch': The exoplanet period change over epochs, from first epoch to current epoch (in units of days),
                 * 'period_change_by_epoch_err': The uncertainties associated with period_change_by_epoch (in units of days)
         """
-        popt, pcov = curve_fit(self.quad_fit, x, y, sigma=yerr, absolute_sigma=True, **kwargs)
-        unc = np.sqrt(np.diag(pcov))
+        tra_or_occ_enum = [0 if i == 'tra' else 1 for i in tra_or_occ]
+        model = Model(self.quad_fit, independent_vars=['E', 'tra_or_occ'])
+        # TODO: Should we set this as the base estimate for T0 and P or should we try to find a good estimate to start with?
+        params = model.make_params(T0=0., P=1.091423, dPdE=0., tra_or_occ=tra_or_occ_enum)
+        result = model.fit(y, params, weights=1.0/yerr, E=x, tra_or_occ=tra_or_occ_enum)
         return_data = {
-            'conjunction_time': popt[2],
-            'conjunction_time_err': unc[2],
-            'period': popt[1],
-            'period_err': unc[1],
-            'period_change_by_epoch': popt[0],
-            'period_change_by_epoch_err': unc[0],
+            'period': result.params['P'].value,
+            'period_err': result.params['P'].stderr,
+            'conjunction_time': result.params['T0'].value,
+            'conjunction_time_err': result.params['T0'].stderr,
+            'period_change_by_epoch': result.params['dPdE'].value,
+            'period_change_by_epoch_err': result.params['dPdE'].stderr
         }
         return(return_data)
 
 class ModelEphemerisFactory:
     """Factory class for selecting which type of ephemeris class (linear or quadratic) to use."""
     @staticmethod
-    def create_model(model_type, x, y, yerr, **kwargs):
+    def create_model(model_type, x, y, yerr, tra_or_occ, **kwargs):
         """Instantiates the appropriate BaseModelEphemeris subclass and runs fit_model method.
 
+        TODO: Update docstring
         Based on the given user input of model type (linear or quadratic) the factory will create the 
         corresponding subclass of BaseModelEphemeris and run the fit_model method to recieve the model 
         ephemeris return data dictionary.
         
         Parameters
         ----------
             model_type: str
@@ -211,79 +237,82 @@
         models = {
             'linear': LinearModelEphemeris(),
             'quadratic': QuadraticModelEphemeris()
         }
         if model_type not in models:
             raise ValueError(f"Invalid model type: {model_type}")
         model = models[model_type]
-        return model.fit_model(x, y, yerr, **kwargs)
+        return model.fit_model(x, y, yerr, tra_or_occ, **kwargs)
 
 
 class Ephemeris(object):
     """Represents the model ephemeris using transit midpoint data over epochs.
-
+    TODO: Update docstring
     Parameters
     -----------
     transit_times: TransitTimes obj
         A successfully instantiated TransitTimes object holding epochs, mid transit times, and uncertainties.
         
     Raises
     ----------
      ValueError:
         Raised if transit_times is not an instance of the TransitTimes object.
     """
-    def __init__(self, transit_times):
+    def __init__(self, timing_data):
         """Initializing the transit times object and model ephermeris object
-        
+        TODO: Update docstring
         Parameters
         -----------
         transit_times: TransitTimes obj
             A successfully instantiated TransitTimes object holding epochs, mid transit times, and uncertainties.
         
         Raises
         ------
             ValueError :
                 error raised if 'transit_times' is not an instance of 'TransitTimes' object.
         """
-        self.transit_times = transit_times
+        self.timing_data = timing_data
         self._validate()
 
     def _validate(self):
         """Check that transit_times is an instance of the TransitTimes object.
-        
+        TODO: Update docstring
         Raises
         ------
             ValueError :
                 error raised if 'transit_times' is not an instance of 'TransitTimes' object.
         """
-        if not isinstance(self.transit_times, TransitTimes):
-            raise ValueError("Variable 'transit_times' expected type of object 'TransitTimes'.")
+        if not isinstance(self.timing_data, TimingData):
+            raise ValueError("Variable 'timing_data' expected type of object 'TimingData'.")
         
-    def _get_transit_times_data(self):
+    def _get_timing_data(self):
         """Returns transit time data for use.
 
+        TODO: Update docstring
         Returns the epoch, mid transit time, and mid transit time error data from the TransitTimes object.
 
         Returns
         -------
             x: numpy.ndarray[int]
                 The epoch data as recieved from the TransitTimes object.
             y: numpy.ndarray[float]
                 The mid transit time data as recieved from the TransitTimes object.
             yerr: numpy.ndarray[float]
                 The mid transit time error data as recieved from the TransitTimes object.
         """
-        x = self.transit_times.epochs
-        y = self.transit_times.mid_transit_times
-        yerr = self.transit_times.mid_transit_times_uncertainties
-        return x, y, yerr
+        x = self.timing_data.epochs
+        y = self.timing_data.mid_times
+        yerr = self.timing_data.mid_time_uncertainties
+        tra_or_occ = self.timing_data.tra_or_occ
+        return x, y, yerr, tra_or_occ
     
     def _get_model_parameters(self, model_type, **kwargs):
         """Creates the model ephemeris object and returns model parameters.
         
+        TODO: Update docstring
         This method processes and fetches data from the TransitTimes object to be used in the model ephemeris. 
         It creates the appropriate subclass of BaseModelEphemeris using the ModelEphemeris factory, then runs 
         the fit_model method to return the model parameters dictionary.
 
         Parameters
         ----------
             model_type: str
@@ -307,18 +336,18 @@
 
         Raises
         ------
             ValueError:
                 If model specified is not a valid subclass of BaseModelEphemeris, which is either 'linear' or 'quadratic'.
         """
         # Step 1: Get data from transit times obj
-        x, y, yerr = self._get_transit_times_data()
+        x, y, yerr, tra_or_occ = self._get_timing_data()
         # Step 2: Create the model with the given variables & user inputs. 
         # This will return a dictionary with the model parameters as key value pairs.
-        model_ephemeris_data = ModelEphemerisFactory.create_model(model_type, x, y, yerr, **kwargs)
+        model_ephemeris_data = ModelEphemerisFactory.create_model(model_type, x, y, yerr, tra_or_occ, **kwargs)
         # Step 3: Return the data dictionary with the model parameters
         return model_ephemeris_data
     
     def _get_k_value(self, model_type):
         """Returns the number of parameters value to be used in the BIC calculation.
         
         Parameters
@@ -343,14 +372,15 @@
             return 3
         else:
             return ValueError('Only linear and quadratic models are supported at this time.')
     
     def _calc_linear_model_uncertainties(self, T0_err, P_err):
         """Calculates the uncertainties of a given linear model when compared to actual data in TransitTimes.
         
+        TODO: Update docstring
         Uses the equation σ(t pred, tra) = √(σ(T0)^2 + σ(P)^2 * E^2) where σ(T0)=conjunction time error, 
         E=epoch, and σ(P)=period error, to calculate the uncertainties between the model data and actual 
         data over epochs.
         
         Parameters
         ----------
         T0_err: numpy.ndarray[float]
@@ -359,19 +389,28 @@
             The calculated period errors from a linear model ephemeris.
         
         Returns
         -------
             A list of uncertainties associated with the model ephemeris data passed in, calculated with the 
             equation above and the TransitTimes epochs.
         """
-        return np.sqrt((T0_err**2) + ((self.transit_times.epochs**2)*(P_err**2)))
+        result = []
+        for i, t_type in enumerate(self.timing_data.tra_or_occ):
+            if t_type == 'tra':
+                # transit data
+                result.append(np.sqrt((T0_err**2) + ((self.timing_data.epochs[i]**2)*(P_err**2))))
+            elif t_type == 'occ':
+                # occultation data
+                result.append(np.sqrt(((T0_err**2) + (0.5 * (P_err**2))) + ((self.timing_data.epochs[i]**2)*(P_err**2))))
+        return np.array(result)
     
     def _calc_quadratic_model_uncertainties(self, T0_err, P_err, dPdE_err):
         """Calculates the uncertainties of a given quadratic model when compared to actual data in TransitTimes.
         
+        TODO: Update docstring
         Uses the equation σ(t pred, tra) = √(σ(T0)^2 + (σ(P)^2 * E^2) + (1/4 * σ(dP/dE)^2 * E^4)) where 
         σ(T0)=conjunction time error, E=epoch, σ(P)=period error, and σ(dP/dE)=period change by epoch error, 
         to calculate the uncertainties between the model data and actual data over epochs.
         
         Parameters
         ----------
         T0_err: numpy.ndarray[float]
@@ -382,63 +421,91 @@
             The calculated change in epoch over period error for a quadratic model ephemeris.
         
         Returns
         -------
             A list of uncertainties associated with the model ephemeris passed in, calculated with the 
             equation above and the TransitTimes epochs.
         """
-        return np.sqrt((T0_err**2) + ((self.transit_times.epochs**2)*(P_err**2)) + ((1/4)*(self.transit_times.epochs**4)*(dPdE_err**2)))
+        # Have both transits and occultations, calculate different value for each
+        result = []
+        for i, t_type in enumerate(self.timing_data.tra_or_occ):
+            if t_type == 'tra':
+                # transit data
+                result.append(np.sqrt((T0_err**2) + ((self.timing_data.epochs[i]**2)*(P_err**2)) + ((1/4)*(self.timing_data.epochs[i]**4)*(dPdE_err**2))))
+            elif t_type == 'occ':
+                # occultation data
+                result.append(np.sqrt(((T0_err**2) + (0.5 * (P_err**2))) + ((self.timing_data.epochs[i]**2)*(P_err**2)) + ((1/4)*(self.timing_data.epochs[i]**4)*(dPdE_err**2))))
+        return np.array(result)
     
-    def _calc_linear_ephemeris(self, epochs, period, conjunction_time):
+    def _calc_linear_ephemeris(self, E, P, T0):
         """Calculates the mid transit times using parameters from a linear model ephemeris.
         
+        TODO: Update docstring
         Uses the equation (T0 + PE) to calculate the mid transit times over each epoch where T0 is 
         conjunction time, P is period, and E is epoch.
 
         Parameters
         ----------
-            epochs: numpy.ndarray[int]
+            E: numpy.ndarray[int]
                 The epochs pulled from the TransitTimes object.
-            period: float
+            P: float
                 The period of the exoplanet transit as calculated by the linear ephemeris model.
-            conjunction_time: float
+            T0: float
                 The conjunction time of the exoplanet transit as calculated by the linear ephemeris model.
 
         Returns
         -------
             A numpy array of mid transit times calculated over each epoch using the equation above.
         """
-        return ((period*epochs) + conjunction_time)
+        result = []
+        for i, t_type in enumerate(self.timing_data.tra_or_occ):
+            if t_type == 'tra':
+                # transit data
+                result.append(T0 + (P*E[i]))
+            elif t_type == 'occ':
+                # occultation data
+                result.append((T0 + 0.5*P) + (P*E[i]))
+        return np.array(result)
     
-    def _calc_quadratic_ephemeris(self, epochs, period, conjunction_time, period_change_by_epoch):
+    def _calc_quadratic_ephemeris(self, E, P, T0, dPdE):
         """Calculates the mid transit times using parameters from a quadratic model ephemeris.
 
+        TODO: Update docstring
         Uses the equation (T0 + PE + 0.5 * dPdE * E^2) to calculate the mid transit times over each epoch 
         where T0 is conjunction time, P is period, E is epoch, and dPdE is period change with respect to epoch.
 
         Parameters
         ----------
-            epochs: numpy.ndarray[int]
+            E: numpy.ndarray[int]
                 The epochs pulled from the TransitTimes object.
-            period: float
+            P: float
                 The period of the exoplanet transit as calculated by the linear ephemeris model.
-            conjunction_time: float
+            T0: float
                 The conjunction time of the exoplanet transit as calculated by the linear ephemeris model.
-            period_change_by_epoch: float
+            dPdE: float
                 The period change with respect to epoch as calculated by the linear ephemeris model.
 
         Returns
         -------
             A numpy array of mid transit times calculated over each epoch using the equation above.
         """
-        return((0.5*period_change_by_epoch*(epochs**2)) + (period*epochs) + conjunction_time)
+        result = []
+        for i, t_type in enumerate(self.timing_data.tra_or_occ):
+            if t_type == 'tra':
+                # transit data
+                result.append(T0 + P*E[i] + 0.5*dPdE*E[i]*E[i])
+            elif t_type == 'occ':
+                # occultation data
+                result.append((T0 + 0.5*P) + P*E[i] + 0.5*dPdE*E[i]*E[i])
+        return np.array(result)
     
     def _calc_chi_squared(self, model_data):
         """Calculates the residual chi squared values for the model ephemeris.
 
+        TODO: Update docstring
         STEP 1: Get the observed transit times and observed transit times uncertainties from transit_times.py.
 
         STEP 2: Calculate the chi-squared value for the observed and model data, then return this value.
         
         Parameters
         ----------
             model_data : numpy.ndarray[float]
@@ -447,22 +514,33 @@
         
         Returns
         -------
             Chi-squared value : float
                 The chi-squared value calculated from the observed and model data.
         """
         # STEP 1: Get observed transit times
-        observed_data = self.transit_times.mid_transit_times
-        uncertainties = self.transit_times.mid_transit_times_uncertainties
+        observed_data = self.timing_data.mid_times
+        uncertainties = self.timing_data.mid_time_uncertainties
         # STEP 2: calculate X2 with observed data and model data
         return np.sum(((observed_data - model_data)/uncertainties)**2)
     
+    def _subtract_plotting_parameters(self, model_data, T0, P, E):
+        result = []
+        for i, t_type in enumerate(self.timing_data.tra_or_occ):
+            if t_type == 'tra':
+                # transit data
+                result.append(model_data[i] - T0 - (P*E[i]))
+            elif t_type == 'occ':
+                # occultation data
+                result.append(model_data[i] - T0 - (0.5*P) - (P*E[i]))
+        return np.array(result)
+    
     def get_model_ephemeris(self, model_type):
         """Fits the transit data to a specified model using scipy.optimize.curve_fit function.
-        
+        TODO: Update docstring
         Parameters
         ----------
             model_type: str
                 Either 'linear' or 'quadratic'. Represents the type of ephemeris to fit the data to.
 
         Returns
         ------- 
@@ -474,27 +552,27 @@
                 * 'conjunction_time_err': The uncertainties associated with conjunction_time
             
             If a quadratic model was chosen, the same variables are returned, and an additional parameter is included in the dictionary:
             
                 * 'period_change_by_epoch': The exoplanet period change over epochs, from first epoch to current epoch (in units of days),
                 * 'period_change_by_epoch_err': The uncertainties associated with period_change_by_epoch (in units of days),
         """
-        parameters = self._get_model_parameters(model_type)
-        parameters['model_type'] = model_type
+        model_ephemeris_data = self._get_model_parameters(model_type)
+        model_ephemeris_data['model_type'] = model_type
         # Once we get parameters back, we call _calc_linear_ephemeris 
         if model_type == 'linear':
             # Return dict with parameters and model data
-            parameters['model_data'] = self._calc_linear_ephemeris(self.transit_times.epochs, parameters['period'], parameters['conjunction_time'])
+            model_ephemeris_data['model_data'] = self._calc_linear_ephemeris(self.timing_data.epochs, model_ephemeris_data['period'], model_ephemeris_data['conjunction_time'])
         elif model_type == 'quadratic':
-            parameters['model_data'] = self._calc_quadratic_ephemeris(self.transit_times.epochs, parameters['period'], parameters['conjunction_time'], parameters['period_change_by_epoch'])
-        return parameters
+            model_ephemeris_data['model_data'] = self._calc_quadratic_ephemeris(self.timing_data.epochs, model_ephemeris_data['period'], model_ephemeris_data['conjunction_time'], model_ephemeris_data['period_change_by_epoch'])
+        return model_ephemeris_data
     
     def get_ephemeris_uncertainties(self, model_params):
         """Calculates the uncertainties of a specific model data when compared to the actual data. 
-        
+        TODO: Update docstring
         Uses the equation 
         
         .. math::
             \\sigma(\\text{t pred, tra}) = \\sqrt{(\\sigma(T_0)^2 + \\sigma(P)^2 * E^2)}
         
         for linear models and 
 
@@ -578,14 +656,15 @@
         quadratic_bic = self.calc_bic(quadratic_data)
         delta_bic = linear_bic - quadratic_bic
         return delta_bic
     
     def plot_model_ephemeris(self, model_data_dict, save_plot=False, save_filepath=None):
         """Returns a MatplotLib scatter plot showing predicted mid transit times from the model ephemeris over epochs.
 
+        TODO: Update docstring
         STEP 1: Plot a scatterplot of epochs (from transit_times.py) vs model_data, which is an array of floats that is a value of 'model_data_dict'.
 
         STEP 2: Save the plot if indicated by the user.
 
         Parameters
         ----------
             model_data_dict: dict
@@ -595,25 +674,25 @@
             save_filepath: Optional(str)
                 The path used to save the plot if `save_plot` is True.
         
         Returns
         ------- 
             A MatplotLib plot of epochs vs. model predicted mid-transit times.
         """
-        plt.scatter(x=self.transit_times.epochs, y=model_data_dict['model_data'])
+        plt.scatter(x=self.timing_data.epochs, y=model_data_dict['model_data'])
         plt.xlabel('Epochs')
-        plt.ylabel('Model Predicted Mid-Transit Times (units)')
-        plt.title(f'Predicted {model_data_dict["model_type"]} Model Mid Transit Times over Epochs')
+        plt.ylabel('Model Predicted Mid-Times (units)')
+        plt.title(f'Predicted {model_data_dict["model_type"].capitalize()} Model Mid Times over Epochs')
         if save_plot == True:
             plt.savefig(save_filepath)
         plt.show()
 
     def plot_timing_uncertainties(self, model_data_dict, save_plot=False, save_filepath=None):
         """Returns a MatplotLib scatter plot showing timing uncertainties over epochs.
-
+        TODO: Update docstring, hwo do we label the lines now that we have additional way of calculating y for occultations?
         STEP 1: Get the uncertianies from the model data dictionary.
 
         STEP 2: Get the model data, which is an arrary of floats representing the predicted mid-transit time data, the conjunction time and the inital period. Subtract the conjunction time and the initial period from this array.
 
         STEP 3: Plot this modified model data, showing the maximum and minimum model uncertainity at each point.
 
         STEP 4: Save the plot if indicated by the user. 
@@ -629,32 +708,35 @@
         
         Returns
         ------- 
             A MatplotLib plot of timing uncertainties.
         """
         # get uncertainties
         model_uncertainties = self.get_ephemeris_uncertainties(model_data_dict)
-        x = self.transit_times.epochs
-        # get T(E) - T0 - PE
-        y = (model_data_dict['model_data'] - model_data_dict['conjunction_time'] - (model_data_dict['period']*self.transit_times.epochs))
+        x = self.timing_data.epochs
+        # get T(E) - T0 - PE  OR  T(E) - T0 - 0.5P - PE
+        # TODO: Make this calculation a separate function
+        y = self._subtract_plotting_parameters(model_data_dict['model_data'], model_data_dict['conjunction_time'], model_data_dict['period'], self.timing_data.epochs)
         # plot the y line, then the line +- the uncertainties
         plt.plot(x, y, c='blue', label='$t(E) - T_{0} - PE$')
         plt.plot(x, y + model_uncertainties, c='red', label='$(t(E) - T_{0} - PE) + σ_{t^{pred}_{tra}}$')
         plt.plot(x, y - model_uncertainties, c='red', label='$(t(E) - T_{0} - PE) - σ_{t^{pred}_{tra}}$')
         # Add labels and show legend
         plt.xlabel('Epochs')
-        plt.ylabel('Days')
+        plt.ylabel('Seconds') # TODO: Are these days or seconds?
+        plt.title(f'Uncertainties of Predicted {model_data_dict["model_type"].capitalize()} Model Ephemeris Mid Times')
         plt.legend()
         if save_plot is True:
             plt.savefig(save_filepath)
         plt.show()
 
     def plot_oc_plot(self, save_plot=False, save_filepath=None):
         """Returns a MatplotLib scatter plot showing observed vs. calculated values of mid transit times for linear and quadratic model ephemerides over epochs.
 
+        TODO: Update docstring
         STEP 1: Call 'get_model_ephemeris' for both the linear and quadratic model types. 
 
         STEP 2: Calculate the quadratic model curve, which follows the formula :math:`y = 0.5 \\frac{dP_0}{dE} * (E - \\text{median} E)^2.`
 
         STEP 3: Plot the quadratic model curve vs. epochs from transit_times.py. Plot the error bars at each data point using the \\
         'mid_transit_times_uncertainties' from transit_times.py.
 
@@ -671,30 +753,38 @@
         -------
             A MatplotLib plot of observed vs. calculated values of mid transit times for linear and quadratic model ephemerides over epochs.
         """
         # y = T0 - PE - 0.5 dP/dE E^2
         lin_model = self.get_model_ephemeris('linear')
         quad_model = self.get_model_ephemeris('quadratic')
         # y = 0.5 dP/dE * (E - median E)^2
-        quad_model_curve = ((1/2)*quad_model['period_change_by_epoch'])*((self.transit_times.epochs - np.median(self.transit_times.epochs))**2)
-        # plot points w/ x=epoch, y=T0-PE, yerr=sigmaT0
-        plt.errorbar(self.transit_times.epochs, (self.transit_times.mid_transit_times - lin_model['conjunction_time'] - (lin_model['period']*self.transit_times.epochs)), 
-                    yerr=self.transit_times.mid_transit_times_uncertainties, marker='o', ls='', color='#0033A0',
+        # TODO: Make this calculation a separate function
+        quad_model_curve = ((1/2)*quad_model['period_change_by_epoch'])*((self.timing_data.epochs - np.median(self.timing_data.epochs))**2)
+        # plot points w/ x=epoch, y=T(E)-T0-PE, yerr=sigmaT0
+        y = self._subtract_plotting_parameters(self.timing_data.mid_times, lin_model['conjunction_time'], lin_model['period'], self.timing_data.epochs)
+        plt.errorbar(self.timing_data.epochs, y, yerr=self.timing_data.mid_time_uncertainties, 
+                    marker='o', ls='', color='#0033A0',
                     label=r'$t(E) - T_0 - P E$')
-        plt.plot(self.transit_times.epochs,
+        plt.plot(self.timing_data.epochs,
                  (quad_model_curve),
                  color='#D64309', label=r'$\frac{1}{2}(\frac{dP}{dE})E^2$')
         plt.legend()
         plt.xlabel('E - Median E')
         plt.ylabel('O-C (seconds)')
+        plt.title('Observed Minus Caluclated Plot')
         if save_plot is True:
             plt.savefig(save_filepath)
         plt.show()
 
     def plot_running_delta_bic(self, save_plot=False, save_filepath=None):
+        # TODO: Need to change this, how do we plot with occultations introduced? 
+        # Maybe we still keep all epochs as a variable?
+        # We also use mid times and uncertainties, so we will have to figure out how to account 
+        # for the occultation data in here
+
         """Returns a MatPlotlib scatterplot of epochs vs. :math:`\\Delta BIC` for each epoch.
 
         STEP 1: Get the epochs, mid transit times and mid transit times uncertainties from 'transit_times.py'.
 
         STEP 2: Create a list of the :math:`\\Delta BIC` values. For the first 3 epochs, the :math:`\\Delta BIC` value is zero. For the subsequent epochs\\
         call 'calc_delta_bic' and append the returned value to the list of delta bic values.
 
@@ -710,68 +800,82 @@
                 The path used to save the plot if `save_plot` is True.
                 
         Returns
         -------
             A MatplotLib scatter plot of epochs vs. :math:`\\Delta BIC` for each epoch.
         """
         delta_bics = []
-        all_epochs = self.transit_times.epochs
-        all_mid_transit_times = self.transit_times.mid_transit_times
-        all_uncertainties = self.transit_times.mid_transit_times_uncertainties
+        all_epochs = self.timing_data.epochs
+        all_mid_times = self.timing_data.mid_times
+        all_uncertainties = self.timing_data.mid_time_uncertainties
+        all_tra_or_occ = self.timing_data.tra_or_occ
         # for each epoch (starting at 3?), calculate the delta bic, plot delta bics over epoch
         for i in range(0, len(all_epochs)):
             if i < 2:
                 delta_bics.append(int(0))
             else:
-                self.transit_times.mid_transit_times = all_mid_transit_times[:i+1]
-                self.transit_times.mid_transit_times_uncertainties = all_uncertainties[:i+1]
-                self.transit_times.epochs = all_epochs[:i+1]
+                self.timing_data.epochs = all_epochs[:i+1]
+                self.timing_data.mid_times = all_mid_times[:i+1]
+                self.timing_data.mid_time_uncertainties = all_uncertainties[:i+1]
+                self.timing_data.tra_or_occ = all_tra_or_occ[:i+1]
                 delta_bic = self.calc_delta_bic()
                 delta_bics.append(delta_bic)
-        plt.scatter(x=self.transit_times.epochs, y=delta_bics)
+        plt.scatter(x=self.timing_data.epochs, y=delta_bics)
         plt.grid(True)
-        plt.plot(self.transit_times.epochs, delta_bics)
+        plt.plot(self.timing_data.epochs, delta_bics)
+        plt.xlabel('Epoch')
+        plt.ylabel('$\Delta$BIC')
+        plt.title("Value of $\Delta$BIC as Observational Epochs Increase")
         if save_plot is True:
             plt.savefig(save_filepath)
         plt.show()
 
 if __name__ == '__main__':
     # STEP 1: Upload datra from file
-    filepath = "../../malia_examples/WASP12b_transit_ephemeris.csv"
-    data = np.genfromtxt(filepath, delimiter=',', names=True)
+    filepath = "../../wasp12b_tra_occ.csv"
+    # filepath = "../../malia_examples/WASP12b_transit_ephemeris.csv"
+    data = np.genfromtxt(filepath, delimiter=',', names=True, dtype=None, encoding=None)
     # STEP 2: Break data up into epochs, mid transit times, and error
     # STEP 2.5 (Optional): Make sure the epochs are integers and not floats
+    tra_or_occs = data["tra_or_occ"]
     epochs = data["epoch"].astype('int')
     mid_transit_times = data["transit_time"]
     mid_transit_times_err = data["sigma_transit_time"]
     # STEP 3: Create new transit times object with above data
-    # transit_times_obj1 = TransitTimes('jd', epochs, mid_transit_times, mid_transit_times_err, object_ra=97.64, object_dec=29.67, observatory_lat=43.60, observatory_lon=-116.21)
-    # print(vars(transit_times_obj1))
-    transit_times_obj1 = TransitTimes('jd', epochs, mid_transit_times, mid_transit_times_err, time_scale='tdb')
-
-
-    # print(f"EPOCHS: {transit_times_obj1.epochs}\n")
-    # print(f"MID TRANSIT TIMES: {transit_times_obj1.mid_transit_times}\n")
-    # # STEP 4: Create new ephemeris object with transit times object
-    # ephemeris_obj1 = Ephemeris(transit_times_obj1)
-    # # STEP 5: Get model ephemeris data
-    # linear_model_data = ephemeris_obj1.get_model_ephemeris('linear')
-    # quad_model_data = ephemeris_obj1.get_model_ephemeris('quadratic')
+    # times_obj1 = TimingData('jd', epochs, mid_transit_times, mid_transit_times_err, tra_or_occ=tra_or_occs, object_ra=97.64, object_dec=29.67, observatory_lat=43.60, observatory_lon=-116.21)
+    # times_obj1 = TimingData('jd', epochs, mid_transit_times, mid_transit_times_err, time_scale='tdb')
+    times_obj1 = TimingData('jd', epochs, mid_transit_times, mid_transit_times_err, time_scale='tdb', tra_or_occ=tra_or_occs)
+    # STEP 4: Create new ephemeris object with transit times object
+    ephemeris_obj1 = Ephemeris(times_obj1)
+    # STEP 5: Get model ephemeris data & BIC values
+    # # LINEAR MODEL
+    linear_model_data = ephemeris_obj1.get_model_ephemeris('linear')
     # print(linear_model_data)
+    linear_model_uncertainties = ephemeris_obj1.get_ephemeris_uncertainties(linear_model_data)
+    # print(linear_model_uncertainties)
+    lin_bic = ephemeris_obj1.calc_bic(linear_model_data)
+    # print(lin_bic)
+    # # QUADRATIC MODEL
+    quad_model_data = ephemeris_obj1.get_model_ephemeris('quadratic')
     # print(quad_model_data)
-    # # ephemeris_obj1.plot_model_ephemeris(linear_model_data)
-    # # ephemeris_obj1.plot_model_ephemeris(quad_model_data)
-    # ephemeris_obj1.plot_oc_plot()
-    # model_uncertainties = ephemeris_obj1.get_ephemeris_uncertainties(model_data)
-    # print(model_uncertainties)
-    # # STEP 6: Show a plot of the model ephemeris data
-    # # ephemeris_obj1.plot_model_ephemeris(model_data, save_plot=False)
-    # # # STEP 7: Uncertainties plot
-    # # ephemeris_obj1.plot_timing_uncertainties(model_data, save_plot=False)
-    # # bic = ephemeris_obj1.calc_bic(model_data)
-    # # print(bic)
-
-    # # print(ephemeris_obj1.calc_delta_bic())
-    # print(ephemeris_obj1.plot_running_delta_bic(save_plot=False))
-    # # ephemeris_obj1.plot_running_delta_bic(save_plot=False)
+    quad_model_uncertainties = ephemeris_obj1.get_ephemeris_uncertainties(quad_model_data)
+    # print(quad_model_uncertainties)
+    quad_bic = ephemeris_obj1.calc_bic(quad_model_data)
+    # print(quad_bic)
+    # STEP 5.5: Get the delta BIC value for both models
+    delta_bic = ephemeris_obj1.calc_delta_bic()
+    # print(delta_bic)
+
+    # STEP 6: Show a plot of the model ephemeris data
+    # ephemeris_obj1.plot_model_ephemeris(linear_model_data, save_plot=False)
+    # ephemeris_obj1.plot_model_ephemeris(quad_model_data, save_plot=False)
+
+    # STEP 7: Uncertainties plot
+    # ephemeris_obj1.plot_timing_uncertainties(linear_model_data, save_plot=False)
+    # ephemeris_obj1.plot_timing_uncertainties(quad_model_data, save_plot=False)
+    
+    # STEP 8: O-C Plot
+    # ephemeris_obj1.plot_oc_plot(save_plot=False)
 
-    # # ephemeris_obj1.plot_oc_plot(False)
+    # STEP 9: Running delta BIC plot
+    ephemeris_obj1.plot_running_delta_bic(save_plot=False)
+
```

### Comparing `susie-1.0.9/src/susie/transit_times.py` & `susie-1.1.0/src/susie/timing_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,153 +1,166 @@
 import numpy as np
 from astropy import time
 from astropy import coordinates as coord
 from astropy import units as u
 import logging
 
-# TESTING
+class TimingData():
+    """Represents timing mid point data over observations. Holds data to be accessed by Ephemeris class.
 
-# class TransitTimes():
-#     def __init__(self):
-#         # pass in all the same stuff for transit times
-#         pass
-
-# class OccultationTimes():
-#     def __init__(self):
-#         # pass in all the same stuff for occultation times
-#         pass
-
-class TransitTimes():
-    """Represents transit midpoint data over time. Holds data to be accessed by Ephemeris class.
+    The TimingData object processes, formats, and holds user data to be passed to the ephemeris object.
     
-    The transit_times object is a class which formats user data to be passed to the ephemeris.py object. \
-        This object creates and/or formats the array of uncertainties in mid_transit_times. This object \
-            will also correct user data to use the Barycentric Julian Date as the timing system and Barycentric \
-                Dynamical time as the time scale.
-
-    STEP 1: Make an array of 1's to be the uncertainities in the same shape as epochs and mid_transit_times.
+    Timing conversions are applied to ensure that all data is processed correctly and users are aware of 
+    timing formats and scales, which can give rise to false calculations in our metrics. If data is not specified
+    to be in Barycentric Julian Date format with the TDB time scale, timing data will be corrected for barycentric
+    light travel time using the Astropy Time utilities. 
+    
+    If mid time uncertainties are not provided, we will generate placeholder values of 1.
 
-    STEP 2: Check that the time system and scale are correct, and if not correct them to be JD and TBD.
+    Our implementations rely on Numpy functions. This object implements checks to ensure that data are stored in 
+    Numpy arrays and are of correct data types. The appropriate Type or Value Error is raised if there are any issues.
+    
+    If timing data contains both transit mid times and occultation mid times, users can pass in an array of 'tra' 
+    and 'occ' strings that correspond to the epochs, mid time, and uncertainty timing data. If passed in, timing data
+    will be separated according to the order of the tra_or_occ array and stored in their corresponding objects.
 
-    STEP 3: Check that the array's are formatted properly. The appropriate Type or Value Error is raised if there are any issues.
- 
     Parameters
     ------------
         time_format: str 
-            An abbreviation of the data's timing system. Abbreviations for systems can be found on [Astropy's Time documentation](https://docs.astropy.org/en/stable/time/#id3).
-        epochs: numpy.ndarray(int)
-            List of reference points for transit observations represented in the transit times data.
-        mid_transit_times: numpy.ndarray(float)
-            List of observed transit midpoints in days corresponding with epochs.
-        mid_transit_times_uncertainties: Optional(numpy.ndarray[float])
-            List of uncertainties in days corresponding with transit midpoints. If given None, will be replaced with array of 1's with same shape as `mid_transit_times`.
+            An abbreviation of the data's time system. Abbreviations for systems can be found on [Astropy's Time documentation](https://docs.astropy.org/en/stable/time/#id3).
+        epochs: numpy.ndarray[int]
+            List of orbit number reference points for timing observations
+        mid_times: numpy.ndarray[float]
+            List of observed timing mid points corresponding with epochs, in timing units given by time_format
+        mid_time_uncertainties: Optional(numpy.ndarray[float])
+            List of uncertainties corresponding to timing mid points, in timing units given by time_format. If given None, will be replaced with array of 1's with same shape as `mid_times`.
         time_scale: Optional(str)
-            An abbreviation of the data's timing scale. Abbreviations for scales can be found on [Astropy's Time documentation](https://docs.astropy.org/en/stable/time/#id6).
+            An abbreviation of the data's time scale. Abbreviations for scales can be found on [Astropy's Time documentation](https://docs.astropy.org/en/stable/time/#id6).
         object_ra: Optional(float)
-            The right ascension in degrees of observed object represented by data.
+            The right ascension of observed object represented by data, in degrees
         object_dec: Optional(float)
-            The declination in degrees of observed object represented by data.
+            The declination of observed object represented by data, in degrees
         observatory_lon: Optional(float)
-            The longitude in degrees of observatory data was collected from.
+            The longitude of observatory data was collected from, in degrees
         observatory_lat: Optional(float) 
-            The latitude in degrees of observatory data was collected from.
+            The latitude of observatory data was collected from, in degrees
+    
     Raises
     ------
         Error raised if  
-            * parameters are not NumPy Arrays 
-            * parameters are not the same shape of array 
+            * parameters are not NumPy Arrays
+            * timing data arrays are not the same shape
             * the values of epochs are not all ints
-            * the values of mid_transit_times and unertainites are not all floats
-            * values of uncertainities are not all positive.
+            * the values of mid_times and uncertainites are not all floats
+            * values of uncertainities are not all positive
+            * values of transit or occultation array or not all 'tra' or 'occ'
 
     Side Effects
     -------------
-        Variables epochs and mid_transit_times are shifted to start at zero by subtracting the minimum number from each value.
+        Variables epochs and mid_times are shifted to start at zero by subtracting the minimum number from each value
     """
-    # def __init__(self, time_format, epochs, mid_transit_times, mid_transit_times_uncertainties=None, tra_or_occ=None, time_scale=None, object_ra=None, object_dec=None, observatory_lon=None, observatory_lat=None):
-    def __init__(self, time_format, epochs, mid_transit_times, mid_transit_times_uncertainties=None, time_scale=None, object_ra=None, object_dec=None, observatory_lon=None, observatory_lat=None):
+    def __init__(self, time_format, epochs, mid_times, mid_time_uncertainties=None, tra_or_occ=None, time_scale=None, object_ra=None, object_dec=None, observatory_lon=None, observatory_lat=None):
+        # In ephemeris, we would probably check if we had both transits and occultations
+        # If so, we would need to account for that (maybe just in the fitting implementation? anywhere else?)
+        # If not, then we just assign our data to the transit times data and let it run!
+        # Although, need to look into this still. Might just have this implemented in model fits and plotting?
+        self.transits = None
+        self.occultations = None
         self.epochs = epochs
-        self.mid_transit_times = mid_transit_times
-        if mid_transit_times_uncertainties is None:
-            # Make an array of 1s in the same shape of epochs and mid_transit_times
-            mid_transit_times_uncertainties =  np.ones_like(self.epochs, dtype=float)
-        self.mid_transit_times_uncertainties = mid_transit_times_uncertainties
+        self.mid_times = mid_times
+        self.tra_or_occ = tra_or_occ
+        if mid_time_uncertainties is None:
+            # If no uncertainties provided, make an array of 1s in the same shape of epochs
+            mid_time_uncertainties =  np.ones_like(self.epochs, dtype=float)
+        self.mid_time_uncertainties = mid_time_uncertainties
         # Check that timing system and scale are JD and TDB
         if time_format != 'jd' or time_scale != 'tdb':
-            # TODO: Make sure they know default scale is UTC
             # If not correct time format and scale, create time objects and run corrections
             logging.warning(f"Recieved time format {time_format} and time scale {time_scale}. " 
-                            "Correcting all times to BJD timing system with TDB time scale. If this is incorrect, please set the time format and time scale for TransitTime object.")
-            self.mid_transit_times = None
-            self.mid_transit_times_uncertainties = None
-            mid_transit_times_obj = time.Time(mid_transit_times, format=time_format, scale=time_scale)
-            mid_transit_times_uncertainties_obj = time.Time(mid_transit_times_uncertainties, format=time_format, scale=time_scale)
-            self._validate_times(mid_transit_times_obj, mid_transit_times_uncertainties_obj, (object_ra, object_dec), (observatory_lon, observatory_lat))
+                            "Correcting all times to BJD timing system with TDB time scale. \
+                             If no time scale is given, default is automatically assigned to UTC. \
+                             If this is incorrect, please set the time format and time scale for TransitTime object.")
+            # Set timing data to None for now
+            self.mid_times = None
+            self.mid_time_uncertainties = None
+            mid_times_obj = time.Time(mid_times, format=time_format, scale=time_scale)
+            mid_time_uncertainties_obj = time.Time(mid_time_uncertainties, format=time_format, scale=time_scale)
+            self._validate_times(mid_times_obj, mid_time_uncertainties_obj, (object_ra, object_dec), (observatory_lon, observatory_lat))
         # Call validation function
         self._validate()
-        # Once everything is validated and corrected, we can separate into transits and occultations if we are given the tra_or_occ data
-        # if tra_or_occ is not None:
-        #     for epoch, mtt, mtt_err in zip(self.epochs, self.mid_transit_times, self.mid_transit_times_uncertainties):
-        #         foiwehf
 
     def _calc_barycentric_time(self, time_obj, obj_location, obs_location):
         """Function to correct non-barycentric time formats to Barycentric Julian Date in TDB time scale.
 
-        STEP 1: Checks if given placeholder values of 1. If given placeholder values, no correction needed and array of 1's returned.
-
-        STEP 2: If given actual values, correct the values to be Barycentric Julian Date in TDB time scale. Return corrected values.
+        This function will run under the given circumstances:
+            * If the timing format provided is not JD (time_format == 'jd')
+            * If the timing scale is not provided
+            * If the timing scale provided is not TDB (time_sclae == 'tdb')
+
+        Calculates the light travel time for the given Astropy timing object and adds the light 
+        travel time to each original value in the given timing data. If the given Astropy timing object time data 
+        contains a list of 1s, which means this is placeholder timing uncertainty data, no timing correction will 
+        be applied as this is not real data. If the timing correction proceeds, the `light_travel_time` function 
+        from Astropy will be applied and added to the original timing data. Timing data corrected for Barycentric 
+        light travel time will be returned.
 
         Parameters
         ----------
             time_obj : numpy.ndarray[float]
-                List to be corrected to the Barycentric Julian Date in TDB time scale.
-            obj_location : numpy.ndarray[float]
-                List of the RA and DEC in degrees of the object being observed.
-            obs_location : Optional(numpy.ndarray[float])                           NOTE considered optional only if keyword argument - check for these
-                List of the longitude and latitude in degrees of the site of observation. If None given, uses gravitational center of Earth at North Pole.
+               List of timing data to be corrected to the Barycentric Julian Date time format in the TDB time scale.
+            obj_location : Astropy.coordinates.SkyCoord obj
+                The RA and DEC in degrees of the object being observed, stored as an Astropy coordinates.SkyCoord object.
+            obs_location : Astropy.coordinates.EarthLocation obj
+                The longitude and latitude in degrees of the site of observation, stored as an Astropy coordinates.EarthLocation object. 
+                If None given, uses gravitational center of Earth at North Pole.
        
         Returns
         -------
             time_obj.value : numpy.ndarray[float]
-                Returned only if no correction needed. Placeholder array of 1s with same shape as `mid_transit_times`.
+                Returned only if these are placeholder uncertainties and no correction is needed.
             corrected_time_vals : numpy.ndarray[float]
-                List now corrected to Barycentric Julian Date in TDB time scale.
+                List of mid times corrected to Barycentric Julian Date time format with TDB time scale.
         """
         # If given uncertainties, check they are actual values and not placeholders vals of 1
         # If they are placeholder vals, no correction needed, just return array of 1s
         if np.all(time_obj.value == 1):
             return time_obj.value
         time_obj.location = obs_location
         ltt_bary = time_obj.light_travel_time(obj_location)
         corrected_time_vals = (time_obj.tdb+ltt_bary).value
         return corrected_time_vals
     
-    def _validate_times(self, mid_transit_times_obj, mid_transit_times_uncertainties_obj, obj_coords, obs_coords):
-        """Checks that object and observatory coordinates are in correct format for correction function, passes the observed transit midpoints and the uncertainties in observed transit midpoints to the correction function. 
-    
-        STEP 1: Checks if there are object coordinates (right ascension and declination). Raises a ValueError if not.
-
-        STEP 2: Checks if there are observatory coordinates (latitude and longitude). Raises a warning and uses the gravitational center of Earth at the North Pole if not.
+    def _validate_times(self, mid_times_obj, mid_time_uncertainties_obj, obj_coords, obs_coords):
+        """Validates object and observatory information and populates Astropy objects for barycentric light travel time correction.
 
-        STEP 3: Performs corrections to 'mid_transit_times_obj' and 'mid_transit_times_uncertainties_obj' by calling '_calc_barycentric_time'
+        Checks that object coordinates (right ascension and declination) and are of correct types. If correct object 
+        coordinates are given, will create an Astropy SkyCoord object. Checks that observatory coordinates (longitude 
+        and latitude) are given and of correct types. If given, will populate an Astropy EarthLocation object. If not
+        given, will populate Astropy EarthLocation with gravitational center of Earth at North Pole. Passes the validated
+        SkyCoord, EarthLocation, and Time objects to the `_calc_barycentric_time` correction function to convert times
+        to BJD TDB timing format and scale.
 
         Parameters
         ----------
-            mid_transit_times_obj : (astropy.time.Time[array, string, string])         
-                List of transit midpoints, time_format, and time_scale 
-            mid_trnasit_times_uncertainties_obj : Optional(astropy.time.Time[array, string, string])      NOTE also not really uncertainties in strings - maybe reformat the description
-                List of uncertainties corresponding with transit midpoints, time_format, and time_scale. If given None initailly, have been replaced with array of 1's with same shape as `mid_transit_times`.
-            obj_coords : numpy.ndarray[float]
-                List of the RA and DEC in degrees of the object being observed.
-            obs_coords : Optional(numpy.ndarray[float])             
-                List of the longitude and latitude in degrees of the site of observation. If None given, use gravitational center of Earth at North Pole.
+            mid_times_obj : (astropy.time.Time[numpy.ndarray[floats], string, string])
+                An Astropy Time object containing the mid time data, time format, and time scale
+            mid_time_uncertainties_obj : Optional(astropy.time.Time[numpy.ndarray[floats], string, string])
+                An Astropy Time object containing timing uncertainty data, time format, and time scale. If no uncertainties intially given, data has been replaced with array of 1's with same shape as `mid_times`.
+            obj_coords : object_ra: float, object_dec: float)
+                Tuple of the right ascension and declination in degrees of the object being observed.
+            obs_coords : Optional((observatory_lon: float, observatory_lat: float))    
+                Tuple of the longitude and latitude in degrees of the site of observation.
 
         Raises
             ValueError :
                 Error if None recieved for object_ra or object_dec.
+            Warning:
+                Warning if no observatory coordinates are given.
+                Warning notifying user that barycentric light travel time correction is taking place with the given
+                information.
         ------
 
         """
         # check if there are objects coords, raise error if not
         if all(elem is None for elem in obj_coords):
             raise ValueError("Recieved None for object right ascension and/or declination. " 
                              "Please enter ICRS coordinate values in degrees for object_ra and object_dec for TransitTime object.")
@@ -158,69 +171,174 @@
             obs_location = coord.EarthLocation.from_geocentric(0., 0., 0., unit=u.m)
         else:
             obs_location = coord.EarthLocation.from_geodetic(obs_coords[0], obs_coords[1])
         obj_location = coord.SkyCoord(ra=obj_coords[0], dec=obj_coords[1], unit='deg', frame='icrs')
         logging.warning(f"Using ICRS coordinates in degrees of RA and Dec {round(obj_location.ra.value, 2), round(obj_location.dec.value, 2)} for time correction. "
                         f"Using geodetic Earth coordinates in degrees of longitude and latitude {round(obs_location.lon.value, 2), round(obs_location.lat.value, 2)} for time correction.")
         # Perform correction, will return array of corrected times
-        self.mid_transit_times_uncertainties = self._calc_barycentric_time(mid_transit_times_uncertainties_obj, obj_location, obs_location)
-        self.mid_transit_times = self._calc_barycentric_time(mid_transit_times_obj, obj_location, obs_location)
+        self.mid_time_uncertainties = self._calc_barycentric_time(mid_time_uncertainties_obj, obj_location, obs_location)
+        self.mid_times = self._calc_barycentric_time(mid_times_obj, obj_location, obs_location)
 
+    def _validate_tra_or_occ(self):
+        # Check that object is of type array
+        if not isinstance(self.tra_or_occ, np.ndarray):
+            raise TypeError("The variable 'tra_or_occ' expected a NumPy array (np.ndarray) but received a different data type")
+        # Check if any values are not valid in tra_or_occ array
+        if any(val not in ['tra', 'occ'] for val in self.tra_or_occ):
+            raise ValueError("tra_or_occ array cannot contain string values other than 'tra' or 'occ'")
+        # Check the shape 
+        if self.tra_or_occ.shape != self.mid_time_uncertainties.shape != self.mid_times.shape != self.epochs.shape:
+            raise ValueError("Shapes of 'tra_or_occ', 'mid_time_uncertainties', 'mid_times', and 'epochs' arrays do not match.")
+        # strings
+        if not all(isinstance(value, str) for value in self.tra_or_occ):
+            raise TypeError("All values in 'tra_or_occ' must be of type string.")
+        # null values
+        if np.issubdtype(self.tra_or_occ.dtype, np.number) and np.any(np.isnan(self.tra_or_occ)):
+            raise ValueError("The 'tra_or_occ' array contains NaN (Not-a-Number) values.")
+   
     def _validate(self):
         """Checks that all object attributes are of correct types and within value constraints.
-        STEP 1: Check all object attributes are of type array.
-
-        STEP 2: Check all object attributes are of same shape.
 
-        STEP 3: Check all object attributes contain correct value type.
-
-        STEP 4: Check all object attributes contain no null values.
-
-        STEP 5: Check 'mid_transit_times_uncertainties' contains non-negative and non-zero values.
+        Validates the types of the main data attributes: epochs, mid_times, and mid_time_uncertainties. 
+        The following checks are in place:
+            * Contained in numpy arrays
+            * Epochs are integers
+            * Mid times and uncertainties are floats
+            * No null or nan values are in the data
+            * Epochs, mid times, and uncertainties all contain the same amount of data points
+            * All uncertainties are positive
+        If the epochs and mid times do not start at zero, the arrays will be shifted to start at zero by 
+        subtracting the minimum value of the array from each data point in the array.
 
         Raises
         ------
             TypeError :
-                Error if 'epochs', 'mid_traisit_times', or 'mid_transit_times_uncertainties' are not NumPy arrays.
+                Error if 'epochs', 'mid_traisit_times', or 'mid_time_uncertainties' are not NumPy arrays.
             ValueError :
-                Error if shapes of 'epochs', 'mid_transit_times', and 'mid_transit_times_uncertainties' arrays do not match.
+                Error if shapes of 'epochs', 'mid_times', and 'mid_time_uncertainties' arrays do not match.
             TypeError :
-                Error if values in 'epochs' are not ints, values in 'mid_transit_times' or 'mid_transit_times_uncertainties" are not floats. 
+                Error if values in 'epochs' are not ints, values in 'mid_times' or 'mid_time_uncertainties" are not floats. 
             ValueError :
-                Error if 'epochs', 'mid_transit_times', or 'mid_transit_times_uncertainties' contain a NaN (Not-a-Number) value.
+                Error if 'epochs', 'mid_times', or 'mid_time_uncertainties' contain a NaN (Not-a-Number) value.
             ValueError :
-                Error if 'mid_transit_times_uncertainties' contains a negative or zero value.
+                Error if 'mid_time_uncertainties' contains a negative or zero value.
         """
         # Check that all are of type array
         if not isinstance(self.epochs, np.ndarray):
             raise TypeError("The variable 'epochs' expected a NumPy array (np.ndarray) but received a different data type")
-        if not isinstance(self.mid_transit_times, np.ndarray):
-            raise TypeError("The variable 'mid_transit_times' expected a NumPy array (np.ndarray) but received a different data type")
-        if not isinstance(self.mid_transit_times_uncertainties, np.ndarray):
-            raise TypeError("The variable 'mid_transit_times_uncertainties' expected a NumPy array (np.ndarray) but received a different data type")
+        if not isinstance(self.mid_times, np.ndarray):
+            raise TypeError("The variable 'mid_times' expected a NumPy array (np.ndarray) but received a different data type")
+        if not isinstance(self.mid_time_uncertainties, np.ndarray):
+            raise TypeError("The variable 'mid_time_uncertainties' expected a NumPy array (np.ndarray) but received a different data type")
         # Check that all are same shape
-        if self.epochs.shape != self.mid_transit_times.shape != self.mid_transit_times_uncertainties.shape:
-            raise ValueError("Shapes of 'epochs', 'mid_transit_times', and 'mid_transit_times_uncertainties' arrays do not match.")
+        if self.epochs.shape != self.mid_times.shape != self.mid_time_uncertainties.shape:
+            raise ValueError("Shapes of 'epochs', 'mid_times', and 'mid_time_uncertainties' arrays do not match.")
         # Check that all values in arrays are correct
         # if not all(isinstance(value, (int, np.int64)) for value in self.epochs) or not all(isinstance(value, (int, np.int32)) for value in self.epochs):
         if not all(isinstance(value, (int, np.int64, np.int32)) for value in self.epochs):
             raise TypeError("All values in 'epochs' must be of type int, numpy.int64, or numpy.int32.")
-        if not all(isinstance(value, float) for value in self.mid_transit_times):
-            raise TypeError("All values in 'mid_transit_times' must be of type float.")
-        if not all(isinstance(value, float) for value in self.mid_transit_times_uncertainties):
-            raise TypeError("All values in 'mid_transit_times_uncertainties' must be of type float.")
+        if not all(isinstance(value, float) for value in self.mid_times):
+            raise TypeError("All values in 'mid_times' must be of type float.")
+        if not all(isinstance(value, float) for value in self.mid_time_uncertainties):
+            raise TypeError("All values in 'mid_time_uncertainties' must be of type float.")
         # Check that there are no null values
         if np.any(np.isnan(self.epochs)):
             raise ValueError("The 'epochs' array contains NaN (Not-a-Number) values.")
-        if np.any(np.isnan(self.mid_transit_times)):
-            raise ValueError("The 'mid_transit_times' array contains NaN (Not-a-Number) values.")
-        if np.any(np.isnan(self.mid_transit_times_uncertainties)):
-            raise ValueError("The 'mid_transit_times_uncertainties' array contains NaN (Not-a-Number) values.")
-        # Check that mid_transit_times_uncertainties are positive and non-zero (greater than zero)
-        if not np.all(self.mid_transit_times_uncertainties > 0):
-            raise ValueError("The 'mid_transit_times_uncertainties' array must contain non-negative and non-zero values.")
+        if np.any(np.isnan(self.mid_times)):
+            raise ValueError("The 'mid_times' array contains NaN (Not-a-Number) values.")
+        if np.any(np.isnan(self.mid_time_uncertainties)):
+            raise ValueError("The 'mid_time_uncertainties' array contains NaN (Not-a-Number) values.")
+        # Check that mid_time_uncertainties are positive and non-zero (greater than zero)
+        if not np.all(self.mid_time_uncertainties > 0):
+            raise ValueError("The 'mid_time_uncertainties' array must contain non-negative and non-zero values.")
         if self.epochs[0] != 0:
             # Shift epochs and mid transit times
             self.epochs -= np.min(self.epochs)
             # TODO import warning that we are minimizing their epochs and transit times
-        if self.mid_transit_times[0] != 0:
-            self.mid_transit_times -= np.min(self.mid_transit_times)
+        if self.mid_times[0] != 0:
+            self.mid_times -= np.min(self.mid_times)
+        if self.tra_or_occ is None:
+            # Create list of just 'tra'
+            self.tra_or_occ = np.array(['tra' for element in self.epochs])
+        if self.tra_or_occ is not None:
+            self._validate_tra_or_occ()
+
+
+"""———————————————————— OLD CODE, MAY NOT BE NEEDED ————————————————————"""
+
+
+# class TransitTimes():
+#     """Represents the pre-processed transit mid point timing data over observations.
+    
+#     Parameters
+#     ------------
+#         epochs: numpy.ndarray[int]
+#             List of orbit number reference points for transit timing observations
+#         mid_times: numpy.ndarray[float]
+#             List of observed transit timing mid points corresponding with epochs
+#         mid_time_uncertainties: numpy.ndarray[float]
+#             List of uncertainties corresponding to transit mid-times
+#     """
+#     def __init__(self, epochs, mid_times, mid_time_uncertainties):
+#         self.epochs = epochs
+#         self.mid_times = mid_times
+#         self.mid_time_uncertainties = mid_time_uncertainties
+
+
+# class OccultationTimes():
+#     """Represents the pre-processed occultation mid point timing data over observations.
+    
+#     Parameters
+#     ------------
+#         epochs: numpy.ndarray[int]
+#             List of orbit number reference points for occultation timing observations
+#         mid_times: numpy.ndarray[float]
+#             List of observed occultation timing mid points corresponding with epochs
+#         mid_time_uncertainties: numpy.ndarray[float]
+#             List of uncertainties corresponding to occultation mid-times
+#     """
+#     def __init__(self, epochs, mid_times, mid_time_uncertainties):
+#         self.epochs = epochs
+#         self.mid_times = mid_times
+#         self.mid_time_uncertainties = mid_time_uncertainties
+
+# def _validate_tra_or_occ_data(self,t_epochs,t_mid_times,t_mid_time_uncertainties,o_epochs, o_mid_times, o_mid_time_uncertainties):
+    #     # Check that all are of type array
+    #     if not isinstance(t_mid_times, np.ndarray):
+    #         raise TypeError("The variable 't_mid_times' expected a NumPy array (np.ndarray) but received a different data type")
+    #     if not isinstance(t_mid_time_uncertainties, np.ndarray):
+    #         raise TypeError("The variable 't_mid_time_uncertainties' expected a NumPy array (np.ndarray) but received a different data type")
+    #     if not isinstance(o_epochs, np.ndarray):
+    #         raise TypeError("The variable 'o_epochs' expected a NumPy array (np.ndarray) but received a different data type")
+    #     if not isinstance(o_mid_times, np.ndarray):
+    #         raise TypeError("The variable 'o_mid_times' expected a NumPy array (np.ndarray) but received a different data type")
+    #     if not isinstance(o_mid_time_uncertainties, np.ndarray):
+    #         raise TypeError("The variable 'o_mid_time_uncertainties' expected a NumPy array (np.ndarray) but received a different data type")
+    #     # Check that all are same shape
+    #     if t_epochs.shape != t_mid_times.shape != t_mid_time_uncertainties.shape:
+    #         raise ValueError("Shapes of 't_epochs', 't_mid_times', and 't_mid_time_uncertainties' arrays do not match.")
+    #     if o_epochs.shape != o_mid_times.shape != o_mid_time_uncertainties.shape:
+    #         raise ValueError("Shapes of 'o_epochs', 'o_mid_times', and 'o_mid_time_uncertainties' arrays do not match.")
+
+# # Once everything is validated and corrected, we can separate into transits and occultations if we are given the tra_or_occ data
+        # if self.tra_or_occ is None:
+        #     # All data are transit data
+        #     self.transits = TransitTimes(self.epochs, self.mid_times, self.mid_time_uncertainties)
+        # else:
+        #     self._validate_tra_or_occ(tra_or_occ)
+        #     tra_or_occ = np.char.strip(tra_or_occ) # Strip any whitespace
+        #     # Separate epochs, mid times, and uncertainties into their respective lists
+        #     # t_epochs = []
+        #     # for i in range(len(tra_or_occ)):
+        #     #     if tra_or_occ[i] == 'tra':
+        #     #         t_epochs.append(self.epochs[i])
+
+        #     t_epochs = np.array([self.epochs[i] for i in range(len(tra_or_occ)) if tra_or_occ[i] == 'tra'])
+        #     t_mid_times = np.array([self.mid_times[i] for i in range(len(tra_or_occ)) if tra_or_occ[i] == 'tra'])
+        #     t_mid_time_uncertainties = np.array([self.mid_time_uncertainties[i] for i in range(len(tra_or_occ)) if tra_or_occ[i] == 'tra'])
+        #     o_epochs = np.array([self.epochs[i] for i in range(len(tra_or_occ)) if tra_or_occ[i] == 'occ'])
+        #     o_mid_times = np.array([self.mid_times[i] for i in range(len(tra_or_occ)) if tra_or_occ[i] == 'occ'])
+        #     o_mid_time_uncertainties = np.array([self.mid_time_uncertainties[i] for i in range(len(tra_or_occ)) if tra_or_occ[i] == 'occ'])
+        #     self._validate_tra_or_occ_data(self,t_epochs,t_mid_times,t_mid_time_uncertainties,o_epochs, o_mid_times, o_mid_time_uncertainties)
+        #     # Create transit and occultation objects
+        #     self.transits = TransitTimes(t_epochs, t_mid_times, t_mid_time_uncertainties)
+        #     self.occultations = OccultationTimes(o_epochs, o_mid_times, o_mid_time_uncertainties)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `susie-1.0.9/src/susie.egg-info/PKG-INFO` & `susie-1.1.0/src/susie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: susie
-Version: 1.0.9
+Version: 1.1.0
 Summary: Susie allows users to input exoplanet transit data and return information detailing possible tidal decay.
 Author: Malia Barker, Holly VanLooy, Adrienne Kirk
 Author-email: maliabarker@icloud.com, hollyvanlooy@u.boisestate.edu, adriennekirk@u.boisestate.edu
 Project-URL: Bug Tracker, https://github.com/BoiseStatePlanetary/susie/issues
 Project-URL: Repository, https://github.com/BoiseStatePlanetary/susie/
 Project-URL: Documentation, https://susie.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
-Requires-Dist: scipy
+Requires-Dist: lmfit
 Requires-Dist: matplotlib
 Requires-Dist: astropy
 
 # The Susie Python Package
 A package for exoplanet transit decay calculations and visualizations.
 
 https://susie.readthedocs.io/en/latest/
```

### Comparing `susie-1.0.9/tests/test_transit_times.py` & `susie-1.1.0/tests/test_transit_times.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import sys
 sys.path.append(".")
-from src.susie.transit_times import TransitTimes
+from src.susie.timing_data import TimingData
 import unittest
 import numpy as np
 
 # test_epochs = [0, 294, 298, 573, 579, 594, 602, 636, 637, 655, 677, 897, 901, 911, 912, 919, 941, 941, 963, 985, 992, 994, 995, 997, 1015, 1247, 1257, 1258, 1260, 1272, 1287, 1290, 1311, 1312, 1313, 1316, 1317, 1323, 1324, 1333, 1334, 1344, 1345, 1346, 1347, 1357, 1365, 1366, 1585, 1589, 1611, 1619, 1621, 1633, 1637, 1640, 1653, 1661, 1662, 1914, 1915, 1916, 1917, 1937, 1938, 1960, 1964, 1967, 1968, 1969, 1978, 1981, 1991, 1996, 2005, 2012, 2019, 2021, 2022, 2264, 2286, 2288, 2318, 2319, 2331, 2332, 2338, 2339, 2371, 2593, 2634, 2635, 2667, 2668, 2690, 2892, 2910, 2921, 2924, 2942, 2943, 2978, 2979, 2984, 2985, 2988, 2992, 2992, 2997, 2999, 3010, 3017, 3018, 3019, 3217, 3239, 3248, 3260, 3261, 3264, 3306, 3307, 3314, 3316, 3318, 3335, 3335, 3336, 3339, 3341, 3341, 3342, 3342, 3345, 3356, 3570, 3625, 3646, 3657]
 # test_mtts = [0.0, 320.8780000000261, 325.24399999994785, 625.3850000002421, 631.933999999892, 648.3059999998659, 657.0360000003129, 694.1440000003204, 695.2370000001974, 714.8820000002161, 738.8940000003204, 979.0049999998882, 983.3710000002757, 994.285000000149, 995.3769999998622, 1003.0160000002943, 1027.0270000002347, 1027.027999999933, 1051.0389999998733, 1075.0509999999776, 1082.691000000108, 1084.8730000001378, 1085.9650000003166, 1088.1480000000447, 1107.7930000000633, 1361.003000000026, 1371.9169999998994, 1373.0079999999143, 1375.191000000108, 1388.2889999998733, 1404.658999999985, 1407.933999999892, 1430.8530000001192, 1431.945000000298, 1433.036000000313, 1436.3100000000559, 1437.4020000002347, 1443.9500000001863, 1445.0419999998994, 1454.8640000000596, 1455.9560000002384, 1466.8700000001118, 1467.9620000002906, 1469.0530000003055, 1470.1450000000186, 1481.058999999892, 1489.7900000000373, 1490.8810000000522, 1729.9020000002347, 1734.2690000003204, 1758.2800000002608, 1767.0109999999404, 1769.194000000134, 1782.2910000002012, 1786.657000000123, 1789.9300000001676, 1804.1189999999478, 1812.851000000257, 1813.942000000272, 2088.9799999999814, 2090.0709999999963, 2091.163000000175, 2092.25400000019, 2114.0819999999367, 2115.1740000001155, 2139.185000000056, 2143.5509999999776, 2146.8250000001863, 2147.916000000201, 2149.0079999999143, 2158.8310000002384, 2162.1049999999814, 2173.0190000003204, 2178.4769999999553, 2188.2990000001155, 2195.939000000246, 2203.5789999999106, 2205.7620000001043, 2206.853000000119, 2470.9769999999553, 2494.9879999998957, 2497.1710000000894, 2529.913000000175, 2531.0049999998882, 2544.1019999999553, 2545.19299999997, 2551.7420000000857, 2552.8330000001006, 2587.7590000000782, 2830.0540000000037, 2874.8020000001416, 2875.8930000001565, 2910.81799999997, 2911.910000000149, 2935.9210000000894, 3156.388000000268, 3176.033999999985, 3188.0389999998733, 3191.313000000082, 3210.9590000002645, 3212.0500000002794, 3250.25, 3251.341000000015, 3256.7990000001155, 3257.8900000001304, 3261.1639999998733, 3265.529000000097, 3265.530999999959, 3270.9870000001974, 3273.1699999999255, 3285.1750000002794, 3292.814999999944, 3293.907000000123, 3294.998000000138, 3511.098999999929, 3535.1099999998696, 3544.933999999892, 3558.0300000002608, 3559.121999999974, 3562.3960000001825, 3608.2349999998696, 3609.3270000000484, 3616.966000000015, 3619.149999999907, 3621.3330000001006, 3639.885000000242, 3639.8870000001043, 3640.978000000119, 3644.253000000026, 3646.435000000056, 3646.435000000056, 3647.526000000071, 3647.526000000071, 3650.8009999999776, 3662.805999999866, 3896.3700000001118, 3956.3980000000447, 3979.31799999997, 3991.323000000324]
 # test_mtts_err = [0.00043, 0.00028, 0.00062, 0.00042, 0.00043, 0.00032, 0.00036, 0.00046, 0.00041, 0.00019, 0.00043, 0.00072, 0.00079, 0.00037, 0.00031, 0.0004, 0.0004, 0.00028, 0.00028, 0.00068, 0.00035, 0.00029, 0.00024, 0.00029, 0.00039, 0.00027, 0.00021, 0.00027, 0.00024, 0.00032, 0.00031, 0.00022, 0.00018, 0.00017, 0.00033, 0.00011, 0.0001, 0.00017, 0.00032, 0.00039, 0.00035, 0.00034, 0.00035, 0.00032, 0.00042, 0.00037, 0.00037, 0.00031, 0.00033, 0.00039, 0.0003, 0.0003, 0.0003, 0.0003, 0.00046, 0.00024, 0.00038, 0.00027, 0.00029, 0.00021, 0.0003, 0.00033, 0.00071, 0.00019, 0.00043, 0.00034, 0.00034, 0.00019, 0.00019, 0.00031, 0.00028, 0.00032, 0.0004, 0.00029, 0.00029, 0.00025, 0.00034, 0.00034, 0.00046, 0.00043, 0.00039, 0.00049, 0.00046, 0.00049, 0.00035, 0.00036, 0.00022, 0.0002, 0.00031, 0.00042, 0.00033, 0.00033, 0.00055, 0.00023, 0.00021, 0.00035, 0.00025, 0.00034, 0.00037, 0.00028, 0.00023, 0.00028, 0.00039, 0.00024, 0.00022, 0.00029, 0.00043, 0.00036, 0.00026, 0.00048, 0.00032, 0.0004, 0.00018, 0.00021, 0.00056, 0.00023, 0.0003, 0.00022, 0.00034, 0.00028, 0.00027, 0.00035, 0.00031, 0.00032, 0.00033, 0.0005, 0.00031, 0.00032, 0.00091, 0.00035, 0.00026, 0.00021, 0.00034, 0.00034, 0.00038, 0.0004, 0.00026, 0.0003, 0.00044]
 test_epochs = np.array([0, 294, 298, 573])
 test_mtts = np.array([0.0, 320.8780000000261, 325.24399999994785, 625.3850000002421])
 test_mtts_err = np.array([0.00043, 0.00028, 0.00062, 0.00042])
-class TestTransitTimes(unittest.TestCase):
+tra_or_occ = np.array(['tra','occ','tra','occ'])
+class TestTimingData(unittest.TestCase):
     """
     Tests:
     beep
     ** s = successful, us = unsuccessful
         test s that each variable is of np.ndarray type=done
         test us that each variable is of np.ndarray type=done
         test s that values in each array are of specified type (epochs=ints, mid_transit_times=floats, uncertainties=floats)=done
@@ -30,222 +31,361 @@
         successful 0, neg and positive =done
         epochs - type of variable (np.array), type of values (int), values are what u expect (if u pass in starting at 0, >0, <0)
         mid transit times - type of variable (np.array), type of values (float), values are what u expect (if u pass in starting at 0, >0, <0)
         mid transit time uncertainties - type of var (np.array), type of vals (float), values are what u expect (if pass in None, array of ones, else (if you pass in actual data and not None) data you pass in
         midtransit times are non-neg
     """
 
-    # Set Up and Tear down Transit times
+    
    
        
     # Test instantiating with correct and incorrect timescales
     def test_successful_instantiation_jd_tdb_timescale(self):
-        """
-            Testing successful instantiation of Transit Times object with the given parameters:
-                epochs: 
-                mid_transit_times:
-                mid_transit_time_errors:
+        """Successful creation of the TimingData object with proper timescale
 
+            Creating the TimingData object with the proper timescale of JD TDB which is
+            barycentric Julian Date. Also including uncertainties.
         """
         # Should not get any errors, the epochs and transit times should be the same as they are inputted
-        self.transit_times = TransitTimes('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
-        self.assertIsInstance(self.transit_times, TransitTimes)  # Check if the object is an instance of TransitTimes
-        shifted_epochs = test_epochs - np.min(test_epochs)
-        self.assertTrue(np.array_equal(self.transit_times.epochs, shifted_epochs))  # Check if epochs remain unchanged
-        self.assertTrue(np.array_equal(self.transit_times.mid_transit_times, test_mtts))  # Check mid_transit_times
-        self.assertTrue(np.array_equal(self.transit_times.mid_transit_times_uncertainties, test_mtts_err))  # Check uncertainties
+        self.timing_data = TimingData('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
+        self.assertIsInstance(self.timing_data, TimingData)  # Check if the object is an instance of TransitTimes
+        shifted_epochs = test_epochs - np.min(test_epochs) 
+        self.assertTrue(np.array_equal(self.timing_data.epochs, shifted_epochs))  # Check if epochs remain unchanged
+        self.assertTrue(np.array_equal(self.timing_data.mid_times, test_mtts))  # Check mid_transit_times
+        self.assertTrue(np.array_equal(self.timing_data.mid_time_uncertainties, test_mtts_err))  # Check uncertainties
 
     def test_s_init_jd_tdb_no_uncertainties(self):
+        """ Successful creation of the TimingData object with proper timescale
+
+            Creating the TimingData object with the proper timescale of JD TDB which is
+            barycentric Julian Date. Not including uncertainties.
+        """
         # Should not get any errors, the epochs and transit times should be the same as they are inputted
-        self.transit_times = TransitTimes('jd', test_epochs, test_mtts, time_scale='tdb')
-        self.assertIsInstance(self.transit_times, TransitTimes)  # Check if the object is an instance of TransitTimes
+        self.timing_data = TimingData('jd', test_epochs, test_mtts, time_scale='tdb')
+        self.assertIsInstance(self.timing_data, TimingData )  # Check if the object is an instance of TransitTimes
         shifted_epochs = test_epochs - np.min(test_epochs)
         shifted_mtt = test_mtts - np.min(test_mtts)
         new_uncertainties = np.ones_like(test_epochs, dtype=float)
-        self.assertTrue(np.array_equal(self.transit_times.epochs, shifted_epochs))  # Check if epochs remain unchanged
-        self.assertTrue(np.array_equal(self.transit_times.mid_transit_times, shifted_mtt))  # Check mid_transit_times
-        self.assertTrue(np.array_equal(self.transit_times.mid_transit_times_uncertainties, new_uncertainties))  # Check uncertainties chage this back!!!
+        self.assertTrue(np.array_equal(self.timing_data.epochs, shifted_epochs))  # Check if epochs remain unchanged
+        self.assertTrue(np.array_equal(self.timing_data.mid_times, shifted_mtt))  # Check mid_transit_times
+        self.assertTrue(np.array_equal(self.timing_data.mid_time_uncertainties, new_uncertainties))  # Check uncertainties chage this back!!!
+
 
-    
 
-    # Test instantiating with correct and incorrect timescales
 
+    # Test successful np.arrays
+    def test_suc_arrays(self):
+        """ Successful test to check that epochs, mid times, mid time uncertainties, and tra_or_occ are all type np.arrays
+
+        """
+        self.timing_data =  TimingData('jd', test_epochs, test_mtts, test_mtts_err, tra_or_occ, time_scale='tdb')
+        self.assertTrue(all(isinstance(value, np.ndarray) for value in self.timing_data.epochs))
+        self.assertTrue(all(isinstance(value, np.ndarray) for value in self.timing_data.mid_times))
+        self.assertTrue(all(isinstance(value, np.ndarray) for value in self.timing_data.mid_time_uncertainties))  
+        self.assertTrue(all(isinstance(value, np.ndarray) for value in self.timing_data.tra_or_occ))  
 
-    # Tests for numpy array validation
+    # Tests for unsucessful np.arrays
     def test_us_epochs_arr_type_str(self):
-        # epochs are strings instead of numpy array
+        """ Unsuccessful test to check for numpy array validation for the epochs.
+            
+            The epochs are strings instead of numpy array and should raise an error.
+        """
         string_test_epochs_arr = str(test_epochs)
         with self.assertRaises(TypeError, msg="The variable 'epochs' expected a NumPy array (np.ndarray) but received a different data type"):
-            TransitTimes('jd', string_test_epochs_arr, test_mtts, test_mtts_err, time_scale='tdb')
+             TimingData('jd', string_test_epochs_arr, test_mtts, test_mtts_err, time_scale='tdb')
      
     def test_us_mtts_arr_type_str(self):
-        # midtransitstimes are strings instead of numpy array
+        """ Unsuccessful test to check for numpy array validation for the mid times.
+
+            The mid times are strings instead of numpy array and should raise an error.
+        """
         string_test_mtts_arr = str(test_mtts)
         with self.assertRaises(TypeError, msg="The variable 'mid_transit_times' expected a NumPy array (np.ndarray) but received a different data type"):
-            TransitTimes('jd', test_epochs, string_test_mtts_arr, test_mtts_err, time_scale='tdb')
+             TimingData('jd', test_epochs, string_test_mtts_arr, test_mtts_err, time_scale='tdb')
     
     def test_us_mtts_err_arr_type_str(self):
-        # mid transit times uncertainites are strings instead of numpy array
+        """ Unsuccessful test to check for numpy array validation for the mid time uncertainties.
+        
+            The mid time uncertainites are strings instead of numpy array and should raise an error.
+        """
         string_test_mtts_err_arr = str(test_mtts_err)
         with self.assertRaises(TypeError, msg="The variable 'mid_transit_times_uncertainties' expected a NumPy array (np.ndarray) but received a different data type"):
-            TransitTimes('jd', test_epochs, test_mtts, string_test_mtts_err_arr, time_scale='tdb')
+             TimingData('jd', test_epochs, test_mtts, string_test_mtts_err_arr, time_scale='tdb')
 
-
-    # Test for data value type validation
+    
+    # Test for successful data value type validation
     def test_s_vars_value_types(self):
-        # should not get any errors
-        self.transit_times = TransitTimes('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
-        self.assertTrue(all(isinstance(value, (int, np.int64)) for value in self.transit_times.epochs))
-        self.assertTrue(all(isinstance(value, float) for value in self.transit_times.mid_transit_times))
-        self.assertTrue(all(isinstance(value, float) for value in self.transit_times.mid_transit_times_uncertainties))
+        """ Successful test to check the correct data type
+
+            Epochs should be integers, mid times should be floats, mid time uncertainties should be floats and tra_or_occ should be strings.
+        """
+        self.timing_data =  TimingData('jd', test_epochs, test_mtts, test_mtts_err, tra_or_occ, time_scale='tdb')
+        self.assertTrue(all(isinstance(value, (int, np.int64)) for value in self.timing_data.epochs))
+        self.assertTrue(all(isinstance(value, float) for value in self.timing_data.mid_times))
+        self.assertTrue(all(isinstance(value, float) for value in self.timing_data.mid_time_uncertainties))
+        self.assertTrue(all(isinstance(value, str) for value in self.timing_data.tra_or_occ))
    
+    # Test for unsuccessful data value type validation
     def test_us_epochs_value_types_float(self):
-        # epochs are floats 
+        """ Unsuccessful test to check for data type validation of the epochs.
+
+            The epochs are floats instead of integers and should raise an error.
+        """
         float_test_epochs = test_epochs.astype(float)
         with self.assertRaises(TypeError, msg="All values in 'epochs' must be of type int."):
-            TransitTimes('jd', float_test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
+             TimingData('jd', float_test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
     
     def test_us_mtts_value_types_int(self):
-        # mid transit times are int error is not being raised
+        """ Unsuccessful test to check for data type validation of the mid times.
+
+            The mid times are integers instead of floats and should raise an error.
+        """
         int_test_mtts= test_mtts.astype(int)
         with self.assertRaises(TypeError, msg="All values in 'mid_transit_times' must be of type float."):
-            TransitTimes('jd', test_epochs, int_test_mtts, test_mtts_err, time_scale='tdb')
+             TimingData('jd', test_epochs, int_test_mtts, test_mtts_err, time_scale='tdb')
     
     def test_us_mtts_err_value_types_int(self):
-        # mid transit times uncertanties are int
+        """ Unsuccessful test to check for data type validation of the mid time uncertainties.
+
+            The mid time uncertainties are integers instead of floats and should raise an error.
+        """
         int_test_mtts_err= test_mtts_err.astype(int)
         with self.assertRaises(TypeError, msg="All values in 'mid_transit_times_uncertainties' must be of type float."):
-            TransitTimes('jd', test_epochs, test_mtts, int_test_mtts_err, time_scale='tdb')
+             TimingData('jd', test_epochs, test_mtts, int_test_mtts_err, time_scale='tdb')
 
 
-    # Checks that epochs work with positive, negative and 0 values when shifted in validation
+    # Checks that epochs work with positive, negative and 0 values when shifted 
     def test_shifted_epochs_zero(self):
-        # shifted epochs work with 0 value
+        """ Successful test to check the shifted epochs function works when the epochs start with 0.
+
+            The epochs should remain the same as the array already starts at zero.
+        """
         test_epochs_zero = np.array([0, 294, 298, 573]).astype(int)
         shifted_epochs_zero = np.array([0, 294, 298, 573]).astype(int)
-        self.transit_times = TransitTimes('jd', test_epochs_zero, test_mtts, test_mtts_err, time_scale='tdb')
-        self.assertTrue(np.array_equal(self.transit_times.epochs, shifted_epochs_zero))
+        self.timing_data =  TimingData('jd', test_epochs_zero, test_mtts, test_mtts_err, time_scale='tdb')
+        self.assertTrue(np.array_equal(self.timing_data.epochs, shifted_epochs_zero))
     
     def test_shifted_epochs_pos(self):
-        # shifted epochs work with postive values
+        """ Successful test to check the shifted epochs function works when the epochs start with a positive number.
+
+            The epochs should shift to start with zero.
+        """
         test_epochs_pos = np.array([1, 294, 298, 573]).astype(int)
         shifted_epochs_pos = np.array([0, 293, 297, 572]).astype(int)
-        self.transit_times = TransitTimes('jd', test_epochs_pos, test_mtts, test_mtts_err, time_scale='tdb')
-        self.assertTrue(np.array_equal(self.transit_times.epochs, shifted_epochs_pos))
+        self.timing_data =  TimingData('jd', test_epochs_pos, test_mtts, test_mtts_err, time_scale='tdb')
+        self.assertTrue(np.array_equal(self.timing_data.epochs, shifted_epochs_pos))
 
     def test_shifted_epochs_neg(self):
-        # shifted epochs work with negative values
+        """ Successful test to check the shifted epochs function works when the epochs start with a negative number.
+
+            The epochs should shift to start with zero.
+        """
         test_epochs_neg = np.array([-1, 294, 298, 573]).astype(int)
         shifted_epochs_neg = np.array([0, 295, 299, 574]).astype(int)
-        self.transit_times = TransitTimes('jd', test_epochs_neg, test_mtts, test_mtts_err, time_scale='tdb')
-        self.assertTrue(np.array_equal(self.transit_times.epochs, shifted_epochs_neg))
+        self.timing_data =  TimingData('jd', test_epochs_neg, test_mtts, test_mtts_err, time_scale='tdb')
+        self.assertTrue(np.array_equal(self.timing_data.epochs, shifted_epochs_neg))
 
 
-    # Checks that mid transit times work with positive, negative and 0 values when shifted in validation
+    # Checks that mid transit times work with positive, negative and 0 values when shifted 
     def test_shifted_mtts_zero(self):
-        #shifted mtts work with 0
+        """ Successful test to check the shifted mid times function works when the mid times start with 0.
+
+            The mid times should remain the same as the array already starts at zero.
+        """
         test_mtts_zero = np.array([0.0, 320.8780000000261, 325.24399999994785, 625.3850000002421])
         shifted_mtts_zero = np.array([0.0, 320.8780000000261, 325.24399999994785, 625.3850000002421])
-        self.transit_times = TransitTimes('jd', test_epochs, test_mtts_zero, test_mtts_err, time_scale='tdb')
-        self.assertTrue(np.array_equal(self.transit_times.mid_transit_times, shifted_mtts_zero))
+        self.timing_data =  TimingData('jd', test_epochs, test_mtts_zero, test_mtts_err, time_scale='tdb')
+        self.assertTrue(np.array_equal(self.timing_data.mid_times, shifted_mtts_zero))
 
     def test_shifted_mtts_pos(self):
-        #shifted mtts work with 1
+        """ Successful test to check the shifted mid times function works when the mid times start with a positive number.
+
+            The mid times should shift to start with zero.
+        """
         test_mtts_pos = np.array([1.0, 320.8780000000261, 325.24399999994785, 625.3850000002421])
         shifted_mtts_pos = np.array([0.0, 319.8780000000261, 324.24399999994785, 624.3850000002421])
-        self.transit_times = TransitTimes('jd', test_epochs, test_mtts_pos, test_mtts_err, time_scale='tdb')
-        self.assertTrue(np.array_equal(self.transit_times.mid_transit_times, shifted_mtts_pos))
+        self.timing_data =  TimingData('jd', test_epochs, test_mtts_pos, test_mtts_err, time_scale='tdb')
+        self.assertTrue(np.array_equal(self.timing_data.mid_times, shifted_mtts_pos))
     
     def test_shifted_mtts_neg(self):
-        #shifted mtts work with -1
+        """ Successful test to check the shifted mid times function works when the mid times start with a negative number.
+
+            The mid times should shift to start with zero.
+        """
         test_mtts_neg = np.array([-1.0, 320.8780000000261, 325.24399999994785, 625.3850000002421])
         shifted_mtts_neg = np.array([0.0, 321.8780000000261, 326.24399999994785, 626.3850000002421])
-        self.transit_times = TransitTimes('jd', test_epochs, test_mtts_neg, test_mtts_err, time_scale='tdb')
-        self.assertTrue(np.array_equal(self.transit_times.mid_transit_times, shifted_mtts_neg))
+        self.timing_data =  TimingData('jd', test_epochs, test_mtts_neg, test_mtts_err, time_scale='tdb')
+        self.assertTrue(np.array_equal(self.timing_data.mid_times, shifted_mtts_neg))
 
 #<————————————————————————————————————————————————————————————————————————————————————————>
-    #mid transit times uncertainties different arrays
     def test_no_mtts_err(self):
-        # mid transit time errors are none
+        """ Successful test for when no mid time uncertainties are given.
+
+            If no mid time uncertainties are given the certainties will be an array ones with a data type of floats and the length of the mid times array.
+        """
         test_mtts_err = None
-        self.transit_times = TransitTimes('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
+        self.timing_data =  TimingData('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
         if test_mtts_err is None:
             new_uncertainities= np.ones_like(test_epochs,dtype=float)
             self.assertTrue(np.all(new_uncertainities==np.ones_like(test_epochs,dtype=float)))
         
     def test_mid_transit_err_ones(self):
-        # mid transit time errors are ones
+        """ Successful test for when the mid time uncertainties are an array of ones.
+        
+        """
         new_test_mtts_err=np.ones_like(test_mtts_err)
-        self.transit_times=TransitTimes('jd', test_epochs, test_mtts, new_test_mtts_err, time_scale='tdb')
-        self.assertTrue(np.array_equal(self.transit_times.mid_transit_times_uncertainties,new_test_mtts_err))
+        self.timing_data= TimingData('jd', test_epochs, test_mtts, new_test_mtts_err, time_scale='tdb')
+        self.assertTrue(np.array_equal(self.timing_data.mid_time_uncertainties,new_test_mtts_err))
 
     def test_mid_transit_err_neg(self):
-        # mid transit time errors are negative
-      test_mtts_err_neg= np.array([-0.00043, -0.00028, -0.00062, -0.00042])
-      with self.assertRaises(ValueError, msg="The 'mid_transit_times_uncertainties' array must contain non-negative and non-zero values."):
-            TransitTimes('jd', test_epochs, test_mtts, test_mtts_err_neg, time_scale='tdb')  
+        """ Unsuccessful test for when the mid time uncertainties are negative.
+
+            The mid time uncertainties must be postive and will raise an error if the values are negative.
+        """
+        test_mtts_err_neg= np.array([-0.00043, -0.00028, -0.00062, -0.00042])
+        with self.assertRaises(ValueError, msg="The 'mid_transit_times_uncertainties' array must contain non-negative and non-zero values."):
+             TimingData('jd', test_epochs, test_mtts, test_mtts_err_neg, time_scale='tdb')  
       
     
     def test_mid_transit_err_zero(self):
-        # mid transit time errors are zero
-      test_mtts_err_zero= np.array([0.,0.,0.,0.])
-      with self.assertRaises(ValueError, msg="The 'mid_transit_times_uncertainties' array must contain non-negative and non-zero values."):
-            TransitTimes('jd', test_epochs, test_mtts, test_mtts_err_zero, time_scale='tdb')  
+        """ Unsuccessful test for when the mid time uncertainties are zero.
+
+            The mid time uncertianties must be postive and greater than zero and will raise an error if the values are zero.
+        """
+        test_mtts_err_zero= np.array([0.,0.,0.,0.])
+        with self.assertRaises(ValueError, msg="The 'mid_transit_times_uncertainties' array must contain non-negative and non-zero values."):
+             TimingData('jd', test_epochs, test_mtts, test_mtts_err_zero, time_scale='tdb')  
 
     def test_mid_transit_err_self(self):
-        # if the data is good then returns the same data
-        self.transit_times = TransitTimes('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
-        self.assertTrue(np.array_equal(self.transit_times.mid_transit_times_uncertainties, test_mtts_err))
+        """ Successful test for postive and greater than zero mid time uncertainties.
 
-    #variables have the same shape
+        """
+        self.timing_data =  TimingData('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
+        self.assertTrue(np.array_equal(self.timing_data.mid_time_uncertainties, test_mtts_err))
+
+    # Tests for the same shape of arrays
     def test_variable_shape(self):
-        self.transit_times = TransitTimes('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
-        self.assertEqual(test_epochs.shape, test_mtts.shape, test_mtts_err.shape)
+        """ Successful test to check that all of the varibles have the same shape.
+
+        """
+        self.timing_data =  TimingData('jd', test_epochs, test_mtts, test_mtts_err, tra_or_occ, time_scale='tdb')
+        self.assertEqual(test_epochs.shape, test_mtts.shape, test_mtts_err.shape, tra_or_occ.shape)
 
-    #variables do not have the same shape
     def test_variable_shape_fail(self):
+        """ Unsuccessful test of the varibles shape.
+
+            The epochs, mid times and mid time uncertainties all have different shapes.
+        """
         new_test_epochs= np.array([0, 298, 573])  
         new_test_mtts= np.array([0.0, 625.3850000002421])
+        new_tra_or_occ = np.array(['tra','tra','occ','occ','occ'])
         with self.assertRaises(ValueError, msg="Shapes of 'epochs', 'mid_transit_times', and 'mid_transit_times_uncertainties' arrays do not match."):
-            TransitTimes('jd', new_test_epochs, new_test_mtts, test_mtts_err, time_scale='tdb')  
+             TimingData('jd', new_test_epochs, new_test_mtts, test_mtts_err, new_tra_or_occ, time_scale='tdb')  
     
-   #successful no NaN values in variables
+   # Tests for NaN values
     def successful_no_nan_values(self):
-        self.transit_times = TransitTimes('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
+        """ Successful test for no Not a Number (NaN) values.
+
+            No NaN values in epochs, mid times and mid times uncertainties.
+        """
+        self.timing_data =  TimingData('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb')
         self.assertNotIn(np.nan,test_epochs)
         self.assertNotIn(np.nan,test_mtts)
         self.assertNotIn(np.nan,test_mtts_err)
 
-
-    #mid transit times have no NaN values
     def test_mtts_nan(self):
+        """ Unsuccessful test to check NaN values in mid times.
+
+            Mid times cannot have any NaN values within the array.
+        """
         new_test_mtts=np.array([0., np.nan , 298. ,573.], dtype=float)
         with self.assertRaises(ValueError, msg="The 'mid_transit_times' array contains NaN (Not-a-Number) values."):
-            TransitTimes('jd', test_epochs, new_test_mtts, test_mtts_err, time_scale='tdb')  
+             TimingData('jd', test_epochs, new_test_mtts, test_mtts_err, time_scale='tdb')  
     
     
-     #mid transit time uncertainites have no NaN values
     def test_mtts_err_nan(self):
+        """ Unsuccessful test to check NaN values in mid times uncertainties.
+
+            Mid times uncertainties cannot have any NaN values within the array.
+        """
         new_test_mtts_err=np.array([0.00043, np.nan, 0.00062, 0.00042], dtype=float)
         with self.assertRaises(ValueError, msg="The 'mid_transit_times_uncertainties' array contains NaN (Not-a-Number) values."):
-            TransitTimes('jd', test_epochs, test_mtts, new_test_mtts_err, time_scale='tdb')  
+             TimingData('jd', test_epochs, test_mtts, new_test_mtts_err, time_scale='tdb')  
+
+    # #tests for calc_barycentric_time
+    # test_time_obj_ones=np.array([1.0, 1.0, 1.0, 1.0])
+    # test_time_obj=np.array([0.00034,0.0006,0.0005,0.0008])
+    # test_obj_location= np.array([1.0,2.0])
+    # test_obs_locations=np.array([2.0,3.0])
+    # #check uncertainties arent ones
+    # def calc_bary_time_instantiation(self):
+    #     self.timing_data =  TimingData('jd', test_epochs, test_mtts, test_mtts_err, object_ra=97.64, object_dec=29.67, observatory_lat=43.60, observatory_lon=-116.21)
+    #     self.assertIsInstance(self.timing_data,  TimingData)
+    
+    # def calc_bary_time_uncertinties(self):
+    #    test_mtts_err=np.array([1.0, 1.0, 1.0, 1.0])
+    #    self.timing_data =  TimingData('jd', test_epochs, test_mtts,test_mtts_err, object_ra=97.64, object_dec=29.67, observatory_lat=43.60, observatory_lon=-116.21)
+
+
+    # Tests for validate tra_or_occ
+    ###### NEED TO FINISH ######
+    def test_tra_or_occ_None(self):
+        self.timing_data = TimingData('jd', test_epochs, test_mtts, test_mtts_err, time_scale='tdb', tra_or_occ = None)
+        expected_result = np.array(['tra','tra','tra','tra'])
+        result = self.timing_data._validate()
+        self.assertTrue(np.allclose(expected_result, result, rtol=1e-05, atol=1e-08))
+
+    
+    def test_only_tra_or_occ_value(self):
+        """ Unsuccessful test to check if the tra_or_occ array contains values other than 'tra' or 'occ'.
+
+        """
+        not_tra_or_occ = np.array(['tra','occ','trac','oc'])
+        with self.assertRaises(ValueError, msg="tra_or_occ array cannot contain string values other than 'tra' or 'occ'"):
+             TimingData('jd', test_epochs, test_mtts, test_mtts_err,not_tra_or_occ, time_scale='tdb')  
+
+    def test_tra_or_occ_array(self):
+        """ Unsuccessful test to check if the tra_or_occ varible is a numpy array.
+
+        """
+        not_tra_or_occ = str(tra_or_occ)
+        with self.assertRaises(TypeError, msg= "The variable 'tra_or_occ' expected a NumPy array (np.ndarray) but received a different data type"):
+             TimingData('jd', test_epochs, test_mtts, test_mtts_err,not_tra_or_occ, time_scale='tdb')  
+
+
+    def test_tra_or_occ_shape(self):
+        """ Unsuccessful test to check the length of the tra_or_occ array.
+
+            The tra_or_occ array must be the same length as the epochs. mid times and mid time uncertainties arrays.
+        """
+        not_tra_or_occ = np.array(['occ','tra','occ'])
+        with self.assertRaises(ValueError, msg= "Shapes of 'tra_or_occ', 'mid_time_uncertainties', and 'mid_times' arrays do not match."):
+             TimingData('jd', test_epochs, test_mtts, test_mtts_err,not_tra_or_occ, time_scale='tdb')  
+
+    def test_tra_or_occ_str(self):
+        """ Unsuccessful test to check the data values within the tra_or_occ array.
+
+            The data values must be a string and will raise an error if not.
+        """
+        not_tra_or_occ = np.array([1,2,3,4])
+        with self.assertRaises(ValueError, msg= "All values in 'tra_or_occ' must be of type string."):
+             TimingData('jd', test_epochs, test_mtts, test_mtts_err,not_tra_or_occ, time_scale='tdb')  
+    
+
+    def test_tra_or_occ_no_null(self):
+        """ Unsuccessful test to check if any null values are in the tra_or_occ array.
+
+            The data values cannot contain any null values of an error will be rasied if not.
+        """
+        not_tra_or_occ = np.array(['tra','occ', None, None])
+        with self.assertRaises(ValueError, msg = "The 'tra_or_occ' array contains NaN (Not-a-Number) values."):
+             TimingData('jd', test_epochs, test_mtts, test_mtts_err,not_tra_or_occ, time_scale='tdb')  
+    
+
 
-    #tests for calc_barycentric_time
-    test_time_obj_ones=np.array([1.0, 1.0, 1.0, 1.0])
-    test_time_obj=np.array([0.00034,0.0006,0.0005,0.0008])
-    test_obj_location= np.array([1.0,2.0])
-    test_obs_locations=np.array([2.0,3.0])
-    #check uncertainties arent ones
-    def calc_bary_time_instantiation(self):
-        self.transit_times = TransitTimes('jd', test_epochs, test_mtts, test_mtts_err, object_ra=97.64, object_dec=29.67, observatory_lat=43.60, observatory_lon=-116.21)
-        self.assertIsInstance(self.transit_times, TransitTimes)
-    
-    def calc_bary_time_uncertinties(self):
-       test_mtts_err=np.array([1.0, 1.0, 1.0, 1.0])
-       self.transit_times= TransitTimes('jd', test_epochs, test_mtts,test_mtts_err, object_ra=97.64, object_dec=29.67, observatory_lat=43.60, observatory_lon=-116.21)
     
     # def test_successful_instantiation_jd_no_timescale(self):
     #     transit_times = TransitTimes('jd', )
     # def test_successful_instantiation_jd_non_tdb_timescale(self):
     #     transit_times = TransitTimes('jd', )
     # def test_successful_instantiation_non_jd_tdb_timescale(self):
     #     transit_times = TransitTimes('mjd', time_scale='tdb')
```

