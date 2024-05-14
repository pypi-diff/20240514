# Comparing `tmp/promptedgraphs-0.3.3.tar.gz` & `tmp/promptedgraphs-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptedgraphs-0.3.3.tar", max compression
+gzip compressed data, was "promptedgraphs-0.4.3.tar", max compression
```

## Comparing `promptedgraphs-0.3.3.tar` & `promptedgraphs-0.4.3.tar`

### file list

```diff
@@ -1,25 +1,54 @@
--rw-r--r--   0        0        0     1080 2024-02-28 18:20:57.799261 promptedgraphs-0.3.3/LICENSE
--rw-r--r--   0        0        0     6635 2024-02-28 18:20:57.799261 promptedgraphs-0.3.3/README.md
--rw-r--r--   0        0        0      153 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/__init__.py
--rw-r--r--   0        0        0      119 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/__main__.py
--rw-r--r--   0        0        0      825 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/cli.py
--rw-r--r--   0        0        0      989 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/config.py
--rw-r--r--   0        0        0     9034 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/data_extraction.py
--rw-r--r--   0        0        0     7450 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/entity_recognition.py
--rw-r--r--   0        0        0     1056 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/example.py
--rw-r--r--   0        0        0      284 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/helpers.py
--rw-r--r--   0        0        0     8822 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/ideation.py
--rw-r--r--   0        0        0        0 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/llms/__init__.py
--rw-r--r--   0        0        0     1599 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/llms/coding.py
--rw-r--r--   0        0        0      997 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/llms/helpers.py
--rw-r--r--   0        0        0     3613 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/llms/openai_streaming.py
--rw-r--r--   0        0        0     4529 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/llms/openai_token_counter.py
--rw-r--r--   0        0        0     1028 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/models.py
--rw-r--r--   0        0        0      553 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/parsers.py
--rw-r--r--   0        0        0        0 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/sources/__init__.py
--rw-r--r--   0        0        0     7742 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/sources/datagraph_from_class.py
--rw-r--r--   0        0        0     9250 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/sources/datagraph_from_pydantic.py
--rw-r--r--   0        0        0     1889 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/sources/rtfm.py
--rw-r--r--   0        0        0     2643 2024-02-28 18:20:57.815261 promptedgraphs-0.3.3/promptedgraphs/vis.py
--rw-r--r--   0        0        0     1678 2024-02-28 18:21:57.611466 promptedgraphs-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     8393 1970-01-01 00:00:00.000000 promptedgraphs-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-14 18:10:49.347981 promptedgraphs-0.4.3/LICENSE
+-rw-r--r--   0        0        0     6485 2024-05-14 18:10:49.347981 promptedgraphs-0.4.3/README.md
+-rw-r--r--   0        0        0      153 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/__main__.py
+-rw-r--r--   0        0        0      825 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/cli.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/code_execution/__init__.py
+-rw-r--r--   0        0        0     2905 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/code_execution/safer_python_exec.py
+-rw-r--r--   0        0        0     1724 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/config.py
+-rw-r--r--   0        0        0     9034 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/data_extraction.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/data_modeling/__init__.py
+-rw-r--r--   0        0        0    19771 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/data_modeling/conceptual.py
+-rw-r--r--   0        0        0      453 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/data_modeling/logical.py
+-rw-r--r--   0        0        0      383 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/data_modeling/physical.py
+-rw-r--r--   0        0        0      122 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/entity_linking/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/entity_linking/__init__.py
+-rw-r--r--   0        0        0      549 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/entity_linking/link.py
+-rw-r--r--   0        0        0      320 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/entity_linking/upsertion.py
+-rw-r--r--   0        0        0     7435 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/entity_recognition.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/entity_resolution/__init__.py
+-rw-r--r--   0        0        0      665 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/entity_resolution/resolve.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/extraction/__init__.py
+-rw-r--r--   0        0        0     6198 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/extraction/data_from_text.py
+-rw-r--r--   0        0        0     3995 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/extraction/entities_from_text.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/generation/__init__.py
+-rw-r--r--   0        0        0     8287 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/generation/data_from_model.py
+-rw-r--r--   0        0        0     9475 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/generation/schema_from_data.py
+-rw-r--r--   0        0        0     2430 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/generation/schema_from_model.py
+-rw-r--r--   0        0        0     1622 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/llms/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/llms/anthropic_chat.py
+-rw-r--r--   0        0        0     1938 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/llms/chat.py
+-rw-r--r--   0        0        0     1599 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/llms/coding.py
+-rw-r--r--   0        0        0      997 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/llms/helpers.py
+-rw-r--r--   0        0        0     1398 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/llms/openai_chat.py
+-rw-r--r--   0        0        0     3674 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/llms/openai_streaming.py
+-rw-r--r--   0        0        0     5472 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/llms/usage.py
+-rw-r--r--   0        0        0     1028 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/models.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/normalization/__init__.py
+-rw-r--r--   0        0        0     8938 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/normalization/object_to_data.py
+-rw-r--r--   0        0        0      352 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/normalization/schema_to_schema.py
+-rw-r--r--   0        0        0     3957 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/normalization/vis_graphs.py
+-rw-r--r--   0        0        0      553 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/parsers.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/sources/__init__.py
+-rw-r--r--   0        0        0     7742 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/sources/datagraph_from_class.py
+-rw-r--r--   0        0        0     9254 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/sources/datagraph_from_pydantic.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/statistical/__init__.py
+-rw-r--r--   0        0        0    11837 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/statistical/data_analysis.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/validation/__init__.py
+-rw-r--r--   0        0        0      946 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/validation/validate_data.py
+-rw-r--r--   0        0        0      396 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/validation/validate_schema.py
+-rw-r--r--   0        0        0     2657 2024-05-14 18:10:49.363981 promptedgraphs-0.4.3/promptedgraphs/vis.py
+-rw-r--r--   0        0        0     1934 2024-05-14 18:13:50.964285 promptedgraphs-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     8773 1970-01-01 00:00:00.000000 promptedgraphs-0.4.3/PKG-INFO
```

### Comparing `promptedgraphs-0.3.3/LICENSE` & `promptedgraphs-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `promptedgraphs-0.3.3/README.md` & `promptedgraphs-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ### Entity Recognition
 
 from [examples/er_reviews.ipynb](https://github.com/closedloop-technologies/PromptedGraphs/blob/main/examples/er_reviews.ipynb)
 
 ```python
 from spacy import displacy
 from promptedgraphs.config import Config
