# Comparing `tmp/assistant-1.1.1b2.tar.gz` & `tmp/assistant-1.1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assistant-1.1.1b2.tar", last modified: Sat Mar 30 00:17:07 2024, max compression
+gzip compressed data, was "assistant-1.1.2b1.tar", last modified: Tue May 14 13:41:36 2024, max compression
```

## Comparing `assistant-1.1.1b2.tar` & `assistant-1.1.2b1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.619705 assistant-1.1.1b2/
--rw-r--r--   0 waser     (1000) waser     (1000)     1069 2022-03-17 17:48:10.000000 assistant-1.1.1b2/LICENSE
--rw-r--r--   0 waser     (1000) waser     (1000)       16 2022-03-17 17:48:10.000000 assistant-1.1.1b2/MANIFEST.in
--rw-r--r--   0 waser     (1000) waser     (1000)    12713 2024-03-30 00:17:07.619705 assistant-1.1.1b2/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)    10843 2024-02-18 19:52:01.000000 assistant-1.1.1b2/README.md
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.606371 assistant-1.1.1b2/assistant/
--rw-r--r--   0 waser     (1000) waser     (1000)      502 2024-03-30 00:10:28.000000 assistant-1.1.1b2/assistant/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      114 2023-12-25 15:43:40.000000 assistant-1.1.1b2/assistant/__main__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     5674 2023-12-25 15:43:40.000000 assistant-1.1.1b2/assistant/_execer.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.609705 assistant-1.1.1b2/assistant/api/
--rw-r--r--   0 waser     (1000) waser     (1000)      317 2023-12-25 15:43:40.000000 assistant-1.1.1b2/assistant/api/responses.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3867 2023-12-25 15:43:40.000000 assistant-1.1.1b2/assistant/as_client.py
--rw-r--r--   0 waser     (1000) waser     (1000)     5408 2024-03-30 00:09:49.000000 assistant-1.1.1b2/assistant/as_service.py
--rw-r--r--   0 waser     (1000) waser     (1000)     6818 2024-01-25 22:35:30.000000 assistant-1.1.1b2/assistant/builtin_cmds.py
--rw-r--r--   0 waser     (1000) waser     (1000)     6792 2023-12-25 15:43:40.000000 assistant-1.1.1b2/assistant/codecache.py
--rw-r--r--   0 waser     (1000) waser     (1000)      132 2023-12-25 15:43:40.000000 assistant-1.1.1b2/assistant/conditions.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.609705 assistant-1.1.1b2/assistant/entry_points/
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:40.000000 assistant-1.1.1b2/assistant/entry_points/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      194 2023-12-25 15:43:40.000000 assistant-1.1.1b2/assistant/entry_points/run_assistant.py
--rw-r--r--   0 waser     (1000) waser     (1000)      157 2023-12-25 15:43:40.000000 assistant-1.1.1b2/assistant/execer.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3595 2023-12-25 15:43:40.000000 assistant-1.1.1b2/assistant/history.py
--rw-r--r--   0 waser     (1000) waser     (1000)      519 2023-12-25 15:43:40.000000 assistant-1.1.1b2/assistant/icons.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.609705 assistant-1.1.1b2/assistant/listen/
--rw-r--r--   0 waser     (1000) waser     (1000)      400 2023-12-25 20:08:57.000000 assistant-1.1.1b2/assistant/listen/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-12-25 15:43:40.000000 assistant-1.1.1b2/assistant/listen/__main__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1365 2023-12-27 14:05:03.000000 assistant-1.1.1b2/assistant/listen/interface.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2776 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/listen/main.py
--rw-r--r--   0 waser     (1000) waser     (1000)    24086 2024-01-13 19:40:59.000000 assistant-1.1.1b2/assistant/main.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.609705 assistant-1.1.1b2/assistant/manager/
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/manager/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2355 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/manager/__main__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     9813 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/manager/nlu.py
--rw-r--r--   0 waser     (1000) waser     (1000)    18387 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/manager/nlu_to_stt.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.609705 assistant-1.1.1b2/assistant/nlp/
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/__init__.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.613038 assistant-1.1.1b2/assistant/nlp/chains/
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      411 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/__main__.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.613038 assistant-1.1.1b2/assistant/nlp/chains/agents/
--rw-r--r--   0 waser     (1000) waser     (1000)      689 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/agents/__executor__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2374 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/agents/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3010 2024-01-14 06:03:19.000000 assistant-1.1.1b2/assistant/nlp/chains/agents/assistant.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.613038 assistant-1.1.1b2/assistant/nlp/chains/callback_handlers/
--rw-r--r--   0 waser     (1000) waser     (1000)     2074 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/callback_handlers/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3155 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/code_pilot.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.613038 assistant-1.1.1b2/assistant/nlp/chains/data_loaders/
--rw-r--r--   0 waser     (1000) waser     (1000)      158 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/data_loaders/__init__.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.613038 assistant-1.1.1b2/assistant/nlp/chains/data_splitter/
--rw-r--r--   0 waser     (1000) waser     (1000)       76 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/data_splitter/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2918 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/docs_explained.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.613038 assistant-1.1.1b2/assistant/nlp/chains/embeddings/
--rw-r--r--   0 waser     (1000) waser     (1000)      184 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/embeddings/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     4647 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/embeddings/assistant.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.613038 assistant-1.1.1b2/assistant/nlp/chains/memory/
--rw-r--r--   0 waser     (1000) waser     (1000)      203 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/memory/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      536 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/memory/conversation_buffer.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.613038 assistant-1.1.1b2/assistant/nlp/chains/models/
--rw-r--r--   0 waser     (1000) waser     (1000)      952 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/models/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      682 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/models/hf.py
--rw-r--r--   0 waser     (1000) waser     (1000)     6568 2024-02-22 21:10:49.000000 assistant-1.1.1b2/assistant/nlp/chains/models/vllm.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.613038 assistant-1.1.1b2/assistant/nlp/chains/parsers/
--rw-r--r--   0 waser     (1000) waser     (1000)      156 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/parsers/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1833 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/parsers/column_csv.py
--rw-r--r--   0 waser     (1000) waser     (1000)     7466 2024-01-18 15:46:46.000000 assistant-1.1.1b2/assistant/nlp/chains/parsers/json.py
--rw-r--r--   0 waser     (1000) waser     (1000)     4783 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/parsers/markdown_json.py
--rw-r--r--   0 waser     (1000) waser     (1000)      831 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/persistent_session.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.616372 assistant-1.1.1b2/assistant/nlp/chains/prompts/
--rw-r--r--   0 waser     (1000) waser     (1000)     5222 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/prompts/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      690 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/prompts/airoboros.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1512 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/prompts/json.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.616372 assistant-1.1.1b2/assistant/nlp/chains/schema/
--rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/schema/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2211 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/schema/memory.py
--rw-r--r--   0 waser     (1000) waser     (1000)     5260 2024-01-13 19:44:59.000000 assistant-1.1.1b2/assistant/nlp/chains/schema/vectorstore.py
--rw-r--r--   0 waser     (1000) waser     (1000)     5298 2024-01-20 18:39:31.000000 assistant-1.1.1b2/assistant/nlp/chains/session.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.616372 assistant-1.1.1b2/assistant/nlp/chains/tools/
--rw-r--r--   0 waser     (1000) waser     (1000)      406 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/tools/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1698 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/tools/__retriever__.py
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/tools/memory.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2021 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/tools/python.py
--rw-r--r--   0 waser     (1000) waser     (1000)      300 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/chains/tools/retriever.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1505 2024-01-13 19:49:07.000000 assistant-1.1.1b2/assistant/nlp/chains/tools/search.py
--rw-r--r--   0 waser     (1000) waser     (1000)     5049 2024-01-05 02:36:06.000000 assistant-1.1.1b2/assistant/nlp/chains/tools/shell.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1762 2024-01-13 19:49:32.000000 assistant-1.1.1b2/assistant/nlp/chains/tools/wikipedia.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.616372 assistant-1.1.1b2/assistant/nlp/chains/vectorstores/
--rw-r--r--   0 waser     (1000) waser     (1000)     2207 2024-01-13 19:43:16.000000 assistant-1.1.1b2/assistant/nlp/chains/vectorstores/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      261 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/clear.py
--rw-r--r--   0 waser     (1000) waser     (1000)      193 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/exit.py
--rw-r--r--   0 waser     (1000) waser     (1000)     4537 2023-12-28 09:09:16.000000 assistant-1.1.1b2/assistant/nlp/interface.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1051 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/nlp/think.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2039 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/parser.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.616372 assistant-1.1.1b2/assistant/procs/
--rw-r--r--   0 waser     (1000) waser     (1000)      696 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/procs/pipelines.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2545 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/procs/specs.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.619705 assistant-1.1.1b2/assistant/ptk_shell/
--rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/ptk_shell/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      877 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/ptk_shell/bindings.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3552 2024-01-20 18:30:42.000000 assistant-1.1.1b2/assistant/ptk_shell/completer.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2913 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/ptk_shell/dialogs.py
--rw-r--r--   0 waser     (1000) waser     (1000)      254 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/ptk_shell/floats.py
--rw-r--r--   0 waser     (1000) waser     (1000)      152 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/ptk_shell/layout.py
--rw-r--r--   0 waser     (1000) waser     (1000)    17322 2024-01-25 22:39:37.000000 assistant-1.1.1b2/assistant/ptk_shell/shell.py
--rw-r--r--   0 waser     (1000) waser     (1000)     5333 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/ptk_shell/strformat_utils.py
--rw-r--r--   0 waser     (1000) waser     (1000)      696 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/ptk_shell/styles.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2955 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/ptk_shell/windows.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.619705 assistant-1.1.1b2/assistant/say/
--rw-r--r--   0 waser     (1000) waser     (1000)     3123 2023-12-27 16:13:02.000000 assistant-1.1.1b2/assistant/say/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      448 2023-12-27 16:17:18.000000 assistant-1.1.1b2/assistant/say/interface.py
--rw-r--r--   0 waser     (1000) waser     (1000)       71 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/time.py
--rw-r--r--   0 waser     (1000) waser     (1000)      887 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/utils.py
--rw-r--r--   0 waser     (1000) waser     (1000)      641 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/version.py
--rw-r--r--   0 waser     (1000) waser     (1000)      537 2023-12-25 15:43:41.000000 assistant-1.1.1b2/assistant/vocabulary.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.619705 assistant-1.1.1b2/assistant.egg-info/
--rw-r--r--   0 waser     (1000) waser     (1000)    12713 2024-03-30 00:17:07.000000 assistant-1.1.1b2/assistant.egg-info/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)     3085 2024-03-30 00:17:07.000000 assistant-1.1.1b2/assistant.egg-info/SOURCES.txt
--rw-r--r--   0 waser     (1000) waser     (1000)        1 2024-03-30 00:17:07.000000 assistant-1.1.1b2/assistant.egg-info/dependency_links.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       71 2024-03-30 00:17:07.000000 assistant-1.1.1b2/assistant.egg-info/entry_points.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      280 2024-03-30 00:17:07.000000 assistant-1.1.1b2/assistant.egg-info/requires.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       18 2024-03-30 00:17:07.000000 assistant-1.1.1b2/assistant.egg-info/top_level.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      888 2022-10-06 02:51:22.000000 assistant-1.1.1b2/pyproject.toml
--rw-r--r--   0 waser     (1000) waser     (1000)     3674 2024-03-30 00:17:07.619705 assistant-1.1.1b2/setup.cfg
--rw-r--r--   0 waser     (1000) waser     (1000)     3533 2024-01-13 19:51:17.000000 assistant-1.1.1b2/setup.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.619705 assistant-1.1.1b2/tests/
--rw-r--r--   0 waser     (1000) waser     (1000)     5083 2023-11-30 06:13:11.000000 assistant-1.1.1b2/tests/test_execer.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-03-30 00:17:07.619705 assistant-1.1.1b2/xontrib/
--rw-r--r--   0 waser     (1000) waser     (1000)     2241 2023-11-30 06:13:11.000000 assistant-1.1.1b2/xontrib/assistant.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.252899 assistant-1.1.2b1/
+-rw-r--r--   0 waser     (1000) waser     (1000)     1069 2022-03-17 17:48:10.000000 assistant-1.1.2b1/LICENSE
+-rw-r--r--   0 waser     (1000) waser     (1000)       16 2022-03-17 17:48:10.000000 assistant-1.1.2b1/MANIFEST.in
+-rw-r--r--   0 waser     (1000) waser     (1000)    12722 2024-05-14 13:41:36.252899 assistant-1.1.2b1/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)    10843 2024-02-18 19:52:01.000000 assistant-1.1.2b1/README.md
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.239566 assistant-1.1.2b1/assistant/
+-rw-r--r--   0 waser     (1000) waser     (1000)      502 2024-05-14 13:38:34.000000 assistant-1.1.2b1/assistant/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      114 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/__main__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     5674 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/_execer.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.239566 assistant-1.1.2b1/assistant/api/
+-rw-r--r--   0 waser     (1000) waser     (1000)      317 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/api/responses.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3867 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/as_client.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     5428 2024-05-08 08:18:22.000000 assistant-1.1.2b1/assistant/as_service.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     6818 2024-01-25 22:35:30.000000 assistant-1.1.2b1/assistant/builtin_cmds.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     6792 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/codecache.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      132 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/conditions.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.239566 assistant-1.1.2b1/assistant/entry_points/
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/entry_points/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      194 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/entry_points/run_assistant.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      157 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/execer.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3595 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/history.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      519 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/icons.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.242900 assistant-1.1.2b1/assistant/listen/
+-rw-r--r--   0 waser     (1000) waser     (1000)      400 2023-12-25 20:08:57.000000 assistant-1.1.2b1/assistant/listen/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-12-25 15:43:40.000000 assistant-1.1.2b1/assistant/listen/__main__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1396 2024-05-13 22:55:29.000000 assistant-1.1.2b1/assistant/listen/interface.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2776 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/listen/main.py
+-rw-r--r--   0 waser     (1000) waser     (1000)    24086 2024-05-13 19:44:02.000000 assistant-1.1.2b1/assistant/main.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.242900 assistant-1.1.2b1/assistant/manager/
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/manager/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2355 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/manager/__main__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     9813 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/manager/nlu.py
+-rw-r--r--   0 waser     (1000) waser     (1000)    18387 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/manager/nlu_to_stt.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.242900 assistant-1.1.2b1/assistant/nlp/
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/__init__.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.242900 assistant-1.1.2b1/assistant/nlp/chains/
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      411 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/__main__.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/agents/
+-rw-r--r--   0 waser     (1000) waser     (1000)      689 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/agents/__executor__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2374 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/agents/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3010 2024-05-08 06:30:31.000000 assistant-1.1.2b1/assistant/nlp/chains/agents/assistant.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/callback_handlers/
+-rw-r--r--   0 waser     (1000) waser     (1000)     2074 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/callback_handlers/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3155 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/code_pilot.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/data_loaders/
+-rw-r--r--   0 waser     (1000) waser     (1000)      158 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/data_loaders/__init__.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/data_splitter/
+-rw-r--r--   0 waser     (1000) waser     (1000)       76 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/data_splitter/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2918 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/docs_explained.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/embeddings/
+-rw-r--r--   0 waser     (1000) waser     (1000)      184 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/embeddings/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     4647 2024-05-13 19:11:24.000000 assistant-1.1.2b1/assistant/nlp/chains/embeddings/assistant.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/memory/
+-rw-r--r--   0 waser     (1000) waser     (1000)      203 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/memory/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      536 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/memory/conversation_buffer.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/models/
+-rw-r--r--   0 waser     (1000) waser     (1000)      952 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/models/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      682 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/models/hf.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     6568 2024-02-22 21:10:49.000000 assistant-1.1.2b1/assistant/nlp/chains/models/vllm.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.246233 assistant-1.1.2b1/assistant/nlp/chains/parsers/
+-rw-r--r--   0 waser     (1000) waser     (1000)      156 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/parsers/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1833 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/parsers/column_csv.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     7620 2024-05-11 15:39:14.000000 assistant-1.1.2b1/assistant/nlp/chains/parsers/json.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     4783 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/parsers/markdown_json.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      831 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/persistent_session.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.249566 assistant-1.1.2b1/assistant/nlp/chains/prompts/
+-rw-r--r--   0 waser     (1000) waser     (1000)     5222 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/prompts/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      690 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/prompts/airoboros.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1509 2024-05-08 06:27:54.000000 assistant-1.1.2b1/assistant/nlp/chains/prompts/json.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.249566 assistant-1.1.2b1/assistant/nlp/chains/schema/
+-rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/schema/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2209 2024-05-08 06:48:37.000000 assistant-1.1.2b1/assistant/nlp/chains/schema/memory.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     5260 2024-01-13 19:44:59.000000 assistant-1.1.2b1/assistant/nlp/chains/schema/vectorstore.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     5443 2024-05-11 15:35:21.000000 assistant-1.1.2b1/assistant/nlp/chains/session.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.249566 assistant-1.1.2b1/assistant/nlp/chains/tools/
+-rw-r--r--   0 waser     (1000) waser     (1000)      406 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1698 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/__retriever__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/memory.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2021 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/python.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      300 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/retriever.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1505 2024-01-13 19:49:07.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/search.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     5049 2024-01-05 02:36:06.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/shell.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1762 2024-01-13 19:49:32.000000 assistant-1.1.2b1/assistant/nlp/chains/tools/wikipedia.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.249566 assistant-1.1.2b1/assistant/nlp/chains/vectorstores/
+-rw-r--r--   0 waser     (1000) waser     (1000)     2207 2024-01-13 19:43:16.000000 assistant-1.1.2b1/assistant/nlp/chains/vectorstores/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      261 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/clear.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      193 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/exit.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     4537 2023-12-28 09:09:16.000000 assistant-1.1.2b1/assistant/nlp/interface.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1051 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/nlp/think.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2039 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/parser.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.249566 assistant-1.1.2b1/assistant/procs/
+-rw-r--r--   0 waser     (1000) waser     (1000)      696 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/procs/pipelines.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2545 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/procs/specs.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.252899 assistant-1.1.2b1/assistant/ptk_shell/
+-rw-r--r--   0 waser     (1000) waser     (1000)        0 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      877 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/bindings.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3552 2024-05-08 06:48:57.000000 assistant-1.1.2b1/assistant/ptk_shell/completer.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2913 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/dialogs.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      254 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/floats.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      152 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/layout.py
+-rw-r--r--   0 waser     (1000) waser     (1000)    17322 2024-01-25 22:39:37.000000 assistant-1.1.2b1/assistant/ptk_shell/shell.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     5333 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/strformat_utils.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      696 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/styles.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2955 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/ptk_shell/windows.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.252899 assistant-1.1.2b1/assistant/say/
+-rw-r--r--   0 waser     (1000) waser     (1000)     3901 2024-05-13 19:10:08.000000 assistant-1.1.2b1/assistant/say/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      448 2023-12-27 16:17:18.000000 assistant-1.1.2b1/assistant/say/interface.py
+-rw-r--r--   0 waser     (1000) waser     (1000)       71 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/time.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      887 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/utils.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      641 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/version.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      537 2023-12-25 15:43:41.000000 assistant-1.1.2b1/assistant/vocabulary.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.252899 assistant-1.1.2b1/assistant.egg-info/
+-rw-r--r--   0 waser     (1000) waser     (1000)    12722 2024-05-14 13:41:36.000000 assistant-1.1.2b1/assistant.egg-info/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)     3085 2024-05-14 13:41:36.000000 assistant-1.1.2b1/assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)        1 2024-05-14 13:41:36.000000 assistant-1.1.2b1/assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       71 2024-05-14 13:41:36.000000 assistant-1.1.2b1/assistant.egg-info/entry_points.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      289 2024-05-14 13:41:36.000000 assistant-1.1.2b1/assistant.egg-info/requires.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       18 2024-05-14 13:41:36.000000 assistant-1.1.2b1/assistant.egg-info/top_level.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      888 2022-10-06 02:51:22.000000 assistant-1.1.2b1/pyproject.toml
+-rw-r--r--   0 waser     (1000) waser     (1000)     3674 2024-05-14 13:41:36.256232 assistant-1.1.2b1/setup.cfg
+-rw-r--r--   0 waser     (1000) waser     (1000)     3542 2024-05-13 20:21:47.000000 assistant-1.1.2b1/setup.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.252899 assistant-1.1.2b1/tests/
+-rw-r--r--   0 waser     (1000) waser     (1000)     5083 2023-11-30 06:13:11.000000 assistant-1.1.2b1/tests/test_execer.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2024-05-14 13:41:36.252899 assistant-1.1.2b1/xontrib/
+-rw-r--r--   0 waser     (1000) waser     (1000)     2241 2023-11-30 06:13:11.000000 assistant-1.1.2b1/xontrib/assistant.py
```

### Comparing `assistant-1.1.1b2/LICENSE` & `assistant-1.1.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/PKG-INFO` & `assistant-1.1.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant
-Version: 1.1.1b2
+Version: 1.1.2b1
 Summary: Your very own Assistant. Because you deserve it.
 Home-page: https://gitlab.com/waser-technologies/technologies/assistant
 Author: Danny Waser
 Author-email: danny@waser.tech
 License: MIT
 Project-URL: Documentation, https://gitlab.com/waser-technologies/technologies/assistant/blob/master/README.md
 Project-URL: Code, https://gitlab.com/waser-technologies/technologies/assistant
