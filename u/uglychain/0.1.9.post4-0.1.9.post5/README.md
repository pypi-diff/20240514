# Comparing `tmp/uglychain-0.1.9.post4.tar.gz` & `tmp/uglychain-0.1.9.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uglychain-0.1.9.post4.tar", max compression
+gzip compressed data, was "uglychain-0.1.9.post5.tar", max compression
```

## Comparing `uglychain-0.1.9.post4.tar` & `uglychain-0.1.9.post5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     1063 2024-01-26 22:51:45.177208 uglychain-0.1.9.post4/LICENSE
--rw-r--r--   0        0        0     7215 2024-01-31 10:20:29.287357 uglychain-0.1.9.post4/README.md
--rw-r--r--   0        0        0     2229 2024-02-28 05:00:53.545982 uglychain-0.1.9.post4/pyproject.toml
--rw-r--r--   0        0        0      475 2024-02-27 14:11:51.720784 uglychain-0.1.9.post4/uglychain/__init__.py
--rw-r--r--   0        0        0      229 2024-02-27 14:11:51.720784 uglychain-0.1.9.post4/uglychain/chains/__init__.py
--rw-r--r--   0        0        0     3086 2024-02-23 13:54:05.770895 uglychain-0.1.9.post4/uglychain/chains/base.py
--rw-r--r--   0        0        0      190 2024-02-08 01:18:36.545320 uglychain-0.1.9.post4/uglychain/chains/llm/__init__.py
--rw-r--r--   0        0        0     7085 2024-02-28 04:36:25.222036 uglychain-0.1.9.post4/uglychain/chains/llm/llm.py
--rw-r--r--   0        0        0     1115 2024-02-06 10:14:47.450355 uglychain-0.1.9.post4/uglychain/chains/llm/prompt.py
--rw-r--r--   0        0        0     5149 2024-02-28 04:40:16.190028 uglychain-0.1.9.post4/uglychain/chains/map.py
--rw-r--r--   0        0        0     3959 2024-02-18 21:59:52.832616 uglychain-0.1.9.post4/uglychain/chains/react.py
--rw-r--r--   0        0        0     7128 2024-02-23 13:54:05.770895 uglychain-0.1.9.post4/uglychain/chains/react_bad.py
--rw-r--r--   0        0        0     2634 2024-02-06 10:13:41.978357 uglychain-0.1.9.post4/uglychain/chains/reduce.py
--rw-r--r--   0        0        0      302 2024-02-27 14:11:51.720784 uglychain-0.1.9.post4/uglychain/llm/__init__.py
--rw-r--r--   0        0        0     9900 2024-02-25 23:55:56.908422 uglychain-0.1.9.post4/uglychain/llm/base.py
--rw-r--r--   0        0        0      206 2024-02-20 10:11:23.505455 uglychain-0.1.9.post4/uglychain/llm/instructor/__init__.py
--rw-r--r--   0        0        0       38 2024-02-20 10:11:23.505455 uglychain-0.1.9.post4/uglychain/llm/instructor/errors.py
--rw-r--r--   0        0        0     2294 2024-02-20 10:11:23.505455 uglychain-0.1.9.post4/uglychain/llm/instructor/json.py
--rw-r--r--   0        0        0     2394 2024-02-20 10:11:23.505455 uglychain-0.1.9.post4/uglychain/llm/instructor/yaml.py
--rw-r--r--   0        0        0     1737 2024-02-27 14:11:51.720784 uglychain-0.1.9.post4/uglychain/llm/llama_index.py
--rw-r--r--   0        0        0       70 2024-02-27 14:11:51.724784 uglychain-0.1.9.post4/uglychain/llm/provider/__init__.py
--rw-r--r--   0        0        0      497 2024-02-27 14:11:51.724784 uglychain-0.1.9.post4/uglychain/llm/provider/baichuan.py
--rw-r--r--   0        0        0     4538 2024-02-27 14:11:51.724784 uglychain-0.1.9.post4/uglychain/llm/provider/chatgpt.py
--rw-r--r--   0        0        0      304 2024-02-27 14:11:51.724784 uglychain-0.1.9.post4/uglychain/llm/provider/copilot.py
--rw-r--r--   0        0        0      317 2024-02-27 14:11:51.724784 uglychain-0.1.9.post4/uglychain/llm/provider/custom.py
--rw-r--r--   0        0        0     4579 2024-02-27 14:11:51.724784 uglychain-0.1.9.post4/uglychain/llm/provider/dashscope.py
--rw-r--r--   0        0        0      264 2024-02-27 14:11:51.724784 uglychain-0.1.9.post4/uglychain/llm/provider/error.py
--rw-r--r--   0        0        0     2786 2024-02-27 14:11:51.728784 uglychain-0.1.9.post4/uglychain/llm/provider/gemini.py
--rw-r--r--   0        0        0     2411 2024-02-27 14:11:51.728784 uglychain-0.1.9.post4/uglychain/llm/provider/model.py
--rw-r--r--   0        0        0     2211 2024-02-27 14:11:51.728784 uglychain-0.1.9.post4/uglychain/llm/provider/ollama.py
--rw-r--r--   0        0        0     2460 2024-02-27 14:11:51.728784 uglychain-0.1.9.post4/uglychain/llm/provider/openai_api.py
--rw-r--r--   0        0        0     4352 2024-02-27 14:11:51.728784 uglychain-0.1.9.post4/uglychain/llm/provider/sparkapi.py
--rw-r--r--   0        0        0     2107 2024-02-27 14:11:51.728784 uglychain-0.1.9.post4/uglychain/llm/provider/yi.py
--rw-r--r--   0        0        0     4109 2024-02-27 14:11:51.732784 uglychain-0.1.9.post4/uglychain/llm/provider/zhipu.py
--rw-r--r--   0        0        0     5744 2024-02-20 10:11:23.505455 uglychain-0.1.9.post4/uglychain/llm/tools.py
--rw-r--r--   0        0        0      141 2024-02-18 07:37:49.340108 uglychain-0.1.9.post4/uglychain/retrievers/__init__.py
--rw-r--r--   0        0        0     2177 2024-02-18 07:37:49.340108 uglychain-0.1.9.post4/uglychain/retrievers/arxiv.py
--rw-r--r--   0        0        0     1779 2024-02-18 07:37:49.340108 uglychain-0.1.9.post4/uglychain/retrievers/base.py
--rw-r--r--   0        0        0     2165 2024-02-23 13:54:05.770895 uglychain-0.1.9.post4/uglychain/retrievers/bing.py
--rw-r--r--   0        0        0     4673 2024-02-27 14:11:51.732784 uglychain-0.1.9.post4/uglychain/retrievers/bm25.py
--rw-r--r--   0        0        0     1630 2024-02-27 14:11:51.732784 uglychain-0.1.9.post4/uglychain/retrievers/combine.py
--rw-r--r--   0        0        0      357 2024-02-18 07:37:49.340108 uglychain-0.1.9.post4/uglychain/retrievers/custom.py
--rw-r--r--   0        0        0     2750 2024-02-18 07:37:49.340108 uglychain-0.1.9.post4/uglychain/retrievers/llama_index.py
--rw-r--r--   0        0        0     1182 2024-02-27 14:11:51.732784 uglychain-0.1.9.post4/uglychain/retrievers/model.py
--rw-r--r--   0        0        0     1605 2024-02-18 07:37:49.344108 uglychain-0.1.9.post4/uglychain/retrievers/retrieve_with_llm.py
--rw-r--r--   0        0        0      254 2024-02-20 10:11:23.505455 uglychain-0.1.9.post4/uglychain/storage/__init__.py
--rw-r--r--   0        0        0      276 2024-02-18 07:37:49.344108 uglychain-0.1.9.post4/uglychain/storage/base.py
--rw-r--r--   0        0        0      466 2024-02-18 07:37:49.344108 uglychain-0.1.9.post4/uglychain/storage/dill.py
--rw-r--r--   0        0        0     1113 2024-02-20 10:11:23.505455 uglychain-0.1.9.post4/uglychain/storage/file.py
--rw-r--r--   0        0        0     1032 2024-02-18 07:37:49.344108 uglychain-0.1.9.post4/uglychain/storage/llama_index.py
--rw-r--r--   0        0        0     1983 2024-02-23 13:54:05.770895 uglychain-0.1.9.post4/uglychain/storage/sqlite.py
--rw-r--r--   0        0        0      202 2024-02-14 10:25:47.181706 uglychain-0.1.9.post4/uglychain/tools/__init__.py
--rw-r--r--   0        0        0     1724 2024-02-18 07:37:49.344108 uglychain-0.1.9.post4/uglychain/tools/code_runner.py
--rw-r--r--   0        0        0     1812 2024-02-02 05:30:44.719220 uglychain-0.1.9.post4/uglychain/tools/languages/applescript.py
--rw-r--r--   0        0        0      883 2024-02-02 04:54:16.891306 uglychain-0.1.9.post4/uglychain/tools/languages/base.py
--rw-r--r--   0        0        0    12732 2024-02-18 07:37:49.344108 uglychain-0.1.9.post4/uglychain/tools/languages/ipython.py
--rw-r--r--   0        0        0     1924 2024-02-02 05:01:01.963290 uglychain-0.1.9.post4/uglychain/tools/languages/javascript.py
--rw-r--r--   0        0        0     2183 2024-02-02 05:00:03.843292 uglychain-0.1.9.post4/uglychain/tools/languages/powershell.py
--rw-r--r--   0        0        0     1454 2024-02-18 07:37:49.344108 uglychain-0.1.9.post4/uglychain/tools/languages/python.py
--rw-r--r--   0        0        0     2316 2024-02-04 01:03:36.202888 uglychain-0.1.9.post4/uglychain/tools/languages/r.py
--rw-r--r--   0        0        0     2727 2024-02-02 04:58:54.083295 uglychain-0.1.9.post4/uglychain/tools/languages/shell.py
--rw-r--r--   0        0        0     6290 2024-02-15 01:03:03.044612 uglychain-0.1.9.post4/uglychain/tools/languages/subprocess_language.py
--rw-r--r--   0        0        0      388 2024-02-18 07:37:49.344108 uglychain-0.1.9.post4/uglychain/tools/search.py
--rw-r--r--   0        0        0      270 2024-02-06 03:06:22.453705 uglychain-0.1.9.post4/uglychain/tools/text_completion.py
--rw-r--r--   0        0        0      236 2024-02-27 14:11:51.732784 uglychain-0.1.9.post4/uglychain/utils/__init__.py
--rw-r--r--   0        0        0     1913 2024-02-27 14:11:51.732784 uglychain-0.1.9.post4/uglychain/utils/config.py
--rw-r--r--   0        0        0      487 2024-02-27 14:11:51.732784 uglychain-0.1.9.post4/uglychain/utils/enum.py
--rw-r--r--   0        0        0     1683 2024-02-06 10:11:26.118363 uglychain-0.1.9.post4/uglychain/utils/nlp.py
--rw-r--r--   0        0        0      681 2024-01-30 01:09:40.967697 uglychain-0.1.9.post4/uglychain/utils/retry_decorator.py
--rw-r--r--   0        0        0      850 2024-02-23 13:54:05.770895 uglychain-0.1.9.post4/uglychain/utils/singleton.py
--rw-r--r--   0        0        0    18911 2024-01-30 01:22:48.943666 uglychain-0.1.9.post4/uglychain/utils/stop_words.py
--rw-r--r--   0        0        0      273 2024-02-08 01:18:36.553320 uglychain-0.1.9.post4/uglychain/worker/__init__.py
--rw-r--r--   0        0        0     1805 2024-02-18 07:37:49.344108 uglychain-0.1.9.post4/uglychain/worker/base.py
--rw-r--r--   0        0        0     1609 2024-02-04 11:35:32.877749 uglychain-0.1.9.post4/uglychain/worker/classify.py
--rw-r--r--   0        0        0     4199 2024-02-14 10:32:33.849690 uglychain-0.1.9.post4/uglychain/worker/code_interpreter.py
--rw-r--r--   0        0        0     5966 2024-02-06 03:08:17.985702 uglychain-0.1.9.post4/uglychain/worker/planner.py
--rw-r--r--   0        0        0     2877 2024-02-04 11:11:01.857793 uglychain-0.1.9.post4/uglychain/worker/summary.py
--rw-r--r--   0        0        0     1085 2024-02-03 11:33:49.057316 uglychain-0.1.9.post4/uglychain/worker/transformer.py
--rw-r--r--   0        0        0     9237 1970-01-01 00:00:00.000000 uglychain-0.1.9.post4/setup.py
--rw-r--r--   0        0        0     9335 1970-01-01 00:00:00.000000 uglychain-0.1.9.post4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-01-26 22:51:45.177208 uglychain-0.1.9.post5/LICENSE
+-rw-r--r--   0        0        0     7215 2024-01-31 10:20:29.287357 uglychain-0.1.9.post5/README.md
+-rw-r--r--   0        0        0     2229 2024-02-28 05:37:38.205899 uglychain-0.1.9.post5/pyproject.toml
+-rw-r--r--   0        0        0      475 2024-02-27 14:11:51.720784 uglychain-0.1.9.post5/uglychain/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-27 14:11:51.720784 uglychain-0.1.9.post5/uglychain/chains/__init__.py
+-rw-r--r--   0        0        0     3086 2024-02-23 13:54:05.770895 uglychain-0.1.9.post5/uglychain/chains/base.py
+-rw-r--r--   0        0        0      190 2024-02-08 01:18:36.545320 uglychain-0.1.9.post5/uglychain/chains/llm/__init__.py
+-rw-r--r--   0        0        0     7085 2024-02-28 05:37:12.597900 uglychain-0.1.9.post5/uglychain/chains/llm/llm.py
+-rw-r--r--   0        0        0     1115 2024-02-06 10:14:47.450355 uglychain-0.1.9.post5/uglychain/chains/llm/prompt.py
+-rw-r--r--   0        0        0     5149 2024-02-28 04:40:16.190028 uglychain-0.1.9.post5/uglychain/chains/map.py
+-rw-r--r--   0        0        0     3959 2024-02-18 21:59:52.832616 uglychain-0.1.9.post5/uglychain/chains/react.py
+-rw-r--r--   0        0        0     7128 2024-02-23 13:54:05.770895 uglychain-0.1.9.post5/uglychain/chains/react_bad.py
+-rw-r--r--   0        0        0     2634 2024-02-06 10:13:41.978357 uglychain-0.1.9.post5/uglychain/chains/reduce.py
+-rw-r--r--   0        0        0      302 2024-02-27 14:11:51.720784 uglychain-0.1.9.post5/uglychain/llm/__init__.py
+-rw-r--r--   0        0        0     9900 2024-02-25 23:55:56.908422 uglychain-0.1.9.post5/uglychain/llm/base.py
+-rw-r--r--   0        0        0      206 2024-02-20 10:11:23.505455 uglychain-0.1.9.post5/uglychain/llm/instructor/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-20 10:11:23.505455 uglychain-0.1.9.post5/uglychain/llm/instructor/errors.py
+-rw-r--r--   0        0        0     2294 2024-02-20 10:11:23.505455 uglychain-0.1.9.post5/uglychain/llm/instructor/json.py
+-rw-r--r--   0        0        0     2394 2024-02-20 10:11:23.505455 uglychain-0.1.9.post5/uglychain/llm/instructor/yaml.py
+-rw-r--r--   0        0        0     1737 2024-02-27 14:11:51.720784 uglychain-0.1.9.post5/uglychain/llm/llama_index.py
+-rw-r--r--   0        0        0       70 2024-02-27 14:11:51.724784 uglychain-0.1.9.post5/uglychain/llm/provider/__init__.py
+-rw-r--r--   0        0        0      497 2024-02-27 14:11:51.724784 uglychain-0.1.9.post5/uglychain/llm/provider/baichuan.py
+-rw-r--r--   0        0        0     4538 2024-02-27 14:11:51.724784 uglychain-0.1.9.post5/uglychain/llm/provider/chatgpt.py
+-rw-r--r--   0        0        0      304 2024-02-27 14:11:51.724784 uglychain-0.1.9.post5/uglychain/llm/provider/copilot.py
+-rw-r--r--   0        0        0      317 2024-02-27 14:11:51.724784 uglychain-0.1.9.post5/uglychain/llm/provider/custom.py
+-rw-r--r--   0        0        0     4579 2024-02-27 14:11:51.724784 uglychain-0.1.9.post5/uglychain/llm/provider/dashscope.py
+-rw-r--r--   0        0        0      264 2024-02-27 14:11:51.724784 uglychain-0.1.9.post5/uglychain/llm/provider/error.py
+-rw-r--r--   0        0        0     2786 2024-02-27 14:11:51.728784 uglychain-0.1.9.post5/uglychain/llm/provider/gemini.py
+-rw-r--r--   0        0        0     2411 2024-02-27 14:11:51.728784 uglychain-0.1.9.post5/uglychain/llm/provider/model.py
+-rw-r--r--   0        0        0     2211 2024-02-27 14:11:51.728784 uglychain-0.1.9.post5/uglychain/llm/provider/ollama.py
+-rw-r--r--   0        0        0     2460 2024-02-27 14:11:51.728784 uglychain-0.1.9.post5/uglychain/llm/provider/openai_api.py
+-rw-r--r--   0        0        0     4352 2024-02-27 14:11:51.728784 uglychain-0.1.9.post5/uglychain/llm/provider/sparkapi.py
+-rw-r--r--   0        0        0     2107 2024-02-27 14:11:51.728784 uglychain-0.1.9.post5/uglychain/llm/provider/yi.py
+-rw-r--r--   0        0        0     4109 2024-02-27 14:11:51.732784 uglychain-0.1.9.post5/uglychain/llm/provider/zhipu.py
+-rw-r--r--   0        0        0     5744 2024-02-20 10:11:23.505455 uglychain-0.1.9.post5/uglychain/llm/tools.py
+-rw-r--r--   0        0        0      141 2024-02-18 07:37:49.340108 uglychain-0.1.9.post5/uglychain/retrievers/__init__.py
+-rw-r--r--   0        0        0     2177 2024-02-18 07:37:49.340108 uglychain-0.1.9.post5/uglychain/retrievers/arxiv.py
+-rw-r--r--   0        0        0     1779 2024-02-18 07:37:49.340108 uglychain-0.1.9.post5/uglychain/retrievers/base.py
+-rw-r--r--   0        0        0     2165 2024-02-23 13:54:05.770895 uglychain-0.1.9.post5/uglychain/retrievers/bing.py
+-rw-r--r--   0        0        0     4673 2024-02-27 14:11:51.732784 uglychain-0.1.9.post5/uglychain/retrievers/bm25.py
+-rw-r--r--   0        0        0     1630 2024-02-27 14:11:51.732784 uglychain-0.1.9.post5/uglychain/retrievers/combine.py
+-rw-r--r--   0        0        0      357 2024-02-18 07:37:49.340108 uglychain-0.1.9.post5/uglychain/retrievers/custom.py
+-rw-r--r--   0        0        0     2750 2024-02-18 07:37:49.340108 uglychain-0.1.9.post5/uglychain/retrievers/llama_index.py
+-rw-r--r--   0        0        0     1182 2024-02-27 14:11:51.732784 uglychain-0.1.9.post5/uglychain/retrievers/model.py
+-rw-r--r--   0        0        0     1605 2024-02-18 07:37:49.344108 uglychain-0.1.9.post5/uglychain/retrievers/retrieve_with_llm.py
+-rw-r--r--   0        0        0      254 2024-02-20 10:11:23.505455 uglychain-0.1.9.post5/uglychain/storage/__init__.py
+-rw-r--r--   0        0        0      276 2024-02-18 07:37:49.344108 uglychain-0.1.9.post5/uglychain/storage/base.py
+-rw-r--r--   0        0        0      466 2024-02-18 07:37:49.344108 uglychain-0.1.9.post5/uglychain/storage/dill.py
+-rw-r--r--   0        0        0     1113 2024-02-20 10:11:23.505455 uglychain-0.1.9.post5/uglychain/storage/file.py
+-rw-r--r--   0        0        0     1032 2024-02-18 07:37:49.344108 uglychain-0.1.9.post5/uglychain/storage/llama_index.py
+-rw-r--r--   0        0        0     1983 2024-02-23 13:54:05.770895 uglychain-0.1.9.post5/uglychain/storage/sqlite.py
+-rw-r--r--   0        0        0      202 2024-02-14 10:25:47.181706 uglychain-0.1.9.post5/uglychain/tools/__init__.py
+-rw-r--r--   0        0        0     1724 2024-02-18 07:37:49.344108 uglychain-0.1.9.post5/uglychain/tools/code_runner.py
+-rw-r--r--   0        0        0     1812 2024-02-02 05:30:44.719220 uglychain-0.1.9.post5/uglychain/tools/languages/applescript.py
+-rw-r--r--   0        0        0      883 2024-02-02 04:54:16.891306 uglychain-0.1.9.post5/uglychain/tools/languages/base.py
+-rw-r--r--   0        0        0    12732 2024-02-18 07:37:49.344108 uglychain-0.1.9.post5/uglychain/tools/languages/ipython.py
+-rw-r--r--   0        0        0     1924 2024-02-02 05:01:01.963290 uglychain-0.1.9.post5/uglychain/tools/languages/javascript.py
+-rw-r--r--   0        0        0     2183 2024-02-02 05:00:03.843292 uglychain-0.1.9.post5/uglychain/tools/languages/powershell.py
+-rw-r--r--   0        0        0     1454 2024-02-18 07:37:49.344108 uglychain-0.1.9.post5/uglychain/tools/languages/python.py
+-rw-r--r--   0        0        0     2316 2024-02-04 01:03:36.202888 uglychain-0.1.9.post5/uglychain/tools/languages/r.py
+-rw-r--r--   0        0        0     2727 2024-02-02 04:58:54.083295 uglychain-0.1.9.post5/uglychain/tools/languages/shell.py
+-rw-r--r--   0        0        0     6290 2024-02-15 01:03:03.044612 uglychain-0.1.9.post5/uglychain/tools/languages/subprocess_language.py
+-rw-r--r--   0        0        0      388 2024-02-18 07:37:49.344108 uglychain-0.1.9.post5/uglychain/tools/search.py
+-rw-r--r--   0        0        0      270 2024-02-06 03:06:22.453705 uglychain-0.1.9.post5/uglychain/tools/text_completion.py
+-rw-r--r--   0        0        0      236 2024-02-27 14:11:51.732784 uglychain-0.1.9.post5/uglychain/utils/__init__.py
+-rw-r--r--   0        0        0     1913 2024-02-27 14:11:51.732784 uglychain-0.1.9.post5/uglychain/utils/config.py
+-rw-r--r--   0        0        0      487 2024-02-27 14:11:51.732784 uglychain-0.1.9.post5/uglychain/utils/enum.py
+-rw-r--r--   0        0        0     1683 2024-02-06 10:11:26.118363 uglychain-0.1.9.post5/uglychain/utils/nlp.py
+-rw-r--r--   0        0        0      681 2024-01-30 01:09:40.967697 uglychain-0.1.9.post5/uglychain/utils/retry_decorator.py
+-rw-r--r--   0        0        0      850 2024-02-23 13:54:05.770895 uglychain-0.1.9.post5/uglychain/utils/singleton.py
+-rw-r--r--   0        0        0    18911 2024-01-30 01:22:48.943666 uglychain-0.1.9.post5/uglychain/utils/stop_words.py
+-rw-r--r--   0        0        0      273 2024-02-08 01:18:36.553320 uglychain-0.1.9.post5/uglychain/worker/__init__.py
+-rw-r--r--   0        0        0     1805 2024-02-18 07:37:49.344108 uglychain-0.1.9.post5/uglychain/worker/base.py
+-rw-r--r--   0        0        0     1609 2024-02-04 11:35:32.877749 uglychain-0.1.9.post5/uglychain/worker/classify.py
+-rw-r--r--   0        0        0     4199 2024-02-14 10:32:33.849690 uglychain-0.1.9.post5/uglychain/worker/code_interpreter.py
+-rw-r--r--   0        0        0     5966 2024-02-06 03:08:17.985702 uglychain-0.1.9.post5/uglychain/worker/planner.py
+-rw-r--r--   0        0        0     2877 2024-02-04 11:11:01.857793 uglychain-0.1.9.post5/uglychain/worker/summary.py
+-rw-r--r--   0        0        0     1085 2024-02-03 11:33:49.057316 uglychain-0.1.9.post5/uglychain/worker/transformer.py
+-rw-r--r--   0        0        0     9237 1970-01-01 00:00:00.000000 uglychain-0.1.9.post5/setup.py
+-rw-r--r--   0        0        0     9335 1970-01-01 00:00:00.000000 uglychain-0.1.9.post5/PKG-INFO
```

### Comparing `uglychain-0.1.9.post4/LICENSE` & `uglychain-0.1.9.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/README.md` & `uglychain-0.1.9.post5/README.md`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/pyproject.toml` & `uglychain-0.1.9.post5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uglychain"
-version = "0.1.9.post4"
+version = "0.1.9.post5"
 description = "UglyChain：更好用的 LLM 应用构建工具"
 license = "MIT"
 authors = ["uglyboy <uglyboy@uglyboy.cn>"]
 readme = "README.md"
 repository = "https://github.com/uglyboy-tl/uglychain"
 documentation = "https://uglychain.uglyboy.cn"
```

