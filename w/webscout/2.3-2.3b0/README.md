# Comparing `tmp/webscout-2.3.tar.gz` & `tmp/webscout-2.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-2.3.tar", last modified: Mon May 13 10:26:44 2024, max compression
+gzip compressed data, was "webscout-2.3b0.tar", last modified: Mon May 13 08:26:00 2024, max compression
```

## Comparing `webscout-2.3.tar` & `webscout-2.3b0.tar`

### file list

```diff
@@ -1,78 +1,70 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 10:26:44.829917 webscout-2.3/
-drwxrwxrwx   0        0        0        0 2024-05-13 10:26:40.900384 webscout-2.3/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:26:40.921401 webscout-2.3/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.3/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.3/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:26:40.982367 webscout-2.3/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.3/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.3/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.3/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.3/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:26:41.053128 webscout-2.3/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.3/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.3/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.3/LICENSE.md
--rw-rw-rw-   0        0        0    46601 2024-05-13 10:26:44.816928 webscout-2.3/PKG-INFO
--rw-rw-rw-   0        0        0    44185 2024-05-12 05:27:05.000000 webscout-2.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 10:26:44.830921 webscout-2.3/setup.cfg
--rw-rw-rw-   0        0        0     2691 2024-05-13 08:59:13.000000 webscout-2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:26:41.419763 webscout-2.3/webscout/
--rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.3/webscout/AIauto.py
--rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.3/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33266 2024-05-12 05:18:53.000000 webscout-2.3/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.3/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.3/webscout/LLM.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:26:43.095285 webscout-2.3/webscout/Local/
--rw-rw-rw-   0        0        0      220 2024-05-13 10:17:11.000000 webscout-2.3/webscout/Local/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-13 10:17:01.000000 webscout-2.3/webscout/Local/_version.py
--rw-rw-rw-   0        0        0    17153 2024-05-13 10:22:12.000000 webscout-2.3/webscout/Local/formats.py
--rw-rw-rw-   0        0        0    27611 2024-05-13 10:21:04.000000 webscout-2.3/webscout/Local/model.py
--rw-rw-rw-   0        0        0     4372 2024-05-13 10:22:16.000000 webscout-2.3/webscout/Local/samplers.py
--rw-rw-rw-   0        0        0    24868 2024-05-13 10:21:08.000000 webscout-2.3/webscout/Local/thread.py
--rw-rw-rw-   0        0        0     5454 2024-05-13 10:22:08.000000 webscout-2.3/webscout/Local/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:26:44.295984 webscout-2.3/webscout/Provider/
--rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.3/webscout/Provider/Berlin4h.py
--rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.3/webscout/Provider/Blackboxai.py
--rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.3/webscout/Provider/ChatGPTUK.py
--rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.3/webscout/Provider/Cohere.py
--rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.3/webscout/Provider/Gemini.py
--rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.3/webscout/Provider/Groq.py
--rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.3/webscout/Provider/Koboldai.py
--rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.3/webscout/Provider/Leo.py
--rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.3/webscout/Provider/Llama2.py
--rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.3/webscout/Provider/OpenGPT.py
--rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.3/webscout/Provider/Openai.py
--rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.3/webscout/Provider/Perplexity.py
--rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.3/webscout/Provider/Phind.py
--rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.3/webscout/Provider/Reka.py
--rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.3/webscout/Provider/ThinkAnyAI.py
--rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.3/webscout/Provider/Xjai.py
--rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.3/webscout/Provider/Yepchat.py
--rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.3/webscout/Provider/Youchat.py
--rw-rw-rw-   0        0        0     1318 2024-05-13 09:09:36.000000 webscout-2.3/webscout/Provider/__init__.py
--rw-rw-rw-   0        0        0     2206 2024-05-13 10:17:20.000000 webscout-2.3/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.3/webscout/__main__.py
--rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.3/webscout/async_providers.py
--rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-2.3/webscout/cli.py
--rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.3/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.3/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.3/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.3/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.3/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.3/webscout/utils.py
--rw-rw-rw-   0        0        0       23 2024-05-11 09:00:53.000000 webscout-2.3/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.3/webscout/voice.py
--rw-rw-rw-   0        0        0    84668 2024-05-12 05:18:15.000000 webscout-2.3/webscout/webai.py
--rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-2.3/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-2.3/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:26:44.746041 webscout-2.3/webscout.egg-info/
--rw-rw-rw-   0        0        0    46601 2024-05-13 10:26:39.000000 webscout-2.3/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1772 2024-05-13 10:26:40.000000 webscout-2.3/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 10:26:39.000000 webscout-2.3/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-13 10:26:39.000000 webscout-2.3/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      366 2024-05-13 10:26:39.000000 webscout-2.3/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-13 10:26:39.000000 webscout-2.3/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.429375 webscout-2.3b0/
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.019969 webscout-2.3b0/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.055985 webscout-2.3b0/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.089983 webscout-2.3b0/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.103987 webscout-2.3b0/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.3b0/LICENSE.md
+-rw-rw-rw-   0        0        0    46603 2024-05-13 08:26:00.421374 webscout-2.3b0/PKG-INFO
+-rw-rw-rw-   0        0        0    44185 2024-05-12 05:27:05.000000 webscout-2.3b0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 08:26:00.429375 webscout-2.3b0/setup.cfg
+-rw-rw-rw-   0        0        0     2696 2024-05-13 08:03:16.000000 webscout-2.3b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.231150 webscout-2.3b0/webscout/
+-rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.3b0/webscout/AIauto.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33266 2024-05-12 05:18:53.000000 webscout-2.3b0/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/LLM.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.387383 webscout-2.3b0/webscout/Provider/
+-rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.3b0/webscout/Provider/Berlin4h.py
+-rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.3b0/webscout/Provider/Blackboxai.py
+-rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.3b0/webscout/Provider/ChatGPTUK.py
+-rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.3b0/webscout/Provider/Cohere.py
+-rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.3b0/webscout/Provider/Gemini.py
+-rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.3b0/webscout/Provider/Groq.py
+-rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.3b0/webscout/Provider/Koboldai.py
+-rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.3b0/webscout/Provider/Leo.py
+-rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.3b0/webscout/Provider/Llama2.py
+-rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.3b0/webscout/Provider/OpenGPT.py
+-rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.3b0/webscout/Provider/Openai.py
+-rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.3b0/webscout/Provider/Perplexity.py
+-rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.3b0/webscout/Provider/Phind.py
+-rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.3b0/webscout/Provider/Reka.py
+-rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.3b0/webscout/Provider/ThinkAnyAI.py
+-rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.3b0/webscout/Provider/Xjai.py
+-rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.3b0/webscout/Provider/Yepchat.py
+-rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.3b0/webscout/Provider/Youchat.py
+-rw-rw-rw-   0        0        0     1318 2024-05-12 05:15:53.000000 webscout-2.3b0/webscout/Provider/__init__.py
+-rw-rw-rw-   0        0        0     2256 2024-05-13 08:07:51.000000 webscout-2.3b0/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/__main__.py
+-rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.3b0/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/cli.py
+-rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.3b0/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.3b0/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.3b0/webscout/utils.py
+-rw-rw-rw-   0        0        0       23 2024-05-11 09:00:53.000000 webscout-2.3b0/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/voice.py
+-rw-rw-rw-   0        0        0    84668 2024-05-12 05:18:15.000000 webscout-2.3b0/webscout/webai.py
+-rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-2.3b0/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-2.3b0/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.395371 webscout-2.3b0/webscout.egg-info/
+-rw-rw-rw-   0        0        0    46603 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1592 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      366 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/top_level.txt
```

### Comparing `webscout-2.3/DeepWEBS/documents/query_results_extractor.py` & `webscout-2.3b0/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-2.3b0/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/DeepWEBS/networks/filepath_converter.py` & `webscout-2.3b0/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/DeepWEBS/networks/google_searcher.py` & `webscout-2.3b0/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/DeepWEBS/networks/network_configs.py` & `webscout-2.3b0/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/DeepWEBS/networks/webpage_fetcher.py` & `webscout-2.3b0/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/DeepWEBS/utilsdw/enver.py` & `webscout-2.3b0/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/DeepWEBS/utilsdw/logger.py` & `webscout-2.3b0/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/LICENSE.md` & `webscout-2.3b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-2.3/PKG-INFO` & `webscout-2.3b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.3
+Version: 2.3b0
 Summary: Search for anything using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
