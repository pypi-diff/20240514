# Comparing `tmp/structstore-0.1.2.tar.gz` & `tmp/structstore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structstore-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "structstore-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `structstore-0.1.2.tar` & `structstore-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     4656 2024-05-14 08:45:24.019774 structstore-0.1.2/CMakeLists.txt
--rw-r--r--   0        0        0     1489 2022-11-06 13:29:39.097613 structstore-0.1.2/LICENSE
--rw-r--r--   0        0        0     3879 2024-05-13 22:03:39.240898 structstore-0.1.2/README.md
--rw-r--r--   0        0        0      709 2024-05-14 08:27:19.167743 structstore-0.1.2/cmake/NanobindStubgen.cmake
--rw-r--r--   0        0        0      462 2024-05-13 21:53:42.800696 structstore-0.1.2/cmake/StructStoreConfig.cmake.in
--rw-r--r--   0        0        0      378 2024-05-13 21:20:28.538842 structstore-0.1.2/cmake/StructStoreConfigVersion.cmake.in
--rw-r--r--   0        0        0      385 2024-05-13 21:43:45.044481 structstore-0.1.2/include/structstore/structstore.hpp
--rw-r--r--   0        0        0    13883 2024-05-13 21:43:45.034481 structstore-0.1.2/include/structstore/stst_alloc.hpp
--rw-r--r--   0        0        0     4772 2024-05-13 21:43:45.004481 structstore-0.1.2/include/structstore/stst_containers.hpp
--rw-r--r--   0        0        0     4721 2024-05-13 21:43:45.094481 structstore-0.1.2/include/structstore/stst_field.hpp
--rw-r--r--   0        0        0     1178 2024-05-13 21:07:08.207963 structstore-0.1.2/include/structstore/stst_hashstring.hpp
--rw-r--r--   0        0        0     1578 2024-05-13 21:07:08.201296 structstore-0.1.2/include/structstore/stst_lock.hpp
--rw-r--r--   0        0        0     1255 2024-05-13 21:43:45.071147 structstore-0.1.2/include/structstore/stst_serialization.hpp
--rw-r--r--   0        0        0     4230 2024-05-13 21:43:45.084481 structstore-0.1.2/include/structstore/stst_shared.hpp
--rw-r--r--   0        0        0     5402 2024-05-13 21:43:45.104481 structstore-0.1.2/include/structstore/stst_structstore.hpp
--rw-r--r--   0        0        0     1422 2024-05-14 07:45:17.149944 structstore-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1250 2022-11-18 12:53:02.673000 structstore-0.1.2/src/main.bak.cpp
--rw-r--r--   0        0        0     1355 2022-11-20 10:32:04.499910 structstore-0.1.2/src/main.cpp
--rw-r--r--   0        0        0     1024 2024-05-13 21:43:45.054481 structstore-0.1.2/src/structstore.cpp
--rw-r--r--   0        0        0      246 2024-05-14 08:45:37.725425 structstore-0.1.2/src/structstore/__init__.py
--rw-r--r--   0        0        0    16900 2024-05-14 08:43:18.453931 structstore-0.1.2/src/structstore_bindings.cpp
--rw-r--r--   0        0        0      975 2024-05-13 21:43:44.997814 structstore-0.1.2/src/structstore_containers.cpp
--rw-r--r--   0        0        0      336 2024-05-13 21:43:45.064481 structstore-0.1.2/src/structstore_field.cpp
--rw-r--r--   0        0        0     2644 2024-05-13 21:43:45.017814 structstore-0.1.2/src/structstore_serialization.cpp
--rw-r--r--   0        0        0     8919 2024-05-13 21:43:45.027814 structstore-0.1.2/src/structstore_shared.cpp
--rw-r--r--   0        0        0     4220 1970-01-01 00:00:00.000000 structstore-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4654 2024-05-14 10:52:56.843891 structstore-0.1.3/CMakeLists.txt
+-rw-r--r--   0        0        0     1489 2022-11-06 13:29:39.097613 structstore-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3879 2024-05-13 22:03:39.240898 structstore-0.1.3/README.md
+-rw-r--r--   0        0        0      709 2024-05-14 08:27:19.167743 structstore-0.1.3/cmake/NanobindStubgen.cmake
+-rw-r--r--   0        0        0      462 2024-05-13 21:53:42.800696 structstore-0.1.3/cmake/StructStoreConfig.cmake.in
+-rw-r--r--   0        0        0      378 2024-05-13 21:20:28.538842 structstore-0.1.3/cmake/StructStoreConfigVersion.cmake.in
+-rw-r--r--   0        0        0      385 2024-05-13 21:43:45.044481 structstore-0.1.3/include/structstore/structstore.hpp
+-rw-r--r--   0        0        0    13883 2024-05-13 21:43:45.034481 structstore-0.1.3/include/structstore/stst_alloc.hpp
+-rw-r--r--   0        0        0     4778 2024-05-14 09:32:31.984724 structstore-0.1.3/include/structstore/stst_containers.hpp
+-rw-r--r--   0        0        0     4721 2024-05-13 21:43:45.094481 structstore-0.1.3/include/structstore/stst_field.hpp
+-rw-r--r--   0        0        0     1178 2024-05-13 21:07:08.207963 structstore-0.1.3/include/structstore/stst_hashstring.hpp
+-rw-r--r--   0        0        0     1578 2024-05-14 10:53:18.590588 structstore-0.1.3/include/structstore/stst_lock.hpp
+-rw-r--r--   0        0        0     1255 2024-05-13 21:43:45.071147 structstore-0.1.3/include/structstore/stst_serialization.hpp
+-rw-r--r--   0        0        0     4230 2024-05-13 21:43:45.084481 structstore-0.1.3/include/structstore/stst_shared.hpp
+-rw-r--r--   0        0        0     5402 2024-05-13 21:43:45.104481 structstore-0.1.3/include/structstore/stst_structstore.hpp
+-rw-r--r--   0        0        0     1422 2024-05-14 07:45:17.149944 structstore-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1250 2022-11-18 12:53:02.673000 structstore-0.1.3/src/main.bak.cpp
+-rw-r--r--   0        0        0     1355 2022-11-20 10:32:04.499910 structstore-0.1.3/src/main.cpp
+-rw-r--r--   0        0        0     1024 2024-05-13 21:43:45.054481 structstore-0.1.3/src/structstore.cpp
+-rw-r--r--   0        0        0      246 2024-05-14 08:55:55.247860 structstore-0.1.3/src/structstore/__init__.py
+-rw-r--r--   0        0        0    16977 2024-05-14 11:06:51.575343 structstore-0.1.3/src/structstore_bindings.cpp
+-rw-r--r--   0        0        0      975 2024-05-13 21:43:44.997814 structstore-0.1.3/src/structstore_containers.cpp
+-rw-r--r--   0        0        0      336 2024-05-13 21:43:45.064481 structstore-0.1.3/src/structstore_field.cpp
+-rw-r--r--   0        0        0     2644 2024-05-13 21:43:45.017814 structstore-0.1.3/src/structstore_serialization.cpp
+-rw-r--r--   0        0        0     8919 2024-05-13 21:43:45.027814 structstore-0.1.3/src/structstore_shared.cpp
+-rw-r--r--   0        0        0     4220 1970-01-01 00:00:00.000000 structstore-0.1.3/PKG-INFO
```

### Comparing `structstore-0.1.2/CMakeLists.txt` & `structstore-0.1.3/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cmake_minimum_required(VERSION 3.10)
-project(structstore VERSION 0.1.2)
+project(structstore VERSION 0.1.3)
 
 set(PY_VERSION_SUFFIX "")
 set(PY_FULL_VERSION ${PROJECT_VERSION}${PY_VERSION_SUFFIX})
 
 # make sure that the Python and CMake versions match
 if (DEFINED PY_BUILD_CMAKE_PACKAGE_VERSION)
     if (NOT "${PY_BUILD_CMAKE_PACKAGE_VERSION}" MATCHES "^${PY_FULL_VERSION}$")