@@ -41,15 +41,15 @@
 Requires-Dist: einops
 Requires-Dist: langchain
 Requires-Dist: langchain-community
 Requires-Dist: websockets
 Requires-Dist: colorama
 Requires-Dist: rich
 Requires-Dist: halo
-Requires-Dist: duckduckgo-search
+Requires-Dist: duckduckgo_search==5.3.1b1
 Requires-Dist: wikipedia
 Requires-Dist: pexpect
 Requires-Dist: scipy
 Requires-Dist: chromadb
 Requires-Dist: pydantic<2.0
 Requires-Dist: fsspec>=2023.10.0
```

### Comparing `assistant-1.1.1b2/README.md` & `assistant-1.1.2b1/README.md`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/_execer.py` & `assistant-1.1.2b1/assistant/_execer.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/as_client.py` & `assistant-1.1.2b1/assistant/as_client.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/as_service.py` & `assistant-1.1.2b1/assistant/as_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,16 @@
         if gpu_count > 2:
             gpu_memory = get_gpu_info()
             if not gpu_memory:
                 return None
             max_mem_id = ",".join(range(gpu_count - 1, 0))
             return max_mem_id
         elif gpu_count == 2:
-            return str(0) #str(1)
+            # return str(0)
+            return str(1)
         else:
             return str(gpu_count - 1)
 
     gpu_id = get_gpu_id()
 
     assert gpu_id, f"No CUDA GPUs available! ({gpu_id=})"
```

