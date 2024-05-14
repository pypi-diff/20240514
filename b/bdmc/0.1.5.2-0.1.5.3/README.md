# Comparing `tmp/bdmc-0.1.5.2.tar.gz` & `tmp/bdmc-0.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdmc-0.1.5.2.tar", last modified: Tue May 14 03:52:51 2024, max compression
+gzip compressed data, was "bdmc-0.1.5.3.tar", last modified: Tue May 14 09:09:57 2024, max compression
```

## Comparing `bdmc-0.1.5.2.tar` & `bdmc-0.1.5.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5466 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/README.md
--rw-r--r--   0        0        0      547 2024-05-14 03:52:51.047887 bdmc-0.1.5.2/pyproject.toml
--rw-r--r--   0        0        0      556 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/__init__.py
--rw-r--r--   0        0        0      419 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/modules/cmd.py
--rw-r--r--   0        0        0    17495 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/modules/controller.py
--rw-r--r--   0        0        0     2266 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/modules/debug.py
--rw-r--r--   0        0        0      574 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/modules/logger.py
--rw-r--r--   0        0        0     1356 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/modules/port.py
--rw-r--r--   0        0        0     7529 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/src/bdmc/modules/seriald.py
--rw-r--r--   0        0        0      682 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/tests/find_tests.py
--rw-r--r--   0        0        0     4380 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/tests/test_context.py
--rw-r--r--   0        0        0     1989 2024-05-14 03:52:31.475907 bdmc-0.1.5.2/tests/test_controller.py
--rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     5466 2024-05-14 09:09:37.596335 bdmc-0.1.5.3/README.md
+-rw-r--r--   0        0        0      547 2024-05-14 09:09:57.744408 bdmc-0.1.5.3/pyproject.toml
+-rw-r--r--   0        0        0      556 2024-05-14 09:09:37.596335 bdmc-0.1.5.3/src/bdmc/__init__.py
+-rw-r--r--   0        0        0      419 2024-05-14 09:09:37.596335 bdmc-0.1.5.3/src/bdmc/modules/cmd.py
+-rw-r--r--   0        0        0    17599 2024-05-14 09:09:37.596335 bdmc-0.1.5.3/src/bdmc/modules/controller.py
+-rw-r--r--   0        0        0     2266 2024-05-14 09:09:37.596335 bdmc-0.1.5.3/src/bdmc/modules/debug.py
+-rw-r--r--   0        0        0      574 2024-05-14 09:09:37.596335 bdmc-0.1.5.3/src/bdmc/modules/logger.py
+-rw-r--r--   0        0        0     1356 2024-05-14 09:09:37.596335 bdmc-0.1.5.3/src/bdmc/modules/port.py
+-rw-r--r--   0        0        0     7529 2024-05-14 09:09:37.596335 bdmc-0.1.5.3/src/bdmc/modules/seriald.py
+-rw-r--r--   0        0        0      682 2024-05-14 09:09:37.596335 bdmc-0.1.5.3/tests/find_tests.py
+-rw-r--r--   0        0        0     4380 2024-05-14 09:09:37.596335 bdmc-0.1.5.3/tests/test_context.py
+-rw-r--r--   0        0        0     1989 2024-05-14 09:09:37.596335 bdmc-0.1.5.3/tests/test_controller.py
+-rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.3/PKG-INFO
```

### Comparing `bdmc-0.1.5.2/README.md` & `bdmc-0.1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.2/pyproject.toml` & `bdmc-0.1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdmc"
-version = "0.1.5.2"
+version = "0.1.5.3"
 description = "An api wrapper lib designed for the uptech BDMC divers"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "pyserial>=3.5",
     "coloredlogs>=15.0.1",
```

### Comparing `bdmc-0.1.5.2/src/bdmc/__init__.py` & `bdmc-0.1.5.3/src/bdmc/__init__.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.2/src/bdmc/modules/controller.py` & `bdmc-0.1.5.3/src/bdmc/modules/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,16 +258,17 @@
         return self._serial
 
     def stop_msg_sending(self) -> Self:
         """
         Stop the message sending by setting the _msg_send_thread_should_run flag to False and joining the message send thread.
         """
         if self._msg_send_thread is None:
-            _logger.error("Message sending thread is not running")
+            _logger.error("Message sending thread is not running.")
             return self
+        _logger.info("Try to stop message sending thread.")
         self._msg_send_thread_should_run = False
         self._msg_send_thread.join()
         self._msg_send_thread = None
         return self
 
     def start_msg_sending(self) -> Self:
         """
@@ -278,32 +279,35 @@
             _logger.error("Serial port is not connected")
             if not self._serial.open():
                 _logger.error(f"Failed to open serial port {self._serial.port}")
                 return self
 
         _logger.info("MSG sending thread starting")
         self._msg_send_thread_should_run = True
-        _logger.info(f"MSG sending thread started")
-        self._msg_send_thread = Thread(name="msg_send_thread", target=self._msg_sending_loop)
-        self._msg_send_thread.daemon = True
-        self._msg_send_thread.start()
-        _logger.info("MSG sending thread stopped")
-        return self
 
-    def _msg_sending_loop(self) -> None:
-        """
-        A function that handles the sending of messages in a loop.
-        It continuously retrieves messages from a queue and writes them to a channel until the thread should stop running.
-        Returns None.
-        """
+        cmd_queue_get = self._cmd_queue.get
+        serial_write = self._serial.write
 
-        while self._msg_send_thread_should_run:
-            temp = self._cmd_queue.get()
-            _logger.debug(f"Writing {temp} to channel,remaining {self._cmd_queue.qsize()}")
-            self._serial.write(temp)
+        def _msg_sending_loop() -> None:
+            """
+            A function that handles the sending of messages in a loop.
+            It continuously retrieves messages from a queue and writes them to a channel until the thread should stop running.
+            Returns None.
+            """
+
+            while self._msg_send_thread_should_run:
+                temp = cmd_queue_get()
+                _logger.debug(f"Writing {temp} to channel.")
+                serial_write(temp)
+            _logger.info("MSG sending thread sopped")
+
+        self._msg_send_thread = Thread(name="msg_send_thread", target=_msg_sending_loop, daemon=True)
+        self._msg_send_thread.start()
+        _logger.info("MSG sending thread started")
+        return self
 
     def set_motors_speed(self, speeds: Sequence[int | float]) -> Self:
         """
         Set the speed for each motor based on the provided speed_list.
 
         Parameters:
             speeds (Sequence[int|float]): A list of speeds for each motor.
```

### Comparing `bdmc-0.1.5.2/src/bdmc/modules/debug.py` & `bdmc-0.1.5.3/src/bdmc/modules/debug.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.2/src/bdmc/modules/logger.py` & `bdmc-0.1.5.3/src/bdmc/modules/logger.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.2/src/bdmc/modules/port.py` & `bdmc-0.1.5.3/src/bdmc/modules/port.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.2/src/bdmc/modules/seriald.py` & `bdmc-0.1.5.3/src/bdmc/modules/seriald.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.2/tests/find_tests.py` & `bdmc-0.1.5.3/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.2/tests/test_context.py` & `bdmc-0.1.5.3/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.2/tests/test_controller.py` & `bdmc-0.1.5.3/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.2/PKG-INFO` & `bdmc-0.1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdmc
-Version: 0.1.5.2
+Version: 0.1.5.3
 Summary: An api wrapper lib designed for the uptech BDMC divers
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: pyserial>=3.5
 Requires-Dist: coloredlogs>=15.0.1
 Description-Content-Type: text/markdown
```

