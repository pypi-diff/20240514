# Comparing `tmp/transformers-re-1.1.2.tar.gz` & `tmp/transformers-re-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\desktop\program\python\wheel\transformers-re\dist\.tmp-w4wc_fq6\transformers-re-1.1.2.tar", last modified: Wed Feb 28 15:33:20 2024, max compression
+gzip compressed data, was "D:\desktop\program\python\wheel\transformers-re\dist\.tmp-sq8rcwul\transformers-re-1.1.3.tar", last modified: Tue May 14 13:49:00 2024, max compression
```

## Comparing `transformers-re-1.1.2.tar` & `transformers-re-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 15:33:20.000000 transformers-re-1.1.2/
--rw-rw-rw-   0        0        0    11558 2024-02-28 15:31:52.000000 transformers-re-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     8323 2024-02-28 15:33:20.000000 transformers-re-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     7863 2024-02-13 12:49:13.000000 transformers-re-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-02-28 15:33:20.000000 transformers-re-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      873 2024-02-28 15:30:49.000000 transformers-re-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-28 15:33:20.000000 transformers-re-1.1.2/transformers_re.egg-info/
--rw-rw-rw-   0        0        0     8323 2024-02-28 15:33:20.000000 transformers-re-1.1.2/transformers_re.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-02-28 15:33:20.000000 transformers-re-1.1.2/transformers_re.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 15:33:20.000000 transformers-re-1.1.2/transformers_re.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-02-28 15:33:20.000000 transformers-re-1.1.2/transformers_re.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-02-28 15:33:20.000000 transformers-re-1.1.2/transformers_re.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13822 2024-02-13 01:55:24.000000 transformers-re-1.1.2/transformers_re.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:49:00.000000 transformers-re-1.1.3/
+-rw-rw-rw-   0        0        0    11558 2024-02-28 15:31:52.000000 transformers-re-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     8463 2024-05-14 13:49:00.000000 transformers-re-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8003 2024-05-14 13:46:49.000000 transformers-re-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 13:49:00.000000 transformers-re-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      873 2024-05-14 13:46:49.000000 transformers-re-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:49:00.000000 transformers-re-1.1.3/transformers_re.egg-info/
+-rw-rw-rw-   0        0        0     8463 2024-05-14 13:49:00.000000 transformers-re-1.1.3/transformers_re.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-05-14 13:49:00.000000 transformers-re-1.1.3/transformers_re.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 13:49:00.000000 transformers-re-1.1.3/transformers_re.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-14 13:49:00.000000 transformers-re-1.1.3/transformers_re.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-14 13:49:00.000000 transformers-re-1.1.3/transformers_re.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14437 2024-05-14 13:25:11.000000 transformers-re-1.1.3/transformers_re.py
```

### Comparing `transformers-re-1.1.2/LICENSE` & `transformers-re-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `transformers-re-1.1.2/PKG-INFO` & `transformers-re-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-re
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Regular Expression constraint for Language Models of transformers. With this module, you can force the LLMs to generate following your regex. Using regex in tokens and tensors are also implemented in this project.
 Home-page: https://github.com/kuangkzh/transformers-re
 Author: kuangzh
 Author-email: 1432245553@qq.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -30,14 +30,15 @@
 - prompt: the prompt input into model.
 - pattern: regex pattern.
 - num_proc: the number of processors to process regex match.
 - fail_strategy: default: 'eos'. The strategy when no token can use. It can be:
     - List[int]: token ids when no token can use.
     - 'eos': automatically choose the tokenizer.eos_token_id
 - debug: default: False. Control the debug information output.
+- guess_token: default: False. Try to guess the next token to accelerate generating. Guessing a wrong token will slow down the generation.
 
 
 **Attributes**:
 - generated_text(str): Cached text. Generation can be restored from it to prevent running error of regex mismatch
 - match(regex.Match): The Match object of generated text and pattern
 
 **Usage example**:
```

### Comparing `transformers-re-1.1.2/README.md` & `transformers-re-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 - prompt: the prompt input into model.
 - pattern: regex pattern.
 - num_proc: the number of processors to process regex match.
 - fail_strategy: default: 'eos'. The strategy when no token can use. It can be:
     - List[int]: token ids when no token can use.
     - 'eos': automatically choose the tokenizer.eos_token_id
 - debug: default: False. Control the debug information output.
+- guess_token: default: False. Try to guess the next token to accelerate generating. Guessing a wrong token will slow down the generation.
 
 
 **Attributes**:
 - generated_text(str): Cached text. Generation can be restored from it to prevent running error of regex mismatch
 - match(regex.Match): The Match object of generated text and pattern
 
 **Usage example**:
```

### Comparing `transformers-re-1.1.2/setup.py` & `transformers-re-1.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='transformers-re',
-    version='1.1.2',
+    version='1.1.3',
     author='kuangzh',
     author_email='1432245553@qq.com',
     url='https://github.com/kuangkzh/transformers-re',
     description='A Regular Expression constraint for Language Models of transformers. With this module, you can force '
                 'the LLMs to generate following your regex. Using regex in tokens and tensors are also implemented in '
                 'this project.',
     long_description=long_description,
