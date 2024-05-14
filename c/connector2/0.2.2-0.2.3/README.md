# Comparing `tmp/connector2-0.2.2.tar.gz` & `tmp/connector2-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connector2-0.2.2.tar", last modified: Thu May  9 17:44:39 2024, max compression
+gzip compressed data, was "connector2-0.2.3.tar", last modified: Tue May 14 19:49:53 2024, max compression
```

## Comparing `connector2-0.2.2.tar` & `connector2-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 tsingh     (501) staff       (20)        0 2024-05-09 17:44:39.612603 connector2-0.2.2/
--rw-r--r--   0 tsingh     (501) staff       (20)     1074 2023-07-21 17:38:20.000000 connector2-0.2.2/LICENSE.md
--rw-r--r--   0 tsingh     (501) staff       (20)     7877 2024-05-09 17:44:39.612534 connector2-0.2.2/PKG-INFO
--rw-r--r--   0 tsingh     (501) staff       (20)     7448 2024-05-09 17:44:17.000000 connector2-0.2.2/README.md
-drwxr-xr-x   0 tsingh     (501) staff       (20)        0 2024-05-09 17:44:39.611351 connector2-0.2.2/connector/
--rw-r--r--   0 tsingh     (501) staff       (20)      981 2023-08-18 18:00:00.000000 connector2-0.2.2/connector/__init__.py
--rw-r--r--   0 tsingh     (501) staff       (20)      497 2024-05-09 17:44:39.612899 connector2-0.2.2/connector/_version.py
--rw-r--r--   0 tsingh     (501) staff       (20)    10689 2024-05-09 17:44:17.000000 connector2-0.2.2/connector/cli.py
--rw-r--r--   0 tsingh     (501) staff       (20)     1277 2024-05-08 18:36:41.000000 connector2-0.2.2/connector/googlecloud.py
--rw-r--r--   0 tsingh     (501) staff       (20)     2086 2024-05-08 18:36:41.000000 connector2-0.2.2/connector/googledrive.py
--rw-r--r--   0 tsingh     (501) staff       (20)     5371 2024-05-08 15:27:29.000000 connector2-0.2.2/connector/init_conda_env.py
--rw-r--r--   0 tsingh     (501) staff       (20)     1645 2024-05-08 18:36:41.000000 connector2-0.2.2/connector/remote.py
--rw-r--r--   0 tsingh     (501) staff       (20)     1896 2023-08-25 17:59:10.000000 connector2-0.2.2/connector/restricted.py
--rw-r--r--   0 tsingh     (501) staff       (20)     1993 2024-05-08 18:36:41.000000 connector2-0.2.2/connector/utils.py
-drwxr-xr-x   0 tsingh     (501) staff       (20)        0 2024-05-09 17:44:39.612285 connector2-0.2.2/connector2.egg-info/
--rw-r--r--   0 tsingh     (501) staff       (20)     7877 2024-05-09 17:44:39.000000 connector2-0.2.2/connector2.egg-info/PKG-INFO
--rw-r--r--   0 tsingh     (501) staff       (20)      461 2024-05-09 17:44:39.000000 connector2-0.2.2/connector2.egg-info/SOURCES.txt
--rw-r--r--   0 tsingh     (501) staff       (20)        1 2024-05-09 17:44:39.000000 connector2-0.2.2/connector2.egg-info/dependency_links.txt
--rw-r--r--   0 tsingh     (501) staff       (20)       81 2024-05-09 17:44:39.000000 connector2-0.2.2/connector2.egg-info/entry_points.txt
--rw-r--r--   0 tsingh     (501) staff       (20)       47 2024-05-09 17:44:39.000000 connector2-0.2.2/connector2.egg-info/requires.txt
--rw-r--r--   0 tsingh     (501) staff       (20)       10 2024-05-09 17:44:39.000000 connector2-0.2.2/connector2.egg-info/top_level.txt
--rw-r--r--   0 tsingh     (501) staff       (20)      208 2024-05-09 17:44:39.612809 connector2-0.2.2/setup.cfg
--rw-r--r--   0 tsingh     (501) staff       (20)      984 2024-05-07 20:51:21.000000 connector2-0.2.2/setup.py
--rw-r--r--   0 tsingh     (501) staff       (20)    86677 2023-08-18 18:00:00.000000 connector2-0.2.2/versioneer.py
+drwxr-xr-x   0 tsingh     (501) staff       (20)        0 2024-05-14 19:49:53.593524 connector2-0.2.3/
+-rw-r--r--   0 tsingh     (501) staff       (20)     1074 2023-07-21 17:38:20.000000 connector2-0.2.3/LICENSE.md
+-rw-r--r--   0 tsingh     (501) staff       (20)     7877 2024-05-14 19:49:53.593451 connector2-0.2.3/PKG-INFO
+-rw-r--r--   0 tsingh     (501) staff       (20)     7448 2024-05-09 17:44:17.000000 connector2-0.2.3/README.md
+drwxr-xr-x   0 tsingh     (501) staff       (20)        0 2024-05-14 19:49:53.591567 connector2-0.2.3/connector/
+-rw-r--r--   0 tsingh     (501) staff       (20)      981 2023-08-18 18:00:00.000000 connector2-0.2.3/connector/__init__.py
+-rw-r--r--   0 tsingh     (501) staff       (20)      497 2024-05-14 19:49:53.593925 connector2-0.2.3/connector/_version.py
+-rw-r--r--   0 tsingh     (501) staff       (20)    10734 2024-05-14 19:49:18.000000 connector2-0.2.3/connector/cli.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     1277 2024-05-08 18:36:41.000000 connector2-0.2.3/connector/googlecloud.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     2086 2024-05-08 18:36:41.000000 connector2-0.2.3/connector/googledrive.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     5371 2024-05-08 15:27:29.000000 connector2-0.2.3/connector/init_conda_env.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     1645 2024-05-08 18:36:41.000000 connector2-0.2.3/connector/remote.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     1896 2023-08-25 17:59:10.000000 connector2-0.2.3/connector/restricted.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     1993 2024-05-08 18:36:41.000000 connector2-0.2.3/connector/utils.py
+drwxr-xr-x   0 tsingh     (501) staff       (20)        0 2024-05-14 19:49:53.593157 connector2-0.2.3/connector2.egg-info/
+-rw-r--r--   0 tsingh     (501) staff       (20)     7877 2024-05-14 19:49:53.000000 connector2-0.2.3/connector2.egg-info/PKG-INFO
+-rw-r--r--   0 tsingh     (501) staff       (20)      461 2024-05-14 19:49:53.000000 connector2-0.2.3/connector2.egg-info/SOURCES.txt
+-rw-r--r--   0 tsingh     (501) staff       (20)        1 2024-05-14 19:49:53.000000 connector2-0.2.3/connector2.egg-info/dependency_links.txt
+-rw-r--r--   0 tsingh     (501) staff       (20)       81 2024-05-14 19:49:53.000000 connector2-0.2.3/connector2.egg-info/entry_points.txt
+-rw-r--r--   0 tsingh     (501) staff       (20)       47 2024-05-14 19:49:53.000000 connector2-0.2.3/connector2.egg-info/requires.txt
+-rw-r--r--   0 tsingh     (501) staff       (20)       10 2024-05-14 19:49:53.000000 connector2-0.2.3/connector2.egg-info/top_level.txt
+-rw-r--r--   0 tsingh     (501) staff       (20)      208 2024-05-14 19:49:53.593821 connector2-0.2.3/setup.cfg
+-rw-r--r--   0 tsingh     (501) staff       (20)      984 2024-05-07 20:51:21.000000 connector2-0.2.3/setup.py
+-rw-r--r--   0 tsingh     (501) staff       (20)    86677 2023-08-18 18:00:00.000000 connector2-0.2.3/versioneer.py
```

### Comparing `connector2-0.2.2/LICENSE.md` & `connector2-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `connector2-0.2.2/PKG-INFO` & `connector2-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connector2
-Version: 0.2.2
+Version: 0.2.3
 Summary: Provides the default template for creating Python Package.
 Home-page: https://github.com/tjsinghlab/connector
 Author: Singh Lab
 Author-email: singhlab@nygenome.org
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `connector2-0.2.2/README.md` & `connector2-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `connector2-0.2.2/connector/__init__.py` & `connector2-0.2.3/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `connector2-0.2.2/connector/cli.py` & `connector2-0.2.3/connector/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     sync_drive_parser = subparsers.add_parser(
         'drive', help='Connect local directory to a Google Drive directory.')
     sync_drive_parser.add_argument(
         '-d', '--dir', choices=['up', 'down'], help='Choose direction to sync files, with up being local to remote (default: up)', default='up')
     sync_drive_parser.add_argument(
         '-p', '--project-name', type=str, help='The basename of the Google Drive project directory to sync to. Defaults to CLOUD_ROOT, then to the name of the current working directory.')
     sync_drive_parser.add_argument(
-        '-f', '--folder', choices=['src', 'data','figures'], help='Choose folder to sync (default: data)', default='data')
+        '-f', '--folder', choices=['src', 'data', 'figures', 'results'], help='Choose folder to sync (default: data)', default='data')
     sync_drive_parser.add_argument(
         '-s', '--subdir', type=str, help='The subdirectory within the local src/ or data/ directory to sync.', default='')
     sync_drive_parser.add_argument(
         '-t', '--target', choices=['personal', 'shared'], help='Choose which folder to share (default: shared)', default='shared')
     sync_drive_parser.add_argument('--max-size-mb', type=int, default=10,
                                    help='The maximum size of files to sync, in megabytes. Defaults to 10.')
     sync_drive_parser.add_argument('-o', '--open', action='store_true', help='Open remote drive.')
