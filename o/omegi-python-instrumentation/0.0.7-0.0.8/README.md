# Comparing `tmp/omegi_python_instrumentation-0.0.7.tar.gz` & `tmp/omegi-python-instrumentation-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi_python_instrumentation-0.0.7.tar", last modified: Mon May 13 04:24:35 2024, max compression
+gzip compressed data, was "omegi-python-instrumentation-0.0.8.tar", last modified: Tue May 14 07:28:02 2024, max compression
```

## Comparing `omegi_python_instrumentation-0.0.7.tar` & `omegi-python-instrumentation-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-13 04:24:35.441855 omegi_python_instrumentation-0.0.7/
--rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi_python_instrumentation-0.0.7/LICENSE.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-13 04:24:35.441666 omegi_python_instrumentation-0.0.7/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi_python_instrumentation-0.0.7/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi_python_instrumentation-0.0.7/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-13 04:24:35.441904 omegi_python_instrumentation-0.0.7/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2318 2024-05-13 04:22:13.000000 omegi_python_instrumentation-0.0.7/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-13 04:24:35.438914 omegi_python_instrumentation-0.0.7/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-13 04:24:35.440402 omegi_python_instrumentation-0.0.7/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1861 2024-05-12 16:36:10.000000 omegi_python_instrumentation-0.0.7/src/omegi/OmegiDecorator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     3085 2024-05-13 04:12:52.000000 omegi_python_instrumentation-0.0.7/src/omegi/OmegiSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2104 2024-05-13 03:46:40.000000 omegi_python_instrumentation-0.0.7/src/omegi/OmegiUtil.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      592 2024-05-13 04:18:09.000000 omegi_python_instrumentation-0.0.7/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-13 04:24:35.441383 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-13 04:24:35.000000 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      487 2024-05-13 04:24:35.000000 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-13 04:24:35.000000 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)       90 2024-05-13 04:24:35.000000 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/entry_points.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-13 04:24:35.000000 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-13 04:24:35.000000 omegi_python_instrumentation-0.0.7/src/omegi_python_instrumentation.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.474537 omegi-python-instrumentation-0.0.8/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi-python-instrumentation-0.0.8/LICENSE.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 07:28:02.474408 omegi-python-instrumentation-0.0.8/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi-python-instrumentation-0.0.8/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-python-instrumentation-0.0.8/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-14 07:28:02.474583 omegi-python-instrumentation-0.0.8/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2482 2024-05-14 07:28:00.000000 omegi-python-instrumentation-0.0.8/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.470813 omegi-python-instrumentation-0.0.8/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.471570 omegi-python-instrumentation-0.0.8/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2085 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.8/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.472032 omegi-python-instrumentation-0.0.8/src/omegi/decorator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-python-instrumentation-0.0.8/src/omegi/decorator/OmegiDecorator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-python-instrumentation-0.0.8/src/omegi/decorator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.472468 omegi-python-instrumentation-0.0.8/src/omegi/exporter/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1985 2024-05-14 07:22:33.000000 omegi-python-instrumentation-0.0.8/src/omegi/exporter/OmegiSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-python-instrumentation-0.0.8/src/omegi/exporter/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.473698 omegi-python-instrumentation-0.0.8/src/omegi/util/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1627 2024-05-14 01:15:00.000000 omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiDependencyInstrument.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2343 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiErrorSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiSamplerSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2120 2024-05-14 07:24:09.000000 omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiTracingSetup.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-python-instrumentation-0.0.8/src/omegi/util/UtilFunction.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-python-instrumentation-0.0.8/src/omegi/util/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:28:02.474232 omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      550 2024-05-14 07:28:02.000000 omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      711 2024-05-14 07:28:02.000000 omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-14 07:28:02.000000 omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1104 2024-05-14 07:28:02.000000 omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-14 07:28:02.000000 omegi-python-instrumentation-0.0.8/src/omegi_python_instrumentation.egg-info/top_level.txt
```

### Comparing `omegi_python_instrumentation-0.0.7/src/omegi/OmegiDecorator.py` & `omegi-python-instrumentation-0.0.8/src/omegi/decorator/OmegiDecorator.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,21 +3,28 @@
 import threading
 
 
 def omegi_decorator(tracer):
     def decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
-            print("IN TRACING DECORATOR", flush=True)
+            signature = inspect.signature(func)
+            bound_args = signature.bind(*args, **kwargs)
+            bound_args.apply_defaults()
+            arguments = []
+            for name, value in bound_args.arguments.items():
+                param = signature.parameters[name]
+                arg_type = param.annotation if param.annotation != inspect.Parameter.empty else type(value)
+                arguments.append(f"{name}: {arg_type.__name__} = {value}")
             with tracer.start_as_current_span(name=f"{func.__module__}.{func.__name__}") as span:
                 span.set_attribute("module", func.__module__)
                 span.set_attribute("name", func.__name__)
                 span.set_attribute("thread.name", threading.current_thread().name)
                 span.set_attribute("thread.id", threading.current_thread().ident)
-                span.set_attribute("arguments", str(inspect.signature(func).bind(*args, **kwargs).arguments))
+                span.set_attribute("arguments", arguments)
                 return func(*args, **kwargs)
         return wrapper
     return decorator
 
 
 def requests_omegi_decorator(tracer):
     def decorator(func):
```

### Comparing `omegi_python_instrumentation-0.0.7/src/omegi/OmegiUtil.py` & `omegi-python-instrumentation-0.0.8/src/omegi/util/OmegiTracingSetup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib
 import inspect
 import logging
 import os
 
-from .OmegiDecorator import omegi_decorator
+from omegi.decorator.OmegiDecorator import omegi_decorator
 
 
 def wrap_functions(tracer):
     logging.info("[OMEGIUTIL] wrap_functions: STARTED")
     for module_name in _get_project_modules(_find_project_root()):
         module = importlib.import_module(module_name)
         wrapped_functions = set()
@@ -42,8 +42,8 @@
         for file in files:
             if file.endswith('.py'):
                 module_path = os.path.relpath(os.path.join(root, file), project_root)
                 module_name = module_path.replace('/', '.').replace('\\', '.')[:-3]
                 if not module_path.startswith(".venv") and not module_path.startswith("omegi") and module_name != "omegi.OmegiUtil":
                     project_modules.append(module_name)
     logging.info(f"[OMEGIUTIL] _get_project_modules: ENDED -> {project_modules}")
-    return project_modules
+    return project_modules
```

