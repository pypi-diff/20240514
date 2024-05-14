# Comparing `tmp/kurumii-1.4.8.4.tar.gz` & `tmp/kurumii-1.4.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kurumii-1.4.8.4.tar", last modified: Sun May 12 11:41:21 2024, max compression
+gzip compressed data, was "kurumii-1.4.8.6.tar", last modified: Tue May 14 12:38:01 2024, max compression
```

## Comparing `kurumii-1.4.8.4.tar` & `kurumii-1.4.8.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 11:41:21.787351 kurumii-1.4.8.4/
--rw-rw-rw-   0        0        0      309 2024-05-12 11:41:21.786355 kurumii-1.4.8.4/PKG-INFO
--rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 kurumii-1.4.8.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 11:41:21.773390 kurumii-1.4.8.4/kurumii/
--rw-rw-rw-   0        0        0     3963 2024-05-12 11:41:14.000000 kurumii-1.4.8.4/kurumii/__init__.py
--rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 kurumii-1.4.8.4/kurumii/additional_functions.py
--rw-rw-rw-   0        0        0    15234 2024-04-23 14:40:29.000000 kurumii-1.4.8.4/kurumii/ascii.py
--rw-rw-rw-   0        0        0    46861 2024-05-12 11:40:47.000000 kurumii-1.4.8.4/kurumii/colors.py
--rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 kurumii-1.4.8.4/kurumii/data_manipulation.py
--rw-rw-rw-   0        0        0    38183 2024-04-17 13:12:42.000000 kurumii-1.4.8.4/kurumii/database.py
--rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 kurumii-1.4.8.4/kurumii/files.py
--rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 kurumii-1.4.8.4/kurumii/id.py
--rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 kurumii-1.4.8.4/kurumii/jsonify.py
--rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 kurumii-1.4.8.4/kurumii/keyboard.py
--rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 kurumii-1.4.8.4/kurumii/print_additions.py
--rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 kurumii-1.4.8.4/kurumii/profanities.py
--rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 kurumii-1.4.8.4/kurumii/youtube.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:41:21.784361 kurumii-1.4.8.4/kurumii.egg-info/
--rw-rw-rw-   0        0        0      309 2024-05-12 11:41:21.000000 kurumii-1.4.8.4/kurumii.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2024-05-12 11:41:21.000000 kurumii-1.4.8.4/kurumii.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 11:41:21.000000 kurumii-1.4.8.4/kurumii.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-12 11:41:21.000000 kurumii-1.4.8.4/kurumii.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-12 11:41:21.000000 kurumii-1.4.8.4/kurumii.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 11:41:21.788349 kurumii-1.4.8.4/setup.cfg
--rw-rw-rw-   0        0        0      388 2024-05-12 11:41:00.000000 kurumii-1.4.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:38:01.722028 kurumii-1.4.8.6/
+-rw-rw-rw-   0        0        0      309 2024-05-14 12:38:01.722028 kurumii-1.4.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 kurumii-1.4.8.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 12:38:01.707311 kurumii-1.4.8.6/kurumii/
+-rw-rw-rw-   0        0        0     4003 2024-05-14 12:36:01.000000 kurumii-1.4.8.6/kurumii/__init__.py
+-rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 kurumii-1.4.8.6/kurumii/additional_functions.py
+-rw-rw-rw-   0        0        0      805 2024-05-14 12:35:38.000000 kurumii-1.4.8.6/kurumii/api_request.py
+-rw-rw-rw-   0        0        0    15433 2024-05-13 11:39:32.000000 kurumii-1.4.8.6/kurumii/ascii.py
+-rw-rw-rw-   0        0        0    46861 2024-05-12 11:40:47.000000 kurumii-1.4.8.6/kurumii/colors.py
+-rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 kurumii-1.4.8.6/kurumii/data_manipulation.py
+-rw-rw-rw-   0        0        0    38183 2024-04-17 13:12:42.000000 kurumii-1.4.8.6/kurumii/database.py
+-rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 kurumii-1.4.8.6/kurumii/files.py
+-rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 kurumii-1.4.8.6/kurumii/id.py
+-rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 kurumii-1.4.8.6/kurumii/jsonify.py
+-rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 kurumii-1.4.8.6/kurumii/keyboard.py
+-rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 kurumii-1.4.8.6/kurumii/print_additions.py
+-rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 kurumii-1.4.8.6/kurumii/profanities.py
+-rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 kurumii-1.4.8.6/kurumii/youtube.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:38:01.719723 kurumii-1.4.8.6/kurumii.egg-info/
+-rw-rw-rw-   0        0        0      309 2024-05-14 12:38:01.000000 kurumii-1.4.8.6/kurumii.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-05-14 12:38:01.000000 kurumii-1.4.8.6/kurumii.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 12:38:01.000000 kurumii-1.4.8.6/kurumii.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-14 12:38:01.000000 kurumii-1.4.8.6/kurumii.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 12:38:01.000000 kurumii-1.4.8.6/kurumii.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 12:38:01.722028 kurumii-1.4.8.6/setup.cfg
+-rw-rw-rw-   0        0        0      388 2024-05-14 12:37:57.000000 kurumii-1.4.8.6/setup.py
```

### Comparing `kurumii-1.4.8.4/kurumii/__init__.py` & `kurumii-1.4.8.6/kurumii/__init__.py`

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

### Comparing `kurumii-1.4.8.4/kurumii/additional_functions.py` & `kurumii-1.4.8.6/kurumii/additional_functions.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.4/kurumii/ascii.py` & `kurumii-1.4.8.6/kurumii/ascii.py`

 * *Files 4% similar despite different names*

```diff
@@ -639,30 +639,47 @@
 "        ",
 "   _    ",
 " _| |_  ",
 "|_   _| ",
 "  |_|   ",
 "        ",
 "        "