-from promptedgraphs.entity_recognition import extract_entities
+from promptedgraphs.extraction.entities_from_text import entities_from_text
 
 labels = {
     "POSITIVE": "A postive review of a product or service.",
     "NEGATIVE": "A negative review of a product or service.",
     "NEUTRAL": "A neutral review of a product or service.",
 }
 
@@ -56,35 +56,29 @@
 2. "The service was quite poor and the staff was rude."
 3. "The item is okay. Nothing special, but it gets the job done."
 """.strip()
 
 
 # Label Sentiment
 ents = []
-async for msg in extract_entities(
+async for msg in entities_from_text(
     name="sentiment",
     description="Sentiment Analysis of Customer Reviews",
     text=text_of_reviews,
     labels=labels,
     config=Config(),  # Reads `OPENAI_API_KEY` from .env file or environment
 ):
     ents.append(msg)
 
 # Show Results using spacy.displacy
-displacy.render(
-    {
-        "text": text_of_reviews,
-        "ents": [e.to_dict() for e in ents],
-    },
-    style="ent",
-    jupyter=True,
-    manual=True,
-    options={
-        "colors": {"POSITIVE": "#7aecec", "NEGATIVE": "#f44336", "NEUTRAL": "#f4f442"}
-    },
+render_entities(
+    text=text_of_reviews,
+    entities=ents,
+    labels=labels,
+    colors = {"POSITIVE": "#7aecec", "NEGATIVE": "#f44336", "NEUTRAL": "#f4f442"}
 )
 ```
 ![displacy-sentiment-example](./assets/displacy-sentiment-example.png?raw=true)
 
 ### Brainstorming Data
 Generate a list of data that fits a given data model.
 
@@ -132,15 +126,14 @@
 
 from [examples/de_chatintents.ipynb](https://github.com/closedloop-technologies/PromptedGraphs/blob/main/examples/de_chatintents.ipynb)
 
 ```python
 from pydantic import BaseModel, Field
 
 from promptedgraphs.config import Config
-from promptedgraphs.data_extraction import extract_data
 
 
 class UserIntent(BaseModel):
     """The UserIntent entity, representing the canonical description of what a user desires to achieve in a given conversation."""
 
     intent_name: str = Field(
         title="Intent Name",
@@ -162,16 +155,16 @@
         title="Intent Description",
         description="A detailed explanation of the user's intent",
     )
 
 
 msg = """It's a busy day, I need to send an email and to buy groceries"""
 
