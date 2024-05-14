# Comparing `tmp/mopac_step-2024.5.14.tar.gz` & `tmp/mopac_step-2024.5.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mopac_step-2024.5.14.tar", last modified: Tue May 14 20:38:15 2024, max compression
+gzip compressed data, was "mopac_step-2024.5.14.1.tar", last modified: Tue May 14 20:59:02 2024, max compression
```

## Comparing `mopac_step-2024.5.14.tar` & `mopac_step-2024.5.14.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:38:15.042104 mopac_step-2024.5.14/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-05-14 20:38:15.042104 mopac_step-2024.5.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:38:15.034104 mopac_step-2024.5.14/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:38:15.034104 mopac_step-2024.5.14/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:38:15.034104 mopac_step-2024.5.14/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9525 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:38:15.034104 mopac_step-2024.5.14/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:38:15.034104 mopac_step-2024.5.14/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:38:15.034104 mopac_step-2024.5.14/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:38:15.046104 mopac_step-2024.5.14/mopac_step/
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-14 20:38:15.046104 mopac_step-2024.5.14/mopac_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:38:15.042104 mopac_step-2024.5.14/mopac_step/data/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/data/mopac.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (127)    24413 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/data/seamm-mopac.yml
--rw-r--r--   0 runner    (1001) docker     (127)    43307 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/forceconstants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/forceconstants_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/forceconstants_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/ir_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/ir_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    19533 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/lewis_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/lewis_structure_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/lewis_structure_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    64682 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    16498 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/mopac.py
--rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/mopac_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/mopac_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/optimization_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/thermodynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/thermodynamics_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/thermodynamics_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/tk_forceconstants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/tk_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/tk_lewis_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/tk_mopac.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/tk_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/mopac_step/tk_thermodynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:38:15.042104 mopac_step-2024.5.14/mopac_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-05-14 20:38:15.000000 mopac_step-2024.5.14/mopac_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-14 20:38:15.000000 mopac_step-2024.5.14/mopac_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:38:15.000000 mopac_step-2024.5.14/mopac_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-14 20:38:15.000000 mopac_step-2024.5.14/mopac_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 20:38:15.000000 mopac_step-2024.5.14/mopac_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 20:38:15.000000 mopac_step-2024.5.14/mopac_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:38:00.000000 mopac_step-2024.5.14/mopac_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-14 20:38:15.042104 mopac_step-2024.5.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:38:15.042104 mopac_step-2024.5.14/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/tests/test_mopac_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-14 20:37:57.000000 mopac_step-2024.5.14/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:59:02.309392 mopac_step-2024.5.14.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-05-14 20:59:02.309392 mopac_step-2024.5.14.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:59:02.301392 mopac_step-2024.5.14.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:59:02.301392 mopac_step-2024.5.14.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:59:02.301392 mopac_step-2024.5.14.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9525 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:59:02.301392 mopac_step-2024.5.14.1/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:59:02.301392 mopac_step-2024.5.14.1/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:59:02.301392 mopac_step-2024.5.14.1/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:59:02.309392 mopac_step-2024.5.14.1/mopac_step/
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-14 20:59:02.309392 mopac_step-2024.5.14.1/mopac_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:59:02.309392 mopac_step-2024.5.14.1/mopac_step/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/data/mopac.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    24413 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/data/seamm-mopac.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    43307 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/forceconstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/forceconstants_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/forceconstants_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/ir_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/ir_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19533 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/lewis_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/lewis_structure_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/lewis_structure_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64682 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16498 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/mopac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/mopac_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/mopac_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/optimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/thermodynamics_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/thermodynamics_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/tk_forceconstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/tk_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/tk_lewis_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/tk_mopac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/tk_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/mopac_step/tk_thermodynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:59:02.309392 mopac_step-2024.5.14.1/mopac_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-05-14 20:59:02.000000 mopac_step-2024.5.14.1/mopac_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-14 20:59:02.000000 mopac_step-2024.5.14.1/mopac_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:59:02.000000 mopac_step-2024.5.14.1/mopac_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-14 20:59:02.000000 mopac_step-2024.5.14.1/mopac_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 20:59:02.000000 mopac_step-2024.5.14.1/mopac_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 20:59:02.000000 mopac_step-2024.5.14.1/mopac_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:58:47.000000 mopac_step-2024.5.14.1/mopac_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-14 20:59:02.309392 mopac_step-2024.5.14.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:59:02.309392 mopac_step-2024.5.14.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/tests/test_mopac_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-14 20:58:44.000000 mopac_step-2024.5.14.1/versioneer.py
```

### Comparing `mopac_step-2024.5.14/CONTRIBUTING.rst` & `mopac_step-2024.5.14.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/HISTORY.rst` & `mopac_step-2024.5.14.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/LICENSE` & `mopac_step-2024.5.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/PKG-INFO` & `mopac_step-2024.5.14.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mopac_step
-Version: 2024.5.14
+Version: 2024.5.14.1
 Summary: A SEAMM plug-in to setup, run and analyze semiempirical calculations with MOPAC
 Home-page: https://github.com/molssi-seam/mopac_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,MOPAC,semiempirical,orbitals
 Platform: Linux
