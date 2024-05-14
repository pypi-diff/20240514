# Comparing `tmp/biaplotter-0.0.2.tar.gz` & `tmp/biaplotter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biaplotter-0.0.2.tar", last modified: Tue May  7 13:47:55 2024, max compression
+gzip compressed data, was "biaplotter-0.0.3.tar", last modified: Tue May 14 15:00:21 2024, max compression
```

## Comparing `biaplotter-0.0.2.tar` & `biaplotter-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:55.919432 biaplotter-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-07 13:47:45.000000 biaplotter-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-07 13:47:45.000000 biaplotter-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-07 13:47:55.919432 biaplotter-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-07 13:47:45.000000 biaplotter-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-07 13:47:45.000000 biaplotter-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-07 13:47:55.919432 biaplotter-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:55.915432 biaplotter-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:55.915432 biaplotter-0.0.2/src/biaplotter/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:55.919432 biaplotter-0.0.2/src/biaplotter/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/_tests/test_artists.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/_tests/test_selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    17302 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/artists.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18420 2024-05-07 13:47:45.000000 biaplotter-0.0.2/src/biaplotter/selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:55.919432 biaplotter-0.0.2/src/biaplotter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-07 13:47:55.000000 biaplotter-0.0.2/src/biaplotter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-07 13:47:55.000000 biaplotter-0.0.2/src/biaplotter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:47:55.000000 biaplotter-0.0.2/src/biaplotter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 13:47:55.000000 biaplotter-0.0.2/src/biaplotter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 13:47:55.000000 biaplotter-0.0.2/src/biaplotter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 13:47:55.000000 biaplotter-0.0.2/src/biaplotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:00:21.556127 biaplotter-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-14 15:00:11.000000 biaplotter-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 15:00:11.000000 biaplotter-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-14 15:00:21.556127 biaplotter-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-14 15:00:11.000000 biaplotter-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-14 15:00:11.000000 biaplotter-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-14 15:00:21.556127 biaplotter-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:00:21.552127 biaplotter-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:00:21.552127 biaplotter-0.0.3/src/biaplotter/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-14 15:00:11.000000 biaplotter-0.0.3/src/biaplotter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:00:21.556127 biaplotter-0.0.3/src/biaplotter/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:00:11.000000 biaplotter-0.0.3/src/biaplotter/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-14 15:00:11.000000 biaplotter-0.0.3/src/biaplotter/_tests/test_artists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-14 15:00:11.000000 biaplotter-0.0.3/src/biaplotter/_tests/test_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-14 15:00:11.000000 biaplotter-0.0.3/src/biaplotter/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17302 2024-05-14 15:00:11.000000 biaplotter-0.0.3/src/biaplotter/artists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-14 15:00:11.000000 biaplotter-0.0.3/src/biaplotter/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-14 15:00:11.000000 biaplotter-0.0.3/src/biaplotter/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18420 2024-05-14 15:00:11.000000 biaplotter-0.0.3/src/biaplotter/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:00:21.556127 biaplotter-0.0.3/src/biaplotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-14 15:00:21.000000 biaplotter-0.0.3/src/biaplotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-14 15:00:21.000000 biaplotter-0.0.3/src/biaplotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:00:21.000000 biaplotter-0.0.3/src/biaplotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 15:00:21.000000 biaplotter-0.0.3/src/biaplotter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 15:00:21.000000 biaplotter-0.0.3/src/biaplotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 15:00:21.000000 biaplotter-0.0.3/src/biaplotter.egg-info/top_level.txt
```

### Comparing `biaplotter-0.0.2/LICENSE` & `biaplotter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biaplotter-0.0.2/PKG-INFO` & `biaplotter-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biaplotter
-Version: 0.0.2
+Version: 0.0.3
 Summary: A base napari plotter widget for interactive plotting
 Home-page: https://github.com/BiAPoL/biaplotter
 Author: Marcelo Leomil Zoccoler
 Author-email: marzoccoler@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/BiAPoL/biaplotter/issues
 Project-URL: Documentation, https://github.com/BiAPoL/biaplotter#README.md
```

### Comparing `biaplotter-0.0.2/README.md` & `biaplotter-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `biaplotter-0.0.2/pyproject.toml` & `biaplotter-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biaplotter-0.0.2/setup.cfg` & `biaplotter-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `biaplotter-0.0.2/src/biaplotter/_tests/test_artists.py` & `biaplotter-0.0.3/src/biaplotter/_tests/test_artists.py`

 * *Files identical despite different names*

### Comparing `biaplotter-0.0.2/src/biaplotter/_tests/test_selectors.py` & `biaplotter-0.0.3/src/biaplotter/_tests/test_selectors.py`

 * *Files identical despite different names*

### Comparing `biaplotter-0.0.2/src/biaplotter/artists.py` & `biaplotter-0.0.3/src/biaplotter/artists.py`

 * *Files identical despite different names*

### Comparing `biaplotter-0.0.2/src/biaplotter/plotter.py` & `biaplotter-0.0.3/src/biaplotter/plotter.py`

 * *Files identical despite different names*

### Comparing `biaplotter-0.0.2/src/biaplotter/selectors.py` & `biaplotter-0.0.3/src/biaplotter/selectors.py`

 * *Files identical despite different names*

### Comparing `biaplotter-0.0.2/src/biaplotter.egg-info/PKG-INFO` & `biaplotter-0.0.3/src/biaplotter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biaplotter
-Version: 0.0.2
+Version: 0.0.3
 Summary: A base napari plotter widget for interactive plotting
 Home-page: https://github.com/BiAPoL/biaplotter
 Author: Marcelo Leomil Zoccoler
 Author-email: marzoccoler@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/BiAPoL/biaplotter/issues
 Project-URL: Documentation, https://github.com/BiAPoL/biaplotter#README.md
```

### Comparing `biaplotter-0.0.2/src/biaplotter.egg-info/SOURCES.txt` & `biaplotter-0.0.3/src/biaplotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