```

#### html2text {}

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.3 Summary: Search for anything
-using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt
-videos, temporary email and phone number generation, has TTS support, and webai
-(terminal gpt and open interpreter). Author: OEvortex Author-email:
-helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
-Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
-github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
-youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: License :: Other/
-Proprietary License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Programming Language :: Python :: Implementation :: CPython Classifier: Topic
-:: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Description-Content-Type: text/
-markdown License-File: LICENSE.md Requires-Dist: docstring_inheritance
-Requires-Dist: click Requires-Dist: curl_cffi Requires-Dist: lxml Requires-
-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist: tqdm Requires-Dist:
-webdriver-manager Requires-Dist: halo>=0.0.31 Requires-Dist: g4f>=0.2.2.3
-Requires-Dist: rich Requires-Dist: python-dotenv Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify Requires-Dist: pydantic Requires-Dist: requests
-Requires-Dist: sse_starlette Requires-Dist: termcolor Requires-Dist: tiktoken
-Requires-Dist: tldextract Requires-Dist: orjson Requires-Dist: PyYAML Requires-
-Dist: appdirs Requires-Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client
-Requires-Dist: clipman Requires-Dist: playsound Provides-Extra: dev Requires-
-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
-Provides-Extra: local Requires-Dist: llama-cpp-python; extra == "local"
-Requires-Dist: colorama; extra == "local" Requires-Dist: numpy; extra ==
-"local"
+Metadata-Version: 2.1 Name: webscout Version: 2.3b0 Summary: Search for
+anything using Google, DuckDuckGo, phind.com. Also contains AI models, can
+transcribe yt videos, temporary email and phone number generation, has TTS
+support, and webai (terminal gpt and open interpreter). Author: OEvortex
+Author-email: helpingai5@gmail.com License: HelpingAI Simplified Universal
+License Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
+Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
+https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: License ::
+Other/Proprietary License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
+:: Software Development :: Libraries :: Python Modules Description-Content-
+Type: text/markdown License-File: LICENSE.md Requires-Dist:
+docstring_inheritance Requires-Dist: click Requires-Dist: curl_cffi Requires-
+Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
+tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
+Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
+Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
+Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
+Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
+Requires-Dist: PyYAML Requires-Dist: appdirs Requires-Dist: GoogleBard1>=2.1.4
+Requires-Dist: tls_client Requires-Dist: clipman Requires-Dist: playsound
+Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist:
+pytest>=7.4.2; extra == "dev" Provides-Extra: local Requires-Dist: llama-cpp-
+python; extra == "local" Requires-Dist: colorama; extra == "local" Requires-
+Dist: numpy; extra == "local"
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
 phind.com. Also containes AI models, can transcribe yt videos, temporary email
```

