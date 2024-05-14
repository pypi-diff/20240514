# Comparing `tmp/deltafi-2.0rc1714076410617.tar.gz` & `tmp/deltafi-2.0rc1715691282958.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-2.0rc1714076410617.tar", max compression
+gzip compressed data, was "deltafi-2.0rc1715691282958.tar", max compression
```

## Comparing `deltafi-2.0rc1714076410617.tar` & `deltafi-2.0rc1715691282958.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-2.0rc1714076410617/README.md
--rw-r--r--   0        0        0      709 2023-09-08 11:24:47.608536 deltafi-2.0rc1714076410617/deltafi/__init__.py
--rw-r--r--   0        0        0     5323 2024-04-25 20:19:24.267191 deltafi-2.0rc1714076410617/deltafi/action.py
--rw-r--r--   0        0        0     2847 2023-10-13 13:53:29.360657 deltafi-2.0rc1714076410617/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      865 2024-04-25 20:19:24.267191 deltafi-2.0rc1714076410617/deltafi/actiontype.py
--rw-r--r--   0        0        0    11301 2024-04-25 20:19:24.267191 deltafi-2.0rc1714076410617/deltafi/domain.py
--rw-r--r--   0        0        0      943 2024-04-25 20:19:24.267191 deltafi-2.0rc1714076410617/deltafi/exception.py
--rw-r--r--   0        0        0     1090 2023-11-16 03:01:54.189409 deltafi-2.0rc1714076410617/deltafi/genericmodel.py
--rw-r--r--   0        0        0     1656 2024-04-25 20:19:24.268191 deltafi-2.0rc1714076410617/deltafi/input.py
--rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-2.0rc1714076410617/deltafi/logger.py
--rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-2.0rc1714076410617/deltafi/metric.py
--rw-r--r--   0        0        0    12294 2024-04-25 20:19:24.268191 deltafi-2.0rc1714076410617/deltafi/plugin.py
--rw-r--r--   0        0        0     8177 2024-04-25 20:19:24.268191 deltafi-2.0rc1714076410617/deltafi/result.py
--rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-2.0rc1714076410617/deltafi/storage.py
--rw-r--r--   0        0        0      709 2023-09-08 11:24:47.609536 deltafi-2.0rc1714076410617/deltafi/test_kit/__init__.py
--rw-r--r--   0        0        0     1378 2023-09-08 11:24:47.609536 deltafi-2.0rc1714076410617/deltafi/test_kit/assertions.py
--rw-r--r--   0        0        0    12178 2024-04-25 20:19:24.268191 deltafi-2.0rc1714076410617/deltafi/test_kit/compare_helpers.py
--rw-r--r--   0        0        0      833 2023-08-07 14:10:09.593662 deltafi-2.0rc1714076410617/deltafi/test_kit/constants.py
--rw-r--r--   0        0        0     2090 2024-01-26 17:47:35.400662 deltafi-2.0rc1714076410617/deltafi/test_kit/domain.py
--rw-r--r--   0        0        0     1899 2024-01-26 17:47:35.400662 deltafi-2.0rc1714076410617/deltafi/test_kit/egress.py
--rw-r--r--   0        0        0     2587 2024-01-26 17:47:35.400662 deltafi-2.0rc1714076410617/deltafi/test_kit/enrich.py
--rw-r--r--   0        0        0    14602 2024-04-25 20:19:24.269191 deltafi-2.0rc1714076410617/deltafi/test_kit/framework.py
--rw-r--r--   0        0        0     4085 2024-04-25 20:19:24.269191 deltafi-2.0rc1714076410617/deltafi/test_kit/transform.py
--rw-r--r--   0        0        0     1933 2024-01-26 17:47:35.408662 deltafi-2.0rc1714076410617/deltafi/test_kit/validate.py
--rw-r--r--   0        0        0     1310 2024-04-25 20:20:40.177429 deltafi-2.0rc1714076410617/pyproject.toml
--rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 deltafi-2.0rc1714076410617/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-08-18 19:46:59.247988 deltafi-2.0rc1715691282958/README.md
+-rw-r--r--   0        0        0      709 2023-10-18 22:01:21.233230 deltafi-2.0rc1715691282958/deltafi/__init__.py
+-rw-r--r--   0        0        0     5343 2024-05-09 17:57:35.270646 deltafi-2.0rc1715691282958/deltafi/action.py
+-rw-r--r--   0        0        0     2847 2023-10-18 22:01:21.233230 deltafi-2.0rc1715691282958/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      913 2024-05-09 17:57:35.293647 deltafi-2.0rc1715691282958/deltafi/actiontype.py
+-rw-r--r--   0        0        0    12112 2024-05-09 17:57:35.320649 deltafi-2.0rc1715691282958/deltafi/domain.py
+-rw-r--r--   0        0        0      943 2024-05-09 17:57:35.330650 deltafi-2.0rc1715691282958/deltafi/exception.py
+-rw-r--r--   0        0        0     1090 2023-11-15 21:51:57.337445 deltafi-2.0rc1715691282958/deltafi/genericmodel.py
+-rw-r--r--   0        0        0     1656 2024-05-09 17:57:35.343650 deltafi-2.0rc1715691282958/deltafi/input.py
+-rw-r--r--   0        0        0     2136 2023-08-18 19:46:59.249988 deltafi-2.0rc1715691282958/deltafi/logger.py
+-rw-r--r--   0        0        0      967 2023-08-18 19:46:59.249988 deltafi-2.0rc1715691282958/deltafi/metric.py
+-rw-r--r--   0        0        0    12422 2024-05-09 17:57:35.361652 deltafi-2.0rc1715691282958/deltafi/plugin.py
+-rw-r--r--   0        0        0     8210 2024-05-09 17:57:35.385653 deltafi-2.0rc1715691282958/deltafi/result.py
+-rw-r--r--   0        0        0     2740 2023-08-18 19:46:59.249988 deltafi-2.0rc1715691282958/deltafi/storage.py
+-rw-r--r--   0        0        0      709 2023-10-18 22:01:21.234230 deltafi-2.0rc1715691282958/deltafi/test_kit/__init__.py
+-rw-r--r--   0        0        0     1378 2023-10-18 22:01:21.235230 deltafi-2.0rc1715691282958/deltafi/test_kit/assertions.py
+-rw-r--r--   0        0        0    12957 2024-05-13 20:31:46.468118 deltafi-2.0rc1715691282958/deltafi/test_kit/compare_helpers.py
+-rw-r--r--   0        0        0      833 2023-10-18 22:01:21.235230 deltafi-2.0rc1715691282958/deltafi/test_kit/constants.py
+-rw-r--r--   0        0        0     2090 2024-01-24 00:43:35.834381 deltafi-2.0rc1715691282958/deltafi/test_kit/domain.py
+-rw-r--r--   0        0        0     1899 2024-01-17 20:15:36.113816 deltafi-2.0rc1715691282958/deltafi/test_kit/egress.py
+-rw-r--r--   0        0        0     2587 2024-01-24 00:43:35.834381 deltafi-2.0rc1715691282958/deltafi/test_kit/enrich.py
+-rw-r--r--   0        0        0    13033 2024-05-09 17:57:35.386653 deltafi-2.0rc1715691282958/deltafi/test_kit/framework.py
+-rw-r--r--   0        0        0     4085 2024-05-09 17:57:35.387653 deltafi-2.0rc1715691282958/deltafi/test_kit/transform.py
+-rw-r--r--   0        0        0     1933 2024-01-24 00:43:35.836381 deltafi-2.0rc1715691282958/deltafi/test_kit/validate.py
+-rw-r--r--   0        0        0     1310 2024-05-14 12:55:12.823647 deltafi-2.0rc1715691282958/pyproject.toml
+-rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 deltafi-2.0rc1715691282958/PKG-INFO
```

### Comparing `deltafi-2.0rc1714076410617/deltafi/__init__.py` & `deltafi-2.0rc1715691282958/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/action.py` & `deltafi-2.0rc1715691282958/deltafi/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 #    limitations under the License.
 #
 
 from abc import ABC, abstractmethod
 from typing import Any, List
 
 from deltafi.actiontype import ActionType