### Comparing `uglychain-0.1.9.post4/uglychain/chains/base.py` & `uglychain-0.1.9.post5/uglychain/chains/base.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/chains/llm/llm.py` & `uglychain-0.1.9.post5/uglychain/chains/llm/llm.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         """
         # assert not (self.tools and self.response_model), "tools and response_model cannot be set at the same time"
         if self.tools:
             assert (
                 self.response_model is None or self.response_model == ActionResopnse
             ), "response_model must be ActionResopnse if tools is set"
         self.llm = self.model(self.is_init_delay)
-        del self.model
         logger.success(f"{self.model} loaded")
+        del self.model
         if self.system_prompt:
             self.llm.set_system_prompt(self.system_prompt)
         self.prompt = self.prompt_template
 
     @property
     def input_keys(self) -> List[str]:
         """Get the input keys.
```

### Comparing `uglychain-0.1.9.post4/uglychain/chains/llm/prompt.py` & `uglychain-0.1.9.post5/uglychain/chains/llm/prompt.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/chains/map.py` & `uglychain-0.1.9.post5/uglychain/chains/map.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/chains/react.py` & `uglychain-0.1.9.post5/uglychain/chains/react.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/chains/react_bad.py` & `uglychain-0.1.9.post5/uglychain/chains/react_bad.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/chains/reduce.py` & `uglychain-0.1.9.post5/uglychain/chains/reduce.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/base.py` & `uglychain-0.1.9.post5/uglychain/llm/base.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/instructor/json.py` & `uglychain-0.1.9.post5/uglychain/llm/instructor/json.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/instructor/yaml.py` & `uglychain-0.1.9.post5/uglychain/llm/instructor/yaml.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/llama_index.py` & `uglychain-0.1.9.post5/uglychain/llm/llama_index.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/provider/chatgpt.py` & `uglychain-0.1.9.post5/uglychain/llm/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/provider/dashscope.py` & `uglychain-0.1.9.post5/uglychain/llm/provider/dashscope.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/provider/gemini.py` & `uglychain-0.1.9.post5/uglychain/llm/provider/gemini.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/provider/model.py` & `uglychain-0.1.9.post5/uglychain/llm/provider/model.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/provider/ollama.py` & `uglychain-0.1.9.post5/uglychain/llm/provider/ollama.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/provider/openai_api.py` & `uglychain-0.1.9.post5/uglychain/llm/provider/openai_api.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/provider/sparkapi.py` & `uglychain-0.1.9.post5/uglychain/llm/provider/sparkapi.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/provider/yi.py` & `uglychain-0.1.9.post5/uglychain/llm/provider/yi.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/provider/zhipu.py` & `uglychain-0.1.9.post5/uglychain/llm/provider/zhipu.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/llm/tools.py` & `uglychain-0.1.9.post5/uglychain/llm/tools.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/retrievers/arxiv.py` & `uglychain-0.1.9.post5/uglychain/retrievers/arxiv.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/retrievers/base.py` & `uglychain-0.1.9.post5/uglychain/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/retrievers/bing.py` & `uglychain-0.1.9.post5/uglychain/retrievers/bing.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/retrievers/bm25.py` & `uglychain-0.1.9.post5/uglychain/retrievers/bm25.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/retrievers/combine.py` & `uglychain-0.1.9.post5/uglychain/retrievers/combine.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/retrievers/llama_index.py` & `uglychain-0.1.9.post5/uglychain/retrievers/llama_index.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/retrievers/model.py` & `uglychain-0.1.9.post5/uglychain/retrievers/model.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/retrievers/retrieve_with_llm.py` & `uglychain-0.1.9.post5/uglychain/retrievers/retrieve_with_llm.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/storage/file.py` & `uglychain-0.1.9.post5/uglychain/storage/file.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/storage/llama_index.py` & `uglychain-0.1.9.post5/uglychain/storage/llama_index.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/storage/sqlite.py` & `uglychain-0.1.9.post5/uglychain/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/tools/code_runner.py` & `uglychain-0.1.9.post5/uglychain/tools/code_runner.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/tools/languages/applescript.py` & `uglychain-0.1.9.post5/uglychain/tools/languages/applescript.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/tools/languages/base.py` & `uglychain-0.1.9.post5/uglychain/tools/languages/base.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/tools/languages/ipython.py` & `uglychain-0.1.9.post5/uglychain/tools/languages/ipython.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/tools/languages/javascript.py` & `uglychain-0.1.9.post5/uglychain/tools/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/tools/languages/powershell.py` & `uglychain-0.1.9.post5/uglychain/tools/languages/powershell.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/tools/languages/python.py` & `uglychain-0.1.9.post5/uglychain/tools/languages/python.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/tools/languages/r.py` & `uglychain-0.1.9.post5/uglychain/tools/languages/r.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/tools/languages/shell.py` & `uglychain-0.1.9.post5/uglychain/tools/languages/shell.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/tools/languages/subprocess_language.py` & `uglychain-0.1.9.post5/uglychain/tools/languages/subprocess_language.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/utils/config.py` & `uglychain-0.1.9.post5/uglychain/utils/config.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/utils/nlp.py` & `uglychain-0.1.9.post5/uglychain/utils/nlp.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/utils/retry_decorator.py` & `uglychain-0.1.9.post5/uglychain/utils/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/utils/singleton.py` & `uglychain-0.1.9.post5/uglychain/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/utils/stop_words.py` & `uglychain-0.1.9.post5/uglychain/utils/stop_words.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/worker/base.py` & `uglychain-0.1.9.post5/uglychain/worker/base.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/worker/classify.py` & `uglychain-0.1.9.post5/uglychain/worker/classify.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/worker/code_interpreter.py` & `uglychain-0.1.9.post5/uglychain/worker/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/worker/planner.py` & `uglychain-0.1.9.post5/uglychain/worker/planner.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/worker/summary.py` & `uglychain-0.1.9.post5/uglychain/worker/summary.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/uglychain/worker/transformer.py` & `uglychain-0.1.9.post5/uglychain/worker/transformer.py`

 * *Files identical despite different names*

### Comparing `uglychain-0.1.9.post4/setup.py` & `uglychain-0.1.9.post5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                                                                             'llama-index-embeddings-openai[llama-index]>=0.1.0,<0.2.0'],
  'ollama': ['ollama[ollama]>=0.1.6,<0.2.0'],
  'openai': ['tiktoken[openai]>=0.5.2,<0.6.0'],
  'sparkapi': ['websockets[sparkapi]>=12.0,<13.0']}
 
 setup_kwargs = {
     'name': 'uglychain',
-    'version': '0.1.9.post4',
+    'version': '0.1.9.post5',
     'description': 'UglyChain：更好用的 LLM 应用构建工具',
     'long_description': '[![Release Notes][release-shield]][release-url]\n[![Contributors][contributors-shield]][contributors-url]\n[![Forks][forks-shield]][forks-url]\n[![Stargazers][stars-shield]][stars-url]\n[![Issues][issues-shield]][issues-url]\n[![MIT License][license-shield]][license-url]\n\n<!-- PROJECT LOGO -->\n<br />\n<div align="center">\n  <a href="https://github.com/uglyboy-tl/UglyChain">\n    <!-- <img src="images/logo.png" alt="Logo" width="80" height="80"> -->\n  </a>\n\n  <h3 align="center">UglyChain</h3>\n\n  <p align="center">\n    ⚡ UglyChain：更好用的 LLM 应用构建工具 ⚡\n    <br />\n    <a href="https://uglychain.uglyboy.cn"><strong>Explore the docs »</strong></a>\n    <br />\n    <br />\n    <a href="https://github.com/uglyboy-tl/UglyChain/issues">Report Bug</a>\n    ·\n    <a href="https://github.com/uglyboy-tl/UglyChain/issues">Request Feature</a>\n  </p>\n</div>\n\n## 🤔 What is UglyChain?\n现在有很多利用大模型 LLM 进行应用构建的工具，最有名的就是 LangChain。早期的 LangChain 整个框架并不完善，很多并不直观的定义和调用方式，以及将内部功能封装得太彻底，使的难以定制化的更充分的利用大模型的能力来解决问题。所以我就开发的最初的 UglyGPT（UglyChain的原型），试图解决这个问题。\n\n到了今天，GPTs 也已经面世很长时间了，也有了越来越多的 LLM 应用构建工具。但是这些工具都有一个共同的问题：**不够直观**。\n从底层来说，现在的大模型是基于 Chat 进行接口交互的，这对于应用开发而言并不友好，因为应用开发更多的是模板化的结构化内容生成，而不是对话式的交互。所以我们需要一个对应用开发更加友好的接口，这就是 UglyChain 的初衷。\n\n## Features\n\n- 📦 对大模型接口进行封装，提供对工程化更加直观易懂的交互方式，而不是传统的对话式交互。\n  - 可以参数化 Prompt，更加方便地进行批量调用\n  - 可以对 Prompt 进行结构化返回，方便后续处理\n  - 可以对 Prompt 进行角色设置，方便模型进行角色扮演（这个过程无需操控 Message）\n- 🔗 对大模型的高级调用进行封装，提供更加方便的交互方式\n  - 提供了类似于 MapReduce 的功能，可以通过 MapChain 对多个 Prompt 进行并行调用，也可以用 ReduceChain 对多个 Prompt 进行串行调用\n  - 大模型最优质的能力之一就是拥有 ReAct 能力。我们提供了 ReActChain 便捷的实现这种能力。\n- 💾 提供了搜索引擎的封装，可以方便地进行搜索引擎的调用。\n  - 注意我们只封装了搜索过程的调用，而没有提供搜索引擎的搭建。如果要构建基于 RAG 的应用，需要利用其他的工具完成资料库的建立，而我们只提供对资料库搜索功能的封装。\n\n## Getting Started\n\nWith pip:\n\n```bash\npip install uglychain\n```\n\n## Usage\n\n### LLM\n\n> 这是最基础的模型调用类，其他的高级类也都继承和使用了这个类的基本功能。\n\n快速使用：\n\n```python\nfrom uglychain import LLM, Model\n\nllm = LLM()\nprint(llm("你是谁？")) # 与模型对话，返回字符串的回答\n```\n\n调整基础配置选项：\n\n```python\nllm = LLM(model = Model.YI) # 可以选择更多的模型，如 Model.GPT3_TURBO、Model.GPT4 等等\nllm = LLM(system_prompt = "我想让你担任职业顾问。我将为您提供一个在职业生涯中寻求指导的人，您的任务是帮助他们根据自己的技能、兴趣和经验确定最适合的职业。您还应该对可用的各种选项进行研究，解释不同行业的就业市场趋势，并就哪些资格对追求特定领域有益提出建议。") # 可以对模型设置角色，这样模型就会以这个角色的视角来回答问题。设置的内容保存在 System Message 中。\n```\n\n参数化 prompt：\n\n```python\nllm = LLM(prompt_template = "{object}的{position}是谁？")\nprint(llm(object = "《红楼梦》", position = "作者"))\nprint(llm(object = "上海市", position = "市长"))\n```\n\n对于 prompt 中只有一个参数的情况，可以直接传入参数：\n\n```python\nllm = LLM("介绍一下{object}")\nprint(llm("Transformer"))\n```\n\n结构化返回结果：\n\n```python\nclass UserDetail(BaseModel):\n    name: str\n    age: int\n\nllm = LLM(response_model=UserDetail)\nprint(llm("Extract Jason is 25 years old")) # UserDetail(name=\'Jason\', age=25)\n```\n\n### MapChain\n\n> 这是一个可以并行对同类型 Prompt 进行调用的类，可以大大提高调用效率。\n\n快速使用：\n\n```python\nfrom uglychain import MapChain\n\nllm = MapChain()\nprint(llm([\n        {"input": "How old are you?"},\n        {"input": "What is the meaning of life?"},\n        {"input": "What is the hottest day of the year?"},\n    ]))\n```\n\n类似于 LLM，也可以对 MapChain 进行更高阶的使用：\n\n```python\nclass AUTHOR(BaseModel):\n    name: str = Field(..., description="姓名")\n    introduction: str = Field(..., description="简介")\n\nllm = MapChain(prompt_template="{book}的{position}是谁？", response_model=AUTHOR, map_keys=["book",])\ninput = [\n    "《红楼梦》",\n    "《西游记》",\n    "《三国演义》",\n    "《水浒传》",\n]\nprint(llm(book=input, position="作者"))\n```\n\n## Roadmap\n\n- [x] 增加 FunctionCall 的能力\n- [ ] 增加 Memory 的能力\n\n## Contributing\n\nContributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.\n\nIf you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".\nDon\'t forget to give the project a star! Thanks again!\n\n1. Fork the Project\n2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)\n3. Commit your Changes (`git commit -m \'Add some AmazingFeature\'`)\n4. Push to the Branch (`git push origin feature/AmazingFeature`)\n5. Open a Pull Request\n\n## License\n\nDistributed under the MIT License. See `LICENSE.txt` for more information.\n\n<!-- MARKDOWN LINKS & IMAGES -->\n<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->\n[release-shield]:https://img.shields.io/github/release/uglyboy-tl/UglyChain.svg?style=for-the-badge\n[release-url]: https://github.com/uglyboy-tl/UglyChain/releases\n[contributors-shield]: https://img.shields.io/github/contributors/uglyboy-tl/UglyChain.svg?style=for-the-badge\n[contributors-url]: https://github.com/uglyboy-tl/UglyChain/graphs/contributors\n[forks-shield]: https://img.shields.io/github/forks/uglyboy-tl/UglyChain.svg?style=for-the-badge\n[forks-url]: https://github.com/uglyboy-tl/UglyChain/network/members\n[stars-shield]: https://img.shields.io/github/stars/uglyboy-tl/UglyChain.svg?style=for-the-badge\n[stars-url]: https://github.com/uglyboy-tl/UglyChain/stargazers\n[issues-shield]: https://img.shields.io/github/issues/uglyboy-tl/UglyChain.svg?style=for-the-badge\n[issues-url]: https://github.com/uglyboy-tl/UglyChain/issues\n[license-shield]: https://img.shields.io/github/license/uglyboy-tl/UglyChain.svg?style=for-the-badge\n[license-url]: https://github.com/uglyboy-tl/UglyChain/blob/master/LICENSE.txt',
     'author': 'uglyboy',
     'author_email': 'uglyboy@uglyboy.cn',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/uglyboy-tl/uglychain',
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 [dashscope]>=1.14.1,<2.0.0'], 'gemini': ['google-generativeai
 [gemini]>=0.3.2,<0.4.0'], 'ipython': ['ipykernel[ipython]>=6.26.0,<7.0.0'],
 'llama-index:python_full_version >= "3.8.1" and python_version < "3.12"':
 ['llama-index-core[llama-index]>=0.10.1,<0.11.0', 'llama-index-embeddings-
 openai[llama-index]>=0.1.0,<0.2.0'], 'ollama': ['ollama
 [ollama]>=0.1.6,<0.2.0'], 'openai': ['tiktoken[openai]>=0.5.2,<0.6.0'],
 'sparkapi': ['websockets[sparkapi]>=12.0,<13.0']} setup_kwargs = { 'name':
-'uglychain', 'version': '0.1.9.post4', 'description': 'UglyChainï¼æ´å¥½ç¨ç
+'uglychain', 'version': '0.1.9.post5', 'description': 'UglyChainï¼æ´å¥½ç¨ç
 LLM åºç¨æå»ºå·¥å·', 'long_description': '[![Release Notes][release-
 shield]][release-url]\n[![Contributors][contributors-shield]][contributors-
 url]\n[![Forks][forks-shield]][forks-url]\n[![Stargazers][stars-shield]][stars-
 url]\n[![Issues][issues-shield]][issues-url]\n[![MIT License][license-shield]]
 [license-url]\n\n\n
 \n
                                  \n _\_n_ _\_n_ \n\n
```

### Comparing `uglychain-0.1.9.post4/PKG-INFO` & `uglychain-0.1.9.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uglychain
-Version: 0.1.9.post4
+Version: 0.1.9.post5
 Summary: UglyChain：更好用的 LLM 应用构建工具
 Home-page: https://github.com/uglyboy-tl/uglychain
 License: MIT
 Author: uglyboy
 Author-email: uglyboy@uglyboy.cn
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

