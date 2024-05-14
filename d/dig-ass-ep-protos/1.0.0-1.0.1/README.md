# Comparing `tmp/dig_ass_ep_protos-1.0.0.tar.gz` & `tmp/dig_ass_ep_protos-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_ep_protos-1.0.0.tar", last modified: Thu May  2 11:12:45 2024, max compression
+gzip compressed data, was "dig_ass_ep_protos-1.0.1.tar", last modified: Mon May 13 14:29:53 2024, max compression
```

## Comparing `dig_ass_ep_protos-1.0.0.tar` & `dig_ass_ep_protos-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:12:45.685662 dig_ass_ep_protos-1.0.0/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-1.0.0/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-05-02 11:12:45.685662 dig_ass_ep_protos-1.0.0/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-1.0.0/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:12:45.685662 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2205 2024-05-02 11:12:44.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1559 2024-05-02 11:12:44.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-05-02 11:12:44.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1176 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:12:45.685662 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-05-02 11:12:45.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      508 2024-05-02 11:12:45.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-02 11:12:45.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-05-02 11:12:45.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-05-02 11:12:45.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-09 19:55:06.000000 dig_ass_ep_protos-1.0.0/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-02 11:12:45.685662 dig_ass_ep_protos-1.0.0/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      797 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.0/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:29:53.007382 dig_ass_ep_protos-1.0.1/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-1.0.1/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      367 2024-05-13 14:29:53.007382 dig_ass_ep_protos-1.0.1/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-1.0.1/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:29:53.007382 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2205 2024-05-13 14:29:51.000000 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1559 2024-05-13 14:29:51.000000 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-05-13 14:29:51.000000 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-13 14:27:05.000000 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1153 2024-05-13 14:05:24.000000 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:29:53.007382 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      367 2024-05-13 14:29:52.000000 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      508 2024-05-13 14:29:53.000000 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-13 14:29:52.000000 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-13 14:29:53.000000 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-05-13 14:29:53.000000 dig_ass_ep_protos-1.0.1/dig_ass_ep_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       56 2024-05-13 14:20:27.000000 dig_ass_ep_protos-1.0.1/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-13 14:29:53.007382 dig_ass_ep_protos-1.0.1/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      797 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.1/setup.py
```

### Comparing `dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py` & `dig_ass_ep_protos-1.0.1/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi` & `dig_ass_ep_protos-1.0.1/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py` & `dig_ass_ep_protos-1.0.1/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/client.py` & `dig_ass_ep_protos-1.0.1/dig_ass_ep_protos/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,34 +3,30 @@
 )
 from dig_ass_ep_protos.DigitalAssistantEntryPoint_pb2 import (
     DigitalAssistantEntryPointRequest,
     DigitalAssistantEntryPointResponse,
     OuterContextItem,
 )
 
-from .abstract_client import AbstractClient
+from agi_med_utils.abstract_client import AbstractClient
 
 
 class EntryPointClient(AbstractClient):
     def __init__(self, address) -> None:
         super().__init__(address)
         self._stub = DigitalAssistantEntryPointStub(self._channel)
 
-    def __call__(
-        self, text: str, outer_context: dict, image: bytearray, pdf: bytearray
-    ):
+    def __call__(self, text: str, outer_context: dict, image: bytearray, pdf: bytearray):
         request = DigitalAssistantEntryPointRequest(
             Text=text,
             OuterContext=OuterContextItem(
                 Sex=outer_context['Sex'],
                 Age=outer_context['Age'],
                 UserId=outer_context['UserId'],
                 SessionId=outer_context['SessionId'],
                 ClientId=outer_context['ClientId'],
             ),
             Image=image,
             PDF=pdf,
         )
-        response: DigitalAssistantEntryPointResponse = self._stub.GetTextResponse(
-            request
-        )
+        response: DigitalAssistantEntryPointResponse = self._stub.GetTextResponse(request)
         return response.Text
```

### Comparing `dig_ass_ep_protos-1.0.0/setup.py` & `dig_ass_ep_protos-1.0.1/setup.py`

 * *Files identical despite different names*