-        
-        
-        
-
 ],
 "=":[
     
 "         ",   
 " ______  ",
 "|______| ",
 " ______  ",
 "|______| ",
 "         ",
 "         "
+],
+"_":[
+    
          
          
+"         ",        
+"         ",        
+"         ",        
+"         ",
+" ______  ",
+"|______| ",
+"         "
+],
+":":[
+    
+"    ",    
+" _  ",
+"(_) ",
+"    ",
+" _  ",
+"(_) ",
+"    "
+    
 
 ]
 
 }
 
 def print_ascii(text):
 
@@ -806,8 +823,9 @@
     for line_num in range(len(ascii_art_['A'])):
         for char in text:
             if char in ascii_art_:
                 combined_art += ascii_art_[char][line_num]  # Concatenate ASCII art for each character
             else:
                 return print(f' Unsuported character: {char}')
         combined_art += "\n"  # Add a newline after each line of characters
-    return(f"\033[38;2;{color}m{combined_art}\033[0m")
+    return(f"\033[38;2;{color}m{combined_art}\033[0m")
+
```

### Comparing `kurumii-1.4.8.4/kurumii/colors.py` & `kurumii-1.4.8.6/kurumii/colors.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.4/kurumii/data_manipulation.py` & `kurumii-1.4.8.6/kurumii/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.4/kurumii/database.py` & `kurumii-1.4.8.6/kurumii/database.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.4/kurumii/files.py` & `kurumii-1.4.8.6/kurumii/files.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.4/kurumii/id.py` & `kurumii-1.4.8.6/kurumii/id.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.4/kurumii/jsonify.py` & `kurumii-1.4.8.6/kurumii/jsonify.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.4/kurumii/keyboard.py` & `kurumii-1.4.8.6/kurumii/keyboard.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.4/kurumii/print_additions.py` & `kurumii-1.4.8.6/kurumii/print_additions.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.4/kurumii/profanities.py` & `kurumii-1.4.8.6/kurumii/profanities.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.4/kurumii/youtube.py` & `kurumii-1.4.8.6/kurumii/youtube.py`

 * *Files identical despite different names*

