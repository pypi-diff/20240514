# Comparing `tmp/ETLT-MySQL-0.10.1.tar.gz` & `tmp/etlt_mysql-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ETLT-MySQL-0.10.1.tar", last modified: Mon Oct 26 17:45:42 2020, max compression
+gzip compressed data, was "etlt_mysql-1.0.0.tar", max compression
```

## Comparing `ETLT-MySQL-0.10.1.tar` & `etlt_mysql-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,9 @@
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:45:42.199103 ETLT-MySQL-0.10.1/
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:45:42.193103 ETLT-MySQL-0.10.1/ETLT_MySQL.egg-info/
--rw-rw-r--   0 water     (1000) water     (1000)     4375 2020-10-26 17:45:42.000000 ETLT-MySQL-0.10.1/ETLT_MySQL.egg-info/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)      341 2020-10-26 17:45:42.000000 ETLT-MySQL-0.10.1/ETLT_MySQL.egg-info/SOURCES.txt
--rw-rw-r--   0 water     (1000) water     (1000)        1 2020-10-26 17:45:42.000000 ETLT-MySQL-0.10.1/ETLT_MySQL.egg-info/dependency_links.txt
--rw-rw-r--   0 water     (1000) water     (1000)       31 2020-10-26 17:45:42.000000 ETLT-MySQL-0.10.1/ETLT_MySQL.egg-info/requires.txt
--rw-rw-r--   0 water     (1000) water     (1000)       16 2020-10-26 17:45:42.000000 ETLT-MySQL-0.10.1/ETLT_MySQL.egg-info/top_level.txt
--rw-rw-r--   0 water     (1000) water     (1000)     4375 2020-10-26 17:45:42.198103 ETLT-MySQL-0.10.1/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)     3481 2020-10-26 17:30:28.000000 ETLT-MySQL-0.10.1/README.rst
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:45:42.194103 ETLT-MySQL-0.10.1/etlt_mysql/
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-MySQL-0.10.1/etlt_mysql/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:45:42.195103 ETLT-MySQL-0.10.1/etlt_mysql/writer/
--rw-rw-r--   0 water     (1000) water     (1000)     6985 2020-10-26 17:29:23.000000 ETLT-MySQL-0.10.1/etlt_mysql/writer/MySqlLoaderWriter.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-MySQL-0.10.1/etlt_mysql/writer/__init__.py
--rw-rw-r--   0 water     (1000) water     (1000)       38 2020-10-26 17:45:42.200103 ETLT-MySQL-0.10.1/setup.cfg
--rw-rw-r--   0 water     (1000) water     (1000)     1198 2020-10-26 17:45:33.000000 ETLT-MySQL-0.10.1/setup.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:45:42.188103 ETLT-MySQL-0.10.1/test/
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 17:45:42.197103 ETLT-MySQL-0.10.1/test/writer/
--rw-rw-r--   0 water     (1000) water     (1000)     3043 2016-09-05 08:43:02.000000 ETLT-MySQL-0.10.1/test/writer/MySqlLoaderWriterTest.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:29.000000 ETLT-MySQL-0.10.1/test/writer/__init__.py
+-rw-r--r--   0        0        0     1092 2016-07-17 10:14:05.000000 etlt_mysql-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1443 2024-05-14 05:06:00.683088 etlt_mysql-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:29.000000 etlt_mysql-1.0.0/etlt_mysql/__init__.py
+-rw-r--r--   0        0        0     7063 2024-05-14 04:55:05.312772 etlt_mysql-1.0.0/etlt_mysql/writer/MySqlLoaderWriter.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:29.000000 etlt_mysql-1.0.0/etlt_mysql/writer/__init__.py
+-rw-r--r--   0        0        0     8251 2024-05-14 04:57:31.333968 etlt_mysql-1.0.0/etlt_mysql/writer/__pycache__/MySqlLoaderWriter.cpython-312.pyc
+-rw-r--r--   0        0        0      158 2024-05-14 04:57:31.332968 etlt_mysql-1.0.0/etlt_mysql/writer/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      986 2024-05-14 05:10:31.447024 etlt_mysql-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2421 1970-01-01 00:00:00.000000 etlt_mysql-1.0.0/PKG-INFO
```

### Comparing `ETLT-MySQL-0.10.1/etlt_mysql/writer/MySqlLoaderWriter.py` & `etlt_mysql-1.0.0/etlt_mysql/writer/MySqlLoaderWriter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import os
 from abc import ABC
 from decimal import Decimal
-from typing import Any, Dict
+from typing import Any, Dict, Optional
+from uuid import UUID
 
 import pytz
 from etlt.writer.SqlLoaderWriter import SqlLoaderWriter
 
 
 class MySqlLoaderWriter(SqlLoaderWriter, ABC):
     """
@@ -16,162 +17,162 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def write_bool(value: bool, file: Any) -> None:
         """
         Writes a boolean as a field to a CSV file.
 
