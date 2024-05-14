# Comparing `tmp/xai_sdk-0.0.4.tar.gz` & `tmp/xai_sdk-0.0.5.tar.gz`

## Comparing `xai_sdk-0.0.4.tar` & `xai_sdk-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,42 @@
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/Makefile
--rwxr-xr-x   0        0        0     1476 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/create_bindings.sh
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/__about__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/__init__.py
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/chat.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/client.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/files.py
--rw-r--r--   0        0        0    22585 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/grok.py
--rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/ide.py
--rw-r--r--   0        0        0    13253 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/sampler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/__init__.py
--rw-r--r--   0        0        0     6903 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/chat_pb2.py
--rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/chat_pb2.pyi
--rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/chat_pb2_grpc.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/files_pb2.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/files_pb2.pyi
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/files_pb2_grpc.py
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/sampler_public_pb2.py
--rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/sampler_public_pb2.pyi
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/sampler_public_pb2_grpc.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/stateless_chat_pb2.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/stateless_chat_pb2.pyi
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/stateless_chat_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/google/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/google/api/__init__.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/google/api/http_pb2.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/src/xai_sdk/proto/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/README.md
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 xai_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/Makefile
+-rwxr-xr-x   0        0        0     1703 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/create_bindings.sh
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/__about__.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/__init__.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/chat.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/client.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/files.py
+-rw-r--r--   0        0        0    22409 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/grok.py
+-rw-r--r--   0        0        0    17016 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/ide.py
+-rw-r--r--   0        0        0    14216 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/sampler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/__init__.py
+-rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/chat_pb2.py
+-rw-r--r--   0        0        0    12809 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/chat_pb2.pyi
+-rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/chat_pb2_grpc.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/files_pb2.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/files_pb2.pyi
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/files_pb2_grpc.py
+-rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/prod_search_pb2.py
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/prod_search_pb2.pyi
+-rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/prod_search_pb2_grpc.py
+-rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/sampler_public_pb2.py
+-rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/sampler_public_pb2.pyi
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/sampler_public_pb2_grpc.py
+-rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/stateless_chat_pb2.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/stateless_chat_pb2.pyi
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/stateless_chat_pb2_grpc.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/x_entities_pb2.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/x_entities_pb2.pyi
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/x_entities_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/http_pb2.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/README.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/PKG-INFO
```

### Comparing `xai_sdk-0.0.4/Makefile` & `xai_sdk-0.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.4/create_bindings.sh` & `xai_sdk-0.0.5/create_bindings.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env bash
 
