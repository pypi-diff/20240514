# Comparing `tmp/pywayne-1.0.0.7.0.tar.gz` & `tmp/pywayne-1.0.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywayne-1.0.0.7.0.tar", last modified: Thu Apr 18 13:58:31 2024, max compression
+gzip compressed data, was "pywayne-1.0.0.7.1.tar", last modified: Tue May 14 06:56:28 2024, max compression
```

## Comparing `pywayne-1.0.0.7.0.tar` & `pywayne-1.0.0.7.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:58:31.971439 pywayne-1.0.0.7.0/
--rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.0/LICENSE
--rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-04-18 13:58:31.971068 pywayne-1.0.0.7.0/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.0/README.md
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:58:31.964113 pywayne-1.0.0.7.0/bin/
--rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.7.0/bin/gettool
--rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.7.0/bin/gettool.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:58:31.966592 pywayne-1.0.0.7.0/pywayne/
--rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.0/pywayne/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)      242 2024-04-18 13:57:44.000000 pywayne-1.0.0.7.0/pywayne/__version__.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:58:31.967621 pywayne-1.0.0.7.0/pywayne/adb/
--rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.0/pywayne/adb/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.0/pywayne/adb/logcat_reader.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:58:31.968092 pywayne-1.0.0.7.0/pywayne/ahrs/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.0/pywayne/ahrs/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.0/pywayne/ahrs/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:58:31.968831 pywayne-1.0.0.7.0/pywayne/calibration/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.0/pywayne/calibration/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.7.0/pywayne/calibration/magnetometer_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.7.0/pywayne/calibration/temporal_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.0/pywayne/data_structure.py
--rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.7.0/pywayne/dsp.py
--rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.7.0/pywayne/gui.py
--rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.0/pywayne/math.py
--rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.0/pywayne/plot.py
--rw-r--r--   0 wayne      (503) staff       (20)    15758 2024-04-18 13:58:16.000000 pywayne-1.0.0.7.0/pywayne/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:58:31.969687 pywayne-1.0.0.7.0/pywayne/vio/
--rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.0/pywayne/vio/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.0/pywayne/vio/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:58:31.970219 pywayne-1.0.0.7.0/pywayne/visualization/
--rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.7.0/pywayne/visualization/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.7.0/pywayne/visualization/pangolin.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:58:31.970722 pywayne-1.0.0.7.0/pywayne.egg-info/
--rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-04-18 13:58:31.000000 pywayne-1.0.0.7.0/pywayne.egg-info/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      692 2024-04-18 13:58:31.000000 pywayne-1.0.0.7.0/pywayne.egg-info/SOURCES.txt
--rw-r--r--   0 wayne      (503) staff       (20)      184 2024-04-18 13:58:31.000000 pywayne-1.0.0.7.0/pywayne.egg-info/dependency_links.txt
--rw-r--r--   0 wayne      (503) staff       (20)      162 2024-04-18 13:58:31.000000 pywayne-1.0.0.7.0/pywayne.egg-info/requires.txt
--rw-r--r--   0 wayne      (503) staff       (20)        8 2024-04-18 13:58:31.000000 pywayne-1.0.0.7.0/pywayne.egg-info/top_level.txt
--rw-r--r--   0 wayne      (503) staff       (20)       38 2024-04-18 13:58:31.971492 pywayne-1.0.0.7.0/setup.cfg
--rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.7.0/setup.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 06:56:28.077300 pywayne-1.0.0.7.1/
+-rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.1/LICENSE
+-rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-05-14 06:56:28.076974 pywayne-1.0.0.7.1/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.1/README.md
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 06:56:28.069843 pywayne-1.0.0.7.1/bin/
+-rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.7.1/bin/gettool
+-rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.7.1/bin/gettool.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 06:56:28.072223 pywayne-1.0.0.7.1/pywayne/
+-rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.1/pywayne/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)      242 2024-05-14 06:46:35.000000 pywayne-1.0.0.7.1/pywayne/__version__.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 06:56:28.073344 pywayne-1.0.0.7.1/pywayne/adb/
+-rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.1/pywayne/adb/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.1/pywayne/adb/logcat_reader.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 06:56:28.073898 pywayne-1.0.0.7.1/pywayne/ahrs/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.1/pywayne/ahrs/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.1/pywayne/ahrs/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 06:56:28.075361 pywayne-1.0.0.7.1/pywayne/calibration/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.1/pywayne/calibration/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.7.1/pywayne/calibration/magnetometer_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.7.1/pywayne/calibration/temporal_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.1/pywayne/data_structure.py
+-rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.7.1/pywayne/dsp.py
+-rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.7.1/pywayne/gui.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.1/pywayne/math.py
+-rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.1/pywayne/plot.py
+-rw-r--r--   0 wayne      (503) staff       (20)    15318 2024-05-14 06:55:26.000000 pywayne-1.0.0.7.1/pywayne/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 06:56:28.075940 pywayne-1.0.0.7.1/pywayne/vio/
+-rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.1/pywayne/vio/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.1/pywayne/vio/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 06:56:28.076405 pywayne-1.0.0.7.1/pywayne/visualization/
+-rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.7.1/pywayne/visualization/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.7.1/pywayne/visualization/pangolin.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 06:56:28.076694 pywayne-1.0.0.7.1/pywayne.egg-info/
+-rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-05-14 06:56:27.000000 pywayne-1.0.0.7.1/pywayne.egg-info/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      692 2024-05-14 06:56:28.000000 pywayne-1.0.0.7.1/pywayne.egg-info/SOURCES.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      184 2024-05-14 06:56:27.000000 pywayne-1.0.0.7.1/pywayne.egg-info/dependency_links.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      162 2024-05-14 06:56:27.000000 pywayne-1.0.0.7.1/pywayne.egg-info/requires.txt
+-rw-r--r--   0 wayne      (503) staff       (20)        8 2024-05-14 06:56:27.000000 pywayne-1.0.0.7.1/pywayne.egg-info/top_level.txt
+-rw-r--r--   0 wayne      (503) staff       (20)       38 2024-05-14 06:56:28.077354 pywayne-1.0.0.7.1/setup.cfg
+-rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.7.1/setup.py
```

### Comparing `pywayne-1.0.0.7.0/LICENSE` & `pywayne-1.0.0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/PKG-INFO` & `pywayne-1.0.0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.7.0
+Version: 1.0.0.7.1
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.7.0/README.md` & `pywayne-1.0.0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/bin/gettool.py` & `pywayne-1.0.0.7.1/bin/gettool.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/pywayne/adb/logcat_reader.py` & `pywayne-1.0.0.7.1/pywayne/adb/logcat_reader.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/pywayne/ahrs/tools.py` & `pywayne-1.0.0.7.1/pywayne/ahrs/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/pywayne/calibration/magnetometer_calibration.py` & `pywayne-1.0.0.7.1/pywayne/calibration/magnetometer_calibration.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/pywayne/data_structure.py` & `pywayne-1.0.0.7.1/pywayne/data_structure.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/pywayne/dsp.py` & `pywayne-1.0.0.7.1/pywayne/dsp.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/pywayne/gui.py` & `pywayne-1.0.0.7.1/pywayne/gui.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/pywayne/math.py` & `pywayne-1.0.0.7.1/pywayne/math.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/pywayne/plot.py` & `pywayne-1.0.0.7.1/pywayne/plot.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/pywayne/tools.py` & `pywayne-1.0.0.7.1/pywayne/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -408,40 +408,28 @@
 
     if update and os.path.exists(config_yaml_file):
         existing_config = read_yaml_config(config_yaml_file)
     else:
         existing_config = {}
 
     with lock:
