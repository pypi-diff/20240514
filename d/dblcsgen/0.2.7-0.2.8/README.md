# Comparing `tmp/dblcsgen-0.2.7.tar.gz` & `tmp/dblcsgen-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblcsgen-0.2.7.tar", last modified: Mon May 13 11:55:28 2024, max compression
+gzip compressed data, was "dblcsgen-0.2.8.tar", last modified: Tue May 14 07:09:12 2024, max compression
```

## Comparing `dblcsgen-0.2.7.tar` & `dblcsgen-0.2.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.322348 dblcsgen-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 11:55:26.000000 dblcsgen-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-05-13 11:55:28.322348 dblcsgen-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-05-13 11:55:26.000000 dblcsgen-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.322348 dblcsgen-0.2.7/dblcsgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-05-13 11:55:28.000000 dblcsgen-0.2.7/dblcsgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-13 11:55:28.000000 dblcsgen-0.2.7/dblcsgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:55:28.000000 dblcsgen-0.2.7/dblcsgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-13 11:55:28.000000 dblcsgen-0.2.7/dblcsgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 11:55:28.000000 dblcsgen-0.2.7/dblcsgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:55:28.322348 dblcsgen-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.310349 dblcsgen-0.2.7/sglang/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.310349 dblcsgen-0.2.7/sglang/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/backend/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/backend/runtime_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/global_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.310349 dblcsgen-0.2.7/sglang/lang/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/lang/chat_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/lang/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    28189 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/lang/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/lang/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/lang/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/launch_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.314349 dblcsgen-0.2.7/sglang/srt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.314349 dblcsgen-0.2.7/sglang/srt/constrained/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/constrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/constrained/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/constrained/fsm_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/constrained/jump_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/flush_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/hf_transformers_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.314349 dblcsgen-0.2.7/sglang/srt/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/layers/context_flashattention_nopad.py
--rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/layers/extend_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/layers/logits_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/layers/radix_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/layers/token_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.314349 dblcsgen-0.2.7/sglang/srt/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/detokenizer_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/io_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.318349 dblcsgen-0.2.7/sglang/srt/managers/router/
--rw-r--r--   0 runner    (1001) docker     (127)    19910 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/router/infer_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/router/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    29391 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/router/model_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/router/model_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/router/radix_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/router/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12294 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/tokenizer_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/memory_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/mm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.318349 dblcsgen-0.2.7/sglang/srt/models/
--rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/commandr.py
--rw-r--r--   0 runner    (1001) docker     (127)    14158 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/dbrx.py
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/dbrx_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/gemma.py
--rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14941 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/llava.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/mixtral.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/qwen.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/qwen2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/stablelm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/yivl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/openai_api_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/openai_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/sampling_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/server_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/weight_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.322348 dblcsgen-0.2.7/sglang/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/test/test_conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/test/test_openai_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/test/test_programs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.730622 dblcsgen-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 07:09:10.000000 dblcsgen-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-05-14 07:09:12.730622 dblcsgen-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-05-14 07:09:10.000000 dblcsgen-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.730622 dblcsgen-0.2.8/dblcsgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-05-14 07:09:12.000000 dblcsgen-0.2.8/dblcsgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-14 07:09:12.000000 dblcsgen-0.2.8/dblcsgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:09:12.000000 dblcsgen-0.2.8/dblcsgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 07:09:12.000000 dblcsgen-0.2.8/dblcsgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 07:09:12.000000 dblcsgen-0.2.8/dblcsgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:09:12.730622 dblcsgen-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.718622 dblcsgen-0.2.8/sglang/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.718622 dblcsgen-0.2.8/sglang/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/backend/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/backend/runtime_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/global_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.718622 dblcsgen-0.2.8/sglang/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/lang/chat_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/lang/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27999 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/lang/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11522 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/lang/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/lang/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/launch_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.722622 dblcsgen-0.2.8/sglang/srt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.722622 dblcsgen-0.2.8/sglang/srt/constrained/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/constrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/constrained/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/constrained/fsm_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/constrained/jump_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/flush_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/hf_transformers_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.722622 dblcsgen-0.2.8/sglang/srt/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/layers/context_flashattention_nopad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/layers/extend_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/layers/logits_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/layers/radix_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/layers/token_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.722622 dblcsgen-0.2.8/sglang/srt/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/detokenizer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/io_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.726622 dblcsgen-0.2.8/sglang/srt/managers/router/
+-rw-r--r--   0 runner    (1001) docker     (127)    20204 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/router/infer_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/router/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29381 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/router/model_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/router/model_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/router/radix_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/router/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/tokenizer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/memory_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/mm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.726622 dblcsgen-0.2.8/sglang/srt/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/commandr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14158 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/dbrx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/dbrx_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/gemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14941 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/llava.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/mixtral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/qwen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/qwen2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/stablelm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/yivl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/openai_api_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/openai_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/sampling_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/server_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/weight_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.730622 dblcsgen-0.2.8/sglang/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/test/test_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/test/test_openai_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/test/test_programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/utils.py
```

### Comparing `dblcsgen-0.2.7/LICENSE` & `dblcsgen-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/PKG-INFO` & `dblcsgen-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.7
+Version: 0.2.8
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dblcsgen-0.2.7/README.md` & `dblcsgen-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/dblcsgen.egg-info/PKG-INFO` & `dblcsgen-0.2.8/dblcsgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.7
+Version: 0.2.8
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dblcsgen-0.2.7/dblcsgen.egg-info/SOURCES.txt` & `dblcsgen-0.2.8/dblcsgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/pyproject.toml` & `dblcsgen-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dblcsgen"
-version = "0.2.7"
+version = "0.2.8"
 description = "DBLC Fast Structured Generation"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `dblcsgen-0.2.7/sglang/__init__.py` & `dblcsgen-0.2.8/sglang/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.15"
+__version__ = "0.2.8"
 
 # SGL API Components
 from sglang.api import (
     Runtime,
     assistant,
     assistant_begin,
     assistant_end,
@@ -18,29 +18,23 @@
     system,
     user,
     user_begin,
     user_end,
 )
 
 # SGL Backends
-from sglang.backend.anthropic import Anthropic
-from sglang.backend.openai import OpenAI
 from sglang.backend.runtime_endpoint import RuntimeEndpoint
-from sglang.backend.vertexai import VertexAI
 
 # Global Configurations
 from sglang.global_config import global_config
 
 # public APIs management
 __all__ = [
     "global_config",
-    "Anthropic",
-    "OpenAI",
     "RuntimeEndpoint",
-    "VertexAI",
     "function",
     "Runtime",
     "set_default_backend",
     "flush_cache",
     "get_server_args",
     "gen",
     "gen_int",
```

