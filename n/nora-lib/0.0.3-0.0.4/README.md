# Comparing `tmp/nora_lib-0.0.3.tar.gz` & `tmp/nora_lib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nora_lib-0.0.3.tar", last modified: Thu May  9 17:33:47 2024, max compression
+gzip compressed data, was "nora_lib-0.0.4.tar", last modified: Tue May 14 16:13:39 2024, max compression
```

## Comparing `nora_lib-0.0.3.tar` & `nora_lib-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.362088 nora_lib-0.0.3/
--rw-r--r--   0 reganh     (502) staff       (20)      407 2024-05-09 17:33:47.361834 nora_lib-0.0.3/PKG-INFO
--rw-r--r--   0 reganh     (502) staff       (20)      887 2024-05-09 17:31:43.000000 nora_lib-0.0.3/README.md
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.356611 nora_lib-0.0.3/nora_lib/
--rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.3/nora_lib/__init__.py
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.358215 nora_lib-0.0.3/nora_lib/context/
--rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-09 17:26:38.000000 nora_lib-0.0.3/nora_lib/context/__init__.py
--rw-r--r--   0 reganh     (502) staff       (20)     3130 2024-05-09 17:26:38.000000 nora_lib-0.0.3/nora_lib/context/context_service.py
--rw-r--r--   0 reganh     (502) staff       (20)      757 2024-05-09 17:26:38.000000 nora_lib-0.0.3/nora_lib/context/models.py
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.358715 nora_lib-0.0.3/nora_lib/interactions/
--rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-09 17:26:38.000000 nora_lib-0.0.3/nora_lib/interactions/__init__.py
--rw-r--r--   0 reganh     (502) staff       (20)     4163 2024-05-09 17:26:38.000000 nora_lib-0.0.3/nora_lib/interactions/interactions_service.py
--rw-r--r--   0 reganh     (502) staff       (20)     3377 2024-05-09 17:26:38.000000 nora_lib-0.0.3/nora_lib/interactions/models.py
--rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.3/nora_lib/py.typed
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.359171 nora_lib-0.0.3/nora_lib/tasks/
--rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.3/nora_lib/tasks/__init__.py
--rw-r--r--   0 reganh     (502) staff       (20)      925 2024-05-03 17:18:14.000000 nora_lib-0.0.3/nora_lib/tasks/models.py
--rw-r--r--   0 reganh     (502) staff       (20)     1793 2024-05-03 17:18:14.000000 nora_lib-0.0.3/nora_lib/tasks/state.py
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.361256 nora_lib-0.0.3/nora_lib.egg-info/
--rw-r--r--   0 reganh     (502) staff       (20)      407 2024-05-09 17:33:47.000000 nora_lib-0.0.3/nora_lib.egg-info/PKG-INFO
--rw-r--r--   0 reganh     (502) staff       (20)      587 2024-05-09 17:33:47.000000 nora_lib-0.0.3/nora_lib.egg-info/SOURCES.txt
--rw-r--r--   0 reganh     (502) staff       (20)        1 2024-05-09 17:33:47.000000 nora_lib-0.0.3/nora_lib.egg-info/dependency_links.txt
--rw-r--r--   0 reganh     (502) staff       (20)       64 2024-05-09 17:33:47.000000 nora_lib-0.0.3/nora_lib.egg-info/requires.txt
--rw-r--r--   0 reganh     (502) staff       (20)       15 2024-05-09 17:33:47.000000 nora_lib-0.0.3/nora_lib.egg-info/top_level.txt
--rw-r--r--   0 reganh     (502) staff       (20)       90 2024-05-03 17:18:14.000000 nora_lib-0.0.3/pyproject.toml
--rw-r--r--   0 reganh     (502) staff       (20)       38 2024-05-09 17:33:47.362140 nora_lib-0.0.3/setup.cfg
--rw-r--r--   0 reganh     (502) staff       (20)      600 2024-05-09 17:29:40.000000 nora_lib-0.0.3/setup.py
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.359344 nora_lib-0.0.3/tests/
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.359876 nora_lib-0.0.3/tests/tasks/
--rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.3/tests/tasks/__init__.py
--rw-r--r--   0 reganh     (502) staff       (20)     2670 2024-05-03 17:18:14.000000 nora_lib-0.0.3/tests/tasks/test_state.py
--rw-r--r--   0 reganh     (502) staff       (20)      123 2024-05-03 17:18:14.000000 nora_lib-0.0.3/tests/test_placeholder.py
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.274597 nora_lib-0.0.4/
+-rw-r--r--   0 reganh     (502) staff       (20)      407 2024-05-14 16:13:39.274310 nora_lib-0.0.4/PKG-INFO
+-rw-r--r--   0 reganh     (502) staff       (20)      887 2024-05-09 17:31:43.000000 nora_lib-0.0.4/README.md
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.265471 nora_lib-0.0.4/nora_lib/
+-rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.4/nora_lib/__init__.py
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.267147 nora_lib-0.0.4/nora_lib/context/
+-rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-09 17:26:38.000000 nora_lib-0.0.4/nora_lib/context/__init__.py
+-rw-r--r--   0 reganh     (502) staff       (20)     3390 2024-05-14 16:12:32.000000 nora_lib-0.0.4/nora_lib/context/context_service.py
+-rw-r--r--   0 reganh     (502) staff       (20)      757 2024-05-09 17:26:38.000000 nora_lib-0.0.4/nora_lib/context/models.py
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.271911 nora_lib-0.0.4/nora_lib/interactions/
+-rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-09 17:26:38.000000 nora_lib-0.0.4/nora_lib/interactions/__init__.py
+-rw-r--r--   0 reganh     (502) staff       (20)     4731 2024-05-14 16:12:32.000000 nora_lib-0.0.4/nora_lib/interactions/interactions_service.py
+-rw-r--r--   0 reganh     (502) staff       (20)     3381 2024-05-14 16:12:32.000000 nora_lib-0.0.4/nora_lib/interactions/models.py
+-rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.4/nora_lib/py.typed
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.272604 nora_lib-0.0.4/nora_lib/tasks/
+-rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.4/nora_lib/tasks/__init__.py
+-rw-r--r--   0 reganh     (502) staff       (20)      925 2024-05-03 17:18:14.000000 nora_lib-0.0.4/nora_lib/tasks/models.py
+-rw-r--r--   0 reganh     (502) staff       (20)     1793 2024-05-03 17:18:14.000000 nora_lib-0.0.4/nora_lib/tasks/state.py
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.273778 nora_lib-0.0.4/nora_lib.egg-info/
+-rw-r--r--   0 reganh     (502) staff       (20)      407 2024-05-14 16:13:39.000000 nora_lib-0.0.4/nora_lib.egg-info/PKG-INFO
+-rw-r--r--   0 reganh     (502) staff       (20)      587 2024-05-14 16:13:39.000000 nora_lib-0.0.4/nora_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 reganh     (502) staff       (20)        1 2024-05-14 16:13:39.000000 nora_lib-0.0.4/nora_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 reganh     (502) staff       (20)       64 2024-05-14 16:13:39.000000 nora_lib-0.0.4/nora_lib.egg-info/requires.txt
+-rw-r--r--   0 reganh     (502) staff       (20)       15 2024-05-14 16:13:39.000000 nora_lib-0.0.4/nora_lib.egg-info/top_level.txt
+-rw-r--r--   0 reganh     (502) staff       (20)       90 2024-05-03 17:18:14.000000 nora_lib-0.0.4/pyproject.toml
+-rw-r--r--   0 reganh     (502) staff       (20)       38 2024-05-14 16:13:39.274659 nora_lib-0.0.4/setup.cfg
+-rw-r--r--   0 reganh     (502) staff       (20)      600 2024-05-14 16:12:32.000000 nora_lib-0.0.4/setup.py
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.272794 nora_lib-0.0.4/tests/
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.273115 nora_lib-0.0.4/tests/tasks/
+-rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.4/tests/tasks/__init__.py
+-rw-r--r--   0 reganh     (502) staff       (20)     2670 2024-05-03 17:18:14.000000 nora_lib-0.0.4/tests/tasks/test_state.py
+-rw-r--r--   0 reganh     (502) staff       (20)      123 2024-05-03 17:18:14.000000 nora_lib-0.0.4/tests/test_placeholder.py
```

### Comparing `nora_lib-0.0.3/README.md` & `nora_lib-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.3/nora_lib/context/context_service.py` & `nora_lib-0.0.4/nora_lib/context/context_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,21 @@
             interactions_base_url, interactions_bearer_token, timeout
         )
         self.agent_actor_id = agent_actor_id
 
     def _get_interactions_service(self, url, token, timeout) -> InteractionsService:
         return InteractionsService(url, timeout, token)
 
