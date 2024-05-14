# Comparing `tmp/cancer_simulation-0.7.3.tar.gz` & `tmp/cancer_simulation-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cancer_simulation-0.7.3.tar", last modified: Tue May 14 04:17:51 2024, max compression
+gzip compressed data, was "cancer_simulation-0.7.4.tar", last modified: Tue May 14 05:30:21 2024, max compression
```

## Comparing `cancer_simulation-0.7.3.tar` & `cancer_simulation-0.7.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-14 04:17:51.428361 cancer_simulation-0.7.3/
--rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      599 2024-05-14 04:17:51.428361 cancer_simulation-0.7.3/PKG-INFO
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)    11757 2024-05-14 04:13:21.000000 cancer_simulation-0.7.3/README.md
-drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-14 04:17:51.424361 cancer_simulation-0.7.3/cancer_simulation.egg-info/
--rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      599 2024-05-14 04:17:51.000000 cancer_simulation-0.7.3/cancer_simulation.egg-info/PKG-INFO
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      390 2024-05-14 04:17:51.000000 cancer_simulation-0.7.3/cancer_simulation.egg-info/SOURCES.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        1 2024-05-14 04:17:51.000000 cancer_simulation-0.7.3/cancer_simulation.egg-info/dependency_links.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       34 2024-05-14 04:17:51.000000 cancer_simulation-0.7.3/cancer_simulation.egg-info/entry_points.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       62 2024-05-14 04:17:51.000000 cancer_simulation-0.7.3/cancer_simulation.egg-info/requires.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        4 2024-05-14 04:17:51.000000 cancer_simulation-0.7.3/cancer_simulation.egg-info/top_level.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       38 2024-05-14 04:17:51.428361 cancer_simulation-0.7.3/setup.cfg
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      822 2024-05-14 04:17:44.000000 cancer_simulation-0.7.3/setup.py
-drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-14 04:17:51.424361 cancer_simulation-0.7.3/src/
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       30 2024-05-12 18:56:52.000000 cancer_simulation-0.7.3/src/__init__.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     3168 2024-05-13 20:56:21.000000 cancer_simulation-0.7.3/src/automaton.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     1625 2024-05-12 17:43:44.000000 cancer_simulation-0.7.3/src/cell.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      274 2024-05-14 04:13:21.000000 cancer_simulation-0.7.3/src/constants.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)    12399 2024-05-13 13:03:22.000000 cancer_simulation-0.7.3/src/csimulation.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     8368 2024-05-13 20:53:28.000000 cancer_simulation-0.7.3/src/entity.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2924 2024-05-12 19:00:03.000000 cancer_simulation-0.7.3/src/grid.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     5155 2024-05-14 04:14:52.000000 cancer_simulation-0.7.3/src/variables.py
+drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-14 05:30:21.269339 cancer_simulation-0.7.4/
+-rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      599 2024-05-14 05:30:21.269339 cancer_simulation-0.7.4/PKG-INFO
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)    11757 2024-05-14 04:13:21.000000 cancer_simulation-0.7.4/README.md
+drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-14 05:30:21.269339 cancer_simulation-0.7.4/cancer_simulation.egg-info/
+-rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      599 2024-05-14 05:30:21.000000 cancer_simulation-0.7.4/cancer_simulation.egg-info/PKG-INFO
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      390 2024-05-14 05:30:21.000000 cancer_simulation-0.7.4/cancer_simulation.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        1 2024-05-14 05:30:21.000000 cancer_simulation-0.7.4/cancer_simulation.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       34 2024-05-14 05:30:21.000000 cancer_simulation-0.7.4/cancer_simulation.egg-info/entry_points.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       62 2024-05-14 05:30:21.000000 cancer_simulation-0.7.4/cancer_simulation.egg-info/requires.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        4 2024-05-14 05:30:21.000000 cancer_simulation-0.7.4/cancer_simulation.egg-info/top_level.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       38 2024-05-14 05:30:21.269339 cancer_simulation-0.7.4/setup.cfg
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      822 2024-05-14 05:30:07.000000 cancer_simulation-0.7.4/setup.py
+drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-14 05:30:21.269339 cancer_simulation-0.7.4/src/
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       30 2024-05-12 18:56:52.000000 cancer_simulation-0.7.4/src/__init__.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     3168 2024-05-14 05:20:47.000000 cancer_simulation-0.7.4/src/automaton.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     1625 2024-05-12 17:43:44.000000 cancer_simulation-0.7.4/src/cell.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      274 2024-05-14 04:13:21.000000 cancer_simulation-0.7.4/src/constants.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)    12399 2024-05-13 13:03:22.000000 cancer_simulation-0.7.4/src/csimulation.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     8368 2024-05-14 05:19:28.000000 cancer_simulation-0.7.4/src/entity.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2924 2024-05-12 19:00:03.000000 cancer_simulation-0.7.4/src/grid.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     5152 2024-05-14 05:22:27.000000 cancer_simulation-0.7.4/src/variables.py
```

### Comparing `cancer_simulation-0.7.3/PKG-INFO` & `cancer_simulation-0.7.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cancer_simulation
-Version: 0.7.3
+Version: 0.7.4
 Summary: A simple cancer and chemotherapy simulation
 Home-page: https://github.com/Zhukowych/CancerSimulation
 Requires-Dist: pygame==2.5.2
 Requires-Dist: pygame-chart==1.0.0
 Requires-Dist: numpy==1.26.3
 Requires-Dist: PyYAML==6.0.1
