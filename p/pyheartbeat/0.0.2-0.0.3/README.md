# Comparing `tmp/pyheartbeat-0.0.2.tar.gz` & `tmp/pyheartbeat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyheartbeat-0.0.2.tar", last modified: Tue May  7 13:59:33 2024, max compression
+gzip compressed data, was "pyheartbeat-0.0.3.tar", last modified: Tue May 14 12:38:33 2024, max compression
```

## Comparing `pyheartbeat-0.0.2.tar` & `pyheartbeat-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 13:59:33.231012 pyheartbeat-0.0.2/
--rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 pyheartbeat-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2115 2024-05-07 13:59:33.219832 pyheartbeat-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1279 2024-05-07 13:58:40.000000 pyheartbeat-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 13:59:33.211424 pyheartbeat-0.0.2/pyheartbeat/
--rw-rw-rw-   0        0        0       69 2024-05-07 13:50:50.000000 pyheartbeat-0.0.2/pyheartbeat/__init__.py
--rw-rw-rw-   0        0        0     3416 2024-05-06 17:50:42.000000 pyheartbeat-0.0.2/pyheartbeat/heartbeat_library.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:59:33.217423 pyheartbeat-0.0.2/pyheartbeat.egg-info/
--rw-rw-rw-   0        0        0     2115 2024-05-07 13:59:33.000000 pyheartbeat-0.0.2/pyheartbeat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-07 13:59:33.000000 pyheartbeat-0.0.2/pyheartbeat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 13:59:33.000000 pyheartbeat-0.0.2/pyheartbeat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-07 13:59:33.000000 pyheartbeat-0.0.2/pyheartbeat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-07 13:59:33.000000 pyheartbeat-0.0.2/pyheartbeat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 13:59:33.231012 pyheartbeat-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1065 2024-05-07 13:58:16.000000 pyheartbeat-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:38:33.881574 pyheartbeat-0.0.3/
+-rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 pyheartbeat-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2084 2024-05-14 12:38:33.880084 pyheartbeat-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2024-05-14 12:36:25.000000 pyheartbeat-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 12:38:33.872133 pyheartbeat-0.0.3/pyheartbeat/
+-rw-rw-rw-   0        0        0       69 2024-05-07 13:50:50.000000 pyheartbeat-0.0.3/pyheartbeat/__init__.py
+-rw-rw-rw-   0        0        0     4083 2024-05-14 12:33:33.000000 pyheartbeat-0.0.3/pyheartbeat/heartbeat_library.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:38:33.878087 pyheartbeat-0.0.3/pyheartbeat.egg-info/
+-rw-rw-rw-   0        0        0     2084 2024-05-14 12:38:33.000000 pyheartbeat-0.0.3/pyheartbeat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-14 12:38:33.000000 pyheartbeat-0.0.3/pyheartbeat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 12:38:33.000000 pyheartbeat-0.0.3/pyheartbeat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-14 12:38:33.000000 pyheartbeat-0.0.3/pyheartbeat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-14 12:38:33.000000 pyheartbeat-0.0.3/pyheartbeat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 12:38:33.881574 pyheartbeat-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1065 2024-05-14 12:36:55.000000 pyheartbeat-0.0.3/setup.py
```

### Comparing `pyheartbeat-0.0.2/LICENSE` & `pyheartbeat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyheartbeat-0.0.2/PKG-INFO` & `pyheartbeat-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyheartbeat
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: pyheartbeat,heartbeat_library,heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,26 +19,26 @@
 You can install the Python Heartbeat Library using pip:
 
 pip install pyheartbeat
 
 # Example
 
 ```python
-===============================================================================================================================
+======================================================================================================
 from pyheartbeat import setUrl, heartbeat, killHeartbeat
 
 # Set the URL for sending pulses
-setUrl("https://{your_url}")
+setUrl("https://your_url")
 
 # Start the heartbeat with a pulse every x seconds
-heartbeat(interval = {seconds}, name = '{process name}', description = '{process description}', additional_info = {''}, show_response = True)
+heartbeat(interval = 600, name = 'process name', description = 'process description', additional_info = 'additional info', show_response = True, show_logs = True)
 
 # Your main script logic goes here...
 
 # When your script ends or encounters an error, stop the heartbeat
 killHeartbeat()
-===============================================================================================================================
+======================================================================================================
 ```
 
 # License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `pyheartbeat-0.0.2/README.md` & `pyheartbeat-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 You can install the Python Heartbeat Library using pip:
 
 pip install pyheartbeat
 
 # Example
 
 ```python
-===============================================================================================================================
+======================================================================================================
 from pyheartbeat import setUrl, heartbeat, killHeartbeat
 
 # Set the URL for sending pulses
-setUrl("https://{your_url}")
+setUrl("https://your_url")
 
 # Start the heartbeat with a pulse every x seconds
-heartbeat(interval = {seconds}, name = '{process name}', description = '{process description}', additional_info = {''}, show_response = True)
+heartbeat(interval = 600, name = 'process name', description = 'process description', additional_info = 'additional info', show_response = True, show_logs = True)
 
 # Your main script logic goes here...
 
 # When your script ends or encounters an error, stop the heartbeat
 killHeartbeat()
-===============================================================================================================================
+======================================================================================================
 ```
 
 # License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `pyheartbeat-0.0.2/pyheartbeat/heartbeat_library.py` & `pyheartbeat-0.0.3/pyheartbeat/heartbeat_library.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 # Define the pulse sending URL
 url = ""
 
 # Heartbeat control variable
 variable_parameter = True
 
