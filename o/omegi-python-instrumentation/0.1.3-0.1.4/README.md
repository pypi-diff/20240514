# Comparing `tmp/omegi-python-instrumentation-0.1.3.tar.gz` & `tmp/omegi-python-instrumentation-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi-python-instrumentation-0.1.3.tar", last modified: Tue May 14 08:46:17 2024, max compression
+gzip compressed data, was "omegi-python-instrumentation-0.1.4.tar", last modified: Tue May 14 08:53:12 2024, max compression
```

## Comparing `omegi-python-instrumentation-0.1.3.tar` & `omegi-python-instrumentation-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.652584 omegi-python-instrumentation-0.1.3/
--rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.1.3/LICENSE.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:46:17.652448 omegi-python-instrumentation-0.1.3/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.1.3/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.1.3/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 08:46:17.652648 omegi-python-instrumentation-0.1.3/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 08:46:11.000000 omegi-python-instrumentation-0.1.3/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.648863 omegi-python-instrumentation-0.1.3/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.649702 omegi-python-instrumentation-0.1.3/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2321 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.3/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.650163 omegi-python-instrumentation-0.1.3/src/omegi/decorator/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.1.3/src/omegi/decorator/OmegiDecorator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.1.3/src/omegi/decorator/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.650493 omegi-python-instrumentation-0.1.3/src/omegi/exporter/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2020 2024-05-14 08:04:27.000000 omegi-python-instrumentation-0.1.3/src/omegi/exporter/OmegiSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.1.3/src/omegi/exporter/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.651757 omegi-python-instrumentation-0.1.3/src/omegi/util/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1379 2024-05-14 08:35:26.000000 omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiDependencyInstrument.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiErrorSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiSamplerSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2434 2024-05-14 08:45:58.000000 omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiTracingSetup.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.1.3/src/omegi/util/UtilFunction.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.1.3/src/omegi/util/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:46:17.652281 omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:46:17.000000 omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 08:46:17.000000 omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 08:46:17.000000 omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 08:46:17.000000 omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 08:46:17.000000 omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:53:12.130993 omegi-python-instrumentation-0.1.4/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.1.4/LICENSE.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:53:12.130870 omegi-python-instrumentation-0.1.4/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.1.4/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.1.4/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 08:53:12.131035 omegi-python-instrumentation-0.1.4/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 08:51:07.000000 omegi-python-instrumentation-0.1.4/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:53:12.126736 omegi-python-instrumentation-0.1.4/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:53:12.127545 omegi-python-instrumentation-0.1.4/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2329 2024-05-14 08:52:40.000000 omegi-python-instrumentation-0.1.4/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:53:12.128099 omegi-python-instrumentation-0.1.4/src/omegi/decorator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.1.4/src/omegi/decorator/OmegiDecorator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.1.4/src/omegi/decorator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:53:12.128507 omegi-python-instrumentation-0.1.4/src/omegi/exporter/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2020 2024-05-14 08:04:27.000000 omegi-python-instrumentation-0.1.4/src/omegi/exporter/OmegiSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.1.4/src/omegi/exporter/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:53:12.129917 omegi-python-instrumentation-0.1.4/src/omegi/util/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1379 2024-05-14 08:35:26.000000 omegi-python-instrumentation-0.1.4/src/omegi/util/OmegiDependencyInstrument.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.4/src/omegi/util/OmegiErrorSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.4/src/omegi/util/OmegiSamplerSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1529 2024-05-14 08:52:40.000000 omegi-python-instrumentation-0.1.4/src/omegi/util/OmegiTracingSetup.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.1.4/src/omegi/util/UtilFunction.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.1.4/src/omegi/util/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:53:12.130695 omegi-python-instrumentation-0.1.4/src/omegi_python_instrumentation.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:53:12.000000 omegi-python-instrumentation-0.1.4/src/omegi_python_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 08:53:12.000000 omegi-python-instrumentation-0.1.4/src/omegi_python_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 08:53:12.000000 omegi-python-instrumentation-0.1.4/src/omegi_python_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 08:53:12.000000 omegi-python-instrumentation-0.1.4/src/omegi_python_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 08:53:12.000000 omegi-python-instrumentation-0.1.4/src/omegi_python_instrumentation.egg-info/top_level.txt
```

### Comparing `omegi-python-instrumentation-0.1.3/PKG-INFO` & `omegi-python-instrumentation-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi-python-instrumentation-0.1.3/setup.py` & `omegi-python-instrumentation-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="omegi-python-instrumentation",
-    version="0.1.3",
+    version="0.1.4",
     author="Omegi",
     author_email="canon1107@naver.com",
     description="Python Instrumentation for Automatic Error Logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TeamOmegi/Instrumentation-Python",
     project_urls={
```

### Comparing `omegi-python-instrumentation-0.1.3/src/omegi/__init__.py` & `omegi-python-instrumentation-0.1.4/src/omegi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 from .exporter.OmegiSpanExporter import OmegiKafkaSpanExporter
 from .util.OmegiDependencyInstrument import instrument_dependencies
 from .util.OmegiTracingSetup import wrap_functions
 
 
 class OmegiInstrumentor(BaseInstrumentor):
-    def __init__(self, app=None, project_root=None):
+    def __init__(self, app=None):
         self.app = app
-        self.project_root = project_root
+        self.project_root = os.getenv("OMEGI_PROJECT_ROOT", "/app")
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return []
 
     def instrument(self):
         self._instrument()
```

### Comparing `omegi-python-instrumentation-0.1.3/src/omegi/decorator/OmegiDecorator.py` & `omegi-python-instrumentation-0.1.4/src/omegi/decorator/OmegiDecorator.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.3/src/omegi/exporter/OmegiSpanExporter.py` & `omegi-python-instrumentation-0.1.4/src/omegi/exporter/OmegiSpanExporter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiDependencyInstrument.py` & `omegi-python-instrumentation-0.1.4/src/omegi/util/OmegiDependencyInstrument.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiErrorSpanFormatter.py` & `omegi-python-instrumentation-0.1.4/src/omegi/util/OmegiErrorSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.3/src/omegi/util/OmegiSamplerSpanFormatter.py` & `omegi-python-instrumentation-0.1.4/src/omegi/util/OmegiSamplerSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.3/src/omegi/util/UtilFunction.py` & `omegi-python-instrumentation-0.1.4/src/omegi/util/UtilFunction.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/PKG-INFO` & `omegi-python-instrumentation-0.1.4/src/omegi_python_instrumentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/SOURCES.txt` & `omegi-python-instrumentation-0.1.4/src/omegi_python_instrumentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.3/src/omegi_python_instrumentation.egg-info/requires.txt` & `omegi-python-instrumentation-0.1.4/src/omegi_python_instrumentation.egg-info/requires.txt`

 * *Files identical despite different names*

