# Comparing `tmp/flightcondition-24.3.31.tar.gz` & `tmp/flightcondition-24.5.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightcondition-24.3.31.tar", last modified: Mon Apr  1 02:32:56 2024, max compression
+gzip compressed data, was "flightcondition-24.5.13.tar", last modified: Tue May 14 01:39:40 2024, max compression
```

## Comparing `flightcondition-24.3.31.tar` & `flightcondition-24.5.13.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2024-04-01 02:32:56.570133 flightcondition-24.3.31/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1073 2022-03-31 22:06:28.000000 flightcondition-24.3.31/LICENSE
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    14496 2024-04-01 02:32:56.570133 flightcondition-24.3.31/PKG-INFO
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13666 2024-04-01 02:32:07.000000 flightcondition-24.3.31/README.md
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1673 2024-04-01 02:32:56.573134 flightcondition-24.3.31/setup.cfg
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      132 2022-07-21 02:57:11.000000 flightcondition-24.3.31/setup.py
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2024-04-01 02:32:56.292952 flightcondition-24.3.31/src/
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2024-04-01 02:32:56.447133 flightcondition-24.3.31/src/flightcondition/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      587 2022-08-17 22:55:21.000000 flightcondition-24.3.31/src/flightcondition/__init__.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     7777 2024-04-01 02:32:07.000000 flightcondition-24.3.31/src/flightcondition/__main__.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    34813 2024-04-01 02:32:07.000000 flightcondition-24.3.31/src/flightcondition/atmosphere.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8554 2022-08-21 19:03:21.000000 flightcondition-24.3.31/src/flightcondition/boundarylayer.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8190 2023-08-07 01:41:17.000000 flightcondition-24.3.31/src/flightcondition/common.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4170 2024-04-01 02:32:07.000000 flightcondition-24.3.31/src/flightcondition/constants.py
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2024-04-01 02:32:56.556135 flightcondition-24.3.31/src/flightcondition/data/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4453 2023-01-20 22:21:17.000000 flightcondition-24.3.31/src/flightcondition/data/constants_en.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    30564 2023-01-20 22:21:17.000000 flightcondition-24.3.31/src/flightcondition/data/fc_units_en.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    52578 2024-04-01 02:32:07.000000 flightcondition-24.3.31/src/flightcondition/flightcondition.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    11868 2023-01-24 00:34:12.000000 flightcondition-24.3.31/src/flightcondition/isentropicflow.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4128 2023-08-07 01:34:03.000000 flightcondition-24.3.31/src/flightcondition/nondimensional.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     2662 2022-08-16 02:54:58.000000 flightcondition-24.3.31/src/flightcondition/normalshock.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     6157 2023-08-05 02:53:31.000000 flightcondition-24.3.31/src/flightcondition/units.py
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2024-04-01 02:32:56.528133 flightcondition-24.3.31/src/flightcondition.egg-info/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    14496 2024-04-01 02:32:55.000000 flightcondition-24.3.31/src/flightcondition.egg-info/PKG-INFO
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      794 2024-04-01 02:32:56.000000 flightcondition-24.3.31/src/flightcondition.egg-info/SOURCES.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2024-04-01 02:32:55.000000 flightcondition-24.3.31/src/flightcondition.egg-info/dependency_links.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       66 2024-04-01 02:32:55.000000 flightcondition-24.3.31/src/flightcondition.egg-info/entry_points.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       44 2024-04-01 02:32:55.000000 flightcondition-24.3.31/src/flightcondition.egg-info/requires.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       16 2024-04-01 02:32:55.000000 flightcondition-24.3.31/src/flightcondition.egg-info/top_level.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2022-04-24 20:23:49.000000 flightcondition-24.3.31/src/flightcondition.egg-info/zip-safe
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2024-05-14 01:39:40.604202 flightcondition-24.5.13/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1073 2022-03-31 22:06:28.000000 flightcondition-24.5.13/LICENSE
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    14496 2024-05-14 01:39:40.605202 flightcondition-24.5.13/PKG-INFO
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13666 2024-04-01 02:32:07.000000 flightcondition-24.5.13/README.md
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1673 2024-05-14 01:39:40.608203 flightcondition-24.5.13/setup.cfg
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      132 2022-07-21 02:57:11.000000 flightcondition-24.5.13/setup.py
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2024-05-14 01:39:40.306659 flightcondition-24.5.13/src/
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2024-05-14 01:39:40.467291 flightcondition-24.5.13/src/flightcondition/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      587 2022-08-17 22:55:21.000000 flightcondition-24.5.13/src/flightcondition/__init__.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     7982 2024-05-14 01:38:46.000000 flightcondition-24.5.13/src/flightcondition/__main__.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    35782 2024-05-14 01:38:46.000000 flightcondition-24.5.13/src/flightcondition/atmosphere.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8554 2022-08-21 19:03:21.000000 flightcondition-24.5.13/src/flightcondition/boundarylayer.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8190 2023-08-07 01:41:17.000000 flightcondition-24.5.13/src/flightcondition/common.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4170 2024-04-01 02:32:07.000000 flightcondition-24.5.13/src/flightcondition/constants.py
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2024-05-14 01:39:40.588377 flightcondition-24.5.13/src/flightcondition/data/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4453 2023-01-20 22:21:17.000000 flightcondition-24.5.13/src/flightcondition/data/constants_en.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    30564 2023-01-20 22:21:17.000000 flightcondition-24.5.13/src/flightcondition/data/fc_units_en.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    53020 2024-05-14 01:38:46.000000 flightcondition-24.5.13/src/flightcondition/flightcondition.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    11868 2023-01-24 00:34:12.000000 flightcondition-24.5.13/src/flightcondition/isentropicflow.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4122 2024-05-14 01:38:46.000000 flightcondition-24.5.13/src/flightcondition/nondimensional.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     2662 2022-08-16 02:54:58.000000 flightcondition-24.5.13/src/flightcondition/normalshock.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     6157 2023-08-05 02:53:31.000000 flightcondition-24.5.13/src/flightcondition/units.py
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2024-05-14 01:39:40.557138 flightcondition-24.5.13/src/flightcondition.egg-info/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    14496 2024-05-14 01:39:39.000000 flightcondition-24.5.13/src/flightcondition.egg-info/PKG-INFO
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      794 2024-05-14 01:39:40.000000 flightcondition-24.5.13/src/flightcondition.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2024-05-14 01:39:39.000000 flightcondition-24.5.13/src/flightcondition.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       66 2024-05-14 01:39:39.000000 flightcondition-24.5.13/src/flightcondition.egg-info/entry_points.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       44 2024-05-14 01:39:39.000000 flightcondition-24.5.13/src/flightcondition.egg-info/requires.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       16 2024-05-14 01:39:39.000000 flightcondition-24.5.13/src/flightcondition.egg-info/top_level.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2022-04-24 20:23:49.000000 flightcondition-24.5.13/src/flightcondition.egg-info/zip-safe
```

### Comparing `flightcondition-24.3.31/LICENSE` & `flightcondition-24.5.13/LICENSE`

 * *Files identical despite different names*

### Comparing `flightcondition-24.3.31/PKG-INFO` & `flightcondition-24.5.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightcondition
-Version: 24.3.31
+Version: 24.5.13
 Summary: Airspeed conversions (true/calibrated/equivalent/Mach),
 Home-page: https://github.com/MattCJones/flightcondition
 Author: Matthew C. Jones
 Author-email: matt.c.jones.aoe@gmail.com
 License: MIT License
 Keywords: utility,aerospace,engineering,design
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flightcondition-24.3.31/README.md` & `flightcondition-24.5.13/README.md`

 * *Files identical despite different names*

### Comparing `flightcondition-24.3.31/setup.cfg` & `flightcondition-24.5.13/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Topic :: Scientific/Engineering
 	Topic :: Utilities
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
-version = 24.03.31
+version = 24.05.13
 
 [options]
 packages = find:
 package_dir = 
 	= src
 zip_safe = True
 python_requires = >=3.8
