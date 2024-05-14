# Comparing `tmp/omegi-python-instrumentation-0.0.8.tar.gz` & `tmp/omegi-python-instrumentation-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi-python-instrumentation-0.0.8.tar", last modified: Tue May 14 07:28:02 2024, max compression
+gzip compressed data, was "omegi-python-instrumentation-0.0.9.tar", last modified: Tue May 14 07:41:00 2024, max compression
```

## Comparing `omegi-python-instrumentation-0.0.8.tar` & `omegi-python-instrumentation-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.474537 omegi-python-instrumentation-0.0.8/
--rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.0.8/LICENSE.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 07:28:02.474408 omegi-python-instrumentation-0.0.8/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.0.8/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.0.8/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 07:28:02.474583 omegi-python-instrumentation-0.0.8/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 07:28:00.000000 omegi-python-instrumentation-0.0.8/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.470813 omegi-python-instrumentation-0.0.8/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.471570 omegi-python-instrumentation-0.0.8/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2085 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.8/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.472032 omegi-python-instrumentation-0.0.8/src/omegi/decorator/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.0.8/src/omegi/decorator/OmegiDecorator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.0.8/src/omegi/decorator/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.472468 omegi-python-instrumentation-0.0.8/src/omegi/exporter/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1985 2024-05-14 07:22:33.000000 omegi-python-instrumentation-0.0.8/src/omegi/exporter/OmegiSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.0.8/src/omegi/exporter/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.473698 omegi-python-instrumentation-0.0.8/src/omegi/util/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1627 2024-05-14 01:15:00.000000 omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiDependencyInstrument.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiErrorSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiSamplerSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2120 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiTracingSetup.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.0.8/src/omegi/util/UtilFunction.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.0.8/src/omegi/util/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.474232 omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 07:28:02.000000 omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 07:28:02.000000 omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 07:28:02.000000 omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 07:28:02.000000 omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 07:28:02.000000 omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.378965 omegi-python-instrumentation-0.0.9/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.0.9/LICENSE.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 07:41:00.378845 omegi-python-instrumentation-0.0.9/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.0.9/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.0.9/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 07:41:00.379013 omegi-python-instrumentation-0.0.9/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 07:38:05.000000 omegi-python-instrumentation-0.0.9/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.375114 omegi-python-instrumentation-0.0.9/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.376051 omegi-python-instrumentation-0.0.9/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2130 2024-05-14 07:37:56.000000 omegi-python-instrumentation-0.0.9/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.376505 omegi-python-instrumentation-0.0.9/src/omegi/decorator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.0.9/src/omegi/decorator/OmegiDecorator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.0.9/src/omegi/decorator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.376906 omegi-python-instrumentation-0.0.9/src/omegi/exporter/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1985 2024-05-14 07:22:33.000000 omegi-python-instrumentation-0.0.9/src/omegi/exporter/OmegiSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.0.9/src/omegi/exporter/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.378064 omegi-python-instrumentation-0.0.9/src/omegi/util/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1627 2024-05-14 01:15:00.000000 omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiDependencyInstrument.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiErrorSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiSamplerSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2120 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiTracingSetup.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.0.9/src/omegi/util/UtilFunction.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.0.9/src/omegi/util/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:41:00.378658 omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 07:41:00.000000 omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 07:41:00.000000 omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 07:41:00.000000 omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 07:41:00.000000 omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 07:41:00.000000 omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/top_level.txt
```

### Comparing `omegi-python-instrumentation-0.0.8/PKG-INFO` & `omegi-python-instrumentation-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi-python-instrumentation-0.0.8/setup.py` & `omegi-python-instrumentation-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="omegi-python-instrumentation",
-    version="0.0.8",
+    version="0.0.9",
     author="Omegi",
     author_email="canon1107@naver.com",
     description="Python Instrumentation for Automatic Error Logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TeamOmegi/Instrumentation-Python",
     project_urls={
```

### Comparing `omegi-python-instrumentation-0.0.8/src/omegi/__init__.py` & `omegi-python-instrumentation-0.0.9/src/omegi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 
 from .exporter.OmegiSpanExporter import OmegiKafkaSpanExporter
 from .util.OmegiDependencyInstrument import instrument_dependencies
 from .util.OmegiTracingSetup import wrap_functions
 
 
 class OmegiInstrumentor(BaseInstrumentor):
+    def __init__(self, app=None):
+        self.app = app
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return []
 
-    def instrument(self, app=None):
-        self._instrument(app=app)
+    def instrument(self):
+        self._instrument()
 
-    def _instrument(self, app):
+    def _instrument(self):
         """
         SETTING UP INSTRUMENTATION
         1. Figure Custom TraceExporter and SpanProcessor
         TraceExporter exports spans to Kafka.
         Kafka server urls can be figured through environment variables
         2. Figure Other Instrumentations
         By installed libraries this library detects fast api, django, flask, elasticsearch
@@ -38,16 +40,16 @@
         span_processor = BatchSpanProcessor(custom_exporter)
         trace.set_tracer_provider(TracerProvider(
             resource=Resource.create({"service.name": os.getenv("OMEGI_SERVICE_NAME")}),
         ))
         trace.get_tracer_provider().add_span_processor(span_processor)
         tracer = trace.get_tracer(__name__)
         # Setup Instrumentations
-        if app is not None:
-            self._start_depending_instumentation(app=app)
+        if self.app is not None:
+            self._start_depending_instumentation(app=self.app)
         # Setup Tracing Functions
         wrap_functions(tracer)
 
     def _uninstrument(self, **kwargs):
         return unwrap(kwargs)
 
     def _start_depending_instumentation(self, app):
```

### Comparing `omegi-python-instrumentation-0.0.8/src/omegi/decorator/OmegiDecorator.py` & `omegi-python-instrumentation-0.0.9/src/omegi/decorator/OmegiDecorator.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.8/src/omegi/exporter/OmegiSpanExporter.py` & `omegi-python-instrumentation-0.0.9/src/omegi/exporter/OmegiSpanExporter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiDependencyInstrument.py` & `omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiDependencyInstrument.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiErrorSpanFormatter.py` & `omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiErrorSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiSamplerSpanFormatter.py` & `omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiSamplerSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiTracingSetup.py` & `omegi-python-instrumentation-0.0.9/src/omegi/util/OmegiTracingSetup.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.8/src/omegi/util/UtilFunction.py` & `omegi-python-instrumentation-0.0.9/src/omegi/util/UtilFunction.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/PKG-INFO` & `omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/SOURCES.txt` & `omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/requires.txt` & `omegi-python-instrumentation-0.0.9/src/omegi_python_instrumentation.egg-info/requires.txt`

 * *Files identical despite different names*