-from deltafi.genericmodel import GenericModel
 from deltafi.domain import Context, DeltaFileMessage
+from deltafi.genericmodel import GenericModel
 from deltafi.input import EgressInput, TransformInput
 from deltafi.result import *
 from pydantic import BaseModel
 
 
 class Action(ABC):
     def __init__(self, action_type: ActionType, description: str, valid_result_types: tuple):
@@ -44,28 +44,31 @@
     @abstractmethod
     def execute(self, context: Context, action_input: Any, params: BaseModel):
         pass
 
     def execute_action(self, event):
         if event.delta_file_messages is None or not len(event.delta_file_messages):
             raise RuntimeError(f"Received event with no delta file messages for did {event.context.did}")
-
         if event.context.collect is not None:
-            result = self.execute(event.context, self.collect([self.build_input(event.context, delta_file_message)
-                                                               for delta_file_message in event.delta_file_messages]),
-                                  self.param_class().model_validate(event.params))
+            result = self.execute(
+                event.context,
+                self.collect([self.build_input(event.context, delta_file_message)
+                              for delta_file_message in event.delta_file_messages]),
+                self.param_class().model_validate(event.params))
         else:
-            result = self.execute(event.context, self.build_input(event.context, event.delta_file_messages[0]),
-                                  self.param_class().model_validate(event.params))
+            result = self.execute(
+                event.context,
+                self.build_input(event.context, event.delta_file_messages[0]),
+                self.param_class().model_validate(event.params))
 
         self.validate_type(result)
         return result
 
     @staticmethod