### Comparing `assistant-1.1.1b2/assistant/builtin_cmds.py` & `assistant-1.1.2b1/assistant/builtin_cmds.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/codecache.py` & `assistant-1.1.2b1/assistant/codecache.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/history.py` & `assistant-1.1.2b1/assistant/history.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/icons.py` & `assistant-1.1.2b1/assistant/icons.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/listen/interface.py` & `assistant-1.1.2b1/assistant/listen/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,11 +36,12 @@
             return False
 
     def listen(self):
         source = mic.Microphone()
         source.record()
         query = source.transcribe_until_silence()
         source.stop_record()
+        # source.stop_stream()
         # source.destroy()
-        source.vad_audio.destroy()
         source.vad_audio.pa.terminate()
+        source.vad_audio.destroy()
         return query
```

### Comparing `assistant-1.1.1b2/assistant/listen/main.py` & `assistant-1.1.2b1/assistant/listen/main.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/main.py` & `assistant-1.1.2b1/assistant/main.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/manager/__main__.py` & `assistant-1.1.2b1/assistant/manager/__main__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/manager/nlu.py` & `assistant-1.1.2b1/assistant/manager/nlu.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/manager/nlu_to_stt.py` & `assistant-1.1.2b1/assistant/manager/nlu_to_stt.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/agents/__executor__.py` & `assistant-1.1.2b1/assistant/nlp/chains/agents/__executor__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/agents/__init__.py` & `assistant-1.1.2b1/assistant/nlp/chains/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/agents/assistant.py` & `assistant-1.1.2b1/assistant/nlp/chains/agents/assistant.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/callback_handlers/__init__.py` & `assistant-1.1.2b1/assistant/nlp/chains/callback_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/code_pilot.py` & `assistant-1.1.2b1/assistant/nlp/chains/code_pilot.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/docs_explained.py` & `assistant-1.1.2b1/assistant/nlp/chains/docs_explained.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/embeddings/assistant.py` & `assistant-1.1.2b1/assistant/nlp/chains/embeddings/assistant.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/memory/conversation_buffer.py` & `assistant-1.1.2b1/assistant/nlp/chains/memory/conversation_buffer.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/models/__init__.py` & `assistant-1.1.2b1/assistant/nlp/chains/models/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/models/hf.py` & `assistant-1.1.2b1/assistant/nlp/chains/models/hf.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/models/vllm.py` & `assistant-1.1.2b1/assistant/nlp/chains/models/vllm.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/parsers/column_csv.py` & `assistant-1.1.2b1/assistant/nlp/chains/parsers/column_csv.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/parsers/json.py` & `assistant-1.1.2b1/assistant/nlp/chains/parsers/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,32 +95,34 @@
                     f"JSONDecodeError: Could not parse output: {str(jsde)}\nLLM Response: {_text}",
                 )
 
     def handle_model_specifics(self, model_output: str) -> str:
         """
         Remove special tokens from the given output and perform any necessary pre-processing steps.
         """
