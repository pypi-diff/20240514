# Comparing `tmp/confcls-0.0.1.tar.gz` & `tmp/confcls-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confcls-0.0.1.tar", max compression
+gzip compressed data, was "confcls-0.1.0.tar", max compression
```

## Comparing `confcls-0.0.1.tar` & `confcls-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0      187 2024-05-14 09:51:31.518086 confcls-0.0.1/confcls/__init__.py
--rw-r--r--   0        0        0     2352 2024-05-14 08:53:55.090298 confcls-0.0.1/confcls/configurable.py
--rw-r--r--   0        0        0      494 2024-05-14 14:44:48.827305 confcls-0.0.1/confcls/object.py
--rw-r--r--   0        0        0      495 2024-05-14 14:37:56.615389 confcls-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      615 2024-05-14 14:45:36.451057 confcls-0.0.1/setup.py
--rw-r--r--   0        0        0      346 2024-05-14 14:45:36.451234 confcls-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1480 2024-05-14 14:52:17.715267 confcls-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5233 2024-05-14 17:19:43.661312 confcls-0.1.0/README.md
+-rw-r--r--   0        0        0      187 2024-05-14 09:51:31.518086 confcls-0.1.0/confcls/__init__.py
+-rw-r--r--   0        0        0     2352 2024-05-14 08:53:55.090298 confcls-0.1.0/confcls/configurable.py
+-rw-r--r--   0        0        0      494 2024-05-14 14:44:48.827305 confcls-0.1.0/confcls/object.py
+-rw-r--r--   0        0        0      848 2024-05-14 17:32:10.808944 confcls-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6033 2024-05-14 17:34:09.155202 confcls-0.1.0/setup.py
+-rw-r--r--   0        0        0     5921 2024-05-14 17:34:09.155445 confcls-0.1.0/PKG-INFO
```

### Comparing `confcls-0.0.1/confcls/configurable.py` & `confcls-0.1.0/confcls/configurable.py`

 * *Files identical despite different names*

