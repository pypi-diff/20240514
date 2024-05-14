# Comparing `tmp/structstore-0.1.1.tar.gz` & `tmp/structstore-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structstore-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "structstore-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `structstore-0.1.1.tar` & `structstore-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     4600 2024-05-13 21:47:23.384277 structstore-0.1.1/CMakeLists.txt
--rw-r--r--   0        0        0     1489 2022-11-06 13:29:39.097613 structstore-0.1.1/LICENSE
--rw-r--r--   0        0        0     3867 2024-05-13 11:45:15.567967 structstore-0.1.1/README.md
--rw-r--r--   0        0        0      738 2024-05-13 16:01:09.724654 structstore-0.1.1/cmake/NanobindStubgen.cmake
--rw-r--r--   0        0        0      462 2024-05-13 21:53:42.800696 structstore-0.1.1/cmake/StructStoreConfig.cmake.in
--rw-r--r--   0        0        0      378 2024-05-13 21:20:28.538842 structstore-0.1.1/cmake/StructStoreConfigVersion.cmake.in
--rw-r--r--   0        0        0      385 2024-05-13 21:43:45.044481 structstore-0.1.1/include/structstore/structstore.hpp
--rw-r--r--   0        0        0    13883 2024-05-13 21:43:45.034481 structstore-0.1.1/include/structstore/stst_alloc.hpp
--rw-r--r--   0        0        0     4772 2024-05-13 21:43:45.004481 structstore-0.1.1/include/structstore/stst_containers.hpp
--rw-r--r--   0        0        0     4721 2024-05-13 21:43:45.094481 structstore-0.1.1/include/structstore/stst_field.hpp
--rw-r--r--   0        0        0     1178 2024-05-13 21:07:08.207963 structstore-0.1.1/include/structstore/stst_hashstring.hpp
--rw-r--r--   0        0        0     1578 2024-05-13 21:07:08.201296 structstore-0.1.1/include/structstore/stst_lock.hpp
--rw-r--r--   0        0        0     1255 2024-05-13 21:43:45.071147 structstore-0.1.1/include/structstore/stst_serialization.hpp
--rw-r--r--   0        0        0     4230 2024-05-13 21:43:45.084481 structstore-0.1.1/include/structstore/stst_shared.hpp
--rw-r--r--   0        0        0     5402 2024-05-13 21:43:45.104481 structstore-0.1.1/include/structstore/stst_structstore.hpp
--rw-r--r--   0        0        0     1422 2024-05-13 21:58:00.494559 structstore-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1250 2022-11-18 12:53:02.673000 structstore-0.1.1/src/main.bak.cpp
--rw-r--r--   0        0        0     1355 2022-11-20 10:32:04.499910 structstore-0.1.1/src/main.cpp
--rw-r--r--   0        0        0     1024 2024-05-13 21:43:45.054481 structstore-0.1.1/src/structstore.cpp
--rw-r--r--   0        0        0      169 2024-05-13 21:36:44.288448 structstore-0.1.1/src/structstore/__init__.py
--rw-r--r--   0        0        0    16935 2024-05-13 21:45:04.027734 structstore-0.1.1/src/structstore_bindings.cpp
--rw-r--r--   0        0        0      975 2024-05-13 21:43:44.997814 structstore-0.1.1/src/structstore_containers.cpp
--rw-r--r--   0        0        0      336 2024-05-13 21:43:45.064481 structstore-0.1.1/src/structstore_field.cpp
--rw-r--r--   0        0        0     2644 2024-05-13 21:43:45.017814 structstore-0.1.1/src/structstore_serialization.cpp
--rw-r--r--   0        0        0     8919 2024-05-13 21:43:45.027814 structstore-0.1.1/src/structstore_shared.cpp
--rw-r--r--   0        0        0     4208 1970-01-01 00:00:00.000000 structstore-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4656 2024-05-14 08:45:24.019774 structstore-0.1.2/CMakeLists.txt
+-rw-r--r--   0        0        0     1489 2022-11-06 13:29:39.097613 structstore-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3879 2024-05-13 22:03:39.240898 structstore-0.1.2/README.md
+-rw-r--r--   0        0        0      709 2024-05-14 08:27:19.167743 structstore-0.1.2/cmake/NanobindStubgen.cmake
+-rw-r--r--   0        0        0      462 2024-05-13 21:53:42.800696 structstore-0.1.2/cmake/StructStoreConfig.cmake.in
+-rw-r--r--   0        0        0      378 2024-05-13 21:20:28.538842 structstore-0.1.2/cmake/StructStoreConfigVersion.cmake.in
+-rw-r--r--   0        0        0      385 2024-05-13 21:43:45.044481 structstore-0.1.2/include/structstore/structstore.hpp
+-rw-r--r--   0        0        0    13883 2024-05-13 21:43:45.034481 structstore-0.1.2/include/structstore/stst_alloc.hpp
+-rw-r--r--   0        0        0     4772 2024-05-13 21:43:45.004481 structstore-0.1.2/include/structstore/stst_containers.hpp
+-rw-r--r--   0        0        0     4721 2024-05-13 21:43:45.094481 structstore-0.1.2/include/structstore/stst_field.hpp
+-rw-r--r--   0        0        0     1178 2024-05-13 21:07:08.207963 structstore-0.1.2/include/structstore/stst_hashstring.hpp
+-rw-r--r--   0        0        0     1578 2024-05-13 21:07:08.201296 structstore-0.1.2/include/structstore/stst_lock.hpp
+-rw-r--r--   0        0        0     1255 2024-05-13 21:43:45.071147 structstore-0.1.2/include/structstore/stst_serialization.hpp
+-rw-r--r--   0        0        0     4230 2024-05-13 21:43:45.084481 structstore-0.1.2/include/structstore/stst_shared.hpp
+-rw-r--r--   0        0        0     5402 2024-05-13 21:43:45.104481 structstore-0.1.2/include/structstore/stst_structstore.hpp
+-rw-r--r--   0        0        0     1422 2024-05-14 07:45:17.149944 structstore-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1250 2022-11-18 12:53:02.673000 structstore-0.1.2/src/main.bak.cpp
+-rw-r--r--   0        0        0     1355 2022-11-20 10:32:04.499910 structstore-0.1.2/src/main.cpp
+-rw-r--r--   0        0        0     1024 2024-05-13 21:43:45.054481 structstore-0.1.2/src/structstore.cpp
+-rw-r--r--   0        0        0      246 2024-05-14 08:45:37.725425 structstore-0.1.2/src/structstore/__init__.py
+-rw-r--r--   0        0        0    16900 2024-05-14 08:43:18.453931 structstore-0.1.2/src/structstore_bindings.cpp
+-rw-r--r--   0        0        0      975 2024-05-13 21:43:44.997814 structstore-0.1.2/src/structstore_containers.cpp
+-rw-r--r--   0        0        0      336 2024-05-13 21:43:45.064481 structstore-0.1.2/src/structstore_field.cpp
+-rw-r--r--   0        0        0     2644 2024-05-13 21:43:45.017814 structstore-0.1.2/src/structstore_serialization.cpp
+-rw-r--r--   0        0        0     8919 2024-05-13 21:43:45.027814 structstore-0.1.2/src/structstore_shared.cpp
+-rw-r--r--   0        0        0     4220 1970-01-01 00:00:00.000000 structstore-0.1.2/PKG-INFO
```

### Comparing `structstore-0.1.1/CMakeLists.txt` & `structstore-0.1.2/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cmake_minimum_required(VERSION 3.10)
-project(structstore VERSION 0.1.1)
+project(structstore VERSION 0.1.2)
 
 set(PY_VERSION_SUFFIX "")
 set(PY_FULL_VERSION ${PROJECT_VERSION}${PY_VERSION_SUFFIX})
 
 # make sure that the Python and CMake versions match
 if (DEFINED PY_BUILD_CMAKE_PACKAGE_VERSION)
     if (NOT "${PY_BUILD_CMAKE_PACKAGE_VERSION}" MATCHES "^${PY_FULL_VERSION}$")
