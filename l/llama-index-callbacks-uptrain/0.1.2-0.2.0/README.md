# Comparing `tmp/llama_index_callbacks_uptrain-0.1.2.tar.gz` & `tmp/llama_index_callbacks_uptrain-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_callbacks_uptrain-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_callbacks_uptrain-0.2.0.tar", max compression
```

## Comparing `llama_index_callbacks_uptrain-0.1.2.tar` & `llama_index_callbacks_uptrain-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3067 2024-03-04 17:06:26.867268 llama_index_callbacks_uptrain-0.1.2/README.md
--rw-r--r--   0        0        0      108 2024-03-04 17:06:26.867268 llama_index_callbacks_uptrain-0.1.2/llama_index/callbacks/uptrain/__init__.py
--rw-r--r--   0        0        0    12525 2024-03-04 17:06:26.867268 llama_index_callbacks_uptrain-0.1.2/llama_index/callbacks/uptrain/base.py
--rw-r--r--   0        0        0     1479 2024-03-04 17:06:26.867268 llama_index_callbacks_uptrain-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 llama_index_callbacks_uptrain-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3067 2024-05-14 17:07:21.223821 llama_index_callbacks_uptrain-0.2.0/README.md
+-rw-r--r--   0        0        0      108 2024-05-14 17:07:21.223821 llama_index_callbacks_uptrain-0.2.0/llama_index/callbacks/uptrain/__init__.py
+-rw-r--r--   0        0        0    13144 2024-05-14 17:07:21.223821 llama_index_callbacks_uptrain-0.2.0/llama_index/callbacks/uptrain/base.py
+-rw-r--r--   0        0        0     1508 2024-05-14 17:07:21.223821 llama_index_callbacks_uptrain-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3684 1970-01-01 00:00:00.000000 llama_index_callbacks_uptrain-0.2.0/PKG-INFO
```

### Comparing `llama_index_callbacks_uptrain-0.1.2/README.md` & `llama_index_callbacks_uptrain-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_callbacks_uptrain-0.1.2/llama_index/callbacks/uptrain/base.py` & `llama_index_callbacks_uptrain-0.2.0/llama_index/callbacks/uptrain/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,31 +9,32 @@
     CBEventType,
 )
 
 
 class UpTrainDataSchema:
     """UpTrain data schema."""
 
-    def __init__(self, project_name_prefix: str) -> None:
+    def __init__(self, project_name: str) -> None:
         """Initialize the UpTrain data schema."""
         # For tracking project name and results
-        self.project_name_prefix: str = project_name_prefix
+        self.project_name: str = project_name
         self.uptrain_results: DefaultDict[str, Any] = defaultdict(list)
 
         # For tracking event types - reranking, sub_question
         self.eval_types: Set[str] = set()
 
         ## SYNTHESIZE
         self.question: str = ""
         self.context: str = ""
         self.response: str = ""
 
         ## RERANKING
         self.old_context: List[str] = []
         self.new_context: List[str] = []
+        self.reranking_type: Literal["resize", "rerank"] = "rerank"
 
         ## SUB_QUESTION
         # Map of sub question ID to question, context, and response
         self.sub_question_map: DefaultDict[str, dict] = defaultdict(dict)
         # Parent ID of sub questions
         self.sub_question_parent_id: str = ""
         # Parent question
