# Comparing `tmp/arducam_config_parser-0.1.1.tar.gz` & `tmp/arducam_config_parser-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arducam_config_parser-0.1.1.tar", last modified: Fri Jan 21 08:55:12 2022, max compression
+gzip compressed data, was "arducam_config_parser-0.1.2.tar", last modified: Tue May 14 09:16:55 2024, max compression
```

## Comparing `arducam_config_parser-0.1.1.tar` & `arducam_config_parser-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-21 08:55:12.183888 arducam_config_parser-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-01-21 08:55:12.183888 arducam_config_parser-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-21 08:55:12.179888 arducam_config_parser-0.1.1/arducam_config_parser/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/arducam_config_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3498 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/arducam_config_parser/arducam_config_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-21 08:55:12.179888 arducam_config_parser-0.1.1/arducam_config_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-01-21 08:55:12.000000 arducam_config_parser-0.1.1/arducam_config_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-01-21 08:55:12.000000 arducam_config_parser-0.1.1/arducam_config_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-21 08:55:12.000000 arducam_config_parser-0.1.1/arducam_config_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-21 08:55:12.000000 arducam_config_parser-0.1.1/arducam_config_parser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-21 08:55:12.179888 arducam_config_parser-0.1.1/msvc/
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/msvc/arducam_config_parser.sln
--rw-r--r--   0 runner    (1001) docker     (121)     8302 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/msvc/arducam_config_parser.vcxproj
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/msvc/arducam_config_parser.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-01-21 08:55:12.183888 arducam_config_parser-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-21 08:55:12.183888 arducam_config_parser-0.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/src/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/src/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     8028 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/src/arducam_config_parser.c
--rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/src/arducam_config_parser.h
--rw-r--r--   0 runner    (1001) docker     (121)     9239 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/src/ini.c
--rw-r--r--   0 runner    (1001) docker     (121)     4932 2022-01-21 08:55:05.000000 arducam_config_parser-0.1.1/src/ini.h
+drwxrwxrwx   0        0        0        0 2024-05-14 09:16:55.630155 arducam_config_parser-0.1.2/
+-rw-rw-rw-   0        0        0       44 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      877 2024-05-14 09:16:55.630155 arducam_config_parser-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 09:16:55.614539 arducam_config_parser-0.1.2/arducam_config_parser/
+-rw-rw-rw-   0        0        0       38 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/arducam_config_parser/__init__.py
+-rw-rw-rw-   0        0        0     3616 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/arducam_config_parser/arducam_config_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:16:55.630155 arducam_config_parser-0.1.2/arducam_config_parser.egg-info/
+-rw-rw-rw-   0        0        0      877 2024-05-14 09:16:55.000000 arducam_config_parser-0.1.2/arducam_config_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2024-05-14 09:16:55.000000 arducam_config_parser-0.1.2/arducam_config_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 09:16:55.000000 arducam_config_parser-0.1.2/arducam_config_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-14 09:16:55.000000 arducam_config_parser-0.1.2/arducam_config_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 09:16:55.614539 arducam_config_parser-0.1.2/msvc/
+-rw-rw-rw-   0        0        0     1454 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/msvc/arducam_config_parser.sln
+-rw-rw-rw-   0        0        0     8473 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/msvc/arducam_config_parser.vcxproj
+-rw-rw-rw-   0        0        0     1296 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/msvc/arducam_config_parser.vcxproj.filters
+-rw-rw-rw-   0        0        0       70 2024-05-14 09:16:55.630155 arducam_config_parser-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1979 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:16:55.630155 arducam_config_parser-0.1.2/src/
+-rw-rw-rw-   0        0        0     3035 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/src/LICENSE.txt
+-rw-rw-rw-   0        0        0     1119 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/src/Makefile
+-rw-rw-rw-   0        0        0     8273 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/src/arducam_config_parser.c
+-rw-rw-rw-   0        0        0     3297 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/src/arducam_config_parser.h
+drwxrwxrwx   0        0        0        0 2024-05-14 09:16:55.630155 arducam_config_parser-0.1.2/src/debian/
+-rw-rw-rw-   0        0        0      469 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/src/debian/changelog
+-rw-rw-rw-   0        0        0        3 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/src/debian/compat
+-rw-rw-rw-   0        0        0      375 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/src/debian/control
+-rw-rw-rw-   0        0        0       44 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/src/debian/copyright
+-rw-rw-rw-   0        0        0      185 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/src/debian/rules
+drwxrwxrwx   0        0        0        0 2024-05-14 09:16:55.630155 arducam_config_parser-0.1.2/src/debian/source/
+-rw-rw-rw-   0        0        0       12 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/src/debian/source/format
+-rw-rw-rw-   0        0        0     9562 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/src/ini.c
+-rw-rw-rw-   0        0        0     5084 2024-05-14 09:16:31.000000 arducam_config_parser-0.1.2/src/ini.h
```

### Comparing `arducam_config_parser-0.1.1/arducam_config_parser/arducam_config_parser.py` & `arducam_config_parser-0.1.2/arducam_config_parser/arducam_config_parser.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-# -*- coding: utf-8 -*-
-from ctypes import *
-import sys, os
-import platform
-
-try:
-    abs_path = os.path.dirname(os.path.abspath(__file__))
-    if platform.system() == "Windows":
-        lib_name = "arducam_config_parser.dll"
-    elif platform.system() == "Linux":
-        lib_name = "libarducam_config_parser.so"
-
-    abs_lib_name = os.path.join(abs_path, lib_name)
-    if os.path.exists(abs_lib_name):
-        _lib = cdll.LoadLibrary(abs_lib_name)
-    else:
-        _lib = cdll.LoadLibrary(lib_name)
-except Exception as e:
-    print("Load libarducam_config_parser fail.")
-    print("Make sure you have arducam_config_parser installed.")
-    print(
-        "For more information, please visit: https://github.com/ArduCAM/arducam_config_parser"
-    )
-    print(e)
-    sys.exit(0)
-
-
-MAX_CONFIGS = 8192
-SECTION_TYPE_CAMERA = 0x01 << 24
-SECTION_TYPE_BOARD = 0x02 << 24
-SECTION_TYPE_REG = 0x03 << 24
-
-SECTION_TYPE_BOARD_2 = SECTION_TYPE_BOARD | (0x02 << 16)
-SECTION_TYPE_BOARD_3_2 = SECTION_TYPE_BOARD | (0x04 << 16)
-SECTION_TYPE_BOARD_3_3 = SECTION_TYPE_BOARD | (0x03 << 16)
-SECTION_TYPE_REG_3_2 = SECTION_TYPE_REG | (0x04 << 16)
-SECTION_TYPE_REG_3_3 = SECTION_TYPE_REG | (0x03 << 16)
-
-CONFIG_TYPE_REG = 0x0001
-CONFIG_TYPE_VRCMD = 0x0002
-CONFIG_TYPE_DELAY = 0x0003
-
-# +───────────────+───────────+──────────────+
-# |     8bit      |    8bit   |    16bit     |
-# +───────────────+───────────+──────────────+
-# | section type  | usb type  | config type  |
-# +───────────────+───────────+──────────────+
-
-
-class Config(Structure):
-    _fields_ = [
-        ("type", c_uint32),
-        ("params", c_uint32 * 16),
-        ("params_length", c_uint8),
-    ]
-
-
-class Control(Structure):
-    _fields_ = [
-        ("min", c_int64),
-        ("max", c_int64),
-        ("step", c_int32),
-        ("def", c_int64),
-        ("flags", c_uint32),
-        ("name", c_char * 128),
-        ("func", c_char * 128),
-        ("code", c_char_p),
-    ]
-
-
-class CameraParam(Structure):
-    _fields_ = [
-        ("cfg_mode", c_uint32),
-        ("type", c_char * 50),
-        ("width", c_uint32),
-        ("height", c_uint32),
-        ("bit_width", c_uint8),
-        ("format", c_uint16),
-        ("i2c_mode", c_uint8),
-        ("i2c_addr", c_uint16),
-        ("trans_lvl", c_uint32),
-    ]
-
-    def getdict(struct):
-        return dict(
-            (
-                field.upper(),
-                getattr(struct, field)
-                if field != "format"
-                else (struct.format >> 8, struct.format & 0xFF),
-            )
-            for field, _ in struct._fields_
-        )
-
-
-class CameraConfigs(Structure):
-    _fields_ = [
-        ("camera_param", CameraParam),
-        ("configs", POINTER(Config)),
-        ("configs_length", c_uint32),
-        ("controls", POINTER(Control)),
-        ("controls_length", c_uint32),
-    ]
-
-
-parse = _lib.arducam_parse_config
-parse.argtypes = [c_char_p, POINTER(CameraConfigs)]
-
-
-def LoadConfigFile(name):
-    cfgs = CameraConfigs()
-    if sys.version_info[0] == 3:
-        filename = name.encode('gbk') if platform.system() == "Windows" else name.encode('utf-8')
-    else:
-        filename = name
-    if parse(filename, byref(cfgs)) != 0:
-        raise RuntimeError("Loading configuration file {} failed.".format(name))
-    return cfgs
+# -*- coding: utf-8 -*-
+from ctypes import *
+import sys, os
+import platform
+
+try:
+    abs_path = os.path.dirname(os.path.abspath(__file__))
+    if platform.system() == "Windows":
+        lib_name = "arducam_config_parser.dll"
+    elif platform.system() == "Linux":
+        lib_name = "libarducam_config_parser.so"
+
+    abs_lib_name = os.path.join(abs_path, lib_name)
+    if os.path.exists(abs_lib_name):
+        _lib = cdll.LoadLibrary(abs_lib_name)
+    else:
+        _lib = cdll.LoadLibrary(lib_name)
+except Exception as e:
+    print("Load libarducam_config_parser fail.")
+    print("Make sure you have arducam_config_parser installed.")
+    print(
+        "For more information, please visit: https://github.com/ArduCAM/arducam_config_parser"
+    )
+    print(e)
+    sys.exit(0)
+
+
+MAX_CONFIGS = 8192
+SECTION_TYPE_CAMERA = 0x01 << 24
+SECTION_TYPE_BOARD = 0x02 << 24
+SECTION_TYPE_REG = 0x03 << 24
+
+SECTION_TYPE_BOARD_2 = SECTION_TYPE_BOARD | (0x02 << 16)
+SECTION_TYPE_BOARD_3_2 = SECTION_TYPE_BOARD | (0x04 << 16)
+SECTION_TYPE_BOARD_3_3 = SECTION_TYPE_BOARD | (0x03 << 16)
+SECTION_TYPE_REG_3_2 = SECTION_TYPE_REG | (0x04 << 16)
+SECTION_TYPE_REG_3_3 = SECTION_TYPE_REG | (0x03 << 16)
+
+CONFIG_TYPE_REG = 0x0001
+CONFIG_TYPE_VRCMD = 0x0002
+CONFIG_TYPE_DELAY = 0x0003
+
+# +───────────────+───────────+──────────────+
+# |     8bit      |    8bit   |    16bit     |
+# +───────────────+───────────+──────────────+
+# | section type  | usb type  | config type  |
+# +───────────────+───────────+──────────────+
+
+
+class Config(Structure):
+    _fields_ = [
+        ("type", c_uint32),
+        ("params", c_uint32 * 16),
+        ("params_length", c_uint8),
+    ]
+
+
+class Control(Structure):
+    _fields_ = [
+        ("min", c_int64),
+        ("max", c_int64),
+        ("step", c_int32),
+        ("def", c_int64),
+        ("flags", c_uint32),
+        ("name", c_char * 128),
+        ("func", c_char * 128),
+        ("code", c_char_p),
+    ]
+
+
+class CameraParam(Structure):
+    _fields_ = [
+        ("cfg_mode", c_uint32),
+        ("type", c_char * 50),
+        ("width", c_uint32),
+        ("height", c_uint32),
+        ("bit_width", c_uint8),
+        ("format", c_uint16),
+        ("i2c_mode", c_uint8),
+        ("i2c_addr", c_uint16),
+        ("trans_lvl", c_uint32),
+    ]
+
+    def getdict(struct):
+        return dict(
+            (
+                field.upper(),
+                getattr(struct, field)
+                if field != "format"
+                else (struct.format >> 8, struct.format & 0xFF),
+            )
+            for field, _ in struct._fields_
+        )
+
+
+class CameraConfigs(Structure):
+    _fields_ = [
+        ("camera_param", CameraParam),
+        ("configs", POINTER(Config)),
+        ("configs_length", c_uint32),
+        ("controls", POINTER(Control)),
+        ("controls_length", c_uint32),
+    ]
+
+
+parse = _lib.arducam_parse_config
+parse.argtypes = [c_char_p, POINTER(CameraConfigs)]
+
+
+def LoadConfigFile(name):
+    cfgs = CameraConfigs()
+    if sys.version_info[0] == 3:
+        filename = name.encode('gbk') if platform.system() == "Windows" else name.encode('utf-8')
+    else:
+        filename = name
+    if parse(filename, byref(cfgs)) != 0:
+        raise RuntimeError("Loading configuration file {} failed.".format(name))
+    return cfgs
```

### Comparing `arducam_config_parser-0.1.1/arducam_config_parser.egg-info/PKG-INFO` & `arducam_config_parser-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-Metadata-Version: 2.1
-Name: arducam-config-parser
-Version: 0.1.1
-Summary: arducam_config_parser is a python wrapper for dynamic libraries. 
-Home-page: https://github.com/ArduCAM/arducam_config_parser
-Author: ArduCam
-Author-email: support@arducam.com
-License: UNKNOWN
-Platform: Windows
-Platform: Linux
-Classifier: Programming Language :: Python
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Description-Content-Type: text/markdown
-
-## Introduction
-This project is based on the open source project [inih](https://github.com/benhoyt/inih), which is used to parse the .cfg format configuration file of ArduCam.
-
-Note: arducam_config_parser.py is a python wrapper for dynamic libraries. To use it, you need to install the dynamic library first.
-
-### Built
-```
-cd src
-make clean && make
-```
-
-### Installation
-`make install`
-
+Metadata-Version: 2.1
+Name: arducam_config_parser
+Version: 0.1.2
+Summary: arducam_config_parser is a python wrapper for dynamic libraries. 
+Home-page: https://github.com/ArduCAM/arducam_config_parser
+Author: ArduCam
+Author-email: support@arducam.com
+Platform: Windows
+Platform: Linux
+Classifier: Programming Language :: Python
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Description-Content-Type: text/markdown
+
+## Introduction
+This project is based on the open source project [inih](https://github.com/benhoyt/inih), which is used to parse the .cfg format configuration file of ArduCam.
+
+Note: arducam_config_parser.py is a python wrapper for dynamic libraries. To use it, you need to install the dynamic library first.
+
+### Built
+```
+cd src
+make clean && make
+```
+
+### Installation
+`sudo make install`
```

### Comparing `arducam_config_parser-0.1.1/msvc/arducam_config_parser.sln` & `arducam_config_parser-0.1.2/msvc/arducam_config_parser.sln`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-﻿
-Microsoft Visual Studio Solution File, Format Version 12.00
-# Visual Studio 15
-VisualStudioVersion = 15.0.28307.960
-MinimumVisualStudioVersion = 10.0.40219.1
-Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "arducam_config_parser", "arducam_config_parser.vcxproj", "{1F23EED4-4DE7-4191-9E28-C6C4363281F4}"
-EndProject
-Global
-	GlobalSection(SolutionConfigurationPlatforms) = preSolution
-		Debug|x64 = Debug|x64
-		Debug|x86 = Debug|x86
-		Release|x64 = Release|x64
-		Release|x86 = Release|x86
-	EndGlobalSection
-	GlobalSection(ProjectConfigurationPlatforms) = postSolution
-		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Debug|x64.ActiveCfg = Debug|x64
-		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Debug|x64.Build.0 = Debug|x64
-		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Debug|x86.ActiveCfg = Debug|Win32
-		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Debug|x86.Build.0 = Debug|Win32
-		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Release|x64.ActiveCfg = Release|x64
-		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Release|x64.Build.0 = Release|x64
-		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Release|x86.ActiveCfg = Release|Win32
-		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Release|x86.Build.0 = Release|Win32
-	EndGlobalSection
-	GlobalSection(SolutionProperties) = preSolution
-		HideSolutionNode = FALSE
-	EndGlobalSection
-	GlobalSection(ExtensibilityGlobals) = postSolution
-		SolutionGuid = {1E283DFE-3EB8-4AEB-A0F2-C8792833CF63}
-	EndGlobalSection
-EndGlobal
+﻿
+Microsoft Visual Studio Solution File, Format Version 12.00
+# Visual Studio 15
+VisualStudioVersion = 15.0.28307.960
+MinimumVisualStudioVersion = 10.0.40219.1
+Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "arducam_config_parser", "arducam_config_parser.vcxproj", "{1F23EED4-4DE7-4191-9E28-C6C4363281F4}"
+EndProject
+Global
+	GlobalSection(SolutionConfigurationPlatforms) = preSolution
+		Debug|x64 = Debug|x64
+		Debug|x86 = Debug|x86
+		Release|x64 = Release|x64
+		Release|x86 = Release|x86
+	EndGlobalSection
+	GlobalSection(ProjectConfigurationPlatforms) = postSolution
+		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Debug|x64.ActiveCfg = Debug|x64
+		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Debug|x64.Build.0 = Debug|x64
+		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Debug|x86.ActiveCfg = Debug|Win32
+		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Debug|x86.Build.0 = Debug|Win32
+		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Release|x64.ActiveCfg = Release|x64
+		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Release|x64.Build.0 = Release|x64
+		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Release|x86.ActiveCfg = Release|Win32
+		{1F23EED4-4DE7-4191-9E28-C6C4363281F4}.Release|x86.Build.0 = Release|Win32
+	EndGlobalSection
+	GlobalSection(SolutionProperties) = preSolution
+		HideSolutionNode = FALSE
+	EndGlobalSection
+	GlobalSection(ExtensibilityGlobals) = postSolution
+		SolutionGuid = {1E283DFE-3EB8-4AEB-A0F2-C8792833CF63}
+	EndGlobalSection
+EndGlobal
```

### Comparing `arducam_config_parser-0.1.1/msvc/arducam_config_parser.vcxproj` & `arducam_config_parser-0.1.2/msvc/arducam_config_parser.vcxproj`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 26% similar despite different names*

```diff
@@ -1,519 +1,530 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 7574  .0" encoding="ut
-00000020: 662d 3822 3f3e 0a3c 5072 6f6a 6563 7420  f-8"?>.<Project 
-00000030: 4465 6661 756c 7454 6172 6765 7473 3d22  DefaultTargets="
-00000040: 4275 696c 6422 2054 6f6f 6c73 5665 7273  Build" ToolsVers
-00000050: 696f 6e3d 2231 352e 3022 2078 6d6c 6e73  ion="15.0" xmlns
-00000060: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
-00000070: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f64  .microsoft.com/d
-00000080: 6576 656c 6f70 6572 2f6d 7362 7569 6c64  eveloper/msbuild
-00000090: 2f32 3030 3322 3e0a 2020 3c49 7465 6d47  /2003">.  <ItemG
-000000a0: 726f 7570 204c 6162 656c 3d22 5072 6f6a  roup Label="Proj
-000000b0: 6563 7443 6f6e 6669 6775 7261 7469 6f6e  ectConfiguration
-000000c0: 7322 3e0a 2020 2020 3c50 726f 6a65 6374  s">.    <Project
-000000d0: 436f 6e66 6967 7572 6174 696f 6e20 496e  Configuration In
-000000e0: 636c 7564 653d 2244 6562 7567 7c57 696e  clude="Debug|Win
-000000f0: 3332 223e 0a20 2020 2020 203c 436f 6e66  32">.      <Conf
-00000100: 6967 7572 6174 696f 6e3e 4465 6275 673c  iguration>Debug<
-00000110: 2f43 6f6e 6669 6775 7261 7469 6f6e 3e0a  /Configuration>.
-00000120: 2020 2020 2020 3c50 6c61 7466 6f72 6d3e        <Platform>
-00000130: 5769 6e33 323c 2f50 6c61 7466 6f72 6d3e  Win32</Platform>
-00000140: 0a20 2020 203c 2f50 726f 6a65 6374 436f  .    </ProjectCo
-00000150: 6e66 6967 7572 6174 696f 6e3e 0a20 2020  nfiguration>.   
-00000160: 203c 5072 6f6a 6563 7443 6f6e 6669 6775   <ProjectConfigu
-00000170: 7261 7469 6f6e 2049 6e63 6c75 6465 3d22  ration Include="
-00000180: 5265 6c65 6173 657c 5769 6e33 3222 3e0a  Release|Win32">.
-00000190: 2020 2020 2020 3c43 6f6e 6669 6775 7261        <Configura
-000001a0: 7469 6f6e 3e52 656c 6561 7365 3c2f 436f  tion>Release</Co
-000001b0: 6e66 6967 7572 6174 696f 6e3e 0a20 2020  nfiguration>.   
-000001c0: 2020 203c 506c 6174 666f 726d 3e57 696e     <Platform>Win
-000001d0: 3332 3c2f 506c 6174 666f 726d 3e0a 2020  32</Platform>.  
-000001e0: 2020 3c2f 5072 6f6a 6563 7443 6f6e 6669    </ProjectConfi
-000001f0: 6775 7261 7469 6f6e 3e0a 2020 2020 3c50  guration>.    <P
-00000200: 726f 6a65 6374 436f 6e66 6967 7572 6174  rojectConfigurat
-00000210: 696f 6e20 496e 636c 7564 653d 2244 6562  ion Include="Deb
-00000220: 7567 7c78 3634 223e 0a20 2020 2020 203c  ug|x64">.      <
-00000230: 436f 6e66 6967 7572 6174 696f 6e3e 4465  Configuration>De
-00000240: 6275 673c 2f43 6f6e 6669 6775 7261 7469  bug</Configurati
-00000250: 6f6e 3e0a 2020 2020 2020 3c50 6c61 7466  on>.      <Platf
-00000260: 6f72 6d3e 7836 343c 2f50 6c61 7466 6f72  orm>x64</Platfor
-00000270: 6d3e 0a20 2020 203c 2f50 726f 6a65 6374  m>.    </Project
-00000280: 436f 6e66 6967 7572 6174 696f 6e3e 0a20  Configuration>. 
-00000290: 2020 203c 5072 6f6a 6563 7443 6f6e 6669     <ProjectConfi
-000002a0: 6775 7261 7469 6f6e 2049 6e63 6c75 6465  guration Include
-000002b0: 3d22 5265 6c65 6173 657c 7836 3422 3e0a  ="Release|x64">.
-000002c0: 2020 2020 2020 3c43 6f6e 6669 6775 7261        <Configura
-000002d0: 7469 6f6e 3e52 656c 6561 7365 3c2f 436f  tion>Release</Co
-000002e0: 6e66 6967 7572 6174 696f 6e3e 0a20 2020  nfiguration>.   
-000002f0: 2020 203c 506c 6174 666f 726d 3e78 3634     <Platform>x64
-00000300: 3c2f 506c 6174 666f 726d 3e0a 2020 2020  </Platform>.    
-00000310: 3c2f 5072 6f6a 6563 7443 6f6e 6669 6775  </ProjectConfigu
-00000320: 7261 7469 6f6e 3e0a 2020 3c2f 4974 656d  ration>.  </Item
-00000330: 4772 6f75 703e 0a20 203c 4974 656d 4772  Group>.  <ItemGr
-00000340: 6f75 703e 0a20 2020 203c 436c 436f 6d70  oup>.    <ClComp
-00000350: 696c 6520 496e 636c 7564 653d 222e 2e5c  ile Include="..\
-00000360: 7372 635c 6172 6475 6361 6d5f 636f 6e66  src\arducam_conf
-00000370: 6967 5f70 6172 7365 722e 6322 202f 3e0a  ig_parser.c" />.
-00000380: 2020 2020 3c43 6c43 6f6d 7069 6c65 2049      <ClCompile I
-00000390: 6e63 6c75 6465 3d22 2e2e 5c73 7263 5c69  nclude="..\src\i
-000003a0: 6e69 2e63 2220 2f3e 0a20 203c 2f49 7465  ni.c" />.  </Ite
-000003b0: 6d47 726f 7570 3e0a 2020 3c49 7465 6d47  mGroup>.  <ItemG
-000003c0: 726f 7570 3e0a 2020 2020 3c43 6c49 6e63  roup>.    <ClInc
-000003d0: 6c75 6465 2049 6e63 6c75 6465 3d22 2e2e  lude Include="..
-000003e0: 5c73 7263 5c61 7264 7563 616d 5f63 6f6e  \src\arducam_con
-000003f0: 6669 675f 7061 7273 6572 2e68 2220 2f3e  fig_parser.h" />
-00000400: 0a20 2020 203c 436c 496e 636c 7564 6520  .    <ClInclude 
-00000410: 496e 636c 7564 653d 222e 2e5c 7372 635c  Include="..\src\
-00000420: 696e 692e 6822 202f 3e0a 2020 3c2f 4974  ini.h" />.  </It
-00000430: 656d 4772 6f75 703e 0a20 203c 5072 6f70  emGroup>.  <Prop
-00000440: 6572 7479 4772 6f75 7020 4c61 6265 6c3d  ertyGroup Label=
-00000450: 2247 6c6f 6261 6c73 223e 0a20 2020 203c  "Globals">.    <
-00000460: 5643 5072 6f6a 6563 7456 6572 7369 6f6e  VCProjectVersion
-00000470: 3e31 352e 303c 2f56 4350 726f 6a65 6374  >15.0</VCProject
-00000480: 5665 7273 696f 6e3e 0a20 2020 203c 5072  Version>.    <Pr
-00000490: 6f6a 6563 7447 7569 643e 7b31 4632 3345  ojectGuid>{1F23E
-000004a0: 4544 342d 3444 4537 2d34 3139 312d 3945  ED4-4DE7-4191-9E
-000004b0: 3238 2d43 3643 3433 3633 3238 3146 347d  28-C6C4363281F4}
-000004c0: 3c2f 5072 6f6a 6563 7447 7569 643e 0a20  </ProjectGuid>. 
-000004d0: 2020 203c 4b65 7977 6f72 643e 5769 6e33     <Keyword>Win3
-000004e0: 3250 726f 6a3c 2f4b 6579 776f 7264 3e0a  2Proj</Keyword>.
-000004f0: 2020 2020 3c52 6f6f 744e 616d 6573 7061      <RootNamespa
-00000500: 6365 3e61 7264 7563 616d 5f63 6f6e 6669  ce>arducam_confi
-00000510: 675f 7061 7273 6572 3c2f 526f 6f74 4e61  g_parser</RootNa
-00000520: 6d65 7370 6163 653e 0a20 2020 203c 5769  mespace>.    <Wi
-00000530: 6e64 6f77 7354 6172 6765 7450 6c61 7466  ndowsTargetPlatf
-00000540: 6f72 6d56 6572 7369 6f6e 3e31 302e 302e  ormVersion>10.0.
-00000550: 3137 3736 332e 303c 2f57 696e 646f 7773  17763.0</Windows
-00000560: 5461 7267 6574 506c 6174 666f 726d 5665  TargetPlatformVe
-00000570: 7273 696f 6e3e 0a20 203c 2f50 726f 7065  rsion>.  </Prope
-00000580: 7274 7947 726f 7570 3e0a 2020 3c49 6d70  rtyGroup>.  <Imp
-00000590: 6f72 7420 5072 6f6a 6563 743d 2224 2856  ort Project="$(V
-000005a0: 4354 6172 6765 7473 5061 7468 295c 4d69  CTargetsPath)\Mi
-000005b0: 6372 6f73 6f66 742e 4370 702e 4465 6661  crosoft.Cpp.Defa
-000005c0: 756c 742e 7072 6f70 7322 202f 3e0a 2020  ult.props" />.  
-000005d0: 3c50 726f 7065 7274 7947 726f 7570 2043  <PropertyGroup C
-000005e0: 6f6e 6469 7469 6f6e 3d22 2724 2843 6f6e  ondition="'$(Con
-000005f0: 6669 6775 7261 7469 6f6e 297c 2428 506c  figuration)|$(Pl
-00000600: 6174 666f 726d 2927 3d3d 2744 6562 7567  atform)'=='Debug
-00000610: 7c57 696e 3332 2722 204c 6162 656c 3d22  |Win32'" Label="
-00000620: 436f 6e66 6967 7572 6174 696f 6e22 3e0a  Configuration">.
-00000630: 2020 2020 3c43 6f6e 6669 6775 7261 7469      <Configurati
-00000640: 6f6e 5479 7065 3e44 796e 616d 6963 4c69  onType>DynamicLi
-00000650: 6272 6172 793c 2f43 6f6e 6669 6775 7261  brary</Configura
-00000660: 7469 6f6e 5479 7065 3e0a 2020 2020 3c55  tionType>.    <U
-00000670: 7365 4465 6275 674c 6962 7261 7269 6573  seDebugLibraries
-00000680: 3e74 7275 653c 2f55 7365 4465 6275 674c  >true</UseDebugL
-00000690: 6962 7261 7269 6573 3e0a 2020 2020 3c50  ibraries>.    <P
-000006a0: 6c61 7466 6f72 6d54 6f6f 6c73 6574 3e76  latformToolset>v
-000006b0: 3134 313c 2f50 6c61 7466 6f72 6d54 6f6f  141</PlatformToo
-000006c0: 6c73 6574 3e0a 2020 2020 3c43 6861 7261  lset>.    <Chara
-000006d0: 6374 6572 5365 743e 556e 6963 6f64 653c  cterSet>Unicode<
-000006e0: 2f43 6861 7261 6374 6572 5365 743e 0a20  /CharacterSet>. 
-000006f0: 203c 2f50 726f 7065 7274 7947 726f 7570   </PropertyGroup
-00000700: 3e0a 2020 3c50 726f 7065 7274 7947 726f  >.  <PropertyGro
-00000710: 7570 2043 6f6e 6469 7469 6f6e 3d22 2724  up Condition="'$
-00000720: 2843 6f6e 6669 6775 7261 7469 6f6e 297c  (Configuration)|
-00000730: 2428 506c 6174 666f 726d 2927 3d3d 2752  $(Platform)'=='R
-00000740: 656c 6561 7365 7c57 696e 3332 2722 204c  elease|Win32'" L
-00000750: 6162 656c 3d22 436f 6e66 6967 7572 6174  abel="Configurat
-00000760: 696f 6e22 3e0a 2020 2020 3c43 6f6e 6669  ion">.    <Confi
-00000770: 6775 7261 7469 6f6e 5479 7065 3e44 796e  gurationType>Dyn
-00000780: 616d 6963 4c69 6272 6172 793c 2f43 6f6e  amicLibrary</Con
-00000790: 6669 6775 7261 7469 6f6e 5479 7065 3e0a  figurationType>.
-000007a0: 2020 2020 3c55 7365 4465 6275 674c 6962      <UseDebugLib
-000007b0: 7261 7269 6573 3e66 616c 7365 3c2f 5573  raries>false</Us
-000007c0: 6544 6562 7567 4c69 6272 6172 6965 733e  eDebugLibraries>
-000007d0: 0a20 2020 203c 506c 6174 666f 726d 546f  .    <PlatformTo
-000007e0: 6f6c 7365 743e 7631 3431 3c2f 506c 6174  olset>v141</Plat
-000007f0: 666f 726d 546f 6f6c 7365 743e 0a20 2020  formToolset>.   
-00000800: 203c 5768 6f6c 6550 726f 6772 616d 4f70   <WholeProgramOp
-00000810: 7469 6d69 7a61 7469 6f6e 3e74 7275 653c  timization>true<
-00000820: 2f57 686f 6c65 5072 6f67 7261 6d4f 7074  /WholeProgramOpt
-00000830: 696d 697a 6174 696f 6e3e 0a20 2020 203c  imization>.    <
-00000840: 4368 6172 6163 7465 7253 6574 3e55 6e69  CharacterSet>Uni
-00000850: 636f 6465 3c2f 4368 6172 6163 7465 7253  code</CharacterS
-00000860: 6574 3e0a 2020 3c2f 5072 6f70 6572 7479  et>.  </Property
-00000870: 4772 6f75 703e 0a20 203c 5072 6f70 6572  Group>.  <Proper
-00000880: 7479 4772 6f75 7020 436f 6e64 6974 696f  tyGroup Conditio
-00000890: 6e3d 2227 2428 436f 6e66 6967 7572 6174  n="'$(Configurat
-000008a0: 696f 6e29 7c24 2850 6c61 7466 6f72 6d29  ion)|$(Platform)
-000008b0: 273d 3d27 4465 6275 677c 7836 3427 2220  '=='Debug|x64'" 
-000008c0: 4c61 6265 6c3d 2243 6f6e 6669 6775 7261  Label="Configura
-000008d0: 7469 6f6e 223e 0a20 2020 203c 436f 6e66  tion">.    <Conf
-000008e0: 6967 7572 6174 696f 6e54 7970 653e 4479  igurationType>Dy
-000008f0: 6e61 6d69 634c 6962 7261 7279 3c2f 436f  namicLibrary</Co
-00000900: 6e66 6967 7572 6174 696f 6e54 7970 653e  nfigurationType>
-00000910: 0a20 2020 203c 5573 6544 6562 7567 4c69  .    <UseDebugLi
-00000920: 6272 6172 6965 733e 7472 7565 3c2f 5573  braries>true</Us
-00000930: 6544 6562 7567 4c69 6272 6172 6965 733e  eDebugLibraries>
-00000940: 0a20 2020 203c 506c 6174 666f 726d 546f  .    <PlatformTo
-00000950: 6f6c 7365 743e 7631 3431 3c2f 506c 6174  olset>v141</Plat
-00000960: 666f 726d 546f 6f6c 7365 743e 0a20 2020  formToolset>.   
-00000970: 203c 4368 6172 6163 7465 7253 6574 3e55   <CharacterSet>U
-00000980: 6e69 636f 6465 3c2f 4368 6172 6163 7465  nicode</Characte
-00000990: 7253 6574 3e0a 2020 3c2f 5072 6f70 6572  rSet>.  </Proper
-000009a0: 7479 4772 6f75 703e 0a20 203c 5072 6f70  tyGroup>.  <Prop
-000009b0: 6572 7479 4772 6f75 7020 436f 6e64 6974  ertyGroup Condit
-000009c0: 696f 6e3d 2227 2428 436f 6e66 6967 7572  ion="'$(Configur
-000009d0: 6174 696f 6e29 7c24 2850 6c61 7466 6f72  ation)|$(Platfor
-000009e0: 6d29 273d 3d27 5265 6c65 6173 657c 7836  m)'=='Release|x6
-000009f0: 3427 2220 4c61 6265 6c3d 2243 6f6e 6669  4'" Label="Confi
-00000a00: 6775 7261 7469 6f6e 223e 0a20 2020 203c  guration">.    <
-00000a10: 436f 6e66 6967 7572 6174 696f 6e54 7970  ConfigurationTyp
-00000a20: 653e 4479 6e61 6d69 634c 6962 7261 7279  e>DynamicLibrary
-00000a30: 3c2f 436f 6e66 6967 7572 6174 696f 6e54  </ConfigurationT
-00000a40: 7970 653e 0a20 2020 203c 5573 6544 6562  ype>.    <UseDeb
-00000a50: 7567 4c69 6272 6172 6965 733e 6661 6c73  ugLibraries>fals
-00000a60: 653c 2f55 7365 4465 6275 674c 6962 7261  e</UseDebugLibra
-00000a70: 7269 6573 3e0a 2020 2020 3c50 6c61 7466  ries>.    <Platf
-00000a80: 6f72 6d54 6f6f 6c73 6574 3e76 3134 313c  ormToolset>v141<
-00000a90: 2f50 6c61 7466 6f72 6d54 6f6f 6c73 6574  /PlatformToolset
-00000aa0: 3e0a 2020 2020 3c57 686f 6c65 5072 6f67  >.    <WholeProg
-00000ab0: 7261 6d4f 7074 696d 697a 6174 696f 6e3e  ramOptimization>
-00000ac0: 7472 7565 3c2f 5768 6f6c 6550 726f 6772  true</WholeProgr
-00000ad0: 616d 4f70 7469 6d69 7a61 7469 6f6e 3e0a  amOptimization>.
-00000ae0: 2020 2020 3c43 6861 7261 6374 6572 5365      <CharacterSe
-00000af0: 743e 556e 6963 6f64 653c 2f43 6861 7261  t>Unicode</Chara
-00000b00: 6374 6572 5365 743e 0a20 203c 2f50 726f  cterSet>.  </Pro
-00000b10: 7065 7274 7947 726f 7570 3e0a 2020 3c49  pertyGroup>.  <I
-00000b20: 6d70 6f72 7420 5072 6f6a 6563 743d 2224  mport Project="$
-00000b30: 2856 4354 6172 6765 7473 5061 7468 295c  (VCTargetsPath)\
-00000b40: 4d69 6372 6f73 6f66 742e 4370 702e 7072  Microsoft.Cpp.pr
-00000b50: 6f70 7322 202f 3e0a 2020 3c49 6d70 6f72  ops" />.  <Impor
-00000b60: 7447 726f 7570 204c 6162 656c 3d22 4578  tGroup Label="Ex
-00000b70: 7465 6e73 696f 6e53 6574 7469 6e67 7322  tensionSettings"
-00000b80: 3e0a 2020 3c2f 496d 706f 7274 4772 6f75  >.  </ImportGrou
-00000b90: 703e 0a20 203c 496d 706f 7274 4772 6f75  p>.  <ImportGrou
-00000ba0: 7020 4c61 6265 6c3d 2253 6861 7265 6422  p Label="Shared"
-00000bb0: 3e0a 2020 3c2f 496d 706f 7274 4772 6f75  >.  </ImportGrou
-00000bc0: 703e 0a20 203c 496d 706f 7274 4772 6f75  p>.  <ImportGrou
-00000bd0: 7020 4c61 6265 6c3d 2250 726f 7065 7274  p Label="Propert
-00000be0: 7953 6865 6574 7322 2043 6f6e 6469 7469  ySheets" Conditi
-00000bf0: 6f6e 3d22 2724 2843 6f6e 6669 6775 7261  on="'$(Configura
-00000c00: 7469 6f6e 297c 2428 506c 6174 666f 726d  tion)|$(Platform
-00000c10: 2927 3d3d 2744 6562 7567 7c57 696e 3332  )'=='Debug|Win32
-00000c20: 2722 3e0a 2020 2020 3c49 6d70 6f72 7420  '">.    <Import 
-00000c30: 5072 6f6a 6563 743d 2224 2855 7365 7252  Project="$(UserR
-00000c40: 6f6f 7444 6972 295c 4d69 6372 6f73 6f66  ootDir)\Microsof
-00000c50: 742e 4370 702e 2428 506c 6174 666f 726d  t.Cpp.$(Platform
-00000c60: 292e 7573 6572 2e70 726f 7073 2220 436f  ).user.props" Co
-00000c70: 6e64 6974 696f 6e3d 2265 7869 7374 7328  ndition="exists(
-00000c80: 2724 2855 7365 7252 6f6f 7444 6972 295c  '$(UserRootDir)\
-00000c90: 4d69 6372 6f73 6f66 742e 4370 702e 2428  Microsoft.Cpp.$(
-00000ca0: 506c 6174 666f 726d 292e 7573 6572 2e70  Platform).user.p
-00000cb0: 726f 7073 2729 2220 4c61 6265 6c3d 224c  rops')" Label="L
-00000cc0: 6f63 616c 4170 7044 6174 6150 6c61 7466  ocalAppDataPlatf
-00000cd0: 6f72 6d22 202f 3e0a 2020 3c2f 496d 706f  orm" />.  </Impo
-00000ce0: 7274 4772 6f75 703e 0a20 203c 496d 706f  rtGroup>.  <Impo
-00000cf0: 7274 4772 6f75 7020 4c61 6265 6c3d 2250  rtGroup Label="P
-00000d00: 726f 7065 7274 7953 6865 6574 7322 2043  ropertySheets" C
-00000d10: 6f6e 6469 7469 6f6e 3d22 2724 2843 6f6e  ondition="'$(Con
-00000d20: 6669 6775 7261 7469 6f6e 297c 2428 506c  figuration)|$(Pl
-00000d30: 6174 666f 726d 2927 3d3d 2752 656c 6561  atform)'=='Relea
-00000d40: 7365 7c57 696e 3332 2722 3e0a 2020 2020  se|Win32'">.    
-00000d50: 3c49 6d70 6f72 7420 5072 6f6a 6563 743d  <Import Project=
-00000d60: 2224 2855 7365 7252 6f6f 7444 6972 295c  "$(UserRootDir)\
-00000d70: 4d69 6372 6f73 6f66 742e 4370 702e 2428  Microsoft.Cpp.$(
-00000d80: 506c 6174 666f 726d 292e 7573 6572 2e70  Platform).user.p
-00000d90: 726f 7073 2220 436f 6e64 6974 696f 6e3d  rops" Condition=
-00000da0: 2265 7869 7374 7328 2724 2855 7365 7252  "exists('$(UserR
-00000db0: 6f6f 7444 6972 295c 4d69 6372 6f73 6f66  ootDir)\Microsof
-00000dc0: 742e 4370 702e 2428 506c 6174 666f 726d  t.Cpp.$(Platform
-00000dd0: 292e 7573 6572 2e70 726f 7073 2729 2220  ).user.props')" 
-00000de0: 4c61 6265 6c3d 224c 6f63 616c 4170 7044  Label="LocalAppD
-00000df0: 6174 6150 6c61 7466 6f72 6d22 202f 3e0a  ataPlatform" />.
-00000e00: 2020 3c2f 496d 706f 7274 4772 6f75 703e    </ImportGroup>
-00000e10: 0a20 203c 496d 706f 7274 4772 6f75 7020  .  <ImportGroup 
-00000e20: 4c61 6265 6c3d 2250 726f 7065 7274 7953  Label="PropertyS
-00000e30: 6865 6574 7322 2043 6f6e 6469 7469 6f6e  heets" Condition
-00000e40: 3d22 2724 2843 6f6e 6669 6775 7261 7469  ="'$(Configurati
-00000e50: 6f6e 297c 2428 506c 6174 666f 726d 2927  on)|$(Platform)'
-00000e60: 3d3d 2744 6562 7567 7c78 3634 2722 3e0a  =='Debug|x64'">.
-00000e70: 2020 2020 3c49 6d70 6f72 7420 5072 6f6a      <Import Proj
-00000e80: 6563 743d 2224 2855 7365 7252 6f6f 7444  ect="$(UserRootD
-00000e90: 6972 295c 4d69 6372 6f73 6f66 742e 4370  ir)\Microsoft.Cp
-00000ea0: 702e 2428 506c 6174 666f 726d 292e 7573  p.$(Platform).us
-00000eb0: 6572 2e70 726f 7073 2220 436f 6e64 6974  er.props" Condit
-00000ec0: 696f 6e3d 2265 7869 7374 7328 2724 2855  ion="exists('$(U
-00000ed0: 7365 7252 6f6f 7444 6972 295c 4d69 6372  serRootDir)\Micr
-00000ee0: 6f73 6f66 742e 4370 702e 2428 506c 6174  osoft.Cpp.$(Plat
-00000ef0: 666f 726d 292e 7573 6572 2e70 726f 7073  form).user.props
-00000f00: 2729 2220 4c61 6265 6c3d 224c 6f63 616c  ')" Label="Local
-00000f10: 4170 7044 6174 6150 6c61 7466 6f72 6d22  AppDataPlatform"
-00000f20: 202f 3e0a 2020 3c2f 496d 706f 7274 4772   />.  </ImportGr
-00000f30: 6f75 703e 0a20 203c 496d 706f 7274 4772  oup>.  <ImportGr
-00000f40: 6f75 7020 4c61 6265 6c3d 2250 726f 7065  oup Label="Prope
-00000f50: 7274 7953 6865 6574 7322 2043 6f6e 6469  rtySheets" Condi
-00000f60: 7469 6f6e 3d22 2724 2843 6f6e 6669 6775  tion="'$(Configu
-00000f70: 7261 7469 6f6e 297c 2428 506c 6174 666f  ration)|$(Platfo
-00000f80: 726d 2927 3d3d 2752 656c 6561 7365 7c78  rm)'=='Release|x
-00000f90: 3634 2722 3e0a 2020 2020 3c49 6d70 6f72  64'">.    <Impor
-00000fa0: 7420 5072 6f6a 6563 743d 2224 2855 7365  t Project="$(Use
-00000fb0: 7252 6f6f 7444 6972 295c 4d69 6372 6f73  rRootDir)\Micros
-00000fc0: 6f66 742e 4370 702e 2428 506c 6174 666f  oft.Cpp.$(Platfo
-00000fd0: 726d 292e 7573 6572 2e70 726f 7073 2220  rm).user.props" 
-00000fe0: 436f 6e64 6974 696f 6e3d 2265 7869 7374  Condition="exist
-00000ff0: 7328 2724 2855 7365 7252 6f6f 7444 6972  s('$(UserRootDir
-00001000: 295c 4d69 6372 6f73 6f66 742e 4370 702e  )\Microsoft.Cpp.
-00001010: 2428 506c 6174 666f 726d 292e 7573 6572  $(Platform).user
-00001020: 2e70 726f 7073 2729 2220 4c61 6265 6c3d  .props')" Label=
-00001030: 224c 6f63 616c 4170 7044 6174 6150 6c61  "LocalAppDataPla
-00001040: 7466 6f72 6d22 202f 3e0a 2020 3c2f 496d  tform" />.  </Im
-00001050: 706f 7274 4772 6f75 703e 0a20 203c 5072  portGroup>.  <Pr
-00001060: 6f70 6572 7479 4772 6f75 7020 4c61 6265  opertyGroup Labe
-00001070: 6c3d 2255 7365 724d 6163 726f 7322 202f  l="UserMacros" /
-00001080: 3e0a 2020 3c50 726f 7065 7274 7947 726f  >.  <PropertyGro
-00001090: 7570 2043 6f6e 6469 7469 6f6e 3d22 2724  up Condition="'$
-000010a0: 2843 6f6e 6669 6775 7261 7469 6f6e 297c  (Configuration)|
-000010b0: 2428 506c 6174 666f 726d 2927 3d3d 2744  $(Platform)'=='D
-000010c0: 6562 7567 7c57 696e 3332 2722 3e0a 2020  ebug|Win32'">.  
-000010d0: 2020 3c4c 696e 6b49 6e63 7265 6d65 6e74    <LinkIncrement
-000010e0: 616c 3e74 7275 653c 2f4c 696e 6b49 6e63  al>true</LinkInc
-000010f0: 7265 6d65 6e74 616c 3e0a 2020 2020 3c4f  remental>.    <O
-00001100: 7574 4469 723e 2428 536f 6c75 7469 6f6e  utDir>$(Solution
-00001110: 4469 7229 2e2e 5c62 696e 5c24 2850 6c61  Dir)..\bin\$(Pla
-00001120: 7466 6f72 6d29 5c24 2843 6f6e 6669 6775  tform)\$(Configu
-00001130: 7261 7469 6f6e 295c 3c2f 4f75 7444 6972  ration)\</OutDir
-00001140: 3e0a 2020 2020 3c49 6e74 4469 723e 2428  >.    <IntDir>$(
-00001150: 536f 6c75 7469 6f6e 4469 7229 2e2e 5c6f  SolutionDir)..\o
-00001160: 626a 5c24 2850 6c61 7466 6f72 6d29 5c24  bj\$(Platform)\$
-00001170: 2843 6f6e 6669 6775 7261 7469 6f6e 295c  (Configuration)\
-00001180: 3c2f 496e 7444 6972 3e0a 2020 3c2f 5072  </IntDir>.  </Pr
-00001190: 6f70 6572 7479 4772 6f75 703e 0a20 203c  opertyGroup>.  <
-000011a0: 5072 6f70 6572 7479 4772 6f75 7020 436f  PropertyGroup Co
-000011b0: 6e64 6974 696f 6e3d 2227 2428 436f 6e66  ndition="'$(Conf
-000011c0: 6967 7572 6174 696f 6e29 7c24 2850 6c61  iguration)|$(Pla
-000011d0: 7466 6f72 6d29 273d 3d27 4465 6275 677c  tform)'=='Debug|
-000011e0: 7836 3427 223e 0a20 2020 203c 4c69 6e6b  x64'">.    <Link
-000011f0: 496e 6372 656d 656e 7461 6c3e 7472 7565  Incremental>true
-00001200: 3c2f 4c69 6e6b 496e 6372 656d 656e 7461  </LinkIncrementa
-00001210: 6c3e 0a20 2020 203c 4f75 7444 6972 3e24  l>.    <OutDir>$
-00001220: 2853 6f6c 7574 696f 6e44 6972 292e 2e5c  (SolutionDir)..\
-00001230: 6269 6e5c 2428 506c 6174 666f 726d 295c  bin\$(Platform)\
-00001240: 2428 436f 6e66 6967 7572 6174 696f 6e29  $(Configuration)
-00001250: 5c3c 2f4f 7574 4469 723e 0a20 2020 203c  \</OutDir>.    <
-00001260: 496e 7444 6972 3e24 2853 6f6c 7574 696f  IntDir>$(Solutio
-00001270: 6e44 6972 292e 2e5c 6f62 6a5c 2428 506c  nDir)..\obj\$(Pl
-00001280: 6174 666f 726d 295c 2428 436f 6e66 6967  atform)\$(Config
-00001290: 7572 6174 696f 6e29 5c3c 2f49 6e74 4469  uration)\</IntDi
-000012a0: 723e 0a20 203c 2f50 726f 7065 7274 7947  r>.  </PropertyG
-000012b0: 726f 7570 3e0a 2020 3c50 726f 7065 7274  roup>.  <Propert
-000012c0: 7947 726f 7570 2043 6f6e 6469 7469 6f6e  yGroup Condition
-000012d0: 3d22 2724 2843 6f6e 6669 6775 7261 7469  ="'$(Configurati
-000012e0: 6f6e 297c 2428 506c 6174 666f 726d 2927  on)|$(Platform)'
-000012f0: 3d3d 2752 656c 6561 7365 7c57 696e 3332  =='Release|Win32
-00001300: 2722 3e0a 2020 2020 3c4c 696e 6b49 6e63  '">.    <LinkInc
-00001310: 7265 6d65 6e74 616c 3e66 616c 7365 3c2f  remental>false</
-00001320: 4c69 6e6b 496e 6372 656d 656e 7461 6c3e  LinkIncremental>
-00001330: 0a20 2020 203c 4f75 7444 6972 3e24 2853  .    <OutDir>$(S
-00001340: 6f6c 7574 696f 6e44 6972 292e 2e5c 6269  olutionDir)..\bi
-00001350: 6e5c 2428 506c 6174 666f 726d 295c 2428  n\$(Platform)\$(
-00001360: 436f 6e66 6967 7572 6174 696f 6e29 5c3c  Configuration)\<
-00001370: 2f4f 7574 4469 723e 0a20 2020 203c 496e  /OutDir>.    <In
-00001380: 7444 6972 3e24 2853 6f6c 7574 696f 6e44  tDir>$(SolutionD
-00001390: 6972 292e 2e5c 6f62 6a5c 2428 506c 6174  ir)..\obj\$(Plat
-000013a0: 666f 726d 295c 2428 436f 6e66 6967 7572  form)\$(Configur
-000013b0: 6174 696f 6e29 5c3c 2f49 6e74 4469 723e  ation)\</IntDir>
-000013c0: 0a20 203c 2f50 726f 7065 7274 7947 726f  .  </PropertyGro
-000013d0: 7570 3e0a 2020 3c50 726f 7065 7274 7947  up>.  <PropertyG
-000013e0: 726f 7570 2043 6f6e 6469 7469 6f6e 3d22  roup Condition="
-000013f0: 2724 2843 6f6e 6669 6775 7261 7469 6f6e  '$(Configuration
-00001400: 297c 2428 506c 6174 666f 726d 2927 3d3d  )|$(Platform)'==
-00001410: 2752 656c 6561 7365 7c78 3634 2722 3e0a  'Release|x64'">.
-00001420: 2020 2020 3c4c 696e 6b49 6e63 7265 6d65      <LinkIncreme
-00001430: 6e74 616c 3e66 616c 7365 3c2f 4c69 6e6b  ntal>false</Link
-00001440: 496e 6372 656d 656e 7461 6c3e 0a20 2020  Incremental>.   
-00001450: 203c 4f75 7444 6972 3e24 2853 6f6c 7574   <OutDir>$(Solut
-00001460: 696f 6e44 6972 292e 2e5c 6269 6e5c 2428  ionDir)..\bin\$(
-00001470: 506c 6174 666f 726d 295c 2428 436f 6e66  Platform)\$(Conf
-00001480: 6967 7572 6174 696f 6e29 5c3c 2f4f 7574  iguration)\</Out
-00001490: 4469 723e 0a20 2020 203c 496e 7444 6972  Dir>.    <IntDir
-000014a0: 3e24 2853 6f6c 7574 696f 6e44 6972 292e  >$(SolutionDir).
-000014b0: 2e5c 6f62 6a5c 2428 506c 6174 666f 726d  .\obj\$(Platform
-000014c0: 295c 2428 436f 6e66 6967 7572 6174 696f  )\$(Configuratio
-000014d0: 6e29 5c3c 2f49 6e74 4469 723e 0a20 203c  n)\</IntDir>.  <
-000014e0: 2f50 726f 7065 7274 7947 726f 7570 3e0a  /PropertyGroup>.
-000014f0: 2020 3c49 7465 6d44 6566 696e 6974 696f    <ItemDefinitio
-00001500: 6e47 726f 7570 2043 6f6e 6469 7469 6f6e  nGroup Condition
-00001510: 3d22 2724 2843 6f6e 6669 6775 7261 7469  ="'$(Configurati
-00001520: 6f6e 297c 2428 506c 6174 666f 726d 2927  on)|$(Platform)'
-00001530: 3d3d 2744 6562 7567 7c57 696e 3332 2722  =='Debug|Win32'"
-00001540: 3e0a 2020 2020 3c43 6c43 6f6d 7069 6c65  >.    <ClCompile
-00001550: 3e0a 2020 2020 2020 3c50 7265 636f 6d70  >.      <Precomp
-00001560: 696c 6564 4865 6164 6572 3e0a 2020 2020  iledHeader>.    
-00001570: 2020 3c2f 5072 6563 6f6d 7069 6c65 6448    </PrecompiledH
-00001580: 6561 6465 723e 0a20 2020 2020 203c 5761  eader>.      <Wa
-00001590: 726e 696e 674c 6576 656c 3e4c 6576 656c  rningLevel>Level
-000015a0: 333c 2f57 6172 6e69 6e67 4c65 7665 6c3e  3</WarningLevel>
-000015b0: 0a20 2020 2020 203c 4f70 7469 6d69 7a61  .      <Optimiza
-000015c0: 7469 6f6e 3e44 6973 6162 6c65 643c 2f4f  tion>Disabled</O
-000015d0: 7074 696d 697a 6174 696f 6e3e 0a20 2020  ptimization>.   
-000015e0: 2020 203c 5344 4c43 6865 636b 3e74 7275     <SDLCheck>tru
-000015f0: 653c 2f53 444c 4368 6563 6b3e 0a20 2020  e</SDLCheck>.   
-00001600: 2020 203c 5072 6570 726f 6365 7373 6f72     <Preprocessor
-00001610: 4465 6669 6e69 7469 6f6e 733e 5749 4e33  Definitions>WIN3
-00001620: 323b 5f44 4542 5547 3b5f 434f 4e53 4f4c  2;_DEBUG;_CONSOL
-00001630: 453b 2528 5072 6570 726f 6365 7373 6f72  E;%(Preprocessor
-00001640: 4465 6669 6e69 7469 6f6e 7329 3b41 5244  Definitions);ARD
-00001650: 5543 414d 5f44 4c4c 3c2f 5072 6570 726f  UCAM_DLL</Prepro
-00001660: 6365 7373 6f72 4465 6669 6e69 7469 6f6e  cessorDefinition
-00001670: 733e 0a20 2020 2020 203c 436f 6e66 6f72  s>.      <Confor
-00001680: 6d61 6e63 654d 6f64 653e 7472 7565 3c2f  manceMode>true</
-00001690: 436f 6e66 6f72 6d61 6e63 654d 6f64 653e  ConformanceMode>
-000016a0: 0a20 2020 203c 2f43 6c43 6f6d 7069 6c65  .    </ClCompile
-000016b0: 3e0a 2020 2020 3c4c 696e 6b3e 0a20 2020  >.    <Link>.   
-000016c0: 2020 203c 5375 6253 7973 7465 6d3e 436f     <SubSystem>Co
-000016d0: 6e73 6f6c 653c 2f53 7562 5379 7374 656d  nsole</SubSystem
-000016e0: 3e0a 2020 2020 2020 3c47 656e 6572 6174  >.      <Generat
-000016f0: 6544 6562 7567 496e 666f 726d 6174 696f  eDebugInformatio
-00001700: 6e3e 7472 7565 3c2f 4765 6e65 7261 7465  n>true</Generate
-00001710: 4465 6275 6749 6e66 6f72 6d61 7469 6f6e  DebugInformation
-00001720: 3e0a 2020 2020 3c2f 4c69 6e6b 3e0a 2020  >.    </Link>.  
-00001730: 3c2f 4974 656d 4465 6669 6e69 7469 6f6e  </ItemDefinition
-00001740: 4772 6f75 703e 0a20 203c 4974 656d 4465  Group>.  <ItemDe
-00001750: 6669 6e69 7469 6f6e 4772 6f75 7020 436f  finitionGroup Co
-00001760: 6e64 6974 696f 6e3d 2227 2428 436f 6e66  ndition="'$(Conf
-00001770: 6967 7572 6174 696f 6e29 7c24 2850 6c61  iguration)|$(Pla
-00001780: 7466 6f72 6d29 273d 3d27 4465 6275 677c  tform)'=='Debug|
-00001790: 7836 3427 223e 0a20 2020 203c 436c 436f  x64'">.    <ClCo
-000017a0: 6d70 696c 653e 0a20 2020 2020 203c 5072  mpile>.      <Pr
-000017b0: 6563 6f6d 7069 6c65 6448 6561 6465 723e  ecompiledHeader>
-000017c0: 0a20 2020 2020 203c 2f50 7265 636f 6d70  .      </Precomp
-000017d0: 696c 6564 4865 6164 6572 3e0a 2020 2020  iledHeader>.    
-000017e0: 2020 3c57 6172 6e69 6e67 4c65 7665 6c3e    <WarningLevel>
-000017f0: 4c65 7665 6c33 3c2f 5761 726e 696e 674c  Level3</WarningL
-00001800: 6576 656c 3e0a 2020 2020 2020 3c4f 7074  evel>.      <Opt
-00001810: 696d 697a 6174 696f 6e3e 4469 7361 626c  imization>Disabl
-00001820: 6564 3c2f 4f70 7469 6d69 7a61 7469 6f6e  ed</Optimization
-00001830: 3e0a 2020 2020 2020 3c53 444c 4368 6563  >.      <SDLChec
-00001840: 6b3e 7472 7565 3c2f 5344 4c43 6865 636b  k>true</SDLCheck
-00001850: 3e0a 2020 2020 2020 3c50 7265 7072 6f63  >.      <Preproc
-00001860: 6573 736f 7244 6566 696e 6974 696f 6e73  essorDefinitions
-00001870: 3e5f 4445 4255 473b 5f43 4f4e 534f 4c45  >_DEBUG;_CONSOLE
-00001880: 3b25 2850 7265 7072 6f63 6573 736f 7244  ;%(PreprocessorD
-00001890: 6566 696e 6974 696f 6e73 293b 4152 4455  efinitions);ARDU
-000018a0: 4341 4d5f 444c 4c3c 2f50 7265 7072 6f63  CAM_DLL</Preproc
-000018b0: 6573 736f 7244 6566 696e 6974 696f 6e73  essorDefinitions
-000018c0: 3e0a 2020 2020 2020 3c43 6f6e 666f 726d  >.      <Conform
-000018d0: 616e 6365 4d6f 6465 3e74 7275 653c 2f43  anceMode>true</C
-000018e0: 6f6e 666f 726d 616e 6365 4d6f 6465 3e0a  onformanceMode>.
-000018f0: 2020 2020 3c2f 436c 436f 6d70 696c 653e      </ClCompile>
-00001900: 0a20 2020 203c 4c69 6e6b 3e0a 2020 2020  .    <Link>.    
-00001910: 2020 3c53 7562 5379 7374 656d 3e43 6f6e    <SubSystem>Con
-00001920: 736f 6c65 3c2f 5375 6253 7973 7465 6d3e  sole</SubSystem>
-00001930: 0a20 2020 2020 203c 4765 6e65 7261 7465  .      <Generate
-00001940: 4465 6275 6749 6e66 6f72 6d61 7469 6f6e  DebugInformation
-00001950: 3e74 7275 653c 2f47 656e 6572 6174 6544  >true</GenerateD
-00001960: 6562 7567 496e 666f 726d 6174 696f 6e3e  ebugInformation>
-00001970: 0a20 2020 203c 2f4c 696e 6b3e 0a20 203c  .    </Link>.  <
-00001980: 2f49 7465 6d44 6566 696e 6974 696f 6e47  /ItemDefinitionG
-00001990: 726f 7570 3e0a 2020 3c49 7465 6d44 6566  roup>.  <ItemDef
-000019a0: 696e 6974 696f 6e47 726f 7570 2043 6f6e  initionGroup Con
-000019b0: 6469 7469 6f6e 3d22 2724 2843 6f6e 6669  dition="'$(Confi
-000019c0: 6775 7261 7469 6f6e 297c 2428 506c 6174  guration)|$(Plat
-000019d0: 666f 726d 2927 3d3d 2752 656c 6561 7365  form)'=='Release
-000019e0: 7c57 696e 3332 2722 3e0a 2020 2020 3c43  |Win32'">.    <C
-000019f0: 6c43 6f6d 7069 6c65 3e0a 2020 2020 2020  lCompile>.      
-00001a00: 3c50 7265 636f 6d70 696c 6564 4865 6164  <PrecompiledHead
-00001a10: 6572 3e0a 2020 2020 2020 3c2f 5072 6563  er>.      </Prec
-00001a20: 6f6d 7069 6c65 6448 6561 6465 723e 0a20  ompiledHeader>. 
-00001a30: 2020 2020 203c 5761 726e 696e 674c 6576       <WarningLev
-00001a40: 656c 3e4c 6576 656c 333c 2f57 6172 6e69  el>Level3</Warni
-00001a50: 6e67 4c65 7665 6c3e 0a20 2020 2020 203c  ngLevel>.      <
-00001a60: 4f70 7469 6d69 7a61 7469 6f6e 3e4d 6178  Optimization>Max
-00001a70: 5370 6565 643c 2f4f 7074 696d 697a 6174  Speed</Optimizat
-00001a80: 696f 6e3e 0a20 2020 2020 203c 4675 6e63  ion>.      <Func
-00001a90: 7469 6f6e 4c65 7665 6c4c 696e 6b69 6e67  tionLevelLinking
-00001aa0: 3e74 7275 653c 2f46 756e 6374 696f 6e4c  >true</FunctionL
-00001ab0: 6576 656c 4c69 6e6b 696e 673e 0a20 2020  evelLinking>.   
-00001ac0: 2020 203c 496e 7472 696e 7369 6346 756e     <IntrinsicFun
-00001ad0: 6374 696f 6e73 3e74 7275 653c 2f49 6e74  ctions>true</Int
-00001ae0: 7269 6e73 6963 4675 6e63 7469 6f6e 733e  rinsicFunctions>
-00001af0: 0a20 2020 2020 203c 5344 4c43 6865 636b  .      <SDLCheck
-00001b00: 3e74 7275 653c 2f53 444c 4368 6563 6b3e  >true</SDLCheck>
-00001b10: 0a20 2020 2020 203c 5072 6570 726f 6365  .      <Preproce
-00001b20: 7373 6f72 4465 6669 6e69 7469 6f6e 733e  ssorDefinitions>
-00001b30: 5749 4e33 323b 4e44 4542 5547 3b5f 434f  WIN32;NDEBUG;_CO
-00001b40: 4e53 4f4c 453b 2528 5072 6570 726f 6365  NSOLE;%(Preproce
-00001b50: 7373 6f72 4465 6669 6e69 7469 6f6e 7329  ssorDefinitions)
-00001b60: 3b41 5244 5543 414d 5f44 4c4c 3c2f 5072  ;ARDUCAM_DLL</Pr
-00001b70: 6570 726f 6365 7373 6f72 4465 6669 6e69  eprocessorDefini
-00001b80: 7469 6f6e 733e 0a20 2020 2020 203c 436f  tions>.      <Co
-00001b90: 6e66 6f72 6d61 6e63 654d 6f64 653e 7472  nformanceMode>tr
-00001ba0: 7565 3c2f 436f 6e66 6f72 6d61 6e63 654d  ue</ConformanceM
-00001bb0: 6f64 653e 0a20 2020 203c 2f43 6c43 6f6d  ode>.    </ClCom
-00001bc0: 7069 6c65 3e0a 2020 2020 3c4c 696e 6b3e  pile>.    <Link>
-00001bd0: 0a20 2020 2020 203c 5375 6253 7973 7465  .      <SubSyste
-00001be0: 6d3e 436f 6e73 6f6c 653c 2f53 7562 5379  m>Console</SubSy
-00001bf0: 7374 656d 3e0a 2020 2020 2020 3c45 6e61  stem>.      <Ena
-00001c00: 626c 6543 4f4d 4441 5446 6f6c 6469 6e67  bleCOMDATFolding
-00001c10: 3e74 7275 653c 2f45 6e61 626c 6543 4f4d  >true</EnableCOM
-00001c20: 4441 5446 6f6c 6469 6e67 3e0a 2020 2020  DATFolding>.    
-00001c30: 2020 3c4f 7074 696d 697a 6552 6566 6572    <OptimizeRefer
-00001c40: 656e 6365 733e 7472 7565 3c2f 4f70 7469  ences>true</Opti
-00001c50: 6d69 7a65 5265 6665 7265 6e63 6573 3e0a  mizeReferences>.
-00001c60: 2020 2020 2020 3c47 656e 6572 6174 6544        <GenerateD
-00001c70: 6562 7567 496e 666f 726d 6174 696f 6e3e  ebugInformation>
-00001c80: 7472 7565 3c2f 4765 6e65 7261 7465 4465  true</GenerateDe
-00001c90: 6275 6749 6e66 6f72 6d61 7469 6f6e 3e0a  bugInformation>.
-00001ca0: 2020 2020 3c2f 4c69 6e6b 3e0a 2020 3c2f      </Link>.  </
-00001cb0: 4974 656d 4465 6669 6e69 7469 6f6e 4772  ItemDefinitionGr
-00001cc0: 6f75 703e 0a20 203c 4974 656d 4465 6669  oup>.  <ItemDefi
-00001cd0: 6e69 7469 6f6e 4772 6f75 7020 436f 6e64  nitionGroup Cond
-00001ce0: 6974 696f 6e3d 2227 2428 436f 6e66 6967  ition="'$(Config
-00001cf0: 7572 6174 696f 6e29 7c24 2850 6c61 7466  uration)|$(Platf
-00001d00: 6f72 6d29 273d 3d27 5265 6c65 6173 657c  orm)'=='Release|
-00001d10: 7836 3427 223e 0a20 2020 203c 436c 436f  x64'">.    <ClCo
-00001d20: 6d70 696c 653e 0a20 2020 2020 203c 5072  mpile>.      <Pr
-00001d30: 6563 6f6d 7069 6c65 6448 6561 6465 723e  ecompiledHeader>
-00001d40: 0a20 2020 2020 203c 2f50 7265 636f 6d70  .      </Precomp
-00001d50: 696c 6564 4865 6164 6572 3e0a 2020 2020  iledHeader>.    
-00001d60: 2020 3c57 6172 6e69 6e67 4c65 7665 6c3e    <WarningLevel>
-00001d70: 4c65 7665 6c33 3c2f 5761 726e 696e 674c  Level3</WarningL
-00001d80: 6576 656c 3e0a 2020 2020 2020 3c4f 7074  evel>.      <Opt
-00001d90: 696d 697a 6174 696f 6e3e 4d61 7853 7065  imization>MaxSpe
-00001da0: 6564 3c2f 4f70 7469 6d69 7a61 7469 6f6e  ed</Optimization
-00001db0: 3e0a 2020 2020 2020 3c46 756e 6374 696f  >.      <Functio
-00001dc0: 6e4c 6576 656c 4c69 6e6b 696e 673e 7472  nLevelLinking>tr
-00001dd0: 7565 3c2f 4675 6e63 7469 6f6e 4c65 7665  ue</FunctionLeve
-00001de0: 6c4c 696e 6b69 6e67 3e0a 2020 2020 2020  lLinking>.      
-00001df0: 3c49 6e74 7269 6e73 6963 4675 6e63 7469  <IntrinsicFuncti
-00001e00: 6f6e 733e 7472 7565 3c2f 496e 7472 696e  ons>true</Intrin
-00001e10: 7369 6346 756e 6374 696f 6e73 3e0a 2020  sicFunctions>.  
-00001e20: 2020 2020 3c53 444c 4368 6563 6b3e 7472      <SDLCheck>tr
-00001e30: 7565 3c2f 5344 4c43 6865 636b 3e0a 2020  ue</SDLCheck>.  
-00001e40: 2020 2020 3c50 7265 7072 6f63 6573 736f      <Preprocesso
-00001e50: 7244 6566 696e 6974 696f 6e73 3e4e 4445  rDefinitions>NDE
-00001e60: 4255 473b 5f43 4f4e 534f 4c45 3b25 2850  BUG;_CONSOLE;%(P
-00001e70: 7265 7072 6f63 6573 736f 7244 6566 696e  reprocessorDefin
-00001e80: 6974 696f 6e73 293b 4152 4455 4341 4d5f  itions);ARDUCAM_
-00001e90: 444c 4c3c 2f50 7265 7072 6f63 6573 736f  DLL</Preprocesso
-00001ea0: 7244 6566 696e 6974 696f 6e73 3e0a 2020  rDefinitions>.  
-00001eb0: 2020 2020 3c43 6f6e 666f 726d 616e 6365      <Conformance
-00001ec0: 4d6f 6465 3e74 7275 653c 2f43 6f6e 666f  Mode>true</Confo
-00001ed0: 726d 616e 6365 4d6f 6465 3e0a 2020 2020  rmanceMode>.    
-00001ee0: 3c2f 436c 436f 6d70 696c 653e 0a20 2020  </ClCompile>.   
-00001ef0: 203c 4c69 6e6b 3e0a 2020 2020 2020 3c53   <Link>.      <S
-00001f00: 7562 5379 7374 656d 3e43 6f6e 736f 6c65  ubSystem>Console
-00001f10: 3c2f 5375 6253 7973 7465 6d3e 0a20 2020  </SubSystem>.   
-00001f20: 2020 203c 456e 6162 6c65 434f 4d44 4154     <EnableCOMDAT
-00001f30: 466f 6c64 696e 673e 7472 7565 3c2f 456e  Folding>true</En
-00001f40: 6162 6c65 434f 4d44 4154 466f 6c64 696e  ableCOMDATFoldin
-00001f50: 673e 0a20 2020 2020 203c 4f70 7469 6d69  g>.      <Optimi
-00001f60: 7a65 5265 6665 7265 6e63 6573 3e74 7275  zeReferences>tru
-00001f70: 653c 2f4f 7074 696d 697a 6552 6566 6572  e</OptimizeRefer
-00001f80: 656e 6365 733e 0a20 2020 2020 203c 4765  ences>.      <Ge
-00001f90: 6e65 7261 7465 4465 6275 6749 6e66 6f72  nerateDebugInfor
-00001fa0: 6d61 7469 6f6e 3e74 7275 653c 2f47 656e  mation>true</Gen
-00001fb0: 6572 6174 6544 6562 7567 496e 666f 726d  erateDebugInform
-00001fc0: 6174 696f 6e3e 0a20 2020 203c 2f4c 696e  ation>.    </Lin
-00001fd0: 6b3e 0a20 203c 2f49 7465 6d44 6566 696e  k>.  </ItemDefin
-00001fe0: 6974 696f 6e47 726f 7570 3e0a 2020 3c49  itionGroup>.  <I
-00001ff0: 6d70 6f72 7420 5072 6f6a 6563 743d 2224  mport Project="$
-00002000: 2856 4354 6172 6765 7473 5061 7468 295c  (VCTargetsPath)\
-00002010: 4d69 6372 6f73 6f66 742e 4370 702e 7461  Microsoft.Cpp.ta
-00002020: 7267 6574 7322 202f 3e0a 2020 3c49 6d70  rgets" />.  <Imp
-00002030: 6f72 7447 726f 7570 204c 6162 656c 3d22  ortGroup Label="
-00002040: 4578 7465 6e73 696f 6e54 6172 6765 7473  ExtensionTargets
-00002050: 223e 0a20 203c 2f49 6d70 6f72 7447 726f  ">.  </ImportGro
-00002060: 7570 3e0a 3c2f 5072 6f6a 6563 743e       up>.</Project>
+00000020: 662d 3822 3f3e 0d0a 3c50 726f 6a65 6374  f-8"?>..<Project
+00000030: 2044 6566 6175 6c74 5461 7267 6574 733d   DefaultTargets=
+00000040: 2242 7569 6c64 2220 546f 6f6c 7356 6572  "Build" ToolsVer
+00000050: 7369 6f6e 3d22 3135 2e30 2220 786d 6c6e  sion="15.0" xmln
+00000060: 733d 2268 7474 703a 2f2f 7363 6865 6d61  s="http://schema
+00000070: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
+00000080: 6465 7665 6c6f 7065 722f 6d73 6275 696c  developer/msbuil
+00000090: 642f 3230 3033 223e 0d0a 2020 3c49 7465  d/2003">..  <Ite
+000000a0: 6d47 726f 7570 204c 6162 656c 3d22 5072  mGroup Label="Pr
+000000b0: 6f6a 6563 7443 6f6e 6669 6775 7261 7469  ojectConfigurati
+000000c0: 6f6e 7322 3e0d 0a20 2020 203c 5072 6f6a  ons">..    <Proj
+000000d0: 6563 7443 6f6e 6669 6775 7261 7469 6f6e  ectConfiguration
+000000e0: 2049 6e63 6c75 6465 3d22 4465 6275 677c   Include="Debug|
+000000f0: 5769 6e33 3222 3e0d 0a20 2020 2020 203c  Win32">..      <
+00000100: 436f 6e66 6967 7572 6174 696f 6e3e 4465  Configuration>De
+00000110: 6275 673c 2f43 6f6e 6669 6775 7261 7469  bug</Configurati
+00000120: 6f6e 3e0d 0a20 2020 2020 203c 506c 6174  on>..      <Plat
+00000130: 666f 726d 3e57 696e 3332 3c2f 506c 6174  form>Win32</Plat
+00000140: 666f 726d 3e0d 0a20 2020 203c 2f50 726f  form>..    </Pro
+00000150: 6a65 6374 436f 6e66 6967 7572 6174 696f  jectConfiguratio
+00000160: 6e3e 0d0a 2020 2020 3c50 726f 6a65 6374  n>..    <Project
+00000170: 436f 6e66 6967 7572 6174 696f 6e20 496e  Configuration In
+00000180: 636c 7564 653d 2252 656c 6561 7365 7c57  clude="Release|W
+00000190: 696e 3332 223e 0d0a 2020 2020 2020 3c43  in32">..      <C
+000001a0: 6f6e 6669 6775 7261 7469 6f6e 3e52 656c  onfiguration>Rel
+000001b0: 6561 7365 3c2f 436f 6e66 6967 7572 6174  ease</Configurat
+000001c0: 696f 6e3e 0d0a 2020 2020 2020 3c50 6c61  ion>..      <Pla
+000001d0: 7466 6f72 6d3e 5769 6e33 323c 2f50 6c61  tform>Win32</Pla
+000001e0: 7466 6f72 6d3e 0d0a 2020 2020 3c2f 5072  tform>..    </Pr
+000001f0: 6f6a 6563 7443 6f6e 6669 6775 7261 7469  ojectConfigurati
+00000200: 6f6e 3e0d 0a20 2020 203c 5072 6f6a 6563  on>..    <Projec
+00000210: 7443 6f6e 6669 6775 7261 7469 6f6e 2049  tConfiguration I
+00000220: 6e63 6c75 6465 3d22 4465 6275 677c 7836  nclude="Debug|x6
+00000230: 3422 3e0d 0a20 2020 2020 203c 436f 6e66  4">..      <Conf
+00000240: 6967 7572 6174 696f 6e3e 4465 6275 673c  iguration>Debug<
+00000250: 2f43 6f6e 6669 6775 7261 7469 6f6e 3e0d  /Configuration>.
+00000260: 0a20 2020 2020 203c 506c 6174 666f 726d  .      <Platform
+00000270: 3e78 3634 3c2f 506c 6174 666f 726d 3e0d  >x64</Platform>.
+00000280: 0a20 2020 203c 2f50 726f 6a65 6374 436f  .    </ProjectCo
+00000290: 6e66 6967 7572 6174 696f 6e3e 0d0a 2020  nfiguration>..  
+000002a0: 2020 3c50 726f 6a65 6374 436f 6e66 6967    <ProjectConfig
+000002b0: 7572 6174 696f 6e20 496e 636c 7564 653d  uration Include=
+000002c0: 2252 656c 6561 7365 7c78 3634 223e 0d0a  "Release|x64">..
+000002d0: 2020 2020 2020 3c43 6f6e 6669 6775 7261        <Configura
+000002e0: 7469 6f6e 3e52 656c 6561 7365 3c2f 436f  tion>Release</Co
+000002f0: 6e66 6967 7572 6174 696f 6e3e 0d0a 2020  nfiguration>..  
+00000300: 2020 2020 3c50 6c61 7466 6f72 6d3e 7836      <Platform>x6
+00000310: 343c 2f50 6c61 7466 6f72 6d3e 0d0a 2020  4</Platform>..  
+00000320: 2020 3c2f 5072 6f6a 6563 7443 6f6e 6669    </ProjectConfi
+00000330: 6775 7261 7469 6f6e 3e0d 0a20 203c 2f49  guration>..  </I
+00000340: 7465 6d47 726f 7570 3e0d 0a20 203c 4974  temGroup>..  <It
+00000350: 656d 4772 6f75 703e 0d0a 2020 2020 3c43  emGroup>..    <C
+00000360: 6c43 6f6d 7069 6c65 2049 6e63 6c75 6465  lCompile Include
+00000370: 3d22 2e2e 5c73 7263 5c61 7264 7563 616d  ="..\src\arducam
+00000380: 5f63 6f6e 6669 675f 7061 7273 6572 2e63  _config_parser.c
+00000390: 2220 2f3e 0d0a 2020 2020 3c43 6c43 6f6d  " />..    <ClCom
+000003a0: 7069 6c65 2049 6e63 6c75 6465 3d22 2e2e  pile Include="..
+000003b0: 5c73 7263 5c69 6e69 2e63 2220 2f3e 0d0a  \src\ini.c" />..
+000003c0: 2020 3c2f 4974 656d 4772 6f75 703e 0d0a    </ItemGroup>..
+000003d0: 2020 3c49 7465 6d47 726f 7570 3e0d 0a20    <ItemGroup>.. 
+000003e0: 2020 203c 436c 496e 636c 7564 6520 496e     <ClInclude In
+000003f0: 636c 7564 653d 222e 2e5c 7372 635c 6172  clude="..\src\ar
+00000400: 6475 6361 6d5f 636f 6e66 6967 5f70 6172  ducam_config_par
+00000410: 7365 722e 6822 202f 3e0d 0a20 2020 203c  ser.h" />..    <
+00000420: 436c 496e 636c 7564 6520 496e 636c 7564  ClInclude Includ
+00000430: 653d 222e 2e5c 7372 635c 696e 692e 6822  e="..\src\ini.h"
+00000440: 202f 3e0d 0a20 203c 2f49 7465 6d47 726f   />..  </ItemGro
+00000450: 7570 3e0d 0a20 203c 5072 6f70 6572 7479  up>..  <Property
+00000460: 4772 6f75 7020 4c61 6265 6c3d 2247 6c6f  Group Label="Glo
+00000470: 6261 6c73 223e 0d0a 2020 2020 3c56 4350  bals">..    <VCP
+00000480: 726f 6a65 6374 5665 7273 696f 6e3e 3135  rojectVersion>15
+00000490: 2e30 3c2f 5643 5072 6f6a 6563 7456 6572  .0</VCProjectVer
+000004a0: 7369 6f6e 3e0d 0a20 2020 203c 5072 6f6a  sion>..    <Proj
+000004b0: 6563 7447 7569 643e 7b31 4632 3345 4544  ectGuid>{1F23EED
+000004c0: 342d 3444 4537 2d34 3139 312d 3945 3238  4-4DE7-4191-9E28
+000004d0: 2d43 3643 3433 3633 3238 3146 347d 3c2f  -C6C4363281F4}</
+000004e0: 5072 6f6a 6563 7447 7569 643e 0d0a 2020  ProjectGuid>..  
+000004f0: 2020 3c4b 6579 776f 7264 3e57 696e 3332    <Keyword>Win32
+00000500: 5072 6f6a 3c2f 4b65 7977 6f72 643e 0d0a  Proj</Keyword>..
+00000510: 2020 2020 3c52 6f6f 744e 616d 6573 7061      <RootNamespa
+00000520: 6365 3e61 7264 7563 616d 5f63 6f6e 6669  ce>arducam_confi
+00000530: 675f 7061 7273 6572 3c2f 526f 6f74 4e61  g_parser</RootNa
+00000540: 6d65 7370 6163 653e 0d0a 2020 2020 3c57  mespace>..    <W
+00000550: 696e 646f 7773 5461 7267 6574 506c 6174  indowsTargetPlat
+00000560: 666f 726d 5665 7273 696f 6e3e 3130 2e30  formVersion>10.0
+00000570: 2e31 3737 3633 2e30 3c2f 5769 6e64 6f77  .17763.0</Window
+00000580: 7354 6172 6765 7450 6c61 7466 6f72 6d56  sTargetPlatformV
+00000590: 6572 7369 6f6e 3e0d 0a20 203c 2f50 726f  ersion>..  </Pro
+000005a0: 7065 7274 7947 726f 7570 3e0d 0a20 203c  pertyGroup>..  <
+000005b0: 496d 706f 7274 2050 726f 6a65 6374 3d22  Import Project="
+000005c0: 2428 5643 5461 7267 6574 7350 6174 6829  $(VCTargetsPath)
+000005d0: 5c4d 6963 726f 736f 6674 2e43 7070 2e44  \Microsoft.Cpp.D
+000005e0: 6566 6175 6c74 2e70 726f 7073 2220 2f3e  efault.props" />
+000005f0: 0d0a 2020 3c50 726f 7065 7274 7947 726f  ..  <PropertyGro
+00000600: 7570 2043 6f6e 6469 7469 6f6e 3d22 2724  up Condition="'$
+00000610: 2843 6f6e 6669 6775 7261 7469 6f6e 297c  (Configuration)|
+00000620: 2428 506c 6174 666f 726d 2927 3d3d 2744  $(Platform)'=='D
+00000630: 6562 7567 7c57 696e 3332 2722 204c 6162  ebug|Win32'" Lab
+00000640: 656c 3d22 436f 6e66 6967 7572 6174 696f  el="Configuratio
+00000650: 6e22 3e0d 0a20 2020 203c 436f 6e66 6967  n">..    <Config
+00000660: 7572 6174 696f 6e54 7970 653e 4479 6e61  urationType>Dyna
+00000670: 6d69 634c 6962 7261 7279 3c2f 436f 6e66  micLibrary</Conf
+00000680: 6967 7572 6174 696f 6e54 7970 653e 0d0a  igurationType>..
+00000690: 2020 2020 3c55 7365 4465 6275 674c 6962      <UseDebugLib
+000006a0: 7261 7269 6573 3e74 7275 653c 2f55 7365  raries>true</Use
+000006b0: 4465 6275 674c 6962 7261 7269 6573 3e0d  DebugLibraries>.
+000006c0: 0a20 2020 203c 506c 6174 666f 726d 546f  .    <PlatformTo
+000006d0: 6f6c 7365 743e 7631 3431 3c2f 506c 6174  olset>v141</Plat
+000006e0: 666f 726d 546f 6f6c 7365 743e 0d0a 2020  formToolset>..  
+000006f0: 2020 3c43 6861 7261 6374 6572 5365 743e    <CharacterSet>
+00000700: 556e 6963 6f64 653c 2f43 6861 7261 6374  Unicode</Charact
+00000710: 6572 5365 743e 0d0a 2020 3c2f 5072 6f70  erSet>..  </Prop
+00000720: 6572 7479 4772 6f75 703e 0d0a 2020 3c50  ertyGroup>..  <P
+00000730: 726f 7065 7274 7947 726f 7570 2043 6f6e  ropertyGroup Con
+00000740: 6469 7469 6f6e 3d22 2724 2843 6f6e 6669  dition="'$(Confi
+00000750: 6775 7261 7469 6f6e 297c 2428 506c 6174  guration)|$(Plat
+00000760: 666f 726d 2927 3d3d 2752 656c 6561 7365  form)'=='Release
+00000770: 7c57 696e 3332 2722 204c 6162 656c 3d22  |Win32'" Label="
+00000780: 436f 6e66 6967 7572 6174 696f 6e22 3e0d  Configuration">.
+00000790: 0a20 2020 203c 436f 6e66 6967 7572 6174  .    <Configurat
+000007a0: 696f 6e54 7970 653e 4479 6e61 6d69 634c  ionType>DynamicL
+000007b0: 6962 7261 7279 3c2f 436f 6e66 6967 7572  ibrary</Configur
+000007c0: 6174 696f 6e54 7970 653e 0d0a 2020 2020  ationType>..    
+000007d0: 3c55 7365 4465 6275 674c 6962 7261 7269  <UseDebugLibrari
+000007e0: 6573 3e66 616c 7365 3c2f 5573 6544 6562  es>false</UseDeb
+000007f0: 7567 4c69 6272 6172 6965 733e 0d0a 2020  ugLibraries>..  
+00000800: 2020 3c50 6c61 7466 6f72 6d54 6f6f 6c73    <PlatformTools
+00000810: 6574 3e76 3134 313c 2f50 6c61 7466 6f72  et>v141</Platfor
+00000820: 6d54 6f6f 6c73 6574 3e0d 0a20 2020 203c  mToolset>..    <
+00000830: 5768 6f6c 6550 726f 6772 616d 4f70 7469  WholeProgramOpti
+00000840: 6d69 7a61 7469 6f6e 3e74 7275 653c 2f57  mization>true</W
+00000850: 686f 6c65 5072 6f67 7261 6d4f 7074 696d  holeProgramOptim
+00000860: 697a 6174 696f 6e3e 0d0a 2020 2020 3c43  ization>..    <C
+00000870: 6861 7261 6374 6572 5365 743e 556e 6963  haracterSet>Unic
+00000880: 6f64 653c 2f43 6861 7261 6374 6572 5365  ode</CharacterSe
+00000890: 743e 0d0a 2020 3c2f 5072 6f70 6572 7479  t>..  </Property
+000008a0: 4772 6f75 703e 0d0a 2020 3c50 726f 7065  Group>..  <Prope
+000008b0: 7274 7947 726f 7570 2043 6f6e 6469 7469  rtyGroup Conditi
+000008c0: 6f6e 3d22 2724 2843 6f6e 6669 6775 7261  on="'$(Configura
+000008d0: 7469 6f6e 297c 2428 506c 6174 666f 726d  tion)|$(Platform
+000008e0: 2927 3d3d 2744 6562 7567 7c78 3634 2722  )'=='Debug|x64'"
+000008f0: 204c 6162 656c 3d22 436f 6e66 6967 7572   Label="Configur
+00000900: 6174 696f 6e22 3e0d 0a20 2020 203c 436f  ation">..    <Co
+00000910: 6e66 6967 7572 6174 696f 6e54 7970 653e  nfigurationType>
+00000920: 4479 6e61 6d69 634c 6962 7261 7279 3c2f  DynamicLibrary</
+00000930: 436f 6e66 6967 7572 6174 696f 6e54 7970  ConfigurationTyp
+00000940: 653e 0d0a 2020 2020 3c55 7365 4465 6275  e>..    <UseDebu
+00000950: 674c 6962 7261 7269 6573 3e74 7275 653c  gLibraries>true<
+00000960: 2f55 7365 4465 6275 674c 6962 7261 7269  /UseDebugLibrari
+00000970: 6573 3e0d 0a20 2020 203c 506c 6174 666f  es>..    <Platfo
+00000980: 726d 546f 6f6c 7365 743e 7631 3431 3c2f  rmToolset>v141</
+00000990: 506c 6174 666f 726d 546f 6f6c 7365 743e  PlatformToolset>
+000009a0: 0d0a 2020 2020 3c43 6861 7261 6374 6572  ..    <Character
+000009b0: 5365 743e 556e 6963 6f64 653c 2f43 6861  Set>Unicode</Cha
+000009c0: 7261 6374 6572 5365 743e 0d0a 2020 3c2f  racterSet>..  </
+000009d0: 5072 6f70 6572 7479 4772 6f75 703e 0d0a  PropertyGroup>..
+000009e0: 2020 3c50 726f 7065 7274 7947 726f 7570    <PropertyGroup
+000009f0: 2043 6f6e 6469 7469 6f6e 3d22 2724 2843   Condition="'$(C
+00000a00: 6f6e 6669 6775 7261 7469 6f6e 297c 2428  onfiguration)|$(
+00000a10: 506c 6174 666f 726d 2927 3d3d 2752 656c  Platform)'=='Rel
+00000a20: 6561 7365 7c78 3634 2722 204c 6162 656c  ease|x64'" Label
+00000a30: 3d22 436f 6e66 6967 7572 6174 696f 6e22  ="Configuration"
+00000a40: 3e0d 0a20 2020 203c 436f 6e66 6967 7572  >..    <Configur
+00000a50: 6174 696f 6e54 7970 653e 4479 6e61 6d69  ationType>Dynami
+00000a60: 634c 6962 7261 7279 3c2f 436f 6e66 6967  cLibrary</Config
+00000a70: 7572 6174 696f 6e54 7970 653e 0d0a 2020  urationType>..  
+00000a80: 2020 3c55 7365 4465 6275 674c 6962 7261    <UseDebugLibra
+00000a90: 7269 6573 3e66 616c 7365 3c2f 5573 6544  ries>false</UseD
+00000aa0: 6562 7567 4c69 6272 6172 6965 733e 0d0a  ebugLibraries>..
+00000ab0: 2020 2020 3c50 6c61 7466 6f72 6d54 6f6f      <PlatformToo
+00000ac0: 6c73 6574 3e76 3134 313c 2f50 6c61 7466  lset>v141</Platf
+00000ad0: 6f72 6d54 6f6f 6c73 6574 3e0d 0a20 2020  ormToolset>..   
+00000ae0: 203c 5768 6f6c 6550 726f 6772 616d 4f70   <WholeProgramOp
+00000af0: 7469 6d69 7a61 7469 6f6e 3e74 7275 653c  timization>true<
+00000b00: 2f57 686f 6c65 5072 6f67 7261 6d4f 7074  /WholeProgramOpt
+00000b10: 696d 697a 6174 696f 6e3e 0d0a 2020 2020  imization>..    
+00000b20: 3c43 6861 7261 6374 6572 5365 743e 556e  <CharacterSet>Un
+00000b30: 6963 6f64 653c 2f43 6861 7261 6374 6572  icode</Character
+00000b40: 5365 743e 0d0a 2020 3c2f 5072 6f70 6572  Set>..  </Proper
+00000b50: 7479 4772 6f75 703e 0d0a 2020 3c49 6d70  tyGroup>..  <Imp
+00000b60: 6f72 7420 5072 6f6a 6563 743d 2224 2856  ort Project="$(V
+00000b70: 4354 6172 6765 7473 5061 7468 295c 4d69  CTargetsPath)\Mi
+00000b80: 6372 6f73 6f66 742e 4370 702e 7072 6f70  crosoft.Cpp.prop
+00000b90: 7322 202f 3e0d 0a20 203c 496d 706f 7274  s" />..  <Import
+00000ba0: 4772 6f75 7020 4c61 6265 6c3d 2245 7874  Group Label="Ext
+00000bb0: 656e 7369 6f6e 5365 7474 696e 6773 223e  ensionSettings">
+00000bc0: 0d0a 2020 3c2f 496d 706f 7274 4772 6f75  ..  </ImportGrou
+00000bd0: 703e 0d0a 2020 3c49 6d70 6f72 7447 726f  p>..  <ImportGro
+00000be0: 7570 204c 6162 656c 3d22 5368 6172 6564  up Label="Shared
+00000bf0: 223e 0d0a 2020 3c2f 496d 706f 7274 4772  ">..  </ImportGr
+00000c00: 6f75 703e 0d0a 2020 3c49 6d70 6f72 7447  oup>..  <ImportG
+00000c10: 726f 7570 204c 6162 656c 3d22 5072 6f70  roup Label="Prop
+00000c20: 6572 7479 5368 6565 7473 2220 436f 6e64  ertySheets" Cond
+00000c30: 6974 696f 6e3d 2227 2428 436f 6e66 6967  ition="'$(Config
+00000c40: 7572 6174 696f 6e29 7c24 2850 6c61 7466  uration)|$(Platf
+00000c50: 6f72 6d29 273d 3d27 4465 6275 677c 5769  orm)'=='Debug|Wi
+00000c60: 6e33 3227 223e 0d0a 2020 2020 3c49 6d70  n32'">..    <Imp
+00000c70: 6f72 7420 5072 6f6a 6563 743d 2224 2855  ort Project="$(U
+00000c80: 7365 7252 6f6f 7444 6972 295c 4d69 6372  serRootDir)\Micr
+00000c90: 6f73 6f66 742e 4370 702e 2428 506c 6174  osoft.Cpp.$(Plat
+00000ca0: 666f 726d 292e 7573 6572 2e70 726f 7073  form).user.props
+00000cb0: 2220 436f 6e64 6974 696f 6e3d 2265 7869  " Condition="exi
+00000cc0: 7374 7328 2724 2855 7365 7252 6f6f 7444  sts('$(UserRootD
+00000cd0: 6972 295c 4d69 6372 6f73 6f66 742e 4370  ir)\Microsoft.Cp
+00000ce0: 702e 2428 506c 6174 666f 726d 292e 7573  p.$(Platform).us
+00000cf0: 6572 2e70 726f 7073 2729 2220 4c61 6265  er.props')" Labe
+00000d00: 6c3d 224c 6f63 616c 4170 7044 6174 6150  l="LocalAppDataP
+00000d10: 6c61 7466 6f72 6d22 202f 3e0d 0a20 203c  latform" />..  <
+00000d20: 2f49 6d70 6f72 7447 726f 7570 3e0d 0a20  /ImportGroup>.. 
+00000d30: 203c 496d 706f 7274 4772 6f75 7020 4c61   <ImportGroup La
+00000d40: 6265 6c3d 2250 726f 7065 7274 7953 6865  bel="PropertyShe
+00000d50: 6574 7322 2043 6f6e 6469 7469 6f6e 3d22  ets" Condition="
+00000d60: 2724 2843 6f6e 6669 6775 7261 7469 6f6e  '$(Configuration
+00000d70: 297c 2428 506c 6174 666f 726d 2927 3d3d  )|$(Platform)'==
+00000d80: 2752 656c 6561 7365 7c57 696e 3332 2722  'Release|Win32'"
+00000d90: 3e0d 0a20 2020 203c 496d 706f 7274 2050  >..    <Import P
+00000da0: 726f 6a65 6374 3d22 2428 5573 6572 526f  roject="$(UserRo
+00000db0: 6f74 4469 7229 5c4d 6963 726f 736f 6674  otDir)\Microsoft
+00000dc0: 2e43 7070 2e24 2850 6c61 7466 6f72 6d29  .Cpp.$(Platform)
+00000dd0: 2e75 7365 722e 7072 6f70 7322 2043 6f6e  .user.props" Con
+00000de0: 6469 7469 6f6e 3d22 6578 6973 7473 2827  dition="exists('
+00000df0: 2428 5573 6572 526f 6f74 4469 7229 5c4d  $(UserRootDir)\M
+00000e00: 6963 726f 736f 6674 2e43 7070 2e24 2850  icrosoft.Cpp.$(P
+00000e10: 6c61 7466 6f72 6d29 2e75 7365 722e 7072  latform).user.pr
+00000e20: 6f70 7327 2922 204c 6162 656c 3d22 4c6f  ops')" Label="Lo
+00000e30: 6361 6c41 7070 4461 7461 506c 6174 666f  calAppDataPlatfo
+00000e40: 726d 2220 2f3e 0d0a 2020 3c2f 496d 706f  rm" />..  </Impo
+00000e50: 7274 4772 6f75 703e 0d0a 2020 3c49 6d70  rtGroup>..  <Imp
+00000e60: 6f72 7447 726f 7570 204c 6162 656c 3d22  ortGroup Label="
+00000e70: 5072 6f70 6572 7479 5368 6565 7473 2220  PropertySheets" 
+00000e80: 436f 6e64 6974 696f 6e3d 2227 2428 436f  Condition="'$(Co
+00000e90: 6e66 6967 7572 6174 696f 6e29 7c24 2850  nfiguration)|$(P
+00000ea0: 6c61 7466 6f72 6d29 273d 3d27 4465 6275  latform)'=='Debu
+00000eb0: 677c 7836 3427 223e 0d0a 2020 2020 3c49  g|x64'">..    <I
+00000ec0: 6d70 6f72 7420 5072 6f6a 6563 743d 2224  mport Project="$
+00000ed0: 2855 7365 7252 6f6f 7444 6972 295c 4d69  (UserRootDir)\Mi
+00000ee0: 6372 6f73 6f66 742e 4370 702e 2428 506c  crosoft.Cpp.$(Pl
+00000ef0: 6174 666f 726d 292e 7573 6572 2e70 726f  atform).user.pro
+00000f00: 7073 2220 436f 6e64 6974 696f 6e3d 2265  ps" Condition="e
+00000f10: 7869 7374 7328 2724 2855 7365 7252 6f6f  xists('$(UserRoo
+00000f20: 7444 6972 295c 4d69 6372 6f73 6f66 742e  tDir)\Microsoft.
+00000f30: 4370 702e 2428 506c 6174 666f 726d 292e  Cpp.$(Platform).
+00000f40: 7573 6572 2e70 726f 7073 2729 2220 4c61  user.props')" La
+00000f50: 6265 6c3d 224c 6f63 616c 4170 7044 6174  bel="LocalAppDat
+00000f60: 6150 6c61 7466 6f72 6d22 202f 3e0d 0a20  aPlatform" />.. 
+00000f70: 203c 2f49 6d70 6f72 7447 726f 7570 3e0d   </ImportGroup>.
+00000f80: 0a20 203c 496d 706f 7274 4772 6f75 7020  .  <ImportGroup 
+00000f90: 4c61 6265 6c3d 2250 726f 7065 7274 7953  Label="PropertyS
+00000fa0: 6865 6574 7322 2043 6f6e 6469 7469 6f6e  heets" Condition
+00000fb0: 3d22 2724 2843 6f6e 6669 6775 7261 7469  ="'$(Configurati
+00000fc0: 6f6e 297c 2428 506c 6174 666f 726d 2927  on)|$(Platform)'
+00000fd0: 3d3d 2752 656c 6561 7365 7c78 3634 2722  =='Release|x64'"
+00000fe0: 3e0d 0a20 2020 203c 496d 706f 7274 2050  >..    <Import P
+00000ff0: 726f 6a65 6374 3d22 2428 5573 6572 526f  roject="$(UserRo
+00001000: 6f74 4469 7229 5c4d 6963 726f 736f 6674  otDir)\Microsoft
+00001010: 2e43 7070 2e24 2850 6c61 7466 6f72 6d29  .Cpp.$(Platform)
+00001020: 2e75 7365 722e 7072 6f70 7322 2043 6f6e  .user.props" Con
+00001030: 6469 7469 6f6e 3d22 6578 6973 7473 2827  dition="exists('
+00001040: 2428 5573 6572 526f 6f74 4469 7229 5c4d  $(UserRootDir)\M
+00001050: 6963 726f 736f 6674 2e43 7070 2e24 2850  icrosoft.Cpp.$(P
+00001060: 6c61 7466 6f72 6d29 2e75 7365 722e 7072  latform).user.pr
+00001070: 6f70 7327 2922 204c 6162 656c 3d22 4c6f  ops')" Label="Lo
+00001080: 6361 6c41 7070 4461 7461 506c 6174 666f  calAppDataPlatfo
+00001090: 726d 2220 2f3e 0d0a 2020 3c2f 496d 706f  rm" />..  </Impo
+000010a0: 7274 4772 6f75 703e 0d0a 2020 3c50 726f  rtGroup>..  <Pro
+000010b0: 7065 7274 7947 726f 7570 204c 6162 656c  pertyGroup Label
+000010c0: 3d22 5573 6572 4d61 6372 6f73 2220 2f3e  ="UserMacros" />
+000010d0: 0d0a 2020 3c50 726f 7065 7274 7947 726f  ..  <PropertyGro
+000010e0: 7570 2043 6f6e 6469 7469 6f6e 3d22 2724  up Condition="'$
+000010f0: 2843 6f6e 6669 6775 7261 7469 6f6e 297c  (Configuration)|
+00001100: 2428 506c 6174 666f 726d 2927 3d3d 2744  $(Platform)'=='D
+00001110: 6562 7567 7c57 696e 3332 2722 3e0d 0a20  ebug|Win32'">.. 
+00001120: 2020 203c 4c69 6e6b 496e 6372 656d 656e     <LinkIncremen
+00001130: 7461 6c3e 7472 7565 3c2f 4c69 6e6b 496e  tal>true</LinkIn
+00001140: 6372 656d 656e 7461 6c3e 0d0a 2020 2020  cremental>..    
+00001150: 3c4f 7574 4469 723e 2428 536f 6c75 7469  <OutDir>$(Soluti
+00001160: 6f6e 4469 7229 2e2e 5c62 696e 5c24 2850  onDir)..\bin\$(P
+00001170: 6c61 7466 6f72 6d29 5c24 2843 6f6e 6669  latform)\$(Confi
+00001180: 6775 7261 7469 6f6e 295c 3c2f 4f75 7444  guration)\</OutD
+00001190: 6972 3e0d 0a20 2020 203c 496e 7444 6972  ir>..    <IntDir
+000011a0: 3e24 2853 6f6c 7574 696f 6e44 6972 292e  >$(SolutionDir).
+000011b0: 2e5c 6f62 6a5c 2428 506c 6174 666f 726d  .\obj\$(Platform
+000011c0: 295c 2428 436f 6e66 6967 7572 6174 696f  )\$(Configuratio
+000011d0: 6e29 5c3c 2f49 6e74 4469 723e 0d0a 2020  n)\</IntDir>..  
+000011e0: 3c2f 5072 6f70 6572 7479 4772 6f75 703e  </PropertyGroup>
+000011f0: 0d0a 2020 3c50 726f 7065 7274 7947 726f  ..  <PropertyGro
+00001200: 7570 2043 6f6e 6469 7469 6f6e 3d22 2724  up Condition="'$
+00001210: 2843 6f6e 6669 6775 7261 7469 6f6e 297c  (Configuration)|
+00001220: 2428 506c 6174 666f 726d 2927 3d3d 2744  $(Platform)'=='D
+00001230: 6562 7567 7c78 3634 2722 3e0d 0a20 2020  ebug|x64'">..   
+00001240: 203c 4c69 6e6b 496e 6372 656d 656e 7461   <LinkIncrementa
+00001250: 6c3e 7472 7565 3c2f 4c69 6e6b 496e 6372  l>true</LinkIncr
+00001260: 656d 656e 7461 6c3e 0d0a 2020 2020 3c4f  emental>..    <O
+00001270: 7574 4469 723e 2428 536f 6c75 7469 6f6e  utDir>$(Solution
+00001280: 4469 7229 2e2e 5c62 696e 5c24 2850 6c61  Dir)..\bin\$(Pla
+00001290: 7466 6f72 6d29 5c24 2843 6f6e 6669 6775  tform)\$(Configu
+000012a0: 7261 7469 6f6e 295c 3c2f 4f75 7444 6972  ration)\</OutDir
+000012b0: 3e0d 0a20 2020 203c 496e 7444 6972 3e24  >..    <IntDir>$
+000012c0: 2853 6f6c 7574 696f 6e44 6972 292e 2e5c  (SolutionDir)..\
+000012d0: 6f62 6a5c 2428 506c 6174 666f 726d 295c  obj\$(Platform)\
+000012e0: 2428 436f 6e66 6967 7572 6174 696f 6e29  $(Configuration)
+000012f0: 5c3c 2f49 6e74 4469 723e 0d0a 2020 3c2f  \</IntDir>..  </
+00001300: 5072 6f70 6572 7479 4772 6f75 703e 0d0a  PropertyGroup>..
+00001310: 2020 3c50 726f 7065 7274 7947 726f 7570    <PropertyGroup
+00001320: 2043 6f6e 6469 7469 6f6e 3d22 2724 2843   Condition="'$(C
+00001330: 6f6e 6669 6775 7261 7469 6f6e 297c 2428  onfiguration)|$(
+00001340: 506c 6174 666f 726d 2927 3d3d 2752 656c  Platform)'=='Rel
+00001350: 6561 7365 7c57 696e 3332 2722 3e0d 0a20  ease|Win32'">.. 
+00001360: 2020 203c 4c69 6e6b 496e 6372 656d 656e     <LinkIncremen
+00001370: 7461 6c3e 6661 6c73 653c 2f4c 696e 6b49  tal>false</LinkI
+00001380: 6e63 7265 6d65 6e74 616c 3e0d 0a20 2020  ncremental>..   
+00001390: 203c 4f75 7444 6972 3e24 2853 6f6c 7574   <OutDir>$(Solut
+000013a0: 696f 6e44 6972 292e 2e5c 6269 6e5c 2428  ionDir)..\bin\$(
+000013b0: 506c 6174 666f 726d 295c 2428 436f 6e66  Platform)\$(Conf
+000013c0: 6967 7572 6174 696f 6e29 5c3c 2f4f 7574  iguration)\</Out
+000013d0: 4469 723e 0d0a 2020 2020 3c49 6e74 4469  Dir>..    <IntDi
+000013e0: 723e 2428 536f 6c75 7469 6f6e 4469 7229  r>$(SolutionDir)
+000013f0: 2e2e 5c6f 626a 5c24 2850 6c61 7466 6f72  ..\obj\$(Platfor
+00001400: 6d29 5c24 2843 6f6e 6669 6775 7261 7469  m)\$(Configurati
+00001410: 6f6e 295c 3c2f 496e 7444 6972 3e0d 0a20  on)\</IntDir>.. 
+00001420: 203c 2f50 726f 7065 7274 7947 726f 7570   </PropertyGroup
+00001430: 3e0d 0a20 203c 5072 6f70 6572 7479 4772  >..  <PropertyGr
+00001440: 6f75 7020 436f 6e64 6974 696f 6e3d 2227  oup Condition="'
+00001450: 2428 436f 6e66 6967 7572 6174 696f 6e29  $(Configuration)
+00001460: 7c24 2850 6c61 7466 6f72 6d29 273d 3d27  |$(Platform)'=='
+00001470: 5265 6c65 6173 657c 7836 3427 223e 0d0a  Release|x64'">..
+00001480: 2020 2020 3c4c 696e 6b49 6e63 7265 6d65      <LinkIncreme
+00001490: 6e74 616c 3e66 616c 7365 3c2f 4c69 6e6b  ntal>false</Link
+000014a0: 496e 6372 656d 656e 7461 6c3e 0d0a 2020  Incremental>..  
+000014b0: 2020 3c4f 7574 4469 723e 2428 536f 6c75    <OutDir>$(Solu
+000014c0: 7469 6f6e 4469 7229 2e2e 5c62 696e 5c24  tionDir)..\bin\$
+000014d0: 2850 6c61 7466 6f72 6d29 5c24 2843 6f6e  (Platform)\$(Con
+000014e0: 6669 6775 7261 7469 6f6e 295c 3c2f 4f75  figuration)\</Ou
+000014f0: 7444 6972 3e0d 0a20 2020 203c 496e 7444  tDir>..    <IntD
+00001500: 6972 3e24 2853 6f6c 7574 696f 6e44 6972  ir>$(SolutionDir
+00001510: 292e 2e5c 6f62 6a5c 2428 506c 6174 666f  )..\obj\$(Platfo
+00001520: 726d 295c 2428 436f 6e66 6967 7572 6174  rm)\$(Configurat
+00001530: 696f 6e29 5c3c 2f49 6e74 4469 723e 0d0a  ion)\</IntDir>..
+00001540: 2020 3c2f 5072 6f70 6572 7479 4772 6f75    </PropertyGrou
+00001550: 703e 0d0a 2020 3c49 7465 6d44 6566 696e  p>..  <ItemDefin
+00001560: 6974 696f 6e47 726f 7570 2043 6f6e 6469  itionGroup Condi
+00001570: 7469 6f6e 3d22 2724 2843 6f6e 6669 6775  tion="'$(Configu
+00001580: 7261 7469 6f6e 297c 2428 506c 6174 666f  ration)|$(Platfo
+00001590: 726d 2927 3d3d 2744 6562 7567 7c57 696e  rm)'=='Debug|Win
+000015a0: 3332 2722 3e0d 0a20 2020 203c 436c 436f  32'">..    <ClCo
+000015b0: 6d70 696c 653e 0d0a 2020 2020 2020 3c50  mpile>..      <P
+000015c0: 7265 636f 6d70 696c 6564 4865 6164 6572  recompiledHeader
+000015d0: 3e0d 0a20 2020 2020 203c 2f50 7265 636f  >..      </Preco
+000015e0: 6d70 696c 6564 4865 6164 6572 3e0d 0a20  mpiledHeader>.. 
+000015f0: 2020 2020 203c 5761 726e 696e 674c 6576       <WarningLev
+00001600: 656c 3e4c 6576 656c 333c 2f57 6172 6e69  el>Level3</Warni
+00001610: 6e67 4c65 7665 6c3e 0d0a 2020 2020 2020  ngLevel>..      
+00001620: 3c4f 7074 696d 697a 6174 696f 6e3e 4469  <Optimization>Di
+00001630: 7361 626c 6564 3c2f 4f70 7469 6d69 7a61  sabled</Optimiza
+00001640: 7469 6f6e 3e0d 0a20 2020 2020 203c 5344  tion>..      <SD
+00001650: 4c43 6865 636b 3e74 7275 653c 2f53 444c  LCheck>true</SDL
+00001660: 4368 6563 6b3e 0d0a 2020 2020 2020 3c50  Check>..      <P
+00001670: 7265 7072 6f63 6573 736f 7244 6566 696e  reprocessorDefin
+00001680: 6974 696f 6e73 3e57 494e 3332 3b5f 4445  itions>WIN32;_DE
+00001690: 4255 473b 5f43 4f4e 534f 4c45 3b25 2850  BUG;_CONSOLE;%(P
+000016a0: 7265 7072 6f63 6573 736f 7244 6566 696e  reprocessorDefin
+000016b0: 6974 696f 6e73 293b 4152 4455 4341 4d5f  itions);ARDUCAM_
+000016c0: 444c 4c3c 2f50 7265 7072 6f63 6573 736f  DLL</Preprocesso
+000016d0: 7244 6566 696e 6974 696f 6e73 3e0d 0a20  rDefinitions>.. 
+000016e0: 2020 2020 203c 436f 6e66 6f72 6d61 6e63       <Conformanc
+000016f0: 654d 6f64 653e 7472 7565 3c2f 436f 6e66  eMode>true</Conf
+00001700: 6f72 6d61 6e63 654d 6f64 653e 0d0a 2020  ormanceMode>..  
+00001710: 2020 3c2f 436c 436f 6d70 696c 653e 0d0a    </ClCompile>..
+00001720: 2020 2020 3c4c 696e 6b3e 0d0a 2020 2020      <Link>..    
+00001730: 2020 3c53 7562 5379 7374 656d 3e43 6f6e    <SubSystem>Con
+00001740: 736f 6c65 3c2f 5375 6253 7973 7465 6d3e  sole</SubSystem>
+00001750: 0d0a 2020 2020 2020 3c47 656e 6572 6174  ..      <Generat
+00001760: 6544 6562 7567 496e 666f 726d 6174 696f  eDebugInformatio
+00001770: 6e3e 7472 7565 3c2f 4765 6e65 7261 7465  n>true</Generate
+00001780: 4465 6275 6749 6e66 6f72 6d61 7469 6f6e  DebugInformation
+00001790: 3e0d 0a20 2020 203c 2f4c 696e 6b3e 0d0a  >..    </Link>..
+000017a0: 2020 3c2f 4974 656d 4465 6669 6e69 7469    </ItemDefiniti
+000017b0: 6f6e 4772 6f75 703e 0d0a 2020 3c49 7465  onGroup>..  <Ite
+000017c0: 6d44 6566 696e 6974 696f 6e47 726f 7570  mDefinitionGroup
+000017d0: 2043 6f6e 6469 7469 6f6e 3d22 2724 2843   Condition="'$(C
+000017e0: 6f6e 6669 6775 7261 7469 6f6e 297c 2428  onfiguration)|$(
+000017f0: 506c 6174 666f 726d 2927 3d3d 2744 6562  Platform)'=='Deb
+00001800: 7567 7c78 3634 2722 3e0d 0a20 2020 203c  ug|x64'">..    <
+00001810: 436c 436f 6d70 696c 653e 0d0a 2020 2020  ClCompile>..    
+00001820: 2020 3c50 7265 636f 6d70 696c 6564 4865    <PrecompiledHe
+00001830: 6164 6572 3e0d 0a20 2020 2020 203c 2f50  ader>..      </P
+00001840: 7265 636f 6d70 696c 6564 4865 6164 6572  recompiledHeader
+00001850: 3e0d 0a20 2020 2020 203c 5761 726e 696e  >..      <Warnin
+00001860: 674c 6576 656c 3e4c 6576 656c 333c 2f57  gLevel>Level3</W
+00001870: 6172 6e69 6e67 4c65 7665 6c3e 0d0a 2020  arningLevel>..  
+00001880: 2020 2020 3c4f 7074 696d 697a 6174 696f      <Optimizatio
+00001890: 6e3e 4469 7361 626c 6564 3c2f 4f70 7469  n>Disabled</Opti
+000018a0: 6d69 7a61 7469 6f6e 3e0d 0a20 2020 2020  mization>..     
+000018b0: 203c 5344 4c43 6865 636b 3e74 7275 653c   <SDLCheck>true<
+000018c0: 2f53 444c 4368 6563 6b3e 0d0a 2020 2020  /SDLCheck>..    
+000018d0: 2020 3c50 7265 7072 6f63 6573 736f 7244    <PreprocessorD
+000018e0: 6566 696e 6974 696f 6e73 3e5f 4445 4255  efinitions>_DEBU
+000018f0: 473b 5f43 4f4e 534f 4c45 3b25 2850 7265  G;_CONSOLE;%(Pre
+00001900: 7072 6f63 6573 736f 7244 6566 696e 6974  processorDefinit
+00001910: 696f 6e73 293b 4152 4455 4341 4d5f 444c  ions);ARDUCAM_DL
+00001920: 4c3c 2f50 7265 7072 6f63 6573 736f 7244  L</PreprocessorD
+00001930: 6566 696e 6974 696f 6e73 3e0d 0a20 2020  efinitions>..   
+00001940: 2020 203c 436f 6e66 6f72 6d61 6e63 654d     <ConformanceM
+00001950: 6f64 653e 7472 7565 3c2f 436f 6e66 6f72  ode>true</Confor
+00001960: 6d61 6e63 654d 6f64 653e 0d0a 2020 2020  manceMode>..    
+00001970: 3c2f 436c 436f 6d70 696c 653e 0d0a 2020  </ClCompile>..  
+00001980: 2020 3c4c 696e 6b3e 0d0a 2020 2020 2020    <Link>..      
+00001990: 3c53 7562 5379 7374 656d 3e43 6f6e 736f  <SubSystem>Conso
+000019a0: 6c65 3c2f 5375 6253 7973 7465 6d3e 0d0a  le</SubSystem>..
+000019b0: 2020 2020 2020 3c47 656e 6572 6174 6544        <GenerateD
+000019c0: 6562 7567 496e 666f 726d 6174 696f 6e3e  ebugInformation>
+000019d0: 7472 7565 3c2f 4765 6e65 7261 7465 4465  true</GenerateDe
+000019e0: 6275 6749 6e66 6f72 6d61 7469 6f6e 3e0d  bugInformation>.
+000019f0: 0a20 2020 203c 2f4c 696e 6b3e 0d0a 2020  .    </Link>..  
+00001a00: 3c2f 4974 656d 4465 6669 6e69 7469 6f6e  </ItemDefinition
+00001a10: 4772 6f75 703e 0d0a 2020 3c49 7465 6d44  Group>..  <ItemD
+00001a20: 6566 696e 6974 696f 6e47 726f 7570 2043  efinitionGroup C
+00001a30: 6f6e 6469 7469 6f6e 3d22 2724 2843 6f6e  ondition="'$(Con
+00001a40: 6669 6775 7261 7469 6f6e 297c 2428 506c  figuration)|$(Pl
+00001a50: 6174 666f 726d 2927 3d3d 2752 656c 6561  atform)'=='Relea
+00001a60: 7365 7c57 696e 3332 2722 3e0d 0a20 2020  se|Win32'">..   
+00001a70: 203c 436c 436f 6d70 696c 653e 0d0a 2020   <ClCompile>..  
+00001a80: 2020 2020 3c50 7265 636f 6d70 696c 6564      <Precompiled
+00001a90: 4865 6164 6572 3e0d 0a20 2020 2020 203c  Header>..      <
+00001aa0: 2f50 7265 636f 6d70 696c 6564 4865 6164  /PrecompiledHead
+00001ab0: 6572 3e0d 0a20 2020 2020 203c 5761 726e  er>..      <Warn
+00001ac0: 696e 674c 6576 656c 3e4c 6576 656c 333c  ingLevel>Level3<
+00001ad0: 2f57 6172 6e69 6e67 4c65 7665 6c3e 0d0a  /WarningLevel>..
+00001ae0: 2020 2020 2020 3c4f 7074 696d 697a 6174        <Optimizat
+00001af0: 696f 6e3e 4d61 7853 7065 6564 3c2f 4f70  ion>MaxSpeed</Op
+00001b00: 7469 6d69 7a61 7469 6f6e 3e0d 0a20 2020  timization>..   
+00001b10: 2020 203c 4675 6e63 7469 6f6e 4c65 7665     <FunctionLeve
+00001b20: 6c4c 696e 6b69 6e67 3e74 7275 653c 2f46  lLinking>true</F
+00001b30: 756e 6374 696f 6e4c 6576 656c 4c69 6e6b  unctionLevelLink
+00001b40: 696e 673e 0d0a 2020 2020 2020 3c49 6e74  ing>..      <Int
+00001b50: 7269 6e73 6963 4675 6e63 7469 6f6e 733e  rinsicFunctions>
+00001b60: 7472 7565 3c2f 496e 7472 696e 7369 6346  true</IntrinsicF
+00001b70: 756e 6374 696f 6e73 3e0d 0a20 2020 2020  unctions>..     
+00001b80: 203c 5344 4c43 6865 636b 3e74 7275 653c   <SDLCheck>true<
+00001b90: 2f53 444c 4368 6563 6b3e 0d0a 2020 2020  /SDLCheck>..    
+00001ba0: 2020 3c50 7265 7072 6f63 6573 736f 7244    <PreprocessorD
+00001bb0: 6566 696e 6974 696f 6e73 3e57 494e 3332  efinitions>WIN32
+00001bc0: 3b4e 4445 4255 473b 5f43 4f4e 534f 4c45  ;NDEBUG;_CONSOLE
+00001bd0: 3b25 2850 7265 7072 6f63 6573 736f 7244  ;%(PreprocessorD
+00001be0: 6566 696e 6974 696f 6e73 293b 4152 4455  efinitions);ARDU
+00001bf0: 4341 4d5f 444c 4c3c 2f50 7265 7072 6f63  CAM_DLL</Preproc
+00001c00: 6573 736f 7244 6566 696e 6974 696f 6e73  essorDefinitions
+00001c10: 3e0d 0a20 2020 2020 203c 436f 6e66 6f72  >..      <Confor
+00001c20: 6d61 6e63 654d 6f64 653e 7472 7565 3c2f  manceMode>true</
+00001c30: 436f 6e66 6f72 6d61 6e63 654d 6f64 653e  ConformanceMode>
+00001c40: 0d0a 2020 2020 3c2f 436c 436f 6d70 696c  ..    </ClCompil
+00001c50: 653e 0d0a 2020 2020 3c4c 696e 6b3e 0d0a  e>..    <Link>..
+00001c60: 2020 2020 2020 3c53 7562 5379 7374 656d        <SubSystem
+00001c70: 3e43 6f6e 736f 6c65 3c2f 5375 6253 7973  >Console</SubSys
+00001c80: 7465 6d3e 0d0a 2020 2020 2020 3c45 6e61  tem>..      <Ena
+00001c90: 626c 6543 4f4d 4441 5446 6f6c 6469 6e67  bleCOMDATFolding
+00001ca0: 3e74 7275 653c 2f45 6e61 626c 6543 4f4d  >true</EnableCOM
+00001cb0: 4441 5446 6f6c 6469 6e67 3e0d 0a20 2020  DATFolding>..   
+00001cc0: 2020 203c 4f70 7469 6d69 7a65 5265 6665     <OptimizeRefe
+00001cd0: 7265 6e63 6573 3e74 7275 653c 2f4f 7074  rences>true</Opt
+00001ce0: 696d 697a 6552 6566 6572 656e 6365 733e  imizeReferences>
+00001cf0: 0d0a 2020 2020 2020 3c47 656e 6572 6174  ..      <Generat
+00001d00: 6544 6562 7567 496e 666f 726d 6174 696f  eDebugInformatio
+00001d10: 6e3e 7472 7565 3c2f 4765 6e65 7261 7465  n>true</Generate
+00001d20: 4465 6275 6749 6e66 6f72 6d61 7469 6f6e  DebugInformation
+00001d30: 3e0d 0a20 2020 203c 2f4c 696e 6b3e 0d0a  >..    </Link>..
+00001d40: 2020 3c2f 4974 656d 4465 6669 6e69 7469    </ItemDefiniti
+00001d50: 6f6e 4772 6f75 703e 0d0a 2020 3c49 7465  onGroup>..  <Ite
+00001d60: 6d44 6566 696e 6974 696f 6e47 726f 7570  mDefinitionGroup
+00001d70: 2043 6f6e 6469 7469 6f6e 3d22 2724 2843   Condition="'$(C
+00001d80: 6f6e 6669 6775 7261 7469 6f6e 297c 2428  onfiguration)|$(
+00001d90: 506c 6174 666f 726d 2927 3d3d 2752 656c  Platform)'=='Rel
+00001da0: 6561 7365 7c78 3634 2722 3e0d 0a20 2020  ease|x64'">..   
+00001db0: 203c 436c 436f 6d70 696c 653e 0d0a 2020   <ClCompile>..  
+00001dc0: 2020 2020 3c50 7265 636f 6d70 696c 6564      <Precompiled
+00001dd0: 4865 6164 6572 3e0d 0a20 2020 2020 203c  Header>..      <
+00001de0: 2f50 7265 636f 6d70 696c 6564 4865 6164  /PrecompiledHead
+00001df0: 6572 3e0d 0a20 2020 2020 203c 5761 726e  er>..      <Warn
+00001e00: 696e 674c 6576 656c 3e4c 6576 656c 333c  ingLevel>Level3<
+00001e10: 2f57 6172 6e69 6e67 4c65 7665 6c3e 0d0a  /WarningLevel>..
+00001e20: 2020 2020 2020 3c4f 7074 696d 697a 6174        <Optimizat
+00001e30: 696f 6e3e 4d61 7853 7065 6564 3c2f 4f70  ion>MaxSpeed</Op
+00001e40: 7469 6d69 7a61 7469 6f6e 3e0d 0a20 2020  timization>..   
+00001e50: 2020 203c 4675 6e63 7469 6f6e 4c65 7665     <FunctionLeve
+00001e60: 6c4c 696e 6b69 6e67 3e74 7275 653c 2f46  lLinking>true</F
+00001e70: 756e 6374 696f 6e4c 6576 656c 4c69 6e6b  unctionLevelLink
+00001e80: 696e 673e 0d0a 2020 2020 2020 3c49 6e74  ing>..      <Int
+00001e90: 7269 6e73 6963 4675 6e63 7469 6f6e 733e  rinsicFunctions>
+00001ea0: 7472 7565 3c2f 496e 7472 696e 7369 6346  true</IntrinsicF
+00001eb0: 756e 6374 696f 6e73 3e0d 0a20 2020 2020  unctions>..     
+00001ec0: 203c 5344 4c43 6865 636b 3e74 7275 653c   <SDLCheck>true<
+00001ed0: 2f53 444c 4368 6563 6b3e 0d0a 2020 2020  /SDLCheck>..    
+00001ee0: 2020 3c50 7265 7072 6f63 6573 736f 7244    <PreprocessorD
+00001ef0: 6566 696e 6974 696f 6e73 3e4e 4445 4255  efinitions>NDEBU
+00001f00: 473b 5f43 4f4e 534f 4c45 3b25 2850 7265  G;_CONSOLE;%(Pre
+00001f10: 7072 6f63 6573 736f 7244 6566 696e 6974  processorDefinit
+00001f20: 696f 6e73 293b 4152 4455 4341 4d5f 444c  ions);ARDUCAM_DL
+00001f30: 4c3c 2f50 7265 7072 6f63 6573 736f 7244  L</PreprocessorD
+00001f40: 6566 696e 6974 696f 6e73 3e0d 0a20 2020  efinitions>..   
+00001f50: 2020 203c 436f 6e66 6f72 6d61 6e63 654d     <ConformanceM
+00001f60: 6f64 653e 7472 7565 3c2f 436f 6e66 6f72  ode>true</Confor
+00001f70: 6d61 6e63 654d 6f64 653e 0d0a 2020 2020  manceMode>..    
+00001f80: 3c2f 436c 436f 6d70 696c 653e 0d0a 2020  </ClCompile>..  
+00001f90: 2020 3c4c 696e 6b3e 0d0a 2020 2020 2020    <Link>..      
+00001fa0: 3c53 7562 5379 7374 656d 3e43 6f6e 736f  <SubSystem>Conso
+00001fb0: 6c65 3c2f 5375 6253 7973 7465 6d3e 0d0a  le</SubSystem>..
+00001fc0: 2020 2020 2020 3c45 6e61 626c 6543 4f4d        <EnableCOM
+00001fd0: 4441 5446 6f6c 6469 6e67 3e74 7275 653c  DATFolding>true<
+00001fe0: 2f45 6e61 626c 6543 4f4d 4441 5446 6f6c  /EnableCOMDATFol
+00001ff0: 6469 6e67 3e0d 0a20 2020 2020 203c 4f70  ding>..      <Op
+00002000: 7469 6d69 7a65 5265 6665 7265 6e63 6573  timizeReferences
+00002010: 3e74 7275 653c 2f4f 7074 696d 697a 6552  >true</OptimizeR
+00002020: 6566 6572 656e 6365 733e 0d0a 2020 2020  eferences>..    
+00002030: 2020 3c47 656e 6572 6174 6544 6562 7567    <GenerateDebug
+00002040: 496e 666f 726d 6174 696f 6e3e 7472 7565  Information>true
+00002050: 3c2f 4765 6e65 7261 7465 4465 6275 6749  </GenerateDebugI
+00002060: 6e66 6f72 6d61 7469 6f6e 3e0d 0a20 2020  nformation>..   
+00002070: 203c 2f4c 696e 6b3e 0d0a 2020 3c2f 4974   </Link>..  </It
+00002080: 656d 4465 6669 6e69 7469 6f6e 4772 6f75  emDefinitionGrou
+00002090: 703e 0d0a 2020 3c49 6d70 6f72 7420 5072  p>..  <Import Pr
+000020a0: 6f6a 6563 743d 2224 2856 4354 6172 6765  oject="$(VCTarge
+000020b0: 7473 5061 7468 295c 4d69 6372 6f73 6f66  tsPath)\Microsof
+000020c0: 742e 4370 702e 7461 7267 6574 7322 202f  t.Cpp.targets" /
+000020d0: 3e0d 0a20 203c 496d 706f 7274 4772 6f75  >..  <ImportGrou
+000020e0: 7020 4c61 6265 6c3d 2245 7874 656e 7369  p Label="Extensi
+000020f0: 6f6e 5461 7267 6574 7322 3e0d 0a20 203c  onTargets">..  <
+00002100: 2f49 6d70 6f72 7447 726f 7570 3e0d 0a3c  /ImportGroup>..<
+00002110: 2f50 726f 6a65 6374 3e                   /Project>
```

### Comparing `arducam_config_parser-0.1.1/msvc/arducam_config_parser.vcxproj.filters` & `arducam_config_parser-0.1.2/msvc/arducam_config_parser.vcxproj.filters`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 (with BOM) text*

 * *Files 9% similar despite different names*

```diff
@@ -1,79 +1,81 @@
 00000000: efbb bf3c 3f78 6d6c 2076 6572 7369 6f6e  ...<?xml version
 00000010: 3d22 312e 3022 2065 6e63 6f64 696e 673d  ="1.0" encoding=
-00000020: 2275 7466 2d38 223f 3e0a 3c50 726f 6a65  "utf-8"?>.<Proje
-00000030: 6374 2054 6f6f 6c73 5665 7273 696f 6e3d  ct ToolsVersion=
-00000040: 2234 2e30 2220 786d 6c6e 733d 2268 7474  "4.0" xmlns="htt
-00000050: 703a 2f2f 7363 6865 6d61 732e 6d69 6372  p://schemas.micr
-00000060: 6f73 6f66 742e 636f 6d2f 6465 7665 6c6f  osoft.com/develo
-00000070: 7065 722f 6d73 6275 696c 642f 3230 3033  per/msbuild/2003
-00000080: 223e 0a20 203c 4974 656d 4772 6f75 703e  ">.  <ItemGroup>
-00000090: 0a20 2020 203c 4669 6c74 6572 2049 6e63  .    <Filter Inc
-000000a0: 6c75 6465 3d22 e6ba 90e6 9687 e4bb b622  lude="........."
-000000b0: 3e0a 2020 2020 2020 3c55 6e69 7175 6549  >.      <UniqueI
-000000c0: 6465 6e74 6966 6965 723e 7b34 4643 3733  dentifier>{4FC73
-000000d0: 3746 312d 4337 4135 2d34 3337 362d 4130  7F1-C7A5-4376-A0
-000000e0: 3636 2d32 4133 3244 3735 3241 3246 467d  66-2A32D752A2FF}
-000000f0: 3c2f 556e 6971 7565 4964 656e 7469 6669  </UniqueIdentifi
-00000100: 6572 3e0a 2020 2020 2020 3c45 7874 656e  er>.      <Exten
-00000110: 7369 6f6e 733e 6370 703b 633b 6363 3b63  sions>cpp;c;cc;c
-00000120: 7878 3b64 6566 3b6f 646c 3b69 646c 3b68  xx;def;odl;idl;h
-00000130: 706a 3b62 6174 3b61 736d 3b61 736d 783c  pj;bat;asm;asmx<
-00000140: 2f45 7874 656e 7369 6f6e 733e 0a20 2020  /Extensions>.   
-00000150: 203c 2f46 696c 7465 723e 0a20 2020 203c   </Filter>.    <
-00000160: 4669 6c74 6572 2049 6e63 6c75 6465 3d22  Filter Include="
-00000170: e5a4 b4e6 9687 e4bb b622 3e0a 2020 2020  .........">.    
-00000180: 2020 3c55 6e69 7175 6549 6465 6e74 6966    <UniqueIdentif
-00000190: 6965 723e 7b39 3339 3935 3338 302d 3839  ier>{93995380-89
-000001a0: 4244 2d34 6230 342d 3838 4542 2d36 3235  BD-4b04-88EB-625
-000001b0: 4642 4535 3245 4246 427d 3c2f 556e 6971  FBE52EBFB}</Uniq
-000001c0: 7565 4964 656e 7469 6669 6572 3e0a 2020  ueIdentifier>.  
-000001d0: 2020 2020 3c45 7874 656e 7369 6f6e 733e      <Extensions>
-000001e0: 683b 6868 3b68 7070 3b68 7878 3b68 6d3b  h;hh;hpp;hxx;hm;
-000001f0: 696e 6c3b 696e 633b 6970 703b 7873 643c  inl;inc;ipp;xsd<
-00000200: 2f45 7874 656e 7369 6f6e 733e 0a20 2020  /Extensions>.   
-00000210: 203c 2f46 696c 7465 723e 0a20 2020 203c   </Filter>.    <
-00000220: 4669 6c74 6572 2049 6e63 6c75 6465 3d22  Filter Include="
-00000230: e8b5 84e6 ba90 e696 87e4 bbb6 223e 0a20  ............">. 
-00000240: 2020 2020 203c 556e 6971 7565 4964 656e       <UniqueIden
-00000250: 7469 6669 6572 3e7b 3637 4441 3641 4236  tifier>{67DA6AB6
-00000260: 2d46 3830 302d 3463 3038 2d38 4237 412d  -F800-4c08-8B7A-
-00000270: 3833 4242 3132 3141 4144 3031 7d3c 2f55  83BB121AAD01}</U
-00000280: 6e69 7175 6549 6465 6e74 6966 6965 723e  niqueIdentifier>
-00000290: 0a20 2020 2020 203c 4578 7465 6e73 696f  .      <Extensio
-000002a0: 6e73 3e72 633b 6963 6f3b 6375 723b 626d  ns>rc;ico;cur;bm
-000002b0: 703b 646c 673b 7263 323b 7263 743b 6269  p;dlg;rc2;rct;bi
-000002c0: 6e3b 7267 733b 6769 663b 6a70 673b 6a70  n;rgs;gif;jpg;jp
-000002d0: 6567 3b6a 7065 3b72 6573 783b 7469 6666  eg;jpe;resx;tiff
-000002e0: 3b74 6966 3b70 6e67 3b77 6176 3b6d 6663  ;tif;png;wav;mfc
-000002f0: 7269 6262 6f6e 2d6d 733c 2f45 7874 656e  ribbon-ms</Exten
-00000300: 7369 6f6e 733e 0a20 2020 203c 2f46 696c  sions>.    </Fil
-00000310: 7465 723e 0a20 203c 2f49 7465 6d47 726f  ter>.  </ItemGro
-00000320: 7570 3e0a 2020 3c49 7465 6d47 726f 7570  up>.  <ItemGroup
-00000330: 3e0a 2020 2020 3c43 6c43 6f6d 7069 6c65  >.    <ClCompile
-00000340: 2049 6e63 6c75 6465 3d22 2e2e 5c73 7263   Include="..\src
-00000350: 5c61 7264 7563 616d 5f63 6f6e 6669 675f  \arducam_config_
-00000360: 7061 7273 6572 2e63 223e 0a20 2020 2020  parser.c">.     
-00000370: 203c 4669 6c74 6572 3ee6 ba90 e696 87e4   <Filter>.......
-00000380: bbb6 3c2f 4669 6c74 6572 3e0a 2020 2020  ..</Filter>.    
-00000390: 3c2f 436c 436f 6d70 696c 653e 0a20 2020  </ClCompile>.   
-000003a0: 203c 436c 436f 6d70 696c 6520 496e 636c   <ClCompile Incl
-000003b0: 7564 653d 222e 2e5c 7372 635c 696e 692e  ude="..\src\ini.
-000003c0: 6322 3e0a 2020 2020 2020 3c46 696c 7465  c">.      <Filte
-000003d0: 723e e6ba 90e6 9687 e4bb b63c 2f46 696c  r>.........</Fil
-000003e0: 7465 723e 0a20 2020 203c 2f43 6c43 6f6d  ter>.    </ClCom
-000003f0: 7069 6c65 3e0a 2020 3c2f 4974 656d 4772  pile>.  </ItemGr
-00000400: 6f75 703e 0a20 203c 4974 656d 4772 6f75  oup>.  <ItemGrou
-00000410: 703e 0a20 2020 203c 436c 496e 636c 7564  p>.    <ClInclud
-00000420: 6520 496e 636c 7564 653d 222e 2e5c 7372  e Include="..\sr
-00000430: 635c 6172 6475 6361 6d5f 636f 6e66 6967  c\arducam_config
-00000440: 5f70 6172 7365 722e 6822 3e0a 2020 2020  _parser.h">.    
-00000450: 2020 3c46 696c 7465 723e e5a4 b4e6 9687    <Filter>......
-00000460: e4bb b63c 2f46 696c 7465 723e 0a20 2020  ...</Filter>.   
-00000470: 203c 2f43 6c49 6e63 6c75 6465 3e0a 2020   </ClInclude>.  
-00000480: 2020 3c43 6c49 6e63 6c75 6465 2049 6e63    <ClInclude Inc
-00000490: 6c75 6465 3d22 2e2e 5c73 7263 5c69 6e69  lude="..\src\ini
-000004a0: 2e68 223e 0a20 2020 2020 203c 4669 6c74  .h">.      <Filt
-000004b0: 6572 3ee5 a4b4 e696 87e4 bbb6 3c2f 4669  er>.........</Fi
-000004c0: 6c74 6572 3e0a 2020 2020 3c2f 436c 496e  lter>.    </ClIn
-000004d0: 636c 7564 653e 0a20 203c 2f49 7465 6d47  clude>.  </ItemG
-000004e0: 726f 7570 3e0a 3c2f 5072 6f6a 6563 743e  roup>.</Project>
+00000020: 2275 7466 2d38 223f 3e0d 0a3c 5072 6f6a  "utf-8"?>..<Proj
+00000030: 6563 7420 546f 6f6c 7356 6572 7369 6f6e  ect ToolsVersion
+00000040: 3d22 342e 3022 2078 6d6c 6e73 3d22 6874  ="4.0" xmlns="ht
+00000050: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
+00000060: 726f 736f 6674 2e63 6f6d 2f64 6576 656c  rosoft.com/devel
+00000070: 6f70 6572 2f6d 7362 7569 6c64 2f32 3030  oper/msbuild/200
+00000080: 3322 3e0d 0a20 203c 4974 656d 4772 6f75  3">..  <ItemGrou
+00000090: 703e 0d0a 2020 2020 3c46 696c 7465 7220  p>..    <Filter 
+000000a0: 496e 636c 7564 653d 22e6 ba90 e696 87e4  Include=".......
+000000b0: bbb6 223e 0d0a 2020 2020 2020 3c55 6e69  ..">..      <Uni
+000000c0: 7175 6549 6465 6e74 6966 6965 723e 7b34  queIdentifier>{4
+000000d0: 4643 3733 3746 312d 4337 4135 2d34 3337  FC737F1-C7A5-437
+000000e0: 362d 4130 3636 2d32 4133 3244 3735 3241  6-A066-2A32D752A
+000000f0: 3246 467d 3c2f 556e 6971 7565 4964 656e  2FF}</UniqueIden
+00000100: 7469 6669 6572 3e0d 0a20 2020 2020 203c  tifier>..      <
+00000110: 4578 7465 6e73 696f 6e73 3e63 7070 3b63  Extensions>cpp;c
+00000120: 3b63 633b 6378 783b 6465 663b 6f64 6c3b  ;cc;cxx;def;odl;
+00000130: 6964 6c3b 6870 6a3b 6261 743b 6173 6d3b  idl;hpj;bat;asm;
+00000140: 6173 6d78 3c2f 4578 7465 6e73 696f 6e73  asmx</Extensions
+00000150: 3e0d 0a20 2020 203c 2f46 696c 7465 723e  >..    </Filter>
+00000160: 0d0a 2020 2020 3c46 696c 7465 7220 496e  ..    <Filter In
+00000170: 636c 7564 653d 22e5 a4b4 e696 87e4 bbb6  clude=".........
+00000180: 223e 0d0a 2020 2020 2020 3c55 6e69 7175  ">..      <Uniqu
+00000190: 6549 6465 6e74 6966 6965 723e 7b39 3339  eIdentifier>{939
+000001a0: 3935 3338 302d 3839 4244 2d34 6230 342d  95380-89BD-4b04-
+000001b0: 3838 4542 2d36 3235 4642 4535 3245 4246  88EB-625FBE52EBF
+000001c0: 427d 3c2f 556e 6971 7565 4964 656e 7469  B}</UniqueIdenti
+000001d0: 6669 6572 3e0d 0a20 2020 2020 203c 4578  fier>..      <Ex
+000001e0: 7465 6e73 696f 6e73 3e68 3b68 683b 6870  tensions>h;hh;hp
+000001f0: 703b 6878 783b 686d 3b69 6e6c 3b69 6e63  p;hxx;hm;inl;inc
+00000200: 3b69 7070 3b78 7364 3c2f 4578 7465 6e73  ;ipp;xsd</Extens
+00000210: 696f 6e73 3e0d 0a20 2020 203c 2f46 696c  ions>..    </Fil
+00000220: 7465 723e 0d0a 2020 2020 3c46 696c 7465  ter>..    <Filte
+00000230: 7220 496e 636c 7564 653d 22e8 b584 e6ba  r Include=".....
+00000240: 90e6 9687 e4bb b622 3e0d 0a20 2020 2020  .......">..     
+00000250: 203c 556e 6971 7565 4964 656e 7469 6669   <UniqueIdentifi
+00000260: 6572 3e7b 3637 4441 3641 4236 2d46 3830  er>{67DA6AB6-F80
+00000270: 302d 3463 3038 2d38 4237 412d 3833 4242  0-4c08-8B7A-83BB
+00000280: 3132 3141 4144 3031 7d3c 2f55 6e69 7175  121AAD01}</Uniqu
+00000290: 6549 6465 6e74 6966 6965 723e 0d0a 2020  eIdentifier>..  
+000002a0: 2020 2020 3c45 7874 656e 7369 6f6e 733e      <Extensions>
+000002b0: 7263 3b69 636f 3b63 7572 3b62 6d70 3b64  rc;ico;cur;bmp;d
+000002c0: 6c67 3b72 6332 3b72 6374 3b62 696e 3b72  lg;rc2;rct;bin;r
+000002d0: 6773 3b67 6966 3b6a 7067 3b6a 7065 673b  gs;gif;jpg;jpeg;
+000002e0: 6a70 653b 7265 7378 3b74 6966 663b 7469  jpe;resx;tiff;ti
+000002f0: 663b 706e 673b 7761 763b 6d66 6372 6962  f;png;wav;mfcrib
+00000300: 626f 6e2d 6d73 3c2f 4578 7465 6e73 696f  bon-ms</Extensio
+00000310: 6e73 3e0d 0a20 2020 203c 2f46 696c 7465  ns>..    </Filte
+00000320: 723e 0d0a 2020 3c2f 4974 656d 4772 6f75  r>..  </ItemGrou
+00000330: 703e 0d0a 2020 3c49 7465 6d47 726f 7570  p>..  <ItemGroup
+00000340: 3e0d 0a20 2020 203c 436c 436f 6d70 696c  >..    <ClCompil
+00000350: 6520 496e 636c 7564 653d 222e 2e5c 7372  e Include="..\sr
+00000360: 635c 6172 6475 6361 6d5f 636f 6e66 6967  c\arducam_config
+00000370: 5f70 6172 7365 722e 6322 3e0d 0a20 2020  _parser.c">..   
+00000380: 2020 203c 4669 6c74 6572 3ee6 ba90 e696     <Filter>.....
+00000390: 87e4 bbb6 3c2f 4669 6c74 6572 3e0d 0a20  ....</Filter>.. 
+000003a0: 2020 203c 2f43 6c43 6f6d 7069 6c65 3e0d     </ClCompile>.
+000003b0: 0a20 2020 203c 436c 436f 6d70 696c 6520  .    <ClCompile 
+000003c0: 496e 636c 7564 653d 222e 2e5c 7372 635c  Include="..\src\
+000003d0: 696e 692e 6322 3e0d 0a20 2020 2020 203c  ini.c">..      <
+000003e0: 4669 6c74 6572 3ee6 ba90 e696 87e4 bbb6  Filter>.........
+000003f0: 3c2f 4669 6c74 6572 3e0d 0a20 2020 203c  </Filter>..    <
+00000400: 2f43 6c43 6f6d 7069 6c65 3e0d 0a20 203c  /ClCompile>..  <
+00000410: 2f49 7465 6d47 726f 7570 3e0d 0a20 203c  /ItemGroup>..  <
+00000420: 4974 656d 4772 6f75 703e 0d0a 2020 2020  ItemGroup>..    
+00000430: 3c43 6c49 6e63 6c75 6465 2049 6e63 6c75  <ClInclude Inclu
+00000440: 6465 3d22 2e2e 5c73 7263 5c61 7264 7563  de="..\src\arduc
+00000450: 616d 5f63 6f6e 6669 675f 7061 7273 6572  am_config_parser
+00000460: 2e68 223e 0d0a 2020 2020 2020 3c46 696c  .h">..      <Fil
+00000470: 7465 723e e5a4 b4e6 9687 e4bb b63c 2f46  ter>.........</F
+00000480: 696c 7465 723e 0d0a 2020 2020 3c2f 436c  ilter>..    </Cl
+00000490: 496e 636c 7564 653e 0d0a 2020 2020 3c43  Include>..    <C
+000004a0: 6c49 6e63 6c75 6465 2049 6e63 6c75 6465  lInclude Include
+000004b0: 3d22 2e2e 5c73 7263 5c69 6e69 2e68 223e  ="..\src\ini.h">
+000004c0: 0d0a 2020 2020 2020 3c46 696c 7465 723e  ..      <Filter>
+000004d0: e5a4 b4e6 9687 e4bb b63c 2f46 696c 7465  .........</Filte
+000004e0: 723e 0d0a 2020 2020 3c2f 436c 496e 636c  r>..    </ClIncl
+000004f0: 7564 653e 0d0a 2020 3c2f 4974 656d 4772  ude>..  </ItemGr
+00000500: 6f75 703e 0d0a 3c2f 5072 6f6a 6563 743e  oup>..</Project>
```

### Comparing `arducam_config_parser-0.1.1/setup.py` & `arducam_config_parser-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup, find_packages
-from setuptools.command.build_ext import build_ext
-import platform, subprocess
-
-try:
-    # read the contents of your README file
-    from os import path
-
-    this_directory = path.abspath(path.dirname(__file__))
-    with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
-        long_description = f.read()
-except:
-    long_description = None
-
-system = platform.system()
-bits = platform.architecture()[0]
-bit = "x64" if bits == "64bit" else "x86"
-
-
-class Build(build_ext):
-    def run(self):
-        if system == "Linux":
-            subprocess.call("ls ", shell=True)
-            subprocess.call("cd ./src && make clean && make", shell=True)
-            subprocess.call("cp ./bin/*.so ./arducam_config_parser/", shell=True)
-        elif system == "Windows":
-            subprocess.call(
-                "cd ./msvc && msbuild arducam_config_parser.sln /t:Rebuild /p:Configuration=Release",
-                shell=True,
-            )
-            subprocess.call(
-                "cp ./bin/*/Release/*.dll ./arducam_config_parser/", shell=True
-            )
-
-
-setup_kwargs = {
-    "name": "arducam_config_parser",
-    "version": "0.1.1",
-    "description": "arducam_config_parser is a python wrapper for dynamic libraries. ",
-    "long_description": long_description,
-    "long_description_content_type": "text/markdown",  # This is important!
-    "author": "ArduCam",
-    "author_email": "support@arducam.com",
-    "url": "https://github.com/ArduCAM/arducam_config_parser",
-    "packages": find_packages(),
-    "package_data": {"": ["*"]},
-    "include_package_data": True,
-    "platforms": ["Windows", "Linux"],
-    "cmdclass": {"build_ext": Build},
-    "classifiers": [
-        "Programming Language :: Python",
-        "Operating System :: Microsoft :: Windows",
-        "Operating System :: Unix",
-    ],
-}
-
-
-setup(**setup_kwargs)
+# -*- coding: utf-8 -*-
+from setuptools import setup, find_packages
+from setuptools.command.build_ext import build_ext
+import platform, subprocess
+
+try:
+    # read the contents of your README file
+    from os import path
+
+    this_directory = path.abspath(path.dirname(__file__))
+    with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
+        long_description = f.read()
+except:
+    long_description = None
+
+system = platform.system()
+bits = platform.architecture()[0]
+bit = "x64" if bits == "64bit" else "x86"
+
+
+class Build(build_ext):
+    def run(self):
+        if system == "Linux":
+            subprocess.call("ls ", shell=True)
+            subprocess.call("cd ./src && make clean && make", shell=True)
+            subprocess.call("cp ./bin/*.so ./arducam_config_parser/", shell=True)
+        elif system == "Windows":
+            subprocess.call(
+                "cd ./msvc && msbuild arducam_config_parser.sln /t:Rebuild /p:Configuration=Release",
+                shell=True,
+            )
+            subprocess.call(
+                "cp ./bin/*/Release/*.dll ./arducam_config_parser/", shell=True
+            )
+
+
+setup_kwargs = {
+    "name": "arducam_config_parser",
+    "version": "0.1.2",
+    "description": "arducam_config_parser is a python wrapper for dynamic libraries. ",
+    "long_description": long_description,
+    "long_description_content_type": "text/markdown",  # This is important!
+    "author": "ArduCam",
+    "author_email": "support@arducam.com",
+    "url": "https://github.com/ArduCAM/arducam_config_parser",
+    "packages": find_packages(),
+    "package_data": {"": ["*"]},
+    "include_package_data": True,
+    "platforms": ["Windows", "Linux"],
+    "cmdclass": {"build_ext": Build},
+    "classifiers": [
+        "Programming Language :: Python",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: Unix",
+    ],
+}
+
+
+setup(**setup_kwargs)
```

### Comparing `arducam_config_parser-0.1.1/src/LICENSE.txt` & `arducam_config_parser-0.1.2/src/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-Copyright (c) 2019, ArduCam <http://www.arducam.com>.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-    * Redistributions of source code must retain the above copyright
-      notice, this list of conditions and the following disclaimer.
-    * Redistributions in binary form must reproduce the above copyright
-      notice, this list of conditions and the following disclaimer in the
-      documentation and/or other materials provided with the distribution.
-    * Neither the name of Ben Hoyt nor the names of its contributors
-      may be used to endorse or promote products derived from this software
-      without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY BEN HOYT ''AS IS'' AND ANY
-EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL BEN HOYT BE LIABLE FOR ANY
-DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
-The "inih" library is distributed under the New BSD license:
-
-Copyright (c) 2009, Ben Hoyt
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-    * Redistributions of source code must retain the above copyright
-      notice, this list of conditions and the following disclaimer.
-    * Redistributions in binary form must reproduce the above copyright
-      notice, this list of conditions and the following disclaimer in the
-      documentation and/or other materials provided with the distribution.
-    * Neither the name of Ben Hoyt nor the names of its contributors
-      may be used to endorse or promote products derived from this software
-      without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY BEN HOYT ''AS IS'' AND ANY
-EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL BEN HOYT BE LIABLE FOR ANY
-DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Copyright (c) 2019, ArduCam <http://www.arducam.com>.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+    * Redistributions of source code must retain the above copyright
+      notice, this list of conditions and the following disclaimer.
+    * Redistributions in binary form must reproduce the above copyright
+      notice, this list of conditions and the following disclaimer in the
+      documentation and/or other materials provided with the distribution.
+    * Neither the name of Ben Hoyt nor the names of its contributors
+      may be used to endorse or promote products derived from this software
+      without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY BEN HOYT ''AS IS'' AND ANY
+EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL BEN HOYT BE LIABLE FOR ANY
+DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+
+The "inih" library is distributed under the New BSD license:
+
+Copyright (c) 2009, Ben Hoyt
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+    * Redistributions of source code must retain the above copyright
+      notice, this list of conditions and the following disclaimer.
+    * Redistributions in binary form must reproduce the above copyright
+      notice, this list of conditions and the following disclaimer in the
+      documentation and/or other materials provided with the distribution.
+    * Neither the name of Ben Hoyt nor the names of its contributors
+      may be used to endorse or promote products derived from this software
+      without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY BEN HOYT ''AS IS'' AND ANY
+EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL BEN HOYT BE LIABLE FOR ANY
+DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `arducam_config_parser-0.1.1/src/Makefile` & `arducam_config_parser-0.1.2/src/Makefile`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-CROSS_COMPILE ?=
-CXX		= $(CROSS_COMPILE)g++
-CC		= $(CROSS_COMPILE)gcc
-CXXFLAGS	+= -Wall -O2 -std=c++0x -fPIC -I.
-CFLAGS		+= -Wall -O2 -std=c99 -fPIC  -I. -fvisibility=hidden -DARDUCAM_DLL -DARDUCAM_DLL_EXPORTS
-ODIR		= ../obj
-LIBS 		=
-
-LDIR		= ../bin
-
-DEPS		= ini.h arducam_config_parser.h
-
-_OBJ		= ini.o arducam_config_parser.o
-OBJ 		= $(patsubst %,$(ODIR)/%,$(_OBJ))
-
-
-$(ODIR)/%.o: %.c $(DEPS)
-	@mkdir -p $(@D)
-	$(CC) -c -o $@ $< $(CFLAGS)
-
-all:libarducam_config_parser.so libarducam_config_parser.a
-
-libarducam_config_parser.so:  $(OBJ)
-	@mkdir -p $(LDIR)
-	$(CC) -shared -o $(LDIR)/$@ $^ $(LIBS) $(CFLAGS)
-	
-libarducam_config_parser.a: $(OBJ)
-	ar cr $(LDIR)/$@  -o $^
-
-.PHONY:clean
-
-clean:
-	rm -f $(ODIR)/*.o
-	rm -f $(LDIR)/*
-
-.PHONY:install
-
-install:
-	sudo install -m 644 $(LDIR)/libarducam_config_parser.so /usr/lib/
-	sudo install -m 444 arducam_config_parser.h /usr/include/
-
-.PHONY:uninstall
-
-uninstall:
-	sudo rm /usr/lib/libarducam_config_parser.so
-	sudo rm /usr/include/arducam_config_parser.h
+CROSS_COMPILE ?=
+CXX		= $(CROSS_COMPILE)g++
+CC		= $(CROSS_COMPILE)gcc
+CXXFLAGS	+= -Wall -O2 -std=c++0x -fPIC -I.
+CFLAGS		+= -Wall -O2 -std=c99 -fPIC  -I. -fvisibility=hidden -DARDUCAM_DLL -DARDUCAM_DLL_EXPORTS
+ODIR		= ../obj
+LIBS 		=
+
+LDIR		= ../bin
+
+DEPS		= ini.h arducam_config_parser.h
+
+_OBJ		= ini.o arducam_config_parser.o
+OBJ 		= $(patsubst %,$(ODIR)/%,$(_OBJ))
+
+DESTDIR     ?=
+
+$(ODIR)/%.o: %.c $(DEPS)
+	@mkdir -p $(@D)
+	$(CC) -c -o $@ $< $(CFLAGS)
+
+all:libarducam_config_parser.so libarducam_config_parser.a
+
+libarducam_config_parser.so:  $(OBJ)
+	@mkdir -p $(LDIR)
+	$(CC) -shared -o $(LDIR)/$@ $^ $(LIBS) $(CFLAGS)
+
+libarducam_config_parser.a: $(OBJ)
+	ar cr $(LDIR)/$@  -o $^
+
+.PHONY:clean
+
+clean:
+	rm -f $(ODIR)/*.o
+	rm -f $(LDIR)/*
+
+.PHONY:install
+
+install:
+	mkdir -p $(DESTDIR)/usr/lib $(DESTDIR)/usr/include
+	install -m 0644 $(LDIR)/lib*.so* $(DESTDIR)/usr/lib/
+	install -m 0644 arducam_config_parser.h $(DESTDIR)/usr/include/
+
+.PHONY:uninstall
+
+uninstall:
+	rm $(DESTDIR)/usr/lib/libarducam_config_parser.so
+	rm $(DESTDIR)/usr/include/arducam_config_parser.h
```

### Comparing `arducam_config_parser-0.1.1/src/arducam_config_parser.c` & `arducam_config_parser-0.1.2/src/arducam_config_parser.c`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,245 +1,245 @@
-#if defined(_MSC_VER) && !defined(_CRT_SECURE_NO_WARNINGS)
-#define _CRT_SECURE_NO_WARNINGS
-#endif
-
-#include <stdio.h>
-#include <stdlib.h>
-#include <string.h>
-#include <ctype.h>
-#include "ini.h"
-#include "arducam_config_parser.h"
-
-TypeMap section_types[] = {
-    {"camera parameter", SECTION_TYPE_CAMERA},
-    {"control parameter", SECTION_TYPE_CONTROL},
-    {"board parameter", SECTION_TYPE_BOARD},
-    {"board parameter||dev2", SECTION_TYPE_BOARD_2},
-    {"board parameter||dev3||inf2", SECTION_TYPE_BOARD_3_2},
-    {"board parameter||dev3||inf3", SECTION_TYPE_BOARD_3_3},
-    {"register parameter", SECTION_TYPE_REG},
-    {"register parameter||dev3||inf2", SECTION_TYPE_REG_3_2},
-    {"register parameter||dev3||inf3", SECTION_TYPE_REG_3_3},
-    {0, 0},
-};
-
-TypeMap config_types[] = {
-    {"REG", CONFIG_TYPE_REG},
-    {"DELAY", CONFIG_TYPE_DELAY},
-    {"VRCMD", CONFIG_TYPE_VRCMD},
-    {0, 0},
-};
-
-TypeMap control_types[] = {
-    {"MIN_VALUE", CONTROL_TYPE_MIN},
-    {"MAX_VALUE", CONTROL_TYPE_MAX},
-    {"STEP", CONTROL_TYPE_STEP},
-    {"DEF", CONTROL_TYPE_DEF},
-    {"CTRL_NAME", CONTROL_TYPE_NAME},
-    {"FUNC_NAME", CONTROL_TYPE_FUNC},
-    {0, 0},
-};
-
-static uint32_t get_type(TypeMap map[], const char *name){
-    int i;
-    for(i = 0; map[i].name && strcmp(map[i].name, name); i++);
-    return map[i].type;
-}
-
-static uint32_t parse_number(const char* value){
-    const char *temp = value;
-    for(int i = 0 ; i < strlen(value);i++){
-        if(isspace((unsigned char)*temp)){
-            temp++;
-            continue;
-        }
-    }
-    if(*temp == '0' && (*(temp + 1) == 'x' || *(temp + 1) == 'X'))
-        return strtol(value, NULL, 16);
-    else
-        return strtol(value, NULL, 10);
-}
-
-static int64_t parse_numberll(const char* value){
-    const char *temp = value;
-    for(int i = 0 ; i < strlen(value);i++){
-        if(isspace((unsigned char)*temp)){
-            temp++;
-            continue;
-        }
-    }
-    if (strlen(temp) <= 2)
-        return strtoll(value, NULL, 10);
-    if(*temp == '0' && (*(temp + 1) == 'x' || *(temp + 1) == 'X'))
-        return strtoll(value, NULL, 16);
-    else
-        return strtoll(value, NULL, 10);
-}
-
-static void parse_params(Config *config, const char *src){
-    const char* delim = ",";
-    int count = 0;
-    char *origin = (char*)malloc(strlen(src) + 1);
-    strncpy(origin, src, strlen(src) + 1);
-    char *result;
-    result = strtok(origin, delim);
-    while(result != NULL){
-        config->params[count++] = parse_number(result);
-        result = strtok(NULL, delim);
-    }
-    config->params_length = count;
-    free(origin);
-}
-
-static void parse_camera_parameter(CameraParam *camera_param, const char *name, const char *value){
-    Config cfg;
-    if(!strcmp(name, "CFG_MODE")){
-        camera_param->cfg_mode = parse_number(value);
-    }else if(!strcmp(name, "TYPE")){
-        strncpy(camera_param->type, value, sizeof(camera_param->type));
-    }else if(!strcmp(name, "BIT_WIDTH")){
-        camera_param->bit_width = parse_number(value);
-    }else if(!strcmp(name, "I2C_MODE")){
-        camera_param->i2c_mode = parse_number(value);
-    }else if(!strcmp(name, "I2C_ADDR")){
-        camera_param->i2c_addr = parse_number(value);
-    }else if(!strcmp(name, "TRANS_LVL")){
-        camera_param->trans_lvl = parse_number(value);
-    }else if(!strcmp(name, "SIZE")){
-        parse_params(&cfg, value);
-        if(cfg.params_length == 2){
-            camera_param->width = cfg.params[0];
-            camera_param->height = cfg.params[1];
-        }
-    }else if(!strcmp(name, "FORMAT")){
-        parse_params(&cfg, value);
-        if(cfg.params_length == 2)
-            camera_param->format = (cfg.params[0] << 8) | cfg.params[1];
-        else if(cfg.params_length == 1)
-            camera_param->format = (cfg.params[0] << 8);
-    }
-}
-
-static void parse_control_parameter(
-        Control *ctrl, const char *name, const char *value ) {
-    if (name == NULL) {
-        ctrl->code = malloc(strlen(value) + 1);
-        ctrl->code[0] = '\0';
-        strcpy(ctrl->code, value);
-        return;
-    }
-
-    switch (get_type(control_types, name))
-    {
-    case CONTROL_TYPE_MIN:
-        ctrl->min = parse_numberll(value);
-        break;
-    case CONTROL_TYPE_MAX:
-        ctrl->max = parse_numberll(value);
-        break;
-    case CONTROL_TYPE_STEP:
-        ctrl->step = parse_numberll(value);
-        break;
-    case CONTROL_TYPE_DEF:
-        ctrl->def = parse_numberll(value);
-        break;
-    case CONTROL_TYPE_NAME:
-        strncpy(ctrl->name, value, 127);
-        break;
-    case CONTROL_TYPE_FUNC:
-        strncpy(ctrl->func, value, 127);
-        break;
-    default:
-        break;
-    }
-}
-
-
-static int parser_handle(void* user, const char* section, const char* name,
-                  const char* value)
-{
-    if(!user) return 0;
-    CameraConfigs *configs = (CameraConfigs *)user;
-    uint32_t config_type, section_type;
-
-    if(!(section_type = get_type(section_types, section)))
-        return 1;
-
-    if (name == NULL && value == NULL) {
-        if (section_type == SECTION_TYPE_CONTROL) {
-            if (configs->controls_length == 0 && configs->controls == NULL) {
-                configs->controls_length = 1;
-                configs->controls =
-                    malloc(sizeof(Control) * configs->controls_length);
-            } else {
-                configs->controls_length++;
-                configs->controls = realloc(configs->controls, 
-                    sizeof(Control) * configs->controls_length);
-            }
-        }
-        return 1;
-    }
-
-    if(section_type == SECTION_TYPE_CAMERA){
-        parse_camera_parameter(&configs->camera_param, name, value);
-    }else if (section_type == SECTION_TYPE_CONTROL){
-        parse_control_parameter(
-            &configs->controls[configs->controls_length - 1], name, value);
-
-    }else if((config_type = get_type(config_types, name))){
-        configs->configs_length++;
-        if (configs->configs_length == 1) {
-            configs->configs = malloc(sizeof(Config) * 100);
-        } else if (configs->configs_length % 100 == 0){
-            configs->configs = 
-                realloc(configs->configs, 
-                        sizeof(Config) * (configs->configs_length + 100));
-        }
-
-        Config *config = &configs->configs[configs->configs_length - 1];
-        config->type = section_type | config_type;
-        parse_params(config, value);
-    }
-
-    return 1;
-}
-
-void dump_camera_parameter(CameraParam *camera_param){
-    LOG("CFG_MODE : %d", camera_param->cfg_mode);
-    LOG("TYPE     : %s", camera_param->type);
-    LOG("WIDTH    : %d", camera_param->width);
-    LOG("HEIGHT   : %d", camera_param->height);
-    LOG("BIT_WIDTH: %d", camera_param->bit_width);
-    LOG("FORMAT   : 0x%02X", camera_param->format);
-    LOG("I2C_MODE : %d", camera_param->i2c_mode);
-    LOG("I2C_ADDR : %d", camera_param->i2c_addr);
-    LOG("TRANS_LVL: %d", camera_param->trans_lvl);
-}
-
-void dump_controls(CameraConfigs configs) {
-    for (int i = 0; i < configs.controls_length; i++) {
-        LOG("MIN_VALUE  = %ld", configs.controls[i].min);
-        LOG("MAX_VALUE  = %ld", configs.controls[i].max);
-        LOG("STEP       = %d", configs.controls[i].step);
-        LOG("DEF        = %ld", configs.controls[i].def);
-        LOG("CTRL_NAME	= %s", configs.controls[i].name);
-        LOG("FUNC_NAME	= %s", configs.controls[i].func);
-        LOG("%s", configs.controls[i].code);
-    }
-}
-
-void dump_configs(CameraConfigs *configs){
-    uint32_t lastSection = 0;
-    for (int i = 0; i < configs->configs_length; i++){
-        if(lastSection != (configs->configs[i].type >> 16)){
-            LOG("[0x%04X]", (configs->configs[i].type >> 16));
-            lastSection = configs->configs[i].type >> 16;
-        }
-        for(int j = 0; j < configs->configs[i].params_length; j++)
-            printf("0x%04X ", configs->configs[i].params[j]);
-        printf("\n");
-    }
-}
-
-int arducam_parse_config(const char *file_name, CameraConfigs *cam_cfgs){
-    return ini_parse(file_name, parser_handle, cam_cfgs);
-}
+#if defined(_MSC_VER) && !defined(_CRT_SECURE_NO_WARNINGS)
+#define _CRT_SECURE_NO_WARNINGS
+#endif
+
+#include <stdio.h>
+#include <stdlib.h>
+#include <string.h>
+#include <ctype.h>
+#include "ini.h"
+#include "arducam_config_parser.h"
+
+TypeMap section_types[] = {
+    {"camera parameter", SECTION_TYPE_CAMERA},
+    {"control parameter", SECTION_TYPE_CONTROL},
+    {"board parameter", SECTION_TYPE_BOARD},
+    {"board parameter||dev2", SECTION_TYPE_BOARD_2},
+    {"board parameter||dev3||inf2", SECTION_TYPE_BOARD_3_2},
+    {"board parameter||dev3||inf3", SECTION_TYPE_BOARD_3_3},
+    {"register parameter", SECTION_TYPE_REG},
+    {"register parameter||dev3||inf2", SECTION_TYPE_REG_3_2},
+    {"register parameter||dev3||inf3", SECTION_TYPE_REG_3_3},
+    {0, 0},
+};
+
+TypeMap config_types[] = {
+    {"REG", CONFIG_TYPE_REG},
+    {"DELAY", CONFIG_TYPE_DELAY},
+    {"VRCMD", CONFIG_TYPE_VRCMD},
+    {0, 0},
+};
+
+TypeMap control_types[] = {
+    {"MIN_VALUE", CONTROL_TYPE_MIN},
+    {"MAX_VALUE", CONTROL_TYPE_MAX},
+    {"STEP", CONTROL_TYPE_STEP},
+    {"DEF", CONTROL_TYPE_DEF},
+    {"CTRL_NAME", CONTROL_TYPE_NAME},
+    {"FUNC_NAME", CONTROL_TYPE_FUNC},
+    {0, 0},
+};
+
+static uint32_t get_type(TypeMap map[], const char *name){
+    int i;
+    for(i = 0; map[i].name && strcmp(map[i].name, name); i++);
+    return map[i].type;
+}
+
+static uint32_t parse_number(const char* value){
+    const char *temp = value;
+    for(int i = 0 ; i < strlen(value);i++){
+        if(isspace((unsigned char)*temp)){
+            temp++;
+            continue;
+        }
+    }
+    if(*temp == '0' && (*(temp + 1) == 'x' || *(temp + 1) == 'X'))
+        return strtol(value, NULL, 16);
+    else
+        return strtol(value, NULL, 10);
+}
+
+static int64_t parse_numberll(const char* value){
+    const char *temp = value;
+    for(int i = 0 ; i < strlen(value);i++){
+        if(isspace((unsigned char)*temp)){
+            temp++;
+            continue;
+        }
+    }
+    if (strlen(temp) <= 2)
+        return strtoll(value, NULL, 10);
+    if(*temp == '0' && (*(temp + 1) == 'x' || *(temp + 1) == 'X'))
+        return strtoll(value, NULL, 16);
+    else
+        return strtoll(value, NULL, 10);
+}
+
+static void parse_params(Config *config, const char *src){
+    const char* delim = ",";
+    int count = 0;
+    char *origin = (char*)malloc(strlen(src) + 1);
+    strncpy(origin, src, strlen(src) + 1);
+    char *result;
+    result = strtok(origin, delim);
+    while(result != NULL){
+        config->params[count++] = parse_number(result);
+        result = strtok(NULL, delim);
+    }
+    config->params_length = count;
+    free(origin);
+}
+
+static void parse_camera_parameter(CameraParam *camera_param, const char *name, const char *value){
+    Config cfg;
+    if(!strcmp(name, "CFG_MODE")){
+        camera_param->cfg_mode = parse_number(value);
+    }else if(!strcmp(name, "TYPE")){
+        strncpy(camera_param->type, value, sizeof(camera_param->type));
+    }else if(!strcmp(name, "BIT_WIDTH")){
+        camera_param->bit_width = parse_number(value);
+    }else if(!strcmp(name, "I2C_MODE")){
+        camera_param->i2c_mode = parse_number(value);
+    }else if(!strcmp(name, "I2C_ADDR")){
+        camera_param->i2c_addr = parse_number(value);
+    }else if(!strcmp(name, "TRANS_LVL")){
+        camera_param->trans_lvl = parse_number(value);
+    }else if(!strcmp(name, "SIZE")){
+        parse_params(&cfg, value);
+        if(cfg.params_length == 2){
+            camera_param->width = cfg.params[0];
+            camera_param->height = cfg.params[1];
+        }
+    }else if(!strcmp(name, "FORMAT")){
+        parse_params(&cfg, value);
+        if(cfg.params_length == 2)
+            camera_param->format = (cfg.params[0] << 8) | cfg.params[1];
+        else if(cfg.params_length == 1)
+            camera_param->format = (cfg.params[0] << 8);
+    }
+}
+
+static void parse_control_parameter(
+        Control *ctrl, const char *name, const char *value ) {
+    if (name == NULL) {
+        ctrl->code = malloc(strlen(value) + 1);
+        ctrl->code[0] = '\0';
+        strcpy(ctrl->code, value);
+        return;
+    }
+
+    switch (get_type(control_types, name))
+    {
+    case CONTROL_TYPE_MIN:
+        ctrl->min = parse_numberll(value);
+        break;
+    case CONTROL_TYPE_MAX:
+        ctrl->max = parse_numberll(value);
+        break;
+    case CONTROL_TYPE_STEP:
+        ctrl->step = parse_numberll(value);
+        break;
+    case CONTROL_TYPE_DEF:
+        ctrl->def = parse_numberll(value);
+        break;
+    case CONTROL_TYPE_NAME:
+        strncpy(ctrl->name, value, 127);
+        break;
+    case CONTROL_TYPE_FUNC:
+        strncpy(ctrl->func, value, 127);
+        break;
+    default:
+        break;
+    }
+}
+
+
+static int parser_handle(void* user, const char* section, const char* name,
+                  const char* value)
+{
+    if(!user) return 0;
+    CameraConfigs *configs = (CameraConfigs *)user;
+    uint32_t config_type, section_type;
+
+    if(!(section_type = get_type(section_types, section)))
+        return 1;
+
+    if (name == NULL && value == NULL) {
+        if (section_type == SECTION_TYPE_CONTROL) {
+            if (configs->controls_length == 0 && configs->controls == NULL) {
+                configs->controls_length = 1;
+                configs->controls =
+                    malloc(sizeof(Control) * configs->controls_length);
+            } else {
+                configs->controls_length++;
+                configs->controls = realloc(configs->controls, 
+                    sizeof(Control) * configs->controls_length);
+            }
+        }
+        return 1;
+    }
+
+    if(section_type == SECTION_TYPE_CAMERA){
+        parse_camera_parameter(&configs->camera_param, name, value);
+    }else if (section_type == SECTION_TYPE_CONTROL){
+        parse_control_parameter(
+            &configs->controls[configs->controls_length - 1], name, value);
+
+    }else if((config_type = get_type(config_types, name))){
+        configs->configs_length++;
+        if (configs->configs_length == 1) {
+            configs->configs = malloc(sizeof(Config) * 100);
+        } else if (configs->configs_length % 100 == 0){
+            configs->configs = 
+                realloc(configs->configs, 
+                        sizeof(Config) * (configs->configs_length + 100));
+        }
+
+        Config *config = &configs->configs[configs->configs_length - 1];
+        config->type = section_type | config_type;
+        parse_params(config, value);
+    }
+
+    return 1;
+}
+
+void dump_camera_parameter(CameraParam *camera_param){
+    LOG("CFG_MODE : %d", camera_param->cfg_mode);
+    LOG("TYPE     : %s", camera_param->type);
+    LOG("WIDTH    : %d", camera_param->width);
+    LOG("HEIGHT   : %d", camera_param->height);
+    LOG("BIT_WIDTH: %d", camera_param->bit_width);
+    LOG("FORMAT   : 0x%02X", camera_param->format);
+    LOG("I2C_MODE : %d", camera_param->i2c_mode);
+    LOG("I2C_ADDR : %d", camera_param->i2c_addr);
+    LOG("TRANS_LVL: %d", camera_param->trans_lvl);
+}
+
+void dump_controls(CameraConfigs configs) {
+    for (int i = 0; i < configs.controls_length; i++) {
+        LOG("MIN_VALUE  = %ld", configs.controls[i].min);
+        LOG("MAX_VALUE  = %ld", configs.controls[i].max);
+        LOG("STEP       = %d", configs.controls[i].step);
+        LOG("DEF        = %ld", configs.controls[i].def);
+        LOG("CTRL_NAME	= %s", configs.controls[i].name);
+        LOG("FUNC_NAME	= %s", configs.controls[i].func);
+        LOG("%s", configs.controls[i].code);
+    }
+}
+
+void dump_configs(CameraConfigs *configs){
+    uint32_t lastSection = 0;
+    for (int i = 0; i < configs->configs_length; i++){
+        if(lastSection != (configs->configs[i].type >> 16)){
+            LOG("[0x%04X]", (configs->configs[i].type >> 16));
+            lastSection = configs->configs[i].type >> 16;
+        }
+        for(int j = 0; j < configs->configs[i].params_length; j++)
+            printf("0x%04X ", configs->configs[i].params[j]);
+        printf("\n");
+    }
+}
+
+int arducam_parse_config(const char *file_name, CameraConfigs *cam_cfgs){
+    return ini_parse(file_name, parser_handle, cam_cfgs);
+}
```

### Comparing `arducam_config_parser-0.1.1/src/arducam_config_parser.h` & `arducam_config_parser-0.1.2/src/arducam_config_parser.h`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-#ifndef __ARDUCAM_CONFIG_PARSER_H__
-#define __ARDUCAM_CONFIG_PARSER_H__
-
-#if defined _WIN32 || defined __CYGWIN__
-  #define DLL_IMPORT __declspec(dllimport)
-  #define DLL_EXPORT __declspec(dllexport)
-  #define DLL_LOCAL
-#else
-  #if __GNUC__ >= 4
-    #define DLL_IMPORT __attribute__ ((visibility ("default")))
-    #define DLL_EXPORT __attribute__ ((visibility ("default")))
-    #define DLL_LOCAL  __attribute__ ((visibility ("hidden")))
-  #else
-    #define DLL_IMPORT
-    #define DLL_EXPORT
-    #define DLL_LOCAL
-  #endif
-#endif
-
-#ifdef ARDUCAM_DLL
-  #ifdef ARDUCAM_DLL_EXPORTS
-    #define ARDUCAM_API DLL_EXPORT
-  #else
-    #define ARDUCAM_API DLL_IMPORT
-  #endif
-  #define ARDUCAM_LOCAL DLL_LOCAL
-#else
-  #define ARDUCAM_API
-  #define ARDUCAM_LOCAL
-#endif
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-#include <stdint.h>
-#define MAX_CONFIGS 8192
-
-#define SECTION_TYPE_CAMERA     (0x01 << 24)
-#define SECTION_TYPE_BOARD      (0x02 << 24)
-#define SECTION_TYPE_REG        (0x03 << 24)
-#define SECTION_TYPE_CONTROL    (0x04 << 24)
-
-#define SECTION_TYPE_BOARD_2    (SECTION_TYPE_BOARD | (0x02 << 16))
-#define SECTION_TYPE_BOARD_3_2  (SECTION_TYPE_BOARD | (0x04 << 16))
-#define SECTION_TYPE_BOARD_3_3  (SECTION_TYPE_BOARD | (0x03 << 16))
-
-#define SECTION_TYPE_REG_3_2    (SECTION_TYPE_REG | (0x04 << 16))
-#define SECTION_TYPE_REG_3_3    (SECTION_TYPE_REG | (0x03 << 16))
-
-#define CONFIG_TYPE_REG     0x0001
-#define CONFIG_TYPE_VRCMD   0x0002
-#define CONFIG_TYPE_DELAY   0x0003
-
-#define CONTROL_TYPE_MIN    0x0001
-#define CONTROL_TYPE_MAX    0x0002
-#define CONTROL_TYPE_STEP   0x0003
-#define CONTROL_TYPE_DEF    0x0004
-#define CONTROL_TYPE_NAME   0x0005
-#define CONTROL_TYPE_FUNC   0x0006
-
-
-// 
-// +───────────────+───────────+──────────────+
-// |     8bit      |    8bit   |    16bit     |
-// +───────────────+───────────+──────────────+
-// | section type  | usb type  | config type  |
-// +───────────────+───────────+──────────────+
-
-typedef struct {
-    const char *name;
-    int type;
-} TypeMap;
-
-#if !defined(__ARDUCAM_STRUCT_CONTROL__)
-#define __ARDUCAM_STRUCT_CONTROL__
-typedef struct {
-    int64_t min;
-    int64_t max;
-    int32_t step;
-    int64_t def;
-    uint32_t flags;
-    char name[128];
-    char func[128];
-    char *code;
-} Control;
-#endif
-
-typedef struct {
-    uint32_t type;
-    uint32_t params[16];
-    uint8_t params_length;
-} Config;
-
-typedef struct {
-    uint32_t cfg_mode;
-    char type[50];
-    uint32_t width;
-    uint32_t height;
-    uint8_t bit_width;
-    uint16_t format;
-    uint8_t i2c_mode;
-    uint16_t i2c_addr;
-    uint32_t trans_lvl;
-} CameraParam;
-
-typedef struct {
-    CameraParam camera_param;
-    Config *configs;
-    uint32_t configs_length;
-    Control *controls;
-    uint32_t controls_length;
-} CameraConfigs;
-
-
-#define LOG(fmt, ...) fprintf(stderr, fmt "\n", ##__VA_ARGS__)
-
-
-ARDUCAM_API int arducam_parse_config(const char *file_name, CameraConfigs *cam_cfgs);
-
-#ifdef __cplusplus
-}
-#endif
-
+#ifndef __ARDUCAM_CONFIG_PARSER_H__
+#define __ARDUCAM_CONFIG_PARSER_H__
+
+#if defined _WIN32 || defined __CYGWIN__
+  #define DLL_IMPORT __declspec(dllimport)
+  #define DLL_EXPORT __declspec(dllexport)
+  #define DLL_LOCAL
+#else
+  #if __GNUC__ >= 4
+    #define DLL_IMPORT __attribute__ ((visibility ("default")))
+    #define DLL_EXPORT __attribute__ ((visibility ("default")))
+    #define DLL_LOCAL  __attribute__ ((visibility ("hidden")))
+  #else
+    #define DLL_IMPORT
+    #define DLL_EXPORT
+    #define DLL_LOCAL
+  #endif
+#endif
+
+#ifdef ARDUCAM_DLL
+  #ifdef ARDUCAM_DLL_EXPORTS
+    #define ARDUCAM_API DLL_EXPORT
+  #else
+    #define ARDUCAM_API DLL_IMPORT
+  #endif
+  #define ARDUCAM_LOCAL DLL_LOCAL
+#else
+  #define ARDUCAM_API
+  #define ARDUCAM_LOCAL
+#endif
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include <stdint.h>
+#define MAX_CONFIGS 8192
+
+#define SECTION_TYPE_CAMERA     (0x01 << 24)
+#define SECTION_TYPE_BOARD      (0x02 << 24)
+#define SECTION_TYPE_REG        (0x03 << 24)
+#define SECTION_TYPE_CONTROL    (0x04 << 24)
+
+#define SECTION_TYPE_BOARD_2    (SECTION_TYPE_BOARD | (0x02 << 16))
+#define SECTION_TYPE_BOARD_3_2  (SECTION_TYPE_BOARD | (0x04 << 16))
+#define SECTION_TYPE_BOARD_3_3  (SECTION_TYPE_BOARD | (0x03 << 16))
+
+#define SECTION_TYPE_REG_3_2    (SECTION_TYPE_REG | (0x04 << 16))
+#define SECTION_TYPE_REG_3_3    (SECTION_TYPE_REG | (0x03 << 16))
+
+#define CONFIG_TYPE_REG     0x0001
+#define CONFIG_TYPE_VRCMD   0x0002
+#define CONFIG_TYPE_DELAY   0x0003
+
+#define CONTROL_TYPE_MIN    0x0001
+#define CONTROL_TYPE_MAX    0x0002
+#define CONTROL_TYPE_STEP   0x0003
+#define CONTROL_TYPE_DEF    0x0004
+#define CONTROL_TYPE_NAME   0x0005
+#define CONTROL_TYPE_FUNC   0x0006
+
+
+// 
+// +───────────────+───────────+──────────────+
+// |     8bit      |    8bit   |    16bit     |
+// +───────────────+───────────+──────────────+
+// | section type  | usb type  | config type  |
+// +───────────────+───────────+──────────────+
+
+typedef struct {
+    const char *name;
+    int type;
+} TypeMap;
+
+#if !defined(__ARDUCAM_STRUCT_CONTROL__)
+#define __ARDUCAM_STRUCT_CONTROL__
+typedef struct {
+    int64_t min;
+    int64_t max;
+    int32_t step;
+    int64_t def;
+    uint32_t flags;
+    char name[128];
+    char func[128];
+    char *code;
+} Control;
+#endif
+
+typedef struct {
+    uint32_t type;
+    uint32_t params[16];
+    uint8_t params_length;
+} Config;
+
+typedef struct {
+    uint32_t cfg_mode;
+    char type[50];
+    uint32_t width;
+    uint32_t height;
+    uint8_t bit_width;
+    uint16_t format;
+    uint8_t i2c_mode;
+    uint16_t i2c_addr;
+    uint32_t trans_lvl;
+} CameraParam;
+
+typedef struct {
+    CameraParam camera_param;
+    Config *configs;
+    uint32_t configs_length;
+    Control *controls;
+    uint32_t controls_length;
+} CameraConfigs;
+
+
+#define LOG(fmt, ...) fprintf(stderr, fmt "\n", ##__VA_ARGS__)
+
+
+ARDUCAM_API int arducam_parse_config(const char *file_name, CameraConfigs *cam_cfgs);
+
+#ifdef __cplusplus
+}
+#endif
+
 #endif
```

### Comparing `arducam_config_parser-0.1.1/src/ini.h` & `arducam_config_parser-0.1.2/src/ini.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-/* inih -- simple .INI file parser
-
-SPDX-License-Identifier: BSD-3-Clause
-
-Copyright (C) 2009-2019, Ben Hoyt
-
-inih is released under the New BSD license (see LICENSE.txt). Go to the project
-home page for more info:
-
-https://github.com/benhoyt/inih
-
-*/
-
-#ifndef __INI_H__
-#define __INI_H__
-
-/* Make this header file easier to include in C++ code */
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-#include <stdio.h>
-
-/* Nonzero if ini_handler callback should accept lineno parameter. */
-#ifndef INI_HANDLER_LINENO
-#define INI_HANDLER_LINENO 0
-#endif
-
-/* Typedef for prototype of handler function. */
-#if INI_HANDLER_LINENO
-typedef int (*ini_handler)(void* user, const char* section,
-                           const char* name, const char* value,
-                           int lineno);
-#else
-typedef int (*ini_handler)(void* user, const char* section,
-                           const char* name, const char* value);
-#endif
-
-/* Typedef for prototype of fgets-style reader function. */
-typedef char* (*ini_reader)(char* str, int num, void* stream);
-
-/* Parse given INI-style file. May have [section]s, name=value pairs
-   (whitespace stripped), and comments starting with ';' (semicolon). Section
-   is "" if name=value pair parsed before any section heading. name:value
-   pairs are also supported as a concession to Python's configparser.
-
-   For each name=value pair parsed, call handler function with given user
-   pointer as well as section, name, and value (data only valid for duration
-   of handler call). Handler should return nonzero on success, zero on error.
-
-   Returns 0 on success, line number of first error on parse error (doesn't
-   stop on first error), -1 on file open error, or -2 on memory allocation
-   error (only when INI_USE_STACK is zero).
-*/
-int ini_parse(const char* filename, ini_handler handler, void* user);
-
-/* Same as ini_parse(), but takes a FILE* instead of filename. This doesn't
-   close the file when it's finished -- the caller must do that. */
-int ini_parse_file(FILE* file, ini_handler handler, void* user);
-
-/* Same as ini_parse(), but takes an ini_reader function pointer instead of
-   filename. Used for implementing custom or string-based I/O (see also
-   ini_parse_string). */
-int ini_parse_stream(ini_reader reader, void* stream, ini_handler handler,
-                     void* user);
-
-/* Same as ini_parse(), but takes a zero-terminated string with the INI data
-instead of a file. Useful for parsing INI data from a network socket or
-already in memory. */
-int ini_parse_string(const char* string, ini_handler handler, void* user);
-
-/* Nonzero to allow multi-line value parsing, in the style of Python's
-   configparser. If allowed, ini_parse() will call the handler with the same
-   name for each subsequent line parsed. */
-#ifndef INI_ALLOW_MULTILINE
-#define INI_ALLOW_MULTILINE 1
-#endif
-
-/* Nonzero to allow a UTF-8 BOM sequence (0xEF 0xBB 0xBF) at the start of
-   the file. See https://github.com/benhoyt/inih/issues/21 */
-#ifndef INI_ALLOW_BOM
-#define INI_ALLOW_BOM 1
-#endif
-
-/* Chars that begin a start-of-line comment. Per Python configparser, allow
-   both ; and # comments at the start of a line by default. */
-#ifndef INI_START_COMMENT_PREFIXES
-#define INI_START_COMMENT_PREFIXES ";#"
-#endif
-
-/*"/"*/
-#ifndef CUSTOMIZE_COMMENT
-#define CUSTOMIZE_COMMENT(str) ('/' == *str && '/' == *(str + 1))
-#endif
-
-#ifndef SUBSECTION_SEPARATOR
-#define SUBSECTION_SEPARATOR '|'
-#endif
-
-/* Nonzero to allow inline comments (with valid inline comment characters
-   specified by INI_INLINE_COMMENT_PREFIXES). Set to 0 to turn off and match
-   Python 3.2+ configparser behaviour. */
-#ifndef INI_ALLOW_INLINE_COMMENTS
-#define INI_ALLOW_INLINE_COMMENTS 1
-#endif
-#ifndef INI_INLINE_COMMENT_PREFIXES
-#define INI_INLINE_COMMENT_PREFIXES ";"
-#endif
-
-/* Nonzero to use stack for line buffer, zero to use heap (malloc/free). */
-#ifndef INI_USE_STACK
-#define INI_USE_STACK 1
-#endif
-
-/* Maximum line length for any line in INI file (stack or heap). Note that
-   this must be 3 more than the longest line (due to '\r', '\n', and '\0'). */
-#ifndef INI_MAX_LINE
-#define INI_MAX_LINE 200
-#endif
-
-/* Nonzero to allow heap line buffer to grow via realloc(), zero for a
-   fixed-size buffer of INI_MAX_LINE bytes. Only applies if INI_USE_STACK is
-   zero. */
-#ifndef INI_ALLOW_REALLOC
-#define INI_ALLOW_REALLOC 0
-#endif
-
-/* Initial size in bytes for heap line buffer. Only applies if INI_USE_STACK
-   is zero. */
-#ifndef INI_INITIAL_ALLOC
-#define INI_INITIAL_ALLOC 200
-#endif
-
-/* Stop parsing on first error (default is to keep parsing). */
-#ifndef INI_STOP_ON_FIRST_ERROR
-#define INI_STOP_ON_FIRST_ERROR 0
-#endif
-
-/* Nonzero to call the handler at the start of each new section (with
-   name and value NULL). Default is to only call the handler on
-   each name=value pair. */
-#ifndef INI_CALL_HANDLER_ON_NEW_SECTION
-#define INI_CALL_HANDLER_ON_NEW_SECTION 1
-#endif
-
-#ifdef __cplusplus
-}
-#endif
-
-#endif /* __INI_H__ */
+/* inih -- simple .INI file parser
+
+SPDX-License-Identifier: BSD-3-Clause
+
+Copyright (C) 2009-2019, Ben Hoyt
+
+inih is released under the New BSD license (see LICENSE.txt). Go to the project
+home page for more info:
+
+https://github.com/benhoyt/inih
+
+*/
+
+#ifndef __INI_H__
+#define __INI_H__
+
+/* Make this header file easier to include in C++ code */
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include <stdio.h>
+
+/* Nonzero if ini_handler callback should accept lineno parameter. */
+#ifndef INI_HANDLER_LINENO
+#define INI_HANDLER_LINENO 0
+#endif
+
+/* Typedef for prototype of handler function. */
+#if INI_HANDLER_LINENO
+typedef int (*ini_handler)(void* user, const char* section,
+                           const char* name, const char* value,
+                           int lineno);
+#else
+typedef int (*ini_handler)(void* user, const char* section,
+                           const char* name, const char* value);
+#endif
+
+/* Typedef for prototype of fgets-style reader function. */
+typedef char* (*ini_reader)(char* str, int num, void* stream);
+
+/* Parse given INI-style file. May have [section]s, name=value pairs
+   (whitespace stripped), and comments starting with ';' (semicolon). Section
+   is "" if name=value pair parsed before any section heading. name:value
+   pairs are also supported as a concession to Python's configparser.
+
+   For each name=value pair parsed, call handler function with given user
+   pointer as well as section, name, and value (data only valid for duration
+   of handler call). Handler should return nonzero on success, zero on error.
+
+   Returns 0 on success, line number of first error on parse error (doesn't
+   stop on first error), -1 on file open error, or -2 on memory allocation
+   error (only when INI_USE_STACK is zero).
+*/
+int ini_parse(const char* filename, ini_handler handler, void* user);
+
+/* Same as ini_parse(), but takes a FILE* instead of filename. This doesn't
+   close the file when it's finished -- the caller must do that. */
+int ini_parse_file(FILE* file, ini_handler handler, void* user);
+
+/* Same as ini_parse(), but takes an ini_reader function pointer instead of
+   filename. Used for implementing custom or string-based I/O (see also
+   ini_parse_string). */
+int ini_parse_stream(ini_reader reader, void* stream, ini_handler handler,
+                     void* user);
+
+/* Same as ini_parse(), but takes a zero-terminated string with the INI data
+instead of a file. Useful for parsing INI data from a network socket or
+already in memory. */
+int ini_parse_string(const char* string, ini_handler handler, void* user);
+
+/* Nonzero to allow multi-line value parsing, in the style of Python's
+   configparser. If allowed, ini_parse() will call the handler with the same
+   name for each subsequent line parsed. */
+#ifndef INI_ALLOW_MULTILINE
+#define INI_ALLOW_MULTILINE 1
+#endif
+
+/* Nonzero to allow a UTF-8 BOM sequence (0xEF 0xBB 0xBF) at the start of
+   the file. See https://github.com/benhoyt/inih/issues/21 */
+#ifndef INI_ALLOW_BOM
+#define INI_ALLOW_BOM 1
+#endif
+
+/* Chars that begin a start-of-line comment. Per Python configparser, allow
+   both ; and # comments at the start of a line by default. */
+#ifndef INI_START_COMMENT_PREFIXES
+#define INI_START_COMMENT_PREFIXES ";#"
+#endif
+
+/*"/"*/
+#ifndef CUSTOMIZE_COMMENT
+#define CUSTOMIZE_COMMENT(str) ('/' == *str && '/' == *(str + 1))
+#endif
+
+#ifndef SUBSECTION_SEPARATOR
+#define SUBSECTION_SEPARATOR '|'
+#endif
+
+/* Nonzero to allow inline comments (with valid inline comment characters
+   specified by INI_INLINE_COMMENT_PREFIXES). Set to 0 to turn off and match
+   Python 3.2+ configparser behaviour. */
+#ifndef INI_ALLOW_INLINE_COMMENTS
+#define INI_ALLOW_INLINE_COMMENTS 1
+#endif
+#ifndef INI_INLINE_COMMENT_PREFIXES
+#define INI_INLINE_COMMENT_PREFIXES ";"
+#endif
+
+/* Nonzero to use stack for line buffer, zero to use heap (malloc/free). */
+#ifndef INI_USE_STACK
+#define INI_USE_STACK 1
+#endif
+
+/* Maximum line length for any line in INI file (stack or heap). Note that
+   this must be 3 more than the longest line (due to '\r', '\n', and '\0'). */
+#ifndef INI_MAX_LINE
+#define INI_MAX_LINE 1024
+#endif
+
+/* Nonzero to allow heap line buffer to grow via realloc(), zero for a
+   fixed-size buffer of INI_MAX_LINE bytes. Only applies if INI_USE_STACK is
+   zero. */
+#ifndef INI_ALLOW_REALLOC
+#define INI_ALLOW_REALLOC 0
+#endif
+
+/* Initial size in bytes for heap line buffer. Only applies if INI_USE_STACK
+   is zero. */
+#ifndef INI_INITIAL_ALLOC
+#define INI_INITIAL_ALLOC 1024
+#endif
+
+/* Stop parsing on first error (default is to keep parsing). */
+#ifndef INI_STOP_ON_FIRST_ERROR
+#define INI_STOP_ON_FIRST_ERROR 0
+#endif
+
+/* Nonzero to call the handler at the start of each new section (with
+   name and value NULL). Default is to only call the handler on
+   each name=value pair. */
+#ifndef INI_CALL_HANDLER_ON_NEW_SECTION
+#define INI_CALL_HANDLER_ON_NEW_SECTION 1
+#endif
+
+#ifdef __cplusplus
+}
+#endif
+
+#endif /* __INI_H__ */
```

