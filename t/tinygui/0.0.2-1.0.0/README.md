# Comparing `tmp/tinygui-0.0.2.tar.gz` & `tmp/tinygui-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinygui-0.0.2.tar", last modified: Mon May 13 07:14:20 2024, max compression
+gzip compressed data, was "tinygui-1.0.0.tar", last modified: Thu Mar 14 06:37:43 2024, max compression
```

## Comparing `tinygui-0.0.2.tar` & `tinygui-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 07:14:20.409894 tinygui-0.0.2/
--rw-rw-rw-   0        0        0     1093 2024-05-13 06:57:47.000000 tinygui-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      511 2024-05-13 07:14:20.407896 tinygui-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      620 2024-05-13 07:13:51.000000 tinygui-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 07:14:20.409894 tinygui-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 07:14:20.379503 tinygui-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 07:14:20.386933 tinygui-0.0.2/src/tinygui/
--rw-rw-rw-   0        0        0       21 2024-04-29 06:18:32.000000 tinygui-0.0.2/src/tinygui/__init__.py
--rw-rw-rw-   0        0        0     1269 2024-04-29 06:18:32.000000 tinygui-0.0.2/src/tinygui/tinygui.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:14:20.406893 tinygui-0.0.2/src/tinygui.egg-info/
--rw-rw-rw-   0        0        0      511 2024-05-13 07:14:20.000000 tinygui-0.0.2/src/tinygui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-05-13 07:14:20.000000 tinygui-0.0.2/src/tinygui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 07:14:20.000000 tinygui-0.0.2/src/tinygui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 07:14:20.000000 tinygui-0.0.2/src/tinygui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-14 06:37:43.850327 tinygui-1.0.0/
+-rw-rw-rw-   0        0        0     1093 2024-01-17 07:33:18.000000 tinygui-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      503 2024-03-14 06:37:43.848331 tinygui-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2024-03-14 06:30:58.000000 tinygui-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-14 06:37:43.850368 tinygui-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-14 06:37:43.814422 tinygui-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-03-14 06:37:43.822410 tinygui-1.0.0/src/tinygui/
+-rw-rw-rw-   0        0        0       21 2024-03-14 06:29:18.000000 tinygui-1.0.0/src/tinygui/__init__.py
+-rw-rw-rw-   0        0        0     1269 2024-03-14 06:30:58.000000 tinygui-1.0.0/src/tinygui/tinygui.py
+drwxrwxrwx   0        0        0        0 2024-03-14 06:37:43.847334 tinygui-1.0.0/src/tinygui.egg-info/
+-rw-rw-rw-   0        0        0      503 2024-03-14 06:37:43.000000 tinygui-1.0.0/src/tinygui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-03-14 06:37:43.000000 tinygui-1.0.0/src/tinygui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-14 06:37:43.000000 tinygui-1.0.0/src/tinygui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-03-14 06:37:43.000000 tinygui-1.0.0/src/tinygui.egg-info/top_level.txt
```

### Comparing `tinygui-0.0.2/LICENSE` & `tinygui-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinygui-0.0.2/pyproject.toml` & `tinygui-1.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "tinygui"
-version = "0.0.2"
+version = "1.0.0"
 authors = [
   { name = "xiaoheli", email = "1173324325@qq.com" },
 ]
 dependencies = []
-description = "A small example package for gui"
+description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `tinygui-0.0.2/src/tinygui/tinygui.py` & `tinygui-1.0.0/src/tinygui/tinygui.py`

 * *Files identical despite different names*

