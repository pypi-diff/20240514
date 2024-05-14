# Comparing `tmp/omegi-python-instrumentation-0.1.1.tar.gz` & `tmp/omegi-python-instrumentation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi-python-instrumentation-0.1.1.tar", last modified: Tue May 14 08:04:36 2024, max compression
+gzip compressed data, was "omegi-python-instrumentation-0.1.2.tar", last modified: Tue May 14 08:36:16 2024, max compression
```

## Comparing `omegi-python-instrumentation-0.1.1.tar` & `omegi-python-instrumentation-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.139507 omegi-python-instrumentation-0.1.1/
--rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.1.1/LICENSE.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:04:36.139387 omegi-python-instrumentation-0.1.1/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.1.1/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.1.1/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 08:04:36.139548 omegi-python-instrumentation-0.1.1/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 08:04:27.000000 omegi-python-instrumentation-0.1.1/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.135845 omegi-python-instrumentation-0.1.1/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.136585 omegi-python-instrumentation-0.1.1/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2321 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.1/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.137030 omegi-python-instrumentation-0.1.1/src/omegi/decorator/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.1.1/src/omegi/decorator/OmegiDecorator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.1.1/src/omegi/decorator/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.137230 omegi-python-instrumentation-0.1.1/src/omegi/exporter/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2020 2024-05-14 08:04:27.000000 omegi-python-instrumentation-0.1.1/src/omegi/exporter/OmegiSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.1.1/src/omegi/exporter/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.138689 omegi-python-instrumentation-0.1.1/src/omegi/util/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1627 2024-05-14 01:15:00.000000 omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiDependencyInstrument.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiErrorSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiSamplerSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2126 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiTracingSetup.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.1.1/src/omegi/util/UtilFunction.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.1.1/src/omegi/util/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:04:36.139229 omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:04:36.000000 omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 08:04:36.000000 omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 08:04:36.000000 omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 08:04:36.000000 omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 08:04:36.000000 omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.013219 omegi-python-instrumentation-0.1.2/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.1.2/LICENSE.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:36:16.013102 omegi-python-instrumentation-0.1.2/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.1.2/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.1.2/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 08:36:16.013267 omegi-python-instrumentation-0.1.2/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 08:36:05.000000 omegi-python-instrumentation-0.1.2/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.009454 omegi-python-instrumentation-0.1.2/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.010215 omegi-python-instrumentation-0.1.2/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2321 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.2/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.010670 omegi-python-instrumentation-0.1.2/src/omegi/decorator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.1.2/src/omegi/decorator/OmegiDecorator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.1.2/src/omegi/decorator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.010986 omegi-python-instrumentation-0.1.2/src/omegi/exporter/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2020 2024-05-14 08:04:27.000000 omegi-python-instrumentation-0.1.2/src/omegi/exporter/OmegiSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.1.2/src/omegi/exporter/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.012390 omegi-python-instrumentation-0.1.2/src/omegi/util/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1379 2024-05-14 08:35:26.000000 omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiDependencyInstrument.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiErrorSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiSamplerSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2126 2024-05-14 07:50:48.000000 omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiTracingSetup.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.1.2/src/omegi/util/UtilFunction.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.1.2/src/omegi/util/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 08:36:16.012932 omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 08:36:15.000000 omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 08:36:15.000000 omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 08:36:15.000000 omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 08:36:15.000000 omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 08:36:15.000000 omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/top_level.txt
```

### Comparing `omegi-python-instrumentation-0.1.1/PKG-INFO` & `omegi-python-instrumentation-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi-python-instrumentation-0.1.1/setup.py` & `omegi-python-instrumentation-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="omegi-python-instrumentation",
-    version="0.1.1",
+    version="0.1.2",
     author="Omegi",
     author_email="canon1107@naver.com",
     description="Python Instrumentation for Automatic Error Logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TeamOmegi/Instrumentation-Python",
     project_urls={
```

### Comparing `omegi-python-instrumentation-0.1.1/src/omegi/__init__.py` & `omegi-python-instrumentation-0.1.2/src/omegi/__init__.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.1/src/omegi/decorator/OmegiDecorator.py` & `omegi-python-instrumentation-0.1.2/src/omegi/decorator/OmegiDecorator.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.1/src/omegi/exporter/OmegiSpanExporter.py` & `omegi-python-instrumentation-0.1.2/src/omegi/exporter/OmegiSpanExporter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiErrorSpanFormatter.py` & `omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiErrorSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiSamplerSpanFormatter.py` & `omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiSamplerSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.1/src/omegi/util/OmegiTracingSetup.py` & `omegi-python-instrumentation-0.1.2/src/omegi/util/OmegiTracingSetup.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.1/src/omegi/util/UtilFunction.py` & `omegi-python-instrumentation-0.1.2/src/omegi/util/UtilFunction.py`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/PKG-INFO` & `omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/SOURCES.txt` & `omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omegi-python-instrumentation-0.1.1/src/omegi_python_instrumentation.egg-info/requires.txt` & `omegi-python-instrumentation-0.1.2/src/omegi_python_instrumentation.egg-info/requires.txt`

 * *Files identical despite different names*

