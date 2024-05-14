# Comparing `tmp/idiap-devtools-1.0.0.tar.gz` & `tmp/idiap_devtools-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idiap-devtools-1.0.0.tar", last modified: Wed Jun 21 18:05:31 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `idiap-devtools-1.0.0.tar` & `idiap_devtools-2.0.0.tar`

### file list

```diff
@@ -1,62 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:05:31.641298 idiap-devtools-1.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:05:31.633298 idiap-devtools-1.0.0/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)     1459 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/LICENSES/BSD-3-Clause.txt
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1927 2023-06-21 18:05:31.641298 idiap-devtools-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-21 18:03:18.000000 idiap-devtools-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:05:31.633298 idiap-devtools-1.0.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/doc/api.rst
--rw-rw-rw-   0 root         (0) root         (0)     4039 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/doc/catalog.json
--rw-rw-rw-   0 root         (0) root         (0)      404 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/doc/cli.rst
--rw-rw-rw-   0 root         (0) root         (0)     8672 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/doc/develop.rst
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/doc/install.rst
--rw-rw-rw-   0 root         (0) root         (0)     1020 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/doc/nitpick-exceptions.txt
--rw-rw-rw-   0 root         (0) root         (0)     2898 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/doc/release.rst
--rw-rw-rw-   0 root         (0) root         (0)     2108 2023-06-21 18:03:18.000000 idiap-devtools-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 18:05:31.641298 idiap-devtools-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:05:31.629298 idiap-devtools-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:05:31.633298 idiap-devtools-1.0.0/src/idiap_devtools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 18:05:09.000000 idiap-devtools-1.0.0/src/idiap_devtools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6227 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/click.py
--rw-rw-rw-   0 root         (0) root         (0)     3538 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/conda.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:05:31.637298 idiap-devtools-1.0.0/src/idiap_devtools/gitlab/
--rw-rw-rw-   0 root         (0) root         (0)     3147 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/gitlab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12685 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/gitlab/changelog.py
--rw-rw-rw-   0 root         (0) root         (0)    25309 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/gitlab/release.py
--rw-rw-rw-   0 root         (0) root         (0)     3672 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/gitlab/runners.py
--rw-rw-rw-   0 root         (0) root         (0)     3686 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/logging.py
--rw-rw-rw-   0 root         (0) root         (0)    11447 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/profile.py
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/python.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:05:31.637298 idiap-devtools-1.0.0/src/idiap_devtools/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 18:05:09.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    15142 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/env.py
--rw-rw-rw-   0 root         (0) root         (0)     4141 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/fullenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:05:31.641298 idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/
--rw-rw-rw-   0 root         (0) root         (0)     1114 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7100 2023-06-21 17:53:29.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/badges.py
--rw-rw-rw-   0 root         (0) root         (0)     6028 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/changelog.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/getpath.py
--rw-rw-rw-   0 root         (0) root         (0)     2215 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/lasttag.py
--rw-rw-rw-   0 root         (0) root         (0)     8825 2023-06-21 15:12:06.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/release.py
--rw-rw-rw-   0 root         (0) root         (0)     9099 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/runners.py
--rw-rw-rw-   0 root         (0) root         (0)     4897 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     6476 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/scripts/update_pins.py
--rw-rw-rw-   0 root         (0) root         (0)     5500 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/update_pins.py
--rw-rw-rw-   0 root         (0) root         (0)     3910 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/src/idiap_devtools/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:05:31.637298 idiap-devtools-1.0.0/src/idiap_devtools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1927 2023-06-21 18:05:31.000000 idiap-devtools-1.0.0/src/idiap_devtools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1550 2023-06-21 18:05:31.000000 idiap-devtools-1.0.0/src/idiap_devtools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 18:05:31.000000 idiap-devtools-1.0.0/src/idiap_devtools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-21 18:05:31.000000 idiap-devtools-1.0.0/src/idiap_devtools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      276 2023-06-21 18:05:31.000000 idiap-devtools-1.0.0/src/idiap_devtools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-21 18:05:31.000000 idiap-devtools-1.0.0/src/idiap_devtools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 18:05:31.000000 idiap-devtools-1.0.0/src/idiap_devtools.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:05:31.641298 idiap-devtools-1.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 18:05:09.000000 idiap-devtools-1.0.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/tests/test_devtools.py
--rw-rw-rw-   0 root         (0) root         (0)     2989 2023-06-21 14:11:15.000000 idiap-devtools-1.0.0/tests/test_release.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/doc/api.rst
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/doc/catalog.json
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/doc/cli.rst
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/doc/conf.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/doc/index.rst
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/doc/install.rst
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/doc/links.rst
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/doc/nitpick-exceptions.txt
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/doc/release.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/__init__.py
+-rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/click.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/logging.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/python.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/utils.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/gitlab/__init__.py
+-rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/gitlab/changelog.py
+-rw-r--r--   0        0        0    17000 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/gitlab/release.py
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/gitlab/runners.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/scripts/__init__.py
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/scripts/badges.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/scripts/changelog.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/scripts/cli.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/scripts/getpath.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/scripts/jobs.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/scripts/lasttag.py
+-rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/scripts/release.py
+-rw-r--r--   0        0        0     9059 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/scripts/runners.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/src/idiap_devtools/scripts/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/tests/test_devtools.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/.gitignore
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/README.md
+-rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 idiap_devtools-2.0.0/PKG-INFO
```

### Comparing `idiap-devtools-1.0.0/LICENSES/BSD-3-Clause.txt` & `idiap_devtools-2.0.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `idiap-devtools-1.0.0/PKG-INFO` & `idiap_devtools-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,56 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: idiap-devtools
-Version: 1.0.0
-Summary: This package contains a *pot-pourri* of various tools required to develop python packages at Idiap's GitLab infrastructure
-Author-email: Andre Anjos <andre.anjos@idiap.ch>
-License: BSD 3-Clause License
-Project-URL: documentation, https://idiap-devtools.readthedocs.io/en/v1.0.0/
+Version: 2.0.0
+Summary: A *pot-pourri* of various tools required to develop python packages at Idiap's GitLab infrastructure
+Project-URL: documentation, https://idiap-devtools.readthedocs.io/en/v2.0.0/
 Project-URL: homepage, https://pypi.org/project/idiap-devtools
 Project-URL: repository, https://gitlab.idiap.ch/software/idiap-devtools
 Project-URL: changelog, https://gitlab.idiap.ch/software/idiap-devtools/-/releases
+Author-email: Andre Anjos <andre.anjos@idiap.ch>
+License-Expression: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: qa
+Requires-Python: >=3.10
+Requires-Dist: click>=8
+Requires-Dist: gitpython
+Requires-Dist: packaging
+Requires-Dist: python-dateutil
+Requires-Dist: python-gitlab
+Requires-Dist: pytz
+Requires-Dist: tomli
+Requires-Dist: tomlkit
 Provides-Extra: doc
+Requires-Dist: auto-intersphinx; extra == 'doc'
+Requires-Dist: furo; extra == 'doc'
+Requires-Dist: sphinx; extra == 'doc'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'doc'
+Requires-Dist: sphinx-click; extra == 'doc'
+Requires-Dist: sphinx-copybutton; extra == 'doc'
+Requires-Dist: sphinx-inline-tabs; extra == 'doc'
+Provides-Extra: qa
+Requires-Dist: pre-commit; extra == 'qa'
 Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Description-Content-Type: text/markdown
 
 <!--
 Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 
 SPDX-License-Identifier: BSD-3-Clause
 -->
 
