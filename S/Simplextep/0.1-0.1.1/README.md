# Comparing `tmp/simplextep-0.1.tar.gz` & `tmp/simplextep-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplextep-0.1.tar", last modified: Tue May 14 20:43:14 2024, max compression
+gzip compressed data, was "simplextep-0.1.1.tar", last modified: Tue May 14 21:07:54 2024, max compression
```

## Comparing `simplextep-0.1.tar` & `simplextep-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 20:43:14.263409 simplextep-0.1/
--rw-rw-rw-   0        0        0     1082 2024-05-14 20:05:02.000000 simplextep-0.1/LICENSE
--rw-rw-rw-   0        0        0      331 2024-05-14 20:43:14.263409 simplextep-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       12 2024-05-14 20:05:02.000000 simplextep-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 20:43:14.263409 simplextep-0.1/Simplextep.egg-info/
--rw-rw-rw-   0        0        0      331 2024-05-14 20:43:14.000000 simplextep-0.1/Simplextep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-05-14 20:43:14.000000 simplextep-0.1/Simplextep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 20:43:14.000000 simplextep-0.1/Simplextep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-14 20:43:14.000000 simplextep-0.1/Simplextep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 20:43:14.000000 simplextep-0.1/Simplextep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 20:43:14.263409 simplextep-0.1/setup.cfg
--rw-rw-rw-   0        0        0      408 2024-05-14 20:42:39.000000 simplextep-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:07:54.317052 simplextep-0.1.1/
+-rw-rw-rw-   0        0        0     1082 2024-05-14 20:05:02.000000 simplextep-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      336 2024-05-14 21:07:54.314051 simplextep-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2024-05-14 20:51:03.000000 simplextep-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 21:07:54.311399 simplextep-0.1.1/Simplextep.egg-info/
+-rw-rw-rw-   0        0        0      336 2024-05-14 21:07:54.000000 simplextep-0.1.1/Simplextep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-05-14 21:07:54.000000 simplextep-0.1.1/Simplextep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 21:07:54.000000 simplextep-0.1.1/Simplextep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-14 21:07:54.000000 simplextep-0.1.1/Simplextep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 21:07:54.000000 simplextep-0.1.1/Simplextep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 21:07:54.317400 simplextep-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      383 2024-05-14 21:05:36.000000 simplextep-0.1.1/setup.py
```

### Comparing `simplextep-0.1/LICENSE` & `simplextep-0.1.1/LICENSE`

 * *Files identical despite different names*

