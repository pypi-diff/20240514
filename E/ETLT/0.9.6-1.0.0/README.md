# Comparing `tmp/ETLT-0.9.6.tar.gz` & `tmp/etlt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ETLT-0.9.6.tar", last modified: Mon Oct 26 17:10:57 2020, max compression
+gzip compressed data, was "etlt-1.0.0.tar", max compression
```

## Comparing `ETLT-0.9.6.tar` & `etlt-1.0.0.tar`

### file list

```diff
@@ -1,66 +1,38 @@
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.191696 ETLT-0.9.6/
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.184696 ETLT-0.9.6/ETLT.egg-info/
--rw-rw-r--   0 water     (1000) water     (1000)     4536 2020-10-26 17:10:57.000000 ETLT-0.9.6/ETLT.egg-info/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)     1501 2020-10-26 17:10:57.000000 ETLT-0.9.6/ETLT.egg-info/SOURCES.txt
--rw-rw-r--   0 water     (1000) water     (1000)        1 2020-10-26 17:10:57.000000 ETLT-0.9.6/ETLT.egg-info/dependency_links.txt
--rw-rw-r--   0 water     (1000) water     (1000)       18 2020-10-26 17:10:57.000000 ETLT-0.9.6/ETLT.egg-info/requires.txt
--rw-rw-r--   0 water     (1000) water     (1000)       10 2020-10-26 17:10:57.000000 ETLT-0.9.6/ETLT.egg-info/top_level.txt
--rw-rw-r--   0 water     (1000) water     (1000)     4536 2020-10-26 17:10:57.190696 ETLT-0.9.6/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)     3646 2020-04-20 02:17:41.000000 ETLT-0.9.6/README.rst
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.184696 ETLT-0.9.6/etlt/
--rw-rw-r--   0 water     (1000) water     (1000)    12953 2020-10-26 16:47:21.000000 ETLT-0.9.6/etlt/Transformer.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-0.9.6/etlt/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.185696 ETLT-0.9.6/etlt/cleaner/
--rw-rw-r--   0 water     (1000) water     (1000)     3366 2020-10-26 16:51:42.000000 ETLT-0.9.6/etlt/cleaner/DateCleaner.py
--rw-rw-r--   0 water     (1000) water     (1000)     1412 2020-10-26 16:56:27.000000 ETLT-0.9.6/etlt/cleaner/MoneyCleaner.py
--rw-rw-r--   0 water     (1000) water     (1000)      711 2020-10-26 16:51:42.000000 ETLT-0.9.6/etlt/cleaner/WhitespaceCleaner.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-0.9.6/etlt/cleaner/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.186696 ETLT-0.9.6/etlt/condition/
--rw-rw-r--   0 water     (1000) water     (1000)      786 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/condition/AndCondition.py
--rw-rw-r--   0 water     (1000) water     (1000)     1085 2020-10-26 16:54:55.000000 ETLT-0.9.6/etlt/condition/CompoundCondition.py
--rw-rw-r--   0 water     (1000) water     (1000)      606 2020-10-26 16:37:24.000000 ETLT-0.9.6/etlt/condition/Condition.py
--rw-rw-r--   0 water     (1000) water     (1000)      827 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/condition/FalseCondition.py
--rw-rw-r--   0 water     (1000) water     (1000)      990 2020-10-26 16:37:24.000000 ETLT-0.9.6/etlt/condition/GlobCondition.py
--rw-rw-r--   0 water     (1000) water     (1000)     2573 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/condition/InListCondition.py
--rw-rw-r--   0 water     (1000) water     (1000)      799 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/condition/OrCondition.py
--rw-rw-r--   0 water     (1000) water     (1000)      950 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/condition/PlainCondition.py
--rw-rw-r--   0 water     (1000) water     (1000)     1058 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/condition/RegularExpressionCondition.py
--rw-rw-r--   0 water     (1000) water     (1000)     1849 2020-10-26 16:55:07.000000 ETLT-0.9.6/etlt/condition/SimpleCondition.py
--rw-rw-r--   0 water     (1000) water     (1000)     2892 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/condition/SimpleConditionFactory.py
--rw-rw-r--   0 water     (1000) water     (1000)      820 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/condition/TrueCondition.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-0.9.6/etlt/condition/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.186696 ETLT-0.9.6/etlt/dimension/
--rw-rw-r--   0 water     (1000) water     (1000)     3767 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/dimension/RegularDimension.py
--rw-rw-r--   0 water     (1000) water     (1000)     5399 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/dimension/Type2ReferenceDimension.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-0.9.6/etlt/dimension/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.187696 ETLT-0.9.6/etlt/helper/
--rw-rw-r--   0 water     (1000) water     (1000)     2063 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/helper/Allen.py
--rw-rw-r--   0 water     (1000) water     (1000)     6008 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/helper/Type2CondenseHelper.py
--rw-rw-r--   0 water     (1000) water     (1000)    14097 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/helper/Type2Helper.py
--rw-rw-r--   0 water     (1000) water     (1000)     4436 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/helper/Type2JoinHelper.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-0.9.6/etlt/helper/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.187696 ETLT-0.9.6/etlt/reader/
--rw-rw-r--   0 water     (1000) water     (1000)     2470 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/reader/Reader.py
--rw-rw-r--   0 water     (1000) water     (1000)     8309 2020-10-26 16:37:24.000000 ETLT-0.9.6/etlt/reader/UniversalCsvReader.py
--rw-rw-r--   0 water     (1000) water     (1000)     2354 2020-10-26 16:37:24.000000 ETLT-0.9.6/etlt/reader/UniversalCsvReaderFormatHelper.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-0.9.6/etlt/reader/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.188696 ETLT-0.9.6/etlt/writer/
--rw-rw-r--   0 water     (1000) water     (1000)     3790 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/writer/SqlLoaderWriter.py
--rw-rw-r--   0 water     (1000) water     (1000)     1972 2020-10-26 16:37:23.000000 ETLT-0.9.6/etlt/writer/Writer.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-0.9.6/etlt/writer/__init__.py
--rw-rw-r--   0 water     (1000) water     (1000)       38 2020-10-26 17:10:57.191696 ETLT-0.9.6/setup.cfg
--rw-rw-r--   0 water     (1000) water     (1000)     1147 2020-10-26 17:10:48.000000 ETLT-0.9.6/setup.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.184696 ETLT-0.9.6/test/
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.188696 ETLT-0.9.6/test/cleaner/
--rw-rw-r--   0 water     (1000) water     (1000)     5789 2019-04-10 09:59:04.000000 ETLT-0.9.6/test/cleaner/DateCleanerTest.py
--rw-rw-r--   0 water     (1000) water     (1000)     2686 2020-09-11 04:34:12.000000 ETLT-0.9.6/test/cleaner/MoneyCleanerTest.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-0.9.6/test/cleaner/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.188696 ETLT-0.9.6/test/condition/
--rw-rw-r--   0 water     (1000) water     (1000)     1544 2016-08-10 19:51:04.000000 ETLT-0.9.6/test/condition/InListConditionTest.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-0.9.6/test/condition/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:10:57.190696 ETLT-0.9.6/test/helper/
--rw-rw-r--   0 water     (1000) water     (1000)     2762 2016-08-14 12:39:39.000000 ETLT-0.9.6/test/helper/AllenTest.py
--rw-rw-r--   0 water     (1000) water     (1000)    23092 2016-08-15 08:08:46.000000 ETLT-0.9.6/test/helper/Type2CondenseHelperTest.py
--rw-rw-r--   0 water     (1000) water     (1000)     3124 2016-08-16 08:16:29.000000 ETLT-0.9.6/test/helper/Type2HelperTest.py
--rwxrwxrwx   0 water     (1000) water     (1000)    33380 2016-08-14 14:29:48.000000 ETLT-0.9.6/test/helper/Type2JoinHelperTest.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-0.9.6/test/helper/__init__.py
+-rw-r--r--   0        0        0     1092 2016-06-20 04:53:11.000000 etlt-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1375 2024-05-14 04:40:10.082282 etlt-1.0.0/README.md
+-rw-r--r--   0        0        0    14343 2024-05-14 03:04:51.489643 etlt-1.0.0/etlt/Transformer.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:29.000000 etlt-1.0.0/etlt/__init__.py
+-rw-r--r--   0        0        0     4315 2024-05-14 03:04:51.481643 etlt-1.0.0/etlt/cleaner/DateCleaner.py
+-rw-r--r--   0        0        0     1541 2024-05-14 03:10:10.778591 etlt-1.0.0/etlt/cleaner/MoneyCleaner.py
+-rw-r--r--   0        0        0      686 2024-05-14 02:08:01.276425 etlt-1.0.0/etlt/cleaner/WhitespaceCleaner.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:29.000000 etlt-1.0.0/etlt/cleaner/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-14 02:10:57.483263 etlt-1.0.0/etlt/condition/AndCondition.py
+-rw-r--r--   0        0        0     1065 2024-05-14 02:08:01.229424 etlt-1.0.0/etlt/condition/CompoundCondition.py
+-rw-r--r--   0        0        0      632 2024-05-14 02:08:01.290425 etlt-1.0.0/etlt/condition/Condition.py
+-rw-r--r--   0        0        0      840 2024-05-14 02:10:57.465263 etlt-1.0.0/etlt/condition/FalseCondition.py
+-rw-r--r--   0        0        0      982 2024-05-14 02:20:43.302026 etlt-1.0.0/etlt/condition/GlobCondition.py
+-rw-r--r--   0        0        0     2565 2024-05-14 02:20:43.035020 etlt-1.0.0/etlt/condition/InListCondition.py
+-rw-r--r--   0        0        0      831 2024-05-14 02:20:43.313026 etlt-1.0.0/etlt/condition/OrCondition.py
+-rw-r--r--   0        0        0      963 2024-05-14 02:20:43.309026 etlt-1.0.0/etlt/condition/PlainCondition.py
+-rw-r--r--   0        0        0     1070 2024-05-14 02:20:43.307026 etlt-1.0.0/etlt/condition/RegularExpressionCondition.py
+-rw-r--r--   0        0        0     1779 2024-05-14 02:20:43.317026 etlt-1.0.0/etlt/condition/SimpleCondition.py
+-rw-r--r--   0        0        0     2968 2024-05-14 02:20:43.305026 etlt-1.0.0/etlt/condition/SimpleConditionFactory.py
+-rw-r--r--   0        0        0      838 2024-05-14 02:20:43.315026 etlt-1.0.0/etlt/condition/TrueCondition.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:29.000000 etlt-1.0.0/etlt/condition/__init__.py
+-rw-r--r--   0        0        0     3705 2024-05-14 02:25:15.662956 etlt-1.0.0/etlt/dimension/RegularDimension.py
+-rw-r--r--   0        0        0     5199 2024-05-14 02:35:22.075139 etlt-1.0.0/etlt/dimension/Type2ReferenceDimension.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:29.000000 etlt-1.0.0/etlt/dimension/__init__.py
+-rw-r--r--   0        0        0     2088 2024-05-14 02:35:22.077139 etlt-1.0.0/etlt/helper/Allen.py
+-rw-r--r--   0        0        0     6088 2024-05-14 02:35:22.022137 etlt-1.0.0/etlt/helper/Type2CondenseHelper.py
+-rw-r--r--   0        0        0    14042 2024-05-14 02:41:35.996276 etlt-1.0.0/etlt/helper/Type2Helper.py
+-rw-r--r--   0        0        0     4474 2024-05-14 02:47:07.137499 etlt-1.0.0/etlt/helper/Type2JoinHelper.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:29.000000 etlt-1.0.0/etlt/helper/__init__.py
+-rw-r--r--   0        0        0     2468 2024-05-14 02:47:07.431505 etlt-1.0.0/etlt/reader/Reader.py
+-rw-r--r--   0        0        0     9131 2024-05-14 02:51:53.041733 etlt-1.0.0/etlt/reader/UniversalCsvReader.py
+-rw-r--r--   0        0        0     2423 2024-05-14 03:04:51.494643 etlt-1.0.0/etlt/reader/UniversalCsvReaderFormatHelper.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:29.000000 etlt-1.0.0/etlt/reader/__init__.py
+-rw-r--r--   0        0        0     3887 2024-05-14 02:56:12.052369 etlt-1.0.0/etlt/writer/SqlLoaderWriter.py
+-rw-r--r--   0        0        0     1974 2024-05-14 03:04:51.475643 etlt-1.0.0/etlt/writer/Writer.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:29.000000 etlt-1.0.0/etlt/writer/__init__.py
+-rw-r--r--   0        0        0     1027 2024-05-14 04:40:45.773059 etlt-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 etlt-1.0.0/PKG-INFO
```

### Comparing `ETLT-0.9.6/etlt/Transformer.py` & `etlt-1.0.0/etlt/Transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import abc
 import copy
 import re
 import time
 import traceback
