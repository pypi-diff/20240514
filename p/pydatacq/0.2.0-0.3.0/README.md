# Comparing `tmp/pydatacq-0.2.0.tar.gz` & `tmp/pydatacq-0.3.0.tar.gz`

## Comparing `pydatacq-0.2.0.tar` & `pydatacq-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0  4487098 2020-02-02 00:00:00.000000 pydatacq-0.2.0/resources/fft.mp4
--rw-r--r--   0        0        0  3412266 2020-02-02 00:00:00.000000 pydatacq-0.2.0/resources/fm_sine.mp4
--rw-r--r--   0        0        0  2480308 2020-02-02 00:00:00.000000 pydatacq-0.2.0/resources/thd.mp4
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/demo_fm_sine.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/fft.py
--rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/fft_calculations.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/live_fm_sine.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/matplotlib_rc.py
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/osc.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/thd.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/pydatacq/__init__.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/pydatacq/live_data.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/pydatacq/live_sds.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/pydatacq/live_window.py
--rw-r--r--   0        0        0    17738 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/pydatacq/sds.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/pydatacq/siglent.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pydatacq-0.2.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pydatacq-0.2.0/LICENSE
--rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 pydatacq-0.2.0/README.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pydatacq-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    14431 2020-02-02 00:00:00.000000 pydatacq-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0  4487098 2020-02-02 00:00:00.000000 pydatacq-0.3.0/resources/fft.mp4
+-rw-r--r--   0        0        0  3412266 2020-02-02 00:00:00.000000 pydatacq-0.3.0/resources/fm_sine.mp4
+-rw-r--r--   0        0        0  2480308 2020-02-02 00:00:00.000000 pydatacq-0.3.0/resources/thd.mp4
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/examples/demo_fm_sine.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/examples/fft.py
+-rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/examples/fft_calculations.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/examples/live_fm_sine.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/examples/matplotlib_rc.py
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/examples/osc.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/examples/thd.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/pydatacq/__init__.py
+-rw-r--r--   0        0        0     6937 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/pydatacq/live_data.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/pydatacq/live_sds.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/pydatacq/live_window.py
+-rw-r--r--   0        0        0    17805 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/pydatacq/sds.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pydatacq-0.3.0/src/pydatacq/siglent.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pydatacq-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pydatacq-0.3.0/LICENSE
+-rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 pydatacq-0.3.0/README.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pydatacq-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    14431 2020-02-02 00:00:00.000000 pydatacq-0.3.0/PKG-INFO
```

### Comparing `pydatacq-0.2.0/resources/fft.mp4` & `pydatacq-0.3.0/resources/fft.mp4`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/resources/fm_sine.mp4` & `pydatacq-0.3.0/resources/fm_sine.mp4`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/resources/thd.mp4` & `pydatacq-0.3.0/resources/thd.mp4`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/src/examples/demo_fm_sine.py` & `pydatacq-0.3.0/src/examples/demo_fm_sine.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/src/examples/fft.py` & `pydatacq-0.3.0/src/examples/fft.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/src/examples/fft_calculations.py` & `pydatacq-0.3.0/src/examples/fft_calculations.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/src/examples/live_fm_sine.py` & `pydatacq-0.3.0/src/examples/live_fm_sine.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/src/examples/matplotlib_rc.py` & `pydatacq-0.3.0/src/examples/matplotlib_rc.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/src/examples/osc.py` & `pydatacq-0.3.0/src/examples/osc.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/src/examples/thd.py` & `pydatacq-0.3.0/src/examples/thd.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/src/pydatacq/live_data.py` & `pydatacq-0.3.0/src/pydatacq/live_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,21 +33,14 @@
     be set upon instantiation.
 
     By default the uvloop implementation for the event loop will be
     used because of its higher speed. This can be disabled at
     instantiation of the class.
     '''
 
-    _go_on = True
-    __updates = 0
-
-    # interval for fps display
-    __fps_interval = 1 # seconds
-    __consumer_cb = None
-
     #
     def __init__(self,consumer_cb,id=None,fps=False,queue_maxsize=1,
                  timestamp=False,use_uvloop=True,yields=True):
         '''
         This does not start the data acquisition yet. Use start() for that.
 
         Parameters:
@@ -81,14 +74,17 @@
                      which seems to be faster that the default asyncio
                      event loop. If False, will use asyncio's event loop.
         yields :    Should return False if get_data() never yields.
         '''
         self.__consumer_cb = consumer_cb
         if use_uvloop:
             asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+        self.__fps_interval = 1
+        self.__updates = 0
+        self._go_on = True
         self.__fps = fps
         self.__queue_maxsize = queue_maxsize
         self.__timestamp = timestamp
         self._yields = yields
         self._id = id if id is not None else type(self).__name__
```

### Comparing `pydatacq-0.2.0/src/pydatacq/live_sds.py` & `pydatacq-0.3.0/src/pydatacq/live_sds.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     
     # 
     def _next_channel(self):
         '''
         Yields the next channel for which to retrieve data.
         It cycles through all the channels in self.channels.
         '''
-        while super()._go_on:
+        while self._go_on:
             for ch in self.channels:
                 yield ch
         yield None
 
 
     # 
     async def get_data(self):
```

### Comparing `pydatacq-0.2.0/src/pydatacq/live_window.py` & `pydatacq-0.3.0/src/pydatacq/live_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 class LiveWindow():
     '''
     Shows a non-blocking matplotlib window.
     Artists can be presented to the draw() method
     where they will be shown by blitting.
     '''
 
-    fig = None
-    ax = None
-
     #
     def __init__(self,windowTitle=None,plotTitle=None,onclose_cb=None):
         '''
         Parameters:
 
         windowTitle : title of the matplotlib window
         plotTitle : title of the plot
```

### Comparing `pydatacq-0.2.0/src/pydatacq/sds.py` & `pydatacq-0.3.0/src/pydatacq/sds.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,20 @@
 
     This class has only been tested on the SDS1202X-E model.
 
     See the "SDS1000 Series & SDS2000X & SDS2000X-E ProgrammingGuide PG01-E02D.pdf"
     which can be downloaded from https://www.siglent.com/upload_file/document/SDS1000%20Series&SDS2000X&SDS2000X-E_ProgrammingGuide_PG01-E02D.pdf
     '''
 
-    _divisions = 14
-    _channel = 0
+
+    # 
+    def __init__(self,ip,port):
+        self._divisions = 14
+        super().__init__(ip,port)
+
 
     # This translates the display value (-127..128) to a voltage.
     def _toV(self,x,vgain,voffset,probe_att):
         return (x / 128 * vgain * 5 - voffset) * probe_att
 
 
     #
```

### Comparing `pydatacq-0.2.0/src/pydatacq/siglent.py` & `pydatacq-0.3.0/src/pydatacq/siglent.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/LICENSE` & `pydatacq-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/README.md` & `pydatacq-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pydatacq-0.2.0/pyproject.toml` & `pydatacq-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pydatacq"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="kvdijken", email="sla_nippers_0x@icloud.com" },
 ]
 dependencies = ["numpy","scipy","uvloop","matplotlib","quantiphy"]
 
 description = "A package for asynchronous data acquisition"
 readme = "README.md"
```

### Comparing `pydatacq-0.2.0/PKG-INFO` & `pydatacq-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydatacq
-Version: 0.2.0
+Version: 0.3.0
 Summary: A package for asynchronous data acquisition
 Project-URL: Homepage, https://github.com/kvdijken/pydatacq
 Author-email: kvdijken <sla_nippers_0x@icloud.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

