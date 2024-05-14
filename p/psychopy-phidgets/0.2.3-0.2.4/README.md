# Comparing `tmp/psychopy-phidgets-0.2.3.tar.gz` & `tmp/psychopy-phidgets-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\psychopy-phidgets-0.2.3.tar", last modified: Thu Jul  6 12:40:37 2023, max compression
+gzip compressed data, was "psychopy-phidgets-0.2.4.tar", last modified: Tue May 14 12:04:12 2024, max compression
```

## Comparing `psychopy-phidgets-0.2.3.tar` & `psychopy-phidgets-0.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:40:37.357078 psychopy-phidgets-0.2.3/
--rw-rw-rw-   0        0        0    35823 2023-01-07 04:09:42.000000 psychopy-phidgets-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      148 2023-07-05 21:27:20.000000 psychopy-phidgets-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      482 2023-07-06 12:40:37.357078 psychopy-phidgets-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      140 2023-01-07 04:23:08.000000 psychopy-phidgets-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 12:40:37.339614 psychopy-phidgets-0.2.3/psychopy_phidgets/
--rw-rw-rw-   0        0        0      101 2023-07-05 20:38:09.000000 psychopy-phidgets-0.2.3/psychopy_phidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:40:37.348103 psychopy-phidgets-0.2.3/psychopy_phidgets/component/
--rw-rw-rw-   0        0        0        0 2023-01-07 06:01:44.000000 psychopy-phidgets-0.2.3/psychopy_phidgets/component/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:40:37.350098 psychopy-phidgets-0.2.3/psychopy_phidgets/component/classic/
--rw-rw-rw-   0        0        0     6096 2022-06-01 16:19:48.000000 psychopy-phidgets-0.2.3/psychopy_phidgets/component/classic/phidgets.png
--rw-rw-rw-   0        0        0    14287 2022-06-01 16:19:54.000000 psychopy-phidgets-0.2.3/psychopy_phidgets/component/classic/phidgets@2x.png
-drwxrwxrwx   0        0        0        0 2023-07-06 12:40:37.353088 psychopy-phidgets-0.2.3/psychopy_phidgets/component/dark/
--rw-rw-rw-   0        0        0     6096 2022-06-01 16:19:48.000000 psychopy-phidgets-0.2.3/psychopy_phidgets/component/dark/phidgets.png
--rw-rw-rw-   0        0        0    14287 2022-06-01 16:19:54.000000 psychopy-phidgets-0.2.3/psychopy_phidgets/component/dark/phidgets@2x.png
-drwxrwxrwx   0        0        0        0 2023-07-06 12:40:37.355085 psychopy-phidgets-0.2.3/psychopy_phidgets/component/light/
--rw-rw-rw-   0        0        0     6096 2022-06-01 16:19:48.000000 psychopy-phidgets-0.2.3/psychopy_phidgets/component/light/phidgets.png
--rw-rw-rw-   0        0        0    14287 2022-06-01 16:19:54.000000 psychopy-phidgets-0.2.3/psychopy_phidgets/component/light/phidgets@2x.png
--rw-rw-rw-   0        0        0     6423 2023-07-05 20:54:04.000000 psychopy-phidgets-0.2.3/psychopy_phidgets/component/phidgets.py
--rw-rw-rw-   0        0        0     2726 2023-01-07 21:32:46.000000 psychopy-phidgets-0.2.3/psychopy_phidgets/phidgets.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:40:37.346107 psychopy-phidgets-0.2.3/psychopy_phidgets.egg-info/
--rw-rw-rw-   0        0        0      482 2023-07-06 12:40:37.000000 psychopy-phidgets-0.2.3/psychopy_phidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      759 2023-07-06 12:40:37.000000 psychopy-phidgets-0.2.3/psychopy_phidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 12:40:37.000000 psychopy-phidgets-0.2.3/psychopy_phidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      184 2023-07-06 12:40:37.000000 psychopy-phidgets-0.2.3/psychopy_phidgets.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-05 21:27:21.000000 psychopy-phidgets-0.2.3/psychopy_phidgets.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-07-06 12:40:37.000000 psychopy-phidgets-0.2.3/psychopy_phidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-06 12:40:37.000000 psychopy-phidgets-0.2.3/psychopy_phidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 12:40:37.357078 psychopy-phidgets-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1179 2023-07-06 12:38:49.000000 psychopy-phidgets-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:04:12.753950 psychopy-phidgets-0.2.4/
+-rw-rw-rw-   0        0        0    35823 2023-04-01 12:04:28.000000 psychopy-phidgets-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      148 2024-05-09 15:03:51.000000 psychopy-phidgets-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      482 2024-05-14 12:04:12.753950 psychopy-phidgets-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      140 2023-04-01 12:04:28.000000 psychopy-phidgets-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 12:04:12.737611 psychopy-phidgets-0.2.4/psychopy_phidgets/
+-rw-rw-rw-   0        0        0      101 2024-05-09 15:03:51.000000 psychopy-phidgets-0.2.4/psychopy_phidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:04:12.753950 psychopy-phidgets-0.2.4/psychopy_phidgets/component/
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:03:51.000000 psychopy-phidgets-0.2.4/psychopy_phidgets/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:04:12.753950 psychopy-phidgets-0.2.4/psychopy_phidgets/component/classic/
+-rw-rw-rw-   0        0        0     6096 2024-05-09 15:03:51.000000 psychopy-phidgets-0.2.4/psychopy_phidgets/component/classic/phidgets.png
+-rw-rw-rw-   0        0        0    14287 2024-05-09 15:03:51.000000 psychopy-phidgets-0.2.4/psychopy_phidgets/component/classic/phidgets@2x.png
+drwxrwxrwx   0        0        0        0 2024-05-14 12:04:12.753950 psychopy-phidgets-0.2.4/psychopy_phidgets/component/dark/
+-rw-rw-rw-   0        0        0     6096 2024-05-09 15:03:51.000000 psychopy-phidgets-0.2.4/psychopy_phidgets/component/dark/phidgets.png
+-rw-rw-rw-   0        0        0    14287 2024-05-09 15:03:51.000000 psychopy-phidgets-0.2.4/psychopy_phidgets/component/dark/phidgets@2x.png
+drwxrwxrwx   0        0        0        0 2024-05-14 12:04:12.753950 psychopy-phidgets-0.2.4/psychopy_phidgets/component/light/
+-rw-rw-rw-   0        0        0     6096 2024-05-09 15:03:51.000000 psychopy-phidgets-0.2.4/psychopy_phidgets/component/light/phidgets.png
+-rw-rw-rw-   0        0        0    14287 2024-05-09 15:03:51.000000 psychopy-phidgets-0.2.4/psychopy_phidgets/component/light/phidgets@2x.png
+-rw-rw-rw-   0        0        0     6443 2024-05-14 11:59:57.000000 psychopy-phidgets-0.2.4/psychopy_phidgets/component/phidgets.py
+-rw-rw-rw-   0        0        0     2814 2024-05-09 15:03:51.000000 psychopy-phidgets-0.2.4/psychopy_phidgets/phidgets.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:04:12.752167 psychopy-phidgets-0.2.4/psychopy_phidgets.egg-info/
+-rw-rw-rw-   0        0        0      482 2024-05-14 12:04:12.000000 psychopy-phidgets-0.2.4/psychopy_phidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      759 2024-05-14 12:04:12.000000 psychopy-phidgets-0.2.4/psychopy_phidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 12:04:12.000000 psychopy-phidgets-0.2.4/psychopy_phidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      184 2024-05-14 12:04:12.000000 psychopy-phidgets-0.2.4/psychopy_phidgets.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-14 12:04:12.000000 psychopy-phidgets-0.2.4/psychopy_phidgets.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2024-05-14 12:04:12.000000 psychopy-phidgets-0.2.4/psychopy_phidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-14 12:04:12.000000 psychopy-phidgets-0.2.4/psychopy_phidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 12:04:12.753950 psychopy-phidgets-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1179 2024-05-14 12:02:54.000000 psychopy-phidgets-0.2.4/setup.py
```

### Comparing `psychopy-phidgets-0.2.3/LICENSE` & `psychopy-phidgets-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.2.3/psychopy_phidgets/component/classic/phidgets.png` & `psychopy-phidgets-0.2.4/psychopy_phidgets/component/classic/phidgets.png`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.2.3/psychopy_phidgets/component/classic/phidgets@2x.png` & `psychopy-phidgets-0.2.4/psychopy_phidgets/component/classic/phidgets@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.2.3/psychopy_phidgets/component/dark/phidgets.png` & `psychopy-phidgets-0.2.4/psychopy_phidgets/component/dark/phidgets.png`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.2.3/psychopy_phidgets/component/dark/phidgets@2x.png` & `psychopy-phidgets-0.2.4/psychopy_phidgets/component/dark/phidgets@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.2.3/psychopy_phidgets/component/light/phidgets.png` & `psychopy-phidgets-0.2.4/psychopy_phidgets/component/light/phidgets.png`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.2.3/psychopy_phidgets/component/light/phidgets@2x.png` & `psychopy-phidgets-0.2.4/psychopy_phidgets/component/light/phidgets@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.2.3/psychopy_phidgets/component/phidgets.py` & `psychopy-phidgets-0.2.4/psychopy_phidgets/component/phidgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 """
 from psychopy.experiment.components import BaseComponent, Param, _translate
 from psychopy import prefs, logging
 
 #Modeled after qmix/pump
 
 from pathlib import Path
-from psychopy.localization import _localized as __localized
-_localized = __localized.copy()
+#from psychopy.localization import _localized as __localized
+# _localized = __localized.copy()
+_localized = {}
 
 _localized.update({'channelList': _translate('Channel List'),
                    'serialNumber': _translate('Serial Number'),
                    'reversedRelay': _translate('Reversed Relay'),
                    'syncToScreen': _translate('Sync to screen')
                    })
```

