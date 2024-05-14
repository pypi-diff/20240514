# Comparing `tmp/bc_korea_vector_map-0.2.0.tar.gz` & `tmp/bc_korea_vector_map-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bc_korea_vector_map-0.2.0.tar", last modified: Tue May 14 12:47:20 2024, max compression
+gzip compressed data, was "bc_korea_vector_map-0.2.1.tar", last modified: Tue May 14 13:16:29 2024, max compression
```

## Comparing `bc_korea_vector_map-0.2.0.tar` & `bc_korea_vector_map-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 12:47:20.542533 bc_korea_vector_map-0.2.0/
--rw-rw-rw-   0        0        0     1086 2024-05-14 00:33:26.000000 bc_korea_vector_map-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      334 2024-05-14 12:47:20.541533 bc_korea_vector_map-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-14 12:27:45.000000 bc_korea_vector_map-0.2.0/README.md
--rw-rw-rw-   0        0        0      320 2024-05-14 12:46:10.000000 bc_korea_vector_map-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 12:47:20.543533 bc_korea_vector_map-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 12:47:20.515224 bc_korea_vector_map-0.2.0/src/
--rw-rw-rw-   0        0        0       47 2024-05-14 12:39:09.000000 bc_korea_vector_map-0.2.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:47:20.539533 bc_korea_vector_map-0.2.0/src/bc_korea_vector_map.egg-info/
--rw-rw-rw-   0        0        0      334 2024-05-14 12:47:20.000000 bc_korea_vector_map-0.2.0/src/bc_korea_vector_map.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-14 12:47:20.000000 bc_korea_vector_map-0.2.0/src/bc_korea_vector_map.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 12:47:20.000000 bc_korea_vector_map-0.2.0/src/bc_korea_vector_map.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-14 12:47:20.000000 bc_korea_vector_map-0.2.0/src/bc_korea_vector_map.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 13:16:29.073852 bc_korea_vector_map-0.2.1/
+-rw-rw-rw-   0        0        0     1086 2024-05-14 00:33:26.000000 bc_korea_vector_map-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      334 2024-05-14 13:16:29.070163 bc_korea_vector_map-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-14 12:27:45.000000 bc_korea_vector_map-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 13:16:29.047562 bc_korea_vector_map-0.2.1/bc_korea_vector_map/
+-rw-rw-rw-   0        0        0       47 2024-05-14 12:39:09.000000 bc_korea_vector_map-0.2.1/bc_korea_vector_map/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:16:29.068588 bc_korea_vector_map-0.2.1/bc_korea_vector_map.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-05-14 13:16:28.000000 bc_korea_vector_map-0.2.1/bc_korea_vector_map.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-14 13:16:29.000000 bc_korea_vector_map-0.2.1/bc_korea_vector_map.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 13:16:28.000000 bc_korea_vector_map-0.2.1/bc_korea_vector_map.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-14 13:16:28.000000 bc_korea_vector_map-0.2.1/bc_korea_vector_map.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      320 2024-05-14 13:14:41.000000 bc_korea_vector_map-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 13:16:29.074356 bc_korea_vector_map-0.2.1/setup.cfg
```

### Comparing `bc_korea_vector_map-0.2.0/LICENSE` & `bc_korea_vector_map-0.2.1/LICENSE`

 * *Files identical despite different names*

