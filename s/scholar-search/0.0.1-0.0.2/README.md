# Comparing `tmp/scholar_search-0.0.1.tar.gz` & `tmp/scholar_search-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scholar_search-0.0.1.tar", last modified: Mon May 13 05:05:01 2024, max compression
+gzip compressed data, was "scholar_search-0.0.2.tar", last modified: Tue May 14 03:44:57 2024, max compression
```

## Comparing `scholar_search-0.0.1.tar` & `scholar_search-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 aemiller   (501) staff       (20)        0 2024-05-13 05:05:01.298503 scholar_search-0.0.1/
--rw-r--r--   0 aemiller   (501) staff       (20)     1068 2024-05-13 05:00:43.000000 scholar_search-0.0.1/LICENSE
--rw-r--r--   0 aemiller   (501) staff       (20)      787 2024-05-13 05:05:01.298306 scholar_search-0.0.1/PKG-INFO
--rw-r--r--   0 aemiller   (501) staff       (20)    10456 2024-05-13 04:54:33.000000 scholar_search-0.0.1/README.md
--rw-r--r--   0 aemiller   (501) staff       (20)       81 2024-05-12 21:23:20.000000 scholar_search-0.0.1/pyproject.toml
-drwxr-xr-x   0 aemiller   (501) staff       (20)        0 2024-05-13 05:05:01.297068 scholar_search-0.0.1/sch/
--rw-r--r--   0 aemiller   (501) staff       (20)     3093 2024-05-13 04:49:40.000000 scholar_search-0.0.1/sch/__init__.py
--rw-r--r--   0 aemiller   (501) staff       (20)     2215 2024-05-13 04:56:29.000000 scholar_search-0.0.1/sch/cli.py
--rw-r--r--   0 aemiller   (501) staff       (20)    27354 2024-05-11 14:46:29.000000 scholar_search-0.0.1/sch/commands.py
--rw-r--r--   0 aemiller   (501) staff       (20)      123 2024-05-13 03:00:35.000000 scholar_search-0.0.1/sch/errors.py
--rw-r--r--   0 aemiller   (501) staff       (20)     6921 2024-05-11 17:41:15.000000 scholar_search-0.0.1/sch/readme.py
--rw-r--r--   0 aemiller   (501) staff       (20)    21932 2024-05-13 02:26:28.000000 scholar_search-0.0.1/sch/server.py
--rw-r--r--   0 aemiller   (501) staff       (20)     3978 2024-05-12 00:17:25.000000 scholar_search-0.0.1/sch/utils.py
-drwxr-xr-x   0 aemiller   (501) staff       (20)        0 2024-05-13 05:05:01.298113 scholar_search-0.0.1/scholar_search.egg-info/
--rw-r--r--   0 aemiller   (501) staff       (20)      787 2024-05-13 05:05:01.000000 scholar_search-0.0.1/scholar_search.egg-info/PKG-INFO
--rw-r--r--   0 aemiller   (501) staff       (20)      369 2024-05-13 05:05:01.000000 scholar_search-0.0.1/scholar_search.egg-info/SOURCES.txt
--rw-r--r--   0 aemiller   (501) staff       (20)        1 2024-05-13 05:05:01.000000 scholar_search-0.0.1/scholar_search.egg-info/dependency_links.txt
--rw-r--r--   0 aemiller   (501) staff       (20)       36 2024-05-13 05:05:01.000000 scholar_search-0.0.1/scholar_search.egg-info/entry_points.txt
--rw-r--r--   0 aemiller   (501) staff       (20)       29 2024-05-13 05:05:01.000000 scholar_search-0.0.1/scholar_search.egg-info/requires.txt
--rw-r--r--   0 aemiller   (501) staff       (20)        4 2024-05-13 05:05:01.000000 scholar_search-0.0.1/scholar_search.egg-info/top_level.txt
--rw-r--r--   0 aemiller   (501) staff       (20)       38 2024-05-13 05:05:01.298543 scholar_search-0.0.1/setup.cfg
--rw-r--r--   0 aemiller   (501) staff       (20)     1045 2024-05-13 04:55:57.000000 scholar_search-0.0.1/setup.py
+drwxr-xr-x   0 aemiller   (501) staff       (20)        0 2024-05-14 03:44:57.306104 scholar_search-0.0.2/
+-rw-r--r--   0 aemiller   (501) staff       (20)     1068 2024-05-14 03:44:09.000000 scholar_search-0.0.2/LICENSE
+-rw-r--r--   0 aemiller   (501) staff       (20)      860 2024-05-14 03:44:57.305921 scholar_search-0.0.2/PKG-INFO
+-rw-r--r--   0 aemiller   (501) staff       (20)    10847 2024-05-14 03:44:09.000000 scholar_search-0.0.2/README.md
+-rw-r--r--   0 aemiller   (501) staff       (20)       81 2024-05-14 03:44:09.000000 scholar_search-0.0.2/pyproject.toml
+drwxr-xr-x   0 aemiller   (501) staff       (20)        0 2024-05-14 03:44:57.304606 scholar_search-0.0.2/sch/
+-rw-r--r--   0 aemiller   (501) staff       (20)     3093 2024-05-14 03:44:09.000000 scholar_search-0.0.2/sch/__init__.py
+-rw-r--r--   0 aemiller   (501) staff       (20)     2215 2024-05-14 03:44:09.000000 scholar_search-0.0.2/sch/cli.py
+-rw-r--r--   0 aemiller   (501) staff       (20)    27384 2024-05-14 03:44:09.000000 scholar_search-0.0.2/sch/commands.py
+-rw-r--r--   0 aemiller   (501) staff       (20)      123 2024-05-14 03:44:09.000000 scholar_search-0.0.2/sch/errors.py
+-rw-r--r--   0 aemiller   (501) staff       (20)     6921 2024-05-14 03:44:09.000000 scholar_search-0.0.2/sch/readme.py
+-rw-r--r--   0 aemiller   (501) staff       (20)    21932 2024-05-14 03:44:09.000000 scholar_search-0.0.2/sch/server.py
+-rw-r--r--   0 aemiller   (501) staff       (20)     3978 2024-05-14 03:44:09.000000 scholar_search-0.0.2/sch/utils.py
+drwxr-xr-x   0 aemiller   (501) staff       (20)        0 2024-05-14 03:44:57.305632 scholar_search-0.0.2/scholar_search.egg-info/
+-rw-r--r--   0 aemiller   (501) staff       (20)      860 2024-05-14 03:44:57.000000 scholar_search-0.0.2/scholar_search.egg-info/PKG-INFO
+-rw-r--r--   0 aemiller   (501) staff       (20)      369 2024-05-14 03:44:57.000000 scholar_search-0.0.2/scholar_search.egg-info/SOURCES.txt
+-rw-r--r--   0 aemiller   (501) staff       (20)        1 2024-05-14 03:44:57.000000 scholar_search-0.0.2/scholar_search.egg-info/dependency_links.txt
+-rw-r--r--   0 aemiller   (501) staff       (20)       36 2024-05-14 03:44:57.000000 scholar_search-0.0.2/scholar_search.egg-info/entry_points.txt
+-rw-r--r--   0 aemiller   (501) staff       (20)       55 2024-05-14 03:44:57.000000 scholar_search-0.0.2/scholar_search.egg-info/requires.txt
+-rw-r--r--   0 aemiller   (501) staff       (20)        4 2024-05-14 03:44:57.000000 scholar_search-0.0.2/scholar_search.egg-info/top_level.txt
+-rw-r--r--   0 aemiller   (501) staff       (20)       38 2024-05-14 03:44:57.306145 scholar_search-0.0.2/setup.cfg
+-rw-r--r--   0 aemiller   (501) staff       (20)     1097 2024-05-14 03:44:24.000000 scholar_search-0.0.2/setup.py
```

### Comparing `scholar_search-0.0.1/LICENSE` & `scholar_search-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scholar_search-0.0.1/sch/__init__.py` & `scholar_search-0.0.2/sch/__init__.py`

 * *Files identical despite different names*

### Comparing `scholar_search-0.0.1/sch/cli.py` & `scholar_search-0.0.2/sch/cli.py`

 * *Files identical despite different names*

### Comparing `scholar_search-0.0.1/sch/commands.py` & `scholar_search-0.0.2/sch/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,17 @@
         # so that args start at the correct color offset from the command.
         for i, param in enumerate(sig.parameters.values(), self.depth + 1):
             depth_color = COLOR_WHEEL.get(i).value
             node_color = f"{{.{depth_color}}}"
             colored_sig_parts.append(f"`{str(param)}`{node_color}")
 
         return (
-            "(" + ", ".join(colored_sig_parts) + f") -> `{retval}`{{.{RETURN_COLOR}}}"
+            "("
+            + ", ".join(colored_sig_parts)
+            + f") -> `{retval}`{{.{RETURN_COLOR.value}}}"
         )
 
     @property
     def docstring(self) -> str:
         command_help = getdoc(self.command_func)
         if command_help:
             # "Re-pad" the newlines to be indented forward 4 spaces, after they
```

### Comparing `scholar_search-0.0.1/sch/readme.py` & `scholar_search-0.0.2/sch/readme.py`

 * *Files identical despite different names*

### Comparing `scholar_search-0.0.1/sch/server.py` & `scholar_search-0.0.2/sch/server.py`

 * *Files identical despite different names*

### Comparing `scholar_search-0.0.1/sch/utils.py` & `scholar_search-0.0.2/sch/utils.py`

 * *Files identical despite different names*

### Comparing `scholar_search-0.0.1/setup.py` & `scholar_search-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import setup, find_packages
 
 setup(
     name="scholar-search",
-    version="0.0.1",
+    version="0.0.2",
     license="MIT",
     description="a macro search bar",
     author="Adam Miller",
     author_email="miller@adammiller.io",
     url="https://github.com/adammillerio/sch",
     download_url="https://github.com/adammillerio/sch/archive/v0.0.1.tar.gz",
     keywords=[],
@@ -25,12 +25,13 @@
     include_package_data=True,
     install_requires=[
         "anytree",
         "flask",
         "click",
         "pypandoc",
     ],
+    extras_require={"pandoc": ["pypandoc-binary"]},
     entry_points="""
     [console_scripts]
     sch=sch.cli:sch
   """,
 )
```