```

### Comparing `cancer_simulation-0.7.3/README.md` & `cancer_simulation-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.3/cancer_simulation.egg-info/PKG-INFO` & `cancer_simulation-0.7.4/cancer_simulation.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cancer_simulation
-Version: 0.7.3
+Version: 0.7.4
 Summary: A simple cancer and chemotherapy simulation
 Home-page: https://github.com/Zhukowych/CancerSimulation
 Requires-Dist: pygame==2.5.2
 Requires-Dist: pygame-chart==1.0.0
 Requires-Dist: numpy==1.26.3
 Requires-Dist: PyYAML==6.0.1
```

### Comparing `cancer_simulation-0.7.3/setup.py` & `cancer_simulation-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cancer_simulation",
-    version='0.7.3',
+    version='0.7.4',
     packages=find_packages(),
     description="A simple cancer and chemotherapy simulation",
     long_description="""We implemented cancer development and chemotherapy impact simulation using
                    stochastic cellular automaton with Python. The main feature of implemented 
                    app is capability of simulating different treatment strategies under same-
                    type cancer behavior.""",
     url = "https://github.com/Zhukowych/CancerSimulation",
```

### Comparing `cancer_simulation-0.7.3/src/automaton.py` & `cancer_simulation-0.7.4/src/automaton.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -77,17 +77,17 @@
 
             entity.cell = None
             entity.neighbors = None
             entity.free_neighbors = None
 
         self.edge_cells = edge_cells
 
-        self.variables.time_step()
         self.process_chemotherapy()
         self.spawn_immune_cells()
+        self.variables.time_step()
 
     def process_chemotherapy(self):
         """Process effect of chemotherapy on cell"""
         if self.variables.is_injection_start:
             self.variables.injection_number += 1
 
     def spawn_immune_cells(self):
```

### Comparing `cancer_simulation-0.7.3/src/cell.py` & `cancer_simulation-0.7.4/src/cell.py`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.3/src/csimulation.py` & `cancer_simulation-0.7.4/src/csimulation.py`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.3/src/entity.py` & `cancer_simulation-0.7.4/src/entity.py`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.3/src/grid.py` & `cancer_simulation-0.7.4/src/grid.py`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.3/src/variables.py` & `cancer_simulation-0.7.4/src/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,33 +105,30 @@
             return False
 
         return True
 
     @property
     def is_injection_start(self) -> bool:
         """Return true if it is a day of injection"""
-
         if not self.is_treatment:
             return False
 
         days_from_start = self.days_elapsed - self.treatment_start_time
-
         if days_from_start % self.injection_interval == 0 and self.time % 24 == 0:
             return True
         return False
 
     @property
     def days_from_injection(self) -> int:
         """Return number of days from last injection""" 
         if self.is_injection_start:
             return 0
         return self.days_elapsed - self.treatment_start_time - (self.injection_number - 1) * self.injection_interval
 
 
-
 class ConfigFileException(Exception):
     """Exception for incorrect config file"""
 
 
 def read_variables(filepath: str) -> list[Variables]:
     """
     Read configuration file and return list of Variables for
```

