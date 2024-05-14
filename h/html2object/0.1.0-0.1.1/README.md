# Comparing `tmp/html2object-0.1.0.tar.gz` & `tmp/html2object-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2object-0.1.0.tar", last modified: Tue May 14 19:14:32 2024, max compression
+gzip compressed data, was "html2object-0.1.1.tar", last modified: Tue May 14 19:45:50 2024, max compression
```

## Comparing `html2object-0.1.0.tar` & `html2object-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 boterop   (1000) boterop   (1000)        0 2024-05-14 19:14:32.738246 html2object-0.1.0/
--rw-rw-r--   0 boterop   (1000) boterop   (1000)     1064 2024-05-14 18:49:20.000000 html2object-0.1.0/LICENSE
--rw-r--r--   0 boterop   (1000) boterop   (1000)     1920 2024-05-14 19:14:32.738246 html2object-0.1.0/PKG-INFO
--rw-rw-r--   0 boterop   (1000) boterop   (1000)      939 2024-05-14 18:48:34.000000 html2object-0.1.0/README.md
-drwxrwxr-x   0 boterop   (1000) boterop   (1000)        0 2024-05-14 19:14:32.738246 html2object-0.1.0/html2object.egg-info/
--rw-r--r--   0 boterop   (1000) boterop   (1000)     1920 2024-05-14 19:14:32.000000 html2object-0.1.0/html2object.egg-info/PKG-INFO
--rw-rw-r--   0 boterop   (1000) boterop   (1000)      211 2024-05-14 19:14:32.000000 html2object-0.1.0/html2object.egg-info/SOURCES.txt
--rw-rw-r--   0 boterop   (1000) boterop   (1000)        1 2024-05-14 19:14:32.000000 html2object-0.1.0/html2object.egg-info/dependency_links.txt
--rw-rw-r--   0 boterop   (1000) boterop   (1000)        6 2024-05-14 19:14:32.000000 html2object-0.1.0/html2object.egg-info/top_level.txt
--rw-rw-r--   0 boterop   (1000) boterop   (1000)       38 2024-05-14 19:14:32.738246 html2object-0.1.0/setup.cfg
--rw-rw-r--   0 boterop   (1000) boterop   (1000)     1182 2024-05-14 19:13:23.000000 html2object-0.1.0/setup.py
-drwxrwxr-x   0 boterop   (1000) boterop   (1000)        0 2024-05-14 19:14:32.738246 html2object-0.1.0/tests/
--rw-rw-r--   0 boterop   (1000) boterop   (1000)        0 2024-05-14 16:56:04.000000 html2object-0.1.0/tests/__init__.py
--rw-rw-r--   0 boterop   (1000) boterop   (1000)     2688 2024-05-14 17:09:59.000000 html2object-0.1.0/tests/test_html_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:45:50.202280 html2object-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 19:45:41.000000 html2object-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-14 19:45:50.202280 html2object-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-14 19:45:41.000000 html2object-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:45:50.202280 html2object-0.1.1/html2object.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-14 19:45:50.000000 html2object-0.1.1/html2object.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-14 19:45:50.000000 html2object-0.1.1/html2object.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:45:50.000000 html2object-0.1.1/html2object.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 19:45:50.000000 html2object-0.1.1/html2object.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:45:50.202280 html2object-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-14 19:45:41.000000 html2object-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:45:50.202280 html2object-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:45:41.000000 html2object-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-14 19:45:41.000000 html2object-0.1.1/tests/test_html_element.py
```

### Comparing `html2object-0.1.0/LICENSE` & `html2object-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `html2object-0.1.0/setup.py` & `html2object-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name="html2object",
-    version="0.1.0",
+    version="0.1.1",
     author="boterop",
     author_email="boterop22@gmail.com",
     description="Tools to handle the CRUD of .html files as objects.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    url="https://github.com/boterop/html_utils",
+    url="https://github.com/boterop/html2object",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.12",
     ],
-    keywords="html, utils, html_utils, html_element, html_parser, html_writer, html_reader, html_crud, html_object, html_file, html_utils.py, html_element.py, html_parser.py, html_writer.py, html_reader.py, html_crud.py, html_object.py, html_file.py",
+    keywords="html, utils, html_utils, html_element, html_parser, html_writer, html_reader, html_crud, html_object, html_file, html_utils.py, html_element.py, html_parser.py, html_writer.py, html_reader.py, html_crud.py, html_object.py, html_file.py, html2object, html2object.py, html2object.py",
     install_requires=[],
     python_requires=">=3.6",
 )
```

### Comparing `html2object-0.1.0/tests/test_html_element.py` & `html2object-0.1.1/tests/test_html_element.py`

 * *Files identical despite different names*

