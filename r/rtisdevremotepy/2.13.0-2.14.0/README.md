# Comparing `tmp/rtisdevremotepy-2.13.0.tar.gz` & `tmp/rtisdevremotepy-2.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\woute\Projects\rtisdevremotepy\dist\.tmp-0i7gwwdi\rtisdevremotepy-2.13.0.tar", last modified: Tue Apr  9 07:07:43 2024, max compression
+gzip compressed data, was "C:\Users\woute\Projects\rtisdevremotepy\dist\.tmp-hmakbs83\rtisdevremotepy-2.14.0.tar", last modified: Tue May 14 06:52:01 2024, max compression
```

## Comparing `rtisdevremotepy-2.13.0.tar` & `rtisdevremotepy-2.14.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 07:07:43.000000 rtisdevremotepy-2.13.0/
--rw-rw-rw-   0        0        0    21286 2024-04-04 14:00:40.000000 rtisdevremotepy-2.13.0/LICENSE
--rw-rw-rw-   0        0        0       37 2024-04-05 06:55:48.000000 rtisdevremotepy-2.13.0/MANIFEST.in
--rw-rw-rw-   0        0        0    32556 2024-04-09 07:07:43.000000 rtisdevremotepy-2.13.0/PKG-INFO
--rw-rw-rw-   0        0        0     6641 2024-04-09 07:06:32.000000 rtisdevremotepy-2.13.0/README.md
--rw-rw-rw-   0        0        0     1449 2024-04-09 07:06:32.000000 rtisdevremotepy-2.13.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-09 07:07:43.000000 rtisdevremotepy-2.13.0/rtisdevremotepy/
--rw-rw-rw-   0        0        0    63570 2024-04-09 07:06:32.000000 rtisdevremotepy-2.13.0/rtisdevremotepy/RTISDevRemotePy.py
--rw-rw-rw-   0        0        0     5515 2024-04-09 07:06:32.000000 rtisdevremotepy-2.13.0/rtisdevremotepy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:07:43.000000 rtisdevremotepy-2.13.0/rtisdevremotepy/rtisdevremote/
--rw-rw-rw-   0        0        0    19280 2024-03-29 14:16:26.000000 rtisdevremotepy-2.13.0/rtisdevremotepy/rtisdevremote/RTISDevRemote.py
--rw-rw-rw-   0        0        0     1314 2024-03-29 14:16:26.000000 rtisdevremotepy-2.13.0/rtisdevremotepy/rtisdevremote/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:07:43.000000 rtisdevremotepy-2.13.0/rtisdevremotepy.egg-info/
--rw-rw-rw-   0        0        0    32556 2024-04-09 07:07:43.000000 rtisdevremotepy-2.13.0/rtisdevremotepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2024-04-09 07:07:43.000000 rtisdevremotepy-2.13.0/rtisdevremotepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 07:07:43.000000 rtisdevremotepy-2.13.0/rtisdevremotepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 07:07:43.000000 rtisdevremotepy-2.13.0/rtisdevremotepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-09 07:07:43.000000 rtisdevremotepy-2.13.0/rtisdevremotepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 07:07:43.000000 rtisdevremotepy-2.13.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/
+-rw-rw-rw-   0        0        0    21286 2024-04-04 14:00:40.000000 rtisdevremotepy-2.14.0/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-04-05 06:55:48.000000 rtisdevremotepy-2.14.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    32556 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6641 2024-05-14 06:48:35.000000 rtisdevremotepy-2.14.0/README.md
+-rw-rw-rw-   0        0        0     1449 2024-05-14 06:48:35.000000 rtisdevremotepy-2.14.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy/
+-rw-rw-rw-   0        0        0    63899 2024-05-14 06:48:35.000000 rtisdevremotepy-2.14.0/rtisdevremotepy/RTISDevRemotePy.py
+-rw-rw-rw-   0        0        0     5515 2024-05-14 06:48:35.000000 rtisdevremotepy-2.14.0/rtisdevremotepy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy/rtisdevremote/
+-rw-rw-rw-   0        0        0    19280 2024-03-29 14:16:26.000000 rtisdevremotepy-2.14.0/rtisdevremotepy/rtisdevremote/RTISDevRemote.py
+-rw-rw-rw-   0        0        0     1314 2024-03-29 14:16:26.000000 rtisdevremotepy-2.14.0/rtisdevremotepy/rtisdevremote/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/
+-rw-rw-rw-   0        0        0    32556 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/setup.cfg
```

### Comparing `rtisdevremotepy-2.13.0/LICENSE` & `rtisdevremotepy-2.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtisdevremotepy-2.13.0/PKG-INFO` & `rtisdevremotepy-2.14.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtisdevremotepy
-Version: 2.13.0
+Version: 2.14.0
 Summary: Python wrapper for using RTIS Dev remotely
 Author-email: Wouter Jansen <wouter.jansen@uantwerpen.be>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
