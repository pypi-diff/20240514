# Comparing `tmp/pydfuutil-0.0.5.tar.gz` & `tmp/pydfuutil-0.11.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydfuutil-0.0.5.tar", last modified: Mon May  6 14:50:40 2024, max compression
+gzip compressed data, was "pydfuutil-0.11.0b0.tar", last modified: Tue May 14 19:01:35 2024, max compression
```

## Comparing `pydfuutil-0.0.5.tar` & `pydfuutil-0.11.0b0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:50:40.818125 pydfuutil-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-05-06 14:50:40.818125 pydfuutil-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:50:40.814125 pydfuutil-0.0.5/pydfuutil/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35935 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/dfu.py
--rw-r--r--   0 runner    (1001) docker     (127)    19557 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/dfu_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/dfu_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/dfuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/dfuse_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/lmdfu.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/portable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/quirks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pydfuutil/usb_dfu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:50:40.814125 pydfuutil-0.0.5/pydfuutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-05-06 14:50:40.000000 pydfuutil-0.0.5/pydfuutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 14:50:40.000000 pydfuutil-0.0.5/pydfuutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:50:40.000000 pydfuutil-0.0.5/pydfuutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-06 14:50:40.000000 pydfuutil-0.0.5/pydfuutil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 14:50:40.000000 pydfuutil-0.0.5/pydfuutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 14:50:40.000000 pydfuutil-0.0.5/pydfuutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 14:50:40.818125 pydfuutil-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:50:40.814125 pydfuutil-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/tests/test_dfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/tests/test_dfu_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/tests/test_dfu_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    14411 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/tests/test_dfuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/tests/test_dfuse_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/tests/test_lmdfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-06 14:50:24.000000 pydfuutil-0.0.5/tests/test_quirks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:01:35.031600 pydfuutil-0.11.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20542 2024-05-14 19:01:35.031600 pydfuutil-0.11.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:01:35.027600 pydfuutil-0.11.0b0/pydfuutil/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27026 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/dfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/dfu_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/dfu_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13853 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/dfu_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28368 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/dfuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/dfuse_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/lsusb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/portable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11287 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/quirks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pydfuutil/usb_dfu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:01:35.027600 pydfuutil-0.11.0b0/pydfuutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20542 2024-05-14 19:01:35.000000 pydfuutil-0.11.0b0/pydfuutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-14 19:01:35.000000 pydfuutil-0.11.0b0/pydfuutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:01:35.000000 pydfuutil-0.11.0b0/pydfuutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-14 19:01:35.000000 pydfuutil-0.11.0b0/pydfuutil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 19:01:35.000000 pydfuutil-0.11.0b0/pydfuutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 19:01:35.000000 pydfuutil-0.11.0b0/pydfuutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:01:35.031600 pydfuutil-0.11.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:01:35.027600 pydfuutil-0.11.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/tests/test_dfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/tests/test_dfu_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/tests/test_dfu_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/tests/test_dfuse_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-14 19:01:25.000000 pydfuutil-0.11.0b0/tests/test_quirks.py
```

### Comparing `pydfuutil-0.0.5/LICENSE` & `pydfuutil-0.11.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.5/PKG-INFO` & `pydfuutil-0.11.0b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydfuutil
-Version: 0.0.5
+Version: 0.11.0b0
 Summary: PyDfuUtil - Pure python fork of dfu-util wrappers to libusb
 Author-email: o-murphy <thehelixpg@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -185,116 +185,152 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyusb
 Requires-Dist: libusb-package
-Requires-Dist: construct
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Provides-Extra: rich
 Requires-Dist: rich; extra == "rich"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pylint; extra == "test"
 
