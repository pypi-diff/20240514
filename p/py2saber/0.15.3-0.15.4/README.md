# Comparing `tmp/py2saber-0.15.3.tar.gz` & `tmp/py2saber-0.15.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2saber-0.15.3.tar", last modified: Mon May 13 17:00:57 2024, max compression
+gzip compressed data, was "py2saber-0.15.4.tar", last modified: Mon May 13 18:46:20 2024, max compression
```

## Comparing `py2saber-0.15.3.tar` & `py2saber-0.15.4.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 17:00:57.644857 py2saber-0.15.3/
--rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.15.3/COPYING
--rw-r--r--   0 jramboz    (501) staff       (20)       36 2024-05-13 16:57:53.000000 py2saber-0.15.3/MANIFEST.in
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 17:00:57.642950 py2saber-0.15.3/OpenCore_OEM/
--rw-r--r--   0 jramboz    (501) staff       (20)    12004 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/BEEP.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88656 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_10_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_1_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_2_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_3_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_4_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_5_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_6_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_7_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_8_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_9_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/HUM_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/POWEROFF_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/POWERON_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWING.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 17:00:57.644632 py2saber-0.15.3/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.15.3/README.md
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 17:00:57.643081 py2saber-0.15.3/dist/
--rwxr-xr-x   0 jramboz    (501) staff       (20)    20380 2023-07-23 18:03:06.000000 py2saber-0.15.3/dist/pycodesign.py
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 17:00:57.644358 py2saber-0.15.3/py2saber.egg-info/
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 17:00:57.000000 py2saber-0.15.3/py2saber.egg-info/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)     1213 2024-05-13 17:00:57.000000 py2saber-0.15.3/py2saber.egg-info/SOURCES.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-13 17:00:57.000000 py2saber-0.15.3/py2saber.egg-info/dependency_links.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-13 17:00:57.000000 py2saber-0.15.3/py2saber.egg-info/entry_points.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-13 17:00:57.000000 py2saber-0.15.3/py2saber.egg-info/requires.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       13 2024-05-13 17:00:57.000000 py2saber-0.15.3/py2saber.egg-info/top_level.txt
--rw-r--r--   0 jramboz    (501) staff       (20)    30549 2024-05-13 16:59:40.000000 py2saber-0.15.3/py2saber.py
--rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-05-13 16:59:40.000000 py2saber-0.15.3/pyproject.toml
--rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-13 17:00:57.644890 py2saber-0.15.3/setup.cfg
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 18:46:20.427146 py2saber-0.15.4/
+-rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.15.4/COPYING
+-rw-r--r--   0 jramboz    (501) staff       (20)       35 2024-05-13 18:09:11.000000 py2saber-0.15.4/MANIFEST.in
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 18:46:20.426910 py2saber-0.15.4/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.15.4/README.md
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 18:46:20.410412 py2saber-0.15.4/py2saber/
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 18:46:20.426368 py2saber-0.15.4/py2saber/OpenCore_OEM/
+-rw-r--r--   0 jramboz    (501) staff       (20)    12004 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/BEEP.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88656 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_10_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_1_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_2_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_3_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_4_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_5_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_6_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_7_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_8_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_9_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/HUM_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/POWEROFF_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/POWERON_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWING.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)      239 2024-05-13 18:45:52.000000 py2saber-0.15.4/py2saber/__init__.py
+-rw-r--r--   0 jramboz    (501) staff       (20)       68 2024-03-20 15:23:40.000000 py2saber-0.15.4/py2saber/__main__.py
+-rw-r--r--   0 jramboz    (501) staff       (20)    30549 2024-05-13 18:45:52.000000 py2saber-0.15.4/py2saber/py2saber.py
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 18:46:20.426619 py2saber-0.15.4/py2saber.egg-info/
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 18:46:20.000000 py2saber-0.15.4/py2saber.egg-info/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     1524 2024-05-13 18:46:20.000000 py2saber-0.15.4/py2saber.egg-info/SOURCES.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-13 18:46:20.000000 py2saber-0.15.4/py2saber.egg-info/dependency_links.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-13 18:46:20.000000 py2saber-0.15.4/py2saber.egg-info/entry_points.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-13 18:46:20.000000 py2saber-0.15.4/py2saber.egg-info/requires.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        9 2024-05-13 18:46:20.000000 py2saber-0.15.4/py2saber.egg-info/top_level.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-05-13 18:45:52.000000 py2saber-0.15.4/pyproject.toml
+-rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-13 18:46:20.427184 py2saber-0.15.4/setup.cfg
```

### Comparing `py2saber-0.15.3/COPYING` & `py2saber-0.15.4/COPYING`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/BEEP.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/BEEP.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/CLASH_10_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_10_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/CLASH_1_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_1_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/CLASH_2_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_2_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/CLASH_3_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_3_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/CLASH_4_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_4_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/CLASH_5_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_5_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/CLASH_6_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_6_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/CLASH_7_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_7_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/CLASH_8_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_8_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/CLASH_9_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/CLASH_9_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/HUM_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/HUM_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/POWEROFF_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/POWEROFF_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/POWERON_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/POWERON_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWING.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWING.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW` & `py2saber-0.15.4/py2saber/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/PKG-INFO` & `py2saber-0.15.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.15.3
+Version: 0.15.4
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,15 +680,15 @@
         
 Project-URL: Homepage, https://github.com/jramboz/py2saber
 Keywords: polaris,ludosport,lightsabers,opencore
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: pyserial>=3.5
 Requires-Dist: py-getch
 
 # py2saber
 `py2saber` is a Python library and command-line utility for working with [OpenCore](https://github.com/LamaDiLuce/polaris-opencore)-based lightsabers. It is a re-implementation of [Ian "Nuntis" Jukes](http://sabers.amazer.uk/) excellent [sendtosaber](https://github.com/Nuntis-Spayz/Send-To-Saber) program, and extends on Nuntis' work in several ways:
```