-        :param bool value: The boolean.
-        :param Any file: The file like object
+        :param value: The boolean.
+        :param file: The file like object
         """
         if value:
             file.write('1')
         else:
             file.write('0')
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def write_date(value: datetime.date, file: Any) -> None:
         """
         Writes a date as a field to a CSV file.
 
-        :param datetime.date value: The date.
-        :param Any file: The file like object
+        :param value: The date.
+        :param file: The file like object
         """
         file.write(value.isoformat())
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def write_datetime(value: datetime.datetime, file: Any) -> None:
         """
         Writes a datetime as a field to a CSV file.
 
-        :param datetime.datetime value: The date.
-        :param Any file: The file like object
+        :param value: The date.
+        :param file: The file like object
         """
         zone = value.tzinfo
         if zone and zone != pytz.utc:
             raise ValueError('Only native and UTC timezone supported')
         file.write(value.isoformat())
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def write_timedelta(value: datetime.timedelta, file: Any) -> None:
         """
         Writes a timedelta as a field to a CSV file.
 
-        :param datetime.timedelta value: The timedelta.
-        :param Any file: The file like object
+        :param value: The timedelta.
+        :param file: The file like object
         """
         MySqlLoaderWriter.write_string(str(value), file)
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def write_decimal(value: Decimal, file: Any) -> None:
         """
         Writes a decimal as a field to a CSV file.
 
-        :param Decimal value: The decimal.
-        :param Any file: The file like object
+        :param value: The decimal.
+        :param file: The file like object
         """
         file.write(str(value))
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def write_float(value: float, file: Any) -> None:
         """
         Writes a float as a field to a CSV file.
 
-        :param float value: The float.
-        :param Any file: The file like object
+        :param value: The float.
+        :param file: The file like object
         """
         file.write(str(value))
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def write_int(value: int, file: Any) -> None:
         """
         Writes an integer as a field to a CSV file.
 
-        :param int value: The integer.
-        :param Any file: The file like object
+        :param value: The integer.
+        :param file: The file like object
         """
         file.write(str(value))
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def write_none(_, file: Any) -> None:
         """
         Writes None as a field to a CSV file.
 
-        :param None _: The None object.
-        :param Any file: The file like object
+        :param _: The None object.
+        :param file: The file like object
         """
         file.write('\\N')
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def write_string(value: str, file: Any) -> None:
         """
         Writes a string as a field to a CSV file.
 
-        :param str value: The string.
-        :param Any file: The file.
+        :param value: The string.
+        :param file: The file.
         """
         if value == '':
             file.write('\\N')
         else:
             file.write("'")
             file.write(value.replace('\\', '\\\\').replace("'", "\\'"))
             file.write("'")
 
     # ------------------------------------------------------------------------------------------------------------------
     def writerow(self, row: Dict[str, Any]) -> None:
         """
         Writes a row to the destination file.
 
-        :param dict[str,Any] row: The row.
+        :param row: The row.
         """
         for field in self._fields:
             self._write_field(row[field])
             self._file.write(',')
 
         self._file.write(os.linesep)
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def write_uuid(value, file: Any) -> None:
+    def write_uuid(value: UUID, file: Any) -> None:
         """
         Writes a UUID as a field to a CSV file.
 
-        :param uuid.UUID value: The UUID.
-        :param Any file: The file like object
+        :param value: The UUID.
+        :param file: The file like object
         """
         MySqlLoaderWriter.write_string(str(value), file)
 
     # ------------------------------------------------------------------------------------------------------------------
-    def get_bulk_load_sql(self, table_name: str) -> str:
+    def get_bulk_load_sql(self, table_name: str, partition: Optional[str] = None) -> str:
         """
         Returns a SQL statement for bulk loading the data into a table.
 
-        :param str table_name: The name of the table.
-
-        :rtype: str
+        :param table_name: The name of the table.
+        :param partition: When applicable, the name of the partition in which the data must be loaded.`
         """
         sql = "load data local infile '{FILENAME}'"
         sql += ' into table `{TABLE_NAME}`'
+        if partition is not None:
+            sql += ' partition ({PARTITION})'
         sql += ' character set {ENCODING}'
         sql += " fields terminated by ','"
         sql += " optionally enclosed by '\\\''"
         sql += " escaped by '\\\\'"
         sql += " lines terminated by '\\n'"
 
         return sql.format(FILENAME=self._filename,  # @todo Quoting of filename
-                          ENCODING=self._encoding,
-                          TABLE_NAME=table_name)
+                          ENCODING=self._encoding, TABLE_NAME=table_name, PARTITION=partition)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 MySqlLoaderWriter.register_handler("<class 'bool'>", MySqlLoaderWriter.write_bool)
 MySqlLoaderWriter.register_handler("<class 'datetime.date'>", MySqlLoaderWriter.write_date)
 MySqlLoaderWriter.register_handler("<class 'datetime.datetime'>", MySqlLoaderWriter.write_datetime)
 MySqlLoaderWriter.register_handler("<class 'datetime.timedelta'>", MySqlLoaderWriter.write_timedelta)
```

