# Comparing `tmp/dig_ass_critic_protos-1.0.2.tar.gz` & `tmp/dig_ass_critic_protos-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_critic_protos-1.0.2.tar", last modified: Mon May 13 14:30:18 2024, max compression
+gzip compressed data, was "dig_ass_critic_protos-1.0.3.tar", last modified: Tue May 14 10:02:36 2024, max compression
```

## Comparing `dig_ass_critic_protos-1.0.2.tar` & `dig_ass_critic_protos-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:18.281465 dig_ass_critic_protos-1.0.2/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_critic_protos-1.0.2/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      375 2024-05-13 14:30:18.281465 dig_ass_critic_protos-1.0.2/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:31.000000 dig_ass_critic_protos-1.0.2/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:18.281465 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2874 2024-05-13 14:30:16.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2610 2024-05-13 14:30:16.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3010 2024-05-13 14:30:16.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-13 14:24:44.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1577 2024-05-13 14:08:18.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:18.281465 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      375 2024-05-13 14:30:18.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      540 2024-05-13 14:30:18.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-13 14:30:18.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-13 14:30:18.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-13 14:30:18.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       56 2024-05-13 14:20:34.000000 dig_ass_critic_protos-1.0.2/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-13 14:30:18.281465 dig_ass_critic_protos-1.0.2/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      809 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.2/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:02:36.690117 dig_ass_critic_protos-1.0.3/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_critic_protos-1.0.3/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      375 2024-05-14 10:02:36.690117 dig_ass_critic_protos-1.0.3/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:31.000000 dig_ass_critic_protos-1.0.3/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:02:36.690117 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2874 2024-05-14 10:02:35.000000 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2610 2024-05-14 10:02:35.000000 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3010 2024-05-14 10:02:35.000000 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-14 10:01:31.000000 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1577 2024-05-13 14:08:18.000000 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:02:36.690117 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      375 2024-05-14 10:02:36.000000 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      540 2024-05-14 10:02:36.000000 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-14 10:02:36.000000 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-14 10:02:36.000000 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-14 10:02:36.000000 dig_ass_critic_protos-1.0.3/dig_ass_critic_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       56 2024-05-14 10:00:02.000000 dig_ass_critic_protos-1.0.3/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-14 10:02:36.690117 dig_ass_critic_protos-1.0.3/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      809 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.3/setup.py
```

### Comparing `dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py` & `dig_ass_critic_protos-1.0.3/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi` & `dig_ass_critic_protos-1.0.3/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py` & `dig_ass_critic_protos-1.0.3/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/client.py` & `dig_ass_critic_protos-1.0.3/dig_ass_critic_protos/client.py`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/SOURCES.txt` & `dig_ass_critic_protos-1.0.3/dig_ass_critic_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-1.0.2/setup.py` & `dig_ass_critic_protos-1.0.3/setup.py`

 * *Files identical despite different names*