### Comparing `dblcsgen-0.2.7/sglang/api.py` & `dblcsgen-0.2.8/sglang/api.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/backend/base_backend.py` & `dblcsgen-0.2.8/sglang/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/backend/runtime_endpoint.py` & `dblcsgen-0.2.8/sglang/backend/runtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/global_config.py` & `dblcsgen-0.2.8/sglang/global_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
         # Output configs
         self.skip_special_tokens_in_output = True
         self.spaces_between_special_tokens_in_out = True
 
         # Optimization configs
         self.eager_fill_image = False
-        self.enable_prefix_sharing = True
+        self.enable_precache_with_tracing = True
         self.enable_parallel_encoding = True
         self.enable_parallel_decoding = True
 
         # Choices: ["no_adjust", "adjust_cache"]
         # no_adjust: Do not adjust the position embedding of KV cache.
         # adjust_cache: Adjust the position embedding of KV cache.
         self.concate_and_append_mode = "no_adjust"
```

### Comparing `dblcsgen-0.2.7/sglang/lang/chat_template.py` & `dblcsgen-0.2.8/sglang/lang/chat_template.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/lang/compiler.py` & `dblcsgen-0.2.8/sglang/lang/compiler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/lang/interpreter.py` & `dblcsgen-0.2.8/sglang/lang/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,17 @@
     default_sampling_para,
     num_threads,
     progress_bar,
 ):
     if hasattr(backend, "endpoint"):
         backend = backend.endpoint
 
