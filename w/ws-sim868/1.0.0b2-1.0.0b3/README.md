# Comparing `tmp/ws_sim868-1.0.0b2.tar.gz` & `tmp/ws_sim868-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws_sim868-1.0.0b2.tar", last modified: Sun Feb 25 22:52:46 2024, max compression
+gzip compressed data, was "ws_sim868-1.0.0b3.tar", last modified: Tue May 14 05:39:38 2024, max compression
```

## Comparing `ws_sim868-1.0.0b2.tar` & `ws_sim868-1.0.0b3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 22:52:46.943547 ws_sim868-1.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-25 22:52:37.000000 ws_sim868-1.0.0b2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-25 22:52:46.943547 ws_sim868-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-25 22:52:37.000000 ws_sim868-1.0.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 22:52:37.000000 ws_sim868-1.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-25 22:52:46.943547 ws_sim868-1.0.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 22:52:46.939547 ws_sim868-1.0.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 22:52:46.943547 ws_sim868-1.0.0b2/src/ws_sim868/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 22:52:37.000000 ws_sim868-1.0.0b2/src/ws_sim868/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-02-25 22:52:37.000000 ws_sim868-1.0.0b2/src/ws_sim868/modemUnit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 22:52:46.943547 ws_sim868-1.0.0b2/src/ws_sim868.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-25 22:52:46.000000 ws_sim868-1.0.0b2/src/ws_sim868.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-25 22:52:46.000000 ws_sim868-1.0.0b2/src/ws_sim868.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 22:52:46.000000 ws_sim868-1.0.0b2/src/ws_sim868.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-25 22:52:46.000000 ws_sim868-1.0.0b2/src/ws_sim868.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:38.491824 ws_sim868-1.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 05:39:32.000000 ws_sim868-1.0.0b3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-14 05:39:38.491824 ws_sim868-1.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-14 05:39:32.000000 ws_sim868-1.0.0b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 05:39:32.000000 ws_sim868-1.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-14 05:39:38.495824 ws_sim868-1.0.0b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:38.491824 ws_sim868-1.0.0b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:38.491824 ws_sim868-1.0.0b3/src/ws_sim868/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:32.000000 ws_sim868-1.0.0b3/src/ws_sim868/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-14 05:39:32.000000 ws_sim868-1.0.0b3/src/ws_sim868/modemUnit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:38.491824 ws_sim868-1.0.0b3/src/ws_sim868.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-14 05:39:38.000000 ws_sim868-1.0.0b3/src/ws_sim868.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 05:39:38.000000 ws_sim868-1.0.0b3/src/ws_sim868.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 05:39:38.000000 ws_sim868-1.0.0b3/src/ws_sim868.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 05:39:38.000000 ws_sim868-1.0.0b3/src/ws_sim868.egg-info/top_level.txt
```

### Comparing `ws_sim868-1.0.0b2/LICENSE.txt` & `ws_sim868-1.0.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ws_sim868-1.0.0b2/PKG-INFO` & `ws_sim868-1.0.0b3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ws_sim868
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Python package to control the Waveshare GSM/GPRS/GNSS Pi HAT
 Home-page: https://github.com/matthewnaruzny/ws_sim868
 Author: Matthew Naruzny
-Author-email: matthewnaruzny@gmail.com
+Author-email: matthew@mnaruzny.com
 Project-URL: Bug Tracker, https://github.com/matthewnaruzny/ws_sim868/issues
 Project-URL: Repository, https://github.com/matthewnaruzny/ws_sim868
 Project-URL: Documentation, https://matthewnaruzny.github.io/ws_sim868/ws_sim868/modemUnit.html
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ws_sim868-1.0.0b2/README.md` & `ws_sim868-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `ws_sim868-1.0.0b2/setup.cfg` & `ws_sim868-1.0.0b3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = ws_sim868
-version = 1.0.0-beta.2
+version = 1.0.0-beta.3
 author = Matthew Naruzny
-author_email = matthewnaruzny@gmail.com
+author_email = matthew@mnaruzny.com
 description = Python package to control the Waveshare GSM/GPRS/GNSS Pi HAT
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/matthewnaruzny/ws_sim868
 project_urls = 
 	Bug Tracker = https://github.com/matthewnaruzny/ws_sim868/issues
 	Repository = https://github.com/matthewnaruzny/ws_sim868
```

### Comparing `ws_sim868-1.0.0b2/src/ws_sim868/modemUnit.py` & `ws_sim868-1.0.0b3/src/ws_sim868/modemUnit.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,23 +76,24 @@
     def __str__(self):
         return self.cgnsinf
 
 
 
 
 class ModemUnit:
