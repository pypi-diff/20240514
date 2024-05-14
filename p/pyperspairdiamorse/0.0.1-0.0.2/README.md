# Comparing `tmp/pyperspairdiamorse-0.0.1.tar.gz` & `tmp/pyperspairdiamorse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyperspairdiamorse-0.0.1.tar", last modified: Sun May  5 13:02:38 2024, max compression
+gzip compressed data, was "pyperspairdiamorse-0.0.2.tar", last modified: Tue May 14 21:24:01 2024, max compression
```

## Comparing `pyperspairdiamorse-0.0.1.tar` & `pyperspairdiamorse-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0 ananev    (1000) ananev    (1000)        0 2024-05-05 13:02:38.550153 pyperspairdiamorse-0.0.1/
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)    35821 2023-10-30 16:40:18.000000 pyperspairdiamorse-0.0.1/LICENSE.txt
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     1737 2024-05-05 13:02:38.548147 pyperspairdiamorse-0.0.1/PKG-INFO
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     1088 2024-05-04 15:55:37.000000 pyperspairdiamorse-0.0.1/README.md
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)       38 2024-05-05 13:02:38.551152 pyperspairdiamorse-0.0.1/setup.cfg
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     2428 2024-05-05 13:02:10.000000 pyperspairdiamorse-0.0.1/setup.py
-drwxrwxrwx   0 ananev    (1000) ananev    (1000)        0 2024-05-05 13:02:38.132682 pyperspairdiamorse-0.0.1/src/
-drwxrwxrwx   0 ananev    (1000) ananev    (1000)        0 2024-05-05 13:02:38.165755 pyperspairdiamorse-0.0.1/src/baselib/
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)        0 2023-10-30 16:40:19.000000 pyperspairdiamorse-0.0.1/src/baselib/__init__.py
-drwxrwxrwx   0 ananev    (1000) ananev    (1000)        0 2024-05-05 13:02:38.418870 pyperspairdiamorse-0.0.1/src/baselib/include/
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)    11157 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.1/src/baselib/include/CubicalComplex.hpp
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     5734 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.1/src/baselib/include/MorseVectorField.hpp
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     1583 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.1/src/baselib/include/PackedMap.hpp
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     5971 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.1/src/baselib/include/SEDT.hpp
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     1834 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.1/src/baselib/include/SimpleComplex.hpp
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     1926 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.1/src/baselib/include/VertexMap.hpp
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     2986 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.1/src/baselib/include/chainComplexExtraction.hpp
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     1465 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.1/src/baselib/include/collections.hpp
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)    10858 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.1/src/baselib/include/persistence.hpp
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     3503 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.1/src/baselib/include/restricted.hpp
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     6405 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.1/src/baselib/include/traversals.hpp
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     7303 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.1/src/baselib/include/vectorFieldExtraction.hpp
-drwxrwxrwx   0 ananev    (1000) ananev    (1000)        0 2024-05-05 13:02:38.156217 pyperspairdiamorse-0.0.1/src/pyperspairdiamorse/
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     3289 2024-05-05 12:50:34.000000 pyperspairdiamorse-0.0.1/src/pyperspairdiamorse/pyperspairdiamorse.cpp
-drwxrwxrwx   0 ananev    (1000) ananev    (1000)        0 2024-05-05 13:02:38.525440 pyperspairdiamorse-0.0.1/src/pyperspairdiamorse.egg-info/
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)     1737 2024-05-05 13:02:37.000000 pyperspairdiamorse-0.0.1/src/pyperspairdiamorse.egg-info/PKG-INFO
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)      830 2024-05-05 13:02:37.000000 pyperspairdiamorse-0.0.1/src/pyperspairdiamorse.egg-info/SOURCES.txt
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)        1 2024-05-05 13:02:37.000000 pyperspairdiamorse-0.0.1/src/pyperspairdiamorse.egg-info/dependency_links.txt
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)       64 2024-05-05 13:02:37.000000 pyperspairdiamorse-0.0.1/src/pyperspairdiamorse.egg-info/entry_points.txt
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)        6 2024-05-05 13:02:37.000000 pyperspairdiamorse-0.0.1/src/pyperspairdiamorse.egg-info/requires.txt
--rwxrwxrwx   0 ananev    (1000) ananev    (1000)       27 2024-05-05 13:02:37.000000 pyperspairdiamorse-0.0.1/src/pyperspairdiamorse.egg-info/top_level.txt
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-05-14 21:24:01.916282 pyperspairdiamorse-0.0.2/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35821 2023-10-30 16:40:18.000000 pyperspairdiamorse-0.0.2/LICENSE.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1737 2024-05-14 21:24:01.915952 pyperspairdiamorse-0.0.2/PKG-INFO
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1088 2024-05-04 15:55:37.000000 pyperspairdiamorse-0.0.2/README.md
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2024-05-14 21:24:01.916509 pyperspairdiamorse-0.0.2/setup.cfg
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2428 2024-05-14 21:23:11.000000 pyperspairdiamorse-0.0.2/setup.py
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-05-14 21:24:01.894707 pyperspairdiamorse-0.0.2/src/
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-05-14 21:24:01.898701 pyperspairdiamorse-0.0.2/src/baselib/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2023-10-30 16:40:19.000000 pyperspairdiamorse-0.0.2/src/baselib/__init__.py
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-05-14 21:24:01.909526 pyperspairdiamorse-0.0.2/src/baselib/include/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11157 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.2/src/baselib/include/CubicalComplex.hpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5734 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.2/src/baselib/include/MorseVectorField.hpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1583 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.2/src/baselib/include/PackedMap.hpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5971 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.2/src/baselib/include/SEDT.hpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1834 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.2/src/baselib/include/SimpleComplex.hpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1926 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.2/src/baselib/include/VertexMap.hpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2986 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.2/src/baselib/include/chainComplexExtraction.hpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1465 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.2/src/baselib/include/collections.hpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10858 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.2/src/baselib/include/persistence.hpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3503 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.2/src/baselib/include/restricted.hpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6405 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.2/src/baselib/include/traversals.hpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7303 2024-05-04 16:00:56.000000 pyperspairdiamorse-0.0.2/src/baselib/include/vectorFieldExtraction.hpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-05-14 21:24:01.897853 pyperspairdiamorse-0.0.2/src/pyperspairdiamorse/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3155 2024-05-14 21:20:23.000000 pyperspairdiamorse-0.0.2/src/pyperspairdiamorse/pyperspairdiamorse.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-05-14 21:24:01.914943 pyperspairdiamorse-0.0.2/src/pyperspairdiamorse.egg-info/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1737 2024-05-14 21:24:01.000000 pyperspairdiamorse-0.0.2/src/pyperspairdiamorse.egg-info/PKG-INFO
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      876 2024-05-14 21:24:01.000000 pyperspairdiamorse-0.0.2/src/pyperspairdiamorse.egg-info/SOURCES.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)        1 2024-05-14 21:24:01.000000 pyperspairdiamorse-0.0.2/src/pyperspairdiamorse.egg-info/dependency_links.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       64 2024-05-14 21:24:01.000000 pyperspairdiamorse-0.0.2/src/pyperspairdiamorse.egg-info/entry_points.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)        6 2024-05-14 21:24:01.000000 pyperspairdiamorse-0.0.2/src/pyperspairdiamorse.egg-info/requires.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       27 2024-05-14 21:24:01.000000 pyperspairdiamorse-0.0.2/src/pyperspairdiamorse.egg-info/top_level.txt
```

### Comparing `pyperspairdiamorse-0.0.1/LICENSE.txt` & `pyperspairdiamorse-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/PKG-INFO` & `pyperspairdiamorse-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperspairdiamorse
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cross-platform C++ library of persistent pair extractor using the diamorse approach
 Home-page: UNKNOWN
 Author: Andrey S. Zubov, Kirill M. Gerke, Andrey A. Ananev
 Author-email: andrey.ananev@phystech.edu
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyperspairdiamorse-0.0.1/README.md` & `pyperspairdiamorse-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/setup.py` & `pyperspairdiamorse-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 import os
 from setuptools import setup, Extension, find_packages
 import pip
 
 