```

### Comparing `flightcondition-24.3.31/src/flightcondition/__init__.py` & `flightcondition-24.5.13/src/flightcondition/__init__.py`

 * *Files identical despite different names*

### Comparing `flightcondition-24.3.31/src/flightcondition/__main__.py` & `flightcondition-24.5.13/src/flightcondition/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -125,15 +125,18 @@
         action='store_true', help="display abbreviated output")
     parser.add_argument(  # hidden option to turn off pretty print
         '--no-pretty-print', dest='no_pretty_print', default=False,
         action='store_true', help=argparse.SUPPRESS)
     parser.add_argument(
         '--model', dest='model', metavar='', nargs=None,
         type=str, default=None,
-        help=f"Atmospheric model, e.g., 'standard' or 'msis2.1'")
+        help=("Atmospheric model, e.g., 'standard' or 'msis2.1'. If using msis"
+              " use '--datetime' for the date/time "
+              "(default='2003-01-01T00:00') , '--lon' for longitude "
+              "(default=0), and '--lat' for latitude (default=0)"))
     parser.add_argument(
         '--datetime', dest='datetime', metavar='', nargs=None, type=str,
         default=None, help=argparse.SUPPRESS)
     parser.add_argument(
         '--lon', dest='lon', metavar='', nargs=None, type=float,
         default=None, help=argparse.SUPPRESS)
     parser.add_argument(
```

### Comparing `flightcondition-24.3.31/src/flightcondition/atmosphere.py` & `flightcondition-24.5.13/src/flightcondition/atmosphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,31 +203,46 @@
         'O': 'atomic_oxygen',
         'He': 'helium',
         'H': 'hydrogen',
         'Ar': 'argon',
         'N': 'nitrogen',
         'aO': 'anomalous_oxygen',
         'NO': 'nitric_oxide',
+        'nrho': 'number_density',
     }
 
     def __init__(self, species_arr, full_output=True, units=None):
         """Initialize Species class.
 
         Args:
             species_arr (array): Array of species concentrations
         """
