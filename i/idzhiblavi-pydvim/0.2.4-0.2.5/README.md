# Comparing `tmp/idzhiblavi_pydvim-0.2.4.tar.gz` & `tmp/idzhiblavi_pydvim-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idzhiblavi_pydvim-0.2.4.tar", last modified: Tue May 14 17:21:25 2024, max compression
+gzip compressed data, was "idzhiblavi_pydvim-0.2.5.tar", last modified: Tue May 14 17:22:19 2024, max compression
```

## Comparing `idzhiblavi_pydvim-0.2.4.tar` & `idzhiblavi_pydvim-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-14 17:21:25.998793 idzhiblavi_pydvim-0.2.4/
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     1074 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.4/LICENSE
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-14 17:21:25.998735 idzhiblavi_pydvim-0.2.4/PKG-INFO
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       63 2024-05-13 06:05:43.000000 idzhiblavi_pydvim-0.2.4/README.md
-drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-14 17:21:25.997799 idzhiblavi_pydvim-0.2.4/dvim/
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.4/dvim/__init__.py
--rwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)     1097 2024-05-14 17:20:34.000000 idzhiblavi_pydvim-0.2.4/dvim/__main__.py
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     3496 2024-05-14 17:20:46.000000 idzhiblavi_pydvim-0.2.4/dvim/runner.py
-drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-14 17:21:25.998570 idzhiblavi_pydvim-0.2.4/idzhiblavi_pydvim.egg-info/
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-14 17:21:25.000000 idzhiblavi_pydvim-0.2.4/idzhiblavi_pydvim.egg-info/PKG-INFO
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      293 2024-05-14 17:21:25.000000 idzhiblavi_pydvim-0.2.4/idzhiblavi_pydvim.egg-info/SOURCES.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        1 2024-05-14 17:21:25.000000 idzhiblavi_pydvim-0.2.4/idzhiblavi_pydvim.egg-info/dependency_links.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       55 2024-05-14 17:21:25.000000 idzhiblavi_pydvim-0.2.4/idzhiblavi_pydvim.egg-info/entry_points.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        5 2024-05-14 17:21:25.000000 idzhiblavi_pydvim-0.2.4/idzhiblavi_pydvim.egg-info/top_level.txt
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      589 2024-05-14 17:21:25.999052 idzhiblavi_pydvim-0.2.4/setup.cfg
--rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       38 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.4/setup.py
+drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-14 17:22:19.603219 idzhiblavi_pydvim-0.2.5/
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     1074 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.5/LICENSE
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-14 17:22:19.603160 idzhiblavi_pydvim-0.2.5/PKG-INFO
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       63 2024-05-13 06:05:43.000000 idzhiblavi_pydvim-0.2.5/README.md
+drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-14 17:22:19.602259 idzhiblavi_pydvim-0.2.5/dvim/
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.5/dvim/__init__.py
+-rwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)     1102 2024-05-14 17:21:58.000000 idzhiblavi_pydvim-0.2.5/dvim/__main__.py
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)     3496 2024-05-14 17:20:46.000000 idzhiblavi_pydvim-0.2.5/dvim/runner.py
+drwxr-xr-x   0 dzhiblavi (652670108) LD\Domain Users (593637566)        0 2024-05-14 17:22:19.602950 idzhiblavi_pydvim-0.2.5/idzhiblavi_pydvim.egg-info/
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      300 2024-05-14 17:22:19.000000 idzhiblavi_pydvim-0.2.5/idzhiblavi_pydvim.egg-info/PKG-INFO
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      293 2024-05-14 17:22:19.000000 idzhiblavi_pydvim-0.2.5/idzhiblavi_pydvim.egg-info/SOURCES.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        1 2024-05-14 17:22:19.000000 idzhiblavi_pydvim-0.2.5/idzhiblavi_pydvim.egg-info/dependency_links.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       55 2024-05-14 17:22:19.000000 idzhiblavi_pydvim-0.2.5/idzhiblavi_pydvim.egg-info/entry_points.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)        5 2024-05-14 17:22:19.000000 idzhiblavi_pydvim-0.2.5/idzhiblavi_pydvim.egg-info/top_level.txt
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)      589 2024-05-14 17:22:19.603469 idzhiblavi_pydvim-0.2.5/setup.cfg
+-rw-r--r--   0 dzhiblavi (652670108) LD\Domain Users (593637566)       38 2024-05-13 06:05:12.000000 idzhiblavi_pydvim-0.2.5/setup.py
```

### Comparing `idzhiblavi_pydvim-0.2.4/LICENSE` & `idzhiblavi_pydvim-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `idzhiblavi_pydvim-0.2.4/dvim/__main__.py` & `idzhiblavi_pydvim-0.2.5/dvim/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 import click
-from runner import Runner
+from dvim.runner import Runner
 
 
 @click.command()
 @click.option("--debug/--no-debug", default=False)
 @click.option("--executable", default="nvim")
 @click.option("--workspace", default=None)
 @click.option("--session", default=None)
```

### Comparing `idzhiblavi_pydvim-0.2.4/dvim/runner.py` & `idzhiblavi_pydvim-0.2.5/dvim/runner.py`

 * *Files identical despite different names*

### Comparing `idzhiblavi_pydvim-0.2.4/setup.cfg` & `idzhiblavi_pydvim-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = idzhiblavi_pydvim
-version = 0.2.4
+version = 0.2.5
 license_files = LICENSE
 author = Ibragim Dzhiblavi
 author_email = dzhiblavi@gmail.com
 description = Lightweight neovim wrapper
 long_description = file:README.md
 project_urls = 
 	Source = https://github.com/dzhiblavi/pydvim
```

