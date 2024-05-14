# Comparing `tmp/REFPROP_connector-0.3.8.tar.gz` & `tmp/REFPROP_connector-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "REFPROP_connector-0.3.8.tar", last modified: Wed Dec 13 17:05:13 2023, max compression
+gzip compressed data, was "REFPROP_connector-0.3.9.tar", last modified: Tue May  7 08:33:04 2024, max compression
```

## Comparing `REFPROP_connector-0.3.8.tar` & `REFPROP_connector-0.3.9.tar`

### file list

```diff
@@ -1,37 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-12-13 17:05:13.136480 REFPROP_connector-0.3.8/
--rw-rw-rw-   0        0        0       26 2022-06-23 09:23:17.000000 REFPROP_connector-0.3.8/.gitignore
--rw-rw-rw-   0        0        0    35823 2021-12-10 08:32:10.000000 REFPROP_connector-0.3.8/LICENSE
--rw-rw-rw-   0        0        0     7423 2023-12-13 17:05:13.136480 REFPROP_connector-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     5261 2023-07-14 14:18:47.000000 REFPROP_connector-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-12-13 17:05:13.067481 REFPROP_connector-0.3.8/REFPROPConnector/
--rwxrwxrwx   0        0        0  5280688 2021-12-10 08:32:10.000000 REFPROP_connector-0.3.8/REFPROPConnector/NIST2310.EXE
-drwxrwxrwx   0        0        0        0 2023-12-13 17:05:13.070480 REFPROP_connector-0.3.8/REFPROPConnector/Support/
--rw-rw-rw-   0        0        0        0 2022-02-03 11:33:25.000000 REFPROP_connector-0.3.8/REFPROPConnector/Support/__init__.py
--rw-rw-rw-   0        0        0     2211 2023-12-13 16:56:24.000000 REFPROP_connector-0.3.8/REFPROPConnector/Support/constants.py
--rw-rw-rw-   0        0        0    14753 2023-12-13 16:52:42.000000 REFPROP_connector-0.3.8/REFPROPConnector/Support/refprop_names_tree.py
-drwxrwxrwx   0        0        0        0 2023-12-13 17:05:13.099499 REFPROP_connector-0.3.8/REFPROPConnector/Support/resources/
--rw-rw-rw-   0        0        0       30 2023-12-13 16:59:54.000000 REFPROP_connector-0.3.8/REFPROPConnector/Support/resources/REFPROP_exec.dat
--rw-rw-rw-   0        0        0    28642 2023-09-30 19:06:42.000000 REFPROP_connector-0.3.8/REFPROPConnector/Support/resources/REFPROP_names.xml
--rw-rw-rw-   0        0        0        0 2022-02-03 11:35:20.000000 REFPROP_connector-0.3.8/REFPROPConnector/Support/resources/__init__.py
--rw-rw-rw-   0        0        0     3006 2023-09-30 19:04:14.000000 REFPROP_connector-0.3.8/REFPROPConnector/Support/resources/file_handler.py
--rw-rw-rw-   0        0        0    28966 2023-09-30 19:06:26.000000 REFPROP_connector-0.3.8/REFPROPConnector/Support/resources/rp_names_file_generator.py
-drwxrwxrwx   0        0        0        0 2023-12-13 17:05:13.112499 REFPROP_connector-0.3.8/REFPROPConnector/Tools/
--rw-rw-rw-   0        0        0        0 2023-09-30 16:18:06.000000 REFPROP_connector-0.3.8/REFPROPConnector/Tools/__init__.py
--rw-rw-rw-   0        0        0    12110 2023-07-14 14:17:58.000000 REFPROP_connector-0.3.8/REFPROPConnector/Tools/refprop_plotter.py
--rw-rw-rw-   0        0        0     1289 2023-09-30 16:56:34.000000 REFPROP_connector-0.3.8/REFPROPConnector/Tools/units_converter.py
--rw-rw-rw-   0        0        0      280 2023-09-30 16:21:57.000000 REFPROP_connector-0.3.8/REFPROPConnector/__init__.py
--rw-rw-rw-   0        0        0    27343 2023-12-13 16:53:10.000000 REFPROP_connector-0.3.8/REFPROPConnector/refprop_calculator.py
-drwxrwxrwx   0        0        0        0 2023-12-13 17:05:13.068480 REFPROP_connector-0.3.8/REFPROPConnectorTest/
--rw-rw-rw-   0        0        0        0 2021-12-10 10:12:18.000000 REFPROP_connector-0.3.8/REFPROPConnectorTest/__init__.py
--rw-rw-rw-   0        0        0     4817 2023-12-13 16:59:48.000000 REFPROP_connector-0.3.8/REFPROPConnectorTest/test_file.py
-drwxrwxrwx   0        0        0        0 2023-12-13 17:05:13.134481 REFPROP_connector-0.3.8/REFPROP_connector.egg-info/
--rw-rw-rw-   0        0        0     7423 2023-12-13 17:05:12.000000 REFPROP_connector-0.3.8/REFPROP_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      966 2023-12-13 17:05:12.000000 REFPROP_connector-0.3.8/REFPROP_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-13 17:05:12.000000 REFPROP_connector-0.3.8/REFPROP_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-12-13 17:05:12.000000 REFPROP_connector-0.3.8/REFPROP_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-12-13 17:05:12.000000 REFPROP_connector-0.3.8/REFPROP_connector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-07-14 13:26:58.000000 REFPROP_connector-0.3.8/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-12-13 17:05:13.137499 REFPROP_connector-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2268 2023-12-13 17:03:44.000000 REFPROP_connector-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-13 17:05:13.135480 REFPROP_connector-0.3.8/twine_upload/
--rw-rw-rw-   0        0        0     1089 2022-06-21 16:26:22.000000 REFPROP_connector-0.3.8/twine_upload/pip_upload.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:33:04.151889 REFPROP_connector-0.3.9/
+-rw-rw-rw-   0        0        0       26 2022-06-23 09:23:17.000000 REFPROP_connector-0.3.9/.gitignore
+-rw-rw-rw-   0        0        0    35823 2021-12-10 08:32:10.000000 REFPROP_connector-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0     8204 2024-05-07 08:33:04.152890 REFPROP_connector-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5898 2024-05-07 08:30:41.000000 REFPROP_connector-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 08:33:04.107888 REFPROP_connector-0.3.9/REFPROPConnector/
+drwxrwxrwx   0        0        0        0 2024-05-07 08:33:04.116888 REFPROP_connector-0.3.9/REFPROPConnector/Handlers/
+drwxrwxrwx   0        0        0        0 2024-05-07 08:33:04.118888 REFPROP_connector-0.3.9/REFPROPConnector/Handlers/Tools/
+-rw-rw-rw-   0        0        0        0 2023-09-30 16:18:06.000000 REFPROP_connector-0.3.9/REFPROPConnector/Handlers/Tools/__init__.py
+-rw-rw-rw-   0        0        0    12110 2023-07-14 14:17:58.000000 REFPROP_connector-0.3.9/REFPROPConnector/Handlers/Tools/refprop_plotter.py
+-rw-rw-rw-   0        0        0     1293 2024-02-05 07:39:25.000000 REFPROP_connector-0.3.9/REFPROPConnector/Handlers/Tools/units_converter.py
+-rw-rw-rw-   0        0        0     6626 2024-05-07 08:22:41.000000 REFPROP_connector-0.3.9/REFPROPConnector/Handlers/__base_handler.py
+-rw-rw-rw-   0        0        0      182 2024-05-07 08:02:17.000000 REFPROP_connector-0.3.9/REFPROPConnector/Handlers/__init__.py
+-rw-rw-rw-   0        0        0     3948 2024-05-07 07:55:18.000000 REFPROP_connector-0.3.9/REFPROPConnector/Handlers/__quality_iteration.py
+-rw-rw-rw-   0        0        0     1165 2024-02-06 08:36:24.000000 REFPROP_connector-0.3.9/REFPROPConnector/Handlers/__variable.py
+-rw-rw-rw-   0        0        0     1873 2024-05-07 08:22:41.000000 REFPROP_connector-0.3.9/REFPROPConnector/Handlers/coolprop_handler.py
+-rw-rw-rw-   0        0        0     2314 2024-05-07 08:22:41.000000 REFPROP_connector-0.3.9/REFPROPConnector/Handlers/refprop_handler.py
+-rwxrwxrwx   0        0        0  5280688 2021-12-10 08:32:10.000000 REFPROP_connector-0.3.9/REFPROPConnector/NIST2310.EXE
+drwxrwxrwx   0        0        0        0 2024-05-07 08:33:04.126888 REFPROP_connector-0.3.9/REFPROPConnector/Support/
+-rw-rw-rw-   0        0        0        0 2022-02-03 11:33:25.000000 REFPROP_connector-0.3.9/REFPROPConnector/Support/__init__.py
+-rw-rw-rw-   0        0        0     2211 2023-12-13 16:56:24.000000 REFPROP_connector-0.3.9/REFPROPConnector/Support/constants.py
+-rw-rw-rw-   0        0        0    14753 2023-12-13 16:52:42.000000 REFPROP_connector-0.3.9/REFPROPConnector/Support/refprop_names_tree.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:33:04.130888 REFPROP_connector-0.3.9/REFPROPConnector/Support/resources/
+-rw-rw-rw-   0        0        0       30 2024-05-07 08:23:13.000000 REFPROP_connector-0.3.9/REFPROPConnector/Support/resources/REFPROP_exec.dat
+-rw-rw-rw-   0        0        0    28642 2023-09-30 19:06:42.000000 REFPROP_connector-0.3.9/REFPROPConnector/Support/resources/REFPROP_names.xml
+-rw-rw-rw-   0        0        0        0 2022-02-03 11:35:20.000000 REFPROP_connector-0.3.9/REFPROPConnector/Support/resources/__init__.py
+-rw-rw-rw-   0        0        0     3006 2023-09-30 19:04:14.000000 REFPROP_connector-0.3.9/REFPROPConnector/Support/resources/file_handler.py
+-rw-rw-rw-   0        0        0    28966 2023-09-30 19:06:26.000000 REFPROP_connector-0.3.9/REFPROPConnector/Support/resources/rp_names_file_generator.py
+-rw-rw-rw-   0        0        0      332 2024-02-06 08:37:39.000000 REFPROP_connector-0.3.9/REFPROPConnector/__init__.py
+-rw-rw-rw-   0        0        0    19872 2024-05-07 08:30:41.000000 REFPROP_connector-0.3.9/REFPROPConnector/refprop_calculator.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:33:04.111888 REFPROP_connector-0.3.9/REFPROPConnectorTest/
+-rw-rw-rw-   0        0        0        0 2021-12-10 10:12:18.000000 REFPROP_connector-0.3.9/REFPROPConnectorTest/__init__.py
+-rw-rw-rw-   0        0        0     3196 2024-02-06 23:00:01.000000 REFPROP_connector-0.3.9/REFPROPConnectorTest/test_dll_runtime.py
+-rw-rw-rw-   0        0        0     5929 2024-05-07 08:23:13.000000 REFPROP_connector-0.3.9/REFPROPConnectorTest/test_file.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:33:04.150889 REFPROP_connector-0.3.9/REFPROP_connector.egg-info/
+-rw-rw-rw-   0        0        0     8204 2024-05-07 08:33:03.000000 REFPROP_connector-0.3.9/REFPROP_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1296 2024-05-07 08:33:03.000000 REFPROP_connector-0.3.9/REFPROP_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 08:33:03.000000 REFPROP_connector-0.3.9/REFPROP_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-07 08:33:03.000000 REFPROP_connector-0.3.9/REFPROP_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-05-07 08:33:03.000000 REFPROP_connector-0.3.9/REFPROP_connector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      113 2024-02-05 07:39:25.000000 REFPROP_connector-0.3.9/requirements.txt
+-rw-rw-rw-   0        0        0       86 2024-05-07 08:33:04.155889 REFPROP_connector-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2268 2024-05-07 08:30:41.000000 REFPROP_connector-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:33:04.151889 REFPROP_connector-0.3.9/twine_upload/
+-rw-rw-rw-   0        0        0     1089 2022-06-21 16:26:22.000000 REFPROP_connector-0.3.9/twine_upload/pip_upload.py
```

### Comparing `REFPROP_connector-0.3.8/LICENSE` & `REFPROP_connector-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.8/PKG-INFO` & `REFPROP_connector-0.3.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: REFPROP_connector
-Version: 0.3.8
+Version: 0.3.9
 Summary: Tools for launching REFPROP calculation and retrieving results from python
 Home-page: https://www.dief.unifi.it/vp-177-serg-group-english-version.html
 Author: Pietro Ungar
 Author-email: pietro.ungar@unifi.it
 License: GNU GPLv3
