# Comparing `tmp/auto-intersphinx-1.0.3.tar.gz` & `tmp/auto_intersphinx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-intersphinx-1.0.3.tar", last modified: Wed Jun 21 17:18:04 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `auto-intersphinx-1.0.3.tar` & `auto_intersphinx-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.359602 auto-intersphinx-1.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.351602 auto-intersphinx-1.0.3/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)     1459 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/LICENSES/BSD-3-Clause.txt
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2184 2023-06-21 17:18:04.359602 auto-intersphinx-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-21 17:13:08.000000 auto-intersphinx-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.355602 auto-intersphinx-1.0.3/doc/
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/doc/api.rst
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/doc/cli.rst
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/doc/install.rst
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)    11995 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/doc/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-06-21 17:13:08.000000 auto-intersphinx-1.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 17:18:04.359602 auto-intersphinx-1.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.351602 auto-intersphinx-1.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.355602 auto-intersphinx-1.0.3/src/auto_intersphinx/
--rw-rw-rw-   0 root         (0) root         (0)    11585 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    40377 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/catalog.json
--rw-rw-rw-   0 root         (0) root         (0)    24725 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/catalog.py
--rw-rw-rw-   0 root         (0) root         (0)     6304 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/check_packages.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/dump_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     6438 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/update_catalog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.355602 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2184 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      886 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.359602 auto-intersphinx-1.0.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.359602 auto-intersphinx-1.0.3/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)     1241 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/data/catalog.json
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/data/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     8318 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/test_auto_intersphinx.py
--rw-rw-rw-   0 root         (0) root         (0)     4675 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/test_check_packages.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/test_dump_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     7718 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/test_update_catalog.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/doc/api.rst
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/doc/cli.rst
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/doc/conf.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/doc/index.rst
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/doc/install.rst
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/doc/links.rst
+-rw-r--r--   0        0        0    11995 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/doc/usage.rst
+-rw-r--r--   0        0        0    11562 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/src/auto_intersphinx/__init__.py
+-rw-r--r--   0        0        0    39757 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/src/auto_intersphinx/catalog.json
+-rw-r--r--   0        0        0    24378 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/src/auto_intersphinx/catalog.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/src/auto_intersphinx/check_packages.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/src/auto_intersphinx/cli.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/src/auto_intersphinx/dump_objects.py
+-rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/src/auto_intersphinx/update_catalog.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     8206 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/tests/test_auto_intersphinx.py
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/tests/test_check_packages.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/tests/test_dump_objects.py
+-rw-r--r--   0        0        0     7718 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/tests/test_update_catalog.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/tests/data/catalog.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/tests/data/requirements.txt
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/README.md
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 auto_intersphinx-1.1.0/PKG-INFO
```

### Comparing `auto-intersphinx-1.0.3/LICENSES/BSD-3-Clause.txt` & `auto_intersphinx-1.1.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.3/README.md` & `auto_intersphinx-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
 SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 
 SPDX-License-Identifier: BSD-3-Clause
 -->
 