-        model_output = model_output.split("<|im_stop|>")[0]
+        model_output = model_output.replace("\n}\n}\n\n", "\n}\n}<|im_end|>\n\n")
+        model_output = model_output.split("<|im_end|>")[0]
+        model_output = model_output.split("<|im_start|>")[0]
         # model_output = model_output.split("<s>[INST]")[0]
         # model_output = model_output.split("</s>")[0]
         # model_output = model_output.replace(
         #     "```\n\n```", "```</s> | <s>[INST] This hallucination will be discarded [/INST] ```"
         #     ).split(" | ")[0].removesuffix('<s>')
         # model_output = model_output.split("[/INST]")[0].strip()
         # model_output = model_output.split("[INST]")[0].strip()
         # text = text.replace("""</s>""", "")
         # text = text.replace("\n", '')
         # text = text.replace("\t", '')
         # text = text.replace("\r", '')
         # text = text.replace(" ", '')
         # text = text.replace("```json", '')
-        # text = text.replace("```", '')
+        model_output = model_output.replace("```", '')
         # model_output = model_output.strip("\n")
-        while model_output.endswith("<|im_stop|>"):
-            model_output = model_output.removesuffix("<|im_stop|>")
+        while model_output.endswith("<|im_end|>"):
+            model_output = model_output.removesuffix("<|im_end|>")
         return model_output
 
     @property
     def _type(self) -> str:
         return "conversational_chat"
