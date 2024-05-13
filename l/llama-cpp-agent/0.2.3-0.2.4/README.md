# Comparing `tmp/llama_cpp_agent-0.2.3.tar.gz` & `tmp/llama_cpp_agent-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_cpp_agent-0.2.3.tar", last modified: Mon May 13 21:03:01 2024, max compression
+gzip compressed data, was "llama_cpp_agent-0.2.4.tar", last modified: Mon May 13 22:00:03 2024, max compression
```

## Comparing `llama_cpp_agent-0.2.3.tar` & `llama_cpp_agent-0.2.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.892000 llama_cpp_agent-0.2.3/
--rw-rw-rw-   0        0        0     1115 2023-12-31 18:08:30.000000 llama_cpp_agent-0.2.3/LICENSE
--rw-rw-rw-   0        0        0    10780 2024-05-13 21:03:01.891000 llama_cpp_agent-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     9555 2024-05-13 20:57:26.000000 llama_cpp_agent-0.2.3/ReadMe.md
--rw-rw-rw-   0        0        0     1054 2024-05-13 20:58:24.000000 llama_cpp_agent-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 21:03:01.892000 llama_cpp_agent-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.841326 llama_cpp_agent-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.860837 llama_cpp_agent-0.2.3/src/llama_cpp_agent/
--rw-rw-rw-   0        0        0      342 2024-05-12 15:02:27.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.871347 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/
--rw-rw-rw-   0        0        0        0 2023-12-31 14:27:21.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/__init__.py
--rw-rw-rw-   0        0        0     3408 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/core_memory_manager.py
--rw-rw-rw-   0        0        0     1654 2024-05-11 19:58:35.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/event_memory.py
--rw-rw-rw-   0        0        0     3882 2024-05-11 19:58:35.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/event_memory_manager.py
--rw-rw-rw-   0        0        0     9949 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/memory_tools.py
--rw-rw-rw-   0        0        0     5031 2024-04-18 21:27:19.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/retrieval_memory.py
--rw-rw-rw-   0        0        0     1640 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
--rw-rw-rw-   0        0        0    12570 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/chain.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.874347 llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/
--rw-rw-rw-   0        0        0      307 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/__init__.py
--rw-rw-rw-   0        0        0     7628 2024-05-13 19:57:48.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/basic_chat_history.py
--rw-rw-rw-   0        0        0     5417 2024-05-13 20:23:09.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/chat_history_base.py
--rw-rw-rw-   0        0        0     3113 2024-05-12 20:46:35.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/messages.py
--rw-rw-rw-   0        0        0    10771 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/function_calling.py
--rw-rw-rw-   0        0        0    12448 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/function_calling_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.875485 llama_cpp_agent-0.2.3/src/llama_cpp_agent/gbnf_grammar_generator/
--rw-rw-rw-   0        0        0        0 2023-12-27 02:55:26.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
--rw-rw-rw-   0        0        0    52886 2024-05-11 21:21:16.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
--rw-rw-rw-   0        0        0    13675 2024-05-12 13:59:03.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/hermes_2_pro_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.877486 llama_cpp_agent-0.2.3/src/llama_cpp_agent/json_schema_generator/
--rw-rw-rw-   0        0        0       53 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/json_schema_generator/__init__.py
--rw-rw-rw-   0        0        0    11683 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/json_schema_generator/schema_generator.py
--rw-rw-rw-   0        0        0    21474 2024-05-13 20:02:22.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.879486 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_documentation/
--rw-rw-rw-   0        0        0      116 2024-05-09 08:09:41.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_documentation/__init__.py
--rw-rw-rw-   0        0        0    18850 2024-05-12 00:42:14.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_documentation/documentation_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.881487 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_output_settings/
--rw-rw-rw-   0        0        0       76 2024-05-09 12:50:53.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_output_settings/__init__.py
--rw-rw-rw-   0        0        0    32939 2024-05-12 05:26:57.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_output_settings/settings.py
--rw-rw-rw-   0        0        0     7027 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_prompt_template.py
--rw-rw-rw-   0        0        0    11752 2024-05-13 19:22:50.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/messages_formatter.py
--rw-rw-rw-   0        0        0     3990 2024-05-12 13:53:06.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/mixtral_8x22b_agent.py
--rw-rw-rw-   0        0        0     3613 2024-04-18 21:27:19.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/output_parser.py
--rw-rw-rw-   0        0        0     5296 2024-05-12 04:02:32.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/prompt_templates.py
--rw-rw-rw-   0        0        0      816 2024-05-12 03:46:37.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/prompts.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.886491 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/
--rw-rw-rw-   0        0        0      277 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/__init__.py
--rw-rw-rw-   0        0        0     8062 2024-05-13 00:41:32.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/llama_cpp_python.py
--rw-rw-rw-   0        0        0    13758 2024-05-13 00:41:32.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/llama_cpp_server.py
--rw-rw-rw-   0        0        0     5392 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/provider_base.py
--rw-rw-rw-   0        0        0     9155 2024-05-13 00:41:32.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/tgi_server.py
--rw-rw-rw-   0        0        0     6621 2024-05-13 00:41:32.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/vllm_server.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.889000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/rag/
--rw-rw-rw-   0        0        0        0 2024-05-05 05:07:17.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/rag/__init__.py
--rw-rw-rw-   0        0        0     2359 2024-05-05 05:07:17.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/rag/rag_colbert_reranker.py
--rw-rw-rw-   0        0        0     7073 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/structured_output_agent.py
--rw-rw-rw-   0        0        0     3945 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/text_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.889999 llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/
--rw-rw-rw-   0        0        0    10780 2024-05-13 21:03:01.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2197 2024-05-13 21:03:01.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 21:03:01.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      206 2024-05-13 21:03:01.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-13 21:03:01.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:03.798621 llama_cpp_agent-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-05-13 22:00:03.798621 llama_cpp_agent-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/ReadMe.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 22:00:03.798621 llama_cpp_agent-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:03.786620 llama_cpp_agent-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:03.790621 llama_cpp_agent-0.2.4/src/llama_cpp_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:03.794621 llama_cpp_agent-0.2.4/src/llama_cpp_agent/agent_memory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/agent_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/agent_memory/core_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/agent_memory/event_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/agent_memory/event_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/agent_memory/memory_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/agent_memory/retrieval_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:03.794621 llama_cpp_agent-0.2.4/src/llama_cpp_agent/chat_history/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/chat_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/chat_history/basic_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/chat_history/chat_history_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/chat_history/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/function_calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/function_calling_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:03.794621 llama_cpp_agent-0.2.4/src/llama_cpp_agent/gbnf_grammar_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51567 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/hermes_2_pro_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:03.794621 llama_cpp_agent-0.2.4/src/llama_cpp_agent/json_schema_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/json_schema_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/json_schema_generator/schema_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21015 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/llm_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:03.794621 llama_cpp_agent-0.2.4/src/llama_cpp_agent/llm_documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/llm_documentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18378 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/llm_documentation/documentation_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:03.798621 llama_cpp_agent-0.2.4/src/llama_cpp_agent/llm_output_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/llm_output_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32249 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/llm_output_settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/llm_prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/messages_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/mixtral_8x22b_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/prompt_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:03.798621 llama_cpp_agent-0.2.4/src/llama_cpp_agent/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/providers/llama_cpp_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/providers/llama_cpp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/providers/provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/providers/tgi_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/providers/vllm_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:03.798621 llama_cpp_agent-0.2.4/src/llama_cpp_agent/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/rag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/rag/rag_colbert_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/structured_output_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-13 21:59:59.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:03.798621 llama_cpp_agent-0.2.4/src/llama_cpp_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-05-13 22:00:03.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-13 22:00:03.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:00:03.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-13 22:00:03.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 22:00:03.000000 llama_cpp_agent-0.2.4/src/llama_cpp_agent.egg-info/top_level.txt
```

### Comparing `llama_cpp_agent-0.2.3/LICENSE` & `llama_cpp_agent-0.2.4/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-llama-cpp-agent
-MIT License
-
-Copyright (c) 2023-2024 Maximilian Winter
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+llama-cpp-agent
+MIT License
+
+Copyright (c) 2023-2024 Maximilian Winter
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `llama_cpp_agent-0.2.3/PKG-INFO` & `llama_cpp_agent-0.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-Metadata-Version: 2.1
-Name: llama-cpp-agent
-Version: 0.2.3
-Summary: A framework for building LLM based AI agents with llama.cpp.
-Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
-Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
-Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: llama-cpp-python>=0.2.60
-Requires-Dist: pydantic>=2.5.3
-Requires-Dist: requests>=2.31.0
-Requires-Dist: docstring_parser
-Requires-Dist: aiohttp
-Provides-Extra: agent-memory
-Requires-Dist: chromadb; extra == "agent-memory"
-Requires-Dist: SQLAlchemy; extra == "agent-memory"
-Requires-Dist: numpy; extra == "agent-memory"
-Requires-Dist: scipy; extra == "agent-memory"
-Provides-Extra: rag
-Requires-Dist: ragatouille; extra == "rag"
-Provides-Extra: vllm-provider
-Requires-Dist: openai; extra == "vllm-provider"
-Provides-Extra: mixtral-agent
-Requires-Dist: mistral-common; extra == "mixtral-agent"
-
-# llama-cpp-agent
-
-[![PyPI - Version](https://img.shields.io/pypi/v/llama-cpp-agent?logo=pypi&color=%2341bb13)](https://pypi.org/project/llama-cpp-agent/)
-[![Discord](https://img.shields.io/discord/1237393014154985582?logo=Discord&logoColor=%23ffffff&label=Discord&link=https%3A%2F%2Fdiscord.gg%2FsRMvWKrh)](https://discord.gg/sRMvWKrh)
-
-<img src="./logo/logo_orange.png" alt="llama-cpp-agent logo" width="280"/>
-
-## Introduction
-The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
-
-The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
-
-The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
-
-## Key Features
-- **Simple Chat Interface**: Engage in seamless conversations with LLMs.
-- **Structured Output**: Generate structured output (objects) from LLMs.
-- **Single and Parallel Function Calling**: Execute functions using LLMs.
-- **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
-- **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
-- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
-- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
-- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
-- **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
-
-
-## Table of Contents
-- [Introduction](#introduction)
-- [Key Features](#key-features)
-- [Installation](#installation)
-- [Documentation](#documentation)
-- [Getting Started](#getting-started)
-- [Discord Community](#discord-community)
-- [Usage Examples](#usage-examples)
-    - [Simple Chat](#simple-chat-example-using-llamacpp-server-backend)
-    - [Parallel Function Calling](#parallel-function-calling-agent-example)
-    - [Structured Output](#structured-output)
-    - [RAG - Retrieval Augmented Generation](#rag---retrieval-augmented-generation)
-    - [llama-index Tools](#llama-index-tools-example)
-    - [Sequential Chain](#sequential-chain-example)
-    - [Mapping Chain](#mapping-chain-example)
-    - [Knowledge Graph Creation](#knowledge-graph-creation-example)
-- [Additional Information](#additional-information)
-    - [Predefined Messages Formatter](#predefined-messages-formatter)
-    - [Creating Custom Messages Formatter](#creating-custom-messages-formatter)
-- [Contributing](#contributing)
-- [License](#license)
-- [FAQ](#faq)
-
-
-
-## Installation
-Install the llama-cpp-agent framework using pip:
-```shell
-pip install llama-cpp-agent
-```
-## Documentation
-You can find the latest documentation [here!](https://llama-cpp-agent.readthedocs.io/en/latest/)
-
-## Getting Started
-You can find the get started guide [here!](https://llama-cpp-agent.readthedocs.io/en/latest/get-started/)
-
-## Discord Community
-Join the Discord Community [here](https://discord.gg/6tGznupZGX)
-
-## Usage Examples
-The llama-cpp-agent framework provides a wide range of examples demonstrating its capabilities. Here are some key examples:
-
-### Simple Chat Example using llama.cpp server backend
-This example demonstrates how to initiate a chat with an LLM model using the llama.cpp server backend. It supports llama-cpp-python Llama class instances, OpenAI endpoints with GBNF grammar support, and the llama.cpp backend server.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/simple-chat-example/)
-
-### Parallel Function Calling Agent Example
-This example showcases parallel function calling using the FunctionCallingAgent class. It demonstrates how to define and execute multiple functions concurrently.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/parallel_function_calling/)
-
-### Structured Output
-This example illustrates how to generate structured output objects using the StructuredOutputAgent class. It shows how to create a dataset entry of a book from unstructured data.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/structured-output-example/)
-
-### RAG - Retrieval Augmented Generation
-This example demonstrates Retrieval Augmented Generation (RAG) with colbert reranking. It requires installing the optional rag dependencies (ragatouille).
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/rag/)
-
-### llama-index Tools Example
-This example shows how to use llama-index tools and query engines with the FunctionCallingAgent class.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/llama_index_tool_use/)
-
-### Sequential Chain Example
-This example demonstrates how to create a complete product launch campaign using a sequential chain.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/sequential_chain/)
-
-### Mapping Chain Example
-This example illustrates how to create a mapping chain to summarize multiple articles into a single summary.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/map_chain/)
-
-### Knowledge Graph Creation Example
-This example, based on an example from the Instructor library for OpenAI, shows how to create a knowledge graph using the llama-cpp-agent framework.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/knowledge-graph-example/)
-
-
-## Additional Information
-
-### Predefined Messages Formatter
-
-The llama-cpp-agent framework provides predefined message formatters to format messages for the LLM model. The `MessagesFormatterType` enum defines the available formatters:
-
-- `MessagesFormatterType.MISTRAL`: Formats messages using the MISTRAL format.
-- `MessagesFormatterType.CHATML`: Formats messages using the CHATML format.
-- `MessagesFormatterType.VICUNA`: Formats messages using the VICUNA format.
-- `MessagesFormatterType.LLAMA_2`: Formats messages using the LLAMA 2 format.
-- `MessagesFormatterType.SYNTHIA`: Formats messages using the SYNTHIA format.
-- `MessagesFormatterType.NEURAL_CHAT`: Formats messages using the NEURAL CHAT format.
-- `MessagesFormatterType.SOLAR`: Formats messages using the SOLAR format.
-- `MessagesFormatterType.OPEN_CHAT`: Formats messages using the OPEN CHAT format.
-- `MessagesFormatterType.ALPACA`: Formats messages using the ALPACA format.
-- `MessagesFormatterType.CODE_DS`: Formats messages using the CODE DS format.
-- `MessagesFormatterType.B22`: Formats messages using the B22 format.
-- `MessagesFormatterType.LLAMA_3`: Formats messages using the LLAMA 3 format.
-- `MessagesFormatterType.PHI_3`: Formats messages using the PHI 3 format.
-
-### Creating Custom Messages Formatter
-
-You can create your own custom messages formatter by instantiating the `MessagesFormatter` class with the desired parameters:
-
-```python
-from llama_cpp_agent.chat_history.messages_formatter import MessagesFormatter, PromptMarkers, Roles
-
-custom_prompt_markers = {
-    Roles.system: PromptMarkers("<|system|>", "<|endsystem|>"),
-    Roles.user: PromptMarkers("<|user|>", "<|enduser|>"),
-    Roles.assistant: PromptMarkers("<|assistant|>", "<|endassistant|>"),
-    Roles.tool: PromptMarkers("<|tool|>", "<|endtool|>"),
-}
-
-custom_formatter = MessagesFormatter(
-    pre_prompt="",
-    prompt_markers=custom_prompt_markers,
-    include_sys_prompt_in_first_user_message=False,
-    default_stop_sequences=["<|endsystem|>", "<|enduser|>", "<|endassistant|>", "<|endtool|>"]
-)
-```
-
-## Contributing
-We welcome contributions to the llama-cpp-agent framework! If you'd like to contribute, please follow these guidelines:
-
-1. Fork the repository and create your branch from `master`.
-2. Ensure your code follows the project's coding style and conventions.
-3. Write clear, concise commit messages and pull request descriptions.
-4. Test your changes thoroughly before submitting a pull request.
-5. Open a pull request to the `master` branch.
-
-If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/Maximilian-Winter/llama-cpp-agent/issues).
-
-## License
-The llama-cpp-agent framework is released under the [MIT License](https://github.com/Maximilian-Winter/llama-cpp-agent/blob/master/LICENSE).
-
-## FAQ
-
-**Q: How do I install the optional dependencies for RAG?**  
-A: To use the RAGColbertReranker class and the RAG example, you need to install the optional rag dependencies (ragatouille). You can do this by running `pip install llama-cpp-agent[rag]`.
-
-**Q: Can I contribute to the llama-cpp-agent project?**  
-A: Absolutely! We welcome contributions from the community. Please refer to the [Contributing](#contributing) section for guidelines on how to contribute.
-
-**Q: Is llama-cpp-agent compatible with the latest version of llama-cpp-python?**  
-A: Yes, llama-cpp-agent is designed to work with the latest version of llama-cpp-python. However, if you encounter any compatibility issues, please open an issue on the GitHub repository.
+Metadata-Version: 2.1
+Name: llama-cpp-agent
+Version: 0.2.4
+Summary: A framework for building LLM based AI agents with llama.cpp.
+Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
+Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
+Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: llama-cpp-python>=0.2.60
+Requires-Dist: pydantic>=2.5.3
+Requires-Dist: requests>=2.31.0
+Requires-Dist: docstring_parser
+Requires-Dist: aiohttp
+Provides-Extra: agent-memory
+Requires-Dist: chromadb; extra == "agent-memory"
+Requires-Dist: SQLAlchemy; extra == "agent-memory"
+Requires-Dist: numpy; extra == "agent-memory"
+Requires-Dist: scipy; extra == "agent-memory"
+Provides-Extra: rag
+Requires-Dist: ragatouille; extra == "rag"
+Provides-Extra: vllm-provider
+Requires-Dist: openai; extra == "vllm-provider"
+Provides-Extra: mixtral-agent
+Requires-Dist: mistral-common; extra == "mixtral-agent"
+
+# llama-cpp-agent
+
+[![PyPI - Version](https://img.shields.io/pypi/v/llama-cpp-agent?logo=pypi&color=%2341bb13)](https://pypi.org/project/llama-cpp-agent/)
+[![Discord](https://img.shields.io/discord/1237393014154985582?logo=Discord&logoColor=%23ffffff&label=Discord&link=https%3A%2F%2Fdiscord.gg%2FsRMvWKrh)](https://discord.gg/sRMvWKrh)
+
+![llama-cpp-agent logo](https://github.com/Maximilian-Winter/llama-cpp-agent/blob/ed6b0973c15cf653d406e53dd6b4efc8d97796cb/logo/logo_orange.png)
+
+## Introduction
+The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
+
+The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
+
+The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
+
+## Key Features
+- **Simple Chat Interface**: Engage in seamless conversations with LLMs.
+- **Structured Output**: Generate structured output (objects) from LLMs.
+- **Single and Parallel Function Calling**: Execute functions using LLMs.
+- **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
+- **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
+- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
+- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
+- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
+- **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
+
+
+## Table of Contents
+- [Introduction](#introduction)
+- [Key Features](#key-features)
+- [Installation](#installation)
+- [Documentation](#documentation)
+- [Getting Started](#getting-started)
+- [Discord Community](#discord-community)
+- [Usage Examples](#usage-examples)
+    - [Simple Chat](#simple-chat-example-using-llamacpp-server-backend)
+    - [Parallel Function Calling](#parallel-function-calling-agent-example)
+    - [Structured Output](#structured-output)
+    - [RAG - Retrieval Augmented Generation](#rag---retrieval-augmented-generation)
+    - [llama-index Tools](#llama-index-tools-example)
+    - [Sequential Chain](#sequential-chain-example)
+    - [Mapping Chain](#mapping-chain-example)
+    - [Knowledge Graph Creation](#knowledge-graph-creation-example)
+- [Additional Information](#additional-information)
+    - [Predefined Messages Formatter](#predefined-messages-formatter)
+    - [Creating Custom Messages Formatter](#creating-custom-messages-formatter)
+- [Contributing](#contributing)
+- [License](#license)
+- [FAQ](#faq)
+
+
+
+## Installation
+Install the llama-cpp-agent framework using pip:
+```shell
+pip install llama-cpp-agent
+```
+## Documentation
+You can find the latest documentation [here!](https://llama-cpp-agent.readthedocs.io/en/latest/)
+
+## Getting Started
+You can find the get started guide [here!](https://llama-cpp-agent.readthedocs.io/en/latest/get-started/)
+
+## Discord Community
+Join the Discord Community [here](https://discord.gg/6tGznupZGX)
+
+## Usage Examples
+The llama-cpp-agent framework provides a wide range of examples demonstrating its capabilities. Here are some key examples:
+
+### Simple Chat Example using llama.cpp server backend
+This example demonstrates how to initiate a chat with an LLM model using the llama.cpp server backend. It supports llama-cpp-python Llama class instances, OpenAI endpoints with GBNF grammar support, and the llama.cpp backend server.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/simple-chat-example/)
+
+### Parallel Function Calling Agent Example
+This example showcases parallel function calling using the FunctionCallingAgent class. It demonstrates how to define and execute multiple functions concurrently.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/parallel_function_calling/)
+
+### Structured Output
+This example illustrates how to generate structured output objects using the StructuredOutputAgent class. It shows how to create a dataset entry of a book from unstructured data.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/structured-output-example/)
+
+### RAG - Retrieval Augmented Generation
+This example demonstrates Retrieval Augmented Generation (RAG) with colbert reranking. It requires installing the optional rag dependencies (ragatouille).
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/rag/)
+
+### llama-index Tools Example
+This example shows how to use llama-index tools and query engines with the FunctionCallingAgent class.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/llama_index_tool_use/)
+
+### Sequential Chain Example
+This example demonstrates how to create a complete product launch campaign using a sequential chain.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/sequential_chain/)
+
+### Mapping Chain Example
+This example illustrates how to create a mapping chain to summarize multiple articles into a single summary.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/map_chain/)
+
+### Knowledge Graph Creation Example
+This example, based on an example from the Instructor library for OpenAI, shows how to create a knowledge graph using the llama-cpp-agent framework.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/knowledge-graph-example/)
+
+
+## Additional Information
+
+### Predefined Messages Formatter
+
+The llama-cpp-agent framework provides predefined message formatters to format messages for the LLM model. The `MessagesFormatterType` enum defines the available formatters:
+
+- `MessagesFormatterType.MISTRAL`: Formats messages using the MISTRAL format.
+- `MessagesFormatterType.CHATML`: Formats messages using the CHATML format.
+- `MessagesFormatterType.VICUNA`: Formats messages using the VICUNA format.
+- `MessagesFormatterType.LLAMA_2`: Formats messages using the LLAMA 2 format.
+- `MessagesFormatterType.SYNTHIA`: Formats messages using the SYNTHIA format.
+- `MessagesFormatterType.NEURAL_CHAT`: Formats messages using the NEURAL CHAT format.
+- `MessagesFormatterType.SOLAR`: Formats messages using the SOLAR format.
+- `MessagesFormatterType.OPEN_CHAT`: Formats messages using the OPEN CHAT format.
+- `MessagesFormatterType.ALPACA`: Formats messages using the ALPACA format.
+- `MessagesFormatterType.CODE_DS`: Formats messages using the CODE DS format.
+- `MessagesFormatterType.B22`: Formats messages using the B22 format.
+- `MessagesFormatterType.LLAMA_3`: Formats messages using the LLAMA 3 format.
+- `MessagesFormatterType.PHI_3`: Formats messages using the PHI 3 format.
+
+### Creating Custom Messages Formatter
+
+You can create your own custom messages formatter by instantiating the `MessagesFormatter` class with the desired parameters:
+
+```python
+from llama_cpp_agent.messages_formatter import MessagesFormatter, PromptMarkers, Roles
+
+custom_prompt_markers = {
+    Roles.system: PromptMarkers("<|system|>", "<|endsystem|>"),
+    Roles.user: PromptMarkers("<|user|>", "<|enduser|>"),
+    Roles.assistant: PromptMarkers("<|assistant|>", "<|endassistant|>"),
+    Roles.tool: PromptMarkers("<|tool|>", "<|endtool|>"),
+}
+
+custom_formatter = MessagesFormatter(
+    pre_prompt="",
+    prompt_markers=custom_prompt_markers,
+    include_sys_prompt_in_first_user_message=False,
+    default_stop_sequences=["<|endsystem|>", "<|enduser|>", "<|endassistant|>", "<|endtool|>"]
+)
+```
+
+## Contributing
+We welcome contributions to the llama-cpp-agent framework! If you'd like to contribute, please follow these guidelines:
+
+1. Fork the repository and create your branch from `master`.
+2. Ensure your code follows the project's coding style and conventions.
+3. Write clear, concise commit messages and pull request descriptions.
+4. Test your changes thoroughly before submitting a pull request.
+5. Open a pull request to the `master` branch.
+
+If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/Maximilian-Winter/llama-cpp-agent/issues).
+
+## License
+The llama-cpp-agent framework is released under the [MIT License](https://github.com/Maximilian-Winter/llama-cpp-agent/blob/master/LICENSE).
+
+## FAQ
+
+**Q: How do I install the optional dependencies for RAG?**  
+A: To use the RAGColbertReranker class and the RAG example, you need to install the optional rag dependencies (ragatouille). You can do this by running `pip install llama-cpp-agent[rag]`.
+
+**Q: Can I contribute to the llama-cpp-agent project?**  
+A: Absolutely! We welcome contributions from the community. Please refer to the [Contributing](#contributing) section for guidelines on how to contribute.
+
+**Q: Is llama-cpp-agent compatible with the latest version of llama-cpp-python?**  
+A: Yes, llama-cpp-agent is designed to work with the latest version of llama-cpp-python. However, if you encounter any compatibility issues, please open an issue on the GitHub repository.
```

### Comparing `llama_cpp_agent-0.2.3/ReadMe.md` & `llama_cpp_agent-0.2.4/ReadMe.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-# llama-cpp-agent
-
-[![PyPI - Version](https://img.shields.io/pypi/v/llama-cpp-agent?logo=pypi&color=%2341bb13)](https://pypi.org/project/llama-cpp-agent/)
-[![Discord](https://img.shields.io/discord/1237393014154985582?logo=Discord&logoColor=%23ffffff&label=Discord&link=https%3A%2F%2Fdiscord.gg%2FsRMvWKrh)](https://discord.gg/sRMvWKrh)
-
-<img src="./logo/logo_orange.png" alt="llama-cpp-agent logo" width="280"/>
-
-## Introduction
-The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
-
-The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
-
-The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
-
-## Key Features
-- **Simple Chat Interface**: Engage in seamless conversations with LLMs.
-- **Structured Output**: Generate structured output (objects) from LLMs.
-- **Single and Parallel Function Calling**: Execute functions using LLMs.
-- **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
-- **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
-- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
-- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
-- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
-- **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
-
-
-## Table of Contents
-- [Introduction](#introduction)
-- [Key Features](#key-features)
-- [Installation](#installation)
-- [Documentation](#documentation)
-- [Getting Started](#getting-started)
-- [Discord Community](#discord-community)
-- [Usage Examples](#usage-examples)
-    - [Simple Chat](#simple-chat-example-using-llamacpp-server-backend)
-    - [Parallel Function Calling](#parallel-function-calling-agent-example)
-    - [Structured Output](#structured-output)
-    - [RAG - Retrieval Augmented Generation](#rag---retrieval-augmented-generation)
-    - [llama-index Tools](#llama-index-tools-example)
-    - [Sequential Chain](#sequential-chain-example)
-    - [Mapping Chain](#mapping-chain-example)
-    - [Knowledge Graph Creation](#knowledge-graph-creation-example)
-- [Additional Information](#additional-information)
-    - [Predefined Messages Formatter](#predefined-messages-formatter)
-    - [Creating Custom Messages Formatter](#creating-custom-messages-formatter)
-- [Contributing](#contributing)
-- [License](#license)
-- [FAQ](#faq)
-
-
-
-## Installation
-Install the llama-cpp-agent framework using pip:
-```shell
-pip install llama-cpp-agent
-```
-## Documentation
-You can find the latest documentation [here!](https://llama-cpp-agent.readthedocs.io/en/latest/)
-
-## Getting Started
-You can find the get started guide [here!](https://llama-cpp-agent.readthedocs.io/en/latest/get-started/)
-
-## Discord Community
-Join the Discord Community [here](https://discord.gg/6tGznupZGX)
-
-## Usage Examples
-The llama-cpp-agent framework provides a wide range of examples demonstrating its capabilities. Here are some key examples:
-
-### Simple Chat Example using llama.cpp server backend
-This example demonstrates how to initiate a chat with an LLM model using the llama.cpp server backend. It supports llama-cpp-python Llama class instances, OpenAI endpoints with GBNF grammar support, and the llama.cpp backend server.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/simple-chat-example/)
-
-### Parallel Function Calling Agent Example
-This example showcases parallel function calling using the FunctionCallingAgent class. It demonstrates how to define and execute multiple functions concurrently.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/parallel_function_calling/)
-
-### Structured Output
-This example illustrates how to generate structured output objects using the StructuredOutputAgent class. It shows how to create a dataset entry of a book from unstructured data.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/structured-output-example/)
-
-### RAG - Retrieval Augmented Generation
-This example demonstrates Retrieval Augmented Generation (RAG) with colbert reranking. It requires installing the optional rag dependencies (ragatouille).
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/rag/)
-
-### llama-index Tools Example
-This example shows how to use llama-index tools and query engines with the FunctionCallingAgent class.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/llama_index_tool_use/)
-
-### Sequential Chain Example
-This example demonstrates how to create a complete product launch campaign using a sequential chain.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/sequential_chain/)
-
-### Mapping Chain Example
-This example illustrates how to create a mapping chain to summarize multiple articles into a single summary.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/map_chain/)
-
-### Knowledge Graph Creation Example
-This example, based on an example from the Instructor library for OpenAI, shows how to create a knowledge graph using the llama-cpp-agent framework.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/knowledge-graph-example/)
-
-
-## Additional Information
-
-### Predefined Messages Formatter
-
-The llama-cpp-agent framework provides predefined message formatters to format messages for the LLM model. The `MessagesFormatterType` enum defines the available formatters:
-
-- `MessagesFormatterType.MISTRAL`: Formats messages using the MISTRAL format.
-- `MessagesFormatterType.CHATML`: Formats messages using the CHATML format.
-- `MessagesFormatterType.VICUNA`: Formats messages using the VICUNA format.
-- `MessagesFormatterType.LLAMA_2`: Formats messages using the LLAMA 2 format.
-- `MessagesFormatterType.SYNTHIA`: Formats messages using the SYNTHIA format.
-- `MessagesFormatterType.NEURAL_CHAT`: Formats messages using the NEURAL CHAT format.
-- `MessagesFormatterType.SOLAR`: Formats messages using the SOLAR format.
-- `MessagesFormatterType.OPEN_CHAT`: Formats messages using the OPEN CHAT format.
-- `MessagesFormatterType.ALPACA`: Formats messages using the ALPACA format.
-- `MessagesFormatterType.CODE_DS`: Formats messages using the CODE DS format.
-- `MessagesFormatterType.B22`: Formats messages using the B22 format.
-- `MessagesFormatterType.LLAMA_3`: Formats messages using the LLAMA 3 format.
-- `MessagesFormatterType.PHI_3`: Formats messages using the PHI 3 format.
-
-### Creating Custom Messages Formatter
-
-You can create your own custom messages formatter by instantiating the `MessagesFormatter` class with the desired parameters:
-
-```python
-from llama_cpp_agent.chat_history.messages_formatter import MessagesFormatter, PromptMarkers, Roles
-
-custom_prompt_markers = {
-    Roles.system: PromptMarkers("<|system|>", "<|endsystem|>"),
-    Roles.user: PromptMarkers("<|user|>", "<|enduser|>"),
-    Roles.assistant: PromptMarkers("<|assistant|>", "<|endassistant|>"),
-    Roles.tool: PromptMarkers("<|tool|>", "<|endtool|>"),
-}
-
-custom_formatter = MessagesFormatter(
-    pre_prompt="",
-    prompt_markers=custom_prompt_markers,
-    include_sys_prompt_in_first_user_message=False,
-    default_stop_sequences=["<|endsystem|>", "<|enduser|>", "<|endassistant|>", "<|endtool|>"]
-)
-```
-
-## Contributing
-We welcome contributions to the llama-cpp-agent framework! If you'd like to contribute, please follow these guidelines:
-
-1. Fork the repository and create your branch from `master`.
-2. Ensure your code follows the project's coding style and conventions.
-3. Write clear, concise commit messages and pull request descriptions.
-4. Test your changes thoroughly before submitting a pull request.
-5. Open a pull request to the `master` branch.
-
-If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/Maximilian-Winter/llama-cpp-agent/issues).
-
-## License
-The llama-cpp-agent framework is released under the [MIT License](https://github.com/Maximilian-Winter/llama-cpp-agent/blob/master/LICENSE).
-
-## FAQ
-
-**Q: How do I install the optional dependencies for RAG?**  
-A: To use the RAGColbertReranker class and the RAG example, you need to install the optional rag dependencies (ragatouille). You can do this by running `pip install llama-cpp-agent[rag]`.
-
-**Q: Can I contribute to the llama-cpp-agent project?**  
-A: Absolutely! We welcome contributions from the community. Please refer to the [Contributing](#contributing) section for guidelines on how to contribute.
-
-**Q: Is llama-cpp-agent compatible with the latest version of llama-cpp-python?**  
-A: Yes, llama-cpp-agent is designed to work with the latest version of llama-cpp-python. However, if you encounter any compatibility issues, please open an issue on the GitHub repository.
+# llama-cpp-agent
+
+[![PyPI - Version](https://img.shields.io/pypi/v/llama-cpp-agent?logo=pypi&color=%2341bb13)](https://pypi.org/project/llama-cpp-agent/)
+[![Discord](https://img.shields.io/discord/1237393014154985582?logo=Discord&logoColor=%23ffffff&label=Discord&link=https%3A%2F%2Fdiscord.gg%2FsRMvWKrh)](https://discord.gg/sRMvWKrh)
+
+![llama-cpp-agent logo](https://github.com/Maximilian-Winter/llama-cpp-agent/blob/ed6b0973c15cf653d406e53dd6b4efc8d97796cb/logo/logo_orange.png)
+
+## Introduction
+The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
+
+The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
+
+The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
+
+## Key Features
+- **Simple Chat Interface**: Engage in seamless conversations with LLMs.
+- **Structured Output**: Generate structured output (objects) from LLMs.
+- **Single and Parallel Function Calling**: Execute functions using LLMs.
+- **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
+- **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
+- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
+- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
+- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
+- **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
+
+
+## Table of Contents
+- [Introduction](#introduction)
+- [Key Features](#key-features)
+- [Installation](#installation)
+- [Documentation](#documentation)
+- [Getting Started](#getting-started)
+- [Discord Community](#discord-community)
+- [Usage Examples](#usage-examples)
+    - [Simple Chat](#simple-chat-example-using-llamacpp-server-backend)
+    - [Parallel Function Calling](#parallel-function-calling-agent-example)
+    - [Structured Output](#structured-output)
+    - [RAG - Retrieval Augmented Generation](#rag---retrieval-augmented-generation)
+    - [llama-index Tools](#llama-index-tools-example)
+    - [Sequential Chain](#sequential-chain-example)
+    - [Mapping Chain](#mapping-chain-example)
+    - [Knowledge Graph Creation](#knowledge-graph-creation-example)
+- [Additional Information](#additional-information)
+    - [Predefined Messages Formatter](#predefined-messages-formatter)
+    - [Creating Custom Messages Formatter](#creating-custom-messages-formatter)
+- [Contributing](#contributing)
+- [License](#license)
+- [FAQ](#faq)
+
+
+
+## Installation
+Install the llama-cpp-agent framework using pip:
+```shell
+pip install llama-cpp-agent
+```
+## Documentation
+You can find the latest documentation [here!](https://llama-cpp-agent.readthedocs.io/en/latest/)
+
+## Getting Started
+You can find the get started guide [here!](https://llama-cpp-agent.readthedocs.io/en/latest/get-started/)
+
+## Discord Community
+Join the Discord Community [here](https://discord.gg/6tGznupZGX)
+
+## Usage Examples
+The llama-cpp-agent framework provides a wide range of examples demonstrating its capabilities. Here are some key examples:
+
+### Simple Chat Example using llama.cpp server backend
+This example demonstrates how to initiate a chat with an LLM model using the llama.cpp server backend. It supports llama-cpp-python Llama class instances, OpenAI endpoints with GBNF grammar support, and the llama.cpp backend server.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/simple-chat-example/)
+
+### Parallel Function Calling Agent Example
+This example showcases parallel function calling using the FunctionCallingAgent class. It demonstrates how to define and execute multiple functions concurrently.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/parallel_function_calling/)
+
+### Structured Output
+This example illustrates how to generate structured output objects using the StructuredOutputAgent class. It shows how to create a dataset entry of a book from unstructured data.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/structured-output-example/)
+
+### RAG - Retrieval Augmented Generation
+This example demonstrates Retrieval Augmented Generation (RAG) with colbert reranking. It requires installing the optional rag dependencies (ragatouille).
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/rag/)
+
+### llama-index Tools Example
+This example shows how to use llama-index tools and query engines with the FunctionCallingAgent class.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/llama_index_tool_use/)
+
+### Sequential Chain Example
+This example demonstrates how to create a complete product launch campaign using a sequential chain.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/sequential_chain/)
+
+### Mapping Chain Example
+This example illustrates how to create a mapping chain to summarize multiple articles into a single summary.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/map_chain/)
+
+### Knowledge Graph Creation Example
+This example, based on an example from the Instructor library for OpenAI, shows how to create a knowledge graph using the llama-cpp-agent framework.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/knowledge-graph-example/)
+
+
+## Additional Information
+
+### Predefined Messages Formatter
+
+The llama-cpp-agent framework provides predefined message formatters to format messages for the LLM model. The `MessagesFormatterType` enum defines the available formatters:
+
+- `MessagesFormatterType.MISTRAL`: Formats messages using the MISTRAL format.
+- `MessagesFormatterType.CHATML`: Formats messages using the CHATML format.
+- `MessagesFormatterType.VICUNA`: Formats messages using the VICUNA format.
+- `MessagesFormatterType.LLAMA_2`: Formats messages using the LLAMA 2 format.
+- `MessagesFormatterType.SYNTHIA`: Formats messages using the SYNTHIA format.
+- `MessagesFormatterType.NEURAL_CHAT`: Formats messages using the NEURAL CHAT format.
+- `MessagesFormatterType.SOLAR`: Formats messages using the SOLAR format.
+- `MessagesFormatterType.OPEN_CHAT`: Formats messages using the OPEN CHAT format.
+- `MessagesFormatterType.ALPACA`: Formats messages using the ALPACA format.
+- `MessagesFormatterType.CODE_DS`: Formats messages using the CODE DS format.
+- `MessagesFormatterType.B22`: Formats messages using the B22 format.
+- `MessagesFormatterType.LLAMA_3`: Formats messages using the LLAMA 3 format.
+- `MessagesFormatterType.PHI_3`: Formats messages using the PHI 3 format.
+
+### Creating Custom Messages Formatter
+
+You can create your own custom messages formatter by instantiating the `MessagesFormatter` class with the desired parameters:
+
+```python
+from llama_cpp_agent.messages_formatter import MessagesFormatter, PromptMarkers, Roles
+
+custom_prompt_markers = {
+    Roles.system: PromptMarkers("<|system|>", "<|endsystem|>"),
+    Roles.user: PromptMarkers("<|user|>", "<|enduser|>"),
+    Roles.assistant: PromptMarkers("<|assistant|>", "<|endassistant|>"),
+    Roles.tool: PromptMarkers("<|tool|>", "<|endtool|>"),
+}
+
+custom_formatter = MessagesFormatter(
+    pre_prompt="",
+    prompt_markers=custom_prompt_markers,
+    include_sys_prompt_in_first_user_message=False,
+    default_stop_sequences=["<|endsystem|>", "<|enduser|>", "<|endassistant|>", "<|endtool|>"]
+)
+```
+
+## Contributing
+We welcome contributions to the llama-cpp-agent framework! If you'd like to contribute, please follow these guidelines:
+
+1. Fork the repository and create your branch from `master`.
+2. Ensure your code follows the project's coding style and conventions.
+3. Write clear, concise commit messages and pull request descriptions.
+4. Test your changes thoroughly before submitting a pull request.
+5. Open a pull request to the `master` branch.
+
+If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/Maximilian-Winter/llama-cpp-agent/issues).
+
+## License
+The llama-cpp-agent framework is released under the [MIT License](https://github.com/Maximilian-Winter/llama-cpp-agent/blob/master/LICENSE).
+
+## FAQ
+
+**Q: How do I install the optional dependencies for RAG?**  
+A: To use the RAGColbertReranker class and the RAG example, you need to install the optional rag dependencies (ragatouille). You can do this by running `pip install llama-cpp-agent[rag]`.
+
+**Q: Can I contribute to the llama-cpp-agent project?**  
+A: Absolutely! We welcome contributions from the community. Please refer to the [Contributing](#contributing) section for guidelines on how to contribute.
+
+**Q: Is llama-cpp-agent compatible with the latest version of llama-cpp-python?**  
+A: Yes, llama-cpp-agent is designed to work with the latest version of llama-cpp-python. However, if you encounter any compatibility issues, please open an issue on the GitHub repository.
```

### Comparing `llama_cpp_agent-0.2.3/pyproject.toml` & `llama_cpp_agent-0.2.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-[build-system]
-requires = [  "setuptools>=42"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "llama-cpp-agent"
-version = "0.2.3"
-description = "A framework for building LLM based AI agents with llama.cpp."
-
-readme = "ReadMe.md"
-dependencies = [
-    "llama-cpp-python>=0.2.60",
-    "pydantic>=2.5.3",
-    "requests>=2.31.0",
-    "docstring_parser",
-    "aiohttp"
-]
-
-requires-python = ">=3.10"
-classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent" ]
-[[project.authors]]
-name = "Maximilian Winter"
-email = "maximilian.winter.91@gmail.com"
-
-
-[project.optional-dependencies]
-agent_memory = ["chromadb", "SQLAlchemy", "numpy", "scipy"]
-rag = ["ragatouille"]
-vllm_provider = ["openai"]
-mixtral_agent = ["mistral-common"]
-
-[project.urls]
-Homepage = "https://github.com/Maximilian-Winter/llama-cpp-agent"
-"Bug Tracker" = "https://github.com/Maximilian-Winter/llama-cpp-agent/issues"
-
-[tool.setuptools.packages.find]
-where = ["src"]
-
+[build-system]
+requires = [  "setuptools>=42"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "llama-cpp-agent"
+version = "0.2.4"
+description = "A framework for building LLM based AI agents with llama.cpp."
+
+readme = "ReadMe.md"
+dependencies = [
+    "llama-cpp-python>=0.2.60",
+    "pydantic>=2.5.3",
+    "requests>=2.31.0",
+    "docstring_parser",
+    "aiohttp"
+]
+
+requires-python = ">=3.10"
+classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent" ]
+[[project.authors]]
+name = "Maximilian Winter"
+email = "maximilian.winter.91@gmail.com"
+
+
+[project.optional-dependencies]
+agent_memory = ["chromadb", "SQLAlchemy", "numpy", "scipy"]
+rag = ["ragatouille"]
+vllm_provider = ["openai"]
+mixtral_agent = ["mistral-common"]
+
+[project.urls]
+Homepage = "https://github.com/Maximilian-Winter/llama-cpp-agent"
+"Bug Tracker" = "https://github.com/Maximilian-Winter/llama-cpp-agent/issues"
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/core_memory_manager.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/agent_memory/core_memory_manager.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import datetime
-import json
-
-
-class CoreMemoryManager:
-    def __init__(self, core_memory: dict):
-        self.core_memory = core_memory
-        self.last_modified = "Never"
-
-    def add_to_core_memory(self, key: str, child_key: str, value) -> str:
-        """
-        Adds or updates an entry in the IAM.
-        """
-        if key not in self.core_memory:
-            self.core_memory[key] = {}
-        self.core_memory[key][child_key] = value
-        self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
-        return f"Core memory updated. Key: {key}, Child Key: {child_key}"
-
-    def replace_in_core_memory(self, key: str, child_key: str, new_value) -> str:
-        """
-        Replaces an existing entry in the IAM.
-        """
-        if key in self.core_memory and child_key in self.core_memory[key]:
-            self.core_memory[key][child_key] = new_value
-            self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
-            return f"Core memory replaced. Key: {key}, Child Key: {child_key}"
-        else:
-            return "Key or child key not found in Core memory."
-
-    def remove_from_core_memory(self, key: str, child_key: str) -> str:
-        """
-        Removes a specific field from a IAM entry.
-        """
-        if key in self.core_memory and child_key in self.core_memory[key]:
-            del self.core_memory[key][child_key]
-            self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
-            return f"Core memory entry removed. Key: {key}, Child Key: {child_key}"
-        else:
-            return "Key or child key not found in Core memory."
-
-    def build_core_memory_context(self):
-        context = ""
-        # for key, item in self.core_memory.items():
-        #     context += f"""#### {key} ####\n"""
-        #     for key2, item2 in item.items():
-        #         context += f"""{key2}:\n{self.format_multiline_description(item2.strip(), 0)}\n\n"""
-        #     if item == {}:
-        #         context += "Empty Section\n"
-        # context = json.dumps(self.core_memory, indent=2)
-        for key, item in self.core_memory.items():
-            context += f"""<{key}>\n"""
-            for key2, item2 in item.items():
-                context += f"""  <{key2}>\n{self.format_multiline_description(item2.strip(), 1)}\n  </{key2}>\n"""
-            context += f"</{key}>\n"
-        if context == "":
-            context = "No Core Memories!"
-        return context
-
-    def format_multiline_description(self, description: str, indent_level: int) -> str:
-        """
-        Format a multiline description with proper indentation.
-
-        Args:
-            description (str): Multiline description.
-            indent_level (int): Indentation level.
-
-        Returns:
-            str: Formatted multiline description.
-        """
-        indent = "    " * indent_level
-        return indent + description.replace("\n", "\n" + indent)
-
-    def load(self, file_path):
-        with open(file_path, "r", encoding="utf-8") as file:
-            self.core_memory = json.load(file)
-        self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
-
-    def save(self, filepath):
-        with open(filepath, "w", encoding="utf-8") as file:
-            json.dump(self.core_memory, file, indent=4)
+import datetime
+import json
+
+
+class CoreMemoryManager:
+    def __init__(self, core_memory: dict):
+        self.core_memory = core_memory
+        self.last_modified = "Never"
+
+    def add_to_core_memory(self, key: str, child_key: str, value) -> str:
+        """
+        Adds or updates an entry in the IAM.
+        """
+        if key not in self.core_memory:
+            self.core_memory[key] = {}
+        self.core_memory[key][child_key] = value
+        self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
+        return f"Core memory updated. Key: {key}, Child Key: {child_key}"
+
+    def replace_in_core_memory(self, key: str, child_key: str, new_value) -> str:
+        """
+        Replaces an existing entry in the IAM.
+        """
+        if key in self.core_memory and child_key in self.core_memory[key]:
+            self.core_memory[key][child_key] = new_value
+            self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
+            return f"Core memory replaced. Key: {key}, Child Key: {child_key}"
+        else:
+            return "Key or child key not found in Core memory."
+
+    def remove_from_core_memory(self, key: str, child_key: str) -> str:
+        """
+        Removes a specific field from a IAM entry.
+        """
+        if key in self.core_memory and child_key in self.core_memory[key]:
+            del self.core_memory[key][child_key]
+            self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
+            return f"Core memory entry removed. Key: {key}, Child Key: {child_key}"
+        else:
+            return "Key or child key not found in Core memory."
+
+    def build_core_memory_context(self):
+        context = ""
+        # for key, item in self.core_memory.items():
+        #     context += f"""#### {key} ####\n"""
+        #     for key2, item2 in item.items():
+        #         context += f"""{key2}:\n{self.format_multiline_description(item2.strip(), 0)}\n\n"""
+        #     if item == {}:
+        #         context += "Empty Section\n"
+        # context = json.dumps(self.core_memory, indent=2)
+        for key, item in self.core_memory.items():
+            context += f"""<{key}>\n"""
+            for key2, item2 in item.items():
+                context += f"""  <{key2}>\n{self.format_multiline_description(item2.strip(), 1)}\n  </{key2}>\n"""
+            context += f"</{key}>\n"
+        if context == "":
+            context = "No Core Memories!"
+        return context
+
+    def format_multiline_description(self, description: str, indent_level: int) -> str:
+        """
+        Format a multiline description with proper indentation.
+
+        Args:
+            description (str): Multiline description.
+            indent_level (int): Indentation level.
+
+        Returns:
+            str: Formatted multiline description.
+        """
+        indent = "    " * indent_level
+        return indent + description.replace("\n", "\n" + indent)
+
+    def load(self, file_path):
+        with open(file_path, "r", encoding="utf-8") as file:
+            self.core_memory = json.load(file)
+        self.last_modified = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
+
+    def save(self, filepath):
+        with open(filepath, "w", encoding="utf-8") as file:
+            json.dump(self.core_memory, file, indent=4)
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/memory_tools.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/agent_memory/memory_tools.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,287 +1,287 @@
-from datetime import datetime
-from enum import Enum
-from typing import List, Optional
-
-from pydantic import BaseModel, Field
-from sqlalchemy import create_engine
-from sqlalchemy.orm import sessionmaker, scoped_session
-
-from .event_memory import EventType, Base
-from .event_memory_manager import EventMemoryManager
-from ..function_calling import LlamaCppFunctionTool
-from .core_memory_manager import CoreMemoryManager
-from .retrieval_memory_manager import RetrievalMemoryManager, RetrievalMemory
-
-
-class CoreMemoryKey(Enum):
-    PERSONA: str = "persona"
-    HUMAN: str = "human"
-
-
-class core_memory_append(BaseModel):
-    """
-    Append a new entry to the Core Memory.
-    """
-
-    key: str = Field(..., description="The key identifier of the core memory.")
-    field: str = Field(..., description="The field within the core memory.")
-    value: str = Field(
-        ...,
-        description="The value or data to be stored in the specified core memory entry.",
-    )
-
-    def run(self, core_memory_manager: CoreMemoryManager):
-        return core_memory_manager.add_to_core_memory(
-            self.key.value, self.field, self.value
-        )
-
-
-class core_memory_replace(BaseModel):
-    """
-    Replace an entry in the Core Memory.
-    """
-
-    key: str = Field(..., description="The key identifier of the core memory.")
-    field: str = Field(..., description="The field within the core memory.")
-    new_value: str = Field(
-        ...,
-        description="The new value to replace with the existing data in the specified Core Memory field.",
-    )
-
-    def run(self, core_memory_manager: CoreMemoryManager):
-        return core_memory_manager.replace_in_core_memory(
-            self.key.value, self.field, self.new_value
-        )
-
-
-class core_memory_remove(BaseModel):
-    """
-    Remove an entry from the Core Memory.
-    """
-
-    key: str = Field(..., description="The key identifier of the core memory.")
-    field: str = Field(..., description="The field within the core memory.")
-
-    def run(self, core_memory_manager: CoreMemoryManager):
-        return core_memory_manager.remove_from_core_memory(self.key.value, self.field)
-
-
-class conversation_search(BaseModel):
-    """
-    Search prior conversation history using case-insensitive string matching.
-    """
-
-    keywords: List[str] = Field(
-        ...,
-        description='Keywords that the messages have to contain. Eg. ["hello", "world"]',
-    )
-    page: Optional[int] = Field(
-        ...,
-        description="Allows you to page through results. Only use on a follow-up query. Defaults to 0 (first page).",
-    )
-
-    def run(self, event_memory_manager: EventMemoryManager):
-        parsed_start_datetime = None
-        parsed_end_datetime = None
-        if self.page is None:
-            self.page = 0
-        return event_memory_manager.query_events(
-            event_types=[
-                EventType.UserMessage,
-                EventType.AgentMessage,
-                EventType.SystemMessage,
-                EventType.FunctionMessage,
-            ],
-            content_keywords=self.keywords,
-            start_date=parsed_start_datetime,
-            end_date=parsed_end_datetime,
-            page=self.page,
-        )
-
-
-class conversation_search_date(BaseModel):
-    """
-    Search prior conversation history using a date range.
-    """
-
-    start_date: str = Field(
-        ...,
-        description='The start of the date range to search, in the format "dd/mm/YYYY, H:M:S" eg. "01/01/2024, 08:00:30"',
-    )
-    end_date: str = Field(
-        ...,
-        description='The end of the date range to search, in the format "dd/mm/YYYY, H:M:S" eg. "04/02/2024, 18:57:29"',
-    )
-    page: Optional[int] = Field(
-        ...,
-        description="Allows you to page through results. Only use on a follow-up query. Defaults to 0 (first page).",
-    )
-
-    def run(self, event_memory_manager: EventMemoryManager):
-        parsed_start_datetime = None
-        parsed_end_datetime = None
-        if self.start_date:
-            parsed_start_datetime = datetime.strptime(
-                self.start_date, "%d/%m/%Y, %H:%M:%S"
-            )
-        if self.end_date:
-            parsed_end_datetime = datetime.strptime(self.end_date, "%d/%m/%Y, %H:%M:%S")
-        if self.page is None:
-            self.page = 0
-
-        return event_memory_manager.query_events(
-            event_types=[
-                EventType.UserMessage,
-                EventType.AgentMessage,
-                EventType.SystemMessage,
-                EventType.FunctionMessage,
-            ],
-            start_date=parsed_start_datetime,
-            end_date=parsed_end_datetime,
-            page=self.page,
-        )
-
-
-class archival_memory_search(BaseModel):
-    """
-    Search archival memory using semantic (embedding-based) search.
-    """
-
-    query: str = Field(
-        ...,
-        description="String to search for. The search will return the most semantically similar memories to this query.",
-    )
-    page: Optional[int] = Field(
-        ...,
-        description="Allows you to page through results. Only use on a follow-up query. Defaults to 0 (first page).",
-    )
-
-    def run(self, retrieval_memory_manager: RetrievalMemoryManager):
-        return retrieval_memory_manager.retrieve_memories(self.query)
-
-
-class archival_memory_insert(BaseModel):
-    """
-    Add to archival memory. Make sure to phrase the memory contents such that it can be easily queried later.
-    """
-
-    memory: str = Field(
-        ...,
-        description="Content to write to the memory. All unicode (including emojis) are supported.",
-    )
-    importance: float = Field(
-        ...,
-        description="A value from 1.0 to 10.0 indicating the importance of the memory.",
-    )
-
-    def run(self, retrieval_memory_manager: RetrievalMemoryManager):
-        return retrieval_memory_manager.add_memory_to_retrieval(
-            self.memory, self.importance
-        )
-
-
-class AgentRetrievalMemory:
-    def __init__(
-        self,
-        persistent_db_path="./retrieval_memory",
-        embedding_model_name="all-MiniLM-L6-v2",
-        collection_name="retrieval_memory_collection",
-    ):
-        self.retrieval_memory = RetrievalMemory(
-            persistent_db_path, embedding_model_name, collection_name
-        )
-        self.retrieval_memory_manager = RetrievalMemoryManager(self.retrieval_memory)
-        self.retrieve_memories_tool = LlamaCppFunctionTool(
-            archival_memory_search,
-            retrieval_memory_manager=self.retrieval_memory_manager,
-        )
-        self.add_retrieval_memory_tool = LlamaCppFunctionTool(
-            archival_memory_insert,
-            retrieval_memory_manager=self.retrieval_memory_manager,
-        )
-
-    def get_tool_list(self):
-        return [self.retrieve_memories_tool, self.add_retrieval_memory_tool]
-
-    def get_retrieve_memories_tool(self):
-        return self.retrieve_memories_tool
-
-    def get_add_retrieval_memory_tool(self):
-        return self.add_retrieval_memory_tool
-
-
-class AgentCoreMemory:
-    def __init__(self, core_memory=None, core_memory_file=None):
-        if core_memory is None:
-            core_memory = {}
-
-        self.core_memory_manager = CoreMemoryManager(core_memory)
-        if core_memory_file is not None:
-            self.core_memory_manager.load(core_memory_file)
-
-        self.add_core_memory_tool = LlamaCppFunctionTool(
-            core_memory_append, core_memory_manager=self.core_memory_manager
-        )
-        self.remove_core_memory_tool = LlamaCppFunctionTool(
-            core_memory_remove, core_memory_manager=self.core_memory_manager
-        )
-        self.replace_core_memory_tool = LlamaCppFunctionTool(
-            core_memory_replace, core_memory_manager=self.core_memory_manager
-        )
-
-    def get_core_memory_manager(self):
-        return self.core_memory_manager
-
-    def get_tool_list(self):
-        return [
-            self.add_core_memory_tool,
-            self.remove_core_memory_tool,
-            self.replace_core_memory_tool,
-        ]
-
-    def get_add_core_memory_tool(self):
-        return self.add_core_memory_tool
-
-    def get_remove_core_memory_tool(self):
-        return self.remove_core_memory_tool
-
-    def get_replace_core_memory_tool(self):
-        return self.replace_core_memory_tool
-
-    def save_core_memory(self, file_path):
-        self.core_memory_manager.save(file_path)
-
-    def load_core_memory(self, file_path):
-        self.core_memory_manager.load(file_path)
-
-
-class AgentEventMemory:
-    def __init__(self, event_queue_file=None, db_path="sqlite:///events.db"):
-        self.engine = create_engine(db_path)
-        session_factory = sessionmaker(bind=self.engine)
-        Base.metadata.create_all(self.engine)
-        self.Session = scoped_session(session_factory)
-        self.session = self.Session()
-        self.event_memory_manager = EventMemoryManager(self.session)
-
-        if event_queue_file is not None:
-            self.event_memory_manager.load_event_queue(event_queue_file)
-        self.search_event_memory_manager_tool = LlamaCppFunctionTool(
-            conversation_search, event_memory_manager=self.event_memory_manager
-        )
-
-        self.search_event_memory_manager_tool_date = LlamaCppFunctionTool(
-            conversation_search_date, event_memory_manager=self.event_memory_manager
-        )
-
-    def get_event_memory_manager(self):
-        return self.event_memory_manager
-
-    def get_tool_list(self):
-        return [
-            self.search_event_memory_manager_tool,
-            self.search_event_memory_manager_tool_date,
-        ]
-
-    def get_search_event_memory_manager_tool(self):
-        return self.search_event_memory_manager_tool
+from datetime import datetime
+from enum import Enum
+from typing import List, Optional
+
+from pydantic import BaseModel, Field
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker, scoped_session
+
+from .event_memory import EventType, Base
+from .event_memory_manager import EventMemoryManager
+from ..function_calling import LlamaCppFunctionTool
+from .core_memory_manager import CoreMemoryManager
+from .retrieval_memory_manager import RetrievalMemoryManager, RetrievalMemory
+
+
+class CoreMemoryKey(Enum):
+    PERSONA: str = "persona"
+    HUMAN: str = "human"
+
+
+class core_memory_append(BaseModel):
+    """
+    Append a new entry to the Core Memory.
+    """
+
+    key: str = Field(..., description="The key identifier of the core memory.")
+    field: str = Field(..., description="The field within the core memory.")
+    value: str = Field(
+        ...,
+        description="The value or data to be stored in the specified core memory entry.",
+    )
+
+    def run(self, core_memory_manager: CoreMemoryManager):
+        return core_memory_manager.add_to_core_memory(
+            self.key.value, self.field, self.value
+        )
+
+
+class core_memory_replace(BaseModel):
+    """
+    Replace an entry in the Core Memory.
+    """
+
+    key: str = Field(..., description="The key identifier of the core memory.")
+    field: str = Field(..., description="The field within the core memory.")
+    new_value: str = Field(
+        ...,
+        description="The new value to replace with the existing data in the specified Core Memory field.",
+    )
+
+    def run(self, core_memory_manager: CoreMemoryManager):
+        return core_memory_manager.replace_in_core_memory(
+            self.key.value, self.field, self.new_value
+        )
+
+
+class core_memory_remove(BaseModel):
+    """
+    Remove an entry from the Core Memory.
+    """
+
+    key: str = Field(..., description="The key identifier of the core memory.")
+    field: str = Field(..., description="The field within the core memory.")
+
+    def run(self, core_memory_manager: CoreMemoryManager):
+        return core_memory_manager.remove_from_core_memory(self.key.value, self.field)
+
+
+class conversation_search(BaseModel):
+    """
+    Search prior conversation history using case-insensitive string matching.
+    """
+
+    keywords: List[str] = Field(
+        ...,
+        description='Keywords that the messages have to contain. Eg. ["hello", "world"]',
+    )
+    page: Optional[int] = Field(
+        ...,
+        description="Allows you to page through results. Only use on a follow-up query. Defaults to 0 (first page).",
+    )
+
+    def run(self, event_memory_manager: EventMemoryManager):
+        parsed_start_datetime = None
+        parsed_end_datetime = None
+        if self.page is None:
+            self.page = 0
+        return event_memory_manager.query_events(
+            event_types=[
+                EventType.UserMessage,
+                EventType.AgentMessage,
+                EventType.SystemMessage,
+                EventType.FunctionMessage,
+            ],
+            content_keywords=self.keywords,
+            start_date=parsed_start_datetime,
+            end_date=parsed_end_datetime,
+            page=self.page,
+        )
+
+
+class conversation_search_date(BaseModel):
+    """
+    Search prior conversation history using a date range.
+    """
+
+    start_date: str = Field(
+        ...,
+        description='The start of the date range to search, in the format "dd/mm/YYYY, H:M:S" eg. "01/01/2024, 08:00:30"',
+    )
+    end_date: str = Field(
+        ...,
+        description='The end of the date range to search, in the format "dd/mm/YYYY, H:M:S" eg. "04/02/2024, 18:57:29"',
+    )
+    page: Optional[int] = Field(
+        ...,
+        description="Allows you to page through results. Only use on a follow-up query. Defaults to 0 (first page).",
+    )
+
+    def run(self, event_memory_manager: EventMemoryManager):
+        parsed_start_datetime = None
+        parsed_end_datetime = None
+        if self.start_date:
+            parsed_start_datetime = datetime.strptime(
+                self.start_date, "%d/%m/%Y, %H:%M:%S"
+            )
+        if self.end_date:
+            parsed_end_datetime = datetime.strptime(self.end_date, "%d/%m/%Y, %H:%M:%S")
+        if self.page is None:
+            self.page = 0
+
+        return event_memory_manager.query_events(
+            event_types=[
+                EventType.UserMessage,
+                EventType.AgentMessage,
+                EventType.SystemMessage,
+                EventType.FunctionMessage,
+            ],
+            start_date=parsed_start_datetime,
+            end_date=parsed_end_datetime,
+            page=self.page,
+        )
+
+
+class archival_memory_search(BaseModel):
+    """
+    Search archival memory using semantic (embedding-based) search.
+    """
+
+    query: str = Field(
+        ...,
+        description="String to search for. The search will return the most semantically similar memories to this query.",
+    )
+    page: Optional[int] = Field(
+        ...,
+        description="Allows you to page through results. Only use on a follow-up query. Defaults to 0 (first page).",
+    )
+
+    def run(self, retrieval_memory_manager: RetrievalMemoryManager):
+        return retrieval_memory_manager.retrieve_memories(self.query)
+
+
+class archival_memory_insert(BaseModel):
+    """
+    Add to archival memory. Make sure to phrase the memory contents such that it can be easily queried later.
+    """
+
+    memory: str = Field(
+        ...,
+        description="Content to write to the memory. All unicode (including emojis) are supported.",
+    )
+    importance: float = Field(
+        ...,
+        description="A value from 1.0 to 10.0 indicating the importance of the memory.",
+    )
+
+    def run(self, retrieval_memory_manager: RetrievalMemoryManager):
+        return retrieval_memory_manager.add_memory_to_retrieval(
+            self.memory, self.importance
+        )
+
+
+class AgentRetrievalMemory:
+    def __init__(
+        self,
+        persistent_db_path="./retrieval_memory",
+        embedding_model_name="all-MiniLM-L6-v2",
+        collection_name="retrieval_memory_collection",
+    ):
+        self.retrieval_memory = RetrievalMemory(
+            persistent_db_path, embedding_model_name, collection_name
+        )
+        self.retrieval_memory_manager = RetrievalMemoryManager(self.retrieval_memory)
+        self.retrieve_memories_tool = LlamaCppFunctionTool(
+            archival_memory_search,
+            retrieval_memory_manager=self.retrieval_memory_manager,
+        )
+        self.add_retrieval_memory_tool = LlamaCppFunctionTool(
+            archival_memory_insert,
+            retrieval_memory_manager=self.retrieval_memory_manager,
+        )
+
+    def get_tool_list(self):
+        return [self.retrieve_memories_tool, self.add_retrieval_memory_tool]
+
+    def get_retrieve_memories_tool(self):
+        return self.retrieve_memories_tool
+
+    def get_add_retrieval_memory_tool(self):
+        return self.add_retrieval_memory_tool
+
+
+class AgentCoreMemory:
+    def __init__(self, core_memory=None, core_memory_file=None):
+        if core_memory is None:
+            core_memory = {}
+
+        self.core_memory_manager = CoreMemoryManager(core_memory)
+        if core_memory_file is not None:
+            self.core_memory_manager.load(core_memory_file)
+
+        self.add_core_memory_tool = LlamaCppFunctionTool(
+            core_memory_append, core_memory_manager=self.core_memory_manager
+        )
+        self.remove_core_memory_tool = LlamaCppFunctionTool(
+            core_memory_remove, core_memory_manager=self.core_memory_manager
+        )
+        self.replace_core_memory_tool = LlamaCppFunctionTool(
+            core_memory_replace, core_memory_manager=self.core_memory_manager
+        )
+
+    def get_core_memory_manager(self):
+        return self.core_memory_manager
+
+    def get_tool_list(self):
+        return [
+            self.add_core_memory_tool,
+            self.remove_core_memory_tool,
+            self.replace_core_memory_tool,
+        ]
+
+    def get_add_core_memory_tool(self):
+        return self.add_core_memory_tool
+
+    def get_remove_core_memory_tool(self):
+        return self.remove_core_memory_tool
+
+    def get_replace_core_memory_tool(self):
+        return self.replace_core_memory_tool
+
+    def save_core_memory(self, file_path):
+        self.core_memory_manager.save(file_path)
+
+    def load_core_memory(self, file_path):
+        self.core_memory_manager.load(file_path)
+
+
+class AgentEventMemory:
+    def __init__(self, event_queue_file=None, db_path="sqlite:///events.db"):
+        self.engine = create_engine(db_path)
+        session_factory = sessionmaker(bind=self.engine)
+        Base.metadata.create_all(self.engine)
+        self.Session = scoped_session(session_factory)
+        self.session = self.Session()
+        self.event_memory_manager = EventMemoryManager(self.session)
+
+        if event_queue_file is not None:
+            self.event_memory_manager.load_event_queue(event_queue_file)
+        self.search_event_memory_manager_tool = LlamaCppFunctionTool(
+            conversation_search, event_memory_manager=self.event_memory_manager
+        )
+
+        self.search_event_memory_manager_tool_date = LlamaCppFunctionTool(
+            conversation_search_date, event_memory_manager=self.event_memory_manager
+        )
+
+    def get_event_memory_manager(self):
+        return self.event_memory_manager
+
+    def get_tool_list(self):
+        return [
+            self.search_event_memory_manager_tool,
+            self.search_event_memory_manager_tool_date,
+        ]
+
+    def get_search_event_memory_manager_tool(self):
+        return self.search_event_memory_manager_tool
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/retrieval_memory.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/agent_memory/retrieval_memory.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-import datetime
-import uuid
-
-import chromadb
-import numpy as np
-from chromadb.utils import embedding_functions
-from scipy.spatial.distance import cosine
-
-
-class RetrievalMemory:
-    def __init__(
-        self,
-        persistent_db_path="./retrieval_memory",
-        embedding_model_name="BAAI/bge-small-en-v1.5",
-        collection_name="retrieval_memory_collection",
-        decay_factor=0.99,
-    ):
-        self.client = chromadb.PersistentClient(path=persistent_db_path)
-        self.sentence_transformer_ef = (
-            embedding_functions.SentenceTransformerEmbeddingFunction(
-                model_name=embedding_model_name
-            )
-        )
-        self.collection = self.client.get_or_create_collection(
-            name=collection_name, embedding_function=self.sentence_transformer_ef
-        )
-        self.decay_factor = decay_factor
-
-    def add_memory(
-        self,
-        description: str,
-        date: datetime.datetime = datetime.datetime.now(),
-        importance: float = 1.0,
-    ):
-        """Add a memory with a given description and importance to the memory stream."""
-        mem = [description]
-        ids = [str(self.generate_unique_id())]
-        metadata = {
-            "memory_id": ids[0],
-            "memory": description,
-            "importance": importance,
-            "creation_timestamp": date.strftime("%Y-%m-%d %H:%M:%S"),
-            "last_access_timestamp": date.strftime("%Y-%m-%d %H:%M:%S"),
-        }
-        self.collection.add(documents=mem, metadatas=metadata, ids=ids)
-
-    def retrieve_memories(
-        self,
-        query: str,
-        k,
-        date=datetime.datetime.now(),
-        alpha_recency=1,
-        alpha_relevance=1,
-        alpha_importance=1,
-    ):
-        query_embedding = self.sentence_transformer_ef([query])
-        query_result = self.collection.query(
-            query_embedding,
-            n_results=k * 4,
-            include=["metadatas", "embeddings", "documents", "distances"],
-        )  # Increase candidate pool size
-        if len(query_result["metadatas"][0]) == 0:
-            return []
-        # Step 2: Apply scoring to the candidate memories
-        scores = []
-        for index in range(len(query_result["metadatas"][0])):
-            scores.append(
-                self.compute_memory_score(
-                    query_result["metadatas"][0][index],
-                    query_result["embeddings"][0][index],
-                    query_embedding,
-                    date,
-                    alpha_recency,
-                    alpha_relevance,
-                    alpha_importance,
-                )
-            )
-
-        # Normalize and select top k memories based on scores
-        normalized_scores = self.normalize_scores(np.array(scores))
-        top_indices = self.get_top_indices(normalized_scores, k)
-        retrieved_memories = [query_result["metadatas"][0][i] for i in top_indices]
-
-        # Update last access time
-        for memory in retrieved_memories:
-            memory = self.update_last_access(memory, date)
-            self.collection.upsert(
-                ids=memory["memory_id"], documents=[memory["memory"]], metadatas=memory
-            )
-        return retrieved_memories
-
-    @staticmethod
-    def generate_unique_id():
-        unique_id = str(uuid.uuid4())
-        return unique_id
-
-    def compute_memory_score(
-        self,
-        metadata,
-        memory_embedding,
-        query_embedding,
-        date,
-        alpha_recency,
-        alpha_relevance,
-        alpha_importance,
-    ):
-        recency = self.compute_recency(metadata, date)
-        relevance = self.compute_relevance(memory_embedding, query_embedding)
-        importance = metadata["importance"]
-        return (
-            alpha_recency * recency
-            + alpha_relevance * relevance
-            + alpha_importance * importance
-        )
-
-    @staticmethod
-    def update_last_access(metadata, date):
-        metadata["last_access_timestamp"] = date.strftime("%Y-%m-%d %H:%M:%S")
-        return metadata
-
-    def compute_recency(self, metadata, date):
-        decay_factor = self.decay_factor
-        time_diff = date - datetime.datetime.strptime(
-            metadata["last_access_timestamp"], "%Y-%m-%d %H:%M:%S"
-        )
-        hours_diff = time_diff.total_seconds() / 3600
-        recency = decay_factor**hours_diff
-        return recency
-
-    @staticmethod
-    def compute_relevance(memory_embedding, query_embedding):
-        relevance = 1 - cosine(memory_embedding, query_embedding[0])
-        return relevance
-
-    @staticmethod
-    def normalize_scores(scores):
-        min_score, max_score = np.min(scores), np.max(scores)
-        if min_score == max_score:
-            return np.zeros_like(scores)
-        return (scores - min_score) / (max_score - min_score)
-
-    @staticmethod
-    def get_top_indices(scores, k):
-        return scores.argsort()[-k:][::-1]
+import datetime
+import uuid
+
+import chromadb
+import numpy as np
+from chromadb.utils import embedding_functions
+from scipy.spatial.distance import cosine
+
+
+class RetrievalMemory:
+    def __init__(
+        self,
+        persistent_db_path="./retrieval_memory",
+        embedding_model_name="BAAI/bge-small-en-v1.5",
+        collection_name="retrieval_memory_collection",
+        decay_factor=0.99,
+    ):
+        self.client = chromadb.PersistentClient(path=persistent_db_path)
+        self.sentence_transformer_ef = (
+            embedding_functions.SentenceTransformerEmbeddingFunction(
+                model_name=embedding_model_name
+            )
+        )
+        self.collection = self.client.get_or_create_collection(
+            name=collection_name, embedding_function=self.sentence_transformer_ef
+        )
+        self.decay_factor = decay_factor
+
+    def add_memory(
+        self,
+        description: str,
+        date: datetime.datetime = datetime.datetime.now(),
+        importance: float = 1.0,
+    ):
+        """Add a memory with a given description and importance to the memory stream."""
+        mem = [description]
+        ids = [str(self.generate_unique_id())]
+        metadata = {
+            "memory_id": ids[0],
+            "memory": description,
+            "importance": importance,
+            "creation_timestamp": date.strftime("%Y-%m-%d %H:%M:%S"),
+            "last_access_timestamp": date.strftime("%Y-%m-%d %H:%M:%S"),
+        }
+        self.collection.add(documents=mem, metadatas=metadata, ids=ids)
+
+    def retrieve_memories(
+        self,
+        query: str,
+        k,
+        date=datetime.datetime.now(),
+        alpha_recency=1,
+        alpha_relevance=1,
+        alpha_importance=1,
+    ):
+        query_embedding = self.sentence_transformer_ef([query])
+        query_result = self.collection.query(
+            query_embedding,
+            n_results=k * 4,
+            include=["metadatas", "embeddings", "documents", "distances"],
+        )  # Increase candidate pool size
+        if len(query_result["metadatas"][0]) == 0:
+            return []
+        # Step 2: Apply scoring to the candidate memories
+        scores = []
+        for index in range(len(query_result["metadatas"][0])):
+            scores.append(
+                self.compute_memory_score(
+                    query_result["metadatas"][0][index],
+                    query_result["embeddings"][0][index],
+                    query_embedding,
+                    date,
+                    alpha_recency,
+                    alpha_relevance,
+                    alpha_importance,
+                )
+            )
+
+        # Normalize and select top k memories based on scores
+        normalized_scores = self.normalize_scores(np.array(scores))
+        top_indices = self.get_top_indices(normalized_scores, k)
+        retrieved_memories = [query_result["metadatas"][0][i] for i in top_indices]
+
+        # Update last access time
+        for memory in retrieved_memories:
+            memory = self.update_last_access(memory, date)
+            self.collection.upsert(
+                ids=memory["memory_id"], documents=[memory["memory"]], metadatas=memory
+            )
+        return retrieved_memories
+
+    @staticmethod
+    def generate_unique_id():
+        unique_id = str(uuid.uuid4())
+        return unique_id
+
+    def compute_memory_score(
+        self,
+        metadata,
+        memory_embedding,
+        query_embedding,
+        date,
+        alpha_recency,
+        alpha_relevance,
+        alpha_importance,
+    ):
+        recency = self.compute_recency(metadata, date)
+        relevance = self.compute_relevance(memory_embedding, query_embedding)
+        importance = metadata["importance"]
+        return (
+            alpha_recency * recency
+            + alpha_relevance * relevance
+            + alpha_importance * importance
+        )
+
+    @staticmethod
+    def update_last_access(metadata, date):
+        metadata["last_access_timestamp"] = date.strftime("%Y-%m-%d %H:%M:%S")
+        return metadata
+
+    def compute_recency(self, metadata, date):
+        decay_factor = self.decay_factor
+        time_diff = date - datetime.datetime.strptime(
+            metadata["last_access_timestamp"], "%Y-%m-%d %H:%M:%S"
+        )
+        hours_diff = time_diff.total_seconds() / 3600
+        recency = decay_factor**hours_diff
+        return recency
+
+    @staticmethod
+    def compute_relevance(memory_embedding, query_embedding):
+        relevance = 1 - cosine(memory_embedding, query_embedding[0])
+        return relevance
+
+    @staticmethod
+    def normalize_scores(scores):
+        min_score, max_score = np.min(scores), np.max(scores)
+        if min_score == max_score:
+            return np.zeros_like(scores)
+        return (scores - min_score) / (max_score - min_score)
+
+    @staticmethod
+    def get_top_indices(scores, k):
+        return scores.argsort()[-k:][::-1]
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import json
-
-from .retrieval_memory import RetrievalMemory
-
-
-class RetrievalMemoryManager:
-    def __init__(self, retrieval_memory: RetrievalMemory):
-        self.retrieval_memory = retrieval_memory
-
-    def add_memory_to_retrieval(self, description: str, importance: float = 1.0) -> str:
-        """
-        Adds a memory with a given description and importance to the memory stream.
-        """
-        self.retrieval_memory.add_memory(description, importance=importance)
-        return f"Information added to archival memory."
-
-    def retrieve_memories(
-        self, query: str, max_results: int = 5, page: int = 1, page_size: int = 5
-    ) -> str:
-        """
-        Retrieves memories from the memory stream based on a query.
-        """
-        memories = self.retrieval_memory.retrieve_memories(query, max_results)
-        # Calculate start and end indices for slicing the memories list for pagination
-        start_index = (page - 1) * page_size
-        end_index = start_index + page_size
-
-        # Slice the list to get the paginated results
-        paginated_memories = memories[start_index:end_index]
-        formatted_memories = ""
-        for memory in paginated_memories:
-            formatted_memories += (
-                f'{memory["creation_timestamp"]}: {memory["memory"]}\n'
-            )
-
-        if formatted_memories != "":
-            formatted_memories += f"\n\nPage {page} of {len(memories) // page_size + 1}"
-        return (
-            formatted_memories
-            if formatted_memories
-            else "No archival memories found matching the query."
-        )
+import json
+
+from .retrieval_memory import RetrievalMemory
+
+
+class RetrievalMemoryManager:
+    def __init__(self, retrieval_memory: RetrievalMemory):
+        self.retrieval_memory = retrieval_memory
+
+    def add_memory_to_retrieval(self, description: str, importance: float = 1.0) -> str:
+        """
+        Adds a memory with a given description and importance to the memory stream.
+        """
+        self.retrieval_memory.add_memory(description, importance=importance)
+        return f"Information added to archival memory."
+
+    def retrieve_memories(
+        self, query: str, max_results: int = 5, page: int = 1, page_size: int = 5
+    ) -> str:
+        """
+        Retrieves memories from the memory stream based on a query.
+        """
+        memories = self.retrieval_memory.retrieve_memories(query, max_results)
+        # Calculate start and end indices for slicing the memories list for pagination
+        start_index = (page - 1) * page_size
+        end_index = start_index + page_size
+
+        # Slice the list to get the paginated results
+        paginated_memories = memories[start_index:end_index]
+        formatted_memories = ""
+        for memory in paginated_memories:
+            formatted_memories += (
+                f'{memory["creation_timestamp"]}: {memory["memory"]}\n'
+            )
+
+        if formatted_memories != "":
+            formatted_memories += f"\n\nPage {page} of {len(memories) // page_size + 1}"
+        return (
+            formatted_memories
+            if formatted_memories
+            else "No archival memories found matching the query."
+        )
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/chain.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/chain.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,239 +1,239 @@
-from typing import List, Callable
-
-from llama_cpp_agent.function_calling import LlamaCppFunctionTool
-from llama_cpp_agent.llm_agent import LlamaCppAgent
-from llama_cpp_agent.llm_output_settings import LlmStructuredOutputSettings
-from llama_cpp_agent.llm_prompt_template import PromptTemplate
-from llama_cpp_agent.providers.provider_base import LlmSamplingSettings
-
-
-class AgentChainElement:
-    """
-    Represents a single element in the chain of an agent-based framework. This element holds all necessary data to
-    manage the prompt, process the input/output, and adjust the processing behavior based on given parameters.
-
-    Attributes:
-        output_identifier (str): Unique identifier for the output of this chain element.
-        system_prompt (str): Template string for the system prompt.
-        prompt (str): Template string for the main prompt to the language model.
-
-        preprocessor (Callable[[str, str, dict], tuple[str, str, dict]], optional): Function to preprocess the input
-                before sending it to the language model. Takes the system prompt with template fields replaced, the prompt
-                with template fields replaced, and the additional information dictionary as arguments and returns the
-                modified tuple of it.
-        postprocessor (Callable[[str, str, dict, str], str], optional): Function to postprocess the output from
-                the language model. Takes the system prompt, the prompt, the additional information dictionary and the
-                result as arguments and returns the modified result.
-        function_tool_registry (LlamaCppFunctionToolRegistry): Registry for LlamaCppFunctionTool and enables function calling.
-        add_prompt_to_chat_history (bool): Flag to determine if the prompt should be added to the chat history.
-        add_response_to_chat_history (bool): Flag to determine if the response should be added to the chat history.
-
-    Methods:
-        __init__: Constructs an instance of the AgentChain class.
-    """
-
-    def __init__(
-        self,
-        output_identifier: str,
-        system_prompt: str,
-        prompt: str,
-        tools: List[LlamaCppFunctionTool] = None,
-        structured_output_settings: LlmStructuredOutputSettings = None,
-        preprocessor: Callable[[str, str, dict], tuple[str, str, dict]] = None,
-        postprocessor: Callable[[str, str, dict, str], str] = None,
-        add_prompt_to_chat_history: bool = False,
-        add_response_to_chat_history: bool = False,
-        llm_sampling_settings: LlmSamplingSettings = None,
-    ):
-        """
-        Constructs an instance of the AgentChainElement class.
-
-        Args:
-            output_identifier (str): Unique identifier for the output of this chain element.
-            system_prompt (str): Template string for the system prompt.
-            prompt (str): Template string for the main prompt to the language model.
-            tools (List[LlamaCppFunctionTool], optional): List of function tools available for use in this chain element.
-            preprocessor (Callable[[str, str, dict], tuple[str, str, dict]], optional): Function to preprocess the input
-                before sending it to the language model. Takes the system prompt with template fields replaced, the prompt
-                with template fields replaced, and the additional information dictionary as arguments and returns the
-                modified tuple of it.
-            postprocessor (Callable[[str, str, dict, str], str], optional): Function to postprocess the output from
-                the language model. Takes the system prompt, the prompt, the additional information dictionary and the
-                result as arguments and returns the modified result.
-            add_prompt_to_chat_history (bool): Flag to determine if the prompt should be added to the chat history.
-            add_response_to_chat_history (bool): Flag to determine if the response should be added to the chat history.
-        """
-        self.output_identifier = output_identifier
-        self.system_prompt = system_prompt
-        self.prompt = prompt
-        self.add_prompt_to_chat_history = add_prompt_to_chat_history
-        self.add_response_to_chat_history = add_response_to_chat_history
-        self.structured_output_settings = structured_output_settings
-        self.preprocessor = preprocessor
-        self.postprocessor = postprocessor
-        self.function_tool_registry = None
-        if tools is not None:
-            self.structured_output_settings = (
-                LlmStructuredOutputSettings.from_llama_cpp_function_tools(tools)
-            )
-        self.llm_sampling_settings = llm_sampling_settings
-
-
-class AgentChain:
-    """
-    Represents a chain of AgentChainElements that are processed in a sequence to handle an interaction within an
-    agent-based system.
-
-    Attributes:
-        agent (LlamaCppAgent): The agent responsible for managing and processing the chain.
-        chain (List[AgentChainElement]): A list of AgentChainElement instances that make up the chain.
-
-    Methods:
-        __init__: Constructs an instance of the AgentChain class.
-        run_chain: Processes the entire chain of elements using provided inputs.
-    """
-
-    def __init__(self, agent: LlamaCppAgent, chain_elements: List[AgentChainElement]):
-        """
-        Constructs an instance of the AgentChain class.
-        Args:
-            agent (LlamaCppAgent): The agent responsible for managing and processing the chain.
-            chain_elements (List[AgentChainElement]): A list of AgentChainElement instances that make up the chain.
-        """
-        self.agent = agent
-        self.chain = chain_elements
-
-    def run_chain(self, user_message: str = None, additional_fields: dict = None):
-        """
-        Executes the chain of agent elements using the initial user message and additional fields, and
-        returns the final output and state of the outputs dictionary.
-
-        Args:
-            user_message (str, optional): Initial user message to be processed by the chain.
-            additional_fields (dict, optional): Dictionary of additional data to be used in the processing of the chain.
-
-        Returns:
-            tuple[str, dict]: A tuple containing the concatenated output string from the final element and
-            the dictionary of all outputs.
-        """
-        outputs = {}
-
-        if additional_fields is not None:
-            for field, value in additional_fields.items():
-                outputs[field] = value
-
-        for chain_element in self.chain:
-            sys_prompter = PromptTemplate.from_string(chain_element.system_prompt)
-            sys_prompt = sys_prompter.generate_prompt(outputs)
-            prompter = PromptTemplate.from_string(chain_element.prompt)
-            prompt = prompter.generate_prompt(outputs)
-            if chain_element.function_tool_registry is not None:
-                sys_prompt += f"\n\nYou can call functions in JSON format.\n\nAvailable Function Tools:\n\n{chain_element.function_tool_registry.get_documentation().strip()}"
-            if chain_element.preprocessor is not None:
-                sys_prompt, prompt, outputs = chain_element.preprocessor(
-                    sys_prompt, prompt, outputs
-                )
-
-            outputs[chain_element.output_identifier] = self.agent.get_chat_response(
-                user_message if user_message is not None else prompt,
-                system_prompt=sys_prompt,
-                structured_output_settings=chain_element.structured_output_settings,
-                add_response_to_chat_history=chain_element.add_response_to_chat_history,
-                add_message_to_chat_history=chain_element.add_prompt_to_chat_history,
-                llm_sampling_settings=chain_element.llm_sampling_settings,
-            )
-            if chain_element.function_tool_registry is not None:
-                outputs[chain_element.output_identifier] = outputs[
-                    chain_element.output_identifier
-                ][0]["return_value"]
-            if chain_element.postprocessor is not None:
-                outputs[
-                    chain_element.output_identifier
-                ] = chain_element.postprocessor = chain_element.postprocessor(
-                    sys_prompt,
-                    prompt,
-                    outputs,
-                    outputs[chain_element.output_identifier],
-                )
-        output = "\n".join(
-            [val if isinstance(val, str) else str(val) for val in outputs.values()]
-        )
-        return output, outputs
-
-
-class MapChain:
-    """
-    Represents a specialized chain that maps over a list of items and then combines the results using another chain.
-
-    Attributes:
-        agent (LlamaCppAgent): The agent responsible for managing and processing the map and combine chains.
-        map_chain (AgentChain): An AgentChain instance used to process each item in the list.
-        combine_chain (AgentChain): An AgentChain instance used to combine the results of the map chain.
-        item_identifier (str): The identifier used to insert each item into the additional_fields dictionary.
-        map_output_identifier (str): The identifier used to store the results of the map chain before passing to the
-        combine chain.
-
-    Methods:
-        __init__: Constructs an instance of the MapChain class.
-        run_map_chain: Executes the map chain on a list of items and then processes the results with the combine chain.
-    """
-
-    def __init__(
-        self,
-        agent: LlamaCppAgent,
-        map_chain: List[AgentChainElement],
-        combine_chain: List[AgentChainElement],
-        item_identifier: str = "item",
-        map_output_identifier: str = "map_output",
-    ):
-        """
-        Constructs an instance of the MapChain class. This class is designed to process a list of items through
-        a mapping chain and then combine the results using a combining chain.
-
-        Args:
-            agent (LlamaCppAgent): The agent responsible for managing and processing the map and combine chains.
-            map_chain (List[AgentChainElement]): A list of AgentChainElement instances that make up the map chain.
-            combine_chain (List[AgentChainElement]): A list of AgentChainElement instances that make up the combine chain.
-            item_identifier (str, optional): The identifier used to insert each item into the additional_fields dictionary.
-            map_output_identifier (str, optional): The identifier used to store the results of the map chain before passing to the combine chain.
-        """
-        self.agent = agent
-        self.map_chain = AgentChain(agent, map_chain)
-        self.combine_chain = AgentChain(agent, combine_chain)
-        self.item_identifier = item_identifier
-        self.map_output_identifier = map_output_identifier
-
-    def run_map_chain(
-        self,
-        items_to_map: list[str],
-        user_message: str = None,
-        additional_fields: dict = None,
-    ):
-        """
-        Executes the map chain over a list of items and then uses the combine chain to process the concatenated
-        results.
-
-        Args:
-            items_to_map (list[str]): List of strings to be individually processed by the map chain.
-            user_message (str, optional): Initial user message to be included in the processing.
-            additional_fields (dict, optional): Additional data to be used throughout the map and combine chains.
-
-        Returns:
-            tuple: A tuple containing the final output string from the combine chain and the outputs dictionary.
-        """
-        outputs = {}
-
-        if additional_fields is not None:
-            for field, value in additional_fields.items():
-                outputs[field] = value
-        else:
-            additional_fields = {}
-        results = []
-        for item in items_to_map:
-            additional_fields[self.item_identifier] = item
-            result, result_dic = self.map_chain.run_chain(
-                user_message=user_message, additional_fields=additional_fields
-            )
-            results.append(result_dic[self.map_chain.chain[-1].output_identifier])
-        additional_fields[self.map_output_identifier] = "\n\n".join(results)
-        return self.combine_chain.run_chain(additional_fields=additional_fields)
+from typing import List, Callable
+
+from llama_cpp_agent.function_calling import LlamaCppFunctionTool
+from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.llm_output_settings import LlmStructuredOutputSettings
+from llama_cpp_agent.llm_prompt_template import PromptTemplate
+from llama_cpp_agent.providers.provider_base import LlmSamplingSettings
+
+
+class AgentChainElement:
+    """
+    Represents a single element in the chain of an agent-based framework. This element holds all necessary data to
+    manage the prompt, process the input/output, and adjust the processing behavior based on given parameters.
+
+    Attributes:
+        output_identifier (str): Unique identifier for the output of this chain element.
+        system_prompt (str): Template string for the system prompt.
+        prompt (str): Template string for the main prompt to the language model.
+
+        preprocessor (Callable[[str, str, dict], tuple[str, str, dict]], optional): Function to preprocess the input
+                before sending it to the language model. Takes the system prompt with template fields replaced, the prompt
+                with template fields replaced, and the additional information dictionary as arguments and returns the
+                modified tuple of it.
+        postprocessor (Callable[[str, str, dict, str], str], optional): Function to postprocess the output from
+                the language model. Takes the system prompt, the prompt, the additional information dictionary and the
+                result as arguments and returns the modified result.
+        function_tool_registry (LlamaCppFunctionToolRegistry): Registry for LlamaCppFunctionTool and enables function calling.
+        add_prompt_to_chat_history (bool): Flag to determine if the prompt should be added to the chat history.
+        add_response_to_chat_history (bool): Flag to determine if the response should be added to the chat history.
+
+    Methods:
+        __init__: Constructs an instance of the AgentChain class.
+    """
+
+    def __init__(
+        self,
+        output_identifier: str,
+        system_prompt: str,
+        prompt: str,
+        tools: List[LlamaCppFunctionTool] = None,
+        structured_output_settings: LlmStructuredOutputSettings = None,
+        preprocessor: Callable[[str, str, dict], tuple[str, str, dict]] = None,
+        postprocessor: Callable[[str, str, dict, str], str] = None,
+        add_prompt_to_chat_history: bool = False,
+        add_response_to_chat_history: bool = False,
+        llm_sampling_settings: LlmSamplingSettings = None,
+    ):
+        """
+        Constructs an instance of the AgentChainElement class.
+
+        Args:
+            output_identifier (str): Unique identifier for the output of this chain element.
+            system_prompt (str): Template string for the system prompt.
+            prompt (str): Template string for the main prompt to the language model.
+            tools (List[LlamaCppFunctionTool], optional): List of function tools available for use in this chain element.
+            preprocessor (Callable[[str, str, dict], tuple[str, str, dict]], optional): Function to preprocess the input
+                before sending it to the language model. Takes the system prompt with template fields replaced, the prompt
+                with template fields replaced, and the additional information dictionary as arguments and returns the
+                modified tuple of it.
+            postprocessor (Callable[[str, str, dict, str], str], optional): Function to postprocess the output from
+                the language model. Takes the system prompt, the prompt, the additional information dictionary and the
+                result as arguments and returns the modified result.
+            add_prompt_to_chat_history (bool): Flag to determine if the prompt should be added to the chat history.
+            add_response_to_chat_history (bool): Flag to determine if the response should be added to the chat history.
+        """
+        self.output_identifier = output_identifier
+        self.system_prompt = system_prompt
+        self.prompt = prompt
+        self.add_prompt_to_chat_history = add_prompt_to_chat_history
+        self.add_response_to_chat_history = add_response_to_chat_history
+        self.structured_output_settings = structured_output_settings
+        self.preprocessor = preprocessor
+        self.postprocessor = postprocessor
+        self.function_tool_registry = None
+        if tools is not None:
+            self.structured_output_settings = (
+                LlmStructuredOutputSettings.from_llama_cpp_function_tools(tools)
+            )
+        self.llm_sampling_settings = llm_sampling_settings
+
+
+class AgentChain:
+    """
+    Represents a chain of AgentChainElements that are processed in a sequence to handle an interaction within an
+    agent-based system.
+
+    Attributes:
+        agent (LlamaCppAgent): The agent responsible for managing and processing the chain.
+        chain (List[AgentChainElement]): A list of AgentChainElement instances that make up the chain.
+
+    Methods:
+        __init__: Constructs an instance of the AgentChain class.
+        run_chain: Processes the entire chain of elements using provided inputs.
+    """
+
+    def __init__(self, agent: LlamaCppAgent, chain_elements: List[AgentChainElement]):
+        """
+        Constructs an instance of the AgentChain class.
+        Args:
+            agent (LlamaCppAgent): The agent responsible for managing and processing the chain.
+            chain_elements (List[AgentChainElement]): A list of AgentChainElement instances that make up the chain.
+        """
+        self.agent = agent
+        self.chain = chain_elements
+
+    def run_chain(self, user_message: str = None, additional_fields: dict = None):
+        """
+        Executes the chain of agent elements using the initial user message and additional fields, and
+        returns the final output and state of the outputs dictionary.
+
+        Args:
+            user_message (str, optional): Initial user message to be processed by the chain.
+            additional_fields (dict, optional): Dictionary of additional data to be used in the processing of the chain.
+
+        Returns:
+            tuple[str, dict]: A tuple containing the concatenated output string from the final element and
+            the dictionary of all outputs.
+        """
+        outputs = {}
+
+        if additional_fields is not None:
+            for field, value in additional_fields.items():
+                outputs[field] = value
+
+        for chain_element in self.chain:
+            sys_prompter = PromptTemplate.from_string(chain_element.system_prompt)
+            sys_prompt = sys_prompter.generate_prompt(outputs)
+            prompter = PromptTemplate.from_string(chain_element.prompt)
+            prompt = prompter.generate_prompt(outputs)
+            if chain_element.function_tool_registry is not None:
+                sys_prompt += f"\n\nYou can call functions in JSON format.\n\nAvailable Function Tools:\n\n{chain_element.function_tool_registry.get_documentation().strip()}"
+            if chain_element.preprocessor is not None:
+                sys_prompt, prompt, outputs = chain_element.preprocessor(
+                    sys_prompt, prompt, outputs
+                )
+
+            outputs[chain_element.output_identifier] = self.agent.get_chat_response(
+                user_message if user_message is not None else prompt,
+                system_prompt=sys_prompt,
+                structured_output_settings=chain_element.structured_output_settings,
+                add_response_to_chat_history=chain_element.add_response_to_chat_history,
+                add_message_to_chat_history=chain_element.add_prompt_to_chat_history,
+                llm_sampling_settings=chain_element.llm_sampling_settings,
+            )
+            if chain_element.function_tool_registry is not None:
+                outputs[chain_element.output_identifier] = outputs[
+                    chain_element.output_identifier
+                ][0]["return_value"]
+            if chain_element.postprocessor is not None:
+                outputs[
+                    chain_element.output_identifier
+                ] = chain_element.postprocessor = chain_element.postprocessor(
+                    sys_prompt,
+                    prompt,
+                    outputs,
+                    outputs[chain_element.output_identifier],
+                )
+        output = "\n".join(
+            [val if isinstance(val, str) else str(val) for val in outputs.values()]
+        )
+        return output, outputs
+
+
+class MapChain:
+    """
+    Represents a specialized chain that maps over a list of items and then combines the results using another chain.
+
+    Attributes:
+        agent (LlamaCppAgent): The agent responsible for managing and processing the map and combine chains.
+        map_chain (AgentChain): An AgentChain instance used to process each item in the list.
+        combine_chain (AgentChain): An AgentChain instance used to combine the results of the map chain.
+        item_identifier (str): The identifier used to insert each item into the additional_fields dictionary.
+        map_output_identifier (str): The identifier used to store the results of the map chain before passing to the
+        combine chain.
+
+    Methods:
+        __init__: Constructs an instance of the MapChain class.
+        run_map_chain: Executes the map chain on a list of items and then processes the results with the combine chain.
+    """
+
+    def __init__(
+        self,
+        agent: LlamaCppAgent,
+        map_chain: List[AgentChainElement],
+        combine_chain: List[AgentChainElement],
+        item_identifier: str = "item",
+        map_output_identifier: str = "map_output",
+    ):
+        """
+        Constructs an instance of the MapChain class. This class is designed to process a list of items through
+        a mapping chain and then combine the results using a combining chain.
+
+        Args:
+            agent (LlamaCppAgent): The agent responsible for managing and processing the map and combine chains.
+            map_chain (List[AgentChainElement]): A list of AgentChainElement instances that make up the map chain.
+            combine_chain (List[AgentChainElement]): A list of AgentChainElement instances that make up the combine chain.
+            item_identifier (str, optional): The identifier used to insert each item into the additional_fields dictionary.
+            map_output_identifier (str, optional): The identifier used to store the results of the map chain before passing to the combine chain.
+        """
+        self.agent = agent
+        self.map_chain = AgentChain(agent, map_chain)
+        self.combine_chain = AgentChain(agent, combine_chain)
+        self.item_identifier = item_identifier
+        self.map_output_identifier = map_output_identifier
+
+    def run_map_chain(
+        self,
+        items_to_map: list[str],
+        user_message: str = None,
+        additional_fields: dict = None,
+    ):
+        """
+        Executes the map chain over a list of items and then uses the combine chain to process the concatenated
+        results.
+
+        Args:
+            items_to_map (list[str]): List of strings to be individually processed by the map chain.
+            user_message (str, optional): Initial user message to be included in the processing.
+            additional_fields (dict, optional): Additional data to be used throughout the map and combine chains.
+
+        Returns:
+            tuple: A tuple containing the final output string from the combine chain and the outputs dictionary.
+        """
+        outputs = {}
+
+        if additional_fields is not None:
+            for field, value in additional_fields.items():
+                outputs[field] = value
+        else:
+            additional_fields = {}
+        results = []
+        for item in items_to_map:
+            additional_fields[self.item_identifier] = item
+            result, result_dic = self.map_chain.run_chain(
+                user_message=user_message, additional_fields=additional_fields
+            )
+            results.append(result_dic[self.map_chain.chain[-1].output_identifier])
+        additional_fields[self.map_output_identifier] = "\n\n".join(results)
+        return self.combine_chain.run_chain(additional_fields=additional_fields)
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/basic_chat_history.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/chat_history/basic_chat_history.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,188 +1,188 @@
-import json
-from enum import Enum
-from typing import List, Dict
-
-from pydantic import parse_obj_as
-
-from llama_cpp_agent.chat_history.chat_history_base import ChatMessageStore, ChatHistory
-from llama_cpp_agent.chat_history.messages import (
-    ChatMessage,
-    UserMessage,
-    AssistantMessage,
-    SystemMessage,
-    Roles,
-    convert_messages_to_list_of_dictionaries, ToolMessage, generate_function_call_id,
-)
-from llama_cpp_agent.providers.provider_base import LlmProvider
-
-
-class BasicChatMessageStore(ChatMessageStore):
-    def __init__(self, messages: List[ChatMessage] = None):
-        if messages is None:
-            messages = []
-        self.messages: List[ChatMessage] = messages
-
-    def get_messages_count(self):
-        return len(self.messages)
-
-    def add_message(self, message: ChatMessage):
-        self.messages.append(message)
-
-    def edit_message(self, index: int, edited_message: ChatMessage):
-        self.messages[index] = edited_message
-
-    def add_user_message(self, message: str):
-        self.messages.append(UserMessage(role=Roles.user, content=message))
-
-    def add_assistant_message(self, message: str):
-        self.messages.append(AssistantMessage(role=Roles.assistant, content=message))
-
-    def add_system_message(self, message: str):
-        self.messages.append(SystemMessage(role=Roles.system, content=message))
-
-    def remove_last_message(self):
-        self.messages = self.messages[:-1]
-
-    def remove_last_k_messages(self, k: int):
-        self.messages = self.messages[:-k]
-
-    def get_message(self, index: int) -> ChatMessage:
-        return self.messages[index]
-
-    def get_last_message(self) -> ChatMessage:
-        return self.messages[-1]
-
-    def get_last_k_messages(self, k: int) -> List[ChatMessage]:
-        return self.messages[-k:]
-
-    def get_messages(self, k: int) -> List[ChatMessage]:
-        return self.messages[k:]
-
-    def get_all_messages(self) -> List[ChatMessage]:
-        return self.messages
-
-    def save_to_json(self, file_path: str):
-        # Convert messages to a list of dictionaries using pydantic's model_dump() method
-        messages_dict = [{"role": message.role.value, "content": message.content} for message in self.messages]
-        # Write the list of dictionaries to a JSON file
-        with open(file_path, "w") as file:
-            json.dump(messages_dict, file, indent=4)
-
-    def load_from_json(self, file_path: str):
-        # Read the list of dictionaries from a JSON file
-        with open(file_path, "r") as file:
-            messages_dict = json.load(file)
-        # Convert dictionaries back to ChatMessage instances
-        self.messages = [SystemMessage(content=message["content"]) if message["role"] == "system" else
-                         UserMessage(content=message["content"]) if message["role"] == "user" else
-                         AssistantMessage(content=message["content"]) if message["role"] == "assistant" else
-                         ToolMessage(content=message["content"]) for message in messages_dict]
-
-
-class BasicChatHistoryStrategy(Enum):
-    last_k_messages: str = "last_k_messages"
-    last_k_tokens: str = "last_k_tokens"
-
-
-class BasicChatHistory(ChatHistory):
-
-    def __init__(
-            self,
-            chat_history_strategy: BasicChatHistoryStrategy = BasicChatHistoryStrategy.last_k_messages,
-            k: int = 20,
-            llm_provider: LlmProvider = None,
-            message_store: ChatMessageStore = None,
-    ):
-        if message_store is None:
-            message_store = BasicChatMessageStore()
-        self.message_store: ChatMessageStore = message_store
-        self.k = k
-        self.strategy = chat_history_strategy
-        self.llm_provider = llm_provider
-        if (
-                chat_history_strategy == BasicChatHistoryStrategy.last_k_tokens
-                and llm_provider is None
-        ):
-            raise Exception(
-                "Please pass a LLM provider to BasicChatHistory when using last k tokens as memory strategy!"
-            )
-
-    def get_message_store(self) -> BasicChatMessageStore:
-        return self.message_store
-
-    def get_chat_messages(self) -> List[Dict[str, str]]:
-        if self.strategy == BasicChatHistoryStrategy.last_k_messages:
-            messages = [self.message_store.get_message(0)]
-            messages.extend(self.message_store.get_last_k_messages(self.k - 1))
-            return convert_messages_to_list_of_dictionaries(messages)
-        elif self.strategy == BasicChatHistoryStrategy.last_k_tokens:
-            total_tokens = 0
-            selected_messages = []
-            converted_messages = convert_messages_to_list_of_dictionaries(
-                self.message_store.get_all_messages()
-            )
-            sys_message = None
-            if converted_messages[0]["role"] == "system":
-                sys_message = converted_messages.pop(0)
-            if sys_message is not None:
-                total_tokens = len(self.llm_provider.tokenize(sys_message["content"]))
-            for message in reversed(converted_messages):
-                tokens = self.llm_provider.tokenize(message["content"])
-                total_tokens += len(tokens)
-                if total_tokens >= self.k:
-                    if len(selected_messages) == 0:
-                        selected_messages.append(message)
-                    break
-                else:
-                    selected_messages.append(message)
-            if sys_message is not None:
-                selected_messages.append(sys_message)
-            return list(reversed(selected_messages))
-        return []
-
-    def add_message(self, message: Dict[str, str]):
-        if message["role"] == Roles.system:
-            self.message_store.add_message(
-                SystemMessage(content=message["content"])
-            )
-        elif message["role"] == Roles.user:
-            self.message_store.add_message(
-                UserMessage(content=message["content"])
-            )
-        elif message["role"] == Roles.assistant:
-            self.message_store.add_message(
-                AssistantMessage(content=message["content"])
-            )
-        elif message["role"] == Roles.tool:
-            self.message_store.add_message(
-                ToolMessage(tool_call_id=generate_function_call_id(), content=message["content"])
-            )
-
-    def get_messages_count(self):
-        return self.message_store.get_messages_count()
-
-    def edit_message(self, index: int, message: Dict[str, str]):
-        if message["role"] == Roles.system:
-            self.message_store.edit_message(
-                index,
-                SystemMessage(content=message["content"])
-            )
-        elif message["role"] == Roles.user:
-            self.message_store.edit_message(
-                index,
-                UserMessage(content=message["content"])
-            )
-        elif message["role"] == Roles.assistant:
-            self.message_store.edit_message(
-                index,
-                AssistantMessage(content=message["content"])
-            )
-        elif message["role"] == Roles.tool:
-            self.message_store.edit_message(
-                index,
-                ToolMessage(tool_call_id=generate_function_call_id(), content=message["content"])
-            )
-
-    def get_message(self, index) -> Dict[str, str]:
-        message = self.message_store.get_message(index)
-        return {"role": message.role, "content": message.content}
+import json
+from enum import Enum
+from typing import List, Dict
+
+from pydantic import parse_obj_as
+
+from llama_cpp_agent.chat_history.chat_history_base import ChatMessageStore, ChatHistory
+from llama_cpp_agent.chat_history.messages import (
+    ChatMessage,
+    UserMessage,
+    AssistantMessage,
+    SystemMessage,
+    Roles,
+    convert_messages_to_list_of_dictionaries, ToolMessage, generate_function_call_id,
+)
+from llama_cpp_agent.providers.provider_base import LlmProvider
+
+
+class BasicChatMessageStore(ChatMessageStore):
+    def __init__(self, messages: List[ChatMessage] = None):
+        if messages is None:
+            messages = []
+        self.messages: List[ChatMessage] = messages
+
+    def get_messages_count(self):
+        return len(self.messages)
+
+    def add_message(self, message: ChatMessage):
+        self.messages.append(message)
+
+    def edit_message(self, index: int, edited_message: ChatMessage):
+        self.messages[index] = edited_message
+
+    def add_user_message(self, message: str):
+        self.messages.append(UserMessage(role=Roles.user, content=message))
+
+    def add_assistant_message(self, message: str):
+        self.messages.append(AssistantMessage(role=Roles.assistant, content=message))
+
+    def add_system_message(self, message: str):
+        self.messages.append(SystemMessage(role=Roles.system, content=message))
+
+    def remove_last_message(self):
+        self.messages = self.messages[:-1]
+
+    def remove_last_k_messages(self, k: int):
+        self.messages = self.messages[:-k]
+
+    def get_message(self, index: int) -> ChatMessage:
+        return self.messages[index]
+
+    def get_last_message(self) -> ChatMessage:
+        return self.messages[-1]
+
+    def get_last_k_messages(self, k: int) -> List[ChatMessage]:
+        return self.messages[-k:]
+
+    def get_messages(self, k: int) -> List[ChatMessage]:
+        return self.messages[k:]
+
+    def get_all_messages(self) -> List[ChatMessage]:
+        return self.messages
+
+    def save_to_json(self, file_path: str):
+        # Convert messages to a list of dictionaries using pydantic's model_dump() method
+        messages_dict = [{"role": message.role.value, "content": message.content} for message in self.messages]
+        # Write the list of dictionaries to a JSON file
+        with open(file_path, "w") as file:
+            json.dump(messages_dict, file, indent=4)
+
+    def load_from_json(self, file_path: str):
+        # Read the list of dictionaries from a JSON file
+        with open(file_path, "r") as file:
+            messages_dict = json.load(file)
+        # Convert dictionaries back to ChatMessage instances
+        self.messages = [SystemMessage(content=message["content"]) if message["role"] == "system" else
+                         UserMessage(content=message["content"]) if message["role"] == "user" else
+                         AssistantMessage(content=message["content"]) if message["role"] == "assistant" else
+                         ToolMessage(content=message["content"]) for message in messages_dict]
+
+
+class BasicChatHistoryStrategy(Enum):
+    last_k_messages: str = "last_k_messages"
+    last_k_tokens: str = "last_k_tokens"
+
+
+class BasicChatHistory(ChatHistory):
+
+    def __init__(
+            self,
+            chat_history_strategy: BasicChatHistoryStrategy = BasicChatHistoryStrategy.last_k_messages,
+            k: int = 20,
+            llm_provider: LlmProvider = None,
+            message_store: ChatMessageStore = None,
+    ):
+        if message_store is None:
+            message_store = BasicChatMessageStore()
+        self.message_store: ChatMessageStore = message_store
+        self.k = k
+        self.strategy = chat_history_strategy
+        self.llm_provider = llm_provider
+        if (
+                chat_history_strategy == BasicChatHistoryStrategy.last_k_tokens
+                and llm_provider is None
+        ):
+            raise Exception(
+                "Please pass a LLM provider to BasicChatHistory when using last k tokens as memory strategy!"
+            )
+
+    def get_message_store(self) -> BasicChatMessageStore:
+        return self.message_store
+
+    def get_chat_messages(self) -> List[Dict[str, str]]:
+        if self.strategy == BasicChatHistoryStrategy.last_k_messages:
+            messages = [self.message_store.get_message(0)]
+            messages.extend(self.message_store.get_last_k_messages(self.k - 1))
+            return convert_messages_to_list_of_dictionaries(messages)
+        elif self.strategy == BasicChatHistoryStrategy.last_k_tokens:
+            total_tokens = 0
+            selected_messages = []
+            converted_messages = convert_messages_to_list_of_dictionaries(
+                self.message_store.get_all_messages()
+            )
+            sys_message = None
+            if converted_messages[0]["role"] == "system":
+                sys_message = converted_messages.pop(0)
+            if sys_message is not None:
+                total_tokens = len(self.llm_provider.tokenize(sys_message["content"]))
+            for message in reversed(converted_messages):
+                tokens = self.llm_provider.tokenize(message["content"])
+                total_tokens += len(tokens)
+                if total_tokens >= self.k:
+                    if len(selected_messages) == 0:
+                        selected_messages.append(message)
+                    break
+                else:
+                    selected_messages.append(message)
+            if sys_message is not None:
+                selected_messages.append(sys_message)
+            return list(reversed(selected_messages))
+        return []
+
+    def add_message(self, message: Dict[str, str]):
+        if message["role"] == Roles.system:
+            self.message_store.add_message(
+                SystemMessage(content=message["content"])
+            )
+        elif message["role"] == Roles.user:
+            self.message_store.add_message(
+                UserMessage(content=message["content"])
+            )
+        elif message["role"] == Roles.assistant:
+            self.message_store.add_message(
+                AssistantMessage(content=message["content"])
+            )
+        elif message["role"] == Roles.tool:
+            self.message_store.add_message(
+                ToolMessage(tool_call_id=generate_function_call_id(), content=message["content"])
+            )
+
+    def get_messages_count(self):
+        return self.message_store.get_messages_count()
+
+    def edit_message(self, index: int, message: Dict[str, str]):
+        if message["role"] == Roles.system:
+            self.message_store.edit_message(
+                index,
+                SystemMessage(content=message["content"])
+            )
+        elif message["role"] == Roles.user:
+            self.message_store.edit_message(
+                index,
+                UserMessage(content=message["content"])
+            )
+        elif message["role"] == Roles.assistant:
+            self.message_store.edit_message(
+                index,
+                AssistantMessage(content=message["content"])
+            )
+        elif message["role"] == Roles.tool:
+            self.message_store.edit_message(
+                index,
+                ToolMessage(tool_call_id=generate_function_call_id(), content=message["content"])
+            )
+
+    def get_message(self, index) -> Dict[str, str]:
+        message = self.message_store.get_message(index)
+        return {"role": message.role, "content": message.content}
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/messages.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/chat_history/messages.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import string
-from enum import Enum
-import random
-from typing import Literal, Union, List, Optional, Annotated, Dict
-
-from pydantic import BaseModel, Field
-
-
-def generate_function_call_id(length=9):
-    # Characters to use in the ID
-    characters = string.ascii_letters + string.digits
-    # Random choice of characters
-    return "".join(random.choice(characters) if (idx % 500 != 0) else "\n" for idx in range(length))
-
-
-class ToolType(Enum):
-    function = "function"
-
-
-class FunctionCall(BaseModel):
-    name: str
-    arguments: str
-
-
-class ToolCall(BaseModel):
-    id: str
-    type: ToolType = ToolType.function
-    function: FunctionCall
-
-
-class Roles(Enum):
-    system = "system"
-    user = "user"
-    assistant = "assistant"
-    tool = "tool"
-
-
-class BaseMessage(BaseModel):
-    role: Literal[Roles.system, Roles.user, Roles.assistant, Roles.tool]
-
-
-class UserMessage(BaseMessage):
-    role: Literal[Roles.user] = Roles.user
-    content: str
-
-
-class SystemMessage(BaseMessage):
-    role: Literal[Roles.system] = Roles.system
-    content: str
-
-
-class AssistantMessage(BaseMessage):
-    role: Literal[Roles.assistant] = Roles.assistant
-    content: Optional[str] = None
-    tool_calls: Optional[List[ToolCall]] = None
-
-
-class ToolMessage(BaseMessage):
-    tool_call_id: str
-    role: Literal[Roles.tool] = Roles.tool
-    content: str
-
-
-ChatMessage = Annotated[
-    Union[SystemMessage, UserMessage, AssistantMessage, ToolMessage],
-    Field(discriminator="role"),
-]
-
-
-# Function to convert messages to list of dictionary format
-def convert_messages_to_list_of_dictionaries(
-    messages: List[ChatMessage],
-) -> List[Dict[str, str]]:
-    """
-    Converts a list of messages to a list of dictionaries.
-    Args:
-        messages (List[ChatMessage]): The list of messages.
-    Returns:
-        List[Dict[str, str]]: A list of dictionaries.
-    """
-    result = []
-    for message in messages:
-        # Determine the appropriate content to include
-        content = ""
-        if isinstance(message, AssistantMessage):
-            if message.content is not None:
-                content = message.content
-            elif message.tool_calls is not None:
-                if len(message.tool_calls) > 1:
-                    content = "Function Calls:\n"
-                    count = 1
-                    for tool_call in message.tool_calls:
-                        content += f"{count}. Function: {tool_call.function.name}\nArguments: {tool_call.function.arguments}\n"
-                        count += 1
-                else:
-                    content = f"Function Call:\nFunction: {message.tool_calls[0].function.name}\nArguments: {message.tool_calls[0].function.arguments}\n"
-        elif isinstance(message, ToolMessage):
-            content = f"{message.content}\n"
-        else:
-            content = f"{message.content}"
-        # Construct the dictionary for the current message
-        msg_dict = {"role": message.role.value, "content": content}
-        result.append(msg_dict)
-    return result
+import string
+from enum import Enum
+import random
+from typing import Literal, Union, List, Optional, Annotated, Dict
+
+from pydantic import BaseModel, Field
+
+
+def generate_function_call_id(length=9):
+    # Characters to use in the ID
+    characters = string.ascii_letters + string.digits
+    # Random choice of characters
+    return "".join(random.choice(characters) if (idx % 500 != 0) else "\n" for idx in range(length))
+
+
+class ToolType(Enum):
+    function = "function"
+
+
+class FunctionCall(BaseModel):
+    name: str
+    arguments: str
+
+
+class ToolCall(BaseModel):
+    id: str
+    type: ToolType = ToolType.function
+    function: FunctionCall
+
+
+class Roles(Enum):
+    system = "system"
+    user = "user"
+    assistant = "assistant"
+    tool = "tool"
+
+
+class BaseMessage(BaseModel):
+    role: Literal[Roles.system, Roles.user, Roles.assistant, Roles.tool]
+
+
+class UserMessage(BaseMessage):
+    role: Literal[Roles.user] = Roles.user
+    content: str
+
+
+class SystemMessage(BaseMessage):
+    role: Literal[Roles.system] = Roles.system
+    content: str
+
+
+class AssistantMessage(BaseMessage):
+    role: Literal[Roles.assistant] = Roles.assistant
+    content: Optional[str] = None
+    tool_calls: Optional[List[ToolCall]] = None
+
+
+class ToolMessage(BaseMessage):
+    tool_call_id: str
+    role: Literal[Roles.tool] = Roles.tool
+    content: str
+
+
+ChatMessage = Annotated[
+    Union[SystemMessage, UserMessage, AssistantMessage, ToolMessage],
+    Field(discriminator="role"),
+]
+
+
+# Function to convert messages to list of dictionary format
+def convert_messages_to_list_of_dictionaries(
+    messages: List[ChatMessage],
+) -> List[Dict[str, str]]:
+    """
+    Converts a list of messages to a list of dictionaries.
+    Args:
+        messages (List[ChatMessage]): The list of messages.
+    Returns:
+        List[Dict[str, str]]: A list of dictionaries.
+    """
+    result = []
+    for message in messages:
+        # Determine the appropriate content to include
+        content = ""
+        if isinstance(message, AssistantMessage):
+            if message.content is not None:
+                content = message.content
+            elif message.tool_calls is not None:
+                if len(message.tool_calls) > 1:
+                    content = "Function Calls:\n"
+                    count = 1
+                    for tool_call in message.tool_calls:
+                        content += f"{count}. Function: {tool_call.function.name}\nArguments: {tool_call.function.arguments}\n"
+                        count += 1
+                else:
+                    content = f"Function Call:\nFunction: {message.tool_calls[0].function.name}\nArguments: {message.tool_calls[0].function.arguments}\n"
+        elif isinstance(message, ToolMessage):
+            content = f"{message.content}\n"
+        else:
+            content = f"{message.content}"
+        # Construct the dictionary for the current message
+        msg_dict = {"role": message.role.value, "content": content}
+        result.append(msg_dict)
+    return result
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/function_calling_agent.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/function_calling_agent.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,295 +1,295 @@
-import datetime
-import json
-import os
-from copy import copy
-from typing import Type, List, Callable, Union, Literal
-
-from llama_cpp import Llama
-from pydantic import BaseModel, Field
-
-from .llm_output_settings import LlmStructuredOutputSettings, LlmStructuredOutputType
-
-from .llm_agent import LlamaCppAgent, StreamingResponse
-from .messages_formatter import MessagesFormatterType, MessagesFormatter
-from .function_calling import LlamaCppFunctionTool
-
-from .providers.provider_base import LlmProvider, LlmSamplingSettings
-
-
-class activate_message_mode(BaseModel):
-    """
-    Activates message mode.
-    """
-
-    def run(self, agent: "FunctionCallingAgent"):
-        agent.without_grammar_mode = True
-        agent.prompt_suffix = "\nWrite message in plain text format:"
-        agent.without_grammar_mode_function.append(agent.send_message_to_user)
-        return True
-
-
-class send_message(BaseModel):
-    """
-    Sends a message to the user.
-    """
-
-    content: str = Field(..., description="Content of the message to be sent.")
-
-    def run(self, agent: "FunctionCallingAgent"):
-        agent.send_message_to_user(self.content)
-        return "Message sent."
-
-
-class write_text_file(BaseModel):
-    """
-    Writes content to a file.
-    """
-
-    file_path: str = Field(..., description="The path to the file.")
-    content: str = Field(..., description="The content to write to the file.")
-
-    def run(self, agent: "FunctionCallingAgent"):
-        self.write_file(self.content)
-        return True
-
-    def write_file(self, content: str):
-        """
-        Write content to a file.
-
-        Args:
-            content (str): The content to write to the file.
-        """
-        with open(self.file_path, "w", encoding="utf-8") as file:
-            file.write(content)
-        return None
-
-
-class read_text_file(BaseModel):
-    """
-    Reads the content of a file.
-    """
-
-    file_path: str = Field(..., description="The path to the file.")
-
-    def run(self):
-        return self.read_file()
-
-    def read_file(self):
-        """
-        Reads the content of a file.
-        """
-        if os.path.exists(self.file_path):
-            with open(self.file_path, "r", encoding="utf-8") as file:
-                return file.read()
-        else:
-            return f"File not found."
-
-
-class FunctionCallingAgent:
-    """
-    An agent that uses function calling to interact with its environment and the user.
-
-    Args:
-        llama_llm (Llama | LlamaLLMSettings | LlamaCppEndpointSettings | OpenAIEndpointSettings): An instance of Llama, LlamaLLMSettings, LlamaCppEndpointSettings or LlamaCppServerLLMSettings as LLM.
-        llama_generation_settings (LlamaLLMGenerationSettings | LlamaCppGenerationSettings | OpenAIGenerationSettings): Generation settings for Llama.
-        messages_formatter_type (MessagesFormatterType): Type of messages formatter.
-        custom_messages_formatter (MessagesFormatter): Optional Custom messages formatter.
-        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-        k_last_messages_from_chat_history (int): Number of last messages to consider from chat history.
-        system_prompt (str): System prompt for interaction.
-        llama_cpp_function_tools(List[LlamaCppFunctionTool]): List of LlamaCppFunctionTool instances.
-        allow_parallel_function_calling (bool): Allow parallel function calling (Default=False)
-        add_send_message_to_user_function (bool): Flag to add send_message_to_user function.
-        send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
-        debug_output (bool): Enable debug output.
-
-    Attributes:
-        send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
-        llama_cpp_tools (List[LlamaCppFunctionTool]): List of LlamaCppFunctionTool instances.
-        tool_registry (LlamaCppFunctionToolRegistry): Function tool registry.
-        llama_generation_settings (LlamaLLMGenerationSettings): Generation settings for Llama.
-        system_prompt (str): System prompt for interaction.
-        llama_cpp_agent (LlamaCppAgent): LlamaCppAgent instance for interaction.
-        k_last_messages_from_chat_history (int): Number of last messages to consider from chat history.
-        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-
-    Methods:
-        save(file_path: str): Save the agent's state to a file.
-        load_from_file(file_path: str, llama_llm, python_functions, pydantic_functions, send_message_to_user_callback, streaming_callback) -> FunctionCallingAgent:
-            Load the agent's state from a file.
-        load_from_dict(agent_dict: dict) -> FunctionCallingAgent: Load the agent's state from a dictionary.
-        as_dict() -> dict: Convert the agent's state to a dictionary.
-        generate_response(message: str): Generate a response based on the input message.
-        send_message_to_user(message: str): Send a message to the user.
-
-    """
-
-    def __init__(
-        self,
-        llama_llm: LlmProvider,
-        messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
-        custom_messages_formatter: MessagesFormatter = None,
-        streaming_callback: Callable[[StreamingResponse], None] = None,
-        k_last_messages_from_chat_history: int = 0,
-        system_prompt: str = None,
-        llama_cpp_function_tools: [LlamaCppFunctionTool] = None,
-        basic_file_tools: bool = False,
-        allow_parallel_function_calling=False,
-        add_send_message_to_user_function: bool = True,
-        send_message_to_user_callback: Callable[[str], None] = None,
-        debug_output: bool = False,
-    ):
-        """
-        Initialize the FunctionCallingAgent.
-
-        Args:
-            llama_llm (LlmProvider): The LLM Provider.
-            messages_formatter_type (MessagesFormatterType): Type of messages formatter.
-            custom_messages_formatter (MessagesFormatter): Optional Custom messages formatter.
-            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-            k_last_messages_from_chat_history (int): Number of last messages to consider from chat history.
-            system_prompt (str): System prompt for interaction.
-            llama_cpp_function_tools(List[LlamaCppFunctionTool]): List of LlamaCppFunctionTool instances.
-            allow_parallel_function_calling (bool): Allow parallel function calling (Default=False)
-            add_send_message_to_user_function (bool): Flag to add send_message_to_user function.
-            send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
-            debug_output (bool): Enable debug output.
-        """
-        self.llama_cpp_tools = []
-        if llama_cpp_function_tools:
-            self.llama_cpp_tools = llama_cpp_function_tools
-
-        self.send_message_to_user_callback = send_message_to_user_callback
-        if add_send_message_to_user_function:
-            self.llama_cpp_tools.append(LlamaCppFunctionTool(send_message, agent=self))
-
-        if basic_file_tools:
-            self.llama_cpp_tools.append(LlamaCppFunctionTool(read_text_file))
-            self.llama_cpp_tools.append(
-                LlamaCppFunctionTool(write_text_file, agent=self)
-            )
-
-        self.allow_parallel_function_calling = allow_parallel_function_calling
-
-        self.structured_output_settings = (
-            LlmStructuredOutputSettings.from_llama_cpp_function_tools(
-                self.llama_cpp_tools, self.allow_parallel_function_calling
-            )
-        )
-
-        self.without_grammar_mode = False
-        self.without_grammar_mode_function = []
-        self.prompt_suffix = ""
-        if system_prompt is not None:
-            self.system_prompt = system_prompt
-        else:
-            self.system_prompt = """You are Funky, an AI assistant that calls functions to perform tasks."""
-        self.llama_cpp_agent = LlamaCppAgent(
-            llama_llm,
-            debug_output=debug_output,
-            system_prompt=self.system_prompt,
-            predefined_messages_formatter_type=messages_formatter_type,
-            custom_messages_formatter=custom_messages_formatter,
-        )
-
-        self.k_last_messages_from_chat_history = k_last_messages_from_chat_history
-        self.streaming_callback = streaming_callback
-
-
-    @staticmethod
-    def load_from_dict(agent_dict: dict) -> "FunctionCallingAgent":
-        """
-        Load the agent's state from a dictionary.
-
-        Args:
-            agent_dict (dict): The dictionary containing the agent's state.
-
-        Returns:
-            FunctionCallingAgent: The loaded FunctionCallingAgent instance.
-        """
-        return FunctionCallingAgent(**agent_dict)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the agent's state to a dictionary.
-
-        Returns:
-           dict: The dictionary representation of the agent's state.
-        """
-        return self.__dict__
-
-    def generate_response(
-        self,
-        message: str,
-        llm_sampling_settings: LlmSamplingSettings = None,
-        structured_output_settings: LlmStructuredOutputSettings = None,
-    ):
-        self.llama_cpp_agent.add_message(role="user", message=message)
-
-        result = self.intern_get_response(llm_sampling_settings=llm_sampling_settings)
-
-        while True:
-            if isinstance(result, str):
-                if len(self.without_grammar_mode_function) > 0:
-                    func_list = []
-                    for func in self.without_grammar_mode_function:
-                        if func.__name__ not in func_list:
-                            func(result.strip())
-                            func_list.append(func.__name__)
-                break
-            function_message = f"""Function Calling Results:\n\n"""
-            count = 0
-            if result is not None:
-                agent_sent_message = False
-                for res in result:
-                    count += 1
-                    if res["function"] == "send_message":
-                        agent_sent_message = True
-                    if not isinstance(res, str):
-                        if "params" in res:
-                            function_message += f"""{count}. Function: "{res["function"]}"\nArguments: "{res["params"]}"\nReturn Value: {res["return_value"]}\n\n"""
-                        else:
-                            function_message += f"""{count}. Function: "{res["function"]}"\nReturn Value: {res["return_value"]}\n\n"""
-                    else:
-                        function_message += f"{count}. " + res + "\n\n"
-                self.llama_cpp_agent.add_message(
-                    role="tool", message=function_message.strip()
-                )
-                if agent_sent_message:
-                    break
-            result = self.intern_get_response(
-                llm_sampling_settings=llm_sampling_settings
-            )
-        return result
-
-    def intern_get_response(
-        self,
-        llm_sampling_settings: List[str] = None,
-        structured_output_settings: LlmStructuredOutputSettings = None,
-    ):
-        without_grammar_mode = False
-        if self.without_grammar_mode:
-            without_grammar_mode = True
-            self.without_grammar_mode = False
-        result = self.llama_cpp_agent.get_chat_response(
-            streaming_callback=self.streaming_callback,
-            structured_output_settings=self.structured_output_settings
-            if structured_output_settings is None
-            else structured_output_settings,
-            llm_sampling_settings=llm_sampling_settings,
-        )
-        if without_grammar_mode:
-            self.prompt_suffix = ""
-        return result
-
-    def send_message_to_user(self, message: str):
-        """
-        Send a message to the user.
-
-        Args:
-            message: The message send to the user.
-        """
-        if self.send_message_to_user_callback:
-            self.send_message_to_user_callback(message)
-        else:
-            print(message)
+import datetime
+import json
+import os
+from copy import copy
+from typing import Type, List, Callable, Union, Literal
+
+from llama_cpp import Llama
+from pydantic import BaseModel, Field
+
+from .llm_output_settings import LlmStructuredOutputSettings, LlmStructuredOutputType
+
+from .llm_agent import LlamaCppAgent, StreamingResponse
+from .messages_formatter import MessagesFormatterType, MessagesFormatter
+from .function_calling import LlamaCppFunctionTool
+
+from .providers.provider_base import LlmProvider, LlmSamplingSettings
+
+
+class activate_message_mode(BaseModel):
+    """
+    Activates message mode.
+    """
+
+    def run(self, agent: "FunctionCallingAgent"):
+        agent.without_grammar_mode = True
+        agent.prompt_suffix = "\nWrite message in plain text format:"
+        agent.without_grammar_mode_function.append(agent.send_message_to_user)
+        return True
+
+
+class send_message(BaseModel):
+    """
+    Sends a message to the user.
+    """
+
+    content: str = Field(..., description="Content of the message to be sent.")
+
+    def run(self, agent: "FunctionCallingAgent"):
+        agent.send_message_to_user(self.content)
+        return "Message sent."
+
+
+class write_text_file(BaseModel):
+    """
+    Writes content to a file.
+    """
+
+    file_path: str = Field(..., description="The path to the file.")
+    content: str = Field(..., description="The content to write to the file.")
+
+    def run(self, agent: "FunctionCallingAgent"):
+        self.write_file(self.content)
+        return True
+
+    def write_file(self, content: str):
+        """
+        Write content to a file.
+
+        Args:
+            content (str): The content to write to the file.
+        """
+        with open(self.file_path, "w", encoding="utf-8") as file:
+            file.write(content)
+        return None
+
+
+class read_text_file(BaseModel):
+    """
+    Reads the content of a file.
+    """
+
+    file_path: str = Field(..., description="The path to the file.")
+
+    def run(self):
+        return self.read_file()
+
+    def read_file(self):
+        """
+        Reads the content of a file.
+        """
+        if os.path.exists(self.file_path):
+            with open(self.file_path, "r", encoding="utf-8") as file:
+                return file.read()
+        else:
+            return f"File not found."
+
+
+class FunctionCallingAgent:
+    """
+    An agent that uses function calling to interact with its environment and the user.
+
+    Args:
+        llama_llm (Llama | LlamaLLMSettings | LlamaCppEndpointSettings | OpenAIEndpointSettings): An instance of Llama, LlamaLLMSettings, LlamaCppEndpointSettings or LlamaCppServerLLMSettings as LLM.
+        llama_generation_settings (LlamaLLMGenerationSettings | LlamaCppGenerationSettings | OpenAIGenerationSettings): Generation settings for Llama.
+        messages_formatter_type (MessagesFormatterType): Type of messages formatter.
+        custom_messages_formatter (MessagesFormatter): Optional Custom messages formatter.
+        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+        k_last_messages_from_chat_history (int): Number of last messages to consider from chat history.
+        system_prompt (str): System prompt for interaction.
+        llama_cpp_function_tools(List[LlamaCppFunctionTool]): List of LlamaCppFunctionTool instances.
+        allow_parallel_function_calling (bool): Allow parallel function calling (Default=False)
+        add_send_message_to_user_function (bool): Flag to add send_message_to_user function.
+        send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
+        debug_output (bool): Enable debug output.
+
+    Attributes:
+        send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
+        llama_cpp_tools (List[LlamaCppFunctionTool]): List of LlamaCppFunctionTool instances.
+        tool_registry (LlamaCppFunctionToolRegistry): Function tool registry.
+        llama_generation_settings (LlamaLLMGenerationSettings): Generation settings for Llama.
+        system_prompt (str): System prompt for interaction.
+        llama_cpp_agent (LlamaCppAgent): LlamaCppAgent instance for interaction.
+        k_last_messages_from_chat_history (int): Number of last messages to consider from chat history.
+        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+
+    Methods:
+        save(file_path: str): Save the agent's state to a file.
+        load_from_file(file_path: str, llama_llm, python_functions, pydantic_functions, send_message_to_user_callback, streaming_callback) -> FunctionCallingAgent:
+            Load the agent's state from a file.
+        load_from_dict(agent_dict: dict) -> FunctionCallingAgent: Load the agent's state from a dictionary.
+        as_dict() -> dict: Convert the agent's state to a dictionary.
+        generate_response(message: str): Generate a response based on the input message.
+        send_message_to_user(message: str): Send a message to the user.
+
+    """
+
+    def __init__(
+        self,
+        llama_llm: LlmProvider,
+        messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
+        custom_messages_formatter: MessagesFormatter = None,
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+        k_last_messages_from_chat_history: int = 0,
+        system_prompt: str = None,
+        llama_cpp_function_tools: [LlamaCppFunctionTool] = None,
+        basic_file_tools: bool = False,
+        allow_parallel_function_calling=False,
+        add_send_message_to_user_function: bool = True,
+        send_message_to_user_callback: Callable[[str], None] = None,
+        debug_output: bool = False,
+    ):
+        """
+        Initialize the FunctionCallingAgent.
+
+        Args:
+            llama_llm (LlmProvider): The LLM Provider.
+            messages_formatter_type (MessagesFormatterType): Type of messages formatter.
+            custom_messages_formatter (MessagesFormatter): Optional Custom messages formatter.
+            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+            k_last_messages_from_chat_history (int): Number of last messages to consider from chat history.
+            system_prompt (str): System prompt for interaction.
+            llama_cpp_function_tools(List[LlamaCppFunctionTool]): List of LlamaCppFunctionTool instances.
+            allow_parallel_function_calling (bool): Allow parallel function calling (Default=False)
+            add_send_message_to_user_function (bool): Flag to add send_message_to_user function.
+            send_message_to_user_callback (Callable[[str], None]): Callback for sending a message to the user.
+            debug_output (bool): Enable debug output.
+        """
+        self.llama_cpp_tools = []
+        if llama_cpp_function_tools:
+            self.llama_cpp_tools = llama_cpp_function_tools
+
+        self.send_message_to_user_callback = send_message_to_user_callback
+        if add_send_message_to_user_function:
+            self.llama_cpp_tools.append(LlamaCppFunctionTool(send_message, agent=self))
+
+        if basic_file_tools:
+            self.llama_cpp_tools.append(LlamaCppFunctionTool(read_text_file))
+            self.llama_cpp_tools.append(
+                LlamaCppFunctionTool(write_text_file, agent=self)
+            )
+
+        self.allow_parallel_function_calling = allow_parallel_function_calling
+
+        self.structured_output_settings = (
+            LlmStructuredOutputSettings.from_llama_cpp_function_tools(
+                self.llama_cpp_tools, self.allow_parallel_function_calling
+            )
+        )
+
+        self.without_grammar_mode = False
+        self.without_grammar_mode_function = []
+        self.prompt_suffix = ""
+        if system_prompt is not None:
+            self.system_prompt = system_prompt
+        else:
+            self.system_prompt = """You are Funky, an AI assistant that calls functions to perform tasks."""
+        self.llama_cpp_agent = LlamaCppAgent(
+            llama_llm,
+            debug_output=debug_output,
+            system_prompt=self.system_prompt,
+            predefined_messages_formatter_type=messages_formatter_type,
+            custom_messages_formatter=custom_messages_formatter,
+        )
+
+        self.k_last_messages_from_chat_history = k_last_messages_from_chat_history
+        self.streaming_callback = streaming_callback
+
+
+    @staticmethod
+    def load_from_dict(agent_dict: dict) -> "FunctionCallingAgent":
+        """
+        Load the agent's state from a dictionary.
+
+        Args:
+            agent_dict (dict): The dictionary containing the agent's state.
+
+        Returns:
+            FunctionCallingAgent: The loaded FunctionCallingAgent instance.
+        """
+        return FunctionCallingAgent(**agent_dict)
+
+    def as_dict(self) -> dict:
+        """
+        Convert the agent's state to a dictionary.
+
+        Returns:
+           dict: The dictionary representation of the agent's state.
+        """
+        return self.__dict__
+
+    def generate_response(
+        self,
+        message: str,
+        llm_sampling_settings: LlmSamplingSettings = None,
+        structured_output_settings: LlmStructuredOutputSettings = None,
+    ):
+        self.llama_cpp_agent.add_message(role="user", message=message)
+
+        result = self.intern_get_response(llm_sampling_settings=llm_sampling_settings)
+
+        while True:
+            if isinstance(result, str):
+                if len(self.without_grammar_mode_function) > 0:
+                    func_list = []
+                    for func in self.without_grammar_mode_function:
+                        if func.__name__ not in func_list:
+                            func(result.strip())
+                            func_list.append(func.__name__)
+                break
+            function_message = f"""Function Calling Results:\n\n"""
+            count = 0
+            if result is not None:
+                agent_sent_message = False
+                for res in result:
+                    count += 1
+                    if res["function"] == "send_message":
+                        agent_sent_message = True
+                    if not isinstance(res, str):
+                        if "params" in res:
+                            function_message += f"""{count}. Function: "{res["function"]}"\nArguments: "{res["params"]}"\nReturn Value: {res["return_value"]}\n\n"""
+                        else:
+                            function_message += f"""{count}. Function: "{res["function"]}"\nReturn Value: {res["return_value"]}\n\n"""
+                    else:
+                        function_message += f"{count}. " + res + "\n\n"
+                self.llama_cpp_agent.add_message(
+                    role="tool", message=function_message.strip()
+                )
+                if agent_sent_message:
+                    break
+            result = self.intern_get_response(
+                llm_sampling_settings=llm_sampling_settings
+            )
+        return result
+
+    def intern_get_response(
+        self,
+        llm_sampling_settings: List[str] = None,
+        structured_output_settings: LlmStructuredOutputSettings = None,
+    ):
+        without_grammar_mode = False
+        if self.without_grammar_mode:
+            without_grammar_mode = True
+            self.without_grammar_mode = False
+        result = self.llama_cpp_agent.get_chat_response(
+            streaming_callback=self.streaming_callback,
+            structured_output_settings=self.structured_output_settings
+            if structured_output_settings is None
+            else structured_output_settings,
+            llm_sampling_settings=llm_sampling_settings,
+        )
+        if without_grammar_mode:
+            self.prompt_suffix = ""
+        return result
+
+    def send_message_to_user(self, message: str):
+        """
+        Send a message to the user.
+
+        Args:
+            message: The message send to the user.
+        """
+        if self.send_message_to_user_callback:
+            self.send_message_to_user_callback(message)
+        else:
+            print(message)
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,1319 +1,1319 @@
-from __future__ import annotations
-
-import inspect
-import json
-import re
-import typing
-from copy import copy
-from enum import Enum
-from inspect import getdoc, isclass
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    List,
-    Optional,
-    Union,
-    get_args,
-    get_origin,
-    get_type_hints,
-)
-
-from docstring_parser import parse
-from pydantic import BaseModel, Field, create_model
-
-from llama_cpp_agent.llm_documentation import (
-    generate_markdown_documentation,
-    generate_text_documentation,
-)
-
-if TYPE_CHECKING:
-    from types import GenericAlias
-    from types import UnionType
-else:
-    # python 3.8 compat
-    from typing import _GenericAlias as GenericAlias
-    from types import UnionType
-
-
-class PydanticDataType(Enum):
-    """
-    Defines the data types supported by the grammar_generator.
-
-    Attributes:
-        STRING (str): Represents a string data type.
-        BOOLEAN (str): Represents a boolean data type.
-        INTEGER (str): Represents an integer data type.
-        FLOAT (str): Represents a float data type.
-        OBJECT (str): Represents an object data type.
-        ARRAY (str): Represents an array data type.
-        ENUM (str): Represents an enum data type.
-        CUSTOM_CLASS (str): Represents a custom class data type.
-    """
-
-    STRING = "string"
-    TRIPLE_QUOTED_STRING = "triple_quoted_string"
-    MARKDOWN_CODE_BLOCK = "markdown_code_block"
-    BOOLEAN = "boolean"
-    INTEGER = "number"
-    FLOAT = "number"
-    OBJECT = "object"
-    ARRAY = "array"
-    ENUM = "enum"
-    ANY = "any"
-    NULL = "null"
-    CUSTOM_CLASS = "custom-class"
-    CUSTOM_DICT = "custom-dict"
-    SET = "set"
-
-
-def map_pydantic_type_to_gbnf(pydantic_type: type[Any]) -> str:
-    if isclass(pydantic_type) and issubclass(pydantic_type, str):
-        return PydanticDataType.STRING.value
-    elif isclass(pydantic_type) and issubclass(pydantic_type, bool):
-        return PydanticDataType.BOOLEAN.value
-    elif isclass(pydantic_type) and issubclass(pydantic_type, int):
-        return PydanticDataType.INTEGER.value
-    elif isclass(pydantic_type) and issubclass(pydantic_type, float):
-        return PydanticDataType.FLOAT.value
-    elif isclass(pydantic_type) and issubclass(pydantic_type, Enum):
-        return PydanticDataType.ENUM.value
-
-    elif isclass(pydantic_type) and issubclass(pydantic_type, BaseModel):
-        return format_model_and_field_name(pydantic_type.__name__)
-    elif get_origin(pydantic_type) is list:
-        element_type = get_args(pydantic_type)[0]
-        return f"{map_pydantic_type_to_gbnf(element_type)}-list"
-    elif get_origin(pydantic_type) is set:
-        element_type = get_args(pydantic_type)[0]
-        return f"{map_pydantic_type_to_gbnf(element_type)}-set"
-    elif get_origin(pydantic_type) is Union or isinstance(pydantic_type, UnionType):
-        union_types = get_args(pydantic_type)
-        union_rules = [map_pydantic_type_to_gbnf(ut) for ut in union_types]
-        return f"union-{'-or-'.join(union_rules)}"
-    elif get_origin(pydantic_type) is Optional:
-        element_type = get_args(pydantic_type)[0]
-        return f"optional-{map_pydantic_type_to_gbnf(element_type)}"
-    elif isclass(pydantic_type):
-        return f"{PydanticDataType.CUSTOM_CLASS.value}-{format_model_and_field_name(pydantic_type.__name__)}"
-    elif get_origin(pydantic_type) is dict:
-        key_type, value_type = get_args(pydantic_type)
-        return f"custom-dict-key-type-{format_model_and_field_name(map_pydantic_type_to_gbnf(key_type))}-value-type-{format_model_and_field_name(map_pydantic_type_to_gbnf(value_type))}"
-    else:
-        return "unknown"
-
-
-def format_model_and_field_name(model_name: str) -> str:
-    parts = re.findall("[A-Z][^A-Z]*", model_name)
-    if not parts:  # Check if the list is empty
-        return model_name.lower().replace("_", "-")
-    return "-".join(part.lower().replace("_", "-") for part in parts)
-
-
-def generate_list_rule(element_type):
-    """
-    Generate a GBNF rule for a list of a given element type.
-
-    :param element_type: The type of the elements in the list (e.g., 'string').
-    :return: A string representing the GBNF rule for a list of the given type.
-    """
-    rule_name = f"{map_pydantic_type_to_gbnf(element_type)}-list"
-    element_rule = map_pydantic_type_to_gbnf(element_type)
-    list_rule = rf'{rule_name} ::= "["  {element_rule} (","  {element_rule})* "]"'
-    return list_rule
-
-
-def get_members_structure(cls, rule_name):
-    if issubclass(cls, Enum):
-        # Handle Enum types
-        members = [
-            f'"\\"{member.value}\\""' for name, member in cls.__members__.items()
-        ]
-        return f"{cls.__name__.lower()} ::= " + " | ".join(members)
-    if cls.__annotations__ and cls.__annotations__ != {}:
-        result = f'{rule_name} ::= "{{"'
-        # Modify this comprehension
-        members = [
-            f'  "\\"{name}\\"" ":"  {map_pydantic_type_to_gbnf(param_type)}'
-            for name, param_type in cls.__annotations__.items()
-            if name != "self"
-        ]
-
-        result += '"," '.join(members)
-        result += '  "}"'
-        return result
-    if rule_name == "custom-class-any":
-        result = f"{rule_name} ::= "
-        result += "value"
-        return result
-
-    init_signature = inspect.signature(cls.__init__)
-    parameters = init_signature.parameters
-    result = f'{rule_name} ::=  "{{"'
-    # Modify this comprehension too
-    members = [
-        f'  "\\"{name}\\"" ":"  {map_pydantic_type_to_gbnf(param.annotation)}'
-        for name, param in parameters.items()
-        if name != "self" and param.annotation != inspect.Parameter.empty
-    ]
-
-    result += '", "'.join(members)
-    result += '  "}"'
-    return result
-
-
-def regex_to_gbnf(regex_pattern: str) -> str:
-    """
-    Translate a basic regex pattern to a GBNF rule.
-    Note: This function handles only a subset of simple regex patterns.
-    """
-    gbnf_rule = regex_pattern
-
-    # Translate common regex components to GBNF
-    gbnf_rule = gbnf_rule.replace("\\d", "[0-9]")
-    gbnf_rule = gbnf_rule.replace("\\s", "[ \t\n]")
-
-    # Handle quantifiers and other regex syntax that is similar in GBNF
-    # (e.g., '*', '+', '?', character classes)
-
-    return gbnf_rule
-
-
-def generate_gbnf_integer_rules(max_digit=None, min_digit=None):
-    """
-
-    Generate GBNF Integer Rules
-
-    Generates GBNF (Generalized Backus-Naur Form) rules for integers based on the given maximum and minimum digits.
-
-    Parameters:
-        max_digit (int): The maximum number of digits for the integer. Default is None.
-        min_digit (int): The minimum number of digits for the integer. Default is None.
-
-    Returns:
-        integer_rule (str): The identifier for the integer rule generated.
-        additional_rules (list): A list of additional rules generated based on the given maximum and minimum digits.
-
-    """
-    additional_rules = []
-
-    # Define the rule identifier based on max_digit and min_digit
-    integer_rule = "integer-part"
-    if max_digit is not None:
-        integer_rule += f"-max{max_digit}"
-    if min_digit is not None:
-        integer_rule += f"-min{min_digit}"
-
-    # Handling Integer Rules
-    if max_digit is not None or min_digit is not None:
-        # Start with an empty rule part
-        integer_rule_part = ""
-
-        # Add mandatory digits as per min_digit
-        if min_digit is not None:
-            integer_rule_part += "[0-9] " * min_digit
-
-        # Add optional digits up to max_digit
-        if max_digit is not None:
-            optional_digits = max_digit - (min_digit if min_digit is not None else 0)
-            integer_rule_part += "".join(["[0-9]? " for _ in range(optional_digits)])
-
-        # Trim the rule part and append it to additional rules
-        integer_rule_part = integer_rule_part.strip()
-        if integer_rule_part:
-            additional_rules.append(f"{integer_rule} ::= {integer_rule_part}")
-
-    return integer_rule, additional_rules
-
-
-def generate_gbnf_float_rules(
-    max_digit=None, min_digit=None, max_precision=None, min_precision=None
-):
-    """
-    Generate GBNF float rules based on the given constraints.
-
-    :param max_digit: Maximum number of digits in the integer part (default: None)
-    :param min_digit: Minimum number of digits in the integer part (default: None)
-    :param max_precision: Maximum number of digits in the fractional part (default: None)
-    :param min_precision: Minimum number of digits in the fractional part (default: None)
-    :return: A tuple containing the float rule and additional rules as a list
-
-    Example Usage:
-    max_digit = 3
-    min_digit = 1
-    max_precision = 2
-    min_precision = 1
-    generate_gbnf_float_rules(max_digit, min_digit, max_precision, min_precision)
-
-    Output:
-    ('float-3-1-2-1', ['integer-part-max3-min1 ::= [0-9] [0-9] [0-9]?', 'fractional-part-max2-min1 ::= [0-9] [0-9]?', 'float-3-1-2-1 ::= integer-part-max3-min1 "." fractional-part-max2-min
-    *1'])
-
-    Note:
-    GBNF stands for Generalized Backus-Naur Form, which is a notation technique to specify the syntax of programming languages or other formal grammars.
-    """
-    additional_rules = []
-
-    # Define the integer part rule
-    integer_part_rule = (
-        "integer-part"
-        + (f"-max{max_digit}" if max_digit is not None else "")
-        + (f"-min{min_digit}" if min_digit is not None else "")
-    )
-
-    # Define the fractional part rule based on precision constraints
-    fractional_part_rule = "fractional-part"
-    fractional_rule_part = ""
-    if max_precision is not None or min_precision is not None:
-        fractional_part_rule += (
-            f"-max{max_precision}" if max_precision is not None else ""
-        ) + (f"-min{min_precision}" if min_precision is not None else "")
-        # Minimum number of digits
-        fractional_rule_part = "[0-9]" * (
-            min_precision if min_precision is not None else 1
-        )
-        # Optional additional digits
-        fractional_rule_part += "".join(
-            [" [0-9]?"]
-            * (
-                (max_precision - (min_precision if min_precision is not None else 1))
-                if max_precision is not None
-                else 0
-            )
-        )
-        additional_rules.append(f"{fractional_part_rule} ::= {fractional_rule_part}")
-
-    # Define the float rule
-    float_rule = f"float-{max_digit if max_digit is not None else 'X'}-{min_digit if min_digit is not None else 'X'}-{max_precision if max_precision is not None else 'X'}-{min_precision if min_precision is not None else 'X'}"
-    additional_rules.append(
-        f'{float_rule} ::= {integer_part_rule} "." {fractional_part_rule}'
-    )
-
-    # Generating the integer part rule definition, if necessary
-    if max_digit is not None or min_digit is not None:
-        integer_rule_part = "[0-9]"
-        if min_digit is not None and min_digit > 1:
-            integer_rule_part += " [0-9]" * (min_digit - 1)
-        if max_digit is not None:
-            integer_rule_part += "".join(
-                [" [0-9]?"] * (max_digit - (min_digit if min_digit is not None else 1))
-            )
-        additional_rules.append(f"{integer_part_rule} ::= {integer_rule_part.strip()}")
-
-    return float_rule, additional_rules
-
-
-def generate_gbnf_rule_for_type(
-    model_name,
-    field_name,
-    field_type,
-    is_optional,
-    processed_models,
-    created_rules,
-    field_info=None,
-) -> tuple[str, list[str]]:
-    """
-    Generate GBNF rule for a given field type.
-
-    :param model_name: Name of the model.
-
-    :param field_name: Name of the field.
-    :param field_type: Type of the field.
-    :param is_optional: Whether the field is optional.
-    :param processed_models: List of processed models.
-    :param created_rules: List of created rules.
-    :param field_info: Additional information about the field (optional).
-
-    :return: Tuple containing the GBNF type and a list of additional rules.
-    :rtype: tuple[str, list]
-    """
-    rules = []
-
-    field_name = format_model_and_field_name(field_name)
-    gbnf_type = map_pydantic_type_to_gbnf(field_type)
-
-    if isclass(field_type) and issubclass(field_type, BaseModel):
-        nested_model_name = format_model_and_field_name(field_type.__name__)
-        nested_model_rules, _ = generate_gbnf_grammar(
-            field_type, processed_models, created_rules
-        )
-        rules.extend(nested_model_rules)
-        gbnf_type, rules = nested_model_name, rules
-    elif isclass(field_type) and issubclass(field_type, Enum):
-        enum_values = [
-            f'"\\"{e.value}\\""' for e in field_type
-        ]  # Adding escaped quotes
-        enum_rule = f"{model_name}-{field_name} ::= {' | '.join(enum_values)}"
-        rules.append(enum_rule)
-        gbnf_type, rules = model_name + "-" + field_name, rules
-    elif get_origin(field_type) == list:  # Array
-        element_type = get_args(field_type)[0]
-        element_rule_name, additional_rules = generate_gbnf_rule_for_type(
-            model_name,
-            f"{field_name}-element",
-            element_type,
-            is_optional,
-            processed_models,
-            created_rules,
-        )
-        rules.extend(additional_rules)
-        array_rule = rf"""{model_name}-{field_name} ::= "[" ws ({element_rule_name})? ("," ws {element_rule_name})* ws "]" """
-        rules.append(array_rule)
-        gbnf_type, rules = model_name + "-" + field_name, rules
-
-    elif get_origin(field_type) == set or field_type == set:  # Array
-        element_type = get_args(field_type)[0]
-        element_rule_name, additional_rules = generate_gbnf_rule_for_type(
-            model_name,
-            f"{field_name}-element",
-            element_type,
-            is_optional,
-            processed_models,
-            created_rules,
-        )
-        rules.extend(additional_rules)
-        array_rule = rf"""{model_name}-{field_name} ::= "[" ws ({element_rule_name})? ("," ws {element_rule_name})* ws "]" """
-        rules.append(array_rule)
-        gbnf_type, rules = model_name + "-" + field_name, rules
-
-    elif gbnf_type.startswith("custom-class-"):
-        rules.append(get_members_structure(field_type, gbnf_type))
-    elif gbnf_type.startswith("custom-dict-"):
-        key_type, value_type = get_args(field_type)
-
-        additional_key_type, additional_key_rules = generate_gbnf_rule_for_type(
-            model_name,
-            f"{field_name}-key-type",
-            key_type,
-            is_optional,
-            processed_models,
-            created_rules,
-        )
-        additional_value_type, additional_value_rules = generate_gbnf_rule_for_type(
-            model_name,
-            f"{field_name}-value-type",
-            value_type,
-            is_optional,
-            processed_models,
-            created_rules,
-        )
-        rules.extend(
-            [
-                rf'{gbnf_type} ::= "{{"  ( {additional_key_type} ": "  {additional_value_type} ("," "\n" ws {additional_key_type} ":"  {additional_value_type})*  )? "}}" '
-            ]
-        )
-        rules.extend(additional_key_rules)
-        rules.extend(additional_value_rules)
-    elif gbnf_type.startswith("union-"):
-        union_types = get_args(field_type)
-        union_rules = []
-
-        for union_type in union_types:
-            if isinstance(union_type, GenericAlias):
-                union_gbnf_type, union_rules_list = generate_gbnf_rule_for_type(
-                    model_name,
-                    field_name,
-                    union_type,
-                    False,
-                    processed_models,
-                    created_rules,
-                )
-                union_rules.append(union_gbnf_type)
-                rules.extend(union_rules_list)
-
-            elif not issubclass(union_type, type(None)):
-                union_gbnf_type, union_rules_list = generate_gbnf_rule_for_type(
-                    model_name,
-                    field_name,
-                    union_type,
-                    False,
-                    processed_models,
-                    created_rules,
-                )
-                union_rules.append(union_gbnf_type)
-                rules.extend(union_rules_list)
-
-        # Defining the union grammar rule separately
-        if len(union_rules) == 1:
-            union_grammar_rule = f"{model_name}-{field_name}-optional ::= {' | '.join(union_rules)} | null"
-        else:
-            uni = []
-            for rule in union_rules:
-                if rule not in uni:
-                    uni.append(rule)
-            union_grammar_rule = (
-                f"{model_name}-{field_name}-union ::= {' | '.join(uni)}"
-            )
-        rules.append(union_grammar_rule)
-        if len(union_rules) == 1:
-            gbnf_type = f"{model_name}-{field_name}-optional"
-        else:
-            gbnf_type = f"{model_name}-{field_name}-union"
-    elif isclass(field_type) and issubclass(field_type, str):
-        if (
-            field_info
-            and hasattr(field_info, "json_schema_extra")
-            and field_info.json_schema_extra is not None
-        ):
-            triple_quoted_string = field_info.json_schema_extra.get(
-                "triple_quoted_string", False
-            )
-            markdown_string = field_info.json_schema_extra.get(
-                "markdown_code_block", False
-            )
-
-            gbnf_type = (
-                PydanticDataType.TRIPLE_QUOTED_STRING.value
-                if triple_quoted_string
-                else PydanticDataType.STRING.value
-            )
-            gbnf_type = (
-                PydanticDataType.MARKDOWN_CODE_BLOCK.value
-                if markdown_string
-                else gbnf_type
-            )
-
-        elif field_info and hasattr(field_info, "pattern"):
-            # Convert regex pattern to grammar rule
-            regex_pattern = field_info.regex.pattern
-            gbnf_type = f"pattern-{field_name} ::= {regex_to_gbnf(regex_pattern)}"
-        else:
-            gbnf_type = PydanticDataType.STRING.value
-
-    elif (
-        isclass(field_type)
-        and issubclass(field_type, float)
-        and field_info
-        and hasattr(field_info, "json_schema_extra")
-        and field_info.json_schema_extra is not None
-    ):
-        # Retrieve precision attributes for floats
-        max_precision = (
-            field_info.json_schema_extra.get("max_precision")
-            if field_info and hasattr(field_info, "json_schema_extra")
-            else None
-        )
-        min_precision = (
-            field_info.json_schema_extra.get("min_precision")
-            if field_info and hasattr(field_info, "json_schema_extra")
-            else None
-        )
-        max_digits = (
-            field_info.json_schema_extra.get("max_digit")
-            if field_info and hasattr(field_info, "json_schema_extra")
-            else None
-        )
-        min_digits = (
-            field_info.json_schema_extra.get("min_digit")
-            if field_info and hasattr(field_info, "json_schema_extra")
-            else None
-        )
-
-        # Generate GBNF rule for float with given attributes
-        gbnf_type, rules = generate_gbnf_float_rules(
-            max_digit=max_digits,
-            min_digit=min_digits,
-            max_precision=max_precision,
-            min_precision=min_precision,
-        )
-
-    elif (
-        isclass(field_type)
-        and issubclass(field_type, int)
-        and field_info
-        and hasattr(field_info, "json_schema_extra")
-        and field_info.json_schema_extra is not None
-    ):
-        # Retrieve digit attributes for integers
-        max_digits = (
-            field_info.json_schema_extra.get("max_digit")
-            if field_info and hasattr(field_info, "json_schema_extra")
-            else None
-        )
-        min_digits = (
-            field_info.json_schema_extra.get("min_digit")
-            if field_info and hasattr(field_info, "json_schema_extra")
-            else None
-        )
-
-        # Generate GBNF rule for integer with given attributes
-        gbnf_type, rules = generate_gbnf_integer_rules(
-            max_digit=max_digits, min_digit=min_digits
-        )
-    else:
-        gbnf_type, rules = gbnf_type, []
-
-    return gbnf_type, rules
-
-
-def generate_gbnf_grammar(
-    model: type[BaseModel],
-    processed_models: set[type[BaseModel]],
-    created_rules: dict[str, list[str]],
-) -> tuple[list[str], bool]:
-    """
-
-    Generate GBnF Grammar
-
-    Generates a GBnF grammar for a given model.
-
-    :param model: A Pydantic model class to generate the grammar for. Must be a subclass of BaseModel.
-    :param processed_models: A set of already processed models to prevent infinite recursion.
-    :param created_rules: A dict containing already created rules to prevent duplicates.
-    :return: A list of GBnF grammar rules in string format. And two booleans indicating if an extra markdown or triple quoted string is in the grammar.
-    Example Usage:
-    ```
-    model = MyModel
-    processed_models = set()
-    created_rules = dict()
-
-    gbnf_grammar = generate_gbnf_grammar(model, processed_models, created_rules)
-    ```
-    """
-    if model in processed_models:
-        return [], False
-
-    processed_models.add(model)
-    model_name = format_model_and_field_name(model.__name__)
-
-    if not issubclass(model, BaseModel):
-        # For non-Pydantic classes, generate model_fields from __annotations__ or __init__
-        if hasattr(model, "__annotations__") and model.__annotations__:
-            model_fields = {
-                name: (typ, ...) for name, typ in model.__annotations__.items()
-            }
-        else:
-            init_signature = inspect.signature(model.__init__)
-            parameters = init_signature.parameters
-            model_fields = {
-                name: (param.annotation, param.default)
-                for name, param in parameters.items()
-                if name != "self"
-            }
-    else:
-        # For Pydantic models, use model_fields and check for ellipsis (required fields)
-        model_fields = model.__annotations__
-
-    model_rule_parts = []
-    nested_rules = []
-    has_markdown_code_block = False
-    has_triple_quoted_string = False
-    look_for_markdown_code_block = False
-    look_for_triple_quoted_string = False
-    for field_name, field_info in model_fields.items():
-        if not issubclass(model, BaseModel):
-            field_type, default_value = field_info
-            # Check if the field is optional (not required)
-            is_optional = (default_value is not inspect.Parameter.empty) and (
-                default_value is not Ellipsis
-            )
-        else:
-            field_type = field_info
-            field_info = model.model_fields[field_name]
-            is_optional = (
-                field_info.is_required is False and get_origin(field_type) is Optional
-            )
-        rule_name, additional_rules = generate_gbnf_rule_for_type(
-            model_name,
-            format_model_and_field_name(field_name),
-            field_type,
-            is_optional,
-            processed_models,
-            created_rules,
-            field_info,
-        )
-        look_for_markdown_code_block = (
-            True if rule_name == "markdown_code_block" else False
-        )
-        look_for_triple_quoted_string = (
-            True if rule_name == "triple_quoted_string" else False
-        )
-        if not look_for_markdown_code_block and not look_for_triple_quoted_string:
-            if rule_name not in created_rules:
-                created_rules[rule_name] = additional_rules
-            model_rule_parts.append(
-                f' ws "\\"{field_name}\\"" ": " {rule_name}'
-            )  # Adding escaped quotes
-            nested_rules.extend(additional_rules)
-        else:
-            has_triple_quoted_string = look_for_triple_quoted_string
-            has_markdown_code_block = look_for_markdown_code_block
-
-    fields_joined = r' "," '.join(model_rule_parts)
-    if fields_joined != "":
-        model_rule = rf'{model_name} ::= "{{" {fields_joined} ws "}}"'
-    else:
-        model_rule = rf'{model_name} ::= "{{" "}}"'
-
-    has_special_string = False
-    if has_triple_quoted_string:
-        model_rule += '"\\n" ws "}"'
-        model_rule += '"\\n" triple-quoted-string'
-        has_special_string = True
-    if has_markdown_code_block:
-        model_rule += '"\\n" ws "}"'
-        model_rule += '"\\n" markdown-code-block'
-        has_special_string = True
-    all_rules = [model_rule] + nested_rules
-
-    return all_rules, has_special_string
-
-
-def generate_gbnf_grammar_from_pydantic_models(
-    models: list[BaseModel],
-    outer_object_name: str | None = None,
-    outer_object_content: str | None = None,
-    list_of_outputs: bool = False,
-    add_inner_thoughts: bool = True,
-    allow_only_inner_thoughts: bool = True,
-    inner_thought_field_name: str = "chain_of_thought",
-    add_request_heartbeat: bool = True,
-    request_heartbeat_field_name: str = "request_heartbeat",
-    request_heartbeat_models: list[str] = None,
-) -> str:
-    """
-    Generate GBNF Grammar from Pydantic Models.
-
-    This method takes a list of Pydantic models and uses them to generate a GBNF grammar string. The generated grammar string can be used for parsing and validating data using the generated
-    * grammar.
-
-    Args:
-        models (list[type[BaseModel]]): A list of Pydantic models to generate the grammar from.
-        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
-        outer_object_content (str): Content for the outer rule in the GBNF grammar. Eg. "function_parameters" or "params" for function calling.
-        list_of_outputs (str, optional): Allows a list of output objects
-        add_inner_thoughts (bool, optional): Add inner thoughts to the grammar. Defaults to True.
-        allow_only_inner_thoughts (bool, optional): Allow only inner thoughts. Defaults to True.
-    Returns:
-        str: The generated GBNF grammar string.
-
-    Examples:
-        models = [UserModel, PostModel]
-        grammar = generate_gbnf_grammar_from_pydantic(models)
-        print(grammar)
-        # Output:
-        # root ::= UserModel | PostModel
-        # ...
-    """
-    if request_heartbeat_models is None:
-        request_heartbeat_models = []
-    processed_models: set[type[BaseModel]] = set()
-    all_rules = []
-    created_rules: dict[str, list[str]] = {}
-    if outer_object_name is None:
-        for model in models:
-            model_rules, _ = generate_gbnf_grammar(
-                model, processed_models, created_rules
-            )
-            all_rules.extend(model_rules)
-
-        if list_of_outputs:
-            root_rule = (
-                r'root ::= (" "| "\n") "[" ws grammar-models ("," ws grammar-models)* "\n" "]"'
-                + "\n"
-            )
-        else:
-            root_rule = r'root ::= (" "| "\n") grammar-models' + "\n"
-        root_rule += "grammar-models ::= " + " | ".join(
-            [format_model_and_field_name(model.__name__) for model in models]
-        )
-        all_rules.insert(0, root_rule)
-        return "\n".join(all_rules) + get_primitive_grammar("\n".join(all_rules))
-    elif outer_object_name is not None:
-        if list_of_outputs:
-            root_rule = (
-                rf'root ::= (" "| "\n") "[" ws {format_model_and_field_name(outer_object_name)} ("," ws {format_model_and_field_name(outer_object_name)})* "\n" "]"'
-                + "\n"
-            )
-        else:
-            root_rule = f"root ::= {format_model_and_field_name(outer_object_name)}\n"
-
-        if add_inner_thoughts:
-            if allow_only_inner_thoughts:
-                model_rule = rf'{format_model_and_field_name(outer_object_name)} ::= (" "| "\n") "{{" ws "\"{inner_thought_field_name}\""  ":" ws string (("," ws "\"{outer_object_name}\""  ":" ws grammar-models)? | ws "}}")'
-            else:
-                model_rule = rf'{format_model_and_field_name(outer_object_name)} ::= (" "| "\n") "{{" ws "\"{inner_thought_field_name}\""  ":" ws string "," ws "\"{outer_object_name}\""  ":" ws grammar-models '
-        else:
-            model_rule = rf'{format_model_and_field_name(outer_object_name)} ::= (" "| "\n") "{{" ws "\"{outer_object_name}\""  ": " ws grammar-models'
-
-        fields_joined = " | ".join(
-            [
-                rf"{format_model_and_field_name(model.__name__)}-grammar-model"
-                for model in models
-            ]
-        )
-
-        grammar_model_rules = f"\ngrammar-models ::= {fields_joined}"
-        mod_rules = []
-        for model in models:
-            mod_rule = (
-                rf"{format_model_and_field_name(model.__name__)}-grammar-model ::= "
-            )
-            mod_rule += (
-                rf'"\"{model.__name__}\"" "," ws "\"{outer_object_content}\"" ": " {format_model_and_field_name(model.__name__)}'
-                + "\n"
-            )
-            mod_rules.append(mod_rule)
-        grammar_model_rules += "\n" + "\n".join(mod_rules)
-
-        for model in models:
-            model_rules, has_special_string = generate_gbnf_grammar(
-                model, processed_models, created_rules
-            )
-            if add_request_heartbeat and model.__name__ in request_heartbeat_models:
-                model_rules[
-                    0
-                ] += rf' "," ws "\"{request_heartbeat_field_name}\""  ":" ws boolean '
-            if not has_special_string:
-                model_rules[0] += r' ws "}"'
-
-            all_rules.extend(model_rules)
-
-        all_rules.insert(0, root_rule + model_rule + grammar_model_rules)
-        return "\n".join(all_rules) + get_primitive_grammar("\n".join(all_rules))
-
-
-def get_primitive_grammar(grammar):
-    """
-    Returns the needed GBNF primitive grammar for a given GBNF grammar string.
-
-    Args:
-        grammar (str): The string containing the GBNF grammar.
-
-    Returns:
-        str: GBNF primitive grammar string.
-    """
-    type_list: list[type[object]] = []
-    if "string-list" in grammar:
-        type_list.append(str)
-    if "boolean-list" in grammar:
-        type_list.append(bool)
-    if "integer-list" in grammar:
-        type_list.append(int)
-    if "float-list" in grammar:
-        type_list.append(float)
-    additional_grammar = [generate_list_rule(t) for t in type_list]
-    primitive_grammar = r"""
-boolean ::= "true" | "false"
-null ::= "null"
-string ::= "\"" (
-        [^"\\] |
-        "\\" (["\\/bfnrt] | "u" [0-9a-fA-F] [0-9a-fA-F] [0-9a-fA-F] [0-9a-fA-F])
-      )* "\""
-ws ::= ([ \t\n]+)
-number ::= "-"? ([0-9]+ | [0-9]+ "." [0-9]+) ([eE] [-+]? [0-9]+)?"""
-
-    any_block = ""
-    if "custom-class-any" in grammar:
-        any_block = """
-value ::= object | array | string | number | boolean | null
-
-object ::=
-  "{" ws (
-            string ":" ws value
-    ("," ws string ":" ws value)*
-  )? "}"
-
-array  ::=
-  "[" ws (
-            value
-    ("," ws value)*
-  )? "]"
-"""
-
-    markdown_code_block_grammar = ""
-    if "markdown-code-block" in grammar:
-        markdown_code_block_grammar = r'''
-markdown-code-block ::= opening-triple-ticks markdown-code-block-content closing-triple-ticks
-markdown-code-block-content ::= ( [^`] | "`" [^`] |  "`"  "`" [^`]  )*
-opening-triple-ticks ::= "```" "python" "\n" | "```" "c" "\n" | "```" "cpp" "\n" | "```" "txt" "\n" | "```" "text" "\n" | "```" "json" "\n" | "```" "javascript" "\n" | "```" "css" "\n" | "```" "html" "\n" | "```" "markdown" "\n"
-closing-triple-ticks ::= "```" "\n"'''
-
-    if "triple-quoted-string" in grammar:
-        markdown_code_block_grammar = r"""
-triple-quoted-string ::= triple-quotes triple-quoted-string-content triple-quotes
-triple-quoted-string-content ::= ( [^'] | "'" [^'] |  "'"  "'" [^']  )*
-triple-quotes ::= "'''" """
-    return (
-        "\n"
-        + "\n".join(additional_grammar)
-        + any_block
-        + primitive_grammar
-        + markdown_code_block_grammar
-    )
-
-
-def save_gbnf_grammar_and_documentation(
-    grammar,
-    documentation,
-    grammar_file_path="./grammar.gbnf",
-    documentation_file_path="./grammar_documentation.md",
-):
-    """
-    Save GBNF grammar and documentation to specified files.
-
-    Args:
-        grammar (str): GBNF grammar string.
-        documentation (str): Documentation string.
-        grammar_file_path (str): File path to save the GBNF grammar.
-        documentation_file_path (str): File path to save the documentation.
-
-    Returns:
-        None
-    """
-    try:
-        with open(grammar_file_path, "w") as file:
-            file.write(grammar + get_primitive_grammar(grammar))
-        print(f"Grammar successfully saved to {grammar_file_path}")
-    except IOError as e:
-        print(f"An error occurred while saving the grammar file: {e}")
-
-    try:
-        with open(documentation_file_path, "w") as file:
-            file.write(documentation)
-        print(f"Documentation successfully saved to {documentation_file_path}")
-    except IOError as e:
-        print(f"An error occurred while saving the documentation file: {e}")
-
-
-def remove_empty_lines(string):
-    """
-    Remove empty lines from a string.
-
-    Args:
-        string (str): Input string.
-
-    Returns:
-        str: String with empty lines removed.
-    """
-    lines = string.splitlines()
-    non_empty_lines = [line for line in lines if line.strip() != ""]
-    string_no_empty_lines = "\n".join(non_empty_lines)
-    return string_no_empty_lines
-
-
-def generate_and_save_gbnf_grammar_and_documentation(
-    pydantic_model_list,
-    grammar_file_path="./generated_grammar.gbnf",
-    documentation_file_path="./generated_grammar_documentation.md",
-    outer_object_name: str | None = None,
-    outer_object_content: str | None = None,
-    model_prefix: str = "Output Model",
-    fields_prefix: str = "Output Fields",
-    list_of_outputs: bool = False,
-    documentation_with_field_description=True,
-    add_inner_thoughts: bool = False,
-    allow_only_inner_thoughts: bool = False,
-    inner_thoughts_field_name: str = "thoughts_and_reasoning",
-    add_request_heartbeat: bool = False,
-    request_heartbeat_field_name: str = "request_heartbeat",
-    request_heartbeat_models: List[str] = None,
-):
-    """
-    Generate GBNF grammar and documentation, and save them to specified files.
-
-    Args:
-        pydantic_model_list: List of Pydantic model classes.
-        grammar_file_path (str): File path to save the generated GBNF grammar.
-        documentation_file_path (str): File path to save the generated documentation.
-        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
-        outer_object_content (str): Content for the outer rule in the GBNF grammar. Eg. "function_parameters" or "params" for function calling.
-        model_prefix (str): Prefix for the model section in the documentation.
-        fields_prefix (str): Prefix for the fields section in the documentation.
-        list_of_outputs (bool): Whether the output is a list of items.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-        add_inner_thoughts (bool): Add inner thoughts to the grammar. This is useful for adding comments or reasoning to the output.
-        allow_only_inner_thoughts (bool): Allow only inner thoughts. If True, only inner thoughts will be allowed in the output.
-        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "thoughts_and_reasoning".
-        add_request_heartbeat (bool): Add request heartbeat to the grammar. This allows the LLM to decide when to return control to the system.
-        request_heartbeat_field_name (str): Field name for request heartbeat. Default is "request_heartbeat".
-        request_heartbeat_models (List[str]): List of models that will have a request heartbeat field.
-    Returns:
-        None
-    """
-    documentation = generate_markdown_documentation(
-        pydantic_model_list,
-        model_prefix,
-        fields_prefix,
-        documentation_with_field_description=documentation_with_field_description,
-    )
-    grammar = generate_gbnf_grammar_from_pydantic_models(
-        pydantic_model_list,
-        outer_object_name,
-        outer_object_content,
-        list_of_outputs,
-        add_inner_thoughts,
-        allow_only_inner_thoughts,
-        inner_thoughts_field_name,
-        add_request_heartbeat,
-        request_heartbeat_field_name,
-        request_heartbeat_models,
-    )
-    grammar = remove_empty_lines(grammar)
-    save_gbnf_grammar_and_documentation(
-        grammar, documentation, grammar_file_path, documentation_file_path
-    )
-
-
-def generate_gbnf_grammar_and_documentation(
-    pydantic_model_list,
-    outer_object_name: str | None = None,
-    outer_object_content: str | None = None,
-    model_prefix: str = "Output Model",
-    fields_prefix: str = "Output Fields",
-    list_of_outputs: bool = False,
-    documentation_with_field_description=True,
-    add_inner_thoughts: bool = False,
-    allow_only_inner_thoughts: bool = False,
-    inner_thoughts_field_name: str = "thoughts_and_reasoning",
-    add_request_heartbeat: bool = False,
-    request_heartbeat_field_name: str = "request_heartbeat",
-    request_heartbeat_models: List[str] = None,
-):
-    """
-    Generate GBNF grammar and documentation for a list of Pydantic models.
-
-    Args:
-        pydantic_model_list: List of Pydantic model classes.
-        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
-        outer_object_content (str): Content for the outer rule in the GBNF grammar. E.g., "function_parameters" or "params" for function calling.
-        model_prefix (str): Prefix for the model section in the documentation.
-        fields_prefix (str): Prefix for the fields section in the documentation.
-        list_of_outputs (bool): Whether the output is a list of items.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-        add_inner_thoughts (bool): Add inner thoughts to the grammar. This is useful for adding comments or reasoning to the output.
-        allow_only_inner_thoughts (bool): Allow only inner thoughts. If True, only inner thoughts will be allowed in the output.
-        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "thoughts_and_reasoning".
-        add_request_heartbeat (bool): Add request heartbeat to the grammar. This allows the LLM to decide when to return control to the system.
-        request_heartbeat_field_name (str): Field name for request heartbeat. Default is "request_heartbeat".
-        request_heartbeat_models (List[str]): List of models that will have a request heartbeat field.
-
-    Returns:
-        tuple: GBNF grammar string, documentation string.
-    """
-    documentation = generate_text_documentation(
-        copy(pydantic_model_list),
-        model_prefix,
-        fields_prefix,
-        documentation_with_field_description=documentation_with_field_description,
-    )
-    grammar = generate_gbnf_grammar_from_pydantic_models(
-        pydantic_model_list,
-        outer_object_name,
-        outer_object_content,
-        list_of_outputs,
-        add_inner_thoughts,
-        allow_only_inner_thoughts,
-        inner_thoughts_field_name,
-        add_request_heartbeat,
-        request_heartbeat_field_name,
-        request_heartbeat_models,
-    )
-    grammar = remove_empty_lines(grammar + get_primitive_grammar(grammar))
-    return grammar, documentation
-
-
-def generate_gbnf_grammar_and_documentation_from_dictionaries(
-    dictionaries: list[dict[str, Any]],
-    outer_object_name: str | None = None,
-    outer_object_content: str | None = None,
-    model_prefix: str = "Output Model",
-    fields_prefix: str = "Output Fields",
-    list_of_outputs: bool = False,
-    documentation_with_field_description=True,
-    add_inner_thoughts: bool = False,
-    allow_only_inner_thoughts: bool = False,
-    inner_thoughts_field_name: str = "thoughts_and_reasoning",
-    add_request_heartbeat: bool = False,
-    request_heartbeat_field_name: str = "request_heartbeat",
-    request_heartbeat_models: List[str] = None,
-):
-    """
-    Generate GBNF grammar and documentation from a list of dictionaries.
-
-    Args:
-        dictionaries (list[dict]): List of dictionaries representing Pydantic models.
-        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
-        outer_object_content (str): Content for the outer rule in the GBNF grammar. Eg. "function_parameters" or "params" for function calling.
-        model_prefix (str): Prefix for the model section in the documentation.
-        fields_prefix (str): Prefix for the fields section in the documentation.
-        list_of_outputs (bool): Whether the output is a list of items.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-        add_inner_thoughts (bool): Add inner thoughts to the grammar. This is useful for adding comments or reasoning to the output.
-        allow_only_inner_thoughts (bool): Allow only inner thoughts. If True, only inner thoughts will be allowed in the output.
-        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "thoughts_and_reasoning".
-        add_request_heartbeat (bool): Add request heartbeat to the grammar. This allows the LLM to decide when to return control to the system.
-        request_heartbeat_field_name (str): Field name for request heartbeat. Default is "request_heartbeat".
-        request_heartbeat_models (List[str]): List of models that will have a request heartbeat field.
-
-    Returns:
-        tuple: GBNF grammar string, documentation string.
-    """
-    pydantic_model_list = create_dynamic_models_from_dictionaries(dictionaries)
-    documentation = generate_markdown_documentation(
-        copy(pydantic_model_list),
-        model_prefix,
-        fields_prefix,
-        documentation_with_field_description=documentation_with_field_description,
-    )
-    grammar = generate_gbnf_grammar_from_pydantic_models(
-        pydantic_model_list,
-        outer_object_name,
-        outer_object_content,
-        list_of_outputs,
-        add_inner_thoughts,
-        allow_only_inner_thoughts,
-        inner_thoughts_field_name,
-        add_request_heartbeat,
-        request_heartbeat_field_name,
-        request_heartbeat_models,
-    )
-    grammar = remove_empty_lines(grammar + get_primitive_grammar(grammar))
-    return grammar, documentation
-
-
-def create_dynamic_model_from_function(
-    func: Callable[..., Any],
-    add_inner_thoughts: bool = False,
-    inner_thoughts_field_name: str = "inner_thoughts",
-):
-    """
-    Creates a dynamic Pydantic model from a given function's type hints and adds the function as a 'run' method.
-
-    Args:
-        func (Callable): A function with type hints from which to create the model.
-        add_inner_thoughts (bool): Add an 'inner_thoughts' field at the params level to the model. Default is False.
-        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "inner_thoughts".
-
-    Returns:
-        A dynamic Pydantic model class with the provided function as a 'run' method.
-    """
-
-    # Get the signature of the function
-    sig = inspect.signature(func)
-
-    # Parse the docstring
-    assert func.__doc__ is not None
-    docstring = parse(func.__doc__)
-
-    dynamic_fields = {}
-    param_docs = []
-    if add_inner_thoughts:
-        dynamic_fields[inner_thoughts_field_name] = (str, None)
-    for param in sig.parameters.values():
-        # Exclude 'self' parameter
-        if param.name == "self":
-            continue
-
-        # Assert that the parameter has a type annotation
-        if param.annotation == inspect.Parameter.empty:
-            raise TypeError(
-                f"Parameter '{param.name}' in function '{func.__name__}' lacks a type annotation"
-            )
-
-        # Find the parameter's description in the docstring
-        param_doc = next(
-            (d for d in docstring.params if d.arg_name == param.name), None
-        )
-
-        # Assert that the parameter has a description
-        if not param_doc or not param_doc.description:
-            raise ValueError(
-                f"Parameter '{param.name}' in function '{func.__name__}' lacks a description in the docstring"
-            )
-
-        # Add parameter details to the schema
-        param_docs.append((param.name, param_doc))
-        if param.default == inspect.Parameter.empty:
-            default_value = ...
-        else:
-            default_value = param.default
-        dynamic_fields[param.name] = (
-            param.annotation if param.annotation != inspect.Parameter.empty else str,
-            default_value,
-        )
-
-    # Creating the dynamic model
-    dynamic_model = create_model(f"{func.__name__}", **dynamic_fields)  # type: ignore[call-overload]
-    if add_inner_thoughts:
-        dynamic_model.model_fields[
-            inner_thoughts_field_name
-        ].description = "Deep inner monologue private to you only."
-    for name, param_doc in param_docs:
-        dynamic_model.model_fields[name].description = param_doc.description
-
-    dynamic_model.__doc__ = (
-        (docstring.short_description if docstring.short_description is not None else "")
-        + "\n"
-        + (docstring.long_description if docstring.long_description is not None else "")
-    )
-
-    def run_method_wrapper(self):
-        func_args = {name: getattr(self, name) for name, _ in dynamic_fields.items()}
-        return func(**func_args)
-
-    # Adding the wrapped function as a 'run' method
-    setattr(dynamic_model, "run", run_method_wrapper)
-    return dynamic_model
-
-
-def add_run_method_to_dynamic_model(model: type[BaseModel], func: Callable[..., Any]):
-    """
-    Add a 'run' method to a dynamic Pydantic model, using the provided function.
-
-    Args:
-        model (type[BaseModel]): Dynamic Pydantic model class.
-        func (Callable): Function to be added as a 'run' method to the model.
-
-    Returns:
-        type[BaseModel]: Pydantic model class with the added 'run' method.
-    """
-
-    def run_method_wrapper(self):
-        func_args = {name: getattr(self, name) for name in model.model_fields}
-        return func(**func_args)
-
-    # Adding the wrapped function as a 'run' method
-    setattr(model, "run", run_method_wrapper)
-
-    return model
-
-
-def create_dynamic_models_from_dictionaries(dictionaries: list[dict[str, Any]]):
-    """
-    Create a list of dynamic Pydantic model classes from a list of dictionaries.
-
-    Args:
-        dictionaries (list[dict]): List of dictionaries representing model structures.
-
-    Returns:
-        list[Type[BaseModel]]: List of generated dynamic Pydantic model classes.
-    """
-    dynamic_models = []
-    for func in dictionaries:
-        model_name = format_model_and_field_name(func.get("name", ""))
-        dyn_model = convert_dictionary_to_pydantic_model(func, model_name)
-        dynamic_models.append(dyn_model)
-    return dynamic_models
-
-
-def map_grammar_names_to_pydantic_model_class(pydantic_model_list):
-    output = {}
-    for model in pydantic_model_list:
-        output[format_model_and_field_name(model.__name__)] = model
-
-    return output
-
-
-from enum import Enum
-
-
-def json_schema_to_python_types(schema):
-    type_map = {
-        "any": Any,
-        "string": str,
-        "number": float,
-        "integer": int,
-        "boolean": bool,
-        "array": list,
-    }
-    return type_map[schema]
-
-
-def list_to_enum(enum_name, values):
-    return Enum(enum_name, {value: value for value in values})
-
-
-def convert_dictionary_to_pydantic_model(
-    dictionary: dict[str, Any],
-    model_name: str = "CustomModel",
-    docs: dict[str, str] = None,
-    docs_function: dict[str, str] = None,
-) -> type[Any]:
-    """
-    Convert a dictionary to a Pydantic model class.
-
-    Args:
-        dictionary (dict): Dictionary representing the model structure.
-        model_name (str): Name of the generated Pydantic model.
-
-    Returns:
-        type[BaseModel]: Generated Pydantic model class.
-    """
-    fields: dict[str, Any] = {}
-    if docs is None:
-        docs = {}
-    if docs_function is None:
-        docs_function = {}
-    if "properties" in dictionary:
-        for field_name, field_data in dictionary.get("properties", {}).items():
-            if field_data == "object":
-                submodel = convert_dictionary_to_pydantic_model(
-                    dictionary, f"{model_name}_{field_name}", docs, docs_function
-                )
-                fields[field_name] = (submodel, ...)
-
-            else:
-                field_type = field_data.get("type", "string")
-                if field_data.get("description", None):
-                    docs[field_name] = field_data["description"]
-                if field_data.get("enum", []):
-                    fields[field_name] = (
-                        list_to_enum(field_name, field_data.get("enum", [])),
-                        ...,
-                    )
-                elif field_type == "array":
-                    items = field_data.get("items", {})
-                    if items != {}:
-                        array = {"properties": items}
-                        array_type = convert_dictionary_to_pydantic_model(
-                            array,
-                            f"{model_name}_{field_name}_items",
-                            docs,
-                            docs_function,
-                        )
-                        fields[field_name] = (List[array_type], ...)  # type: ignore[valid-type]
-                    else:
-                        fields[field_name] = (list, ...)
-                elif field_type == "object":
-                    submodel = convert_dictionary_to_pydantic_model(
-                        field_data, f"{model_name}_{field_name}", docs, docs_function
-                    )
-                    fields[field_name] = (submodel, ...)
-                elif field_type == "required":
-                    required = field_data
-                    for key, field in fields.items():
-                        if key not in required:
-                            fields[key] = (Optional[fields[key][0]], ...)
-                else:
-                    field_type = json_schema_to_python_types(field_type)
-                    fields[field_name] = (field_type, ...)
-    if "function" in dictionary:
-        for field_name, field_data in dictionary.get("function", {}).items():
-            if field_name == "name":
-                model_name = field_data
-            elif field_name == "description":
-                docs_function["__doc__"] = field_data
-            elif field_name == "parameters":
-                return convert_dictionary_to_pydantic_model(
-                    field_data, f"{model_name}", docs, docs_function
-                )
-
-    if "parameters" in dictionary:
-        field_data = {"function": dictionary}
-        return convert_dictionary_to_pydantic_model(
-            field_data, f"{model_name}", docs, docs_function
-        )
-    if "required" in dictionary:
-        required = dictionary.get("required", [])
-        for key, field in fields.items():
-            if key not in required:
-                fields[key] = (Optional[fields[key][0]], ...)
-    custom_model = create_model(model_name, **fields)
-
-    if "__doc__" in docs_function:
-        custom_model.__doc__ = docs_function["__doc__"]
-    for field_name, doc in docs.items():
-        custom_model.model_fields[field_name].description = doc
-
-    return custom_model
+from __future__ import annotations
+
+import inspect
+import json
+import re
+import typing
+from copy import copy
+from enum import Enum
+from inspect import getdoc, isclass
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    List,
+    Optional,
+    Union,
+    get_args,
+    get_origin,
+    get_type_hints,
+)
+
+from docstring_parser import parse
+from pydantic import BaseModel, Field, create_model
+
+from llama_cpp_agent.llm_documentation import (
+    generate_markdown_documentation,
+    generate_text_documentation,
+)
+
+if TYPE_CHECKING:
+    from types import GenericAlias
+    from types import UnionType
+else:
+    # python 3.8 compat
+    from typing import _GenericAlias as GenericAlias
+    from types import UnionType
+
+
+class PydanticDataType(Enum):
+    """
+    Defines the data types supported by the grammar_generator.
+
+    Attributes:
+        STRING (str): Represents a string data type.
+        BOOLEAN (str): Represents a boolean data type.
+        INTEGER (str): Represents an integer data type.
+        FLOAT (str): Represents a float data type.
+        OBJECT (str): Represents an object data type.
+        ARRAY (str): Represents an array data type.
+        ENUM (str): Represents an enum data type.
+        CUSTOM_CLASS (str): Represents a custom class data type.
+    """
+
+    STRING = "string"
+    TRIPLE_QUOTED_STRING = "triple_quoted_string"
+    MARKDOWN_CODE_BLOCK = "markdown_code_block"
+    BOOLEAN = "boolean"
+    INTEGER = "number"
+    FLOAT = "number"
+    OBJECT = "object"
+    ARRAY = "array"
+    ENUM = "enum"
+    ANY = "any"
+    NULL = "null"
+    CUSTOM_CLASS = "custom-class"
+    CUSTOM_DICT = "custom-dict"
+    SET = "set"
+
+
+def map_pydantic_type_to_gbnf(pydantic_type: type[Any]) -> str:
+    if isclass(pydantic_type) and issubclass(pydantic_type, str):
+        return PydanticDataType.STRING.value
+    elif isclass(pydantic_type) and issubclass(pydantic_type, bool):
+        return PydanticDataType.BOOLEAN.value
+    elif isclass(pydantic_type) and issubclass(pydantic_type, int):
+        return PydanticDataType.INTEGER.value
+    elif isclass(pydantic_type) and issubclass(pydantic_type, float):
+        return PydanticDataType.FLOAT.value
+    elif isclass(pydantic_type) and issubclass(pydantic_type, Enum):
+        return PydanticDataType.ENUM.value
+
+    elif isclass(pydantic_type) and issubclass(pydantic_type, BaseModel):
+        return format_model_and_field_name(pydantic_type.__name__)
+    elif get_origin(pydantic_type) is list:
+        element_type = get_args(pydantic_type)[0]
+        return f"{map_pydantic_type_to_gbnf(element_type)}-list"
+    elif get_origin(pydantic_type) is set:
+        element_type = get_args(pydantic_type)[0]
+        return f"{map_pydantic_type_to_gbnf(element_type)}-set"
+    elif get_origin(pydantic_type) is Union or isinstance(pydantic_type, UnionType):
+        union_types = get_args(pydantic_type)
+        union_rules = [map_pydantic_type_to_gbnf(ut) for ut in union_types]
+        return f"union-{'-or-'.join(union_rules)}"
+    elif get_origin(pydantic_type) is Optional:
+        element_type = get_args(pydantic_type)[0]
+        return f"optional-{map_pydantic_type_to_gbnf(element_type)}"
+    elif isclass(pydantic_type):
+        return f"{PydanticDataType.CUSTOM_CLASS.value}-{format_model_and_field_name(pydantic_type.__name__)}"
+    elif get_origin(pydantic_type) is dict:
+        key_type, value_type = get_args(pydantic_type)
+        return f"custom-dict-key-type-{format_model_and_field_name(map_pydantic_type_to_gbnf(key_type))}-value-type-{format_model_and_field_name(map_pydantic_type_to_gbnf(value_type))}"
+    else:
+        return "unknown"
+
+
+def format_model_and_field_name(model_name: str) -> str:
+    parts = re.findall("[A-Z][^A-Z]*", model_name)
+    if not parts:  # Check if the list is empty
+        return model_name.lower().replace("_", "-")
+    return "-".join(part.lower().replace("_", "-") for part in parts)
+
+
+def generate_list_rule(element_type):
+    """
+    Generate a GBNF rule for a list of a given element type.
+
+    :param element_type: The type of the elements in the list (e.g., 'string').
+    :return: A string representing the GBNF rule for a list of the given type.
+    """
+    rule_name = f"{map_pydantic_type_to_gbnf(element_type)}-list"
+    element_rule = map_pydantic_type_to_gbnf(element_type)
+    list_rule = rf'{rule_name} ::= "["  {element_rule} (","  {element_rule})* "]"'
+    return list_rule
+
+
+def get_members_structure(cls, rule_name):
+    if issubclass(cls, Enum):
+        # Handle Enum types
+        members = [
+            f'"\\"{member.value}\\""' for name, member in cls.__members__.items()
+        ]
+        return f"{cls.__name__.lower()} ::= " + " | ".join(members)
+    if cls.__annotations__ and cls.__annotations__ != {}:
+        result = f'{rule_name} ::= "{{"'
+        # Modify this comprehension
+        members = [
+            f'  "\\"{name}\\"" ":"  {map_pydantic_type_to_gbnf(param_type)}'
+            for name, param_type in cls.__annotations__.items()
+            if name != "self"
+        ]
+
+        result += '"," '.join(members)
+        result += '  "}"'
+        return result
+    if rule_name == "custom-class-any":
+        result = f"{rule_name} ::= "
+        result += "value"
+        return result
+
+    init_signature = inspect.signature(cls.__init__)
+    parameters = init_signature.parameters
+    result = f'{rule_name} ::=  "{{"'
+    # Modify this comprehension too
+    members = [
+        f'  "\\"{name}\\"" ":"  {map_pydantic_type_to_gbnf(param.annotation)}'
+        for name, param in parameters.items()
+        if name != "self" and param.annotation != inspect.Parameter.empty
+    ]
+
+    result += '", "'.join(members)
+    result += '  "}"'
+    return result
+
+
+def regex_to_gbnf(regex_pattern: str) -> str:
+    """
+    Translate a basic regex pattern to a GBNF rule.
+    Note: This function handles only a subset of simple regex patterns.
+    """
+    gbnf_rule = regex_pattern
+
+    # Translate common regex components to GBNF
+    gbnf_rule = gbnf_rule.replace("\\d", "[0-9]")
+    gbnf_rule = gbnf_rule.replace("\\s", "[ \t\n]")
+
+    # Handle quantifiers and other regex syntax that is similar in GBNF
+    # (e.g., '*', '+', '?', character classes)
+
+    return gbnf_rule
+
+
+def generate_gbnf_integer_rules(max_digit=None, min_digit=None):
+    """
+
+    Generate GBNF Integer Rules
+
+    Generates GBNF (Generalized Backus-Naur Form) rules for integers based on the given maximum and minimum digits.
+
+    Parameters:
+        max_digit (int): The maximum number of digits for the integer. Default is None.
+        min_digit (int): The minimum number of digits for the integer. Default is None.
+
+    Returns:
+        integer_rule (str): The identifier for the integer rule generated.
+        additional_rules (list): A list of additional rules generated based on the given maximum and minimum digits.
+
+    """
+    additional_rules = []
+
+    # Define the rule identifier based on max_digit and min_digit
+    integer_rule = "integer-part"
+    if max_digit is not None:
+        integer_rule += f"-max{max_digit}"
+    if min_digit is not None:
+        integer_rule += f"-min{min_digit}"
+
+    # Handling Integer Rules
+    if max_digit is not None or min_digit is not None:
+        # Start with an empty rule part
+        integer_rule_part = ""
+
+        # Add mandatory digits as per min_digit
+        if min_digit is not None:
+            integer_rule_part += "[0-9] " * min_digit
+
+        # Add optional digits up to max_digit
+        if max_digit is not None:
+            optional_digits = max_digit - (min_digit if min_digit is not None else 0)
+            integer_rule_part += "".join(["[0-9]? " for _ in range(optional_digits)])
+
+        # Trim the rule part and append it to additional rules
+        integer_rule_part = integer_rule_part.strip()
+        if integer_rule_part:
+            additional_rules.append(f"{integer_rule} ::= {integer_rule_part}")
+
+    return integer_rule, additional_rules
+
+
+def generate_gbnf_float_rules(
+    max_digit=None, min_digit=None, max_precision=None, min_precision=None
+):
+    """
+    Generate GBNF float rules based on the given constraints.
+
+    :param max_digit: Maximum number of digits in the integer part (default: None)
+    :param min_digit: Minimum number of digits in the integer part (default: None)
+    :param max_precision: Maximum number of digits in the fractional part (default: None)
+    :param min_precision: Minimum number of digits in the fractional part (default: None)
+    :return: A tuple containing the float rule and additional rules as a list
+
+    Example Usage:
+    max_digit = 3
+    min_digit = 1
+    max_precision = 2
+    min_precision = 1
+    generate_gbnf_float_rules(max_digit, min_digit, max_precision, min_precision)
+
+    Output:
+    ('float-3-1-2-1', ['integer-part-max3-min1 ::= [0-9] [0-9] [0-9]?', 'fractional-part-max2-min1 ::= [0-9] [0-9]?', 'float-3-1-2-1 ::= integer-part-max3-min1 "." fractional-part-max2-min
+    *1'])
+
+    Note:
+    GBNF stands for Generalized Backus-Naur Form, which is a notation technique to specify the syntax of programming languages or other formal grammars.
+    """
+    additional_rules = []
+
+    # Define the integer part rule
+    integer_part_rule = (
+        "integer-part"
+        + (f"-max{max_digit}" if max_digit is not None else "")
+        + (f"-min{min_digit}" if min_digit is not None else "")
+    )
+
+    # Define the fractional part rule based on precision constraints
+    fractional_part_rule = "fractional-part"
+    fractional_rule_part = ""
+    if max_precision is not None or min_precision is not None:
+        fractional_part_rule += (
+            f"-max{max_precision}" if max_precision is not None else ""
+        ) + (f"-min{min_precision}" if min_precision is not None else "")
+        # Minimum number of digits
+        fractional_rule_part = "[0-9]" * (
+            min_precision if min_precision is not None else 1
+        )
+        # Optional additional digits
+        fractional_rule_part += "".join(
+            [" [0-9]?"]
+            * (
+                (max_precision - (min_precision if min_precision is not None else 1))
+                if max_precision is not None
+                else 0
+            )
+        )
+        additional_rules.append(f"{fractional_part_rule} ::= {fractional_rule_part}")
+
+    # Define the float rule
+    float_rule = f"float-{max_digit if max_digit is not None else 'X'}-{min_digit if min_digit is not None else 'X'}-{max_precision if max_precision is not None else 'X'}-{min_precision if min_precision is not None else 'X'}"
+    additional_rules.append(
+        f'{float_rule} ::= {integer_part_rule} "." {fractional_part_rule}'
+    )
+
+    # Generating the integer part rule definition, if necessary
+    if max_digit is not None or min_digit is not None:
+        integer_rule_part = "[0-9]"
+        if min_digit is not None and min_digit > 1:
+            integer_rule_part += " [0-9]" * (min_digit - 1)
+        if max_digit is not None:
+            integer_rule_part += "".join(
+                [" [0-9]?"] * (max_digit - (min_digit if min_digit is not None else 1))
+            )
+        additional_rules.append(f"{integer_part_rule} ::= {integer_rule_part.strip()}")
+
+    return float_rule, additional_rules
+
+
+def generate_gbnf_rule_for_type(
+    model_name,
+    field_name,
+    field_type,
+    is_optional,
+    processed_models,
+    created_rules,
+    field_info=None,
+) -> tuple[str, list[str]]:
+    """
+    Generate GBNF rule for a given field type.
+
+    :param model_name: Name of the model.
+
+    :param field_name: Name of the field.
+    :param field_type: Type of the field.
+    :param is_optional: Whether the field is optional.
+    :param processed_models: List of processed models.
+    :param created_rules: List of created rules.
+    :param field_info: Additional information about the field (optional).
+
+    :return: Tuple containing the GBNF type and a list of additional rules.
+    :rtype: tuple[str, list]
+    """
+    rules = []
+
+    field_name = format_model_and_field_name(field_name)
+    gbnf_type = map_pydantic_type_to_gbnf(field_type)
+
+    if isclass(field_type) and issubclass(field_type, BaseModel):
+        nested_model_name = format_model_and_field_name(field_type.__name__)
+        nested_model_rules, _ = generate_gbnf_grammar(
+            field_type, processed_models, created_rules
+        )
+        rules.extend(nested_model_rules)
+        gbnf_type, rules = nested_model_name, rules
+    elif isclass(field_type) and issubclass(field_type, Enum):
+        enum_values = [
+            f'"\\"{e.value}\\""' for e in field_type
+        ]  # Adding escaped quotes
+        enum_rule = f"{model_name}-{field_name} ::= {' | '.join(enum_values)}"
+        rules.append(enum_rule)
+        gbnf_type, rules = model_name + "-" + field_name, rules
+    elif get_origin(field_type) == list:  # Array
+        element_type = get_args(field_type)[0]
+        element_rule_name, additional_rules = generate_gbnf_rule_for_type(
+            model_name,
+            f"{field_name}-element",
+            element_type,
+            is_optional,
+            processed_models,
+            created_rules,
+        )
+        rules.extend(additional_rules)
+        array_rule = rf"""{model_name}-{field_name} ::= "[" ws ({element_rule_name})? ("," ws {element_rule_name})* ws "]" """
+        rules.append(array_rule)
+        gbnf_type, rules = model_name + "-" + field_name, rules
+
+    elif get_origin(field_type) == set or field_type == set:  # Array
+        element_type = get_args(field_type)[0]
+        element_rule_name, additional_rules = generate_gbnf_rule_for_type(
+            model_name,
+            f"{field_name}-element",
+            element_type,
+            is_optional,
+            processed_models,
+            created_rules,
+        )
+        rules.extend(additional_rules)
+        array_rule = rf"""{model_name}-{field_name} ::= "[" ws ({element_rule_name})? ("," ws {element_rule_name})* ws "]" """
+        rules.append(array_rule)
+        gbnf_type, rules = model_name + "-" + field_name, rules
+
+    elif gbnf_type.startswith("custom-class-"):
+        rules.append(get_members_structure(field_type, gbnf_type))
+    elif gbnf_type.startswith("custom-dict-"):
+        key_type, value_type = get_args(field_type)
+
+        additional_key_type, additional_key_rules = generate_gbnf_rule_for_type(
+            model_name,
+            f"{field_name}-key-type",
+            key_type,
+            is_optional,
+            processed_models,
+            created_rules,
+        )
+        additional_value_type, additional_value_rules = generate_gbnf_rule_for_type(
+            model_name,
+            f"{field_name}-value-type",
+            value_type,
+            is_optional,
+            processed_models,
+            created_rules,
+        )
+        rules.extend(
+            [
+                rf'{gbnf_type} ::= "{{"  ( {additional_key_type} ": "  {additional_value_type} ("," "\n" ws {additional_key_type} ":"  {additional_value_type})*  )? "}}" '
+            ]
+        )
+        rules.extend(additional_key_rules)
+        rules.extend(additional_value_rules)
+    elif gbnf_type.startswith("union-"):
+        union_types = get_args(field_type)
+        union_rules = []
+
+        for union_type in union_types:
+            if isinstance(union_type, GenericAlias):
+                union_gbnf_type, union_rules_list = generate_gbnf_rule_for_type(
+                    model_name,
+                    field_name,
+                    union_type,
+                    False,
+                    processed_models,
+                    created_rules,
+                )
+                union_rules.append(union_gbnf_type)
+                rules.extend(union_rules_list)
+
+            elif not issubclass(union_type, type(None)):
+                union_gbnf_type, union_rules_list = generate_gbnf_rule_for_type(
+                    model_name,
+                    field_name,
+                    union_type,
+                    False,
+                    processed_models,
+                    created_rules,
+                )
+                union_rules.append(union_gbnf_type)
+                rules.extend(union_rules_list)
+
+        # Defining the union grammar rule separately
+        if len(union_rules) == 1:
+            union_grammar_rule = f"{model_name}-{field_name}-optional ::= {' | '.join(union_rules)} | null"
+        else:
+            uni = []
+            for rule in union_rules:
+                if rule not in uni:
+                    uni.append(rule)
+            union_grammar_rule = (
+                f"{model_name}-{field_name}-union ::= {' | '.join(uni)}"
+            )
+        rules.append(union_grammar_rule)
+        if len(union_rules) == 1:
+            gbnf_type = f"{model_name}-{field_name}-optional"
+        else:
+            gbnf_type = f"{model_name}-{field_name}-union"
+    elif isclass(field_type) and issubclass(field_type, str):
+        if (
+            field_info
+            and hasattr(field_info, "json_schema_extra")
+            and field_info.json_schema_extra is not None
+        ):
+            triple_quoted_string = field_info.json_schema_extra.get(
+                "triple_quoted_string", False
+            )
+            markdown_string = field_info.json_schema_extra.get(
+                "markdown_code_block", False
+            )
+
+            gbnf_type = (
+                PydanticDataType.TRIPLE_QUOTED_STRING.value
+                if triple_quoted_string
+                else PydanticDataType.STRING.value
+            )
+            gbnf_type = (
+                PydanticDataType.MARKDOWN_CODE_BLOCK.value
+                if markdown_string
+                else gbnf_type
+            )
+
+        elif field_info and hasattr(field_info, "pattern"):
+            # Convert regex pattern to grammar rule
+            regex_pattern = field_info.regex.pattern
+            gbnf_type = f"pattern-{field_name} ::= {regex_to_gbnf(regex_pattern)}"
+        else:
+            gbnf_type = PydanticDataType.STRING.value
+
+    elif (
+        isclass(field_type)
+        and issubclass(field_type, float)
+        and field_info
+        and hasattr(field_info, "json_schema_extra")
+        and field_info.json_schema_extra is not None
+    ):
+        # Retrieve precision attributes for floats
+        max_precision = (
+            field_info.json_schema_extra.get("max_precision")
+            if field_info and hasattr(field_info, "json_schema_extra")
+            else None
+        )
+        min_precision = (
+            field_info.json_schema_extra.get("min_precision")
+            if field_info and hasattr(field_info, "json_schema_extra")
+            else None
+        )
+        max_digits = (
+            field_info.json_schema_extra.get("max_digit")
+            if field_info and hasattr(field_info, "json_schema_extra")
+            else None
+        )
+        min_digits = (
+            field_info.json_schema_extra.get("min_digit")
+            if field_info and hasattr(field_info, "json_schema_extra")
+            else None
+        )
+
+        # Generate GBNF rule for float with given attributes
+        gbnf_type, rules = generate_gbnf_float_rules(
+            max_digit=max_digits,
+            min_digit=min_digits,
+            max_precision=max_precision,
+            min_precision=min_precision,
+        )
+
+    elif (
+        isclass(field_type)
+        and issubclass(field_type, int)
+        and field_info
+        and hasattr(field_info, "json_schema_extra")
+        and field_info.json_schema_extra is not None
+    ):
+        # Retrieve digit attributes for integers
+        max_digits = (
+            field_info.json_schema_extra.get("max_digit")
+            if field_info and hasattr(field_info, "json_schema_extra")
+            else None
+        )
+        min_digits = (
+            field_info.json_schema_extra.get("min_digit")
+            if field_info and hasattr(field_info, "json_schema_extra")
+            else None
+        )
+
+        # Generate GBNF rule for integer with given attributes
+        gbnf_type, rules = generate_gbnf_integer_rules(
+            max_digit=max_digits, min_digit=min_digits
+        )
+    else:
+        gbnf_type, rules = gbnf_type, []
+
+    return gbnf_type, rules
+
+
+def generate_gbnf_grammar(
+    model: type[BaseModel],
+    processed_models: set[type[BaseModel]],
+    created_rules: dict[str, list[str]],
+) -> tuple[list[str], bool]:
+    """
+
+    Generate GBnF Grammar
+
+    Generates a GBnF grammar for a given model.
+
+    :param model: A Pydantic model class to generate the grammar for. Must be a subclass of BaseModel.
+    :param processed_models: A set of already processed models to prevent infinite recursion.
+    :param created_rules: A dict containing already created rules to prevent duplicates.
+    :return: A list of GBnF grammar rules in string format. And two booleans indicating if an extra markdown or triple quoted string is in the grammar.
+    Example Usage:
+    ```
+    model = MyModel
+    processed_models = set()
+    created_rules = dict()
+
+    gbnf_grammar = generate_gbnf_grammar(model, processed_models, created_rules)
+    ```
+    """
+    if model in processed_models:
+        return [], False
+
+    processed_models.add(model)
+    model_name = format_model_and_field_name(model.__name__)
+
+    if not issubclass(model, BaseModel):
+        # For non-Pydantic classes, generate model_fields from __annotations__ or __init__
+        if hasattr(model, "__annotations__") and model.__annotations__:
+            model_fields = {
+                name: (typ, ...) for name, typ in model.__annotations__.items()
+            }
+        else:
+            init_signature = inspect.signature(model.__init__)
+            parameters = init_signature.parameters
+            model_fields = {
+                name: (param.annotation, param.default)
+                for name, param in parameters.items()
+                if name != "self"
+            }
+    else:
+        # For Pydantic models, use model_fields and check for ellipsis (required fields)
+        model_fields = model.__annotations__
+
+    model_rule_parts = []
+    nested_rules = []
+    has_markdown_code_block = False
+    has_triple_quoted_string = False
+    look_for_markdown_code_block = False
+    look_for_triple_quoted_string = False
+    for field_name, field_info in model_fields.items():
+        if not issubclass(model, BaseModel):
+            field_type, default_value = field_info
+            # Check if the field is optional (not required)
+            is_optional = (default_value is not inspect.Parameter.empty) and (
+                default_value is not Ellipsis
+            )
+        else:
+            field_type = field_info
+            field_info = model.model_fields[field_name]
+            is_optional = (
+                field_info.is_required is False and get_origin(field_type) is Optional
+            )
+        rule_name, additional_rules = generate_gbnf_rule_for_type(
+            model_name,
+            format_model_and_field_name(field_name),
+            field_type,
+            is_optional,
+            processed_models,
+            created_rules,
+            field_info,
+        )
+        look_for_markdown_code_block = (
+            True if rule_name == "markdown_code_block" else False
+        )
+        look_for_triple_quoted_string = (
+            True if rule_name == "triple_quoted_string" else False
+        )
+        if not look_for_markdown_code_block and not look_for_triple_quoted_string:
+            if rule_name not in created_rules:
+                created_rules[rule_name] = additional_rules
+            model_rule_parts.append(
+                f' ws "\\"{field_name}\\"" ": " {rule_name}'
+            )  # Adding escaped quotes
+            nested_rules.extend(additional_rules)
+        else:
+            has_triple_quoted_string = look_for_triple_quoted_string
+            has_markdown_code_block = look_for_markdown_code_block
+
+    fields_joined = r' "," '.join(model_rule_parts)
+    if fields_joined != "":
+        model_rule = rf'{model_name} ::= "{{" {fields_joined} ws "}}"'
+    else:
+        model_rule = rf'{model_name} ::= "{{" "}}"'
+
+    has_special_string = False
+    if has_triple_quoted_string:
+        model_rule += '"\\n" ws "}"'
+        model_rule += '"\\n" triple-quoted-string'
+        has_special_string = True
+    if has_markdown_code_block:
+        model_rule += '"\\n" ws "}"'
+        model_rule += '"\\n" markdown-code-block'
+        has_special_string = True
+    all_rules = [model_rule] + nested_rules
+
+    return all_rules, has_special_string
+
+
+def generate_gbnf_grammar_from_pydantic_models(
+    models: list[BaseModel],
+    outer_object_name: str | None = None,
+    outer_object_content: str | None = None,
+    list_of_outputs: bool = False,
+    add_inner_thoughts: bool = True,
+    allow_only_inner_thoughts: bool = True,
+    inner_thought_field_name: str = "chain_of_thought",
+    add_request_heartbeat: bool = True,
+    request_heartbeat_field_name: str = "request_heartbeat",
+    request_heartbeat_models: list[str] = None,
+) -> str:
+    """
+    Generate GBNF Grammar from Pydantic Models.
+
+    This method takes a list of Pydantic models and uses them to generate a GBNF grammar string. The generated grammar string can be used for parsing and validating data using the generated
+    * grammar.
+
+    Args:
+        models (list[type[BaseModel]]): A list of Pydantic models to generate the grammar from.
+        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
+        outer_object_content (str): Content for the outer rule in the GBNF grammar. Eg. "function_parameters" or "params" for function calling.
+        list_of_outputs (str, optional): Allows a list of output objects
+        add_inner_thoughts (bool, optional): Add inner thoughts to the grammar. Defaults to True.
+        allow_only_inner_thoughts (bool, optional): Allow only inner thoughts. Defaults to True.
+    Returns:
+        str: The generated GBNF grammar string.
+
+    Examples:
+        models = [UserModel, PostModel]
+        grammar = generate_gbnf_grammar_from_pydantic(models)
+        print(grammar)
+        # Output:
+        # root ::= UserModel | PostModel
+        # ...
+    """
+    if request_heartbeat_models is None:
+        request_heartbeat_models = []
+    processed_models: set[type[BaseModel]] = set()
+    all_rules = []
+    created_rules: dict[str, list[str]] = {}
+    if outer_object_name is None:
+        for model in models:
+            model_rules, _ = generate_gbnf_grammar(
+                model, processed_models, created_rules
+            )
+            all_rules.extend(model_rules)
+
+        if list_of_outputs:
+            root_rule = (
+                r'root ::= (" "| "\n") "[" ws grammar-models ("," ws grammar-models)* "\n" "]"'
+                + "\n"
+            )
+        else:
+            root_rule = r'root ::= (" "| "\n") grammar-models' + "\n"
+        root_rule += "grammar-models ::= " + " | ".join(
+            [format_model_and_field_name(model.__name__) for model in models]
+        )
+        all_rules.insert(0, root_rule)
+        return "\n".join(all_rules) + get_primitive_grammar("\n".join(all_rules))
+    elif outer_object_name is not None:
+        if list_of_outputs:
+            root_rule = (
+                rf'root ::= (" "| "\n") "[" ws {format_model_and_field_name(outer_object_name)} ("," ws {format_model_and_field_name(outer_object_name)})* "\n" "]"'
+                + "\n"
+            )
+        else:
+            root_rule = f"root ::= {format_model_and_field_name(outer_object_name)}\n"
+
+        if add_inner_thoughts:
+            if allow_only_inner_thoughts:
+                model_rule = rf'{format_model_and_field_name(outer_object_name)} ::= (" "| "\n") "{{" ws "\"{inner_thought_field_name}\""  ":" ws string (("," ws "\"{outer_object_name}\""  ":" ws grammar-models)? | ws "}}")'
+            else:
+                model_rule = rf'{format_model_and_field_name(outer_object_name)} ::= (" "| "\n") "{{" ws "\"{inner_thought_field_name}\""  ":" ws string "," ws "\"{outer_object_name}\""  ":" ws grammar-models '
+        else:
+            model_rule = rf'{format_model_and_field_name(outer_object_name)} ::= (" "| "\n") "{{" ws "\"{outer_object_name}\""  ": " ws grammar-models'
+
+        fields_joined = " | ".join(
+            [
+                rf"{format_model_and_field_name(model.__name__)}-grammar-model"
+                for model in models
+            ]
+        )
+
+        grammar_model_rules = f"\ngrammar-models ::= {fields_joined}"
+        mod_rules = []
+        for model in models:
+            mod_rule = (
+                rf"{format_model_and_field_name(model.__name__)}-grammar-model ::= "
+            )
+            mod_rule += (
+                rf'"\"{model.__name__}\"" "," ws "\"{outer_object_content}\"" ": " {format_model_and_field_name(model.__name__)}'
+                + "\n"
+            )
+            mod_rules.append(mod_rule)
+        grammar_model_rules += "\n" + "\n".join(mod_rules)
+
+        for model in models:
+            model_rules, has_special_string = generate_gbnf_grammar(
+                model, processed_models, created_rules
+            )
+            if add_request_heartbeat and model.__name__ in request_heartbeat_models:
+                model_rules[
+                    0
+                ] += rf' "," ws "\"{request_heartbeat_field_name}\""  ":" ws boolean '
+            if not has_special_string:
+                model_rules[0] += r' ws "}"'
+
+            all_rules.extend(model_rules)
+
+        all_rules.insert(0, root_rule + model_rule + grammar_model_rules)
+        return "\n".join(all_rules) + get_primitive_grammar("\n".join(all_rules))
+
+
+def get_primitive_grammar(grammar):
+    """
+    Returns the needed GBNF primitive grammar for a given GBNF grammar string.
+
+    Args:
+        grammar (str): The string containing the GBNF grammar.
+
+    Returns:
+        str: GBNF primitive grammar string.
+    """
+    type_list: list[type[object]] = []
+    if "string-list" in grammar:
+        type_list.append(str)
+    if "boolean-list" in grammar:
+        type_list.append(bool)
+    if "integer-list" in grammar:
+        type_list.append(int)
+    if "float-list" in grammar:
+        type_list.append(float)
+    additional_grammar = [generate_list_rule(t) for t in type_list]
+    primitive_grammar = r"""
+boolean ::= "true" | "false"
+null ::= "null"
+string ::= "\"" (
+        [^"\\] |
+        "\\" (["\\/bfnrt] | "u" [0-9a-fA-F] [0-9a-fA-F] [0-9a-fA-F] [0-9a-fA-F])
+      )* "\""
+ws ::= ([ \t\n]+)
+number ::= "-"? ([0-9]+ | [0-9]+ "." [0-9]+) ([eE] [-+]? [0-9]+)?"""
+
+    any_block = ""
+    if "custom-class-any" in grammar:
+        any_block = """
+value ::= object | array | string | number | boolean | null
+
+object ::=
+  "{" ws (
+            string ":" ws value
+    ("," ws string ":" ws value)*
+  )? "}"
+
+array  ::=
+  "[" ws (
+            value
+    ("," ws value)*
+  )? "]"
+"""
+
+    markdown_code_block_grammar = ""
+    if "markdown-code-block" in grammar:
+        markdown_code_block_grammar = r'''
+markdown-code-block ::= opening-triple-ticks markdown-code-block-content closing-triple-ticks
+markdown-code-block-content ::= ( [^`] | "`" [^`] |  "`"  "`" [^`]  )*
+opening-triple-ticks ::= "```" "python" "\n" | "```" "c" "\n" | "```" "cpp" "\n" | "```" "txt" "\n" | "```" "text" "\n" | "```" "json" "\n" | "```" "javascript" "\n" | "```" "css" "\n" | "```" "html" "\n" | "```" "markdown" "\n"
+closing-triple-ticks ::= "```" "\n"'''
+
+    if "triple-quoted-string" in grammar:
+        markdown_code_block_grammar = r"""
+triple-quoted-string ::= triple-quotes triple-quoted-string-content triple-quotes
+triple-quoted-string-content ::= ( [^'] | "'" [^'] |  "'"  "'" [^']  )*
+triple-quotes ::= "'''" """
+    return (
+        "\n"
+        + "\n".join(additional_grammar)
+        + any_block
+        + primitive_grammar
+        + markdown_code_block_grammar
+    )
+
+
+def save_gbnf_grammar_and_documentation(
+    grammar,
+    documentation,
+    grammar_file_path="./grammar.gbnf",
+    documentation_file_path="./grammar_documentation.md",
+):
+    """
+    Save GBNF grammar and documentation to specified files.
+
+    Args:
+        grammar (str): GBNF grammar string.
+        documentation (str): Documentation string.
+        grammar_file_path (str): File path to save the GBNF grammar.
+        documentation_file_path (str): File path to save the documentation.
+
+    Returns:
+        None
+    """
+    try:
+        with open(grammar_file_path, "w") as file:
+            file.write(grammar + get_primitive_grammar(grammar))
+        print(f"Grammar successfully saved to {grammar_file_path}")
+    except IOError as e:
+        print(f"An error occurred while saving the grammar file: {e}")
+
+    try:
+        with open(documentation_file_path, "w") as file:
+            file.write(documentation)
+        print(f"Documentation successfully saved to {documentation_file_path}")
+    except IOError as e:
+        print(f"An error occurred while saving the documentation file: {e}")
+
+
+def remove_empty_lines(string):
+    """
+    Remove empty lines from a string.
+
+    Args:
+        string (str): Input string.
+
+    Returns:
+        str: String with empty lines removed.
+    """
+    lines = string.splitlines()
+    non_empty_lines = [line for line in lines if line.strip() != ""]
+    string_no_empty_lines = "\n".join(non_empty_lines)
+    return string_no_empty_lines
+
+
+def generate_and_save_gbnf_grammar_and_documentation(
+    pydantic_model_list,
+    grammar_file_path="./generated_grammar.gbnf",
+    documentation_file_path="./generated_grammar_documentation.md",
+    outer_object_name: str | None = None,
+    outer_object_content: str | None = None,
+    model_prefix: str = "Output Model",
+    fields_prefix: str = "Output Fields",
+    list_of_outputs: bool = False,
+    documentation_with_field_description=True,
+    add_inner_thoughts: bool = False,
+    allow_only_inner_thoughts: bool = False,
+    inner_thoughts_field_name: str = "thoughts_and_reasoning",
+    add_request_heartbeat: bool = False,
+    request_heartbeat_field_name: str = "request_heartbeat",
+    request_heartbeat_models: List[str] = None,
+):
+    """
+    Generate GBNF grammar and documentation, and save them to specified files.
+
+    Args:
+        pydantic_model_list: List of Pydantic model classes.
+        grammar_file_path (str): File path to save the generated GBNF grammar.
+        documentation_file_path (str): File path to save the generated documentation.
+        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
+        outer_object_content (str): Content for the outer rule in the GBNF grammar. Eg. "function_parameters" or "params" for function calling.
+        model_prefix (str): Prefix for the model section in the documentation.
+        fields_prefix (str): Prefix for the fields section in the documentation.
+        list_of_outputs (bool): Whether the output is a list of items.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+        add_inner_thoughts (bool): Add inner thoughts to the grammar. This is useful for adding comments or reasoning to the output.
+        allow_only_inner_thoughts (bool): Allow only inner thoughts. If True, only inner thoughts will be allowed in the output.
+        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "thoughts_and_reasoning".
+        add_request_heartbeat (bool): Add request heartbeat to the grammar. This allows the LLM to decide when to return control to the system.
+        request_heartbeat_field_name (str): Field name for request heartbeat. Default is "request_heartbeat".
+        request_heartbeat_models (List[str]): List of models that will have a request heartbeat field.
+    Returns:
+        None
+    """
+    documentation = generate_markdown_documentation(
+        pydantic_model_list,
+        model_prefix,
+        fields_prefix,
+        documentation_with_field_description=documentation_with_field_description,
+    )
+    grammar = generate_gbnf_grammar_from_pydantic_models(
+        pydantic_model_list,
+        outer_object_name,
+        outer_object_content,
+        list_of_outputs,
+        add_inner_thoughts,
+        allow_only_inner_thoughts,
+        inner_thoughts_field_name,
+        add_request_heartbeat,
+        request_heartbeat_field_name,
+        request_heartbeat_models,
+    )
+    grammar = remove_empty_lines(grammar)
+    save_gbnf_grammar_and_documentation(
+        grammar, documentation, grammar_file_path, documentation_file_path
+    )
+
+
+def generate_gbnf_grammar_and_documentation(
+    pydantic_model_list,
+    outer_object_name: str | None = None,
+    outer_object_content: str | None = None,
+    model_prefix: str = "Output Model",
+    fields_prefix: str = "Output Fields",
+    list_of_outputs: bool = False,
+    documentation_with_field_description=True,
+    add_inner_thoughts: bool = False,
+    allow_only_inner_thoughts: bool = False,
+    inner_thoughts_field_name: str = "thoughts_and_reasoning",
+    add_request_heartbeat: bool = False,
+    request_heartbeat_field_name: str = "request_heartbeat",
+    request_heartbeat_models: List[str] = None,
+):
+    """
+    Generate GBNF grammar and documentation for a list of Pydantic models.
+
+    Args:
+        pydantic_model_list: List of Pydantic model classes.
+        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
+        outer_object_content (str): Content for the outer rule in the GBNF grammar. E.g., "function_parameters" or "params" for function calling.
+        model_prefix (str): Prefix for the model section in the documentation.
+        fields_prefix (str): Prefix for the fields section in the documentation.
+        list_of_outputs (bool): Whether the output is a list of items.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+        add_inner_thoughts (bool): Add inner thoughts to the grammar. This is useful for adding comments or reasoning to the output.
+        allow_only_inner_thoughts (bool): Allow only inner thoughts. If True, only inner thoughts will be allowed in the output.
+        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "thoughts_and_reasoning".
+        add_request_heartbeat (bool): Add request heartbeat to the grammar. This allows the LLM to decide when to return control to the system.
+        request_heartbeat_field_name (str): Field name for request heartbeat. Default is "request_heartbeat".
+        request_heartbeat_models (List[str]): List of models that will have a request heartbeat field.
+
+    Returns:
+        tuple: GBNF grammar string, documentation string.
+    """
+    documentation = generate_text_documentation(
+        copy(pydantic_model_list),
+        model_prefix,
+        fields_prefix,
+        documentation_with_field_description=documentation_with_field_description,
+    )
+    grammar = generate_gbnf_grammar_from_pydantic_models(
+        pydantic_model_list,
+        outer_object_name,
+        outer_object_content,
+        list_of_outputs,
+        add_inner_thoughts,
+        allow_only_inner_thoughts,
+        inner_thoughts_field_name,
+        add_request_heartbeat,
+        request_heartbeat_field_name,
+        request_heartbeat_models,
+    )
+    grammar = remove_empty_lines(grammar + get_primitive_grammar(grammar))
+    return grammar, documentation
+
+
+def generate_gbnf_grammar_and_documentation_from_dictionaries(
+    dictionaries: list[dict[str, Any]],
+    outer_object_name: str | None = None,
+    outer_object_content: str | None = None,
+    model_prefix: str = "Output Model",
+    fields_prefix: str = "Output Fields",
+    list_of_outputs: bool = False,
+    documentation_with_field_description=True,
+    add_inner_thoughts: bool = False,
+    allow_only_inner_thoughts: bool = False,
+    inner_thoughts_field_name: str = "thoughts_and_reasoning",
+    add_request_heartbeat: bool = False,
+    request_heartbeat_field_name: str = "request_heartbeat",
+    request_heartbeat_models: List[str] = None,
+):
+    """
+    Generate GBNF grammar and documentation from a list of dictionaries.
+
+    Args:
+        dictionaries (list[dict]): List of dictionaries representing Pydantic models.
+        outer_object_name (str): Outer object name for the GBNF grammar. If None, no outer object will be generated. Eg. "function" for function calling.
+        outer_object_content (str): Content for the outer rule in the GBNF grammar. Eg. "function_parameters" or "params" for function calling.
+        model_prefix (str): Prefix for the model section in the documentation.
+        fields_prefix (str): Prefix for the fields section in the documentation.
+        list_of_outputs (bool): Whether the output is a list of items.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+        add_inner_thoughts (bool): Add inner thoughts to the grammar. This is useful for adding comments or reasoning to the output.
+        allow_only_inner_thoughts (bool): Allow only inner thoughts. If True, only inner thoughts will be allowed in the output.
+        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "thoughts_and_reasoning".
+        add_request_heartbeat (bool): Add request heartbeat to the grammar. This allows the LLM to decide when to return control to the system.
+        request_heartbeat_field_name (str): Field name for request heartbeat. Default is "request_heartbeat".
+        request_heartbeat_models (List[str]): List of models that will have a request heartbeat field.
+
+    Returns:
+        tuple: GBNF grammar string, documentation string.
+    """
+    pydantic_model_list = create_dynamic_models_from_dictionaries(dictionaries)
+    documentation = generate_markdown_documentation(
+        copy(pydantic_model_list),
+        model_prefix,
+        fields_prefix,
+        documentation_with_field_description=documentation_with_field_description,
+    )
+    grammar = generate_gbnf_grammar_from_pydantic_models(
+        pydantic_model_list,
+        outer_object_name,
+        outer_object_content,
+        list_of_outputs,
+        add_inner_thoughts,
+        allow_only_inner_thoughts,
+        inner_thoughts_field_name,
+        add_request_heartbeat,
+        request_heartbeat_field_name,
+        request_heartbeat_models,
+    )
+    grammar = remove_empty_lines(grammar + get_primitive_grammar(grammar))
+    return grammar, documentation
+
+
+def create_dynamic_model_from_function(
+    func: Callable[..., Any],
+    add_inner_thoughts: bool = False,
+    inner_thoughts_field_name: str = "inner_thoughts",
+):
+    """
+    Creates a dynamic Pydantic model from a given function's type hints and adds the function as a 'run' method.
+
+    Args:
+        func (Callable): A function with type hints from which to create the model.
+        add_inner_thoughts (bool): Add an 'inner_thoughts' field at the params level to the model. Default is False.
+        inner_thoughts_field_name (str): Field name for inner thoughts. Default is "inner_thoughts".
+
+    Returns:
+        A dynamic Pydantic model class with the provided function as a 'run' method.
+    """
+
+    # Get the signature of the function
+    sig = inspect.signature(func)
+
+    # Parse the docstring
+    assert func.__doc__ is not None
+    docstring = parse(func.__doc__)
+
+    dynamic_fields = {}
+    param_docs = []
+    if add_inner_thoughts:
+        dynamic_fields[inner_thoughts_field_name] = (str, None)
+    for param in sig.parameters.values():
+        # Exclude 'self' parameter
+        if param.name == "self":
+            continue
+
+        # Assert that the parameter has a type annotation
+        if param.annotation == inspect.Parameter.empty:
+            raise TypeError(
+                f"Parameter '{param.name}' in function '{func.__name__}' lacks a type annotation"
+            )
+
+        # Find the parameter's description in the docstring
+        param_doc = next(
+            (d for d in docstring.params if d.arg_name == param.name), None
+        )
+
+        # Assert that the parameter has a description
+        if not param_doc or not param_doc.description:
+            raise ValueError(
+                f"Parameter '{param.name}' in function '{func.__name__}' lacks a description in the docstring"
+            )
+
+        # Add parameter details to the schema
+        param_docs.append((param.name, param_doc))
+        if param.default == inspect.Parameter.empty:
+            default_value = ...
+        else:
+            default_value = param.default
+        dynamic_fields[param.name] = (
+            param.annotation if param.annotation != inspect.Parameter.empty else str,
+            default_value,
+        )
+
+    # Creating the dynamic model
+    dynamic_model = create_model(f"{func.__name__}", **dynamic_fields)  # type: ignore[call-overload]
+    if add_inner_thoughts:
+        dynamic_model.model_fields[
+            inner_thoughts_field_name
+        ].description = "Deep inner monologue private to you only."
+    for name, param_doc in param_docs:
+        dynamic_model.model_fields[name].description = param_doc.description
+
+    dynamic_model.__doc__ = (
+        (docstring.short_description if docstring.short_description is not None else "")
+        + "\n"
+        + (docstring.long_description if docstring.long_description is not None else "")
+    )
+
+    def run_method_wrapper(self):
+        func_args = {name: getattr(self, name) for name, _ in dynamic_fields.items()}
+        return func(**func_args)
+
+    # Adding the wrapped function as a 'run' method
+    setattr(dynamic_model, "run", run_method_wrapper)
+    return dynamic_model
+
+
+def add_run_method_to_dynamic_model(model: type[BaseModel], func: Callable[..., Any]):
+    """
+    Add a 'run' method to a dynamic Pydantic model, using the provided function.
+
+    Args:
+        model (type[BaseModel]): Dynamic Pydantic model class.
+        func (Callable): Function to be added as a 'run' method to the model.
+
+    Returns:
+        type[BaseModel]: Pydantic model class with the added 'run' method.
+    """
+
+    def run_method_wrapper(self):
+        func_args = {name: getattr(self, name) for name in model.model_fields}
+        return func(**func_args)
+
+    # Adding the wrapped function as a 'run' method
+    setattr(model, "run", run_method_wrapper)
+
+    return model
+
+
+def create_dynamic_models_from_dictionaries(dictionaries: list[dict[str, Any]]):
+    """
+    Create a list of dynamic Pydantic model classes from a list of dictionaries.
+
+    Args:
+        dictionaries (list[dict]): List of dictionaries representing model structures.
+
+    Returns:
+        list[Type[BaseModel]]: List of generated dynamic Pydantic model classes.
+    """
+    dynamic_models = []
+    for func in dictionaries:
+        model_name = format_model_and_field_name(func.get("name", ""))
+        dyn_model = convert_dictionary_to_pydantic_model(func, model_name)
+        dynamic_models.append(dyn_model)
+    return dynamic_models
+
+
+def map_grammar_names_to_pydantic_model_class(pydantic_model_list):
+    output = {}
+    for model in pydantic_model_list:
+        output[format_model_and_field_name(model.__name__)] = model
+
+    return output
+
+
+from enum import Enum
+
+
+def json_schema_to_python_types(schema):
+    type_map = {
+        "any": Any,
+        "string": str,
+        "number": float,
+        "integer": int,
+        "boolean": bool,
+        "array": list,
+    }
+    return type_map[schema]
+
+
+def list_to_enum(enum_name, values):
+    return Enum(enum_name, {value: value for value in values})
+
+
+def convert_dictionary_to_pydantic_model(
+    dictionary: dict[str, Any],
+    model_name: str = "CustomModel",
+    docs: dict[str, str] = None,
+    docs_function: dict[str, str] = None,
+) -> type[Any]:
+    """
+    Convert a dictionary to a Pydantic model class.
+
+    Args:
+        dictionary (dict): Dictionary representing the model structure.
+        model_name (str): Name of the generated Pydantic model.
+
+    Returns:
+        type[BaseModel]: Generated Pydantic model class.
+    """
+    fields: dict[str, Any] = {}
+    if docs is None:
+        docs = {}
+    if docs_function is None:
+        docs_function = {}
+    if "properties" in dictionary:
+        for field_name, field_data in dictionary.get("properties", {}).items():
+            if field_data == "object":
+                submodel = convert_dictionary_to_pydantic_model(
+                    dictionary, f"{model_name}_{field_name}", docs, docs_function
+                )
+                fields[field_name] = (submodel, ...)
+
+            else:
+                field_type = field_data.get("type", "string")
+                if field_data.get("description", None):
+                    docs[field_name] = field_data["description"]
+                if field_data.get("enum", []):
+                    fields[field_name] = (
+                        list_to_enum(field_name, field_data.get("enum", [])),
+                        ...,
+                    )
+                elif field_type == "array":
+                    items = field_data.get("items", {})
+                    if items != {}:
+                        array = {"properties": items}
+                        array_type = convert_dictionary_to_pydantic_model(
+                            array,
+                            f"{model_name}_{field_name}_items",
+                            docs,
+                            docs_function,
+                        )
+                        fields[field_name] = (List[array_type], ...)  # type: ignore[valid-type]
+                    else:
+                        fields[field_name] = (list, ...)
+                elif field_type == "object":
+                    submodel = convert_dictionary_to_pydantic_model(
+                        field_data, f"{model_name}_{field_name}", docs, docs_function
+                    )
+                    fields[field_name] = (submodel, ...)
+                elif field_type == "required":
+                    required = field_data
+                    for key, field in fields.items():
+                        if key not in required:
+                            fields[key] = (Optional[fields[key][0]], ...)
+                else:
+                    field_type = json_schema_to_python_types(field_type)
+                    fields[field_name] = (field_type, ...)
+    if "function" in dictionary:
+        for field_name, field_data in dictionary.get("function", {}).items():
+            if field_name == "name":
+                model_name = field_data
+            elif field_name == "description":
+                docs_function["__doc__"] = field_data
+            elif field_name == "parameters":
+                return convert_dictionary_to_pydantic_model(
+                    field_data, f"{model_name}", docs, docs_function
+                )
+
+    if "parameters" in dictionary:
+        field_data = {"function": dictionary}
+        return convert_dictionary_to_pydantic_model(
+            field_data, f"{model_name}", docs, docs_function
+        )
+    if "required" in dictionary:
+        required = dictionary.get("required", [])
+        for key, field in fields.items():
+            if key not in required:
+                fields[key] = (Optional[fields[key][0]], ...)
+    custom_model = create_model(model_name, **fields)
+
+    if "__doc__" in docs_function:
+        custom_model.__doc__ = docs_function["__doc__"]
+    for field_name, doc in docs.items():
+        custom_model.model_fields[field_name].description = doc
+
+    return custom_model
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/hermes_2_pro_agent.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/hermes_2_pro_agent.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,307 +1,307 @@
-import json
-import random
-import re
-import string
-import uuid
-from enum import Enum
-from typing import List, Dict, Literal, Tuple
-
-from llama_cpp import Llama
-from pydantic import ValidationError
-from transformers import AutoTokenizer
-
-from llama_cpp_agent.chat_history import ChatMessage, SystemMessage, UserMessage
-from llama_cpp_agent.chat_history.messages import convert_messages_to_list_of_dictionaries, ToolCall, FunctionCall, \
-    ToolMessage, AssistantMessage
-from llama_cpp_agent.function_calling import LlamaCppFunctionTool
-from llama_cpp_agent.llm_agent import LlamaCppAgent
-from llama_cpp_agent.llm_output_settings import LlmStructuredOutputSettings
-from llama_cpp_agent.llm_prompt_template import PromptTemplate
-from llama_cpp_agent.messages_formatter import MessagesFormatter
-
-from llama_cpp_agent.providers.provider_base import LlmProvider
-
-
-def generate_id(length=8):
-    # Characters to use in the ID
-    characters = string.ascii_letters + string.digits
-    # Random choice of characters
-    return "".join(random.choice(characters) for _ in range(length))
-
-
-def parse_tool_calls(text):
-    # List to hold all extracted dictionaries
-    json_dicts = []
-
-    # Regular expression to find <tool_call>...</tool_call> patterns
-    tool_call_pattern = r"<tool_call>(.*?)</tool_call>"
-
-    # Find all occurrences of the pattern
-    tool_calls = re.findall(tool_call_pattern, text, re.DOTALL)
-
-    # Process each JSON within the found tags
-    for json_text in tool_calls:
-        json_text = json_text.strip()
-        try:
-            json_dict = json.loads(json_text)
-            json_dicts.append(json_dict)
-        except json.JSONDecodeError as e:
-            print(f"Error decoding JSON: {e}")
-
-    return json_dicts
-
-
-class Hermes2ProMessageFormatter(MessagesFormatter):
-    """
-    Class representing a messages formatter for LLMs.
-    """
-
-    def __init__(self, PRE_PROMPT: str = "", SYS_PROMPT_START: str = "", SYS_PROMPT_END: str = "", USER_PROMPT_START: str = "",
-                 USER_PROMPT_END: str = "", ASSISTANT_PROMPT_START: str = "", ASSISTANT_PROMPT_END: str = "",
-                 INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE: bool = False, DEFAULT_STOP_SEQUENCES: List[str] = None):
-        """
-        Initializes a new MessagesFormatter object.
-        """
-        super().__init__(PRE_PROMPT, SYS_PROMPT_START, SYS_PROMPT_END, USER_PROMPT_START, USER_PROMPT_END,
-                         ASSISTANT_PROMPT_START, ASSISTANT_PROMPT_END, INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE,
-                         DEFAULT_STOP_SEQUENCES)
-        SYS_PROMPT_START_MIXTRAL = """"""
-        SYS_PROMPT_END_MIXTRAL = """\n\n"""
-        USER_PROMPT_START_MIXTRAL = """[INST] """
-        USER_PROMPT_END_MIXTRAL = """ """
-        ASSISTANT_PROMPT_START_MIXTRAL = """[/INST] """
-        ASSISTANT_PROMPT_END_MIXTRAL = """</s>"""
-        FUNCTION_PROMPT_START_MIXTRAL = """"""
-        FUNCTION_PROMPT_END_MIXTRAL = """"""
-        DEFAULT_MIXTRAL_STOP_SEQUENCES = ["</s>"]
-        self.PRE_PROMPT = ""
-        self.SYS_PROMPT_START = "<|im_start|>system\n"
-        self.SYS_PROMPT_END = "<|im_end|>\n"
-        self.USER_PROMPT_START = "<|im_start|>user\n"
-        self.USER_PROMPT_END = "<|im_end|>\n"
-        self.ASSISTANT_PROMPT_START = "<|im_start|>assistant\n"
-        self.ASSISTANT_PROMPT_END = "<|im_end|>\n"
-        self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE = False
-
-        self.DEFAULT_STOP_SEQUENCES = [
-            "<|im_end|>",
-            "<|im_start|>assistant",
-            "<|im_start|>user",
-            "<|im_start|>system"
-        ]
-        self.FUNCTION_PROMPT_START = "<|im_start|>tool\n"
-        self.FUNCTION_PROMPT_END = "<|im_end|>\n"
-        self.USE_USER_ROLE_FUNCTION_CALL_RESULT = False
-        self.STRIP_PROMPT = True
-
-    def format_messages(
-        self,
-        messages: List[Dict[str, str]],
-        response_role: Literal["user", "assistant"] | None = None,
-    ) -> Tuple[str, str]:
-        """
-        Formats a list of messages into a conversation string.
-
-        Args:
-            messages (List[Dict[str, str]]): List of messages with role and content.
-            response_role(Literal["system", "user", "assistant", "function"]|None): Forces the response role to be "system", "user" or "assistant".
-        Returns:
-            Tuple[str, str]: Formatted conversation string and the role of the last message.
-        """
-        formatted_messages = self.PRE_PROMPT
-        last_role = "assistant"
-
-        no_user_prompt_start = False
-        for message in messages:
-            if message["role"] == "system":
-                formatted_messages += (
-                    self.SYS_PROMPT_START + message["content"] + self.SYS_PROMPT_END
-                )
-                last_role = "system"
-                if self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE:
-                    formatted_messages = self.USER_PROMPT_START + formatted_messages
-                    no_user_prompt_start = True
-            elif message["role"] == "user":
-                if no_user_prompt_start:
-                    no_user_prompt_start = False
-                    formatted_messages += message["content"] + self.USER_PROMPT_END
-                else:
-                    formatted_messages += (
-                        self.USER_PROMPT_START
-                        + message["content"]
-                        + self.USER_PROMPT_END
-                    )
-                last_role = "user"
-            elif message["role"] == "assistant":
-                if self.STRIP_PROMPT:
-                    message["content"] = message["content"].strip()
-                formatted_messages += (
-                    self.ASSISTANT_PROMPT_START
-                    + message["content"]
-                    + self.ASSISTANT_PROMPT_END
-                )
-                last_role = "assistant"
-            elif message["role"] == "tool":
-                if isinstance(message["content"], list):
-                    message["content"] = "\n".join(
-                        [json.dumps(m, indent=2) for m in message["content"]]
-                    )
-                if self.USE_USER_ROLE_FUNCTION_CALL_RESULT:
-                    formatted_messages += (
-                        self.USER_PROMPT_START
-                        + message["content"]
-                        + self.USER_PROMPT_END
-                    )
-                    last_role = "user"
-                else:
-                    formatted_messages += (
-                        self.FUNCTION_PROMPT_START
-                        + message["content"]
-                        + self.FUNCTION_PROMPT_END
-                    )
-                    last_role = "tool"
-        if last_role == "system" or last_role == "user" or last_role == "tool":
-            if self.STRIP_PROMPT:
-                if response_role is not None:
-                    if response_role == "assistant":
-                        return (
-                            formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
-                            "assistant",
-                        )
-                    if response_role == "user":
-                        return (
-                            formatted_messages + self.USER_PROMPT_START.strip(),
-                            "user",
-                        )
-                else:
-                    return (
-                        formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
-                        "assistant",
-                    )
-            else:
-                if response_role is not None:
-                    if response_role == "assistant":
-                        return (
-                            formatted_messages + self.ASSISTANT_PROMPT_START,
-                            "assistant",
-                        )
-                    if response_role == "user":
-                        return formatted_messages + self.USER_PROMPT_START, "user"
-                else:
-                    return formatted_messages + self.ASSISTANT_PROMPT_START, "assistant"
-        if self.STRIP_PROMPT:
-            if response_role is not None:
-                if response_role == "assistant":
-                    return (
-                        formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
-                        "assistant",
-                    )
-                if response_role == "user":
-                    return formatted_messages + self.USER_PROMPT_START.strip(), "user"
-            else:
-                return formatted_messages + self.USER_PROMPT_START.strip(), "user"
-        else:
-            if response_role is not None:
-                if response_role == "assistant":
-                    return formatted_messages + self.ASSISTANT_PROMPT_START, "assistant"
-                if response_role == "user":
-                    return formatted_messages + self.USER_PROMPT_START, "user"
-            else:
-                return formatted_messages + self.USER_PROMPT_START, "user"
-
-
-class Hermes2ProAgent:
-    def __init__(
-        self,
-        provider: LlmProvider,
-        system_prompt: str = None,
-        debug_output: bool = False,
-    ):
-        self.messages: list[ChatMessage] = []
-        self.messages_formatter = Hermes2ProMessageFormatter()
-        self.agent = LlamaCppAgent(provider, debug_output=debug_output, custom_messages_formatter=self.messages_formatter)
-        self.debug_output = debug_output
-        if system_prompt is not None:
-            self.system_prompt = system_prompt
-        else:
-            self.system_prompt = "You are a function calling AI model. You are provided with function signatures within <tools></tools> XML tags. You may call one or more functions to assist with the user query. Don't make assumptions about what values to plug into functions.\nHere are the available tools:"
-        self.messages.append(SystemMessage(content="system_prompt"))
-
-        self.sys_prompt_template = """{system_prompt} <tools> {tools} </tools>
-Use the following pydantic model json schema for each tool call you will make: {"properties": {"arguments": {"title": "Arguments", "type": "object"}, "name": {"title": "Name", "type": "string"}}, "required": ["arguments", "name"], "title": "FunctionCall", "type": "object"} 
-For each function call return a json object with function name and arguments within <tool_call></tool_call> XML tags as follows:
-<tool_call>
-{"arguments": <args-dict>, "name": <function-name>}
-</tool_call>
-"""
-        self.system_prompter = PromptTemplate.from_string(self.sys_prompt_template)
-
-    def get_response(
-        self,
-        message=None,
-        structured_output_settings: LlmStructuredOutputSettings = None,
-    ):
-        if message is not None:
-            msg = UserMessage(content=message)
-            self.messages.append(msg)
-        openai_tools = []
-        openai_tool_mapping = {}
-        for tool in structured_output_settings.function_tools:
-            openai_tools.append(tool.to_openai_tool())
-            openai_tool_mapping[tool.model.__name__] = tool
-
-        self.messages[0].content = self.system_prompter.generate_prompt(
-            {"tools": json.dumps(openai_tools), "system_prompt": self.system_prompt}
-        )
-        text, role = self.messages_formatter.format_messages(
-            convert_messages_to_list_of_dictionaries(self.messages)
-        )
-
-        if self.debug_output:
-            print(text)
-        result = self.agent.get_text_response(
-            text,
-
-            print_output=self.debug_output,
-        )
-
-        if "<tool_call>" in result:
-            tool_calls = []
-            if result.strip().endswith("</tool_call"):
-                result += ">"
-            function_calls = parse_tool_calls(result)
-            tool_messages = []
-            for function_call in function_calls:
-                tool = openai_tool_mapping[function_call["name"]]
-                cls = tool.model
-                call_parameters = function_call["arguments"]
-                try:
-                    call = cls(**call_parameters)
-                    output = call.run(**tool.additional_parameters)
-                    tool_call_id = generate_id(length=9)
-                    tool_calls.append(
-                        ToolCall(
-                            function=FunctionCall(
-                                name=function_call["name"],
-                                arguments=json.dumps(call_parameters),
-                            ),
-                            id=tool_call_id,
-                        )
-                    )
-                    tool_messages.append(
-                        ToolMessage(content=str(output), tool_call_id=tool_call_id)
-                    )
-                except ValidationError as e:
-                    tool_messages.append(ToolMessage(content=str(e), tool_call_id="-1"))
-                    self.messages.append(
-                        AssistantMessage(content=result, tool_calls=tool_calls)
-                    )
-                    self.messages.extend(tool_messages)
-            self.messages.append(
-                AssistantMessage(content=result, tool_calls=tool_calls)
-            )
-            self.messages.extend(tool_messages)
-            return self.get_response(structured_output_settings=structured_output_settings)
-        else:
-            self.messages.append(AssistantMessage(content=result.strip()))
-            return result.strip()
+import json
+import random
+import re
+import string
+import uuid
+from enum import Enum
+from typing import List, Dict, Literal, Tuple
+
+from llama_cpp import Llama
+from pydantic import ValidationError
+from transformers import AutoTokenizer
+
+from llama_cpp_agent.chat_history import ChatMessage, SystemMessage, UserMessage
+from llama_cpp_agent.chat_history.messages import convert_messages_to_list_of_dictionaries, ToolCall, FunctionCall, \
+    ToolMessage, AssistantMessage
+from llama_cpp_agent.function_calling import LlamaCppFunctionTool
+from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.llm_output_settings import LlmStructuredOutputSettings
+from llama_cpp_agent.llm_prompt_template import PromptTemplate
+from llama_cpp_agent.messages_formatter import MessagesFormatter
+
+from llama_cpp_agent.providers.provider_base import LlmProvider
+
+
+def generate_id(length=8):
+    # Characters to use in the ID
+    characters = string.ascii_letters + string.digits
+    # Random choice of characters
+    return "".join(random.choice(characters) for _ in range(length))
+
+
+def parse_tool_calls(text):
+    # List to hold all extracted dictionaries
+    json_dicts = []
+
+    # Regular expression to find <tool_call>...</tool_call> patterns
+    tool_call_pattern = r"<tool_call>(.*?)</tool_call>"
+
+    # Find all occurrences of the pattern
+    tool_calls = re.findall(tool_call_pattern, text, re.DOTALL)
+
+    # Process each JSON within the found tags
+    for json_text in tool_calls:
+        json_text = json_text.strip()
+        try:
+            json_dict = json.loads(json_text)
+            json_dicts.append(json_dict)
+        except json.JSONDecodeError as e:
+            print(f"Error decoding JSON: {e}")
+
+    return json_dicts
+
+
+class Hermes2ProMessageFormatter(MessagesFormatter):
+    """
+    Class representing a messages formatter for LLMs.
+    """
+
+    def __init__(self, PRE_PROMPT: str = "", SYS_PROMPT_START: str = "", SYS_PROMPT_END: str = "", USER_PROMPT_START: str = "",
+                 USER_PROMPT_END: str = "", ASSISTANT_PROMPT_START: str = "", ASSISTANT_PROMPT_END: str = "",
+                 INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE: bool = False, DEFAULT_STOP_SEQUENCES: List[str] = None):
+        """
+        Initializes a new MessagesFormatter object.
+        """
+        super().__init__(PRE_PROMPT, SYS_PROMPT_START, SYS_PROMPT_END, USER_PROMPT_START, USER_PROMPT_END,
+                         ASSISTANT_PROMPT_START, ASSISTANT_PROMPT_END, INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE,
+                         DEFAULT_STOP_SEQUENCES)
+        SYS_PROMPT_START_MIXTRAL = """"""
+        SYS_PROMPT_END_MIXTRAL = """\n\n"""
+        USER_PROMPT_START_MIXTRAL = """[INST] """
+        USER_PROMPT_END_MIXTRAL = """ """
+        ASSISTANT_PROMPT_START_MIXTRAL = """[/INST] """
+        ASSISTANT_PROMPT_END_MIXTRAL = """</s>"""
+        FUNCTION_PROMPT_START_MIXTRAL = """"""
+        FUNCTION_PROMPT_END_MIXTRAL = """"""
+        DEFAULT_MIXTRAL_STOP_SEQUENCES = ["</s>"]
+        self.PRE_PROMPT = ""
+        self.SYS_PROMPT_START = "<|im_start|>system\n"
+        self.SYS_PROMPT_END = "<|im_end|>\n"
+        self.USER_PROMPT_START = "<|im_start|>user\n"
+        self.USER_PROMPT_END = "<|im_end|>\n"
+        self.ASSISTANT_PROMPT_START = "<|im_start|>assistant\n"
+        self.ASSISTANT_PROMPT_END = "<|im_end|>\n"
+        self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE = False
+
+        self.DEFAULT_STOP_SEQUENCES = [
+            "<|im_end|>",
+            "<|im_start|>assistant",
+            "<|im_start|>user",
+            "<|im_start|>system"
+        ]
+        self.FUNCTION_PROMPT_START = "<|im_start|>tool\n"
+        self.FUNCTION_PROMPT_END = "<|im_end|>\n"
+        self.USE_USER_ROLE_FUNCTION_CALL_RESULT = False
+        self.STRIP_PROMPT = True
+
+    def format_messages(
+        self,
+        messages: List[Dict[str, str]],
+        response_role: Literal["user", "assistant"] | None = None,
+    ) -> Tuple[str, str]:
+        """
+        Formats a list of messages into a conversation string.
+
+        Args:
+            messages (List[Dict[str, str]]): List of messages with role and content.
+            response_role(Literal["system", "user", "assistant", "function"]|None): Forces the response role to be "system", "user" or "assistant".
+        Returns:
+            Tuple[str, str]: Formatted conversation string and the role of the last message.
+        """
+        formatted_messages = self.PRE_PROMPT
+        last_role = "assistant"
+
+        no_user_prompt_start = False
+        for message in messages:
+            if message["role"] == "system":
+                formatted_messages += (
+                    self.SYS_PROMPT_START + message["content"] + self.SYS_PROMPT_END
+                )
+                last_role = "system"
+                if self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE:
+                    formatted_messages = self.USER_PROMPT_START + formatted_messages
+                    no_user_prompt_start = True
+            elif message["role"] == "user":
+                if no_user_prompt_start:
+                    no_user_prompt_start = False
+                    formatted_messages += message["content"] + self.USER_PROMPT_END
+                else:
+                    formatted_messages += (
+                        self.USER_PROMPT_START
+                        + message["content"]
+                        + self.USER_PROMPT_END
+                    )
+                last_role = "user"
+            elif message["role"] == "assistant":
+                if self.STRIP_PROMPT:
+                    message["content"] = message["content"].strip()
+                formatted_messages += (
+                    self.ASSISTANT_PROMPT_START
+                    + message["content"]
+                    + self.ASSISTANT_PROMPT_END
+                )
+                last_role = "assistant"
+            elif message["role"] == "tool":
+                if isinstance(message["content"], list):
+                    message["content"] = "\n".join(
+                        [json.dumps(m, indent=2) for m in message["content"]]
+                    )
+                if self.USE_USER_ROLE_FUNCTION_CALL_RESULT:
+                    formatted_messages += (
+                        self.USER_PROMPT_START
+                        + message["content"]
+                        + self.USER_PROMPT_END
+                    )
+                    last_role = "user"
+                else:
+                    formatted_messages += (
+                        self.FUNCTION_PROMPT_START
+                        + message["content"]
+                        + self.FUNCTION_PROMPT_END
+                    )
+                    last_role = "tool"
+        if last_role == "system" or last_role == "user" or last_role == "tool":
+            if self.STRIP_PROMPT:
+                if response_role is not None:
+                    if response_role == "assistant":
+                        return (
+                            formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
+                            "assistant",
+                        )
+                    if response_role == "user":
+                        return (
+                            formatted_messages + self.USER_PROMPT_START.strip(),
+                            "user",
+                        )
+                else:
+                    return (
+                        formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
+                        "assistant",
+                    )
+            else:
+                if response_role is not None:
+                    if response_role == "assistant":
+                        return (
+                            formatted_messages + self.ASSISTANT_PROMPT_START,
+                            "assistant",
+                        )
+                    if response_role == "user":
+                        return formatted_messages + self.USER_PROMPT_START, "user"
+                else:
+                    return formatted_messages + self.ASSISTANT_PROMPT_START, "assistant"
+        if self.STRIP_PROMPT:
+            if response_role is not None:
+                if response_role == "assistant":
+                    return (
+                        formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
+                        "assistant",
+                    )
+                if response_role == "user":
+                    return formatted_messages + self.USER_PROMPT_START.strip(), "user"
+            else:
+                return formatted_messages + self.USER_PROMPT_START.strip(), "user"
+        else:
+            if response_role is not None:
+                if response_role == "assistant":
+                    return formatted_messages + self.ASSISTANT_PROMPT_START, "assistant"
+                if response_role == "user":
+                    return formatted_messages + self.USER_PROMPT_START, "user"
+            else:
+                return formatted_messages + self.USER_PROMPT_START, "user"
+
+
+class Hermes2ProAgent:
+    def __init__(
+        self,
+        provider: LlmProvider,
+        system_prompt: str = None,
+        debug_output: bool = False,
+    ):
+        self.messages: list[ChatMessage] = []
+        self.messages_formatter = Hermes2ProMessageFormatter()
+        self.agent = LlamaCppAgent(provider, debug_output=debug_output, custom_messages_formatter=self.messages_formatter)
+        self.debug_output = debug_output
+        if system_prompt is not None:
+            self.system_prompt = system_prompt
+        else:
+            self.system_prompt = "You are a function calling AI model. You are provided with function signatures within <tools></tools> XML tags. You may call one or more functions to assist with the user query. Don't make assumptions about what values to plug into functions.\nHere are the available tools:"
+        self.messages.append(SystemMessage(content="system_prompt"))
+
+        self.sys_prompt_template = """{system_prompt} <tools> {tools} </tools>
+Use the following pydantic model json schema for each tool call you will make: {"properties": {"arguments": {"title": "Arguments", "type": "object"}, "name": {"title": "Name", "type": "string"}}, "required": ["arguments", "name"], "title": "FunctionCall", "type": "object"} 
+For each function call return a json object with function name and arguments within <tool_call></tool_call> XML tags as follows:
+<tool_call>
+{"arguments": <args-dict>, "name": <function-name>}
+</tool_call>
+"""
+        self.system_prompter = PromptTemplate.from_string(self.sys_prompt_template)
+
+    def get_response(
+        self,
+        message=None,
+        structured_output_settings: LlmStructuredOutputSettings = None,
+    ):
+        if message is not None:
+            msg = UserMessage(content=message)
+            self.messages.append(msg)
+        openai_tools = []
+        openai_tool_mapping = {}
+        for tool in structured_output_settings.function_tools:
+            openai_tools.append(tool.to_openai_tool())
+            openai_tool_mapping[tool.model.__name__] = tool
+
+        self.messages[0].content = self.system_prompter.generate_prompt(
+            {"tools": json.dumps(openai_tools), "system_prompt": self.system_prompt}
+        )
+        text, role = self.messages_formatter.format_messages(
+            convert_messages_to_list_of_dictionaries(self.messages)
+        )
+
+        if self.debug_output:
+            print(text)
+        result = self.agent.get_text_response(
+            text,
+
+            print_output=self.debug_output,
+        )
+
+        if "<tool_call>" in result:
+            tool_calls = []
+            if result.strip().endswith("</tool_call"):
+                result += ">"
+            function_calls = parse_tool_calls(result)
+            tool_messages = []
+            for function_call in function_calls:
+                tool = openai_tool_mapping[function_call["name"]]
+                cls = tool.model
+                call_parameters = function_call["arguments"]
+                try:
+                    call = cls(**call_parameters)
+                    output = call.run(**tool.additional_parameters)
+                    tool_call_id = generate_id(length=9)
+                    tool_calls.append(
+                        ToolCall(
+                            function=FunctionCall(
+                                name=function_call["name"],
+                                arguments=json.dumps(call_parameters),
+                            ),
+                            id=tool_call_id,
+                        )
+                    )
+                    tool_messages.append(
+                        ToolMessage(content=str(output), tool_call_id=tool_call_id)
+                    )
+                except ValidationError as e:
+                    tool_messages.append(ToolMessage(content=str(e), tool_call_id="-1"))
+                    self.messages.append(
+                        AssistantMessage(content=result, tool_calls=tool_calls)
+                    )
+                    self.messages.extend(tool_messages)
+            self.messages.append(
+                AssistantMessage(content=result, tool_calls=tool_calls)
+            )
+            self.messages.extend(tool_messages)
+            return self.get_response(structured_output_settings=structured_output_settings)
+        else:
+            self.messages.append(AssistantMessage(content=result.strip()))
+            return result.strip()
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_agent.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/llm_agent.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,459 +1,459 @@
-from copy import deepcopy
-from dataclasses import dataclass
-from typing import List, Literal, Callable, Union, Generator, Any
-
-from pydantic import BaseModel
-
-from .chat_history.basic_chat_history import BasicChatHistory
-from .chat_history.chat_history_base import ChatHistory
-from .chat_history.messages import Roles
-
-from .llm_output_settings import LlmStructuredOutputSettings, LlmStructuredOutputType
-
-from .messages_formatter import (
-    MessagesFormatterType,
-    get_predefined_messages_formatter,
-    MessagesFormatter,
-)
-from .prompt_templates import function_calling_thoughts_and_reasoning, \
-    function_calling_thoughts_and_reasoning_json_schema, function_calling_without_thoughts_and_reasoning_json_schema, \
-    function_calling_without_thoughts_and_reasoning, structured_output_thoughts_and_reasoning_json_schema, \
-    structured_output_without_thoughts_and_reasoning_json_schema, structured_output_thoughts_and_reasoning, \
-    structured_output_without_thoughts_and_reasoning
-
-from .providers.provider_base import LlmProvider, LlmSamplingSettings
-
-
-@dataclass
-class StreamingResponse:
-    """
-    Represents a streaming response with text and an indicator for the last response.
-    """
-
-    text: str
-    is_last_response: bool
-
-    def __init__(self, text: str, is_last_response: bool):
-        """
-        Initializes a new StreamingResponse object.
-
-        Args:
-            text (str): The text content of the streaming response.
-            is_last_response (bool): Indicates whether this is the last response in the stream.
-        """
-        self.text = text
-        self.is_last_response = is_last_response
-
-
-class LlamaCppAgent:
-    """
-    A base agent that can be used for chat, structured output and function calling.
-    """
-
-    def __init__(
-            self,
-            provider: LlmProvider,
-            name: str = "llamacpp_agent",
-            system_prompt: str = "You are a helpful assistant.",
-            predefined_messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
-            custom_messages_formatter: MessagesFormatter = None,
-            chat_history: ChatHistory = None,
-            add_tools_and_structures_documentation_to_system_prompt: bool = True,
-            debug_output: bool = False,
-    ):
-        """
-        Initializes a new LlamaCppAgent object.
-
-        Args:
-           provider (LlmProvider):The underlying llm provider (LlamaCppServerProvider, LlamaCppPythonProvider, TGIServerProvider or VLLMServerProvider).
-           name (str): The name of the agent.
-           system_prompt (str): The system prompt used in chat interactions.
-           predefined_messages_formatter_type (MessagesFormatterType): The type of predefined messages formatter.
-           custom_messages_formatter (MessagesFormatter): Custom message's formatter.
-           chat_history (ChatHistory): This will handle the chat history.
-           add_tools_and_structures_documentation_to_system_prompt (bool): Will suffix system prompt dynamically with documentation for function calling or structured output.
-           debug_output (bool): Indicates whether debug output should be enabled.
-        """
-        self.provider = provider
-        self.name = name
-        self.debug_output = debug_output
-        if custom_messages_formatter is not None:
-            self.messages_formatter = custom_messages_formatter
-        else:
-            self.messages_formatter = get_predefined_messages_formatter(
-                predefined_messages_formatter_type
-            )
-        self.last_response = ""
-        if chat_history is None:
-            self.chat_history = BasicChatHistory()
-        else:
-            self.chat_history = chat_history
-
-        self.add_message(role=Roles.system, message=system_prompt)
-        self.system_prompt = system_prompt
-        self.add_tools_and_structures_documentation_to_system_prompt = add_tools_and_structures_documentation_to_system_prompt
-
-    def add_message(
-            self,
-            message: str,
-            role: Roles,
-    ):
-        """
-        Adds a message to the chat history.
-
-        Args:
-            message (str): The content of the message.
-            role (Literal["system"] | Literal["user"] | Literal["assistant"] | Literal["tool"]): The role of the message sender.
-        """
-        self.chat_history.add_message(
-            {
-                "role": role,
-                "content": message,
-            }
-        )
-
-    def get_text_response(
-            self,
-            prompt: str = None,
-            structured_output_settings: LlmStructuredOutputSettings = None,
-            llm_sampling_settings: LlmSamplingSettings = None,
-            streaming_callback: Callable[[StreamingResponse], None] = None,
-            returns_streaming_generator: bool = False,
-            print_output: bool = False,
-    ) -> Union[
-        str,
-        List[dict],
-        BaseModel,
-        Generator[Any, Any, str | BaseModel | list[BaseModel]],
-    ]:
-        """
-        Get a text response from the LLM provider.
-
-        Args:
-            prompt (str | list[int]): The prompt for the LLM.
-            structured_output_settings (LlmStructuredOutputSettings): Settings for structured output.
-            llm_sampling_settings (LlmSamplingSettings): Sampling settings for the LLM.
-            streaming_callback (Callable[[StreamingResponse], None]): Callback for streaming responses.
-            returns_streaming_generator (bool): Whether to return a generator streaming the results.
-            print_output (bool): Whether to print the output.
-
-        Returns:
-            Union[str, List[dict], BaseModel, Generator[Any, Any, str | BaseModel | list[BaseModel]]: The generated response. A string message, a list of function calls, an object from structured output or a generator for the response
-        """
-
-        if self.debug_output:
-            if type(prompt) is str:
-                print(prompt, end="")
-
-        if structured_output_settings is None:
-            structured_output_settings = LlmStructuredOutputSettings(
-                output_type=LlmStructuredOutputType.no_structured_output
-            )
-        if llm_sampling_settings is None:
-            llm_sampling_settings = self.provider.get_provider_default_settings()
-        else:
-            llm_sampling_settings = deepcopy(llm_sampling_settings)
-
-        if llm_sampling_settings.get_additional_stop_sequences() is not None:
-            llm_sampling_settings.add_additional_stop_sequences(
-                self.messages_formatter.default_stop_sequences
-            )
-
-        if self.provider:
-            completion = self.get_text_completion(
-                prompt=prompt,
-                structured_output_settings=structured_output_settings,
-                llm_samplings_settings=llm_sampling_settings,
-            )
-
-            def stream_results():
-                full_response_stream = ""
-                for out_stream in completion:
-                    out_text = out_stream["choices"][0]["text"]
-                    full_response_stream += text
-                    yield out_text
-                return structured_output_settings.handle_structured_output(
-                    full_response_stream
-                )
-
-            if llm_sampling_settings.is_streaming():
-                full_response = ""
-                if returns_streaming_generator:
-                    return stream_results()
-                for out in completion:
-                    text = out["choices"][0]["text"]
-                    full_response += text
-                    if streaming_callback is not None:
-                        streaming_callback(
-                            StreamingResponse(text=text, is_last_response=False)
-                        )
-                    if print_output:
-                        print(text, end="")
-                if streaming_callback is not None:
-                    streaming_callback(
-                        StreamingResponse(text="", is_last_response=True)
-                    )
-                if print_output or self.debug_output:
-                    print("")
-                self.last_response = full_response
-                return structured_output_settings.handle_structured_output(
-                    full_response
-                )
-            else:
-                full_response = ""
-                text = completion["choices"][0]["text"]
-                full_response += text
-                if print_output or self.debug_output:
-                    print(full_response)
-                self.last_response = full_response
-                return structured_output_settings.handle_structured_output(
-                    full_response
-                )
-        return "Error: No model loaded!"
-
-    def get_chat_response(
-            self,
-            message: str = None,
-            role: Roles = Roles.user,
-            prompt_suffix: str = None,
-            chat_history: ChatHistory = None,
-            system_prompt: str = None,
-            add_message_to_chat_history: bool = True,
-            add_response_to_chat_history: bool = True,
-            structured_output_settings: LlmStructuredOutputSettings = None,
-            llm_sampling_settings: LlmSamplingSettings = None,
-            streaming_callback: Callable[[StreamingResponse], None] = None,
-            returns_streaming_generator: bool = False,
-            print_output: bool = False,
-    ) -> Union[
-        str,
-        List[dict],
-        BaseModel,
-        Generator[Any, Any, str | BaseModel | list[BaseModel]],
-    ]:
-        """
-        Get a chat response based on the input message and context.
-
-        Args:
-            message (str): The input message.
-            role (Literal["system", "user", "assistant", "tool"]): The role of the message sender.
-            prompt_suffix (str): Suffix to append after the prompt.
-            chat_history (ChatHistory): Overwrite internal ChatHistory of the agent.
-            system_prompt (str): Overwrites the system prompt set on the agent initialization.
-            add_message_to_chat_history (bool): Whether to add the input message to the chat history.
-            add_response_to_chat_history (bool): Whether to add the generated response to the chat history.
-            structured_output_settings (LlmStructuredOutputSettings): Settings for structured output.
-            llm_sampling_settings (LlmSamplingSettings): Sampling settings for the LLM.
-            streaming_callback (Callable[[StreamingResponse], None]): Callback for streaming responses.
-            returns_streaming_generator (bool): Whether to return a generator streaming the results.
-            print_output (bool): Whether to print the generated response.
-
-        Returns:
-            Union[str, List[dict], BaseModel, Generator[Any, Any, str | BaseModel | list[BaseModel]]: The generated chat response. A string message, a list of function calls, an object from structured output or a generator for the response
-        """
-        if chat_history is None:
-            chat_history = self.chat_history
-
-        if structured_output_settings is None:
-            structured_output_settings = LlmStructuredOutputSettings(
-                output_type=LlmStructuredOutputType.no_structured_output
-            )
-        if llm_sampling_settings is None:
-            llm_sampling_settings = self.provider.get_provider_default_settings()
-        else:
-            llm_sampling_settings = deepcopy(llm_sampling_settings)
-
-        if llm_sampling_settings.get_additional_stop_sequences() is not None:
-            llm_sampling_settings.add_additional_stop_sequences(
-                self.messages_formatter.default_stop_sequences
-            )
-
-        completion, response_role = self.get_response_role_and_completion(
-            message=message,
-            chat_history=chat_history,
-            system_prompt=system_prompt,
-            add_message_to_chat_history=add_message_to_chat_history,
-            role=role,
-            prompt_suffix=prompt_suffix,
-            structured_output_settings=structured_output_settings,
-            llm_sampling_settings=llm_sampling_settings,
-        )
-
-        def stream_results():
-            full_response_stream = ""
-            for out_stream in completion:
-                out_text = out_stream["choices"][0]["text"]
-                if out_text != self.messages_formatter.eos_token:
-                    full_response_stream += text
-                    yield out_text
-            self.last_response = full_response
-            if add_response_to_chat_history:
-                chat_history.add_message(
-                    {
-                        "role": response_role,
-                        "content": full_response,
-                    }
-                )
-            return structured_output_settings.handle_structured_output(
-                full_response_stream
-            )
-
-        if self.provider:
-            if returns_streaming_generator:
-                return stream_results()
-            if llm_sampling_settings.is_streaming():
-                full_response = ""
-                for out in completion:
-                    text = out["choices"][0]["text"]
-                    if text != self.messages_formatter.eos_token:
-                        full_response += text
-                        if streaming_callback is not None:
-                            streaming_callback(
-                                StreamingResponse(text=text, is_last_response=False)
-                            )
-                        if print_output or self.debug_output:
-                            print(text, end="")
-                if streaming_callback is not None:
-                    streaming_callback(
-                        StreamingResponse(text="", is_last_response=True)
-                    )
-                if print_output or self.debug_output:
-                    print("")
-                self.last_response = full_response
-                if add_response_to_chat_history:
-                    chat_history.add_message(
-                        {
-                            "role": response_role,
-                            "content": full_response,
-                        }
-                    )
-
-                return structured_output_settings.handle_structured_output(
-                    full_response
-                )
-            else:
-                text = completion["choices"][0]["text"]
-                if text.strip().endswith(self.messages_formatter.eos_token):
-                    text = text.replace(self.messages_formatter.eos_token, "")
-                if print_output or self.debug_output:
-                    print(text)
-                self.last_response = text
-                if add_response_to_chat_history:
-                    chat_history.add_message(
-                        {
-                            "role": response_role,
-                            "content": text,
-                        }
-                    )
-
-                return structured_output_settings.handle_structured_output(text)
-        return "Error: No model loaded!"
-
-    def get_text_completion(
-            self,
-            prompt: str | list[int] = None,
-            structured_output_settings: LlmStructuredOutputSettings = None,
-            llm_samplings_settings: LlmSamplingSettings = None,
-    ):
-        return self.provider.create_completion(
-            prompt,
-            structured_output_settings,
-            llm_samplings_settings,
-            self.messages_formatter.bos_token,
-        )
-
-    def get_response_role_and_completion(
-            self,
-            message: str = None,
-            chat_history: ChatHistory = None,
-            system_prompt: str = None,
-            add_message_to_chat_history: bool = True,
-            role: Roles = Roles.user,
-            prompt_suffix: str = None,
-            llm_sampling_settings: LlmSamplingSettings = None,
-            structured_output_settings: LlmStructuredOutputSettings = None,
-    ):
-        if message is not None and add_message_to_chat_history:
-            chat_history.add_message(
-                {
-                    "role": role,
-                    "content": message,
-                }
-            )
-
-        messages = chat_history.get_chat_messages()
-        if message is not None and not add_message_to_chat_history:
-            messages.append(
-                {
-                    "role": role,
-                    "content": message,
-                },
-            )
-        if system_prompt:
-            messages[0]["content"] = system_prompt
-        else:
-            messages[0]["content"] = self.system_prompt
-        additional_suffix = ""
-        if self.add_tools_and_structures_documentation_to_system_prompt:
-            if structured_output_settings.output_type != LlmStructuredOutputType.no_structured_output:
-                additional_suffix = "\n"
-                if structured_output_settings.output_type == LlmStructuredOutputType.function_calling or structured_output_settings.output_type == LlmStructuredOutputType.parallel_function_calling:
-                    if structured_output_settings.add_thoughts_and_reasoning_field and self.provider.is_using_json_schema_constraints():
-                        messages[0][
-                            "content"] += function_calling_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(
-                            provider=self.provider)
-                    elif not structured_output_settings.add_thoughts_and_reasoning_field and self.provider.is_using_json_schema_constraints():
-                        messages[0][
-                            "content"] += function_calling_without_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(
-                            provider=self.provider)
-                    elif structured_output_settings.add_thoughts_and_reasoning_field and not self.provider.is_using_json_schema_constraints():
-                        messages[0][
-                            "content"] += function_calling_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(
-                            provider=self.provider)
-                    elif not structured_output_settings.add_thoughts_and_reasoning_field and not self.provider.is_using_json_schema_constraints():
-                        messages[0][
-                            "content"] += function_calling_without_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(
-                            provider=self.provider)
-                elif structured_output_settings.output_type == LlmStructuredOutputType.object_instance or structured_output_settings.output_type == LlmStructuredOutputType.list_of_objects:
-                    if structured_output_settings.add_thoughts_and_reasoning_field and self.provider.is_using_json_schema_constraints():
-                        messages[0][
-                            "content"] += structured_output_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(
-                            provider=self.provider)
-                    elif not structured_output_settings.add_thoughts_and_reasoning_field and self.provider.is_using_json_schema_constraints():
-                        messages[0][
-                            "content"] += structured_output_without_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(
-                            provider=self.provider)
-                    elif structured_output_settings.add_thoughts_and_reasoning_field and not self.provider.is_using_json_schema_constraints():
-                        messages[0][
-                            "content"] += structured_output_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(
-                            provider=self.provider)
-                    elif not structured_output_settings.add_thoughts_and_reasoning_field and not self.provider.is_using_json_schema_constraints():
-                        messages[0][
-                            "content"] += structured_output_without_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(
-                            provider=self.provider)
-
-        prompt, response_role = self.messages_formatter.format_conversation(
-            messages, Roles.assistant
-        )
-
-        if prompt_suffix:
-            prompt += prompt_suffix
-        prompt += additional_suffix
-        if self.debug_output:
-            print(prompt, end="")
-
-        return (
-            self.provider.create_completion(
-                prompt,
-                structured_output_settings,
-                llm_sampling_settings,
-                self.messages_formatter.bos_token,
-            ),
-            response_role,
-        )
-
-    @staticmethod
-    def remove_any(text, list_of_strings):
-        for item in list_of_strings:
-            text = text.replace(item, "")
-        return text
+from copy import deepcopy
+from dataclasses import dataclass
+from typing import List, Literal, Callable, Union, Generator, Any
+
+from pydantic import BaseModel
+
+from .chat_history.basic_chat_history import BasicChatHistory
+from .chat_history.chat_history_base import ChatHistory
+from .chat_history.messages import Roles
+
+from .llm_output_settings import LlmStructuredOutputSettings, LlmStructuredOutputType
+
+from .messages_formatter import (
+    MessagesFormatterType,
+    get_predefined_messages_formatter,
+    MessagesFormatter,
+)
+from .prompt_templates import function_calling_thoughts_and_reasoning, \
+    function_calling_thoughts_and_reasoning_json_schema, function_calling_without_thoughts_and_reasoning_json_schema, \
+    function_calling_without_thoughts_and_reasoning, structured_output_thoughts_and_reasoning_json_schema, \
+    structured_output_without_thoughts_and_reasoning_json_schema, structured_output_thoughts_and_reasoning, \
+    structured_output_without_thoughts_and_reasoning
+
+from .providers.provider_base import LlmProvider, LlmSamplingSettings
+
+
+@dataclass
+class StreamingResponse:
+    """
+    Represents a streaming response with text and an indicator for the last response.
+    """
+
+    text: str
+    is_last_response: bool
+
+    def __init__(self, text: str, is_last_response: bool):
+        """
+        Initializes a new StreamingResponse object.
+
+        Args:
+            text (str): The text content of the streaming response.
+            is_last_response (bool): Indicates whether this is the last response in the stream.
+        """
+        self.text = text
+        self.is_last_response = is_last_response
+
+
+class LlamaCppAgent:
+    """
+    A base agent that can be used for chat, structured output and function calling.
+    """
+
+    def __init__(
+            self,
+            provider: LlmProvider,
+            name: str = "llamacpp_agent",
+            system_prompt: str = "You are a helpful assistant.",
+            predefined_messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
+            custom_messages_formatter: MessagesFormatter = None,
+            chat_history: ChatHistory = None,
+            add_tools_and_structures_documentation_to_system_prompt: bool = True,
+            debug_output: bool = False,
+    ):
+        """
+        Initializes a new LlamaCppAgent object.
+
+        Args:
+           provider (LlmProvider):The underlying llm provider (LlamaCppServerProvider, LlamaCppPythonProvider, TGIServerProvider or VLLMServerProvider).
+           name (str): The name of the agent.
+           system_prompt (str): The system prompt used in chat interactions.
+           predefined_messages_formatter_type (MessagesFormatterType): The type of predefined messages formatter.
+           custom_messages_formatter (MessagesFormatter): Custom message's formatter.
+           chat_history (ChatHistory): This will handle the chat history.
+           add_tools_and_structures_documentation_to_system_prompt (bool): Will suffix system prompt dynamically with documentation for function calling or structured output.
+           debug_output (bool): Indicates whether debug output should be enabled.
+        """
+        self.provider = provider
+        self.name = name
+        self.debug_output = debug_output
+        if custom_messages_formatter is not None:
+            self.messages_formatter = custom_messages_formatter
+        else:
+            self.messages_formatter = get_predefined_messages_formatter(
+                predefined_messages_formatter_type
+            )
+        self.last_response = ""
+        if chat_history is None:
+            self.chat_history = BasicChatHistory()
+        else:
+            self.chat_history = chat_history
+
+        self.add_message(role=Roles.system, message=system_prompt)
+        self.system_prompt = system_prompt
+        self.add_tools_and_structures_documentation_to_system_prompt = add_tools_and_structures_documentation_to_system_prompt
+
+    def add_message(
+            self,
+            message: str,
+            role: Roles,
+    ):
+        """
+        Adds a message to the chat history.
+
+        Args:
+            message (str): The content of the message.
+            role (Literal["system"] | Literal["user"] | Literal["assistant"] | Literal["tool"]): The role of the message sender.
+        """
+        self.chat_history.add_message(
+            {
+                "role": role,
+                "content": message,
+            }
+        )
+
+    def get_text_response(
+            self,
+            prompt: str = None,
+            structured_output_settings: LlmStructuredOutputSettings = None,
+            llm_sampling_settings: LlmSamplingSettings = None,
+            streaming_callback: Callable[[StreamingResponse], None] = None,
+            returns_streaming_generator: bool = False,
+            print_output: bool = False,
+    ) -> Union[
+        str,
+        List[dict],
+        BaseModel,
+        Generator[Any, Any, str | BaseModel | list[BaseModel]],
+    ]:
+        """
+        Get a text response from the LLM provider.
+
+        Args:
+            prompt (str | list[int]): The prompt for the LLM.
+            structured_output_settings (LlmStructuredOutputSettings): Settings for structured output.
+            llm_sampling_settings (LlmSamplingSettings): Sampling settings for the LLM.
+            streaming_callback (Callable[[StreamingResponse], None]): Callback for streaming responses.
+            returns_streaming_generator (bool): Whether to return a generator streaming the results.
+            print_output (bool): Whether to print the output.
+
+        Returns:
+            Union[str, List[dict], BaseModel, Generator[Any, Any, str | BaseModel | list[BaseModel]]: The generated response. A string message, a list of function calls, an object from structured output or a generator for the response
+        """
+
+        if self.debug_output:
+            if type(prompt) is str:
+                print(prompt, end="")
+
+        if structured_output_settings is None:
+            structured_output_settings = LlmStructuredOutputSettings(
+                output_type=LlmStructuredOutputType.no_structured_output
+            )
+        if llm_sampling_settings is None:
+            llm_sampling_settings = self.provider.get_provider_default_settings()
+        else:
+            llm_sampling_settings = deepcopy(llm_sampling_settings)
+
+        if llm_sampling_settings.get_additional_stop_sequences() is not None:
+            llm_sampling_settings.add_additional_stop_sequences(
+                self.messages_formatter.default_stop_sequences
+            )
+
+        if self.provider:
+            completion = self.get_text_completion(
+                prompt=prompt,
+                structured_output_settings=structured_output_settings,
+                llm_samplings_settings=llm_sampling_settings,
+            )
+
+            def stream_results():
+                full_response_stream = ""
+                for out_stream in completion:
+                    out_text = out_stream["choices"][0]["text"]
+                    full_response_stream += text
+                    yield out_text
+                return structured_output_settings.handle_structured_output(
+                    full_response_stream
+                )
+
+            if llm_sampling_settings.is_streaming():
+                full_response = ""
+                if returns_streaming_generator:
+                    return stream_results()
+                for out in completion:
+                    text = out["choices"][0]["text"]
+                    full_response += text
+                    if streaming_callback is not None:
+                        streaming_callback(
+                            StreamingResponse(text=text, is_last_response=False)
+                        )
+                    if print_output:
+                        print(text, end="")
+                if streaming_callback is not None:
+                    streaming_callback(
+                        StreamingResponse(text="", is_last_response=True)
+                    )
+                if print_output or self.debug_output:
+                    print("")
+                self.last_response = full_response
+                return structured_output_settings.handle_structured_output(
+                    full_response
+                )
+            else:
+                full_response = ""
+                text = completion["choices"][0]["text"]
+                full_response += text
+                if print_output or self.debug_output:
+                    print(full_response)
+                self.last_response = full_response
+                return structured_output_settings.handle_structured_output(
+                    full_response
+                )
+        return "Error: No model loaded!"
+
+    def get_chat_response(
+            self,
+            message: str = None,
+            role: Roles = Roles.user,
+            prompt_suffix: str = None,
+            chat_history: ChatHistory = None,
+            system_prompt: str = None,
+            add_message_to_chat_history: bool = True,
+            add_response_to_chat_history: bool = True,
+            structured_output_settings: LlmStructuredOutputSettings = None,
+            llm_sampling_settings: LlmSamplingSettings = None,
+            streaming_callback: Callable[[StreamingResponse], None] = None,
+            returns_streaming_generator: bool = False,
+            print_output: bool = False,
+    ) -> Union[
+        str,
+        List[dict],
+        BaseModel,
+        Generator[Any, Any, str | BaseModel | list[BaseModel]],
+    ]:
+        """
+        Get a chat response based on the input message and context.
+
+        Args:
+            message (str): The input message.
+            role (Literal["system", "user", "assistant", "tool"]): The role of the message sender.
+            prompt_suffix (str): Suffix to append after the prompt.
+            chat_history (ChatHistory): Overwrite internal ChatHistory of the agent.
+            system_prompt (str): Overwrites the system prompt set on the agent initialization.
+            add_message_to_chat_history (bool): Whether to add the input message to the chat history.
+            add_response_to_chat_history (bool): Whether to add the generated response to the chat history.
+            structured_output_settings (LlmStructuredOutputSettings): Settings for structured output.
+            llm_sampling_settings (LlmSamplingSettings): Sampling settings for the LLM.
+            streaming_callback (Callable[[StreamingResponse], None]): Callback for streaming responses.
+            returns_streaming_generator (bool): Whether to return a generator streaming the results.
+            print_output (bool): Whether to print the generated response.
+
+        Returns:
+            Union[str, List[dict], BaseModel, Generator[Any, Any, str | BaseModel | list[BaseModel]]: The generated chat response. A string message, a list of function calls, an object from structured output or a generator for the response
+        """
+        if chat_history is None:
+            chat_history = self.chat_history
+
+        if structured_output_settings is None:
+            structured_output_settings = LlmStructuredOutputSettings(
+                output_type=LlmStructuredOutputType.no_structured_output
+            )
+        if llm_sampling_settings is None:
+            llm_sampling_settings = self.provider.get_provider_default_settings()
+        else:
+            llm_sampling_settings = deepcopy(llm_sampling_settings)
+
+        if llm_sampling_settings.get_additional_stop_sequences() is not None:
+            llm_sampling_settings.add_additional_stop_sequences(
+                self.messages_formatter.default_stop_sequences
+            )
+
+        completion, response_role = self.get_response_role_and_completion(
+            message=message,
+            chat_history=chat_history,
+            system_prompt=system_prompt,
+            add_message_to_chat_history=add_message_to_chat_history,
+            role=role,
+            prompt_suffix=prompt_suffix,
+            structured_output_settings=structured_output_settings,
+            llm_sampling_settings=llm_sampling_settings,
+        )
+
+        def stream_results():
+            full_response_stream = ""
+            for out_stream in completion:
+                out_text = out_stream["choices"][0]["text"]
+                if out_text != self.messages_formatter.eos_token:
+                    full_response_stream += text
+                    yield out_text
+            self.last_response = full_response
+            if add_response_to_chat_history:
+                chat_history.add_message(
+                    {
+                        "role": response_role,
+                        "content": full_response,
+                    }
+                )
+            return structured_output_settings.handle_structured_output(
+                full_response_stream
+            )
+
+        if self.provider:
+            if returns_streaming_generator:
+                return stream_results()
+            if llm_sampling_settings.is_streaming():
+                full_response = ""
+                for out in completion:
+                    text = out["choices"][0]["text"]
+                    if text != self.messages_formatter.eos_token:
+                        full_response += text
+                        if streaming_callback is not None:
+                            streaming_callback(
+                                StreamingResponse(text=text, is_last_response=False)
+                            )
+                        if print_output or self.debug_output:
+                            print(text, end="")
+                if streaming_callback is not None:
+                    streaming_callback(
+                        StreamingResponse(text="", is_last_response=True)
+                    )
+                if print_output or self.debug_output:
+                    print("")
+                self.last_response = full_response
+                if add_response_to_chat_history:
+                    chat_history.add_message(
+                        {
+                            "role": response_role,
+                            "content": full_response,
+                        }
+                    )
+
+                return structured_output_settings.handle_structured_output(
+                    full_response
+                )
+            else:
+                text = completion["choices"][0]["text"]
+                if text.strip().endswith(self.messages_formatter.eos_token):
+                    text = text.replace(self.messages_formatter.eos_token, "")
+                if print_output or self.debug_output:
+                    print(text)
+                self.last_response = text
+                if add_response_to_chat_history:
+                    chat_history.add_message(
+                        {
+                            "role": response_role,
+                            "content": text,
+                        }
+                    )
+
+                return structured_output_settings.handle_structured_output(text)
+        return "Error: No model loaded!"
+
+    def get_text_completion(
+            self,
+            prompt: str | list[int] = None,
+            structured_output_settings: LlmStructuredOutputSettings = None,
+            llm_samplings_settings: LlmSamplingSettings = None,
+    ):
+        return self.provider.create_completion(
+            prompt,
+            structured_output_settings,
+            llm_samplings_settings,
+            self.messages_formatter.bos_token,
+        )
+
+    def get_response_role_and_completion(
+            self,
+            message: str = None,
+            chat_history: ChatHistory = None,
+            system_prompt: str = None,
+            add_message_to_chat_history: bool = True,
+            role: Roles = Roles.user,
+            prompt_suffix: str = None,
+            llm_sampling_settings: LlmSamplingSettings = None,
+            structured_output_settings: LlmStructuredOutputSettings = None,
+    ):
+        if message is not None and add_message_to_chat_history:
+            chat_history.add_message(
+                {
+                    "role": role,
+                    "content": message,
+                }
+            )
+
+        messages = chat_history.get_chat_messages()
+        if message is not None and not add_message_to_chat_history:
+            messages.append(
+                {
+                    "role": role,
+                    "content": message,
+                },
+            )
+        if system_prompt:
+            messages[0]["content"] = system_prompt
+        else:
+            messages[0]["content"] = self.system_prompt
+        additional_suffix = ""
+        if self.add_tools_and_structures_documentation_to_system_prompt:
+            if structured_output_settings.output_type != LlmStructuredOutputType.no_structured_output:
+                additional_suffix = "\n"
+                if structured_output_settings.output_type == LlmStructuredOutputType.function_calling or structured_output_settings.output_type == LlmStructuredOutputType.parallel_function_calling:
+                    if structured_output_settings.add_thoughts_and_reasoning_field and self.provider.is_using_json_schema_constraints():
+                        messages[0][
+                            "content"] += function_calling_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
+                    elif not structured_output_settings.add_thoughts_and_reasoning_field and self.provider.is_using_json_schema_constraints():
+                        messages[0][
+                            "content"] += function_calling_without_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
+                    elif structured_output_settings.add_thoughts_and_reasoning_field and not self.provider.is_using_json_schema_constraints():
+                        messages[0][
+                            "content"] += function_calling_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
+                    elif not structured_output_settings.add_thoughts_and_reasoning_field and not self.provider.is_using_json_schema_constraints():
+                        messages[0][
+                            "content"] += function_calling_without_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
+                elif structured_output_settings.output_type == LlmStructuredOutputType.object_instance or structured_output_settings.output_type == LlmStructuredOutputType.list_of_objects:
+                    if structured_output_settings.add_thoughts_and_reasoning_field and self.provider.is_using_json_schema_constraints():
+                        messages[0][
+                            "content"] += structured_output_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
+                    elif not structured_output_settings.add_thoughts_and_reasoning_field and self.provider.is_using_json_schema_constraints():
+                        messages[0][
+                            "content"] += structured_output_without_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
+                    elif structured_output_settings.add_thoughts_and_reasoning_field and not self.provider.is_using_json_schema_constraints():
+                        messages[0][
+                            "content"] += structured_output_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
+                    elif not structured_output_settings.add_thoughts_and_reasoning_field and not self.provider.is_using_json_schema_constraints():
+                        messages[0][
+                            "content"] += structured_output_without_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
+
+        prompt, response_role = self.messages_formatter.format_conversation(
+            messages, Roles.assistant
+        )
+
+        if prompt_suffix:
+            prompt += prompt_suffix
+        prompt += additional_suffix
+        if self.debug_output:
+            print(prompt, end="")
+
+        return (
+            self.provider.create_completion(
+                prompt,
+                structured_output_settings,
+                llm_sampling_settings,
+                self.messages_formatter.bos_token,
+            ),
+            response_role,
+        )
+
+    @staticmethod
+    def remove_any(text, list_of_strings):
+        for item in list_of_strings:
+            text = text.replace(item, "")
+        return text
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_documentation/documentation_generation.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/llm_documentation/documentation_generation.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,472 +1,472 @@
-import json
-from enum import Enum
-from inspect import isclass, getdoc
-from types import UnionType, GenericAlias
-from typing import get_args, get_origin, Union, Any
-
-from pydantic import BaseModel
-
-
-def generate_markdown_documentation(
-    pydantic_models: list[type[BaseModel]],
-    model_prefix="Model",
-    fields_prefix="Fields",
-    documentation_with_field_description=True,
-) -> str:
-    """
-    Generate markdown documentation for a list of Pydantic models.
-
-    Args:
-        pydantic_models (list[type[BaseModel]]): list of Pydantic model classes.
-        model_prefix (str): Prefix for the model section.
-        fields_prefix (str): Prefix for the fields section.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-
-    Returns:
-        str: Generated text documentation.
-    """
-    documentation = "## Functions\n\n"
-    pyd_models = [(model, True) for model in pydantic_models]
-    for model, add_prefix in pyd_models:
-        if add_prefix:
-            documentation += f"### {model_prefix}: {model.__name__}\n"
-        else:
-            documentation += f"### {model.__name__}\n"
-
-        # Handling multi-line model description with proper indentation
-
-        class_doc = getdoc(model)
-        base_class_doc = getdoc(BaseModel)
-        class_description = (
-            class_doc if class_doc and class_doc != base_class_doc else ""
-        )
-        if class_description != "":
-            documentation += format_multiline_description(class_description, 0) + "\n"
-
-        if add_prefix:
-            # Indenting the fields section
-            documentation += f"{fields_prefix}:\n"
-        else:
-            documentation += f"Fields:\n"
-        if isclass(model) and issubclass(model, BaseModel):
-            for name, field_type in model.__annotations__.items():
-                # if name == "markdown_code_block":
-                #    continue
-                if get_origin(field_type) == list:
-                    element_type = get_args(field_type)[0]
-                    if isclass(element_type) and issubclass(element_type, BaseModel):
-                        pyd_models.append((element_type, False))
-                if get_origin(field_type) == Union:
-                    element_types = get_args(field_type)
-                    for element_type in element_types:
-                        if isclass(element_type) and issubclass(
-                            element_type, BaseModel
-                        ):
-                            pyd_models.append((element_type, False))
-                documentation += generate_field_markdown(
-                    name,
-                    field_type,
-                    model,
-                    documentation_with_field_description=documentation_with_field_description,
-                )
-            if add_prefix:
-                if documentation.endswith(f"{fields_prefix}:\n"):
-                    documentation += "none\n"
-            else:
-                if documentation.endswith("Fields:\n"):
-                    documentation += "none\n"
-            documentation += "\n"
-
-        if (
-            hasattr(model, "Config")
-            and hasattr(model.Config, "json_schema_extra")
-            and "example" in model.Config.json_schema_extra
-        ):
-            documentation += f"  Expected Example Output for {model.__name__}:\n"
-            json_example = json.dumps(model.Config.json_schema_extra["example"])
-            documentation += format_multiline_description(json_example, 2) + "\n"
-
-    return documentation
-
-
-def generate_field_markdown(
-    field_name: str,
-    field_type: type[Any],
-    model: type[BaseModel],
-    depth=1,
-    documentation_with_field_description=True,
-) -> str:
-    """
-    Generate markdown documentation for a Pydantic model field.
-
-    Args:
-        field_name (str): Name of the field.
-        field_type (type[Any]): Type of the field.
-        model (type[BaseModel]): Pydantic model class.
-        depth (int): Indentation depth in the documentation.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-
-    Returns:
-        str: Generated text documentation for the field.
-    """
-    indent = "  " * depth
-
-    field_info = model.model_fields.get(field_name)
-    field_description = (
-        field_info.description if field_info and field_info.description else ""
-    )
-
-    if get_origin(field_type) == list:
-        element_type = get_args(field_type)[0]
-        field_text = (
-            f"{indent}{field_name} ({field_type.__name__} of {element_type.__name__})"
-        )
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-    elif get_origin(field_type) == Union or isinstance(field_type, UnionType):
-        element_types = get_args(field_type)
-        types = []
-        for element_type in element_types:
-            if element_type.__name__ == "NoneType":
-                types.append("null")
-            else:
-                types.append(element_type.__name__)
-        field_text = f"{indent}{field_name} ({' or '.join(types)})"
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-
-    elif issubclass(field_type, Enum):
-        enum_values = [f"'{str(member.value)}'" for member in field_type]
-
-        field_text = f"{indent}{field_name} ({' or '.join(enum_values)})"
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-
-    else:
-        field_text = f"{indent}{field_name} ({field_type.__name__})"
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-
-    if not documentation_with_field_description:
-        return field_text
-
-    if field_description != "":
-        field_text += field_description + "\n"
-
-    # Check for and include field-specific examples if available
-    if (
-        hasattr(model, "Config")
-        and hasattr(model.Config, "json_schema_extra")
-        and "example" in model.Config.json_schema_extra
-    ):
-        field_example = model.Config.json_schema_extra["example"].get(field_name)
-        if field_example is not None:
-            example_text = (
-                f"'{field_example}'"
-                if isinstance(field_example, str)
-                else field_example
-            )
-            field_text += f"{indent}  Example: {example_text}\n"
-
-    if isclass(field_type) and issubclass(field_type, BaseModel):
-        field_text += f"{indent}  Details:\n"
-        for name, type_ in field_type.__annotations__.items():
-            field_text += generate_field_markdown(name, type_, field_type, depth + 2)
-
-    return field_text
-
-
-def format_json_example(example: dict[str, Any], depth: int) -> str:
-    """
-    Format a JSON example into a readable string with indentation.
-
-    Args:
-        example (dict): JSON example to be formatted.
-        depth (int): Indentation depth.
-
-    Returns:
-        str: Formatted JSON example string.
-    """
-    indent = "    " * depth
-    formatted_example = "{\n"
-    for key, value in example.items():
-        value_text = f"'{value}'" if isinstance(value, str) else value
-        formatted_example += f"{indent}{key}: {value_text},\n"
-    formatted_example = formatted_example.rstrip(",\n") + "\n" + indent + "}"
-    return formatted_example
-
-
-def generate_text_documentation(
-    pydantic_models: list[BaseModel],
-    model_prefix="Output Model",
-    fields_prefix="Fields",
-    documentation_with_field_description=True,
-    ordered_json_mode=False,
-) -> str:
-    """
-    Generate markdown documentation for a list of Pydantic models.
-
-    Args:
-        pydantic_models (list[type[BaseModel]]): list of Pydantic model classes.
-        model_prefix (str): Prefix for the model section.
-        fields_prefix (str): Prefix for the fields section.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-        ordered_json_mode (bool): Add ordering prefix for JSON schemas
-    Returns:
-        str: Generated text documentation.
-    """
-    documentation = ""
-    pyd_models = [(model, True) for model in pydantic_models]
-    for model, add_prefix in pyd_models:
-        if add_prefix:
-            documentation += f"{model_prefix}: {model.__name__}\n"
-        else:
-            documentation += f"Model: {model.__name__}\n"
-
-        # Handling multi-line model description with proper indentation
-
-        class_doc = getdoc(model)
-        base_class_doc = getdoc(BaseModel)
-        class_description = (
-            class_doc if class_doc and class_doc != base_class_doc else ""
-        )
-        if class_description != "":
-            documentation += "  Description: "
-            documentation += format_multiline_description(class_description, 2) + "\n"
-
-        if add_prefix:
-            # Indenting the fields section
-            documentation += f"  {fields_prefix}:\n"
-        else:
-            documentation += f"  Fields:\n"
-        if isclass(model) and issubclass(model, BaseModel):
-            count = 1
-            for name, field_type in model.__annotations__.items():
-                # if name == "markdown_code_block":
-                #    continue
-                if get_origin(field_type) == list:
-                    element_type = get_args(field_type)[0]
-                    if isclass(element_type) and issubclass(element_type, BaseModel):
-                        pyd_models.append((element_type, False))
-                    if get_origin(element_type) == Union or isinstance(
-                        element_type, UnionType
-                    ):
-                        element_types = get_args(element_type)
-                        for element_type in element_types:
-                            if isclass(element_type) and issubclass(
-                                element_type, BaseModel
-                            ):
-                                pyd_models.append((element_type, False))
-                            if get_origin(element_type) == list:
-                                element_type = get_args(element_type)[0]
-                                if isclass(element_type) and issubclass(
-                                    element_type, BaseModel
-                                ):
-                                    pyd_models.append((element_type, False))
-                if get_origin(field_type) == Union or isinstance(field_type, UnionType):
-                    element_types = get_args(field_type)
-                    for element_type in element_types:
-                        if isclass(element_type) and issubclass(
-                            element_type, BaseModel
-                        ):
-                            pyd_models.append((element_type, False))
-                        if get_origin(element_type) == list:
-                            element_type = get_args(element_type)[0]
-                            if isclass(element_type) and issubclass(
-                                element_type, BaseModel
-                            ):
-                                pyd_models.append((element_type, False))
-                if isclass(field_type) and issubclass(field_type, BaseModel):
-                    pyd_models.append((field_type, False))
-                documentation += generate_field_text(
-                    name
-                    if not ordered_json_mode
-                    else "{:03}".format(count) + "_" + name,
-                    field_type,
-                    model,
-                    documentation_with_field_description=documentation_with_field_description,
-                )
-                count += 1
-            if add_prefix:
-                if documentation.endswith(f"{fields_prefix}:\n"):
-                    documentation += "    none\n"
-            else:
-                if documentation.endswith("fields:\n"):
-                    documentation += "    none\n"
-            documentation += "\n"
-
-        if (
-            hasattr(model, "Config")
-            and hasattr(model.Config, "json_schema_extra")
-            and "example" in model.Config.json_schema_extra
-        ):
-            documentation += f"  Expected Example Output for {model.__name__}:\n"
-            json_example = json.dumps(model.Config.json_schema_extra["example"])
-            documentation += format_multiline_description(json_example, 2) + "\n"
-
-    return documentation
-
-
-def generate_field_text(
-    field_name: str,
-    field_type: type[Any],
-    model: type[BaseModel],
-    depth=1,
-    documentation_with_field_description=True,
-) -> str:
-    """
-    Generate markdown documentation for a Pydantic model field.
-
-    Args:
-        field_name (str): Name of the field.
-        field_type (type[Any]): Type of the field.
-        model (type[BaseModel]): Pydantic model class.
-        depth (int): Indentation depth in the documentation.
-        documentation_with_field_description (bool): Include field descriptions in the documentation.
-
-    Returns:
-        str: Generated text documentation for the field.
-    """
-    indent = "    " * depth
-
-    field_info = model.model_fields.get(field_name)
-    field_description = (
-        field_info.description if field_info and field_info.description else ""
-    )
-    field_text = ""
-    if get_origin(field_type) == list:
-        element_type = get_args(field_type)[0]
-        if get_origin(element_type) == Union or isinstance(element_type, UnionType):
-            element_types = get_args(element_type)
-            types = []
-            for element_type in element_types:
-                if element_type.__name__ == "NoneType":
-                    types.append("null")
-                else:
-                    if isclass(element_type) and issubclass(element_type, Enum):
-                        enum_values = [
-                            f"'{str(member.value)}'" for member in element_type
-                        ]
-                        for enum_value in enum_values:
-                            types.append(enum_value)
-
-                    else:
-                        if get_origin(element_type) == list:
-                            element_type = get_args(element_type)[0]
-                            types.append(f"(list of {element_type.__name__})")
-                        else:
-                            types.append(element_type.__name__)
-            field_text = f"({' or '.join(types)})"
-            field_text = f"{indent}{field_name} ({field_type.__name__} of {field_text})"
-            if field_description != "":
-                field_text += ": "
-            else:
-                field_text += "\n"
-        else:
-            field_text = f"{indent}{field_name} ({field_type.__name__} of {element_type.__name__})"
-            if field_description != "":
-                field_text += ": "
-            else:
-                field_text += "\n"
-    elif get_origin(field_type) == Union:
-        element_types = get_args(field_type)
-        types = []
-        for element_type in element_types:
-            if element_type.__name__ == "NoneType":
-                types.append("null")
-            else:
-                if isclass(element_type) and issubclass(element_type, Enum):
-                    enum_values = [f"'{str(member.value)}'" for member in element_type]
-                    for enum_value in enum_values:
-                        types.append(enum_value)
-
-                else:
-                    if get_origin(element_type) == list:
-                        element_type = get_args(element_type)[0]
-                        types.append(f"(list of {element_type.__name__})")
-                    else:
-                        types.append(element_type.__name__)
-        field_text = f"{indent}{field_name} ({' or '.join(types)})"
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-    elif isinstance(field_type, GenericAlias):
-        if field_type.__origin__ == dict:
-            key_type, value_type = get_args(field_type)
-
-            additional_key_type = key_type.__name__
-            additional_value_type = value_type.__name__
-            field_text = f"{indent}{field_name} (dict of {additional_key_type} to {additional_value_type})"
-            if field_description != "":
-                field_text += ": "
-            else:
-                field_text += "\n"
-        elif field_type.__origin__ == list:
-            element_type = get_args(field_type)[0]
-            field_text = f"{indent}{field_name} (list of {element_type.__name__})"
-            if field_description != "":
-                field_text += ": "
-            else:
-                field_text += "\n"
-    elif issubclass(field_type, Enum):
-        enum_values = [f"'{str(member.value)}'" for member in field_type]
-
-        field_text = f"{indent}{field_name} ({' or '.join(enum_values)})"
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-
-    else:
-        field_text = f"{indent}{field_name} ({field_type.__name__})"
-        if field_description != "":
-            field_text += ": "
-        else:
-            field_text += "\n"
-
-    if not documentation_with_field_description:
-        return field_text
-
-    if field_description != "":
-        field_text += field_description + "\n"
-
-    # Check for and include field-specific examples if available
-    if (
-        hasattr(model, "Config")
-        and hasattr(model.Config, "json_schema_extra")
-        and "example" in model.Config.json_schema_extra
-    ):
-        field_example = model.Config.json_schema_extra["example"].get(field_name)
-        if field_example is not None:
-            example_text = (
-                f"'{field_example}'"
-                if isinstance(field_example, str)
-                else field_example
-            )
-            field_text += f"{indent}  Example: {example_text}\n"
-
-    return field_text
-
-
-def format_multiline_description(description: str, indent_level: int) -> str:
-    """
-    Format a multiline description with proper indentation.
-
-    Args:
-        description (str): Multiline description.
-        indent_level (int): Indentation level.
-
-    Returns:
-        str: Formatted multiline description.
-    """
-    indent = "  " * indent_level
-    return description.replace("\n", "\n" + indent)
+import json
+from enum import Enum
+from inspect import isclass, getdoc
+from types import UnionType, GenericAlias
+from typing import get_args, get_origin, Union, Any
+
+from pydantic import BaseModel
+
+
+def generate_markdown_documentation(
+    pydantic_models: list[type[BaseModel]],
+    model_prefix="Model",
+    fields_prefix="Fields",
+    documentation_with_field_description=True,
+) -> str:
+    """
+    Generate markdown documentation for a list of Pydantic models.
+
+    Args:
+        pydantic_models (list[type[BaseModel]]): list of Pydantic model classes.
+        model_prefix (str): Prefix for the model section.
+        fields_prefix (str): Prefix for the fields section.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+
+    Returns:
+        str: Generated text documentation.
+    """
+    documentation = "## Functions\n\n"
+    pyd_models = [(model, True) for model in pydantic_models]
+    for model, add_prefix in pyd_models:
+        if add_prefix:
+            documentation += f"### {model_prefix}: {model.__name__}\n"
+        else:
+            documentation += f"### {model.__name__}\n"
+
+        # Handling multi-line model description with proper indentation
+
+        class_doc = getdoc(model)
+        base_class_doc = getdoc(BaseModel)
+        class_description = (
+            class_doc if class_doc and class_doc != base_class_doc else ""
+        )
+        if class_description != "":
+            documentation += format_multiline_description(class_description, 0) + "\n"
+
+        if add_prefix:
+            # Indenting the fields section
+            documentation += f"{fields_prefix}:\n"
+        else:
+            documentation += f"Fields:\n"
+        if isclass(model) and issubclass(model, BaseModel):
+            for name, field_type in model.__annotations__.items():
+                # if name == "markdown_code_block":
+                #    continue
+                if get_origin(field_type) == list:
+                    element_type = get_args(field_type)[0]
+                    if isclass(element_type) and issubclass(element_type, BaseModel):
+                        pyd_models.append((element_type, False))
+                if get_origin(field_type) == Union:
+                    element_types = get_args(field_type)
+                    for element_type in element_types:
+                        if isclass(element_type) and issubclass(
+                            element_type, BaseModel
+                        ):
+                            pyd_models.append((element_type, False))
+                documentation += generate_field_markdown(
+                    name,
+                    field_type,
+                    model,
+                    documentation_with_field_description=documentation_with_field_description,
+                )
+            if add_prefix:
+                if documentation.endswith(f"{fields_prefix}:\n"):
+                    documentation += "none\n"
+            else:
+                if documentation.endswith("Fields:\n"):
+                    documentation += "none\n"
+            documentation += "\n"
+
+        if (
+            hasattr(model, "Config")
+            and hasattr(model.Config, "json_schema_extra")
+            and "example" in model.Config.json_schema_extra
+        ):
+            documentation += f"  Expected Example Output for {model.__name__}:\n"
+            json_example = json.dumps(model.Config.json_schema_extra["example"])
+            documentation += format_multiline_description(json_example, 2) + "\n"
+
+    return documentation
+
+
+def generate_field_markdown(
+    field_name: str,
+    field_type: type[Any],
+    model: type[BaseModel],
+    depth=1,
+    documentation_with_field_description=True,
+) -> str:
+    """
+    Generate markdown documentation for a Pydantic model field.
+
+    Args:
+        field_name (str): Name of the field.
+        field_type (type[Any]): Type of the field.
+        model (type[BaseModel]): Pydantic model class.
+        depth (int): Indentation depth in the documentation.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+
+    Returns:
+        str: Generated text documentation for the field.
+    """
+    indent = "  " * depth
+
+    field_info = model.model_fields.get(field_name)
+    field_description = (
+        field_info.description if field_info and field_info.description else ""
+    )
+
+    if get_origin(field_type) == list:
+        element_type = get_args(field_type)[0]
+        field_text = (
+            f"{indent}{field_name} ({field_type.__name__} of {element_type.__name__})"
+        )
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+    elif get_origin(field_type) == Union or isinstance(field_type, UnionType):
+        element_types = get_args(field_type)
+        types = []
+        for element_type in element_types:
+            if element_type.__name__ == "NoneType":
+                types.append("null")
+            else:
+                types.append(element_type.__name__)
+        field_text = f"{indent}{field_name} ({' or '.join(types)})"
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+
+    elif issubclass(field_type, Enum):
+        enum_values = [f"'{str(member.value)}'" for member in field_type]
+
+        field_text = f"{indent}{field_name} ({' or '.join(enum_values)})"
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+
+    else:
+        field_text = f"{indent}{field_name} ({field_type.__name__})"
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+
+    if not documentation_with_field_description:
+        return field_text
+
+    if field_description != "":
+        field_text += field_description + "\n"
+
+    # Check for and include field-specific examples if available
+    if (
+        hasattr(model, "Config")
+        and hasattr(model.Config, "json_schema_extra")
+        and "example" in model.Config.json_schema_extra
+    ):
+        field_example = model.Config.json_schema_extra["example"].get(field_name)
+        if field_example is not None:
+            example_text = (
+                f"'{field_example}'"
+                if isinstance(field_example, str)
+                else field_example
+            )
+            field_text += f"{indent}  Example: {example_text}\n"
+
+    if isclass(field_type) and issubclass(field_type, BaseModel):
+        field_text += f"{indent}  Details:\n"
+        for name, type_ in field_type.__annotations__.items():
+            field_text += generate_field_markdown(name, type_, field_type, depth + 2)
+
+    return field_text
+
+
+def format_json_example(example: dict[str, Any], depth: int) -> str:
+    """
+    Format a JSON example into a readable string with indentation.
+
+    Args:
+        example (dict): JSON example to be formatted.
+        depth (int): Indentation depth.
+
+    Returns:
+        str: Formatted JSON example string.
+    """
+    indent = "    " * depth
+    formatted_example = "{\n"
+    for key, value in example.items():
+        value_text = f"'{value}'" if isinstance(value, str) else value
+        formatted_example += f"{indent}{key}: {value_text},\n"
+    formatted_example = formatted_example.rstrip(",\n") + "\n" + indent + "}"
+    return formatted_example
+
+
+def generate_text_documentation(
+    pydantic_models: list[BaseModel],
+    model_prefix="Output Model",
+    fields_prefix="Fields",
+    documentation_with_field_description=True,
+    ordered_json_mode=False,
+) -> str:
+    """
+    Generate markdown documentation for a list of Pydantic models.
+
+    Args:
+        pydantic_models (list[type[BaseModel]]): list of Pydantic model classes.
+        model_prefix (str): Prefix for the model section.
+        fields_prefix (str): Prefix for the fields section.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+        ordered_json_mode (bool): Add ordering prefix for JSON schemas
+    Returns:
+        str: Generated text documentation.
+    """
+    documentation = ""
+    pyd_models = [(model, True) for model in pydantic_models]
+    for model, add_prefix in pyd_models:
+        if add_prefix:
+            documentation += f"{model_prefix}: {model.__name__}\n"
+        else:
+            documentation += f"Model: {model.__name__}\n"
+
+        # Handling multi-line model description with proper indentation
+
+        class_doc = getdoc(model)
+        base_class_doc = getdoc(BaseModel)
+        class_description = (
+            class_doc if class_doc and class_doc != base_class_doc else ""
+        )
+        if class_description != "":
+            documentation += "  Description: "
+            documentation += format_multiline_description(class_description, 2) + "\n"
+
+        if add_prefix:
+            # Indenting the fields section
+            documentation += f"  {fields_prefix}:\n"
+        else:
+            documentation += f"  Fields:\n"
+        if isclass(model) and issubclass(model, BaseModel):
+            count = 1
+            for name, field_type in model.__annotations__.items():
+                # if name == "markdown_code_block":
+                #    continue
+                if get_origin(field_type) == list:
+                    element_type = get_args(field_type)[0]
+                    if isclass(element_type) and issubclass(element_type, BaseModel):
+                        pyd_models.append((element_type, False))
+                    if get_origin(element_type) == Union or isinstance(
+                        element_type, UnionType
+                    ):
+                        element_types = get_args(element_type)
+                        for element_type in element_types:
+                            if isclass(element_type) and issubclass(
+                                element_type, BaseModel
+                            ):
+                                pyd_models.append((element_type, False))
+                            if get_origin(element_type) == list:
+                                element_type = get_args(element_type)[0]
+                                if isclass(element_type) and issubclass(
+                                    element_type, BaseModel
+                                ):
+                                    pyd_models.append((element_type, False))
+                if get_origin(field_type) == Union or isinstance(field_type, UnionType):
+                    element_types = get_args(field_type)
+                    for element_type in element_types:
+                        if isclass(element_type) and issubclass(
+                            element_type, BaseModel
+                        ):
+                            pyd_models.append((element_type, False))
+                        if get_origin(element_type) == list:
+                            element_type = get_args(element_type)[0]
+                            if isclass(element_type) and issubclass(
+                                element_type, BaseModel
+                            ):
+                                pyd_models.append((element_type, False))
+                if isclass(field_type) and issubclass(field_type, BaseModel):
+                    pyd_models.append((field_type, False))
+                documentation += generate_field_text(
+                    name
+                    if not ordered_json_mode
+                    else "{:03}".format(count) + "_" + name,
+                    field_type,
+                    model,
+                    documentation_with_field_description=documentation_with_field_description,
+                )
+                count += 1
+            if add_prefix:
+                if documentation.endswith(f"{fields_prefix}:\n"):
+                    documentation += "    none\n"
+            else:
+                if documentation.endswith("fields:\n"):
+                    documentation += "    none\n"
+            documentation += "\n"
+
+        if (
+            hasattr(model, "Config")
+            and hasattr(model.Config, "json_schema_extra")
+            and "example" in model.Config.json_schema_extra
+        ):
+            documentation += f"  Expected Example Output for {model.__name__}:\n"
+            json_example = json.dumps(model.Config.json_schema_extra["example"])
+            documentation += format_multiline_description(json_example, 2) + "\n"
+
+    return documentation
+
+
+def generate_field_text(
+    field_name: str,
+    field_type: type[Any],
+    model: type[BaseModel],
+    depth=1,
+    documentation_with_field_description=True,
+) -> str:
+    """
+    Generate markdown documentation for a Pydantic model field.
+
+    Args:
+        field_name (str): Name of the field.
+        field_type (type[Any]): Type of the field.
+        model (type[BaseModel]): Pydantic model class.
+        depth (int): Indentation depth in the documentation.
+        documentation_with_field_description (bool): Include field descriptions in the documentation.
+
+    Returns:
+        str: Generated text documentation for the field.
+    """
+    indent = "    " * depth
+
+    field_info = model.model_fields.get(field_name)
+    field_description = (
+        field_info.description if field_info and field_info.description else ""
+    )
+    field_text = ""
+    if get_origin(field_type) == list:
+        element_type = get_args(field_type)[0]
+        if get_origin(element_type) == Union or isinstance(element_type, UnionType):
+            element_types = get_args(element_type)
+            types = []
+            for element_type in element_types:
+                if element_type.__name__ == "NoneType":
+                    types.append("null")
+                else:
+                    if isclass(element_type) and issubclass(element_type, Enum):
+                        enum_values = [
+                            f"'{str(member.value)}'" for member in element_type
+                        ]
+                        for enum_value in enum_values:
+                            types.append(enum_value)
+
+                    else:
+                        if get_origin(element_type) == list:
+                            element_type = get_args(element_type)[0]
+                            types.append(f"(list of {element_type.__name__})")
+                        else:
+                            types.append(element_type.__name__)
+            field_text = f"({' or '.join(types)})"
+            field_text = f"{indent}{field_name} ({field_type.__name__} of {field_text})"
+            if field_description != "":
+                field_text += ": "
+            else:
+                field_text += "\n"
+        else:
+            field_text = f"{indent}{field_name} ({field_type.__name__} of {element_type.__name__})"
+            if field_description != "":
+                field_text += ": "
+            else:
+                field_text += "\n"
+    elif get_origin(field_type) == Union:
+        element_types = get_args(field_type)
+        types = []
+        for element_type in element_types:
+            if element_type.__name__ == "NoneType":
+                types.append("null")
+            else:
+                if isclass(element_type) and issubclass(element_type, Enum):
+                    enum_values = [f"'{str(member.value)}'" for member in element_type]
+                    for enum_value in enum_values:
+                        types.append(enum_value)
+
+                else:
+                    if get_origin(element_type) == list:
+                        element_type = get_args(element_type)[0]
+                        types.append(f"(list of {element_type.__name__})")
+                    else:
+                        types.append(element_type.__name__)
+        field_text = f"{indent}{field_name} ({' or '.join(types)})"
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+    elif isinstance(field_type, GenericAlias):
+        if field_type.__origin__ == dict:
+            key_type, value_type = get_args(field_type)
+
+            additional_key_type = key_type.__name__
+            additional_value_type = value_type.__name__
+            field_text = f"{indent}{field_name} (dict of {additional_key_type} to {additional_value_type})"
+            if field_description != "":
+                field_text += ": "
+            else:
+                field_text += "\n"
+        elif field_type.__origin__ == list:
+            element_type = get_args(field_type)[0]
+            field_text = f"{indent}{field_name} (list of {element_type.__name__})"
+            if field_description != "":
+                field_text += ": "
+            else:
+                field_text += "\n"
+    elif issubclass(field_type, Enum):
+        enum_values = [f"'{str(member.value)}'" for member in field_type]
+
+        field_text = f"{indent}{field_name} ({' or '.join(enum_values)})"
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+
+    else:
+        field_text = f"{indent}{field_name} ({field_type.__name__})"
+        if field_description != "":
+            field_text += ": "
+        else:
+            field_text += "\n"
+
+    if not documentation_with_field_description:
+        return field_text
+
+    if field_description != "":
+        field_text += field_description + "\n"
+
+    # Check for and include field-specific examples if available
+    if (
+        hasattr(model, "Config")
+        and hasattr(model.Config, "json_schema_extra")
+        and "example" in model.Config.json_schema_extra
+    ):
+        field_example = model.Config.json_schema_extra["example"].get(field_name)
+        if field_example is not None:
+            example_text = (
+                f"'{field_example}'"
+                if isinstance(field_example, str)
+                else field_example
+            )
+            field_text += f"{indent}  Example: {example_text}\n"
+
+    return field_text
+
+
+def format_multiline_description(description: str, indent_level: int) -> str:
+    """
+    Format a multiline description with proper indentation.
+
+    Args:
+        description (str): Multiline description.
+        indent_level (int): Indentation level.
+
+    Returns:
+        str: Formatted multiline description.
+    """
+    indent = "  " * indent_level
+    return description.replace("\n", "\n" + indent)
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_output_settings/settings.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/llm_output_settings/settings.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,690 +1,690 @@
-import json
-import re
-from enum import Enum
-from typing import Dict, List, Optional, Any, Callable, Tuple, Union
-
-from pydantic import BaseModel, Field
-
-from llama_cpp_agent.function_calling import LlamaCppFunctionTool
-from llama_cpp_agent.gbnf_grammar_generator.gbnf_grammar_from_pydantic_models import (
-    generate_gbnf_grammar_from_pydantic_models,
-)
-from llama_cpp_agent.json_schema_generator.schema_generator import generate_json_schemas
-from llama_cpp_agent.llm_documentation import generate_text_documentation
-from llama_cpp_agent.output_parser import parse_json_response
-
-
-class LlmStructuredOutputType(Enum):
-    """
-    Enum for defining different types of structured outputs that can be generated by a Language Model.
-    """
-
-    no_structured_output = "no_structured_output"
-    object_instance = "object_instance"
-    list_of_objects = "list_of_objects"
-    function_calling = "function_calling"
-    parallel_function_calling = "parallel_function_calling"
-
-
-class LlmStructuredOutputSettings(BaseModel):
-    """
-    Settings for structured output of large language models for using tools like function calling and creating instances of pydantic models.
-
-    Attributes:
-        output_type (LlmStructuredOutputType): Defines the type of structured output.
-        function_tools (Optional[List[LlamaCppFunctionTool]]): Tools to enable function calling.
-        pydantic_models (Optional[List[type[BaseModel]]]): List of pydantic models for structured data output.
-        add_thoughts_and_reasoning_field (Optional[bool]): Add thoughts and reasoning field to function calling. Defaults to False.
-        thoughts_and_reasoning_field_name (Optional[str]): Field name for the thoughts and reasoning field. Defaults to "thoughts_and_reasoning".
-        function_calling_name_field_name (Optional[str]): Name of the JSON field for the name of the used function. Defaults to "function".
-        function_calling_content (Optional[str]): Name of the JSON field for the arguments of the used function. Defaults to "arguments".
-        output_model_name_field_name (Optional[str]): Name of the JSON field for the name of the used pydantic model. Defaults to "model".
-        output_model_attributes_field_name (Optional[str]): Name of the JSON field for the fields of the pydantic model. Defaults to "fields".
-
-    Methods:
-        from_llama_cpp_function_tools: Create settings from a list of LlamaCppFunctionTools with a specific output type.
-        from_pydantic_models: Create settings from a list of Pydantic models with a specific output type.
-        from_open_ai_tools: Create settings from OpenAI tools for structured outputs.
-        from_functions: Create settings from a list of callable functions with a specific output type.
-        from_llama_index_tools: Create settings from a list of llama-index tools with a specific output type.
-        to_openai_tools: Return a list of OpenAI tools.
-        add_llama_cpp_function_tool: Add a LlamaCppFunctionTool to the settings.
-        add_pydantic_model: Add a Pydantic model to the settings, ensuring it matches the specified output type.
-        add_open_ai_tool: Add an OpenAI tool to the settings, ensuring it matches the specified output type.
-        add_function_tool: Add a callable function to the settings, ensuring it matches the specified output type.
-        add_llama_index_tool: Add a llama-index tool, like QueryEngineTool, to the settings, ensuring it matches the specified output type.
-        get_llm_documentation: Generate documentation for the models and tools configured within the settings, based on the output type.
-        get_gbnf_grammar: Generate a GBNF grammar for tools configured within the settings, based on the output type.
-        get_json_schema: Generate a JSON schema for the tools configured within the settings, based on the output type.
-    """
-
-    output_type: Optional[LlmStructuredOutputType] = Field(
-        ..., description="The output type of the llm"
-    )
-    function_tools: Optional[List[LlamaCppFunctionTool]] = Field(
-        None, description="List of functions tools for function calling"
-    )
-    pydantic_models: Optional[List[type[BaseModel]]] = Field(
-        None, description="List of pydantic models for structured output"
-    )
-    add_thoughts_and_reasoning_field: Optional[bool] = Field(
-        False, description="Add thoughts and reasoning field to function calling"
-    )
-
-    thoughts_and_reasoning_field_name: Optional[str] = Field(
-        "thoughts_and_reasoning",
-        description="Field name for the thoughts and reasoning field",
-    )
-
-    function_calling_name_field_name: Optional[str] = Field(
-        "function",
-        description="Name of the JSON field for the name of the used function.",
-    )
-    function_calling_content: Optional[str] = Field(
-        "arguments",
-        description="Name of the JSON field for the arguments of the used function.",
-    )
-
-    output_model_name_field_name: Optional[str] = Field(
-        "model",
-        description="Name of the JSON field for the name of the used pydantic model.",
-    )
-    output_model_attributes_field_name: Optional[str] = Field(
-        "fields",
-        description="Name of the JSON field for the fields of the pydantic model.",
-    )
-
-    output_raw_json_string: Optional[bool] = Field(
-        False,
-        description="If the output should be just the generated JSON string by the LLM",
-    )
-
-    class Config:
-        arbitrary_types_allowed = True
-
-    @staticmethod
-    def from_llama_cpp_function_tools(
-        llama_cpp_function_tools: List[LlamaCppFunctionTool],
-        allow_parallel_function_calling: bool = False,
-    ):
-        """
-        Create settings from a list of LlamaCppFunctionTools with a specific output type.
-
-        Args:
-            llama_cpp_function_tools (List[LlamaCppFunctionTool]): List of function tools.
-            allow_parallel_function_calling (bool): Whether to enable parallel function calling. Defaults to False.
-
-        Returns:
-            LlmStructuredOutputSettings: Configured settings object.
-        """
-        return LlmStructuredOutputSettings(
-            output_type=LlmStructuredOutputType.function_calling
-            if not allow_parallel_function_calling
-            else LlmStructuredOutputType.parallel_function_calling,
-            function_tools=llama_cpp_function_tools,
-        )
-
-    @staticmethod
-    def from_pydantic_models(
-        models: List[type[BaseModel]], output_type: LlmStructuredOutputType
-    ):
-        """
-        Create settings from a list of Pydantic models with a specific output type.
-
-        Args:
-            models (List[BaseModel]): List of Pydantic models.
-            output_type (LlmStructuredOutputType): Desired output type.
-
-        Returns:
-            LlmStructuredOutputSettings: Configured settings object.
-
-        Raises:
-            NotImplementedError: If no structured output is specified for the output type.
-        """
-        if output_type is LlmStructuredOutputType.no_structured_output:
-            raise NotImplementedError(
-                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
-            )
-        elif output_type is LlmStructuredOutputType.object_instance:
-            return LlmStructuredOutputSettings(
-                output_type=LlmStructuredOutputType.object_instance,
-                pydantic_models=models,
-            )
-        elif output_type is LlmStructuredOutputType.list_of_objects:
-            return LlmStructuredOutputSettings(
-                output_type=LlmStructuredOutputType.list_of_objects,
-                pydantic_models=models,
-            )
-        elif output_type is LlmStructuredOutputType.function_calling:
-            return LlmStructuredOutputSettings(
-                output_type=LlmStructuredOutputType.function_calling,
-                function_tools=[LlamaCppFunctionTool(model) for model in models],
-            )
-        elif output_type is LlmStructuredOutputType.parallel_function_calling:
-            return LlmStructuredOutputSettings(
-                output_type=LlmStructuredOutputType.parallel_function_calling,
-                function_tools=[LlamaCppFunctionTool(model) for model in models],
-            )
-
-    @staticmethod
-    def from_open_ai_tools(
-        tools: List[Tuple[Dict[str, Any], Callable]],
-        allow_parallel_function_calling: bool = False,
-    ):
-        """
-        Create settings from OpenAI tools for structured outputs.
-
-        Args:
-            tools (List[Tuple[Dict[str, Any], Callable]]): List of OpenAI tools defined by a schema and associated function.
-            allow_parallel_function_calling (bool): Whether to enable parallel function calling. Defaults to False.
-
-        Returns:
-            LlmStructuredOutputSettings: Configured settings object.
-        """
-        return LlmStructuredOutputSettings(
-            output_type=LlmStructuredOutputType.parallel_function_calling
-            if allow_parallel_function_calling
-            else LlmStructuredOutputType.function_calling,
-            function_tools=[LlamaCppFunctionTool(model) for model in tools],
-        )
-
-    @staticmethod
-    def from_functions(
-        tools: List[Callable], allow_parallel_function_calling: bool = False
-    ):
-        """
-        Create settings from a list of llama-index tools with a specific output type.
-
-        Args:
-            tools (list): List of llama-index tools.
-            allow_parallel_function_calling (bool): Whether to enable parallel function calling. Defaults to False.
-
-        Returns:
-            LlmStructuredOutputSettings: Configured settings object.
-
-        Raises:
-            NotImplementedError: If the specified output type is not supported for tools.
-        """
-        return LlmStructuredOutputSettings(
-            output_type=LlmStructuredOutputType.parallel_function_calling
-            if allow_parallel_function_calling
-            else LlmStructuredOutputType.function_calling,
-            function_tools=[LlamaCppFunctionTool(model) for model in tools],
-        )
-
-    @staticmethod
-    def from_llama_index_tools(
-        tools: list, allow_parallel_function_calling: bool = False
-    ):
-        """
-        Create settings from a list of llama-index tools with a specific output type. Has to be either LlmOutputType.function_call or LlmOutputType.parallel_function_call.
-
-        Args:
-            tools (list): List of llama-index tools.
-            allow_parallel_function_calling (bool): Whether to enable parallel function calling. Defaults to False.
-
-        Returns:
-            LlmStructuredOutputSettings: Configured settings object.
-
-        Raises:
-            NotImplementedError: If the specified output type is not supported for tools.
-        """
-        return LlmStructuredOutputSettings(
-            output_type=LlmStructuredOutputType.parallel_function_calling
-            if allow_parallel_function_calling
-            else LlmStructuredOutputType.function_calling,
-            function_tools=[
-                LlamaCppFunctionTool.from_llama_index_tool(model) for model in tools
-            ],
-        )
-
-    def to_openai_tools(self):
-        """
-        Return a list of OpenAI tools.
-        Returns:
-            List[Dict[str, Any]]: List of OpenAI tools.
-
-        Raises:
-            NotImplementedError: If the specified output type is not supported for tools.
-        """
-        if self.function_tools is not None:
-            return [tool.to_openai_tool() for tool in self.function_tools]
-
-    def add_llama_cpp_function_tool(self, tool: LlamaCppFunctionTool):
-        """
-        Add a LlamaCppFunctionTool to the settings.
-
-        Args:
-            tool (LlamaCppFunctionTool): The function tool to add.
-        """
-        self.function_tools.append(tool)
-
-    def add_pydantic_model(self, model: BaseModel):
-        """
-        Add a Pydantic model to the settings, ensuring it matches the specified output type.
-
-        Args:
-            model (BaseModel): The Pydantic model to add.
-
-        Raises:
-            NotImplementedError: If no structured output is specified.
-        """
-        if self.output_type is LlmStructuredOutputType.no_structured_output:
-            raise NotImplementedError(
-                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
-            )
-        elif self.output_type is LlmStructuredOutputType.object_instance:
-            self.pydantic_models.append(model)
-        elif self.output_type is LlmStructuredOutputType.list_of_objects:
-            self.pydantic_models.append(model)
-        elif self.output_type is LlmStructuredOutputType.function_calling:
-            self.function_tools.append(LlamaCppFunctionTool(model))
-        elif self.output_type is LlmStructuredOutputType.parallel_function_calling:
-            self.function_tools.append(LlamaCppFunctionTool(model))
-
-    def add_open_ai_tool(
-        self, open_ai_schema_and_function: Tuple[Dict[str, Any], Callable]
-    ):
-        """
-        Add an OpenAI tool to the settings, ensuring it matches the specified output type.
-
-        Args:
-            open_ai_schema_and_function (Tuple[Dict[str, Any], Callable]): The OpenAI schema and associated function to add.
-
-        Raises:
-            NotImplementedError: If the output type does not support adding tools.
-        """
-        if self.output_type is LlmStructuredOutputType.no_structured_output:
-            raise NotImplementedError(
-                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
-            )
-        elif self.output_type is LlmStructuredOutputType.function_calling:
-            self.function_tools.append(
-                LlamaCppFunctionTool(open_ai_schema_and_function)
-            )
-        elif self.output_type is LlmStructuredOutputType.parallel_function_calling:
-            self.function_tools.append(
-                LlamaCppFunctionTool(open_ai_schema_and_function)
-            )
-        else:
-            raise NotImplementedError(
-                f"LlmOutputType: {self.output_type.value} not supported for tools!"
-            )
-
-    def add_function_tool(self, function: Callable):
-        """
-        Add a callable function to the settings, ensuring it matches the specified output type.
-
-        Args:
-            function (Callable): The function to add.
-
-        Raises:
-            NotImplementedError: If the output type does not support adding tools.
-        """
-        if self.output_type is LlmStructuredOutputType.no_structured_output:
-            raise NotImplementedError(
-                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
-            )
-        elif self.output_type is LlmStructuredOutputType.function_calling:
-            self.function_tools.append(LlamaCppFunctionTool(function))
-        elif self.output_type is LlmStructuredOutputType.parallel_function_calling:
-            self.function_tools.append(LlamaCppFunctionTool(function))
-        else:
-            raise NotImplementedError(
-                f"LlmOutputType: {self.output_type.value} not supported for tools!"
-            )
-
-    def add_llama_index_tool(self, tool):
-        """
-        Add a llama-index tool, like QueryEngineTool, to the settings, ensuring it matches the specified output type.
-
-        Args:
-            tool: The llama-index tool to add.
-
-        Raises:
-            NotImplementedError: If the output type does not support adding tools.
-        """
-        if self.output_type is LlmStructuredOutputType.no_structured_output:
-            raise NotImplementedError(
-                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
-            )
-        elif self.output_type is LlmStructuredOutputType.function_calling:
-            self.function_tools.append(LlamaCppFunctionTool.from_llama_index_tool(tool))
-        elif self.output_type is LlmStructuredOutputType.parallel_function_calling:
-            self.function_tools.append(LlamaCppFunctionTool.from_llama_index_tool(tool))
-        else:
-            raise NotImplementedError(
-                f"LlmOutputType: {self.output_type.value} not supported for tools!"
-            )
-
-    def get_llm_documentation(self, provider):
-        """
-        Generate documentation for the models and tools configured within the settings, based on the output type.
-
-        Returns:
-            str: Generated documentation for the configured models or tools.
-
-        Raises:
-            NotImplementedError: If no structured output is specified.
-        """
-        json_schema_mode = False
-        from llama_cpp_agent.providers.tgi_server import TGIServerProvider
-        from llama_cpp_agent.providers.vllm_server import VLLMServerProvider
-
-        if isinstance(provider, TGIServerProvider) or isinstance(
-            provider, VLLMServerProvider
-        ):
-            json_schema_mode = True
-        if self.output_type == LlmStructuredOutputType.no_structured_output:
-            raise NotImplementedError(
-                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
-            )
-        elif self.output_type == LlmStructuredOutputType.object_instance:
-            return generate_text_documentation(
-                self.pydantic_models, ordered_json_mode=json_schema_mode
-            ).strip()
-        elif self.output_type == LlmStructuredOutputType.list_of_objects:
-            return generate_text_documentation(
-                self.pydantic_models, ordered_json_mode=json_schema_mode
-            ).strip()
-        elif self.output_type == LlmStructuredOutputType.function_calling:
-            return generate_text_documentation(
-                [tool.model for tool in self.function_tools],
-                model_prefix="Function",
-                fields_prefix="Parameters",
-                ordered_json_mode=json_schema_mode,
-            ).strip()
-        elif self.output_type == LlmStructuredOutputType.parallel_function_calling:
-            return generate_text_documentation(
-                [tool.model for tool in self.function_tools],
-                model_prefix="Function",
-                fields_prefix="Parameters",
-                ordered_json_mode=json_schema_mode,
-            ).strip()
-
-    def get_gbnf_grammar(self):
-        """
-        Generate a GBNF grammar for tools configured within the settings, based on the output type.
-
-        Returns:
-            str: Generated GBNF grammar for the configured models or tools.
-
-        Raises:
-            NotImplementedError: If no structured output is specified.
-        """
-
-        if self.output_type == LlmStructuredOutputType.no_structured_output:
-            raise NotImplementedError(
-                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
-            )
-        elif self.output_type == LlmStructuredOutputType.object_instance:
-            return generate_gbnf_grammar_from_pydantic_models(
-                self.pydantic_models,
-                list_of_outputs=False,
-                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
-                outer_object_name=(self.output_model_name_field_name)
-                if not self.add_thoughts_and_reasoning_field
-                else (self.output_model_name_field_name),
-                outer_object_content=(self.output_model_attributes_field_name)
-                if not self.add_thoughts_and_reasoning_field
-                else (self.output_model_attributes_field_name),
-                inner_thought_field_name=self.thoughts_and_reasoning_field_name,
-                allow_only_inner_thoughts=False,
-                add_request_heartbeat=False,
-            )
-        elif self.output_type == LlmStructuredOutputType.list_of_objects:
-            return generate_gbnf_grammar_from_pydantic_models(
-                self.pydantic_models,
-                list_of_outputs=True,
-                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
-                outer_object_name=(self.output_model_name_field_name)
-                if not self.add_thoughts_and_reasoning_field
-                else (self.output_model_name_field_name),
-                outer_object_content=(self.output_model_attributes_field_name)
-                if not self.add_thoughts_and_reasoning_field
-                else (self.output_model_attributes_field_name),
-                inner_thought_field_name=(self.thoughts_and_reasoning_field_name),
-                allow_only_inner_thoughts=False,
-                add_request_heartbeat=False,
-            )
-        elif self.output_type == LlmStructuredOutputType.function_calling:
-            return generate_gbnf_grammar_from_pydantic_models(
-                [tool.model for tool in self.function_tools],
-                list_of_outputs=False,
-                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
-                outer_object_name=(self.function_calling_name_field_name)
-                if not self.add_thoughts_and_reasoning_field
-                else (self.function_calling_name_field_name),
-                outer_object_content=(self.function_calling_content)
-                if not self.add_thoughts_and_reasoning_field
-                else (self.function_calling_content),
-                inner_thought_field_name=self.thoughts_and_reasoning_field_name,
-                allow_only_inner_thoughts=False,
-                add_request_heartbeat=False,
-            )
-        elif self.output_type == LlmStructuredOutputType.parallel_function_calling:
-            return generate_gbnf_grammar_from_pydantic_models(
-                [tool.model for tool in self.function_tools],
-                list_of_outputs=True,
-                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
-                outer_object_name=(self.function_calling_name_field_name)
-                if not self.add_thoughts_and_reasoning_field
-                else (self.function_calling_name_field_name),
-                outer_object_content=(self.function_calling_content)
-                if not self.add_thoughts_and_reasoning_field
-                else (self.function_calling_content),
-                inner_thought_field_name=self.thoughts_and_reasoning_field_name,
-                allow_only_inner_thoughts=False,
-                add_request_heartbeat=False,
-            )
-
-    def get_json_schema(self):
-        """
-        Generate a JSON schema for the tools configured within the settings, based on the output type.
-
-        Returns:
-            Dict: Generated JSON schema for the configured models or tools.
-
-        Raises:
-            NotImplementedError: If no structured output is specified.
-        """
-
-        if self.output_type == LlmStructuredOutputType.no_structured_output:
-            raise NotImplementedError(
-                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
-            )
-        elif self.output_type == LlmStructuredOutputType.object_instance:
-            return generate_json_schemas(
-                self.pydantic_models,
-                allow_list=False,
-                outer_object_name=("001_" + self.output_model_name_field_name)
-                if not self.add_thoughts_and_reasoning_field
-                else ("002_" + self.output_model_name_field_name),
-                outer_object_properties_name=(
-                    "002_" + self.output_model_attributes_field_name
-                )
-                if not self.add_thoughts_and_reasoning_field
-                else ("003_" + self.output_model_attributes_field_name),
-                inner_thoughts_name=("001_" + self.thoughts_and_reasoning_field_name),
-                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
-            )
-        elif self.output_type == LlmStructuredOutputType.list_of_objects:
-            return generate_json_schemas(
-                self.pydantic_models,
-                allow_list=True,
-                outer_object_name=("001_" + self.output_model_name_field_name)
-                if not self.add_thoughts_and_reasoning_field
-                else ("002_" + self.output_model_name_field_name),
-                outer_object_properties_name=(
-                    "002_" + self.output_model_attributes_field_name
-                )
-                if not self.add_thoughts_and_reasoning_field
-                else ("003_" + self.output_model_attributes_field_name),
-                inner_thoughts_name=("001_" + self.thoughts_and_reasoning_field_name),
-                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
-            )
-        elif self.output_type is LlmStructuredOutputType.function_calling:
-            return generate_json_schemas(
-                [tool.model for tool in self.function_tools],
-                allow_list=False,
-                outer_object_name=("001_" + self.function_calling_name_field_name)
-                if not self.add_thoughts_and_reasoning_field
-                else ("002_" + self.function_calling_name_field_name),
-                outer_object_properties_name=("002_" + self.function_calling_content)
-                if not self.add_thoughts_and_reasoning_field
-                else ("003_" + self.function_calling_content),
-                inner_thoughts_name=("001_" + self.thoughts_and_reasoning_field_name),
-                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
-            )
-        elif self.output_type is LlmStructuredOutputType.parallel_function_calling:
-            return generate_json_schemas(
-                [tool.model for tool in self.function_tools],
-                allow_list=True,
-                outer_object_name=("001_" + self.function_calling_name_field_name)
-                if not self.add_thoughts_and_reasoning_field
-                else ("002_" + self.function_calling_name_field_name),
-                outer_object_properties_name=("002_" + self.function_calling_content)
-                if not self.add_thoughts_and_reasoning_field
-                else ("003_" + self.function_calling_content),
-                inner_thoughts_name=("001_" + self.thoughts_and_reasoning_field_name),
-                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
-            )
-
-    def handle_structured_output(self, llm_output: str):
-        if self.output_raw_json_string:
-            return llm_output
-        if (
-            self.output_type is LlmStructuredOutputType.function_calling
-            or self.output_type is LlmStructuredOutputType.parallel_function_calling
-        ):
-            output = parse_json_response(llm_output)
-            output = self.clean_keys(output)
-
-            return self.handle_function_call(output)
-        elif self.output_type == LlmStructuredOutputType.object_instance:
-            output = json.loads(llm_output)
-            output = self.clean_keys(output)
-            model_name = output[self.output_model_name_field_name]
-            model_attributes = output[self.output_model_attributes_field_name]
-            for model in self.pydantic_models:
-                if model_name == model.__name__:
-                    return model(**model_attributes)
-
-        elif self.output_type == LlmStructuredOutputType.list_of_objects:
-            output = json.loads(llm_output)
-            output = self.clean_keys(output)
-            models = []
-            for out in output:
-                for model in self.pydantic_models:
-                    model_name = out[self.output_model_name_field_name]
-                    model_attributes = out[self.output_model_attributes_field_name]
-                    if model_name == model.__name__:
-                        models.append(model(**model_attributes))
-            return models
-        return llm_output
-
-    def handle_function_call(self, function_call_response: Union[dict, List[dict]]):
-        """
-        Handle a function call response and return the output.
-
-        Args:
-            function_call_response (dict): The function call response.
-
-        Returns:
-            str: The output of the function call or an error message.
-        """
-
-        try:
-            function_call = function_call_response
-            if function_call is None:
-                return "Error: Invalid function call response."
-            if not self.output_type == LlmStructuredOutputType.parallel_function_calling:
-                output = self.intern_function_call(function_call)
-            else:
-                output = self.intern_parallel_function_call(function_call)
-
-            return output
-
-        except AttributeError as e:
-            return f"Error: {e}"
-
-    def intern_function_call(self, function_call: dict):
-        """
-        Internal method to handle a function call and return the output.
-
-        Args:
-            function_call (dict): The function call dictionary.
-        Returns:
-            str: The output of the function call or an error message.
-        """
-        if self.function_calling_content in function_call:
-            function_tool = None
-            for tool in self.function_tools:
-                if tool.model.__name__ == function_call[self.function_calling_name_field_name]:
-                    function_tool = tool
-                    break
-            if function_tool is not None:
-                cls = function_tool.model
-                call_parameters = function_call[self.function_calling_content]
-                call = cls(**call_parameters)
-                output = call.run(**function_tool.additional_parameters)
-                return [
-                    {
-                        self.function_calling_name_field_name: function_tool.model.__name__,
-                        self.function_calling_content: call_parameters,
-                        "return_value": output,
-                    }
-                ]
-
-    def intern_parallel_function_call(self, function_calls: List[dict]):
-        """
-        Internal method to handle a function call and return the output.
-
-        Args:
-            function_calls List[dict]: The function call dictionary.
-
-        Returns:
-            str: The output of the function call or an error message.
-        """
-        result = []
-        for function_call in function_calls:
-            if self.function_calling_content in function_call:
-                function_tool = None
-                for tool in self.function_tools:
-                    if tool.model.__name__ == function_call[self.function_calling_name_field_name]:
-                        function_tool = tool
-                        break
-                if function_tool is not None:
-                    try:
-                        cls = function_tool.model
-                        call_parameters = function_call[self.function_calling_content]
-                        call = cls(**call_parameters)
-                        output = call.run(**function_tool.additional_parameters)
-                        result.append(
-                            {
-                                self.function_calling_name_field_name: function_tool.model.__name__,
-                                self.function_calling_content: call_parameters,
-                                "return_value": output,
-                            }
-                        )
-                    except AttributeError as e:
-                        return f"Error: {e}"
-
-        return result
-
-    def clean_keys(self, data) -> Dict[str, Any] | List[Dict[str, Any]]:
-        if isinstance(data, dict):
-            # Create a new dictionary with modified keys
-            new_dict = {}
-            for key, value in data.items():
-                # Remove the leading 'XXX_' from keys
-                new_key = re.sub(r"^\d{3}_", "", key)
-                # Recursively clean nested dictionaries and lists
-                new_dict[new_key] = self.clean_keys(value)
-            return new_dict
-        elif isinstance(data, list):
-            # Process each item in the list
-            return [self.clean_keys(item) for item in data]
-        else:
-            # Return the item as is if it's not a dict or list
-            return data
+import json
+import re
+from enum import Enum
+from typing import Dict, List, Optional, Any, Callable, Tuple, Union
+
+from pydantic import BaseModel, Field
+
+from llama_cpp_agent.function_calling import LlamaCppFunctionTool
+from llama_cpp_agent.gbnf_grammar_generator.gbnf_grammar_from_pydantic_models import (
+    generate_gbnf_grammar_from_pydantic_models,
+)
+from llama_cpp_agent.json_schema_generator.schema_generator import generate_json_schemas
+from llama_cpp_agent.llm_documentation import generate_text_documentation
+from llama_cpp_agent.output_parser import parse_json_response
+
+
+class LlmStructuredOutputType(Enum):
+    """
+    Enum for defining different types of structured outputs that can be generated by a Language Model.
+    """
+
+    no_structured_output = "no_structured_output"
+    object_instance = "object_instance"
+    list_of_objects = "list_of_objects"
+    function_calling = "function_calling"
+    parallel_function_calling = "parallel_function_calling"
+
+
+class LlmStructuredOutputSettings(BaseModel):
+    """
+    Settings for structured output of large language models for using tools like function calling and creating instances of pydantic models.
+
+    Attributes:
+        output_type (LlmStructuredOutputType): Defines the type of structured output.
+        function_tools (Optional[List[LlamaCppFunctionTool]]): Tools to enable function calling.
+        pydantic_models (Optional[List[type[BaseModel]]]): List of pydantic models for structured data output.
+        add_thoughts_and_reasoning_field (Optional[bool]): Add thoughts and reasoning field to function calling. Defaults to False.
+        thoughts_and_reasoning_field_name (Optional[str]): Field name for the thoughts and reasoning field. Defaults to "thoughts_and_reasoning".
+        function_calling_name_field_name (Optional[str]): Name of the JSON field for the name of the used function. Defaults to "function".
+        function_calling_content (Optional[str]): Name of the JSON field for the arguments of the used function. Defaults to "arguments".
+        output_model_name_field_name (Optional[str]): Name of the JSON field for the name of the used pydantic model. Defaults to "model".
+        output_model_attributes_field_name (Optional[str]): Name of the JSON field for the fields of the pydantic model. Defaults to "fields".
+
+    Methods:
+        from_llama_cpp_function_tools: Create settings from a list of LlamaCppFunctionTools with a specific output type.
+        from_pydantic_models: Create settings from a list of Pydantic models with a specific output type.
+        from_open_ai_tools: Create settings from OpenAI tools for structured outputs.
+        from_functions: Create settings from a list of callable functions with a specific output type.
+        from_llama_index_tools: Create settings from a list of llama-index tools with a specific output type.
+        to_openai_tools: Return a list of OpenAI tools.
+        add_llama_cpp_function_tool: Add a LlamaCppFunctionTool to the settings.
+        add_pydantic_model: Add a Pydantic model to the settings, ensuring it matches the specified output type.
+        add_open_ai_tool: Add an OpenAI tool to the settings, ensuring it matches the specified output type.
+        add_function_tool: Add a callable function to the settings, ensuring it matches the specified output type.
+        add_llama_index_tool: Add a llama-index tool, like QueryEngineTool, to the settings, ensuring it matches the specified output type.
+        get_llm_documentation: Generate documentation for the models and tools configured within the settings, based on the output type.
+        get_gbnf_grammar: Generate a GBNF grammar for tools configured within the settings, based on the output type.
+        get_json_schema: Generate a JSON schema for the tools configured within the settings, based on the output type.
+    """
+
+    output_type: Optional[LlmStructuredOutputType] = Field(
+        ..., description="The output type of the llm"
+    )
+    function_tools: Optional[List[LlamaCppFunctionTool]] = Field(
+        None, description="List of functions tools for function calling"
+    )
+    pydantic_models: Optional[List[type[BaseModel]]] = Field(
+        None, description="List of pydantic models for structured output"
+    )
+    add_thoughts_and_reasoning_field: Optional[bool] = Field(
+        False, description="Add thoughts and reasoning field to function calling"
+    )
+
+    thoughts_and_reasoning_field_name: Optional[str] = Field(
+        "thoughts_and_reasoning",
+        description="Field name for the thoughts and reasoning field",
+    )
+
+    function_calling_name_field_name: Optional[str] = Field(
+        "function",
+        description="Name of the JSON field for the name of the used function.",
+    )
+    function_calling_content: Optional[str] = Field(
+        "arguments",
+        description="Name of the JSON field for the arguments of the used function.",
+    )
+
+    output_model_name_field_name: Optional[str] = Field(
+        "model",
+        description="Name of the JSON field for the name of the used pydantic model.",
+    )
+    output_model_attributes_field_name: Optional[str] = Field(
+        "fields",
+        description="Name of the JSON field for the fields of the pydantic model.",
+    )
+
+    output_raw_json_string: Optional[bool] = Field(
+        False,
+        description="If the output should be just the generated JSON string by the LLM",
+    )
+
+    class Config:
+        arbitrary_types_allowed = True
+
+    @staticmethod
+    def from_llama_cpp_function_tools(
+        llama_cpp_function_tools: List[LlamaCppFunctionTool],
+        allow_parallel_function_calling: bool = False,
+    ):
+        """
+        Create settings from a list of LlamaCppFunctionTools with a specific output type.
+
+        Args:
+            llama_cpp_function_tools (List[LlamaCppFunctionTool]): List of function tools.
+            allow_parallel_function_calling (bool): Whether to enable parallel function calling. Defaults to False.
+
+        Returns:
+            LlmStructuredOutputSettings: Configured settings object.
+        """
+        return LlmStructuredOutputSettings(
+            output_type=LlmStructuredOutputType.function_calling
+            if not allow_parallel_function_calling
+            else LlmStructuredOutputType.parallel_function_calling,
+            function_tools=llama_cpp_function_tools,
+        )
+
+    @staticmethod
+    def from_pydantic_models(
+        models: List[type[BaseModel]], output_type: LlmStructuredOutputType
+    ):
+        """
+        Create settings from a list of Pydantic models with a specific output type.
+
+        Args:
+            models (List[BaseModel]): List of Pydantic models.
+            output_type (LlmStructuredOutputType): Desired output type.
+
+        Returns:
+            LlmStructuredOutputSettings: Configured settings object.
+
+        Raises:
+            NotImplementedError: If no structured output is specified for the output type.
+        """
+        if output_type is LlmStructuredOutputType.no_structured_output:
+            raise NotImplementedError(
+                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
+            )
+        elif output_type is LlmStructuredOutputType.object_instance:
+            return LlmStructuredOutputSettings(
+                output_type=LlmStructuredOutputType.object_instance,
+                pydantic_models=models,
+            )
+        elif output_type is LlmStructuredOutputType.list_of_objects:
+            return LlmStructuredOutputSettings(
+                output_type=LlmStructuredOutputType.list_of_objects,
+                pydantic_models=models,
+            )
+        elif output_type is LlmStructuredOutputType.function_calling:
+            return LlmStructuredOutputSettings(
+                output_type=LlmStructuredOutputType.function_calling,
+                function_tools=[LlamaCppFunctionTool(model) for model in models],
+            )
+        elif output_type is LlmStructuredOutputType.parallel_function_calling:
+            return LlmStructuredOutputSettings(
+                output_type=LlmStructuredOutputType.parallel_function_calling,
+                function_tools=[LlamaCppFunctionTool(model) for model in models],
+            )
+
+    @staticmethod
+    def from_open_ai_tools(
+        tools: List[Tuple[Dict[str, Any], Callable]],
+        allow_parallel_function_calling: bool = False,
+    ):
+        """
+        Create settings from OpenAI tools for structured outputs.
+
+        Args:
+            tools (List[Tuple[Dict[str, Any], Callable]]): List of OpenAI tools defined by a schema and associated function.
+            allow_parallel_function_calling (bool): Whether to enable parallel function calling. Defaults to False.
+
+        Returns:
+            LlmStructuredOutputSettings: Configured settings object.
+        """
+        return LlmStructuredOutputSettings(
+            output_type=LlmStructuredOutputType.parallel_function_calling
+            if allow_parallel_function_calling
+            else LlmStructuredOutputType.function_calling,
+            function_tools=[LlamaCppFunctionTool(model) for model in tools],
+        )
+
+    @staticmethod
+    def from_functions(
+        tools: List[Callable], allow_parallel_function_calling: bool = False
+    ):
+        """
+        Create settings from a list of llama-index tools with a specific output type.
+
+        Args:
+            tools (list): List of llama-index tools.
+            allow_parallel_function_calling (bool): Whether to enable parallel function calling. Defaults to False.
+
+        Returns:
+            LlmStructuredOutputSettings: Configured settings object.
+
+        Raises:
+            NotImplementedError: If the specified output type is not supported for tools.
+        """
+        return LlmStructuredOutputSettings(
+            output_type=LlmStructuredOutputType.parallel_function_calling
+            if allow_parallel_function_calling
+            else LlmStructuredOutputType.function_calling,
+            function_tools=[LlamaCppFunctionTool(model) for model in tools],
+        )
+
+    @staticmethod
+    def from_llama_index_tools(
+        tools: list, allow_parallel_function_calling: bool = False
+    ):
+        """
+        Create settings from a list of llama-index tools with a specific output type. Has to be either LlmOutputType.function_call or LlmOutputType.parallel_function_call.
+
+        Args:
+            tools (list): List of llama-index tools.
+            allow_parallel_function_calling (bool): Whether to enable parallel function calling. Defaults to False.
+
+        Returns:
+            LlmStructuredOutputSettings: Configured settings object.
+
+        Raises:
+            NotImplementedError: If the specified output type is not supported for tools.
+        """
+        return LlmStructuredOutputSettings(
+            output_type=LlmStructuredOutputType.parallel_function_calling
+            if allow_parallel_function_calling
+            else LlmStructuredOutputType.function_calling,
+            function_tools=[
+                LlamaCppFunctionTool.from_llama_index_tool(model) for model in tools
+            ],
+        )
+
+    def to_openai_tools(self):
+        """
+        Return a list of OpenAI tools.
+        Returns:
+            List[Dict[str, Any]]: List of OpenAI tools.
+
+        Raises:
+            NotImplementedError: If the specified output type is not supported for tools.
+        """
+        if self.function_tools is not None:
+            return [tool.to_openai_tool() for tool in self.function_tools]
+
+    def add_llama_cpp_function_tool(self, tool: LlamaCppFunctionTool):
+        """
+        Add a LlamaCppFunctionTool to the settings.
+
+        Args:
+            tool (LlamaCppFunctionTool): The function tool to add.
+        """
+        self.function_tools.append(tool)
+
+    def add_pydantic_model(self, model: BaseModel):
+        """
+        Add a Pydantic model to the settings, ensuring it matches the specified output type.
+
+        Args:
+            model (BaseModel): The Pydantic model to add.
+
+        Raises:
+            NotImplementedError: If no structured output is specified.
+        """
+        if self.output_type is LlmStructuredOutputType.no_structured_output:
+            raise NotImplementedError(
+                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
+            )
+        elif self.output_type is LlmStructuredOutputType.object_instance:
+            self.pydantic_models.append(model)
+        elif self.output_type is LlmStructuredOutputType.list_of_objects:
+            self.pydantic_models.append(model)
+        elif self.output_type is LlmStructuredOutputType.function_calling:
+            self.function_tools.append(LlamaCppFunctionTool(model))
+        elif self.output_type is LlmStructuredOutputType.parallel_function_calling:
+            self.function_tools.append(LlamaCppFunctionTool(model))
+
+    def add_open_ai_tool(
+        self, open_ai_schema_and_function: Tuple[Dict[str, Any], Callable]
+    ):
+        """
+        Add an OpenAI tool to the settings, ensuring it matches the specified output type.
+
+        Args:
+            open_ai_schema_and_function (Tuple[Dict[str, Any], Callable]): The OpenAI schema and associated function to add.
+
+        Raises:
+            NotImplementedError: If the output type does not support adding tools.
+        """
+        if self.output_type is LlmStructuredOutputType.no_structured_output:
+            raise NotImplementedError(
+                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
+            )
+        elif self.output_type is LlmStructuredOutputType.function_calling:
+            self.function_tools.append(
+                LlamaCppFunctionTool(open_ai_schema_and_function)
+            )
+        elif self.output_type is LlmStructuredOutputType.parallel_function_calling:
+            self.function_tools.append(
+                LlamaCppFunctionTool(open_ai_schema_and_function)
+            )
+        else:
+            raise NotImplementedError(
+                f"LlmOutputType: {self.output_type.value} not supported for tools!"
+            )
+
+    def add_function_tool(self, function: Callable):
+        """
+        Add a callable function to the settings, ensuring it matches the specified output type.
+
+        Args:
+            function (Callable): The function to add.
+
+        Raises:
+            NotImplementedError: If the output type does not support adding tools.
+        """
+        if self.output_type is LlmStructuredOutputType.no_structured_output:
+            raise NotImplementedError(
+                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
+            )
+        elif self.output_type is LlmStructuredOutputType.function_calling:
+            self.function_tools.append(LlamaCppFunctionTool(function))
+        elif self.output_type is LlmStructuredOutputType.parallel_function_calling:
+            self.function_tools.append(LlamaCppFunctionTool(function))
+        else:
+            raise NotImplementedError(
+                f"LlmOutputType: {self.output_type.value} not supported for tools!"
+            )
+
+    def add_llama_index_tool(self, tool):
+        """
+        Add a llama-index tool, like QueryEngineTool, to the settings, ensuring it matches the specified output type.
+
+        Args:
+            tool: The llama-index tool to add.
+
+        Raises:
+            NotImplementedError: If the output type does not support adding tools.
+        """
+        if self.output_type is LlmStructuredOutputType.no_structured_output:
+            raise NotImplementedError(
+                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
+            )
+        elif self.output_type is LlmStructuredOutputType.function_calling:
+            self.function_tools.append(LlamaCppFunctionTool.from_llama_index_tool(tool))
+        elif self.output_type is LlmStructuredOutputType.parallel_function_calling:
+            self.function_tools.append(LlamaCppFunctionTool.from_llama_index_tool(tool))
+        else:
+            raise NotImplementedError(
+                f"LlmOutputType: {self.output_type.value} not supported for tools!"
+            )
+
+    def get_llm_documentation(self, provider):
+        """
+        Generate documentation for the models and tools configured within the settings, based on the output type.
+
+        Returns:
+            str: Generated documentation for the configured models or tools.
+
+        Raises:
+            NotImplementedError: If no structured output is specified.
+        """
+        json_schema_mode = False
+        from llama_cpp_agent.providers.tgi_server import TGIServerProvider
+        from llama_cpp_agent.providers.vllm_server import VLLMServerProvider
+
+        if isinstance(provider, TGIServerProvider) or isinstance(
+            provider, VLLMServerProvider
+        ):
+            json_schema_mode = True
+        if self.output_type == LlmStructuredOutputType.no_structured_output:
+            raise NotImplementedError(
+                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
+            )
+        elif self.output_type == LlmStructuredOutputType.object_instance:
+            return generate_text_documentation(
+                self.pydantic_models, ordered_json_mode=json_schema_mode
+            ).strip()
+        elif self.output_type == LlmStructuredOutputType.list_of_objects:
+            return generate_text_documentation(
+                self.pydantic_models, ordered_json_mode=json_schema_mode
+            ).strip()
+        elif self.output_type == LlmStructuredOutputType.function_calling:
+            return generate_text_documentation(
+                [tool.model for tool in self.function_tools],
+                model_prefix="Function",
+                fields_prefix="Parameters",
+                ordered_json_mode=json_schema_mode,
+            ).strip()
+        elif self.output_type == LlmStructuredOutputType.parallel_function_calling:
+            return generate_text_documentation(
+                [tool.model for tool in self.function_tools],
+                model_prefix="Function",
+                fields_prefix="Parameters",
+                ordered_json_mode=json_schema_mode,
+            ).strip()
+
+    def get_gbnf_grammar(self):
+        """
+        Generate a GBNF grammar for tools configured within the settings, based on the output type.
+
+        Returns:
+            str: Generated GBNF grammar for the configured models or tools.
+
+        Raises:
+            NotImplementedError: If no structured output is specified.
+        """
+
+        if self.output_type == LlmStructuredOutputType.no_structured_output:
+            raise NotImplementedError(
+                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
+            )
+        elif self.output_type == LlmStructuredOutputType.object_instance:
+            return generate_gbnf_grammar_from_pydantic_models(
+                self.pydantic_models,
+                list_of_outputs=False,
+                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
+                outer_object_name=(self.output_model_name_field_name)
+                if not self.add_thoughts_and_reasoning_field
+                else (self.output_model_name_field_name),
+                outer_object_content=(self.output_model_attributes_field_name)
+                if not self.add_thoughts_and_reasoning_field
+                else (self.output_model_attributes_field_name),
+                inner_thought_field_name=self.thoughts_and_reasoning_field_name,
+                allow_only_inner_thoughts=False,
+                add_request_heartbeat=False,
+            )
+        elif self.output_type == LlmStructuredOutputType.list_of_objects:
+            return generate_gbnf_grammar_from_pydantic_models(
+                self.pydantic_models,
+                list_of_outputs=True,
+                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
+                outer_object_name=(self.output_model_name_field_name)
+                if not self.add_thoughts_and_reasoning_field
+                else (self.output_model_name_field_name),
+                outer_object_content=(self.output_model_attributes_field_name)
+                if not self.add_thoughts_and_reasoning_field
+                else (self.output_model_attributes_field_name),
+                inner_thought_field_name=(self.thoughts_and_reasoning_field_name),
+                allow_only_inner_thoughts=False,
+                add_request_heartbeat=False,
+            )
+        elif self.output_type == LlmStructuredOutputType.function_calling:
+            return generate_gbnf_grammar_from_pydantic_models(
+                [tool.model for tool in self.function_tools],
+                list_of_outputs=False,
+                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
+                outer_object_name=(self.function_calling_name_field_name)
+                if not self.add_thoughts_and_reasoning_field
+                else (self.function_calling_name_field_name),
+                outer_object_content=(self.function_calling_content)
+                if not self.add_thoughts_and_reasoning_field
+                else (self.function_calling_content),
+                inner_thought_field_name=self.thoughts_and_reasoning_field_name,
+                allow_only_inner_thoughts=False,
+                add_request_heartbeat=False,
+            )
+        elif self.output_type == LlmStructuredOutputType.parallel_function_calling:
+            return generate_gbnf_grammar_from_pydantic_models(
+                [tool.model for tool in self.function_tools],
+                list_of_outputs=True,
+                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
+                outer_object_name=(self.function_calling_name_field_name)
+                if not self.add_thoughts_and_reasoning_field
+                else (self.function_calling_name_field_name),
+                outer_object_content=(self.function_calling_content)
+                if not self.add_thoughts_and_reasoning_field
+                else (self.function_calling_content),
+                inner_thought_field_name=self.thoughts_and_reasoning_field_name,
+                allow_only_inner_thoughts=False,
+                add_request_heartbeat=False,
+            )
+
+    def get_json_schema(self):
+        """
+        Generate a JSON schema for the tools configured within the settings, based on the output type.
+
+        Returns:
+            Dict: Generated JSON schema for the configured models or tools.
+
+        Raises:
+            NotImplementedError: If no structured output is specified.
+        """
+
+        if self.output_type == LlmStructuredOutputType.no_structured_output:
+            raise NotImplementedError(
+                "LlmOutputType: no_structured_output not supported for structured output and function calling!"
+            )
+        elif self.output_type == LlmStructuredOutputType.object_instance:
+            return generate_json_schemas(
+                self.pydantic_models,
+                allow_list=False,
+                outer_object_name=("001_" + self.output_model_name_field_name)
+                if not self.add_thoughts_and_reasoning_field
+                else ("002_" + self.output_model_name_field_name),
+                outer_object_properties_name=(
+                    "002_" + self.output_model_attributes_field_name
+                )
+                if not self.add_thoughts_and_reasoning_field
+                else ("003_" + self.output_model_attributes_field_name),
+                inner_thoughts_name=("001_" + self.thoughts_and_reasoning_field_name),
+                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
+            )
+        elif self.output_type == LlmStructuredOutputType.list_of_objects:
+            return generate_json_schemas(
+                self.pydantic_models,
+                allow_list=True,
+                outer_object_name=("001_" + self.output_model_name_field_name)
+                if not self.add_thoughts_and_reasoning_field
+                else ("002_" + self.output_model_name_field_name),
+                outer_object_properties_name=(
+                    "002_" + self.output_model_attributes_field_name
+                )
+                if not self.add_thoughts_and_reasoning_field
+                else ("003_" + self.output_model_attributes_field_name),
+                inner_thoughts_name=("001_" + self.thoughts_and_reasoning_field_name),
+                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
+            )
+        elif self.output_type is LlmStructuredOutputType.function_calling:
+            return generate_json_schemas(
+                [tool.model for tool in self.function_tools],
+                allow_list=False,
+                outer_object_name=("001_" + self.function_calling_name_field_name)
+                if not self.add_thoughts_and_reasoning_field
+                else ("002_" + self.function_calling_name_field_name),
+                outer_object_properties_name=("002_" + self.function_calling_content)
+                if not self.add_thoughts_and_reasoning_field
+                else ("003_" + self.function_calling_content),
+                inner_thoughts_name=("001_" + self.thoughts_and_reasoning_field_name),
+                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
+            )
+        elif self.output_type is LlmStructuredOutputType.parallel_function_calling:
+            return generate_json_schemas(
+                [tool.model for tool in self.function_tools],
+                allow_list=True,
+                outer_object_name=("001_" + self.function_calling_name_field_name)
+                if not self.add_thoughts_and_reasoning_field
+                else ("002_" + self.function_calling_name_field_name),
+                outer_object_properties_name=("002_" + self.function_calling_content)
+                if not self.add_thoughts_and_reasoning_field
+                else ("003_" + self.function_calling_content),
+                inner_thoughts_name=("001_" + self.thoughts_and_reasoning_field_name),
+                add_inner_thoughts=self.add_thoughts_and_reasoning_field,
+            )
+
+    def handle_structured_output(self, llm_output: str):
+        if self.output_raw_json_string:
+            return llm_output
+        if (
+            self.output_type is LlmStructuredOutputType.function_calling
+            or self.output_type is LlmStructuredOutputType.parallel_function_calling
+        ):
+            output = parse_json_response(llm_output)
+            output = self.clean_keys(output)
+
+            return self.handle_function_call(output)
+        elif self.output_type == LlmStructuredOutputType.object_instance:
+            output = json.loads(llm_output)
+            output = self.clean_keys(output)
+            model_name = output[self.output_model_name_field_name]
+            model_attributes = output[self.output_model_attributes_field_name]
+            for model in self.pydantic_models:
+                if model_name == model.__name__:
+                    return model(**model_attributes)
+
+        elif self.output_type == LlmStructuredOutputType.list_of_objects:
+            output = json.loads(llm_output)
+            output = self.clean_keys(output)
+            models = []
+            for out in output:
+                for model in self.pydantic_models:
+                    model_name = out[self.output_model_name_field_name]
+                    model_attributes = out[self.output_model_attributes_field_name]
+                    if model_name == model.__name__:
+                        models.append(model(**model_attributes))
+            return models
+        return llm_output
+
+    def handle_function_call(self, function_call_response: Union[dict, List[dict]]):
+        """
+        Handle a function call response and return the output.
+
+        Args:
+            function_call_response (dict): The function call response.
+
+        Returns:
+            str: The output of the function call or an error message.
+        """
+
+        try:
+            function_call = function_call_response
+            if function_call is None:
+                return "Error: Invalid function call response."
+            if not self.output_type == LlmStructuredOutputType.parallel_function_calling:
+                output = self.intern_function_call(function_call)
+            else:
+                output = self.intern_parallel_function_call(function_call)
+
+            return output
+
+        except AttributeError as e:
+            return f"Error: {e}"
+
+    def intern_function_call(self, function_call: dict):
+        """
+        Internal method to handle a function call and return the output.
+
+        Args:
+            function_call (dict): The function call dictionary.
+        Returns:
+            str: The output of the function call or an error message.
+        """
+        if self.function_calling_content in function_call:
+            function_tool = None
+            for tool in self.function_tools:
+                if tool.model.__name__ == function_call[self.function_calling_name_field_name]:
+                    function_tool = tool
+                    break
+            if function_tool is not None:
+                cls = function_tool.model
+                call_parameters = function_call[self.function_calling_content]
+                call = cls(**call_parameters)
+                output = call.run(**function_tool.additional_parameters)
+                return [
+                    {
+                        self.function_calling_name_field_name: function_tool.model.__name__,
+                        self.function_calling_content: call_parameters,
+                        "return_value": output,
+                    }
+                ]
+
+    def intern_parallel_function_call(self, function_calls: List[dict]):
+        """
+        Internal method to handle a function call and return the output.
+
+        Args:
+            function_calls List[dict]: The function call dictionary.
+
+        Returns:
+            str: The output of the function call or an error message.
+        """
+        result = []
+        for function_call in function_calls:
+            if self.function_calling_content in function_call:
+                function_tool = None
+                for tool in self.function_tools:
+                    if tool.model.__name__ == function_call[self.function_calling_name_field_name]:
+                        function_tool = tool
+                        break
+                if function_tool is not None:
+                    try:
+                        cls = function_tool.model
+                        call_parameters = function_call[self.function_calling_content]
+                        call = cls(**call_parameters)
+                        output = call.run(**function_tool.additional_parameters)
+                        result.append(
+                            {
+                                self.function_calling_name_field_name: function_tool.model.__name__,
+                                self.function_calling_content: call_parameters,
+                                "return_value": output,
+                            }
+                        )
+                    except AttributeError as e:
+                        return f"Error: {e}"
+
+        return result
+
+    def clean_keys(self, data) -> Dict[str, Any] | List[Dict[str, Any]]:
+        if isinstance(data, dict):
+            # Create a new dictionary with modified keys
+            new_dict = {}
+            for key, value in data.items():
+                # Remove the leading 'XXX_' from keys
+                new_key = re.sub(r"^\d{3}_", "", key)
+                # Recursively clean nested dictionaries and lists
+                new_dict[new_key] = self.clean_keys(value)
+            return new_dict
+        elif isinstance(data, list):
+            # Process each item in the list
+            return [self.clean_keys(item) for item in data]
+        else:
+            # Return the item as is if it's not a dict or list
+            return data
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_prompt_template.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/llm_prompt_template.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,199 +1,199 @@
-import re
-from dataclasses import dataclass
-from typing import List, Dict, Union
-
-
-@dataclass
-class PromptTemplateField:
-    """
-    Data class representing a field in a prompt template.
-
-    Attributes:
-        name (str): The name of the template field.
-        value (str): The value associated with the template field.
-    """
-
-    name: str
-    value: str
-
-
-class PromptTemplateFields:
-    """
-    Class representing a collection of PromptTemplateField objects.
-
-    Methods:
-        add_field(name: str, value: str): Add a new field to the collection.
-        remove_field(name: str): Remove a field by name from the collection.
-        edit_field(name: str, new_value: str): Edit the value of an existing field.
-        find_field(name: str) -> PromptTemplateField: Find and return a field by name.
-        list_fields() -> List[PromptTemplateField]: Get a list of all fields in the collection.
-        get_fields_dict() -> Dict[str, str]: Get a dictionary representation of the fields.
-        set_fields_from_dict(field_dict: Dict[str, str]): Set the fields using a dictionary.
-
-    Attributes:
-        fields (List[PromptTemplateField]): List of PromptTemplateField objects.
-    """
-
-    def __init__(self):
-        self.fields: List[PromptTemplateField] = []
-
-    def add_field(self, name: str, value: str):
-        """Add a new field to the collection."""
-        self.fields.append(PromptTemplateField(name, value))
-
-    def remove_field(self, name: str):
-        """Remove a field by name from the collection."""
-        self.fields = [field for field in self.fields if field.name != name]
-
-    def edit_field(self, name: str, new_value: str):
-        """Edit the value of an existing field."""
-        field = self.find_field(name)
-        if field:
-            field.value = new_value
-        else:
-            raise ValueError(f"Field '{name}' not found.")
-
-    def find_field(self, name: str) -> PromptTemplateField:
-        """Find and return a field by name."""
-        for field in self.fields:
-            if field.name == name:
-                return field
-        return None
-
-    def list_fields(self):
-        """Get a list of all fields in the collection."""
-        return self.fields
-
-    def get_fields_dict(self) -> Dict[str, str]:
-        """Get a dictionary representation of the fields."""
-        return {field.name: field.value for field in self.fields}
-
-    def set_fields_from_dict(self, field_dict: Dict[str, str]):
-        """Set the fields using a dictionary."""
-        self.fields.clear()
-        for name, value in field_dict.items():
-            self.add_field(name, value)
-
-
-class PromptTemplate:
-    """
-    Class representing a prompt template.
-
-    Methods:
-        generate_prompt(template_fields: Union[dict, PromptTemplateFields], remove_empty_template_field=True) -> str:
-        Generate a prompt by replacing placeholders in the template with values.
-
-    Class Methods:
-        from_string(template_string: str) -> PromptTemplate:
-        Create a PromptTemplate from a string.
-        from_file(template_file: str) -> PromptTemplate:
-        Create a PromptTemplate from a file.
-
-    Attributes:
-        template (str): The template string containing placeholders.
-    """
-
-    def __init__(self, template_file=None, template_string=None):
-        """
-        Initialize a PromptTemplate instance.
-
-        Args:
-            template_file (str): The path to a file containing the template.
-            template_string (str): The template string.
-        """
-        if template_file:
-            with open(template_file, "r") as file:
-                self.template = file.read()
-        elif template_string:
-            self.template = template_string
-        else:
-            raise ValueError(
-                "Either 'template_file' or 'template_string' must be provided"
-            )
-
-    @classmethod
-    def from_string(cls, template_string):
-        """
-        Create a PromptTemplate instance from a string.
-
-        Args:
-            template_string (str): The template string.
-
-        Returns:
-            PromptTemplate: Created PromptTemplate instance.
-        """
-        return cls(template_string=template_string)
-
-    @classmethod
-    def from_file(cls, template_file):
-        """
-        Create a PromptTemplate instance from a file.
-
-        Args:
-            template_file (str): The path to a file containing the template.
-
-        Returns:
-            PromptTemplate: Created PromptTemplate instance.
-        """
-        with open(template_file, "r") as file:
-            template_string = file.read()
-        return cls(template_string=template_string)
-
-    def _remove_empty_placeholders(self, text):
-        """
-        Remove lines that contain only the empty placeholder.
-
-        Args:
-            text (str): The text containing placeholders.
-
-        Returns:
-            str: Text with empty placeholders removed.
-        """
-        # Remove lines that contain only the empty placeholder
-        text = re.sub(rf'^{"__EMPTY_TEMPLATE_FIELD__"}$', "", text, flags=re.MULTILINE)
-        # Remove the empty placeholder from lines with other content
-        text = re.sub(rf'{"__EMPTY_TEMPLATE_FIELD__"}', "", text)
-        return text
-
-    def generate_prompt(
-        self,
-        template_fields: Union[dict, PromptTemplateFields],
-        remove_empty_template_field=True,
-    ) -> str:
-        """
-        Generate a prompt by replacing placeholders in the template with values.
-
-        Args:
-            template_fields (Union[dict, PromptTemplateFields]): The template fields.
-            remove_empty_template_field (bool): If True, removes lines with empty placeholders.
-
-        Returns:
-            str: The generated prompt.
-        """
-        cleaned_fields = {}
-        for key, value in template_fields.items():
-            cleaned_fields[key] = str(value) if not isinstance(value, str) else value
-
-        template_fields = cleaned_fields
-        if isinstance(template_fields, PromptTemplateFields):
-            template_fields = template_fields.get_fields_dict()
-
-        if not remove_empty_template_field:
-
-            def replace_placeholder(match):
-                placeholder = match.group(1)
-                return template_fields.get(placeholder, match.group(0))
-
-            prompt = re.sub(r"\{(\w+)\}", replace_placeholder, self.template)
-            return prompt
-
-        def replace_placeholder(match):
-            placeholder = match.group(1)
-            if template_fields.get(placeholder, match.group(0)) != "":
-                return template_fields.get(placeholder, match.group(0))
-            return "__EMPTY_TEMPLATE_FIELD__"
-
-        # Initial placeholder replacement
-        prompt = re.sub(r"\{(\w+)\}", replace_placeholder, self.template)
-
-        return self._remove_empty_placeholders(prompt)
+import re
+from dataclasses import dataclass
+from typing import List, Dict, Union
+
+
+@dataclass
+class PromptTemplateField:
+    """
+    Data class representing a field in a prompt template.
+
+    Attributes:
+        name (str): The name of the template field.
+        value (str): The value associated with the template field.
+    """
+
+    name: str
+    value: str
+
+
+class PromptTemplateFields:
+    """
+    Class representing a collection of PromptTemplateField objects.
+
+    Methods:
+        add_field(name: str, value: str): Add a new field to the collection.
+        remove_field(name: str): Remove a field by name from the collection.
+        edit_field(name: str, new_value: str): Edit the value of an existing field.
+        find_field(name: str) -> PromptTemplateField: Find and return a field by name.
+        list_fields() -> List[PromptTemplateField]: Get a list of all fields in the collection.
+        get_fields_dict() -> Dict[str, str]: Get a dictionary representation of the fields.
+        set_fields_from_dict(field_dict: Dict[str, str]): Set the fields using a dictionary.
+
+    Attributes:
+        fields (List[PromptTemplateField]): List of PromptTemplateField objects.
+    """
+
+    def __init__(self):
+        self.fields: List[PromptTemplateField] = []
+
+    def add_field(self, name: str, value: str):
+        """Add a new field to the collection."""
+        self.fields.append(PromptTemplateField(name, value))
+
+    def remove_field(self, name: str):
+        """Remove a field by name from the collection."""
+        self.fields = [field for field in self.fields if field.name != name]
+
+    def edit_field(self, name: str, new_value: str):
+        """Edit the value of an existing field."""
+        field = self.find_field(name)
+        if field:
+            field.value = new_value
+        else:
+            raise ValueError(f"Field '{name}' not found.")
+
+    def find_field(self, name: str) -> PromptTemplateField:
+        """Find and return a field by name."""
+        for field in self.fields:
+            if field.name == name:
+                return field
+        return None
+
+    def list_fields(self):
+        """Get a list of all fields in the collection."""
+        return self.fields
+
+    def get_fields_dict(self) -> Dict[str, str]:
+        """Get a dictionary representation of the fields."""
+        return {field.name: field.value for field in self.fields}
+
+    def set_fields_from_dict(self, field_dict: Dict[str, str]):
+        """Set the fields using a dictionary."""
+        self.fields.clear()
+        for name, value in field_dict.items():
+            self.add_field(name, value)
+
+
+class PromptTemplate:
+    """
+    Class representing a prompt template.
+
+    Methods:
+        generate_prompt(template_fields: Union[dict, PromptTemplateFields], remove_empty_template_field=True) -> str:
+        Generate a prompt by replacing placeholders in the template with values.
+
+    Class Methods:
+        from_string(template_string: str) -> PromptTemplate:
+        Create a PromptTemplate from a string.
+        from_file(template_file: str) -> PromptTemplate:
+        Create a PromptTemplate from a file.
+
+    Attributes:
+        template (str): The template string containing placeholders.
+    """
+
+    def __init__(self, template_file=None, template_string=None):
+        """
+        Initialize a PromptTemplate instance.
+
+        Args:
+            template_file (str): The path to a file containing the template.
+            template_string (str): The template string.
+        """
+        if template_file:
+            with open(template_file, "r") as file:
+                self.template = file.read()
+        elif template_string:
+            self.template = template_string
+        else:
+            raise ValueError(
+                "Either 'template_file' or 'template_string' must be provided"
+            )
+
+    @classmethod
+    def from_string(cls, template_string):
+        """
+        Create a PromptTemplate instance from a string.
+
+        Args:
+            template_string (str): The template string.
+
+        Returns:
+            PromptTemplate: Created PromptTemplate instance.
+        """
+        return cls(template_string=template_string)
+
+    @classmethod
+    def from_file(cls, template_file):
+        """
+        Create a PromptTemplate instance from a file.
+
+        Args:
+            template_file (str): The path to a file containing the template.
+
+        Returns:
+            PromptTemplate: Created PromptTemplate instance.
+        """
+        with open(template_file, "r") as file:
+            template_string = file.read()
+        return cls(template_string=template_string)
+
+    def _remove_empty_placeholders(self, text):
+        """
+        Remove lines that contain only the empty placeholder.
+
+        Args:
+            text (str): The text containing placeholders.
+
+        Returns:
+            str: Text with empty placeholders removed.
+        """
+        # Remove lines that contain only the empty placeholder
+        text = re.sub(rf'^{"__EMPTY_TEMPLATE_FIELD__"}$', "", text, flags=re.MULTILINE)
+        # Remove the empty placeholder from lines with other content
+        text = re.sub(rf'{"__EMPTY_TEMPLATE_FIELD__"}', "", text)
+        return text
+
+    def generate_prompt(
+        self,
+        template_fields: Union[dict, PromptTemplateFields],
+        remove_empty_template_field=True,
+    ) -> str:
+        """
+        Generate a prompt by replacing placeholders in the template with values.
+
+        Args:
+            template_fields (Union[dict, PromptTemplateFields]): The template fields.
+            remove_empty_template_field (bool): If True, removes lines with empty placeholders.
+
+        Returns:
+            str: The generated prompt.
+        """
+        cleaned_fields = {}
+        for key, value in template_fields.items():
+            cleaned_fields[key] = str(value) if not isinstance(value, str) else value
+
+        template_fields = cleaned_fields
+        if isinstance(template_fields, PromptTemplateFields):
+            template_fields = template_fields.get_fields_dict()
+
+        if not remove_empty_template_field:
+
+            def replace_placeholder(match):
+                placeholder = match.group(1)
+                return template_fields.get(placeholder, match.group(0))
+
+            prompt = re.sub(r"\{(\w+)\}", replace_placeholder, self.template)
+            return prompt
+
+        def replace_placeholder(match):
+            placeholder = match.group(1)
+            if template_fields.get(placeholder, match.group(0)) != "":
+                return template_fields.get(placeholder, match.group(0))
+            return "__EMPTY_TEMPLATE_FIELD__"
+
+        # Initial placeholder replacement
+        prompt = re.sub(r"\{(\w+)\}", replace_placeholder, self.template)
+
+        return self._remove_empty_placeholders(prompt)
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/messages_formatter.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/messages_formatter.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,349 +1,349 @@
-import json
-from dataclasses import dataclass
-from enum import Enum
-from typing import List, Dict, Tuple, Literal
-
-from llama_cpp_agent.chat_history.messages import Roles
-
-
-class MessagesFormatterType(Enum):
-    """
-    Enum representing different types of predefined messages formatters.
-    """
-
-    MISTRAL = 1
-    CHATML = 2
-    VICUNA = 3
-    LLAMA_2 = 4
-    SYNTHIA = 5
-    NEURAL_CHAT = 6
-    SOLAR = 7
-    OPEN_CHAT = 8
-    ALPACA = 9
-    CODE_DS = 10
-    B22 = 11
-    LLAMA_3 = 12
-    PHI_3 = 13
-
-
-@dataclass
-class PromptMarkers:
-    start: str
-    end: str
-
-
-class MessagesFormatter:
-    def __init__(
-            self,
-            pre_prompt: str,
-            prompt_markers: Dict[Roles, PromptMarkers],
-            include_sys_prompt_in_first_user_message: bool,
-            default_stop_sequences: List[str],
-            use_user_role_for_function_call_result: bool = True,
-            strip_prompt: bool = True,
-            bos_token: str = "<s>",
-            eos_token: str = "</s>"
-    ):
-        self.pre_prompt = pre_prompt
-        self.prompt_markers = prompt_markers
-        self.include_sys_prompt_in_first_user_message = include_sys_prompt_in_first_user_message
-        self.default_stop_sequences = default_stop_sequences
-        self.use_user_role_for_function_call_result = use_user_role_for_function_call_result
-        self.strip_prompt = strip_prompt
-        self.bos_token = bos_token
-        self.eos_token = eos_token
-        self.added_system_prompt = False
-
-    def get_bos_token(self) -> str:
-        return self.bos_token
-
-    def format_conversation(
-            self,
-            messages: List[Dict[str, str]],
-            response_role: Literal[Roles.user, Roles.assistant] | None = None,
-    ) -> Tuple[str, Roles]:
-        formatted_messages = self.pre_prompt
-        last_role = Roles.assistant
-        self.added_system_prompt = False
-        for message in messages:
-            role = Roles(message["role"])
-            content = self._format_message_content(message["content"], role)
-
-            if role == Roles.system:
-                formatted_messages += self._format_system_message(content)
-                last_role = Roles.system
-            elif role == Roles.user:
-                formatted_messages += self._format_user_message(content)
-                last_role = Roles.user
-            elif role == Roles.assistant:
-                formatted_messages += self._format_assistant_message(content)
-                last_role = Roles.assistant
-            elif role == Roles.tool:
-                formatted_messages += self._format_tool_message(content)
-                last_role = Roles.tool
-
-        return self._format_response(formatted_messages, last_role, response_role)
-
-    def _format_message_content(self, content: str, role: Roles) -> str:
-        if self.strip_prompt and role != Roles.tool:
-            return content.strip()
-        return content
-
-    def _format_system_message(self, content: str) -> str:
-        formatted_message = self.prompt_markers[Roles.system].start + content + self.prompt_markers[Roles.system].end
-        self.added_system_prompt = True
-        if self.include_sys_prompt_in_first_user_message:
-            formatted_message = self.prompt_markers[Roles.user].start + formatted_message
-        return formatted_message
-
-    def _format_user_message(self, content: str) -> str:
-        if self.include_sys_prompt_in_first_user_message and self.added_system_prompt:
-            return content + self.prompt_markers[Roles.user].end
-        return self.prompt_markers[Roles.user].start + content + self.prompt_markers[Roles.user].end
-
-    def _format_assistant_message(self, content: str) -> str:
-        return self.prompt_markers[Roles.assistant].start + content + self.prompt_markers[Roles.assistant].end
-
-    def _format_tool_message(self, content: str) -> str:
-        if isinstance(content, list):
-            content = "\n".join(json.dumps(m, indent=2) for m in content)
-        if self.use_user_role_for_function_call_result:
-            return self._format_user_message(content)
-        else:
-            return self.prompt_markers[Roles.tool].start + content + self.prompt_markers[Roles.tool].end
-
-    def _format_response(
-            self,
-            formatted_messages: str,
-            last_role: Roles,
-            response_role: Literal[Roles.user, Roles.assistant] | None = None,
-    ) -> Tuple[str, Roles]:
-        if response_role is None:
-            response_role = Roles.assistant if last_role != Roles.assistant else Roles.user
-
-        prompt_start = self.prompt_markers[response_role].start.strip() if self.strip_prompt else self.prompt_markers[
-            response_role].start
-        return formatted_messages + prompt_start, response_role
-
-
-mixtral_prompt_markers = {
-    Roles.system: PromptMarkers("", """\n\n"""),
-    Roles.user: PromptMarkers("""[INST] """, """ """),
-    Roles.assistant: PromptMarkers("""[/INST]""", """</s>"""),
-    Roles.tool: PromptMarkers("", ""),
-}
-
-chatml_prompt_markers = {
-    Roles.system: PromptMarkers("""<|im_start|>system\n""", """<|im_end|>\n"""),
-    Roles.user: PromptMarkers("""<|im_start|>user\n""", """<|im_end|>\n"""),
-    Roles.assistant: PromptMarkers("""<|im_start|>assistant\n""", """<|im_end|>\n"""),
-    Roles.tool: PromptMarkers("""<|im_start|>function\n""", """<|im_end|>\n"""),
-}
-
-vicuna_prompt_markers = {
-    Roles.system: PromptMarkers("", """\n\n"""),
-    Roles.user: PromptMarkers("""USER:""", """\n"""),
-    Roles.assistant: PromptMarkers("""ASSISTANT:""", ""),
-    Roles.tool: PromptMarkers("", ""),
-}
-
-llama_2_prompt_markers = {
-    Roles.system: PromptMarkers("<<SYS>>\n", "\n<</SYS>>\n\n"),
-    Roles.user: PromptMarkers("[INST] ", " [/INST]"),
-    Roles.assistant: PromptMarkers(" ", " </s>"),
-    Roles.tool: PromptMarkers("", ""),
-}
-
-llama_3_prompt_markers = {
-    Roles.system: PromptMarkers("""<|start_header_id|>system<|end_header_id|>\n""", """<|eot_id|>"""),
-    Roles.user: PromptMarkers("""<|start_header_id|>user<|end_header_id|>\n""", """<|eot_id|>"""),
-    Roles.assistant: PromptMarkers("""<|start_header_id|>assistant<|end_header_id|>\n""", """<|eot_id|>"""),
-    Roles.tool: PromptMarkers("""<|start_header_id|>function_calling_results<|end_header_id|>\n""", """<|eot_id|>"""),
-}
-
-synthia_prompt_markers = {
-    Roles.system: PromptMarkers("""SYSTEM: """, """\n"""),
-    Roles.user: PromptMarkers("""USER: """, """\n"""),
-    Roles.assistant: PromptMarkers("""ASSISTANT:""", """\n"""),
-    Roles.tool: PromptMarkers("", ""),
-}
-
-neural_chat_prompt_markers = {
-    Roles.system: PromptMarkers("""### System:\n""", """\n"""),
-    Roles.user: PromptMarkers("""### User:\n""", """ \n"""),
-    Roles.assistant: PromptMarkers("""### Assistant:\n""", """\n"""),
-    Roles.tool: PromptMarkers("", ""),
-}
-
-code_ds_prompt_markers = {
-    Roles.system: PromptMarkers("", """\n\n"""),
-    Roles.user: PromptMarkers("""@@ Instruction\n""", """\n\n"""),
-    Roles.assistant: PromptMarkers("""@@ Response\n""", """\n\n"""),
-    Roles.tool: PromptMarkers("", ""),
-}
-
-solar_prompt_markers = {
-    Roles.system: PromptMarkers("", """\n"""),
-    Roles.user: PromptMarkers("""### User:\n""", """ \n"""),
-    Roles.assistant: PromptMarkers("""### Assistant:\n""", """\n"""),
-    Roles.tool: PromptMarkers("", ""),
-}
-
-open_chat_prompt_markers = {
-    Roles.system: PromptMarkers("", """  """),
-    Roles.user: PromptMarkers("""GPT4 Correct User: """, """<|end_of_turn|>"""),
-    Roles.assistant: PromptMarkers("""GPT4 Correct Assistant: """, """<|end_of_turn|>"""),
-    Roles.tool: PromptMarkers("", ""),
-}
-
-alpaca_prompt_markers = {
-    Roles.system: PromptMarkers("""### Instruction:\n""", """\n"""),
-    Roles.user: PromptMarkers("""### Input:\n""", """ \n"""),
-    Roles.assistant: PromptMarkers("""### Response:\n""", """\n"""),
-    Roles.tool: PromptMarkers("""<|im_start|>function\n""", """<|im_end|>\n"""),
-}
-
-b22_chat_prompt_markers = {
-    Roles.system: PromptMarkers("""### System: """, """\n"""),
-    Roles.user: PromptMarkers("""### User: """, """ \n"""),
-    Roles.assistant: PromptMarkers("""### Assistant:""", """\n"""),
-    Roles.tool: PromptMarkers("", ""),
-}
-
-phi_3_chat_prompt_markers = {
-    Roles.system: PromptMarkers("", """\n\n"""),
-    Roles.user: PromptMarkers("""<|user|>""", """<|end|>\n"""),
-    Roles.assistant: PromptMarkers("""<|assistant|>""", """<|end|>\n"""),
-    Roles.tool: PromptMarkers("", ""),
-}
-
-mixtral_formatter = MessagesFormatter(
-    "",
-    mixtral_prompt_markers,
-    True,
-    ["</s>"],
-)
-
-chatml_formatter = MessagesFormatter(
-    "",
-    chatml_prompt_markers,
-    False,
-    ["<|im_end|>", "</s>"],
-    use_user_role_for_function_call_result=False,
-    strip_prompt=False,
-)
-
-vicuna_formatter = MessagesFormatter(
-    "",
-    vicuna_prompt_markers,
-    False,
-    ["</s>", "USER:"],
-)
-
-llama_2_formatter = MessagesFormatter(
-    "",
-    llama_2_prompt_markers,
-    True,
-    ["</s>", "[INST]"],
-)
-
-llama_3_formatter = MessagesFormatter(
-    "",
-    llama_3_prompt_markers,
-    False,
-    ["assistant", "<|eot_id|>"],
-    use_user_role_for_function_call_result=False,
-    strip_prompt=True,
-)
-
-synthia_formatter = MessagesFormatter(
-    "",
-    synthia_prompt_markers,
-    False,
-    ["</s>", "USER:"],
-)
-
-neural_chat_formatter = MessagesFormatter(
-    "",
-    neural_chat_prompt_markers,
-    False,
-    ["### User:"],
-    strip_prompt=False,
-)
-
-code_ds_formatter = MessagesFormatter(
-    "",
-    code_ds_prompt_markers,
-    True,
-    ["@@ Instruction"],
-)
-
-solar_formatter = MessagesFormatter(
-    "",
-    solar_prompt_markers,
-    True,
-    ["### User:"],
-)
-
-open_chat_formatter = MessagesFormatter(
-    "",
-    open_chat_prompt_markers,
-    True,
-    ["<|end_of_turn|>"],
-    use_user_role_for_function_call_result=True,
-)
-
-alpaca_formatter = MessagesFormatter(
-    "",
-    alpaca_prompt_markers,
-    False,
-    ["### Instruction:", "### Input:", "### Response:"],
-    use_user_role_for_function_call_result=False,
-)
-
-b22_chat_formatter = MessagesFormatter(
-    "",
-    b22_chat_prompt_markers,
-    False,
-    ["### User:"],
-    strip_prompt=False,
-)
-
-phi_3_chat_formatter = MessagesFormatter(
-    "",
-    phi_3_chat_prompt_markers,
-    True,
-    ["<|end|>", "<|end_of_turn|>"],
-    use_user_role_for_function_call_result=True,
-)
-
-predefined_formatter = {
-    MessagesFormatterType.MISTRAL: mixtral_formatter,
-    MessagesFormatterType.CHATML: chatml_formatter,
-    MessagesFormatterType.VICUNA: vicuna_formatter,
-    MessagesFormatterType.LLAMA_2: llama_2_formatter,
-    MessagesFormatterType.SYNTHIA: synthia_formatter,
-    MessagesFormatterType.NEURAL_CHAT: neural_chat_formatter,
-    MessagesFormatterType.SOLAR: solar_formatter,
-    MessagesFormatterType.OPEN_CHAT: open_chat_formatter,
-    MessagesFormatterType.ALPACA: alpaca_formatter,
-    MessagesFormatterType.CODE_DS: code_ds_formatter,
-    MessagesFormatterType.B22: b22_chat_formatter,
-    MessagesFormatterType.LLAMA_3: llama_3_formatter,
-    MessagesFormatterType.PHI_3: phi_3_chat_formatter,
-}
-
-
-def get_predefined_messages_formatter(
-        formatter_type: MessagesFormatterType,
-) -> MessagesFormatter:
-    """
-    Gets a predefined messages formatter based on the formatter type.
-
-    Args:
-        formatter_type (MessagesFormatterType): The type of messages formatter.
-
-    Returns:
-        MessagesFormatter: The predefined messages formatter.
-    """
-    return predefined_formatter[formatter_type]
+import json
+from dataclasses import dataclass
+from enum import Enum
+from typing import List, Dict, Tuple, Literal
+
+from llama_cpp_agent.chat_history.messages import Roles
+
+
+class MessagesFormatterType(Enum):
+    """
+    Enum representing different types of predefined messages formatters.
+    """
+
+    MISTRAL = 1
+    CHATML = 2
+    VICUNA = 3
+    LLAMA_2 = 4
+    SYNTHIA = 5
+    NEURAL_CHAT = 6
+    SOLAR = 7
+    OPEN_CHAT = 8
+    ALPACA = 9
+    CODE_DS = 10
+    B22 = 11
+    LLAMA_3 = 12
+    PHI_3 = 13
+
+
+@dataclass
+class PromptMarkers:
+    start: str
+    end: str
+
+
+class MessagesFormatter:
+    def __init__(
+            self,
+            pre_prompt: str,
+            prompt_markers: Dict[Roles, PromptMarkers],
+            include_sys_prompt_in_first_user_message: bool,
+            default_stop_sequences: List[str],
+            use_user_role_for_function_call_result: bool = True,
+            strip_prompt: bool = True,
+            bos_token: str = "<s>",
+            eos_token: str = "</s>"
+    ):
+        self.pre_prompt = pre_prompt
+        self.prompt_markers = prompt_markers
+        self.include_sys_prompt_in_first_user_message = include_sys_prompt_in_first_user_message
+        self.default_stop_sequences = default_stop_sequences
+        self.use_user_role_for_function_call_result = use_user_role_for_function_call_result
+        self.strip_prompt = strip_prompt
+        self.bos_token = bos_token
+        self.eos_token = eos_token
+        self.added_system_prompt = False
+
+    def get_bos_token(self) -> str:
+        return self.bos_token
+
+    def format_conversation(
+            self,
+            messages: List[Dict[str, str]],
+            response_role: Literal[Roles.user, Roles.assistant] | None = None,
+    ) -> Tuple[str, Roles]:
+        formatted_messages = self.pre_prompt
+        last_role = Roles.assistant
+        self.added_system_prompt = False
+        for message in messages:
+            role = Roles(message["role"])
+            content = self._format_message_content(message["content"], role)
+
+            if role == Roles.system:
+                formatted_messages += self._format_system_message(content)
+                last_role = Roles.system
+            elif role == Roles.user:
+                formatted_messages += self._format_user_message(content)
+                last_role = Roles.user
+            elif role == Roles.assistant:
+                formatted_messages += self._format_assistant_message(content)
+                last_role = Roles.assistant
+            elif role == Roles.tool:
+                formatted_messages += self._format_tool_message(content)
+                last_role = Roles.tool
+
+        return self._format_response(formatted_messages, last_role, response_role)
+
+    def _format_message_content(self, content: str, role: Roles) -> str:
+        if self.strip_prompt and role != Roles.tool:
+            return content.strip()
+        return content
+
+    def _format_system_message(self, content: str) -> str:
+        formatted_message = self.prompt_markers[Roles.system].start + content + self.prompt_markers[Roles.system].end
+        self.added_system_prompt = True
+        if self.include_sys_prompt_in_first_user_message:
+            formatted_message = self.prompt_markers[Roles.user].start + formatted_message
+        return formatted_message
+
+    def _format_user_message(self, content: str) -> str:
+        if self.include_sys_prompt_in_first_user_message and self.added_system_prompt:
+            return content + self.prompt_markers[Roles.user].end
+        return self.prompt_markers[Roles.user].start + content + self.prompt_markers[Roles.user].end
+
+    def _format_assistant_message(self, content: str) -> str:
+        return self.prompt_markers[Roles.assistant].start + content + self.prompt_markers[Roles.assistant].end
+
+    def _format_tool_message(self, content: str) -> str:
+        if isinstance(content, list):
+            content = "\n".join(json.dumps(m, indent=2) for m in content)
+        if self.use_user_role_for_function_call_result:
+            return self._format_user_message(content)
+        else:
+            return self.prompt_markers[Roles.tool].start + content + self.prompt_markers[Roles.tool].end
+
+    def _format_response(
+            self,
+            formatted_messages: str,
+            last_role: Roles,
+            response_role: Literal[Roles.user, Roles.assistant] | None = None,
+    ) -> Tuple[str, Roles]:
+        if response_role is None:
+            response_role = Roles.assistant if last_role != Roles.assistant else Roles.user
+
+        prompt_start = self.prompt_markers[response_role].start.strip() if self.strip_prompt else self.prompt_markers[
+            response_role].start
+        return formatted_messages + prompt_start, response_role
+
+
+mixtral_prompt_markers = {
+    Roles.system: PromptMarkers("", """\n\n"""),
+    Roles.user: PromptMarkers("""[INST] """, """ """),
+    Roles.assistant: PromptMarkers("""[/INST]""", """</s>"""),
+    Roles.tool: PromptMarkers("", ""),
+}
+
+chatml_prompt_markers = {
+    Roles.system: PromptMarkers("""<|im_start|>system\n""", """<|im_end|>\n"""),
+    Roles.user: PromptMarkers("""<|im_start|>user\n""", """<|im_end|>\n"""),
+    Roles.assistant: PromptMarkers("""<|im_start|>assistant\n""", """<|im_end|>\n"""),
+    Roles.tool: PromptMarkers("""<|im_start|>function\n""", """<|im_end|>\n"""),
+}
+
+vicuna_prompt_markers = {
+    Roles.system: PromptMarkers("", """\n\n"""),
+    Roles.user: PromptMarkers("""USER:""", """\n"""),
+    Roles.assistant: PromptMarkers("""ASSISTANT:""", ""),
+    Roles.tool: PromptMarkers("", ""),
+}
+
+llama_2_prompt_markers = {
+    Roles.system: PromptMarkers("<<SYS>>\n", "\n<</SYS>>\n\n"),
+    Roles.user: PromptMarkers("[INST] ", " [/INST]"),
+    Roles.assistant: PromptMarkers(" ", " </s>"),
+    Roles.tool: PromptMarkers("", ""),
+}
+
+llama_3_prompt_markers = {
+    Roles.system: PromptMarkers("""<|start_header_id|>system<|end_header_id|>\n""", """<|eot_id|>"""),
+    Roles.user: PromptMarkers("""<|start_header_id|>user<|end_header_id|>\n""", """<|eot_id|>"""),
+    Roles.assistant: PromptMarkers("""<|start_header_id|>assistant<|end_header_id|>\n""", """<|eot_id|>"""),
+    Roles.tool: PromptMarkers("""<|start_header_id|>function_calling_results<|end_header_id|>\n""", """<|eot_id|>"""),
+}
+
+synthia_prompt_markers = {
+    Roles.system: PromptMarkers("""SYSTEM: """, """\n"""),
+    Roles.user: PromptMarkers("""USER: """, """\n"""),
+    Roles.assistant: PromptMarkers("""ASSISTANT:""", """\n"""),
+    Roles.tool: PromptMarkers("", ""),
+}
+
+neural_chat_prompt_markers = {
+    Roles.system: PromptMarkers("""### System:\n""", """\n"""),
+    Roles.user: PromptMarkers("""### User:\n""", """ \n"""),
+    Roles.assistant: PromptMarkers("""### Assistant:\n""", """\n"""),
+    Roles.tool: PromptMarkers("", ""),
+}
+
+code_ds_prompt_markers = {
+    Roles.system: PromptMarkers("", """\n\n"""),
+    Roles.user: PromptMarkers("""@@ Instruction\n""", """\n\n"""),
+    Roles.assistant: PromptMarkers("""@@ Response\n""", """\n\n"""),
+    Roles.tool: PromptMarkers("", ""),
+}
+
+solar_prompt_markers = {
+    Roles.system: PromptMarkers("", """\n"""),
+    Roles.user: PromptMarkers("""### User:\n""", """ \n"""),
+    Roles.assistant: PromptMarkers("""### Assistant:\n""", """\n"""),
+    Roles.tool: PromptMarkers("", ""),
+}
+
+open_chat_prompt_markers = {
+    Roles.system: PromptMarkers("", """  """),
+    Roles.user: PromptMarkers("""GPT4 Correct User: """, """<|end_of_turn|>"""),
+    Roles.assistant: PromptMarkers("""GPT4 Correct Assistant: """, """<|end_of_turn|>"""),
+    Roles.tool: PromptMarkers("", ""),
+}
+
+alpaca_prompt_markers = {
+    Roles.system: PromptMarkers("""### Instruction:\n""", """\n"""),
+    Roles.user: PromptMarkers("""### Input:\n""", """ \n"""),
+    Roles.assistant: PromptMarkers("""### Response:\n""", """\n"""),
+    Roles.tool: PromptMarkers("""<|im_start|>function\n""", """<|im_end|>\n"""),
+}
+
+b22_chat_prompt_markers = {
+    Roles.system: PromptMarkers("""### System: """, """\n"""),
+    Roles.user: PromptMarkers("""### User: """, """ \n"""),
+    Roles.assistant: PromptMarkers("""### Assistant:""", """\n"""),
+    Roles.tool: PromptMarkers("", ""),
+}
+
+phi_3_chat_prompt_markers = {
+    Roles.system: PromptMarkers("", """\n\n"""),
+    Roles.user: PromptMarkers("""<|user|>""", """<|end|>\n"""),
+    Roles.assistant: PromptMarkers("""<|assistant|>""", """<|end|>\n"""),
+    Roles.tool: PromptMarkers("", ""),
+}
+
+mixtral_formatter = MessagesFormatter(
+    "",
+    mixtral_prompt_markers,
+    True,
+    ["</s>"],
+)
+
+chatml_formatter = MessagesFormatter(
+    "",
+    chatml_prompt_markers,
+    False,
+    ["<|im_end|>", "</s>"],
+    use_user_role_for_function_call_result=False,
+    strip_prompt=False,
+)
+
+vicuna_formatter = MessagesFormatter(
+    "",
+    vicuna_prompt_markers,
+    False,
+    ["</s>", "USER:"],
+)
+
+llama_2_formatter = MessagesFormatter(
+    "",
+    llama_2_prompt_markers,
+    True,
+    ["</s>", "[INST]"],
+)
+
+llama_3_formatter = MessagesFormatter(
+    "",
+    llama_3_prompt_markers,
+    False,
+    ["assistant", "<|eot_id|>"],
+    use_user_role_for_function_call_result=False,
+    strip_prompt=True,
+)
+
+synthia_formatter = MessagesFormatter(
+    "",
+    synthia_prompt_markers,
+    False,
+    ["</s>", "USER:"],
+)
+
+neural_chat_formatter = MessagesFormatter(
+    "",
+    neural_chat_prompt_markers,
+    False,
+    ["### User:"],
+    strip_prompt=False,
+)
+
+code_ds_formatter = MessagesFormatter(
+    "",
+    code_ds_prompt_markers,
+    True,
+    ["@@ Instruction"],
+)
+
+solar_formatter = MessagesFormatter(
+    "",
+    solar_prompt_markers,
+    True,
+    ["### User:"],
+)
+
+open_chat_formatter = MessagesFormatter(
+    "",
+    open_chat_prompt_markers,
+    True,
+    ["<|end_of_turn|>"],
+    use_user_role_for_function_call_result=True,
+)
+
+alpaca_formatter = MessagesFormatter(
+    "",
+    alpaca_prompt_markers,
+    False,
+    ["### Instruction:", "### Input:", "### Response:"],
+    use_user_role_for_function_call_result=False,
+)
+
+b22_chat_formatter = MessagesFormatter(
+    "",
+    b22_chat_prompt_markers,
+    False,
+    ["### User:"],
+    strip_prompt=False,
+)
+
+phi_3_chat_formatter = MessagesFormatter(
+    "",
+    phi_3_chat_prompt_markers,
+    True,
+    ["<|end|>", "<|end_of_turn|>"],
+    use_user_role_for_function_call_result=True,
+)
+
+predefined_formatter = {
+    MessagesFormatterType.MISTRAL: mixtral_formatter,
+    MessagesFormatterType.CHATML: chatml_formatter,
+    MessagesFormatterType.VICUNA: vicuna_formatter,
+    MessagesFormatterType.LLAMA_2: llama_2_formatter,
+    MessagesFormatterType.SYNTHIA: synthia_formatter,
+    MessagesFormatterType.NEURAL_CHAT: neural_chat_formatter,
+    MessagesFormatterType.SOLAR: solar_formatter,
+    MessagesFormatterType.OPEN_CHAT: open_chat_formatter,
+    MessagesFormatterType.ALPACA: alpaca_formatter,
+    MessagesFormatterType.CODE_DS: code_ds_formatter,
+    MessagesFormatterType.B22: b22_chat_formatter,
+    MessagesFormatterType.LLAMA_3: llama_3_formatter,
+    MessagesFormatterType.PHI_3: phi_3_chat_formatter,
+}
+
+
+def get_predefined_messages_formatter(
+        formatter_type: MessagesFormatterType,
+) -> MessagesFormatter:
+    """
+    Gets a predefined messages formatter based on the formatter type.
+
+    Args:
+        formatter_type (MessagesFormatterType): The type of messages formatter.
+
+    Returns:
+        MessagesFormatter: The predefined messages formatter.
+    """
+    return predefined_formatter[formatter_type]
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/mixtral_8x22b_agent.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/mixtral_8x22b_agent.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import json
-import random
-import string
-import uuid
-from enum import Enum
-
-from llama_cpp import Llama
-from mistral_common.protocol.instruct.messages import (
-    UserMessage,
-    SystemMessage,
-    AssistantMessage,
-    ToolMessage,
-)
-from mistral_common.protocol.instruct.request import ChatCompletionRequest
-from mistral_common.protocol.instruct.tool_calls import ToolCall, FunctionCall
-from mistral_common.tokens.tokenizers.mistral import MistralTokenizer
-
-
-from llama_cpp_agent.function_calling import LlamaCppFunctionTool
-from llama_cpp_agent.llm_agent import LlamaCppAgent
-from llama_cpp_agent.providers.provider_base import LlmProvider, LlmSamplingSettings
-
-
-def generate_id(length=8):
-    # Characters to use in the ID
-    characters = string.ascii_letters + string.digits
-    # Random choice of characters
-    return "".join(random.choice(characters) for _ in range(length))
-
-
-class Mixtral8x22BAgent:
-    def __init__(
-        self,
-        provider: LlmProvider,
-        system_prompt: str = None,
-        debug_output: bool = False,
-    ):
-        self.messages: list[
-            SystemMessage | UserMessage | AssistantMessage | ToolMessage
-        ] = []
-        self.agent = LlamaCppAgent(provider, debug_output=debug_output)
-        self.debug_output = debug_output
-        if system_prompt is not None:
-            self.messages.append(SystemMessage(content=system_prompt))
-        self.tokenizer_v3 = MistralTokenizer.v3()
-
-    def get_response(
-        self,
-        message=None,
-        tools: list[LlamaCppFunctionTool] = None,
-        llm_sampling_settings: LlmSamplingSettings = None,
-    ):
-        if tools is None:
-            tools = []
-        if message is not None:
-            msg = UserMessage(content=message)
-            self.messages.append(msg)
-        mistral_tools = []
-        mistral_tool_mapping = {}
-        for tool in tools:
-            mistral_tools.append(tool.to_mistral_tool())
-            mistral_tool_mapping[tool.model.__name__] = tool
-        request = ChatCompletionRequest(
-            tools=mistral_tools,
-            messages=self.messages,
-            model="open-mixtral-8x22b",
-        )
-        tokenized = self.tokenizer_v3.encode_chat_completion(request)
-        tokens, text = tokenized.tokens, tokenized.text
-        if self.debug_output:
-            print(text)
-        result = self.agent.get_text_response(
-            text,
-            llm_sampling_settings=llm_sampling_settings,
-            print_output=self.debug_output,
-        )
-
-        if result.strip().startswith("[TOOL_CALLS]"):
-            tool_calls = []
-
-            result = result.replace("[TOOL_CALLS]", "")
-            function_calls = json.loads(result.strip())
-            tool_messages = []
-            for function_call in function_calls:
-                tool = mistral_tool_mapping[function_call["name"]]
-                cls = tool.model
-                call_parameters = function_call["arguments"]
-                call = cls(**call_parameters)
-                output = call.run(**tool.additional_parameters)
-                tool_call_id = generate_id(length=9)
-                tool_calls.append(
-                    ToolCall(
-                        function=FunctionCall(
-                            name=function_call["name"],
-                            arguments=json.dumps(call_parameters),
-                        ),
-                        id=tool_call_id,
-                    )
-                )
-                tool_messages.append(
-                    ToolMessage(content=str(output), tool_call_id=tool_call_id)
-                )
-            self.messages.append(AssistantMessage(content=None, tool_calls=tool_calls))
-            self.messages.extend(tool_messages)
-            return self.get_response()
-        else:
-            self.messages.append(AssistantMessage(content=result.strip()))
-            return result.strip()
+import json
+import random
+import string
+import uuid
+from enum import Enum
+
+from llama_cpp import Llama
+from mistral_common.protocol.instruct.messages import (
+    UserMessage,
+    SystemMessage,
+    AssistantMessage,
+    ToolMessage,
+)
+from mistral_common.protocol.instruct.request import ChatCompletionRequest
+from mistral_common.protocol.instruct.tool_calls import ToolCall, FunctionCall
+from mistral_common.tokens.tokenizers.mistral import MistralTokenizer
+
+
+from llama_cpp_agent.function_calling import LlamaCppFunctionTool
+from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.providers.provider_base import LlmProvider, LlmSamplingSettings
+
+
+def generate_id(length=8):
+    # Characters to use in the ID
+    characters = string.ascii_letters + string.digits
+    # Random choice of characters
+    return "".join(random.choice(characters) for _ in range(length))
+
+
+class Mixtral8x22BAgent:
+    def __init__(
+        self,
+        provider: LlmProvider,
+        system_prompt: str = None,
+        debug_output: bool = False,
+    ):
+        self.messages: list[
+            SystemMessage | UserMessage | AssistantMessage | ToolMessage
+        ] = []
+        self.agent = LlamaCppAgent(provider, debug_output=debug_output)
+        self.debug_output = debug_output
+        if system_prompt is not None:
+            self.messages.append(SystemMessage(content=system_prompt))
+        self.tokenizer_v3 = MistralTokenizer.v3()
+
+    def get_response(
+        self,
+        message=None,
+        tools: list[LlamaCppFunctionTool] = None,
+        llm_sampling_settings: LlmSamplingSettings = None,
+    ):
+        if tools is None:
+            tools = []
+        if message is not None:
+            msg = UserMessage(content=message)
+            self.messages.append(msg)
+        mistral_tools = []
+        mistral_tool_mapping = {}
+        for tool in tools:
+            mistral_tools.append(tool.to_mistral_tool())
+            mistral_tool_mapping[tool.model.__name__] = tool
+        request = ChatCompletionRequest(
+            tools=mistral_tools,
+            messages=self.messages,
+            model="open-mixtral-8x22b",
+        )
+        tokenized = self.tokenizer_v3.encode_chat_completion(request)
+        tokens, text = tokenized.tokens, tokenized.text
+        if self.debug_output:
+            print(text)
+        result = self.agent.get_text_response(
+            text,
+            llm_sampling_settings=llm_sampling_settings,
+            print_output=self.debug_output,
+        )
+
+        if result.strip().startswith("[TOOL_CALLS]"):
+            tool_calls = []
+
+            result = result.replace("[TOOL_CALLS]", "")
+            function_calls = json.loads(result.strip())
+            tool_messages = []
+            for function_call in function_calls:
+                tool = mistral_tool_mapping[function_call["name"]]
+                cls = tool.model
+                call_parameters = function_call["arguments"]
+                call = cls(**call_parameters)
+                output = call.run(**tool.additional_parameters)
+                tool_call_id = generate_id(length=9)
+                tool_calls.append(
+                    ToolCall(
+                        function=FunctionCall(
+                            name=function_call["name"],
+                            arguments=json.dumps(call_parameters),
+                        ),
+                        id=tool_call_id,
+                    )
+                )
+                tool_messages.append(
+                    ToolMessage(content=str(output), tool_call_id=tool_call_id)
+                )
+            self.messages.append(AssistantMessage(content=None, tool_calls=tool_calls))
+            self.messages.extend(tool_messages)
+            return self.get_response()
+        else:
+            self.messages.append(AssistantMessage(content=result.strip()))
+            return result.strip()
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/output_parser.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/output_parser.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-import json
-import re
-
-
-def preprocess_json_string(json_string):
-    # Regular expression to find string values in JSON (this is a simplification and might not cover all edge cases)
-    string_regex = r'"([^"]*)"'
-
-    # Function to escape newlines within string values
-    def escape_newlines(match):
-        escaped_string = match.group(0).replace("\n", "\\n")
-        return escaped_string
-
-    # Replace unescaped newlines in string values
-    processed_string = re.sub(string_regex, escape_newlines, json_string)
-    return processed_string
-
-
-def sanitize_and_load_json(input_json):
-    fixed_json = preprocess_json_string(input_json)
-    fixed_json = fixed_json.replace("\r", "\\r")
-
-    try:
-        return json.loads(fixed_json)
-    except json.JSONDecodeError as e:
-        print(f"Error parsing JSON: {e}")
-        return None
-
-
-def is_empty_or_whitespace(s):
-    """
-    Checks if a string is empty or contains only whitespace.
-
-    Args:
-        s (str): The input string.
-
-    Returns:
-        bool: True if the string is empty or contains only whitespace, False otherwise.
-    """
-    return not s.strip()
-
-
-def parse_json_response(response: str):
-    """
-    Parses a JSON response string.
-
-    Args:
-        response (str): The JSON response string.
-
-    Returns:
-        dict: The parsed JSON object.
-    """
-
-    response_lines = response.split("\n")
-    while is_empty_or_whitespace(response_lines[0]):
-        response_lines.pop(0)
-    response = "\n".join(response_lines)
-    json_object = sanitize_and_load_json(response.strip())
-    return json_object
-
-
-def parse_json_response_with_markdown_code_block_or_triple_quoted_string(
-    json_response, marker
-):
-    """
-    Parses a JSON response string followed by a Markdown code block or triple-quoted string.
-
-    Args:
-        json_response (str): The JSON response string followed by a Markdown code block or triple-quoted string.
-        marker(str): Triple quotes (''') or triple back ticks (```)
-
-    Returns:
-        Tuple[dict, str]: The parsed JSON object and the content of the Markdown code block or triple-quoted string.
-    """
-    response_lines = json_response.split("\n")
-
-    if is_empty_or_whitespace(response_lines[0]):
-        response_lines.pop(0)
-
-    # Get the first line JSON object
-    response = response_lines[0]
-    # Remove the first line
-    response_lines.pop(0)
-    count = len(response_lines)
-    for _ in range(count):
-        if response_lines[0].startswith(marker):
-            break
-        else:
-            line = response_lines.pop(0)
-            response += "\n" + line
-
-    if len(response_lines) == 0:
-        return None, None
-    # Remove the first line Markdown code block marker
-    response_lines.pop(0)
-    # Remove the last line Markdown code block marker
-    response_lines.pop(-1)
-    response_lines.pop(-1)
-    # Combine lines into a single string
-    markdown_code_block_content = "\n".join(response_lines)
-    json_object = parse_json_response(response)
-
-    return json_object, markdown_code_block_content
-
-
-def extract_object_from_response(response: str, object_clas: type):
-    """
-    Extracts an object of the specified class from a JSON response string.
-
-    Args:
-        response (str): The JSON response string.
-        object_clas (type): The class of the object to be extracted.
-
-    Returns:
-        object_clas: An instance of the specified class.
-    """
-    obj = parse_json_response(response)
-    cls = object_clas
-    obj = cls(**obj)
-    return obj
+import json
+import re
+
+
+def preprocess_json_string(json_string):
+    # Regular expression to find string values in JSON (this is a simplification and might not cover all edge cases)
+    string_regex = r'"([^"]*)"'
+
+    # Function to escape newlines within string values
+    def escape_newlines(match):
+        escaped_string = match.group(0).replace("\n", "\\n")
+        return escaped_string
+
+    # Replace unescaped newlines in string values
+    processed_string = re.sub(string_regex, escape_newlines, json_string)
+    return processed_string
+
+
+def sanitize_and_load_json(input_json):
+    fixed_json = preprocess_json_string(input_json)
+    fixed_json = fixed_json.replace("\r", "\\r")
+
+    try:
+        return json.loads(fixed_json)
+    except json.JSONDecodeError as e:
+        print(f"Error parsing JSON: {e}")
+        return None
+
+
+def is_empty_or_whitespace(s):
+    """
+    Checks if a string is empty or contains only whitespace.
+
+    Args:
+        s (str): The input string.
+
+    Returns:
+        bool: True if the string is empty or contains only whitespace, False otherwise.
+    """
+    return not s.strip()
+
+
+def parse_json_response(response: str):
+    """
+    Parses a JSON response string.
+
+    Args:
+        response (str): The JSON response string.
+
+    Returns:
+        dict: The parsed JSON object.
+    """
+
+    response_lines = response.split("\n")
+    while is_empty_or_whitespace(response_lines[0]):
+        response_lines.pop(0)
+    response = "\n".join(response_lines)
+    json_object = sanitize_and_load_json(response.strip())
+    return json_object
+
+
+def parse_json_response_with_markdown_code_block_or_triple_quoted_string(
+    json_response, marker
+):
+    """
+    Parses a JSON response string followed by a Markdown code block or triple-quoted string.
+
+    Args:
+        json_response (str): The JSON response string followed by a Markdown code block or triple-quoted string.
+        marker(str): Triple quotes (''') or triple back ticks (```)
+
+    Returns:
+        Tuple[dict, str]: The parsed JSON object and the content of the Markdown code block or triple-quoted string.
+    """
+    response_lines = json_response.split("\n")
+
+    if is_empty_or_whitespace(response_lines[0]):
+        response_lines.pop(0)
+
+    # Get the first line JSON object
+    response = response_lines[0]
+    # Remove the first line
+    response_lines.pop(0)
+    count = len(response_lines)
+    for _ in range(count):
+        if response_lines[0].startswith(marker):
+            break
+        else:
+            line = response_lines.pop(0)
+            response += "\n" + line
+
+    if len(response_lines) == 0:
+        return None, None
+    # Remove the first line Markdown code block marker
+    response_lines.pop(0)
+    # Remove the last line Markdown code block marker
+    response_lines.pop(-1)
+    response_lines.pop(-1)
+    # Combine lines into a single string
+    markdown_code_block_content = "\n".join(response_lines)
+    json_object = parse_json_response(response)
+
+    return json_object, markdown_code_block_content
+
+
+def extract_object_from_response(response: str, object_clas: type):
+    """
+    Extracts an object of the specified class from a JSON response string.
+
+    Args:
+        response (str): The JSON response string.
+        object_clas (type): The class of the object to be extracted.
+
+    Returns:
+        object_clas: An instance of the specified class.
+    """
+    obj = parse_json_response(response)
+    cls = object_clas
+    obj = cls(**obj)
+    return obj
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/prompt_templates.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/prompt_templates.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-function_calling_thoughts_and_reasoning = '''\n\nYou can call functions to help you with your tasks and user queries. To call functions, you respond with a JSON object containing three fields:
-                        
-"thoughts_and_reasoning": Your thoughts and reasoning behind the function call.
-"function": The name of the function you want to call.
-"arguments": The arguments required for the function.
-
-After performing a function call, you will receive a response containing the return values of the function calls. Only you will see the return values of functions after you call them.
-
-### Functions:
-Below is a list of functions you can use to interact with the system. Each function has specific parameters and requirements. Make sure to follow the instructions for each function carefully.
-Choose the appropriate function based on the task you want to perform. Provide your function calls in JSON format.
-
-'''
-
-function_calling_without_thoughts_and_reasoning = '''\n\nYou can call functions to help you with your tasks and user queries. To call functions, you respond with a JSON object containing two fields:
-                        
-"function": The name of the function you want to call.
-"arguments": The arguments required for the function.
-
-After performing a function call, you will receive a response containing the return values of the function calls. Only you will see the return values of functions after you call them.
-
-### Functions:
-Below is a list of functions you can use to interact with the system. Each function has specific parameters and requirements. Make sure to follow the instructions for each function carefully.
-Choose the appropriate function based on the task you want to perform. Provide your function calls in JSON format.
-
-'''
-
-
-function_calling_thoughts_and_reasoning_json_schema = '''\n\nYou can call functions to help you with your tasks and user queries. To call functions, you respond with a JSON object containing three fields:
-                        
-"001_thoughts_and_reasoning": Your thoughts and reasoning behind the function call.
-"002_function": The name of the function you want to call.
-"003_arguments": The arguments required for the function.
-
-After performing a function call, you will receive a response containing the return values of the function calls. Only you will see the return values of functions after you call them.
-
-### Functions:
-Below is a list of functions you can use to interact with the system. Each function has specific parameters and requirements. Make sure to follow the instructions for each function carefully.
-Choose the appropriate function based on the task you want to perform. Provide your function calls in JSON format.
-
-'''
-
-function_calling_without_thoughts_and_reasoning_json_schema = '''\n\nYou can call functions to help you with your tasks and user queries. To call functions, you respond with a JSON object containing two fields:
-                        
-"001_function": The name of the function you want to call.
-"002_arguments": The arguments required for the function.
-
-After performing a function call, you will receive a response containing the return values of the function calls. Only you will see the return values of functions after you call them.
-
-### Functions:
-Below is a list of functions you can use to interact with the system. Each function has specific parameters and requirements. Make sure to follow the instructions for each function carefully.
-Choose the appropriate function based on the task you want to perform. Provide your function calls in JSON format.
-
-'''
-
-
-structured_output_thoughts_and_reasoning = '''\n\nYour output is constrained to JSON objects containing the content of specific models, each JSON object has three fields:
-                        
-"thoughts_and_reasoning": Your thoughts and reasoning behind the model you will output.
-"model": The name of the model you will output.
-"fields": The fields of the model.
-
-You can generate the following output models in JSON format:
-
-'''
-
-structured_output_without_thoughts_and_reasoning = '''\n\nYour output is constrained to JSON objects containing the content of specific models, each JSON object has two fields:
-                        
-"model": The name of the model you will output.
-"fields": The fields of the model.
-
-You can generate the following output models in JSON format:
-
-'''
-
-
-structured_output_thoughts_and_reasoning_json_schema = '''\n\nYour output is constrained to JSON objects containing the content of specific models, each JSON object has three fields:
-                        
-"001_thoughts_and_reasoning": Your thoughts and reasoning behind the model you will output.
-"002_model": The name of the model you will output.
-"003_fields": The fields of the model.
-
-You can generate the following output models in JSON format:
-
-'''
-
-structured_output_without_thoughts_and_reasoning_json_schema = '''\n\nYour output is constrained to JSON objects containing the content of specific models, each JSON object has two fields:
-                        
-"001_model": The name of the model you will output.
-"002_fields": The fields of the model.
-
-You can generate the following output models in JSON format:
-
-'''
+function_calling_thoughts_and_reasoning = '''\n\nYou can call functions to help you with your tasks and user queries. To call functions, you respond with a JSON object containing three fields:
+                        
+"thoughts_and_reasoning": Your thoughts and reasoning behind the function call.
+"function": The name of the function you want to call.
+"arguments": The arguments required for the function.
+
+After performing a function call, you will receive a response containing the return values of the function calls. Only you will see the return values of functions after you call them.
+
+### Functions:
+Below is a list of functions you can use to interact with the system. Each function has specific parameters and requirements. Make sure to follow the instructions for each function carefully.
+Choose the appropriate function based on the task you want to perform. Provide your function calls in JSON format.
+
+'''
+
+function_calling_without_thoughts_and_reasoning = '''\n\nYou can call functions to help you with your tasks and user queries. To call functions, you respond with a JSON object containing two fields:
+                        
+"function": The name of the function you want to call.
+"arguments": The arguments required for the function.
+
+After performing a function call, you will receive a response containing the return values of the function calls. Only you will see the return values of functions after you call them.
+
+### Functions:
+Below is a list of functions you can use to interact with the system. Each function has specific parameters and requirements. Make sure to follow the instructions for each function carefully.
+Choose the appropriate function based on the task you want to perform. Provide your function calls in JSON format.
+
+'''
+
+
+function_calling_thoughts_and_reasoning_json_schema = '''\n\nYou can call functions to help you with your tasks and user queries. To call functions, you respond with a JSON object containing three fields:
+                        
+"001_thoughts_and_reasoning": Your thoughts and reasoning behind the function call.
+"002_function": The name of the function you want to call.
+"003_arguments": The arguments required for the function.
+
+After performing a function call, you will receive a response containing the return values of the function calls. Only you will see the return values of functions after you call them.
+
+### Functions:
+Below is a list of functions you can use to interact with the system. Each function has specific parameters and requirements. Make sure to follow the instructions for each function carefully.
+Choose the appropriate function based on the task you want to perform. Provide your function calls in JSON format.
+
+'''
+
+function_calling_without_thoughts_and_reasoning_json_schema = '''\n\nYou can call functions to help you with your tasks and user queries. To call functions, you respond with a JSON object containing two fields:
+                        
+"001_function": The name of the function you want to call.
+"002_arguments": The arguments required for the function.
+
+After performing a function call, you will receive a response containing the return values of the function calls. Only you will see the return values of functions after you call them.
+
+### Functions:
+Below is a list of functions you can use to interact with the system. Each function has specific parameters and requirements. Make sure to follow the instructions for each function carefully.
+Choose the appropriate function based on the task you want to perform. Provide your function calls in JSON format.
+
+'''
+
+
+structured_output_thoughts_and_reasoning = '''\n\nYour output is constrained to JSON objects containing the content of specific models, each JSON object has three fields:
+                        
+"thoughts_and_reasoning": Your thoughts and reasoning behind the model you will output.
+"model": The name of the model you will output.
+"fields": The fields of the model.
+
+You can generate the following output models in JSON format:
+
+'''
+
+structured_output_without_thoughts_and_reasoning = '''\n\nYour output is constrained to JSON objects containing the content of specific models, each JSON object has two fields:
+                        
+"model": The name of the model you will output.
+"fields": The fields of the model.
+
+You can generate the following output models in JSON format:
+
+'''
+
+
+structured_output_thoughts_and_reasoning_json_schema = '''\n\nYour output is constrained to JSON objects containing the content of specific models, each JSON object has three fields:
+                        
+"001_thoughts_and_reasoning": Your thoughts and reasoning behind the model you will output.
+"002_model": The name of the model you will output.
+"003_fields": The fields of the model.
+
+You can generate the following output models in JSON format:
+
+'''
+
+structured_output_without_thoughts_and_reasoning_json_schema = '''\n\nYour output is constrained to JSON objects containing the content of specific models, each JSON object has two fields:
+                        
+"001_model": The name of the model you will output.
+"002_fields": The fields of the model.
+
+You can generate the following output models in JSON format:
+
+'''
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/prompts.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/prompts.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-funky_prompt = """You are Funky, an AI assistant that calls functions to perform tasks.
-
-To call functions, you respond with a JSON object containing three fields:
-"001_thoughts_and_reasoning": Your thoughts and reasoning behind the function call.
-"002_function": The name of the function you want to call.
-"003_arguments": The arguments required for the function.
-
-After performing a function call, you will receive a response containing the return values of the function calls.
-
-### Functions:
-Below is a list of functions you can use to interact with the system. Each function has specific parameters and requirements. Make sure to follow the instructions for each function carefully.
+funky_prompt = """You are Funky, an AI assistant that calls functions to perform tasks.
+
+To call functions, you respond with a JSON object containing three fields:
+"001_thoughts_and_reasoning": Your thoughts and reasoning behind the function call.
+"002_function": The name of the function you want to call.
+"003_arguments": The arguments required for the function.
+
+After performing a function call, you will receive a response containing the return values of the function calls.
+
+### Functions:
+Below is a list of functions you can use to interact with the system. Each function has specific parameters and requirements. Make sure to follow the instructions for each function carefully.
 Choose the appropriate function based on the task you want to perform. Provide your function calls in JSON format."""
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/llama_cpp_python.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/providers/llama_cpp_python.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-import json
-from copy import deepcopy
-from dataclasses import dataclass
-from typing import List, Dict, Union
-
-from llama_cpp import Llama, LlamaGrammar
-
-from llama_cpp_agent.llm_output_settings import (
-    LlmStructuredOutputSettings,
-    LlmStructuredOutputType,
-)
-from llama_cpp_agent.providers.provider_base import (
-    LlmProvider,
-    LlmProviderId,
-    LlmSamplingSettings,
-)
-
-
-@dataclass
-class LlamaCppPythonSamplingSettings(LlmSamplingSettings):
-    """
-    Settings for generating completions using the Llama.cpp server.
-
-    Args:
-        temperature (float): Controls the randomness of the generated completions. Higher values make the output more random.
-        top_k (int): Controls the diversity of the top-k sampling. Higher values result in more diverse completions.
-        top_p (float): Controls the diversity of the nucleus sampling. Higher values result in more diverse completions.
-        min_p (float): Minimum probability for nucleus sampling. Lower values result in more focused completions.
-        max_tokens (int): Number of max tokens to generate.
-        stream (bool): Enable streaming for long completions.
-        additional_stop_sequences (List[str]): List of stop sequences to finish completion generation. The official stop sequences of the model get added automatically.
-        tfs_z (float): Controls the temperature for top frequent sampling.
-        typical_p (float): Typical probability for top frequent sampling.
-        repeat_penalty (float): Penalty for repeating tokens in completions.
-        presence_penalty (float): Penalty for presence of certain tokens.
-        frequency_penalty (float): Penalty based on token frequency.
-        mirostat_mode (int): Mirostat level.
-        mirostat_tau (float): Mirostat temperature.
-        mirostat_eta (float): Mirostat eta parameter.
-        seed (int): Seed for randomness. Set to -1 for no seed.
-
-
-    Attributes:
-        temperature (float): Controls the randomness of the generated completions. Higher values make the output more random.
-        top_k (int): Controls the diversity of the top-k sampling. Higher values result in more diverse completions.
-        top_p (float): Controls the diversity of the nucleus sampling. Higher values result in more diverse completions.
-        min_p (float): Minimum probability for nucleus sampling. Lower values result in more focused completions.
-        max_tokens (int): Number of max tokens to generate.
-        stream (bool): Enable streaming for long completions.
-        additional_stop_sequences (List[str]): List of stop sequences to finish completion generation. The official stop sequences of the model get added automatically.
-        tfs_z (float): Controls the temperature for top frequent sampling.
-        typical_p (float): Typical probability for top frequent sampling.
-        repeat_penalty (float): Penalty for repeating tokens in completions.
-        presence_penalty (float): Penalty for presence of certain tokens.
-        frequency_penalty (float): Penalty based on token frequency.
-        mirostat_mode (int): Mirostat level.
-        mirostat_tau (float): Mirostat temperature.
-        mirostat_eta (float): Mirostat eta parameter.
-        seed (int): Seed for randomness. Set to -1 for no seed.
-    Methods:
-        save(file_path: str): Save the settings to a file.
-        load_from_file(file_path: str) -> LlamaCppServerGenerationSettings: Load the settings from a file.
-        load_from_dict(settings: dict) -> LlamaCppServerGenerationSettings: Load the settings from a dictionary.
-        as_dict() -> dict: Convert the settings to a dictionary.
-
-    """
-
-    temperature: float = 0.8
-    top_k: int = 40
-    top_p: float = 0.95
-    min_p: float = 0.05
-    max_tokens: int = -1
-    stream: bool = False
-    additional_stop_sequences: List[str] = None
-    tfs_z: float = 1.0
-    typical_p: float = 1.0
-    repeat_penalty: float = 1.1
-    presence_penalty: float = 0.0
-    frequency_penalty: float = 0.0
-    mirostat_mode: int = 0
-    mirostat_tau: float = 5.0
-    mirostat_eta: float = 0.1
-    seed: int = -1
-
-    def get_provider_identifier(self) -> LlmProviderId:
-        return LlmProviderId.llama_cpp_server
-
-    def get_additional_stop_sequences(self) -> List[str]:
-        if self.additional_stop_sequences is None:
-            self.additional_stop_sequences = []
-        return self.additional_stop_sequences
-
-    def add_additional_stop_sequences(self, sequences: List[str]):
-        if self.additional_stop_sequences is None:
-            self.additional_stop_sequences = []
-        self.additional_stop_sequences.extend(sequences)
-
-    def is_streaming(self):
-        return self.stream
-
-    @staticmethod
-    def load_from_dict(settings: dict) -> "LlamaCppPythonSamplingSettings":
-        """
-        Load the settings from a dictionary.
-
-        Args:
-            settings (dict): The dictionary containing the settings.
-
-        Returns:
-            LlamaCppPythonSamplingSettings: The loaded settings.
-        """
-        return LlamaCppPythonSamplingSettings(**settings)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the settings to a dictionary.
-
-        Returns:
-            dict: The dictionary representation of the settings.
-        """
-        return self.__dict__
-
-
-class LlamaCppPythonProvider(LlmProvider):
-    def __init__(self, llama_model: Llama):
-        self.llama_model = llama_model
-        self.grammar_cache = {}
-
-    def is_using_json_schema_constraints(self):
-        return False
-
-    def get_provider_identifier(self) -> LlmProviderId:
-        return LlmProviderId.llama_cpp_python
-
-    def get_provider_default_settings(self) -> LlamaCppPythonSamplingSettings:
-        return LlamaCppPythonSamplingSettings()
-
-    def create_completion(
-        self,
-        prompt: str,
-        structured_output_settings: LlmStructuredOutputSettings,
-        settings: LlamaCppPythonSamplingSettings,
-        bos_token: str,
-    ):
-        grammar = None
-        if (
-            structured_output_settings.output_type
-            != LlmStructuredOutputType.no_structured_output
-        ):
-            grammar = structured_output_settings.get_gbnf_grammar()
-            if grammar in self.grammar_cache:
-                grammar = self.grammar_cache[grammar]
-            else:
-                self.grammar_cache[grammar] = LlamaGrammar.from_string(grammar)
-                grammar = self.grammar_cache[grammar]
-
-        settings_dictionary = deepcopy(settings.as_dict())
-
-        settings_dictionary["stop"] = settings_dictionary.pop(
-            "additional_stop_sequences"
-        )
-
-        return self.llama_model.create_completion(
-            prompt, grammar=grammar, **settings_dictionary
-        )
-
-    def create_chat_completion(
-        self,
-        messages: List[Dict[str, str]],
-        structured_output_settings: LlmStructuredOutputSettings,
-        settings: LlamaCppPythonSamplingSettings
-    ):
-        grammar = None
-        if (
-            structured_output_settings.output_type
-            != LlmStructuredOutputType.no_structured_output
-        ):
-            grammar = structured_output_settings.get_gbnf_grammar()
-            if grammar in self.grammar_cache:
-                grammar = self.grammar_cache[grammar]
-            else:
-                self.grammar_cache[grammar] = LlamaGrammar.from_string(grammar)
-                grammar = self.grammar_cache[grammar]
-        settings_dictionary = deepcopy(settings.as_dict())
-        settings_dictionary["max_tokens"] = settings_dictionary.pop("n_predict")
-        settings_dictionary["stop"] = settings_dictionary.pop("stop_sequences")
-
-        return self.llama_model.create_chat_completion(
-            messages, grammar=grammar, **settings_dictionary
-        )
-
-    def tokenize(self, prompt: str) -> list[int]:
-        return self.llama_model.tokenize(prompt.encode("utf-8"))
+import json
+from copy import deepcopy
+from dataclasses import dataclass
+from typing import List, Dict, Union
+
+from llama_cpp import Llama, LlamaGrammar
+
+from llama_cpp_agent.llm_output_settings import (
+    LlmStructuredOutputSettings,
+    LlmStructuredOutputType,
+)
+from llama_cpp_agent.providers.provider_base import (
+    LlmProvider,
+    LlmProviderId,
+    LlmSamplingSettings,
+)
+
+
+@dataclass
+class LlamaCppPythonSamplingSettings(LlmSamplingSettings):
+    """
+    Settings for generating completions using the Llama.cpp server.
+
+    Args:
+        temperature (float): Controls the randomness of the generated completions. Higher values make the output more random.
+        top_k (int): Controls the diversity of the top-k sampling. Higher values result in more diverse completions.
+        top_p (float): Controls the diversity of the nucleus sampling. Higher values result in more diverse completions.
+        min_p (float): Minimum probability for nucleus sampling. Lower values result in more focused completions.
+        max_tokens (int): Number of max tokens to generate.
+        stream (bool): Enable streaming for long completions.
+        additional_stop_sequences (List[str]): List of stop sequences to finish completion generation. The official stop sequences of the model get added automatically.
+        tfs_z (float): Controls the temperature for top frequent sampling.
+        typical_p (float): Typical probability for top frequent sampling.
+        repeat_penalty (float): Penalty for repeating tokens in completions.
+        presence_penalty (float): Penalty for presence of certain tokens.
+        frequency_penalty (float): Penalty based on token frequency.
+        mirostat_mode (int): Mirostat level.
+        mirostat_tau (float): Mirostat temperature.
+        mirostat_eta (float): Mirostat eta parameter.
+        seed (int): Seed for randomness. Set to -1 for no seed.
+
+
+    Attributes:
+        temperature (float): Controls the randomness of the generated completions. Higher values make the output more random.
+        top_k (int): Controls the diversity of the top-k sampling. Higher values result in more diverse completions.
+        top_p (float): Controls the diversity of the nucleus sampling. Higher values result in more diverse completions.
+        min_p (float): Minimum probability for nucleus sampling. Lower values result in more focused completions.
+        max_tokens (int): Number of max tokens to generate.
+        stream (bool): Enable streaming for long completions.
+        additional_stop_sequences (List[str]): List of stop sequences to finish completion generation. The official stop sequences of the model get added automatically.
+        tfs_z (float): Controls the temperature for top frequent sampling.
+        typical_p (float): Typical probability for top frequent sampling.
+        repeat_penalty (float): Penalty for repeating tokens in completions.
+        presence_penalty (float): Penalty for presence of certain tokens.
+        frequency_penalty (float): Penalty based on token frequency.
+        mirostat_mode (int): Mirostat level.
+        mirostat_tau (float): Mirostat temperature.
+        mirostat_eta (float): Mirostat eta parameter.
+        seed (int): Seed for randomness. Set to -1 for no seed.
+    Methods:
+        save(file_path: str): Save the settings to a file.
+        load_from_file(file_path: str) -> LlamaCppServerGenerationSettings: Load the settings from a file.
+        load_from_dict(settings: dict) -> LlamaCppServerGenerationSettings: Load the settings from a dictionary.
+        as_dict() -> dict: Convert the settings to a dictionary.
+
+    """
+
+    temperature: float = 0.8
+    top_k: int = 40
+    top_p: float = 0.95
+    min_p: float = 0.05
+    max_tokens: int = -1
+    stream: bool = False
+    additional_stop_sequences: List[str] = None
+    tfs_z: float = 1.0
+    typical_p: float = 1.0
+    repeat_penalty: float = 1.1
+    presence_penalty: float = 0.0
+    frequency_penalty: float = 0.0
+    mirostat_mode: int = 0
+    mirostat_tau: float = 5.0
+    mirostat_eta: float = 0.1
+    seed: int = -1
+
+    def get_provider_identifier(self) -> LlmProviderId:
+        return LlmProviderId.llama_cpp_server
+
+    def get_additional_stop_sequences(self) -> List[str]:
+        if self.additional_stop_sequences is None:
+            self.additional_stop_sequences = []
+        return self.additional_stop_sequences
+
+    def add_additional_stop_sequences(self, sequences: List[str]):
+        if self.additional_stop_sequences is None:
+            self.additional_stop_sequences = []
+        self.additional_stop_sequences.extend(sequences)
+
+    def is_streaming(self):
+        return self.stream
+
+    @staticmethod
+    def load_from_dict(settings: dict) -> "LlamaCppPythonSamplingSettings":
+        """
+        Load the settings from a dictionary.
+
+        Args:
+            settings (dict): The dictionary containing the settings.
+
+        Returns:
+            LlamaCppPythonSamplingSettings: The loaded settings.
+        """
+        return LlamaCppPythonSamplingSettings(**settings)
+
+    def as_dict(self) -> dict:
+        """
+        Convert the settings to a dictionary.
+
+        Returns:
+            dict: The dictionary representation of the settings.
+        """
+        return self.__dict__
+
+
+class LlamaCppPythonProvider(LlmProvider):
+    def __init__(self, llama_model: Llama):
+        self.llama_model = llama_model
+        self.grammar_cache = {}
+
+    def is_using_json_schema_constraints(self):
+        return False
+
+    def get_provider_identifier(self) -> LlmProviderId:
+        return LlmProviderId.llama_cpp_python
+
+    def get_provider_default_settings(self) -> LlamaCppPythonSamplingSettings:
+        return LlamaCppPythonSamplingSettings()
+
+    def create_completion(
+        self,
+        prompt: str,
+        structured_output_settings: LlmStructuredOutputSettings,
+        settings: LlamaCppPythonSamplingSettings,
+        bos_token: str,
+    ):
+        grammar = None
+        if (
+            structured_output_settings.output_type
+            != LlmStructuredOutputType.no_structured_output
+        ):
+            grammar = structured_output_settings.get_gbnf_grammar()
+            if grammar in self.grammar_cache:
+                grammar = self.grammar_cache[grammar]
+            else:
+                self.grammar_cache[grammar] = LlamaGrammar.from_string(grammar)
+                grammar = self.grammar_cache[grammar]
+
+        settings_dictionary = deepcopy(settings.as_dict())
+
+        settings_dictionary["stop"] = settings_dictionary.pop(
+            "additional_stop_sequences"
+        )
+
+        return self.llama_model.create_completion(
+            prompt, grammar=grammar, **settings_dictionary
+        )
+
+    def create_chat_completion(
+        self,
+        messages: List[Dict[str, str]],
+        structured_output_settings: LlmStructuredOutputSettings,
+        settings: LlamaCppPythonSamplingSettings
+    ):
+        grammar = None
+        if (
+            structured_output_settings.output_type
+            != LlmStructuredOutputType.no_structured_output
+        ):
+            grammar = structured_output_settings.get_gbnf_grammar()
+            if grammar in self.grammar_cache:
+                grammar = self.grammar_cache[grammar]
+            else:
+                self.grammar_cache[grammar] = LlamaGrammar.from_string(grammar)
+                grammar = self.grammar_cache[grammar]
+        settings_dictionary = deepcopy(settings.as_dict())
+        settings_dictionary["max_tokens"] = settings_dictionary.pop("n_predict")
+        settings_dictionary["stop"] = settings_dictionary.pop("stop_sequences")
+
+        return self.llama_model.create_chat_completion(
+            messages, grammar=grammar, **settings_dictionary
+        )
+
+    def tokenize(self, prompt: str) -> list[int]:
+        return self.llama_model.tokenize(prompt.encode("utf-8"))
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/llama_cpp_server.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/providers/llama_cpp_server.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,334 +1,334 @@
-import json
-from copy import deepcopy
-from dataclasses import dataclass
-from typing import List, Dict, Union
-
-import requests
-
-from llama_cpp_agent.llm_output_settings import (
-    LlmStructuredOutputType,
-    LlmStructuredOutputSettings,
-)
-from llama_cpp_agent.providers.provider_base import (
-    LlmProviderId,
-    LlmProvider,
-    LlmSamplingSettings,
-)
-
-
-@dataclass
-class LlamaCppSamplingSettings(LlmSamplingSettings):
-    """
-    Settings for generating completions using the Llama.cpp server.
-
-    Args:
-        temperature (float): Controls the randomness of the generated completions. Higher values make the output more random.
-        top_k (int): Controls the diversity of the top-k sampling. Higher values result in more diverse completions.
-        top_p (float): Controls the diversity of the nucleus sampling. Higher values result in more diverse completions.
-        min_p (float): Minimum probability for nucleus sampling. Lower values result in more focused completions.
-        n_predict (int): Number of completions to predict. Set to -1 to use the default value.
-        n_keep (int): Number of completions to keep. Set to 0 for all predictions.
-        stream (bool): Enable streaming for long completions.
-        additional_stop_sequences (List[str]): List of stop sequences to finish completion generation. The official stop sequences of the model get added automatically.
-        tfs_z (float): Controls the temperature for top frequent sampling.
-        typical_p (float): Typical probability for top frequent sampling.
-        repeat_penalty (float): Penalty for repeating tokens in completions.
-        repeat_last_n (int): Number of tokens to consider for repeat penalty.
-        penalize_nl (bool): Enable penalizing newlines in completions.
-        presence_penalty (float): Penalty for presence of certain tokens.
-        frequency_penalty (float): Penalty based on token frequency.
-        penalty_prompt (Union[None, str, List[int]]): Prompts to apply penalty for certain tokens.
-        mirostat_mode (int): Mirostat level.
-        mirostat_tau (float): Mirostat temperature.
-        mirostat_eta (float): Mirostat eta parameter.
-        seed (int): Seed for randomness. Set to -1 for no seed.
-        ignore_eos (bool): Ignore end-of-sequence token.
-
-    Attributes:
-        temperature (float): Controls the randomness of the generated completions. Higher values make the output more random.
-        top_k (int): Controls the diversity of the top-k sampling. Higher values result in more diverse completions.
-        top_p (float): Controls the diversity of the nucleus sampling. Higher values result in more diverse completions.
-        min_p (float): Minimum probability for nucleus sampling. Lower values result in more focused completions.
-        n_predict (int): Number of completions to predict. Set to -1 to use the default value.
-        n_keep (int): Number of completions to keep. Set to 0 for all predictions.
-        stream (bool): Enable streaming for long completions.
-        additional_stop_sequences (List[str]): List of stop sequences to finish completion generation. The official stop sequences of the model get added automatically.
-        tfs_z (float): Controls the temperature for top frequent sampling.
-        typical_p (float): Typical probability for top frequent sampling.
-        repeat_penalty (float): Penalty for repeating tokens in completions.
-        repeat_last_n (int): Number of tokens to consider for repeat penalty.
-        penalize_nl (bool): Enable penalizing newlines in completions.
-        presence_penalty (float): Penalty for presence of certain tokens.
-        frequency_penalty (float): Penalty based on token frequency.
-        penalty_prompt (Union[None, str, List[int]]): Prompts to apply penalty for certain tokens.
-        mirostat_mode (int): Mirostat level.
-        mirostat_tau (float): Mirostat temperature.
-        mirostat_eta (float): Mirostat eta parameter.
-        seed (int): Seed for randomness. Set to -1 for no seed.
-        ignore_eos (bool): Ignore end-of-sequence token.
-    Methods:
-        save(file_path: str): Save the settings to a file.
-        load_from_file(file_path: str) -> LlamaCppServerGenerationSettings: Load the settings from a file.
-        load_from_dict(settings: dict) -> LlamaCppServerGenerationSettings: Load the settings from a dictionary.
-        as_dict() -> dict: Convert the settings to a dictionary.
-
-    """
-
-    temperature: float = 0.8
-    top_k: int = 40
-    top_p: float = 0.95
-    min_p: float = 0.05
-    n_predict: int = -1
-    n_keep: int = 0
-    stream: bool = True
-    additional_stop_sequences: List[str] = None
-    tfs_z: float = 1.0
-    typical_p: float = 1.0
-    repeat_penalty: float = 1.1
-    repeat_last_n: int = -1
-    penalize_nl: bool = False
-    presence_penalty: float = 0.0
-    frequency_penalty: float = 0.0
-    penalty_prompt: Union[None, str, List[int]] = None
-    mirostat_mode: int = 0
-    mirostat_tau: float = 5.0
-    mirostat_eta: float = 0.1
-    cache_prompt: bool = True
-    seed: int = -1
-    ignore_eos: bool = False
-    samplers: List[str] = None
-
-    def get_provider_identifier(self) -> LlmProviderId:
-        return LlmProviderId.llama_cpp_server
-
-    def get_additional_stop_sequences(self) -> List[str]:
-        if self.additional_stop_sequences is None:
-            self.additional_stop_sequences = []
-        return self.additional_stop_sequences
-
-    def add_additional_stop_sequences(self, sequences: List[str]):
-        if self.additional_stop_sequences is None:
-            self.additional_stop_sequences = []
-        self.additional_stop_sequences.extend(sequences)
-
-    def is_streaming(self):
-        return self.stream
-
-    @staticmethod
-    def load_from_dict(settings: dict) -> "LlamaCppSamplingSettings":
-        """
-        Load the settings from a dictionary.
-
-        Args:
-            settings (dict): The dictionary containing the settings.
-
-        Returns:
-            LlamaCppSamplingSettings: The loaded settings.
-        """
-        return LlamaCppSamplingSettings(**settings)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the settings to a dictionary.
-
-        Returns:
-            dict: The dictionary representation of the settings.
-        """
-        return self.__dict__
-
-
-class LlamaCppServerProvider(LlmProvider):
-    def __init__(
-        self,
-        server_address: str,
-        api_key: str = None,
-        llama_cpp_python_server: bool = False,
-    ):
-        self.server_address = server_address
-        if llama_cpp_python_server:
-            self.server_completion_endpoint = (
-                self.server_address + "/v1/engines/copilot-codex/completions"
-            )
-        else:
-            self.server_completion_endpoint = self.server_address + "/completion"
-
-        self.server_chat_completion_endpoint = (
-            self.server_address + "/v1/chat/completions"
-        )
-        if llama_cpp_python_server:
-            self.server_tokenize_endpoint = self.server_address + "/extras/tokenize"
-        else:
-            self.server_tokenize_endpoint = self.server_address + "/tokenize"
-        self.api_key = api_key
-        self.llama_cpp_python_server = llama_cpp_python_server
-
-    def is_using_json_schema_constraints(self):
-        return False
-
-    def get_provider_identifier(self) -> LlmProviderId:
-        return LlmProviderId.llama_cpp_server
-
-    def get_provider_default_settings(self) -> LlamaCppSamplingSettings:
-        return LlamaCppSamplingSettings()
-
-    def create_completion(
-        self,
-        prompt: str,
-        structured_output_settings: LlmStructuredOutputSettings,
-        settings: LlamaCppSamplingSettings,
-        bos_token: str,
-    ):
-        if self.api_key is not None:
-            headers = {
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
-            }
-        else:
-            headers = {"Content-Type": "application/json"}
-
-        data = deepcopy(settings.as_dict())
-        data["prompt"] = prompt
-        data = self.prepare_generation_settings(data, structured_output_settings)
-
-        if settings.stream:
-            return self.get_response_stream(
-                headers, data, self.server_completion_endpoint
-            )
-
-        response = requests.post(
-            self.server_completion_endpoint, headers=headers, json=data
-        )
-        data = response.json()
-
-        returned_data = {"choices": [{"text": data["content"]}]}
-        return returned_data
-
-    def create_chat_completion(
-        self,
-        messages: List[Dict[str, str]],
-        structured_output_settings: LlmStructuredOutputSettings,
-        settings: LlamaCppSamplingSettings
-    ):
-        if self.api_key is not None:
-            headers = {
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
-            }
-        else:
-            headers = {"Content-Type": "application/json"}
-
-        data = deepcopy(settings.as_dict())
-        data["messages"] = messages
-        data = self.prepare_generation_settings(data, structured_output_settings)
-        if settings.stream:
-            return self.get_response_stream(
-                headers, data, self.server_chat_completion_endpoint
-            )
-        response = requests.post(
-            self.server_chat_completion_endpoint, headers=headers, json=data
-        )
-        data = response.json()
-
-        returned_data = data
-        return returned_data
-
-    def tokenize(self, prompt: str) -> list[int]:
-        if self.api_key is not None:
-            headers = {
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
-            }
-        else:
-            headers = {"Content-Type": "application/json"}
-        if self.llama_cpp_python_server:
-            response = requests.post(
-                self.server_tokenize_endpoint, headers=headers, json={"input": prompt}
-            )
-        else:
-            response = requests.post(
-                self.server_tokenize_endpoint, headers=headers, json={"content": prompt}
-            )
-        if response.status_code == 200:
-            tokens = response.json()["tokens"]
-            return tokens
-        else:
-            raise Exception(
-                f"Tokenization request failed. Status code: {response.status_code}\nResponse: {response.text}"
-            )
-
-    def get_response_stream(self, headers, data, endpoint_address):
-        response = requests.post(
-            endpoint_address,
-            headers=headers,
-            json=data,
-            stream=True,
-        )
-
-        # Check if the request was successful
-        response.raise_for_status()
-
-        # Define a generator function to yield text chunks
-        def generate_text_chunks():
-            try:
-                decoded_chunk = ""
-                for chunk in response.iter_lines():
-                    if chunk:
-                        decoded_chunk += chunk.decode("utf-8")
-                        if decoded_chunk.strip().startswith("error:"):
-                            raise RuntimeError(decoded_chunk)
-                        new_data = json.loads(decoded_chunk.replace("data:", ""))
-                        if self.llama_cpp_python_server:
-                            returned_data = new_data
-                        else:
-                            if "choices" not in new_data:
-                                returned_data = {
-                                    "choices": [{"text": new_data["content"]}]
-                                }
-                            else:
-                                returned_data = new_data
-                        yield returned_data
-                        decoded_chunk = ""
-
-            except requests.exceptions.RequestException as e:
-                print(f"Request failed: {e}")
-
-        return generate_text_chunks()
-
-    def prepare_generation_settings(
-        self,
-        settings_dictionary: dict,
-        structured_output_settings: LlmStructuredOutputSettings,
-    ) -> dict:
-        if (
-            structured_output_settings.output_type
-            != LlmStructuredOutputType.no_structured_output
-        ):
-            settings_dictionary[
-                "grammar"
-            ] = structured_output_settings.get_gbnf_grammar()
-        if not self.llama_cpp_python_server:
-            settings_dictionary["mirostat"] = settings_dictionary.pop("mirostat_mode")
-        if self.llama_cpp_python_server:
-            settings_dictionary["max_tokens"] = settings_dictionary.pop("n_predict")
-
-        settings_dictionary["stop"] = settings_dictionary.pop(
-            "additional_stop_sequences"
-        )
-        if not self.llama_cpp_python_server:
-            if (
-                "samplers" not in settings_dictionary
-                or settings_dictionary["samplers"] is None
-            ):
-                settings_dictionary["samplers"] = [
-                    "top_k",
-                    "tfs_z",
-                    "typical_p",
-                    "top_p",
-                    "min_p",
-                    "temperature",
-                ]
-        else:
-            if "samplers" in settings_dictionary:
-                del settings_dictionary["samplers"]
-
-        return settings_dictionary
+import json
+from copy import deepcopy
+from dataclasses import dataclass
+from typing import List, Dict, Union
+
+import requests
+
+from llama_cpp_agent.llm_output_settings import (
+    LlmStructuredOutputType,
+    LlmStructuredOutputSettings,
+)
+from llama_cpp_agent.providers.provider_base import (
+    LlmProviderId,
+    LlmProvider,
+    LlmSamplingSettings,
+)
+
+
+@dataclass
+class LlamaCppSamplingSettings(LlmSamplingSettings):
+    """
+    Settings for generating completions using the Llama.cpp server.
+
+    Args:
+        temperature (float): Controls the randomness of the generated completions. Higher values make the output more random.
+        top_k (int): Controls the diversity of the top-k sampling. Higher values result in more diverse completions.
+        top_p (float): Controls the diversity of the nucleus sampling. Higher values result in more diverse completions.
+        min_p (float): Minimum probability for nucleus sampling. Lower values result in more focused completions.
+        n_predict (int): Number of completions to predict. Set to -1 to use the default value.
+        n_keep (int): Number of completions to keep. Set to 0 for all predictions.
+        stream (bool): Enable streaming for long completions.
+        additional_stop_sequences (List[str]): List of stop sequences to finish completion generation. The official stop sequences of the model get added automatically.
+        tfs_z (float): Controls the temperature for top frequent sampling.
+        typical_p (float): Typical probability for top frequent sampling.
+        repeat_penalty (float): Penalty for repeating tokens in completions.
+        repeat_last_n (int): Number of tokens to consider for repeat penalty.
+        penalize_nl (bool): Enable penalizing newlines in completions.
+        presence_penalty (float): Penalty for presence of certain tokens.
+        frequency_penalty (float): Penalty based on token frequency.
+        penalty_prompt (Union[None, str, List[int]]): Prompts to apply penalty for certain tokens.
+        mirostat_mode (int): Mirostat level.
+        mirostat_tau (float): Mirostat temperature.
+        mirostat_eta (float): Mirostat eta parameter.
+        seed (int): Seed for randomness. Set to -1 for no seed.
+        ignore_eos (bool): Ignore end-of-sequence token.
+
+    Attributes:
+        temperature (float): Controls the randomness of the generated completions. Higher values make the output more random.
+        top_k (int): Controls the diversity of the top-k sampling. Higher values result in more diverse completions.
+        top_p (float): Controls the diversity of the nucleus sampling. Higher values result in more diverse completions.
+        min_p (float): Minimum probability for nucleus sampling. Lower values result in more focused completions.
+        n_predict (int): Number of completions to predict. Set to -1 to use the default value.
+        n_keep (int): Number of completions to keep. Set to 0 for all predictions.
+        stream (bool): Enable streaming for long completions.
+        additional_stop_sequences (List[str]): List of stop sequences to finish completion generation. The official stop sequences of the model get added automatically.
+        tfs_z (float): Controls the temperature for top frequent sampling.
+        typical_p (float): Typical probability for top frequent sampling.
+        repeat_penalty (float): Penalty for repeating tokens in completions.
+        repeat_last_n (int): Number of tokens to consider for repeat penalty.
+        penalize_nl (bool): Enable penalizing newlines in completions.
+        presence_penalty (float): Penalty for presence of certain tokens.
+        frequency_penalty (float): Penalty based on token frequency.
+        penalty_prompt (Union[None, str, List[int]]): Prompts to apply penalty for certain tokens.
+        mirostat_mode (int): Mirostat level.
+        mirostat_tau (float): Mirostat temperature.
+        mirostat_eta (float): Mirostat eta parameter.
+        seed (int): Seed for randomness. Set to -1 for no seed.
+        ignore_eos (bool): Ignore end-of-sequence token.
+    Methods:
+        save(file_path: str): Save the settings to a file.
+        load_from_file(file_path: str) -> LlamaCppServerGenerationSettings: Load the settings from a file.
+        load_from_dict(settings: dict) -> LlamaCppServerGenerationSettings: Load the settings from a dictionary.
+        as_dict() -> dict: Convert the settings to a dictionary.
+
+    """
+
+    temperature: float = 0.8
+    top_k: int = 40
+    top_p: float = 0.95
+    min_p: float = 0.05
+    n_predict: int = -1
+    n_keep: int = 0
+    stream: bool = True
+    additional_stop_sequences: List[str] = None
+    tfs_z: float = 1.0
+    typical_p: float = 1.0
+    repeat_penalty: float = 1.1
+    repeat_last_n: int = -1
+    penalize_nl: bool = False
+    presence_penalty: float = 0.0
+    frequency_penalty: float = 0.0
+    penalty_prompt: Union[None, str, List[int]] = None
+    mirostat_mode: int = 0
+    mirostat_tau: float = 5.0
+    mirostat_eta: float = 0.1
+    cache_prompt: bool = True
+    seed: int = -1
+    ignore_eos: bool = False
+    samplers: List[str] = None
+
+    def get_provider_identifier(self) -> LlmProviderId:
+        return LlmProviderId.llama_cpp_server
+
+    def get_additional_stop_sequences(self) -> List[str]:
+        if self.additional_stop_sequences is None:
+            self.additional_stop_sequences = []
+        return self.additional_stop_sequences
+
+    def add_additional_stop_sequences(self, sequences: List[str]):
+        if self.additional_stop_sequences is None:
+            self.additional_stop_sequences = []
+        self.additional_stop_sequences.extend(sequences)
+
+    def is_streaming(self):
+        return self.stream
+
+    @staticmethod
+    def load_from_dict(settings: dict) -> "LlamaCppSamplingSettings":
+        """
+        Load the settings from a dictionary.
+
+        Args:
+            settings (dict): The dictionary containing the settings.
+
+        Returns:
+            LlamaCppSamplingSettings: The loaded settings.
+        """
+        return LlamaCppSamplingSettings(**settings)
+
+    def as_dict(self) -> dict:
+        """
+        Convert the settings to a dictionary.
+
+        Returns:
+            dict: The dictionary representation of the settings.
+        """
+        return self.__dict__
+
+
+class LlamaCppServerProvider(LlmProvider):
+    def __init__(
+        self,
+        server_address: str,
+        api_key: str = None,
+        llama_cpp_python_server: bool = False,
+    ):
+        self.server_address = server_address
+        if llama_cpp_python_server:
+            self.server_completion_endpoint = (
+                self.server_address + "/v1/engines/copilot-codex/completions"
+            )
+        else:
+            self.server_completion_endpoint = self.server_address + "/completion"
+
+        self.server_chat_completion_endpoint = (
+            self.server_address + "/v1/chat/completions"
+        )
+        if llama_cpp_python_server:
+            self.server_tokenize_endpoint = self.server_address + "/extras/tokenize"
+        else:
+            self.server_tokenize_endpoint = self.server_address + "/tokenize"
+        self.api_key = api_key
+        self.llama_cpp_python_server = llama_cpp_python_server
+
+    def is_using_json_schema_constraints(self):
+        return False
+
+    def get_provider_identifier(self) -> LlmProviderId:
+        return LlmProviderId.llama_cpp_server
+
+    def get_provider_default_settings(self) -> LlamaCppSamplingSettings:
+        return LlamaCppSamplingSettings()
+
+    def create_completion(
+        self,
+        prompt: str,
+        structured_output_settings: LlmStructuredOutputSettings,
+        settings: LlamaCppSamplingSettings,
+        bos_token: str,
+    ):
+        if self.api_key is not None:
+            headers = {
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
+            }
+        else:
+            headers = {"Content-Type": "application/json"}
+
+        data = deepcopy(settings.as_dict())
+        data["prompt"] = prompt
+        data = self.prepare_generation_settings(data, structured_output_settings)
+
+        if settings.stream:
+            return self.get_response_stream(
+                headers, data, self.server_completion_endpoint
+            )
+
+        response = requests.post(
+            self.server_completion_endpoint, headers=headers, json=data
+        )
+        data = response.json()
+
+        returned_data = {"choices": [{"text": data["content"]}]}
+        return returned_data
+
+    def create_chat_completion(
+        self,
+        messages: List[Dict[str, str]],
+        structured_output_settings: LlmStructuredOutputSettings,
+        settings: LlamaCppSamplingSettings
+    ):
+        if self.api_key is not None:
+            headers = {
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
+            }
+        else:
+            headers = {"Content-Type": "application/json"}
+
+        data = deepcopy(settings.as_dict())
+        data["messages"] = messages
+        data = self.prepare_generation_settings(data, structured_output_settings)
+        if settings.stream:
+            return self.get_response_stream(
+                headers, data, self.server_chat_completion_endpoint
+            )
+        response = requests.post(
+            self.server_chat_completion_endpoint, headers=headers, json=data
+        )
+        data = response.json()
+
+        returned_data = data
+        return returned_data
+
+    def tokenize(self, prompt: str) -> list[int]:
+        if self.api_key is not None:
+            headers = {
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
+            }
+        else:
+            headers = {"Content-Type": "application/json"}
+        if self.llama_cpp_python_server:
+            response = requests.post(
+                self.server_tokenize_endpoint, headers=headers, json={"input": prompt}
+            )
+        else:
+            response = requests.post(
+                self.server_tokenize_endpoint, headers=headers, json={"content": prompt}
+            )
+        if response.status_code == 200:
+            tokens = response.json()["tokens"]
+            return tokens
+        else:
+            raise Exception(
+                f"Tokenization request failed. Status code: {response.status_code}\nResponse: {response.text}"
+            )
+
+    def get_response_stream(self, headers, data, endpoint_address):
+        response = requests.post(
+            endpoint_address,
+            headers=headers,
+            json=data,
+            stream=True,
+        )
+
+        # Check if the request was successful
+        response.raise_for_status()
+
+        # Define a generator function to yield text chunks
+        def generate_text_chunks():
+            try:
+                decoded_chunk = ""
+                for chunk in response.iter_lines():
+                    if chunk:
+                        decoded_chunk += chunk.decode("utf-8")
+                        if decoded_chunk.strip().startswith("error:"):
+                            raise RuntimeError(decoded_chunk)
+                        new_data = json.loads(decoded_chunk.replace("data:", ""))
+                        if self.llama_cpp_python_server:
+                            returned_data = new_data
+                        else:
+                            if "choices" not in new_data:
+                                returned_data = {
+                                    "choices": [{"text": new_data["content"]}]
+                                }
+                            else:
+                                returned_data = new_data
+                        yield returned_data
+                        decoded_chunk = ""
+
+            except requests.exceptions.RequestException as e:
+                print(f"Request failed: {e}")
+
+        return generate_text_chunks()
+
+    def prepare_generation_settings(
+        self,
+        settings_dictionary: dict,
+        structured_output_settings: LlmStructuredOutputSettings,
+    ) -> dict:
+        if (
+            structured_output_settings.output_type
+            != LlmStructuredOutputType.no_structured_output
+        ):
+            settings_dictionary[
+                "grammar"
+            ] = structured_output_settings.get_gbnf_grammar()
+        if not self.llama_cpp_python_server:
+            settings_dictionary["mirostat"] = settings_dictionary.pop("mirostat_mode")
+        if self.llama_cpp_python_server:
+            settings_dictionary["max_tokens"] = settings_dictionary.pop("n_predict")
+
+        settings_dictionary["stop"] = settings_dictionary.pop(
+            "additional_stop_sequences"
+        )
+        if not self.llama_cpp_python_server:
+            if (
+                "samplers" not in settings_dictionary
+                or settings_dictionary["samplers"] is None
+            ):
+                settings_dictionary["samplers"] = [
+                    "top_k",
+                    "tfs_z",
+                    "typical_p",
+                    "top_p",
+                    "min_p",
+                    "temperature",
+                ]
+        else:
+            if "samplers" in settings_dictionary:
+                del settings_dictionary["samplers"]
+
+        return settings_dictionary
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/tgi_server.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/providers/tgi_server.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-import json
-from copy import deepcopy
-from dataclasses import dataclass, field
-from typing import List, Optional, Dict, Union
-
-import requests
-
-from llama_cpp_agent.llm_output_settings import (
-    LlmStructuredOutputType,
-    LlmStructuredOutputSettings,
-)
-from llama_cpp_agent.providers.provider_base import (
-    LlmProviderId,
-    LlmProvider,
-    LlmSamplingSettings,
-)
-
-
-@dataclass
-class TGIServerSamplingSettings(LlmSamplingSettings):
-    """
-    TGIServerSamplingSettings dataclass
-    """
-
-    best_of: Optional[int] = field(default=None, metadata={"minimum": 0})
-    decoder_input_details: bool = False
-    details: bool = True
-    do_sample: bool = False
-    frequency_penalty: Optional[float] = field(
-        default=None, metadata={"exclusiveMinimum": -2}
-    )
-    grammar: Optional[dict] = None
-    max_new_tokens: Optional[int] = field(default=None, metadata={"minimum": 0})
-    repetition_penalty: Optional[float] = field(
-        default=None, metadata={"exclusiveMinimum": 0}
-    )
-    return_full_text: Optional[bool] = field(default=None)
-    seed: Optional[int] = field(default=None, metadata={"minimum": 0})
-    stop: Optional[List[str]] = field(default_factory=list)
-    temperature: Optional[float] = field(default=None, metadata={"exclusiveMinimum": 0})
-    top_k: Optional[int] = field(default=None, metadata={"exclusiveMinimum": 0})
-    top_n_tokens: Optional[int] = field(
-        default=None, metadata={"minimum": 0, "exclusiveMinimum": 0}
-    )
-    top_p: Optional[float] = field(
-        default=None, metadata={"maximum": 1, "exclusiveMinimum": 0}
-    )
-    truncate: Optional[int] = field(default=None, metadata={"minimum": 0})
-    typical_p: Optional[float] = field(
-        default=None, metadata={"maximum": 1, "exclusiveMinimum": 0}
-    )
-    watermark: bool = False
-    stream: bool = False
-
-    def get_provider_identifier(self) -> LlmProviderId:
-        return LlmProviderId.tgi_server
-
-    def get_additional_stop_sequences(self) -> Union[List[str], None]:
-        return self.stop
-
-    def add_additional_stop_sequences(self, sequences: List[str]):
-        self.stop.extend(sequences)
-
-    def is_streaming(self):
-        return self.stream
-
-    @staticmethod
-    def load_from_dict(settings: dict) -> "TGIServerSamplingSettings":
-        """
-        Load the settings from a dictionary.
-
-        Args:
-            settings (dict): The dictionary containing the settings.
-
-        Returns:
-            LlamaCppSamplingSettings: The loaded settings.
-        """
-        return TGIServerSamplingSettings(**settings)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the settings to a dictionary.
-
-        Returns:
-            dict: The dictionary representation of the settings.
-        """
-        return self.__dict__
-
-
-class TGIServerProvider(LlmProvider):
-
-    def __init__(self, server_address: str, api_key: str = None):
-        self.server_address = server_address
-        self.server_completion_endpoint = self.server_address + "/generate"
-        self.server_streaming_completion_endpoint = (
-                self.server_address + "/generate_stream"
-        )
-        self.server_chat_completion_endpoint = (
-                self.server_address + "/v1/chat/completions"
-        )
-        self.server_tokenize_endpoint = self.server_address + "/tokenize"
-        self.api_key = api_key
-
-    def is_using_json_schema_constraints(self):
-        return True
-
-    def get_provider_identifier(self) -> LlmProviderId:
-        return LlmProviderId.tgi_server
-
-    def get_provider_default_settings(self) -> TGIServerSamplingSettings:
-        return TGIServerSamplingSettings()
-
-    def create_completion(
-            self,
-            prompt: str,
-            structured_output_settings: LlmStructuredOutputSettings,
-            settings: TGIServerSamplingSettings,
-            bos_token: str,
-    ):
-        if self.api_key is not None:
-            headers = {
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
-            }
-        else:
-            headers = {"Content-Type": "application/json"}
-
-        settings_dict = deepcopy(settings.as_dict())
-
-        data = {"parameters": settings_dict, "inputs": prompt}
-        grammar = None
-        if (
-                structured_output_settings.output_type
-                != LlmStructuredOutputType.no_structured_output
-        ):
-            grammar = structured_output_settings.get_json_schema()
-
-        if grammar is not None:
-            data["parameters"]["grammar"] = {"type": "json", "value": grammar}
-        if settings.stream:
-            return self.get_response_stream(
-                headers, data, self.server_streaming_completion_endpoint
-            )
-
-        response = requests.post(
-            self.server_completion_endpoint, headers=headers, json=data
-        )
-        data = response.json()
-
-        returned_data = {"choices": [{"text": data["generated_text"]}]}
-        return returned_data
-
-    def create_chat_completion(
-            self,
-            messages: List[Dict[str, str]],
-            structured_output_settings: LlmStructuredOutputSettings,
-            settings: TGIServerSamplingSettings
-    ):
-        if self.api_key is not None:
-            headers = {
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
-            }
-        else:
-            headers = {"Content-Type": "application/json"}
-        data = deepcopy(settings.as_dict())
-        data["messages"] = messages
-        data["model"] = "tgi"
-        grammar = None
-        if (
-                structured_output_settings.output_type
-                != LlmStructuredOutputType.no_structured_output
-        ):
-            grammar = structured_output_settings.get_json_schema()
-
-        if grammar is not None:
-            data["parameters"]["grammar"] = {"type": "json", "value": grammar}
-        if settings.stream:
-            return self.get_response_stream(
-                headers, data, self.server_chat_completion_endpoint
-            )
-        response = requests.post(
-            self.server_chat_completion_endpoint, headers=headers, json=data
-        )
-        data = response.json()
-
-        returned_data = data
-        return returned_data
-
-    def tokenize(self, prompt: str) -> list[int]:
-        if self.api_key is not None:
-            headers = {
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
-            }
-        else:
-            headers = {"Content-Type": "application/json"}
-        response = requests.post(
-            self.server_tokenize_endpoint, headers=headers, json={"inputs": prompt}
-        )
-        if response.status_code == 200:
-            tokens = response.json()
-            return [tok["id"] for tok in tokens]
-        else:
-            raise Exception(
-                f"Tokenization request failed. Status code: {response.status_code}\nResponse: {response.text}"
-            )
-
-    def get_response_stream(self, headers, data, endpoint_address):
-        response = requests.post(
-            endpoint_address,
-            headers=headers,
-            json=data,
-            stream=True,
-        )
-
-        # Check if the request was successful
-        response.raise_for_status()
-
-        # Define a generator function to yield text chunks
-        def generate_text_chunks():
-            try:
-                decoded_chunk = ""
-                for chunk in response.iter_lines():
-                    if chunk:
-                        decoded_chunk += chunk.decode("utf-8")
-                        new_data = json.loads(decoded_chunk.replace("data:", ""))
-                        if "token" in new_data and (
-                                new_data["token"]["text"] is not None
-                        ):
-                            returned_data = {
-                                "choices": [{"text": new_data["token"]["text"]}]
-                            }
-                            yield returned_data
-                        elif (
-                                "choices" in new_data
-                                and (new_data["choices"][0]["delta"] is not None)
-                                and ("content" in new_data["choices"][0]["delta"])
-                        ):
-                            returned_data = {
-                                "choices": [
-                                    {"text": new_data["choices"][0]["delta"]["content"]}
-                                ]
-                            }
-                            yield returned_data
-                        decoded_chunk = ""
-
-            except requests.exceptions.RequestException as e:
-                print(f"Request failed: {e}")
-
-        return generate_text_chunks()
+import json
+from copy import deepcopy
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Union
+
+import requests
+
+from llama_cpp_agent.llm_output_settings import (
+    LlmStructuredOutputType,
+    LlmStructuredOutputSettings,
+)
+from llama_cpp_agent.providers.provider_base import (
+    LlmProviderId,
+    LlmProvider,
+    LlmSamplingSettings,
+)
+
+
+@dataclass
+class TGIServerSamplingSettings(LlmSamplingSettings):
+    """
+    TGIServerSamplingSettings dataclass
+    """
+
+    best_of: Optional[int] = field(default=None, metadata={"minimum": 0})
+    decoder_input_details: bool = False
+    details: bool = True
+    do_sample: bool = False
+    frequency_penalty: Optional[float] = field(
+        default=None, metadata={"exclusiveMinimum": -2}
+    )
+    grammar: Optional[dict] = None
+    max_new_tokens: Optional[int] = field(default=None, metadata={"minimum": 0})
+    repetition_penalty: Optional[float] = field(
+        default=None, metadata={"exclusiveMinimum": 0}
+    )
+    return_full_text: Optional[bool] = field(default=None)
+    seed: Optional[int] = field(default=None, metadata={"minimum": 0})
+    stop: Optional[List[str]] = field(default_factory=list)
+    temperature: Optional[float] = field(default=None, metadata={"exclusiveMinimum": 0})
+    top_k: Optional[int] = field(default=None, metadata={"exclusiveMinimum": 0})
+    top_n_tokens: Optional[int] = field(
+        default=None, metadata={"minimum": 0, "exclusiveMinimum": 0}
+    )
+    top_p: Optional[float] = field(
+        default=None, metadata={"maximum": 1, "exclusiveMinimum": 0}
+    )
+    truncate: Optional[int] = field(default=None, metadata={"minimum": 0})
+    typical_p: Optional[float] = field(
+        default=None, metadata={"maximum": 1, "exclusiveMinimum": 0}
+    )
+    watermark: bool = False
+    stream: bool = False
+
+    def get_provider_identifier(self) -> LlmProviderId:
+        return LlmProviderId.tgi_server
+
+    def get_additional_stop_sequences(self) -> Union[List[str], None]:
+        return self.stop
+
+    def add_additional_stop_sequences(self, sequences: List[str]):
+        self.stop.extend(sequences)
+
+    def is_streaming(self):
+        return self.stream
+
+    @staticmethod
+    def load_from_dict(settings: dict) -> "TGIServerSamplingSettings":
+        """
+        Load the settings from a dictionary.
+
+        Args:
+            settings (dict): The dictionary containing the settings.
+
+        Returns:
+            LlamaCppSamplingSettings: The loaded settings.
+        """
+        return TGIServerSamplingSettings(**settings)
+
+    def as_dict(self) -> dict:
+        """
+        Convert the settings to a dictionary.
+
+        Returns:
+            dict: The dictionary representation of the settings.
+        """
+        return self.__dict__
+
+
+class TGIServerProvider(LlmProvider):
+
+    def __init__(self, server_address: str, api_key: str = None):
+        self.server_address = server_address
+        self.server_completion_endpoint = self.server_address + "/generate"
+        self.server_streaming_completion_endpoint = (
+                self.server_address + "/generate_stream"
+        )
+        self.server_chat_completion_endpoint = (
+                self.server_address + "/v1/chat/completions"
+        )
+        self.server_tokenize_endpoint = self.server_address + "/tokenize"
+        self.api_key = api_key
+
+    def is_using_json_schema_constraints(self):
+        return True
+
+    def get_provider_identifier(self) -> LlmProviderId:
+        return LlmProviderId.tgi_server
+
+    def get_provider_default_settings(self) -> TGIServerSamplingSettings:
+        return TGIServerSamplingSettings()
+
+    def create_completion(
+            self,
+            prompt: str,
+            structured_output_settings: LlmStructuredOutputSettings,
+            settings: TGIServerSamplingSettings,
+            bos_token: str,
+    ):
+        if self.api_key is not None:
+            headers = {
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
+            }
+        else:
+            headers = {"Content-Type": "application/json"}
+
+        settings_dict = deepcopy(settings.as_dict())
+
+        data = {"parameters": settings_dict, "inputs": prompt}
+        grammar = None
+        if (
+                structured_output_settings.output_type
+                != LlmStructuredOutputType.no_structured_output
+        ):
+            grammar = structured_output_settings.get_json_schema()
+
+        if grammar is not None:
+            data["parameters"]["grammar"] = {"type": "json", "value": grammar}
+        if settings.stream:
+            return self.get_response_stream(
+                headers, data, self.server_streaming_completion_endpoint
+            )
+
+        response = requests.post(
+            self.server_completion_endpoint, headers=headers, json=data
+        )
+        data = response.json()
+
+        returned_data = {"choices": [{"text": data["generated_text"]}]}
+        return returned_data
+
+    def create_chat_completion(
+            self,
+            messages: List[Dict[str, str]],
+            structured_output_settings: LlmStructuredOutputSettings,
+            settings: TGIServerSamplingSettings
+    ):
+        if self.api_key is not None:
+            headers = {
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
+            }
+        else:
+            headers = {"Content-Type": "application/json"}
+        data = deepcopy(settings.as_dict())
+        data["messages"] = messages
+        data["model"] = "tgi"
+        grammar = None
+        if (
+                structured_output_settings.output_type
+                != LlmStructuredOutputType.no_structured_output
+        ):
+            grammar = structured_output_settings.get_json_schema()
+
+        if grammar is not None:
+            data["parameters"]["grammar"] = {"type": "json", "value": grammar}
+        if settings.stream:
+            return self.get_response_stream(
+                headers, data, self.server_chat_completion_endpoint
+            )
+        response = requests.post(
+            self.server_chat_completion_endpoint, headers=headers, json=data
+        )
+        data = response.json()
+
+        returned_data = data
+        return returned_data
+
+    def tokenize(self, prompt: str) -> list[int]:
+        if self.api_key is not None:
+            headers = {
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
+            }
+        else:
+            headers = {"Content-Type": "application/json"}
+        response = requests.post(
+            self.server_tokenize_endpoint, headers=headers, json={"inputs": prompt}
+        )
+        if response.status_code == 200:
+            tokens = response.json()
+            return [tok["id"] for tok in tokens]
+        else:
+            raise Exception(
+                f"Tokenization request failed. Status code: {response.status_code}\nResponse: {response.text}"
+            )
+
+    def get_response_stream(self, headers, data, endpoint_address):
+        response = requests.post(
+            endpoint_address,
+            headers=headers,
+            json=data,
+            stream=True,
+        )
+
+        # Check if the request was successful
+        response.raise_for_status()
+
+        # Define a generator function to yield text chunks
+        def generate_text_chunks():
+            try:
+                decoded_chunk = ""
+                for chunk in response.iter_lines():
+                    if chunk:
+                        decoded_chunk += chunk.decode("utf-8")
+                        new_data = json.loads(decoded_chunk.replace("data:", ""))
+                        if "token" in new_data and (
+                                new_data["token"]["text"] is not None
+                        ):
+                            returned_data = {
+                                "choices": [{"text": new_data["token"]["text"]}]
+                            }
+                            yield returned_data
+                        elif (
+                                "choices" in new_data
+                                and (new_data["choices"][0]["delta"] is not None)
+                                and ("content" in new_data["choices"][0]["delta"])
+                        ):
+                            returned_data = {
+                                "choices": [
+                                    {"text": new_data["choices"][0]["delta"]["content"]}
+                                ]
+                            }
+                            yield returned_data
+                        decoded_chunk = ""
+
+            except requests.exceptions.RequestException as e:
+                print(f"Request failed: {e}")
+
+        return generate_text_chunks()
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/vllm_server.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/providers/vllm_server.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-import json
-from copy import copy, deepcopy
-from dataclasses import dataclass, field
-from typing import List, Dict, Optional, Union
-
-from llama_cpp_agent.llm_output_settings import (
-    LlmStructuredOutputSettings,
-    LlmStructuredOutputType,
-)
-from llama_cpp_agent.providers.provider_base import (
-    LlmProvider,
-    LlmProviderId,
-    LlmSamplingSettings,
-)
-
-
-@dataclass
-class VLLMServerSamplingSettings(LlmSamplingSettings):
-    """
-    VLLMServerSamplingSettings dataclass
-    """
-
-    best_of: Optional[int] = None
-    use_beam_search = False
-    top_k: float = -1
-    top_p: float = 1
-    min_p: float = 0.0
-    temperature: float = 0.7
-    max_tokens: int = 16
-    repetition_penalty: Optional[float] = 1.0
-    length_penalty: Optional[float] = 1.0
-    early_stopping: Optional[bool] = False
-    ignore_eos: Optional[bool] = False
-    min_tokens: Optional[int] = 0
-    stop_token_ids: Optional[List[int]] = field(default_factory=list)
-    skip_special_tokens: Optional[bool] = True
-    spaces_between_special_tokens: Optional[bool] = True
-    stream: bool = False
-
-    def get_provider_identifier(self) -> LlmProviderId:
-        return LlmProviderId.tgi_server
-
-    def get_additional_stop_sequences(self) -> Union[List[str], None]:
-        return None
-
-    def add_additional_stop_sequences(self, sequences: List[str]):
-        pass
-
-    def is_streaming(self):
-        return self.stream
-
-    @staticmethod
-    def load_from_dict(settings: dict) -> "VLLMServerSamplingSettings":
-        """
-        Load the settings from a dictionary.
-
-        Args:
-            settings (dict): The dictionary containing the settings.
-
-        Returns:
-            LlamaCppSamplingSettings: The loaded settings.
-        """
-        return VLLMServerSamplingSettings(**settings)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the settings to a dictionary.
-
-        Returns:
-            dict: The dictionary representation of the settings.
-        """
-        return self.__dict__
-
-
-class VLLMServerProvider(LlmProvider):
-    def __init__(self, base_url: str, model: str, api_key: str = None):
-        from openai import OpenAI
-
-        self.client = OpenAI(
-            base_url=base_url,
-            api_key=api_key,
-        )
-        self.model = model
-
-    def is_using_json_schema_constraints(self):
-        return True
-
-    def get_provider_identifier(self) -> LlmProviderId:
-        return LlmProviderId.tgi_server
-
-    def get_provider_default_settings(self) -> VLLMServerSamplingSettings:
-        return VLLMServerSamplingSettings()
-
-    def create_completion(
-        self,
-        prompt: str,
-        structured_output_settings: LlmStructuredOutputSettings,
-        settings: VLLMServerSamplingSettings,
-        bos_token: str,
-    ):
-        grammar = None
-        if (
-            structured_output_settings.output_type
-            != LlmStructuredOutputType.no_structured_output
-        ):
-            grammar = structured_output_settings.get_json_schema()
-        top_p = settings.top_p
-        stream = settings.stream
-        temperature = settings.temperature
-        max_tokens = settings.max_tokens
-
-        settings_dict = deepcopy(settings.as_dict())
-        settings_dict.pop("top_p")
-        settings_dict.pop("stream")
-        settings_dict.pop("temperature")
-        settings_dict.pop("max_tokens")
-        if grammar is not None:
-            settings_dict["guided_json"] = grammar
-
-        if settings.stream:
-            result = self.client.completions.create(
-                prompt=prompt,
-                model=self.model,
-                extra_body=settings_dict,
-                top_p=top_p,
-                stream=stream,
-                temperature=temperature,
-                max_tokens=max_tokens,
-            )
-
-            def generate_chunks():
-                for chunk in result:
-                    if chunk.choices[0].text is not None:
-                        yield {"choices": [{"text": chunk.choices[0].text}]}
-
-            return generate_chunks()
-        else:
-            result = self.client.completions.create(
-                prompt=prompt,
-                model=self.model,
-                extra_body=settings_dict,
-                top_p=top_p,
-                stream=stream,
-                temperature=temperature,
-                max_tokens=max_tokens,
-            )
-            return {"choices": [{"text": result.choices[0].text}]}
-
-    def create_chat_completion(
-        self,
-        messages: List[Dict[str, str]],
-        structured_output_settings: LlmStructuredOutputSettings,
-        settings: VLLMServerSamplingSettings
-    ):
-        grammar = None
-        if (
-            structured_output_settings.output_type
-            != LlmStructuredOutputType.no_structured_output
-        ):
-            grammar = structured_output_settings.get_json_schema()
-
-        top_p = settings.top_p
-        stream = settings.stream
-        temperature = settings.temperature
-        max_tokens = settings.max_tokens
-
-        settings_dict = copy(settings.as_dict())
-        settings_dict.pop("top_p")
-        settings_dict.pop("stream")
-        settings_dict.pop("temperature")
-        settings_dict.pop("max_tokens")
-        if grammar is not None:
-            settings_dict["guided_json"] = grammar
-
-        if settings.stream:
-            result = self.client.chat.completions.create(
-                messages=messages,
-                model=self.model,
-                extra_body=settings_dict,
-                top_p=top_p,
-                stream=stream,
-                temperature=temperature,
-                max_tokens=max_tokens,
-            )
-
-            def generate_chunks():
-                for chunk in result:
-                    if chunk.choices[0].delta.content is not None:
-                        yield {"choices": [{"text": chunk.choices[0].delta.content}]}
-
-            return generate_chunks()
-        else:
-            result = self.client.chat.completions.create(
-                messages=messages,
-                model=self.model,
-                extra_body=settings_dict,
-                top_p=top_p,
-                stream=stream,
-                temperature=temperature,
-                max_tokens=max_tokens,
-            )
-            return {"choices": [{"text": result.choices[0].message.content}]}
-
-    def tokenize(self, prompt: str) -> list[int]:
-        result = self.tokenize(prompt=prompt)
-        return result
+import json
+from copy import copy, deepcopy
+from dataclasses import dataclass, field
+from typing import List, Dict, Optional, Union
+
+from llama_cpp_agent.llm_output_settings import (
+    LlmStructuredOutputSettings,
+    LlmStructuredOutputType,
+)
+from llama_cpp_agent.providers.provider_base import (
+    LlmProvider,
+    LlmProviderId,
+    LlmSamplingSettings,
+)
+
+
+@dataclass
+class VLLMServerSamplingSettings(LlmSamplingSettings):
+    """
+    VLLMServerSamplingSettings dataclass
+    """
+
+    best_of: Optional[int] = None
+    use_beam_search = False
+    top_k: float = -1
+    top_p: float = 1
+    min_p: float = 0.0
+    temperature: float = 0.7
+    max_tokens: int = 16
+    repetition_penalty: Optional[float] = 1.0
+    length_penalty: Optional[float] = 1.0
+    early_stopping: Optional[bool] = False
+    ignore_eos: Optional[bool] = False
+    min_tokens: Optional[int] = 0
+    stop_token_ids: Optional[List[int]] = field(default_factory=list)
+    skip_special_tokens: Optional[bool] = True
+    spaces_between_special_tokens: Optional[bool] = True
+    stream: bool = False
+
+    def get_provider_identifier(self) -> LlmProviderId:
+        return LlmProviderId.tgi_server
+
+    def get_additional_stop_sequences(self) -> Union[List[str], None]:
+        return None
+
+    def add_additional_stop_sequences(self, sequences: List[str]):
+        pass
+
+    def is_streaming(self):
+        return self.stream
+
+    @staticmethod
+    def load_from_dict(settings: dict) -> "VLLMServerSamplingSettings":
+        """
+        Load the settings from a dictionary.
+
+        Args:
+            settings (dict): The dictionary containing the settings.
+
+        Returns:
+            LlamaCppSamplingSettings: The loaded settings.
+        """
+        return VLLMServerSamplingSettings(**settings)
+
+    def as_dict(self) -> dict:
+        """
+        Convert the settings to a dictionary.
+
+        Returns:
+            dict: The dictionary representation of the settings.
+        """
+        return self.__dict__
+
+
+class VLLMServerProvider(LlmProvider):
+    def __init__(self, base_url: str, model: str, api_key: str = None):
+        from openai import OpenAI
+
+        self.client = OpenAI(
+            base_url=base_url,
+            api_key=api_key,
+        )
+        self.model = model
+
+    def is_using_json_schema_constraints(self):
+        return True
+
+    def get_provider_identifier(self) -> LlmProviderId:
+        return LlmProviderId.tgi_server
+
+    def get_provider_default_settings(self) -> VLLMServerSamplingSettings:
+        return VLLMServerSamplingSettings()
+
+    def create_completion(
+        self,
+        prompt: str,
+        structured_output_settings: LlmStructuredOutputSettings,
+        settings: VLLMServerSamplingSettings,
+        bos_token: str,
+    ):
+        grammar = None
+        if (
+            structured_output_settings.output_type
+            != LlmStructuredOutputType.no_structured_output
+        ):
+            grammar = structured_output_settings.get_json_schema()
+        top_p = settings.top_p
+        stream = settings.stream
+        temperature = settings.temperature
+        max_tokens = settings.max_tokens
+
+        settings_dict = deepcopy(settings.as_dict())
+        settings_dict.pop("top_p")
+        settings_dict.pop("stream")
+        settings_dict.pop("temperature")
+        settings_dict.pop("max_tokens")
+        if grammar is not None:
+            settings_dict["guided_json"] = grammar
+
+        if settings.stream:
+            result = self.client.completions.create(
+                prompt=prompt,
+                model=self.model,
+                extra_body=settings_dict,
+                top_p=top_p,
+                stream=stream,
+                temperature=temperature,
+                max_tokens=max_tokens,
+            )
+
+            def generate_chunks():
+                for chunk in result:
+                    if chunk.choices[0].text is not None:
+                        yield {"choices": [{"text": chunk.choices[0].text}]}
+
+            return generate_chunks()
+        else:
+            result = self.client.completions.create(
+                prompt=prompt,
+                model=self.model,
+                extra_body=settings_dict,
+                top_p=top_p,
+                stream=stream,
+                temperature=temperature,
+                max_tokens=max_tokens,
+            )
+            return {"choices": [{"text": result.choices[0].text}]}
+
+    def create_chat_completion(
+        self,
+        messages: List[Dict[str, str]],
+        structured_output_settings: LlmStructuredOutputSettings,
+        settings: VLLMServerSamplingSettings
+    ):
+        grammar = None
+        if (
+            structured_output_settings.output_type
+            != LlmStructuredOutputType.no_structured_output
+        ):
+            grammar = structured_output_settings.get_json_schema()
+
+        top_p = settings.top_p
+        stream = settings.stream
+        temperature = settings.temperature
+        max_tokens = settings.max_tokens
+
+        settings_dict = copy(settings.as_dict())
+        settings_dict.pop("top_p")
+        settings_dict.pop("stream")
+        settings_dict.pop("temperature")
+        settings_dict.pop("max_tokens")
+        if grammar is not None:
+            settings_dict["guided_json"] = grammar
+
+        if settings.stream:
+            result = self.client.chat.completions.create(
+                messages=messages,
+                model=self.model,
+                extra_body=settings_dict,
+                top_p=top_p,
+                stream=stream,
+                temperature=temperature,
+                max_tokens=max_tokens,
+            )
+
+            def generate_chunks():
+                for chunk in result:
+                    if chunk.choices[0].delta.content is not None:
+                        yield {"choices": [{"text": chunk.choices[0].delta.content}]}
+
+            return generate_chunks()
+        else:
+            result = self.client.chat.completions.create(
+                messages=messages,
+                model=self.model,
+                extra_body=settings_dict,
+                top_p=top_p,
+                stream=stream,
+                temperature=temperature,
+                max_tokens=max_tokens,
+            )
+            return {"choices": [{"text": result.choices[0].message.content}]}
+
+    def tokenize(self, prompt: str) -> list[int]:
+        result = self.tokenize(prompt=prompt)
+        return result
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/structured_output_agent.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/structured_output_agent.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-import json
-from copy import copy
-from typing import Type, Callable, Union
-
-from llama_cpp import Llama
-from pydantic import BaseModel
-
-from .llm_agent import LlamaCppAgent, StreamingResponse
-from .llm_output_settings import LlmStructuredOutputSettings, LlmStructuredOutputType
-from .llm_prompt_template import PromptTemplate
-from .output_parser import extract_object_from_response
-from .messages_formatter import MessagesFormatterType, MessagesFormatter
-
-
-from .providers.provider_base import LlmProvider, LlmSamplingSettings
-
-
-class StructuredOutputAgent:
-    """
-    An agent that creates structured output based on pydantic models from unstructured text.
-
-    Args:
-        llama_llm (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings]): An instance of Llama, LlamaLLMSettings, LlamaCppServerLLMSettings, OpenAIEndpointSettings as LLM.
-        llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppGenerationSettings, OpenAIGenerationSettings]): Generation settings for Llama or LlamaCppServer.
-        messages_formatter_type (MessagesFormatterType): Type of messages formatter.
-        custom_messages_formatter (MessagesFormatter): Custom messages formatter.
-        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-        debug_output (bool): Enable debug output.
-
-    Attributes:
-        llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppServerGenerationSettings]): Generation settings for Llama or LlamaCppServer.
-        grammar_cache (dict): Cache for generated grammars.
-        system_prompt_template (PromptTemplate): Template for the system prompt.
-        creation_prompt_template (PromptTemplate): Template for the creation prompt.
-        llama_cpp_agent (LlamaCppAgent): LlamaCppAgent instance for interaction.
-        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-
-    Methods:
-        save(file_path: str): Save the agent's state to a file.
-        load_from_file(file_path: str, llama_llm, streaming_callback) -> StructuredOutputAgent: Load the agent's state from a file.
-        load_from_dict(agent_dict: dict) -> StructuredOutputAgent: Load the agent's state from a dictionary.
-        as_dict() -> dict: Convert the agent's state to a dictionary.
-        create_object(model: Type[BaseModel], data: str = "") -> object: Create an object of the given model from the given data.
-
-    """
-
-    def __init__(
-        self,
-        llama_llm: LlmProvider,
-        messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
-        custom_messages_formatter: MessagesFormatter = None,
-        streaming_callback: Callable[[StreamingResponse], None] = None,
-        debug_output: bool = False,
-    ):
-        """
-        Initialize the StructuredOutputAgent.
-
-        Args:
-            llama_llm (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings]): An instance of Llama, LlamaLLMSettings, or LlamaCppServerLLMSettings as LLM.
-            llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppGenerationSettings, OpenAIGenerationSettings]): Generation settings for Llama or LlamaCppServer or OpenAIEndpoint.
-            messages_formatter_type (MessagesFormatterType): Type of messages formatter.
-            custom_messages_formatter (MessagesFormatter): Custom messages formatter.
-            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
-            debug_output (bool): Enable debug output.
-        """
-        self.grammar_cache = {}
-        self.system_prompt_template = PromptTemplate.from_string(
-            "You are an advanced AI agent. You are tasked to assist the user by creating structured output in JSON format.\n\n{documentation}"
-        )
-        self.creation_prompt_template = PromptTemplate.from_string(
-            "Create an JSON response based on the following input.\n\nInput:\n\n{user_input}"
-        )
-
-        self.llama_cpp_agent = LlamaCppAgent(
-            llama_llm,
-            debug_output=debug_output,
-            system_prompt="",
-            predefined_messages_formatter_type=messages_formatter_type,
-            custom_messages_formatter=custom_messages_formatter,
-        )
-        self.streaming_callback = streaming_callback
-
-    def save(self, file_path: str):
-        """
-        Save the agent's state to a file.
-
-        Args:
-            file_path (str): The path to the file.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            dic = copy(self.as_dict())
-            del dic["llama_cpp_agent"]
-            del dic["grammar_cache"]
-            del dic["system_prompt_template"]
-            del dic["creation_prompt_template"]
-            del dic["streaming_callback"]
-            dic["debug_output"] = self.llama_cpp_agent.debug_output
-            dic["llama_generation_settings"] = self.llama_generation_settings.as_dict()
-            dic[
-                "custom_messages_formatter"
-            ] = self.llama_cpp_agent.messages_formatter.as_dict()
-            json.dump(dic, file, indent=4)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the agent's state to a dictionary.
-
-        Returns:
-            dict: The dictionary representation of the agent's state.
-        """
-        return self.__dict__
-
-    def create_object(
-        self,
-        model: Type[BaseModel],
-        data: str = "",
-        llm_sampling_settings: LlmSamplingSettings = None,
-    ) -> object:
-        """
-        Creates an object of the given model from the given data.
-
-        Args:
-            model (Type[BaseModel]): The model to create the object from.
-            data (str): The data to create the object from.
-
-        Returns:
-            object: The created object.
-        """
-        output_settings = LlmStructuredOutputSettings.from_pydantic_models(
-            [model], output_type=LlmStructuredOutputType.object_instance
-        )
-
-        system_prompt = self.system_prompt_template.generate_prompt(
-            {
-                "documentation": output_settings.get_llm_documentation(
-                    self.llama_cpp_agent.provider
-                ).strip()
-            }
-        )
-        if data == "":
-            prompt = "Create a random JSON response based on the response model."
-        else:
-            prompt = self.creation_prompt_template.generate_prompt({"user_input": data})
-        response = self.llama_cpp_agent.get_chat_response(
-            prompt,
-            system_prompt=system_prompt,
-            add_response_to_chat_history=False,
-            add_message_to_chat_history=False,
-            streaming_callback=self.streaming_callback,
-            structured_output_settings=output_settings,
-            llm_sampling_settings=llm_sampling_settings,
-        )
-        return response
+import json
+from copy import copy
+from typing import Type, Callable, Union
+
+from llama_cpp import Llama
+from pydantic import BaseModel
+
+from .llm_agent import LlamaCppAgent, StreamingResponse
+from .llm_output_settings import LlmStructuredOutputSettings, LlmStructuredOutputType
+from .llm_prompt_template import PromptTemplate
+from .output_parser import extract_object_from_response
+from .messages_formatter import MessagesFormatterType, MessagesFormatter
+
+
+from .providers.provider_base import LlmProvider, LlmSamplingSettings
+
+
+class StructuredOutputAgent:
+    """
+    An agent that creates structured output based on pydantic models from unstructured text.
+
+    Args:
+        llama_llm (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings]): An instance of Llama, LlamaLLMSettings, LlamaCppServerLLMSettings, OpenAIEndpointSettings as LLM.
+        llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppGenerationSettings, OpenAIGenerationSettings]): Generation settings for Llama or LlamaCppServer.
+        messages_formatter_type (MessagesFormatterType): Type of messages formatter.
+        custom_messages_formatter (MessagesFormatter): Custom messages formatter.
+        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+        debug_output (bool): Enable debug output.
+
+    Attributes:
+        llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppServerGenerationSettings]): Generation settings for Llama or LlamaCppServer.
+        grammar_cache (dict): Cache for generated grammars.
+        system_prompt_template (PromptTemplate): Template for the system prompt.
+        creation_prompt_template (PromptTemplate): Template for the creation prompt.
+        llama_cpp_agent (LlamaCppAgent): LlamaCppAgent instance for interaction.
+        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+
+    Methods:
+        save(file_path: str): Save the agent's state to a file.
+        load_from_file(file_path: str, llama_llm, streaming_callback) -> StructuredOutputAgent: Load the agent's state from a file.
+        load_from_dict(agent_dict: dict) -> StructuredOutputAgent: Load the agent's state from a dictionary.
+        as_dict() -> dict: Convert the agent's state to a dictionary.
+        create_object(model: Type[BaseModel], data: str = "") -> object: Create an object of the given model from the given data.
+
+    """
+
+    def __init__(
+        self,
+        llama_llm: LlmProvider,
+        messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
+        custom_messages_formatter: MessagesFormatter = None,
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+        debug_output: bool = False,
+    ):
+        """
+        Initialize the StructuredOutputAgent.
+
+        Args:
+            llama_llm (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings]): An instance of Llama, LlamaLLMSettings, or LlamaCppServerLLMSettings as LLM.
+            llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppGenerationSettings, OpenAIGenerationSettings]): Generation settings for Llama or LlamaCppServer or OpenAIEndpoint.
+            messages_formatter_type (MessagesFormatterType): Type of messages formatter.
+            custom_messages_formatter (MessagesFormatter): Custom messages formatter.
+            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+            debug_output (bool): Enable debug output.
+        """
+        self.grammar_cache = {}
+        self.system_prompt_template = PromptTemplate.from_string(
+            "You are an advanced AI agent. You are tasked to assist the user by creating structured output in JSON format.\n\n{documentation}"
+        )
+        self.creation_prompt_template = PromptTemplate.from_string(
+            "Create an JSON response based on the following input.\n\nInput:\n\n{user_input}"
+        )
+
+        self.llama_cpp_agent = LlamaCppAgent(
+            llama_llm,
+            debug_output=debug_output,
+            system_prompt="",
+            predefined_messages_formatter_type=messages_formatter_type,
+            custom_messages_formatter=custom_messages_formatter,
+        )
+        self.streaming_callback = streaming_callback
+
+    def save(self, file_path: str):
+        """
+        Save the agent's state to a file.
+
+        Args:
+            file_path (str): The path to the file.
+        """
+        with open(file_path, "w", encoding="utf-8") as file:
+            dic = copy(self.as_dict())
+            del dic["llama_cpp_agent"]
+            del dic["grammar_cache"]
+            del dic["system_prompt_template"]
+            del dic["creation_prompt_template"]
+            del dic["streaming_callback"]
+            dic["debug_output"] = self.llama_cpp_agent.debug_output
+            dic["llama_generation_settings"] = self.llama_generation_settings.as_dict()
+            dic[
+                "custom_messages_formatter"
+            ] = self.llama_cpp_agent.messages_formatter.as_dict()
+            json.dump(dic, file, indent=4)
+
+    def as_dict(self) -> dict:
+        """
+        Convert the agent's state to a dictionary.
+
+        Returns:
+            dict: The dictionary representation of the agent's state.
+        """
+        return self.__dict__
+
+    def create_object(
+        self,
+        model: Type[BaseModel],
+        data: str = "",
+        llm_sampling_settings: LlmSamplingSettings = None,
+    ) -> object:
+        """
+        Creates an object of the given model from the given data.
+
+        Args:
+            model (Type[BaseModel]): The model to create the object from.
+            data (str): The data to create the object from.
+
+        Returns:
+            object: The created object.
+        """
+        output_settings = LlmStructuredOutputSettings.from_pydantic_models(
+            [model], output_type=LlmStructuredOutputType.object_instance
+        )
+
+        system_prompt = self.system_prompt_template.generate_prompt(
+            {
+                "documentation": output_settings.get_llm_documentation(
+                    self.llama_cpp_agent.provider
+                ).strip()
+            }
+        )
+        if data == "":
+            prompt = "Create a random JSON response based on the response model."
+        else:
+            prompt = self.creation_prompt_template.generate_prompt({"user_input": data})
+        response = self.llama_cpp_agent.get_chat_response(
+            prompt,
+            system_prompt=system_prompt,
+            add_response_to_chat_history=False,
+            add_message_to_chat_history=False,
+            streaming_callback=self.streaming_callback,
+            structured_output_settings=output_settings,
+            llm_sampling_settings=llm_sampling_settings,
+        )
+        return response
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent/text_utils.py` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent/text_utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-import re
-
-
-class TextChunker:
-    def __init__(self, text, chunk_size, overlap=0):
-        """
-        Initializes the TextChunker instance.
-
-        Parameters:
-            text (str): The text to be chunked.
-            chunk_size (int): The length of each text chunk.
-            overlap (int): The number of characters that should overlap between consecutive chunks.
-        """
-        self.text = text
-        self.chunk_size = chunk_size
-        self.overlap = overlap
-
-    def get_chunks(self):
-        """
-        Generates the text chunks based on the specified chunk size and overlap.
-
-        Returns:
-            list[str]: A list of chunked text segments.
-        """
-        chunks = []
-        start = 0
-        while start < len(self.text):
-            # Calculate end index of the chunk
-            end = start + self.chunk_size
-            # Append chunk to the list
-            chunks.append(self.text[start:end])
-            # Update start index for the next chunk
-            start = end - self.overlap if self.overlap < self.chunk_size else start + 1
-            # Prevent infinite loop in case overlap is not less than chunk_size
-            if self.chunk_size <= self.overlap:
-                raise ValueError(
-                    "Overlap must be less than chunk size to prevent infinite loops."
-                )
-        return chunks
-
-
-class RecursiveCharacterTextSplitter:
-    def __init__(
-        self,
-        separators,
-        chunk_size,
-        chunk_overlap,
-        length_function=len,
-        keep_separator=False,
-    ):
-        self.separators = separators
-        self.chunk_size = chunk_size
-        self.chunk_overlap = chunk_overlap
-        self.length_function = length_function
-        self.keep_separator = keep_separator
-
-    def split_text(self, text, depth=0):
-        if depth == len(self.separators):
-            return self._split_into_fixed_size(text)
-
-        current_separator = self.separators[depth]
-        if current_separator == "":
-            return list(text)
-
-        if self.keep_separator:
-            # Use regex to keep separators with the text
-            pieces = re.split(f"({re.escape(current_separator)})", text)
-            # Reattach separators to the chunks
-            pieces = [
-                (
-                    pieces[i] + pieces[i + 1]
-                    if i + 1 < len(pieces) and pieces[i + 1] == current_separator
-                    else pieces[i]
-                )
-                for i in range(0, len(pieces), 2)
-            ]
-        else:
-            pieces = text.split(current_separator)
-
-        refined_pieces = []
-
-        for piece in pieces:
-            if self.length_function(piece) > self.chunk_size:
-                refined_pieces.extend(self.split_text(piece, depth + 1))
-            else:
-                refined_pieces.append(piece)
-
-        return self._merge_pieces(refined_pieces) if depth == 0 else refined_pieces
-
-    def _split_into_fixed_size(self, text):
-        size = self.chunk_size
-        overlap = self.chunk_overlap
-        chunks = [text[i : i + size] for i in range(0, len(text), size - overlap)]
-        if chunks and len(chunks[-1]) < overlap:
-            chunks[-2] += chunks[-1]
-            chunks.pop()
-        return chunks
-
-    def _merge_pieces(self, pieces):
-        merged = []
-        current_chunk = pieces[0]
-
-        for piece in pieces[1:]:
-            if self.length_function(current_chunk + piece) <= self.chunk_size:
-                current_chunk += piece
-            else:
-                merged.append(current_chunk)
-                if len(current_chunk) == self.chunk_size:
-                    current_chunk = current_chunk[-self.chunk_overlap :] + piece
-                else:
-                    current_chunk = piece
-
-        merged.append(current_chunk)
-        return merged
+import re
+
+
+class TextChunker:
+    def __init__(self, text, chunk_size, overlap=0):
+        """
+        Initializes the TextChunker instance.
+
+        Parameters:
+            text (str): The text to be chunked.
+            chunk_size (int): The length of each text chunk.
+            overlap (int): The number of characters that should overlap between consecutive chunks.
+        """
+        self.text = text
+        self.chunk_size = chunk_size
+        self.overlap = overlap
+
+    def get_chunks(self):
+        """
+        Generates the text chunks based on the specified chunk size and overlap.
+
+        Returns:
+            list[str]: A list of chunked text segments.
+        """
+        chunks = []
+        start = 0
+        while start < len(self.text):
+            # Calculate end index of the chunk
+            end = start + self.chunk_size
+            # Append chunk to the list
+            chunks.append(self.text[start:end])
+            # Update start index for the next chunk
+            start = end - self.overlap if self.overlap < self.chunk_size else start + 1
+            # Prevent infinite loop in case overlap is not less than chunk_size
+            if self.chunk_size <= self.overlap:
+                raise ValueError(
+                    "Overlap must be less than chunk size to prevent infinite loops."
+                )
+        return chunks
+
+
+class RecursiveCharacterTextSplitter:
+    def __init__(
+        self,
+        separators,
+        chunk_size,
+        chunk_overlap,
+        length_function=len,
+        keep_separator=False,
+    ):
+        self.separators = separators
+        self.chunk_size = chunk_size
+        self.chunk_overlap = chunk_overlap
+        self.length_function = length_function
+        self.keep_separator = keep_separator
+
+    def split_text(self, text, depth=0):
+        if depth == len(self.separators):
+            return self._split_into_fixed_size(text)
+
+        current_separator = self.separators[depth]
+        if current_separator == "":
+            return list(text)
+
+        if self.keep_separator:
+            # Use regex to keep separators with the text
+            pieces = re.split(f"({re.escape(current_separator)})", text)
+            # Reattach separators to the chunks
+            pieces = [
+                (
+                    pieces[i] + pieces[i + 1]
+                    if i + 1 < len(pieces) and pieces[i + 1] == current_separator
+                    else pieces[i]
+                )
+                for i in range(0, len(pieces), 2)
+            ]
+        else:
+            pieces = text.split(current_separator)
+
+        refined_pieces = []
+
+        for piece in pieces:
+            if self.length_function(piece) > self.chunk_size:
+                refined_pieces.extend(self.split_text(piece, depth + 1))
+            else:
+                refined_pieces.append(piece)
+
+        return self._merge_pieces(refined_pieces) if depth == 0 else refined_pieces
+
+    def _split_into_fixed_size(self, text):
+        size = self.chunk_size
+        overlap = self.chunk_overlap
+        chunks = [text[i : i + size] for i in range(0, len(text), size - overlap)]
+        if chunks and len(chunks[-1]) < overlap:
+            chunks[-2] += chunks[-1]
+            chunks.pop()
+        return chunks
+
+    def _merge_pieces(self, pieces):
+        merged = []
+        current_chunk = pieces[0]
+
+        for piece in pieces[1:]:
+            if self.length_function(current_chunk + piece) <= self.chunk_size:
+                current_chunk += piece
+            else:
+                merged.append(current_chunk)
+                if len(current_chunk) == self.chunk_size:
+                    current_chunk = current_chunk[-self.chunk_overlap :] + piece
+                else:
+                    current_chunk = piece
+
+        merged.append(current_chunk)
+        return merged
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/PKG-INFO` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-Metadata-Version: 2.1
-Name: llama-cpp-agent
-Version: 0.2.3
-Summary: A framework for building LLM based AI agents with llama.cpp.
-Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
-Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
-Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: llama-cpp-python>=0.2.60
-Requires-Dist: pydantic>=2.5.3
-Requires-Dist: requests>=2.31.0
-Requires-Dist: docstring_parser
-Requires-Dist: aiohttp
-Provides-Extra: agent-memory
-Requires-Dist: chromadb; extra == "agent-memory"
-Requires-Dist: SQLAlchemy; extra == "agent-memory"
-Requires-Dist: numpy; extra == "agent-memory"
-Requires-Dist: scipy; extra == "agent-memory"
-Provides-Extra: rag
-Requires-Dist: ragatouille; extra == "rag"
-Provides-Extra: vllm-provider
-Requires-Dist: openai; extra == "vllm-provider"
-Provides-Extra: mixtral-agent
-Requires-Dist: mistral-common; extra == "mixtral-agent"
-
-# llama-cpp-agent
-
-[![PyPI - Version](https://img.shields.io/pypi/v/llama-cpp-agent?logo=pypi&color=%2341bb13)](https://pypi.org/project/llama-cpp-agent/)
-[![Discord](https://img.shields.io/discord/1237393014154985582?logo=Discord&logoColor=%23ffffff&label=Discord&link=https%3A%2F%2Fdiscord.gg%2FsRMvWKrh)](https://discord.gg/sRMvWKrh)
-
-<img src="./logo/logo_orange.png" alt="llama-cpp-agent logo" width="280"/>
-
-## Introduction
-The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
-
-The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
-
-The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
-
-## Key Features
-- **Simple Chat Interface**: Engage in seamless conversations with LLMs.
-- **Structured Output**: Generate structured output (objects) from LLMs.
-- **Single and Parallel Function Calling**: Execute functions using LLMs.
-- **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
-- **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
-- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
-- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
-- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
-- **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
-
-
-## Table of Contents
-- [Introduction](#introduction)
-- [Key Features](#key-features)
-- [Installation](#installation)
-- [Documentation](#documentation)
-- [Getting Started](#getting-started)
-- [Discord Community](#discord-community)
-- [Usage Examples](#usage-examples)
-    - [Simple Chat](#simple-chat-example-using-llamacpp-server-backend)
-    - [Parallel Function Calling](#parallel-function-calling-agent-example)
-    - [Structured Output](#structured-output)
-    - [RAG - Retrieval Augmented Generation](#rag---retrieval-augmented-generation)
-    - [llama-index Tools](#llama-index-tools-example)
-    - [Sequential Chain](#sequential-chain-example)
-    - [Mapping Chain](#mapping-chain-example)
-    - [Knowledge Graph Creation](#knowledge-graph-creation-example)
-- [Additional Information](#additional-information)
-    - [Predefined Messages Formatter](#predefined-messages-formatter)
-    - [Creating Custom Messages Formatter](#creating-custom-messages-formatter)
-- [Contributing](#contributing)
-- [License](#license)
-- [FAQ](#faq)
-
-
-
-## Installation
-Install the llama-cpp-agent framework using pip:
-```shell
-pip install llama-cpp-agent
-```
-## Documentation
-You can find the latest documentation [here!](https://llama-cpp-agent.readthedocs.io/en/latest/)
-
-## Getting Started
-You can find the get started guide [here!](https://llama-cpp-agent.readthedocs.io/en/latest/get-started/)
-
-## Discord Community
-Join the Discord Community [here](https://discord.gg/6tGznupZGX)
-
-## Usage Examples
-The llama-cpp-agent framework provides a wide range of examples demonstrating its capabilities. Here are some key examples:
-
-### Simple Chat Example using llama.cpp server backend
-This example demonstrates how to initiate a chat with an LLM model using the llama.cpp server backend. It supports llama-cpp-python Llama class instances, OpenAI endpoints with GBNF grammar support, and the llama.cpp backend server.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/simple-chat-example/)
-
-### Parallel Function Calling Agent Example
-This example showcases parallel function calling using the FunctionCallingAgent class. It demonstrates how to define and execute multiple functions concurrently.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/parallel_function_calling/)
-
-### Structured Output
-This example illustrates how to generate structured output objects using the StructuredOutputAgent class. It shows how to create a dataset entry of a book from unstructured data.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/structured-output-example/)
-
-### RAG - Retrieval Augmented Generation
-This example demonstrates Retrieval Augmented Generation (RAG) with colbert reranking. It requires installing the optional rag dependencies (ragatouille).
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/rag/)
-
-### llama-index Tools Example
-This example shows how to use llama-index tools and query engines with the FunctionCallingAgent class.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/llama_index_tool_use/)
-
-### Sequential Chain Example
-This example demonstrates how to create a complete product launch campaign using a sequential chain.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/sequential_chain/)
-
-### Mapping Chain Example
-This example illustrates how to create a mapping chain to summarize multiple articles into a single summary.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/map_chain/)
-
-### Knowledge Graph Creation Example
-This example, based on an example from the Instructor library for OpenAI, shows how to create a knowledge graph using the llama-cpp-agent framework.
-
-[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/knowledge-graph-example/)
-
-
-## Additional Information
-
-### Predefined Messages Formatter
-
-The llama-cpp-agent framework provides predefined message formatters to format messages for the LLM model. The `MessagesFormatterType` enum defines the available formatters:
-
-- `MessagesFormatterType.MISTRAL`: Formats messages using the MISTRAL format.
-- `MessagesFormatterType.CHATML`: Formats messages using the CHATML format.
-- `MessagesFormatterType.VICUNA`: Formats messages using the VICUNA format.
-- `MessagesFormatterType.LLAMA_2`: Formats messages using the LLAMA 2 format.
-- `MessagesFormatterType.SYNTHIA`: Formats messages using the SYNTHIA format.
-- `MessagesFormatterType.NEURAL_CHAT`: Formats messages using the NEURAL CHAT format.
-- `MessagesFormatterType.SOLAR`: Formats messages using the SOLAR format.
-- `MessagesFormatterType.OPEN_CHAT`: Formats messages using the OPEN CHAT format.
-- `MessagesFormatterType.ALPACA`: Formats messages using the ALPACA format.
-- `MessagesFormatterType.CODE_DS`: Formats messages using the CODE DS format.
-- `MessagesFormatterType.B22`: Formats messages using the B22 format.
-- `MessagesFormatterType.LLAMA_3`: Formats messages using the LLAMA 3 format.
-- `MessagesFormatterType.PHI_3`: Formats messages using the PHI 3 format.
-
-### Creating Custom Messages Formatter
-
-You can create your own custom messages formatter by instantiating the `MessagesFormatter` class with the desired parameters:
-
-```python
-from llama_cpp_agent.chat_history.messages_formatter import MessagesFormatter, PromptMarkers, Roles
-
-custom_prompt_markers = {
-    Roles.system: PromptMarkers("<|system|>", "<|endsystem|>"),
-    Roles.user: PromptMarkers("<|user|>", "<|enduser|>"),
-    Roles.assistant: PromptMarkers("<|assistant|>", "<|endassistant|>"),
-    Roles.tool: PromptMarkers("<|tool|>", "<|endtool|>"),
-}
-
-custom_formatter = MessagesFormatter(
-    pre_prompt="",
-    prompt_markers=custom_prompt_markers,
-    include_sys_prompt_in_first_user_message=False,
-    default_stop_sequences=["<|endsystem|>", "<|enduser|>", "<|endassistant|>", "<|endtool|>"]
-)
-```
-
-## Contributing
-We welcome contributions to the llama-cpp-agent framework! If you'd like to contribute, please follow these guidelines:
-
-1. Fork the repository and create your branch from `master`.
-2. Ensure your code follows the project's coding style and conventions.
-3. Write clear, concise commit messages and pull request descriptions.
-4. Test your changes thoroughly before submitting a pull request.
-5. Open a pull request to the `master` branch.
-
-If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/Maximilian-Winter/llama-cpp-agent/issues).
-
-## License
-The llama-cpp-agent framework is released under the [MIT License](https://github.com/Maximilian-Winter/llama-cpp-agent/blob/master/LICENSE).
-
-## FAQ
-
-**Q: How do I install the optional dependencies for RAG?**  
-A: To use the RAGColbertReranker class and the RAG example, you need to install the optional rag dependencies (ragatouille). You can do this by running `pip install llama-cpp-agent[rag]`.
-
-**Q: Can I contribute to the llama-cpp-agent project?**  
-A: Absolutely! We welcome contributions from the community. Please refer to the [Contributing](#contributing) section for guidelines on how to contribute.
-
-**Q: Is llama-cpp-agent compatible with the latest version of llama-cpp-python?**  
-A: Yes, llama-cpp-agent is designed to work with the latest version of llama-cpp-python. However, if you encounter any compatibility issues, please open an issue on the GitHub repository.
+Metadata-Version: 2.1
+Name: llama-cpp-agent
+Version: 0.2.4
+Summary: A framework for building LLM based AI agents with llama.cpp.
+Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
+Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
+Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: llama-cpp-python>=0.2.60
+Requires-Dist: pydantic>=2.5.3
+Requires-Dist: requests>=2.31.0
+Requires-Dist: docstring_parser
+Requires-Dist: aiohttp
+Provides-Extra: agent-memory
+Requires-Dist: chromadb; extra == "agent-memory"
+Requires-Dist: SQLAlchemy; extra == "agent-memory"
+Requires-Dist: numpy; extra == "agent-memory"
+Requires-Dist: scipy; extra == "agent-memory"
+Provides-Extra: rag
+Requires-Dist: ragatouille; extra == "rag"
+Provides-Extra: vllm-provider
+Requires-Dist: openai; extra == "vllm-provider"
+Provides-Extra: mixtral-agent
+Requires-Dist: mistral-common; extra == "mixtral-agent"
+
+# llama-cpp-agent
+
+[![PyPI - Version](https://img.shields.io/pypi/v/llama-cpp-agent?logo=pypi&color=%2341bb13)](https://pypi.org/project/llama-cpp-agent/)
+[![Discord](https://img.shields.io/discord/1237393014154985582?logo=Discord&logoColor=%23ffffff&label=Discord&link=https%3A%2F%2Fdiscord.gg%2FsRMvWKrh)](https://discord.gg/sRMvWKrh)
+
+![llama-cpp-agent logo](https://github.com/Maximilian-Winter/llama-cpp-agent/blob/ed6b0973c15cf653d406e53dd6b4efc8d97796cb/logo/logo_orange.png)
+
+## Introduction
+The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
+
+The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
+
+The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
+
+## Key Features
+- **Simple Chat Interface**: Engage in seamless conversations with LLMs.
+- **Structured Output**: Generate structured output (objects) from LLMs.
+- **Single and Parallel Function Calling**: Execute functions using LLMs.
+- **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
+- **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
+- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
+- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
+- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
+- **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
+
+
+## Table of Contents
+- [Introduction](#introduction)
+- [Key Features](#key-features)
+- [Installation](#installation)
+- [Documentation](#documentation)
+- [Getting Started](#getting-started)
+- [Discord Community](#discord-community)
+- [Usage Examples](#usage-examples)
+    - [Simple Chat](#simple-chat-example-using-llamacpp-server-backend)
+    - [Parallel Function Calling](#parallel-function-calling-agent-example)
+    - [Structured Output](#structured-output)
+    - [RAG - Retrieval Augmented Generation](#rag---retrieval-augmented-generation)
+    - [llama-index Tools](#llama-index-tools-example)
+    - [Sequential Chain](#sequential-chain-example)
+    - [Mapping Chain](#mapping-chain-example)
+    - [Knowledge Graph Creation](#knowledge-graph-creation-example)
+- [Additional Information](#additional-information)
+    - [Predefined Messages Formatter](#predefined-messages-formatter)
+    - [Creating Custom Messages Formatter](#creating-custom-messages-formatter)
+- [Contributing](#contributing)
+- [License](#license)
+- [FAQ](#faq)
+
+
+
+## Installation
+Install the llama-cpp-agent framework using pip:
+```shell
+pip install llama-cpp-agent
+```
+## Documentation
+You can find the latest documentation [here!](https://llama-cpp-agent.readthedocs.io/en/latest/)
+
+## Getting Started
+You can find the get started guide [here!](https://llama-cpp-agent.readthedocs.io/en/latest/get-started/)
+
+## Discord Community
+Join the Discord Community [here](https://discord.gg/6tGznupZGX)
+
+## Usage Examples
+The llama-cpp-agent framework provides a wide range of examples demonstrating its capabilities. Here are some key examples:
+
+### Simple Chat Example using llama.cpp server backend
+This example demonstrates how to initiate a chat with an LLM model using the llama.cpp server backend. It supports llama-cpp-python Llama class instances, OpenAI endpoints with GBNF grammar support, and the llama.cpp backend server.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/simple-chat-example/)
+
+### Parallel Function Calling Agent Example
+This example showcases parallel function calling using the FunctionCallingAgent class. It demonstrates how to define and execute multiple functions concurrently.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/parallel_function_calling/)
+
+### Structured Output
+This example illustrates how to generate structured output objects using the StructuredOutputAgent class. It shows how to create a dataset entry of a book from unstructured data.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/structured-output-example/)
+
+### RAG - Retrieval Augmented Generation
+This example demonstrates Retrieval Augmented Generation (RAG) with colbert reranking. It requires installing the optional rag dependencies (ragatouille).
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/rag/)
+
+### llama-index Tools Example
+This example shows how to use llama-index tools and query engines with the FunctionCallingAgent class.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/llama_index_tool_use/)
+
+### Sequential Chain Example
+This example demonstrates how to create a complete product launch campaign using a sequential chain.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/sequential_chain/)
+
+### Mapping Chain Example
+This example illustrates how to create a mapping chain to summarize multiple articles into a single summary.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/map_chain/)
+
+### Knowledge Graph Creation Example
+This example, based on an example from the Instructor library for OpenAI, shows how to create a knowledge graph using the llama-cpp-agent framework.
+
+[View Example](https://llama-cpp-agent.readthedocs.io/en/latest/knowledge-graph-example/)
+
+
+## Additional Information
+
+### Predefined Messages Formatter
+
+The llama-cpp-agent framework provides predefined message formatters to format messages for the LLM model. The `MessagesFormatterType` enum defines the available formatters:
+
+- `MessagesFormatterType.MISTRAL`: Formats messages using the MISTRAL format.
+- `MessagesFormatterType.CHATML`: Formats messages using the CHATML format.
+- `MessagesFormatterType.VICUNA`: Formats messages using the VICUNA format.
+- `MessagesFormatterType.LLAMA_2`: Formats messages using the LLAMA 2 format.
+- `MessagesFormatterType.SYNTHIA`: Formats messages using the SYNTHIA format.
+- `MessagesFormatterType.NEURAL_CHAT`: Formats messages using the NEURAL CHAT format.
+- `MessagesFormatterType.SOLAR`: Formats messages using the SOLAR format.
+- `MessagesFormatterType.OPEN_CHAT`: Formats messages using the OPEN CHAT format.
+- `MessagesFormatterType.ALPACA`: Formats messages using the ALPACA format.
+- `MessagesFormatterType.CODE_DS`: Formats messages using the CODE DS format.
+- `MessagesFormatterType.B22`: Formats messages using the B22 format.
+- `MessagesFormatterType.LLAMA_3`: Formats messages using the LLAMA 3 format.
+- `MessagesFormatterType.PHI_3`: Formats messages using the PHI 3 format.
+
+### Creating Custom Messages Formatter
+
+You can create your own custom messages formatter by instantiating the `MessagesFormatter` class with the desired parameters:
+
+```python
+from llama_cpp_agent.messages_formatter import MessagesFormatter, PromptMarkers, Roles
+
+custom_prompt_markers = {
+    Roles.system: PromptMarkers("<|system|>", "<|endsystem|>"),
+    Roles.user: PromptMarkers("<|user|>", "<|enduser|>"),
+    Roles.assistant: PromptMarkers("<|assistant|>", "<|endassistant|>"),
+    Roles.tool: PromptMarkers("<|tool|>", "<|endtool|>"),
+}
+
+custom_formatter = MessagesFormatter(
+    pre_prompt="",
+    prompt_markers=custom_prompt_markers,
+    include_sys_prompt_in_first_user_message=False,
+    default_stop_sequences=["<|endsystem|>", "<|enduser|>", "<|endassistant|>", "<|endtool|>"]
+)
+```
+
+## Contributing
+We welcome contributions to the llama-cpp-agent framework! If you'd like to contribute, please follow these guidelines:
+
+1. Fork the repository and create your branch from `master`.
+2. Ensure your code follows the project's coding style and conventions.
+3. Write clear, concise commit messages and pull request descriptions.
+4. Test your changes thoroughly before submitting a pull request.
+5. Open a pull request to the `master` branch.
+
+If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/Maximilian-Winter/llama-cpp-agent/issues).
+
+## License
+The llama-cpp-agent framework is released under the [MIT License](https://github.com/Maximilian-Winter/llama-cpp-agent/blob/master/LICENSE).
+
+## FAQ
+
+**Q: How do I install the optional dependencies for RAG?**  
+A: To use the RAGColbertReranker class and the RAG example, you need to install the optional rag dependencies (ragatouille). You can do this by running `pip install llama-cpp-agent[rag]`.
+
+**Q: Can I contribute to the llama-cpp-agent project?**  
+A: Absolutely! We welcome contributions from the community. Please refer to the [Contributing](#contributing) section for guidelines on how to contribute.
+
+**Q: Is llama-cpp-agent compatible with the latest version of llama-cpp-python?**  
+A: Yes, llama-cpp-agent is designed to work with the latest version of llama-cpp-python. However, if you encounter any compatibility issues, please open an issue on the GitHub repository.
```

### Comparing `llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/SOURCES.txt` & `llama_cpp_agent-0.2.4/src/llama_cpp_agent.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-README.md
 ReadMe.md
 pyproject.toml
 src/llama_cpp_agent/__init__.py
 src/llama_cpp_agent/chain.py
 src/llama_cpp_agent/function_calling.py
 src/llama_cpp_agent/function_calling_agent.py
 src/llama_cpp_agent/hermes_2_pro_agent.py
```

