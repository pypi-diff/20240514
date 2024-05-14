# Comparing `tmp/omegi-python-instrumentation-0.1.2.tar.gz` & `tmp/omegi-python-instrumentation-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi-python-instrumentation-0.1.2.tar", last modified: Tue May 14 08:36:16 2024, max compression
+gzip compressed data, was "omegi-python-instrumentation-0.1.3.tar", last modified: Tue May 14 08:46:17 2024, max compression
```

## Comparing `omegi-python-instrumentation-0.1.2.tar` & `omegi-python-instrumentation-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.013219 omegi-python-instrumentation-0.1.2/
--rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.1.2/LICENSE.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:36:16.013102 omegi-python-instrumentation-0.1.2/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.1.2/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.1.2/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 08:36:16.013267 omegi-python-instrumentation-0.1.2/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 08:36:05.000000 omegi-python-instrumentation-0.1.2/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.009454 omegi-python-instrumentation-0.1.2/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.010215 omegi-python-instrumentation-0.1.2/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2321 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.2/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.010670 omegi-python-instrumentation-0.1.2/src/omegi/decorator/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.1.2/src/omegi/decorator/OmegiDecorator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.1.2/src/omegi/decorator/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.010986 omegi-python-instrumentation-0.1.2/src/omegi/exporter/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2020 2024-05-14 08:04:27.000000 omegi-python-instrumentation-0.1.2/src/omegi/exporter/OmegiSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.1.2/src/omegi/exporter/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.012390 omegi-python-instrumentation-0.1.2/src/omegi/util/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1379 2024-05-14 08:35:26.000000 omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiDependencyInstrument.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiErrorSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiSamplerSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2126 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiTracingSetup.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.1.2/src/omegi/util/UtilFunction.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.1.2/src/omegi/util/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.012932 omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:36:15.000000 omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 08:36:15.000000 omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 08:36:15.000000 omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 08:36:15.000000 omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 08:36:15.000000 omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.652584 omegi-python-instrumentation-0.1.3/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.1.3/LICENSE.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:46:17.652448 omegi-python-instrumentation-0.1.3/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.1.3/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.1.3/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 08:46:17.652648 omegi-python-instrumentation-0.1.3/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 08:46:11.000000 omegi-python-instrumentation-0.1.3/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.648863 omegi-python-instrumentation-0.1.3/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.649702 omegi-python-instrumentation-0.1.3/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2321 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.3/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.650163 omegi-python-instrumentation-0.1.3/src/omegi/decorator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.1.3/src/omegi/decorator/OmegiDecorator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.1.3/src/omegi/decorator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.650493 omegi-python-instrumentation-0.1.3/src/omegi/exporter/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2020 2024-05-14 08:04:27.000000 omegi-python-instrumentation-0.1.3/src/omegi/exporter/OmegiSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.1.3/src/omegi/exporter/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.651757 omegi-python-instrumentation-0.1.3/src/omegi/util/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1379 2024-05-14 08:35:26.000000 omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiDependencyInstrument.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiErrorSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiSamplerSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2434 2024-05-14 08:45:58.000000 omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiTracingSetup.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.1.3/src/omegi/util/UtilFunction.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.1.3/src/omegi/util/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.652281 omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:46:17.000000 omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 08:46:17.000000 omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 08:46:17.000000 omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 08:46:17.000000 omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 08:46:17.000000 omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/top_level.txt
```

### Comparing `omegi-python-instrumentation-0.1.2/PKG-INFO` & `omegi-python-instrumentation-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi-python-instrumentation-0.1.2/setup.py` & `omegi-python-instrumentation-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="omegi-python-instrumentation",
-    version="0.1.2",
+    version="0.1.3",
     author="Omegi",
     author_email="canon1107@naver.com",
     description="Python Instrumentation for Automatic Error Logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TeamOmegi/Instrumentation-Python",
     project_urls={
```

### Comparing `omegi-python-instrumentation-0.1.2/src/omegi/__init__.py` & `omegi-python-instrumentation-0.1.3/src/omegi/__init__.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.2/src/omegi/decorator/OmegiDecorator.py` & `omegi-python-instrumentation-0.1.3/src/omegi/decorator/OmegiDecorator.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.2/src/omegi/exporter/OmegiSpanExporter.py` & `omegi-python-instrumentation-0.1.3/src/omegi/exporter/OmegiSpanExporter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiDependencyInstrument.py` & `omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiDependencyInstrument.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiErrorSpanFormatter.py` & `omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiErrorSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiSamplerSpanFormatter.py` & `omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiSamplerSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiTracingSetup.py` & `omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiTracingSetup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,23 @@
 import logging
 import os
 
 from omegi.decorator.OmegiDecorator import omegi_decorator
 
 
 def wrap_functions(tracer, project_root):
+    script_path = os.path.abspath(__file__)
+    script_dir = os.path.dirname(script_path)
+    temp_root = os.path.dirname(script_dir)
+    print("!!!!!!!!!!!!!!!!!", script_path, flush=True)
+    print("!!!!!!!!!!!!!!!!!", script_dir, flush=True)
+    print("!!!!!!!!!!!!!!!!!", temp_root, flush=True)
+
     logging.info("[OMEGIUTIL] wrap_functions: STARTED")
-    for module_name in _get_project_modules(project_root):
+    for module_name in _get_project_modules(_find_project_root()):
         module = importlib.import_module(module_name)
         wrapped_functions = set()
         for name, obj in inspect.getmembers(module):
             if inspect.isfunction(obj) :
                 if obj not in wrapped_functions:
                     logging.info(f"[OMEGIUTIL] wrap_functions: INPROGRESS -> wrapped module {module} {name}")
                     decorator = omegi_decorator(tracer)
```

### Comparing `omegi-python-instrumentation-0.1.2/src/omegi/util/UtilFunction.py` & `omegi-python-instrumentation-0.1.3/src/omegi/util/UtilFunction.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/PKG-INFO` & `omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/SOURCES.txt` & `omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/requires.txt` & `omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/requires.txt`

 * *Files identical despite different names*