-        self._N2 = species_arr[0]
-        self._O2 = species_arr[1]
-        self._O = species_arr[2]
-        self._He = species_arr[3]
-        self._H = species_arr[4]
-        self._Ar = species_arr[5]
-        self._N = species_arr[6]
-        self._aO = species_arr[7]
-        self._NO = species_arr[8]
+        N2_mn3 = species_arr[0]
+        O2_mn3 = species_arr[1]
+        O_mn3 = species_arr[2]
+        He_mn3 = species_arr[3]
+        H_mn3 = species_arr[4]
+        Ar_mn3 = species_arr[5]
+        N_mn3 = species_arr[6]
+        aO_mn3 = species_arr[7]
+        NO_mn3 = species_arr[8]
+
+        self._nrho = N2_mn3 + O2_mn3 + O_mn3 + He_mn3 + H_mn3 + Ar_mn3 + N_mn3\
+                   + aO_mn3 + NO_mn3
+
+        self._N2 = N2_mn3/self._nrho
+        self._O2 = O2_mn3/self._nrho
+        self._O = O_mn3/self._nrho
+        self._He = He_mn3/self._nrho
+        self._H = H_mn3/self._nrho
+        self._Ar = Ar_mn3/self._nrho
+        self._N = N_mn3/self._nrho
+        self._aO = aO_mn3/self._nrho
+        self._NO = NO_mn3/self._nrho
+
         self.full_output = full_output
         self.units = units
 
     def tostring(self, full_output=None, units=None, max_sym_chars=None,
                  max_name_chars=None, pretty_print=True):
         """Output string representation of class object.
 
@@ -248,17 +263,18 @@
             else:
                 full_output = self.full_output
 
         if units is not None:
             self.units = units
 
         if self.units == 'US':
-            species_units   = '1/ft^3'
+            nrho_units   = '1/ft^3'
         else:  # SI units
-            species_units   = '1/m^3'
+            nrho_units   = '1/m^3'
+        species_units   = ''
 
         # Insert longer variable name into output
         if max_sym_chars is None:
             max_sym_chars = max([len(v) for v in self.names_dict.keys()])
         if max_name_chars is None:
             max_name_chars = max([len(v) for v in self.names_dict.values()])
 
@@ -304,21 +320,27 @@
                                 fmt_val="10.5g", pretty_print=pretty_print)
         NO_str = self._vartostr(var=self.NO, var_str='NO',
                                 to_units=species_units,
                                 max_sym_chars=max_sym_chars,
                                 max_name_chars=max_name_chars,
                                 fmt_val="10.5g", pretty_print=pretty_print)
 
+        nrho_str = self._vartostr(var=self.nrho, var_str='nrho',
+                                to_units=nrho_units,
+                                max_sym_chars=max_sym_chars,
+                                max_name_chars=max_name_chars,
+                                fmt_val="10.5g", pretty_print=pretty_print)
+
         # Assemble output string
         if full_output:
             repr_str = (f"{N2_str}\n{O2_str}\n{O_str}\n{He_str}\n{H_str}"
-                        f"\n{Ar_str}\n{N_str}\n{aO_str}\n{NO_str}")
+                        f"\n{Ar_str}\n{N_str}\n{aO_str}\n{NO_str}\n{nrho_str}")
         else:
             repr_str = (f"{N2_str}\n{O2_str}\n{O_str}\n{He_str}\n{H_str}"
-                        f"\n{Ar_str}\n{N_str}\n{aO_str}\n{NO_str}")
+                        f"\n{Ar_str}\n{N_str}\n{aO_str}\n{NO_str}\n{nrho_str}")
         return repr_str
 
 
     @_property_decorators
     def N2(self):
         """Diatomic nitrogen. """
         return self._N2
@@ -356,17 +378,22 @@
     @_property_decorators
     def aO(self):
         """Anomalous oxygen. """
         return self._aO
 
     @_property_decorators
     def NO(self):
-        """Nitric oxide."""
+        """Nitric oxide. """
         return self._NO
 
+    @_property_decorators
+    def nrho(self):
+        """Number density. """
+        return self._nrho
+
 
 class Atmosphere(DimensionalData):
     """Compute quantities from International Civil Aviation Organization (ICAO)
     1993, which extends the US 1976 Standard Atmospheric Model to 80 km.
 
     Usage:
         from flightcondition import Atmosphere, unit