@@ -181,15 +181,15 @@
     #----
     # Subparser for the sync_bucket command to connect to Google Cloud Storage
     sync_drive_parser = subparsers.add_parser(
         'gcp', help='Connect local directory to a Google Cloud Storage bucket.')
     sync_drive_parser.add_argument(
         '-d', '--dir', choices=['up', 'down'], help='Choose direction to sync files, with up being local to remote (default: down)', default='down')
     sync_drive_parser.add_argument(
-        '-f', '--folder', choices=['src', 'data'], help='Choose folder to sync (default: data)', default='data')
+        '-f', '--folder', choices=['src', 'data', 'figures', 'results'], help='Choose folder to sync (default: data)', default='data')
     sync_drive_parser.add_argument(
         '-s', '--subdir', type=str, help='The subdirectory within the local src/ or data/ directory to sync.', default='')
     sync_drive_parser.add_argument('--max-size-mb', type=int, default=10,
                                 help='The maximum size of files to sync, in megabytes. Defaults to 10.')
     sync_drive_parser.add_argument('-o', '--open', action='store_true', help='Open remote bucket.')
     sync_drive_parser.add_argument('-ls', '--list', action='store_true', help='List bucket files.')
 
@@ -204,15 +204,15 @@
     sync_remote_parser.add_argument(
         '-r', '--remote-dir', type=str, help='The remote directory to sync to.')
     sync_remote_parser.add_argument(
         '-d', '--dir', choices=['up', 'down'], help='Choose direction to sync files, with up being local to remote (default: up)', default='up')
     sync_remote_parser.add_argument(
         '-s', '--subdir', type=str, help='The subdirectory within the local src/ or data/ directory to sync.', default='')
     sync_remote_parser.add_argument(
-        '-f', '--folder', choices=['src', 'data', 'figures'], help='Choose folder to sync (default: data)', default='data')
+        '-f', '--folder', choices=['src', 'data', 'figures', 'results'], help='Choose folder to sync (default: data)', default='data')
     sync_remote_parser.add_argument('--max-size-mb', type=int, default=10,
                                 help='The maximum size of files to sync, in megabytes. Defaults to 10.')
     sync_remote_parser.add_argument('-ls', '--list', action='store_true', help='List remote cluster files.')
 
     args = parser.parse_args()
     
     if args.command == 'config':
