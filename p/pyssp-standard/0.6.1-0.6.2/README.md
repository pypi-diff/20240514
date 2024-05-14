# Comparing `tmp/pyssp_standard-0.6.1.tar.gz` & `tmp/pyssp_standard-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyssp_standard-0.6.1.tar", last modified: Sat Mar 23 17:41:41 2024, max compression
+gzip compressed data, was "pyssp_standard-0.6.2.tar", last modified: Tue May 14 20:05:11 2024, max compression
```

## Comparing `pyssp_standard-0.6.1.tar` & `pyssp_standard-0.6.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 17:41:41.630550 pyssp_standard-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-23 17:41:41.626550 pyssp_standard-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 17:41:41.626550 pyssp_standard-0.6.1/pyssp_standard/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/common_content_ssc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/fmu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/parameter_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/srmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/ssb.py
--rw-r--r--   0 runner    (1001) docker     (127)     9733 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/ssd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/ssm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/ssp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/ssv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/transformation_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-03-23 17:41:36.000000 pyssp_standard-0.6.1/pyssp_standard/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 17:41:41.626550 pyssp_standard-0.6.1/pyssp_standard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-23 17:41:41.000000 pyssp_standard-0.6.1/pyssp_standard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-23 17:41:41.000000 pyssp_standard-0.6.1/pyssp_standard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 17:41:41.000000 pyssp_standard-0.6.1/pyssp_standard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-23 17:41:41.000000 pyssp_standard-0.6.1/pyssp_standard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-23 17:41:41.000000 pyssp_standard-0.6.1/pyssp_standard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-23 17:41:41.630550 pyssp_standard-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-23 17:41:37.000000 pyssp_standard-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:05:11.215636 pyssp_standard-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-14 20:05:11.215636 pyssp_standard-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:05:11.215636 pyssp_standard-0.6.2/pyssp_standard/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/common_content_ssc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/fmu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/parameter_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/srmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/ssb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/ssd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/ssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/ssp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/ssv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/transformation_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/pyssp_standard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:05:11.215636 pyssp_standard-0.6.2/pyssp_standard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-14 20:05:11.000000 pyssp_standard-0.6.2/pyssp_standard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-14 20:05:11.000000 pyssp_standard-0.6.2/pyssp_standard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:05:11.000000 pyssp_standard-0.6.2/pyssp_standard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 20:05:11.000000 pyssp_standard-0.6.2/pyssp_standard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 20:05:11.000000 pyssp_standard-0.6.2/pyssp_standard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 20:05:11.215636 pyssp_standard-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-14 20:05:03.000000 pyssp_standard-0.6.2/setup.py
```

### Comparing `pyssp_standard-0.6.1/LICENSE` & `pyssp_standard-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/PKG-INFO` & `pyssp_standard-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyssp_standard
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simple python package for reading, modifying and creating files, specified in the SSP Standard
 Home-page: https://github.com/FGHaider/pyssp
 Download-URL: https://github.com/FGHaider/pyssp/archive/refs/tags/v_01.tar.gz
 Author: Fredrik Haider
 Author-email: 
 License: MIT
 Keywords: SSP,system,engineering
```

### Comparing `pyssp_standard-0.6.1/README.md` & `pyssp_standard-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/pyssp_standard/common_content_ssc.py` & `pyssp_standard-0.6.2/pyssp_standard/common_content_ssc.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/pyssp_standard/fmu.py` & `pyssp_standard-0.6.2/pyssp_standard/fmu.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/pyssp_standard/parameter_types.py` & `pyssp_standard-0.6.2/pyssp_standard/parameter_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
         if type(parameter_type) is ET.Element:
             self.parameter_type = parameter_type.tag.split('}')[-1]
             self.parameter = self.__create_parameter__(self.parameter_type, parameter_type.attrib)
         elif type(parameter_type) is str:
             self.parameter_type = parameter_type
             self.parameter = self.__create_parameter__(parameter_type, attributes)
+        else:
+            raise Exception(f"No parameter type is provided attribs: {attributes}")
 
     def element(self):
         if self.namespace == 'ssc':
             return ET.Element(QName(self.namespaces[self.namespace], self.parameter_type))
         else:
             return ET.Element(QName(self.namespaces[self.namespace], self.parameter_type), attrib=self.parameter)
