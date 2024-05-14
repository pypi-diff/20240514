# Comparing `tmp/webscout-2.3b0.tar.gz` & `tmp/webscout-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-2.3b0.tar", last modified: Mon May 13 08:26:00 2024, max compression
+gzip compressed data, was "webscout-2.4.tar", last modified: Tue May 14 08:09:36 2024, max compression
```

## Comparing `webscout-2.3b0.tar` & `webscout-2.4.tar`

### file list

```diff
@@ -1,70 +1,78 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.429375 webscout-2.3b0/
-drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.019969 webscout-2.3b0/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.055985 webscout-2.3b0/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.089983 webscout-2.3b0/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.103987 webscout-2.3b0/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.3b0/LICENSE.md
--rw-rw-rw-   0        0        0    46603 2024-05-13 08:26:00.421374 webscout-2.3b0/PKG-INFO
--rw-rw-rw-   0        0        0    44185 2024-05-12 05:27:05.000000 webscout-2.3b0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 08:26:00.429375 webscout-2.3b0/setup.cfg
--rw-rw-rw-   0        0        0     2696 2024-05-13 08:03:16.000000 webscout-2.3b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.231150 webscout-2.3b0/webscout/
--rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.3b0/webscout/AIauto.py
--rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33266 2024-05-12 05:18:53.000000 webscout-2.3b0/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/LLM.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.387383 webscout-2.3b0/webscout/Provider/
--rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.3b0/webscout/Provider/Berlin4h.py
--rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.3b0/webscout/Provider/Blackboxai.py
--rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.3b0/webscout/Provider/ChatGPTUK.py
--rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.3b0/webscout/Provider/Cohere.py
--rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.3b0/webscout/Provider/Gemini.py
--rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.3b0/webscout/Provider/Groq.py
--rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.3b0/webscout/Provider/Koboldai.py
--rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.3b0/webscout/Provider/Leo.py
--rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.3b0/webscout/Provider/Llama2.py
--rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.3b0/webscout/Provider/OpenGPT.py
--rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.3b0/webscout/Provider/Openai.py
--rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.3b0/webscout/Provider/Perplexity.py
--rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.3b0/webscout/Provider/Phind.py
--rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.3b0/webscout/Provider/Reka.py
--rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.3b0/webscout/Provider/ThinkAnyAI.py
--rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.3b0/webscout/Provider/Xjai.py
--rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.3b0/webscout/Provider/Yepchat.py
--rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.3b0/webscout/Provider/Youchat.py
--rw-rw-rw-   0        0        0     1318 2024-05-12 05:15:53.000000 webscout-2.3b0/webscout/Provider/__init__.py
--rw-rw-rw-   0        0        0     2256 2024-05-13 08:07:51.000000 webscout-2.3b0/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/__main__.py
--rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.3b0/webscout/async_providers.py
--rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/cli.py
--rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.3b0/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.3b0/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.3b0/webscout/utils.py
--rw-rw-rw-   0        0        0       23 2024-05-11 09:00:53.000000 webscout-2.3b0/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/voice.py
--rw-rw-rw-   0        0        0    84668 2024-05-12 05:18:15.000000 webscout-2.3b0/webscout/webai.py
--rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-2.3b0/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-2.3b0/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.395371 webscout-2.3b0/webscout.egg-info/
--rw-rw-rw-   0        0        0    46603 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1592 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      366 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:36.593874 webscout-2.4/
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:34.441542 webscout-2.4/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.4/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:34.493543 webscout-2.4/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.4/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.4/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.4/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:34.578528 webscout-2.4/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.4/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.4/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.4/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.4/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.4/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:34.647523 webscout-2.4/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.4/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.4/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.4/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.4/LICENSE.md
+-rw-rw-rw-   0        0        0    46621 2024-05-14 08:09:36.585804 webscout-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    44186 2024-05-14 08:07:30.000000 webscout-2.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 08:09:36.594431 webscout-2.4/setup.cfg
+-rw-rw-rw-   0        0        0     2722 2024-05-14 08:06:21.000000 webscout-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:35.079857 webscout-2.4/webscout/
+-rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.4/webscout/AIauto.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.4/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33266 2024-05-12 05:18:53.000000 webscout-2.4/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.4/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.4/webscout/LLM.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:35.409845 webscout-2.4/webscout/Local/
+-rw-rw-rw-   0        0        0      217 2024-05-14 07:50:22.000000 webscout-2.4/webscout/Local/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-13 10:17:01.000000 webscout-2.4/webscout/Local/_version.py
+-rw-rw-rw-   0        0        0    17153 2024-05-13 10:22:12.000000 webscout-2.4/webscout/Local/formats.py
+-rw-rw-rw-   0        0        0    27611 2024-05-13 10:21:04.000000 webscout-2.4/webscout/Local/model.py
+-rw-rw-rw-   0        0        0     4372 2024-05-13 10:22:16.000000 webscout-2.4/webscout/Local/samplers.py
+-rw-rw-rw-   0        0        0    26786 2024-05-14 05:00:48.000000 webscout-2.4/webscout/Local/thread.py
+-rw-rw-rw-   0        0        0     6108 2024-05-14 05:14:09.000000 webscout-2.4/webscout/Local/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:36.553417 webscout-2.4/webscout/Provider/
+-rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.4/webscout/Provider/Berlin4h.py
+-rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.4/webscout/Provider/Blackboxai.py
+-rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.4/webscout/Provider/ChatGPTUK.py
+-rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.4/webscout/Provider/Cohere.py
+-rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.4/webscout/Provider/Gemini.py
+-rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.4/webscout/Provider/Groq.py
+-rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.4/webscout/Provider/Koboldai.py
+-rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.4/webscout/Provider/Leo.py
+-rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.4/webscout/Provider/Llama2.py
+-rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.4/webscout/Provider/OpenGPT.py
+-rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.4/webscout/Provider/Openai.py
+-rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.4/webscout/Provider/Perplexity.py
+-rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.4/webscout/Provider/Phind.py
+-rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.4/webscout/Provider/Reka.py
+-rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.4/webscout/Provider/ThinkAnyAI.py
+-rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.4/webscout/Provider/Xjai.py
+-rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.4/webscout/Provider/Yepchat.py
+-rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.4/webscout/Provider/Youchat.py
+-rw-rw-rw-   0        0        0     1318 2024-05-13 09:09:36.000000 webscout-2.4/webscout/Provider/__init__.py
+-rw-rw-rw-   0        0        0     2214 2024-05-14 03:52:34.000000 webscout-2.4/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.4/webscout/__main__.py
+-rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.4/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-2.4/webscout/cli.py
+-rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.4/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.4/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.4/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.4/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.4/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.4/webscout/utils.py
+-rw-rw-rw-   0        0        0       23 2024-05-11 09:00:53.000000 webscout-2.4/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.4/webscout/voice.py
+-rw-rw-rw-   0        0        0    84668 2024-05-12 05:18:15.000000 webscout-2.4/webscout/webai.py
+-rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-2.4/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-2.4/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:36.562417 webscout-2.4/webscout.egg-info/
+-rw-rw-rw-   0        0        0    46621 2024-05-14 08:09:32.000000 webscout-2.4/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1772 2024-05-14 08:09:33.000000 webscout-2.4/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:09:32.000000 webscout-2.4/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-14 08:09:32.000000 webscout-2.4/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      378 2024-05-14 08:09:32.000000 webscout-2.4/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-14 08:09:32.000000 webscout-2.4/webscout.egg-info/top_level.txt
```

### Comparing `webscout-2.3b0/DeepWEBS/documents/query_results_extractor.py` & `webscout-2.4/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-2.4/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/DeepWEBS/networks/filepath_converter.py` & `webscout-2.4/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/DeepWEBS/networks/google_searcher.py` & `webscout-2.4/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/DeepWEBS/networks/network_configs.py` & `webscout-2.4/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/DeepWEBS/networks/webpage_fetcher.py` & `webscout-2.4/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/DeepWEBS/utilsdw/enver.py` & `webscout-2.4/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/DeepWEBS/utilsdw/logger.py` & `webscout-2.4/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/LICENSE.md` & `webscout-2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/PKG-INFO` & `webscout-2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.3b0
-Summary: Search for anything using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).
+Version: 2.4
+Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex
@@ -46,29 +46,29 @@
 Requires-Dist: tldextract
 Requires-Dist: orjson
 Requires-Dist: PyYAML
 Requires-Dist: appdirs
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: tls_client
 Requires-Dist: clipman