@@ -74,45 +74,52 @@
     target_link_libraries(${TARGET} PRIVATE
             ${YAML_CPP_LIBRARIES}
             rt)
 endforeach ()
 
 # install
 
-if (DEFINED PY_BUILD_CMAKE_PACKAGE_VERSION)
-    install(TARGETS structstore_lib
-            EXPORT StructStoreTargets
-            COMPONENT python_modules
-            DESTINATION ${PY_BUILD_CMAKE_MODULE_NAME})
-    install(TARGETS structstore_bindings
-            COMPONENT python_modules
-            DESTINATION ${PY_BUILD_CMAKE_MODULE_NAME})
-    install(DIRECTORY ${PROJECT_SOURCE_DIR}/include
-            COMPONENT python_modules
-            DESTINATION ${PY_BUILD_CMAKE_MODULE_NAME})
-
-    include(cmake/NanobindStubgen.cmake)
-    nanobind_stubgen(structstore_bindings)
-    nanobind_stubgen_install(structstore_bindings ${PY_BUILD_CMAKE_MODULE_NAME})
-
-    export(TARGETS structstore_lib
-            FILE "${PROJECT_BINARY_DIR}/MyLibTargets.cmake")
-    export(PACKAGE StructStore)
-    configure_file(${PROJECT_SOURCE_DIR}/cmake/StructStoreConfig.cmake.in
-            "${PROJECT_BINARY_DIR}/StructStoreConfig.cmake" @ONLY)
-    configure_file(${PROJECT_SOURCE_DIR}/cmake/StructStoreConfigVersion.cmake.in
-            "${PROJECT_BINARY_DIR}/StructStoreConfigVersion.cmake" @ONLY)
-    install(FILES
-            "${PROJECT_BINARY_DIR}/StructStoreConfig.cmake"
-            "${PROJECT_BINARY_DIR}/StructStoreConfigVersion.cmake"
-            COMPONENT python_modules
-            DESTINATION ${PY_BUILD_CMAKE_MODULE_NAME}/cmake)
-    install(EXPORT StructStoreTargets
-            COMPONENT python_modules
-            DESTINATION ${PY_BUILD_CMAKE_MODULE_NAME}/cmake)
+if (DEFINED PY_BUILD_CMAKE_MODULE_NAME)
+    set(STRUCTSTORE_INSTALL_DIR ${PY_BUILD_CMAKE_MODULE_NAME})
 else ()
     set(CMAKE_INSTALL_PREFIX ${PROJECT_SOURCE_DIR})
