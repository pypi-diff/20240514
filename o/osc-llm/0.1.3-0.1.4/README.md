# Comparing `tmp/osc_llm-0.1.3.tar.gz` & `tmp/osc_llm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc_llm-0.1.3.tar", max compression
+gzip compressed data, was "osc_llm-0.1.4.tar", max compression
```

## Comparing `osc_llm-0.1.3.tar` & `osc_llm-0.1.4.tar`

### file list

```diff
@@ -1,47 +1,45 @@
--rw-r--r--   0        0        0      765 2024-05-09 08:34:18.837586 osc_llm-0.1.3/README.md
--rw-r--r--   0        0        0      253 2024-04-30 00:21:10.635963 osc_llm-0.1.3/osc_llm/__init__.py
--rw-r--r--   0        0        0     6755 2024-05-09 10:15:03.646846 osc_llm-0.1.3/osc_llm/__main__.py
--rw-r--r--   0        0        0       51 2024-04-27 15:22:11.337904 osc_llm-0.1.3/osc_llm/architectures/__init__.py
--rw-r--r--   0        0        0     8089 2024-04-27 15:21:42.709990 osc_llm-0.1.3/osc_llm/architectures/transformer_decoder.py
--rw-r--r--   0        0        0     4697 2024-05-08 23:04:00.078814 osc_llm-0.1.3/osc_llm/chat.py
--rw-r--r--   0        0        0      136 2024-04-29 08:59:09.247275 osc_llm-0.1.3/osc_llm/chat_templates/__init__.py
--rw-r--r--   0        0        0     1663 2024-05-09 08:19:44.319893 osc_llm-0.1.3/osc_llm/chat_templates/base.py
--rw-r--r--   0        0        0     1058 2024-05-09 08:43:14.223105 osc_llm-0.1.3/osc_llm/chat_templates/chatml.py
--rw-r--r--   0        0        0     2933 2024-05-09 08:19:52.915836 osc_llm-0.1.3/osc_llm/chat_templates/llama.py
--rw-r--r--   0        0        0     1314 2024-04-29 23:11:24.182541 osc_llm-0.1.3/osc_llm/config.py
--rw-r--r--   0        0        0       48 2024-04-27 15:57:52.529093 osc_llm-0.1.3/osc_llm/demos/__init__.py
--rw-r--r--   0        0        0     5517 2024-04-27 16:06:43.049671 osc_llm-0.1.3/osc_llm/demos/language_model.py
--rw-r--r--   0        0        0       83 2024-04-29 23:43:54.288202 osc_llm-0.1.3/osc_llm/engines/__init__.py
--rw-r--r--   0        0        0     1951 2024-05-09 00:43:57.688337 osc_llm-0.1.3/osc_llm/engines/base.py
--rw-r--r--   0        0        0     4207 2024-05-07 01:00:24.504971 osc_llm-0.1.3/osc_llm/engines/v1.py
--rw-r--r--   0        0        0     4916 2024-04-30 14:10:25.104449 osc_llm-0.1.3/osc_llm/engines/v2.py
--rw-r--r--   0        0        0      705 2024-05-09 10:13:55.630489 osc_llm-0.1.3/osc_llm/layers/__init__.py
--rw-r--r--   0        0        0      650 2024-04-27 15:10:30.656849 osc_llm-0.1.3/osc_llm/layers/activation.py
--rw-r--r--   0        0        0     6224 2024-04-27 15:10:30.680848 osc_llm-0.1.3/osc_llm/layers/attention.py
--rw-r--r--   0        0        0      186 2024-04-27 15:17:53.918752 osc_llm-0.1.3/osc_llm/layers/dropout.py
--rw-r--r--   0        0        0     2238 2024-04-27 15:10:30.684848 osc_llm-0.1.3/osc_llm/layers/embedding.py
--rw-r--r--   0        0        0     3371 2024-04-27 15:10:30.684848 osc_llm-0.1.3/osc_llm/layers/feedforward.py
--rw-r--r--   0        0        0      336 2024-04-27 15:10:30.684848 osc_llm-0.1.3/osc_llm/layers/head.py
--rw-r--r--   0        0        0     2745 2024-04-27 15:10:30.684848 osc_llm-0.1.3/osc_llm/layers/kv_cache.py
--rw-r--r--   0        0        0     6023 2024-05-09 10:13:37.142379 osc_llm-0.1.3/osc_llm/layers/linear.py
--rw-r--r--   0        0        0      823 2024-04-27 15:10:30.688848 osc_llm-0.1.3/osc_llm/layers/normalization.py
--rw-r--r--   0        0        0      416 2024-04-27 15:17:28.926844 osc_llm-0.1.3/osc_llm/model_helpers/__init__.py
--rw-r--r--   0        0        0     4350 2024-05-09 10:16:01.331095 osc_llm-0.1.3/osc_llm/model_helpers/base.py
--rw-r--r--   0        0        0     3054 2024-04-27 15:16:30.027073 osc_llm-0.1.3/osc_llm/model_helpers/llama.py
--rw-r--r--   0        0        0     3285 2024-05-09 07:37:31.990997 osc_llm-0.1.3/osc_llm/model_helpers/qwen.py
--rw-r--r--   0        0        0       46 2024-04-27 15:00:44.802617 osc_llm-0.1.3/osc_llm/optimizers/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-27 15:00:44.802617 osc_llm-0.1.3/osc_llm/optimizers/scheduler.py
--rw-r--r--   0        0        0      139 2024-05-09 10:14:52.802794 osc_llm-0.1.3/osc_llm/quantizers/__init__.py
--rw-r--r--   0        0        0      717 2024-04-27 15:10:37.244808 osc_llm-0.1.3/osc_llm/quantizers/base.py
--rw-r--r--   0        0        0     8861 2024-04-27 15:33:29.096094 osc_llm-0.1.3/osc_llm/quantizers/int4.py
--rw-r--r--   0        0        0     3912 2024-05-09 10:18:30.539547 osc_llm-0.1.3/osc_llm/quantizers/int8.py
--rw-r--r--   0        0        0       74 2024-04-27 15:04:12.071947 osc_llm-0.1.3/osc_llm/samplers/__init__.py
--rw-r--r--   0        0        0      903 2024-04-27 15:04:12.079947 osc_llm-0.1.3/osc_llm/samplers/base.py
--rw-r--r--   0        0        0     1122 2024-05-09 11:29:40.084349 osc_llm-0.1.3/osc_llm/samplers/top_k.py
--rw-r--r--   0        0        0     1121 2024-04-27 15:04:12.083947 osc_llm-0.1.3/osc_llm/samplers/top_p.py
--rw-r--r--   0        0        0        0 2024-05-06 11:34:05.202914 osc_llm-0.1.3/osc_llm/servers/__init__.py
--rw-r--r--   0        0        0     7453 2024-05-09 11:17:44.753636 osc_llm-0.1.3/osc_llm/servers/openai.py
--rw-r--r--   0        0        0     8873 2024-05-09 08:14:53.581992 osc_llm-0.1.3/osc_llm/tokenizer.py
--rw-r--r--   0        0        0     6405 2024-05-06 10:35:40.498735 osc_llm-0.1.3/osc_llm/utils.py
--rw-r--r--   0        0        0      547 2024-05-08 23:00:15.836746 osc_llm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1626 1970-01-01 00:00:00.000000 osc_llm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1809 2024-05-14 08:53:38.515299 osc_llm-0.1.4/README.md
+-rw-r--r--   0        0        0      253 2024-04-30 00:21:10.635963 osc_llm-0.1.4/osc_llm/__init__.py
+-rw-r--r--   0        0        0     6755 2024-05-14 06:47:02.440862 osc_llm-0.1.4/osc_llm/__main__.py
+-rw-r--r--   0        0        0       51 2024-04-27 15:22:11.337904 osc_llm-0.1.4/osc_llm/architectures/__init__.py
+-rw-r--r--   0        0        0     8714 2024-05-14 21:34:40.711264 osc_llm-0.1.4/osc_llm/architectures/transformer_decoder.py
+-rw-r--r--   0        0        0     4618 2024-05-14 21:34:23.938634 osc_llm-0.1.4/osc_llm/chat.py
+-rw-r--r--   0        0        0      178 2024-05-10 19:18:14.078967 osc_llm-0.1.4/osc_llm/chat_templates/__init__.py
+-rw-r--r--   0        0        0     2381 2024-05-14 08:11:14.162668 osc_llm-0.1.4/osc_llm/chat_templates/base.py
+-rw-r--r--   0        0        0     1243 2024-05-10 19:18:05.762999 osc_llm-0.1.4/osc_llm/chat_templates/chatglm.py
+-rw-r--r--   0        0        0     1052 2024-05-10 15:02:28.353483 osc_llm-0.1.4/osc_llm/chat_templates/chatml.py
+-rw-r--r--   0        0        0     2998 2024-05-12 01:07:05.171122 osc_llm-0.1.4/osc_llm/chat_templates/llama.py
+-rw-r--r--   0        0        0     1314 2024-04-29 23:11:24.182541 osc_llm-0.1.4/osc_llm/config.py
+-rw-r--r--   0        0        0       83 2024-04-29 23:43:54.288202 osc_llm-0.1.4/osc_llm/engines/__init__.py
+-rw-r--r--   0        0        0     1951 2024-05-09 00:43:57.688337 osc_llm-0.1.4/osc_llm/engines/base.py
+-rw-r--r--   0        0        0     4415 2024-05-12 02:14:14.779802 osc_llm-0.1.4/osc_llm/engines/v1.py
+-rw-r--r--   0        0        0     4916 2024-04-30 14:10:25.104449 osc_llm-0.1.4/osc_llm/engines/v2.py
+-rw-r--r--   0        0        0      742 2024-05-12 01:04:34.995436 osc_llm-0.1.4/osc_llm/layers/__init__.py
+-rw-r--r--   0        0        0      650 2024-04-27 15:10:30.656849 osc_llm-0.1.4/osc_llm/layers/activation.py
+-rw-r--r--   0        0        0     7100 2024-05-11 02:07:54.277363 osc_llm-0.1.4/osc_llm/layers/attention.py
+-rw-r--r--   0        0        0      186 2024-04-27 15:17:53.918752 osc_llm-0.1.4/osc_llm/layers/dropout.py
+-rw-r--r--   0        0        0     2238 2024-04-27 15:10:30.684848 osc_llm-0.1.4/osc_llm/layers/embedding.py
+-rw-r--r--   0        0        0     7718 2024-05-13 03:52:36.763618 osc_llm-0.1.4/osc_llm/layers/feedforward.py
+-rw-r--r--   0        0        0      336 2024-04-27 15:10:30.684848 osc_llm-0.1.4/osc_llm/layers/head.py
+-rw-r--r--   0        0        0     2745 2024-04-27 15:10:30.684848 osc_llm-0.1.4/osc_llm/layers/kv_cache.py
+-rw-r--r--   0        0        0     6023 2024-05-09 10:13:37.142379 osc_llm-0.1.4/osc_llm/layers/linear.py
+-rw-r--r--   0        0        0      823 2024-04-27 15:10:30.688848 osc_llm-0.1.4/osc_llm/layers/normalization.py
+-rw-r--r--   0        0        0      476 2024-05-11 02:36:34.029609 osc_llm-0.1.4/osc_llm/model_helpers/__init__.py
+-rw-r--r--   0        0        0     5307 2024-05-14 06:30:15.939422 osc_llm-0.1.4/osc_llm/model_helpers/base.py
+-rw-r--r--   0        0        0     2690 2024-05-12 00:37:30.862834 osc_llm-0.1.4/osc_llm/model_helpers/chatglm.py
+-rw-r--r--   0        0        0     3054 2024-04-27 15:16:30.027073 osc_llm-0.1.4/osc_llm/model_helpers/llama.py
+-rw-r--r--   0        0        0     8206 2024-05-10 14:25:45.437854 osc_llm-0.1.4/osc_llm/model_helpers/qwen.py
+-rw-r--r--   0        0        0      139 2024-05-09 10:14:52.802794 osc_llm-0.1.4/osc_llm/quantizers/__init__.py
+-rw-r--r--   0        0        0      717 2024-04-27 15:10:37.244808 osc_llm-0.1.4/osc_llm/quantizers/base.py
+-rw-r--r--   0        0        0     8861 2024-04-27 15:33:29.096094 osc_llm-0.1.4/osc_llm/quantizers/int4.py
+-rw-r--r--   0        0        0     3912 2024-05-09 10:18:30.539547 osc_llm-0.1.4/osc_llm/quantizers/int8.py
+-rw-r--r--   0        0        0       74 2024-04-27 15:04:12.071947 osc_llm-0.1.4/osc_llm/samplers/__init__.py
+-rw-r--r--   0        0        0      903 2024-04-27 15:04:12.079947 osc_llm-0.1.4/osc_llm/samplers/base.py
+-rw-r--r--   0        0        0     1122 2024-05-09 11:29:40.084349 osc_llm-0.1.4/osc_llm/samplers/top_k.py
+-rw-r--r--   0        0        0     1121 2024-04-27 15:04:12.083947 osc_llm-0.1.4/osc_llm/samplers/top_p.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:34:05.202914 osc_llm-0.1.4/osc_llm/servers/__init__.py
+-rw-r--r--   0        0        0     7566 2024-05-14 21:01:20.596843 osc_llm-0.1.4/osc_llm/servers/openai.py
+-rw-r--r--   0        0        0     8999 2024-05-12 02:11:06.295796 osc_llm-0.1.4/osc_llm/tokenizer.py
+-rw-r--r--   0        0        0     7136 2024-05-14 21:02:58.383637 osc_llm-0.1.4/osc_llm/utils.py
+-rw-r--r--   0        0        0      717 2024-05-14 20:58:22.477897 osc_llm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 osc_llm-0.1.4/PKG-INFO
```

### Comparing `osc_llm-0.1.3/osc_llm/__main__.py` & `osc_llm-0.1.4/osc_llm/__main__.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/architectures/transformer_decoder.py` & `osc_llm-0.1.4/osc_llm/architectures/transformer_decoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -172,14 +172,31 @@
         
         return x
     
     def load_state_dict(self, state_dict: Mapping[str, Any], strict: bool = True, assign: bool = True):
         # 保证在用torch.device('meta')构建模型后, 可以运行model.to('cuda:xxx'),不然会由于cos和sin是meta data而报错
         self.setup_rope_cache(max_length=self.max_length)
         return super().load_state_dict(state_dict, strict, assign)