-# PyDfuUtil - Pure python fork of **[dfu-util](https://github.com/Stefan-Schmidt/dfu-util)** wrappers to **[libusb](https://github.com/libusb/libusb)**
+# PyDfuUtil - Pure python fork of **[dfu-util](https://dfu-util.sourceforge.net/)** wrappers to **[libusb](https://github.com/libusb/libusb)**
 
 [![PyPI Version](https://img.shields.io/pypi/v/pydfuutil?label=PyPI&logo=pypi)](https://pypi.org/project/pydfuutil/)
 
 ## Table of contents
 * **[Introduction](#introduction)**
 * **[Requirements](#requirements-and-platform-support)**
 * **[Installing](#installing)**
+* **[Usage](#installing)**
+  + [**Manual page**](https://dfu-util.sourceforge.net/dfu-util.1.html)
+  + [**dfu-util** (pydfuutil-util)](#pydfuutil)
+  + [**dfu-suffix** (pydfuutil-suffix)](#pydfuutil-suffix)
+  + [**dfu-prefix** (pydfuutil-prefix)](#pydfuutil-prefix)
+  + [**lsusb** (pydfuutil-lsusb)](#pydfuutil-lsusb)
 * **[Todos](#todos)**
 * **[Getting help](#getting-help)**
 * **[About](#about)**
 * **[Footnotes](#footnotes)**
 
 
 ## Introduction
 
 * **PyDFUUtil** provides for easy access to the devices that supports **DFU** interface over host machine's **Universal Serial Bus (USB)**
 system for Python 3.
-* **PyDFUUtil** is an open realisation of original **[dfu-util](https://github.com/Stefan-Schmidt/dfu-util)**
+* **PyDFUUtil** is an open realisation of original **[dfu-util](https://dfu-util.sourceforge.net/)**
 and thin wrapper over **[libusb](https://github.com/libusb/libusb)** _(uses **[PyUsb](https://github.com/pyusb/pyusb)** library as a backend)_.
 
 > [!WARNING]
 > The current status of the project is BETA version.
 > Use it for your own risk
 
+> [!IMPORTANT]
+> Current version implements but not tested with real `dfuse` devices!
+
 > [!TIP]
 > Searching for contributors for testing the library
 
 ## Requirements and platform support
 
 * Since **PyDFUUtil** uses the **[libusb](https://github.com/libusb/libusb)** library it has similar dependencies for using **[libusb](https://github.com/libusb/libusb)**
-* It uses python **[construct](https://github.com/construct/construct)** library for simple unpacking C-structs.
 * **PyDFUUtil** primarily tested on Linux and Windows, 
-but also can work on each platform where **[PyUsb](https://github.com/construct/construct)** and **[construct](https://github.com/construct/construct)** libraries are available, including MacOS
+but also can work on each platform where **[PyUsb](https://github.com/construct/construct)** library are available, including MacOS
 
 
 ## Installing
 
 **PyDFUUtil** is generally installed through pip
 
     # the latest official release
     python -m pip install pydfuutil
 
     # install a specific version (e.g. 0.0.1b1)
     python -m pip install pydfuutil==0.0.1b1
 
 ## Usage
 
-### dfu-util
+### pydfuutil
 ```Bash
 pydfuutil -h 
 # or
 python -m pydfuutil -h
 
 ####### usage:
-usage: pydfuutil [-h] [-V] [-v] [-l] [-e] [-d <deviceID>:<productID>] [-p <bus/port>] [-c <config>] [-i <intf_num>] [-a <alt>] [-t <size>] [-U <file>] [-D <file>] [-R] [-s <address>]
+usage: pydfuutil [-h] [-V] [-v] [-l] [-e] [-E <seconds>]
+                 [-d <vid>:<pid>[,<vid_dfu>:<pid_dfu>]] [-n <dnum>] [-p <bus-port. ... .port>]
+                 [-c <config_nr>] [-i <intf_nr>] [-S <serial_str>[,<serial_str_dfu>]]
+                 [-a <alt>] [-t <size>] [-U <file>] [-Z <bytes>] [-D <file>] [-R] [-w]
+                 [-s <address><:...>]
 
 Python implementation of DFU-Util tools
 
 options:
   -h, --help            show this help message and exit
   -V, --version         Print the version number
   -v, --verbose         Print verbose debug statements
   -l, --list            List the currently attached DFU capable USB devices
   -e, --detach          Detach the currently attached DFU capable USB devices
-  -d <deviceID>:<productID>, --device <deviceID>:<productID>
-                        Specify Vendor/Product ID of DFU device
-  -p <bus/port>, --path <bus/port>
+  -E <seconds>, --detach-delay <seconds>
+                        Time to wait before reopening a device after detach
+  -d <vid>:<pid>[,<vid_dfu>:<pid_dfu>], --device <vid>:<pid>[,<vid_dfu>:<pid_dfu>]
+                        Specify Vendor/Product ID(s) of DFU device
+  -n <dnum>, --devnum <dnum>
+                        Match given device number (devnum from --list)
+  -p <bus-port. ... .port>, --path <bus-port. ... .port>
                         Specify path to DFU device
-  -c <config>, --cfg <config>
+  -c <config_nr>, --cfg <config_nr>
                         Specify the Configuration of DFU device
-  -i <interface>, --intf <interface>
+  -i <intf_nr>, --intf <intf_nr>
                         Specify the DFU Interface number
+  -S <serial_str>[,<serial_str_dfu>], --serial <serial_str>[,<serial_str_dfu>]
+                        Specify Serial String of DFU device
   -a <alt>, --alt <alt>
                         Specify the Altsetting of the DFU Interface
   -t <size>, --transfer-size <size>
                         Specify the number of bytes per USB Transfer
   -U <file>, --upload <file>
                         Read firmware from device into <file>
+  -Z <bytes>, --upload-size <bytes>
+                        Read firmware from device into <file>
   -D <file>, --download <file>
-                        Write firmware from <file> into device
+                        Read firmware from device into <file>
   -R, --reset           Issue USB Reset signalling once we`re finished
-  -s <address>, --dfuse-address <address>
-                        ST DfuSe mode, specify target address for raw file download or upload. Not applicable for DfuSe file (.dfu) downloads
+  -w, --wait            Wait for device to appear
+  -s <address><:...>, --dfuse-address <address><:...>
+                        ST DfuSe mode string, specifying target
+                        address for raw file download or upload
+                        (not applicable for DfuSe file (.dfu) downloads).
+                        Add more DfuSe options separated with ':'
+
+                        leave
+                                Leave DFU mode (jump to application)
+                        mass-erase
+                                Erase the whole device (requires "force")
+                        unprotect
+                                Erase read protected device (requires "force")
+                        will-reset
+                                Expect device to reset (e.g. option bytes write)
+                        force
+                                You really know what you are doing!
+                        <length>
+                                Length of firmware to upload from device
 ```
 
-### dfu-suffix
+### pydfuutil-suffix
 ```Bash
 pydfuutil-suffix -h
 # or 
 python -m pydfuutil.suffix -h
 
-
+####### usage:
 usage: dfu-suffix [-h] [-V] (-c | -a | -D) [-p <productID>] [-v <vendorID>] [-d <deviceID>] [-s <address>] [-T] <file>
 
 positional arguments:
   <file>                Target filename
 
 options:
   -h, --help            Print this help message
@@ -307,32 +343,89 @@
   -v <vendorID>, --vid <vendorID>
                         Add vendor ID into DFU suffix in <file>
   -d <deviceID>, --did <deviceID>
                         Add device ID into DFU suffix in <file>
   -s <address>, --stellaris-address <address>
                         Specify lmdfu address for LMDFU_ADD
   -T, --stellaris       Set lmdfu mode to LMDFU_CHECK
+```
+
+### pydfuutil-prefix
+```Bash
+pydfuutil-prefix -h
+# or 
+python -m pydfuutil.prefix -h
+
+####### usage:
+usage: pydfuutil-prefix [-h] [-V] (-c | -D | -a) [-s <address>] [-T]
+                        [-L]
+                        <file>
+
+
+positional arguments:
+  <file>                Target filename
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         Print the version number
+  -c, --check           Check DFU suffix of <file>
+  -D, --delete          Delete DFU suffix from <file>
+  -a, --add             Add DFU suffix to <file>
+
+In combination with -a:
+  -s <address>, --stellaris-address <address>
+                        Add TI Stellaris address prefix to <file>
+
+In combination with -a or -D or -c:
+  -T, --stellaris       Act on TI Stellaris address prefix of <file>
 
+In combination with -a or -D or -c:
+  -L, --lpc-prefix      Use NXP LPC DFU prefix format
+```
+
+### pydfuutil-lsusb
+```Bash
+pydfuutil-lsusb -h
+# or 
+python -m pydfuutil.lsusb -h
+
+####### usage:
+usage: pydfuutil-prefix [-v] [-s [[bus]:][devnum]]
+                        [-d vendor:[product]] [-D device] [-t] [-V]    
+                        [-h]
+
+options:
+  -v, --verbose        Increase verbosity (show descriptors)
+  -s [[bus]:][devnum]  Show only devices with specified device and/or  
+                       bus numbers (in decimal)
+  -d vendor:[product]  Show only devices with the specified vendor     
+                       and product ID numbers (in hexadecimal)
+  -D device            Selects which device lsusb will examine by      
+                       UNIX-like path simulate
+  -t, --tree           Simulate UNIX-like physical USB device
+                       hierarchy
+  -V, --version        Print the version number
+  -h, --help           Show this help message and exit
 ```
 
 #### Done:
 - [x] dfu
 - [x] dfu_file
 - [x] dfu_load
 - [x] portable
 - [x] quirks
-- [x] suffix + cli entry point
+- [x] suffix
 - [x] usb_dfu
 - [x] lmdfu
 - [x] dfuse_mem
 - [x] dfuse
-- [x] dfu-util cli entry point (not fully supported yet)
+- [x] dfu-util
 
 #### Todo
-- [ ] Update sources to latest original version "dfu-util-0.11"
+- [x] Update sources to latest original version "dfu-util-0.11"
 
 [//]: # (https://dfu-util.sourceforge.net/)
 [//]: # (- https://sourceforge.net/p/dfu-util/dfu-util/ci/master/tree/)
 
 
 ## Getting help
 * To report a bug or propose a new feature, use our issue tracker. But please search the database before opening a new issue.
@@ -349,19 +442,19 @@
 USB. It ranges from small devices like micro-controller boards up to mobile
 phones. With dfu-util you are able to download firmware to your device or
 upload firmware from it.
 
 dfu-util has been tested with Openmoko Neo1973 and Freerunner and many
 other devices.
 
-* **[The official website](http://dfu-util.gnumonks.org)**
+* **[The official website](https://dfu-util.sourceforge.net/)**
 * **[DFU 1.0 spec](http://www.usb.org/developers/devclass_docs/usbdfu10.pdf)**
 * **[DFU 1.1 spec](http://www.usb.org/developers/devclass_docs/DFU_1.1.pdf)**
 
 ## RISK NOTICE
 > [!IMPORTANT]
 > THE CODE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE MATERIALS OR THE USE OR OTHER DEALINGS IN THE MATERIALS.
 
 ## Footnotes
 * On systems that still default to Python 2, replace python with python3
-* Project is in develop, it fulls of not implemented statements that's not according to original **[dfu-util](https://github.com/Stefan-Schmidt/dfu-util)**!
+* Project is in develop, it fulls issues not according to original **[dfu-util](https://github.com/Stefan-Schmidt/dfu-util)**!
```

### Comparing `pydfuutil-0.0.5/pydfuutil/dfu.py` & `pydfuutil-0.11.0b0/pydfuutil/dfu.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program; if not, write to the Free Software
 Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 """
 
-# import inspect
 import sys
 from dataclasses import dataclass
 from enum import IntEnum, IntFlag
 
 import usb.util
+from usb.core import USBError
 
+from pydfuutil.dfuse_mem import MemSegment
+from pydfuutil.exceptions import _IOError
 from pydfuutil.logger import logger
 from pydfuutil.portable import milli_sleep
 from pydfuutil.usb_dfu import FuncDescriptor
 
-_logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
+_logger = logger.getChild('dfu')
 
 
 class State(IntEnum):
     """Dfu states"""
     APP_IDLE = 0x00
     APP_DETACH = 0x01
     DFU_IDLE = 0x02
@@ -47,18 +49,15 @@
 
     UNKNOWN_ERROR = -1
 
     def to_string(self):
         """
         :return: State.self name by State Enum
         """
-        return state_to_string(self)
-
-
-
+        return _state_to_string(self)
 
 
 class Status(IntEnum):
     """Dfu statuses"""
     OK = 0x00
     ERROR_TARGET = 0x01
     ERROR_FILE = 0x02
@@ -76,44 +75,47 @@
     ERROR_UNKNOWN = 0x0e
     ERROR_STALLEDPKT = 0x0f
 
     def to_string(self):
         """
         :return: Status.self name by Status Enum
         """
-        return status_to_string(self)
+        return _status_to_string(self)
 
 
-class Command(IntEnum):
+class Request(IntEnum):
     """Dfu commands"""
     DETACH = 0
     DNLOAD = 1
     UPLOAD = 2
     GETSTATUS = 3
     CLRSTATUS = 4
     GETSTATE = 5
     ABORT = 6
 
 
 # /* DFU interface */
-class Mode(IntFlag):
+class IFF(IntFlag):
     """Dfu modes"""
-    IFF_DFU = 0x0001  # /* DFU Mode, (not Runtime) */
-    IFF_VENDOR = 0x0100
-    IFF_PRODUCT = 0x0200
-    IFF_CONFIG = 0x0400
-    IFF_IFACE = 0x0800
-    IFF_ALT = 0x1000
-    IFF_DEVNUM = 0x2000
-    IFF_PATH = 0x4000
+    DFU = 0x0001  # /* DFU Mode, (not Runtime) */
+    VENDOR = 0x0100
+    PRODUCT = 0x0200
+    CONFIG = 0x0400
+    IFACE = 0x0800
+    ALT = 0x1000
+    DEVNUM = 0x2000
+    PATH = 0x4000
     # DFU_IFF_DFU = 0x0001  /* DFU Mode, (not Runtime) */
     # DFU_IFF_ALT = 0x0002  /* Multiple alternate settings */
 
+    def __repr__(self):
+        return f"<{self.__class__.__name__}.{self._name_}: 0x{self._value_:04x}>"
 
-@dataclass(frozen=True)
+
+@dataclass
 class StatusRetVal:
     """
     Converts dfu_get_status result bytes to applicable dataclass
     This is based off of DFU_GETSTATUS
     the data structure to be populated with the results
     """
     # pylint: disable=invalid-name
@@ -162,22 +164,25 @@
     bcdDevice: int = None
     configuration: int = None
     interface: int = None
     altsetting: int = None
     alt_name: str = None
     bus: int = None
     devnum: int = None
-    path: [str, int] = None
-    flags: [Mode, int] = 0
-    count: int = None
+    path: [str, int] = None  # FIXME: deprecated
+    flags: [IFF, int] = 0
+    count: int = None  # FIXME: deprecated
     dev: usb.core.Device = None
     quirks: int = None
     bwPollTimeout: int = 0
+    bMaxPacketSize0: int = 0
     serial_name: str = ""
-    usb_dfu_func_desc: FuncDescriptor = None
+    func_dfu: FuncDescriptor = None
+    next: 'DfuIf' = None
+    mem_layout: MemSegment = None
 
 
     @property
     def device_ids(self) -> dict:
         """Returns filter dict for usb.core.find() by VID:PID"""
         id_filter = {}
         if self.vendor:
@@ -187,39 +192,42 @@
         return id_filter
 
     # The binds to direct dfu functions to get more pythonic
     # Use them better instead of direct
 
     def detach(self, timeout: int) -> bytes:
         """Binds self to dfu.detach()"""
-        return detach(self.dev, self.interface, timeout)
+        return _detach(self.dev, self.interface, timeout)
 
     def download(self, transaction: int, data_or_length: [bytes, int]) -> int:
         """Binds self to dfu.download()"""
-        return download(self.dev, self.interface, transaction, data_or_length)
+        return _download(self.dev, self.interface, transaction, data_or_length)
 
     def upload(self, transaction: int, data_or_length: [bytes, int]) -> bytes:
         """Binds self to dfu.upload()"""
-        return upload(self.dev, self.interface, transaction, data_or_length)
+        return _upload(self.dev, self.interface, transaction, data_or_length)
 
     def abort(self) -> int:
         """Binds self to dfu.abort()"""
-        return abort(self.dev, self.interface)
+        return _abort(self.dev, self.interface)
 
     def get_status(self) -> StatusRetVal:
         """Binds self to dfu.get_status()"""
-        return get_status(self.dev, self.interface)
+        return _get_status(self.dev, self.interface)
+
+    def clear_status(self) -> int:
+        return _clear_status(self.dev, self.interface)
 
     def get_state(self) -> State:
         """Binds self to dfu.get_state()"""
-        return get_state(self.dev, self.interface)
+        return _get_state(self.dev, self.interface)
 
     def abort_to_idle(self):
         """Binds self to dfu.abort_to_idle()"""
-        return abort_to_idle(self)
+        return _abort_to_idle(self)
 
 
 def init(timeout: int) -> None:
     """
     Initiate dfu_util library with specified commands timeout
     :param timeout in milliseconds
     :return: None
@@ -231,261 +239,244 @@
     if timeout > 0:
         TIMEOUT = timeout
     else:
         if 0 != DEBUG_LEVEL:
             raise ValueError(f"dfu_init: Invalid timeout value {timeout}")
 
 
-# def verify_init() -> int:
-#     """
-#     Verifies provided TIMEOUT and DEBUG_LEVEL
-#     NOTE: (function: typing.Callable) not needed cause python can get it from stack
-#     :raise ValueError with caller function name
-#     :return: 0
-#     """
-#     caller = inspect.stack()[0][3]
-#     if INVALID_DFU_TIMEOUT == TIMEOUT:
-#         if 0 != DEBUG_LEVEL:
-#             raise ValueError(f'"{caller}": dfu system not initialized properly.')
-#     return 0
-
-
 def debug(level: int) -> None:
     """
     NOTE: Maybe not needed cause python can define globals after
     :param level: logging level (DEBUG, INFO, WARNING, ERROR)
     """
 
     # pylint: disable=global-statement
     global DEBUG_LEVEL
     DEBUG_LEVEL = level
     _logger.setLevel(level)
 
 
-def detach(device: usb.core.Device, interface: int, timeout: int) -> bytes:
+def _detach(device: usb.core.Device, interface: int, timeout: int) -> bytes:
     """
     DETACH Request (DFU Spec 1.0, Section 5.1)
 
     Sends to device command to switch it to DFU mode
     u have to free device and handle it again
     :param device: the usb_dev_handle to communicate with
     :param interface: the interface to communicate with
     :param timeout: the timeout in ms the USB device should wait for a pending
     :return: bytes or < 0 on error
     """
-    # verify_init()
+
     _logger.debug('DETACH...')
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
-        bRequest=Command.DETACH,
+        bRequest=Request.DETACH,
         wValue=timeout,
         wIndex=interface,
         data_or_wLength=None,
         timeout=TIMEOUT,
     )
     _logger.debug(f'DETACH {result >= 0}')
     return result
 
 
-def download(device: usb.core.Device,
-             interface: int,
-             transaction: int,
-             data_or_length: [bytes, int]) -> int:
+def _download(device: usb.core.Device,
+              interface: int,
+              transaction: int,
+              data_or_length: [bytes, int]) -> int:
     """
     DNLOAD Request (DFU Spec 1.0, Section 6.1.1)
 
     Download data to special page of DFU device
     :param device: the usb_dev_handle to communicate with
     :param interface: the interface to communicate with
     :param transaction: start page int(total_data_size/xfer_size)
     :param data_or_length: the data to transfer
     :return: downloaded data or error code in bytes
     """
-    # verify_init()
+
     _logger.debug('DFU_DOWNLOAD...')
 
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
-        bRequest=Command.DNLOAD,
+        bRequest=Request.DNLOAD,
         wValue=transaction,
         wIndex=interface,
         data_or_wLength=data_or_length,
         timeout=TIMEOUT,
     )
 
     _logger.debug(f'DFU_DOWNLOAD {result >= 0}')
     return result
 
 
-def upload(device: usb.core.Device,
-           interface: int,
-           transaction: int,
-           data_or_length: [bytes, int]) -> bytes:
+def _upload(device: usb.core.Device,
+            interface: int,
+            transaction: int,
+            data_or_length: [bytes, int]) -> bytes:
     """
     UPLOAD Request (DFU Spec 1.0, Section 6.2)
 
     Uploads data from special page of DFU device
     :param device: the usb_dev_handle to communicate with
     :param interface: the interface to communicate with
     :param transaction: start page int(total_data_size/xfer_size)
     :param data_or_length: the buffer to put the received data in
     :return: uploaded bytes or < 0 on error
     """
-    # verify_init()
-    _logger.debug('UPLOAD...')
 
+    _logger.debug('UPLOAD...')
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_IN
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
-        bRequest=Command.UPLOAD,
+        bRequest=Request.UPLOAD,
         wValue=transaction,
         wIndex=interface,
         data_or_wLength=data_or_length,
         timeout=TIMEOUT,
     )
-
     _logger.debug(f'UPLOAD {len(result) >= 0}')
 
     return result.tobytes()
 
 
-def get_status(device: usb.core.Device, interface: int) -> StatusRetVal:
+def _get_status(device: usb.core.Device, interface: int) -> StatusRetVal:
     """
      GETSTATUS Request (DFU Spec 1.0, Section 6.1.2)
 
     Returns DFU interface status
     :param device: the usb_dev_handle to communicate with
     :param interface: the interface to communicate with
     :return: StatusRetVal
     """
-    # verify_init()
+
     _logger.debug('DFU_GET_STATUS...')
 
     length = 6
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_IN
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
-        bRequest=Command.GETSTATUS,
+        bRequest=Request.GETSTATUS,
         wValue=0,
         wIndex=interface,
         data_or_wLength=length,
         timeout=TIMEOUT,
     )
 
     if len(result) == length:
         status = StatusRetVal.from_bytes(result.tobytes())
         _logger.debug(f'GET_STATUS {len(result) == 6}')
         _logger.debug(f'CURRENT STATE {status.bState.to_string()}')
         return status
     return StatusRetVal.from_bytes(result)
 
 
-def clear_status(device: usb.core.Device, interface: int) -> int:
+def _clear_status(device: usb.core.Device, interface: int) -> int:
     """
     CLRSTATUS Request (DFU Spec 1.0, Section 6.1.3)
 
     Clears DFU interface status
     :param device: the usb_dev_handle to communicate with
     :param interface: the interface to communicate with
     :return: return 0 or < 0 on an error
     """
-    # verify_init()
+
     _logger.debug('CLEAR_STATUS...')
 
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
-        bRequest=Command.CLRSTATUS,
+        bRequest=Request.CLRSTATUS,
         wValue=0,
         wIndex=interface,
         data_or_wLength=None,
         timeout=TIMEOUT,
     )
     _logger.debug(f'CLEAR_STATUS {result >= 0}')
 
     return result
 
 
-def get_state(device: usb.core.Device, interface: int) -> [State, int]:
+def _get_state(device: usb.core.Device, interface: int) -> [State, int]:
     """
     GETSTATE Request (DFU Spec 1.0, Section 6.1.5)
 
     Returns DFU interface state
     :param device: the usb_dev_handle to communicate with
     :param interface: the interface to communicate with
     :return: returns the state or < 0 on error
     """
-    # verify_init()
 
     length = 1
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_IN
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
-        bRequest=Command.GETSTATE,
+        bRequest=Request.GETSTATE,
         wValue=0,
         wIndex=interface,
         data_or_wLength=length,
         timeout=TIMEOUT,
     )
     value = result.tobytes()[0] < 1
     if value < 1:
         return State(-1)
     if value in State.__members__.values():
         value = State(value)
     return value
 
 
-def abort(device: usb.core.Device, interface: int) -> int:
+def _abort(device: usb.core.Device, interface: int) -> int:
     """
     ABORT Request (DFU Spec 1.0, Section 6.1.4)
 
     Aborts DFU command
     :param device: the usb_dev_handle to communicate with
     :param interface: the interface to communicate with
     :return: returns 0 or < 0 on an error
     """
-    # verify_init()
+
     _logger.debug('ABORT...')
 
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
-        bRequest=Command.ABORT,
+        bRequest=Request.ABORT,
         wValue=0,
         wIndex=interface,
         data_or_wLength=None,
         timeout=TIMEOUT,
     )
 
     _logger.debug(f'ABORT {result >= 0}')
 
     return result
 
 
-def state_to_string(state: int) -> [str, None]:
+def _state_to_string(state: int) -> [str, None]:
     """
     :param state:
     :return: State name by State Enum
     """
     try:
         return _STATES_NAMES[State(state)]
     except (ValueError, KeyError):
         return None
 
 
-def status_to_string(status: int) -> [str, None]:
+def _status_to_string(status: int) -> [str, None]:
     """
     :param status:
     :return: State name by Status Enum
     """
     try:
         return _DFU_STATUS_NAMES[Status(status)]
     except (ValueError, KeyError):
@@ -502,15 +493,14 @@
     State.DFU_MANIFEST_SYNC: 'dfuMANIFEST-SYNC',
     State.DFU_MANIFEST: 'dfuMANIFEST',
     State.DFU_MANIFEST_WAIT_RESET: 'dfuMANIFEST-WAIT-RESET',
     State.DFU_UPLOAD_IDLE: 'dfuUPLOAD-IDLE',
     State.DFU_ERROR: 'dfuERROR',
 }
 
-
 _DFU_STATUS_NAMES = {
     Status.OK: "No error condition is present",
     Status.ERROR_TARGET: "File is not targeted for use by this device",
     Status.ERROR_FILE: "File is for this device but fails some vendor-specific test",
     Status.ERROR_WRITE: "Device is unable to write memory",
     Status.ERROR_ERASE: "Memory erase function failed",
     Status.ERROR_CHECK_ERASED: "Memory erase check failed",
@@ -525,30 +515,41 @@
     Status.ERROR_USBR: "Device detected unexpected USB reset signalling",
     Status.ERROR_POR: "Device detected unexpected power on reset",
     Status.ERROR_UNKNOWN: "Something went wrong, but the device does not know what it was",
     Status.ERROR_STALLEDPKT: "Device stalled an unexpected request"
 }
 
 
-def abort_to_idle(dif: DfuIf):
-    if dif.abort() < 0:
-        _logger.error("Error sending dfu abort request")
-        sys.exit(1)
-    if (ret := int(dst := dif.get_status())) < 0:
-        _logger.error("Error during abort get_status")
-        sys.exit(1)
+def _abort_to_idle(dif: DfuIf):
+    try:
+        dif.abort()
+    except USBError:
+        raise _IOError("Error sending dfu abort request")
+    try:
+        dst = dif.get_status()
+    except USBError:
+        raise _IOError("Error during abort get_status")
     if dst.bState != State.DFU_IDLE:
-        _logger.error("Failed to enter idle state on abort")
-        sys.exit(1)
+        raise _IOError("Failed to enter idle state on abort")
     milli_sleep(dst.bwPollTimeout)
-    return ret
+    return dst
 
 
 # global definitions
 DEBUG: int = 0
 
 INVALID_DFU_TIMEOUT = -1
 
 TIMEOUT: int = INVALID_DFU_TIMEOUT
 TRANSACTION: int = 0
 
 DEBUG_LEVEL: int = 0
+
+__all__ = (
+    "Request",
+    "Status",
+    "State",
+    "StatusRetVal",
+    "DfuIf",
+    'IFF',
+    'init'
+)
```

### Comparing `pydfuutil-0.0.5/pydfuutil/dfu_file.py` & `pydfuutil-0.11.0b0/pydfuutil/dfu_file.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,32 +13,26 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program; if not, write to the Free Software
 Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 """
-
+import errno
 import io
-import os
 import struct
 import sys
 import warnings
 from dataclasses import dataclass, field
-from enum import Enum
-
-from construct import (Struct, Const, ByteSwapped, Default,
-                       Int32ub, Int16ub, Int8sb,
-                       ConstError, StreamError)
+from enum import IntEnum
 
+from pydfuutil.exceptions import NoInputError, _IOError, DataError, except_and_safe_exit, UsageError
 from pydfuutil.logger import logger
 
-__all__ = ('DFUFile', 'parse_dfu_suffix', 'generate_dfu_suffix')
-
-_logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
+_logger = logger.getChild('dfu_file')
 
 DFU_SUFFIX_LENGTH = 16
 LMDFU_PREFIX_LENGTH = 8
 LPCDFU_PREFIX_LENGTH = 16
 STDIN_CHUNK_SIZE = 65536
 
 crc32_table = [
@@ -83,104 +77,82 @@
     0xa7672661, 0xd06016f7, 0x4969474d, 0x3e6e77db, 0xaed16a4a, 0xd9d65adc,
     0x40df0b66, 0x37d83bf0, 0xa9bcae53, 0xdebb9ec5, 0x47b2cf7f, 0x30b5ffe9,
     0xbdbdf21c, 0xcabac28a, 0x53b39330, 0x24b4a3a6, 0xbad03605, 0xcdd70693,
     0x54de5729, 0x23d967bf, 0xb3667a2e, 0xc4614ab8, 0x5d681b02, 0x2a6f2b94,
     0xb40bbe37, 0xc30c8ea1, 0x5a05df1b, 0x2d02ef8d
 ]
 
-_suffix = ByteSwapped(Struct(
-    dwCRC=Default(Int32ub, 0xffffffff),
-    bLength=Const(DFU_SUFFIX_LENGTH, Int8sb),
-    ucDfuSignature=Const(b'DFU'),
-    bcdDFU=Int16ub,
-    idVendor=Int16ub,
-    idProduct=Int16ub,
-    bcdDevice=Int16ub,
-))
-
-
-@dataclass
-class DFUFile:  # pylint: disable=too-many-instance-attributes, invalid-name
-    """Class to store DFU file data"""
-    name: [str, None]
-    file_p: io.FileIO = None
-    size: int = 0
-    dwCRC: int = 0
-    suffix_len: int = 0
-    bcdDFU: int = 0
-    idVendor: int = 0xffff  # wildcard value
-    idProduct: int = 0xffff  # wildcard value
-    bcdDevice: int = 0xffff  # wildcard value
-
-    def parse_dfu_suffix(self) -> int:
-        """Bind parse_dfu_suffix to DFUFile instance"""
-        return parse_dfu_suffix(self)
-
-    def generate_dfu_suffix(self) -> int:
-        """Bind generate_dfu_suffix to DFUFile instance"""
-        return generate_dfu_suffix(self)
-
 
 @dataclass
 class DFUFileSize:
-    total: int
-    prefix: int
-    suffix: int
+    """Dfu file size struct"""
+    total: int = 0
+    prefix: int = 0
+    suffix: int = 0
 
 
-class SuffixReq(Enum):
+class SuffixReq(IntEnum):
+    """Suffix requirement"""
     NO_SUFFIX = 0
     NEEDS_SUFFIX = 1
     MAYBE_SUFFIX = 2
 
 
-class PrefixReq(Enum):
-    NO_SUFFIX = 0
-    NEEDS_SUFFIX = 1
-    MAYBE_SUFFIX = 2
+class PrefixReq(IntEnum):
+    """Prefix requirement"""
+    NO_PREFIX = 0
+    NEEDS_PREFIX = 1
+    MAYBE_PREFIX = 2
 
 
-class PrefixType(Enum):
+class PrefixType(IntEnum):
+    """Dfu prefix type"""
     ZERO_PREFIX = 0
     LMDFU_PREFIX = 1
     LPCDFU_UNENCRYPTED_PREFIX = 2
 
 
 @dataclass
-class DFUFile011:  # pylint: disable=too-many-instance-attributes, invalid-name
+class DfuFile:  # pylint: disable=too-many-instance-attributes, invalid-name
     """Class to store DFU file data"""
     name: [str, None]
     firmware: [bytearray, bytes] = field(default_factory=bytearray)
     file_p: io.FileIO = None
-    size: DFUFileSize = None
+    size: DFUFileSize = field(default_factory=DFUFileSize)
     lmdfu_address: int = 0
-    prefix_type: PrefixType = None
+    prefix_type: PrefixType = PrefixType.ZERO_PREFIX
     dwCRC: int = 0
     bcdDFU: int = 0
     idVendor: int = 0xffff  # wildcard value
     idProduct: int = 0xffff  # wildcard value
     bcdDevice: int = 0xffff  # wildcard value
 
-    def parse_dfu_suffix(self) -> int:
-        """Bind parse_dfu_suffix to DFUFile instance"""
-        return parse_dfu_suffix(self)
-
-    def generate_dfu_suffix(self) -> int:
-        """Bind generate_dfu_suffix to DFUFile instance"""
-        return generate_dfu_suffix(self)
+    def dump(self, write_suffix: bool, write_prefix: bool) -> None:
+        """writes suffix and/or prefix to dfu file"""
+        return _store_file(self, write_suffix, write_prefix)
+
+    def load(self, check_suffix: SuffixReq, check_prefix: PrefixReq) -> None:
+        """loads suffix and/or prefix from dfu file"""
+        return _load_file(self, check_suffix, check_prefix)
+
+    def write_crc(self, crc: int, buf: [bytes, bytearray]) -> int:
+        """writes desired data to dfu file"""
+        return _write_crc(self.file_p, crc, buf)
+
+    def show_suffix_and_prefix(self) -> None:
+        """Prints suffix and prefix of dfu file"""
+        _show_suffix_and_prefix(self)
 
 
 def crc32_byte(accum: int, delta: int):
-    """
-    Calculate a 32-bit CRC
-    """
+    """Calculate a 32-bit CRC"""
     return crc32_table[(accum ^ delta) & 0xff] ^ (accum >> 8)
 
 
-def probe_prefix(file: DFUFile011):
+def _probe_prefix(file: DfuFile):
     prefix = file.firmware
 
     if file.size.total < LMDFU_PREFIX_LENGTH:
         return 1
     if prefix[0] == 0x01 and prefix[1] == 0x00:
         payload_len = ((prefix[7] << 24) | (prefix[6] << 16)
                        | (prefix[5] << 8) | prefix[4])
@@ -195,197 +167,190 @@
         file.prefix_type = PrefixType.LPCDFU_UNENCRYPTED_PREFIX
         file.size.prefix = LPCDFU_PREFIX_LENGTH
     if file.size.prefix + file.size.suffix > file.size.total:
         return 1
     return 0
 
 
-def write_crc(f: DFUFile.file_p, crc: int, buf: [bytes, bytearray], size: int) -> int:
+def _write_crc(f: [io.FileIO, io.BytesIO], crc: int, buf: [bytes, bytearray]) -> int:
+    """writes desired data to dfu file"""
+
     # compute CRC
+    size = len(buf)
     for x in range(0, size):
         crc = crc32_byte(crc, buf[x])
 
     # write data
-    if f.write(buf, size) != size:
-        _logger.error(f"Could not write {size} bytes to {f}")
+    if f.write(buf) != size:
+        raise _IOError(f"Could not write {size} bytes to {f}")
 
     return crc
 
 
-def load_file(file: DFUFile011, check_suffix: SuffixReq, check_prefix: PrefixReq):
+@except_and_safe_exit(_logger)
+def _load_file(file: DfuFile, check_suffix: SuffixReq, check_prefix: PrefixReq) -> None:
+    """loads suffix and/or prefix from dfu file"""
 
     file.size.prefix = 0
     file.size.suffix = 0
 
-    # default values, if no valid suffix is found
     file.bcdDFU = 0
-    file.idVendor = 0xffff  # wildcard value
-    file.idProduct = 0xffff  # wildcard value
-    file.bcdDevice = 0xffff  # wildcard value
+    file.idVendor = 0xffff
+    file.idProduct = 0xffff
+    file.bcdDevice = 0xffff
 
-    # default values, if no valid prefix is found
     file.lmdfu_address = 0
-
-    file.firmware = None
-
-    if file.name and file.name != '-':
-
-        if sys.stdin.isatty():
-            print("Please provide input via stdin.")
-            return None
-
-        # Check if the platform is Windows
-        if sys.platform.startswith("win"):
-            import msvcrt
-            # Set stdin to binary mode
-            msvcrt.setmode(sys.stdin.fileno(), os.O_BINARY)
-
+    if file.name == "-":
         file.firmware = bytearray()
         read_bytes = sys.stdin.buffer.read(STDIN_CHUNK_SIZE)
-        file.firmware += read_bytes
-        file.size.total = len(read_bytes)
-
-        while len(read_bytes) == STDIN_CHUNK_SIZE:
+        while read_bytes:
+            file.firmware.extend(read_bytes)
             read_bytes = sys.stdin.buffer.read(STDIN_CHUNK_SIZE)
-            file.firmware += read_bytes
-            file.size.total += len(read_bytes)
-
+        file.size.total = len(file.firmware)
         _logger.debug(f"Read {file.size.total} bytes from stdin")
 
-        # Never require suffix when reading from stdin
-        check_suffix = SuffixReq.MAYBE_SUFFIX
+        check_suffix = PrefixReq.MAYBE_PREFIX
     else:
-        with open(file.name, 'rb') as file.file_p:
-            file.firmware = file.file_p.read()
-            file.size.total = len(file.firmware)
-
-    # TODO
-    raise NotImplementedError
-    # # Check for possible DFU file suffix by trying to parse one
-    # if check_suffix != SuffixReq.NO_SUFFIX:
-    #     dfusuffix = file.firmware[-16:] if file.size['total'] >= 16 else None
-    #     missing_suffix = False
-    #     reason = None
-    #
-    #     if not dfusuffix:
-    #         reason = "File too short for DFU suffix"
-    #         missing_suffix = True
-    #     elif dfusuffix[10:13] != b'DFU':
-    #         reason = "Invalid DFU suffix signature"
-    #         missing_suffix = True
-    #     else:
-    #         crc = 0xffffffff
-    #         for byte in file.firmware[:-16]:
-    #             crc = crc32_byte(crc, byte)
-    #
-    #         file.dwCRC = struct.unpack('<I', dfusuffix[12:16])[0]
-    #         if file.dwCRC != crc:
-    #             reason = "DFU suffix CRC does not match"
-    #             missing_suffix = True
-    #         else:
-    #             file.bcdDFU = struct.unpack('<H', dfusuffix[6:8])[0]
-    #             _logger.debug(f"DFU suffix version {file.bcdDFU}")
-    #
-    #             file.size.suffix = dfusuffix[11]
-    #             if file.size.suffix < 16:
-    #                 raise ValueError("Unsupported DFU suffix length")
-    #             if file.size.suffix > file.size.total:
-    #                 raise ValueError("Invalid DFU suffix length")
-    #
-    #             file.idVendor = struct.unpack('<H', dfusuffix[4:6])[0]
-    #             file.idProduct = struct.unpack('<H', dfusuffix[2:4])[0]
-    #             file.bcdDevice = struct.unpack('<H', dfusuffix[0:2])[0]
-    #
-    #     if missing_suffix:
-    #         if check_suffix == SuffixReq.NEEDS_SUFFIX:
-    #             _logger.info(f"{reason}")
-    #             _logger.info("A valid DFU suffix will be required in a future dfu-util release")
-    #             # raise ValueError("Valid DFU suffix needed")
-    #
-    #     elif check_suffix == SuffixReq.MAYBE_SUFFIX:
-    #         _logger.warning(f"{reason}")
+        try:
+            with open(file.name, "rb") as f:
+                file.firmware = f.read()
+                file.size.total = len(file.firmware)
+        except IOError as e:
+            if e.errno == errno.ENOENT:
+                raise NoInputError(f"Could not open file {file.name} for reading") from e
+            if e.errno == errno.EACCES:
+                raise _IOError(f"Permission denied: {file.name}") from e
+            raise _IOError(f"Error reading file {file.name}: {e}") from e
+
+    missing_suffix, reason = False, None
+    if file.size.total < DFU_SUFFIX_LENGTH:
+        reason = "File too short for DFU suffix"
+        missing_suffix = True
+    else:
+        dfu_suffix = file.firmware[-DFU_SUFFIX_LENGTH:]
+
+        crc = 0xffffffff
+        for byte in file.firmware[:-4]:
+            crc = crc32_byte(crc, byte)
+
+        if dfu_suffix[8:11] != b'UFD':
+            reason = "Invalid DFU suffix signature"
+            missing_suffix = True
+        elif struct.unpack('<I', dfu_suffix[12:])[0] != crc:
+            reason = "DFU suffix CRC does not match"
+            missing_suffix = True
+        else:
+            file.bcdDFU = struct.unpack('<H', dfu_suffix[6:8])[0]
+            _logger.debug(f"DFU suffix version {file.bcdDFU}")
+
+            file.size.suffix = dfu_suffix[11]
+            if file.size.suffix < DFU_SUFFIX_LENGTH:
+                raise DataError(f"Unsupported DFU suffix length {file.size.suffix}")
+            if file.size.suffix > file.size.total:
+                raise DataError(f"Invalid DFU suffix length {file.size.suffix}")
+
+            file.idVendor = struct.unpack('<H', dfu_suffix[4:6])[0]
+            file.idProduct = struct.unpack('<H', dfu_suffix[2:4])[0]
+            file.bcdDevice = struct.unpack('<H', dfu_suffix[0:2])[0]
+
+    if missing_suffix:
+        if check_suffix == PrefixReq.NEEDS_PREFIX:
+            raise DataError(reason + " Valid DFU suffix needed")
+        if check_suffix == PrefixReq.MAYBE_PREFIX:
+            _logger.warning(f"{reason}")
+            warnings.warn(
+                "A valid DFU suffix will be required in a future dfu-util release",
+                FutureWarning
+            )
+    else:
+        if check_suffix == PrefixReq.NO_PREFIX:
+            raise DataError("Please remove existing DFU suffix before adding a new one.")
 
+    res = _probe_prefix(file)
+    if (res or file.size.prefix == 0) and check_prefix == PrefixReq.NEEDS_PREFIX:
+        raise UsageError("Valid DFU prefix needed")
+    if file.size.prefix and check_prefix == PrefixReq.NO_PREFIX:
+        raise DataError("A prefix already exists, please delete it first")
+    if file.size.prefix:
+        data = file.firmware
+        if file.prefix_type == PrefixType.LMDFU_PREFIX:
+            _logger.debug(f"Possible TI Stellaris DFU prefix with the following properties\n"
+                          f"Address:        0x{file.lmdfu_address:08x}\n"
+                          f"Payload length: {struct.unpack('<I', data[4:8])[0]}")
+        elif file.prefix_type == PrefixType.LPCDFU_UNENCRYPTED_PREFIX:
+            _logger.info(f"Possible unencrypted NXP LPC DFU prefix with the following properties\n"
+                         f"Payload length: {struct.unpack('<H', data[2:4])[0] >> 1} kiByte")
+        else:
+            raise DataError("Unknown DFU prefix type")
+
+
+@except_and_safe_exit(_logger)
+def _store_file(file: DfuFile, write_suffix: bool, write_prefix: bool) -> None:
+    """writes suffix and/or prefix to dfu file"""
 
-def store_file(file: DFUFile011, write_suffix: int, write_prefix: int):
     crc = 0xffffffff
 
     try:
         with open(file.name, 'wb') as file.file_p:
 
-            # write prefix, if any
+            # Write prefix, if any
             if write_prefix:
                 if file.prefix_type == PrefixType.LMDFU_PREFIX:
-                    lmdfu_prefix = bytearray(LMDFU_PREFIX_LENGTH)
                     addr = file.lmdfu_address // 1024
+                    len_payload = file.size.total - file.size.prefix - file.size.suffix
 
-                    # lmdfu_dfu_prefix payload length excludes prefix and suffix
-                    len_ = file.size.total - file.size.prefix - file.size.suffix
-
+                    lmdfu_prefix = bytearray(LMDFU_PREFIX_LENGTH)
                     lmdfu_prefix[0] = 0x01  # STELLARIS_DFU_PROG
-                    lmdfu_prefix[1] = 0x00  # Reserved
-                    lmdfu_prefix[2] = addr & 0xff
-                    lmdfu_prefix[3] = addr >> 8
-                    lmdfu_prefix[4] = len_ & 0xff
-                    lmdfu_prefix[5] = (len_ >> 8) & 0xff
-                    lmdfu_prefix[6] = (len_ >> 16) & 0xff
-                    lmdfu_prefix[7] = (len_ >> 24)
-
-                    crc = write_crc(file.file_p, crc, lmdfu_prefix, LMDFU_PREFIX_LENGTH)
-
-                if file.prefix_type == PrefixType.LPCDFU_UNENCRYPTED_PREFIX:
-                    lpcdfu_prefix = bytearray(LPCDFU_PREFIX_LENGTH)
-
-                    # Payload is firmware and prefix rounded to 512 bytes
-                    len_ = (file.size.total - file.size.suffix + 511) // 512
-
-                    lpcdfu_prefix[0] = 0x1a  # Unencypted
-                    lpcdfu_prefix[1] = 0x3f  # Reserved
-                    lpcdfu_prefix[2] = (len_ & 0xff)
-                    lpcdfu_prefix[3] = (len_ >> 8) & 0xff
+                    lmdfu_prefix[2:4] = addr.to_bytes(2, 'little')
+                    lmdfu_prefix[4:8] = len_payload.to_bytes(4, 'little')
+
+                    crc = _write_crc(file.file_p, crc, lmdfu_prefix)
+
+                elif file.prefix_type == PrefixType.LPCDFU_UNENCRYPTED_PREFIX:
+                    len_payload = (file.size.total - file.size.suffix + 511) // 512
+
+                    lpc_dfu_prefix = bytearray(LPCDFU_PREFIX_LENGTH)
+                    lpc_dfu_prefix[0] = 0x1a  # Unencrypted
+                    lpc_dfu_prefix[1] = 0x3f  # Reserved
+                    lpc_dfu_prefix[2:4] = len_payload.to_bytes(2, 'little')
+
                     for i in range(12, LPCDFU_PREFIX_LENGTH):
-                        lpcdfu_prefix[i] = 0xff
+                        lpc_dfu_prefix[i] = 0xff
 
-                    crc = write_crc(file.file_p, crc, lpcdfu_prefix, LPCDFU_PREFIX_LENGTH)
+                    crc = _write_crc(file.file_p, crc, lpc_dfu_prefix)
 
-            # write firmware binary
-            crc = write_crc(file.file_p, crc, file.firmware[file.size.prefix:],
-                            file.size.total + file.size.prefix + file.size.suffix)
+            # Write firmware binary
+            crc = _write_crc(file.file_p, crc,
+                             file.firmware[file.size.prefix:file.size.total - file.size.suffix])
 
-            # write suffix, if any
+            # Write suffix, if any
             if write_suffix:
-                dfusuffix = bytearray(DFU_SUFFIX_LENGTH)
+                dfu_suffix = bytearray(16)
+                dfu_suffix[0:2] = file.bcdDevice.to_bytes(2, 'little')
+                dfu_suffix[2:4] = file.idProduct.to_bytes(2, 'little')
+                dfu_suffix[4:6] = file.idVendor.to_bytes(2, 'little')
+                dfu_suffix[6:8] = file.bcdDFU.to_bytes(2, 'little')
+                dfu_suffix[8:11] = b'UFD'
+                dfu_suffix[11] = DFU_SUFFIX_LENGTH
+
+                crc = file.write_crc(crc, dfu_suffix[:-4])
+
+                dfu_suffix[12:16] = crc.to_bytes(4, 'little')
+                _write_crc(file.file_p, crc, dfu_suffix[12:])
+
+    except IOError as e:
+        if e.errno == errno.ENOENT:
+            raise _IOError(f"Could not open file {file.name} for writing") from e
+        if e.errno == errno.EACCES:
+            raise _IOError(f"Permission denied: {file.name}") from e
+        raise _IOError(f"Error opening file {file.name}: {e}") from e
 
-                dfusuffix[0] = file.bcdDevice & 0xff
-                dfusuffix[1] = file.bcdDevice >> 8
-                dfusuffix[2] = file.idProduct & 0xff
-                dfusuffix[3] = file.idProduct >> 8
-                dfusuffix[4] = file.idVendor & 0xff
-                dfusuffix[5] = file.idVendor >> 8
-                dfusuffix[6] = file.bcdDFU & 0xff
-                dfusuffix[7] = file.bcdDFU >> 8
-                dfusuffix[8] = ord('U')
-                dfusuffix[9] = ord('F')
-                dfusuffix[10] = ord('D')
-                dfusuffix[11] = DFU_SUFFIX_LENGTH
-
-                crc = write_crc(file.file_p, crc, dfusuffix, DFU_SUFFIX_LENGTH - 4)
-
-                dfusuffix[12] = crc
-                dfusuffix[13] = crc >> 8
-                dfusuffix[14] = crc >> 16
-                dfusuffix[15] = crc >> 24
-
-                crc = write_crc(file.file_p, crc, dfusuffix[12:], 4)
-
-    except OSError as err:
-        _logger.debug(err)
-        raise OSError(f"Could not open file {file.name} for writing")
 
-
-def show_suffix_and_prefix(file: DFUFile011) -> None:
+def _show_suffix_and_prefix(file: DfuFile) -> None:
+    """Prints suffix and prefix of dfu file"""
 
     if file.size.prefix == LPCDFU_PREFIX_LENGTH:
         print(f"The file {file.name} contains a TI Stellaris "
               f"DFU prefix with the following properties:")
         print(f"Address:\t0x{file.lmdfu_address:08x}")
     elif file.size.prefix == LPCDFU_PREFIX_LENGTH:
         prefix = file.firmware
@@ -402,126 +367,13 @@
         print(f"Product ID:\t0x{file.idProduct:04X}")
         print(f"Vendor ID:\t0x{file.idVendor:04X}")
         print(f"BCD DFU:\t0x{file.bcdDFU:04X}")
         print(f"Length:\t\t{file.size.suffix}")
         print(f"CRC:\t\t0x{file.dwCRC:08X}")
 
 
-def parse_dfu_suffix(file: DFUFile) -> int:
-    """
-    reads the file_p and name member, fills in all others
-    FIXME: deprecated
-    :param file:
-    :return: 0 if no DFU suffix, positive if valid DFU suffix, negative on file read error
-    """
-    warnings.warn("parse_dfu_suffix is deprecated", FutureWarning)
-
-    crc = 0xffffffff
-    dfu_suffix = bytearray([0] * DFU_SUFFIX_LENGTH)
-
-    try:
-        with io.FileIO(file.name, 'rb') as file.file_p:
-            file.size = file.file_p.seek(0, os.SEEK_END)
-            file.file_p.seek(0)
-
-            if file.size < DFU_SUFFIX_LENGTH:
-                _logger.error("File too short for DFU suffix")
-                return 0
-
-            firmware = bytearray(file.file_p.read(file.size))
-
-            for i in range(file.size - 4):
-                crc = crc32_byte(crc, firmware[i])
-
-            del firmware
-
-            file.file_p.seek(-DFU_SUFFIX_LENGTH, os.SEEK_END)
-            ret = file.file_p.readinto(dfu_suffix)
-
-            if ret < 0:
-                _logger.error("Could not read DFU suffix")
-                return ret
-            if ret < DFU_SUFFIX_LENGTH:
-                _logger.error("Could not read whole DFU suffix")
-                return -1
-
-            suffix = _suffix.parse(dfu_suffix)
-            file.dwCRC = suffix.dwCRC
-
-            if file.dwCRC != crc:
-                _logger.error("DFU CRC does not match")
-                return 0
-
-            file.bcdDFU = suffix.bcdDFU
-            _logger.info(f"Dfu suffix version {hex(file.bcdDFU)}")
-
-            file.suffix_len = dfu_suffix[11]
-            if file.suffix_len < DFU_SUFFIX_LENGTH:
-                _logger.error(f"Unsupported DFU suffix length {file.suffix_len}")
-                return 0
-
-            file.idVendor = suffix.idVendor
-            file.idProduct = suffix.idProduct
-            file.bcdDevice = suffix.bcdDevice
-
-    except StreamError as e:
-        _logger.error(f"Could not read whole DFU suffix, {e}")
-        ret = -1
-    except ConstError as e:
-        _logger.error(f"No valid DFU suffix signature, {e}")
-        ret = 0
-    except Exception as e:
-        _logger.exception(e)
-        ret = -1
-    return ret
-
-
-def generate_dfu_suffix(file: DFUFile) -> int:
-    """
-    reads file, generates CRC and adds DFU suffix to file
-    :param file:
-    :return: positive on success, negative on errors
-    """
-    warnings.warn("generate_dfu_suffix is deprecated", FutureWarning)
-
-    file.size = 0
-    file.dwCRC = 0xffffffff
-    file.suffix_len = DFU_SUFFIX_LENGTH
-    file.bcdDFU = 0x0100  # Default to bcdDFU version 1.0
-
-    suffix_data = {
-        'bcdDevice': file.bcdDevice,
-        'idProduct': file.idProduct,
-        'idVendor': file.idVendor,
-        'bcdDFU': file.bcdDFU,
-        'bLength': file.suffix_len
-    }
-
-    dfu_suffix = bytearray(_suffix.build(suffix_data))
-
-    try:
-        with io.FileIO(file.name, 'rb+') as file_p:
-            file.size = file_p.seek(0, os.SEEK_END)
-            file_p.seek(0)
-
-            # Make space for all but CRC
-            firmware = bytearray(file_p.read(file.size))
-            firmware.extend(dfu_suffix[:12])
-            # Calculate CRC. It is calculated over file and suffix excluding the CRC itself
-            for i in range(file.size + file.suffix_len - 4):
-                file.dwCRC = crc32_byte(file.dwCRC, firmware[i])
-
-            del firmware
-
-            dfu_suffix[12:16] = ByteSwapped(_suffix.subcon.dwCRC).build(file.dwCRC)
-
-            # Move to the end of the file
-            file_p.seek(0, os.SEEK_END)
-
-            # Add the suffix at the end of the file
-            ret = file_p.write(dfu_suffix)
-
-    except Exception as e:
-        _logger.exception(e)
-        ret = -1
-
-    return ret
+__all__ = (
+    'DfuFile',
+    'SuffixReq',
+    'PrefixReq',
+    'PrefixType',
+)
```

### Comparing `pydfuutil-0.0.5/pydfuutil/dfu_load.py` & `pydfuutil-0.11.0b0/pydfuutil/dfu_load.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,194 +18,177 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program; if not, write to the Free Software
 Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 """
-import logging
-
-import usb
-
+from usb.core import USBError
 from pydfuutil import dfu
-from pydfuutil.dfu_file import DFUFile
+from pydfuutil.dfu_file import DfuFile
+from pydfuutil.exceptions import _IOError, SoftwareError, except_and_safe_exit
 from pydfuutil.logger import logger
 from pydfuutil.portable import milli_sleep
 from pydfuutil.progress import Progress
-from pydfuutil.quirks import QUIRK_POLLTIMEOUT, DEFAULT_POLLTIMEOUT
+from pydfuutil.quirks import QUIRK, DEFAULT_POLLTIMEOUT
 
-_logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
+_logger = logger.getChild('dfu_load')
 
 
+@except_and_safe_exit(_logger)
 def do_upload(dif: dfu.DfuIf,
               xfer_size: int,
-              file: DFUFile = None,
+              file: DfuFile = None,
               expected_size: int = -1) -> [int, bytes]:
     """
     Uploads data from DFU device from special page
     :param dif: dfu.dfu_if
     :param xfer_size: chunk size
-    :param file: optional - DFUFile object
+    :param file: optional - DfuFile object
     :param expected_size: optional - total bytes expected to be uploaded
     :return: uploaded bytes or error code
     """
 
     _logger.info("Copying data from DFU device to PC")
 
     total_bytes = 0
     transaction = dfu.TRANSACTION  # start page
-    buf = bytearray(xfer_size)
 
     with Progress() as progress:
-        progress_total = expected_size if expected_size >= 0 else None
         progress.start_task(
             description="Starting upload",
-            total=progress_total
+            total=expected_size if expected_size >= 0 else None
         )
-        # ret = 0  # need there?
-        try:
-            while True:
-                rc = dif.upload(transaction, buf)
+        while True:
+            try:
+                rc = dif.upload(transaction, xfer_size)
+            except USBError as e:
+                _logger.warning(f"Error during upload: {e}")
+                ret = rc
+                break
 
-                if len(rc) < 0:
-                    _logger.error("Error during upload")
-                    ret = rc
-                    break
+            file.write_crc(0, rc)
 
-                if file:
-                    write_rc = file.file_p.write(rc)
-                    # TODO: replace to dfu_file_write_crc
+            total_bytes += len(rc)
 
-                    if write_rc < len(rc):
-                        _logger.error(f'Short file write: {write_rc}')
-                        ret = total_bytes
-                        break
+            if total_bytes < 0:
+                raise SoftwareError("Received too many bytes (wraparound)")
 
-                total_bytes += len(rc)
+            transaction += 1
+            progress.update(advance=len(rc), description="Uploading...")
 
-                if total_bytes < 0:
-                    raise IOError("Received too many bytes (wraparound)")
+            # last block, return
+            if len(rc) < xfer_size or total_bytes >= expected_size >= 0:
+                ret = total_bytes
+                break
 
+        progress.update(description='Upload finished!')
 
-                transaction += 1
-                progress.update(advance=len(rc), description="Uploading...")
+        _logger.debug(f"Received a total of {total_bytes} bytes")
 
-                # last block, return
-                if (len(rc) < xfer_size) or (total_bytes >= expected_size >= 0):
-                    ret = total_bytes
-                    break
+        if expected_size not in (0, total_bytes):
+            _logger.warning("Unexpected number of bytes uploaded from device")
 
-            progress.update(description='Upload finished!')
-
-            _logger.debug(f"Received a total of {total_bytes} bytes")
-
-            if expected_size != 0 and total_bytes != expected_size:
-                _logger.warning("Unexpected number of bytes uploaded from device")
-
-            return ret
-        except IOError as e:
-            _logger.error(e)
-            return -1
+        return ret
 
 
 # pylint: disable=too-many-branches
-def do_dnload(dif: dfu.DfuIf, xfer_size: int, file: DFUFile, quirks: int) -> int:
+@except_and_safe_exit(_logger)
+def do_download(dif: dfu.DfuIf, xfer_size: int, file: DfuFile) -> int:
     """
     :param dif: DfuIf instance
     :param xfer_size: transaction size
-    :param file: DFUFile instance
-    :param quirks: quirks  TODO: replace to DFUFile011 with quirks
+    :param file: DfuFile instance
     verbose: is verbose useless cause of using python's logging
     :return:
     """
 
+    buf = file.firmware
+
+    expected_size = file.size.total - file.size.suffix
     bytes_sent = 0
-    # # TODO: new one
-    # buf = file.firmware
-    # expected_size = file.size.total - file.size.suffix;
-    # bytes_sent = 0
-    buf = bytearray(xfer_size)
 
     _logger.info("Copying data from PC to DFU device")
 
-    try:
+    with Progress() as progress:
+        progress.start_task(
+            description="Starting download",
+            total=expected_size if expected_size >= 0 else None
+        )
 
-        with Progress() as progress:
-            total_size = file.size - file.suffix_len  # TODO: replace to expected_size
-            progress.start_task(
-                description="Starting download",
-                total=total_size if total_size >= 0 else None
-            )
-
-            while bytes_sent < file.size - file.suffix_len:
-                # Note: no idea what's there
-                # bytes_left = file.size - file.suffix_len - bytes_sent
-                # chunk_size = min(bytes_left, xfer_size)
+        while bytes_sent < expected_size:
+            # Note: no idea what's there
+            # bytes_left = file.size - file.suffix_len - bytes_sent
+            # chunk_size = min(bytes_left, xfer_size)
 
-                if (ret := file.file_p.readinto(buf)) < 0:  # Handle read error
-                    raise IOError(f"Error reading file: {file.name}")
+            if (ret := file.file_p.readinto(buf)) < 0:  # Handle read error
+                raise _IOError(f"Error reading file: {file.name}")
 
+            try:
                 ret = dif.download(ret, buf[:ret] if ret else None)
+            except USBError as e:
+                raise _IOError(f"Error during download: {e}") from e
+            bytes_sent += ret
+
+            while True:
+                try:
+                    status = dif.get_status()
+                except USBError as e:
+                    raise _IOError(f"Error during download get_status {e}") from e
+                if status.bState in (dfu.State.DFU_DOWNLOAD_IDLE, dfu.State.DFU_ERROR):
+                    break
+                # Wait while the device executes flashing
+                milli_sleep(
+                    DEFAULT_POLLTIMEOUT
+                    if dif.quirks & QUIRK.POLLTIMEOUT
+                    else status.bwPollTimeout
+                )
+
+            if status.bStatus != dfu.Status.OK:
+                logger.error("Transfer failed!")
+                logger.info(f"state({status.bState}) = {status.bState.to_string()}, "
+                            f"status({status.bStatus}) = {status.bStatus.to_string()}")
+                raise _IOError("Downloading failed!")
 
-                if ret < 0:
-                    raise IOError("Error during download")
-                bytes_sent += ret
-
-                while True:
-                    if int(status := dif.get_status()) < 0:
-                        raise IOError("Error during download get_status")
-                    if status.bState in (dfu.State.DFU_DOWNLOAD_IDLE, dfu.State.DFU_ERROR):
-                        break
-                    # Wait while the device executes flashing
-                    milli_sleep(
-                        DEFAULT_POLLTIMEOUT
-                        if quirks & QUIRK_POLLTIMEOUT
-                        else status.bwPollTimeout
-                    )
-
-                if status.bStatus != dfu.Status.OK:
-                    logger.error("Transfer failed!")
-                    logger.info(f"state({status.bState}) = {status.bState.to_string()}, "
-                                f"status({status.bStatus}) = {status.bStatus.to_string()}")
-                    raise IOError("Downloading failed!")
-
-                progress.update(description="Downloading...", advance=xfer_size//1000)
-
-            # Send one zero-sized download request to signalize end
-            if dif.download(dfu.TRANSACTION, bytes()) < 0:
-                raise IOError("Error sending completion packet")
-
-            progress.update(description="Download finished!")
-            _logger.info("finished!")
-            _logger.debug(f"Sent a total of {bytes_sent} bytes")
-
-            # Transition to MANIFEST_SYNC state
-            if int(status := dif.get_status()) < 0:
-                raise IOError("Unable to read DFU status")
+            progress.update(description="Downloading...", advance=xfer_size // 1000)
+
+        # Send one zero-sized download request to signalize end
+        try:
+            dif.download(dfu.TRANSACTION, bytes())
+        except USBError as e:
+            raise _IOError(f"Error sending completion packet {e}") from e
+
+        progress.update(description="Download finished!")
+        _logger.info("finished!")
+        _logger.debug(f"Sent a total of {bytes_sent} bytes")
+
+        # Transition to MANIFEST_SYNC state
+        try:
+            status = dif.get_status()
+        except USBError as e:
+            raise _IOError(f"Unable to read DFU status: {e}") from e
+        _logger.info(f"state({status.bState}) = {status.bState.to_string()}, "
+                     f"status({status.bStatus}) = {status.bStatus.to_string()}")
+
+        if not dif.quirks & QUIRK.POLLTIMEOUT:
+            milli_sleep(status.bwPollTimeout)
+
+        # Deal correctly with ManifestationTolerant=0 / WillDetach bits
+        while status.bState in (dfu.State.DFU_MANIFEST_SYNC, dfu.State.DFU_MANIFEST):
+            # Some devices need some time before we can obtain the status
+            milli_sleep(1000)
+            try:
+                status = dif.get_status()
+            except USBError as e:
+                raise _IOError(f"Unable to read DFU status: {e}") from e
             _logger.info(f"state({status.bState}) = {status.bState.to_string()}, "
                          f"status({status.bStatus}) = {status.bStatus.to_string()}")
 
-            if not quirks & QUIRK_POLLTIMEOUT:
-                milli_sleep(status.bwPollTimeout)
+        if status.bState == dfu.State.DFU_IDLE:
+            _logger.info("Done!")
+    return bytes_sent
+
 
-            # Deal correctly with ManifestationTolerant=0 / WillDetach bits
-            while status.bState in (dfu.State.DFU_MANIFEST_SYNC, dfu.State.DFU_MANIFEST):
-                # Some devices need some time before we can obtain the status
-                milli_sleep(1000)
-                if int(status := dif.get_status()) < 0:
-                    raise IOError("Unable to read DFU status")
-                _logger.info(f"state({status.bState}) = {status.bState.to_string()}, "
-                             f"status({status.bStatus}) = {status.bStatus.to_string()}")
-
-            if status.bState == dfu.State.DFU_IDLE:
-                _logger.info("Done!")
-        return bytes_sent
-
-    except IOError as err:
-        _logger.error(err)
-        return -1
-
-
-def init() -> None:
-    """Init dfu_load props"""
-    dfu.debug(dfu.DEBUG)
-    dfu.init(dfu.TIMEOUT)
+__all__ = (
+    'do_upload',
+    'do_download'
+)
```

### Comparing `pydfuutil-0.0.5/pydfuutil/dfuse_mem.py` & `pydfuutil-0.11.0b0/pydfuutil/dfuse_mem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 """
 Helper functions for reading the memory map in a device
 following the ST DfuSe 1.1a specification.
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
+
+This program is free software; you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation; either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program; if not, write to the Free Software
+Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 """
 import logging
 import re
 from dataclasses import dataclass, field
 from enum import IntFlag
 from typing import Iterator
 
 from pydfuutil.logger import logger
 
-_logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
+_logger = logger.getChild('dfuse_mem')
 
 
 class DFUSE(IntFlag):
     """DFUSE read/write flags"""
     READABLE = 0x1
     ERASABLE = 0x2
     WRITEABLE = 0x4
@@ -102,18 +116,14 @@
         """
         if self.start <= address <= self.end:
             return self
         if self.next is not None:
             return self.next.find(address)
         return None
 
-    # def free(self) -> None:
-    #     """Useless cause of garbage collector"""
-    #     raise NotImplementedError("Useless cause of garbage collector")
-
 
 def add_segment(segment_stack: [MemSegment, None], segment: MemSegment) -> MemSegment:
     """
     :param segment_stack:
     :param segment:
     :return: 0 if ok
     """
@@ -137,19 +147,14 @@
     :return: MemSegment instance if found, None otherwise.
     """
     if not segment_stack:
         return None
     return segment_stack.find(address)
 
 
-# def free_segment_list(segment_stack: MemSegment) -> None:
-#     """Useless cause of garbage collector"""
-#     raise NotImplementedError("Useless cause of garbage collector")
-
-
 # Parse memory map from interface descriptor string
 # encoded as per ST document UM0424 section 4.3.2.
 
 def parse_memory_layout(intf_desc: [str, bytes], verbose: bool = False) -> [MemSegment, None]:
     """
     Parse memory map from interface descriptor string
     encoded as per ST document UM0424 section 4.3.2.
@@ -232,7 +237,16 @@
 
         _logger.debug(f"Parsed details of {count} segments")
 
     if address is None:
         _logger.error(f"Could not read address, {address=}")
 
     return segment_stack
+
+
+__all__ = (
+    "DFUSE",
+    "MemSegment",
+    "add_segment",
+    "find_segment",
+    "parse_memory_layout"
+)
```

### Comparing `pydfuutil-0.0.5/pydfuutil/progress.py` & `pydfuutil-0.11.0b0/pydfuutil/progress.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,25 @@
-"""Progress bar utilities"""
+"""
+Progress bar utilities
+(C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
+
+This program is free software; you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation; either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program; if not, write to the Free Software
+Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
+"""
 
 
 import sys
 from abc import ABC, abstractmethod
```

### Comparing `pydfuutil-0.0.5/pydfuutil.egg-info/PKG-INFO` & `pydfuutil-0.11.0b0/pydfuutil.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydfuutil
-Version: 0.0.5
+Version: 0.11.0b0
 Summary: PyDfuUtil - Pure python fork of dfu-util wrappers to libusb
 Author-email: o-murphy <thehelixpg@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -185,116 +185,152 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyusb
 Requires-Dist: libusb-package
-Requires-Dist: construct
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Provides-Extra: rich
 Requires-Dist: rich; extra == "rich"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pylint; extra == "test"
 
-# PyDfuUtil - Pure python fork of **[dfu-util](https://github.com/Stefan-Schmidt/dfu-util)** wrappers to **[libusb](https://github.com/libusb/libusb)**
+# PyDfuUtil - Pure python fork of **[dfu-util](https://dfu-util.sourceforge.net/)** wrappers to **[libusb](https://github.com/libusb/libusb)**
 
 [![PyPI Version](https://img.shields.io/pypi/v/pydfuutil?label=PyPI&logo=pypi)](https://pypi.org/project/pydfuutil/)
 
 ## Table of contents
 * **[Introduction](#introduction)**
 * **[Requirements](#requirements-and-platform-support)**
 * **[Installing](#installing)**
+* **[Usage](#installing)**
+  + [**Manual page**](https://dfu-util.sourceforge.net/dfu-util.1.html)
+  + [**dfu-util** (pydfuutil-util)](#pydfuutil)
+  + [**dfu-suffix** (pydfuutil-suffix)](#pydfuutil-suffix)
+  + [**dfu-prefix** (pydfuutil-prefix)](#pydfuutil-prefix)
+  + [**lsusb** (pydfuutil-lsusb)](#pydfuutil-lsusb)
 * **[Todos](#todos)**
 * **[Getting help](#getting-help)**
 * **[About](#about)**
 * **[Footnotes](#footnotes)**
 
 
 ## Introduction
 
 * **PyDFUUtil** provides for easy access to the devices that supports **DFU** interface over host machine's **Universal Serial Bus (USB)**
 system for Python 3.
-* **PyDFUUtil** is an open realisation of original **[dfu-util](https://github.com/Stefan-Schmidt/dfu-util)**
+* **PyDFUUtil** is an open realisation of original **[dfu-util](https://dfu-util.sourceforge.net/)**
 and thin wrapper over **[libusb](https://github.com/libusb/libusb)** _(uses **[PyUsb](https://github.com/pyusb/pyusb)** library as a backend)_.
 
 > [!WARNING]
 > The current status of the project is BETA version.
 > Use it for your own risk
 
+> [!IMPORTANT]
+> Current version implements but not tested with real `dfuse` devices!
+
 > [!TIP]
 > Searching for contributors for testing the library
 
 ## Requirements and platform support
 
 * Since **PyDFUUtil** uses the **[libusb](https://github.com/libusb/libusb)** library it has similar dependencies for using **[libusb](https://github.com/libusb/libusb)**
-* It uses python **[construct](https://github.com/construct/construct)** library for simple unpacking C-structs.
 * **PyDFUUtil** primarily tested on Linux and Windows, 
-but also can work on each platform where **[PyUsb](https://github.com/construct/construct)** and **[construct](https://github.com/construct/construct)** libraries are available, including MacOS
+but also can work on each platform where **[PyUsb](https://github.com/construct/construct)** library are available, including MacOS
 
 
 ## Installing
 
 **PyDFUUtil** is generally installed through pip
 
     # the latest official release
     python -m pip install pydfuutil
 
     # install a specific version (e.g. 0.0.1b1)
     python -m pip install pydfuutil==0.0.1b1
 
 ## Usage
 
-### dfu-util
+### pydfuutil
 ```Bash
 pydfuutil -h 
 # or
 python -m pydfuutil -h
 
 ####### usage:
-usage: pydfuutil [-h] [-V] [-v] [-l] [-e] [-d <deviceID>:<productID>] [-p <bus/port>] [-c <config>] [-i <intf_num>] [-a <alt>] [-t <size>] [-U <file>] [-D <file>] [-R] [-s <address>]
+usage: pydfuutil [-h] [-V] [-v] [-l] [-e] [-E <seconds>]
+                 [-d <vid>:<pid>[,<vid_dfu>:<pid_dfu>]] [-n <dnum>] [-p <bus-port. ... .port>]
+                 [-c <config_nr>] [-i <intf_nr>] [-S <serial_str>[,<serial_str_dfu>]]
+                 [-a <alt>] [-t <size>] [-U <file>] [-Z <bytes>] [-D <file>] [-R] [-w]
+                 [-s <address><:...>]
 
 Python implementation of DFU-Util tools
 
 options:
   -h, --help            show this help message and exit
   -V, --version         Print the version number
   -v, --verbose         Print verbose debug statements
   -l, --list            List the currently attached DFU capable USB devices
   -e, --detach          Detach the currently attached DFU capable USB devices
-  -d <deviceID>:<productID>, --device <deviceID>:<productID>
-                        Specify Vendor/Product ID of DFU device
-  -p <bus/port>, --path <bus/port>
+  -E <seconds>, --detach-delay <seconds>
+                        Time to wait before reopening a device after detach
+  -d <vid>:<pid>[,<vid_dfu>:<pid_dfu>], --device <vid>:<pid>[,<vid_dfu>:<pid_dfu>]
+                        Specify Vendor/Product ID(s) of DFU device
+  -n <dnum>, --devnum <dnum>
+                        Match given device number (devnum from --list)
+  -p <bus-port. ... .port>, --path <bus-port. ... .port>
                         Specify path to DFU device
-  -c <config>, --cfg <config>
+  -c <config_nr>, --cfg <config_nr>
                         Specify the Configuration of DFU device
-  -i <interface>, --intf <interface>
+  -i <intf_nr>, --intf <intf_nr>
                         Specify the DFU Interface number
+  -S <serial_str>[,<serial_str_dfu>], --serial <serial_str>[,<serial_str_dfu>]
+                        Specify Serial String of DFU device
   -a <alt>, --alt <alt>
                         Specify the Altsetting of the DFU Interface
   -t <size>, --transfer-size <size>
                         Specify the number of bytes per USB Transfer
   -U <file>, --upload <file>
                         Read firmware from device into <file>
+  -Z <bytes>, --upload-size <bytes>
+                        Read firmware from device into <file>
   -D <file>, --download <file>
-                        Write firmware from <file> into device
+                        Read firmware from device into <file>
   -R, --reset           Issue USB Reset signalling once we`re finished
-  -s <address>, --dfuse-address <address>
-                        ST DfuSe mode, specify target address for raw file download or upload. Not applicable for DfuSe file (.dfu) downloads
+  -w, --wait            Wait for device to appear
+  -s <address><:...>, --dfuse-address <address><:...>
+                        ST DfuSe mode string, specifying target
+                        address for raw file download or upload
+                        (not applicable for DfuSe file (.dfu) downloads).
+                        Add more DfuSe options separated with ':'
+
+                        leave
+                                Leave DFU mode (jump to application)
+                        mass-erase
+                                Erase the whole device (requires "force")
+                        unprotect
+                                Erase read protected device (requires "force")
+                        will-reset
+                                Expect device to reset (e.g. option bytes write)
+                        force
+                                You really know what you are doing!
+                        <length>
+                                Length of firmware to upload from device
 ```
 
-### dfu-suffix
+### pydfuutil-suffix
 ```Bash
 pydfuutil-suffix -h
 # or 
 python -m pydfuutil.suffix -h
 
-
+####### usage:
 usage: dfu-suffix [-h] [-V] (-c | -a | -D) [-p <productID>] [-v <vendorID>] [-d <deviceID>] [-s <address>] [-T] <file>
 
 positional arguments:
   <file>                Target filename
 
 options:
   -h, --help            Print this help message
@@ -307,32 +343,89 @@
   -v <vendorID>, --vid <vendorID>
                         Add vendor ID into DFU suffix in <file>
   -d <deviceID>, --did <deviceID>
                         Add device ID into DFU suffix in <file>
   -s <address>, --stellaris-address <address>
                         Specify lmdfu address for LMDFU_ADD
   -T, --stellaris       Set lmdfu mode to LMDFU_CHECK
+```
+
+### pydfuutil-prefix
+```Bash
+pydfuutil-prefix -h
+# or 
+python -m pydfuutil.prefix -h
+
+####### usage:
+usage: pydfuutil-prefix [-h] [-V] (-c | -D | -a) [-s <address>] [-T]
+                        [-L]
+                        <file>
+
+
+positional arguments:
+  <file>                Target filename
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         Print the version number
+  -c, --check           Check DFU suffix of <file>
+  -D, --delete          Delete DFU suffix from <file>
+  -a, --add             Add DFU suffix to <file>
+
+In combination with -a:
+  -s <address>, --stellaris-address <address>
+                        Add TI Stellaris address prefix to <file>
+
+In combination with -a or -D or -c:
+  -T, --stellaris       Act on TI Stellaris address prefix of <file>
 
+In combination with -a or -D or -c:
+  -L, --lpc-prefix      Use NXP LPC DFU prefix format
+```
+
+### pydfuutil-lsusb
+```Bash
+pydfuutil-lsusb -h
+# or 
+python -m pydfuutil.lsusb -h
+
+####### usage:
+usage: pydfuutil-prefix [-v] [-s [[bus]:][devnum]]
+                        [-d vendor:[product]] [-D device] [-t] [-V]    
+                        [-h]
+
+options:
+  -v, --verbose        Increase verbosity (show descriptors)
+  -s [[bus]:][devnum]  Show only devices with specified device and/or  
+                       bus numbers (in decimal)
+  -d vendor:[product]  Show only devices with the specified vendor     
+                       and product ID numbers (in hexadecimal)
+  -D device            Selects which device lsusb will examine by      
+                       UNIX-like path simulate
+  -t, --tree           Simulate UNIX-like physical USB device
+                       hierarchy
+  -V, --version        Print the version number
+  -h, --help           Show this help message and exit
 ```
 
 #### Done:
 - [x] dfu
 - [x] dfu_file
 - [x] dfu_load
 - [x] portable
 - [x] quirks
-- [x] suffix + cli entry point
+- [x] suffix
 - [x] usb_dfu
 - [x] lmdfu
 - [x] dfuse_mem
 - [x] dfuse
-- [x] dfu-util cli entry point (not fully supported yet)
+- [x] dfu-util
 
 #### Todo
-- [ ] Update sources to latest original version "dfu-util-0.11"
+- [x] Update sources to latest original version "dfu-util-0.11"
 
 [//]: # (https://dfu-util.sourceforge.net/)
 [//]: # (- https://sourceforge.net/p/dfu-util/dfu-util/ci/master/tree/)
 
 
 ## Getting help
 * To report a bug or propose a new feature, use our issue tracker. But please search the database before opening a new issue.
@@ -349,19 +442,19 @@
 USB. It ranges from small devices like micro-controller boards up to mobile
 phones. With dfu-util you are able to download firmware to your device or
 upload firmware from it.
 
 dfu-util has been tested with Openmoko Neo1973 and Freerunner and many
 other devices.
 
-* **[The official website](http://dfu-util.gnumonks.org)**
+* **[The official website](https://dfu-util.sourceforge.net/)**
 * **[DFU 1.0 spec](http://www.usb.org/developers/devclass_docs/usbdfu10.pdf)**
 * **[DFU 1.1 spec](http://www.usb.org/developers/devclass_docs/DFU_1.1.pdf)**
 
 ## RISK NOTICE
 > [!IMPORTANT]
 > THE CODE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE MATERIALS OR THE USE OR OTHER DEALINGS IN THE MATERIALS.
 
 ## Footnotes
 * On systems that still default to Python 2, replace python with python3
-* Project is in develop, it fulls of not implemented statements that's not according to original **[dfu-util](https://github.com/Stefan-Schmidt/dfu-util)**!
+* Project is in develop, it fulls issues not according to original **[dfu-util](https://github.com/Stefan-Schmidt/dfu-util)**!
```

### Comparing `pydfuutil-0.0.5/pydfuutil.egg-info/SOURCES.txt` & `pydfuutil-0.11.0b0/pydfuutil.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 pyproject.toml
 setup.py
 pydfuutil/__init__.py
 pydfuutil/__main__.py
 pydfuutil/dfu.py
 pydfuutil/dfu_file.py
 pydfuutil/dfu_load.py
+pydfuutil/dfu_util.py
 pydfuutil/dfuse.py
 pydfuutil/dfuse_mem.py
 pydfuutil/exceptions.py
-pydfuutil/lmdfu.py
 pydfuutil/logger.py
+pydfuutil/lsusb.py
 pydfuutil/portable.py
+pydfuutil/prefix.py
 pydfuutil/progress.py
 pydfuutil/quirks.py
 pydfuutil/suffix.py
 pydfuutil/usb_dfu.py
 pydfuutil.egg-info/PKG-INFO
 pydfuutil.egg-info/SOURCES.txt
 pydfuutil.egg-info/dependency_links.txt
 pydfuutil.egg-info/entry_points.txt
 pydfuutil.egg-info/requires.txt
 pydfuutil.egg-info/top_level.txt
 tests/test_dfu.py
 tests/test_dfu_file.py
 tests/test_dfu_load.py
-tests/test_dfuse.py
 tests/test_dfuse_mem.py
-tests/test_lmdfu.py
 tests/test_main.py
 tests/test_progress.py
 tests/test_quirks.py
```

### Comparing `pydfuutil-0.0.5/pyproject.toml` & `pydfuutil-0.11.0b0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pydfuutil"
-version = "0.0.5"
+version = "0.11.0b0"
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
 ]
 description = "PyDfuUtil - Pure python fork of dfu-util wrappers to libusb"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["dfu_util", "dfu-util", "pydfu", "libusb", "python", "python3"]
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
-dependencies = ['pyusb', 'libusb-package', 'construct']
+dependencies = ['pyusb', 'libusb-package']
 
 
 [project.urls]
 "Homepage" = "https://github.com/o-murphy/pydfuutil"
 "Bug Reports" = "https://github.com/o-murphy/pydfuutil/issues"
 "Source" = "https://github.com/o-murphy/pydfuutil"
 
@@ -62,7 +62,9 @@
     "pytest",
     "pylint",
 ]
 
 [project.scripts]
 pydfuutil = "pydfuutil.__main__:main"
 pydfuutil-suffix = "pydfuutil.suffix:main"
+pydfuutil-prefix = "pydfuutil.prefix:main"
+pydfuutil-lsusb = "pydfuutil.lsusb:main"
```

### Comparing `pydfuutil-0.0.5/tests/test_dfu.py` & `pydfuutil-0.11.0b0/tests/test_dfu.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     def setUp(self):
         dfu.init(1000)
 
     def test_init(self):
         self.assertEqual(dfu.TIMEOUT, 1000)
 
     def test_str(self):
-        self.assertEqual(dfu.status_to_string(dfu.Status.OK), "No error condition is present")
+        self.assertEqual(dfu._status_to_string(dfu.Status.OK), "No error condition is present")
         self.assertEqual(dfu.Status.OK.to_string(), "No error condition is present")
-        self.assertEqual(dfu.state_to_string(dfu.State.APP_IDLE), "appIDLE")
+        self.assertEqual(dfu._state_to_string(dfu.State.APP_IDLE), "appIDLE")
         self.assertEqual(dfu.State.APP_IDLE.to_string(), "appIDLE")
 
     @patch("usb.core.find")
     def test_detach(self, mock_find):
         # Mocking the device
         mock_device = MagicMock()
 
@@ -28,20 +28,20 @@
 
         # Mocking the return value of ctrl_transfer method
         mock_device.ctrl_transfer.return_value = 1
 
         # Calling the function
         interface = 0
         timeout = 1000
-        result = dfu.detach(mock_device, interface, timeout)
+        result = dfu._detach(mock_device, interface, timeout)
 
         # Assertions
         mock_device.ctrl_transfer.assert_called_once_with(
             bmRequestType=0x21 | 0x01,
-            bRequest=dfu.Command.DETACH,  # Assuming Command.DETACH is 23
+            bRequest=dfu.Request.DETACH,  # Assuming Request.DETACH is 23
             wValue=timeout,
             wIndex=interface,
             data_or_wLength=None,
             timeout=1000,  # Assuming TIMEOUT is 1000
         )
         self.assertEqual(result, 1)  # Assuming success returns 1
 
@@ -56,20 +56,20 @@
         # Mocking the return value of ctrl_transfer method
         mock_device.ctrl_transfer.return_value = array.array('B', [0] * 10)
 
         # Calling the function
         interface = 0
         transaction = 0
         data = bytes(10)
-        result = dfu.upload(mock_device, interface, transaction, data)
+        result = dfu._upload(mock_device, interface, transaction, data)
 
         # Assertions
         mock_device.ctrl_transfer.assert_called_once_with(
             bmRequestType=0xa1,
-            bRequest=dfu.Command.UPLOAD,  # Assuming Command.UPLOAD
+            bRequest=dfu.Request.UPLOAD,  # Assuming Request.UPLOAD
             wValue=transaction,
             wIndex=interface,
             data_or_wLength=data,
             timeout=1000,  # Assuming TIMEOUT is 1000
         )
         self.assertEqual(result, data)  # Assuming success returns bytes(10)
 
@@ -84,20 +84,20 @@
         # Mocking the return value of ctrl_transfer method
         mock_device.ctrl_transfer.return_value = 10
 
         # Calling the function
         interface = 0
         transaction = 0
         data = bytes(10)
-        result = dfu.download(mock_device, interface, transaction, data)
+        result = dfu._download(mock_device, interface, transaction, data)
 
         # Assertions
         mock_device.ctrl_transfer.assert_called_once_with(
             bmRequestType=0x21,
-            bRequest=dfu.Command.DNLOAD,  # Assuming Command.DNLOAD
+            bRequest=dfu.Request.DNLOAD,  # Assuming Request.DNLOAD
             wValue=transaction,
             wIndex=interface,
             data_or_wLength=data,
             timeout=1000,  # Assuming TIMEOUT is 1000
         )
         self.assertEqual(result, len(data))  # Assuming success returns 10
 
@@ -112,20 +112,20 @@
         # Mocking the return value of ctrl_transfer method
         mock_device.ctrl_transfer.return_value = array.array('B', [0] * 6)
 
         # Calling the function
         interface = 0
         transaction = 0
         length = 6
-        status = dfu.get_status(mock_device, interface)
+        status = dfu._get_status(mock_device, interface)
 
         # Assertions
         mock_device.ctrl_transfer.assert_called_once_with(
             bmRequestType=0xa1,
-            bRequest=dfu.Command.GETSTATUS,  # Assuming Command.GETSTATUS
+            bRequest=dfu.Request.GETSTATUS,  # Assuming Request.GETSTATUS
             wValue=transaction,
             wIndex=interface,
             data_or_wLength=length,
             timeout=1000,  # Assuming TIMEOUT is 1000
         )
         self.assertEqual(status.bState, 0)  # Assuming success returns 0
 
@@ -139,20 +139,20 @@
 
         # Mocking the return value of ctrl_transfer method
         mock_device.ctrl_transfer.return_value = 0
 
         # Calling the function
         interface = 0
         transaction = 0
-        result = dfu.clear_status(mock_device, interface)
+        result = dfu._clear_status(mock_device, interface)
 
         # Assertions
         mock_device.ctrl_transfer.assert_called_once_with(
             bmRequestType=0x21,
-            bRequest=dfu.Command.CLRSTATUS,  # Assuming Command.CLRSTATUS
+            bRequest=dfu.Request.CLRSTATUS,  # Assuming Request.CLRSTATUS
             wValue=transaction,
             wIndex=interface,
             data_or_wLength=None,
             timeout=1000,  # Assuming TIMEOUT is 1000
         )
         self.assertEqual(result, 0)  # Assuming success returns 0
 
@@ -166,20 +166,20 @@
 
         # Mocking the return value of ctrl_transfer method
         mock_device.ctrl_transfer.return_value = 0
 
         # Calling the function
         interface = 0
         transaction = 0
-        result = dfu.abort(mock_device, interface)
+        result = dfu._abort(mock_device, interface)
 
         # Assertions
         mock_device.ctrl_transfer.assert_called_once_with(
             bmRequestType=0x21,
-            bRequest=dfu.Command.ABORT,  # Assuming Command.ABORT
+            bRequest=dfu.Request.ABORT,  # Assuming Request.ABORT
             wValue=transaction,
             wIndex=interface,
             data_or_wLength=None,
             timeout=1000,  # Assuming TIMEOUT is 1000
         )
         self.assertEqual(result, 0)  # Assuming success returns 0
```

### Comparing `pydfuutil-0.0.5/tests/test_dfu_load.py` & `pydfuutil-0.11.0b0/tests/test_dfu_load.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import unittest
-from unittest.mock import Mock, patch
+from unittest.mock import Mock, patch, MagicMock
 
 from pydfuutil import dfu
-from pydfuutil.dfu_load import DFUFile, do_upload, do_dnload
+from pydfuutil.dfu_load import DfuFile, do_upload, do_download
 
 
 class TestDFULoader(unittest.TestCase):
 
     def test_dfu_load_do_upload(self):
         xfer_size = 256
-        file = DFUFile(name='test_file', file_p=Mock())  # Provide a mock file object
+        file = DfuFile(name='test_file', file_p=Mock())  # Provide a mock file object
         total_size = 4096
 
         dif = Mock()
         dif.upload.return_value = bytes(xfer_size)
         dif.get_status.return_value = total_size
 
         # Mock file_p.write to return the length of the data written
@@ -24,24 +24,26 @@
         self.assertEqual(result, total_size)  # Assuming expected_size bytes are received
 
     def test_dfu_load_do_dnload(self):
 
         xfer_size = 1024
         result = dfu.StatusRetVal(dfu.Status.OK, 100, dfu.State.DFU_DOWNLOAD_IDLE, 0)
 
-        dif = Mock()
+        dif = Mock(spec_set=dfu.DfuIf)
         dif.download.return_value = xfer_size
         dif.get_status.return_value = result
 
-        file = DFUFile(name='test_file', file_p=Mock(), size=xfer_size, suffix_len=0)
-        quirks = 0
+        file = DfuFile(name='test_file', file_p=Mock())
+        file.size.total = xfer_size * 10
+        file.size.suffix = 0
+        dif.quirks = 0
 
         # Mock file_p.readinto to return the length of the data read
         with patch.object(file.file_p, 'readinto', return_value=xfer_size) as mock_readinto:
-            result = do_dnload(dif, xfer_size, file, quirks)
+            result = do_download(dif, xfer_size, file)
 
         # Assertions
-        self.assertEqual(result, xfer_size)  # Assuming xfer_size bytes are sent
+        self.assertEqual(result, file.size.total)  # Assuming xfer_size bytes are sent
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pydfuutil-0.0.5/tests/test_dfuse_mem.py` & `pydfuutil-0.11.0b0/tests/test_dfuse_mem.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.5/tests/test_progress.py` & `pydfuutil-0.11.0b0/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.5/tests/test_quirks.py` & `pydfuutil-0.11.0b0/tests/test_quirks.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 logger.setLevel(logging.DEBUG)
 
 
 class TestSetQuirks(unittest.TestCase):
 
     def test_quirk_polltimeout(self):
-        self.assertEqual(set_quirks(VENDOR_OPENMOKO, 123, 1), QUIRK_POLLTIMEOUT)
-        self.assertEqual(set_quirks(VENDOR_FIC, 456, 1), QUIRK_POLLTIMEOUT)
-        self.assertEqual(set_quirks(VENDOR_VOTI, 789, 1), QUIRK_POLLTIMEOUT)
+        self.assertEqual(get_quirks(VENDOR.OPENMOKO, PRODUCT.FREERUNNER_FIRST , 1), QUIRK.POLLTIMEOUT)
+        self.assertEqual(get_quirks(VENDOR.FIC, PRODUCT.FREERUNNER_LAST, 1), QUIRK.POLLTIMEOUT)
+        self.assertEqual(get_quirks(VENDOR.VOTI, PRODUCT.OPENPCD, 1), QUIRK.POLLTIMEOUT)
 
     def test_quirk_force_dfu11(self):
-        self.assertEqual(set_quirks(VENDOR_LEAFLABS, PRODUCT_MAPLE3, 0x0200), QUIRK_FORCE_DFU11)
-        self.assertEqual(set_quirks(VENDOR_LEAFLABS, PRODUCT_MAPLE3, 0x0100), 0)
-        self.assertEqual(set_quirks(VENDOR_LEAFLABS, 123, 0x0200), 0)
-        self.assertEqual(set_quirks(VENDOR_LEAFLABS, PRODUCT_MAPLE3, 0x0300), 0)
+        self.assertEqual(get_quirks(VENDOR.LEAFLABS, PRODUCT.MAPLE3, 0x0200), QUIRK.FORCE_DFU11)
+        self.assertEqual(get_quirks(VENDOR.LEAFLABS, PRODUCT.MAPLE3, 0x0100), 0)
+        self.assertEqual(get_quirks(VENDOR.LEAFLABS, PRODUCT.MAPLE3, 0x0200), QUIRK.FORCE_DFU11)
+        self.assertEqual(get_quirks(VENDOR.LEAFLABS, PRODUCT.MAPLE3, 0x0300), 0)
 
 if __name__ == '__main__':
     unittest.main()
```