@@ -48,30 +49,30 @@
 
     """
 
     def __init__(
         self,
         api_key: str,
         key_type: Literal["uptrain", "openai"],
-        project_name_prefix: str = "llama",
+        project_name: str = "uptrain_llamaindex",
     ) -> None:
         """Initialize the UpTrain callback handler."""
         try:
             from uptrain import APIClient, EvalLLM, Settings
         except ImportError:
             raise ImportError(
                 "UpTrainCallbackHandler requires the 'uptrain' package. "
                 "Please install it using 'pip install uptrain'."
             )
         nest_asyncio.apply()
         super().__init__(
             event_starts_to_ignore=[],
             event_ends_to_ignore=[],
         )
-        self.schema = UpTrainDataSchema(project_name_prefix=project_name_prefix)
+        self.schema = UpTrainDataSchema(project_name=project_name)
         self._event_pairs_by_id: Dict[str, List[CBEvent]] = defaultdict(list)
         self._trace_map: Dict[str, List[str]] = defaultdict(list)
 
         # Based on whether the user enters an UpTrain API key or an OpenAI API key, the client is initialized
         # If both are entered, the UpTrain API key is used
         if key_type == "uptrain":
             settings = Settings(uptrain_access_token=api_key)
@@ -80,31 +81,34 @@
             settings = Settings(openai_api_key=api_key)
             self.uptrain_client = EvalLLM(settings=settings)
         else:
             raise ValueError("Invalid key type: Must be 'uptrain' or 'openai'")
 
     def uptrain_evaluate(
         self,
-        project_name: str,
+        evaluation_name: str,
         data: List[Dict[str, str]],
         checks: List[str],
     ) -> None:
         """Run an evaluation on the UpTrain server using UpTrain client."""
         if self.uptrain_client.__class__.__name__ == "APIClient":
             uptrain_result = self.uptrain_client.log_and_evaluate(
-                project_name=project_name,
+                project_name=self.schema.project_name,
+                evaluation_name=evaluation_name,
                 data=data,
                 checks=checks,
             )
         else:
             uptrain_result = self.uptrain_client.evaluate(
+                project_name=self.schema.project_name,
+                evaluation_name=evaluation_name,
                 data=data,
                 checks=checks,
             )
-        self.schema.uptrain_results[project_name].append(uptrain_result)
+        self.schema.uptrain_results[self.schema.project_name].append(uptrain_result)
 
         score_name_map = {
             "score_context_relevance": "Context Relevance Score",
             "score_factual_accuracy": "Factual Accuracy Score",
             "score_response_completeness": "Response Completeness Score",
             "score_sub_query_completeness": "Sub Query Completeness Score",
             "score_context_reranking": "Context Reranking Score",
@@ -173,15 +177,15 @@
             )
         event = CBEvent(event_type, payload=payload, id_=event_id)
         self._event_pairs_by_id[event.id_].append(event)
         self._trace_map = defaultdict(list)
         if event_id == self.schema.sub_question_parent_id:
             # Perform individual evaluations for sub questions (but send all sub questions at once)
             self.uptrain_evaluate(
-                project_name=f"{self.schema.project_name_prefix}_sub_question_answering",
+                evaluation_name="sub_question_answering",
                 data=list(self.schema.sub_question_map.values()),
                 checks=[
                     Evals.CONTEXT_RELEVANCE,
                     Evals.FACTUAL_ACCURACY,
                     Evals.RESPONSE_COMPLETENESS,
                 ],
             )
@@ -193,32 +197,41 @@
             sub_questions_formatted = "\n".join(
                 [
                     f"{index}. {string}"
                     for index, string in enumerate(sub_questions, start=1)
                 ]
             )
             self.uptrain_evaluate(
-                project_name=f"{self.schema.project_name_prefix}_sub_query_completeness",
+                evaluation_name="sub_query_completeness",
                 data=[
                     {
                         "question": self.schema.parent_question,
                         "sub_questions": sub_questions_formatted,
                     }
                 ],
                 checks=[Evals.SUB_QUERY_COMPLETENESS],
             )
+            self.schema.eval_types.remove("sub_question")
         # Should not be called for sub questions
         if (
             event_type is CBEventType.SYNTHESIZE
             and "sub_question" not in self.schema.eval_types
         ):
             self.schema.response = payload["response"].response
             # Perform evaluation for synthesization
+            if "reranking" in self.schema.eval_types:
+                if self.schema.reranking_type == "rerank":
+                    evaluation_name = "question_answering_rerank"
+                else:
+                    evaluation_name = "question_answering_resize"
+                self.schema.eval_types.remove("reranking")
+            else:
+                evaluation_name = "question_answering"
             self.uptrain_evaluate(
-                project_name=f"{self.schema.project_name_prefix}_question_answering",
+                evaluation_name=evaluation_name,
                 data=[
                     {
                         "question": self.schema.question,
                         "context": self.schema.context,
                         "response": self.schema.response,
                     }
                 ],
@@ -229,46 +242,48 @@
                 ],
             )
 
         elif event_type is CBEventType.RERANKING:
             # Store new context data
             self.schema.new_context = [node.text for node in payload["nodes"]]
             if len(self.schema.old_context) == len(self.schema.new_context):
+                self.schema.reranking_type = "rerank"
                 context = "\n".join(
                     [
                         f"{index}. {string}"
                         for index, string in enumerate(self.schema.old_context, start=1)
                     ]
                 )
                 reranked_context = "\n".join(
                     [
                         f"{index}. {string}"
                         for index, string in enumerate(self.schema.new_context, start=1)
                     ]
                 )
                 # Perform evaluation for reranking
                 self.uptrain_evaluate(
-                    project_name=f"{self.schema.project_name_prefix}_context_reranking",
+                    evaluation_name="context_reranking",
                     data=[
                         {
                             "question": self.schema.question,
                             "context": context,
                             "reranked_context": reranked_context,
                         }
                     ],
                     checks=[
                         Evals.CONTEXT_RERANKING,
                     ],
                 )
             else:
+                self.schema.reranking_type = "resize"
                 context = "\n".join(self.schema.old_context)
                 concise_context = "\n".join(self.schema.new_context)
                 # Perform evaluation for resizing
                 self.uptrain_evaluate(
-                    project_name=f"{self.schema.project_name_prefix}_context_conciseness",
+                    evaluation_name="context_conciseness",
                     data=[
                         {
                             "question": self.schema.question,
                             "context": context,
                             "concise_context": concise_context,
                         }
                     ],
```

### Comparing `llama_index_callbacks_uptrain-0.1.2/pyproject.toml` & `llama_index_callbacks_uptrain-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
 authors = ["Dhruv Chawla <dhruv@uptrain.ai>"]
-description = "llama-index callbacks uptrain integration"
+description = "UpTrain Callback for performing evaluations on the LlamaIndex pipeline"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-callbacks-uptrain"
 readme = "README.md"
-version = "0.1.2"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = ">=0.10.0"
-uptrain = ">=0.6.6"
+uptrain = ">=0.7.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_callbacks_uptrain-0.1.2/PKG-INFO` & `llama_index_callbacks_uptrain-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: llama-index-callbacks-uptrain
-Version: 0.1.2
-Summary: llama-index callbacks uptrain integration
+Version: 0.2.0
+Summary: UpTrain Callback for performing evaluations on the LlamaIndex pipeline
 License: MIT
 Author: Dhruv Chawla
 Author-email: dhruv@uptrain.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: llama-index-core (>=0.10.0)
-Requires-Dist: uptrain (>=0.6.6)
+Requires-Dist: uptrain (>=0.7.1)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Callbacks Integration: UpTrain
 
 UpTrain ([github](https://github.com/uptrain-ai/uptrain) || [website](https://uptrain.ai/) || [docs](https://docs.uptrain.ai/getting-started/introduction)) is an open-source platform to evaluate and improve Generative AI applications. It provides grades for 20+ preconfigured checks (covering language, code, embedding use cases), performs root cause analysis on failure cases and gives insights on how to resolve them. Once you add UpTrainCallbackHandler to your existing LlamaIndex pipeline, it will automatically capture the right data, run evaluations and display the results in the output.
 
 More details on UpTrain's evaluations can be found [here](https://github.com/uptrain-ai/uptrain?tab=readme-ov-file#pre-built-evaluations-we-offer-).
```