-python -m grpc_tools.protoc -I../../backend/proto  -I../../backend/proto/google/api --python_out=src/xai_sdk/proto --pyi_out=src/xai_sdk/proto --grpc_python_out=src/xai_sdk/proto ../../backend/proto/chat.proto ../../backend/proto/sampler_public.proto ../../backend/proto/google/api/annotations.proto ../../backend/proto/google/api/http.proto ../../backend/proto/files.proto ../../backend/proto/stateless_chat.proto
+python -m grpc_tools.protoc -I../../backend/proto  -I../../backend/proto/google/api --python_out=src/xai_sdk/proto --pyi_out=src/xai_sdk/proto --grpc_python_out=src/xai_sdk/proto ../../backend/proto/chat.proto ../../backend/proto/prod_search.proto ../../backend/proto/sampler_public.proto ../../backend/proto/google/api/annotations.proto ../../backend/proto/google/api/http.proto ../../backend/proto/files.proto ../../backend/proto/stateless_chat.proto ../../backend/proto/x_entities.proto
 
 # Change imports to be relative
 for file in src/xai_sdk/proto/*; do
   # Check if the file is a regular file
   if [[ -f "$file" ]]; then
     sed -i '' 's/^import sampler_public_pb2/from . import sampler_public_pb2/' "$file"
+    sed -i '' 's/^import prod_search_pb2/from . import prod_search_pb2/' "$file"
     sed -i '' 's/^import chat_pb2/from . import chat_pb2/' "$file"
     sed -i '' 's/^import files_pb2/from . import files_pb2/' "$file"
     sed -i '' 's/^import stateless_chat_pb2/from . import stateless_chat_pb2/' "$file"
+    sed -i '' 's/^import x_entities/from . import x_entities/' "$file"
     sed -i '' 's/^from google.api/from .google.api/' "$file"
   fi
 done
 
 for file in src/xai_sdk/proto/google/api/*; do
   if [[ -f "$file" ]]; then
     sed -i '' 's/^from google.api import/from . import/' "$file"
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/__init__.py` & `xai_sdk-0.0.5/src/xai_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.4/src/xai_sdk/chat.py` & `xai_sdk-0.0.5/src/xai_sdk/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,15 @@
         return self._conversation.responses
 
     @property
     def fun_mode(self) -> bool:
         """Returns true if the conversation happens in fun mode."""
         return self._conversation.system_prompt_name == "fun"
 
-    async def add_response_no_stream(
-        self, user_message: str
-    ) -> stateless_chat_pb2.StatelessResponse:
+    async def add_response_no_stream(self, user_message: str) -> stateless_chat_pb2.StatelessResponse:
         """Same as `add_response` but doesn't return a token stream.
 
         Use this function if you are only interested in the complete response and don't need to
         stream the individual tokens.
 
         Args:
             user_message: Message the user has entered.
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/client.py` & `xai_sdk-0.0.5/src/xai_sdk/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,37 +26,39 @@
 
     def __init__(
         self,
         api_key: Optional[str] = None,
         *,
         initial_rng_seed: Optional[int] = None,
         api_host: str = "api.x.ai",
+        metadata: Optional[tuple[tuple[str, str]]] = None,
     ) -> None:
         """Initializes a new instance of the `Client` class.
 
         Args:
             api_key: API key to use. If unspecified, the API key is read from the `XAI_API_KEY`
                 environment variable.
             initial_rng_seed: Used to make calls to the API deterministic given the initial seed and
                 the order of API calls. If unspecified, a random seed will be sampled for every new
                 instance of the `Client` class.
             api_host: Hostname of the API server.
+            metadata: Metadata to be sent with each gRPC request. Each tuple should contain a key/value pair
 
         Raises:
             ValueError: If the `XAI_API_KEY` environment variable is not set.
             ValueError: If the API key is empty.
         """
         if api_key is None:
             api_key = _get_api_from_env()
 
         if not api_key:
             raise ValueError("Empty xAI API key provided.")
 
         # Create a channel to connect to the API host. Use the API key for authentication.
-        call_credentials = grpc.metadata_call_credentials(_APIAuthPlugin(api_key))
+        call_credentials = grpc.metadata_call_credentials(_APIAuthPlugin(api_key, metadata))
         channel_credentials = grpc.ssl_channel_credentials()
         credentials = grpc.composite_channel_credentials(channel_credentials, call_credentials)
         async_channel = grpc.aio.secure_channel(api_host, credentials)
 
         # Create the stubs used by the SDK. Note that they don't create any connections until being
         # used.
         self.sampler = sampler.AsyncSampler(
@@ -75,31 +77,39 @@
 
     Raises:
         ValueError: If the `XAI_API_KEY` environment variable is not set.
     """
     api_key = os.environ.get("XAI_API_KEY")
     if api_key is None:
         raise ValueError(
-            "Trying to read the xAI API key from the XAI_API_KEY environment variable "
-            "but it doesn't exist."
+            "Trying to read the xAI API key from the XAI_API_KEY environment variable but it doesn't exist."
         )
     else:
         return api_key
 
 
 class _APIAuthPlugin(grpc.AuthMetadataPlugin):
     """A specification for API-key based authentication."""
 
-    def __init__(self, api_key: str) -> None:
+    def __init__(self, api_key: str, metadata) -> None:
         """Initializes a new instance of the `_APIAuthPlugin` class.
 
         Args:
             api_key: A valid xAI API key.
+            metadata: Metadata to be sent with each gRPC request. Each tuple should contain a key/value pair
         """
         self._api_key = api_key
+        self._metadata = metadata
 
     def __call__(
         self, context: grpc.AuthMetadataPluginCallback, callback: grpc.AuthMetadataPluginCallback
     ):
         """See `grpc.AuthMetadataPlugin.__call__`."""
         del context  # Unused.
-        callback((("apikey", self._api_key),), None)
+
+        api_key = ("apikey", self._api_key)
+        if self._metadata is not None:
+            metadata = self._metadata + (api_key,)
+        else:
+            metadata = (api_key,)
+        callback(metadata, None)
+
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/files.py` & `xai_sdk-0.0.5/src/xai_sdk/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,29 +41,25 @@
             local_file_name: Local filename.
             remote_file_name: Name of the file in the IDE.
         """
         # Read the file content.
         with open(local_file_name, "rb") as f:
             await self.upload(remote_file_name, f.read())
 
-    async def upload(
-        self, file_name: str, content: bytes, mime_type: str = "", overwrite: bool = True
-    ) -> None:
+    async def upload(self, file_name: str, content: bytes, mime_type: str = "", overwrite: bool = True) -> None:
         """Creates a new file in the IDE.
 
         Args:
             file_name: Name of the file in the IDE.
             content: File contents.
             mime_type: Mime type of the file.
             overwrite: True if the file shall be overwritten when it's re-uploaded.
         """
         await self._stub.UploadFile(
-            files_pb2.UploadFileRequest(
-                file_name=file_name, content=content, mime_type=mime_type, overwrite=overwrite
-            )
+            files_pb2.UploadFileRequest(file_name=file_name, content=content, mime_type=mime_type, overwrite=overwrite)
         )
 
     async def list(self) -> list[files_pb2.FileMetadata]:
         """Returns the metadata of all files stored in the IDE.
 
         Returns:
             Metadata of all uploaded files.
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/grok.py` & `xai_sdk-0.0.5/src/xai_sdk/grok.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,15 @@
         """
         c = Conversation(self._stub, model_name, fun_mode, conversation_id)
         await c.load()
         return c
 
     async def list_conversations(self) -> list[chat_pb2.Conversation]:
         """Returns a list of all conversations."""
-        response: chat_pb2.ListConversationsResponse = await self._stub.ListConversations(
-            empty_pb2.Empty()
-        )
+        response: chat_pb2.ListConversationsResponse = await self._stub.ListConversations(empty_pb2.Empty())
         return list(response.conversations)
 
 
 class Conversation:
     """SDK for interacting with a Grok conversation.
 
     A Grok conversation is composed of a forest of responses. It's not a tree because there can be
@@ -222,35 +220,29 @@
             raise ValueError("Cannot load conversation without providing conversation ID.")
 
         self._conversation = await self._stub.GetConversation(
             chat_pb2.GetConversationRequest(conversation_id=self._conversation_id)
         )
 
         # Clear the response cache.
-        self._responses = {
-            r.response_id: Response(r, self, self._stub) for r in self._conversation.responses
-        }
+        self._responses = {r.response_id: Response(r, self, self._stub) for r in self._conversation.responses}
 
         # Update the leave response ID to the most recently generated message.
         if self._conversation.responses:
             self._leaf_response_id = self._conversation.responses[-1].response_id
 
     async def delete(self):
         """Deletes this conversation."""
         self._check_not_deleted()
         await self._stub.DeleteConversation(
-            chat_pb2.DeleteConversationRequest(
-                conversation_id=self._get_conversation_or_raise().conversation_id
-            )
+            chat_pb2.DeleteConversationRequest(conversation_id=self._get_conversation_or_raise().conversation_id)
         )
         self._deleted = True
 
-    def add_response(
-        self, user_message: str
-    ) -> tuple[AsyncGenerator[str, "Response"], asyncio.Future["Response"]]:
+    def add_response(self, user_message: str) -> tuple[AsyncGenerator[str, "Response"], asyncio.Future["Response"]]:
         """Adds a new response to this conversation.
 
         The response is added to the graph with its parent being the current `leaf` response.
 
         Args:
             user_message: Message written by the user. If empty, no user response is generated.
 
@@ -371,17 +363,15 @@
         Don't use this API unless you know what you're doing.
         """
         self._check_not_deleted()
         self._responses[response.response_id] = response
 
     async def _create_conversation(self):
         """Creates a new conversation."""
-        conversation: chat_pb2.Conversation = await self._stub.CreateConversation(
-            chat_pb2.CreateConversationRequest()
-        )
+        conversation: chat_pb2.Conversation = await self._stub.CreateConversation(chat_pb2.CreateConversationRequest())
         self._conversation_id = conversation.conversation_id
         self._conversation = conversation
 
     def _get_conversation_or_raise(self) -> chat_pb2.Conversation:
         """Returns the conversation proto or raises an error if the proto hasn't been loaded.
 
         Raises:
@@ -403,31 +393,27 @@
 
 class Response:
     """Represents a single response in a conversation.
 
     Note that the properties of the response are cached client-side. Call the refresh function
     """
 
-    def __init__(
-        self, response: chat_pb2.Response, conversation: Conversation, stub: chat_pb2_grpc.ChatStub
-    ):
+    def __init__(self, response: chat_pb2.Response, conversation: Conversation, stub: chat_pb2_grpc.ChatStub):
         """Initializes a new instance of the `Response` class.
 
         Args:
             response: Raw proto response object returned from the API.
             conversation: Conversation this response belongs to.
             stub: Stub used to communicate with the xAI API.
         """
         self._response = response
         self._conversation = conversation
         self._stub = stub
 
-    def replace(
-        self, new_message: str
-    ) -> tuple[AsyncGenerator[str, "Response"], asyncio.Future["Response"]]:
+    def replace(self, new_message: str) -> tuple[AsyncGenerator[str, "Response"], asyncio.Future["Response"]]:
         """Replaces the text of this message with a new text.
 
         Note: If this is a user response, a new model response will be sampled. If this is a model
         response, it will be replaced by a new response with the given message. In both cases, the
         return value is a model response.
         """
         if self.sender == "human":
@@ -501,17 +487,15 @@
         Raises:
             KeyError: If the parent response cannot be found.
         """
         if self.parent_response_id is not None:
             try:
                 return self._conversation.get_response(self.parent_response_id)
             except KeyError as e:
-                raise KeyError(
-                    f"Cannot find parent response with ID {self.parent_response_id}."
-                ) from e
+                raise KeyError(f"Cannot find parent response with ID {self.parent_response_id}.") from e
         return None
 
     @property
     def children(self) -> list["Response"]:
         """Returns a list of all child responses."""
         return list(self._conversation.get_children(self.response_id))
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/ide.py` & `xai_sdk-0.0.5/src/xai_sdk/ide.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,16 +249,15 @@
         Returns:
             The generated text.
         """
         if rng_seed is None:
             rng_seed = self._get_next_rng_seed()
 
         logging.debug(
-            f"Generating %d tokens [seed=%d, temperature=%f, "
-            f"nucleus_p=%f, stop_tokens=%s, stop_strings=%s].",
+            "Generating %d tokens [seed=%d, temperature=%f, nucleus_p=%f, stop_tokens=%s, stop_strings=%s].",
             max_len,
             rng_seed,
             temperature,
             nucleus_p,
             stop_tokens,
             stop_strings,
         )
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/sampler.py` & `xai_sdk-0.0.5/src/xai_sdk/sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,20 @@
 
 import dataclasses
 import logging
 import random
 from typing import AsyncGenerator, Optional, Sequence, Union
 
 from .proto import sampler_public_pb2, sampler_public_pb2_grpc
-
+from .proto.sampler_public_pb2 import PromptInput, TokenIds
 
 class AsyncSampler:
     """Allows sampling from the raw model API. All functions are asynchronous."""
 
-    def __init__(
-        self, stub: sampler_public_pb2_grpc.SamplerStub, initial_rng_seed: Optional[int] = None
-    ):
+    def __init__(self, stub: sampler_public_pb2_grpc.SamplerStub, initial_rng_seed: Optional[int] = None):
         """Initializes a new instance of the `Sampler` class.
 
         Args:
             stub: The gRPC stub to use for interacting with the API.
             initial_rng_seed: First RNG seed to use for sampling. Each time we sample from the model
                 and no RNG seed is explicitly specified, we deterministically generate a new seed
                 based on the initial seed. This ensures that the generated responses are
@@ -70,14 +68,15 @@
 
         return [Token.from_proto(token) for token in tokens]
 
     async def sample(
         self,
         prompt: Union[str, Sequence[int], Sequence["Token"]],
         *,
+        inputs: Sequence[Union[str, int, bytes]] = (),
         model_name: str = "",
         max_len: int = 256,
         temperature: float = 0.7,
         nucleus_p: float = 0.95,
         stop_tokens: Optional[list[str]] = None,
         stop_strings: Optional[list[str]] = None,
         rng_seed: Optional[int] = None,
@@ -85,16 +84,18 @@
         allowed_tokens: Optional[Sequence[Union[int, str]]] = None,
         disallowed_tokens: Optional[Sequence[Union[int, str]]] = None,
         augment_tokens: bool = True,
     ) -> AsyncGenerator["Token", None]:
         """Generates a model response by continuing `prompt`.
 
         Args:
-            prompt: Prompt to continue. This can either be a string, a sequence of token IDs, or a
-                sequence of `Token` instances.
+            prompt: [Deprecated, use inputs instead] Prompt to continue. This can either be a string, a sequence of
+                token IDs, or a sequence of `Token` instances.
+            inputs: Multimodal input of the model. This can be a sequence of strings, token IDs, image in bytes or
+                base64 encoded string.
             model_name: Name of the model to sample from. Leave empty to sample from the default
                 model.
             max_len: Maximum number of tokens to generate.
             temperature: Temperature of the final softmax operation. The lower the temperature, the
                 lower the variance of the token distribution. In the limit, the distribution
                 collapses onto the single token with the highest probability.
             nucleus_p: Threshold of the Top-P sampling technique: We rank all tokens by their
@@ -122,24 +123,20 @@
                 `disallowed_tokens` will be augmented to include both the passed token and the
                 version with leading whitespace. This is useful because most words have two
                 corresponding vocabulary entries: one with leading whitespace and one without.
 
         Yields:
             A sequence of `Token` instances.
         """
-        # If the prompt is empty, there is nothing we can do.
-        if not prompt:
-            return
 
         if rng_seed is None:
             rng_seed = self._get_next_rng_seed()
 
         logging.debug(
-            "Sampling %d tokens [seed=%d, temperature=%f, nucleus_p=%f, stop_tokens=%s, "
-            "stop_strings=%s].",
+            "Sampling %d tokens [seed=%d, temperature=%f, nucleus_p=%f, stop_tokens=%s, stop_strings=%s].",
             max_len,
             rng_seed,
             temperature,
             nucleus_p,
             stop_tokens,
             stop_strings,
         )
@@ -151,36 +148,50 @@
                 stop_tokens = stop_tokens + [f"▁{t}" for t in stop_tokens]
             if allowed_tokens:
                 allowed_tokens = list(allowed_tokens) + [
                     f"▁{t}" for t in allowed_tokens if isinstance(t, str) and not t.startswith("▁")
                 ]
             if disallowed_tokens:
                 disallowed_tokens = list(disallowed_tokens) + [
-                    f"▁{t}"
-                    for t in disallowed_tokens
-                    if isinstance(t, str) and not t.startswith("▁")
+                    f"▁{t}" for t in disallowed_tokens if isinstance(t, str) and not t.startswith("▁")
                 ]
 
-        prompt = await self._prompt_to_token_ids(prompt, model_name)
+        # Convert inputs
+        converted_inputs = []
+        if inputs:
+            for element in inputs:
+                if isinstance(element, str):
+                    if element.startswith("data:image"):
+                        converted_inputs.append(PromptInput(image_base64=element))
+                    converted_inputs.append(PromptInput(text=element))
+                elif isinstance(element, list):
+                    converted_inputs.append(PromptInput(token_ids=TokenIds(element)))
+                elif isinstance(element, bytes):
+                    converted_inputs.append(PromptInput(image_bytes=element))
+                else:
+                    logging.error("Invalid input type %s.", type(element))
+        else:
+            logging.warning("Usage of prompt argument is deprecated. Please use inputs instead.")
+            converted_inputs = (PromptInput(text=prompt),)
+
         request = sampler_public_pb2.SampleTokensRequest(
-            prompt=prompt,
+            inputs=converted_inputs,
             settings=sampler_public_pb2.SampleSettings(
                 max_len=max_len or 0,
                 temperature=temperature,
                 nucleus_p=nucleus_p,
                 stop_tokens=stop_tokens or [],
                 stop_strings=stop_strings or [],
                 rng_seed=rng_seed,
                 allowed_tokens=[_parse_input_token(t) for t in allowed_tokens or []],
                 disallowed_tokens=[_parse_input_token(t) for t in disallowed_tokens or []],
             ),
             return_attention=return_attention,
             model_name=model_name,
         )
-
         response = self._stub.SampleTokens(request)
 
         token_counter = 0
         async for token in response:
             if token.HasField("token"):
                 token_counter += 1
                 if token_counter % 10 == 0:
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/proto/chat_pb2.py` & `xai_sdk-0.0.5/src/xai_sdk/proto/prod_search_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,74 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: chat.proto
+# source: prod_search.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from . import x_entities_pb2 as x__entities__pb2
 
-from . import sampler_public_pb2 as sampler__public__pb2
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nchat.proto\x12\nprompt_ide\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x14sampler_public.proto\"I\n\x19RegenerateResponseRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x13\n\x0bresponse_id\x18\x02 \x01(\t\"\x1b\n\x19\x43reateConversationRequest\"1\n\x16GetConversationRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\"4\n\x19\x44\x65leteConversationRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\"L\n\x19ListConversationsResponse\x12/\n\rconversations\x18\x01 \x03(\x0b\x32\x18.prompt_ide.Conversation\"I\n\x14GenerateTitleRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x18\n\x10leaf_response_id\x18\x02 \x01(\t\"*\n\x15GenerateTitleResponse\x12\x11\n\tnew_title\x18\x01 \x01(\t\"p\n\x17\x41\x64\x64ModelResponseRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x0f\n\x07partial\x18\x03 \x01(\x08\x12\x1a\n\x12parent_response_id\x18\x04 \x01(\t\"T\n\x19UpdateConversationRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0f\n\x07starred\x18\x03 \x01(\x08\"\xa2\x01\n\x12\x41\x64\x64ResponseRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x12\n\nmodel_name\x18\x03 \x01(\t\x12\x1a\n\x12parent_response_id\x18\x05 \x01(\t\x12\x10\n\x08use_grok\x18\x06 \x01(\x08\x12\x1a\n\x12system_prompt_name\x18\x07 \x01(\tJ\x04\x08\x04\x10\x05\"\xe4\x01\n\x13\x41\x64\x64ResponseResponse\x12-\n\ruser_response\x18\x01 \x01(\x0b\x32\x14.prompt_ide.ResponseH\x00\x12\x31\n\x05token\x18\x02 \x01(\x0b\x32 .prompt_ide.SampleTokensResponseH\x00\x12.\n\x0emodel_response\x18\x03 \x01(\x0b\x32\x14.prompt_ide.ResponseH\x00\x12/\n\x0cquery_action\x18\x04 \x01(\x0b\x32\x17.prompt_ide.QueryActionH\x00\x42\n\n\x08response\"*\n\x0bQueryAction\x12\r\n\x05query\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\xd2\x01\n\x0c\x43onversation\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0f\n\x07starred\x18\x06 \x01(\x08\x12/\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodify_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\tresponses\x18\x05 \x03(\x0b\x32\x14.prompt_ide.Response\"\xe1\x01\n\x08Response\x12\x13\n\x0bresponse_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x0e\n\x06sender\x18\x03 \x01(\t\x12/\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12parent_response_id\x18\x05 \x01(\t\x12\x0e\n\x06manual\x18\x06 \x01(\x08\x12\x0f\n\x07partial\x18\x07 \x01(\x08\x12\x0e\n\x06shared\x18\x08 \x01(\x08\x12\r\n\x05query\x18\t \x01(\t\x12\x12\n\nquery_type\x18\n \x01(\t\"H\n\x18ShareConversationRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x13\n\x0bresponse_id\x18\x02 \x01(\t\".\n\x19ShareConversationResponse\x12\x11\n\tshared_id\x18\x01 \x01(\t2\x99\x06\n\x04\x43hat\x12W\n\x12\x43reateConversation\x12%.prompt_ide.CreateConversationRequest\x1a\x18.prompt_ide.Conversation\"\x00\x12Q\n\x0fGetConversation\x12\".prompt_ide.GetConversationRequest\x1a\x18.prompt_ide.Conversation\"\x00\x12T\n\x11ListConversations\x12\x16.google.protobuf.Empty\x1a%.prompt_ide.ListConversationsResponse\"\x00\x12R\n\x0b\x41\x64\x64Response\x12\x1e.prompt_ide.AddResponseRequest\x1a\x1f.prompt_ide.AddResponseResponse\"\x00\x30\x01\x12U\n\x12\x44\x65leteConversation\x12%.prompt_ide.DeleteConversationRequest\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\rGenerateTitle\x12 .prompt_ide.GenerateTitleRequest\x1a!.prompt_ide.GenerateTitleResponse\"\x00\x12W\n\x12UpdateConversation\x12%.prompt_ide.UpdateConversationRequest\x1a\x18.prompt_ide.Conversation\"\x00\x12O\n\x10\x41\x64\x64ModelResponse\x12#.prompt_ide.AddModelResponseRequest\x1a\x14.prompt_ide.Response\"\x00\x12\x62\n\x11ShareConversation\x12$.prompt_ide.ShareConversationRequest\x1a%.prompt_ide.ShareConversationResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11prod_search.proto\x12\nprompt_ide\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x10x_entities.proto\";\n\x18GetXCuratedTrendsRequest\x12\r\n\x05limit\x18\x01 \x01(\x05\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\"E\n\x19GetXCuratedTrendsResponse\x12(\n\x06trends\x18\x01 \x03(\x0b\x32\x18.prompt_ide.XTrendResult\"\"\n\x14GetXTrendByIdRequest\x12\n\n\x02id\x18\x01 \x01(\t\"@\n\x15GetXTrendByIdResponse\x12\'\n\x05trend\x18\x01 \x01(\x0b\x32\x18.prompt_ide.XTrendResult\"\xb2\x01\n\rSearchRequest\x12\r\n\x05query\x18\x01 \x01(\t\x12\x15\n\rforce_refresh\x18\x02 \x01(\x08\x12\x12\n\nmodel_name\x18\x03 \x01(\t\x12\x0e\n\x06prompt\x18\x04 \x01(\t\x12\x11\n\tsearch_id\x18\x05 \x01(\t\x12\x17\n\x0f\x62\x61\x63kend_address\x18\x06 \x01(\t\x12\x12\n\nforce_rust\x18\x07 \x01(\x08\x12\x17\n\x0fimage_generator\x18\x08 \x01(\t\"\xe1\x02\n\x0eSearchResponse\x12\x36\n\x10x_search_results\x18\x01 \x01(\x0b\x32\x1a.prompt_ide.XSearchResultsH\x00\x12:\n\x12web_search_results\x18\x02 \x01(\x0b\x32\x1c.prompt_ide.WebSearchResultsH\x00\x12\x0e\n\x04text\x18\x03 \x01(\tH\x00\x12\x46\n\x18image_generation_results\x18\x04 \x01(\x0b\x32\".prompt_ide.ImageGenerationResultsH\x00\x12\x34\n\x0fx_trend_results\x18\x05 \x01(\x0b\x32\x19.prompt_ide.XTrendResultsH\x00\x12\x13\n\tsearch_id\x18\x06 \x01(\tH\x00\x12-\n\x05\x64\x65\x62ug\x18\x07 \x01(\x0b\x32\x1c.prompt_ide.DebugInformationH\x00\x42\t\n\x07payload\"4\n\x0eXSearchResults\x12\"\n\x07results\x18\x01 \x03(\x0b\x32\x11.prompt_ide.XPost\":\n\rXTrendResults\x12)\n\x07results\x18\x01 \x03(\x0b\x32\x18.prompt_ide.XTrendResult\"\xe6\x01\n\x0fWebSearchResult\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0f\n\x07preview\x18\x04 \x01(\t\x12\x1a\n\x12search_engine_text\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x11\n\tsite_name\x18\x07 \x01(\t\x12\x16\n\x0emetadata_title\x18\x08 \x01(\t\x12\x0f\n\x07\x63reator\x18\t \x01(\t\x12\r\n\x05image\x18\n \x01(\t\x12\x0f\n\x07\x66\x61vicon\x18\x0b \x01(\t\x12\x13\n\x0b\x63itation_id\x18\x0c \x01(\tJ\x04\x08\x03\x10\x04\"@\n\x10WebSearchResults\x12,\n\x07results\x18\x01 \x03(\x0b\x32\x1b.prompt_ide.WebSearchResult\":\n\x15ImageGenerationResult\x12\x11\n\timage_url\x18\x01 \x01(\t\x12\x0e\n\x06prompt\x18\x02 \x01(\t\"e\n\x16ImageGenerationResults\x12\x32\n\x07results\x18\x01 \x03(\x0b\x32!.prompt_ide.ImageGenerationResult\x12\x17\n\x0fimage_generator\x18\x02 \x01(\t\"F\n\x1fGetMostRecentSearchQueryRequest\x12\r\n\x05limit\x18\x01 \x01(\x05\x12\x14\n\x0cquery_prefix\x18\x02 \x01(\t\"/\n\x0bSearchQuery\x12\x11\n\tsearch_id\x18\x01 \x01(\t\x12\r\n\x05query\x18\x02 \x01(\t\"?\n\x13SearchQueryResponse\x12(\n\x07queries\x18\x01 \x03(\x0b\x32\x17.prompt_ide.SearchQuery\"-\n\x18\x44\x65leteSearchQueryRequest\x12\x11\n\tsearch_id\x18\x01 \x01(\t\"%\n\x14\x43ompleteQueryRequest\x12\r\n\x05query\x18\x01 \x01(\t\"&\n\x15\x43ompleteQueryResponse\x12\r\n\x05query\x18\x01 \x01(\t\"P\n\x19SummarizeWebResultRequest\x12\r\n\x05query\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x17\n\x0f\x62\x61\x63kend_address\x18\x03 \x01(\t\",\n\x1aSummarizeWebResultResponse\x12\x0e\n\x06\x61nswer\x18\x01 \x01(\t\"h\n\x17WebsiteDebugInformation\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x10\n\x08raw_html\x18\x02 \x01(\t\x12\x13\n\x0bparsed_text\x18\x03 \x01(\t\x12\x19\n\x11summarized_chunks\x18\x04 \x03(\t\"i\n\x10\x44\x65\x62ugInformation\x12\x1e\n\x16\x66ormatted_model_prompt\x18\x01 \x01(\t\x12\x35\n\x08websites\x18\x02 \x03(\x0b\x32#.prompt_ide.WebsiteDebugInformation2\x8b\x05\n\x06Search\x12\x43\n\x06Search\x12\x19.prompt_ide.SearchRequest\x1a\x1a.prompt_ide.SearchResponse\"\x00\x30\x01\x12j\n\x18GetMostRecentSearchQuery\x12+.prompt_ide.GetMostRecentSearchQueryRequest\x1a\x1f.prompt_ide.SearchQueryResponse\"\x00\x12S\n\x11\x44\x65leteSearchQuery\x12$.prompt_ide.DeleteSearchQueryRequest\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\rCompleteQuery\x12 .prompt_ide.CompleteQueryRequest\x1a!.prompt_ide.CompleteQueryResponse\"\x00\x12g\n\x12SummarizeWebResult\x12%.prompt_ide.SummarizeWebResultRequest\x1a&.prompt_ide.SummarizeWebResultResponse\"\x00\x30\x01\x12\x62\n\x11GetXCuratedTrends\x12$.prompt_ide.GetXCuratedTrendsRequest\x1a%.prompt_ide.GetXCuratedTrendsResponse\"\x00\x12V\n\rGetXTrendById\x12 .prompt_ide.GetXTrendByIdRequest\x1a!.prompt_ide.GetXTrendByIdResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'chat_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prod_search_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
-  _globals['_REGENERATERESPONSEREQUEST']._serialized_start=110
-  _globals['_REGENERATERESPONSEREQUEST']._serialized_end=183
-  _globals['_CREATECONVERSATIONREQUEST']._serialized_start=185
-  _globals['_CREATECONVERSATIONREQUEST']._serialized_end=212
-  _globals['_GETCONVERSATIONREQUEST']._serialized_start=214
-  _globals['_GETCONVERSATIONREQUEST']._serialized_end=263
-  _globals['_DELETECONVERSATIONREQUEST']._serialized_start=265
-  _globals['_DELETECONVERSATIONREQUEST']._serialized_end=317
-  _globals['_LISTCONVERSATIONSRESPONSE']._serialized_start=319
-  _globals['_LISTCONVERSATIONSRESPONSE']._serialized_end=395
-  _globals['_GENERATETITLEREQUEST']._serialized_start=397
-  _globals['_GENERATETITLEREQUEST']._serialized_end=470
-  _globals['_GENERATETITLERESPONSE']._serialized_start=472
-  _globals['_GENERATETITLERESPONSE']._serialized_end=514
-  _globals['_ADDMODELRESPONSEREQUEST']._serialized_start=516
-  _globals['_ADDMODELRESPONSEREQUEST']._serialized_end=628
-  _globals['_UPDATECONVERSATIONREQUEST']._serialized_start=630
-  _globals['_UPDATECONVERSATIONREQUEST']._serialized_end=714
-  _globals['_ADDRESPONSEREQUEST']._serialized_start=717
-  _globals['_ADDRESPONSEREQUEST']._serialized_end=879
-  _globals['_ADDRESPONSERESPONSE']._serialized_start=882
-  _globals['_ADDRESPONSERESPONSE']._serialized_end=1110
-  _globals['_QUERYACTION']._serialized_start=1112
-  _globals['_QUERYACTION']._serialized_end=1154
-  _globals['_CONVERSATION']._serialized_start=1157
-  _globals['_CONVERSATION']._serialized_end=1367
-  _globals['_RESPONSE']._serialized_start=1370
-  _globals['_RESPONSE']._serialized_end=1595
-  _globals['_SHARECONVERSATIONREQUEST']._serialized_start=1597
-  _globals['_SHARECONVERSATIONREQUEST']._serialized_end=1669
-  _globals['_SHARECONVERSATIONRESPONSE']._serialized_start=1671
-  _globals['_SHARECONVERSATIONRESPONSE']._serialized_end=1717
-  _globals['_CHAT']._serialized_start=1720
-  _globals['_CHAT']._serialized_end=2513
+  _globals['_GETXCURATEDTRENDSREQUEST']._serialized_start=113
+  _globals['_GETXCURATEDTRENDSREQUEST']._serialized_end=172
+  _globals['_GETXCURATEDTRENDSRESPONSE']._serialized_start=174
+  _globals['_GETXCURATEDTRENDSRESPONSE']._serialized_end=243
+  _globals['_GETXTRENDBYIDREQUEST']._serialized_start=245
+  _globals['_GETXTRENDBYIDREQUEST']._serialized_end=279
+  _globals['_GETXTRENDBYIDRESPONSE']._serialized_start=281
+  _globals['_GETXTRENDBYIDRESPONSE']._serialized_end=345
+  _globals['_SEARCHREQUEST']._serialized_start=348
+  _globals['_SEARCHREQUEST']._serialized_end=526
+  _globals['_SEARCHRESPONSE']._serialized_start=529
+  _globals['_SEARCHRESPONSE']._serialized_end=882
+  _globals['_XSEARCHRESULTS']._serialized_start=884
+  _globals['_XSEARCHRESULTS']._serialized_end=936
+  _globals['_XTRENDRESULTS']._serialized_start=938
+  _globals['_XTRENDRESULTS']._serialized_end=996
+  _globals['_WEBSEARCHRESULT']._serialized_start=999
+  _globals['_WEBSEARCHRESULT']._serialized_end=1229
+  _globals['_WEBSEARCHRESULTS']._serialized_start=1231
+  _globals['_WEBSEARCHRESULTS']._serialized_end=1295
+  _globals['_IMAGEGENERATIONRESULT']._serialized_start=1297
+  _globals['_IMAGEGENERATIONRESULT']._serialized_end=1355
+  _globals['_IMAGEGENERATIONRESULTS']._serialized_start=1357
+  _globals['_IMAGEGENERATIONRESULTS']._serialized_end=1458
+  _globals['_GETMOSTRECENTSEARCHQUERYREQUEST']._serialized_start=1460
+  _globals['_GETMOSTRECENTSEARCHQUERYREQUEST']._serialized_end=1530
+  _globals['_SEARCHQUERY']._serialized_start=1532
+  _globals['_SEARCHQUERY']._serialized_end=1579
+  _globals['_SEARCHQUERYRESPONSE']._serialized_start=1581
+  _globals['_SEARCHQUERYRESPONSE']._serialized_end=1644
+  _globals['_DELETESEARCHQUERYREQUEST']._serialized_start=1646
+  _globals['_DELETESEARCHQUERYREQUEST']._serialized_end=1691
+  _globals['_COMPLETEQUERYREQUEST']._serialized_start=1693
+  _globals['_COMPLETEQUERYREQUEST']._serialized_end=1730
+  _globals['_COMPLETEQUERYRESPONSE']._serialized_start=1732
+  _globals['_COMPLETEQUERYRESPONSE']._serialized_end=1770
+  _globals['_SUMMARIZEWEBRESULTREQUEST']._serialized_start=1772
+  _globals['_SUMMARIZEWEBRESULTREQUEST']._serialized_end=1852
+  _globals['_SUMMARIZEWEBRESULTRESPONSE']._serialized_start=1854
+  _globals['_SUMMARIZEWEBRESULTRESPONSE']._serialized_end=1898
+  _globals['_WEBSITEDEBUGINFORMATION']._serialized_start=1900
+  _globals['_WEBSITEDEBUGINFORMATION']._serialized_end=2004
+  _globals['_DEBUGINFORMATION']._serialized_start=2006
+  _globals['_DEBUGINFORMATION']._serialized_end=2111
+  _globals['_SEARCH']._serialized_start=2114
+  _globals['_SEARCH']._serialized_end=2765
 # @@protoc_insertion_point(module_scope)
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/proto/chat_pb2_grpc.py` & `xai_sdk-0.0.5/src/xai_sdk/proto/chat_pb2_grpc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # fmt: off
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 from . import chat_pb2 as chat__pb2
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
 class ChatStub(object):
     """Utility for interacting with a model via a chat-like interface.
     """
 
     def __init__(self, channel):
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/proto/files_pb2.py` & `xai_sdk-0.0.5/src/xai_sdk/proto/files_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: files.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
+
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0b\x66iles.proto\x12\nprompt_ide\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"]\n\x11UploadFileRequest\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\x0c\x12\x11\n\tmime_type\x18\x03 \x01(\t\x12\x11\n\toverwrite\x18\x04 \x01(\x08\"y\n\x0c\x46ileMetadata\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x12\n\nsize_bytes\x18\x02 \x01(\x05\x12\x11\n\tmime_type\x18\x03 \x01(\t\x12/\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x11RenameFileRequest\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x15\n\rnew_file_name\x18\x02 \x01(\t\"(\n\x13\x44ownloadFileRequest\x12\x11\n\tfile_name\x18\x01 \x01(\t\"I\n\nFileObject\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.prompt_ide.FileMetadata\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\x0c\"s\n\x11ListFilesResponse\x12\x14\n\x0cstorage_used\x18\x01 \x01(\x05\x12\x1f\n\x17storage_available_total\x18\x02 \x01(\x05\x12\'\n\x05\x66iles\x18\x03 \x03(\x0b\x32\x18.prompt_ide.FileMetadata\"&\n\x11\x44\x65leteFileRequest\x12\x11\n\tfile_name\x18\x01 \x01(\t2\xf0\x02\n\x04\x46ile\x12G\n\nUploadFile\x12\x1d.prompt_ide.UploadFileRequest\x1a\x18.prompt_ide.FileMetadata\"\x00\x12I\n\x0c\x44ownloadFile\x12\x1f.prompt_ide.DownloadFileRequest\x1a\x16.prompt_ide.FileObject\"\x00\x12\x44\n\tListFiles\x12\x16.google.protobuf.Empty\x1a\x1d.prompt_ide.ListFilesResponse\"\x00\x12G\n\nRenameFile\x12\x1d.prompt_ide.RenameFileRequest\x1a\x18.prompt_ide.FileMetadata\"\x00\x12\x45\n\nDeleteFile\x12\x1d.prompt_ide.DeleteFileRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'files_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_UPLOADFILEREQUEST']._serialized_start=89
   _globals['_UPLOADFILEREQUEST']._serialized_end=182
   _globals['_FILEMETADATA']._serialized_start=184
   _globals['_FILEMETADATA']._serialized_end=305
   _globals['_RENAMEFILEREQUEST']._serialized_start=307
   _globals['_RENAMEFILEREQUEST']._serialized_end=368
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/proto/files_pb2.pyi` & `xai_sdk-0.0.5/src/xai_sdk/proto/files_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,70 @@
-from typing import ClassVar as _ClassVar
-from typing import Iterable as _Iterable
-from typing import Mapping as _Mapping
-from typing import Optional as _Optional
-from typing import Union as _Union
-
-from google.protobuf import descriptor as _descriptor
 from google.protobuf import empty_pb2 as _empty_pb2
-from google.protobuf import message as _message
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf.internal import containers as _containers
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class UploadFileRequest(_message.Message):
-    __slots__ = ["file_name", "content", "mime_type", "overwrite"]
+    __slots__ = ("file_name", "content", "mime_type", "overwrite")
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     CONTENT_FIELD_NUMBER: _ClassVar[int]
     MIME_TYPE_FIELD_NUMBER: _ClassVar[int]
     OVERWRITE_FIELD_NUMBER: _ClassVar[int]
     file_name: str
     content: bytes
     mime_type: str
     overwrite: bool
-    def __init__(
-        self,
-        file_name: _Optional[str] = ...,
-        content: _Optional[bytes] = ...,
-        mime_type: _Optional[str] = ...,
-        overwrite: bool = ...,
-    ) -> None: ...
+    def __init__(self, file_name: _Optional[str] = ..., content: _Optional[bytes] = ..., mime_type: _Optional[str] = ..., overwrite: bool = ...) -> None: ...
 
 class FileMetadata(_message.Message):
-    __slots__ = ["file_name", "size_bytes", "mime_type", "create_time"]
+    __slots__ = ("file_name", "size_bytes", "mime_type", "create_time")
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     SIZE_BYTES_FIELD_NUMBER: _ClassVar[int]
     MIME_TYPE_FIELD_NUMBER: _ClassVar[int]
     CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
     file_name: str
     size_bytes: int
     mime_type: str
     create_time: _timestamp_pb2.Timestamp
-    def __init__(
-        self,
-        file_name: _Optional[str] = ...,
-        size_bytes: _Optional[int] = ...,
-        mime_type: _Optional[str] = ...,
-        create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
-    ) -> None: ...
+    def __init__(self, file_name: _Optional[str] = ..., size_bytes: _Optional[int] = ..., mime_type: _Optional[str] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
 class RenameFileRequest(_message.Message):
-    __slots__ = ["file_name", "new_file_name"]
+    __slots__ = ("file_name", "new_file_name")
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     NEW_FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     file_name: str
     new_file_name: str
-    def __init__(
-        self, file_name: _Optional[str] = ..., new_file_name: _Optional[str] = ...
-    ) -> None: ...
+    def __init__(self, file_name: _Optional[str] = ..., new_file_name: _Optional[str] = ...) -> None: ...
 
 class DownloadFileRequest(_message.Message):
-    __slots__ = ["file_name"]
+    __slots__ = ("file_name",)
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     file_name: str
     def __init__(self, file_name: _Optional[str] = ...) -> None: ...
 
 class FileObject(_message.Message):
-    __slots__ = ["metadata", "content"]
+    __slots__ = ("metadata", "content")
     METADATA_FIELD_NUMBER: _ClassVar[int]
     CONTENT_FIELD_NUMBER: _ClassVar[int]
     metadata: FileMetadata
     content: bytes
-    def __init__(
-        self,
-        metadata: _Optional[_Union[FileMetadata, _Mapping]] = ...,
-        content: _Optional[bytes] = ...,
-    ) -> None: ...
+    def __init__(self, metadata: _Optional[_Union[FileMetadata, _Mapping]] = ..., content: _Optional[bytes] = ...) -> None: ...
 
 class ListFilesResponse(_message.Message):
-    __slots__ = ["storage_used", "storage_available_total", "files"]
+    __slots__ = ("storage_used", "storage_available_total", "files")
     STORAGE_USED_FIELD_NUMBER: _ClassVar[int]
     STORAGE_AVAILABLE_TOTAL_FIELD_NUMBER: _ClassVar[int]
     FILES_FIELD_NUMBER: _ClassVar[int]
     storage_used: int
     storage_available_total: int
     files: _containers.RepeatedCompositeFieldContainer[FileMetadata]
-    def __init__(
-        self,
-        storage_used: _Optional[int] = ...,
-        storage_available_total: _Optional[int] = ...,
-        files: _Optional[_Iterable[_Union[FileMetadata, _Mapping]]] = ...,
-    ) -> None: ...
+    def __init__(self, storage_used: _Optional[int] = ..., storage_available_total: _Optional[int] = ..., files: _Optional[_Iterable[_Union[FileMetadata, _Mapping]]] = ...) -> None: ...
 
 class DeleteFileRequest(_message.Message):
-    __slots__ = ["file_name"]
+    __slots__ = ("file_name",)
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     file_name: str
     def __init__(self, file_name: _Optional[str] = ...) -> None: ...
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/proto/files_pb2_grpc.py` & `xai_sdk-0.0.5/src/xai_sdk/proto/files_pb2_grpc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # fmt: off
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 from . import files_pb2 as files__pb2
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
 class FileStub(object):
     """Service for uploading, downloading, and deleting files. We only allow storing somewhat small
     files using this service (e.g. 5 MiB - check the implementation for details).
     """
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/proto/sampler_public_pb2.py` & `xai_sdk-0.0.5/src/xai_sdk/proto/sampler_public_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,75 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: sampler_public.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from .google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
-from .google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14sampler_public.proto\x12\nprompt_ide\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x8d\x01\n\x13SampleTokensRequest\x12\x0e\n\x06prompt\x18\x01 \x03(\r\x12,\n\x08settings\x18\x02 \x01(\x0b\x32\x1a.prompt_ide.SampleSettings\x12\x18\n\x10return_attention\x18\x04 \x01(\x08\x12\x12\n\nmodel_name\x18\x05 \x01(\tJ\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07\"w\n\x14SampleTokensResponse\x12\"\n\x05token\x18\x01 \x01(\x0b\x32\x11.prompt_ide.TokenH\x00\x12)\n\x06\x62udget\x18\x02 \x01(\x0b\x32\x17.prompt_ide.TokenBudgetH\x00\x42\n\n\x08responseJ\x04\x08\x03\x10\x04\"\xe9\x01\n\x0eSampleSettings\x12\x0f\n\x07max_len\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x02\x12\x11\n\tnucleus_p\x18\x03 \x01(\x02\x12\x13\n\x0bstop_tokens\x18\x04 \x03(\t\x12\x14\n\x0cstop_strings\x18\x07 \x03(\t\x12\x10\n\x08rng_seed\x18\x05 \x01(\x04\x12.\n\x0e\x61llowed_tokens\x18\x06 \x03(\x0b\x32\x16.prompt_ide.InputToken\x12\x31\n\x11\x64isallowed_tokens\x18\x08 \x03(\x0b\x32\x16.prompt_ide.InputToken\"A\n\nInputToken\x12\x16\n\x0cstring_token\x18\x01 \x01(\tH\x00\x12\x12\n\x08token_id\x18\x02 \x01(\rH\x00\x42\x07\n\x05token\"\xca\x01\n\x05Token\x12&\n\x0b\x66inal_logit\x18\x01 \x01(\x0b\x32\x11.prompt_ide.Logit\x12 \n\x05top_k\x18\x04 \x03(\x0b\x32\x11.prompt_ide.Logit\x12\x11\n\tattention\x18\x05 \x03(\x02\x12/\n\ntoken_type\x18\x03 \x01(\x0e\x32\x1b.prompt_ide.Token.TokenType\"-\n\tTokenType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04USER\x10\x01\x12\t\n\x05MODEL\x10\x02J\x04\x08\x02\x10\x03\"=\n\x05Logit\x12\x10\n\x08token_id\x18\x01 \x01(\r\x12\x14\n\x0cstring_token\x18\x02 \x01(\t\x12\x0c\n\x04prob\x18\x03 \x01(\x02\"3\n\x0fTokenizeRequest\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\"5\n\x10TokenizeResponse\x12!\n\x06tokens\x18\x01 \x03(\x0b\x32\x11.prompt_ide.Token\"N\n\x18ListTransactionsResponse\x12\x32\n\x0ctransactions\x18\x01 \x03(\x0b\x32\x1c.prompt_ide.TokenTransaction\"\x95\x01\n\x10TokenTransaction\x12\x19\n\x11num_prompt_tokens\x18\x01 \x01(\x05\x12\x1c\n\x14num_generated_tokens\x18\x02 \x01(\x05\x12\x17\n\x0f\x63ost_multiplier\x18\x03 \x01(\x05\x12/\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"8\n\x0bTokenBudget\x12\x13\n\x0btoken_limit\x18\x01 \x01(\x05\x12\x14\n\x0ctokens_spent\x18\x02 \x01(\x05\x32\xcd\x03\n\x07Sampler\x12{\n\x0cSampleTokens\x12\x1f.prompt_ide.SampleTokensRequest\x1a .prompt_ide.SampleTokensResponse\"&\x82\xd3\xe4\x93\x02 \"\x1b/rest/sampler/sample-tokens:\x01*0\x01\x12h\n\x08Tokenize\x12\x1b.prompt_ide.TokenizeRequest\x1a\x1c.prompt_ide.TokenizeResponse\"!\x82\xd3\xe4\x93\x02\x1b\"\x16/rest/sampler/tokenize:\x01*\x12t\n\x10ListTransactions\x12\x16.google.protobuf.Empty\x1a$.prompt_ide.ListTransactionsResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/rest/sampler/transactions\x12\x65\n\x0eGetTokenBudget\x12\x16.google.protobuf.Empty\x1a\x17.prompt_ide.TokenBudget\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/rest/sampler/token-budgetB\x1cZ\x1ax.ai/prompt_ide;prompt_ideb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14sampler_public.proto\x12\nprompt_ide\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xba\x01\n\x13SampleTokensRequest\x12\x12\n\x06prompt\x18\x01 \x03(\rB\x02\x18\x01\x12\'\n\x06inputs\x18\x07 \x03(\x0b\x32\x17.prompt_ide.PromptInput\x12,\n\x08settings\x18\x02 \x01(\x0b\x32\x1a.prompt_ide.SampleSettings\x12\x18\n\x10return_attention\x18\x04 \x01(\x08\x12\x12\n\nmodel_name\x18\x05 \x01(\tJ\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07\"\x82\x01\n\x0bPromptInput\x12\x0e\n\x04text\x18\x01 \x01(\tH\x00\x12\x15\n\x0bimage_bytes\x18\x02 \x01(\x0cH\x00\x12\x16\n\x0cimage_base64\x18\x03 \x01(\tH\x00\x12)\n\ttoken_ids\x18\x04 \x01(\x0b\x32\x14.prompt_ide.TokenIdsH\x00\x42\t\n\x07payload\"\x1a\n\x08TokenIds\x12\x0e\n\x06tokens\x18\x01 \x03(\r\"\xac\x01\n\x14SampleTokensResponse\x12\"\n\x05token\x18\x01 \x01(\x0b\x32\x11.prompt_ide.TokenH\x00\x12)\n\x06\x62udget\x18\x02 \x01(\x0b\x32\x17.prompt_ide.TokenBudgetH\x00\x12\x33\n\x0btransaction\x18\x04 \x01(\x0b\x32\x1c.prompt_ide.TokenTransactionH\x00\x42\n\n\x08responseJ\x04\x08\x03\x10\x04\"\x8a\x01\n\x1eTokenizeAndSampleTokensRequest\x12\x0c\n\x04text\x18\x01 \x01(\t\x12,\n\x08settings\x18\x02 \x01(\x0b\x32\x1a.prompt_ide.SampleSettings\x12\x18\n\x10return_attention\x18\x04 \x01(\x08\x12\x12\n\nmodel_name\x18\x05 \x01(\t\"\xe9\x01\n\x0eSampleSettings\x12\x0f\n\x07max_len\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x02\x12\x11\n\tnucleus_p\x18\x03 \x01(\x02\x12\x13\n\x0bstop_tokens\x18\x04 \x03(\t\x12\x14\n\x0cstop_strings\x18\x07 \x03(\t\x12\x10\n\x08rng_seed\x18\x05 \x01(\x04\x12.\n\x0e\x61llowed_tokens\x18\x06 \x03(\x0b\x32\x16.prompt_ide.InputToken\x12\x31\n\x11\x64isallowed_tokens\x18\x08 \x03(\x0b\x32\x16.prompt_ide.InputToken\"A\n\nInputToken\x12\x16\n\x0cstring_token\x18\x01 \x01(\tH\x00\x12\x12\n\x08token_id\x18\x02 \x01(\rH\x00\x42\x07\n\x05token\"\xca\x01\n\x05Token\x12&\n\x0b\x66inal_logit\x18\x01 \x01(\x0b\x32\x11.prompt_ide.Logit\x12 \n\x05top_k\x18\x04 \x03(\x0b\x32\x11.prompt_ide.Logit\x12\x11\n\tattention\x18\x05 \x03(\x02\x12/\n\ntoken_type\x18\x03 \x01(\x0e\x32\x1b.prompt_ide.Token.TokenType\"-\n\tTokenType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04USER\x10\x01\x12\t\n\x05MODEL\x10\x02J\x04\x08\x02\x10\x03\"=\n\x05Logit\x12\x10\n\x08token_id\x18\x01 \x01(\r\x12\x14\n\x0cstring_token\x18\x02 \x01(\t\x12\x0c\n\x04prob\x18\x03 \x01(\x02\"3\n\x0fTokenizeRequest\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\"5\n\x10TokenizeResponse\x12!\n\x06tokens\x18\x01 \x03(\x0b\x32\x11.prompt_ide.Token\"N\n\x18ListTransactionsResponse\x12\x32\n\x0ctransactions\x18\x01 \x03(\x0b\x32\x1c.prompt_ide.TokenTransaction\"\xee\x01\n\x10TokenTransaction\x12\x19\n\x11num_prompt_tokens\x18\x01 \x01(\x05\x12\x1c\n\x14num_generated_tokens\x18\x02 \x01(\x05\x12\x17\n\x0f\x63ost_multiplier\x18\x03 \x01(\x05\x12/\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10transaction_type\x18\x05 \x01(\t\x12\x16\n\x0etransaction_id\x18\x06 \x01(\t\x12\x12\n\nmodel_name\x18\x07 \x01(\t\x12\x11\n\tconfirmed\x18\x08 \x01(\x08\"1\n\x15GetTokenBudgetRequest\x12\x18\n\x10transaction_type\x18\x01 \x01(\t\"g\n\x0bTokenBudget\x12\x13\n\x0btoken_limit\x18\x01 \x01(\x05\x12\x14\n\x0ctokens_spent\x18\x02 \x01(\x05\x12\x15\n\rrequest_limit\x18\x03 \x01(\x05\x12\x16\n\x0erequests_spent\x18\x04 \x01(\x05\x32\xf9\x04\n\x07Sampler\x12{\n\x0cSampleTokens\x12\x1f.prompt_ide.SampleTokensRequest\x1a .prompt_ide.SampleTokensResponse\"&\x82\xd3\xe4\x93\x02 \"\x1b/rest/sampler/sample-tokens:\x01*0\x01\x12h\n\x08Tokenize\x12\x1b.prompt_ide.TokenizeRequest\x1a\x1c.prompt_ide.TokenizeResponse\"!\x82\xd3\xe4\x93\x02\x1b\"\x16/rest/sampler/tokenize:\x01*\x12\x9e\x01\n\x17TokenizeAndSampleTokens\x12*.prompt_ide.TokenizeAndSampleTokensRequest\x1a .prompt_ide.SampleTokensResponse\"3\x82\xd3\xe4\x93\x02-\"(/rest/sampler/tokenize-and-sample-tokens:\x01*0\x01\x12t\n\x10ListTransactions\x12\x16.google.protobuf.Empty\x1a$.prompt_ide.ListTransactionsResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/rest/sampler/transactions\x12p\n\x0eGetTokenBudget\x12!.prompt_ide.GetTokenBudgetRequest\x1a\x17.prompt_ide.TokenBudget\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/rest/sampler/token-budgetB\x1cZ\x1ax.ai/prompt_ide;prompt_ideb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sampler_public_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\032x.ai/prompt_ide;prompt_ide'
-  _SAMPLER.methods_by_name['SampleTokens']._options = None
-  _SAMPLER.methods_by_name['SampleTokens']._serialized_options = b'\202\323\344\223\002 \"\033/rest/sampler/sample-tokens:\001*'
-  _SAMPLER.methods_by_name['Tokenize']._options = None
-  _SAMPLER.methods_by_name['Tokenize']._serialized_options = b'\202\323\344\223\002\033\"\026/rest/sampler/tokenize:\001*'
-  _SAMPLER.methods_by_name['ListTransactions']._options = None
-  _SAMPLER.methods_by_name['ListTransactions']._serialized_options = b'\202\323\344\223\002\034\022\032/rest/sampler/transactions'
-  _SAMPLER.methods_by_name['GetTokenBudget']._options = None
-  _SAMPLER.methods_by_name['GetTokenBudget']._serialized_options = b'\202\323\344\223\002\034\022\032/rest/sampler/token-budget'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z\032x.ai/prompt_ide;prompt_ide'
+  _globals['_SAMPLETOKENSREQUEST'].fields_by_name['prompt']._options = None
+  _globals['_SAMPLETOKENSREQUEST'].fields_by_name['prompt']._serialized_options = b'\030\001'
+  _globals['_SAMPLER'].methods_by_name['SampleTokens']._options = None
+  _globals['_SAMPLER'].methods_by_name['SampleTokens']._serialized_options = b'\202\323\344\223\002 \"\033/rest/sampler/sample-tokens:\001*'
+  _globals['_SAMPLER'].methods_by_name['Tokenize']._options = None
+  _globals['_SAMPLER'].methods_by_name['Tokenize']._serialized_options = b'\202\323\344\223\002\033\"\026/rest/sampler/tokenize:\001*'
+  _globals['_SAMPLER'].methods_by_name['TokenizeAndSampleTokens']._options = None
+  _globals['_SAMPLER'].methods_by_name['TokenizeAndSampleTokens']._serialized_options = b'\202\323\344\223\002-\"(/rest/sampler/tokenize-and-sample-tokens:\001*'
+  _globals['_SAMPLER'].methods_by_name['ListTransactions']._options = None
+  _globals['_SAMPLER'].methods_by_name['ListTransactions']._serialized_options = b'\202\323\344\223\002\034\022\032/rest/sampler/transactions'
+  _globals['_SAMPLER'].methods_by_name['GetTokenBudget']._options = None
+  _globals['_SAMPLER'].methods_by_name['GetTokenBudget']._serialized_options = b'\202\323\344\223\002\034\022\032/rest/sampler/token-budget'
   _globals['_SAMPLETOKENSREQUEST']._serialized_start=129
-  _globals['_SAMPLETOKENSREQUEST']._serialized_end=270
-  _globals['_SAMPLETOKENSRESPONSE']._serialized_start=272
-  _globals['_SAMPLETOKENSRESPONSE']._serialized_end=391
-  _globals['_SAMPLESETTINGS']._serialized_start=394
-  _globals['_SAMPLESETTINGS']._serialized_end=627
-  _globals['_INPUTTOKEN']._serialized_start=629
-  _globals['_INPUTTOKEN']._serialized_end=694
-  _globals['_TOKEN']._serialized_start=697
-  _globals['_TOKEN']._serialized_end=899
-  _globals['_TOKEN_TOKENTYPE']._serialized_start=848
-  _globals['_TOKEN_TOKENTYPE']._serialized_end=893
-  _globals['_LOGIT']._serialized_start=901
-  _globals['_LOGIT']._serialized_end=962
-  _globals['_TOKENIZEREQUEST']._serialized_start=964
-  _globals['_TOKENIZEREQUEST']._serialized_end=1015
-  _globals['_TOKENIZERESPONSE']._serialized_start=1017
-  _globals['_TOKENIZERESPONSE']._serialized_end=1070
-  _globals['_LISTTRANSACTIONSRESPONSE']._serialized_start=1072
-  _globals['_LISTTRANSACTIONSRESPONSE']._serialized_end=1150
-  _globals['_TOKENTRANSACTION']._serialized_start=1153
-  _globals['_TOKENTRANSACTION']._serialized_end=1302
-  _globals['_TOKENBUDGET']._serialized_start=1304
-  _globals['_TOKENBUDGET']._serialized_end=1360
-  _globals['_SAMPLER']._serialized_start=1363
-  _globals['_SAMPLER']._serialized_end=1824
+  _globals['_SAMPLETOKENSREQUEST']._serialized_end=315
+  _globals['_PROMPTINPUT']._serialized_start=318
+  _globals['_PROMPTINPUT']._serialized_end=448
+  _globals['_TOKENIDS']._serialized_start=450
+  _globals['_TOKENIDS']._serialized_end=476
+  _globals['_SAMPLETOKENSRESPONSE']._serialized_start=479
+  _globals['_SAMPLETOKENSRESPONSE']._serialized_end=651
+  _globals['_TOKENIZEANDSAMPLETOKENSREQUEST']._serialized_start=654
+  _globals['_TOKENIZEANDSAMPLETOKENSREQUEST']._serialized_end=792
+  _globals['_SAMPLESETTINGS']._serialized_start=795
+  _globals['_SAMPLESETTINGS']._serialized_end=1028
+  _globals['_INPUTTOKEN']._serialized_start=1030
+  _globals['_INPUTTOKEN']._serialized_end=1095
+  _globals['_TOKEN']._serialized_start=1098
+  _globals['_TOKEN']._serialized_end=1300
+  _globals['_TOKEN_TOKENTYPE']._serialized_start=1249
+  _globals['_TOKEN_TOKENTYPE']._serialized_end=1294
+  _globals['_LOGIT']._serialized_start=1302
+  _globals['_LOGIT']._serialized_end=1363
+  _globals['_TOKENIZEREQUEST']._serialized_start=1365
+  _globals['_TOKENIZEREQUEST']._serialized_end=1416
+  _globals['_TOKENIZERESPONSE']._serialized_start=1418
+  _globals['_TOKENIZERESPONSE']._serialized_end=1471
+  _globals['_LISTTRANSACTIONSRESPONSE']._serialized_start=1473
+  _globals['_LISTTRANSACTIONSRESPONSE']._serialized_end=1551
+  _globals['_TOKENTRANSACTION']._serialized_start=1554
+  _globals['_TOKENTRANSACTION']._serialized_end=1792
+  _globals['_GETTOKENBUDGETREQUEST']._serialized_start=1794
+  _globals['_GETTOKENBUDGETREQUEST']._serialized_end=1843
+  _globals['_TOKENBUDGET']._serialized_start=1845
+  _globals['_TOKENBUDGET']._serialized_end=1948
+  _globals['_SAMPLER']._serialized_start=1951
+  _globals['_SAMPLER']._serialized_end=2584
 # @@protoc_insertion_point(module_scope)
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/proto/sampler_public_pb2.pyi` & `xai_sdk-0.0.5/src/xai_sdk/proto/sampler_public_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,74 @@
-from typing import ClassVar as _ClassVar
-from typing import Iterable as _Iterable
-from typing import Mapping as _Mapping
-from typing import Optional as _Optional
-from typing import Union as _Union
-
-from google.protobuf import descriptor as _descriptor
+from .google.api import annotations_pb2 as _annotations_pb2
 from google.protobuf import empty_pb2 as _empty_pb2
-from google.protobuf import message as _message
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
-
-from .google.api import annotations_pb2 as _annotations_pb2
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class SampleTokensRequest(_message.Message):
-    __slots__ = ["prompt", "settings", "return_attention", "model_name"]
+    __slots__ = ("prompt", "inputs", "settings", "return_attention", "model_name")
     PROMPT_FIELD_NUMBER: _ClassVar[int]
+    INPUTS_FIELD_NUMBER: _ClassVar[int]
     SETTINGS_FIELD_NUMBER: _ClassVar[int]
     RETURN_ATTENTION_FIELD_NUMBER: _ClassVar[int]
     MODEL_NAME_FIELD_NUMBER: _ClassVar[int]
     prompt: _containers.RepeatedScalarFieldContainer[int]
+    inputs: _containers.RepeatedCompositeFieldContainer[PromptInput]
     settings: SampleSettings
     return_attention: bool
     model_name: str
-    def __init__(
-        self,
-        prompt: _Optional[_Iterable[int]] = ...,
-        settings: _Optional[_Union[SampleSettings, _Mapping]] = ...,
-        return_attention: bool = ...,
-        model_name: _Optional[str] = ...,
-    ) -> None: ...
+    def __init__(self, prompt: _Optional[_Iterable[int]] = ..., inputs: _Optional[_Iterable[_Union[PromptInput, _Mapping]]] = ..., settings: _Optional[_Union[SampleSettings, _Mapping]] = ..., return_attention: bool = ..., model_name: _Optional[str] = ...) -> None: ...
+
+class PromptInput(_message.Message):
+    __slots__ = ("text", "image_bytes", "image_base64", "token_ids")
+    TEXT_FIELD_NUMBER: _ClassVar[int]
+    IMAGE_BYTES_FIELD_NUMBER: _ClassVar[int]
+    IMAGE_BASE64_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_IDS_FIELD_NUMBER: _ClassVar[int]
+    text: str
+    image_bytes: bytes
+    image_base64: str
+    token_ids: TokenIds
+    def __init__(self, text: _Optional[str] = ..., image_bytes: _Optional[bytes] = ..., image_base64: _Optional[str] = ..., token_ids: _Optional[_Union[TokenIds, _Mapping]] = ...) -> None: ...
+
+class TokenIds(_message.Message):
+    __slots__ = ("tokens",)
+    TOKENS_FIELD_NUMBER: _ClassVar[int]
+    tokens: _containers.RepeatedScalarFieldContainer[int]
+    def __init__(self, tokens: _Optional[_Iterable[int]] = ...) -> None: ...
 
 class SampleTokensResponse(_message.Message):
-    __slots__ = ["token", "budget"]
+    __slots__ = ("token", "budget", "transaction")
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     BUDGET_FIELD_NUMBER: _ClassVar[int]
+    TRANSACTION_FIELD_NUMBER: _ClassVar[int]
     token: Token
     budget: TokenBudget
-    def __init__(
-        self,
-        token: _Optional[_Union[Token, _Mapping]] = ...,
-        budget: _Optional[_Union[TokenBudget, _Mapping]] = ...,
-    ) -> None: ...
+    transaction: TokenTransaction
+    def __init__(self, token: _Optional[_Union[Token, _Mapping]] = ..., budget: _Optional[_Union[TokenBudget, _Mapping]] = ..., transaction: _Optional[_Union[TokenTransaction, _Mapping]] = ...) -> None: ...
+
+class TokenizeAndSampleTokensRequest(_message.Message):
+    __slots__ = ("text", "settings", "return_attention", "model_name")
+    TEXT_FIELD_NUMBER: _ClassVar[int]
+    SETTINGS_FIELD_NUMBER: _ClassVar[int]
+    RETURN_ATTENTION_FIELD_NUMBER: _ClassVar[int]
+    MODEL_NAME_FIELD_NUMBER: _ClassVar[int]
+    text: str
+    settings: SampleSettings
+    return_attention: bool
+    model_name: str
+    def __init__(self, text: _Optional[str] = ..., settings: _Optional[_Union[SampleSettings, _Mapping]] = ..., return_attention: bool = ..., model_name: _Optional[str] = ...) -> None: ...
 
 class SampleSettings(_message.Message):
-    __slots__ = [
-        "max_len",
-        "temperature",
-        "nucleus_p",
-        "stop_tokens",
-        "stop_strings",
-        "rng_seed",
-        "allowed_tokens",
-        "disallowed_tokens",
-    ]
+    __slots__ = ("max_len", "temperature", "nucleus_p", "stop_tokens", "stop_strings", "rng_seed", "allowed_tokens", "disallowed_tokens")
     MAX_LEN_FIELD_NUMBER: _ClassVar[int]
     TEMPERATURE_FIELD_NUMBER: _ClassVar[int]
     NUCLEUS_P_FIELD_NUMBER: _ClassVar[int]
     STOP_TOKENS_FIELD_NUMBER: _ClassVar[int]
     STOP_STRINGS_FIELD_NUMBER: _ClassVar[int]
     RNG_SEED_FIELD_NUMBER: _ClassVar[int]
     ALLOWED_TOKENS_FIELD_NUMBER: _ClassVar[int]
@@ -68,120 +77,104 @@
     temperature: float
     nucleus_p: float
     stop_tokens: _containers.RepeatedScalarFieldContainer[str]
     stop_strings: _containers.RepeatedScalarFieldContainer[str]
     rng_seed: int
     allowed_tokens: _containers.RepeatedCompositeFieldContainer[InputToken]
     disallowed_tokens: _containers.RepeatedCompositeFieldContainer[InputToken]
-    def __init__(
-        self,
-        max_len: _Optional[int] = ...,
-        temperature: _Optional[float] = ...,
-        nucleus_p: _Optional[float] = ...,
-        stop_tokens: _Optional[_Iterable[str]] = ...,
-        stop_strings: _Optional[_Iterable[str]] = ...,
-        rng_seed: _Optional[int] = ...,
-        allowed_tokens: _Optional[_Iterable[_Union[InputToken, _Mapping]]] = ...,
-        disallowed_tokens: _Optional[_Iterable[_Union[InputToken, _Mapping]]] = ...,
-    ) -> None: ...
+    def __init__(self, max_len: _Optional[int] = ..., temperature: _Optional[float] = ..., nucleus_p: _Optional[float] = ..., stop_tokens: _Optional[_Iterable[str]] = ..., stop_strings: _Optional[_Iterable[str]] = ..., rng_seed: _Optional[int] = ..., allowed_tokens: _Optional[_Iterable[_Union[InputToken, _Mapping]]] = ..., disallowed_tokens: _Optional[_Iterable[_Union[InputToken, _Mapping]]] = ...) -> None: ...
 
 class InputToken(_message.Message):
-    __slots__ = ["string_token", "token_id"]
+    __slots__ = ("string_token", "token_id")
     STRING_TOKEN_FIELD_NUMBER: _ClassVar[int]
     TOKEN_ID_FIELD_NUMBER: _ClassVar[int]
     string_token: str
     token_id: int
-    def __init__(
-        self, string_token: _Optional[str] = ..., token_id: _Optional[int] = ...
-    ) -> None: ...
+    def __init__(self, string_token: _Optional[str] = ..., token_id: _Optional[int] = ...) -> None: ...
 
 class Token(_message.Message):
-    __slots__ = ["final_logit", "top_k", "attention", "token_type"]
-
+    __slots__ = ("final_logit", "top_k", "attention", "token_type")
     class TokenType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
+        __slots__ = ()
         UNKNOWN: _ClassVar[Token.TokenType]
         USER: _ClassVar[Token.TokenType]
         MODEL: _ClassVar[Token.TokenType]
     UNKNOWN: Token.TokenType
     USER: Token.TokenType
     MODEL: Token.TokenType
     FINAL_LOGIT_FIELD_NUMBER: _ClassVar[int]
     TOP_K_FIELD_NUMBER: _ClassVar[int]
     ATTENTION_FIELD_NUMBER: _ClassVar[int]
     TOKEN_TYPE_FIELD_NUMBER: _ClassVar[int]
     final_logit: Logit
     top_k: _containers.RepeatedCompositeFieldContainer[Logit]
     attention: _containers.RepeatedScalarFieldContainer[float]
     token_type: Token.TokenType
-    def __init__(
-        self,
-        final_logit: _Optional[_Union[Logit, _Mapping]] = ...,
-        top_k: _Optional[_Iterable[_Union[Logit, _Mapping]]] = ...,
-        attention: _Optional[_Iterable[float]] = ...,
-        token_type: _Optional[_Union[Token.TokenType, str]] = ...,
-    ) -> None: ...
+    def __init__(self, final_logit: _Optional[_Union[Logit, _Mapping]] = ..., top_k: _Optional[_Iterable[_Union[Logit, _Mapping]]] = ..., attention: _Optional[_Iterable[float]] = ..., token_type: _Optional[_Union[Token.TokenType, str]] = ...) -> None: ...
 
 class Logit(_message.Message):
-    __slots__ = ["token_id", "string_token", "prob"]
+    __slots__ = ("token_id", "string_token", "prob")
     TOKEN_ID_FIELD_NUMBER: _ClassVar[int]
     STRING_TOKEN_FIELD_NUMBER: _ClassVar[int]
     PROB_FIELD_NUMBER: _ClassVar[int]
     token_id: int
     string_token: str
     prob: float
-    def __init__(
-        self,
-        token_id: _Optional[int] = ...,
-        string_token: _Optional[str] = ...,
-        prob: _Optional[float] = ...,
-    ) -> None: ...
+    def __init__(self, token_id: _Optional[int] = ..., string_token: _Optional[str] = ..., prob: _Optional[float] = ...) -> None: ...
 
 class TokenizeRequest(_message.Message):
-    __slots__ = ["text", "model_name"]
+    __slots__ = ("text", "model_name")
     TEXT_FIELD_NUMBER: _ClassVar[int]
     MODEL_NAME_FIELD_NUMBER: _ClassVar[int]
     text: str
     model_name: str
     def __init__(self, text: _Optional[str] = ..., model_name: _Optional[str] = ...) -> None: ...
 
 class TokenizeResponse(_message.Message):
-    __slots__ = ["tokens"]
+    __slots__ = ("tokens",)
     TOKENS_FIELD_NUMBER: _ClassVar[int]
     tokens: _containers.RepeatedCompositeFieldContainer[Token]
     def __init__(self, tokens: _Optional[_Iterable[_Union[Token, _Mapping]]] = ...) -> None: ...
 
 class ListTransactionsResponse(_message.Message):
-    __slots__ = ["transactions"]
+    __slots__ = ("transactions",)
     TRANSACTIONS_FIELD_NUMBER: _ClassVar[int]
     transactions: _containers.RepeatedCompositeFieldContainer[TokenTransaction]
-    def __init__(
-        self, transactions: _Optional[_Iterable[_Union[TokenTransaction, _Mapping]]] = ...
-    ) -> None: ...
+    def __init__(self, transactions: _Optional[_Iterable[_Union[TokenTransaction, _Mapping]]] = ...) -> None: ...
 
 class TokenTransaction(_message.Message):
-    __slots__ = ["num_prompt_tokens", "num_generated_tokens", "cost_multiplier", "create_time"]
+    __slots__ = ("num_prompt_tokens", "num_generated_tokens", "cost_multiplier", "create_time", "transaction_type", "transaction_id", "model_name", "confirmed")
     NUM_PROMPT_TOKENS_FIELD_NUMBER: _ClassVar[int]
     NUM_GENERATED_TOKENS_FIELD_NUMBER: _ClassVar[int]
     COST_MULTIPLIER_FIELD_NUMBER: _ClassVar[int]
     CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
+    TRANSACTION_TYPE_FIELD_NUMBER: _ClassVar[int]
+    TRANSACTION_ID_FIELD_NUMBER: _ClassVar[int]
+    MODEL_NAME_FIELD_NUMBER: _ClassVar[int]
+    CONFIRMED_FIELD_NUMBER: _ClassVar[int]
     num_prompt_tokens: int
     num_generated_tokens: int
     cost_multiplier: int
     create_time: _timestamp_pb2.Timestamp
-    def __init__(
-        self,
-        num_prompt_tokens: _Optional[int] = ...,
-        num_generated_tokens: _Optional[int] = ...,
-        cost_multiplier: _Optional[int] = ...,
-        create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
-    ) -> None: ...
+    transaction_type: str
+    transaction_id: str
+    model_name: str
+    confirmed: bool
+    def __init__(self, num_prompt_tokens: _Optional[int] = ..., num_generated_tokens: _Optional[int] = ..., cost_multiplier: _Optional[int] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., transaction_type: _Optional[str] = ..., transaction_id: _Optional[str] = ..., model_name: _Optional[str] = ..., confirmed: bool = ...) -> None: ...
+
+class GetTokenBudgetRequest(_message.Message):
+    __slots__ = ("transaction_type",)
+    TRANSACTION_TYPE_FIELD_NUMBER: _ClassVar[int]
+    transaction_type: str
+    def __init__(self, transaction_type: _Optional[str] = ...) -> None: ...
 
 class TokenBudget(_message.Message):
-    __slots__ = ["token_limit", "tokens_spent"]
+    __slots__ = ("token_limit", "tokens_spent", "request_limit", "requests_spent")
     TOKEN_LIMIT_FIELD_NUMBER: _ClassVar[int]
     TOKENS_SPENT_FIELD_NUMBER: _ClassVar[int]
+    REQUEST_LIMIT_FIELD_NUMBER: _ClassVar[int]
+    REQUESTS_SPENT_FIELD_NUMBER: _ClassVar[int]
     token_limit: int
     tokens_spent: int
-    def __init__(
-        self, token_limit: _Optional[int] = ..., tokens_spent: _Optional[int] = ...
-    ) -> None: ...
+    request_limit: int
+    requests_spent: int
+    def __init__(self, token_limit: _Optional[int] = ..., tokens_spent: _Optional[int] = ..., request_limit: _Optional[int] = ..., requests_spent: _Optional[int] = ...) -> None: ...
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/proto/sampler_public_pb2_grpc.py` & `xai_sdk-0.0.5/src/xai_sdk/proto/sampler_public_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # fmt: off
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from . import sampler_public_pb2 as sampler__public__pb2
 
 
 class SamplerStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
@@ -22,22 +22,27 @@
                 response_deserializer=sampler__public__pb2.SampleTokensResponse.FromString,
                 )
         self.Tokenize = channel.unary_unary(
                 '/prompt_ide.Sampler/Tokenize',
                 request_serializer=sampler__public__pb2.TokenizeRequest.SerializeToString,
                 response_deserializer=sampler__public__pb2.TokenizeResponse.FromString,
                 )
+        self.TokenizeAndSampleTokens = channel.unary_stream(
+                '/prompt_ide.Sampler/TokenizeAndSampleTokens',
+                request_serializer=sampler__public__pb2.TokenizeAndSampleTokensRequest.SerializeToString,
+                response_deserializer=sampler__public__pb2.SampleTokensResponse.FromString,
+                )
         self.ListTransactions = channel.unary_unary(
                 '/prompt_ide.Sampler/ListTransactions',
                 request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                 response_deserializer=sampler__public__pb2.ListTransactionsResponse.FromString,
                 )
         self.GetTokenBudget = channel.unary_unary(
                 '/prompt_ide.Sampler/GetTokenBudget',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                request_serializer=sampler__public__pb2.GetTokenBudgetRequest.SerializeToString,
                 response_deserializer=sampler__public__pb2.TokenBudget.FromString,
                 )
 
 
 class SamplerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -52,14 +57,22 @@
     def Tokenize(self, request, context):
         """Tokenizes the incoming text. Result is delivered in a Logit proto with zero log probs.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def TokenizeAndSampleTokens(self, request, context):
+        """Tokenizes the text and then samples from the model. This can reduce network latencies when all
+        we need to do is tokenize and the immediately sample.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ListTransactions(self, request, context):
         """Returns all token transactions in the current accounting period.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -79,22 +92,27 @@
                     response_serializer=sampler__public__pb2.SampleTokensResponse.SerializeToString,
             ),
             'Tokenize': grpc.unary_unary_rpc_method_handler(
                     servicer.Tokenize,
                     request_deserializer=sampler__public__pb2.TokenizeRequest.FromString,
                     response_serializer=sampler__public__pb2.TokenizeResponse.SerializeToString,
             ),
+            'TokenizeAndSampleTokens': grpc.unary_stream_rpc_method_handler(
+                    servicer.TokenizeAndSampleTokens,
+                    request_deserializer=sampler__public__pb2.TokenizeAndSampleTokensRequest.FromString,
+                    response_serializer=sampler__public__pb2.SampleTokensResponse.SerializeToString,
+            ),
             'ListTransactions': grpc.unary_unary_rpc_method_handler(
                     servicer.ListTransactions,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=sampler__public__pb2.ListTransactionsResponse.SerializeToString,
             ),
             'GetTokenBudget': grpc.unary_unary_rpc_method_handler(
                     servicer.GetTokenBudget,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    request_deserializer=sampler__public__pb2.GetTokenBudgetRequest.FromString,
                     response_serializer=sampler__public__pb2.TokenBudget.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'prompt_ide.Sampler', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
@@ -134,14 +152,31 @@
         return grpc.experimental.unary_unary(request, target, '/prompt_ide.Sampler/Tokenize',
             sampler__public__pb2.TokenizeRequest.SerializeToString,
             sampler__public__pb2.TokenizeResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def TokenizeAndSampleTokens(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/prompt_ide.Sampler/TokenizeAndSampleTokens',
+            sampler__public__pb2.TokenizeAndSampleTokensRequest.SerializeToString,
+            sampler__public__pb2.SampleTokensResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ListTransactions(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -162,11 +197,11 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/prompt_ide.Sampler/GetTokenBudget',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            sampler__public__pb2.GetTokenBudgetRequest.SerializeToString,
             sampler__public__pb2.TokenBudget.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/proto/stateless_chat_pb2.pyi` & `xai_sdk-0.0.5/src/xai_sdk/proto/google/api/http_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,42 @@
-from typing import ClassVar as _ClassVar
-from typing import Iterable as _Iterable
-from typing import Mapping as _Mapping
-from typing import Optional as _Optional
-from typing import Union as _Union
-
+from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
-from google.protobuf import empty_pb2 as _empty_pb2
 from google.protobuf import message as _message
-from google.protobuf.internal import containers as _containers
-from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
-
-from .google.api import annotations_pb2 as _annotations_pb2
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class StatelessConversation(_message.Message):
-    __slots__ = [
-        "stateless_conversation_id",
-        "responses",
-        "system_prompt_name",
-        "name",
-        "username",
-        "expose_username_to_grok",
-    ]
-    STATELESS_CONVERSATION_ID_FIELD_NUMBER: _ClassVar[int]
-    RESPONSES_FIELD_NUMBER: _ClassVar[int]
-    SYSTEM_PROMPT_NAME_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    USERNAME_FIELD_NUMBER: _ClassVar[int]
-    EXPOSE_USERNAME_TO_GROK_FIELD_NUMBER: _ClassVar[int]
-    stateless_conversation_id: str
-    responses: _containers.RepeatedCompositeFieldContainer[StatelessResponse]
-    system_prompt_name: str
-    name: str
-    username: str
-    expose_username_to_grok: bool
-    def __init__(
-        self,
-        stateless_conversation_id: _Optional[str] = ...,
-        responses: _Optional[_Iterable[_Union[StatelessResponse, _Mapping]]] = ...,
-        system_prompt_name: _Optional[str] = ...,
-        name: _Optional[str] = ...,
-        username: _Optional[str] = ...,
-        expose_username_to_grok: bool = ...,
-    ) -> None: ...
-
-class StatelessResponse(_message.Message):
-    __slots__ = ["sender", "message", "query"]
-
-    class Sender(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-        UNKNOWN: _ClassVar[StatelessResponse.Sender]
-        HUMAN: _ClassVar[StatelessResponse.Sender]
-        ASSISTANT: _ClassVar[StatelessResponse.Sender]
-    UNKNOWN: StatelessResponse.Sender
-    HUMAN: StatelessResponse.Sender
-    ASSISTANT: StatelessResponse.Sender
-    SENDER_FIELD_NUMBER: _ClassVar[int]
-    MESSAGE_FIELD_NUMBER: _ClassVar[int]
-    QUERY_FIELD_NUMBER: _ClassVar[int]
-    sender: StatelessResponse.Sender
-    message: str
-    query: str
-    def __init__(
-        self,
-        sender: _Optional[_Union[StatelessResponse.Sender, str]] = ...,
-        message: _Optional[str] = ...,
-        query: _Optional[str] = ...,
-    ) -> None: ...
-
-class DeleteLoggedConversationsRequest(_message.Message):
-    __slots__ = ["accounting_key"]
-    ACCOUNTING_KEY_FIELD_NUMBER: _ClassVar[int]
-    accounting_key: str
-    def __init__(self, accounting_key: _Optional[str] = ...) -> None: ...
+class Http(_message.Message):
+    __slots__ = ("rules",)
+    RULES_FIELD_NUMBER: _ClassVar[int]
+    rules: _containers.RepeatedCompositeFieldContainer[HttpRule]
+    def __init__(self, rules: _Optional[_Iterable[_Union[HttpRule, _Mapping]]] = ...) -> None: ...
+
+class HttpRule(_message.Message):
+    __slots__ = ("selector", "get", "put", "post", "delete", "patch", "custom", "body", "additional_bindings")
+    SELECTOR_FIELD_NUMBER: _ClassVar[int]
+    GET_FIELD_NUMBER: _ClassVar[int]
+    PUT_FIELD_NUMBER: _ClassVar[int]
+    POST_FIELD_NUMBER: _ClassVar[int]
+    DELETE_FIELD_NUMBER: _ClassVar[int]
+    PATCH_FIELD_NUMBER: _ClassVar[int]
+    CUSTOM_FIELD_NUMBER: _ClassVar[int]
+    BODY_FIELD_NUMBER: _ClassVar[int]
+    ADDITIONAL_BINDINGS_FIELD_NUMBER: _ClassVar[int]
+    selector: str
+    get: str
+    put: str
+    post: str
+    delete: str
+    patch: str
+    custom: CustomHttpPattern
+    body: str
+    additional_bindings: _containers.RepeatedCompositeFieldContainer[HttpRule]
+    def __init__(self, selector: _Optional[str] = ..., get: _Optional[str] = ..., put: _Optional[str] = ..., post: _Optional[str] = ..., delete: _Optional[str] = ..., patch: _Optional[str] = ..., custom: _Optional[_Union[CustomHttpPattern, _Mapping]] = ..., body: _Optional[str] = ..., additional_bindings: _Optional[_Iterable[_Union[HttpRule, _Mapping]]] = ...) -> None: ...
+
+class CustomHttpPattern(_message.Message):
+    __slots__ = ("kind", "path")
+    KIND_FIELD_NUMBER: _ClassVar[int]
+    PATH_FIELD_NUMBER: _ClassVar[int]
+    kind: str
+    path: str
+    def __init__(self, kind: _Optional[str] = ..., path: _Optional[str] = ...) -> None: ...
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/proto/stateless_chat_pb2_grpc.py` & `xai_sdk-0.0.5/src/xai_sdk/proto/stateless_chat_pb2_grpc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # fmt: off
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from . import stateless_chat_pb2 as stateless__chat__pb2
 
 
 class StatelessChatStub(object):
     """This is a simplified interface for interacting with Grok. It's entirely stateless but exposes
     less information than the full implementation in chat.proto. It's main purpose is to power the
     Grok-on-X experience.
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/proto/google/api/annotations_pb2.py` & `xai_sdk-0.0.5/src/xai_sdk/proto/google/api/annotations_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/annotations.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from . import http_pb2 as google_dot_api_dot_http__pb2
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
-from . import http_pb2 as google_dot_api_dot_http__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cgoogle/api/annotations.proto\x12\ngoogle.api\x1a\x15google/api/http.proto\x1a google/protobuf/descriptor.proto:E\n\x04http\x12\x1e.google.protobuf.MethodOptions\x18\xb0\xca\xbc\" \x01(\x0b\x32\x14.google.api.HttpRuleBn\n\x0e\x63om.google.apiB\x10\x41nnotationsProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xa2\x02\x04GAPIb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.annotations_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(http)
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\020AnnotationsProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\242\002\004GAPI'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\016com.google.apiB\020AnnotationsProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\242\002\004GAPI'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `xai_sdk-0.0.4/src/xai_sdk/proto/google/api/http_pb2.py` & `xai_sdk-0.0.5/src/xai_sdk/proto/google/api/http_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/http.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15google/api/http.proto\x12\ngoogle.api\"+\n\x04Http\x12#\n\x05rules\x18\x01 \x03(\x0b\x32\x14.google.api.HttpRule\"\xea\x01\n\x08HttpRule\x12\x10\n\x08selector\x18\x01 \x01(\t\x12\r\n\x03get\x18\x02 \x01(\tH\x00\x12\r\n\x03put\x18\x03 \x01(\tH\x00\x12\x0e\n\x04post\x18\x04 \x01(\tH\x00\x12\x10\n\x06\x64\x65lete\x18\x05 \x01(\tH\x00\x12\x0f\n\x05patch\x18\x06 \x01(\tH\x00\x12/\n\x06\x63ustom\x18\x08 \x01(\x0b\x32\x1d.google.api.CustomHttpPatternH\x00\x12\x0c\n\x04\x62ody\x18\x07 \x01(\t\x12\x31\n\x13\x61\x64\x64itional_bindings\x18\x0b \x03(\x0b\x32\x14.google.api.HttpRuleB\t\n\x07pattern\"/\n\x11\x43ustomHttpPattern\x12\x0c\n\x04kind\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\tBj\n\x0e\x63om.google.apiB\tHttpProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xf8\x01\x01\xa2\x02\x04GAPIb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.http_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\tHttpProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\370\001\001\242\002\004GAPI'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\016com.google.apiB\tHttpProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\370\001\001\242\002\004GAPI'
   _globals['_HTTP']._serialized_start=37
   _globals['_HTTP']._serialized_end=80
   _globals['_HTTPRULE']._serialized_start=83
   _globals['_HTTPRULE']._serialized_end=317
   _globals['_CUSTOMHTTPPATTERN']._serialized_start=319
   _globals['_CUSTOMHTTPPATTERN']._serialized_end=366
 # @@protoc_insertion_point(module_scope)
```

### Comparing `xai_sdk-0.0.4/LICENSE.txt` & `xai_sdk-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.4/pyproject.toml` & `xai_sdk-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -80,16 +80,19 @@
 
 [tool.black]
 target-version = ["py37"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
+exclude = ["src/xai_sdk"]
 target-version = "py37"
 line-length = 120
+
+[tool.ruff.lint]
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
@@ -124,21 +127,21 @@
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["xai_sdk"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
 source_pkgs = ["xai_sdk", "tests"]
 branch = true
 parallel = true
```

### Comparing `xai_sdk-0.0.4/PKG-INFO` & `xai_sdk-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: xai-sdk
-Version: 0.0.4
+Version: 0.0.5
 Project-URL: Documentation, https://x.ai/api/sdk.html
 Author-email: Toby Pohlen <pohlen@x.ai>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

