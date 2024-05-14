# Comparing `tmp/vulavula-0.1.1.tar.gz` & `tmp/vulavula-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulavula-0.1.1.tar", last modified: Thu May  2 11:16:44 2024, max compression
+gzip compressed data, was "vulavula-0.2.0.tar", last modified: Tue May 14 08:04:04 2024, max compression
```

## Comparing `vulavula-0.1.1.tar` & `vulavula-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     5336 2024-05-01 17:41:53.374894 vulavula-0.1.1/README.md
--rw-r--r--   0        0        0      912 2024-05-02 11:16:44.820504 vulavula-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 06:16:28.668957 vulavula-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 15:37:52.520889 vulavula-0.1.1/tests/audio/test1.mp3
--rw-r--r--   0        0        0     3284 2024-05-01 17:41:53.376004 vulavula-0.1.1/tests/test_nlu.py
--rw-r--r--   0        0        0     2150 2024-05-01 17:41:53.376223 vulavula-0.1.1/tests/test_sentiment.py
--rw-r--r--   0        0        0     3429 2024-05-01 17:41:53.376541 vulavula-0.1.1/tests/test_transcribe.py
--rw-r--r--   0        0        0     1884 2024-05-01 17:41:53.376685 vulavula-0.1.1/tests/test_transport.py
--rw-r--r--   0        0        0       35 2024-05-01 17:41:53.376769 vulavula-0.1.1/vulavula/__init__.py
--rw-r--r--   0        0        0       35 2024-05-01 17:41:53.376848 vulavula-0.1.1/vulavula/client/__init__.py
--rw-r--r--   0        0        0     3985 2024-05-01 17:41:53.376982 vulavula-0.1.1/vulavula/client/client.py
--rw-r--r--   0        0        0     4555 2024-05-01 17:41:53.377242 vulavula-0.1.1/vulavula/client/nlu.py
--rw-r--r--   0        0        0     2704 2024-05-01 17:41:53.377347 vulavula-0.1.1/vulavula/client/sentiment.py
--rw-r--r--   0        0        0     5667 2024-05-01 17:41:53.377627 vulavula-0.1.1/vulavula/client/transcribe.py
--rw-r--r--   0        0        0     3633 2024-05-01 17:41:53.377741 vulavula-0.1.1/vulavula/client/transport.py
--rw-r--r--   0        0        0        1 2024-05-01 17:41:53.377828 vulavula-0.1.1/vulavula/common/__init__.py
--rw-r--r--   0        0        0      942 2024-05-01 17:41:53.378112 vulavula-0.1.1/vulavula/common/error_handler.py
--rw-r--r--   0        0        0     2748 2024-05-01 17:41:53.378366 vulavula-0.1.1/vulavula/common/response_handler.py
--rw-r--r--   0        0        0       29 2024-05-01 17:41:53.378448 vulavula-0.1.1/vulavula/config/__init__.py
--rw-r--r--   0        0        0      323 2024-05-01 17:41:53.378562 vulavula-0.1.1/vulavula/config/config.py
--rw-r--r--   0        0        0        1 2024-05-01 17:41:53.378636 vulavula-0.1.1/vulavula/models/__init__.py
--rw-r--r--   0        0        0      220 2024-05-01 17:41:53.378712 vulavula-0.1.1/vulavula/models/types/__init__.py
--rw-r--r--   0        0        0      105 2024-05-01 17:41:53.378800 vulavula-0.1.1/vulavula/models/types/entity_recognition.py
--rw-r--r--   0        0        0     1529 2024-05-01 17:41:53.378896 vulavula-0.1.1/vulavula/models/types/intent_classification.py
--rw-r--r--   0        0        0      105 2024-05-01 17:41:53.378976 vulavula-0.1.1/vulavula/models/types/sentiment_analysis.py
--rw-r--r--   0        0        0     5968 1970-01-01 00:00:00.000000 vulavula-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5347 2024-05-14 08:02:22.995087 vulavula-0.2.0/README.md
+-rw-r--r--   0        0        0      912 2024-05-14 08:04:04.815674 vulavula-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 06:16:28.668957 vulavula-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 15:37:52.520889 vulavula-0.2.0/tests/audio/test1.mp3
+-rw-r--r--   0        0        0     3284 2024-05-01 17:41:53.376004 vulavula-0.2.0/tests/test_nlu.py
+-rw-r--r--   0        0        0     2150 2024-05-01 17:41:53.376223 vulavula-0.2.0/tests/test_sentiment.py
+-rw-r--r--   0        0        0     3435 2024-05-14 08:02:22.995802 vulavula-0.2.0/tests/test_transcribe.py
+-rw-r--r--   0        0        0     1884 2024-05-01 17:41:53.376685 vulavula-0.2.0/tests/test_transport.py
+-rw-r--r--   0        0        0       35 2024-05-01 17:41:53.376769 vulavula-0.2.0/vulavula/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-01 17:41:53.376848 vulavula-0.2.0/vulavula/client/__init__.py
+-rw-r--r--   0        0        0     3901 2024-05-14 08:02:22.996329 vulavula-0.2.0/vulavula/client/client.py
+-rw-r--r--   0        0        0     4555 2024-05-01 17:41:53.377242 vulavula-0.2.0/vulavula/client/nlu.py
+-rw-r--r--   0        0        0     2704 2024-05-01 17:41:53.377347 vulavula-0.2.0/vulavula/client/sentiment.py
+-rw-r--r--   0        0        0     5586 2024-05-14 08:02:22.996533 vulavula-0.2.0/vulavula/client/transcribe.py
+-rw-r--r--   0        0        0     3633 2024-05-01 17:41:53.377741 vulavula-0.2.0/vulavula/client/transport.py
+-rw-r--r--   0        0        0        1 2024-05-01 17:41:53.377828 vulavula-0.2.0/vulavula/common/__init__.py
+-rw-r--r--   0        0        0      942 2024-05-01 17:41:53.378112 vulavula-0.2.0/vulavula/common/error_handler.py
+-rw-r--r--   0        0        0     2748 2024-05-01 17:41:53.378366 vulavula-0.2.0/vulavula/common/response_handler.py
+-rw-r--r--   0        0        0       29 2024-05-01 17:41:53.378448 vulavula-0.2.0/vulavula/config/__init__.py
+-rw-r--r--   0        0        0      323 2024-05-01 17:41:53.378562 vulavula-0.2.0/vulavula/config/config.py
+-rw-r--r--   0        0        0        1 2024-05-01 17:41:53.378636 vulavula-0.2.0/vulavula/models/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-01 17:41:53.378712 vulavula-0.2.0/vulavula/models/types/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-01 17:41:53.378800 vulavula-0.2.0/vulavula/models/types/entity_recognition.py
+-rw-r--r--   0        0        0     1529 2024-05-01 17:41:53.378896 vulavula-0.2.0/vulavula/models/types/intent_classification.py
+-rw-r--r--   0        0        0      105 2024-05-01 17:41:53.378976 vulavula-0.2.0/vulavula/models/types/sentiment_analysis.py
+-rw-r--r--   0        0        0     5979 1970-01-01 00:00:00.000000 vulavula-0.2.0/PKG-INFO
```

### Comparing `vulavula-0.1.1/README.md` & `vulavula-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 #### General Exception Handling
 While `VulavulaError` handles expected API-related errors, your application might encounter other unexpected exceptions. It's important to prepare for these to ensure your application can recover gracefully. 
 
 Here's a general approach to handle unexpected exceptions:
 ```python
 try:
-    response = client.transcribe()
+    upload_id, response = client.transcribe()
     print("Action Succeeded:", response)
 except VulavulaError as e:
     print("Handled VulavulaError:", e.message)
     if 'details' in e.error_data:
         print("Detailed Error Information:", e.error_data['details'])
 except Exception as e:
     print("Unhandled Exception:", str(e))
```