@@ -96,15 +96,15 @@
         COMPONENT python_modules
         DESTINATION ${STRUCTSTORE_INSTALL_DIR})
 
 include(cmake/NanobindStubgen.cmake)
 nanobind_stubgen(structstore_bindings)
 nanobind_stubgen_install(structstore_bindings ${STRUCTSTORE_INSTALL_DIR})
 
-# inspired from https://stackoverflow.com/a/49857699
+# inspired by https://stackoverflow.com/a/49857699
 export(TARGETS structstore_lib
         FILE "${PROJECT_BINARY_DIR}/StructStoreTargets.cmake")
 export(PACKAGE StructStore)
 configure_file(${PROJECT_SOURCE_DIR}/cmake/StructStoreConfig.cmake.in
         "${PROJECT_BINARY_DIR}/StructStoreConfig.cmake" @ONLY)
 configure_file(${PROJECT_SOURCE_DIR}/cmake/StructStoreConfigVersion.cmake.in
         "${PROJECT_BINARY_DIR}/StructStoreConfigVersion.cmake" @ONLY)
```

### Comparing `structstore-0.1.2/LICENSE` & `structstore-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/README.md` & `structstore-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/cmake/NanobindStubgen.cmake` & `structstore-0.1.3/cmake/NanobindStubgen.cmake`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/include/structstore/stst_alloc.hpp` & `structstore-0.1.3/include/structstore/stst_alloc.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/include/structstore/stst_containers.hpp` & `structstore-0.1.3/include/structstore/stst_containers.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
     size_t rows() const { return _rows; }
 
     size_t cols() const { return _cols; }
 
     bool is_vector() const { return _is_vector; }
 
-    void from(size_t rows, size_t cols, double* data, bool is_vector) {
+    void from(size_t rows, size_t cols, const double* data, bool is_vector) {
         if (data == _data) {
             if (rows != _rows || cols != _cols) {
                 throw std::runtime_error("setting matrix data to same pointer but different size");
             }
             _is_vector = is_vector;
             return;
         }
```

