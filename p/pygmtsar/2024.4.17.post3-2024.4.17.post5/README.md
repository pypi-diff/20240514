# Comparing `tmp/pygmtsar-2024.4.17.post3.tar.gz` & `tmp/pygmtsar-2024.4.17.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtsar-2024.4.17.post3.tar", last modified: Thu May  9 08:12:10 2024, max compression
+gzip compressed data, was "pygmtsar-2024.4.17.post5.tar", last modified: Tue May 14 19:44:00 2024, max compression
```

## Comparing `pygmtsar-2024.4.17.post3.tar` & `pygmtsar-2024.4.17.post5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-09 08:12:10.448568 pygmtsar-2024.4.17.post3/
--rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17.post3/LICENSE.txt
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-09 08:12:10.448246 pygmtsar-2024.4.17.post3/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17.post3/README.md
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-09 08:12:10.446506 pygmtsar-2024.4.17.post3/pygmtsar/
--rw-r--r--   0 mbg        (501) staff       (20)    18153 2024-04-26 09:12:06.000000 pygmtsar-2024.4.17.post3/pygmtsar/ASF.py
--rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17.post3/pygmtsar/AWS.py
--rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17.post3/pygmtsar/GMT.py
--rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17.post3/pygmtsar/IO.py
--rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17.post3/pygmtsar/NCubeVTK.py
--rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17.post3/pygmtsar/PRM.py
--rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17.post3/pygmtsar/PRM_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17.post3/pygmtsar/S1.py
--rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack.py
--rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_align.py
--rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_base.py
--rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_dem.py
--rw-r--r--   0 mbg        (501) staff       (20)    44539 2024-05-08 11:23:30.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_detrend.py
--rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_export.py
--rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_geocode.py
--rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_incidence.py
--rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_landmask.py
--rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_multilooking.py
--rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_orbits.py
--rw-r--r--   0 mbg        (501) staff       (20)    47608 2024-05-07 07:53:29.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_phasediff.py
--rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_prm.py
--rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_ps.py
--rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_reframe.py
--rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_reframe_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    46858 2024-05-01 05:44:48.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_sbas.py
--rw-r--r--   0 mbg        (501) staff       (20)     9103 2024-04-26 15:00:33.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_stl.py
--rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_tidal.py
--rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_topo.py
--rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_trans.py
--rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_trans_inv.py
--rw-r--r--   0 mbg        (501) staff       (20)    27198 2024-04-28 10:15:51.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_unwrap.py
--rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_unwrap_snaphu.py
--rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17.post3/pygmtsar/Tiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.4.17.post3/pygmtsar/XYZTiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17.post3/pygmtsar/_Stack_merge.py
--rw-r--r--   0 mbg        (501) staff       (20)     1040 2024-05-08 11:26:31.000000 pygmtsar-2024.4.17.post3/pygmtsar/__init__.py
--rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17.post3/pygmtsar/datagrid.py
--rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17.post3/pygmtsar/tqdm_dask.py
--rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17.post3/pygmtsar/tqdm_joblib.py
--rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17.post3/pygmtsar/utils.py
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-09 08:12:10.447869 pygmtsar-2024.4.17.post3/pygmtsar.egg-info/
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-09 08:12:10.000000 pygmtsar-2024.4.17.post3/pygmtsar.egg-info/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-05-09 08:12:10.000000 pygmtsar-2024.4.17.post3/pygmtsar.egg-info/SOURCES.txt
--rw-r--r--   0 mbg        (501) staff       (20)        1 2024-05-09 08:12:10.000000 pygmtsar-2024.4.17.post3/pygmtsar.egg-info/dependency_links.txt
--rw-r--r--   0 mbg        (501) staff       (20)      330 2024-05-09 08:12:10.000000 pygmtsar-2024.4.17.post3/pygmtsar.egg-info/requires.txt
--rw-r--r--   0 mbg        (501) staff       (20)        9 2024-05-09 08:12:10.000000 pygmtsar-2024.4.17.post3/pygmtsar.egg-info/top_level.txt
--rw-r--r--   0 mbg        (501) staff       (20)       38 2024-05-09 08:12:10.448630 pygmtsar-2024.4.17.post3/setup.cfg
--rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-04-11 03:27:25.000000 pygmtsar-2024.4.17.post3/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-14 19:44:00.677231 pygmtsar-2024.4.17.post5/
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17.post5/LICENSE.txt
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-14 19:44:00.676901 pygmtsar-2024.4.17.post5/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17.post5/README.md
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-14 19:44:00.675332 pygmtsar-2024.4.17.post5/pygmtsar/
+-rw-r--r--   0 mbg        (501) staff       (20)    18153 2024-04-26 09:12:06.000000 pygmtsar-2024.4.17.post5/pygmtsar/ASF.py
+-rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17.post5/pygmtsar/AWS.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17.post5/pygmtsar/GMT.py
+-rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17.post5/pygmtsar/IO.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17.post5/pygmtsar/NCubeVTK.py
+-rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17.post5/pygmtsar/PRM.py
+-rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17.post5/pygmtsar/PRM_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17.post5/pygmtsar/S1.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack.py
+-rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_align.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_dem.py
+-rw-r--r--   0 mbg        (501) staff       (20)    44539 2024-05-08 11:23:30.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_detrend.py
+-rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_export.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_geocode.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_incidence.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_landmask.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_multilooking.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_orbits.py
+-rw-r--r--   0 mbg        (501) staff       (20)    47608 2024-05-07 07:53:29.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_phasediff.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_prm.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_ps.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_reframe.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_reframe_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    46915 2024-05-13 12:07:20.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_sbas.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9590 2024-05-14 18:56:19.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_stl.py
+-rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_tidal.py
+-rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_topo.py
+-rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_trans.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_trans_inv.py
+-rw-r--r--   0 mbg        (501) staff       (20)    27198 2024-04-28 10:15:51.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_unwrap.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17.post5/pygmtsar/Stack_unwrap_snaphu.py
+-rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17.post5/pygmtsar/Tiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10025 2024-05-14 05:42:17.000000 pygmtsar-2024.4.17.post5/pygmtsar/XYZTiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17.post5/pygmtsar/_Stack_merge.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1040 2024-05-14 19:43:23.000000 pygmtsar-2024.4.17.post5/pygmtsar/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17.post5/pygmtsar/datagrid.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17.post5/pygmtsar/tqdm_dask.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17.post5/pygmtsar/tqdm_joblib.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17.post5/pygmtsar/utils.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-14 19:44:00.676568 pygmtsar-2024.4.17.post5/pygmtsar.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-14 19:44:00.000000 pygmtsar-2024.4.17.post5/pygmtsar.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-05-14 19:44:00.000000 pygmtsar-2024.4.17.post5/pygmtsar.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2024-05-14 19:44:00.000000 pygmtsar-2024.4.17.post5/pygmtsar.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      330 2024-05-14 19:44:00.000000 pygmtsar-2024.4.17.post5/pygmtsar.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2024-05-14 19:44:00.000000 pygmtsar-2024.4.17.post5/pygmtsar.egg-info/top_level.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       38 2024-05-14 19:44:00.677284 pygmtsar-2024.4.17.post5/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-04-11 03:27:25.000000 pygmtsar-2024.4.17.post5/setup.py
```

### Comparing `pygmtsar-2024.4.17.post3/LICENSE.txt` & `pygmtsar-2024.4.17.post5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/PKG-INFO` & `pygmtsar-2024.4.17.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.4.17.post3
+Version: 2024.4.17.post5
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.4.17.post3/README.md` & `pygmtsar-2024.4.17.post5/README.md`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/ASF.py` & `pygmtsar-2024.4.17.post5/pygmtsar/ASF.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/AWS.py` & `pygmtsar-2024.4.17.post5/pygmtsar/AWS.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/GMT.py` & `pygmtsar-2024.4.17.post5/pygmtsar/GMT.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/IO.py` & `pygmtsar-2024.4.17.post5/pygmtsar/IO.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/NCubeVTK.py` & `pygmtsar-2024.4.17.post5/pygmtsar/NCubeVTK.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/PRM.py` & `pygmtsar-2024.4.17.post5/pygmtsar/PRM.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/PRM_gmtsar.py` & `pygmtsar-2024.4.17.post5/pygmtsar/PRM_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/S1.py` & `pygmtsar-2024.4.17.post5/pygmtsar/S1.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_align.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_align.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_base.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_base.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_dem.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_dem.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_detrend.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_detrend.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_export.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_export.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_geocode.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_geocode.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_incidence.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_incidence.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_landmask.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_landmask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_multilooking.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_multilooking.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_orbits.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_orbits.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_phasediff.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_phasediff.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_prm.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_prm.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_ps.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_ps.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_reframe.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_reframe.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_reframe_gmtsar.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_reframe_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_sbas.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_sbas.py`

 * *Files 0% similar despite different names*