-    # Extract prefix by tracing and cache it
-    if len(batch_arguments) > 1:
-        pin_program(program, backend)
+    # Pre-cache the common prefix for a batch. The prefix is extracted by tracing the program.
+    if global_config.enable_precache_with_tracing and len(batch_arguments) > 1:
+        cache_program(program, backend)
 
     # Run all programs
     if num_threads == "auto":
         num_threads = max(96, multiprocessing.cpu_count() * 16)
     num_threads = min(num_threads, len(batch_arguments))
 
     if num_threads == 1:
@@ -150,29 +150,20 @@
 
         if progress_bar:
             pbar.close()
 
     return rets
 
 
-def pin_program(program, backend):
-    if global_config.enable_prefix_sharing and program.pin_prefix_rid is None:
-        # TODO: handle multiple backends
-        from sglang.lang.tracer import extract_prefix_by_tracing
-
-        prefix = extract_prefix_by_tracing(program, backend)
-        if prefix and len(prefix) > 64:
-            prefix_rid = backend.cache_prefix(prefix)
-            program.pin_prefix_rid = prefix_rid
-            return prefix_rid
-    return None
+def cache_program(program, backend):
+    from sglang.lang.tracer import extract_prefix_by_tracing
 
-
-def unpin_program(program, backend):
-    pass
+    prefix = extract_prefix_by_tracing(program, backend)
+    if prefix and len(prefix) > 64:
+        backend.cache_prefix(prefix)
 
 
 class StreamExecutor:
     """A stream executor that executes SGL expressions in a background thread."""
 
     def __init__(
         self,
@@ -318,15 +309,15 @@
             if expr is None:
                 self.queue.task_done()
                 break
 
             try:
                 self._execute(expr)
             except Exception as e:
-                print(f"Error in stream_executor: {get_exception_traceback()}")
+                # print(f"Error in stream_executor: {get_exception_traceback()}")
                 error = e
                 break
             self.queue.task_done()
             if self.stream_text_event:
                 self.stream_text_event.set()
 
         # Clean the queue and events
@@ -698,17 +689,18 @@
     def text(self):
         return self.stream_executor.text()
 
     def messages(self):
         return self.stream_executor.messages()
 
     def sync(self):
-        ret = self.stream_executor.sync()
-        self.error = self.stream_executor.error
-        return ret
+        return self.stream_executor.sync()
+
+    def error(self):
+        return self.stream_executor.error
 
     def text_iter(self, var_name: Optional[str] = None):
         if self.stream_executor.stream:
             prev = 0
             if var_name is None:
                 event = self.stream_executor.stream_text_event
                 while True:
```

### Comparing `dblcsgen-0.2.7/sglang/lang/ir.py` & `dblcsgen-0.2.8/sglang/lang/ir.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,57 +35,14 @@
             self.temperature,
             self.top_p,
             self.top_k,
             self.frequency_penalty,
             self.presence_penalty,
         )
 
