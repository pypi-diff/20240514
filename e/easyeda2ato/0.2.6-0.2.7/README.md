# Comparing `tmp/easyeda2ato-0.2.6.tar.gz` & `tmp/easyeda2ato-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyeda2ato-0.2.6.tar", last modified: Fri Apr 12 00:30:55 2024, max compression
+gzip compressed data, was "easyeda2ato-0.2.7.tar", last modified: Tue May 14 16:55:08 2024, max compression
```

## Comparing `easyeda2ato-0.2.6.tar` & `easyeda2ato-0.2.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-12 00:30:55.333295 easyeda2ato-0.2.6/
--rw-r--r--   0 narayanpowderly   (501) staff       (20)    34523 2023-11-20 17:47:17.000000 easyeda2ato-0.2.6/LICENSE
--rw-r--r--   0 narayanpowderly   (501) staff       (20)      283 2024-04-11 00:42:55.000000 easyeda2ato-0.2.6/MANIFEST.in
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     6141 2024-04-12 00:30:55.333473 easyeda2ato-0.2.6/PKG-INFO
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     5351 2024-03-15 22:17:17.000000 easyeda2ato-0.2.6/README.md
-drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-12 00:30:55.330078 easyeda2ato-0.2.6/easyeda2ato.egg-info/
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     6141 2024-04-12 00:30:55.000000 easyeda2ato-0.2.6/easyeda2ato.egg-info/PKG-INFO
--rw-r--r--   0 narayanpowderly   (501) staff       (20)      917 2024-04-12 00:30:55.000000 easyeda2ato-0.2.6/easyeda2ato.egg-info/SOURCES.txt
--rw-r--r--   0 narayanpowderly   (501) staff       (20)        1 2024-04-12 00:30:55.000000 easyeda2ato-0.2.6/easyeda2ato.egg-info/dependency_links.txt
--rw-r--r--   0 narayanpowderly   (501) staff       (20)       62 2024-04-12 00:30:55.000000 easyeda2ato-0.2.6/easyeda2ato.egg-info/entry_points.txt
--rw-r--r--   0 narayanpowderly   (501) staff       (20)        1 2024-04-11 17:56:19.000000 easyeda2ato-0.2.6/easyeda2ato.egg-info/not-zip-safe
--rw-r--r--   0 narayanpowderly   (501) staff       (20)       57 2024-04-12 00:30:55.000000 easyeda2ato-0.2.6/easyeda2ato.egg-info/requires.txt
--rw-r--r--   0 narayanpowderly   (501) staff       (20)       14 2024-04-12 00:30:55.000000 easyeda2ato-0.2.6/easyeda2ato.egg-info/top_level.txt
-drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-12 00:30:55.330719 easyeda2ato-0.2.6/easyeda2kicad/
--rw-r--r--   0 narayanpowderly   (501) staff       (20)       75 2024-04-11 18:04:43.000000 easyeda2ato-0.2.6/easyeda2kicad/__init__.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)    14263 2024-04-11 22:00:00.000000 easyeda2ato-0.2.6/easyeda2kicad/__main__.py
-drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-12 00:30:55.331056 easyeda2ato-0.2.6/easyeda2kicad/atopile/
--rw-r--r--   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 01:17:18.000000 easyeda2ato-0.2.6/easyeda2kicad/atopile/__init__.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     3892 2024-04-11 18:28:55.000000 easyeda2ato-0.2.6/easyeda2kicad/atopile/export_ato.py
-drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-12 00:30:55.331800 easyeda2ato-0.2.6/easyeda2kicad/easyeda/
--rw-r--r--   0 narayanpowderly   (501) staff       (20)        0 2023-12-11 18:29:50.000000 easyeda2ato-0.2.6/easyeda2kicad/easyeda/__init__.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     2307 2024-03-15 22:15:55.000000 easyeda2ato-0.2.6/easyeda2kicad/easyeda/easyeda_api.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     9743 2024-03-15 22:15:55.000000 easyeda2ato-0.2.6/easyeda2kicad/easyeda/easyeda_importer.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)    14438 2024-03-15 22:15:55.000000 easyeda2ato-0.2.6/easyeda2kicad/easyeda/parameters_easyeda.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     1833 2023-12-11 18:29:50.000000 easyeda2ato-0.2.6/easyeda2kicad/easyeda/svg_path_parser.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     5263 2023-12-11 18:29:50.000000 easyeda2ato-0.2.6/easyeda2kicad/helpers.py
-drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-12 00:30:55.333130 easyeda2ato-0.2.6/easyeda2kicad/kicad/
--rw-r--r--   0 narayanpowderly   (501) staff       (20)        0 2023-12-11 18:29:50.000000 easyeda2ato-0.2.6/easyeda2kicad/kicad/__init__.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     4737 2024-04-11 20:11:04.000000 easyeda2ato-0.2.6/easyeda2kicad/kicad/export_kicad_3d_model.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)    18124 2024-04-12 00:04:11.000000 easyeda2ato-0.2.6/easyeda2kicad/kicad/export_kicad_footprint.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)    12792 2023-12-11 18:29:50.000000 easyeda2ato-0.2.6/easyeda2kicad/kicad/export_kicad_symbol.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     7207 2023-12-11 18:29:50.000000 easyeda2ato-0.2.6/easyeda2kicad/kicad/parameters_kicad_footprint.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)    22150 2023-12-11 18:29:50.000000 easyeda2ato-0.2.6/easyeda2kicad/kicad/parameters_kicad_symbol.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     1244 2023-12-11 18:09:41.000000 easyeda2ato-0.2.6/pyproject.toml
--rw-r--r--   0 narayanpowderly   (501) staff       (20)      446 2024-04-12 00:30:55.333844 easyeda2ato-0.2.6/setup.cfg
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     1721 2024-04-12 00:29:34.000000 easyeda2ato-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:55:08.859468 easyeda2ato-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-14 16:55:08.859468 easyeda2ato-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:55:08.859468 easyeda2ato-0.2.7/easyeda2ato.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-14 16:55:08.000000 easyeda2ato-0.2.7/easyeda2ato.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-14 16:55:08.000000 easyeda2ato-0.2.7/easyeda2ato.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:55:08.000000 easyeda2ato-0.2.7/easyeda2ato.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 16:55:08.000000 easyeda2ato-0.2.7/easyeda2ato.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:55:08.000000 easyeda2ato-0.2.7/easyeda2ato.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 16:55:08.000000 easyeda2ato-0.2.7/easyeda2ato.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 16:55:08.000000 easyeda2ato-0.2.7/easyeda2ato.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:55:08.855468 easyeda2ato-0.2.7/easyeda2kicad/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14263 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:55:08.859468 easyeda2ato-0.2.7/easyeda2kicad/atopile/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/atopile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/atopile/export_ato.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:55:08.859468 easyeda2ato-0.2.7/easyeda2kicad/easyeda/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/easyeda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/easyeda/easyeda_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/easyeda/easyeda_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14438 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/easyeda/parameters_easyeda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/easyeda/svg_path_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:55:08.859468 easyeda2ato-0.2.7/easyeda2kicad/kicad/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/kicad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/kicad/export_kicad_3d_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18124 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/kicad/export_kicad_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12792 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/kicad/export_kicad_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/kicad/parameters_kicad_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22150 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/easyeda2kicad/kicad/parameters_kicad_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 16:55:08.859468 easyeda2ato-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-14 16:55:04.000000 easyeda2ato-0.2.7/setup.py
```

### Comparing `easyeda2ato-0.2.6/LICENSE` & `easyeda2ato-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/PKG-INFO` & `easyeda2ato-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyeda2ato
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python script that convert any electronic components from LCSC or EasyEDA to a Kicad library
 Home-page: https://github.com/uPesy/easyeda2kicad.py
 Author: uPesy
 Author-email: contact@upesy.com
 License: AGPL-3.0
 Project-URL: Code, https://github.com/uPesy/easyeda2kicad.py
 Keywords: easyeda kicad library conversion
