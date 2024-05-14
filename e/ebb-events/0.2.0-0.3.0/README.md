# Comparing `tmp/ebb_events-0.2.0.tar.gz` & `tmp/ebb_events-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebb_events-0.2.0.tar", max compression
+gzip compressed data, was "ebb_events-0.3.0.tar", max compression
```

## Comparing `ebb_events-0.2.0.tar` & `ebb_events-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.2.0/LICENSE
--rw-r--r--   0        0        0     8800 2024-05-10 21:40:45.942475 ebb_events-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.2.0/ebb_events/__init__.py
--rw-r--r--   0        0        0     7572 2024-05-10 21:40:45.943169 ebb_events-0.2.0/ebb_events/builders/event_builder.py
--rw-r--r--   0        0        0      231 2024-05-06 17:16:47.745004 ebb_events-0.2.0/ebb_events/constants.py
--rw-r--r--   0        0        0     8523 2024-05-10 21:40:45.943550 ebb_events-0.2.0/ebb_events/consumers/event_consumer.py
--rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.2.0/ebb_events/enums.py
--rw-r--r--   0        0        0      414 2024-05-10 21:40:45.943826 ebb_events-0.2.0/ebb_events/event_payload_utils.py
--rw-r--r--   0        0        0     2668 2024-05-10 21:40:45.944168 ebb_events-0.2.0/ebb_events/event_schema.py
--rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.2.0/ebb_events/exceptions.py
--rw-r--r--   0        0        0      571 2024-05-10 21:40:45.944486 ebb_events-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9298 1970-01-01 00:00:00.000000 ebb_events-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8842 2024-05-14 16:56:47.897263 ebb_events-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.3.0/ebb_events/__init__.py
+-rw-r--r--   0        0        0     8308 2024-05-14 16:56:47.897743 ebb_events-0.3.0/ebb_events/builders/event_builder.py
+-rw-r--r--   0        0        0     9236 2024-05-14 16:56:47.898243 ebb_events-0.3.0/ebb_events/consumers/event_consumer.py
+-rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.3.0/ebb_events/enums.py
+-rw-r--r--   0        0        0      414 2024-05-10 21:40:45.943826 ebb_events-0.3.0/ebb_events/event_payload_utils.py
+-rw-r--r--   0        0        0     2668 2024-05-13 20:48:51.509330 ebb_events-0.3.0/ebb_events/event_schema.py
+-rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.3.0/ebb_events/exceptions.py
+-rw-r--r--   0        0        0      263 2024-05-14 16:56:47.898608 ebb_events-0.3.0/ebb_events/field_constants.py
+-rw-r--r--   0        0        0      571 2024-05-14 16:56:47.899028 ebb_events-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9340 1970-01-01 00:00:00.000000 ebb_events-0.3.0/PKG-INFO
```

### Comparing `ebb_events-0.2.0/LICENSE` & `ebb_events-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebb_events-0.2.0/README.md` & `ebb_events-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,27 +12,34 @@
     system_id="test-system",
     event_type="data",
     subsystem_id="test-subsystem",
     device_id="test-device-01",
 )
 
 event_topic = event_envelope.build_event_topic()
-event_payload = event_envelope.build_event_payload_json(message={...}, metadata={...})  # Builds a payload of the expected ebb-events structure
+# Builds a JSON payload of the expected ebb-events structure
+event_payload = event_envelope.build_event_payload_json(
+    message={...},
+    serial_number="ABC123",
+    metadata={...},
+    datetime_obj=my_datetime
+)
 ```
 
 Use ebb-events package to consume events published with this expected ebb-events structure
 ```python
 from ebb_events.consumers.event_consumer import EventConsumer
 
 my_event_payload = {...}
 event_consumer = EventConsumer(payload=my_event_payload)
 
 event_consumer.get_event_message()  # Retrieves the dict message found in the payload's `data` field
 event_consumer.get_event_time()
 event_conumser.get_event_system_id()
+event_consumer.get_device_serial_number()
 ```
 
 # Topic Structure:
 One thing that this package enforces is a topic structure for publishing MQTT messages to a broker. Well defined topics help Our topic structure is as follows:
 * _\<organization\>/\<system-id\>/\<event-type\>/\<subsystem-id\>/\<device-id\>_
 
 ### Topic Naming Rules:
@@ -71,15 +78,15 @@
 {
     "id": str(uuid),
     "time": str,  # [RFC3339](https://datatracker.ietf.org/doc/html/rfc3339) format
     "source": str,  # same as topic string
     "type": str,
     "data": {
         "metadata": {
-            "serial_number": str,  # Example of potential metadata, this is not a required metadata field
+            "serial_number": str,
             ...
         },
         ...  # unique nested JSON dependent on event-type
     }
 }
 ```