@@ -645,14 +672,15 @@
         _version = 2 if _version == 2.0 else _version
 
         self.model = f"msis{_version:1.1f}"
 
         _out = msis.run(dates=self._datetime, lons=self._lon, lats=self._lat,
                         alts=h_km, f107s=self._f107, f107as=self._f107a,
                         version=_version)
+        _out[np.isnan(_out)] = 0.0
         N_species = 9  # N2 O2 O He H Ar N aO NO
         N_fc = len(self._h)
         out = _out.reshape((N_fc, N_species+2))
 
         # Unpack # TODO 2024-03-25: get this to work for arrays of altitudes
         rho_kgpm3 = out[:, 0]
         N2_mn3 = out[:, 1]
```

### Comparing `flightcondition-24.3.31/src/flightcondition/boundarylayer.py` & `flightcondition-24.5.13/src/flightcondition/boundarylayer.py`

 * *Files identical despite different names*

### Comparing `flightcondition-24.3.31/src/flightcondition/common.py` & `flightcondition-24.5.13/src/flightcondition/common.py`

 * *Files identical despite different names*

### Comparing `flightcondition-24.3.31/src/flightcondition/constants.py` & `flightcondition-24.5.13/src/flightcondition/constants.py`

 * *Files identical despite different names*

### Comparing `flightcondition-24.3.31/src/flightcondition/data/constants_en.txt` & `flightcondition-24.5.13/src/flightcondition/data/constants_en.txt`

 * *Files identical despite different names*

### Comparing `flightcondition-24.3.31/src/flightcondition/data/fc_units_en.txt` & `flightcondition-24.5.13/src/flightcondition/data/fc_units_en.txt`

 * *Files identical despite different names*

### Comparing `flightcondition-24.3.31/src/flightcondition/flightcondition.py` & `flightcondition-24.5.13/src/flightcondition/flightcondition.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,15 @@
         'L': 'length_scale',
         'Re': 'reynolds_number',
         'h_BL_lamr': 'boundary_thickness_laminar',
         'h_BL_turb': 'boundary_thickness_turbulent',
         'Cf_lamr': 'friction_coefficient_laminar',
         'Cf_turb': 'friction_coefficient_turbulent',
         'h_yplus1': 'wall_distance_yplus1',