```

### Comparing `transformers-re-1.1.2/transformers_re.egg-info/PKG-INFO` & `transformers-re-1.1.3/transformers_re.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-re
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Regular Expression constraint for Language Models of transformers. With this module, you can force the LLMs to generate following your regex. Using regex in tokens and tensors are also implemented in this project.
 Home-page: https://github.com/kuangkzh/transformers-re
 Author: kuangzh
 Author-email: 1432245553@qq.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -30,14 +30,15 @@
 - prompt: the prompt input into model.
 - pattern: regex pattern.
 - num_proc: the number of processors to process regex match.
 - fail_strategy: default: 'eos'. The strategy when no token can use. It can be:
     - List[int]: token ids when no token can use.
     - 'eos': automatically choose the tokenizer.eos_token_id
 - debug: default: False. Control the debug information output.
+- guess_token: default: False. Try to guess the next token to accelerate generating. Guessing a wrong token will slow down the generation.
 
 
 **Attributes**:
 - generated_text(str): Cached text. Generation can be restored from it to prevent running error of regex mismatch
 - match(regex.Match): The Match object of generated text and pattern
 
 **Usage example**:
```

### Comparing `transformers-re-1.1.2/transformers_re.py` & `transformers-re-1.1.3/transformers_re.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,24 +88,26 @@
     Usage example:
     >>> with RegexLogitsProcessor(tokenizer, prompt, pattern) as regex_logits_processor:
     >>>   model.generate(logits_processor=[regex_logits_processor])
     Attributes:
         generated_text(str): Cached text. Generation can be restored from it to prevent running error of regex mismatch
         match(regex.Match): The Match object of generated text and pattern
     """
-    def __init__(self, tokenizer, prompt, pattern, num_proc=1, fail_strategy='eos', debug=False):
+    def __init__(self, tokenizer, prompt, pattern, num_proc=1, fail_strategy='eos', debug=False, guess_token=False):
         """
         :param tokenizer: transformers.Tokenizer
         :param prompt: the prompt input into model.
         :param pattern: regex pattern.
         :param num_proc: the number of processors to process regex match.
         :param fail_strategy: default: 'eos'. The strategy when no token can use. It can be:
                             - List[int]: token ids when no token can use.
                             - 'eos': automatically choose the tokenizer.eos_token_id
         :param debug: default: False. Control the debug information output.
+        :param guess_token: default: False. Try to guess the next token to accelerate generating.
+                            Guessing a wrong token will slow down the generation.
         """
         self.tokenizer = tokenizer
         self.pattern = regex.compile(pattern)
         self.prompt_token_len = len(tokenizer(prompt)['input_ids'])
         self.fail_strategy = [tokenizer.eos_token_id] if fail_strategy == 'eos' else fail_strategy
         self.debug = debug
         vocab = [(idx, tokenizer.decode(idx)) for _, idx in tokenizer.get_vocab().items()]
@@ -124,14 +126,16 @@
 
             return _regex_match
 
         self.process_list = [multiprocess.Process(target=regex_service(i), daemon=True) for i in range(num_proc)]
 
         self.generated_text = ""
         self.match = None
+        self.is_guess = guess_token
+        self.guess_token = None
 
     def __enter__(self):
         [proc.start() for proc in self.process_list]
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         [proc.kill() for proc in self.process_list]
@@ -144,21 +148,27 @@
                           "Set debug=True to track the generation process. \n"
                           "You can restore your text from RegexPrefixProcessor.generated_text.")
 
     def __call__(self, input_ids, scores):
         assert len(input_ids) == 1, "Only generation for batchsize 1 is surpported"
         self.generated_text = self.tokenizer.decode(input_ids[0, self.prompt_token_len:])
 
-        [q.put(self.generated_text) for q in self.q_in]
-        self.match = self.pattern.match(self.generated_text, partial=True)
-        candidates = sum([q.get() for q in self.q_out], [])
+        candidates = None if self.guess_token is None else sum([q.get() for q in self.q_out], [])
+        if input_ids[0, -1] != self.guess_token:
+            [q.put(self.generated_text) for q in self.q_in]
+            self.match = self.pattern.match(self.generated_text, partial=True)
+            candidates = sum([q.get() for q in self.q_out], [])
         candidates = candidates if candidates else self.fail_strategy
         mask = torch.zeros_like(scores).scatter(1, torch.LongTensor([candidates]).to(scores.device), 1).bool()
         scores = scores.where(mask, -torch.inf * torch.ones_like(scores))
 
+        if self.is_guess:
+            self.guess_token = scores[0].argmax()
+            [q.put(self.generated_text + self.tokenizer.decode(self.guess_token)) for q in self.q_in]
+
         if self.debug:
             candidates_repr = (f"{len(candidates)} tokens" if len(candidates) > 10 else candidates)
             print(f"generated:{self.generated_text} candidates:{candidates_repr}")
         return scores
 
 
 def get_token_mapping(tokenizer, s):
```

