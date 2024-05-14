# Comparing `tmp/omegi-python-instrumentation-0.1.0.tar.gz` & `tmp/omegi-python-instrumentation-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi-python-instrumentation-0.1.0.tar", last modified: Tue May 14 07:51:21 2024, max compression
+gzip compressed data, was "omegi-python-instrumentation-0.1.1.tar", last modified: Tue May 14 08:04:36 2024, max compression
```

## Comparing `omegi-python-instrumentation-0.1.0.tar` & `omegi-python-instrumentation-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.342616 omegi-python-instrumentation-0.1.0/
--rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.1.0/LICENSE.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 07:51:21.342504 omegi-python-instrumentation-0.1.0/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.1.0/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.1.0/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 07:51:21.342652 omegi-python-instrumentation-0.1.0/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 07:51:08.000000 omegi-python-instrumentation-0.1.0/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.339145 omegi-python-instrumentation-0.1.0/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.339857 omegi-python-instrumentation-0.1.0/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2321 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.0/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.340190 omegi-python-instrumentation-0.1.0/src/omegi/decorator/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.1.0/src/omegi/decorator/OmegiDecorator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.1.0/src/omegi/decorator/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.340489 omegi-python-instrumentation-0.1.0/src/omegi/exporter/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1985 2024-05-14 07:22:33.000000 omegi-python-instrumentation-0.1.0/src/omegi/exporter/OmegiSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.1.0/src/omegi/exporter/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.341837 omegi-python-instrumentation-0.1.0/src/omegi/util/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1627 2024-05-14 01:15:00.000000 omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiDependencyInstrument.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiErrorSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiSamplerSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2126 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiTracingSetup.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.1.0/src/omegi/util/UtilFunction.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.1.0/src/omegi/util/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:51:21.342352 omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 07:51:21.000000 omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 07:51:21.000000 omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 07:51:21.000000 omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 07:51:21.000000 omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 07:51:21.000000 omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.139507 omegi-python-instrumentation-0.1.1/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.1.1/LICENSE.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:04:36.139387 omegi-python-instrumentation-0.1.1/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.1.1/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.1.1/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 08:04:36.139548 omegi-python-instrumentation-0.1.1/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 08:04:27.000000 omegi-python-instrumentation-0.1.1/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.135845 omegi-python-instrumentation-0.1.1/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.136585 omegi-python-instrumentation-0.1.1/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2321 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.1/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.137030 omegi-python-instrumentation-0.1.1/src/omegi/decorator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.1.1/src/omegi/decorator/OmegiDecorator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.1.1/src/omegi/decorator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.137230 omegi-python-instrumentation-0.1.1/src/omegi/exporter/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2020 2024-05-14 08:04:27.000000 omegi-python-instrumentation-0.1.1/src/omegi/exporter/OmegiSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.1.1/src/omegi/exporter/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.138689 omegi-python-instrumentation-0.1.1/src/omegi/util/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1627 2024-05-14 01:15:00.000000 omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiDependencyInstrument.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiErrorSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiSamplerSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2126 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiTracingSetup.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.1.1/src/omegi/util/UtilFunction.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.1.1/src/omegi/util/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.139229 omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:04:36.000000 omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 08:04:36.000000 omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 08:04:36.000000 omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 08:04:36.000000 omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 08:04:36.000000 omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/top_level.txt
```

### Comparing `omegi-python-instrumentation-0.1.0/PKG-INFO` & `omegi-python-instrumentation-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi-python-instrumentation-0.1.0/setup.py` & `omegi-python-instrumentation-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="omegi-python-instrumentation",
-    version="0.1.0",
+    version="0.1.1",
     author="Omegi",
     author_email="canon1107@naver.com",
     description="Python Instrumentation for Automatic Error Logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TeamOmegi/Instrumentation-Python",
     project_urls={
```

### Comparing `omegi-python-instrumentation-0.1.0/src/omegi/__init__.py` & `omegi-python-instrumentation-0.1.1/src/omegi/__init__.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.0/src/omegi/decorator/OmegiDecorator.py` & `omegi-python-instrumentation-0.1.1/src/omegi/decorator/OmegiDecorator.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.0/src/omegi/exporter/OmegiSpanExporter.py` & `omegi-python-instrumentation-0.1.1/src/omegi/exporter/OmegiSpanExporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 from typing import Sequence
 
+from kafka import KafkaProducer
 from opentelemetry.sdk.trace.export import SpanExporter
 from opentelemetry.trace import Span, StatusCode
 
 from omegi.util.OmegiErrorSpanFormatter import format_error_spans
 from omegi.util.OmegiSamplerSpanFormatter import format_sampler_spans
 from omegi.util.UtilFunction import decide_export
 
@@ -13,15 +14,15 @@
 class OmegiKafkaSpanExporter(SpanExporter):
     def __init__(self):
         self.kafka_servers = os.environ.get('OMEGI_KAFKA_CONFIG', 'localhost:9092').split(',')
         self.error_topic = os.environ.get('OMEGI_KAFKA_TOPIC_ERROR', 'error')
         self.flow_topic = os.environ.get('OMEGI_KAFKA_TOPIC_FLOW', 'flow')
         self.token = os.environ.get('OMEGI_TOKEN', "your_token")
         self.flow_rate = 1 / int(os.environ.get('OMEGI_FLOW_RATE', 5))
-        # self.producer = KafkaProducer(bootstrap_servers=kafka_servers)
+        self.producer = KafkaProducer(bootstrap_servers=self.kafka_servers)
 
     def export(self, spans: Sequence[Span]):
         self._process_sampler_spans(spans)
         self._process_error_spans(spans)
 
     def _process_sampler_spans(self, spans: Sequence[Span]):
         if decide_export(spans[0].get_span_context().trace_id, rate=self.flow_rate):
```

### Comparing `omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiDependencyInstrument.py` & `omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiDependencyInstrument.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiErrorSpanFormatter.py` & `omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiErrorSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiSamplerSpanFormatter.py` & `omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiSamplerSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.0/src/omegi/util/OmegiTracingSetup.py` & `omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiTracingSetup.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.0/src/omegi/util/UtilFunction.py` & `omegi-python-instrumentation-0.1.1/src/omegi/util/UtilFunction.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/PKG-INFO` & `omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/SOURCES.txt` & `omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.0/src/omegi_python_instrumentation.egg-info/requires.txt` & `omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/requires.txt`

 * *Files identical despite different names*