@@ -471,15 +471,15 @@
 
 ## Installation
 
 ### Dependencies
 * Python 3.6 or higher with modules:
   * Numpy
   * Scipy
-* Supported RTIS Dev version is v2.13.0.
+* Supported RTIS Dev version is v2.14.0.
 
 ### From PyPi
 You can install this module from the [PyPi repository](https://pypi.org/project/rtisdevremotepy/) like any other:
 ```bash
 pip install rtisdevremotepy
 ```
```

### Comparing `rtisdevremotepy-2.13.0/README.md` & `rtisdevremotepy-2.14.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ## Installation
 
 ### Dependencies
 * Python 3.6 or higher with modules:
   * Numpy
   * Scipy
-* Supported RTIS Dev version is v2.13.0.
+* Supported RTIS Dev version is v2.14.0.
 
 ### From PyPi
 You can install this module from the [PyPi repository](https://pypi.org/project/rtisdevremotepy/) like any other:
 ```bash
 pip install rtisdevremotepy
 ```
```

### Comparing `rtisdevremotepy-2.13.0/pyproject.toml` & `rtisdevremotepy-2.14.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rtisdevremotepy"
-version = "2.13.0"
+version = "2.14.0"
 description = "Python wrapper for using RTIS Dev remotely"
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [{ name = "Wouter Jansen", email = "wouter.jansen@uantwerpen.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 6 - Mature",
     "Programming Language :: Python",
```

### Comparing `rtisdevremotepy-2.13.0/rtisdevremotepy/RTISDevRemotePy.py` & `rtisdevremotepy-2.14.0/rtisdevremotepy/RTISDevRemotePy.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     >>> plt.show()
 """
 
 from typing import List
 from rtisdevremotepy.rtisdevremote import RTISDevRemote
 
 # Global settings
-RTISDEV_VERSION = "2.13.0"
+RTISDEV_VERSION = "2.14.0"
 
 
 class RTISDev:
     """This is class describing a wrapper of the RTIS Dev Remote library to
     %   use RTIS Dev remotely over self.ip from Python. Quickly develop with connected RTIS devices.
     %   Almost all RTIS Dev functions are available as well as automatic conversion of RTIS Dev custom class objects.
 
@@ -353,16 +353,16 @@
         return result
 
     def set_processing_settings(self, configName: str, premade: str = None,
                                 jsonPath: str = None, customPath: str = None,
                                 microphoneLayout: str = "eRTIS_v3D1", mode: int = 1, directions: int = 181,
                                 azimuthLowLimit : float = -90, azimuthHighLimit: float = 90,
                                 elevationLowLimit : float = -90, elevationHighLimit : float = 90,
-                                minRange: float = 0.5, maxRange: float = 5, pdmEnable: bool = True,
-                                matchedFilterEnable: bool = True, preFilterEnable: bool = False,
+                                elevation2DAngle: float = 0, minRange: float = 0.5, maxRange: float = 5,
+                                pdmEnable: bool = True, matchedFilterEnable: bool = True, preFilterEnable: bool = False,
                                 beamformingEnable: bool = True, postFilterEnable : bool = False,
                                 enveloppeEnable: bool = True, cleanEnable: bool = True, preloadToggle: bool = True,
                                 preFilter=None, postFilter=None, meanEnergyRangeMultiplier: float = 2,
                                 maxEnergyRangeThresholdMultiplier: float = 0.5) -> bool:
         """Set the processing settings. All parameters are optional and most have default values.
            Please read their decription carefully.
 
@@ -403,14 +403,17 @@
 
            elevationLowLimit : float (default = -90)
                The lower limit of the elevation in degrees of the directions to generate. Has to be between -90 and 90.
 
            elevationHighLimit : float (default = 90)
                The higher limit of the elevation in degrees of the directions to generate. Has to be between -90 and 90.
 
+           elevation2DAngle : float (default = 0)
+               The angle in degrees of the elevation in the 2D mode generation. Has to be between -90 and 90.
+
            minRange : float (default = 0.5)
                The minimum distance in meters of the energyscape to generate.
 
            maxRange : float (default = 5)
                The maximum distance in meters of the energyscape to generate.
 
            pdmEnable : bool (default = True)
@@ -538,23 +541,22 @@
                                                pass_zero=False).astype(np.float32)
                >>> rtisdev.set_processing_settings(postFilter=postf, postFilterEnable=True, configName=config_uuid)
         """
 
         method_name = "set_processing_settings"
         arguments = ["configName", "premade", "jsonPath", "customPath", "microphoneLayout", "mode",
                      "directions", "azimuthLowLimit", "azimuthHighLimit", "elevationLowLimit", "elevationHighLimit",
-                     "minRange", "maxRange",
-                     "pdmEnable", "preFilterEnable", "matchedFilterEnable", "beamformingEnable", "postFilterEnable",
-                     "enveloppeEnable", "cleanEnable", "preloadToggle", "preFilter", "postFilter",
-                     "meanEnergyRangeMultiplier", "maxEnergyRangeThresholdMultiplier"]
+                     "elevation2DAngle", "minRange", "maxRange", "pdmEnable", "preFilterEnable", "matchedFilterEnable",
+                     "beamformingEnable", "postFilterEnable", "enveloppeEnable", "cleanEnable", "preloadToggle",
+                     "preFilter", "postFilter", "meanEnergyRangeMultiplier", "maxEnergyRangeThresholdMultiplier"]
         values = (configName, premade, jsonPath, customPath, microphoneLayout, mode,
-                  directions, azimuthLowLimit, azimuthHighLimit, elevationLowLimit , elevationHighLimit, minRange,
-                  maxRange, pdmEnable, preFilterEnable, matchedFilterEnable, beamformingEnable, postFilterEnable,
-                  enveloppeEnable, cleanEnable, preloadToggle, preFilter, postFilter,
-                  meanEnergyRangeMultiplier, maxEnergyRangeThresholdMultiplier)
+                  directions, azimuthLowLimit, azimuthHighLimit, elevationLowLimit , elevationHighLimit,
+                  elevation2DAngle, minRange, maxRange, pdmEnable, preFilterEnable, matchedFilterEnable,
+                  beamformingEnable, postFilterEnable, enveloppeEnable, cleanEnable, preloadToggle,
+                  preFilter, postFilter, meanEnergyRangeMultiplier, maxEnergyRangeThresholdMultiplier)
 
         result, issues = RTISDevRemote.send_command(self.ip, RTISDEV_VERSION, method_name, arguments, values)
 
         if len(issues) == 1:
             raise Exception(issues[0])
         elif len(issues) > 1:
             raise Exception(issues)
@@ -636,15 +638,15 @@
     def get_settings(self, recordingPremade: str = None, recordingJsonPath: str = None, recordingCallCustom: str = None,
                      processingPremade: str = None, processingJsonPath: str = None, processingCustomPath: str = None,
                      microphoneSamples: int = 163840, microphoneSampleFrequency: int = 4500000,
                      callSampleFrequency: int = 450000, callDuration: float = 2.5, callMinimumFrequency: int = 25000,
                      callMaximumFrequency: int = 50000, callEmissions: int = 1,
                      microphoneLayout: str = "eRTIS_v3D1", mode: int = 1, directions: int = 181,
                      azimuthLowLimit: float = -90, azimuthHighLimit: float = 90,
-                     elevationLowLimit: float = -90, elevationHighLimit: float = 90,
+                     elevationLowLimit: float = -90, elevationHighLimit: float = 90, elevation2DAngle: float = 0,
                      minRange: float = 0.5, maxRange: float = 5, pdmEnable: bool = True, preFilterEnable: bool = True,
                      matchedFilterEnable: bool = True,
                      beamformingEnable: bool = True, enveloppeEnable: bool = True, postFilterEnable: bool = False,
                      cleanEnable: bool = True, preloadToggle: bool = True, preFilter=None,
                      postFilter=None, meanEnergyRangeMultiplier: float = 2,
                      maxEnergyRangeThresholdMultiplier: float = 0.5, configName: str = "") -> dict:
         """Returns an `RTISSettings` object with all chosen recording and processing settings based on the
@@ -719,14 +721,17 @@
 
            elevationLowLimit : float (default = -90)
                The lower limit of the elevation in degrees of the directions to generate. Has to be between -90 and 90.
 
            elevationHighLimit : float (default = 90)
                The higher limit of the elevation in degrees of the directions to generate. Has to be between -90 and 90.
 
+           elevation2DAngle : float (default = 0)
+               The angle in degrees of the elevation in the 2D mode generation. Has to be between -90 and 90.
+
            minRange : float (default = 0.5)
                The minimum distance in meters of the energyscape to generate.
 
            maxRange : float (default = 5)
                The maximum distance in meters of the energyscape to generate.
 
            pdmEnable : bool (default = True)
@@ -774,33 +779,31 @@
            -------
            settings : RTISSettings object as dict
                The complete class containing all RTIS settings for recording and processing. Returns 'None' or
                will raise an exception on failure.
            """
 
         method_name = "get_settings"
-        arguments = ["recordingPremade", "recordingJsonPath", "recordingCallCustom",
-                     "processingPremade", "processingJsonPath", "processingCustomPath",
-                     "microphoneSamples", "microphoneSampleFrequency",
-                     "callSampleFrequency", "callDuration", "callMinimumFrequency", "callMaximumFrequency",
-                     "callEmissions", "microphoneLayout", "mode",
-                     "directions", "azimuthLowLimit", "azimuthHighLimit", "elevationLowLimit" , "elevationHighLimit",
-                     "minRange", "maxRange", "pdmEnable", "preFilterEnable", "matchedFilterEnable",
+        arguments = ["recordingPremade", "recordingJsonPath", "recordingCallCustom", "microphoneSamples",
+                     "microphoneSampleFrequency", "callSampleFrequency", "callDuration", "callMinimumFrequency",
+                     "callMaximumFrequency", "callEmissions", "microphoneLayout", "mode", "directions",
+                     "azimuthLowLimit", "azimuthHighLimit", "elevationLowLimit" , "elevationHighLimit",
+                     "elevation2DAngle", "minRange", "maxRange", "pdmEnable", "preFilterEnable", "matchedFilterEnable",
                      "beamformingEnable", "postFilterEnable", "enveloppeEnable", "cleanEnable",
                      "preloadToggle", "preFilter", "postFilter", "meanEnergyRangeMultiplier",
                      "maxEnergyRangeThresholdMultiplier", "configName"]
         values = (recordingPremade, recordingJsonPath, recordingCallCustom,
                   processingPremade, processingJsonPath, processingCustomPath,
                   microphoneSamples, microphoneSampleFrequency,
                   callSampleFrequency, callDuration, callMinimumFrequency, callMaximumFrequency,
                   callEmissions, microphoneLayout, mode,
-                  directions, azimuthLowLimit, azimuthHighLimit, elevationLowLimit , elevationHighLimit, minRange,
-                  maxRange, pdmEnable, preFilterEnable, matchedFilterEnable, beamformingEnable, postFilterEnable,
-                  enveloppeEnable, cleanEnable, preloadToggle, preFilter, postFilter,
-                  meanEnergyRangeMultiplier, maxEnergyRangeThresholdMultiplier, configName)
+                  directions, azimuthLowLimit, azimuthHighLimit, elevationLowLimit , elevationHighLimit,
+                  elevation2DAngle, minRange, maxRange, pdmEnable, preFilterEnable, matchedFilterEnable,
+                  beamformingEnable, postFilterEnable, enveloppeEnable, cleanEnable, preloadToggle,
+                  preFilter, postFilter, meanEnergyRangeMultiplier, maxEnergyRangeThresholdMultiplier, configName)
 
         result, issues = RTISDevRemote.send_command(self.ip, RTISDEV_VERSION, method_name, arguments, values)
 
         if len(issues) == 1:
             raise Exception(issues[0])
         elif len(issues) > 1:
             raise Exception(issues)
```

### Comparing `rtisdevremotepy-2.13.0/rtisdevremotepy/__init__.py` & `rtisdevremotepy-2.14.0/rtisdevremotepy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,8 +103,8 @@
     >>> plt.title("RTIS Dev - 2D Energyscape Example")
     >>> ax = plt.gca()
     >>> ax.invert_yaxis()
     >>> ax.set_aspect("auto")
     >>> plt.show()
 """
 from .RTISDevRemotePy import *
-__version__ = "2.13.0"
+__version__ = "2.14.0"
```

### Comparing `rtisdevremotepy-2.13.0/rtisdevremotepy/rtisdevremote/RTISDevRemote.py` & `rtisdevremotepy-2.14.0/rtisdevremotepy/rtisdevremote/RTISDevRemote.py`

 * *Files identical despite different names*

### Comparing `rtisdevremotepy-2.13.0/rtisdevremotepy/rtisdevremote/__init__.py` & `rtisdevremotepy-2.14.0/rtisdevremotepy/rtisdevremote/__init__.py`

 * *Files identical despite different names*

### Comparing `rtisdevremotepy-2.13.0/rtisdevremotepy.egg-info/PKG-INFO` & `rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtisdevremotepy
-Version: 2.13.0
+Version: 2.14.0
 Summary: Python wrapper for using RTIS Dev remotely
 Author-email: Wouter Jansen <wouter.jansen@uantwerpen.be>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
@@ -471,15 +471,15 @@
 
 ## Installation
 
 ### Dependencies
 * Python 3.6 or higher with modules:
   * Numpy
   * Scipy
-* Supported RTIS Dev version is v2.13.0.
+* Supported RTIS Dev version is v2.14.0.
 
 ### From PyPi
 You can install this module from the [PyPi repository](https://pypi.org/project/rtisdevremotepy/) like any other:
 ```bash
 pip install rtisdevremotepy
 ```
```

### Comparing `rtisdevremotepy-2.13.0/rtisdevremotepy.egg-info/SOURCES.txt` & `rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

