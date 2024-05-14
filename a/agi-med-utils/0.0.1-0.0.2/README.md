# Comparing `tmp/agi_med_utils-0.0.1.tar.gz` & `tmp/agi_med_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agi_med_utils-0.0.1.tar", last modified: Mon May 13 13:50:44 2024, max compression
+gzip compressed data, was "agi_med_utils-0.0.2.tar", last modified: Tue May 14 09:52:11 2024, max compression
```

## Comparing `agi_med_utils-0.0.1.tar` & `agi_med_utils-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 13:50:44.435187 agi_med_utils-0.0.1/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-05-13 08:33:25.000000 agi_med_utils-0.0.1/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      731 2024-05-13 13:50:44.435187 agi_med_utils-0.0.1/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      110 2024-05-13 08:25:13.000000 agi_med_utils-0.0.1/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 13:50:44.431187 agi_med_utils-0.0.1/agi_med_utils/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-13 08:38:18.000000 agi_med_utils-0.0.1/agi_med_utils/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-13 10:18:02.000000 agi_med_utils-0.0.1/agi_med_utils/abstract_client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 13:50:44.431187 agi_med_utils-0.0.1/agi_med_utils/config/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.1/agi_med_utils/config/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      523 2024-05-13 09:00:12.000000 agi_med_utils-0.0.1/agi_med_utils/config/config.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      232 2024-05-13 09:00:59.000000 agi_med_utils-0.0.1/agi_med_utils/config/singleton.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1280 2024-05-13 10:04:34.000000 agi_med_utils-0.0.1/agi_med_utils/errors.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 13:50:44.431187 agi_med_utils-0.0.1/agi_med_utils/llm/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.1/agi_med_utils/llm/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1212 2024-05-13 09:21:28.000000 agi_med_utils-0.0.1/agi_med_utils/llm/giga_access.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1519 2024-05-13 09:01:27.000000 agi_med_utils-0.0.1/agi_med_utils/llm/yandex_access.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 13:50:44.431187 agi_med_utils-0.0.1/agi_med_utils.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      731 2024-05-13 13:50:44.000000 agi_med_utils-0.0.1/agi_med_utils.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      510 2024-05-13 13:50:44.000000 agi_med_utils-0.0.1/agi_med_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-13 13:50:44.000000 agi_med_utils-0.0.1/agi_med_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      270 2024-05-13 13:50:44.000000 agi_med_utils-0.0.1/agi_med_utils.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       14 2024-05-13 13:50:44.000000 agi_med_utils-0.0.1/agi_med_utils.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      272 2024-05-13 13:47:34.000000 agi_med_utils-0.0.1/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-13 13:50:44.435187 agi_med_utils-0.0.1/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      778 2024-05-13 08:36:40.000000 agi_med_utils-0.0.1/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 09:52:11.215214 agi_med_utils-0.0.2/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-05-13 08:33:25.000000 agi_med_utils-0.0.2/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      348 2024-05-14 09:52:11.215214 agi_med_utils-0.0.2/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      110 2024-05-13 08:25:13.000000 agi_med_utils-0.0.2/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 09:52:11.215214 agi_med_utils-0.0.2/agi_med_utils/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-14 09:41:59.000000 agi_med_utils-0.0.2/agi_med_utils/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-13 10:18:02.000000 agi_med_utils-0.0.2/agi_med_utils/abstract_client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 09:52:11.215214 agi_med_utils-0.0.2/agi_med_utils/config/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.2/agi_med_utils/config/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      523 2024-05-13 09:00:12.000000 agi_med_utils-0.0.2/agi_med_utils/config/config.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      232 2024-05-13 09:00:59.000000 agi_med_utils-0.0.2/agi_med_utils/config/singleton.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 09:52:11.215214 agi_med_utils-0.0.2/agi_med_utils/llm/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.2/agi_med_utils/llm/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1212 2024-05-13 09:21:28.000000 agi_med_utils-0.0.2/agi_med_utils/llm/giga_access.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1519 2024-05-13 09:01:27.000000 agi_med_utils-0.0.2/agi_med_utils/llm/yandex_access.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 09:52:11.215214 agi_med_utils-0.0.2/agi_med_utils.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      348 2024-05-14 09:52:11.000000 agi_med_utils-0.0.2/agi_med_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      486 2024-05-14 09:52:11.000000 agi_med_utils-0.0.2/agi_med_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-14 09:52:11.000000 agi_med_utils-0.0.2/agi_med_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       67 2024-05-14 09:52:11.000000 agi_med_utils-0.0.2/agi_med_utils.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       14 2024-05-14 09:52:11.000000 agi_med_utils-0.0.2/agi_med_utils.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       70 2024-05-14 09:41:09.000000 agi_med_utils-0.0.2/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-14 09:52:11.215214 agi_med_utils-0.0.2/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      778 2024-05-13 08:36:40.000000 agi_med_utils-0.0.2/setup.py
```

### Comparing `agi_med_utils-0.0.1/agi_med_utils/config/config.py` & `agi_med_utils-0.0.2/agi_med_utils/config/config.py`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.1/agi_med_utils/llm/giga_access.py` & `agi_med_utils-0.0.2/agi_med_utils/llm/giga_access.py`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.1/agi_med_utils/llm/yandex_access.py` & `agi_med_utils-0.0.2/agi_med_utils/llm/yandex_access.py`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.1/setup.py` & `agi_med_utils-0.0.2/setup.py`

 * *Files identical despite different names*