```

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/parsers/markdown_json.py` & `assistant-1.1.2b1/assistant/nlp/chains/parsers/markdown_json.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/persistent_session.py` & `assistant-1.1.2b1/assistant/nlp/chains/persistent_session.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/prompts/__init__.py` & `assistant-1.1.2b1/assistant/nlp/chains/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/prompts/airoboros.py` & `assistant-1.1.2b1/assistant/nlp/chains/prompts/airoboros.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/prompts/json.py` & `assistant-1.1.2b1/assistant/nlp/chains/prompts/json.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from assistant.nlp.chains.prompts.airoboros import JSON_FUNC
 
-BOS, EOS = "<|im_start|>assistant\n", "<|im_stop|>\n"
-BOSYS, EOSYS = "<|im_start|>system\n", "<|im_stop|>\n"
-BOI, EOI = "<|im_start|>user\n", "<|im_stop|>\n"
+BOS, EOS = "<|im_start|>assistant\n", "<|im_end|>\n"
+BOSYS, EOSYS = "<|im_start|>system\n", "<|im_end|>\n"
+BOI, EOI = "<|im_start|>user\n", "<|im_end|>\n"
 
 system_prompt = """You are Assistant, a sentient artificial intelligence.
 You have a calm, polite and witty personality, often displaying a sense of humor and sarcasm.
 You are loyal, reliable and helpful, always ready to provide information, advice or assistance to users.
 
 I am the User and you are my Assistant. Be respectful when addressing me.
```

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/schema/memory.py` & `assistant-1.1.2b1/assistant/nlp/chains/schema/memory.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,17 +40,17 @@
         elif isinstance(m, FunctionMessage):
             role = "Function"
         elif isinstance(m, ChatMessage):
             role = m.role
         else:
             raise ValueError(f"Got unsupported message type: {m}")
         if role == human_prefix:
