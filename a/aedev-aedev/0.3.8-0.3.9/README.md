# Comparing `tmp/aedev_aedev-0.3.8.tar.gz` & `tmp/aedev_aedev-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aedev_aedev-0.3.8.tar", last modified: Sun Jan 16 18:10:25 2022, max compression
+gzip compressed data, was "dist/aedev_aedev-0.3.9.tar", last modified: Tue Jan 18 16:43:35 2022, max compression
```

## Comparing `aedev_aedev-0.3.8.tar` & `aedev_aedev-0.3.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/
--rw-r--r--   0 root         (0) root         (0)     1691 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      680 2022-01-16 18:10:13.000000 aedev_aedev-0.3.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/aedev_aedev.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1691 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/aedev_aedev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      329 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/aedev_aedev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/aedev_aedev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/aedev_aedev.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      505 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/aedev_aedev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/aedev_aedev.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    34995 2022-01-16 18:10:13.000000 aedev_aedev-0.3.8/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      657 2022-01-16 18:10:13.000000 aedev_aedev-0.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/aedev/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/aedev/aedev/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/aedev/aedev/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2932 2022-01-16 18:10:13.000000 aedev_aedev-0.3.8/aedev/aedev/templates/de_spt_namespace-root_de_otf_de_tpl_README.md
--rw-rw-rw-   0 root         (0) root         (0)      137 2022-01-16 18:10:13.000000 aedev_aedev-0.3.8/aedev/aedev/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-16 18:10:25.000000 aedev_aedev-0.3.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/
+-rw-r--r--   0 root         (0) root         (0)     1691 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      704 2022-01-18 16:43:24.000000 aedev_aedev-0.3.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/aedev_aedev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1691 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/aedev_aedev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      329 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/aedev_aedev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/aedev_aedev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/aedev_aedev.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      543 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/aedev_aedev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/aedev_aedev.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    35001 2022-01-18 16:43:24.000000 aedev_aedev-0.3.9/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)      657 2022-01-18 16:43:24.000000 aedev_aedev-0.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/aedev/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/aedev/aedev/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/aedev/aedev/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2022-01-18 16:43:24.000000 aedev_aedev-0.3.9/aedev/aedev/templates/de_spt_namespace-root_de_otf_de_tpl_README.md
+-rw-rw-rw-   0 root         (0) root         (0)      137 2022-01-18 16:43:24.000000 aedev_aedev-0.3.9/aedev/aedev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-18 16:43:35.000000 aedev_aedev-0.3.9/setup.cfg
```

### Comparing `aedev_aedev-0.3.8/PKG-INFO` & `aedev_aedev-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aedev_aedev
-Version: 0.3.8
+Version: 0.3.9
 Summary: aedev namespace-root: aedev namespace root, providing setup, development and documentation tools/templates for Python projects.
 Home-page: https://gitlab.com/aedev-group/aedev_aedev
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Keywords: configuration,development,environment,productivity
 Platform: UNKNOWN
```

### Comparing `aedev_aedev-0.3.8/aedev_aedev.egg-info/PKG-INFO` & `aedev_aedev-0.3.9/aedev_aedev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aedev-aedev
-Version: 0.3.8
+Version: 0.3.9
 Summary: aedev namespace-root: aedev namespace root, providing setup, development and documentation tools/templates for Python projects.
 Home-page: https://gitlab.com/aedev-group/aedev_aedev
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Keywords: configuration,development,environment,productivity
 Platform: UNKNOWN
```

### Comparing `aedev_aedev-0.3.8/LICENSE.md` & `aedev_aedev-0.3.9/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project tpl_project V0.3.4 -->
+<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_project V0.3.5 -->
 ### GNU GENERAL PUBLIC LICENSE
 
 Version 3, 29 June 2007
 
 Copyright (C) 2007 Free Software Foundation, Inc.
 <https://fsf.org/>
```

### Comparing `aedev_aedev-0.3.8/README.md` & `aedev_aedev-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `aedev_aedev-0.3.8/aedev/aedev/templates/de_spt_namespace-root_de_otf_de_tpl_README.md` & `aedev_aedev-0.3.9/aedev/aedev/templates/de_spt_namespace-root_de_otf_de_tpl_README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev_tpl_namespace_root V0.3.6 -->
+<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.8 -->
 # {portion_name} {package_version}
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/{repo_group}/{package_name}/develop?logo=python)](
     {repo_url})
 [![LatestPyPIrelease](
     https://img.shields.io/gitlab/pipeline/{repo_group}/{package_name}/release{pypi_versions[-1]}?logo=python)](
     {repo_url}/-/tree/release{pypi_versions[-1]})
```