-    install(TARGETS structstore_lib LIBRARY DESTINATION structstore)
-    install(TARGETS structstore_bindings LIBRARY DESTINATION structstore)
+    set(STRUCTSTORE_INSTALL_DIR install)
+endif ()
+
+install(TARGETS structstore_lib
+        EXPORT StructStoreTargets
+        COMPONENT python_modules
+        DESTINATION ${STRUCTSTORE_INSTALL_DIR})
+install(TARGETS structstore_bindings
+        COMPONENT python_modules
+        DESTINATION ${STRUCTSTORE_INSTALL_DIR})
+install(DIRECTORY ${PROJECT_SOURCE_DIR}/include
+        COMPONENT python_modules
+        DESTINATION ${STRUCTSTORE_INSTALL_DIR})
+
+include(cmake/NanobindStubgen.cmake)
+nanobind_stubgen(structstore_bindings)
+nanobind_stubgen_install(structstore_bindings ${STRUCTSTORE_INSTALL_DIR})
+
+# inspired from https://stackoverflow.com/a/49857699
+export(TARGETS structstore_lib
+        FILE "${PROJECT_BINARY_DIR}/StructStoreTargets.cmake")
+export(PACKAGE StructStore)
+configure_file(${PROJECT_SOURCE_DIR}/cmake/StructStoreConfig.cmake.in
+        "${PROJECT_BINARY_DIR}/StructStoreConfig.cmake" @ONLY)
+configure_file(${PROJECT_SOURCE_DIR}/cmake/StructStoreConfigVersion.cmake.in
+        "${PROJECT_BINARY_DIR}/StructStoreConfigVersion.cmake" @ONLY)
+install(FILES
+        "${PROJECT_BINARY_DIR}/StructStoreConfig.cmake"
+        "${PROJECT_BINARY_DIR}/StructStoreConfigVersion.cmake"
+        COMPONENT python_modules
+        DESTINATION ${STRUCTSTORE_INSTALL_DIR}/cmake)
+install(EXPORT StructStoreTargets
+        COMPONENT python_modules
+        DESTINATION ${STRUCTSTORE_INSTALL_DIR}/cmake)
+
+if (NOT DEFINED PY_BUILD_CMAKE_PACKAGE_VERSION)
+    set(STRUCTSTORE_INCLUDE_DIRS ${PROJECT_SOURCE_DIR}/include)
+    set(STRUCTSTORE_LIBRARIES structstore_lib)
 
     add_subdirectory(examples)
 endif ()