### Comparing `structstore-0.1.2/include/structstore/stst_field.hpp` & `structstore-0.1.3/include/structstore/stst_field.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/include/structstore/stst_hashstring.hpp` & `structstore-0.1.3/include/structstore/stst_hashstring.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/include/structstore/stst_lock.hpp` & `structstore-0.1.3/include/structstore/stst_lock.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/include/structstore/stst_serialization.hpp` & `structstore-0.1.3/include/structstore/stst_serialization.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/include/structstore/stst_shared.hpp` & `structstore-0.1.3/include/structstore/stst_shared.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/include/structstore/stst_structstore.hpp` & `structstore-0.1.3/include/structstore/stst_structstore.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/pyproject.toml` & `structstore-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/src/main.bak.cpp` & `structstore-0.1.3/src/main.bak.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/src/main.cpp` & `structstore-0.1.3/src/main.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/src/structstore.cpp` & `structstore-0.1.3/src/structstore.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/src/structstore_bindings.cpp` & `structstore-0.1.3/src/structstore_bindings.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -90,28 +90,17 @@
         access.get<int>() = nb::cast<int>(value);
     } else if (nb::isinstance<nb::float_>(value)) {
         access.set_type<double>();
         access.get<double>() = nb::cast<double>(value);
     } else if (nb::isinstance<nb::str>(value)) {
         access.set_type<structstore::string>();
         access.get<structstore::string>() = nb::cast<std::string>(value);
-    } else if (nb::isinstance<nb::list>(value)
-               || nb::isinstance<nb::tuple>(value)
-               || nb::isinstance<List>(value)) {
-        access.set_type<List>();
-        List& list = access.get<List>();
-        list.clear();
-        int i = 0;
-        for (const auto& val: nb::cast<nb::list>(value)) {
-            from_object(list.push_back(), val, std::to_string(i));
-            ++i;
-        }
     } else if (nb::ndarray_check(value)) {
         access.set_type<Matrix>();
-        auto array = nb::cast<nb::ndarray<nb::numpy, double>>(value);
+        auto array = nb::cast<nb::ndarray<const double>>(value);
         size_t rows, cols;
         bool is_vector = false;
         if (array.ndim() == 1) {
             rows = array.shape(0);
             cols = 1;
             is_vector = true;
         } else if (array.ndim() == 2) {
@@ -128,15 +117,15 @@
         store.clear();
         for (const auto& [key, val]: dict) {
             std::string key_str = nb::cast<std::string>(key);
             from_object(store[key_str.c_str()], dict[key], key_str);
         }
     } else if (nb::hasattr(value, "__slots__")) {
         access.set_type<StructStore>();
-        auto slots = nb::list(value.attr("__slots__"));
+        auto slots = nb::iterable(value.attr("__slots__"));
         StructStore& store = access.get<StructStore>();
         store.clear();
         for (const auto& key: slots) {
             std::string key_str = nb::cast<std::string>(key);
             from_object(store[key_str.c_str()], nb::getattr(value, key), key_str);
         }
     } else if (nb::isinstance<nb::dict>(value)) {
@@ -153,14 +142,23 @@
                 throw nb::type_error(msg.str().c_str());
             }
             std::string key_str = nb::cast<std::string>(key);
             from_object(store[key_str.c_str()], dict[key], key_str);
         }
     } else if (value.is_none()) {
         access.clear();
+    } else if (nb::isinstance<nb::iterable>(value)) {
+        access.set_type<List>();
+        List& list = access.get<List>();
+        list.clear();
+        int i = 0;
+        for (const auto& val: nb::cast<nb::iterable>(value)) {
+            from_object(list.push_back(), val, std::to_string(i));
+            ++i;
+        }
     } else {
         std::ostringstream msg;
         msg << "field '" << field_name << "' has unsupported type '" << nb::cast<std::string>(nb::str(value.type()))
             << "'";
         throw nb::type_error(msg.str().c_str());
     }
 }