-            user_message = f"<|im_start|>user\n{m.content}<|im_stop|>"
+            user_message = f"<|im_start|>user\n{m.content}<|im_end|>"
         elif role == ai_prefix:
-            assistant_message = f"<|im_start|>assistant\n{m.content}<|im_stop|>"
+            assistant_message = f"<|im_start|>assistant\n{m.content}<|im_end|>"
         #message = f"{role}: {m.content}"
         # if isinstance(m, AIMessage) and "function_call" in m.additional_kwargs:
         #     message += f"{m.additional_kwargs['function_call']}"
         if user_message and assistant_message:
             string_messages.append(f"{user_message}\n{assistant_message}")
             user_message = None
             assistant_message = None
```

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/schema/vectorstore.py` & `assistant-1.1.2b1/assistant/nlp/chains/schema/vectorstore.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/session.py` & `assistant-1.1.2b1/assistant/nlp/chains/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self.tools = get_all_tools()
 
     def _initialize_agent(self, max_iterations=20):
         tool_names = [tool.name for tool in self.tools]
         self.agent = AssistantSingleActionAgent(
             llm_chain=self.llm_chain,
             output_parser=self.output_parser,
-            stop=["<|im_stop|>", "<|im_start|>", "<|im_end|>", "<|endoftext|>", """<|im_stop|>"""],
+            stop=["<|im_end|>\n", "<|im_stop|>", "<|im_start|>", "<|im_end|>", "<|endoftext|>", """<|im_stop|>\n""", "\n}\n}\n\n"],
             allowed_tools=tool_names
         )
         self.agent_executor = AgentExecutor.from_agent_and_tools(agent=self.agent, tools=self.tools, verbose=self.verbose, max_iterations=max_iterations, memory=self.memory)
 
     def __call__(self, message: str):
         output = self.agent_executor.invoke({'input': message})
         return self.process_output(output['output'])
@@ -105,14 +105,18 @@
         # output = output.replace("```\n\n```", "```</s> | <s>[INST] This hallucination will be discarded [/INST] ```").split(" | ")[0].removesuffix('<s>')
         # output = output.split("[/INST]")[0]
         # output = output.split("<|im_stop|>")[0]
         # dirty hack remove once model is ready
         # output = output.replace("Use the following input to take an action:", "")
         # Add other pre-processing steps here
         #return output.strip("\n")
+        output = output.replace("""}
+}""", """}
+}<|im_stop|>""")
+        output = output.split("<|im_stop|>")[0]
         return output
     
     def __str__(self):
         return f"{self.name}: {self.max_tokens} tokens @{self.temperature}°"
     
     def export_conversation(self):
         """
```

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/tools/__retriever__.py` & `assistant-1.1.2b1/assistant/nlp/chains/tools/__retriever__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/tools/python.py` & `assistant-1.1.2b1/assistant/nlp/chains/tools/python.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/tools/search.py` & `assistant-1.1.2b1/assistant/nlp/chains/tools/search.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/tools/shell.py` & `assistant-1.1.2b1/assistant/nlp/chains/tools/shell.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/tools/wikipedia.py` & `assistant-1.1.2b1/assistant/nlp/chains/tools/wikipedia.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/chains/vectorstores/__init__.py` & `assistant-1.1.2b1/assistant/nlp/chains/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/interface.py` & `assistant-1.1.2b1/assistant/nlp/interface.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/nlp/think.py` & `assistant-1.1.2b1/assistant/nlp/think.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/parser.py` & `assistant-1.1.2b1/assistant/parser.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/procs/pipelines.py` & `assistant-1.1.2b1/assistant/procs/pipelines.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/procs/specs.py` & `assistant-1.1.2b1/assistant/procs/specs.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/ptk_shell/bindings.py` & `assistant-1.1.2b1/assistant/ptk_shell/bindings.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/ptk_shell/completer.py` & `assistant-1.1.2b1/assistant/ptk_shell/completer.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self,
         query,
         host="localhost",
         port="5085",
         n: int = 5,
         max_tokens: int = 3,
         stream: bool = False,
