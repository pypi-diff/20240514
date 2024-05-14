# Comparing `tmp/ghfc_utils-0.0.2.tar.gz` & `tmp/ghfc_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghfc_utils-0.0.2.tar", last modified: Tue May 14 11:35:48 2024, max compression
+gzip compressed data, was "ghfc_utils-0.0.3.tar", last modified: Tue May 14 13:59:45 2024, max compression
```

## Comparing `ghfc_utils-0.0.2.tar` & `ghfc_utils-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:35:48.178895 ghfc_utils-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2024-05-14 11:35:35.000000 ghfc_utils-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5285 2024-05-14 11:35:48.178895 ghfc_utils-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4736 2024-05-14 11:35:35.000000 ghfc_utils-0.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       94 2024-05-14 11:35:35.000000 ghfc_utils-0.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      816 2024-05-14 11:35:48.178895 ghfc_utils-0.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:35:48.174895 ghfc_utils-0.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:35:48.178895 ghfc_utils-0.0.2/src/ghfc_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 11:35:35.000000 ghfc_utils-0.0.2/src/ghfc_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12125 2024-05-14 11:35:35.000000 ghfc_utils-0.0.2/src/ghfc_utils/slivar_reannotator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:35:48.178895 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5285 2024-05-14 11:35:48.000000 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      336 2024-05-14 11:35:48.000000 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 11:35:48.000000 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2024-05-14 11:35:48.000000 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-14 11:35:48.000000 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-14 11:35:48.000000 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:59:45.259286 ghfc_utils-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-05-14 13:59:33.000000 ghfc_utils-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3514 2024-05-14 13:59:45.259286 ghfc_utils-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2945 2024-05-14 13:59:33.000000 ghfc_utils-0.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       94 2024-05-14 13:59:33.000000 ghfc_utils-0.0.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-14 13:59:45.259286 ghfc_utils-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:59:45.259286 ghfc_utils-0.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:59:45.259286 ghfc_utils-0.0.3/src/ghfc_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:59:33.000000 ghfc_utils-0.0.3/src/ghfc_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12125 2024-05-14 13:59:33.000000 ghfc_utils-0.0.3/src/ghfc_utils/slivar_reannotator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:59:45.259286 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3514 2024-05-14 13:59:45.000000 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      336 2024-05-14 13:59:45.000000 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:59:45.000000 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-14 13:59:45.000000 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-14 13:59:45.000000 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-14 13:59:45.000000 ghfc_utils-0.0.3/src/ghfc_utils.egg-info/top_level.txt
```

### Comparing `ghfc_utils-0.0.2/LICENSE` & `ghfc_utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ghfc_utils-0.0.2/setup.cfg` & `ghfc_utils-0.0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ghfc_utils
-version = v0.0.2
+version = v0.0.3
 author = Freddy Cliquet
 author_email = freddy.cliquet@pasteur.fr
 description = Various tools and scripts used in the GHFC lab
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.pasteur.fr/ghfc/ghfc-utils
 licence = MIT License
@@ -20,14 +20,15 @@
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	numpy
 	pandas
 	argparse
 	pyranges
+	yaml
 
 [options.package_data]
 * = *.yaml
 
 [options.entry_points]
 console_scripts = 
 	ghfc-reannotate = ghfc_utils:slivar_reannotator.main
```

### Comparing `ghfc_utils-0.0.2/src/ghfc_utils/slivar_reannotator.py` & `ghfc_utils-0.0.3/src/ghfc_utils/slivar_reannotator.py`

 * *Files identical despite different names*

