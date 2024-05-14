# Comparing `tmp/ousint-0.1.0.tar.gz` & `tmp/ousint-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ousint-0.1.0.tar", last modified: Mon May 13 23:59:34 2024, max compression
+gzip compressed data, was "ousint-0.2.tar", last modified: Tue May 14 00:06:11 2024, max compression
```

## Comparing `ousint-0.1.0.tar` & `ousint-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 23:59:34.373654 ousint-0.1.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     1065 2024-05-13 23:48:16.000000 ousint-0.1.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      313 2024-05-13 23:59:34.373654 ousint-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 23:59:34.369655 ousint-0.1.0/ousint/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-05-13 23:55:14.000000 ousint-0.1.0/ousint/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)       84 2024-05-13 23:55:35.000000 ousint-0.1.0/ousint/module.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 23:59:34.373654 ousint-0.1.0/ousint.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      313 2024-05-13 23:59:34.000000 ousint-0.1.0/ousint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      187 2024-05-13 23:59:34.000000 ousint-0.1.0/ousint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-13 23:59:34.000000 ousint-0.1.0/ousint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-05-13 23:59:34.000000 ousint-0.1.0/ousint.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      544 2024-04-11 15:38:22.000000 ousint-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-13 23:59:34.373654 ousint-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      407 2024-05-13 23:59:11.000000 ousint-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-14 00:06:11.725108 ousint-0.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1065 2024-05-13 23:48:16.000000 ousint-0.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      311 2024-05-14 00:06:11.725108 ousint-0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-14 00:06:11.721109 ousint-0.2/ousint/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-05-13 23:55:14.000000 ousint-0.2/ousint/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       84 2024-05-13 23:55:35.000000 ousint-0.2/ousint/module.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-14 00:06:11.725108 ousint-0.2/ousint.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      311 2024-05-14 00:06:11.000000 ousint-0.2/ousint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      187 2024-05-14 00:06:11.000000 ousint-0.2/ousint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-14 00:06:11.000000 ousint-0.2/ousint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-05-14 00:06:11.000000 ousint-0.2/ousint.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      535 2024-05-14 00:02:13.000000 ousint-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-14 00:06:11.725108 ousint-0.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      405 2024-05-14 00:04:43.000000 ousint-0.2/setup.py
```

### Comparing `ousint-0.1.0/LICENSE` & `ousint-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ousint-0.1.0/pyproject.toml` & `ousint-0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-name = "python-template"
+name = "ousint"
 version = "0.1.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<3.12"
```