-    def param_class( ):
+    def param_class():
         """Factory method to create and return an empty GenericModel instance.
 
         Returns
         -------
         GenericModel
             an empty GenericModel instance
         """
@@ -106,15 +109,16 @@
 
     def execute(self, context: Context, input_placeholder: Any, params: BaseModel):
         return self.ingress(context, params)
 
 
 class TransformAction(Action, ABC):
     def __init__(self, description: str):
-        super().__init__(ActionType.TRANSFORM, description, (TransformResult, TransformResults, ErrorResult, FilterResult))
+        super().__init__(ActionType.TRANSFORM, description,
+                         (TransformResult, TransformResults, ErrorResult, FilterResult))
 
     def build_input(self, context: Context, delta_file_message: DeltaFileMessage):
         return TransformInput(content=delta_file_message.content_list, metadata=delta_file_message.metadata)
 
     def collect(self, transform_inputs: List[TransformInput]):
         all_content = []
         all_metadata = {}
```

### Comparing `deltafi-2.0rc1714076410617/deltafi/actioneventqueue.py` & `deltafi-2.0rc1715691282958/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/actiontype.py` & `deltafi-2.0rc1715691282958/deltafi/actiontype.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,11 +16,13 @@
 #    limitations under the License.
 #
 
 from enum import Enum
 
 
 class ActionType(Enum):
+    INGRESS = "INGRESS"
     TIMED_INGRESS = "TIMED_INGRESS"
     TRANSFORM = "TRANSFORM"
     EGRESS = "EGRESS"
+    PUBLISH = "PUBLISH"
     UNKNOWN = "UNKNOWN"
```

### Comparing `deltafi-2.0rc1714076410617/deltafi/domain.py` & `deltafi-2.0rc1715691282958/deltafi/domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,67 +36,95 @@
     @property
     def key(self) -> str:
         return f"{self.clazz}:{self.action}:{self.did}"
 
 
 class Context(NamedTuple):
     did: str
-    action_flow: str
+    delta_file_name: str
+    data_source: str
+    flow_name: str
+    flow_id: str
     action_name: str
-    source_filename: str
-    ingress_flow: str
-    egress_flow: str
-    system: str
+    action_id: str
+    action_version: str
     hostname: str
+    system_name: str
     content_service: ContentService
     collect: dict = None
     collected_dids: List[str] = None
     memo: str = None
     logger: Logger = None
 
     @classmethod
     def create(cls, context: dict, hostname: str, content_service: ContentService, logger: Logger):
         did = context['did']
-        action_name_parts = context['name'].split(".")
-        action_flow = action_name_parts[0]
-        action_name = action_name_parts[1]
-        if 'sourceFilename' in context:
-            source_filename = context['sourceFilename']
-        else:
-            source_filename = None
-        ingress_flow = context['ingressFlow']
-        if 'egressFlow' in context:
-            egress_flow = context['egressFlow']
+        if 'deltaFileName' in context:
+            delta_file_name = context['deltaFileName']
         else:
