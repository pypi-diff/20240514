# Comparing `tmp/ehdtd-0.2.3.tar.gz` & `tmp/ehdtd-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd-0.2.3.tar", max compression
+gzip compressed data, was "ehdtd-0.2.5.tar", max compression
```

## Comparing `ehdtd-0.2.3.tar` & `ehdtd-0.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.2.3/LICENSE
--rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.2.3/README.md
--rw-r--r--   0        0        0      952 2024-04-12 05:36:22.441712 ehdtd-0.2.3/ehdtd/__init__.py
--rw-r--r--   0        0        0    23764 2024-04-07 11:48:58.674464 ehdtd-0.2.3/ehdtd/binance.py
--rw-r--r--   0        0        0   121818 2024-05-08 17:25:12.689950 ehdtd-0.2.3/ehdtd/ehdtd.py
--rw-r--r--   0        0        0     6539 2024-04-07 09:34:20.505668 ehdtd-0.2.3/ehdtd/ehdtd_common_functions.py
--rw-r--r--   0        0        0      705 2024-05-08 17:27:53.764861 ehdtd-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.2.5/README.md
+-rw-r--r--   0        0        0      952 2024-04-12 05:36:22.441712 ehdtd-0.2.5/ehdtd/__init__.py
+-rw-r--r--   0        0        0    23764 2024-04-07 11:48:58.674464 ehdtd-0.2.5/ehdtd/binance.py
+-rw-r--r--   0        0        0   120405 2024-05-14 08:08:35.324906 ehdtd-0.2.5/ehdtd/ehdtd.py
+-rw-r--r--   0        0        0     6539 2024-04-07 09:34:20.505668 ehdtd-0.2.5/ehdtd/ehdtd_common_functions.py
+-rw-r--r--   0        0        0      705 2024-05-14 08:11:25.231141 ehdtd-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.2.5/PKG-INFO
```

### Comparing `ehdtd-0.2.3/LICENSE` & `ehdtd-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.3/README.md` & `ehdtd-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.3/ehdtd/__init__.py` & `ehdtd-0.2.5/ehdtd/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.3/ehdtd/binance.py` & `ehdtd-0.2.5/ehdtd/binance.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.3/ehdtd/ehdtd.py` & `ehdtd-0.2.5/ehdtd/ehdtd.py`

 * *Files 0% similar despite different names*

```diff
@@ -2822,48 +2822,31 @@
         'db_name': 'ehdtd',
         'db_user': 'ehdtd',
         'db_pass': 'xxxxxxxxx',
         'db_host': '127.0.0.1',
         'db_port': '5432'
     }
 
-    fetch_data = [
-        {
-            'symbol': symbol,
-            'interval': interval
-        }
     ]
 