+# Pulse thread
+pulse_thread = None
 
 # 0
 def setUrl(url_):
     '''
     ----------------------------------------------------------
     Function to set a URL for pulse sending
 
@@ -46,71 +48,88 @@
             "processDescription": f"{description}",
             "additionalData": f"{additional_info}"
         })
         headers = {'Content-Type': 'application/json'}
         response = requests.request("POST", url, headers=headers, data=payload)
 
     except Exception as e:
-        print('\nError sending pulse! ', e)
+        print('\n*** Error sending pulse! *** >', e)
 
     finally:
         try:
             if show_response:
-                print(f'Heartbeat response: {response.status_code}')
+                print(f'>>> Heartbeat response: {response.status_code} <<<')
             pass
         except:
             pass 
 
 
 # 2
-def pulse(interval, name, description, additional_info, show_response):
+def pulse(interval, name, description, additional_info, show_response, show_logs):
     '''
     ----------------------------------------------------------
     Function to send a pulse to the server at regular intervals
 
     Parameters:
         interval (int): time between pulses (in seconds)
         name (str): process name
         description (str): process description
         additional_info (str) (optional): additional process data
         show_response (bool) (optional): show server response
+        show_logs (bool) (optional): show log messages
     ----------------------------------------------------------
     '''
 
     while variable_parameter:
         sendPulse(name, description, additional_info, show_response)
-        time.sleep(interval)
+
+        # If the variable_parameter is False, break the loop
+        for _ in range(interval):
+            if not variable_parameter:
+                break # break the loop
+            time.sleep(1)
+
+    if show_logs:
+        print('>>> Heartbeat thread has ended. <<<')
 
 
 # 3
-def heartbeat(interval = 600, name = '', description = '', additional_info = '', show_response = False):
+def heartbeat(interval = 600, name = '', description = '', additional_info = '', show_response = False, show_logs = False):
     '''
     ----------------------------------------------------------
     Function to start the heartbeat
 
     Parameters:
         interval (int): time between pulses (in seconds)
         name (str): process name
         description (str): process description
         additional_info (str) (optional): additional process data
         show_response (bool) (optional): show server response
+        show_logs (bool) (optional): show log messages
     ----------------------------------------------------------
     '''
+    global pulse_thread
 
     try:
-        pulse_thread = threading.Thread(target=pulse, args=(interval, name, description, additional_info, show_response))
+        # If there is already a thread running, wait for it to finish
+        if pulse_thread is not None:
+            pulse_thread.join(timeout=1.0)
+
+
+        # Start the pulse thread
+        pulse_thread = threading.Thread(target=pulse, args=(interval, name, description, additional_info, show_response, show_logs))
         pulse_thread.start()
 
     except Exception as e:
-        print('Error in heartbeat thread! ', e)
+        print('*** Error in heartbeat thread! *** > ', e)
 
 
 # 4
 def killHeartbeat():
     '''
     ----------------------------------------------------------
     Function to stop the heartbeat
     ----------------------------------------------------------
     '''
 
     global variable_parameter
-    variable_parameter = not variable_parameter
+    variable_parameter = False
```

### Comparing `pyheartbeat-0.0.2/pyheartbeat.egg-info/PKG-INFO` & `pyheartbeat-0.0.3/pyheartbeat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyheartbeat
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: pyheartbeat,heartbeat_library,heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,26 +19,26 @@
 You can install the Python Heartbeat Library using pip:
 
 pip install pyheartbeat
 
 # Example
 
 ```python
-===============================================================================================================================
+======================================================================================================
 from pyheartbeat import setUrl, heartbeat, killHeartbeat
 
 # Set the URL for sending pulses
-setUrl("https://{your_url}")
+setUrl("https://your_url")
 
 # Start the heartbeat with a pulse every x seconds
-heartbeat(interval = {seconds}, name = '{process name}', description = '{process description}', additional_info = {''}, show_response = True)
+heartbeat(interval = 600, name = 'process name', description = 'process description', additional_info = 'additional info', show_response = True, show_logs = True)
 
 # Your main script logic goes here...
 
 # When your script ends or encounters an error, stop the heartbeat
 killHeartbeat()
-===============================================================================================================================
+======================================================================================================
 ```
 
 # License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `pyheartbeat-0.0.2/setup.py` & `pyheartbeat-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-version = '0.0.2'
+version = '0.0.3'
 readme = open('README.md').read()
 
 setup(name='pyheartbeat',
     version=version,
     license='MIT License',
     author='Pedro Ferreira Braz',
     long_description=readme,
```

