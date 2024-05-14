# Comparing `tmp/llama_cpp_agent-0.2.5.tar.gz` & `tmp/llama_cpp_agent-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_cpp_agent-0.2.5.tar", last modified: Mon May 13 22:06:35 2024, max compression
+gzip compressed data, was "llama_cpp_agent-0.2.6.tar", last modified: Tue May 14 01:13:30 2024, max compression
```

## Comparing `llama_cpp_agent-0.2.5.tar` & `llama_cpp_agent-0.2.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:35.353949 llama_cpp_agent-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-13 22:06:35.353949 llama_cpp_agent-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/ReadMe.md
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 22:06:35.353949 llama_cpp_agent-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:35.341949 llama_cpp_agent-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:35.345949 llama_cpp_agent-0.2.5/src/llama_cpp_agent/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:35.349949 llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/core_memory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/event_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/event_memory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/memory_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/retrieval_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:35.349949 llama_cpp_agent-0.2.5/src/llama_cpp_agent/chat_history/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/chat_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/chat_history/basic_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/chat_history/chat_history_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/chat_history/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/function_calling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/function_calling_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:35.349949 llama_cpp_agent-0.2.5/src/llama_cpp_agent/gbnf_grammar_generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51567 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/hermes_2_pro_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:35.349949 llama_cpp_agent-0.2.5/src/llama_cpp_agent/json_schema_generator/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/json_schema_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/json_schema_generator/schema_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21015 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/llm_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:35.349949 llama_cpp_agent-0.2.5/src/llama_cpp_agent/llm_documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/llm_documentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18378 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/llm_documentation/documentation_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:35.349949 llama_cpp_agent-0.2.5/src/llama_cpp_agent/llm_output_settings/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/llm_output_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32249 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/llm_output_settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/llm_prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/messages_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/mixtral_8x22b_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/prompt_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:35.353949 llama_cpp_agent-0.2.5/src/llama_cpp_agent/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/providers/llama_cpp_python.py
--rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/providers/llama_cpp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/providers/provider_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/providers/tgi_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/providers/vllm_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:35.353949 llama_cpp_agent-0.2.5/src/llama_cpp_agent/rag/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/rag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/rag/rag_colbert_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/structured_output_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-13 22:06:30.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:06:35.353949 llama_cpp_agent-0.2.5/src/llama_cpp_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-13 22:06:35.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-13 22:06:35.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:06:35.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-13 22:06:35.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 22:06:35.000000 llama_cpp_agent-0.2.5/src/llama_cpp_agent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:30.400668 llama_cpp_agent-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-14 01:13:30.400668 llama_cpp_agent-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/ReadMe.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:13:30.400668 llama_cpp_agent-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:30.392668 llama_cpp_agent-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:30.396668 llama_cpp_agent-0.2.6/src/llama_cpp_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:30.396668 llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/core_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/event_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/event_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/memory_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/retrieval_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:30.396668 llama_cpp_agent-0.2.6/src/llama_cpp_agent/chat_history/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/chat_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/chat_history/basic_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/chat_history/chat_history_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/chat_history/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/function_calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/function_calling_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:30.396668 llama_cpp_agent-0.2.6/src/llama_cpp_agent/gbnf_grammar_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51567 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/hermes_2_pro_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:30.396668 llama_cpp_agent-0.2.6/src/llama_cpp_agent/json_schema_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/json_schema_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/json_schema_generator/schema_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21015 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/llm_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:30.396668 llama_cpp_agent-0.2.6/src/llama_cpp_agent/llm_documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/llm_documentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18378 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/llm_documentation/documentation_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:30.400668 llama_cpp_agent-0.2.6/src/llama_cpp_agent/llm_output_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/llm_output_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32249 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/llm_output_settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/llm_prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/messages_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/mixtral_8x22b_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/prompt_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:30.400668 llama_cpp_agent-0.2.6/src/llama_cpp_agent/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/providers/llama_cpp_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/providers/llama_cpp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/providers/provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/providers/tgi_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/providers/vllm_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:30.400668 llama_cpp_agent-0.2.6/src/llama_cpp_agent/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/rag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/rag/rag_colbert_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/structured_output_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-14 01:13:26.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:13:30.400668 llama_cpp_agent-0.2.6/src/llama_cpp_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-14 01:13:30.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-14 01:13:30.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 01:13:30.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 01:13:30.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:13:30.000000 llama_cpp_agent-0.2.6/src/llama_cpp_agent.egg-info/top_level.txt
```

### Comparing `llama_cpp_agent-0.2.5/LICENSE` & `llama_cpp_agent-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/PKG-INFO` & `llama_cpp_agent-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.2.5
+Version: 0.2.6
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llama_cpp_agent-0.2.5/ReadMe.md` & `llama_cpp_agent-0.2.6/ReadMe.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/pyproject.toml` & `llama_cpp_agent-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [  "setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llama-cpp-agent"
-version = "0.2.5"
+version = "0.2.6"
 description = "A framework for building LLM based AI agents with llama.cpp."
 
 readme = "ReadMe.md"
 dependencies = [
     "llama-cpp-python>=0.2.60",
     "pydantic>=2.5.3",
     "requests>=2.31.0",
```

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/core_memory_manager.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/core_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/event_memory.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/event_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/event_memory_manager.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/event_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/memory_tools.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/memory_tools.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/retrieval_memory.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/retrieval_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/chain.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/chain.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/chat_history/basic_chat_history.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/chat_history/basic_chat_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,17 +108,22 @@
             )
 
     def get_message_store(self) -> BasicChatMessageStore:
         return self.message_store
 
     def get_chat_messages(self) -> List[Dict[str, str]]:
         if self.strategy == BasicChatHistoryStrategy.last_k_messages:
-            messages = [self.message_store.get_message(0)]
-            messages.extend(self.message_store.get_last_k_messages(self.k - 1))
-            return convert_messages_to_list_of_dictionaries(messages)
+            converted_messages = convert_messages_to_list_of_dictionaries(
+                self.message_store.get_last_k_messages(self.k - 1)
+            )
+            if len(converted_messages) == self.k and converted_messages[0]["role"] != "system":
+                messages = [convert_messages_to_list_of_dictionaries(self.message_store.get_message(0))]
+                messages.extend(converted_messages[1:])
+                return messages
+            return converted_messages
         elif self.strategy == BasicChatHistoryStrategy.last_k_tokens:
             total_tokens = 0
             selected_messages = []
             converted_messages = convert_messages_to_list_of_dictionaries(
                 self.message_store.get_all_messages()
             )
             sys_message = None
```

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/chat_history/chat_history_base.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/chat_history/chat_history_base.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/chat_history/messages.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/chat_history/messages.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/function_calling.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/function_calling.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/function_calling_agent.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/function_calling_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 from copy import copy
 from typing import Type, List, Callable, Union, Literal
 
 from llama_cpp import Llama
 from pydantic import BaseModel, Field
 
+from .chat_history.messages import Roles
 from .llm_output_settings import LlmStructuredOutputSettings, LlmStructuredOutputType
 
 from .llm_agent import LlamaCppAgent, StreamingResponse
 from .messages_formatter import MessagesFormatterType, MessagesFormatter
 from .function_calling import LlamaCppFunctionTool
 
 from .providers.provider_base import LlmProvider, LlmSamplingSettings
@@ -220,15 +221,15 @@
 
     def generate_response(
         self,
         message: str,
         llm_sampling_settings: LlmSamplingSettings = None,
         structured_output_settings: LlmStructuredOutputSettings = None,
     ):
-        self.llama_cpp_agent.add_message(role="user", message=message)
+        self.llama_cpp_agent.add_message(role=Roles.user, message=message)
 
         result = self.intern_get_response(llm_sampling_settings=llm_sampling_settings)
 
         while True:
             if isinstance(result, str):
                 if len(self.without_grammar_mode_function) > 0:
                     func_list = []
@@ -249,15 +250,15 @@
                         if "params" in res:
                             function_message += f"""{count}. Function: "{res["function"]}"\nArguments: "{res["params"]}"\nReturn Value: {res["return_value"]}\n\n"""
                         else:
                             function_message += f"""{count}. Function: "{res["function"]}"\nReturn Value: {res["return_value"]}\n\n"""
                     else:
                         function_message += f"{count}. " + res + "\n\n"
                 self.llama_cpp_agent.add_message(
-                    role="tool", message=function_message.strip()
+                    role=Roles.tool, message=function_message.strip()
                 )
                 if agent_sent_message:
                     break
             result = self.intern_get_response(
                 llm_sampling_settings=llm_sampling_settings
             )
         return result
```

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/hermes_2_pro_agent.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/hermes_2_pro_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/json_schema_generator/schema_generator.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/json_schema_generator/schema_generator.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/llm_agent.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/llm_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/llm_documentation/documentation_generation.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/llm_documentation/documentation_generation.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/llm_output_settings/settings.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/llm_output_settings/settings.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/llm_prompt_template.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/llm_prompt_template.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/messages_formatter.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/messages_formatter.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/mixtral_8x22b_agent.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/mixtral_8x22b_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/output_parser.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/prompt_templates.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/prompts.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/providers/llama_cpp_python.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/providers/llama_cpp_python.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/providers/llama_cpp_server.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/providers/llama_cpp_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/providers/provider_base.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/providers/provider_base.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/providers/tgi_server.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/providers/tgi_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/providers/vllm_server.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/providers/vllm_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/rag/rag_colbert_reranker.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/rag/rag_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/structured_output_agent.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/structured_output_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent/text_utils.py` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent/text_utils.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent.egg-info/PKG-INFO` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.2.5
+Version: 0.2.6
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llama_cpp_agent-0.2.5/src/llama_cpp_agent.egg-info/SOURCES.txt` & `llama_cpp_agent-0.2.6/src/llama_cpp_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