### Comparing `psychopy-phidgets-0.2.3/psychopy_phidgets/phidgets.py` & `psychopy-phidgets-0.2.4/psychopy_phidgets/phidgets.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Part of the PsychoPy library
-# Copyright (C) 2002-2018 Jonathan Peirce (C) 2019-2022 Open Science Tools Ltd.
-# Distributed under the terms of the GNU General Public License (GPL).
-# Contributor: maqadri - mqadri@holycross.edu
-
-"""
-    Interface to Phidgets for relay control
-"""
-
-#Future - add analog input, digital input, digital output (5V) via 8/8/8 Interfacekit
-
-from psychopy import prefs, logging
-from psychopy import core
-
-all_phidgets = {}
-
-class PhidgetOutputComponent:
-    def __init__(self, channelList=None, serialNumber=-1, reversedRelay=False):
-        """
-
-        Parameters
-        ----------
-        channelList : list
-            The channels controlled by this component
-            
-        serialNumber : int
-            The serial number for the phidget you want to control
-
-        reversedRelay : bool
-            The starting state for the relay - open (0) or closed (1)
-        """
-
-        if channelList is None:
-            channelList = [0]
-
-        import Phidget22.Devices.DigitalOutput as DigitalOutput
-        import Phidget22.PhidgetException
-
-        self.phidget_outputs = []
-        if reversedRelay:
-            self.default_state = 1
-        else:
-            self.default_state = 0
-        self.status = ''
-
-        for channel in channelList:
-            all_phidgets_code = '{:}-{:}'.format(int(serialNumber),channel)
-            if all_phidgets_code not in all_phidgets.keys():
-                digitalOutput = DigitalOutput.DigitalOutput()
-                digitalOutput.setDeviceSerialNumber(int(serialNumber))
-                digitalOutput.setChannel(channel)
-                digitalOutput.openWaitForAttachment(100)
-                all_phidgets[all_phidgets_code] = digitalOutput
-            else:
-                digitalOutput = all_phidgets[all_phidgets_code]
-
-            self.phidget_outputs.append(digitalOutput)
-
-    def __del__(self):
-        self.openRelay()
-
-    def closeRelay(self):
-        [ch.setState(1-self.default_state) for ch in self.phidget_outputs]
-        # for ch in self.phidget_outputs:
-        #     if self.default_state == 1:
-        #         ch.setState(0)
-        #     else:
-        #         ch.setState(1)
-
-    def openRelay(self):
-        [ch.setState(self.default_state) for ch in self.phidget_outputs]
-        # for ch in self.phidget_outputs:
-        #     ch.setState(self.default_state)
-
-    #Currently not being used
-    def toggleRelay(self):
-        [ch.setState(1-ch.getState()) for ch in self.phidget_outputs]
-        # for ch in self.phidget_outputs:
-        #     if ch.getState() == 1:
-        #         ch.setState(0)
-        #     else:
-        #         ch.setState(1)
-        
-
-
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Part of the PsychoPy library
+# Copyright (C) 2002-2018 Jonathan Peirce (C) 2019-2022 Open Science Tools Ltd.
+# Distributed under the terms of the GNU General Public License (GPL).
+# Contributor: maqadri - mqadri@holycross.edu
+
+"""
+    Interface to Phidgets for relay control
+"""
+
+#Future - add analog input, digital input, digital output (5V) via 8/8/8 Interfacekit
+
+from psychopy import prefs, logging
+from psychopy import core
+
+all_phidgets = {}
+
+class PhidgetOutputComponent:
+    def __init__(self, channelList=None, serialNumber=-1, reversedRelay=False):
+        """
+
+        Parameters
+        ----------
+        channelList : list
+            The channels controlled by this component
+            
+        serialNumber : int
+            The serial number for the phidget you want to control
+
+        reversedRelay : bool
+            The starting state for the relay - open (0) or closed (1)
+        """
+
+        if channelList is None:
+            channelList = [0]
+
+        import Phidget22.Devices.DigitalOutput as DigitalOutput
+        import Phidget22.PhidgetException
+
+        self.phidget_outputs = []
+        if reversedRelay:
+            self.default_state = 1
+        else:
+            self.default_state = 0
+        self.status = ''
+
+        for channel in channelList:
+            all_phidgets_code = '{:}-{:}'.format(int(serialNumber),channel)
+            if all_phidgets_code not in all_phidgets.keys():
+                digitalOutput = DigitalOutput.DigitalOutput()
+                digitalOutput.setDeviceSerialNumber(int(serialNumber))
+                digitalOutput.setChannel(channel)
+                digitalOutput.openWaitForAttachment(100)
+                all_phidgets[all_phidgets_code] = digitalOutput
+            else:
+                digitalOutput = all_phidgets[all_phidgets_code]
+
+            self.phidget_outputs.append(digitalOutput)
+
+    def __del__(self):
+        self.openRelay()
+
+    def closeRelay(self):
+        [ch.setState(1-self.default_state) for ch in self.phidget_outputs]
+        # for ch in self.phidget_outputs:
+        #     if self.default_state == 1:
+        #         ch.setState(0)
+        #     else:
+        #         ch.setState(1)
+
+    def openRelay(self):
+        [ch.setState(self.default_state) for ch in self.phidget_outputs]
+        # for ch in self.phidget_outputs:
+        #     ch.setState(self.default_state)
+
+    #Currently not being used
+    def toggleRelay(self):
+        [ch.setState(1-ch.getState()) for ch in self.phidget_outputs]
+        # for ch in self.phidget_outputs:
+        #     if ch.getState() == 1:
+        #         ch.setState(0)
+        #     else:
+        #         ch.setState(1)
+        
+
+
```

### Comparing `psychopy-phidgets-0.2.3/psychopy_phidgets.egg-info/SOURCES.txt` & `psychopy-phidgets-0.2.4/psychopy_phidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.2.3/setup.py` & `psychopy-phidgets-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 setup(name='psychopy-phidgets',
-    version='0.2.3',
+    version='0.2.4',
     description='Psychopy plugin providing support for Phidgets',
     long_description='',
     url='https://github.com/maqadri/psychopy-phidgets',
     author='Muhammad A. J. Qadri',
     author_email='mqadri@holycross.edu',
     license='GPL3',
     classifiers=[
```