```

### Comparing `structstore-0.1.1/LICENSE` & `structstore-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/README.md` & `structstore-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 C++17 library and Python bindings.
 
 ## Usage examples
 
 ### C++
 
 ```c++
-#include <structstore.hpp>
+#include <structstore/structstore.hpp>
 namespace stst = structstore;
 
 int main() {
     stst::StructStore store;
     int& num = store["num"];
     num = 5;
     stst::List& list = store["list"];
```

### Comparing `structstore-0.1.1/cmake/NanobindStubgen.cmake` & `structstore-0.1.2/cmake/NanobindStubgen.cmake`

 * *Files 10% similar despite different names*

```diff
@@ -9,11 +9,10 @@
 
 endfunction()
 
 function(nanobind_stubgen_install target destination)
     install(FILES
             $<TARGET_FILE_DIR:${target}>/$<TARGET_FILE_BASE_NAME:${target}>.pyi
             RENAME __init__.pyi
-            EXCLUDE_FROM_ALL
             COMPONENT python_modules
             DESTINATION ${destination}/$<TARGET_FILE_BASE_NAME:${target}>)
 endfunction()
```

### Comparing `structstore-0.1.1/include/structstore/stst_alloc.hpp` & `structstore-0.1.2/include/structstore/stst_alloc.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/include/structstore/stst_containers.hpp` & `structstore-0.1.2/include/structstore/stst_containers.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/include/structstore/stst_field.hpp` & `structstore-0.1.2/include/structstore/stst_field.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/include/structstore/stst_hashstring.hpp` & `structstore-0.1.2/include/structstore/stst_hashstring.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/include/structstore/stst_lock.hpp` & `structstore-0.1.2/include/structstore/stst_lock.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/include/structstore/stst_serialization.hpp` & `structstore-0.1.2/include/structstore/stst_serialization.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/include/structstore/stst_shared.hpp` & `structstore-0.1.2/include/structstore/stst_shared.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/include/structstore/stst_structstore.hpp` & `structstore-0.1.2/include/structstore/stst_structstore.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/pyproject.toml` & `structstore-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/src/main.bak.cpp` & `structstore-0.1.2/src/main.bak.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/src/main.cpp` & `structstore-0.1.2/src/main.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/src/structstore.cpp` & `structstore-0.1.2/src/structstore.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/src/structstore_bindings.cpp` & `structstore-0.1.2/src/structstore_bindings.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         List& list = access.get<List>();
         list.clear();
         int i = 0;
         for (const auto& val: nb::cast<nb::list>(value)) {
             from_object(list.push_back(), val, std::to_string(i));
             ++i;
         }
