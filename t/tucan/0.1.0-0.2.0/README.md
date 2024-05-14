# Comparing `tmp/tucan-0.1.0.tar.gz` & `tmp/tucan-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tucan-0.1.0.tar", last modified: Thu Feb  1 12:05:28 2024, max compression
+gzip compressed data, was "tucan-0.2.0.tar", last modified: Tue May 14 10:48:28 2024, max compression
```

## Comparing `tucan-0.1.0.tar` & `tucan-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2024-02-01 12:05:28.238732 tucan-0.1.0/
--rw-r--r--   0 dauptain   (502) staff       (20)     1060 2023-11-20 20:39:47.000000 tucan-0.1.0/LICENSE.txt
--rw-r--r--   0 dauptain   (502) staff       (20)       95 2023-11-20 20:39:47.000000 tucan-0.1.0/MANIFEST.in
--rw-r--r--   0 dauptain   (502) staff       (20)     5733 2024-02-01 12:05:28.238915 tucan-0.1.0/PKG-INFO
--rw-r--r--   0 dauptain   (502) staff       (20)     4922 2024-02-01 08:37:10.000000 tucan-0.1.0/README.md
--rw-r--r--   0 dauptain   (502) staff       (20)     1082 2024-02-01 12:05:28.239712 tucan-0.1.0/setup.cfg
--rw-r--r--   0 dauptain   (502) staff       (20)       38 2023-11-20 20:39:47.000000 tucan-0.1.0/setup.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2024-02-01 12:05:28.210772 tucan-0.1.0/src/
--rw-r--r--   0 dauptain   (502) staff       (20)     6148 2023-11-21 13:57:09.000000 tucan-0.1.0/src/.DS_Store
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2024-02-01 12:05:28.223405 tucan-0.1.0/src/tucan/
--rw-r--r--   0 dauptain   (502) staff       (20)       42 2024-02-01 12:05:23.000000 tucan-0.1.0/src/tucan/__init__.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2024-02-01 12:05:28.238217 tucan-0.1.0/src/tucan/__pycache__/
--rw-r--r--   0 dauptain   (502) staff       (20)      218 2023-11-20 21:06:04.000000 tucan-0.1.0/src/tucan/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     7342 2024-02-01 08:23:35.000000 tucan-0.1.0/src/tucan/__pycache__/clean_ifdef.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    16987 2024-02-01 08:27:38.000000 tucan-0.1.0/src/tucan/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     2441 2024-01-18 09:05:54.000000 tucan-0.1.0/src/tucan/__pycache__/imports_ftn.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     2743 2024-01-18 09:05:54.000000 tucan-0.1.0/src/tucan/__pycache__/imports_main.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     3947 2024-01-18 09:05:54.000000 tucan-0.1.0/src/tucan/__pycache__/imports_py.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     9433 2024-01-31 17:40:27.000000 tucan-0.1.0/src/tucan/__pycache__/kw_lang.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     7418 2024-01-31 17:56:56.000000 tucan-0.1.0/src/tucan/__pycache__/package_analysis.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     5642 2024-01-31 17:40:27.000000 tucan-0.1.0/src/tucan/__pycache__/struct_c.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    12941 2024-01-26 12:33:29.000000 tucan-0.1.0/src/tucan/__pycache__/struct_common.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     8292 2024-01-29 15:34:09.000000 tucan-0.1.0/src/tucan/__pycache__/struct_ftn.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     3911 2024-01-03 03:13:04.000000 tucan-0.1.0/src/tucan/__pycache__/struct_main.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     6597 2024-01-31 17:40:27.000000 tucan-0.1.0/src/tucan/__pycache__/struct_py.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     7442 2024-01-31 17:40:27.000000 tucan-0.1.0/src/tucan/__pycache__/unformat_c.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    10897 2024-01-25 15:28:39.000000 tucan-0.1.0/src/tucan/__pycache__/unformat_common.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    20955 2024-01-29 15:34:09.000000 tucan-0.1.0/src/tucan/__pycache__/unformat_ftn.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     2545 2024-01-03 03:25:28.000000 tucan-0.1.0/src/tucan/__pycache__/unformat_main.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     7251 2024-01-31 17:40:27.000000 tucan-0.1.0/src/tucan/__pycache__/unformat_py.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     5074 2024-02-01 08:23:12.000000 tucan-0.1.0/src/tucan/clean_ifdef.py
--rw-r--r--   0 dauptain   (502) staff       (20)    13194 2024-02-01 08:27:33.000000 tucan-0.1.0/src/tucan/cli.py
--rw-r--r--   0 dauptain   (502) staff       (20)      763 2023-12-27 08:38:53.000000 tucan-0.1.0/src/tucan/imports_common.py
--rw-r--r--   0 dauptain   (502) staff       (20)     1667 2023-12-27 08:38:53.000000 tucan-0.1.0/src/tucan/imports_ftn.py
--rw-r--r--   0 dauptain   (502) staff       (20)     1327 2023-12-27 08:38:53.000000 tucan-0.1.0/src/tucan/imports_main.py
--rw-r--r--   0 dauptain   (502) staff       (20)     2840 2023-12-27 08:38:53.000000 tucan-0.1.0/src/tucan/imports_py.py
--rw-r--r--   0 dauptain   (502) staff       (20)     8948 2024-01-29 15:40:08.000000 tucan-0.1.0/src/tucan/kw_lang.py
--rw-r--r--   0 dauptain   (502) staff       (20)     4696 2024-01-31 17:56:28.000000 tucan-0.1.0/src/tucan/package_analysis.py
--rw-r--r--   0 dauptain   (502) staff       (20)     4276 2024-01-29 15:41:07.000000 tucan-0.1.0/src/tucan/struct_c.py
--rw-r--r--   0 dauptain   (502) staff       (20)     9078 2024-01-26 12:33:27.000000 tucan-0.1.0/src/tucan/struct_common.py
--rw-r--r--   0 dauptain   (502) staff       (20)     5795 2024-01-26 13:59:47.000000 tucan-0.1.0/src/tucan/struct_ftn.py
--rw-r--r--   0 dauptain   (502) staff       (20)     2407 2024-01-03 02:40:39.000000 tucan-0.1.0/src/tucan/struct_main.py
--rw-r--r--   0 dauptain   (502) staff       (20)     4513 2024-01-29 15:37:08.000000 tucan-0.1.0/src/tucan/struct_py.py
--rw-r--r--   0 dauptain   (502) staff       (20)     4962 2024-01-29 15:42:36.000000 tucan-0.1.0/src/tucan/unformat_c.py
--rw-r--r--   0 dauptain   (502) staff       (20)     6839 2024-01-25 15:24:35.000000 tucan-0.1.0/src/tucan/unformat_common.py
--rw-r--r--   0 dauptain   (502) staff       (20)    15668 2024-01-26 13:59:55.000000 tucan-0.1.0/src/tucan/unformat_ftn.py
--rw-r--r--   0 dauptain   (502) staff       (20)     1184 2024-01-03 02:39:34.000000 tucan-0.1.0/src/tucan/unformat_main.py
--rw-r--r--   0 dauptain   (502) staff       (20)     5771 2024-01-29 15:37:37.000000 tucan-0.1.0/src/tucan/unformat_py.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2024-02-01 12:05:28.226593 tucan-0.1.0/src/tucan.egg-info/
--rw-r--r--   0 dauptain   (502) staff       (20)     5733 2024-02-01 12:05:28.000000 tucan-0.1.0/src/tucan.egg-info/PKG-INFO
--rw-r--r--   0 dauptain   (502) staff       (20)     1628 2024-02-01 12:05:28.000000 tucan-0.1.0/src/tucan.egg-info/SOURCES.txt
--rw-r--r--   0 dauptain   (502) staff       (20)        1 2024-02-01 12:05:28.000000 tucan-0.1.0/src/tucan.egg-info/dependency_links.txt
--rw-r--r--   0 dauptain   (502) staff       (20)       41 2024-02-01 12:05:28.000000 tucan-0.1.0/src/tucan.egg-info/entry_points.txt
--rw-r--r--   0 dauptain   (502) staff       (20)       83 2024-02-01 12:05:28.000000 tucan-0.1.0/src/tucan.egg-info/requires.txt
--rw-r--r--   0 dauptain   (502) staff       (20)        6 2024-02-01 12:05:28.000000 tucan-0.1.0/src/tucan.egg-info/top_level.txt
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2024-05-14 10:48:28.542808 tucan-0.2.0/
+-rw-r--r--   0 dauptain   (502) staff       (20)     1060 2023-11-20 20:39:47.000000 tucan-0.2.0/LICENSE.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)       95 2023-11-20 20:39:47.000000 tucan-0.2.0/MANIFEST.in
+-rw-r--r--   0 dauptain   (502) staff       (20)     7749 2024-05-14 10:48:28.542885 tucan-0.2.0/PKG-INFO
+-rw-r--r--   0 dauptain   (502) staff       (20)     6938 2024-02-01 12:26:27.000000 tucan-0.2.0/README.md
+-rw-r--r--   0 dauptain   (502) staff       (20)     1082 2024-05-14 10:48:28.543465 tucan-0.2.0/setup.cfg
+-rw-r--r--   0 dauptain   (502) staff       (20)       38 2023-11-20 20:39:47.000000 tucan-0.2.0/setup.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2024-05-14 10:48:28.517266 tucan-0.2.0/src/
+-rw-r--r--   0 dauptain   (502) staff       (20)     6148 2024-04-25 14:34:03.000000 tucan-0.2.0/src/.DS_Store
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2024-05-14 10:48:28.528799 tucan-0.2.0/src/tucan/
+-rw-r--r--   0 dauptain   (502) staff       (20)       42 2024-05-14 10:46:14.000000 tucan-0.2.0/src/tucan/__init__.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2024-05-14 10:48:28.542365 tucan-0.2.0/src/tucan/__pycache__/
+-rw-r--r--   0 dauptain   (502) staff       (20)      218 2024-02-01 12:15:12.000000 tucan-0.2.0/src/tucan/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    14440 2024-05-13 14:36:41.000000 tucan-0.2.0/src/tucan/__pycache__/clean_ifdef.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    17543 2024-05-13 14:36:41.000000 tucan-0.2.0/src/tucan/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1323 2024-02-29 17:00:28.000000 tucan-0.2.0/src/tucan/__pycache__/imports_c.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     2441 2024-01-18 09:05:54.000000 tucan-0.2.0/src/tucan/__pycache__/imports_ftn.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     3183 2024-02-29 17:00:28.000000 tucan-0.2.0/src/tucan/__pycache__/imports_main.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     3947 2024-01-18 09:05:54.000000 tucan-0.2.0/src/tucan/__pycache__/imports_py.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     9512 2024-05-13 20:39:25.000000 tucan-0.2.0/src/tucan/__pycache__/kw_lang.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     7926 2024-05-02 11:37:49.000000 tucan-0.2.0/src/tucan/__pycache__/package_analysis.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     5586 2024-05-02 09:37:34.000000 tucan-0.2.0/src/tucan/__pycache__/struct_c.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    15060 2024-05-13 20:43:31.000000 tucan-0.2.0/src/tucan/__pycache__/struct_common.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    10112 2024-05-13 20:44:18.000000 tucan-0.2.0/src/tucan/__pycache__/struct_ftn.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     4206 2024-05-13 14:36:41.000000 tucan-0.2.0/src/tucan/__pycache__/struct_main.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     8360 2024-05-13 14:51:07.000000 tucan-0.2.0/src/tucan/__pycache__/struct_py.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     7374 2024-02-09 13:04:11.000000 tucan-0.2.0/src/tucan/__pycache__/unformat_c.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    12498 2024-05-13 14:36:41.000000 tucan-0.2.0/src/tucan/__pycache__/unformat_common.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    21992 2024-05-07 13:35:34.000000 tucan-0.2.0/src/tucan/__pycache__/unformat_ftn.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     2804 2024-05-13 14:36:41.000000 tucan-0.2.0/src/tucan/__pycache__/unformat_main.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     7764 2024-03-05 16:53:14.000000 tucan-0.2.0/src/tucan/__pycache__/unformat_py.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    10612 2024-05-13 13:14:05.000000 tucan-0.2.0/src/tucan/clean_ifdef.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    13624 2024-05-13 13:13:16.000000 tucan-0.2.0/src/tucan/cli.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     1199 2024-02-29 17:03:40.000000 tucan-0.2.0/src/tucan/guess_language.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      923 2024-02-29 17:00:07.000000 tucan-0.2.0/src/tucan/imports_c.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      763 2023-12-27 08:38:53.000000 tucan-0.2.0/src/tucan/imports_common.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     1667 2023-12-27 08:38:53.000000 tucan-0.2.0/src/tucan/imports_ftn.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     1591 2024-02-29 16:59:22.000000 tucan-0.2.0/src/tucan/imports_main.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     2840 2023-12-27 08:38:53.000000 tucan-0.2.0/src/tucan/imports_py.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     9065 2024-05-13 20:39:22.000000 tucan-0.2.0/src/tucan/kw_lang.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     5212 2024-05-02 11:37:38.000000 tucan-0.2.0/src/tucan/package_analysis.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     4007 2024-05-02 09:31:09.000000 tucan-0.2.0/src/tucan/struct_c.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    10257 2024-05-13 20:41:21.000000 tucan-0.2.0/src/tucan/struct_common.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     7560 2024-05-13 20:44:16.000000 tucan-0.2.0/src/tucan/struct_ftn.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     2668 2024-05-13 13:11:47.000000 tucan-0.2.0/src/tucan/struct_main.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     5174 2024-05-13 14:50:45.000000 tucan-0.2.0/src/tucan/struct_py.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     4964 2024-02-09 13:04:09.000000 tucan-0.2.0/src/tucan/unformat_c.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     8117 2024-05-13 13:15:49.000000 tucan-0.2.0/src/tucan/unformat_common.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    15078 2024-05-07 13:35:31.000000 tucan-0.2.0/src/tucan/unformat_ftn.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     1398 2024-05-13 13:12:05.000000 tucan-0.2.0/src/tucan/unformat_main.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     6059 2024-03-05 16:53:12.000000 tucan-0.2.0/src/tucan/unformat_py.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2024-05-14 10:48:28.530972 tucan-0.2.0/src/tucan.egg-info/
+-rw-r--r--   0 dauptain   (502) staff       (20)     7749 2024-05-14 10:48:28.000000 tucan-0.2.0/src/tucan.egg-info/PKG-INFO
+-rw-r--r--   0 dauptain   (502) staff       (20)     1727 2024-05-14 10:48:28.000000 tucan-0.2.0/src/tucan.egg-info/SOURCES.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)        1 2024-05-14 10:48:28.000000 tucan-0.2.0/src/tucan.egg-info/dependency_links.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)       41 2024-05-14 10:48:28.000000 tucan-0.2.0/src/tucan.egg-info/entry_points.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)       83 2024-05-14 10:48:28.000000 tucan-0.2.0/src/tucan.egg-info/requires.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)        6 2024-05-14 10:48:28.000000 tucan-0.2.0/src/tucan.egg-info/top_level.txt
```

### Comparing `tucan-0.1.0/LICENSE.txt` & `tucan-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tucan-0.1.0/PKG-INFO` & `tucan-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tucan
-Version: 0.1.0
+Version: 0.2.0
 Summary: Unformatter Tool to allow parsing and analysis of code base.
 Home-page: https://gitlab.com/cerfacs/tucan
 Author: Antoine Dauptain, Thibault Marzlin, CoopTeam-CERFACS
 Author-email: coop@cerfacs.fr
 Project-URL: Homepage, https://gitlab.com/cerfacs/tucan
 Project-URL: Documentation, https://tucan.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.com/cerfacs/tucan/-/issues
@@ -17,26 +17,38 @@
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 ![tucan](https://images.unsplash.com/photo-1611788542170-38cf842212f4?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)
 
-TUCAN (Tool to Unformat, Clean, ands Analyse) is a code parser for scientific codebases. It tager languages are:
+TUCAN (Tool to Unformat, Clean, and Analyse) is a code parser for scientific codebases. Its target languages are:
+
 - Very old FORTRAN
 - Recent FORTRAN
 - Python (Under development)
-- C/C++ (Eazrly development)
+- C/C++ (Early development)
+
+## Installation
+
+You can instal it from [PyPI](https://pypi.org/project/tucan/) with:
+
+```bash
+pip install tucan
+```
+
+You can also install from the sources from one of our [gitlab mirrors](https://codehub.hlrs.de/coes/excellerat-p2/uc-2/tucan).
+
 
 ## What is does?
 
 
-### Remove Coding archaisms
+### Remove coding archaisms
 
-First is it a code cleaner. For example, this loop in `tranfit.f' a piece of CHEMKIN package  good'old FORTRAN:
+First it is a code cleaner. For example, this loop in `tranfit.f', a piece of [CHEMKIN](https://en.wikipedia.org/wiki/CHEMKIN) II package  in good'old FORTRAN77. (Do not worry, recent Chemkin is not written that way, probably)  :
 
 ```fortran
 (547)      DO 2000 K = 1, KK-1
 (548)         DO 2000 J = K+1, KK
 (549)            DO 2000 N = 1, NO
 (550)               COFD(N,J,K) = COFD(N,K,J)
 (551) 2000 CONTINUE
@@ -50,23 +62,26 @@
 (550-550)                 cofd(n,j,k)  =  cofd(n,k,j)
 (551-551)              end do ! 2000
 (551-551)           end do ! 2000
 (551-551)        end do ! 2000
 ```
 
 
-
-The cleaned version simplify the code for further analysis passes, like computing cyclomatic complexity, extracting structures, etc...
+The cleaned version is a simpler code for further analysis passes, like computing cyclomatic complexity, extracting structures, etc...
 
 
 ### Extracting code structure
 
-On the same file `tucan struct tranfit.f` provides a nested dictionary of the code structure. Here is an exemple from a code in very recent fortran:
+
+Here we start from a file of [neko](https://github.com/ExtremeFLOW/neko/blob/develop/src/adt/htable.f90), an HPC code in recent Fortran, finalist for the Gordon Bell Prize in 2023.
+
+`tucan struct htable.f90` provides a nested dictionary of the code structure. Here is a part of the output:
 
 ```yaml
+(...)
 type htable.h_tuple_t :
     At path ['htable', 'h_tuple_t'], name h_tuple_t, lines 47 -> 52
     6 statements over 6 lines
     Complexity 1
     Refers to 1 callables:
        - class
     Contains no inner structures
@@ -96,22 +111,25 @@
     At path ['htable', 'interface_abstract66'], name interface_abstract66, lines 66 -> 73
     8 statements over 8 lines
     Complexity 1
     Contains no callables
     Contains 1 elements:
     - htable.interface_abstract66.htable_hash
     Contains no annotations
+(...)
 ```
 
+*(This output will change as we update and improve tucan in the next versions!)*
+
 This information allows the creation and manipulation of graphs to extract the structure of the code
 
 
-### Interpreting IFDEFS 
+### Interpreting Conditional Inclusions "IF DEFS". 
 
-An other nasty example is the use of ìfdefs in C or FORTRAN:
+An other example of tucan is the analysis of [ifdefs](https://en.cppreference.com/w/c/preprocessor/conditional) in C or FORTRAN:
 
 ```
 #ifdef FRONT
         WRITE(*,*) " FRONT is enabled " ! partial front subroutine
         SUBROUTINE dummy_front(a,b,c)
         WRITE(*,*) " FRONT 1"     ! partial front subroutine
 #else                
@@ -178,11 +196,36 @@
 
         SUBROUTINE dummy_back(a,b,c)
         WRITE(*,*) " BACK is enabled " ! partial front subroutine
         WRITE(*,*) " BACK 1"    ! partial back subroutine
         END SUBROUTINE
 ```
 
+#### scanning ifdef variables
+
+A simpler usage of tucan : scan the current ifdefs variables. Still on [neko](https://github.com/ExtremeFLOW/neko) in the `/src` folder (an old version though) : 
+
+```bash
+/neko/src >tucan ifdef-scan-pkge .
+ - Recursive path gathering ...
+ - Cleaning the paths ...
+ - Analysis completed.
+ - Global ifdef variables : HAVE_PARMETIS, __APPLE__
+ - Local to device/opencl/check.c : CL_ERR_STR(err)
+ - Local to math/bcknd/device/opencl/opr_opgrad.c : CASE(LX), STR(X)
+ - Local to math/bcknd/device/opencl/opr_dudxyz.c : CASE(LX), STR(X)
+ - Local to common/sighdl.c : SIGHDL_ALRM, SIGHDL_USR1, SIGHDL_USR2, SIGHDL_XCPU
+ - Local to math/bcknd/device/opencl/opr_conv1.c : CASE(LX), STR(X)
+ - Local to math/bcknd/device/opencl/opr_cfl.c : CASE(LX), STR(X)
+ - Local to krylov/bcknd/device/opencl/pc_jacobi.c : CASE(LX), STR(X)
+ - Local to math/bcknd/device/opencl/ax_helm.c : CASE(LX), STR(X)
+ - Local to bc/bcknd/device/opencl/symmetry.c : MAX(a,
+ - Local to gs/bcknd/device/opencl/gs.c : GS_OP_ADD, GS_OP_MAX, GS_OP_MIN, GS_OP_MUL
+ - Local to sem/bcknd/device/opencl/coef.c : DXYZDRST_CASE(LX), GEO_CASE(LX), STR(X)
+ - Local to math/bcknd/device/opencl/opr_cdtp.c : CASE(LX), STR(X)
+```
+This feature is useful to see all potential variables that surcharge your codebase via conditional inclusions.
+
 ## More about tucan
 
 `Tucan` is used by  `anubis`, our open-source  tool to explore the git repository of a code, and `marauder's map`  our open-source tool to show codes structures by in-depth vizualisation of callgraphs and code circular-packing .
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tucan-0.1.0/README.md` & `tucan-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 ![tucan](https://images.unsplash.com/photo-1611788542170-38cf842212f4?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)
 
-TUCAN (Tool to Unformat, Clean, ands Analyse) is a code parser for scientific codebases. It tager languages are:
+TUCAN (Tool to Unformat, Clean, and Analyse) is a code parser for scientific codebases. Its target languages are:
+
 - Very old FORTRAN
 - Recent FORTRAN
 - Python (Under development)
-- C/C++ (Eazrly development)
+- C/C++ (Early development)
+
+## Installation
+
+You can instal it from [PyPI](https://pypi.org/project/tucan/) with:
+
+```bash
+pip install tucan
+```
+
+You can also install from the sources from one of our [gitlab mirrors](https://codehub.hlrs.de/coes/excellerat-p2/uc-2/tucan).
+
 
 ## What is does?
 
 
-### Remove Coding archaisms
+### Remove coding archaisms
 
-First is it a code cleaner. For example, this loop in `tranfit.f' a piece of CHEMKIN package  good'old FORTRAN:
+First it is a code cleaner. For example, this loop in `tranfit.f', a piece of [CHEMKIN](https://en.wikipedia.org/wiki/CHEMKIN) II package  in good'old FORTRAN77. (Do not worry, recent Chemkin is not written that way, probably)  :
 
 ```fortran
 (547)      DO 2000 K = 1, KK-1
 (548)         DO 2000 J = K+1, KK
 (549)            DO 2000 N = 1, NO
 (550)               COFD(N,J,K) = COFD(N,K,J)
 (551) 2000 CONTINUE
@@ -29,23 +41,26 @@
 (550-550)                 cofd(n,j,k)  =  cofd(n,k,j)
 (551-551)              end do ! 2000
 (551-551)           end do ! 2000
 (551-551)        end do ! 2000
 ```
 
 
-
-The cleaned version simplify the code for further analysis passes, like computing cyclomatic complexity, extracting structures, etc...
+The cleaned version is a simpler code for further analysis passes, like computing cyclomatic complexity, extracting structures, etc...
 
 
 ### Extracting code structure
 
-On the same file `tucan struct tranfit.f` provides a nested dictionary of the code structure. Here is an exemple from a code in very recent fortran:
+
+Here we start from a file of [neko](https://github.com/ExtremeFLOW/neko/blob/develop/src/adt/htable.f90), an HPC code in recent Fortran, finalist for the Gordon Bell Prize in 2023.
+
+`tucan struct htable.f90` provides a nested dictionary of the code structure. Here is a part of the output:
 
 ```yaml
+(...)
 type htable.h_tuple_t :
     At path ['htable', 'h_tuple_t'], name h_tuple_t, lines 47 -> 52
     6 statements over 6 lines
     Complexity 1
     Refers to 1 callables:
        - class
     Contains no inner structures
@@ -75,22 +90,25 @@
     At path ['htable', 'interface_abstract66'], name interface_abstract66, lines 66 -> 73
     8 statements over 8 lines
     Complexity 1
     Contains no callables
     Contains 1 elements:
     - htable.interface_abstract66.htable_hash
     Contains no annotations
+(...)
 ```
 
+*(This output will change as we update and improve tucan in the next versions!)*
+
 This information allows the creation and manipulation of graphs to extract the structure of the code
 
 
-### Interpreting IFDEFS 
+### Interpreting Conditional Inclusions "IF DEFS". 
 
-An other nasty example is the use of ìfdefs in C or FORTRAN:
+An other example of tucan is the analysis of [ifdefs](https://en.cppreference.com/w/c/preprocessor/conditional) in C or FORTRAN:
 
 ```
 #ifdef FRONT
         WRITE(*,*) " FRONT is enabled " ! partial front subroutine
         SUBROUTINE dummy_front(a,b,c)
         WRITE(*,*) " FRONT 1"     ! partial front subroutine
 #else                
@@ -157,11 +175,36 @@
 
         SUBROUTINE dummy_back(a,b,c)
         WRITE(*,*) " BACK is enabled " ! partial front subroutine
         WRITE(*,*) " BACK 1"    ! partial back subroutine
         END SUBROUTINE
 ```
 
+#### scanning ifdef variables
+
+A simpler usage of tucan : scan the current ifdefs variables. Still on [neko](https://github.com/ExtremeFLOW/neko) in the `/src` folder (an old version though) : 
+
+```bash
+/neko/src >tucan ifdef-scan-pkge .
+ - Recursive path gathering ...
+ - Cleaning the paths ...
+ - Analysis completed.
+ - Global ifdef variables : HAVE_PARMETIS, __APPLE__
+ - Local to device/opencl/check.c : CL_ERR_STR(err)
+ - Local to math/bcknd/device/opencl/opr_opgrad.c : CASE(LX), STR(X)
+ - Local to math/bcknd/device/opencl/opr_dudxyz.c : CASE(LX), STR(X)
+ - Local to common/sighdl.c : SIGHDL_ALRM, SIGHDL_USR1, SIGHDL_USR2, SIGHDL_XCPU
+ - Local to math/bcknd/device/opencl/opr_conv1.c : CASE(LX), STR(X)
+ - Local to math/bcknd/device/opencl/opr_cfl.c : CASE(LX), STR(X)
+ - Local to krylov/bcknd/device/opencl/pc_jacobi.c : CASE(LX), STR(X)
+ - Local to math/bcknd/device/opencl/ax_helm.c : CASE(LX), STR(X)
+ - Local to bc/bcknd/device/opencl/symmetry.c : MAX(a,
+ - Local to gs/bcknd/device/opencl/gs.c : GS_OP_ADD, GS_OP_MAX, GS_OP_MIN, GS_OP_MUL
+ - Local to sem/bcknd/device/opencl/coef.c : DXYZDRST_CASE(LX), GEO_CASE(LX), STR(X)
+ - Local to math/bcknd/device/opencl/opr_cdtp.c : CASE(LX), STR(X)
+```
+This feature is useful to see all potential variables that surcharge your codebase via conditional inclusions.
+
 ## More about tucan
 
 `Tucan` is used by  `anubis`, our open-source  tool to explore the git repository of a code, and `marauder's map`  our open-source tool to show codes structures by in-depth vizualisation of callgraphs and code circular-packing .
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tucan-0.1.0/setup.cfg` & `tucan-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tucan-0.1.0/src/.DS_Store` & `tucan-0.2.0/src/.DS_Store`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0086 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0001  ................
-00000050: 0000 0001 0000 1000 006e 7653 726e 6c6f  .........nvSrnlo
-00000060: 6e67 0000 0000 0000 0000 0000 0000 0000  ng..............
+00000040: 0000 0000 0000 0002 0000 0000 0000 0002  ................
+00000050: 0000 0001 0000 1000 006e 6277 7370 626c  .........nbwspbl
+00000060: 6f62 0000 0000 0000 0000 0000 0000 0000  ob..............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0000 0000 0000 0000 0000 0001 0000 0005  ................
-00000090: 0074 0075 0063 0061 006e 7653 726e 6c6f  .t.u.c.a.nvSrnlo
-000000a0: 6e67 0000 0001 0000 0000 0000 0000 0000  ng..............
+00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000100: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00000110: 0074 0075 0063 0061 006e 6277 7370 626c  .t.u.c.a.nbwspbl
+00000120: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
+00000130: 0203 0405 0607 0709 070b 075d 5368 6f77  ...........]Show
+00000140: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
+00000150: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
+00000160: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
+00000170: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+00000180: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+00000190: 7209 0908 095f 1018 7b7b 3333 342c 2033  r...._..{{334, 3
+000001a0: 3535 7d2c 207b 3932 302c 2034 3336 7d7d  55}, {920, 436}}
+000001b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
+000001c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
+000001d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
+000001e0: 0005 0074 0075 0063 0061 006e 7653 726e  ...t.u.c.a.nvSrn
+000001f0: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0086 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0108 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -317,27 +317,27 @@
 000013c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001430: 0200 0000 2000 0000 6000 0000 0100 0000  .... ...`.......
-00001440: c000 0000 0000 0000 0100 0001 0000 0000  ................
-00001450: 0100 0002 0000 0000 0100 0004 0000 0000  ................
-00001460: 0200 0008 0000 0018 0000 0000 0000 0000  ................
-00001470: 0100 0020 0000 0000 0100 0040 0000 0000  ... .......@....
-00001480: 0100 0080 0000 0000 0100 0100 0000 0000  ................
-00001490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
-000014a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
-000014b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
-000014c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
-000014d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
-000014e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
-000014f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
+00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
+00001440: 0100 0000 8000 0000 0000 0000 0100 0002  ................
+00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
+00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
+00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
+00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
+00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
+000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
+000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
+000014c0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
+000014d0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
+000014e0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
+000014f0: 0000 0000 0140 0000 0000 0000 0000 0000  .....@..........
 00001500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `tucan-0.1.0/src/tucan/__pycache__/cli.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/cli.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,58 +1,65 @@
 magic:    0xa70d0d0a
-moddate:  0xf555bb65 (Thu Feb  1 08:27:33 2024 UTC)
-files sz: 13194
+moddate:  0xec114266 (Mon May 13 13:13:16 2024 UTC)
+files sz: 13624
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 9
+   stacksize : 11
    flags     : 0
    code
       0x970064005a00640164026c015a01640164036c026d035a040100640164
       046c026d055a060100640584005a07020065016a080000000000000000a6
       000000ab000000000000000000650764068400a6000000ab000000000000
       000000a6000000ab0000000000000000005a096509a00a00000000000000
       00000000000000000000000000a6000000ab000000000000000000020065
       016a0b00000000000000006407650c6408ac09a6030000ab030000000000
       000000020065016a0d0000000000000000640a640b640c640dac0ea60400
-      00ab040000000000000000640f8400a6000000ab000000000000000000a6
-      000000ab000000000000000000a6000000ab0000000000000000005a0e65
-      09a00a0000000000000000000000000000000000000000a6000000ab0000
-      00000000000000020065016a0b00000000000000006407650c6408ac09a6
-      030000ab030000000000000000020065016a0d0000000000000000640a64
-      0b640c640dac0ea6040000ab04000000000000000064108400a6000000ab
-      000000000000000000a6000000ab000000000000000000a6000000ab0000
-      000000000000005a0f6509a00a0000000000000000000000000000000000
-      000000a6000000ab000000000000000000020065016a0b00000000000000
-      006407650c6408ac09a6030000ab030000000000000000020065016a0d00
-      00000000000000640a640b640c640dac0ea6040000ab0400000000000000
-      0064118400a6000000ab000000000000000000a6000000ab000000000000
-      000000a6000000ab0000000000000000005a106509a00a00000000000000
-      00000000000000000000000000a6000000ab000000000000000000020065
-      016a0b00000000000000006407650c6408ac09a6030000ab030000000000
-      000000020065016a0d0000000000000000640a640b640c640dac0ea60400
-      00ab04000000000000000064128400a6000000ab000000000000000000a6
-      000000ab000000000000000000a6000000ab0000000000000000005a1165
-      09a00a0000000000000000000000000000000000000000a6000000ab0000
-      00000000000000020065016a0b00000000000000006407650c6408ac09a6
-      030000ab030000000000000000020065016a0d0000000000000000641364
-      14650c64026415ac16a6050000ab050000000000000000020065016a0d00
-      00000000000000640a640b640c640dac0ea6040000ab0400000000000000
-      0064178400a6000000ab000000000000000000a6000000ab000000000000
+      00ab040000000000000000020065016a0d0000000000000000640f641064
+      0c6411ac0ea6040000ab0400000000000000006407650c6412650e641365
+      0e660664148404a6000000ab000000000000000000a6000000ab00000000
+      0000000000a6000000ab000000000000000000a6000000ab000000000000
+      0000005a0f6509a00a0000000000000000000000000000000000000000a6
+      000000ab000000000000000000020065016a0b0000000000000000640765
+      0c6408ac09a6030000ab030000000000000000020065016a0d0000000000
+      000000640a640b640c640dac0ea6040000ab040000000000000000020065
+      016a0d0000000000000000640f6410640c6411ac0ea6040000ab04000000
+      000000000064158400a6000000ab000000000000000000a6000000ab0000
+      00000000000000a6000000ab000000000000000000a6000000ab00000000
+      00000000005a106509a00a00000000000000000000000000000000000000
+      00a6000000ab000000000000000000020065016a0b000000000000000064
+      07650c6408ac09a6030000ab030000000000000000020065016a0d000000
+      0000000000640a640b640c640dac0ea6040000ab04000000000000000064
+      168400a6000000ab000000000000000000a6000000ab0000000000000000
+      00a6000000ab0000000000000000005a116509a00a000000000000000000
+      0000000000000000000000a6000000ab000000000000000000020065016a
+      0b00000000000000006407650c6408ac09a6030000ab0300000000000000
+      00020065016a0d0000000000000000640a640b640c640dac0ea6040000ab
+      04000000000000000064178400a6000000ab000000000000000000a60000
+      00ab000000000000000000a6000000ab0000000000000000005a126509a0
+      0a0000000000000000000000000000000000000000a6000000ab00000000
+      0000000000020065016a0b00000000000000006407650c6408ac09a60300
+      00ab030000000000000000020065016a0d00000000000000006418641965
+      0c6402641aac1ba6050000ab050000000000000000020065016a0d000000
+      0000000000640a640b640c640dac0ea6040000ab04000000000000000002
+      0065016a0d0000000000000000641c641d640c641eac0ea6040000ab0400
+      00000000000000020065016a0d0000000000000000640f6410640c641fac
+      0ea6040000ab04000000000000000064208400a6000000ab000000000000
       000000a6000000ab000000000000000000a6000000ab0000000000000000
-      005a126509a00a0000000000000000000000000000000000000000a60000
-      00ab000000000000000000020065016a0b00000000000000006418650c64
-      08ac09a6030000ab030000000000000000020065016a0d00000000000000
-      00640a640b640c640dac0ea6040000ab04000000000000000064198400a6
-      000000ab000000000000000000a6000000ab000000000000000000a60000
-      00ab0000000000000000005a136509a00a00000000000000000000000000
-      00000000000000a6000000ab000000000000000000020065016a0b000000
-      00000000006418650c6408ac09a6030000ab030000000000000000641a84
-      00a6000000ab000000000000000000a6000000ab0000000000000000005a
-      1464025300
+      00a6000000ab000000000000000000a6000000ab000000000000000000a6
+      000000ab0000000000000000005a136509a00a0000000000000000000000
+      000000000000000000a6000000ab000000000000000000020065016a0b00
+      000000000000006421650c6408ac09a6030000ab03000000000000000002
+      0065016a0d0000000000000000640a640b640c640dac0ea6040000ab0400
+      0000000000000064228400a6000000ab000000000000000000a6000000ab
+      000000000000000000a6000000ab0000000000000000005a146509a00a00
+      00000000000000000000000000000000000000a6000000ab000000000000
+      000000020065016a0b00000000000000006421650c6408ac09a6030000ab
+      03000000000000000064238400a6000000ab000000000000000000a60000
+      00ab0000000000000000005a1564025300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('Module helper for the CLI of tucan')
                  4 STORE_NAME               0 (__doc__)
    
      2           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
@@ -123,301 +130,384 @@
    
     68         202 LOAD_CONST              13 ('dump json data')
    
     64         204 KW_NAMES                14
                206 PRECALL                  4
                210 CALL                     4
    
-    70         220 LOAD_CONST              15 (<code object clean, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 62>)
-               222 MAKE_FUNCTION            0
+    70         220 PUSH_NULL
+               222 LOAD_NAME                1 (click)
+               224 LOAD_ATTR               13 (option)
+   
+    71         234 LOAD_CONST              15 ('-v')
+   
+    72         236 LOAD_CONST              16 ('--verbose')
+   
+    73         238 LOAD_CONST              12 (True)
+   
+    74         240 LOAD_CONST              17 ('verbose mode')
+   
+    70         242 KW_NAMES                14
+               244 PRECALL                  4
+               248 CALL                     4
+   
+    76         258 LOAD_CONST               7 ('filename')
+               260 LOAD_NAME               12 (str)
+               262 LOAD_CONST              18 ('dump')
+               264 LOAD_NAME               14 (bool)
+               266 LOAD_CONST              19 ('verbose')
+               268 LOAD_NAME               14 (bool)
+               270 BUILD_TUPLE              6
+               272 LOAD_CONST              20 (<code object clean, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 62>)
+               274 MAKE_FUNCTION            4 (annotations)
+   
+    70         276 PRECALL                  0
+               280 CALL                     0
+   
+    64         290 PRECALL                  0
+               294 CALL                     0
+   
+    63         304 PRECALL                  0
+               308 CALL                     0
+   
+    62         318 PRECALL                  0
+               322 CALL                     0
+   
+    76         332 STORE_NAME              15 (clean)
+   
+   128         334 LOAD_NAME                9 (main)
+               336 LOAD_METHOD             10 (command)
+               358 PRECALL                  0
+               362 CALL                     0
+   
+   129         372 PUSH_NULL
+               374 LOAD_NAME                1 (click)
+               376 LOAD_ATTR               11 (argument)
+               386 LOAD_CONST               7 ('filename')
+               388 LOAD_NAME               12 (str)
+               390 LOAD_CONST               8 (1)
+               392 KW_NAMES                 9
+               394 PRECALL                  3
+               398 CALL                     3
+   
+   130         408 PUSH_NULL
+               410 LOAD_NAME                1 (click)
+               412 LOAD_ATTR               13 (option)
+   
+   131         422 LOAD_CONST              10 ('-d')
    
-    64         224 PRECALL                  0
-               228 CALL                     0
+   132         424 LOAD_CONST              11 ('--dump')
    
-    63         238 PRECALL                  0
-               242 CALL                     0
+   133         426 LOAD_CONST              12 (True)
    
-    62         252 PRECALL                  0
-               256 CALL                     0
+   134         428 LOAD_CONST              13 ('dump json data')
    
-    70         266 STORE_NAME              14 (clean)
+   130         430 KW_NAMES                14
+               432 PRECALL                  4
+               436 CALL                     4
    
-   122         268 LOAD_NAME                9 (main)
-               270 LOAD_METHOD             10 (command)
-               292 PRECALL                  0
-               296 CALL                     0
+   136         446 PUSH_NULL
+               448 LOAD_NAME                1 (click)
+               450 LOAD_ATTR               13 (option)
    
-   123         306 PUSH_NULL
-               308 LOAD_NAME                1 (click)
-               310 LOAD_ATTR               11 (argument)
-               320 LOAD_CONST               7 ('filename')
-               322 LOAD_NAME               12 (str)
-               324 LOAD_CONST               8 (1)
-               326 KW_NAMES                 9
-               328 PRECALL                  3
-               332 CALL                     3
+   137         460 LOAD_CONST              15 ('-v')
    
-   124         342 PUSH_NULL
-               344 LOAD_NAME                1 (click)
-               346 LOAD_ATTR               13 (option)
+   138         462 LOAD_CONST              16 ('--verbose')
    
-   125         356 LOAD_CONST              10 ('-d')
+   139         464 LOAD_CONST              12 (True)
    
-   126         358 LOAD_CONST              11 ('--dump')
+   140         466 LOAD_CONST              17 ('verbose mode')
    
-   127         360 LOAD_CONST              12 (True)
+   136         468 KW_NAMES                14
+               470 PRECALL                  4
+               474 CALL                     4
    
-   128         362 LOAD_CONST              13 ('dump json data')
+   142         484 LOAD_CONST              21 (<code object struct, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 128>)
+               486 MAKE_FUNCTION            0
    
-   124         364 KW_NAMES                14
-               366 PRECALL                  4
-               370 CALL                     4
+   136         488 PRECALL                  0
+               492 CALL                     0
    
-   130         380 LOAD_CONST              16 (<code object struct, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 122>)
-               382 MAKE_FUNCTION            0
+   130         502 PRECALL                  0
+               506 CALL                     0
    
-   124         384 PRECALL                  0
-               388 CALL                     0
+   129         516 PRECALL                  0
+               520 CALL                     0
    
-   123         398 PRECALL                  0
-               402 CALL                     0
+   128         530 PRECALL                  0
+               534 CALL                     0
    
-   122         412 PRECALL                  0
-               416 CALL                     0
+   142         544 STORE_NAME              16 (struct)
    
-   130         426 STORE_NAME              15 (struct)
+   194         546 LOAD_NAME                9 (main)
+               548 LOAD_METHOD             10 (command)
+               570 PRECALL                  0
+               574 CALL                     0
    
-   182         428 LOAD_NAME                9 (main)
-               430 LOAD_METHOD             10 (command)
-               452 PRECALL                  0
-               456 CALL                     0
+   195         584 PUSH_NULL
+               586 LOAD_NAME                1 (click)
+               588 LOAD_ATTR               11 (argument)
+               598 LOAD_CONST               7 ('filename')
+               600 LOAD_NAME               12 (str)
+               602 LOAD_CONST               8 (1)
+               604 KW_NAMES                 9
+               606 PRECALL                  3
+               610 CALL                     3
    
-   183         466 PUSH_NULL
-               468 LOAD_NAME                1 (click)
-               470 LOAD_ATTR               11 (argument)
-               480 LOAD_CONST               7 ('filename')
-               482 LOAD_NAME               12 (str)
-               484 LOAD_CONST               8 (1)
-               486 KW_NAMES                 9
-               488 PRECALL                  3
-               492 CALL                     3
+   196         620 PUSH_NULL
+               622 LOAD_NAME                1 (click)
+               624 LOAD_ATTR               13 (option)
    
-   184         502 PUSH_NULL
-               504 LOAD_NAME                1 (click)
-               506 LOAD_ATTR               13 (option)
+   197         634 LOAD_CONST              10 ('-d')
    
-   185         516 LOAD_CONST              10 ('-d')
+   198         636 LOAD_CONST              11 ('--dump')
    
-   186         518 LOAD_CONST              11 ('--dump')
+   199         638 LOAD_CONST              12 (True)
    
-   187         520 LOAD_CONST              12 (True)
+   200         640 LOAD_CONST              13 ('dump json data')
    
-   188         522 LOAD_CONST              13 ('dump json data')
+   196         642 KW_NAMES                14
+               644 PRECALL                  4
+               648 CALL                     4
    
-   184         524 KW_NAMES                14
-               526 PRECALL                  4
-               530 CALL                     4
+   202         658 LOAD_CONST              22 (<code object imports, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 194>)
+               660 MAKE_FUNCTION            0
    
-   190         540 LOAD_CONST              17 (<code object imports, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 182>)
-               542 MAKE_FUNCTION            0
+   196         662 PRECALL                  0
+               666 CALL                     0
    
-   184         544 PRECALL                  0
-               548 CALL                     0
+   195         676 PRECALL                  0
+               680 CALL                     0
    
-   183         558 PRECALL                  0
-               562 CALL                     0
+   194         690 PRECALL                  0
+               694 CALL                     0
    
-   182         572 PRECALL                  0
-               576 CALL                     0
+   202         704 STORE_NAME              17 (imports)
    
-   190         586 STORE_NAME              16 (imports)
+   223         706 LOAD_NAME                9 (main)
+               708 LOAD_METHOD             10 (command)
+               730 PRECALL                  0
+               734 CALL                     0
    
-   211         588 LOAD_NAME                9 (main)
-               590 LOAD_METHOD             10 (command)
-               612 PRECALL                  0
-               616 CALL                     0
+   224         744 PUSH_NULL
+               746 LOAD_NAME                1 (click)
+               748 LOAD_ATTR               11 (argument)
+               758 LOAD_CONST               7 ('filename')
+               760 LOAD_NAME               12 (str)
+               762 LOAD_CONST               8 (1)
+               764 KW_NAMES                 9
+               766 PRECALL                  3
+               770 CALL                     3
    
-   212         626 PUSH_NULL
-               628 LOAD_NAME                1 (click)
-               630 LOAD_ATTR               11 (argument)
-               640 LOAD_CONST               7 ('filename')
-               642 LOAD_NAME               12 (str)
-               644 LOAD_CONST               8 (1)
-               646 KW_NAMES                 9
-               648 PRECALL                  3
-               652 CALL                     3
+   225         780 PUSH_NULL
+               782 LOAD_NAME                1 (click)
+               784 LOAD_ATTR               13 (option)
    
-   213         662 PUSH_NULL
-               664 LOAD_NAME                1 (click)
-               666 LOAD_ATTR               13 (option)
+   226         794 LOAD_CONST              10 ('-d')
    
-   214         676 LOAD_CONST              10 ('-d')
+   227         796 LOAD_CONST              11 ('--dump')
    
-   215         678 LOAD_CONST              11 ('--dump')
+   228         798 LOAD_CONST              12 (True)
    
-   216         680 LOAD_CONST              12 (True)
+   229         800 LOAD_CONST              13 ('dump json data')
    
-   217         682 LOAD_CONST              13 ('dump json data')
+   225         802 KW_NAMES                14
+               804 PRECALL                  4
+               808 CALL                     4
    
-   213         684 KW_NAMES                14
-               686 PRECALL                  4
-               690 CALL                     4
+   231         818 LOAD_CONST              23 (<code object ifdef_scan, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 223>)
+               820 MAKE_FUNCTION            0
    
-   219         700 LOAD_CONST              18 (<code object ifdef_scan, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 211>)
-               702 MAKE_FUNCTION            0
+   225         822 PRECALL                  0
+               826 CALL                     0
    
-   213         704 PRECALL                  0
-               708 CALL                     0
+   224         836 PRECALL                  0
+               840 CALL                     0
    
-   212         718 PRECALL                  0
-               722 CALL                     0
+   223         850 PRECALL                  0
+               854 CALL                     0
    
-   211         732 PRECALL                  0
-               736 CALL                     0
+   231         864 STORE_NAME              18 (ifdef_scan)
    
-   219         746 STORE_NAME              17 (ifdef_scan)
+   264         866 LOAD_NAME                9 (main)
+               868 LOAD_METHOD             10 (command)
+               890 PRECALL                  0
+               894 CALL                     0
    
-   252         748 LOAD_NAME                9 (main)
-               750 LOAD_METHOD             10 (command)
-               772 PRECALL                  0
-               776 CALL                     0
+   265         904 PUSH_NULL
+               906 LOAD_NAME                1 (click)
+               908 LOAD_ATTR               11 (argument)
+               918 LOAD_CONST               7 ('filename')
+               920 LOAD_NAME               12 (str)
+               922 LOAD_CONST               8 (1)
+               924 KW_NAMES                 9
+               926 PRECALL                  3
+               930 CALL                     3
    
-   253         786 PUSH_NULL
-               788 LOAD_NAME                1 (click)
-               790 LOAD_ATTR               11 (argument)
-               800 LOAD_CONST               7 ('filename')
-               802 LOAD_NAME               12 (str)
-               804 LOAD_CONST               8 (1)
-               806 KW_NAMES                 9
-               808 PRECALL                  3
-               812 CALL                     3
+   266         940 PUSH_NULL
+               942 LOAD_NAME                1 (click)
+               944 LOAD_ATTR               13 (option)
    
-   254         822 PUSH_NULL
-               824 LOAD_NAME                1 (click)
-               826 LOAD_ATTR               13 (option)
+   267         954 LOAD_CONST              24 ('-def')
    
-   255         836 LOAD_CONST              19 ('-v')
+   268         956 LOAD_CONST              25 ('--definitions')
    
-   256         838 LOAD_CONST              20 ('--variables')
+   269         958 LOAD_NAME               12 (str)
    
-   257         840 LOAD_NAME               12 (str)
+   270         960 LOAD_CONST               2 (None)
    
-   258         842 LOAD_CONST               2 (None)
+   272         962 LOAD_CONST              26 ("definitions to resolve ifdefs. Comma separated ',', no spaces : -v ARG1,ARG2")
    
-   260         844 LOAD_CONST              21 ("Variable to resolve ifdefs. Comma separated ',', no spaces : -v ARG1,ARG2")
+   266         964 KW_NAMES                27
+               966 PRECALL                  5
+               970 CALL                     5
    
-   254         846 KW_NAMES                22
-               848 PRECALL                  5
-               852 CALL                     5
+   274         980 PUSH_NULL
+               982 LOAD_NAME                1 (click)
+               984 LOAD_ATTR               13 (option)
    
-   262         862 PUSH_NULL
-               864 LOAD_NAME                1 (click)
-               866 LOAD_ATTR               13 (option)
+   275         994 LOAD_CONST              10 ('-d')
    
-   263         876 LOAD_CONST              10 ('-d')
+   276         996 LOAD_CONST              11 ('--dump')
    
-   264         878 LOAD_CONST              11 ('--dump')
+   277         998 LOAD_CONST              12 (True)
    
-   265         880 LOAD_CONST              12 (True)
+   278        1000 LOAD_CONST              13 ('dump json data')
    
-   266         882 LOAD_CONST              13 ('dump json data')
+   274        1002 KW_NAMES                14
+              1004 PRECALL                  4
+              1008 CALL                     4
    
-   262         884 KW_NAMES                14
-               886 PRECALL                  4
-               890 CALL                     4
+   280        1018 PUSH_NULL
+              1020 LOAD_NAME                1 (click)
+              1022 LOAD_ATTR               13 (option)
    
-   268         900 LOAD_CONST              23 (<code object ifdef_clean, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 252>)
-               902 MAKE_FUNCTION            0
+   281        1032 LOAD_CONST              28 ('-f')
    
-   262         904 PRECALL                  0
-               908 CALL                     0
+   282        1034 LOAD_CONST              29 ('--fortran')
    
-   254         918 PRECALL                  0
-               922 CALL                     0
+   283        1036 LOAD_CONST              12 (True)
    
-   253         932 PRECALL                  0
-               936 CALL                     0
+   284        1038 LOAD_CONST              30 (' fortran mode (avoid  stripping //)')
    
-   252         946 PRECALL                  0
-               950 CALL                     0
+   280        1040 KW_NAMES                14
+              1042 PRECALL                  4
+              1046 CALL                     4
    
-   268         960 STORE_NAME              18 (ifdef_clean)
+   286        1056 PUSH_NULL
+              1058 LOAD_NAME                1 (click)
+              1060 LOAD_ATTR               13 (option)
    
-   298         962 LOAD_NAME                9 (main)
-               964 LOAD_METHOD             10 (command)
-               986 PRECALL                  0
-               990 CALL                     0
+   287        1070 LOAD_CONST              15 ('-v')
    
-   299        1000 PUSH_NULL
-              1002 LOAD_NAME                1 (click)
-              1004 LOAD_ATTR               11 (argument)
-              1014 LOAD_CONST              24 ('path')
-              1016 LOAD_NAME               12 (str)
-              1018 LOAD_CONST               8 (1)
-              1020 KW_NAMES                 9
-              1022 PRECALL                  3
-              1026 CALL                     3
+   288        1072 LOAD_CONST              16 ('--verbose')
    
-   300        1036 PUSH_NULL
-              1038 LOAD_NAME                1 (click)
-              1040 LOAD_ATTR               13 (option)
+   289        1074 LOAD_CONST              12 (True)
    
-   301        1050 LOAD_CONST              10 ('-d')
+   290        1076 LOAD_CONST              31 ('verbose execution')
    
-   302        1052 LOAD_CONST              11 ('--dump')
+   286        1078 KW_NAMES                14
+              1080 PRECALL                  4
+              1084 CALL                     4
    
-   303        1054 LOAD_CONST              12 (True)
+   292        1094 LOAD_CONST              32 (<code object ifdef_clean, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 264>)
+              1096 MAKE_FUNCTION            0
    
-   304        1056 LOAD_CONST              13 ('dump json data')
+   286        1098 PRECALL                  0
+              1102 CALL                     0
    
-   300        1058 KW_NAMES                14
-              1060 PRECALL                  4
-              1064 CALL                     4
+   280        1112 PRECALL                  0
+              1116 CALL                     0
    
-   306        1074 LOAD_CONST              25 (<code object ifdef_scan_pkge, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 298>)
-              1076 MAKE_FUNCTION            0
+   274        1126 PRECALL                  0
+              1130 CALL                     0
    
-   300        1078 PRECALL                  0
-              1082 CALL                     0
+   266        1140 PRECALL                  0
+              1144 CALL                     0
    
-   299        1092 PRECALL                  0
-              1096 CALL                     0
+   265        1154 PRECALL                  0
+              1158 CALL                     0
    
-   298        1106 PRECALL                  0
-              1110 CALL                     0
+   264        1168 PRECALL                  0
+              1172 CALL                     0
    
-   306        1120 STORE_NAME              19 (ifdef_scan_pkge)
+   292        1182 STORE_NAME              19 (ifdef_clean)
    
-   364        1122 LOAD_NAME                9 (main)
-              1124 LOAD_METHOD             10 (command)
-              1146 PRECALL                  0
-              1150 CALL                     0
+   318        1184 LOAD_NAME                9 (main)
+              1186 LOAD_METHOD             10 (command)
+              1208 PRECALL                  0
+              1212 CALL                     0
    
-   365        1160 PUSH_NULL
-              1162 LOAD_NAME                1 (click)
-              1164 LOAD_ATTR               11 (argument)
-              1174 LOAD_CONST              24 ('path')
-              1176 LOAD_NAME               12 (str)
-              1178 LOAD_CONST               8 (1)
-              1180 KW_NAMES                 9
-              1182 PRECALL                  3
-              1186 CALL                     3
+   319        1222 PUSH_NULL
+              1224 LOAD_NAME                1 (click)
+              1226 LOAD_ATTR               11 (argument)
+              1236 LOAD_CONST              33 ('path')
+              1238 LOAD_NAME               12 (str)
+              1240 LOAD_CONST               8 (1)
+              1242 KW_NAMES                 9
+              1244 PRECALL                  3
+              1248 CALL                     3
    
-   366        1196 LOAD_CONST              26 (<code object package_analysis, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 364>)
-              1198 MAKE_FUNCTION            0
+   320        1258 PUSH_NULL
+              1260 LOAD_NAME                1 (click)
+              1262 LOAD_ATTR               13 (option)
    
-   365        1200 PRECALL                  0
-              1204 CALL                     0
+   321        1272 LOAD_CONST              10 ('-d')
    
-   364        1214 PRECALL                  0
-              1218 CALL                     0
+   322        1274 LOAD_CONST              11 ('--dump')
    
-   366        1228 STORE_NAME              20 (package_analysis)
-              1230 LOAD_CONST               2 (None)
-              1232 RETURN_VALUE
+   323        1276 LOAD_CONST              12 (True)
+   
+   324        1278 LOAD_CONST              13 ('dump json data')
+   
+   320        1280 KW_NAMES                14
+              1282 PRECALL                  4
+              1286 CALL                     4
+   
+   326        1296 LOAD_CONST              34 (<code object ifdef_scan_pkge, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 318>)
+              1298 MAKE_FUNCTION            0
+   
+   320        1300 PRECALL                  0
+              1304 CALL                     0
+   
+   319        1314 PRECALL                  0
+              1318 CALL                     0
+   
+   318        1328 PRECALL                  0
+              1332 CALL                     0
+   
+   326        1342 STORE_NAME              20 (ifdef_scan_pkge)
+   
+   384        1344 LOAD_NAME                9 (main)
+              1346 LOAD_METHOD             10 (command)
+              1368 PRECALL                  0
+              1372 CALL                     0
+   
+   385        1382 PUSH_NULL
+              1384 LOAD_NAME                1 (click)
+              1386 LOAD_ATTR               11 (argument)
+              1396 LOAD_CONST              33 ('path')
+              1398 LOAD_NAME               12 (str)
+              1400 LOAD_CONST               8 (1)
+              1402 KW_NAMES                 9
+              1404 PRECALL                  3
+              1408 CALL                     3
+   
+   386        1418 LOAD_CONST              35 (<code object package_analysis, file "/Users/dauptain/GITLAB/tucan/src/tucan/cli.py", line 384>)
+              1420 MAKE_FUNCTION            0
+   
+   385        1422 PRECALL                  0
+              1426 CALL                     0
+   
+   384        1436 PRECALL                  0
+              1440 CALL                     0
+   
+   386        1450 STORE_NAME              21 (package_analysis)
+              1452 LOAD_CONST               2 (None)
+              1454 RETURN_VALUE
    consts
       'Module helper for the CLI of tucan'
       0
       None
       ('__version__',)
       ('__name__',)
       code
@@ -489,264 +579,271 @@
       1
       ('type', 'nargs')
       '-d'
       '--dump'
       True
       'dump json data'
       ('is_flag', 'help')
+      '-v'
+      '--verbose'
+      'verbose mode'
+      'dump'
+      'verbose'
       code
-         argcount  : 2
-         nlocals   : 5
+         argcount  : 3
+         nlocals   : 6
          stacksize : 4
          flags     : 3
          code
-            0x9700640164026c006d017d02010002007c027c00a6010000ab01000000
-            00000000007d037c00a00200000000000000000000000000000000000000
-            006403a6010000ab010000000000000000640419000000000000000000a0
-            0200000000000000000000000000000000000000006405a6010000ab0100
-            000000000000006401190000000000000000007d04740700000000000000
-            0000007c03a6010000ab01000000000000000001007c03a0040000000000
-            00000000000000000000000000000064067c047a00000064077a000000a6
-            010000ab01000000000000000001007c01721d7c03a00500000000000000
-            0000000000000000000000000064067c047a00000064087a000000a60100
-            00ab01000000000000000001006409530064095300
+            0x9700640164026c006d017d03010002007c037c007c02a6020000ab0200
+            000000000000007d047c00a0020000000000000000000000000000000000
+            0000006403a6010000ab0100000000000000006404190000000000000000
+            00a00200000000000000000000000000000000000000006405a6010000ab
+            0100000000000000006401190000000000000000007d0574070000000000
+            00000000007c04a6010000ab01000000000000000001007c04a004000000
+            000000000000000000000000000000000064067c057a00000064077a0000
+            00a6010000ab01000000000000000001007c01721d7c04a0050000000000
+            00000000000000000000000000000064067c057a00000064087a000000a6
+            010000ab01000000000000000001006409530064095300
           62           0 RESUME                   0
          
-          80           2 LOAD_CONST               1 (0)
+          86           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (('unformat_main',))
                        6 IMPORT_NAME              0 (tucan.unformat_main)
                        8 IMPORT_FROM              1 (unformat_main)
-                      10 STORE_FAST               2 (unformat_main)
+                      10 STORE_FAST               3 (unformat_main)
                       12 POP_TOP
          
-          82          14 PUSH_NULL
-                      16 LOAD_FAST                2 (unformat_main)
+          88          14 PUSH_NULL
+                      16 LOAD_FAST                3 (unformat_main)
                       18 LOAD_FAST                0 (filename)
-                      20 PRECALL                  1
-                      24 CALL                     1
-                      34 STORE_FAST               3 (statements)
-         
-          84          36 LOAD_FAST                0 (filename)
-                      38 LOAD_METHOD              2 (split)
-                      60 LOAD_CONST               3 ('/')
-                      62 PRECALL                  1
-                      66 CALL                     1
-                      76 LOAD_CONST               4 (-1)
-                      78 BINARY_SUBSCR
-                      88 LOAD_METHOD              2 (split)
-                     110 LOAD_CONST               5 ('.')
-                     112 PRECALL                  1
-                     116 CALL                     1
-                     126 LOAD_CONST               1 (0)
-                     128 BINARY_SUBSCR
-                     138 STORE_FAST               4 (base)
-         
-          85         140 LOAD_GLOBAL              7 (NULL + print)
-                     152 LOAD_FAST                3 (statements)
-                     154 PRECALL                  1
-                     158 CALL                     1
-                     168 POP_TOP
-         
-          87         170 LOAD_FAST                3 (statements)
-                     172 LOAD_METHOD              4 (dump_code)
-                     194 LOAD_CONST               6 ('./')
-                     196 LOAD_FAST                4 (base)
-                     198 BINARY_OP                0 (+)
-                     202 LOAD_CONST               7 ('._rfmt')
-                     204 BINARY_OP                0 (+)
-                     208 PRECALL                  1
-                     212 CALL                     1
-                     222 POP_TOP
-         
-          89         224 LOAD_FAST                1 (dump)
-                     226 POP_JUMP_FORWARD_IF_FALSE    29 (to 286)
-         
-          90         228 LOAD_FAST                3 (statements)
-                     230 LOAD_METHOD              5 (dump_json)
-                     252 LOAD_CONST               6 ('./')
-                     254 LOAD_FAST                4 (base)
-                     256 BINARY_OP                0 (+)
-                     260 LOAD_CONST               8 ('.json')
-                     262 BINARY_OP                0 (+)
-                     266 PRECALL                  1
-                     270 CALL                     1
-                     280 POP_TOP
-                     282 LOAD_CONST               9 (None)
-                     284 RETURN_VALUE
+                      20 LOAD_FAST                2 (verbose)
+                      22 PRECALL                  2
+                      26 CALL                     2
+                      36 STORE_FAST               4 (statements)
+         
+          90          38 LOAD_FAST                0 (filename)
+                      40 LOAD_METHOD              2 (split)
+                      62 LOAD_CONST               3 ('/')
+                      64 PRECALL                  1
+                      68 CALL                     1
+                      78 LOAD_CONST               4 (-1)
+                      80 BINARY_SUBSCR
+                      90 LOAD_METHOD              2 (split)
+                     112 LOAD_CONST               5 ('.')
+                     114 PRECALL                  1
+                     118 CALL                     1
+                     128 LOAD_CONST               1 (0)
+                     130 BINARY_SUBSCR
+                     140 STORE_FAST               5 (base)
+         
+          91         142 LOAD_GLOBAL              7 (NULL + print)
+                     154 LOAD_FAST                4 (statements)
+                     156 PRECALL                  1
+                     160 CALL                     1
+                     170 POP_TOP
+         
+          93         172 LOAD_FAST                4 (statements)
+                     174 LOAD_METHOD              4 (dump_code)
+                     196 LOAD_CONST               6 ('./')
+                     198 LOAD_FAST                5 (base)
+                     200 BINARY_OP                0 (+)
+                     204 LOAD_CONST               7 ('._rfmt')
+                     206 BINARY_OP                0 (+)
+                     210 PRECALL                  1
+                     214 CALL                     1
+                     224 POP_TOP
+         
+          95         226 LOAD_FAST                1 (dump)
+                     228 POP_JUMP_FORWARD_IF_FALSE    29 (to 288)
+         
+          96         230 LOAD_FAST                4 (statements)
+                     232 LOAD_METHOD              5 (dump_json)
+                     254 LOAD_CONST               6 ('./')
+                     256 LOAD_FAST                5 (base)
+                     258 BINARY_OP                0 (+)
+                     262 LOAD_CONST               8 ('.json')
+                     264 BINARY_OP                0 (+)
+                     268 PRECALL                  1
+                     272 CALL                     1
+                     282 POP_TOP
+                     284 LOAD_CONST               9 (None)
+                     286 RETURN_VALUE
          
-          89     >>  286 LOAD_CONST               9 (None)
-                     288 RETURN_VALUE
+          95     >>  288 LOAD_CONST               9 (None)
+                     290 RETURN_VALUE
          consts
             "\n    Unformat a fortran of python single file.\n\n    \x08\n    - Merge multiline statements to one line\n    - Split ';' statements\n    - Strip comments.\n    - Strip blank lines.\n    "
             0
             ('unformat_main',)
             '/'
             -1
             '.'
             './'
             '._rfmt'
             '.json'
             None
          names      ('tucan.unformat_main', 'unformat_main', 'split', 'print', 'dump_code', 'dump_json')
-         varnames   ('filename', 'dump', 'unformat_main', 'statements', 'base')
+         varnames   ('filename', 'dump', 'verbose', 'unformat_main', 'statements', 'base')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/cli.py'
          name       'clean'
          firstlineno 62
-         lnotab 0x02120c02160268011e02360204013aff
+         lnotab 0x02180c02180268011e02360204013aff
       code
-         argcount  : 2
-         nlocals   : 10
+         argcount  : 3
+         nlocals   : 11
          stacksize : 7
          flags     : 3
          code
-            0x9700640164026c007d02640164036c016d027d030100640164046c036d
-            047d040100640164056c056d067d05010002007c047c00a6010000ab0100
-            000000000000007d067c03a0070000000000000000000000000000000000
-            000000640602007c057c06a6010000ab0100000000000000007a000000a6
-            010000ab01000000000000000001007c00a0080000000000000000000000
-            0000000000000000006407a6010000ab0100000000000000006408190000
-            00000000000000a008000000000000000000000000000000000000000064
-            09a6010000ab0100000000000000006401190000000000000000007d077c
-            0172617c07640a7a0000007d087c03a00700000000000000000000000000
-            00000000000000640b7c089b009d02a6010000ab01000000000000000001
-            007413000000000000000000007c08640ca6020000ab0200000000000000
-            0035007d097c02a00a00000000000000000000000000000000000000007c
-            067c09640d640eac0fa6040000ab04000000000000000001006402640264
-            02a6020000ab020000000000000000010064025300230031007304770278
-            035900770101005900010001006402530064025300
-         122           0 RESUME                   0
+            0x9700640164026c007d03640164036c016d027d040100640164046c036d
+            047d050100640164056c056d067d06010002007c057c007c02a6020000ab
+            0200000000000000007d077c04a007000000000000000000000000000000
+            0000000000640602007c067c07a6010000ab0100000000000000007a0000
+            00a6010000ab01000000000000000001007c00a008000000000000000000
+            00000000000000000000006407a6010000ab010000000000000000640819
+            000000000000000000a00800000000000000000000000000000000000000
+            006409a6010000ab0100000000000000006401190000000000000000007d
+            087c0172617c08640a7a0000007d097c04a0070000000000000000000000
+            000000000000000000640b7c099b009d02a6010000ab0100000000000000
+            0001007413000000000000000000007c09640ca6020000ab020000000000
+            00000035007d0a7c03a00a00000000000000000000000000000000000000
+            007c077c0a640d640eac0fa6040000ab0400000000000000000100640264
+            026402a6020000ab02000000000000000001006402530023003100730477
+            0278035900770101005900010001006402530064025300
+         128           0 RESUME                   0
          
-         139           2 LOAD_CONST               1 (0)
+         151           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (None)
                        6 IMPORT_NAME              0 (json)
-                       8 STORE_FAST               2 (json)
+                       8 STORE_FAST               3 (json)
          
-         140          10 LOAD_CONST               1 (0)
+         152          10 LOAD_CONST               1 (0)
                       12 LOAD_CONST               3 (('logger',))
                       14 IMPORT_NAME              1 (loguru)
                       16 IMPORT_FROM              2 (logger)
-                      18 STORE_FAST               3 (logger)
+                      18 STORE_FAST               4 (logger)
                       20 POP_TOP
          
-         142          22 LOAD_CONST               1 (0)
+         154          22 LOAD_CONST               1 (0)
                       24 LOAD_CONST               4 (('struct_main',))
                       26 IMPORT_NAME              3 (tucan.struct_main)
                       28 IMPORT_FROM              4 (struct_main)
-                      30 STORE_FAST               4 (struct_main)
+                      30 STORE_FAST               5 (struct_main)
                       32 POP_TOP
          
-         143          34 LOAD_CONST               1 (0)
+         155          34 LOAD_CONST               1 (0)
                       36 LOAD_CONST               5 (('struct_summary_str',))
                       38 IMPORT_NAME              5 (tucan.struct_common)
                       40 IMPORT_FROM              6 (struct_summary_str)
-                      42 STORE_FAST               5 (struct_summary_str)
+                      42 STORE_FAST               6 (struct_summary_str)
                       44 POP_TOP
          
-         145          46 PUSH_NULL
-                      48 LOAD_FAST                4 (struct_main)
+         157          46 PUSH_NULL
+                      48 LOAD_FAST                5 (struct_main)
                       50 LOAD_FAST                0 (filename)
-                      52 PRECALL                  1
-                      56 CALL                     1
-                      66 STORE_FAST               6 (struct_)
-         
-         146          68 LOAD_FAST                3 (logger)
-                      70 LOAD_METHOD              7 (info)
-                      92 LOAD_CONST               6 ('Found following structure:\n')
-                      94 PUSH_NULL
-                      96 LOAD_FAST                5 (struct_summary_str)
-                      98 LOAD_FAST                6 (struct_)
-                     100 PRECALL                  1
-                     104 CALL                     1
-                     114 BINARY_OP                0 (+)
-                     118 PRECALL                  1
-                     122 CALL                     1
-                     132 POP_TOP
-         
-         147         134 LOAD_FAST                0 (filename)
-                     136 LOAD_METHOD              8 (split)
-                     158 LOAD_CONST               7 ('/')
-                     160 PRECALL                  1
-                     164 CALL                     1
-                     174 LOAD_CONST               8 (-1)
-                     176 BINARY_SUBSCR
-                     186 LOAD_METHOD              8 (split)
-                     208 LOAD_CONST               9 ('.')
-                     210 PRECALL                  1
-                     214 CALL                     1
-                     224 LOAD_CONST               1 (0)
-                     226 BINARY_SUBSCR
-                     236 STORE_FAST               7 (base)
-         
-         148         238 LOAD_FAST                1 (dump)
-                     240 POP_JUMP_FORWARD_IF_FALSE    97 (to 436)
-         
-         149         242 LOAD_FAST                7 (base)
-                     244 LOAD_CONST              10 ('.json')
-                     246 BINARY_OP                0 (+)
-                     250 STORE_FAST               8 (newfile)
-         
-         150         252 LOAD_FAST                3 (logger)
-                     254 LOAD_METHOD              7 (info)
-                     276 LOAD_CONST              11 ('Data dumped to ')
-                     278 LOAD_FAST                8 (newfile)
-                     280 FORMAT_VALUE             0
-                     282 BUILD_STRING             2
-                     284 PRECALL                  1
-                     288 CALL                     1
-                     298 POP_TOP
-         
-         151         300 LOAD_GLOBAL             19 (NULL + open)
-                     312 LOAD_FAST                8 (newfile)
-                     314 LOAD_CONST              12 ('w')
-                     316 PRECALL                  2
-                     320 CALL                     2
-                     330 BEFORE_WITH
-                     332 STORE_FAST               9 (fout)
-         
-         152         334 LOAD_FAST                2 (json)
-                     336 LOAD_METHOD             10 (dump)
-                     358 LOAD_FAST                6 (struct_)
-                     360 LOAD_FAST                9 (fout)
-                     362 LOAD_CONST              13 (2)
-                     364 LOAD_CONST              14 (True)
-                     366 KW_NAMES                15
-                     368 PRECALL                  4
-                     372 CALL                     4
-                     382 POP_TOP
+                      52 LOAD_FAST                2 (verbose)
+                      54 PRECALL                  2
+                      58 CALL                     2
+                      68 STORE_FAST               7 (struct_)
+         
+         158          70 LOAD_FAST                4 (logger)
+                      72 LOAD_METHOD              7 (info)
+                      94 LOAD_CONST               6 ('Found following structure:\n')
+                      96 PUSH_NULL
+                      98 LOAD_FAST                6 (struct_summary_str)
+                     100 LOAD_FAST                7 (struct_)
+                     102 PRECALL                  1
+                     106 CALL                     1
+                     116 BINARY_OP                0 (+)
+                     120 PRECALL                  1
+                     124 CALL                     1
+                     134 POP_TOP
+         
+         159         136 LOAD_FAST                0 (filename)
+                     138 LOAD_METHOD              8 (split)
+                     160 LOAD_CONST               7 ('/')
+                     162 PRECALL                  1
+                     166 CALL                     1
+                     176 LOAD_CONST               8 (-1)
+                     178 BINARY_SUBSCR
+                     188 LOAD_METHOD              8 (split)
+                     210 LOAD_CONST               9 ('.')
+                     212 PRECALL                  1
+                     216 CALL                     1
+                     226 LOAD_CONST               1 (0)
+                     228 BINARY_SUBSCR
+                     238 STORE_FAST               8 (base)
+         
+         160         240 LOAD_FAST                1 (dump)
+                     242 POP_JUMP_FORWARD_IF_FALSE    97 (to 438)
+         
+         161         244 LOAD_FAST                8 (base)
+                     246 LOAD_CONST              10 ('.json')
+                     248 BINARY_OP                0 (+)
+                     252 STORE_FAST               9 (newfile)
+         
+         162         254 LOAD_FAST                4 (logger)
+                     256 LOAD_METHOD              7 (info)
+                     278 LOAD_CONST              11 ('Data dumped to ')
+                     280 LOAD_FAST                9 (newfile)
+                     282 FORMAT_VALUE             0
+                     284 BUILD_STRING             2
+                     286 PRECALL                  1
+                     290 CALL                     1
+                     300 POP_TOP
+         
+         163         302 LOAD_GLOBAL             19 (NULL + open)
+                     314 LOAD_FAST                9 (newfile)
+                     316 LOAD_CONST              12 ('w')
+                     318 PRECALL                  2
+                     322 CALL                     2
+                     332 BEFORE_WITH
+                     334 STORE_FAST              10 (fout)
+         
+         164         336 LOAD_FAST                3 (json)
+                     338 LOAD_METHOD             10 (dump)
+                     360 LOAD_FAST                7 (struct_)
+                     362 LOAD_FAST               10 (fout)
+                     364 LOAD_CONST              13 (2)
+                     366 LOAD_CONST              14 (True)
+                     368 KW_NAMES                15
+                     370 PRECALL                  4
+                     374 CALL                     4
+                     384 POP_TOP
          
-         151         384 LOAD_CONST               2 (None)
-                     386 LOAD_CONST               2 (None)
+         163         386 LOAD_CONST               2 (None)
                      388 LOAD_CONST               2 (None)
-                     390 PRECALL                  2
-                     394 CALL                     2
-                     404 POP_TOP
-                     406 LOAD_CONST               2 (None)
-                     408 RETURN_VALUE
-                 >>  410 PUSH_EXC_INFO
-                     412 WITH_EXCEPT_START
-                     414 POP_JUMP_FORWARD_IF_TRUE     4 (to 424)
-                     416 RERAISE                  2
-                 >>  418 COPY                     3
-                     420 POP_EXCEPT
-                     422 RERAISE                  1
-                 >>  424 POP_TOP
-                     426 POP_EXCEPT
-                     428 POP_TOP
+                     390 LOAD_CONST               2 (None)
+                     392 PRECALL                  2
+                     396 CALL                     2
+                     406 POP_TOP
+                     408 LOAD_CONST               2 (None)
+                     410 RETURN_VALUE
+                 >>  412 PUSH_EXC_INFO
+                     414 WITH_EXCEPT_START
+                     416 POP_JUMP_FORWARD_IF_TRUE     4 (to 426)
+                     418 RERAISE                  2
+                 >>  420 COPY                     3
+                     422 POP_EXCEPT
+                     424 RERAISE                  1
+                 >>  426 POP_TOP
+                     428 POP_EXCEPT
                      430 POP_TOP
-                     432 LOAD_CONST               2 (None)
-                     434 RETURN_VALUE
+                     432 POP_TOP
+                     434 LOAD_CONST               2 (None)
+                     436 RETURN_VALUE
          
-         148     >>  436 LOAD_CONST               2 (None)
-                     438 RETURN_VALUE
+         160     >>  438 LOAD_CONST               2 (None)
+                     440 RETURN_VALUE
          ExceptionTable:
-           332 to 382 -> 410 [1] lasti
-           410 to 416 -> 418 [3] lasti
-           424 to 424 -> 418 [3] lasti
+           334 to 384 -> 412 [1] lasti
+           412 to 418 -> 420 [3] lasti
+           426 to 426 -> 420 [3] lasti
          consts
             '\n    Extract structure of a fortran or python single file.\n\n    \x08\n    - Find the nested structures of a code\n    - Find the callables in each structure\n    - Evaluate sizes, CCN\n    '
             0
             None
             ('logger',)
             ('struct_main',)
             ('struct_summary_str',)
@@ -757,21 +854,21 @@
             '.json'
             'Data dumped to '
             'w'
             2
             True
             ('indent', 'sort_keys')
          names      ('json', 'loguru', 'logger', 'tucan.struct_main', 'struct_main', 'tucan.struct_common', 'struct_summary_str', 'info', 'split', 'open', 'dump')
-         varnames   ('filename', 'dump', 'json', 'logger', 'struct_main', 'struct_summary_str', 'struct_', 'base', 'newfile', 'fout')
+         varnames   ('filename', 'dump', 'verbose', 'json', 'logger', 'struct_main', 'struct_summary_str', 'struct_', 'base', 'newfile', 'fout')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/cli.py'
          name       'struct'
-         firstlineno 122
-         lnotab 0x021108010c020c010c0216014201680104010a013001220132ff34fd
+         firstlineno 128
+         lnotab 0x021708010c020c010c0218014201680104010a013001220132ff34fd
       code
          argcount  : 2
          nlocals   : 10
          stacksize : 7
          flags     : 3
          code
             0x9700640164026c007d02640164036c016d027d030100640164046c036d
@@ -785,115 +882,115 @@
             007d077c07640a7a0000007d087c03a00700000000000000000000000000
             00000000000000640b7c089b009d02a6010000ab01000000000000000001
             007413000000000000000000007c08640ca6020000ab0200000000000000
             0035007d097c02a00a00000000000000000000000000000000000000007c
             067c09640d640eac0fa6040000ab04000000000000000001006402640264
             02a6020000ab020000000000000000010064025300230031007304770278
             035900770101005900010001006402530064025300
-         182           0 RESUME                   0
+         194           0 RESUME                   0
          
-         194           2 LOAD_CONST               1 (0)
+         206           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (None)
                        6 IMPORT_NAME              0 (json)
                        8 STORE_FAST               2 (json)
          
-         195          10 LOAD_CONST               1 (0)
+         207          10 LOAD_CONST               1 (0)
                       12 LOAD_CONST               3 (('logger',))
                       14 IMPORT_NAME              1 (loguru)
                       16 IMPORT_FROM              2 (logger)
                       18 STORE_FAST               3 (logger)
                       20 POP_TOP
          
-         197          22 LOAD_CONST               1 (0)
+         209          22 LOAD_CONST               1 (0)
                       24 LOAD_CONST               4 (('imports_main',))
                       26 IMPORT_NAME              3 (tucan.imports_main)
                       28 IMPORT_FROM              4 (imports_main)
                       30 STORE_FAST               4 (imports_main)
                       32 POP_TOP
          
-         198          34 LOAD_CONST               1 (0)
+         210          34 LOAD_CONST               1 (0)
                       36 LOAD_CONST               5 (('imports_summary_str',))
                       38 IMPORT_NAME              5 (tucan.imports_common)
                       40 IMPORT_FROM              6 (imports_summary_str)
                       42 STORE_FAST               5 (imports_summary_str)
                       44 POP_TOP
          
-         200          46 PUSH_NULL
+         212          46 PUSH_NULL
                       48 LOAD_FAST                4 (imports_main)
                       50 LOAD_FAST                0 (filename)
                       52 PRECALL                  1
                       56 CALL                     1
                       66 STORE_FAST               6 (imports_)
          
-         201          68 LOAD_FAST                3 (logger)
+         213          68 LOAD_FAST                3 (logger)
                       70 LOAD_METHOD              7 (info)
                       92 LOAD_CONST               6 ('Found following structure:\n')
                       94 PUSH_NULL
                       96 LOAD_FAST                5 (imports_summary_str)
                       98 LOAD_FAST                6 (imports_)
                      100 PRECALL                  1
                      104 CALL                     1
                      114 BINARY_OP                0 (+)
                      118 PRECALL                  1
                      122 CALL                     1
                      132 POP_TOP
          
-         202         134 LOAD_FAST                1 (dump)
+         214         134 LOAD_FAST                1 (dump)
                      136 POP_JUMP_FORWARD_IF_FALSE   149 (to 436)
          
-         203         138 LOAD_FAST                0 (filename)
+         215         138 LOAD_FAST                0 (filename)
                      140 LOAD_METHOD              8 (split)
                      162 LOAD_CONST               7 ('/')
                      164 PRECALL                  1
                      168 CALL                     1
                      178 LOAD_CONST               8 (-1)
                      180 BINARY_SUBSCR
                      190 LOAD_METHOD              8 (split)
                      212 LOAD_CONST               9 ('.')
                      214 PRECALL                  1
                      218 CALL                     1
                      228 LOAD_CONST               1 (0)
                      230 BINARY_SUBSCR
                      240 STORE_FAST               7 (base)
          
-         204         242 LOAD_FAST                7 (base)
+         216         242 LOAD_FAST                7 (base)
                      244 LOAD_CONST              10 ('_imports.json')
                      246 BINARY_OP                0 (+)
                      250 STORE_FAST               8 (newfile)
          
-         205         252 LOAD_FAST                3 (logger)
+         217         252 LOAD_FAST                3 (logger)
                      254 LOAD_METHOD              7 (info)
                      276 LOAD_CONST              11 ('Data dumped to ')
                      278 LOAD_FAST                8 (newfile)
                      280 FORMAT_VALUE             0
                      282 BUILD_STRING             2
                      284 PRECALL                  1
                      288 CALL                     1
                      298 POP_TOP
          
-         206         300 LOAD_GLOBAL             19 (NULL + open)
+         218         300 LOAD_GLOBAL             19 (NULL + open)
                      312 LOAD_FAST                8 (newfile)
                      314 LOAD_CONST              12 ('w')
                      316 PRECALL                  2
                      320 CALL                     2
                      330 BEFORE_WITH
                      332 STORE_FAST               9 (fout)
          
-         207         334 LOAD_FAST                2 (json)
+         219         334 LOAD_FAST                2 (json)
                      336 LOAD_METHOD             10 (dump)
                      358 LOAD_FAST                6 (imports_)
                      360 LOAD_FAST                9 (fout)
                      362 LOAD_CONST              13 (2)
                      364 LOAD_CONST              14 (True)
                      366 KW_NAMES                15
                      368 PRECALL                  4
                      372 CALL                     4
                      382 POP_TOP
          
-         206         384 LOAD_CONST               2 (None)
+         218         384 LOAD_CONST               2 (None)
                      386 LOAD_CONST               2 (None)
                      388 LOAD_CONST               2 (None)
                      390 PRECALL                  2
                      394 CALL                     2
                      404 POP_TOP
                      406 LOAD_CONST               2 (None)
                      408 RETURN_VALUE
@@ -907,15 +1004,15 @@
                  >>  424 POP_TOP
                      426 POP_EXCEPT
                      428 POP_TOP
                      430 POP_TOP
                      432 LOAD_CONST               2 (None)
                      434 RETURN_VALUE
          
-         202     >>  436 LOAD_CONST               2 (None)
+         214     >>  436 LOAD_CONST               2 (None)
                      438 RETURN_VALUE
          ExceptionTable:
            332 to 382 -> 410 [1] lasti
            410 to 416 -> 418 [3] lasti
            424 to 424 -> 418 [3] lasti
          consts
             '\n    Extract imports of a single file.\n    '
@@ -936,15 +1033,15 @@
             ('indent', 'sort_keys')
          names      ('json', 'loguru', 'logger', 'tucan.imports_main', 'imports_main', 'tucan.imports_common', 'imports_summary_str', 'info', 'split', 'open', 'dump')
          varnames   ('filename', 'dump', 'json', 'logger', 'imports_main', 'imports_summary_str', 'imports_', 'base', 'newfile', 'fout')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/cli.py'
          name       'imports'
-         firstlineno 182
+         firstlineno 194
          lnotab 0x020c08010c020c010c0216014201040168010a013001220132ff34fc
       code
          argcount  : 2
          nlocals   : 15
          stacksize : 7
          flags     : 3
          code
@@ -970,54 +1067,54 @@
             090000000000000000000000000000000000000000640f7c0c9b009d02a6
             010000ab01000000000000000001007c077c0864109c027d0d740b000000
             000000000000007c0c6411a6020000ab02000000000000000035007d0e7c
             02a00a00000000000000000000000000000000000000007c0d7c0e641264
             13ac14a6040000ab0400000000000000000100640264026402a6020000ab
             020000000000000000010064025300230031007304770278035900770101
             005900010001006402530064025300
-         211           0 RESUME                   0
+         223           0 RESUME                   0
          
-         223           2 LOAD_CONST               1 (0)
+         235           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (None)
                        6 IMPORT_NAME              0 (json)
                        8 STORE_FAST               2 (json)
          
-         224          10 LOAD_CONST               1 (0)
+         236          10 LOAD_CONST               1 (0)
                       12 LOAD_CONST               3 (('logger',))
                       14 IMPORT_NAME              1 (loguru)
                       16 IMPORT_FROM              2 (logger)
                       18 STORE_FAST               3 (logger)
                       20 POP_TOP
          
-         225          22 LOAD_CONST               1 (0)
+         237          22 LOAD_CONST               1 (0)
                       24 LOAD_CONST               4 (('scan_ifdef_variables',))
                       26 IMPORT_NAME              3 (tucan.clean_ifdef)
                       28 IMPORT_FROM              4 (scan_ifdef_variables)
                       30 STORE_FAST               4 (scan_ifdef_variables)
                       32 POP_TOP
          
-         228          34 LOAD_GLOBAL             11 (NULL + open)
+         240          34 LOAD_GLOBAL             11 (NULL + open)
                       46 LOAD_FAST                0 (filename)
                       48 LOAD_CONST               5 ('r')
                       50 PRECALL                  2
                       54 CALL                     2
                       64 BEFORE_WITH
                       66 STORE_FAST               5 (fin)
          
-         229          68 LOAD_FAST                5 (fin)
+         241          68 LOAD_FAST                5 (fin)
                       70 LOAD_METHOD              6 (read)
                       92 PRECALL                  0
                       96 CALL                     0
                      106 LOAD_METHOD              7 (split)
                      128 LOAD_CONST               6 ('\n')
                      130 PRECALL                  1
                      134 CALL                     1
                      144 STORE_FAST               6 (lines)
          
-         228         146 LOAD_CONST               2 (None)
+         240         146 LOAD_CONST               2 (None)
                      148 LOAD_CONST               2 (None)
                      150 LOAD_CONST               2 (None)
                      152 PRECALL                  2
                      156 CALL                     2
                      166 POP_TOP
                      168 JUMP_FORWARD            11 (to 192)
                  >>  170 PUSH_EXC_INFO
@@ -1028,127 +1125,127 @@
                      180 POP_EXCEPT
                      182 RERAISE                  1
                  >>  184 POP_TOP
                      186 POP_EXCEPT
                      188 POP_TOP
                      190 POP_TOP
          
-         231     >>  192 PUSH_NULL
+         243     >>  192 PUSH_NULL
                      194 LOAD_FAST                4 (scan_ifdef_variables)
                      196 LOAD_FAST                6 (lines)
                      198 PRECALL                  1
                      202 CALL                     1
                      212 UNPACK_SEQUENCE          2
                      216 STORE_FAST               7 (gv_)
                      218 STORE_FAST               8 (lv_)
          
-         232         220 LOAD_CONST               7 (', ')
+         244         220 LOAD_CONST               7 (', ')
                      222 LOAD_METHOD              8 (join)
                      244 LOAD_FAST                7 (gv_)
                      246 PRECALL                  1
                      250 CALL                     1
                      260 STORE_FAST               9 (gv_s)
          
-         233         262 LOAD_CONST               7 (', ')
+         245         262 LOAD_CONST               7 (', ')
                      264 LOAD_METHOD              8 (join)
                      286 LOAD_FAST                8 (lv_)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 STORE_FAST              10 (lv_s)
          
-         235         304 LOAD_FAST                3 (logger)
+         247         304 LOAD_FAST                3 (logger)
                      306 LOAD_METHOD              9 (info)
                      328 LOAD_CONST               8 ('Global ifdef variables : ')
                      330 LOAD_FAST                9 (gv_s)
                      332 FORMAT_VALUE             0
                      334 BUILD_STRING             2
                      336 PRECALL                  1
                      340 CALL                     1
                      350 POP_TOP
          
-         236         352 LOAD_FAST                8 (lv_)
+         248         352 LOAD_FAST                8 (lv_)
                      354 POP_JUMP_FORWARD_IF_FALSE    25 (to 406)
          
-         237         356 LOAD_FAST                3 (logger)
+         249         356 LOAD_FAST                3 (logger)
                      358 LOAD_METHOD              9 (info)
                      380 LOAD_CONST               9 ('Found local ifdef variables : ')
                      382 LOAD_FAST               10 (lv_s)
                      384 FORMAT_VALUE             0
                      386 BUILD_STRING             2
                      388 PRECALL                  1
                      392 CALL                     1
                      402 POP_TOP
                      404 JUMP_FORWARD            21 (to 448)
          
-         239     >>  406 LOAD_FAST                3 (logger)
+         251     >>  406 LOAD_FAST                3 (logger)
                      408 LOAD_METHOD              9 (info)
                      430 LOAD_CONST              10 ('No local ifdef variables')
                      432 PRECALL                  1
                      436 CALL                     1
                      446 POP_TOP
          
-         241     >>  448 LOAD_FAST                1 (dump)
+         253     >>  448 LOAD_FAST                1 (dump)
                      450 POP_JUMP_FORWARD_IF_FALSE   154 (to 760)
          
-         242         452 LOAD_FAST                0 (filename)
+         254         452 LOAD_FAST                0 (filename)
                      454 LOAD_METHOD              7 (split)
                      476 LOAD_CONST              11 ('/')
                      478 PRECALL                  1
                      482 CALL                     1
                      492 LOAD_CONST              12 (-1)
                      494 BINARY_SUBSCR
                      504 LOAD_METHOD              7 (split)
                      526 LOAD_CONST              13 ('.')
                      528 PRECALL                  1
                      532 CALL                     1
                      542 LOAD_CONST               1 (0)
                      544 BINARY_SUBSCR
                      554 STORE_FAST              11 (base)
          
-         243         556 LOAD_FAST               11 (base)
+         255         556 LOAD_FAST               11 (base)
                      558 LOAD_CONST              14 ('_ifdefs.json')
                      560 BINARY_OP                0 (+)
                      564 STORE_FAST              12 (newfile)
          
-         244         566 LOAD_FAST                3 (logger)
+         256         566 LOAD_FAST                3 (logger)
                      568 LOAD_METHOD              9 (info)
                      590 LOAD_CONST              15 ('Data dumped to ')
                      592 LOAD_FAST               12 (newfile)
                      594 FORMAT_VALUE             0
                      596 BUILD_STRING             2
                      598 PRECALL                  1
                      602 CALL                     1
                      612 POP_TOP
          
-         245         614 LOAD_FAST                7 (gv_)
+         257         614 LOAD_FAST                7 (gv_)
                      616 LOAD_FAST                8 (lv_)
                      618 LOAD_CONST              16 (('global', 'local'))
                      620 BUILD_CONST_KEY_MAP      2
                      622 STORE_FAST              13 (out)
          
-         246         624 LOAD_GLOBAL             11 (NULL + open)
+         258         624 LOAD_GLOBAL             11 (NULL + open)
                      636 LOAD_FAST               12 (newfile)
                      638 LOAD_CONST              17 ('w')
                      640 PRECALL                  2
                      644 CALL                     2
                      654 BEFORE_WITH
                      656 STORE_FAST              14 (fout)
          
-         247         658 LOAD_FAST                2 (json)
+         259         658 LOAD_FAST                2 (json)
                      660 LOAD_METHOD             10 (dump)
                      682 LOAD_FAST               13 (out)
                      684 LOAD_FAST               14 (fout)
                      686 LOAD_CONST              18 (2)
                      688 LOAD_CONST              19 (True)
                      690 KW_NAMES                20
                      692 PRECALL                  4
                      696 CALL                     4
                      706 POP_TOP
          
-         246         708 LOAD_CONST               2 (None)
+         258         708 LOAD_CONST               2 (None)
                      710 LOAD_CONST               2 (None)
                      712 LOAD_CONST               2 (None)
                      714 PRECALL                  2
                      718 CALL                     2
                      728 POP_TOP
                      730 LOAD_CONST               2 (None)
                      732 RETURN_VALUE
@@ -1162,15 +1259,15 @@
                  >>  748 POP_TOP
                      750 POP_EXCEPT
                      752 POP_TOP
                      754 POP_TOP
                      756 LOAD_CONST               2 (None)
                      758 RETURN_VALUE
          
-         241     >>  760 LOAD_CONST               2 (None)
+         253     >>  760 LOAD_CONST               2 (None)
                      762 RETURN_VALUE
          ExceptionTable:
            66 to 144 -> 170 [1] lasti
            170 to 176 -> 178 [3] lasti
            184 to 184 -> 178 [3] lasti
            656 to 706 -> 734 [1] lasti
            734 to 740 -> 742 [3] lasti
@@ -1199,263 +1296,260 @@
             ('indent', 'sort_keys')
          names      ('json', 'loguru', 'logger', 'tucan.clean_ifdef', 'scan_ifdef_variables', 'open', 'read', 'split', 'join', 'info', 'dump')
          varnames   ('filename', 'dump', 'json', 'logger', 'scan_ifdef_variables', 'fin', 'lines', 'gv_', 'lv_', 'gv_s', 'lv_s', 'base', 'newfile', 'out', 'fout')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/cli.py'
          name       'ifdef_scan'
-         firstlineno 211
+         firstlineno 223
          lnotab
             0x020c08010c010c0322014eff2e031c012a012a023001040132022a0204
             0168010a0130010a01220132ff34fb
-      '-v'
-      '--variables'
-      "Variable to resolve ifdefs. Comma separated ',', no spaces : -v ARG1,ARG2"
+      '-def'
+      '--definitions'
+      "definitions to resolve ifdefs. Comma separated ',', no spaces : -v ARG1,ARG2"
       ('type', 'default', 'help')
+      '-f'
+      '--fortran'
+      ' fortran mode (avoid  stripping //)'
+      'verbose execution'
       code
-         argcount  : 3
-         nlocals   : 11
+         argcount  : 5
+         nlocals   : 13
          stacksize : 6
          flags     : 3
          code
-            0x9700640164026c006d017d030100640164036c026d037d0401007c03a0
-            0400000000000000000000000000000000000000007c01a6010000ab0100
-            0000000000000001007c01800367007d016e157c01a00500000000000000
-            000000000000000000000000006405a6010000ab0100000000000000007d
-            017c03a00400000000000000000000000000000000000000007c01a60100
-            00ab0100000000000000000100740d000000000000000000007c006406a6
-            020000ab02000000000000000035007d057c05a007000000000000000000
-            0000000000000000000000a6000000ab000000000000000000a005000000
-            00000000000000000000000000000000006407a6010000ab010000000000
-            0000007d06640464046404a6020000ab02000000000000000001006e0b23
-            00310073047702780359007701010059000100010002007c047c067c01a6
-            020000ab0200000000000000007d067c03a0080000000000000000000000
-            0000000000000000006408a6010000ab01000000000000000001007c0644
-            005d117d077413000000000000000000007c07a6010000ab010000000000
-            00000001008c127c0272877c0064097a0000007d087c06a00a0000000000
-            000000000000000000000000000000640aa6010000ab0100000000000000
-            000100640ba00b00000000000000000000000000000000000000007c01a6
-            010000ab0100000000000000007d097c06a00a0000000000000000000000
-            000000000000000000640c7c019b009d02a6010000ab0100000000000000
-            000100740d000000000000000000007c08640da6020000ab020000000000
-            00000035007d0a7c0aa00c00000000000000000000000000000000000000
-            007c06a6010000ab0100000000000000000100640464046404a6020000ab
-            020000000000000000010064045300230031007304770278035900770101
-            005900010001006404530064045300
-         252           0 RESUME                   0
+            0x9700640164026c006d017d050100640164036c026d037d0601007c0180
+            0367007d016e157c01a00400000000000000000000000000000000000000
+            006405a6010000ab0100000000000000007d01740b000000000000000000
+            007c006406a6020000ab02000000000000000035007d077c07a006000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            00a00400000000000000000000000000000000000000006407a6010000ab
+            0100000000000000007d08640464046404a6020000ab0200000000000000
+            0001006e0b2300310073047702780359007701010059000100010002007c
+            067c087c017c047c03ac08a6040000ab0400000000000000007d087c05a0
+            0700000000000000000000000000000000000000006409a6010000ab0100
+            0000000000000001007c0844005d117d097411000000000000000000007c
+            09a6010000ab01000000000000000001008c127c02729a7c00640a7a0000
+            007d0a7c08a0090000000000000000000000000000000000000000640ba6
+            010000ab0100000000000000000100640ca00a0000000000000000000000
+            0000000000000000007c01a6010000ab0100000000000000007d0b7c08a0
+            090000000000000000000000000000000000000000640d7c019b009d02a6
+            010000ab0100000000000000000100740b000000000000000000007c0a64
+            0ea6020000ab02000000000000000035007d0c7c0ca00b00000000000000
+            000000000000000000000000006407a00a00000000000000000000000000
+            000000000000007c08a6010000ab010000000000000000a6010000ab0100
+            000000000000000100640464046404a6020000ab02000000000000000001
+            006404530023003100730477027803590077010100590001000100640453
+            0064045300
+         264           0 RESUME                   0
          
-         272           2 LOAD_CONST               1 (0)
+         296           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (('logger',))
                        6 IMPORT_NAME              0 (loguru)
                        8 IMPORT_FROM              1 (logger)
-                      10 STORE_FAST               3 (logger)
+                      10 STORE_FAST               5 (logger)
                       12 POP_TOP
          
-         273          14 LOAD_CONST               1 (0)
+         297          14 LOAD_CONST               1 (0)
                       16 LOAD_CONST               3 (('remove_ifdef_from_module',))
                       18 IMPORT_NAME              2 (tucan.clean_ifdef)
                       20 IMPORT_FROM              3 (remove_ifdef_from_module)
-                      22 STORE_FAST               4 (remove_ifdef_from_module)
+                      22 STORE_FAST               6 (remove_ifdef_from_module)
                       24 POP_TOP
          
-         274          26 LOAD_FAST                3 (logger)
-                      28 LOAD_METHOD              4 (critical)
-                      50 LOAD_FAST                1 (variables)
-                      52 PRECALL                  1
-                      56 CALL                     1
-                      66 POP_TOP
+         299          26 LOAD_FAST                1 (definitions)
+                      28 POP_JUMP_FORWARD_IF_NOT_NONE     3 (to 36)
          
-         276          68 LOAD_FAST                1 (variables)
-                      70 POP_JUMP_FORWARD_IF_NOT_NONE     3 (to 78)
+         300          30 BUILD_LIST               0
+                      32 STORE_FAST               1 (definitions)
+                      34 JUMP_FORWARD            21 (to 78)
+         
+         302     >>   36 LOAD_FAST                1 (definitions)
+                      38 LOAD_METHOD              4 (split)
+                      60 LOAD_CONST               5 (',')
+                      62 PRECALL                  1
+                      66 CALL                     1
+                      76 STORE_FAST               1 (definitions)
          
-         277          72 BUILD_LIST               0
-                      74 STORE_FAST               1 (variables)
-                      76 JUMP_FORWARD            21 (to 120)
-         
-         279     >>   78 LOAD_FAST                1 (variables)
-                      80 LOAD_METHOD              5 (split)
-                     102 LOAD_CONST               5 (',')
-                     104 PRECALL                  1
-                     108 CALL                     1
-                     118 STORE_FAST               1 (variables)
-         
-         281     >>  120 LOAD_FAST                3 (logger)
-                     122 LOAD_METHOD              4 (critical)
-                     144 LOAD_FAST                1 (variables)
-                     146 PRECALL                  1
-                     150 CALL                     1
-                     160 POP_TOP
-         
-         282         162 LOAD_GLOBAL             13 (NULL + open)
-                     174 LOAD_FAST                0 (filename)
-                     176 LOAD_CONST               6 ('r')
-                     178 PRECALL                  2
-                     182 CALL                     2
-                     192 BEFORE_WITH
-                     194 STORE_FAST               5 (fin)
-         
-         283         196 LOAD_FAST                5 (fin)
-                     198 LOAD_METHOD              7 (read)
-                     220 PRECALL                  0
-                     224 CALL                     0
-                     234 LOAD_METHOD              5 (split)
-                     256 LOAD_CONST               7 ('\n')
-                     258 PRECALL                  1
-                     262 CALL                     1
-                     272 STORE_FAST               6 (lines)
-         
-         282         274 LOAD_CONST               4 (None)
-                     276 LOAD_CONST               4 (None)
-                     278 LOAD_CONST               4 (None)
-                     280 PRECALL                  2
-                     284 CALL                     2
-                     294 POP_TOP
-                     296 JUMP_FORWARD            11 (to 320)
-                 >>  298 PUSH_EXC_INFO
-                     300 WITH_EXCEPT_START
-                     302 POP_JUMP_FORWARD_IF_TRUE     4 (to 312)
-                     304 RERAISE                  2
-                 >>  306 COPY                     3
-                     308 POP_EXCEPT
-                     310 RERAISE                  1
-                 >>  312 POP_TOP
-                     314 POP_EXCEPT
-                     316 POP_TOP
-                     318 POP_TOP
-         
-         285     >>  320 PUSH_NULL
-                     322 LOAD_FAST                4 (remove_ifdef_from_module)
-                     324 LOAD_FAST                6 (lines)
-                     326 LOAD_FAST                1 (variables)
-                     328 PRECALL                  2
-                     332 CALL                     2
-                     342 STORE_FAST               6 (lines)
-         
-         287         344 LOAD_FAST                3 (logger)
-                     346 LOAD_METHOD              8 (success)
-                     368 LOAD_CONST               8 ('Ifdefs resolved:')
-                     370 PRECALL                  1
-                     374 CALL                     1
-                     384 POP_TOP
+         304     >>   78 LOAD_GLOBAL             11 (NULL + open)
+                      90 LOAD_FAST                0 (filename)
+                      92 LOAD_CONST               6 ('r')
+                      94 PRECALL                  2
+                      98 CALL                     2
+                     108 BEFORE_WITH
+                     110 STORE_FAST               7 (fin)
+         
+         305         112 LOAD_FAST                7 (fin)
+                     114 LOAD_METHOD              6 (read)
+                     136 PRECALL                  0
+                     140 CALL                     0
+                     150 LOAD_METHOD              4 (split)
+                     172 LOAD_CONST               7 ('\n')
+                     174 PRECALL                  1
+                     178 CALL                     1
+                     188 STORE_FAST               8 (lines)
+         
+         304         190 LOAD_CONST               4 (None)
+                     192 LOAD_CONST               4 (None)
+                     194 LOAD_CONST               4 (None)
+                     196 PRECALL                  2
+                     200 CALL                     2
+                     210 POP_TOP
+                     212 JUMP_FORWARD            11 (to 236)
+                 >>  214 PUSH_EXC_INFO
+                     216 WITH_EXCEPT_START
+                     218 POP_JUMP_FORWARD_IF_TRUE     4 (to 228)
+                     220 RERAISE                  2
+                 >>  222 COPY                     3
+                     224 POP_EXCEPT
+                     226 RERAISE                  1
+                 >>  228 POP_TOP
+                     230 POP_EXCEPT
+                     232 POP_TOP
+                     234 POP_TOP
+         
+         306     >>  236 PUSH_NULL
+                     238 LOAD_FAST                6 (remove_ifdef_from_module)
+                     240 LOAD_FAST                8 (lines)
+                     242 LOAD_FAST                1 (definitions)
+                     244 LOAD_FAST                4 (verbose)
+                     246 LOAD_FAST                3 (fortran)
+                     248 KW_NAMES                 8
+                     250 PRECALL                  4
+                     254 CALL                     4
+                     264 STORE_FAST               8 (lines)
+         
+         307         266 LOAD_FAST                5 (logger)
+                     268 LOAD_METHOD              7 (success)
+                     290 LOAD_CONST               9 ('Ifdefs resolved:')
+                     292 PRECALL                  1
+                     296 CALL                     1
+                     306 POP_TOP
+         
+         308         308 LOAD_FAST                8 (lines)
+                     310 GET_ITER
+                 >>  312 FOR_ITER                17 (to 348)
+                     314 STORE_FAST               9 (line)
+         
+         309         316 LOAD_GLOBAL             17 (NULL + print)
+                     328 LOAD_FAST                9 (line)
+                     330 PRECALL                  1
+                     334 CALL                     1
+                     344 POP_TOP
+                     346 JUMP_BACKWARD           18 (to 312)
+         
+         310     >>  348 LOAD_FAST                2 (dump)
+                     350 POP_JUMP_FORWARD_IF_FALSE   154 (to 660)
+         
+         311         352 LOAD_FAST                0 (filename)
+                     354 LOAD_CONST              10 ('_ifdef_resolved')
+                     356 BINARY_OP                0 (+)
+                     360 STORE_FAST              10 (newfile)
+         
+         312         362 LOAD_FAST                8 (lines)
+                     364 LOAD_METHOD              9 (append)
+                     386 LOAD_CONST              11 ('# the ifdefs were resolved by tucan')
+                     388 PRECALL                  1
+                     392 CALL                     1
+                     402 POP_TOP
+         
+         313         404 LOAD_CONST              12 (', ')
+                     406 LOAD_METHOD             10 (join)
+                     428 LOAD_FAST                1 (definitions)
+                     430 PRECALL                  1
+                     434 CALL                     1
+                     444 STORE_FAST              11 (v_s)
+         
+         314         446 LOAD_FAST                8 (lines)
+                     448 LOAD_METHOD              9 (append)
+                     470 LOAD_CONST              13 ('# IFdef Variables: ')
+                     472 LOAD_FAST                1 (definitions)
+                     474 FORMAT_VALUE             0
+                     476 BUILD_STRING             2
+                     478 PRECALL                  1
+                     482 CALL                     1
+                     492 POP_TOP
          
-         288         386 LOAD_FAST                6 (lines)
-                     388 GET_ITER
-                 >>  390 FOR_ITER                17 (to 426)
-                     392 STORE_FAST               7 (line)
-         
-         289         394 LOAD_GLOBAL             19 (NULL + print)
-                     406 LOAD_FAST                7 (line)
-                     408 PRECALL                  1
-                     412 CALL                     1
-                     422 POP_TOP
-                     424 JUMP_BACKWARD           18 (to 390)
-         
-         290     >>  426 LOAD_FAST                2 (dump)
-                     428 POP_JUMP_FORWARD_IF_FALSE   135 (to 700)
-         
-         291         430 LOAD_FAST                0 (filename)
-                     432 LOAD_CONST               9 ('_ifdef_resolved')
-                     434 BINARY_OP                0 (+)
-                     438 STORE_FAST               8 (newfile)
-         
-         292         440 LOAD_FAST                6 (lines)
-                     442 LOAD_METHOD             10 (append)
-                     464 LOAD_CONST              10 ('# the ifdefs were resolved by tucan')
-                     466 PRECALL                  1
-                     470 CALL                     1
-                     480 POP_TOP
-         
-         293         482 LOAD_CONST              11 (', ')
-                     484 LOAD_METHOD             11 (join)
-                     506 LOAD_FAST                1 (variables)
-                     508 PRECALL                  1
-                     512 CALL                     1
-                     522 STORE_FAST               9 (v_s)
-         
-         294         524 LOAD_FAST                6 (lines)
-                     526 LOAD_METHOD             10 (append)
-                     548 LOAD_CONST              12 ('# IFdef Variables: ')
-                     550 LOAD_FAST                1 (variables)
-                     552 FORMAT_VALUE             0
-                     554 BUILD_STRING             2
-                     556 PRECALL                  1
-                     560 CALL                     1
-                     570 POP_TOP
-         
-         295         572 LOAD_GLOBAL             13 (NULL + open)
-                     584 LOAD_FAST                8 (newfile)
-                     586 LOAD_CONST              13 ('w')
-                     588 PRECALL                  2
-                     592 CALL                     2
-                     602 BEFORE_WITH
-                     604 STORE_FAST              10 (fout)
-         
-         296         606 LOAD_FAST               10 (fout)
-                     608 LOAD_METHOD             12 (writelines)
-                     630 LOAD_FAST                6 (lines)
-                     632 PRECALL                  1
-                     636 CALL                     1
-                     646 POP_TOP
-         
-         295         648 LOAD_CONST               4 (None)
-                     650 LOAD_CONST               4 (None)
-                     652 LOAD_CONST               4 (None)
-                     654 PRECALL                  2
-                     658 CALL                     2
-                     668 POP_TOP
-                     670 LOAD_CONST               4 (None)
-                     672 RETURN_VALUE
-                 >>  674 PUSH_EXC_INFO
-                     676 WITH_EXCEPT_START
-                     678 POP_JUMP_FORWARD_IF_TRUE     4 (to 688)
-                     680 RERAISE                  2
-                 >>  682 COPY                     3
-                     684 POP_EXCEPT
-                     686 RERAISE                  1
-                 >>  688 POP_TOP
-                     690 POP_EXCEPT
-                     692 POP_TOP
-                     694 POP_TOP
-                     696 LOAD_CONST               4 (None)
-                     698 RETURN_VALUE
+         315         494 LOAD_GLOBAL             11 (NULL + open)
+                     506 LOAD_FAST               10 (newfile)
+                     508 LOAD_CONST              14 ('w')
+                     510 PRECALL                  2
+                     514 CALL                     2
+                     524 BEFORE_WITH
+                     526 STORE_FAST              12 (fout)
+         
+         316         528 LOAD_FAST               12 (fout)
+                     530 LOAD_METHOD             11 (write)
+                     552 LOAD_CONST               7 ('\n')
+                     554 LOAD_METHOD             10 (join)
+                     576 LOAD_FAST                8 (lines)
+                     578 PRECALL                  1
+                     582 CALL                     1
+                     592 PRECALL                  1
+                     596 CALL                     1
+                     606 POP_TOP
+         
+         315         608 LOAD_CONST               4 (None)
+                     610 LOAD_CONST               4 (None)
+                     612 LOAD_CONST               4 (None)
+                     614 PRECALL                  2
+                     618 CALL                     2
+                     628 POP_TOP
+                     630 LOAD_CONST               4 (None)
+                     632 RETURN_VALUE
+                 >>  634 PUSH_EXC_INFO
+                     636 WITH_EXCEPT_START
+                     638 POP_JUMP_FORWARD_IF_TRUE     4 (to 648)
+                     640 RERAISE                  2
+                 >>  642 COPY                     3
+                     644 POP_EXCEPT
+                     646 RERAISE                  1
+                 >>  648 POP_TOP
+                     650 POP_EXCEPT
+                     652 POP_TOP
+                     654 POP_TOP
+                     656 LOAD_CONST               4 (None)
+                     658 RETURN_VALUE
          
-         290     >>  700 LOAD_CONST               4 (None)
-                     702 RETURN_VALUE
+         310     >>  660 LOAD_CONST               4 (None)
+                     662 RETURN_VALUE
          ExceptionTable:
-           194 to 272 -> 298 [1] lasti
-           298 to 304 -> 306 [3] lasti
-           312 to 312 -> 306 [3] lasti
-           604 to 646 -> 674 [1] lasti
-           674 to 680 -> 682 [3] lasti
-           688 to 688 -> 682 [3] lasti
+           110 to 188 -> 214 [1] lasti
+           214 to 220 -> 222 [3] lasti
+           228 to 228 -> 222 [3] lasti
+           526 to 606 -> 634 [1] lasti
+           634 to 640 -> 642 [3] lasti
+           648 to 648 -> 642 [3] lasti
          consts
             '\n    Show a file with idefs resolved\n    '
             0
             ('logger',)
             ('remove_ifdef_from_module',)
             None
             ','
             'r'
             '\n'
+            ('verbose', 'fortran')
             'Ifdefs resolved:'
             '_ifdef_resolved'
             '# the ifdefs were resolved by tucan'
             ', '
             '# IFdef Variables: '
             'w'
-         names      ('loguru', 'logger', 'tucan.clean_ifdef', 'remove_ifdef_from_module', 'critical', 'split', 'open', 'read', 'success', 'print', 'append', 'join', 'writelines')
-         varnames   ('filename', 'variables', 'dump', 'logger', 'remove_ifdef_from_module', 'fin', 'lines', 'line', 'newfile', 'v_s', 'fout')
+         names      ('loguru', 'logger', 'tucan.clean_ifdef', 'remove_ifdef_from_module', 'split', 'open', 'read', 'success', 'print', 'append', 'join', 'write')
+         varnames   ('filename', 'definitions', 'dump', 'fortran', 'verbose', 'logger', 'remove_ifdef_from_module', 'fin', 'lines', 'line', 'newfile', 'v_s', 'fout')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/cli.py'
          name       'ifdef_clean'
-         firstlineno 252
+         firstlineno 264
          lnotab
-            0x02140c010c012a02040106022a022a0122014eff2e0318022a01080120
-            0104010a012a012a01300122012aff34fb
+            0x02200c010c02040106022a0222014eff2e021e012a010801200104010a
+            012a012a013001220150ff34fb
       'path'
       code
          argcount  : 2
          nlocals   : 17
          stacksize : 7
          flags     : 3
          code
@@ -1479,180 +1573,180 @@
             008c387c0172617c00640e7a0000007d0f7c04a009000000000000000000
             0000000000000000000000640f7c0f9b009d02a6010000ab010000000000
             0000000100741b000000000000000000007c0f6410a6020000ab02000000
             000000000035007d107c02a00e0000000000000000000000000000000000
             0000007c0a7c1064116412ac13a6040000ab040000000000000000010064
             0264026402a6020000ab0200000000000000000100640253002300310073
             04770278035900770101005900010001006402530064025300
-         298           0 RESUME                   0
+         318           0 RESUME                   0
          
-         310           2 LOAD_CONST               1 (0)
+         330           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (None)
                        6 IMPORT_NAME              0 (json)
                        8 STORE_FAST               2 (json)
                       10 LOAD_CONST               1 (0)
                       12 LOAD_CONST               2 (None)
                       14 IMPORT_NAME              1 (os)
                       16 STORE_FAST               3 (os)
          
-         311          18 LOAD_CONST               1 (0)
+         331          18 LOAD_CONST               1 (0)
                       20 LOAD_CONST               3 (('logger',))
                       22 IMPORT_NAME              2 (loguru)
                       24 IMPORT_FROM              3 (logger)
                       26 STORE_FAST               4 (logger)
                       28 POP_TOP
          
-         312          30 LOAD_CONST               1 (0)
+         332          30 LOAD_CONST               1 (0)
                       32 LOAD_CONST               4 (('run_ifdef_pkg_analysis',))
                       34 IMPORT_NAME              4 (tucan.clean_ifdef)
                       36 IMPORT_FROM              5 (run_ifdef_pkg_analysis)
                       38 STORE_FAST               5 (run_ifdef_pkg_analysis)
                       40 POP_TOP
          
-         313          42 LOAD_CONST               1 (0)
+         333          42 LOAD_CONST               1 (0)
                       44 LOAD_CONST               5 (('rec_travel_through_package', 'get_package_files'))
                       46 IMPORT_NAME              6 (tucan.package_analysis)
                       48 IMPORT_FROM              7 (rec_travel_through_package)
                       50 STORE_FAST               6 (rec_travel_through_package)
                       52 IMPORT_FROM              8 (get_package_files)
                       54 STORE_FAST               7 (get_package_files)
                       56 POP_TOP
          
-         318          58 LOAD_FAST                4 (logger)
+         338          58 LOAD_FAST                4 (logger)
                       60 LOAD_METHOD              9 (info)
                       82 LOAD_CONST               6 ('Recursive path gathering ...')
                       84 PRECALL                  1
                       88 CALL                     1
                       98 POP_TOP
          
-         319         100 PUSH_NULL
+         339         100 PUSH_NULL
                      102 LOAD_FAST                6 (rec_travel_through_package)
                      104 LOAD_FAST                0 (path)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               8 (paths)
          
-         320         122 LOAD_FAST                4 (logger)
+         340         122 LOAD_FAST                4 (logger)
                      124 LOAD_METHOD              9 (info)
                      146 LOAD_CONST               7 ('Cleaning the paths ...')
                      148 PRECALL                  1
                      152 CALL                     1
                      162 POP_TOP
          
-         321         164 PUSH_NULL
+         341         164 PUSH_NULL
                      166 LOAD_FAST                7 (get_package_files)
                      168 LOAD_FAST                8 (paths)
                      170 LOAD_FAST                3 (os)
                      172 LOAD_METHOD             10 (getcwd)
                      194 PRECALL                  0
                      198 CALL                     0
                      208 PRECALL                  2
                      212 CALL                     2
                      222 STORE_FAST               9 (files)
          
-         324         224 PUSH_NULL
+         344         224 PUSH_NULL
                      226 LOAD_FAST                5 (run_ifdef_pkg_analysis)
                      228 LOAD_FAST                9 (files)
                      230 PRECALL                  1
                      234 CALL                     1
                      244 STORE_FAST              10 (out)
          
-         325         246 LOAD_CONST               8 (', ')
+         345         246 LOAD_CONST               8 (', ')
                      248 LOAD_METHOD             11 (join)
                      270 LOAD_FAST               10 (out)
                      272 LOAD_CONST               9 ('global')
                      274 BINARY_SUBSCR
                      284 PRECALL                  1
                      288 CALL                     1
                      298 STORE_FAST              11 (gv_s)
          
-         326         300 LOAD_FAST                4 (logger)
+         346         300 LOAD_FAST                4 (logger)
                      302 LOAD_METHOD              9 (info)
                      324 LOAD_CONST              10 ('Global ifdef variables : ')
                      326 LOAD_FAST               11 (gv_s)
                      328 FORMAT_VALUE             0
                      330 BUILD_STRING             2
                      332 PRECALL                  1
                      336 CALL                     1
                      346 POP_TOP
          
-         327         348 LOAD_FAST               10 (out)
+         347         348 LOAD_FAST               10 (out)
                      350 LOAD_CONST              11 ('local')
                      352 BINARY_SUBSCR
                      362 LOAD_METHOD             12 (items)
                      384 PRECALL                  0
                      388 CALL                     0
                      398 GET_ITER
                  >>  400 FOR_ITER                55 (to 512)
                      402 UNPACK_SEQUENCE          2
                      406 STORE_FAST              12 (file)
                      408 STORE_FAST              13 (lv_)
          
-         328         410 LOAD_FAST               13 (lv_)
+         348         410 LOAD_FAST               13 (lv_)
                      412 POP_JUMP_FORWARD_IF_FALSE    48 (to 510)
          
-         329         414 LOAD_CONST               8 (', ')
+         349         414 LOAD_CONST               8 (', ')
                      416 LOAD_METHOD             11 (join)
                      438 LOAD_FAST               13 (lv_)
                      440 PRECALL                  1
                      444 CALL                     1
                      454 STORE_FAST              14 (lv_s)
          
-         330         456 LOAD_FAST                4 (logger)
+         350         456 LOAD_FAST                4 (logger)
                      458 LOAD_METHOD              9 (info)
                      480 LOAD_CONST              12 ('Local to ')
                      482 LOAD_FAST               12 (file)
                      484 FORMAT_VALUE             0
                      486 LOAD_CONST              13 (' : ')
                      488 LOAD_FAST               14 (lv_s)
                      490 FORMAT_VALUE             0
                      492 BUILD_STRING             4
                      494 PRECALL                  1
                      498 CALL                     1
                      508 POP_TOP
                  >>  510 JUMP_BACKWARD           56 (to 400)
          
-         332     >>  512 LOAD_FAST                1 (dump)
+         352     >>  512 LOAD_FAST                1 (dump)
                      514 POP_JUMP_FORWARD_IF_FALSE    97 (to 710)
          
-         333         516 LOAD_FAST                0 (path)
+         353         516 LOAD_FAST                0 (path)
                      518 LOAD_CONST              14 ('package_ifdefs.json')
                      520 BINARY_OP                0 (+)
                      524 STORE_FAST              15 (newfile)
          
-         334         526 LOAD_FAST                4 (logger)
+         354         526 LOAD_FAST                4 (logger)
                      528 LOAD_METHOD              9 (info)
                      550 LOAD_CONST              15 ('Data dumped to ')
                      552 LOAD_FAST               15 (newfile)
                      554 FORMAT_VALUE             0
                      556 BUILD_STRING             2
                      558 PRECALL                  1
                      562 CALL                     1
                      572 POP_TOP
          
-         335         574 LOAD_GLOBAL             27 (NULL + open)
+         355         574 LOAD_GLOBAL             27 (NULL + open)
                      586 LOAD_FAST               15 (newfile)
                      588 LOAD_CONST              16 ('w')
                      590 PRECALL                  2
                      594 CALL                     2
                      604 BEFORE_WITH
                      606 STORE_FAST              16 (fout)
          
-         336         608 LOAD_FAST                2 (json)
+         356         608 LOAD_FAST                2 (json)
                      610 LOAD_METHOD             14 (dump)
                      632 LOAD_FAST               10 (out)
                      634 LOAD_FAST               16 (fout)
                      636 LOAD_CONST              17 (2)
                      638 LOAD_CONST              18 (True)
                      640 KW_NAMES                19
                      642 PRECALL                  4
                      646 CALL                     4
                      656 POP_TOP
          
-         335         658 LOAD_CONST               2 (None)
+         355         658 LOAD_CONST               2 (None)
                      660 LOAD_CONST               2 (None)
                      662 LOAD_CONST               2 (None)
                      664 PRECALL                  2
                      668 CALL                     2
                      678 POP_TOP
                      680 LOAD_CONST               2 (None)
                      682 RETURN_VALUE
@@ -1666,15 +1760,15 @@
                  >>  698 POP_TOP
                      700 POP_EXCEPT
                      702 POP_TOP
                      704 POP_TOP
                      706 LOAD_CONST               2 (None)
                      708 RETURN_VALUE
          
-         332     >>  710 LOAD_CONST               2 (None)
+         352     >>  710 LOAD_CONST               2 (None)
                      712 RETURN_VALUE
          ExceptionTable:
            606 to 656 -> 684 [1] lasti
            684 to 690 -> 692 [3] lasti
            698 to 698 -> 692 [3] lasti
          consts
             '\n    Extract Ifdef variables of a single file.\n    '
@@ -1699,15 +1793,15 @@
             ('indent', 'sort_keys')
          names      ('json', 'os', 'loguru', 'logger', 'tucan.clean_ifdef', 'run_ifdef_pkg_analysis', 'tucan.package_analysis', 'rec_travel_through_package', 'get_package_files', 'info', 'getcwd', 'join', 'items', 'open', 'dump')
          varnames   ('path', 'dump', 'json', 'os', 'logger', 'run_ifdef_pkg_analysis', 'rec_travel_through_package', 'get_package_files', 'paths', 'files', 'out', 'gv_s', 'file', 'lv_', 'lv_s', 'newfile', 'fout')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/cli.py'
          name       'ifdef_scan_pkge'
-         firstlineno 298
+         firstlineno 318
          lnotab
             0x020c10010c010c0110052a0116012a013c031601360130013e0104012a
             01380204010a013001220132ff34fd
       code
          argcount  : 1
          nlocals   : 12
          stacksize : 7
@@ -1725,122 +1819,122 @@
             0100000000000000007d0964087d0a7c04a0080000000000000000000000
             00000000000000000064097c0a9b009d02a6010000ab0100000000000000
             0001007415000000000000000000007c0a640aa6020000ab020000000000
             00000035007d0b7c05a00b00000000000000000000000000000000000000
             007c097c0b640b640cac0da6040000ab0400000000000000000100640464
             046404a6020000ab02000000000000000001006404530023003100730477
             02780359007701010059000100010064045300
-         364           0 RESUME                   0
+         384           0 RESUME                   0
          
-         370           2 LOAD_CONST               1 (0)
+         390           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (('rec_travel_through_package', 'get_package_files', 'run_full_analysis'))
                        6 IMPORT_NAME              0 (tucan.package_analysis)
                        8 IMPORT_FROM              1 (rec_travel_through_package)
                       10 STORE_FAST               1 (rec_travel_through_package)
                       12 IMPORT_FROM              2 (get_package_files)
                       14 STORE_FAST               2 (get_package_files)
                       16 IMPORT_FROM              3 (run_full_analysis)
                       18 STORE_FAST               3 (run_full_analysis)
                       20 POP_TOP
          
-         375          22 LOAD_CONST               1 (0)
+         395          22 LOAD_CONST               1 (0)
                       24 LOAD_CONST               3 (('logger',))
                       26 IMPORT_NAME              4 (loguru)
                       28 IMPORT_FROM              5 (logger)
                       30 STORE_FAST               4 (logger)
                       32 POP_TOP
          
-         376          34 LOAD_CONST               1 (0)
+         396          34 LOAD_CONST               1 (0)
                       36 LOAD_CONST               4 (None)
                       38 IMPORT_NAME              6 (json)
                       40 STORE_FAST               5 (json)
                       42 LOAD_CONST               1 (0)
                       44 LOAD_CONST               4 (None)
                       46 IMPORT_NAME              7 (os)
                       48 STORE_FAST               6 (os)
          
-         378          50 LOAD_FAST                4 (logger)
+         398          50 LOAD_FAST                4 (logger)
                       52 LOAD_METHOD              8 (info)
                       74 LOAD_CONST               5 ('Recursive path gathering ...')
                       76 PRECALL                  1
                       80 CALL                     1
                       90 POP_TOP
          
-         379          92 PUSH_NULL
+         399          92 PUSH_NULL
                       94 LOAD_FAST                1 (rec_travel_through_package)
                       96 LOAD_FAST                0 (path)
                       98 PRECALL                  1
                      102 CALL                     1
                      112 STORE_FAST               7 (paths)
          
-         380         114 LOAD_FAST                4 (logger)
+         400         114 LOAD_FAST                4 (logger)
                      116 LOAD_METHOD              8 (info)
                      138 LOAD_CONST               6 ('Get files ...')
                      140 PRECALL                  1
                      144 CALL                     1
                      154 POP_TOP
          
-         381         156 PUSH_NULL
+         401         156 PUSH_NULL
                      158 LOAD_FAST                2 (get_package_files)
                      160 LOAD_FAST                7 (paths)
                      162 LOAD_FAST                6 (os)
                      164 LOAD_METHOD              9 (getcwd)
                      186 PRECALL                  0
                      190 CALL                     0
                      200 PRECALL                  2
                      204 CALL                     2
                      214 STORE_FAST               8 (files)
          
-         382         216 LOAD_FAST                4 (logger)
+         402         216 LOAD_FAST                4 (logger)
                      218 LOAD_METHOD              8 (info)
                      240 LOAD_CONST               7 ('Running struct ...')
                      242 PRECALL                  1
                      246 CALL                     1
                      256 POP_TOP
          
-         383         258 PUSH_NULL
+         403         258 PUSH_NULL
                      260 LOAD_FAST                3 (run_full_analysis)
                      262 LOAD_FAST                8 (files)
                      264 PRECALL                  1
                      268 CALL                     1
                      278 STORE_FAST               9 (full_analysis)
          
-         385         280 LOAD_CONST               8 ('package_analysis.json')
+         405         280 LOAD_CONST               8 ('package_analysis.json')
                      282 STORE_FAST              10 (newfile)
          
-         386         284 LOAD_FAST                4 (logger)
+         406         284 LOAD_FAST                4 (logger)
                      286 LOAD_METHOD              8 (info)
                      308 LOAD_CONST               9 ('Data dumped to ')
                      310 LOAD_FAST               10 (newfile)
                      312 FORMAT_VALUE             0
                      314 BUILD_STRING             2
                      316 PRECALL                  1
                      320 CALL                     1
                      330 POP_TOP
          
-         387         332 LOAD_GLOBAL             21 (NULL + open)
+         407         332 LOAD_GLOBAL             21 (NULL + open)
                      344 LOAD_FAST               10 (newfile)
                      346 LOAD_CONST              10 ('w')
                      348 PRECALL                  2
                      352 CALL                     2
                      362 BEFORE_WITH
                      364 STORE_FAST              11 (fout)
          
-         388         366 LOAD_FAST                5 (json)
+         408         366 LOAD_FAST                5 (json)
                      368 LOAD_METHOD             11 (dump)
                      390 LOAD_FAST                9 (full_analysis)
                      392 LOAD_FAST               11 (fout)
                      394 LOAD_CONST              11 (2)
                      396 LOAD_CONST              12 (True)
                      398 KW_NAMES                13
                      400 PRECALL                  4
                      404 CALL                     4
                      414 POP_TOP
          
-         387         416 LOAD_CONST               4 (None)
+         407         416 LOAD_CONST               4 (None)
                      418 LOAD_CONST               4 (None)
                      420 LOAD_CONST               4 (None)
                      422 PRECALL                  2
                      426 CALL                     2
                      436 POP_TOP
                      438 LOAD_CONST               4 (None)
                      440 RETURN_VALUE
@@ -1878,24 +1972,26 @@
             ('indent', 'sort_keys')
          names      ('tucan.package_analysis', 'rec_travel_through_package', 'get_package_files', 'run_full_analysis', 'loguru', 'logger', 'json', 'os', 'info', 'getcwd', 'open', 'dump')
          varnames   ('path', 'rec_travel_through_package', 'get_package_files', 'run_full_analysis', 'logger', 'json', 'os', 'paths', 'files', 'full_analysis', 'newfile', 'fout')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/cli.py'
          name       'package_analysis'
-         firstlineno 364
+         firstlineno 384
          lnotab 0x020614050c0110022a0116012a013c012a01160204013001220132ff
-   names      ('__doc__', 'click', 'tucan', '__version__', '_ver_', '__name__', '_name_', 'add_version', 'group', 'main', 'command', 'argument', 'str', 'option', 'clean', 'struct', 'imports', 'ifdef_scan', 'ifdef_clean', 'ifdef_scan_pkge', 'package_analysis')
+   names      ('__doc__', 'click', 'tucan', '__version__', '_ver_', '__name__', '_name_', 'add_version', 'group', 'main', 'command', 'argument', 'str', 'option', 'bool', 'clean', 'struct', 'imports', 'ifdef_scan', 'ifdef_clean', 'ifdef_scan_pkge', 'package_analysis')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/dauptain/GITLAB/tucan/src/tucan/cli.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201040108010c010c03060b1c01020104ff0eff0e02022a260124
-      010e0102010201020102fc100604fa0eff0eff0e080234260124010e0102
-      010201020102fc100604fa0eff0eff0e080234260124010e010201020102
-      0102fc100604fa0eff0eff0e080215260124010e0102010201020102fc10
-      0604fa0eff0eff0e080221260124010e01020102010201020202fa10080e
-      0102010201020102fc100604fa0ef80eff0eff0e10021e260124010e0102
-      010201020102fc100604fa0eff0eff0e08023a2601240104ff0eff0e02
+      010e0102010201020102fc10060e0102010201020102fc100612fa0efa0e
+      ff0eff0e0e0234260124010e0102010201020102fc10060e010201020102
+      0102fc100604fa0efa0eff0eff0e0e0234260124010e0102010201020102
+      fc100604fa0eff0eff0e080215260124010e0102010201020102fc100604
+      fa0eff0eff0e080221260124010e01020102010201020202fa10080e0102
+      010201020102fc10060e0102010201020102fc10060e0102010201020102
+      fc100604fa0efa0efa0ef80eff0eff0e1c021a260124010e010201020102
+      0102fc100604fa0eff0eff0e08023a2601240104ff0eff0e02
```

### Comparing `tucan-0.1.0/src/tucan/__pycache__/imports_ftn.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/imports_ftn.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tucan-0.1.0/src/tucan/__pycache__/imports_main.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/imports_main.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,19 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0x9de28b65 (Wed Dec 27 08:38:53 2023 UTC)
-files sz: 1327
+moddate:  0xeab7e065 (Thu Feb 29 16:59:22 2024 UTC)
+files sz: 1591
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a0401
       00640164046c056d065a060100640164056c076d085a080100640164066c
-      096d0a5a0a01006407650b6408650c6604640984045a0d640a5300
+      096d0a5a0a0100640164076c0b6d0c5a0c0100640164086c0d6d0e5a0e01
+      006409650f640a65106604640b84045a11640c5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nTucan module to handle the import parsing of all files.\n')
                  4 STORE_NAME               0 (__doc__)
    
      4           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('logger',))
@@ -33,45 +34,61 @@
                 32 LOAD_CONST               4 (('unformat_ftn',))
                 34 IMPORT_NAME              5 (tucan.unformat_ftn)
                 36 IMPORT_FROM              6 (unformat_ftn)
                 38 STORE_NAME               6 (unformat_ftn)
                 40 POP_TOP
    
      8          42 LOAD_CONST               1 (0)
-                44 LOAD_CONST               5 (('imports_py',))
-                46 IMPORT_NAME              7 (tucan.imports_py)
-                48 IMPORT_FROM              8 (imports_py)
-                50 STORE_NAME               8 (imports_py)
+                44 LOAD_CONST               5 (('unformat_c',))
+                46 IMPORT_NAME              7 (tucan.unformat_c)
+                48 IMPORT_FROM              8 (unformat_c)
+                50 STORE_NAME               8 (unformat_c)
                 52 POP_TOP
    
      9          54 LOAD_CONST               1 (0)
-                56 LOAD_CONST               6 (('imports_ftn',))
-                58 IMPORT_NAME              9 (tucan.imports_ftn)
-                60 IMPORT_FROM             10 (imports_ftn)
-                62 STORE_NAME              10 (imports_ftn)
+                56 LOAD_CONST               6 (('imports_py',))
+                58 IMPORT_NAME              9 (tucan.imports_py)
+                60 IMPORT_FROM             10 (imports_py)
+                62 STORE_NAME              10 (imports_py)
                 64 POP_TOP
    
-    12          66 LOAD_CONST               7 ('filename')
-                68 LOAD_NAME               11 (str)
-                70 LOAD_CONST               8 ('return')
-                72 LOAD_NAME               12 (dict)
-                74 BUILD_TUPLE              4
-                76 LOAD_CONST               9 (<code object imports_main, file "/Users/dauptain/GITLAB/tucan/src/tucan/imports_main.py", line 12>)
-                78 MAKE_FUNCTION            4 (annotations)
-                80 STORE_NAME              13 (imports_main)
-                82 LOAD_CONST              10 (None)
-                84 RETURN_VALUE
+    10          66 LOAD_CONST               1 (0)
+                68 LOAD_CONST               7 (('imports_ftn',))
+                70 IMPORT_NAME             11 (tucan.imports_ftn)
+                72 IMPORT_FROM             12 (imports_ftn)
+                74 STORE_NAME              12 (imports_ftn)
+                76 POP_TOP
+   
+    11          78 LOAD_CONST               1 (0)
+                80 LOAD_CONST               8 (('imports_c',))
+                82 IMPORT_NAME             13 (tucan.imports_c)
+                84 IMPORT_FROM             14 (imports_c)
+                86 STORE_NAME              14 (imports_c)
+                88 POP_TOP
+   
+    14          90 LOAD_CONST               9 ('filename')
+                92 LOAD_NAME               15 (str)
+                94 LOAD_CONST              10 ('return')
+                96 LOAD_NAME               16 (dict)
+                98 BUILD_TUPLE              4
+               100 LOAD_CONST              11 (<code object imports_main, file "/Users/dauptain/GITLAB/tucan/src/tucan/imports_main.py", line 14>)
+               102 MAKE_FUNCTION            4 (annotations)
+               104 STORE_NAME              17 (imports_main)
+               106 LOAD_CONST              12 (None)
+               108 RETURN_VALUE
    consts
       '\nTucan module to handle the import parsing of all files.\n'
       0
       ('logger',)
       ('unformat_py',)
       ('unformat_ftn',)
+      ('unformat_c',)
       ('imports_py',)
       ('imports_ftn',)
+      ('imports_c',)
       'filename'
       'return'
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 6
          flags     : 3
@@ -87,57 +104,63 @@
             0359007701640484007c024400a6000000ab0000000000000000007d0269
             007d037c00a0060000000000000000000000000000000000000000a60000
             00ab000000000000000000a0070000000000000000000000000000000000
             0000006405a6010000ab0100000000000000007233740100000000000000
             0000006a0800000000000000006406a6010000ab01000000000000000001
             007413000000000000000000007c02a6010000ab0100000000000000007d
             047415000000000000000000007c04a6010000ab0100000000000000007d
-            036ea17c00a0060000000000000000000000000000000000000000a60000
+            036efb7c00a0060000000000000000000000000000000000000000a60000
             00ab000000000000000000a0070000000000000000000000000000000000
             0000006407a6010000ab0100000000000000007233740100000000000000
             0000006a0800000000000000006408a6010000ab01000000000000000001
             007417000000000000000000007c02a6010000ab0100000000000000007d
             047419000000000000000000007c04a6010000ab0100000000000000007d
+            036ea17c00a0060000000000000000000000000000000000000000a60000
+            00ab000000000000000000a0070000000000000000000000000000000000
+            0000006409a6010000ab0100000000000000007233740100000000000000
+            0000006a080000000000000000640aa6010000ab01000000000000000001
+            00741b000000000000000000007c02a6010000ab0100000000000000007d
+            04741d000000000000000000007c04a6010000ab0100000000000000007d
             036e477c00a0060000000000000000000000000000000000000000a60000
-            00ab000000000000000000a00d0000000000000000000000000000000000
-            0000006409a6010000ab010000000000000000640a190000000000000000
-            007d057401000000000000000000006a0e0000000000000000640b7c059b
-            00640c9d03a6010000ab0100000000000000000100690053007c035300
-          12           0 RESUME                   0
+            00ab000000000000000000a00f0000000000000000000000000000000000
+            000000640ba6010000ab010000000000000000640c190000000000000000
+            007d057401000000000000000000006a100000000000000000640d7c059b
+            00640e9d03a6010000ab0100000000000000000100690053007c035300
+          14           0 RESUME                   0
          
-          22           2 LOAD_GLOBAL              1 (NULL + logger)
+          24           2 LOAD_GLOBAL              1 (NULL + logger)
                       14 LOAD_ATTR                1 (info)
                       24 LOAD_CONST               1 ('Analyzing the imports for ')
                       26 LOAD_FAST                0 (filename)
                       28 FORMAT_VALUE             0
                       30 BUILD_STRING             2
                       32 PRECALL                  1
                       36 CALL                     1
                       46 POP_TOP
          
-          23          48 NOP
+          25          48 NOP
          
-          24          50 LOAD_GLOBAL              5 (NULL + open)
+          26          50 LOAD_GLOBAL              5 (NULL + open)
                       62 LOAD_FAST                0 (filename)
                       64 LOAD_CONST               2 ('r')
                       66 PRECALL                  2
                       70 CALL                     2
                       80 BEFORE_WITH
                       82 STORE_FAST               1 (fin)
          
-          25          84 LOAD_FAST                1 (fin)
+          27          84 LOAD_FAST                1 (fin)
                       86 LOAD_METHOD              3 (read)
                      108 PRECALL                  0
                      112 CALL                     0
                      122 LOAD_METHOD              4 (splitlines)
                      144 PRECALL                  0
                      148 CALL                     0
                      158 STORE_FAST               2 (code)
          
-          24         160 LOAD_CONST               3 (None)
+          26         160 LOAD_CONST               3 (None)
                      162 LOAD_CONST               3 (None)
                      164 LOAD_CONST               3 (None)
                      166 PRECALL                  2
                      170 CALL                     2
                      180 POP_TOP
                      182 JUMP_FORWARD            11 (to 206)
                  >>  184 PUSH_EXC_INFO
@@ -150,128 +173,158 @@
                  >>  198 POP_TOP
                      200 POP_EXCEPT
                      202 POP_TOP
                      204 POP_TOP
                  >>  206 JUMP_FORWARD            18 (to 244)
                  >>  208 PUSH_EXC_INFO
          
-          26         210 LOAD_GLOBAL             10 (UnicodeDecodeError)
+          28         210 LOAD_GLOBAL             10 (UnicodeDecodeError)
                      222 CHECK_EXC_MATCH
                      224 POP_JUMP_FORWARD_IF_FALSE     5 (to 236)
                      226 POP_TOP
          
-          27         228 BUILD_MAP                0
+          29         228 BUILD_MAP                0
                      230 SWAP                     2
                      232 POP_EXCEPT
                      234 RETURN_VALUE
          
-          26     >>  236 RERAISE                  0
+          28     >>  236 RERAISE                  0
                  >>  238 COPY                     3
                      240 POP_EXCEPT
                      242 RERAISE                  1
          
-          29     >>  244 LOAD_CONST               4 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/imports_main.py", line 29>)
+          31     >>  244 LOAD_CONST               4 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/imports_main.py", line 31>)
                      246 MAKE_FUNCTION            0
                      248 LOAD_FAST                2 (code)
                      250 GET_ITER
                      252 PRECALL                  0
                      256 CALL                     0
                      266 STORE_FAST               2 (code)
          
-          31         268 BUILD_MAP                0
+          33         268 BUILD_MAP                0
                      270 STORE_FAST               3 (imports_)
          
-          32         272 LOAD_FAST                0 (filename)
+          34         272 LOAD_FAST                0 (filename)
                      274 LOAD_METHOD              6 (lower)
                      296 PRECALL                  0
                      300 CALL                     0
                      310 LOAD_METHOD              7 (endswith)
                      332 LOAD_CONST               5 ('.py')
                      334 PRECALL                  1
                      338 CALL                     1
                      348 POP_JUMP_FORWARD_IF_FALSE    51 (to 452)
          
-          33         350 LOAD_GLOBAL              1 (NULL + logger)
+          35         350 LOAD_GLOBAL              1 (NULL + logger)
                      362 LOAD_ATTR                8 (debug)
                      372 LOAD_CONST               6 ('Python code detected ...')
                      374 PRECALL                  1
                      378 CALL                     1
                      388 POP_TOP
          
-          34         390 LOAD_GLOBAL             19 (NULL + unformat_py)
+          36         390 LOAD_GLOBAL             19 (NULL + unformat_py)
                      402 LOAD_FAST                2 (code)
                      404 PRECALL                  1
                      408 CALL                     1
                      418 STORE_FAST               4 (statements)
          
-          35         420 LOAD_GLOBAL             21 (NULL + imports_py)
+          37         420 LOAD_GLOBAL             21 (NULL + imports_py)
                      432 LOAD_FAST                4 (statements)
                      434 PRECALL                  1
                      438 CALL                     1
                      448 STORE_FAST               3 (imports_)
-                     450 JUMP_FORWARD           161 (to 774)
+                     450 JUMP_FORWARD           251 (to 954)
          
-          36     >>  452 LOAD_FAST                0 (filename)
+          38     >>  452 LOAD_FAST                0 (filename)
                      454 LOAD_METHOD              6 (lower)
                      476 PRECALL                  0
                      480 CALL                     0
                      490 LOAD_METHOD              7 (endswith)
-                     512 LOAD_CONST               7 (('.f', '.F', '.f77', '.f90'))
+                     512 LOAD_CONST               7 (('.f', '.F', '.f77', '.f90', '.inc'))
                      514 PRECALL                  1
                      518 CALL                     1
                      528 POP_JUMP_FORWARD_IF_FALSE    51 (to 632)
          
-          37         530 LOAD_GLOBAL              1 (NULL + logger)
+          39         530 LOAD_GLOBAL              1 (NULL + logger)
                      542 LOAD_ATTR                8 (debug)
                      552 LOAD_CONST               8 ('Fortran code detected ...')
                      554 PRECALL                  1
                      558 CALL                     1
                      568 POP_TOP
          
-          38         570 LOAD_GLOBAL             23 (NULL + unformat_ftn)
+          40         570 LOAD_GLOBAL             23 (NULL + unformat_ftn)
                      582 LOAD_FAST                2 (code)
                      584 PRECALL                  1
                      588 CALL                     1
                      598 STORE_FAST               4 (statements)
          
-          39         600 LOAD_GLOBAL             25 (NULL + imports_ftn)
+          41         600 LOAD_GLOBAL             25 (NULL + imports_ftn)
                      612 LOAD_FAST                4 (statements)
                      614 PRECALL                  1
                      618 CALL                     1
                      628 STORE_FAST               3 (imports_)
-                     630 JUMP_FORWARD            71 (to 774)
+                     630 JUMP_FORWARD           161 (to 954)
          
-          41     >>  632 LOAD_FAST                0 (filename)
+          42     >>  632 LOAD_FAST                0 (filename)
                      634 LOAD_METHOD              6 (lower)
                      656 PRECALL                  0
                      660 CALL                     0
-                     670 LOAD_METHOD             13 (split)
-                     692 LOAD_CONST               9 ('.')
+                     670 LOAD_METHOD              7 (endswith)
+                     692 LOAD_CONST               9 (('.c', '.h'))
                      694 PRECALL                  1
                      698 CALL                     1
-                     708 LOAD_CONST              10 (-1)
-                     710 BINARY_SUBSCR
-                     720 STORE_FAST               5 (ext)
-         
-          42         722 LOAD_GLOBAL              1 (NULL + logger)
-                     734 LOAD_ATTR               14 (error)
-                     744 LOAD_CONST              11 ('Extension ')
-                     746 LOAD_FAST                5 (ext)
-                     748 FORMAT_VALUE             0
-                     750 LOAD_CONST              12 (' not supported, exiting ...')
-                     752 BUILD_STRING             3
-                     754 PRECALL                  1
-                     758 CALL                     1
-                     768 POP_TOP
+                     708 POP_JUMP_FORWARD_IF_FALSE    51 (to 812)
+         
+          43         710 LOAD_GLOBAL              1 (NULL + logger)
+                     722 LOAD_ATTR                8 (debug)
+                     732 LOAD_CONST              10 ('C/C++ code detected ...')
+                     734 PRECALL                  1
+                     738 CALL                     1
+                     748 POP_TOP
+         
+          44         750 LOAD_GLOBAL             27 (NULL + unformat_c)
+                     762 LOAD_FAST                2 (code)
+                     764 PRECALL                  1
+                     768 CALL                     1
+                     778 STORE_FAST               4 (statements)
+         
+          45         780 LOAD_GLOBAL             29 (NULL + imports_c)
+                     792 LOAD_FAST                4 (statements)
+                     794 PRECALL                  1
+                     798 CALL                     1
+                     808 STORE_FAST               3 (imports_)
+                     810 JUMP_FORWARD            71 (to 954)
+         
+          47     >>  812 LOAD_FAST                0 (filename)
+                     814 LOAD_METHOD              6 (lower)
+                     836 PRECALL                  0
+                     840 CALL                     0
+                     850 LOAD_METHOD             15 (split)
+                     872 LOAD_CONST              11 ('.')
+                     874 PRECALL                  1
+                     878 CALL                     1
+                     888 LOAD_CONST              12 (-1)
+                     890 BINARY_SUBSCR
+                     900 STORE_FAST               5 (ext)
+         
+          48         902 LOAD_GLOBAL              1 (NULL + logger)
+                     914 LOAD_ATTR               16 (error)
+                     924 LOAD_CONST              13 ('Extension ')
+                     926 LOAD_FAST                5 (ext)
+                     928 FORMAT_VALUE             0
+                     930 LOAD_CONST              14 (' not supported, exiting ...')
+                     932 BUILD_STRING             3
+                     934 PRECALL                  1
+                     938 CALL                     1
+                     948 POP_TOP
          
-          43         770 BUILD_MAP                0
-                     772 RETURN_VALUE
+          49         950 BUILD_MAP                0
+                     952 RETURN_VALUE
          
-          44     >>  774 LOAD_FAST                3 (imports_)
-                     776 RETURN_VALUE
+          50     >>  954 LOAD_FAST                3 (imports_)
+                     956 RETURN_VALUE
          ExceptionTable:
            50 to 80 -> 208 [0]
            82 to 158 -> 184 [1] lasti
            160 to 182 -> 208 [0]
            184 to 190 -> 192 [3] lasti
            192 to 196 -> 208 [0]
            198 to 198 -> 192 [3] lasti
@@ -287,15 +340,15 @@
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 19
                code
                   0x970067007c005d167d017c01a000000000000000000000000000000000
                   0000000000a6000000ab00000000000000000091028c175300
-                29           0 RESUME                   0
+                31           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                22 (to 52)
                              8 STORE_FAST               1 (line)
                             10 LOAD_FAST                1 (line)
                             12 LOAD_METHOD              0 (lower)
                             34 PRECALL                  0
@@ -306,36 +359,38 @@
                consts
                names      ('lower',)
                varnames   ('.0', 'line')
                freevars   ()
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/imports_main.py'
                name       '<listcomp>'
-               firstlineno 29
+               firstlineno 31
                lnotab 0x
             '.py'
             'Python code detected ...'
-            ('.f', '.F', '.f77', '.f90')
+            ('.f', '.F', '.f77', '.f90', '.inc')
             'Fortran code detected ...'
+            ('.c', '.h')
+            'C/C++ code detected ...'
             '.'
             -1
             'Extension '
             ' not supported, exiting ...'
-         names      ('logger', 'info', 'open', 'read', 'splitlines', 'UnicodeDecodeError', 'lower', 'endswith', 'debug', 'unformat_py', 'imports_py', 'unformat_ftn', 'imports_ftn', 'split', 'error')
+         names      ('logger', 'info', 'open', 'read', 'splitlines', 'UnicodeDecodeError', 'lower', 'endswith', 'debug', 'unformat_py', 'imports_py', 'unformat_ftn', 'imports_ftn', 'unformat_c', 'imports_c', 'split', 'error')
          varnames   ('filename', 'fin', 'code', 'imports_', 'statements', 'ext')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/imports_main.py'
          name       'imports_main'
-         firstlineno 12
+         firstlineno 14
          lnotab
             0x020a2e01020122014cff3202120108ff0803180204014e0128011e0120
-            014e0128011e0120025a0130010401
+            014e0128011e0120014e0128011e0120025a0130010401
       None
-   names      ('__doc__', 'loguru', 'logger', 'tucan.unformat_py', 'unformat_py', 'tucan.unformat_ftn', 'unformat_ftn', 'tucan.imports_py', 'imports_py', 'tucan.imports_ftn', 'imports_ftn', 'str', 'dict', 'imports_main')
+   names      ('__doc__', 'loguru', 'logger', 'tucan.unformat_py', 'unformat_py', 'tucan.unformat_ftn', 'unformat_ftn', 'tucan.unformat_c', 'unformat_c', 'tucan.imports_py', 'imports_py', 'tucan.imports_ftn', 'imports_ftn', 'tucan.imports_c', 'imports_c', 'str', 'dict', 'imports_main')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/dauptain/GITLAB/tucan/src/tucan/imports_main.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104030c020c010c010c010c03
+   lnotab 0x00ff020104030c020c010c010c010c010c010c03
```

### Comparing `tucan-0.1.0/src/tucan/__pycache__/imports_py.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/imports_py.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tucan-0.1.0/src/tucan/__pycache__/package_analysis.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/package_analysis.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xcc89ba65 (Wed Jan 31 17:56:28 2024 UTC)
-files sz: 4696
+moddate:  0x027b3366 (Thu May  2 11:37:38 2024 UTC)
+files sz: 5212
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a0401
@@ -71,58 +71,58 @@
                 92 LOAD_CONST              10 ('return')
                 94 LOAD_NAME               12 (list)
                 96 BUILD_TUPLE              4
                 98 LOAD_CONST              13 (<code object clean_extensions_in_paths, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 38>)
                100 MAKE_FUNCTION            4 (annotations)
                102 STORE_NAME              14 (clean_extensions_in_paths)
    
-    58         104 LOAD_CONST              14 ('clean_paths')
+    62         104 LOAD_CONST              14 ('clean_paths')
                106 LOAD_NAME               12 (list)
                108 LOAD_CONST              15 ('relpath')
                110 LOAD_NAME               11 (str)
                112 LOAD_CONST              10 ('return')
                114 LOAD_NAME               15 (dict)
                116 BUILD_TUPLE              6
-               118 LOAD_CONST              16 (<code object get_package_files, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 58>)
+               118 LOAD_CONST              16 (<code object get_package_files, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 62>)
                120 MAKE_FUNCTION            4 (annotations)
                122 STORE_NAME              16 (get_package_files)
    
-    83         124 LOAD_CONST              17 ('files')
+    87         124 LOAD_CONST              17 ('files')
                126 LOAD_NAME               15 (dict)
                128 LOAD_CONST              10 ('return')
                130 LOAD_NAME               15 (dict)
                132 BUILD_TUPLE              4
-               134 LOAD_CONST              18 (<code object run_full_analysis, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 83>)
+               134 LOAD_CONST              18 (<code object run_full_analysis, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 87>)
                136 MAKE_FUNCTION            4 (annotations)
                138 STORE_NAME              17 (run_full_analysis)
    
-   103         140 LOAD_CONST              14 ('clean_paths')
+   123         140 LOAD_CONST              14 ('clean_paths')
                142 LOAD_NAME               12 (list)
                144 LOAD_CONST              10 ('return')
                146 LOAD_NAME               15 (dict)
                148 BUILD_TUPLE              4
-               150 LOAD_CONST              19 (<code object run_unformat, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 103>)
+               150 LOAD_CONST              19 (<code object run_unformat, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 123>)
                152 MAKE_FUNCTION            4 (annotations)
                154 STORE_NAME              18 (run_unformat)
    
-   125         156 LOAD_CONST              14 ('clean_paths')
+   145         156 LOAD_CONST              14 ('clean_paths')
                158 LOAD_NAME               12 (list)
                160 LOAD_CONST              10 ('return')
                162 LOAD_NAME               15 (dict)
                164 BUILD_TUPLE              4
-               166 LOAD_CONST              20 (<code object run_struct, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 125>)
+               166 LOAD_CONST              20 (<code object run_struct, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 145>)
                168 MAKE_FUNCTION            4 (annotations)
                170 STORE_NAME              19 (run_struct)
    
-   153         172 LOAD_CONST              14 ('clean_paths')
+   173         172 LOAD_CONST              14 ('clean_paths')
                174 LOAD_NAME               12 (list)
                176 LOAD_CONST              10 ('return')
                178 LOAD_NAME               15 (dict)
                180 BUILD_TUPLE              4
-               182 LOAD_CONST              21 (<code object run_imports, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 153>)
+               182 LOAD_CONST              21 (<code object run_imports, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 173>)
                184 MAKE_FUNCTION            4 (annotations)
                186 STORE_NAME              20 (run_imports)
                188 LOAD_CONST               7 (None)
                190 RETURN_VALUE
    consts
       'Module that aims to analyze a whole package based \non the other unitary function of the package'
       0
@@ -255,15 +255,15 @@
                  >>  500 JUMP_BACKWARD          203 (to 96)
          
           27     >>  502 JUMP_BACKWARD          226 (to 52)
          
           35     >>  504 LOAD_FAST                3 (paths_)
                      506 RETURN_VALUE
          consts
-            '\n    List all paths from a folder and its subfolders recursively.\n\n    RECURSIVE\n    '
+            '\n    List all paths from a folder and its sub-folders recursively.\n\n    RECURSIVE\n    '
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 19
                code
                   0x970067007c005d117d017401000000000000000000007c01a6010000ab
@@ -322,47 +322,47 @@
           49           6 LOAD_FAST                0 (paths_list)
                        8 GET_ITER
                  >>   10 FOR_ITER                44 (to 100)
                       12 STORE_FAST               2 (path)
          
           50          14 LOAD_FAST                2 (path)
                       16 LOAD_METHOD              0 (endswith)
-                      38 LOAD_CONST               1 (('.py', '.f90', '.f', '.F', '.f77', '.c'))
+                      38 LOAD_CONST               1 (('.py', '.f', '.F', '.f77', '.f90', '.c', '.cpp', '.h', '.hpp'))
                       40 PRECALL                  1
                       44 CALL                     1
                       54 POP_JUMP_FORWARD_IF_FALSE    21 (to 98)
          
-          51          56 LOAD_FAST                1 (clean_paths)
+          55          56 LOAD_FAST                1 (clean_paths)
                       58 LOAD_METHOD              1 (append)
                       80 LOAD_FAST                2 (path)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_TOP
                  >>   98 JUMP_BACKWARD           45 (to 10)
          
-          53     >>  100 BUILD_LIST               0
+          57     >>  100 BUILD_LIST               0
          
-          54         102 LOAD_GLOBAL              5 (NULL + set)
+          58         102 LOAD_GLOBAL              5 (NULL + set)
                      114 LOAD_FAST                1 (clean_paths)
                      116 PRECALL                  1
                      120 CALL                     1
          
-          53         130 LIST_EXTEND              1
+          57         130 LIST_EXTEND              1
                      132 RETURN_VALUE
          consts
             '\n    Remove unwanted path extensions and duplicates.\n\n    Args:\n        paths_list (list): List of all paths gatheres through recursive analysis\n\n    Returns:\n        list: List of cleaned paths.\n    '
-            ('.py', '.f90', '.f', '.F', '.f77', '.c')
+            ('.py', '.f', '.F', '.f77', '.f90', '.c', '.cpp', '.h', '.hpp')
          names      ('endswith', 'append', 'set')
          varnames   ('paths_list', 'clean_paths', 'path')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py'
          name       'clean_extensions_in_paths'
          firstlineno 38
-         lnotab 0x020a040108012a012c0202011cff
+         lnotab 0x020a040108012a052c0202011cff
       'clean_paths'
       'relpath'
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 6
          flags     : 3
@@ -379,98 +379,98 @@
             000000000000008901a6010000ab010000000000000000a6010000ab0100
             00000000000000a0070000000000000000000000000000000000000000a6
             000000ab0000000000000000007d037c05a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c047c033c0000
             008c4e7c045300
                        0 MAKE_CELL                1 (relpath)
          
-          58           2 RESUME                   0
+          62           2 RESUME                   0
          
-          63           4 BUILD_LIST               0
+          67           4 BUILD_LIST               0
                        6 STORE_FAST               2 (files)
          
-          64           8 LOAD_FAST                0 (clean_paths)
+          68           8 LOAD_FAST                0 (clean_paths)
                       10 GET_ITER
                  >>   12 FOR_ITER                56 (to 126)
                       14 STORE_FAST               3 (path_)
          
-          65          16 LOAD_GLOBAL              1 (NULL + Path)
+          69          16 LOAD_GLOBAL              1 (NULL + Path)
                       28 LOAD_FAST                3 (path_)
                       30 PRECALL                  1
                       34 CALL                     1
                       44 LOAD_METHOD              1 (is_dir)
                       66 PRECALL                  0
                       70 CALL                     0
                       80 POP_JUMP_FORWARD_IF_TRUE    21 (to 124)
          
-          67          82 LOAD_FAST                2 (files)
+          71          82 LOAD_FAST                2 (files)
                       84 LOAD_METHOD              2 (append)
                      106 LOAD_FAST                3 (path_)
                      108 PRECALL                  1
                      112 CALL                     1
                      122 POP_TOP
                  >>  124 JUMP_BACKWARD           57 (to 12)
          
-          69     >>  126 LOAD_GLOBAL              7 (NULL + clean_extensions_in_paths)
+          73     >>  126 LOAD_GLOBAL              7 (NULL + clean_extensions_in_paths)
                      138 LOAD_FAST                2 (files)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 STORE_FAST               2 (files)
          
-          71         156 LOAD_FAST                2 (files)
+          75         156 LOAD_FAST                2 (files)
                      158 POP_JUMP_FORWARD_IF_TRUE    20 (to 200)
          
-          72         160 LOAD_GLOBAL              9 (NULL + logger)
+          76         160 LOAD_GLOBAL              9 (NULL + logger)
                      172 LOAD_ATTR                5 (warning)
                      182 LOAD_CONST               1 ('No files found in the paths provided')
                      184 PRECALL                  1
                      188 CALL                     1
                      198 POP_TOP
          
-          74     >>  200 LOAD_CLOSURE             1 (relpath)
+          78     >>  200 LOAD_CLOSURE             1 (relpath)
                      202 BUILD_TUPLE              1
-                     204 LOAD_CONST               2 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 74>)
+                     204 LOAD_CONST               2 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py", line 78>)
                      206 MAKE_FUNCTION            8 (closure)
                      208 LOAD_FAST                2 (files)
                      210 GET_ITER
                      212 PRECALL                  0
                      216 CALL                     0
                      226 STORE_FAST               2 (files)
          
-          76         228 BUILD_MAP                0
+          80         228 BUILD_MAP                0
                      230 STORE_FAST               4 (out)
          
-          77         232 LOAD_FAST                2 (files)
+          81         232 LOAD_FAST                2 (files)
                      234 GET_ITER
                  >>  236 FOR_ITER                77 (to 392)
                      238 STORE_FAST               5 (file)
          
-          78         240 LOAD_FAST                5 (file)
+          82         240 LOAD_FAST                5 (file)
                      242 LOAD_METHOD              6 (relative_to)
                      264 LOAD_GLOBAL              1 (NULL + Path)
                      276 LOAD_DEREF               1 (relpath)
                      278 PRECALL                  1
                      282 CALL                     1
                      292 PRECALL                  1
                      296 CALL                     1
                      306 LOAD_METHOD              7 (as_posix)
                      328 PRECALL                  0
                      332 CALL                     0
                      342 STORE_FAST               3 (path_)
          
-          79         344 LOAD_FAST                5 (file)
+          83         344 LOAD_FAST                5 (file)
                      346 LOAD_METHOD              7 (as_posix)
                      368 PRECALL                  0
                      372 CALL                     0
                      382 LOAD_FAST                4 (out)
                      384 LOAD_FAST                3 (path_)
                      386 STORE_SUBSCR
                      390 JUMP_BACKWARD           78 (to 236)
          
-          80     >>  392 LOAD_FAST                4 (out)
+          84     >>  392 LOAD_FAST                4 (out)
                      394 RETURN_VALUE
          consts
             '\n    Return all the files useful for a package analysis, with their absolut paths\n    '
             'No files found in the paths provided'
             code
                argcount  : 1
                nlocals   : 2
@@ -478,15 +478,15 @@
                flags     : 19
                code
                   0x9501970067007c005d217d017401000000000000000000008902a60100
                   00ab0100000000000000007401000000000000000000007c01a6010000ab
                   0100000000000000007a0b000091028c225300
                              0 COPY_FREE_VARS           1
                
-                74           2 RESUME                   0
+                78           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                33 (to 76)
                             10 STORE_FAST               1 (p_)
                             12 LOAD_GLOBAL              1 (NULL + Path)
                             24 LOAD_DEREF               2 (relpath)
                             26 PRECALL                  1
@@ -502,176 +502,249 @@
                consts
                names      ('Path',)
                varnames   ('.0', 'p_')
                freevars   ('relpath',)
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py'
                name       '<listcomp>'
-               firstlineno 74
+               firstlineno 78
                lnotab 0x
          names      ('Path', 'is_dir', 'append', 'clean_extensions_in_paths', 'logger', 'warning', 'relative_to', 'as_posix')
          varnames   ('clean_paths', 'relpath', 'files', 'path_', 'out', 'file')
          freevars   ()
          cellvars   ('relpath',)
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py'
          name       'get_package_files'
-         firstlineno 58
+         firstlineno 62
          lnotab 0x04050401080142022c021e02040128021c020401080168013001
       'files'
       code
          argcount  : 1
-         nlocals   : 4
-         stacksize : 6
+         nlocals   : 8
+         stacksize : 5
          flags     : 3
          code
-            0x970069007d017c00a00000000000000000000000000000000000000000
-            00a6000000ab00000000000000000044005d415c0200007d027d03640174
-            03000000000000000000007c03a6010000ab01000000000000000069017c
-            017c023c0000007c017c0219000000000000000000a00200000000000000
-            000000000000000000000000007407000000000000000000007c03a60100
-            00ab010000000000000000a6010000ab01000000000000000001008c4274
-            09000000000000000000006a0500000000000000006402a6010000ab0100
-            0000000000000001007c015300
-          83           0 RESUME                   0
+            0x970069007d0167007d0267007d037c00a0000000000000000000000000
+            000000000000000000a6000000ab00000000000000000044005d7b5c0200
+            007d047d0564017403000000000000000000007c05a6010000ab01000000
+            000000000069017c017c043c0000007405000000000000000000007c05a6
+            010000ab0100000000000000007d067c0669006b020000000072157c02a0
+            0300000000000000000000000000000000000000007c04a6010000ab0100
+            0000000000000001007c0664026b020000000072177c03a0030000000000
+            0000000000000000000000000000007c04a6010000ab0100000000000000
+            00010069007d067c017c0419000000000000000000a00400000000000000
+            000000000000000000000000007c06a6010000ab01000000000000000001
+            008c7c740b000000000000000000006a0600000000000000006403a60100
+            00ab01000000000000000001007c03722c740b000000000000000000006a
+            0700000000000000006404a6010000ab01000000000000000001007c037c
+            027a00000044005d127d0774110000000000000000000064057c07a60200
+            00ab02000000000000000001008c137c015300
+          87           0 RESUME                   0
          
-          94           2 BUILD_MAP                0
+          98           2 BUILD_MAP                0
                        4 STORE_FAST               1 (full_analysis)
          
-          96           6 LOAD_FAST                0 (files)
-                       8 LOAD_METHOD              0 (items)
-                      30 PRECALL                  0
-                      34 CALL                     0
-                      44 GET_ITER
-                 >>   46 FOR_ITER                65 (to 178)
-                      48 UNPACK_SEQUENCE          2
-                      52 STORE_FAST               2 (file)
-                      54 STORE_FAST               3 (path_)
-         
-          97          56 LOAD_CONST               1 ('imports')
-                      58 LOAD_GLOBAL              3 (NULL + imports_main)
-                      70 LOAD_FAST                3 (path_)
-                      72 PRECALL                  1
-                      76 CALL                     1
-                      86 BUILD_MAP                1
-                      88 LOAD_FAST                1 (full_analysis)
-                      90 LOAD_FAST                2 (file)
-                      92 STORE_SUBSCR
-         
-          98          96 LOAD_FAST                1 (full_analysis)
-                      98 LOAD_FAST                2 (file)
-                     100 BINARY_SUBSCR
-                     110 LOAD_METHOD              2 (update)
-                     132 LOAD_GLOBAL              7 (NULL + struct_main)
-                     144 LOAD_FAST                3 (path_)
-                     146 PRECALL                  1
-                     150 CALL                     1
-                     160 PRECALL                  1
-                     164 CALL                     1
-                     174 POP_TOP
-                     176 JUMP_BACKWARD           66 (to 46)
-         
-          99     >>  178 LOAD_GLOBAL              9 (NULL + logger)
-                     190 LOAD_ATTR                5 (success)
-                     200 LOAD_CONST               2 ('Analyze completed.')
-                     202 PRECALL                  1
-                     206 CALL                     1
-                     216 POP_TOP
+         100           6 BUILD_LIST               0
+                       8 STORE_FAST               2 (skipped_files)
          
-         100         218 LOAD_FAST                1 (full_analysis)
-                     220 RETURN_VALUE
+         101          10 BUILD_LIST               0
+                      12 STORE_FAST               3 (unrecoverable_files)
+         
+         102          14 LOAD_FAST                0 (files)
+                      16 LOAD_METHOD              0 (items)
+                      38 PRECALL                  0
+                      42 CALL                     0
+                      52 GET_ITER
+                 >>   54 FOR_ITER               123 (to 302)
+                      56 UNPACK_SEQUENCE          2
+                      60 STORE_FAST               4 (file)
+                      62 STORE_FAST               5 (path_)
+         
+         103          64 LOAD_CONST               1 ('imports')
+                      66 LOAD_GLOBAL              3 (NULL + imports_main)
+                      78 LOAD_FAST                5 (path_)
+                      80 PRECALL                  1
+                      84 CALL                     1
+                      94 BUILD_MAP                1
+                      96 LOAD_FAST                1 (full_analysis)
+                      98 LOAD_FAST                4 (file)
+                     100 STORE_SUBSCR
+         
+         104         104 LOAD_GLOBAL              5 (NULL + struct_main)
+                     116 LOAD_FAST                5 (path_)
+                     118 PRECALL                  1
+                     122 CALL                     1
+                     132 STORE_FAST               6 (analysis)
+         
+         105         134 LOAD_FAST                6 (analysis)
+                     136 BUILD_MAP                0
+                     138 COMPARE_OP               2 (==)
+                     144 POP_JUMP_FORWARD_IF_FALSE    21 (to 188)
+         
+         106         146 LOAD_FAST                2 (skipped_files)
+                     148 LOAD_METHOD              3 (append)
+                     170 LOAD_FAST                4 (file)
+                     172 PRECALL                  1
+                     176 CALL                     1
+                     186 POP_TOP
+         
+         107     >>  188 LOAD_FAST                6 (analysis)
+                     190 LOAD_CONST               2 (None)
+                     192 COMPARE_OP               2 (==)
+                     198 POP_JUMP_FORWARD_IF_FALSE    23 (to 246)
+         
+         108         200 LOAD_FAST                3 (unrecoverable_files)
+                     202 LOAD_METHOD              3 (append)
+                     224 LOAD_FAST                4 (file)
+                     226 PRECALL                  1
+                     230 CALL                     1
+                     240 POP_TOP
+         
+         109         242 BUILD_MAP                0
+                     244 STORE_FAST               6 (analysis)
+         
+         111     >>  246 LOAD_FAST                1 (full_analysis)
+                     248 LOAD_FAST                4 (file)
+                     250 BINARY_SUBSCR
+                     260 LOAD_METHOD              4 (update)
+                     282 LOAD_FAST                6 (analysis)
+                     284 PRECALL                  1
+                     288 CALL                     1
+                     298 POP_TOP
+                     300 JUMP_BACKWARD          124 (to 54)
+         
+         112     >>  302 LOAD_GLOBAL             11 (NULL + logger)
+                     314 LOAD_ATTR                6 (success)
+                     324 LOAD_CONST               3 ('Analyze completed.')
+                     326 PRECALL                  1
+                     330 CALL                     1
+                     340 POP_TOP
+         
+         113         342 LOAD_FAST                3 (unrecoverable_files)
+                     344 POP_JUMP_FORWARD_IF_FALSE    44 (to 434)
+         
+         114         346 LOAD_GLOBAL             11 (NULL + logger)
+                     358 LOAD_ATTR                7 (warning)
+                     368 LOAD_CONST               4 ('Some files could not be parsed correctly')
+                     370 PRECALL                  1
+                     374 CALL                     1
+                     384 POP_TOP
+         
+         115         386 LOAD_FAST                3 (unrecoverable_files)
+                     388 LOAD_FAST                2 (skipped_files)
+                     390 BINARY_OP                0 (+)
+                     394 GET_ITER
+                 >>  396 FOR_ITER                18 (to 434)
+                     398 STORE_FAST               7 (f_)
+         
+         116         400 LOAD_GLOBAL             17 (NULL + print)
+                     412 LOAD_CONST               5 (' - ')
+                     414 LOAD_FAST                7 (f_)
+                     416 PRECALL                  2
+                     420 CALL                     2
+                     430 POP_TOP
+                     432 JUMP_BACKWARD           19 (to 396)
+         
+         120     >>  434 LOAD_FAST                1 (full_analysis)
+                     436 RETURN_VALUE
          consts
             '\n    Gather the data associated to the functions and the imports within a file\n\n    Args:\n        files (dict): key: short_name , value: absolute paths\n\n    Returns:\n        dict: _description_\n    '
             'imports'
+            None
             'Analyze completed.'
-         names      ('items', 'imports_main', 'update', 'struct_main', 'logger', 'success')
-         varnames   ('files', 'full_analysis', 'file', 'path_')
+            'Some files could not be parsed correctly'
+            ' - '
+         names      ('items', 'imports_main', 'struct_main', 'append', 'update', 'logger', 'success', 'warning', 'print')
+         varnames   ('files', 'full_analysis', 'skipped_files', 'unrecoverable_files', 'file', 'path_', 'analysis', 'f_')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py'
          name       'run_full_analysis'
-         firstlineno 83
-         lnotab 0x020b04023201280152012801
+         firstlineno 87
+         lnotab
+            0x020b040204010401320128011e010c012a010c012a0104023801280104
+            0128010e012204
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 7
          flags     : 3
          code
             0x970069007d017c0044005d5f7d027401000000000000000000007c02a6
             010000ab010000000000000000a001000000000000000000000000000000
             0000000000a6000000ab0000000000000000007c017c023c00000064017d
             037c017c021900000000000000000072157405000000000000000000007c
             017c0219000000000000000000a6010000ab0100000000000000007d0374
             07000000000000000000006a04000000000000000064027c039b0064037c
             029b009d04a6010000ab01000000000000000001008c607c015300
-         103           0 RESUME                   0
+         123           0 RESUME                   0
          
-         113           2 BUILD_MAP                0
+         133           2 BUILD_MAP                0
                        4 STORE_FAST               1 (statements)
          
-         114           6 LOAD_FAST                0 (clean_paths)
+         134           6 LOAD_FAST                0 (clean_paths)
                        8 GET_ITER
                  >>   10 FOR_ITER                95 (to 202)
                       12 STORE_FAST               2 (file)
          
-         115          14 LOAD_GLOBAL              1 (NULL + unformat_main)
+         135          14 LOAD_GLOBAL              1 (NULL + unformat_main)
                       26 LOAD_FAST                2 (file)
                       28 PRECALL                  1
                       32 CALL                     1
                       42 LOAD_METHOD              1 (to_nob)
                       64 PRECALL                  0
                       68 CALL                     0
                       78 LOAD_FAST                1 (statements)
                       80 LOAD_FAST                2 (file)
                       82 STORE_SUBSCR
          
-         117          86 LOAD_CONST               1 (0)
+         137          86 LOAD_CONST               1 (0)
                       88 STORE_FAST               3 (nbr_of_stmt)
          
-         118          90 LOAD_FAST                1 (statements)
+         138          90 LOAD_FAST                1 (statements)
                       92 LOAD_FAST                2 (file)
                       94 BINARY_SUBSCR
                      104 POP_JUMP_FORWARD_IF_FALSE    21 (to 148)
          
-         119         106 LOAD_GLOBAL              5 (NULL + len)
+         139         106 LOAD_GLOBAL              5 (NULL + len)
                      118 LOAD_FAST                1 (statements)
                      120 LOAD_FAST                2 (file)
                      122 BINARY_SUBSCR
                      132 PRECALL                  1
                      136 CALL                     1
                      146 STORE_FAST               3 (nbr_of_stmt)
          
-         120     >>  148 LOAD_GLOBAL              7 (NULL + logger)
+         140     >>  148 LOAD_GLOBAL              7 (NULL + logger)
                      160 LOAD_ATTR                4 (info)
                      170 LOAD_CONST               2 ('Found ')
                      172 LOAD_FAST                3 (nbr_of_stmt)
                      174 FORMAT_VALUE             0
                      176 LOAD_CONST               3 (' statements for ')
                      178 LOAD_FAST                2 (file)
                      180 FORMAT_VALUE             0
                      182 BUILD_STRING             4
                      184 PRECALL                  1
                      188 CALL                     1
                      198 POP_TOP
                      200 JUMP_BACKWARD           96 (to 10)
          
-         122     >>  202 LOAD_FAST                1 (statements)
+         142     >>  202 LOAD_FAST                1 (statements)
                      204 RETURN_VALUE
          consts
             '\n    Gather the unformated version of code files within a dict.\n\n    Args:\n        clean_paths (list): List of cleaned paths.\n\n    Returns:\n        dict: File path as key, item as a list of lines with their line number span\n    '
             0
             'Found '
             ' statements for '
          names      ('unformat_main', 'to_nob', 'len', 'logger', 'info')
          varnames   ('clean_paths', 'statements', 'file', 'nbr_of_stmt')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py'
          name       'run_unformat'
-         firstlineno 103
+         firstlineno 123
          lnotab 0x020a040108014802040110012a013602
       code
          argcount  : 1
          nlocals   : 8
          stacksize : 7
          flags     : 3
          code
@@ -683,115 +756,115 @@
             000000000000007d027c0244005d5b7d047409000000000000000000007c
             04a6010000ab0100000000000000007c017c043c00000064017d057c017c
             0419000000000000000000a0050000000000000000000000000000000000
             000000a6000000ab00000000000000000044005d105c0200007d067d077c
             057c076402190000000000000000007a0d00007d058c11740d0000000000
             00000000006a07000000000000000064037c059b0064047c049b009d04a6
             010000ab01000000000000000001008c5c7c015300
-         125           0 RESUME                   0
+         145           0 RESUME                   0
          
-         135           2 BUILD_MAP                0
+         155           2 BUILD_MAP                0
                        4 STORE_FAST               1 (full_struct)
          
-         136           6 BUILD_LIST               0
+         156           6 BUILD_LIST               0
                        8 STORE_FAST               2 (files)
          
-         138          10 LOAD_FAST                0 (clean_paths)
+         158          10 LOAD_FAST                0 (clean_paths)
                       12 GET_ITER
                  >>   14 FOR_ITER                56 (to 128)
                       16 STORE_FAST               3 (path_)
          
-         139          18 LOAD_GLOBAL              1 (NULL + Path)
+         159          18 LOAD_GLOBAL              1 (NULL + Path)
                       30 LOAD_FAST                3 (path_)
                       32 PRECALL                  1
                       36 CALL                     1
                       46 LOAD_METHOD              1 (is_dir)
                       68 PRECALL                  0
                       72 CALL                     0
                       82 POP_JUMP_FORWARD_IF_TRUE    21 (to 126)
          
-         140          84 LOAD_FAST                2 (files)
+         160          84 LOAD_FAST                2 (files)
                       86 LOAD_METHOD              2 (append)
                      108 LOAD_FAST                3 (path_)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 POP_TOP
                  >>  126 JUMP_BACKWARD           57 (to 14)
          
-         142     >>  128 LOAD_GLOBAL              7 (NULL + clean_extensions_in_paths)
+         162     >>  128 LOAD_GLOBAL              7 (NULL + clean_extensions_in_paths)
                      140 LOAD_FAST                2 (files)
                      142 PRECALL                  1
                      146 CALL                     1
                      156 STORE_FAST               2 (files)
          
-         143         158 LOAD_FAST                2 (files)
+         163         158 LOAD_FAST                2 (files)
                      160 GET_ITER
                  >>  162 FOR_ITER                91 (to 346)
                      164 STORE_FAST               4 (file)
          
-         144         166 LOAD_GLOBAL              9 (NULL + struct_main)
+         164         166 LOAD_GLOBAL              9 (NULL + struct_main)
                      178 LOAD_FAST                4 (file)
                      180 PRECALL                  1
                      184 CALL                     1
                      194 LOAD_FAST                1 (full_struct)
                      196 LOAD_FAST                4 (file)
                      198 STORE_SUBSCR
          
-         145         202 LOAD_CONST               1 (0)
+         165         202 LOAD_CONST               1 (0)
                      204 STORE_FAST               5 (total_stmts)
          
-         146         206 LOAD_FAST                1 (full_struct)
+         166         206 LOAD_FAST                1 (full_struct)
                      208 LOAD_FAST                4 (file)
                      210 BINARY_SUBSCR
                      220 LOAD_METHOD              5 (items)
                      242 PRECALL                  0
                      246 CALL                     0
                      256 GET_ITER
                  >>  258 FOR_ITER                16 (to 292)
                      260 UNPACK_SEQUENCE          2
                      264 STORE_FAST               6 (_)
                      266 STORE_FAST               7 (data)
          
-         147         268 LOAD_FAST                5 (total_stmts)
+         167         268 LOAD_FAST                5 (total_stmts)
                      270 LOAD_FAST                7 (data)
                      272 LOAD_CONST               2 ('ssize')
                      274 BINARY_SUBSCR
                      284 BINARY_OP               13 (+=)
                      288 STORE_FAST               5 (total_stmts)
                      290 JUMP_BACKWARD           17 (to 258)
          
-         148     >>  292 LOAD_GLOBAL             13 (NULL + logger)
+         168     >>  292 LOAD_GLOBAL             13 (NULL + logger)
                      304 LOAD_ATTR                7 (info)
                      314 LOAD_CONST               3 ('Found ')
                      316 LOAD_FAST                5 (total_stmts)
                      318 FORMAT_VALUE             0
                      320 LOAD_CONST               4 (' statements for ')
                      322 LOAD_FAST                4 (file)
                      324 FORMAT_VALUE             0
                      326 BUILD_STRING             4
                      328 PRECALL                  1
                      332 CALL                     1
                      342 POP_TOP
                      344 JUMP_BACKWARD           92 (to 162)
          
-         150     >>  346 LOAD_FAST                1 (full_struct)
+         170     >>  346 LOAD_FAST                1 (full_struct)
                      348 RETURN_VALUE
          consts
             '\n    Gather the data associated to the functions within a file.\n\n    Args:\n        clean_paths (list): List of cleaned paths.\n\n    Returns:\n        dict: File path as key, item as dict with function names and their data (NLOC, CCN, etc.)\n    '
             0
             'ssize'
             'Found '
             ' statements for '
          names      ('Path', 'is_dir', 'append', 'clean_extensions_in_paths', 'struct_main', 'items', 'logger', 'info')
          varnames   ('clean_paths', 'full_struct', 'files', 'path_', 'file', 'total_stmts', '_', 'data')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py'
          name       'run_struct'
-         firstlineno 125
+         firstlineno 145
          lnotab 0x020a04010402080142012c021e010801240104013e0118013602
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 4
          flags     : 3
          code
@@ -800,86 +873,86 @@
             000000000000000000a6000000ab00000000000000000073157c02a00200
             000000000000000000000000000000000000007c03a6010000ab01000000
             000000000001008c397407000000000000000000007c02a6010000ab0100
             000000000000007d027c0244005d147d047409000000000000000000007c
             04a6010000ab0100000000000000007c017c043c0000008c15740b000000
             000000000000006a0600000000000000006401a6010000ab010000000000
             00000001007c015300
-         153           0 RESUME                   0
+         173           0 RESUME                   0
          
-         163           2 BUILD_MAP                0
+         183           2 BUILD_MAP                0
                        4 STORE_FAST               1 (full_imports)
          
-         164           6 BUILD_LIST               0
+         184           6 BUILD_LIST               0
                        8 STORE_FAST               2 (files)
          
-         166          10 LOAD_FAST                0 (clean_paths)
+         186          10 LOAD_FAST                0 (clean_paths)
                       12 GET_ITER
                  >>   14 FOR_ITER                56 (to 128)
                       16 STORE_FAST               3 (path_)
          
-         167          18 LOAD_GLOBAL              1 (NULL + Path)
+         187          18 LOAD_GLOBAL              1 (NULL + Path)
                       30 LOAD_FAST                3 (path_)
                       32 PRECALL                  1
                       36 CALL                     1
                       46 LOAD_METHOD              1 (is_dir)
                       68 PRECALL                  0
                       72 CALL                     0
                       82 POP_JUMP_FORWARD_IF_TRUE    21 (to 126)
          
-         168          84 LOAD_FAST                2 (files)
+         188          84 LOAD_FAST                2 (files)
                       86 LOAD_METHOD              2 (append)
                      108 LOAD_FAST                3 (path_)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 POP_TOP
                  >>  126 JUMP_BACKWARD           57 (to 14)
          
-         170     >>  128 LOAD_GLOBAL              7 (NULL + clean_extensions_in_paths)
+         190     >>  128 LOAD_GLOBAL              7 (NULL + clean_extensions_in_paths)
                      140 LOAD_FAST                2 (files)
                      142 PRECALL                  1
                      146 CALL                     1
                      156 STORE_FAST               2 (files)
          
-         171         158 LOAD_FAST                2 (files)
+         191         158 LOAD_FAST                2 (files)
                      160 GET_ITER
                  >>  162 FOR_ITER                20 (to 204)
                      164 STORE_FAST               4 (file)
          
-         172         166 LOAD_GLOBAL              9 (NULL + imports_main)
+         192         166 LOAD_GLOBAL              9 (NULL + imports_main)
                      178 LOAD_FAST                4 (file)
                      180 PRECALL                  1
                      184 CALL                     1
                      194 LOAD_FAST                1 (full_imports)
                      196 LOAD_FAST                4 (file)
                      198 STORE_SUBSCR
                      202 JUMP_BACKWARD           21 (to 162)
          
-         173     >>  204 LOAD_GLOBAL             11 (NULL + logger)
+         193     >>  204 LOAD_GLOBAL             11 (NULL + logger)
                      216 LOAD_ATTR                6 (success)
                      226 LOAD_CONST               1 ('Imports found.')
                      228 PRECALL                  1
                      232 CALL                     1
                      242 POP_TOP
          
-         174         244 LOAD_FAST                1 (full_imports)
+         194         244 LOAD_FAST                1 (full_imports)
                      246 RETURN_VALUE
          consts
             '\n    Gather the imports within a file.\n\n    Args:\n        clean_paths (list): List of cleaned paths.\n\n    Returns:\n        dict: File path as key, dict of function with their imports as item.\n    '
             'Imports found.'
          names      ('Path', 'is_dir', 'append', 'clean_extensions_in_paths', 'imports_main', 'logger', 'success')
          varnames   ('clean_paths', 'full_imports', 'files', 'path_', 'file')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py'
          name       'run_imports'
-         firstlineno 153
+         firstlineno 173
          lnotab 0x020a04010402080142012c021e01080126012801
       (None,)
    names      ('__doc__', 'pathlib', 'Path', 'loguru', 'logger', 'tucan.unformat_main', 'unformat_main', 'tucan.struct_main', 'struct_main', 'tucan.imports_main', 'imports_main', 'str', 'list', 'rec_travel_through_package', 'clean_extensions_in_paths', 'dict', 'get_package_files', 'run_full_analysis', 'run_unformat', 'run_struct', 'run_imports')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/dauptain/GITLAB/tucan/src/tucan/package_analysis.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104030c010c010c010c010c03161b1014141910141016101c
+   lnotab 0x00ff020104030c010c010c010c010c03161b1018141910241016101c
```

### Comparing `tucan-0.1.0/src/tucan/__pycache__/struct_c.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/struct_c.cpython-311.pyc`

 * *Files 24% similar despite different names*

#### Python bytecode

```diff
@@ -1,23 +1,23 @@
 magic:    0xa70d0d0a
-moddate:  0x13c7b765 (Mon Jan 29 15:41:07 2024 UTC)
-files sz: 4276
+moddate:  0x5d5d3366 (Thu May  2 09:31:09 2024 UTC)
+files sz: 4007
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 6
+   stacksize : 8
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a030100640064
       036c046d055a050100640064046c066d075a070100640064056c086d095a
       096d0a5a0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064066c0e6d0f5a0f01
-      0064076507640865106604640984045a1164076507640865106604640a84
-      045a12640b65136408650265136513660219000000000000000000660464
-      0c84045a14640d6515640865156604640e84045a16640d65156408651766
-      04640f84045a1864015300
+      006407650764086510640965116606640a84045a12641364076507640865
+      10640965116606640c84055a13640d6514640e6515640965026514651466
+      02190000000000000000006606640f84045a166410651764096517660464
+      1184045a1864106517640965156604641284045a1964015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (re)
                  8 STORE_NAME               0 (re)
    
@@ -41,22 +41,22 @@
                 40 LOAD_CONST               4 (('Statements',))
                 42 IMPORT_NAME              6 (tucan.unformat_common)
                 44 IMPORT_FROM              7 (Statements)
                 46 STORE_NAME               7 (Statements)
                 48 POP_TOP
    
      5          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               5 (('find_words_before_left_parenthesis', 'buffer_item', 'stack_item', 'struct_from_stack', 'struct_augment'))
+                52 LOAD_CONST               5 (('find_words_before_left_parenthesis', 'new_buffer_item', 'new_stack_item', 'struct_from_stack', 'struct_augment'))
                 54 IMPORT_NAME              8 (tucan.struct_common)
                 56 IMPORT_FROM              9 (find_words_before_left_parenthesis)
                 58 STORE_NAME               9 (find_words_before_left_parenthesis)
-                60 IMPORT_FROM             10 (buffer_item)
-                62 STORE_NAME              10 (buffer_item)
-                64 IMPORT_FROM             11 (stack_item)
-                66 STORE_NAME              11 (stack_item)
+                60 IMPORT_FROM             10 (new_buffer_item)
+                62 STORE_NAME              10 (new_buffer_item)
+                64 IMPORT_FROM             11 (new_stack_item)
+                66 STORE_NAME              11 (new_stack_item)
                 68 IMPORT_FROM             12 (struct_from_stack)
                 70 STORE_NAME              12 (struct_from_stack)
                 72 IMPORT_FROM             13 (struct_augment)
                 74 STORE_NAME              13 (struct_augment)
                 76 POP_TOP
    
     13          78 LOAD_CONST               0 (0)
@@ -64,568 +64,562 @@
                 82 IMPORT_NAME             14 (tucan.kw_lang)
                 84 IMPORT_FROM             15 (KEYWORDS_C)
                 86 STORE_NAME              15 (KEYWORDS_C)
                 88 POP_TOP
    
     15          90 LOAD_CONST               7 ('stmts')
                 92 LOAD_NAME                7 (Statements)
-                94 LOAD_CONST               8 ('return')
-                96 LOAD_NAME               16 (dict)
-                98 BUILD_TUPLE              4
-               100 LOAD_CONST               9 (<code object extract_struct_c, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py", line 15>)
-               102 MAKE_FUNCTION            4 (annotations)
-               104 STORE_NAME              17 (extract_struct_c)
-   
-    26         106 LOAD_CONST               7 ('stmts')
-               108 LOAD_NAME                7 (Statements)
-               110 LOAD_CONST               8 ('return')
-               112 LOAD_NAME               16 (dict)
-               114 BUILD_TUPLE              4
-               116 LOAD_CONST              10 (<code object _extract_on_cleaned_c, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py", line 26>)
-               118 MAKE_FUNCTION            4 (annotations)
-               120 STORE_NAME              18 (_extract_on_cleaned_c)
-   
-    98         122 LOAD_CONST              11 ('line')
-               124 LOAD_NAME               19 (str)
-               126 LOAD_CONST               8 ('return')
-               128 LOAD_NAME                2 (Tuple)
-               130 LOAD_NAME               19 (str)
-               132 LOAD_NAME               19 (str)
-               134 BUILD_TUPLE              2
-               136 BINARY_SUBSCR
-               146 BUILD_TUPLE              4
-               148 LOAD_CONST              12 (<code object _parse_type_name_c, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py", line 98>)
-               150 MAKE_FUNCTION            4 (annotations)
-               152 STORE_NAME              20 (_parse_type_name_c)
-   
-   128         154 LOAD_CONST              13 ('code')
-               156 LOAD_NAME               21 (list)
-               158 LOAD_CONST               8 ('return')
-               160 LOAD_NAME               21 (list)
-               162 BUILD_TUPLE              4
-               164 LOAD_CONST              14 (<code object find_callables_c, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py", line 128>)
-               166 MAKE_FUNCTION            4 (annotations)
-               168 STORE_NAME              22 (find_callables_c)
-   
-   140         170 LOAD_CONST              13 ('code')
-               172 LOAD_NAME               21 (list)
-               174 LOAD_CONST               8 ('return')
-               176 LOAD_NAME               23 (int)
-               178 BUILD_TUPLE              4
-               180 LOAD_CONST              15 (<code object compute_ccn_approx_c, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py", line 140>)
-               182 MAKE_FUNCTION            4 (annotations)
-               184 STORE_NAME              24 (compute_ccn_approx_c)
-               186 LOAD_CONST               1 (None)
-               188 RETURN_VALUE
+                94 LOAD_CONST               8 ('verbose')
+                96 LOAD_NAME               16 (bool)
+                98 LOAD_CONST               9 ('return')
+               100 LOAD_NAME               17 (dict)
+               102 BUILD_TUPLE              6
+               104 LOAD_CONST              10 (<code object extract_struct_c, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py", line 15>)
+               106 MAKE_FUNCTION            4 (annotations)
+               108 STORE_NAME              18 (extract_struct_c)
+   
+    27         110 LOAD_CONST              19 ((False,))
+               112 LOAD_CONST               7 ('stmts')
+               114 LOAD_NAME                7 (Statements)
+               116 LOAD_CONST               8 ('verbose')
+               118 LOAD_NAME               16 (bool)
+               120 LOAD_CONST               9 ('return')
+               122 LOAD_NAME               17 (dict)
+               124 BUILD_TUPLE              6
+               126 LOAD_CONST              12 (<code object _extract_on_cleaned_c, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py", line 27>)
+               128 MAKE_FUNCTION            5 (defaults, annotations)
+               130 STORE_NAME              19 (_extract_on_cleaned_c)
+   
+    91         132 LOAD_CONST              13 ('line')
+               134 LOAD_NAME               20 (str)
+               136 LOAD_CONST              14 ('line_idx')
+               138 LOAD_NAME               21 (int)
+               140 LOAD_CONST               9 ('return')
+               142 LOAD_NAME                2 (Tuple)
+               144 LOAD_NAME               20 (str)
+               146 LOAD_NAME               20 (str)
+               148 BUILD_TUPLE              2
+               150 BINARY_SUBSCR
+               160 BUILD_TUPLE              6
+               162 LOAD_CONST              15 (<code object _parse_type_name_c, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py", line 91>)
+               164 MAKE_FUNCTION            4 (annotations)
+               166 STORE_NAME              22 (_parse_type_name_c)
+   
+   121         168 LOAD_CONST              16 ('code')
+               170 LOAD_NAME               23 (list)
+               172 LOAD_CONST               9 ('return')
+               174 LOAD_NAME               23 (list)
+               176 BUILD_TUPLE              4
+               178 LOAD_CONST              17 (<code object find_callables_c, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py", line 121>)
+               180 MAKE_FUNCTION            4 (annotations)
+               182 STORE_NAME              24 (find_callables_c)
+   
+   133         184 LOAD_CONST              16 ('code')
+               186 LOAD_NAME               23 (list)
+               188 LOAD_CONST               9 ('return')
+               190 LOAD_NAME               21 (int)
+               192 BUILD_TUPLE              4
+               194 LOAD_CONST              18 (<code object compute_ccn_approx_c, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py", line 133>)
+               196 MAKE_FUNCTION            4 (annotations)
+               198 STORE_NAME              25 (compute_ccn_approx_c)
+               200 LOAD_CONST               1 (None)
+               202 RETURN_VALUE
    consts
       0
       None
       ('Tuple', 'List')
       ('logger',)
       ('Statements',)
-      ('find_words_before_left_parenthesis', 'buffer_item', 'stack_item', 'struct_from_stack', 'struct_augment')
+      ('find_words_before_left_parenthesis', 'new_buffer_item', 'new_stack_item', 'struct_from_stack', 'struct_augment')
       ('KEYWORDS_C',)
       'stmts'
+      'verbose'
       'return'
       code
-         argcount  : 1
-         nlocals   : 3
+         argcount  : 2
+         nlocals   : 4
          stacksize : 6
          flags     : 3
          code
             0x97007c00a0000000000000000000000000000000000000000000a60000
-            00ab0000000000000000007d017403000000000000000000007c00a60100
-            00ab0100000000000000007d027405000000000000000000007c027c0174
-            0600000000000000000000740800000000000000000000a6040000ab0400
-            000000000000007d027c025300
+            00ab0000000000000000007d027403000000000000000000007c007c01ac
+            01a6020000ab0200000000000000007d037405000000000000000000007c
+            037c02740600000000000000000000740800000000000000000000a60400
+            00ab0400000000000000007d037c035300
           15           0 RESUME                   0
          
-          20           2 LOAD_FAST                0 (stmts)
+          21           2 LOAD_FAST                0 (stmts)
                        4 LOAD_METHOD              0 (to_code)
                       26 PRECALL                  0
                       30 CALL                     0
-                      40 STORE_FAST               1 (clean_code)
+                      40 STORE_FAST               2 (clean_code)
          
-          21          42 LOAD_GLOBAL              3 (NULL + _extract_on_cleaned_c)
+          22          42 LOAD_GLOBAL              3 (NULL + _extract_on_cleaned_c)
                       54 LOAD_FAST                0 (stmts)
-                      56 PRECALL                  1
-                      60 CALL                     1
-                      70 STORE_FAST               2 (all_structs)
-         
-          22          72 LOAD_GLOBAL              5 (NULL + struct_augment)
-                      84 LOAD_FAST                2 (all_structs)
-                      86 LOAD_FAST                1 (clean_code)
-                      88 LOAD_GLOBAL              6 (find_callables_c)
-                     100 LOAD_GLOBAL              8 (compute_ccn_approx_c)
-                     112 PRECALL                  4
-                     116 CALL                     4
-                     126 STORE_FAST               2 (all_structs)
+                      56 LOAD_FAST                1 (verbose)
+                      58 KW_NAMES                 1
+                      60 PRECALL                  2
+                      64 CALL                     2
+                      74 STORE_FAST               3 (all_structs)
+         
+          23          76 LOAD_GLOBAL              5 (NULL + struct_augment)
+                      88 LOAD_FAST                3 (all_structs)
+                      90 LOAD_FAST                2 (clean_code)
+                      92 LOAD_GLOBAL              6 (find_callables_c)
+                     104 LOAD_GLOBAL              8 (compute_ccn_approx_c)
+                     116 PRECALL                  4
+                     120 CALL                     4
+                     130 STORE_FAST               3 (all_structs)
          
-          23         128 LOAD_FAST                2 (all_structs)
-                     130 RETURN_VALUE
+          24         132 LOAD_FAST                3 (all_structs)
+                     134 RETURN_VALUE
          consts
             'Main calls to build structure form statements\n\n    statements is the output of tucan.unformat_c.unformat_c\n    '
+            ('verbose',)
          names      ('to_code', '_extract_on_cleaned_c', 'struct_augment', 'find_callables_c', 'compute_ccn_approx_c')
-         varnames   ('stmts', 'clean_code', 'all_structs')
+         varnames   ('stmts', 'verbose', 'clean_code', 'all_structs')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py'
          name       'extract_struct_c'
          firstlineno 15
-         lnotab 0x020528011e013801
+         lnotab 0x0206280122013801
+      False
       code
-         argcount  : 1
-         nlocals   : 17
-         stacksize : 15
+         argcount  : 2
+         nlocals   : 16
+         stacksize : 12
          flags     : 3
          code
-            0x970067007d0167007d0267007d0364017d0464017d05640267017d0674
+            0x970067007d0267007d0367007d0464017d0564017d06640267017d0774
             01000000000000000000007c006a0100000000000000007c006a02000000
-            0000000000a6020000ab020000000000000000440090015d5e5c0200007d
-            075c0200007d087d097c0464037a0d00007d0464047d0a74070000000000
-            00000000007c07a6010000ab010000000000000000010064057c07760072
-            757409000000000000000000007c07a6010000ab0100000000000000005c
-            0200007d0b7d0c7c06a00500000000000000000000000000000000000000
-            007c05a6010000ab01000000000000000001007c01a00500000000000000
-            00000000000000000000000000740d000000000000000000007c0b7c0c7c
-            077c087c04ac06a6050000ab050000000000000000a6010000ab01000000
-            000000000001007c03a00500000000000000000000000000000000000000
-            007c0ca6010000ab01000000000000000001007407000000000000000000
-            0064077c03a6020000ab020000000000000000010064047d0a7c0744005d
-            c37d0d7c0a7c0d7a0d00007d0a7c0d64086b020000000072057c0564037a
-            0d00007d057c0d64096b020000000072ab7c0564037a1700007d057c057c
-            06640a190000000000000000006b0200000000729a740700000000000000
-            000000640b7c03a6020000ab02000000000000000001007c01640a190000
-            000000000000005c0500007d0b7d0c7d0e7d0f7d107c02a0050000000000
-            000000000000000000000000000000740f000000000000000000007c0b7c
-            0c7c03a0080000000000000000000000000000000000000000a6000000ab
-            0000000000000000007c0f7c107c0e7c097c047c07ac0ca6090000ab0900
-            00000000000000a6010000ab01000000000000000001007c03a009000000
-            0000000000000000000000000000000000640aa6010000ab010000000000
-            00000001007c01a009000000000000000000000000000000000000000064
-            0aa6010000ab01000000000000000001007c06a009000000000000000000
-            0000000000000000000000640aa6010000ab01000000000000000001008c
-            c490018c607415000000000000000000007c026700640da201ac0ea60200
-            00ab0200000000000000005300
-          26           0 RESUME                   0
-         
-          28           2 BUILD_LIST               0
-                       4 STORE_FAST               1 (buffer)
-         
-          29           6 BUILD_LIST               0
-                       8 STORE_FAST               2 (stack)
-         
-          30          10 BUILD_LIST               0
-                      12 STORE_FAST               3 (path)
+            0000000000a6020000ab020000000000000000440090015d3a5c0200007d
+            085c0200007d097d0a7c0564037a0d00007d0564047d0b64057c08760072
+            687407000000000000000000007c087c09a6020000ab0200000000000000
+            005c0200007d0c7d0d7c07a0040000000000000000000000000000000000
+            0000007c06a6010000ab01000000000000000001007c04a0040000000000
+            0000000000000000000000000000007c0da6010000ab0100000000000000
+            0001007c02a0040000000000000000000000000000000000000000740b00
+            0000000000000000007c0c7c047c0d7c087c097c057c01ac06a6070000ab
+            070000000000000000a6010000ab010000000000000000010064047d0b7c
+            0844005dbb7d0e7c0b7c0e7a0d00007d0b7c0e64076b020000000072057c
+            0664037a0d00007d067c0e64086b020000000072a37c0664037a1700007d
+            067c067c076409190000000000000000006b020000000072927c01722474
+            0d000000000000000000006a070000000000000000640a74110000000000
+            00000000007c04a6010000ab0100000000000000009b009d02a6010000ab
+            01000000000000000001007c026409190000000000000000007d0f7c03a0
+            040000000000000000000000000000000000000000741300000000000000
+            0000007c0f7c0a7c057c08a6040000ab040000000000000000a6010000ab
+            01000000000000000001007c04a00a000000000000000000000000000000
+            00000000006409a6010000ab01000000000000000001007c02a00a000000
+            00000000000000000000000000000000006409a6010000ab010000000000
+            00000001007c07a00a000000000000000000000000000000000000000064
+            09a6010000ab01000000000000000001008cbc90018c3c74170000000000
+            00000000007c036700640ba201ac0ca6020000ab02000000000000000053
+            00
+          27           0 RESUME                   0
+         
+          29           2 BUILD_LIST               0
+                       4 STORE_FAST               2 (buffer)
+         
+          30           6 BUILD_LIST               0
+                       8 STORE_FAST               3 (stack)
+         
+          31          10 BUILD_LIST               0
+                      12 STORE_FAST               4 (path)
          
-          32          14 LOAD_CONST               1 (0)
-                      16 STORE_FAST               4 (stat_idx)
+          33          14 LOAD_CONST               1 (0)
+                      16 STORE_FAST               5 (stat_idx)
          
-          34          18 LOAD_CONST               1 (0)
-                      20 STORE_FAST               5 (level)
+          35          18 LOAD_CONST               1 (0)
+                      20 STORE_FAST               6 (level)
          
-          35          22 LOAD_CONST               2 (None)
+          36          22 LOAD_CONST               2 (None)
                       24 BUILD_LIST               1
-                      26 STORE_FAST               6 (stack_level)
+                      26 STORE_FAST               7 (stack_level)
          
-          37          28 LOAD_GLOBAL              1 (NULL + zip)
+          38          28 LOAD_GLOBAL              1 (NULL + zip)
                       40 LOAD_FAST                0 (stmts)
                       42 LOAD_ATTR                1 (stmt)
                       52 LOAD_FAST                0 (stmts)
                       54 LOAD_ATTR                2 (lines)
                       64 PRECALL                  2
                       68 CALL                     2
                       78 GET_ITER
                  >>   80 EXTENDED_ARG             1
-                      82 FOR_ITER               350 (to 784)
+                      82 FOR_ITER               314 (to 712)
                       84 UNPACK_SEQUENCE          2
-                      88 STORE_FAST               7 (line)
+                      88 STORE_FAST               8 (line)
                       90 UNPACK_SEQUENCE          2
-                      94 STORE_FAST               8 (line_idx1)
-                      96 STORE_FAST               9 (line_idx2)
+                      94 STORE_FAST               9 (line_idx1)
+                      96 STORE_FAST              10 (line_idx2)
          
-          38          98 LOAD_FAST                4 (stat_idx)
+          39          98 LOAD_FAST                5 (stat_idx)
                      100 LOAD_CONST               3 (1)
                      102 BINARY_OP               13 (+=)
-                     106 STORE_FAST               4 (stat_idx)
+                     106 STORE_FAST               5 (stat_idx)
+         
+          40         108 LOAD_CONST               4 ('')
+                     110 STORE_FAST              11 (part)
+         
+          44         112 LOAD_CONST               5 ('###===')
+                     114 LOAD_FAST                8 (line)
+                     116 CONTAINS_OP              0
+                     118 POP_JUMP_FORWARD_IF_FALSE   104 (to 328)
+         
+          45         120 LOAD_GLOBAL              7 (NULL + _parse_type_name_c)
+                     132 LOAD_FAST                8 (line)
+                     134 LOAD_FAST                9 (line_idx1)
+                     136 PRECALL                  2
+                     140 CALL                     2
+                     150 UNPACK_SEQUENCE          2
+                     154 STORE_FAST              12 (type_)
+                     156 STORE_FAST              13 (name)
+         
+          46         158 LOAD_FAST                7 (stack_level)
+                     160 LOAD_METHOD              4 (append)
+                     182 LOAD_FAST                6 (level)
+                     184 PRECALL                  1
+                     188 CALL                     1
+                     198 POP_TOP
+         
+          47         200 LOAD_FAST                4 (path)
+                     202 LOAD_METHOD              4 (append)
+                     224 LOAD_FAST               13 (name)
+                     226 PRECALL                  1
+                     230 CALL                     1
+                     240 POP_TOP
+         
+          48         242 LOAD_FAST                2 (buffer)
+                     244 LOAD_METHOD              4 (append)
+         
+          49         266 LOAD_GLOBAL             11 (NULL + new_buffer_item)
+         
+          50         278 LOAD_FAST               12 (type_)
+         
+          51         280 LOAD_FAST                4 (path)
+         
+          52         282 LOAD_FAST               13 (name)
+         
+          53         284 LOAD_FAST                8 (line)
          
-          39         108 LOAD_CONST               4 ('')
-                     110 STORE_FAST              10 (part)
+          54         286 LOAD_FAST                9 (line_idx1)
          
-          40         112 LOAD_GLOBAL              7 (NULL + print)
-                     124 LOAD_FAST                7 (line)
-                     126 PRECALL                  1
-                     130 CALL                     1
-                     140 POP_TOP
-         
-          43         142 LOAD_CONST               5 ('###===')
-                     144 LOAD_FAST                7 (line)
-                     146 CONTAINS_OP              0
-                     148 POP_JUMP_FORWARD_IF_FALSE   117 (to 384)
-         
-          44         150 LOAD_GLOBAL              9 (NULL + _parse_type_name_c)
-                     162 LOAD_FAST                7 (line)
-                     164 PRECALL                  1
-                     168 CALL                     1
-                     178 UNPACK_SEQUENCE          2
-                     182 STORE_FAST              11 (type_)
-                     184 STORE_FAST              12 (name)
-         
-          45         186 LOAD_FAST                6 (stack_level)
-                     188 LOAD_METHOD              5 (append)
-                     210 LOAD_FAST                5 (level)
-                     212 PRECALL                  1
-                     216 CALL                     1
-                     226 POP_TOP
-         
-          46         228 LOAD_FAST                1 (buffer)
-                     230 LOAD_METHOD              5 (append)
-         
-          47         252 LOAD_GLOBAL             13 (NULL + buffer_item)
-         
-          48         264 LOAD_FAST               11 (type_)
-         
-          49         266 LOAD_FAST               12 (name)
-         
-          50         268 LOAD_FAST                7 (line)
-         
-          51         270 LOAD_FAST                8 (line_idx1)
-         
-          52         272 LOAD_FAST                4 (stat_idx)
-         
-          47         274 KW_NAMES                 6
-                     276 PRECALL                  5
-                     280 CALL                     5
-         
-          46         290 PRECALL                  1
-                     294 CALL                     1
-                     304 POP_TOP
-         
-          55         306 LOAD_FAST                3 (path)
-                     308 LOAD_METHOD              5 (append)
-                     330 LOAD_FAST               12 (name)
-                     332 PRECALL                  1
-                     336 CALL                     1
-                     346 POP_TOP
-         
-          56         348 LOAD_GLOBAL              7 (NULL + print)
-                     360 LOAD_CONST               7 ('SOP')
-                     362 LOAD_FAST                3 (path)
-                     364 PRECALL                  2
-                     368 CALL                     2
-                     378 POP_TOP
-         
-          57         380 LOAD_CONST               4 ('')
-                     382 STORE_FAST              10 (part)
-         
-          59     >>  384 LOAD_FAST                7 (line)
-                     386 GET_ITER
-                 >>  388 FOR_ITER               195 (to 780)
-                     390 STORE_FAST              13 (char)
-         
-          60         392 LOAD_FAST               10 (part)
-                     394 LOAD_FAST               13 (char)
-                     396 BINARY_OP               13 (+=)
-                     400 STORE_FAST              10 (part)
+          55         288 LOAD_FAST                5 (stat_idx)
          
-          61         402 LOAD_FAST               13 (char)
-                     404 LOAD_CONST               8 ('{')
+          56         290 LOAD_FAST                1 (verbose)
+         
+          49         292 KW_NAMES                 6
+                     294 PRECALL                  7
+                     298 CALL                     7
+         
+          48         308 PRECALL                  1
+                     312 CALL                     1
+                     322 POP_TOP
+         
+          59         324 LOAD_CONST               4 ('')
+                     326 STORE_FAST              11 (part)
+         
+          61     >>  328 LOAD_FAST                8 (line)
+                     330 GET_ITER
+                 >>  332 FOR_ITER               187 (to 708)
+                     334 STORE_FAST              14 (char)
+         
+          62         336 LOAD_FAST               11 (part)
+                     338 LOAD_FAST               14 (char)
+                     340 BINARY_OP               13 (+=)
+                     344 STORE_FAST              11 (part)
+         
+          63         346 LOAD_FAST               14 (char)
+                     348 LOAD_CONST               7 ('{')
+                     350 COMPARE_OP               2 (==)
+                     356 POP_JUMP_FORWARD_IF_FALSE     5 (to 368)
+         
+          64         358 LOAD_FAST                6 (level)
+                     360 LOAD_CONST               3 (1)
+                     362 BINARY_OP               13 (+=)
+                     366 STORE_FAST               6 (level)
+         
+          65     >>  368 LOAD_FAST               14 (char)
+                     370 LOAD_CONST               8 ('}')
+                     372 COMPARE_OP               2 (==)
+                     378 POP_JUMP_FORWARD_IF_FALSE   163 (to 706)
+         
+          66         380 LOAD_FAST                6 (level)
+                     382 LOAD_CONST               3 (1)
+                     384 BINARY_OP               23 (-=)
+                     388 STORE_FAST               6 (level)
+         
+          67         390 LOAD_FAST                6 (level)
+                     392 LOAD_FAST                7 (stack_level)
+                     394 LOAD_CONST               9 (-1)
+                     396 BINARY_SUBSCR
                      406 COMPARE_OP               2 (==)
-                     412 POP_JUMP_FORWARD_IF_FALSE     5 (to 424)
+                     412 POP_JUMP_FORWARD_IF_FALSE   146 (to 706)
+         
+          68         414 LOAD_FAST                1 (verbose)
+                     416 POP_JUMP_FORWARD_IF_FALSE    36 (to 490)
          
-          62         414 LOAD_FAST                5 (level)
-                     416 LOAD_CONST               3 (1)
-                     418 BINARY_OP               13 (+=)
-                     422 STORE_FAST               5 (level)
-         
-          63     >>  424 LOAD_FAST               13 (char)
-                     426 LOAD_CONST               9 ('}')
-                     428 COMPARE_OP               2 (==)
-                     434 POP_JUMP_FORWARD_IF_FALSE   171 (to 778)
-         
-          64         436 LOAD_FAST                5 (level)
-                     438 LOAD_CONST               3 (1)
-                     440 BINARY_OP               23 (-=)
-                     444 STORE_FAST               5 (level)
-         
-          65         446 LOAD_FAST                5 (level)
-                     448 LOAD_FAST                6 (stack_level)
-                     450 LOAD_CONST              10 (-1)
-                     452 BINARY_SUBSCR
-                     462 COMPARE_OP               2 (==)
-                     468 POP_JUMP_FORWARD_IF_FALSE   154 (to 778)
-         
-          66         470 LOAD_GLOBAL              7 (NULL + print)
-                     482 LOAD_CONST              11 ('EOP')
-                     484 LOAD_FAST                3 (path)
-                     486 PRECALL                  2
-                     490 CALL                     2
-                     500 POP_TOP
-         
-          67         502 LOAD_FAST                1 (buffer)
-                     504 LOAD_CONST              10 (-1)
-                     506 BINARY_SUBSCR
-                     516 UNPACK_SEQUENCE          5
-                     520 STORE_FAST              11 (type_)
-                     522 STORE_FAST              12 (name)
-                     524 STORE_FAST              14 (line_start)
-                     526 STORE_FAST              15 (line_idx)
-                     528 STORE_FAST              16 (statement_idx)
-         
-          68         530 LOAD_FAST                2 (stack)
-                     532 LOAD_METHOD              5 (append)
-         
-          69         554 LOAD_GLOBAL             15 (NULL + stack_item)
-         
-          70         566 LOAD_FAST               11 (type_)
-         
-          71         568 LOAD_FAST               12 (name)
-         
-          72         570 LOAD_FAST                3 (path)
-                     572 LOAD_METHOD              8 (copy)
-                     594 PRECALL                  0
-                     598 CALL                     0
-         
-          73         608 LOAD_FAST               15 (line_idx)
-         
-          74         610 LOAD_FAST               16 (statement_idx)
-         
-          75         612 LOAD_FAST               14 (line_start)
-         
-          76         614 LOAD_FAST                9 (line_idx2)
-         
-          77         616 LOAD_FAST                4 (stat_idx)
-         
-          78         618 LOAD_FAST                7 (line)
-         
-          69         620 KW_NAMES                12
-                     622 PRECALL                  9
-                     626 CALL                     9
-         
-          68         636 PRECALL                  1
-                     640 CALL                     1
-                     650 POP_TOP
-         
-          81         652 LOAD_FAST                3 (path)
-                     654 LOAD_METHOD              9 (pop)
-                     676 LOAD_CONST              10 (-1)
-                     678 PRECALL                  1
-                     682 CALL                     1
-                     692 POP_TOP
-         
-          82         694 LOAD_FAST                1 (buffer)
-                     696 LOAD_METHOD              9 (pop)
-                     718 LOAD_CONST              10 (-1)
-                     720 PRECALL                  1
-                     724 CALL                     1
-                     734 POP_TOP
-         
-          83         736 LOAD_FAST                6 (stack_level)
-                     738 LOAD_METHOD              9 (pop)
-                     760 LOAD_CONST              10 (-1)
-                     762 PRECALL                  1
-                     766 CALL                     1
-                     776 POP_TOP
-                 >>  778 JUMP_BACKWARD          196 (to 388)
-         
-          59     >>  780 EXTENDED_ARG             1
-                     782 JUMP_BACKWARD          352 (to 80)
-         
-          86     >>  784 LOAD_GLOBAL             21 (NULL + struct_from_stack)
-                     796 LOAD_FAST                2 (stack)
-                     798 BUILD_LIST               0
-                     800 LOAD_CONST              13 (('function ', 'subroutine ', 'derived_type ', 'userdef_type ', 'pointer '))
-                     802 LIST_EXTEND              1
-                     804 KW_NAMES                14
-                     806 PRECALL                  2
-                     810 CALL                     2
-                     820 RETURN_VALUE
+          69         418 LOAD_GLOBAL             13 (NULL + logger)
+                     430 LOAD_ATTR                7 (critical)
+                     440 LOAD_CONST              10 ('Stop :')
+                     442 LOAD_GLOBAL             17 (NULL + str)
+                     454 LOAD_FAST                4 (path)
+                     456 PRECALL                  1
+                     460 CALL                     1
+                     470 FORMAT_VALUE             0
+                     472 BUILD_STRING             2
+                     474 PRECALL                  1
+                     478 CALL                     1
+                     488 POP_TOP
+         
+          70     >>  490 LOAD_FAST                2 (buffer)
+                     492 LOAD_CONST               9 (-1)
+                     494 BINARY_SUBSCR
+                     504 STORE_FAST              15 (last_buff)
+         
+          71         506 LOAD_FAST                3 (stack)
+                     508 LOAD_METHOD              4 (append)
+         
+          72         530 LOAD_GLOBAL             19 (NULL + new_stack_item)
+                     542 LOAD_FAST               15 (last_buff)
+                     544 LOAD_FAST               10 (line_idx2)
+                     546 LOAD_FAST                5 (stat_idx)
+                     548 LOAD_FAST                8 (line)
+                     550 PRECALL                  4
+                     554 CALL                     4
+         
+          71         564 PRECALL                  1
+                     568 CALL                     1
+                     578 POP_TOP
+         
+          74         580 LOAD_FAST                4 (path)
+                     582 LOAD_METHOD             10 (pop)
+                     604 LOAD_CONST               9 (-1)
+                     606 PRECALL                  1
+                     610 CALL                     1
+                     620 POP_TOP
+         
+          75         622 LOAD_FAST                2 (buffer)
+                     624 LOAD_METHOD             10 (pop)
+                     646 LOAD_CONST               9 (-1)
+                     648 PRECALL                  1
+                     652 CALL                     1
+                     662 POP_TOP
+         
+          76         664 LOAD_FAST                7 (stack_level)
+                     666 LOAD_METHOD             10 (pop)
+                     688 LOAD_CONST               9 (-1)
+                     690 PRECALL                  1
+                     694 CALL                     1
+                     704 POP_TOP
+                 >>  706 JUMP_BACKWARD          188 (to 332)
+         
+          61     >>  708 EXTENDED_ARG             1
+                     710 JUMP_BACKWARD          316 (to 80)
+         
+          79     >>  712 LOAD_GLOBAL             23 (NULL + struct_from_stack)
+                     724 LOAD_FAST                3 (stack)
+                     726 BUILD_LIST               0
+                     728 LOAD_CONST              11 (('function ', 'subroutine ', 'derived_type ', 'userdef_type ', 'pointer '))
+                     730 LIST_EXTEND              1
+                     732 KW_NAMES                12
+                     734 PRECALL                  2
+                     738 CALL                     2
+                     748 RETURN_VALUE
          consts
             'Extract structure from cleaned statements.'
             0
             None
             1
             ''
             '###==='
-            ('type_', 'name', 'first_line', 'line_idx', 'statement_idx')
-            'SOP'
+            ('type_', 'path', 'name', 'first_line', 'line_idx', 'statement_idx', 'verbose')
             '{'
             '}'
             -1
-            'EOP'
-            ('type_', 'name', 'path', 'start_line_idx', 'start_statement_idx', 'start_line', 'end_line_idx', 'end_statement_idx', 'end_line')
+            'Stop :'
             ('function ', 'subroutine ', 'derived_type ', 'userdef_type ', 'pointer ')
             ('main_types',)
-         names      ('zip', 'stmt', 'lines', 'print', '_parse_type_name_c', 'append', 'buffer_item', 'stack_item', 'copy', 'pop', 'struct_from_stack')
-         varnames   ('stmts', 'buffer', 'stack', 'path', 'stat_idx', 'level', 'stack_level', 'line', 'line_idx1', 'line_idx2', 'part', 'type_', 'name', 'char', 'line_start', 'line_idx', 'statement_idx')
+         names      ('zip', 'stmt', 'lines', '_parse_type_name_c', 'append', 'new_buffer_item', 'logger', 'critical', 'str', 'new_stack_item', 'pop', 'struct_from_stack')
+         varnames   ('stmts', 'verbose', 'buffer', 'stack', 'path', 'stat_idx', 'level', 'stack_level', 'line', 'line_idx1', 'line_idx2', 'part', 'type_', 'name', 'char', 'last_buff')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py'
          name       '_extract_on_cleaned_c'
-         firstlineno 26
+         firstlineno 27
          lnotab
-            0x020204010401040204020401060246010a0104011e03080124012a0118
-            010c01020102010201020102fb10ff10092a012001040208010a010c010a
-            010c010a01180120011c0118010c01020102012601020102010201020102
-            0102f710ff100d2a012a012ce8041b
+            0x020204010401040204020401060246010a010404080126012a012a0118
+            010c0102010201020102010201020102f910ff100b040208010a010c010a
+            010c010a011801040148011001180122ff10032a012a012cf10412
       'line'
+      'line_idx'
       code
-         argcount  : 1
-         nlocals   : 5
-         stacksize : 5
+         argcount  : 2
+         nlocals   : 6
+         stacksize : 7
          flags     : 3
          code
             0x97007c00a0000000000000000000000000000000000000000000a60000
             00ab00000000000000000064016b0200000000720264025300640344005d
-            327d017c00a0000000000000000000000000000000000000000000a60000
+            457d027c00a0000000000000000000000000000000000000000000a60000
             00ab000000000000000000a0010000000000000000000000000000000000
-            0000007c019b0064049d02a6010000ab01000000000000000072067c017c
-            0166026302010053008c337c00a002000000000000000000000000000000
-            000000000064056404a6020000ab020000000000000000a0030000000000
-            000000000000000000000000000000a6000000ab00000000000000000064
-            0664078502190000000000000000005c0200007d027d037c026408760072
-            0364097d046e287c02640a76007203640b7d046e217c02640c7600720364
-            0d7d046e1a7c02a004000000000000000000000000000000000000000064
-            0ea6010000ab0100000000000000007203640f7d046e0264107d047c047c
-            03a00500000000000000000000000000000000000000006411a6010000ab
-            01000000000000000066025300
-          98           0 RESUME                   0
+            0000007c029b0064049d02a6010000ab01000000000000000072197c027c
+            027405000000000000000000007c0164057a000000a6010000ab01000000
+            00000000007a00000066026302010053008c467c00a00300000000000000
+            0000000000000000000000000064066404a6020000ab0200000000000000
+            00a0040000000000000000000000000000000000000000a6000000ab0000
+            00000000000000640764088502190000000000000000005c0200007d037d
+            047c03640976007203640a7d056e287c03640b76007203640c7d056e217c
+            03640d76007203640e7d056e1a7c03a00500000000000000000000000000
+            00000000000000640fa6010000ab010000000000000000720364107d056e
+            0264117d057c057c04a00600000000000000000000000000000000000000
+            006412a6010000ab01000000000000000066025300
+          91           0 RESUME                   0
          
-         102           2 LOAD_FAST                0 (line)
+          95           2 LOAD_FAST                0 (line)
                        4 LOAD_METHOD              0 (strip)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 LOAD_CONST               1 ('')
                       42 COMPARE_OP               2 (==)
                       48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
          
-         103          50 LOAD_CONST               2 ((None, None))
+          96          50 LOAD_CONST               2 ((None, None))
                       52 RETURN_VALUE
          
-         105     >>   54 LOAD_CONST               3 (('for', 'if', 'else', 'switch'))
+          98     >>   54 LOAD_CONST               3 (('for', 'if', 'else', 'switch'))
                       56 GET_ITER
-                 >>   58 FOR_ITER                50 (to 160)
-                      60 STORE_FAST               1 (kw)
+                 >>   58 FOR_ITER                69 (to 198)
+                      60 STORE_FAST               2 (kw)
          
-         106          62 LOAD_FAST                0 (line)
+          99          62 LOAD_FAST                0 (line)
                       64 LOAD_METHOD              0 (strip)
                       86 PRECALL                  0
                       90 CALL                     0
                      100 LOAD_METHOD              1 (startswith)
-                     122 LOAD_FAST                1 (kw)
+                     122 LOAD_FAST                2 (kw)
                      124 FORMAT_VALUE             0
                      126 LOAD_CONST               4 (' ')
                      128 BUILD_STRING             2
                      130 PRECALL                  1
                      134 CALL                     1
-                     144 POP_JUMP_FORWARD_IF_FALSE     6 (to 158)
+                     144 POP_JUMP_FORWARD_IF_FALSE    25 (to 196)
          
-         107         146 LOAD_FAST                1 (kw)
-                     148 LOAD_FAST                1 (kw)
-                     150 BUILD_TUPLE              2
-                     152 SWAP                     2
-                     154 POP_TOP
-                     156 RETURN_VALUE
-         
-         106     >>  158 JUMP_BACKWARD           51 (to 58)
-         
-         109     >>  160 LOAD_FAST                0 (line)
-                     162 LOAD_METHOD              2 (replace)
-                     184 LOAD_CONST               5 ('(')
-                     186 LOAD_CONST               4 (' ')
-                     188 PRECALL                  2
-                     192 CALL                     2
-                     202 LOAD_METHOD              3 (split)
-                     224 PRECALL                  0
-                     228 CALL                     0
-                     238 LOAD_CONST               6 (0)
-                     240 LOAD_CONST               7 (2)
-                     242 BUILD_SLICE              2
-                     244 BINARY_SUBSCR
-                     254 UNPACK_SEQUENCE          2
-                     258 STORE_FAST               2 (rtype)
-                     260 STORE_FAST               3 (name)
-         
-         110         262 LOAD_FAST                2 (rtype)
-                     264 LOAD_CONST               8 (('void',))
-                     266 CONTAINS_OP              0
-                     268 POP_JUMP_FORWARD_IF_FALSE     3 (to 276)
-         
-         111         270 LOAD_CONST               9 ('subroutine ')
-                     272 STORE_FAST               4 (type_)
-                     274 JUMP_FORWARD            40 (to 356)
-         
-         112     >>  276 LOAD_FAST                2 (rtype)
-                     278 LOAD_CONST              10 (('int', 'double', 'char', 'float'))
-                     280 CONTAINS_OP              0
-                     282 POP_JUMP_FORWARD_IF_FALSE     3 (to 290)
-         
-         113         284 LOAD_CONST              11 ('function ')
-                     286 STORE_FAST               4 (type_)
-                     288 JUMP_FORWARD            33 (to 356)
-         
-         114     >>  290 LOAD_FAST                2 (rtype)
-                     292 LOAD_CONST              12 (('struct', 'enum', 'class'))
-                     294 CONTAINS_OP              0
-                     296 POP_JUMP_FORWARD_IF_FALSE     3 (to 304)
-         
-         115         298 LOAD_CONST              13 ('userdef_type ')
-                     300 STORE_FAST               4 (type_)
-                     302 JUMP_FORWARD            26 (to 356)
-         
-         116     >>  304 LOAD_FAST                2 (rtype)
-                     306 LOAD_METHOD              4 (endswith)
-                     328 LOAD_CONST              14 ('*')
-                     330 PRECALL                  1
-                     334 CALL                     1
-                     344 POP_JUMP_FORWARD_IF_FALSE     3 (to 352)
-         
-         117         346 LOAD_CONST              15 ('pointer ')
-                     348 STORE_FAST               4 (type_)
-                     350 JUMP_FORWARD             2 (to 356)
-         
-         119     >>  352 LOAD_CONST              16 ('unknown ')
-                     354 STORE_FAST               4 (type_)
-         
-         121     >>  356 LOAD_FAST                4 (type_)
-                     358 LOAD_FAST                3 (name)
-                     360 LOAD_METHOD              5 (rstrip)
-                     382 LOAD_CONST              17 ('{')
-                     384 PRECALL                  1
-                     388 CALL                     1
-                     398 BUILD_TUPLE              2
-                     400 RETURN_VALUE
+         100         146 LOAD_FAST                2 (kw)
+                     148 LOAD_FAST                2 (kw)
+                     150 LOAD_GLOBAL              5 (NULL + str)
+                     162 LOAD_FAST                1 (line_idx)
+                     164 LOAD_CONST               5 (1)
+                     166 BINARY_OP                0 (+)
+                     170 PRECALL                  1
+                     174 CALL                     1
+                     184 BINARY_OP                0 (+)
+                     188 BUILD_TUPLE              2
+                     190 SWAP                     2
+                     192 POP_TOP
+                     194 RETURN_VALUE
+         
+          99     >>  196 JUMP_BACKWARD           70 (to 58)
+         
+         102     >>  198 LOAD_FAST                0 (line)
+                     200 LOAD_METHOD              3 (replace)
+                     222 LOAD_CONST               6 ('(')
+                     224 LOAD_CONST               4 (' ')
+                     226 PRECALL                  2
+                     230 CALL                     2
+                     240 LOAD_METHOD              4 (split)
+                     262 PRECALL                  0
+                     266 CALL                     0
+                     276 LOAD_CONST               7 (0)
+                     278 LOAD_CONST               8 (2)
+                     280 BUILD_SLICE              2
+                     282 BINARY_SUBSCR
+                     292 UNPACK_SEQUENCE          2
+                     296 STORE_FAST               3 (rtype)
+                     298 STORE_FAST               4 (name)
+         
+         103         300 LOAD_FAST                3 (rtype)
+                     302 LOAD_CONST               9 (('void',))
+                     304 CONTAINS_OP              0
+                     306 POP_JUMP_FORWARD_IF_FALSE     3 (to 314)
+         
+         104         308 LOAD_CONST              10 ('subroutine ')
+                     310 STORE_FAST               5 (type_)
+                     312 JUMP_FORWARD            40 (to 394)
+         
+         105     >>  314 LOAD_FAST                3 (rtype)
+                     316 LOAD_CONST              11 (('int', 'double', 'char', 'float'))
+                     318 CONTAINS_OP              0
+                     320 POP_JUMP_FORWARD_IF_FALSE     3 (to 328)
+         
+         106         322 LOAD_CONST              12 ('function ')
+                     324 STORE_FAST               5 (type_)
+                     326 JUMP_FORWARD            33 (to 394)
+         
+         107     >>  328 LOAD_FAST                3 (rtype)
+                     330 LOAD_CONST              13 (('struct', 'enum', 'class'))
+                     332 CONTAINS_OP              0
+                     334 POP_JUMP_FORWARD_IF_FALSE     3 (to 342)
+         
+         108         336 LOAD_CONST              14 ('userdef_type ')
+                     338 STORE_FAST               5 (type_)
+                     340 JUMP_FORWARD            26 (to 394)
+         
+         109     >>  342 LOAD_FAST                3 (rtype)
+                     344 LOAD_METHOD              5 (endswith)
+                     366 LOAD_CONST              15 ('*')
+                     368 PRECALL                  1
+                     372 CALL                     1
+                     382 POP_JUMP_FORWARD_IF_FALSE     3 (to 390)
+         
+         110         384 LOAD_CONST              16 ('pointer ')
+                     386 STORE_FAST               5 (type_)
+                     388 JUMP_FORWARD             2 (to 394)
+         
+         112     >>  390 LOAD_CONST              17 ('unknown ')
+                     392 STORE_FAST               5 (type_)
+         
+         114     >>  394 LOAD_FAST                5 (type_)
+                     396 LOAD_FAST                4 (name)
+                     398 LOAD_METHOD              6 (rstrip)
+                     420 LOAD_CONST              18 ('{')
+                     422 PRECALL                  1
+                     426 CALL                     1
+                     436 BUILD_TUPLE              2
+                     438 RETURN_VALUE
          consts
             'expect a lowercase stripped line\n    takes the second word as the name\n    '
             ''
             (None, None)
             ('for', 'if', 'else', 'switch')
             ' '
+            1
             '('
             0
             2
             ('void',)
             'subroutine '
             ('int', 'double', 'char', 'float')
             'function '
             ('struct', 'enum', 'class')
             'userdef_type '
             '*'
             'pointer '
             'unknown '
             '{'
-         names      ('strip', 'startswith', 'replace', 'split', 'endswith', 'rstrip')
-         varnames   ('line', 'kw', 'rtype', 'name', 'type_')
+         names      ('strip', 'startswith', 'str', 'replace', 'split', 'endswith', 'rstrip')
+         varnames   ('line', 'line_idx', 'kw', 'rtype', 'name', 'type_')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py'
          name       '_parse_type_name_c'
-         firstlineno 98
+         firstlineno 91
          lnotab
-            0x020430010402080154010cff020366010801060108010601080106012a
+            0x0204300104020801540132ff020366010801060108010601080106012a
             0106020402
       'code'
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 7
          flags     : 3
@@ -633,50 +627,50 @@
             0x970067007d017c0044005d367d027c01a0000000000000000000000000
             0000000000000000007403000000000000000000007c02a0020000000000
             000000000000000000000000000000a6000000ab000000000000000000a6
             010000ab010000000000000000a6010000ab01000000000000000001008c
             37640184007407000000000000000000007c01a6010000ab010000000000
             0000004400a6000000ab0000000000000000007d03740900000000000000
             0000007c03a6010000ab0100000000000000005300
-         128           0 RESUME                   0
+         121           0 RESUME                   0
          
-         130           2 BUILD_LIST               0
+         123           2 BUILD_LIST               0
                        4 STORE_FAST               1 (candidates)
          
-         131           6 LOAD_FAST                0 (code)
+         124           6 LOAD_FAST                0 (code)
                        8 GET_ITER
                  >>   10 FOR_ITER                54 (to 120)
                       12 STORE_FAST               2 (line)
          
-         132          14 LOAD_FAST                1 (candidates)
+         125          14 LOAD_FAST                1 (candidates)
                       16 LOAD_METHOD              0 (extend)
                       38 LOAD_GLOBAL              3 (NULL + find_words_before_left_parenthesis)
                       50 LOAD_FAST                2 (line)
                       52 LOAD_METHOD              2 (strip)
                       74 PRECALL                  0
                       78 CALL                     0
                       88 PRECALL                  1
                       92 CALL                     1
                      102 PRECALL                  1
                      106 CALL                     1
                      116 POP_TOP
                      118 JUMP_BACKWARD           55 (to 10)
          
-         136     >>  120 LOAD_CONST               1 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py", line 136>)
+         129     >>  120 LOAD_CONST               1 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py", line 129>)
                      122 MAKE_FUNCTION            0
                      124 LOAD_GLOBAL              7 (NULL + set)
                      136 LOAD_FAST                1 (candidates)
                      138 PRECALL                  1
                      142 CALL                     1
                      152 GET_ITER
                      154 PRECALL                  0
                      158 CALL                     0
                      168 STORE_FAST               3 (matches)
          
-         137         170 LOAD_GLOBAL              9 (NULL + sorted)
+         130         170 LOAD_GLOBAL              9 (NULL + sorted)
                      182 LOAD_FAST                3 (matches)
                      184 PRECALL                  1
                      188 CALL                     1
                      198 RETURN_VALUE
          consts
             'Find callables in c'
             code
@@ -684,15 +678,15 @@
                nlocals   : 2
                stacksize : 4
                flags     : 19
                code
                   0x970067007c005d1f7d017c017400000000000000000000007601af0b7c
                   01a0010000000000000000000000000000000000000000a6000000ab0000
                   0000000000000091028c205300
-               136           0 RESUME                   0
+               129           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                31 (to 70)
                              8 STORE_FAST               1 (cand)
                             10 LOAD_FAST                1 (cand)
                             12 LOAD_GLOBAL              0 (KEYWORDS_C)
                             24 CONTAINS_OP              1
@@ -707,75 +701,76 @@
                consts
                names      ('KEYWORDS_C', 'strip')
                varnames   ('.0', 'cand')
                freevars   ()
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py'
                name       '<listcomp>'
-               firstlineno 136
+               firstlineno 129
                lnotab 0x
          names      ('extend', 'find_words_before_left_parenthesis', 'strip', 'set', 'sorted')
          varnames   ('code', 'candidates', 'line', 'matches')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py'
          name       'find_callables_c'
-         firstlineno 128
+         firstlineno 121
          lnotab 0x0202040108016a043201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a01000000000000000064016402a0
             0200000000000000000000000000000000000000007c00a6010000ab0100
             00000000000000a6020000ab0200000000000000007d0174070000000000
             00000000007c01a6010000ab01000000000000000064037a0000007d027c
             025300
-         140           0 RESUME                   0
+         133           0 RESUME                   0
          
-         142           2 LOAD_GLOBAL              1 (NULL + re)
+         135           2 LOAD_GLOBAL              1 (NULL + re)
                       14 LOAD_ATTR                1 (findall)
          
-         143          24 LOAD_CONST               1 ('(?i)(if |else |for |case |default )')
+         136          24 LOAD_CONST               1 ('(?i)(if |else |for |case |default )')
                       26 LOAD_CONST               2 ('\n')
                       28 LOAD_METHOD              2 (join)
                       50 LOAD_FAST                0 (code)
                       52 PRECALL                  1
                       56 CALL                     1
          
-         142          66 PRECALL                  2
+         135          66 PRECALL                  2
                       70 CALL                     2
                       80 STORE_FAST               1 (decision_points)
          
-         145          82 LOAD_GLOBAL              7 (NULL + len)
+         138          82 LOAD_GLOBAL              7 (NULL + len)
                       94 LOAD_FAST                1 (decision_points)
                       96 PRECALL                  1
                      100 CALL                     1
                      110 LOAD_CONST               3 (1)
                      112 BINARY_OP                0 (+)
                      116 STORE_FAST               2 (complexity)
          
-         146         118 LOAD_FAST                2 (complexity)
+         139         118 LOAD_FAST                2 (complexity)
                      120 RETURN_VALUE
          consts
             'Count decision points (if, else if, do, select, etc.)'
             '(?i)(if |else |for |case |default )'
             '\n'
             1
          names      ('re', 'findall', 'join', 'len')
          varnames   ('code', 'decision_points', 'complexity')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py'
          name       'compute_ccn_approx_c'
-         firstlineno 140
+         firstlineno 133
          lnotab 0x020216012aff10032401
-   names      ('re', 'typing', 'Tuple', 'List', 'loguru', 'logger', 'tucan.unformat_common', 'Statements', 'tucan.struct_common', 'find_words_before_left_parenthesis', 'buffer_item', 'stack_item', 'struct_from_stack', 'struct_augment', 'tucan.kw_lang', 'KEYWORDS_C', 'dict', 'extract_struct_c', '_extract_on_cleaned_c', 'str', '_parse_type_name_c', 'list', 'find_callables_c', 'int', 'compute_ccn_approx_c')
+      (False,)
+   names      ('re', 'typing', 'Tuple', 'List', 'loguru', 'logger', 'tucan.unformat_common', 'Statements', 'tucan.struct_common', 'find_words_before_left_parenthesis', 'new_buffer_item', 'new_stack_item', 'struct_from_stack', 'struct_augment', 'tucan.kw_lang', 'KEYWORDS_C', 'bool', 'dict', 'extract_struct_c', '_extract_on_cleaned_c', 'str', 'int', '_parse_type_name_c', 'list', 'find_callables_c', 'compute_ccn_approx_c')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_c.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201080110010c010c011c080c02100b1048201e100c
+   lnotab 0x00ff0201080110010c010c011c080c02140c1640241e100c
```

### Comparing `tucan-0.1.0/src/tucan/__pycache__/struct_common.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/struct_ftn.cpython-311.pyc`

 * *Files 25% similar despite different names*

#### Python bytecode

```diff
@@ -1,1980 +1,1432 @@
 magic:    0xa70d0d0a
-moddate:  0x97a6b365 (Fri Jan 26 12:33:27 2024 UTC)
-files sz: 9078
+moddate:  0xa07b4266 (Mon May 13 20:44:16 2024 UTC)
+files sz: 7560
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 29
+   stacksize : 5
    flags     : 0
    code
-      0x970064005a00640164026c015a01640164036c026d035a036d045a046d
-      055a050100640164046c066d075a070100640164056c086d095a09010064
-      06650a64076503650a190000000000000000006604640884045a0b640665
-      0a6409650c6604640a84045a0d640b650c64096504650c19000000000000
-      0000006604640c84045a0e640d650f6409650c6604640e84045a10640f65
-      0c64096504650c190000000000000000006604641084045a116411650c64
-      12650c6413650c641465126415651264096503650c650c650c6512651266
-      0519000000000000000000660c641684045a136411650c6412650c640665
-      0a64176512641865126419650c641a6512641b6512641c650c6409650365
-      0c650c650a65126512650c65126512650c66091900000000000000000066
-      14641d84045a146431641e650a641f650a6420650a6409650f6608642184
-      055a156422650f6409650f6604642384045a166424650a6425650c640965
-      0a6606642684045a17642765126428651264296504650a19000000000000
-      000000640965046608642a84045a18642b650f6412650c6409650a660664
-      2c84045a19642b650f642d6504650c19000000000000000000642e650564
-      2f65056409650f660a643084045a1a64025300
+      0x9700640064016c005a00640064026c016d025a020100640064036c036d
+      045a040100640064046c056d065a066d075a076d085a086d095a096d0a5a
+      0a0100640064056c036d0b5a0b0100640064066c0c6d0d5a0d6d0e5a0e6d
+      0f5a0f010002006510650d6407ac08a6020000ab0200000000000000005a
+      1102006510650e6407ac08a6020000ab0200000000000000005a12650f5a
+      1364096504640a65146604640b84045a15641464096504640a6514660464
+      0d84055a16640e6517640f65186604641084045a196411651a640a651a66
+      04641284045a1b6411651a640a65186604641384045a1c64015300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('\nModule that gather the most common functions of struct.\n')
-                 4 STORE_NAME               0 (__doc__)
-   
-     5           6 LOAD_CONST               1 (0)
-                 8 LOAD_CONST               2 (None)
-                10 IMPORT_NAME              1 (re)
-                12 STORE_NAME               1 (re)
-   
-     6          14 LOAD_CONST               1 (0)
-                16 LOAD_CONST               3 (('Tuple', 'List', 'Callable'))
-                18 IMPORT_NAME              2 (typing)
-                20 IMPORT_FROM              3 (Tuple)
-                22 STORE_NAME               3 (Tuple)
-                24 IMPORT_FROM              4 (List)
-                26 STORE_NAME               4 (List)
-                28 IMPORT_FROM              5 (Callable)
-                30 STORE_NAME               5 (Callable)
+     1           2 LOAD_CONST               0 (0)
+                 4 LOAD_CONST               1 (None)
+                 6 IMPORT_NAME              0 (re)
+                 8 STORE_NAME               0 (re)
+   
+     2          10 LOAD_CONST               0 (0)
+                12 LOAD_CONST               2 (('logger',))
+                14 IMPORT_NAME              1 (loguru)
+                16 IMPORT_FROM              2 (logger)
+                18 STORE_NAME               2 (logger)
+                20 POP_TOP
+   
+     3          22 LOAD_CONST               0 (0)
+                24 LOAD_CONST               3 (('Statements',))
+                26 IMPORT_NAME              3 (tucan.unformat_common)
+                28 IMPORT_FROM              4 (Statements)
+                30 STORE_NAME               4 (Statements)
                 32 POP_TOP
    
-     7          34 LOAD_CONST               1 (0)
-                36 LOAD_CONST               4 (('deepcopy',))
-                38 IMPORT_NAME              6 (copy)
-                40 IMPORT_FROM              7 (deepcopy)
-                42 STORE_NAME               7 (deepcopy)
-                44 POP_TOP
-   
-     8          46 LOAD_CONST               1 (0)
-                48 LOAD_CONST               5 (('logger',))
-                50 IMPORT_NAME              8 (loguru)
-                52 IMPORT_FROM              9 (logger)
-                54 STORE_NAME               9 (logger)
-                56 POP_TOP
-   
-    10          58 LOAD_CONST               6 ('path')
-                60 LOAD_NAME               10 (list)
-                62 LOAD_CONST               7 ('paths_to_clean')
-                64 LOAD_NAME                3 (Tuple)
-                66 LOAD_NAME               10 (list)
-                68 BINARY_SUBSCR
-                78 BUILD_TUPLE              4
-                80 LOAD_CONST               8 (<code object path_clean, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 10>)
-                82 MAKE_FUNCTION            4 (annotations)
-                84 STORE_NAME              11 (path_clean)
-   
-    23          86 LOAD_CONST               6 ('path')
-                88 LOAD_NAME               10 (list)
-                90 LOAD_CONST               9 ('return')
-                92 LOAD_NAME               12 (str)
-                94 BUILD_TUPLE              4
-                96 LOAD_CONST              10 (<code object list2pathref, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 23>)
-                98 MAKE_FUNCTION            4 (annotations)
-               100 STORE_NAME              13 (list2pathref)
-   
-    28         102 LOAD_CONST              11 ('pathstr')
-               104 LOAD_NAME               12 (str)
-               106 LOAD_CONST               9 ('return')
-               108 LOAD_NAME                4 (List)
-               110 LOAD_NAME               12 (str)
-               112 BINARY_SUBSCR
-               122 BUILD_TUPLE              4
-               124 LOAD_CONST              12 (<code object pathref_ascendants, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 28>)
-               126 MAKE_FUNCTION            4 (annotations)
-               128 STORE_NAME              14 (pathref_ascendants)
-   
-    38         130 LOAD_CONST              13 ('main_structs')
-               132 LOAD_NAME               15 (dict)
-               134 LOAD_CONST               9 ('return')
-               136 LOAD_NAME               12 (str)
-               138 BUILD_TUPLE              4
-               140 LOAD_CONST              14 (<code object struct_summary_str, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 38>)
-               142 MAKE_FUNCTION            4 (annotations)
-               144 STORE_NAME              16 (struct_summary_str)
-   
-    71         146 LOAD_CONST              15 ('line')
-               148 LOAD_NAME               12 (str)
-               150 LOAD_CONST               9 ('return')
-               152 LOAD_NAME                4 (List)
-               154 LOAD_NAME               12 (str)
-               156 BINARY_SUBSCR
-               166 BUILD_TUPLE              4
-               168 LOAD_CONST              16 (<code object find_words_before_left_parenthesis, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 71>)
-               170 MAKE_FUNCTION            4 (annotations)
-               172 STORE_NAME              17 (find_words_before_left_parenthesis)
-   
-   102         174 LOAD_CONST              17 ('type_')
-   
-   103         176 LOAD_NAME               12 (str)
-   
-   102         178 LOAD_CONST              18 ('name')
-   
-   104         180 LOAD_NAME               12 (str)
-   
-   102         182 LOAD_CONST              19 ('first_line')
-   
-   105         184 LOAD_NAME               12 (str)
-   
-   102         186 LOAD_CONST              20 ('line_idx')
-   
-   106         188 LOAD_NAME               18 (int)
-   
-   102         190 LOAD_CONST              21 ('statement_idx')
-   
-   107         192 LOAD_NAME               18 (int)
-   
-   102         194 LOAD_CONST               9 ('return')
-   
-   108         196 LOAD_NAME                3 (Tuple)
-               198 LOAD_NAME               12 (str)
-               200 LOAD_NAME               12 (str)
-               202 LOAD_NAME               12 (str)
-               204 LOAD_NAME               18 (int)
-               206 LOAD_NAME               18 (int)
-               208 BUILD_TUPLE              5
-               210 BINARY_SUBSCR
-   
-   102         220 BUILD_TUPLE             12
-               222 LOAD_CONST              22 (<code object buffer_item, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 102>)
-               224 MAKE_FUNCTION            4 (annotations)
-               226 STORE_NAME              19 (buffer_item)
-   
-   123         228 LOAD_CONST              17 ('type_')
-   
-   124         230 LOAD_NAME               12 (str)
-   
-   123         232 LOAD_CONST              18 ('name')
-   
-   125         234 LOAD_NAME               12 (str)
-   
-   123         236 LOAD_CONST               6 ('path')
-   
-   126         238 LOAD_NAME               10 (list)
-   
-   123         240 LOAD_CONST              23 ('start_line_idx')
-   
-   127         242 LOAD_NAME               18 (int)
-   
-   123         244 LOAD_CONST              24 ('start_statement_idx')
-   
-   128         246 LOAD_NAME               18 (int)
-   
-   123         248 LOAD_CONST              25 ('start_line')
-   
-   129         250 LOAD_NAME               12 (str)
-   
-   123         252 LOAD_CONST              26 ('end_line_idx')
-   
-   130         254 LOAD_NAME               18 (int)
-   
-   123         256 LOAD_CONST              27 ('end_statement_idx')
-   
-   131         258 LOAD_NAME               18 (int)
-   
-   123         260 LOAD_CONST              28 ('end_line')
-   
-   132         262 LOAD_NAME               12 (str)
-   
-   123         264 LOAD_CONST               9 ('return')
-   
-   133         266 LOAD_NAME                3 (Tuple)
-               268 LOAD_NAME               12 (str)
-               270 LOAD_NAME               12 (str)
-               272 LOAD_NAME               10 (list)
-               274 LOAD_NAME               18 (int)
-               276 LOAD_NAME               18 (int)
-               278 LOAD_NAME               12 (str)
-               280 LOAD_NAME               18 (int)
-               282 LOAD_NAME               18 (int)
-               284 LOAD_NAME               12 (str)
-               286 BUILD_TUPLE              9
-               288 BINARY_SUBSCR
-   
-   123         298 BUILD_TUPLE             20
-               300 LOAD_CONST              29 (<code object stack_item, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 123>)
-               302 MAKE_FUNCTION            4 (annotations)
-               304 STORE_NAME              20 (stack_item)
-   
-   155         306 LOAD_CONST              49 ((None,))
-               308 LOAD_CONST              30 ('stack')
-               310 LOAD_NAME               10 (list)
-               312 LOAD_CONST              31 ('main_types')
-               314 LOAD_NAME               10 (list)
-               316 LOAD_CONST              32 ('skip_types')
-               318 LOAD_NAME               10 (list)
-               320 LOAD_CONST               9 ('return')
-               322 LOAD_NAME               15 (dict)
-               324 BUILD_TUPLE              8
-               326 LOAD_CONST              33 (<code object struct_from_stack, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 155>)
-               328 MAKE_FUNCTION            5 (defaults, annotations)
-               330 STORE_NAME              21 (struct_from_stack)
-   
-   197         332 LOAD_CONST              34 ('struct')
-               334 LOAD_NAME               15 (dict)
-               336 LOAD_CONST               9 ('return')
-               338 LOAD_NAME               15 (dict)
-               340 BUILD_TUPLE              4
-               342 LOAD_CONST              35 (<code object get_struct_sizes, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 197>)
-               344 MAKE_FUNCTION            4 (annotations)
-               346 STORE_NAME              22 (get_struct_sizes)
-   
-   210         348 LOAD_CONST              36 ('list_')
-               350 LOAD_NAME               10 (list)
-               352 LOAD_CONST              37 ('parent')
-               354 LOAD_NAME               12 (str)
-               356 LOAD_CONST               9 ('return')
-               358 LOAD_NAME               10 (list)
-               360 BUILD_TUPLE              6
-               362 LOAD_CONST              38 (<code object replace_self, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 210>)
-               364 MAKE_FUNCTION            4 (annotations)
-               366 STORE_NAME              23 (replace_self)
-   
-   218         368 LOAD_CONST              39 ('beg')
-               370 LOAD_NAME               18 (int)
-               372 LOAD_CONST              40 ('end')
-               374 LOAD_NAME               18 (int)
-               376 LOAD_CONST              41 ('safes')
-               378 LOAD_NAME                4 (List)
-               380 LOAD_NAME               10 (list)
-               382 BINARY_SUBSCR
-               392 LOAD_CONST               9 ('return')
-               394 LOAD_NAME                4 (List)
-               396 BUILD_TUPLE              8
-               398 LOAD_CONST              42 (<code object _strip_safe_lines, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 218>)
-               400 MAKE_FUNCTION            4 (annotations)
-               402 STORE_NAME              24 (_strip_safe_lines)
-   
-   242         404 LOAD_CONST              43 ('struct_in')
-               406 LOAD_NAME               15 (dict)
-               408 LOAD_CONST              18 ('name')
-               410 LOAD_NAME               12 (str)
-               412 LOAD_CONST               9 ('return')
-               414 LOAD_NAME               10 (list)
-               416 BUILD_TUPLE              6
-               418 LOAD_CONST              44 (<code object struct_actual_lines, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 242>)
-               420 MAKE_FUNCTION            4 (annotations)
-               422 STORE_NAME              25 (struct_actual_lines)
-   
-   256         424 LOAD_CONST              43 ('struct_in')
-               426 LOAD_NAME               15 (dict)
-               428 LOAD_CONST              45 ('clean_code')
-               430 LOAD_NAME                4 (List)
-               432 LOAD_NAME               12 (str)
-               434 BINARY_SUBSCR
-               444 LOAD_CONST              46 ('find_callables')
-               446 LOAD_NAME                5 (Callable)
-               448 LOAD_CONST              47 ('compute_ccn')
-               450 LOAD_NAME                5 (Callable)
-               452 LOAD_CONST               9 ('return')
-               454 LOAD_NAME               15 (dict)
-               456 BUILD_TUPLE             10
-               458 LOAD_CONST              48 (<code object struct_augment, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 256>)
-               460 MAKE_FUNCTION            4 (annotations)
-               462 STORE_NAME              26 (struct_augment)
-               464 LOAD_CONST               2 (None)
-               466 RETURN_VALUE
+     4          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               4 (('find_words_before_left_parenthesis', 'new_buffer_item', 'new_stack_item', 'struct_from_stack', 'struct_augment'))
+                38 IMPORT_NAME              5 (tucan.struct_common)
+                40 IMPORT_FROM              6 (find_words_before_left_parenthesis)
+                42 STORE_NAME               6 (find_words_before_left_parenthesis)
+                44 IMPORT_FROM              7 (new_buffer_item)
+                46 STORE_NAME               7 (new_buffer_item)
+                48 IMPORT_FROM              8 (new_stack_item)
+                50 STORE_NAME               8 (new_stack_item)
+                52 IMPORT_FROM              9 (struct_from_stack)
+                54 STORE_NAME               9 (struct_from_stack)
+                56 IMPORT_FROM             10 (struct_augment)
+                58 STORE_NAME              10 (struct_augment)
+                60 POP_TOP
+   
+    11          62 LOAD_CONST               0 (0)
+                64 LOAD_CONST               5 (('rm_parenthesis_content',))
+                66 IMPORT_NAME              3 (tucan.unformat_common)
+                68 IMPORT_FROM             11 (rm_parenthesis_content)
+                70 STORE_NAME              11 (rm_parenthesis_content)
+                72 POP_TOP
+   
+    15          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               6 (('STRUCTURES_FTN', 'NESTS_FTN', 'OTHERS_FTN'))
+                78 IMPORT_NAME             12 (tucan.kw_lang)
+                80 IMPORT_FROM             13 (STRUCTURES_FTN)
+                82 STORE_NAME              13 (STRUCTURES_FTN)
+                84 IMPORT_FROM             14 (NESTS_FTN)
+                86 STORE_NAME              14 (NESTS_FTN)
+                88 IMPORT_FROM             15 (OTHERS_FTN)
+                90 STORE_NAME              15 (OTHERS_FTN)
+                92 POP_TOP
+   
+    18          94 PUSH_NULL
+                96 LOAD_NAME               16 (sorted)
+                98 LOAD_NAME               13 (STRUCTURES_FTN)
+               100 LOAD_CONST               7 (True)
+               102 KW_NAMES                 8
+               104 PRECALL                  2
+               108 CALL                     2
+               118 STORE_NAME              17 (PARTS)
+   
+    19         120 PUSH_NULL
+               122 LOAD_NAME               16 (sorted)
+               124 LOAD_NAME               14 (NESTS_FTN)
+               126 LOAD_CONST               7 (True)
+               128 KW_NAMES                 8
+               130 PRECALL                  2
+               134 CALL                     2
+               144 STORE_NAME              18 (NESTS)
+   
+    20         146 LOAD_NAME               15 (OTHERS_FTN)
+               148 STORE_NAME              19 (INTRINSICS)
+   
+    23         150 LOAD_CONST               9 ('stmts')
+               152 LOAD_NAME                4 (Statements)
+               154 LOAD_CONST              10 ('return')
+               156 LOAD_NAME               20 (dict)
+               158 BUILD_TUPLE              4
+               160 LOAD_CONST              11 (<code object extract_struct_ftn, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py", line 23>)
+               162 MAKE_FUNCTION            4 (annotations)
+               164 STORE_NAME              21 (extract_struct_ftn)
+   
+    38         166 LOAD_CONST              20 ((False,))
+               168 LOAD_CONST               9 ('stmts')
+               170 LOAD_NAME                4 (Statements)
+               172 LOAD_CONST              10 ('return')
+               174 LOAD_NAME               20 (dict)
+               176 BUILD_TUPLE              4
+               178 LOAD_CONST              13 (<code object _extract_on_cleaned_ftn, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py", line 38>)
+               180 MAKE_FUNCTION            5 (defaults, annotations)
+               182 STORE_NAME              22 (_extract_on_cleaned_ftn)
+   
+   176         184 LOAD_CONST              14 ('line')
+               186 LOAD_NAME               23 (str)
+               188 LOAD_CONST              15 ('line_nb')
+               190 LOAD_NAME               24 (int)
+               192 BUILD_TUPLE              4
+               194 LOAD_CONST              16 (<code object _parse_name_ftn, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py", line 176>)
+               196 MAKE_FUNCTION            4 (annotations)
+               198 STORE_NAME              25 (_parse_name_ftn)
+   
+   210         200 LOAD_CONST              17 ('code')
+               202 LOAD_NAME               26 (list)
+               204 LOAD_CONST              10 ('return')
+               206 LOAD_NAME               26 (list)
+               208 BUILD_TUPLE              4
+               210 LOAD_CONST              18 (<code object find_callables_ftn, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py", line 210>)
+               212 MAKE_FUNCTION            4 (annotations)
+               214 STORE_NAME              27 (find_callables_ftn)
+   
+   224         216 LOAD_CONST              17 ('code')
+               218 LOAD_NAME               26 (list)
+               220 LOAD_CONST              10 ('return')
+               222 LOAD_NAME               24 (int)
+               224 BUILD_TUPLE              4
+               226 LOAD_CONST              19 (<code object compute_ccn_approx_ftn, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py", line 224>)
+               228 MAKE_FUNCTION            4 (annotations)
+               230 STORE_NAME              28 (compute_ccn_approx_ftn)
+               232 LOAD_CONST               1 (None)
+               234 RETURN_VALUE
    consts
-      '\nModule that gather the most common functions of struct.\n'
       0
       None
-      ('Tuple', 'List', 'Callable')
-      ('deepcopy',)
       ('logger',)
-      'path'
-      'paths_to_clean'
+      ('Statements',)
+      ('find_words_before_left_parenthesis', 'new_buffer_item', 'new_stack_item', 'struct_from_stack', 'struct_augment')
+      ('rm_parenthesis_content',)
+      ('STRUCTURES_FTN', 'NESTS_FTN', 'OTHERS_FTN')
+      True
+      ('reverse',)
+      'stmts'
+      'return'
       code
          argcount  : 2
-         nlocals   : 7
+         nlocals   : 4
          stacksize : 6
          flags     : 3
          code
-            0x970067007d027c0144005d567d037401000000000000000000007c00a6
-            010000ab010000000000000000a001000000000000000000000000000000
-            00000000007401000000000000000000007c03a6010000ab010000000000
-            000000a6010000ab01000000000000000072257c02a00200000000000000
-            000000000000000000000000007407000000000000000000007c03a60100
-            00ab01000000000000000064017a0a0000a6010000ab0100000000000000
-            0001008c5767007d047409000000000000000000007c00a6010000ab0100
-            0000000000000044005d1e5c0200007d057d067c057c02760172157c04a0
-            0200000000000000000000000000000000000000007c06a6010000ab0100
-            0000000000000001008c1f7c045300
-          10           0 RESUME                   0
-         
-          12           2 BUILD_LIST               0
-                       4 STORE_FAST               2 (indexes_to_clean)
-         
-          13           6 LOAD_FAST                1 (paths_to_clean)
-                       8 GET_ITER
-                 >>   10 FOR_ITER                86 (to 184)
-                      12 STORE_FAST               3 (ptc)
-         
-          14          14 LOAD_GLOBAL              1 (NULL + list2pathref)
-                      26 LOAD_FAST                0 (path)
-                      28 PRECALL                  1
-                      32 CALL                     1
-                      42 LOAD_METHOD              1 (startswith)
-                      64 LOAD_GLOBAL              1 (NULL + list2pathref)
-                      76 LOAD_FAST                3 (ptc)
-                      78 PRECALL                  1
-                      82 CALL                     1
-                      92 PRECALL                  1
-                      96 CALL                     1
-                     106 POP_JUMP_FORWARD_IF_FALSE    37 (to 182)
-         
-          15         108 LOAD_FAST                2 (indexes_to_clean)
-                     110 LOAD_METHOD              2 (append)
-                     132 LOAD_GLOBAL              7 (NULL + len)
-                     144 LOAD_FAST                3 (ptc)
-                     146 PRECALL                  1
-                     150 CALL                     1
-                     160 LOAD_CONST               1 (1)
-                     162 BINARY_OP               10 (-)
-                     166 PRECALL                  1
-                     170 CALL                     1
-                     180 POP_TOP
-                 >>  182 JUMP_BACKWARD           87 (to 10)
-         
-          16     >>  184 BUILD_LIST               0
-                     186 STORE_FAST               4 (new_path)
-         
-          17         188 LOAD_GLOBAL              9 (NULL + enumerate)
-                     200 LOAD_FAST                0 (path)
-                     202 PRECALL                  1
-                     206 CALL                     1
-                     216 GET_ITER
-                 >>  218 FOR_ITER                30 (to 280)
-                     220 UNPACK_SEQUENCE          2
-                     224 STORE_FAST               5 (i)
-                     226 STORE_FAST               6 (step)
-         
-          18         228 LOAD_FAST                5 (i)
-                     230 LOAD_FAST                2 (indexes_to_clean)
-                     232 CONTAINS_OP              1
-                     234 POP_JUMP_FORWARD_IF_FALSE    21 (to 278)
-         
-          19         236 LOAD_FAST                4 (new_path)
-                     238 LOAD_METHOD              2 (append)
-                     260 LOAD_FAST                6 (step)
-                     262 PRECALL                  1
-                     266 CALL                     1
-                     276 POP_TOP
-                 >>  278 JUMP_BACKWARD           31 (to 218)
-         
-          20     >>  280 LOAD_FAST                4 (new_path)
-                     282 RETURN_VALUE
-         consts
-            'Remove the unwanted steps of the paths'
-            1
-         names      ('list2pathref', 'startswith', 'append', 'len', 'enumerate')
-         varnames   ('path', 'paths_to_clean', 'indexes_to_clean', 'ptc', 'new_path', 'i', 'step')
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       'path_clean'
-         firstlineno 10
-         lnotab 0x0202040108015e014c010401280108012c01
-      'return'
-      code
-         argcount  : 1
-         nlocals   : 1
-         stacksize : 3
-         flags     : 3
-         code
-            0x97006401a00000000000000000000000000000000000000000007c00a6
-            010000ab0100000000000000005300
+            0x97007c00a0000000000000000000000000000000000000000000a60000
+            00ab0000000000000000007d0209007403000000000000000000007c007c
+            01ac01a6020000ab0200000000000000007d036e11230074040000000000
+            000000000024007204010059006402530077007803590077017407000000
+            000000000000007c037c02740800000000000000000000740a0000000000
+            0000000000a6040000ab0400000000000000007d037c035300
           23           0 RESUME                   0
          
-          25           2 LOAD_CONST               1 ('.')
-                       4 LOAD_METHOD              0 (join)
-                      26 LOAD_FAST                0 (path)
-                      28 PRECALL                  1
-                      32 CALL                     1
-                      42 RETURN_VALUE
-         consts
-            'The way we will refer to path here in strings'
-            '.'
-         names      ('join',)
-         varnames   ('path',)
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       'list2pathref'
-         firstlineno 23
-         lnotab 0x0202
-      'pathstr'
-      code
-         argcount  : 1
-         nlocals   : 3
-         stacksize : 5
-         flags     : 3
-         code
-            0x970067007d017c00a00000000000000000000000000000000000000000
-            006401a6010000ab0100000000000000007d027403000000000000000000
-            007c02a6010000ab01000000000000000064026b0400000000724a7c02a0
-            0200000000000000000000000000000000000000006403a6010000ab0100
-            0000000000000001007c01a0030000000000000000000000000000000000
-            0000007409000000000000000000007c02a6010000ab0100000000000000
-            00a6010000ab01000000000000000001007403000000000000000000007c
-            02a6010000ab01000000000000000064026b0400000000b04a7c015300
-          28           0 RESUME                   0
-         
-          30           2 BUILD_LIST               0
-                       4 STORE_FAST               1 (out)
-         
-          31           6 LOAD_FAST                0 (pathstr)
-                       8 LOAD_METHOD              0 (split)
-                      30 LOAD_CONST               1 ('.')
-                      32 PRECALL                  1
-                      36 CALL                     1
-                      46 STORE_FAST               2 (path)
-         
-          32          48 LOAD_GLOBAL              3 (NULL + len)
-                      60 LOAD_FAST                2 (path)
-                      62 PRECALL                  1
-                      66 CALL                     1
-                      76 LOAD_CONST               2 (1)
-                      78 COMPARE_OP               4 (>)
-                      84 POP_JUMP_FORWARD_IF_FALSE    74 (to 234)
-         
-          33     >>   86 LOAD_FAST                2 (path)
-                      88 LOAD_METHOD              2 (pop)
-                     110 LOAD_CONST               3 (-1)
-                     112 PRECALL                  1
-                     116 CALL                     1
-                     126 POP_TOP
-         
-          34         128 LOAD_FAST                1 (out)
-                     130 LOAD_METHOD              3 (append)
-                     152 LOAD_GLOBAL              9 (NULL + list2pathref)
-                     164 LOAD_FAST                2 (path)
-                     166 PRECALL                  1
-                     170 CALL                     1
-                     180 PRECALL                  1
-                     184 CALL                     1
-                     194 POP_TOP
-         
-          32         196 LOAD_GLOBAL              3 (NULL + len)
-                     208 LOAD_FAST                2 (path)
-                     210 PRECALL                  1
-                     214 CALL                     1
-                     224 LOAD_CONST               2 (1)
-                     226 COMPARE_OP               4 (>)
-                     232 POP_JUMP_BACKWARD_IF_TRUE    74 (to 86)
+          28           2 LOAD_FAST                0 (stmts)
+                       4 LOAD_METHOD              0 (to_code)
+                      26 PRECALL                  0
+                      30 CALL                     0
+                      40 STORE_FAST               2 (clean_code)
+         
+          30          42 NOP
+         
+          31          44 LOAD_GLOBAL              3 (NULL + _extract_on_cleaned_ftn)
+                      56 LOAD_FAST                0 (stmts)
+                      58 LOAD_FAST                1 (verbose)
+                      60 KW_NAMES                 1
+                      62 PRECALL                  2
+                      66 CALL                     2
+                      76 STORE_FAST               3 (all_structs)
+                      78 JUMP_FORWARD            17 (to 114)
+                 >>   80 PUSH_EXC_INFO
+         
+          32          82 LOAD_GLOBAL              4 (RuntimeError)
+                      94 CHECK_EXC_MATCH
+                      96 POP_JUMP_FORWARD_IF_FALSE     4 (to 106)
+                      98 POP_TOP
+         
+          33         100 POP_EXCEPT
+                     102 LOAD_CONST               2 (None)
+                     104 RETURN_VALUE
+         
+          32     >>  106 RERAISE                  0
+                 >>  108 COPY                     3
+                     110 POP_EXCEPT
+                     112 RERAISE                  1
+         
+          34     >>  114 LOAD_GLOBAL              7 (NULL + struct_augment)
+                     126 LOAD_FAST                3 (all_structs)
+                     128 LOAD_FAST                2 (clean_code)
+                     130 LOAD_GLOBAL              8 (find_callables_ftn)
+                     142 LOAD_GLOBAL             10 (compute_ccn_approx_ftn)
+                     154 PRECALL                  4
+                     158 CALL                     4
+                     168 STORE_FAST               3 (all_structs)
          
-          35     >>  234 LOAD_FAST                1 (out)
-                     236 RETURN_VALUE
+          35         170 LOAD_FAST                3 (all_structs)
+                     172 RETURN_VALUE
+         ExceptionTable:
+           44 to 76 -> 80 [0]
+           80 to 98 -> 108 [1] lasti
+           106 to 106 -> 108 [1] lasti
          consts
-            'Return all ascendends of a path'
-            '.'
-            1
-            -1
-         names      ('split', 'len', 'pop', 'append', 'list2pathref')
-         varnames   ('pathstr', 'out', 'path')
+            'Main calls to build structure form statements\n\n    statements is the output of tucan.unformat_ftn.unformat_ftn\n    '
+            ('verbose',)
+            None
+         names      ('to_code', '_extract_on_cleaned_ftn', 'RuntimeError', 'struct_augment', 'find_callables_ftn', 'compute_ccn_approx_ftn')
+         varnames   ('stmts', 'verbose', 'clean_code', 'all_structs')
          freevars   ()
          cellvars   ()
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       'pathref_ascendants'
-         firstlineno 28
-         lnotab 0x020204012a0126012a0144fe2603
-      'main_structs'
+         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py'
+         name       'extract_struct_ftn'
+         firstlineno 23
+         lnotab 0x0205280202012601120106ff08023801
+      False
       code
-         argcount  : 1
-         nlocals   : 6
-         stacksize : 12
+         argcount  : 2
+         nlocals   : 33
+         stacksize : 15
          flags     : 3
          code
-            0x970067007d017c00a00000000000000000000000000000000000000000
-            00a6000000ab000000000000000000440090025d0a5c0200007d027d037c
-            01a001000000000000000000000000000000000000000064017c03640219
-            0000000000000000009b0064037c029b0064049d05a6010000ab01000000
-            000000000001007c01a00100000000000000000000000000000000000000
-            0064057c036406190000000000000000009b0064077c0364081900000000
-            00000000009b0064097c03640a19000000000000000000640b1900000000
-            00000000009b00640c7c03640a19000000000000000000640d1900000000
-            00000000009b009d08a6010000ab01000000000000000001007c01a00100
-            00000000000000000000000000000000000000640e7c03640f1900000000
-            00000000009b0064107c036411190000000000000000009b0064129d05a6
-            010000ab01000000000000000001007c01a0010000000000000000000000
-            00000000000000000064137c036414190000000000000000009b009d02a6
-            010000ab01000000000000000001007c0364151900000000000000000072
-            4d64166416a00200000000000000000000000000000000000000007c0364
-            1519000000000000000000a6010000ab0100000000000000007a0000007d
-            047c01a00100000000000000000000000000000000000000006417740700
-            0000000000000000007c03641519000000000000000000a6010000ab0100
-            000000000000009b0064187c049b009d04a6010000ab0100000000000000
-            0001006e157c01a001000000000000000000000000000000000000000064
-            19a6010000ab01000000000000000001007c03641a190000000000000000
-            00724d641b641ba00200000000000000000000000000000000000000007c
-            03641a19000000000000000000a6010000ab0100000000000000007a0000
-            007d047c01a0010000000000000000000000000000000000000000641c74
-            07000000000000000000007c03641a19000000000000000000a6010000ab
-            0100000000000000009b00641d7c049b009d04a6010000ab010000000000
-            00000001006e157c01a00100000000000000000000000000000000000000
-            00641ea6010000ab01000000000000000001007c03641f19000000000000
-            0000007266642084007c03641f19000000000000000000a0000000000000
-            000000000000000000000000000000a6000000ab00000000000000000044
-            00a6000000ab0000000000000000007d0564166416a00200000000000000
-            000000000000000000000000007c05a6010000ab0100000000000000007a
-            0000007d047c01a001000000000000000000000000000000000000000064
-            177407000000000000000000007c05a6010000ab0100000000000000009b
-            0064187c049b009d04a6010000ab010000000000000000010090018cf57c
-            01a00100000000000000000000000000000000000000006421a6010000ab
-            010000000000000000010090028c0c6401a0020000000000000000000000
-            0000000000000000007c01a6010000ab0100000000000000005300
+            0x970067007d0267007d0367007d0467007d0567007d0664017d07740100
+            0000000000000000007c006a0100000000000000007c006a020000000000
+            000000a6020000ab020000000000000000440090045d275c0200007d085c
+            0200007d097d0a7c0764027a0d00007d077c08a003000000000000000000
+            00000000000000000000006403a6010000ab0100000000000000007d0874
+            0900000000000000000000740a00000000000000000000740c0000000000
+            00000000007a0000006404ac05a6020000ab02000000000000000044005d
+            857d0b7c08a00700000000000000000000000000000000000000007c0b64
+            037a000000a6010000ab01000000000000000073067c087c0b6b02000000
+            0072657c05a00800000000000000000000000000000000000000007c08a6
+            010000ab01000000000000000001007413000000000000000000007c087c
+            09a6020000ab0200000000000000007d0c7c04a008000000000000000000
+            00000000000000000000007c0ca6010000ab01000000000000000001007c
+            02a008000000000000000000000000000000000000000074150000000000
+            00000000007c0b7c047c0c7c087c097c077c01ac06a6070000ab07000000
+            0000000000a6010000ab010000000000000000010001006e018c8664077c
+            0876009001725c7c08a00b00000000000000000000000000000000000000
+            0064086409a6020000ab020000000000000000a00b000000000000000000
+            000000000000000000000064076409a6020000ab020000000000000000a0
+            0c0000000000000000000000000000000000000000a6000000ab00000000
+            00000000007d0d640a7c0d760072477c0da00d0000000000000000000000
+            000000000000000000640aa6010000ab0100000000000000005c0200007d
+            0e7d0f7c0fa00c0000000000000000000000000000000000000000a60000
+            00ab0000000000000000007d107c0ea00d00000000000000000000000000
+            00000000000000a6000000ab000000000000000000640b19000000000000
+            0000007d116e047c0d7d107c107d11640ca00e0000000000000000000000
+            0000000000000000007c04640d640b850219000000000000000000a60100
+            00ab010000000000000000640c7a0000007c107a0000007d12640ca00e00
+            000000000000000000000000000000000000007c04a6010000ab01000000
+            0000000000640c7a0000007c117a0000007d137c04a00800000000000000
+            000000000000000000000000007c11a6010000ab01000000000000000001
+            007c02640b190000000000000000007d14741f000000000000000000006a
+            100000000000000000640e7c139b00640f7c129b0064107c146a11000000
+            00000000009b009d06a6010000ab01000000000000000001007415000000
+            0000000000000064077c047c137c087c097c077c017c126701ac11a60800
+            00ab0800000000000000007d157c03a00800000000000000000000000000
+            000000000000007425000000000000000000007c157c097c077c087c01ac
+            12a6050000ab050000000000000000a6010000ab01000000000000000001
+            007c04a0130000000000000000000000000000000000000000640ba60100
+            00ab01000000000000000001007c08a00700000000000000000000000000
+            000000000000006413a6010000ab01000000000000000072787c08a01400
+            000000000000000000000000000000000000006414a6010000ab01000000
+            00000000007d167c08a01400000000000000000000000000000000000000
+            006415a6010000ab0100000000000000007d177c087c1664027a0000007c
+            17850219000000000000000000a00c000000000000000000000000000000
+            0000000000a6000000ab0000000000000000007d187c187c02640b190000
+            000000000000006a150000000000000000760172207c02640b1900000000
+            00000000006a150000000000000000a00800000000000000000000000000
+            000000000000007c18a6010000ab01000000000000000001007c08a00700
+            000000000000000000000000000000000000006416a6010000ab01000000
+            0000000000728564177c08760072817c08a0140000000000000000000000
+            0000000000000000006417a6010000ab0100000000000000007d1664187d
+            1964097d187c087c16640d85021900000000000000000044005d1a7d1a7c
+            1a64146b0200000000720364047d198c0b7c1a64156b0200000000720201
+            006e087c1972057c187c1a7a0d00007d188c1b7c18a00c00000000000000
+            00000000000000000000000000a6000000ab0000000000000000007d187c
+            187c02640b190000000000000000006a150000000000000000760172207c
+            02640b190000000000000000006a150000000000000000a0080000000000
+            0000000000000000000000000000007c18a6010000ab0100000000000000
+            0001007c08a00700000000000000000000000000000000000000006419a6
+            010000ab01000000000000000073187c08a00c0000000000000000000000
+            000000000000000000a6000000ab000000000000000000641a6b02000000
+            0072ab7c06a00800000000000000000000000000000000000000007c08a6
+            010000ab010000000000000000010009007c02640b190000000000000000
+            007d146e392300742c000000000000000000002400722c0100641b7c099b
+            00641c7c089b009d047d1b741f000000000000000000006a170000000000
+            0000007c1ba6010000ab0100000000000000000100743100000000000000
+            0000007c1ba6010000ab010000000000000000820177007803590077017c
+            03a008000000000000000000000000000000000000000074250000000000
+            00000000007c147c0a7c077c087c01ac12a6050000ab0500000000000000
+            00a6010000ab01000000000000000001007c04a013000000000000000000
+            0000000000000000000000640ba6010000ab01000000000000000001007c
+            02a0130000000000000000000000000000000000000000640ba6010000ab
+            010000000000000000010090048c2790048c297c0344005d8c7d1c7c1c6a
+            190000000000000000a00d00000000000000000000000000000000000000
+            00641da6010000ab010000000000000000640119000000000000000000a0
+            0c0000000000000000000000000000000000000000a6000000ab00000000
+            00000000007d1d7c1d7c1c6a1a00000000000000007601724f640ca00e00
+            000000000000000000000000000000000000007c04a6010000ab01000000
+            00000000007d1e741f000000000000000000006a1b000000000000000064
+            1e7c1e9b00641f7c1d9b0064207c1c6a1c00000000000000009b0064217c
+            1c6a1d00000000000000009b0064227c1c6a1900000000000000009b0064
+            237c1c6a1a00000000000000009b009d0ca6010000ab0100000000000000
+            0001008c8d743d000000000000000000007c05a6010000ab010000000000
+            000000743d000000000000000000007c06a6010000ab0100000000000000
+            006b030000000072457401000000000000000000007c057c06a6020000ab
+            02000000000000000044005d1e5c0200007d1f7d20741f00000000000000
+            0000006a1000000000000000007c1f9b0064247c209b009d03a6010000ab
+            01000000000000000001008c1f741f000000000000000000006a1f000000
+            00000000006425a6010000ab010000000000000000010069005300744100
+            0000000000000000007c03740a00000000000000000000640767017a0000
+            00ac26a6020000ab0200000000000000005300
           38           0 RESUME                   0
          
-          39           2 BUILD_LIST               0
-                       4 STORE_FAST               1 (out)
+          40           2 BUILD_LIST               0
+                       4 STORE_FAST               2 (buffer_pile)
          
-          40           6 LOAD_FAST                0 (main_structs)
-                       8 LOAD_METHOD              0 (items)
-                      30 PRECALL                  0
-                      34 CALL                     0
-                      44 GET_ITER
-                 >>   46 EXTENDED_ARG             2
-                      48 FOR_ITER               522 (to 1094)
-                      50 UNPACK_SEQUENCE          2
-                      54 STORE_FAST               2 (part)
-                      56 STORE_FAST               3 (data)
-         
-          41          58 LOAD_FAST                1 (out)
-                      60 LOAD_METHOD              1 (append)
-                      82 LOAD_CONST               1 ('\n')
-                      84 LOAD_FAST                3 (data)
-                      86 LOAD_CONST               2 ('type')
-                      88 BINARY_SUBSCR
-                      98 FORMAT_VALUE             0
-                     100 LOAD_CONST               3 (' ')
-                     102 LOAD_FAST                2 (part)
-                     104 FORMAT_VALUE             0
-                     106 LOAD_CONST               4 (' :')
-                     108 BUILD_STRING             5
-                     110 PRECALL                  1
-                     114 CALL                     1
-                     124 POP_TOP
-         
-          42         126 LOAD_FAST                1 (out)
-                     128 LOAD_METHOD              1 (append)
-         
-          43         150 LOAD_CONST               5 ('    At path ')
-                     152 LOAD_FAST                3 (data)
-                     154 LOAD_CONST               6 ('path')
-                     156 BINARY_SUBSCR
-                     166 FORMAT_VALUE             0
-                     168 LOAD_CONST               7 (', name ')
-                     170 LOAD_FAST                3 (data)
-                     172 LOAD_CONST               8 ('name')
-                     174 BINARY_SUBSCR
-                     184 FORMAT_VALUE             0
-                     186 LOAD_CONST               9 (', lines ')
-                     188 LOAD_FAST                3 (data)
-                     190 LOAD_CONST              10 ('lines')
-                     192 BINARY_SUBSCR
-                     202 LOAD_CONST              11 (0)
-                     204 BINARY_SUBSCR
-                     214 FORMAT_VALUE             0
-                     216 LOAD_CONST              12 (' -> ')
-                     218 LOAD_FAST                3 (data)
-                     220 LOAD_CONST              10 ('lines')
-                     222 BINARY_SUBSCR
-                     232 LOAD_CONST              13 (-1)
-                     234 BINARY_SUBSCR
-                     244 FORMAT_VALUE             0
-                     246 BUILD_STRING             8
-         
-          42         248 PRECALL                  1
-                     252 CALL                     1
-                     262 POP_TOP
-         
-          45         264 LOAD_FAST                1 (out)
-                     266 LOAD_METHOD              1 (append)
-                     288 LOAD_CONST              14 ('    ')
-                     290 LOAD_FAST                3 (data)
-                     292 LOAD_CONST              15 ('ssize')
-                     294 BINARY_SUBSCR
-                     304 FORMAT_VALUE             0
-                     306 LOAD_CONST              16 (' statements over ')
-                     308 LOAD_FAST                3 (data)
-                     310 LOAD_CONST              17 ('NLOC')
-                     312 BINARY_SUBSCR
-                     322 FORMAT_VALUE             0
-                     324 LOAD_CONST              18 (' lines')
-                     326 BUILD_STRING             5
-                     328 PRECALL                  1
-                     332 CALL                     1
-                     342 POP_TOP
-         
-          46         344 LOAD_FAST                1 (out)
-                     346 LOAD_METHOD              1 (append)
-                     368 LOAD_CONST              19 ('    Complexity ')
-                     370 LOAD_FAST                3 (data)
-                     372 LOAD_CONST              20 ('CCN')
-                     374 BINARY_SUBSCR
-                     384 FORMAT_VALUE             0
-                     386 BUILD_STRING             2
-                     388 PRECALL                  1
-                     392 CALL                     1
-                     402 POP_TOP
-         
-          47         404 LOAD_FAST                3 (data)
-                     406 LOAD_CONST              21 ('callables')
-                     408 BINARY_SUBSCR
-                     418 POP_JUMP_FORWARD_IF_FALSE    77 (to 574)
-         
-          48         420 LOAD_CONST              22 ('\n       - ')
-                     422 LOAD_CONST              22 ('\n       - ')
-                     424 LOAD_METHOD              2 (join)
-                     446 LOAD_FAST                3 (data)
-                     448 LOAD_CONST              21 ('callables')
-                     450 BINARY_SUBSCR
-                     460 PRECALL                  1
-                     464 CALL                     1
-                     474 BINARY_OP                0 (+)
-                     478 STORE_FAST               4 (list_str)
-         
-          50         480 LOAD_FAST                1 (out)
-                     482 LOAD_METHOD              1 (append)
-                     504 LOAD_CONST              23 ('    Refers to ')
-                     506 LOAD_GLOBAL              7 (NULL + len)
-                     518 LOAD_FAST                3 (data)
-                     520 LOAD_CONST              21 ('callables')
-                     522 BINARY_SUBSCR
-                     532 PRECALL                  1
-                     536 CALL                     1
-                     546 FORMAT_VALUE             0
-                     548 LOAD_CONST              24 (' callables:')
-                     550 LOAD_FAST                4 (list_str)
-                     552 FORMAT_VALUE             0
-                     554 BUILD_STRING             4
-                     556 PRECALL                  1
-                     560 CALL                     1
-                     570 POP_TOP
-                     572 JUMP_FORWARD            21 (to 616)
-         
-          52     >>  574 LOAD_FAST                1 (out)
-                     576 LOAD_METHOD              1 (append)
-                     598 LOAD_CONST              25 ('    Contains no callables')
-                     600 PRECALL                  1
-                     604 CALL                     1
-                     614 POP_TOP
-         
-          53     >>  616 LOAD_FAST                3 (data)
-                     618 LOAD_CONST              26 ('contains')
-                     620 BINARY_SUBSCR
-                     630 POP_JUMP_FORWARD_IF_FALSE    77 (to 786)
-         
-          54         632 LOAD_CONST              27 ('\n    - ')
-                     634 LOAD_CONST              27 ('\n    - ')
-                     636 LOAD_METHOD              2 (join)
-                     658 LOAD_FAST                3 (data)
-                     660 LOAD_CONST              26 ('contains')
-                     662 BINARY_SUBSCR
-                     672 PRECALL                  1
-                     676 CALL                     1
-                     686 BINARY_OP                0 (+)
-                     690 STORE_FAST               4 (list_str)
-         
-          55         692 LOAD_FAST                1 (out)
-                     694 LOAD_METHOD              1 (append)
-                     716 LOAD_CONST              28 ('    Contains ')
-                     718 LOAD_GLOBAL              7 (NULL + len)
-                     730 LOAD_FAST                3 (data)
-                     732 LOAD_CONST              26 ('contains')
-                     734 BINARY_SUBSCR
-                     744 PRECALL                  1
-                     748 CALL                     1
-                     758 FORMAT_VALUE             0
-                     760 LOAD_CONST              29 (' elements:')
-                     762 LOAD_FAST                4 (list_str)
-                     764 FORMAT_VALUE             0
-                     766 BUILD_STRING             4
-                     768 PRECALL                  1
-                     772 CALL                     1
-                     782 POP_TOP
-                     784 JUMP_FORWARD            21 (to 828)
-         
-          57     >>  786 LOAD_FAST                1 (out)
-                     788 LOAD_METHOD              1 (append)
-                     810 LOAD_CONST              30 ('    Contains no inner structures')
-                     812 PRECALL                  1
-                     816 CALL                     1
-                     826 POP_TOP
-         
-          59     >>  828 LOAD_FAST                3 (data)
-                     830 LOAD_CONST              31 ('annotations')
-                     832 BINARY_SUBSCR
-                     842 POP_JUMP_FORWARD_IF_FALSE   102 (to 1048)
-         
-          60         844 LOAD_CONST              32 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 60>)
-                     846 MAKE_FUNCTION            0
-                     848 LOAD_FAST                3 (data)
-                     850 LOAD_CONST              31 ('annotations')
-                     852 BINARY_SUBSCR
-                     862 LOAD_METHOD              0 (items)
-                     884 PRECALL                  0
-                     888 CALL                     0
-                     898 GET_ITER
-                     900 PRECALL                  0
-                     904 CALL                     0
-                     914 STORE_FAST               5 (keyvals)
-         
-          61         916 LOAD_CONST              22 ('\n       - ')
-                     918 LOAD_CONST              22 ('\n       - ')
-                     920 LOAD_METHOD              2 (join)
-                     942 LOAD_FAST                5 (keyvals)
-                     944 PRECALL                  1
-                     948 CALL                     1
-                     958 BINARY_OP                0 (+)
-                     962 STORE_FAST               4 (list_str)
-         
-          63         964 LOAD_FAST                1 (out)
-                     966 LOAD_METHOD              1 (append)
-                     988 LOAD_CONST              23 ('    Refers to ')
-                     990 LOAD_GLOBAL              7 (NULL + len)
-                    1002 LOAD_FAST                5 (keyvals)
-                    1004 PRECALL                  1
-                    1008 CALL                     1
-                    1018 FORMAT_VALUE             0
-                    1020 LOAD_CONST              24 (' callables:')
-                    1022 LOAD_FAST                4 (list_str)
-                    1024 FORMAT_VALUE             0
-                    1026 BUILD_STRING             4
-                    1028 PRECALL                  1
-                    1032 CALL                     1
-                    1042 POP_TOP
-                    1044 EXTENDED_ARG             1
-                    1046 JUMP_BACKWARD          501 (to 46)
-         
-          65     >> 1048 LOAD_FAST                1 (out)
-                    1050 LOAD_METHOD              1 (append)
-                    1072 LOAD_CONST              33 ('    Contains no annotations')
-                    1074 PRECALL                  1
-                    1078 CALL                     1
-                    1088 POP_TOP
-                    1090 EXTENDED_ARG             2
-                    1092 JUMP_BACKWARD          524 (to 46)
-         
-          68     >> 1094 LOAD_CONST               1 ('\n')
-                    1096 LOAD_METHOD              2 (join)
-                    1118 LOAD_FAST                1 (out)
-                    1120 PRECALL                  1
-                    1124 CALL                     1
-                    1134 RETURN_VALUE
-         consts
-            None
-            '\n'
-            'type'
-            ' '
-            ' :'
-            '    At path '
-            'path'
-            ', name '
-            'name'
-            ', lines '
-            'lines'
-            0
-            ' -> '
-            -1
-            '    '
-            'ssize'
-            ' statements over '
-            'NLOC'
-            ' lines'
-            '    Complexity '
-            'CCN'
-            'callables'
-            '\n       - '
-            '    Refers to '
-            ' callables:'
-            '    Contains no callables'
-            'contains'
-            '\n    - '
-            '    Contains '
-            ' elements:'
-            '    Contains no inner structures'
-            'annotations'
-            code
-               argcount  : 1
-               nlocals   : 3
-               stacksize : 4
-               flags     : 19
-               code
-                  0x970067007c005d125c0200007d017d0274000000000000000000000064
-                  007a0000007c027a00000091028c135300
-                60           0 RESUME                   0
-                             2 BUILD_LIST               0
-                             4 LOAD_FAST                0 (.0)
-                       >>    6 FOR_ITER                18 (to 44)
-                             8 UNPACK_SEQUENCE          2
-                            12 STORE_FAST               1 (key)
-                            14 STORE_FAST               2 (values)
-                            16 LOAD_GLOBAL              0 (keys)
-                            28 LOAD_CONST               0 (':')
-                            30 BINARY_OP                0 (+)
-                            34 LOAD_FAST                2 (values)
-                            36 BINARY_OP                0 (+)
-                            40 LIST_APPEND              2
-                            42 JUMP_BACKWARD           19 (to 6)
-                       >>   44 RETURN_VALUE
-               consts
-                  ':'
-               names      ('keys',)
-               varnames   ('.0', 'key', 'values')
-               freevars   ()
-               cellvars   ()
-               filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-               name       '<listcomp>'
-               firstlineno 60
-               lnotab 0x
-            '    Contains no annotations'
-         names      ('items', 'append', 'join', 'len')
-         varnames   ('main_structs', 'out', 'part', 'data', 'list_str', 'keyvals')
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       'struct_summary_str'
-         firstlineno 38
-         lnotab
-            0x0201040134014401180162ff100350013c0110013c025e022a0110013c
-            015e022a0210014801300254022e03
-      'line'
-      code
-         argcount  : 1
-         nlocals   : 8
-         stacksize : 6
-         flags     : 3
-         code
-            0x97007c00a00000000000000000000000000000000000000000006401a6
-            010000ab01000000000000000064026b040000000073197c00a000000000
-            00000000000000000000000000000000006401a6010000ab010000000000
-            00000064036b0200000000720264047d0064057d01740300000000000000
-            0000006a0200000000000000007c017c00a6020000ab0200000000000000
-            007d0267007d0364067d047c0244005d5d7d0564047d0674070000000000
-            00000000007409000000000000000000007c05a6010000ab010000000000
-            00000064036407a6030000ab03000000000000000044005d1f7d077c057c
-            0764087a0a0000190000000000000000007c047600720201006e0f7c057c
-            0764087a0a0000190000000000000000007c067a0000007d068c207c0664
-            046b030000000072157c03a0050000000000000000000000000000000000
-            0000007c06a6010000ab01000000000000000001008c5e7c035300
-          71           0 RESUME                   0
-         
-          76           2 LOAD_FAST                0 (line)
-                       4 LOAD_METHOD              0 (count)
-                      26 LOAD_CONST               1 ('(')
-                      28 PRECALL                  1
-                      32 CALL                     1
-                      42 LOAD_CONST               2 (50)
-                      44 COMPARE_OP               4 (>)
-                      50 POP_JUMP_FORWARD_IF_TRUE    25 (to 102)
-                      52 LOAD_FAST                0 (line)
-                      54 LOAD_METHOD              0 (count)
-                      76 LOAD_CONST               1 ('(')
-                      78 PRECALL                  1
-                      82 CALL                     1
-                      92 LOAD_CONST               3 (0)
-                      94 COMPARE_OP               2 (==)
-                     100 POP_JUMP_FORWARD_IF_FALSE     2 (to 106)
-         
-          77     >>  102 LOAD_CONST               4 ('')
-                     104 STORE_FAST               0 (line)
-         
-          80     >>  106 LOAD_CONST               5 ('(.*?\\S)\\(')
-                     108 STORE_FAST               1 (pattern)
-         
-          82         110 LOAD_GLOBAL              3 (NULL + re)
-                     122 LOAD_ATTR                2 (findall)
-                     132 LOAD_FAST                1 (pattern)
-                     134 LOAD_FAST                0 (line)
-                     136 PRECALL                  2
-                     140 CALL                     2
-                     150 STORE_FAST               2 (matches)
-         
-          83         152 BUILD_LIST               0
-                     154 STORE_FAST               3 (clean_matches)
-         
-          85         156 LOAD_CONST               6 (',+-/*<>=;|(){}[]:~ ')
-                     158 STORE_FAST               4 (tokens)
-         
-          86         160 LOAD_FAST                2 (matches)
-                     162 GET_ITER
-                 >>  164 FOR_ITER                93 (to 352)
-                     166 STORE_FAST               5 (match_)
-         
-          87         168 LOAD_CONST               4 ('')
-                     170 STORE_FAST               6 (token)
-         
-          88         172 LOAD_GLOBAL              7 (NULL + range)
-                     184 LOAD_GLOBAL              9 (NULL + len)
-                     196 LOAD_FAST                5 (match_)
-                     198 PRECALL                  1
-                     202 CALL                     1
-                     212 LOAD_CONST               3 (0)
-                     214 LOAD_CONST               7 (-1)
-                     216 PRECALL                  3
-                     220 CALL                     3
-                     230 GET_ITER
-                 >>  232 FOR_ITER                31 (to 296)
-                     234 STORE_FAST               7 (i)
-         
-          89         236 LOAD_FAST                5 (match_)
-                     238 LOAD_FAST                7 (i)
-                     240 LOAD_CONST               8 (1)
-                     242 BINARY_OP               10 (-)
-                     246 BINARY_SUBSCR
-                     256 LOAD_FAST                4 (tokens)
-                     258 CONTAINS_OP              0
-                     260 POP_JUMP_FORWARD_IF_FALSE     2 (to 266)
-         
-          90         262 POP_TOP
-                     264 JUMP_FORWARD            15 (to 296)
-         
-          91     >>  266 LOAD_FAST                5 (match_)
-                     268 LOAD_FAST                7 (i)
-                     270 LOAD_CONST               8 (1)
-                     272 BINARY_OP               10 (-)
-                     276 BINARY_SUBSCR
-                     286 LOAD_FAST                6 (token)
-                     288 BINARY_OP                0 (+)
-                     292 STORE_FAST               6 (token)
-                     294 JUMP_BACKWARD           32 (to 232)
-         
-          93     >>  296 LOAD_FAST                6 (token)
-                     298 LOAD_CONST               4 ('')
-                     300 COMPARE_OP               3 (!=)
-                     306 POP_JUMP_FORWARD_IF_FALSE    21 (to 350)
-         
-          94         308 LOAD_FAST                3 (clean_matches)
-                     310 LOAD_METHOD              5 (append)
-                     332 LOAD_FAST                6 (token)
-                     334 PRECALL                  1
-                     338 CALL                     1
-                     348 POP_TOP
-                 >>  350 JUMP_BACKWARD           94 (to 164)
+          41           6 BUILD_LIST               0
+                       8 STORE_FAST               3 (stack)
          
-          95     >>  352 LOAD_FAST                3 (clean_matches)
-                     354 RETURN_VALUE
+          42          10 BUILD_LIST               0
+                      12 STORE_FAST               4 (path)
+         
+          44          14 BUILD_LIST               0
+                      16 STORE_FAST               5 (entry_)
+         
+          45          18 BUILD_LIST               0
+                      20 STORE_FAST               6 (out_)
+         
+          46          22 LOAD_CONST               1 (0)
+                      24 STORE_FAST               7 (stat_idx)
+         
+          47          26 LOAD_GLOBAL              1 (NULL + zip)
+                      38 LOAD_FAST                0 (stmts)
+                      40 LOAD_ATTR                1 (stmt)
+                      50 LOAD_FAST                0 (stmts)
+                      52 LOAD_ATTR                2 (lines)
+                      62 PRECALL                  2
+                      66 CALL                     2
+                      76 GET_ITER
+                 >>   78 EXTENDED_ARG             4
+                      80 FOR_ITER              1063 (to 2208)
+                      82 UNPACK_SEQUENCE          2
+                      86 STORE_FAST               8 (line)
+                      88 UNPACK_SEQUENCE          2
+                      92 STORE_FAST               9 (line_idx1)
+                      94 STORE_FAST              10 (line_idx2)
+         
+          48          96 LOAD_FAST                7 (stat_idx)
+                      98 LOAD_CONST               2 (1)
+                     100 BINARY_OP               13 (+=)
+                     104 STORE_FAST               7 (stat_idx)
+         
+          50         106 LOAD_FAST                8 (line)
+                     108 LOAD_METHOD              3 (lstrip)
+                     130 LOAD_CONST               3 (' ')
+                     132 PRECALL                  1
+                     136 CALL                     1
+                     146 STORE_FAST               8 (line)
+         
+          55         148 LOAD_GLOBAL              9 (NULL + sorted)
+                     160 LOAD_GLOBAL             10 (PARTS)
+                     172 LOAD_GLOBAL             12 (NESTS)
+                     184 BINARY_OP                0 (+)
+                     188 LOAD_CONST               4 (True)
+                     190 KW_NAMES                 5
+                     192 PRECALL                  2
+                     196 CALL                     2
+                     206 GET_ITER
+                 >>  208 FOR_ITER               133 (to 476)
+                     210 STORE_FAST              11 (part)
+         
+          56         212 LOAD_FAST                8 (line)
+                     214 LOAD_METHOD              7 (startswith)
+                     236 LOAD_FAST               11 (part)
+                     238 LOAD_CONST               3 (' ')
+                     240 BINARY_OP                0 (+)
+                     244 PRECALL                  1
+                     248 CALL                     1
+                     258 POP_JUMP_FORWARD_IF_TRUE     6 (to 272)
+                     260 LOAD_FAST                8 (line)
+                     262 LOAD_FAST               11 (part)
+                     264 COMPARE_OP               2 (==)
+                     270 POP_JUMP_FORWARD_IF_FALSE   101 (to 474)
+         
+          58     >>  272 LOAD_FAST                5 (entry_)
+                     274 LOAD_METHOD              8 (append)
+                     296 LOAD_FAST                8 (line)
+                     298 PRECALL                  1
+                     302 CALL                     1
+                     312 POP_TOP
+         
+          59         314 LOAD_GLOBAL             19 (NULL + _parse_name_ftn)
+                     326 LOAD_FAST                8 (line)
+                     328 LOAD_FAST                9 (line_idx1)
+                     330 PRECALL                  2
+                     334 CALL                     2
+                     344 STORE_FAST              12 (name)
+         
+          60         346 LOAD_FAST                4 (path)
+                     348 LOAD_METHOD              8 (append)
+                     370 LOAD_FAST               12 (name)
+                     372 PRECALL                  1
+                     376 CALL                     1
+                     386 POP_TOP
+         
+          61         388 LOAD_FAST                2 (buffer_pile)
+                     390 LOAD_METHOD              8 (append)
+         
+          62         412 LOAD_GLOBAL             21 (NULL + new_buffer_item)
+         
+          63         424 LOAD_FAST               11 (part)
+         
+          64         426 LOAD_FAST                4 (path)
+         
+          65         428 LOAD_FAST               12 (name)
+         
+          66         430 LOAD_FAST                8 (line)
+         
+          67         432 LOAD_FAST                9 (line_idx1)
+         
+          68         434 LOAD_FAST                7 (stat_idx)
+         
+          69         436 LOAD_FAST                1 (verbose)
+         
+          62         438 KW_NAMES                 6
+                     440 PRECALL                  7
+                     444 CALL                     7
+         
+          61         454 PRECALL                  1
+                     458 CALL                     1
+                     468 POP_TOP
+         
+          72         470 POP_TOP
+                     472 JUMP_FORWARD             1 (to 476)
+         
+          56     >>  474 JUMP_BACKWARD          134 (to 208)
+         
+          74     >>  476 LOAD_CONST               7 ('procedure')
+                     478 LOAD_FAST                8 (line)
+                     480 CONTAINS_OP              0
+                     482 EXTENDED_ARG             1
+                     484 POP_JUMP_FORWARD_IF_FALSE   348 (to 1182)
+         
+          75         486 LOAD_FAST                8 (line)
+                     488 LOAD_METHOD             11 (replace)
+                     510 LOAD_CONST               8 ('::')
+                     512 LOAD_CONST               9 ('')
+                     514 PRECALL                  2
+                     518 CALL                     2
+                     528 LOAD_METHOD             11 (replace)
+                     550 LOAD_CONST               7 ('procedure')
+                     552 LOAD_CONST               9 ('')
+                     554 PRECALL                  2
+                     558 CALL                     2
+                     568 LOAD_METHOD             12 (strip)
+                     590 PRECALL                  0
+                     594 CALL                     0
+                     604 STORE_FAST              13 (line_clean)
+         
+          76         606 LOAD_CONST              10 ('=>')
+                     608 LOAD_FAST               13 (line_clean)
+                     610 CONTAINS_OP              0
+                     612 POP_JUMP_FORWARD_IF_FALSE    71 (to 756)
+         
+          77         614 LOAD_FAST               13 (line_clean)
+                     616 LOAD_METHOD             13 (split)
+                     638 LOAD_CONST              10 ('=>')
+                     640 PRECALL                  1
+                     644 CALL                     1
+                     654 UNPACK_SEQUENCE          2
+                     658 STORE_FAST              14 (front)
+                     660 STORE_FAST              15 (tail)
+         
+          78         662 LOAD_FAST               15 (tail)
+                     664 LOAD_METHOD             12 (strip)
+                     686 PRECALL                  0
+                     690 CALL                     0
+                     700 STORE_FAST              16 (target)
+         
+          79         702 LOAD_FAST               14 (front)
+                     704 LOAD_METHOD             13 (split)
+                     726 PRECALL                  0
+                     730 CALL                     0
+                     740 LOAD_CONST              11 (-1)
+                     742 BINARY_SUBSCR
+                     752 STORE_FAST              17 (proxy)
+                     754 JUMP_FORWARD             4 (to 764)
+         
+          81     >>  756 LOAD_FAST               13 (line_clean)
+                     758 STORE_FAST              16 (target)
+         
+          82         760 LOAD_FAST               16 (target)
+                     762 STORE_FAST              17 (proxy)
+         
+          84     >>  764 LOAD_CONST              12 ('.')
+                     766 LOAD_METHOD             14 (join)
+                     788 LOAD_FAST                4 (path)
+                     790 LOAD_CONST              13 (None)
+                     792 LOAD_CONST              11 (-1)
+                     794 BUILD_SLICE              2
+                     796 BINARY_SUBSCR
+                     806 PRECALL                  1
+                     810 CALL                     1
+                     820 LOAD_CONST              12 ('.')
+                     822 BINARY_OP                0 (+)
+                     826 LOAD_FAST               16 (target)
+                     828 BINARY_OP                0 (+)
+                     832 STORE_FAST              18 (target_name)
+         
+          85         834 LOAD_CONST              12 ('.')
+                     836 LOAD_METHOD             14 (join)
+                     858 LOAD_FAST                4 (path)
+                     860 PRECALL                  1
+                     864 CALL                     1
+                     874 LOAD_CONST              12 ('.')
+                     876 BINARY_OP                0 (+)
+                     880 LOAD_FAST               17 (proxy)
+                     882 BINARY_OP                0 (+)
+                     886 STORE_FAST              19 (proxy_name)
+         
+          86         888 LOAD_FAST                4 (path)
+                     890 LOAD_METHOD              8 (append)
+                     912 LOAD_FAST               17 (proxy)
+                     914 PRECALL                  1
+                     918 CALL                     1
+                     928 POP_TOP
+         
+          87         930 LOAD_FAST                2 (buffer_pile)
+                     932 LOAD_CONST              11 (-1)
+                     934 BINARY_SUBSCR
+                     944 STORE_FAST              20 (last_buff)
+         
+          89         946 LOAD_GLOBAL             31 (NULL + logger)
+                     958 LOAD_ATTR               16 (warning)
+                     968 LOAD_CONST              14 ('Adding proxy ')
+                     970 LOAD_FAST               19 (proxy_name)
+                     972 FORMAT_VALUE             0
+                     974 LOAD_CONST              15 (' (pointer to ')
+                     976 LOAD_FAST               18 (target_name)
+                     978 FORMAT_VALUE             0
+                     980 LOAD_CONST              16 (') to ')
+                     982 LOAD_FAST               20 (last_buff)
+                     984 LOAD_ATTR               17 (name)
+                     994 FORMAT_VALUE             0
+                     996 BUILD_STRING             6
+                     998 PRECALL                  1
+                    1002 CALL                     1
+                    1012 POP_TOP
+         
+          91        1014 LOAD_GLOBAL             21 (NULL + new_buffer_item)
+         
+          92        1026 LOAD_CONST               7 ('procedure')
+         
+          93        1028 LOAD_FAST                4 (path)
+         
+          94        1030 LOAD_FAST               19 (proxy_name)
+         
+          95        1032 LOAD_FAST                8 (line)
+         
+          96        1034 LOAD_FAST                9 (line_idx1)
+         
+          97        1036 LOAD_FAST                7 (stat_idx)
+         
+          98        1038 LOAD_FAST                1 (verbose)
+         
+          99        1040 LOAD_FAST               18 (target_name)
+                    1042 BUILD_LIST               1
+         
+          91        1044 KW_NAMES                17
+                    1046 PRECALL                  8
+                    1050 CALL                     8
+                    1060 STORE_FAST              21 (buf_)
+         
+         101        1062 LOAD_FAST                3 (stack)
+                    1064 LOAD_METHOD              8 (append)
+         
+         102        1086 LOAD_GLOBAL             37 (NULL + new_stack_item)
+         
+         103        1098 LOAD_FAST               21 (buf_)
+         
+         104        1100 LOAD_FAST                9 (line_idx1)
+         
+         105        1102 LOAD_FAST                7 (stat_idx)
+         
+         106        1104 LOAD_FAST                8 (line)
+         
+         107        1106 LOAD_FAST                1 (verbose)
+         
+         102        1108 KW_NAMES                18
+                    1110 PRECALL                  5
+                    1114 CALL                     5
+         
+         101        1124 PRECALL                  1
+                    1128 CALL                     1
+                    1138 POP_TOP
+         
+         109        1140 LOAD_FAST                4 (path)
+                    1142 LOAD_METHOD             19 (pop)
+                    1164 LOAD_CONST              11 (-1)
+                    1166 PRECALL                  1
+                    1170 CALL                     1
+                    1180 POP_TOP
+         
+         111     >> 1182 LOAD_FAST                8 (line)
+                    1184 LOAD_METHOD              7 (startswith)
+                    1206 LOAD_CONST              19 ('_type')
+                    1208 PRECALL                  1
+                    1212 CALL                     1
+                    1222 POP_JUMP_FORWARD_IF_FALSE   120 (to 1464)
+         
+         112        1224 LOAD_FAST                8 (line)
+                    1226 LOAD_METHOD             20 (index)
+                    1248 LOAD_CONST              20 ('(')
+                    1250 PRECALL                  1
+                    1254 CALL                     1
+                    1264 STORE_FAST              22 (strt_)
+         
+         113        1266 LOAD_FAST                8 (line)
+                    1268 LOAD_METHOD             20 (index)
+                    1290 LOAD_CONST              21 (')')
+                    1292 PRECALL                  1
+                    1296 CALL                     1
+                    1306 STORE_FAST              23 (end_)
+         
+         114        1308 LOAD_FAST                8 (line)
+                    1310 LOAD_FAST               22 (strt_)
+                    1312 LOAD_CONST               2 (1)
+                    1314 BINARY_OP                0 (+)
+                    1318 LOAD_FAST               23 (end_)
+                    1320 BUILD_SLICE              2
+                    1322 BINARY_SUBSCR
+                    1332 LOAD_METHOD             12 (strip)
+                    1354 PRECALL                  0
+                    1358 CALL                     0
+                    1368 STORE_FAST              24 (parent)
+         
+         116        1370 LOAD_FAST               24 (parent)
+                    1372 LOAD_FAST                2 (buffer_pile)
+                    1374 LOAD_CONST              11 (-1)
+                    1376 BINARY_SUBSCR
+                    1386 LOAD_ATTR               21 (parents)
+                    1396 CONTAINS_OP              1
+                    1398 POP_JUMP_FORWARD_IF_FALSE    32 (to 1464)
+         
+         117        1400 LOAD_FAST                2 (buffer_pile)
+                    1402 LOAD_CONST              11 (-1)
+                    1404 BINARY_SUBSCR
+                    1414 LOAD_ATTR               21 (parents)
+                    1424 LOAD_METHOD              8 (append)
+                    1446 LOAD_FAST               24 (parent)
+                    1448 PRECALL                  1
+                    1452 CALL                     1
+                    1462 POP_TOP
+         
+         119     >> 1464 LOAD_FAST                8 (line)
+                    1466 LOAD_METHOD              7 (startswith)
+                    1488 LOAD_CONST              22 ('type')
+                    1490 PRECALL                  1
+                    1494 CALL                     1
+                    1504 POP_JUMP_FORWARD_IF_FALSE   133 (to 1772)
+                    1506 LOAD_CONST              23 ('extends')
+                    1508 LOAD_FAST                8 (line)
+                    1510 CONTAINS_OP              0
+                    1512 POP_JUMP_FORWARD_IF_FALSE   129 (to 1772)
+         
+         120        1514 LOAD_FAST                8 (line)
+                    1516 LOAD_METHOD             20 (index)
+                    1538 LOAD_CONST              23 ('extends')
+                    1540 PRECALL                  1
+                    1544 CALL                     1
+                    1554 STORE_FAST              22 (strt_)
+         
+         121        1556 LOAD_CONST              24 (False)
+                    1558 STORE_FAST              25 (read)
+         
+         122        1560 LOAD_CONST               9 ('')
+                    1562 STORE_FAST              24 (parent)
+         
+         123        1564 LOAD_FAST                8 (line)
+                    1566 LOAD_FAST               22 (strt_)
+                    1568 LOAD_CONST              13 (None)
+                    1570 BUILD_SLICE              2
+                    1572 BINARY_SUBSCR
+                    1582 GET_ITER
+                 >> 1584 FOR_ITER                26 (to 1638)
+                    1586 STORE_FAST              26 (char)
+         
+         124        1588 LOAD_FAST               26 (char)
+                    1590 LOAD_CONST              20 ('(')
+                    1592 COMPARE_OP               2 (==)
+                    1598 POP_JUMP_FORWARD_IF_FALSE     3 (to 1606)
+         
+         125        1600 LOAD_CONST               4 (True)
+                    1602 STORE_FAST              25 (read)
+                    1604 JUMP_BACKWARD           11 (to 1584)
+         
+         126     >> 1606 LOAD_FAST               26 (char)
+                    1608 LOAD_CONST              21 (')')
+                    1610 COMPARE_OP               2 (==)
+                    1616 POP_JUMP_FORWARD_IF_FALSE     2 (to 1622)
+         
+         127        1618 POP_TOP
+                    1620 JUMP_FORWARD             8 (to 1638)
+         
+         129     >> 1622 LOAD_FAST               25 (read)
+                    1624 POP_JUMP_FORWARD_IF_FALSE     5 (to 1636)
+         
+         130        1626 LOAD_FAST               24 (parent)
+                    1628 LOAD_FAST               26 (char)
+                    1630 BINARY_OP               13 (+=)
+                    1634 STORE_FAST              24 (parent)
+                 >> 1636 JUMP_BACKWARD           27 (to 1584)
+         
+         131     >> 1638 LOAD_FAST               24 (parent)
+                    1640 LOAD_METHOD             12 (strip)
+                    1662 PRECALL                  0
+                    1666 CALL                     0
+                    1676 STORE_FAST              24 (parent)
+         
+         133        1678 LOAD_FAST               24 (parent)
+                    1680 LOAD_FAST                2 (buffer_pile)
+                    1682 LOAD_CONST              11 (-1)
+                    1684 BINARY_SUBSCR
+                    1694 LOAD_ATTR               21 (parents)
+                    1704 CONTAINS_OP              1
+                    1706 POP_JUMP_FORWARD_IF_FALSE    32 (to 1772)
+         
+         134        1708 LOAD_FAST                2 (buffer_pile)
+                    1710 LOAD_CONST              11 (-1)
+                    1712 BINARY_SUBSCR
+                    1722 LOAD_ATTR               21 (parents)
+                    1732 LOAD_METHOD              8 (append)
+                    1754 LOAD_FAST               24 (parent)
+                    1756 PRECALL                  1
+                    1760 CALL                     1
+                    1770 POP_TOP
+         
+         136     >> 1772 LOAD_FAST                8 (line)
+                    1774 LOAD_METHOD              7 (startswith)
+                    1796 LOAD_CONST              25 ('end ')
+                    1798 PRECALL                  1
+                    1802 CALL                     1
+                    1812 POP_JUMP_FORWARD_IF_TRUE    24 (to 1862)
+                    1814 LOAD_FAST                8 (line)
+                    1816 LOAD_METHOD             12 (strip)
+                    1838 PRECALL                  0
+                    1842 CALL                     0
+                    1852 LOAD_CONST              26 ('end')
+                    1854 COMPARE_OP               2 (==)
+                    1860 POP_JUMP_FORWARD_IF_FALSE   171 (to 2204)
+         
+         137     >> 1862 LOAD_FAST                6 (out_)
+                    1864 LOAD_METHOD              8 (append)
+                    1886 LOAD_FAST                8 (line)
+                    1888 PRECALL                  1
+                    1892 CALL                     1
+                    1902 POP_TOP
+         
+         138        1904 NOP
+         
+         139        1906 LOAD_FAST                2 (buffer_pile)
+                    1908 LOAD_CONST              11 (-1)
+                    1910 BINARY_SUBSCR
+                    1920 STORE_FAST              20 (last_buff)
+                    1922 JUMP_FORWARD            57 (to 2038)
+                 >> 1924 PUSH_EXC_INFO
+         
+         140        1926 LOAD_GLOBAL             44 (IndexError)
+                    1938 CHECK_EXC_MATCH
+                    1940 POP_JUMP_FORWARD_IF_FALSE    44 (to 2030)
+                    1942 POP_TOP
+         
+         141        1944 LOAD_CONST              27 ('No buffer for line ')
+                    1946 LOAD_FAST                9 (line_idx1)
+                    1948 FORMAT_VALUE             0
+                    1950 LOAD_CONST              28 (':')
+                    1952 LOAD_FAST                8 (line)
+                    1954 FORMAT_VALUE             0
+                    1956 BUILD_STRING             4
+                    1958 STORE_FAST              27 (msg)
+         
+         142        1960 LOAD_GLOBAL             31 (NULL + logger)
+                    1972 LOAD_ATTR               23 (critical)
+                    1982 LOAD_FAST               27 (msg)
+                    1984 PRECALL                  1
+                    1988 CALL                     1
+                    1998 POP_TOP
+         
+         143        2000 LOAD_GLOBAL             49 (NULL + RuntimeError)
+                    2012 LOAD_FAST               27 (msg)
+                    2014 PRECALL                  1
+                    2018 CALL                     1
+                    2028 RAISE_VARARGS            1
+         
+         140     >> 2030 RERAISE                  0
+                 >> 2032 COPY                     3
+                    2034 POP_EXCEPT
+                    2036 RERAISE                  1
+         
+         145     >> 2038 LOAD_FAST                3 (stack)
+                    2040 LOAD_METHOD              8 (append)
+         
+         146        2062 LOAD_GLOBAL             37 (NULL + new_stack_item)
+         
+         147        2074 LOAD_FAST               20 (last_buff)
+         
+         148        2076 LOAD_FAST               10 (line_idx2)
+         
+         149        2078 LOAD_FAST                7 (stat_idx)
+         
+         150        2080 LOAD_FAST                8 (line)
+         
+         151        2082 LOAD_FAST                1 (verbose)
+         
+         146        2084 KW_NAMES                18
+                    2086 PRECALL                  5
+                    2090 CALL                     5
+         
+         145        2100 PRECALL                  1
+                    2104 CALL                     1
+                    2114 POP_TOP
+         
+         153        2116 LOAD_FAST                4 (path)
+                    2118 LOAD_METHOD             19 (pop)
+                    2140 LOAD_CONST              11 (-1)
+                    2142 PRECALL                  1
+                    2146 CALL                     1
+                    2156 POP_TOP
+         
+         154        2158 LOAD_FAST                2 (buffer_pile)
+                    2160 LOAD_METHOD             19 (pop)
+                    2182 LOAD_CONST              11 (-1)
+                    2184 PRECALL                  1
+                    2188 CALL                     1
+                    2198 POP_TOP
+         
+         155        2200 EXTENDED_ARG             4
+                    2202 JUMP_BACKWARD         1063 (to 78)
+         
+         136     >> 2204 EXTENDED_ARG             4
+                    2206 JUMP_BACKWARD         1065 (to 78)
+         
+         158     >> 2208 LOAD_FAST                3 (stack)
+                    2210 GET_ITER
+                 >> 2212 FOR_ITER               140 (to 2494)
+                    2214 STORE_FAST              28 (stack_item)
+         
+         159        2216 LOAD_FAST               28 (stack_item)
+                    2218 LOAD_ATTR               25 (type_)
+                    2228 LOAD_METHOD             13 (split)
+                    2250 LOAD_CONST              29 ('_')
+                    2252 PRECALL                  1
+                    2256 CALL                     1
+                    2266 LOAD_CONST               1 (0)
+                    2268 BINARY_SUBSCR
+                    2278 LOAD_METHOD             12 (strip)
+                    2300 PRECALL                  0
+                    2304 CALL                     0
+                    2314 STORE_FAST              29 (short_type)
+         
+         160        2316 LOAD_FAST               29 (short_type)
+                    2318 LOAD_FAST               28 (stack_item)
+                    2320 LOAD_ATTR               26 (end_line)
+                    2330 CONTAINS_OP              1
+                    2332 POP_JUMP_FORWARD_IF_FALSE    79 (to 2492)
+         
+         161        2334 LOAD_CONST              12 ('.')
+                    2336 LOAD_METHOD             14 (join)
+                    2358 LOAD_FAST                4 (path)
+                    2360 PRECALL                  1
+                    2364 CALL                     1
+                    2374 STORE_FAST              30 (pathstr)
+         
+         162        2376 LOAD_GLOBAL             31 (NULL + logger)
+                    2388 LOAD_ATTR               27 (debug)
+         
+         163        2398 LOAD_CONST              30 ('End mismatch \nat ')
+                    2400 LOAD_FAST               30 (pathstr)
+                    2402 FORMAT_VALUE             0
+                    2404 LOAD_CONST              31 (' for ')
+                    2406 LOAD_FAST               29 (short_type)
+                    2408 FORMAT_VALUE             0
+                    2410 LOAD_CONST              32 (":\n '")
+                    2412 LOAD_FAST               28 (stack_item)
+                    2414 LOAD_ATTR               28 (start_line_idx)
+                    2424 FORMAT_VALUE             0
+                    2426 LOAD_CONST              33 ("' to '")
+                    2428 LOAD_FAST               28 (stack_item)
+                    2430 LOAD_ATTR               29 (end_line_idx)
+                    2440 FORMAT_VALUE             0
+                    2442 LOAD_CONST              34 ("'.\n For ")
+                    2444 LOAD_FAST               28 (stack_item)
+                    2446 LOAD_ATTR               25 (type_)
+                    2456 FORMAT_VALUE             0
+                    2458 LOAD_CONST              35 (' in ')
+                    2460 LOAD_FAST               28 (stack_item)
+                    2462 LOAD_ATTR               26 (end_line)
+                    2472 FORMAT_VALUE             0
+                    2474 BUILD_STRING            12
+         
+         162        2476 PRECALL                  1
+                    2480 CALL                     1
+                    2490 POP_TOP
+                 >> 2492 JUMP_BACKWARD          141 (to 2212)
+         
+         165     >> 2494 LOAD_GLOBAL             61 (NULL + len)
+                    2506 LOAD_FAST                5 (entry_)
+                    2508 PRECALL                  1
+                    2512 CALL                     1
+                    2522 LOAD_GLOBAL             61 (NULL + len)
+                    2534 LOAD_FAST                6 (out_)
+                    2536 PRECALL                  1
+                    2540 CALL                     1
+                    2550 COMPARE_OP               3 (!=)
+                    2556 POP_JUMP_FORWARD_IF_FALSE    69 (to 2696)
+         
+         166        2558 LOAD_GLOBAL              1 (NULL + zip)
+                    2570 LOAD_FAST                5 (entry_)
+                    2572 LOAD_FAST                6 (out_)
+                    2574 PRECALL                  2
+                    2578 CALL                     2
+                    2588 GET_ITER
+                 >> 2590 FOR_ITER                30 (to 2652)
+                    2592 UNPACK_SEQUENCE          2
+                    2596 STORE_FAST              31 (aa)
+                    2598 STORE_FAST              32 (bb)
+         
+         167        2600 LOAD_GLOBAL             31 (NULL + logger)
+                    2612 LOAD_ATTR               16 (warning)
+                    2622 LOAD_FAST               31 (aa)
+                    2624 FORMAT_VALUE             0
+                    2626 LOAD_CONST              36 ('<>')
+                    2628 LOAD_FAST               32 (bb)
+                    2630 FORMAT_VALUE             0
+                    2632 BUILD_STRING             3
+                    2634 PRECALL                  1
+                    2638 CALL                     1
+                    2648 POP_TOP
+                    2650 JUMP_BACKWARD           31 (to 2590)
+         
+         168     >> 2652 LOAD_GLOBAL             31 (NULL + logger)
+                    2664 LOAD_ATTR               31 (error)
+         
+         169        2674 LOAD_CONST              37 ('Missing one structure statement such as end if... removing file from current analysis')
+         
+         168        2676 PRECALL                  1
+                    2680 CALL                     1
+                    2690 POP_TOP
+         
+         171        2692 BUILD_MAP                0
+                    2694 RETURN_VALUE
+         
+         173     >> 2696 LOAD_GLOBAL             65 (NULL + struct_from_stack)
+                    2708 LOAD_FAST                3 (stack)
+                    2710 LOAD_GLOBAL             10 (PARTS)
+                    2722 LOAD_CONST               7 ('procedure')
+                    2724 BUILD_LIST               1
+                    2726 BINARY_OP                0 (+)
+                    2730 KW_NAMES                38
+                    2732 PRECALL                  2
+                    2736 CALL                     2
+                    2746 RETURN_VALUE
+         ExceptionTable:
+           1906 to 1920 -> 1924 [1]
+           1924 to 2030 -> 2032 [2] lasti
          consts
-            'Find all words before a left parenthesis in a line'
-            '('
-            50
+            'Extract structure from cleaned statements.'
             0
+            1
+            ' '
+            True
+            ('reverse',)
+            ('type_', 'path', 'name', 'first_line', 'line_idx', 'statement_idx', 'verbose')
+            'procedure'
+            '::'
             ''
-            '(.*?\\S)\\('
-            ',+-/*<>=;|(){}[]:~ '
+            '=>'
             -1
-            1
-         names      ('count', 're', 'findall', 'range', 'len', 'append')
-         varnames   ('line', 'pattern', 'matches', 'clean_matches', 'tokens', 'match_', 'token', 'i')
+            '.'
+            None
+            'Adding proxy '
+            ' (pointer to '
+            ') to '
+            ('type_', 'path', 'name', 'first_line', 'line_idx', 'statement_idx', 'verbose', 'callables')
+            ('verbose',)
+            '_type'
+            '('
+            ')'
+            'type'
+            'extends'
+            False
+            'end '
+            'end'
+            'No buffer for line '
+            ':'
+            '_'
+            'End mismatch \nat '
+            ' for '
+            ":\n '"
+            "' to '"
+            "'.\n For "
+            ' in '
+            '<>'
+            'Missing one structure statement such as end if... removing file from current analysis'
+            ('main_types',)
+         names      ('zip', 'stmt', 'lines', 'lstrip', 'sorted', 'PARTS', 'NESTS', 'startswith', 'append', '_parse_name_ftn', 'new_buffer_item', 'replace', 'strip', 'split', 'join', 'logger', 'warning', 'name', 'new_stack_item', 'pop', 'index', 'parents', 'IndexError', 'critical', 'RuntimeError', 'type_', 'end_line', 'debug', 'start_line_idx', 'end_line_idx', 'len', 'error', 'struct_from_stack')
+         varnames   ('stmts', 'verbose', 'buffer_pile', 'stack', 'path', 'entry_', 'out_', 'stat_idx', 'line', 'line_idx1', 'line_idx2', 'part', 'name', 'line_clean', 'front', 'tail', 'target', 'proxy', 'target_name', 'proxy_name', 'last_buff', 'buf_', 'strt_', 'end_', 'parent', 'read', 'char', 'msg', 'stack_item', 'short_type', 'pathstr', 'aa', 'bb')
          freevars   ()
          cellvars   ()
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       'find_words_before_left_parenthesis'
-         firstlineno 71
+         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py'
+         name       '_extract_on_cleaned_ftn'
+         firstlineno 38
          lnotab
-            0x02056401040304022a01040204010801040140011a0104011e020c012c
-            01
-      'type_'
-      'name'
-      'first_line'
-      'line_idx'
-      'statement_idx'
+            0x020204010401040204010401040146010a022a0540013c022a0120012a
+            0118010c0102010201020102010201020102f910ff100b04f002120a0178
+            01080130012801360204010402460136012a01100244020c010201020102
+            01020102010201020104f8120a18010c01020102010201020102fb10ff10
+            082a022a012a012a013e021e01400232012a010401040118010c0106010c
+            01040204010c0128021e0140025a012a01020114011201100128011efd08
+            0518010c01020102010201020102fb10ff10082a012a0104ed0416080164
+            0112012a0116014eff120340012a013401160102ff10030402
+      'line'
+      'line_nb'
       code
-         argcount  : 5
-         nlocals   : 5
+         argcount  : 2
+         nlocals   : 3
          stacksize : 5
          flags     : 3
-         code 0x97007c007c017c027c037c0466055300
-         102           0 RESUME                   0
-         
-         111           2 LOAD_FAST                0 (type_)
-         
-         112           4 LOAD_FAST                1 (name)
-         
-         113           6 LOAD_FAST                2 (first_line)
-         
-         114           8 LOAD_FAST                3 (line_idx)
-         
-         115          10 LOAD_FAST                4 (statement_idx)
-         
-         110          12 BUILD_TUPLE              5
-                      14 RETURN_VALUE
-         consts
-            'Forces buffers to keep the same logic across languages'
-         names      ()
-         varnames   ('type_', 'name', 'first_line', 'line_idx', 'statement_idx')
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       'buffer_item'
-         firstlineno 102
-         lnotab 0x0209020102010201020102fb
-      'start_line_idx'
-      'start_statement_idx'
-      'start_line'
-      'end_line_idx'
-      'end_statement_idx'
-      'end_line'
-      code
-         argcount  : 9
-         nlocals   : 9
-         stacksize : 9
-         flags     : 3
          code
-            0x970009007c026401190000000000000000007c016b0300000000722774
-            01000000000000000000006a010000000000000000640274050000000000
-            00000000007c02a6010000ab0100000000000000009b0064037c019b009d
-            04a6010000ab01000000000000000001006e212300740600000000000000
-            00000024007214010074090000000000000000000064047c019b0064059d
-            03a6010000ab010000000000000000820177007803590077017c007c017c
-            027c037c047c057c067c077c0866095300
-         123           0 RESUME                   0
-         
-         136           2 NOP
-         
-         137           4 LOAD_FAST                2 (path)
-                       6 LOAD_CONST               1 (-1)
-                       8 BINARY_SUBSCR
-                      18 LOAD_FAST                1 (name)
-                      20 COMPARE_OP               3 (!=)
-                      26 POP_JUMP_FORWARD_IF_FALSE    39 (to 106)
-         
-         138          28 LOAD_GLOBAL              1 (NULL + logger)
-                      40 LOAD_ATTR                1 (warning)
-                      50 LOAD_CONST               2 ('Path ')
-                      52 LOAD_GLOBAL              5 (NULL + str)
-                      64 LOAD_FAST                2 (path)
-                      66 PRECALL                  1
-                      70 CALL                     1
-                      80 FORMAT_VALUE             0
-                      82 LOAD_CONST               3 (' does not end with ')
-                      84 LOAD_FAST                1 (name)
-                      86 FORMAT_VALUE             0
-                      88 BUILD_STRING             4
-                      90 PRECALL                  1
-                      94 CALL                     1
-                     104 POP_TOP
-                 >>  106 JUMP_FORWARD            33 (to 174)
-                 >>  108 PUSH_EXC_INFO
-         
-         139         110 LOAD_GLOBAL              6 (IndexError)
-                     122 CHECK_EXC_MATCH
-                     124 POP_JUMP_FORWARD_IF_FALSE    20 (to 166)
-                     126 POP_TOP
-         
-         140         128 LOAD_GLOBAL              9 (NULL + RuntimeError)
-                     140 LOAD_CONST               4 ('Structure -')
-                     142 LOAD_FAST                1 (name)
-                     144 FORMAT_VALUE             0
-                     146 LOAD_CONST               5 ('- has no path')
-                     148 BUILD_STRING             3
-                     150 PRECALL                  1
-                     154 CALL                     1
-                     164 RAISE_VARARGS            1
-         
-         139     >>  166 RERAISE                  0
-                 >>  168 COPY                     3
-                     170 POP_EXCEPT
-                     172 RERAISE                  1
-         
-         143     >>  174 LOAD_FAST                0 (type_)
-         
-         144         176 LOAD_FAST                1 (name)
-         
-         145         178 LOAD_FAST                2 (path)
-         
-         146         180 LOAD_FAST                3 (start_line_idx)
-         
-         147         182 LOAD_FAST                4 (start_statement_idx)
-         
-         148         184 LOAD_FAST                5 (start_line)
-         
-         149         186 LOAD_FAST                6 (end_line_idx)
-         
-         150         188 LOAD_FAST                7 (end_statement_idx)
-         
-         151         190 LOAD_FAST                8 (end_line)
+            0x97007401000000000000000000007c00a6010000ab0100000000000000
+            007d007c00a0010000000000000000000000000000000000000000a60000
+            00ab00000000000000000064011900000000000000000074040000000000
+            00000000007600727c7c00a0010000000000000000000000000000000000
+            000000a6000000ab00000000000000000064011900000000000000000074
+            07000000000000000000007c01a6010000ab0100000000000000007a0000
+            007d0264027c007600724c7c0264037c00a0010000000000000000000000
+            0000000000000000006404a6010000ab0100000000000000006405190000
+            00000000000000a001000000000000000000000000000000000000000064
+            06a6010000ab010000000000000000640519000000000000000000a00400
+            00000000000000000000000000000000000000a6000000ab000000000000
+            0000007a0000007a0d00007d027c0253007c00a001000000000000000000
+            0000000000000000000000a6000000ab0000000000000000006401190000
+            00000000000000a005000000000000000000000000000000000000000064
+            07a6010000ab010000000000000000724e64087c007600722e7c00a00100
+            000000000000000000000000000000000000006408a6010000ab01000000
+            0000000000640519000000000000000000a0040000000000000000000000
+            000000000000000000a6000000ab0000000000000000007d026e1a7c00a0
+            010000000000000000000000000000000000000000a6000000ab00000000
+            00000000006409190000000000000000007d027c0253007c00a006000000
+            00000000000000000000000000000000006406640aa6020000ab02000000
+            00000000007d0009007c00a0010000000000000000000000000000000000
+            000000a6000000ab0000000000000000006409190000000000000000007d
+            026e3a2300740e000000000000000000002400722d01007c00a001000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            006401190000000000000000007407000000000000000000007c01a60100
+            00ab0100000000000000007a0000007d0259006e0477007803590077017c
+            025300
+         176           0 RESUME                   0
+         
+         181           2 LOAD_GLOBAL              1 (NULL + rm_parenthesis_content)
+                      14 LOAD_FAST                0 (line)
+                      16 PRECALL                  1
+                      20 CALL                     1
+                      30 STORE_FAST               0 (line)
+         
+         183          32 LOAD_FAST                0 (line)
+                      34 LOAD_METHOD              1 (split)
+                      56 PRECALL                  0
+                      60 CALL                     0
+                      70 LOAD_CONST               1 (0)
+                      72 BINARY_SUBSCR
+                      82 LOAD_GLOBAL              4 (NESTS)
+                      94 CONTAINS_OP              0
+                      96 POP_JUMP_FORWARD_IF_FALSE   124 (to 346)
+         
+         184          98 LOAD_FAST                0 (line)
+                     100 LOAD_METHOD              1 (split)
+                     122 PRECALL                  0
+                     126 CALL                     0
+                     136 LOAD_CONST               1 (0)
+                     138 BINARY_SUBSCR
+                     148 LOAD_GLOBAL              7 (NULL + str)
+                     160 LOAD_FAST                1 (line_nb)
+                     162 PRECALL                  1
+                     166 CALL                     1
+                     176 BINARY_OP                0 (+)
+                     180 STORE_FAST               2 (name)
+         
+         185         182 LOAD_CONST               2 ('#LABEL')
+                     184 LOAD_FAST                0 (line)
+                     186 CONTAINS_OP              0
+                     188 POP_JUMP_FORWARD_IF_FALSE    76 (to 342)
+         
+         186         190 LOAD_FAST                2 (name)
+                     192 LOAD_CONST               3 ('_')
+                     194 LOAD_FAST                0 (line)
+                     196 LOAD_METHOD              1 (split)
+                     218 LOAD_CONST               4 ('#')
+                     220 PRECALL                  1
+                     224 CALL                     1
+                     234 LOAD_CONST               5 (-1)
+                     236 BINARY_SUBSCR
+                     246 LOAD_METHOD              1 (split)
+                     268 LOAD_CONST               6 (':')
+                     270 PRECALL                  1
+                     274 CALL                     1
+                     284 LOAD_CONST               5 (-1)
+                     286 BINARY_SUBSCR
+                     296 LOAD_METHOD              4 (strip)
+                     318 PRECALL                  0
+                     322 CALL                     0
+                     332 BINARY_OP                0 (+)
+                     336 BINARY_OP               13 (+=)
+                     340 STORE_FAST               2 (name)
+         
+         187     >>  342 LOAD_FAST                2 (name)
+                     344 RETURN_VALUE
+         
+         189     >>  346 LOAD_FAST                0 (line)
+                     348 LOAD_METHOD              1 (split)
+                     370 PRECALL                  0
+                     374 CALL                     0
+                     384 LOAD_CONST               1 (0)
+                     386 BINARY_SUBSCR
+                     396 LOAD_METHOD              5 (startswith)
+                     418 LOAD_CONST               7 ('type')
+                     420 PRECALL                  1
+                     424 CALL                     1
+                     434 POP_JUMP_FORWARD_IF_FALSE    78 (to 592)
+         
+         191         436 LOAD_CONST               8 ('::')
+                     438 LOAD_FAST                0 (line)
+                     440 CONTAINS_OP              0
+                     442 POP_JUMP_FORWARD_IF_FALSE    46 (to 536)
+         
+         192         444 LOAD_FAST                0 (line)
+                     446 LOAD_METHOD              1 (split)
+                     468 LOAD_CONST               8 ('::')
+                     470 PRECALL                  1
+                     474 CALL                     1
+                     484 LOAD_CONST               5 (-1)
+                     486 BINARY_SUBSCR
+                     496 LOAD_METHOD              4 (strip)
+                     518 PRECALL                  0
+                     522 CALL                     0
+                     532 STORE_FAST               2 (name)
+                     534 JUMP_FORWARD            26 (to 588)
+         
+         194     >>  536 LOAD_FAST                0 (line)
+                     538 LOAD_METHOD              1 (split)
+                     560 PRECALL                  0
+                     564 CALL                     0
+                     574 LOAD_CONST               9 (1)
+                     576 BINARY_SUBSCR
+                     586 STORE_FAST               2 (name)
+         
+         195     >>  588 LOAD_FAST                2 (name)
+                     590 RETURN_VALUE
+         
+         197     >>  592 LOAD_FAST                0 (line)
+                     594 LOAD_METHOD              6 (replace)
+                     616 LOAD_CONST               6 (':')
+                     618 LOAD_CONST              10 (' ')
+                     620 PRECALL                  2
+                     624 CALL                     2
+                     634 STORE_FAST               0 (line)
+         
+         198         636 NOP
+         
+         199         638 LOAD_FAST                0 (line)
+                     640 LOAD_METHOD              1 (split)
+                     662 PRECALL                  0
+                     666 CALL                     0
+                     676 LOAD_CONST               9 (1)
+                     678 BINARY_SUBSCR
+                     688 STORE_FAST               2 (name)
+                     690 JUMP_FORWARD            58 (to 808)
+                 >>  692 PUSH_EXC_INFO
+         
+         200         694 LOAD_GLOBAL             14 (IndexError)
+                     706 CHECK_EXC_MATCH
+                     708 POP_JUMP_FORWARD_IF_FALSE    45 (to 800)
+                     710 POP_TOP
+         
+         201         712 LOAD_FAST                0 (line)
+                     714 LOAD_METHOD              1 (split)
+                     736 PRECALL                  0
+                     740 CALL                     0
+                     750 LOAD_CONST               1 (0)
+                     752 BINARY_SUBSCR
+                     762 LOAD_GLOBAL              7 (NULL + str)
+                     774 LOAD_FAST                1 (line_nb)
+                     776 PRECALL                  1
+                     780 CALL                     1
+                     790 BINARY_OP                0 (+)
+                     794 STORE_FAST               2 (name)
+                     796 POP_EXCEPT
+                     798 JUMP_FORWARD             4 (to 808)
+         
+         200     >>  800 RERAISE                  0
+                 >>  802 COPY                     3
+                     804 POP_EXCEPT
+                     806 RERAISE                  1
          
-         142         192 BUILD_TUPLE              9
-                     194 RETURN_VALUE
+         204     >>  808 LOAD_FAST                2 (name)
+                     810 RETURN_VALUE
          ExceptionTable:
-           4 to 104 -> 108 [0]
-           108 to 166 -> 168 [1] lasti
+           638 to 688 -> 692 [0]
+           692 to 794 -> 802 [1] lasti
+           800 to 800 -> 802 [1] lasti
          consts
-            'Forces stacks to keep the same logic across languages'
+            'expect a lowercase stripped line\n    takes the second word as the name\n    '
+            0
+            '#LABEL'
+            '_'
+            '#'
             -1
-            'Path '
-            ' does not end with '
-            'Structure -'
-            '- has no path'
-         names      ('logger', 'warning', 'str', 'IndexError', 'RuntimeError')
-         varnames   ('type_', 'name', 'path', 'start_line_idx', 'start_statement_idx', 'start_line', 'end_line_idx', 'end_statement_idx', 'end_line')
+            ':'
+            'type'
+            '::'
+            1
+            ' '
+         names      ('rm_parenthesis_content', 'split', 'NESTS', 'str', 'strip', 'startswith', 'replace', 'IndexError')
+         varnames   ('line', 'line_nb', 'name')
          freevars   ()
          cellvars   ()
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       'stack_item'
-         firstlineno 123
+         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py'
+         name       '_parse_name_ftn'
+         firstlineno 176
          lnotab
-            0x020d020118015201120126ff0804020102010201020102010201020102
-            0102f7
-      'stack'
-      'main_types'
-      'skip_types'
+            0x02051e02420154010801980104025a0208015c02340104022c01020138
+            01120158ff0804
+      'code'
       code
-         argcount  : 3
-         nlocals   : 16
-         stacksize : 10
+         argcount  : 1
+         nlocals   : 4
+         stacksize : 7
          flags     : 3
          code
-            0x970069007d037c02800267007d0267007d047c0044005d1f5e037d057d
-            067d077d087c057c02760072157c04a00000000000000000000000000000
-            000000000000007c07a6010000ab01000000000000000001008c207c0044
-            005d3f5c0900007d057d067d077d097d0a7d0b7d0c7d0d7d0e7403000000
-            000000000000007c077c04a6020000ab0200000000000000007d0f7c057c
-            017600721f7c0f7c067c057c0b7c097c0c67027c0a7c0d67026700690064
-            029c087c037405000000000000000000007c0fa6010000ab010000000000
-            0000003c0000008c407c035300
-         155           0 RESUME                   0
-         
-         158           2 BUILD_MAP                0
-                       4 STORE_FAST               3 (struct)
-         
-         159           6 LOAD_FAST                2 (skip_types)
-                       8 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 14)
-         
-         160          10 BUILD_LIST               0
-                      12 STORE_FAST               2 (skip_types)
-         
-         162     >>   14 BUILD_LIST               0
-                      16 STORE_FAST               4 (path_to_skip)
-         
-         163          18 LOAD_FAST                0 (stack)
-                      20 GET_ITER
-                 >>   22 FOR_ITER                31 (to 86)
-                      24 UNPACK_EX                3
-                      26 STORE_FAST               5 (type_)
-                      28 STORE_FAST               6 (name)
-                      30 STORE_FAST               7 (path)
-                      32 STORE_FAST               8 (_)
-         
-         164          34 LOAD_FAST                5 (type_)
-                      36 LOAD_FAST                2 (skip_types)
-                      38 CONTAINS_OP              0
-                      40 POP_JUMP_FORWARD_IF_FALSE    21 (to 84)
-         
-         165          42 LOAD_FAST                4 (path_to_skip)
-                      44 LOAD_METHOD              0 (append)
-                      66 LOAD_FAST                7 (path)
-                      68 PRECALL                  1
-                      72 CALL                     1
-                      82 POP_TOP
-                 >>   84 JUMP_BACKWARD           32 (to 22)
-         
-         177     >>   86 LOAD_FAST                0 (stack)
+            0x970067007d017c0044005d817d0264017c02760072477c01a000000000
+            00000000000000000000000000000000007c02a001000000000000000000
+            00000000000000000000006402a6010000ab010000000000000000640319
+            000000000000000000a00100000000000000000000000000000000000000
+            00a6000000ab000000000000000000640419000000000000000000a60100
+            00ab01000000000000000001008c4d7c01a0020000000000000000000000
+            0000000000000000007407000000000000000000007c02a0040000000000
+            000000000000000000000000000000a6000000ab000000000000000000a6
+            010000ab010000000000000000a6010000ab01000000000000000001008c
+            8264058400740b000000000000000000007c01a6010000ab010000000000
+            0000004400a6000000ab0000000000000000007d03740d00000000000000
+            0000007c03a6010000ab0100000000000000005300
+         210           0 RESUME                   0
          
-         167          88 GET_ITER
-                 >>   90 FOR_ITER                63 (to 218)
-                      92 UNPACK_SEQUENCE          9
+         212           2 BUILD_LIST               0
+                       4 STORE_FAST               1 (candidates)
          
-         168          96 STORE_FAST               5 (type_)
-         
-         169          98 STORE_FAST               6 (name)
-         
-         170         100 STORE_FAST               7 (path)
-         
-         171         102 STORE_FAST               9 (start_line_idx)
-         
-         172         104 STORE_FAST              10 (start_statement_idx)
-         
-         173         106 STORE_FAST              11 (start_line)
-         
-         174         108 STORE_FAST              12 (end_line_idx)
-         
-         175         110 STORE_FAST              13 (end_statement_idx)
-         
-         176         112 STORE_FAST              14 (end_line)
-         
-         180         114 LOAD_GLOBAL              3 (NULL + path_clean)
-                     126 LOAD_FAST                7 (path)
-                     128 LOAD_FAST                4 (path_to_skip)
-                     130 PRECALL                  2
-                     134 CALL                     2
-                     144 STORE_FAST              15 (cleaned_path)
-         
-         182         146 LOAD_FAST                5 (type_)
-                     148 LOAD_FAST                1 (main_types)
-                     150 CONTAINS_OP              0
-                     152 POP_JUMP_FORWARD_IF_FALSE    31 (to 216)
-         
-         184         154 LOAD_FAST               15 (cleaned_path)
-         
-         185         156 LOAD_FAST                6 (name)
-         
-         186         158 LOAD_FAST                5 (type_)
-         
-         187         160 LOAD_FAST               11 (start_line)
-         
-         188         162 LOAD_FAST                9 (start_line_idx)
-                     164 LOAD_FAST               12 (end_line_idx)
-                     166 BUILD_LIST               2
-         
-         189         168 LOAD_FAST               10 (start_statement_idx)
-                     170 LOAD_FAST               13 (end_statement_idx)
-                     172 BUILD_LIST               2
-         
-         190         174 BUILD_LIST               0
-         
-         191         176 BUILD_MAP                0
+         213           6 LOAD_FAST                0 (code)
+                       8 GET_ITER
+                 >>   10 FOR_ITER               129 (to 270)
+                      12 STORE_FAST               2 (line)
          
-         183         178 LOAD_CONST               2 (('path', 'name', 'type', 'linestart', 'lines', 'statements', 'contains', 'annotations'))
-                     180 BUILD_CONST_KEY_MAP      8
-                     182 LOAD_FAST                3 (struct)
-                     184 LOAD_GLOBAL              5 (NULL + list2pathref)
-                     196 LOAD_FAST               15 (cleaned_path)
-                     198 PRECALL                  1
-                     202 CALL                     1
-                     212 STORE_SUBSCR
-                 >>  216 JUMP_BACKWARD           64 (to 90)
+         214          14 LOAD_CONST               1 (' call ')
+                      16 LOAD_FAST                2 (line)
+                      18 CONTAINS_OP              0
+                      20 POP_JUMP_FORWARD_IF_FALSE    71 (to 164)
+         
+         215          22 LOAD_FAST                1 (candidates)
+                      24 LOAD_METHOD              0 (append)
+                      46 LOAD_FAST                2 (line)
+                      48 LOAD_METHOD              1 (split)
+                      70 LOAD_CONST               2 ('(')
+                      72 PRECALL                  1
+                      76 CALL                     1
+                      86 LOAD_CONST               3 (0)
+                      88 BINARY_SUBSCR
+                      98 LOAD_METHOD              1 (split)
+                     120 PRECALL                  0
+                     124 CALL                     0
+                     134 LOAD_CONST               4 (-1)
+                     136 BINARY_SUBSCR
+                     146 PRECALL                  1
+                     150 CALL                     1
+                     160 POP_TOP
+                     162 JUMP_BACKWARD           77 (to 10)
          
-         194     >>  218 LOAD_FAST                3 (struct)
-                     220 RETURN_VALUE
-         consts
-            'Build a dictionary of all structures'
-            None
-            ('path', 'name', 'type', 'linestart', 'lines', 'statements', 'contains', 'annotations')
-         names      ('append', 'path_clean', 'list2pathref')
-         varnames   ('stack', 'main_types', 'skip_types', 'struct', 'path_to_skip', 'type_', 'name', 'path', '_', 'start_line_idx', 'start_statement_idx', 'start_line', 'end_line_idx', 'end_statement_idx', 'end_line', 'cleaned_path')
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       'struct_from_stack'
-         firstlineno 155
-         lnotab
-            0x02030401040104020401100108012c0c02f60801020102010201020102
-            01020102010201020420020802020102010201020106010601020102f828
-            0b
-      'struct'
-      code
-         argcount  : 1
-         nlocals   : 4
-         stacksize : 4
-         flags     : 3
-         code
-            0x970069007d017c00a00000000000000000000000000000000000000000
-            00a6000000ab00000000000000000044005d6f5c0200007d027d0369007c
-            017c023c0000007c03640119000000000000000000640219000000000000
-            0000007c036401190000000000000000006403190000000000000000007a
-            0a000064047a0000007c017c021900000000000000000064053c0000007c
-            036406190000000000000000006402190000000000000000007c03640619
-            0000000000000000006403190000000000000000007a0a00007c017c0219
-            00000000000000000064073c00000067007c017c02190000000000000000
-            0064083c00000067007c017c021900000000000000000064093c0000008c
-            707c015300
-         197           0 RESUME                   0
-         
-         199           2 BUILD_MAP                0
-                       4 STORE_FAST               1 (struct_aspects)
-         
-         200           6 LOAD_FAST                0 (struct)
-                       8 LOAD_METHOD              0 (items)
-                      30 PRECALL                  0
-                      34 CALL                     0
-                      44 GET_ITER
-                 >>   46 FOR_ITER               111 (to 270)
-                      48 UNPACK_SEQUENCE          2
-                      52 STORE_FAST               2 (part)
-                      54 STORE_FAST               3 (data)
-         
-         201          56 BUILD_MAP                0
-                      58 LOAD_FAST                1 (struct_aspects)
-                      60 LOAD_FAST                2 (part)
-                      62 STORE_SUBSCR
-         
-         202          66 LOAD_FAST                3 (data)
-                      68 LOAD_CONST               1 ('lines')
-                      70 BINARY_SUBSCR
-                      80 LOAD_CONST               2 (-1)
-                      82 BINARY_SUBSCR
-                      92 LOAD_FAST                3 (data)
-                      94 LOAD_CONST               1 ('lines')
-                      96 BINARY_SUBSCR
-                     106 LOAD_CONST               3 (0)
-                     108 BINARY_SUBSCR
-                     118 BINARY_OP               10 (-)
-                     122 LOAD_CONST               4 (1)
-                     124 BINARY_OP                0 (+)
-                     128 LOAD_FAST                1 (struct_aspects)
-                     130 LOAD_FAST                2 (part)
-                     132 BINARY_SUBSCR
-                     142 LOAD_CONST               5 ('NLOC')
-                     144 STORE_SUBSCR
-         
-         203         148 LOAD_FAST                3 (data)
-                     150 LOAD_CONST               6 ('statements')
-                     152 BINARY_SUBSCR
-                     162 LOAD_CONST               2 (-1)
-                     164 BINARY_SUBSCR
-                     174 LOAD_FAST                3 (data)
-                     176 LOAD_CONST               6 ('statements')
-                     178 BINARY_SUBSCR
-                     188 LOAD_CONST               3 (0)
-                     190 BINARY_SUBSCR
-                     200 BINARY_OP               10 (-)
-                     204 LOAD_FAST                1 (struct_aspects)
-                     206 LOAD_FAST                2 (part)
-                     208 BINARY_SUBSCR
-                     218 LOAD_CONST               7 ('ssize')
-                     220 STORE_SUBSCR
-         
-         204         224 BUILD_LIST               0
-                     226 LOAD_FAST                1 (struct_aspects)
-                     228 LOAD_FAST                2 (part)
-                     230 BINARY_SUBSCR
-                     240 LOAD_CONST               8 ('callables')
-                     242 STORE_SUBSCR
-         
-         205         246 BUILD_LIST               0
-                     248 LOAD_FAST                1 (struct_aspects)
-                     250 LOAD_FAST                2 (part)
-                     252 BINARY_SUBSCR
-                     262 LOAD_CONST               9 ('CCN')
-                     264 STORE_SUBSCR
-                     268 JUMP_BACKWARD          112 (to 46)
+         217     >>  164 LOAD_FAST                1 (candidates)
+                     166 LOAD_METHOD              2 (extend)
+                     188 LOAD_GLOBAL              7 (NULL + find_words_before_left_parenthesis)
+                     200 LOAD_FAST                2 (line)
+                     202 LOAD_METHOD              4 (strip)
+                     224 PRECALL                  0
+                     228 CALL                     0
+                     238 PRECALL                  1
+                     242 CALL                     1
+                     252 PRECALL                  1
+                     256 CALL                     1
+                     266 POP_TOP
+                     268 JUMP_BACKWARD          130 (to 10)
+         
+         219     >>  270 LOAD_CONST               5 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py", line 219>)
+                     272 MAKE_FUNCTION            0
+                     274 LOAD_GLOBAL             11 (NULL + set)
+                     286 LOAD_FAST                1 (candidates)
+                     288 PRECALL                  1
+                     292 CALL                     1
+                     302 GET_ITER
+                     304 PRECALL                  0
+                     308 CALL                     0
+                     318 STORE_FAST               3 (matches)
          
-         206     >>  270 LOAD_FAST                1 (struct_aspects)
-                     272 RETURN_VALUE
+         221         320 LOAD_GLOBAL             13 (NULL + sorted)
+                     332 LOAD_FAST                3 (matches)
+                     334 PRECALL                  1
+                     338 CALL                     1
+                     348 RETURN_VALUE
          consts
-            'Compute the size of strict items (statefull)'
-            'lines'
-            -1
+            'Find callables in python'
+            ' call '
+            '('
             0
-            1
-            'NLOC'
-            'statements'
-            'ssize'
-            'callables'
-            'CCN'
-         names      ('items',)
-         varnames   ('struct', 'struct_aspects', 'part', 'data')
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       'get_struct_sizes'
-         firstlineno 197
-         lnotab 0x0202040132010a0152014c0116011801
-      'list_'
-      'parent'
-      code
-         argcount  : 2
-         nlocals   : 2
-         stacksize : 2
-         flags     : 3
-         code
-            0x8701970088016601640184087c004400a6000000ab0000000000000000
-            005300
-                       0 MAKE_CELL                1 (parent)
-         
-         210           2 RESUME                   0
-         
-         212           4 LOAD_CLOSURE             1 (parent)
-                       6 BUILD_TUPLE              1
-                       8 LOAD_CONST               1 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 212>)
-                      10 MAKE_FUNCTION            8 (closure)
-         
-         214          12 LOAD_FAST                0 (list_)
-         
-         212          14 GET_ITER
-                      16 PRECALL                  0
-                      20 CALL                     0
-                      30 RETURN_VALUE
-         consts
-            'Replace the self keyword in a parentality path'
+            -1
             code
                argcount  : 1
                nlocals   : 2
-               stacksize : 7
+               stacksize : 4
                flags     : 19
                code
-                  0x9501970067007c005d1b7d017c01a00000000000000000000000000000
-                  000000000000006400890264017a000000a6020000ab0200000000000000
-                  0091028c1c5300
-                             0 COPY_FREE_VARS           1
-               
-               212           2 RESUME                   0
-                             4 BUILD_LIST               0
-                             6 LOAD_FAST                0 (.0)
-                       >>    8 FOR_ITER                27 (to 64)
-               
-               214          10 STORE_FAST               1 (item)
-               
-               213          12 LOAD_FAST                1 (item)
-                            14 LOAD_METHOD              0 (replace)
-                            36 LOAD_CONST               0 ('self.')
-                            38 LOAD_DEREF               2 (parent)
-                            40 LOAD_CONST               1 ('.')
-                            42 BINARY_OP                0 (+)
-                            46 PRECALL                  2
-                            50 CALL                     2
-               
-               212          60 LIST_APPEND              2
-                            62 JUMP_BACKWARD           28 (to 8)
-                       >>   64 RETURN_VALUE
+                  0x970067007c005d0d7d017c017400000000000000000000007601af0b7c
+                  0191028c0e5300
+               219           0 RESUME                   0
+                             2 BUILD_LIST               0
+                             4 LOAD_FAST                0 (.0)
+                       >>    6 FOR_ITER                13 (to 34)
+                             8 STORE_FAST               1 (cand)
+                            10 LOAD_FAST                1 (cand)
+                            12 LOAD_GLOBAL              0 (INTRINSICS)
+                            24 CONTAINS_OP              1
+                            26 POP_JUMP_BACKWARD_IF_FALSE    11 (to 6)
+                            28 LOAD_FAST                1 (cand)
+                            30 LIST_APPEND              2
+                            32 JUMP_BACKWARD           14 (to 6)
+                       >>   34 RETURN_VALUE
                consts
-                  'self.'
-                  '.'
-               names      ('replace',)
-               varnames   ('.0', 'item')
-               freevars   ('parent',)
+               names      ('INTRINSICS',)
+               varnames   ('.0', 'cand')
+               freevars   ()
                cellvars   ()
-               filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
+               filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py'
                name       '<listcomp>'
-               firstlineno 212
-               lnotab 0x0a0202ff30ff
-         names      ()
-         varnames   ('list_', 'parent')
-         freevars   ()
-         cellvars   ('parent',)
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       'replace_self'
-         firstlineno 210
-         lnotab 0x0402080202fe
-      'beg'
-      'end'
-      'safes'
-      code
-         argcount  : 3
-         nlocals   : 7
-         stacksize : 5
-         flags     : 3
-         code
-            0x970067007d037401000000000000000000007c007c0164017a000000a6
-            020000ab02000000000000000044005d3a7d0464027d057c0244005d1c7d
-            067c047c066403190000000000000000006b0500000000720e7c047c0664
-            01190000000000000000006b0100000000720264047d058c1d7c0573157c
-            03a00100000000000000000000000000000000000000007c04a6010000ab
-            01000000000000000001008c3b7c035300
-         218           0 RESUME                   0
-         
-         230           2 BUILD_LIST               0
-                       4 STORE_FAST               3 (iter_)
-         
-         231           6 LOAD_GLOBAL              1 (NULL + range)
-                      18 LOAD_FAST                0 (beg)
-                      20 LOAD_FAST                1 (end)
-                      22 LOAD_CONST               1 (1)
-                      24 BINARY_OP                0 (+)
-                      28 PRECALL                  2
-                      32 CALL                     2
-                      42 GET_ITER
-                 >>   44 FOR_ITER                58 (to 162)
-                      46 STORE_FAST               4 (i)
-         
-         232          48 LOAD_CONST               2 (False)
-                      50 STORE_FAST               5 (blocked)
-         
-         233          52 LOAD_FAST                2 (safes)
-                      54 GET_ITER
-                 >>   56 FOR_ITER                28 (to 114)
-                      58 STORE_FAST               6 (safe)
-         
-         234          60 LOAD_FAST                4 (i)
-                      62 LOAD_FAST                6 (safe)
-                      64 LOAD_CONST               3 (0)
-                      66 BINARY_SUBSCR
-                      76 COMPARE_OP               5 (>=)
-                      82 POP_JUMP_FORWARD_IF_FALSE    14 (to 112)
-                      84 LOAD_FAST                4 (i)
-                      86 LOAD_FAST                6 (safe)
-                      88 LOAD_CONST               1 (1)
-                      90 BINARY_SUBSCR
-                     100 COMPARE_OP               1 (<=)
-                     106 POP_JUMP_FORWARD_IF_FALSE     2 (to 112)
-         
-         236         108 LOAD_CONST               4 (True)
-                     110 STORE_FAST               5 (blocked)
-                 >>  112 JUMP_BACKWARD           29 (to 56)
-         
-         237     >>  114 LOAD_FAST                5 (blocked)
-                     116 POP_JUMP_FORWARD_IF_TRUE    21 (to 160)
-         
-         238         118 LOAD_FAST                3 (iter_)
-                     120 LOAD_METHOD              1 (append)
-                     142 LOAD_FAST                4 (i)
-                     144 PRECALL                  1
-                     148 CALL                     1
-                     158 POP_TOP
-                 >>  160 JUMP_BACKWARD           59 (to 44)
-         
-         239     >>  162 LOAD_FAST                3 (iter_)
-                     164 RETURN_VALUE
-         consts
-            'Return an iterable stripped from safe zones\n    beg=100\n    end = 110\n    safes = [[103,104],[106,109]]\n\n    100\n    101\n    102\n    105\n    \n    '
-            1
-            False
-            0
-            True
-         names      ('range', 'append')
-         varnames   ('beg', 'end', 'safes', 'iter_', 'i', 'blocked', 'safe')
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       '_strip_safe_lines'
-         firstlineno 218
-         lnotab 0x020c04012a01040108013002060104012c01
-      'struct_in'
-      code
-         argcount  : 2
-         nlocals   : 5
-         stacksize : 6
-         flags     : 3
-         code
-            0x97007c007c01190000000000000000007d0267007d037c026401190000
-            0000000000000044005d437d047c03a00000000000000000000000000000
-            000000000000007c007c0419000000000000000000640219000000000000
-            00000064031900000000000000000064047a0a00007c007c041900000000
-            000000000064021900000000000000000064041900000000000000000064
-            047a0a00006702a6010000ab01000000000000000001008c447403000000
-            000000000000007c02640219000000000000000000640319000000000000
-            00000064047a0a00007c0264021900000000000000000064041900000000
-            000000000064047a0a00007c03a6030000ab0300000000000000005300
-         242           0 RESUME                   0
-         
-         248           2 LOAD_FAST                0 (struct_in)
-                       4 LOAD_FAST                1 (name)
-                       6 BINARY_SUBSCR
-                      16 STORE_FAST               2 (data)
-         
-         249          18 BUILD_LIST               0
-                      20 STORE_FAST               3 (safes)
-         
-         250          22 LOAD_FAST                2 (data)
-                      24 LOAD_CONST               1 ('contains')
-                      26 BINARY_SUBSCR
-                      36 GET_ITER
-                 >>   38 FOR_ITER                67 (to 174)
-                      40 STORE_FAST               4 (sub_name)
-         
-         251          42 LOAD_FAST                3 (safes)
-                      44 LOAD_METHOD              0 (append)
-                      66 LOAD_FAST                0 (struct_in)
-                      68 LOAD_FAST                4 (sub_name)
-                      70 BINARY_SUBSCR
-                      80 LOAD_CONST               2 ('statements')
-                      82 BINARY_SUBSCR
-                      92 LOAD_CONST               3 (0)
-                      94 BINARY_SUBSCR
-                     104 LOAD_CONST               4 (1)
-                     106 BINARY_OP               10 (-)
-                     110 LOAD_FAST                0 (struct_in)
-                     112 LOAD_FAST                4 (sub_name)
-                     114 BINARY_SUBSCR
-                     124 LOAD_CONST               2 ('statements')
-                     126 BINARY_SUBSCR
-                     136 LOAD_CONST               4 (1)
-                     138 BINARY_SUBSCR
-                     148 LOAD_CONST               4 (1)
-                     150 BINARY_OP               10 (-)
-                     154 BUILD_LIST               2
-                     156 PRECALL                  1
-                     160 CALL                     1
-                     170 POP_TOP
-                     172 JUMP_BACKWARD           68 (to 38)
-         
-         253     >>  174 LOAD_GLOBAL              3 (NULL + _strip_safe_lines)
-                     186 LOAD_FAST                2 (data)
-                     188 LOAD_CONST               2 ('statements')
-                     190 BINARY_SUBSCR
-                     200 LOAD_CONST               3 (0)
-                     202 BINARY_SUBSCR
-                     212 LOAD_CONST               4 (1)
-                     214 BINARY_OP               10 (-)
-                     218 LOAD_FAST                2 (data)
-                     220 LOAD_CONST               2 ('statements')
-                     222 BINARY_SUBSCR
-                     232 LOAD_CONST               4 (1)
-                     234 BINARY_SUBSCR
-                     244 LOAD_CONST               4 (1)
-                     246 BINARY_OP               10 (-)
-                     250 LOAD_FAST                3 (safes)
-                     252 PRECALL                  3
-                     256 CALL                     3
-                     266 RETURN_VALUE
-         consts
-            'returns an iterable with only the statement relative to this part\n    excluding contained parts.\n    \n    WARNING:The -1 on statements is systematic because statements numbering is starting at 1\n    '
-            'contains'
-            'statements'
-            0
-            1
-         names      ('append', '_strip_safe_lines')
-         varnames   ('struct_in', 'name', 'data', 'safes', 'sub_name')
+               firstlineno 219
+               lnotab 0x
+         names      ('append', 'split', 'extend', 'find_words_before_left_parenthesis', 'strip', 'set', 'sorted')
+         varnames   ('code', 'candidates', 'line', 'matches')
          freevars   ()
          cellvars   ()
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       'struct_actual_lines'
-         firstlineno 242
-         lnotab 0x02061001040114018402
-      'clean_code'
-      'find_callables'
-      'compute_ccn'
+         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py'
+         name       'find_callables_ftn'
+         firstlineno 210
+         lnotab 0x02020401080108018e026a023202
       code
-         argcount  : 4
-         nlocals   : 12
+         argcount  : 1
+         nlocals   : 3
          stacksize : 6
          flags     : 3
          code
-            0x870197007401000000000000000000007c00a6010000ab010000000000
-            0000007d047c04a0010000000000000000000000000000000000000000a6
-            000000ab00000000000000000044005d4b5c0200007d057d067c06640119
-            0000000000000000006402190000000000000000007c0664011900000000
-            00000000006403190000000000000000007a0a000064047a0000007c0664
-            053c0000007c066406190000000000000000006402190000000000000000
-            007c066406190000000000000000006403190000000000000000007a0a00
-            0064047a0000007c0664073c0000008c4c7c04a001000000000000000000
-            0000000000000000000000a6000000ab00000000000000000044005da75c
-            0200007d077d067c066408190000000000000000007d0874050000000000
-            00000000007c06640819000000000000000000a6010000ab010000000000
-            00000064046b040000000072767c06640819000000000000000000640964
-            028502190000000000000000007d0909007c047407000000000000000000
-            007c09a6010000ab01000000000000000019000000000000000000640a19
-            000000000000000000a00400000000000000000000000000000000000000
-            007407000000000000000000007c08a6010000ab010000000000000000a6
-            010000ab01000000000000000001006e102300740a000000000000000000
-            0024007203010059006e0477007803590077017407000000000000000000
-            007c09a6010000ab0100000000000000007c047c07190000000000000000
-            00640b3c0000008c9c64097c047c0719000000000000000000640b3c0000
-            008ca87c04a0010000000000000000000000000000000000000000a60000
-            00ab00000000000000000044005db45c0200007d077d06740d0000000000
-            00000000007c047c07a6020000ab0200000000000000007d0a8801660164
-            0c84087c0a4400a6000000ab0000000000000000007d0b02007c027c0ba6
-            010000ab0100000000000000007c06640d3c0000007c047c071900000000
-            0000000000640b190000000000000000008125740f000000000000000000
-            007c06640d190000000000000000007c047c071900000000000000000064
-            0b19000000000000000000a6020000ab0200000000000000007c06640d3c
-            0000007c047c0719000000000000000000640e1900000000000000000064
-            0f76007232740f000000000000000000007c06640a190000000000000000
-            007c07a6020000ab0200000000000000007c06640a3c000000740f000000
-            000000000000007c06640d190000000000000000007c07a6020000ab0200
-            000000000000007c06640d3c00000002007c037c0ba6010000ab01000000
-            00000000007c0664103c0000008cb57c045300
-                       0 MAKE_CELL                1 (clean_code)
-         
-         256           2 RESUME                   0
-         
-         258           4 LOAD_GLOBAL              1 (NULL + deepcopy)
-                      16 LOAD_FAST                0 (struct_in)
-                      18 PRECALL                  1
-                      22 CALL                     1
-                      32 STORE_FAST               4 (struct)
-         
-         260          34 LOAD_FAST                4 (struct)
-                      36 LOAD_METHOD              1 (items)
-                      58 PRECALL                  0
-                      62 CALL                     0
-                      72 GET_ITER
-                 >>   74 FOR_ITER                75 (to 226)
-                      76 UNPACK_SEQUENCE          2
-                      80 STORE_FAST               5 (_)
-                      82 STORE_FAST               6 (data)
+            0x97007401000000000000000000006a01000000000000000064016402a0
+            0200000000000000000000000000000000000000007c00a6010000ab0100
+            00000000000000a6020000ab0200000000000000007d0174070000000000
+            00000000007c01a6010000ab01000000000000000064037a0000007d027c
+            025300
+         224           0 RESUME                   0
+         
+         226           2 LOAD_GLOBAL              1 (NULL + re)
+                      14 LOAD_ATTR                1 (findall)
+         
+         227          24 LOAD_CONST               1 ('(?i)(if |else if|do |select case|select default)')
+                      26 LOAD_CONST               2 ('\n')
+                      28 LOAD_METHOD              2 (join)
+                      50 LOAD_FAST                0 (code)
+                      52 PRECALL                  1
+                      56 CALL                     1
+         
+         226          66 PRECALL                  2
+                      70 CALL                     2
+                      80 STORE_FAST               1 (decision_points)
+         
+         229          82 LOAD_GLOBAL              7 (NULL + len)
+                      94 LOAD_FAST                1 (decision_points)
+                      96 PRECALL                  1
+                     100 CALL                     1
+                     110 LOAD_CONST               3 (1)
+                     112 BINARY_OP                0 (+)
+                     116 STORE_FAST               2 (complexity)
          
-         261          84 LOAD_FAST                6 (data)
-                      86 LOAD_CONST               1 ('lines')
-                      88 BINARY_SUBSCR
-                      98 LOAD_CONST               2 (-1)
-                     100 BINARY_SUBSCR
-                     110 LOAD_FAST                6 (data)
-                     112 LOAD_CONST               1 ('lines')
-                     114 BINARY_SUBSCR
-                     124 LOAD_CONST               3 (0)
-                     126 BINARY_SUBSCR
-                     136 BINARY_OP               10 (-)
-                     140 LOAD_CONST               4 (1)
-                     142 BINARY_OP                0 (+)
-                     146 LOAD_FAST                6 (data)
-                     148 LOAD_CONST               5 ('NLOC')
-                     150 STORE_SUBSCR
-         
-         262         154 LOAD_FAST                6 (data)
-                     156 LOAD_CONST               6 ('statements')
-                     158 BINARY_SUBSCR
-                     168 LOAD_CONST               2 (-1)
-                     170 BINARY_SUBSCR
-                     180 LOAD_FAST                6 (data)
-                     182 LOAD_CONST               6 ('statements')
-                     184 BINARY_SUBSCR
-                     194 LOAD_CONST               3 (0)
-                     196 BINARY_SUBSCR
-                     206 BINARY_OP               10 (-)
-                     210 LOAD_CONST               4 (1)
-                     212 BINARY_OP                0 (+)
-                     216 LOAD_FAST                6 (data)
-                     218 LOAD_CONST               7 ('ssize')
-                     220 STORE_SUBSCR
-                     224 JUMP_BACKWARD           76 (to 74)
-         
-         265     >>  226 LOAD_FAST                4 (struct)
-                     228 LOAD_METHOD              1 (items)
-                     250 PRECALL                  0
-                     254 CALL                     0
-                     264 GET_ITER
-                 >>  266 FOR_ITER               167 (to 602)
-                     268 UNPACK_SEQUENCE          2
-                     272 STORE_FAST               7 (part)
-                     274 STORE_FAST               6 (data)
-         
-         266         276 LOAD_FAST                6 (data)
-                     278 LOAD_CONST               8 ('path')
-                     280 BINARY_SUBSCR
-                     290 STORE_FAST               8 (path)
-         
-         267         292 LOAD_GLOBAL              5 (NULL + len)
-                     304 LOAD_FAST                6 (data)
-                     306 LOAD_CONST               8 ('path')
-                     308 BINARY_SUBSCR
-                     318 PRECALL                  1
-                     322 CALL                     1
-                     332 LOAD_CONST               4 (1)
-                     334 COMPARE_OP               4 (>)
-                     340 POP_JUMP_FORWARD_IF_FALSE   118 (to 578)
-         
-         268         342 LOAD_FAST                6 (data)
-                     344 LOAD_CONST               8 ('path')
-                     346 BINARY_SUBSCR
-                     356 LOAD_CONST               9 (None)
-                     358 LOAD_CONST               2 (-1)
-                     360 BUILD_SLICE              2
-                     362 BINARY_SUBSCR
-                     372 STORE_FAST               9 (parent)
-         
-         269         374 NOP
-         
-         270         376 LOAD_FAST                4 (struct)
-                     378 LOAD_GLOBAL              7 (NULL + list2pathref)
-                     390 LOAD_FAST                9 (parent)
-                     392 PRECALL                  1
-                     396 CALL                     1
-                     406 BINARY_SUBSCR
-                     416 LOAD_CONST              10 ('contains')
-                     418 BINARY_SUBSCR
-                     428 LOAD_METHOD              4 (append)
-                     450 LOAD_GLOBAL              7 (NULL + list2pathref)
-                     462 LOAD_FAST                8 (path)
-                     464 PRECALL                  1
-                     468 CALL                     1
-                     478 PRECALL                  1
-                     482 CALL                     1
-                     492 POP_TOP
-                     494 JUMP_FORWARD            16 (to 528)
-                 >>  496 PUSH_EXC_INFO
-         
-         271         498 LOAD_GLOBAL             10 (KeyError)
-                     510 CHECK_EXC_MATCH
-                     512 POP_JUMP_FORWARD_IF_FALSE     3 (to 520)
-                     514 POP_TOP
-         
-         272         516 POP_EXCEPT
-                     518 JUMP_FORWARD             4 (to 528)
-         
-         271     >>  520 RERAISE                  0
-                 >>  522 COPY                     3
-                     524 POP_EXCEPT
-                     526 RERAISE                  1
-         
-         274     >>  528 LOAD_GLOBAL              7 (NULL + list2pathref)
-                     540 LOAD_FAST                9 (parent)
-                     542 PRECALL                  1
-                     546 CALL                     1
-                     556 LOAD_FAST                4 (struct)
-                     558 LOAD_FAST                7 (part)
-                     560 BINARY_SUBSCR
-                     570 LOAD_CONST              11 ('parent')
-                     572 STORE_SUBSCR
-                     576 JUMP_BACKWARD          156 (to 266)
-         
-         276     >>  578 LOAD_CONST               9 (None)
-                     580 LOAD_FAST                4 (struct)
-                     582 LOAD_FAST                7 (part)
-                     584 BINARY_SUBSCR
-                     594 LOAD_CONST              11 ('parent')
-                     596 STORE_SUBSCR
-                     600 JUMP_BACKWARD          168 (to 266)
-         
-         279     >>  602 LOAD_FAST                4 (struct)
-                     604 LOAD_METHOD              1 (items)
-                     626 PRECALL                  0
-                     630 CALL                     0
-                     640 GET_ITER
-                 >>  642 FOR_ITER               180 (to 1004)
-                     644 UNPACK_SEQUENCE          2
-                     648 STORE_FAST               7 (part)
-                     650 STORE_FAST               6 (data)
-         
-         280         652 LOAD_GLOBAL             13 (NULL + struct_actual_lines)
-                     664 LOAD_FAST                4 (struct)
-                     666 LOAD_FAST                7 (part)
-                     668 PRECALL                  2
-                     672 CALL                     2
-                     682 STORE_FAST              10 (actual_lines)
-         
-         281         684 LOAD_CLOSURE             1 (clean_code)
-                     686 BUILD_TUPLE              1
-                     688 LOAD_CONST              12 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py", line 281>)
-                     690 MAKE_FUNCTION            8 (closure)
-                     692 LOAD_FAST               10 (actual_lines)
-                     694 GET_ITER
-                     696 PRECALL                  0
-                     700 CALL                     0
-                     710 STORE_FAST              11 (sub_code)
-         
-         288         712 PUSH_NULL
-                     714 LOAD_FAST                2 (find_callables)
-                     716 LOAD_FAST               11 (sub_code)
-                     718 PRECALL                  1
-                     722 CALL                     1
-                     732 LOAD_FAST                6 (data)
-                     734 LOAD_CONST              13 ('callables')
-                     736 STORE_SUBSCR
-         
-         289         740 LOAD_FAST                4 (struct)
-                     742 LOAD_FAST                7 (part)
-                     744 BINARY_SUBSCR
-                     754 LOAD_CONST              11 ('parent')
-                     756 BINARY_SUBSCR
-                     766 POP_JUMP_FORWARD_IF_NONE    37 (to 842)
-         
-         290         768 LOAD_GLOBAL             15 (NULL + replace_self)
-                     780 LOAD_FAST                6 (data)
-                     782 LOAD_CONST              13 ('callables')
-                     784 BINARY_SUBSCR
-                     794 LOAD_FAST                4 (struct)
-                     796 LOAD_FAST                7 (part)
-                     798 BINARY_SUBSCR
-                     808 LOAD_CONST              11 ('parent')
-                     810 BINARY_SUBSCR
-                     820 PRECALL                  2
-                     824 CALL                     2
-                     834 LOAD_FAST                6 (data)
-                     836 LOAD_CONST              13 ('callables')
-                     838 STORE_SUBSCR
-         
-         291     >>  842 LOAD_FAST                4 (struct)
-                     844 LOAD_FAST                7 (part)
-                     846 BINARY_SUBSCR
-                     856 LOAD_CONST              14 ('type')
-                     858 BINARY_SUBSCR
-                     868 LOAD_CONST              15 (('class',))
-                     870 CONTAINS_OP              0
-                     872 POP_JUMP_FORWARD_IF_FALSE    50 (to 974)
-         
-         292         874 LOAD_GLOBAL             15 (NULL + replace_self)
-                     886 LOAD_FAST                6 (data)
-                     888 LOAD_CONST              10 ('contains')
-                     890 BINARY_SUBSCR
-                     900 LOAD_FAST                7 (part)
-                     902 PRECALL                  2
-                     906 CALL                     2
-                     916 LOAD_FAST                6 (data)
-                     918 LOAD_CONST              10 ('contains')
-                     920 STORE_SUBSCR
-         
-         293         924 LOAD_GLOBAL             15 (NULL + replace_self)
-                     936 LOAD_FAST                6 (data)
-                     938 LOAD_CONST              13 ('callables')
-                     940 BINARY_SUBSCR
-                     950 LOAD_FAST                7 (part)
-                     952 PRECALL                  2
-                     956 CALL                     2
-                     966 LOAD_FAST                6 (data)
-                     968 LOAD_CONST              13 ('callables')
-                     970 STORE_SUBSCR
-         
-         295     >>  974 PUSH_NULL
-                     976 LOAD_FAST                3 (compute_ccn)
-                     978 LOAD_FAST               11 (sub_code)
-                     980 PRECALL                  1
-                     984 CALL                     1
-                     994 LOAD_FAST                6 (data)
-                     996 LOAD_CONST              16 ('CCN')
-                     998 STORE_SUBSCR
-                    1002 JUMP_BACKWARD          181 (to 642)
-         
-         297     >> 1004 LOAD_FAST                4 (struct)
-                    1006 RETURN_VALUE
-         ExceptionTable:
-           376 to 492 -> 496 [1]
-           496 to 514 -> 522 [2] lasti
-           520 to 520 -> 522 [2] lasti
+         230         118 LOAD_FAST                2 (complexity)
+                     120 RETURN_VALUE
          consts
-            'Complete the description of each struct item'
-            'lines'
-            -1
-            0
+            'Count decision points (if, else if, do, select, etc.)'
+            '(?i)(if |else if|do |select case|select default)'
+            '\n'
             1
-            'NLOC'
-            'statements'
-            'ssize'
-            'path'
-            None
-            'contains'
-            'parent'
-            code
-               argcount  : 1
-               nlocals   : 2
-               stacksize : 4
-               flags     : 19
-               code
-                  0x9501970067007c005d0a7d0189027c011900000000000000000091028c
-                  0b5300
-                             0 COPY_FREE_VARS           1
-               
-               281           2 RESUME                   0
-                             4 BUILD_LIST               0
-                             6 LOAD_FAST                0 (.0)
-                       >>    8 FOR_ITER                10 (to 30)
-                            10 STORE_FAST               1 (i)
-                            12 LOAD_DEREF               2 (clean_code)
-                            14 LOAD_FAST                1 (i)
-                            16 BINARY_SUBSCR
-                            26 LIST_APPEND              2
-                            28 JUMP_BACKWARD           11 (to 8)
-                       >>   30 RETURN_VALUE
-               consts
-               names      ()
-               varnames   ('.0', 'i')
-               freevars   ('clean_code',)
-               cellvars   ()
-               filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-               name       '<listcomp>'
-               firstlineno 281
-               lnotab 0x
-            'callables'
-            'type'
-            ('class',)
-            'CCN'
-         names      ('deepcopy', 'items', 'len', 'list2pathref', 'append', 'KeyError', 'struct_actual_lines', 'replace_self')
-         varnames   ('struct_in', 'clean_code', 'find_callables', 'compute_ccn', 'struct', '_', 'data', 'part', 'path', 'parent', 'actual_lines', 'sub_code')
+         names      ('re', 'findall', 'join', 'len')
+         varnames   ('code', 'decision_points', 'complexity')
          freevars   ()
-         cellvars   ('clean_code',)
-         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
-         name       'struct_augment'
-         firstlineno 256
-         lnotab
-            0x04021e02320146014803320110013201200102017a01120104ff080332
-            021803320120011c071c011c014a012001320132021e02
-      (None,)
-   names      ('__doc__', 're', 'typing', 'Tuple', 'List', 'Callable', 'copy', 'deepcopy', 'loguru', 'logger', 'list', 'path_clean', 'str', 'list2pathref', 'pathref_ascendants', 'dict', 'struct_summary_str', 'find_words_before_left_parenthesis', 'int', 'buffer_item', 'stack_item', 'struct_from_stack', 'get_struct_sizes', 'replace_self', '_strip_safe_lines', 'struct_actual_lines', 'struct_augment')
+         cellvars   ()
+         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py'
+         name       'compute_ccn_approx_ftn'
+         firstlineno 224
+         lnotab 0x020216012aff10032401
+      (False,)
+   names      ('re', 'loguru', 'logger', 'tucan.unformat_common', 'Statements', 'tucan.struct_common', 'find_words_before_left_parenthesis', 'new_buffer_item', 'new_stack_item', 'struct_from_stack', 'struct_augment', 'rm_parenthesis_content', 'tucan.kw_lang', 'STRUCTURES_FTN', 'NESTS_FTN', 'OTHERS_FTN', 'sorted', 'PARTS', 'NESTS', 'INTRINSICS', 'dict', 'extract_struct_ftn', '_extract_on_cleaned_ftn', 'str', 'int', '_parse_name_ftn', 'list', 'find_callables_ftn', 'compute_ccn_approx_ftn')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_common.py'
+   filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_ftn.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010404080114010c010c021c0d10051c0a10211c1f020102ff02
-      0202fe020302fd020402fc020502fb020618fa0815020102ff020202fe02
-      0302fd020402fc020502fb020602fa020702f9020802f8020902f7020a20
-      f608201a2a100d14082418140e
+      0x00ff020108010c010c011c070c0414031a011a010403100f127f000b10
+      22100e
```

### Comparing `tucan-0.1.0/src/tucan/__pycache__/struct_main.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/struct_main.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0x27c99465 (Wed Jan  3 02:40:39 2024 UTC)
-files sz: 2407
+moddate:  0x93114266 (Mon May 13 13:11:47 2024 UTC)
+files sz: 2668
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 4
+   stacksize : 7
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a0401
       00640164046c056d065a060100640164056c076d085a080100640164066c
       096d0a5a0a0100640164076c0b6d0c5a0c0100640164086c0d6d0e5a0e01
-      006409650f640a65106604640b84045a116409650f640a65106604640c84
-      045a12640d5300
+      00640164096c0f6d105a1001006411640b6511640c6512640d6513660664
+      0e84055a14640b6511640d65136604640f84045a1564105300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('Global function to handle the struct analysis of various languages')
                  4 STORE_NAME               0 (__doc__)
    
      2           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('logger',))
@@ -62,115 +62,131 @@
      9          78 LOAD_CONST               1 (0)
                 80 LOAD_CONST               8 (('extract_struct_c',))
                 82 IMPORT_NAME             13 (tucan.struct_c)
                 84 IMPORT_FROM             14 (extract_struct_c)
                 86 STORE_NAME              14 (extract_struct_c)
                 88 POP_TOP
    
-    12          90 LOAD_CONST               9 ('filename')
-                92 LOAD_NAME               15 (str)
-                94 LOAD_CONST              10 ('return')
-                96 LOAD_NAME               16 (dict)
-                98 BUILD_TUPLE              4
-               100 LOAD_CONST              11 (<code object struct_main, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_main.py", line 12>)
-               102 MAKE_FUNCTION            4 (annotations)
-               104 STORE_NAME              17 (struct_main)
-   
-    55         106 LOAD_CONST               9 ('filename')
-               108 LOAD_NAME               15 (str)
-               110 LOAD_CONST              10 ('return')
-               112 LOAD_NAME               16 (dict)
-               114 BUILD_TUPLE              4
-               116 LOAD_CONST              12 (<code object create_empty_struct, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_main.py", line 55>)
-               118 MAKE_FUNCTION            4 (annotations)
-               120 STORE_NAME              18 (create_empty_struct)
-               122 LOAD_CONST              13 (None)
-               124 RETURN_VALUE
+    10          90 LOAD_CONST               1 (0)
+                92 LOAD_CONST               9 (('remove_ifdef_from_module',))
+                94 IMPORT_NAME             15 (tucan.clean_ifdef)
+                96 IMPORT_FROM             16 (remove_ifdef_from_module)
+                98 STORE_NAME              16 (remove_ifdef_from_module)
+               100 POP_TOP
+   
+    13         102 LOAD_CONST              17 ((False,))
+               104 LOAD_CONST              11 ('filename')
+               106 LOAD_NAME               17 (str)
+               108 LOAD_CONST              12 ('verbose')
+               110 LOAD_NAME               18 (bool)
+               112 LOAD_CONST              13 ('return')
+               114 LOAD_NAME               19 (dict)
+               116 BUILD_TUPLE              6
+               118 LOAD_CONST              14 (<code object struct_main, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_main.py", line 13>)
+               120 MAKE_FUNCTION            5 (defaults, annotations)
+               122 STORE_NAME              20 (struct_main)
+   
+    58         124 LOAD_CONST              11 ('filename')
+               126 LOAD_NAME               17 (str)
+               128 LOAD_CONST              13 ('return')
+               130 LOAD_NAME               19 (dict)
+               132 BUILD_TUPLE              4
+               134 LOAD_CONST              15 (<code object create_empty_struct, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_main.py", line 58>)
+               136 MAKE_FUNCTION            4 (annotations)
+               138 STORE_NAME              21 (create_empty_struct)
+               140 LOAD_CONST              16 (None)
+               142 RETURN_VALUE
    consts
       'Global function to handle the struct analysis of various languages'
       0
       ('logger',)
       ('unformat_py',)
       ('unformat_ftn',)
       ('unformat_c',)
       ('extract_struct_py',)
       ('extract_struct_ftn',)
       ('extract_struct_c',)
+      ('remove_ifdef_from_module',)
+      False
       'filename'
+      'verbose'
       'return'
       code
-         argcount  : 1
-         nlocals   : 6
+         argcount  : 2
+         nlocals   : 7
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a01000000000000000064017c009b
             009d02a6010000ab01000000000000000001000900740500000000000000
-            0000007c006402a6020000ab02000000000000000035007d017c01a00300
+            0000007c006402a6020000ab02000000000000000035007d027c02a00300
             00000000000000000000000000000000000000a6000000ab000000000000
             000000a0040000000000000000000000000000000000000000a6000000ab
-            0000000000000000007d02640364036403a6020000ab0200000000000000
+            0000000000000000007d03640364036403a6020000ab0200000000000000
             0001006e0b230031007304770278035900770101005900010001006e1223
             00740a000000000000000000002400720501006900630259005300770078
-            0359007701640484007c024400a6000000ab0000000000000000007d027c
+            0359007701640484007c034400a6000000ab0000000000000000007d037c
             00a0060000000000000000000000000000000000000000a6000000ab0000
             00000000000000a007000000000000000000000000000000000000000064
-            05a6010000ab01000000000000000072337401000000000000000000006a
+            05a6010000ab01000000000000000072357401000000000000000000006a
             0800000000000000006406a6010000ab0100000000000000000100741300
-            0000000000000000007c02a6010000ab0100000000000000007d03741500
-            0000000000000000007c03a6010000ab0100000000000000007d046efb7c
-            00a0060000000000000000000000000000000000000000a6000000ab0000
-            00000000000000a007000000000000000000000000000000000000000064
-            07a6010000ab01000000000000000072337401000000000000000000006a
-            0800000000000000006408a6010000ab0100000000000000000100741700
-            0000000000000000007c02a6010000ab0100000000000000007d03741900
-            0000000000000000007c03a6010000ab0100000000000000007d046ea17c
-            00a0060000000000000000000000000000000000000000a6000000ab0000
-            00000000000000a007000000000000000000000000000000000000000064
-            09a6010000ab01000000000000000072337401000000000000000000006a
-            080000000000000000640aa6010000ab0100000000000000000100741b00
-            0000000000000000007c02a6010000ab0100000000000000007d03741d00
-            0000000000000000007c03a6010000ab0100000000000000007d046e477c
-            00a0060000000000000000000000000000000000000000a6000000ab0000
-            00000000000000a00f000000000000000000000000000000000000000064
-            0ba6010000ab010000000000000000640c190000000000000000007d0574
-            01000000000000000000006a100000000000000000640d7c059b00640e9d
-            03a6010000ab0100000000000000000100690053007c045300
-          12           0 RESUME                   0
+            0000000000000000007c03a6010000ab0100000000000000007d04741500
+            0000000000000000007c047c01a6020000ab0200000000000000007d0590
+            016e227c00a0060000000000000000000000000000000000000000a60000
+            00ab000000000000000000a0070000000000000000000000000000000000
+            0000006407a6010000ab0100000000000000007247740100000000000000
+            0000006a0800000000000000006408a6010000ab01000000000000000001
+            007417000000000000000000007c0367006409640aac0ba6040000ab0400
+            000000000000007d037419000000000000000000007c03a6010000ab0100
+            000000000000007d04741b000000000000000000007c047c01a6020000ab
+            0200000000000000007d056eb47c00a00600000000000000000000000000
+            00000000000000a6000000ab000000000000000000a00700000000000000
+            00000000000000000000000000640ca6010000ab01000000000000000072
+            467401000000000000000000006a080000000000000000640da6010000ab
+            01000000000000000001007417000000000000000000007c0367006409ac
+            0ea6030000ab0300000000000000007d03741d000000000000000000007c
+            03a6010000ab0100000000000000007d04741f000000000000000000007c
+            047c01a6020000ab0200000000000000007d056e477c00a0060000000000
+            000000000000000000000000000000a6000000ab000000000000000000a0
+            100000000000000000000000000000000000000000640fa6010000ab0100
+            000000000000006410190000000000000000007d06740100000000000000
+            0000006a11000000000000000064117c069b0064129d03a6010000ab0100
+            000000000000000100690053007c055300
+          13           0 RESUME                   0
          
-          26           2 LOAD_GLOBAL              1 (NULL + logger)
+          27           2 LOAD_GLOBAL              1 (NULL + logger)
                       14 LOAD_ATTR                1 (info)
                       24 LOAD_CONST               1 ('Struct analysis on ')
                       26 LOAD_FAST                0 (filename)
                       28 FORMAT_VALUE             0
                       30 BUILD_STRING             2
                       32 PRECALL                  1
                       36 CALL                     1
                       46 POP_TOP
          
-          27          48 NOP
+          28          48 NOP
          
-          28          50 LOAD_GLOBAL              5 (NULL + open)
+          29          50 LOAD_GLOBAL              5 (NULL + open)
                       62 LOAD_FAST                0 (filename)
                       64 LOAD_CONST               2 ('r')
                       66 PRECALL                  2
                       70 CALL                     2
                       80 BEFORE_WITH
-                      82 STORE_FAST               1 (fin)
+                      82 STORE_FAST               2 (fin)
          
-          29          84 LOAD_FAST                1 (fin)
+          30          84 LOAD_FAST                2 (fin)
                       86 LOAD_METHOD              3 (read)
                      108 PRECALL                  0
                      112 CALL                     0
                      122 LOAD_METHOD              4 (splitlines)
                      144 PRECALL                  0
                      148 CALL                     0
-                     158 STORE_FAST               2 (code)
+                     158 STORE_FAST               3 (code)
          
-          28         160 LOAD_CONST               3 (None)
+          29         160 LOAD_CONST               3 (None)
                      162 LOAD_CONST               3 (None)
                      164 LOAD_CONST               3 (None)
                      166 PRECALL                  2
                      170 CALL                     2
                      180 POP_TOP
                      182 JUMP_FORWARD            11 (to 206)
                  >>  184 PUSH_EXC_INFO
@@ -183,155 +199,178 @@
                  >>  198 POP_TOP
                      200 POP_EXCEPT
                      202 POP_TOP
                      204 POP_TOP
                  >>  206 JUMP_FORWARD            18 (to 244)
                  >>  208 PUSH_EXC_INFO
          
-          30         210 LOAD_GLOBAL             10 (UnicodeDecodeError)
+          31         210 LOAD_GLOBAL             10 (UnicodeDecodeError)
                      222 CHECK_EXC_MATCH
                      224 POP_JUMP_FORWARD_IF_FALSE     5 (to 236)
                      226 POP_TOP
          
-          31         228 BUILD_MAP                0
+          32         228 BUILD_MAP                0
                      230 SWAP                     2
                      232 POP_EXCEPT
                      234 RETURN_VALUE
          
-          30     >>  236 RERAISE                  0
+          31     >>  236 RERAISE                  0
                  >>  238 COPY                     3
                      240 POP_EXCEPT
                      242 RERAISE                  1
          
-          33     >>  244 LOAD_CONST               4 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_main.py", line 33>)
+          34     >>  244 LOAD_CONST               4 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/struct_main.py", line 34>)
                      246 MAKE_FUNCTION            0
-                     248 LOAD_FAST                2 (code)
+                     248 LOAD_FAST                3 (code)
                      250 GET_ITER
                      252 PRECALL                  0
                      256 CALL                     0
-                     266 STORE_FAST               2 (code)
+                     266 STORE_FAST               3 (code)
          
-          35         268 LOAD_FAST                0 (filename)
+          36         268 LOAD_FAST                0 (filename)
                      270 LOAD_METHOD              6 (lower)
                      292 PRECALL                  0
                      296 CALL                     0
                      306 LOAD_METHOD              7 (endswith)
                      328 LOAD_CONST               5 ('.py')
                      330 PRECALL                  1
                      334 CALL                     1
-                     344 POP_JUMP_FORWARD_IF_FALSE    51 (to 448)
+                     344 POP_JUMP_FORWARD_IF_FALSE    53 (to 452)
          
-          36         346 LOAD_GLOBAL              1 (NULL + logger)
+          37         346 LOAD_GLOBAL              1 (NULL + logger)
                      358 LOAD_ATTR                8 (debug)
                      368 LOAD_CONST               6 ('Python code detected ...')
                      370 PRECALL                  1
                      374 CALL                     1
                      384 POP_TOP
          
-          37         386 LOAD_GLOBAL             19 (NULL + unformat_py)
-                     398 LOAD_FAST                2 (code)
+          38         386 LOAD_GLOBAL             19 (NULL + unformat_py)
+                     398 LOAD_FAST                3 (code)
                      400 PRECALL                  1
                      404 CALL                     1
-                     414 STORE_FAST               3 (statements)
+                     414 STORE_FAST               4 (statements)
          
-          38         416 LOAD_GLOBAL             21 (NULL + extract_struct_py)
-                     428 LOAD_FAST                3 (statements)
-                     430 PRECALL                  1
-                     434 CALL                     1
-                     444 STORE_FAST               4 (struct_)
-                     446 JUMP_FORWARD           251 (to 950)
-         
-          39     >>  448 LOAD_FAST                0 (filename)
-                     450 LOAD_METHOD              6 (lower)
-                     472 PRECALL                  0
-                     476 CALL                     0
-                     486 LOAD_METHOD              7 (endswith)
-                     508 LOAD_CONST               7 (('.f', '.F', '.f77', '.f90'))
-                     510 PRECALL                  1
-                     514 CALL                     1
-                     524 POP_JUMP_FORWARD_IF_FALSE    51 (to 628)
-         
-          40         526 LOAD_GLOBAL              1 (NULL + logger)
-                     538 LOAD_ATTR                8 (debug)
-                     548 LOAD_CONST               8 ('Fortran code detected ...')
-                     550 PRECALL                  1
-                     554 CALL                     1
-                     564 POP_TOP
-         
-          41         566 LOAD_GLOBAL             23 (NULL + unformat_ftn)
-                     578 LOAD_FAST                2 (code)
-                     580 PRECALL                  1
-                     584 CALL                     1
-                     594 STORE_FAST               3 (statements)
-         
-          42         596 LOAD_GLOBAL             25 (NULL + extract_struct_ftn)
-                     608 LOAD_FAST                3 (statements)
-                     610 PRECALL                  1
-                     614 CALL                     1
-                     624 STORE_FAST               4 (struct_)
-                     626 JUMP_FORWARD           161 (to 950)
-         
-          43     >>  628 LOAD_FAST                0 (filename)
-                     630 LOAD_METHOD              6 (lower)
-                     652 PRECALL                  0
-                     656 CALL                     0
-                     666 LOAD_METHOD              7 (endswith)
-                     688 LOAD_CONST               9 (('.c', '.cpp', '.cc'))
-                     690 PRECALL                  1
-                     694 CALL                     1
-                     704 POP_JUMP_FORWARD_IF_FALSE    51 (to 808)
-         
-          44         706 LOAD_GLOBAL              1 (NULL + logger)
-                     718 LOAD_ATTR                8 (debug)
-                     728 LOAD_CONST              10 ('C/C++ code detected ...')
-                     730 PRECALL                  1
-                     734 CALL                     1
-                     744 POP_TOP
-         
-          45         746 LOAD_GLOBAL             27 (NULL + unformat_c)
-                     758 LOAD_FAST                2 (code)
-                     760 PRECALL                  1
-                     764 CALL                     1
-                     774 STORE_FAST               3 (statements)
-         
-          46         776 LOAD_GLOBAL             29 (NULL + extract_struct_c)
-                     788 LOAD_FAST                3 (statements)
-                     790 PRECALL                  1
-                     794 CALL                     1
-                     804 STORE_FAST               4 (struct_)
-                     806 JUMP_FORWARD            71 (to 950)
-         
-          48     >>  808 LOAD_FAST                0 (filename)
-                     810 LOAD_METHOD              6 (lower)
-                     832 PRECALL                  0
-                     836 CALL                     0
-                     846 LOAD_METHOD             15 (split)
-                     868 LOAD_CONST              11 ('.')
-                     870 PRECALL                  1
-                     874 CALL                     1
-                     884 LOAD_CONST              12 (-1)
-                     886 BINARY_SUBSCR
-                     896 STORE_FAST               5 (ext)
-         
-          49         898 LOAD_GLOBAL              1 (NULL + logger)
-                     910 LOAD_ATTR               16 (error)
-                     920 LOAD_CONST              13 ('Extension ')
-                     922 LOAD_FAST                5 (ext)
-                     924 FORMAT_VALUE             0
-                     926 LOAD_CONST              14 (' not supported, exiting ...')
-                     928 BUILD_STRING             3
-                     930 PRECALL                  1
-                     934 CALL                     1
-                     944 POP_TOP
+          39         416 LOAD_GLOBAL             21 (NULL + extract_struct_py)
+                     428 LOAD_FAST                4 (statements)
+                     430 LOAD_FAST                1 (verbose)
+                     432 PRECALL                  2
+                     436 CALL                     2
+                     446 STORE_FAST               5 (struct_)
+                     448 EXTENDED_ARG             1
+                     450 JUMP_FORWARD           290 (to 1032)
+         
+          40     >>  452 LOAD_FAST                0 (filename)
+                     454 LOAD_METHOD              6 (lower)
+                     476 PRECALL                  0
+                     480 CALL                     0
+                     490 LOAD_METHOD              7 (endswith)
+                     512 LOAD_CONST               7 (('.f', '.F', '.f77', '.f90'))
+                     514 PRECALL                  1
+                     518 CALL                     1
+                     528 POP_JUMP_FORWARD_IF_FALSE    71 (to 672)
+         
+          41         530 LOAD_GLOBAL              1 (NULL + logger)
+                     542 LOAD_ATTR                8 (debug)
+                     552 LOAD_CONST               8 ('Fortran code detected ...')
+                     554 PRECALL                  1
+                     558 CALL                     1
+                     568 POP_TOP
+         
+          42         570 LOAD_GLOBAL             23 (NULL + remove_ifdef_from_module)
+                     582 LOAD_FAST                3 (code)
+                     584 BUILD_LIST               0
+                     586 LOAD_CONST               9 (False)
+                     588 LOAD_CONST              10 (True)
+                     590 KW_NAMES                11
+                     592 PRECALL                  4
+                     596 CALL                     4
+                     606 STORE_FAST               3 (code)
+         
+          43         608 LOAD_GLOBAL             25 (NULL + unformat_ftn)
+                     620 LOAD_FAST                3 (code)
+                     622 PRECALL                  1
+                     626 CALL                     1
+                     636 STORE_FAST               4 (statements)
+         
+          44         638 LOAD_GLOBAL             27 (NULL + extract_struct_ftn)
+                     650 LOAD_FAST                4 (statements)
+                     652 LOAD_FAST                1 (verbose)
+                     654 PRECALL                  2
+                     658 CALL                     2
+                     668 STORE_FAST               5 (struct_)
+                     670 JUMP_FORWARD           180 (to 1032)
+         
+          45     >>  672 LOAD_FAST                0 (filename)
+                     674 LOAD_METHOD              6 (lower)
+                     696 PRECALL                  0
+                     700 CALL                     0
+                     710 LOAD_METHOD              7 (endswith)
+                     732 LOAD_CONST              12 (('.c', '.cpp', '.cc', '.h', '.hpp'))
+                     734 PRECALL                  1
+                     738 CALL                     1
+                     748 POP_JUMP_FORWARD_IF_FALSE    70 (to 890)
+         
+          46         750 LOAD_GLOBAL              1 (NULL + logger)
+                     762 LOAD_ATTR                8 (debug)
+                     772 LOAD_CONST              13 ('C/C++ code detected ...')
+                     774 PRECALL                  1
+                     778 CALL                     1
+                     788 POP_TOP
+         
+          47         790 LOAD_GLOBAL             23 (NULL + remove_ifdef_from_module)
+                     802 LOAD_FAST                3 (code)
+                     804 BUILD_LIST               0
+                     806 LOAD_CONST               9 (False)
+                     808 KW_NAMES                14
+                     810 PRECALL                  3
+                     814 CALL                     3
+                     824 STORE_FAST               3 (code)
+         
+          48         826 LOAD_GLOBAL             29 (NULL + unformat_c)
+                     838 LOAD_FAST                3 (code)
+                     840 PRECALL                  1
+                     844 CALL                     1
+                     854 STORE_FAST               4 (statements)
+         
+          49         856 LOAD_GLOBAL             31 (NULL + extract_struct_c)
+                     868 LOAD_FAST                4 (statements)
+                     870 LOAD_FAST                1 (verbose)
+                     872 PRECALL                  2
+                     876 CALL                     2
+                     886 STORE_FAST               5 (struct_)
+                     888 JUMP_FORWARD            71 (to 1032)
+         
+          51     >>  890 LOAD_FAST                0 (filename)
+                     892 LOAD_METHOD              6 (lower)
+                     914 PRECALL                  0
+                     918 CALL                     0
+                     928 LOAD_METHOD             16 (split)
+                     950 LOAD_CONST              15 ('.')
+                     952 PRECALL                  1
+                     956 CALL                     1
+                     966 LOAD_CONST              16 (-1)
+                     968 BINARY_SUBSCR
+                     978 STORE_FAST               6 (ext)
+         
+          52         980 LOAD_GLOBAL              1 (NULL + logger)
+                     992 LOAD_ATTR               17 (error)
+                    1002 LOAD_CONST              17 ('Extension ')
+                    1004 LOAD_FAST                6 (ext)
+                    1006 FORMAT_VALUE             0
+                    1008 LOAD_CONST              18 (' not supported, exiting ...')
+                    1010 BUILD_STRING             3
+                    1012 PRECALL                  1
+                    1016 CALL                     1
+                    1026 POP_TOP
          
-          50         946 BUILD_MAP                0
-                     948 RETURN_VALUE
+          53        1028 BUILD_MAP                0
+                    1030 RETURN_VALUE
          
-          52     >>  950 LOAD_FAST                4 (struct_)
-                     952 RETURN_VALUE
+          55     >> 1032 LOAD_FAST                5 (struct_)
+                    1034 RETURN_VALUE
          ExceptionTable:
            50 to 80 -> 208 [0]
            82 to 158 -> 184 [1] lasti
            160 to 182 -> 208 [0]
            184 to 190 -> 192 [3] lasti
            192 to 196 -> 208 [0]
            198 to 198 -> 192 [3] lasti
@@ -347,15 +386,15 @@
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 19
                code
                   0x970067007c005d167d017c01a000000000000000000000000000000000
                   0000000000a6000000ab00000000000000000091028c175300
-                33           0 RESUME                   0
+                34           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                22 (to 52)
                              8 STORE_FAST               1 (line)
                             10 LOAD_FAST                1 (line)
                             12 LOAD_METHOD              0 (lower)
                             34 PRECALL                  0
@@ -366,99 +405,104 @@
                consts
                names      ('lower',)
                varnames   ('.0', 'line')
                freevars   ()
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_main.py'
                name       '<listcomp>'
-               firstlineno 33
+               firstlineno 34
                lnotab 0x
             '.py'
             'Python code detected ...'
             ('.f', '.F', '.f77', '.f90')
             'Fortran code detected ...'
-            ('.c', '.cpp', '.cc')
+            False
+            True
+            ('verbose', 'fortran')
+            ('.c', '.cpp', '.cc', '.h', '.hpp')
             'C/C++ code detected ...'
+            ('verbose',)
             '.'
             -1
             'Extension '
             ' not supported, exiting ...'
-         names      ('logger', 'info', 'open', 'read', 'splitlines', 'UnicodeDecodeError', 'lower', 'endswith', 'debug', 'unformat_py', 'extract_struct_py', 'unformat_ftn', 'extract_struct_ftn', 'unformat_c', 'extract_struct_c', 'split', 'error')
-         varnames   ('filename', 'fin', 'code', 'statements', 'struct_', 'ext')
+         names      ('logger', 'info', 'open', 'read', 'splitlines', 'UnicodeDecodeError', 'lower', 'endswith', 'debug', 'unformat_py', 'extract_struct_py', 'remove_ifdef_from_module', 'unformat_ftn', 'extract_struct_ftn', 'unformat_c', 'extract_struct_c', 'split', 'error')
+         varnames   ('filename', 'verbose', 'fin', 'code', 'statements', 'struct_', 'ext')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_main.py'
          name       'struct_main'
-         firstlineno 12
+         firstlineno 13
          lnotab
-            0x020e2e01020122014cff3202120108ff080318024e0128011e0120014e
-            0128011e0120014e0128011e0120025a0130010402
+            0x020e2e01020122014cff3202120108ff080318024e0128011e0124014e
+            01280126011e0122014e01280124011e0122025a0130010402
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 13
          flags     : 3
          code
             0x97007c00640164016700670064026402670264037c007c006701640267
             00640364049c0b69017d017c015300
-          55           0 RESUME                   0
+          58           0 RESUME                   0
          
-          66           2 LOAD_FAST                0 (filename)
+          69           2 LOAD_FAST                0 (filename)
          
-          67           4 LOAD_CONST               1 (1)
+          70           4 LOAD_CONST               1 (1)
          
-          68           6 LOAD_CONST               1 (1)
+          71           6 LOAD_CONST               1 (1)
          
-          69           8 BUILD_LIST               0
+          72           8 BUILD_LIST               0
          
-          70          10 BUILD_LIST               0
+          73          10 BUILD_LIST               0
          
-          71          12 LOAD_CONST               2 (0)
+          74          12 LOAD_CONST               2 (0)
                       14 LOAD_CONST               2 (0)
                       16 BUILD_LIST               2
          
-          72          18 LOAD_CONST               3 (None)
+          75          18 LOAD_CONST               3 (None)
          
-          73          20 LOAD_FAST                0 (filename)
+          76          20 LOAD_FAST                0 (filename)
          
-          74          22 LOAD_FAST                0 (filename)
+          77          22 LOAD_FAST                0 (filename)
                       24 BUILD_LIST               1
          
-          75          26 LOAD_CONST               2 (0)
+          78          26 LOAD_CONST               2 (0)
          
-          76          28 BUILD_LIST               0
+          79          28 BUILD_LIST               0
          
-          77          30 LOAD_CONST               3 (None)
+          80          30 LOAD_CONST               3 (None)
          
-          66          32 LOAD_CONST               4 (('CCN', 'NLOC', 'callables', 'contains', 'lines', 'linestart', 'name', 'path', 'ssize', 'statements', 'type'))
+          69          32 LOAD_CONST               4 (('CCN', 'NLOC', 'callables', 'contains', 'lines', 'linestart', 'name', 'path', 'ssize', 'statements', 'type'))
                       34 BUILD_CONST_KEY_MAP     11
          
-          65          36 BUILD_MAP                1
+          68          36 BUILD_MAP                1
                       38 STORE_FAST               1 (struct_)
          
-          80          40 LOAD_FAST                1 (struct_)
+          83          40 LOAD_FAST                1 (struct_)
                       42 RETURN_VALUE
          consts
             '\n    Function to create an empty structure output.\n\n    Args:\n        filename (str): Name of the file (with its path) to parse.\n\n    Returns:\n        dict: Empty structure dict i.e. with defaults values.\n    '
             1
             0
             None
             ('CCN', 'NLOC', 'callables', 'contains', 'lines', 'linestart', 'name', 'path', 'ssize', 'statements', 'type')
          names      ()
          varnames   ('filename', 'struct_')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_main.py'
          name       'create_empty_struct'
-         firstlineno 55
+         firstlineno 58
          lnotab
             0x020b0201020102010201020106010201020104010201020102f504ff04
             0f
       None
-   names      ('__doc__', 'loguru', 'logger', 'tucan.unformat_py', 'unformat_py', 'tucan.unformat_ftn', 'unformat_ftn', 'tucan.unformat_c', 'unformat_c', 'tucan.struct_py', 'extract_struct_py', 'tucan.struct_ftn', 'extract_struct_ftn', 'tucan.struct_c', 'extract_struct_c', 'str', 'dict', 'struct_main', 'create_empty_struct')
+      (False,)
+   names      ('__doc__', 'loguru', 'logger', 'tucan.unformat_py', 'unformat_py', 'tucan.unformat_ftn', 'unformat_ftn', 'tucan.unformat_c', 'unformat_c', 'tucan.struct_py', 'extract_struct_py', 'tucan.struct_ftn', 'extract_struct_ftn', 'tucan.struct_c', 'extract_struct_c', 'tucan.clean_ifdef', 'remove_ifdef_from_module', 'str', 'bool', 'dict', 'struct_main', 'create_empty_struct')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/dauptain/GITLAB/tucan/src/tucan/struct_main.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104010c020c010c010c010c010c010c03102b
+   lnotab 0x00ff020104010c020c010c010c010c010c010c010c03162d
```

### Comparing `tucan-0.1.0/src/tucan/__pycache__/unformat_c.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/unformat_c.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x6cc7b765 (Mon Jan 29 15:42:36 2024 UTC)
-files sz: 4962
+moddate:  0xc922c665 (Fri Feb  9 13:04:09 2024 UTC)
+files sz: 4964
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -283,36 +283,35 @@
          argcount  : 1
          nlocals   : 10
          stacksize : 5
          flags     : 3
          code
             0x970067007d0167007d0264017d0364027d047401000000000000000000
             007c006a0100000000000000007c006a020000000000000000a6020000ab
-            02000000000000000044005df65c0200007d055c0200007d067d077c0544
+            02000000000000000044005df05c0200007d055c0200007d067d077c0544
             005d187d087c0864036b020000000072057c0464047a0d00007d047c0864
             056b020000000072057c0464047a1700007d048c197c05a0030000000000
             0000000000000000000000000000006406a6010000ab0100000000000000
             00722d7c01a00400000000000000000000000000000000000000007c05a6
             010000ab01000000000000000001007c02a0040000000000000000000000
             0000000000000000007c067c076702a6010000ab01000000000000000001
             008c657c0380177c05a00500000000000000000000000000000000000000
             00a6000000ab0000000000000000007d037c067d096e1a7c0364077c05a0
             060000000000000000000000000000000000000000a6000000ab00000000
             00000000007a0000007a0d00007d037c03a0070000000000000000000000
-            0000000000000000006408a6010000ab010000000000000000731b7c03a0
+            0000000000000000006408a6010000ab01000000000000000073157c03a0
             0700000000000000000000000000000000000000006405a6010000ab0100
-            0000000000000072347c0464026b0200000000722e7c01a0040000000000
-            0000000000000000000000000000007c03a6010000ab0100000000000000
-            0001007c02a00400000000000000000000000000000000000000007c097c
-            076702a6010000ab010000000000000000010064017d038cf77c03812f7c
-            03a0060000000000000000000000000000000000000000a6000000ab0000
-            0000000000000064096b030000000072177411000000000000000000006a
-            090000000000000000640a7c039b009d02a6010000ab0100000000000000
-            0001007415000000000000000000007c017c02a6020000ab020000000000
-            0000005300
+            00000000000000722e7c01a0040000000000000000000000000000000000
+            0000007c03a6010000ab01000000000000000001007c02a0040000000000
+            0000000000000000000000000000007c097c076702a6010000ab01000000
+            0000000000010064017d038cf17c03812f7c03a006000000000000000000
+            0000000000000000000000a6000000ab00000000000000000064096b0300
+            00000072177411000000000000000000006a090000000000000000640a7c
+            039b009d02a6010000ab0100000000000000000100741500000000000000
+            0000007c017c02a6020000ab0200000000000000005300
           51           0 RESUME                   0
          
           53           2 BUILD_LIST               0
                        4 STORE_FAST               1 (new_stmt)
          
           54           6 BUILD_LIST               0
                        8 STORE_FAST               2 (new_lines)
@@ -327,15 +326,15 @@
                       30 LOAD_FAST                0 (stmts)
                       32 LOAD_ATTR                1 (stmt)
                       42 LOAD_FAST                0 (stmts)
                       44 LOAD_ATTR                2 (lines)
                       54 PRECALL                  2
                       58 CALL                     2
                       68 GET_ITER
-                 >>   70 FOR_ITER               246 (to 564)
+                 >>   70 FOR_ITER               240 (to 552)
                       72 UNPACK_SEQUENCE          2
                       76 STORE_FAST               5 (line)
                       78 UNPACK_SEQUENCE          2
                       82 STORE_FAST               6 (lstart)
                       84 STORE_FAST               7 (lend)
          
           59          86 LOAD_FAST                5 (line)
@@ -413,72 +412,68 @@
                      372 STORE_FAST               3 (stmt)
          
           77     >>  374 LOAD_FAST                3 (stmt)
                      376 LOAD_METHOD              7 (endswith)
                      398 LOAD_CONST               8 (';')
                      400 PRECALL                  1
                      404 CALL                     1
-                     414 POP_JUMP_FORWARD_IF_TRUE    27 (to 470)
+                     414 POP_JUMP_FORWARD_IF_TRUE    21 (to 458)
                      416 LOAD_FAST                3 (stmt)
                      418 LOAD_METHOD              7 (endswith)
                      440 LOAD_CONST               5 ('}')
                      442 PRECALL                  1
                      446 CALL                     1
-                     456 POP_JUMP_FORWARD_IF_FALSE    52 (to 562)
-                     458 LOAD_FAST                4 (level)
-                     460 LOAD_CONST               2 (0)
-                     462 COMPARE_OP               2 (==)
-                     468 POP_JUMP_FORWARD_IF_FALSE    46 (to 562)
-         
-          78     >>  470 LOAD_FAST                1 (new_stmt)
-                     472 LOAD_METHOD              4 (append)
-                     494 LOAD_FAST                3 (stmt)
-                     496 PRECALL                  1
-                     500 CALL                     1
-                     510 POP_TOP
-         
-          79         512 LOAD_FAST                2 (new_lines)
-                     514 LOAD_METHOD              4 (append)
-                     536 LOAD_FAST                9 (istart)
-                     538 LOAD_FAST                7 (lend)
-                     540 BUILD_LIST               2
-                     542 PRECALL                  1
-                     546 CALL                     1
-                     556 POP_TOP
-         
-          80         558 LOAD_CONST               1 (None)
-                     560 STORE_FAST               3 (stmt)
-                 >>  562 JUMP_BACKWARD          247 (to 70)
-         
-          83     >>  564 LOAD_FAST                3 (stmt)
-                     566 POP_JUMP_FORWARD_IF_NONE    47 (to 662)
-                     568 LOAD_FAST                3 (stmt)
-                     570 LOAD_METHOD              6 (strip)
-                     592 PRECALL                  0
-                     596 CALL                     0
-                     606 LOAD_CONST               9 ('')
-                     608 COMPARE_OP               3 (!=)
-                     614 POP_JUMP_FORWARD_IF_FALSE    23 (to 662)
-         
-          84         616 LOAD_GLOBAL             17 (NULL + logger)
-                     628 LOAD_ATTR                9 (warning)
-                     638 LOAD_CONST              10 ('Last statement not finished by ; \n ')
-                     640 LOAD_FAST                3 (stmt)
-                     642 FORMAT_VALUE             0
-                     644 BUILD_STRING             2
-                     646 PRECALL                  1
-                     650 CALL                     1
-                     660 POP_TOP
-         
-          85     >>  662 LOAD_GLOBAL             21 (NULL + Statements)
-                     674 LOAD_FAST                1 (new_stmt)
-                     676 LOAD_FAST                2 (new_lines)
-                     678 PRECALL                  2
-                     682 CALL                     2
-                     692 RETURN_VALUE
+                     456 POP_JUMP_FORWARD_IF_FALSE    46 (to 550)
+         
+          78     >>  458 LOAD_FAST                1 (new_stmt)
+                     460 LOAD_METHOD              4 (append)
+                     482 LOAD_FAST                3 (stmt)
+                     484 PRECALL                  1
+                     488 CALL                     1
+                     498 POP_TOP
+         
+          79         500 LOAD_FAST                2 (new_lines)
+                     502 LOAD_METHOD              4 (append)
+                     524 LOAD_FAST                9 (istart)
+                     526 LOAD_FAST                7 (lend)
+                     528 BUILD_LIST               2
+                     530 PRECALL                  1
+                     534 CALL                     1
+                     544 POP_TOP
+         
+          80         546 LOAD_CONST               1 (None)
+                     548 STORE_FAST               3 (stmt)
+                 >>  550 JUMP_BACKWARD          241 (to 70)
+         
+          83     >>  552 LOAD_FAST                3 (stmt)
+                     554 POP_JUMP_FORWARD_IF_NONE    47 (to 650)
+                     556 LOAD_FAST                3 (stmt)
+                     558 LOAD_METHOD              6 (strip)
+                     580 PRECALL                  0
+                     584 CALL                     0
+                     594 LOAD_CONST               9 ('')
+                     596 COMPARE_OP               3 (!=)
+                     602 POP_JUMP_FORWARD_IF_FALSE    23 (to 650)
+         
+          84         604 LOAD_GLOBAL             17 (NULL + logger)
+                     616 LOAD_ATTR                9 (warning)
+                     626 LOAD_CONST              10 ('Last statement not finished by ; \n ')
+                     628 LOAD_FAST                3 (stmt)
+                     630 FORMAT_VALUE             0
+                     632 BUILD_STRING             2
+                     634 PRECALL                  1
+                     638 CALL                     1
+                     648 POP_TOP
+         
+          85     >>  650 LOAD_GLOBAL             21 (NULL + Statements)
+                     662 LOAD_FAST                1 (new_stmt)
+                     664 LOAD_FAST                2 (new_lines)
+                     666 PRECALL                  2
+                     670 CALL                     2
+                     680 RETURN_VALUE
          consts
             'Align lines not finished by ; '
             None
             0
             '{'
             1
             '}'
@@ -492,15 +487,15 @@
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_c.py'
          name       'align_unfinished_lines'
          firstlineno 51
          lnotab
             0x02020401040104010401440208010c010a010c010c032a012a012e0102
-            02040128010602340260012a012e01060334012e01
+            02040128010602340254012a012e01060334012e01
       code
          argcount  : 1
          nlocals   : 9
          stacksize : 7
          flags     : 3
          code
             0x970067007d0167007d027401000000000000000000007c006a01000000
@@ -897,15 +892,14 @@
             0200000000000000006402a6020000ab0200000000000000007c015f0200
             000000000000007409000000000000000000007c0164036404a6030000ab
             0300000000000000007d01740b000000000000000000007c016403a60200
             00ab0200000000000000007d01740b000000000000000000007c016405a6
             020000ab0200000000000000007d01740d000000000000000000007c01a6
             010000ab0100000000000000007d01740f000000000000000000007c01a6
             010000ab0100000000000000007d017411000000000000000000007c01a6
-            010000ab0100000000000000007d017413000000000000000000007c01a6
             010000ab0100000000000000007d017c015300
          144           0 RESUME                   0
          
          154           2 LOAD_GLOBAL              1 (NULL + new_stmts)
                       14 LOAD_FAST                0 (code)
                       16 PRECALL                  1
                       20 CALL                     1
@@ -967,43 +961,37 @@
          
          162         314 LOAD_GLOBAL             15 (NULL + align_unfinished_lines)
                      326 LOAD_FAST                1 (stmts)
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               1 (stmts)
          
-         163         344 LOAD_GLOBAL             17 (NULL + split_multiple_statements)
+         164         344 LOAD_GLOBAL             17 (NULL + split_declarations)
                      356 LOAD_FAST                1 (stmts)
                      358 PRECALL                  1
                      362 CALL                     1
                      372 STORE_FAST               1 (stmts)
          
-         164         374 LOAD_GLOBAL             19 (NULL + split_declarations)
-                     386 LOAD_FAST                1 (stmts)
-                     388 PRECALL                  1
-                     392 CALL                     1
-                     402 STORE_FAST               1 (stmts)
-         
-         168         404 LOAD_FAST                1 (stmts)
-                     406 RETURN_VALUE
+         168         374 LOAD_FAST                1 (stmts)
+                     376 RETURN_VALUE
          consts
             "\n    Unformat C code by stripping comments and moving leading '&' characters.\n\n    Args:\n        code (List[str]): List of C code lines.\n\n    Returns:\n        List[Tuple[str, Tuple[int, int]]]: List of unformatted code statements along with line number ranges.\n    "
             '"'
             "'"
             '/*'
             '*/'
             '//'
-         names      ('new_stmts', 'eat_spaces', 'stmt', 'remove_strings', 'align_multiline_blocks', 'clean_inline_comments', 'clean_blanks', 'align_unfinished_lines', 'split_multiple_statements', 'split_declarations')
+         names      ('new_stmts', 'eat_spaces', 'stmt', 'remove_strings', 'align_multiline_blocks', 'clean_inline_comments', 'clean_blanks', 'align_unfinished_lines', 'split_declarations')
          varnames   ('code', 'stmts')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_c.py'
          name       'unformat_c'
          firstlineno 144
-         lnotab 0x020a1e013201340134012201200120011e011e011e011e04
+         lnotab 0x020a1e013201340134012201200120011e011e021e04
       None
    names      ('typing', 'List', 'loguru', 'logger', 'tucan.unformat_common', 'Statements', 'new_stmts', 'get_indent', 'eat_spaces', 'remove_strings', 'clean_blanks', 'clean_inline_comments', 'rm_parenthesis_content', 'clean_pure_comments', 'align_multiline_blocks', 'split_multi_statement_lines', 'tucan.kw_lang', 'KEYWORDS_C', 'remove_space_in_front_of_variables', 'align_unfinished_lines', 'split_multiple_statements', 'split_declarations', 'str', 'unformat_c')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_c.py'
    name       '<module>'
```

### Comparing `tucan-0.1.0/src/tucan/__pycache__/unformat_common.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/unformat_common.cpython-311.pyc`

 * *Files 19% similar despite different names*

#### Python bytecode

```diff
@@ -1,23 +1,24 @@
 magic:    0xa70d0d0a
-moddate:  0x337db265 (Thu Jan 25 15:24:35 2024 UTC)
-files sz: 6839
+moddate:  0x85124266 (Mon May 13 13:15:49 2024 UTC)
+files sz: 8117
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 16777216
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a046d
       055a050100640164046c066d075a070100640164056c086d095a09010064
-      0164066c0a5a0a650702004700640784006408a6020000ab020000000000
-      000000a6000000ab0000000000000000005a0b6424640c84045a0c642564
-      0f84045a0d64266427641684055a0e6428641884045a0f6429641984045a
-      10642a642b641c84055a11642a642b641d84055a126428641e84045a1364
-      2c642184045a14642d642384045a1564065300
+      0164066c0a5a0a64075a0b64085a0c64095a0d640a5a0e65070200470064
+      0b8400640ca6020000ab020000000000000000a6000000ab000000000000
+      0000005a0f642e641084045a10642f641384045a1164306431641a84055a
+      126432641c84045a136433641d84045a1464346435642084055a15643464
+      35642184055a166432642284045a176436642584045a186437642784045a
+      1964386439642b84055a1a6438643a642d84055a1b64065300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nModule that gather the most common functions of unformat\n')
                  4 STORE_NAME               0 (__doc__)
    
      5           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('annotations',))
@@ -50,138 +51,166 @@
                 56 POP_TOP
    
      9          58 LOAD_CONST               1 (0)
                 60 LOAD_CONST               6 (None)
                 62 IMPORT_NAME             10 (json)
                 64 STORE_NAME              10 (json)
    
-    12          66 LOAD_NAME                7 (dataclass)
+    11          66 LOAD_CONST               7 ('ª')
+                68 STORE_NAME              11 (CHAR_CMT_START)
    
-    13          68 PUSH_NULL
-                70 LOAD_BUILD_CLASS
-                72 LOAD_CONST               7 (<code object Statements, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 12>)
-                74 MAKE_FUNCTION            0
-                76 LOAD_CONST               8 ('Statements')
-                78 PRECALL                  2
-                82 CALL                     2
-   
-    12          92 PRECALL                  0
-                96 CALL                     0
-   
-    13         106 STORE_NAME              11 (Statements)
-   
-    46         108 LOAD_CONST              36 (('code', 'List[str]', 'return', 'Statements'))
-               110 LOAD_CONST              12 (<code object new_stmts, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 46>)
-               112 MAKE_FUNCTION            4 (annotations)
-               114 STORE_NAME              12 (new_stmts)
-   
-    53         116 LOAD_CONST              37 (('code', 'List[str]', 'string_char', 'str', 'return', 'List[str]'))
-               118 LOAD_CONST              15 (<code object remove_strings, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 53>)
-               120 MAKE_FUNCTION            4 (annotations)
-               122 STORE_NAME              13 (remove_strings)
-   
-    82         124 LOAD_CONST              38 (('(', ')', True))
-               126 LOAD_CONST              39 (('buffer', 'str', 'lchar', 'str', 'rchar', 'str', 'return', 'str'))
-               128 LOAD_CONST              22 (<code object rm_parenthesis_content, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 82>)
-               130 MAKE_FUNCTION            5 (defaults, annotations)
-               132 STORE_NAME              14 (rm_parenthesis_content)
-   
-   101         134 LOAD_CONST              40 (('stmts', 'Statements', 'return', 'Statements'))
-               136 LOAD_CONST              24 (<code object clean_blanks, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 101>)
-               138 MAKE_FUNCTION            4 (annotations)
-               140 STORE_NAME              15 (clean_blanks)
-   
-   130         142 LOAD_CONST              41 (('code', 'List[str]', 'return', 'List[str]'))
-               144 LOAD_CONST              25 (<code object eat_spaces, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 130>)
-               146 MAKE_FUNCTION            4 (annotations)
-               148 STORE_NAME              16 (eat_spaces)
-   
-   157         150 LOAD_CONST              42 (('#',))
-               152 LOAD_CONST              43 (('stmts', 'Statements', 'symbol', 'str', 'return', 'Statements'))
-               154 LOAD_CONST              28 (<code object clean_inline_comments, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 157>)
-               156 MAKE_FUNCTION            5 (defaults, annotations)
-               158 STORE_NAME              17 (clean_inline_comments)
-   
-   174         160 LOAD_CONST              42 (('#',))
-               162 LOAD_CONST              43 (('stmts', 'Statements', 'symbol', 'str', 'return', 'Statements'))
-               164 LOAD_CONST              29 (<code object clean_pure_comments, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 174>)
-               166 MAKE_FUNCTION            5 (defaults, annotations)
-               168 STORE_NAME              18 (clean_pure_comments)
-   
-   188         170 LOAD_CONST              40 (('stmts', 'Statements', 'return', 'Statements'))
-               172 LOAD_CONST              30 (<code object split_multi_statement_lines, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 188>)
-               174 MAKE_FUNCTION            4 (annotations)
-               176 STORE_NAME              19 (split_multi_statement_lines)
-   
-   204         178 LOAD_CONST              44 (('stmts', 'Statements', 'markup_in', 'str', 'markup_out', 'str', 'return', 'Statements'))
-               180 LOAD_CONST              33 (<code object align_multiline_blocks, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 204>)
-               182 MAKE_FUNCTION            4 (annotations)
-               184 STORE_NAME              20 (align_multiline_blocks)
+    12          70 LOAD_CONST               8 ('»')
+                72 STORE_NAME              12 (CHAR_CMT_STOP)
    
-   245         186 LOAD_CONST              45 (('line', 'str', 'return', 'str'))
-               188 LOAD_CONST              35 (<code object get_indent, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 245>)
+    13          74 LOAD_CONST               9 ('Ì')
+                76 STORE_NAME              13 (CHAR_EOL)
+   
+    14          78 LOAD_CONST              10 ('Ý')
+                80 STORE_NAME              14 (CHAR_CMT_EOL)
+   
+    16          82 LOAD_NAME                7 (dataclass)
+   
+    17          84 PUSH_NULL
+                86 LOAD_BUILD_CLASS
+                88 LOAD_CONST              11 (<code object Statements, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 16>)
+                90 MAKE_FUNCTION            0
+                92 LOAD_CONST              12 ('Statements')
+                94 PRECALL                  2
+                98 CALL                     2
+   
+    16         108 PRECALL                  0
+               112 CALL                     0
+   
+    17         122 STORE_NAME              15 (Statements)
+   
+    50         124 LOAD_CONST              46 (('code', 'List[str]', 'return', 'Statements'))
+               126 LOAD_CONST              16 (<code object new_stmts, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 50>)
+               128 MAKE_FUNCTION            4 (annotations)
+               130 STORE_NAME              16 (new_stmts)
+   
+    57         132 LOAD_CONST              47 (('code', 'List[str]', 'string_char', 'str', 'return', 'List[str]'))
+               134 LOAD_CONST              19 (<code object remove_strings, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 57>)
+               136 MAKE_FUNCTION            4 (annotations)
+               138 STORE_NAME              17 (remove_strings)
+   
+    86         140 LOAD_CONST              48 (('(', ')', True))
+               142 LOAD_CONST              49 (('buffer', 'str', 'lchar', 'str', 'rchar', 'str', 'return', 'str'))
+               144 LOAD_CONST              26 (<code object rm_parenthesis_content, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 86>)
+               146 MAKE_FUNCTION            5 (defaults, annotations)
+               148 STORE_NAME              18 (rm_parenthesis_content)
+   
+   105         150 LOAD_CONST              50 (('stmts', 'Statements', 'return', 'Statements'))
+               152 LOAD_CONST              28 (<code object clean_blanks, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 105>)
+               154 MAKE_FUNCTION            4 (annotations)
+               156 STORE_NAME              19 (clean_blanks)
+   
+   134         158 LOAD_CONST              51 (('code', 'List[str]', 'return', 'List[str]'))
+               160 LOAD_CONST              29 (<code object eat_spaces, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 134>)
+               162 MAKE_FUNCTION            4 (annotations)
+               164 STORE_NAME              20 (eat_spaces)
+   
+   161         166 LOAD_CONST              52 (('#',))
+               168 LOAD_CONST              53 (('stmts', 'Statements', 'symbol', 'str', 'return', 'Statements'))
+               170 LOAD_CONST              32 (<code object clean_inline_comments, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 161>)
+               172 MAKE_FUNCTION            5 (defaults, annotations)
+               174 STORE_NAME              21 (clean_inline_comments)
+   
+   178         176 LOAD_CONST              52 (('#',))
+               178 LOAD_CONST              53 (('stmts', 'Statements', 'symbol', 'str', 'return', 'Statements'))
+               180 LOAD_CONST              33 (<code object clean_pure_comments, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 178>)
+               182 MAKE_FUNCTION            5 (defaults, annotations)
+               184 STORE_NAME              22 (clean_pure_comments)
+   
+   192         186 LOAD_CONST              50 (('stmts', 'Statements', 'return', 'Statements'))
+               188 LOAD_CONST              34 (<code object split_multi_statement_lines, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 192>)
                190 MAKE_FUNCTION            4 (annotations)
-               192 STORE_NAME              21 (get_indent)
-               194 LOAD_CONST               6 (None)
-               196 RETURN_VALUE
+               192 STORE_NAME              23 (split_multi_statement_lines)
+   
+   208         194 LOAD_CONST              54 (('stmts', 'Statements', 'markup_in', 'str', 'markup_out', 'str', 'return', 'Statements'))
+               196 LOAD_CONST              37 (<code object align_multiline_blocks, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 208>)
+               198 MAKE_FUNCTION            4 (annotations)
+               200 STORE_NAME              24 (align_multiline_blocks)
+   
+   249         202 LOAD_CONST              55 (('line', 'str', 'return', 'str'))
+               204 LOAD_CONST              39 (<code object get_indent, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 249>)
+               206 MAKE_FUNCTION            4 (annotations)
+               208 STORE_NAME              25 (get_indent)
+   
+   262         210 LOAD_CONST              56 ((False,))
+               212 LOAD_CONST              57 (('line', 'str', 'fortran', 'bool', 'return', 'str'))
+               214 LOAD_CONST              43 (<code object strip_c_comment, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 262>)
+               216 MAKE_FUNCTION            5 (defaults, annotations)
+               218 STORE_NAME              26 (strip_c_comment)
+   
+   291         220 LOAD_CONST              56 ((False,))
+               222 LOAD_CONST              58 (('lines', 'List[str]', 'fortran', 'bool', 'return', 'List[str]'))
+               224 LOAD_CONST              45 (<code object clean_c_comments, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 291>)
+               226 MAKE_FUNCTION            5 (defaults, annotations)
+               228 STORE_NAME              27 (clean_c_comments)
+               230 LOAD_CONST               6 (None)
+               232 RETURN_VALUE
    consts
       '\nModule that gather the most common functions of unformat\n'
       0
       ('annotations',)
       ('Tuple', 'List')
       ('dataclass',)
       ('logger',)
       None
+      'ª'
+      '»'
+      'Ì'
+      'Ý'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a036402650464033c00000064015a
             056404650464053c000000640684005a06640784005a07640884005a0864
             0984005a09640a84005a0a64015300
-          12           0 RESUME                   0
+          16           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Statements')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          14          12 LOAD_CONST               1 (None)
+          18          12 LOAD_CONST               1 (None)
                       14 STORE_NAME               3 (stmt)
                       16 LOAD_CONST               2 ('List[str]')
                       18 LOAD_NAME                4 (__annotations__)
                       20 LOAD_CONST               3 ('stmt')
                       22 STORE_SUBSCR
          
-          15          26 LOAD_CONST               1 (None)
+          19          26 LOAD_CONST               1 (None)
                       28 STORE_NAME               5 (lines)
                       30 LOAD_CONST               4 ('List[Tuple[int, int]]')
                       32 LOAD_NAME                4 (__annotations__)
                       34 LOAD_CONST               5 ('lines')
                       36 STORE_SUBSCR
          
-          17          40 LOAD_CONST               6 (<code object __str__, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 17>)
+          21          40 LOAD_CONST               6 (<code object __str__, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 21>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               6 (__str__)
          
-          25          46 LOAD_CONST               7 (<code object to_code, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 25>)
+          29          46 LOAD_CONST               7 (<code object to_code, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 29>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               7 (to_code)
          
-          29          52 LOAD_CONST               8 (<code object to_nob, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 29>)
+          33          52 LOAD_CONST               8 (<code object to_nob, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 33>)
                       54 MAKE_FUNCTION            0
                       56 STORE_NAME               8 (to_nob)
          
-          32          58 LOAD_CONST               9 (<code object dump_json, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 32>)
+          36          58 LOAD_CONST               9 (<code object dump_json, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 36>)
                       60 MAKE_FUNCTION            0
                       62 STORE_NAME               9 (dump_json)
          
-          38          64 LOAD_CONST              10 (<code object dump_code, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 38>)
+          42          64 LOAD_CONST              10 (<code object dump_code, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 42>)
                       66 MAKE_FUNCTION            0
                       68 STORE_NAME              10 (dump_code)
                       70 LOAD_CONST               1 (None)
                       72 RETURN_VALUE
          consts
             'Statements'
             None
@@ -197,35 +226,35 @@
                code
                   0x970064017d017401000000000000000000007c006a0100000000000000
                   007c006a020000000000000000a6020000ab02000000000000000044005d
                   175c0200007d025c0200007d037d047c0164027c039b0064037c049b0064
                   047c029b0064059d077a0d00007d018c187c0164067a0d00007d017c0164
                   077407000000000000000000007c006a010000000000000000a6010000ab
                   0100000000000000009b009d027a0d00007d017c015300
-                17           0 RESUME                   0
+                21           0 RESUME                   0
                
-                18           2 LOAD_CONST               1 ('')
+                22           2 LOAD_CONST               1 ('')
                              4 STORE_FAST               1 (out)
                
-                19           6 LOAD_GLOBAL              1 (NULL + zip)
+                23           6 LOAD_GLOBAL              1 (NULL + zip)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (stmt)
                             30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                2 (lines)
                             42 PRECALL                  2
                             46 CALL                     2
                             56 GET_ITER
                        >>   58 FOR_ITER                23 (to 106)
                             60 UNPACK_SEQUENCE          2
                             64 STORE_FAST               2 (line)
                             66 UNPACK_SEQUENCE          2
                             70 STORE_FAST               3 (i1)
                             72 STORE_FAST               4 (i2)
                
-                20          74 LOAD_FAST                1 (out)
+                24          74 LOAD_FAST                1 (out)
                             76 LOAD_CONST               2 ('(')
                             78 LOAD_FAST                3 (i1)
                             80 FORMAT_VALUE             0
                             82 LOAD_CONST               3 ('-')
                             84 LOAD_FAST                4 (i2)
                             86 FORMAT_VALUE             0
                             88 LOAD_CONST               4 (')  ')
@@ -233,32 +262,32 @@
                             92 FORMAT_VALUE             0
                             94 LOAD_CONST               5 ('\n')
                             96 BUILD_STRING             7
                             98 BINARY_OP               13 (+=)
                            102 STORE_FAST               1 (out)
                            104 JUMP_BACKWARD           24 (to 58)
                
-                21     >>  106 LOAD_FAST                1 (out)
+                25     >>  106 LOAD_FAST                1 (out)
                            108 LOAD_CONST               6 ('=======================')
                            110 BINARY_OP               13 (+=)
                            114 STORE_FAST               1 (out)
                
-                22         116 LOAD_FAST                1 (out)
+                26         116 LOAD_FAST                1 (out)
                            118 LOAD_CONST               7 ('Statements found : ')
                            120 LOAD_GLOBAL              7 (NULL + len)
                            132 LOAD_FAST                0 (self)
                            134 LOAD_ATTR                1 (stmt)
                            144 PRECALL                  1
                            148 CALL                     1
                            158 FORMAT_VALUE             0
                            160 BUILD_STRING             2
                            162 BINARY_OP               13 (+=)
                            166 STORE_FAST               1 (out)
                
-                23         168 LOAD_FAST                1 (out)
+                27         168 LOAD_FAST                1 (out)
                            170 RETURN_VALUE
                consts
                   None
                   ''
                   '('
                   '-'
                   ')  '
@@ -267,46 +296,46 @@
                   'Statements found : '
                names      ('zip', 'stmt', 'lines', 'len')
                varnames   ('self', 'out', 'line', 'i1', 'i2')
                freevars   ()
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
                name       '__str__'
-               firstlineno 17
+               firstlineno 21
                lnotab 0x02010401440120010a013401
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x9700640184007c006a0000000000000000004400a6000000ab00000000
                   00000000007d017c015300
-                25           0 RESUME                   0
+                29           0 RESUME                   0
                
-                26           2 LOAD_CONST               1 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 26>)
+                30           2 LOAD_CONST               1 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 30>)
                              4 MAKE_FUNCTION            0
                              6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (stmt)
                             18 GET_ITER
                             20 PRECALL                  0
                             24 CALL                     0
                             34 STORE_FAST               1 (out)
                
-                27          36 LOAD_FAST                1 (out)
+                31          36 LOAD_FAST                1 (out)
                             38 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code 0x970067007c005d077d017c019b0064009d0291028c085300
-                      26           0 RESUME                   0
+                      30           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 7 (to 22)
                                    8 STORE_FAST               1 (stmt)
                                   10 LOAD_FAST                1 (stmt)
                                   12 FORMAT_VALUE             0
                                   14 LOAD_CONST               0 ('\n')
@@ -318,36 +347,36 @@
                         '\n'
                      names      ()
                      varnames   ('.0', 'stmt')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
                      name       '<listcomp>'
-                     firstlineno 26
+                     firstlineno 30
                      lnotab 0x
                names      ('stmt',)
                varnames   ('self', 'out')
                freevars   ()
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
                name       'to_code'
-               firstlineno 25
+               firstlineno 29
                lnotab 0x02012201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 16777219
                code
                   0x9700640184007401000000000000000000007c006a0100000000000000
                   007c006a020000000000000000a6020000ab0200000000000000004400a6
                   000000ab0000000000000000005300
-                29           0 RESUME                   0
+                33           0 RESUME                   0
                
-                30           2 LOAD_CONST               1 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 30>)
+                34           2 LOAD_CONST               1 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 34>)
                              4 MAKE_FUNCTION            0
                              6 LOAD_GLOBAL              1 (NULL + zip)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (stmt)
                             30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                2 (lines)
                             42 PRECALL                  2
@@ -360,15 +389,15 @@
                   None
                   code
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 16777235
                      code 0x970067007c005d095c0200007d017d027c017c02670291028c0a5300
-                      30           0 RESUME                   0
+                      34           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 UNPACK_SEQUENCE          2
                                   12 STORE_FAST               1 (st)
                                   14 STORE_FAST               2 (lsp)
                                   16 LOAD_FAST                1 (st)
@@ -380,23 +409,23 @@
                      consts
                      names      ()
                      varnames   ('.0', 'st', 'lsp')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
                      name       '<listcomp>'
-                     firstlineno 30
+                     firstlineno 34
                      lnotab 0x
                names      ('zip', 'stmt', 'lines')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
                name       'to_nob'
-               firstlineno 29
+               firstlineno 33
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 7
                flags     : 16777219
                code
@@ -404,49 +433,49 @@
                   009d02a6010000ab01000000000000000001007405000000000000000000
                   007c016402a6020000ab02000000000000000035007d0274070000000000
                   00000000006a0400000000000000007c00a0050000000000000000000000
                   000000000000000000a6000000ab0000000000000000007c0264036404ac
                   05a6040000ab0400000000000000000100640064006400a6020000ab0200
                   000000000000000100640053002300310073047702780359007701010059
                   000100010064005300
-                32           0 RESUME                   0
+                36           0 RESUME                   0
                
-                34           2 LOAD_GLOBAL              1 (NULL + logger)
+                38           2 LOAD_GLOBAL              1 (NULL + logger)
                             14 LOAD_ATTR                1 (info)
                             24 LOAD_CONST               1 ('Data dumped to ')
                             26 LOAD_FAST                1 (newfile)
                             28 FORMAT_VALUE             0
                             30 BUILD_STRING             2
                             32 PRECALL                  1
                             36 CALL                     1
                             46 POP_TOP
                
-                35          48 LOAD_GLOBAL              5 (NULL + open)
+                39          48 LOAD_GLOBAL              5 (NULL + open)
                             60 LOAD_FAST                1 (newfile)
                             62 LOAD_CONST               2 ('w')
                             64 PRECALL                  2
                             68 CALL                     2
                             78 BEFORE_WITH
                             80 STORE_FAST               2 (fout)
                
-                36          82 LOAD_GLOBAL              7 (NULL + json)
+                40          82 LOAD_GLOBAL              7 (NULL + json)
                             94 LOAD_ATTR                4 (dump)
                            104 LOAD_FAST                0 (self)
                            106 LOAD_METHOD              5 (to_nob)
                            128 PRECALL                  0
                            132 CALL                     0
                            142 LOAD_FAST                2 (fout)
                            144 LOAD_CONST               3 (2)
                            146 LOAD_CONST               4 (True)
                            148 KW_NAMES                 5
                            150 PRECALL                  4
                            154 CALL                     4
                            164 POP_TOP
                
-                35         166 LOAD_CONST               0 (None)
+                39         166 LOAD_CONST               0 (None)
                            168 LOAD_CONST               0 (None)
                            170 LOAD_CONST               0 (None)
                            172 PRECALL                  2
                            176 CALL                     2
                            186 POP_TOP
                            188 LOAD_CONST               0 (None)
                            190 RETURN_VALUE
@@ -476,50 +505,50 @@
                   ('indent', 'sort_keys')
                names      ('logger', 'info', 'open', 'json', 'dump', 'to_nob')
                varnames   ('self', 'newfile', 'fout')
                freevars   ()
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
                name       'dump_json'
-               firstlineno 32
+               firstlineno 36
                lnotab 0x02022e01220154ff
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
                flags     : 16777219
                code
                   0x97007401000000000000000000007c016401a6020000ab020000000000
                   00000035007d027c02a00100000000000000000000000000000000000000
                   007c00a0020000000000000000000000000000000000000000a6000000ab
                   000000000000000000a6010000ab01000000000000000001006400640064
                   00a6020000ab02000000000000000001006e0b2300310073047702780359
                   007701010059000100010074070000000000000000000064027c019b009d
                   02a6010000ab010000000000000000010064005300
-                38           0 RESUME                   0
+                42           0 RESUME                   0
                
-                40           2 LOAD_GLOBAL              1 (NULL + open)
+                44           2 LOAD_GLOBAL              1 (NULL + open)
                             14 LOAD_FAST                1 (newfile)
                             16 LOAD_CONST               1 ('w')
                             18 PRECALL                  2
                             22 CALL                     2
                             32 BEFORE_WITH
                             34 STORE_FAST               2 (fout)
                
-                41          36 LOAD_FAST                2 (fout)
+                45          36 LOAD_FAST                2 (fout)
                             38 LOAD_METHOD              1 (writelines)
                             60 LOAD_FAST                0 (self)
                             62 LOAD_METHOD              2 (to_code)
                             84 PRECALL                  0
                             88 CALL                     0
                             98 PRECALL                  1
                            102 CALL                     1
                            112 POP_TOP
                
-                40         114 LOAD_CONST               0 (None)
+                44         114 LOAD_CONST               0 (None)
                            116 LOAD_CONST               0 (None)
                            118 LOAD_CONST               0 (None)
                            120 PRECALL                  2
                            124 CALL                     2
                            134 POP_TOP
                            136 JUMP_FORWARD            11 (to 160)
                        >>  138 PUSH_EXC_INFO
@@ -530,15 +559,15 @@
                            148 POP_EXCEPT
                            150 RERAISE                  1
                        >>  152 POP_TOP
                            154 POP_EXCEPT
                            156 POP_TOP
                            158 POP_TOP
                
-                42     >>  160 LOAD_GLOBAL              7 (NULL + print)
+                46     >>  160 LOAD_GLOBAL              7 (NULL + print)
                            172 LOAD_CONST               2 ('\n\nCleaned version dumped in ')
                            174 LOAD_FAST                1 (newfile)
                            176 FORMAT_VALUE             0
                            178 BUILD_STRING             2
                            180 PRECALL                  1
                            184 CALL                     1
                            194 POP_TOP
@@ -554,67 +583,67 @@
                   '\n\nCleaned version dumped in '
                names      ('open', 'writelines', 'to_code', 'print')
                varnames   ('self', 'newfile', 'fout')
                freevars   ()
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
                name       'dump_code'
-               firstlineno 38
+               firstlineno 42
                lnotab 0x020222014eff2e02
          names      ('__name__', '__module__', '__qualname__', 'stmt', '__annotations__', 'lines', '__str__', 'to_code', 'to_nob', 'dump_json', 'dump_code')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
          name       'Statements'
-         firstlineno 12
+         firstlineno 16
          lnotab 0x0c020e010e020608060406030606
       'Statements'
       'code'
       'List[str]'
       'return'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 7
          flags     : 16777219
          code
             0x97007401000000000000000000007c0064018400740300000000000000
             0000007c00a6010000ab0100000000000000004400a6000000ab00000000
             0000000000a6020000ab0200000000000000005300
-          46           0 RESUME                   0
+          50           0 RESUME                   0
          
-          47           2 LOAD_GLOBAL              1 (NULL + Statements)
+          51           2 LOAD_GLOBAL              1 (NULL + Statements)
          
-          48          14 LOAD_FAST                0 (code)
+          52          14 LOAD_FAST                0 (code)
          
-          49          16 LOAD_CONST               1 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 49>)
+          53          16 LOAD_CONST               1 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py", line 53>)
                       18 MAKE_FUNCTION            0
                       20 LOAD_GLOBAL              3 (NULL + enumerate)
                       32 LOAD_FAST                0 (code)
                       34 PRECALL                  1
                       38 CALL                     1
                       48 GET_ITER
                       50 PRECALL                  0
                       54 CALL                     0
          
-          47          64 PRECALL                  2
+          51          64 PRECALL                  2
                       68 CALL                     2
                       78 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 16777235
                code
                   0x970067007c005d0f5c0200007d017d027c0164007a0000007c0164007a
                   000000670291028c105300
-                49           0 RESUME                   0
+                53           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                15 (to 38)
                              8 UNPACK_SEQUENCE          2
                             12 STORE_FAST               1 (i)
                             14 STORE_FAST               2 (_)
                             16 LOAD_FAST                1 (i)
@@ -631,23 +660,23 @@
                   1
                names      ()
                varnames   ('.0', 'i', '_')
                freevars   ()
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
                name       '<listcomp>'
-               firstlineno 49
+               firstlineno 53
                lnotab 0x
          names      ('Statements', 'enumerate')
          varnames   ('code',)
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
          name       'new_stmts'
-         firstlineno 46
+         firstlineno 50
          lnotab 0x02010c01020130fe
       'string_char'
       'str'
       code
          argcount  : 2
          nlocals   : 8
          stacksize : 5
@@ -655,110 +684,110 @@
          code
             0x970067007d027c0044005d4d7d0364017d0464027d0564027d067c0344
             005d267d077c077c016b020000000072117c04730364037d046e0c7c057c
             079b0064049d027a0d00007d0564017d0464027d067c0473067c057c077a
             0d00007d058c217c067c077a0d00007d068c277c0472057c057c067a0d00
             007d057c02a00000000000000000000000000000000000000000007c05a6
             010000ab01000000000000000001008c4e7c025300
-          53           0 RESUME                   0
+          57           0 RESUME                   0
          
-          54           2 BUILD_LIST               0
+          58           2 BUILD_LIST               0
                        4 STORE_FAST               2 (new_stmt)
          
-          56           6 LOAD_FAST                0 (code)
+          60           6 LOAD_FAST                0 (code)
                        8 GET_ITER
                  >>   10 FOR_ITER                77 (to 166)
                       12 STORE_FAST               3 (line)
          
-          57          14 LOAD_CONST               1 (False)
+          61          14 LOAD_CONST               1 (False)
                       16 STORE_FAST               4 (inside_string_context)
          
-          58          18 LOAD_CONST               2 ('')
+          62          18 LOAD_CONST               2 ('')
                       20 STORE_FAST               5 (buffer)
          
-          59          22 LOAD_CONST               2 ('')
+          63          22 LOAD_CONST               2 ('')
                       24 STORE_FAST               6 (tmp_buffer)
          
-          60          26 LOAD_FAST                3 (line)
+          64          26 LOAD_FAST                3 (line)
                       28 GET_ITER
                  >>   30 FOR_ITER                38 (to 108)
                       32 STORE_FAST               7 (char)
          
-          61          34 LOAD_FAST                7 (char)
+          65          34 LOAD_FAST                7 (char)
                       36 LOAD_FAST                1 (string_char)
                       38 COMPARE_OP               2 (==)
                       44 POP_JUMP_FORWARD_IF_FALSE    17 (to 80)
          
-          62          46 LOAD_FAST                4 (inside_string_context)
+          66          46 LOAD_FAST                4 (inside_string_context)
                       48 POP_JUMP_FORWARD_IF_TRUE     3 (to 56)
          
-          63          50 LOAD_CONST               3 (True)
+          67          50 LOAD_CONST               3 (True)
                       52 STORE_FAST               4 (inside_string_context)
                       54 JUMP_FORWARD            12 (to 80)
          
-          65     >>   56 LOAD_FAST                5 (buffer)
+          69     >>   56 LOAD_FAST                5 (buffer)
                       58 LOAD_FAST                7 (char)
                       60 FORMAT_VALUE             0
                       62 LOAD_CONST               4 ('___')
                       64 BUILD_STRING             2
                       66 BINARY_OP               13 (+=)
                       70 STORE_FAST               5 (buffer)
          
-          66          72 LOAD_CONST               1 (False)
+          70          72 LOAD_CONST               1 (False)
                       74 STORE_FAST               4 (inside_string_context)
          
-          67          76 LOAD_CONST               2 ('')
+          71          76 LOAD_CONST               2 ('')
                       78 STORE_FAST               6 (tmp_buffer)
          
-          70     >>   80 LOAD_FAST                4 (inside_string_context)
+          74     >>   80 LOAD_FAST                4 (inside_string_context)
                       82 POP_JUMP_FORWARD_IF_TRUE     6 (to 96)
          
-          71          84 LOAD_FAST                5 (buffer)
+          75          84 LOAD_FAST                5 (buffer)
                       86 LOAD_FAST                7 (char)
                       88 BINARY_OP               13 (+=)
                       92 STORE_FAST               5 (buffer)
                       94 JUMP_BACKWARD           33 (to 30)
          
-          73     >>   96 LOAD_FAST                6 (tmp_buffer)
+          77     >>   96 LOAD_FAST                6 (tmp_buffer)
                       98 LOAD_FAST                7 (char)
                      100 BINARY_OP               13 (+=)
                      104 STORE_FAST               6 (tmp_buffer)
                      106 JUMP_BACKWARD           39 (to 30)
          
-          75     >>  108 LOAD_FAST                4 (inside_string_context)
+          79     >>  108 LOAD_FAST                4 (inside_string_context)
                      110 POP_JUMP_FORWARD_IF_FALSE     5 (to 122)
          
-          76         112 LOAD_FAST                5 (buffer)
+          80         112 LOAD_FAST                5 (buffer)
                      114 LOAD_FAST                6 (tmp_buffer)
                      116 BINARY_OP               13 (+=)
                      120 STORE_FAST               5 (buffer)
          
-          78     >>  122 LOAD_FAST                2 (new_stmt)
+          82     >>  122 LOAD_FAST                2 (new_stmt)
                      124 LOAD_METHOD              0 (append)
                      146 LOAD_FAST                5 (buffer)
                      148 PRECALL                  1
                      152 CALL                     1
                      162 POP_TOP
                      164 JUMP_BACKWARD           78 (to 10)
          
-          79     >>  166 LOAD_FAST                2 (new_stmt)
+          83     >>  166 LOAD_FAST                2 (new_stmt)
                      168 RETURN_VALUE
          consts
             None
             False
             ''
             True
             '___'
          names      ('append',)
          varnames   ('code', 'string_char', 'new_stmt', 'line', 'inside_string_context', 'buffer', 'tmp_buffer', 'char')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
          name       'remove_strings'
-         firstlineno 53
+         firstlineno 57
          lnotab
             0x02010402080104010401040108010c010401060210010401040304010c
             020c0204010a022c01
       '('
       ')'
       True
       'buffer'
@@ -773,91 +802,91 @@
             0x970064017d0464027d057c0044005d237d067c0464016b020000000072
             057c057c067a0d00007d057c067c016b020000000072057c0464037a0d00
             007d047c067c026b020000000072057c0464037a1700007d048c247c0372
             2c7c05a00000000000000000000000000000000000000000007c016402a6
             020000ab0200000000000000007d057c05a0000000000000000000000000
             0000000000000000007c026402a6020000ab0200000000000000007d057c
             055300
-          82           0 RESUME                   0
+          86           0 RESUME                   0
          
-          84           2 LOAD_CONST               1 (0)
+          88           2 LOAD_CONST               1 (0)
                        4 STORE_FAST               4 (lvl)
          
-          85           6 LOAD_CONST               2 ('')
+          89           6 LOAD_CONST               2 ('')
                        8 STORE_FAST               5 (out)
          
-          86          10 LOAD_FAST                0 (buffer)
+          90          10 LOAD_FAST                0 (buffer)
                       12 GET_ITER
                  >>   14 FOR_ITER                35 (to 86)
                       16 STORE_FAST               6 (char)
          
-          87          18 LOAD_FAST                4 (lvl)
+          91          18 LOAD_FAST                4 (lvl)
                       20 LOAD_CONST               1 (0)
                       22 COMPARE_OP               2 (==)
                       28 POP_JUMP_FORWARD_IF_FALSE     5 (to 40)
          
-          88          30 LOAD_FAST                5 (out)
+          92          30 LOAD_FAST                5 (out)
                       32 LOAD_FAST                6 (char)
                       34 BINARY_OP               13 (+=)
                       38 STORE_FAST               5 (out)
          
-          89     >>   40 LOAD_FAST                6 (char)
+          93     >>   40 LOAD_FAST                6 (char)
                       42 LOAD_FAST                1 (lchar)
                       44 COMPARE_OP               2 (==)
                       50 POP_JUMP_FORWARD_IF_FALSE     5 (to 62)
          
-          90          52 LOAD_FAST                4 (lvl)
+          94          52 LOAD_FAST                4 (lvl)
                       54 LOAD_CONST               3 (1)
                       56 BINARY_OP               13 (+=)
                       60 STORE_FAST               4 (lvl)
          
-          92     >>   62 LOAD_FAST                6 (char)
+          96     >>   62 LOAD_FAST                6 (char)
                       64 LOAD_FAST                2 (rchar)
                       66 COMPARE_OP               2 (==)
                       72 POP_JUMP_FORWARD_IF_FALSE     5 (to 84)
          
-          93          74 LOAD_FAST                4 (lvl)
+          97          74 LOAD_FAST                4 (lvl)
                       76 LOAD_CONST               3 (1)
                       78 BINARY_OP               23 (-=)
                       82 STORE_FAST               4 (lvl)
                  >>   84 JUMP_BACKWARD           36 (to 14)
          
-          95     >>   86 LOAD_FAST                3 (greedy)
+          99     >>   86 LOAD_FAST                3 (greedy)
                       88 POP_JUMP_FORWARD_IF_FALSE    44 (to 178)
          
-          96          90 LOAD_FAST                5 (out)
+         100          90 LOAD_FAST                5 (out)
                       92 LOAD_METHOD              0 (replace)
                      114 LOAD_FAST                1 (lchar)
                      116 LOAD_CONST               2 ('')
                      118 PRECALL                  2
                      122 CALL                     2
                      132 STORE_FAST               5 (out)
          
-          97         134 LOAD_FAST                5 (out)
+         101         134 LOAD_FAST                5 (out)
                      136 LOAD_METHOD              0 (replace)
                      158 LOAD_FAST                2 (rchar)
                      160 LOAD_CONST               2 ('')
                      162 PRECALL                  2
                      166 CALL                     2
                      176 STORE_FAST               5 (out)
          
-          98     >>  178 LOAD_FAST                5 (out)
+         102     >>  178 LOAD_FAST                5 (out)
                      180 RETURN_VALUE
          consts
             'Remove the content of parenthesis'
             0
             ''
             1
          names      ('replace',)
          varnames   ('buffer', 'lchar', 'rchar', 'greedy', 'lvl', 'out', 'char')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
          name       'rm_parenthesis_content'
-         firstlineno 82
+         firstlineno 86
          lnotab 0x02020401040108010c010a010c010a020c010c0204012c012c01
       'stmts'
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 5
          flags     : 16777219
@@ -872,98 +901,98 @@
             01724c7c0164021900000000000000000064016b030000000072407c01a0
             0400000000000000000000000000000000000000006401a6010000ab0100
             0000000000000001007c0264021900000000000000000064031900000000
             00000000007d057c02a00400000000000000000000000000000000000000
             007c0564047a0000007c0564047a0000006702a6010000ab010000000000
             0000000100740b000000000000000000007c017c02a6020000ab02000000
             00000000005300
-         101           0 RESUME                   0
+         105           0 RESUME                   0
          
-         111           2 BUILD_LIST               0
+         115           2 BUILD_LIST               0
                        4 STORE_FAST               1 (new_stmt)
          
-         112           6 BUILD_LIST               0
+         116           6 BUILD_LIST               0
                        8 STORE_FAST               2 (new_lines)
          
-         113          10 LOAD_GLOBAL              1 (NULL + zip)
+         117          10 LOAD_GLOBAL              1 (NULL + zip)
                       22 LOAD_FAST                0 (stmts)
                       24 LOAD_ATTR                1 (stmt)
                       34 LOAD_FAST                0 (stmts)
                       36 LOAD_ATTR                2 (lines)
                       46 PRECALL                  2
                       50 CALL                     2
                       60 GET_ITER
                  >>   62 FOR_ITER                72 (to 208)
                       64 UNPACK_SEQUENCE          2
                       68 STORE_FAST               3 (line)
                       70 STORE_FAST               4 (lines_span)
          
-         114          72 LOAD_FAST                3 (line)
+         118          72 LOAD_FAST                3 (line)
                       74 LOAD_METHOD              3 (strip)
                       96 PRECALL                  0
                      100 CALL                     0
                      110 LOAD_CONST               1 ('')
                      112 COMPARE_OP               2 (==)
                      118 POP_JUMP_FORWARD_IF_FALSE     1 (to 122)
          
-         115         120 JUMP_BACKWARD           30 (to 62)
+         119         120 JUMP_BACKWARD           30 (to 62)
          
-         117     >>  122 LOAD_FAST                1 (new_stmt)
+         121     >>  122 LOAD_FAST                1 (new_stmt)
                      124 LOAD_METHOD              4 (append)
                      146 LOAD_FAST                3 (line)
                      148 PRECALL                  1
                      152 CALL                     1
                      162 POP_TOP
          
-         118         164 LOAD_FAST                2 (new_lines)
+         122         164 LOAD_FAST                2 (new_lines)
                      166 LOAD_METHOD              4 (append)
                      188 LOAD_FAST                4 (lines_span)
                      190 PRECALL                  1
                      194 CALL                     1
                      204 POP_TOP
                      206 JUMP_BACKWARD           73 (to 62)
          
-         121     >>  208 LOAD_FAST                1 (new_stmt)
+         125     >>  208 LOAD_FAST                1 (new_stmt)
                      210 POP_JUMP_FORWARD_IF_FALSE    76 (to 364)
          
-         122         212 LOAD_FAST                1 (new_stmt)
+         126         212 LOAD_FAST                1 (new_stmt)
                      214 LOAD_CONST               2 (-1)
                      216 BINARY_SUBSCR
                      226 LOAD_CONST               1 ('')
                      228 COMPARE_OP               3 (!=)
                      234 POP_JUMP_FORWARD_IF_FALSE    64 (to 364)
          
-         123         236 LOAD_FAST                1 (new_stmt)
+         127         236 LOAD_FAST                1 (new_stmt)
                      238 LOAD_METHOD              4 (append)
                      260 LOAD_CONST               1 ('')
                      262 PRECALL                  1
                      266 CALL                     1
                      276 POP_TOP
          
-         124         278 LOAD_FAST                2 (new_lines)
+         128         278 LOAD_FAST                2 (new_lines)
                      280 LOAD_CONST               2 (-1)
                      282 BINARY_SUBSCR
                      292 LOAD_CONST               3 (0)
                      294 BINARY_SUBSCR
                      304 STORE_FAST               5 (last_line)
          
-         125         306 LOAD_FAST                2 (new_lines)
+         129         306 LOAD_FAST                2 (new_lines)
                      308 LOAD_METHOD              4 (append)
                      330 LOAD_FAST                5 (last_line)
                      332 LOAD_CONST               4 (1)
                      334 BINARY_OP                0 (+)
                      338 LOAD_FAST                5 (last_line)
                      340 LOAD_CONST               4 (1)
                      342 BINARY_OP                0 (+)
                      346 BUILD_LIST               2
                      348 PRECALL                  1
                      352 CALL                     1
                      362 POP_TOP
          
-         127     >>  364 LOAD_GLOBAL             11 (NULL + Statements)
+         131     >>  364 LOAD_GLOBAL             11 (NULL + Statements)
                      376 LOAD_FAST                1 (new_stmt)
                      378 LOAD_FAST                2 (new_lines)
                      380 PRECALL                  2
                      384 CALL                     2
                      394 RETURN_VALUE
          consts
             '\n    Perform the first pass to strip comments and blank lines.\n\n    Args:\n        code (List[str]): List of code lines.\n\n    Returns:\n        List[Tuple[str, int]]: List of code lines without comments and blank lines.\n    '
@@ -973,15 +1002,15 @@
             1
          names      ('zip', 'stmt', 'lines', 'strip', 'append', 'Statements')
          varnames   ('stmts', 'new_stmt', 'new_lines', 'line', 'lines_span', 'last_line')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
          name       'clean_blanks'
-         firstlineno 101
+         firstlineno 105
          lnotab 0x020a040104013e01300102022a012c03040118012a011c013a02
       code
          argcount  : 1
          nlocals   : 8
          stacksize : 6
          flags     : 16777219
          code
@@ -992,115 +1021,115 @@
             007d057d0609007c02a00200000000000000000000000000000000000000
             00a6000000ab0000000000000000007c0564027a00000019000000000000
             0000007d076e12230074060000000000000000000024007205010064017d
             0759006e0477007803590077017c0664036b0200000000720f7c04640476
             01720a7c076405760172067c037c067a0d00007d036e066e057c037c067a
             0d00007d037c067d048c537c01a004000000000000000000000000000000
             00000000007c03a6010000ab01000000000000000001008c9d7c015300
-         130           0 RESUME                   0
+         134           0 RESUME                   0
          
-         132           2 BUILD_LIST               0
+         136           2 BUILD_LIST               0
                        4 STORE_FAST               1 (new_stmt)
          
-         133           6 LOAD_FAST                0 (code)
+         137           6 LOAD_FAST                0 (code)
                        8 GET_ITER
                  >>   10 FOR_ITER               156 (to 324)
                       12 STORE_FAST               2 (line)
          
-         134          14 LOAD_GLOBAL              1 (NULL + get_indent)
+         138          14 LOAD_GLOBAL              1 (NULL + get_indent)
                       26 LOAD_FAST                2 (line)
                       28 PRECALL                  1
                       32 CALL                     1
                       42 STORE_FAST               3 (out)
          
-         136          44 LOAD_CONST               1 (None)
+         140          44 LOAD_CONST               1 (None)
                       46 STORE_FAST               4 (prevchar)
          
-         137          48 LOAD_GLOBAL              3 (NULL + enumerate)
+         141          48 LOAD_GLOBAL              3 (NULL + enumerate)
                       60 LOAD_FAST                2 (line)
                       62 LOAD_METHOD              2 (strip)
                       84 PRECALL                  0
                       88 CALL                     0
                       98 PRECALL                  1
                      102 CALL                     1
                      112 GET_ITER
                  >>  114 FOR_ITER                82 (to 280)
                      116 UNPACK_SEQUENCE          2
                      120 STORE_FAST               5 (i)
                      122 STORE_FAST               6 (char)
          
-         138         124 NOP
+         142         124 NOP
          
-         139         126 LOAD_FAST                2 (line)
+         143         126 LOAD_FAST                2 (line)
                      128 LOAD_METHOD              2 (strip)
                      150 PRECALL                  0
                      154 CALL                     0
                      164 LOAD_FAST                5 (i)
                      166 LOAD_CONST               2 (1)
                      168 BINARY_OP                0 (+)
                      172 BINARY_SUBSCR
                      182 STORE_FAST               7 (next_char)
                      184 JUMP_FORWARD            18 (to 222)
                  >>  186 PUSH_EXC_INFO
          
-         140         188 LOAD_GLOBAL              6 (IndexError)
+         144         188 LOAD_GLOBAL              6 (IndexError)
                      200 CHECK_EXC_MATCH
                      202 POP_JUMP_FORWARD_IF_FALSE     5 (to 214)
                      204 POP_TOP
          
-         141         206 LOAD_CONST               1 (None)
+         145         206 LOAD_CONST               1 (None)
                      208 STORE_FAST               7 (next_char)
                      210 POP_EXCEPT
                      212 JUMP_FORWARD             4 (to 222)
          
-         140     >>  214 RERAISE                  0
+         144     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          
-         143     >>  222 LOAD_FAST                6 (char)
+         147     >>  222 LOAD_FAST                6 (char)
                      224 LOAD_CONST               3 (' ')
                      226 COMPARE_OP               2 (==)
                      232 POP_JUMP_FORWARD_IF_FALSE    15 (to 264)
          
-         144         234 LOAD_FAST                4 (prevchar)
+         148         234 LOAD_FAST                4 (prevchar)
                      236 LOAD_CONST               4 ((' ', ':', ';', ','))
                      238 CONTAINS_OP              1
                      240 POP_JUMP_FORWARD_IF_FALSE    10 (to 262)
                      242 LOAD_FAST                7 (next_char)
                      244 LOAD_CONST               5 ((':', ';', ','))
                      246 CONTAINS_OP              1
                      248 POP_JUMP_FORWARD_IF_FALSE     6 (to 262)
          
-         145         250 LOAD_FAST                3 (out)
+         149         250 LOAD_FAST                3 (out)
                      252 LOAD_FAST                6 (char)
                      254 BINARY_OP               13 (+=)
                      258 STORE_FAST               3 (out)
                      260 JUMP_FORWARD             6 (to 274)
          
-         147     >>  262 JUMP_FORWARD             5 (to 274)
+         151     >>  262 JUMP_FORWARD             5 (to 274)
          
-         149     >>  264 LOAD_FAST                3 (out)
+         153     >>  264 LOAD_FAST                3 (out)
                      266 LOAD_FAST                6 (char)
                      268 BINARY_OP               13 (+=)
                      272 STORE_FAST               3 (out)
          
-         151     >>  274 LOAD_FAST                6 (char)
+         155     >>  274 LOAD_FAST                6 (char)
                      276 STORE_FAST               4 (prevchar)
                      278 JUMP_BACKWARD           83 (to 114)
          
-         152     >>  280 LOAD_FAST                1 (new_stmt)
+         156     >>  280 LOAD_FAST                1 (new_stmt)
                      282 LOAD_METHOD              4 (append)
                      304 LOAD_FAST                3 (out)
                      306 PRECALL                  1
                      310 CALL                     1
                      320 POP_TOP
                      322 JUMP_BACKWARD          157 (to 10)
          
-         153     >>  324 LOAD_FAST                1 (new_stmt)
+         157     >>  324 LOAD_FAST                1 (new_stmt)
                      326 RETURN_VALUE
          ExceptionTable:
            126 to 182 -> 186 [2]
            186 to 208 -> 216 [3] lasti
            214 to 214 -> 216 [3] lasti
          consts
             'Remove unwanted multiple spacing '
@@ -1111,15 +1140,15 @@
             (':', ';', ',')
          names      ('get_indent', 'enumerate', 'strip', 'IndexError', 'append')
          varnames   ('code', 'new_stmt', 'line', 'out', 'prevchar', 'i', 'char', 'next_char')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
          name       'eat_spaces'
-         firstlineno 130
+         firstlineno 134
          lnotab
             0x0202040108011e0204014c0102013e01120108ff08030c0110010c0202
             020a0206012c01
       '#'
       'symbol'
       code
          argcount  : 2
@@ -1135,78 +1164,78 @@
             0000000000a6000000ab0000000000000000007d047c04a0050000000000
             000000000000000000000000000000a6000000ab00000000000000000064
             026b020000000072018c4f7c02a006000000000000000000000000000000
             00000000007c04a6010000ab01000000000000000001007c03a006000000
             00000000000000000000000000000000007c05a6010000ab010000000000
             00000001008c7a740f000000000000000000007c027c03a6020000ab0200
             000000000000005300
-         157           0 RESUME                   0
+         161           0 RESUME                   0
          
-         161           2 BUILD_LIST               0
+         165           2 BUILD_LIST               0
                        4 STORE_FAST               2 (new_stmt)
          
-         162           6 BUILD_LIST               0
+         166           6 BUILD_LIST               0
                        8 STORE_FAST               3 (new_lines)
          
-         163          10 LOAD_GLOBAL              1 (NULL + zip)
+         167          10 LOAD_GLOBAL              1 (NULL + zip)
                       22 LOAD_FAST                0 (stmts)
                       24 LOAD_ATTR                1 (stmt)
                       34 LOAD_FAST                0 (stmts)
                       36 LOAD_ATTR                2 (lines)
                       46 PRECALL                  2
                       50 CALL                     2
                       60 GET_ITER
                  >>   62 FOR_ITER               121 (to 306)
                       64 UNPACK_SEQUENCE          2
                       68 STORE_FAST               4 (line)
                       70 STORE_FAST               5 (lines_span)
          
-         165          72 LOAD_FAST                1 (symbol)
+         169          72 LOAD_FAST                1 (symbol)
                       74 LOAD_FAST                4 (line)
                       76 CONTAINS_OP              0
                       78 POP_JUMP_FORWARD_IF_FALSE    70 (to 220)
          
-         166          80 LOAD_FAST                4 (line)
+         170          80 LOAD_FAST                4 (line)
                       82 LOAD_METHOD              3 (split)
                      104 LOAD_FAST                1 (symbol)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               1 (0)
                      122 BINARY_SUBSCR
                      132 LOAD_METHOD              4 (rstrip)
                      154 PRECALL                  0
                      158 CALL                     0
                      168 STORE_FAST               4 (line)
          
-         167         170 LOAD_FAST                4 (line)
+         171         170 LOAD_FAST                4 (line)
                      172 LOAD_METHOD              5 (strip)
                      194 PRECALL                  0
                      198 CALL                     0
                      208 LOAD_CONST               2 ('')
                      210 COMPARE_OP               2 (==)
                      216 POP_JUMP_FORWARD_IF_FALSE     1 (to 220)
          
-         168         218 JUMP_BACKWARD           79 (to 62)
+         172         218 JUMP_BACKWARD           79 (to 62)
          
-         169     >>  220 LOAD_FAST                2 (new_stmt)
+         173     >>  220 LOAD_FAST                2 (new_stmt)
                      222 LOAD_METHOD              6 (append)
                      244 LOAD_FAST                4 (line)
                      246 PRECALL                  1
                      250 CALL                     1
                      260 POP_TOP
          
-         170         262 LOAD_FAST                3 (new_lines)
+         174         262 LOAD_FAST                3 (new_lines)
                      264 LOAD_METHOD              6 (append)
                      286 LOAD_FAST                5 (lines_span)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 POP_TOP
                      304 JUMP_BACKWARD          122 (to 62)
          
-         172     >>  306 LOAD_GLOBAL             15 (NULL + Statements)
+         176     >>  306 LOAD_GLOBAL             15 (NULL + Statements)
                      318 LOAD_FAST                2 (new_stmt)
                      320 LOAD_FAST                3 (new_lines)
                      322 PRECALL                  2
                      326 CALL                     2
                      336 RETURN_VALUE
          consts
             '\n   \n    '
@@ -1214,15 +1243,15 @@
             ''
          names      ('zip', 'stmt', 'lines', 'split', 'rstrip', 'strip', 'append', 'Statements')
          varnames   ('stmts', 'symbol', 'new_stmt', 'new_lines', 'line', 'lines_span')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
          name       'clean_inline_comments'
-         firstlineno 157
+         firstlineno 161
          lnotab 0x0204040104013e0208015a01300102012a012c02
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 4
          flags     : 16777219
          code
@@ -1230,74 +1259,74 @@
             00000000007c006a020000000000000000a6020000ab0200000000000000
             0044005d455c0200007d047d057c04a00300000000000000000000000000
             000000000000007c01a6010000ab01000000000000000072018c1b7c02a0
             0400000000000000000000000000000000000000007c04a6010000ab0100
             0000000000000001007c03a0040000000000000000000000000000000000
             0000007c05a6010000ab01000000000000000001008c46740b0000000000
             00000000007c027c03a6020000ab0200000000000000005300
-         174           0 RESUME                   0
+         178           0 RESUME                   0
          
-         178           2 BUILD_LIST               0
+         182           2 BUILD_LIST               0
                        4 STORE_FAST               2 (new_stmt)
          
-         179           6 BUILD_LIST               0
+         183           6 BUILD_LIST               0
                        8 STORE_FAST               3 (new_lines)
          
-         180          10 LOAD_GLOBAL              1 (NULL + zip)
+         184          10 LOAD_GLOBAL              1 (NULL + zip)
                       22 LOAD_FAST                0 (stmts)
                       24 LOAD_ATTR                1 (stmt)
                       34 LOAD_FAST                0 (stmts)
                       36 LOAD_ATTR                2 (lines)
                       46 PRECALL                  2
                       50 CALL                     2
                       60 GET_ITER
                  >>   62 FOR_ITER                69 (to 202)
                       64 UNPACK_SEQUENCE          2
                       68 STORE_FAST               4 (line)
                       70 STORE_FAST               5 (lines_span)
          
-         181          72 LOAD_FAST                4 (line)
+         185          72 LOAD_FAST                4 (line)
                       74 LOAD_METHOD              3 (startswith)
                       96 LOAD_FAST                1 (symbol)
                       98 PRECALL                  1
                      102 CALL                     1
                      112 POP_JUMP_FORWARD_IF_FALSE     1 (to 116)
          
-         182         114 JUMP_BACKWARD           27 (to 62)
+         186         114 JUMP_BACKWARD           27 (to 62)
          
-         183     >>  116 LOAD_FAST                2 (new_stmt)
+         187     >>  116 LOAD_FAST                2 (new_stmt)
                      118 LOAD_METHOD              4 (append)
                      140 LOAD_FAST                4 (line)
                      142 PRECALL                  1
                      146 CALL                     1
                      156 POP_TOP
          
-         184         158 LOAD_FAST                3 (new_lines)
+         188         158 LOAD_FAST                3 (new_lines)
                      160 LOAD_METHOD              4 (append)
                      182 LOAD_FAST                5 (lines_span)
                      184 PRECALL                  1
                      188 CALL                     1
                      198 POP_TOP
                      200 JUMP_BACKWARD           70 (to 62)
          
-         185     >>  202 LOAD_GLOBAL             11 (NULL + Statements)
+         189     >>  202 LOAD_GLOBAL             11 (NULL + Statements)
                      214 LOAD_FAST                2 (new_stmt)
                      216 LOAD_FAST                3 (new_lines)
                      218 PRECALL                  2
                      222 CALL                     2
                      232 RETURN_VALUE
          consts
             '\n   \n    '
          names      ('zip', 'stmt', 'lines', 'startswith', 'append', 'Statements')
          varnames   ('stmts', 'symbol', 'new_stmt', 'new_lines', 'line', 'lines_span')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
          name       'clean_pure_comments'
-         firstlineno 174
+         firstlineno 178
          lnotab 0x0204040104013e012a0102012a012c01
       code
          argcount  : 1
          nlocals   : 8
          stacksize : 7
          flags     : 16777219
          code
@@ -1311,114 +1340,114 @@
             0500000000000000000000000000000000000000006401a6010000ab0100
             0000000000000044005d437d077c01a00300000000000000000000000000
             000000000000007c067c07a0060000000000000000000000000000000000
             000000a6000000ab0000000000000000007a000000a6010000ab01000000
             000000000001007c02a00300000000000000000000000000000000000000
             007c047c056702a6010000ab01000000000000000001008c448ca2740f00
             0000000000000000007c017c02a6020000ab0200000000000000005300
-         188           0 RESUME                   0
+         192           0 RESUME                   0
          
-         190           2 BUILD_LIST               0
+         194           2 BUILD_LIST               0
                        4 STORE_FAST               1 (new_stmt)
          
-         191           6 BUILD_LIST               0
+         195           6 BUILD_LIST               0
                        8 STORE_FAST               2 (new_lines)
          
-         192          10 LOAD_GLOBAL              1 (NULL + zip)
+         196          10 LOAD_GLOBAL              1 (NULL + zip)
                       22 LOAD_FAST                0 (stmts)
                       24 LOAD_ATTR                1 (stmt)
                       34 LOAD_FAST                0 (stmts)
                       36 LOAD_ATTR                2 (lines)
                       46 PRECALL                  2
                       50 CALL                     2
                       60 GET_ITER
                  >>   62 FOR_ITER               161 (to 386)
                       64 UNPACK_SEQUENCE          2
                       68 STORE_FAST               3 (line)
                       70 UNPACK_SEQUENCE          2
                       74 STORE_FAST               4 (lstart)
                       76 STORE_FAST               5 (lend)
          
-         193          78 LOAD_CONST               1 (';')
+         197          78 LOAD_CONST               1 (';')
                       80 LOAD_FAST                3 (line)
                       82 CONTAINS_OP              1
                       84 POP_JUMP_FORWARD_IF_FALSE    45 (to 176)
          
-         194          86 LOAD_FAST                1 (new_stmt)
+         198          86 LOAD_FAST                1 (new_stmt)
                       88 LOAD_METHOD              3 (append)
                      110 LOAD_FAST                3 (line)
                      112 PRECALL                  1
                      116 CALL                     1
                      126 POP_TOP
          
-         195         128 LOAD_FAST                2 (new_lines)
+         199         128 LOAD_FAST                2 (new_lines)
                      130 LOAD_METHOD              3 (append)
                      152 LOAD_FAST                4 (lstart)
                      154 LOAD_FAST                5 (lend)
                      156 BUILD_LIST               2
                      158 PRECALL                  1
                      162 CALL                     1
                      172 POP_TOP
                      174 JUMP_BACKWARD           57 (to 62)
          
-         197     >>  176 LOAD_GLOBAL              9 (NULL + get_indent)
+         201     >>  176 LOAD_GLOBAL              9 (NULL + get_indent)
                      188 LOAD_FAST                3 (line)
                      190 PRECALL                  1
                      194 CALL                     1
                      204 STORE_FAST               6 (indent)
          
-         198         206 LOAD_FAST                3 (line)
+         202         206 LOAD_FAST                3 (line)
                      208 LOAD_METHOD              5 (split)
                      230 LOAD_CONST               1 (';')
                      232 PRECALL                  1
                      236 CALL                     1
                      246 GET_ITER
                  >>  248 FOR_ITER                67 (to 384)
                      250 STORE_FAST               7 (stmt)
          
-         199         252 LOAD_FAST                1 (new_stmt)
+         203         252 LOAD_FAST                1 (new_stmt)
                      254 LOAD_METHOD              3 (append)
                      276 LOAD_FAST                6 (indent)
                      278 LOAD_FAST                7 (stmt)
                      280 LOAD_METHOD              6 (strip)
                      302 PRECALL                  0
                      306 CALL                     0
                      316 BINARY_OP                0 (+)
                      320 PRECALL                  1
                      324 CALL                     1
                      334 POP_TOP
          
-         200         336 LOAD_FAST                2 (new_lines)
+         204         336 LOAD_FAST                2 (new_lines)
                      338 LOAD_METHOD              3 (append)
                      360 LOAD_FAST                4 (lstart)
                      362 LOAD_FAST                5 (lend)
                      364 BUILD_LIST               2
                      366 PRECALL                  1
                      370 CALL                     1
                      380 POP_TOP
                      382 JUMP_BACKWARD           68 (to 248)
          
-         198     >>  384 JUMP_BACKWARD          162 (to 62)
+         202     >>  384 JUMP_BACKWARD          162 (to 62)
          
-         201     >>  386 LOAD_GLOBAL             15 (NULL + Statements)
+         205     >>  386 LOAD_GLOBAL             15 (NULL + Statements)
                      398 LOAD_FAST                1 (new_stmt)
                      400 LOAD_FAST                2 (new_lines)
                      402 PRECALL                  2
                      406 CALL                     2
                      416 RETURN_VALUE
          consts
             'Split statements on ;'
             ';'
          names      ('zip', 'stmt', 'lines', 'append', 'get_indent', 'split', 'strip', 'Statements')
          varnames   ('stmts', 'new_stmt', 'new_lines', 'line', 'lstart', 'lend', 'indent', 'stmt')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
          name       'split_multi_statement_lines'
-         firstlineno 188
+         firstlineno 192
          lnotab 0x020204010401440108012a0130021e012e01540130fe0203
       'markup_in'
       'markup_out'
       code
          argcount  : 3
          nlocals   : 14
          stacksize : 5
@@ -1438,161 +1467,161 @@
             0200000000720864077d087c077c017a0d00007d078c107c0d7c046b0200
             000000720864057d087c077c027a0d00007d078c1e7c077c0d7a0d00007d
             078c247c08732e7c05a00600000000000000000000000000000000000000
             007c07a6010000ab01000000000000000001007c06a00600000000000000
             000000000000000000000000007c0c7c0b6702a6010000ab010000000000
             000000010064047d078ca4740f000000000000000000007c057c06a60200
             00ab0200000000000000005300
-         204           0 RESUME                   0
+         208           0 RESUME                   0
          
-         206           2 LOAD_FAST                1 (markup_in)
+         210           2 LOAD_FAST                1 (markup_in)
                        4 STORE_FAST               3 (proxy_in)
          
-         207           6 LOAD_FAST                2 (markup_out)
+         211           6 LOAD_FAST                2 (markup_out)
                        8 STORE_FAST               4 (proxy_out)
          
-         208          10 LOAD_GLOBAL              1 (NULL + len)
+         212          10 LOAD_GLOBAL              1 (NULL + len)
                       22 LOAD_FAST                1 (markup_in)
                       24 PRECALL                  1
                       28 CALL                     1
                       38 LOAD_CONST               1 (1)
                       40 COMPARE_OP               4 (>)
                       46 POP_JUMP_FORWARD_IF_FALSE     2 (to 52)
          
-         209          48 LOAD_CONST               2 ('ª')
+         213          48 LOAD_CONST               2 ('ª')
                       50 STORE_FAST               3 (proxy_in)
          
-         210     >>   52 LOAD_GLOBAL              1 (NULL + len)
+         214     >>   52 LOAD_GLOBAL              1 (NULL + len)
                       64 LOAD_FAST                2 (markup_out)
                       66 PRECALL                  1
                       70 CALL                     1
                       80 LOAD_CONST               1 (1)
                       82 COMPARE_OP               4 (>)
                       88 POP_JUMP_FORWARD_IF_FALSE     2 (to 94)
          
-         211          90 LOAD_CONST               3 ('»')
+         215          90 LOAD_CONST               3 ('»')
                       92 STORE_FAST               4 (proxy_out)
          
-         213     >>   94 BUILD_LIST               0
+         217     >>   94 BUILD_LIST               0
                       96 STORE_FAST               5 (new_stmt)
          
-         214          98 BUILD_LIST               0
+         218          98 BUILD_LIST               0
                      100 STORE_FAST               6 (new_lines)
          
-         215         102 LOAD_CONST               4 ('')
+         219         102 LOAD_CONST               4 ('')
                      104 STORE_FAST               7 (buffer)
          
-         217         106 LOAD_CONST               5 (False)
+         221         106 LOAD_CONST               5 (False)
                      108 STORE_FAST               8 (in_multiline)
          
-         218         110 LOAD_GLOBAL              3 (NULL + zip)
+         222         110 LOAD_GLOBAL              3 (NULL + zip)
                      122 LOAD_FAST                0 (stmts)
                      124 LOAD_ATTR                2 (stmt)
                      134 LOAD_FAST                0 (stmts)
                      136 LOAD_ATTR                3 (lines)
                      146 PRECALL                  2
                      150 CALL                     2
                      160 GET_ITER
                  >>  162 FOR_ITER               163 (to 490)
                      164 UNPACK_SEQUENCE          2
                      168 STORE_FAST               9 (line)
                      170 UNPACK_SEQUENCE          2
                      174 STORE_FAST              10 (lstart)
                      176 STORE_FAST              11 (lend)
          
-         219         178 LOAD_FAST                8 (in_multiline)
+         223         178 LOAD_FAST                8 (in_multiline)
                      180 POP_JUMP_FORWARD_IF_FALSE    23 (to 228)
          
-         220         182 LOAD_CONST               6 (' ')
+         224         182 LOAD_CONST               6 (' ')
                      184 LOAD_FAST                9 (line)
                      186 LOAD_METHOD              4 (lstrip)
                      208 PRECALL                  0
                      212 CALL                     0
                      222 BINARY_OP                0 (+)
                      226 STORE_FAST               9 (line)
          
-         222     >>  228 LOAD_FAST                8 (in_multiline)
+         226     >>  228 LOAD_FAST                8 (in_multiline)
                      230 POP_JUMP_FORWARD_IF_TRUE     2 (to 236)
          
-         223         232 LOAD_FAST               10 (lstart)
+         227         232 LOAD_FAST               10 (lstart)
                      234 STORE_FAST              12 (last_start)
          
-         226     >>  236 LOAD_FAST                9 (line)
+         230     >>  236 LOAD_FAST                9 (line)
                      238 LOAD_METHOD              5 (replace)
                      260 LOAD_FAST                1 (markup_in)
                      262 LOAD_FAST                3 (proxy_in)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 LOAD_METHOD              5 (replace)
                      300 LOAD_FAST                2 (markup_out)
                      302 LOAD_FAST                4 (proxy_out)
                      304 PRECALL                  2
                      308 CALL                     2
                      318 GET_ITER
                  >>  320 FOR_ITER                35 (to 392)
                      322 STORE_FAST              13 (char)
          
-         227         324 LOAD_FAST               13 (char)
+         231         324 LOAD_FAST               13 (char)
                      326 LOAD_FAST                3 (proxy_in)
                      328 COMPARE_OP               2 (==)
                      334 POP_JUMP_FORWARD_IF_FALSE     8 (to 352)
          
-         228         336 LOAD_CONST               7 (True)
+         232         336 LOAD_CONST               7 (True)
                      338 STORE_FAST               8 (in_multiline)
          
-         229         340 LOAD_FAST                7 (buffer)
+         233         340 LOAD_FAST                7 (buffer)
                      342 LOAD_FAST                1 (markup_in)
                      344 BINARY_OP               13 (+=)
                      348 STORE_FAST               7 (buffer)
                      350 JUMP_BACKWARD           16 (to 320)
          
-         230     >>  352 LOAD_FAST               13 (char)
+         234     >>  352 LOAD_FAST               13 (char)
                      354 LOAD_FAST                4 (proxy_out)
                      356 COMPARE_OP               2 (==)
                      362 POP_JUMP_FORWARD_IF_FALSE     8 (to 380)
          
-         231         364 LOAD_CONST               5 (False)
+         235         364 LOAD_CONST               5 (False)
                      366 STORE_FAST               8 (in_multiline)
          
-         232         368 LOAD_FAST                7 (buffer)
+         236         368 LOAD_FAST                7 (buffer)
                      370 LOAD_FAST                2 (markup_out)
                      372 BINARY_OP               13 (+=)
                      376 STORE_FAST               7 (buffer)
                      378 JUMP_BACKWARD           30 (to 320)
          
-         234     >>  380 LOAD_FAST                7 (buffer)
+         238     >>  380 LOAD_FAST                7 (buffer)
                      382 LOAD_FAST               13 (char)
                      384 BINARY_OP               13 (+=)
                      388 STORE_FAST               7 (buffer)
                      390 JUMP_BACKWARD           36 (to 320)
          
-         237     >>  392 LOAD_FAST                8 (in_multiline)
+         241     >>  392 LOAD_FAST                8 (in_multiline)
                      394 POP_JUMP_FORWARD_IF_TRUE    46 (to 488)
          
-         238         396 LOAD_FAST                5 (new_stmt)
+         242         396 LOAD_FAST                5 (new_stmt)
                      398 LOAD_METHOD              6 (append)
                      420 LOAD_FAST                7 (buffer)
                      422 PRECALL                  1
                      426 CALL                     1
                      436 POP_TOP
          
-         239         438 LOAD_FAST                6 (new_lines)
+         243         438 LOAD_FAST                6 (new_lines)
                      440 LOAD_METHOD              6 (append)
                      462 LOAD_FAST               12 (last_start)
                      464 LOAD_FAST               11 (lend)
                      466 BUILD_LIST               2
                      468 PRECALL                  1
                      472 CALL                     1
                      482 POP_TOP
          
-         240         484 LOAD_CONST               4 ('')
+         244         484 LOAD_CONST               4 ('')
                      486 STORE_FAST               7 (buffer)
                  >>  488 JUMP_BACKWARD          164 (to 162)
          
-         243     >>  490 LOAD_GLOBAL             15 (NULL + Statements)
+         247     >>  490 LOAD_GLOBAL             15 (NULL + Statements)
                      502 LOAD_FAST                5 (new_stmt)
                      504 LOAD_FAST                6 (new_lines)
                      506 PRECALL                  2
                      510 CALL                     2
                      520 RETURN_VALUE
          consts
             None
@@ -1605,92 +1634,313 @@
             True
          names      ('len', 'zip', 'stmt', 'lines', 'lstrip', 'replace', 'append', 'Statements')
          varnames   ('stmts', 'markup_in', 'markup_out', 'proxy_in', 'proxy_out', 'new_stmt', 'new_lines', 'buffer', 'in_multiline', 'line', 'lstart', 'lend', 'last_start', 'char')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
          name       'align_multiline_blocks'
-         firstlineno 204
+         firstlineno 208
          lnotab
             0x02020401040126010401260104020401040104020401440104012e0204
             01040358010c0104010c010c0104010c020c0304012a012e010603
       'line'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 3
          flags     : 16777219
          code
             0x970064017d017c0044005d1b7d027c0264026b020000000072067c0164
             037a0d00007d018c0e7c0264046b0300000000720201006e067c0164047a
             0d00007d018c1c7c015300
-         245           0 RESUME                   0
+         249           0 RESUME                   0
          
-         246           2 LOAD_CONST               1 ('')
+         250           2 LOAD_CONST               1 ('')
                        4 STORE_FAST               1 (_indent)
          
-         247           6 LOAD_FAST                0 (line)
+         251           6 LOAD_FAST                0 (line)
                        8 GET_ITER
                  >>   10 FOR_ITER                27 (to 66)
                       12 STORE_FAST               2 (char)
          
-         248          14 LOAD_FAST                2 (char)
+         252          14 LOAD_FAST                2 (char)
                       16 LOAD_CONST               2 ('\t')
                       18 COMPARE_OP               2 (==)
                       24 POP_JUMP_FORWARD_IF_FALSE     6 (to 38)
          
-         249          26 LOAD_FAST                1 (_indent)
+         253          26 LOAD_FAST                1 (_indent)
                       28 LOAD_CONST               3 ('    ')
                       30 BINARY_OP               13 (+=)
                       34 STORE_FAST               1 (_indent)
                       36 JUMP_BACKWARD           14 (to 10)
          
-         250     >>   38 LOAD_FAST                2 (char)
+         254     >>   38 LOAD_FAST                2 (char)
                       40 LOAD_CONST               4 (' ')
                       42 COMPARE_OP               3 (!=)
                       48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
          
-         251          50 POP_TOP
+         255          50 POP_TOP
                       52 JUMP_FORWARD             6 (to 66)
          
-         253     >>   54 LOAD_FAST                1 (_indent)
+         257     >>   54 LOAD_FAST                1 (_indent)
                       56 LOAD_CONST               4 (' ')
                       58 BINARY_OP               13 (+=)
                       62 STORE_FAST               1 (_indent)
                       64 JUMP_BACKWARD           28 (to 10)
          
-         254     >>   66 LOAD_FAST                1 (_indent)
+         258     >>   66 LOAD_FAST                1 (_indent)
                       68 RETURN_VALUE
          consts
             None
             ''
             '\t'
             '    '
             ' '
          names      ()
          varnames   ('line', '_indent', 'char')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
          name       'get_indent'
-         firstlineno 245
+         firstlineno 249
          lnotab 0x0201040108010c010c010c0104020c01
+      False
+      'fortran'
+      'bool'
+      code
+         argcount  : 2
+         nlocals   : 6
+         stacksize : 4
+         flags     : 16777219
+         code
+            0x970064017d0264027d037c00a000000000000000000000000000000000
+            00000000006403740200000000000000000000a6020000ab020000000000
+            000000a00000000000000000000000000000000000000000006404740400
+            000000000000000000a6020000ab020000000000000000a0000000000000
+            0000000000000000000000000000006405740600000000000000000000a6
+            020000ab0200000000000000007d047c0444005d5e7d057c057408000000
+            000000000000006b0200000000720e7c027c057a0d00007d027c0364066b
+            0200000000720264027d038c1b7c057404000000000000000000006b0200
+            00000072057c03810364077d038c2b7c057406000000000000000000006b
+            020000000072057c03810364027d038c3b7c057402000000000000000000
+            006b0200000000720f7c0364027500720b7c01730364067d038c4f7c027c
+            057a0d00007d028c557c036402750072057c027c057a0d00007d028c5f7c
+            02a000000000000000000000000000000000000000000074020000000000
+            00000000006403a6020000ab0200000000000000007d027c025300
+         262           0 RESUME                   0
+         
+         266           2 LOAD_CONST               1 ('')
+                       4 STORE_FAST               2 (cline)
+         
+         267           6 LOAD_CONST               2 (True)
+                       8 STORE_FAST               3 (read)
+         
+         268          10 LOAD_FAST                0 (line)
+                      12 LOAD_METHOD              0 (replace)
+                      34 LOAD_CONST               3 ('//')
+                      36 LOAD_GLOBAL              2 (CHAR_CMT_EOL)
+                      48 PRECALL                  2
+                      52 CALL                     2
+                      62 LOAD_METHOD              0 (replace)
+                      84 LOAD_CONST               4 ('/*')
+                      86 LOAD_GLOBAL              4 (CHAR_CMT_START)
+                      98 PRECALL                  2
+                     102 CALL                     2
+                     112 LOAD_METHOD              0 (replace)
+                     134 LOAD_CONST               5 ('*/')
+                     136 LOAD_GLOBAL              6 (CHAR_CMT_STOP)
+                     148 PRECALL                  2
+                     152 CALL                     2
+                     162 STORE_FAST               4 (_line)
+         
+         269         164 LOAD_FAST                4 (_line)
+                     166 GET_ITER
+                 >>  168 FOR_ITER                94 (to 358)
+                     170 STORE_FAST               5 (char)
+         
+         270         172 LOAD_FAST                5 (char)
+                     174 LOAD_GLOBAL              8 (CHAR_EOL)
+                     186 COMPARE_OP               2 (==)
+                     192 POP_JUMP_FORWARD_IF_FALSE    14 (to 222)
+         
+         271         194 LOAD_FAST                2 (cline)
+                     196 LOAD_FAST                5 (char)
+                     198 BINARY_OP               13 (+=)
+                     202 STORE_FAST               2 (cline)
+         
+         272         204 LOAD_FAST                3 (read)
+                     206 LOAD_CONST               6 (None)
+                     208 COMPARE_OP               2 (==)
+                     214 POP_JUMP_FORWARD_IF_FALSE     2 (to 220)
+         
+         273         216 LOAD_CONST               2 (True)
+                     218 STORE_FAST               3 (read)
+                 >>  220 JUMP_BACKWARD           27 (to 168)
+         
+         274     >>  222 LOAD_FAST                5 (char)
+                     224 LOAD_GLOBAL              4 (CHAR_CMT_START)
+                     236 COMPARE_OP               2 (==)
+                     242 POP_JUMP_FORWARD_IF_FALSE     5 (to 254)
+                     244 LOAD_FAST                3 (read)
+                     246 POP_JUMP_FORWARD_IF_NONE     3 (to 254)
+         
+         275         248 LOAD_CONST               7 (False)
+                     250 STORE_FAST               3 (read)
+                     252 JUMP_BACKWARD           43 (to 168)
+         
+         276     >>  254 LOAD_FAST                5 (char)
+                     256 LOAD_GLOBAL              6 (CHAR_CMT_STOP)
+                     268 COMPARE_OP               2 (==)
+                     274 POP_JUMP_FORWARD_IF_FALSE     5 (to 286)
+                     276 LOAD_FAST                3 (read)
+                     278 POP_JUMP_FORWARD_IF_NONE     3 (to 286)
+         
+         277         280 LOAD_CONST               2 (True)
+                     282 STORE_FAST               3 (read)
+                     284 JUMP_BACKWARD           59 (to 168)
+         
+         278     >>  286 LOAD_FAST                5 (char)
+                     288 LOAD_GLOBAL              2 (CHAR_CMT_EOL)
+                     300 COMPARE_OP               2 (==)
+                     306 POP_JUMP_FORWARD_IF_FALSE    15 (to 338)
+                     308 LOAD_FAST                3 (read)
+                     310 LOAD_CONST               2 (True)
+                     312 IS_OP                    0
+                     314 POP_JUMP_FORWARD_IF_FALSE    11 (to 338)
+         
+         279         316 LOAD_FAST                1 (fortran)
+                     318 POP_JUMP_FORWARD_IF_TRUE     3 (to 326)
+         
+         280         320 LOAD_CONST               6 (None)
+                     322 STORE_FAST               3 (read)
+                     324 JUMP_BACKWARD           79 (to 168)
+         
+         282     >>  326 LOAD_FAST                2 (cline)
+                     328 LOAD_FAST                5 (char)
+                     330 BINARY_OP               13 (+=)
+                     334 STORE_FAST               2 (cline)
+                     336 JUMP_BACKWARD           85 (to 168)
+         
+         284     >>  338 LOAD_FAST                3 (read)
+                     340 LOAD_CONST               2 (True)
+                     342 IS_OP                    0
+                     344 POP_JUMP_FORWARD_IF_FALSE     5 (to 356)
+         
+         285         346 LOAD_FAST                2 (cline)
+                     348 LOAD_FAST                5 (char)
+                     350 BINARY_OP               13 (+=)
+                     354 STORE_FAST               2 (cline)
+                 >>  356 JUMP_BACKWARD           95 (to 168)
+         
+         287     >>  358 LOAD_FAST                2 (cline)
+                     360 LOAD_METHOD              0 (replace)
+                     382 LOAD_GLOBAL              2 (CHAR_CMT_EOL)
+                     394 LOAD_CONST               3 ('//')
+                     396 PRECALL                  2
+                     400 CALL                     2
+                     410 STORE_FAST               2 (cline)
+         
+         288         412 LOAD_FAST                2 (cline)
+                     414 RETURN_VALUE
+         consts
+            '\n    Fortran=True :  equivalent to cpp --traditional\n    '
+            ''
+            True
+            '//'
+            '/*'
+            '*/'
+            None
+            False
+         names      ('replace', 'CHAR_CMT_EOL', 'CHAR_CMT_START', 'CHAR_CMT_STOP', 'CHAR_EOL')
+         varnames   ('line', 'fortran', 'cline', 'read', '_line', 'char')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
+         name       'strip_c_comment'
+         firstlineno 262
+         lnotab
+            0x0204040104019a01080116010a010c0106011a0106011a0106011e0104
+            0106020c0208010c023601
+      'lines'
+      code
+         argcount  : 2
+         nlocals   : 4
+         stacksize : 4
+         flags     : 16777219
+         code
+            0x9700740000000000000000000000a00100000000000000000000000000
+            000000000000007c00a6010000ab0100000000000000007d027405000000
+            000000000000007c027c01ac01a6020000ab020000000000000000a00300
+            000000000000000000000000000000000000007400000000000000000000
+            00a6010000ab0100000000000000007d037409000000000000000000007c
+            00a6010000ab0100000000000000007409000000000000000000007c03a6
+            010000ab0100000000000000006b020000000073024a0082017c035300
+         291           0 RESUME                   0
+         
+         292           2 LOAD_GLOBAL              0 (CHAR_EOL)
+                      14 LOAD_METHOD              1 (join)
+                      36 LOAD_FAST                0 (lines)
+                      38 PRECALL                  1
+                      42 CALL                     1
+                      52 STORE_FAST               2 (raw)
+         
+         293          54 LOAD_GLOBAL              5 (NULL + strip_c_comment)
+                      66 LOAD_FAST                2 (raw)
+                      68 LOAD_FAST                1 (fortran)
+                      70 KW_NAMES                 1
+                      72 PRECALL                  2
+                      76 CALL                     2
+                      86 LOAD_METHOD              3 (split)
+                     108 LOAD_GLOBAL              0 (CHAR_EOL)
+                     120 PRECALL                  1
+                     124 CALL                     1
+                     134 STORE_FAST               3 (out)
+         
+         294         136 LOAD_GLOBAL              9 (NULL + len)
+                     148 LOAD_FAST                0 (lines)
+                     150 PRECALL                  1
+                     154 CALL                     1
+                     164 LOAD_GLOBAL              9 (NULL + len)
+                     176 LOAD_FAST                3 (out)
+                     178 PRECALL                  1
+                     182 CALL                     1
+                     192 COMPARE_OP               2 (==)
+                     198 POP_JUMP_FORWARD_IF_TRUE     2 (to 204)
+                     200 LOAD_ASSERTION_ERROR
+                     202 RAISE_VARARGS            1
+         
+         295     >>  204 LOAD_FAST                3 (out)
+                     206 RETURN_VALUE
+         consts
+            None
+            ('fortran',)
+         names      ('CHAR_EOL', 'join', 'strip_c_comment', 'split', 'len')
+         varnames   ('lines', 'fortran', 'raw', 'out')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
+         name       'clean_c_comments'
+         firstlineno 291
+         lnotab 0x0201340152014401
       ('code', 'List[str]', 'return', 'Statements')
       ('code', 'List[str]', 'string_char', 'str', 'return', 'List[str]')
       ('(', ')', True)
       ('buffer', 'str', 'lchar', 'str', 'rchar', 'str', 'return', 'str')
       ('stmts', 'Statements', 'return', 'Statements')
       ('code', 'List[str]', 'return', 'List[str]')
       ('#',)
       ('stmts', 'Statements', 'symbol', 'str', 'return', 'Statements')
       ('stmts', 'Statements', 'markup_in', 'str', 'markup_out', 'str', 'return', 'Statements')
       ('line', 'str', 'return', 'str')
-   names      ('__doc__', '__future__', 'annotations', 'typing', 'Tuple', 'List', 'dataclasses', 'dataclass', 'loguru', 'logger', 'json', 'Statements', 'new_stmts', 'remove_strings', 'rm_parenthesis_content', 'clean_blanks', 'eat_spaces', 'clean_inline_comments', 'clean_pure_comments', 'split_multi_statement_lines', 'align_multiline_blocks', 'get_indent')
+      (False,)
+      ('line', 'str', 'fortran', 'bool', 'return', 'str')
+      ('lines', 'List[str]', 'fortran', 'bool', 'return', 'List[str]')
+   names      ('__doc__', '__future__', 'annotations', 'typing', 'Tuple', 'List', 'dataclasses', 'dataclass', 'loguru', 'logger', 'json', 'CHAR_CMT_START', 'CHAR_CMT_STOP', 'CHAR_EOL', 'CHAR_CMT_EOL', 'Statements', 'new_stmts', 'remove_strings', 'rm_parenthesis_content', 'clean_blanks', 'eat_spaces', 'clean_inline_comments', 'clean_pure_comments', 'split_multi_statement_lines', 'align_multiline_blocks', 'get_indent', 'strip_c_comment', 'clean_c_comments')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_common.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020104040c0110010c010c010803020118ff0e0102210807081d0a
-      13081d081b0a110a0e08100829
+      0x00ff020104040c0110010c010c0108020401040104010402020118ff0e
+      0102210807081d0a13081d081b0a110a0e08100829080d0a1d
```

### Comparing `tucan-0.1.0/src/tucan/__pycache__/unformat_ftn.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/unformat_ftn.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xdbbab365 (Fri Jan 26 13:59:55 2024 UTC)
-files sz: 15668
+moddate:  0x232e3a66 (Tue May  7 13:35:31 2024 UTC)
+files sz: 15078
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -15,16 +15,18 @@
       14640b6515640665166604640c84045a17640d6501651519000000000000
       000000640665016515190000000000000000006604640e84045a18640565
       07640665076604640f84045a19640d650165151900000000000000000064
       0665016515190000000000000000006604641084045a1a640d6501651519
       000000000000000000640665016515190000000000000000006604641184
       045a1b640d65016515190000000000000000006406650165151900000000
       00000000006604641284045a1c640d650165151900000000000000000064
-      0665016515190000000000000000006604641384045a1d64146501651519
-      000000000000000000640665076604641584045a1e64165300
+      0665016515190000000000000000006604641384045a1d640d6501651519
+      000000000000000000640665016515190000000000000000006604641484
+      045a1e64156501651519000000000000000000640665076604641684045a
+      1f64175300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('List',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (List)
                 10 STORE_NAME               1 (List)
@@ -83,127 +85,140 @@
                106 LOAD_CONST               6 ('return')
                108 LOAD_NAME                7 (Statements)
                110 BUILD_TUPLE              4
                112 LOAD_CONST               8 (<code object align_start_continuations, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 42>)
                114 MAKE_FUNCTION            4 (annotations)
                116 STORE_NAME              18 (align_start_continuations)
    
-    69         118 LOAD_CONST               5 ('stmts')
+    72         118 LOAD_CONST               5 ('stmts')
                120 LOAD_NAME                7 (Statements)
                122 LOAD_CONST               6 ('return')
                124 LOAD_NAME                7 (Statements)
                126 BUILD_TUPLE              4
-               128 LOAD_CONST               9 (<code object ftn_align_labelled_continuations, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 69>)
+               128 LOAD_CONST               9 (<code object ftn_align_labelled_continuations, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 72>)
                130 MAKE_FUNCTION            4 (annotations)
                132 STORE_NAME              19 (ftn_align_labelled_continuations)
    
-   106         134 LOAD_CONST               5 ('stmts')
+    98         134 LOAD_CONST               5 ('stmts')
                136 LOAD_NAME                7 (Statements)
                138 LOAD_CONST               6 ('return')
                140 LOAD_NAME                7 (Statements)
                142 BUILD_TUPLE              4
-               144 LOAD_CONST              10 (<code object ftn_make_oneliners_conditionals_multilines, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 106>)
+               144 LOAD_CONST              10 (<code object ftn_make_oneliners_conditionals_multilines, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 98>)
                146 MAKE_FUNCTION            4 (annotations)
                148 STORE_NAME              20 (ftn_make_oneliners_conditionals_multilines)
    
-   167         150 LOAD_CONST              11 ('line')
+   151         150 LOAD_CONST              11 ('line')
                152 LOAD_NAME               21 (str)
                154 LOAD_CONST               6 ('return')
                156 LOAD_NAME               22 (list)
                158 BUILD_TUPLE              4
-               160 LOAD_CONST              12 (<code object split_oneliner, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 167>)
+               160 LOAD_CONST              12 (<code object split_oneliner, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 151>)
                162 MAKE_FUNCTION            4 (annotations)
                164 STORE_NAME              23 (split_oneliner)
    
-   198         166 LOAD_CONST              13 ('lines')
+   182         166 LOAD_CONST              13 ('lines')
                168 LOAD_NAME                1 (List)
                170 LOAD_NAME               21 (str)
                172 BINARY_SUBSCR
                182 LOAD_CONST               6 ('return')
                184 LOAD_NAME                1 (List)
                186 LOAD_NAME               21 (str)
                188 BINARY_SUBSCR
                198 BUILD_TUPLE              4
-               200 LOAD_CONST              14 (<code object ftn_remove_space_in_front_of_variables, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 198>)
+               200 LOAD_CONST              14 (<code object ftn_remove_space_in_front_of_variables, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 182>)
                202 MAKE_FUNCTION            4 (annotations)
                204 STORE_NAME              24 (ftn_remove_space_in_front_of_variables)
    
-   230         206 LOAD_CONST               5 ('stmts')
+   214         206 LOAD_CONST               5 ('stmts')
                208 LOAD_NAME                7 (Statements)
                210 LOAD_CONST               6 ('return')
                212 LOAD_NAME                7 (Statements)
                214 BUILD_TUPLE              4
-               216 LOAD_CONST              15 (<code object ftn_clean_labelled_loops_oldftn, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 230>)
+               216 LOAD_CONST              15 (<code object ftn_clean_labelled_loops_oldftn, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 214>)
                218 MAKE_FUNCTION            4 (annotations)
                220 STORE_NAME              25 (ftn_clean_labelled_loops_oldftn)
    
-   292         222 LOAD_CONST              13 ('lines')
+   276         222 LOAD_CONST              13 ('lines')
                224 LOAD_NAME                1 (List)
                226 LOAD_NAME               21 (str)
                228 BINARY_SUBSCR
                238 LOAD_CONST               6 ('return')
                240 LOAD_NAME                1 (List)
                242 LOAD_NAME               21 (str)
                244 BINARY_SUBSCR
                254 BUILD_TUPLE              4
-               256 LOAD_CONST              16 (<code object ftn_suppress_goto_references, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 292>)
+               256 LOAD_CONST              16 (<code object ftn_suppress_goto_references, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 276>)
                258 MAKE_FUNCTION            4 (annotations)
                260 STORE_NAME              26 (ftn_suppress_goto_references)
    
-   307         262 LOAD_CONST              13 ('lines')
+   291         262 LOAD_CONST              13 ('lines')
                264 LOAD_NAME                1 (List)
                266 LOAD_NAME               21 (str)
                268 BINARY_SUBSCR
                278 LOAD_CONST               6 ('return')
                280 LOAD_NAME                1 (List)
                282 LOAD_NAME               21 (str)
                284 BINARY_SUBSCR
                294 BUILD_TUPLE              4
-               296 LOAD_CONST              17 (<code object ftn_clean_labelled_loops_newftn, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 307>)
+               296 LOAD_CONST              17 (<code object ftn_clean_labelled_loops_newftn, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 291>)
                298 MAKE_FUNCTION            4 (annotations)
                300 STORE_NAME              27 (ftn_clean_labelled_loops_newftn)
    
-   339         302 LOAD_CONST              13 ('lines')
+   332         302 LOAD_CONST              13 ('lines')
                304 LOAD_NAME                1 (List)
                306 LOAD_NAME               21 (str)
                308 BINARY_SUBSCR
                318 LOAD_CONST               6 ('return')
                320 LOAD_NAME                1 (List)
                322 LOAD_NAME               21 (str)
                324 BINARY_SUBSCR
                334 BUILD_TUPLE              4
-               336 LOAD_CONST              18 (<code object ftn_clean_intrinsics_declarations, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 339>)
+               336 LOAD_CONST              18 (<code object ftn_clean_operators, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 332>)
                338 MAKE_FUNCTION            4 (annotations)
-               340 STORE_NAME              28 (ftn_clean_intrinsics_declarations)
+               340 STORE_NAME              28 (ftn_clean_operators)
    
-   414         342 LOAD_CONST              13 ('lines')
+   346         342 LOAD_CONST              13 ('lines')
                344 LOAD_NAME                1 (List)
                346 LOAD_NAME               21 (str)
                348 BINARY_SUBSCR
                358 LOAD_CONST               6 ('return')
                360 LOAD_NAME                1 (List)
                362 LOAD_NAME               21 (str)
                364 BINARY_SUBSCR
                374 BUILD_TUPLE              4
-               376 LOAD_CONST              19 (<code object ftn_old_fix_end_multiline, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 414>)
+               376 LOAD_CONST              19 (<code object ftn_clean_intrinsics_declarations, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 346>)
                378 MAKE_FUNCTION            4 (annotations)
-               380 STORE_NAME              29 (ftn_old_fix_end_multiline)
+               380 STORE_NAME              29 (ftn_clean_intrinsics_declarations)
    
-   455         382 LOAD_CONST              20 ('code')
+   416         382 LOAD_CONST              13 ('lines')
                384 LOAD_NAME                1 (List)
                386 LOAD_NAME               21 (str)
                388 BINARY_SUBSCR
                398 LOAD_CONST               6 ('return')
-               400 LOAD_NAME                7 (Statements)
-               402 BUILD_TUPLE              4
-               404 LOAD_CONST              21 (<code object unformat_ftn, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 455>)
-               406 MAKE_FUNCTION            4 (annotations)
-               408 STORE_NAME              30 (unformat_ftn)
-               410 LOAD_CONST              22 (None)
-               412 RETURN_VALUE
+               400 LOAD_NAME                1 (List)
+               402 LOAD_NAME               21 (str)
+               404 BINARY_SUBSCR
+               414 BUILD_TUPLE              4
+               416 LOAD_CONST              20 (<code object ftn_clean_type_keywords, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 416>)
+               418 MAKE_FUNCTION            4 (annotations)
+               420 STORE_NAME              30 (ftn_clean_type_keywords)
+   
+   439         422 LOAD_CONST              21 ('code')
+               424 LOAD_NAME                1 (List)
+               426 LOAD_NAME               21 (str)
+               428 BINARY_SUBSCR
+               438 LOAD_CONST               6 ('return')
+               440 LOAD_NAME                7 (Statements)
+               442 BUILD_TUPLE              4
+               444 LOAD_CONST              22 (<code object unformat_ftn, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 439>)
+               446 MAKE_FUNCTION            4 (annotations)
+               448 STORE_NAME              31 (unformat_ftn)
+               450 LOAD_CONST              23 (None)
+               452 RETURN_VALUE
    consts
       0
       ('List',)
       ('logger',)
       ('KEYWORDS_FTN',)
       ('Statements', 'new_stmts', 'remove_strings', 'clean_blanks', 'clean_inline_comments', 'clean_pure_comments', 'align_multiline_blocks', 'split_multi_statement_lines', 'get_indent', 'eat_spaces')
       'stmts'
@@ -341,34 +356,40 @@
          argcount  : 1
          nlocals   : 7
          stacksize : 5
          flags     : 3
          code
             0x970067007d0167007d0264017d037401000000000000000000007c006a
             0100000000000000007c006a020000000000000000a6020000ab02000000
-            0000000000440090015d135c0200007d045c0200007d057d067c04a00300
+            0000000000440090015d6c5c0200007d045c0200007d057d067c04a00300
             00000000000000000000000000000000000000a6000000ab000000000000
             000000a00400000000000000000000000000000000000000006402a60100
             00ab01000000000000000072447c03a00500000000000000000000000000
             000000000000006402a6010000ab01000000000000000064037a0000007c
             04a0060000000000000000000000000000000000000000a6000000ab0000
             00000000000000640464058502190000000000000000007a0000007c0164
-            063c0000007c067c0264061900000000000000000064043c0000006e977c
+            063c0000007c067c0264061900000000000000000064043c0000006ef07c
             04a0030000000000000000000000000000000000000000a6000000ab0000
             00000000000000a004000000000000000000000000000000000000000064
             07a6010000ab01000000000000000072447c03a005000000000000000000
             00000000000000000000006407a6010000ab01000000000000000064037a
             0000007c04a0060000000000000000000000000000000000000000a60000
             00ab000000000000000000640464058502190000000000000000007a0000
             007c0164063c0000007c067c0264061900000000000000000064043c0000
-            006e2c7c01a00700000000000000000000000000000000000000007c04a6
-            010000ab01000000000000000001007c02a0070000000000000000000000
-            0000000000000000007c057c066702a6010000ab01000000000000000001
-            007c016406190000000000000000007d0390018c15741100000000000000
-            0000007c017c02a6020000ab0200000000000000005300
+            006e857c04a00400000000000000000000000000000000000000006408a6
+            010000ab01000000000000000072447c03a0050000000000000000000000
+            0000000000000000006408a6010000ab01000000000000000064037a0000
+            007c04a0060000000000000000000000000000000000000000a6000000ab
+            000000000000000000640464058502190000000000000000007a0000007c
+            0164063c0000007c067c0264061900000000000000000064043c0000006e
+            2c7c01a00700000000000000000000000000000000000000007c04a60100
+            00ab01000000000000000001007c02a00700000000000000000000000000
+            000000000000007c057c066702a6010000ab01000000000000000001007c
+            016406190000000000000000007d0390018c6e7411000000000000000000
+            007c017c02a6020000ab0200000000000000005300
           42           0 RESUME                   0
          
           51           2 BUILD_LIST               0
                        4 STORE_FAST               1 (new_stmt)
          
           52           6 BUILD_LIST               0
                        8 STORE_FAST               2 (new_lines)
@@ -381,15 +402,15 @@
                       28 LOAD_ATTR                1 (stmt)
                       38 LOAD_FAST                0 (stmts)
                       40 LOAD_ATTR                2 (lines)
                       50 PRECALL                  2
                       54 CALL                     2
                       64 GET_ITER
                  >>   66 EXTENDED_ARG             1
-                      68 FOR_ITER               275 (to 620)
+                      68 FOR_ITER               364 (to 798)
                       70 UNPACK_SEQUENCE          2
                       74 STORE_FAST               4 (line)
                       76 UNPACK_SEQUENCE          2
                       80 STORE_FAST               5 (lstart)
                       82 STORE_FAST               6 (lend)
          
           55          84 LOAD_FAST                4 (line)
@@ -424,15 +445,15 @@
          
           57         274 LOAD_FAST                6 (lend)
                      276 LOAD_FAST                2 (new_lines)
                      278 LOAD_CONST               6 (-1)
                      280 BINARY_SUBSCR
                      290 LOAD_CONST               4 (1)
                      292 STORE_SUBSCR
-                     296 JUMP_FORWARD           151 (to 600)
+                     296 JUMP_FORWARD           240 (to 778)
          
           58     >>  298 LOAD_FAST                4 (line)
                      300 LOAD_METHOD              3 (lstrip)
                      322 PRECALL                  0
                      326 CALL                     0
                      336 LOAD_METHOD              4 (startswith)
                      358 LOAD_CONST               7 ('$')
@@ -462,214 +483,219 @@
          
           60         488 LOAD_FAST                6 (lend)
                      490 LOAD_FAST                2 (new_lines)
                      492 LOAD_CONST               6 (-1)
                      494 BINARY_SUBSCR
                      504 LOAD_CONST               4 (1)
                      506 STORE_SUBSCR
-                     510 JUMP_FORWARD            44 (to 600)
+                     510 JUMP_FORWARD           133 (to 778)
          
-          62     >>  512 LOAD_FAST                1 (new_stmt)
-                     514 LOAD_METHOD              7 (append)
-                     536 LOAD_FAST                4 (line)
+          61     >>  512 LOAD_FAST                4 (line)
+                     514 LOAD_METHOD              4 (startswith)
+                     536 LOAD_CONST               8 ('     +')
                      538 PRECALL                  1
                      542 CALL                     1
-                     552 POP_TOP
-         
-          63         554 LOAD_FAST                2 (new_lines)
-                     556 LOAD_METHOD              7 (append)
-                     578 LOAD_FAST                5 (lstart)
-                     580 LOAD_FAST                6 (lend)
-                     582 BUILD_LIST               2
-                     584 PRECALL                  1
-                     588 CALL                     1
-                     598 POP_TOP
+                     552 POP_JUMP_FORWARD_IF_FALSE    68 (to 690)
          
-          65     >>  600 LOAD_FAST                1 (new_stmt)
-                     602 LOAD_CONST               6 (-1)
-                     604 BINARY_SUBSCR
-                     614 STORE_FAST               3 (last_line)
-                     616 EXTENDED_ARG             1
-                     618 JUMP_BACKWARD          277 (to 66)
-         
-          66     >>  620 LOAD_GLOBAL             17 (NULL + Statements)
-                     632 LOAD_FAST                1 (new_stmt)
-                     634 LOAD_FAST                2 (new_lines)
-                     636 PRECALL                  2
-                     640 CALL                     2
-                     650 RETURN_VALUE
+          62         554 LOAD_FAST                3 (last_line)
+                     556 LOAD_METHOD              5 (rstrip)
+                     578 LOAD_CONST               8 ('     +')
+                     580 PRECALL                  1
+                     584 CALL                     1
+                     594 LOAD_CONST               3 (' ')
+                     596 BINARY_OP                0 (+)
+                     600 LOAD_FAST                4 (line)
+                     602 LOAD_METHOD              6 (strip)
+                     624 PRECALL                  0
+                     628 CALL                     0
+                     638 LOAD_CONST               4 (1)
+                     640 LOAD_CONST               5 (None)
+                     642 BUILD_SLICE              2
+                     644 BINARY_SUBSCR
+                     654 BINARY_OP                0 (+)
+                     658 LOAD_FAST                1 (new_stmt)
+                     660 LOAD_CONST               6 (-1)
+                     662 STORE_SUBSCR
+         
+          63         666 LOAD_FAST                6 (lend)
+                     668 LOAD_FAST                2 (new_lines)
+                     670 LOAD_CONST               6 (-1)
+                     672 BINARY_SUBSCR
+                     682 LOAD_CONST               4 (1)
+                     684 STORE_SUBSCR
+                     688 JUMP_FORWARD            44 (to 778)
+         
+          65     >>  690 LOAD_FAST                1 (new_stmt)
+                     692 LOAD_METHOD              7 (append)
+                     714 LOAD_FAST                4 (line)
+                     716 PRECALL                  1
+                     720 CALL                     1
+                     730 POP_TOP
+         
+          66         732 LOAD_FAST                2 (new_lines)
+                     734 LOAD_METHOD              7 (append)
+                     756 LOAD_FAST                5 (lstart)
+                     758 LOAD_FAST                6 (lend)
+                     760 BUILD_LIST               2
+                     762 PRECALL                  1
+                     766 CALL                     1
+                     776 POP_TOP
+         
+          68     >>  778 LOAD_FAST                1 (new_stmt)
+                     780 LOAD_CONST               6 (-1)
+                     782 BINARY_SUBSCR
+                     792 STORE_FAST               3 (last_line)
+                     794 EXTENDED_ARG             1
+                     796 JUMP_BACKWARD          366 (to 66)
+         
+          69     >>  798 LOAD_GLOBAL             17 (NULL + Statements)
+                     810 LOAD_FAST                1 (new_stmt)
+                     812 LOAD_FAST                2 (new_lines)
+                     814 PRECALL                  2
+                     818 CALL                     2
+                     828 RETURN_VALUE
          consts
             'Align continuation with amprsand\n    \n    For example\n\n     FORMAT("Lorem ipsum\n    & sic hamet") \n    \n    '
             ''
             '&'
             ' '
             1
             None
             -1
             '$'
+            '     +'
          names      ('zip', 'stmt', 'lines', 'lstrip', 'startswith', 'rstrip', 'strip', 'append', 'Statements')
          varnames   ('stmts', 'new_stmt', 'new_lines', 'last_line', 'line', 'lstart', 'lend')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
          name       'align_start_continuations'
          firstlineno 42
-         lnotab 0x020904010401040146014e01700118014e01700118022a012e021401
+         lnotab
+            0x020904010401040146014e01700118014e01700118012a01700118022a
+            012e021401
       code
          argcount  : 1
-         nlocals   : 9
+         nlocals   : 6
          stacksize : 7
          flags     : 3
          code
             0x970067007d0167007d027401000000000000000000007c006a01000000
             00000000007c006a020000000000000000a6020000ab0200000000000000
-            0044005db45c0200007d035c0200007d047d0564017d067c0344005d237d
-            077c0764026b030000000072167c07a00300000000000000000000000000
-            00000000000000a6000000ab000000000000000000730201006e067c067c
-            077a0d00007d068c247409000000000000000000007c06a0050000000000
-            000000000000000000000000000000a6000000ab000000000000000000a6
-            010000ab01000000000000000064036b0200000000723374090000000000
-            00000000007c06a6010000ab0100000000000000007d087c016404780278
-            02190000000000000000007c037c0864058502190000000000000000007a
-            0d0000630363023c0000007c057c0264041900000000000000000064033c
-            0000008c887c01a00600000000000000000000000000000000000000007c
-            03a6010000ab01000000000000000001007c02a006000000000000000000
-            00000000000000000000007c047c056702a6010000ab0100000000000000
-            0001008cb5740f000000000000000000007c017c02a6020000ab02000000
-            00000000005300
-          69           0 RESUME                   0
+            0044005d705c0200007d035c0200007d047d057c03640164028502190000
+            0000000000000064036b0200000000722e7c036402190000000000000000
+            006404760072247c01640578027802190000000000000000007c03640664
+            078502190000000000000000007a0d0000630363023c0000007c057c0264
+            051900000000000000000064083c0000008c447c01a00300000000000000
+            000000000000000000000000007c03a6010000ab01000000000000000001
+            007c02a00300000000000000000000000000000000000000007c047c0567
+            02a6010000ab01000000000000000001008c717409000000000000000000
+            007c017c02a6020000ab0200000000000000005300
+          72           0 RESUME                   0
          
-          81           2 BUILD_LIST               0
+          84           2 BUILD_LIST               0
                        4 STORE_FAST               1 (new_stmt)
          
-          82           6 BUILD_LIST               0
+          85           6 BUILD_LIST               0
                        8 STORE_FAST               2 (new_lines)
          
-          83          10 LOAD_GLOBAL              1 (NULL + zip)
+          86          10 LOAD_GLOBAL              1 (NULL + zip)
                       22 LOAD_FAST                0 (stmts)
                       24 LOAD_ATTR                1 (stmt)
                       34 LOAD_FAST                0 (stmts)
                       36 LOAD_ATTR                2 (lines)
                       46 PRECALL                  2
                       50 CALL                     2
                       60 GET_ITER
-                 >>   62 FOR_ITER               180 (to 424)
+                 >>   62 FOR_ITER               112 (to 288)
                       64 UNPACK_SEQUENCE          2
                       68 STORE_FAST               3 (line)
                       70 UNPACK_SEQUENCE          2
                       74 STORE_FAST               4 (lstart)
                       76 STORE_FAST               5 (lend)
          
-          85          78 LOAD_CONST               1 ('')
-                      80 STORE_FAST               6 (buffer)
-         
-          86          82 LOAD_FAST                3 (line)
-                      84 GET_ITER
-                 >>   86 FOR_ITER                35 (to 158)
-                      88 STORE_FAST               7 (char)
-         
-          87          90 LOAD_FAST                7 (char)
-                      92 LOAD_CONST               2 (' ')
-                      94 COMPARE_OP               3 (!=)
-                     100 POP_JUMP_FORWARD_IF_FALSE    22 (to 146)
-                     102 LOAD_FAST                7 (char)
-                     104 LOAD_METHOD              3 (isdigit)
-                     126 PRECALL                  0
-                     130 CALL                     0
-                     140 POP_JUMP_FORWARD_IF_TRUE     2 (to 146)
-         
-          88         142 POP_TOP
-                     144 JUMP_FORWARD             6 (to 158)
-         
-          89     >>  146 LOAD_FAST                6 (buffer)
-                     148 LOAD_FAST                7 (char)
-                     150 BINARY_OP               13 (+=)
-                     154 STORE_FAST               6 (buffer)
-                     156 JUMP_BACKWARD           36 (to 86)
-         
-          91     >>  158 LOAD_GLOBAL              9 (NULL + len)
-                     170 LOAD_FAST                6 (buffer)
-                     172 LOAD_METHOD              5 (strip)
-                     194 PRECALL                  0
-                     198 CALL                     0
-                     208 PRECALL                  1
-                     212 CALL                     1
-                     222 LOAD_CONST               3 (1)
-                     224 COMPARE_OP               2 (==)
-                     230 POP_JUMP_FORWARD_IF_FALSE    51 (to 334)
-         
-          93         232 LOAD_GLOBAL              9 (NULL + len)
-                     244 LOAD_FAST                6 (buffer)
-                     246 PRECALL                  1
-                     250 CALL                     1
-                     260 STORE_FAST               8 (reach)
-         
-          94         262 LOAD_FAST                1 (new_stmt)
-                     264 LOAD_CONST               4 (-1)
-                     266 COPY                     2
-                     268 COPY                     2
-                     270 BINARY_SUBSCR
-                     280 LOAD_FAST                3 (line)
-                     282 LOAD_FAST                8 (reach)
-                     284 LOAD_CONST               5 (None)
-                     286 BUILD_SLICE              2
-                     288 BINARY_SUBSCR
-                     298 BINARY_OP               13 (+=)
-                     302 SWAP                     3
-                     304 SWAP                     2
-                     306 STORE_SUBSCR
-         
-          97         310 LOAD_FAST                5 (lend)
-                     312 LOAD_FAST                2 (new_lines)
-                     314 LOAD_CONST               4 (-1)
-                     316 BINARY_SUBSCR
-                     326 LOAD_CONST               3 (1)
-                     328 STORE_SUBSCR
-                     332 JUMP_BACKWARD          136 (to 62)
-         
-          99     >>  334 LOAD_FAST                1 (new_stmt)
-                     336 LOAD_METHOD              6 (append)
-                     358 LOAD_FAST                3 (line)
-                     360 PRECALL                  1
-                     364 CALL                     1
-                     374 POP_TOP
+          87          78 LOAD_FAST                3 (line)
+                      80 LOAD_CONST               1 (0)
+                      82 LOAD_CONST               2 (5)
+                      84 BUILD_SLICE              2
+                      86 BINARY_SUBSCR
+                      96 LOAD_CONST               3 ('     ')
+                      98 COMPARE_OP               2 (==)
+                     104 POP_JUMP_FORWARD_IF_FALSE    46 (to 198)
+                     106 LOAD_FAST                3 (line)
+                     108 LOAD_CONST               2 (5)
+                     110 BINARY_SUBSCR
+                     120 LOAD_CONST               4 ('0123456789*')
+                     122 CONTAINS_OP              0
+                     124 POP_JUMP_FORWARD_IF_FALSE    36 (to 198)
+         
+          88         126 LOAD_FAST                1 (new_stmt)
+                     128 LOAD_CONST               5 (-1)
+                     130 COPY                     2
+                     132 COPY                     2
+                     134 BINARY_SUBSCR
+                     144 LOAD_FAST                3 (line)
+                     146 LOAD_CONST               6 (7)
+                     148 LOAD_CONST               7 (None)
+                     150 BUILD_SLICE              2
+                     152 BINARY_SUBSCR
+                     162 BINARY_OP               13 (+=)
+                     166 SWAP                     3
+                     168 SWAP                     2
+                     170 STORE_SUBSCR
+         
+          89         174 LOAD_FAST                5 (lend)
+                     176 LOAD_FAST                2 (new_lines)
+                     178 LOAD_CONST               5 (-1)
+                     180 BINARY_SUBSCR
+                     190 LOAD_CONST               8 (1)
+                     192 STORE_SUBSCR
+                     196 JUMP_BACKWARD           68 (to 62)
+         
+          91     >>  198 LOAD_FAST                1 (new_stmt)
+                     200 LOAD_METHOD              3 (append)
+                     222 LOAD_FAST                3 (line)
+                     224 PRECALL                  1
+                     228 CALL                     1
+                     238 POP_TOP
+         
+          92         240 LOAD_FAST                2 (new_lines)
+                     242 LOAD_METHOD              3 (append)
+                     264 LOAD_FAST                4 (lstart)
+                     266 LOAD_FAST                5 (lend)
+                     268 BUILD_LIST               2
+                     270 PRECALL                  1
+                     274 CALL                     1
+                     284 POP_TOP
+                     286 JUMP_BACKWARD          113 (to 62)
          
-         100         376 LOAD_FAST                2 (new_lines)
-                     378 LOAD_METHOD              6 (append)
-                     400 LOAD_FAST                4 (lstart)
-                     402 LOAD_FAST                5 (lend)
-                     404 BUILD_LIST               2
-                     406 PRECALL                  1
-                     410 CALL                     1
-                     420 POP_TOP
-                     422 JUMP_BACKWARD          181 (to 62)
-         
-         102     >>  424 LOAD_GLOBAL             15 (NULL + Statements)
-                     436 LOAD_FAST                1 (new_stmt)
-                     438 LOAD_FAST                2 (new_lines)
-                     440 PRECALL                  2
-                     444 CALL                     2
-                     454 RETURN_VALUE
+          94     >>  288 LOAD_GLOBAL              9 (NULL + Statements)
+                     300 LOAD_FAST                1 (new_stmt)
+                     302 LOAD_FAST                2 (new_lines)
+                     304 PRECALL                  2
+                     308 CALL                     2
+                     318 RETURN_VALUE
          consts
             "Align labelled continuations , very old style\n   15 FORMAT(\n     1/' TRANFT:  Transport property fitting,',\n     2/'           CHEMKIN-II Version ',A,', August 1994',\nC*****precision > double\n     3/'           DOUBLE PRECISION')\n\n     becomes\n    15 FORMAT(' TRANFT:  Transport property fitting,',' CHEMKIN-II Version ',A,', August 1994','DOUBLE PRECISION') \n    \n    "
-            ''
-            ' '
-            1
+            0
+            5
+            '     '
+            '0123456789*'
             -1
+            7
             None
-         names      ('zip', 'stmt', 'lines', 'isdigit', 'len', 'strip', 'append', 'Statements')
-         varnames   ('stmts', 'new_stmt', 'new_lines', 'line', 'lstart', 'lend', 'buffer', 'char', 'reach')
+            1
+         names      ('zip', 'stmt', 'lines', 'append', 'Statements')
+         varnames   ('stmts', 'new_stmt', 'new_lines', 'line', 'lstart', 'lend')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
          name       'ftn_align_labelled_continuations'
-         firstlineno 69
-         lnotab
-            0x020c04010401440204010801340104010c024a021e01300318022a0130
-            02
+         firstlineno 72
+         lnotab 0x020c0401040144013001300118022a013002
       code
          argcount  : 1
          nlocals   : 8
          stacksize : 11
          flags     : 3
          code
             0x970067007d0167007d027401000000000000000000007c006a01000000
@@ -718,23 +744,23 @@
             00000000000000000000007c047c056702a6010000ab0100000000000000
             0001007c01a00500000000000000000000000000000000000000007c0764
             0c7a000000a6010000ab01000000000000000001006e157c01a005000000
             00000000000000000000000000000000007c03a6010000ab010000000000
             00000001007c02a00500000000000000000000000000000000000000007c
             047c056702a6010000ab010000000000000000010090028cbd7417000000
             000000000000007c017c02a6020000ab0200000000000000005300
-         106           0 RESUME                   0
+          98           0 RESUME                   0
          
-         115           2 BUILD_LIST               0
+         107           2 BUILD_LIST               0
                        4 STORE_FAST               1 (new_stmt)
          
-         116           6 BUILD_LIST               0
+         108           6 BUILD_LIST               0
                        8 STORE_FAST               2 (new_lines)
          
-         117          10 LOAD_GLOBAL              1 (NULL + zip)
+         109          10 LOAD_GLOBAL              1 (NULL + zip)
                       22 LOAD_FAST                0 (stmts)
                       24 LOAD_ATTR                1 (stmt)
                       34 LOAD_FAST                0 (stmts)
                       36 LOAD_ATTR                2 (lines)
                       46 PRECALL                  2
                       50 CALL                     2
                       60 GET_ITER
@@ -742,34 +768,34 @@
                       64 FOR_ITER               699 (to 1464)
                       66 UNPACK_SEQUENCE          2
                       70 STORE_FAST               3 (line)
                       72 UNPACK_SEQUENCE          2
                       76 STORE_FAST               4 (lstart)
                       78 STORE_FAST               5 (lend)
          
-         118          80 LOAD_CONST               1 ('do')
+         110          80 LOAD_CONST               1 ('do')
                       82 LOAD_FAST                3 (line)
                       84 LOAD_METHOD              3 (split)
                      106 PRECALL                  0
                      110 CALL                     0
                      120 CONTAINS_OP              0
                      122 POP_JUMP_FORWARD_IF_FALSE   165 (to 454)
          
-         119         124 LOAD_CONST               2 (': do')
+         111         124 LOAD_CONST               2 (': do')
                      126 LOAD_FAST                3 (line)
                      128 LOAD_METHOD              4 (strip)
                      150 PRECALL                  0
                      154 CALL                     0
                      164 CONTAINS_OP              0
                      166 POP_JUMP_FORWARD_IF_FALSE   120 (to 408)
          
-         120         168 LOAD_FAST                1 (new_stmt)
+         112         168 LOAD_FAST                1 (new_stmt)
                      170 LOAD_METHOD              5 (append)
          
-         121         192 LOAD_FAST                3 (line)
+         113         192 LOAD_FAST                3 (line)
                      194 LOAD_METHOD              6 (replace)
                      216 LOAD_CONST               3 (' ')
                      218 LOAD_METHOD              7 (join)
                      240 LOAD_FAST                3 (line)
                      242 LOAD_METHOD              3 (split)
                      264 PRECALL                  0
                      268 CALL                     0
@@ -784,221 +810,221 @@
                      346 CALL                     0
                      356 PRECALL                  1
                      360 CALL                     1
                      370 BINARY_OP                0 (+)
                      374 PRECALL                  2
                      378 CALL                     2
          
-         120         388 PRECALL                  1
+         112         388 PRECALL                  1
                      392 CALL                     1
                      402 POP_TOP
                      404 EXTENDED_ARG             1
                      406 JUMP_FORWARD           503 (to 1414)
          
-         124     >>  408 LOAD_FAST                1 (new_stmt)
+         116     >>  408 LOAD_FAST                1 (new_stmt)
                      410 LOAD_METHOD              5 (append)
                      432 LOAD_FAST                3 (line)
                      434 PRECALL                  1
                      438 CALL                     1
                      448 POP_TOP
                      450 EXTENDED_ARG             1
                      452 JUMP_FORWARD           480 (to 1414)
          
-         126     >>  454 LOAD_FAST                3 (line)
+         118     >>  454 LOAD_FAST                3 (line)
                      456 LOAD_METHOD              4 (strip)
                      478 PRECALL                  0
                      482 CALL                     0
                      492 LOAD_METHOD              8 (startswith)
                      514 LOAD_CONST               5 ('if ')
                      516 PRECALL                  1
                      520 CALL                     1
                      530 POP_JUMP_FORWARD_IF_FALSE   169 (to 870)
                      532 LOAD_CONST               6 (' then')
                      534 LOAD_FAST                3 (line)
                      536 CONTAINS_OP              1
                      538 POP_JUMP_FORWARD_IF_FALSE   165 (to 870)
          
-         128         540 LOAD_GLOBAL             19 (NULL + split_oneliner)
+         120         540 LOAD_GLOBAL             19 (NULL + split_oneliner)
                      552 LOAD_FAST                3 (line)
                      554 PRECALL                  1
                      558 CALL                     1
                      568 STORE_FAST               6 (splitted_parts)
          
-         130         570 LOAD_GLOBAL             21 (NULL + get_indent)
+         122         570 LOAD_GLOBAL             21 (NULL + get_indent)
                      582 LOAD_FAST                3 (line)
                      584 PRECALL                  1
                      588 CALL                     1
                      598 STORE_FAST               7 (indent)
          
-         131         600 LOAD_FAST                1 (new_stmt)
+         123         600 LOAD_FAST                1 (new_stmt)
                      602 LOAD_METHOD              5 (append)
                      624 LOAD_FAST                6 (splitted_parts)
                      626 LOAD_CONST               7 (0)
                      628 BINARY_SUBSCR
                      638 LOAD_CONST               6 (' then')
                      640 BINARY_OP                0 (+)
                      644 PRECALL                  1
                      648 CALL                     1
                      658 POP_TOP
          
-         132         660 LOAD_FAST                2 (new_lines)
+         124         660 LOAD_FAST                2 (new_lines)
                      662 LOAD_METHOD              5 (append)
                      684 LOAD_FAST                4 (lstart)
                      686 LOAD_FAST                5 (lend)
                      688 BUILD_LIST               2
                      690 PRECALL                  1
                      694 CALL                     1
                      704 POP_TOP
          
-         133         706 LOAD_FAST                1 (new_stmt)
+         125         706 LOAD_FAST                1 (new_stmt)
                      708 LOAD_METHOD              5 (append)
                      730 LOAD_FAST                7 (indent)
                      732 LOAD_CONST               8 ('   ')
                      734 BINARY_OP                0 (+)
                      738 LOAD_FAST                6 (splitted_parts)
                      740 LOAD_CONST               9 (-1)
                      742 BINARY_SUBSCR
                      752 BINARY_OP                0 (+)
                      756 PRECALL                  1
                      760 CALL                     1
                      770 POP_TOP
          
-         134         772 LOAD_FAST                2 (new_lines)
+         126         772 LOAD_FAST                2 (new_lines)
                      774 LOAD_METHOD              5 (append)
                      796 LOAD_FAST                4 (lstart)
                      798 LOAD_FAST                5 (lend)
                      800 BUILD_LIST               2
                      802 PRECALL                  1
                      806 CALL                     1
                      816 POP_TOP
          
-         135         818 LOAD_FAST                1 (new_stmt)
+         127         818 LOAD_FAST                1 (new_stmt)
                      820 LOAD_METHOD              5 (append)
                      842 LOAD_FAST                7 (indent)
                      844 LOAD_CONST              10 ('end if')
                      846 BINARY_OP                0 (+)
                      850 PRECALL                  1
                      854 CALL                     1
                      864 POP_TOP
                      866 EXTENDED_ARG             1
                      868 JUMP_FORWARD           272 (to 1414)
          
-         145     >>  870 LOAD_FAST                3 (line)
+         129     >>  870 LOAD_FAST                3 (line)
                      872 LOAD_METHOD              4 (strip)
                      894 PRECALL                  0
                      898 CALL                     0
                      908 LOAD_METHOD              8 (startswith)
                      930 LOAD_CONST              11 ('where ')
                      932 PRECALL                  1
                      936 CALL                     1
                      946 POP_JUMP_FORWARD_IF_FALSE   212 (to 1372)
          
-         146         948 LOAD_GLOBAL             19 (NULL + split_oneliner)
+         130         948 LOAD_GLOBAL             19 (NULL + split_oneliner)
                      960 LOAD_FAST                3 (line)
                      962 PRECALL                  1
                      966 CALL                     1
                      976 STORE_FAST               6 (splitted_parts)
          
-         148         978 LOAD_FAST                6 (splitted_parts)
+         132         978 LOAD_FAST                6 (splitted_parts)
                      980 LOAD_CONST               9 (-1)
                      982 BINARY_SUBSCR
                      992 POP_JUMP_FORWARD_IF_TRUE    46 (to 1086)
          
-         149         994 LOAD_FAST                1 (new_stmt)
+         133         994 LOAD_FAST                1 (new_stmt)
                      996 LOAD_METHOD              5 (append)
                     1018 LOAD_FAST                3 (line)
                     1020 PRECALL                  1
                     1024 CALL                     1
                     1034 POP_TOP
          
-         150        1036 LOAD_FAST                2 (new_lines)
+         134        1036 LOAD_FAST                2 (new_lines)
                     1038 LOAD_METHOD              5 (append)
                     1060 LOAD_FAST                4 (lstart)
                     1062 LOAD_FAST                5 (lend)
                     1064 BUILD_LIST               2
                     1066 PRECALL                  1
                     1070 CALL                     1
                     1080 POP_TOP
          
-         151        1082 EXTENDED_ARG             2
+         135        1082 EXTENDED_ARG             2
                     1084 JUMP_BACKWARD          512 (to 62)
          
-         153     >> 1086 LOAD_GLOBAL             21 (NULL + get_indent)
+         137     >> 1086 LOAD_GLOBAL             21 (NULL + get_indent)
                     1098 LOAD_FAST                3 (line)
                     1100 PRECALL                  1
                     1104 CALL                     1
                     1114 STORE_FAST               7 (indent)
          
-         154        1116 LOAD_FAST                1 (new_stmt)
+         138        1116 LOAD_FAST                1 (new_stmt)
                     1118 LOAD_METHOD              5 (append)
                     1140 LOAD_FAST                6 (splitted_parts)
                     1142 LOAD_CONST               7 (0)
                     1144 BINARY_SUBSCR
                     1154 PRECALL                  1
                     1158 CALL                     1
                     1168 POP_TOP
          
-         155        1170 LOAD_FAST                2 (new_lines)
+         139        1170 LOAD_FAST                2 (new_lines)
                     1172 LOAD_METHOD              5 (append)
                     1194 LOAD_FAST                4 (lstart)
                     1196 LOAD_FAST                5 (lend)
                     1198 BUILD_LIST               2
                     1200 PRECALL                  1
                     1204 CALL                     1
                     1214 POP_TOP
          
-         156        1216 LOAD_FAST                1 (new_stmt)
+         140        1216 LOAD_FAST                1 (new_stmt)
                     1218 LOAD_METHOD              5 (append)
                     1240 LOAD_FAST                7 (indent)
                     1242 LOAD_FAST                6 (splitted_parts)
                     1244 LOAD_CONST               9 (-1)
                     1246 BINARY_SUBSCR
                     1256 BINARY_OP                0 (+)
                     1260 PRECALL                  1
                     1264 CALL                     1
                     1274 POP_TOP
          
-         157        1276 LOAD_FAST                2 (new_lines)
+         141        1276 LOAD_FAST                2 (new_lines)
                     1278 LOAD_METHOD              5 (append)
                     1300 LOAD_FAST                4 (lstart)
                     1302 LOAD_FAST                5 (lend)
                     1304 BUILD_LIST               2
                     1306 PRECALL                  1
                     1310 CALL                     1
                     1320 POP_TOP
          
-         158        1322 LOAD_FAST                1 (new_stmt)
+         142        1322 LOAD_FAST                1 (new_stmt)
                     1324 LOAD_METHOD              5 (append)
                     1346 LOAD_FAST                7 (indent)
                     1348 LOAD_CONST              12 ('end where')
                     1350 BINARY_OP                0 (+)
                     1354 PRECALL                  1
                     1358 CALL                     1
                     1368 POP_TOP
                     1370 JUMP_FORWARD            21 (to 1414)
          
-         161     >> 1372 LOAD_FAST                1 (new_stmt)
+         145     >> 1372 LOAD_FAST                1 (new_stmt)
                     1374 LOAD_METHOD              5 (append)
                     1396 LOAD_FAST                3 (line)
                     1398 PRECALL                  1
                     1402 CALL                     1
                     1412 POP_TOP
          
-         163     >> 1414 LOAD_FAST                2 (new_lines)
+         147     >> 1414 LOAD_FAST                2 (new_lines)
                     1416 LOAD_METHOD              5 (append)
                     1438 LOAD_FAST                4 (lstart)
                     1440 LOAD_FAST                5 (lend)
                     1442 BUILD_LIST               2
                     1444 PRECALL                  1
                     1448 CALL                     1
                     1458 POP_TOP
                     1460 EXTENDED_ARG             2
                     1462 JUMP_BACKWARD          701 (to 62)
          
-         164     >> 1464 LOAD_GLOBAL             23 (NULL + Statements)
+         148     >> 1464 LOAD_GLOBAL             23 (NULL + Statements)
                     1476 LOAD_FAST                1 (new_stmt)
                     1478 LOAD_FAST                2 (new_lines)
                     1480 PRECALL                  2
                     1484 CALL                     2
                     1494 RETURN_VALUE
          consts
             '_summary_\n\n    Args:\n        stmts (Statements): _description_\n\n    Returns:\n        Statements: _description_\n    '
@@ -1016,18 +1042,18 @@
             'end where'
          names      ('zip', 'stmt', 'lines', 'split', 'strip', 'append', 'replace', 'join', 'startswith', 'split_oneliner', 'get_indent', 'Statements')
          varnames   ('stmts', 'new_stmt', 'new_lines', 'line', 'lstart', 'lend', 'splitted_parts', 'indent')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
          name       'ftn_make_oneliners_conditionals_multilines'
-         firstlineno 106
+         firstlineno 98
          lnotab
             0x02090401040146012c012c011801c4ff14042e0256021e021e013c012e
-            0142012e01340a4e011e0210012a012e0104021e0136012e013c012e0132
+            0142012e0134024e011e0210012a012e0104021e0136012e013c012e0132
             032a023201
       'line'
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 6
          flags     : 3
@@ -1039,112 +1065,112 @@
             05760072547c027c057a0d00007d027c01a0020000000000000000000000
             0000000000000000006404a6010000ab01000000000000000001007c0173
             377c03a00100000000000000000000000000000000000000007c02a60100
             00ab01000000000000000001007c03a00100000000000000000000000000
             000000000000007c007c0464057a00000064068502190000000000000000
             00a6010000ab010000000000000000010001006e078c7c7c027c057a0d00
             007d028c827c0373037c0267017d037c035300
-         167           0 RESUME                   0
+         151           0 RESUME                   0
          
-         177           2 BUILD_LIST               0
+         161           2 BUILD_LIST               0
                        4 STORE_FAST               1 (path)
          
-         178           6 LOAD_CONST               1 ('')
+         162           6 LOAD_CONST               1 ('')
                        8 STORE_FAST               2 (new_stmt)
          
-         179          10 BUILD_LIST               0
+         163          10 BUILD_LIST               0
                       12 STORE_FAST               3 (split_parts)
          
-         180          14 LOAD_GLOBAL              1 (NULL + enumerate)
+         164          14 LOAD_GLOBAL              1 (NULL + enumerate)
                       26 LOAD_FAST                0 (line)
                       28 PRECALL                  1
                       32 CALL                     1
                       42 GET_ITER
                  >>   44 FOR_ITER               129 (to 304)
                       46 UNPACK_SEQUENCE          2
                       50 STORE_FAST               4 (idx)
                       52 STORE_FAST               5 (char)
          
-         181          54 LOAD_CONST               2 ('(')
+         165          54 LOAD_CONST               2 ('(')
                       56 LOAD_FAST                5 (char)
                       58 CONTAINS_OP              0
                       60 POP_JUMP_FORWARD_IF_FALSE    27 (to 116)
          
-         182          62 LOAD_FAST                2 (new_stmt)
+         166          62 LOAD_FAST                2 (new_stmt)
                       64 LOAD_FAST                5 (char)
                       66 BINARY_OP               13 (+=)
                       70 STORE_FAST               2 (new_stmt)
          
-         183          72 LOAD_FAST                1 (path)
+         167          72 LOAD_FAST                1 (path)
                       74 LOAD_METHOD              1 (append)
                       96 LOAD_FAST                5 (char)
                       98 PRECALL                  1
                      102 CALL                     1
                      112 POP_TOP
                      114 JUMP_BACKWARD           36 (to 44)
          
-         184     >>  116 LOAD_CONST               3 (')')
+         168     >>  116 LOAD_CONST               3 (')')
                      118 LOAD_FAST                5 (char)
                      120 CONTAINS_OP              0
                      122 POP_JUMP_FORWARD_IF_FALSE    84 (to 292)
          
-         185         124 LOAD_FAST                2 (new_stmt)
+         169         124 LOAD_FAST                2 (new_stmt)
                      126 LOAD_FAST                5 (char)
                      128 BINARY_OP               13 (+=)
                      132 STORE_FAST               2 (new_stmt)
          
-         186         134 LOAD_FAST                1 (path)
+         170         134 LOAD_FAST                1 (path)
                      136 LOAD_METHOD              2 (pop)
                      158 LOAD_CONST               4 (-1)
                      160 PRECALL                  1
                      164 CALL                     1
                      174 POP_TOP
          
-         187         176 LOAD_FAST                1 (path)
+         171         176 LOAD_FAST                1 (path)
                      178 POP_JUMP_FORWARD_IF_TRUE    55 (to 290)
          
-         188         180 LOAD_FAST                3 (split_parts)
+         172         180 LOAD_FAST                3 (split_parts)
                      182 LOAD_METHOD              1 (append)
                      204 LOAD_FAST                2 (new_stmt)
                      206 PRECALL                  1
                      210 CALL                     1
                      220 POP_TOP
          
-         189         222 LOAD_FAST                3 (split_parts)
+         173         222 LOAD_FAST                3 (split_parts)
                      224 LOAD_METHOD              1 (append)
                      246 LOAD_FAST                0 (line)
                      248 LOAD_FAST                4 (idx)
                      250 LOAD_CONST               5 (1)
                      252 BINARY_OP                0 (+)
                      256 LOAD_CONST               6 (None)
                      258 BUILD_SLICE              2
                      260 BINARY_SUBSCR
                      270 PRECALL                  1
                      274 CALL                     1
                      284 POP_TOP
          
-         190         286 POP_TOP
+         174         286 POP_TOP
                      288 JUMP_FORWARD             7 (to 304)
          
-         187     >>  290 JUMP_BACKWARD          124 (to 44)
+         171     >>  290 JUMP_BACKWARD          124 (to 44)
          
-         192     >>  292 LOAD_FAST                2 (new_stmt)
+         176     >>  292 LOAD_FAST                2 (new_stmt)
                      294 LOAD_FAST                5 (char)
                      296 BINARY_OP               13 (+=)
                      300 STORE_FAST               2 (new_stmt)
                      302 JUMP_BACKWARD          130 (to 44)
          
-         193     >>  304 LOAD_FAST                3 (split_parts)
+         177     >>  304 LOAD_FAST                3 (split_parts)
                      306 POP_JUMP_FORWARD_IF_TRUE     3 (to 314)
          
-         194         308 LOAD_FAST                2 (new_stmt)
+         178         308 LOAD_FAST                2 (new_stmt)
                      310 BUILD_LIST               1
                      312 STORE_FAST               3 (split_parts)
          
-         195     >>  314 LOAD_FAST                3 (split_parts)
+         179     >>  314 LOAD_FAST                3 (split_parts)
                      316 RETURN_VALUE
          consts
             '_summary_\n\n    Args:\n        line (str): _description_\n\n    Returns:\n        list: _description_\n    '
             ''
             '('
             ')'
             -1
@@ -1152,15 +1178,15 @@
             None
          names      ('enumerate', 'append', 'pop')
          varnames   ('line', 'path', 'new_stmt', 'split_parts', 'idx', 'char')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
          name       'split_oneliner'
-         firstlineno 167
+         firstlineno 151
          lnotab
             0x020a040104010401280108010a012c0108010a012a0104012a01400104
             fd02050c0104010601
       'lines'
       code
          argcount  : 1
          nlocals   : 6
@@ -1178,72 +1204,72 @@
             00a6000000ab00000000000000000064011900000000000000000064057a
             0000007c02a0000000000000000000000000000000000000000000a60000
             00ab00000000000000000064011900000000000000000064047a000000a6
             020000ab0200000000000000007d037409000000000000000000006a0500
             0000000000000064067c049b0064079d03a6010000ab0100000000000000
             0001007c01a00600000000000000000000000000000000000000007c03a6
             010000ab01000000000000000001008cd57c015300
-         198           0 RESUME                   0
+         182           0 RESUME                   0
          
-         209           2 BUILD_LIST               0
+         193           2 BUILD_LIST               0
                        4 STORE_FAST               1 (new_stmt)
          
-         210           6 LOAD_FAST                0 (lines)
+         194           6 LOAD_FAST                0 (lines)
                        8 GET_ITER
                  >>   10 FOR_ITER               212 (to 436)
                       12 STORE_FAST               2 (line)
          
-         211          14 LOAD_FAST                2 (line)
+         195          14 LOAD_FAST                2 (line)
                       16 STORE_FAST               3 (stmt)
          
-         212          18 NOP
+         196          18 NOP
          
-         213          20 LOAD_FAST                2 (line)
+         197          20 LOAD_FAST                2 (line)
                       22 LOAD_METHOD              0 (split)
                       44 PRECALL                  0
                       48 CALL                     0
                       58 LOAD_CONST               1 (0)
                       60 BINARY_SUBSCR
                       70 STORE_FAST               4 (item0)
          
-         214          72 LOAD_FAST                2 (line)
+         198          72 LOAD_FAST                2 (line)
                       74 LOAD_METHOD              0 (split)
                       96 PRECALL                  0
                      100 CALL                     0
                      110 LOAD_CONST               2 (1)
                      112 BINARY_SUBSCR
                      122 STORE_FAST               5 (item1)
                      124 JUMP_FORWARD            18 (to 162)
                  >>  126 PUSH_EXC_INFO
          
-         215         128 LOAD_GLOBAL              2 (IndexError)
+         199         128 LOAD_GLOBAL              2 (IndexError)
                      140 CHECK_EXC_MATCH
                      142 POP_JUMP_FORWARD_IF_FALSE     5 (to 154)
                      144 POP_TOP
          
-         216         146 LOAD_CONST               3 (None)
+         200         146 LOAD_CONST               3 (None)
                      148 STORE_FAST               5 (item1)
                      150 POP_EXCEPT
                      152 JUMP_FORWARD             4 (to 162)
          
-         215     >>  154 RERAISE                  0
+         199     >>  154 RERAISE                  0
                  >>  156 COPY                     3
                      158 POP_EXCEPT
                      160 RERAISE                  1
          
-         218     >>  162 LOAD_FAST                5 (item1)
+         202     >>  162 LOAD_FAST                5 (item1)
                      164 LOAD_CONST               4 ('=')
                      166 COMPARE_OP               2 (==)
                      172 POP_JUMP_FORWARD_IF_FALSE   109 (to 392)
                      174 LOAD_FAST                4 (item0)
                      176 LOAD_GLOBAL              4 (KEYWORDS_FTN)
                      188 CONTAINS_OP              0
                      190 POP_JUMP_FORWARD_IF_FALSE   100 (to 392)
          
-         219         192 LOAD_FAST                2 (line)
+         203         192 LOAD_FAST                2 (line)
                      194 LOAD_METHOD              3 (replace)
                      216 LOAD_FAST                2 (line)
                      218 LOAD_METHOD              0 (split)
                      240 PRECALL                  0
                      244 CALL                     0
                      254 LOAD_CONST               1 (0)
                      256 BINARY_SUBSCR
@@ -1257,36 +1283,36 @@
                      312 BINARY_SUBSCR
                      322 LOAD_CONST               4 ('=')
                      324 BINARY_OP                0 (+)
                      328 PRECALL                  2
                      332 CALL                     2
                      342 STORE_FAST               3 (stmt)
          
-         220         344 LOAD_GLOBAL              9 (NULL + logger)
+         204         344 LOAD_GLOBAL              9 (NULL + logger)
                      356 LOAD_ATTR                5 (warning)
          
-         221         366 LOAD_CONST               6 ('A Fortran Keywords ')
+         205         366 LOAD_CONST               6 ('A Fortran Keywords ')
                      368 LOAD_FAST                4 (item0)
                      370 FORMAT_VALUE             0
                      372 LOAD_CONST               7 (' is used as a variable in the code. Bad Practice Should Be Avoided')
                      374 BUILD_STRING             3
          
-         220         376 PRECALL                  1
+         204         376 PRECALL                  1
                      380 CALL                     1
                      390 POP_TOP
          
-         224     >>  392 LOAD_FAST                1 (new_stmt)
+         208     >>  392 LOAD_FAST                1 (new_stmt)
                      394 LOAD_METHOD              6 (append)
                      416 LOAD_FAST                3 (stmt)
                      418 PRECALL                  1
                      422 CALL                     1
                      432 POP_TOP
                      434 JUMP_BACKWARD          213 (to 10)
          
-         226     >>  436 LOAD_FAST                1 (new_stmt)
+         210     >>  436 LOAD_FAST                1 (new_stmt)
                      438 RETURN_VALUE
          ExceptionTable:
            20 to 122 -> 126 [1]
            126 to 148 -> 156 [2] lasti
            154 to 154 -> 156 [2] lasti
          consts
             '\n    Detect keywords used as variables, and make sure it is without space:\n\n    TYPE = 300 \n    becomes\n    TYPE= 300 \n    \n    This way, a true keyword is always followed by a space, and will be tetected,\n    but false keywords wont\n    '
@@ -1299,15 +1325,15 @@
             ' is used as a variable in the code. Bad Practice Should Be Avoided'
          names      ('split', 'IndexError', 'KEYWORDS_FTN', 'replace', 'logger', 'warning', 'append')
          varnames   ('lines', 'new_stmt', 'line', 'stmt', 'item0', 'item1')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
          name       'ftn_remove_space_in_front_of_variables'
-         firstlineno 198
+         firstlineno 182
          lnotab
             0x020b040108010401020134013801120108ff08031e01980116010aff10
             042c02
       code
          argcount  : 1
          nlocals   : 12
          stacksize : 6
@@ -1344,29 +1370,29 @@
             00ab01000000000000000001007c037219740f000000000000000000007c
             09a6010000ab0100000000000000007c036404190000000000000000006b
             0200000000b08590018ca47c01a005000000000000000000000000000000
             00000000007c08a6010000ab01000000000000000001007c02a005000000
             00000000000000000000000000000000007c067c076702a6010000ab0100
             00000000000000010090018cd27415000000000000000000007c017c02a6
             020000ab0200000000000000005300
-         230           0 RESUME                   0
+         214           0 RESUME                   0
          
-         254           2 BUILD_LIST               0
+         238           2 BUILD_LIST               0
                        4 STORE_FAST               1 (new_stmt)
          
-         255           6 BUILD_LIST               0
+         239           6 BUILD_LIST               0
                        8 STORE_FAST               2 (new_lines)
          
-         256          10 BUILD_LIST               0
+         240          10 BUILD_LIST               0
                       12 STORE_FAST               3 (do_loop_lbl)
          
-         257          14 BUILD_LIST               0
+         241          14 BUILD_LIST               0
                       16 STORE_FAST               4 (do_loop_indent)
          
-         258          18 LOAD_GLOBAL              1 (NULL + zip)
+         242          18 LOAD_GLOBAL              1 (NULL + zip)
                       30 LOAD_FAST                0 (stmts)
                       32 LOAD_ATTR                1 (stmt)
                       42 LOAD_FAST                0 (stmts)
                       44 LOAD_ATTR                2 (lines)
                       54 PRECALL                  2
                       58 CALL                     2
                       68 GET_ITER
@@ -1374,201 +1400,201 @@
                       72 FOR_ITER               464 (to 1002)
                       74 UNPACK_SEQUENCE          2
                       78 STORE_FAST               5 (line)
                       80 UNPACK_SEQUENCE          2
                       84 STORE_FAST               6 (lstart)
                       86 STORE_FAST               7 (lend)
          
-         259          88 LOAD_FAST                5 (line)
+         243          88 LOAD_FAST                5 (line)
                       90 STORE_FAST               8 (stmt)
          
-         261          92 NOP
+         245          92 NOP
          
-         262          94 LOAD_FAST                5 (line)
+         246          94 LOAD_FAST                5 (line)
                       96 LOAD_METHOD              3 (split)
                      118 PRECALL                  0
                      122 CALL                     0
                      132 LOAD_CONST               1 (0)
                      134 BINARY_SUBSCR
                      144 STORE_FAST               9 (item0)
          
-         263         146 LOAD_FAST                5 (line)
+         247         146 LOAD_FAST                5 (line)
                      148 LOAD_METHOD              3 (split)
                      170 PRECALL                  0
                      174 CALL                     0
                      184 LOAD_CONST               2 (1)
                      186 BINARY_SUBSCR
                      196 STORE_FAST              10 (item1)
                      198 JUMP_FORWARD            60 (to 320)
                  >>  200 PUSH_EXC_INFO
          
-         264         202 LOAD_GLOBAL              8 (IndexError)
+         248         202 LOAD_GLOBAL              8 (IndexError)
                      214 CHECK_EXC_MATCH
                      216 POP_JUMP_FORWARD_IF_FALSE    47 (to 312)
                      218 POP_TOP
          
-         265         220 LOAD_FAST                1 (new_stmt)
+         249         220 LOAD_FAST                1 (new_stmt)
                      222 LOAD_METHOD              5 (append)
                      244 LOAD_FAST                8 (stmt)
                      246 PRECALL                  1
                      250 CALL                     1
                      260 POP_TOP
          
-         266         262 LOAD_FAST                2 (new_lines)
+         250         262 LOAD_FAST                2 (new_lines)
                      264 LOAD_METHOD              5 (append)
                      286 LOAD_FAST                6 (lstart)
                      288 LOAD_FAST                7 (lend)
                      290 BUILD_LIST               2
                      292 PRECALL                  1
                      296 CALL                     1
                      306 POP_TOP
          
-         267         308 POP_EXCEPT
+         251         308 POP_EXCEPT
                      310 JUMP_BACKWARD          121 (to 70)
          
-         264     >>  312 RERAISE                  0
+         248     >>  312 RERAISE                  0
                  >>  314 COPY                     3
                      316 POP_EXCEPT
                      318 RERAISE                  1
          
-         269     >>  320 LOAD_FAST                9 (item0)
+         253     >>  320 LOAD_FAST                9 (item0)
                      322 LOAD_CONST               3 ('do')
                      324 COMPARE_OP               2 (==)
                      330 POP_JUMP_FORWARD_IF_FALSE    90 (to 512)
          
-         270         332 LOAD_FAST               10 (item1)
+         254         332 LOAD_FAST               10 (item1)
                      334 LOAD_METHOD              6 (isdigit)
                      356 PRECALL                  0
                      360 CALL                     0
                      370 POP_JUMP_FORWARD_IF_FALSE    70 (to 512)
          
-         271         372 LOAD_GLOBAL             15 (NULL + int)
+         255         372 LOAD_GLOBAL             15 (NULL + int)
                      384 LOAD_FAST               10 (item1)
                      386 PRECALL                  1
                      390 CALL                     1
                      400 STORE_FAST              11 (value)
          
-         272         402 LOAD_FAST                3 (do_loop_lbl)
+         256         402 LOAD_FAST                3 (do_loop_lbl)
                      404 LOAD_METHOD              5 (append)
                      426 LOAD_FAST               11 (value)
                      428 PRECALL                  1
                      432 CALL                     1
                      442 POP_TOP
          
-         273         444 LOAD_FAST                4 (do_loop_indent)
+         257         444 LOAD_FAST                4 (do_loop_indent)
                      446 LOAD_METHOD              5 (append)
                      468 LOAD_GLOBAL             17 (NULL + get_indent)
                      480 LOAD_FAST                5 (line)
                      482 PRECALL                  1
                      486 CALL                     1
                      496 PRECALL                  1
                      500 CALL                     1
                      510 POP_TOP
          
-         276     >>  512 LOAD_FAST                9 (item0)
+         260     >>  512 LOAD_FAST                9 (item0)
                      514 LOAD_METHOD              6 (isdigit)
                      536 PRECALL                  0
                      540 CALL                     0
                      550 POP_JUMP_FORWARD_IF_FALSE   179 (to 910)
                      552 LOAD_FAST                3 (do_loop_lbl)
                      554 POP_JUMP_FORWARD_IF_FALSE   177 (to 910)
          
-         277         556 LOAD_GLOBAL             15 (NULL + int)
+         261         556 LOAD_GLOBAL             15 (NULL + int)
                      568 LOAD_FAST                9 (item0)
                      570 PRECALL                  1
                      574 CALL                     1
                      584 STORE_FAST              11 (value)
          
-         278         586 LOAD_FAST                3 (do_loop_lbl)
+         262         586 LOAD_FAST                3 (do_loop_lbl)
                      588 POP_JUMP_FORWARD_IF_FALSE   158 (to 906)
                      590 LOAD_GLOBAL             15 (NULL + int)
                      602 LOAD_FAST                9 (item0)
                      604 PRECALL                  1
                      608 CALL                     1
                      618 LOAD_FAST                3 (do_loop_lbl)
                      620 LOAD_CONST               4 (-1)
                      622 BINARY_SUBSCR
                      632 COMPARE_OP               2 (==)
                      638 POP_JUMP_FORWARD_IF_FALSE   133 (to 906)
          
-         279     >>  640 LOAD_FAST                4 (do_loop_indent)
+         263     >>  640 LOAD_FAST                4 (do_loop_indent)
                      642 LOAD_CONST               4 (-1)
                      644 BINARY_SUBSCR
                      654 LOAD_CONST               5 ('end do ! ')
                      656 LOAD_FAST                3 (do_loop_lbl)
                      658 LOAD_CONST               4 (-1)
                      660 BINARY_SUBSCR
                      670 FORMAT_VALUE             0
                      672 BUILD_STRING             2
                      674 BINARY_OP                0 (+)
                      678 STORE_FAST               8 (stmt)
          
-         280         680 LOAD_FAST                4 (do_loop_indent)
+         264         680 LOAD_FAST                4 (do_loop_indent)
                      682 LOAD_METHOD              9 (pop)
                      704 LOAD_CONST               4 (-1)
                      706 PRECALL                  1
                      710 CALL                     1
                      720 POP_TOP
          
-         281         722 LOAD_FAST                3 (do_loop_lbl)
+         265         722 LOAD_FAST                3 (do_loop_lbl)
                      724 LOAD_METHOD              9 (pop)
                      746 LOAD_CONST               4 (-1)
                      748 PRECALL                  1
                      752 CALL                     1
                      762 POP_TOP
          
-         282         764 LOAD_FAST                1 (new_stmt)
+         266         764 LOAD_FAST                1 (new_stmt)
                      766 LOAD_METHOD              5 (append)
                      788 LOAD_FAST                8 (stmt)
                      790 PRECALL                  1
                      794 CALL                     1
                      804 POP_TOP
          
-         283         806 LOAD_FAST                2 (new_lines)
+         267         806 LOAD_FAST                2 (new_lines)
                      808 LOAD_METHOD              5 (append)
                      830 LOAD_FAST                6 (lstart)
                      832 LOAD_FAST                7 (lend)
                      834 BUILD_LIST               2
                      836 PRECALL                  1
                      840 CALL                     1
                      850 POP_TOP
          
-         278         852 LOAD_FAST                3 (do_loop_lbl)
+         262         852 LOAD_FAST                3 (do_loop_lbl)
                      854 POP_JUMP_FORWARD_IF_FALSE    25 (to 906)
                      856 LOAD_GLOBAL             15 (NULL + int)
                      868 LOAD_FAST                9 (item0)
                      870 PRECALL                  1
                      874 CALL                     1
                      884 LOAD_FAST                3 (do_loop_lbl)
                      886 LOAD_CONST               4 (-1)
                      888 BINARY_SUBSCR
                      898 COMPARE_OP               2 (==)
                      904 POP_JUMP_BACKWARD_IF_TRUE   133 (to 640)
                  >>  906 EXTENDED_ARG             1
                      908 JUMP_BACKWARD          420 (to 70)
          
-         286     >>  910 LOAD_FAST                1 (new_stmt)
+         270     >>  910 LOAD_FAST                1 (new_stmt)
                      912 LOAD_METHOD              5 (append)
                      934 LOAD_FAST                8 (stmt)
                      936 PRECALL                  1
                      940 CALL                     1
                      950 POP_TOP
          
-         287         952 LOAD_FAST                2 (new_lines)
+         271         952 LOAD_FAST                2 (new_lines)
                      954 LOAD_METHOD              5 (append)
                      976 LOAD_FAST                6 (lstart)
                      978 LOAD_FAST                7 (lend)
                      980 BUILD_LIST               2
                      982 PRECALL                  1
                      986 CALL                     1
                      996 POP_TOP
                      998 EXTENDED_ARG             1
                     1000 JUMP_BACKWARD          466 (to 70)
          
-         289     >> 1002 LOAD_GLOBAL             21 (NULL + Statements)
+         273     >> 1002 LOAD_GLOBAL             21 (NULL + Statements)
                     1014 LOAD_FAST                1 (new_stmt)
                     1016 LOAD_FAST                2 (new_lines)
                     1018 PRECALL                  2
                     1022 CALL                     2
                     1032 RETURN_VALUE
          ExceptionTable:
            94 to 196 -> 200 [1]
@@ -1583,15 +1609,15 @@
             'end do ! '
          names      ('zip', 'stmt', 'lines', 'split', 'IndexError', 'append', 'isdigit', 'int', 'get_indent', 'pop', 'Statements')
          varnames   ('stmts', 'new_stmt', 'new_lines', 'do_loop_lbl', 'do_loop_indent', 'line', 'lstart', 'lend', 'stmt', 'item0', 'item1', 'value')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
          name       'ftn_clean_labelled_loops_oldftn'
-         firstlineno 230
+         firstlineno 214
          lnotab
             0x021804010401040104014601040202013401380112012a012e0104fd08
             050c0128011e012a0144032c011e01360128012a012a012a012efb3a082a
             013202
       code
          argcount  : 1
          nlocals   : 5
@@ -1610,33 +1636,33 @@
             000000000000000000a6000000ab00000000000000000064011900000000
             0000000000a6010000ab01000000000000000064027a050000a6020000ab
             02000000000000000064037a0000007c02a0010000000000000000000000
             000000000000000000a6000000ab00000000000000000064011900000000
             00000000007a00000064047a0000007d038cbc7c01a00500000000000000
             000000000000000000000000007c03a6010000ab01000000000000000001
             008cdd7c015300
-         292           0 RESUME                   0
+         276           0 RESUME                   0
          
-         296           2 BUILD_LIST               0
+         280           2 BUILD_LIST               0
                        4 STORE_FAST               1 (new_stmt)
          
-         297           6 LOAD_FAST                0 (lines)
+         281           6 LOAD_FAST                0 (lines)
                        8 GET_ITER
                  >>   10 FOR_ITER               220 (to 452)
                       12 STORE_FAST               2 (line)
          
-         298          14 LOAD_FAST                2 (line)
+         282          14 LOAD_FAST                2 (line)
                       16 STORE_FAST               3 (stmt)
          
-         299          18 LOAD_GLOBAL              0 (KEYWORDS_FTN)
+         283          18 LOAD_GLOBAL              0 (KEYWORDS_FTN)
                       30 GET_ITER
                  >>   32 FOR_ITER               187 (to 408)
                       34 STORE_FAST               4 (keyword)
          
-         300          36 LOAD_FAST                4 (keyword)
+         284          36 LOAD_FAST                4 (keyword)
                       38 LOAD_FAST                2 (line)
                       40 LOAD_METHOD              1 (split)
                       62 PRECALL                  0
                       66 CALL                     0
                       76 CONTAINS_OP              0
                       78 POP_JUMP_FORWARD_IF_FALSE   163 (to 406)
                       80 LOAD_FAST                2 (line)
@@ -1646,15 +1672,15 @@
                      118 LOAD_CONST               1 (0)
                      120 BINARY_SUBSCR
                      130 LOAD_METHOD              2 (isdigit)
                      152 PRECALL                  0
                      156 CALL                     0
                      166 POP_JUMP_FORWARD_IF_FALSE   119 (to 406)
          
-         301         168 LOAD_FAST                2 (line)
+         285         168 LOAD_FAST                2 (line)
                      170 LOAD_METHOD              3 (replace)
                      192 LOAD_FAST                2 (line)
                      194 LOAD_METHOD              1 (split)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 LOAD_CONST               1 (0)
                      232 BINARY_SUBSCR
@@ -1681,927 +1707,1024 @@
                      384 BINARY_SUBSCR
                      394 BINARY_OP                0 (+)
                      398 LOAD_CONST               4 (')')
                      400 BINARY_OP                0 (+)
                      404 STORE_FAST               3 (stmt)
                  >>  406 JUMP_BACKWARD          188 (to 32)
          
-         302     >>  408 LOAD_FAST                1 (new_stmt)
+         286     >>  408 LOAD_FAST                1 (new_stmt)
                      410 LOAD_METHOD              5 (append)
                      432 LOAD_FAST                3 (stmt)
                      434 PRECALL                  1
                      438 CALL                     1
                      448 POP_TOP
                      450 JUMP_BACKWARD          221 (to 10)
          
-         303     >>  452 LOAD_FAST                1 (new_stmt)
+         287     >>  452 LOAD_FAST                1 (new_stmt)
                      454 RETURN_VALUE
          consts
             'Remove the GOTO references , put them at the end of the line\n    \n    '
             0
             ' '
             '  ! ('
             ')'
          names      ('KEYWORDS_FTN', 'split', 'isdigit', 'replace', 'len', 'append')
          varnames   ('lines', 'new_stmt', 'line', 'stmt', 'keyword')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
          name       'ftn_suppress_goto_references'
-         firstlineno 292
+         firstlineno 276
          lnotab 0x020404010801040112018401f0012c01
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 9
          flags     : 3
          code
-            0x970067007d01640d640374000000000000000000000064047400000000
+            0x970067007d01640c640374000000000000000000000064047400000000
             000000000000006405740000000000000000000000640674000000000000
-            00000000006608640784057d027c0044005d657d0302007c027c03640864
+            00000000006608640784057d027c0044005d587d0302007c027c03640864
             02a6030000ab0300000000000000007d0302007c027c0364016402a60300
             00ab0300000000000000007d0302007c027c0364096402a6030000ab0300
             000000000000007d0302007c027c03640a6402a6030000ab030000000000
             0000007d0302007c027c03640b6402a6030000ab0300000000000000007d
-            0302007c027c036409640ca6030000ab0300000000000000007d037c01a0
-            0100000000000000000000000000000000000000007c03a6010000ab0100
-            0000000000000001008c667c015300
-         307           0 RESUME                   0
+            037c01a00100000000000000000000000000000000000000007c03a60100
+            00ab01000000000000000001008c597c015300
+         291           0 RESUME                   0
          
-         312           2 BUILD_LIST               0
+         296           2 BUILD_LIST               0
                        4 STORE_FAST               1 (new_stmt)
          
-         314           6 LOAD_CONST              13 (('do', ':'))
+         298           6 LOAD_CONST              12 (('do', ':'))
                        8 LOAD_CONST               3 ('line')
                       10 LOAD_GLOBAL              0 (str)
                       22 LOAD_CONST               4 ('pattern')
                       24 LOAD_GLOBAL              0 (str)
                       36 LOAD_CONST               5 ('sep')
                       38 LOAD_GLOBAL              0 (str)
                       50 LOAD_CONST               6 ('return')
                       52 LOAD_GLOBAL              0 (str)
                       64 BUILD_TUPLE              8
-                      66 LOAD_CONST               7 (<code object _move_labels, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 314>)
+                      66 LOAD_CONST               7 (<code object _move_labels, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 298>)
                       68 MAKE_FUNCTION            5 (defaults, annotations)
                       70 STORE_FAST               2 (_move_labels)
          
-         326          72 LOAD_FAST                0 (lines)
+         321          72 LOAD_FAST                0 (lines)
                       74 GET_ITER
-                 >>   76 FOR_ITER               101 (to 280)
+                 >>   76 FOR_ITER                88 (to 254)
                       78 STORE_FAST               3 (line)
          
-         328          80 PUSH_NULL
+         323          80 PUSH_NULL
                       82 LOAD_FAST                2 (_move_labels)
                       84 LOAD_FAST                3 (line)
                       86 LOAD_CONST               8 ('block')
                       88 LOAD_CONST               2 (':')
                       90 PRECALL                  3
                       94 CALL                     3
                      104 STORE_FAST               3 (line)
          
-         329         106 PUSH_NULL
+         324         106 PUSH_NULL
                      108 LOAD_FAST                2 (_move_labels)
                      110 LOAD_FAST                3 (line)
                      112 LOAD_CONST               1 ('do')
                      114 LOAD_CONST               2 (':')
                      116 PRECALL                  3
                      120 CALL                     3
                      130 STORE_FAST               3 (line)
          
-         330         132 PUSH_NULL
+         325         132 PUSH_NULL
                      134 LOAD_FAST                2 (_move_labels)
                      136 LOAD_FAST                3 (line)
                      138 LOAD_CONST               9 ('if')
                      140 LOAD_CONST               2 (':')
                      142 PRECALL                  3
                      146 CALL                     3
                      156 STORE_FAST               3 (line)
          
-         331         158 PUSH_NULL
+         326         158 PUSH_NULL
                      160 LOAD_FAST                2 (_move_labels)
                      162 LOAD_FAST                3 (line)
                      164 LOAD_CONST              10 ('entry')
                      166 LOAD_CONST               2 (':')
                      168 PRECALL                  3
                      172 CALL                     3
                      182 STORE_FAST               3 (line)
          
-         332         184 PUSH_NULL
+         327         184 PUSH_NULL
                      186 LOAD_FAST                2 (_move_labels)
                      188 LOAD_FAST                3 (line)
                      190 LOAD_CONST              11 ('select_case')
                      192 LOAD_CONST               2 (':')
                      194 PRECALL                  3
                      198 CALL                     3
                      208 STORE_FAST               3 (line)
          
-         333         210 PUSH_NULL
-                     212 LOAD_FAST                2 (_move_labels)
-                     214 LOAD_FAST                3 (line)
-                     216 LOAD_CONST               9 ('if')
-                     218 LOAD_CONST              12 ('=')
-                     220 PRECALL                  3
-                     224 CALL                     3
-                     234 STORE_FAST               3 (line)
-         
-         335         236 LOAD_FAST                1 (new_stmt)
-                     238 LOAD_METHOD              1 (append)
-                     260 LOAD_FAST                3 (line)
-                     262 PRECALL                  1
-                     266 CALL                     1
-                     276 POP_TOP
-                     278 JUMP_BACKWARD          102 (to 76)
+         328         210 LOAD_FAST                1 (new_stmt)
+                     212 LOAD_METHOD              1 (append)
+                     234 LOAD_FAST                3 (line)
+                     236 PRECALL                  1
+                     240 CALL                     1
+                     250 POP_TOP
+                     252 JUMP_BACKWARD           89 (to 76)
          
-         337     >>  280 LOAD_FAST                1 (new_stmt)
-                     282 RETURN_VALUE
+         330     >>  254 LOAD_FAST                1 (new_stmt)
+                     256 RETURN_VALUE
          consts
             ' Move modern labels at the end of the line \n    \n     We keep label to show the name in struct\n    '
             'do'
             ':'
             'line'
             'pattern'
             'sep'
             'return'
             code
                argcount  : 3
-               nlocals   : 5
+               nlocals   : 8
                stacksize : 4
                flags     : 19
                code
-                  0x97007c027c017a00000064017a0000007c00760073247c0264017a0000
-                  007c017a00000064017a0000007c00760073177c027c017a00000064027a
-                  0000007c007600730d7c0264017a0000007c017a00000064027a0000007c
-                  00760072777c00a00000000000000000000000000000000000000000007c
-                  02a6010000ab010000000000000000640319000000000000000000a00100
-                  00000000000000000000000000000000000000a6000000ab000000000000
-                  0000007d037c00a00200000000000000000000000000000000000000007c
-                  02a6010000ab0100000000000000007d047407000000000000000000007c
-                  00a6010000ab0100000000000000007c007c0464047a0000006400850219
-                  000000000000000000a00400000000000000000000000000000000000000
-                  00a6000000ab0000000000000000007a00000064057a0000007c037a0000
-                  007d007c005300
-               314           0 RESUME                   0
-               
-               315           2 LOAD_FAST                2 (sep)
-                             4 LOAD_FAST                1 (pattern)
-                             6 BINARY_OP                0 (+)
-                            10 LOAD_CONST               1 (' ')
-                            12 BINARY_OP                0 (+)
-                            16 LOAD_FAST                0 (line)
-                            18 CONTAINS_OP              0
-                            20 POP_JUMP_FORWARD_IF_TRUE    36 (to 94)
-               
-               316          22 LOAD_FAST                2 (sep)
-                            24 LOAD_CONST               1 (' ')
-                            26 BINARY_OP                0 (+)
-                            30 LOAD_FAST                1 (pattern)
-                            32 BINARY_OP                0 (+)
-                            36 LOAD_CONST               1 (' ')
-                            38 BINARY_OP                0 (+)
-                            42 LOAD_FAST                0 (line)
-                            44 CONTAINS_OP              0
-                            46 POP_JUMP_FORWARD_IF_TRUE    23 (to 94)
-               
-               317          48 LOAD_FAST                2 (sep)
-                            50 LOAD_FAST                1 (pattern)
-                            52 BINARY_OP                0 (+)
-                            56 LOAD_CONST               2 ('(')
-                            58 BINARY_OP                0 (+)
-                            62 LOAD_FAST                0 (line)
-                            64 CONTAINS_OP              0
-                            66 POP_JUMP_FORWARD_IF_TRUE    13 (to 94)
-               
-               318          68 LOAD_FAST                2 (sep)
-                            70 LOAD_CONST               1 (' ')
-                            72 BINARY_OP                0 (+)
-                            76 LOAD_FAST                1 (pattern)
-                            78 BINARY_OP                0 (+)
-                            82 LOAD_CONST               2 ('(')
-                            84 BINARY_OP                0 (+)
-                            88 LOAD_FAST                0 (line)
-                            90 CONTAINS_OP              0
-                            92 POP_JUMP_FORWARD_IF_FALSE   119 (to 332)
-               
-               321     >>   94 LOAD_FAST                0 (line)
-                            96 LOAD_METHOD              0 (split)
-                           118 LOAD_FAST                2 (sep)
-                           120 PRECALL                  1
-                           124 CALL                     1
-                           134 LOAD_CONST               3 (0)
-                           136 BINARY_SUBSCR
-                           146 LOAD_METHOD              1 (strip)
-                           168 PRECALL                  0
-                           172 CALL                     0
-                           182 STORE_FAST               3 (label)
-               
-               322         184 LOAD_FAST                0 (line)
-                           186 LOAD_METHOD              2 (find)
-                           208 LOAD_FAST                2 (sep)
-                           210 PRECALL                  1
-                           214 CALL                     1
-                           224 STORE_FAST               4 (index)
-               
-               323         226 LOAD_GLOBAL              7 (NULL + get_indent)
-                           238 LOAD_FAST                0 (line)
-                           240 PRECALL                  1
-                           244 CALL                     1
-                           254 LOAD_FAST                0 (line)
-                           256 LOAD_FAST                4 (index)
-                           258 LOAD_CONST               4 (1)
-                           260 BINARY_OP                0 (+)
-                           264 LOAD_CONST               0 (None)
-                           266 BUILD_SLICE              2
-                           268 BINARY_SUBSCR
-                           278 LOAD_METHOD              4 (rstrip)
-                           300 PRECALL                  0
-                           304 CALL                     0
-                           314 BINARY_OP                0 (+)
-                           318 LOAD_CONST               5 (' #LABEL :')
-                           320 BINARY_OP                0 (+)
-                           324 LOAD_FAST                3 (label)
+                  0x97007c017c00760173047c027c00760172027c0053007c00a000000000
+                  00000000000000000000000000000000007c02a6010000ab010000000000
+                  000000640119000000000000000000a00100000000000000000000000000
+                  00000000000000a6000000ab0000000000000000007d0364027d047c0344
+                  005d0d7d057c0564037600720201006e067c047c057a0d00007d048c0e7c
+                  047c016b020000000072777c00a000000000000000000000000000000000
+                  00000000007c02a6010000ab010000000000000000640419000000000000
+                  000000a0020000000000000000000000000000000000000000a6000000ab
+                  0000000000000000007d067c00a003000000000000000000000000000000
+                  00000000007c02a6010000ab0100000000000000007d0774090000000000
+                  00000000007c00a6010000ab0100000000000000007c007c0764017a0000
+                  006405850219000000000000000000a00100000000000000000000000000
+                  00000000000000a6000000ab0000000000000000007a00000064067a0000
+                  007c067a0000007d007c005300
+               298           0 RESUME                   0
+               
+               304           2 LOAD_FAST                1 (pattern)
+                             4 LOAD_FAST                0 (line)
+                             6 CONTAINS_OP              1
+                             8 POP_JUMP_FORWARD_IF_TRUE     4 (to 18)
+                            10 LOAD_FAST                2 (sep)
+                            12 LOAD_FAST                0 (line)
+                            14 CONTAINS_OP              1
+                            16 POP_JUMP_FORWARD_IF_FALSE     2 (to 22)
+               
+               305     >>   18 LOAD_FAST                0 (line)
+                            20 RETURN_VALUE
+               
+               307     >>   22 LOAD_FAST                0 (line)
+                            24 LOAD_METHOD              0 (split)
+                            46 LOAD_FAST                2 (sep)
+                            48 PRECALL                  1
+                            52 CALL                     1
+                            62 LOAD_CONST               1 (1)
+                            64 BINARY_SUBSCR
+                            74 LOAD_METHOD              1 (rstrip)
+                            96 PRECALL                  0
+                           100 CALL                     0
+                           110 STORE_FAST               3 (rhs)
+               
+               308         112 LOAD_CONST               2 ('')
+                           114 STORE_FAST               4 (rhs1)
+               
+               309         116 LOAD_FAST                3 (rhs)
+                           118 GET_ITER
+                       >>  120 FOR_ITER                13 (to 148)
+                           122 STORE_FAST               5 (char)
+               
+               310         124 LOAD_FAST                5 (char)
+                           126 LOAD_CONST               3 (' (')
+                           128 CONTAINS_OP              0
+                           130 POP_JUMP_FORWARD_IF_FALSE     2 (to 136)
+               
+               311         132 POP_TOP
+                           134 JUMP_FORWARD             6 (to 148)
+               
+               312     >>  136 LOAD_FAST                4 (rhs1)
+                           138 LOAD_FAST                5 (char)
+                           140 BINARY_OP               13 (+=)
+                           144 STORE_FAST               4 (rhs1)
+                           146 JUMP_BACKWARD           14 (to 120)
+               
+               314     >>  148 LOAD_FAST                4 (rhs1)
+                           150 LOAD_FAST                1 (pattern)
+                           152 COMPARE_OP               2 (==)
+                           158 POP_JUMP_FORWARD_IF_FALSE   119 (to 398)
+               
+               316         160 LOAD_FAST                0 (line)
+                           162 LOAD_METHOD              0 (split)
+                           184 LOAD_FAST                2 (sep)
+                           186 PRECALL                  1
+                           190 CALL                     1
+                           200 LOAD_CONST               4 (0)
+                           202 BINARY_SUBSCR
+                           212 LOAD_METHOD              2 (strip)
+                           234 PRECALL                  0
+                           238 CALL                     0
+                           248 STORE_FAST               6 (label)
+               
+               317         250 LOAD_FAST                0 (line)
+                           252 LOAD_METHOD              3 (find)
+                           274 LOAD_FAST                2 (sep)
+                           276 PRECALL                  1
+                           280 CALL                     1
+                           290 STORE_FAST               7 (index)
+               
+               318         292 LOAD_GLOBAL              9 (NULL + get_indent)
+                           304 LOAD_FAST                0 (line)
+                           306 PRECALL                  1
+                           310 CALL                     1
+                           320 LOAD_FAST                0 (line)
+                           322 LOAD_FAST                7 (index)
+                           324 LOAD_CONST               1 (1)
                            326 BINARY_OP                0 (+)
-                           330 STORE_FAST               0 (line)
+                           330 LOAD_CONST               5 (None)
+                           332 BUILD_SLICE              2
+                           334 BINARY_SUBSCR
+                           344 LOAD_METHOD              1 (rstrip)
+                           366 PRECALL                  0
+                           370 CALL                     0
+                           380 BINARY_OP                0 (+)
+                           384 LOAD_CONST               6 (' ! NESTING_LABEL# ')
+                           386 BINARY_OP                0 (+)
+                           390 LOAD_FAST                6 (label)
+                           392 BINARY_OP                0 (+)
+                           396 STORE_FAST               0 (line)
                
-               324     >>  332 LOAD_FAST                0 (line)
-                           334 RETURN_VALUE
+               319     >>  398 LOAD_FAST                0 (line)
+                           400 RETURN_VALUE
                consts
-                  None
-                  ' '
-                  '('
-                  0
+                  '\n        eigenvalues: block\n\n        becomes block ! NESTING_LABEL# eigenvalues\n        '
                   1
-                  ' #LABEL :'
-               names      ('split', 'strip', 'find', 'get_indent', 'rstrip')
-               varnames   ('line', 'pattern', 'sep', 'label', 'index')
+                  ''
+                  ' ('
+                  0
+                  None
+                  ' ! NESTING_LABEL# '
+               names      ('split', 'rstrip', 'strip', 'find', 'get_indent')
+               varnames   ('line', 'pattern', 'sep', 'rhs', 'rhs1', 'char', 'label', 'index')
                freevars   ()
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
                name       '_move_labels'
-               firstlineno 314
-               lnotab 0x020114011a0114011a035a012a016a01
+               firstlineno 298
+               lnotab 0x0206100104025a0104010801080104010c020c025a012a016a01
             'block'
             'if'
             'entry'
             'select_case'
-            '='
             ('do', ':')
          names      ('str', 'append')
          varnames   ('lines', 'new_stmt', '_move_labels', 'line')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
          name       'ftn_clean_labelled_loops_newftn'
-         firstlineno 307
-         lnotab 0x02050402420c08021a011a011a011a011a011a022c02
+         firstlineno 291
+         lnotab 0x02050402421708021a011a011a011a011a012c02
       code
          argcount  : 1
-         nlocals   : 4
-         stacksize : 9
+         nlocals   : 3
+         stacksize : 5
          flags     : 3
          code
-            0x970067007d016448640374000000000000000000000064047400000000
-            000000000000006405740000000000000000000000640674000000000000
-            00000000006608640784057d027c00440090035d267d037c03a001000000
-            000000000000000000000000000000000064086409a6020000ab02000000
-            00000000007d037c03a00100000000000000000000000000000000000000
-            00640a640ba6020000ab0200000000000000007d037c03a0010000000000
-            000000000000000000000000000000640c640da6020000ab020000000000
-            0000007d037c03a001000000000000000000000000000000000000000064
-            0e640fa6020000ab0200000000000000007d037c03a00100000000000000
-            000000000000000000000000006410640fa6020000ab0200000000000000
-            007d037c03a0010000000000000000000000000000000000000000641164
-            0fa6020000ab0200000000000000007d037c03a001000000000000000000
-            00000000000000000000006412640fa6020000ab0200000000000000007d
-            037c03a001000000000000000000000000000000000000000064136414a6
-            020000ab0200000000000000007d037c03a0010000000000000000000000
-            00000000000000000064156414a6020000ab0200000000000000007d037c
-            03a001000000000000000000000000000000000000000064166417a60200
-            00ab0200000000000000007d037c03a00100000000000000000000000000
-            0000000000000064186419a6020000ab0200000000000000007d037c03a0
-            010000000000000000000000000000000000000000641a641ba6020000ab
-            0200000000000000007d037c03a001000000000000000000000000000000
-            0000000000641c641da6020000ab0200000000000000007d037c03a00100
-            00000000000000000000000000000000000000641e641fa6020000ab0200
-            000000000000007d037c03a0010000000000000000000000000000000000
-            00000064206421a6020000ab0200000000000000007d037c03a001000000
-            000000000000000000000000000000000064226423a6020000ab02000000
-            00000000007d037c03a00100000000000000000000000000000000000000
-            0064246425a6020000ab0200000000000000007d037c03a0010000000000
-            00000000000000000000000000000064266427a6020000ab020000000000
+            0x970067007d017c0044005d857d027c02a0000000000000000000000000
+            00000000000000000064016402a6020000ab0200000000000000007d027c
+            02a000000000000000000000000000000000000000000064036404a60200
+            00ab0200000000000000007d027c02a00000000000000000000000000000
+            0000000000000064056406a6020000ab0200000000000000007d027c02a0
+            00000000000000000000000000000000000000000064076408a6020000ab
+            0200000000000000007d027c02a000000000000000000000000000000000
+            00000000006409640aa6020000ab0200000000000000007d027c01a00100
+            000000000000000000000000000000000000007c02a6010000ab01000000
+            000000000001008c867c015300
+         332           0 RESUME                   0
+         
+         334           2 BUILD_LIST               0
+                       4 STORE_FAST               1 (new_stmt)
+         
+         335           6 LOAD_FAST                0 (lines)
+                       8 GET_ITER
+                 >>   10 FOR_ITER               133 (to 278)
+                      12 STORE_FAST               2 (line)
+         
+         336          14 LOAD_FAST                2 (line)
+                      16 LOAD_METHOD              0 (replace)
+                      38 LOAD_CONST               1 ('::')
+                      40 LOAD_CONST               2 (' :: ')
+                      42 PRECALL                  2
+                      46 CALL                     2
+                      56 STORE_FAST               2 (line)
+         
+         337          58 LOAD_FAST                2 (line)
+                      60 LOAD_METHOD              0 (replace)
+                      82 LOAD_CONST               3 ('==')
+                      84 LOAD_CONST               4 ('.eq.')
+                      86 PRECALL                  2
+                      90 CALL                     2
+                     100 STORE_FAST               2 (line)
+         
+         338         102 LOAD_FAST                2 (line)
+                     104 LOAD_METHOD              0 (replace)
+                     126 LOAD_CONST               5 ('/=')
+                     128 LOAD_CONST               6 ('.ne.')
+                     130 PRECALL                  2
+                     134 CALL                     2
+                     144 STORE_FAST               2 (line)
+         
+         339         146 LOAD_FAST                2 (line)
+                     148 LOAD_METHOD              0 (replace)
+                     170 LOAD_CONST               7 ('>=')
+                     172 LOAD_CONST               8 ('.ge.')
+                     174 PRECALL                  2
+                     178 CALL                     2
+                     188 STORE_FAST               2 (line)
+         
+         340         190 LOAD_FAST                2 (line)
+                     192 LOAD_METHOD              0 (replace)
+                     214 LOAD_CONST               9 ('<=')
+                     216 LOAD_CONST              10 ('.le.')
+                     218 PRECALL                  2
+                     222 CALL                     2
+                     232 STORE_FAST               2 (line)
+         
+         342         234 LOAD_FAST                1 (new_stmt)
+                     236 LOAD_METHOD              1 (append)
+                     258 LOAD_FAST                2 (line)
+                     260 PRECALL                  1
+                     264 CALL                     1
+                     274 POP_TOP
+                     276 JUMP_BACKWARD          134 (to 10)
+         
+         344     >>  278 LOAD_FAST                1 (new_stmt)
+                     280 RETURN_VALUE
+         consts
+            None
+            '::'
+            ' :: '
+            '=='
+            '.eq.'
+            '/='
+            '.ne.'
+            '>='
+            '.ge.'
+            '<='
+            '.le.'
+         names      ('replace', 'append')
+         varnames   ('lines', 'new_stmt', 'line')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
+         name       'ftn_clean_operators'
+         firstlineno 332
+         lnotab 0x0202040108012c012c012c012c012c022c02
+      code
+         argcount  : 1
+         nlocals   : 5
+         stacksize : 7
+         flags     : 3
+         code
+            0x970067007d016401740000000000000000000000640274000000000000
+            000000000064037400000000000000000000006606640484047d027c0044
+            0090015da77d037c03a00100000000000000000000000000000000000000
+            0064056406a6020000ab0200000000000000007d037c03a0010000000000
+            00000000000000000000000000000064076408a6020000ab020000000000
             0000007d037c03a001000000000000000000000000000000000000000064
-            286429a6020000ab0200000000000000007d037c03a00100000000000000
-            00000000000000000000000000642a642ba6020000ab0200000000000000
-            007d037c03a0010000000000000000000000000000000000000000642c64
-            2da6020000ab0200000000000000007d037c03a001000000000000000000
-            0000000000000000000000642e642fa6020000ab0200000000000000007d
-            037c03a001000000000000000000000000000000000000000064306431a6
+            09640aa6020000ab0200000000000000007d037c03a00100000000000000
+            00000000000000000000000000640b640ca6020000ab0200000000000000
+            007d037c03a0010000000000000000000000000000000000000000640d64
+            0ea6020000ab0200000000000000007d037c03a001000000000000000000
+            0000000000000000000000640f6410a6020000ab0200000000000000007d
+            037c03a001000000000000000000000000000000000000000064116412a6
             020000ab0200000000000000007d037c03a0010000000000000000000000
-            00000000000000000064326433a6020000ab0200000000000000007d037c
-            03a001000000000000000000000000000000000000000064346435a60200
+            00000000000000000064136414a6020000ab0200000000000000007d037c
+            03a001000000000000000000000000000000000000000064156414a60200
             00ab0200000000000000007d037c03a00100000000000000000000000000
-            0000000000000064366437a6020000ab0200000000000000007d037c03a0
-            01000000000000000000000000000000000000000064386439a6020000ab
-            0200000000000000007d037c03a001000000000000000000000000000000
-            0000000000643a643ba6020000ab0200000000000000007d037c03a00100
-            00000000000000000000000000000000000000643c643da6020000ab0200
+            0000000000000064166417a6020000ab0200000000000000007d0302007c
+            027c036418a6020000ab0200000000000000007d0302007c027c036419a6
+            020000ab0200000000000000007d0302007c027c03641aa6020000ab0200
             000000000000007d037c03a0010000000000000000000000000000000000
-            000000643e643fa6020000ab0200000000000000007d037c03a001000000
-            000000000000000000000000000000000064406441a6020000ab02000000
+            000000641b641ca6020000ab0200000000000000007d037c03a001000000
+            0000000000000000000000000000000000641d641ea6020000ab02000000
             00000000007d037c03a00100000000000000000000000000000000000000
-            0064426443a6020000ab0200000000000000007d0302007c027c03644464
-            02a6030000ab0300000000000000007d0302007c027c0364016402a60300
-            00ab0300000000000000007d0302007c027c0364456402a6030000ab0300
-            000000000000007d0302007c027c0364466402a6030000ab030000000000
-            0000007d0302007c027c0364476402a6030000ab0300000000000000007d
-            0302007c027c0364456442a6030000ab0300000000000000007d037c01a0
-            0200000000000000000000000000000000000000007c03a6010000ab0100
-            00000000000000010090038c287c015300
-         339           0 RESUME                   0
+            00641f6420a6020000ab0200000000000000007d037c03a0010000000000
+            00000000000000000000000000000064216422a6020000ab020000000000
+            0000007d03642344005d1e7d047c03a00100000000000000000000000000
+            000000000000007c049b0064249d027c049b0064259d02a6020000ab0200
+            000000000000007d038c1f7c03a001000000000000000000000000000000
+            000000000064266427a6020000ab0200000000000000007d037c01a00200
+            000000000000000000000000000000000000007c03a6010000ab01000000
+            0000000000010090018ca97c015300
+         346           0 RESUME                   0
          
-         341           2 BUILD_LIST               0
+         348           2 BUILD_LIST               0
                        4 STORE_FAST               1 (new_stmt)
          
-         343           6 LOAD_CONST              72 (('do', ':'))
-                       8 LOAD_CONST               3 ('line')
-                      10 LOAD_GLOBAL              0 (str)
-                      22 LOAD_CONST               4 ('pattern')
-                      24 LOAD_GLOBAL              0 (str)
-                      36 LOAD_CONST               5 ('sep')
-                      38 LOAD_GLOBAL              0 (str)
-                      50 LOAD_CONST               6 ('return')
-                      52 LOAD_GLOBAL              0 (str)
-                      64 BUILD_TUPLE              8
-                      66 LOAD_CONST               7 (<code object _move_labels, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 343>)
-                      68 MAKE_FUNCTION            5 (defaults, annotations)
-                      70 STORE_FAST               2 (_move_labels)
-         
-         355          72 LOAD_FAST                0 (lines)
-                      74 GET_ITER
-                 >>   76 EXTENDED_ARG             3
-                      78 FOR_ITER               806 (to 1692)
-                      80 STORE_FAST               3 (line)
-         
-         356          82 LOAD_FAST                3 (line)
-                      84 LOAD_METHOD              1 (replace)
-                     106 LOAD_CONST               8 ('pure function')
-                     108 LOAD_CONST               9 ('function_pure ')
-                     110 PRECALL                  2
-                     114 CALL                     2
-                     124 STORE_FAST               3 (line)
-         
-         357         126 LOAD_FAST                3 (line)
-                     128 LOAD_METHOD              1 (replace)
-                     150 LOAD_CONST              10 ('elemental function')
-                     152 LOAD_CONST              11 ('function_elemental ')
-                     154 PRECALL                  2
-                     158 CALL                     2
-                     168 STORE_FAST               3 (line)
-         
-         358         170 LOAD_FAST                3 (line)
-                     172 LOAD_METHOD              1 (replace)
-                     194 LOAD_CONST              12 ('recursive function')
-                     196 LOAD_CONST              13 ('function_recursive ')
-                     198 PRECALL                  2
-                     202 CALL                     2
-                     212 STORE_FAST               3 (line)
-         
-         360         214 LOAD_FAST                3 (line)
-                     216 LOAD_METHOD              1 (replace)
-                     238 LOAD_CONST              14 ('double precision function')
-                     240 LOAD_CONST              15 ('function ')
-                     242 PRECALL                  2
-                     246 CALL                     2
-                     256 STORE_FAST               3 (line)
-         
-         361         258 LOAD_FAST                3 (line)
-                     260 LOAD_METHOD              1 (replace)
-                     282 LOAD_CONST              16 ('real function')
-                     284 LOAD_CONST              15 ('function ')
-                     286 PRECALL                  2
-                     290 CALL                     2
-                     300 STORE_FAST               3 (line)
-         
-         362         302 LOAD_FAST                3 (line)
-                     304 LOAD_METHOD              1 (replace)
-                     326 LOAD_CONST              17 ('integer function')
-                     328 LOAD_CONST              15 ('function ')
-                     330 PRECALL                  2
-                     334 CALL                     2
-                     344 STORE_FAST               3 (line)
-         
-         363         346 LOAD_FAST                3 (line)
-                     348 LOAD_METHOD              1 (replace)
-                     370 LOAD_CONST              18 ('logical function')
-                     372 LOAD_CONST              15 ('function ')
-                     374 PRECALL                  2
-                     378 CALL                     2
-                     388 STORE_FAST               3 (line)
-         
-         366         390 LOAD_FAST                3 (line)
-                     392 LOAD_METHOD              1 (replace)
-                     414 LOAD_CONST              19 ('selectcase')
-                     416 LOAD_CONST              20 ('select_case ')
-                     418 PRECALL                  2
-                     422 CALL                     2
-                     432 STORE_FAST               3 (line)
-         
-         367         434 LOAD_FAST                3 (line)
-                     436 LOAD_METHOD              1 (replace)
-                     458 LOAD_CONST              21 ('select case')
-                     460 LOAD_CONST              20 ('select_case ')
-                     462 PRECALL                  2
-                     466 CALL                     2
-                     476 STORE_FAST               3 (line)
-         
-         368         478 LOAD_FAST                3 (line)
-                     480 LOAD_METHOD              1 (replace)
-                     502 LOAD_CONST              22 ('select type')
-                     504 LOAD_CONST              23 ('select_type ')
-                     506 PRECALL                  2
-                     510 CALL                     2
-                     520 STORE_FAST               3 (line)
-         
-         370         522 LOAD_FAST                3 (line)
-                     524 LOAD_METHOD              1 (replace)
-                     546 LOAD_CONST              24 ('elemental subroutine')
-                     548 LOAD_CONST              25 ('subroutine_elemental ')
-                     550 PRECALL                  2
-                     554 CALL                     2
-                     564 STORE_FAST               3 (line)
-         
-         371         566 LOAD_FAST                3 (line)
-                     568 LOAD_METHOD              1 (replace)
-                     590 LOAD_CONST              26 ('recursive subroutine')
-                     592 LOAD_CONST              27 ('subroutine_recursive ')
-                     594 PRECALL                  2
-                     598 CALL                     2
-                     608 STORE_FAST               3 (line)
-         
-         373         610 LOAD_FAST                3 (line)
-                     612 LOAD_METHOD              1 (replace)
-                     634 LOAD_CONST              28 ('module procedure')
-                     636 LOAD_CONST              29 ('module_procedure ')
-                     638 PRECALL                  2
-                     642 CALL                     2
-                     652 STORE_FAST               3 (line)
-         
-         376         654 LOAD_FAST                3 (line)
-                     656 LOAD_METHOD              1 (replace)
-                     678 LOAD_CONST              30 ('double precision')
-                     680 LOAD_CONST              31 ('double_precision ')
-                     682 PRECALL                  2
-                     686 CALL                     2
-                     696 STORE_FAST               3 (line)
-         
-         378         698 LOAD_FAST                3 (line)
-                     700 LOAD_METHOD              1 (replace)
-                     722 LOAD_CONST              32 ('type,public,abstract')
-                     724 LOAD_CONST              33 ('type_public_abstract ')
-                     726 PRECALL                  2
-                     730 CALL                     2
-                     740 STORE_FAST               3 (line)
-         
-         379         742 LOAD_FAST                3 (line)
-                     744 LOAD_METHOD              1 (replace)
-                     766 LOAD_CONST              34 ('type,public')
-                     768 LOAD_CONST              35 ('type_public ')
-                     770 PRECALL                  2
-                     774 CALL                     2
-                     784 STORE_FAST               3 (line)
-         
-         380         786 LOAD_FAST                3 (line)
-                     788 LOAD_METHOD              1 (replace)
-                     810 LOAD_CONST              36 ('type,private,abstract')
-                     812 LOAD_CONST              37 ('type_private_abstract ')
-                     814 PRECALL                  2
-                     818 CALL                     2
-                     828 STORE_FAST               3 (line)
+         350           6 LOAD_CONST               1 ('line')
+                       8 LOAD_GLOBAL              0 (str)
+                      20 LOAD_CONST               2 ('keyword')
+                      22 LOAD_GLOBAL              0 (str)
+                      34 LOAD_CONST               3 ('return')
+                      36 LOAD_GLOBAL              0 (str)
+                      48 BUILD_TUPLE              6
+                      50 LOAD_CONST               4 (<code object _remove_decorators, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 350>)
+                      52 MAKE_FUNCTION            4 (annotations)
+                      54 STORE_FAST               2 (_remove_decorators)
+         
+         372          56 LOAD_FAST                0 (lines)
+                      58 GET_ITER
+                 >>   60 EXTENDED_ARG             1
+                      62 FOR_ITER               423 (to 910)
+                      64 STORE_FAST               3 (line)
+         
+         375          66 LOAD_FAST                3 (line)
+                      68 LOAD_METHOD              1 (replace)
+                      90 LOAD_CONST               5 ('double precision')
+                      92 LOAD_CONST               6 ('double_precision ')
+                      94 PRECALL                  2
+                      98 CALL                     2
+                     108 STORE_FAST               3 (line)
+         
+         376         110 LOAD_FAST                3 (line)
+                     112 LOAD_METHOD              1 (replace)
+                     134 LOAD_CONST               7 ('module procedure')
+                     136 LOAD_CONST               8 ('module_procedure ')
+                     138 PRECALL                  2
+                     142 CALL                     2
+                     152 STORE_FAST               3 (line)
+         
+         377         154 LOAD_FAST                3 (line)
+                     156 LOAD_METHOD              1 (replace)
+                     178 LOAD_CONST               9 ('type,public,abstract')
+                     180 LOAD_CONST              10 ('type_public_abstract ')
+                     182 PRECALL                  2
+                     186 CALL                     2
+                     196 STORE_FAST               3 (line)
+         
+         378         198 LOAD_FAST                3 (line)
+                     200 LOAD_METHOD              1 (replace)
+                     222 LOAD_CONST              11 ('type,public')
+                     224 LOAD_CONST              12 ('type_public ')
+                     226 PRECALL                  2
+                     230 CALL                     2
+                     240 STORE_FAST               3 (line)
+         
+         379         242 LOAD_FAST                3 (line)
+                     244 LOAD_METHOD              1 (replace)
+                     266 LOAD_CONST              13 ('type,private,abstract')
+                     268 LOAD_CONST              14 ('type_private_abstract ')
+                     270 PRECALL                  2
+                     274 CALL                     2
+                     284 STORE_FAST               3 (line)
+         
+         380         286 LOAD_FAST                3 (line)
+                     288 LOAD_METHOD              1 (replace)
+                     310 LOAD_CONST              15 ('type,private')
+                     312 LOAD_CONST              16 ('type_private ')
+                     314 PRECALL                  2
+                     318 CALL                     2
+                     328 STORE_FAST               3 (line)
+         
+         381         330 LOAD_FAST                3 (line)
+                     332 LOAD_METHOD              1 (replace)
+                     354 LOAD_CONST              17 ('type is')
+                     356 LOAD_CONST              18 ('type_is ')
+                     358 PRECALL                  2
+                     362 CALL                     2
+                     372 STORE_FAST               3 (line)
+         
+         382         374 LOAD_FAST                3 (line)
+                     376 LOAD_METHOD              1 (replace)
+                     398 LOAD_CONST              19 ('selectcase')
+                     400 LOAD_CONST              20 ('select_case ')
+                     402 PRECALL                  2
+                     406 CALL                     2
+                     416 STORE_FAST               3 (line)
+         
+         383         418 LOAD_FAST                3 (line)
+                     420 LOAD_METHOD              1 (replace)
+                     442 LOAD_CONST              21 ('select case')
+                     444 LOAD_CONST              20 ('select_case ')
+                     446 PRECALL                  2
+                     450 CALL                     2
+                     460 STORE_FAST               3 (line)
+         
+         384         462 LOAD_FAST                3 (line)
+                     464 LOAD_METHOD              1 (replace)
+                     486 LOAD_CONST              22 ('select type')
+                     488 LOAD_CONST              23 ('select_type ')
+                     490 PRECALL                  2
+                     494 CALL                     2
+                     504 STORE_FAST               3 (line)
+         
+         387         506 PUSH_NULL
+                     508 LOAD_FAST                2 (_remove_decorators)
+                     510 LOAD_FAST                3 (line)
+                     512 LOAD_CONST              24 ('function')
+                     514 PRECALL                  2
+                     518 CALL                     2
+                     528 STORE_FAST               3 (line)
          
-         381         830 LOAD_FAST                3 (line)
-                     832 LOAD_METHOD              1 (replace)
-                     854 LOAD_CONST              38 ('type,private')
-                     856 LOAD_CONST              39 ('type_private ')
-                     858 PRECALL                  2
-                     862 CALL                     2
-                     872 STORE_FAST               3 (line)
-         
-         383         874 LOAD_FAST                3 (line)
-                     876 LOAD_METHOD              1 (replace)
-                     898 LOAD_CONST              40 ('interface')
-                     900 LOAD_CONST              41 ('interface ')
-                     902 PRECALL                  2
-                     906 CALL                     2
-                     916 STORE_FAST               3 (line)
-         
-         384         918 LOAD_FAST                3 (line)
-                     920 LOAD_METHOD              1 (replace)
-                     942 LOAD_CONST              42 ('abstract interface')
-                     944 LOAD_CONST              43 ('interface_abstract ')
-                     946 PRECALL                  2
-                     950 CALL                     2
-                     960 STORE_FAST               3 (line)
-         
-         386         962 LOAD_FAST                3 (line)
-                     964 LOAD_METHOD              1 (replace)
-                     986 LOAD_CONST              44 ('enddo')
-                     988 LOAD_CONST              45 ('end do ')
-                     990 PRECALL                  2
-                     994 CALL                     2
-                    1004 STORE_FAST               3 (line)
-         
-         387        1006 LOAD_FAST                3 (line)
-                    1008 LOAD_METHOD              1 (replace)
-                    1030 LOAD_CONST              46 ('endif')
-                    1032 LOAD_CONST              47 ('end if ')
-                    1034 PRECALL                  2
-                    1038 CALL                     2
-                    1048 STORE_FAST               3 (line)
-         
-         388        1050 LOAD_FAST                3 (line)
-                    1052 LOAD_METHOD              1 (replace)
-                    1074 LOAD_CONST              48 ('endwhere')
-                    1076 LOAD_CONST              49 ('end where ')
-                    1078 PRECALL                  2
-                    1082 CALL                     2
-                    1092 STORE_FAST               3 (line)
-         
-         389        1094 LOAD_FAST                3 (line)
-                    1096 LOAD_METHOD              1 (replace)
-                    1118 LOAD_CONST              50 ('endmodule')
-                    1120 LOAD_CONST              51 ('end module ')
-                    1122 PRECALL                  2
-                    1126 CALL                     2
-                    1136 STORE_FAST               3 (line)
-         
-         391        1138 LOAD_FAST                3 (line)
-                    1140 LOAD_METHOD              1 (replace)
-                    1162 LOAD_CONST              52 ('associate(')
-                    1164 LOAD_CONST              53 ('associate (')
-                    1166 PRECALL                  2
-                    1170 CALL                     2
-                    1180 STORE_FAST               3 (line)
-         
-         392        1182 LOAD_FAST                3 (line)
-                    1184 LOAD_METHOD              1 (replace)
-                    1206 LOAD_CONST              54 ('if(')
-                    1208 LOAD_CONST              55 ('if (')
-                    1210 PRECALL                  2
-                    1214 CALL                     2
-                    1224 STORE_FAST               3 (line)
-         
-         393        1226 LOAD_FAST                3 (line)
-                    1228 LOAD_METHOD              1 (replace)
-                    1250 LOAD_CONST              56 ('do(')
-                    1252 LOAD_CONST              57 ('do (')
-                    1254 PRECALL                  2
-                    1258 CALL                     2
-                    1268 STORE_FAST               3 (line)
-         
-         394        1270 LOAD_FAST                3 (line)
-                    1272 LOAD_METHOD              1 (replace)
-                    1294 LOAD_CONST              58 ('type(')
-                    1296 LOAD_CONST              59 ('type (')
-                    1298 PRECALL                  2
-                    1302 CALL                     2
-                    1312 STORE_FAST               3 (line)
-         
-         395        1314 LOAD_FAST                3 (line)
-                    1316 LOAD_METHOD              1 (replace)
-                    1338 LOAD_CONST              60 ('type is')
-                    1340 LOAD_CONST              61 ('type_is ')
-                    1342 PRECALL                  2
-                    1346 CALL                     2
-                    1356 STORE_FAST               3 (line)
-         
-         397        1358 LOAD_FAST                3 (line)
-                    1360 LOAD_METHOD              1 (replace)
-                    1382 LOAD_CONST              62 (')then')
-                    1384 LOAD_CONST              63 (') then ')
-                    1386 PRECALL                  2
-                    1390 CALL                     2
-                    1400 STORE_FAST               3 (line)
-         
-         399        1402 LOAD_FAST                3 (line)
-                    1404 LOAD_METHOD              1 (replace)
-                    1426 LOAD_CONST              64 ('::')
-                    1428 LOAD_CONST              65 (' :: ')
-                    1430 PRECALL                  2
-                    1434 CALL                     2
-                    1444 STORE_FAST               3 (line)
-         
-         400        1446 LOAD_FAST                3 (line)
-                    1448 LOAD_METHOD              1 (replace)
-                    1470 LOAD_CONST              66 ('=')
-                    1472 LOAD_CONST              67 (' = ')
-                    1474 PRECALL                  2
-                    1478 CALL                     2
-                    1488 STORE_FAST               3 (line)
-         
-         402        1490 PUSH_NULL
-                    1492 LOAD_FAST                2 (_move_labels)
-                    1494 LOAD_FAST                3 (line)
-                    1496 LOAD_CONST              68 ('block')
-                    1498 LOAD_CONST               2 (':')
-                    1500 PRECALL                  3
-                    1504 CALL                     3
-                    1514 STORE_FAST               3 (line)
-         
-         403        1516 PUSH_NULL
-                    1518 LOAD_FAST                2 (_move_labels)
-                    1520 LOAD_FAST                3 (line)
-                    1522 LOAD_CONST               1 ('do')
-                    1524 LOAD_CONST               2 (':')
-                    1526 PRECALL                  3
-                    1530 CALL                     3
-                    1540 STORE_FAST               3 (line)
-         
-         404        1542 PUSH_NULL
-                    1544 LOAD_FAST                2 (_move_labels)
-                    1546 LOAD_FAST                3 (line)
-                    1548 LOAD_CONST              69 ('if')
-                    1550 LOAD_CONST               2 (':')
-                    1552 PRECALL                  3
-                    1556 CALL                     3
-                    1566 STORE_FAST               3 (line)
-         
-         405        1568 PUSH_NULL
-                    1570 LOAD_FAST                2 (_move_labels)
-                    1572 LOAD_FAST                3 (line)
-                    1574 LOAD_CONST              70 ('entry')
-                    1576 LOAD_CONST               2 (':')
-                    1578 PRECALL                  3
-                    1582 CALL                     3
-                    1592 STORE_FAST               3 (line)
-         
-         406        1594 PUSH_NULL
-                    1596 LOAD_FAST                2 (_move_labels)
-                    1598 LOAD_FAST                3 (line)
-                    1600 LOAD_CONST              71 ('select_case')
-                    1602 LOAD_CONST               2 (':')
-                    1604 PRECALL                  3
-                    1608 CALL                     3
-                    1618 STORE_FAST               3 (line)
-         
-         407        1620 PUSH_NULL
-                    1622 LOAD_FAST                2 (_move_labels)
-                    1624 LOAD_FAST                3 (line)
-                    1626 LOAD_CONST              69 ('if')
-                    1628 LOAD_CONST              66 ('=')
-                    1630 PRECALL                  3
-                    1634 CALL                     3
-                    1644 STORE_FAST               3 (line)
-         
-         409        1646 LOAD_FAST                1 (new_stmt)
-                    1648 LOAD_METHOD              2 (append)
-                    1670 LOAD_FAST                3 (line)
-                    1672 PRECALL                  1
-                    1676 CALL                     1
-                    1686 POP_TOP
-                    1688 EXTENDED_ARG             3
-                    1690 JUMP_BACKWARD          808 (to 76)
+         388         530 PUSH_NULL
+                     532 LOAD_FAST                2 (_remove_decorators)
+                     534 LOAD_FAST                3 (line)
+                     536 LOAD_CONST              25 ('subroutine')
+                     538 PRECALL                  2
+                     542 CALL                     2
+                     552 STORE_FAST               3 (line)
+         
+         389         554 PUSH_NULL
+                     556 LOAD_FAST                2 (_remove_decorators)
+                     558 LOAD_FAST                3 (line)
+                     560 LOAD_CONST              26 ('interface')
+                     562 PRECALL                  2
+                     566 CALL                     2
+                     576 STORE_FAST               3 (line)
+         
+         392         578 LOAD_FAST                3 (line)
+                     580 LOAD_METHOD              1 (replace)
+                     602 LOAD_CONST              27 ('enddo')
+                     604 LOAD_CONST              28 ('end do ')
+                     606 PRECALL                  2
+                     610 CALL                     2
+                     620 STORE_FAST               3 (line)
+         
+         393         622 LOAD_FAST                3 (line)
+                     624 LOAD_METHOD              1 (replace)
+                     646 LOAD_CONST              29 ('endif')
+                     648 LOAD_CONST              30 ('end if ')
+                     650 PRECALL                  2
+                     654 CALL                     2
+                     664 STORE_FAST               3 (line)
+         
+         394         666 LOAD_FAST                3 (line)
+                     668 LOAD_METHOD              1 (replace)
+                     690 LOAD_CONST              31 ('endwhere')
+                     692 LOAD_CONST              32 ('end where ')
+                     694 PRECALL                  2
+                     698 CALL                     2
+                     708 STORE_FAST               3 (line)
+         
+         395         710 LOAD_FAST                3 (line)
+                     712 LOAD_METHOD              1 (replace)
+                     734 LOAD_CONST              33 ('endmodule')
+                     736 LOAD_CONST              34 ('end module ')
+                     738 PRECALL                  2
+                     742 CALL                     2
+                     752 STORE_FAST               3 (line)
+         
+         398         754 LOAD_CONST              35 (('function', 'subroutine', 'interface', 'if', 'do', 'type', 'associate'))
+                     756 GET_ITER
+                 >>  758 FOR_ITER                30 (to 820)
+                     760 STORE_FAST               4 (keyword)
+         
+         407         762 LOAD_FAST                3 (line)
+                     764 LOAD_METHOD              1 (replace)
+                     786 LOAD_FAST                4 (keyword)
+                     788 FORMAT_VALUE             0
+                     790 LOAD_CONST              36 ('(')
+                     792 BUILD_STRING             2
+                     794 LOAD_FAST                4 (keyword)
+                     796 FORMAT_VALUE             0
+                     798 LOAD_CONST              37 (' (')
+                     800 BUILD_STRING             2
+                     802 PRECALL                  2
+                     806 CALL                     2
+                     816 STORE_FAST               3 (line)
+                     818 JUMP_BACKWARD           31 (to 758)
+         
+         409     >>  820 LOAD_FAST                3 (line)
+                     822 LOAD_METHOD              1 (replace)
+                     844 LOAD_CONST              38 (')then')
+                     846 LOAD_CONST              39 (') then ')
+                     848 PRECALL                  2
+                     852 CALL                     2
+                     862 STORE_FAST               3 (line)
+         
+         411         864 LOAD_FAST                1 (new_stmt)
+                     866 LOAD_METHOD              2 (append)
+                     888 LOAD_FAST                3 (line)
+                     890 PRECALL                  1
+                     894 CALL                     1
+                     904 POP_TOP
+                     906 EXTENDED_ARG             1
+                     908 JUMP_BACKWARD          425 (to 60)
          
-         411     >> 1692 LOAD_FAST                1 (new_stmt)
-                    1694 RETURN_VALUE
+         413     >>  910 LOAD_FAST                1 (new_stmt)
+                     912 RETURN_VALUE
          consts
             ' clean oddities in fortran declarations'
-            'do'
-            ':'
             'line'
-            'pattern'
-            'sep'
+            'keyword'
             'return'
             code
-               argcount  : 3
-               nlocals   : 5
-               stacksize : 4
+               argcount  : 2
+               nlocals   : 4
+               stacksize : 5
                flags     : 19
                code
-                  0x97007c027c017a00000064017a0000007c00760073247c0264017a0000
-                  007c017a00000064017a0000007c00760073177c027c017a00000064027a
-                  0000007c007600730d7c0264017a0000007c017a00000064027a0000007c
-                  00760072777c00a00000000000000000000000000000000000000000007c
-                  02a6010000ab010000000000000000640319000000000000000000a00100
+                  0x97007c017c00760172027c0053007c00a0000000000000000000000000
+                  000000000000000000a6000000ab000000000000000000a0010000000000
+                  0000000000000000000000000000006401a6010000ab0100000000000000
+                  00721e7c00a002000000000000000000000000000000000000000064017c
+                  017a00000064027c017a000000a6020000ab02000000000000000001007c
+                  0053007c00a0020000000000000000000000000000000000000000640364
+                  04a6020000ab020000000000000000a00200000000000000000000000000
+                  0000000000000064056404a6020000ab02000000000000000064047a0000
+                  007d027c02a003000000000000000000000000000000000000000064047c
+                  017a00000064047a000000a6010000ab0100000000000000007d037c0364
+                  066b020000000072027c0053007409000000000000000000007c00a60100
+                  00ab0100000000000000007c007c0364077a000000640885021900000000
+                  00000000007a00000064097a0000007c01a0050000000000000000000000
+                  000000000000000000a6000000ab0000000000000000007a000000640a7a
+                  0000007c0064087c0364077a000000850219000000000000000000a00000
                   00000000000000000000000000000000000000a6000000ab000000000000
-                  0000007d037c00a00200000000000000000000000000000000000000007c
-                  02a6010000ab0100000000000000007d047407000000000000000000007c
-                  00a6010000ab0100000000000000007c007c0464047a0000006400850219
-                  000000000000000000a00400000000000000000000000000000000000000
-                  00a6000000ab0000000000000000007a00000064057a0000007c037a0000
-                  007d007c005300
-               343           0 RESUME                   0
-               
-               344           2 LOAD_FAST                2 (sep)
-                             4 LOAD_FAST                1 (pattern)
-                             6 BINARY_OP                0 (+)
-                            10 LOAD_CONST               1 (' ')
-                            12 BINARY_OP                0 (+)
-                            16 LOAD_FAST                0 (line)
-                            18 CONTAINS_OP              0
-                            20 POP_JUMP_FORWARD_IF_TRUE    36 (to 94)
-               
-               345          22 LOAD_FAST                2 (sep)
-                            24 LOAD_CONST               1 (' ')
-                            26 BINARY_OP                0 (+)
-                            30 LOAD_FAST                1 (pattern)
-                            32 BINARY_OP                0 (+)
-                            36 LOAD_CONST               1 (' ')
-                            38 BINARY_OP                0 (+)
-                            42 LOAD_FAST                0 (line)
-                            44 CONTAINS_OP              0
-                            46 POP_JUMP_FORWARD_IF_TRUE    23 (to 94)
-               
-               346          48 LOAD_FAST                2 (sep)
-                            50 LOAD_FAST                1 (pattern)
-                            52 BINARY_OP                0 (+)
-                            56 LOAD_CONST               2 ('(')
-                            58 BINARY_OP                0 (+)
-                            62 LOAD_FAST                0 (line)
-                            64 CONTAINS_OP              0
-                            66 POP_JUMP_FORWARD_IF_TRUE    13 (to 94)
-               
-               347          68 LOAD_FAST                2 (sep)
-                            70 LOAD_CONST               1 (' ')
-                            72 BINARY_OP                0 (+)
-                            76 LOAD_FAST                1 (pattern)
-                            78 BINARY_OP                0 (+)
-                            82 LOAD_CONST               2 ('(')
-                            84 BINARY_OP                0 (+)
-                            88 LOAD_FAST                0 (line)
-                            90 CONTAINS_OP              0
-                            92 POP_JUMP_FORWARD_IF_FALSE   119 (to 332)
-               
-               350     >>   94 LOAD_FAST                0 (line)
-                            96 LOAD_METHOD              0 (split)
-                           118 LOAD_FAST                2 (sep)
-                           120 PRECALL                  1
-                           124 CALL                     1
-                           134 LOAD_CONST               3 (0)
-                           136 BINARY_SUBSCR
-                           146 LOAD_METHOD              1 (strip)
-                           168 PRECALL                  0
-                           172 CALL                     0
-                           182 STORE_FAST               3 (label)
-               
-               351         184 LOAD_FAST                0 (line)
-                           186 LOAD_METHOD              2 (find)
-                           208 LOAD_FAST                2 (sep)
-                           210 PRECALL                  1
-                           214 CALL                     1
-                           224 STORE_FAST               4 (index)
-               
-               352         226 LOAD_GLOBAL              7 (NULL + get_indent)
-                           238 LOAD_FAST                0 (line)
-                           240 PRECALL                  1
-                           244 CALL                     1
-                           254 LOAD_FAST                0 (line)
-                           256 LOAD_FAST                4 (index)
-                           258 LOAD_CONST               4 (1)
-                           260 BINARY_OP                0 (+)
-                           264 LOAD_CONST               0 (None)
-                           266 BUILD_SLICE              2
-                           268 BINARY_SUBSCR
-                           278 LOAD_METHOD              4 (rstrip)
-                           300 PRECALL                  0
-                           304 CALL                     0
-                           314 BINARY_OP                0 (+)
-                           318 LOAD_CONST               5 (' #LABEL :')
-                           320 BINARY_OP                0 (+)
-                           324 LOAD_FAST                3 (label)
-                           326 BINARY_OP                0 (+)
-                           330 STORE_FAST               0 (line)
+                  0000007a0000007d007c005300
+               350           0 RESUME                   0
+               
+               355           2 LOAD_FAST                1 (keyword)
+                             4 LOAD_FAST                0 (line)
+                             6 CONTAINS_OP              1
+                             8 POP_JUMP_FORWARD_IF_FALSE     2 (to 14)
+               
+               356          10 LOAD_FAST                0 (line)
+                            12 RETURN_VALUE
+               
+               358     >>   14 LOAD_FAST                0 (line)
+                            16 LOAD_METHOD              0 (lstrip)
+                            38 PRECALL                  0
+                            42 CALL                     0
+                            52 LOAD_METHOD              1 (startswith)
+                            74 LOAD_CONST               1 ('end')
+                            76 PRECALL                  1
+                            80 CALL                     1
+                            90 POP_JUMP_FORWARD_IF_FALSE    30 (to 152)
+               
+               359          92 LOAD_FAST                0 (line)
+                            94 LOAD_METHOD              2 (replace)
+                           116 LOAD_CONST               1 ('end')
+                           118 LOAD_FAST                1 (keyword)
+                           120 BINARY_OP                0 (+)
+                           124 LOAD_CONST               2 ('end ')
+                           126 LOAD_FAST                1 (keyword)
+                           128 BINARY_OP                0 (+)
+                           132 PRECALL                  2
+                           136 CALL                     2
+                           146 POP_TOP
+               
+               360         148 LOAD_FAST                0 (line)
+                           150 RETURN_VALUE
+               
+               363     >>  152 LOAD_FAST                0 (line)
+                           154 LOAD_METHOD              2 (replace)
+                           176 LOAD_CONST               3 ('(')
+                           178 LOAD_CONST               4 (' ')
+                           180 PRECALL                  2
+                           184 CALL                     2
+                           194 LOAD_METHOD              2 (replace)
+                           216 LOAD_CONST               5 (')')
+                           218 LOAD_CONST               4 (' ')
+                           220 PRECALL                  2
+                           224 CALL                     2
+                           234 LOAD_CONST               4 (' ')
+                           236 BINARY_OP                0 (+)
+                           240 STORE_FAST               2 (line_no_par)
+               
+               364         242 LOAD_FAST                2 (line_no_par)
+                           244 LOAD_METHOD              3 (find)
+                           266 LOAD_CONST               4 (' ')
+                           268 LOAD_FAST                1 (keyword)
+                           270 BINARY_OP                0 (+)
+                           274 LOAD_CONST               4 (' ')
+                           276 BINARY_OP                0 (+)
+                           280 PRECALL                  1
+                           284 CALL                     1
+                           294 STORE_FAST               3 (idx)
+               
+               365         296 LOAD_FAST                3 (idx)
+                           298 LOAD_CONST               6 (-1)
+                           300 COMPARE_OP               2 (==)
+                           306 POP_JUMP_FORWARD_IF_FALSE     2 (to 312)
+               
+               366         308 LOAD_FAST                0 (line)
+                           310 RETURN_VALUE
+               
+               368     >>  312 LOAD_GLOBAL              9 (NULL + get_indent)
+                           324 LOAD_FAST                0 (line)
+                           326 PRECALL                  1
+                           330 CALL                     1
+               
+               369         340 LOAD_FAST                0 (line)
+                           342 LOAD_FAST                3 (idx)
+                           344 LOAD_CONST               7 (1)
+                           346 BINARY_OP                0 (+)
+                           350 LOAD_CONST               8 (None)
+                           352 BUILD_SLICE              2
+                           354 BINARY_SUBSCR
+               
+               368         364 BINARY_OP                0 (+)
+               
+               370         368 LOAD_CONST               9 (' ! ')
                
-               353     >>  332 LOAD_FAST                0 (line)
-                           334 RETURN_VALUE
+               368         370 BINARY_OP                0 (+)
+               
+               370         374 LOAD_FAST                1 (keyword)
+                           376 LOAD_METHOD              5 (upper)
+                           398 PRECALL                  0
+                           402 CALL                     0
+               
+               368         412 BINARY_OP                0 (+)
+               
+               370         416 LOAD_CONST              10 ('# ')
+               
+               368         418 BINARY_OP                0 (+)
+               
+               370         422 LOAD_FAST                0 (line)
+                           424 LOAD_CONST               8 (None)
+                           426 LOAD_FAST                3 (idx)
+                           428 LOAD_CONST               7 (1)
+                           430 BINARY_OP                0 (+)
+                           434 BUILD_SLICE              2
+                           436 BINARY_SUBSCR
+                           446 LOAD_METHOD              0 (lstrip)
+                           468 PRECALL                  0
+                           472 CALL                     0
+               
+               368         482 BINARY_OP                0 (+)
+                           486 STORE_FAST               0 (line)
+               
+               371         488 LOAD_FAST                0 (line)
+                           490 RETURN_VALUE
                consts
-                  None
-                  ' '
+                  'usual cleanup before fortran structures:\n        - check ends\n        - put decorators at the back\n        '
+                  'end'
+                  'end '
                   '('
-                  0
+                  ' '
+                  ')'
+                  -1
                   1
-                  ' #LABEL :'
-               names      ('split', 'strip', 'find', 'get_indent', 'rstrip')
-               varnames   ('line', 'pattern', 'sep', 'label', 'index')
+                  None
+                  ' ! '
+                  '# '
+               names      ('lstrip', 'startswith', 'replace', 'find', 'get_indent', 'upper')
+               varnames   ('line', 'keyword', 'line_no_par', 'idx')
                freevars   ()
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
-               name       '_move_labels'
-               firstlineno 343
-               lnotab 0x020114011a0114011a035a012a016a01
-            'pure function'
-            'function_pure '
-            'elemental function'
-            'function_elemental '
-            'recursive function'
-            'function_recursive '
-            'double precision function'
-            'function '
-            'real function'
-            'integer function'
-            'logical function'
-            'selectcase'
-            'select_case '
-            'select case'
-            'select type'
-            'select_type '
-            'elemental subroutine'
-            'subroutine_elemental '
-            'recursive subroutine'
-            'subroutine_recursive '
-            'module procedure'
-            'module_procedure '
+               name       '_remove_decorators'
+               firstlineno 350
+               lnotab
+                  0x0205080104024e01380104035a0136010c0104021c0118ff040202fe04
+                  0226fe040202fe04023cfe0603
             'double precision'
             'double_precision '
+            'module procedure'
+            'module_procedure '
             'type,public,abstract'
             'type_public_abstract '
             'type,public'
             'type_public '
             'type,private,abstract'
             'type_private_abstract '
             'type,private'
             'type_private '
+            'type is'
+            'type_is '
+            'selectcase'
+            'select_case '
+            'select case'
+            'select type'
+            'select_type '
+            'function'
+            'subroutine'
             'interface'
-            'interface '
-            'abstract interface'
-            'interface_abstract '
             'enddo'
             'end do '
             'endif'
             'end if '
             'endwhere'
             'end where '
             'endmodule'
             'end module '
-            'associate('
-            'associate ('
-            'if('
-            'if ('
-            'do('
-            'do ('
-            'type('
-            'type ('
-            'type is'
-            'type_is '
+            ('function', 'subroutine', 'interface', 'if', 'do', 'type', 'associate')
+            '('
+            ' ('
             ')then'
             ') then '
-            '::'
-            ' :: '
-            '='
-            ' = '
-            'block'
-            'if'
-            'entry'
-            'select_case'
-            ('do', ':')
          names      ('str', 'replace', 'append')
-         varnames   ('lines', 'new_stmt', '_move_labels', 'line')
+         varnames   ('lines', 'new_stmt', '_remove_decorators', 'line', 'keyword')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
          name       'ftn_clean_intrinsics_declarations'
-         firstlineno 339
+         firstlineno 346
          lnotab
-            0x02020402420c0a012c012c012c022c012c012c012c032c012c012c022c
-            012c022c032c022c012c012c012c022c012c022c012c012c012c022c012c
-            012c012c012c022c022c012c021a011a011a011a011a011a022e02
+            0x0202040232160a032c012c012c012c012c012c012c012c012c012c0318
+            01180118032c012c012c012c0308093a022c022e02
       code
          argcount  : 1
-         nlocals   : 5
-         stacksize : 1
+         nlocals   : 4
+         stacksize : 4
          flags     : 3
-         code 0x970064017d0164027d0264037d0364047d047c005300
-         414           0 RESUME                   0
-         
-         422           2 LOAD_CONST               1 ('(/')
-                       4 STORE_FAST               1 (markup_left)
-         
-         423           6 LOAD_CONST               2 ('/)')
-                       8 STORE_FAST               2 (markup_right)
-         
-         424          10 LOAD_CONST               3 ('ª')
-                      12 STORE_FAST               3 (proxy_left)
-         
-         425          14 LOAD_CONST               4 ('»')
-                      16 STORE_FAST               4 (proxy_right)
+         code
+            0x9700640174000000000000000000000064027400000000000000000000
+            006604640384047d0167007d027c0044005d497d037c03a0010000000000
+            000000000000000000000000000000a6000000ab000000000000000000a0
+            0200000000000000000000000000000000000000006404a6010000ab0100
+            00000000000000720b02007c017c03a6010000ab0100000000000000007d
+            037c02a00300000000000000000000000000000000000000007c03a60100
+            00ab01000000000000000001008c4a7c025300
+         416           0 RESUME                   0
+         
+         419           2 LOAD_CONST               1 ('line')
+                       4 LOAD_GLOBAL              0 (str)
+                      16 LOAD_CONST               2 ('return')
+                      18 LOAD_GLOBAL              0 (str)
+                      30 BUILD_TUPLE              4
+                      32 LOAD_CONST               3 (<code object _clean_type, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py", line 419>)
+                      34 MAKE_FUNCTION            4 (annotations)
+                      36 STORE_FAST               1 (_clean_type)
+         
+         430          38 BUILD_LIST               0
+                      40 STORE_FAST               2 (new_stmt)
+         
+         431          42 LOAD_FAST                0 (lines)
+                      44 GET_ITER
+                 >>   46 FOR_ITER                73 (to 194)
+                      48 STORE_FAST               3 (line)
+         
+         432          50 LOAD_FAST                3 (line)
+                      52 LOAD_METHOD              1 (lstrip)
+                      74 PRECALL                  0
+                      78 CALL                     0
+                      88 LOAD_METHOD              2 (startswith)
+                     110 LOAD_CONST               4 ('type')
+                     112 PRECALL                  1
+                     116 CALL                     1
+                     126 POP_JUMP_FORWARD_IF_FALSE    11 (to 150)
+         
+         433         128 PUSH_NULL
+                     130 LOAD_FAST                1 (_clean_type)
+                     132 LOAD_FAST                3 (line)
+                     134 PRECALL                  1
+                     138 CALL                     1
+                     148 STORE_FAST               3 (line)
+         
+         435     >>  150 LOAD_FAST                2 (new_stmt)
+                     152 LOAD_METHOD              3 (append)
+                     174 LOAD_FAST                3 (line)
+                     176 PRECALL                  1
+                     180 CALL                     1
+                     190 POP_TOP
+                     192 JUMP_BACKWARD           74 (to 46)
          
-         452          18 LOAD_FAST                0 (lines)
-                      20 RETURN_VALUE
+         436     >>  194 LOAD_FAST                2 (new_stmt)
+                     196 RETURN_VALUE
          consts
-            "Fix end parenthesis of multilines\n    eg in tranfit.f:\n       20 FORMAT (/,' DATA HAS BEEN FIT OVER THE RANGE:  TLOW=',F9.2,\n     1        ', THIGH=',F9.2)\n    last ) should be a /)\n    "
-            '(/'
-            '/)'
-            'ª'
-            '»'
-         names      ()
-         varnames   ('lines', 'markup_left', 'markup_right', 'proxy_left', 'proxy_right')
+            ' Replace  type( declarations by _type('
+            'line'
+            'return'
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 5
+               flags     : 19
+               code
+                  0x97007c00a0000000000000000000000000000000000000000000640164
+                  02a6020000ab02000000000000000064031900000000000000000064046b
+                  020000000072177c00a00000000000000000000000000000000000000000
+                  00640564066407a6030000ab03000000000000000053007c00a000000000
+                  000000000000000000000000000000000064016402a6020000ab02000000
+                  00000000006403640885021900000000000000000064096b020000000072
+                  177c00a0000000000000000000000000000000000000000000640a640b64
+                  07a6030000ab03000000000000000053007c00a000000000000000000000
+                  000000000000000000000064016402a6020000ab02000000000000000064
+                  0319000000000000000000640c760072027c0053007c00a0000000000000
+                  00000000000000000000000000000064016402a6020000ab020000000000
+                  000000640319000000000000000000640d6b020000000072177c00a00000
+                  000000000000000000000000000000000000006405640e6407a6030000ab
+                  03000000000000000053007c005300
+               419           0 RESUME                   0
+               
+               420           2 LOAD_FAST                0 (line)
+                             4 LOAD_METHOD              0 (replace)
+                            26 LOAD_CONST               1 (' ')
+                            28 LOAD_CONST               2 ('')
+                            30 PRECALL                  2
+                            34 CALL                     2
+                            44 LOAD_CONST               3 (4)
+                            46 BINARY_SUBSCR
+                            56 LOAD_CONST               4 ('(')
+                            58 COMPARE_OP               2 (==)
+                            64 POP_JUMP_FORWARD_IF_FALSE    23 (to 112)
+               
+               421          66 LOAD_FAST                0 (line)
+                            68 LOAD_METHOD              0 (replace)
+                            90 LOAD_CONST               5 ('type')
+                            92 LOAD_CONST               6 ('_type')
+                            94 LOAD_CONST               7 (1)
+                            96 PRECALL                  3
+                           100 CALL                     3
+                           110 RETURN_VALUE
+               
+               422     >>  112 LOAD_FAST                0 (line)
+                           114 LOAD_METHOD              0 (replace)
+                           136 LOAD_CONST               1 (' ')
+                           138 LOAD_CONST               2 ('')
+                           140 PRECALL                  2
+                           144 CALL                     2
+                           154 LOAD_CONST               3 (4)
+                           156 LOAD_CONST               8 (6)
+                           158 BUILD_SLICE              2
+                           160 BINARY_SUBSCR
+                           170 LOAD_CONST               9 ('is')
+                           172 COMPARE_OP               2 (==)
+                           178 POP_JUMP_FORWARD_IF_FALSE    23 (to 226)
+               
+               423         180 LOAD_FAST                0 (line)
+                           182 LOAD_METHOD              0 (replace)
+                           204 LOAD_CONST              10 ('type is')
+                           206 LOAD_CONST              11 ('#typeis')
+                           208 LOAD_CONST               7 (1)
+                           210 PRECALL                  3
+                           214 CALL                     3
+                           224 RETURN_VALUE
+               
+               424     >>  226 LOAD_FAST                0 (line)
+                           228 LOAD_METHOD              0 (replace)
+                           250 LOAD_CONST               1 (' ')
+                           252 LOAD_CONST               2 ('')
+                           254 PRECALL                  2
+                           258 CALL                     2
+                           268 LOAD_CONST               3 (4)
+                           270 BINARY_SUBSCR
+                           280 LOAD_CONST              12 (' azertyuiopqsdfghjklmwxcvbn')
+                           282 CONTAINS_OP              0
+                           284 POP_JUMP_FORWARD_IF_FALSE     2 (to 290)
+               
+               425         286 LOAD_FAST                0 (line)
+                           288 RETURN_VALUE
+               
+               426     >>  290 LOAD_FAST                0 (line)
+                           292 LOAD_METHOD              0 (replace)
+                           314 LOAD_CONST               1 (' ')
+                           316 LOAD_CONST               2 ('')
+                           318 PRECALL                  2
+                           322 CALL                     2
+                           332 LOAD_CONST               3 (4)
+                           334 BINARY_SUBSCR
+                           344 LOAD_CONST              13 (',')
+                           346 COMPARE_OP               2 (==)
+                           352 POP_JUMP_FORWARD_IF_FALSE    23 (to 400)
+               
+               427         354 LOAD_FAST                0 (line)
+                           356 LOAD_METHOD              0 (replace)
+                           378 LOAD_CONST               5 ('type')
+                           380 LOAD_CONST              14 ('type ')
+                           382 LOAD_CONST               7 (1)
+                           384 PRECALL                  3
+                           388 CALL                     3
+                           398 RETURN_VALUE
+               
+               429     >>  400 LOAD_FAST                0 (line)
+                           402 RETURN_VALUE
+               consts
+                  None
+                  ' '
+                  ''
+                  4
+                  '('
+                  'type'
+                  '_type'
+                  1
+                  6
+                  'is'
+                  'type is'
+                  '#typeis'
+                  ' azertyuiopqsdfghjklmwxcvbn'
+                  ','
+                  'type '
+               names      ('replace',)
+               varnames   ('line',)
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
+               name       '_clean_type'
+               firstlineno 419
+               lnotab 0x020140012e0144012e013c01040140012e02
+            'type'
+         names      ('str', 'lstrip', 'startswith', 'append')
+         varnames   ('lines', '_clean_type', 'new_stmt', 'line')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
-         name       'ftn_old_fix_end_multiline'
-         firstlineno 414
-         lnotab 0x0208040104010401041b
+         name       'ftn_clean_type_keywords'
+         firstlineno 416
+         lnotab 0x0203240b040108014e0116022c01
       'code'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 5
          flags     : 3
          code
@@ -2615,206 +2738,215 @@
             0200000000000000007c015f030000000000000000740900000000000000
             0000007c016a0300000000000000006405a6020000ab0200000000000000
             007c015f030000000000000000740b000000000000000000007c016406a6
             020000ab0200000000000000007d01740d000000000000000000007c01a6
             010000ab0100000000000000007d01740f000000000000000000007c01a6
             010000ab0100000000000000007d017411000000000000000000007c01a6
             010000ab0100000000000000007d017413000000000000000000007c01a6
-            010000ab0100000000000000007d017415000000000000000000007c016a
-            030000000000000000a6010000ab0100000000000000007c015f03000000
-            00000000007417000000000000000000007c0164076408a6030000ab0300
-            000000000000007d017419000000000000000000007c01a6010000ab0100
+            010000ab0100000000000000007d017415000000000000000000007c0164
+            076408a6030000ab0300000000000000007d017417000000000000000000
+            007c016a030000000000000000a6010000ab0100000000000000007c015f
+            0300000000000000007419000000000000000000007c01a6010000ab0100
             000000000000007d01741b000000000000000000007c016a030000000000
             000000a6010000ab0100000000000000007c015f03000000000000000074
-            1d000000000000000000007c01a6010000ab0100000000000000007d0174
-            1f000000000000000000007c016a030000000000000000a6010000ab0100
-            000000000000007c015f0300000000000000007421000000000000000000
+            1d000000000000000000007c016a030000000000000000a6010000ab0100
+            000000000000007c015f030000000000000000741f000000000000000000
+            007c01a6010000ab0100000000000000007d017421000000000000000000
             007c016a030000000000000000a6010000ab0100000000000000007c015f
-            0300000000000000007423000000000000000000007c01a6010000ab0100
-            000000000000007d017425000000000000000000007c016a030000000000
-            000000a6010000ab0100000000000000007c015f0300000000000000007c
-            015300
-         455           0 RESUME                   0
+            0300000000000000007423000000000000000000007c016a030000000000
+            000000a6010000ab0100000000000000007c015f03000000000000000074
+            25000000000000000000007c01a6010000ab0100000000000000007d0174
+            27000000000000000000007c016a030000000000000000a6010000ab0100
+            000000000000007c015f0300000000000000007c015300
+         439           0 RESUME                   0
          
-         465           2 LOAD_GLOBAL              1 (NULL + new_stmts)
+         449           2 LOAD_GLOBAL              1 (NULL + new_stmts)
                       14 LOAD_FAST                0 (code)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               1 (stmts)
          
-         467          32 LOAD_GLOBAL              3 (NULL + clean_pure_comments)
+         451          32 LOAD_GLOBAL              3 (NULL + clean_pure_comments)
                       44 LOAD_FAST                1 (stmts)
                       46 LOAD_CONST               1 ('c')
                       48 PRECALL                  2
                       52 CALL                     2
                       62 STORE_FAST               1 (stmts)
          
-         468          64 LOAD_GLOBAL              3 (NULL + clean_pure_comments)
+         452          64 LOAD_GLOBAL              3 (NULL + clean_pure_comments)
                       76 LOAD_FAST                1 (stmts)
                       78 LOAD_CONST               2 ('C')
                       80 PRECALL                  2
                       84 CALL                     2
                       94 STORE_FAST               1 (stmts)
          
-         469          96 LOAD_GLOBAL              3 (NULL + clean_pure_comments)
+         453          96 LOAD_GLOBAL              3 (NULL + clean_pure_comments)
                      108 LOAD_FAST                1 (stmts)
                      110 LOAD_CONST               3 ('*')
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_FAST               1 (stmts)
          
-         471         128 LOAD_GLOBAL              5 (NULL + eat_spaces)
+         455         128 LOAD_GLOBAL              5 (NULL + eat_spaces)
                      140 LOAD_FAST                1 (stmts)
                      142 LOAD_ATTR                3 (stmt)
                      152 PRECALL                  1
                      156 CALL                     1
                      166 LOAD_FAST                1 (stmts)
                      168 STORE_ATTR               3 (stmt)
          
-         472         178 LOAD_GLOBAL              9 (NULL + remove_strings)
+         456         178 LOAD_GLOBAL              9 (NULL + remove_strings)
                      190 LOAD_FAST                1 (stmts)
                      192 LOAD_ATTR                3 (stmt)
                      202 LOAD_CONST               4 ('"')
                      204 PRECALL                  2
                      208 CALL                     2
                      218 LOAD_FAST                1 (stmts)
                      220 STORE_ATTR               3 (stmt)
          
-         473         230 LOAD_GLOBAL              9 (NULL + remove_strings)
+         457         230 LOAD_GLOBAL              9 (NULL + remove_strings)
                      242 LOAD_FAST                1 (stmts)
                      244 LOAD_ATTR                3 (stmt)
                      254 LOAD_CONST               5 ("'")
                      256 PRECALL                  2
                      260 CALL                     2
                      270 LOAD_FAST                1 (stmts)
                      272 STORE_ATTR               3 (stmt)
          
-         475         282 LOAD_GLOBAL             11 (NULL + clean_inline_comments)
+         459         282 LOAD_GLOBAL             11 (NULL + clean_inline_comments)
                      294 LOAD_FAST                1 (stmts)
                      296 LOAD_CONST               6 ('!')
                      298 PRECALL                  2
                      302 CALL                     2
                      312 STORE_FAST               1 (stmts)
          
-         477         314 LOAD_GLOBAL             13 (NULL + clean_blanks)
+         461         314 LOAD_GLOBAL             13 (NULL + clean_blanks)
                      326 LOAD_FAST                1 (stmts)
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               1 (stmts)
          
-         478         344 LOAD_GLOBAL             15 (NULL + align_end_continuations)
+         462         344 LOAD_GLOBAL             15 (NULL + align_end_continuations)
                      356 LOAD_FAST                1 (stmts)
                      358 PRECALL                  1
                      362 CALL                     1
                      372 STORE_FAST               1 (stmts)
          
-         479         374 LOAD_GLOBAL             17 (NULL + align_start_continuations)
+         463         374 LOAD_GLOBAL             17 (NULL + align_start_continuations)
                      386 LOAD_FAST                1 (stmts)
                      388 PRECALL                  1
                      392 CALL                     1
                      402 STORE_FAST               1 (stmts)
          
-         480         404 LOAD_GLOBAL             19 (NULL + ftn_align_labelled_continuations)
+         464         404 LOAD_GLOBAL             19 (NULL + ftn_align_labelled_continuations)
                      416 LOAD_FAST                1 (stmts)
                      418 PRECALL                  1
                      422 CALL                     1
                      432 STORE_FAST               1 (stmts)
          
-         482         434 LOAD_GLOBAL             21 (NULL + ftn_old_fix_end_multiline)
+         465         434 LOAD_GLOBAL             21 (NULL + align_multiline_blocks)
                      446 LOAD_FAST                1 (stmts)
-                     448 LOAD_ATTR                3 (stmt)
-                     458 PRECALL                  1
-                     462 CALL                     1
-                     472 LOAD_FAST                1 (stmts)
-                     474 STORE_ATTR               3 (stmt)
-         
-         483         484 LOAD_GLOBAL             23 (NULL + align_multiline_blocks)
-                     496 LOAD_FAST                1 (stmts)
-                     498 LOAD_CONST               7 ('(/')
-                     500 LOAD_CONST               8 ('/)')
-                     502 PRECALL                  3
-                     506 CALL                     3
-                     516 STORE_FAST               1 (stmts)
+                     448 LOAD_CONST               7 ('(/')
+                     450 LOAD_CONST               8 ('/)')
+                     452 PRECALL                  3
+                     456 CALL                     3
+                     466 STORE_FAST               1 (stmts)
+         
+         467         468 LOAD_GLOBAL             23 (NULL + ftn_clean_operators)
+                     480 LOAD_FAST                1 (stmts)
+                     482 LOAD_ATTR                3 (stmt)
+                     492 PRECALL                  1
+                     496 CALL                     1
+                     506 LOAD_FAST                1 (stmts)
+                     508 STORE_ATTR               3 (stmt)
          
-         484         518 LOAD_GLOBAL             25 (NULL + split_multi_statement_lines)
+         468         518 LOAD_GLOBAL             25 (NULL + split_multi_statement_lines)
                      530 LOAD_FAST                1 (stmts)
                      532 PRECALL                  1
                      536 CALL                     1
                      546 STORE_FAST               1 (stmts)
          
-         486         548 LOAD_GLOBAL             27 (NULL + ftn_clean_intrinsics_declarations)
+         471         548 LOAD_GLOBAL             27 (NULL + ftn_clean_type_keywords)
                      560 LOAD_FAST                1 (stmts)
                      562 LOAD_ATTR                3 (stmt)
                      572 PRECALL                  1
                      576 CALL                     1
                      586 LOAD_FAST                1 (stmts)
                      588 STORE_ATTR               3 (stmt)
          
-         487         598 LOAD_GLOBAL             29 (NULL + ftn_clean_labelled_loops_oldftn)
+         472         598 LOAD_GLOBAL             29 (NULL + ftn_clean_intrinsics_declarations)
                      610 LOAD_FAST                1 (stmts)
-                     612 PRECALL                  1
-                     616 CALL                     1
-                     626 STORE_FAST               1 (stmts)
-         
-         488         628 LOAD_GLOBAL             31 (NULL + ftn_clean_labelled_loops_newftn)
-                     640 LOAD_FAST                1 (stmts)
-                     642 LOAD_ATTR                3 (stmt)
-                     652 PRECALL                  1
-                     656 CALL                     1
-                     666 LOAD_FAST                1 (stmts)
-                     668 STORE_ATTR               3 (stmt)
+                     612 LOAD_ATTR                3 (stmt)
+                     622 PRECALL                  1
+                     626 CALL                     1
+                     636 LOAD_FAST                1 (stmts)
+                     638 STORE_ATTR               3 (stmt)
+         
+         473         648 LOAD_GLOBAL             31 (NULL + ftn_clean_labelled_loops_oldftn)
+                     660 LOAD_FAST                1 (stmts)
+                     662 PRECALL                  1
+                     666 CALL                     1
+                     676 STORE_FAST               1 (stmts)
          
-         490         678 LOAD_GLOBAL             33 (NULL + ftn_suppress_goto_references)
+         474         678 LOAD_GLOBAL             33 (NULL + ftn_clean_labelled_loops_newftn)
                      690 LOAD_FAST                1 (stmts)
                      692 LOAD_ATTR                3 (stmt)
                      702 PRECALL                  1
                      706 CALL                     1
                      716 LOAD_FAST                1 (stmts)
                      718 STORE_ATTR               3 (stmt)
          
-         491         728 LOAD_GLOBAL             35 (NULL + ftn_make_oneliners_conditionals_multilines)
+         476         728 LOAD_GLOBAL             35 (NULL + ftn_suppress_goto_references)
                      740 LOAD_FAST                1 (stmts)
-                     742 PRECALL                  1
-                     746 CALL                     1
-                     756 STORE_FAST               1 (stmts)
-         
-         492         758 LOAD_GLOBAL             37 (NULL + ftn_remove_space_in_front_of_variables)
-                     770 LOAD_FAST                1 (stmts)
-                     772 LOAD_ATTR                3 (stmt)
-                     782 PRECALL                  1
-                     786 CALL                     1
-                     796 LOAD_FAST                1 (stmts)
-                     798 STORE_ATTR               3 (stmt)
+                     742 LOAD_ATTR                3 (stmt)
+                     752 PRECALL                  1
+                     756 CALL                     1
+                     766 LOAD_FAST                1 (stmts)
+                     768 STORE_ATTR               3 (stmt)
+         
+         477         778 LOAD_GLOBAL             37 (NULL + ftn_make_oneliners_conditionals_multilines)
+                     790 LOAD_FAST                1 (stmts)
+                     792 PRECALL                  1
+                     796 CALL                     1
+                     806 STORE_FAST               1 (stmts)
+         
+         478         808 LOAD_GLOBAL             39 (NULL + ftn_remove_space_in_front_of_variables)
+                     820 LOAD_FAST                1 (stmts)
+                     822 LOAD_ATTR                3 (stmt)
+                     832 PRECALL                  1
+                     836 CALL                     1
+                     846 LOAD_FAST                1 (stmts)
+                     848 STORE_ATTR               3 (stmt)
          
-         494         808 LOAD_FAST                1 (stmts)
-                     810 RETURN_VALUE
+         480         858 LOAD_FAST                1 (stmts)
+                     860 RETURN_VALUE
          consts
             "\n    Unformat Fortran code by stripping comments and moving leading '&' characters.\n\n    Args:\n        code (List[str]): List of Fortran code lines.\n\n    Returns:\n        List[Tuple[str, Tuple[int, int]]]: List of unformatted code statements along with line number ranges.\n    "
             'c'
             'C'
             '*'
             '"'
             "'"
             '!'
             '(/'
             '/)'
-         names      ('new_stmts', 'clean_pure_comments', 'eat_spaces', 'stmt', 'remove_strings', 'clean_inline_comments', 'clean_blanks', 'align_end_continuations', 'align_start_continuations', 'ftn_align_labelled_continuations', 'ftn_old_fix_end_multiline', 'align_multiline_blocks', 'split_multi_statement_lines', 'ftn_clean_intrinsics_declarations', 'ftn_clean_labelled_loops_oldftn', 'ftn_clean_labelled_loops_newftn', 'ftn_suppress_goto_references', 'ftn_make_oneliners_conditionals_multilines', 'ftn_remove_space_in_front_of_variables')
+         names      ('new_stmts', 'clean_pure_comments', 'eat_spaces', 'stmt', 'remove_strings', 'clean_inline_comments', 'clean_blanks', 'align_end_continuations', 'align_start_continuations', 'ftn_align_labelled_continuations', 'align_multiline_blocks', 'ftn_clean_operators', 'split_multi_statement_lines', 'ftn_clean_type_keywords', 'ftn_clean_intrinsics_declarations', 'ftn_clean_labelled_loops_oldftn', 'ftn_clean_labelled_loops_newftn', 'ftn_suppress_goto_references', 'ftn_make_oneliners_conditionals_multilines', 'ftn_remove_space_in_front_of_variables')
          varnames   ('code', 'stmts')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
          name       'unformat_ftn'
-         firstlineno 455
+         firstlineno 439
          lnotab
-            0x020a1e0220012001200232013401340220021e011e011e011e02320122
-            011e0232011e01320232011e013202
+            0x020a1e0220012001200232013401340220021e011e011e011e01220232
+            011e03320132011e01320232011e013202
       None
-   names      ('typing', 'List', 'loguru', 'logger', 'tucan.kw_lang', 'KEYWORDS_FTN', 'tucan.unformat_common', 'Statements', 'new_stmts', 'remove_strings', 'clean_blanks', 'clean_inline_comments', 'clean_pure_comments', 'align_multiline_blocks', 'split_multi_statement_lines', 'get_indent', 'eat_spaces', 'align_end_continuations', 'align_start_continuations', 'ftn_align_labelled_continuations', 'ftn_make_oneliners_conditionals_multilines', 'str', 'list', 'split_oneliner', 'ftn_remove_space_in_front_of_variables', 'ftn_clean_labelled_loops_oldftn', 'ftn_suppress_goto_references', 'ftn_clean_labelled_loops_newftn', 'ftn_clean_intrinsics_declarations', 'ftn_old_fix_end_multiline', 'unformat_ftn')
+   names      ('typing', 'List', 'loguru', 'logger', 'tucan.kw_lang', 'KEYWORDS_FTN', 'tucan.unformat_common', 'Statements', 'new_stmts', 'remove_strings', 'clean_blanks', 'clean_inline_comments', 'clean_pure_comments', 'align_multiline_blocks', 'split_multi_statement_lines', 'get_indent', 'eat_spaces', 'align_end_continuations', 'align_start_continuations', 'ftn_align_labelled_continuations', 'ftn_make_oneliners_conditionals_multilines', 'str', 'list', 'split_oneliner', 'ftn_remove_space_in_front_of_variables', 'ftn_clean_labelled_loops_oldftn', 'ftn_suppress_goto_references', 'ftn_clean_labelled_loops_newftn', 'ftn_clean_operators', 'ftn_clean_intrinsics_declarations', 'ftn_clean_type_keywords', 'unformat_ftn')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_ftn.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c010c02300d1018101b1025103d101f2820103e280f28
-      20284b2829
+      0x00ff02010c010c010c02300d1018101e101a1035101f2820103e280f28
+      29280e28462817
```

### Comparing `tucan-0.1.0/src/tucan/__pycache__/unformat_main.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/unformat_main.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,19 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0xe6c89465 (Wed Jan  3 02:39:34 2024 UTC)
-files sz: 1184
+moddate:  0xa5114266 (Mon May 13 13:12:05 2024 UTC)
+files sz: 1398
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 4
+   stacksize : 7
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a0401
-      00640164046c056d065a060100640164056c076d085a0801006406650964
-      07650a6604640884045a0b64095300
+      00640164046c056d065a060100640164056c076d085a080100640164066c
+      096d0a5a0a0100640d6408650b6409650c640a650d6606640b84055a0e64
+      0c5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('Global function to handle the unformat of various languages')
                  4 STORE_NAME               0 (__doc__)
    
      2           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('logger',))
@@ -39,85 +40,101 @@
      6          42 LOAD_CONST               1 (0)
                 44 LOAD_CONST               5 (('unformat_c',))
                 46 IMPORT_NAME              7 (tucan.unformat_c)
                 48 IMPORT_FROM              8 (unformat_c)
                 50 STORE_NAME               8 (unformat_c)
                 52 POP_TOP
    
-     9          54 LOAD_CONST               6 ('filename')
-                56 LOAD_NAME                9 (str)
-                58 LOAD_CONST               7 ('return')
-                60 LOAD_NAME               10 (list)
-                62 BUILD_TUPLE              4
-                64 LOAD_CONST               8 (<code object unformat_main, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_main.py", line 9>)
-                66 MAKE_FUNCTION            4 (annotations)
-                68 STORE_NAME              11 (unformat_main)
-                70 LOAD_CONST               9 (None)
-                72 RETURN_VALUE
+     7          54 LOAD_CONST               1 (0)
+                56 LOAD_CONST               6 (('remove_ifdef_from_module',))
+                58 IMPORT_NAME              9 (tucan.clean_ifdef)
+                60 IMPORT_FROM             10 (remove_ifdef_from_module)
+                62 STORE_NAME              10 (remove_ifdef_from_module)
+                64 POP_TOP
+   
+    10          66 LOAD_CONST              13 ((False,))
+                68 LOAD_CONST               8 ('filename')
+                70 LOAD_NAME               11 (str)
+                72 LOAD_CONST               9 ('verbose')
+                74 LOAD_NAME               12 (bool)
+                76 LOAD_CONST              10 ('return')
+                78 LOAD_NAME               13 (list)
+                80 BUILD_TUPLE              6
+                82 LOAD_CONST              11 (<code object unformat_main, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_main.py", line 10>)
+                84 MAKE_FUNCTION            5 (defaults, annotations)
+                86 STORE_NAME              14 (unformat_main)
+                88 LOAD_CONST              12 (None)
+                90 RETURN_VALUE
    consts
       'Global function to handle the unformat of various languages'
       0
       ('logger',)
       ('unformat_py',)
       ('unformat_ftn',)
       ('unformat_c',)
+      ('remove_ifdef_from_module',)
+      False
       'filename'
+      'verbose'
       'return'
       code
-         argcount  : 1
-         nlocals   : 5
+         argcount  : 2
+         nlocals   : 6
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c006401a6020000ab020000000000
-            00000035007d017c01a00100000000000000000000000000000000000000
+            00000035007d027c02a00100000000000000000000000000000000000000
             00a6000000ab000000000000000000a00200000000000000000000000000
-            00000000000000a6000000ab0000000000000000007d02640264026402a6
+            00000000000000a6000000ab0000000000000000007d03640264026402a6
             020000ab02000000000000000001006e0b23003100730477027803590077
-            010100590001000100640384007c024400a6000000ab0000000000000000
-            007d027c00a0030000000000000000000000000000000000000000a60000
+            010100590001000100640384007c034400a6000000ab0000000000000000
+            007d037c00a0030000000000000000000000000000000000000000a60000
             00ab000000000000000000a0040000000000000000000000000000000000
-            0000006404a6010000ab0100000000000000007224740b00000000000000
+            0000006404a6010000ab0100000000000000007225740b00000000000000
             0000006a0600000000000000006405a6010000ab01000000000000000001
-            00740f000000000000000000007c02a6010000ab0100000000000000007d
-            036edd7c00a0030000000000000000000000000000000000000000a60000
-            00ab000000000000000000a0040000000000000000000000000000000000
-            0000006406a6010000ab0100000000000000007224740b00000000000000
-            0000006a0600000000000000006407a6010000ab01000000000000000001
-            007411000000000000000000007c02a6010000ab0100000000000000007d
-            036e927c00a0030000000000000000000000000000000000000000a60000
-            00ab000000000000000000a0040000000000000000000000000000000000
-            0000006408a6010000ab0100000000000000007224740b00000000000000
-            0000006a0600000000000000006409a6010000ab01000000000000000001
-            007413000000000000000000007c02a6010000ab0100000000000000007d
-            036e477c00a0030000000000000000000000000000000000000000a60000
-            00ab000000000000000000a00a0000000000000000000000000000000000
-            000000640aa6010000ab010000000000000000640b190000000000000000
-            007d04740b000000000000000000006a0b0000000000000000640c7c049b
-            00640d9d03a6010000ab010000000000000000010067007d037c035300
-           9           0 RESUME                   0
+            00740f000000000000000000007c03a6010000ab0100000000000000007d
+            0490016e017c00a0030000000000000000000000000000000000000000a6
+            000000ab000000000000000000a004000000000000000000000000000000
+            00000000006406a6010000ab0100000000000000007237740b0000000000
+            00000000006a0600000000000000006407a6010000ab0100000000000000
+            0001007411000000000000000000007c0367007c016408ac09a6040000ab
+            0400000000000000007d037413000000000000000000007c03a6010000ab
+            0100000000000000007d046ea37c00a00300000000000000000000000000
+            00000000000000a6000000ab000000000000000000a00400000000000000
+            00000000000000000000000000640aa6010000ab01000000000000000072
+            35740b000000000000000000006a060000000000000000640ba6010000ab
+            01000000000000000001007411000000000000000000007c0367007c01a6
+            030000ab0300000000000000007d037415000000000000000000007c03a6
+            010000ab0100000000000000007d046e477c00a003000000000000000000
+            0000000000000000000000a6000000ab000000000000000000a00b000000
+            0000000000000000000000000000000000640ca6010000ab010000000000
+            000000640d190000000000000000007d05740b000000000000000000006a
+            0c0000000000000000640e7c059b00640f9d03a6010000ab010000000000
+            000000010067007d047c045300
+          10           0 RESUME                   0
          
-          19           2 LOAD_GLOBAL              1 (NULL + open)
+          20           2 LOAD_GLOBAL              1 (NULL + open)
                       14 LOAD_FAST                0 (filename)
                       16 LOAD_CONST               1 ('r')
                       18 PRECALL                  2
                       22 CALL                     2
                       32 BEFORE_WITH
-                      34 STORE_FAST               1 (fin)
+                      34 STORE_FAST               2 (fin)
          
-          20          36 LOAD_FAST                1 (fin)
+          21          36 LOAD_FAST                2 (fin)
                       38 LOAD_METHOD              1 (read)
                       60 PRECALL                  0
                       64 CALL                     0
                       74 LOAD_METHOD              2 (splitlines)
                       96 PRECALL                  0
                      100 CALL                     0
-                     110 STORE_FAST               2 (code)
+                     110 STORE_FAST               3 (code)
          
-          19         112 LOAD_CONST               2 (None)
+          20         112 LOAD_CONST               2 (None)
                      114 LOAD_CONST               2 (None)
                      116 LOAD_CONST               2 (None)
                      118 PRECALL                  2
                      122 CALL                     2
                      132 POP_TOP
                      134 JUMP_FORWARD            11 (to 158)
                  >>  136 PUSH_EXC_INFO
@@ -128,122 +145,141 @@
                      146 POP_EXCEPT
                      148 RERAISE                  1
                  >>  150 POP_TOP
                      152 POP_EXCEPT
                      154 POP_TOP
                      156 POP_TOP
          
-          22     >>  158 LOAD_CONST               3 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_main.py", line 22>)
+          23     >>  158 LOAD_CONST               3 (<code object <listcomp>, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_main.py", line 23>)
                      160 MAKE_FUNCTION            0
-                     162 LOAD_FAST                2 (code)
+                     162 LOAD_FAST                3 (code)
                      164 GET_ITER
                      166 PRECALL                  0
                      170 CALL                     0
-                     180 STORE_FAST               2 (code)
+                     180 STORE_FAST               3 (code)
          
-          24         182 LOAD_FAST                0 (filename)
+          25         182 LOAD_FAST                0 (filename)
                      184 LOAD_METHOD              3 (lower)
                      206 PRECALL                  0
                      210 CALL                     0
                      220 LOAD_METHOD              4 (endswith)
                      242 LOAD_CONST               4 ('.py')
                      244 PRECALL                  1
                      248 CALL                     1
-                     258 POP_JUMP_FORWARD_IF_FALSE    36 (to 332)
+                     258 POP_JUMP_FORWARD_IF_FALSE    37 (to 334)
          
-          25         260 LOAD_GLOBAL             11 (NULL + logger)
+          26         260 LOAD_GLOBAL             11 (NULL + logger)
                      272 LOAD_ATTR                6 (debug)
                      282 LOAD_CONST               5 ('Python code detected ...')
                      284 PRECALL                  1
                      288 CALL                     1
                      298 POP_TOP
          
-          26         300 LOAD_GLOBAL             15 (NULL + unformat_py)
-                     312 LOAD_FAST                2 (code)
+          27         300 LOAD_GLOBAL             15 (NULL + unformat_py)
+                     312 LOAD_FAST                3 (code)
                      314 PRECALL                  1
                      318 CALL                     1
-                     328 STORE_FAST               3 (statements)
-                     330 JUMP_FORWARD           221 (to 774)
-         
-          27     >>  332 LOAD_FAST                0 (filename)
-                     334 LOAD_METHOD              3 (lower)
-                     356 PRECALL                  0
-                     360 CALL                     0
-                     370 LOAD_METHOD              4 (endswith)
-                     392 LOAD_CONST               6 (('.f', '.F', '.f77', '.f90'))
-                     394 PRECALL                  1
-                     398 CALL                     1
-                     408 POP_JUMP_FORWARD_IF_FALSE    36 (to 482)
-         
-          28         410 LOAD_GLOBAL             11 (NULL + logger)
-                     422 LOAD_ATTR                6 (debug)
-                     432 LOAD_CONST               7 ('Fortran code detected ...')
-                     434 PRECALL                  1
-                     438 CALL                     1
-                     448 POP_TOP
-         
-          29         450 LOAD_GLOBAL             17 (NULL + unformat_ftn)
-                     462 LOAD_FAST                2 (code)
-                     464 PRECALL                  1
-                     468 CALL                     1
-                     478 STORE_FAST               3 (statements)
-                     480 JUMP_FORWARD           146 (to 774)
-         
-          30     >>  482 LOAD_FAST                0 (filename)
-                     484 LOAD_METHOD              3 (lower)
-                     506 PRECALL                  0
-                     510 CALL                     0
-                     520 LOAD_METHOD              4 (endswith)
-                     542 LOAD_CONST               8 (('.c', '.cpp', '.cc'))
-                     544 PRECALL                  1
-                     548 CALL                     1
-                     558 POP_JUMP_FORWARD_IF_FALSE    36 (to 632)
-         
-          31         560 LOAD_GLOBAL             11 (NULL + logger)
-                     572 LOAD_ATTR                6 (debug)
-                     582 LOAD_CONST               9 ('C/C++ code detected ...')
+                     328 STORE_FAST               4 (statements)
+                     330 EXTENDED_ARG             1
+                     332 JUMP_FORWARD           257 (to 848)
+         
+          28     >>  334 LOAD_FAST                0 (filename)
+                     336 LOAD_METHOD              3 (lower)
+                     358 PRECALL                  0
+                     362 CALL                     0
+                     372 LOAD_METHOD              4 (endswith)
+                     394 LOAD_CONST               6 (('.f', '.F', '.f77', '.f90'))
+                     396 PRECALL                  1
+                     400 CALL                     1
+                     410 POP_JUMP_FORWARD_IF_FALSE    55 (to 522)
+         
+          29         412 LOAD_GLOBAL             11 (NULL + logger)
+                     424 LOAD_ATTR                6 (debug)
+                     434 LOAD_CONST               7 ('Fortran code detected ...')
+                     436 PRECALL                  1
+                     440 CALL                     1
+                     450 POP_TOP
+         
+          30         452 LOAD_GLOBAL             17 (NULL + remove_ifdef_from_module)
+                     464 LOAD_FAST                3 (code)
+                     466 BUILD_LIST               0
+                     468 LOAD_FAST                1 (verbose)
+                     470 LOAD_CONST               8 (True)
+                     472 KW_NAMES                 9
+                     474 PRECALL                  4
+                     478 CALL                     4
+                     488 STORE_FAST               3 (code)
+         
+          31         490 LOAD_GLOBAL             19 (NULL + unformat_ftn)
+                     502 LOAD_FAST                3 (code)
+                     504 PRECALL                  1
+                     508 CALL                     1
+                     518 STORE_FAST               4 (statements)
+                     520 JUMP_FORWARD           163 (to 848)
+         
+          32     >>  522 LOAD_FAST                0 (filename)
+                     524 LOAD_METHOD              3 (lower)
+                     546 PRECALL                  0
+                     550 CALL                     0
+                     560 LOAD_METHOD              4 (endswith)
+                     582 LOAD_CONST              10 (('.c', '.cpp', '.cc', '.h'))
                      584 PRECALL                  1
                      588 CALL                     1
-                     598 POP_TOP
+                     598 POP_JUMP_FORWARD_IF_FALSE    53 (to 706)
          
-          32         600 LOAD_GLOBAL             19 (NULL + unformat_c)
-                     612 LOAD_FAST                2 (code)
-                     614 PRECALL                  1
-                     618 CALL                     1
-                     628 STORE_FAST               3 (statements)
-                     630 JUMP_FORWARD            71 (to 774)
-         
-          34     >>  632 LOAD_FAST                0 (filename)
-                     634 LOAD_METHOD              3 (lower)
-                     656 PRECALL                  0
-                     660 CALL                     0
-                     670 LOAD_METHOD             10 (split)
-                     692 LOAD_CONST              10 ('.')
-                     694 PRECALL                  1
-                     698 CALL                     1
-                     708 LOAD_CONST              11 (-1)
-                     710 BINARY_SUBSCR
-                     720 STORE_FAST               4 (ext)
-         
-          35         722 LOAD_GLOBAL             11 (NULL + logger)
-                     734 LOAD_ATTR               11 (error)
-                     744 LOAD_CONST              12 ('Extension ')
-                     746 LOAD_FAST                4 (ext)
-                     748 FORMAT_VALUE             0
-                     750 LOAD_CONST              13 (' not supported, exiting ...')
-                     752 BUILD_STRING             3
-                     754 PRECALL                  1
-                     758 CALL                     1
-                     768 POP_TOP
+          33         600 LOAD_GLOBAL             11 (NULL + logger)
+                     612 LOAD_ATTR                6 (debug)
+                     622 LOAD_CONST              11 ('C/C++ code detected ...')
+                     624 PRECALL                  1
+                     628 CALL                     1
+                     638 POP_TOP
+         
+          34         640 LOAD_GLOBAL             17 (NULL + remove_ifdef_from_module)
+                     652 LOAD_FAST                3 (code)
+                     654 BUILD_LIST               0
+                     656 LOAD_FAST                1 (verbose)
+                     658 PRECALL                  3
+                     662 CALL                     3
+                     672 STORE_FAST               3 (code)
+         
+          35         674 LOAD_GLOBAL             21 (NULL + unformat_c)
+                     686 LOAD_FAST                3 (code)
+                     688 PRECALL                  1
+                     692 CALL                     1
+                     702 STORE_FAST               4 (statements)
+                     704 JUMP_FORWARD            71 (to 848)
+         
+          37     >>  706 LOAD_FAST                0 (filename)
+                     708 LOAD_METHOD              3 (lower)
+                     730 PRECALL                  0
+                     734 CALL                     0
+                     744 LOAD_METHOD             11 (split)
+                     766 LOAD_CONST              12 ('.')
+                     768 PRECALL                  1
+                     772 CALL                     1
+                     782 LOAD_CONST              13 (-1)
+                     784 BINARY_SUBSCR
+                     794 STORE_FAST               5 (ext)
+         
+          38         796 LOAD_GLOBAL             11 (NULL + logger)
+                     808 LOAD_ATTR               12 (error)
+                     818 LOAD_CONST              14 ('Extension ')
+                     820 LOAD_FAST                5 (ext)
+                     822 FORMAT_VALUE             0
+                     824 LOAD_CONST              15 (' not supported, exiting ...')
+                     826 BUILD_STRING             3
+                     828 PRECALL                  1
+                     832 CALL                     1
+                     842 POP_TOP
          
-          36         770 BUILD_LIST               0
-                     772 STORE_FAST               3 (statements)
+          39         844 BUILD_LIST               0
+                     846 STORE_FAST               4 (statements)
          
-          38     >>  774 LOAD_FAST                3 (statements)
-                     776 RETURN_VALUE
+          41     >>  848 LOAD_FAST                4 (statements)
+                     850 RETURN_VALUE
          ExceptionTable:
            34 to 110 -> 136 [1] lasti
            136 to 142 -> 144 [3] lasti
            150 to 150 -> 144 [3] lasti
          consts
             '\n    Main function to call to get an unformated version of the code\n\n    Args:\n        filename (str): _description_\n\n    Returns:\n        list: _description_\n    '
             'r'
@@ -252,15 +288,15 @@
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 19
                code
                   0x970067007c005d167d017c01a000000000000000000000000000000000
                   0000000000a6000000ab00000000000000000091028c175300
-                22           0 RESUME                   0
+                23           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                22 (to 52)
                              8 STORE_FAST               1 (line)
                             10 LOAD_FAST                1 (line)
                             12 LOAD_METHOD              0 (lower)
                             34 PRECALL                  0
@@ -271,38 +307,41 @@
                consts
                names      ('lower',)
                varnames   ('.0', 'line')
                freevars   ()
                cellvars   ()
                filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_main.py'
                name       '<listcomp>'
-               firstlineno 22
+               firstlineno 23
                lnotab 0x
             '.py'
             'Python code detected ...'
             ('.f', '.F', '.f77', '.f90')
             'Fortran code detected ...'
-            ('.c', '.cpp', '.cc')
+            True
+            ('fortran',)
+            ('.c', '.cpp', '.cc', '.h')
             'C/C++ code detected ...'
             '.'
             -1
             'Extension '
             ' not supported, exiting ...'
-         names      ('open', 'read', 'splitlines', 'lower', 'endswith', 'logger', 'debug', 'unformat_py', 'unformat_ftn', 'unformat_c', 'split', 'error')
-         varnames   ('filename', 'fin', 'code', 'statements', 'ext')
+         names      ('open', 'read', 'splitlines', 'lower', 'endswith', 'logger', 'debug', 'unformat_py', 'remove_ifdef_from_module', 'unformat_ftn', 'unformat_c', 'split', 'error')
+         varnames   ('filename', 'verbose', 'fin', 'code', 'statements', 'ext')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_main.py'
          name       'unformat_main'
-         firstlineno 9
+         firstlineno 10
          lnotab
-            0x020a22014cff2e0318024e01280120014e01280120014e01280120025a
-            0130010402
+            0x020a22014cff2e0318024e01280122014e012801260120014e01280122
+            0120025a0130010402
       None
-   names      ('__doc__', 'loguru', 'logger', 'tucan.unformat_py', 'unformat_py', 'tucan.unformat_ftn', 'unformat_ftn', 'tucan.unformat_c', 'unformat_c', 'str', 'list', 'unformat_main')
+      (False,)
+   names      ('__doc__', 'loguru', 'logger', 'tucan.unformat_py', 'unformat_py', 'tucan.unformat_ftn', 'unformat_ftn', 'tucan.unformat_c', 'unformat_c', 'tucan.clean_ifdef', 'remove_ifdef_from_module', 'str', 'bool', 'list', 'unformat_main')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_main.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104010c020c010c010c03
+   lnotab 0x00ff020104010c020c010c010c010c03
```

### Comparing `tucan-0.1.0/src/tucan/__pycache__/unformat_py.cpython-311.pyc` & `tucan-0.2.0/src/tucan/__pycache__/unformat_py.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,26 +1,27 @@
 magic:    0xa70d0d0a
-moddate:  0x41c6b765 (Mon Jan 29 15:37:37 2024 UTC)
-files sz: 5771
+moddate:  0xf84de765 (Tue Mar  5 16:53:12 2024 UTC)
+files sz: 6059
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a056d065a066d075a076d085a086d095a096d0a5a0a6d0b5a
       0b6d0c5a0c01006404640564069c025a0d64076503650e19000000000000
       00000064086503650e190000000000000000006604640984045a0f640765
       03650e1900000000000000000064086503650e1900000000000000000066
       04640a84045a10640b6505640865056604640c84045a11640b6505640d65
       0e640865056606640e84045a12640b6505640865056604640f84045a1364
-      076503650e190000000000000000006410650e6411650e64086503650e19
-      0000000000000000006608641284045a1464076503650e19000000000000
-      000000640865056604641384045a1564145300
+      076503650e1900000000000000000064086503650e190000000000000000
+      006604641084045a1464076503650e190000000000000000006411650e64
+      12650e64086503650e190000000000000000006608641384045a15640765
+      03650e19000000000000000000640865056604641484045a1664155300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('logger',))
                  6 IMPORT_NAME              0 (loguru)
                  8 IMPORT_FROM              1 (logger)
                 10 STORE_NAME               1 (logger)
@@ -113,43 +114,56 @@
                196 LOAD_CONST               8 ('return')
                198 LOAD_NAME                5 (Statements)
                200 BUILD_TUPLE              4
                202 LOAD_CONST              15 (<code object align_context_block, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_py.py", line 93>)
                204 MAKE_FUNCTION            4 (annotations)
                206 STORE_NAME              19 (align_context_block)
    
-   135         208 LOAD_CONST               7 ('code')
+   133         208 LOAD_CONST               7 ('code')
                210 LOAD_NAME                3 (List)
                212 LOAD_NAME               14 (str)
                214 BINARY_SUBSCR
-               224 LOAD_CONST              16 ('fstring_char')
-               226 LOAD_NAME               14 (str)
-               228 LOAD_CONST              17 ('other_char')
-               230 LOAD_NAME               14 (str)
-               232 LOAD_CONST               8 ('return')
-               234 LOAD_NAME                3 (List)
-               236 LOAD_NAME               14 (str)
-               238 BINARY_SUBSCR
-               248 BUILD_TUPLE              8
-               250 LOAD_CONST              18 (<code object split_fstrings, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_py.py", line 135>)
-               252 MAKE_FUNCTION            4 (annotations)
-               254 STORE_NAME              20 (split_fstrings)
+               224 LOAD_CONST               8 ('return')
+               226 LOAD_NAME                3 (List)
+               228 LOAD_NAME               14 (str)
+               230 BINARY_SUBSCR
+               240 BUILD_TUPLE              4
+               242 LOAD_CONST              16 (<code object replace_keywords, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_py.py", line 133>)
+               244 MAKE_FUNCTION            4 (annotations)
+               246 STORE_NAME              20 (replace_keywords)
    
-   172         256 LOAD_CONST               7 ('code')
-               258 LOAD_NAME                3 (List)
-               260 LOAD_NAME               14 (str)
-               262 BINARY_SUBSCR
+   142         248 LOAD_CONST               7 ('code')
+               250 LOAD_NAME                3 (List)
+               252 LOAD_NAME               14 (str)
+               254 BINARY_SUBSCR
+               264 LOAD_CONST              17 ('fstring_char')
+               266 LOAD_NAME               14 (str)
+               268 LOAD_CONST              18 ('other_char')
+               270 LOAD_NAME               14 (str)
                272 LOAD_CONST               8 ('return')
-               274 LOAD_NAME                5 (Statements)
-               276 BUILD_TUPLE              4
-               278 LOAD_CONST              19 (<code object unformat_py, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_py.py", line 172>)
-               280 MAKE_FUNCTION            4 (annotations)
-               282 STORE_NAME              21 (unformat_py)
-               284 LOAD_CONST              20 (None)
-               286 RETURN_VALUE
+               274 LOAD_NAME                3 (List)
+               276 LOAD_NAME               14 (str)
+               278 BINARY_SUBSCR
+               288 BUILD_TUPLE              8
+               290 LOAD_CONST              19 (<code object split_fstrings, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_py.py", line 142>)
+               292 MAKE_FUNCTION            4 (annotations)
+               294 STORE_NAME              21 (split_fstrings)
+   
+   179         296 LOAD_CONST               7 ('code')
+               298 LOAD_NAME                3 (List)
+               300 LOAD_NAME               14 (str)
+               302 BINARY_SUBSCR
+               312 LOAD_CONST               8 ('return')
+               314 LOAD_NAME                5 (Statements)
+               316 BUILD_TUPLE              4
+               318 LOAD_CONST              20 (<code object unformat_py, file "/Users/dauptain/GITLAB/tucan/src/tucan/unformat_py.py", line 179>)
+               320 MAKE_FUNCTION            4 (annotations)
+               322 STORE_NAME              22 (unformat_py)
+               324 LOAD_CONST              21 (None)
+               326 RETURN_VALUE
    consts
       0
       ('logger',)
       ('List',)
       ('Statements', 'new_stmts', 'remove_strings', 'clean_blanks', 'eat_spaces', 'clean_inline_comments', 'split_multi_statement_lines', 'get_indent')
       'ª'
       '»'
@@ -728,14 +742,64 @@
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_py.py'
          name       'align_context_block'
          firstlineno 93
          lnotab
             0x020a04010401040104014401040104011e022c010a0108012a01020108
             0102012e0112013aff080202fb0209040130012e010602
+      code
+         argcount  : 1
+         nlocals   : 4
+         stacksize : 5
+         flags     : 3
+         code
+            0x970067007d017c0044005d2d7d027c02a0000000000000000000000000
+            00000000000000000064016402a6020000ab0200000000000000007d037c
+            01a00100000000000000000000000000000000000000007c03a6010000ab
+            01000000000000000001008c2e7c015300
+         133           0 RESUME                   0
+         
+         135           2 BUILD_LIST               0
+                       4 STORE_FAST               1 (new_stmt)
+         
+         137           6 LOAD_FAST                0 (code)
+                       8 GET_ITER
+                 >>   10 FOR_ITER                45 (to 102)
+                      12 STORE_FAST               2 (line)
+         
+         138          14 LOAD_FAST                2 (line)
+                      16 LOAD_METHOD              0 (replace)
+                      38 LOAD_CONST               1 ('super()')
+                      40 LOAD_CONST               2 ('self_super')
+                      42 PRECALL                  2
+                      46 CALL                     2
+                      56 STORE_FAST               3 (new_line)
+         
+         139          58 LOAD_FAST                1 (new_stmt)
+                      60 LOAD_METHOD              1 (append)
+                      82 LOAD_FAST                3 (new_line)
+                      84 PRECALL                  1
+                      88 CALL                     1
+                      98 POP_TOP
+                     100 JUMP_BACKWARD           46 (to 10)
+         
+         140     >>  102 LOAD_FAST                1 (new_stmt)
+                     104 RETURN_VALUE
+         consts
+            'replace some uneasy keywords for parsing'
+            'super()'
+            'self_super'
+         names      ('replace', 'append')
+         varnames   ('code', 'new_stmt', 'line', 'new_line')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_py.py'
+         name       'replace_keywords'
+         firstlineno 133
+         lnotab 0x0202040208012c012c01
       'fstring_char'
       'other_char'
       code
          argcount  : 3
          nlocals   : 9
          stacksize : 5
          flags     : 3
@@ -744,113 +808,113 @@
             005d487d087c087c016b0200000000720b7c0764046b0200000000720364
             057d056e0264017d057c0572087c087c026b0200000000720264067d087c
             067c087a0d00007d067c0572227c0864076b020000000072117c06640064
             088502190000000000000000007c017a00000064077a0000007d066e0b7c
             0864096b020000000072057c067c017a0d00007d067c087d078c497c03a0
             0000000000000000000000000000000000000000007c06a6010000ab0100
             0000000000000001008c697c035300
-         135           0 RESUME                   0
+         142           0 RESUME                   0
          
-         136           2 BUILD_LIST               0
+         143           2 BUILD_LIST               0
                        4 STORE_FAST               3 (new_stmt)
          
-         138           6 LOAD_FAST                0 (code)
+         145           6 LOAD_FAST                0 (code)
                        8 GET_ITER
                  >>   10 FOR_ITER               104 (to 220)
                       12 STORE_FAST               4 (line)
          
-         139          14 LOAD_CONST               1 (False)
+         146          14 LOAD_CONST               1 (False)
                       16 STORE_FAST               5 (inside_fstring_context)
          
-         141          18 LOAD_CONST               2 ('')
+         148          18 LOAD_CONST               2 ('')
                       20 STORE_FAST               6 (buffer)
          
-         142          22 LOAD_CONST               3 (' ')
+         149          22 LOAD_CONST               3 (' ')
                       24 STORE_FAST               7 (last_char)
          
-         143          26 LOAD_FAST                4 (line)
+         150          26 LOAD_FAST                4 (line)
                       28 GET_ITER
                  >>   30 FOR_ITER                72 (to 176)
                       32 STORE_FAST               8 (char)
          
-         144          34 LOAD_FAST                8 (char)
+         151          34 LOAD_FAST                8 (char)
                       36 LOAD_FAST                1 (fstring_char)
                       38 COMPARE_OP               2 (==)
                       44 POP_JUMP_FORWARD_IF_FALSE    11 (to 68)
          
-         145          46 LOAD_FAST                7 (last_char)
+         152          46 LOAD_FAST                7 (last_char)
                       48 LOAD_CONST               4 ('f')
                       50 COMPARE_OP               2 (==)
                       56 POP_JUMP_FORWARD_IF_FALSE     3 (to 64)
          
-         146          58 LOAD_CONST               5 (True)
+         153          58 LOAD_CONST               5 (True)
                       60 STORE_FAST               5 (inside_fstring_context)
                       62 JUMP_FORWARD             2 (to 68)
          
-         148     >>   64 LOAD_CONST               1 (False)
+         155     >>   64 LOAD_CONST               1 (False)
                       66 STORE_FAST               5 (inside_fstring_context)
          
-         150     >>   68 LOAD_FAST                5 (inside_fstring_context)
+         157     >>   68 LOAD_FAST                5 (inside_fstring_context)
                       70 POP_JUMP_FORWARD_IF_FALSE     8 (to 88)
                       72 LOAD_FAST                8 (char)
                       74 LOAD_FAST                2 (other_char)
                       76 COMPARE_OP               2 (==)
                       82 POP_JUMP_FORWARD_IF_FALSE     2 (to 88)
          
-         151          84 LOAD_CONST               6 ('_')
+         158          84 LOAD_CONST               6 ('_')
                       86 STORE_FAST               8 (char)
          
-         153     >>   88 LOAD_FAST                6 (buffer)
+         160     >>   88 LOAD_FAST                6 (buffer)
                       90 LOAD_FAST                8 (char)
                       92 BINARY_OP               13 (+=)
                       96 STORE_FAST               6 (buffer)
          
-         155          98 LOAD_FAST                5 (inside_fstring_context)
+         162          98 LOAD_FAST                5 (inside_fstring_context)
                      100 POP_JUMP_FORWARD_IF_FALSE    34 (to 170)
          
-         156         102 LOAD_FAST                8 (char)
+         163         102 LOAD_FAST                8 (char)
                      104 LOAD_CONST               7 ('{')
                      106 COMPARE_OP               2 (==)
                      112 POP_JUMP_FORWARD_IF_FALSE    17 (to 148)
          
-         158         114 LOAD_FAST                6 (buffer)
+         165         114 LOAD_FAST                6 (buffer)
                      116 LOAD_CONST               0 (None)
                      118 LOAD_CONST               8 (-2)
                      120 BUILD_SLICE              2
                      122 BINARY_SUBSCR
                      132 LOAD_FAST                1 (fstring_char)
                      134 BINARY_OP                0 (+)
                      138 LOAD_CONST               7 ('{')
                      140 BINARY_OP                0 (+)
                      144 STORE_FAST               6 (buffer)
                      146 JUMP_FORWARD            11 (to 170)
          
-         160     >>  148 LOAD_FAST                8 (char)
+         167     >>  148 LOAD_FAST                8 (char)
                      150 LOAD_CONST               9 ('}')
                      152 COMPARE_OP               2 (==)
                      158 POP_JUMP_FORWARD_IF_FALSE     5 (to 170)
          
-         162         160 LOAD_FAST                6 (buffer)
+         169         160 LOAD_FAST                6 (buffer)
                      162 LOAD_FAST                1 (fstring_char)
                      164 BINARY_OP               13 (+=)
                      168 STORE_FAST               6 (buffer)
          
-         165     >>  170 LOAD_FAST                8 (char)
+         172     >>  170 LOAD_FAST                8 (char)
                      172 STORE_FAST               7 (last_char)
                      174 JUMP_BACKWARD           73 (to 30)
          
-         167     >>  176 LOAD_FAST                3 (new_stmt)
+         174     >>  176 LOAD_FAST                3 (new_stmt)
                      178 LOAD_METHOD              0 (append)
                      200 LOAD_FAST                6 (buffer)
                      202 PRECALL                  1
                      206 CALL                     1
                      216 POP_TOP
                      218 JUMP_BACKWARD          105 (to 10)
          
-         168     >>  220 LOAD_FAST                3 (new_stmt)
+         175     >>  220 LOAD_FAST                3 (new_stmt)
                      222 RETURN_VALUE
          consts
             None
             False
             ''
             ' '
             'f'
@@ -861,15 +925,15 @@
             '}'
          names      ('append',)
          varnames   ('code', 'fstring_char', 'other_char', 'new_stmt', 'line', 'inside_fstring_context', 'buffer', 'last_char', 'char')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_py.py'
          name       'split_fstrings'
-         firstlineno 135
+         firstlineno 142
          lnotab
             0x02010402080104020401040108010c010c0106020402100104020a0204
             010c0222020c020a0306022c01
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 5
@@ -894,169 +958,181 @@
             015f020000000000000000740d000000000000000000007c016a02000000
             00000000006404a6020000ab0200000000000000007c015f020000000000
             0000007411000000000000000000007c016405a6020000ab020000000000
             0000007d017413000000000000000000007c01a6010000ab010000000000
             0000007d017415000000000000000000007c01a6010000ab010000000000
             0000007d017417000000000000000000007c01a6010000ab010000000000
             0000007d017419000000000000000000007c016a020000000000000000a6
-            010000ab0100000000000000007c015f0200000000000000007c015300
-         172           0 RESUME                   0
+            010000ab0100000000000000007c015f020000000000000000741b000000
+            000000000000007c016a020000000000000000a6010000ab010000000000
+            0000007c015f0200000000000000007c015300
+         179           0 RESUME                   0
          
-         182           2 LOAD_GLOBAL              1 (NULL + new_stmts)
+         189           2 LOAD_GLOBAL              1 (NULL + new_stmts)
                       14 LOAD_FAST                0 (code)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               1 (stmts)
          
-         183          32 LOAD_GLOBAL              3 (NULL + eat_spaces)
+         190          32 LOAD_GLOBAL              3 (NULL + eat_spaces)
                       44 LOAD_FAST                1 (stmts)
                       46 LOAD_ATTR                2 (stmt)
                       56 PRECALL                  1
                       60 CALL                     1
                       70 LOAD_FAST                1 (stmts)
                       72 STORE_ATTR               2 (stmt)
          
-         184          82 LOAD_GLOBAL              7 (NULL + remove_combined_chars)
+         191          82 LOAD_GLOBAL              7 (NULL + remove_combined_chars)
                       94 LOAD_FAST                1 (stmts)
                       96 LOAD_ATTR                2 (stmt)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_FAST                1 (stmts)
                      122 STORE_ATTR               2 (stmt)
          
-         185         132 LOAD_GLOBAL              9 (NULL + align_continuation_lines)
+         192         132 LOAD_GLOBAL              9 (NULL + align_continuation_lines)
                      144 LOAD_FAST                1 (stmts)
                      146 PRECALL                  1
                      150 CALL                     1
                      160 STORE_FAST               1 (stmts)
          
-         186         162 LOAD_GLOBAL             11 (NULL + align_multiline_strings)
+         193         162 LOAD_GLOBAL             11 (NULL + align_multiline_strings)
                      174 LOAD_FAST                1 (stmts)
                      176 LOAD_CONST               1 ('ª')
                      178 PRECALL                  2
                      182 CALL                     2
                      192 STORE_FAST               1 (stmts)
          
-         187         194 LOAD_GLOBAL             11 (NULL + align_multiline_strings)
+         194         194 LOAD_GLOBAL             11 (NULL + align_multiline_strings)
                      206 LOAD_FAST                1 (stmts)
                      208 LOAD_CONST               2 ('»')
                      210 PRECALL                  2
                      214 CALL                     2
                      224 STORE_FAST               1 (stmts)
          
-         189         226 LOAD_GLOBAL             13 (NULL + remove_strings)
+         196         226 LOAD_GLOBAL             13 (NULL + remove_strings)
                      238 LOAD_FAST                1 (stmts)
                      240 LOAD_ATTR                2 (stmt)
                      250 LOAD_CONST               1 ('ª')
                      252 PRECALL                  2
                      256 CALL                     2
                      266 LOAD_FAST                1 (stmts)
                      268 STORE_ATTR               2 (stmt)
          
-         190         278 LOAD_GLOBAL             13 (NULL + remove_strings)
+         197         278 LOAD_GLOBAL             13 (NULL + remove_strings)
                      290 LOAD_FAST                1 (stmts)
                      292 LOAD_ATTR                2 (stmt)
                      302 LOAD_CONST               2 ('»')
                      304 PRECALL                  2
                      308 CALL                     2
                      318 LOAD_FAST                1 (stmts)
                      320 STORE_ATTR               2 (stmt)
          
-         191         330 LOAD_GLOBAL             15 (NULL + split_fstrings)
+         198         330 LOAD_GLOBAL             15 (NULL + split_fstrings)
                      342 LOAD_FAST                1 (stmts)
                      344 LOAD_ATTR                2 (stmt)
                      354 LOAD_CONST               3 ("'")
                      356 LOAD_CONST               4 ('"')
                      358 PRECALL                  3
                      362 CALL                     3
                      372 LOAD_FAST                1 (stmts)
                      374 STORE_ATTR               2 (stmt)
          
-         192         384 LOAD_GLOBAL             15 (NULL + split_fstrings)
+         199         384 LOAD_GLOBAL             15 (NULL + split_fstrings)
                      396 LOAD_FAST                1 (stmts)
                      398 LOAD_ATTR                2 (stmt)
                      408 LOAD_CONST               4 ('"')
                      410 LOAD_CONST               3 ("'")
                      412 PRECALL                  3
                      416 CALL                     3
                      426 LOAD_FAST                1 (stmts)
                      428 STORE_ATTR               2 (stmt)
          
-         193         438 LOAD_GLOBAL             13 (NULL + remove_strings)
+         200         438 LOAD_GLOBAL             13 (NULL + remove_strings)
                      450 LOAD_FAST                1 (stmts)
                      452 LOAD_ATTR                2 (stmt)
                      462 LOAD_CONST               3 ("'")
                      464 PRECALL                  2
                      468 CALL                     2
                      478 LOAD_FAST                1 (stmts)
                      480 STORE_ATTR               2 (stmt)
          
-         194         490 LOAD_GLOBAL             13 (NULL + remove_strings)
+         201         490 LOAD_GLOBAL             13 (NULL + remove_strings)
                      502 LOAD_FAST                1 (stmts)
                      504 LOAD_ATTR                2 (stmt)
                      514 LOAD_CONST               4 ('"')
                      516 PRECALL                  2
                      520 CALL                     2
                      530 LOAD_FAST                1 (stmts)
                      532 STORE_ATTR               2 (stmt)
          
-         196         542 LOAD_GLOBAL             17 (NULL + clean_inline_comments)
+         203         542 LOAD_GLOBAL             17 (NULL + clean_inline_comments)
                      554 LOAD_FAST                1 (stmts)
                      556 LOAD_CONST               5 ('#')
                      558 PRECALL                  2
                      562 CALL                     2
                      572 STORE_FAST               1 (stmts)
          
-         197         574 LOAD_GLOBAL             19 (NULL + clean_blanks)
+         204         574 LOAD_GLOBAL             19 (NULL + clean_blanks)
                      586 LOAD_FAST                1 (stmts)
                      588 PRECALL                  1
                      592 CALL                     1
                      602 STORE_FAST               1 (stmts)
          
-         198         604 LOAD_GLOBAL             21 (NULL + split_multi_statement_lines)
+         205         604 LOAD_GLOBAL             21 (NULL + split_multi_statement_lines)
                      616 LOAD_FAST                1 (stmts)
                      618 PRECALL                  1
                      622 CALL                     1
                      632 STORE_FAST               1 (stmts)
          
-         199         634 LOAD_GLOBAL             23 (NULL + align_context_block)
+         206         634 LOAD_GLOBAL             23 (NULL + align_context_block)
                      646 LOAD_FAST                1 (stmts)
                      648 PRECALL                  1
                      652 CALL                     1
                      662 STORE_FAST               1 (stmts)
          
-         201         664 LOAD_GLOBAL             25 (NULL + getback_combined_chars)
+         207         664 LOAD_GLOBAL             25 (NULL + replace_keywords)
                      676 LOAD_FAST                1 (stmts)
                      678 LOAD_ATTR                2 (stmt)
                      688 PRECALL                  1
                      692 CALL                     1
                      702 LOAD_FAST                1 (stmts)
                      704 STORE_ATTR               2 (stmt)
          
-         202         714 LOAD_FAST                1 (stmts)
-                     716 RETURN_VALUE
+         208         714 LOAD_GLOBAL             27 (NULL + getback_combined_chars)
+                     726 LOAD_FAST                1 (stmts)
+                     728 LOAD_ATTR                2 (stmt)
+                     738 PRECALL                  1
+                     742 CALL                     1
+                     752 LOAD_FAST                1 (stmts)
+                     754 STORE_ATTR               2 (stmt)
+         
+         209         764 LOAD_FAST                1 (stmts)
+                     766 RETURN_VALUE
          consts
             '\n    Unformat Python code by stripping comments and breaking multiline statements.\n\n    Args:\n        code (List[str]): List of Python code lines.\n\n    Returns:\n        Statements: List of unformatted code statements along with line number ranges.\n    '
             'ª'
             '»'
             "'"
             '"'
             '#'
-         names      ('new_stmts', 'eat_spaces', 'stmt', 'remove_combined_chars', 'align_continuation_lines', 'align_multiline_strings', 'remove_strings', 'split_fstrings', 'clean_inline_comments', 'clean_blanks', 'split_multi_statement_lines', 'align_context_block', 'getback_combined_chars')
+         names      ('new_stmts', 'eat_spaces', 'stmt', 'remove_combined_chars', 'align_continuation_lines', 'align_multiline_strings', 'remove_strings', 'split_fstrings', 'clean_inline_comments', 'clean_blanks', 'split_multi_statement_lines', 'align_context_block', 'replace_keywords', 'getback_combined_chars')
          varnames   ('code', 'stmts')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_py.py'
          name       'unformat_py'
-         firstlineno 172
+         firstlineno 179
          lnotab
             0x020a1e01320132011e012001200234013401360136013401340220011e
-            011e011e023201
+            011e011e0132013201
       None
-   names      ('loguru', 'logger', 'typing', 'List', 'tucan.unformat_common', 'Statements', 'new_stmts', 'remove_strings', 'clean_blanks', 'eat_spaces', 'clean_inline_comments', 'split_multi_statement_lines', 'get_indent', 'COMB_CHARS', 'str', 'remove_combined_chars', 'getback_combined_chars', 'align_continuation_lines', 'align_multiline_strings', 'align_context_block', 'split_fstrings', 'unformat_py')
+   names      ('loguru', 'logger', 'typing', 'List', 'tucan.unformat_common', 'Statements', 'new_stmts', 'remove_strings', 'clean_blanks', 'eat_spaces', 'clean_inline_comments', 'split_multi_statement_lines', 'get_indent', 'COMB_CHARS', 'str', 'remove_combined_chars', 'getback_combined_chars', 'align_continuation_lines', 'align_multiline_strings', 'align_context_block', 'replace_keywords', 'split_fstrings', 'unformat_py')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/dauptain/GITLAB/tucan/src/tucan/unformat_py.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c02280d020102fe0605280b280b10111421102a3025
+   lnotab
+      0x00ff02010c010c02280d020102fe0605280b280b101114211028280930
+      25
```

### Comparing `tucan-0.1.0/src/tucan/cli.py` & `tucan-0.2.0/src/tucan/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,27 +63,33 @@
 @click.argument("filename", type=str, nargs=1)
 @click.option(
     "-d",
     "--dump",
     is_flag=True,
     help="dump json data",
 )
-def clean(filename, dump):
+@click.option(
+    "-v",
+    "--verbose",
+    is_flag=True,
+    help="verbose mode",
+)
+def clean(filename:str, dump:bool,verbose:bool):
     """
     Unformat a fortran of python single file.
 
     \b
     - Merge multiline statements to one line
     - Split ';' statements
     - Strip comments.
     - Strip blank lines.
     """
     from tucan.unformat_main import unformat_main
 
-    statements = unformat_main(filename)
+    statements = unformat_main(filename, verbose)
 
     base = filename.split("/")[-1].split(".")[0]
     print(statements)
 
     statements.dump_code("./" + base + "._rfmt")
 
     if dump:
@@ -123,30 +129,36 @@
 @click.argument("filename", type=str, nargs=1)
 @click.option(
     "-d",
     "--dump",
     is_flag=True,
     help="dump json data",
 )
-def struct(filename, dump):
+@click.option(
+    "-v",
+    "--verbose",
+    is_flag=True,
+    help="verbose mode",
+)
+def struct(filename, dump, verbose):
     """
     Extract structure of a fortran or python single file.
 
     \b
     - Find the nested structures of a code
     - Find the callables in each structure
     - Evaluate sizes, CCN
     """
     import json
     from loguru import logger
 
     from tucan.struct_main import struct_main
     from tucan.struct_common import struct_summary_str
 
-    struct_ = struct_main(filename)
+    struct_ = struct_main(filename,verbose)
     logger.info("Found following structure:\n" + struct_summary_str(struct_))
     base = filename.split("/")[-1].split(".")[0]
     if dump:
         newfile = base + ".json"
         logger.info(f"Data dumped to {newfile}")
         with open(newfile, "w") as fout:
             json.dump(struct_, fout, indent=2, sort_keys=True)
@@ -248,56 +260,64 @@
 
 
 
 
 @main.command()
 @click.argument("filename", type=str, nargs=1)
 @click.option(
-    "-v",
-    "--variables",
+    "-def",
+    "--definitions",
     type=str,
     default=None,
     # multiple=True,
-    help="Variable to resolve ifdefs. Comma separated ',', no spaces : -v ARG1,ARG2",
+    help="definitions to resolve ifdefs. Comma separated ',', no spaces : -v ARG1,ARG2",
 )
 @click.option(
     "-d",
     "--dump",
     is_flag=True,
     help="dump json data",
 )
-def ifdef_clean(filename, variables,dump):
+@click.option(
+    "-f",
+    "--fortran",
+    is_flag=True,
+    help=" fortran mode (avoid  stripping //)",
+)
+@click.option(
+    "-v",
+    "--verbose",
+    is_flag=True,
+    help="verbose execution",
+)
+def ifdef_clean(filename, definitions,dump,fortran,verbose):
     """
     Show a file with idefs resolved
     """
     from loguru import logger
     from tucan.clean_ifdef import remove_ifdef_from_module
-    logger.critical(variables)
     
-    if variables is None:
-        variables=[]
+    if definitions is None:
+        definitions=[]
     else:
-        variables=variables.split(",")
+        definitions=definitions.split(",")
 
-    logger.critical(variables)
     with open(filename,"r") as fin:
-        lines = fin.read().split("\n")
-     
-    lines = remove_ifdef_from_module(lines,variables)
-    
+        lines = fin.read().split("\n") 
+    lines = remove_ifdef_from_module(lines,definitions,verbose=verbose, fortran=fortran)
     logger.success("Ifdefs resolved:")
     for line in lines:
         print(line)
     if dump:
         newfile=filename+"_ifdef_resolved"
         lines.append("# the ifdefs were resolved by tucan")
-        v_s = ", ".join(variables)
-        lines.append(f"# IFdef Variables: {variables}")
+        v_s = ", ".join(definitions)
+        lines.append(f"# IFdef Variables: {definitions}")
         with open(newfile, "w") as fout:
-            fout.writelines(lines)
+            fout.write("\n".join(lines))
 
 @main.command()
 @click.argument("path", type=str, nargs=1)
 @click.option(
     "-d",
     "--dump",
     is_flag=True,
```

### Comparing `tucan-0.1.0/src/tucan/imports_common.py` & `tucan-0.2.0/src/tucan/imports_common.py`

 * *Files identical despite different names*

### Comparing `tucan-0.1.0/src/tucan/imports_ftn.py` & `tucan-0.2.0/src/tucan/imports_ftn.py`

 * *Files identical despite different names*

### Comparing `tucan-0.1.0/src/tucan/imports_main.py` & `tucan-0.2.0/src/tucan/imports_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Tucan module to handle the import parsing of all files.
 """
 from loguru import logger
 
 from tucan.unformat_py import unformat_py
 from tucan.unformat_ftn import unformat_ftn
+from tucan.unformat_c import unformat_c
 from tucan.imports_py import imports_py
 from tucan.imports_ftn import imports_ftn
+from tucan.imports_c import imports_c
 
 
 def imports_main(filename: str) -> dict:
     """
     Extract the imports of a code file.
 
     Args:
@@ -29,16 +31,20 @@
     code = [line.lower() for line in code]  # Lower case for all
 
     imports_ = {}
     if filename.lower().endswith(".py"):
         logger.debug(f"Python code detected ...")
         statements = unformat_py(code)
         imports_ = imports_py(statements)
-    elif filename.lower().endswith((".f", ".F", ".f77", ".f90")):
+    elif filename.lower().endswith((".f", ".F", ".f77", ".f90", ".inc")):
         logger.debug(f"Fortran code detected ...")
         statements = unformat_ftn(code)
         imports_ = imports_ftn(statements)
+    elif filename.lower().endswith((".c", ".h")):
+        logger.debug(f"C/C++ code detected ...")
+        statements = unformat_c(code)
+        imports_ = imports_c(statements)
     else:
         ext = filename.lower().split(".")[-1]
         logger.error(f"Extension {ext} not supported, exiting ...")
         return {}
     return imports_
```

### Comparing `tucan-0.1.0/src/tucan/imports_py.py` & `tucan-0.2.0/src/tucan/imports_py.py`

 * *Files identical despite different names*

### Comparing `tucan-0.1.0/src/tucan/kw_lang.py` & `tucan-0.2.0/src/tucan/kw_lang.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,17 @@
     'extern', 'false', 'float', 'for', 'goto', 'if', 'inline', 'int', 'long',
     'nullptr', 'register', 'restrict', 'return', 'short', 'signed', 'sizeof',
     'static', 'static_assert', 'struct', 'switch', 'thread_local', 'true',
     'typedef', 'typeof', 'typeof_unqual', 'union', 'unsigned', 'void', 'volatile',
     'while', '_Alignas', '_Alignof', '_Atomic', '_BitInt', '_Bool', '_Complex',
     '_Decimal128', '_Decimal32', '_Decimal64', '_Generic', '_Imaginary',
     '_Noreturn', '_Static_assert', '_Thread_local',
-    'printf',
+    'printf','snprintf',
+    'strlen','strcmp','strcpy','strncmp',
+    'max','min'
 ]
 
 
 KEYWORDS_PY = [
     "abs",
     "aiter",
     "all",
@@ -164,14 +166,15 @@
     "btest" : "other",
     "call" : "other",
     "case" : "other",
     "ceiling" : "other",
     "char" : "other",
     "character" : "other",
     "close" : "other",
+    "class" : "other",
     "cmplx" : "other",
     "common" : "other",
     "conjg" : "other",
     "contains" : "other",
     "continue" : "other",
     "cos" : "other",
     "cosh" : "other",
@@ -201,14 +204,15 @@
     "equivalence" : "other",
     "erf" : "other",
     "erfc" : "other",
     "etime" : "other",
     "exit" : "other",
     "exp" : "other",
     "exponent" : "other",
+    "extends" : "other",
     "extends_type_of" : "other",
     "external" : "other",
     "floor" : "other",
     "forall" : "nesting",
     "format" : "other",
     "fraction" : "other",
     "function" : "structure",
```

### Comparing `tucan-0.1.0/src/tucan/package_analysis.py` & `tucan-0.2.0/src/tucan/package_analysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from tucan.unformat_main import unformat_main
 from tucan.struct_main import struct_main
 from tucan.imports_main import imports_main
 
 
 def rec_travel_through_package(path: str,  optional_paths: list = None,) -> list:
     """
-    List all paths from a folder and its subfolders recursively.
+    List all paths from a folder and its sub-folders recursively.
 
     RECURSIVE
     """
     if not optional_paths:
         optional_paths = []
 
     current_paths_list = [path, *optional_paths]
@@ -43,15 +43,19 @@
         paths_list (list): List of all paths gatheres through recursive analysis
 
     Returns:
         list: List of cleaned paths.
     """
     clean_paths = []
     for path in paths_list:
-        if path.endswith((".py", ".f90", ".f", ".F", ".f77", ".c")):
+        if path.endswith((
+            ".py", 
+            ".f", ".F", ".f77", ".f90", 
+            ".c",".cpp", ".h",".hpp"
+            )):
             clean_paths.append(path)
 
     return [
         *set(clean_paths),
     ]
 
 
@@ -89,18 +93,34 @@
 
     Returns:
         dict: _description_
     """
 
     full_analysis = {}
     
+    skipped_files=[]
+    unrecoverable_files=[]
     for file ,path_ in files.items():
         full_analysis[file] = {"imports": imports_main(path_)}
-        full_analysis[file].update(struct_main(path_))
+        analysis = struct_main(path_)
+        if analysis == {}:
+            skipped_files.append(file)
+        if analysis == None:
+            unrecoverable_files.append(file)
+            analysis={}
+            
+        full_analysis[file].update(analysis)
     logger.success("Analyze completed.")
+    if unrecoverable_files:
+        logger.warning("Some files could not be parsed correctly")
+        for f_ in unrecoverable_files+skipped_files:
+            print(" - ", f_)
+  
+
+        
     return full_analysis
 
 
 def run_unformat(clean_paths: list) -> dict:
     """
     Gather the unformated version of code files within a dict.
```

### Comparing `tucan-0.1.0/src/tucan/struct_c.py` & `tucan-0.2.0/src/tucan/struct_c.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,79 @@
 import re
 from typing import Tuple, List
 from loguru import logger
 from tucan.unformat_common import Statements
 from tucan.struct_common import (
     find_words_before_left_parenthesis,
-    buffer_item,
-    stack_item,
+    new_buffer_item,
+    new_stack_item,
     struct_from_stack,
     struct_augment,
 )
 
 from tucan.kw_lang import KEYWORDS_C
 
-def extract_struct_c(stmts: Statements) -> dict:
+def extract_struct_c(stmts: Statements, verbose:bool) -> dict:
     """Main calls to build structure form statements
 
     statements is the output of tucan.unformat_c.unformat_c
     """
+    
     clean_code = stmts.to_code()
-    all_structs = _extract_on_cleaned_c(stmts)
+    all_structs = _extract_on_cleaned_c(stmts, verbose=verbose)
     all_structs = struct_augment(all_structs, clean_code, find_callables_c, compute_ccn_approx_c)
     return all_structs
 
 
-def _extract_on_cleaned_c(stmts: Statements) -> dict:
+def _extract_on_cleaned_c(stmts: Statements, verbose:bool=False) -> dict:
     """Extract structure from cleaned statements."""
     buffer = []
     stack = []
     path = []
 
     stat_idx = 0
 
     level = 0
     stack_level=[None]
 
     for line, (line_idx1, line_idx2) in zip(stmts.stmt, stmts.lines):
         stat_idx += 1
         part=""
-        print(line)
+        #print(line)
         
         
         if "###===" in line:
-                type_,name = _parse_type_name_c(line)
+                type_,name = _parse_type_name_c(line,line_idx1)
                 stack_level.append(level)
+                path.append(name)
                 buffer.append(
-                    buffer_item(
+                    new_buffer_item(
                         type_=type_,
+                        path=path,
                         name=name,
                         first_line=line,
                         line_idx=line_idx1,
                         statement_idx=stat_idx,
+                        verbose=verbose
                     )
                 )
-                path.append(name)
-                print("SOP", path)
                 part=""
         
         for char in line:
             part+=char
             if char=="{":
                 level +=1
             if char=="}":
                 level -=1
                 if level == stack_level[-1]:  
-                    print("EOP", path)
-                    (type_, name, line_start, line_idx, statement_idx) = buffer[-1]
+                    if verbose:
+                        logger.critical(f"Stop :{str(path)}")
+                    last_buff = buffer[-1]
                     stack.append(
-                        stack_item(
-                            type_=type_,
-                            name=name,
-                            path=path.copy(),
-                            start_line_idx=line_idx,
-                            start_statement_idx=statement_idx,
-                            start_line=line_start,
-                            end_line_idx=line_idx2,
-                            end_statement_idx=stat_idx,
-                            end_line=line,
-                        )
+                        new_stack_item(last_buff,line_idx2,stat_idx,line)
                     )
                     path.pop(-1)
                     buffer.pop(-1)
                     stack_level.pop(-1)
                 
 
     return struct_from_stack(stack, main_types=[
@@ -91,24 +84,24 @@
             "subroutine ",
             "derived_type ",
             "userdef_type ",
             "pointer "
         ])
 
 
-def _parse_type_name_c(line: str)->Tuple[str, str]:
+def _parse_type_name_c(line: str, line_idx:int)->Tuple[str, str]:
     """expect a lowercase stripped line
     takes the second word as the name
     """
     if line.strip()=="":
         return None,None
 
     for kw in ["for", "if", "else", "switch"]:
         if line.strip().startswith(f"{kw} "):
-            return kw, kw
+            return kw, kw+str(line_idx+1)
     
     rtype,name = line.replace("(", " ").split()[0:2]
     if rtype in ["void"]:
         type_ = "subroutine "
     elif rtype in ["int", "double", "char","float"]:
         type_ = "function "
     elif rtype in ["struct","enum","class" ]:
```

### Comparing `tucan-0.1.0/src/tucan/struct_common.py` & `tucan-0.2.0/src/tucan/struct_common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Module that gather the most common functions of struct.
 """
 
 import re
+from dataclasses import dataclass
 from typing import Tuple, List,Callable
 from copy import deepcopy
 from loguru import logger
+from typing import List
 
 def path_clean(path: list, paths_to_clean: Tuple[list]):
     """Remove the unwanted steps of the paths"""
     indexes_to_clean = []
     for ptc in paths_to_clean:
         if list2pathref(path).startswith(list2pathref(ptc)):
             indexes_to_clean.append(len(ptc) - 1)
@@ -44,31 +46,32 @@
         )
         out.append(f'    {data["ssize"]} statements over {data["NLOC"]} lines')
         out.append(f'    Complexity {data["CCN"]}')
         if data["callables"]:
             list_str = "\n       - " + "\n       - ".join(data["callables"])
 
             out.append(f'    Refers to {len(data["callables"])} callables:{list_str}')
-        else:
-            out.append(f"    Contains no callables")
+        
         if data["contains"]:
             list_str = "\n    - " + "\n    - ".join(data["contains"])
             out.append(f'    Contains {len(data["contains"])} elements:{list_str}')
-        else:
-            out.append(f"    Contains no inner structures")
+
+
+        if data["parents"]:
+            list_str = "\n       - " + "\n       - ".join(data["parents"])
+            out.append(f'    Refers to {len(data["parents"])} parents:{list_str}')
         
         if data["annotations"]:
-            keyvals=[ keys+":"+values for key,values in data["annotations"].items()]
+            keyvals=[ key+":"+values for key,values in data["annotations"].items()]
             list_str = "\n       - " + "\n       - ".join(keyvals)
 
             out.append(f'    Refers to {len(keyvals)} callables:{list_str}')
-        else:
-            out.append(f"    Contains no annotations")
         
 
+
     return "\n".join(out)
 
 
 def find_words_before_left_parenthesis(line: str) -> List[str]:
     """Find all words before a left parenthesis in a line"""
 
     # Adding a threshold to avoid long running time (most likely for big arithmetic lines)
@@ -78,134 +81,162 @@
 
     # Define a regular expression pattern to find words before a left parenthesis
     pattern = r"(.*?\S)\("
     # Use re.findall to find all matches in the code
     matches = re.findall(pattern, line)
     clean_matches = []
 
-    tokens = ",+-/*<>=;|(){}[]:~ "
+    tokens = ",+-/*<>=;|(){}[]:&!~ "
     for match_ in matches:
         token=""
         for i in range(len(match_),0,-1):
             if match_[i-1] in tokens:
                 break
             token=match_[i-1]+token
         
         if token != "":
             clean_matches.append(token)
     return clean_matches
 
 
 ########################################################
 # BUFFER of detection
-
-
-def buffer_item(
-    type_: str,
-    name: str,
-    first_line: str,
-    line_idx: int,
-    statement_idx: int,
-) -> Tuple[str, str, str, int, int]:
+@dataclass
+class BufferItem():
     """Forces buffers to keep the same logic across languages"""
-    return (
-        type_,
-        name,
-        first_line,
-        line_idx,
-        statement_idx,
+    type_: str=None
+    name: str=None
+    path: list=None
+    first_line: str=None
+    line_idx: int=None
+    statement_idx: int=None
+    parents:List[str]=None
+    callables:List[str]=None
+    contains:List[str]=None
+
+def new_buffer_item(
+        type_: str=None,
+        name: str=None,
+        path: List[str]=None,
+        first_line: str=None,
+        line_idx: int=None,
+        statement_idx: int=None,
+        verbose:bool=False,
+        parents:List[str]=None,
+        callables:List[str]=None,
+        contains:List[str]=None,    
+    )-> BufferItem:
+
+    if verbose:
+        fname = ".".join(path)
+        logger.critical(f"START l.{line_idx} for "+fname)
+    if parents is None:
+        parents=[]
+    if callables is None:
+        callables=[]
+    if contains is None:
+        contains=[]
+    out = BufferItem(
+        type_=type_,
+        name=name,
+        path=path,
+        first_line=first_line,
+        line_idx=line_idx,
+        statement_idx=statement_idx,
+        parents=parents,
+        callables=callables,
+        contains=contains
     )
-
+    return out
 
 ########################################################
 # STACK of detection
-
-
-def stack_item(
-    type_: str,
-    name: str,
-    path: list,
-    start_line_idx: int,
-    start_statement_idx: int,
-    start_line: str,
-    end_line_idx: int,
-    end_statement_idx: int,
-    end_line: str,
-) -> Tuple[str, str, list, int, int, str, int, int, str]:
-    """Forces stacks to keep the same logic across languages"""
-
-    try:
-        if path[-1] != name:  # last item of path should be name
-            logger.warning(f"Path {str(path)} does not end with {name}")
-    except IndexError:
-        raise RuntimeError(f"Structure -{name}- has no path")
-
-    return (
-        type_,
-        name,
-        path,
-        start_line_idx,
-        start_statement_idx,
-        start_line,
-        end_line_idx,
-        end_statement_idx,
-        end_line,
+@dataclass
+class StackItem():
+    """Forces buffers to keep the same logic across languages"""
+    type_: str
+    name: str
+    path: list
+    start_line_idx: int
+    start_statement_idx: int
+    start_line: str
+    end_line_idx: int
+    end_statement_idx: int
+    end_line: str
+    parents:List[str]=None
+    callables:List[str]=None
+    contains:List[str]=None
+
+
+def new_stack_item(
+        buf:BufferItem,
+        end_line_idx:int,
+        end_statement_idx:int,
+        end_line:str,
+        verbose:bool=False
+    )-> StackItem:
+    if verbose:
+        fname = ".".join(buf.path)
+        logger.critical(f"END l.{end_line_idx} for "+fname)
+    out =StackItem(
+        type_=buf.type_,
+        name=buf.name,
+        path=buf.path.copy(),
+        start_line_idx=buf.line_idx,
+        start_statement_idx=buf.statement_idx,
+        start_line=buf.first_line,
+        parents=buf.parents,
+        callables=buf.callables,
+        contains=buf.contains,
+        end_line_idx=end_line_idx,
+        end_statement_idx=end_statement_idx,
+        end_line=end_line,
     )
+    return out
 
 
 def struct_from_stack(stack: list, main_types: list, skip_types: list = None) -> dict:
     """Build a dictionary of all structures"""
     # Build nested structure
     struct = {}
     if skip_types is None:
         skip_types = []
 
     path_to_skip = []
-    for type_, name, path, *_ in stack:
-        if type_ in skip_types:
-            path_to_skip.append(path)
-
-    for (
-        type_,
-        name,
-        path,
-        start_line_idx,
-        start_statement_idx,
-        start_line,
-        end_line_idx,
-        end_statement_idx,
-        end_line,
-    ) in stack:
-        # logger.warning(path)
-        # logger.warning(path_to_skip)
-        cleaned_path = path_clean(path, path_to_skip)
-        # logger.warning(cleaned_path)
-        if type_ in main_types:
+    for stack_item in stack:
+        if stack_item.type_ in skip_types:
+            path_to_skip.append(stack_item.path)
+
+    for stack_item in stack:
+        cleaned_path = path_clean(stack_item.path, path_to_skip)
+        if stack_item.type_ in main_types:
+            #logger.warning(f"Adding {list2pathref(cleaned_path)}")
             struct[list2pathref(cleaned_path)] = {
                 "path": cleaned_path,
-                "name": name,
-                "type": type_,
-                "linestart": start_line,
-                "lines": [start_line_idx, end_line_idx],
-                "statements": [start_statement_idx, end_statement_idx], #Warning: here statements starts at 1!!!
-                "contains": [],
+                "name": stack_item.name,
+                "type": stack_item.type_,
+                "linestart": stack_item.start_line,
+                "lines": [stack_item.start_line_idx, stack_item.end_line_idx],
+                "statements": [stack_item.start_statement_idx, stack_item.end_statement_idx], #Warning: here statements starts at 1!!!
+                "contains": stack_item.contains,
+                "parents":stack_item.parents,
+                "callables":stack_item.callables,
                 "annotations":{},
             }
 
     return struct
 
 
 def get_struct_sizes(struct: dict) -> dict:
     """Compute the size of strict items (statefull)"""
     struct_aspects = {}
     for part, data in struct.items():
         struct_aspects[part] = {}
         struct_aspects[part]["NLOC"] = data["lines"][-1] - data["lines"][0] + 1
         struct_aspects[part]["ssize"] = data["statements"][-1] - data["statements"][0]
-        struct_aspects[part]["callables"] = []
         struct_aspects[part]["CCN"] = []
     return struct_aspects
 
 
 
 def replace_self(list_:list, parent:str)->list:
     """Replace the self keyword in a parentality path"""
@@ -267,31 +298,31 @@
         if len(data["path"]) > 1:
             parent = data["path"][:-1]
             try:
                 struct[list2pathref(parent)]["contains"].append(list2pathref(path))
             except KeyError:
                 pass
                 #will happen for scripts, with "dummy" not always referenced.
-            struct[part]["parent"]=list2pathref(parent)
-        else:
-            struct[part]["parent"]=None
+            #struct[part]["parents"].append(list2pathref(parent))
+        # else:
+        #     struct[part]["parent"]=None
 
     # add language specific analyses
     for part, data in struct.items():
         actual_lines=struct_actual_lines(struct,part)
         sub_code = [clean_code[i] for i in actual_lines]
         # logger.critical(part)
         # for i,line in enumerate(clean_code):
         #     if i  in actual_lines:
         #         logger.success(line)
         #     else:
         #         logger.warning(line)
-        data["callables"] = find_callables(sub_code)
-        if struct[part]["parent"] is not None:
-            data["callables"] = replace_self(data["callables"],struct[part]["parent"])
+        data["callables"].extend(find_callables(sub_code))
+        if struct[part]["parents"]:
+            data["callables"] = replace_self(data["callables"],struct[part]["parents"][0])
         if struct[part]["type"] in ["class"]:
             data["contains"] = replace_self(data["contains"],part)
             data["callables"] = replace_self(data["callables"],part)
 
         data["CCN"] = compute_ccn(sub_code)
 
     return struct
```

### Comparing `tucan-0.1.0/src/tucan/struct_main.py` & `tucan-0.2.0/src/tucan/struct_main.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 from tucan.unformat_py import unformat_py
 from tucan.unformat_ftn import unformat_ftn
 from tucan.unformat_c import unformat_c
 from tucan.struct_py import extract_struct_py
 from tucan.struct_ftn import extract_struct_ftn
 from tucan.struct_c import extract_struct_c
+from tucan.clean_ifdef import remove_ifdef_from_module
 
 
-def struct_main(filename: str) -> dict:
+def struct_main(filename: str, verbose:bool=False) -> dict:
     """
     Extract structure of a fortran or python file.
     - Find the nested structures of a code
     - Find the callables in each structure
     - Evaluate sizes, CCN
 
     Args:
@@ -31,23 +32,25 @@
         return {}
 
     code = [line.lower() for line in code]  # Lower case for all
 
     if filename.lower().endswith(".py"):
         logger.debug(f"Python code detected ...")
         statements = unformat_py(code)
-        struct_ = extract_struct_py(statements)
+        struct_ = extract_struct_py(statements, verbose)
     elif filename.lower().endswith((".f", ".F", ".f77", ".f90")):
         logger.debug(f"Fortran code detected ...")
+        code = remove_ifdef_from_module(code , [], verbose=False, fortran=True)
         statements = unformat_ftn(code)
-        struct_ = extract_struct_ftn(statements)
-    elif filename.lower().endswith((".c", ".cpp", ".cc")):
+        struct_ = extract_struct_ftn(statements,verbose)
+    elif filename.lower().endswith((".c", ".cpp", ".cc", ".h", ".hpp")):
         logger.debug(f"C/C++ code detected ...")
+        code = remove_ifdef_from_module(code , [], verbose=False)
         statements = unformat_c(code)
-        struct_ = extract_struct_c(statements)
+        struct_ = extract_struct_c(statements, verbose)
     else:
         ext = filename.lower().split(".")[-1]
         logger.error(f"Extension {ext} not supported, exiting ...")
         return {}
 
     return struct_
```

### Comparing `tucan-0.1.0/src/tucan/struct_py.py` & `tucan-0.2.0/src/tucan/struct_py.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import re
 from typing import Tuple
 from loguru import logger
 from tucan.unformat_common import Statements
 from tucan.struct_common import (
     find_words_before_left_parenthesis,
-    buffer_item,
-    stack_item,
+    new_buffer_item,
+    new_stack_item,
     struct_from_stack,
     struct_augment,
+    list2pathref,
 )
 from tucan.kw_lang import KEYWORDS_PY
 
 
-def extract_struct_py(statements: Statements) -> dict:
+def extract_struct_py(statements: Statements, verbose:bool) -> dict:
     """Main calls to build structure form statements
 
     statements is the output of tucan.unformat_py.unformat_py
     """
-
+    # TODO: verbose not supported for python
     clean_code = statements.to_code()
     all_structs = _extract_on_cleaned_py(statements)
     all_structs = struct_augment(all_structs,clean_code,find_callables_py,compute_ccn_approx_py)
+    for part, data in all_structs.items():
+        if data["type"]=="class":
+           data["parents"].extend(find_class_inheritance(data["linestart"]))
     return all_structs
 
 
 def _extract_on_cleaned_py(stmts: Statements) -> dict:
     """Extract structure from cleaned statements."""
     buffer = []
     stack = []
@@ -50,59 +54,68 @@
                     f"Multiple indent at {path} for '{line}' with last indent : {last_indent} and current : {indent}"
                 )
                 indent = last_indent + 1
             type_, name = parse_name_py(last_line)
 
             path.append(name)
             buffer.append(
-                buffer_item(
+                new_buffer_item(
                     type_=type_,
+                    path=path,
                     name=name,
                     first_line=last_line,
                     line_idx=last_idx,
                     statement_idx=stat_idx,
                 )
             )
             last_line = line
             last_idx = line_idx2
             last_indent = indent
             continue
 
         elif indent < last_indent:
             for _ in range(last_indent - indent):
-                (type_, name, first_line, line_idx, statement_idx) = buffer[-1]
+                last_buff = buffer[-1]
                 stack.append(
-                    stack_item(
-                        type_=type_,
-                        name=name,
-                        path=path.copy(),
-                        start_line_idx=line_idx,
-                        start_statement_idx=statement_idx,
-                        start_line=first_line,
-                        end_line_idx=last_idx,
-                        end_statement_idx=stat_idx,
-                        end_line=line,
-                    )
+                    new_stack_item(last_buff,last_idx, stat_idx,line)
                 )
                 path.pop(-1)
                 buffer.pop(-1)
             last_line = line
             last_indent = indent
             last_idx = line_idx1
             continue
 
         last_line = line
         last_indent = indent
         last_idx = line_idx1
 
-    return struct_from_stack(
+    struct = struct_from_stack(
         stack, main_types=["def", "class"], skip_types=["if", "for"]
     )
 
 
+    struct=explicit_methods(struct)
+
+    return struct
+
+
+def explicit_methods(struct:dict):
+    """prepend names of methods by their classes name"""
+    for part, data in struct.items():
+        path=data["path"]
+        if len(path)>1:
+            father_part=list2pathref(path[:-1])
+            if father_part in struct:
+                if struct[father_part]["type"]=="class":
+                    data["name"]=      struct[father_part]["name"]+"."+data["name"]      
+    return struct
+
+
+
 def parse_name_py(line: str) -> Tuple[str, str]:
     """expect a lowercase stripped line
     takes the second word as the name
     """
     type_ = line.strip().split()[0]
 
     try:
@@ -131,14 +144,26 @@
     id2 = line.rfind(')')
     out={}
     for arg in line[id1+1: id2].split(","):
         if ":" in arg:
             arg,type_=arg.split("=")[0].split(":")
             out[arg]=type_
     return out
-            
 
+def find_class_inheritance(line:str) -> list:
+    """Find the potential inheritance in a class"""
+    id1 = line.find('(')
+    id2 = line.rfind(')')
+    
+    out = line[id1+1: id2]
+    if "," in out:
+        return [item.strip() for item in out.split(",")]
+    elif len(out) == 0:
+        return []
+    else:
+        return out.strip()
+   
 def compute_ccn_approx_py(code: list) -> int:
     """Count decision points (if, else if, do, select, etc.)"""
     decision_points = re.findall(r"(?i)(if |elif|for|try|except )", "\n".join(code))
     complexity = len(decision_points) + 1
     return complexity
```

### Comparing `tucan-0.1.0/src/tucan/unformat_c.py` & `tucan-0.2.0/src/tucan/unformat_c.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         if stmt is None:
             stmt = line.rstrip()
             istart = lstart
         else:
             stmt += " "+line.strip()
 
-        if stmt.endswith(";") or (stmt.endswith("}") and level==0):
+        if stmt.endswith(";") or stmt.endswith("}"):# and level==0):
             new_stmt.append(stmt)
             new_lines.append([istart, lend])
             stmt=None
         
        
     if stmt is not None and stmt.strip() != "":
         logger.warning(f"Last statement not finished by ; \n {stmt}")
@@ -156,13 +156,13 @@
     stmts.stmt = remove_strings(stmts.stmt, '"')
     stmts.stmt = remove_strings(stmts.stmt, "'")
     stmts = align_multiline_blocks(stmts, "/*", "*/")
     stmts = clean_inline_comments(stmts, "/*") # this ine must follow the align multiline block
     stmts = clean_inline_comments(stmts, "//")
     stmts = clean_blanks(stmts)                # this one must follow the clean inline, to remove blank lines
     stmts = align_unfinished_lines(stmts)
-    stmts = split_multiple_statements(stmts)
+    #stmts = split_multiple_statements(stmts)
     stmts = split_declarations(stmts)
     
     #stmts = remove_space_in_front_of_variables(stmts)
 
     return stmts
```

### Comparing `tucan-0.1.0/src/tucan/unformat_common.py` & `tucan-0.2.0/src/tucan/unformat_common.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 from __future__ import annotations
 from typing import Tuple,List
 from dataclasses import dataclass
 from loguru import logger
 import json
 
+CHAR_CMT_START = "\xaa"
+CHAR_CMT_STOP = "\xbb"
+CHAR_EOL = "\xcc"
+CHAR_CMT_EOL = "\xdd"
 
 @dataclass
 class Statements():
     stmt:List[str]= None
     lines:List[Tuple[int,int]]= None
 
     def __str__(self):
@@ -247,8 +251,45 @@
     for char in line:
         if char == "\t":
             _indent+="    "
         elif char != " ":
             break
         else:
             _indent+=" "
-    return _indent
+    return _indent
+
+
+
+def strip_c_comment(line:str, fortran:bool=False)->str:
+    """
+    Fortran=True :  equivalent to cpp --traditional
+    """
+    cline=""
+    read=True
+    _line =line.replace("//", CHAR_CMT_EOL).replace("/*", CHAR_CMT_START).replace("*/",CHAR_CMT_STOP)
+    for char in _line:
+        if char == CHAR_EOL:
+            cline+=char
+            if read==None:
+                read=True
+        elif char == CHAR_CMT_START and read is not None:
+            read=False                 # Read False if multiline Comment
+        elif char == CHAR_CMT_STOP and read is not None:
+            read=True
+        elif char == CHAR_CMT_EOL and read is True:
+            if not fortran:
+                read=None         # Read None if single line comment
+            else:
+                cline+=char        # Skipp this in Fortran            
+        else:
+            if read is True :
+                cline+=char
+    
+    cline = cline.replace(CHAR_CMT_EOL,"//")
+    return cline
+
+
+def clean_c_comments(lines:List[str],fortran:bool=False)->List[str]:    
+    raw = CHAR_EOL.join(lines)
+    out = strip_c_comment(raw,fortran=fortran).split(CHAR_EOL)
+    assert len(lines) == len(out)
+    return out
```

### Comparing `tucan-0.1.0/src/tucan/unformat_ftn.py` & `tucan-0.2.0/src/tucan/unformat_ftn.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,17 @@
     for line, (lstart, lend) in zip(stmts.stmt, stmts.lines):
         if line.lstrip().startswith("&"):
             new_stmt[-1] = last_line.rstrip("&") + " " + line.strip()[1:]
             new_lines[-1][1] = lend
         elif line.lstrip().startswith("$"):
             new_stmt[-1] = last_line.rstrip("$") + " " + line.strip()[1:]
             new_lines[-1][1] = lend
+        elif line.startswith("     +"):
+            new_stmt[-1] = last_line.rstrip("     +") + " " + line.strip()[1:]
+            new_lines[-1][1] = lend
         else:
             new_stmt.append(line)
             new_lines.append([lstart, lend])
 
         last_line = new_stmt[-1]
     return Statements(new_stmt, new_lines)
 
@@ -77,27 +80,16 @@
      becomes
     15 FORMAT(' TRANFT:  Transport property fitting,',' CHEMKIN-II Version ',A,', August 1994','DOUBLE PRECISION') 
     
     """
     new_stmt = []
     new_lines = []
     for line, (lstart, lend) in zip(stmts.stmt, stmts.lines):
-        
-        buffer=""
-        for char in line:
-            if char != " " and not char.isdigit():
-                break
-            buffer+= char
-
-        if len(buffer.strip()) == 1 :
-            #logger.critical(str(lstart)+":"+line)
-            reach = len(buffer)
-            new_stmt[-1] += line[reach:]
-            #logger.critical("adding:"+line[reach:])
-            
+        if line[0:5]=="     " and (line[5] in "0123456789*"):
+            new_stmt[-1]+=line[7:]
             new_lines[-1][1] = lend
         else:
             new_stmt.append(line)
             new_lines.append([lstart, lend])
 
     return Statements(new_stmt, new_lines)
 
@@ -129,22 +121,14 @@
             #logger.critical(str(splitted_parts))
             indent = get_indent(line)
             new_stmt.append(splitted_parts[0]+ " then")
             new_lines.append([lstart, lend])
             new_stmt.append(indent + "   "+ splitted_parts[-1])
             new_lines.append([lstart, lend])
             new_stmt.append(indent + "end if")
-            # elif "goto" in line:
-            #     splitted_parts = split_oneliner(line)
-            #     indent = get_indent(line)
-            #     new_stmt.append(splitted_parts[0])
-            #     new_lines.append([lstart, lend])
-            #     new_stmt.append(indent + "end if")
-            # else:
-            #     new_stmt.append(line)
 
         elif line.strip().startswith("where "):
             splitted_parts = split_oneliner(line)
 
             if not splitted_parts[-1]:
                 new_stmt.append(line)
                 new_lines.append([lstart, lend])
@@ -308,152 +292,152 @@
     """ Move modern labels at the end of the line 
     
      We keep label to show the name in struct
     """
     new_stmt = []
    
     def _move_labels(line:str, pattern:str="do", sep:str=":")->str:
-        if (sep+pattern+" " in line 
-            or sep+" "+pattern+" " in line
-            or sep+pattern+"(" in line
-            or sep+" "+pattern+"(" in line
-            
-        ):
+        """
+        eigenvalues: block
+
+        becomes block ! NESTING_LABEL# eigenvalues
+        """
+        if pattern not in line or sep not in line:
+            return line
+
+        rhs = line.split(sep)[1].rstrip()
+        rhs1=""
+        for char in rhs:
+            if char in " (":
+                break
+            rhs1+=char
+        
+        if rhs1==pattern:
+
             label = line.split(sep)[0].strip()
             index=line.find(sep)
-            line = get_indent(line)+line[index+1:].rstrip()+ " #LABEL :"+label 
+            line = get_indent(line)+line[index+1:].rstrip()+ " ! NESTING_LABEL# "+label
         return line
 
     for line in lines:
         
         line = _move_labels(line, "block", ":")
         line = _move_labels(line, "do", ":")
         line = _move_labels(line, "if", ":")
         line = _move_labels(line, "entry", ":")
         line = _move_labels(line, "select_case", ":")
-        line = _move_labels(line, "if", "=")
+        new_stmt.append(line)
+       
+    return new_stmt
+
+def ftn_clean_operators(lines:List[str]) -> List[str]:
 
+    new_stmt = []
+    for line in lines:
+        line =line.replace("::", " :: ")
+        line =line.replace("==", ".eq.")
+        line =line.replace("/=", ".ne.")
+        line =line.replace(">=", ".ge.")
+        line =line.replace("<=", ".le.")
+        #line =line.replace("=", " = ")
         new_stmt.append(line)
        
     return new_stmt
 
 def ftn_clean_intrinsics_declarations(lines:List[str]) -> List[str]:
     """ clean oddities in fortran declarations"""
     new_stmt = []
    
-    def _move_labels(line:str, pattern:str="do", sep:str=":")->str:
-        if (sep+pattern+" " in line 
-            or sep+" "+pattern+" " in line
-            or sep+pattern+"(" in line
-            or sep+" "+pattern+"(" in line
-            
-        ):
-            label = line.split(sep)[0].strip()
-            index=line.find(sep)
-            line = get_indent(line)+line[index+1:].rstrip()+ " #LABEL :"+label
+    def _remove_decorators(line:str, keyword:str)->str:
+        """usual cleanup before fortran structures:
+        - check ends
+        - put decorators at the back
+        """
+        if keyword not in line:
+            return line
+        
+        if line.lstrip().startswith("end"):
+            line.replace("end"+keyword,"end "+keyword )
+            return line
+        
+
+        line_no_par = line.replace("("," ").replace(")"," ")+ " " # Here we add " " to make sure a keyword last on the line still trigger (" "+keyword+" ") for the replacement
+        idx = line_no_par.find(" "+keyword+" ")
+        if idx == -1:
+            return line
+        
+        line = (get_indent(line) 
+                + line[idx+1:]
+                + " ! "+keyword.upper() +"# "+line[:idx+1].lstrip())
         return line
-
     for line in lines:
-        line =line.replace("pure function", "function_pure ")
-        line =line.replace("elemental function", "function_elemental ")
-        line =line.replace("recursive function", "function_recursive ")
-        
-        line =line.replace("double precision function", "function ") 
-        line =line.replace("real function", "function ") 
-        line =line.replace("integer function", "function ")
-        line =line.replace("logical function", "function ")
-        
-
-        line =line.replace("selectcase", "select_case ")
-        line =line.replace("select case", "select_case ")
-        line =line.replace("select type", "select_type ")
-        
-        line =line.replace("elemental subroutine", "subroutine_elemental ")
-        line =line.replace("recursive subroutine", "subroutine_recursive ")
-        
-        line =line.replace("module procedure", "module_procedure ")
-        
 
+        # merge multiple words
         line =line.replace("double precision", "double_precision ")
-        
+        line =line.replace("module procedure", "module_procedure ")
         line =line.replace("type,public,abstract", "type_public_abstract ")
         line =line.replace("type,public", "type_public ")
         line =line.replace("type,private,abstract", "type_private_abstract ")
         line =line.replace("type,private", "type_private ")
+        line =line.replace("type is", "type_is ")
+        line =line.replace("selectcase", "select_case ")
+        line =line.replace("select case", "select_case ")
+        line =line.replace("select type", "select_type ")
         
-        line =line.replace("interface", "interface ")
-        line =line.replace("abstract interface", "interface_abstract ")
         
+        line = _remove_decorators(line, "function")
+        line = _remove_decorators(line, "subroutine")
+        line = _remove_decorators(line, "interface")
+
+
         line =line.replace("enddo", "end do ")
         line =line.replace("endif", "end if ")       # Important to add supp. spacing , incase of a following elmt.
         line =line.replace("endwhere", "end where ")
         line =line.replace("endmodule", "end module ")       # Important to add supp. spacing , incase of a following elmt.
-
-        line =line.replace("associate(", "associate (")
-        line =line.replace("if(", "if (")
-        line =line.replace("do(", "do (")
-        line =line.replace("type(", "type (")
-        line =line.replace("type is", "type_is ")
         
+        # slpit left parenthesis - and right ...
+        for keyword in [
+                "function",
+                "subroutine",
+                "interface",
+                "if",
+                "do",
+                "type",
+                "associate"
+            ]:
+            line=line.replace(f"{keyword}(",f"{keyword} (")
+
         line =line.replace(")then", ") then ")
         
-        line =line.replace("::", " :: ")
-        line =line.replace("=", " = ")
-        
-        line = _move_labels(line, "block", ":")
-        line = _move_labels(line, "do", ":")
-        line = _move_labels(line, "if", ":")
-        line = _move_labels(line, "entry", ":")
-        line = _move_labels(line, "select_case", ":")
-        line = _move_labels(line, "if", "=")
-
         new_stmt.append(line)
        
     return new_stmt
 
 
-def ftn_old_fix_end_multiline(lines:List[str])->List[str]:
-    """Fix end parenthesis of multilines
-    eg in tranfit.f:
-       20 FORMAT (/,' DATA HAS BEEN FIT OVER THE RANGE:  TLOW=',F9.2,
-     1        ', THIGH=',F9.2)
-    last ) should be a /)
-    """
+def ftn_clean_type_keywords(lines:List[str]) -> List[str]:
+    """ Replace  type( declarations by _type("""
     
-    markup_left = "(/"
-    markup_right = "/)"
-    proxy_left="\xaa"
-    proxy_right="\xbb"
-    
-    #lines_rep=[ line.replace(markup_left,proxy_left).replace(markup_right,proxy_right) for line in lines]
-
-    # stack_par=0
-    # lines_clean=[]
-    # for line in lines_rep:
-    #     buffer=""
-    #     for char in line:
-    #         if char == "(":
-    #             stack_par +=1
-    #         if char == ")":
-    #             stack_par -=1
-            
-    #         if stack_par == -1:
-    #             #logger.warning(f"Loosy end : {line}")
-    #             buffer += proxy_right
-    #             #logger.warning(f"Loosy end : {buffer}")
-    #             stack_par = 0
-    #         else: 
-    #             buffer+=char
-
-    #     lines_clean.append(buffer)
-                
-    # #lines_out=[ line.replace(proxy_left,markup_left).replace(proxy_right,markup_right) for line in lines_clean]
-
+    def _clean_type(line:str)-> str:
+        if line.replace(" ","")[4]=="(":         #for type(bcdhjzks)
+            return line.replace("type","_type",1)
+        elif line.replace(" ","")[4:6]=="is":    #for select type ; type is
+            return line.replace("type is","#typeis",1)
+        elif line.replace(" ","")[4] in " azertyuiopqsdfghjklmwxcvbn":        #well formed keyword
+            return line
+        elif line.replace(" ","")[4]==",":  
+            return line.replace("type","type ",1)   #for  type, extend (need the space to identify the end of keyword)
+        else:
+            return line
+    new_stmt=[]
+    for line in lines:
+        if line.lstrip().startswith("type"):
+            line = _clean_type(line)
             
-    return lines #lines_rep #clean
+        new_stmt.append(line)    
+    return new_stmt
 
 
 def unformat_ftn(code: List[str]) -> Statements:
     """
     Unformat Fortran code by stripping comments and moving leading '&' characters.
 
     Args:
@@ -474,19 +458,21 @@
 
     stmts = clean_inline_comments(stmts, "!")
     
     stmts = clean_blanks(stmts)
     stmts = align_end_continuations(stmts)
     stmts = align_start_continuations(stmts)
     stmts = ftn_align_labelled_continuations(stmts)
-    
-    stmts.stmt = ftn_old_fix_end_multiline(stmts.stmt)  # Necessary because fortran is verrry lenient !
     stmts = align_multiline_blocks(stmts, "(/", "/)")
+    
+    stmts.stmt = ftn_clean_operators(stmts.stmt) 
     stmts = split_multi_statement_lines(stmts)
-
+    
+    #stmts.stmt = ftn_clean_type_declarations(stmts.stmt) # not sure we need this now
+    stmts.stmt = ftn_clean_type_keywords(stmts.stmt)
     stmts.stmt = ftn_clean_intrinsics_declarations(stmts.stmt)
     stmts = ftn_clean_labelled_loops_oldftn(stmts)
     stmts.stmt = ftn_clean_labelled_loops_newftn(stmts.stmt)
 
     stmts.stmt = ftn_suppress_goto_references(stmts.stmt)   # !!After ftn_clean_labelled_loops_oldftn, or you cannot end loops
     stmts = ftn_make_oneliners_conditionals_multilines(stmts)
     stmts.stmt = ftn_remove_space_in_front_of_variables(stmts.stmt)
```

### Comparing `tucan-0.1.0/src/tucan/unformat_main.py` & `tucan-0.2.0/src/tucan/unformat_main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Global function to handle the unformat of various languages"""
 from loguru import logger
 
 from tucan.unformat_py import unformat_py
 from tucan.unformat_ftn import unformat_ftn
 from tucan.unformat_c import unformat_c
+from tucan.clean_ifdef import remove_ifdef_from_module
 
 
-def unformat_main(filename: str) -> list:
+def unformat_main(filename: str,verbose:bool=False) -> list:
     """
     Main function to call to get an unformated version of the code
 
     Args:
         filename (str): _description_
 
     Returns:
@@ -22,17 +23,19 @@
     code = [line.lower() for line in code]  # Lower case for all
 
     if filename.lower().endswith(".py"):
         logger.debug(f"Python code detected ...")
         statements = unformat_py(code)
     elif filename.lower().endswith((".f", ".F", ".f77", ".f90")):
         logger.debug(f"Fortran code detected ...")
+        code = remove_ifdef_from_module(code , [], verbose, fortran=True)
         statements = unformat_ftn(code)
-    elif filename.lower().endswith((".c", ".cpp", ".cc")):
+    elif filename.lower().endswith((".c", ".cpp", ".cc", ".h")):
         logger.debug(f"C/C++ code detected ...")
+        code = remove_ifdef_from_module(code , [], verbose)
         statements = unformat_c(code)
     else:
         ext = filename.lower().split(".")[-1]
         logger.error(f"Extension {ext} not supported, exiting ...")
         statements = []
 
     return statements
```

### Comparing `tucan-0.1.0/src/tucan/unformat_py.py` & `tucan-0.2.0/src/tucan/unformat_py.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,22 @@
         if not inside_block_context:
             new_stmt.append(indent+buffer)
             new_lines.append([this_start, lend])
             buffer=""
 
     return Statements(new_stmt,new_lines)  
 
+def replace_keywords(code:List[str])->List[str]:
+    """replace some uneasy keywords for parsing"""
+    new_stmt=[]
 
+    for line in code:
+        new_line=line.replace("super()", "self_super")
+        new_stmt.append(new_line)
+    return new_stmt
 
 def split_fstrings(code:List[str], fstring_char:str, other_char:str)->List[str]:
     new_stmt=[]
 
     for line in code:
         inside_fstring_context=False
         #inside_escape_context=False
@@ -193,10 +200,10 @@
     stmts.stmt = remove_strings(stmts.stmt,"'")
     stmts.stmt = remove_strings(stmts.stmt,'"')
     
     stmts = clean_inline_comments(stmts,"#") 
     stmts = clean_blanks(stmts)
     stmts = split_multi_statement_lines(stmts)
     stmts = align_context_block(stmts)
-    
+    stmts.stmt = replace_keywords(stmts.stmt)
     stmts.stmt = getback_combined_chars(stmts.stmt)
     return stmts
```

### Comparing `tucan-0.1.0/src/tucan.egg-info/PKG-INFO` & `tucan-0.2.0/src/tucan.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tucan
-Version: 0.1.0
+Version: 0.2.0
 Summary: Unformatter Tool to allow parsing and analysis of code base.
 Home-page: https://gitlab.com/cerfacs/tucan
 Author: Antoine Dauptain, Thibault Marzlin, CoopTeam-CERFACS
 Author-email: coop@cerfacs.fr
 Project-URL: Homepage, https://gitlab.com/cerfacs/tucan
 Project-URL: Documentation, https://tucan.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.com/cerfacs/tucan/-/issues
@@ -17,26 +17,38 @@
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 ![tucan](https://images.unsplash.com/photo-1611788542170-38cf842212f4?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)
 
-TUCAN (Tool to Unformat, Clean, ands Analyse) is a code parser for scientific codebases. It tager languages are:
+TUCAN (Tool to Unformat, Clean, and Analyse) is a code parser for scientific codebases. Its target languages are:
+
 - Very old FORTRAN
 - Recent FORTRAN
 - Python (Under development)
-- C/C++ (Eazrly development)
+- C/C++ (Early development)
+
+## Installation
+
+You can instal it from [PyPI](https://pypi.org/project/tucan/) with:
+
+```bash
+pip install tucan
+```
+
+You can also install from the sources from one of our [gitlab mirrors](https://codehub.hlrs.de/coes/excellerat-p2/uc-2/tucan).
+
 
 ## What is does?
 
 
-### Remove Coding archaisms
+### Remove coding archaisms
 
-First is it a code cleaner. For example, this loop in `tranfit.f' a piece of CHEMKIN package  good'old FORTRAN:
+First it is a code cleaner. For example, this loop in `tranfit.f', a piece of [CHEMKIN](https://en.wikipedia.org/wiki/CHEMKIN) II package  in good'old FORTRAN77. (Do not worry, recent Chemkin is not written that way, probably)  :
 
 ```fortran
 (547)      DO 2000 K = 1, KK-1
 (548)         DO 2000 J = K+1, KK
 (549)            DO 2000 N = 1, NO
 (550)               COFD(N,J,K) = COFD(N,K,J)
 (551) 2000 CONTINUE
@@ -50,23 +62,26 @@
 (550-550)                 cofd(n,j,k)  =  cofd(n,k,j)
 (551-551)              end do ! 2000
 (551-551)           end do ! 2000
 (551-551)        end do ! 2000
 ```
 
 
-
-The cleaned version simplify the code for further analysis passes, like computing cyclomatic complexity, extracting structures, etc...
+The cleaned version is a simpler code for further analysis passes, like computing cyclomatic complexity, extracting structures, etc...
 
 
 ### Extracting code structure
 
-On the same file `tucan struct tranfit.f` provides a nested dictionary of the code structure. Here is an exemple from a code in very recent fortran:
+
+Here we start from a file of [neko](https://github.com/ExtremeFLOW/neko/blob/develop/src/adt/htable.f90), an HPC code in recent Fortran, finalist for the Gordon Bell Prize in 2023.
+
+`tucan struct htable.f90` provides a nested dictionary of the code structure. Here is a part of the output:
 
 ```yaml
+(...)
 type htable.h_tuple_t :
     At path ['htable', 'h_tuple_t'], name h_tuple_t, lines 47 -> 52
     6 statements over 6 lines
     Complexity 1
     Refers to 1 callables:
        - class
     Contains no inner structures
@@ -96,22 +111,25 @@
     At path ['htable', 'interface_abstract66'], name interface_abstract66, lines 66 -> 73
     8 statements over 8 lines
     Complexity 1
     Contains no callables
     Contains 1 elements:
     - htable.interface_abstract66.htable_hash
     Contains no annotations
+(...)
 ```
 
+*(This output will change as we update and improve tucan in the next versions!)*
+
 This information allows the creation and manipulation of graphs to extract the structure of the code
 
 
-### Interpreting IFDEFS 
+### Interpreting Conditional Inclusions "IF DEFS". 
 
-An other nasty example is the use of ìfdefs in C or FORTRAN:
+An other example of tucan is the analysis of [ifdefs](https://en.cppreference.com/w/c/preprocessor/conditional) in C or FORTRAN:
 
 ```
 #ifdef FRONT
         WRITE(*,*) " FRONT is enabled " ! partial front subroutine
         SUBROUTINE dummy_front(a,b,c)
         WRITE(*,*) " FRONT 1"     ! partial front subroutine
 #else                
@@ -178,11 +196,36 @@
 
         SUBROUTINE dummy_back(a,b,c)
         WRITE(*,*) " BACK is enabled " ! partial front subroutine
         WRITE(*,*) " BACK 1"    ! partial back subroutine
         END SUBROUTINE
 ```
 
+#### scanning ifdef variables
+
+A simpler usage of tucan : scan the current ifdefs variables. Still on [neko](https://github.com/ExtremeFLOW/neko) in the `/src` folder (an old version though) : 
+
+```bash
+/neko/src >tucan ifdef-scan-pkge .
+ - Recursive path gathering ...
+ - Cleaning the paths ...
+ - Analysis completed.
+ - Global ifdef variables : HAVE_PARMETIS, __APPLE__
+ - Local to device/opencl/check.c : CL_ERR_STR(err)
+ - Local to math/bcknd/device/opencl/opr_opgrad.c : CASE(LX), STR(X)
+ - Local to math/bcknd/device/opencl/opr_dudxyz.c : CASE(LX), STR(X)
+ - Local to common/sighdl.c : SIGHDL_ALRM, SIGHDL_USR1, SIGHDL_USR2, SIGHDL_XCPU
+ - Local to math/bcknd/device/opencl/opr_conv1.c : CASE(LX), STR(X)
+ - Local to math/bcknd/device/opencl/opr_cfl.c : CASE(LX), STR(X)
+ - Local to krylov/bcknd/device/opencl/pc_jacobi.c : CASE(LX), STR(X)
+ - Local to math/bcknd/device/opencl/ax_helm.c : CASE(LX), STR(X)
+ - Local to bc/bcknd/device/opencl/symmetry.c : MAX(a,
+ - Local to gs/bcknd/device/opencl/gs.c : GS_OP_ADD, GS_OP_MAX, GS_OP_MIN, GS_OP_MUL
+ - Local to sem/bcknd/device/opencl/coef.c : DXYZDRST_CASE(LX), GEO_CASE(LX), STR(X)
+ - Local to math/bcknd/device/opencl/opr_cdtp.c : CASE(LX), STR(X)
+```
+This feature is useful to see all potential variables that surcharge your codebase via conditional inclusions.
+
 ## More about tucan
 
 `Tucan` is used by  `anubis`, our open-source  tool to explore the git repository of a code, and `marauder's map`  our open-source tool to show codes structures by in-depth vizualisation of callgraphs and code circular-packing .
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tucan-0.1.0/src/tucan.egg-info/SOURCES.txt` & `tucan-0.2.0/src/tucan.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 README.md
 setup.cfg
 setup.py
 src/.DS_Store
 src/tucan/__init__.py
 src/tucan/clean_ifdef.py
 src/tucan/cli.py
+src/tucan/guess_language.py
+src/tucan/imports_c.py
 src/tucan/imports_common.py
 src/tucan/imports_ftn.py
 src/tucan/imports_main.py
 src/tucan/imports_py.py
 src/tucan/kw_lang.py
 src/tucan/package_analysis.py
 src/tucan/struct_c.py
@@ -28,14 +30,15 @@
 src/tucan.egg-info/dependency_links.txt
 src/tucan.egg-info/entry_points.txt
 src/tucan.egg-info/requires.txt
 src/tucan.egg-info/top_level.txt
 src/tucan/__pycache__/__init__.cpython-311.pyc
 src/tucan/__pycache__/clean_ifdef.cpython-311.pyc
 src/tucan/__pycache__/cli.cpython-311.pyc
+src/tucan/__pycache__/imports_c.cpython-311.pyc
 src/tucan/__pycache__/imports_ftn.cpython-311.pyc
 src/tucan/__pycache__/imports_main.cpython-311.pyc
 src/tucan/__pycache__/imports_py.cpython-311.pyc
 src/tucan/__pycache__/kw_lang.cpython-311.pyc
 src/tucan/__pycache__/package_analysis.cpython-311.pyc
 src/tucan/__pycache__/struct_c.cpython-311.pyc
 src/tucan/__pycache__/struct_common.cpython-311.pyc
```

