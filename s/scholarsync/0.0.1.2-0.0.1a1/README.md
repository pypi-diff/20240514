# Comparing `tmp/scholarsync-0.0.1.2.tar.gz` & `tmp/scholarsync-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scholarsync-0.0.1.2.tar", last modified: Tue May 14 04:16:25 2024, max compression
+gzip compressed data, was "scholarsync-0.0.1a1.tar", last modified: Tue May 14 03:23:55 2024, max compression
```

## Comparing `scholarsync-0.0.1.2.tar` & `scholarsync-0.0.1a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 04:16:25.531877 scholarsync-0.0.1.2/
--rw-rw-rw-   0        0        0     6407 2024-05-07 15:48:34.000000 scholarsync-0.0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2642 2024-05-14 04:16:25.531877 scholarsync-0.0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1956 2024-05-14 04:16:02.000000 scholarsync-0.0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 04:16:25.469377 scholarsync-0.0.1.2/scholarsync/
--rw-rw-rw-   0        0        0        0 2024-05-04 11:09:37.000000 scholarsync-0.0.1.2/scholarsync/__init__.py
--rw-rw-rw-   0        0        0    80560 2024-05-14 03:04:35.000000 scholarsync-0.0.1.2/scholarsync/aio.py
-drwxrwxrwx   0        0        0        0 2024-05-14 04:16:25.516252 scholarsync-0.0.1.2/scholarsync/data/
--rw-rw-rw-   0        0        0     6407 2024-05-07 15:47:59.000000 scholarsync-0.0.1.2/scholarsync/data/LICENSE.txt
--rw-rw-rw-   0        0        0     1698 2024-05-07 15:21:11.000000 scholarsync-0.0.1.2/scholarsync/data/README.md
--rw-rw-rw-   0        0        0    17901 2024-05-07 15:17:14.000000 scholarsync-0.0.1.2/scholarsync/data/help.txt
--rw-rw-rw-   0        0        0       45 2024-05-05 06:30:21.000000 scholarsync-0.0.1.2/scholarsync/data/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 04:16:25.516252 scholarsync-0.0.1.2/scholarsync.egg-info/
--rw-rw-rw-   0        0        0     2642 2024-05-14 04:16:25.000000 scholarsync-0.0.1.2/scholarsync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2024-05-14 04:16:25.000000 scholarsync-0.0.1.2/scholarsync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 04:16:25.000000 scholarsync-0.0.1.2/scholarsync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-14 04:16:25.000000 scholarsync-0.0.1.2/scholarsync.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2024-05-14 04:16:25.000000 scholarsync-0.0.1.2/scholarsync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-14 04:16:25.000000 scholarsync-0.0.1.2/scholarsync.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 04:16:25.531877 scholarsync-0.0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      663 2024-05-14 04:00:10.000000 scholarsync-0.0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:23:55.344557 scholarsync-0.0.1a1/
+-rw-rw-rw-   0        0        0     6407 2024-05-07 15:48:34.000000 scholarsync-0.0.1a1/LICENSE
+-rw-rw-rw-   0        0        0     2312 2024-05-14 03:23:55.344557 scholarsync-0.0.1a1/PKG-INFO
+-rw-rw-rw-   0        0        0     1698 2024-05-07 15:21:11.000000 scholarsync-0.0.1a1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 03:23:55.250806 scholarsync-0.0.1a1/scholarsync/
+-rw-rw-rw-   0        0        0        0 2024-05-04 11:09:37.000000 scholarsync-0.0.1a1/scholarsync/__init__.py
+-rw-rw-rw-   0        0        0    80560 2024-05-14 03:04:35.000000 scholarsync-0.0.1a1/scholarsync/aio.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:23:55.328932 scholarsync-0.0.1a1/scholarsync/data/
+-rw-rw-rw-   0        0        0     6407 2024-05-07 15:47:59.000000 scholarsync-0.0.1a1/scholarsync/data/LICENSE.txt
+-rw-rw-rw-   0        0        0     1698 2024-05-07 15:21:11.000000 scholarsync-0.0.1a1/scholarsync/data/README.md
+-rw-rw-rw-   0        0        0    17901 2024-05-07 15:17:14.000000 scholarsync-0.0.1a1/scholarsync/data/help.txt
+-rw-rw-rw-   0        0        0       45 2024-05-05 06:30:21.000000 scholarsync-0.0.1a1/scholarsync/data/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 03:23:55.328932 scholarsync-0.0.1a1/scholarsync.egg-info/
+-rw-rw-rw-   0        0        0     2312 2024-05-14 03:23:55.000000 scholarsync-0.0.1a1/scholarsync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2024-05-14 03:23:55.000000 scholarsync-0.0.1a1/scholarsync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 03:23:55.000000 scholarsync-0.0.1a1/scholarsync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-14 03:23:55.000000 scholarsync-0.0.1a1/scholarsync.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2024-05-14 03:23:55.000000 scholarsync-0.0.1a1/scholarsync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-14 03:23:55.000000 scholarsync-0.0.1a1/scholarsync.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 03:23:55.344557 scholarsync-0.0.1a1/setup.cfg
+-rw-rw-rw-   0        0        0     1770 2024-05-14 03:23:48.000000 scholarsync-0.0.1a1/setup.py
```

### Comparing `scholarsync-0.0.1.2/LICENSE` & `scholarsync-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `scholarsync-0.0.1.2/PKG-INFO` & `scholarsync-0.0.1a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scholarsync
-Version: 0.0.1.2
+Version: 0.0.1a1
 Summary: The Literature mining and processing utility
 Home-page: UNKNOWN
 Author: AA
 Author-email: idonthaveemail@mail.com
 License: UNKNOWN
 Description: # Combined Data Mining Utility
         
@@ -14,28 +14,19 @@
         
         ### Prerequisites
         
         Ensure you have Python installed on your system. The script is compatible with both Python 2 and 3.
         
         ### Installation
         
-        1. pip install scholarsync
-        	
-        
-        To address the error message,
-        	WARNING: The script scholarsync is installed in '/home/username/.local/bin' which is not on PATH.
-        	 open a terminal and type the following command, then press Enter:
-        
-        .. code-block:: bash
-        
-           echo 'export PATH="$PATH:/home/username/.local/bin"' >> ~/.bashrc && source ~/.bashrc
-        
-        Replace ``username`` with your actual username.
+        1. Clone or download the script to your local machine.
         
+        2. Navigate to the directory containing the script.
         
+        3. Run the script using Python.
         
         
         ## Usage
         
         Upon running the script, you will be prompted with a menu to select the desired functionality. The available options include:
         
         - PubMed search/query
```

