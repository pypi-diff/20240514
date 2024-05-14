# Comparing `tmp/omegi-python-instrumentation-0.0.9.tar.gz` & `tmp/omegi-python-instrumentation-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi-python-instrumentation-0.0.9.tar", last modified: Tue May 14 07:41:00 2024, max compression
+gzip compressed data, was "omegi-python-instrumentation-0.1.0.tar", last modified: Tue May 14 07:51:21 2024, max compression
```

## Comparing `omegi-python-instrumentation-0.0.9.tar` & `omegi-python-instrumentation-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.378965 omegi-python-instrumentation-0.0.9/
--rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.0.9/LICENSE.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 07:41:00.378845 omegi-python-instrumentation-0.0.9/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.0.9/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.0.9/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 07:41:00.379013 omegi-python-instrumentation-0.0.9/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 07:38:05.000000 omegi-python-instrumentation-0.0.9/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.375114 omegi-python-instrumentation-0.0.9/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.376051 omegi-python-instrumentation-0.0.9/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2130 2024-05-14 07:37:56.000000 omegi-python-instrumentation-0.0.9/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.376505 omegi-python-instrumentation-0.0.9/src/omegi/decorator/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.0.9/src/omegi/decorator/OmegiDecorator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.0.9/src/omegi/decorator/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.376906 omegi-python-instrumentation-0.0.9/src/omegi/exporter/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1985 2024-05-14 07:22:33.000000 omegi-python-instrumentation-0.0.9/src/omegi/exporter/OmegiSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.0.9/src/omegi/exporter/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.378064 omegi-python-instrumentation-0.0.9/src/omegi/util/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1627 2024-05-14 01:15:00.000000 omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiDependencyInstrument.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiErrorSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiSamplerSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2120 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiTracingSetup.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.0.9/src/omegi/util/UtilFunction.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.0.9/src/omegi/util/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.378658 omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 07:41:00.000000 omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 07:41:00.000000 omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 07:41:00.000000 omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 07:41:00.000000 omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 07:41:00.000000 omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.342616 omegi-python-instrumentation-0.1.0/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.1.0/LICENSE.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 07:51:21.342504 omegi-python-instrumentation-0.1.0/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.1.0/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.1.0/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 07:51:21.342652 omegi-python-instrumentation-0.1.0/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 07:51:08.000000 omegi-python-instrumentation-0.1.0/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.339145 omegi-python-instrumentation-0.1.0/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.339857 omegi-python-instrumentation-0.1.0/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2321 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.0/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.340190 omegi-python-instrumentation-0.1.0/src/omegi/decorator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.1.0/src/omegi/decorator/OmegiDecorator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.1.0/src/omegi/decorator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.340489 omegi-python-instrumentation-0.1.0/src/omegi/exporter/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1985 2024-05-14 07:22:33.000000 omegi-python-instrumentation-0.1.0/src/omegi/exporter/OmegiSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.1.0/src/omegi/exporter/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.341837 omegi-python-instrumentation-0.1.0/src/omegi/util/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1627 2024-05-14 01:15:00.000000 omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiDependencyInstrument.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiErrorSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiSamplerSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2126 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiTracingSetup.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.1.0/src/omegi/util/UtilFunction.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.1.0/src/omegi/util/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.342352 omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 07:51:21.000000 omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 07:51:21.000000 omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 07:51:21.000000 omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 07:51:21.000000 omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 07:51:21.000000 omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/top_level.txt
```

### Comparing `omegi-python-instrumentation-0.0.9/PKG-INFO` & `omegi-python-instrumentation-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi-python-instrumentation-0.0.9/setup.py` & `omegi-python-instrumentation-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="omegi-python-instrumentation",
-    version="0.0.9",
+    version="0.1.0",
     author="Omegi",
     author_email="canon1107@naver.com",
     description="Python Instrumentation for Automatic Error Logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TeamOmegi/Instrumentation-Python",
     project_urls={
```

### Comparing `omegi-python-instrumentation-0.0.9/src/omegi/__init__.py` & `omegi-python-instrumentation-0.1.0/src/omegi/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 from typing import Collection
 
 from opentelemetry import trace
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation.utils import unwrap
 from opentelemetry.sdk.resources import Resource
@@ -10,16 +11,17 @@
 
 from .exporter.OmegiSpanExporter import OmegiKafkaSpanExporter
 from .util.OmegiDependencyInstrument import instrument_dependencies
 from .util.OmegiTracingSetup import wrap_functions
 
 
 class OmegiInstrumentor(BaseInstrumentor):
-    def __init__(self, app=None):
+    def __init__(self, app=None, project_root=None):
         self.app = app
+        self.project_root = project_root
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return []
 
     def instrument(self):
         self._instrument()
 
@@ -31,26 +33,28 @@
         Kafka server urls can be figured through environment variables
         2. Figure Other Instrumentations
         By installed libraries this library detects fast api, django, flask, elasticsearch
         detected library's instrumentation is enabled automatically
         3. Set Function tracing
         detect module's functions and wrap it in decorator to enable tracing
         """
+        if self.project_root is None:
+            logging.error("Please set Project root")
         # Setup Custom Exporter, SpanProcessor
         custom_exporter = OmegiKafkaSpanExporter()
         span_processor = BatchSpanProcessor(custom_exporter)
         trace.set_tracer_provider(TracerProvider(
             resource=Resource.create({"service.name": os.getenv("OMEGI_SERVICE_NAME")}),
         ))
         trace.get_tracer_provider().add_span_processor(span_processor)
         tracer = trace.get_tracer(__name__)
         # Setup Instrumentations
         if self.app is not None:
             self._start_depending_instumentation(app=self.app)
         # Setup Tracing Functions
-        wrap_functions(tracer)
+        wrap_functions(tracer, self.project_root)
 
     def _uninstrument(self, **kwargs):
         return unwrap(kwargs)
 
     def _start_depending_instumentation(self, app):
-        instrument_dependencies(app)
+        instrument_dependencies(self.app)
```

### Comparing `omegi-python-instrumentation-0.0.9/src/omegi/decorator/OmegiDecorator.py` & `omegi-python-instrumentation-0.1.0/src/omegi/decorator/OmegiDecorator.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.9/src/omegi/exporter/OmegiSpanExporter.py` & `omegi-python-instrumentation-0.1.0/src/omegi/exporter/OmegiSpanExporter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiDependencyInstrument.py` & `omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiDependencyInstrument.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiErrorSpanFormatter.py` & `omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiErrorSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiSamplerSpanFormatter.py` & `omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiSamplerSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiTracingSetup.py` & `omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiTracingSetup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import inspect
 import logging
 import os
 
 from omegi.decorator.OmegiDecorator import omegi_decorator
 
 
-def wrap_functions(tracer):
+def wrap_functions(tracer, project_root):
     logging.info("[OMEGIUTIL] wrap_functions: STARTED")
-    for module_name in _get_project_modules(_find_project_root()):
+    for module_name in _get_project_modules(project_root):
         module = importlib.import_module(module_name)
         wrapped_functions = set()
         for name, obj in inspect.getmembers(module):
             if inspect.isfunction(obj) :
                 if obj not in wrapped_functions:
                     logging.info(f"[OMEGIUTIL] wrap_functions: INPROGRESS -> wrapped module {module} {name}")
                     decorator = omegi_decorator(tracer)
```

### Comparing `omegi-python-instrumentation-0.0.9/src/omegi/util/UtilFunction.py` & `omegi-python-instrumentation-0.1.0/src/omegi/util/UtilFunction.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/PKG-INFO` & `omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/SOURCES.txt` & `omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/requires.txt` & `omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/requires.txt`

 * *Files identical despite different names*

