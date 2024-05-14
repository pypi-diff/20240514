# Comparing `tmp/deepnccl-2.1.0rc2.tar.gz` & `tmp/deepnccl-2.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepnccl-2.1.0rc2.tar", last modified: Thu Apr 11 04:45:23 2024, max compression
+gzip compressed data, was "deepnccl-2.1.0rc3.tar", last modified: Mon Apr 29 04:46:46 2024, max compression
```

## Comparing `deepnccl-2.1.0rc2.tar` & `deepnccl-2.1.0rc3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:45:23.028818 deepnccl-2.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)      713 2024-04-11 04:45:23.024896 deepnccl-2.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2706 2024-03-25 09:41:58.000000 deepnccl-2.1.0rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:45:22.907805 deepnccl-2.1.0rc2/deepnccl/
--rw-r--r--   0 root         (0) root         (0)     1329 2024-04-10 07:55:35.000000 deepnccl-2.1.0rc2/deepnccl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:45:23.003358 deepnccl-2.1.0rc2/deepnccl.egg-info/
--rw-r--r--   0 root         (0) root         (0)      713 2024-04-11 04:45:22.000000 deepnccl-2.1.0rc2/deepnccl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      233 2024-04-11 04:45:22.000000 deepnccl-2.1.0rc2/deepnccl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 04:45:22.000000 deepnccl-2.1.0rc2/deepnccl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-11 04:45:22.000000 deepnccl-2.1.0rc2/deepnccl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-11 04:45:22.000000 deepnccl-2.1.0rc2/deepnccl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-11 04:45:22.000000 deepnccl-2.1.0rc2/deepnccl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 04:45:23.031514 deepnccl-2.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3383 2024-04-11 04:45:05.000000 deepnccl-2.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:46:46.058338 deepnccl-2.1.0rc3/
+-rw-r--r--   0 root         (0) root         (0)      713 2024-04-29 04:46:46.058338 deepnccl-2.1.0rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2706 2024-04-29 03:01:29.000000 deepnccl-2.1.0rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:46:46.057338 deepnccl-2.1.0rc3/deepnccl/
+-rw-r--r--   0 root         (0) root         (0)     1329 2024-04-29 03:01:29.000000 deepnccl-2.1.0rc3/deepnccl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:46:46.057338 deepnccl-2.1.0rc3/deepnccl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      713 2024-04-29 04:46:46.000000 deepnccl-2.1.0rc3/deepnccl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      233 2024-04-29 04:46:46.000000 deepnccl-2.1.0rc3/deepnccl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 04:46:46.000000 deepnccl-2.1.0rc3/deepnccl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-29 04:46:46.000000 deepnccl-2.1.0rc3/deepnccl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-29 04:46:46.000000 deepnccl-2.1.0rc3/deepnccl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-29 04:46:46.000000 deepnccl-2.1.0rc3/deepnccl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 04:46:46.058338 deepnccl-2.1.0rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3383 2024-04-29 04:35:40.000000 deepnccl-2.1.0rc3/setup.py
```

### Comparing `deepnccl-2.1.0rc2/PKG-INFO` & `deepnccl-2.1.0rc3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1
 Name: deepnccl
-Version: 2.1.0rc2
+Version: 2.1.0rc3
 Summary: DEEP-NCCL is an AI-Accelerator communication framework for NVIDIA-NCCL. It implements optimized all-reduce, all-gather, reduce, broadcast, reduce-scatter, all-to-all,as well as any send/receive based communication pattern.It has been optimized to achieve high bandwidth on aliyun machines using PCIe, NVLink, NVswitch,as well as networking using InfiniBand Verbs, eRDMA or TCP/IP sockets.
 Home-page: https://help.aliyun.com/document_detail/462422.html?spm=a2c4g.462031.0.0.c5f96b4drcx52F
 Author: Alibaba Cloud
 License: Copyright (C) Alibaba Group Holding Limited
 Keywords: Distributed,Deep Learning,Communication,NCCL,DEEPGPU
 Requires-Python: >=3.8
```

### Comparing `deepnccl-2.1.0rc2/README.md` & `deepnccl-2.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `deepnccl-2.1.0rc2/deepnccl/__init__.py` & `deepnccl-2.1.0rc3/deepnccl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepnccl-2.1.0rc2/deepnccl.egg-info/PKG-INFO` & `deepnccl-2.1.0rc3/deepnccl.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1
 Name: deepnccl
-Version: 2.1.0rc2
+Version: 2.1.0rc3
 Summary: DEEP-NCCL is an AI-Accelerator communication framework for NVIDIA-NCCL. It implements optimized all-reduce, all-gather, reduce, broadcast, reduce-scatter, all-to-all,as well as any send/receive based communication pattern.It has been optimized to achieve high bandwidth on aliyun machines using PCIe, NVLink, NVswitch,as well as networking using InfiniBand Verbs, eRDMA or TCP/IP sockets.
 Home-page: https://help.aliyun.com/document_detail/462422.html?spm=a2c4g.462031.0.0.c5f96b4drcx52F
 Author: Alibaba Cloud
 License: Copyright (C) Alibaba Group Holding Limited
 Keywords: Distributed,Deep Learning,Communication,NCCL,DEEPGPU
 Requires-Python: >=3.8
```

### Comparing `deepnccl-2.1.0rc2/setup.py` & `deepnccl-2.1.0rc3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 
 import os
 import subprocess
 from setuptools import setup
 from setuptools.command.install import install
 
-version = "2.1.0rc2"
+version = "2.1.0rc3"
 package_name = "deepnccl"
 _root_path_deepgpu = "https://mirrors.aliyun.com/deepgpu/"
 _root_path_deepnccl = f"{_root_path_deepgpu}/deepnccl/{version}/deep-nccl-{version}"
 _temp_path = f"{os.environ['HOME']}/.deepnccl/"
 _temp_log = f"{_temp_path}/log"
 
 def get_os_name():
```

