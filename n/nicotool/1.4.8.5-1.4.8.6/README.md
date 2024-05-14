# Comparing `tmp/nicotool-1.4.8.5.tar.gz` & `tmp/nicotool-1.4.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicotool-1.4.8.5.tar", last modified: Mon May 13 11:40:10 2024, max compression
+gzip compressed data, was "nicotool-1.4.8.6.tar", last modified: Tue May 14 12:36:43 2024, max compression
```

## Comparing `nicotool-1.4.8.5.tar` & `nicotool-1.4.8.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 11:40:10.664332 nicotool-1.4.8.5/
--rw-rw-rw-   0        0        0      307 2024-05-13 11:40:10.663328 nicotool-1.4.8.5/PKG-INFO
--rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 nicotool-1.4.8.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 11:40:10.631520 nicotool-1.4.8.5/nicotool/
--rw-rw-rw-   0        0        0     3963 2024-05-12 11:41:14.000000 nicotool-1.4.8.5/nicotool/__init__.py
--rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 nicotool-1.4.8.5/nicotool/additional_functions.py
--rw-rw-rw-   0        0        0    15433 2024-05-13 11:39:32.000000 nicotool-1.4.8.5/nicotool/ascii.py
--rw-rw-rw-   0        0        0    46861 2024-05-12 11:40:47.000000 nicotool-1.4.8.5/nicotool/colors.py
--rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 nicotool-1.4.8.5/nicotool/data_manipulation.py
--rw-rw-rw-   0        0        0    38183 2024-04-17 13:12:42.000000 nicotool-1.4.8.5/nicotool/database.py
--rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 nicotool-1.4.8.5/nicotool/files.py
--rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 nicotool-1.4.8.5/nicotool/id.py
--rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 nicotool-1.4.8.5/nicotool/jsonify.py
--rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 nicotool-1.4.8.5/nicotool/keyboard.py
--rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 nicotool-1.4.8.5/nicotool/print_additions.py
--rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 nicotool-1.4.8.5/nicotool/profanities.py
--rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 nicotool-1.4.8.5/nicotool/youtube.py
-drwxrwxrwx   0        0        0        0 2024-05-13 11:40:10.659267 nicotool-1.4.8.5/nicotool.egg-info/
--rw-rw-rw-   0        0        0      307 2024-05-13 11:40:10.000000 nicotool-1.4.8.5/nicotool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-05-13 11:40:10.000000 nicotool-1.4.8.5/nicotool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 11:40:10.000000 nicotool-1.4.8.5/nicotool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-13 11:40:10.000000 nicotool-1.4.8.5/nicotool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-13 11:40:10.000000 nicotool-1.4.8.5/nicotool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 11:40:10.665330 nicotool-1.4.8.5/setup.cfg
--rw-rw-rw-   0        0        0      386 2024-05-13 11:39:53.000000 nicotool-1.4.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:36:43.815548 nicotool-1.4.8.6/
+-rw-rw-rw-   0        0        0      307 2024-05-14 12:36:43.815548 nicotool-1.4.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 nicotool-1.4.8.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 12:36:43.800205 nicotool-1.4.8.6/nicotool/
+-rw-rw-rw-   0        0        0     4003 2024-05-14 12:36:01.000000 nicotool-1.4.8.6/nicotool/__init__.py
+-rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 nicotool-1.4.8.6/nicotool/additional_functions.py
+-rw-rw-rw-   0        0        0      805 2024-05-14 12:35:38.000000 nicotool-1.4.8.6/nicotool/api_request.py
+-rw-rw-rw-   0        0        0    15433 2024-05-13 11:39:32.000000 nicotool-1.4.8.6/nicotool/ascii.py
+-rw-rw-rw-   0        0        0    46861 2024-05-12 11:40:47.000000 nicotool-1.4.8.6/nicotool/colors.py
+-rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 nicotool-1.4.8.6/nicotool/data_manipulation.py
+-rw-rw-rw-   0        0        0    38183 2024-04-17 13:12:42.000000 nicotool-1.4.8.6/nicotool/database.py
+-rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 nicotool-1.4.8.6/nicotool/files.py
+-rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 nicotool-1.4.8.6/nicotool/id.py
+-rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 nicotool-1.4.8.6/nicotool/jsonify.py
+-rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 nicotool-1.4.8.6/nicotool/keyboard.py
+-rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 nicotool-1.4.8.6/nicotool/print_additions.py
+-rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 nicotool-1.4.8.6/nicotool/profanities.py
+-rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 nicotool-1.4.8.6/nicotool/youtube.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:36:43.813552 nicotool-1.4.8.6/nicotool.egg-info/
+-rw-rw-rw-   0        0        0      307 2024-05-14 12:36:43.000000 nicotool-1.4.8.6/nicotool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2024-05-14 12:36:43.000000 nicotool-1.4.8.6/nicotool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 12:36:43.000000 nicotool-1.4.8.6/nicotool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-14 12:36:43.000000 nicotool-1.4.8.6/nicotool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-14 12:36:43.000000 nicotool-1.4.8.6/nicotool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 12:36:43.816547 nicotool-1.4.8.6/setup.cfg
+-rw-rw-rw-   0        0        0      386 2024-05-14 12:36:08.000000 nicotool-1.4.8.6/setup.py
```

### Comparing `nicotool-1.4.8.5/nicotool/__init__.py` & `nicotool-1.4.8.6/nicotool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 from .youtube import downloadYoutube
 
 from .database import(add_data_to_table,check_if_database_exists,check_if_key_exists,
 convert_to_db_format,create_sqlite_database,create_table,delete_database,unconvert,
 table_exists,edit_data_in_table,edit_table,get_primary_columns,load_all_data,load_data_from_key,
 purge_database,purge_table,remove_data_from_table,purge_database_data,remove_table,backup_database,check_if_table_exists)
 
+from .api_request import request_api
+
 from .colors import (get_all_colors,get_color_hex,verify_hex_color,hex_to_int)
 # if is_connected():
 #     def get_latest_version(package_name):
 #         """Get the latest version of a package from PyPI."""
 #         try:
 #             client = xmlrpc.client.ServerProxy('https://pypi.org/pypi')
 #             releases = client.package_releases(package_name)
```

### Comparing `nicotool-1.4.8.5/nicotool/additional_functions.py` & `nicotool-1.4.8.6/nicotool/additional_functions.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.5/nicotool/ascii.py` & `nicotool-1.4.8.6/nicotool/ascii.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.5/nicotool/colors.py` & `nicotool-1.4.8.6/nicotool/colors.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.5/nicotool/data_manipulation.py` & `nicotool-1.4.8.6/nicotool/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.5/nicotool/database.py` & `nicotool-1.4.8.6/nicotool/database.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.5/nicotool/files.py` & `nicotool-1.4.8.6/nicotool/files.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.5/nicotool/id.py` & `nicotool-1.4.8.6/nicotool/id.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.5/nicotool/jsonify.py` & `nicotool-1.4.8.6/nicotool/jsonify.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.5/nicotool/keyboard.py` & `nicotool-1.4.8.6/nicotool/keyboard.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.5/nicotool/print_additions.py` & `nicotool-1.4.8.6/nicotool/print_additions.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.5/nicotool/profanities.py` & `nicotool-1.4.8.6/nicotool/profanities.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.5/nicotool/youtube.py` & `nicotool-1.4.8.6/nicotool/youtube.py`

 * *Files identical despite different names*