-from typing import Any, Dict, List
+from pprint import pformat
+from typing import Any, Dict, List, Optional, Tuple
 
 from etlt.cleaner.WhitespaceCleaner import WhitespaceCleaner
 from etlt.reader.Reader import Reader
 from etlt.writer.SqlLoaderWriter import SqlLoaderWriter
 
 
 class Transformer(metaclass=abc.ABCMeta):
@@ -20,18 +21,18 @@
                  source_reader: Reader,
                  transformed_writer: SqlLoaderWriter,
                  parked_writer: SqlLoaderWriter,
                  ignored_writer: SqlLoaderWriter):
         """
         Object constructor.
 
-        :param Reader source_reader: Object for reading source rows.
-        :param SqlLoaderWriter transformed_writer: Object for writing successfully transformed rows.
-        :param SqlLoaderWriter parked_writer: Object for writing parked rows.
-        :param SqlLoaderWriter ignored_writer: Object for writing ignored rows.
+        :param source_reader: Object for reading source rows.
+        :param transformed_writer: Object for writing successfully transformed rows.
+        :param parked_writer: Object for writing parked rows.
+        :param ignored_writer: Object for writing ignored rows.
         """
 
         self._count_total: int = 0
         """
         The number of rows processed.
         """
 
@@ -91,57 +92,58 @@
         """
 
         self._ignored_writer: SqlLoaderWriter = ignored_writer
         """
         Object for writing ignored rows.
         """
 
-        self._mandatory_fields: List[str] = []
+        self.__mandatory_fields: List[str] = []
         """
-        The mandatory fields (or columns) in the output row.
+        The mandatory fields (columns) in the output row.
         """
 
         self._steps: List[callable] = []
         """
         All _step<n> methods where n is an integer in this class sorted by n.
         """
 
+        self.__init_fields()
+
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def _log(message):
+    def _log(message: str) -> None:
         """
         Logs a message.
 
-        :param str message: The log message.
-
-        :rtype: None
+        :param message: The log message.
         """
         #  @todo Replace with log package.
-        print(time.strftime('%Y-%m-%d %H:%M:%S', time.localtime()) + ' ' + str(message), flush=True)
+        print(time.strftime('%Y-%m-%d %H:%M:%S', time.gmtime()) + ' ' + str(message), flush=True)
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _handle_exception(self, row, exception) -> None:
+    def _handle_exception(self, row: Dict[str, Any], exception: Exception) -> None:
         """
         Logs an exception occurred during transformation of a row.
 
-        :param list|dict|() row: The source row.
-        :param Exception exception: The exception.
+        :param row: The source row.
+        :param exception: The exception.
         """
         self._log('Error during processing of line {0:d}.'.format(self._source_reader.row_number))
-        self._log(row)
+        self._log(pformat(row))
         self._log(str(exception))
         self._log(traceback.format_exc())
 
     # ------------------------------------------------------------------------------------------------------------------
     def _find_all_step_methods(self) -> None:
         """
         Finds all _step<n> methods where n is an integer in this class.
         """
-        steps = ([method for method in dir(self) if callable(getattr(self, method)) and
-                  re.match(r'_step\d+\d+.*', method)])
+        steps = (
+                [method for method in dir(self) if
+                 callable(getattr(self, method)) and re.match(r'_step\d+\d+.*', method)])
         steps = sorted(steps)
         for step in steps:
             self._steps.append(getattr(self, step))
 
     # ------------------------------------------------------------------------------------------------------------------
     def _transform_rows(self) -> None:
         """
@@ -149,58 +151,52 @@
         """
         self._find_all_step_methods()
 
         for row in self._source_reader.next():
             self._transform_row_wrapper(row)
 
     # ------------------------------------------------------------------------------------------------------------------
-    def pre_park_row(self, park_info, in_row) -> None:
+    def pre_park_row(self, park_info: str, in_row: Dict[str, Any]) -> None:
         """
         This method will be called just be for sending an input row to be parked to the parked writer.
 
-        :param str park_info: The park info.
-        :param dict[str,str] in_row: The original input row.
-
-        :rtype: None
+        :param park_info: The park info.
+        :param in_row: The original input row.
         """
         pass
 
     # ------------------------------------------------------------------------------------------------------------------
-    def pre_ignore_row(self, ignore_info, in_row) -> None:
+    def pre_ignore_row(self, ignore_info: str, in_row: Dict[str, Any]) -> None:
         """
         This method will be called just be for sending an input row to be ignored to the ignore writer.
 
-        :param str ignore_info: The ignore info.
-        :param dict[str,str] in_row: The original input row.
-
-        :rtype: None
+        :param ignore_info: The ignore info.
+        :param in_row: The original input row.
         """
         pass
 
     # ------------------------------------------------------------------------------------------------------------------
     def _transform_row_wrapper(self, row: Dict[str, Any]) -> None:
         """
         Transforms a single source row.
 
-        :param dict[str,any] row: The source row.
+        :param row: The source row.
         """
         self._count_total += 1
 
         try:
             # Transform the naturals keys in line to technical keys.
             in_row = copy.copy(row)
             out_row = {}
             park_info, ignore_info = self._transform_row(in_row, out_row)
 
         except Exception as e:
             # Log the exception.
             self._handle_exception(row, e)
-            # Keep track of the number of errors.
             self._count_error += 1
-            # This row must be parked.
             park_info = 'Exception'
             # Keep our IDE happy.
             ignore_info = None
             out_row = {}
 
         if park_info:
             # Park the row.
@@ -214,91 +210,85 @@
             self._count_ignore += 1
         else:
             # Write the technical keys and measures to the output file.
             self._transformed_writer.writerow(out_row)
             self._count_transform += 1
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _transform_row(self, in_row, out_row):
+    def _transform_row(self, in_row: Dict[str, Any], out_row: Dict[str, Any]) -> Tuple[Optional[str], Optional[str]]:
         """
         Transforms an input row to an output row (i.e. (partial) dimensional data).
 
-        :param dict[str,str] in_row: The input row.
-        :param dict[str,T] out_row: The output row.
-
-        :rtype: (str,str)
+        :param in_row: The input row.
+        :param out_row: The output row.
         """
         tmp_row = {}
 
         for step in self._steps:
             park_info, ignore_info = step(in_row, tmp_row, out_row)
             if park_info or ignore_info:
                 return park_info, ignore_info
 
         return None, None
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _step00(self, in_row, tmp_row, out_row):
+    def _step00(self, in_row: Dict[str, Any], tmp_row: Dict[str, Any], out_row: Dict[str, Any]) -> Tuple[
+        Optional[str], Optional[str]]:
         """
         Prunes whitespace for all fields in the input row.
 
