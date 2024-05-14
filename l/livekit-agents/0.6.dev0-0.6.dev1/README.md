# Comparing `tmp/livekit_agents-0.6.dev0.tar.gz` & `tmp/livekit_agents-0.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_agents-0.6.dev0.tar", last modified: Wed May  1 00:22:19 2024, max compression
+gzip compressed data, was "livekit_agents-0.6.dev1.tar", last modified: Wed May  1 00:52:12 2024, max compression
```

## Comparing `livekit_agents-0.6.dev0.tar` & `livekit_agents-0.6.dev1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.621821 livekit_agents-0.6.dev0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.625821 livekit_agents-0.6.dev0/livekit/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.629821 livekit_agents-0.6.dev0/livekit/agents/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/sleep.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/wait_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/apipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.629821 livekit_agents-0.6.dev0/livekit/agents/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/cli/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/cli/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/cli/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.629821 livekit_agents-0.6.dev0/livekit/agents/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/codecs/mp3.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/http_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.629821 livekit_agents-0.6.dev0/livekit/agents/ipc/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/ipc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/ipc/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/ipc/job_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/ipc/job_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/ipc/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/ipc_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/job_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/job_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.629821 livekit_agents-0.6.dev0/livekit/agents/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/llm/function_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/llm/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.629821 livekit_agents-0.6.dev0/livekit/agents/stt/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/stt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/stt/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/stt/stt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/livekit/agents/tokenize/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/tokenize/sentence_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/livekit/agents/tts/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/tts/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/tts/tts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/livekit/agents/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/utils/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/utils/exp_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/utils/moving_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/vad.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/livekit/agents/voice_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/voice_assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30779 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/voice_assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/voice_assistant/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16319 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/livekit_agents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-01 00:22:19.000000 livekit_agents-0.6.dev0/livekit_agents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-01 00:22:19.000000 livekit_agents-0.6.dev0/livekit_agents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:22:19.000000 livekit_agents-0.6.dev0/livekit_agents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-01 00:22:19.000000 livekit_agents-0.6.dev0/livekit_agents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:22:19.000000 livekit_agents-0.6.dev0/livekit_agents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.590407 livekit_agents-0.6.dev1/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.594407 livekit_agents-0.6.dev1/livekit/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/wait_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/apipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/cli/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/cli/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/cli/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/codecs/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/http_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/ipc/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/ipc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/ipc/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/ipc/job_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/ipc/job_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/ipc/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/ipc_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/job_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/job_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/llm/function_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/llm/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/stt/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/stt/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/stt/stt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/tokenize/sentence_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/livekit/agents/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/tts/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/tts/tts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/livekit/agents/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/utils/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/utils/exp_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/utils/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/livekit/agents/voice_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/voice_assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30755 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/voice_assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/voice_assistant/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16319 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/livekit_agents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-01 00:52:12.000000 livekit_agents-0.6.dev1/livekit_agents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-01 00:52:12.000000 livekit_agents-0.6.dev1/livekit_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:52:12.000000 livekit_agents-0.6.dev1/livekit_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-01 00:52:12.000000 livekit_agents-0.6.dev1/livekit_agents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:52:12.000000 livekit_agents-0.6.dev1/livekit_agents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/setup.py
```

### Comparing `livekit_agents-0.6.dev0/PKG-INFO` & `livekit_agents-0.6.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.6.dev0
+Version: 0.6.dev1
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
```

### Comparing `livekit_agents-0.6.dev0/livekit/agents/__init__.py` & `livekit_agents-0.6.dev1/livekit/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/aio/channel.py` & `livekit_agents-0.6.dev1/livekit/agents/aio/channel.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/aio/debug.py` & `livekit_agents-0.6.dev1/livekit/agents/aio/debug.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/aio/interval.py` & `livekit_agents-0.6.dev1/livekit/agents/aio/interval.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/aio/select.py` & `livekit_agents-0.6.dev1/livekit/agents/aio/select.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/aio/sleep.py` & `livekit_agents-0.6.dev1/livekit/agents/aio/sleep.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/aio/wait_group.py` & `livekit_agents-0.6.dev1/livekit/agents/aio/wait_group.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/apipe.py` & `livekit_agents-0.6.dev1/livekit/agents/apipe.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/cli/cli.py` & `livekit_agents-0.6.dev1/livekit/agents/cli/cli.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/cli/log.py` & `livekit_agents-0.6.dev1/livekit/agents/cli/log.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/cli/protocol.py` & `livekit_agents-0.6.dev1/livekit/agents/cli/protocol.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/cli/watcher.py` & `livekit_agents-0.6.dev1/livekit/agents/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/codecs/__init__.py` & `livekit_agents-0.6.dev1/livekit/agents/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/codecs/mp3.py` & `livekit_agents-0.6.dev1/livekit/agents/codecs/mp3.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/http_server.py` & `livekit_agents-0.6.dev1/livekit/agents/http_server.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/ipc/job_main.py` & `livekit_agents-0.6.dev1/livekit/agents/ipc/job_main.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/ipc/job_process.py` & `livekit_agents-0.6.dev1/livekit/agents/ipc/job_process.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/ipc/protocol.py` & `livekit_agents-0.6.dev1/livekit/agents/ipc/protocol.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/ipc_enc.py` & `livekit_agents-0.6.dev1/livekit/agents/ipc_enc.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/job_context.py` & `livekit_agents-0.6.dev1/livekit/agents/job_context.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/job_request.py` & `livekit_agents-0.6.dev1/livekit/agents/job_request.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/llm/__init__.py` & `livekit_agents-0.6.dev1/livekit/agents/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/llm/function_context.py` & `livekit_agents-0.6.dev1/livekit/agents/llm/function_context.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/llm/llm.py` & `livekit_agents-0.6.dev1/livekit/agents/llm/llm.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/plugin.py` & `livekit_agents-0.6.dev1/livekit/agents/plugin.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/stt/stream_adapter.py` & `livekit_agents-0.6.dev1/livekit/agents/stt/stream_adapter.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/stt/stt.py` & `livekit_agents-0.6.dev1/livekit/agents/stt/stt.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/tokenize/sentence_tokenizer.py` & `livekit_agents-0.6.dev1/livekit/agents/tokenize/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/tts/stream_adapter.py` & `livekit_agents-0.6.dev1/livekit/agents/tts/stream_adapter.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/tts/tts.py` & `livekit_agents-0.6.dev1/livekit/agents/tts/tts.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/utils/event_emitter.py` & `livekit_agents-0.6.dev1/livekit/agents/utils/event_emitter.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/utils/exp_filter.py` & `livekit_agents-0.6.dev1/livekit/agents/utils/exp_filter.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/utils/misc.py` & `livekit_agents-0.6.dev1/livekit/agents/utils/misc.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/utils/moving_average.py` & `livekit_agents-0.6.dev1/livekit/agents/utils/moving_average.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/vad.py` & `livekit_agents-0.6.dev1/livekit/agents/vad.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/version.py` & `livekit_agents-0.6.dev1/livekit/agents/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.6.dev0"
+__version__ = "0.6.dev1"
```

### Comparing `livekit_agents-0.6.dev0/livekit/agents/voice_assistant/assistant.py` & `livekit_agents-0.6.dev1/livekit/agents/voice_assistant/assistant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import contextlib
 import contextvars
 import time