-    def to_openai_kwargs(self):
-        # OpenAI does not support top_k, so we drop it here
-        if self.regex is not None:
-            warnings.warn("Regular expression is not supported in the OpenAI backend.")
-        return {
-            "max_tokens": self.max_new_tokens,
-            "stop": self.stop or None,
-            "temperature": self.temperature,
-            "top_p": self.top_p,
-            "frequency_penalty": self.frequency_penalty,
-            "presence_penalty": self.presence_penalty,
-        }
-
-    def to_vertexai_kwargs(self):
-        if self.regex is not None:
-            warnings.warn(
-                "Regular expression is not supported in the VertexAI backend."
-            )
-        return {
-            "candidate_count": 1,
-            "max_output_tokens": self.max_new_tokens,
-            "stop_sequences": self.stop,
-            "temperature": self.temperature,
-            "top_p": self.top_p,
-            "top_k": self.top_k if self.top_k > 0 else None,
-        }
-
-    def to_anthropic_kwargs(self):
-        # Anthropic does not support frequency_penalty or presence_penalty, so we drop it here
-        if self.regex is not None:
-            warnings.warn(
-                "Regular expression is not supported in the Anthropic backend."
-            )
-        return {
-            "max_tokens": self.max_new_tokens,
-            "stop_sequences": (
-                self.stop if isinstance(self.stop, (list, tuple)) else [self.stop]
-            ),
-            "temperature": self.temperature,
-            "top_p": self.top_p,
-            "top_k": self.top_k,
-        }
-
     def to_srt_kwargs(self):
         return {
             "max_new_tokens": self.max_new_tokens,
             "stop": self.stop,
             "temperature": self.temperature,
             "top_p": self.top_p,
             "top_k": self.top_k,
@@ -189,25 +146,19 @@
 
     def trace(self, *, backend=None, **kwargs):
         from sglang.lang.tracer import trace_program
 
         backend = backend or global_config.default_backend
         return trace_program(self, kwargs, backend)
 
-    def pin(self, backend=None):
-        from sglang.lang.interpreter import pin_program
-
-        backend = backend or global_config.default_backend
-        return pin_program(self, backend)
-
-    def unpin(self, backend=None):
-        from sglang.lang.interpreter import unpin_program
+    def cache(self, backend=None):
+        from sglang.lang.interpreter import cache_program
 
         backend = backend or global_config.default_backend
-        return unpin_program(self, backend)
+        return cache_program(self, backend)
 
     def compile(self, *, backend=None):
         from sglang.lang.compiler import compile_func
 
         return compile_func(self, backend)
 
     def __call__(self, *args, **kwargs):
```

### Comparing `dblcsgen-0.2.7/sglang/lang/tracer.py` & `dblcsgen-0.2.8/sglang/lang/tracer.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/constrained/__init__.py` & `dblcsgen-0.2.8/sglang/srt/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/constrained/base_cache.py` & `dblcsgen-0.2.8/sglang/srt/constrained/base_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/constrained/fsm_cache.py` & `dblcsgen-0.2.8/sglang/srt/constrained/fsm_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/constrained/jump_forward.py` & `dblcsgen-0.2.8/sglang/srt/constrained/jump_forward.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/conversation.py` & `dblcsgen-0.2.8/sglang/srt/conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/hf_transformers_utils.py` & `dblcsgen-0.2.8/sglang/srt/hf_transformers_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/layers/context_flashattention_nopad.py` & `dblcsgen-0.2.8/sglang/srt/layers/context_flashattention_nopad.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/layers/extend_attention.py` & `dblcsgen-0.2.8/sglang/srt/layers/extend_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/layers/logits_processor.py` & `dblcsgen-0.2.8/sglang/srt/layers/logits_processor.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/layers/radix_attention.py` & `dblcsgen-0.2.8/sglang/srt/layers/radix_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/layers/token_attention.py` & `dblcsgen-0.2.8/sglang/srt/layers/token_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/managers/detokenizer_manager.py` & `dblcsgen-0.2.8/sglang/srt/managers/detokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/managers/io_struct.py` & `dblcsgen-0.2.8/sglang/srt/managers/io_struct.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/managers/router/infer_batch.py` & `dblcsgen-0.2.8/sglang/srt/managers/router/infer_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,25 @@
 
 
 class FinishReason(IntEnum):
     EOS_TOKEN = auto()
     LENGTH = auto()
     STOP_STR = auto()
 
+    @staticmethod
+    def to_str(reason):
+        if reason == FinishReason.EOS_TOKEN:
+            return None
+        elif reason == FinishReason.LENGTH:
+            return "length"
+        elif reason == FinishReason.STOP_STR:
+            return "stop"
+        else:
+            return None
+
 
 class Req:
     def __init__(self, rid, input_text, input_ids):
         self.rid = rid
         self.input_text = input_text
         self.input_ids = input_ids
         self.output_ids = []
```

### Comparing `dblcsgen-0.2.7/sglang/srt/managers/router/manager.py` & `dblcsgen-0.2.8/sglang/srt/managers/router/manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import logging
 
 import uvloop
 import zmq
 import zmq.asyncio
 
-from sglang import global_config
+from sglang.global_config import global_config
 from sglang.srt.managers.router.model_rpc import ModelRpcClient
 from sglang.srt.server_args import PortArgs, ServerArgs
 from sglang.srt.utils import get_exception_traceback
 
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
```

### Comparing `dblcsgen-0.2.7/sglang/srt/managers/router/model_rpc.py` & `dblcsgen-0.2.8/sglang/srt/managers/router/model_rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from sglang.srt.constrained.jump_forward import JumpForwardCache
 from sglang.srt.hf_transformers_utils import get_processor, get_tokenizer
 from sglang.srt.managers.io_struct import (
     BatchTokenIDOut,
     FlushCacheReq,
     TokenizedGenerateReqInput,
 )
-from sglang.srt.managers.router.infer_batch import Batch, ForwardMode, Req
+from sglang.srt.managers.router.infer_batch import Batch, ForwardMode, Req, FinishReason
 from sglang.srt.managers.router.model_runner import ModelRunner
 from sglang.srt.managers.router.radix_cache import RadixCache
 from sglang.srt.managers.router.scheduler import Scheduler
 from sglang.srt.model_config import ModelConfig
 from sglang.srt.server_args import PortArgs, ServerArgs
 from sglang.srt.utils import (
     get_exception_traceback,
@@ -608,15 +608,15 @@
 
                 meta_info = {
                     "prompt_tokens": req.prompt_tokens,
                     "completion_tokens": len(req.input_ids)
                     + len(req.output_ids)
                     - req.prompt_tokens,
                     "completion_tokens_wo_jump_forward": req.completion_tokens_wo_jump_forward,
-                    "finish_reason": str(req.finish_reason),  # FIXME: convert to the correct string
+                    "finish_reason": FinishReason.to_str(req.finish_reason),
                     "hit_stop_str": req.hit_stop_str,
                 }
                 if req.return_logprob:
                     (
                         meta_info["prefill_token_logprobs"],
                         meta_info["decode_token_logprobs"],
                         meta_info["prefill_top_logprobs"],
```

### Comparing `dblcsgen-0.2.7/sglang/srt/managers/router/model_runner.py` & `dblcsgen-0.2.8/sglang/srt/managers/router/model_runner.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/managers/router/radix_cache.py` & `dblcsgen-0.2.8/sglang/srt/managers/router/radix_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/managers/router/scheduler.py` & `dblcsgen-0.2.8/sglang/srt/managers/router/scheduler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/managers/tokenizer_manager.py` & `dblcsgen-0.2.8/sglang/srt/managers/tokenizer_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,14 @@
         self.send_to_router = context.socket(zmq.PUSH)
         self.send_to_router.connect(f"tcp://127.0.0.1:{port_args.router_port}")
 
         self.model_path = server_args.model_path
         self.hf_config = get_config(
             self.model_path, trust_remote_code=server_args.trust_remote_code
         )
-
         self.context_len = get_context_length(self.hf_config)
 
         if is_multimodal_model(self.model_path):
             self.processor = get_processor(
                 server_args.tokenizer_path,
                 tokenizer_mode=server_args.tokenizer_mode,
                 trust_remote_code=server_args.trust_remote_code,
@@ -152,14 +151,20 @@
             rid = obj.rid
 
             if obj.input_ids is None:
                 input_ids = self.tokenizer.encode(obj.text)
             else:
                 input_ids = obj.input_ids
 
+            if len(input_ids) >= self.context_len:
+                raise ValueError(
+                    f"The input ({len(input_ids)} tokens) is longer than the "
+                    f"model's context length ({self.context_len} tokens)"
+                )
+
             sampling_params = SamplingParams(**obj.sampling_params)
             if sampling_params.max_new_tokens != 0:
                 sampling_params.normalize(self.tokenizer)
                 sampling_params.verify()
 
             if isinstance(obj.image_data, list) and len(obj.image_data) > 0:
                 pixel_values, image_hash, image_size = await self.get_pixel_values(
```

### Comparing `dblcsgen-0.2.7/sglang/srt/memory_pool.py` & `dblcsgen-0.2.8/sglang/srt/memory_pool.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/mm_utils.py` & `dblcsgen-0.2.8/sglang/srt/mm_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/model_config.py` & `dblcsgen-0.2.8/sglang/srt/model_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/models/commandr.py` & `dblcsgen-0.2.8/sglang/srt/models/commandr.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/models/dbrx.py` & `dblcsgen-0.2.8/sglang/srt/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/models/dbrx_config.py` & `dblcsgen-0.2.8/sglang/srt/models/dbrx_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/models/gemma.py` & `dblcsgen-0.2.8/sglang/srt/models/gemma.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/models/llama2.py` & `dblcsgen-0.2.8/sglang/srt/models/llama2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/models/llava.py` & `dblcsgen-0.2.8/sglang/srt/models/llava.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/models/mixtral.py` & `dblcsgen-0.2.8/sglang/srt/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/models/qwen.py` & `dblcsgen-0.2.8/sglang/srt/models/qwen.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/models/qwen2.py` & `dblcsgen-0.2.8/sglang/srt/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/models/stablelm.py` & `dblcsgen-0.2.8/sglang/srt/models/stablelm.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/models/yivl.py` & `dblcsgen-0.2.8/sglang/srt/models/yivl.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/openai_api_adapter.py` & `dblcsgen-0.2.8/sglang/srt/openai_api_adapter.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/openai_protocol.py` & `dblcsgen-0.2.8/sglang/srt/openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/sampling_params.py` & `dblcsgen-0.2.8/sglang/srt/sampling_params.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/server.py` & `dblcsgen-0.2.8/sglang/srt/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import aiohttp
 import psutil
 import requests
 import uvicorn
 import uvloop
 from fastapi import FastAPI, Request
-from fastapi.responses import Response, StreamingResponse
+from fastapi.responses import JSONResponse, Response, StreamingResponse
 
 from sglang.backend.runtime_endpoint import RuntimeEndpoint
 from sglang.srt.constrained import disable_cache
 from sglang.srt.hf_transformers_utils import get_tokenizer
 from sglang.srt.managers.detokenizer_manager import start_detokenizer_process
 from sglang.srt.managers.io_struct import GenerateReqInput
 from sglang.srt.managers.router.manager import start_router_process
@@ -86,16 +86,19 @@
         async def stream_results():
             async for out in tokenizer_manager.generate_request(obj):
                 yield f"data: {json.dumps(out, ensure_ascii=False)}\n\n"
             yield "data: [DONE]\n\n"
 
         return StreamingResponse(stream_results(), media_type="text/event-stream")
 
-    ret = await tokenizer_manager.generate_request(obj).__anext__()
-    return ret
+    try:
+        ret = await tokenizer_manager.generate_request(obj).__anext__()
+        return ret
+    except ValueError as e:
+        return JSONResponse({"error": str(e)}, status_code=400)
 
 
 @app.post("/v1/completions")
 async def openai_v1_completions(raw_request: Request):
     return await v1_completions(tokenizer_manager, raw_request)
```

### Comparing `dblcsgen-0.2.7/sglang/srt/server_args.py` & `dblcsgen-0.2.8/sglang/srt/server_args.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/utils.py` & `dblcsgen-0.2.8/sglang/srt/utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/srt/weight_utils.py` & `dblcsgen-0.2.8/sglang/srt/weight_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/test/test_conversation.py` & `dblcsgen-0.2.8/sglang/test/test_conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/test/test_openai_protocol.py` & `dblcsgen-0.2.8/sglang/test/test_openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/test/test_programs.py` & `dblcsgen-0.2.8/sglang/test/test_programs.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/test/test_utils.py` & `dblcsgen-0.2.8/sglang/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.7/sglang/utils.py` & `dblcsgen-0.2.8/sglang/utils.py`

 * *Files identical despite different names*

