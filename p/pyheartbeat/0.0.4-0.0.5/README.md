# Comparing `tmp/pyheartbeat-0.0.4.tar.gz` & `tmp/pyheartbeat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyheartbeat-0.0.4.tar", last modified: Tue May 14 13:51:45 2024, max compression
+gzip compressed data, was "pyheartbeat-0.0.5.tar", last modified: Tue May 14 14:15:06 2024, max compression
```

## Comparing `pyheartbeat-0.0.4.tar` & `pyheartbeat-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 13:51:45.959200 pyheartbeat-0.0.4/
--rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 pyheartbeat-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2085 2024-05-14 13:51:45.956189 pyheartbeat-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1249 2024-05-14 13:51:14.000000 pyheartbeat-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 13:51:45.949931 pyheartbeat-0.0.4/pyheartbeat/
--rw-rw-rw-   0        0        0       69 2024-05-07 13:50:50.000000 pyheartbeat-0.0.4/pyheartbeat/__init__.py
--rw-rw-rw-   0        0        0     4520 2024-05-14 13:41:56.000000 pyheartbeat-0.0.4/pyheartbeat/heartbeat_library.py
-drwxrwxrwx   0        0        0        0 2024-05-14 13:51:45.954929 pyheartbeat-0.0.4/pyheartbeat.egg-info/
--rw-rw-rw-   0        0        0     2085 2024-05-14 13:51:45.000000 pyheartbeat-0.0.4/pyheartbeat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-14 13:51:45.000000 pyheartbeat-0.0.4/pyheartbeat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 13:51:45.000000 pyheartbeat-0.0.4/pyheartbeat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-14 13:51:45.000000 pyheartbeat-0.0.4/pyheartbeat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-14 13:51:45.000000 pyheartbeat-0.0.4/pyheartbeat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 13:51:45.960203 pyheartbeat-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1065 2024-05-14 13:50:59.000000 pyheartbeat-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:15:06.551667 pyheartbeat-0.0.5/
+-rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 pyheartbeat-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2085 2024-05-14 14:15:06.548655 pyheartbeat-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1249 2024-05-14 13:51:14.000000 pyheartbeat-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 14:15:06.533561 pyheartbeat-0.0.5/pyheartbeat/
+-rw-rw-rw-   0        0        0       69 2024-05-07 13:50:50.000000 pyheartbeat-0.0.5/pyheartbeat/__init__.py
+-rw-rw-rw-   0        0        0     4441 2024-05-14 14:14:51.000000 pyheartbeat-0.0.5/pyheartbeat/heartbeat_library.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:15:06.547659 pyheartbeat-0.0.5/pyheartbeat.egg-info/
+-rw-rw-rw-   0        0        0     2085 2024-05-14 14:15:06.000000 pyheartbeat-0.0.5/pyheartbeat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-14 14:15:06.000000 pyheartbeat-0.0.5/pyheartbeat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 14:15:06.000000 pyheartbeat-0.0.5/pyheartbeat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-14 14:15:06.000000 pyheartbeat-0.0.5/pyheartbeat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-14 14:15:06.000000 pyheartbeat-0.0.5/pyheartbeat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 14:15:06.552654 pyheartbeat-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1065 2024-05-14 14:15:01.000000 pyheartbeat-0.0.5/setup.py
```

### Comparing `pyheartbeat-0.0.4/LICENSE` & `pyheartbeat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyheartbeat-0.0.4/PKG-INFO` & `pyheartbeat-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyheartbeat
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: pyheartbeat,heartbeat_library,heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyheartbeat-0.0.4/README.md` & `pyheartbeat-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyheartbeat-0.0.4/pyheartbeat/heartbeat_library.py` & `pyheartbeat-0.0.5/pyheartbeat/heartbeat_library.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,17 +87,14 @@
 
         # If the variable_parameter is False, break the loop
         for _ in range(interval):
             if not variable_parameter:
                 break # break the loop
             time.sleep(1)
 
-    if show_logs:
-        print('>>> Heartbeat thread has ended. <<<')
-
 
 # 3
 def heartbeat(interval = 600, name = '', description = '', additional_info = '', show_response = False, show_logs = False):
     '''
     ----------------------------------------------------------
     Function to start the heartbeat
 
@@ -106,15 +103,15 @@
         name (str): process name
         description (str): process description
         additional_info (str) (optional): additional process data
         show_response (bool) (optional): show server response
         show_logs (bool) (optional): show log messages
     ----------------------------------------------------------
     '''
-    
+
     global variable_parameter, pulse_thread
 
     # Set variable_parameter to True
     variable_parameter = True
 
     try:
         # If there is already a thread running, wait for it to finish
@@ -139,10 +136,10 @@
 
     global variable_parameter, pulse_thread
     variable_parameter = False
     time.sleep(1)
 
     # Check the status of the thread
     if pulse_thread is not None and pulse_thread.is_alive():
-        print('>>> Heartbeat thread is still running. <<<')
+        print('!!! Heartbeat thread is still running. !!!')
     else:
         print('>>> Heartbeat thread has ended. <<<')
```

### Comparing `pyheartbeat-0.0.4/pyheartbeat.egg-info/PKG-INFO` & `pyheartbeat-0.0.5/pyheartbeat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyheartbeat
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: pyheartbeat,heartbeat_library,heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyheartbeat-0.0.4/setup.py` & `pyheartbeat-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-version = '0.0.4'
+version = '0.0.5'
 readme = open('README.md').read()
 
 setup(name='pyheartbeat',
     version=version,
     license='MIT License',
     author='Pedro Ferreira Braz',
     long_description=readme,
```