-from typing import Any, AsyncIterable, Callable, Literal, override
+from typing import Any, AsyncIterable, Callable, Literal
 
 from attrs import define
 from livekit import rtc
 
 from .. import aio, utils
 from .. import llm as allm
 from .. import stt as astt
@@ -159,15 +159,14 @@
         self._speech_prob = 0.0
         self._speaking_avg = utils.MovingAverage(
             int(self._opts.int_speech_duration * 100)
         )
         self._transcripted_text, self._interim_text = "", ""
         self._start_future = asyncio.Future()
 
-    @override
     def on(self, event: EventTypes, callback: Callable | None = None) -> Callable:
         """Register a callback for an event
 
         Args:
             event: the event to listen to (see EventTypes)
                 - user_started_speaking: the user started speaking
                 - user_stopped_speaking: the user stopped speaking
```

### Comparing `livekit_agents-0.6.dev0/livekit/agents/voice_assistant/plotter.py` & `livekit_agents-0.6.dev1/livekit/agents/voice_assistant/plotter.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit/agents/worker.py` & `livekit_agents-0.6.dev1/livekit/agents/worker.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/livekit_agents.egg-info/PKG-INFO` & `livekit_agents-0.6.dev1/livekit_agents.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.6.dev0
+Version: 0.6.dev1
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
```

### Comparing `livekit_agents-0.6.dev0/livekit_agents.egg-info/SOURCES.txt` & `livekit_agents-0.6.dev1/livekit_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev0/setup.py` & `livekit_agents-0.6.dev1/setup.py`

 * *Files identical despite different names*