-    def __init__(self, port='/dev/ttyS0', baudrate=115200, log=True):
+    def __init__(self, port='/dev/ttyS0', baudrate=115200, log=True, http_reinit=3):
 
         # Logging
         if log:
             logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
         # Serial Config
         self.__serial_port = port
         self.__serial_baudrate = baudrate
+        self.connect()
 
         # Serial
         self.__ser = serial.Serial(port, baudrate=baudrate)
         self.__write_lock = False
         self.__command_queue = queue.Queue()
         self.__command_last = ""
         self.__command_last_time = 0
@@ -109,24 +110,25 @@
 
         # Network
         self.__network_active = False
         self.__apn_config = None
 
         # HTTP
         self.__http_queue = queue.Queue()
-        self.__http_result = {}
         self.__http_in_request = False
-        self.__http_current_uuid = ""
+        self.__http_current_rqueue = None
         self.__http_current_request = None
-        self.__http_request_cache = {}
+        self.__http_fail_count = 0
+        self.__http_fail_max = http_reinit
 
         # Init Commands
         self.modem_execute("AT+GSN")
 
         # Worker Thread
+        self.__worker_working = True
         self.__mthread = None
         self.__start_worker()
 
     # Modem Base Functionality
     def __process_input(self):
         if self.__ser.in_waiting > 0:
             while self.__ser.in_waiting:
@@ -152,32 +154,32 @@
                     self.__gnss_loc = GPSData(data)
                 elif newline.startswith("+HTTPACTION"):  # HTTP Response
                     self.__write_lock = False
                     reply = newline.split()[1].split(',')
                     cid = int(reply[0])
                     http_status = int(reply[1])
                     data_size = int(reply[2])
-                    self.__http_result[self.__http_current_uuid] = {'cid': cid, 'http_status': http_status,
-                                                                    'data_size': data_size, 'data': None}
+                    assert isinstance(self.__http_current_rqueue, queue.Queue)
+                    self.__http_current_rqueue.put({'cid': cid, 'http_status': http_status,
+                                                    'data_size': data_size})
                     if data_size > 0 and http_status == 200:  # Fetch Data
                         logging.info("Modem: Loading HTTP Data")
                         self.__http_fetch_data()
                     else:
                         self.__http_in_request = False
                         self.__http_current_uuid = None
                         return
                 elif newline.startswith("+HTTPREAD"): # HTTP Response Data
                     while True:
                         if self.__ser.in_waiting > 0:
                             dataline = self.__ser.readline().decode('utf-8')
                             logging.info("Modem: HTTP DATA: " + dataline)
                             self.__write_lock = False
-                            http_result = self.__http_result[self.__http_current_uuid]
-                            http_result['data'] = dataline
-                            self.__http_result[self.__http_current_uuid] = http_result
+                            self.__http_current_rqueue.put(dataline)
+                            self.__http_in_request = False
                             return
                         time.sleep(0.1)
                 elif self.__command_last == 'AT+GSN' and newline != 'AT+GSN' and self.__imei is None:
                     self.__imei = newline
                     self.__write_lock = False
                     return
 