+    
+    def model_size(self, include_embeddings: bool = True) -> int:
+        """Calculate the model size.
+
+        Args:
+            include_embeddings (bool, optional): Include embeddings in the model size. Defaults to True.
+
+        Returns:
+            int: Model size
+        """
+        import itertools
+        model_size = 0
+        for n, children in self.named_children():
+            if n == "embedding" and not include_embeddings:
+                continue
+            model_size += sum([p.numel() * p.dtype.itemsize for p in itertools.chain(children.parameters(), children.buffers())])
+        return model_size
             
     
 def build_rope_cache(seq_len: int, n_elem: int, dtype: torch.dtype, device: torch.device, base: int = 10000, condense_ratio: int = 1) -> RoPECache:
     """Enhanced Transformer with Rotary Position Embedding.
 
     Derived from: https://github.com/labmlai/annotated_deep_learning_paper_implementations/blob/master/labml_nn/
     transformers/rope/__init__.py. MIT License:
```

### Comparing `osc_llm-0.1.3/osc_llm/chat.py` & `osc_llm-0.1.4/osc_llm/chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from .chat_templates import Message
 from .samplers import TopK
 from .engines import LLMEngineV1, LLMEngine, LLMEngineV2
 import torch
 import time
 from pathlib import Path
 from typing import Optional, Literal
-from itertools import chain
 
 
 
 torch.set_float32_matmul_precision('high')
     
 
 @torch.inference_mode()
@@ -51,17 +50,17 @@
                                         sampler=sampler,
                                         max_length=max_length,
                                         devices=[device],
                                         compile=compile)
     engine.setup()
     
     if not hasattr(engine, "decode_model"):
-        model_size = sum([p.numel() * p.dtype.itemsize for p in chain(engine.model.parameters(), engine.model.buffers())])
+        model_size = engine.model.model_size(include_embeddings=False)
     else:
-        model_size = sum([p.numel() * p.dtype.itemsize for p in chain(engine.decode_model.parameters(), engine.decode_model.buffers())])
+        model_size = engine.decode_model.model_size(include_embeddings=False) + engine.prefill_model.model_size(include_embeddings=False)
     
     if compile:
         t = time.perf_counter()
         input_ids = tokenizer.encode_messages([Message(role='user', content="你好")])
         stream = engine.run(input_ids=input_ids, stop_ids=tokenizer.stop_ids)
         token_stream = tokenizer.decode_stream(stream=stream)
         for token in token_stream:
```

### Comparing `osc_llm-0.1.3/osc_llm/chat_templates/base.py` & `osc_llm-0.1.4/osc_llm/chat_templates/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,33 @@
-from typing import List, Literal, Optional
+from typing import List, Literal, Optional, Dict
 from pydantic import BaseModel
 from pathlib import Path
 from ..config import registry, Config
 
 
 
+class Property(BaseModel):
+    type: str
+    description: Optional[str] = None
+    
+class Parameters(BaseModel):
+    type: str 
+    properties: Dict[str, Property]
+    required: List[str]
+
+class Tool(BaseModel):
+    name: str
+    description: str
+    parameters: Parameters
+
 class Message(BaseModel):
-    role: Literal["system", "user", "assistant"]
+    role: Literal["system", "user", "assistant", "observation"]
     content: str
+    metadata: str = ""
+    tools: List[Tool] = []
     
 
 class ChatTemplate():
     
     default_system: Optional[str] = ''
     stop_texts: List[str] = []
     generate_prompt: str = ''
@@ -27,27 +43,34 @@
             messages.append(Message(role="system", content=cls.default_system))
         messages.append(Message(role="user", content=user))
         return cls.apply_messages(messages, add_generate_prompt=add_generate_prompt)
 
     @classmethod
     def get_config(cls) -> Config:
         for k, v in registry.chat_templates.get_all().items():
-            if isinstance(cls, v):
+            if cls == v:
                 name = k
         config_str = f"""
         [chat_template]
         @chat_templates = {name}"""
         config = Config().from_str(config_str)
         return config
     
     @classmethod
     def from_name(cls, name: str) -> "ChatTemplate":
         template_cls = None
         for k, v in registry.chat_templates.get_all().items():
             if k in name:
                 template_cls = v
+        if template_cls is None:
+            raise ValueError(f"Chat template for {name} not found")
         return template_cls
     
     @classmethod
     def from_checkpoint(cls, checkpoint_dir: str) -> "ChatTemplate":
         checkpoint_dir = Path(checkpoint_dir)
+        config_path: Path = checkpoint_dir / "config.cfg"
+        if config_path.exists():
+            config = Config().from_disk(config_path)
+            if 'chat_template' in config:
+                return registry.chat_templates.get(config['chat_template']['@chat_templates'])
         return cls.from_name(checkpoint_dir.stem)
```

### Comparing `osc_llm-0.1.3/osc_llm/chat_templates/chatml.py` & `osc_llm-0.1.4/osc_llm/chat_templates/chatml.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     generate_prompt: str = "<|im_start|>assistant\n"
     
     @classmethod
     def apply_messages(cls, messages: List[Message], add_generate_prompt: bool = True) -> str:
         prompt = ""
         for message in messages:
             if message.role == "user":
-                prompt += f"<|im_start|>user\n{message.content}\n<|im_end|>\n"
+                prompt += f"<|im_start|>user\n{message.content}<|im_end|>\n"
             elif message.role == "assistant":
-                prompt += f"<|im_start|>assistant\n{message.content}\n<|im_end|>\n"
+                prompt += f"<|im_start|>assistant\n{message.content}<|im_end|>\n"
             elif message.role == "system":
-                prompt += f"<|im_start|>system\n{message.content}\n<|im_end|>\n"
+                prompt += f"<|im_start|>system\n{message.content}<|im_end|>\n"
         if add_generate_prompt:
             prompt += cls.generate_prompt
         return prompt
```

### Comparing `osc_llm-0.1.3/osc_llm/chat_templates/llama.py` & `osc_llm-0.1.4/osc_llm/chat_templates/llama.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 from .base import ChatTemplate, Message
 from ..config import registry
 
 
 @registry.chat_templates.register("Llama3-8B-Chinese-Chat")
+@registry.chat_templates.register("llama-3-chinese-8b-instruct")
 @registry.chat_templates.register("Llama-3")
 class Llama3ChatTemplate(ChatTemplate):
     
     stop_texts: List[str] = ["<|end_of_text|>", "<|eot_id|>"]
     generate_prompt: str = "<|start_header_id|>assistant<|end_header_id|>\n\n"
     
     @classmethod
```

### Comparing `osc_llm-0.1.3/osc_llm/config.py` & `osc_llm-0.1.4/osc_llm/config.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/demos/language_model.py` & `osc_llm-0.1.4/osc_llm/model_helpers/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,140 +1,124 @@
-import lightning as L
+import json 
 from pathlib import Path
-from lightning.pytorch.utilities.types import STEP_OUTPUT, OptimizerLRScheduler
-import requests
-from torch.utils.data import Dataset, DataLoader
-from typing import Any, Tuple
-from torch import Tensor
+from typing import Dict
 import torch
-from ..optimizers import get_cosine_lr_scheduler
+from ..config import Config, registry
 from ..utils import build_model
+from ..tokenizer import Tokenizer
+from ..chat_templates import ChatTemplate
+from wasabi import msg
 
 
-class TangShi(Dataset):
-    def __init__(self, 
-                 data_dir: str = 'data',
-                 block_size: int = 40,
-                 download: bool = True,
-                 ) -> None:
-        super().__init__()
-        self.data_dir = Path(data_dir)
-        self.path = self.data_dir / "tangshi.txt"
-        self.block_size = block_size
-        if download:
-            self.download()
-        self.data, self.vocab = self.tokenize()
-        
-    def __len__(self) -> int:
-        return len(self.data) // self.block_size
+
+class HFModelHelper:
+    """huggingface模型转换工具基类,一般情况下只需要完成`weight_map`属性和`osc_config`属性即可。
+    """
+    
+    hf_architecture: str
+    
+    def __init__(self, checkpoint_dir: str):
+        self.checkpoint_dir = Path(checkpoint_dir)
+        with open(self.checkpoint_dir / "config.json", "r") as f:
+            self.hf_config = json.load(f)
+        assert self.hf_architecture in self.hf_config['architectures'], f'Only support {self.hf_architecture} model, current model is {self.hf_config["architectures"]}'
+        try:
+            self.tokenizer = Tokenizer(self.checkpoint_dir)
+        except Exception:
+            msg.warn("No tokenizer found")
+            self.tokenizer = None
     
-    def __getitem__(self, index: int) -> Tuple[Tensor, Tensor]:
-        start = index * self.block_size
-        end = start + self.block_size
-        inputs = self.data[start:end]
-        target = self.data[(start + 1) : (end + 1)]
-        return inputs, target
-    
-    def download(self):
-        if not self.data_dir.exists():
-            self.data_dir.mkdir(parents=True)
-        if self.path.exists():
-            return
-        url = 'https://deepasset.oss-cn-beijing.aliyuncs.com/tangshi.txt'
-        with open(self.path, 'x') as f:
-            f.write(requests.get(url).text)
-            
-    def tokenize(self):
-        ids = []
-        vocab = Vocab()
-        vocab.add_token('<pad>')
-        vocab.add_token('<s>')
-        vocab.add_token('</s>')
-        with open(self.path, encoding="utf8") as f:
-            for line in f:
-                chars = list(line.strip())
-                for char in chars:
-                    vocab.add_token(char)
-                    ids.append(vocab.token2id[char])
-                ids.append(vocab.token2id['</s>'])
-        return torch.tensor(ids, dtype=torch.long), vocab
-        
-                  
-class Vocab():
-    def __init__(self) -> None:
-        self.token2id = {}
-        self.id2token = {}
+    @property
+    def weight_map(self) -> Dict:
+        """用来进行参数名称转换"""
+        raise NotImplementedError("Method not implemented")
     
     @property
-    def vocab_size(self):
-        return len(self.token2id)
+    def osc_config(self) -> Config:
+        """用来构建osc格式模型的配置文件"""
+        raise NotImplementedError("Method not implemented")
     
-    def __len__(self):
-        return len(self.token2id)
-        
-    def add_token(self, token):
-        if token not in self.token2id:
-            self.id2token[len(self.token2id)] = token
-            self.token2id[token] = len(self.token2id)
-            
-            
-            
-class TangshiLanguageModel(L.LightningModule):
-    def __init__(self,
-                 config: str,
-                 lr: float = 1e-4,
-                 block_size: int = 100,
-                 batch_size: int = 16) -> None:
-        super().__init__()
-        self.save_hyperparameters()
-        self.model = build_model(config=config, empty_init=False)
-        self.dataset = TangShi(block_size=block_size)
+    def convert_checkpoint(self, save_dir: str, add_chat_template: bool = True):
+        """将huggingface模型转换为osc格式模型
+
+        Args:
+            save_dir (str): 保存目录
+        """
+        pytorch_model = Path(self.checkpoint_dir) / 'pytorch_model.bin'
+        pytorch_idx_file = Path(self.checkpoint_dir) / 'pytorch_model.bin.index.json'
+        if pytorch_model.exists() or pytorch_idx_file.exists():
+            sd = self.convert_pytorch_format()
+        safetensors_model = Path(self.checkpoint_dir) / 'model.safetensors'
+        safetensors_idx_file = Path(self.checkpoint_dir) / 'model.safetensors.index.json'
+        if safetensors_model.exists() or safetensors_idx_file.exists():
+            sd = self.convert_safetensor_format()
+        if not pytorch_model.exists() and not safetensors_model.exists() and not pytorch_idx_file.exists() and not safetensors_idx_file.exists():
+            raise FileNotFoundError("No pytorch model file found")
+        out_dir = Path(save_dir)
+        if not out_dir.exists():
+            out_dir.mkdir(parents=True)
+        torch.save(sd, out_dir / 'osc_model.pth')
+        if add_chat_template:
+            chat_template = self.get_chat_template()
+            if chat_template:
+                template_config = chat_template.get_config()
+        config = self.osc_config.merge(template_config)
+        config = Config(data=config, section_order=['model', 'chat_template'])
+        config.to_disk(out_dir / 'config.cfg')
+        if self.tokenizer:
+            self.tokenizer.save(out_dir)
+    
+    def convert_pytorch_format(self):
+        sd = {}
+        wmap = self.weight_map
+        index_file = self.checkpoint_dir / 'pytorch_model.bin.index.json'
+        if index_file.exists():
+            with open(index_file, 'r') as f:
+                index = json.load(f)
+            files = [self.checkpoint_dir / file  for file in set(index['weight_map'].values())]
+        else:
+            files = [self.checkpoint_dir / 'pytorch_model.bin']
+        assert len(files) > 0, 'No pytorch model file found'
+        for file in files:
+            weights = torch.load(str(file), map_location='cpu', weights_only=True, mmap=True)
+            for key in weights:
+                if key not in wmap:
+                    msg.warn(f"{key} not in wmap")
+                    continue
+                sd[wmap[key]] = weights[key]
+        return sd
         
-    def forward(self, x: Tensor) -> Tensor:
-        return self.model(x)
+    def convert_safetensor_format(self):
+        sd = {}
+        wmap = self.weight_map
+        index_file = self.checkpoint_dir / 'model.safetensors.index.json'
+        if index_file.exists():
+            with open(index_file, 'r') as f:
+                index = json.load(f)
+            files = [self.checkpoint_dir / file  for file in set(index['weight_map'].values())]
+        else:
+            files = [self.checkpoint_dir / 'model.safetensors']
+        assert len(files) > 0, 'No pytorch model file found'
+        try:
+            from safetensors import safe_open
+        except Exception:
+            raise ImportError("Please install safetensors first, run `pip install safetensors`")
+        for file in files:
+            with safe_open(file, framework='pt') as f:
+                for key in f.keys():
+                    if key not in wmap:
+                        msg.warn(f"{key} not in wmap")
+                        continue
+                    sd[wmap[key]] = f.get_tensor(key)
+        return sd
         
-    def configure_optimizers(self) -> OptimizerLRScheduler:
-        optimizer = torch.optim.Adam(self.parameters(), lr=self.hparams.lr)
-        num_training_steps = self.trainer.estimated_stepping_batches
-        num_warm_up_steps = min(100, num_training_steps // 10)
-        scheduler = get_cosine_lr_scheduler(optimizer, 
-                                            num_training_steps=num_training_steps, 
-                                            num_warm_up_steps=num_warm_up_steps,
-                                            min_lr_ratio=0.01)
-        scheduler_config = {'scheduler': scheduler, 'interval': 'step', 'frequency': 1}
-        return [optimizer], [scheduler_config]
-    
-    def training_step(self, batch: Tuple[Tensor, Tensor], batch_idx: int) -> STEP_OUTPUT:
-        inputs, target = batch
-        logits = self.model(inputs)
-        loss = torch.nn.functional.cross_entropy(logits.view(-1, logits.size(-1)), target.view(-1))
-        self.log('train_loss', loss, on_step=True, prog_bar=True)
-        return loss
-    
-    def train_dataloader(self) -> Any:
-        return DataLoader(self.dataset, batch_size=self.hparams.batch_size, shuffle=True, drop_last=True)
-    
-    def generate(self, 
-                 prompt: str, 
-                 top_k: int = 5, 
-                 max_len: int = 100, 
-                 temperature: float = 1.0):
-        ids = [self.dataset.vocab.token2id[char] for char in prompt]
-        input_pos = torch.arange(len(ids), dtype=torch.long, device=self.device)
-        ids = torch.tensor(ids, dtype=torch.long, device=self.device)
-        self.model.eval()
-        self.model.build_kv_caches(batch_size=1, device=self.device)
-        outputs = []
-        with torch.no_grad():
-            for _ in range(max_len):
-                logits = self.model(ids.reshape(1, -1), input_pos)
-                logits = logits[0, -1] / temperature
-                # 选择概率最大的top_k个token, 其他的token logits设置为负无穷
-                v, _ = torch.topk(logits, min(top_k, logits.size(-1)))
-                logits = torch.where(logits < v[[-1]], -float("Inf"), logits)
-                probs = torch.nn.functional.softmax(logits, dim=-1)
-                ids = torch.multinomial(probs, num_samples=1)
-                if ids[0] == self.dataset.vocab.token2id['</s>']:
-                    break
-                input_pos = input_pos[-1:] + 1
-                outputs.append(self.dataset.vocab.id2token[ids[0].item()])
-        return prompt + "".join(outputs)           
+    def load_checkpoint(self, checkpoint_name: str = 'osc_model.pth', device: str = 'cpu'):
+        model = build_model(config=self.osc_config)
+        model.load_state_dict(torch.load(str(self.checkpoint_dir / checkpoint_name), mmap=True, weights_only=True), assign=True)
+        model.to(device)
+        return model.eval()
+    
+    def get_chat_template(self) -> ChatTemplate:
+        for k, v in registry.chat_templates.get_all().items():
+            if k in self.checkpoint_dir.name: # 简单通过名称匹配
+                return v
+        return None
```

### Comparing `osc_llm-0.1.3/osc_llm/engines/base.py` & `osc_llm-0.1.4/osc_llm/engines/base.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/engines/v1.py` & `osc_llm-0.1.4/osc_llm/engines/v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,30 +23,31 @@
     def load_model(self) -> None:
         config_path = Path(self.checkpoint_dir) / 'config.cfg'
         states_path = Path(self.checkpoint_dir) / 'osc_model.pth'
         
         config = Config().from_disk(config_path)
         assert config['model']['@architectures'] == "TransformerDecoder", "Only TransformerDecoder Architecture is supported"
             
-        with self.fabric.init_module(empty_init=True):
-            self.model = build_model(config=config_path, empty_init=False).eval()
-        
+        self.model = build_model(config=config_path, empty_init=True).eval()
         self.fabric.load_raw(states_path, self.model)
+        self.model = self.fabric.to_device(self.model)
         
         with self.fabric.init_tensor():
             self.model.setup_kv_cache(batch_size=1, max_length=self.max_length, dtype=torch.bfloat16)
             
         
     def compile_model(self) -> None:
         torch._inductor.config.coordinate_descent_tuning = True
         torch._inductor.config.triton.unique_kernel_names = True
         torch._inductor.config.fx_graph_cache = True # Experimental feature to reduce compilation times, will be on by default in future
         torch._inductor.config.triton.cudagraph_trees = False # 目前用作server的时候有bug
         
         torch._dynamo.config.automatic_dynamic_shapes = True
+        torch._dynamo.config.suppress_errors = True
+        torch._dynamo.config.capture_dynamic_output_shape_ops = True
         
         
         self.model: TransformerDecoder = torch.compile(self.model, dynamic=True, fullgraph=True, mode="reduce-overhead")
 
         
     def setup_model(self) -> None:
         self.model = self.fabric.setup_module(self.model)
@@ -66,30 +67,30 @@
         input_ids = self.prefill(input_ids=input_ids.view(1, -1), input_pos=input_pos)
         yield input_ids
         
         # decode
         with self.fabric.init_tensor():
             input_pos = torch.tensor([input_pos[-1].item() + 1])
         max_stop_len = max([len(stop_id) for stop_id in stop_ids])
-        yield_ids = []
-        for i in range(1, max_length - input_pos.item() + 1):
-            with sdpa_kernel(backends=[SDPBackend.MATH]):
+        yield_ids = [] # 用来存储的生成token ids, 直到长度达到stop ids中的最大长度, 然后生成
+        with sdpa_kernel(backends=[SDPBackend.MATH]):
+            for i in range(1, max_length - input_pos.item() + 1):
                 input_ids = input_ids.view(1, -1)
                 next_token_id = self.decode(input_ids=input_ids, input_pos=input_pos)
                 yield_ids.append(next_token_id)
                 # 遍历每一个stop ids
                 for ids in stop_ids:
-                    if len(yield_ids) >= len(ids):
+                    if len(yield_ids) == len(ids):
                         if all(a == b for a, b in zip(yield_ids, ids)):
                             return 
                 if len(yield_ids) >= max_stop_len:
                     yield from yield_ids
                     yield_ids = []
-            input_pos = input_pos.add_(1)
-            input_ids = next_token_id
+                input_pos = input_pos.add_(1)
+                input_ids = next_token_id
         
     def prefill(self, **model_inputs) -> torch.Tensor:
         logits = self.model(**model_inputs)[0, -1]
         idx = self.sampler.sample(logits=logits)
         return idx
     
     def decode(self, **model_inputs) -> torch.Tensor:
```

### Comparing `osc_llm-0.1.3/osc_llm/engines/v2.py` & `osc_llm-0.1.4/osc_llm/engines/v2.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/layers/__init__.py` & `osc_llm-0.1.4/osc_llm/layers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from .normalization import RMSNorm, LayerNorm
 from .attention import CausalSelfAttention
 from .head import LMHead
 from .linear import Linear, WeightOnlyInt4Linear, Int8Linear
 from .embedding import TokenEmbedding, TokenEmbeddingPlus
-from .feedforward import GLU, SwiGLU, MoE, GeGLU
+from .feedforward import GLU, SwiGLU, GeGLU, SparseMoe, SwiGLUV2
 from .activation import ReLU, SiLU, GELU
 from .kv_cache import StaticKVCache
 from .dropout import Dropout
 
 
 __all__ = [
     "RMSNorm",
     "LayerNorm",
     "CausalSelfAttention",
     "LMHead",
     "TokenEmbedding",
     "TokenEmbeddingPlus",
     "GLU",
     "SwiGLU",
-    "MoE",
+    "SwiGLUV2",
     "GeGLU",
     "ReLU",
     "SiLU",
     "GELU",
     "StaticKVCache",
     "Linear",
     "WeightOnlyInt4Linear",
     "Int8Linear",
     "Dropout",
+    "SparseMoe"
 ]
```

### Comparing `osc_llm-0.1.3/osc_llm/layers/activation.py` & `osc_llm-0.1.4/osc_llm/layers/activation.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/layers/attention.py` & `osc_llm-0.1.4/osc_llm/layers/attention.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,26 +32,33 @@
         n_heads: int,
         q_bias: bool = False,
         k_bias: bool = False,
         v_bias: bool = False,
         o_bias: bool = False,
         n_query_groups: Optional[int] = None,
         kv_cache: Optional[KVCache] = None,
+        use_qkv_proj: bool = False,
+        qkv_bias: bool = False
     ):
         super().__init__()
         
         assert n_in % n_heads == 0, f"dim {n_in} must be divisible by n_heads {n_heads}"
         
         self.n_heads = n_heads
         self.head_size = n_in // n_heads
         self.n_query_groups = n_query_groups if n_query_groups else n_heads
         
-        self.q_proj = nn.Linear(n_in, self.n_heads * self.head_size, bias=q_bias)
-        self.k_proj = nn.Linear(n_in, self.n_query_groups * self.head_size, bias=k_bias)
-        self.v_proj = nn.Linear(n_in, self.n_query_groups * self.head_size, bias=v_bias)
+        self.use_qkv_proj = use_qkv_proj
+        if not use_qkv_proj:
+            self.q_proj = nn.Linear(n_in, self.n_heads * self.head_size, bias=q_bias)
+            self.k_proj = nn.Linear(n_in, self.n_query_groups * self.head_size, bias=k_bias)
+            self.v_proj = nn.Linear(n_in, self.n_query_groups * self.head_size, bias=v_bias)
+        else:
+            self.qkv_proj = nn.Linear(n_in, self.n_heads * self.head_size + self.n_query_groups * self.head_size * 2, bias=qkv_bias)
+            
         self.o_proj = nn.Linear(n_in, n_in, bias=o_bias)
         
         self.kv_cache: KVCache = kv_cache
 
 
     def forward(
         self,
@@ -59,18 +66,27 @@
         cos: Optional[torch.Tensor] = None,
         sin: Optional[torch.Tensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
         input_pos: Optional[torch.Tensor] = None
     ):
         
         B, L, D = x.size()  # batch size, sequence length, embedding dimensionality (n_embd)
-
-        q: torch.Tensor = self.q_proj(x).reshape(B, L, self.n_heads, self.head_size).permute(0, 2, 1, 3)
-        k: torch.Tensor = self.k_proj(x).reshape(B, L, self.n_query_groups, self.head_size).permute(0, 2, 1, 3)
-        v: torch.Tensor = self.v_proj(x).reshape(B, L, self.n_query_groups, self.head_size).permute(0, 2, 1, 3)
+        if self.use_qkv_proj:
+            qkv: torch.Tensor = self.qkv_proj(x)
+            q, k, v = qkv.split(
+                [self.n_heads * self.head_size, self.n_query_groups * self.head_size, self.n_query_groups * self.head_size],
+                dim=-1
+            )
+            q = q.reshape(B, L, self.n_heads, self.head_size).permute(0, 2, 1, 3)
+            k = k.reshape(B, L, self.n_query_groups, self.head_size).permute(0, 2, 1, 3)
+            v = v.reshape(B, L, self.n_query_groups, self.head_size).permute(0, 2, 1, 3)
+        else:
+            q: torch.Tensor = self.q_proj(x).reshape(B, L, self.n_heads, self.head_size).permute(0, 2, 1, 3)
+            k: torch.Tensor = self.k_proj(x).reshape(B, L, self.n_query_groups, self.head_size).permute(0, 2, 1, 3)
+            v: torch.Tensor = self.v_proj(x).reshape(B, L, self.n_query_groups, self.head_size).permute(0, 2, 1, 3)
         
         if (cos is not None) and (sin is not None):
             q = apply_rope(q, cos, sin)
             k = apply_rope(k, cos, sin)
             
         if input_pos is not None:
             if not self.kv_cache:
@@ -98,18 +114,18 @@
         scale = 1.0 / math.sqrt(self.head_size)
         y = torch.nn.functional.scaled_dot_product_attention(
             q, k, v, attn_mask=mask, dropout_p=0.0, scale=scale, is_causal=mask is None
         )
         return y.transpose(1, 2)
     
     def setup_kv_cache(self, 
-                     batch_size: int, 
-                     max_seq_length: int, 
-                     device: Optional[torch.device] = None, 
-                     dtype: Optional[torch.dtype] = None) -> None:
+                       batch_size: int, 
+                       max_seq_length: int, 
+                       device: Optional[torch.device] = None, 
+                       dtype: Optional[torch.dtype] = None) -> None:
         n_heads = self.n_query_groups
         k_shape = (batch_size, n_heads, max_seq_length, self.head_size)
         v_shape = (batch_size, n_heads, max_seq_length, self.head_size)
         self.kv_cache.setup(k_shape, v_shape, dtype=dtype, device=device)
 
 
 def apply_rope(x: torch.Tensor, cos: torch.Tensor, sin: torch.Tensor) -> torch.Tensor:
```

### Comparing `osc_llm-0.1.3/osc_llm/layers/embedding.py` & `osc_llm-0.1.4/osc_llm/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/layers/kv_cache.py` & `osc_llm-0.1.4/osc_llm/layers/kv_cache.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/layers/linear.py` & `osc_llm-0.1.4/osc_llm/layers/linear.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/layers/normalization.py` & `osc_llm-0.1.4/osc_llm/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/model_helpers/llama.py` & `osc_llm-0.1.4/osc_llm/model_helpers/llama.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/quantizers/base.py` & `osc_llm-0.1.4/osc_llm/quantizers/base.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/quantizers/int4.py` & `osc_llm-0.1.4/osc_llm/quantizers/int4.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/quantizers/int8.py` & `osc_llm-0.1.4/osc_llm/quantizers/int8.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/samplers/base.py` & `osc_llm-0.1.4/osc_llm/samplers/base.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/samplers/top_k.py` & `osc_llm-0.1.4/osc_llm/samplers/top_k.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/samplers/top_p.py` & `osc_llm-0.1.4/osc_llm/samplers/top_p.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.3/osc_llm/servers/openai.py` & `osc_llm-0.1.4/osc_llm/servers/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from ..engines import LLMEngineV2, LLMEngineV1, LLMEngine
 from ..tokenizer import Tokenizer
 from ..chat_templates import Message
 from ..utils import random_uuid
 from ..samplers import TopK
 from typing import List, Optional, Dict, Union, Literal
-from fastapi import FastAPI
-from fastapi.responses import StreamingResponse, JSONResponse
-import uvicorn
 from pydantic import BaseModel, Field
 import torch
 import time
 
     
 class ErrorResponse(BaseModel):
     object: str = "error"
@@ -117,30 +114,34 @@
     user: Optional[str] = None
     
     
 def main(checkpoint_dir: str,
          engine: Literal['v1', 'v2'] = 'v1',
          accelerator: Literal['cuda', 'cpu', 'gpu', 'auto'] = 'cuda',
          devices: Union[int, List[int]] = 1,
+         max_length: Optional[int] = None,
          host: str = '0.0.0.0',
          port: int = 8000,
          compile: bool = True):
     """openai接口服务
 
     Args:
         checkpoint_dir (str): checkpoint目录
         engine (Literal[&#39;v1&#39;, &#39;v2&#39;], optional): LLMEngine版本. Defaults to 'v1'.
         accelerator (Literal[&#39;cuda&#39;, &#39;cpu&#39;, &#39;gpu&#39;, &#39;auto&#39;], optional): 推理硬件. Defaults to 'cuda'.
         devices (Union[int, List[int]], optional): 设备数量或者设备的ID. Defaults to 1.
         host (str, optional): 主机地址. Defaults to '0.0.0.0'.
         port (int, optional): 端口号. Defaults to 8000.
         compile (bool, optional): 是否编译模型. Defaults to True.
     """
+    from fastapi import FastAPI
+    from fastapi.responses import StreamingResponse, JSONResponse
+    import uvicorn
     
-    app = FastAPI()
+    app = FastAPI(description="OpenAI API")
     
     @app.post("/v1/chat/completions")
     def create_chat_completion(request: ChatCompletionRequest):
         with engine.fabric.init_tensor():
             input_ids = tokenizer.encode_messages(request.messages)
             input_pos = torch.arange(len(input_ids))
         engine.reset_sampler(sampler=TopK(k=100, temperature=request.temperature))
@@ -162,23 +163,23 @@
             completion_tokens = 0
             for token in stream_tokens:
                 content += token
                 completion_tokens += 1
             prompt_tokens = len(input_ids)
             total_tokens = prompt_tokens + completion_tokens
             response = ChatCompletionResponse(id=f"chatcmpl-{random_uuid()}",
-                                                  model=request.model,
-                                                  choices=[ChatCompletionResponseChoice(index=0, message=ChatMessage(role='assistant', content=content))],
-                                                  usage=UsageInfo(prompt_tokens=prompt_tokens, total_tokens=total_tokens, completion_tokens=completion_tokens))
+                                              model=request.model,
+                                              choices=[ChatCompletionResponseChoice(index=0, message=ChatMessage(role='assistant', content=content))],
+                                              usage=UsageInfo(prompt_tokens=prompt_tokens, total_tokens=total_tokens, completion_tokens=completion_tokens))
             return JSONResponse(content=response.model_dump(exclude_unset=True))
     
     if engine == 'v1':
-        engine: LLMEngine = LLMEngineV1(checkpoint_dir, devices=devices, accelerator=accelerator, compile=compile)
+        engine: LLMEngine = LLMEngineV1(checkpoint_dir, devices=devices, accelerator=accelerator, compile=compile, max_length=max_length)
     else:
-        engine: LLMEngine = LLMEngineV2(checkpoint_dir, devices=devices, accelerator=accelerator, compile=compile)
+        engine: LLMEngine = LLMEngineV2(checkpoint_dir, devices=devices, accelerator=accelerator, compile=compile, max_length=max_length)
     engine.setup()
     tokenizer = Tokenizer(checkpoint_dir=checkpoint_dir)
     
     # Todo: 在启动模型编译的情况下第一次运行需要耗费很多时间(几分钟),如何在启动的时候预热模型?
     if compile:
         from wasabi import msg
         msg.warn("you are using compile mode, the first run may take a long time")
```

### Comparing `osc_llm-0.1.3/osc_llm/tokenizer.py` & `osc_llm-0.1.4/osc_llm/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 from pathlib import Path
 from typing import Optional, Union, Generator, List
 import torch
 from .chat_templates import ChatTemplate, Message
+from sentencepiece import SentencePieceProcessor
+from tokenizers import Tokenizer as HFTokenizer
 
 
 class Tokenizer:
     def __init__(self, 
                  checkpoint_dir: Union[Path, str],
                  chat_template: Optional[ChatTemplate] = None,
                  ) -> None:
@@ -19,25 +21,23 @@
         self.bos_id = None
         self.eos_id = None
         
         self.chat_template = chat_template if chat_template else ChatTemplate.from_checkpoint(checkpoint_dir)
 
         # some checkpoints have both files, `.model` takes precedence
         if (vocabulary_path := checkpoint_dir / "tokenizer.model").is_file():
-            from sentencepiece import SentencePieceProcessor
             self.tokenizer_path = checkpoint_dir / "tokenizer.model"
-            self.processor = SentencePieceProcessor(model_file=str(vocabulary_path))
+            self.processor: SentencePieceProcessor = SentencePieceProcessor(model_file=str(vocabulary_path))
             self.backend = "sentencepiece"
             self.bos_id = self.processor.bos_id()
             self.eos_id = self.processor.eos_id()
 
         elif (vocabulary_path := checkpoint_dir / "tokenizer.json").is_file():
-            from tokenizers import Tokenizer as HFTokenizer
             self.tokenizer_path = checkpoint_dir / "tokenizer.json"
-            self.processor = HFTokenizer.from_file(str(vocabulary_path))
+            self.processor: HFTokenizer = HFTokenizer.from_file(str(vocabulary_path))
             self.backend = "huggingface"
 
             if (special_tokens_path := checkpoint_dir / "tokenizer_config.json").is_file():
                 self.tokenizer_config_path = checkpoint_dir / "tokenizer_config.json"
                 with open(special_tokens_path) as fp:
                     config = json.load(fp)
                 bos_token = config.get("bos_token")
@@ -90,16 +90,18 @@
         string: str,
         device: Optional[torch.device] = None,
         bos: Optional[bool] = None,
         eos: bool = False,
         max_length: int = -1,
     ) -> torch.Tensor:
         if self.backend == "huggingface":
-            tokens = self.processor.encode(string).ids
+            self.processor: HFTokenizer
+            tokens = self.processor.encode(string, add_special_tokens=False).ids
         elif self.backend == "sentencepiece":
+            self.processor: SentencePieceProcessor
             tokens = self.processor.encode(string)
         else:
             raise RuntimeError
         if bos or (bos is None and self.use_bos):
             bos_id = self.bos_id
             if bos_id is None:
                 raise NotImplementedError("This tokenizer does not have a defined a bos token")
@@ -176,17 +178,17 @@
             shutil.copyfile(self.tokenizer_config_path, save_dir / self.tokenizer_config_path.name)
             shutil.copyfile(self.generation_config_path, save_dir / self.generation_config_path.name)
         if self.backend == "sentencepiece":
             shutil.copyfile(self.tokenizer_path, save_dir / self.tokenizer_path.name)
             
     @property
     def stop_ids(self) -> List[List[int]]:
-        stop_ids = [[torch.tensor([self.eos_id], dtype=torch.int)]]
+        stop_ids = [torch.tensor([self.eos_id], dtype=torch.int)]
         if self.chat_template:
-            stop_ids.extend([[self.encode(text)] for text in self.chat_template.stop_texts])
+            stop_ids.extend([self.encode(text) for text in self.chat_template.stop_texts])
         return stop_ids
     
     def has_special_chars(self, text: str) -> bool:
         """使用sentencepiece时，检查文本中是否包含特殊字符�.这种情况通常是由于一个中文字符被分割为几个token,而解码时没有合并回去导致的.
         """
         return '�' in text
```

### Comparing `osc_llm-0.1.3/osc_llm/utils.py` & `osc_llm-0.1.4/osc_llm/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -144,8 +144,27 @@
 
     if MPSAccelerator.is_available() or (torch.cuda.is_available() and not torch.cuda.is_bf16_supported()):
         return "16-mixed" if training else "16-true"
     return "bf16-mixed" if training else "bf16-true"
 
 
 def random_uuid() -> str:
-    return str(uuid.uuid4().hex)
+    return str(uuid.uuid4().hex)
+
+def get_model_size(model: torch.nn.Module, contains_embedding: bool = False) -> int:
+    """Get the size of a model in bytes.
+
+    Args:
+        model (torch.nn.Module): the model to get the size of.
+        contains_embedding (bool, optional): whether the model contains an embedding layer. Defaults to False.
+
+    Returns:
+        int: the size of the model in bytes.
+    """
+    size = 0
+    for param in model.parameters():
+        size += param.numel() * param.element_size()
+    if contains_embedding:
+        for name, module in model.named_modules():
+            if isinstance(module, torch.nn.Embedding):
+                size += module.num_embeddings * module.embedding_dim * module.weight.element_size()
+    return size
```