### Comparing `webscout-2.3/README.md` & `webscout-2.3b0/README.md`

 * *Files identical despite different names*

### Comparing `webscout-2.3/setup.py` & `webscout-2.3b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="2.3",
+    version="2.3-beta",
     description="Search for anything using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-2.3/webscout/AIauto.py` & `webscout-2.3b0/webscout/AIauto.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/AIbase.py` & `webscout-2.3b0/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/AIutel.py` & `webscout-2.3b0/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/DWEBS.py` & `webscout-2.3b0/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/LLM.py` & `webscout-2.3b0/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Berlin4h.py` & `webscout-2.3b0/webscout/Provider/Berlin4h.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Blackboxai.py` & `webscout-2.3b0/webscout/Provider/Blackboxai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/ChatGPTUK.py` & `webscout-2.3b0/webscout/Provider/ChatGPTUK.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Cohere.py` & `webscout-2.3b0/webscout/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Gemini.py` & `webscout-2.3b0/webscout/Provider/Gemini.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Groq.py` & `webscout-2.3b0/webscout/Provider/Groq.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Koboldai.py` & `webscout-2.3b0/webscout/Provider/Koboldai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Leo.py` & `webscout-2.3b0/webscout/Provider/Leo.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Llama2.py` & `webscout-2.3b0/webscout/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/OpenGPT.py` & `webscout-2.3b0/webscout/Provider/OpenGPT.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Openai.py` & `webscout-2.3b0/webscout/Provider/Openai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Perplexity.py` & `webscout-2.3b0/webscout/Provider/Perplexity.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Phind.py` & `webscout-2.3b0/webscout/Provider/Phind.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Reka.py` & `webscout-2.3b0/webscout/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/ThinkAnyAI.py` & `webscout-2.3b0/webscout/Provider/ThinkAnyAI.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Xjai.py` & `webscout-2.3b0/webscout/Provider/Xjai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Yepchat.py` & `webscout-2.3b0/webscout/Provider/Yepchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/Youchat.py` & `webscout-2.3b0/webscout/Provider/Youchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/Provider/__init__.py` & `webscout-2.3b0/webscout/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/__init__.py` & `webscout-2.3b0/webscout/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from .webscout_search_async import AsyncWEBS
 from .version import __version__
 from .DWEBS import DeepWEBS
 from .transcriber import transcriber
 from .voice import play_audio
 from .tempid import Client as TempMailClient, TemporaryPhoneNumber
 from .LLM import LLM
