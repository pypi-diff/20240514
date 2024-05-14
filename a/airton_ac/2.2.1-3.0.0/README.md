# Comparing `tmp/airton_ac-2.2.1.tar.gz` & `tmp/airton_ac-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airton_ac-2.2.1.tar", max compression
+gzip compressed data, was "airton_ac-3.0.0.tar", max compression
```

## Comparing `airton_ac-2.2.1.tar` & `airton_ac-3.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-04-14 20:37:58.403951 airton_ac-2.2.1/LICENSE
--rw-r--r--   0        0        0     2621 2024-04-14 20:37:58.403951 airton_ac-2.2.1/README.md
--rw-r--r--   0        0        0       67 2024-04-14 20:37:58.403951 airton_ac-2.2.1/airton_ac/__init__.py
--rw-r--r--   0        0        0     4684 2024-04-14 20:37:58.403951 airton_ac-2.2.1/airton_ac/device.py
--rw-r--r--   0        0        0        0 2024-04-14 20:37:58.403951 airton_ac-2.2.1/airton_ac/domoticz/__init__.py
--rw-r--r--   0        0        0     5141 2024-04-14 20:37:58.403951 airton_ac-2.2.1/airton_ac/domoticz/install.py
--rw-r--r--   0        0        0        0 2024-04-14 20:37:58.403951 airton_ac-2.2.1/airton_ac/py.typed
--rw-r--r--   0        0        0     1071 2024-04-14 20:37:58.403951 airton_ac-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     3449 1970-01-01 00:00:00.000000 airton_ac-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-14 08:44:18.266449 airton_ac-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2621 2024-05-14 08:44:18.266449 airton_ac-3.0.0/README.md
+-rw-r--r--   0        0        0       67 2024-05-14 08:44:18.266449 airton_ac-3.0.0/airton_ac/__init__.py
+-rw-r--r--   0        0        0     4507 2024-05-14 08:44:18.266449 airton_ac-3.0.0/airton_ac/device.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:44:18.266449 airton_ac-3.0.0/airton_ac/domoticz/__init__.py
+-rw-r--r--   0        0        0     5141 2024-05-14 08:44:18.266449 airton_ac-3.0.0/airton_ac/domoticz/install.py
+-rw-r--r--   0        0        0        0 2024-05-14 08:44:18.266449 airton_ac-3.0.0/airton_ac/py.typed
+-rw-r--r--   0        0        0     1070 2024-05-14 08:44:18.266449 airton_ac-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 airton_ac-3.0.0/PKG-INFO
```

### Comparing `airton_ac-2.2.1/LICENSE` & `airton_ac-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airton_ac-2.2.1/README.md` & `airton_ac-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `airton_ac-2.2.1/airton_ac/device.py` & `airton_ac-3.0.0/airton_ac/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Callable, Optional
 
 from local_tuya import (
     Constraint,
     Constraints,
     DataPoint,
     Device,
     DeviceConfig,
@@ -73,23 +72,18 @@
             and values[ACDataPoint.SWING_DIRECTION] == ACDataPoint.SWING,
             sleep=bool(values[ACDataPoint.SLEEP]),
             health=bool(values[ACDataPoint.HEALTH]),
         )
 
 
 class ACDevice(Device[ACState]):
-    def __init__(
-        self,
-        config: DeviceConfig,
-        state_updated_callback: Optional[Callable[[ACState], Any]] = None,
-    ):
+    def __init__(self, config: DeviceConfig):
         super().__init__(
             config,
             ACState.load,
-            state_updated_callback,
             constraints=Constraints(
                 Constraint(
                     ACDataPoint.ECO,
                     True,
                     (ACDataPoint.SET_POINT, None),
                     (ACDataPoint.FAN, {ACFanSpeed.TURBO}),
                     (ACDataPoint.SLEEP, None),
```

### Comparing `airton_ac-2.2.1/airton_ac/domoticz/install.py` & `airton_ac-3.0.0/airton_ac/domoticz/install.py`

 * *Files identical despite different names*

### Comparing `airton_ac-2.2.1/pyproject.toml` & `airton_ac-3.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "airton_ac"
-version = "2.2.1"
+version = "3.0.0"
 description = "Control an Airton AC device over LAN."
 authors = ["Gabriel Pajot <gab@les-cactus.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/airton-ac"
 include = ["airton_ac/py.typed"]
 exclude = ["airton_ac/domoticz/types.py"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 
-local-tuya = ">=2.1,<3"
-local-tuya-domoticz-tools = { version = ">=1.1,<2", optional = true }
+local-tuya = ">=3,<4"
+local-tuya-domoticz-tools = { version = ">=1.2,<2", optional = true }
 
 [tool.poetry.extras]
 domoticz = ["local-tuya-domoticz-tools"]
 
 [tool.poetry.group.test.dependencies]
-pytest = "==8.1.1"
+pytest = "==8.2.0"
 pytest-asyncio = "==0.23.6"
 pytest-mock = "==3.14.0"
-ruff = "==0.3.7"
-mypy = "==1.9.0"
+ruff = "==0.4.4"
+mypy = "==1.10.0"
 pre-commit = "==3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
```

### Comparing `airton_ac-2.2.1/PKG-INFO` & `airton_ac-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: airton_ac
-Version: 2.2.1
+Version: 3.0.0
 Summary: Control an Airton AC device over LAN.
 Home-page: https://github.com/gpajot/airton-ac
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@les-cactus.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: domoticz
-Requires-Dist: local-tuya (>=2.1,<3)
-Requires-Dist: local-tuya-domoticz-tools (>=1.1,<2) ; extra == "domoticz"
+Requires-Dist: local-tuya (>=3,<4)
+Requires-Dist: local-tuya-domoticz-tools (>=1.2,<2) ; extra == "domoticz"
 Project-URL: Repository, https://github.com/gpajot/airton-ac
 Description-Content-Type: text/markdown
 
 # airton-ac
 
 [![tests](https://github.com/gpajot/airton-ac/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/airton-ac/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
 [![version](https://img.shields.io/pypi/v/airton_ac?label=stable)](https://pypi.org/project/airton_ac/)
```

