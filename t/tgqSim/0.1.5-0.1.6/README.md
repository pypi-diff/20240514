# Comparing `tmp/tgqSim-0.1.5.tar.gz` & `tmp/tgqSim-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgqSim-0.1.5.tar", last modified: Mon May 13 10:29:30 2024, max compression
+gzip compressed data, was "tgqSim-0.1.6.tar", last modified: Tue May 14 00:55:31 2024, max compression
```

## Comparing `tgqSim-0.1.5.tar` & `tgqSim-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:29:30.022229 tgqSim-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-13 10:29:29.000000 tgqSim-0.1.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-13 10:29:29.000000 tgqSim-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2024-05-13 10:29:30.022229 tgqSim-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-13 10:29:29.000000 tgqSim-0.1.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 10:29:30.022229 tgqSim-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-13 10:29:29.000000 tgqSim-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:29:30.019230 tgqSim-0.1.5/tgqSim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:29:30.021229 tgqSim-0.1.5/tgqSim/GateSimulation/
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim/GateSimulation/DoubleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim/GateSimulation/SingleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim/GateSimulation/TripleGate.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim/GateSimulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22001 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim/QuantumCircuit.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim/draw_circuit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:29:30.021229 tgqSim-0.1.5/tgqSim/lib/
--rw-rw-rw-   0 root         (0) root         (0)    73408 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim/lib/tgq_simulator.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:29:30.020229 tgqSim-0.1.5/tgqSim.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      430 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-13 10:29:29.000000 tgqSim-0.1.5/tgqSim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:55:31.461296 tgqSim-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-14 00:55:30.000000 tgqSim-0.1.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-14 00:55:30.000000 tgqSim-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2024-05-14 00:55:31.461296 tgqSim-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-14 00:55:30.000000 tgqSim-0.1.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 00:55:31.461296 tgqSim-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-14 00:55:30.000000 tgqSim-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:55:31.458296 tgqSim-0.1.6/tgqSim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:55:31.460296 tgqSim-0.1.6/tgqSim/GateSimulation/
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/GateSimulation/DoubleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/GateSimulation/SingleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/GateSimulation/TripleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/GateSimulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22122 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/QuantumCircuit.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/draw_circuit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:55:31.460296 tgqSim-0.1.6/tgqSim/lib/
+-rw-rw-rw-   0 root         (0) root         (0)    61896 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/lib/cuda_11-8_tgq_simulator.so
+-rw-rw-rw-   0 root         (0) root         (0)    73408 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/lib/cuda_12-4_tgq_simulator.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:55:31.459296 tgqSim-0.1.6/tgqSim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2024-05-14 00:55:31.000000 tgqSim-0.1.6/tgqSim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-14 00:55:31.000000 tgqSim-0.1.6/tgqSim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 00:55:31.000000 tgqSim-0.1.6/tgqSim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-14 00:55:31.000000 tgqSim-0.1.6/tgqSim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-14 00:55:31.000000 tgqSim-0.1.6/tgqSim.egg-info/top_level.txt
```

### Comparing `tgqSim-0.1.5/LICENSE` & `tgqSim-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.5/PKG-INFO` & `tgqSim-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.5
+Version: 0.1.6
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `tgqSim-0.1.5/setup.py` & `tgqSim-0.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tgqSim',
-    version='0.1.5',
+    version='0.1.6',
     description='TGQ量子模拟器',  # 包描述
     long_description="Python for quantum simulation http://www.tiangongqs.com",  # 详细描述
     long_description_content_type='text/markdown',
     author='tiangongqs',  # 作者姓名
     license='MIT',  # 许可证
     package=find_packages(),
     include_package_data=True,
```

### Comparing `tgqSim-0.1.5/tgqSim/GateSimulation/DoubleGate.py` & `tgqSim-0.1.6/tgqSim/GateSimulation/DoubleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.5/tgqSim/GateSimulation/SingleGate.py` & `tgqSim-0.1.6/tgqSim/GateSimulation/SingleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.5/tgqSim/GateSimulation/TripleGate.py` & `tgqSim-0.1.6/tgqSim/GateSimulation/TripleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.5/tgqSim/QuantumCircuit.py` & `tgqSim-0.1.6/tgqSim/QuantumCircuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,17 +150,19 @@
         for deviceid in deviceList:
             if deviceid not in gpuidList:
                 raise ValueError("设置设备ID不存在")
         self.isgpu = True
         self.deviceid = deviceList
     
     def _run_with_device(self):
+        cuda_version = GPUtil.get_cuda_version().replace(".", "-")
+        lib_name = f"cuda_{cuda_version}_tgq_simulator.so"
         current_file_path = os.path.abspath(__file__)
         current_directory = os.path.dirname(current_file_path)
-        dll_path = os.path.abspath(current_directory + '/lib/tgq_simulator.so')
+        dll_path = os.path.abspath(current_directory + '/lib/' + lib_name)
         lib = ctypes.CDLL(dll_path)
         lib.execute_circuit.argtypes = [
             ctypes.POINTER(Float2),
             ctypes.POINTER(GateInfo),
             ctypes.c_int,
             ctypes.c_int,
             ctypes.c_int
```

### Comparing `tgqSim-0.1.5/tgqSim/draw_circuit_tools.py` & `tgqSim-0.1.6/tgqSim/draw_circuit_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.5/tgqSim/lib/tgq_simulator.so` & `tgqSim-0.1.6/tgqSim/lib/cuda_12-4_tgq_simulator.so`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.5/tgqSim.egg-info/PKG-INFO` & `tgqSim-0.1.6/tgqSim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.5
+Version: 0.1.6
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