+    def get_message(self, message_id: str) -> str:
+        message: ReturnedMessage = self.interactions_service.get_message(message_id)
+        if message.annotated_text:
+            return message.annotated_text
+        else:
+            return message.text
+
     def fetch_context(
         self, request: WrappedTaskObject
     ) -> List[ReturnedAgentContextMessage]:
         message_id = request.message_id
 
         returned_messages: List[ReturnedMessage] = (
             self.interactions_service.fetch_messages_and_events_for_forked_thread(
```

### Comparing `nora_lib-0.0.3/nora_lib/context/models.py` & `nora_lib-0.0.4/nora_lib/context/models.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.3/nora_lib/interactions/interactions_service.py` & `nora_lib-0.0.4/nora_lib/interactions/interactions_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,14 +29,31 @@
             event_url,
             json=event.model_dump(),
             headers=self.headers,
             timeout=int(self.timeout),
         )
         response.raise_for_status()
 
+    def get_message(self, message_id: str) -> ReturnedMessage:
+        """Fetch a message from the Interactions API"""
+        message_url = f"{self.base_url}/interaction/v1/search/message"
+        request_body = {
+            "id": message_id,
+        }
+        response = requests.post(
+            message_url,
+            json=request_body,
+            headers=self.headers,
+            timeout=int(self.timeout),
+        )
+        response.raise_for_status()
+        res_dict = response.json()["message"]
+
+        return ReturnedMessage.model_validate(res_dict)
+
     def fetch_thread_messages_and_events_for_message(
         self, message_id: str, event_type: str
     ) -> ThreadRelationsResponse:
         """Fetch messages and associated events from the same thread as provided messagev id"""
         message_url = f"{self.base_url}/interaction/v1/search/message"
         request_body = thread_message_lookup_request(message_id, event_type=event_type)
         response = requests.post(
```

### Comparing `nora_lib-0.0.3/nora_lib/interactions/models.py` & `nora_lib-0.0.4/nora_lib/interactions/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Model for interactions to be sent to the interactions service.
 """
 
 from datetime import datetime
 from enum import Enum
-from typing import Optional, List
+from typing import Dict, List, Optional, Tuple
 from uuid import UUID
 
-from pydantic import BaseModel, Field, field_serializer
+from pydantic import BaseModel, Field, field_serializer, ConfigDict
 
 
 class EventType(str, Enum):
     """Event types for the interactions service"""
 
     AGENT_CONTEXT = "agent:message_context"
     THREAD_FORK = "thread_fork"
@@ -36,14 +36,25 @@
         return str(actor_id)
 
     @field_serializer("timestamp")
     def serialize_timestamp(self, timestamp: datetime):
         return timestamp.isoformat()
 
 
+class ReturnedMessage(BaseModel):
+    """Message format returned by interaction service"""
+
+    message_id: str
+    actor_id: str
+    text: str
+    ts: str
+    annotated_text: Optional[str] = None
+    events: Optional[List[dict]] = None
+
+
 class AgentMessageData(BaseModel):
     """capture requests to and responses from tools within Events"""
 
     message_data: dict  # dict of agent/tool request/response format
     data_sender_actor_id: Optional[str] = None  # agent sending the data
     virtual_thread_id: Optional[str] = None  # tool-provided thread
     tool_call_id: Optional[str] = None  # llm-provided thread
@@ -72,25 +83,14 @@
 
 class ThreadForkEventData(BaseModel):
     """Event data for a thread fork event"""
 
     previous_message_id: str
 
 
-class ReturnedMessage(BaseModel):
-    """Message format returned by interaction service for search by thread"""
-
-    message_id: str
-    actor_id: str
-    text: str
-    ts: str
-    annotated_text: Optional[str] = None
-    events: Optional[List[dict]] = None
-
-
 class ThreadRelationsResponse(BaseModel):
     """Thread format returned by interaction service for thread relations in a search response"""
 
     thread_id: str
     events: Optional[List[Event]] = None  # events associated only with the thread
     messages: Optional[List[ReturnedMessage]] = (
         None  # includes events associated with each message
```

### Comparing `nora_lib-0.0.3/nora_lib/tasks/models.py` & `nora_lib-0.0.4/nora_lib/tasks/models.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.3/nora_lib/tasks/state.py` & `nora_lib-0.0.4/nora_lib/tasks/state.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.3/nora_lib.egg-info/SOURCES.txt` & `nora_lib-0.0.4/nora_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.3/setup.py` & `nora_lib-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 runtime_requirements = ["pydantic>=2,<3", "requests"]
 
 # For running tests, linting, etc
 dev_requirements = ["mypy", "pytest", "black", "types-requests"]
 
 setuptools.setup(
     name="nora_lib",
-    version="0.0.3",
+    version="0.0.4",
     description="For making and coordinating agents and tools",
     url="https://github.com/allenai/nora_lib",
     packages=setuptools.find_packages(exclude=(["tests"])),
     install_requires=runtime_requirements,
     package_data={
         "nora_lib": ["py.typed"],
     },
```

### Comparing `nora_lib-0.0.3/tests/tasks/test_state.py` & `nora_lib-0.0.4/tests/tasks/test_state.py`

 * *Files identical despite different names*

