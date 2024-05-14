# Comparing `tmp/ibott-files-1.0.6.tar.gz` & `tmp/ibott-files-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibott-files-1.0.6.tar", last modified: Sat Mar  2 09:41:57 2024, max compression
+gzip compressed data, was "ibott-files-1.0.7.tar", last modified: Tue May 14 09:24:09 2024, max compression
```

## Comparing `ibott-files-1.0.6.tar` & `ibott-files-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-03-02 09:41:57.452626 ibott-files-1.0.6/
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    11355 2023-10-14 17:23:38.000000 ibott-files-1.0.6/LICENSE
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    16227 2024-03-02 09:41:57.452238 ibott-files-1.0.6/PKG-INFO
-drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-03-02 09:41:57.449808 ibott-files-1.0.6/files_and_folders/
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)        0 2023-10-14 17:23:38.000000 ibott-files-1.0.6/files_and_folders/__init__.py
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)     4843 2023-10-17 17:47:53.000000 ibott-files-1.0.6/files_and_folders/files.py
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)     5002 2024-03-02 09:17:37.000000 ibott-files-1.0.6/files_and_folders/folders.py
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)     1757 2023-10-14 17:25:20.000000 ibott-files-1.0.6/files_and_folders/images.py
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)     3103 2024-03-02 09:13:34.000000 ibott-files-1.0.6/files_and_folders/pdfs.py
-drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-03-02 09:41:57.451631 ibott-files-1.0.6/ibott_files.egg-info/
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    16227 2024-03-02 09:41:57.000000 ibott-files-1.0.6/ibott_files.egg-info/PKG-INFO
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      345 2024-03-02 09:41:57.000000 ibott-files-1.0.6/ibott_files.egg-info/SOURCES.txt
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)        1 2024-03-02 09:41:57.000000 ibott-files-1.0.6/ibott_files.egg-info/dependency_links.txt
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       41 2024-03-02 09:41:57.000000 ibott-files-1.0.6/ibott_files.egg-info/requires.txt
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       18 2024-03-02 09:41:57.000000 ibott-files-1.0.6/ibott_files.egg-info/top_level.txt
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      719 2024-03-02 09:39:04.000000 ibott-files-1.0.6/pyproject.toml
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       38 2024-03-02 09:41:57.452753 ibott-files-1.0.6/setup.cfg
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      710 2024-03-02 09:39:21.000000 ibott-files-1.0.6/setup.py
+drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-05-14 09:24:09.379750 ibott-files-1.0.7/
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    11355 2023-10-14 17:23:38.000000 ibott-files-1.0.7/LICENSE
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    16227 2024-05-14 09:24:09.379471 ibott-files-1.0.7/PKG-INFO
+drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-05-14 09:24:09.374677 ibott-files-1.0.7/files_and_folders/
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)        0 2023-10-14 17:23:38.000000 ibott-files-1.0.7/files_and_folders/__init__.py
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)     4843 2023-10-17 17:47:53.000000 ibott-files-1.0.7/files_and_folders/files.py
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)     5018 2024-05-14 09:20:50.000000 ibott-files-1.0.7/files_and_folders/folders.py
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)     1757 2023-10-14 17:25:20.000000 ibott-files-1.0.7/files_and_folders/images.py
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)     3103 2024-03-02 09:13:34.000000 ibott-files-1.0.7/files_and_folders/pdfs.py
+drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-05-14 09:24:09.378397 ibott-files-1.0.7/ibott_files.egg-info/
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    16227 2024-05-14 09:24:09.000000 ibott-files-1.0.7/ibott_files.egg-info/PKG-INFO
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      345 2024-05-14 09:24:09.000000 ibott-files-1.0.7/ibott_files.egg-info/SOURCES.txt
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)        1 2024-05-14 09:24:09.000000 ibott-files-1.0.7/ibott_files.egg-info/dependency_links.txt
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       41 2024-05-14 09:24:09.000000 ibott-files-1.0.7/ibott_files.egg-info/requires.txt
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       18 2024-05-14 09:24:09.000000 ibott-files-1.0.7/ibott_files.egg-info/top_level.txt
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      719 2024-05-14 09:24:08.000000 ibott-files-1.0.7/pyproject.toml
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       38 2024-05-14 09:24:09.379825 ibott-files-1.0.7/setup.cfg
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      710 2024-03-02 09:39:21.000000 ibott-files-1.0.7/setup.py
```

### Comparing `ibott-files-1.0.6/LICENSE` & `ibott-files-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ibott-files-1.0.6/PKG-INFO` & `ibott-files-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibott-files
-Version: 1.0.6
+Version: 1.0.7
 Summary: This packages crates a simple way to work with, files, folders, images and pdfs.
 Home-page: https://github.com/ecrespo66/files_and_folders
 Author: OnameDohe
 Author-email: OnameDohe <enrique.crespo.debenito@gmail.com>
 License:                                Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ibott-files-1.0.6/files_and_folders/files.py` & `ibott-files-1.0.7/files_and_folders/files.py`

 * *Files identical despite different names*

### Comparing `ibott-files-1.0.6/files_and_folders/folders.py` & `ibott-files-1.0.7/files_and_folders/folders.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         """
         Get List of files, in folder
         Returns:
         list -- list of files
         """
         file_list = []
         for file in os.listdir(self.path):
-            if extension in file:
+            if extension.upper() in file.upper():
                 file_list.append(File(self.path + "\\" + file))
         return file_list
 
     def download_file(self, url, name=None):
         """
         Download file from url
         Arguments:
```

### Comparing `ibott-files-1.0.6/files_and_folders/images.py` & `ibott-files-1.0.7/files_and_folders/images.py`

 * *Files identical despite different names*

### Comparing `ibott-files-1.0.6/files_and_folders/pdfs.py` & `ibott-files-1.0.7/files_and_folders/pdfs.py`

 * *Files identical despite different names*

### Comparing `ibott-files-1.0.6/ibott_files.egg-info/PKG-INFO` & `ibott-files-1.0.7/ibott_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibott-files
-Version: 1.0.6
+Version: 1.0.7
 Summary: This packages crates a simple way to work with, files, folders, images and pdfs.
 Home-page: https://github.com/ecrespo66/files_and_folders
 Author: OnameDohe
 Author-email: OnameDohe <enrique.crespo.debenito@gmail.com>
 License:                                Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ibott-files-1.0.6/pyproject.toml` & `ibott-files-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "Pillow","PyPDF2", "requests","PyMuPDF"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ibott-files"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
     { name="OnameDohe", email="enrique.crespo.debenito@gmail.com" },
 ]
 description = "This packages crates a simple way to work with, files, folders, images and pdfs."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `ibott-files-1.0.6/setup.py` & `ibott-files-1.0.7/setup.py`

 * *Files identical despite different names*

