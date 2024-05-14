# Comparing `tmp/cosolvkit-0.4.3.tar.gz` & `tmp/cosolvkit-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosolvkit-0.4.3.tar", last modified: Sun May 12 22:36:56 2024, max compression
+gzip compressed data, was "cosolvkit-0.4.4.tar", last modified: Tue May 14 17:33:53 2024, max compression
```

## Comparing `cosolvkit-0.4.3.tar` & `cosolvkit-0.4.4.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:36:56.162469 cosolvkit-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-12 22:36:56.158470 cosolvkit-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:36:56.158470 cosolvkit-0.4.3/cosolvkit/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    58843 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/cosolvent_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:36:56.158470 cosolvkit-0.4.3/cosolvkit/data/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/aromatic.json
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/cosolvents.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/forcefields.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/h_bonding.json
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/lipophilic.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/negative.json
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/positive.json
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:36:56.158470 cosolvkit-0.4.3/cosolvkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-12 22:36:56.000000 cosolvkit-0.4.3/cosolvkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-12 22:36:56.000000 cosolvkit-0.4.3/cosolvkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 22:36:56.000000 cosolvkit-0.4.3/cosolvkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-12 22:36:56.000000 cosolvkit-0.4.3/cosolvkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 22:36:56.000000 cosolvkit-0.4.3/cosolvkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-12 22:36:56.000000 cosolvkit-0.4.3/cosolvkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 22:36:56.162469 cosolvkit-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:53.811404 cosolvkit-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 17:33:53.811404 cosolvkit-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:53.807404 cosolvkit-0.4.4/cosolvkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58843 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/cosolvent_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:53.811404 cosolvkit-0.4.4/cosolvkit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/aromatic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/cosolvents.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/forcefields.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/h_bonding.json
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/lipophilic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/negative.json
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/positive.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:53.811404 cosolvkit-0.4.4/cosolvkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 17:33:53.000000 cosolvkit-0.4.4/cosolvkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 17:33:53.000000 cosolvkit-0.4.4/cosolvkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:33:53.000000 cosolvkit-0.4.4/cosolvkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 17:33:53.000000 cosolvkit-0.4.4/cosolvkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:33:53.000000 cosolvkit-0.4.4/cosolvkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 17:33:53.000000 cosolvkit-0.4.4/cosolvkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:53.811404 cosolvkit-0.4.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/scripts/create_cosolvent_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/scripts/post_simulation_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 17:33:53.811404 cosolvkit-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/setup.py
```

### Comparing `cosolvkit-0.4.3/LICENSE` & `cosolvkit-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.3/README.md` & `cosolvkit-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![License: LGPL v2.1](https://img.shields.io/badge/License-LGPL_v2.1-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html) [![PyPI - Version](https://img.shields.io/pypi/v/cosolvkit)](https://pypi.org/project/cosolvkit/0.4.3/) [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![License: LGPL v2.1](https://img.shields.io/badge/License-LGPL_v2.1-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html) [![PyPI - Version](https://img.shields.io/pypi/v/cosolvkit)](https://pypi.org/project/cosolvkit/0.4.4/) [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
 [![Documentation Status](https://readthedocs.org/projects/cosolvkit/badge/?version=latest)](https://cosolvkit.readthedocs.io/en/latest/?badge=latest)
       
     
 
 # CosolvKit
 The python package for creating cosolvent system.  
 
@@ -10,15 +10,15 @@
 
 ## Documentation
 The installation instructions, documentation and tutorials can be found on http://cosolvkit.readthedocs.io/.
 
 ## Installation
 I highly recommend you to install the Anaconda distribution (https://www.continuum.io/downloads) if you want a clean python environnment with nearly all the prerequisites already installed. To install everything properly, you just have to do this:
 ```bash
-$ conda create -n cosolvkit -c conda-forge -f cosolvkit_env.yml
+$ conda create -n cosolvkit -c conda-forge -f environment.yml
 ```
 For faster installation, use `mamba` or `micromamba` instead of `conda`.
 
 Finally, we can install the `CosolvKit` package via `pip`:
 ```bash
 $ pip instal cosolvkit
 ```
```

### Comparing `cosolvkit-0.4.3/cosolvkit/analysis.py` & `cosolvkit-0.4.4/cosolvkit/analysis.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.3/cosolvkit/config.py` & `cosolvkit-0.4.4/cosolvkit/config.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.3/cosolvkit/cosolvent_system.py` & `cosolvkit-0.4.4/cosolvkit/cosolvent_system.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.3/cosolvkit/data/cosolvents.json` & `cosolvkit-0.4.4/cosolvkit/data/cosolvents.json`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.3/cosolvkit/simulation.py` & `cosolvkit-0.4.4/cosolvkit/simulation.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.3/cosolvkit/utils.py` & `cosolvkit-0.4.4/cosolvkit/utils.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.3/cosolvkit.egg-info/SOURCES.txt` & `cosolvkit-0.4.4/cosolvkit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,8 +17,11 @@
 cosolvkit/data/aromatic.json
 cosolvkit/data/config.json
 cosolvkit/data/cosolvents.json
 cosolvkit/data/forcefields.json
 cosolvkit/data/h_bonding.json
 cosolvkit/data/lipophilic.json
 cosolvkit/data/negative.json
-cosolvkit/data/positive.json
+cosolvkit/data/positive.json
+scripts/__init__.py
+scripts/create_cosolvent_system.py
+scripts/post_simulation_processing.py
```