-version = "0.0.1"
+version = "0.0.2"
 libName = "pyperspairdiamorse"
 
 file_dir_path = os.path.dirname(os.path.realpath(__file__))
 
 
 def package_files(directory):
     return [os.path.join(p, f) for p, d, files in os.walk(directory) for f in files]
```

### Comparing `pyperspairdiamorse-0.0.1/src/baselib/include/CubicalComplex.hpp` & `pyperspairdiamorse-0.0.2/src/baselib/include/CubicalComplex.hpp`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/src/baselib/include/MorseVectorField.hpp` & `pyperspairdiamorse-0.0.2/src/baselib/include/MorseVectorField.hpp`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/src/baselib/include/PackedMap.hpp` & `pyperspairdiamorse-0.0.2/src/baselib/include/PackedMap.hpp`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/src/baselib/include/SEDT.hpp` & `pyperspairdiamorse-0.0.2/src/baselib/include/SEDT.hpp`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/src/baselib/include/SimpleComplex.hpp` & `pyperspairdiamorse-0.0.2/src/baselib/include/SimpleComplex.hpp`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/src/baselib/include/VertexMap.hpp` & `pyperspairdiamorse-0.0.2/src/baselib/include/VertexMap.hpp`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/src/baselib/include/chainComplexExtraction.hpp` & `pyperspairdiamorse-0.0.2/src/baselib/include/chainComplexExtraction.hpp`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/src/baselib/include/collections.hpp` & `pyperspairdiamorse-0.0.2/src/baselib/include/collections.hpp`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/src/baselib/include/persistence.hpp` & `pyperspairdiamorse-0.0.2/src/baselib/include/persistence.hpp`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/src/baselib/include/restricted.hpp` & `pyperspairdiamorse-0.0.2/src/baselib/include/restricted.hpp`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/src/baselib/include/traversals.hpp` & `pyperspairdiamorse-0.0.2/src/baselib/include/traversals.hpp`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/src/baselib/include/vectorFieldExtraction.hpp` & `pyperspairdiamorse-0.0.2/src/baselib/include/vectorFieldExtraction.hpp`

 * *Files identical despite different names*