```

### Comparing `mopac_step-2024.5.14/README.rst` & `mopac_step-2024.5.14.1/README.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/docs/Makefile` & `mopac_step-2024.5.14.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/docs/_static/SEAMM inverted.png` & `mopac_step-2024.5.14.1/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/docs/_static/SEAMM logo.png` & `mopac_step-2024.5.14.1/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/docs/_static/molssi_main_logo.png` & `mopac_step-2024.5.14.1/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/docs/_static/molssi_main_logo_inverted_white.png` & `mopac_step-2024.5.14.1/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/docs/_static/molssi_square.png` & `mopac_step-2024.5.14.1/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/docs/_static/nsf.png` & `mopac_step-2024.5.14.1/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/docs/conf.py` & `mopac_step-2024.5.14.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/docs/developer_guide/installation.rst` & `mopac_step-2024.5.14.1/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/docs/getting_started/index.rst` & `mopac_step-2024.5.14.1/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/docs/index.rst` & `mopac_step-2024.5.14.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/docs/make.bat` & `mopac_step-2024.5.14.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/__init__.py` & `mopac_step-2024.5.14.1/mopac_step/__init__.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/data/mopac.ini` & `mopac_step-2024.5.14.1/mopac_step/data/mopac.ini`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/data/properties.csv` & `mopac_step-2024.5.14.1/mopac_step/data/properties.csv`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/data/references.bib` & `mopac_step-2024.5.14.1/mopac_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/energy.py` & `mopac_step-2024.5.14.1/mopac_step/energy.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/energy_parameters.py` & `mopac_step-2024.5.14.1/mopac_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/energy_step.py` & `mopac_step-2024.5.14.1/mopac_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/forceconstants.py` & `mopac_step-2024.5.14.1/mopac_step/forceconstants.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/forceconstants_parameters.py` & `mopac_step-2024.5.14.1/mopac_step/forceconstants_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/forceconstants_step.py` & `mopac_step-2024.5.14.1/mopac_step/forceconstants_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/installer.py` & `mopac_step-2024.5.14.1/mopac_step/installer.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/ir.py` & `mopac_step-2024.5.14.1/mopac_step/ir.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/ir_parameters.py` & `mopac_step-2024.5.14.1/mopac_step/ir_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/ir_step.py` & `mopac_step-2024.5.14.1/mopac_step/ir_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/lewis_structure.py` & `mopac_step-2024.5.14.1/mopac_step/lewis_structure.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/lewis_structure_parameters.py` & `mopac_step-2024.5.14.1/mopac_step/lewis_structure_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/lewis_structure_step.py` & `mopac_step-2024.5.14.1/mopac_step/lewis_structure_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/metadata.py` & `mopac_step-2024.5.14.1/mopac_step/metadata.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/mopac.py` & `mopac_step-2024.5.14.1/mopac_step/mopac.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/mopac_base.py` & `mopac_step-2024.5.14.1/mopac_step/mopac_base.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/mopac_step.py` & `mopac_step-2024.5.14.1/mopac_step/mopac_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/optimization.py` & `mopac_step-2024.5.14.1/mopac_step/optimization.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/optimization_parameters.py` & `mopac_step-2024.5.14.1/mopac_step/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/optimization_step.py` & `mopac_step-2024.5.14.1/mopac_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/thermodynamics.py` & `mopac_step-2024.5.14.1/mopac_step/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/thermodynamics_parameters.py` & `mopac_step-2024.5.14.1/mopac_step/thermodynamics_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/thermodynamics_step.py` & `mopac_step-2024.5.14.1/mopac_step/thermodynamics_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/tk_energy.py` & `mopac_step-2024.5.14.1/mopac_step/tk_energy.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/tk_forceconstants.py` & `mopac_step-2024.5.14.1/mopac_step/tk_forceconstants.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/tk_ir.py` & `mopac_step-2024.5.14.1/mopac_step/tk_ir.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/tk_lewis_structure.py` & `mopac_step-2024.5.14.1/mopac_step/tk_lewis_structure.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/tk_mopac.py` & `mopac_step-2024.5.14.1/mopac_step/tk_mopac.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/tk_optimization.py` & `mopac_step-2024.5.14.1/mopac_step/tk_optimization.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step/tk_thermodynamics.py` & `mopac_step-2024.5.14.1/mopac_step/tk_thermodynamics.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step.egg-info/PKG-INFO` & `mopac_step-2024.5.14.1/mopac_step.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mopac_step
-Version: 2024.5.14
+Version: 2024.5.14.1
 Summary: A SEAMM plug-in to setup, run and analyze semiempirical calculations with MOPAC
 Home-page: https://github.com/molssi-seam/mopac_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,MOPAC,semiempirical,orbitals
 Platform: Linux
```

### Comparing `mopac_step-2024.5.14/mopac_step.egg-info/SOURCES.txt` & `mopac_step-2024.5.14.1/mopac_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/mopac_step.egg-info/entry_points.txt` & `mopac_step-2024.5.14.1/mopac_step.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/setup.py` & `mopac_step-2024.5.14.1/setup.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/tests/test_mopac_step.py` & `mopac_step-2024.5.14.1/tests/test_mopac_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2024.5.14/versioneer.py` & `mopac_step-2024.5.14.1/versioneer.py`

 * *Files identical despite different names*

