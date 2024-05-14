# Comparing `tmp/metals_api_zylalabs-0.3.tar.gz` & `tmp/metals_api_zylalabs-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metals_api_zylalabs-0.3.tar", last modified: Mon May 13 19:52:24 2024, max compression
+gzip compressed data, was "metals_api_zylalabs-0.4.tar", last modified: Tue May 14 14:16:53 2024, max compression
```

## Comparing `metals_api_zylalabs-0.3.tar` & `metals_api_zylalabs-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 19:52:24.013785 metals_api_zylalabs-0.3/
--rw-rw-rw-   0        0        0     1072 2024-05-13 19:52:24.012772 metals_api_zylalabs-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      963 2024-05-13 19:51:07.000000 metals_api_zylalabs-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 19:52:23.983941 metals_api_zylalabs-0.3/metals_api_zylalabs/
--rw-rw-rw-   0        0        0       88 2024-05-13 19:50:11.000000 metals_api_zylalabs-0.3/metals_api_zylalabs/__init__.py
--rw-rw-rw-   0        0        0      621 2024-05-13 19:49:31.000000 metals_api_zylalabs-0.3/metals_api_zylalabs/client.py
-drwxrwxrwx   0        0        0        0 2024-05-13 19:52:24.011432 metals_api_zylalabs-0.3/metals_api_zylalabs.egg-info/
--rw-rw-rw-   0        0        0     1072 2024-05-13 19:52:23.000000 metals_api_zylalabs-0.3/metals_api_zylalabs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-13 19:52:23.000000 metals_api_zylalabs-0.3/metals_api_zylalabs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 19:52:23.000000 metals_api_zylalabs-0.3/metals_api_zylalabs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-13 19:52:23.000000 metals_api_zylalabs-0.3/metals_api_zylalabs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 19:52:24.014775 metals_api_zylalabs-0.3/setup.cfg
--rw-rw-rw-   0        0        0      333 2024-05-13 19:48:50.000000 metals_api_zylalabs-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:16:53.285132 metals_api_zylalabs-0.4/
+-rw-rw-rw-   0        0        0     3663 2024-05-14 14:16:53.284439 metals_api_zylalabs-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3556 2024-05-14 14:15:18.000000 metals_api_zylalabs-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 14:16:53.265133 metals_api_zylalabs-0.4/metals_api_zylalabs/
+-rw-rw-rw-   0        0        0       88 2024-05-13 19:50:11.000000 metals_api_zylalabs-0.4/metals_api_zylalabs/__init__.py
+-rw-rw-rw-   0        0        0      621 2024-05-13 19:49:31.000000 metals_api_zylalabs-0.4/metals_api_zylalabs/client.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:16:53.282138 metals_api_zylalabs-0.4/metals_api_zylalabs.egg-info/
+-rw-rw-rw-   0        0        0     3663 2024-05-14 14:16:53.000000 metals_api_zylalabs-0.4/metals_api_zylalabs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-14 14:16:53.000000 metals_api_zylalabs-0.4/metals_api_zylalabs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 14:16:53.000000 metals_api_zylalabs-0.4/metals_api_zylalabs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-14 14:16:53.000000 metals_api_zylalabs-0.4/metals_api_zylalabs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 14:16:53.286140 metals_api_zylalabs-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      333 2024-05-14 14:09:55.000000 metals_api_zylalabs-0.4/setup.py
```

### Comparing `metals_api_zylalabs-0.3/metals_api_zylalabs/client.py` & `metals_api_zylalabs-0.4/metals_api_zylalabs/client.py`

 * *Files identical despite different names*