### Comparing `pyperspairdiamorse-0.0.1/src/pyperspairdiamorse/pyperspairdiamorse.cpp` & `pyperspairdiamorse-0.0.2/src/pyperspairdiamorse/pyperspairdiamorse.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,106 +1,102 @@
 #include <Python.h>
-#include <iostream>
 #include <exception>
+#include <iostream>
 #include <numpy/arrayobject.h>
 #include <numpy/ndarrayobject.h>
 #include <numpy/npy_common.h>
 
 #include "PersPairExtractor.h"
 
 static char module_docstring[] = "TBA";
 static char ppe_docstring[] = "TBA";
 
-static PyObject *extract(PyObject *self, PyObject *args, PyObject *keywds)
-{
-    import_array();
-    Py_Initialize();
-
-    PyObject *input_data_py;
-
-    static char *kwlist[] = {"image", NULL};
-    if (!PyArg_ParseTupleAndKeywords(
-            args, keywds, "O", kwlist, &input_data_py))
-        return NULL;
-    std::size_t len = PyArray_SIZE(input_data_py);
-    int dimData = PyArray_NDIM(input_data_py);
-    npy_intp *dim_array = PyArray_DIMS(input_data_py);
-
-    Triplet triplet;
-    if (dimData >= 1)
-        triplet.x = dim_array[0];
-    if (dimData >= 2)
-        triplet.y = dim_array[1];
-    if (dimData >= 3)
-        triplet.z = dim_array[2];
-    input_data_py = PyArray_ContiguousFromAny(input_data_py, NPY_INT32, 0, 0);
-
-    int *PyArrayData = (int *)PyArray_DATA(input_data_py);
-    std::vector<PhaseValue> data(len);
-    for(std::size_t i = 0; i < len; ++i){
-        data[i] = static_cast<PhaseValue>(PyArrayData[i]);
+static PyObject *extract(PyObject *self, PyObject *args, PyObject *keywds) {
+  import_array();
+  Py_Initialize();
+
+  PyObject *input_data_py;
+
+  static char *kwlist[] = {"image", NULL};
+  if (!PyArg_ParseTupleAndKeywords(args, keywds, "O", kwlist, &input_data_py))
+    return NULL;
+  std::size_t len = PyArray_SIZE(input_data_py);
+  int dimData = PyArray_NDIM(input_data_py);
+  npy_intp *dim_array = PyArray_DIMS(input_data_py);
+
+  Triplet triplet;
+  if (dimData >= 1)
+    triplet.x = dim_array[0];
+  if (dimData >= 2)
+    triplet.y = dim_array[1];
+  if (dimData >= 3)
+    triplet.z = dim_array[2];
+  input_data_py = PyArray_ContiguousFromAny(input_data_py, NPY_INT32, 0, 0);
+
+  int *PyArrayData = (int *)PyArray_DATA(input_data_py);
+  std::vector<PhaseValue> data(len);
+  for (std::size_t i = 0; i < len; ++i) {
+    data[i] = static_cast<PhaseValue>(PyArrayData[i]);
+  }
+
+  auto create_empty_numpy_array = []() -> PyObject * {
+    // Создаем пустой массив
+    npy_intp dims[1] = {0}; // размерность массива
+    PyObject *pArray = PyArray_SimpleNew(
+        1, dims, NPY_FLOAT); // создаем пустой массив типа double
+    return pArray;
+  };
+
+  auto fill_array =
+      [create_empty_numpy_array](
+          const std::vector<std::pair<float, float>> &in) -> PyObject * {
+    if (in.empty()) {
+      return create_empty_numpy_array();
     }
+    std::vector<float> out(in.size() * 2);
+    for (std::size_t i = 0; i < in.size(); ++i) {
+      const auto &v = in[i];
+      out[2 * i] = v.first;
+      out[2 * i + 1] = v.second;
+    }
+    npy_intp dims[2] = {in.size(), 2};
+    PyObject *array = PyArray_SimpleNew(2, dims, NPY_FLOAT);
+    memcpy(PyArray_DATA(array), out.data(), in.size() * 2 * sizeof(float));
+    return array;
+  };
+
+  auto result = PersPairExtractor::extract(data, triplet);
+
+  auto ar_pd0 = fill_array(result.pd0);
+  auto ar_pd1 = fill_array(result.pd1);
+  auto ar_pd2 = fill_array(result.pd2);
+
+  PyObject *list_result = PyList_New(3);
+  PyList_SetItem(list_result, 0, ar_pd0);
+  PyList_SetItem(list_result, 1, ar_pd1);
+  PyList_SetItem(list_result, 2, ar_pd2);
 
-    auto create_empty_numpy_array = []()->PyObject* {
-        // Создаем пустой массив
-        npy_intp dims[1] = {0}; // размерность массива
-        PyObject* pArray = PyArray_SimpleNew(1, dims, NPY_FLOAT); // создаем пустой массив типа double
-        return pArray;
-    };
-
-    auto fill_array = [create_empty_numpy_array](const std::vector<std::pair<float,float>>& in) -> PyObject*
-    {   
-        if(in.empty()){
-            return create_empty_numpy_array();
-        }
-        std::vector<float> out(in.size() * 2);
-        for (std::size_t i = 0; i < in.size(); ++i)
-        {   
-            const auto& v = in[i];
-            out[2*i] = v.first;
-            out[2*i + 1] = v.second;
-        }
-        npy_intp dims[2] = {in.size(), 2};
-        PyObject *array = PyArray_SimpleNew(2, dims, NPY_FLOAT);
-        memcpy(PyArray_DATA(array), out.data(), in.size() * 2 * sizeof(float));
-        return array;
-    };
-
-    auto result = PersPairExtractor::extract(data, triplet);
-
-    auto ar_pd0 = fill_array(result.pd0);
-    auto ar_pd1 = fill_array(result.pd1);
-    auto ar_pd2 = fill_array(result.pd2);
-    
-    PyObject *list_result = PyList_New(3);
-    PyList_SetItem(list_result, 0, ar_pd0);
-    PyList_SetItem(list_result, 1, ar_pd1);
-    PyList_SetItem(list_result, 2, ar_pd2);
-
-    return list_result;
+  return list_result;
 }
 
-static void test(PyObject *self, PyObject *args, PyObject *keywds)
-{
-    return;
-}
+static void test(PyObject *self, PyObject *args, PyObject *keywds) { return; }
 
 static PyMethodDef module_methods[] = {
-    {"extract", (PyCFunction)extract, METH_VARARGS | METH_KEYWORDS, ppe_docstring},
+    {"extract", (PyCFunction)extract, METH_VARARGS | METH_KEYWORDS,
+     ppe_docstring},
     {"test", (PyCFunction)test, METH_VARARGS | METH_KEYWORDS, ppe_docstring},
     {NULL, NULL, 0, NULL}};
 
-static struct PyModuleDef moduledef = {PyModuleDef_HEAD_INIT, "pyperspairdiamorse",
-                                       module_docstring, -1, module_methods};
-
-PyMODINIT_FUNC PyInit_pyperspairdiamorse(void)
-{
-    Py_Initialize();
-    import_array();
-    PyObject *module = PyModule_Create(&moduledef);
-    if (!module)
-    {
-        return NULL;
-    }
-    import_array();
-    return module;
+static struct PyModuleDef moduledef = {PyModuleDef_HEAD_INIT,
+                                       "pyperspairdiamorse", module_docstring,
+                                       -1, module_methods};
+
+PyMODINIT_FUNC PyInit_pyperspairdiamorse(void) {
+  Py_Initialize();
+  import_array();
+  PyObject *module = PyModule_Create(&moduledef);
+  if (!module) {
+    return NULL;
+  }
+  import_array();
+  return module;
 }
```

### Comparing `pyperspairdiamorse-0.0.1/src/pyperspairdiamorse.egg-info/PKG-INFO` & `pyperspairdiamorse-0.0.2/src/pyperspairdiamorse.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperspairdiamorse
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cross-platform C++ library of persistent pair extractor using the diamorse approach
 Home-page: UNKNOWN
 Author: Andrey S. Zubov, Kirill M. Gerke, Andrey A. Ananev
 Author-email: andrey.ananev@phystech.edu
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyperspairdiamorse-0.0.1/src/pyperspairdiamorse.egg-info/SOURCES.txt` & `pyperspairdiamorse-0.0.2/src/pyperspairdiamorse.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 src/baselib/include/VertexMap.hpp
 src/baselib/include/chainComplexExtraction.hpp
 src/baselib/include/collections.hpp
 src/baselib/include/persistence.hpp
 src/baselib/include/restricted.hpp
 src/baselib/include/traversals.hpp
 src/baselib/include/vectorFieldExtraction.hpp
+src/pyperspairdiamorse/pyperspairdiamorse.cpp
 src/pyperspairdiamorse.egg-info/PKG-INFO
 src/pyperspairdiamorse.egg-info/SOURCES.txt
 src/pyperspairdiamorse.egg-info/dependency_links.txt
 src/pyperspairdiamorse.egg-info/entry_points.txt
 src/pyperspairdiamorse.egg-info/requires.txt
 src/pyperspairdiamorse.egg-info/top_level.txt
```

