# Comparing `tmp/llama_cpp_agent-0.2.2.tar.gz` & `tmp/llama_cpp_agent-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_cpp_agent-0.2.2.tar", last modified: Sun May 12 23:03:07 2024, max compression
+gzip compressed data, was "llama_cpp_agent-0.2.3.tar", last modified: Mon May 13 21:03:01 2024, max compression
```

## Comparing `llama_cpp_agent-0.2.2.tar` & `llama_cpp_agent-0.2.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 23:03:07.348589 llama_cpp_agent-0.2.2/
--rw-rw-rw-   0        0        0     1115 2023-12-31 18:08:30.000000 llama_cpp_agent-0.2.2/LICENSE
--rw-rw-rw-   0        0        0    10023 2024-05-12 23:03:07.347082 llama_cpp_agent-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     8798 2024-05-12 19:32:32.000000 llama_cpp_agent-0.2.2/ReadMe.md
--rw-rw-rw-   0        0        0     1054 2024-05-12 23:02:47.000000 llama_cpp_agent-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 23:03:07.348589 llama_cpp_agent-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-12 23:03:07.308616 llama_cpp_agent-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-12 23:03:07.323478 llama_cpp_agent-0.2.2/src/llama_cpp_agent/
--rw-rw-rw-   0        0        0      342 2024-05-12 15:02:27.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 23:03:07.332022 llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/
--rw-rw-rw-   0        0        0        0 2023-12-31 14:27:21.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/__init__.py
--rw-rw-rw-   0        0        0     3408 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/core_memory_manager.py
--rw-rw-rw-   0        0        0     1654 2024-05-11 19:58:35.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/event_memory.py
--rw-rw-rw-   0        0        0     3882 2024-05-11 19:58:35.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/event_memory_manager.py
--rw-rw-rw-   0        0        0     9949 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/memory_tools.py
--rw-rw-rw-   0        0        0     5031 2024-04-18 21:27:19.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/retrieval_memory.py
--rw-rw-rw-   0        0        0     1640 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
--rw-rw-rw-   0        0        0    12570 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/chain.py
-drwxrwxrwx   0        0        0        0 2024-05-12 23:03:07.334021 llama_cpp_agent-0.2.2/src/llama_cpp_agent/chat_history/
--rw-rw-rw-   0        0        0      307 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/chat_history/__init__.py
--rw-rw-rw-   0        0        0     6999 2024-05-12 00:16:58.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/chat_history/basic_chat_history.py
--rw-rw-rw-   0        0        0     1834 2024-05-12 00:07:51.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/chat_history/chat_history_base.py
--rw-rw-rw-   0        0        0     3113 2024-05-12 20:46:35.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/chat_history/messages.py
--rw-rw-rw-   0        0        0    10771 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/function_calling.py
--rw-rw-rw-   0        0        0    12448 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/function_calling_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-12 23:03:07.335022 llama_cpp_agent-0.2.2/src/llama_cpp_agent/gbnf_grammar_generator/
--rw-rw-rw-   0        0        0        0 2023-12-27 02:55:26.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
--rw-rw-rw-   0        0        0    52886 2024-05-11 21:21:16.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
--rw-rw-rw-   0        0        0    13675 2024-05-12 13:59:03.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/hermes_2_pro_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-12 23:03:07.337021 llama_cpp_agent-0.2.2/src/llama_cpp_agent/json_schema_generator/
--rw-rw-rw-   0        0        0       53 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/json_schema_generator/__init__.py
--rw-rw-rw-   0        0        0    11683 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/json_schema_generator/schema_generator.py
--rw-rw-rw-   0        0        0    21379 2024-05-12 20:44:35.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/llm_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-12 23:03:07.338526 llama_cpp_agent-0.2.2/src/llama_cpp_agent/llm_documentation/
--rw-rw-rw-   0        0        0      116 2024-05-09 08:09:41.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/llm_documentation/__init__.py
--rw-rw-rw-   0        0        0    18850 2024-05-12 00:42:14.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/llm_documentation/documentation_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-12 23:03:07.339075 llama_cpp_agent-0.2.2/src/llama_cpp_agent/llm_output_settings/
--rw-rw-rw-   0        0        0       76 2024-05-09 12:50:53.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/llm_output_settings/__init__.py
--rw-rw-rw-   0        0        0    32939 2024-05-12 05:26:57.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/llm_output_settings/settings.py
--rw-rw-rw-   0        0        0     7027 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/llm_prompt_template.py
--rw-rw-rw-   0        0        0    22304 2024-05-12 23:00:15.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/messages_formatter.py
--rw-rw-rw-   0        0        0     3990 2024-05-12 13:53:06.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/mixtral_8x22b_agent.py
--rw-rw-rw-   0        0        0     3613 2024-04-18 21:27:19.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/output_parser.py
--rw-rw-rw-   0        0        0     5296 2024-05-12 04:02:32.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/prompt_templates.py
--rw-rw-rw-   0        0        0      816 2024-05-12 03:46:37.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/prompts.py
-drwxrwxrwx   0        0        0        0 2024-05-12 23:03:07.344081 llama_cpp_agent-0.2.2/src/llama_cpp_agent/providers/
--rw-rw-rw-   0        0        0      277 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/providers/__init__.py
--rw-rw-rw-   0        0        0     8076 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/providers/llama_cpp_python.py
--rw-rw-rw-   0        0        0    13772 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/providers/llama_cpp_server.py
--rw-rw-rw-   0        0        0     5392 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/providers/provider_base.py
--rw-rw-rw-   0        0        0     9067 2024-05-12 03:32:34.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/providers/tgi_server.py
--rw-rw-rw-   0        0        0     6607 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/providers/vllm_server.py
-drwxrwxrwx   0        0        0        0 2024-05-12 23:03:07.345081 llama_cpp_agent-0.2.2/src/llama_cpp_agent/rag/
--rw-rw-rw-   0        0        0        0 2024-05-05 05:07:17.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/rag/__init__.py
--rw-rw-rw-   0        0        0     2359 2024-05-05 05:07:17.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/rag/rag_colbert_reranker.py
--rw-rw-rw-   0        0        0     7073 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/structured_output_agent.py
--rw-rw-rw-   0        0        0     3945 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent/text_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 23:03:07.346080 llama_cpp_agent-0.2.2/src/llama_cpp_agent.egg-info/
--rw-rw-rw-   0        0        0    10023 2024-05-12 23:03:07.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2187 2024-05-12 23:03:07.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 23:03:07.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      206 2024-05-12 23:03:07.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-12 23:03:07.000000 llama_cpp_agent-0.2.2/src/llama_cpp_agent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.892000 llama_cpp_agent-0.2.3/
+-rw-rw-rw-   0        0        0     1115 2023-12-31 18:08:30.000000 llama_cpp_agent-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0    10780 2024-05-13 21:03:01.891000 llama_cpp_agent-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9555 2024-05-13 20:57:26.000000 llama_cpp_agent-0.2.3/ReadMe.md
+-rw-rw-rw-   0        0        0     1054 2024-05-13 20:58:24.000000 llama_cpp_agent-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 21:03:01.892000 llama_cpp_agent-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.841326 llama_cpp_agent-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.860837 llama_cpp_agent-0.2.3/src/llama_cpp_agent/
+-rw-rw-rw-   0        0        0      342 2024-05-12 15:02:27.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.871347 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/
+-rw-rw-rw-   0        0        0        0 2023-12-31 14:27:21.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/__init__.py
+-rw-rw-rw-   0        0        0     3408 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/core_memory_manager.py
+-rw-rw-rw-   0        0        0     1654 2024-05-11 19:58:35.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/event_memory.py
+-rw-rw-rw-   0        0        0     3882 2024-05-11 19:58:35.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/event_memory_manager.py
+-rw-rw-rw-   0        0        0     9949 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/memory_tools.py
+-rw-rw-rw-   0        0        0     5031 2024-04-18 21:27:19.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/retrieval_memory.py
+-rw-rw-rw-   0        0        0     1640 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
+-rw-rw-rw-   0        0        0    12570 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/chain.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.874347 llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/
+-rw-rw-rw-   0        0        0      307 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/__init__.py
+-rw-rw-rw-   0        0        0     7628 2024-05-13 19:57:48.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/basic_chat_history.py
+-rw-rw-rw-   0        0        0     5417 2024-05-13 20:23:09.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/chat_history_base.py
+-rw-rw-rw-   0        0        0     3113 2024-05-12 20:46:35.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/messages.py
+-rw-rw-rw-   0        0        0    10771 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/function_calling.py
+-rw-rw-rw-   0        0        0    12448 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/function_calling_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.875485 llama_cpp_agent-0.2.3/src/llama_cpp_agent/gbnf_grammar_generator/
+-rw-rw-rw-   0        0        0        0 2023-12-27 02:55:26.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
+-rw-rw-rw-   0        0        0    52886 2024-05-11 21:21:16.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
+-rw-rw-rw-   0        0        0    13675 2024-05-12 13:59:03.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/hermes_2_pro_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.877486 llama_cpp_agent-0.2.3/src/llama_cpp_agent/json_schema_generator/
+-rw-rw-rw-   0        0        0       53 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/json_schema_generator/__init__.py
+-rw-rw-rw-   0        0        0    11683 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/json_schema_generator/schema_generator.py
+-rw-rw-rw-   0        0        0    21474 2024-05-13 20:02:22.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.879486 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_documentation/
+-rw-rw-rw-   0        0        0      116 2024-05-09 08:09:41.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_documentation/__init__.py
+-rw-rw-rw-   0        0        0    18850 2024-05-12 00:42:14.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_documentation/documentation_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.881487 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_output_settings/
+-rw-rw-rw-   0        0        0       76 2024-05-09 12:50:53.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_output_settings/__init__.py
+-rw-rw-rw-   0        0        0    32939 2024-05-12 05:26:57.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_output_settings/settings.py
+-rw-rw-rw-   0        0        0     7027 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_prompt_template.py
+-rw-rw-rw-   0        0        0    11752 2024-05-13 19:22:50.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/messages_formatter.py
+-rw-rw-rw-   0        0        0     3990 2024-05-12 13:53:06.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/mixtral_8x22b_agent.py
+-rw-rw-rw-   0        0        0     3613 2024-04-18 21:27:19.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/output_parser.py
+-rw-rw-rw-   0        0        0     5296 2024-05-12 04:02:32.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/prompt_templates.py
+-rw-rw-rw-   0        0        0      816 2024-05-12 03:46:37.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/prompts.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.886491 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/
+-rw-rw-rw-   0        0        0      277 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/__init__.py
+-rw-rw-rw-   0        0        0     8062 2024-05-13 00:41:32.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/llama_cpp_python.py
+-rw-rw-rw-   0        0        0    13758 2024-05-13 00:41:32.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/llama_cpp_server.py
+-rw-rw-rw-   0        0        0     5392 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/provider_base.py
+-rw-rw-rw-   0        0        0     9155 2024-05-13 00:41:32.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/tgi_server.py
+-rw-rw-rw-   0        0        0     6621 2024-05-13 00:41:32.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/vllm_server.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.889000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/rag/
+-rw-rw-rw-   0        0        0        0 2024-05-05 05:07:17.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/rag/__init__.py
+-rw-rw-rw-   0        0        0     2359 2024-05-05 05:07:17.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/rag/rag_colbert_reranker.py
+-rw-rw-rw-   0        0        0     7073 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/structured_output_agent.py
+-rw-rw-rw-   0        0        0     3945 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent/text_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:03:01.889999 llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/
+-rw-rw-rw-   0        0        0    10780 2024-05-13 21:03:01.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2197 2024-05-13 21:03:01.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 21:03:01.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      206 2024-05-13 21:03:01.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-13 21:03:01.000000 llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/top_level.txt
```

### Comparing `llama_cpp_agent-0.2.2/LICENSE` & `llama_cpp_agent-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/PKG-INFO` & `llama_cpp_agent-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.2.2
+Version: 0.2.3
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,18 @@
 Provides-Extra: vllm-provider
 Requires-Dist: openai; extra == "vllm-provider"
 Provides-Extra: mixtral-agent
 Requires-Dist: mistral-common; extra == "mixtral-agent"
 
 # llama-cpp-agent
 
