# Comparing `tmp/linien-server-2.0.0rc3.tar.gz` & `tmp/linien_server-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-server-2.0.0rc3.tar", last modified: Fri Apr  5 14:09:00 2024, max compression
+gzip compressed data, was "linien_server-2.0.1.tar", last modified: Mon May 13 15:18:02 2024, max compression
```

## Comparing `linien-server-2.0.0rc3.tar` & `linien_server-2.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:09:00.482061 linien-server-2.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-05 14:09:00.478062 linien-server-2.0.0rc3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:09:00.478062 linien-server-2.0.0rc3/linien_server/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/acquisition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:09:00.478062 linien-server-2.0.0rc3/linien_server/autolock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/autolock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/autolock/algorithm_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/autolock/autolock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/autolock/robust.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/autolock/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/autolock/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/csr.py
--rw-r--r--   0 runner    (1001) docker     (127)    15789 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/csrmap.py
--rw-r--r--   0 runner    (1001) docker     (127)  2083740 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/gateware.bin
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/iir_coeffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/linien-server.service
--rwxr-xr-x   0 runner    (1001) docker     (127)     8368 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/mdio-tool
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/mdio_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/noise_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:09:00.478062 linien-server-2.0.0rc3/linien_server/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/optimization/approach_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/optimization/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/optimization/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/optimization/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29168 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/registers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15684 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/linien_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:09:00.478062 linien-server-2.0.0rc3/linien_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-05 14:09:00.000000 linien-server-2.0.0rc3/linien_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-05 14:09:00.000000 linien-server-2.0.0rc3/linien_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:09:00.000000 linien-server-2.0.0rc3/linien_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-05 14:09:00.000000 linien-server-2.0.0rc3/linien_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-05 14:09:00.000000 linien-server-2.0.0rc3/linien_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 14:09:00.000000 linien-server-2.0.0rc3/linien_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-05 14:08:46.000000 linien-server-2.0.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:09:00.482061 linien-server-2.0.0rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:18:02.605410 linien_server-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-13 15:18:02.605410 linien_server-2.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:18:02.601410 linien_server-2.0.1/linien_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/acquisition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:18:02.605410 linien_server-2.0.1/linien_server/autolock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/autolock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/autolock/algorithm_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/autolock/autolock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/autolock/robust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/autolock/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/autolock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/csr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15789 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/csrmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2083740 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/gateware.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/iir_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/linien-server.service
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8368 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/mdio-tool
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/mdio_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/noise_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:18:02.605410 linien_server-2.0.1/linien_server/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/optimization/approach_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/optimization/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/optimization/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/optimization/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29168 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15684 2024-05-13 15:17:51.000000 linien_server-2.0.1/linien_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:18:02.605410 linien_server-2.0.1/linien_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-13 15:18:02.000000 linien_server-2.0.1/linien_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-13 15:18:02.000000 linien_server-2.0.1/linien_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:18:02.000000 linien_server-2.0.1/linien_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-13 15:18:02.000000 linien_server-2.0.1/linien_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 15:18:02.000000 linien_server-2.0.1/linien_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 15:18:02.000000 linien_server-2.0.1/linien_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-13 15:17:51.000000 linien_server-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:18:02.605410 linien_server-2.0.1/setup.cfg
```

### Comparing `linien-server-2.0.0rc3/PKG-INFO` & `linien_server-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: linien-server
-Version: 2.0.0rc3
+Version: 2.0.1
 Summary: Server components of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: cma<4.0,>=3.0.3
 Requires-Dist: fire>=0.6.0
 Requires-Dist: influxdb-client[ciso]<2.0,>=1.9
 Requires-Dist: pylpsd>=0.1.4
 Requires-Dist: pyrp3<3.0,>=2.0.1; platform_machine == "armv7l"
-Requires-Dist: linien-common==2.0.0rc3
+Requires-Dist: linien-common==2.0.1
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