```

### Comparing `ebb_events-0.2.0/ebb_events/builders/event_builder.py` & `ebb_events-0.3.0/ebb_events/builders/event_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 from datetime import datetime, timezone
 import json
 from typing import Optional
 from uuid import uuid4
 
 from marshmallow import ValidationError
-from ebb_events.constants import DATA, ID, METADATA, SOURCE, TIME, TYPE
+from ebb_events.field_constants import (
+    DATA,
+    ID,
+    METADATA,
+    SOURCE,
+    TIME,
+    TYPE,
+    SERIAL_NUMBER,
+)
 from ebb_events.event_schema import EventEnvelopeSchema, EventPayloadSchema
 from ebb_events.exceptions import PayloadFormatException, TopicFormatException
 
 
 class EventEnvelope:
     """
     EventEnvelope class used to build the event payload and topic
@@ -41,29 +49,29 @@
             and self.event_type == other.event_type
             and self.subsystem_id == other.subsystem_id
             and self.device_id == other.device_id
         )
 
     def _validate(self):
         """
-        Validate that the fields passed to EventEnvelope follow expected format and rules
+        Validate that the fields passed to EventEnvelope follow expected format and rules.
 
         Return: None if valid fields
         Raises: TopicFormatException for invalid fields
         """
         envelope_schema = EventEnvelopeSchema()
         errors = envelope_schema.validate(envelope_schema.dump(self))
         if errors:
             # errors will be a dictionary of validation errors
             raise TopicFormatException(errors)
 
     def _format_time(self, datetime_raw: Optional[datetime] = None) -> str:
         """
-        Helper takes in datetime object or None and returns the string datetime in RFC3339 format UTC
-        If None - timestamp is .now()
+        Helper takes in datetime object or None and returns the string datetime in RFC3339 format UTC.
+        If None - timestamp is datetime.now().
 
         Format: YYYY-MM-DDThh:mm:ss.ssssss+/-hh:mm
         """
         datetime_raw = (
             datetime_raw if datetime_raw is not None else datetime.now(timezone.utc)
         )
         if (
@@ -71,51 +79,57 @@
             or datetime_raw.tzinfo.utcoffset(datetime_raw) is None
         ):
             datetime_raw = datetime_raw.replace(tzinfo=timezone.utc)
         return datetime_raw.isoformat()
 
     def build_event_topic(self) -> str:
         """
-        Joins the EventEnvelope fields to form a valid topic string
-        Note: Fields are validated in __init__ so no need to re-validate here
+        Joins the EventEnvelope fields to form a valid topic string.
+        Note: Fields are validated in __init__ so no need to re-validate here.
         Returns:
             str: _description_
         """
         topic = f"{self.organization}/{self.system_id}/{self.event_type}/{self.subsystem_id}/{self.device_id}"
         # This should be enforced by the ._validate() call and the EventEnvelopeSchema too
         if len(topic) > 256:
             raise TopicFormatException("Topic length cannot exceed 256 characters.")
         return topic
 
     def build_event_payload_dict(
         self,
         message: dict,
+        serial_number: str = None,
         metadata: dict = {},
         datetime_obj: Optional[datetime] = None,
         remove_nones: bool = False,
     ) -> dict:
         """
         Method validates the message structure, builds and returns the expected
         event payload to be used in the MQTT payload as a json serializable dictionary.
         NOTE: Returned object is a python dictionary, not a json object. In order to publish this,
         one must either `json.dumps()` this result or use `build_event_payload_json()` method.
 
         Args:
-            message (dict): Dictionary containing the message information that is being published
-            metadata (dict): Dictionary containing metadata information to be included in the data
-            datetime_obj (Optional[datetime]): datetime obj to use as event time
-            remove_nones (bool): If set to True, all key:value pairs where value=None or NaN will
+            message (dict): Dictionary containing the message information that is being published.
+            serial_number (str): String serial number of the sensor publishing this event
+                    This will be added to metadata dict and will overwrite any metadata field
+                    named "serial_number".
+            metadata (dict): Dictionary containing extra metadata information to be included in the data.
+            datetime_obj (Optional[datetime]): datetime obj to use as event time.
+            remove_nones (bool): If set to True, all key:value pairs where value=None will
                                     be removed/omitted from the resulting payload dict
 
         Returns:
-            dict: Dictionary of the expected MQTT event message format
+            dict: Dictionary of the expected MQTT event message format.
 
         Exceptions:
-            Raises 'PayloadFormatException' if the topic or message does not meet the expected format
+            Raises 'PayloadFormatException' if the topic or message does not meet the expected format.
         """
+        if serial_number is not None:
+            metadata[SERIAL_NUMBER] = str(serial_number)
         payload_schema = EventPayloadSchema(context={"remove_nones": remove_nones})
         if datetime_obj is not None and type(datetime_obj) is not datetime:
             raise PayloadFormatException(
                 "datetime_obj must be a valid datetime object."
             )
         try:
             event_payload = {
@@ -147,37 +161,42 @@
                 "Payload message and metadata must be JSON serializable dictionaries."
             )
         return payload_schema.dump(deserialized_payload)
 
     def build_event_payload_json(
         self,
         message: dict,
+        serial_number: str = None,
         metadata: dict = {},
         datetime_obj: Optional[datetime] = None,
         remove_nones: bool = False,
     ):
         """
         Method validates the message structure, builds and returns the expected
         event payload to be used in the MQTT payload as a JSON formatted str.
 
-        This returned value can be immediately placed in an MQTT publish call as it's a json string
+        This returned value can be immediately placed in an MQTT publish call as it's a json string.
 
         Args:
-            message (dict): Dictionary containing the message information that is being published
-            metadata (dict): Dictionary containing metadata information to be included in the data
-            datetime_obj (Optional[datetime]): datetime obj to use as event time
-            remove_nones (bool): If set to True, all key:value pairs where value=None or NaN will
-                                    be removed/omitted from the resulting payload json
+            message (dict): Dictionary containing the message information that is being published.
+            serial_number (str): String serial number of the sensor publishing this event
+                    This will be added to metadata dict and will overwrite any metadata field
+                    named "serial_number".
+            metadata (dict): Dictionary containing extra metadata information to be included in the data
+            datetime_obj (Optional[datetime]): datetime obj to use as event time.
+            remove_nones (bool): If set to True, all key:value pairs where value=None will
+                                    be removed/omitted from the resulting payload json.
 
         Returns:
-            dict: Dictionary of the expected MQTT event message format
+            dict: Dictionary of the expected MQTT event message format.
 
         Exceptions:
-            Raises 'PayloadFormatException' if the topic or message does not meet the expected format
+            Raises 'PayloadFormatException' if the topic or message does not meet the expected format.
         """
         payload_dict = self.build_event_payload_dict(
             message=message,
+            serial_number=serial_number,
             metadata=metadata,
             datetime_obj=datetime_obj,
             remove_nones=remove_nones,
         )
         return json.dumps(payload_dict)
```

### Comparing `ebb_events-0.2.0/ebb_events/consumers/event_consumer.py` & `ebb_events-0.3.0/ebb_events/consumers/event_consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 import copy
 from datetime import datetime
 from marshmallow import ValidationError
-from ebb_events.constants import DATA, ID, METADATA, SOURCE, TIME, TYPE
+from ebb_events.field_constants import (
+    DATA,
+    ID,
+    METADATA,
+    SERIAL_NUMBER,
+    SOURCE,
+    TIME,
+    TYPE,
+)
 from ebb_events.builders.event_builder import EventEnvelope
 from ebb_events.event_schema import EventPayloadSchema
 from ebb_events.exceptions import PayloadFormatException
 
 
 class EventConsumer:
     """
