# Comparing `tmp/openinference_instrumentation-0.1.5.tar.gz` & `tmp/openinference_instrumentation-0.1.6.tar.gz`

## Comparing `openinference_instrumentation-0.1.5.tar` & `openinference_instrumentation-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10589 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.5/src/openinference/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.5/src/openinference/instrumentation/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.5/src/openinference/instrumentation/version.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.5/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.5/LICENSE
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.5/README.md
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/src/openinference/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/src/openinference/instrumentation/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/src/openinference/instrumentation/version.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/LICENSE
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/README.md
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 openinference_instrumentation-0.1.6/PKG-INFO
```

### Comparing `openinference_instrumentation-0.1.5/src/openinference/instrumentation/__init__.py` & `openinference_instrumentation-0.1.6/src/openinference/instrumentation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,20 @@
     get_current,
     get_value,
     set_value,
 )
 from opentelemetry.util.types import AttributeValue
 from typing_extensions import Self
 
+# The following line is needed to ensure that other modules using the
+# `openinference.instrumentation` path can be discovered by Bazel. For details,
+# see: https://github.com/Arize-ai/openinference/issues/398
+__path__ = __import__("pkgutil").extend_path(__path__, __name__)
+
+
 CONTEXT_ATTRIBUTES = (
     SpanAttributes.SESSION_ID,
     SpanAttributes.USER_ID,
     SpanAttributes.METADATA,
     SpanAttributes.TAG_TAGS,
     SpanAttributes.LLM_PROMPT_TEMPLATE,
     SpanAttributes.LLM_PROMPT_TEMPLATE_VERSION,
```

### Comparing `openinference_instrumentation-0.1.5/LICENSE` & `openinference_instrumentation-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation-0.1.5/pyproject.toml` & `openinference_instrumentation-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation-0.1.5/PKG-INFO` & `openinference_instrumentation-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation
-Version: 0.1.5
+Version: 0.1.6
 Summary: OpenInference instrumentation utilities
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/openinference-instrumentation
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