-            egress_flow = None
-        system = context['systemName']
+            delta_file_name = None
+        if 'dataSource' in context:
+            data_source = context['dataSource']
+        else:
+            data_source = None
+        if 'flowName' in context:
+            flow_name = context['flowName']
+        else:
+            flow_name = None
+        if 'flowId' in context:
+            flow_id = context['flowId']
+        else:
+            flow_id = None
+        if 'actionName' in context:
+            action_name = context['actionName']
+        else:
+            action_name = None
+        if 'actionId' in context:
+            action_id = context['actionId']
+        else:
+            action_id = None
+        if 'actionVersion' in context:
+            action_version = context['actionVersion']
+        else:
+            action_version = None
+        if 'hostname' in context:
+            hostname = context['hostname']
+        else:
+            hostname = None
+        if 'systemName' in context:
+            system_name = context['systemName']
+        else:
+            system_name = None
         if 'collect' in context:
             collect = context['collect']
         else:
             collect = None
         if 'collectedDids' in context:
             collected_dids = context['collectedDids']
         else:
             collected_dids = None
         if 'memo' in context:
             memo = context['memo']
         else:
             memo = None
+
         return Context(did=did,
-                       action_flow=action_flow,
+                       delta_file_name=delta_file_name,
+                       data_source=data_source,
+                       flow_name=flow_name,
+                       flow_id=flow_id,
                        action_name=action_name,
-                       source_filename=source_filename,
-                       ingress_flow=ingress_flow,
-                       egress_flow=egress_flow,
-                       system=system,
+                       action_id=action_id,
+                       action_version=action_version,
                        hostname=hostname,
-                       content_service=content_service,
+                       system_name=system_name,
                        collect=collect,
                        collected_dids=collected_dids,
                        memo=memo,
+                       content_service=content_service,
                        logger=logger)
 
 
 class Content:
     """
     A Content class that holds information about a piece of content, including its name, segments, mediaType, and service.
     Attributes:
@@ -193,15 +221,14 @@
             size_remaining -= segment.size
             new_segments.append(segment)
             if size_remaining == 0:
                 break
 
         return new_segments
 
-
     def get_size(self):
         """
         Returns the size of the content in bytes.
 
         Returns:
             int: The size of the content in bytes.
         """
@@ -314,15 +341,16 @@
     context: Context
     params: dict
     queue_name: str
     return_address: str
 
     @classmethod
     def create(cls, event: dict, hostname: str, content_service: ContentService, logger: Logger):
-        delta_file_messages = [DeltaFileMessage.from_dict(delta_file_message, content_service) for delta_file_message in event['deltaFileMessages']]
+        delta_file_messages = [DeltaFileMessage.from_dict(delta_file_message, content_service) for delta_file_message in
+                               event['deltaFileMessages']]
         context = Context.create(event['actionContext'], hostname, content_service, logger)
         params = event['actionParams']
         queue_name = None
         if 'queueName' in event:
             queue_name = event['queueName']
         return_address = None
         if 'returnAddress' in event:
```

### Comparing `deltafi-2.0rc1714076410617/deltafi/exception.py` & `deltafi-2.0rc1715691282958/deltafi/exception.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/genericmodel.py` & `deltafi-2.0rc1715691282958/deltafi/genericmodel.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/input.py` & `deltafi-2.0rc1715691282958/deltafi/input.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/logger.py` & `deltafi-2.0rc1715691282958/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/metric.py` & `deltafi-2.0rc1715691282958/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/plugin.py` & `deltafi-2.0rc1715691282958/deltafi/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 
 
 def _coordinates():
     return PluginCoordinates(os.getenv('PROJECT_GROUP'), os.getenv('PROJECT_NAME'), os.getenv('PROJECT_VERSION'))
 
 
 def _setup_queue(max_connections):
-    redis_url = os.getenv('REDIS_URL', 'http://deltafi-redis-master:6379')
-    password = os.getenv('REDIS_PASSWORD')
-    return ActionEventQueue(redis_url, max_connections, password)
+    url = os.getenv('VALKEY_URL', 'http://deltafi-valkey-master:6379')
+    password = os.getenv('VALKEY_PASSWORD')
+    return ActionEventQueue(url, max_connections, password)
 
 
 def _setup_content_service():
     minio_url = os.getenv('MINIO_URL', 'http://deltafi-minio:9000')
     return ContentService(minio_url,
                           os.getenv('MINIO_ACCESSKEY'),
                           os.getenv('MINIO_SECRETKEY'))
@@ -282,15 +282,18 @@
                     result = ErrorResult(event.context,
                                          f"Action execution {type(e)} exception", f"{str(e)}\n{traceback.format_exc()}")
 
                 action.action_execution = None
 
                 response = {
                     'did': event.context.did,
-                    'action': event.context.action_flow + "." + event.context.action_name,
+                    'flowName': event.context.flow_name,
+                    'flowId': event.context.flow_id,
+                    'actionName': event.context.action_name,
+                    'actionId': event.context.action_id,
                     'start': start_time,
                     'stop': time.time(),
                     'type': result.result_type,
                     'metrics': [metric.json() for metric in result.metrics]
                 }
                 if result.result_key is not None:
                     response[result.result_key] = result.response()
```

### Comparing `deltafi-2.0rc1714076410617/deltafi/result.py` & `deltafi-2.0rc1715691282958/deltafi/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,20 +92,20 @@
             'message': self.filtered_cause,
             'context': self.filtered_context,
             'annotations': self.annotations
         }
 
 
 class IngressResultItem:
-    def __init__(self, context: Context, filename: str):
+    def __init__(self, context: Context, delta_file_name: str):
         self.context = context
-        self.filename = filename
         self._did = str(uuid.uuid4())
         self.content = []
         self.metadata = {}
+        self.delta_file_name = delta_file_name
 
     @property
     def did(self):
         return self._did
 
     # content can be a single Content or a List[Content]
     def add_content(self, content):
@@ -136,15 +136,15 @@
     def add_metadata(self, key: str, value: str):
         self.metadata[key] = value
         return self
 
     def response(self):
         return {
             'did': self._did,
-            'filename': self.filename,
+            'deltaFileName': self.delta_file_name,
             'metadata': self.metadata,
             'content': [content.json() for content in self.content]
         }
 
 
 class IngressStatusEnum(Enum):
     HEALTHY = 'HEALTHY'
@@ -152,16 +152,16 @@
     UNHEALTHY = 'UNHEALTHY'
 
 
 class IngressResult(Result):
     def __init__(self, context: Context):
         super().__init__('ingress', 'INGRESS', context)
         self.memo = None
-        self.execute_immediate = False
         self.ingress_result_items = []
+        self.execute_immediate = False
         self.status = IngressStatusEnum.HEALTHY
         self.statusMessage = None
 
     def add_item(self, ingress_result_item: IngressResultItem):
         self.ingress_result_items.append(ingress_result_item)
         return self
```

### Comparing `deltafi-2.0rc1714076410617/deltafi/storage.py` & `deltafi-2.0rc1715691282958/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/test_kit/__init__.py` & `deltafi-2.0rc1715691282958/deltafi/test_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/test_kit/assertions.py` & `deltafi-2.0rc1715691282958/deltafi/test_kit/assertions.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/test_kit/compare_helpers.py` & `deltafi-2.0rc1715691282958/deltafi/test_kit/compare_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,61 +65,66 @@
                 paths within the object from comparison; if empty or not provided, then no excludes are applied."""
         if regex_exclusion_list is None:
             regex_exclusion_list = []
         self.excludes = regex_exclusion_list
         self.ignore_order = ignore_order
 
     def __perform_find(self, obj: object, item):
