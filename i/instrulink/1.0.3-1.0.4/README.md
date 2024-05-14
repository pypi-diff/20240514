# Comparing `tmp/instrulink-1.0.3.tar.gz` & `tmp/instrulink-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instrulink-1.0.3.tar", last modified: Wed Aug  9 21:14:34 2023, max compression
+gzip compressed data, was "instrulink-1.0.4.tar", last modified: Tue May 14 19:12:50 2024, max compression
```

## Comparing `instrulink-1.0.3.tar` & `instrulink-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 21:14:34.381966 instrulink-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-09 21:14:21.000000 instrulink-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-09 21:14:21.000000 instrulink-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-09 21:14:34.381966 instrulink-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-09 21:14:21.000000 instrulink-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 21:14:34.377966 instrulink-1.0.3/instrulink/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/bk_2555.py
--rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/keysight_33500b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/keysight_e5061b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/nidaq.py
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/oscilloscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    58548 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/rigol_dg1022z.py
--rw-r--r--   0 runner    (1001) docker     (123)    25707 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/rigol_ds1054z.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/si_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/sutter_mp285a.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/visa_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/waveform_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-08-09 21:14:21.000000 instrulink-1.0.3/instrulink/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 21:14:34.377966 instrulink-1.0.3/instrulink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-09 21:14:34.000000 instrulink-1.0.3/instrulink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-09 21:14:34.000000 instrulink-1.0.3/instrulink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 21:14:34.000000 instrulink-1.0.3/instrulink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 21:14:34.000000 instrulink-1.0.3/instrulink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-09 21:14:34.000000 instrulink-1.0.3/instrulink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-09 21:14:34.000000 instrulink-1.0.3/instrulink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-09 21:14:21.000000 instrulink-1.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 21:14:34.381966 instrulink-1.0.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-09 21:14:21.000000 instrulink-1.0.3/scripts/list_visa_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-09 21:14:21.000000 instrulink-1.0.3/scripts/test_33500b.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-09 21:14:21.000000 instrulink-1.0.3/scripts/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-09 21:14:21.000000 instrulink-1.0.3/scripts/test_e5061b.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-09 21:14:21.000000 instrulink-1.0.3/scripts/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-09 21:14:21.000000 instrulink-1.0.3/scripts/test_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-09 21:14:21.000000 instrulink-1.0.3/scripts/test_nidaq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-08-09 21:14:21.000000 instrulink-1.0.3/scripts/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-08-09 21:14:21.000000 instrulink-1.0.3/scripts/test_smoothed_waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 21:14:34.381966 instrulink-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-09 21:14:21.000000 instrulink-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:12:50.287524 instrulink-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-14 19:12:45.000000 instrulink-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 19:12:45.000000 instrulink-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-14 19:12:50.287524 instrulink-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-14 19:12:45.000000 instrulink-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:12:50.283523 instrulink-1.0.4/instrulink/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31627 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/bk_2555.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21215 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/keysight_33500b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/keysight_e5061b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/nidaq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15692 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/oscilloscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58510 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/rigol_dg1022z.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25791 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/rigol_ds1054z.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/si_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16548 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/sutter_mp285a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/visa_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15441 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/waveform_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17853 2024-05-14 19:12:45.000000 instrulink-1.0.4/instrulink/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:12:50.287524 instrulink-1.0.4/instrulink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-14 19:12:50.000000 instrulink-1.0.4/instrulink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-14 19:12:50.000000 instrulink-1.0.4/instrulink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:12:50.000000 instrulink-1.0.4/instrulink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:12:50.000000 instrulink-1.0.4/instrulink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 19:12:50.000000 instrulink-1.0.4/instrulink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 19:12:50.000000 instrulink-1.0.4/instrulink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 19:12:45.000000 instrulink-1.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:12:50.287524 instrulink-1.0.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-14 19:12:45.000000 instrulink-1.0.4/scripts/list_visa_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-14 19:12:45.000000 instrulink-1.0.4/scripts/test_33500b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-14 19:12:45.000000 instrulink-1.0.4/scripts/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-14 19:12:45.000000 instrulink-1.0.4/scripts/test_e5061b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-14 19:12:45.000000 instrulink-1.0.4/scripts/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-14 19:12:45.000000 instrulink-1.0.4/scripts/test_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-14 19:12:45.000000 instrulink-1.0.4/scripts/test_nidaq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-14 19:12:45.000000 instrulink-1.0.4/scripts/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-14 19:12:45.000000 instrulink-1.0.4/scripts/test_smoothed_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:12:50.287524 instrulink-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-14 19:12:45.000000 instrulink-1.0.4/setup.py
```

### Comparing `instrulink-1.0.3/LICENSE` & `instrulink-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/PKG-INFO` & `instrulink-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: instrulink
-Version: 1.0.3
-Summary: Python package to interface diverse laboratory instruments
-Home-page: https://github.com/tjjlemaire/instrulink
-Author: Theo Lemaire
-Author-email: theo.lemaire1@gmail.com
-License: MIT
-Keywords: laboratory instrument interface python
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Physics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # instrulink
 
 This python package provides built-in classes to interface diverse laboratory instruments, including:
 - **waveform generators**: [Rigol DG 1022Z](https://www.rigolna.com/products/waveform-generators/dg1000z/) (`RigolDG1022Z`)
 - **oscilloscopes**: [B&K Precision 2555](https://www.bkprecision.com/products/oscilloscopes/2555) (`BK2555`), [Rigol DS 1054Z](https://www.rigolna.com/products/digital-oscilloscopes/1000z/) (`RigolDS1054Z`)
 - **micro-manipulators**: [Sutter Instruments MP-285A](https://www.sutter.com/MICROMANIPULATION/mp285_frame.html) (`SutterMP285A`)
 - **infrared cameras**: FLIR cameras (`Camera`)
```

### Comparing `instrulink-1.0.3/README.md` & `instrulink-1.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: instrulink
+Version: 1.0.4
+Summary: Python package to interface diverse laboratory instruments
+Home-page: https://github.com/tjjlemaire/instrulink
+Author: Theo Lemaire
+Author-email: theo.lemaire1@gmail.com
+License: MIT
+Keywords: laboratory instrument interface python
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Physics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: colorlog
+Requires-Dist: pyvisa
+Requires-Dist: pyserial
+Requires-Dist: matplotlib
+Requires-Dist: nidaqmx
+
 # instrulink
 
 This python package provides built-in classes to interface diverse laboratory instruments, including:
 - **waveform generators**: [Rigol DG 1022Z](https://www.rigolna.com/products/waveform-generators/dg1000z/) (`RigolDG1022Z`)
 - **oscilloscopes**: [B&K Precision 2555](https://www.bkprecision.com/products/oscilloscopes/2555) (`BK2555`), [Rigol DS 1054Z](https://www.rigolna.com/products/digital-oscilloscopes/1000z/) (`RigolDS1054Z`)
 - **micro-manipulators**: [Sutter Instruments MP-285A](https://www.sutter.com/MICROMANIPULATION/mp285_frame.html) (`SutterMP285A`)
 - **infrared cameras**: FLIR cameras (`Camera`)
```

### Comparing `instrulink-1.0.3/instrulink/bk_2555.py` & `instrulink-1.0.4/instrulink/bk_2555.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-04-07 17:51:29
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-05-11 17:26:57
+# @Last Modified time: 2024-05-07 15:26:41
 # @Last Modified time: 2022-04-08 21:17:22
 
 import re
 import struct
 
 from .constants import *
 from .si_utils import *
@@ -184,51 +184,51 @@
         # Extract image and return
         return self.read_raw()
 
     # --------------------- SCALES / OFFSETS ---------------------
 
     def auto_setup(self):
         ''' Perform auto-setup. '''
-        logger.info('running oscilloscope auto-setup...')
+        self.log('running auto-setup...')
         self.write('ASET')
 
     def set_temporal_scale(self, value):
         ''' Set the temporal scale (in s/div) '''
         # If not in set, replace with closest valid number (in log-distance)
         if value not in self.TDIVS:
             value = self.TDIVS[np.abs(np.log(self.TDIVS) - np.log(value)).argmin()]
-        logger.info(f'setting time scale to {si_format(value, 2)}s/div')
+        self.log(f'setting time scale to {si_format(value, 2)}s/div')
         self.write(f'TDIV {self.si_process(value)}S')
     
     def get_temporal_scale(self):
         ''' Get the temporal scale (in s/div) '''
         out = self.query('TDIV?')
         return self.process_float_mo(out, f'TDIV ({SI_REGEXP})([A-z]+)', 'temporal scale')
     
     def set_vertical_scale(self, ich, value):
         ''' Set the vertical sensitivity of the specified channel (in V/div) '''
         self.check_channel_index(ich)
         if value > self.MAX_VDIV:
             logger.warning(
                 f'target vertical scale ({value} V/div) above instrument limit ({self.MAX_VDIV} V/div) -> restricting')
             value = self.MAX_VDIV
-        logger.info(f'setting channel {ich} vertical scale to {si_format(value, 2)}V/div')
+        self.log(f'setting channel {ich} vertical scale to {si_format(value, 2)}V/div')
         self.write(f'C{ich}: VDIV {self.si_process(value)}V')
 
     def get_vertical_scale(self, ich):
         ''' Get the vertical sensitivity of the specified channel (in V/div) '''
         self.check_channel_index(ich)
         out = self.query(f'C{ich}: VDIV?')
         return self.process_float_mo(
             out, f'C{ich}:VDIV ({SI_REGEXP})([A-z]+)', f'channel {ich} vertical scale')
 
     def set_vertical_offset(self, ich, value):
         ''' Set the vertical offset of the specified channel (in V) '''
         self.check_channel_index(ich)
-        logger.info(f'setting channel {ich} vertical offset to {si_format(value, 2)}V/div')
+        self.log(f'setting channel {ich} vertical offset to {si_format(value, 2)}V/div')
         self.write(f'C{ich}: OFST {self.si_process(value)}V')
 
     def get_vertical_offset(self, ich):
         ''' Get the vertical offset of the specified channel (in V) '''
         self.check_channel_index(ich)
         out = self.query(f'C{ich}: OFST?')
         return self.process_float_mo(
@@ -294,15 +294,15 @@
             if f is not None:
                 if not is_within (f, flims):
                     raise VisaError(
                         f'{k} value ({si_format(f, 1)}Hz) outside of frequency limits ({flims_str}) with current temporal scale ({si_format(tdiv, 1)}s/div)')
         fdict = {'flow': flow, 'fhigh': fhigh}
         fdict = {k: v for k, v in fdict.items() if v is not None}
         fstr = ', '.join([f'{k} = {si_format(f, 1)}Hz' for k, f in fdict.items()])
-        logger.info(f'setting {ftype} filter on channel {ich} with {fstr}')
+        self.log(f'setting {ftype} filter on channel {ich} with {fstr}')
         # Generate instruction code
         s = f'C{ich}:FILTS TYPE,{ftype}'
         if flow is not None:
             sf = si_format(flow, 1, space='').upper()
             s = f'{s},LOWLIMIT,{sf}Hz'
         if fhigh is not None:
             sf = si_format(fhigh, 1, space='').upper()
@@ -334,30 +334,30 @@
         out = self.query(f'C{ich}:ATTN?')
         mo = re.match(f'C{ich}:ATTN ({INT_REGEXP})', out)
         return float(mo[1])
     
     def set_probe_attenuation(self, ich, value):
         ''' Set the vertical attenuation factor of a specific channel '''
         self.check_channel_index(ich)
-        logger.info(f'setting channel {ich} probe attenuation factor to {value}')
+        self.log(f'setting channel {ich} probe attenuation factor to {value}')
         self.write(f'C{ich}:ATTN {value}')
 
     def get_coupling_mode(self, ich):
         ''' Get the coupling mode of a specific channel '''
         out = self.query(f'C{ich}: CPL?')
         mo = re.match(f'C{ich}:CPL ([A-z0-9]+)', out)
         return mo[1]
 
     def set_coupling_mode(self, ich, value):
         ''' Set the coupling mode of a specific channel '''
         self.check_channel_index(ich)
         if value not in self.COUPLING_MODES:
             raise VisaError(
                 f'invalid coupling mode: {value} (candidates are {self.COUPLING_MODES})')
-        logger.info(f'setting channel {ich} coupling mode to {value}')
+        self.log(f'setting channel {ich} coupling mode to {value}')
         self.write(f'C{ich}: CPL {value}')
 
     # --------------------- CURSORS ---------------------
 
     def set_cursor_position(self, ich, ctype, cpos):
         ''' 
         Set cursor position at a given screen location
@@ -438,14 +438,18 @@
         ''' Set trigger mode '''
         value = value.upper()
         if value not in self.TRIGGER_MODES:
             raise VisaError(
                 f'{value} not a valid trigger mode (candidates are {self.TRIGGER_MODES})')
         self.write(f'TRMD {value}')
     
+    def set_single_trigger(self):
+        ''' Set trigger mode to single '''
+        self.set_trigger_mode('SINGLE')
+    
     def get_trigger_coupling_mode(self, ich):
         ''' Get the trigger coupling of the selected source. '''
         self.check_channel_index(ich)
         out = self.query(f'C{ich}: TRCP?')
         return re.match(f'C{ich}:TRCP ([A-z]+)', out)[1]
     
     def set_trigger_coupling_mode(self, ich, value):
@@ -470,15 +474,15 @@
     def get_trigger_source(self):
         ''' Get trigger source channel index '''
         return self.get_trigger_options()['source']
     
     def set_trigger_source(self, ich):
         ''' Set trigger source channel index '''
         self.check_channel_index(ich)
-        logger.info(f'setting trigger source to channel {ich}')
+        self.log(f'setting trigger source to channel {ich}')
         ttype = self.get_trigger_type()
         self.write(f'TRSE {ttype},SR,C{ich}')
     
     def get_trigger_slope(self, ich):
         ''' Get trigger slope of a particular trigger source '''
         self.check_channel_index(ich)
         out = self.query(f'C{ich}: TRSL?')
@@ -487,28 +491,28 @@
     def set_trigger_slope(self, ich, value):
         ''' Set trigger slope of a particular trigger source '''
         self.check_channel_index(ich)
         value = value.upper()
         if value not in self.TRIGGER_SLOPES:
             raise VisaError(
                 f'{value} not a valid trigger slope (candidates are {self.TRIGGER_SLOPES})')
-        logger.info(f'setting channel {ich} trigger slope to {value}')
+        self.log(f'setting channel {ich} trigger slope to {value}')
         self.write(f'C{ich}: TRSL {value}')
 
     def get_trigger_level(self, ich):
         ''' Get the trigger level of the specified trigger source (in V) '''
         self.check_channel_index(ich)
         out = self.query(f'C{ich}:TRLV?')
         return self.process_float_mo(
             out, f'C{ich}:TRLV ({SI_REGEXP})([A-z]+)', f'channel {ich} trigger level')
 
     def set_trigger_level(self, ich, value):
         ''' Set the trigger level of the specified trigger source (in V) '''
         self.check_channel_index(ich)
-        logger.info(f'setting channel {ich} trigger level to {si_format(value, 2)}V')
+        self.log(f'setting channel {ich} trigger level to {si_format(value, 2)}V')
         self.write(f'C{ich}:TRLV {self.si_process(value)}V')
 
     def set_trigger_halfamp(self):
         ''' 
         Set the trigger level of the specified trigger source to the
         centre of the signal amplitude.
         '''
@@ -518,15 +522,15 @@
         ''' Get trigger delay (in s) '''
         out = self.query('TRDL?')
         return self.process_float_mo(out, f'TRDL ({FLOAT_REGEXP})([A-z]+)', 'trigger delay')
 
     def set_trigger_delay(self, value):
         ''' Set trigger delay (in s) '''
         value = self.check_trigger_delay(value)
-        logger.info(f'setting trigger time delay to {si_format(value, 2)}s')
+        self.log(f'setting trigger time delay to {si_format(value, 2)}s')
         self.write(f'TRDL {self.si_process(value)}S')
 
     def get_trigger_options(self):
         ''' Get trigger type and options '''
         out = self.query(f'TRIG_SELECT?')
         tt_opts = '|'.join(self.TRIG_TYPES)
         ht_opts = '|'.join(self.HOLD_TYPES)
```

### Comparing `instrulink-1.0.3/instrulink/camera.py` & `instrulink-1.0.4/instrulink/camera.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/instrulink/constants.py` & `instrulink-1.0.4/instrulink/constants.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/instrulink/factory.py` & `instrulink-1.0.4/instrulink/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2023-05-10 23:09:28
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-05-17 15:13:14
+# @Last Modified time: 2023-10-03 09:54:40
 
 from .rigol_dg1022z import RigolDG1022Z
 from .rigol_ds1054z import RigolDS1054Z
 from .bk_2555 import BK2555
 from .sutter_mp285a import SutterMP285A, SutterError
 from .visa_instrument import VisaError
 from .logger import logger
```

### Comparing `instrulink-1.0.3/instrulink/keysight_33500b.py` & `instrulink-1.0.4/instrulink/keysight_33500b.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Email: theo.lemaire@epfl.ch
 # @Date:   2021-02-18 18:05:57
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-05-22 09:52:23
+# @Last Modified time: 2024-05-07 15:28:38
 
 from .visa_instrument import VisaError
 from .waveform_generator import *
 from .logger import logger
 
 
 class Keysight33500B(WaveformGenerator):
@@ -175,27 +175,27 @@
         self.set_trigger_slope('POS')
 
     def set_internal_trigger(self):
         self.set_trigger_source('BUS')
         self.set_trigger_slope('POS')
 
     def single_pulse(self):
-        logger.info('sending single pulse...')
+        self.log('sending single pulse...')
         self.set_trigger_source('BUS')
         self.enable_output()
         self.trigger()
         self.wait()
     
     def wait_for_external_trigger(self):
-        logger.info('waiting for external trigger...')
+        self.log('waiting for external trigger...')
         self.set_trigger_source('EXT')
         self.enable_output()
     
     def wait_for_manual_trigger(self):
-        logger.info('waiting for external trigger...')
+        self.log('waiting for external trigger...')
         self.set_trigger_source('MAN')
         self.enable_output()
 
     # --------------------- TRIGGER OUTPUT ---------------------
 
     def enable_trigger_output(self):
         self.write('OUTP:TRIG ON')
```

### Comparing `instrulink-1.0.3/instrulink/keysight_e5061b.py` & `instrulink-1.0.4/instrulink/keysight_e5061b.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/instrulink/logger.py` & `instrulink-1.0.4/instrulink/logger.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/instrulink/nidaq.py` & `instrulink-1.0.4/instrulink/nidaq.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/instrulink/oscilloscope.py` & `instrulink-1.0.4/instrulink/oscilloscope.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-04-07 17:51:29
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-08-08 12:39:13
+# @Last Modified time: 2024-05-07 16:14:19
 # @Last Modified time: 2022-04-08 21:17:22
 
 import abc
 import re
 import io
 from PIL import Image
 import matplotlib.pyplot as plt
@@ -255,14 +255,23 @@
         ''' Get trigger mode '''
         raise NotImplementedError
      
     @abc.abstractmethod 
     def set_trigger_mode(self, value):
         ''' Set trigger mode '''
         raise NotImplementedError
+    
+    @abc.abstractmethod 
+    def set_single_trigger(self):
+        ''' Set trigger mode to single acquisition '''
+        raise NotImplementedError
+
+    def set_normal_trigger(self):
+        ''' Set trigger mode to normal '''
+        self.set_trigger_mode('NORM')
 
     @abc.abstractmethod
     def get_trigger_coupling_mode(self, *args, **kwargs):
         ''' Get trigger coupling mode. '''
         raise NotImplementedError
     
     @abc.abstractmethod
@@ -451,31 +460,43 @@
         fig, ax = plt.subplots()
         ax.imshow(img)
         ax.axis('off')
         return fig
     
     # --------------------- MULTI-CHANNEL SETTING ---------------------
 
-    def set_multichannel_vscale(self, vscale, ich_signal, ich_trigger=None, trig_detect=None):
+    def set_multichannel_vscale(self, vscales):
         ''' 
-        Set scope vertical scale and trigger settings 
-        
-        :param vdiv: vertical scale of signal channel (V/div)
-        :param ich_signal: signal channel index
-        :param ich_trigger: trigger channel index (optional)
-        :param trig_detect: trigger detection amplitude (defaults to TTL_PAMP / 2)
-        '''
-        # Set trigger detection amplitude if not specified
-        if trig_detect is None:
-           trig_detect = TTL_PAMP / 2
+        Set vertical scales on multiple channels
         
-        # Set vertical scale on signal channel
-        self.set_vertical_scale(ich_signal, vscale)
+        :param vscales: dictionary of (channel index: vertical scale) pairs. 
+            Vertical scales should be provided in (V/div). If "TRIG" is provided 
+            instead of a vertical scale, the channel vertical scale and trigger settings
+            will be automatically adjusted to detect the default TTL pulse amplitude, and 
+            the trigger soruce will be set to this channel. If no "TRIG" is provided, the
+            first channel with a non-"TRIG" vertical scale will be set as the trigger source. 
+        '''
+        # Set "is_trigger_source_set" flag to False
+        is_trigger_source_set = False
+
+        # Loop over all input channels
+        for ich, vscale in vscales.items():
+            
+            # If vscale is 'TRIG', set detection level to TTL / 2 and 
+            # set trigger source to this channel
+            if isinstance(vscale, str):
+                if vscale.upper() == 'TRIG':
+                    vscale = TTL_PAMP // 2
+                    self.set_trigger_level(ich, vscale)
+                    self.set_trigger_source(ich)
+                    is_trigger_source_set = True
+                else:
+                    raise VisaError(f'invalid vscale value: {vscale}')
+
+            # Otherwise, if trigger source is not set, assign it to this channel 
+            elif not is_trigger_source_set:
+                self.set_trigger_source(ich)
+                is_trigger_source_set = True
 
-        # Set vertical scale & trigger level on trigger channel, if any
-        if ich_trigger is not None:
-            self.set_vertical_scale(ich_trigger, trig_detect)
-            self.set_trigger_level(ich_trigger, trig_detect)
+            # In any case, set the vertical scale
+            self.set_vertical_scale(ich, vscale)
 
-        # Set trigger source to appropriate channel
-        self.set_trigger_source(ich_trigger if ich_trigger is not None else ich_signal)
-
```

### Comparing `instrulink-1.0.3/instrulink/rigol_dg1022z.py` & `instrulink-1.0.4/instrulink/rigol_dg1022z.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-03-08 08:37:26
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-08-09 17:12:00
+# @Last Modified time: 2024-05-07 15:42:08
 
 import time
 import re
 from tqdm import tqdm
 import numpy as np
 
 from .waveform_generator import *
@@ -724,15 +724,15 @@
             ttarget = np.linspace(tref[0], tref[-1], self.ARB_WF_MAXNPTS_PER_PACKET)
             y = np.interp(ttarget, tref, y)
         
         if not is_within(y.size, self.ARB_WF_NPTS_BOUNDS):
             raise VisaError(f'invalid waveform size: {y.size} (must be within {self.ARB_WF_NPTS_BOUNDS})')
         
         # Log
-        logger.info(f'uploading {y.size}-points arbitrary waveform into volatile memory')
+        self.log(f'uploading {y.size}-points arbitrary waveform into volatile memory')
 
         # Normalize vector to appropriate range
         if dtype in ('dac', 'dac16'):
             lb, ub = self.ARB_WF_DAC_RANGE
             precision = 0  # no decimals specified for integer values
         elif dtype == 'float':
             lb, ub = self.ARB_WF_FLOAT_RANGE
@@ -835,28 +835,28 @@
         :return: waveform data as numpy array
         '''
         raise NotImplementedError('download_arbitrary_waveform() not implemented yet')
         # Check channel index
         self.check_channel_index(ich)
 
         # # Variant 1: binary transfer by packet (currently not working)
-        # logger.info(f'querying waveform vector from channel {ich} volatile memory')
+        # self.log(f'querying waveform vector from channel {ich} volatile memory')
         # npackages = int(self.query(f'SOUR{ich}:DATA:LOAD? VOLATILE'))
         # data = []
         # for i in range(npackages):
         #     query = f'SOUR{ich}:DATA:LOAD? {i + 1}'
         #     chunk = self.instrument_handle.query_binary_values(
         #         f'{self.PREFIX}{query}', datatype='H', is_big_endian=False)
         #     data += chunk
         # data = np.asarray(data)
 
         # # Variant 2: query waveform data, point by point (currently not working)
         # npts = self.get_waveform_npoints(ich)
         # data = np.zeros(npts, dtype=int)
-        # logger.info(f'querying {npts}-points waveform vector from channel {ich} volatile memory')
+        # self.log(f'querying {npts}-points waveform vector from channel {ich} volatile memory')
         # for idx in tqdm(range(npts)):
         #     val = self.query(f'SOUR{ich}:DATA:VAL? VOLATILE,{idx + 1}')
         #     self.check_error()
         #     data[idx] = int(val)
         
         # Return as vector normalized to [0 - 1] interval
         return data / self.ARB_WF_DAC_MAX
@@ -1168,22 +1168,22 @@
     def get_trigger_slope(self, ich):
         self.check_channel_index(ich)
         return self.query(f'SOUR{ich}:BURS:TRIG:SLOP?')
     
     def wait_for_external_trigger(self, ich):
         ''' Set up channel to wait for external trigger. '''
         self.check_channel_index(ich)
-        logger.info(f'waiting for external trigger on channel {ich}...')
+        self.log(f'waiting for external trigger on channel {ich}...')
         self.set_trigger_source(ich, 'EXT')
         self.enable_output_channel(ich)
     
     def wait_for_manual_trigger(self, ich):
         ''' Set up channel to wait for manual trigger. '''
         self.check_channel_index(ich)
-        logger.info(f'waiting for manual/programmatic trigger on channel {ich}...')
+        self.log(f'waiting for manual/programmatic trigger on channel {ich}...')
         self.set_trigger_source(ich, 'MAN')
         self.enable_output_channel(ich)
 
     # --------------------- TRIGGER OUTPUT ---------------------
     
     def enable_trigger_output(self, ich):
         self.check_channel_index(ich)
@@ -1201,15 +1201,15 @@
     def get_trigger_output_slope(self, ich):
         self.check_channel_index(ich)
         return self.query(f'SOUR{ich}:BURS:TRIGO:SLOP?')
 
     def trigger_channel(self, ich):
         ''' Trigger specific channel programmatically. '''
         self.check_channel_index(ich)
-        logger.info(f'triggering channel {ich} programmatically')
+        self.log(f'triggering channel {ich} programmatically')
         self.write(f'SOUR{ich}:BURS:TRIG:IMM')
         self.wait()
 
     def start_trigger_loop(self, ich, T=None):
         '''
         Start a trigger loop with a specific channel
         
@@ -1234,15 +1234,15 @@
         :param trig_source: trigger source (default: external)
         '''
         # Define default log message
         s = f'setting channel {ich} to trigger {si_format(tburst, 2)}s long TTL pulse train with {si_format(PRF, 2)}Hz internal PRF'
 
         # Set default pulse amplitude if not specified
         if Vpp is None:
-            Vpp = TTL_PAMP / MV_TO_V
+            Vpp = TTL_PAMP  # V
         else:
             s = f'{s}, {si_format(Vpp, 2)}Vpp'
 
         # Complete log message based on trigger source
         if trig_source == 'INT':
             if T is None:
                 T = 2.  # s
@@ -1251,15 +1251,15 @@
             s = f'{s}, triggered externally'
         elif trig_source == 'MAN':
             s = f'{s}, triggered manually/programmatically'
         else:
             raise ValueError(f'invalid trigger source: {trig_source}')
         
         # Log process
-        logger.info(s)
+        self.log(s)
         
         # Apply pulse with specific frequency, amplitude and offset
         self.apply_pulse(ich, PRF, Vpp, offset=Vpp / 2.)
         # Set nominal pulse width
         self.set_pulse_width(ich, TTL_PWIDTH)
         # Set pulse idle level to "bottom"
         self.set_burst_idle_level(ich, 'BOTTOM')
@@ -1305,15 +1305,15 @@
             s = f'{s}, triggered externally'
         elif trig_source == 'MAN':
             s = f'{s}, triggered manually/programmatically'
         else:
             raise ValueError(f'invalid trigger source: {trig_source}')
         
         # Log process
-        logger.info(s)
+        self.log(s)
 
         # If ramping time is specified
         if tramp > 0:
             # Design smoothed waveform with appropriate number of points
             npts = self.ARB_WF_MAXNPTS_PER_PACKET
             _, y = get_DC_smoothed_pulse_envelope(npts, PRF, DC, tramp=tramp, plot=None)
             # Upload it to volatile memory of specified channel, 
@@ -1370,15 +1370,15 @@
         self.disable_output_channel(ich_trig)
         
         # Set trigger channel parameters
         self.set_trigger_pulse_train(ich_trig, PRF, tstim, **kwargs)
 
         # Set carrier channel parameters
         tburst = DC / (100 * PRF)  # s
-        logger.info(f'setting channel {ich_carrier} to output {si_format(tburst, 2)}s long, ({si_format(Fdrive, 2)}Hz, {si_format(Vpp, 3)}Vpp) sine wave triggered externally by channel {ich_trig}')
+        self.log(f'setting channel {ich_carrier} to output {si_format(tburst, 2)}s long, ({si_format(Fdrive, 2)}Hz, {si_format(Vpp, 3)}Vpp) sine wave triggered externally by channel {ich_trig}')
         self.apply_sine(ich_carrier, Fdrive, Vpp)
         self.set_burst_duration(ich_carrier, tburst)  # s
         self.enable_burst(ich_carrier)
         self.set_trigger_source(ich_carrier, 'EXT')
 
         # If carrier amplitude is > 0, enable all outputs 
         # (carrier channel last to avoid erroneous outputs)
@@ -1408,15 +1408,15 @@
         self.disable_output_channel(ich_carrier)
         self.disable_output_channel(ich_mod)
         
         # Set envelope modulating channel parameters
         self.set_AM_pulse_train(ich_mod, PRF, DC, tstim, tramp=tramp, **kwargs)
 
         # Set sinewave channel parameters
-        logger.info(f'setting channel {ich_carrier} to output ({si_format(Fdrive, 2)}Hz, {si_format(Vpp, 3)}Vpp) sine wave amplitude-modulated externally by channel {ich_mod}')
+        self.log(f'setting channel {ich_carrier} to output ({si_format(Fdrive, 2)}Hz, {si_format(Vpp, 3)}Vpp) sine wave amplitude-modulated externally by channel {ich_mod}')
         self.apply_sine(ich_carrier, Fdrive, Vpp, 0)
         self.enable_am(ich_carrier)
         self.set_am_source(ich_carrier, 'EXT')
 
         # If carrier amplitude is > 0, enable all outputs 
         # (carrier channel last to avoid erroneous outputs)
         if Vpp > 0.:
@@ -1524,15 +1524,15 @@
             
             # Log process
             params_str = ', '.join([
                 f'{si_format(Fdrive, 3)}Hz',
                 f'{si_format(Vpp, 3)}Vpp', 
                 f'{ncycles} cycles'
             ])
-            logger.info(f'setting ({params_str}) sine wave looping at {PRF:.1f} Hz on channel {ich}')
+            self.log(f'setting ({params_str}) sine wave looping at {PRF:.1f} Hz on channel {ich}')
             
             # Disable all outputs
             self.disable_output_channel(ich)
             
             # Set sine wave channel parameters
             self.apply_sine(ich, Fdrive, Vpp)
             self.set_burst_internal_period(ich, 1 / PRF)  # s
```

### Comparing `instrulink-1.0.3/instrulink/rigol_ds1054z.py` & `instrulink-1.0.4/instrulink/rigol_ds1054z.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-04-07 17:51:29
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-05-11 17:31:16
+# @Last Modified time: 2024-05-07 15:28:02
 # @Last Modified time: 2022-04-08 21:17:22
 
 import struct
 import numpy as np
 
 from .constants import *
 from .si_utils import *
@@ -129,47 +129,47 @@
         Extract screen capture image in binary format
         
         :return: binary image
         '''
         # Query image
         self.write('DISP:DATA? ON,OFF,PNG')
         # Extract image buffer
-        logger.info('Receiving screen capture...')
+        self.log('Receiving screen capture...')
         buff = self.read_raw() #self.DISPLAY_DATA_BYTES)
-        logger.info(f'read {len(buff)} bytes in .display_data')
+        self.log(f'read {len(buff)} bytes in .display_data')
         return self.decode_ieee_block(buff)
 
     # --------------------- SCALES / OFFSETS ---------------------
 
     def auto_setup(self):
         ''' Perform auto-setup. '''
-        logger.info('running scope auto-setup...')
+        self.log('running auto-setup...')
         self.write('AUT')
 
     def set_temporal_scale(self, value):
         ''' Set the temporal scale (in s/div) '''
         # If not in set, replace with closest valid number (in log-distance)
         if value not in self.TDIVS:
             value = self.TDIVS[np.abs(np.log(self.TDIVS) - np.log(value)).argmin()]
-        logger.info(f'setting time scale to {si_format(value, 2)}s/div')
+        self.log(f'setting time scale to {si_format(value, 2)}s/div')
         self.write(f'TIM:MAIN:SCAL {value}')
     
     def get_temporal_scale(self):
         ''' Get the temporal scale (in s/div) '''
         out = self.query('TIM:MAIN:SCAL?')
         return float(out)
     
     def set_vertical_scale(self, ich, value):
         ''' Set the vertical sensitivity of the specified channel (in V/div) '''
         self.check_channel_index(ich)
         if value > self.MAX_VDIV:
             logger.warning(
                 f'target vertical scale ({value} V/div) above instrument limit ({self.MAX_VDIV} V/div) -> restricting')
             value = self.MAX_VDIV
-        logger.info(f'setting channel {ich} vertical scale to {si_format(value, 2)}V/div')
+        self.log(f'setting channel {ich} vertical scale to {si_format(value, 2)}V/div')
         self.write(f'CHAN{ich}:SCAL {value}')
 
     def get_vertical_scale(self, ich):
         ''' Get the vertical sensitivity of the specified channel (in V/div) '''
         self.check_channel_index(ich)
         out = self.query(f'CHAN{ich}:SCAL?')
         return float(out)
@@ -279,15 +279,15 @@
 
     def set_coupling_mode(self, ich, value):
         ''' Set the coupling mode of a specific channel '''
         self.check_channel_index(ich)
         if value not in self.COUPLING_MODES:
             raise VisaError(
                 f'invalid coupling mode: {value} (candidates are {self.COUPLING_MODES})')
-        logger.info(f'setting channel {ich} coupling mode to {value}')
+        self.log(f'setting channel {ich} coupling mode to {value}')
         self.write(f'CHAN{ich}:COUP {value}')
 
     # --------------------- TRIGGER ---------------------
 
     def get_trigger_mode(self):
         ''' Get trigger mode '''
         return self.query('TRIG:SWE?')
@@ -296,14 +296,18 @@
         ''' Set trigger mode '''
         value = value.upper()
         if value not in self.TRIGGER_MODES:
             raise VisaError(
                 f'{value} not a valid trigger mode (candidates are {self.TRIGGER_MODES})')
         self.write(f'TRIG:SWE {value}')
     
+    def set_single_trigger(self):
+        ''' Set trigger mode to single '''
+        self.set_trigger_mode('SING')
+    
     def get_trigger_coupling_mode(self, ich):
         ''' Get the trigger coupling mode. '''
         if self.get_trigger_source() != ich:
             self.set_trigger_source(ich)
         return self.query('TRIG:COUP?')
     
     def set_trigger_coupling_mode(self, ich, value):
@@ -364,15 +368,15 @@
         ttype = self.get_trigger_type()
         out = self.query(f'TRIG:{ttype}:SOUR?')
         return int(out[-1])
     
     def set_trigger_source(self, ich):
         ''' Set trigger source channel index '''
         self.check_channel_index(ich)
-        logger.info(f'setting trigger source to channel {ich}')
+        self.log(f'setting trigger source to channel {ich}')
         ttype = self.get_trigger_type()
         self.write(f'TRIG:{ttype}:SOUR CHAN{ich}')
     
     def get_trigger_slope(self, ich):
         ''' Get trigger slope for current trigger type '''
         if self.get_trigger_source() != ich:
             self.set_trigger_source(ich)
@@ -384,15 +388,15 @@
         if self.get_trigger_source() != ich:
             self.set_trigger_source(ich)
         value = value.upper()
         if value not in self.TRIGGER_SLOPES:
             raise VisaError(
                 f'{value} not a valid trigger slope (candidates are {self.TRIGGER_SLOPES})')
         ttype = self.get_trigger_type()
-        logger.info(f'setting {ttype} trigger slope to {value}')
+        self.log(f'setting {ttype} trigger slope to {value}')
         self.write(f'TRIG:{ttype}:SLOP {value}')
     
     def get_trigger_level(self, ich):
         ''' Get trigger level (in V) '''
         if self.get_trigger_source() != ich:
             self.set_trigger_source(ich)
         ttype = self.get_trigger_type()
@@ -409,15 +413,15 @@
     def get_trigger_delay(self):
         ''' Get the trigger delay of the specified trigger source (in s) '''
         return float(self.query('TIM:MAIN:OFFS?'))
 
     def set_trigger_delay(self, value):
         ''' Set the trigger delay (in s) '''
         self.check_trigger_delay(value)
-        logger.info(f'setting trigger time delay to {si_format(value, 2)}s')
+        self.log(f'setting trigger time delay to {si_format(value, 2)}s')
         self.write(f'TIM:MAIN:OFFS {value}')
 
     def force_trigger(self):
         ''' Force the instrument to make 1 acquisition '''
         self.write('TFOR')
     
     # --------------------- CURSORS ---------------------
@@ -660,15 +664,15 @@
             self.set_waveform_stop(min(npts, pos + self.MAX_BYTE_LEN - 1))
 
             # Query waveform block and append to buffer
             buff += self.get_raw_waveform_buffer()
 
             # Increment position
             pos += self.MAX_BYTE_LEN
-            logger.info(f'waveform acquisition: fetched {len(buff)}/{npts} points from internal memory')
+            self.log(f'waveform acquisition: fetched {len(buff)}/{npts} points from internal memory')
         
         # Return waveform bytes
         return buff
 
     def get_waveform_data(self, ich, **kwargs):
         '''
         Get waveform data from a specific channel
```

### Comparing `instrulink-1.0.3/instrulink/si_utils.py` & `instrulink-1.0.4/instrulink/si_utils.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/instrulink/sutter_mp285a.py` & `instrulink-1.0.4/instrulink/sutter_mp285a.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-04-27 18:16:34
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-05-11 16:03:27
+# @Last Modified time: 2024-05-07 15:31:12
 
 import serial
 import struct
 import time
 import numpy as np
 
 from .logger import logger
@@ -130,14 +130,18 @@
         ''' Set timeout (s) '''
         self.instrument_handle.timeout = value
 
     # def __del__(self):
     #     logger.info(f'releasing {repr(self)} resource')
     #     self.instrument_handle.close() 
 
+    def log(self, msg):
+        ''' Log a message prefixed with with class name '''
+        logger.info(f'{self.__class__.__name__}: {msg}')
+
     def get_name(self):
         ''' Get controller name '''
         return self.__class__.__name__
     
     def write(self, cmd, convert_to_bytes=True):
         ''' Write a command into the serial instrument '''
         logger.debug(f'WRITE: {cmd}')
@@ -309,15 +313,15 @@
         vreq = None
         if tmove_est > self.timeout:
             vreq = int(np.round(dtot / tcr))
             logger.warning(
                 f'increasing velocity temporarily to {vreq} um/s to cover {dtot:.2f} um within {self.TREL_MAX * 1e2:.0f} % of {self.timeout} s timeout')
             self.set_velocity(vreq)
         if not silent:
-            logger.info(f'moving to position: {self.pos_str(pos)} (delta = {self.pos_str(delta)})')
+            self.log(f'moving to position: {self.pos_str(pos)} (delta = {self.pos_str(delta)})')
         bpos = self.encode_position(pos, prefix='m')  # encode position to bytes
         tmove = time.perf_counter()
         self.write_and_check(bpos, convert_to_bytes=False)  # send position to controller
         tmove = time.perf_counter() - tmove
         # Check that target position has been reached
         new_pos = self.get_position()
         new_delta = pos - new_pos
@@ -328,15 +332,15 @@
         if vreq is not None:
             logger.warning(f'resetting velocity to {v} um/s')
             self.set_velocity(v)
     
     def move_to_origin(self):
         ''' Move to origin '''
         self.set_position([0., 0., 0.])
-        logger.info('moved to origin!')
+        self.log('moved to origin!')
     
     def translate(self, v, **kwargs):
         '''
         Translate by some vector
         
         :param v: XYZ translation vector (um) '''
         pos = self.get_position()
@@ -391,48 +395,48 @@
         '''
         # Check that velocity is within bounds
         res = self.get_resolution()
         vbounds = self.get_vbounds(res)
         if not is_within(v, vbounds):
             raise SutterError(
                 f'velocity value ({v} um/s) is out of specific bounds ({vbounds} um/s)')
-        logger.info(f'setting velocity to {v} um/s')
+        self.log(f'setting velocity to {v} um/s')
         self.encode_velocity_and_resolution(v, res)
         vout = self.get_velocity()
         if vout != v:
             raise SutterError(f'could not set motion speed to {v} um/s (value = {vout} um/s)')
     
     def res_str(self, res):
         ''' Return a string representation of controller movement resolution '''
         resmode = {0: 'low', 1: 'high'}[res]
         return f'{resmode}-resolution'
     
     def set_resolution(self, res):
         ''' Set controller motion resolution (0 for low or 1 for high) '''
-        logger.info(f'setting motion mode to {self.res_str(res)}')
+        self.log(f'setting motion mode to {self.res_str(res)}')
         self.encode_velocity_and_resolution(self.get_velocity(), res)
         resout = self.get_resolution()
         if resout != res:
             raise SutterError(f'could not set motion mode to {self.res_str(res)} (value = {self.res_str(resout)})')
 
     def refresh_panel(self):
         ''' Refresh XYZ info on the front panel '''
         self.write_and_check('n')
     
     def set_origin(self):
         ''' Set origin of the coordinate system to the current position '''
         self.write_and_check('o')
-        logger.info('origin reset!')
+        self.log('origin reset!')
     
     def reset(self):
         ''' Reset controller '''
         self.write('r')  # controller does not reply
     
     def set_absolute_mode(self):
         ''' Set the movement mode to absolute '''
-        logger.info('setting absolute movement mode')
+        self.log('setting absolute movement mode')
         self.write_and_check('a')
     
     def set_relative_mode(self):
         ''' Set the movement mode to relative '''
-        logger.info('setting relative movement mode')
+        self.log('setting relative movement mode')
         self.write_and_check('b')
```

### Comparing `instrulink-1.0.3/instrulink/utils.py` & `instrulink-1.0.4/instrulink/utils.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/instrulink/visa_instrument.py` & `instrulink-1.0.4/instrulink/visa_instrument.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-03-15 09:26:06
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-05-11 16:57:22
+# @Last Modified time: 2024-05-07 15:24:58
 
 import abc
 import pyvisa
 import time
 import re
 import threading
 import numpy as np
@@ -190,14 +190,18 @@
         ''' Get I/O operations timeout paramerer (in ms) '''
         return self.instrument_handle.timeout
     
     @timeout.setter
     def timeout(self, value):
         ''' Set I/O operations timeout paramerer (in ms) '''
         self.instrument_handle.timeout = value
+    
+    def log(self, msg):
+        ''' Log a message prefixed with with class name '''
+        logger.info(f'{self.__class__.__name__}: {msg}')
 
     # --------------------- I/O PROCESSING ---------------------
 
     def si_process(self, val):
         ''' Process an input value to be set '''
         return si_format(val, space='').upper()
```

### Comparing `instrulink-1.0.3/instrulink/waveform_generator.py` & `instrulink-1.0.4/instrulink/waveform_generator.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/instrulink/wf_utils.py` & `instrulink-1.0.4/instrulink/wf_utils.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/instrulink.egg-info/PKG-INFO` & `instrulink-1.0.4/instrulink.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: instrulink
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package to interface diverse laboratory instruments
 Home-page: https://github.com/tjjlemaire/instrulink
 Author: Theo Lemaire
 Author-email: theo.lemaire1@gmail.com
 License: MIT
 Keywords: laboratory instrument interface python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: colorlog
+Requires-Dist: pyvisa
+Requires-Dist: pyserial
+Requires-Dist: matplotlib
+Requires-Dist: nidaqmx
 
 # instrulink
 
 This python package provides built-in classes to interface diverse laboratory instruments, including:
 - **waveform generators**: [Rigol DG 1022Z](https://www.rigolna.com/products/waveform-generators/dg1000z/) (`RigolDG1022Z`)
 - **oscilloscopes**: [B&K Precision 2555](https://www.bkprecision.com/products/oscilloscopes/2555) (`BK2555`), [Rigol DS 1054Z](https://www.rigolna.com/products/digital-oscilloscopes/1000z/) (`RigolDS1054Z`)
 - **micro-manipulators**: [Sutter Instruments MP-285A](https://www.sutter.com/MICROMANIPULATION/mp285_frame.html) (`SutterMP285A`)
```

### Comparing `instrulink-1.0.3/instrulink.egg-info/SOURCES.txt` & `instrulink-1.0.4/instrulink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/scripts/test_33500b.py` & `instrulink-1.0.4/scripts/test_33500b.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/scripts/test_camera.py` & `instrulink-1.0.4/scripts/test_camera.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/scripts/test_e5061b.py` & `instrulink-1.0.4/scripts/test_e5061b.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/scripts/test_generator.py` & `instrulink-1.0.4/scripts/test_generator.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/scripts/test_manipulator.py` & `instrulink-1.0.4/scripts/test_manipulator.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/scripts/test_nidaq.py` & `instrulink-1.0.4/scripts/test_nidaq.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/scripts/test_scope.py` & `instrulink-1.0.4/scripts/test_scope.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/scripts/test_smoothed_waveform.py` & `instrulink-1.0.4/scripts/test_smoothed_waveform.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0.3/setup.py` & `instrulink-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Email: theo.lemaire@epfl.ch
 # @Date:   2017-06-13 09:40:02
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-08-09 17:12:23
+# @Last Modified time: 2024-05-08 19:02:30
 
 import os
 from setuptools import setup
 
 readme_file = 'README.md'
 req_file = 'requirements.txt'
 
@@ -21,15 +21,15 @@
         return f.readlines()
 
 def getFiles(path):
     return [f'{path}/{x}' for x in os.listdir(path)]
 
 setup(
     name='instrulink',
-    version='1.0.3',
+    version='1.0.4',
     description='Python package to interface diverse laboratory instruments',
     long_description_content_type='text/markdown',
     long_description=readme(),
     url='https://github.com/tjjlemaire/instrulink',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
```