-from .Local import *
+# Import Localai models and utilities directly
+from .Localai import *
 import g4f
 # Import provider classes for direct access
 from .Provider import (
    ThinkAnyAI,
    Xjai,
    LLAMA2, 
    AsyncLLAMA2,
```

### Comparing `webscout-2.3/webscout/async_providers.py` & `webscout-2.3b0/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/cli.py` & `webscout-2.3b0/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/g4f.py` & `webscout-2.3b0/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/models.py` & `webscout-2.3b0/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/tempid.py` & `webscout-2.3b0/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/transcriber.py` & `webscout-2.3b0/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/utils.py` & `webscout-2.3b0/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/voice.py` & `webscout-2.3b0/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/webai.py` & `webscout-2.3b0/webscout/webai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/webscout_search.py` & `webscout-2.3b0/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout/webscout_search_async.py` & `webscout-2.3b0/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3/webscout.egg-info/PKG-INFO` & `webscout-2.3b0/webscout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.3
+Version: 2.3b0
 Summary: Search for anything using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
```

#### html2text {}

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.3 Summary: Search for anything
-using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt
-videos, temporary email and phone number generation, has TTS support, and webai
-(terminal gpt and open interpreter). Author: OEvortex Author-email:
-helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
-Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
-github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
-youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: License :: Other/
-Proprietary License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Programming Language :: Python :: Implementation :: CPython Classifier: Topic
-:: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Description-Content-Type: text/
-markdown License-File: LICENSE.md Requires-Dist: docstring_inheritance
-Requires-Dist: click Requires-Dist: curl_cffi Requires-Dist: lxml Requires-
-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist: tqdm Requires-Dist:
-webdriver-manager Requires-Dist: halo>=0.0.31 Requires-Dist: g4f>=0.2.2.3
-Requires-Dist: rich Requires-Dist: python-dotenv Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify Requires-Dist: pydantic Requires-Dist: requests
-Requires-Dist: sse_starlette Requires-Dist: termcolor Requires-Dist: tiktoken
-Requires-Dist: tldextract Requires-Dist: orjson Requires-Dist: PyYAML Requires-
-Dist: appdirs Requires-Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client
-Requires-Dist: clipman Requires-Dist: playsound Provides-Extra: dev Requires-
-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
-Provides-Extra: local Requires-Dist: llama-cpp-python; extra == "local"
-Requires-Dist: colorama; extra == "local" Requires-Dist: numpy; extra ==
-"local"
+Metadata-Version: 2.1 Name: webscout Version: 2.3b0 Summary: Search for
+anything using Google, DuckDuckGo, phind.com. Also contains AI models, can
+transcribe yt videos, temporary email and phone number generation, has TTS
+support, and webai (terminal gpt and open interpreter). Author: OEvortex
+Author-email: helpingai5@gmail.com License: HelpingAI Simplified Universal
+License Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
+Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
+https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: License ::
+Other/Proprietary License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
+:: Software Development :: Libraries :: Python Modules Description-Content-
+Type: text/markdown License-File: LICENSE.md Requires-Dist:
+docstring_inheritance Requires-Dist: click Requires-Dist: curl_cffi Requires-
+Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
+tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
+Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
+Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
+Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
+Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
+Requires-Dist: PyYAML Requires-Dist: appdirs Requires-Dist: GoogleBard1>=2.1.4
+Requires-Dist: tls_client Requires-Dist: clipman Requires-Dist: playsound
+Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist:
+pytest>=7.4.2; extra == "dev" Provides-Extra: local Requires-Dist: llama-cpp-
+python; extra == "local" Requires-Dist: colorama; extra == "local" Requires-
+Dist: numpy; extra == "local"
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
 phind.com. Also containes AI models, can transcribe yt videos, temporary email
```

### Comparing `webscout-2.3/webscout.egg-info/SOURCES.txt` & `webscout-2.3b0/webscout.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -35,21 +35,14 @@
 webscout/webscout_search_async.py
 webscout.egg-info/PKG-INFO
 webscout.egg-info/SOURCES.txt
 webscout.egg-info/dependency_links.txt
 webscout.egg-info/entry_points.txt
 webscout.egg-info/requires.txt
 webscout.egg-info/top_level.txt
-webscout/Local/__init__.py
-webscout/Local/_version.py
-webscout/Local/formats.py
-webscout/Local/model.py
-webscout/Local/samplers.py
-webscout/Local/thread.py
-webscout/Local/utils.py
 webscout/Provider/Berlin4h.py
 webscout/Provider/Blackboxai.py
 webscout/Provider/ChatGPTUK.py
 webscout/Provider/Cohere.py
 webscout/Provider/Gemini.py
 webscout/Provider/Groq.py
 webscout/Provider/Koboldai.py
```