```

### Comparing `pyssp_standard-0.6.1/pyssp_standard/srmd.py` & `pyssp_standard-0.6.2/pyssp_standard/srmd.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/pyssp_standard/ssb.py` & `pyssp_standard-0.6.2/pyssp_standard/ssb.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/pyssp_standard/ssd.py` & `pyssp_standard-0.6.2/pyssp_standard/ssd.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,28 +109,32 @@
 
 
 class System(ModelicaStandard):
 
     def __init__(self, system_element: ET.Element):
         self.name = None
         self.element = None
-        self.__connections = []
+        self.__connections : list[Connection] = []
 
-        self.connectors = []
+        self.connectors : list[Connector] = []
         self.parameter_bindings = []
         self.signal_dictionaries = []
 
         self.__read__(system_element)
 
     def __read__(self, element):
+        self.name = element.get('name', None)
         elements = element.findall('ssd:Elements', namespaces=self.namespaces)
-        self.element = Element(elements[0])
+        if len(elements) > 0:
+            self.element = Element(elements[0])
+
         connections = element.findall('ssd:Connections', namespaces=self.namespaces)
-        for connection in connections[0].findall('ssd:Connection', namespaces=self.namespaces):
-            self.__connections.append(Connection(connection))
+        if len(connections) > 0:
+            for connection in connections[0].findall('ssd:Connection', namespaces=self.namespaces):
+                self.__connections.append(Connection(connection))
 
     @property
     def connections(self):
         return self.__connections
 
 
 class DefaultExperiment(ModelicaStandard):
```

### Comparing `pyssp_standard-0.6.1/pyssp_standard/ssm.py` & `pyssp_standard-0.6.2/pyssp_standard/ssm.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/pyssp_standard/ssp.py` & `pyssp_standard-0.6.2/pyssp_standard/ssp.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/pyssp_standard/ssv.py` & `pyssp_standard-0.6.2/pyssp_standard/ssv.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,16 @@
             parameter_dict['value'] = str(value)
         if name is not None:
             parameter_dict['name'] = name
         if mimetype is not None:
             parameter_dict['mimetype'] = mimetype
         if unit is not None:
             parameter_dict['unit'] = unit
-        self.__parameters.append(Parameter(name=parname, type_name=ptype,
-                                           type_value=ParameterType(ptype, parameter_dict)))
+        p = Parameter(name=parname, type_name=ptype, type_value=ParameterType(ptype, parameter_dict))
+        self.__parameters.append(p)
 
     def add_unit(self, name: str, base_unit: dict = None):
         """
         Add a unit definition to the .ssv file. If base_unit is None, an attempt is made to automatically generate a BaseUnit.
         :param name: e.g. N or J/kg/K
         :param base_unit: A dictionary declaring the base unit as specified by the SSP standard.
         """
```

### Comparing `pyssp_standard-0.6.1/pyssp_standard/standard.py` & `pyssp_standard-0.6.2/pyssp_standard/standard.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/pyssp_standard/transformation_types.py` & `pyssp_standard-0.6.2/pyssp_standard/transformation_types.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/pyssp_standard/unit.py` & `pyssp_standard-0.6.2/pyssp_standard/unit.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/pyssp_standard/unit_conversion.py` & `pyssp_standard-0.6.2/pyssp_standard/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/pyssp_standard/utils.py` & `pyssp_standard-0.6.2/pyssp_standard/utils.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/pyssp_standard.egg-info/PKG-INFO` & `pyssp_standard-0.6.2/pyssp_standard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyssp_standard
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simple python package for reading, modifying and creating files, specified in the SSP Standard
 Home-page: https://github.com/FGHaider/pyssp
 Download-URL: https://github.com/FGHaider/pyssp/archive/refs/tags/v_01.tar.gz
 Author: Fredrik Haider
 Author-email: 
 License: MIT
 Keywords: SSP,system,engineering
```

### Comparing `pyssp_standard-0.6.1/pyssp_standard.egg-info/SOURCES.txt` & `pyssp_standard-0.6.2/pyssp_standard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.6.1/setup.py` & `pyssp_standard-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='pyssp_standard',
     packages=['pyssp_standard'],
-    version='0.6.1',
+    version='0.6.2',
     license='MIT',
     description='Simple python package for reading, modifying and creating files, specified in the SSP Standard',
     long_description='',
     long_description_content_type='text/markdown',
     author='Fredrik Haider',
     author_email='',
     url='https://github.com/FGHaider/pyssp',
```

