# Comparing `tmp/intervalframe-1.1.6.tar.gz` & `tmp/intervalframe-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intervalframe-1.1.6.tar", max compression
+gzip compressed data, was "intervalframe-1.1.7.tar", max compression
```

## Comparing `intervalframe-1.1.6.tar` & `intervalframe-1.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 intervalframe-1.1.6/LICENSE.md
--rwxr-xr-x   0        0        0     1017 2022-01-03 18:58:56.000000 intervalframe-1.1.6/README.md
--rw-r--r--   0        0        0    10244 2024-04-16 02:08:23.772983 intervalframe-1.1.6/intervalframe/.DS_Store
--rw-r--r--   0        0        0      444 2024-04-16 15:17:25.472478 intervalframe-1.1.6/intervalframe/__init__.py
--rw-r--r--   0        0        0     6148 2023-05-08 15:06:34.044574 intervalframe-1.1.6/intervalframe/core/.DS_Store
--rw-r--r--   0        0        0    37509 2024-03-24 14:37:29.349744 intervalframe-1.1.6/intervalframe/core/IntervalFrame.py
--rw-r--r--   0        0        0    18564 2023-05-08 14:58:21.201049 intervalframe-1.1.6/intervalframe/core/IntervalSeries.py
--rw-r--r--   0        0        0     1244 2020-06-30 16:23:05.000000 intervalframe-1.1.6/intervalframe/core/groupby.py
--rw-r--r--   0        0        0     4299 2022-01-10 22:35:34.000000 intervalframe-1.1.6/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc
--rw-r--r--   0        0        0     7166 2023-10-19 17:43:31.000000 intervalframe-1.1.6/intervalframe/core/index/indexers.py
--rw-r--r--   0        0        0     2473 2021-09-21 15:04:53.000000 intervalframe-1.1.6/intervalframe/read/__pycache__/read_h5.cpython-39.pyc
--rw-r--r--   0        0        0     1191 2022-01-10 22:35:34.000000 intervalframe-1.1.6/intervalframe/read/__pycache__/read_text.cpython-39.pyc
--rw-r--r--   0        0        0    20974 2021-02-11 01:01:08.000000 intervalframe-1.1.6/intervalframe/read/h5_utilities.py
--rw-r--r--   0        0        0     6848 2023-03-25 17:26:19.423023 intervalframe-1.1.6/intervalframe/read/read_h5.py
--rw-r--r--   0        0        0      815 2023-01-26 17:56:39.789523 intervalframe-1.1.6/intervalframe/read/read_parquet.py
--rw-r--r--   0        0        0     2453 2023-01-26 20:00:28.520286 intervalframe-1.1.6/intervalframe/read/read_text.py
--rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.6/intervalframe/utilities/h5_utilities.py
--rw-r--r--   0        0        0     2856 2021-09-21 15:04:53.000000 intervalframe-1.1.6/intervalframe/write/__pycache__/write_h5.cpython-39.pyc
--rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.6/intervalframe/write/h5_utilities.py
--rw-r--r--   0        0        0     7188 2023-07-09 18:13:58.775799 intervalframe-1.1.6/intervalframe/write/write_h5.py
--rw-r--r--   0        0        0      736 2023-01-30 21:43:29.435395 intervalframe-1.1.6/intervalframe/write/write_parquet.py
--rw-r--r--   0        0        0      760 2024-04-16 02:10:32.144159 intervalframe-1.1.6/intervalframe/write/write_text.py
--rw-r--r--   0        0        0     2062 2024-04-16 15:36:27.270949 intervalframe-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     2946 1970-01-01 00:00:00.000000 intervalframe-1.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 intervalframe-1.1.7/LICENSE.md
+-rwxr-xr-x   0        0        0     1017 2022-01-03 18:58:56.000000 intervalframe-1.1.7/README.md
+-rw-r--r--   0        0        0    10244 2024-05-14 15:13:54.348884 intervalframe-1.1.7/intervalframe/.DS_Store
+-rw-r--r--   0        0        0      444 2024-05-14 20:24:03.499791 intervalframe-1.1.7/intervalframe/__init__.py
+-rw-r--r--   0        0        0     6148 2023-05-08 15:06:34.044574 intervalframe-1.1.7/intervalframe/core/.DS_Store
+-rw-r--r--   0        0        0    37509 2024-03-24 14:37:29.349744 intervalframe-1.1.7/intervalframe/core/IntervalFrame.py
+-rw-r--r--   0        0        0    18564 2023-05-08 14:58:21.201049 intervalframe-1.1.7/intervalframe/core/IntervalSeries.py
+-rw-r--r--   0        0        0     1244 2020-06-30 16:23:05.000000 intervalframe-1.1.7/intervalframe/core/groupby.py
+-rw-r--r--   0        0        0     4299 2022-01-10 22:35:34.000000 intervalframe-1.1.7/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc
+-rw-r--r--   0        0        0     7166 2023-10-19 17:43:31.000000 intervalframe-1.1.7/intervalframe/core/index/indexers.py
+-rw-r--r--   0        0        0     2473 2021-09-21 15:04:53.000000 intervalframe-1.1.7/intervalframe/read/__pycache__/read_h5.cpython-39.pyc
+-rw-r--r--   0        0        0     1191 2022-01-10 22:35:34.000000 intervalframe-1.1.7/intervalframe/read/__pycache__/read_text.cpython-39.pyc
+-rw-r--r--   0        0        0    20974 2021-02-11 01:01:08.000000 intervalframe-1.1.7/intervalframe/read/h5_utilities.py
+-rw-r--r--   0        0        0     6848 2023-03-25 17:26:19.423023 intervalframe-1.1.7/intervalframe/read/read_h5.py
+-rw-r--r--   0        0        0      815 2023-01-26 17:56:39.789523 intervalframe-1.1.7/intervalframe/read/read_parquet.py
+-rw-r--r--   0        0        0     2453 2023-01-26 20:00:28.520286 intervalframe-1.1.7/intervalframe/read/read_text.py
+-rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.7/intervalframe/utilities/h5_utilities.py
+-rw-r--r--   0        0        0     2856 2021-09-21 15:04:53.000000 intervalframe-1.1.7/intervalframe/write/__pycache__/write_h5.cpython-39.pyc
+-rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.7/intervalframe/write/h5_utilities.py
+-rw-r--r--   0        0        0     7188 2023-07-09 18:13:58.775799 intervalframe-1.1.7/intervalframe/write/write_h5.py
+-rw-r--r--   0        0        0      736 2023-01-30 21:43:29.435395 intervalframe-1.1.7/intervalframe/write/write_parquet.py
+-rw-r--r--   0        0        0      760 2024-04-16 02:10:32.144159 intervalframe-1.1.7/intervalframe/write/write_text.py
+-rw-r--r--   0        0        0     2062 2024-05-14 20:23:52.561661 intervalframe-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2946 1970-01-01 00:00:00.000000 intervalframe-1.1.7/PKG-INFO
```

### Comparing `intervalframe-1.1.6/LICENSE.md` & `intervalframe-1.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/README.md` & `intervalframe-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/.DS_Store` & `intervalframe-1.1.7/intervalframe/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,15 @@
 000012f0: 00b8 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
 00001300: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
 00001310: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
 00001320: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 00001330: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 00001340: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00001350: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