@@ -231,18 +229,18 @@
         return to_object<false>(*field);
     };
     auto set_field = [](T& t, const std::string& name, const nb::object& value) {
         StructStore& store = static_cast<StructStore&>(t);
         auto lock = store.write_lock();
         from_object(store[name.c_str()], value, name);
     };
-    cls.def("__getattr__", get_field, nb::rv_policy::reference_internal);
-    cls.def("__setattr__", set_field);
-    cls.def("__getitem__", get_field, nb::rv_policy::reference_internal);
-    cls.def("__setitem__", set_field);
+    cls.def("__getattr__", get_field, nb::arg("name"), nb::rv_policy::reference_internal);
+    cls.def("__setattr__", set_field, nb::arg("name"), nb::arg("value").none());
+    cls.def("__getitem__", get_field, nb::arg("name"), nb::rv_policy::reference_internal);
+    cls.def("__setitem__", set_field, nb::arg("name"), nb::arg("value").none());
     cls.def("lock", [](T& t) {
         StructStore& store = static_cast<StructStore&>(t);
         store.get_mutex().lock();
         return SpinLockContextManager(&store.get_mutex());
     }, nb::rv_policy::move);
     cls.def("to_yaml", [](T& t) {
         StructStore& store = static_cast<StructStore&>(t);
@@ -369,47 +367,47 @@
         auto lock = list.read_lock();
         return list.size();
     });
     list.def("insert", [](List& list, size_t index, nb::handle& value) {
         auto lock = list.write_lock();
         FieldAccess access = list.insert(index);
         from_object(access, value, std::to_string(index));
-    });
-    list.def("extend", [](List& list, nb::handle& value) {
+    }, nb::arg("index"), nb::arg("value").none());
+    list.def("extend", [](List& list, nb::iterable& value) {
         auto lock = list.write_lock();
-        for (const auto& val: nb::cast<nb::list>(value)) {
+        for (const auto& val: value) {
             std::string field_name = std::to_string(list.size());
             from_object(list.push_back(), val, field_name);
         }
     });
     list.def("append", [](List& list, nb::handle& value) {
         auto lock = list.write_lock();
         from_object(list.push_back(), value, std::to_string(list.size() - 1));
-    });
+    }, nb::arg("value").none());
     list.def("pop", [](List& list, size_t index) {
         auto lock = list.write_lock();
         const auto& res = to_object<true>(list[index].get_field());
         list.erase(index);
         return res;
     });
-    list.def("__add__", [](List& list, nb::handle& value) {
+    list.def("__add__", [](List& list, nb::list& value) {
         auto lock = list.read_lock();
-        return to_list<false>(list) + nb::cast<nb::list>(value);
+        return to_list<false>(list) + value;
     });
-    list.def("__iadd__", [](List& list, nb::handle& value) {
+    list.def("__iadd__", [](List& list, nb::list& value) {
         auto lock = list.write_lock();
-        for (const auto& val: nb::cast<nb::list>(value)) {
+        for (const auto& val: value) {
             from_object(list.push_back(), val, std::to_string(list.size() - 1));
         }
         return to_list<false>(list);
     });
     list.def("__setitem__", [](List& list, size_t index, nb::handle& value) {
         auto lock = list.write_lock();
         from_object(list[index], value, std::to_string(index));
-    });
+    }, nb::arg("index"), nb::arg("value").none());
     list.def("__getitem__", [](List& list, size_t index) {
         auto lock = list.read_lock();
         return to_object<false>(list[index].get_field());
     });
     list.def("__delitem__", [](List& list, size_t index) {
         auto lock = list.write_lock();
         list.erase(index);
```

### Comparing `structstore-0.1.2/src/structstore_containers.cpp` & `structstore-0.1.3/src/structstore_containers.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/src/structstore_serialization.cpp` & `structstore-0.1.3/src/structstore_serialization.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/src/structstore_shared.cpp` & `structstore-0.1.3/src/structstore_shared.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.2/PKG-INFO` & `structstore-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structstore
-Version: 0.1.2
+Version: 0.1.3
 Summary: Structured object storage, dynamically typed, to be shared between processes
 Author-email: Max Mertens <max.mail@dameweb.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: nanobind
 Project-URL: Homepage, https://github.com/mertemba/structstore
```

