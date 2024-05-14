# Comparing `tmp/dig_ass_ocr_protos-0.0.5.tar.gz` & `tmp/dig_ass_ocr_protos-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_ocr_protos-0.0.5.tar", last modified: Thu May  2 11:12:53 2024, max compression
+gzip compressed data, was "dig_ass_ocr_protos-0.0.6.tar", last modified: Mon May 13 14:30:01 2024, max compression
```

## Comparing `dig_ass_ocr_protos-0.0.5.tar` & `dig_ass_ocr_protos-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:12:53.894706 dig_ass_ocr_protos-0.0.5/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.5/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-05-02 11:12:53.894706 dig_ass_ocr_protos-0.0.5/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:44.000000 dig_ass_ocr_protos-0.0.5/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:12:53.894706 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1686 2024-05-02 11:12:52.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      692 2024-05-02 11:12:52.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2914 2024-05-02 11:12:52.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-02 11:11:21.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      662 2024-05-02 11:09:19.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:12:53.894706 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-05-02 11:12:53.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      498 2024-05-02 11:12:53.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-02 11:12:53.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-05-02 11:12:53.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-05-02 11:12:53.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.5/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-02 11:12:53.894706 dig_ass_ocr_protos-0.0.5/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      800 2024-05-02 11:09:19.000000 dig_ass_ocr_protos-0.0.5/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:01.440086 dig_ass_ocr_protos-0.0.6/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.6/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      369 2024-05-13 14:30:01.440086 dig_ass_ocr_protos-0.0.6/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:44.000000 dig_ass_ocr_protos-0.0.6/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:01.440086 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1686 2024-05-13 14:29:59.000000 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      692 2024-05-13 14:29:59.000000 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2914 2024-05-13 14:29:59.000000 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-13 14:27:05.000000 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      676 2024-05-13 14:05:52.000000 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:01.440086 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      369 2024-05-13 14:30:01.000000 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      498 2024-05-13 14:30:01.000000 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-13 14:30:01.000000 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-13 14:30:01.000000 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-05-13 14:30:01.000000 dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       56 2024-05-13 14:20:30.000000 dig_ass_ocr_protos-0.0.6/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-13 14:30:01.440086 dig_ass_ocr_protos-0.0.6/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      800 2024-05-02 11:09:19.000000 dig_ass_ocr_protos-0.0.6/setup.py
```

### Comparing `dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py` & `dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi` & `dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py` & `dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/client.py` & `dig_ass_ocr_protos-0.0.6/dig_ass_ocr_protos/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dig_ass_ocr_protos.DigitalAssistantOCR_pb2_grpc import DigitalAssistantOCRStub
 from dig_ass_ocr_protos.DigitalAssistantOCR_pb2 import (
     DigitalAssistantOCRRequest,
     DigitalAssistantOCRResponse,
 )
 
-from .abstract_client import AbstractClient
+
+from agi_med_utils.abstract_client import AbstractClient
 
 
 class OCRClient(AbstractClient):
     def __init__(self, address) -> None:
         super().__init__(address)
         self._stub = DigitalAssistantOCRStub(self._channel)
```

### Comparing `dig_ass_ocr_protos-0.0.5/setup.py` & `dig_ass_ocr_protos-0.0.6/setup.py`

 * *Files identical despite different names*