-        :param dict in_row: The input row.
-        :param dict tmp_row: Not used.
-        :param dict out_row: Not used.
+        :param in_row: The input row.
+        :param tmp_row: Not used.
+        :param out_row: Not used.
         """
         for key, value in in_row.items():
             in_row[key] = WhitespaceCleaner.clean(value)
 
         return None, None
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _step99(self, in_row, tmp_row, out_row):
+    def _step99(self, in_row: Dict[str, Any], tmp_row: Dict[str, Any], out_row: Dict[str, Any]) -> Tuple[
+        Optional[str], Optional[str]]:
         """
         Validates all mandatory fields are in the output row and are filled.
 
-        :param dict in_row: The input row.
-        :param dict tmp_row: Not used.
-        :param dict out_row: The output row.
+        :param in_row: The input row.
+        :param tmp_row: Not used.
+        :param out_row: The output row.
         """
         park_info = ''
-        for field in self._mandatory_fields:
+        for field in self.__mandatory_fields:
             if field not in out_row or not out_row[field]:
                 if park_info:
                     park_info += ' '
                 park_info += field
 
         return park_info, None
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _load_ignored_rows(self) -> None:
         """
         Loads the ignored rows into the database.
-
-        :rtype: None
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _load_parked_rows(self) -> None:
         """
         Loads the parked rows into the database.
-
-        :rtype: None
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _load_transformed_rows(self) -> None:
         """
         Loads the successfully transformed rows into the database.
-
-        :rtype: None
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     def _log_statistics(self) -> None:
         """
         Log statistics about the number of rows and number of rows per second.
@@ -316,16 +306,14 @@
         self._log('Number of rows per second loaded    : {0:d}'.format(int(rows_per_second_load)))
         self._log('Number of rows per second overall   : {0:d}'.format(int(rows_per_second_overall)))
 
     # ------------------------------------------------------------------------------------------------------------------
     def pre_transform_source_rows(self) -> None:
         """
         This method will be called just before transforming the source rows.
-
-        :rtype: None
         """
         pass
 
     # ------------------------------------------------------------------------------------------------------------------
     def transform_source_rows(self) -> None:
         """
         Transforms the rows for the source system into (partial) dimensional data.
@@ -357,8 +345,41 @@
 
         # Time end of loading parked and ignored rows.
         self._time3 = time.perf_counter()
 
         # Show statistics about number of rows and performance.
         self._log_statistics()
 
-# ----------------------------------------------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------------------------------------------
+    @abc.abstractmethod
+    def _get_input_fields(self) -> List[str]:
+        """
+        Returns the expected names of the columns in the input.
+        """
+        raise NotImplementedError()
+
+    # ------------------------------------------------------------------------------------------------------------------
+    @abc.abstractmethod
+    def _get_mandatory_fields(self) -> List[str]:
+        """
+        Returns the mandatory fields (columns) in the output row.
+        """
+        raise NotImplementedError()
+
+    # ------------------------------------------------------------------------------------------------------------------
+    @abc.abstractmethod
+    def _get_output_fields(self) -> List[str]:
+        """
+        Return the fields (columns) that must be written to the output.
+        """
+        raise NotImplementedError()
+
+    # ------------------------------------------------------------------------------------------------------------------
+    def __init_fields(self) -> None:
+        """
+        Initializes the fields of source, output, and mandatory.
+        """
+        self._source_reader.fields = self._get_input_fields()
+        self.__mandatory_fields = self._get_mandatory_fields()
+        self._transformed_writer.fields = self._get_output_fields()
+
+    # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `ETLT-0.9.6/etlt/cleaner/DateCleaner.py` & `etlt-1.0.0/etlt/cleaner/DateCleaner.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,44 +5,42 @@
 class DateCleaner:
     """
     Utility class for converting dates in miscellaneous formats to ISO-8601 (YYYY-MM-DD) format.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     month_map = {
-        # English
-        'jan': '01',
-        'feb': '02',
-        'mar': '03',
-        'apr': '04',
-        'may': '05',
-        'jun': '06',
-        'jul': '07',
-        'aug': '08',
-        'sep': '09',
-        'oct': '10',
-        'nov': '11',
-        'dec': '12',
-
-        # Dutch
-        'mrt': '03',
-        'mei': '05',
-        'okt': '10'
+            # English
+            'jan': '01',
+            'feb': '02',
+            'mar': '03',
+            'apr': '04',
+            'may': '05',
+            'jun': '06',
+            'jul': '07',
+            'aug': '08',
+            'sep': '09',
+            'oct': '10',
+            'nov': '11',
+            'dec': '12',
+
+            # Dutch
+            'mrt': '03',
+            'mei': '05',
+            'okt': '10'
     }
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def clean(date: Optional[str], ignore_time: bool = False) -> Optional[str]:
         """
         Converts a date in miscellaneous format to ISO-8601 (YYYY-MM-DD) format.
 
-        :param str|None date: The input date.
-        :param bool ignore_time: If true any trailing time prt is ignore.
-
-        :rtype: strNone
+        :param date: The input date.
+        :param ignore_time: Whether any trailing time part must be ignored.
         """
         # Return empty input immediately.
         if not date:
             return date
 
         parts = re.split(r'[\-/. ]', date)
 
@@ -60,14 +58,32 @@
 
             if len(parts[0]) <= 2 and len(parts[1]) <= 2 and len(parts[2]) == 2:
                 # Assume date is in  DD-MM-YY or D-M-YY format.
                 year = '19' + parts[2] if parts[2] >= '20' else '20' + parts[2]
 
                 return year + '-' + ('00' + parts[1])[-2:] + '-' + ('00' + parts[0])[-2:]
 
+        # Try DD-MM-YYYY HH:mm:ss format
+        pattern = r'^(\d{2})\D(\d{2})\D(\d{4})' + ('.*$' if ignore_time else r'(\D(\d{1,2})\D(\d{1,2})\D(\d{1,2}))?$')
+        match = re.match(pattern, date)
+        if match:
+            ret = match.group(3) + '-' + match.group(2) + '-' + match.group(1)
+            if len(match.groups()) == 7 and match.group(4):
+                ret += 'T' + match.group(5) + ':' + match.group(6) + ':' + match.group(7)
+            return ret
+
+        # Try DD-MM-YYYY HH:mm format
+        pattern = r'^(\d{2})\D(\d{2})\D(\d{4})' + ('.*$' if ignore_time else r'(\D(\d{1,2})\D(\d{1,2}))?$')
+        match = re.match(pattern, date)
+        if match:
+            ret = match.group(3) + '-' + match.group(2) + '-' + match.group(1)
+            if len(match.groups()) == 6 and match.group(4):
+                ret += 'T' + match.group(5) + ':' + match.group(6) + ':00'
+            return ret
+
         # Try DDmonYYYY or DDmonYYYY HH:mm:ss format
         pattern = r'^(\d{2})([a-z]{3})(\d{4})' + ('.*$' if ignore_time else r'(\D(\d{1,2})\D(\d{1,2})\D(\d{1,2}))?$')
         match = re.match(pattern, date.lower())
         if match and match.group(2) in DateCleaner.month_map:
             ret = match.group(3) + '-' + DateCleaner.month_map[match.group(2)] + '-' + match.group(1)
             if len(match.groups()) == 7 and match.group(4):
                 ret += 'T' + match.group(5) + ':' + match.group(6) + ':' + match.group(7)
```

### Comparing `ETLT-0.9.6/etlt/cleaner/MoneyCleaner.py` & `etlt-1.0.0/etlt/cleaner/MoneyCleaner.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def clean(amount: Optional[str]) -> Optional[str]:
         """
         Converts a number to a number with decimal point.
 
-        :param str|None amount: The input number.
-
-        :rtype: str|None
+        :param amount: The input number.
         """
         # Return empty input immediately.
         if not amount:
             return amount
 
         if re.search(r'^[0-9]{0,2}([. ][0-9]{3})+(,[0-9]{1,2})?$', amount):
             # Assume amount is in 1.123,12 or 1 123,12 or 1 123 format (Dutch).
@@ -29,11 +27,15 @@
             # Assume amount is in 1,123.12 or 1 123 format (Engels).
             return amount.replace(',', '').replace(' ', '')
 
         if re.search(r'^[0-9]+(,[0-9]{1,2}$)', amount):
             # Assume amount is in 123,12 or in 123,1 format (Dutch).
             return amount.replace(',', '.')
 
+        if re.search(r'^[0-9]{0,2}(\.[0-9]{3})+(\.[0-9]{2})?$', amount):
+            # Amount is in 1.123.12 format.
+            return amount.replace('.', '', 1)
+
         # Format of amount is not recognized. Return amount.
         return amount
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `ETLT-0.9.6/etlt/cleaner/WhitespaceCleaner.py` & `etlt-1.0.0/etlt/cleaner/WhitespaceCleaner.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def clean(string: Optional[str]) -> Optional[str]:
         """
         Prunes whitespace from a string.
 
-        :param str string: The string.
-
-        :rtype: str
+        :param string: The string.
         """
         # Return empty input immediately.
         if not string:
             return string
 
         return string.replace('  ', ' ').strip()
```

### Comparing `ETLT-0.9.6/etlt/condition/AndCondition.py` & `etlt-1.0.0/etlt/condition/OrCondition.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
+from typing import Any, Dict
+
 from etlt.condition.CompoundCondition import CompoundCondition
 
 
 class AndCondition(CompoundCondition):
     """
-    A condition or filter that match (i.e return True) if all child conditions match the row.
+    A condition or filter that match (i.e. return True) if one or more child conditions match the row.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def match(self, row):
+    def match(self, row: Dict[str, Any]) -> bool:
         """
-        Returns True if the row matches all child conditions. Returns False otherwise.
+        Returns True if the row matches one or more child conditions. Returns False otherwise.
 
         :param dict row: The row.
-
-        :rtype: bool
         """
         for condition in self._conditions:
