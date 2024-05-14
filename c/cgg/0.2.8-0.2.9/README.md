# Comparing `tmp/cgg-0.2.8.tar.gz` & `tmp/cgg-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgg-0.2.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cgg-0.2.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cgg-0.2.8.tar` & `cgg-0.2.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1095 2024-01-21 23:59:42.278418 cgg-0.2.8/LICENSE
--rw-r--r--   0        0        0     4066 2024-04-25 00:36:15.159266 cgg-0.2.8/README.md
--rw-r--r--   0        0        0      742 2024-04-25 00:32:11.783810 cgg-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     5563 2024-05-04 00:44:57.266735 cgg-0.2.8/src/cgg/__init__.py
--rw-r--r--   0        0        0     4492 1970-01-01 00:00:00.000000 cgg-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-01-21 23:59:42.278418 cgg-0.2.9/LICENSE
+-rw-r--r--   0        0        0     4181 2024-05-14 21:16:39.284716 cgg-0.2.9/README.md
+-rw-r--r--   0        0        0      742 2024-05-14 21:07:41.542033 cgg-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5710 2024-05-14 21:09:02.160618 cgg-0.2.9/src/cgg/__init__.py
+-rw-r--r--   0        0        0     4603 1970-01-01 00:00:00.000000 cgg-0.2.9/PKG-INFO
```

### Comparing `cgg-0.2.8/LICENSE` & `cgg-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cgg-0.2.8/README.md` & `cgg-0.2.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -125,11 +125,15 @@
 cgg oc
 ```
 Or by (online recognizor p):
 ```
 cgg op
 ```
 #### website
+Click [gguf.io](https://www.gguf.io) (mirror of gguf.us) or launch it straight from console by:
+```
+cgg io
+```
 Click [gguf.us](https://gguf.us) or launch it straight from console by:
 ```
 cgg us
 ```
```

### Comparing `cgg-0.2.8/pyproject.toml` & `cgg-0.2.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "cgg"
 authors = [{name = "calcuis", email = "info@calcu.io"}]
 description = "cgg is a short form of call gguf model/file; cgg is a cmd-based app built on gguf-connector, which allows users interacting with large language model (i.e., chatgpt) via a simple command without coding a long long syntax"
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version"]
-dependencies = ["gguf-connector >=0.7.31"]
+dependencies = ["gguf-connector >=0.7.33"]
 
 [project.urls]
 Homepage = "https://github.com/calcuis/cgg"
 Issues = "https://github.com/calcuis/cgg/issues"
 
 [project.scripts]
 cgg = "cgg.__init__:__init__"
```

### Comparing `cgg-0.2.8/src/cgg/__init__.py` & `cgg-0.2.9/src/cgg/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # !/usr/bin/env python3
 
-__version__="0.2.8"
+__version__="0.2.9"
 
 import argparse, json, os.path, urllib.request
 from rich.progress import Progress
 # rich (refined) #######################################################################
 def get_file_size(url):
     with urllib.request.urlopen(url) as response:
         size = int(response.headers['Content-Length'])
@@ -74,28 +74,31 @@
     subparsers.add_parser('s', help='sample GGUF list (internet required)')
     subparsers.add_parser('pc', help='pdf analyzor c')
     subparsers.add_parser('pp', help='pdf analyzor p')
     subparsers.add_parser('oc', help='wav recognizor c (internet required)')
     subparsers.add_parser('op', help='wav recognizor p (internet required)')
     subparsers.add_parser('vc', help='wav recognizor c')
     subparsers.add_parser('vp', help='wav recognizor p')
+    subparsers.add_parser('io', help='launch to gguf.io (mirror of us)')
     subparsers.add_parser('us', help='launch to gguf.us')
     args = parser.parse_args()
     # if statement below
     if args.subcommand == 'clone':
         clone_file(args.url)
     elif args.subcommand == 's':
         file_path = "https://raw.githubusercontent.com/calcuis/gguf-connector/main/src/gguf_connector/data.json"
         # file_path = os.path.join(os.path.dirname(__file__), 'data.json')
         json_data = read_json_file(file_path)
         print("Please select a GGUF file to download:")
         extract_names(json_data)
         handle_user_input(json_data)
     elif args.subcommand == 'us':
         from gguf_connector import w
+    elif args.subcommand == 'io':
+        from gguf_connector import i
     elif args.subcommand == 'r':
         from gguf_connector import r
     elif args.subcommand == 'oc':
         from gguf_connector import cg
     elif args.subcommand == 'op':
         from gguf_connector import pg
     elif args.subcommand == 'vc':
```

### Comparing `cgg-0.2.8/PKG-INFO` & `cgg-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: cgg
-Version: 0.2.8
+Version: 0.2.9
 Summary: cgg is a short form of call gguf model/file; cgg is a cmd-based app built on gguf-connector, which allows users interacting with large language model (i.e., chatgpt) via a simple command without coding a long long syntax
 Author-email: calcuis <info@calcu.io>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: gguf-connector >=0.7.31
+Requires-Dist: gguf-connector >=0.7.33
 Project-URL: Homepage, https://github.com/calcuis/cgg
 Project-URL: Issues, https://github.com/calcuis/cgg/issues
 
 ### GGUF caller
 
 [<img src="https://raw.githubusercontent.com/calcuis/cgg/master/cgg.gif" width="128" height="128">](https://github.com/calcuis/cgg)
 [![Static Badge](https://img.shields.io/badge/cgg-release-blue?logo=github)](https://github.com/calcuis/cgg/releases)
@@ -136,11 +136,15 @@
 cgg oc
 ```
 Or by (online recognizor p):
 ```
 cgg op
 ```
 #### website
+Click [gguf.io](https://www.gguf.io) (mirror of gguf.us) or launch it straight from console by:
+```
+cgg io
+```
 Click [gguf.us](https://gguf.us) or launch it straight from console by:
 ```
 cgg us
 ```
```

