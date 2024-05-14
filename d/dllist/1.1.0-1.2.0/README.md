# Comparing `tmp/dllist-1.1.0.tar.gz` & `tmp/dllist-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dllist-1.1.0.tar", last modified: Mon Oct 16 20:10:36 2023, max compression
+gzip compressed data, was "dllist-1.2.0.tar", last modified: Tue May 14 20:25:18 2024, max compression
```

## Comparing `dllist-1.1.0.tar` & `dllist-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 brian     (1001) brian     (1001)        0 2023-10-16 20:10:36.546620 dllist-1.1.0/
--rw-rw-r--   0 brian     (1001) brian     (1001)     1466 2023-10-12 20:23:12.000000 dllist-1.1.0/LICENSE
--rw-r--r--   0 brian     (1001) brian     (1001)     1533 2023-10-16 20:10:36.546620 dllist-1.1.0/PKG-INFO
--rw-rw-r--   0 brian     (1001) brian     (1001)      809 2023-10-16 16:57:43.000000 dllist-1.1.0/README.md
-drwxrwxr-x   0 brian     (1001) brian     (1001)        0 2023-10-16 20:10:36.546620 dllist-1.1.0/dllist/
--rw-rw-r--   0 brian     (1001) brian     (1001)     1142 2023-10-16 20:07:05.000000 dllist-1.1.0/dllist/__init__.py
--rw-rw-r--   0 brian     (1001) brian     (1001)     1124 2023-10-16 19:55:25.000000 dllist-1.1.0/dllist/linux.py
--rw-rw-r--   0 brian     (1001) brian     (1001)      771 2023-10-16 19:59:50.000000 dllist-1.1.0/dllist/macos.py
--rw-rw-r--   0 brian     (1001) brian     (1001)        0 2023-10-13 14:15:50.000000 dllist-1.1.0/dllist/py.typed
--rw-rw-r--   0 brian     (1001) brian     (1001)     3020 2023-10-16 20:03:26.000000 dllist-1.1.0/dllist/windows.py
-drwxrwxr-x   0 brian     (1001) brian     (1001)        0 2023-10-16 20:10:36.546620 dllist-1.1.0/dllist.egg-info/
--rw-r--r--   0 brian     (1001) brian     (1001)     1533 2023-10-16 20:10:36.000000 dllist-1.1.0/dllist.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1001) brian     (1001)      344 2023-10-16 20:10:36.000000 dllist-1.1.0/dllist.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1001) brian     (1001)        1 2023-10-16 20:10:36.000000 dllist-1.1.0/dllist.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1001) brian     (1001)       26 2023-10-16 20:10:36.000000 dllist-1.1.0/dllist.egg-info/requires.txt
--rw-rw-r--   0 brian     (1001) brian     (1001)        7 2023-10-16 20:10:36.000000 dllist-1.1.0/dllist.egg-info/top_level.txt
--rw-rw-r--   0 brian     (1001) brian     (1001)     1000 2023-10-16 20:06:58.000000 dllist-1.1.0/pyproject.toml
--rw-rw-r--   0 brian     (1001) brian     (1001)       38 2023-10-16 20:10:36.546620 dllist-1.1.0/setup.cfg
-drwxrwxr-x   0 brian     (1001) brian     (1001)        0 2023-10-16 20:10:36.546620 dllist-1.1.0/test/
--rw-rw-r--   0 brian     (1001) brian     (1001)      619 2023-10-16 19:51:35.000000 dllist-1.1.0/test/test_linux.py
--rw-rw-r--   0 brian     (1001) brian     (1001)      630 2023-10-16 19:51:35.000000 dllist-1.1.0/test/test_macos.py
--rw-rw-r--   0 brian     (1001) brian     (1001)      400 2023-10-16 19:51:42.000000 dllist-1.1.0/test/test_other.py
--rw-rw-r--   0 brian     (1001) brian     (1001)      643 2023-10-16 19:51:35.000000 dllist-1.1.0/test/test_windows.py
+drwxrwxr-x   0 brian     (1001) brian     (1001)        0 2024-05-14 20:25:18.327811 dllist-1.2.0/
+-rw-rw-r--   0 brian     (1001) brian     (1001)     1466 2023-10-12 20:23:12.000000 dllist-1.2.0/LICENSE
+-rw-r--r--   0 brian     (1001) brian     (1001)     1609 2024-05-14 20:25:18.327811 dllist-1.2.0/PKG-INFO
+-rw-rw-r--   0 brian     (1001) brian     (1001)      885 2024-05-14 15:08:52.000000 dllist-1.2.0/README.md
+drwxrwxr-x   0 brian     (1001) brian     (1001)        0 2024-05-14 20:25:18.323811 dllist-1.2.0/dllist/
+-rw-rw-r--   0 brian     (1001) brian     (1001)     1343 2024-05-14 15:08:56.000000 dllist-1.2.0/dllist/__init__.py
+-rw-rw-r--   0 brian     (1001) brian     (1001)      771 2023-10-16 19:59:50.000000 dllist-1.2.0/dllist/macos.py
+-rw-rw-r--   0 brian     (1001) brian     (1001)        0 2023-10-13 14:15:50.000000 dllist-1.2.0/dllist/py.typed
+-rw-rw-r--   0 brian     (1001) brian     (1001)     1373 2024-05-14 15:08:52.000000 dllist-1.2.0/dllist/unix_like.py
+-rw-rw-r--   0 brian     (1001) brian     (1001)     2291 2024-05-14 20:21:37.000000 dllist-1.2.0/dllist/windows.py
+drwxrwxr-x   0 brian     (1001) brian     (1001)        0 2024-05-14 20:25:18.323811 dllist-1.2.0/dllist.egg-info/
+-rw-r--r--   0 brian     (1001) brian     (1001)     1609 2024-05-14 20:25:18.000000 dllist-1.2.0/dllist.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1001) brian     (1001)      348 2024-05-14 20:25:18.000000 dllist-1.2.0/dllist.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1001) brian     (1001)        1 2024-05-14 20:25:18.000000 dllist-1.2.0/dllist.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1001) brian     (1001)       26 2024-05-14 20:25:18.000000 dllist-1.2.0/dllist.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1001) brian     (1001)        7 2024-05-14 20:25:18.000000 dllist-1.2.0/dllist.egg-info/top_level.txt
+-rw-rw-r--   0 brian     (1001) brian     (1001)     1000 2023-10-16 20:06:58.000000 dllist-1.2.0/pyproject.toml
+-rw-rw-r--   0 brian     (1001) brian     (1001)       38 2024-05-14 20:25:18.327811 dllist-1.2.0/setup.cfg
+drwxrwxr-x   0 brian     (1001) brian     (1001)        0 2024-05-14 20:25:18.323811 dllist-1.2.0/test/
+-rw-rw-r--   0 brian     (1001) brian     (1001)      681 2024-05-14 15:08:52.000000 dllist-1.2.0/test/test_linux.py
+-rw-rw-r--   0 brian     (1001) brian     (1001)      630 2023-10-16 19:51:35.000000 dllist-1.2.0/test/test_macos.py
+-rw-rw-r--   0 brian     (1001) brian     (1001)      436 2024-05-14 15:08:52.000000 dllist-1.2.0/test/test_other.py
+-rw-rw-r--   0 brian     (1001) brian     (1001)      643 2023-10-16 19:51:35.000000 dllist-1.2.0/test/test_windows.py
```

### Comparing `dllist-1.1.0/LICENSE` & `dllist-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dllist-1.1.0/PKG-INFO` & `dllist-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dllist
-Version: 1.1.0
+Version: 1.2.0
 Summary: List the shared libraries loaded by the current process.
 Author-email: Brian Ward <bward@flatironinstitute.org>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/wardbrian/dllist
 Project-URL: Bug Tracker, https://github.com/wardbrian/dllist/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,19 @@
 Requires-Dist: pytest-cov; extra == "test"
 
 # dllist
 
 A very small Python library to list the DLLs loaded by the current process.
 This is equivalent to the [`dllist`](https://docs.julialang.org/en/v1/stdlib/Libdl/#Base.Libc.Libdl.dllist) function in Julia.
 
-*Note*: This library is intended to work on macOS, Linux, and Windows. Other platforms will return an empty list and raise a warning.
+*Note*: This library is tested on macOS, Linux, and Windows.
+
+Some platforms which provide the same API as Linux (e.g. FreeBSD) may also work.
+
+Any other platform will return an empty list and raise a warning.
 
 ## Installation
 
 `dllist` is [available on PyPI](https://pypi.org/project/dllist/):
 
 ```
 pip install dllist
```

### Comparing `dllist-1.1.0/README.md` & `dllist-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # dllist
 
 A very small Python library to list the DLLs loaded by the current process.
 This is equivalent to the [`dllist`](https://docs.julialang.org/en/v1/stdlib/Libdl/#Base.Libc.Libdl.dllist) function in Julia.
 
-*Note*: This library is intended to work on macOS, Linux, and Windows. Other platforms will return an empty list and raise a warning.
+*Note*: This library is tested on macOS, Linux, and Windows.
+
+Some platforms which provide the same API as Linux (e.g. FreeBSD) may also work.
+
+Any other platform will return an empty list and raise a warning.
 
 ## Installation
 
 `dllist` is [available on PyPI](https://pypi.org/project/dllist/):
 
 ```
 pip install dllist
```

### Comparing `dllist-1.1.0/dllist/linux.py` & `dllist-1.2.0/dllist/unix_like.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import ctypes
 import warnings
 from ctypes.util import find_library
 from typing import List
 
+# this uses functions common to Linux and a few other Unix-like systems
 # https://man7.org/linux/man-pages/man3/dl_iterate_phdr.3.html
+# https://man.freebsd.org/cgi/man.cgi?query=dl_iterate_phdr
+# https://man.openbsd.org/dl_iterate_phdr
+# https://docs.oracle.com/cd/E88353_01/html/E37843/dl-iterate-phdr-3c.html
 
 
 class dl_phdr_info(ctypes.Structure):
     _fields_ = [
         ("dlpi_addr", ctypes.c_void_p),
         ("dlpi_name", ctypes.c_char_p),
         ("dlpi_phdr", ctypes.c_void_p),
```

### Comparing `dllist-1.1.0/dllist/macos.py` & `dllist-1.2.0/dllist/macos.py`

 * *Files identical despite different names*

### Comparing `dllist-1.1.0/dllist.egg-info/PKG-INFO` & `dllist-1.2.0/dllist.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dllist
-Version: 1.1.0
+Version: 1.2.0
 Summary: List the shared libraries loaded by the current process.
 Author-email: Brian Ward <bward@flatironinstitute.org>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/wardbrian/dllist
 Project-URL: Bug Tracker, https://github.com/wardbrian/dllist/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,19 @@
 Requires-Dist: pytest-cov; extra == "test"
 
 # dllist
 
 A very small Python library to list the DLLs loaded by the current process.
 This is equivalent to the [`dllist`](https://docs.julialang.org/en/v1/stdlib/Libdl/#Base.Libc.Libdl.dllist) function in Julia.
 
-*Note*: This library is intended to work on macOS, Linux, and Windows. Other platforms will return an empty list and raise a warning.
+*Note*: This library is tested on macOS, Linux, and Windows.
+
+Some platforms which provide the same API as Linux (e.g. FreeBSD) may also work.
+
+Any other platform will return an empty list and raise a warning.
 
 ## Installation
 
 `dllist` is [available on PyPI](https://pypi.org/project/dllist/):
 
 ```
 pip install dllist
```

### Comparing `dllist-1.1.0/pyproject.toml` & `dllist-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dllist-1.1.0/test/test_linux.py` & `dllist-1.2.0/test/test_windows.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import platform
 
 import pytest
 
-if not platform.system().startswith("Linux"):
-    pytest.skip(reason="Linux only", allow_module_level=True)
+if not platform.system().startswith("Windows"):
+    pytest.skip(reason="Windows only", allow_module_level=True)
 
 
 from test import print_list
 
 from dllist import dllist
 
 
 def test_dllist_basic() -> None:
     dlls = dllist()
     print_list(dlls)
     assert len(dlls) > 0
-    assert any("libc.so" in dll for dll in dlls)
+    assert any("kernel32.dll" in dll.lower() for dll in dlls)
 
 
 def test_euler() -> None:
     dlls = dllist()
     num_dlls = len(dlls)
 
     euler = pytest.importorskip("euler")
 
     dlls2 = dllist()
     print_list(dlls2)
 
     assert len(dlls2) > num_dlls
-    assert any("/dllist/test/test_éxt/euler.cpython" in dll for dll in dlls2)
+    assert any("\\dllist\\test\\test_éxt\\euler.cp" in dll.lower() for dll in dlls2)
```

### Comparing `dllist-1.1.0/test/test_macos.py` & `dllist-1.2.0/test/test_macos.py`

 * *Files identical despite different names*

