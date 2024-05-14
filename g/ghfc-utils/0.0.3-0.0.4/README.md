# Comparing `tmp/ghfc_utils-0.0.3.tar.gz` & `tmp/ghfc_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghfc_utils-0.0.3.tar", last modified: Tue May 14 13:59:45 2024, max compression
+gzip compressed data, was "ghfc_utils-0.0.4.tar", last modified: Tue May 14 14:11:19 2024, max compression
```

## Comparing `ghfc_utils-0.0.3.tar` & `ghfc_utils-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:59:45.259286 ghfc_utils-0.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2024-05-14 13:59:33.000000 ghfc_utils-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3514 2024-05-14 13:59:45.259286 ghfc_utils-0.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2945 2024-05-14 13:59:33.000000 ghfc_utils-0.0.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)       94 2024-05-14 13:59:33.000000 ghfc_utils-0.0.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-14 13:59:45.259286 ghfc_utils-0.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:59:45.259286 ghfc_utils-0.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:59:45.259286 ghfc_utils-0.0.3/src/ghfc_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:59:33.000000 ghfc_utils-0.0.3/src/ghfc_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12125 2024-05-14 13:59:33.000000 ghfc_utils-0.0.3/src/ghfc_utils/slivar_reannotator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:59:45.259286 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3514 2024-05-14 13:59:45.000000 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      336 2024-05-14 13:59:45.000000 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:59:45.000000 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2024-05-14 13:59:45.000000 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-05-14 13:59:45.000000 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-14 13:59:45.000000 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:11:19.734779 ghfc_utils-0.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-05-14 14:11:06.000000 ghfc_utils-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3516 2024-05-14 14:11:19.734779 ghfc_utils-0.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2945 2024-05-14 14:11:06.000000 ghfc_utils-0.0.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       94 2024-05-14 14:11:06.000000 ghfc_utils-0.0.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      824 2024-05-14 14:11:19.738779 ghfc_utils-0.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:11:19.730779 ghfc_utils-0.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:11:19.734779 ghfc_utils-0.0.4/src/ghfc_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 14:11:06.000000 ghfc_utils-0.0.4/src/ghfc_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12125 2024-05-14 14:11:06.000000 ghfc_utils-0.0.4/src/ghfc_utils/slivar_reannotator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:11:19.734779 ghfc_utils-0.0.4/src/ghfc_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3516 2024-05-14 14:11:19.000000 ghfc_utils-0.0.4/src/ghfc_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      336 2024-05-14 14:11:19.000000 ghfc_utils-0.0.4/src/ghfc_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 14:11:19.000000 ghfc_utils-0.0.4/src/ghfc_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-14 14:11:19.000000 ghfc_utils-0.0.4/src/ghfc_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 14:11:19.000000 ghfc_utils-0.0.4/src/ghfc_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-14 14:11:19.000000 ghfc_utils-0.0.4/src/ghfc_utils.egg-info/top_level.txt
```

### Comparing `ghfc_utils-0.0.3/LICENSE` & `ghfc_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ghfc_utils-0.0.3/PKG-INFO` & `ghfc_utils-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ghfc_utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Various tools and scripts used in the GHFC lab
 Home-page: https://gitlab.pasteur.fr/ghfc/ghfc-utils
 Author: Freddy Cliquet
 Author-email: freddy.cliquet@pasteur.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: argparse
 Requires-Dist: pyranges
-Requires-Dist: yaml
+Requires-Dist: PyYAML
 
 # ghfc-utils
 
 set of small tools designed to help automatize simple task locally or on Pasteur's cluster.
 
 - **ghfc-reannotate** for the postprocessing of slivar files including filtering and geneset reannotation.
```

### Comparing `ghfc_utils-0.0.3/README.md` & `ghfc_utils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ghfc_utils-0.0.3/setup.cfg` & `ghfc_utils-0.0.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ghfc_utils
-version = v0.0.3
+version = v0.0.4
 author = Freddy Cliquet
 author_email = freddy.cliquet@pasteur.fr
 description = Various tools and scripts used in the GHFC lab
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.pasteur.fr/ghfc/ghfc-utils
 licence = MIT License
@@ -20,15 +20,15 @@
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	numpy
 	pandas
 	argparse
 	pyranges
-	yaml
+	PyYAML
 
 [options.package_data]
 * = *.yaml
 
 [options.entry_points]
 console_scripts = 
 	ghfc-reannotate = ghfc_utils:slivar_reannotator.main
```

### Comparing `ghfc_utils-0.0.3/src/ghfc_utils/slivar_reannotator.py` & `ghfc_utils-0.0.4/src/ghfc_utils/slivar_reannotator.py`

 * *Files identical despite different names*

### Comparing `ghfc_utils-0.0.3/src/ghfc_utils.egg-info/PKG-INFO` & `ghfc_utils-0.0.4/src/ghfc_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ghfc_utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Various tools and scripts used in the GHFC lab
 Home-page: https://gitlab.pasteur.fr/ghfc/ghfc-utils
 Author: Freddy Cliquet
 Author-email: freddy.cliquet@pasteur.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: argparse
 Requires-Dist: pyranges
-Requires-Dist: yaml
+Requires-Dist: PyYAML
 
 # ghfc-utils
 
 set of small tools designed to help automatize simple task locally or on Pasteur's cluster.
 
 - **ghfc-reannotate** for the postprocessing of slivar files including filtering and geneset reannotation.
```