@@ -30,211 +38,228 @@
             payload_schema.load(data=payload)
             return True
         except ValidationError:
             return False
 
     def get_event_id(self) -> str:
         """
-        Helper to fetch event's id field as str(id)
+        Helper to fetch event's id field as str(id).
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            str: event's string id
+            str: event's string id.
         """
         if self.is_ebb_event_structure:
             return str(self.raw_payload.get(ID))
         raise PayloadFormatException()
 
     def get_event_time_str(self) -> str:
         """
         Helper to fetch event's time field in RFC3339 format: YYYY-MM-DDThh:mm:ss.ssssss+/-hh:mm
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            str: event's time field
+            str: event's time field.
         """
         if self.is_ebb_event_structure:
             return str(self.raw_payload.get(TIME))
         raise PayloadFormatException()
 
     def get_event_time(self) -> datetime:
         """
-        Helper to fetch event's time field as python datetime object
+        Helper to fetch event's time field as python datetime object.
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            datetime: event's time field
+            datetime: event's time field.
         """
         if self.is_ebb_event_structure:
             return datetime.fromisoformat(self.raw_payload.get(TIME))
         raise PayloadFormatException()
 
     def get_event_source(self) -> str:
         """
-        Helper to fetch event's source as string. For ebb_events, the `source` field matches the MQTT `topic`
+        Helper to fetch event's source as string. For ebb_events, the `source` field matches the MQTT `topic`.
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            str: event's source field
+            str: event's source field.
         """
         if self.is_ebb_event_structure:
             return str(self.raw_payload.get(SOURCE))
         raise PayloadFormatException()
 
     def get_event_topic(self) -> str:
         """
-        Helper to fetch event's topic string. For ebb_events, the MQTT `topic` field matches the event's source
+        Helper to fetch event's topic string. For ebb_events, the MQTT `topic` field matches the event's source.
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            str: event's topic string
+            str: event's topic string.
         """
         return self.get_event_source()
 
     def get_event_type(self) -> str:
         """
-        Helper to fetch event's type as string
+        Helper to fetch event's type as string.
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            str: event's type field
+            str: event's type field.
         """
         if self.is_ebb_event_structure:
             return str(self.raw_payload.get(TYPE))
         raise PayloadFormatException()
 
     def get_event_organization(self) -> str:
         """
-        Helper to fetch event's organization portion of topic hierarchy as string
-        This is the top level of the topic hierarchy
+        Helper to fetch event's organization portion of topic hierarchy as string.
+        This is the top level of the topic hierarchy.
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            str: event's organization portion of the topic hierarchy
+            str: event's organization portion of the topic hierarchy.
         """
         # This ensures that the `source` field matches the expected topic structure
         if self.is_ebb_event_structure:
             topic_list = self.raw_payload.get(SOURCE).split("/")
             return topic_list[0]
         raise PayloadFormatException()
 
     def get_event_system_id(self) -> str:
         """
-        Helper to fetch event's system_id portion of topic hierarchy as string
-        This is the second level of the topic hierarchy
+        Helper to fetch event's system_id portion of topic hierarchy as string.
+        This is the second level of the topic hierarchy.
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            str: event's system_id portion of the topic hierarchy
+            str: event's system_id portion of the topic hierarchy.
         """
         # This ensures that the `source` field matches the expected topic structure
         if self.is_ebb_event_structure:
             topic_list = self.raw_payload.get(SOURCE).split("/")
             return topic_list[1]
         raise PayloadFormatException()
 
     def get_event_subsystem_id(self) -> str:
         """
-        Helper to fetch event's subsystem_id portion of topic hierarchy as string
-        This is the fourth level of the topic hierarchy
+        Helper to fetch event's subsystem_id portion of topic hierarchy as string.
+        This is the fourth level of the topic hierarchy.
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            str: event's subsystem_id portion of the topic hierarchy
+            str: event's subsystem_id portion of the topic hierarchy.
         """
         # This ensures that the `source` field matches the expected topic structure
         if self.is_ebb_event_structure:
             topic_list = self.raw_payload.get(SOURCE).split("/")
             return topic_list[3]
         raise PayloadFormatException()
 
     def get_event_device_id(self) -> str:
         """
-        Helper to fetch event's device_id portion of topic hierarchy as string
-        This is the fourth level of the topic hierarchy
+        Helper to fetch event's device_id portion of topic hierarchy as string.
+        This is the fourth level of the topic hierarchy.
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            str: event's device_id portion of the topic hierarchy
+            str: event's device_id portion of the topic hierarchy.
         """
         # This ensures that the `source` field matches the expected topic structure
         if self.is_ebb_event_structure:
             topic_list = self.raw_payload.get(SOURCE).split("/")
             return topic_list[4]
         raise PayloadFormatException()
 
     def get_event_envelope(self) -> EventEnvelope:
         """
-        Helper to build and return EventEnvelope from payload
+        Helper to build and return EventEnvelope from payload.
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            EventEnvelope: event envelope object with expected fields
+            EventEnvelope: event envelope object with expected fields.
         """
         if self.is_ebb_event_structure:
             return EventEnvelope(
                 organization=self.get_event_organization(),
                 system_id=self.get_event_system_id(),
                 event_type=self.get_event_type(),
                 subsystem_id=self.get_event_subsystem_id(),
                 device_id=self.get_event_device_id(),
             )
         raise PayloadFormatException()
 
     def get_event_message(self, metadata_included=True) -> dict:
         """
-        Helper fetches and returns message dict from payload
-        Metadata field in the message dict is included by default but can be parsed out
+        Helper fetches and returns message dict from payload.
+        Metadata field in the message dict is included by default but can be parsed out.
 
         Args:
             metadata_included (bool, optional): If set to False, returned dict will remove the `metadata` portion of the message.
                                                 Defaults to True.
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            dict: Message value of payload with or without the `metadata` field depending on metadata_included parameter
+            dict: Message value of payload with or without the `metadata` field depending on metadata_included parameter.
         """
         if self.is_ebb_event_structure:
             # Copy of message so that we don't actually alter the raw_payload itself
             message: dict = copy.deepcopy(self.raw_payload.get(DATA))
             if not metadata_included:
                 message.pop(METADATA, {})
             return message
         raise PayloadFormatException()
 
     def get_event_message_metadata(self) -> dict:
         """
-        Helper to fetch and return the metadata dictionary within the payload's event message
+        Helper to fetch and return the metadata dictionary within the payload's event message.
 
         Raises:
-            PayloadFormatException: Raised if event does not match ebb_event structure
+            PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
-            dict: Metadata included in event message
+            dict: Metadata included in event message.
         """
         if self.is_ebb_event_structure:
             return self.raw_payload.get(DATA, {}).get(METADATA, {})
         raise PayloadFormatException()
