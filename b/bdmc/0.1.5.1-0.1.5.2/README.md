# Comparing `tmp/bdmc-0.1.5.1.tar.gz` & `tmp/bdmc-0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdmc-0.1.5.1.tar", last modified: Mon May 13 08:37:14 2024, max compression
+gzip compressed data, was "bdmc-0.1.5.2.tar", last modified: Tue May 14 03:52:51 2024, max compression
```

## Comparing `bdmc-0.1.5.1.tar` & `bdmc-0.1.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5466 2024-05-13 08:36:54.362503 bdmc-0.1.5.1/README.md
--rw-r--r--   0        0        0      547 2024-05-13 08:37:14.022550 bdmc-0.1.5.1/pyproject.toml
--rw-r--r--   0        0        0      556 2024-05-13 08:36:54.362503 bdmc-0.1.5.1/src/bdmc/__init__.py
--rw-r--r--   0        0        0      419 2024-05-13 08:36:54.362503 bdmc-0.1.5.1/src/bdmc/modules/cmd.py
--rw-r--r--   0        0        0    17112 2024-05-13 08:36:54.362503 bdmc-0.1.5.1/src/bdmc/modules/controller.py
--rw-r--r--   0        0        0     2266 2024-05-13 08:36:54.362503 bdmc-0.1.5.1/src/bdmc/modules/debug.py
--rw-r--r--   0        0        0      574 2024-05-13 08:36:54.362503 bdmc-0.1.5.1/src/bdmc/modules/logger.py
--rw-r--r--   0        0        0     1356 2024-05-13 08:36:54.366503 bdmc-0.1.5.1/src/bdmc/modules/port.py
--rw-r--r--   0        0        0     7529 2024-05-13 08:36:54.366503 bdmc-0.1.5.1/src/bdmc/modules/seriald.py
--rw-r--r--   0        0        0      682 2024-05-13 08:36:54.366503 bdmc-0.1.5.1/tests/find_tests.py
--rw-r--r--   0        0        0     4380 2024-05-13 08:36:54.366503 bdmc-0.1.5.1/tests/test_context.py
--rw-r--r--   0        0        0     1989 2024-05-13 08:36:54.366503 bdmc-0.1.5.1/tests/test_controller.py
--rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     5466 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/README.md
+-rw-r--r--   0        0        0      547 2024-05-14 03:52:51.047887 bdmc-0.1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      556 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/__init__.py
+-rw-r--r--   0        0        0      419 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/modules/cmd.py
+-rw-r--r--   0        0        0    17495 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/modules/controller.py
+-rw-r--r--   0        0        0     2266 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/modules/debug.py
+-rw-r--r--   0        0        0      574 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/modules/logger.py
+-rw-r--r--   0        0        0     1356 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/modules/port.py
+-rw-r--r--   0        0        0     7529 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/modules/seriald.py
+-rw-r--r--   0        0        0      682 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/tests/find_tests.py
+-rw-r--r--   0        0        0     4380 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/tests/test_context.py
+-rw-r--r--   0        0        0     1989 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/tests/test_controller.py
+-rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.2/PKG-INFO
```

### Comparing `bdmc-0.1.5.1/README.md` & `bdmc-0.1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.1/pyproject.toml` & `bdmc-0.1.5.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdmc"
-version = "0.1.5.1"
+version = "0.1.5.2"
 description = "An api wrapper lib designed for the uptech BDMC divers"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "pyserial>=3.5",
     "coloredlogs>=15.0.1",
```

### Comparing `bdmc-0.1.5.1/src/bdmc/__init__.py` & `bdmc-0.1.5.2/src/bdmc/__init__.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.1/src/bdmc/modules/controller.py` & `bdmc-0.1.5.2/src/bdmc/modules/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,24 +257,33 @@
         """
         return self._serial
 
     def stop_msg_sending(self) -> Self:
         """
         Stop the message sending by setting the _msg_send_thread_should_run flag to False and joining the message send thread.
         """
+        if self._msg_send_thread is None:
+            _logger.error("Message sending thread is not running")
+            return self
         self._msg_send_thread_should_run = False
         self._msg_send_thread.join()
         self._msg_send_thread = None
         return self
 
     def start_msg_sending(self) -> Self:
         """
         A description of the entire function, its parameters, and its return types.
         """
 
+        if not self._serial.is_connected:
+            _logger.error("Serial port is not connected")
+            if not self._serial.open():
+                _logger.error(f"Failed to open serial port {self._serial.port}")
+                return self
+
         _logger.info("MSG sending thread starting")
         self._msg_send_thread_should_run = True
         _logger.info(f"MSG sending thread started")
         self._msg_send_thread = Thread(name="msg_send_thread", target=self._msg_sending_loop)
         self._msg_send_thread.daemon = True
         self._msg_send_thread.start()
         _logger.info("MSG sending thread stopped")
```

### Comparing `bdmc-0.1.5.1/src/bdmc/modules/debug.py` & `bdmc-0.1.5.2/src/bdmc/modules/debug.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.1/src/bdmc/modules/logger.py` & `bdmc-0.1.5.2/src/bdmc/modules/logger.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.1/src/bdmc/modules/port.py` & `bdmc-0.1.5.2/src/bdmc/modules/port.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.1/src/bdmc/modules/seriald.py` & `bdmc-0.1.5.2/src/bdmc/modules/seriald.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.1/tests/find_tests.py` & `bdmc-0.1.5.2/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.1/tests/test_context.py` & `bdmc-0.1.5.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.1/tests/test_controller.py` & `bdmc-0.1.5.2/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.1/PKG-INFO` & `bdmc-0.1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdmc
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: An api wrapper lib designed for the uptech BDMC divers
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: pyserial>=3.5
 Requires-Dist: coloredlogs>=15.0.1
 Description-Content-Type: text/markdown
```