```diff
@@ -752,15 +752,15 @@
         #print ('NOTE: this function is deprecated, use instead Stack.plot_baseline_attribute()')
         self.plot_baseline_attribute(baseline_pairs, pairs_best, column=column, caption='Baseline Deviation')
 
     def plot_baseline_displacement(self, phase, corr=None, caption=None, cmap='turbo',
                                    displacement=True, unwrap=True,
                                    stl=False, stl_freq='W', stl_periods=52, stl_robust=True,
                                    los=False, tolerance=np.pi/2, xlabel_rotation=45,
-                                   legend=True, legend_alpha=None):
+                                   legend=True, legend_alpha=None, linewidth=0.5):
         """
         Performs 1D unwrapping, linear regression, and STL on a given set of phase values.
     
         The linear regression model is represented as:
             y = β0 + β1 * x
     
         Where:
@@ -853,15 +853,15 @@
                 errors.append(row['phase'] - (end - start))
             else:
                 start = 0
             y_min = min(y_min, start, row['phase'] + start)
             y_max = max(y_max, start, row['phase'] + start)
             plt.plot([row['ref'], row['rep']], [start, row['phase'] + start],
                      c=colors(row['corr']) if corr is not None else 'grey', alpha=0.8,
-                     linewidth=0.5)
+                     linewidth=linewidth)
         #print ('errors', errors)
         #print ('y_min', y_min, 'y_max', y_max)
         if displacement or stl:
             errors = np.asarray(errors)
             #print ('errors', errors)
             weights = df['corr'].values
             nanmask = np.isnan(errors) | np.isnan(weights)
@@ -907,20 +907,20 @@
         if (displacement or stl) and legend:
             plt.legend(framealpha=legend_alpha)
 
     def plot_baseline_displacement_los_mm(self, phase, corr=None, caption=None, cmap='turbo',
                                    displacement=True, unwrap=True,
                                    stl=False, stl_freq='W', stl_periods=52, stl_robust=True,
                                    tolerance=np.pi/2, xlabel_rotation=45,
-                                   legend=True, legend_alpha=None):
+                                   legend=True, legend_alpha=None, linewidth=0.5):
         self.plot_baseline_displacement(phase=phase, corr=corr, caption=caption, cmap=cmap,
                                    displacement=displacement, unwrap=unwrap,
                                    stl=stl, stl_freq=stl_freq, stl_periods=stl_periods, stl_robust=stl_robust,
                                    los=True, tolerance=tolerance, xlabel_rotation=xlabel_rotation,
-                                   legend=legend, legend_alpha=legend_alpha)
+                                   legend=legend, legend_alpha=legend_alpha, linewidth=linewidth)
 
     def rmse(self, data, solution, weight=None):
         """
         Calculate difference between pairs and dates
     
         Use to calculate solution vs pair unwrapped phases difference as
         diff = sbas.stack_vs_cube(phase_unwrap, solution)
```

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_stl.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_stl.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,22 @@
 # ----------------------------------------------------------------------------
 from .Stack_tidal import Stack_tidal
 from .tqdm_dask import tqdm_dask
 
 class Stack_stl(Stack_tidal):
 
     def velocity(self, data):