### Comparing `linien-server-2.0.0rc3/linien_server/__init__.py` & `linien_server-2.0.1/linien_server/__init__.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/acquisition.py` & `linien_server-2.0.1/linien_server/acquisition.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/autolock/algorithm_selection.py` & `linien_server-2.0.1/linien_server/autolock/algorithm_selection.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/autolock/autolock.py` & `linien_server-2.0.1/linien_server/autolock/autolock.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/autolock/robust.py` & `linien_server-2.0.1/linien_server/autolock/robust.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/autolock/simple.py` & `linien_server-2.0.1/linien_server/autolock/simple.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/autolock/utils.py` & `linien_server-2.0.1/linien_server/autolock/utils.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/cli.py` & `linien_server-2.0.1/linien_server/cli.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/csr.py` & `linien_server-2.0.1/linien_server/csr.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/csrmap.py` & `linien_server-2.0.1/linien_server/csrmap.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/gateware.bin` & `linien_server-2.0.1/linien_server/gateware.bin`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/iir_coeffs.py` & `linien_server-2.0.1/linien_server/iir_coeffs.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/influxdb.py` & `linien_server-2.0.1/linien_server/influxdb.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/mdio-tool` & `linien_server-2.0.1/linien_server/mdio-tool`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/mdio_tool.py` & `linien_server-2.0.1/linien_server/mdio_tool.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/noise_analysis.py` & `linien_server-2.0.1/linien_server/noise_analysis.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/optimization/approach_line.py` & `linien_server-2.0.1/linien_server/optimization/approach_line.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/optimization/engine.py` & `linien_server-2.0.1/linien_server/optimization/engine.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/optimization/general.py` & `linien_server-2.0.1/linien_server/optimization/general.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/optimization/optimization.py` & `linien_server-2.0.1/linien_server/optimization/optimization.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/optimization/utils.py` & `linien_server-2.0.1/linien_server/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/parameters.py` & `linien_server-2.0.1/linien_server/parameters.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server/registers.py` & `linien_server-2.0.1/linien_server/registers.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             logic_slow_decimation=16,
         )
 
         for instruction_idx, [wait_for, peak_height] in enumerate(
             self.parameters.autolock_instructions.value
         ):
             new[f"logic_autolock_robust_peak_height_{instruction_idx}"] = peak_height
-            new["logic_autolock_robust_wait_for_{instruction_idx}"] = wait_for
+            new[f"logic_autolock_robust_wait_for_{instruction_idx}"] = wait_for
 
         if self.parameters.lock.value:
             # display combined error signal and control signal
             new.update(
                 {
                     "scopegen_adc_a_sel": csrmap.signals.index(
                         "logic_combined_error_signal"
```

### Comparing `linien-server-2.0.0rc3/linien_server/server.py` & `linien_server-2.0.1/linien_server/server.py`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/linien_server.egg-info/PKG-INFO` & `linien_server-2.0.1/linien_server.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: linien-server
-Version: 2.0.0rc3
+Version: 2.0.1
 Summary: Server components of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: cma<4.0,>=3.0.3
 Requires-Dist: fire>=0.6.0
 Requires-Dist: influxdb-client[ciso]<2.0,>=1.9
 Requires-Dist: pylpsd>=0.1.4
 Requires-Dist: pyrp3<3.0,>=2.0.1; platform_machine == "armv7l"
-Requires-Dist: linien-common==2.0.0rc3
+Requires-Dist: linien-common==2.0.1
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

### Comparing `linien-server-2.0.0rc3/linien_server.egg-info/SOURCES.txt` & `linien_server-2.0.1/linien_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linien-server-2.0.0rc3/pyproject.toml` & `linien_server-2.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linien-server"
-version = "2.0.0rc3"
+version = "2.0.1"
 authors = [
     { name = "Benjamin Wiegand", email = "benjamin.wiegand@physik.hu-berlin.de" },
     { name = "Bastian Leykauf", email = "leykauf@physik.hu-berlin.de" },
     { name = "Robert Jördens", email = "rj@quartiq.de" },
     { name = "Christian Freier", email = "christian.freier@gmail.com" },
     { name = "Doron Behar", email = "doron.behar@gmail.com" },
 ]
@@ -24,15 +24,15 @@
 requires-python = ">=3.10"
 dependencies = [
     "cma>=3.0.3,<4.0",
     "fire>=0.6.0",
     "influxdb-client[ciso]>=1.9,<2.0",
     "pylpsd>=0.1.4",
     "pyrp3>=2.0.1,<3.0;platform_machine=='armv7l'",
-    "linien-common==2.0.0rc3",
+    "linien-common==2.0.1",
 ]
 
 [project.readme]
 text = "Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions."
 content-type = "text/markdown"
 
 [project.urls]
```
