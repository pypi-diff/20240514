# Comparing `tmp/dig_ass_critic_protos-1.0.0.tar.gz` & `tmp/dig_ass_critic_protos-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_critic_protos-1.0.0.tar", last modified: Thu May  2 11:13:10 2024, max compression
+gzip compressed data, was "dig_ass_critic_protos-1.0.2.tar", last modified: Mon May 13 14:30:18 2024, max compression
```

## Comparing `dig_ass_critic_protos-1.0.0.tar` & `dig_ass_critic_protos-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:10.128769 dig_ass_critic_protos-1.0.0/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_critic_protos-1.0.0/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      339 2024-05-02 11:13:10.128769 dig_ass_critic_protos-1.0.0/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:31.000000 dig_ass_critic_protos-1.0.0/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:10.128769 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2828 2024-05-02 11:13:08.000000 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2482 2024-05-02 11:13:08.000000 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3010 2024-05-02 11:13:08.000000 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1674 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:10.128769 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      339 2024-05-02 11:13:10.000000 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      540 2024-05-02 11:13:10.000000 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-02 11:13:10.000000 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-05-02 11:13:10.000000 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-02 11:13:10.000000 dig_ass_critic_protos-1.0.0/dig_ass_critic_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_critic_protos-1.0.0/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-02 11:13:10.128769 dig_ass_critic_protos-1.0.0/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      809 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.0/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:18.281465 dig_ass_critic_protos-1.0.2/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_critic_protos-1.0.2/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      375 2024-05-13 14:30:18.281465 dig_ass_critic_protos-1.0.2/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:31.000000 dig_ass_critic_protos-1.0.2/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:18.281465 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2874 2024-05-13 14:30:16.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2610 2024-05-13 14:30:16.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3010 2024-05-13 14:30:16.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-13 14:24:44.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1577 2024-05-13 14:08:18.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:18.281465 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      375 2024-05-13 14:30:18.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      540 2024-05-13 14:30:18.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-13 14:30:18.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-13 14:30:18.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-13 14:30:18.000000 dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       56 2024-05-13 14:20:34.000000 dig_ass_critic_protos-1.0.2/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-13 14:30:18.281465 dig_ass_critic_protos-1.0.2/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      809 2024-05-02 11:09:19.000000 dig_ass_critic_protos-1.0.2/setup.py
```

### Comparing `dig_ass_critic_protos-1.0.0/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py` & `dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2dig_ass_critic_protos/DigitalAssistantCritic.proto\x12\x11\x64ig.ass.critic.v1\"/\n\x1e\x44igitalAssistantCriticResponse\x12\r\n\x05Score\x18\x01 \x01(\x02\"X\n\x1d\x44igitalAssistantCriticRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12)\n\x04\x43hat\x18\x02 \x01(\x0b\x32\x1b.dig.ass.critic.v1.ChatItem\"\x80\x01\n\x08\x43hatItem\x12\x39\n\x0cOuterContext\x18\x01 \x01(\x0b\x32#.dig.ass.critic.v1.OuterContextItem\x12\x39\n\x0cInnerContext\x18\x02 \x01(\x0b\x32#.dig.ass.critic.v1.InnerContextItem\"a\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\t\x12\x11\n\tSessionId\x18\x04 \x01(\t\x12\x10\n\x08\x43lientId\x18\x05 \x01(\t\"D\n\x10InnerContextItem\x12\x30\n\x08Replicas\x18\x01 \x03(\x0b\x32\x1e.dig.ass.critic.v1.ReplicaItem\";\n\x0bReplicaItem\x12\x0c\n\x04\x42ody\x18\x01 \x01(\t\x12\x0c\n\x04Role\x18\x02 \x01(\x08\x12\x10\n\x08\x44\x61teTime\x18\x03 \x01(\t2\x90\x01\n\x16\x44igitalAssistantCritic\x12v\n\x0fGetTextResponse\x12\x30.dig.ass.critic.v1.DigitalAssistantCriticRequest\x1a\x31.dig.ass.critic.v1.DigitalAssistantCriticResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2dig_ass_critic_protos/DigitalAssistantCritic.proto\x12\x11\x64ig.ass.critic.v1\"/\n\x1e\x44igitalAssistantCriticResponse\x12\r\n\x05Score\x18\x01 \x01(\x02\"X\n\x1d\x44igitalAssistantCriticRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12)\n\x04\x43hat\x18\x02 \x01(\x0b\x32\x1b.dig.ass.critic.v1.ChatItem\"\x80\x01\n\x08\x43hatItem\x12\x39\n\x0cOuterContext\x18\x01 \x01(\x0b\x32#.dig.ass.critic.v1.OuterContextItem\x12\x39\n\x0cInnerContext\x18\x02 \x01(\x0b\x32#.dig.ass.critic.v1.InnerContextItem\"a\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\t\x12\x11\n\tSessionId\x18\x04 \x01(\t\x12\x10\n\x08\x43lientId\x18\x05 \x01(\t\"D\n\x10InnerContextItem\x12\x30\n\x08Replicas\x18\x01 \x03(\x0b\x32\x1e.dig.ass.critic.v1.ReplicaItem\"R\n\x0bReplicaItem\x12\x0c\n\x04\x42ody\x18\x01 \x01(\t\x12\x0c\n\x04Role\x18\x02 \x01(\x08\x12\x10\n\x08\x44\x61teTime\x18\x03 \x01(\t\x12\x15\n\rPreviousScore\x18\x04 \x01(\x02\x32\x90\x01\n\x16\x44igitalAssistantCritic\x12v\n\x0fGetTextResponse\x12\x30.dig.ass.critic.v1.DigitalAssistantCriticRequest\x1a\x31.dig.ass.critic.v1.DigitalAssistantCriticResponseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dig_ass_critic_protos.DigitalAssistantCritic_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_DIGITALASSISTANTCRITICRESPONSE']._serialized_start=73
@@ -28,11 +28,11 @@
   _globals['_CHATITEM']._serialized_start=213
   _globals['_CHATITEM']._serialized_end=341
   _globals['_OUTERCONTEXTITEM']._serialized_start=343
   _globals['_OUTERCONTEXTITEM']._serialized_end=440
   _globals['_INNERCONTEXTITEM']._serialized_start=442
   _globals['_INNERCONTEXTITEM']._serialized_end=510
   _globals['_REPLICAITEM']._serialized_start=512