@@ -200,28 +202,55 @@
         """
         self.__command_queue.put(cmd)
 
     def __health_check(self):
         if time.time() - self.__last_health > 30 and time.time() - self.__command_last_time > 30:
             if self.__write_lock:  # If waiting for reply and waiting over 30 seconds
                 self.power_toggle()
-            elif not self.__write_lock and not self.__command_queue.empty():
+            elif self.__command_queue.empty():
                 self.modem_execute("AT")
 
     def __reinit(self):
+        self.__write_lock = False
+        with self.__command_queue.mutex: # Clear Command Queue
+            self.__command_queue.queue.clear()
+
+        if self.__http_in_request: # Re-queue in-progress HTTP request
+            self.__http_in_request = False
+            self.__http_current_uuid = ""
+            self.__http_queue.put(self.__http_current_request)
+            self.__http_current_request = None
+
+        # Disconnect and Reconnect Serial
+        self.__ser.close()
+        time.sleep(5)
+        self.__ser = serial.Serial(self.__serial_port, baudrate=self.__serial_baudrate)
+
+        time.sleep(5)
+
         if self.__network_active and self.__apn_config is not None: # Network
             self.__network_active = False
             self.network_start()
 
         if self.__gnss_active and self.__gnss_rate != 0: # GNSS
             self.gnss_start(rate=self.__gnss_rate)
 
         if self.__imei is None:
             self.modem_execute("AT+GSN")
 
+    def connect(self):
+        self.__ser = serial.Serial(self.__serial_port, baudrate=self.__serial_baudrate)
+        self.__write_lock = False
+
+    def disconnect(self):
+        """
+        Close serial connection to Modem.
+        """
+        self.__write_lock = True
+        self.__ser.close()
 
     def power_toggle(self) -> None:
         """
         Toggle power of Modem
         """
         logging.critical("Sys: Toggling Modem Power")
         self.__last_health = time.time()
@@ -233,30 +262,14 @@
         while True:
             GPIO.output(7, GPIO.LOW)
             time.sleep(4)
             GPIO.output(7, GPIO.HIGH)
             break
         GPIO.cleanup()
 
-        # Reset
-        self.__write_lock = False
-        with self.__command_queue.mutex:
-            self.__command_queue.queue.clear()
-
-        if self.__http_in_request:
-            self.__http_in_request = False
-            self.__http_current_uuid = ""
-            self.__http_queue.put(self.__http_current_request)
-            self.__http_current_request = None
-
-        # Disconnect and Reconnect Serial
-        self.__ser.close()
-        time.sleep(5)
-        self.__ser = serial.Serial(self.__serial_port, baudrate=self.__serial_baudrate)
-
         time.sleep(5)
         self.__reinit()
 
     def __main_thread(self):
         while self.__worker_working:
             self.__health_check()
 
@@ -332,17 +345,16 @@
 
     def __http_execute_next(self):
         if self.__http_in_request or self.__http_queue.empty():  # Stop if request already in progress or if no requests
             return
 
         self.__http_in_request = True
         req = self.__http_queue.get()
-        self.__http_current_uuid = req['uuid']
+        self.__http_current_rqueue = req['rqueue']
         self.__http_current_request = req
-        self.__http_request_cache[req['uuid']] = req
 
         self.modem_execute("AT+HTTPTERM")
         self.modem_execute("AT+HTTPINIT")
         self.modem_execute('AT+HTTPPARA="URL","' + str(req['url']) + '"')
         self.modem_execute('AT+HTTPPARA="CID",1')
         self.modem_execute('AT+HTTPACTION=' + str(req['method']))
 
@@ -356,30 +368,37 @@
     def __http_request(self, method, url):
         """
         Method to perform a http request.
         :param method: Integer representing HTTP request method. 0 - GET.
         :param url: URL to request.
         :return: Dict containing response code, data size, and data.
         """
-        if self.__network_active is False and self.__apn_config is not None:
+        if self.__network_active is False and self.__apn_config is not None: # Start if not active
             self.network_start()
-        new_uuid = uuid.uuid4()
-        self.__http_result[new_uuid] = None
-        self.__http_queue.put({'url': url, 'method': method, 'uuid': new_uuid})
-        while True:  # Wait for Response
-            if self.__http_result[new_uuid] is not None:
-                if (self.__http_result[new_uuid]['data_size'] != 0 and self.__http_result[new_uuid]['data'] is not None) or self.__http_result[new_uuid]['data_size'] == 0:
-                    res = self.__http_result[new_uuid]
-
-                    # Clear Cache
-                    self.__http_result.pop(new_uuid)
-                    self.__http_request_cache.pop(new_uuid)
 
-                    return res
-            time.sleep(0.1)
+        if self.__http_fail_count >= self.__http_fail_max != 0: # Retry if too many fails
+            logging.warning("Too many failed attempts. Restarting Network.")
+            self.network_stop()
+            self.network_start()
+
+        rqueue = queue.Queue()
+        self.__http_queue.put({'url': url, 'method': method, 'rqueue': rqueue})
+
+        res = rqueue.get() # Wait for result
+
+        # Check Result Code
+        if res['http_status'] >= 600:
+            self.__http_fail_count += 1
+
+        if res['data_size'] > 0:
+            data = rqueue.get() # Wait for data
+            res['data'] = data
+
+        return res
+
 
     def http_get(self, url) -> dict:
         """
         HTTP GET request
         :param url: URL to request
         :return: Dict containing response code, data size, and data.
         """
```

### Comparing `ws_sim868-1.0.0b2/src/ws_sim868.egg-info/PKG-INFO` & `ws_sim868-1.0.0b3/src/ws_sim868.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ws_sim868
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Python package to control the Waveshare GSM/GPRS/GNSS Pi HAT
 Home-page: https://github.com/matthewnaruzny/ws_sim868
 Author: Matthew Naruzny
-Author-email: matthewnaruzny@gmail.com
+Author-email: matthew@mnaruzny.com
 Project-URL: Bug Tracker, https://github.com/matthewnaruzny/ws_sim868/issues
 Project-URL: Repository, https://github.com/matthewnaruzny/ws_sim868
 Project-URL: Documentation, https://matthewnaruzny.github.io/ws_sim868/ws_sim868/modemUnit.html
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