```

### Comparing `connector2-0.2.2/connector/googlecloud.py` & `connector2-0.2.3/connector/googlecloud.py`

 * *Files identical despite different names*

### Comparing `connector2-0.2.2/connector/googledrive.py` & `connector2-0.2.3/connector/googledrive.py`

 * *Files identical despite different names*

### Comparing `connector2-0.2.2/connector/init_conda_env.py` & `connector2-0.2.3/connector/init_conda_env.py`

 * *Files identical despite different names*

### Comparing `connector2-0.2.2/connector/remote.py` & `connector2-0.2.3/connector/remote.py`

 * *Files identical despite different names*

### Comparing `connector2-0.2.2/connector/restricted.py` & `connector2-0.2.3/connector/restricted.py`

 * *Files identical despite different names*

### Comparing `connector2-0.2.2/connector/utils.py` & `connector2-0.2.3/connector/utils.py`

 * *Files identical despite different names*

### Comparing `connector2-0.2.2/connector2.egg-info/PKG-INFO` & `connector2-0.2.3/connector2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connector2
-Version: 0.2.2
+Version: 0.2.3
 Summary: Provides the default template for creating Python Package.
 Home-page: https://github.com/tjsinghlab/connector
 Author: Singh Lab
 Author-email: singhlab@nygenome.org
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `connector2-0.2.2/setup.py` & `connector2-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `connector2-0.2.2/versioneer.py` & `connector2-0.2.3/versioneer.py`

 * *Files identical despite different names*

