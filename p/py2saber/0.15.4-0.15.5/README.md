# Comparing `tmp/py2saber-0.15.4.tar.gz` & `tmp/py2saber-0.15.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2saber-0.15.4.tar", last modified: Mon May 13 18:46:20 2024, max compression
+gzip compressed data, was "py2saber-0.15.5.tar", last modified: Tue May 14 14:52:36 2024, max compression
```

## Comparing `py2saber-0.15.4.tar` & `py2saber-0.15.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 18:46:20.427146 py2saber-0.15.4/
--rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.15.4/COPYING
--rw-r--r--   0 jramboz    (501) staff       (20)       35 2024-05-13 18:09:11.000000 py2saber-0.15.4/MANIFEST.in
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 18:46:20.426910 py2saber-0.15.4/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.15.4/README.md
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 18:46:20.410412 py2saber-0.15.4/py2saber/
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 18:46:20.426368 py2saber-0.15.4/py2saber/OpenCore_OEM/
--rw-r--r--   0 jramboz    (501) staff       (20)    12004 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/BEEP.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88656 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_10_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_1_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_2_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_3_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_4_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_5_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_6_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_7_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_8_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_9_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/HUM_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/POWEROFF_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/POWERON_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWING.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)      239 2024-05-13 18:45:52.000000 py2saber-0.15.4/py2saber/__init__.py
--rw-r--r--   0 jramboz    (501) staff       (20)       68 2024-03-20 15:23:40.000000 py2saber-0.15.4/py2saber/__main__.py
--rw-r--r--   0 jramboz    (501) staff       (20)    30549 2024-05-13 18:45:52.000000 py2saber-0.15.4/py2saber/py2saber.py
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 18:46:20.426619 py2saber-0.15.4/py2saber.egg-info/
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 18:46:20.000000 py2saber-0.15.4/py2saber.egg-info/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)     1524 2024-05-13 18:46:20.000000 py2saber-0.15.4/py2saber.egg-info/SOURCES.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-13 18:46:20.000000 py2saber-0.15.4/py2saber.egg-info/dependency_links.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-13 18:46:20.000000 py2saber-0.15.4/py2saber.egg-info/entry_points.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-13 18:46:20.000000 py2saber-0.15.4/py2saber.egg-info/requires.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        9 2024-05-13 18:46:20.000000 py2saber-0.15.4/py2saber.egg-info/top_level.txt
--rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-05-13 18:45:52.000000 py2saber-0.15.4/pyproject.toml
--rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-13 18:46:20.427184 py2saber-0.15.4/setup.cfg
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-14 14:52:36.908859 py2saber-0.15.5/
+-rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.15.5/COPYING
+-rw-r--r--   0 jramboz    (501) staff       (20)       35 2024-05-13 18:09:11.000000 py2saber-0.15.5/MANIFEST.in
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-14 14:52:36.908619 py2saber-0.15.5/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.15.5/README.md
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-14 14:52:36.890857 py2saber-0.15.5/py2saber/
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-14 14:52:36.907935 py2saber-0.15.5/py2saber/OpenCore_OEM/
+-rw-r--r--   0 jramboz    (501) staff       (20)    12004 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/BEEP.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88656 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_10_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_1_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_2_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_3_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_4_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_5_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_6_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_7_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_8_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_9_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/HUM_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/POWEROFF_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/POWERON_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWING.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)      239 2024-05-14 14:51:35.000000 py2saber-0.15.5/py2saber/__init__.py
+-rw-r--r--   0 jramboz    (501) staff       (20)       77 2024-05-14 14:49:39.000000 py2saber-0.15.5/py2saber/__main__.py
+-rw-r--r--   0 jramboz    (501) staff       (20)    30549 2024-05-14 14:51:35.000000 py2saber-0.15.5/py2saber/py2saber.py
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-14 14:52:36.908252 py2saber-0.15.5/py2saber.egg-info/
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-14 14:52:36.000000 py2saber-0.15.5/py2saber.egg-info/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     1524 2024-05-14 14:52:36.000000 py2saber-0.15.5/py2saber.egg-info/SOURCES.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-14 14:52:36.000000 py2saber-0.15.5/py2saber.egg-info/dependency_links.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-14 14:52:36.000000 py2saber-0.15.5/py2saber.egg-info/entry_points.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-14 14:52:36.000000 py2saber-0.15.5/py2saber.egg-info/requires.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        9 2024-05-14 14:52:36.000000 py2saber-0.15.5/py2saber.egg-info/top_level.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-05-14 14:51:35.000000 py2saber-0.15.5/pyproject.toml
+-rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-14 14:52:36.908896 py2saber-0.15.5/setup.cfg
```

### Comparing `py2saber-0.15.4/COPYING` & `py2saber-0.15.5/COPYING`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/PKG-INFO` & `py2saber-0.15.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.15.4
+Version: 0.15.5
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.15.4/README.md` & `py2saber-0.15.5/README.md`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/BEEP.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/BEEP.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_10_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_10_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_1_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_1_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_2_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_2_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_3_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_3_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_4_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_4_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_5_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_5_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_6_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_6_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_7_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_7_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_8_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_8_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_9_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/CLASH_9_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/HUM_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/HUM_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/POWEROFF_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/POWEROFF_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/POWERON_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/POWERON_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWING.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWING.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW` & `py2saber-0.15.5/py2saber/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/py2saber/py2saber.py` & `py2saber-0.15.5/py2saber/py2saber.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import errno
 from getch import pause_exit
 import glob
 import time
 
 basedir = os.path.dirname(os.path.realpath(__file__))
 
-script_version = '0.15.4'
+script_version = '0.15.5'
 script_authors = 'Jason Ramboz'
 script_repo = 'https://github.com/jramboz/py2saber'
 
 # adapted from https://stackoverflow.com/a/66491013
 class DocDefaultException(Exception):
     """Subclass exceptions use docstring as default message"""
     def __init__(self, msg=None, *args, **kwargs):
```

### Comparing `py2saber-0.15.4/py2saber.egg-info/PKG-INFO` & `py2saber-0.15.5/py2saber.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.15.4
+Version: 0.15.5
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.15.4/py2saber.egg-info/SOURCES.txt` & `py2saber-0.15.5/py2saber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.4/pyproject.toml` & `py2saber-0.15.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py2saber"
-version = "0.15.4"
+version = "0.15.5"
 description = "Python-based utility for OpenCore lightsabers"
 readme = "README.md"
 authors = [{name = "Jason Ramboz", email = "jramboz@gmail.com"}]
 license = {file = "COPYING"}
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