### Comparing `scholarsync-0.0.1.2/README.md` & `scholarsync-0.0.1a1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,28 +6,19 @@
 
 ### Prerequisites
 
 Ensure you have Python installed on your system. The script is compatible with both Python 2 and 3.
 
 ### Installation
 
-1. pip install scholarsync
-	
-
-To address the error message,
-	WARNING: The script scholarsync is installed in '/home/username/.local/bin' which is not on PATH.
-	 open a terminal and type the following command, then press Enter:
-
-.. code-block:: bash
-
-   echo 'export PATH="$PATH:/home/username/.local/bin"' >> ~/.bashrc && source ~/.bashrc
-
-Replace ``username`` with your actual username.
+1. Clone or download the script to your local machine.
 
+2. Navigate to the directory containing the script.
 
+3. Run the script using Python.
 
 
 ## Usage
 
 Upon running the script, you will be prompted with a menu to select the desired functionality. The available options include:
 
 - PubMed search/query
```

### Comparing `scholarsync-0.0.1.2/scholarsync/aio.py` & `scholarsync-0.0.1a1/scholarsync/aio.py`

 * *Files identical despite different names*

### Comparing `scholarsync-0.0.1.2/scholarsync/data/LICENSE.txt` & `scholarsync-0.0.1a1/scholarsync/data/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scholarsync-0.0.1.2/scholarsync/data/README.md` & `scholarsync-0.0.1a1/scholarsync/data/README.md`

 * *Files identical despite different names*

### Comparing `scholarsync-0.0.1.2/scholarsync/data/help.txt` & `scholarsync-0.0.1a1/scholarsync/data/help.txt`

 * *Files identical despite different names*

### Comparing `scholarsync-0.0.1.2/scholarsync.egg-info/PKG-INFO` & `scholarsync-0.0.1a1/scholarsync.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scholarsync
-Version: 0.0.1.2
+Version: 0.0.1a1
 Summary: The Literature mining and processing utility
 Home-page: UNKNOWN
 Author: AA
 Author-email: idonthaveemail@mail.com
 License: UNKNOWN
 Description: # Combined Data Mining Utility
         
@@ -14,28 +14,19 @@
         
         ### Prerequisites
         
         Ensure you have Python installed on your system. The script is compatible with both Python 2 and 3.
         
         ### Installation
         
-        1. pip install scholarsync
-        	
-        
-        To address the error message,
-        	WARNING: The script scholarsync is installed in '/home/username/.local/bin' which is not on PATH.
-        	 open a terminal and type the following command, then press Enter:
-        
-        .. code-block:: bash
-        
-           echo 'export PATH="$PATH:/home/username/.local/bin"' >> ~/.bashrc && source ~/.bashrc
-        
-        Replace ``username`` with your actual username.
+        1. Clone or download the script to your local machine.
         
+        2. Navigate to the directory containing the script.
         
+        3. Run the script using Python.
         
         
         ## Usage
         
         Upon running the script, you will be prompted with a menu to select the desired functionality. The available options include:
         
         - PubMed search/query
```