-00001360: 095f 1018 7b7b 3335 372c 2034 3330 7d2c  ._..{{357, 430},
+00001360: 095f 1018 7b7b 3237 302c 2034 3339 7d2c  ._..{{270, 439},
 00001370: 207b 3932 302c 2034 3336 7d7d 0908 1523   {920, 436}}...#
 00001380: 2f3b 525f 6b6c 6d6e 6f8a 0000 0000 0000  /;R_klmno.......
 00001390: 0101 0000 0000 0000 000d 0000 0000 0000  ................
 000013a0: 0000 0000 0000 0000 008b 0000 0005 0077  ...............w
 000013b0: 0072 0069 0074 0065 6c73 7643 626c 6f62  .r.i.t.elsvCblob
 000013c0: 0000 0316 6270 6c69 7374 3030 d801 0203  ....bplist00....
 000013d0: 0405 0607 0809 0a0b 1956 5758 0a5f 1012  .........VWX._..
```

### Comparing `intervalframe-1.1.6/intervalframe/core/.DS_Store` & `intervalframe-1.1.7/intervalframe/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/core/IntervalFrame.py` & `intervalframe-1.1.7/intervalframe/core/IntervalFrame.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/core/IntervalSeries.py` & `intervalframe-1.1.7/intervalframe/core/IntervalSeries.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/core/groupby.py` & `intervalframe-1.1.7/intervalframe/core/groupby.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc` & `intervalframe-1.1.7/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/core/index/indexers.py` & `intervalframe-1.1.7/intervalframe/core/index/indexers.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/read/__pycache__/read_h5.cpython-39.pyc` & `intervalframe-1.1.7/intervalframe/read/__pycache__/read_h5.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/read/__pycache__/read_text.cpython-39.pyc` & `intervalframe-1.1.7/intervalframe/read/__pycache__/read_text.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/read/h5_utilities.py` & `intervalframe-1.1.7/intervalframe/read/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/read/read_h5.py` & `intervalframe-1.1.7/intervalframe/read/read_h5.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/read/read_parquet.py` & `intervalframe-1.1.7/intervalframe/read/read_parquet.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/read/read_text.py` & `intervalframe-1.1.7/intervalframe/read/read_text.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/utilities/h5_utilities.py` & `intervalframe-1.1.7/intervalframe/utilities/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/write/__pycache__/write_h5.cpython-39.pyc` & `intervalframe-1.1.7/intervalframe/write/__pycache__/write_h5.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/write/h5_utilities.py` & `intervalframe-1.1.7/intervalframe/write/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/write/write_h5.py` & `intervalframe-1.1.7/intervalframe/write/write_h5.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/write/write_parquet.py` & `intervalframe-1.1.7/intervalframe/write/write_parquet.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/intervalframe/write/write_text.py` & `intervalframe-1.1.7/intervalframe/write/write_text.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.6/pyproject.toml` & `intervalframe-1.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "intervalframe"
-version = "1.1.6"
+version = "1.1.7"
 description = "Python package for interval manipulation"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/intervalframe"
 documentation = "https://www.biosciencestack.com/static/intervalframe/docs/index.html"
 keywords = ["cython", "interval", "ailist", "frame"]
 readme = 'README.md'
@@ -33,15 +33,15 @@
 pandas = "^2.0.0"
 ailist = "^2.1.3"
 tabulate = "^0.9.0"
 linear_segment = "^1.1.2"
 h5py = "^3.8.0"
 scipy = "^1.9.1"
 requests = "^2.28.2"
-pyarrow = "^12.0.0"
+pyarrow = "^14.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0",
             "cython>=3.0.0",
```

### Comparing `intervalframe-1.1.6/PKG-INFO` & `intervalframe-1.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intervalframe
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python package for interval manipulation
 Home-page: https://github.com/kylessmith/intervalframe
 License: GPL-2.0-or-later
 Keywords: cython,interval,ailist,frame
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
@@ -30,15 +30,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: ailist (>=2.1.3,<3.0.0)
 Requires-Dist: cython (>=3.0.0,<4.0.0)
 Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: linear_segment (>=1.1.2,<2.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
-Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
+Requires-Dist: pyarrow (>=14.0.0,<15.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://www.biosciencestack.com/static/intervalframe/docs/index.html
 Project-URL: Repository, https://github.com/kylessmith/intervalframe
 Description-Content-Type: text/markdown
```

