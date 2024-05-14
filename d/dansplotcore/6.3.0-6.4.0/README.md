# Comparing `tmp/dansplotcore-6.3.0.tar.gz` & `tmp/dansplotcore-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dansplotcore-6.3.0.tar", last modified: Mon May 13 23:47:15 2024, max compression
+gzip compressed data, was "dansplotcore-6.4.0.tar", last modified: Tue May 14 19:12:35 2024, max compression
```

## Comparing `dansplotcore-6.3.0.tar` & `dansplotcore-6.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-13 23:47:15.649371 dansplotcore-6.3.0/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-13 23:47:15.649371 dansplotcore-6.3.0/PKG-INFO
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-13 23:47:15.649371 dansplotcore-6.3.0/dansplotcore/
--rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.3.0/dansplotcore/__init__.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.3.0/dansplotcore/media.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9713 2024-05-13 23:40:36.000000 dansplotcore-6.3.0/dansplotcore/plot.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.3.0/dansplotcore/primitives.py
--rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.3.0/dansplotcore/process.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9612 2024-05-13 23:31:06.000000 dansplotcore-6.3.0/dansplotcore/show.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.3.0/dansplotcore/transforms.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.3.0/dansplotcore/vector_text.py
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-13 23:47:15.649371 dansplotcore-6.3.0/dansplotcore.egg-info/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-13 23:47:15.000000 dansplotcore-6.3.0/dansplotcore.egg-info/PKG-INFO
--rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-05-13 23:47:15.000000 dansplotcore-6.3.0/dansplotcore.egg-info/SOURCES.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-05-13 23:47:15.000000 dansplotcore-6.3.0/dansplotcore.egg-info/dependency_links.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-05-13 23:47:15.000000 dansplotcore-6.3.0/dansplotcore.egg-info/requires.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-05-13 23:47:15.000000 dansplotcore-6.3.0/dansplotcore.egg-info/top_level.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-05-13 23:47:15.649371 dansplotcore-6.3.0/setup.cfg
--rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-05-13 23:45:54.000000 dansplotcore-6.3.0/setup.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-14 19:12:35.643064 dansplotcore-6.4.0/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-14 19:12:35.643064 dansplotcore-6.4.0/PKG-INFO
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-14 19:12:35.643064 dansplotcore-6.4.0/dansplotcore/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.4.0/dansplotcore/__init__.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.4.0/dansplotcore/media.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9713 2024-05-13 23:40:36.000000 dansplotcore-6.4.0/dansplotcore/plot.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.4.0/dansplotcore/primitives.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2208 2024-05-14 19:02:20.000000 dansplotcore-6.4.0/dansplotcore/process.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9612 2024-05-13 23:31:06.000000 dansplotcore-6.4.0/dansplotcore/show.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.4.0/dansplotcore/transforms.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.4.0/dansplotcore/vector_text.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-14 19:12:35.643064 dansplotcore-6.4.0/dansplotcore.egg-info/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-14 19:12:35.000000 dansplotcore-6.4.0/dansplotcore.egg-info/PKG-INFO
+-rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-05-14 19:12:35.000000 dansplotcore-6.4.0/dansplotcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-05-14 19:12:35.000000 dansplotcore-6.4.0/dansplotcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-05-14 19:12:35.000000 dansplotcore-6.4.0/dansplotcore.egg-info/requires.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-05-14 19:12:35.000000 dansplotcore-6.4.0/dansplotcore.egg-info/top_level.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-05-14 19:12:35.643064 dansplotcore-6.4.0/setup.cfg
+-rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-05-14 19:12:14.000000 dansplotcore-6.4.0/setup.py
```

### Comparing `dansplotcore-6.3.0/dansplotcore/media.py` & `dansplotcore-6.4.0/dansplotcore/media.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.3.0/dansplotcore/plot.py` & `dansplotcore-6.4.0/dansplotcore/plot.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.3.0/dansplotcore/primitives.py` & `dansplotcore-6.4.0/dansplotcore/primitives.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.3.0/dansplotcore/show.py` & `dansplotcore-6.4.0/dansplotcore/show.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.3.0/dansplotcore/transforms.py` & `dansplotcore-6.4.0/dansplotcore/transforms.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.3.0/dansplotcore/vector_text.py` & `dansplotcore-6.4.0/dansplotcore/vector_text.py`

 * *Files identical despite different names*