-        """Returns a dict of matches of the 'item' in the object 'obj'.  The returned dict is empty if there are no
-                matches. Excludes path determined by the constructor."""
-        return DeepSearch(obj, item, verbose_level=2, exclude_regex_paths=self.excludes)
+        """Returns a dict of matches of the 'item' in the object 'obj'.  Both keys and values of dicts are included in
+                the search.  The item may be compiled regex pattern or a string that compiles to a regex pattern.  The
+                returned dict is empty if there are no matches. Excludes path(s) determined by the constructor."""
+        return DeepSearch(obj, item, verbose_level=2, exclude_regex_paths=self.excludes, use_regexp=True)
 
     def is_not_found(self, obj: object, item):
-        """Returns None if there are no occurrences of 'item' in object 'obj' else returns a ValueError.  The argument
-                'item' may be a scalar or a list.  Excludes path and failure on ordering of elements are determined by
-                the constructor."""
+        """Returns None if there are no occurrences of 'item' in object 'obj' else raises a ValueError.  Both keys and
+                values of dicts are included in the search.  If 'item' is a list, then all elements of item must not be
+                found in list, else a ValueError is raised.  The argument 'item' may be a compiled regex pattern, a
+                string that compiles to a regex pattern, or a list of either or both.  Excludes path(s) and failure on
+                ordering of elements are determined by the constructor."""
 
         all_matches = []
 
         if isinstance(item, list):
             for value in item:
                 matches = self.__perform_find(obj, value)
                 if len(matches) > 0:
                     all_matches.append(matches)
         else:
             matches = self.__perform_find(obj, item)
             if len(matches) > 0:
                 all_matches.append(matches)
 
         if len(all_matches) > 0:
-            raise ValueError(f"{all_matches}")
+            raise ValueError("Matches found for items '" + f"{all_matches}" + "'")
 
         assert len(all_matches) == 0
 
     def is_found(self, obj: object, item):
-        """Returns None if there are no occurrences of 'item' in object 'obj' else returns a ValueError.  The argument
-                'item' may be a scalar or a list.  Excludes path and failure on ordering of elements are determined by
-                the constructor."""
+        """Returns None if 'item' occurs in object 'obj' else raises a ValueError.  Both keys and values of dicts are
+                included in the search.  If 'item' is a list, then all elements of item must occur in the object else a
+                ValueError is returned.  The argument 'item' may be a compiled regex pattern, a string that compiles to
+                a regex pattern, or a list of either or both. Excludes path(s) and failure on ordering of elements are
+                determined by the constructor."""
 
-        all_matches = []
+        not_found_items = []
 
         if isinstance(item, list):
             for value in item:
                 matches = self.__perform_find(obj, value)
-                if len(matches) > 0:
-                    all_matches.append(matches)
+                if len(matches) == 0:
+                    not_found_items.append(value)
         else:
             matches = self.__perform_find(obj, item)
-            if len(matches) > 0:
-                all_matches.append(matches)
+            if len(matches) == 0:
+                not_found_items.append(item)
 
-        if len(all_matches) == 0:
-            raise ValueError("No matches found for '" + str(item) + "'")
+        if len(not_found_items) > 0:
+            raise ValueError("No matches found for items '" + f"{not_found_items}" + "'")
 
-        assert len(all_matches) > 0
+        assert len(not_found_items) == 0
 
     def __perform_diff(self, expected, actual):
         """Returns a dict with differences between 'expected' and 'actual'.  The returned dict is empty if 'expected'
                 and 'actual' are equivalent.  Both 'expected' and 'actual' must be dicts. Excludes path and failure on
                 ordering of elements are determined by the constructor.  Elements must match number of repetitions."""
         return DeepDiff(expected, actual, ignore_order=self.ignore_order, report_repetition=True,
                         exclude_regex_paths=self.excludes)
```

### Comparing `deltafi-2.0rc1714076410617/deltafi/test_kit/constants.py` & `deltafi-2.0rc1715691282958/deltafi/test_kit/constants.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/test_kit/domain.py` & `deltafi-2.0rc1715691282958/deltafi/test_kit/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/test_kit/egress.py` & `deltafi-2.0rc1715691282958/deltafi/test_kit/egress.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/test_kit/enrich.py` & `deltafi-2.0rc1715691282958/deltafi/test_kit/enrich.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/test_kit/framework.py` & `deltafi-2.0rc1715691282958/deltafi/test_kit/framework.py`

 * *Files 12% similar despite different names*

```diff
@@ -184,29 +184,18 @@
         self.did = ""
         self.loaded_inputs = []
         self.package_name = package_name
         self.res_path = ""
 
     def __reset__(self, did: str):
         self.content_service = InternalContentService()