-    ehd_ro = EhdtdRO(exchange, fetch_data, db_data)  # Create an instance
+    ehd_ro = EhdtdRO(exchange, db_data)  # Create an instance
 
     ```
     """
 
     def __init__(self,\
                  exchange,\
-                 fetch_data: list[dict],\
                  db_data: dict,\
                  trading_type: str='SPOT',\
                  debug: bool=False):
         """
         EhdtdRO constructor
         =================
             :param self: EhdtdRO instance.
             :param exchange: str exchange name.
-            :param fetch_data: list[dict]
-                                    dicts must have this struct.
-                                        {
-                                            'symbol': 'BTC/USDT',
-                                            'interval': '1d'
-                                        }
-
-                                            symbol: str valid symbol for exchange name.
-                                            interval: str '1m', '3m', '5m', '15m', '30m',
-                                                        '1h', '2h', '4h', '6h', '8h',
-                                                        '12h', '1d', '3d', '1w', '1mo'
 
             :param db_data: dict
                                 dict must have dist struct
                                     {
                                         db_type: str, #Only supported 'postgresql' and 'mysql'.
                                         db_name: str, #Database name.
                                         db_user: str, #Database user.
@@ -2879,15 +2862,14 @@
         """
 
         self.__db_type = None
         self.__db_name = None
         self.__db_engine = None
         self.__db_conn = None
         self.__exchange = None
-        self.__fetch_data = fetch_data
         self.__trading_type = None
         self.__debug = debug
 
         if self.__debug is None or not isinstance(self.__debug, bool):
             err_msg = 'debug must be boolean True or False'
             raise ValueError(err_msg)
 
@@ -2958,72 +2940,65 @@
                 err_msg = 'Wrong database data'
                 raise ValueError(err_msg)
 
         else:
             err_msg = 'Wrong database data'
             raise ValueError(err_msg)
 
-        if not self.__check_fetch_data_struct(self.__fetch_data):
-            err_msg = 'Wrong fetch data'
-            raise ValueError(err_msg)
-
-    def __check_fetch_data_struct(self, fecth_data):
-        """
-        __check_fetch_data_struct
-        =========================
-            This method return true if fetch_data struct it is correct
-                :param self: This instance.
-                :param fetch_data: list[dict].
-
-                :return: bool.
-        """
-
-        result = False
-
-        if fecth_data is not None and isinstance(fecth_data, list) and len(fecth_data) > 0:
-            result = True
-
-            for data_n in fecth_data:
-                result = result and isinstance(data_n, dict)\
-                    and data_n is not None\
-                    and 'symbol' in data_n\
-                    and 'interval' in data_n and isinstance(data_n['symbol'], str)\
-                    and isinstance(data_n['interval'], str)
-                if result:
-                    table_name = self.__get_table_name(data_n['symbol'], data_n['interval'])
-                    result = result and self.__check_table_exists(table_name)
-
-        return result
-
     def __check_table_exists(self, table_name):
         result = False
 
         metadata = sqlalchemy.MetaData()
         metadata.reflect(bind=self.__db_engine)
 
         try:
             table = metadata.tables[table_name] # pylint: disable=unused-variable
             result = True
         except Exception: # pylint: disable=broad-except
             result = False
 
         return result
 
+    def check_if_exists_symbol_interval(self, symbol, interval):
+        """
+        check_if_exists_symbol_interval
+        ===============================
+        Check the connection to a database.
+
+        Parameters:
+            :param self: EhdtdRO instance.
+            :param symbol: str.
+            :param interval: str.
+
+        Returns:
+            :return bool: True if the symbol interval exists in db
+
+        """
+
+        result = False
+
+        __table_name = self.__get_table_name(symbol, interval)
+
+        if self.__check_table_exists(__table_name):
+            result = True
+
+        return result
+
     def __check_database_connection(self):
         """
         check_database_connection
         =========================
 
         Check the connection to a database.
 
         Parameters:
-            self: EhdtdRO instance.
+            :param self: EhdtdRO instance.
 
         Returns:
-            bool: True if the connection is successful, False otherwise.
+            :return bool: True if the connection is successful, False otherwise.
         """
         result = False
 
         try:
             engine = sqlalchemy.create_engine(self.__db_uri)
             with engine.connect() as connection: # pylint: disable=unused-variable
                 result = True
```

### Comparing `ehdtd-0.2.3/ehdtd/ehdtd_common_functions.py` & `ehdtd-0.2.5/ehdtd/ehdtd_common_functions.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.3/pyproject.toml` & `ehdtd-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ehdtd"
-version = "0.2.3"
+version = "0.2.5"
 description = "Ehdtd - cryptoCurrency Exchange history data to database"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/rmalvarezkai/ehdtd"
 
 [tool.poetry.dependencies]
```

### Comparing `ehdtd-0.2.3/PKG-INFO` & `ehdtd-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd
-Version: 0.2.3
+Version: 0.2.5
 Summary: Ehdtd - cryptoCurrency Exchange history data to database
 Home-page: https://github.com/rmalvarezkai/ehdtd
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

