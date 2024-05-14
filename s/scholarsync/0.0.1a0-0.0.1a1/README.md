# Comparing `tmp/scholarsync-0.0.1a0.tar.gz` & `tmp/scholarsync-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scholarsync-0.0.1a0.tar", last modified: Tue May 14 03:18:51 2024, max compression
+gzip compressed data, was "scholarsync-0.0.1a1.tar", last modified: Tue May 14 03:23:55 2024, max compression
```

## Comparing `scholarsync-0.0.1a0.tar` & `scholarsync-0.0.1a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 03:18:51.448999 scholarsync-0.0.1a0/
--rw-rw-rw-   0        0        0     6407 2024-05-07 15:48:34.000000 scholarsync-0.0.1a0/LICENSE
--rw-rw-rw-   0        0        0     2312 2024-05-14 03:18:51.448999 scholarsync-0.0.1a0/PKG-INFO
--rw-rw-rw-   0        0        0     1698 2024-05-07 15:21:11.000000 scholarsync-0.0.1a0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 03:18:51.402118 scholarsync-0.0.1a0/scholarsync/
--rw-rw-rw-   0        0        0        0 2024-05-04 11:09:37.000000 scholarsync-0.0.1a0/scholarsync/__init__.py
--rw-rw-rw-   0        0        0    80560 2024-05-14 03:04:35.000000 scholarsync-0.0.1a0/scholarsync/aio.py
-drwxrwxrwx   0        0        0        0 2024-05-14 03:18:51.448999 scholarsync-0.0.1a0/scholarsync/data/
--rw-rw-rw-   0        0        0     6407 2024-05-07 15:47:59.000000 scholarsync-0.0.1a0/scholarsync/data/LICENSE.txt
--rw-rw-rw-   0        0        0     1698 2024-05-07 15:21:11.000000 scholarsync-0.0.1a0/scholarsync/data/README.md
--rw-rw-rw-   0        0        0    17901 2024-05-07 15:17:14.000000 scholarsync-0.0.1a0/scholarsync/data/help.txt
--rw-rw-rw-   0        0        0       45 2024-05-05 06:30:21.000000 scholarsync-0.0.1a0/scholarsync/data/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 03:18:51.433376 scholarsync-0.0.1a0/scholarsync.egg-info/
--rw-rw-rw-   0        0        0     2312 2024-05-14 03:18:51.000000 scholarsync-0.0.1a0/scholarsync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2024-05-14 03:18:51.000000 scholarsync-0.0.1a0/scholarsync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 03:18:51.000000 scholarsync-0.0.1a0/scholarsync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-14 03:18:51.000000 scholarsync-0.0.1a0/scholarsync.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2024-05-14 03:18:51.000000 scholarsync-0.0.1a0/scholarsync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-14 03:18:51.000000 scholarsync-0.0.1a0/scholarsync.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 03:18:51.448999 scholarsync-0.0.1a0/setup.cfg
--rw-rw-rw-   0        0        0     1137 2024-05-14 03:16:32.000000 scholarsync-0.0.1a0/setup.py
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

### Comparing `scholarsync-0.0.1a0/LICENSE` & `scholarsync-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `scholarsync-0.0.1a0/PKG-INFO` & `scholarsync-0.0.1a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scholarsync
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: The Literature mining and processing utility
 Home-page: UNKNOWN
 Author: AA
 Author-email: idonthaveemail@mail.com
 License: UNKNOWN
 Description: # Combined Data Mining Utility
```

### Comparing `scholarsync-0.0.1a0/README.md` & `scholarsync-0.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `scholarsync-0.0.1a0/scholarsync/aio.py` & `scholarsync-0.0.1a1/scholarsync/aio.py`

 * *Files identical despite different names*

### Comparing `scholarsync-0.0.1a0/scholarsync/data/LICENSE.txt` & `scholarsync-0.0.1a1/scholarsync/data/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scholarsync-0.0.1a0/scholarsync/data/README.md` & `scholarsync-0.0.1a1/scholarsync/data/README.md`

 * *Files identical despite different names*

### Comparing `scholarsync-0.0.1a0/scholarsync/data/help.txt` & `scholarsync-0.0.1a1/scholarsync/data/help.txt`

 * *Files identical despite different names*

### Comparing `scholarsync-0.0.1a0/scholarsync.egg-info/PKG-INFO` & `scholarsync-0.0.1a1/scholarsync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scholarsync
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: The Literature mining and processing utility
 Home-page: UNKNOWN
 Author: AA
 Author-email: idonthaveemail@mail.com
 License: UNKNOWN
 Description: # Combined Data Mining Utility
```

### Comparing `scholarsync-0.0.1a0/setup.py` & `scholarsync-0.0.1a1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,43 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import os
 import site
+import sys
 
 class PostInstallCommand(install):
     """Post-installation for installation mode."""
     def run(self):
         install.run(self)
         # Add the installation directory to the PATH
-        user_base = site.USER_BASE
-        bin_dir = os.path.join(user_base, 'bin')
-        if bin_dir not in os.environ['PATH'].split(os.pathsep):
-            os.environ['PATH'] += os.pathsep + bin_dir
+        bin_dir = self.get_bin_directory()
+        self.create_executable_script(bin_dir)
+
+    def get_bin_directory(self):
+        # Determine the appropriate bin directory based on the operating system
+        if sys.platform.startswith('win'):
+            return os.path.join(site.USER_BASE, 'Scripts')
+        else:
+            return os.path.join(site.USER_BASE, 'bin')
+
+    def create_executable_script(self, bin_dir):
+        # Create a script file that adds the installation directory to PATH and calls scholarsync
+        script_content = f"""\
+@echo off
+setlocal enabledelayedexpansion
+set "PATH=%PATH%;{bin_dir}"
+python -m scholarsync
+"""
+        script_path = os.path.join(bin_dir, 'scholarsync')
+        with open(script_path, 'w') as script_file:
+            script_file.write(script_content)
 
 setup(
     name='scholarsync',
-    version='0.0.1.a',
+    version='0.0.1a1',
     packages=find_packages(),
     author='AA',
     author_email='idonthaveemail@mail.com',
     description='The Literature mining and processing utility',
     long_description=open('README.md').read(),
     package_data={'scholarsync': ['data/*']},
     install_requires=[
```

