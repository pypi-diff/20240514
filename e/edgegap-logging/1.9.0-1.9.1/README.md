# Comparing `tmp/edgegap_logging-1.9.0.tar.gz` & `tmp/edgegap_logging-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_logging-1.9.0.tar", max compression
+gzip compressed data, was "edgegap_logging-1.9.1.tar", max compression
```

## Comparing `edgegap_logging-1.9.0.tar` & `edgegap_logging-1.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1993 2024-05-13 13:37:56.212217 edgegap_logging-1.9.0/LICENSE
--rw-r--r--   0        0        0     2216 2024-05-13 13:37:56.212217 edgegap_logging-1.9.0/README.md
--rw-r--r--   0        0        0      355 2024-05-13 13:37:56.212217 edgegap_logging-1.9.0/edgegap_logging/__init__.py
--rw-r--r--   0        0        0      847 2024-05-13 13:37:56.212217 edgegap_logging-1.9.0/edgegap_logging/_configuration.py
--rw-r--r--   0        0        0     1415 2024-05-13 13:37:56.212217 edgegap_logging-1.9.0/edgegap_logging/_context_logger.py
--rw-r--r--   0        0        0       17 2024-05-13 13:37:56.212217 edgegap_logging-1.9.0/edgegap_logging/_contexts/BUILD
--rw-r--r--   0        0        0       61 2024-05-13 13:37:56.212217 edgegap_logging-1.9.0/edgegap_logging/_contexts/__init__.py
--rw-r--r--   0        0        0       90 2024-05-13 13:37:56.212217 edgegap_logging-1.9.0/edgegap_logging/_contexts/_contexts.py
--rw-r--r--   0        0        0      942 2024-05-13 13:37:56.212217 edgegap_logging-1.9.0/edgegap_logging/_format.py
--rw-r--r--   0        0        0     1299 2024-05-13 13:37:56.212217 edgegap_logging-1.9.0/edgegap_logging/_logging.py
--rw-r--r--   0        0        0     1194 2024-05-13 13:37:56.212217 edgegap_logging-1.9.0/edgegap_logging/_v1_context_logger.py
--rw-r--r--   0        0        0      647 2024-05-13 13:38:57.309101 edgegap_logging-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 edgegap_logging-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-13 19:13:35.309563 edgegap_logging-1.9.1/LICENSE
+-rw-r--r--   0        0        0     2216 2024-05-13 19:13:35.309563 edgegap_logging-1.9.1/README.md
+-rw-r--r--   0        0        0      355 2024-05-13 19:13:35.309563 edgegap_logging-1.9.1/edgegap_logging/__init__.py
+-rw-r--r--   0        0        0      847 2024-05-13 19:13:35.309563 edgegap_logging-1.9.1/edgegap_logging/_configuration.py
+-rw-r--r--   0        0        0     1550 2024-05-13 19:13:35.309563 edgegap_logging-1.9.1/edgegap_logging/_context_logger.py
+-rw-r--r--   0        0        0       17 2024-05-13 19:13:35.309563 edgegap_logging-1.9.1/edgegap_logging/_contexts/BUILD
+-rw-r--r--   0        0        0       61 2024-05-13 19:13:35.309563 edgegap_logging-1.9.1/edgegap_logging/_contexts/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-13 19:13:35.309563 edgegap_logging-1.9.1/edgegap_logging/_contexts/_contexts.py
+-rw-r--r--   0        0        0      942 2024-05-13 19:13:35.309563 edgegap_logging-1.9.1/edgegap_logging/_format.py
+-rw-r--r--   0        0        0     1299 2024-05-13 19:13:35.309563 edgegap_logging-1.9.1/edgegap_logging/_logging.py
+-rw-r--r--   0        0        0     1327 2024-05-13 19:13:35.309563 edgegap_logging-1.9.1/edgegap_logging/_v1_context_logger.py
+-rw-r--r--   0        0        0      647 2024-05-13 19:13:52.353569 edgegap_logging-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 edgegap_logging-1.9.1/PKG-INFO
```

### Comparing `edgegap_logging-1.9.0/LICENSE` & `edgegap_logging-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.9.0/README.md` & `edgegap_logging-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.9.0/edgegap_logging/_configuration.py` & `edgegap_logging-1.9.1/edgegap_logging/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.9.0/edgegap_logging/_context_logger.py` & `edgegap_logging-1.9.1/edgegap_logging/_context_logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,7 +48,12 @@
         """
 
     @abstractmethod
     def critical(self, msg: str, **logger_kwargs):
         """
         This will log a critical message to the logger.
         """
+
+    def exception(self, msg: str, **logger_kwargs):
+        """
+        This will log an exception message to the logger.
+        """
```

### Comparing `edgegap_logging-1.9.0/edgegap_logging/_format.py` & `edgegap_logging-1.9.1/edgegap_logging/_format.py`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.9.0/edgegap_logging/_logging.py` & `edgegap_logging-1.9.1/edgegap_logging/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.9.0/edgegap_logging/_v1_context_logger.py` & `edgegap_logging-1.9.1/edgegap_logging/_v1_context_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,7 +27,10 @@
         self.__logger.warning(msg=msg, extra=self.__context, **logger_kwargs)
 
     def error(self, msg: str, **logger_kwargs):
         self.__logger.error(msg=msg, extra=self.__context, **logger_kwargs)
 
     def critical(self, msg: str, **logger_kwargs):
         self.__logger.critical(msg=msg, extra=self.__context, **logger_kwargs)
+
+    def exception(self, msg: str, **logger_kwargs):
+        self.__logger.exception(msg=msg, extra=self.__context, **logger_kwargs)
```

### Comparing `edgegap_logging-1.9.0/pyproject.toml` & `edgegap_logging-1.9.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-logging"
-version = "1.9.0"
+version = "1.9.1"
 description = "The Edgegap Logging library includes various tools and helpers for interacting with Standard Logging Formatter and Colored Logs. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 colorama = "^0.4.6"
```

### Comparing `edgegap_logging-1.9.0/PKG-INFO` & `edgegap_logging-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-logging
-Version: 1.9.0
+Version: 1.9.1
 Summary: The Edgegap Logging library includes various tools and helpers for interacting with Standard Logging Formatter and Colored Logs. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