-<img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/db41b3184ebc902f50edbd3d27f7a3a1128b7d7d/logo/logo_orange.png" alt="llama-cpp-agent logo" width="400"/>
+[![PyPI - Version](https://img.shields.io/pypi/v/llama-cpp-agent?logo=pypi&color=%2341bb13)](https://pypi.org/project/llama-cpp-agent/)
+[![Discord](https://img.shields.io/discord/1237393014154985582?logo=Discord&logoColor=%23ffffff&label=Discord&link=https%3A%2F%2Fdiscord.gg%2FsRMvWKrh)](https://discord.gg/sRMvWKrh)
+
+<img src="./logo/logo_orange.png" alt="llama-cpp-agent logo" width="280"/>
 
 ## Introduction
 The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
 
 The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
 
 The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
@@ -133,41 +136,50 @@
 
 [View Example](https://llama-cpp-agent.readthedocs.io/en/latest/knowledge-graph-example/)
 
 
 ## Additional Information
 
 ### Predefined Messages Formatter
+
 The llama-cpp-agent framework provides predefined message formatters to format messages for the LLM model. The `MessagesFormatterType` enum defines the available formatters:
 
+- `MessagesFormatterType.MISTRAL`: Formats messages using the MISTRAL format.
 - `MessagesFormatterType.CHATML`: Formats messages using the CHATML format.
-- `MessagesFormatterType.MIXTRAL`: Formats messages using the MIXTRAL format.
 - `MessagesFormatterType.VICUNA`: Formats messages using the VICUNA format.
 - `MessagesFormatterType.LLAMA_2`: Formats messages using the LLAMA 2 format.
 - `MessagesFormatterType.SYNTHIA`: Formats messages using the SYNTHIA format.
 - `MessagesFormatterType.NEURAL_CHAT`: Formats messages using the NEURAL CHAT format.
 - `MessagesFormatterType.SOLAR`: Formats messages using the SOLAR format.
 - `MessagesFormatterType.OPEN_CHAT`: Formats messages using the OPEN CHAT format.
+- `MessagesFormatterType.ALPACA`: Formats messages using the ALPACA format.
+- `MessagesFormatterType.CODE_DS`: Formats messages using the CODE DS format.
+- `MessagesFormatterType.B22`: Formats messages using the B22 format.
+- `MessagesFormatterType.LLAMA_3`: Formats messages using the LLAMA 3 format.
+- `MessagesFormatterType.PHI_3`: Formats messages using the PHI 3 format.
 
 ### Creating Custom Messages Formatter
+
 You can create your own custom messages formatter by instantiating the `MessagesFormatter` class with the desired parameters:
 
 ```python
-from llama_cpp_agent.messages_formatter import MessagesFormatter
+from llama_cpp_agent.chat_history.messages_formatter import MessagesFormatter, PromptMarkers, Roles
+
+custom_prompt_markers = {
+    Roles.system: PromptMarkers("<|system|>", "<|endsystem|>"),
+    Roles.user: PromptMarkers("<|user|>", "<|enduser|>"),
+    Roles.assistant: PromptMarkers("<|assistant|>", "<|endassistant|>"),
+    Roles.tool: PromptMarkers("<|tool|>", "<|endtool|>"),
+}
 
 custom_formatter = MessagesFormatter(
-    PRE_PROMPT="",
-    SYS_PROMPT_START="<|system|>",
-    SYS_PROMPT_END="<|endsystem|>",
-    USER_PROMPT_START="<|user|>",
-    USER_PROMPT_END="<|enduser|>",
-    ASSISTANT_PROMPT_START="<|assistant|>",
-    ASSISTANT_PROMPT_END="<|endassistant|>",
-    INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE=False,
-    DEFAULT_STOP_SEQUENCES=["<|endsystem|>", "<|enduser|>", "<|endassistant|>"]
+    pre_prompt="",
+    prompt_markers=custom_prompt_markers,
+    include_sys_prompt_in_first_user_message=False,
+    default_stop_sequences=["<|endsystem|>", "<|enduser|>", "<|endassistant|>", "<|endtool|>"]
 )
 ```
 
 ## Contributing
 We welcome contributions to the llama-cpp-agent framework! If you'd like to contribute, please follow these guidelines:
 
 1. Fork the repository and create your branch from `master`.
```

### Comparing `llama_cpp_agent-0.2.2/ReadMe.md` & `llama_cpp_agent-0.2.3/ReadMe.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # llama-cpp-agent
 
-<img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/db41b3184ebc902f50edbd3d27f7a3a1128b7d7d/logo/logo_orange.png" alt="llama-cpp-agent logo" width="400"/>
+[![PyPI - Version](https://img.shields.io/pypi/v/llama-cpp-agent?logo=pypi&color=%2341bb13)](https://pypi.org/project/llama-cpp-agent/)
+[![Discord](https://img.shields.io/discord/1237393014154985582?logo=Discord&logoColor=%23ffffff&label=Discord&link=https%3A%2F%2Fdiscord.gg%2FsRMvWKrh)](https://discord.gg/sRMvWKrh)
+
+<img src="./logo/logo_orange.png" alt="llama-cpp-agent logo" width="280"/>
 
 ## Introduction
 The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
 
 The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
 
 The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
@@ -103,41 +106,50 @@
 
 [View Example](https://llama-cpp-agent.readthedocs.io/en/latest/knowledge-graph-example/)
 
 
 ## Additional Information
 
 ### Predefined Messages Formatter
+
 The llama-cpp-agent framework provides predefined message formatters to format messages for the LLM model. The `MessagesFormatterType` enum defines the available formatters:
 
+- `MessagesFormatterType.MISTRAL`: Formats messages using the MISTRAL format.
 - `MessagesFormatterType.CHATML`: Formats messages using the CHATML format.
-- `MessagesFormatterType.MIXTRAL`: Formats messages using the MIXTRAL format.
 - `MessagesFormatterType.VICUNA`: Formats messages using the VICUNA format.
 - `MessagesFormatterType.LLAMA_2`: Formats messages using the LLAMA 2 format.
 - `MessagesFormatterType.SYNTHIA`: Formats messages using the SYNTHIA format.
 - `MessagesFormatterType.NEURAL_CHAT`: Formats messages using the NEURAL CHAT format.
 - `MessagesFormatterType.SOLAR`: Formats messages using the SOLAR format.
 - `MessagesFormatterType.OPEN_CHAT`: Formats messages using the OPEN CHAT format.
+- `MessagesFormatterType.ALPACA`: Formats messages using the ALPACA format.
+- `MessagesFormatterType.CODE_DS`: Formats messages using the CODE DS format.
+- `MessagesFormatterType.B22`: Formats messages using the B22 format.
+- `MessagesFormatterType.LLAMA_3`: Formats messages using the LLAMA 3 format.
+- `MessagesFormatterType.PHI_3`: Formats messages using the PHI 3 format.
 
 ### Creating Custom Messages Formatter
+
 You can create your own custom messages formatter by instantiating the `MessagesFormatter` class with the desired parameters:
 
 ```python
-from llama_cpp_agent.messages_formatter import MessagesFormatter
+from llama_cpp_agent.chat_history.messages_formatter import MessagesFormatter, PromptMarkers, Roles
+
+custom_prompt_markers = {
+    Roles.system: PromptMarkers("<|system|>", "<|endsystem|>"),
+    Roles.user: PromptMarkers("<|user|>", "<|enduser|>"),
+    Roles.assistant: PromptMarkers("<|assistant|>", "<|endassistant|>"),
+    Roles.tool: PromptMarkers("<|tool|>", "<|endtool|>"),
+}
 
 custom_formatter = MessagesFormatter(
-    PRE_PROMPT="",
-    SYS_PROMPT_START="<|system|>",
-    SYS_PROMPT_END="<|endsystem|>",
-    USER_PROMPT_START="<|user|>",
-    USER_PROMPT_END="<|enduser|>",
-    ASSISTANT_PROMPT_START="<|assistant|>",
-    ASSISTANT_PROMPT_END="<|endassistant|>",
-    INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE=False,
-    DEFAULT_STOP_SEQUENCES=["<|endsystem|>", "<|enduser|>", "<|endassistant|>"]
+    pre_prompt="",
+    prompt_markers=custom_prompt_markers,
+    include_sys_prompt_in_first_user_message=False,
+    default_stop_sequences=["<|endsystem|>", "<|enduser|>", "<|endassistant|>", "<|endtool|>"]
 )
 ```
 
 ## Contributing
 We welcome contributions to the llama-cpp-agent framework! If you'd like to contribute, please follow these guidelines:
 
 1. Fork the repository and create your branch from `master`.
```

### Comparing `llama_cpp_agent-0.2.2/pyproject.toml` & `llama_cpp_agent-0.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [  "setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llama-cpp-agent"
-version = "0.2.2"
+version = "0.2.3"
 description = "A framework for building LLM based AI agents with llama.cpp."
 
 readme = "ReadMe.md"
 dependencies = [
     "llama-cpp-python>=0.2.60",
     "pydantic>=2.5.3",
     "requests>=2.31.0",
```

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/core_memory_manager.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/core_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/event_memory.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/event_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/event_memory_manager.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/event_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/memory_tools.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/memory_tools.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/retrieval_memory.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/retrieval_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/chain.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/chain.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/chat_history/basic_chat_history.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/basic_chat_history.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,41 +59,41 @@
         return self.messages[k:]
 
     def get_all_messages(self) -> List[ChatMessage]:
         return self.messages
 
     def save_to_json(self, file_path: str):
         # Convert messages to a list of dictionaries using pydantic's model_dump() method
-        messages_dict = [message.model_dump() for message in self.messages]
+        messages_dict = [{"role": message.role.value, "content": message.content} for message in self.messages]
         # Write the list of dictionaries to a JSON file
         with open(file_path, "w") as file:
             json.dump(messages_dict, file, indent=4)
 
     def load_from_json(self, file_path: str):
         # Read the list of dictionaries from a JSON file
         with open(file_path, "r") as file:
             messages_dict = json.load(file)
         # Convert dictionaries back to ChatMessage instances
-        self.messages = [
-            parse_obj_as(ChatMessage, message) for message in messages_dict
-        ]
+        self.messages = [SystemMessage(content=message["content"]) if message["role"] == "system" else
+                         UserMessage(content=message["content"]) if message["role"] == "user" else
+                         AssistantMessage(content=message["content"]) if message["role"] == "assistant" else
+                         ToolMessage(content=message["content"]) for message in messages_dict]
 
 
 class BasicChatHistoryStrategy(Enum):
     last_k_messages: str = "last_k_messages"
     last_k_tokens: str = "last_k_tokens"
 
 
 class BasicChatHistory(ChatHistory):
 
-
     def __init__(
             self,
             chat_history_strategy: BasicChatHistoryStrategy = BasicChatHistoryStrategy.last_k_messages,
-            k: int = 10,
+            k: int = 20,
             llm_provider: LlmProvider = None,
             message_store: ChatMessageStore = None,
     ):
         if message_store is None:
             message_store = BasicChatMessageStore()
         self.message_store: ChatMessageStore = message_store
         self.k = k
@@ -103,19 +103,22 @@
                 chat_history_strategy == BasicChatHistoryStrategy.last_k_tokens
                 and llm_provider is None
         ):
             raise Exception(
                 "Please pass a LLM provider to BasicChatHistory when using last k tokens as memory strategy!"
             )
 
+    def get_message_store(self) -> BasicChatMessageStore:
+        return self.message_store
+
     def get_chat_messages(self) -> List[Dict[str, str]]:
         if self.strategy == BasicChatHistoryStrategy.last_k_messages:
-            return convert_messages_to_list_of_dictionaries(
-                self.message_store.get_last_k_messages(self.k)
-            )
+            messages = [self.message_store.get_message(0)]
+            messages.extend(self.message_store.get_last_k_messages(self.k - 1))
+            return convert_messages_to_list_of_dictionaries(messages)
         elif self.strategy == BasicChatHistoryStrategy.last_k_tokens:
             total_tokens = 0
             selected_messages = []
             converted_messages = convert_messages_to_list_of_dictionaries(
                 self.message_store.get_all_messages()
             )
             sys_message = None
@@ -134,44 +137,52 @@
                     selected_messages.append(message)
             if sys_message is not None:
                 selected_messages.append(sys_message)
             return list(reversed(selected_messages))
         return []
 
     def add_message(self, message: Dict[str, str]):
-        if message["role"] == "system":
+        if message["role"] == Roles.system:
             self.message_store.add_message(
                 SystemMessage(content=message["content"])
             )
-        elif message["role"] == "user":
+        elif message["role"] == Roles.user:
             self.message_store.add_message(
                 UserMessage(content=message["content"])
             )
-        elif message["role"] == "assistant":
+        elif message["role"] == Roles.assistant:
             self.message_store.add_message(
                 AssistantMessage(content=message["content"])
             )
-        elif message["role"] == "tool":
+        elif message["role"] == Roles.tool:
             self.message_store.add_message(
                 ToolMessage(tool_call_id=generate_function_call_id(), content=message["content"])
             )
 
     def get_messages_count(self):
         return self.message_store.get_messages_count()
 
     def edit_message(self, index: int, message: Dict[str, str]):
-        if message["role"] == "system":
-            self.message_store.edit_message(index,
-                                            SystemMessage(content=message["content"])
-                                            )
-        elif message["role"] == "user":
-            self.message_store.edit_message(index,
-                                            UserMessage(content=message["content"])
-                                            )
-        elif message["role"] == "assistant":
-            self.message_store.edit_message(index,
-                                            AssistantMessage(content=message["content"])
-                                            )
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
 
     def get_message(self, index) -> Dict[str, str]:
         message = self.message_store.get_message(index)
-        return {"role": message.role, "content": message.content}
+        return {"role": message.role, "content": message.content}
```

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/chat_history/messages.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/chat_history/messages.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/function_calling.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/function_calling.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/function_calling_agent.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/function_calling_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/hermes_2_pro_agent.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/hermes_2_pro_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/json_schema_generator/schema_generator.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/json_schema_generator/schema_generator.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/llm_agent.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dataclasses import dataclass
 from typing import List, Literal, Callable, Union, Generator, Any
 
 from pydantic import BaseModel
 
 from .chat_history.basic_chat_history import BasicChatHistory
 from .chat_history.chat_history_base import ChatHistory
+from .chat_history.messages import Roles
 
 from .llm_output_settings import LlmStructuredOutputSettings, LlmStructuredOutputType
 
 from .messages_formatter import (
     MessagesFormatterType,
     get_predefined_messages_formatter,
     MessagesFormatter,
@@ -84,25 +85,22 @@
             )
         self.last_response = ""
         if chat_history is None:
             self.chat_history = BasicChatHistory()
         else:
             self.chat_history = chat_history
 
-        self.add_message(role="system", message=system_prompt)
+        self.add_message(role=Roles.system, message=system_prompt)
         self.system_prompt = system_prompt
         self.add_tools_and_structures_documentation_to_system_prompt = add_tools_and_structures_documentation_to_system_prompt
 
     def add_message(
             self,
             message: str,
-            role: Literal["system"]
-                  | Literal["user"]
-                  | Literal["assistant"]
-                  | Literal["tool"] = "user",
+            role: Roles,
     ):
         """
         Adds a message to the chat history.
 
         Args:
             message (str): The content of the message.
             role (Literal["system"] | Literal["user"] | Literal["assistant"] | Literal["tool"]): The role of the message sender.
@@ -154,15 +152,15 @@
         if llm_sampling_settings is None:
             llm_sampling_settings = self.provider.get_provider_default_settings()
         else:
             llm_sampling_settings = deepcopy(llm_sampling_settings)
 
         if llm_sampling_settings.get_additional_stop_sequences() is not None:
             llm_sampling_settings.add_additional_stop_sequences(
-                self.messages_formatter.DEFAULT_STOP_SEQUENCES
+                self.messages_formatter.default_stop_sequences
             )
 
         if self.provider:
             completion = self.get_text_completion(
                 prompt=prompt,
                 structured_output_settings=structured_output_settings,
                 llm_samplings_settings=llm_sampling_settings,
@@ -212,15 +210,15 @@
                     full_response
                 )
         return "Error: No model loaded!"
 
     def get_chat_response(
             self,
             message: str = None,
-            role: Literal["system", "user", "assistant", "tool"] = "user",
+            role: Roles = Roles.user,
             prompt_suffix: str = None,
             chat_history: ChatHistory = None,
             system_prompt: str = None,
             add_message_to_chat_history: bool = True,
             add_response_to_chat_history: bool = True,
             structured_output_settings: LlmStructuredOutputSettings = None,
             llm_sampling_settings: LlmSamplingSettings = None,
@@ -263,15 +261,15 @@
         if llm_sampling_settings is None:
             llm_sampling_settings = self.provider.get_provider_default_settings()
         else:
             llm_sampling_settings = deepcopy(llm_sampling_settings)
 
         if llm_sampling_settings.get_additional_stop_sequences() is not None:
             llm_sampling_settings.add_additional_stop_sequences(
-                self.messages_formatter.DEFAULT_STOP_SEQUENCES
+                self.messages_formatter.default_stop_sequences
             )
 
         completion, response_role = self.get_response_role_and_completion(
             message=message,
             chat_history=chat_history,
             system_prompt=system_prompt,
             add_message_to_chat_history=add_message_to_chat_history,
@@ -281,38 +279,37 @@
             llm_sampling_settings=llm_sampling_settings,
         )
 
         def stream_results():
             full_response_stream = ""
             for out_stream in completion:
                 out_text = out_stream["choices"][0]["text"]
-                if out_text != self.messages_formatter.EOS_TOKEN:
+                if out_text != self.messages_formatter.eos_token:
                     full_response_stream += text
                     yield out_text
             self.last_response = full_response
             if add_response_to_chat_history:
-                if response_role == "assistant":
-                    chat_history.add_message(
-                        {
-                            "role": response_role,
-                            "content": full_response,
-                        }
-                    )
+                chat_history.add_message(
+                    {
+                        "role": response_role,
+                        "content": full_response,
+                    }
+                )
             return structured_output_settings.handle_structured_output(
                 full_response_stream
             )
 
         if self.provider:
             if returns_streaming_generator:
                 return stream_results()
             if llm_sampling_settings.is_streaming():
                 full_response = ""
                 for out in completion:
                     text = out["choices"][0]["text"]
-                    if text != self.messages_formatter.EOS_TOKEN:
+                    if text != self.messages_formatter.eos_token:
                         full_response += text
                         if streaming_callback is not None:
                             streaming_callback(
                                 StreamingResponse(text=text, is_last_response=False)
                             )
                         if print_output or self.debug_output:
                             print(text, end="")
@@ -320,63 +317,62 @@
                     streaming_callback(
                         StreamingResponse(text="", is_last_response=True)
                     )
                 if print_output or self.debug_output:
                     print("")
                 self.last_response = full_response
                 if add_response_to_chat_history:
-                    if response_role == "assistant":
-                        chat_history.add_message(
-                            {
-                                "role": response_role,
-                                "content": full_response,
-                            }
-                        )
+                    chat_history.add_message(
+                        {
+                            "role": response_role,
+                            "content": full_response,
+                        }
+                    )
 
                 return structured_output_settings.handle_structured_output(
                     full_response
                 )
             else:
                 text = completion["choices"][0]["text"]
-                if text.strip().endswith(self.messages_formatter.EOS_TOKEN):
-                    text = text.replace(self.messages_formatter.EOS_TOKEN, "")
+                if text.strip().endswith(self.messages_formatter.eos_token):
+                    text = text.replace(self.messages_formatter.eos_token, "")
                 if print_output or self.debug_output:
                     print(text)
                 self.last_response = text
                 if add_response_to_chat_history:
-                    if response_role == "assistant":
-                        chat_history.add_message(
-                            {
-                                "role": response_role,
-                                "content": text,
-                            }
-                        )
+                    chat_history.add_message(
+                        {
+                            "role": response_role,
+                            "content": text,
+                        }
+                    )
+
                 return structured_output_settings.handle_structured_output(text)
         return "Error: No model loaded!"
 
     def get_text_completion(
             self,
             prompt: str | list[int] = None,
             structured_output_settings: LlmStructuredOutputSettings = None,
             llm_samplings_settings: LlmSamplingSettings = None,
     ):
         return self.provider.create_completion(
             prompt,
             structured_output_settings,
             llm_samplings_settings,
-            self.messages_formatter.BOS_TOKEN,
+            self.messages_formatter.bos_token,
         )
 
     def get_response_role_and_completion(
             self,
             message: str = None,
             chat_history: ChatHistory = None,
             system_prompt: str = None,
             add_message_to_chat_history: bool = True,
-            role: Literal["system", "user", "assistant", "tool"] = "user",
+            role: Roles = Roles.user,
             prompt_suffix: str = None,
             llm_sampling_settings: LlmSamplingSettings = None,
             structured_output_settings: LlmStructuredOutputSettings = None,
     ):
         if message is not None and add_message_to_chat_history:
             chat_history.add_message(
                 {
@@ -399,47 +395,63 @@
             messages[0]["content"] = self.system_prompt
         additional_suffix = ""
         if self.add_tools_and_structures_documentation_to_system_prompt:
             if structured_output_settings.output_type != LlmStructuredOutputType.no_structured_output:
                 additional_suffix = "\n"
                 if structured_output_settings.output_type == LlmStructuredOutputType.function_calling or structured_output_settings.output_type == LlmStructuredOutputType.parallel_function_calling:
                     if structured_output_settings.add_thoughts_and_reasoning_field and self.provider.is_using_json_schema_constraints():
-                        messages[0]["content"] += function_calling_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(provider=self.provider)
+                        messages[0][
+                            "content"] += function_calling_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
                     elif not structured_output_settings.add_thoughts_and_reasoning_field and self.provider.is_using_json_schema_constraints():
-                        messages[0]["content"] += function_calling_without_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(provider=self.provider)
+                        messages[0][
+                            "content"] += function_calling_without_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
                     elif structured_output_settings.add_thoughts_and_reasoning_field and not self.provider.is_using_json_schema_constraints():
-                        messages[0]["content"] += function_calling_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(provider=self.provider)
+                        messages[0][
+                            "content"] += function_calling_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
                     elif not structured_output_settings.add_thoughts_and_reasoning_field and not self.provider.is_using_json_schema_constraints():
-                        messages[0]["content"] += function_calling_without_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(provider=self.provider)
+                        messages[0][
+                            "content"] += function_calling_without_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
                 elif structured_output_settings.output_type == LlmStructuredOutputType.object_instance or structured_output_settings.output_type == LlmStructuredOutputType.list_of_objects:
                     if structured_output_settings.add_thoughts_and_reasoning_field and self.provider.is_using_json_schema_constraints():
-                        messages[0]["content"] += structured_output_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(provider=self.provider)
+                        messages[0][
+                            "content"] += structured_output_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
                     elif not structured_output_settings.add_thoughts_and_reasoning_field and self.provider.is_using_json_schema_constraints():
-                        messages[0]["content"] += structured_output_without_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(provider=self.provider)
+                        messages[0][
+                            "content"] += structured_output_without_thoughts_and_reasoning_json_schema + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
                     elif structured_output_settings.add_thoughts_and_reasoning_field and not self.provider.is_using_json_schema_constraints():
-                        messages[0]["content"] += structured_output_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(provider=self.provider)
+                        messages[0][
+                            "content"] += structured_output_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
                     elif not structured_output_settings.add_thoughts_and_reasoning_field and not self.provider.is_using_json_schema_constraints():
-                        messages[0]["content"] += structured_output_without_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(provider=self.provider)
+                        messages[0][
+                            "content"] += structured_output_without_thoughts_and_reasoning + structured_output_settings.get_llm_documentation(
+                            provider=self.provider)
 
-        prompt, response_role = self.messages_formatter.format_messages(
-            messages, "assistant"
+        prompt, response_role = self.messages_formatter.format_conversation(
+            messages, Roles.assistant
         )
 
         if prompt_suffix:
             prompt += prompt_suffix
         prompt += additional_suffix
         if self.debug_output:
             print(prompt, end="")
 
         return (
             self.provider.create_completion(
                 prompt,
                 structured_output_settings,
                 llm_sampling_settings,
-                self.messages_formatter.BOS_TOKEN,
+                self.messages_formatter.bos_token,
             ),
             response_role,
         )
 
     @staticmethod
     def remove_any(text, list_of_strings):
         for item in list_of_strings:
```

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/llm_documentation/documentation_generation.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_documentation/documentation_generation.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/llm_output_settings/settings.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_output_settings/settings.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/llm_prompt_template.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/llm_prompt_template.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/mixtral_8x22b_agent.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/mixtral_8x22b_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/output_parser.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/prompt_templates.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/prompts.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/providers/llama_cpp_python.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/llama_cpp_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from copy import copy
+from copy import deepcopy
 from dataclasses import dataclass
 from typing import List, Dict, Union
 
 from llama_cpp import Llama, LlamaGrammar
 
 from llama_cpp_agent.llm_output_settings import (
     LlmStructuredOutputSettings,
@@ -150,43 +150,42 @@
             grammar = structured_output_settings.get_gbnf_grammar()
             if grammar in self.grammar_cache:
                 grammar = self.grammar_cache[grammar]
             else:
                 self.grammar_cache[grammar] = LlamaGrammar.from_string(grammar)
                 grammar = self.grammar_cache[grammar]
 
-        settings_dictionary = copy(settings.as_dict())
+        settings_dictionary = deepcopy(settings.as_dict())
 
         settings_dictionary["stop"] = settings_dictionary.pop(
             "additional_stop_sequences"
         )
 
         return self.llama_model.create_completion(
             prompt, grammar=grammar, **settings_dictionary
         )
 
     def create_chat_completion(
         self,
         messages: List[Dict[str, str]],
         structured_output_settings: LlmStructuredOutputSettings,
-        settings: LlamaCppPythonSamplingSettings,
-        bos_token: str,
+        settings: LlamaCppPythonSamplingSettings
     ):
         grammar = None
         if (
             structured_output_settings.output_type
             != LlmStructuredOutputType.no_structured_output
         ):
             grammar = structured_output_settings.get_gbnf_grammar()
             if grammar in self.grammar_cache:
                 grammar = self.grammar_cache[grammar]
             else:
                 self.grammar_cache[grammar] = LlamaGrammar.from_string(grammar)
                 grammar = self.grammar_cache[grammar]
-        settings_dictionary = copy(settings.as_dict())
+        settings_dictionary = deepcopy(settings.as_dict())
         settings_dictionary["max_tokens"] = settings_dictionary.pop("n_predict")
         settings_dictionary["stop"] = settings_dictionary.pop("stop_sequences")
 
         return self.llama_model.create_chat_completion(
             messages, grammar=grammar, **settings_dictionary
         )
```

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/providers/llama_cpp_server.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/llama_cpp_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from copy import copy
+from copy import deepcopy
 from dataclasses import dataclass
 from typing import List, Dict, Union
 
 import requests
 
 from llama_cpp_agent.llm_output_settings import (
     LlmStructuredOutputType,
@@ -182,15 +182,15 @@
             headers = {
                 "Content-Type": "application/json",
                 "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
             }
         else:
             headers = {"Content-Type": "application/json"}
 
-        data = copy(settings.as_dict())
+        data = deepcopy(settings.as_dict())
         data["prompt"] = prompt
         data = self.prepare_generation_settings(data, structured_output_settings)
 
         if settings.stream:
             return self.get_response_stream(
                 headers, data, self.server_completion_endpoint
             )
@@ -203,26 +203,25 @@
         returned_data = {"choices": [{"text": data["content"]}]}
         return returned_data
 
     def create_chat_completion(
         self,
         messages: List[Dict[str, str]],
         structured_output_settings: LlmStructuredOutputSettings,
-        settings: LlamaCppSamplingSettings,
-        bos_token: str,
+        settings: LlamaCppSamplingSettings
     ):
         if self.api_key is not None:
             headers = {
                 "Content-Type": "application/json",
                 "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
             }
         else:
             headers = {"Content-Type": "application/json"}
 
-        data = copy(settings.as_dict())
+        data = deepcopy(settings.as_dict())
         data["messages"] = messages
         data = self.prepare_generation_settings(data, structured_output_settings)
         if settings.stream:
             return self.get_response_stream(
                 headers, data, self.server_chat_completion_endpoint
             )
         response = requests.post(
```

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/providers/provider_base.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/provider_base.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/providers/tgi_server.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/tgi_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from copy import copy
+from copy import deepcopy
 from dataclasses import dataclass, field
 from typing import List, Optional, Dict, Union
 
 import requests
 
 from llama_cpp_agent.llm_output_settings import (
     LlmStructuredOutputType,
@@ -85,57 +85,57 @@
             dict: The dictionary representation of the settings.
         """
         return self.__dict__
 
 
 class TGIServerProvider(LlmProvider):
 
-
     def __init__(self, server_address: str, api_key: str = None):
         self.server_address = server_address
         self.server_completion_endpoint = self.server_address + "/generate"
         self.server_streaming_completion_endpoint = (
-            self.server_address + "/generate_stream"
+                self.server_address + "/generate_stream"
         )
         self.server_chat_completion_endpoint = (
-            self.server_address + "/v1/chat/completions"
+                self.server_address + "/v1/chat/completions"
         )
         self.server_tokenize_endpoint = self.server_address + "/tokenize"
         self.api_key = api_key
 
     def is_using_json_schema_constraints(self):
         return True
+
     def get_provider_identifier(self) -> LlmProviderId:
         return LlmProviderId.tgi_server
 
     def get_provider_default_settings(self) -> TGIServerSamplingSettings:
         return TGIServerSamplingSettings()
 
     def create_completion(
-        self,
-        prompt: str,
-        structured_output_settings: LlmStructuredOutputSettings,
-        settings: TGIServerSamplingSettings,
-        bos_token: str,
+            self,
+            prompt: str,
+            structured_output_settings: LlmStructuredOutputSettings,
+            settings: TGIServerSamplingSettings,
+            bos_token: str,
     ):
         if self.api_key is not None:
             headers = {
                 "Content-Type": "application/json",
                 "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
             }
         else:
             headers = {"Content-Type": "application/json"}
 
-        settings_dict = copy(settings.as_dict())
+        settings_dict = deepcopy(settings.as_dict())
 
         data = {"parameters": settings_dict, "inputs": prompt}
         grammar = None
         if (
-            structured_output_settings.output_type
-            != LlmStructuredOutputType.no_structured_output
+                structured_output_settings.output_type
+                != LlmStructuredOutputType.no_structured_output
         ):
             grammar = structured_output_settings.get_json_schema()
 
         if grammar is not None:
             data["parameters"]["grammar"] = {"type": "json", "value": grammar}
         if settings.stream:
             return self.get_response_stream(
@@ -147,33 +147,33 @@
         )
         data = response.json()
 
         returned_data = {"choices": [{"text": data["generated_text"]}]}
         return returned_data
 
     def create_chat_completion(
-        self,
-        messages: List[Dict[str, str]],
-        structured_output_settings: LlmStructuredOutputSettings,
-        settings: TGIServerSamplingSettings
+            self,
+            messages: List[Dict[str, str]],
+            structured_output_settings: LlmStructuredOutputSettings,
+            settings: TGIServerSamplingSettings
     ):
         if self.api_key is not None:
             headers = {
                 "Content-Type": "application/json",
                 "Authorization": f"Bearer {self.api_key}",  # Add API key as bearer token
             }
         else:
             headers = {"Content-Type": "application/json"}
-        data = copy(settings.as_dict())
+        data = deepcopy(settings.as_dict())
         data["messages"] = messages
         data["model"] = "tgi"
         grammar = None
         if (
-            structured_output_settings.output_type
-            != LlmStructuredOutputType.no_structured_output
+                structured_output_settings.output_type
+                != LlmStructuredOutputType.no_structured_output
         ):
             grammar = structured_output_settings.get_json_schema()
 
         if grammar is not None:
             data["parameters"]["grammar"] = {"type": "json", "value": grammar}
         if settings.stream:
             return self.get_response_stream(
@@ -222,24 +222,24 @@
             try:
                 decoded_chunk = ""
                 for chunk in response.iter_lines():
                     if chunk:
                         decoded_chunk += chunk.decode("utf-8")
                         new_data = json.loads(decoded_chunk.replace("data:", ""))
                         if "token" in new_data and (
-                            new_data["token"]["text"] is not None
+                                new_data["token"]["text"] is not None
                         ):
                             returned_data = {
                                 "choices": [{"text": new_data["token"]["text"]}]
                             }
                             yield returned_data
                         elif (
-                            "choices" in new_data
-                            and (new_data["choices"][0]["delta"] is not None)
-                            and ("content" in new_data["choices"][0]["delta"])
+                                "choices" in new_data
+                                and (new_data["choices"][0]["delta"] is not None)
+                                and ("content" in new_data["choices"][0]["delta"])
                         ):
                             returned_data = {
                                 "choices": [
                                     {"text": new_data["choices"][0]["delta"]["content"]}
                                 ]
                             }
                             yield returned_data
```

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/providers/vllm_server.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/providers/vllm_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from copy import copy
+from copy import copy, deepcopy
 from dataclasses import dataclass, field
 from typing import List, Dict, Optional, Union
 
 from llama_cpp_agent.llm_output_settings import (
     LlmStructuredOutputSettings,
     LlmStructuredOutputType,
 )
@@ -105,15 +105,15 @@
         ):
             grammar = structured_output_settings.get_json_schema()
         top_p = settings.top_p
         stream = settings.stream
         temperature = settings.temperature
         max_tokens = settings.max_tokens
 
-        settings_dict = copy(settings.as_dict())
+        settings_dict = deepcopy(settings.as_dict())
         settings_dict.pop("top_p")
         settings_dict.pop("stream")
         settings_dict.pop("temperature")
         settings_dict.pop("max_tokens")
         if grammar is not None:
             settings_dict["guided_json"] = grammar
```

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/rag/rag_colbert_reranker.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/rag/rag_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/structured_output_agent.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/structured_output_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent/text_utils.py` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent/text_utils.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent.egg-info/PKG-INFO` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.2.2
+Version: 0.2.3
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,18 @@
 Provides-Extra: vllm-provider
 Requires-Dist: openai; extra == "vllm-provider"
 Provides-Extra: mixtral-agent
 Requires-Dist: mistral-common; extra == "mixtral-agent"
 
 # llama-cpp-agent
 
-<img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/db41b3184ebc902f50edbd3d27f7a3a1128b7d7d/logo/logo_orange.png" alt="llama-cpp-agent logo" width="400"/>
+[![PyPI - Version](https://img.shields.io/pypi/v/llama-cpp-agent?logo=pypi&color=%2341bb13)](https://pypi.org/project/llama-cpp-agent/)
+[![Discord](https://img.shields.io/discord/1237393014154985582?logo=Discord&logoColor=%23ffffff&label=Discord&link=https%3A%2F%2Fdiscord.gg%2FsRMvWKrh)](https://discord.gg/sRMvWKrh)
+
+<img src="./logo/logo_orange.png" alt="llama-cpp-agent logo" width="280"/>
 
 ## Introduction
 The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
 
 The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
 
 The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
@@ -133,41 +136,50 @@
 
 [View Example](https://llama-cpp-agent.readthedocs.io/en/latest/knowledge-graph-example/)
 
 
 ## Additional Information
 
 ### Predefined Messages Formatter
+
 The llama-cpp-agent framework provides predefined message formatters to format messages for the LLM model. The `MessagesFormatterType` enum defines the available formatters:
 
+- `MessagesFormatterType.MISTRAL`: Formats messages using the MISTRAL format.
 - `MessagesFormatterType.CHATML`: Formats messages using the CHATML format.
-- `MessagesFormatterType.MIXTRAL`: Formats messages using the MIXTRAL format.
 - `MessagesFormatterType.VICUNA`: Formats messages using the VICUNA format.
 - `MessagesFormatterType.LLAMA_2`: Formats messages using the LLAMA 2 format.
 - `MessagesFormatterType.SYNTHIA`: Formats messages using the SYNTHIA format.
 - `MessagesFormatterType.NEURAL_CHAT`: Formats messages using the NEURAL CHAT format.
 - `MessagesFormatterType.SOLAR`: Formats messages using the SOLAR format.
 - `MessagesFormatterType.OPEN_CHAT`: Formats messages using the OPEN CHAT format.
+- `MessagesFormatterType.ALPACA`: Formats messages using the ALPACA format.
+- `MessagesFormatterType.CODE_DS`: Formats messages using the CODE DS format.
+- `MessagesFormatterType.B22`: Formats messages using the B22 format.
+- `MessagesFormatterType.LLAMA_3`: Formats messages using the LLAMA 3 format.
+- `MessagesFormatterType.PHI_3`: Formats messages using the PHI 3 format.
 
 ### Creating Custom Messages Formatter
+
 You can create your own custom messages formatter by instantiating the `MessagesFormatter` class with the desired parameters:
 
 ```python
-from llama_cpp_agent.messages_formatter import MessagesFormatter
+from llama_cpp_agent.chat_history.messages_formatter import MessagesFormatter, PromptMarkers, Roles
+
+custom_prompt_markers = {
+    Roles.system: PromptMarkers("<|system|>", "<|endsystem|>"),
+    Roles.user: PromptMarkers("<|user|>", "<|enduser|>"),
+    Roles.assistant: PromptMarkers("<|assistant|>", "<|endassistant|>"),
+    Roles.tool: PromptMarkers("<|tool|>", "<|endtool|>"),
+}
 
 custom_formatter = MessagesFormatter(
-    PRE_PROMPT="",
-    SYS_PROMPT_START="<|system|>",
-    SYS_PROMPT_END="<|endsystem|>",
-    USER_PROMPT_START="<|user|>",
-    USER_PROMPT_END="<|enduser|>",
-    ASSISTANT_PROMPT_START="<|assistant|>",
-    ASSISTANT_PROMPT_END="<|endassistant|>",
-    INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE=False,
-    DEFAULT_STOP_SEQUENCES=["<|endsystem|>", "<|enduser|>", "<|endassistant|>"]
+    pre_prompt="",
+    prompt_markers=custom_prompt_markers,
+    include_sys_prompt_in_first_user_message=False,
+    default_stop_sequences=["<|endsystem|>", "<|enduser|>", "<|endassistant|>", "<|endtool|>"]
 )
 ```
 
 ## Contributing
 We welcome contributions to the llama-cpp-agent framework! If you'd like to contribute, please follow these guidelines:
 
 1. Fork the repository and create your branch from `master`.
```

### Comparing `llama_cpp_agent-0.2.2/src/llama_cpp_agent.egg-info/SOURCES.txt` & `llama_cpp_agent-0.2.3/src/llama_cpp_agent.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+README.md
 ReadMe.md
 pyproject.toml
 src/llama_cpp_agent/__init__.py
 src/llama_cpp_agent/chain.py
 src/llama_cpp_agent/function_calling.py
 src/llama_cpp_agent/function_calling_agent.py
 src/llama_cpp_agent/hermes_2_pro_agent.py
```