@@ -12,16 +12,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pydantic>=2.0.0
+Requires-Dist: requests>2.0.0
+Provides-Extra: dev
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
 
 # easyeda2kicad v0.7.0
 
 _________________
 [![PyPI version](https://badge.fury.io/py/easyeda2kicad.svg)](https://badge.fury.io/py/easyeda2kicad)
 [![License](https://img.shields.io/github/license/upesy/easyeda2kicad.py.svg)](https://pypi.org/project/isort/)
 [![Downloads](https://pepy.tech/badge/easyeda2kicad)](https://pepy.tech/project/easyeda2kicad)
```

#### html2text {}

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1 Name: easyeda2ato Version: 0.2.6 Summary: A Python script
+Metadata-Version: 2.1 Name: easyeda2ato Version: 0.2.7 Summary: A Python script
 that convert any electronic components from LCSC or EasyEDA to a Kicad library
 Home-page: https://github.com/uPesy/easyeda2kicad.py Author: uPesy Author-
 email: contact@upesy.com License: AGPL-3.0 Project-URL: Code, https://
 github.com/uPesy/easyeda2kicad.py Keywords: easyeda kicad library conversion
 Platform: any Classifier: Intended Audience :: Developers Classifier: License
 :: OSI Approved :: GNU Affero General Public License v3 Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering :: Electronic Design Automation (EDA) Requires-
-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra: dev
-License-File: LICENSE # easyeda2kicad v0.7.0 _________________ [![PyPI version]
-(https://badge.fury.io/py/easyeda2kicad.svg)](https://badge.fury.io/py/
-easyeda2kicad) [![License](https://img.shields.io/github/license/upesy/
-easyeda2kicad.py.svg)](https://pypi.org/project/isort/) [![Downloads](https://
-pepy.tech/badge/easyeda2kicad)](https://pepy.tech/project/easyeda2kicad) !
-[Python versions](https://img.shields.io/pypi/pyversions/easyeda2kicad.svg) [!
-[Git hook: pre-commit](https://img.shields.io/badge/pre--commit-enabled-
-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/
-pre-commit) [![Code style: black](https://img.shields.io/badge/code%20style-
-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://
-img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)]
-(https://pycqa.github.io/isort/) [![security: bandit](https://img.shields.io/
-badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
-_________________ A Python script that converts any electronic components from
-[EasyEDA](https://easyeda.com/) or [LCSC](https://www.lcsc.com/) to a Kicad
-library including **3D model** in color. This tool will speed up your PCB
-design workflow especially when using [JLCPCB SMT assembly services](https://
-jlcpcb.com/caa). **It supports library formats for both Kicad v6.x and Kicad
-v5.x.**
+Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: pydantic>=2.0.0 Requires-Dist: requests>2.0.0 Provides-Extra:
+dev Requires-Dist: pre-commit>=2.17.0; extra == "dev" # easyeda2kicad v0.7.0
+_________________ [![PyPI version](https://badge.fury.io/py/easyeda2kicad.svg)]
+(https://badge.fury.io/py/easyeda2kicad) [![License](https://img.shields.io/
+github/license/upesy/easyeda2kicad.py.svg)](https://pypi.org/project/isort/) [!
+[Downloads](https://pepy.tech/badge/easyeda2kicad)](https://pepy.tech/project/
+easyeda2kicad) ![Python versions](https://img.shields.io/pypi/pyversions/
+easyeda2kicad.svg) [![Git hook: pre-commit](https://img.shields.io/badge/pre--
+commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://
+github.com/pre-commit/pre-commit) [![Code style: black](https://img.shields.io/
+badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports:
+isort](https://img.shields.io/badge/%20imports-isort-
+%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [!
+[security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)]
+(https://github.com/PyCQA/bandit) _________________ A Python script that
+converts any electronic components from [EasyEDA](https://easyeda.com/) or
+[LCSC](https://www.lcsc.com/) to a Kicad library including **3D model** in
+color. This tool will speed up your PCB design workflow especially when using
+[JLCPCB SMT assembly services](https://jlcpcb.com/caa). **It supports library
+formats for both Kicad v6.x and Kicad v5.x.**
  [https://raw.githubusercontent.com/uPesy/easyeda2kicad.py/master/ressources/
                                demo_symbol.png]
  [https://raw.githubusercontent.com/uPesy/easyeda2kicad.py/master/ressources/
                               demo_footprint.png]
 ## ð Sponsor and Support If this tool has saved you a lot of time when
 designing a PCB, please consider supporting the project by : - Subscribing to
 uPesy Premium Membership to have access to high-quality electronics tutorials
```

### Comparing `easyeda2ato-0.2.6/README.md` & `easyeda2ato-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/easyeda2ato.egg-info/PKG-INFO` & `easyeda2ato-0.2.7/easyeda2ato.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyeda2ato
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python script that convert any electronic components from LCSC or EasyEDA to a Kicad library
 Home-page: https://github.com/uPesy/easyeda2kicad.py
 Author: uPesy
 Author-email: contact@upesy.com
 License: AGPL-3.0
 Project-URL: Code, https://github.com/uPesy/easyeda2kicad.py
 Keywords: easyeda kicad library conversion
@@ -12,16 +12,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pydantic>=2.0.0
+Requires-Dist: requests>2.0.0
+Provides-Extra: dev
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
 
 # easyeda2kicad v0.7.0
 
 _________________
 [![PyPI version](https://badge.fury.io/py/easyeda2kicad.svg)](https://badge.fury.io/py/easyeda2kicad)
 [![License](https://img.shields.io/github/license/upesy/easyeda2kicad.py.svg)](https://pypi.org/project/isort/)
 [![Downloads](https://pepy.tech/badge/easyeda2kicad)](https://pepy.tech/project/easyeda2kicad)
```

#### html2text {}

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1 Name: easyeda2ato Version: 0.2.6 Summary: A Python script
+Metadata-Version: 2.1 Name: easyeda2ato Version: 0.2.7 Summary: A Python script
 that convert any electronic components from LCSC or EasyEDA to a Kicad library
 Home-page: https://github.com/uPesy/easyeda2kicad.py Author: uPesy Author-
 email: contact@upesy.com License: AGPL-3.0 Project-URL: Code, https://
 github.com/uPesy/easyeda2kicad.py Keywords: easyeda kicad library conversion
 Platform: any Classifier: Intended Audience :: Developers Classifier: License
 :: OSI Approved :: GNU Affero General Public License v3 Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering :: Electronic Design Automation (EDA) Requires-
-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra: dev
-License-File: LICENSE # easyeda2kicad v0.7.0 _________________ [![PyPI version]
-(https://badge.fury.io/py/easyeda2kicad.svg)](https://badge.fury.io/py/
-easyeda2kicad) [![License](https://img.shields.io/github/license/upesy/
-easyeda2kicad.py.svg)](https://pypi.org/project/isort/) [![Downloads](https://
-pepy.tech/badge/easyeda2kicad)](https://pepy.tech/project/easyeda2kicad) !
-[Python versions](https://img.shields.io/pypi/pyversions/easyeda2kicad.svg) [!
-[Git hook: pre-commit](https://img.shields.io/badge/pre--commit-enabled-
-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/
-pre-commit) [![Code style: black](https://img.shields.io/badge/code%20style-
-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://
-img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)]
-(https://pycqa.github.io/isort/) [![security: bandit](https://img.shields.io/
-badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
-_________________ A Python script that converts any electronic components from
-[EasyEDA](https://easyeda.com/) or [LCSC](https://www.lcsc.com/) to a Kicad
-library including **3D model** in color. This tool will speed up your PCB
-design workflow especially when using [JLCPCB SMT assembly services](https://
-jlcpcb.com/caa). **It supports library formats for both Kicad v6.x and Kicad
-v5.x.**
+Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: pydantic>=2.0.0 Requires-Dist: requests>2.0.0 Provides-Extra:
+dev Requires-Dist: pre-commit>=2.17.0; extra == "dev" # easyeda2kicad v0.7.0
+_________________ [![PyPI version](https://badge.fury.io/py/easyeda2kicad.svg)]
+(https://badge.fury.io/py/easyeda2kicad) [![License](https://img.shields.io/
+github/license/upesy/easyeda2kicad.py.svg)](https://pypi.org/project/isort/) [!
+[Downloads](https://pepy.tech/badge/easyeda2kicad)](https://pepy.tech/project/
+easyeda2kicad) ![Python versions](https://img.shields.io/pypi/pyversions/
+easyeda2kicad.svg) [![Git hook: pre-commit](https://img.shields.io/badge/pre--
+commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://
+github.com/pre-commit/pre-commit) [![Code style: black](https://img.shields.io/
+badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports:
+isort](https://img.shields.io/badge/%20imports-isort-
+%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [!
+[security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)]
+(https://github.com/PyCQA/bandit) _________________ A Python script that
+converts any electronic components from [EasyEDA](https://easyeda.com/) or
+[LCSC](https://www.lcsc.com/) to a Kicad library including **3D model** in
+color. This tool will speed up your PCB design workflow especially when using
+[JLCPCB SMT assembly services](https://jlcpcb.com/caa). **It supports library
+formats for both Kicad v6.x and Kicad v5.x.**
  [https://raw.githubusercontent.com/uPesy/easyeda2kicad.py/master/ressources/
                                demo_symbol.png]
  [https://raw.githubusercontent.com/uPesy/easyeda2kicad.py/master/ressources/
                               demo_footprint.png]
 ## ð Sponsor and Support If this tool has saved you a lot of time when
 designing a PCB, please consider supporting the project by : - Subscribing to
 uPesy Premium Membership to have access to high-quality electronics tutorials
```

### Comparing `easyeda2ato-0.2.6/easyeda2ato.egg-info/SOURCES.txt` & `easyeda2ato-0.2.7/easyeda2ato.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/easyeda2kicad/__main__.py` & `easyeda2ato-0.2.7/easyeda2kicad/__main__.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/easyeda2kicad/atopile/export_ato.py` & `easyeda2ato-0.2.7/easyeda2kicad/atopile/export_ato.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 def convert_to_ato(
     ee_symbol: EeSymbol, component_id: str, component_name: str, footprint: str
 ) -> str:
     ato_str = f"component {sanitize_name(component_name)}:\n"
     ato_str += f"    # component {component_name}\n"
     ato_str += f'    footprint = "{footprint}"\n'
     ato_str += f'    lcsc_id = "{component_id}"\n'
+    ato_str += f'    mpn = "{component_id}"\n'
     ato_str += "    # pins\n"
 
     defined_signals = set()
     for ee_pin in ee_symbol.pins:
         # clean the signal name from any non-alphanumeric symbols or leading digits
         signal = sanitize_name(ee_pin.name.text)
```

### Comparing `easyeda2ato-0.2.6/easyeda2kicad/easyeda/easyeda_api.py` & `easyeda2ato-0.2.7/easyeda2kicad/easyeda/easyeda_api.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/easyeda2kicad/easyeda/easyeda_importer.py` & `easyeda2ato-0.2.7/easyeda2kicad/easyeda/easyeda_importer.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/easyeda2kicad/easyeda/parameters_easyeda.py` & `easyeda2ato-0.2.7/easyeda2kicad/easyeda/parameters_easyeda.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/easyeda2kicad/easyeda/svg_path_parser.py` & `easyeda2ato-0.2.7/easyeda2kicad/easyeda/svg_path_parser.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/easyeda2kicad/helpers.py` & `easyeda2ato-0.2.7/easyeda2kicad/helpers.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/easyeda2kicad/kicad/export_kicad_3d_model.py` & `easyeda2ato-0.2.7/easyeda2kicad/kicad/export_kicad_3d_model.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/easyeda2kicad/kicad/export_kicad_footprint.py` & `easyeda2ato-0.2.7/easyeda2kicad/kicad/export_kicad_footprint.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/easyeda2kicad/kicad/export_kicad_symbol.py` & `easyeda2ato-0.2.7/easyeda2kicad/kicad/export_kicad_symbol.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/easyeda2kicad/kicad/parameters_kicad_footprint.py` & `easyeda2ato-0.2.7/easyeda2kicad/kicad/parameters_kicad_footprint.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/easyeda2kicad/kicad/parameters_kicad_symbol.py` & `easyeda2ato-0.2.7/easyeda2kicad/kicad/parameters_kicad_symbol.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/pyproject.toml` & `easyeda2ato-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.6/setup.py` & `easyeda2ato-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     name="easyeda2ato",
     description=(
         "A Python script that convert any electronic components from LCSC or EasyEDA to"
         " a Kicad library"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.2.6",
+    version="0.2.7",
     author="uPesy",
     author_email="contact@upesy.com",
     url="https://github.com/uPesy/easyeda2kicad.py",
     project_urls={
         "Code": "https://github.com/uPesy/easyeda2kicad.py",
     },
     # download_url='',
```