-[![latest-docs](https://img.shields.io/badge/docs-v1.0.3-orange.svg)](https://auto-intersphinx.readthedocs.io/en/v1.0.3/)
-[![build](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.3/pipeline.svg)](https://gitlab.idiap.ch/software/auto-intersphinx/commits/v1.0.3)
-[![coverage](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.3/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/auto-intersphinx/v1.0.3/coverage/index.html)
+[![latest-docs](https://img.shields.io/badge/docs-v1.1.0-orange.svg)](https://auto-intersphinx.readthedocs.io/en/v1.1.0/)
+[![build](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.1.0/pipeline.svg)](https://gitlab.idiap.ch/software/auto-intersphinx/commits/v1.1.0)
+[![coverage](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.1.0/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/auto-intersphinx/v1.1.0/coverage/index.html)
 [![repository](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/software/auto-intersphinx)
 
 # Automatically Links Package Documentation from Their Names
 
 This package contains a [Sphinx](https://www.sphinx-doc.org/) plugin that can
 fill
 [intersphinx](https://www.sphinx-doc.org/en/main/usage/extensions/intersphinx.html)
```

### Comparing `auto-intersphinx-1.0.3/doc/cli.rst` & `auto_intersphinx-1.1.0/doc/cli.rst`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.3/doc/index.rst` & `auto_intersphinx-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.3/doc/usage.rst` & `auto_intersphinx-1.1.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.3/src/auto_intersphinx/__init__.py` & `auto_intersphinx-1.1.0/src/auto_intersphinx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
-
 """Sphinx extension to automatically link package documentation from their
 names.
 
 This package contains a Sphinx plugin that can fill intersphinx mappings
 based on package names.  It simplifies the use of that plugin by
 removing the need of knowing URLs for various API catologs you may want
 to cross-reference.
@@ -89,17 +88,15 @@
             the remote address (if different than ``objects.inv``.)
     """
 
     if name not in mapping:
         mapping[name] = (addr, objects_inv)
 
     elif mapping[name][0] == addr and mapping[name][1] == objects_inv:
-        logger.info(
-            f"Ignoring repeated setting of `{name}' intersphinx_mapping"
-        )
+        logger.info(f"Ignoring repeated setting of `{name}' intersphinx_mapping")
 
     else:
         curr = mapping[name][0]
         curr += "/" if not curr.endswith("/") else ""
         curr += mapping[name][1] if mapping[name][1] else "objects.inv"
 
         newval = addr
```

### Comparing `auto-intersphinx-1.0.3/src/auto_intersphinx/catalog.json` & `auto_intersphinx-1.1.0/src/auto_intersphinx/catalog.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9716355838489762%*

 * *Differences: {"'coverage'": "{'versions': {'7.5.1': 'https://coverage.readthedocs.io/en/7.5.1/', '7.5.0': "*

 * *               "'https://coverage.readthedocs.io/en/7.5.0/', '7.4.4': "*

 * *               "'https://coverage.readthedocs.io/en/7.4.4/', '7.4.3': "*

 * *               "'https://coverage.readthedocs.io/en/7.4.3/', '7.4.2': "*

 * *               "'https://coverage.readthedocs.io/en/7.4.2/', '7.4.1': "*

 * *               "'https://coverage.readthedocs.io/en/7.4.1/', '7.4.0': "*

 * *               "'https://coverage.readthedocs.io/en/7.4.0 […]*

```diff
@@ -48,14 +48,34 @@
             "7.0.0b1": "https://coverage.readthedocs.io/en/7.0.0b1/",
             "7.0.1": "https://coverage.readthedocs.io/en/7.0.1/",
             "7.0.2": "https://coverage.readthedocs.io/en/7.0.2/",
             "7.0.3": "https://coverage.readthedocs.io/en/7.0.3/",
             "7.0.4": "https://coverage.readthedocs.io/en/7.0.4/",
             "7.0.5": "https://coverage.readthedocs.io/en/7.0.5/",
             "7.1.0": "https://coverage.readthedocs.io/en/7.1.0/",
+            "7.2.0": "https://coverage.readthedocs.io/en/7.2.0/",
+            "7.2.1": "https://coverage.readthedocs.io/en/7.2.1/",
+            "7.2.2": "https://coverage.readthedocs.io/en/7.2.2/",
+            "7.2.3": "https://coverage.readthedocs.io/en/7.2.3/",
+            "7.2.4": "https://coverage.readthedocs.io/en/7.2.4/",
+            "7.2.5": "https://coverage.readthedocs.io/en/7.2.5/",
+            "7.2.6": "https://coverage.readthedocs.io/en/7.2.6/",
+            "7.2.7": "https://coverage.readthedocs.io/en/7.2.7/",
+            "7.3.0": "https://coverage.readthedocs.io/en/7.3.0/",
+            "7.3.1": "https://coverage.readthedocs.io/en/7.3.1/",
+            "7.3.2": "https://coverage.readthedocs.io/en/7.3.2/",
+            "7.3.3": "https://coverage.readthedocs.io/en/7.3.3/",
+            "7.3.4": "https://coverage.readthedocs.io/en/7.3.4/",
+            "7.4.0": "https://coverage.readthedocs.io/en/7.4.0/",
+            "7.4.1": "https://coverage.readthedocs.io/en/7.4.1/",
+            "7.4.2": "https://coverage.readthedocs.io/en/7.4.2/",
+            "7.4.3": "https://coverage.readthedocs.io/en/7.4.3/",
+            "7.4.4": "https://coverage.readthedocs.io/en/7.4.4/",
+            "7.5.0": "https://coverage.readthedocs.io/en/7.5.0/",
+            "7.5.1": "https://coverage.readthedocs.io/en/7.5.1/",
             "coverage-4.5.4": "https://coverage.readthedocs.io/en/coverage-4.5.4/",
             "coverage-5.0": "https://coverage.readthedocs.io/en/coverage-5.0/",
             "coverage-5.0.1": "https://coverage.readthedocs.io/en/coverage-5.0.1/",
             "coverage-5.0.2": "https://coverage.readthedocs.io/en/coverage-5.0.2/",
             "coverage-5.0.3": "https://coverage.readthedocs.io/en/coverage-5.0.3/",
             "coverage-5.0.4": "https://coverage.readthedocs.io/en/coverage-5.0.4/",
             "coverage-5.1": "https://coverage.readthedocs.io/en/coverage-5.1/",
@@ -174,15 +194,21 @@
             "4.4.2": "https://docker-py.readthedocs.io/en/4.4.2/",
             "4.4.3": "https://docker-py.readthedocs.io/en/4.4.3/",
             "4.4.4": "https://docker-py.readthedocs.io/en/4.4.4/",
             "5.0.0": "https://docker-py.readthedocs.io/en/5.0.0/",
             "5.0.1": "https://docker-py.readthedocs.io/en/5.0.1/",
             "5.0.2": "https://docker-py.readthedocs.io/en/5.0.2/",
             "5.0.3": "https://docker-py.readthedocs.io/en/5.0.3/",
+            "6.0.0": "https://readthedocs.org/dashboard/docker-py/version/6.0.0/edit/",
             "6.0.1": "https://docker-py.readthedocs.io/en/6.0.1/",
+            "6.1.0": "https://docker-py.readthedocs.io/en/6.1.0/",
+            "6.1.1": "https://docker-py.readthedocs.io/en/6.1.1/",
+            "6.1.2": "https://docker-py.readthedocs.io/en/6.1.2/",
+            "6.1.3": "https://docker-py.readthedocs.io/en/6.1.3/",
+            "7.0.0": "https://docker-py.readthedocs.io/en/7.0.0/",
             "latest": "https://docker-py.readthedocs.io/en/latest/",
             "stable": "https://docker-py.readthedocs.io/en/stable/"
         }
     },
     "docopt": {
         "sources": {},
         "versions": {}
@@ -209,22 +235,25 @@
             "2.5.0": "https://docs.h5py.org/en/2.5.0/",
             "2.6.0": "https://docs.h5py.org/en/2.6.0/",
             "2.7.1": "https://docs.h5py.org/en/2.7.1/",
             "2.8.0": "https://docs.h5py.org/en/2.8.0/",
             "2.9.0": "https://docs.h5py.org/en/2.9.0/",
             "3.0.0": "https://docs.h5py.org/en/3.0.0/",
             "3.1.0": "https://docs.h5py.org/en/3.1.0/",
+            "3.10.0": "https://docs.h5py.org/en/3.10.0/",
+            "3.11.0": "https://docs.h5py.org/en/3.11.0/",
             "3.2.0": "https://docs.h5py.org/en/3.2.0/",
             "3.2.1": "https://docs.h5py.org/en/3.2.1/",
             "3.3.0": "https://docs.h5py.org/en/3.3.0/",
             "3.4.0": "https://docs.h5py.org/en/3.4.0/",
             "3.5.0": "https://docs.h5py.org/en/3.5.0/",
             "3.6.0": "https://docs.h5py.org/en/3.6.0/",
             "3.7.0": "https://docs.h5py.org/en/3.7.0/",
             "3.8.0": "https://docs.h5py.org/en/3.8.0/",
+            "3.9.0": "https://docs.h5py.org/en/3.9.0/",
             "latest": "https://docs.h5py.org/en/latest/",
             "stable": "https://docs.h5py.org/en/stable/"
         }
     },
     "imageio": {
         "sources": {
             "readthedocs": "imageio"
@@ -271,14 +300,33 @@
             "v2.22.2": "https://imageio.readthedocs.io/en/v2.22.2/",
             "v2.22.3": "https://imageio.readthedocs.io/en/v2.22.3/",
             "v2.22.4": "https://imageio.readthedocs.io/en/v2.22.4/",
             "v2.23.0": "https://imageio.readthedocs.io/en/v2.23.0/",
             "v2.24.0": "https://imageio.readthedocs.io/en/v2.24.0/",
             "v2.25.0": "https://imageio.readthedocs.io/en/v2.25.0/",
             "v2.25.1": "https://imageio.readthedocs.io/en/v2.25.1/",
+            "v2.26.0": "https://imageio.readthedocs.io/en/v2.26.0/",
+            "v2.26.1": "https://imageio.readthedocs.io/en/v2.26.1/",
+            "v2.27.0": "https://imageio.readthedocs.io/en/v2.27.0/",
+            "v2.28.0": "https://imageio.readthedocs.io/en/v2.28.0/",
+            "v2.28.1": "https://imageio.readthedocs.io/en/v2.28.1/",
+            "v2.29.0": "https://imageio.readthedocs.io/en/v2.29.0/",
+            "v2.30.0": "https://imageio.readthedocs.io/en/v2.30.0/",
+            "v2.31.0": "https://imageio.readthedocs.io/en/v2.31.0/",
+            "v2.31.1": "https://imageio.readthedocs.io/en/v2.31.1/",
+            "v2.31.2": "https://imageio.readthedocs.io/en/v2.31.2/",
+            "v2.31.3": "https://imageio.readthedocs.io/en/v2.31.3/",
+            "v2.31.4": "https://imageio.readthedocs.io/en/v2.31.4/",
+            "v2.31.5": "https://imageio.readthedocs.io/en/v2.31.5/",
+            "v2.31.6": "https://imageio.readthedocs.io/en/v2.31.6/",
+            "v2.32.0": "https://imageio.readthedocs.io/en/v2.32.0/",
+            "v2.33.0": "https://imageio.readthedocs.io/en/v2.33.0/",
+            "v2.33.1": "https://imageio.readthedocs.io/en/v2.33.1/",
+            "v2.34.0": "https://imageio.readthedocs.io/en/v2.34.0/",
+            "v2.34.1": "https://imageio.readthedocs.io/en/v2.34.1/",
             "v2.4.1": "https://imageio.readthedocs.io/en/v2.4.1/",
             "v2.5.0": "https://imageio.readthedocs.io/en/v2.5.0/",
             "v2.6.1": "https://imageio.readthedocs.io/en/v2.6.1/",
             "v2.8.0": "https://imageio.readthedocs.io/en/v2.8.0/",
             "v2.9.0": "https://imageio.readthedocs.io/en/v2.9.0/"
         }
     },
@@ -296,17 +344,14 @@
             "3.1.x": "https://jinja.palletsprojects.com/en/3.1.x/",
             "latest": "https://jinja.palletsprojects.com/en/latest/"
         }
     },
     "lightning": {
         "sources": {},
         "versions": {
-            "2.0.0": "https://lightning.ai/docs/pytorch/2.0.0/",
-            "2.0.1": "https://lightning.ai/docs/pytorch/2.0.1/",
-            "2.0.2": "https://lightning.ai/docs/pytorch/2.0.2/",
             "latest": "https://lightning.ai/docs/pytorch/latest/",
             "stable": "https://lightning.ai/docs/pytorch/stable/"
         }
     },
     "matplotlib": {
         "sources": {},
         "versions": {
@@ -362,14 +407,25 @@
             "0.55.2": "https://numba.readthedocs.io/en/0.55.2/",
             "0.56.0": "https://numba.readthedocs.io/en/0.56.0/",
             "0.56.0rc1": "https://numba.readthedocs.io/en/0.56.0rc1/",
             "0.56.1": "https://numba.readthedocs.io/en/0.56.1/",
             "0.56.2": "https://numba.readthedocs.io/en/0.56.2/",
             "0.56.3": "https://numba.readthedocs.io/en/0.56.3/",
             "0.56.4": "https://numba.readthedocs.io/en/0.56.4/",
+            "0.57.0": "https://numba.readthedocs.io/en/0.57.0/",
+            "0.57.0rc1": "https://numba.readthedocs.io/en/0.57.0rc1/",
+            "0.57.1": "https://numba.readthedocs.io/en/0.57.1/",
+            "0.57.1rc1": "https://numba.readthedocs.io/en/0.57.1rc1/",
+            "0.58.0": "https://numba.readthedocs.io/en/0.58.0/",
+            "0.58.0rc1": "https://numba.readthedocs.io/en/0.58.0rc1/",
+            "0.58.0rc2": "https://numba.readthedocs.io/en/0.58.0rc2/",
+            "0.58.1": "https://numba.readthedocs.io/en/0.58.1/",
+            "0.59.0": "https://numba.readthedocs.io/en/0.59.0/",
+            "0.59.0rc1": "https://numba.readthedocs.io/en/0.59.0rc1/",
+            "0.59.1": "https://numba.readthedocs.io/en/0.59.1/",
             "latest": "https://numba.readthedocs.io/en/latest/",
             "stable": "https://numba.readthedocs.io/en/stable/"
         }
     },
     "numpy": {
         "sources": {
             "pypi": "numpy"
@@ -433,14 +489,26 @@
     },
     "psutil": {
         "sources": {
             "readthedocs": "psutil"
         },
         "versions": {
             "latest": "https://psutil.readthedocs.io/en/latest/",
+            "release-2.2.1": "https://readthedocs.org/dashboard/psutil/version/release-2.2.1/edit/",
+            "release-3.0.1": "https://readthedocs.org/dashboard/psutil/version/release-3.0.1/edit/",
+            "release-3.1.1": "https://readthedocs.org/dashboard/psutil/version/release-3.1.1/edit/",
+            "release-3.2.2": "https://readthedocs.org/dashboard/psutil/version/release-3.2.2/edit/",
+            "release-3.4.2": "https://readthedocs.org/dashboard/psutil/version/release-3.4.2/edit/",
+            "release-4.2.0": "https://readthedocs.org/dashboard/psutil/version/release-4.2.0/edit/",
+            "release-4.3.1": "https://readthedocs.org/dashboard/psutil/version/release-4.3.1/edit/",
+            "release-4.4.2": "https://readthedocs.org/dashboard/psutil/version/release-4.4.2/edit/",
+            "release-5.0.1": "https://readthedocs.org/dashboard/psutil/version/release-5.0.1/edit/",
+            "release-5.1.3": "https://readthedocs.org/dashboard/psutil/version/release-5.1.3/edit/",
+            "release-5.2.2": "https://readthedocs.org/dashboard/psutil/version/release-5.2.2/edit/",
+            "release-5.3.0": "https://readthedocs.org/dashboard/psutil/version/release-5.3.0/edit/",
             "stable": "https://psutil.readthedocs.io/en/stable/"
         }
     },
     "pybind11": {
         "sources": {
             "readthedocs": "pybind11"
         },
@@ -455,14 +523,19 @@
         },
         "versions": {
             "4.6.x": "https://docs.pytest.org/en/4.6.x/",
             "6.2.x": "https://docs.pytest.org/en/6.2.x/",
             "7.0.x": "https://docs.pytest.org/en/7.0.x/",
             "7.1.x": "https://docs.pytest.org/en/7.1.x/",
             "7.2.x": "https://docs.pytest.org/en/7.2.x/",
+            "7.3.x": "https://docs.pytest.org/en/7.3.x/",
+            "7.4.x": "https://docs.pytest.org/en/7.4.x/",
+            "8.0.x": "https://docs.pytest.org/en/8.0.x/",
+            "8.1.x": "https://docs.pytest.org/en/8.1.x/",
+            "8.2.x": "https://docs.pytest.org/en/8.2.x/",
             "latest": "https://docs.pytest.org/en/latest/",
             "stable": "https://docs.pytest.org/en/stable/"
         }
     },
     "pytest-cov": {
         "sources": {
             "readthedocs": "pytest-cov"
@@ -496,121 +569,18 @@
             "3.8.x": "https://docs.python.org/3.8/",
             "3.9.x": "https://docs.python.org/3.9/",
             "3.x.x": "https://docs.python.org/3/",
             "stable": "https://docs.python.org/"
         }
     },
     "pytorch-lightning": {
-        "sources": {
-            "readthedocs": "pytorch-lightning"
-        },
+        "sources": {},
         "versions": {
-            "0.10.0": "https://pytorch-lightning.readthedocs.io/en/0.10.0/",
-            "0.4.9": "https://pytorch-lightning.readthedocs.io/en/0.4.9/",
-            "0.5.3": "https://pytorch-lightning.readthedocs.io/en/0.5.3/",
-            "0.6.0": "https://pytorch-lightning.readthedocs.io/en/0.6.0/",
-            "0.7.0": "https://pytorch-lightning.readthedocs.io/en/0.7.0/",
-            "0.7.1": "https://pytorch-lightning.readthedocs.io/en/0.7.1/",
-            "0.7.2": "https://pytorch-lightning.readthedocs.io/en/0.7.2/",
-            "0.7.3": "https://pytorch-lightning.readthedocs.io/en/0.7.3/",
-            "0.7.4": "https://pytorch-lightning.readthedocs.io/en/0.7.4/",
-            "0.7.5": "https://pytorch-lightning.readthedocs.io/en/0.7.5/",
-            "0.7.6": "https://pytorch-lightning.readthedocs.io/en/0.7.6/",
-            "0.8.0": "https://pytorch-lightning.readthedocs.io/en/0.8.0/",
-            "0.8.1": "https://pytorch-lightning.readthedocs.io/en/0.8.1/",
-            "0.8.2": "https://pytorch-lightning.readthedocs.io/en/0.8.2/",
-            "0.8.3": "https://pytorch-lightning.readthedocs.io/en/0.8.3/",
-            "0.8.4": "https://pytorch-lightning.readthedocs.io/en/0.8.4/",
-            "0.8.5": "https://pytorch-lightning.readthedocs.io/en/0.8.5/",
-            "0.9.0": "https://pytorch-lightning.readthedocs.io/en/0.9.0/",
-            "1.0.0": "https://pytorch-lightning.readthedocs.io/en/1.0.0/",
-            "1.0.1": "https://pytorch-lightning.readthedocs.io/en/1.0.1/",
-            "1.0.2": "https://pytorch-lightning.readthedocs.io/en/1.0.2/",
-            "1.0.3": "https://pytorch-lightning.readthedocs.io/en/1.0.3/",
-            "1.0.4": "https://pytorch-lightning.readthedocs.io/en/1.0.4/",
-            "1.0.5": "https://pytorch-lightning.readthedocs.io/en/1.0.5/",
-            "1.0.6": "https://pytorch-lightning.readthedocs.io/en/1.0.6/",
-            "1.0.7": "https://pytorch-lightning.readthedocs.io/en/1.0.7/",
-            "1.0.8": "https://pytorch-lightning.readthedocs.io/en/1.0.8/",
-            "1.1.0": "https://pytorch-lightning.readthedocs.io/en/1.1.0/",
-            "1.1.1": "https://pytorch-lightning.readthedocs.io/en/1.1.1/",
-            "1.1.2": "https://pytorch-lightning.readthedocs.io/en/1.1.2/",
-            "1.1.3": "https://pytorch-lightning.readthedocs.io/en/1.1.3/",
-            "1.1.4": "https://pytorch-lightning.readthedocs.io/en/1.1.4/",
-            "1.1.5": "https://pytorch-lightning.readthedocs.io/en/1.1.5/",
-            "1.1.6": "https://pytorch-lightning.readthedocs.io/en/1.1.6/",
-            "1.1.7": "https://pytorch-lightning.readthedocs.io/en/1.1.7/",
-            "1.1.8": "https://pytorch-lightning.readthedocs.io/en/1.1.8/",
-            "1.2.0": "https://pytorch-lightning.readthedocs.io/en/1.2.0/",
-            "1.2.1": "https://pytorch-lightning.readthedocs.io/en/1.2.1/",
-            "1.2.10": "https://pytorch-lightning.readthedocs.io/en/1.2.10/",
-            "1.2.2": "https://pytorch-lightning.readthedocs.io/en/1.2.2/",
-            "1.2.3": "https://pytorch-lightning.readthedocs.io/en/1.2.3/",
-            "1.2.4": "https://pytorch-lightning.readthedocs.io/en/1.2.4/",
-            "1.2.5": "https://pytorch-lightning.readthedocs.io/en/1.2.5/",
-            "1.2.6": "https://pytorch-lightning.readthedocs.io/en/1.2.6/",
-            "1.2.7": "https://pytorch-lightning.readthedocs.io/en/1.2.7/",
-            "1.2.8": "https://pytorch-lightning.readthedocs.io/en/1.2.8/",
-            "1.3.0": "https://pytorch-lightning.readthedocs.io/en/1.3.0/",
-            "1.3.1": "https://pytorch-lightning.readthedocs.io/en/1.3.1/",
-            "1.3.2": "https://pytorch-lightning.readthedocs.io/en/1.3.2/",
-            "1.3.3": "https://pytorch-lightning.readthedocs.io/en/1.3.3/",
-            "1.3.4": "https://pytorch-lightning.readthedocs.io/en/1.3.4/",
-            "1.3.5": "https://pytorch-lightning.readthedocs.io/en/1.3.5/",
-            "1.3.6": "https://pytorch-lightning.readthedocs.io/en/1.3.6/",
-            "1.3.7": "https://pytorch-lightning.readthedocs.io/en/1.3.7/",
-            "1.3.8": "https://pytorch-lightning.readthedocs.io/en/1.3.8/",
-            "1.4.0": "https://pytorch-lightning.readthedocs.io/en/1.4.0/",
-            "1.4.1": "https://pytorch-lightning.readthedocs.io/en/1.4.1/",
-            "1.4.2": "https://pytorch-lightning.readthedocs.io/en/1.4.2/",
-            "1.4.3": "https://pytorch-lightning.readthedocs.io/en/1.4.3/",
-            "1.4.4": "https://pytorch-lightning.readthedocs.io/en/1.4.4/",
-            "1.4.5": "https://pytorch-lightning.readthedocs.io/en/1.4.5/",
-            "1.4.6": "https://pytorch-lightning.readthedocs.io/en/1.4.6/",
-            "1.4.7": "https://pytorch-lightning.readthedocs.io/en/1.4.7/",
-            "1.4.8": "https://pytorch-lightning.readthedocs.io/en/1.4.8/",
-            "1.4.9": "https://pytorch-lightning.readthedocs.io/en/1.4.9/",
-            "1.5.0": "https://pytorch-lightning.readthedocs.io/en/1.5.0/",
-            "1.5.1": "https://pytorch-lightning.readthedocs.io/en/1.5.1/",
-            "1.5.10": "https://pytorch-lightning.readthedocs.io/en/1.5.10/",
-            "1.5.2": "https://pytorch-lightning.readthedocs.io/en/1.5.2/",
-            "1.5.3": "https://pytorch-lightning.readthedocs.io/en/1.5.3/",
-            "1.5.4": "https://pytorch-lightning.readthedocs.io/en/1.5.4/",
-            "1.5.5": "https://pytorch-lightning.readthedocs.io/en/1.5.5/",
-            "1.5.6": "https://pytorch-lightning.readthedocs.io/en/1.5.6/",
-            "1.5.7": "https://pytorch-lightning.readthedocs.io/en/1.5.7/",
-            "1.5.8": "https://pytorch-lightning.readthedocs.io/en/1.5.8/",
-            "1.5.9": "https://pytorch-lightning.readthedocs.io/en/1.5.9/",
-            "1.6.0": "https://pytorch-lightning.readthedocs.io/en/1.6.0/",
-            "1.6.1": "https://pytorch-lightning.readthedocs.io/en/1.6.1/",
-            "1.6.2": "https://pytorch-lightning.readthedocs.io/en/1.6.2/",
-            "1.6.3": "https://pytorch-lightning.readthedocs.io/en/1.6.3/",
-            "1.6.4": "https://pytorch-lightning.readthedocs.io/en/1.6.4/",
-            "1.6.5": "https://pytorch-lightning.readthedocs.io/en/1.6.5/",
-            "1.7.0": "https://pytorch-lightning.readthedocs.io/en/1.7.0/",
-            "1.7.1": "https://pytorch-lightning.readthedocs.io/en/1.7.1/",
-            "1.7.2": "https://pytorch-lightning.readthedocs.io/en/1.7.2/",
-            "1.7.3": "https://pytorch-lightning.readthedocs.io/en/1.7.3/",
-            "1.7.4": "https://pytorch-lightning.readthedocs.io/en/1.7.4/",
-            "1.7.5": "https://pytorch-lightning.readthedocs.io/en/1.7.5/",
-            "1.7.6": "https://pytorch-lightning.readthedocs.io/en/1.7.6/",
-            "1.7.7": "https://pytorch-lightning.readthedocs.io/en/1.7.7/",
-            "1.8.0": "https://pytorch-lightning.readthedocs.io/en/1.8.0/",
-            "1.8.1": "https://pytorch-lightning.readthedocs.io/en/1.8.1/",
-            "1.8.2": "https://pytorch-lightning.readthedocs.io/en/1.8.2/",
-            "1.8.3": "https://pytorch-lightning.readthedocs.io/en/1.8.3/",
-            "1.8.4": "https://pytorch-lightning.readthedocs.io/en/1.8.4/",
-            "1.8.5": "https://pytorch-lightning.readthedocs.io/en/1.8.5/",
-            "1.8.6": "https://pytorch-lightning.readthedocs.io/en/1.8.6/",
-            "1.9.0": "https://pytorch-lightning.readthedocs.io/en/1.9.0/",
-            "1.9.1": "https://pytorch-lightning.readthedocs.io/en/1.9.1/",
-            "1.9.2": "https://pytorch-lightning.readthedocs.io/en/1.9.2/",
-            "future-structure": "https://pytorch-lightning.readthedocs.io/en/future-structure/",
-            "latest": "https://lightning.ai/docs/pytorch/latest/",
-            "stable": "https://lightning.ai/docs/pytorch/stable/"
+            "latest": "https://pytorch-lightning.readthedocs.io/en/latest/",
+            "stable": "https://pytorch-lightning.readthedocs.io/en/stable/"
         }
     },
     "pyyaml": {
         "sources": {},
         "versions": {}
     },
     "pyzmq": {
@@ -627,14 +597,15 @@
             "v15.2.0": "https://pyzmq.readthedocs.io/en/v15.2.0/",
             "v15.3.0": "https://pyzmq.readthedocs.io/en/v15.3.0/",
             "v15.4.0": "https://pyzmq.readthedocs.io/en/v15.4.0/",
             "v16.0.0": "https://pyzmq.readthedocs.io/en/v16.0.0/",
             "v16.0.1": "https://pyzmq.readthedocs.io/en/v16.0.1/",
             "v16.0.2": "https://pyzmq.readthedocs.io/en/v16.0.2/",
             "v16.0.3": "https://pyzmq.readthedocs.io/en/v16.0.3/",
+            "v16.0.4": "https://readthedocs.org/dashboard/pyzmq/version/v16.0.4/edit/",
             "v17.0.0": "https://pyzmq.readthedocs.io/en/v17.0.0/",
             "v17.1.0": "https://pyzmq.readthedocs.io/en/v17.1.0/",
             "v17.1.1": "https://pyzmq.readthedocs.io/en/v17.1.1/",
             "v17.1.2": "https://pyzmq.readthedocs.io/en/v17.1.2/",
             "v17.1.3": "https://pyzmq.readthedocs.io/en/v17.1.3/",
             "v18.0.2": "https://pyzmq.readthedocs.io/en/v18.0.2/",
             "v18.1.1": "https://pyzmq.readthedocs.io/en/v18.1.1/",
@@ -649,15 +620,24 @@
             "v22.3.0": "https://pyzmq.readthedocs.io/en/v22.3.0/",
             "v23.0.0": "https://pyzmq.readthedocs.io/en/v23.0.0/",
             "v23.1.0": "https://pyzmq.readthedocs.io/en/v23.1.0/",
             "v23.2.0": "https://pyzmq.readthedocs.io/en/v23.2.0/",
             "v23.2.1": "https://pyzmq.readthedocs.io/en/v23.2.1/",
             "v24.0.0": "https://pyzmq.readthedocs.io/en/v24.0.0/",
             "v24.0.1": "https://pyzmq.readthedocs.io/en/v24.0.1/",
-            "v25.0.0": "https://pyzmq.readthedocs.io/en/v25.0.0/"
+            "v25.0.0": "https://pyzmq.readthedocs.io/en/v25.0.0/",
+            "v25.0.1": "https://pyzmq.readthedocs.io/en/v25.0.1/",
+            "v25.0.2": "https://pyzmq.readthedocs.io/en/v25.0.2/",
+            "v25.1.0": "https://pyzmq.readthedocs.io/en/v25.1.0/",
+            "v25.1.1": "https://pyzmq.readthedocs.io/en/v25.1.1/",
+            "v25.1.2": "https://pyzmq.readthedocs.io/en/v25.1.2/",
+            "v26.0.0": "https://pyzmq.readthedocs.io/en/v26.0.0/",
+            "v26.0.1": "https://pyzmq.readthedocs.io/en/v26.0.1/",
+            "v26.0.2": "https://pyzmq.readthedocs.io/en/v26.0.2/",
+            "v26.0.3": "https://pyzmq.readthedocs.io/en/v26.0.3/"
         }
     },
     "requests": {
         "sources": {
             "readthedocs": "requests"
         },
         "versions": {
@@ -773,18 +753,23 @@
             "v3.16.1": "https://simplejson.readthedocs.io/en/v3.16.1/",
             "v3.17.0": "https://simplejson.readthedocs.io/en/v3.17.0/",
             "v3.17.1": "https://simplejson.readthedocs.io/en/v3.17.1/",
             "v3.17.2": "https://simplejson.readthedocs.io/en/v3.17.2/",
             "v3.17.3": "https://simplejson.readthedocs.io/en/v3.17.3/",
             "v3.17.4": "https://simplejson.readthedocs.io/en/v3.17.4/",
             "v3.17.5": "https://simplejson.readthedocs.io/en/v3.17.5/",
+            "v3.17.6": "https://readthedocs.org/dashboard/simplejson/version/v3.17.6/edit/",
             "v3.18.0": "https://simplejson.readthedocs.io/en/v3.18.0/",
             "v3.18.1": "https://simplejson.readthedocs.io/en/v3.18.1/",
             "v3.18.2": "https://simplejson.readthedocs.io/en/v3.18.2/",
-            "v3.18.3": "https://simplejson.readthedocs.io/en/v3.18.3/"
+            "v3.18.3": "https://simplejson.readthedocs.io/en/v3.18.3/",
+            "v3.18.4": "https://simplejson.readthedocs.io/en/v3.18.4/",
+            "v3.19.0": "https://simplejson.readthedocs.io/en/v3.19.0/",
+            "v3.19.1": "https://simplejson.readthedocs.io/en/v3.19.1/",
+            "v3.19.2": "https://readthedocs.org/dashboard/simplejson/version/v3.19.2/edit/"
         }
     },
     "six": {
         "sources": {
             "readthedocs": "six"
         },
         "versions": {
@@ -818,22 +803,27 @@
         }
     },
     "sphinx_rtd_theme": {
         "sources": {
             "readthedocs": "sphinx_rtd_theme"
         },
         "versions": {
+            "0.4.3": "https://readthedocs.org/dashboard/sphinx-rtd-theme/version/0.4.3/edit/",
             "0.5.0": "https://sphinx-rtd-theme.readthedocs.io/en/0.5.0/",
             "0.5.1": "https://sphinx-rtd-theme.readthedocs.io/en/0.5.1/",
             "0.5.2": "https://sphinx-rtd-theme.readthedocs.io/en/0.5.2/",
             "1.0.0": "https://sphinx-rtd-theme.readthedocs.io/en/1.0.0/",
             "1.0.0rc1": "https://sphinx-rtd-theme.readthedocs.io/en/1.0.0rc1/",
             "1.1.0": "https://sphinx-rtd-theme.readthedocs.io/en/1.1.0/",
             "1.1.1": "https://sphinx-rtd-theme.readthedocs.io/en/1.1.1/",
             "1.2.0": "https://sphinx-rtd-theme.readthedocs.io/en/1.2.0/",
+            "1.2.1": "https://sphinx-rtd-theme.readthedocs.io/en/1.2.1/",
+            "1.2.2": "https://sphinx-rtd-theme.readthedocs.io/en/1.2.2/",
+            "1.3.0": "https://sphinx-rtd-theme.readthedocs.io/en/1.3.0/",
+            "2.0.0": "https://sphinx-rtd-theme.readthedocs.io/en/2.0.0/",
             "latest": "https://sphinx-rtd-theme.readthedocs.io/en/latest/",
             "stable": "https://sphinx-rtd-theme.readthedocs.io/en/stable/",
             "test-pelson-fix-sphinx-version-not-three-ints": "https://sphinx-rtd-theme.readthedocs.io/en/test-pelson-fix-sphinx-version-not-three-ints/"
         }
     },
     "sphinxcontrib-programoutput": {
         "sources": {
@@ -890,14 +880,21 @@
     },
     "torch": {
         "sources": {},
         "versions": {
             "stable": "https://pytorch.org/docs/stable/"
         }
     },
+    "torchmetrics": {
+        "sources": {},
+        "versions": {
+            "latest": "https://lightning.ai/docs/torchmetrics/latest/",
+            "stable": "https://lightning.ai/docs/torchmetrics/stable/"
+        }
+    },
     "torchvision": {
         "sources": {},
         "versions": {
             "stable": "https://pytorch.org/vision/stable/"
         }
     },
     "tqdm": {
```

### Comparing `auto-intersphinx-1.0.3/src/auto_intersphinx/catalog.py` & `auto_intersphinx-1.1.0/src/auto_intersphinx/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
-
 """This module contains instructions for documentation lookup."""
 
 from __future__ import annotations  # not required for Python >= 3.10
 
 import collections.abc
 import importlib.metadata
 import importlib.resources
@@ -24,17 +23,15 @@
 logger = logging.getLogger(__name__)
 
 
 PackageDictionaryType = dict[str, dict[str, str]]
 """Type for the internal values of :py:class:`Catalog`"""
 
 
-BUILTIN_CATALOG = importlib.resources.files(__package__).joinpath(
-    "catalog.json"
-)
+BUILTIN_CATALOG = importlib.resources.files(__package__).joinpath("catalog.json")
 """Base name for the catalog file distributed with this package."""
 
 
 PEP440_RE = re.compile(
     r"^\s*" + packaging.version.VERSION_PATTERN + r"\s*$",
     re.VERBOSE | re.IGNORECASE,
 )
@@ -132,24 +129,20 @@
         A dictionary, which contains all versions of documentation available
         for the given package on RTD.  If the package's documentation is not
         available on RTD, returns an empty dictionary.
     """
     try:
         url = f"https://readthedocs.org/projects/{package}/versions/"
         logger.debug(f"Reaching for `{url}'...")
-        r = requests.get(
-            f"https://readthedocs.org/projects/{package}/versions/"
-        )
+        r = requests.get(f"https://readthedocs.org/projects/{package}/versions/")
         if r.ok:
             tree = lxml.html.fromstring(r.text)
             return {
                 k.text: _ensure_webdir(k.attrib["href"])
-                for k in tree.xpath(
-                    "//a[contains(@class, 'module-item-title')]"
-                )
+                for k in tree.xpath("//a[contains(@class, 'module-item-title')]")
                 if k.attrib["href"].startswith("http")
             }
 
     except requests.exceptions.RequestException:
         pass
 
     return {}
@@ -213,17 +206,15 @@
     }
     versions_to_probe = sorted(list(version_map.keys()), reverse=True)
 
     if max_entries >= 0:
         versions_to_probe = versions_to_probe[:max_entries]
 
     for k in versions_to_probe:
-        data = _get_json(
-            f"https://pypi.org/pypi/{package}/{version_map[k]}/json"
-        )
+        data = _get_json(f"https://pypi.org/pypi/{package}/{version_map[k]}/json")
         if data is None:
             continue
 
         urls = data["info"]["project_urls"]
         addr = urls.get("Documentation") or urls.get("documentation")
         if addr is not None:
             addr = _ensure_webdir(addr)
@@ -318,17 +309,15 @@
 
     def _ensure_defaults(self, pkg: str) -> None:
         """Ensures a standardised setup for a package entry."""
         self.setdefault(pkg, {"versions": {}, "sources": {}})
         self[pkg].setdefault("versions", {})
         self[pkg].setdefault("sources", {})
 
-    def update_versions_from_environment(
-        self, pkg: str, name: str | None
-    ) -> bool:
+    def update_versions_from_environment(self, pkg: str, name: str | None) -> bool:
         """Replaces package documentation URLs using information from current
         Python environment.
 
         Arguments:
 
             pkg: Name of the package as one would find in pypi.org. This
               name can be different then that of the Python package
@@ -346,17 +335,15 @@
             ``False``, otherwise.
         """
 
         self._ensure_defaults(pkg)
 
         name = name or pkg
 
-        logger.debug(
-            f"{pkg}: checking current Python environment for {name}..."
-        )
+        logger.debug(f"{pkg}: checking current Python environment for {name}...")
 
         versions = docurls_from_environment(name)
         logger.debug(
             f"{pkg}: Found {len(versions)} doc URL(s) at current Python environment"
         )
 
         if versions:
@@ -388,17 +375,15 @@
         self._ensure_defaults(pkg)
 
         name = name or pkg
 
         logger.debug(f"{pkg}: checking readthedocs.org for {name}...")
 
         versions = docurls_from_rtd(name)
-        logger.debug(
-            f"{pkg}: Found {len(versions)} doc URL(s) at readthedocs.org"
-        )
+        logger.debug(f"{pkg}: Found {len(versions)} doc URL(s) at readthedocs.org")
 
         if versions:
             self[pkg]["versions"].update(versions)
             self[pkg]["versions"] = _reorder_versions(self[pkg]["versions"])
             self[pkg]["sources"]["readthedocs"] = name
 
         return len(versions) > 0
@@ -515,29 +500,25 @@
                         ok = self.update_versions_from_rtd(pkg, name)
                         if ok and not keep_going:
                             break
 
                 elif action == "pypi":
                     name = names.get(action, {}).get(pkg, pkg)
                     if name is not None:
-                        ok = self.update_versions_from_pypi(
-                            pkg, name, pypi_max_entries
-                        )
+                        ok = self.update_versions_from_pypi(pkg, name, pypi_max_entries)
                         if ok and not keep_going:
                             break
 
                 else:
                     raise RuntimeError(f"Unrecognized source: {action}")
 
     def self_update(self) -> None:
         """Runs a self-update procedure, by re-looking up known sources."""
         # organises the names as expected by update_versions()
-        names: dict[str, dict[str, str]] = dict(
-            environment={}, readthedocs={}, pypi={}
-        )
+        names: dict[str, dict[str, str]] = dict(environment={}, readthedocs={}, pypi={})
         for pkg, info in self.items():
             for src in ("environment", "readthedocs", "pypi"):
                 names[src][pkg] = info["sources"].get(src)
 
         self.update_versions(pkgs=self.keys(), names=names)
 
 
@@ -600,32 +581,28 @@
     retval: dict[str, str] = {}
     if sorted_versions:
         # there is at least 1 (valid) version number
         latest = sorted_versions[-1]
         retval["latest"] = versions.get("latest", versions[version_map[latest]])
 
         stable_versions = [
-            k
-            for k in sorted_versions
-            if not (k.is_prerelease or k.is_devrelease)
+            k for k in sorted_versions if not (k.is_prerelease or k.is_devrelease)
         ]
         if stable_versions:
             stable = stable_versions[-1]
         else:
             stable = latest
         retval["stable"] = versions.get("stable", versions[version_map[stable]])
 
         # fill-in the remainder of the versions, leave latest on top
         for k in reversed(sorted_versions):
             retval[version_map[k]] = versions[version_map[k]]
             if ".x" in version_map[k]:
                 # copy to a shortened version number as well
-                retval[version_map[k].replace(".x", "")] = versions[
-                    version_map[k]
-                ]
+                retval[version_map[k].replace(".x", "")] = versions[version_map[k]]
             elif k.public != version_map[k]:
                 # copy a standardised version number as well
                 retval[k.public] = versions[version_map[k]]
 
     else:
         # there is either nothing, or just aliases such as stable/latest
         retval["latest"] = (
@@ -659,31 +636,25 @@
         self.reset()
 
     def reset(self):
         """Internally creates all possible aliases for package names and
         versions.
 
         This method will expand the catalog package names and version
-        numbers
-        so that the user can refer to these using environment,
-        readthedocs.org
-        or pypi.org names for packages, and PEP-440 compatible strings
-        for
-        version names during the lookup.
+        numbers so that the user can refer to these using environment,
+        readthedocs.org or pypi.org names for packages, and PEP-440
+        compatible strings for version names during the lookup.
 
         The catalog associated to this lookup is not modified in this
-        process.
-        All augmentations are built-into the object instance.
+        process. All augmentations are built-into the object instance.
         """
         self._version_map: dict[str, dict[str, str]] = {}
         self._package_map: dict[str, str] = {}
         for pkg in self._catalog.keys():
-            self._version_map[pkg] = _prepare_versions(
-                self._catalog[pkg]["versions"]
-            )
+            self._version_map[pkg] = _prepare_versions(self._catalog[pkg]["versions"])
 
             # translations from Python, rtd.org or pypi.org names
             self._package_map[pkg] = pkg
             self._package_map.update(
                 {v: pkg for v in self._catalog[pkg]["sources"].values()}
             )
```

### Comparing `auto-intersphinx-1.0.3/src/auto_intersphinx/check_packages.py` & `auto_intersphinx-1.1.0/src/auto_intersphinx/check_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 
 def _main(args) -> None:
     """Main function, that actually executes the check-package command."""
     setup_verbosity(args.verbose)
 
     builtin_catalog = Catalog()
     if not args.no_builtin:
-        catalog_file = importlib.resources.files(
-            __name__.split(".", 1)[0]
-        ).joinpath("catalog.json")
+        catalog_file = importlib.resources.files(__name__.split(".", 1)[0]).joinpath(
+            "catalog.json"
+        )
         builtin_catalog.loads(catalog_file.read_text())
 
     user_catalog = Catalog()
     if args.user:
         user_catalog.load(args.user)
 
     for p in args.packages:
@@ -55,17 +55,15 @@
             )
             if not args.keep_going:
                 continue
 
         if not args.no_environment:
             versions = docurls_from_environment(p)
             if versions:
-                print(
-                    f"Found {p} documentation in installed Python environment:"
-                )
+                print(f"Found {p} documentation in installed Python environment:")
                 print(textwrap.indent(json.dumps(versions, indent=2), "  | "))
                 if not args.keep_going:
                     continue
 
         if not args.no_rtd:
             versions = docurls_from_rtd(p)
             if versions:
```

### Comparing `auto-intersphinx-1.0.3/src/auto_intersphinx/cli.py` & `auto_intersphinx-1.1.0/src/auto_intersphinx/cli.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.3/src/auto_intersphinx/dump_objects.py` & `auto_intersphinx-1.1.0/src/auto_intersphinx/dump_objects.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.3/src/auto_intersphinx/update_catalog.py` & `auto_intersphinx-1.1.0/src/auto_intersphinx/update_catalog.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.3/tests/data/catalog.json` & `auto_intersphinx-1.1.0/tests/data/catalog.json`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.3/tests/test_auto_intersphinx.py` & `auto_intersphinx-1.1.0/tests/test_auto_intersphinx.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,16 +93,15 @@
         conf,
     )
 
     assert status == 0
 
     assert (
         f"loading intersphinx inventory from "
-        f"https://docs.python.org/{sys.version_info[0]}.{sys.version_info[1]}"
-        in stdout
+        f"https://docs.python.org/{sys.version_info[0]}.{sys.version_info[1]}" in stdout
     )
 
     assert (
         "loading intersphinx inventory from https://numpy.org/doc/stable/objects.inv"
         in stdout
     )
 
@@ -153,18 +152,15 @@
         tmp_path,
         index_rst,
         conf,
     )
 
     assert status == 0
 
-    assert (
-        "loading intersphinx inventory from https://numpy.org/doc/stable/"
-        in stdout
-    )
+    assert "loading intersphinx inventory from https://numpy.org/doc/stable/" in stdout
 
     assert "Ignoring repeated setting of `numpy' intersphinx_mapping" in stdout
 
     assert (htmldir / "index.html").exists()
 
 
 def test_conflict_from_intersphinx_mapping(tmp_path) -> None:
@@ -182,18 +178,15 @@
         tmp_path,
         index_rst,
         conf,
     )
 
     assert status == 0
 
-    assert (
-        "loading intersphinx inventory from https://numpy.org/doc/stable/"
-        in stdout
-    )
+    assert "loading intersphinx inventory from https://numpy.org/doc/stable/" in stdout
 
     assert "Ignoring repeated setting of `numpy' intersphinx_mapping" in stdout
 
     assert (htmldir / "index.html").exists()
 
 
 def test_discover_from_internal_catalog(tmp_path) -> None:
@@ -233,17 +226,15 @@
         tmp_path,
         index_rst,
         conf,
     )
 
     assert status == 0
 
-    assert (
-        "Cannot find suitable catalog entry for `setuptools@61.0.0'" in stderr
-    )
+    assert "Cannot find suitable catalog entry for `setuptools@61.0.0'" in stderr
 
     assert (htmldir / "index.html").exists()
 
 
 def test_error_unknown_package(tmp_path) -> None:
     conf = [
         "auto_intersphinx_packages=[('setuptoolx', '61.0.0'), ('dead-beef-xyz')]",
@@ -258,22 +249,17 @@
         tmp_path,
         index_rst,
         conf,
     )
 
     assert status == 0
 
-    assert (
-        "Cannot find suitable catalog entry for `setuptoolx@61.0.0'" in stderr
-    )
+    assert "Cannot find suitable catalog entry for `setuptoolx@61.0.0'" in stderr
 
-    assert (
-        "Cannot find suitable catalog entry for `dead-beef-xyz@stable'"
-        in stderr
-    )
+    assert "Cannot find suitable catalog entry for `dead-beef-xyz@stable'" in stderr
 
     assert (htmldir / "index.html").exists()
 
 
 def test_discover_from_metadata(tmp_path) -> None:
     conf = [
         "auto_intersphinx_packages=['jinja2']",
```

### Comparing `auto-intersphinx-1.0.3/tests/test_check_packages.py` & `auto_intersphinx-1.1.0/tests/test_check_packages.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,15 @@
     try:
         main(["check-packages", "-vvv", "--keep-going", "requests"])
     except SystemExit:
         pass
 
     output = capsys.readouterr().out
     assert "Found requests in builtin catalog" in output
-    assert (
-        "Found requests documentation in installed Python environment" in output
-    )
+    assert "Found requests documentation in installed Python environment" in output
     assert "Found requests documentation in readthedocs.org" in output
     assert "Found requests documentation in PyPI" in output
 
 
 def test_user_catalog(capsys, datadir):
     user_catalog = datadir / "catalog.json"
 
@@ -63,51 +61,43 @@
         main(["check-packages", "-vvv", f"--user={str(user_catalog)}", "click"])
     except SystemExit:
         pass
 
     output = capsys.readouterr().out
     assert "Found click in user catalog" in output
     assert "Found click in builtin catalog" not in output
-    assert (
-        "Found click documentation in installed Python environment"
-        not in output
-    )
+    assert "Found click documentation in installed Python environment" not in output
     assert "Found click documentation in readthedocs.org" not in output
     assert "Found click documentation in PyPI" not in output
 
 
 def test_stop_at_builtin_catalog(capsys):
     try:
         main(["check-packages", "-vvv", "requests"])
     except SystemExit:
         pass
 
     output = capsys.readouterr().out
     assert "Found requests in user catalog" not in output
     assert "Found requests in builtin catalog" in output
-    assert (
-        "Found requests documentation in installed Python environment"
-        not in output
-    )
+    assert "Found requests documentation in installed Python environment" not in output
     assert "Found requests documentation in readthedocs.org" not in output
     assert "Found requests documentation in PyPI" not in output
 
 
 def test_stop_at_environment(capsys):
     try:
         main(["check-packages", "-vvv", "--no-builtin", "requests"])
     except SystemExit:
         pass
 
     output = capsys.readouterr().out
     assert "Found requests in user catalog" not in output
     assert "Found requests in builtin catalog" not in output
-    assert (
-        "Found requests documentation in installed Python environment" in output
-    )
+    assert "Found requests documentation in installed Python environment" in output
     assert "Found requests documentation in readthedocs.org" not in output
     assert "Found requests documentation in PyPI" not in output
 
 
 def test_stop_at_readthedocs(capsys):
     try:
         main(
@@ -121,18 +111,15 @@
         )
     except SystemExit:
         pass
 
     output = capsys.readouterr().out
     assert "Found requests in user catalog" not in output
     assert "Found requests in builtin catalog" not in output
-    assert (
-        "Found requests documentation in installed Python environment"
-        not in output
-    )
+    assert "Found requests documentation in installed Python environment" not in output
     assert "Found requests documentation in readthedocs.org" in output
     assert "Found requests documentation in PyPI" not in output
 
 
 def test_stop_at_pypi(capsys):
     try:
         main(
@@ -147,13 +134,10 @@
         )
     except SystemExit:
         pass
 
     output = capsys.readouterr().out
     assert "Found requests in user catalog" not in output
     assert "Found requests in builtin catalog" not in output
-    assert (
-        "Found requests documentation in installed Python environment"
-        not in output
-    )
+    assert "Found requests documentation in installed Python environment" not in output
     assert "Found requests documentation in readthedocs.org" not in output
     assert "Found requests documentation in PyPI" in output
```

### Comparing `auto-intersphinx-1.0.3/tests/test_dump_objects.py` & `auto_intersphinx-1.1.0/tests/test_dump_objects.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.3/tests/test_update_catalog.py` & `auto_intersphinx-1.1.0/tests/test_update_catalog.py`

 * *Files identical despite different names*