-[![latest-docs](https://img.shields.io/badge/docs-v1.0.0-orange.svg)](https://idiap-devtools.readthedocs.io/en/v1.0.0/)
-[![build](https://gitlab.idiap.ch/software/idiap-devtools/badges/v1.0.0/pipeline.svg)](https://gitlab.idiap.ch/software/idiap-devtools/commits/v1.0.0)
-[![coverage](https://gitlab.idiap.ch/software/idiap-devtools/badges/v1.0.0/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/idiap-devtools/v1.0.0/coverage/index.html)
+[![latest-docs](https://img.shields.io/badge/docs-v2.0.0-orange.svg)](https://idiap-devtools.readthedocs.io/en/v2.0.0/)
+[![build](https://gitlab.idiap.ch/software/idiap-devtools/badges/v2.0.0/pipeline.svg)](https://gitlab.idiap.ch/software/idiap-devtools/commits/v2.0.0)
+[![coverage](https://gitlab.idiap.ch/software/idiap-devtools/badges/v2.0.0/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/idiap-devtools/v2.0.0/coverage/index.html)
 [![repository](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/software/idiap-devtools)
 
 # Development Tools
 
 This package contains a set of small utilities to support development of Python
 packages through GitLab.  It is targetted for package development at Idiap.
```

### Comparing `idiap-devtools-1.0.0/README.md` & `idiap_devtools-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
 Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 
 SPDX-License-Identifier: BSD-3-Clause
 -->
 
-[![latest-docs](https://img.shields.io/badge/docs-v1.0.0-orange.svg)](https://idiap-devtools.readthedocs.io/en/v1.0.0/)
-[![build](https://gitlab.idiap.ch/software/idiap-devtools/badges/v1.0.0/pipeline.svg)](https://gitlab.idiap.ch/software/idiap-devtools/commits/v1.0.0)
-[![coverage](https://gitlab.idiap.ch/software/idiap-devtools/badges/v1.0.0/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/idiap-devtools/v1.0.0/coverage/index.html)
+[![latest-docs](https://img.shields.io/badge/docs-v2.0.0-orange.svg)](https://idiap-devtools.readthedocs.io/en/v2.0.0/)
+[![build](https://gitlab.idiap.ch/software/idiap-devtools/badges/v2.0.0/pipeline.svg)](https://gitlab.idiap.ch/software/idiap-devtools/commits/v2.0.0)
+[![coverage](https://gitlab.idiap.ch/software/idiap-devtools/badges/v2.0.0/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/idiap-devtools/v2.0.0/coverage/index.html)
 [![repository](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/software/idiap-devtools)
 
 # Development Tools
 
 This package contains a set of small utilities to support development of Python
 packages through GitLab.  It is targetted for package development at Idiap.
```

### Comparing `idiap-devtools-1.0.0/doc/api.rst` & `idiap_devtools-2.0.0/doc/api.rst`

 * *Files 17% similar despite different names*

```diff
@@ -13,19 +13,16 @@
 
 
 .. autosummary::
    :toctree: api
 
    idiap_devtools
    idiap_devtools.click
-   idiap_devtools.conda
    idiap_devtools.logging
-   idiap_devtools.profile
    idiap_devtools.python
-   idiap_devtools.update_pins
    idiap_devtools.utils
 
 .. autosummary::
    :toctree: api/gitlab
 
    idiap_devtools.gitlab
    idiap_devtools.gitlab.changelog
```

### Comparing `idiap-devtools-1.0.0/doc/catalog.json` & `idiap_devtools-2.0.0/doc/catalog.json`

 * *Files identical despite different names*

### Comparing `idiap-devtools-1.0.0/doc/index.rst` & `idiap_devtools-2.0.0/doc/index.rst`

 * *Files 26% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 ===================
  Development Tools
 ===================
 
 .. todolist::
 
 This package contains a set of small utilities to support development of Python
-packages through GitLab.  It is targetted for package development at Idiap.
+packages through GitLab.  It is targetted for package development at Idiap,
+however some of the commands provided can benefit a larger audience.
 
 
 Documentation
 -------------
 
 .. toctree::
    :maxdepth: 2
 
    install
-   develop
    release
    cli
    api
 
 
 Indices and tables
 ------------------
```

### Comparing `idiap-devtools-1.0.0/doc/links.rst` & `idiap_devtools-2.0.0/doc/links.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 .. Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 ..
 .. SPDX-License-Identifier: BSD-3-Clause
 
 .. place re-used URLs here, then include this file
 .. on your other RST sources.
 
-.. _conda: https://conda.io
 .. _idiap: http://www.idiap.ch
 .. _python: http://www.python.org
-.. _mamba: https://mamba.readthedocs.io/en/latest/index.html
-.. _mambaforge: https://github.com/conda-forge/miniforge#mambaforge
-.. _conda-forge: https://conda-forge.org
+.. _pip: https://pip.pypa.io/en/stable/
+.. _uv: https://github.com/astral-sh/uv
+.. _rye: https://github.com/astral-sh/rye
+.. _poetry: https://python-poetry.org
+.. _pixi: https://pixi.sh
 .. _venv: https://docs.python.org/3/library/venv.html
 .. _virtualenv: https://virtualenv.pypa.io/en/latest/
 .. _gitlab-token: https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html
-.. _cookiecutter: https://cookiecutter.readthedocs.io
-.. _cookiecutter-template: https://gitlab.idiap.ch/software/cookiecutter-idiap-pypackage
 .. _semantic version numbers: https://semver.org
-
-.. _pip: https://pip.pypa.io/en/stable/
-.. _pip-e: https://pip.pypa.io/en/stable/cli/pip_install/#cmdoption-e
-.. _pip-config: https://pip.pypa.io/en/stable/topics/configuration/
```

### Comparing `idiap-devtools-1.0.0/doc/release.rst` & `idiap_devtools-2.0.0/doc/release.rst`

 * *Files 7% similar despite different names*

```diff
@@ -25,17 +25,15 @@
 
 Use the ``--help`` flag in each command to learn more about each phase.
 
 .. warning::
 
    Pipelines for stable and non-stable (a.k.a. beta) packages may differ w.r.t.
    deployment locations for various artefacts (e.g. packages and
-   documentation), but also w.r.t. requirements for the version of the profile
-   to be used (e.g. tagged versions non-tagged).  You should check the target
-   development profile CI instructions for details.
+   documentation).
 
 
 Create the Changelogs
 =====================
 
 Use the subcommand ``devtool gitlab changelog <group>/<package>`` to generate a
 changelog.  Follow examples and instructions at :ref:`idiap-devtools.cli`.
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/click.py` & `idiap_devtools-2.0.0/src/idiap_devtools/click.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
 import logging
 import typing
 
 import click
 
-from .profile import get_profile_path
-
 
 def verbosity_option(
     logger: logging.Logger,
     short_name: str = "v",
     name: str = "verbose",
     dflt: int = 0,
     **kwargs: typing.Any,
@@ -54,16 +50,16 @@
 
         dlft: The default verbosity level to use (defaults to 0).
 
         **kwargs: Further keyword-arguments to be forwarded to the underlying
             :py:func:`click.option`
 
 
-    Returns:
-
+    Returns
+    -------
         A callable, that follows the :py:mod:`click`-framework policy for
         option decorators.  Use it accordingly.
     """
 
     def custom_verbosity_option(f):
         def callback(ctx, param, value):
             ctx.meta[name] = value
@@ -71,17 +67,15 @@
                 0: logging.ERROR,
                 1: logging.WARNING,
                 2: logging.INFO,
                 3: logging.DEBUG,
             }[value]
 
             logger.setLevel(log_level)
-            logger.debug(
-                f'Level of Logger("{logger.name}") was set to {log_level}'
-            )
+            logger.debug(f'Level of Logger("{logger.name}") was set to {log_level}')
             return value
 
         return click.option(
             f"-{short_name}",
             f"--{name}",
             count=True,
             type=click.IntRange(min=0, max=3, clamp=True),
@@ -103,46 +97,50 @@
 
 class AliasedGroup(click.Group):
     """Class that handles prefix aliasing for commands."""
 
     def get_command(  # type: ignore
         self, ctx: click.core.Context, cmd_name: str
     ) -> click.Command | None:
-        """Returns the decorated command.
+        """Return the decorated command.
 
         Arguments:
 
             ctx: The current command context being parsed
 
             cmd_name: The subcommand name that was called
 
 
-        Returns:
-
+        Returns
+        -------
             The decorated command with aliasing capabilities
         """
 
         rv = click.Group.get_command(self, ctx, cmd_name)
         if rv is not None:
             return rv
+
         matches = [x for x in self.list_commands(ctx) if x.startswith(cmd_name)]
+
         if not matches:
             return None
-        elif len(matches) == 1:
+
+        if len(matches) == 1:
             return click.Group.get_command(self, ctx, matches[0])
-        ctx.fail("Too many matches: %s" % ", ".join(sorted(matches)))
+
+        ctx.fail("Too many matches: %s" % ", ".join(sorted(matches)))  # noqa
 
 
 class PreserveIndentCommand(click.Command):
     """A click command that preserves text indentation."""
 
     def format_epilog(
         self, _: click.core.Context, formatter: click.formatting.HelpFormatter
     ) -> None:
-        """Formats the command epilog during --help.
+        """Format the command epilog during --help.
 
         Arguments:
 
             _: The current parsing context
 
             formatter: The formatter to use for printing text
         """
@@ -151,54 +149,20 @@
             formatter.write_paragraph()
             for line in self.epilog.split("\n"):
                 formatter.write_text(line)
 
     def format_description(
         self, _: click.core.Context, formatter: click.formatting.HelpFormatter
     ) -> None:
-        """Formats the command description during --help.
+        """Format the command description during --help.
 
         Arguments:
 
             _: The current parsing context
 
             formatter: The formatter to use for printing text
         """
 
         if self.description:
             formatter.write_paragraph()
             for line in self.description.split("\n"):
                 formatter.write_text(line)
-
-
-def validate_profile(_: click.Context, __: str, value: str) -> str:
-    """Callback for click doing a profile name validation.
-
-    Arguments:
-
-        _: current command context
-
-        __: The option being validated
-
-        value: The value set for the option
-
-
-    Returns:
-
-        The validated option value
-    """
-    profile_path = get_profile_path(value)
-    if profile_path is None:
-        raise click.BadParameter(
-            "You have not provided a development profile path "
-            "(-P/--profile) option or set the `default' profile at "
-            "your configuration file.  I need one of these to "
-            "load my development constants"
-        )
-
-    if not (profile_path / "profile.toml").exists():
-        raise click.BadParameter(
-            f"Error while attempting to load the profile `{value}' from "
-            f"`{str(profile_path/'profile.toml')}' - file does not exist!"
-        )
-
-    return value
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/gitlab/__init__.py` & `idiap_devtools-2.0.0/src/idiap_devtools/gitlab/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
-
 """Utilities to interact with GitLab."""
 
-from __future__ import annotations
-
 import logging
 import os
 import pathlib
 import shutil
 import tarfile
 import tempfile
 
@@ -18,44 +15,44 @@
 import gitlab
 import gitlab.v4.objects
 
 logger = logging.getLogger(__name__)
 
 
 def get_gitlab_instance() -> gitlab.Gitlab:
-    """Returns an instance of the gitlab object for remote operations."""
+    """Return an instance of the gitlab object for remote operations."""
     # tries to figure if we can authenticate using a global configuration
-    cfgs = ["~/.python-gitlab.cfg", "/etc/python-gitlab.cfg"]
-    cfgs = [os.path.expanduser(k) for k in cfgs]
-    if any([os.path.exists(k) for k in cfgs]):
-        gl = gitlab.Gitlab.from_config(
-            "idiap", [k for k in cfgs if os.path.exists(k)]
-        )
+    cfgs = [
+        pathlib.Path(k).expanduser()
+        for k in ["~/.python-gitlab.cfg", "/etc/python-gitlab.cfg"]
+    ]
+    if any([k.exists() for k in cfgs]):
+        gl = gitlab.Gitlab.from_config("idiap", [str(k) for k in cfgs if k.exists()])
     else:  # ask the user for a token or use one from the current runner
         server = os.environ.get("CI_SERVER_URL", "https://gitlab.idiap.ch")
         token = os.environ.get("CI_JOB_TOKEN")
         if token is None:
             logger.debug(
                 "Did not find any of %s nor CI_JOB_TOKEN is defined. "
                 "Asking for user token on the command line...",
-                "|".join(cfgs),
+                "|".join([str(k) for k in cfgs]),
             )
             token = input(f"{server} (private) token: ")
         gl = gitlab.Gitlab(server, private_token=token, api_version="4")
 
     return gl
 
 
 def download_path(
     package: gitlab.v4.objects.projects.Project,
     path: str,
     output: pathlib.Path | None = None,
     ref: str | None = None,
 ) -> None:
-    """Downloads paths from gitlab, with an optional recurse.
+    """Download paths from gitlab, with an optional recurse.
 
     This method will download an archive of the repository from chosen
     reference, and then it will search inside the zip blob for the path to be
     copied into output.  It uses :py:class:`zipfile.ZipFile` to do this search.
     This method will not be very efficient for larger repository references,
     but works recursively by default.
 
@@ -87,8 +84,8 @@
 
     with tempfile.TemporaryDirectory() as d:
         with tarfile.open(fileobj=BytesIO(archive), mode="r:gz") as f:
             f.extractall(path=d)
 
         # move stuff to "output"
         basedir = os.listdir(d)[0]
-        shutil.move(os.path.join(d, basedir, path), output)
+        shutil.move(pathlib.Path(d) / basedir / path, output)
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/gitlab/changelog.py` & `idiap_devtools-2.0.0/src/idiap_devtools/gitlab/changelog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
-
 """Utilities for retrieving, parsing and auto-generating changelogs."""
 
-from __future__ import annotations
-
 import datetime
 import io
 import logging
 import textwrap
 import typing
 
 import dateutil.parser
@@ -17,183 +14,174 @@
 import gitlab.v4.objects
 import pytz
 
 logger = logging.getLogger(__name__)
 
 
 def parse_date(s: typing.TextIO | str) -> datetime.datetime:
-    """Parses any date supported by :py:meth:`dateutil.parser.parse`
+    """Parse any date supported by :py:meth:`dateutil.parser.parse`.
 
     Automatically applies the "Europe/Zurich" timezone
 
 
     Arguments:
 
         s: The input readable stream or string to be parsed into a date
 
 
-    Returns:
-
+    Returns
+    -------
         A :py:class:`datetime.datetime`.
     """
     return dateutil.parser.parse(s, ignoretz=True).replace(
         tzinfo=pytz.timezone("Europe/Zurich")
     )
 
 
 def _sort_commits(
     commits: typing.Iterable[gitlab.v4.objects.commits.ProjectCommit],
     reverse: bool,
 ) -> list[typing.Any]:
-    """Sorts gitlab commit objects using their ``committed_date`` attribute.
+    """Sort gitlab commit objects using their ``committed_date`` attribute.
 
     Arguments:
 
         commits: A list of commits to process
 
         reverse: Indicates if the sorting should be reversed
 
 
-    Returns:
-
+    Returns
+    -------
         The input list of ``commits``, sorted
     """
 
-    return sorted(
-        commits, key=lambda x: parse_date(x.committed_date), reverse=reverse
-    )
+    return sorted(commits, key=lambda x: parse_date(x.committed_date), reverse=reverse)
 
 
 def _sort_tags(
     tags: typing.Iterable[gitlab.v4.objects.tags.ProjectTag], reverse: bool
 ) -> list[typing.Any]:
-    """Sorts gitlab tags objects using their ``committed_date`` attribute.
+    """Sort gitlab tags objects using their ``committed_date`` attribute.
 
     Arguments:
 
         tags: A list of tags to process
 
         reverse: Indicates if the sorting should be reversed
 
 
-    Returns:
-
+    Returns
+    -------
         The input list of ``tags``, sorted
     """
 
     return sorted(
         tags,
         key=lambda x: parse_date(x.commit["committed_date"]),
         reverse=reverse,
     )
 
 
 def get_file_from_gitlab(
     gitpkg: gitlab.v4.objects.projects.Project, path: str, ref: str = "main"
 ) -> io.StringIO:
-    """Retrieves a file from a Gitlab repository.
+    """Retrieve a file from a Gitlab repository.
 
     Arguments:
 
         gitpkg: The gitlab project to fetch the datafile from
 
         path: The internal path to the file to retrieve
 
         ref: Branch, commit or reference to get file from, at GitLab
 
 
-    Returns:
-
+    Returns
+    -------
         A string I/O object you can use like a file.
     """
 
     return io.StringIO(gitpkg.files.get(file_path=path, ref=ref).encode())
 
 
 def get_last_tag_date(
     package: gitlab.v4.objects.projects.Project,
 ) -> datetime.datetime:
-    """Returns the last release date for the given package.
+    """Return the last release date for the given package.
 
     Falls back to the first commit date if the package has not yet been tagged
 
 
     Arguments:
 
         package: The gitlab project object from where to fetch the last release
                  date information
 
 
-    Returns:
-
+    Returns
+    -------
         A :py:class:`datetime.datetime` object that refers to the last date the
         package was released.  If the package was never released, then returns
         the date just before the first commit.
 
 
-    Raises:
-
+    Raises
+    ------
         RuntimeError: if the project has no commits.
     """
 
     # according to the Gitlab API documentation, tags are sorted from the last
     # updated to the first, by default - no need to do further sorting!
-    tag_list = package.tags.list(
-        page=1, per_page=1
-    )  # Silence userWarning on list()
+    tag_list = package.tags.list(page=1, per_page=1)  # Silence userWarning on list()
 
     if tag_list:
         # there are tags, use these
         last = tag_list[0]
         logger.debug(
             "Last tag for package %s (id=%d) is %s",
             package.name,
             package.id,
             last.name,
         )
         return parse_date(last.commit["committed_date"]) + datetime.timedelta(
             milliseconds=500
         )
 
-    else:
-        commit_list = package.commits.list(all=True)
+    commit_list = package.commits.list(all=True)
 
-        if commit_list:
-            # there are commits, use these
-            first = _sort_commits(commit_list, reverse=False)[0]
-            logger.debug(
-                "First commit for package %s (id=%d) is from %s",
-                package.name,
-                package.id,
-                first.committed_date,
-            )
-            return parse_date(first.committed_date) - datetime.timedelta(
-                milliseconds=500
-            )
+    if commit_list:
+        # there are commits, use these
+        first = _sort_commits(commit_list, reverse=False)[0]
+        logger.debug(
+            "First commit for package %s (id=%d) is from %s",
+            package.name,
+            package.id,
+            first.committed_date,
+        )
+        return parse_date(first.committed_date) - datetime.timedelta(milliseconds=500)
 
-        else:
-            # there are no commits nor tags - abort
-            raise RuntimeError(
-                "package %s (id=%d) does not have commits "
-                "or tags so I cannot devise a good starting date"
-                % (package.name, package.id)
-            )
+    # there are no commits nor tags - abort
+    raise RuntimeError(
+        "package %s (id=%d) does not have commits "
+        "or tags so I cannot devise a good starting date" % (package.name, package.id)
+    )
 
 
 def _get_tag_changelog(tag: gitlab.v4.objects.tags.ProjectTag) -> str:
     try:
         return tag.release["description"]
     except Exception:
         return ""
 
 
 def _write_one_tag(
     f: typing.TextIO, pkg_name: str, tag: gitlab.v4.objects.tags.ProjectTag
 ) -> None:
-    """Prints commit information for a single tag of a given package.
+    """Print commit information for a single tag of a given package.
 
     Arguments:
 
         f: open text stream, ready to be written at
 
         pkg_name: The name of the package we are writing tags of
 
@@ -205,32 +193,29 @@
     f.write(f"  - {tag.name} ({git_date:%b %d, %Y %H:%M}){newline}{newline}")
 
     for line in _get_tag_changelog(tag).replace("\r\n", "\n").split("\n"):
         line = line.strip()
         if line.startswith("* ") or line.startswith("- "):
             line = line[2:]
 
-        line = line.replace("!", pkg_name + "!").replace(
-            pkg_name + pkg_name, pkg_name
-        )
+        line = line.replace("!", pkg_name + "!").replace(pkg_name + pkg_name, pkg_name)
         line = line.replace("#", pkg_name + "#")
         if not line:
             continue
         f.write(f"    - {line}{newline}")
 
     f.write(f"{newline}")
 
 
 def _write_commits_range(
     f: typing.TextIO,
     pkg_name: str,
     commits: typing.Iterable[gitlab.v4.objects.commits.ProjectCommit],
 ) -> None:
-    """Writes all commits of a given package within a range, to the output
-    file.
+    """Write all commits of a given package within a range, to the output file.
 
     Arguments:
 
         f: open text stream, ready to be written at
 
         pkg_name: The name of the package we are writing tags of
 
@@ -261,16 +246,15 @@
 
 
 def _write_mergerequests_range(
     f: typing.TextIO,
     pkg_name: str,
     mrs: typing.Iterable[gitlab.v4.objects.merge_requests.ProjectMergeRequest],
 ) -> None:
-    """Writes all merge-requests of a given package, with a range, to the
-    output file.
+    """Write all merge-requests of a given package, with a range, to the output file.
 
     Arguments:
 
         f: A :py:class:`File` ready to be written at
 
         pkg_name: The name of the package we are writing tags of
 
@@ -301,25 +285,25 @@
 def get_changes_since(
     gitpkg: gitlab.v4.objects.projects.Project, since: datetime.datetime
 ) -> tuple[
     list[gitlab.v4.objects.merge_requests.ProjectMergeRequest],
     list[gitlab.v4.objects.tags.ProjectTag],
     list[gitlab.v4.objects.commits.ProjectCommit],
 ]:
-    """Gets the list of MRs, tags, and commits since the provided date.
+    """Get the list of MRs, tags, and commits since the provided date.
 
     Arguments:
 
         gitpkg : A gitlab package object
 
         since : a date and time to start looking changes from
 
 
-    Returns:
-
+    Returns
+    -------
         A list of merge requests, tags and commits for the given package, since
         the determined date.
     """
 
     # get tags since release and sort them
     tags = gitpkg.tags.list(all=True)
 
@@ -350,15 +334,15 @@
 
 def write_tags_with_commits(
     f: typing.TextIO,
     gitpkg: gitlab.v4.objects.projects.Project,
     since: datetime.datetime,
     mode: str,
 ) -> None:
-    """Writes all tags and commits of a given package to the output file.
+    """Write all tags and commits of a given package to the output file.
 
     Arguments:
 
         f: A stream ready to be written at
 
         gitpkg: A pointer to the gitlab package object
 
@@ -367,18 +351,15 @@
         mode: One of ``mrs`` (merge-requests), ``commits`` or ``tags``
             indicating how to list entries in the changelog for this package
     """
 
     mrs, tags, commits = get_changes_since(gitpkg, since)
     newline = "\n"
 
-    f.write(
-        f"# {gitpkg.attributes['path_with_namespace']}:"
-        f" patch{newline}{newline}"
-    )
+    f.write(f"# {gitpkg.attributes['path_with_namespace']}: patch{newline}{newline}")
 
     # go through tags and writes each with its message and corresponding
     # commits
     start_date = since
     for tag in tags:
         # write tag name and its text
         _write_one_tag(f, gitpkg.attributes["path_with_namespace"], tag)
@@ -396,32 +377,28 @@
             )
 
         elif mode == "mrs":
             # write merge requests from the previous tag up to this one
             # the attribute 'merged_at' is not available in GitLab API as of 27
             # June 2018
             mrs4tag = [
-                k
-                for k in mrs
-                if (start_date < parse_date(k.updated_at) <= end_date)
+                k for k in mrs if (start_date < parse_date(k.updated_at) <= end_date)
             ]
             _write_mergerequests_range(
                 f, gitpkg.attributes["path_with_namespace"], mrs4tag
             )
 
         start_date = end_date
 
     if mode != "tags":
         if mode == "mrs":
             # write leftover merge requests
             # the attribute 'merged_at' is not available in GitLab API as of 27
             # June 2018
-            leftover_mrs = [
-                k for k in mrs if parse_date(k.updated_at) > start_date
-            ]
+            leftover_mrs = [k for k in mrs if parse_date(k.updated_at) > start_date]
             _write_mergerequests_range(
                 f, gitpkg.attributes["path_with_namespace"], leftover_mrs
             )
 
         else:
             # write leftover commits that were not tagged yet
             leftover_commits = [
@@ -433,15 +410,15 @@
 
 
 def write_tags(
     f: typing.TextIO,
     gitpkg: gitlab.v4.objects.projects.Project,
     since: datetime.datetime,
 ) -> None:
-    """Writes all tags of a given package to the output file.
+    """Write all tags of a given package to the output file.
 
     Arguments:
 
         f: A stream ready to be written at
 
         gitpkg: A pointer to the gitlab package object
 
@@ -450,14 +427,11 @@
 
     tags = gitpkg.tags.list()
     # sort tags by date
     tags = [k for k in tags if parse_date(k.commit["committed_date"]) >= since]
     tags = _sort_tags(tags, reverse=False)
 
     newline = "\n"
-    f.write(
-        f"# {gitpkg.attributes['path_with_namespace']}:"
-        f" patch{newline}{newline}"
-    )
+    f.write(f"# {gitpkg.attributes['path_with_namespace']}: patch{newline}{newline}")
 
     for tag in tags:
         _write_one_tag(f, gitpkg.attributes["path_with_namespace"], tag)
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/gitlab/runners.py` & `idiap_devtools-2.0.0/src/idiap_devtools/gitlab/runners.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,81 +1,75 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
 import logging
 import pathlib
 import typing
 
 import gitlab
 import gitlab.v4.objects
 
 logger = logging.getLogger(__name__)
 
 
 def get_runner_from_description(
     gl: gitlab.Gitlab, descr: str
 ) -> gitlab.v4.objects.runners.Runner:
-    """Retrieves a runner object matching the description, or raises.
+    """Retrieve a runner object matching the description, or raises.
 
     Arguments:
 
         gl: gitlab service instance
 
         descr: the runner description
 
 
-    Returns:
-
+    Returns
+    -------
         The runner object, if one is found matching the description
 
 
-    Raises:
-
+    Raises
+    ------
         RuntimeError: if no runner matching the description is found.
     """
 
     # search for the runner to affect
     runners = [
-        k
-        for k in gl.runners.list(all=True)
-        if k.attributes["description"] == descr
+        k for k in gl.runners.list(all=True) if k.attributes["description"] == descr
     ]
     if not runners:
         raise RuntimeError("Cannot find runner with description = %s", descr)
     the_runner = typing.cast(gitlab.v4.objects.runners.Runner, runners[0])
     logger.info(
         "Found runner %s (id=%d)",
         the_runner.attributes["description"],
         the_runner.attributes["id"],
     )
 
     return the_runner
 
 
-def get_project(
-    gl: gitlab.Gitlab, name: str
-) -> gitlab.v4.objects.projects.Project:
-    """Retrieves one single project."""
+def get_project(gl: gitlab.Gitlab, name: str) -> gitlab.v4.objects.projects.Project:
+    """Retrieve one single project."""
 
     retval = gl.projects.get(name)
     logger.debug(
         "Found gitlab project %s (id=%d)",
         retval.attributes["path_with_namespace"],
         retval.id,
     )
     return retval
 
 
 def get_projects_from_group(
     gl: gitlab.Gitlab, name: str
 ) -> list[gitlab.v4.objects.projects.Project]:
-    """Returns a list with all projects in a GitLab group."""
+    """Return a list with all projects in a GitLab group."""
 
     group = gl.groups.get(name)
     logger.debug(
         "Found gitlab group %s (id=%d)",
         group.attributes["path"],
         group.id,
     )
@@ -93,37 +87,35 @@
         logger.debug("Got data from project %d/%d", k + 1, len(projects))
     return packages
 
 
 def get_projects_from_runner(
     gl: gitlab.Gitlab, runner: gitlab.v4.objects.runners.Runner
 ) -> list[gitlab.v4.objects.projects.Project]:
-    """Retrieves a list of all projects that include a particular runner."""
+    """Retrieve a list of all projects that include a particular runner."""
 
     the_runner = gl.runners.get(runner.id)
     logger.info(
         "Retrieving details for %d projects using runner %s (id=%d). "
         "This may take a while...",
         len(the_runner.projects),
         the_runner.description,
         the_runner.id,
     )
     packages = []
     for k, proj in enumerate(the_runner.projects):
         packages.append(get_project(gl, proj["id"]))
-        logger.debug(
-            "Got data from project %d/%d", k + 1, len(the_runner.projects)
-        )
+        logger.debug("Got data from project %d/%d", k + 1, len(the_runner.projects))
     return packages
 
 
 def get_projects_from_file(
     gl: gitlab.Gitlab, filename: pathlib.Path
 ) -> list[gitlab.v4.objects.projects.Project]:
-    """Retrieves a list of projects based on lines of a file."""
+    """Retrieve a list of projects based on lines of a file."""
 
     packages = []
     with filename.open("rt") as f:
         lines = [k.strip() for k in f.readlines()]
         lines = [k for k in lines if k and not k.startswith("#")]
         logger.info("Loaded %d entries from file %s", len(lines), filename)
         for k, proj in enumerate(lines):
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/logging.py` & `idiap_devtools-2.0.0/src/idiap_devtools/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
-
-""":py:class:`logging.Logger` setup and stream separation"""
+""":py:class:`logging.Logger` setup and stream separation."""
 
 import logging
 import sys
 import typing
 
 
 # debug and info messages are written to sys.stdout
@@ -20,19 +19,19 @@
 
     def filter(self, record):
         return record.levelno <= logging.INFO
 
 
 def setup(
     logger_name: str,
-    format: str = "[%(levelname)s][%(name)s][%(asctime)s] %(message)s",
+    format_: str = "[%(levelname)s][%(name)s][%(asctime)s] %(message)s",
     low_level_stream: typing.TextIO = sys.stdout,
     high_level_stream: typing.TextIO = sys.stderr,
 ) -> logging.Logger:
-    """This function returns a logger object that is ready for console logging.
+    """Return a logger object that is ready for console logging.
 
     Retrieves (as with :py:func:`logging.getLogger()`) the given logger, and
     then attaches 2 handlers (defined on the module) to it:
 
     1. A :py:class:`logging.StreamHandler` to output messages with level equal
        or lower than ``logging.INFO`` to the text-I/O stream
        ``low_level_stream``.  This is implemented by attaching a filter to the
@@ -47,57 +46,55 @@
     is sent to the right stream.
 
 
     Arguments:
 
         logger_name: The name of the module to generate logs for
 
-        format: The format of the logs, see :py:class:`logging.LogRecord` for
+        format_: The format of the logs, see :py:class:`logging.LogRecord` for
             more details. By default, the log contains the logger name, the log
             time, the log level and the massage.
 
         low_level_stream: The stream where to output info messages and below
 
         high_level_stream: The stream where to output warning messages and
             above
 
 
-    Returns:
-
+    Returns
+    -------
         The configured logger. The same logger can be retrieved using the
         :py:func:`logging.getLogger` function.
     """
 
     logger = logging.getLogger(logger_name)
 
-    formatter = logging.Formatter(format)
+    formatter = logging.Formatter(format_)
 
     handlers_installed = {k.name: k for k in logger.handlers}
     debug_logger_name = f"debug_info+{logger_name}"
 
     # First check that logger with a matching name or stream is not already
     # there before attaching a new one.
     if (debug_logger_name not in handlers_installed) or (
-        getattr(handlers_installed[debug_logger_name], "stream")
-        != low_level_stream
+        getattr(handlers_installed[debug_logger_name], "stream") != low_level_stream
     ):
         debug_info = logging.StreamHandler(low_level_stream)
         debug_info.setLevel(logging.DEBUG)
         debug_info.setFormatter(formatter)
         debug_info.addFilter(_InfoFilter())
         debug_info.name = debug_logger_name
         logger.addHandler(debug_info)
 
     error_logger_name = f"warn_err+{logger_name}"
 
     # First check that logger with a matching name or stream is not already
     # there before attaching a new one.
     if (error_logger_name not in handlers_installed) or (
-        getattr(handlers_installed[error_logger_name], "stream")
-        != high_level_stream
+        getattr(handlers_installed[error_logger_name], "stream") != high_level_stream
     ):
         warn_err = logging.StreamHandler(high_level_stream)
         warn_err.setLevel(logging.WARNING)
         warn_err.setFormatter(formatter)
         warn_err.name = error_logger_name
         logger.addHandler(warn_err)
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/python.py` & `idiap_devtools-2.0.0/src/idiap_devtools/python.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
+import pathlib
 
-import pkg_resources
+import packaging.requirements
 import tomli
 
 
 def dependencies_from_pyproject_toml(
-    path: str,
-) -> tuple[str, list[pkg_resources.Requirement]]:
-    """Returns a list with all ``project.optional-dependencies``
+    path: pathlib.Path,
+) -> tuple[str, list[packaging.requirements.Requirement]]:
+    """Return a list with all ``project.optional-dependencies``.
 
     Arguments:
 
         path: The path to a ``pyproject.toml`` file to load
 
 
-    Returns:
-
+    Returns
+    -------
         A list of optional dependencies (if any exist) on the provided python
         project.
     """
 
-    data = tomli.load(open(path, "rb"))
+    data = tomli.load(path.open("rb"))
 
     deps = data.get("project", {}).get("dependencies", [])
     optional_deps = data.get("project", {}).get("optional-dependencies", {})
 
-    retval = list(pkg_resources.parse_requirements(deps))
+    retval = [packaging.requirements.Requirement(k) for k in deps]
     for v in optional_deps.values():
-        retval += list(pkg_resources.parse_requirements(v))
+        retval += [packaging.requirements.Requirement(k) for k in v]
 
     return data.get("project", {}).get("name", "UNKNOWN"), retval
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/__init__.py` & `idiap_devtools-2.0.0/src/idiap_devtools/scripts/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
 import click
 
-from ...click import AliasedGroup
-from ...logging import setup
+from ..click import AliasedGroup
+from ..logging import setup
 from .badges import badges
 from .changelog import changelog
 from .getpath import getpath
 from .jobs import jobs
 from .lasttag import lasttag
 from .release import release
 from .runners import runners
 from .settings import settings
 
 logger = setup(__name__.split(".", 1)[0])
 
 
-@click.group(cls=AliasedGroup)
-def gitlab() -> None:
+@click.group(
+    cls=AliasedGroup,
+    context_settings=dict(help_option_names=["-?", "-h", "--help"]),
+)
+@click.version_option()
+def cli() -> None:
     """Commands that interact directly with GitLab.
 
     Commands defined here are supposed to interact with gitlab, and
-    add/modify/remove resources on it directly.  To avoid repetitive asking,
-    create a configuration file as indicated in the
-    :ref:`idiap-devtools.install.setup.gitlab` section of the user guide.
+    add/modify/remove resources on it directly.
+
+    To avoid repetitive asking, create a configuration file as indicated
+    at :ref:`idiap-devtools.install.setup.gitlab` section of the user
+    guide.
     """
     pass
 
 
-gitlab.add_command(changelog)
-gitlab.add_command(release)
-gitlab.add_command(badges)
-gitlab.add_command(runners)
-gitlab.add_command(jobs)
-gitlab.add_command(getpath)
-gitlab.add_command(lasttag)
-gitlab.add_command(settings)
+cli.add_command(changelog)
+cli.add_command(release)
+cli.add_command(badges)
+cli.add_command(runners)
+cli.add_command(jobs)
+cli.add_command(getpath)
+cli.add_command(lasttag)
+cli.add_command(settings)
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/badges.py` & `idiap_devtools-2.0.0/src/idiap_devtools/scripts/badges.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
 import click
 
-from ...click import PreserveIndentCommand, verbosity_option
-from ...logging import setup
+from ..click import PreserveIndentCommand, verbosity_option
+from ..logging import setup
 
 logger = setup(__name__.split(".", 1)[0])
 
 
 # These show on the gitlab project landing page (not visible on PyPI)
 PROJECT_BADGES = [
     {
@@ -69,23 +67,21 @@
         "link_url": "https://gitlab.idiap.ch/{group}/{name}",
         "image_url": "https://img.shields.io/badge/gitlab-project-0000c0.svg",
     },
 ]
 
 
 def _update_readme(content, info):
-    """Updates the README content provided, replacing badges."""
+    """Update the README content provided, replacing badges."""
     import re
 
     new_badges_text = []
     for badge in README_BADGES:
         data = {k: v.format(**info) for (k, v) in badge.items()}
-        new_badges_text.append(
-            "[![{name}]({image_url})]({link_url})".format(**data)
-        )
+        new_badges_text.append("[![{name}]({image_url})]({link_url})".format(**data))
     new_badges_text = "\n" + "\n".join(new_badges_text) + "\n"
     # matches only 3 or more occurences of markdown badges
     expression = r"(\s?\[\!\[(?P<name>(\s|\w|-)+)\]\((?P<image_url>\S+)\)\]\((?P<link_url>\S+)\)){3,}"
     return re.sub(expression, new_badges_text, content)
 
 
 @click.command(
@@ -121,27 +117,26 @@
 @click.option(
     "-s",
     "--server",
     help="The documentation server. Default value is https://www.idiap.ch/software/{group}",
 )
 @verbosity_option(logger=logger)
 def badges(package, update_readme, dry_run, server, **_) -> None:
-    """Creates stock badges for a project repository."""
+    """Create stock badges for a project repository."""
+
     import typing
 
     import gitlab
 
-    from ...gitlab import get_gitlab_instance
-    from ...gitlab.release import update_files_at_default_branch
+    from ..gitlab import get_gitlab_instance
+    from ..gitlab.release import update_files_at_default_branch
 
     if dry_run:
         click.secho("!!!! DRY RUN MODE !!!!", fg="yellow", bold=True)
-        click.secho(
-            "No changes will be committed to GitLab.", fg="yellow", bold=True
-        )
+        click.secho("No changes will be committed to GitLab.", fg="yellow", bold=True)
 
     if "/" not in package:
         raise RuntimeError('PACKAGE should be specified as "group/name"')
 
     gl = get_gitlab_instance()
 
     # we lookup the gitlab package once
@@ -200,13 +195,13 @@
             )
             if dry_run:
                 click.echo("(dry-run) contents of new README.md:\n")
                 click.echo(readme_content)
         logger.info("All done.")
 
     except gitlab.GitlabGetError:
-        logger.warn(
+        logger.warning(
             "Gitlab access error - package %s does not exist?",
             package,
             exc_info=True,
         )
         click.secho(f"{package}: unknown", bold=True)
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/changelog.py` & `idiap_devtools-2.0.0/src/idiap_devtools/scripts/changelog.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
 import sys
 
 import click
 
-from ...click import PreserveIndentCommand, verbosity_option
-from ...logging import setup
+from ..click import PreserveIndentCommand, verbosity_option
+from ..logging import setup
 
 logger = setup(__name__.split(".", 1)[0])
 
 
 @click.command(
     cls=PreserveIndentCommand,
     epilog="""
@@ -84,54 +82,48 @@
     help="A starting date in any format accepted by dateutil.parser.parse() "
     "(see https://dateutil.readthedocs.io/en/stable/parser.html) from "
     "which you want to generate the changelog.  If not set, the package's"
     "last release date will be used",
 )
 @verbosity_option(logger=logger)
 def changelog(target, output, mode, since, **_) -> None:
-    """Generates changelog file for package(s) from the Gitlab server.
+    """Generate changelog file for package(s) from the Gitlab server.
 
-    This script generates changelogs for either a single package or
-    multiple
-    packages, depending on the value of TARGET.  The changelog (in
-    markdown
+    This script generates changelogs for either a single package or multiple
+    packages, depending on the value of TARGET.  The changelog (in markdown
     format) is written to the output file CHANGELOG.
 
-    There are two modes of operation: you may provide the package name
-    in the
+    There are two modes of operation: you may provide the package name in the
     format ``<gitlab-group>/<package-name>``. Or, optionally, provide an
-    existing file containing a list of packages that will be iterated
-    on.
+    existing file containing a list of packages that will be iterated on.
 
-    For each package, we will contact the Gitlab server and create a
-    changelog
-    using merge-requests (default), tags or commits since a given date.
-    If a
-    starting date is not passed, we'll use the date of the last tagged
-    value or
-    the date of the first commit, if no tags are available in the
-    package.
+    For each package, we will contact the Gitlab server and create a changelog
+    using merge-requests (default), tags or commits since a given date. If a
+    starting date is not passed, we'll use the date of the last tagged value or
+    the date of the first commit, if no tags are available in the package.
     """
+
     import datetime
-    import os
+    import pathlib
 
-    from ...gitlab import get_gitlab_instance
-    from ...gitlab.changelog import (
+    from ..gitlab import get_gitlab_instance
+    from ..gitlab.changelog import (
         get_last_tag_date,
         parse_date,
         write_tags_with_commits,
     )
 
     gl = get_gitlab_instance()
 
     # reads package list or considers name to be a package name
     for tgt in target:
-        if os.path.exists(tgt) and os.path.isfile(tgt):
+        tgt_path = pathlib.Path(tgt)
+        if tgt_path.exists() and tgt_path.is_file():
             logger.info(f"Reading package names from file {tgt}...")
-            with open(tgt) as f:
+            with tgt_path.open() as f:
                 packages = [
                     k.strip()
                     for k in f.readlines()
                     if k.strip() and not k.strip().startswith("#")
                 ]
         else:
             logger.info(f"Assuming {tgt} is a package name...")
@@ -142,16 +134,15 @@
         if since is not None:
             since_dt = parse_date(since)
 
         # iterates over the packages and dumps required information
         for package in packages:
             if "/" not in package:
                 raise RuntimeError(
-                    f"Package names must contain group name"
-                    f" (invalid: {package})"
+                    f"Package names must contain group name (invalid: {package})"
                 )
 
             # retrieves the gitlab package object
             use_package = gl.projects.get(package)
             logger.info(
                 "Found gitlab project %s (id=%d)",
                 use_package.attributes["path_with_namespace"],
@@ -183,12 +174,10 @@
                     'Skipping package %s (visibility not in "%s")...',
                     use_package.attributes["path_with_namespace"],
                     "|".join(visibility),
                 )
                 continue
 
             # write_tags(f, use_package, last_release_date)
-            write_tags_with_commits(
-                output, use_package, last_release_date, mode
-            )
+            write_tags_with_commits(output, use_package, last_release_date, mode)
 
     output.flush()
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/getpath.py` & `idiap_devtools-2.0.0/src/idiap_devtools/scripts/getpath.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
 import click
 
-from ...click import PreserveIndentCommand, verbosity_option
-from ...logging import setup
+from ..click import PreserveIndentCommand, verbosity_option
+from ..logging import setup
 
 logger = setup(__name__.split(".", 1)[0])
 
 
 @click.command(
     cls=PreserveIndentCommand,
     epilog="""
 Examples:
 
-  1. Get the file ``profile.toml`` from software/dev-profile's default branch:
-
-     .. code:: sh
-
-        devtool gitlab getpath software/dev-profile profile.toml
-
-
-  2. Get the directory ``gitlab`` (and eventual sub-directories) from
+  1. Get the directory ``gitlab`` (and eventual sub-directories) from
      software/dev-profile:
 
      .. code:: sh
 
-        devtool gitlab getpath software/dev-profile gitlab
+        devtool getpath software/dev-profile gitlab
 
 """,
 )
 @click.argument("package")
 @click.argument("path")
 @click.argument("output", type=click.Path(exists=False), required=False)
 @click.option(
@@ -41,20 +32,20 @@
     "--ref",
     help="Download path from the provided git reference (may be a branch, "
     "tag or commit hash).  If not set, then use the default package "
     "branch as reference to download.",
 )
 @verbosity_option(logger=logger)
 def getpath(package, path, output, ref, **_) -> None:
-    """Downloads files and directories from gitlab.
+    """Download files and directories from gitlab.
 
     Files are downloaded and stored.  Directories are recursed and fully
     downloaded to the client.
     """
-    from ...gitlab import download_path, get_gitlab_instance
+    from ..gitlab import download_path, get_gitlab_instance
 
     if "/" not in package:
         raise RuntimeError('PACKAGE should be specified as "group/name"')
 
     gl = get_gitlab_instance()
 
     # we lookup the gitlab package once
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/jobs.py` & `idiap_devtools-2.0.0/src/idiap_devtools/scripts/jobs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
 import click
 
-from ...click import PreserveIndentCommand, verbosity_option
-from ...logging import setup
+from ..click import PreserveIndentCommand, verbosity_option
+from ..logging import setup
 
 logger = setup(__name__.split(".", 1)[0])
 
 
 @click.command(
     cls=PreserveIndentCommand,
     epilog="""
@@ -47,16 +45,16 @@
     default="running",
     show_default=True,
     help='The status of jobs we are searching for - one of "running", '
     '"success", "failed" or "canceled"',
 )
 @verbosity_option(logger=logger)
 def jobs(status, tags, **_) -> None:
-    """Lists jobs on a given runner identified by description."""
-    from ...gitlab import get_gitlab_instance
+    """List jobs on a given runner identified by description."""
+    from ..gitlab import get_gitlab_instance
 
     gl = get_gitlab_instance()
 
     tags = tags or ["bob"]
 
     # search for the runner(s) to affect
     runners = gl.runners.list(tag_list=tags)
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/lasttag.py` & `idiap_devtools-2.0.0/src/idiap_devtools/scripts/lasttag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
 import click
 
-from ...click import PreserveIndentCommand, verbosity_option
-from ...logging import setup
+from ..click import PreserveIndentCommand, verbosity_option
+from ..logging import setup
 
 logger = setup(__name__.split(".", 1)[0])
 
 
 @click.command(
     cls=PreserveIndentCommand,
     epilog="""
@@ -31,19 +29,19 @@
         devtool gitlab lasttag beat/beat.core
 
 """,
 )
 @click.argument("package")
 @verbosity_option(logger=logger)
 def lasttag(package, **_) -> None:
-    """Returns the last tag information on a given PACKAGE."""
+    """Return the last tag information on a given PACKAGE."""
     import gitlab
 
-    from ...gitlab import get_gitlab_instance
-    from ...gitlab.changelog import parse_date
+    from ..gitlab import get_gitlab_instance
+    from ..gitlab.changelog import parse_date
 
     if "/" not in package:
         raise RuntimeError('PACKAGE should be specified as "group/name"')
 
     gl = get_gitlab_instance()
 
     # we lookup the gitlab package once
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/release.py` & `idiap_devtools-2.0.0/src/idiap_devtools/scripts/release.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
 import typing
 
 import click
 
-from idiap_devtools.click import validate_profile
-from idiap_devtools.profile import Profile, get_profile_path
-
-from ...click import PreserveIndentCommand, verbosity_option
-from ...logging import setup
+from ..click import PreserveIndentCommand, verbosity_option
+from ..logging import setup
 
 logger = setup(__name__.split(".", 1)[0])
 
 
 @click.command(
     cls=PreserveIndentCommand,
     epilog="""
@@ -36,89 +31,48 @@
   2. The option ``--dry-run`` can be used to let the script print what it would
      do instead of actually doing it:
 
      .. code:: sh
 
         devtool gitlab release -vv --dry-run changelog.md
 
-  3. You may also pin package dependencies upon the release, so that the
-     shipped package respects a particular development profile set of pins:
-
-     .. code:: sh
-
-        devtool gitlab release -vv --pin-dependencies changelog.md
-
-     The `default` profile is used, if set on your configuration file.
-     Otherwise, you may specify it explicitly like:
-
-     .. code:: sh
-
-        devtool gitlab release -vv --profile=specific --pin-dependencies changelog.md
-
 """,
 )
 @click.argument("changelog", type=click.File("rt", lazy=False))
 @click.option(
-    "-P",
-    "--profile",
-    default="default",
-    show_default=True,
-    callback=validate_profile,
-    help="Directory containing the development profile (and a file named "
-    "profile.toml), or the name of a configuration key pointing to the "
-    "development profile to use",
-)
-@click.option(
-    "-p",
-    "--pin-dependencies/--no-pin-dependencies",
-    default=False,
-    help="If set, then pin dependencies from the dev-profile on the package "
-    "to be released.  By default your default dev-profile is used.  You may "
-    "override this using the --profile option",
-)
-@click.option(
     "-d",
     "--dry-run/--no-dry-run",
     default=False,
     help="Only goes through the actions, but does not execute them "
     "(combine with the verbosity flags - e.g. ``-vvv``) to enable "
     "printing to help you understand what will be done",
 )
 @verbosity_option(logger=logger)
 def release(
     changelog: typing.TextIO,
-    profile: str,
-    pin_dependencies: bool,
     dry_run: bool,
     **_,
 ) -> None:
     """Tags packages on GitLab from an input CHANGELOG in markdown format.
 
     By using a CHANGELOG file as an input (e.g. that can be generated with the
     ``changelog`` command), this script goes through all packages listed (and
     in order):
 
-        * Modifies ``pyproject.toml`` with the new release number and pins the
-          dependencies according to the specified profile's constraints (if one
-          was specified)
+        * Modifies ``pyproject.toml`` with the new release number
         * Sets-up the README links to point to the correct pipeline and
           documentation for the package
         * Commits, tags and pushes the git project adding the changelog
           description for the GitLab release page
         * Waits for the pipeline launched by the previous step to end
         * Bumps the package version again, to the next beta patch
         * Re-modifies the README to point to the "latest" documentation and
           pipeline versions
         * Re-commits and pushes the whole with the option ``[ci skip]``.
 
-    N.B.: When the option ``pin-dependencies`` is set, the versions of the
-    dependencies in ``pyproject.toml`` will be pinned to those of the Python
-    ``constraints.txt`` file available in the select development profile
-    (choose using option ``--profile``).
-
     The changelog is expected to have the following structure:
 
     .. code:: markdown
 
        # group-name/package-name: ``major``|``minor``|``patch``
 
          Description of changes in group-name/package-name
@@ -142,56 +96,40 @@
     auto-generate the description for your release.
     """
     import re
     import textwrap
 
     import packaging.version
 
-    from ...gitlab import get_gitlab_instance
-    from ...gitlab.release import (
+    from ..gitlab import get_gitlab_instance
+    from ..gitlab.release import (
         get_next_version,
         release_package,
         wait_for_pipeline_to_finish,
     )
 
     gl = get_gitlab_instance()
 
     # traverse all packages in the changelog, edit older tags with updated
     # comments, tag them with a suggested version, then try to release, and
     # wait until done to proceed to the next package
     changelogs: list[str] = changelog.readlines()
 
-    header_re = re.compile(
-        r"^\s*#+\s*(?P<pkg>\S+(/\S+)+)\s*:\s*(?P<bump>\S+)\s*$"
-    )
+    header_re = re.compile(r"^\s*#+\s*(?P<pkg>\S+(/\S+)+)\s*:\s*(?P<bump>\S+)\s*$")
 
     # find the starts of each package's description at the changelog
-    pkgs = [
-        (line, k) for k, line in enumerate(changelogs) if header_re.match(line)
-    ]
+    pkgs = [(line, k) for k, line in enumerate(changelogs) if header_re.match(line)]
 
     if dry_run:
         click.secho(
             "DRY RUN MODE: No changes will be committed to GitLab.",
             fg="yellow",
             bold=True,
         )
 
-    # loads profile data
-    if pin_dependencies:
-        the_profile = Profile(profile)
-        logger.info(
-            f"Pinning dependencies from profile `{get_profile_path(profile)}'...",
-        )
-    else:
-        the_profile = None
-        logger.warning(
-            "Not pinning dependencies (use --pin-dependencies to change this).",
-        )
-
     for pkg_number, (header, line) in enumerate(pkgs):
         match = header_re.match(header)
 
         assert match, f"Line `{header}' somehow did not match title regexp"
 
         pkg = match.groupdict()["pkg"]
         bump = match.groupdict()["bump"]
@@ -218,17 +156,15 @@
             f"(id={use_package.id})",
         )
 
         # process the "bump" to be performed
         tag = bump.strip().lower()
 
         if tag in ("patch", "minor", "major"):
-            logger.info(
-                f"Processing package {pkg} to perform a {tag} release bump"
-            )
+            logger.info(f"Processing package {pkg} to perform a {tag} release bump")
 
             # gets the "next" tag for this package
             vtag = get_next_version(use_package, bump)
             logger.info(
                 f"Bumping version of "
                 f"{use_package.attributes['path_with_namespace']} "
                 f"to {vtag}",
@@ -247,15 +183,14 @@
 
         # release the package with the found tag and its comments
         pipeline_id = release_package(
             gitpkg=use_package,
             tag_name=vtag,
             tag_comments=description_text,
             dry_run=dry_run,
-            profile=the_profile,
         )
         if not dry_run:
             # now, wait for the pipeline to finish, before we can release the
             # next package
             wait_for_pipeline_to_finish(use_package, pipeline_id)
 
     logger.info(f"Finished processing {changelog.name}")
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/runners.py` & `idiap_devtools-2.0.0/src/idiap_devtools/scripts/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
-import os
+import pathlib
 
 import click
 
-from ...click import AliasedGroup, PreserveIndentCommand, verbosity_option
-from ...logging import setup
+from ..click import AliasedGroup, PreserveIndentCommand, verbosity_option
+from ..logging import setup
 
 logger = setup(__name__.split(".", 1)[0])
 
 
 @click.group(cls=AliasedGroup)
 def runners() -> None:
     """Commands for handling runners."""
@@ -55,38 +53,37 @@
     default=False,
     help="Only goes through the actions, but does not execute them "
     "(combine with the verbosity flags - e.g. ``-vvv``) to enable "
     "printing to help you understand what will be done",
 )
 @verbosity_option(logger)
 def enable(name, targets, group, dry_run, **_) -> None:
-    """Enables runners on whole gitlab groups or single projects.
+    """Enable runners on whole gitlab groups or single projects.
 
     You may provide project names (like "group/project"), whole groups,
     and files containing list of projects to enable at certain runner
     at.
     """
-    import pathlib
 
-    from ...gitlab import get_gitlab_instance
-    from ...gitlab.runners import (
+    from ..gitlab import get_gitlab_instance
+    from ..gitlab.runners import (
         get_project,
         get_projects_from_file,
         get_projects_from_group,
         get_runner_from_description,
     )
 
     gl = get_gitlab_instance()
     gl.auth()
 
     the_runner = get_runner_from_description(gl, name)
 
     packages = []
     for target in targets:
-        if os.path.exists(target):  # it is a file with project names
+        if pathlib.Path(target).exists():  # it is a file with project names
             packages += get_projects_from_file(gl, pathlib.Path(target))
 
         elif not group:  # it is a specific project
             packages.append(get_project(gl, target))
 
         else:  # it is a group - get all projects
             packages += get_projects_from_group(gl, target)
@@ -99,15 +96,15 @@
                 k.id,
             )
 
             # checks if runner is not enabled first
             enabled = False
             for ll in k.runners.list(all=True):
                 if ll.id == the_runner.id:  # it is there already
-                    logger.warn(
+                    logger.warning(
                         "Runner %s (id=%d) is already enabled for project %s",
                         ll.attributes["description"],
                         ll.id,
                         k.attributes["path_with_namespace"],
                     )
                     enabled = True
                     break
@@ -182,15 +179,14 @@
 def disable(name, targets, dry_run, **_) -> None:
     """Disables runners on whole gitlab groups or single projects.
 
     You may provide project names (like "group/project"), whole groups,
     files containing list of projects to load or omit the last argument,
     in which case all projects using this runner will be affected.
     """
-    import pathlib
 
     from ...gitlab import get_gitlab_instance
     from ...gitlab.runners import (
         get_project,
         get_projects_from_file,
         get_projects_from_group,
         get_projects_from_runner,
@@ -203,15 +199,15 @@
     the_runner = get_runner_from_description(gl, name)
 
     packages = []
     for target in targets:
         if "/" in target:  # it is a specific project
             packages.append(get_project(gl, target))
 
-        elif os.path.exists(target):  # it is a file with project names
+        elif pathlib.Path(target).exists():  # it is a file with project names
             packages += get_projects_from_file(gl, pathlib.Path(target))
 
         elif isinstance(target, str) and target:  # it is a group
             packages += get_projects_from_group(gl, target)
 
     if not targets:
         logger.info("Retrieving all runner associated projects...")
@@ -261,30 +257,31 @@
                 k.attributes["path_with_namespace"],
                 k.id,
                 str(e),
             )
 
 
 @runners.command(
+    name="list",
     cls=PreserveIndentCommand,
     epilog="""
 Examples:
 
   1. Lists all projects a runner is associated to:
 
      .. code:: sh
 
         devtool gitlab runners list -vv macmini
 
 """,
 )
 @click.argument("name")
 @verbosity_option(logger=logger)
-def list(name, **_) -> None:
-    """Lists projects a runner is associated to."""
+def list_(name, **_) -> None:
+    """List projects a runner is associated to."""
     from ...gitlab import get_gitlab_instance
     from ...gitlab.runners import get_runner_from_description
 
     gl = get_gitlab_instance()
     gl.auth()
 
     the_runner = get_runner_from_description(gl, name)
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/scripts/gitlab/settings.py` & `idiap_devtools-2.0.0/src/idiap_devtools/scripts/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
+import pathlib
 import typing
 
 import click
 
-from ...click import PreserveIndentCommand, verbosity_option
-from ...logging import setup
+from ..click import PreserveIndentCommand, verbosity_option
+from ..logging import setup
 
 logger = setup(__name__.split(".", 1)[0])
 
 
-def _change_settings(
-    project, info: dict[str, typing.Any], dry_run: bool
-) -> None:
-    """Updates the project settings using ``info``"""
+def _change_settings(project, info: dict[str, typing.Any], dry_run: bool) -> None:
+    """Update the project settings using ``info``."""
 
     name = f"{project.namespace['full_path']}/{project.name}"
     click.echo(f"Changing {name}...")
 
     if info.get("archive") is not None:
         if info["archive"]:
             click.secho("  -> archiving", bold=True)
@@ -29,25 +26,23 @@
                 project.archive()
         else:
             click.secho("  -> unarchiving", bold=True)
             if not dry_run:
                 project.unarchive()
 
     if info.get("description") is not None:
-        click.secho(
-            f"  -> set description to '{info['description']}'", bold=True
-        )
+        click.secho(f"  -> set description to '{info['description']}'", bold=True)
         if not dry_run:
             project.description = info["description"]
             project.save()
 
     if info.get("avatar") is not None:
         click.secho(f"  -> setting avatar to '{info['avatar']}'", bold=True)
         if not dry_run:
-            project.avatar = open(info["avatar"], "rb")
+            project.avatar = pathlib.Path(info["avatar"]).open("rb")
             project.save()
 
 
 @click.command(
     cls=PreserveIndentCommand,
     epilog="""
 Examples:
@@ -99,40 +94,34 @@
     "--dry-run/--no-dry-run",
     default=False,
     help="Only goes through the actions, but does not execute them "
     "(combine with the verbosity flags - e.g. ``-vvv``) to enable "
     "printing to help you understand what will be done",
 )
 @verbosity_option(logger=logger)
-def settings(
-    projects, avatar, description, group, archive, dry_run, **_
-) -> None:
-    """Updates project settings."""
-
-    import os
+def settings(projects, avatar, description, group, archive, dry_run, **_) -> None:
+    """Update project settings."""
 
-    from ...gitlab import get_gitlab_instance
-    from ...gitlab.runners import (
+    from ..gitlab import get_gitlab_instance
+    from ..gitlab.runners import (
         get_project,
         get_projects_from_file,
         get_projects_from_group,
     )
 
     # if we are in a dry-run mode, let's let it be known
     if dry_run:
         click.secho("!!!! DRY RUN MODE !!!!", fg="yellow", bold=True)
-        click.secho(
-            "No changes will be committed to GitLab.", fg="yellow", bold=True
-        )
+        click.secho("No changes will be committed to GitLab.", fg="yellow", bold=True)
 
     gl = get_gitlab_instance()
     gl_projects = []
 
     for target in projects:
-        if os.path.exists(target):  # it is a file with project names
+        if pathlib.Path(target).exists():  # it is a file with project names
             gl_projects += get_projects_from_file(gl, target)
 
         elif not group:  # it is a specific project
             gl_projects.append(get_project(gl, target))
 
         else:  # it is a group - get all projects
             gl_projects += get_projects_from_group(gl, target)
```

### Comparing `idiap-devtools-1.0.0/src/idiap_devtools/utils.py` & `idiap_devtools-2.0.0/src/idiap_devtools/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-from __future__ import annotations
-
 import logging
 import os
 import subprocess
 import sys
 import time
 import typing
 
@@ -22,53 +20,52 @@
 )
 """Time intervals that make up human readable time slots."""
 
 
 def set_environment(
     name: str, value: str, env: dict[str, str] | os._Environ[str] = os.environ
 ) -> str:
-    """Function to setup the environment variable and print debug message.
-
-    Parameters:
-
-        name: The name of the environment variable to set
-
-        value: The value to set the environment variable to
-
-        env: Optional environment (dictionary) where to set the variable at
+    """Set up the environment variable and print debug message.
 
+    Parameters
+    ----------
+    name
+        The name of the environment variable to set
+    value
+        The value to set the environment variable to
+    env
+        Optional environment (dictionary) where to set the variable at
 
-    Returns:
-
+    Returns
+    -------
         The value just set.
     """
 
     env[name] = value
     logger.info(f"environ['{name}'] = '{value}'")
     return value
 
 
 def human_time(seconds: int | float, granularity: int = 2) -> str:
-    """Returns a human readable time string like "1 day, 2 hours".
+    """Return a human readable time string like "1 day, 2 hours".
 
     This function will convert the provided time in seconds into weeks, days,
     hours, minutes and seconds.
 
+    Parameters
+    ----------
+    seconds
+        The number of seconds to convert
+
+    granularity
+        The granularity corresponds to how many elements will output. For a
+        granularity of 2, only the first two non-zero entries are output.
 
-    Parameters:
-
-        seconds: The number of seconds to convert
-
-        granularity: The granularity corresponds to how many elements will
-            output. For a granularity of 2, only the first two non-zero entries
-            are output.
-
-
-    Returns:
-
+    Returns
+    -------
         A string, that contains the human readable time.
     """
     result: list[str | None] = []
 
     for name, count in _INTERVALS:
         value = seconds // count
         if value:
@@ -80,41 +77,42 @@
             # Add a blank if we're in the middle of other values
             if len(result) > 0:
                 result.append(None)
 
     if not result:
         if seconds < 1.0:
             return "%.2f seconds" % seconds
-        else:
-            if seconds == 1:
-                return "1 second"
-            else:
-                return "%d seconds" % seconds
+
+        if seconds == 1:
+            return "1 second"
+
+        return "%d seconds" % seconds
 
     return ", ".join([x for x in result[:granularity] if x is not None])
 
 
 def run_cmdline(
     cmd: list[str],
     logger: logging.Logger,
     **kwargs,
 ) -> int:
-    """Runs a command on a environment, logs output and reports status.
-
-    Parameters:
-
-        cmd: The command to run, with parameters separated on a list of strings
-
-        logger: A logger to log messages to console
-
-        kwargs: Further kwargs to be set on the call to
-            :py:class:`subprocess.Popen`.
-
+    """Run a command on a environment, logs output and reports status.
 
-    Returns:
+    Parameters
+    ----------
+    cmd
+        The command to run, with parameters separated on a list of strings
+    logger
+        A logger to log messages to console
+    kwargs
+        Further kwargs to be set on the call to :py:class:`subprocess.Popen`.
+
+    Returns
+    -------
+        The exit status of the command.
     """
 
     logger.info("(system) %s" % " ".join(cmd))
 
     start = time.time()
 
     p = subprocess.Popen(
@@ -128,16 +126,15 @@
 
     for line in iter(p.stdout.readline, ""):
         sys.stdout.write(line)
         sys.stdout.flush()
 
     if p.wait() != 0:
         raise RuntimeError(
-            "command `%s' exited with error state (%d)"
-            % (" ".join(cmd), p.returncode)
+            "command `%s' exited with error state (%d)" % (" ".join(cmd), p.returncode)
         )
 
     total = time.time() - start
 
     logger.info("command took %s" % human_time(total))
 
     return p.pid
```