+
+    def get_device_serial_number(self) -> str:
+        """
+        Helper to fetch and return the serial number of the publishing device as a string.
+        Pulls this information from the metadata of the event message.
+
+        Raises:
+            PayloadFormatException: Raised if event does not match ebb_event structure.
+
+        Returns:
+            dict: Metadata included in event message.
+        """
+        if self.is_ebb_event_structure:
+            return str(
+                self.raw_payload.get(DATA, {}).get(METADATA, {}).get(SERIAL_NUMBER, "")
+            )
+        raise PayloadFormatException()
```

### Comparing `ebb_events-0.2.0/ebb_events/event_schema.py` & `ebb_events-0.3.0/ebb_events/event_schema.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.2.0/pyproject.toml` & `ebb_events-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ebb-events"
-version = "0.2.0"
+version = "0.3.0"
 description = "Package for building and standardizing MQTT event messages."
 authors = ["Ryan Bloom <ryan.bloom@ebbcarbon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 marshmallow = "^3.21.1"
```

### Comparing `ebb_events-0.2.0/PKG-INFO` & `ebb_events-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebb-events
-Version: 0.2.0
+Version: 0.3.0
 Summary: Package for building and standardizing MQTT event messages.
 Author: Ryan Bloom
 Author-email: ryan.bloom@ebbcarbon.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -26,27 +26,34 @@
     system_id="test-system",
     event_type="data",
     subsystem_id="test-subsystem",
     device_id="test-device-01",
 )
 
 event_topic = event_envelope.build_event_topic()
-event_payload = event_envelope.build_event_payload_json(message={...}, metadata={...})  # Builds a payload of the expected ebb-events structure
+# Builds a JSON payload of the expected ebb-events structure
+event_payload = event_envelope.build_event_payload_json(
+    message={...},
+    serial_number="ABC123",
+    metadata={...},
+    datetime_obj=my_datetime
+)
 ```
 
 Use ebb-events package to consume events published with this expected ebb-events structure
 ```python
 from ebb_events.consumers.event_consumer import EventConsumer
 
 my_event_payload = {...}
 event_consumer = EventConsumer(payload=my_event_payload)
 
 event_consumer.get_event_message()  # Retrieves the dict message found in the payload's `data` field
 event_consumer.get_event_time()
 event_conumser.get_event_system_id()
+event_consumer.get_device_serial_number()
 ```
 
 # Topic Structure:
 One thing that this package enforces is a topic structure for publishing MQTT messages to a broker. Well defined topics help Our topic structure is as follows:
 * _\<organization\>/\<system-id\>/\<event-type\>/\<subsystem-id\>/\<device-id\>_
 
 ### Topic Naming Rules:
@@ -85,15 +92,15 @@
 {
     "id": str(uuid),
     "time": str,  # [RFC3339](https://datatracker.ietf.org/doc/html/rfc3339) format
     "source": str,  # same as topic string
     "type": str,
     "data": {
         "metadata": {
-            "serial_number": str,  # Example of potential metadata, this is not a required metadata field
+            "serial_number": str,
             ...
         },
         ...  # unique nested JSON dependent on event-type
     }
 }
 ```
```