-Requires-Dist: playsound
+Requires-Dist: Helpingai-T2playsound
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 Provides-Extra: local
 Requires-Dist: llama-cpp-python; extra == "local"
 Requires-Dist: colorama; extra == "local"
 Requires-Dist: numpy; extra == "local"
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
-  <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
+  <a href="https://buymeacoffee.com/oevortex"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://youtube.com/@OEvortex">&#10148; Vortex's YouTube Channel</a>
   </div>
 <div align="center">
@@ -83,15 +83,15 @@
 <p align="center">
 <div align="center">
   <img src="https://img.shields.io/badge/WebScout-API-blue?style=for-the-badge&logo=WebScout" alt="WebScout API Badge">
 </div>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
-Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
+Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 
 
 ## Table of Contents
 - [WEBSCOUT](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
@@ -1430,15 +1430,15 @@
 ```
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
-  <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
+  <a href="https://buymeacoffee.com/oevortex"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://youtube.com/@OEvortex">&#10148; Vortex's YouTube Channel</a>
   </div>
 <div align="center">
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.3b0 Summary: Search for
-anything using Google, DuckDuckGo, phind.com. Also contains AI models, can
-transcribe yt videos, temporary email and phone number generation, has TTS
-support, and webai (terminal gpt and open interpreter). Author: OEvortex
-Author-email: helpingai5@gmail.com License: HelpingAI Simplified Universal
-License Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Metadata-Version: 2.1 Name: webscout Version: 2.4 Summary: Search for anything
+using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
+videos, temporary email and phone number generation, has TTS support, webai
+(terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
+email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
+Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
 https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License ::
 Other/Proprietary License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -21,41 +21,41 @@
 Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
 Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
 Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
 Requires-Dist: PyYAML Requires-Dist: appdirs Requires-Dist: GoogleBard1>=2.1.4
-Requires-Dist: tls_client Requires-Dist: clipman Requires-Dist: playsound
-Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist:
-pytest>=7.4.2; extra == "dev" Provides-Extra: local Requires-Dist: llama-cpp-
-python; extra == "local" Requires-Dist: colorama; extra == "local" Requires-
-Dist: numpy; extra == "local"
+Requires-Dist: tls_client Requires-Dist: clipman Requires-Dist: Helpingai-
+T2playsound Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra == "dev"
+Requires-Dist: pytest>=7.4.2; extra == "dev" Provides-Extra: local Requires-
+Dist: llama-cpp-python; extra == "local" Requires-Dist: colorama; extra ==
+"local" Requires-Dist: numpy; extra == "local"
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
- _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
-phind.com. Also containes AI models, can transcribe yt videos, temporary email
- and phone number generation, have TTS support and webai(terminal gpt and open
-interpeter) ## Table of Contents - [WEBSCOUT](#webscout) - [Table of Contents]
-  (#table-of-contents) - [Install](#install) - [CLI version](#cli-version) -
-[Regions](#regions) - [Tempmail and Temp number](#tempmail-and-temp-number) -
-      [Temp number](#temp-number) - [Tempmail](#tempmail) - [Transcriber]
-  (#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
- searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point to remember
-  before using `DeepWEBS`](#point-to-remember-before-using-deepwebs) - [Usage
-Example](#usage-example) - [Text-to-Speech:](#text-to-speech) - [Available TTS
-    Voices:](#available-tts-voices) - [Exceptions](#exceptions) - [usage of
- webscout](#usage-of-webscout) - [1. `text()` - text search by DuckDuckGo.com
-and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom) - [2. `answers
-  ()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-
-    answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search by
-  DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
+   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using Google, DuckDuckGo,
+ phind.com, Contains AI models, can transcribe yt videos, temporary email and
+    phone number generation, has TTS support, webai (terminal gpt and open
+ interpreter) and offline LLMs ## Table of Contents - [WEBSCOUT](#webscout) -
+ [Table of Contents](#table-of-contents) - [Install](#install) - [CLI version]
+ (#cli-version) - [Regions](#regions) - [Tempmail and Temp number](#tempmail-
+   and-temp-number) - [Temp number](#temp-number) - [Tempmail](#tempmail) -
+  [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-
+ advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point
+to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
+   - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-speech) -
+ [Available TTS Voices:](#available-tts-voices) - [Exceptions](#exceptions) -
+    [usage of webscout](#usage-of-webscout) - [1. `text()` - text search by
+DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
+- [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers--
+ -instant-answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search
+ by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
  yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
   search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
  yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
 map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
 [7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
 translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
 DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
```

### Comparing `webscout-2.3b0/README.md` & `webscout-2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
-  <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
+  <a href="https://buymeacoffee.com/oevortex"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://youtube.com/@OEvortex">&#10148; Vortex's YouTube Channel</a>
   </div>
 <div align="center">
@@ -22,15 +22,15 @@
 <p align="center">
 <div align="center">
   <img src="https://img.shields.io/badge/WebScout-API-blue?style=for-the-badge&logo=WebScout" alt="WebScout API Badge">
 </div>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
-Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
+Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 
 
 ## Table of Contents
 - [WEBSCOUT](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
@@ -1369,15 +1369,15 @@
 ```
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
-  <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
+  <a href="https://buymeacoffee.com/oevortex"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://youtube.com/@OEvortex">&#10148; Vortex's YouTube Channel</a>
   </div>
 <div align="center">
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
- _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
-phind.com. Also containes AI models, can transcribe yt videos, temporary email
- and phone number generation, have TTS support and webai(terminal gpt and open
-interpeter) ## Table of Contents - [WEBSCOUT](#webscout) - [Table of Contents]
-  (#table-of-contents) - [Install](#install) - [CLI version](#cli-version) -
-[Regions](#regions) - [Tempmail and Temp number](#tempmail-and-temp-number) -
-      [Temp number](#temp-number) - [Tempmail](#tempmail) - [Transcriber]
-  (#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
- searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point to remember
-  before using `DeepWEBS`](#point-to-remember-before-using-deepwebs) - [Usage
-Example](#usage-example) - [Text-to-Speech:](#text-to-speech) - [Available TTS
-    Voices:](#available-tts-voices) - [Exceptions](#exceptions) - [usage of
- webscout](#usage-of-webscout) - [1. `text()` - text search by DuckDuckGo.com
-and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom) - [2. `answers
-  ()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-
-    answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search by
-  DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
+   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using Google, DuckDuckGo,
+ phind.com, Contains AI models, can transcribe yt videos, temporary email and
+    phone number generation, has TTS support, webai (terminal gpt and open
+ interpreter) and offline LLMs ## Table of Contents - [WEBSCOUT](#webscout) -
+ [Table of Contents](#table-of-contents) - [Install](#install) - [CLI version]
+ (#cli-version) - [Regions](#regions) - [Tempmail and Temp number](#tempmail-
+   and-temp-number) - [Temp number](#temp-number) - [Tempmail](#tempmail) -
+  [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-
+ advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point
+to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
+   - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-speech) -
+ [Available TTS Voices:](#available-tts-voices) - [Exceptions](#exceptions) -
+    [usage of webscout](#usage-of-webscout) - [1. `text()` - text search by
+DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
+- [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers--
+ -instant-answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search
+ by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
  yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
   search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
  yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
 map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
 [7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
 translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
 DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
```

### Comparing `webscout-2.3b0/setup.py` & `webscout-2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="2.3-beta",
-    description="Search for anything using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).",
+    version="2.4",
+    description="Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
@@ -50,14 +50,15 @@
         "tldextract",
         "orjson",
         "PyYAML",
         "appdirs",
         "GoogleBard1>=2.1.4",
         "tls_client",
         "clipman",
+        "Helpingai-T2"
         "playsound",
     ],
     entry_points={
         "console_scripts": [
             "WEBS = webscout.cli:cli",
             "webscout = webscout.webai:main",
         ],
```

### Comparing `webscout-2.3b0/webscout/AIauto.py` & `webscout-2.4/webscout/AIauto.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/AIbase.py` & `webscout-2.4/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/AIutel.py` & `webscout-2.4/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/DWEBS.py` & `webscout-2.4/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/LLM.py` & `webscout-2.4/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Berlin4h.py` & `webscout-2.4/webscout/Provider/Berlin4h.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Blackboxai.py` & `webscout-2.4/webscout/Provider/Blackboxai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/ChatGPTUK.py` & `webscout-2.4/webscout/Provider/ChatGPTUK.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Cohere.py` & `webscout-2.4/webscout/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Gemini.py` & `webscout-2.4/webscout/Provider/Gemini.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Groq.py` & `webscout-2.4/webscout/Provider/Groq.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Koboldai.py` & `webscout-2.4/webscout/Provider/Koboldai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Leo.py` & `webscout-2.4/webscout/Provider/Leo.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Llama2.py` & `webscout-2.4/webscout/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/OpenGPT.py` & `webscout-2.4/webscout/Provider/OpenGPT.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Openai.py` & `webscout-2.4/webscout/Provider/Openai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Perplexity.py` & `webscout-2.4/webscout/Provider/Perplexity.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Phind.py` & `webscout-2.4/webscout/Provider/Phind.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Reka.py` & `webscout-2.4/webscout/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/ThinkAnyAI.py` & `webscout-2.4/webscout/Provider/ThinkAnyAI.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Xjai.py` & `webscout-2.4/webscout/Provider/Xjai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Yepchat.py` & `webscout-2.4/webscout/Provider/Yepchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/Youchat.py` & `webscout-2.4/webscout/Provider/Youchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/Provider/__init__.py` & `webscout-2.4/webscout/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/__init__.py` & `webscout-2.4/webscout/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from .webscout_search_async import AsyncWEBS
 from .version import __version__
 from .DWEBS import DeepWEBS
 from .transcriber import transcriber
 from .voice import play_audio
 from .tempid import Client as TempMailClient, TemporaryPhoneNumber
 from .LLM import LLM
-# Import Localai models and utilities directly
-from .Localai import *
+# from .Local import *
 import g4f
 # Import provider classes for direct access
 from .Provider import (
    ThinkAnyAI,
    Xjai,
    LLAMA2, 
    AsyncLLAMA2,
@@ -78,17 +77,17 @@
    "DeepWEBS",
    "transcriber",
    "play_audio",
    "TempMailClient", 
    "TemporaryPhoneNumber",
    "LLM",
    # Localai models and utilities 
-   "Model",
-   "Thread",
-   "formats", 
+   # "Model",
+   # "Thread",
+   # "formats", 
 
    # AI Providers
    "ThinkAnyAI",
    "Xjai",
    "LLAMA2",
    "AsyncLLAMA2",
    "Cohere",
```

### Comparing `webscout-2.3b0/webscout/async_providers.py` & `webscout-2.4/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/cli.py` & `webscout-2.4/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/g4f.py` & `webscout-2.4/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/models.py` & `webscout-2.4/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/tempid.py` & `webscout-2.4/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/transcriber.py` & `webscout-2.4/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/utils.py` & `webscout-2.4/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/voice.py` & `webscout-2.4/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/webai.py` & `webscout-2.4/webscout/webai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/webscout_search.py` & `webscout-2.4/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout/webscout_search_async.py` & `webscout-2.4/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-2.3b0/webscout.egg-info/PKG-INFO` & `webscout-2.4/webscout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.3b0
-Summary: Search for anything using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).
+Version: 2.4
+Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex
@@ -46,29 +46,29 @@
 Requires-Dist: tldextract
 Requires-Dist: orjson
 Requires-Dist: PyYAML
 Requires-Dist: appdirs
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: tls_client
 Requires-Dist: clipman
-Requires-Dist: playsound
+Requires-Dist: Helpingai-T2playsound
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 Provides-Extra: local
 Requires-Dist: llama-cpp-python; extra == "local"
 Requires-Dist: colorama; extra == "local"
 Requires-Dist: numpy; extra == "local"
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
-  <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
+  <a href="https://buymeacoffee.com/oevortex"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://youtube.com/@OEvortex">&#10148; Vortex's YouTube Channel</a>
   </div>
 <div align="center">
@@ -83,15 +83,15 @@
 <p align="center">
 <div align="center">
   <img src="https://img.shields.io/badge/WebScout-API-blue?style=for-the-badge&logo=WebScout" alt="WebScout API Badge">
 </div>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
-Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
+Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 
 
 ## Table of Contents
 - [WEBSCOUT](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
@@ -1430,15 +1430,15 @@
 ```
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
-  <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
+  <a href="https://buymeacoffee.com/oevortex"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://youtube.com/@OEvortex">&#10148; Vortex's YouTube Channel</a>
   </div>
 <div align="center">
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.3b0 Summary: Search for
-anything using Google, DuckDuckGo, phind.com. Also contains AI models, can
-transcribe yt videos, temporary email and phone number generation, has TTS
-support, and webai (terminal gpt and open interpreter). Author: OEvortex
-Author-email: helpingai5@gmail.com License: HelpingAI Simplified Universal
-License Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Metadata-Version: 2.1 Name: webscout Version: 2.4 Summary: Search for anything
+using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
+videos, temporary email and phone number generation, has TTS support, webai
+(terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
+email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
+Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
 https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License ::
 Other/Proprietary License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -21,41 +21,41 @@
 Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
 Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
 Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
 Requires-Dist: PyYAML Requires-Dist: appdirs Requires-Dist: GoogleBard1>=2.1.4
-Requires-Dist: tls_client Requires-Dist: clipman Requires-Dist: playsound
-Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist:
-pytest>=7.4.2; extra == "dev" Provides-Extra: local Requires-Dist: llama-cpp-
-python; extra == "local" Requires-Dist: colorama; extra == "local" Requires-
-Dist: numpy; extra == "local"
+Requires-Dist: tls_client Requires-Dist: clipman Requires-Dist: Helpingai-
+T2playsound Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra == "dev"
+Requires-Dist: pytest>=7.4.2; extra == "dev" Provides-Extra: local Requires-
+Dist: llama-cpp-python; extra == "local" Requires-Dist: colorama; extra ==
+"local" Requires-Dist: numpy; extra == "local"
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
- _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
-phind.com. Also containes AI models, can transcribe yt videos, temporary email
- and phone number generation, have TTS support and webai(terminal gpt and open
-interpeter) ## Table of Contents - [WEBSCOUT](#webscout) - [Table of Contents]
-  (#table-of-contents) - [Install](#install) - [CLI version](#cli-version) -
-[Regions](#regions) - [Tempmail and Temp number](#tempmail-and-temp-number) -
-      [Temp number](#temp-number) - [Tempmail](#tempmail) - [Transcriber]
-  (#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
- searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point to remember
-  before using `DeepWEBS`](#point-to-remember-before-using-deepwebs) - [Usage
-Example](#usage-example) - [Text-to-Speech:](#text-to-speech) - [Available TTS
-    Voices:](#available-tts-voices) - [Exceptions](#exceptions) - [usage of
- webscout](#usage-of-webscout) - [1. `text()` - text search by DuckDuckGo.com
-and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom) - [2. `answers
-  ()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-
-    answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search by
-  DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
+   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using Google, DuckDuckGo,
+ phind.com, Contains AI models, can transcribe yt videos, temporary email and
+    phone number generation, has TTS support, webai (terminal gpt and open
+ interpreter) and offline LLMs ## Table of Contents - [WEBSCOUT](#webscout) -
+ [Table of Contents](#table-of-contents) - [Install](#install) - [CLI version]
+ (#cli-version) - [Regions](#regions) - [Tempmail and Temp number](#tempmail-
+   and-temp-number) - [Temp number](#temp-number) - [Tempmail](#tempmail) -
+  [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-
+ advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point
+to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
+   - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-speech) -
+ [Available TTS Voices:](#available-tts-voices) - [Exceptions](#exceptions) -
+    [usage of webscout](#usage-of-webscout) - [1. `text()` - text search by
+DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
+- [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers--
+ -instant-answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search
+ by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
  yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
   search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
  yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
 map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
 [7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
 translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
 DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
```

### Comparing `webscout-2.3b0/webscout.egg-info/SOURCES.txt` & `webscout-2.4/webscout.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -35,14 +35,21 @@
 webscout/webscout_search_async.py
 webscout.egg-info/PKG-INFO
 webscout.egg-info/SOURCES.txt
 webscout.egg-info/dependency_links.txt
 webscout.egg-info/entry_points.txt
 webscout.egg-info/requires.txt
 webscout.egg-info/top_level.txt
+webscout/Local/__init__.py
+webscout/Local/_version.py
+webscout/Local/formats.py
+webscout/Local/model.py
+webscout/Local/samplers.py
+webscout/Local/thread.py
+webscout/Local/utils.py
 webscout/Provider/Berlin4h.py
 webscout/Provider/Blackboxai.py
 webscout/Provider/ChatGPTUK.py
 webscout/Provider/Cohere.py
 webscout/Provider/Gemini.py
 webscout/Provider/Groq.py
 webscout/Provider/Koboldai.py
```

