# Comparing `tmp/eazyAI-1.1.tar.gz` & `tmp/eazyAI-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eazyAI-1.1.tar", last modified: Tue May 14 10:50:08 2024, max compression
+gzip compressed data, was "eazyAI-1.1.1.tar", last modified: Tue May 14 10:57:30 2024, max compression
```

## Comparing `eazyAI-1.1.tar` & `eazyAI-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 10:50:08.012099 eazyAI-1.1/
--rw-rw-rw-   0        0        0    35823 2024-05-14 07:06:57.000000 eazyAI-1.1/LICENSE
--rw-rw-rw-   0        0        0      349 2024-05-14 10:50:08.008511 eazyAI-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       91 2024-05-14 07:06:57.000000 eazyAI-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 10:50:07.975551 eazyAI-1.1/eazyAI/
--rw-rw-rw-   0        0        0       31 2024-05-14 07:06:57.000000 eazyAI-1.1/eazyAI/__init__.py
--rw-rw-rw-   0        0        0     2855 2024-05-14 10:49:47.000000 eazyAI-1.1/eazyAI/main.py
-drwxrwxrwx   0        0        0        0 2024-05-14 10:50:08.005511 eazyAI-1.1/eazyAI.egg-info/
--rw-rw-rw-   0        0        0      349 2024-05-14 10:50:07.000000 eazyAI-1.1/eazyAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-05-14 10:50:07.000000 eazyAI-1.1/eazyAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 10:50:07.000000 eazyAI-1.1/eazyAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-14 10:50:07.000000 eazyAI-1.1/eazyAI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 10:50:07.000000 eazyAI-1.1/eazyAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 10:50:08.012099 eazyAI-1.1/setup.cfg
--rw-rw-rw-   0        0        0      458 2024-05-14 10:49:53.000000 eazyAI-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:57:30.321714 eazyAI-1.1.1/
+-rw-rw-rw-   0        0        0    35823 2024-05-14 07:06:57.000000 eazyAI-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      351 2024-05-14 10:57:30.320326 eazyAI-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       91 2024-05-14 07:06:57.000000 eazyAI-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 10:57:30.300395 eazyAI-1.1.1/eazyAI/
+-rw-rw-rw-   0        0        0       83 2024-05-14 10:56:49.000000 eazyAI-1.1.1/eazyAI/__init__.py
+-rw-rw-rw-   0        0        0     4328 2024-05-14 10:56:58.000000 eazyAI-1.1.1/eazyAI/main.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:57:30.318243 eazyAI-1.1.1/eazyAI.egg-info/
+-rw-rw-rw-   0        0        0      351 2024-05-14 10:57:30.000000 eazyAI-1.1.1/eazyAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-05-14 10:57:30.000000 eazyAI-1.1.1/eazyAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 10:57:30.000000 eazyAI-1.1.1/eazyAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-14 10:57:30.000000 eazyAI-1.1.1/eazyAI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-14 10:57:30.000000 eazyAI-1.1.1/eazyAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 10:57:30.321714 eazyAI-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      461 2024-05-14 10:57:04.000000 eazyAI-1.1.1/setup.py
```

### Comparing `eazyAI-1.1/LICENSE` & `eazyAI-1.1.1/LICENSE`

 * *Files identical despite different names*