+        'Kn': 'knudsen_number',
     }
     names_dict = {}
     names_dict.update(_byalt_names)
     names_dict.update(_byvel_names)
     names_dict.update(_bylen_names)
 
 # =========================================================================== #
@@ -1264,19 +1265,23 @@
             var=self.Cf_turb, var_str='Cf_turb', to_units=dimless,
             max_sym_chars=max_sym_chars, max_name_chars=max_name_chars,
             fmt_val="10.5g", pretty_print=pretty_print)
         h_yplus1_str = self._vartostr(
             var=self.h_yplus1, var_str='h_yplus1', to_units=h_BL_units,
             max_sym_chars=max_sym_chars, max_name_chars=max_name_chars,
             fmt_val="10.5g", pretty_print=pretty_print)
+        Kn_str = self._vartostr(
+            var=self.Kn, var_str='Kn', to_units='',
+            max_sym_chars=max_sym_chars, max_name_chars=max_name_chars,
+            fmt_val="10.5g", pretty_print=pretty_print)
 
         if full_output:
             repr_str = (f"{L_str}\n{Re_str}\n{h_BL_lamr_str}\n"
                         f"{h_BL_turb_str}\n{Cf_lamr_str}\n{Cf_turb_str}\n"
-                        f"{h_yplus1_str}")
+                        f"{h_yplus1_str}\n{Kn_str}")
         else:
             repr_str = (f"{L_str}\n{Re_str}")
 
         return repr_str
 
     @to_base_units_wrapper
     def wall_distance_from_yplus(self, yplus):
@@ -1401,7 +1406,14 @@
         return Cf_turb
 
     @_property_decorators
     def h_yplus1(self):
         """Get height from flat plate wall in turbulent flow where yplus=1. """
         h_yplus1 = self.wall_distance_from_yplus(1)
         return h_yplus1
+
+    @_property_decorators
+    def Kn(self):
+        """Get Knudsen number :math:`Kn`"""
+        Kn = NonDimensional.knudsen_number(
+            L=self.L, MFP=self.MFP)
+        return Kn
```

### Comparing `flightcondition-24.3.31/src/flightcondition/isentropicflow.py` & `flightcondition-24.5.13/src/flightcondition/isentropicflow.py`

 * *Files identical despite different names*

### Comparing `flightcondition-24.3.31/src/flightcondition/nondimensional.py` & `flightcondition-24.5.13/src/flightcondition/nondimensional.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 from flightcondition.constants import PhysicalConstants as Phys
 from flightcondition.units import dimless, to_base_units_wrapper
 
 class NonDimensional:
     """Compute non-dimensional flow quantities. """
 
     @staticmethod
-    def knudsen_number(ell, MFP):
+    def knudsen_number(L, MFP):
         """Compute the Knudsen number :math:`K_n`
 
         Args:
-            ell (length): Length scale
+            L (length): Length scale
             MFP (length): Mean free path
 
         Returns:
             dimless: Knudsen number
         """
-        Kn = MFP/ell
+        Kn = MFP/L
         return Kn
 
     @staticmethod
     def mach_number(U, a):
         """Compute Mach number
 
         Args:
```

### Comparing `flightcondition-24.3.31/src/flightcondition/normalshock.py` & `flightcondition-24.5.13/src/flightcondition/normalshock.py`

 * *Files identical despite different names*

### Comparing `flightcondition-24.3.31/src/flightcondition/units.py` & `flightcondition-24.5.13/src/flightcondition/units.py`

 * *Files identical despite different names*

### Comparing `flightcondition-24.3.31/src/flightcondition.egg-info/PKG-INFO` & `flightcondition-24.5.13/src/flightcondition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightcondition
-Version: 24.3.31
+Version: 24.5.13
 Summary: Airspeed conversions (true/calibrated/equivalent/Mach),
 Home-page: https://github.com/MattCJones/flightcondition
 Author: Matthew C. Jones
 Author-email: matt.c.jones.aoe@gmail.com
 License: MIT License
 Keywords: utility,aerospace,engineering,design
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flightcondition-24.3.31/src/flightcondition.egg-info/SOURCES.txt` & `flightcondition-24.5.13/src/flightcondition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

