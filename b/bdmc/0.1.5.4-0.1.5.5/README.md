# Comparing `tmp/bdmc-0.1.5.4.tar.gz` & `tmp/bdmc-0.1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdmc-0.1.5.4.tar", last modified: Tue May 14 10:29:12 2024, max compression
+gzip compressed data, was "bdmc-0.1.5.5.tar", last modified: Tue May 14 10:40:12 2024, max compression
```

## Comparing `bdmc-0.1.5.4.tar` & `bdmc-0.1.5.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5466 2024-05-14 10:28:52.818567 bdmc-0.1.5.4/README.md
--rw-r--r--   0        0        0      547 2024-05-14 10:29:12.610499 bdmc-0.1.5.4/pyproject.toml
--rw-r--r--   0        0        0      556 2024-05-14 10:28:52.818567 bdmc-0.1.5.4/src/bdmc/__init__.py
--rw-r--r--   0        0        0      419 2024-05-14 10:28:52.818567 bdmc-0.1.5.4/src/bdmc/modules/cmd.py
--rw-r--r--   0        0        0    17709 2024-05-14 10:28:52.818567 bdmc-0.1.5.4/src/bdmc/modules/controller.py
--rw-r--r--   0        0        0     2266 2024-05-14 10:28:52.818567 bdmc-0.1.5.4/src/bdmc/modules/debug.py
--rw-r--r--   0        0        0      574 2024-05-14 10:28:52.818567 bdmc-0.1.5.4/src/bdmc/modules/logger.py
--rw-r--r--   0        0        0     1356 2024-05-14 10:28:52.818567 bdmc-0.1.5.4/src/bdmc/modules/port.py
--rw-r--r--   0        0        0     7529 2024-05-14 10:28:52.818567 bdmc-0.1.5.4/src/bdmc/modules/seriald.py
--rw-r--r--   0        0        0      682 2024-05-14 10:28:52.818567 bdmc-0.1.5.4/tests/find_tests.py
--rw-r--r--   0        0        0     4380 2024-05-14 10:28:52.818567 bdmc-0.1.5.4/tests/test_context.py
--rw-r--r--   0        0        0     1989 2024-05-14 10:28:52.818567 bdmc-0.1.5.4/tests/test_controller.py
--rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     5466 2024-05-14 10:39:51.956238 bdmc-0.1.5.5/README.md
+-rw-r--r--   0        0        0      547 2024-05-14 10:40:12.900275 bdmc-0.1.5.5/pyproject.toml
+-rw-r--r--   0        0        0      556 2024-05-14 10:39:51.956238 bdmc-0.1.5.5/src/bdmc/__init__.py
+-rw-r--r--   0        0        0      419 2024-05-14 10:39:51.956238 bdmc-0.1.5.5/src/bdmc/modules/cmd.py
+-rw-r--r--   0        0        0    17697 2024-05-14 10:39:51.956238 bdmc-0.1.5.5/src/bdmc/modules/controller.py
+-rw-r--r--   0        0        0     2266 2024-05-14 10:39:51.956238 bdmc-0.1.5.5/src/bdmc/modules/debug.py
+-rw-r--r--   0        0        0      574 2024-05-14 10:39:51.956238 bdmc-0.1.5.5/src/bdmc/modules/logger.py
+-rw-r--r--   0        0        0     1356 2024-05-14 10:39:51.956238 bdmc-0.1.5.5/src/bdmc/modules/port.py
+-rw-r--r--   0        0        0     7529 2024-05-14 10:39:51.956238 bdmc-0.1.5.5/src/bdmc/modules/seriald.py
+-rw-r--r--   0        0        0      682 2024-05-14 10:39:51.956238 bdmc-0.1.5.5/tests/find_tests.py
+-rw-r--r--   0        0        0     4380 2024-05-14 10:39:51.956238 bdmc-0.1.5.5/tests/test_context.py
+-rw-r--r--   0        0        0     1989 2024-05-14 10:39:51.956238 bdmc-0.1.5.5/tests/test_controller.py
+-rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.5/PKG-INFO
```

### Comparing `bdmc-0.1.5.4/README.md` & `bdmc-0.1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.4/pyproject.toml` & `bdmc-0.1.5.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdmc"
-version = "0.1.5.4"
+version = "0.1.5.5"
 description = "An api wrapper lib designed for the uptech BDMC divers"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "pyserial>=3.5",
     "coloredlogs>=15.0.1",
```

### Comparing `bdmc-0.1.5.4/src/bdmc/__init__.py` & `bdmc-0.1.5.5/src/bdmc/__init__.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.4/src/bdmc/modules/controller.py` & `bdmc-0.1.5.5/src/bdmc/modules/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,16 +261,17 @@
         """
         Stop the message sending by setting the _msg_send_thread_should_run flag to False and joining the message send thread.
         """
         if self._msg_send_thread is None:
             _logger.error("Message sending thread is not running.")
             return self
         _logger.info("Try to stop message sending thread.")
-        if not self._cmd_queue.empty():
-            self._cmd_queue.join()
+        while self._cmd_queue.empty():
+            sleep(0.1)
+
         self._msg_send_thread_should_run = False
         self._cmd_queue.put(b"\r")
         self._msg_send_thread.join()
         self._msg_send_thread = None
         return self
 
     def start_msg_sending(self) -> Self:
```

### Comparing `bdmc-0.1.5.4/src/bdmc/modules/debug.py` & `bdmc-0.1.5.5/src/bdmc/modules/debug.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.4/src/bdmc/modules/logger.py` & `bdmc-0.1.5.5/src/bdmc/modules/logger.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.4/src/bdmc/modules/port.py` & `bdmc-0.1.5.5/src/bdmc/modules/port.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.4/src/bdmc/modules/seriald.py` & `bdmc-0.1.5.5/src/bdmc/modules/seriald.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.4/tests/find_tests.py` & `bdmc-0.1.5.5/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.4/tests/test_context.py` & `bdmc-0.1.5.5/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.4/tests/test_controller.py` & `bdmc-0.1.5.5/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.4/PKG-INFO` & `bdmc-0.1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdmc
-Version: 0.1.5.4
+Version: 0.1.5.5
 Summary: An api wrapper lib designed for the uptech BDMC divers
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: pyserial>=3.5
 Requires-Dist: coloredlogs>=15.0.1
 Description-Content-Type: text/markdown
```