-    } else if (nb::isinstance<nb::ndarray<nb::numpy, double>>(value)) {
+    } else if (nb::ndarray_check(value)) {
         access.set_type<Matrix>();
         auto array = nb::cast<nb::ndarray<nb::numpy, double>>(value);
         size_t rows, cols;
         bool is_vector = false;
         if (array.ndim() == 1) {
             rows = array.shape(0);
             cols = 1;
@@ -181,42 +181,37 @@
         nb::setattr(obj, name.str, to_object<recursive>(store.fields.at(name)));
     }
     return obj;
 }
 
 class SpinLockContextManager {
 
-    SpinMutex* mutex;
-    bool locked;
+    SpinMutex* mutex = nullptr;
 
 public:
 
-    explicit SpinLockContextManager (SpinMutex* mutex)
-        : mutex{mutex}, locked{true} { }
+    explicit SpinLockContextManager(SpinMutex* mutex) : mutex{mutex} {}
 
-    SpinLockContextManager(SpinLockContextManager&& other) noexcept
-            : mutex{other.mutex}, locked{other.locked} {
-        other.locked = false;
+    SpinLockContextManager(SpinLockContextManager&& other) noexcept {
+        std::swap(mutex, other.mutex);
     }
 
     SpinLockContextManager(const SpinLockContextManager&) = delete;
     SpinLockContextManager& operator=(SpinLockContextManager&& other) = delete;
     SpinLockContextManager& operator=(const SpinLockContextManager&) = delete;
 
-    void exit(nb::handle&, nb::handle&, nb::handle&) {
-        if (locked) {
-            locked = false;
+    void unlock() {
+        if (mutex) {
             mutex->unlock();
+            mutex = nullptr;
         }
     }
 
-    ~SpinLockContextManager () {
-        if (locked) {
-            mutex->unlock();
-        }
+    ~SpinLockContextManager() {
+        unlock();
     }
 };
 
 template<typename T>
 void register_structstore_methods(nb::class_<T>& cls) {
     cls.def_prop_ro("__slots__", [](T& t) {
         StructStore& store = static_cast<StructStore&>(t);
@@ -299,15 +294,17 @@
 NB_MODULE(MODULE_NAME, m) {
     m.attr("__version__") = VERSION_INFO;
 
     SimpleNamespace = nb::module_::import_("types").attr("SimpleNamespace");
 
     nb::class_<SpinLockContextManager>(m, "SpinLockContextManager")
             .def("__enter__", [](SpinLockContextManager&) {})
-        .def("__exit__", &SpinLockContextManager::exit);
+            .def("__exit__", [](SpinLockContextManager& con_man, nb::handle, nb::handle, nb::handle) {
+                con_man.unlock();
+            }, nb::arg().none(), nb::arg().none(), nb::arg().none());
 
     nb::class_<StructStore> cls = nb::class_<StructStore>{m, "StructStore"};
     cls.def(nb::init<>());
     register_structstore_methods(cls);
 
     nb::enum_<CleanupMode>(m, "CleanupMode")
             .value("NEVER", NEVER)
```

### Comparing `structstore-0.1.1/src/structstore_containers.cpp` & `structstore-0.1.2/src/structstore_containers.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/src/structstore_serialization.cpp` & `structstore-0.1.2/src/structstore_serialization.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/src/structstore_shared.cpp` & `structstore-0.1.2/src/structstore_shared.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.1/PKG-INFO` & `structstore-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structstore
-Version: 0.1.1
+Version: 0.1.2
 Summary: Structured object storage, dynamically typed, to be shared between processes
 Author-email: Max Mertens <max.mail@dameweb.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: nanobind
 Project-URL: Homepage, https://github.com/mertemba/structstore
 
@@ -14,15 +14,15 @@
 C++17 library and Python bindings.
 
 ## Usage examples
 
 ### C++
 
 ```c++
-#include <structstore.hpp>
+#include <structstore/structstore.hpp>
 namespace stst = structstore;
 
 int main() {
     stst::StructStore store;
     int& num = store["num"];
     num = 5;
     stst::List& list = store["list"];
```