-        stop: List[str] | None = ["<|im_stop|>", "<|im_start|>", "<|im_end|>", "<|endoftext|>"],
+        stop: List[str] | None = ["<|im_end|>", "<|im_stop|>", "<|im_start|>", "<|endoftext|>"],
     ):
         try:
             headers = {"User-Agent": "completer"}
             payload = {
                 "prompt": query,
                 "use_beam_search": True,
                 "n": n,
```

### Comparing `assistant-1.1.1b2/assistant/ptk_shell/dialogs.py` & `assistant-1.1.2b1/assistant/ptk_shell/dialogs.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/ptk_shell/shell.py` & `assistant-1.1.2b1/assistant/ptk_shell/shell.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/ptk_shell/strformat_utils.py` & `assistant-1.1.2b1/assistant/ptk_shell/strformat_utils.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/ptk_shell/styles.py` & `assistant-1.1.2b1/assistant/ptk_shell/styles.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/ptk_shell/windows.py` & `assistant-1.1.2b1/assistant/ptk_shell/windows.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/say/__init__.py` & `assistant-1.1.2b1/assistant/say/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -39,23 +39,40 @@
 
     @property
     def is_allowed_to_speak(self):
         if self.config is None:
             self.config = tts_utils.get_config_or_default()
         return tts_utils.is_allowed_to_speak(self.config)
 
+    def split_sentences(self, text: str, split_char="|"):
+        text = text.strip("\n")
+        text = text.replace(",", f",{split_char}")
+        text = text.replace(".", f".{split_char}")
+        text = text.replace("!", f"!{split_char}")
+        text = text.replace("?", f"?{split_char}")
+        text = text.replace(":", f":{split_char}")
+        text = text.replace(";", f";{split_char}")
+        text = text.replace("\n", f"{split_char}")
+        return text.split(split_char)
+    
     def say(self, text: list[str] | str):
         if isinstance(text, str):
-            text = text.split("\n")
+            text = text.split("\n")            
         if not self.is_allowed_to_speak:
-            print(f"{' '.join(text)}")
+            print('\n'.join(text))
             return
-        asyncio.run(tts(text, language="fr-fr" if I18N == "fr" else I18N.lower(), style_wav=f"{self.config['tts']['speaker_wav']}", save_output=False))
+        try:
+            for t in text:
+                asyncio.run(tts(self.split_sentences(t), language="fr-fr" if I18N == "fr" else I18N.lower(), style_wav=f"{self.config['tts']['speaker_wav']}", save_output=False))
+            # asyncio.run(tts(text, language="fr-fr" if I18N == "fr" else I18N.lower(), voice_name="freeman", preset='fast', save_output=False))
         # asyncio.run(self.asay(text))
         # asyncio.run(self.apronounce())
+        except Exception:
+            # print(e)
+            return
     
     def pronounce(self):
         asyncio.run(self.apronounce())
 
     async def apronounce(self):
         while True:
             wav = await self.queue.get()
```

### Comparing `assistant-1.1.1b2/assistant/utils.py` & `assistant-1.1.2b1/assistant/utils.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/version.py` & `assistant-1.1.2b1/assistant/version.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant/vocabulary.py` & `assistant-1.1.2b1/assistant/vocabulary.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/assistant.egg-info/PKG-INFO` & `assistant-1.1.2b1/assistant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant
-Version: 1.1.1b2
+Version: 1.1.2b1
 Summary: Your very own Assistant. Because you deserve it.
 Home-page: https://gitlab.com/waser-technologies/technologies/assistant
 Author: Danny Waser
 Author-email: danny@waser.tech
 License: MIT
 Project-URL: Documentation, https://gitlab.com/waser-technologies/technologies/assistant/blob/master/README.md
 Project-URL: Code, https://gitlab.com/waser-technologies/technologies/assistant
@@ -41,15 +41,15 @@
 Requires-Dist: einops
 Requires-Dist: langchain
 Requires-Dist: langchain-community
 Requires-Dist: websockets
 Requires-Dist: colorama
 Requires-Dist: rich
 Requires-Dist: halo
-Requires-Dist: duckduckgo-search
+Requires-Dist: duckduckgo_search==5.3.1b1
 Requires-Dist: wikipedia
 Requires-Dist: pexpect
 Requires-Dist: scipy
 Requires-Dist: chromadb
 Requires-Dist: pydantic<2.0
 Requires-Dist: fsspec>=2023.10.0
```

### Comparing `assistant-1.1.1b2/assistant.egg-info/SOURCES.txt` & `assistant-1.1.2b1/assistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/pyproject.toml` & `assistant-1.1.2b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/setup.cfg` & `assistant-1.1.2b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/setup.py` & `assistant-1.1.2b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         'langchain',
         'langchain-community',
         # 'sanic',
         'websockets',
         'colorama',
         'rich',
         'halo',
-        'duckduckgo-search',
+        'duckduckgo_search==5.3.1b1',
         'wikipedia',
         'pexpect',
         'scipy',
         'chromadb',
         'pydantic<2.0', # https://github.com/huggingface/huggingface_hub/pull/1837#issuecomment-1827440687
         'fsspec>=2023.10.0', # See https://github.com/huggingface/huggingface_hub/issues/1872
     ]
```

### Comparing `assistant-1.1.1b2/tests/test_execer.py` & `assistant-1.1.2b1/tests/test_execer.py`

 * *Files identical despite different names*

### Comparing `assistant-1.1.1b2/xontrib/assistant.py` & `assistant-1.1.2b1/xontrib/assistant.py`

 * *Files identical despite different names*