-Download-URL: https://github.com/SERGGroup/REFPROPConnector/archive/refs/tags/0.3.8.tar.gz
+Download-URL: https://github.com/SERGGroup/REFPROPConnector/archive/refs/tags/0.3.9.tar.gz
 Project-URL: Source, https://github.com/SERGGroup/REFPROPConnector
 Project-URL: Tracker, https://github.com/SERGGroup/REFPROPConnector/issues
 Description: # REFPROP connector
         
         __REFPROP connector__ is a tools developed by the [SERG research group](https://www.dief.unifi.it/vp-177-serg-group-english-version.html) 
         of the [University of Florence](https://www.unifi.it/changelang-eng.html) for launching [REFPROP](https://www.nist.gov/srd/refprop) 
         calculation and retrieving results from python. 
@@ -69,28 +69,33 @@
         ### Abstract Class
         
         _AbstractThermodynamicPoint_ is a class that can be overwritten in order to perform some calculation once both 
         independent state variable have been set. It can be useful for example for the evaluation of the reynolds number 
         for a fluid flowing in a pipe.
         
         ```python
-        from REFPROPConnector import AbstractThermodynamicPoint, RefPropHandler
+        from REFPROPConnector import AbstractThermodynamicPoint, RefPropHandler, init_handler
         import numpy as np
         
         
         class TubeSection(AbstractThermodynamicPoint):
         
             def __init__(self, diam, flow_rate):
                 
                 self.diam = diam
                 self.area = np.pi * np.power(diam / 2, 2)
                 self.flow_rate = flow_rate
                 self.Re = 0.
                 
-                refprop = RefPropHandler(["air"], [1])
+                refprop = init_handler(
+        
+                    chosen_subclass=RefPropHandler,
+                    fluids=["air"], composition=[1]
+                    
+                )
         
                 super().__init__(refprop)
         
             def other_calculation(self):
                 
                 mu = self.get_variable("mu") / (10 ** 6)  # conversion uPa*s -> Pa*s
                 self.Re = self.flow_rate * self.diam / (self.area * mu)
@@ -130,14 +135,27 @@
         
         tp = ThermodynamicPoint(["water"], [1.], unit_system="MASS BASE SI")
         tp.list_properties()
         tp.list_unit_systems()
         ```
         Default unit system is __SI with C__
         
+        ### Metastable Calculation
+        
+        You can force the state to represent a metastable condition as follows:  
+        
+        ```python
+        from REFPROPConnector import ThermodynamicPoint
+        
+        tp = ThermodynamicPoint(["water"], [1.], unit_system="MASS BASE SI")
+        tp.metastability = "liq" # or "vap" for vapour metastable condition
+        ```
+        Acceptable keywords for metastability are ["liquid", "liq", "l", ">"] for the liquid metastable state, 
+        or ["vap", "vapour", "vapor", "v", "<"] for the vapour state (keywords **are not** case-sensitive).
+        
         ### Diagram Plotter
         The _DiagramPlotter_ class can be used to plot a specific state diagram that can be then used to describe state 
         transformations. The diagram can be personalized using the _DiagramPlotterOptions_ class. 
         The following is an example on how to use the class.
         
         
         ```python
```

### Comparing `REFPROP_connector-0.3.8/README.md` & `REFPROP_connector-0.3.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -58,28 +58,33 @@
 ### Abstract Class
 
 _AbstractThermodynamicPoint_ is a class that can be overwritten in order to perform some calculation once both 
 independent state variable have been set. It can be useful for example for the evaluation of the reynolds number 
 for a fluid flowing in a pipe.
 
 ```python
-from REFPROPConnector import AbstractThermodynamicPoint, RefPropHandler
+from REFPROPConnector import AbstractThermodynamicPoint, RefPropHandler, init_handler
 import numpy as np
 
 
 class TubeSection(AbstractThermodynamicPoint):
 
     def __init__(self, diam, flow_rate):
         
         self.diam = diam
         self.area = np.pi * np.power(diam / 2, 2)
         self.flow_rate = flow_rate
         self.Re = 0.
         
-        refprop = RefPropHandler(["air"], [1])
+        refprop = init_handler(
+
+            chosen_subclass=RefPropHandler,
+            fluids=["air"], composition=[1]
+            
+        )
 
         super().__init__(refprop)
 
     def other_calculation(self):
         
         mu = self.get_variable("mu") / (10 ** 6)  # conversion uPa*s -> Pa*s
         self.Re = self.flow_rate * self.diam / (self.area * mu)
@@ -119,14 +124,27 @@
 
 tp = ThermodynamicPoint(["water"], [1.], unit_system="MASS BASE SI")
 tp.list_properties()
 tp.list_unit_systems()
 ```
 Default unit system is __SI with C__
 
+### Metastable Calculation
+
+You can force the state to represent a metastable condition as follows:  
+
+```python
+from REFPROPConnector import ThermodynamicPoint
+
+tp = ThermodynamicPoint(["water"], [1.], unit_system="MASS BASE SI")
+tp.metastability = "liq" # or "vap" for vapour metastable condition
+```
+Acceptable keywords for metastability are ["liquid", "liq", "l", ">"] for the liquid metastable state, 
+or ["vap", "vapour", "vapor", "v", "<"] for the vapour state (keywords **are not** case-sensitive).
+
 ### Diagram Plotter
 The _DiagramPlotter_ class can be used to plot a specific state diagram that can be then used to describe state 
 transformations. The diagram can be personalized using the _DiagramPlotterOptions_ class. 
 The following is an example on how to use the class.
 
 
 ```python
```

### Comparing `REFPROP_connector-0.3.8/REFPROPConnector/NIST2310.EXE` & `REFPROP_connector-0.3.9/REFPROPConnector/NIST2310.EXE`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.8/REFPROPConnector/Support/constants.py` & `REFPROP_connector-0.3.9/REFPROPConnector/Support/constants.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.8/REFPROPConnector/Support/refprop_names_tree.py` & `REFPROP_connector-0.3.9/REFPROPConnector/Support/refprop_names_tree.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.8/REFPROPConnector/Support/resources/REFPROP_names.xml` & `REFPROP_connector-0.3.9/REFPROPConnector/Support/resources/REFPROP_names.xml`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.8/REFPROPConnector/Support/resources/file_handler.py` & `REFPROP_connector-0.3.9/REFPROPConnector/Support/resources/file_handler.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.8/REFPROPConnector/Support/resources/rp_names_file_generator.py` & `REFPROP_connector-0.3.9/REFPROPConnector/Support/resources/rp_names_file_generator.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.8/REFPROPConnector/Tools/refprop_plotter.py` & `REFPROP_connector-0.3.9/REFPROPConnector/Handlers/Tools/refprop_plotter.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.8/REFPROPConnector/Tools/units_converter.py` & `REFPROP_connector-0.3.9/REFPROPConnector/Handlers/Tools/units_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 
     else:
 
         return None, conversion_info
 
     return result, conversion_info
 
+
 def __conversion_multiply(value, conversion_info, from_unit, to_unit):
 
     multiplier = conversion_info.conversion_dict[from_unit]["mult"]
     tmp_value = value * multiplier
 
     multiplier = conversion_info.conversion_dict[to_unit]["mult"]
     return tmp_value / multiplier
 
+
 def __conversion_sum_mult(value, conversion_info, from_unit, to_unit):
 
     mult = conversion_info.conversion_dict[from_unit]["mult"]
     sum = conversion_info.conversion_dict[from_unit]["sum"]
     tmp_value = (value + sum) * mult
 
     mult = conversion_info.conversion_dict[to_unit]["mult"]
```

### Comparing `REFPROP_connector-0.3.8/REFPROPConnectorTest/test_file.py` & `REFPROP_connector-0.3.9/REFPROPConnectorTest/test_file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from REFPROPConnector import ThermodynamicPoint, DiagramPlotter, DiagramPlotterOptions
-from REFPROPConnector.Tools.units_converter import convert_variable
+from REFPROPConnector.Handlers.Tools.units_converter import convert_variable
 from REFPROPConnector.Support.constants import get_refprop_name
 from matplotlib import pyplot as plt
 import unittest
 
 
 class TestREFPROPConnector(unittest.TestCase):
 
@@ -108,15 +108,15 @@
         T_ref = 10
         tp_ref = tp.duplicate()
         tp_ref.set_variable("T", T_ref)
         tp_ref.set_variable("P", 0.101325)
 
         tp.reference_state = tp_ref
 
-        self.assertEqual(tp.reference_state.get_variable("T"), T_ref + 273.15)
+        self.assertEqual(tp.reference_state.get_variable("T"), T_ref)
 
     def test_QH_flash(self):
 
         tp = ThermodynamicPoint(["water"], [1])
 
         tp.set_variable("T", 150)
         tp.set_variable("Q", 0)
@@ -173,10 +173,47 @@
         plotter.calculate()
 
         fig, (ax_1) = plt.subplots(1, 1, dpi=200)
         fig.set_size_inches(10, 5)
         plotter.plot(ax_1)
         plt.show()
 
+    def test_equals(self):
+
+        tp = ThermodynamicPoint(["Carbon Dioxide"], [1])
+        tp.set_variable("T", 100)
+        tp.set_variable("P", 0.1)
+
+        tp_new = tp.get_alternative_unit_system("MASS BASE SI")
+        equals = (tp == tp_new)
+
+        self.assertEqual(True, equals)
+
+    def test_metastability(self):
+
+        tp = ThermodynamicPoint(["Carbon Dioxide"], [1])
+
+        t_in = 10
+        tp.set_variable("T", t_in)
+        tp.set_variable("Q", 0)
+        rho_liq = tp.get_variable("rho")
+
+        tp.set_variable("T", t_in)
+        tp.set_variable("Q", 1)
+        rho_vap = tp.get_variable("rho")
+
+        tp_metastb = tp.duplicate()
+        tp_metastb.metastability = "liquid"
+        tp_metastb.set_variable("rho", rho_liq * 0.98 + rho_vap * 0.02)
+        tp_metastb.set_variable("T", t_in)
+
+        tp.set_variable("rho", rho_liq * 0.98 + rho_vap * 0.02)
+        tp.set_variable("T", t_in)
+        print(tp.get_variable("P"))
+        print(tp_metastb.get_variable("P"))
+
+        self.assertTrue(tp.get_variable("P") > tp_metastb.get_variable("P"))
+
 
 if __name__ == '__main__':
+
     unittest.main()
```

### Comparing `REFPROP_connector-0.3.8/REFPROP_connector.egg-info/PKG-INFO` & `REFPROP_connector-0.3.9/REFPROP_connector.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: REFPROP-connector
-Version: 0.3.8
+Version: 0.3.9
 Summary: Tools for launching REFPROP calculation and retrieving results from python
 Home-page: https://www.dief.unifi.it/vp-177-serg-group-english-version.html
 Author: Pietro Ungar
 Author-email: pietro.ungar@unifi.it
 License: GNU GPLv3
-Download-URL: https://github.com/SERGGroup/REFPROPConnector/archive/refs/tags/0.3.8.tar.gz
+Download-URL: https://github.com/SERGGroup/REFPROPConnector/archive/refs/tags/0.3.9.tar.gz
 Project-URL: Source, https://github.com/SERGGroup/REFPROPConnector
 Project-URL: Tracker, https://github.com/SERGGroup/REFPROPConnector/issues
 Description: # REFPROP connector
         
         __REFPROP connector__ is a tools developed by the [SERG research group](https://www.dief.unifi.it/vp-177-serg-group-english-version.html) 
         of the [University of Florence](https://www.unifi.it/changelang-eng.html) for launching [REFPROP](https://www.nist.gov/srd/refprop) 
         calculation and retrieving results from python. 
@@ -69,28 +69,33 @@
         ### Abstract Class
         
         _AbstractThermodynamicPoint_ is a class that can be overwritten in order to perform some calculation once both 
         independent state variable have been set. It can be useful for example for the evaluation of the reynolds number 
         for a fluid flowing in a pipe.
         
         ```python
-        from REFPROPConnector import AbstractThermodynamicPoint, RefPropHandler
+        from REFPROPConnector import AbstractThermodynamicPoint, RefPropHandler, init_handler
         import numpy as np
         
         
         class TubeSection(AbstractThermodynamicPoint):
         
             def __init__(self, diam, flow_rate):
                 
                 self.diam = diam
                 self.area = np.pi * np.power(diam / 2, 2)
                 self.flow_rate = flow_rate
                 self.Re = 0.
                 
-                refprop = RefPropHandler(["air"], [1])
+                refprop = init_handler(
+        
+                    chosen_subclass=RefPropHandler,
+                    fluids=["air"], composition=[1]
+                    
+                )
         
                 super().__init__(refprop)
         
             def other_calculation(self):
                 
                 mu = self.get_variable("mu") / (10 ** 6)  # conversion uPa*s -> Pa*s
                 self.Re = self.flow_rate * self.diam / (self.area * mu)
@@ -130,14 +135,27 @@
         
         tp = ThermodynamicPoint(["water"], [1.], unit_system="MASS BASE SI")
         tp.list_properties()
         tp.list_unit_systems()
         ```
         Default unit system is __SI with C__
         
+        ### Metastable Calculation
+        
+        You can force the state to represent a metastable condition as follows:  
+        
+        ```python
+        from REFPROPConnector import ThermodynamicPoint
+        
+        tp = ThermodynamicPoint(["water"], [1.], unit_system="MASS BASE SI")
+        tp.metastability = "liq" # or "vap" for vapour metastable condition
+        ```
+        Acceptable keywords for metastability are ["liquid", "liq", "l", ">"] for the liquid metastable state, 
+        or ["vap", "vapour", "vapor", "v", "<"] for the vapour state (keywords **are not** case-sensitive).
+        
         ### Diagram Plotter
         The _DiagramPlotter_ class can be used to plot a specific state diagram that can be then used to describe state 
         transformations. The diagram can be personalized using the _DiagramPlotterOptions_ class. 
         The following is an example on how to use the class.
         
         
         ```python
```

### Comparing `REFPROP_connector-0.3.8/REFPROP_connector.egg-info/SOURCES.txt` & `REFPROP_connector-0.3.9/REFPROP_connector.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,32 @@
 requirements.txt
 setup.cfg
 setup.py
 REFPROPConnector/NIST2310.EXE
 REFPROPConnector/__init__.py
 REFPROPConnector/refprop_calculator.py
 REFPROPConnectorTest/__init__.py
+REFPROPConnectorTest/test_dll_runtime.py
 REFPROPConnectorTest/test_file.py
+REFPROPConnector/Handlers/__base_handler.py
+REFPROPConnector/Handlers/__init__.py
+REFPROPConnector/Handlers/__quality_iteration.py
+REFPROPConnector/Handlers/__variable.py
+REFPROPConnector/Handlers/coolprop_handler.py
+REFPROPConnector/Handlers/refprop_handler.py
+REFPROPConnector/Handlers/Tools/__init__.py
+REFPROPConnector/Handlers/Tools/refprop_plotter.py
+REFPROPConnector/Handlers/Tools/units_converter.py
 REFPROPConnector/Support/__init__.py
 REFPROPConnector/Support/constants.py
 REFPROPConnector/Support/refprop_names_tree.py
 REFPROPConnector/Support/resources/REFPROP_exec.dat
 REFPROPConnector/Support/resources/REFPROP_names.xml
 REFPROPConnector/Support/resources/__init__.py
 REFPROPConnector/Support/resources/file_handler.py
 REFPROPConnector/Support/resources/rp_names_file_generator.py
-REFPROPConnector/Tools/__init__.py
-REFPROPConnector/Tools/refprop_plotter.py
-REFPROPConnector/Tools/units_converter.py
 REFPROP_connector.egg-info/PKG-INFO
 REFPROP_connector.egg-info/SOURCES.txt
 REFPROP_connector.egg-info/dependency_links.txt
 REFPROP_connector.egg-info/requires.txt
 REFPROP_connector.egg-info/top_level.txt
 twine_upload/pip_upload.py
```

### Comparing `REFPROP_connector-0.3.8/setup.py` & `REFPROP_connector-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from os import path, listdir
 import setuptools
 
-VERSION = "0.3.8"
+VERSION = "0.3.9"
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
 
     long_description = f.read()
```

### Comparing `REFPROP_connector-0.3.8/twine_upload/pip_upload.py` & `REFPROP_connector-0.3.9/twine_upload/pip_upload.py`

 * *Files identical despite different names*

