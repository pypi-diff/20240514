# Comparing `tmp/sortipy-0.0.2.tar.gz` & `tmp/sortipy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortipy-0.0.2.tar", last modified: Tue May 14 11:13:14 2024, max compression
+gzip compressed data, was "sortipy-0.0.3.tar", last modified: Tue May 14 21:11:44 2024, max compression
```

## Comparing `sortipy-0.0.2.tar` & `sortipy-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 11:13:14.492807 sortipy-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-05-14 10:16:33.000000 sortipy-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-14 10:57:17.000000 sortipy-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      592 2024-05-14 11:13:14.490813 sortipy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-05-14 10:18:52.000000 sortipy-0.0.2/README.md
--rw-rw-rw-   0        0        0       86 2024-05-14 10:58:30.000000 sortipy-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 11:13:14.493805 sortipy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      528 2024-05-14 11:11:50.000000 sortipy-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:13:14.442418 sortipy-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 11:13:14.460786 sortipy-0.0.2/src/sortipy/
--rw-rw-rw-   0        0        0        0 2024-05-14 10:25:51.000000 sortipy-0.0.2/src/sortipy/__init__.py
--rw-rw-rw-   0        0        0      161 2024-05-14 10:27:43.000000 sortipy-0.0.2/src/sortipy/sortipy.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:13:14.489816 sortipy-0.0.2/src/sortipy.egg-info/
--rw-rw-rw-   0        0        0      592 2024-05-14 11:13:14.000000 sortipy-0.0.2/src/sortipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-14 11:13:14.000000 sortipy-0.0.2/src/sortipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 11:13:14.000000 sortipy-0.0.2/src/sortipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 11:13:14.000000 sortipy-0.0.2/src/sortipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.226017 sortipy-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-05-14 10:16:33.000000 sortipy-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-14 10:57:17.000000 sortipy-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3198 2024-05-14 21:11:44.221491 sortipy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2801 2024-05-14 21:07:55.000000 sortipy-0.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-14 10:58:30.000000 sortipy-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 21:11:44.226017 sortipy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      551 2024-05-14 21:09:49.000000 sortipy-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.146071 sortipy-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.174396 sortipy-0.0.3/src/sortipy/
+-rw-rw-rw-   0        0        0        0 2024-05-14 10:25:51.000000 sortipy-0.0.3/src/sortipy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.195730 sortipy-0.0.3/src/sortipy/exceptions/
+-rw-rw-rw-   0        0        0        0 2024-05-14 12:17:07.000000 sortipy-0.0.3/src/sortipy/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1546 2024-05-14 18:48:33.000000 sortipy-0.0.3/src/sortipy/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.206055 sortipy-0.0.3/src/sortipy/models/
+-rw-rw-rw-   0        0        0     1710 2024-05-14 20:28:27.000000 sortipy-0.0.3/src/sortipy/models/Directory.py
+-rw-rw-rw-   0        0        0     2050 2024-05-14 19:05:49.000000 sortipy-0.0.3/src/sortipy/models/File.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 12:14:42.000000 sortipy-0.0.3/src/sortipy/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.213951 sortipy-0.0.3/src/sortipy/sorters/
+-rw-rw-rw-   0        0        0     1458 2024-05-14 20:43:39.000000 sortipy-0.0.3/src/sortipy/sorters/DefaultSorter.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:53:00.000000 sortipy-0.0.3/src/sortipy/sorters/__init__.py
+-rw-rw-rw-   0        0        0     1125 2024-05-14 21:10:53.000000 sortipy-0.0.3/src/sortipy/sortipy.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:11:44.215938 sortipy-0.0.3/src/sortipy.egg-info/
+-rw-rw-rw-   0        0        0     3198 2024-05-14 21:11:44.000000 sortipy-0.0.3/src/sortipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-05-14 21:11:44.000000 sortipy-0.0.3/src/sortipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 21:11:44.000000 sortipy-0.0.3/src/sortipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 21:11:44.000000 sortipy-0.0.3/src/sortipy.egg-info/top_level.txt
```

### Comparing `sortipy-0.0.2/LICENSE` & `sortipy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sortipy-0.0.2/LICENSE.txt` & `sortipy-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

