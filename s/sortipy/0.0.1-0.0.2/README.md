# Comparing `tmp/sortipy-0.0.1.tar.gz` & `tmp/sortipy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortipy-0.0.1.tar", last modified: Tue May 14 10:59:48 2024, max compression
+gzip compressed data, was "sortipy-0.0.2.tar", last modified: Tue May 14 11:13:14 2024, max compression
```

## Comparing `sortipy-0.0.1.tar` & `sortipy-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 10:59:48.475120 sortipy-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-05-14 10:16:33.000000 sortipy-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-14 10:57:17.000000 sortipy-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1893 2024-05-14 10:59:48.472447 sortipy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-05-14 10:18:52.000000 sortipy-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2024-05-14 10:58:30.000000 sortipy-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      707 2024-05-14 10:59:48.484096 sortipy-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 10:59:48.380896 sortipy-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 10:59:48.468880 sortipy-0.0.1/src/sortipy.egg-info/
--rw-rw-rw-   0        0        0     1893 2024-05-14 10:59:48.000000 sortipy-0.0.1/src/sortipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-05-14 10:59:48.000000 sortipy-0.0.1/src/sortipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 10:59:48.000000 sortipy-0.0.1/src/sortipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 10:59:48.000000 sortipy-0.0.1/src/sortipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 11:13:14.492807 sortipy-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-05-14 10:16:33.000000 sortipy-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-14 10:57:17.000000 sortipy-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      592 2024-05-14 11:13:14.490813 sortipy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-14 10:18:52.000000 sortipy-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-14 10:58:30.000000 sortipy-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 11:13:14.493805 sortipy-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      528 2024-05-14 11:11:50.000000 sortipy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:13:14.442418 sortipy-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 11:13:14.460786 sortipy-0.0.2/src/sortipy/
+-rw-rw-rw-   0        0        0        0 2024-05-14 10:25:51.000000 sortipy-0.0.2/src/sortipy/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-05-14 10:27:43.000000 sortipy-0.0.2/src/sortipy/sortipy.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:13:14.489816 sortipy-0.0.2/src/sortipy.egg-info/
+-rw-rw-rw-   0        0        0      592 2024-05-14 11:13:14.000000 sortipy-0.0.2/src/sortipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-14 11:13:14.000000 sortipy-0.0.2/src/sortipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 11:13:14.000000 sortipy-0.0.2/src/sortipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 11:13:14.000000 sortipy-0.0.2/src/sortipy.egg-info/top_level.txt
```

### Comparing `sortipy-0.0.1/LICENSE` & `sortipy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sortipy-0.0.1/LICENSE.txt` & `sortipy-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