-            if not condition.match(row):
-                return False
+            if condition.match(row):
+                return True
 
-        return True
+        return False
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `ETLT-0.9.6/etlt/condition/CompoundCondition.py` & `etlt-1.0.0/etlt/condition/CompoundCondition.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from abc import ABC
+from typing import List
 
 from etlt.condition.Condition import Condition
 
 
 class CompoundCondition(Condition, ABC):
     """
     Abstract parent class for conditions with one or more child conditions.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def __init__(self):
         """
         Object constructor.
         """
-        self._conditions = []
+        self._conditions: List[Condition] = []
         """
         The list of conditions of this compound condition.
-
-        :type: list[gdwh.map.Condition.Condition]
         """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def append_condition(self, condition):
+    def append_condition(self, condition: Condition) -> None:
         """
         Appends a child condition to the list of conditions of this compound condition.
 
-        :param gdwh.map.Condition.Condition condition: The child conditions.
+        :param condition: The child conditions.
         """
         self._conditions.append(condition)
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `ETLT-0.9.6/etlt/condition/FalseCondition.py` & `etlt-1.0.0/etlt/condition/PlainCondition.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,28 @@
+from typing import Any, Dict
+
 from etlt.condition.SimpleCondition import SimpleCondition
 
 
-class FalseCondition(SimpleCondition):
+class PlainCondition(SimpleCondition):
     """
-    A false condition always evaluates to False.
+    A plain condition matches a field in the row against a plain value.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def match(self, row):
+    def match(self, row: Dict[str, Any]) -> bool:
         """
-        Always returns False.
-
-        :param dict row: The row, ignored
+        Returns True if the fields equals the expression of this simple condition. Returns False otherwise.
 
-        :rtype: False
+        :param row: The row.
         """
-        return False
+        return row[self._field] == self._expression
 
     # ------------------------------------------------------------------------------------------------------------------
     @property
-    def scheme(self):
+    def scheme(self) -> str:
         """
-        Returns 'false'.
-
-        :rtype: str
+        Returns 'plain'.
         """
-        return 'false'
+        return 'plain'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `ETLT-0.9.6/etlt/condition/GlobCondition.py` & `etlt-1.0.0/etlt/condition/AndCondition.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,24 @@
-import fnmatch
+from typing import Any, Dict
 
-from etlt.condition.SimpleCondition import SimpleCondition
+from etlt.condition.CompoundCondition import CompoundCondition
 
 
-class GlobCondition(SimpleCondition):
+class AndCondition(CompoundCondition):
     """
-    A glob condition matches a field in the row against a glob expression.
+    A condition or filter that match (i.e. return True) if all child conditions match the row.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def match(self, row):
+    def match(self, row: Dict[str, Any]) -> bool:
         """
-        Returns True if the field matches the glob expression of this simple condition. Returns False otherwise.
+        Returns whether a row matches all child conditions.
 
-        :param dict row: The row.
-
-        :rtype: bool
+        :param row: The row.
         """
-        return fnmatch.fnmatchcase(row[self._field], self._expression)
+        for condition in self._conditions:
+            if not condition.match(row):
+                return False
 
-    # ------------------------------------------------------------------------------------------------------------------
-    @property
-    def scheme(self):
-        """
-        Returns 'glob'.
-
-        :rtype: str
-        """
-        return 'glob'
+        return True
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `ETLT-0.9.6/etlt/condition/InListCondition.py` & `etlt-1.0.0/etlt/condition/InListCondition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,71 @@
+from typing import Any, Dict, List
+
 from etlt.condition.Condition import Condition
+from etlt.condition.SimpleCondition import SimpleCondition
 from etlt.condition.SimpleConditionFactory import SimpleConditionFactory
 
 
 class InListCondition(Condition):
     """
     A list condition matches a single field against a list of conditions.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, field):
+    def __init__(self, field: str):
         """
         Object contructor.
 
         :param str field: The name of the field in the row that must be match against the expression.
         """
-        self._field = field
+        self._field: str = field
         """
         The name of the field in the row that must be match against the list of values.
-
-        :type: str
         """
 
-        self._values = list()
+        self._values: List[str] = list()
         """
         The list of values of plain conditions.
-
-        :type: list[str]
         """
 
-        self._conditions = list()
+        self._conditions: List[SimpleCondition] = list()
         """
         The list of other conditions.
-
-        :type: list[etlt.condition.SimpleCondition.SimpleCondition]
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     @property
-    def field(self):
+    def field(self) -> str:
         """
         Getter for field.
-
-        :rtype: str
         """
         return self._field
 
     # ------------------------------------------------------------------------------------------------------------------
-    def populate_values(self, rows, field):
+    def populate_values(self, rows: List[Dict[str, Any]], field: str):
         """
         Populates the filter values of this filter using list of rows.
 
-        :param list[dict[str,T]] rows: The row set.
-        :param str field: The field name.
+        :param rows: The row set.
+        :param field: The field name.
         """
         self._values.clear()
         for row in rows:
             condition = SimpleConditionFactory.create_condition(self._field, row[field])
             if condition.scheme == 'plain':
                 self._values.append(condition.expression)
             else:
                 self._conditions.append(condition)
 
     # ------------------------------------------------------------------------------------------------------------------
-    def match(self, row):
+    def match(self, row: Dict[str, Any]) -> bool:
         """
-        Returns True if the field is in the list of conditions. Returns False otherwise.
+        Returns whether the field is in the list of conditions.
 
         :param dict row: The row.
-
-        :rtype: bool
         """
         if row[self._field] in self._values:
             return True
 
         for condition in self._conditions:
             if condition.match(row):
                 return True
```

### Comparing `ETLT-0.9.6/etlt/condition/PlainCondition.py` & `etlt-1.0.0/etlt/condition/FalseCondition.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,28 @@
+from typing import Any, Dict
+
 from etlt.condition.SimpleCondition import SimpleCondition
 
 
-class PlainCondition(SimpleCondition):
+class FalseCondition(SimpleCondition):
     """
-    A plain condition matches a field in the row against a plain value.
+    A false condition always evaluates to False.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def match(self, row):
+    def match(self, row: Dict[str, Any]) -> False:
         """
-        Returns True if the fields equals the expression of this simple condition. Returns False otherwise.
-
-        :param dict row: The row.
+        Always returns False.
 
-        :rtype: bool
+        :param row: The row, ignored
         """
-        return row[self._field] == self._expression
+        return False
 
     # ------------------------------------------------------------------------------------------------------------------
     @property
-    def scheme(self):
+    def scheme(self) -> str:
         """
-        Returns 'plain'.
-
-        :rtype: str
+        Returns 'false'.
         """
-        return 'plain'
+        return 'false'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `ETLT-0.9.6/etlt/condition/RegularExpressionCondition.py` & `etlt-1.0.0/etlt/condition/RegularExpressionCondition.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 import re
+from typing import Any, Dict
 
 from etlt.condition.SimpleCondition import SimpleCondition
 
 
 class RegularExpressionCondition(SimpleCondition):
     """
     A regular expression condition matches a field in the row against a regular expression expression.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def match(self, row):
+    def match(self, row: Dict[str, Any]) -> bool:
         """
         Returns True if the field matches the regular expression of this simple condition. Returns False otherwise.
 
-        :param dict row: The row.
-
-        :rtype: bool
+        :param row: The row.
         """
         if re.search(self._expression, row[self._field]):
             return True
 
         return False
 
     # ------------------------------------------------------------------------------------------------------------------
     @property
-    def scheme(self):
+    def scheme(self) -> str:
         """
         Returns 're'.
-
-        :rtype: str
         """
         return 're'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `ETLT-0.9.6/etlt/condition/SimpleCondition.py` & `etlt-1.0.0/etlt/condition/SimpleCondition.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,60 +5,50 @@
 
 class SimpleCondition(Condition):
     """
     A simple condition matches a single field in the row against an expression.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, field, expression):
+    def __init__(self, field: str, expression: str):
         """
         Object contructor.
 
-        :param str field: The name of the field in the row that must be match against the expression.
-        :param str expression: The expression.
+        :param field: The name of the field in the row that must be match against the expression.
+        :param expression: The expression.
         """
-        self._field = field
+        self._field: str = field
         """
         The name of the field in the row that must be match against the expression.
-
-        :type: str
         """
 
-        self._expression = expression
+        self._expression: str = expression
         """
         The expression.
-
-        :type: str
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     @property
-    def expression(self):
+    def expression(self) -> str:
         """
         Returns the expression.
-
-        :rtype: str
         """
         return self._expression
 
     # ------------------------------------------------------------------------------------------------------------------
     @property
-    def field(self):
+    def field(self) -> str:
         """
         Returns the name of the field in the row that must be match against the expression.
-
-        :rtype: str
         """
         return self._field
 
     # ------------------------------------------------------------------------------------------------------------------
     @property
     @abc.abstractmethod
-    def scheme(self):
+    def scheme(self) -> str:
         """
         Returns the scheme of the simple condition.
-
-        :rtype: str
         """
         raise NotImplementedError()
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `ETLT-0.9.6/etlt/condition/SimpleConditionFactory.py` & `etlt-1.0.0/etlt/condition/SimpleConditionFactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,69 @@
 import re
+from typing import Callable, Dict, Tuple
 
 from etlt.condition.FalseCondition import FalseCondition
 from etlt.condition.GlobCondition import GlobCondition
 from etlt.condition.PlainCondition import PlainCondition
 from etlt.condition.RegularExpressionCondition import RegularExpressionCondition
+from etlt.condition.SimpleCondition import SimpleCondition
 from etlt.condition.TrueCondition import TrueCondition
 
 
 class SimpleConditionFactory:
     """
     A factory for simple conditions.
     """
