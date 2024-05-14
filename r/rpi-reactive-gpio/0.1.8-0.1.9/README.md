# Comparing `tmp/rpi_reactive_gpio-0.1.8.tar.gz` & `tmp/rpi_reactive_gpio-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi_reactive_gpio-0.1.8.tar", max compression
+gzip compressed data, was "rpi_reactive_gpio-0.1.9.tar", max compression
```

## Comparing `rpi_reactive_gpio-0.1.8.tar` & `rpi_reactive_gpio-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-07-20 18:29:51.210267 rpi_reactive_gpio-0.1.8/LICENSE
--rw-r--r--   0        0        0       80 2023-07-20 18:29:51.210267 rpi_reactive_gpio-0.1.8/README.md
--rw-r--r--   0        0        0      768 2023-07-20 18:30:15.362476 rpi_reactive_gpio-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      207 2023-07-20 18:29:51.214267 rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/__init__.py
--rw-r--r--   0        0        0     1607 2023-07-20 18:29:51.214267 rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/buttons.py
--rw-r--r--   0        0        0     3534 2023-07-20 18:29:51.214267 rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/leds.py
--rw-r--r--   0        0        0      482 2023-07-20 18:29:51.214267 rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/main.py
--rw-r--r--   0        0        0      850 2023-07-20 18:29:51.214267 rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/pin_manager.py
--rw-r--r--   0        0        0     1263 2023-07-20 18:29:51.214267 rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/scene.py
--rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-09-12 05:22:18.277144 rpi_reactive_gpio-0.1.9/LICENSE
+-rw-r--r--   0        0        0       80 2023-09-12 05:22:18.277144 rpi_reactive_gpio-0.1.9/README.md
+-rw-r--r--   0        0        0      768 2023-09-12 05:22:44.529279 rpi_reactive_gpio-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-09-12 05:22:18.277144 rpi_reactive_gpio-0.1.9/rpi_reactive_gpio/__init__.py
+-rw-r--r--   0        0        0     1607 2023-09-12 05:22:18.277144 rpi_reactive_gpio-0.1.9/rpi_reactive_gpio/buttons.py
+-rw-r--r--   0        0        0     3534 2023-09-12 05:22:18.277144 rpi_reactive_gpio-0.1.9/rpi_reactive_gpio/leds.py
+-rw-r--r--   0        0        0      482 2023-09-12 05:22:18.277144 rpi_reactive_gpio-0.1.9/rpi_reactive_gpio/main.py
+-rw-r--r--   0        0        0      850 2023-09-12 05:22:18.277144 rpi_reactive_gpio-0.1.9/rpi_reactive_gpio/pin_manager.py
+-rw-r--r--   0        0        0     1281 2023-09-12 05:22:18.281144 rpi_reactive_gpio-0.1.9/rpi_reactive_gpio/scene.py
+-rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.9/PKG-INFO
```

### Comparing `rpi_reactive_gpio-0.1.8/LICENSE` & `rpi_reactive_gpio-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.8/pyproject.toml` & `rpi_reactive_gpio-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpi-reactive-gpio"
-version = "0.1.8"
+version = "0.1.9"
 description = "Syntax sugar for controlling RPi.GPIO with reactive design."
 authors = ["MarkParker5 <markparker.it@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rpi_reactive_gpio"}]
 homepage = "https://pypi.org/project/rpi-reactive-gpio/"
 repository = "https://github.com/MarkParker5/rpi-reactive-gpio"
```

### Comparing `rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/buttons.py` & `rpi_reactive_gpio-0.1.9/rpi_reactive_gpio/buttons.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/leds.py` & `rpi_reactive_gpio-0.1.9/rpi_reactive_gpio/leds.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/pin_manager.py` & `rpi_reactive_gpio-0.1.9/rpi_reactive_gpio/pin_manager.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/scene.py` & `rpi_reactive_gpio-0.1.9/rpi_reactive_gpio/scene.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     
     _is_running = False
     
     def main_loop(self, update_interval: float = 1.0, ticks_count: int = 100):
         self._is_running = True
         
         attributes = [getattr(self, a) for a in dir(self)]
-        self.managers = filter(lambda a: isinstance(a, PinManagerProtocol), attributes)
-        self.tickables = filter(lambda a: isinstance(a, Tickable), attributes)
-        self.events = filter(lambda a: isinstance(a, ButtonClick), attributes)
+        self.managers = list(filter(lambda a: isinstance(a, PinManagerProtocol), attributes))
+        self.tickables = list(filter(lambda a: isinstance(a, Tickable), attributes))
+        self.events = list(filter(lambda a: isinstance(a, ButtonClick), attributes))
         
         for event in self.events:
             event.pass_args = [self]
         
         while self._is_running:
             self._update_all()
             for i in range(ticks_count):
```

### Comparing `rpi_reactive_gpio-0.1.8/PKG-INFO` & `rpi_reactive_gpio-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-reactive-gpio
-Version: 0.1.8
+Version: 0.1.9
 Summary: Syntax sugar for controlling RPi.GPIO with reactive design.
 Home-page: https://pypi.org/project/rpi-reactive-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,reactive,rxpy,rx,rpi,rpi-gpio,RPi.GPIO
 Author: MarkParker5
 Author-email: markparker.it@gmail.com
 Requires-Python: >=3.10,<4.0
```