### Comparing `py2saber-0.15.3/README.md` & `py2saber-0.15.4/README.md`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.3/py2saber.egg-info/PKG-INFO` & `py2saber-0.15.4/py2saber.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.15.3
+Version: 0.15.4
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,15 +680,15 @@
         
 Project-URL: Homepage, https://github.com/jramboz/py2saber
 Keywords: polaris,ludosport,lightsabers,opencore
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: pyserial>=3.5
 Requires-Dist: py-getch
 
 # py2saber
 `py2saber` is a Python library and command-line utility for working with [OpenCore](https://github.com/LamaDiLuce/polaris-opencore)-based lightsabers. It is a re-implementation of [Ian "Nuntis" Jukes](http://sabers.amazer.uk/) excellent [sendtosaber](https://github.com/Nuntis-Spayz/Send-To-Saber) program, and extends on Nuntis' work in several ways:
```

### Comparing `py2saber-0.15.3/py2saber.egg-info/SOURCES.txt` & `py2saber-0.15.4/py2saber.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 COPYING
 MANIFEST.in
 README.md
-py2saber.py
 pyproject.toml
-OpenCore_OEM/BEEP.RAW
-OpenCore_OEM/CLASH_10_0.RAW
-OpenCore_OEM/CLASH_1_0.RAW
-OpenCore_OEM/CLASH_2_0.RAW
-OpenCore_OEM/CLASH_3_0.RAW
-OpenCore_OEM/CLASH_4_0.RAW
-OpenCore_OEM/CLASH_5_0.RAW
-OpenCore_OEM/CLASH_6_0.RAW
-OpenCore_OEM/CLASH_7_0.RAW
-OpenCore_OEM/CLASH_8_0.RAW
-OpenCore_OEM/CLASH_9_0.RAW
-OpenCore_OEM/HUM_0.RAW
-OpenCore_OEM/POWEROFF_0.RAW
-OpenCore_OEM/POWERON_0.RAW
-OpenCore_OEM/SMOOTHSWING.RAW
-OpenCore_OEM/SMOOTHSWINGH_1_0.RAW
-OpenCore_OEM/SMOOTHSWINGH_2_0.RAW
-OpenCore_OEM/SMOOTHSWINGH_3_0.RAW
-OpenCore_OEM/SMOOTHSWINGH_4_0.RAW
-OpenCore_OEM/SMOOTHSWINGH_5_0.RAW
-OpenCore_OEM/SMOOTHSWINGH_6_0.RAW
-OpenCore_OEM/SMOOTHSWINGH_7_0.RAW
-OpenCore_OEM/SMOOTHSWINGH_8_0.RAW
-OpenCore_OEM/SMOOTHSWINGL_1_0.RAW
-OpenCore_OEM/SMOOTHSWINGL_2_0.RAW
-OpenCore_OEM/SMOOTHSWINGL_3_0.RAW
-OpenCore_OEM/SMOOTHSWINGL_4_0.RAW
-OpenCore_OEM/SMOOTHSWINGL_5_0.RAW
-OpenCore_OEM/SMOOTHSWINGL_6_0.RAW
-OpenCore_OEM/SMOOTHSWINGL_7_0.RAW
-OpenCore_OEM/SMOOTHSWINGL_8_0.RAW
-dist/pycodesign.py
+py2saber/__init__.py
+py2saber/__main__.py
+py2saber/py2saber.py
 py2saber.egg-info/PKG-INFO
 py2saber.egg-info/SOURCES.txt
 py2saber.egg-info/dependency_links.txt
 py2saber.egg-info/entry_points.txt
 py2saber.egg-info/requires.txt
-py2saber.egg-info/top_level.txt
+py2saber.egg-info/top_level.txt
+py2saber/OpenCore_OEM/BEEP.RAW
+py2saber/OpenCore_OEM/CLASH_10_0.RAW
+py2saber/OpenCore_OEM/CLASH_1_0.RAW
+py2saber/OpenCore_OEM/CLASH_2_0.RAW
+py2saber/OpenCore_OEM/CLASH_3_0.RAW
+py2saber/OpenCore_OEM/CLASH_4_0.RAW
+py2saber/OpenCore_OEM/CLASH_5_0.RAW
+py2saber/OpenCore_OEM/CLASH_6_0.RAW
+py2saber/OpenCore_OEM/CLASH_7_0.RAW
+py2saber/OpenCore_OEM/CLASH_8_0.RAW
+py2saber/OpenCore_OEM/CLASH_9_0.RAW
+py2saber/OpenCore_OEM/HUM_0.RAW
+py2saber/OpenCore_OEM/POWEROFF_0.RAW
+py2saber/OpenCore_OEM/POWERON_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWING.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW
+py2saber/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW
```

### Comparing `py2saber-0.15.3/py2saber.py` & `py2saber-0.15.4/py2saber/py2saber.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import errno
 from getch import pause_exit
 import glob
 import time
 
 basedir = os.path.dirname(os.path.realpath(__file__))
 
-script_version = '0.15.3'
+script_version = '0.15.4'
 script_authors = 'Jason Ramboz'
 script_repo = 'https://github.com/jramboz/py2saber'
 
 # adapted from https://stackoverflow.com/a/66491013
 class DocDefaultException(Exception):
     """Subclass exceptions use docstring as default message"""
     def __init__(self, msg=None, *args, **kwargs):
```

### Comparing `py2saber-0.15.3/pyproject.toml` & `py2saber-0.15.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py2saber"
-version = "0.15.3"
+version = "0.15.4"
 description = "Python-based utility for OpenCore lightsabers"
 readme = "README.md"
 authors = [{name = "Jason Ramboz", email = "jramboz@gmail.com"}]
 license = {file = "COPYING"}
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
@@ -16,14 +16,14 @@
     "Development Status :: 4 - Beta",
 ]
 keywords = ["polaris", "ludosport", "lightsabers", "opencore"]
 dependencies = [
     "pyserial >= 3.5",
     "py-getch"
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/jramboz/py2saber"
 
 [project.scripts]
 py2saber = "py2saber:main_func"
```