-    _constructors = {}
+    _constructors: Dict[str, Callable] = {}
     """
     A map from scheme to object constructors.
-
-    dict[str, callable]
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def _split_scheme(expression):
+    def _split_scheme(expression: str) -> Tuple[str, str]:
         """
         Splits the scheme and actual expression
 
-        :param str expression: The expression.
-
-        :rtype: str
+        :param expression: The expression.
         """
         match = re.search(r'^([a-z]+):(.*)$', expression)
         if not match:
             scheme = 'plain'
             actual = expression
         else:
             scheme = match.group(1)
             actual = match.group(2)
 
         return scheme, actual
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def register_scheme(scheme, constructor):
+    def register_scheme(scheme: str, constructor: Callable) -> None:
         """
         Registers a scheme.
 
-        :param str scheme: The scheme.
-        :param callable constructor: The SimpleCondition constructor.
+        :param scheme: The scheme.
+        :param constructor: The SimpleCondition constructor.
         """
         if not re.search(r'^[a-z]+$', scheme):
             raise ValueError('{0!s} is not a valid scheme'.format(scheme))
 
         if scheme in SimpleConditionFactory._constructors:
             raise ValueError('Scheme {0!s} is registered already'.format(scheme))
 
         SimpleConditionFactory._constructors[scheme] = constructor
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def create_condition(field, expression):
+    def create_condition(field: str, expression: str) -> SimpleCondition:
         """
 
         :param str field: The name of the field.
         :param expression: The expression (including scheme).
-
-        :rtype: gdwh.map.SimpleCondition.SimpleCondition
         """
         scheme, expression = SimpleConditionFactory._split_scheme(expression)
 
         if scheme not in SimpleConditionFactory._constructors:
             raise ValueError('Scheme {0!s} is not registered'.format(scheme))
 
         return SimpleConditionFactory._constructors[scheme](field, expression)
```

### Comparing `ETLT-0.9.6/etlt/condition/TrueCondition.py` & `etlt-1.0.0/etlt/condition/TrueCondition.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,28 @@
+from typing import Any, Dict
+
 from etlt.condition.SimpleCondition import SimpleCondition
 
 
 class TrueCondition(SimpleCondition):
     """
     A true condition always evaluates to True.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def match(self, row):
+    def match(self, row: Dict[str, Any]) -> True:
         """
         Always returns true.
 
         :param dict row: The row, ignored.
-
-        :rtype: True
         """
         return True
 
     # ------------------------------------------------------------------------------------------------------------------
     @property
-    def scheme(self):
+    def scheme(self) -> str:
         """
         Returns 'true'.
-
-        :rtype: str
         """
         return 'true'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `ETLT-0.9.6/etlt/dimension/Type2ReferenceDimension.py` & `etlt-1.0.0/etlt/dimension/Type2ReferenceDimension.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,54 @@
 import abc
 import datetime
+from typing import Any, Dict, List, Optional
 
 
 class Type2ReferenceDimension(metaclass=abc.ABCMeta):
     """
     Abstract class for type2 dimensions for which the reference data is supplied with date intervals.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def __init__(self):
         """
         Object constructor.
         """
 
-        self._key_key = ''
+        self._key_key: str = ''
         """
         The key in the dict returned by call_stored_procedure holding the technical ID.
-
-        :type: str
         """
 
-        self._key_date_start = ''
+        self._key_date_start: str = ''
         """
         The key in the dict returned by call_stored_procedure holding the start date.
-
-        :type: str
         """
 
-        self._key_date_end = ''
+        self._key_date_end: str = ''
         """
         The key in the dict returned by call_stored_procedure holding the end date.
-
-        :type: str
         """
 
-        self._map = {}
+        self._map: Dict[Any, List[Any]] = {}
         """
         The map from natural keys to lists of tuples with start date, end date, and technical keys. The dates must be in
         ISO 8601 (YYYY-MM-DD) format.
-
-        :type: dict[T, list[(str,str,int|None)]]
         """
 
-        # Pre-load look up data in to the map.
         self.pre_load_data()
 
     # ------------------------------------------------------------------------------------------------------------------
-    def get_id(self, natural_key, date, enhancement=None):
+    def get_id(self, natural_key: Any, date: str, enhancement: Any = None) -> Optional[int]:
         """
         Returns the technical ID for a natural key at a date or None if the given natural key is not valid.
 
-        :param T natural_key: The natural key.
-        :param str date: The date in ISO 8601 (YYYY-MM-DD) format.
-        :param T enhancement: Enhancement data of the dimension row.
-
-        :rtype: int|None
+        :param natural_key: The natural key.
+        :param date: The date in ISO 8601 (YYYY-MM-DD) format.
+        :param enhancement: Enhancement data of the dimension row.
         """
         if not date:
             return None
 
         # If the natural key is known return the technical ID immediately.
         if natural_key in self._map:
             for row in self._map[natural_key]:
@@ -81,65 +71,55 @@
             self.post_call_stored_procedure(success)
 
         # Make sure the natural key is in the map.
         if natural_key not in self._map:
             self._map[natural_key] = []
 
         if row[self._key_key]:
-            self._map[natural_key].append((row[self._key_date_start],
-                                           row[self._key_date_end],
-                                           row[self._key_key]))
+            self._map[natural_key].append((row[self._key_date_start], row[self._key_date_end], row[self._key_key]))
         else:
             self._map[natural_key].append((date, date, None))
 
         return row[self._key_key]
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
-    def call_stored_procedure(self, natural_key, date, enhancement):
+    def call_stored_procedure(self, natural_key: Any, date: str, enhancement: Any) -> Dict[str, Any]:
         """
         Call a stored procedure for getting the technical key of a natural key at a date. Returns the technical ID or
         None if the given natural key is not valid.
 
-        :param T natural_key: The natural key.
-        :param str date: The date in ISO 8601 (YYYY-MM-DD) format.
-        :param T enhancement: Enhancement data of the dimension row.
-
-        :rtype: dict
+        :param natural_key: The natural key.
+        :param date: The date in ISO 8601 (YYYY-MM-DD) format.
+        :param enhancement: Enhancement data of the dimension row.
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
-    def pre_load_data(self):
+    def pre_load_data(self) -> None:
         """
-        Can be overridden to pre-load lookup data from a dimension table.
-
-        :rtype: None
+        Can be overridden to preload lookup data from a dimension table.
         """
         pass
 
     # ------------------------------------------------------------------------------------------------------------------
-    def pre_call_stored_procedure(self):
+    def pre_call_stored_procedure(self) -> None:
         """
         This method is invoked before call the stored procedure for getting the technical key of a natural key.
 
         In a concurrent environment override this method to acquire a lock on the dimension or dimension hierarchy.
-
-        :rtype: None
         """
         pass
 
     # ------------------------------------------------------------------------------------------------------------------
-    def post_call_stored_procedure(self, success):
+    def post_call_stored_procedure(self, success: bool) -> None:
         """
         This method is invoked after calling the stored procedure for getting the technical key of a natural key.
 
         In a concurrent environment override this method to release a lock on the dimension or dimension hierarchy and
         to commit or rollback the transaction.
 
-        :param bool success: True: the stored procedure is executed successfully. False: an exception has occurred.
-
-        :rtype: None
+        :param success: True: the stored procedure is executed successfully. False: an exception has occurred.
         """
         pass
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `ETLT-0.9.6/etlt/helper/Allen.py` & `etlt-1.0.0/etlt/helper/Allen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Optional
+
+
 class Allen:
     """
     Utility class for Allen's interval algebra, https://en.wikipedia.org/wiki/Allen%27s_interval_algebra.
     """
     # ------------------------------------------------------------------------------------------------------------------
     X_BEFORE_Y = 1
     X_MEETS_Y = 2
@@ -15,24 +18,22 @@
     X_OVERLAPS_WITH_Y_INVERSE = -3
     X_STARTS_Y_INVERSE = -4
     X_DURING_Y_INVERSE = -5
     X_FINISHES_Y_INVERSE = -6
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def relation(x_start, x_end, y_start, y_end):
+    def relation(x_start: int, x_end: int, y_start: int, y_end: int) -> Optional[int]:
         """
         Returns the relation between two intervals.
 
-        :param int x_start: The start point of the first interval.
-        :param int x_end: The end point of the first interval.
-        :param int y_start: The start point of the second interval.
-        :param int y_end: The end point of the second interval.
-
-        :rtype: int|None
+        :param x_start: The start point of the first interval.
+        :param x_end: The end point of the first interval.
+        :param y_start: The start point of the second interval.
+        :param y_end: The end point of the second interval.
         """
 
         if (x_end - x_start) < 0 or (y_end - y_start) < 0:
             return None
 
         diff_end = y_end - x_end
```

### Comparing `ETLT-0.9.6/etlt/helper/Type2CondenseHelper.py` & `etlt-1.0.0/etlt/helper/Type2CondenseHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
+from typing import Any, Dict, List, Optional, Set, Tuple
+
 from etlt.helper.Allen import Allen
 from etlt.helper.Type2Helper import Type2Helper
 
 
 class Type2CondenseHelper(Type2Helper):
     """
     A helper class for deriving the distinct intervals in reference data with date intervals.
 
     A typical use case for this class is aggregate the reference data for a type 2 dimension into the reference data
     for another type 2 dimension at a higher in the dimension hierarchy.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def _distinct(row1, row2):
+    def _distinct(row1: Tuple[int, int], row2: Tuple[int, int]) -> Optional[List[Tuple[int, int]]]:
         """
         Returns a list of distinct (or none overlapping) intervals if two intervals are overlapping. Returns None if
         the two intervals are none overlapping. The list can have 2 or 3 intervals.
 