-<<<<<<< HEAD
         if did is None:
             self.did = str(uuid.uuid4())
         else:
             self.did = did
-        self.expected_outputs = []
-||||||| parent of 831733c7 (2.0 Refactor)
-        self.did = str(uuid.uuid4())
-        self.expected_outputs = []
-=======
-        if did is None:
-            self.did = str(uuid.uuid4())
-        else:
-            self.did = did
->>>>>>> 831733c7 (2.0 Refactor)
         self.loaded_inputs = []
         self.res_path = ""
 
     def load_file(self, ioc: IOContent):
         file_res = self.res_path.joinpath(ioc.file_name)
         with file_res.open("r") as f:
             contents = f.read()
@@ -233,44 +222,31 @@
 
         return content_list
 
     def make_df_msg(self, test_case: TestCaseBase):
         content_list = self.make_content_list(test_case)
         self.content_service.load(self.loaded_inputs)
 
-<<<<<<< HEAD
-        return DeltaFileMessage(
-            metadata=test_case.in_meta,
-            content_list=content_list,
-            domains=test_case.in_domains,
-            enrichments=test_case.in_enrichments)
-||||||| parent of 831733c7 (2.0 Refactor)
-        return DeltaFileMessage(metadata=test_case.in_meta,
-                                content_list=content_list,
-                                domains=test_case.in_domains,
-                                enrichments=test_case.in_enrichments)
-=======
         return DeltaFileMessage(metadata=test_case.in_meta,
                                 content_list=content_list)
->>>>>>> 831733c7 (2.0 Refactor)
 
     def make_context(self, test_case: TestCaseBase):
         action_name = INGRESS_FLOW + "." + test_case.action.__class__.__name__
         return Context(
             did=self.did,
-            action_flow=INGRESS_FLOW,
+            delta_file_name=test_case.file_name,
+            data_source="DATASRC",
+            flow_name=INGRESS_FLOW,
+            flow_id="FLOWID",
             action_name=action_name,
-            source_filename=test_case.file_name,
-            ingress_flow=INGRESS_FLOW,
-            egress_flow=EGRESS_FLOW,
-            system=SYSTEM,
+            action_id="ACTIONID",
+            action_version="1.0",
             hostname=HOSTNAME,
+            system_name=SYSTEM,
             content_service=self.content_service,
-            collect=None,
-            collected_dids=None,
             logger=get_logger())
 
     def make_event(self, test_case: TestCaseBase):
         return Event(delta_file_messages=[self.make_df_msg(test_case)], context=self.make_context(test_case),
                      params=test_case.parameters, queue_name="", return_address="")
 
     def call_action(self, test_case: TestCaseBase):
@@ -308,47 +284,35 @@
         if test_case.expected_result_type == ErrorResult:
             self.execute_error(test_case)
         elif test_case.expected_result_type == FilterResult:
             self.execute_filter(test_case)
         else:
             raise ValueError(f"unknown type: {test_case.expected_result_type}")
 
-    def compare_content_details(self, expected: LoadedContent, actual: Content):
+    @staticmethod
+    def compare_content_details(expected: LoadedContent, actual: Content):
         assert_equal(expected.content_type, actual.media_type)
         assert_equal(expected.name, actual.name)
 
-    def compare_one_content(self, comparitor: CompareHelper, expected: LoadedContent, actual, index):
+    def compare_one_content(self, comparator: CompareHelper, expected: LoadedContent, actual, index):
         self.compare_content_details(expected, actual)
         seg_id = actual.segments[0].uuid
-        comparitor.compare(expected.data, self.content_service.get_output(seg_id), f"Content[{index}]")
+        comparator.compare(expected.data, self.content_service.get_output(seg_id), f"Content[{index}]")
 
-    def compare_content_list(self, comparitor: CompareHelper, expected_outputs: List[IOContent], content: List):
+    def compare_content_list(self, comparator: CompareHelper, expected_outputs: List[IOContent], content: List):
         assert_equal_len(expected_outputs, content)
         for index, expected_ioc in enumerate(expected_outputs):
             if len(expected_ioc.content_bytes) == 0:
-                expected = LoadedContent(self.did, expected_ioc, self.load_file(output_ioc))
+                expected = LoadedContent(self.did, expected_ioc, self.load_file(expected_ioc))
             else:
                 expected = LoadedContent(self.did, expected_ioc, None)
-            self.compare_one_content(comparitor, expected, content[index], index)
-
-    def compare_one_metric(self, expected: Metric, result: Metric):
-        assert expected.name == result.name
-        assert_equal_with_label(expected.value, result.value, expected.name)
-        assert_keys_and_values(expected.tags, result.tags)
-
-            expected_value = expected['value']
-            if type(expected_value) == str:
-                comparitor.compare(expected_value, actual['value'], f"Domain[{index}]")
-            elif type(expected_value) == IOContent:
-                expected_data = self.load_file(expected_value)
-                comparitor.compare(expected_data, actual['value'], f"Domain[{index}]")
-            else:
-                raise ValueError(f"unknown expected_value type: {type(expected_value)}")
+            self.compare_one_content(comparator, expected, content[index], index)
 
-    def compare_one_metric(self, expected: Metric, result: Metric):
+    @staticmethod
+    def compare_one_metric(expected: Metric, result: Metric):
         assert expected.name == result.name
         assert_equal_with_label(expected.value, result.value, expected.name)
         assert_keys_and_values(expected.tags, result.tags)
 
     def compare_metrics(self, expected_metrics: List[Metric], results: List[Metric]):
         if len(expected_metrics) > 0:
             assert_equal_len(expected_metrics, results)
```

### Comparing `deltafi-2.0rc1714076410617/deltafi/test_kit/transform.py` & `deltafi-2.0rc1715691282958/deltafi/test_kit/transform.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/deltafi/test_kit/validate.py` & `deltafi-2.0rc1715691282958/deltafi/test_kit/validate.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1714076410617/pyproject.toml` & `deltafi-2.0rc1715691282958/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltafi"
-version = "2.0rc1714076410617"
+version = "2.0rc1715691282958"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
@@ -19,27 +19,27 @@
     "Programming Language :: Python :: 3.12"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 deepdiff = ">=6.7.1"
 json-logging = ">=1.3.0"
-minio = ">=7.2.3"
-pydantic = ">=2.5.3"
-redis = ">=5.0.1"
+minio = ">=7.2.5"
+pydantic = ">=2.7.1"
+redis = ">=5.0.4"
 requests = ">=2.31.0"
-urllib3 = ">=2.1.0"
+urllib3 = ">=2.2.1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = ">=7.4.4"
-pytest-mock = ">=3.12.0"
-mockito = ">=1.4.0"
+pytest = ">=8.1.1"
+pytest-mock = ">=3.14.0"
+mockito = ">=1.5.0"
 
 [tool.poetry.urls]
 'Source Code' = "https://gitlab.com/deltafi/deltafi"
 Documentation = "https://docs.deltafi.org/#/"
 'Bug Reports' = "https://chat.deltafi.org/deltafi/channels/bug-reports"
 
 [build-system]
```

### Comparing `deltafi-2.0rc1714076410617/PKG-INFO` & `deltafi-2.0rc1715691282958/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 2.0rc1714076410617
+Version: 2.0rc1715691282958
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -16,19 +16,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Requires-Dist: deepdiff (>=6.7.1)
 Requires-Dist: json-logging (>=1.3.0)
-Requires-Dist: minio (>=7.2.3)
-Requires-Dist: pydantic (>=2.5.3)
-Requires-Dist: redis (>=5.0.1)
+Requires-Dist: minio (>=7.2.5)
+Requires-Dist: pydantic (>=2.7.1)
+Requires-Dist: redis (>=5.0.4)
 Requires-Dist: requests (>=2.31.0)
-Requires-Dist: urllib3 (>=2.1.0)
+Requires-Dist: urllib3 (>=2.2.1)
 Project-URL: Bug Reports, https://chat.deltafi.org/deltafi/channels/bug-reports
 Project-URL: Documentation, https://docs.deltafi.org/#/
 Project-URL: Source Code, https://gitlab.com/deltafi/deltafi
 Description-Content-Type: text/markdown
 
 # DeltaFi Action Kit
```