### Comparing `vulavula-0.1.1/pyproject.toml` & `vulavula-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vulavula"
-version = "0.1.1"
+version = "0.2.0"
 description = "The vulavula Python SDK provides access to the Vulavula API."
 authors = [
     { name = "Raphael Karanja", email = "raphael.karanja@lelapa.ai" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic[dotenv]>=2.7.1",
```

### Comparing `vulavula-0.1.1/tests/test_nlu.py` & `vulavula-0.2.0/tests/test_nlu.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.1/tests/test_sentiment.py` & `vulavula-0.2.0/tests/test_sentiment.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.1/tests/test_transcribe.py` & `vulavula-0.2.0/tests/test_transcribe.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,21 @@
         self.transcribe = Transcribe(self.client_token, self.session)
 
         # Mock successful transcription process
         self.transcribe.transcribe_process = MagicMock(return_value={'status': 'success'})
 
         # Executing the transcribe method
         webhook = "http://example.com/webhook/"
-        result = self.transcribe.transcribe(self.file_path, webhook)
+        upload_id, result = self.transcribe.transcribe(self.file_path, webhook)
 
         # Assertions
         mock_transport_instance.upload_file.assert_called_once_with(self.file_path)
         self.transcribe.transcribe_process.assert_called_once_with(str(fixed_uuid), webhook)
         self.assertEqual(result, {'status': 'success'})
+        self.assertEqual(upload_id, str(fixed_uuid))
 
     def test_transcribe_process(self):
         upload_id = uuid4()
         webhook = "http://example.com/webhook/"
         self.session.post.return_value = MagicMock(status_code=200, json=lambda: {"result": "processed"})
 
         # Assuming _handle_response just returns the json
@@ -72,13 +73,13 @@
 
         # ids and UUID for testing
         test_upload_id = uuid4()
         customer_id = 1
         project_id = 1
 
         # Call the method under test
-        result = self.transcribe.get_transcribed_text(customer_id, project_id, test_upload_id)
+        result = self.transcribe.get_transcribed_text(test_upload_id)
 
         # Assertions
         self.session.post.assert_called_once_with(
-            f"{self.base_url}/customer/{customer_id}/project/{project_id}/{test_upload_id}/get",
+            f"{self.base_url}/transcribe/{test_upload_id}/get",
             headers=self.transcribe.headers)
```

### Comparing `vulavula-0.1.1/tests/test_transport.py` & `vulavula-0.2.0/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.1/vulavula/client/client.py` & `vulavula-0.2.0/vulavula/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,19 +69,17 @@
         return self.transcribe_client.transcribe_process(upload_id, webhook)
 
     def transcribe(self, file_path: str, webhook: Optional[str] = None):
         return self.transcribe_client.transcribe(file_path, webhook)
 
     def get_transcribed_text(
             self,
-            customer_id: int,
-            project_id: int,
             upload_id: UUID
     ):
-        return self.transcribe_client.get_transcribed_text(customer_id, project_id, upload_id)
+        return self.transcribe_client.get_transcribed_text(upload_id)
 
     def get_sentiments(self, data: SentimentAnalysisRequestData):
         return self.sentiments.get_sentiments(data)
 
     def get_entities(self, data: EntityRecognitionRequestData):
         return self.nlu.get_entities(data)
```

### Comparing `vulavula-0.1.1/vulavula/client/nlu.py` & `vulavula-0.2.0/vulavula/client/nlu.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.1/vulavula/client/sentiment.py` & `vulavula-0.2.0/vulavula/client/sentiment.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.1/vulavula/client/transcribe.py` & `vulavula-0.2.0/vulavula/client/transcribe.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,31 +95,29 @@
                 print(result)
             except VulavulaError as e:
                 print(f"An error occurred: {e}")
         """
         upload_response = self.transport.upload_file(file_path)
         upload_id = upload_response.get('upload_id')
         if upload_id:
-            return self.transcribe_process(upload_id, webhook)
+            return upload_id, self.transcribe_process(upload_id, webhook)
         else:
             raise VulavulaError("Failed to upload file and retrieve upload ID.")
 
     def get_transcribed_text(
             self,
-            customer_id: int,
-            project_id: int,
             upload_id: UUID
     ):
         """
         Fetches the transcribed text for a given upload.
 
         Parameters:
             customer_id (int): The ID of the customer.
             project_id (int): The ID of the project.
             upload_id (UUID): The UUID of the uploaded file.
 
         Returns:
             dict: The response from the server after processing the transcription request.
         """
-        url = f"{self.base_url}/customer/{customer_id}/project/{project_id}/{upload_id}/get"
+        url = f"{self.base_url}/transcribe/{upload_id}/get"
         response = self.session.post(url, headers=self.headers)
         return self._handle_response(response)
```

### Comparing `vulavula-0.1.1/vulavula/client/transport.py` & `vulavula-0.2.0/vulavula/client/transport.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.1/vulavula/common/error_handler.py` & `vulavula-0.2.0/vulavula/common/error_handler.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.1/vulavula/common/response_handler.py` & `vulavula-0.2.0/vulavula/common/response_handler.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.1/vulavula/models/types/intent_classification.py` & `vulavula-0.2.0/vulavula/models/types/intent_classification.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.1/PKG-INFO` & `vulavula-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulavula
-Version: 0.1.1
+Version: 0.2.0
 Summary: The vulavula Python SDK provides access to the Vulavula API.
 Keywords: lelapa,vulavula,nlp,intent,multilingual,transcription
 Author-Email: Raphael Karanja <raphael.karanja@lelapa.ai>
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -142,15 +142,15 @@
 
 #### General Exception Handling
 While `VulavulaError` handles expected API-related errors, your application might encounter other unexpected exceptions. It's important to prepare for these to ensure your application can recover gracefully. 
 
 Here's a general approach to handle unexpected exceptions:
 ```python
 try:
-    response = client.transcribe()
+    upload_id, response = client.transcribe()
     print("Action Succeeded:", response)
 except VulavulaError as e:
     print("Handled VulavulaError:", e.message)
     if 'details' in e.error_data:
         print("Detailed Error Information:", e.error_data['details'])
 except Exception as e:
     print("Unhandled Exception:", str(e))
```