-        :param tuple[int,int] row1: The first interval.
-        :param tuple[int,int] row2: The second interval.
-
-        :rtype: None|list(tuple[int,int])
+        :param row1: The first interval.
+        :param row2: The second interval.
         """
         relation = Allen.relation(row1[0], row1[1], row2[0], row2[1])
 
         if relation is None:
             # One of the 2 intervals is invalid.
             return []
 
@@ -94,20 +94,20 @@
             return None  # [(row1[0], row1[1])]
 
         # We got all 13 relation in Allen's interval algebra covered.
         raise ValueError('Unexpected relation {0}'.format(relation))
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def _add_interval(all_intervals, new_interval):
+    def _add_interval(all_intervals: Set[Tuple[int, int]], new_interval: Tuple[int, int]) -> None:
         """
         Adds a new interval to a set of none overlapping intervals.
 
-        :param set[(int,int)] all_intervals: The set of distinct intervals.
-        :param (int,int) new_interval: The new interval.
+        :param all_intervals: The set of distinct intervals.
+        :param new_interval: The new interval.
         """
         intervals = None
         old_interval = None
         for old_interval in all_intervals:
             intervals = Type2CondenseHelper._distinct(new_interval, old_interval)
             if intervals:
                 break
@@ -117,30 +117,28 @@
         else:
             if old_interval:
                 all_intervals.remove(old_interval)
             for distinct_interval in intervals:
                 Type2CondenseHelper._add_interval(all_intervals, distinct_interval)
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _derive_distinct_intervals(self, rows):
+    def _derive_distinct_intervals(self, rows: List[Dict[str, Any]]) -> Set[Tuple[int, int]]:
         """
         Returns the set of distinct intervals in a row set.
 
-        :param list[dict[str,T]] rows: The rows set.
-
-        :rtype: set[(int,int)]
+        :param rows: The rows set.
         """
         ret = set()
         for row in rows:
             self._add_interval(ret, (row[self._key_start_date], row[self._key_end_date]))
 
         return ret
 
     # ------------------------------------------------------------------------------------------------------------------
-    def condense(self):
+    def condense(self) -> None:
         """
         Condense the data set to the distinct intervals based on the pseudo key.
         """
         for pseudo_key, rows in self._rows.items():
             tmp1 = []
             intervals = sorted(self._derive_distinct_intervals(rows))
             for interval in intervals:
```

### Comparing `ETLT-0.9.6/etlt/helper/Type2Helper.py` & `etlt-1.0.0/etlt/helper/Type2Helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,133 +1,119 @@
 import copy
 import datetime
+from typing import Any, Dict, List, Tuple, Union
 
 from etlt.helper.Allen import Allen
 
 
 class Type2Helper:
     """
     A helper class for reference data with date intervals.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, key_start_date, key_end_date, pseudo_key):
+    def __init__(self, key_start_date: str, key_end_date: str, pseudo_key: List[str]):
         """
         Object constructor.
 
-        :param str key_start_date: The key of the start date in the rows.
-        :param str key_end_date: The key of the end date in the rows.
-        :param list[str] pseudo_key: The keys of the columns that form the pseudo key.
+        :param key_start_date: The key of the start date in the rows.
+        :param key_end_date: The key of the end date in the rows.
+        :param pseudo_key: The keys of the columns that form the pseudo key.
         """
-        self.copy = True
+        self.copy: bool = True
         """
         If set to true a copy will be made from the original rows such that the original rows are not modified.
-
-         :type: bool
         """
 
-        self._pseudo_key = list(pseudo_key)
+        self._pseudo_key: List[str] = list(pseudo_key)
         """
         The keys of the columns that form the pseudo key.
-
-        :type: list[str]
         """
 
-        self._key_end_date = key_end_date
+        self._key_end_date: str = key_end_date
         """
         The key of the end date in the rows.
-
-        :type: str
         """
-        self._key_start_date = key_start_date
+
+        self._key_start_date: str = key_start_date
         """
         The key of the start date in the rows.
-
-        :type: str
         """
 
-        self._rows = dict()
+        self._rows: Dict = dict()
         """
         The data set.
-
-        :type: dict
         """
 
-        self._date_type = ''
+        self._date_type: str = ''
         """
         The type of the date fields.
         - date for datetime.date objects
         - str  for strings in ISO 8601 (YYYY-MM-DD) format
         - int for integers
-
-        :type: str
         """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _get_pseudo_key(self, row):
+    def _get_pseudo_key(self, row: Dict[str, Any]) -> Tuple:
         """
         Returns the pseudo key in a row.
 
         :param dict row: The row.
-
-        :rtype: tuple
         """
         ret = list()
         for key in self._pseudo_key:
             ret.append(row[key])
 
         return tuple(ret)
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def _date2int(date):
+    def _date2int(date: Union[str, datetime.date, int]) -> int:
         """
         Returns an integer representation of a date.
 
-        :param str|datetime.date date: The date.
-
-        :rtype: int
+        :param date: The date.
         """
         if isinstance(date, str):
             if date.endswith(' 00:00:00') or date.endswith('T00:00:00'):
                 # Ignore time suffix.
                 date = date[0:-9]
             tmp = datetime.datetime.strptime(date, '%Y-%m-%d')
             return tmp.toordinal()
 
         if isinstance(date, datetime.date):
             return date.toordinal()
 
         if isinstance(date, int):
             return date
 
-        raise ValueError('Unexpected type {0!s}'.format(date.__class__))
+        raise ValueError('Unexpected type {}'.format(date.__class__))
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _rows_date2int(self, rows):
+    def _rows_date2int(self, rows: List[Dict[str, Any]]) -> None:
         """
         Replaces start and end dates in a row set with their integer representation
 
-        :param list[dict[str,T]] rows: The list of rows.
+        :param rows: The list of rows.
         """
         for row in rows:
             # Determine the type of dates based on the first start date.
             if not self._date_type:
                 self._date_type = self._get_date_type(row[self._key_start_date])
 
             # Convert dates to integers.
             row[self._key_start_date] = self._date2int(row[self._key_start_date])
             row[self._key_end_date] = self._date2int(row[self._key_end_date])
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _rows_int2date(self, rows):
+    def _rows_int2date(self, rows: List[Dict[str, Any]]) -> None:
         """
         Replaces start and end dates in the row set with their integer representation
 
-        :param list[dict[str,T]] rows: The list of rows.
+        :param rows: The list of rows.
         """
         for row in rows:
             if self._date_type == 'str':
                 row[self._key_start_date] = datetime.date.fromordinal(row[self._key_start_date]).isoformat()
                 row[self._key_end_date] = datetime.date.fromordinal(row[self._key_end_date]).isoformat()
             elif self._date_type == 'date':
                 row[self._key_start_date] = datetime.date.fromordinal(row[self._key_start_date])