-  _globals['_REPLICAITEM']._serialized_end=571
-  _globals['_DIGITALASSISTANTCRITIC']._serialized_start=574
-  _globals['_DIGITALASSISTANTCRITIC']._serialized_end=718
+  _globals['_REPLICAITEM']._serialized_end=594
+  _globals['_DIGITALASSISTANTCRITIC']._serialized_start=597
+  _globals['_DIGITALASSISTANTCRITIC']._serialized_end=741
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dig_ass_critic_protos-1.0.0/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi` & `dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 class InnerContextItem(_message.Message):
     __slots__ = ("Replicas",)
     REPLICAS_FIELD_NUMBER: _ClassVar[int]
     Replicas: _containers.RepeatedCompositeFieldContainer[ReplicaItem]
     def __init__(self, Replicas: _Optional[_Iterable[_Union[ReplicaItem, _Mapping]]] = ...) -> None: ...
 
 class ReplicaItem(_message.Message):
-    __slots__ = ("Body", "Role", "DateTime")
+    __slots__ = ("Body", "Role", "DateTime", "PreviousScore")
     BODY_FIELD_NUMBER: _ClassVar[int]
     ROLE_FIELD_NUMBER: _ClassVar[int]
     DATETIME_FIELD_NUMBER: _ClassVar[int]
+    PREVIOUSSCORE_FIELD_NUMBER: _ClassVar[int]
     Body: str
     Role: bool
     DateTime: str
-    def __init__(self, Body: _Optional[str] = ..., Role: bool = ..., DateTime: _Optional[str] = ...) -> None: ...
+    PreviousScore: float
+    def __init__(self, Body: _Optional[str] = ..., Role: bool = ..., DateTime: _Optional[str] = ..., PreviousScore: _Optional[float] = ...) -> None: ...
```

### Comparing `dig_ass_critic_protos-1.0.0/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py` & `dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-1.0.0/dig_ass_critic_protos/client.py` & `dig_ass_critic_protos-1.0.2/dig_ass_critic_protos/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     DigitalAssistantCriticResponse,
     ChatItem,
     OuterContextItem,
     InnerContextItem,
     ReplicaItem,
 )
 
-from .abstract_client import AbstractClient
+from agi_med_utils.abstract_client import AbstractClient
 
 
 class CriticClient(AbstractClient):
     def __init__(self, address) -> None:
         super().__init__(address)
         self._stub = DigitalAssistantCriticStub(self._channel)
 
@@ -27,24 +27,15 @@
                 OuterContext=OuterContextItem(
                     Sex=outer_context['Sex'],
                     Age=outer_context['Age'],
                     UserId=outer_context['UserId'],
                     SessionId=outer_context['SessionId'],
                     ClientId=outer_context['ClientId'],
                 ),
-                InnerContext=InnerContextItem(
-                    Replicas=[
-                        self.rep_to_obj(replica)
-                        for replica in inner_context['Replicas']
-                    ]
-                ),
+                InnerContext=InnerContextItem(Replicas=[self.rep_to_obj(replica) for replica in inner_context['Replicas']]),
             ),
         )
         response: DigitalAssistantCriticResponse = self._stub.GetTextResponse(request)
         return response.Score
 
     def rep_to_obj(self, replica_dict):
-        return ReplicaItem(
-            Body=replica_dict['Body'],
-            Role=replica_dict['Role'],
-            DateTime=replica_dict['DateTime'],
-        )
+        return ReplicaItem(Body=replica_dict['Body'], Role=replica_dict['Role'], DateTime=replica_dict['DateTime'], PreviousScore=replica_dict['PreviousScore'])
```

### Comparing `dig_ass_critic_protos-1.0.0/dig_ass_critic_protos.egg-info/SOURCES.txt` & `dig_ass_critic_protos-1.0.2/dig_ass_critic_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-1.0.0/setup.py` & `dig_ass_critic_protos-1.0.2/setup.py`

 * *Files identical despite different names*