-        try:
-            if update:
-                config = deep_merge_dicts(existing_config, config)
-            with open(config_yaml_file, 'w', encoding='UTF-8') as f:
-                yaml.dump(config, f, default_flow_style=False)
-        except IOError as e:
-            print(f"Error writing to file {config_yaml_file}: {e}")
-        except yaml.YAMLError as e:
-            print(f"Error dumping config to YAML: {e}")
+        if update:
+            config = deep_merge_dicts(existing_config, config)
+        with open(config_yaml_file, 'w', encoding='UTF-8') as f:
+            yaml.dump(config, f, default_flow_style=False)
 
 
 def read_yaml_config(config_yaml_file: str):
     """
     Reads and returns the configuration from a YAML file with file lock protection.
 
     :param config_yaml_file: The path to the YAML file from which to read the config.
     :return: A dictionary containing the configuration settings.
     """
 
     lock_file = config_yaml_file + ".lock"
     lock = FileLock(lock_file)
 
     with lock:
-        try:
-            with open(config_yaml_file, 'r', encoding='UTF-8') as f:
-                data = yaml.safe_load(f)
-            return data
-        except IOError as e:
-            print(f"Error reading file {config_yaml_file}: {e}")
-            return {}
-        except yaml.YAMLError as e:
-            print(f"Error parsing YAML file: {e}")
-            return {}
+        with open(config_yaml_file, 'r', encoding='UTF-8') as f:
+            data = yaml.safe_load(f)
+        return data if data is not None else {}
```

### Comparing `pywayne-1.0.0.7.0/pywayne/vio/tools.py` & `pywayne-1.0.0.7.1/pywayne/vio/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/pywayne/visualization/pangolin.py` & `pywayne-1.0.0.7.1/pywayne/visualization/pangolin.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/pywayne.egg-info/PKG-INFO` & `pywayne-1.0.0.7.1/pywayne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.7.0
+Version: 1.0.0.7.1
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.7.0/pywayne.egg-info/SOURCES.txt` & `pywayne-1.0.0.7.1/pywayne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.0/setup.py` & `pywayne-1.0.0.7.1/setup.py`

 * *Files identical despite different names*