@@ -135,74 +121,66 @@
             elif self._date_type == 'int':
                 # Nothing to do.
                 pass
             else:
                 raise ValueError('Unexpected date type {0!s}'.format(self._date_type))
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _rows_sort(self, rows):
+    def _rows_sort(self, rows: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
         """
         Returns a list of rows sorted by start and end date.
 
-        :param list[dict[str,T]] rows: The list of rows.
-
-        :rtype: list[dict[str,T]]
+        :param rows: The list of rows.
         """
         return sorted(rows, key=lambda row: (row[self._key_start_date], row[self._key_end_date]))
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def _get_date_type(date):
+    def _get_date_type(date: Union[str, datetime.date, int]) -> str:
         """
-        Returns the type of a date.
+        Returns the typeof a date.
 
-        :param str|datetime.date date: The date.
-
-        :rtype: str
+        :param date: The date.
         """
         if isinstance(date, str):
             return 'str'
 
         if isinstance(date, datetime.date):
             return 'date'
 
         if isinstance(date, int):
             return 'int'
 
         raise ValueError('Unexpected type {0!s}'.format(date.__class__))
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _equal(self, row1, row2):
+    def _equal(self, row1: Dict[str, Any], row2: Dict[str, Any]) -> bool:
         """
-        Returns True if two rows are identical excluding start and end date. Returns False otherwise.
-
-        :param dict[str,T] row1: The first row.
-        :param dict[str,T] row2: The second row.
+        Returns whether two rows are identical excluding start and end date.
 
-        :rtype: bool
+        :param row1: The first row.
+        :param row2: The second row.
         """
         for key in row1.keys():
             if key not in [self._key_start_date, self._key_end_date]:
                 if row1[key] != row2[key]:
                     return False
 
         return True
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _merge_adjacent_rows(self, rows):
+    def _merge_adjacent_rows(self, rows: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
         """
         Resolves adjacent and overlapping rows. Overlapping rows are resolved as follows:
         * The interval with the most recent begin date prevails for the overlapping period.
-        * If the begin dates are the same the interval with the most recent end date prevails.
-        * If the begin and end dates are equal the last row in the data set prevails.
+        * If the start dates are the same the interval with the most recent end date prevails.
+        * If the start and end dates are equal the last row in the data set prevails.
         Identical (excluding begin and end date) adjacent rows are replace with a single row.
 
-        :param list[dict[str,T]] rows: The rows in a group (i.e. with the same natural key).
-        .
-        :rtype: list[dict[str,T]]
+        :param rows: The rows in a group (i.e. with the same natural key).
         """
         ret = list()
 
         prev_row = None
         for row in rows:
             if prev_row:
                 relation = Allen.relation(prev_row[self._key_start_date],
@@ -295,50 +273,48 @@
 
         if prev_row:
             ret.append(prev_row)
 
         return ret
 
     # ------------------------------------------------------------------------------------------------------------------
-    def enumerate(self, name, start=1):
+    def enumerate(self, name: str, start: int = 1) -> None:
         """
         Enumerates all rows such that the pseudo key and the ordinal number are a unique key.
 
-        :param str name: The key holding the ordinal number.
-        :param int start: The start of the ordinal numbers. Foreach pseudo key the first row has this ordinal number.
+        :param name: The key holding the ordinal number.
+        :param start: The start of the ordinal numbers. Foreach pseudo key the first row has this ordinal number.
         """
         for pseudo_key, rows in self._rows.items():
             rows = self._rows_sort(rows)
             ordinal = start
             for row in rows:
                 row[name] = ordinal
                 ordinal += 1
             self._rows[pseudo_key] = rows
 
     # ------------------------------------------------------------------------------------------------------------------
-    def get_rows(self, sort=False):
+    def get_rows(self, sort: bool = False) -> List:
         """
         Returns the rows of this Type2Helper.
 
-        :param bool sort: If True the rows are sorted by the pseudo key.
+        :param sort: Whether the rows must be sorted by the pseudo key.
         """
         ret = []
         for _, rows in sorted(self._rows.items()) if sort else self._rows.items():
             self._rows_int2date(rows)
             ret.extend(rows)
 
         return ret
 
     # ------------------------------------------------------------------------------------------------------------------
-    def prepare_data(self, rows):
+    def prepare_data(self, rows: List[Dict[str, Any]]) -> None:
         """
         Sets and prepares the rows. The rows are stored in groups in a dictionary. A group is a list of rows with the
         same pseudo key. The key in the dictionary is a tuple with the values of the pseudo key.
-
-        :param list[dict] rows: The rows
         """
         self._rows = dict()
         for row in copy.copy(rows) if self.copy else rows:
             pseudo_key = self._get_pseudo_key(row)
             if pseudo_key not in self._rows:
                 self._rows[pseudo_key] = list()
             self._rows[pseudo_key].append(row)
```

### Comparing `ETLT-0.9.6/etlt/helper/Type2JoinHelper.py` & `etlt-1.0.0/etlt/helper/Type2JoinHelper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,59 @@
+from typing import Any, Dict, List, Optional, Tuple
+
 from etlt.helper.Type2Helper import Type2Helper
 
 
 class Type2JoinHelper(Type2Helper):
     """
     A helper class for joining data sets with date intervals.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def _intersect(start1, end1, start2, end2):
+    def _intersect(start1: int, end1: int, start2: int, end2: int) -> Tuple[Optional[int], Optional[int]]:
         """
         Returns the intersection of two intervals. Returns (None,None) if the intersection is empty.
 
-        :param int start1: The start date of the first interval.
-        :param int end1: The end date of the first interval.
-        :param int start2: The start date of the second interval.
-        :param int end2: The end date of the second interval.
-
-        :rtype: tuple[int|None,int|None]
+        :param start1: The start date of the first interval.
+        :param end1: The end date of the first interval.
+        :param start2: The start date of the second interval.
+        :param end2: The end date of the second interval.
         """
         start = max(start1, start2)
         end = min(end1, end2)
 
         if start > end:
             return None, None
 
         return start, end
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _additional_rows_date2int(self, keys, rows):
+    def _additional_rows_date2int(self, keys: List[Tuple[str, str]], rows: List[Dict[str, Any]]) -> None:
         """
         Replaces start and end dates of the additional date intervals in the row set with their integer representation
 
-        :param list[tuple[str,str]] keys: The other keys with start and end date.
-        :param list[dict[str,T]] rows: The list of rows.
-
-        :rtype: list[dict[str,T]]
+        :param keys: The other keys with start and end date.
+        :param rows: The list of rows.
         """
         for row in rows:
             for key_start_date, key_end_date in keys:
                 if key_start_date not in [self._key_start_date, self._key_end_date]:
                     row[key_start_date] = self._date2int(row[key_start_date])
                 if key_end_date not in [self._key_start_date, self._key_end_date]:
                     row[key_end_date] = self._date2int(row[key_end_date])
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _intersection(self, keys, rows):
+    def _intersection(self, keys: List[Tuple[str, str]], rows: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
         """
         Computes the intersection of the date intervals of two or more reference data sets. If the intersection is empty
         the row is removed from the group.
 
-        :param list[tuple[str,str]] keys: The other keys with start and end date.
-        :param list[dict[str,T]] rows: The list of rows.
-
-        :rtype: list[dict[str,T]]
+        :param keys: The other keys with start and end date.
+        :param rows: The list of rows.
         """
         # If there are no other keys with start and end date (i.e. nothing to merge) return immediately.
         if not keys:
             return rows
 
         ret = list()
         for row in rows:
@@ -79,19 +75,19 @@
                 row[self._key_start_date] = start_date
                 row[self._key_end_date] = end_date
                 ret.append(row)
 
         return ret
 
     # ------------------------------------------------------------------------------------------------------------------
-    def merge(self, keys):
+    def merge(self, keys: List[Tuple[str, str]]) -> None:
         """
         Merges the join on pseudo keys of two or more reference data sets.
 
-        :param list[tuple[str,str]] keys: For each data set the keys of the start and end date.
+        :param keys: For each data set the keys of the start and end date.
         """
         deletes = []
         for pseudo_key, rows in self._rows.items():
             self._additional_rows_date2int(keys, rows)
             rows = self._intersection(keys, rows)
             if rows:
                 rows = self._rows_sort(rows)
```

### Comparing `ETLT-0.9.6/etlt/reader/Reader.py` & `etlt-1.0.0/etlt/reader/Reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,65 @@
 import abc
 import copy
+from typing import List, Optional
 
 
 class Reader(metaclass=abc.ABCMeta):
     """
     Abstract parent class for reading (directly or indirectly) rows from the source.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def __init__(self):
         """
         Object constructor.
         """
-        self._fields = None
-        """
-        The fields (or columns) that this reader will read from the source.
 
-        :type: list[str]|None
+        self._fields: Optional[List[str]] = None
+        """
+        The mapping from field (columns) names to the column numbers in the CSV files.
         """
 
-        self._row_number = -1
+        self._row_number: int = -1
         """
         The row number for identifying the row in the source data.
-
-        :type: int
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     @property
-    def fields(self):
+    def fields(self) -> Optional[List[str]]:
         """
         Getter for fields.
-
-        :rtype: list[str]|None
         """
         return copy.copy(self._fields)
 
     # ------------------------------------------------------------------------------------------------------------------
     @fields.setter
-    def fields(self, fields):
+    def fields(self, fields: Optional[List[str]]) -> None:
         """
         Setter for fields. If set to None this reader yields each row from the source as a list. If set to a list of
         field names this reader yields each row from the source as a dictionary using the given field names.
 
-        :param list[str]|None fields: The fields (or columns) that must be read from the source.
+        :param fields: The fields (or columns) that must be read from the source.
         """
         self._fields = fields
 
     # ------------------------------------------------------------------------------------------------------------------
     @property
-    def row_number(self):
+    def row_number(self) -> int:
         """
         Getter for row count.
-
-        :rtype: int
         """
         return self._row_number
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
-    def get_source_name(self):
+    def get_source_name(self) -> str:
         """
         Returns a name for identifying the current source.
-
-        :rtype: str
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def next(self):
         """
```

### Comparing `ETLT-0.9.6/etlt/reader/UniversalCsvReader.py` & `etlt-1.0.0/etlt/reader/UniversalCsvReader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,206 +1,221 @@
 import bz2
+import copy
 import csv
 from itertools import zip_longest
+from typing import Dict, List, Optional, Union
 
 import chardet
 
 from etlt.reader.Reader import Reader
 from etlt.reader.UniversalCsvReaderFormatHelper import UniversalCsvReaderFormatHelper
 
 
 class UniversalCsvReader(Reader):
     """
-    An universal CSV file reader.
+    A universal CSV file reader.
     - Open uncompressed and gz, bz2 compressed files.
     - Auto encoding and field delimiter detection.
     """
     sample_size = 64 * 1024
 
     line_endings = ['\r\n', '\n\r', '\n', '\r']
 
     delimiters = [',', ';', '\t', '|', ':']
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, filenames, format_helper=None):
+    def __init__(self, filenames: List[str], format_helper=None):
         """
         Object constructor.
 
         :param list(str) filenames: A list of CSV file names.
         """
         Reader.__init__(self)
 
-        self._filenames = filenames
+        self._filenames: List[str] = filenames
         """
         The name of the CSV files.
-
-        :type: list
         """
 
         self._file = None
         """
         The current actual file object.
         """
 
         self._csv_reader = None
         """
         The current actual CSV file object.
 
         :type: _csv.reader
         """
 
-        self._filename = None
+        self._mapping: Optional[Dict[str, int]] = None
+        """
+        The mapping from column names to column numbers.
         """
-        The name of the current file.
 
-        :type: str|None
+        self._filename: Optional[str] = None
+        """
+        The name of the current file.
         """
 
         self._helper = UniversalCsvReaderFormatHelper() if not format_helper else format_helper
         """
         The helper for detecting the appropriate formatting parameters for reading the current CSV file.
-
-        :type: etlt.reader.UniversalCsvReaderFormatHelper.UniversalCsvReaderFormatHelper
         """
 
-        self._formatting_parameters = dict()
+        self._formatting_parameters: Dict[str, str] = dict()
         """
         The CSV formatting parameters for reading the current CSV file.
-
-        :type: dict[str,str]
         """
 
-        self._sample = None
+        self._sample: Optional[Union[str, bytes]] = None
         """
         The sample when detecting automatically formatting parameters.
-
-        :type: None|str|bytes
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     def __enter__(self):
         # Nothing to do.
         pass
 
     # ------------------------------------------------------------------------------------------------------------------
     def __exit__(self, *_):
         self._close()
 
     # ------------------------------------------------------------------------------------------------------------------
-    def get_source_name(self):
+    def get_source_name(self) -> Optional[str]:
         """
         Returns the current source file.
-
-        :rtype str|None:
         """
         return self._filename
 
     # ------------------------------------------------------------------------------------------------------------------
     def next(self):
         """
         Yields the next row from the source files.
         """
         for self._filename in self._filenames:
             self._open()
             for row in self._csv_reader:
                 self._row_number += 1
-                if self._fields:
+                if self._mapping:
+                    yield {column_name: row[index] if 0 <= index < len(row) else '' for column_name, index in
+                           self._mapping.items()}
+                elif self._fields:
                     yield dict(zip_longest(self._fields, row, fillvalue=''))
                 else:
                     yield row
+
             self._close()
             self._row_number = -1
 
         self._filename = None
 
         return
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _open_file(self, mode, encoding=None):
+    @property
+    def mapping(self) -> Optional[Dict[str, int]]:
+        """
+        Getter for mapping.
+        """
+        return copy.copy(self._mapping)
+
+    # ------------------------------------------------------------------------------------------------------------------
+    @mapping.setter
+    def mapping(self, mapping: Optional[Dict[str, int]]):
+        """
+
+        """
+        self._mapping = mapping
+
+    # ------------------------------------------------------------------------------------------------------------------
+    def _open_file(self, mode: str, encoding: Optional[str] = None) -> None:
         """
         Opens the next current file.
 
-        :param str mode: The mode for opening the file.
-        :param str encoding: The encoding of the file.
+        :param mode: The mode for opening the file.
+        :param encoding: The encoding of the file.
         """
         if self._filename[-4:] == '.bz2':
             self._file = bz2.open(self._filename, mode=mode, encoding=encoding)
         else:
             self._file = open(self._filename, mode=mode, encoding=encoding)
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _close(self):
+    def _close(self) -> None:
         """
         Closes the current file.
         """
         if self._file:
             self._file.close()
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _get_sample(self, mode, encoding):
+    def _get_sample(self, mode: str, encoding: Optional[str]) -> None:
         """
         Get a sample from the next current input file.
 
         :param str mode: The mode for opening the file.
         :param str|None encoding: The encoding of the file. None for open the file in binary mode.
         """
         self._open_file(mode, encoding)
         self._sample = self._file.read(UniversalCsvReader.sample_size)
         self._file.close()
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _detect_encoding(self):
+    def _detect_encoding(self) -> None:
         """
         Detects the encoding og the current file.
-        :return:
         """
         self._formatting_parameters['encoding'] = chardet.detect(self._sample)['encoding']
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _detect_delimiter(self):
+    def _detect_delimiter(self) -> None:
         """
         Detects the field delimiter in the sample data.
         """
         candidate_value = ','
         candidate_count = 0
         for delimiter in UniversalCsvReader.delimiters:
             count = self._sample.count(delimiter)
             if count > candidate_count:
                 candidate_value = delimiter
                 candidate_count = count
 
         self._formatting_parameters['delimiter'] = candidate_value
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _detect_line_ending(self):
+    def _detect_line_ending(self) -> None:
         """
         Detects the line ending in the sample data.
         """
         candidate_value = '\n'
         candidate_count = 0
         for line_ending in UniversalCsvReader.line_endings:
             count = self._sample.count(line_ending)
             if count > candidate_count:
                 candidate_value = line_ending
                 candidate_count = count
 
         self._formatting_parameters['line_terminator'] = candidate_value
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _open(self):
+    def _open(self) -> None:
         """
         Opens the next current file with proper settings for encoding and delimiter.
         """
         self._sample = None
 
-        formatting_parameters0 = {'encoding':        'auto',
-                                  'delimiter':       'auto',
-                                  'line_terminator': 'auto',
-                                  'escape_char':     '\\',
-                                  'quote_char':      '"'}
+        formatting_parameters0 = {
+                'encoding':        'auto',
+                'delimiter':       'auto',
+                'line_terminator': 'auto',
+                'escape_char':     '\\',
+                'quote_char':      '"'}
         formatting_parameters1 = self._helper.pass1(self._filename, formatting_parameters0)
         self._formatting_parameters = formatting_parameters1
 
         # Detect encoding.
         if formatting_parameters1['encoding'] == 'auto':
             self._get_sample('rb', None)
             self._detect_encoding()
```

### Comparing `ETLT-0.9.6/etlt/reader/UniversalCsvReaderFormatHelper.py` & `etlt-1.0.0/etlt/reader/UniversalCsvReaderFormatHelper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,45 @@
+from typing import Dict
+
+
 class UniversalCsvReaderFormatHelper:
     """
     A helper class for UniversalCsvReader for setting and correcting the formatting parameters for reading CSV files.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def pass1(self, filename, formatting_parameters0):
+    def pass1(self, filename: str, formatting_parameters: Dict[str, str]) -> Dict[str, str]:
         """
         Returns the formatting parameters for reading the next current CSV file.
 
-        This method is called by UniversalCsvReader before opening the CSV file and before auto detecting parameters.
+        This method is called by UniversalCsvReader before opening the CSV file and before auto-detecting parameters.
 
         Override this method in your own child class according to your needs.
 
         :param str filename: The next current file name.
-        :param dict[str,str] formatting_parameters0: The default formatting parameters. Keys are:
-                                                     - encoding: Use auto for auto detecting.
-                                                     - delimiter: Use auto for auto detecting.
-                                                     - line_terminator: Use auto for auto detecting.
+        :param dict[str,str] formatting_parameters: The default formatting parameters. Keys are:
+                                                     - encoding: Use auto for auto-detecting.
+                                                     - delimiter: Use auto for auto-detecting.
+                                                     - line_terminator: Use auto for auto-detecting.
                                                      - escape_char
                                                      - quote_char
-
-        :rtype: dict[str,str]
         """
-        return formatting_parameters0
+        return formatting_parameters
 
     # ------------------------------------------------------------------------------------------------------------------
-    def pass2(self, filename, formatting_parameters1, formatting_parameters2):
+    def pass2(self, filename: str, formatting_parameters1: Dict[str, str], formatting_parameters2: Dict[str, str]) -> \
+            Dict[str, str]:
         """
         Returns the formatting parameters for reading the next current CSV file.
 
-        This method is called by UniversalCsvReader after auto detecting parameters.
+        This method is called by UniversalCsvReader after auto-detecting parameters.
 
         Override this method in your own child class according to your needs.
 
         :param str filename: The next current file name.
         :param dict[str,str] formatting_parameters1: The formatting parameters as returned by pass1.
         :param dict[str,str] formatting_parameters2: The formatting parameters as returned by pass1 but parameters set
                                                      to auto are replaced with the automatically detected values.
-
-        :rtype: dict[str,str]
         """
         return formatting_parameters2
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `ETLT-0.9.6/etlt/writer/SqlLoaderWriter.py` & `etlt-1.0.0/etlt/writer/SqlLoaderWriter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import abc
+from typing import Any, Optional
 
 from etlt.writer.Writer import Writer
 
 
 class SqlLoaderWriter(Writer):
     """
     Abstract parent class for loading rows to a table in a database using a SQL statement for loading data from file.
@@ -11,102 +12,91 @@
     """
     The handlers for writing objects as a field to a CSV file.
 
     :type: dict[str,callable]
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, filename, encoding='utf8'):
+    def __init__(self, filename: str, encoding: str = 'utf8'):
         """
         Object constructor.
 
-        :param str filename: The destination file for the rows.
-        :param str encoding: The encoding of the text of the destination file.
+        :param filename: The destination file for the rows.
+        :param encoding: The encoding of the text of the destination file.
         """
         Writer.__init__(self)
 
-        self._filename = filename
+        self._filename: str = filename
         """
         The name of the destination file.
-
-        :type: str
         """
 
-        self._encoding = encoding
+        self._encoding: str = encoding
         """
         The encoding of the text in the destination file.
-
-        :type: str
         """
 
-        self._file = None
+        self._file: Any = None
         """
         The underling file object.
-
-        :type: T
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     def __enter__(self):
         self._file = open(self._filename, mode='wt', encoding=self._encoding)
 
     # ------------------------------------------------------------------------------------------------------------------
     def __exit__(self, exc_type, exc_value, traceback):
         self._file.close()
 
     # ------------------------------------------------------------------------------------------------------------------
     @property
-    def filename(self):
+    def filename(self) -> str:
         """
-        Getter for filename.
-
-        :rtype: str
+        Returns the filename.
         """
         return self._filename
 
     # ------------------------------------------------------------------------------------------------------------------
     @property
-    def encoding(self):
+    def encoding(self) -> str:
         """
-        Getter for encoding.
-
-        :rtype: str
+        Returns the encoding.
         """
         return self._encoding
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
-    def get_bulk_load_sql(self, table_name):
+    def get_bulk_load_sql(self, table_name: str, partition: Optional[str] = None) -> str:
         """
         Returns a SQL statement for bulk loading the data writen to the destination file into a table.
 
-        :param str table_name: The name of the table.
-
-        :rtype: str
+        :param table_name: The name of the table.
+        :param partition: When applicable, the name of the partition in which the data must be loaded.`
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def register_handler(class_name, handler):
+    def register_handler(class_name: str, handler: callable) -> None:
         """
         Registers a handler for writing instances of a class as a field to the destination file.
 
-        :param str class_name: The name of the class.
-        :param callable handler: The handler. This handler will be called with two arguments: the object which value
-                                 must be writen to the destination file, the file handler.
+        :param class_name: The name of the class.
+        :param handler: The handler. This handler will be called with two arguments: the object which value must be
+                        writen to the destination file, the file handler.
         """
         SqlLoaderWriter.handlers[class_name] = handler
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _write_field(self, value):
+    def _write_field(self, value: Any):
         """
-        Write a single field to the destination file.
+        Writes a single field to the destination file.
 
-        :param T value: The value of the field.
+        :param value: The value of the field.
         """
         class_name = str(value.__class__)
         if class_name not in self.handlers:
             raise ValueError('No handler has been registered for class: {0!s}'.format(class_name))
         handler = self.handlers[class_name]
         handler(value, self._file)
```