-        years = ((data.date.max() - data.date.min()).dt.days/365.25).item()
-        #print ('years', np.round(years, 3))
-        velocity = data.mean('date')/years
+        print('NOTE: Velocity calculation is changed to use least squares linear fit and can produce different results.')
+        #years = ((data.date.max() - data.date.min()).dt.days/365.25).item()
+        #nanoseconds = data.date.max().astype(int) - data.date.min().astype(int)
+        #print ('years', np.round(years, 3), 'nanoseconds', nanoseconds)
+        #velocity = nanoseconds*data.polyfit('date', 1).polyfit_coefficients.sel(degree=1)/years
+        nanoseconds_per_year = 365.25*24*60*60*1e9
+        # calculate slope per year
+        velocity = nanoseconds_per_year*data.polyfit('date', 1).polyfit_coefficients.sel(degree=1).rename('trend')
         return velocity
 
     def trend(self, data, deg=1):
         import xarray as xr
 
         trend = xr.polyval(data.date, data.polyfit('date', deg).polyfit_coefficients)
         return trend
```

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_tidal.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_tidal.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_topo.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_topo.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_trans.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_trans.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_trans_inv.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_trans_inv.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_unwrap.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_unwrap.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Stack_unwrap_snaphu.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Stack_unwrap_snaphu.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/Tiles.py` & `pygmtsar-2024.4.17.post5/pygmtsar/Tiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/XYZTiles.py` & `pygmtsar-2024.4.17.post5/pygmtsar/XYZTiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,18 @@
         kwargs['url'] = 'https://mt1.google.com/vt/lyrs=y&x={x}&y={y}&z={z}'
         return self.download(geometry, zoom, filename, **kwargs)
 
     def download_openstreetmap(self, geometry, zoom, filename=None, **kwargs):
         kwargs['url'] = 'https://tile.openstreetmap.org/{z}/{x}/{y}.png'
         return self.download(geometry, zoom, filename, **kwargs)
 
+    def download_openrailwaymap(self, geometry, zoom, filename=None, **kwargs):
+        kwargs['url'] = 'https://mt1.google.com/vt/lyrs=r&x={x}&y={y}&z={z}'
+        return self.download(geometry, zoom, filename, **kwargs)
+
     def download(self, geometry, zoom, filename=None, url='https://mt1.google.com/vt/lyrs=y&x={x}&y={y}&z={z}', n_jobs=8, skip_exist=True, debug=False):
         """
         Downloads map tiles for a specified geometry and zoom level from a given tile map service.
 
         Parameters
         ----------
         geometry : object
```

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/_Stack_merge.py` & `pygmtsar-2024.4.17.post5/pygmtsar/_Stack_merge.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/__init__.py` & `pygmtsar-2024.4.17.post5/pygmtsar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 
 # This file is part of the PyGMTSAR project: https://github.com/mobigroup/gmtsar
 # 
 # Copyright (c) 2023, Alexey Pechnikov
 # 
 # Licensed under the BSD 3-Clause License (see LICENSE for details)
 # ----------------------------------------------------------------------------
-__version__ = '2024.4.17.post3'
+__version__ = '2024.4.17.post5'
 
 # unified progress indicators
 from .tqdm_joblib import tqdm_joblib
 from .tqdm_dask import tqdm_dask
 # base NetCDF operations and parameters on NetCDF grid
 from .datagrid import datagrid
 # top level module classes
```

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/datagrid.py` & `pygmtsar-2024.4.17.post5/pygmtsar/datagrid.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/tqdm_dask.py` & `pygmtsar-2024.4.17.post5/pygmtsar/tqdm_dask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/tqdm_joblib.py` & `pygmtsar-2024.4.17.post5/pygmtsar/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar/utils.py` & `pygmtsar-2024.4.17.post5/pygmtsar/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar.egg-info/PKG-INFO` & `pygmtsar-2024.4.17.post5/pygmtsar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.4.17.post3
+Version: 2024.4.17.post5
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.4.17.post3/pygmtsar.egg-info/SOURCES.txt` & `pygmtsar-2024.4.17.post5/pygmtsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post3/setup.py` & `pygmtsar-2024.4.17.post5/setup.py`

 * *Files identical despite different names*

