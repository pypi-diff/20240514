# Comparing `tmp/dataidea-0.1.4.tar.gz` & `tmp/dataidea-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataidea-0.1.4.tar", last modified: Tue May  7 14:50:33 2024, max compression
+gzip compressed data, was "dataidea-0.1.5.tar", last modified: Tue May 14 11:11:27 2024, max compression
```

## Comparing `dataidea-0.1.4.tar` & `dataidea-0.1.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-07 14:50:33.924180 dataidea-0.1.4/
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    11337 2024-04-25 15:06:39.000000 dataidea-0.1.4/LICENSE
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      137 2024-05-07 13:55:08.000000 dataidea-0.1.4/MANIFEST.in
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2864 2024-05-07 14:50:33.924180 dataidea-0.1.4/PKG-INFO
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2009 2024-04-30 16:38:32.000000 dataidea-0.1.4/README.md
-drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-07 14:50:33.916180 dataidea-0.1.4/dataidea/
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       22 2024-05-07 14:13:39.000000 dataidea-0.1.4/dataidea/__init__.py
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1030 2024-05-07 14:13:39.000000 dataidea-0.1.4/dataidea/_modidx.py
-drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-07 14:50:33.924180 dataidea-0.1.4/dataidea/datasets/
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1745 2024-05-06 10:01:07.000000 dataidea-0.1.4/dataidea/datasets/air_passengers.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    37145 2024-05-03 07:05:30.000000 dataidea-0.1.4/dataidea/datasets/boston.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      229 2024-04-19 06:31:05.000000 dataidea-0.1.4/dataidea/datasets/cluster.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     4645 2024-04-19 06:33:56.000000 dataidea-0.1.4/dataidea/datasets/demo.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    47391 2024-04-19 06:31:05.000000 dataidea-0.1.4/dataidea/datasets/fpl.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      370 2024-04-19 06:31:05.000000 dataidea-0.1.4/dataidea/datasets/homeprices.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     3780 2024-04-27 09:00:34.000000 dataidea-0.1.4/dataidea/datasets/mall.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)  2091239 2024-04-19 06:31:05.000000 dataidea-0.1.4/dataidea/datasets/melbourne.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      302 2024-04-19 06:31:05.000000 dataidea-0.1.4/dataidea/datasets/music.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      656 2024-04-19 06:31:05.000000 dataidea-0.1.4/dataidea/datasets/salaries.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    41983 2024-04-27 09:39:55.000000 dataidea-0.1.4/dataidea/datasets/student-mat.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    68558 2024-04-27 09:39:44.000000 dataidea-0.1.4/dataidea/datasets/student-por.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)   108285 2024-04-19 06:31:05.000000 dataidea-0.1.4/dataidea/datasets/titanic.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)  1355781 2024-04-19 06:31:05.000000 dataidea-0.1.4/dataidea/datasets/vgsales.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      217 2024-04-19 06:31:05.000000 dataidea-0.1.4/dataidea/datasets/weather.csv
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1030 2024-04-27 09:51:24.000000 dataidea-0.1.4/dataidea/datasets.py
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      167 2024-04-27 09:39:06.000000 dataidea-0.1.4/dataidea/packages.py
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1230 2024-05-07 14:13:39.000000 dataidea-0.1.4/dataidea/statistics.py
-drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-07 14:50:33.920180 dataidea-0.1.4/dataidea.egg-info/
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2864 2024-05-07 14:50:33.000000 dataidea-0.1.4/dataidea.egg-info/PKG-INFO
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      840 2024-05-07 14:50:33.000000 dataidea-0.1.4/dataidea.egg-info/SOURCES.txt
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        1 2024-05-07 14:50:33.000000 dataidea-0.1.4/dataidea.egg-info/dependency_links.txt
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       59 2024-05-07 14:50:33.000000 dataidea-0.1.4/dataidea.egg-info/entry_points.txt
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        1 2024-05-05 12:55:26.000000 dataidea-0.1.4/dataidea.egg-info/not-zip-safe
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       70 2024-05-07 14:50:33.000000 dataidea-0.1.4/dataidea.egg-info/requires.txt
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        9 2024-05-07 14:50:33.000000 dataidea-0.1.4/dataidea.egg-info/top_level.txt
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1086 2024-05-07 14:50:09.000000 dataidea-0.1.4/settings.ini
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       38 2024-05-07 14:50:33.924180 dataidea-0.1.4/setup.cfg
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2641 2024-05-07 14:28:14.000000 dataidea-0.1.4/setup.py
+drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-14 11:11:27.724284 dataidea-0.1.5/
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    11337 2024-04-25 15:06:39.000000 dataidea-0.1.5/LICENSE
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      137 2024-05-07 13:55:08.000000 dataidea-0.1.5/MANIFEST.in
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    17263 2024-05-14 11:11:27.724284 dataidea-0.1.5/PKG-INFO
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    16408 2024-05-14 11:10:01.000000 dataidea-0.1.5/README.md
+drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-14 11:11:27.712280 dataidea-0.1.5/dataidea/
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      123 2024-05-14 10:38:11.000000 dataidea-0.1.5/dataidea/__init__.py
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1633 2024-05-14 10:23:54.000000 dataidea-0.1.5/dataidea/_modidx.py
+drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-14 11:11:27.724284 dataidea-0.1.5/dataidea/datasets/
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1745 2024-05-06 10:01:07.000000 dataidea-0.1.5/dataidea/datasets/air_passengers.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    37145 2024-05-03 07:05:30.000000 dataidea-0.1.5/dataidea/datasets/boston.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      229 2024-04-19 06:31:05.000000 dataidea-0.1.5/dataidea/datasets/cluster.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     4645 2024-04-19 06:33:56.000000 dataidea-0.1.5/dataidea/datasets/demo.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    47391 2024-04-19 06:31:05.000000 dataidea-0.1.5/dataidea/datasets/fpl.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      370 2024-04-19 06:31:05.000000 dataidea-0.1.5/dataidea/datasets/homeprices.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     3780 2024-04-27 09:00:34.000000 dataidea-0.1.5/dataidea/datasets/mall.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)  2091239 2024-04-19 06:31:05.000000 dataidea-0.1.5/dataidea/datasets/melbourne.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      302 2024-04-19 06:31:05.000000 dataidea-0.1.5/dataidea/datasets/music.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      656 2024-04-19 06:31:05.000000 dataidea-0.1.5/dataidea/datasets/salaries.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    41983 2024-04-27 09:39:55.000000 dataidea-0.1.5/dataidea/datasets/student-mat.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    68558 2024-04-27 09:39:44.000000 dataidea-0.1.5/dataidea/datasets/student-por.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)   108285 2024-04-19 06:31:05.000000 dataidea-0.1.5/dataidea/datasets/titanic.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)  1355781 2024-04-19 06:31:05.000000 dataidea-0.1.5/dataidea/datasets/vgsales.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      217 2024-04-19 06:31:05.000000 dataidea-0.1.5/dataidea/datasets/weather.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1030 2024-04-27 09:51:24.000000 dataidea-0.1.5/dataidea/datasets.py
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      822 2024-05-14 10:23:54.000000 dataidea-0.1.5/dataidea/models.py
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      167 2024-04-27 09:39:06.000000 dataidea-0.1.5/dataidea/packages.py
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1230 2024-05-14 10:23:54.000000 dataidea-0.1.5/dataidea/statistics.py
+drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-14 11:11:27.712280 dataidea-0.1.5/dataidea.egg-info/
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    17263 2024-05-14 11:11:27.000000 dataidea-0.1.5/dataidea.egg-info/PKG-INFO
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      859 2024-05-14 11:11:27.000000 dataidea-0.1.5/dataidea.egg-info/SOURCES.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        1 2024-05-14 11:11:27.000000 dataidea-0.1.5/dataidea.egg-info/dependency_links.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       59 2024-05-14 11:11:27.000000 dataidea-0.1.5/dataidea.egg-info/entry_points.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        1 2024-05-05 12:55:26.000000 dataidea-0.1.5/dataidea.egg-info/not-zip-safe
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       70 2024-05-14 11:11:27.000000 dataidea-0.1.5/dataidea.egg-info/requires.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        9 2024-05-14 11:11:27.000000 dataidea-0.1.5/dataidea.egg-info/top_level.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1086 2024-05-14 10:35:30.000000 dataidea-0.1.5/settings.ini
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       38 2024-05-14 11:11:27.724284 dataidea-0.1.5/setup.cfg
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2641 2024-05-07 14:28:14.000000 dataidea-0.1.5/setup.py
```

### Comparing `dataidea-0.1.4/LICENSE` & `dataidea-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/datasets/air_passengers.csv` & `dataidea-0.1.5/dataidea/datasets/air_passengers.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/datasets/boston.csv` & `dataidea-0.1.5/dataidea/datasets/boston.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/datasets/demo.csv` & `dataidea-0.1.5/dataidea/datasets/demo.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/datasets/fpl.csv` & `dataidea-0.1.5/dataidea/datasets/fpl.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/datasets/mall.csv` & `dataidea-0.1.5/dataidea/datasets/mall.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/datasets/melbourne.csv` & `dataidea-0.1.5/dataidea/datasets/melbourne.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/datasets/salaries.csv` & `dataidea-0.1.5/dataidea/datasets/salaries.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/datasets/student-mat.csv` & `dataidea-0.1.5/dataidea/datasets/student-mat.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/datasets/student-por.csv` & `dataidea-0.1.5/dataidea/datasets/student-por.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/datasets/titanic.csv` & `dataidea-0.1.5/dataidea/datasets/titanic.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/datasets/vgsales.csv` & `dataidea-0.1.5/dataidea/datasets/vgsales.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/datasets.py` & `dataidea-0.1.5/dataidea/datasets.py`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea/statistics.py` & `dataidea-0.1.5/dataidea/statistics.py`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.4/dataidea.egg-info/SOURCES.txt` & `dataidea-0.1.5/dataidea.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 settings.ini
 setup.py
 dataidea/__init__.py
 dataidea/_modidx.py
 dataidea/datasets.py
+dataidea/models.py
 dataidea/packages.py
 dataidea/statistics.py
 dataidea.egg-info/PKG-INFO
 dataidea.egg-info/SOURCES.txt
 dataidea.egg-info/dependency_links.txt
 dataidea.egg-info/entry_points.txt
 dataidea.egg-info/not-zip-safe
```

### Comparing `dataidea-0.1.4/settings.ini` & `dataidea-0.1.5/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = dataidea
 lib_name = %(repo)s
-version = 0.1.4
+version = 0.1.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = dataidea
```

### Comparing `dataidea-0.1.4/setup.py` & `dataidea-0.1.5/setup.py`

 * *Files identical despite different names*

