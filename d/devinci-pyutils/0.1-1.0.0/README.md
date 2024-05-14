# Comparing `tmp/devinci_pyutils-0.1.tar.gz` & `tmp/devinci_pyutils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devinci_pyutils-0.1.tar", last modified: Tue May  7 02:50:20 2024, max compression
+gzip compressed data, was "devinci_pyutils-1.0.0.tar", last modified: Tue May 14 09:18:34 2024, max compression
```

## Comparing `devinci_pyutils-0.1.tar` & `devinci_pyutils-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,26 @@
-drwxr-xr-x   0 vince     (1001) vince     (1001)        0 2024-05-07 02:50:20.588016 devinci_pyutils-0.1/
--rw-r--r--   0 vince     (1001) vince     (1001)     2375 2024-05-07 02:50:20.584015 devinci_pyutils-0.1/PKG-INFO
--rw-r--r--   0 vince     (1001) vince     (1001)     2080 2024-05-07 01:23:59.000000 devinci_pyutils-0.1/README.md
-drwxr-xr-x   0 vince     (1001) vince     (1001)        0 2024-05-07 02:50:20.584015 devinci_pyutils-0.1/devinci_pyutils/
--rw-r--r--   0 vince     (1001) vince     (1001)      158 2024-05-07 02:46:36.000000 devinci_pyutils-0.1/devinci_pyutils/__init__.py
--rw-r--r--   0 vince     (1001) vince     (1001)     1947 2024-05-07 01:23:59.000000 devinci_pyutils-0.1/devinci_pyutils/banner.py
--rw-r--r--   0 vince     (1001) vince     (1001)     1425 2024-05-07 01:39:22.000000 devinci_pyutils-0.1/devinci_pyutils/file_utils.py
--rw-r--r--   0 vince     (1001) vince     (1001)     1333 2024-05-07 01:23:59.000000 devinci_pyutils-0.1/devinci_pyutils/writer.py
-drwxr-xr-x   0 vince     (1001) vince     (1001)        0 2024-05-07 02:50:20.584015 devinci_pyutils-0.1/devinci_pyutils.egg-info/
--rw-r--r--   0 vince     (1001) vince     (1001)     2375 2024-05-07 02:50:20.000000 devinci_pyutils-0.1/devinci_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 vince     (1001) vince     (1001)      284 2024-05-07 02:50:20.000000 devinci_pyutils-0.1/devinci_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 vince     (1001) vince     (1001)        1 2024-05-07 02:50:20.000000 devinci_pyutils-0.1/devinci_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 vince     (1001) vince     (1001)       16 2024-05-07 02:50:20.000000 devinci_pyutils-0.1/devinci_pyutils.egg-info/top_level.txt
--rw-r--r--   0 vince     (1001) vince     (1001)       38 2024-05-07 02:50:20.588016 devinci_pyutils-0.1/setup.cfg
--rw-r--r--   0 vince     (1001) vince     (1001)      499 2024-05-07 02:50:16.000000 devinci_pyutils-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:18:34.221076 devinci_pyutils-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-14 09:18:34.221076 devinci_pyutils-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:18:34.217076 devinci_pyutils-1.0.0/devinci_pyutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/devinci_pyutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/devinci_pyutils/banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/devinci_pyutils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/devinci_pyutils/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/devinci_pyutils/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:18:34.221076 devinci_pyutils-1.0.0/devinci_pyutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-14 09:18:34.000000 devinci_pyutils-1.0.0/devinci_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-14 09:18:34.000000 devinci_pyutils-1.0.0/devinci_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:18:34.000000 devinci_pyutils-1.0.0/devinci_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 09:18:34.000000 devinci_pyutils-1.0.0/devinci_pyutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:18:34.217076 devinci_pyutils-1.0.0/py_scaffold/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/py_scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/py_scaffold/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/py_scaffold/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/py_scaffold/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:18:34.217076 devinci_pyutils-1.0.0/py_scaffold/stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/py_scaffold/stubs/_class.stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/py_scaffold/stubs/_wiki.stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-14 09:18:28.000000 devinci_pyutils-1.0.0/py_scaffold/template_hydrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:18:34.221076 devinci_pyutils-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-14 09:18:33.000000 devinci_pyutils-1.0.0/setup.py
```

### Comparing `devinci_pyutils-0.1/PKG-INFO` & `devinci_pyutils-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devinci-pyutils
-Version: 0.1
+Version: 1.0.0
 Summary: Collection of Python utility modules for developers.
 Home-page: https://gist.github.com/devinci-it/d432708e796d6e6160efe13ee6cc7bbc/
 Author: devinci-it
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `devinci_pyutils-0.1/README.md` & `devinci_pyutils-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `devinci_pyutils-0.1/devinci_pyutils/banner.py` & `devinci_pyutils-1.0.0/devinci_pyutils/banner.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,7 +42,8 @@
         raise ValueError("Invalid alignment. Options: 'left', 'center', 'right'.")
 
     if newline:
         print(border)
     print(banner_text)
     if newline:
         print(border)
+
```

### Comparing `devinci_pyutils-0.1/devinci_pyutils/file_utils.py` & `devinci_pyutils-1.0.0/devinci_pyutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `devinci_pyutils-0.1/devinci_pyutils/writer.py` & `devinci_pyutils-1.0.0/devinci_pyutils/writer.py`

 * *Files identical despite different names*

### Comparing `devinci_pyutils-0.1/devinci_pyutils.egg-info/PKG-INFO` & `devinci_pyutils-1.0.0/devinci_pyutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devinci-pyutils
-Version: 0.1
+Version: 1.0.0
 Summary: Collection of Python utility modules for developers.
 Home-page: https://gist.github.com/devinci-it/d432708e796d6e6160efe13ee6cc7bbc/
 Author: devinci-it
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