-async for intent in extract_data(
-    text=msg, output_type=list[UserIntent], config=Config()
+async for intent in data_from_text(
+    text=msg, output_type=UserIntent, config=Config()
 ):
     print(intent)
 ```
 ```bash
 intent_name='task' description='User wants to complete a task'
 intent_name='communication' description='User wants to send an email'
 intent_name='shopping' description='User wants to buy groceries'
```

### Comparing `promptedgraphs-0.3.3/promptedgraphs/cli.py` & `promptedgraphs-0.4.3/promptedgraphs/cli.py`

 * *Files identical despite different names*

### Comparing `promptedgraphs-0.3.3/promptedgraphs/data_extraction.py` & `promptedgraphs-0.4.3/promptedgraphs/data_extraction.py`

 * *Files identical despite different names*

### Comparing `promptedgraphs-0.3.3/promptedgraphs/entity_recognition.py` & `promptedgraphs-0.4.3/promptedgraphs/entity_recognition.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import tiktoken
 
 from promptedgraphs.config import Config
 from promptedgraphs.llms.openai_streaming import (
     GPT_MODEL,
     streaming_chat_completion_request,
 )
-from promptedgraphs.llms.openai_token_counter import Usage
+from promptedgraphs.llms.usage import Usage
 from promptedgraphs.models import ChatMessage, EntityReference
 from promptedgraphs.parsers import extract_partial_list
 
 # Name and description of entity types
 
 
 SYSTEM_MESSAGE = """
```

### Comparing `promptedgraphs-0.3.3/promptedgraphs/llms/coding.py` & `promptedgraphs-0.4.3/promptedgraphs/llms/coding.py`

 * *Files identical despite different names*

### Comparing `promptedgraphs-0.3.3/promptedgraphs/llms/helpers.py` & `promptedgraphs-0.4.3/promptedgraphs/llms/helpers.py`

 * *Files identical despite different names*

### Comparing `promptedgraphs-0.3.3/promptedgraphs/llms/openai_streaming.py` & `promptedgraphs-0.4.3/promptedgraphs/llms/openai_streaming.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import json
 from collections.abc import AsyncGenerator
 
 from httpx import AsyncClient, ReadTimeout
 from sse_starlette import ServerSentEvent
 
 from promptedgraphs.config import Config
-from promptedgraphs.llms.openai_token_counter import estimate_tokens
+from promptedgraphs.llms.openai_chat import LanguageModel
+from promptedgraphs.llms.usage import estimate_tokens
 from promptedgraphs.models import ChatFunction, ChatMessage
 
-GPT_MODEL = "gpt-3.5-turbo-1106"
-GPT_MODEL_BIG_CONTEXT = "gpt-3.5-turbo-16k-0613"
+GPT_MODEL = LanguageModel.GPT35_turbo.value
+GPT_MODEL_BIG_CONTEXT = LanguageModel.GPT35_turbo.value
 
 
 # @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(3))
 async def streaming_chat_completion_request(
     messages: list[ChatMessage] | None,
     functions: list[ChatFunction] | None = None,
     model=GPT_MODEL,
```

### Comparing `promptedgraphs-0.3.3/promptedgraphs/llms/openai_token_counter.py` & `promptedgraphs-0.4.3/promptedgraphs/llms/usage.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,64 @@
 import json
 import time
+from logging import getLogger
 
 import tiktoken
 
+from promptedgraphs.llms.openai_chat import LanguageModel
+
+logger = getLogger(__name__)
+
 
 class Usage:
     prompt_tokens: int = 0
     completion_tokens: int = 0
 
-    def __init__(self, model: str) -> None:
+    def __init__(self, model: str, computer: str = "unknown") -> None:
         self.model = model
+        self.computer = computer
+        self.duration = 0
+        self.prompt_tokens = 0
+        self.completion_tokens = 0
+        self.start_time = time.time()
 
     def start(self):
-        self.cost = 0
         self.prompt_tokens = 0
         self.completion_tokens = 0
         self.start_time = time.time()
 
     def end(self):
         self.end_time = time.time()
         self.duration = self.end_time - self.start_time
-        self.cost = openai_api_calculate_cost(self, model=self.model)
+
+    @property
+    def cost(self):
+        return self.llm_cost + self.compute_cost
+
+    @property
+    def llm_cost(self):
+        return calculate_langage_model_costs(self, model=self.model)
+
+    @property
+    def compute_cost(self):
+        return calculate_compute_costs(self, computer=self.computer)
 
     def dict(self):
         return {
             "model": self.model,
             "prompt_tokens": self.prompt_tokens,
             "completion_tokens": self.completion_tokens,
             "duration": self.duration,
             "cost": self.cost,
+            "llm_cost": self.llm_cost,
+            "compute_cost": self.compute_cost,
         }
 
     def __repr__(self) -> str:
-        return f"Usage(model={self.model}, prompt_tokens={self.prompt_tokens}, completion_tokens={self.completion_tokens}, duration={self.duration:.4f}, cost={self.cost:.6f})"
+        return f"Usage(model={self.model}, prompt_tokens={self.prompt_tokens}, completion_tokens={self.completion_tokens}, duration={self.duration:.4f}, cost={self.cost:.6f}), compute_cost={self.compute_cost:.6f}), llm_cost={self.llm_cost:.6f})"
 
 
 def num_tokens_from_messages(messages, model="gpt-3.5-turbo-1106"):
     """Returns the number of tokens used by a list of messages.
     See https://github.com/openai/openai-python/blob/main/chatml.md for information on how messages are converted to tokens.
     """
     try:
@@ -86,59 +108,58 @@
             ),
             allowed_special=set(encoding._special_tokens.keys()),
         )
     )
     return function_tokens + message_tokens
 
 
-def openai_api_calculate_cost(usage: Usage, model="gpt-4-1106-preview"):
+def calculate_compute_costs(usage: Usage, computer: str):
+    # Pricing in dollars per 1000 tokens
+    # Compute time calculated assuming AWS ondemand prices
+    # t4g.medium	$0.0336	2	4 GiB	EBS Only	Up to 5 Gigabit
+    default_compute_cost_second = 0.0336 / 60 / 60
+    pricing = {"t4g.medium": 0.0336 / 60 / 60}
+    try:
+        compute_pricing = pricing[computer]
+    except KeyError as e:
+        logger.debug(
+            f"Server {computer} not found in pricing table, using default pricing of {default_compute_cost_second:.6f}"
+        )
+        compute_pricing = default_compute_cost_second
+
+    return round(usage.duration * compute_pricing, 6)
+
+
+def calculate_langage_model_costs(usage: Usage, model: LanguageModel):
     # Pricing in dollars per 1000 tokenspricing = {
     pricing = {
-        "gpt-4-0125-preview": {
-            "prompt": 0.01,
-            "completion": 0.03,
-        },
-        "gpt-4-1106-preview": {
-            "prompt": 0.01,
-            "completion": 0.03,
-        },
-        "gpt-4-1106-vision-preview": {
-            "prompt": 0.01,
-            "completion": 0.03,
-        },
-        "gpt-4": {
+        LanguageModel.GPT4: {
             "prompt": 0.03,
             "completion": 0.06,
         },
-        "gpt-4-32k": {
-            "prompt": 0.06,
-            "completion": 0.12,
-        },
-        "gpt-3.5-turbo-1106": {
+        LanguageModel.GPT35_turbo: {
             "prompt": 0.0010,
             "completion": 0.0020,
         },
-        "gpt-3.5-turbo-instruct": {
-            "prompt": 0.0015,
-            "completion": 0.0020,
-        },
-        "davinci-002": {
-            "prompt": 0.0020,
-            "completion": 0.0020,  # No separate completion price listed
-        },
-        "babbage-002": {
-            "prompt": 0.0004,
-            "completion": 0.0004,  # No separate completion price listed
+        "default": {
+            "prompt": 0.0,
+            "completion": 0.0,
         },
     }
 
     try:
         model_pricing = pricing[model]
-    except KeyError:
-        return 0
+    except KeyError as e:
+        if isinstance(model, LanguageModel):
+            raise ValueError(f"Model {model} not found in pricing table") from e
+        else:
+            logger.warning(
+                f"Model {model} not found in pricing table, using default pricing of 0"
+            )
+            model_pricing = pricing["default"]
 
     prompt_cost = usage.prompt_tokens * model_pricing["prompt"] / 1000
     completion_cost = usage.completion_tokens * model_pricing["completion"] / 1000
 
     total_cost = prompt_cost + completion_cost
     # round to 6 decimals
     return round(total_cost, 6)
```

### Comparing `promptedgraphs-0.3.3/promptedgraphs/models.py` & `promptedgraphs-0.4.3/promptedgraphs/models.py`

 * *Files identical despite different names*

### Comparing `promptedgraphs-0.3.3/promptedgraphs/parsers.py` & `promptedgraphs-0.4.3/promptedgraphs/parsers.py`

 * *Files identical despite different names*

### Comparing `promptedgraphs-0.3.3/promptedgraphs/sources/datagraph_from_class.py` & `promptedgraphs-0.4.3/promptedgraphs/sources/datagraph_from_class.py`

 * *Files identical despite different names*

### Comparing `promptedgraphs-0.3.3/promptedgraphs/sources/datagraph_from_pydantic.py` & `promptedgraphs-0.4.3/promptedgraphs/sources/datagraph_from_pydantic.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import black
 import isort
 import networkx as nx
 import tqdm
 from pydantic import BaseModel, Field
 
+from promptedgraphs.code_execution.safer_python_exec import format_code
 from promptedgraphs.llms.coding import fix_code
 
 logger = logging.getLogger(__name__)
 
 # Restrictive environment
 allowed_globals = {
     "__import__": __import__,
@@ -30,14 +31,15 @@
     dependencies = dependencies or allowed_globals
 
     for snippet in code.split(
         "\n\n"
     ):  # Loading in code by chunks helps with dependency resolution
         dependencies.update(variables)
         exec(snippet, dependencies, variables)
+    DeprecationWarning("This is a deprecated function: use safer_exec")
     return variables
 
 
 def is_pydantic_base_model(cls: Any) -> bool:
     return isinstance(cls, type) and issubclass(cls, BaseModel)
 
 
@@ -197,29 +199,29 @@
 
 
 def aggregate_python_files(fdir):
     fdir = Path(fdir)
     code = []
     for fname in fdir.glob("*.py"):
         with open(fname) as f:
-            c = black.format_str(f.read(), mode=black.FileMode())
+            c = format_code(f.read())
             code.append(c)
             try:
-                black.format_str("\n\n".join(code), mode=black.FileMode())
+                format_code("\n\n".join(code))
             except Exception:
                 logger.error(f"Static code error in: {fname}")
                 return
 
     # move all imports to the top
     code = move_imports_to_top("\n\n".join(code))
     config = isort.Config(profile="black")
     code = isort.code(code, config=config)
 
     # reformat one more time
-    code = black.format_str(code, mode=black.FileMode())
+    code = format_code(code)
 
     with open(fdir / "_all.py", "w") as f:
         f.write(code)
 
     return fdir / "_all.py"
 
 
@@ -244,19 +246,19 @@
         if fname.name == "_all.py":
             continue
         code = Path(fname).read_text()
 
         history = []
         i = 0
         while i < 4:
-            code = black.format_str(code, mode=black.FileMode())
+            code = format_code(code)
             kindofsafe_exec(code)
             # break
             try:
-                code = black.format_str(code, mode=black.FileMode())
+                code = format_code(code)
                 kindofsafe_exec(code)
                 break
             except Exception as e:
                 i += 1
                 if i >= 4:
                     logger.error(f"Code error in: {fname}")
                     return
```

### Comparing `promptedgraphs-0.3.3/promptedgraphs/vis.py` & `promptedgraphs-0.4.3/promptedgraphs/vis.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     elif isinstance(ents[0], EntityReference):
         return sorted({e.label for e in ents})
     else:
         raise ValueError("ents must be a list of EntityReference, BaseModel or dict")
 
 
 def get_colors(fields: list[str], color_palette: list[float] = None):
-    palette = color_palette or sns.color_palette("Set2", 8)
-    return {f: rgb_to_hex(color) for f, color in zip(list(fields), palette)}
+    palette = color_palette or sns.color_palette("Set2", len(fields))
+    return {f: rgb_to_hex(color)[:7] for f, color in zip(list(fields), palette)}
 
 
 def ensure_entities(
     ents: list[EntityReference] | dict | BaseModel, text: str
 ) -> list[EntityReference]:
     if ents is None:
         return None
```

### Comparing `promptedgraphs-0.3.3/pyproject.toml` & `promptedgraphs-0.4.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promptedgraphs"
-version = "0.3.3"
+version = "0.4.3"
 description = "From Dataset Labeling to Deployment: The Power of NLP and LLMs Combined."
 authors = ["Sean Kruzel <sean@closedloop.tech>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "promptedgraphs" }]
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -13,15 +13,16 @@
 ]
 
 [tool.poetry.urls]
 "Repository" = "https://github.com/closedLoop-technologies/promptedgraphs"
 "Bug Tracker" = "https://github.com/closedLoop-technologies/promptedgraphs/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.13"
+python = "<4.0,>=3.10"
+pre-commit = "^3.3.1"
 gcloud = "^0.18.3"
 typer = "^0.9.0"
 pyfiglet = "^1.0.2"
 termcolor = "^2.4.0"
 tabulate = "^0.9.0"
 colorama = "^0.4.6"
 pydantic = "^2.6.3"
@@ -30,19 +31,31 @@
 spacy = "^3.7.4"
 googlemaps = "^4.10.0"
 beautifulsoup4 = "^4.12.3"
 networkx = "^3.2.1"
 pandas = "^2.2.1"
 seaborn = "^0.13.2"
 nltk = "^3.8.1"
-transformers = "^4.38.1"
-python-dotenv = "^1.0.1"
-dataclasses-json = "^0.6.4"
-sse-starlette = "^2.0.0"
-pydantic-settings = "^2.2.1"
+transformers = "^4.37.2"
+matplotlib = "^3.8.0"
+jupyter = "^1.0.0"
+openai = "^1.12.0"
+scikit-learn = "^1.4.0"
+cohere = "^4.47"
+flair = "^0.13.1"
+spacy-experimental = "^0.6.4"
+ipykernel = "^6.29.2"
+amrlib = "^0.8.0"
+unidecode = "^1.3.8"
+penman = "^1.3.0"
+datamodel-code-generator = "^0.25.5"
+pyarrow = "^15.0.2"
+torch = "^2.2.2"
+pydot = "^2.0.0"
+jsonpath-ng = "^1.6.1"
 twine = "^5.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 coverage = "^7.2.5"
 eradicate = "^2.2.0"
 isort = "^5.12.0"
```

### Comparing `promptedgraphs-0.3.3/PKG-INFO` & `promptedgraphs-0.4.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 Metadata-Version: 2.1
 Name: promptedgraphs
-Version: 0.3.3
+Version: 0.4.3
 Summary: From Dataset Labeling to Deployment: The Power of NLP and LLMs Combined.
 License: MIT
 Author: Sean Kruzel
 Author-email: sean@closedloop.tech
-Requires-Python: >=3.10,<3.13
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: amrlib (>=0.8.0,<0.9.0)
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
+Requires-Dist: cohere (>=4.47,<5.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
+Requires-Dist: datamodel-code-generator (>=0.25.5,<0.26.0)
+Requires-Dist: flair (>=0.13.1,<0.14.0)
 Requires-Dist: gcloud (>=0.18.3,<0.19.0)
 Requires-Dist: googlemaps (>=4.10.0,<5.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: ipykernel (>=6.29.2,<7.0.0)
+Requires-Dist: jsonpath-ng (>=1.6.1,<2.0.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
+Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: penman (>=1.3.0,<2.0.0)
+Requires-Dist: pre-commit (>=3.3.1,<4.0.0)
+Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
-Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
+Requires-Dist: pydot (>=2.0.0,<3.0.0)
 Requires-Dist: pyfiglet (>=1.0.2,<2.0.0)
-Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: scikit-learn (>=1.4.0,<2.0.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: spacy (>=3.7.4,<4.0.0)
-Requires-Dist: sse-starlette (>=2.0.0,<3.0.0)
+Requires-Dist: spacy-experimental (>=0.6.4,<0.7.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
-Requires-Dist: transformers (>=4.38.1,<5.0.0)
+Requires-Dist: torch (>=2.2.2,<3.0.0)
+Requires-Dist: transformers (>=4.37.2,<5.0.0)
 Requires-Dist: twine (>=5.0.0,<6.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: unidecode (>=1.3.8,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/closedLoop-technologies/promptedgraphs/issues
 Project-URL: Repository, https://github.com/closedLoop-technologies/promptedgraphs
 Description-Content-Type: text/markdown
 
 # PromptedGraphs
 
 **From Dataset Labeling to Deployment: The Power of NLP and LLMs Combined.**
@@ -80,15 +93,15 @@
 ### Entity Recognition
 
 from [examples/er_reviews.ipynb](https://github.com/closedloop-technologies/PromptedGraphs/blob/main/examples/er_reviews.ipynb)
 
 ```python
 from spacy import displacy
 from promptedgraphs.config import Config
-from promptedgraphs.entity_recognition import extract_entities
+from promptedgraphs.extraction.entities_from_text import entities_from_text
 
 labels = {
     "POSITIVE": "A postive review of a product or service.",
     "NEGATIVE": "A negative review of a product or service.",
     "NEUTRAL": "A neutral review of a product or service.",
 }
 
@@ -97,35 +110,29 @@
 2. "The service was quite poor and the staff was rude."
 3. "The item is okay. Nothing special, but it gets the job done."
 """.strip()
 
 
 # Label Sentiment
 ents = []
-async for msg in extract_entities(
+async for msg in entities_from_text(
     name="sentiment",
     description="Sentiment Analysis of Customer Reviews",
     text=text_of_reviews,
     labels=labels,
     config=Config(),  # Reads `OPENAI_API_KEY` from .env file or environment
 ):
     ents.append(msg)
 
 # Show Results using spacy.displacy
-displacy.render(
-    {
-        "text": text_of_reviews,
-        "ents": [e.to_dict() for e in ents],
-    },
-    style="ent",
-    jupyter=True,
-    manual=True,
-    options={
-        "colors": {"POSITIVE": "#7aecec", "NEGATIVE": "#f44336", "NEUTRAL": "#f4f442"}
-    },
+render_entities(
+    text=text_of_reviews,
+    entities=ents,
+    labels=labels,
+    colors = {"POSITIVE": "#7aecec", "NEGATIVE": "#f44336", "NEUTRAL": "#f4f442"}
 )
 ```
 ![displacy-sentiment-example](./assets/displacy-sentiment-example.png?raw=true)
 
 ### Brainstorming Data
 Generate a list of data that fits a given data model.
 
@@ -173,15 +180,14 @@
 
 from [examples/de_chatintents.ipynb](https://github.com/closedloop-technologies/PromptedGraphs/blob/main/examples/de_chatintents.ipynb)
 
 ```python
 from pydantic import BaseModel, Field
 
 from promptedgraphs.config import Config
-from promptedgraphs.data_extraction import extract_data
 
 
 class UserIntent(BaseModel):
     """The UserIntent entity, representing the canonical description of what a user desires to achieve in a given conversation."""
 
     intent_name: str = Field(
         title="Intent Name",
@@ -203,16 +209,16 @@
         title="Intent Description",
         description="A detailed explanation of the user's intent",
     )
 
 
 msg = """It's a busy day, I need to send an email and to buy groceries"""
 
-async for intent in extract_data(
-    text=msg, output_type=list[UserIntent], config=Config()
+async for intent in data_from_text(
+    text=msg, output_type=UserIntent, config=Config()
 ):
     print(intent)
 ```
 ```bash
 intent_name='task' description='User wants to complete a task'
 intent_name='communication' description='User wants to send an email'
 intent_name='shopping' description='User wants to buy groceries'
```

