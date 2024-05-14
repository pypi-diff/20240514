# Comparing `tmp/vardll-1.3.1.tar.gz` & `tmp/vardll-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vardll-1.3.1.tar", last modified: Mon May 13 20:10:37 2024, max compression
+gzip compressed data, was "vardll-1.3.4.tar", last modified: Tue May 14 21:31:58 2024, max compression
```

## Comparing `vardll-1.3.1.tar` & `vardll-1.3.4.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 20:10:37.113219 vardll-1.3.1/
--rw-rw-rw-   0        0        0      305 2024-05-13 20:10:37.110343 vardll-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1109 2024-05-13 19:52:21.000000 vardll-1.3.1/license
--rw-rw-rw-   0        0        0       42 2024-05-13 20:10:37.114216 vardll-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      534 2024-05-13 20:10:21.000000 vardll-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:10:37.107335 vardll-1.3.1/vardll.egg-info/
--rw-rw-rw-   0        0        0      305 2024-05-13 20:10:36.000000 vardll-1.3.1/vardll.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-13 20:10:36.000000 vardll-1.3.1/vardll.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 20:10:36.000000 vardll-1.3.1/vardll.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-13 20:10:36.000000 vardll-1.3.1/vardll.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-13 20:10:36.000000 vardll-1.3.1/vardll.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 20:10:36.000000 vardll-1.3.1/vardll.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 21:31:58.203422 vardll-1.3.4/
+-rw-rw-rw-   0        0        0      280 2024-05-14 21:31:58.199077 vardll-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1109 2024-05-13 19:52:21.000000 vardll-1.3.4/license
+-rw-rw-rw-   0        0        0       42 2024-05-14 21:31:58.203534 vardll-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      507 2024-05-14 21:26:57.000000 vardll-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:31:58.166190 vardll-1.3.4/vardll/
+-rw-rw-rw-   0        0        0       60 2024-05-13 19:47:11.000000 vardll-1.3.4/vardll/__init__.py
+-rw-rw-rw-   0        0        0      306 2024-05-13 18:24:47.000000 vardll-1.3.4/vardll/dllvariable.py
+-rw-rw-rw-   0        0        0      402 2024-05-13 18:49:06.000000 vardll-1.3.4/vardll/loader.py
+-rw-rw-rw-   0        0        0      534 2024-05-13 20:10:21.000000 vardll-1.3.4/vardll/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:31:58.196617 vardll-1.3.4/vardll.egg-info/
+-rw-rw-rw-   0        0        0      280 2024-05-14 21:31:57.000000 vardll-1.3.4/vardll.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-05-14 21:31:57.000000 vardll-1.3.4/vardll.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 21:31:57.000000 vardll-1.3.4/vardll.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-14 21:31:57.000000 vardll-1.3.4/vardll.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-05-14 21:31:57.000000 vardll-1.3.4/vardll.egg-info/top_level.txt
```

### Comparing `vardll-1.3.1/license` & `vardll-1.3.4/license`

 * *Files identical despite different names*

### Comparing `vardll-1.3.1/setup.py` & `vardll-1.3.4/vardll/setup.py`

 * *Files identical despite different names*

