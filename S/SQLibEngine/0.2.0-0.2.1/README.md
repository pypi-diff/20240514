# Comparing `tmp/SQLibEngine-0.2.0.tar.gz` & `tmp/SQLibEngine-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLibEngine-0.2.0.tar", last modified: Sat May 11 14:23:43 2024, max compression
+gzip compressed data, was "SQLibEngine-0.2.1.tar", last modified: Tue May 14 13:28:08 2024, max compression
```

## Comparing `SQLibEngine-0.2.0.tar` & `SQLibEngine-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:23:43.923232 SQLibEngine-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-11 14:23:43.923232 SQLibEngine-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:23:43.923232 SQLibEngine-0.2.0/SQLib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:23:43.923232 SQLibEngine-0.2.0/SQLib/Database/
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/SQLib/Database/Connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/SQLib/Database/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/SQLib/Database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:23:43.923232 SQLibEngine-0.2.0/SQLib/SQLEngine/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/SQLib/SQLEngine/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/SQLib/SQLEngine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/SQLib/SQLEngine/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/SQLib/SQLEngine/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/SQLib/SQLEngine/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/SQLib/SQLEngine/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/SQLib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:23:43.923232 SQLibEngine-0.2.0/SQLibEngine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-11 14:23:43.000000 SQLibEngine-0.2.0/SQLibEngine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-11 14:23:43.000000 SQLibEngine-0.2.0/SQLibEngine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:23:43.000000 SQLibEngine-0.2.0/SQLibEngine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 14:23:43.000000 SQLibEngine-0.2.0/SQLibEngine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 14:23:43.923232 SQLibEngine-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-11 14:23:32.000000 SQLibEngine-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:08.070773 SQLibEngine-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-14 13:28:08.066773 SQLibEngine-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:08.066773 SQLibEngine-0.2.1/SQLib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:08.066773 SQLibEngine-0.2.1/SQLib/Database/
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/Database/Connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/Database/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/Database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:08.066773 SQLibEngine-0.2.1/SQLib/SQLEngine/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/SQLEngine/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/SQLEngine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/SQLEngine/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/SQLEngine/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/SQLEngine/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/SQLEngine/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:08.066773 SQLibEngine-0.2.1/SQLibEngine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-14 13:28:08.000000 SQLibEngine-0.2.1/SQLibEngine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-14 13:28:08.000000 SQLibEngine-0.2.1/SQLibEngine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:28:08.000000 SQLibEngine-0.2.1/SQLibEngine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 13:28:08.000000 SQLibEngine-0.2.1/SQLibEngine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:28:08.070773 SQLibEngine-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/setup.py
```

### Comparing `SQLibEngine-0.2.0/LICENSE` & `SQLibEngine-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.2.0/PKG-INFO` & `SQLibEngine-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLibEngine
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple SQLite3 wrapper for Python
 Home-page: https://github.com/TRC-Loop/SQLib
 Author: AK
 Author-email: ak@stellar-code.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SQLibEngine-0.2.0/README.md` & `SQLibEngine-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.2.0/SQLib/Database/Connection.py` & `SQLibEngine-0.2.1/SQLib/Database/Connection.py`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.2.0/SQLib/SQLEngine/operations.py` & `SQLibEngine-0.2.1/SQLib/SQLEngine/operations.py`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.2.0/SQLib/SQLEngine/tables.py` & `SQLibEngine-0.2.1/SQLib/SQLEngine/tables.py`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.2.0/SQLib/SQLEngine/util.py` & `SQLibEngine-0.2.1/SQLib/SQLEngine/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import re
 
-def is_sql(string: str) -> bool:
+def is_sql(string: str, sql_keywords: list[str] = ["SELECT", "INSERT", "UPDATE", "DELETE", "CREATE", "DROP", "ALTER", "JOIN", "FROM", "WHERE", "AND", "OR", "IN", "NOT", "NULL", "ORDER BY", "GROUP BY", "HAVING", "LIMIT", "UNION" ]) -> bool:
     """
     Check if a string contains SQL keywords.
     
     :param string: The string to check.
     
     :return: True if the string contains SQL keywords, False otherwise.
     """
-    sql_keywords = [
-        "SELECT", "INSERT", "UPDATE", "DELETE", "CREATE", "DROP",
-        "ALTER", "JOIN", "FROM", "WHERE", "AND", "OR", "IN", "NOT",
-        "NULL", "ORDER BY", "GROUP BY", "HAVING", "LIMIT", "UNION"
-    ]
+    
     regex = r'\b(?:' + '|'.join(sql_keywords) + r')\b'
     return bool(re.search(regex, string.upper()))
```

### Comparing `SQLibEngine-0.2.0/SQLibEngine.egg-info/PKG-INFO` & `SQLibEngine-0.2.1/SQLibEngine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLibEngine
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple SQLite3 wrapper for Python
 Home-page: https://github.com/TRC-Loop/SQLib
 Author: AK
 Author-email: ak@stellar-code.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SQLibEngine-0.2.0/setup.py` & `SQLibEngine-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the README.md file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="SQLibEngine",
-    version="0.2.0",
+    version="0.2.1",
     author="AK",
     author_email="ak@stellar-code.com",
     url="https://github.com/TRC-Loop/SQLib",
     description="A simple SQLite3 wrapper for Python",
     long_description=long_description,  # Set the long description
     long_description_content_type="text/markdown",  # Specify the content type
     packages=find_packages(),
```

