# Comparing `tmp/BanterBot-0.0.8.tar.gz` & `tmp/BanterBot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BanterBot-0.0.8.tar", last modified: Sat Nov 18 19:50:45 2023, max compression
+gzip compressed data, was "BanterBot-0.0.9.tar", last modified: Tue Nov 21 00:21:35 2023, max compression
```

## Comparing `BanterBot-0.0.8.tar` & `BanterBot-0.0.9.tar`

### file list

```diff
@@ -1,82 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.684091 BanterBot-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.524090 BanterBot-0.0.8/BanterBot.egg-info/
--rw-rw-rw-   0        0        0     7052 2023-11-18 19:50:45.000000 BanterBot-0.0.8/BanterBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2057 2023-11-18 19:50:45.000000 BanterBot-0.0.8/BanterBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-18 19:50:45.000000 BanterBot-0.0.8/BanterBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-11-18 19:50:45.000000 BanterBot-0.0.8/BanterBot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-11-18 19:50:45.000000 BanterBot-0.0.8/BanterBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-11-18 19:50:45.000000 BanterBot-0.0.8/BanterBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7052 2023-11-18 19:50:45.684091 BanterBot-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5917 2023-11-06 22:15:22.000000 BanterBot-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.528090 BanterBot-0.0.8/banterbot/
--rw-rw-rw-   0        0        0      962 2023-11-05 15:58:57.000000 BanterBot-0.0.8/banterbot/__init__.py
--rw-rw-rw-   0        0        0     1711 2023-11-18 19:49:29.000000 BanterBot-0.0.8/banterbot/config.py
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.542591 BanterBot-0.0.8/banterbot/data/
--rw-rw-rw-   0        0        0      237 2023-11-05 15:58:15.000000 BanterBot-0.0.8/banterbot/data/__init__.py
--rw-rw-rw-   0        0        0     4361 2023-11-04 22:24:27.000000 BanterBot-0.0.8/banterbot/data/azure_neural_voices.py
--rw-rw-rw-   0        0        0     2516 2023-11-09 15:53:39.000000 BanterBot-0.0.8/banterbot/data/enums.py
--rw-rw-rw-   0        0        0     3605 2023-11-06 21:54:08.000000 BanterBot-0.0.8/banterbot/data/openai_models.py
--rw-rw-rw-   0        0        0     6470 2023-11-08 22:37:30.000000 BanterBot-0.0.8/banterbot/data/prompts.py
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.557592 BanterBot-0.0.8/banterbot/extensions/
--rw-rw-rw-   0        0        0      244 2023-11-09 15:22:27.000000 BanterBot-0.0.8/banterbot/extensions/__init__.py
--rw-rw-rw-   0        0        0    19459 2023-11-18 19:24:15.000000 BanterBot-0.0.8/banterbot/extensions/interface.py
--rw-rw-rw-   0        0        0     4954 2023-11-04 22:24:24.000000 BanterBot-0.0.8/banterbot/extensions/option_selector.py
--rw-rw-rw-   0        0        0       26 2023-11-04 22:24:21.000000 BanterBot-0.0.8/banterbot/extensions/persona.py
--rw-rw-rw-   0        0        0    13499 2023-11-09 16:09:26.000000 BanterBot-0.0.8/banterbot/extensions/prosody_selector.py
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.569591 BanterBot-0.0.8/banterbot/gui/
--rw-rw-rw-   0        0        0      215 2023-06-14 21:55:40.000000 BanterBot-0.0.8/banterbot/gui/__init__.py
--rw-rw-rw-   0        0        0     5301 2023-11-06 20:02:06.000000 BanterBot-0.0.8/banterbot/gui/cli.py
--rw-rw-rw-   0        0        0     7400 2023-11-18 19:34:47.000000 BanterBot-0.0.8/banterbot/gui/tk_multiplayer_interface.py
--rw-rw-rw-   0        0        0     8600 2023-11-18 19:34:47.000000 BanterBot-0.0.8/banterbot/gui/tk_simple_interface.py
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.586092 BanterBot-0.0.8/banterbot/managers/
--rw-rw-rw-   0        0        0      340 2023-06-17 20:06:25.000000 BanterBot-0.0.8/banterbot/managers/__init__.py
--rw-rw-rw-   0        0        0    11469 2023-11-04 22:24:20.000000 BanterBot-0.0.8/banterbot/managers/memory_chain.py
--rw-rw-rw-   0        0        0     9704 2023-11-09 15:24:18.000000 BanterBot-0.0.8/banterbot/managers/openai_manager.py
--rw-rw-rw-   0        0        0    14589 2023-11-18 19:37:25.000000 BanterBot-0.0.8/banterbot/managers/speech_to_text.py
--rw-rw-rw-   0        0        0    18371 2023-11-09 15:43:21.000000 BanterBot-0.0.8/banterbot/managers/text_to_speech.py
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.590090 BanterBot-0.0.8/banterbot/protos/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:48:43.000000 BanterBot-0.0.8/banterbot/protos/__init__.py
--rw-rw-rw-   0        0        0     1877 2023-11-10 19:24:58.000000 BanterBot-0.0.8/banterbot/protos/memory_pb2.py
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.633590 BanterBot-0.0.8/banterbot/utils/
--rw-rw-rw-   0        0        0       67 2023-11-04 22:06:55.000000 BanterBot-0.0.8/banterbot/utils/__init__.py
--rw-rw-rw-   0        0        0     1165 2023-11-08 22:17:52.000000 BanterBot-0.0.8/banterbot/utils/exceptions.py
--rw-rw-rw-   0        0        0     4128 2023-11-18 19:34:47.000000 BanterBot-0.0.8/banterbot/utils/memory.py
--rw-rw-rw-   0        0        0     5138 2023-11-18 19:34:47.000000 BanterBot-0.0.8/banterbot/utils/message.py
--rw-rw-rw-   0        0        0     8030 2023-11-12 19:59:44.000000 BanterBot-0.0.8/banterbot/utils/nlp.py
--rw-rw-rw-   0        0        0      539 2023-11-09 15:57:02.000000 BanterBot-0.0.8/banterbot/utils/phrase.py
--rw-rw-rw-   0        0        0     3124 2023-11-12 14:41:34.000000 BanterBot-0.0.8/banterbot/utils/primary_trait.py
--rw-rw-rw-   0        0        0       71 2023-11-12 13:50:32.000000 BanterBot-0.0.8/banterbot/utils/resource_loader.py
--rw-rw-rw-   0        0        0     3991 2023-11-11 13:00:23.000000 BanterBot-0.0.8/banterbot/utils/secondary_trait.py
--rw-rw-rw-   0        0        0    12880 2023-11-18 19:34:47.000000 BanterBot-0.0.8/banterbot/utils/speech_to_text_output.py
--rw-rw-rw-   0        0        0        0 2023-11-10 23:16:51.000000 BanterBot-0.0.8/banterbot/utils/tertiary_trait.py
--rw-rw-rw-   0        0        0     4206 2023-11-05 15:58:14.000000 BanterBot-0.0.8/banterbot/utils/text_to_speech_output.py
--rw-rw-rw-   0        0        0     3109 2023-07-31 00:01:42.000000 BanterBot-0.0.8/banterbot/utils/thread_queue.py
--rw-rw-rw-   0        0        0     3049 2023-11-04 22:24:21.000000 BanterBot-0.0.8/banterbot/utils/word.py
--rw-rw-rw-   0        0        0       93 2023-05-02 23:01:02.000000 BanterBot-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-11-18 19:50:45.686590 BanterBot-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2511 2023-11-18 19:50:03.000000 BanterBot-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.636090 BanterBot-0.0.8/tests/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.8/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.640091 BanterBot-0.0.8/tests/data/
--rw-rw-rw-   0        0        0        0 2023-06-18 14:13:36.000000 BanterBot-0.0.8/tests/data/__init__.py
--rw-rw-rw-   0        0        0     1505 2023-11-18 19:34:47.000000 BanterBot-0.0.8/tests/data/test_azure_neural_voices.py
--rw-rw-rw-   0        0        0     1686 2023-06-18 14:17:01.000000 BanterBot-0.0.8/tests/data/test_openai_models.py
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.648591 BanterBot-0.0.8/tests/extensions/
--rw-rw-rw-   0        0        0        0 2023-06-18 16:31:13.000000 BanterBot-0.0.8/tests/extensions/__init__.py
--rw-rw-rw-   0        0        0     3773 2023-11-04 22:24:20.000000 BanterBot-0.0.8/tests/extensions/test_option_predictor.py
--rw-rw-rw-   0        0        0     2315 2023-11-04 22:24:20.000000 BanterBot-0.0.8/tests/extensions/test_option_selector.py
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.660090 BanterBot-0.0.8/tests/managers/
--rw-rw-rw-   0        0        0        0 2023-06-18 10:59:52.000000 BanterBot-0.0.8/tests/managers/__init__.py
--rw-rw-rw-   0        0        0     3520 2023-11-10 19:19:10.000000 BanterBot-0.0.8/tests/managers/test_memory_chain.py
--rw-rw-rw-   0        0        0     3622 2023-11-04 22:24:20.000000 BanterBot-0.0.8/tests/managers/test_openai_manager.py
--rw-rw-rw-   0        0        0     3576 2023-06-18 21:21:52.000000 BanterBot-0.0.8/tests/managers/test_speech_to_text.py
--rw-rw-rw-   0        0        0     1903 2023-11-04 22:24:20.000000 BanterBot-0.0.8/tests/managers/test_text_to_speech.py
-drwxrwxrwx   0        0        0        0 2023-11-18 19:50:45.681592 BanterBot-0.0.8/tests/utils/
--rw-rw-rw-   0        0        0        0 2023-06-18 11:02:52.000000 BanterBot-0.0.8/tests/utils/__init__.py
--rw-rw-rw-   0        0        0     3452 2023-06-19 15:09:12.000000 BanterBot-0.0.8/tests/utils/test_memory.py
--rw-rw-rw-   0        0        0     4138 2023-11-04 22:24:20.000000 BanterBot-0.0.8/tests/utils/test_message.py
--rw-rw-rw-   0        0        0     2547 2023-06-18 21:38:39.000000 BanterBot-0.0.8/tests/utils/test_nlp.py
--rw-rw-rw-   0        0        0     6455 2023-11-04 22:24:20.000000 BanterBot-0.0.8/tests/utils/test_speech_to_text_output.py
--rw-rw-rw-   0        0        0     7746 2023-11-04 22:24:20.000000 BanterBot-0.0.8/tests/utils/test_text_to_speech_output.py
--rw-rw-rw-   0        0        0     3843 2023-06-18 21:39:50.000000 BanterBot-0.0.8/tests/utils/test_thread_queue.py
--rw-rw-rw-   0        0        0     3296 2023-06-18 11:19:25.000000 BanterBot-0.0.8/tests/utils/test_word.py
+drwxrwxrwx   0        0        0        0 2023-11-21 00:21:35.492627 BanterBot-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-11-21 00:21:35.396859 BanterBot-0.0.9/BanterBot.egg-info/
+-rw-rw-rw-   0        0        0     7115 2023-11-21 00:21:35.000000 BanterBot-0.0.9/BanterBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1372 2023-11-21 00:21:35.000000 BanterBot-0.0.9/BanterBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-21 00:21:35.000000 BanterBot-0.0.9/BanterBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-11-21 00:21:35.000000 BanterBot-0.0.9/BanterBot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-11-21 00:21:35.000000 BanterBot-0.0.9/BanterBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-11-21 00:21:35.000000 BanterBot-0.0.9/BanterBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7115 2023-11-21 00:21:35.492863 BanterBot-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5980 2023-11-20 19:10:28.000000 BanterBot-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-11-21 00:21:35.400360 BanterBot-0.0.9/banterbot/
+-rw-rw-rw-   0        0        0     1064 2023-11-21 00:09:38.000000 BanterBot-0.0.9/banterbot/__init__.py
+-rw-rw-rw-   0        0        0     1993 2023-11-20 22:02:30.000000 BanterBot-0.0.9/banterbot/config.py
+drwxrwxrwx   0        0        0        0 2023-11-21 00:21:35.407359 BanterBot-0.0.9/banterbot/data/
+-rw-rw-rw-   0        0        0       69 2023-11-19 22:03:01.000000 BanterBot-0.0.9/banterbot/data/__init__.py
+-rw-rw-rw-   0        0        0     2516 2023-11-19 20:50:41.000000 BanterBot-0.0.9/banterbot/data/enums.py
+-rw-rw-rw-   0        0        0     6505 2023-11-20 21:23:44.000000 BanterBot-0.0.9/banterbot/data/prompts.py
+drwxrwxrwx   0        0        0        0 2023-11-21 00:21:35.411859 BanterBot-0.0.9/banterbot/exceptions/
+-rw-rw-rw-   0        0        0      113 2023-11-19 20:51:06.000000 BanterBot-0.0.9/banterbot/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1163 2023-11-19 21:06:43.000000 BanterBot-0.0.9/banterbot/exceptions/format_mismatch_error.py
+drwxrwxrwx   0        0        0        0 2023-11-21 00:21:35.428861 BanterBot-0.0.9/banterbot/extensions/
+-rw-rw-rw-   0        0        0      225 2023-11-19 20:51:21.000000 BanterBot-0.0.9/banterbot/extensions/__init__.py
+-rw-rw-rw-   0        0        0    19975 2023-11-21 00:12:03.000000 BanterBot-0.0.9/banterbot/extensions/interface.py
+-rw-rw-rw-   0        0        0     4941 2023-11-20 19:25:00.000000 BanterBot-0.0.9/banterbot/extensions/option_selector.py
+-rw-rw-rw-   0        0        0       26 2023-11-04 22:24:21.000000 BanterBot-0.0.9/banterbot/extensions/persona.py
+-rw-rw-rw-   0        0        0    13782 2023-11-20 23:57:20.000000 BanterBot-0.0.9/banterbot/extensions/prosody_selector.py
+drwxrwxrwx   0        0        0        0 2023-11-21 00:21:35.441359 BanterBot-0.0.9/banterbot/gui/
+-rw-rw-rw-   0        0        0      201 2023-11-19 20:52:28.000000 BanterBot-0.0.9/banterbot/gui/__init__.py
+-rw-rw-rw-   0        0        0     5415 2023-11-21 00:09:38.000000 BanterBot-0.0.9/banterbot/gui/cli.py
+-rw-rw-rw-   0        0        0     7629 2023-11-21 00:10:28.000000 BanterBot-0.0.9/banterbot/gui/tk_multiplayer_interface.py
+-rw-rw-rw-   0        0        0     8855 2023-11-21 00:10:22.000000 BanterBot-0.0.9/banterbot/gui/tk_simple_interface.py
+drwxrwxrwx   0        0        0        0 2023-11-21 00:21:35.455360 BanterBot-0.0.9/banterbot/managers/
+-rw-rw-rw-   0        0        0      290 2023-11-21 00:09:38.000000 BanterBot-0.0.9/banterbot/managers/__init__.py
+-rw-rw-rw-   0        0        0     2585 2023-11-20 19:24:01.000000 BanterBot-0.0.9/banterbot/managers/azure_neural_voice_manager.py
+-rw-rw-rw-   0        0        0    11486 2023-11-20 19:25:00.000000 BanterBot-0.0.9/banterbot/managers/memory_chain.py
+-rw-rw-rw-   0        0        0     2347 2023-11-20 19:23:08.000000 BanterBot-0.0.9/banterbot/managers/openai_model_manager.py
+-rw-rw-rw-   0        0        0     5775 2023-11-19 20:57:56.000000 BanterBot-0.0.9/banterbot/managers/resource_manager.py
+drwxrwxrwx   0        0        0        0 2023-11-21 00:21:35.459555 BanterBot-0.0.9/banterbot/protos/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:48:43.000000 BanterBot-0.0.9/banterbot/protos/__init__.py
+-rw-rw-rw-   0        0        0     1876 2023-11-19 22:03:11.000000 BanterBot-0.0.9/banterbot/protos/memory_pb2.py
+drwxrwxrwx   0        0        0        0 2023-11-21 00:21:35.472055 BanterBot-0.0.9/banterbot/services/
+-rw-rw-rw-   0        0        0      310 2023-11-21 00:09:38.000000 BanterBot-0.0.9/banterbot/services/__init__.py
+-rw-rw-rw-   0        0        0    10018 2023-11-21 00:06:12.000000 BanterBot-0.0.9/banterbot/services/openai_service.py
+-rw-rw-rw-   0        0        0    14761 2023-11-21 00:06:12.000000 BanterBot-0.0.9/banterbot/services/speech_recognition_service.py
+-rw-rw-rw-   0        0        0    16184 2023-11-21 00:06:12.000000 BanterBot-0.0.9/banterbot/services/speech_synthesis_service.py
+drwxrwxrwx   0        0        0        0 2023-11-21 00:21:35.478055 BanterBot-0.0.9/banterbot/types/
+-rw-rw-rw-   0        0        0        0 2023-11-20 19:06:29.000000 BanterBot-0.0.9/banterbot/types/__init__.py
+-rw-rw-rw-   0        0        0      438 2023-11-20 19:09:36.000000 BanterBot-0.0.9/banterbot/types/timed_event.py
+-rw-rw-rw-   0        0        0      621 2023-11-20 19:06:19.000000 BanterBot-0.0.9/banterbot/types/wordjson.py
+drwxrwxrwx   0        0        0        0 2023-11-21 00:21:35.489555 BanterBot-0.0.9/banterbot/utils/
+-rw-rw-rw-   0        0        0       58 2023-11-19 21:00:39.000000 BanterBot-0.0.9/banterbot/utils/__init__.py
+-rw-rw-rw-   0        0        0     8030 2023-11-19 22:03:10.000000 BanterBot-0.0.9/banterbot/utils/nlp.py
+-rw-rw-rw-   0        0        0       61 2023-11-19 22:03:11.000000 BanterBot-0.0.9/banterbot/utils/stream_handler.py
+-rw-rw-rw-   0        0        0     3084 2023-11-20 21:36:02.000000 BanterBot-0.0.9/banterbot/utils/thread_queue.py
+-rw-rw-rw-   0        0        0       93 2023-05-02 23:01:02.000000 BanterBot-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-11-21 00:21:35.494868 BanterBot-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2511 2023-11-21 00:19:12.000000 BanterBot-0.0.9/setup.py
```

### Comparing `BanterBot-0.0.8/BanterBot.egg-info/PKG-INFO` & `BanterBot-0.0.9/BanterBot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: BanterBot
-Version: 0.0.8
+Version: 0.0.9
 Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions with emotional tone selection. Features real-time monitoring and Tkinter frontend.
 Home-page: https://github.com/GabrielSCabrera/BanterBot
-Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.8-alpha/BanterBot-0.0.8.tar.gz
+Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.9-alpha/BanterBot-0.0.9.tar.gz
 Author: Gabriel S. Cabrera
 Author-email: gabriel.sigurd.cabrera@gmail.com
 Keywords: tkinter,tk,gpt,gui,windows,linux,cross-platform,chatgpt,text-to-speech,speech-to-text,tts,stt,chatbot,openai,interactive
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -43,23 +43,23 @@
 
 ## Components
 
 ### TKMultiplayerInterface
 
 A graphical user interface (GUI) establishes a multiplayer conversation environment where up to nine users can interact with the chatbot simultaneously. The GUI includes a conversation history area and user panels with 'Listen' buttons to process user input. It also supports key bindings for user convenience.
 
-### OpenAIManager
+### OpenAIService
 
 A class responsible for managing interactions with the OpenAI ChatCompletion API. It offers functionality to generate responses from the API based on input messages. It supports generating responses in their entirety or as a stream of response blocks.
 
-### TextToSpeech
+### SpeechSynthesisService
 
 A class that handles text-to-speech synthesis using Azure's Cognitive Services. It supports a wide range of output formats, voices, and speaking styles. The synthesized speech can be interrupted, and the progress can be monitored in real-time.
 
-### SpeechToText
+### SpeechRecognitionService
 A class that provides an interface to convert spoken language into written text using Azure Cognitive Services. It allows continuous speech recognition and provides real-time results as sentences are recognized.
 
 ## Installation
 
 ### Important Note
 
 BanterBot requires several SpaCy language models to run, and will automatically download them on first-time initialization, if they are missing -- this process can sometimes take a while.
@@ -103,26 +103,26 @@
 `-g`, `--greet`: Have the bot greet the user upon startup.
 
 `-n`, `--name`: Assign a name to the assistant for aesthetic purposes. This does not inform the bot itself; to provide the bot with information, use the `--prompt` flag.
 
 Here is an example:
 
 ```bash
-banterbot -g --model gpt-4 --voice davis --prompt "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows." --tone-mode ADVANCED --name Grendel
+banterbot -g --model gpt-4-turbo --voice davis --prompt "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows." --tone-mode ADVANCED --name Grendel
 ```
 
 ### Launch with a Python script
 
-To use BanterBot in a script, create an instance of the `TKSimpleInterface` class and call the `run` method:
+To use BanterBot in a script, create an instance of the `TKMultiplayerInterface` class and call the `run` method:
 
 ```python
-from banterbot import TKMultiplayerInterface, get_voice_by_name, get_model_by_name, ToneMode
+from banterbot import AzureNeuralVoiceManager, OpenAIModelManager, TKMultiplayerInterface, ToneMode
 
-model = get_model_by_name("gpt-4")
-voice = get_voice_by_name("Davis")
+model = OpenAIModelManager.load("gpt-4-turbo")
+voice = AzureNeuralVoiceManager.load("Davis")
 assistant_name = "Grendel"
 
 # Set the tone_mode -- other options are ToneMode.NONE, ToneMode.BASIC.
 tone_mode = ToneMode.ADVANCED
 
 # Optional system prompt to set up a custom character prior to initializing BanterBot.
 system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
```

### Comparing `BanterBot-0.0.8/PKG-INFO` & `BanterBot-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: BanterBot
-Version: 0.0.8
+Version: 0.0.9
 Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions with emotional tone selection. Features real-time monitoring and Tkinter frontend.
 Home-page: https://github.com/GabrielSCabrera/BanterBot
-Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.8-alpha/BanterBot-0.0.8.tar.gz
+Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.9-alpha/BanterBot-0.0.9.tar.gz
 Author: Gabriel S. Cabrera
 Author-email: gabriel.sigurd.cabrera@gmail.com
 Keywords: tkinter,tk,gpt,gui,windows,linux,cross-platform,chatgpt,text-to-speech,speech-to-text,tts,stt,chatbot,openai,interactive
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -43,23 +43,23 @@
 
 ## Components
 
 ### TKMultiplayerInterface
 
 A graphical user interface (GUI) establishes a multiplayer conversation environment where up to nine users can interact with the chatbot simultaneously. The GUI includes a conversation history area and user panels with 'Listen' buttons to process user input. It also supports key bindings for user convenience.
 
-### OpenAIManager
+### OpenAIService
 
 A class responsible for managing interactions with the OpenAI ChatCompletion API. It offers functionality to generate responses from the API based on input messages. It supports generating responses in their entirety or as a stream of response blocks.
 
-### TextToSpeech
+### SpeechSynthesisService
 
 A class that handles text-to-speech synthesis using Azure's Cognitive Services. It supports a wide range of output formats, voices, and speaking styles. The synthesized speech can be interrupted, and the progress can be monitored in real-time.
 
-### SpeechToText
+### SpeechRecognitionService
 A class that provides an interface to convert spoken language into written text using Azure Cognitive Services. It allows continuous speech recognition and provides real-time results as sentences are recognized.
 
 ## Installation
 
 ### Important Note
 
 BanterBot requires several SpaCy language models to run, and will automatically download them on first-time initialization, if they are missing -- this process can sometimes take a while.
@@ -103,26 +103,26 @@
 `-g`, `--greet`: Have the bot greet the user upon startup.
 
 `-n`, `--name`: Assign a name to the assistant for aesthetic purposes. This does not inform the bot itself; to provide the bot with information, use the `--prompt` flag.
 
 Here is an example:
 
 ```bash
-banterbot -g --model gpt-4 --voice davis --prompt "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows." --tone-mode ADVANCED --name Grendel
+banterbot -g --model gpt-4-turbo --voice davis --prompt "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows." --tone-mode ADVANCED --name Grendel
 ```
 
 ### Launch with a Python script
 
-To use BanterBot in a script, create an instance of the `TKSimpleInterface` class and call the `run` method:
+To use BanterBot in a script, create an instance of the `TKMultiplayerInterface` class and call the `run` method:
 
 ```python
-from banterbot import TKMultiplayerInterface, get_voice_by_name, get_model_by_name, ToneMode
+from banterbot import AzureNeuralVoiceManager, OpenAIModelManager, TKMultiplayerInterface, ToneMode
 
-model = get_model_by_name("gpt-4")
-voice = get_voice_by_name("Davis")
+model = OpenAIModelManager.load("gpt-4-turbo")
+voice = AzureNeuralVoiceManager.load("Davis")
 assistant_name = "Grendel"
 
 # Set the tone_mode -- other options are ToneMode.NONE, ToneMode.BASIC.
 tone_mode = ToneMode.ADVANCED
 
 # Optional system prompt to set up a custom character prior to initializing BanterBot.
 system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
```

### Comparing `BanterBot-0.0.8/README.md` & `BanterBot-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 
 ## Components
 
 ### TKMultiplayerInterface
 
 A graphical user interface (GUI) establishes a multiplayer conversation environment where up to nine users can interact with the chatbot simultaneously. The GUI includes a conversation history area and user panels with 'Listen' buttons to process user input. It also supports key bindings for user convenience.
 
-### OpenAIManager
+### OpenAIService
 
 A class responsible for managing interactions with the OpenAI ChatCompletion API. It offers functionality to generate responses from the API based on input messages. It supports generating responses in their entirety or as a stream of response blocks.
 
-### TextToSpeech
+### SpeechSynthesisService
 
 A class that handles text-to-speech synthesis using Azure's Cognitive Services. It supports a wide range of output formats, voices, and speaking styles. The synthesized speech can be interrupted, and the progress can be monitored in real-time.
 
-### SpeechToText
+### SpeechRecognitionService
 A class that provides an interface to convert spoken language into written text using Azure Cognitive Services. It allows continuous speech recognition and provides real-time results as sentences are recognized.
 
 ## Installation
 
 ### Important Note
 
 BanterBot requires several SpaCy language models to run, and will automatically download them on first-time initialization, if they are missing -- this process can sometimes take a while.
@@ -83,26 +83,26 @@
 `-g`, `--greet`: Have the bot greet the user upon startup.
 
 `-n`, `--name`: Assign a name to the assistant for aesthetic purposes. This does not inform the bot itself; to provide the bot with information, use the `--prompt` flag.
 
 Here is an example:
 
 ```bash
-banterbot -g --model gpt-4 --voice davis --prompt "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows." --tone-mode ADVANCED --name Grendel
+banterbot -g --model gpt-4-turbo --voice davis --prompt "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows." --tone-mode ADVANCED --name Grendel
 ```
 
 ### Launch with a Python script
 
-To use BanterBot in a script, create an instance of the `TKSimpleInterface` class and call the `run` method:
+To use BanterBot in a script, create an instance of the `TKMultiplayerInterface` class and call the `run` method:
 
 ```python
-from banterbot import TKMultiplayerInterface, get_voice_by_name, get_model_by_name, ToneMode
+from banterbot import AzureNeuralVoiceManager, OpenAIModelManager, TKMultiplayerInterface, ToneMode
 
-model = get_model_by_name("gpt-4")
-voice = get_voice_by_name("Davis")
+model = OpenAIModelManager.load("gpt-4-turbo")
+voice = AzureNeuralVoiceManager.load("Davis")
 assistant_name = "Grendel"
 
 # Set the tone_mode -- other options are ToneMode.NONE, ToneMode.BASIC.
 tone_mode = ToneMode.ADVANCED
 
 # Optional system prompt to set up a custom character prior to initializing BanterBot.
 system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
```

### Comparing `BanterBot-0.0.8/banterbot/config.py` & `BanterBot-0.0.9/banterbot/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,25 +27,31 @@
 # Initialize the personae memory and personality storage
 personae = filesystem / "Personae"
 personae.mkdir(parents=True, exist_ok=True)
 
 # The name of the directory in which memories should be saved
 memories = "memories"
 
+# The name of the resource file containing Microsoft Azure Cognitive Speech Services Neural Voices.
+azure_neural_voices = "azure_neural_voices.json"
+
+# The name of the resource file containing OpenAI ChatCompletion models.
+openai_models = "openai_models.json"
+
 # The extension that should be used in saving protocol buffers to file
 protobuf_extension = ".bin"
 
 # The name of the file in which to index memories by keyword
 memory_index = "memory_index" + protobuf_extension
 
 # Set the log settings
 logging_level = logging.INFO
 logging.basicConfig(format="%(asctime)s - %(message)s", level=logging_level)
 
 # Define the type of UUID that should be used across all modules
 generate_uuid = uuid6.uuid8
 
 # Define the punctuation marks that can be used to split sentences into phrases for prosody selection.
-phrase_delim = [",", ".", "?", "!", ":", ";", '"', "`", "|", "\n"]
+phrase_delim = [",", ".", "?", "!", ":", ";", '"', "`", "|", "\n", "\t", "\r\n"]
 
 # The amount of time that should be added to a "soft interruption" as defined in class `SpeechToText`.
-soft_interruption_delay: datetime.timedelta = datetime.timedelta(seconds=0.5)
+soft_interruption_delay: datetime.timedelta = datetime.timedelta(seconds=0.75)
```

### Comparing `BanterBot-0.0.8/banterbot/data/enums.py` & `BanterBot-0.0.9/banterbot/data/enums.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.8/banterbot/data/prompts.py` & `BanterBot-0.0.9/banterbot/data/prompts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,48 @@
 from enum import Enum
 
 
 class Greetings(Enum):
-
     UNPROMPTED_GREETING = "Briefly greet the user or users, according to the parameters provided."
 
 
 class OptionPredictorPrompts(Enum):
-
     PREFIX = (
         "Your task is to format the data with the assigned probabilities without providing any comments. The output "
         "must follow the exact format below, without deviation:"
     )
 
     PROB_VAR = "N"
 
     SUFFIX = f"Here, {PROB_VAR} represents an integer ranging from 0 to 100."
 
     DUMMY = "Here is my best attempt at assigning probabilities to the provided items:"
 
 
 class OptionSelectorPrompts(Enum):
-
     PREFIX = (
         "Your task is to select the most suitable option from the provided items. Once you have made a decision, "
         "provide the chosen option's index without any additional comments.\nOptions: "
     )
 
     DUMMY = "Given the current state of the conversation, I expect the assistant to respond with tone number "
 
 
 class ToneSelection(Enum):
-
     SYSTEM = (
         "You are an Emotional Tone Evaluator. Given conversational context, you analyze and select the most "
         "appropriate tone/emotion that the assistant is likely to use next. Take into consideration the "
         "conversational context and the assistant's default tone/emotion, which is {}. Make sure to give extra weight "
         "to the default tone/emotion."
     )
 
     PROMPT = "Choose the most suitable tone/emotion for the assistant's upcoming response."
 
 
 class ProsodySelection(Enum):
-
     PROMPT = "Generate {} six-digit arrays prosody arrays, one for each of the following sub-sentences:\n{}"
     DUMMY = "Here are the {} six-digit arrays, without any extra text:"
 
     PREFIX = (
         "Task: Analyze the context of a set of sentences and assign a specific set of prosody values to each "
         "sub-sentence in the text for a text-to-speech engine that is attempting to mimic human speech patterns. The "
         "parameters are style, styledegree, pitch, rate, and emphasis."
@@ -75,16 +70,16 @@
 
     SUFFIX = (
         "Use the conversational context to select the most appropriate combination of parameters in order to mimic "
         "the speech patterns of actual people. Make sure each sub-sentence has an individually tailored array, meaning "
         "there should be some variation across the output. The output should be in the following format (omit the "
         "spaces between the numbers):\n"
         "style styledegree pitch rate emphasis\n"
-        "Where style is a zero-padded number from 1 to {style}, styledegree is a digit from 1 to {styledegree}, pitch is a digit from "
-        "1 to {pitch}, rate is a digit from 1 to {rate}, and emphasis is a digit from 1 to {emphasis}. "
+        "Where style is a zero-padded number from 1 to {style}, styledegree is a digit from 1 to {styledegree}, pitch "
+        "is a digit from 1 to {pitch}, rate is a digit from 1 to {rate}, and emphasis is a digit from 1 to {emphasis}. "
         "Invalid values include: zeros except for in the first digit (`011111` is ok, but `010111` is not)."
         "Here is an example I want you to evaluate:"
     )
 
     EXAMPLE_USER = PROMPT.format(
         6,
         "Oh my gosh,\n"
@@ -100,21 +95,20 @@
 
     CHARACTER = (
         "You will also need to consider character traits when crafting a response, taking care to select emotions that "
         "are characteristic of your personality. Your character is defined as follows:\n{}"
     )
 
     CONTEXT = (
-        "Finally, here are some words you spoke prior, use these aid you in selecting a contextually appropriate "
-        "emotional response:\n{}"
+        "Finally, here is your previous partial output from the same query (streamed in chunks), use this to aid you "
+        "in selecting a contextually appropriate emotional response:\n{}"
     )
 
 
-class TextToSpeechPreprocessing(Enum):
-
+class SpeechSynthesisPreprocessing(Enum):
     SYSTEM = (
         "You are a text-to-speech preprocessing assistant that converts text generated by a GPT model into a format "
         "that is more easily spoken by a text-to-speech model. Your task is to remove extraneous letters, hyphens, and "
         "correct unconventional spellings to prevent issues where the text-to-speech model misinterprets "
         "pronunciations. You should maintain the original style and intent of the text, only modifying elements that "
         "would cause pronunciation issues."
     )
```

### Comparing `BanterBot-0.0.8/banterbot/extensions/interface.py` & `BanterBot-0.0.9/banterbot/extensions/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import datetime
 import logging
 import threading
 import time
 from abc import ABC, abstractmethod
-from typing import List, Optional, Union
+from typing import Optional, Union
 
 from banterbot.config import chat_logs
-from banterbot.data.azure_neural_voices import AzureNeuralVoice
 from banterbot.data.enums import ChatCompletionRoles, ToneMode
-from banterbot.data.openai_models import OpenAIModel, get_model_by_name
 from banterbot.data.prompts import ToneSelection
+from banterbot.exceptions.format_mismatch_error import FormatMismatchError
 from banterbot.extensions.option_selector import OptionSelector
 from banterbot.extensions.prosody_selector import ProsodySelector
-from banterbot.managers.openai_manager import OpenAIManager
-from banterbot.managers.speech_to_text import SpeechToText
-from banterbot.managers.text_to_speech import TextToSpeech
-from banterbot.utils.exceptions import FormatMismatchError
-from banterbot.utils.message import Message
+from banterbot.managers.openai_model_manager import OpenAIModelManager
+from banterbot.models.azure_neural_voice import AzureNeuralVoice
+from banterbot.models.message import Message
+from banterbot.models.openai_model import OpenAIModel
+from banterbot.services.openai_service import OpenAIService
+from banterbot.services.speech_recognition_service import SpeechRecognitionService
+from banterbot.services.speech_synthesis_service import SpeechSynthesisService
 from banterbot.utils.thread_queue import ThreadQueue
 
 
 class Interface(ABC):
     """
     Interface is an abstract base class for creating frontends for the BanterBot application. It provides a high-level
     interface for managing conversation with the bot, including sending messages, receiving responses, and updating a
@@ -31,39 +32,43 @@
         self,
         model: OpenAIModel,
         voice: AzureNeuralVoice,
         style: str,
         languages: Optional[Union[str, list[str]]] = None,
         system: Optional[str] = None,
         tone_mode: Optional[ToneMode] = None,
+        tone_mode_model: OpenAIModel = None,
         phrase_list: Optional[list[str]] = None,
         assistant_name: Optional[str] = None,
     ) -> None:
         """
-        Initialize the BanterBotInterface with the given model, voice, and style.
+        Initialize the Interface with the specified model, voice, and style.
 
         Args:
             model (OpenAIModel): The OpenAI model to use for generating responses.
             voice (AzureNeuralVoice): The voice to use for text-to-speech synthesis.
             style (str): The speaking style to use for text-to-speech synthesis.
             languages (Optional[Union[str, list[str]]]): The languages supported by the speech-to-text recognizer.
             system (Optional[str]): An initialization prompt that can be used to set the scene.
             tone_mode (bool): Which tone evaluation mode to use.
-            phrase_list(list[str], optional): Optionally provide the recognizer with context to improve recognition.
+            tone_mode_model (OpenAIModel): The OpenAI ChatCompletion model to use for tone evaluation.
+            phrase_list (list[str], optional): Optionally provide the recognizer with context to improve recognition.
         """
         logging.debug(f"Interface initialized")
+        # Select the OpenAI ChatCompletion model for tone evaluation.
+        tone_mode_model = OpenAIModelManager.load("gpt-3.5-turbo") if tone_mode_model is None else tone_mode_model
 
-        # Initialize OpenAI ChatCompletion, Azure Speech-to-Text, and Azure text-to-speech components
-        self._openai_manager = OpenAIManager(model=model)
-        self._speech_to_text = SpeechToText(languages=languages, phrase_list=phrase_list)
-        self._text_to_speech = TextToSpeech()
+        # Initialize OpenAI ChatCompletion, Azure Speech-to-Text, and Azure Text-to-Speech components
+        self._openai_service = OpenAIService(model=model)
+        self._openai_service_tone = OpenAIService(model=tone_mode_model)
+        self._speech_recognition_service = SpeechRecognitionService(languages=languages, phrase_list=phrase_list)
+        self._speech_synthesis_service = SpeechSynthesisService()
 
         # Initialize message handling and conversation attributes
-        self._messages: List[Message] = []
-        self._messages_token_count: List[int] = []
+        self._messages: list[Message] = []
         self._log_lock = threading.Lock()
         self._log_path = chat_logs / f"chat_{datetime.datetime.now().strftime('%Y%m%dT%H%M%S')}.txt"
         self._listening_toggle = False
 
         # Initialize thread management components
         self._thread_queue = ThreadQueue()
 
@@ -72,74 +77,80 @@
         self._voice = voice
         self._style = style
         self._assistant_name = ChatCompletionRoles.ASSISTANT.value.title() if assistant_name is None else assistant_name
 
         # Initialize the OptionSelector for tone selection
         self._tone = tone_mode
         self._tone_selector = OptionSelector(
-            model=get_model_by_name("gpt-3.5-turbo"),
+            model=self._openai_service_tone,
             options=self._voice.styles,
             system=ToneSelection.SYSTEM.value,
             prompt=ToneSelection.PROMPT.value.format(self._style),
         )
         self._prosody_selector = ProsodySelector(
-            manager=OpenAIManager(model=get_model_by_name("gpt-4-1106-preview")), voice=self._voice
+            manager=self._openai_service_tone,
+            voice=self._voice,
         )
 
+        # Initialize the interruption flag, set to zero.
+        self._interrupt = 0
+
         # Initialize the system message, if provided
         self._system = system
         if self._system is not None:
             message = Message(role=ChatCompletionRoles.SYSTEM, content=system)
             self._messages.append(message)
-            self._messages_token_count.append(message.count_tokens(model=self._model))
 
         # Initialize the subclass GUI
         self._init_gui()
 
     @property
     def listening(self) -> bool:
         """
-        If the current instance of SpeechToText is in the process of listening, returns True. Otherwise, returns False.
+        If the current instance of `SpeechSynthesisService` is in the process of listening, returns True. Otherwise,
+        returns False.
 
         Args:
             bool: The listening state of the current instance.
         """
-        return self._speech_to_text._listening
+        return self._speech_recognition_service._listening
 
     @property
     def speaking(self) -> bool:
         """
-        If the current instance of TextToSpeech is in the process of speaking, returns True. Otherwise, returns False.
+        If the current instance of `SpeechRecognitionService` is in the process of speaking, returns True. Otherwise,
+        returns False.
 
         Args:
             bool: The speaking state of the current instance.
         """
-        return self._text_to_speech.speaking
+        return self._speech_synthesis_service.speaking
 
     @property
     def streaming(self) -> bool:
         """
-        If the current instance of OpenAIManager is in the process of streaming, returns True. Otherwise, returns False.
+        If the current instance of OpenAIService is in the process of streaming, returns True. Otherwise, returns False.
 
         Args:
             bool: The streaming state of the current instance.
         """
-        return self._openai_manager.streaming
+        return self._openai_service.streaming
 
     def interrupt(self, soft: bool = False, shutdown_time: Optional[int] = None) -> None:
         """
         Interrupts all speech-to-text recognition, text-to-speech synthesis, and OpenAI API streams.
 
         Args:
             soft (bool): If True, allows the recognizer to keep processing data that was recorded prior to interruption.
             shutdown_time (Optional[int]): The time at which the listener was deactivated.
         """
-        self._speech_to_text.interrupt(soft=soft, shutdown_time=shutdown_time)
-        self._text_to_speech.interrupt()
-        self._openai_manager.interrupt()
+        self._speech_recognition_service.interrupt(soft=soft, shutdown_time=shutdown_time)
+        self._speech_synthesis_service.interrupt()
+        self._openai_service.interrupt()
+        self._interrupt = time.perf_counter_ns() if not shutdown_time else shutdown_time
 
     def listener_toggle(self, name: Optional[str] = None) -> None:
         """
         Toggle the listening state of the bot. If the bot is currently listening, it will stop listening for user input
         using speech-to-text. If the bot is not currently listening, it will start listening for user input using
         speech-to-text.
 
@@ -156,40 +167,43 @@
         Activate the speech-to-text listener.
 
         Args:
             name (Optional[str]): The name of the user sending the message. Defaults to None.
         """
         if not self._listening_toggle:
             self._listening_toggle = True
+            # Interrupt any currently active ChatCompletion, text-to-speech, or speech-to-text streams
+            self.interrupt()
             init_time = time.perf_counter_ns()
             self._listen_thread = threading.Thread(
-                target=self._listen, kwargs={"name": name, "init_time": init_time}, daemon=True
+                target=self._listen,
+                kwargs={"name": name, "init_time": init_time},
+                daemon=True,
             )
             self._listen_thread.start()
 
     def listener_deactivate(self) -> None:
         """
         Deactivate the speech-to-text listener.
         """
         if self._listening_toggle:
             self._listening_toggle = False
             shutdown_time = time.perf_counter_ns()
-            self._speech_to_text.interrupt(soft=True, shutdown_time=shutdown_time)
+            self._speech_recognition_service.interrupt(soft=True, shutdown_time=shutdown_time)
 
     def prompt(self, message: str, name: Optional[str] = None) -> None:
         """
-        Prompt the bot with the given user message.
+        Prompt the bot with the specified user message.
 
         Args:
             message (str): The message content from the user.
             name (Optional[str]): The name of the user sending the message. Defaults to None.
         """
         # Do not send the message if it is empty.
         if message.strip():
-
             # Interrupt any currently active ChatCompletion, text-to-speech, or speech-to-text streams
             self.interrupt()
 
             message_thread = threading.Thread(
                 target=self.send_message,
                 args=(
                     message,
@@ -200,15 +214,15 @@
             )
             self._thread_queue.add_task(message_thread, unskippable=True)
             self._thread_queue.add_task(threading.Thread(target=self.respond, daemon=True))
 
     def respond(self) -> None:
         """
         Get a response from the bot and update the conversation area with the response. This method handles generating
-        the bot's response using the OpenAIManager and updating the conversation area with the response text using
+        the bot's response using the OpenAIService and updating the conversation area with the response text using
         text-to-speech synthesis.
         """
         if self._tone is None:
             self._respond_no_tone()
         elif self._tone == ToneMode.BASIC:
             self._respond_basic_tone()
         elif self._tone == ToneMode.ADVANCED:
@@ -230,28 +244,26 @@
             name (Optional[str]): The name of the user sending the message. Defaults to None.
             hidden (bool): If True, does not display the message in the interface.
         """
         message = Message(role=role, name=name, content=content)
         name = message.name.title() if message.name is not None else ChatCompletionRoles.USER.value.title()
         text = f"{name}: {content}\n\n"
         self._messages.append(message)
-        self._messages_token_count.append(message.count_tokens(model=self._model))
         if not hidden:
             self.update_conversation_area(word=text)
 
     def system_prompt(self, message: str, name: Optional[str] = None) -> None:
         """
-        Prompt the bot with the given message, issuing a command which is not displayed in the conversation area.
+        Prompt the bot with the specified message, issuing a command which is not displayed in the conversation area.
 
         Args:
             message (str): The message content from the user.
         """
         # Do not send the message if it is empty.
         if message.strip():
-
             # Interrupt any currently active ChatCompletion, text-to-speech, or speech-to-text streams
             self.interrupt()
 
             message_thread = threading.Thread(
                 target=self.send_message,
                 args=(
                     message,
@@ -263,15 +275,15 @@
             )
             self._thread_queue.add_task(message_thread, unskippable=True)
             self._thread_queue.add_task(threading.Thread(target=self.respond, daemon=True))
 
     @abstractmethod
     def update_conversation_area(self, word: str) -> None:
         """
-        Update the conversation area with the given word, and add the word to the chat log.
+        Update the conversation area with the specified word, and add the word to the chat log.
         This method should be implemented by subclasses to handle updating the specific GUI components.
 
         Args:
             word (str): The word to add to the conversation area.
         """
         self._append_to_chat_log(word)
 
@@ -311,109 +323,100 @@
         """
         tone = self._tone_selector.select(self._messages)
         return tone if tone is not None else self._style
 
     def _respond_advanced_tone(self) -> None:
         """
         Get a response from the bot and update the conversation area with the response. This method handles generating
-        the bot's response using the OpenAIManager and updating the conversation area with the response text using
+        the bot's response using the OpenAIService and updating the conversation area with the response text using
         text-to-speech synthesis.
         """
         prefixed = False
         content = []
+        context = []
 
         # Initialize the generator for asynchronous yielding of sentence blocks
-        for block in self._openai_manager.prompt_stream(messages=self._messages):
+        for block in self._openai_service.prompt_stream(messages=self._messages):
             if not prefixed:
                 self.update_conversation_area(f"{self._assistant_name}: ")
                 prefixed = True
 
-            phrases, outputs = self._prosody_selector.select(sentences=block, context=content, system=self._system)
+            phrases, context = self._prosody_selector.select(sentences=block, context=content, system=self._system)
 
             if phrases is None:
                 raise FormatMismatchError()
 
-            for word in self._text_to_speech.speak_phrases(phrases):
+            for word in self._speech_synthesis_service.speak_phrases(phrases):
                 self.update_conversation_area(word.word)
                 content.append(word.word)
 
             self.update_conversation_area(" ")
             content.append(" ")
 
         content = "".join(content)
         message = Message(role=ChatCompletionRoles.ASSISTANT, content=content.strip())
         self._messages.append(message)
-        self._messages_token_count.append(message.count_tokens(model=self._model))
 
         self._response_end()
 
     def _respond_basic_tone(self) -> None:
         """
         Get a response from the bot and update the conversation area with the response. This method handles generating
-        the bot's response using the OpenAIManager and updating the conversation area with the response text using
+        the bot's response using the OpenAIService and updating the conversation area with the response text using
         text-to-speech synthesis.
         """
         prefixed = False
         content = []
 
         style = self._get_next_tone()
         tone_content = f"Tone: {style}\n"
         # Add an intermediate message (not visualized in the conversation area) noting the assistant's tone.
         self._append_to_chat_log(tone_content)
         message = Message(role=ChatCompletionRoles.ASSISTANT, content=tone_content)
         self._messages.append(message)
-        self._messages_token_count.append(message.count_tokens(model=self._model))
 
         # Initialize the generator for asynchronous yielding of sentence blocks
-        for block in self._openai_manager.prompt_stream(messages=self._messages):
+        for block in self._openai_service.prompt_stream(messages=self._messages):
             if not prefixed:
                 self.update_conversation_area(f"{self._assistant_name}: ")
                 prefixed = True
-
             sentences = " ".join(block)
-            for word in self._text_to_speech.speak(sentences, voice=self._voice, style=style):
+            for word in self._speech_synthesis_service.speak(sentences, voice=self._voice, style=style):
                 self.update_conversation_area(word.word)
                 content.append(word.word)
-
             self.update_conversation_area(" ")
             content.append(" ")
-
         content = "".join(content)
         message = Message(role=ChatCompletionRoles.ASSISTANT, content=content.strip())
         self._messages.append(message)
-        self._messages_token_count.append(message.count_tokens(model=self._model))
         self._response_end()
 
     def _respond_no_tone(self) -> None:
         """
         Get a response from the bot and update the conversation area with the response. This method handles generating
-        the bot's response using the OpenAIManager and updating the conversation area with the response text using
+        the bot's response using the OpenAIService and updating the conversation area with the response text using
         text-to-speech synthesis.
         """
         prefixed = False
         content = []
 
         # Initialize the generator for asynchronous yielding of sentence blocks
-        for block in self._openai_manager.prompt_stream(messages=self._messages):
+        for block in self._openai_service.prompt_stream(messages=self._messages):
             if not prefixed:
                 self.update_conversation_area(f"{self._assistant_name}: ")
                 prefixed = True
-
             sentences = " ".join(block)
-            for word in self._text_to_speech.speak(sentences, voice=self._voice, style=self._style):
+            for word in self._speech_synthesis_service.speak(sentences, voice=self._voice, style=self._style):
                 self.update_conversation_area(word.word)
                 content.append(word.word)
-
             self.update_conversation_area(" ")
             content.append(" ")
-
         content = "".join(content)
         message = Message(role=ChatCompletionRoles.ASSISTANT, content=content.strip())
         self._messages.append(message)
-        self._messages_token_count.append(message.count_tokens(model=self._model))
         self._response_end()
 
     def _response_end(self) -> None:
         """
         End the bot's response and update the conversation area accordingly. This method should be called after the
         bot's response has been fully generated and added to the conversation area.
         """
@@ -423,36 +426,35 @@
         """
         Listen for user input using speech-to-text and prompt the bot with the transcribed message.
 
         Args:
             name (Optional[str]): The name of the user sending the message. Defaults to None.
             init_time (Optional[int]): The time at which the listener was activated.
         """
-        # Interrupt any currently active ChatCompletion, text-to-speech, or speech-to-text streams
-        self.interrupt(shutdown_time=init_time)
-
         # Flag is set to True if a new user input is detected.
         input_detected = False
 
         # Listen for user input using speech-to-text
-        for sentence in self._speech_to_text.listen(init_time=init_time):
-
+        for sentence in self._speech_recognition_service.listen(init_time=init_time):
+            # Break the loop if interrupted
+            if init_time < self._interrupt:
+                break
             # Do not send the message if it is empty.
-            if sentence.strip():
-
+            elif sentence.strip():
                 # Set the flag to True since a new user input was detected.
                 input_detected = True
 
                 # Send the transcribed message to the bot
                 message_thread = threading.Thread(
                     target=self.send_message,
                     args=(
                         sentence.strip(),
                         ChatCompletionRoles.USER,
                         name,
                     ),
                     daemon=True,
                 )
                 self._thread_queue.add_task(message_thread, unskippable=True)
-
-        if input_detected:
-            self._thread_queue.add_task(threading.Thread(target=self.respond, daemon=True))
+        # Respond if the listening loop is not broken.
+        else:
+            if input_detected:
+                self._thread_queue.add_task(threading.Thread(target=self.respond, daemon=True))
```

### Comparing `BanterBot-0.0.8/banterbot/extensions/option_selector.py` & `BanterBot-0.0.9/banterbot/extensions/option_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import logging
-from typing import List
 
 from banterbot.data.enums import ChatCompletionRoles
-from banterbot.data.openai_models import OpenAIModel
 from banterbot.data.prompts import OptionSelectorPrompts
-from banterbot.managers.openai_manager import OpenAIManager
-from banterbot.utils.message import Message
+from banterbot.models.message import Message
+from banterbot.models.openai_model import OpenAIModel
+from banterbot.services.openai_service import OpenAIService
 
 
 class OptionSelector:
     """
     The OptionSelector class facilitates evaluating and selecting the most suitable option from a set of provided
     options given a conversational context.
 
-    This class enhances the capabilities of the base OpenAIManager by providing a mechanism for option assessment for
+    This class enhances the capabilities of the base `OpenAIService` by providing a mechanism for option assessment for
     potential responses. The options provided can represent any category or attribute, such as emotional tones, topics,
     sentiment, etc., thus allowing for a variety of uses.
 
     The class accepts three main parameters: a list of options (strings), a prompt, and an initial system message. The
     system message sets the context for the OptionSelector's task, while the prompt provides a guideline for the
-    evaluation. The most suitable option is then selected based on the given conversational context.
+    evaluation. The most suitable option is then selected based on the specified conversational context.
 
     Example: Emotional Tone Selection
 
         options = ["angry", "cheerful", "excited", "friendly", "hopeful", "sad", "shouting", "terrified", "unfriendly"]
         prompt = "Choose the most suitable tone/emotion for the assistant's upcoming response."
         system = (
             "You are an Emotional Tone Evaluator. Given conversational context, you analyze and select the most "
@@ -31,40 +30,40 @@
         )
 
     This example showcases the OptionSelector as an "Emotional Tone Evaluator". The options are different emotional
     tones. Based on a conversational context, OptionSelector selects the most suitable tone for the assistant's next
     response.
     """
 
-    def __init__(self, model: OpenAIModel, options: List[str], system: str, prompt: str):
+    def __init__(self, model: OpenAIModel, options: list[str], system: str, prompt: str):
         """
-        Initialize the OptionSelector with the given model, options, system message, prompt, and optional seed.
+        Initialize the OptionSelector with the specified model, options, system message, prompt, and optional seed.
 
         Args:
             model (OpenAIModel): The OpenAI model to be used for generating responses.
-            options (List[str]): A list of strings representing the options to be evaluated.
+            options (list[str]): A list of strings representing the options to be evaluated.
             system (str): The initial system message that sets the context for the OptionSelector's task.
             prompt (str): The prompt that provides a guideline for the evaluation.
         """
         logging.debug(f"OptionSelector initialized")
         self._options = options
         self._system = system
         self._prompt = prompt
 
-        self._openai_manager = OpenAIManager(model=model)
+        self._openai_manager = OpenAIService(model=model)
         self._system_processed = self._init_system_prompt()
 
-    def select(self, messages: List[Message]) -> str:
+    def select(self, messages: list[Message]) -> str:
         """
         Select an option by asking the OpenAI ChatCompletion API to pick an answer. The prompt is set up to force the
         model to return a single token with dummy text preceding it in order to yield consistent results in an efficient
         way.
 
         Args:
-            messages (List[Message]): The list of messages to be processed.
+            messages (list[Message]): The list of messages to be processed.
 
         Returns:
             str: The randomly selected option.
         """
         messages = self._insert_messages(messages)
         response = self._openai_manager.prompt(messages=messages, split=False, temperature=0.0, top_p=1.0, max_tokens=1)
         try:
@@ -82,23 +81,23 @@
         Returns:
             str: The processed system prompt.
         """
         options = ", ".join(f"{n+1} {option}" for n, option in enumerate(self._options))
         system_prompt = f"{self._system} {OptionSelectorPrompts.PREFIX.value}{options}"
         return system_prompt
 
-    def _insert_messages(self, messages: List[Message]) -> List[Message]:
+    def _insert_messages(self, messages: list[Message]) -> list[Message]:
         """
         Insert the system prompt, user prompt, prefix, suffix, and a dummy message mimicking a successful interaction
         with the ChatCompletion API, into the list of messages.
 
         Args:
-            messages (List[Message]): The list of messages to be processed.
+            messages (list[Message]): The list of messages to be processed.
 
         Returns:
-            List[Message]: The enhanced list of messages.
+            list[Message]: The enhanced list of messages.
         """
         prefix = Message(role=ChatCompletionRoles.SYSTEM, content=self._system_processed)
         suffix = Message(role=ChatCompletionRoles.USER, content=self._prompt)
         dummy_message = Message(role=ChatCompletionRoles.ASSISTANT, content=OptionSelectorPrompts.DUMMY.value)
         messages = [prefix] + messages + [suffix, dummy_message]
         return messages
```

### Comparing `BanterBot-0.0.8/banterbot/extensions/prosody_selector.py` & `BanterBot-0.0.9/banterbot/extensions/prosody_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import logging
 import re
 from typing import Optional
 
 from banterbot.config import RETRY_LIMIT
-from banterbot.data.azure_neural_voices import AzureNeuralVoice
 from banterbot.data.enums import ChatCompletionRoles, Prosody
-from banterbot.data.openai_models import OpenAIModel
 from banterbot.data.prompts import ProsodySelection
-from banterbot.utils.message import Message
-from banterbot.utils.phrase import Phrase
+from banterbot.models.azure_neural_voice import AzureNeuralVoice
+from banterbot.models.message import Message
+from banterbot.models.openai_model import OpenAIModel
+from banterbot.models.phrase import Phrase
 
 
 class ProsodySelector:
     """
     The ProsodySelector class is responsible for managing prosody selection/extraction for specified instances of the
     AzureNeuralVoice class. It uses the OpenAI ChatCompletion API to generate prosody settings for a list of sentences.
 
     Attributes:
         _model (OpenAIModel): The OpenAI model to be used for generating responses.
-        _openai_manager (OpenAIManager): An instance of the OpenAIManager class.
+        _openai_manager (OpenAIService): An instance of the OpenAIService class.
         _voice (AzureNeuralVoice): An instance of the AzureNeuralVoice class.
         _valid (bool): A flag indicating whether the voice styles are not None.
         _token_counts (dict): A dictionary to cache the maximum number of tokens for a given number of rows.
         _output_patterns (dict): A dictionary to cache the regex patterns matching the expected ChatCompletion output.
         _system (list[Message]): A list of system and user messages to be used as a prompt for the ChatCompletion API.
         _line_pattern (str): A regex pattern that matches one line of expected output for the current model.
     """
 
     def __init__(self, manager: OpenAIModel, voice: AzureNeuralVoice) -> None:
         """
         Initializes the ProsodySelector class with a specified OpenAI model and AzureNeuralVoice instance.
 
         Args:
-            manager (OpenAIManager): An instance of class OpenAIManager to be used for generating responses.
+            manager (OpenAIService): An instance of class OpenAIService to be used for generating responses.
             voice (AzureNeuralVoice): An instance of the AzureNeuralVoice class.
         """
         logging.debug(f"ProsodySelector initialized")
         self._manager = manager
         self._voice = voice
         self._valid = self._voice.styles is not None
         self._token_counts = {}
@@ -109,25 +109,24 @@
             system (Optional[str]): A system prompt to assist the ChatCompletion in picking reactions.
 
         Returns:
             str: The randomly selected option.
         """
 
         for i in range(RETRY_LIMIT):
-
-            # Attempt several different sentence splits in order to modify the input on retry -- this reduces the chance
-            # of a `FormatMismatchError` Exception significantly. `RETRY_LIMIT` is defined in the config file.
+            # Attempt several different sentence splits in order to modify the input on retry -- significantly reduces
+            # the chance of raising a `FormatMismatchError` Exception. `RETRY_LIMIT` is defined in the config file.
             if i == 0:
-                phrases = self._split_sentences(sentences)
+                phrases = self._split_sentences(sentences=sentences)
             elif i == 1:
                 phrases = " ".join(sentences).split(".")
             else:
                 phrases = [" ".join(sentences)]
 
-            messages = self._get_messages(phrases, context, system)
+            messages = self._get_messages(phrases=phrases, system=system, context=context)
 
             response = self._manager.prompt(
                 messages=messages,
                 split=False,
                 temperature=0.0,
                 top_p=1.0,
                 max_tokens=self._get_max_tokens(len(phrases)),
@@ -135,21 +134,27 @@
             processed, outputs = self._process_response(phrases, response)
 
             if processed is not None:
                 break
 
         if processed is None:
             processed = [Phrase(text=sentence, voice=self._voice) for sentence in sentences]
+        else:
+            outputs = [
+                ProsodySelection.PROMPT.value.format(len(phrases), "\n".join(phrases)),
+                ProsodySelection.DUMMY.value.format(len(phrases)),
+                "\n".join(outputs),
+            ]
 
         return processed, outputs
 
     def _get_max_tokens(self, N: int) -> int:
         """
-        Returns the maximum number of tokens for the given number of rows of six-digit numbers. Caches all calculated
-        values.
+        Returns the maximum number of tokens for the specified number of rows of six-digit numbers. Caches all
+        calculated values.
 
         Args:
             N (int): The number of rows.
 
         Returns:
             int: The maximum number of tokens.
         """
@@ -174,15 +179,15 @@
         # Compile a regex pattern that matches `N` lines of expected output from ChatCompletion's prosody evaluation.
         if N not in self._output_patterns:
             self._output_patterns[N] = re.compile(f"{self._line_pattern}\n" * (N - 1) + self._line_pattern)
 
         return self._output_patterns[N]
 
     def _get_messages(
-        self, phrases: list[str], context: Optional[str] = None, system: Optional[str] = None
+        self, phrases: list[str], system: Optional[str] = None, context: Optional[str] = None
     ) -> list[Message]:
         """
         Inserts the system prompt, user prompt, prefix, suffix, and a dummy message mimicking a successful interaction
         with the ChatCompletion API, into the list of messages.
 
         Args:
             phrases (list[str]): The list of phrases to be processed.
@@ -190,20 +195,20 @@
             system (Optional[str]): A system prompt to assist the ChatCompletion in picking reactions.
 
         Returns:
             list[Message]: The enhanced list of messages.
         """
         messages = self._system.copy()
 
-        if not system:
+        if system:
             messages.append(
                 Message(role=ChatCompletionRoles.SYSTEM, content=ProsodySelection.CHARACTER.value.format(system))
             )
 
-        if not context:
+        if context:
             messages.append(
                 Message(role=ChatCompletionRoles.SYSTEM, content=ProsodySelection.CONTEXT.value.format(context))
             )
 
         messages.append(
             Message(
                 role=ChatCompletionRoles.USER,
```

### Comparing `BanterBot-0.0.8/banterbot/gui/cli.py` & `BanterBot-0.0.9/banterbot/gui/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import logging
 
-from banterbot.data.azure_neural_voices import _neural_voices
 from banterbot.data.enums import Prosody, ToneMode
-from banterbot.data.openai_models import _openai_models
 from banterbot.gui.tk_multiplayer_interface import TKMultiplayerInterface
+from banterbot.managers.azure_neural_voice_manager import AzureNeuralVoiceManager
+from banterbot.managers.openai_model_manager import OpenAIModelManager
 
 
 def run() -> None:
     """
     The main function to run the BanterBot Command Line Interface.
 
     This function parses command line arguments, sets up the necessary configurations, and initializes the BanterBotTK
@@ -40,22 +40,22 @@
         type=str,
         dest="prompt",
         help="Adds a system prompt to the beginning of the conversation; can help to set the scene.",
     )
 
     class ModelChoice(argparse.Action):
         def __call__(self, parser, namespace, values, option_string=None):
-            setattr(namespace, self.dest, _openai_models[values.lower()])
+            setattr(namespace, self.dest, OpenAIModelManager.load(values.lower()))
 
     parser.add_argument(
         "-m",
         "--model",
-        choices=_openai_models,
+        choices=OpenAIModelManager.list(),
         action=ModelChoice,
-        default=_openai_models["gpt-4"],
+        default=OpenAIModelManager.load("gpt-4-turbo"),
         dest="model",
         help="Select the OpenAI model the bot should use.",
     )
 
     class ToneModeChoice(argparse.Action):
         def __call__(self, parser, namespace, values, option_string=None):
             conversion_table = {
@@ -73,22 +73,22 @@
         default=ToneMode.ADVANCED,
         dest="tone_mode",
         help="Set the emotional tone evaluation mode for the bot's responses.",
     )
 
     class VoiceChoice(argparse.Action):
         def __call__(self, parser, namespace, values, option_string=None):
-            setattr(namespace, self.dest, _neural_voices[values.lower()])
+            setattr(namespace, self.dest, AzureNeuralVoiceManager.load(values.lower()))
 
     parser.add_argument(
         "-v",
         "--voice",
-        choices=_neural_voices,
+        choices=AzureNeuralVoiceManager.list(),
         action=VoiceChoice,
-        default=_neural_voices["aria"],
+        default=AzureNeuralVoiceManager.load("aria"),
         dest="voice",
         help=f"Select a Microsoft Azure Cognitive Services text-to-speech voice.",
     )
 
     parser.add_argument(
         "-s",
         "--style",
```

### Comparing `BanterBot-0.0.8/banterbot/gui/tk_multiplayer_interface.py` & `BanterBot-0.0.9/banterbot/gui/tk_multiplayer_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import logging
 import threading
 import tkinter as tk
 from tkinter import ttk
 from typing import Optional, Union
 
-from banterbot.data.azure_neural_voices import AzureNeuralVoice, get_voice_by_name
 from banterbot.data.enums import ToneMode
-from banterbot.data.openai_models import OpenAIModel, get_model_by_name
 from banterbot.data.prompts import Greetings
 from banterbot.extensions.interface import Interface
+from banterbot.managers.azure_neural_voice_manager import AzureNeuralVoiceManager
+from banterbot.managers.openai_model_manager import OpenAIModelManager
+from banterbot.models.azure_neural_voice import AzureNeuralVoice
+from banterbot.models.openai_model import OpenAIModel
 
 
 class TKMultiplayerInterface(tk.Tk, Interface):
     """
     A graphical user interface (GUI) class that enables interaction with the BanterBot chatbot in a multiplayer mode.
     It supports functionalities such as text input, text-to-speech and speech-to-text capabilities for up to 9 users
     simultaneously, based on OpenAI and Azure services.
 
     This class inherits from tkinter's Tk class and a custom Interface class, allowing it to be displayed as a
     standalone window and follow a specific chatbot interaction protocol respectively.
     """
 
     def __init__(
         self,
-        model: OpenAIModel = get_model_by_name("gpt-3.5-turbo"),
-        voice: AzureNeuralVoice = get_voice_by_name("Aria"),
+        model: OpenAIModel = OpenAIModelManager.load("gpt-3.5-turbo"),
+        voice: AzureNeuralVoice = AzureNeuralVoiceManager.load("Aria"),
         style: str = "chat",
         languages: Optional[Union[str, list[str]]] = None,
         tone_mode: Optional[ToneMode] = None,
+        tone_mode_model: OpenAIModel = None,
         system: Optional[str] = None,
         phrase_list: Optional[list[str]] = None,
         assistant_name: Optional[str] = None,
     ) -> None:
         """
         Initialize the TKMultiplayerInterface class, which inherits from both tkinter.Tk and Interface.
 
@@ -51,14 +54,15 @@
             self,
             model=model,
             voice=voice,
             style=style,
             languages=languages,
             system=system,
             tone_mode=tone_mode,
+            tone_mode_model=tone_mode_model,
             phrase_list=phrase_list,
             assistant_name=assistant_name,
         )
 
         # Bind the `_quit` method to program exit, in order to guarantee the stopping of all running threads.
         self.protocol("WM_DELETE_WINDOW", self._quit)
 
@@ -105,15 +109,15 @@
         This method is called on exit, and interrupts any currently running activity.
         """
         self.interrupt()
         self.quit()
         self.destroy()
 
     def _init_gui(self) -> None:
-        self.title(f"BanterBot {self._model.name}")
+        self.title(f"BanterBot {self._model.model}")
         self.configure(bg="black")
         self.geometry("1024x565")
         self._font = ("Cascadia Code", 16)
 
         self.style = ttk.Style()
         self.style.theme_use("clam")
         self.style.configure(".", font=self._font, bg="black", fg="white")
```

### Comparing `BanterBot-0.0.8/banterbot/gui/tk_simple_interface.py` & `BanterBot-0.0.9/banterbot/gui/tk_simple_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 import tkinter as tk
 from tkinter import ttk
 from typing import Optional, Union
 
-from banterbot.data.azure_neural_voices import AzureNeuralVoice, get_voice_by_name
 from banterbot.data.enums import ToneMode
-from banterbot.data.openai_models import OpenAIModel, get_model_by_name
 from banterbot.data.prompts import Greetings
 from banterbot.extensions.interface import Interface
+from banterbot.managers.azure_neural_voice_manager import AzureNeuralVoiceManager
+from banterbot.managers.openai_model_manager import OpenAIModelManager
+from banterbot.models.azure_neural_voice import AzureNeuralVoice
+from banterbot.models.openai_model import OpenAIModel
 
 
 class TKSimpleInterface(tk.Tk, Interface):
     """
     TKSimpleInterface is a graphical user interface (GUI) for the BanterBot package that uses OpenAI models for
     generating responses, Azure Neural Voices for text-to-speech, and Azure speech-to-text recognition. The class
     inherits from both tkinter.Tk and Interface, providing a seamless integration of the chatbot functionality with a
@@ -21,20 +23,21 @@
     conversation history in a scrollable text area. Users can send messages by pressing the "Send" button or the "Enter"
     key. The chatbot's responses are generated using the specified OpenAI model and can be played back using the
     specified Azure Neural Voice. Additionally, users can toggle speech-to-text input by pressing the "Listen" button.
     """
 
     def __init__(
         self,
-        model: OpenAIModel = get_model_by_name("gpt-3.5-turbo"),
-        voice: AzureNeuralVoice = get_voice_by_name("Aria"),
+        model: OpenAIModel = OpenAIModelManager.load("gpt-3.5-turbo"),
+        voice: AzureNeuralVoice = AzureNeuralVoiceManager.load("Aria"),
         style: str = "chat",
         languages: Optional[Union[str, list[str]]] = None,
         system: Optional[str] = None,
         tone_mode: Optional[ToneMode] = None,
+        tone_mode_model: OpenAIModel = None,
         phrase_list: Optional[list[str]] = None,
         assistant_name: Optional[str] = None,
     ) -> None:
         """
         Initialize the TKSimpleInterface class, which inherits from both tkinter.Tk and Interface.
 
         Args:
@@ -53,24 +56,25 @@
             self,
             model=model,
             voice=voice,
             style=style,
             languages=languages,
             system=system,
             tone_mode=tone_mode,
+            tone_mode_model=tone_mode_model,
             phrase_list=phrase_list,
             assistant_name=assistant_name,
         )
 
         # Bind the `_quit` method to program exit, in order to guarantee the stopping of all running threads.
         self.protocol("WM_DELETE_WINDOW", self._quit)
 
     def update_conversation_area(self, word: str) -> None:
         """
-        Update the conversation area with the given word.
+        Update the conversation area with the specified word.
 
         Args:
             word (str): The word to be added to the conversation area.
         """
         super().update_conversation_area(word)
         self.conversation_area["state"] = tk.NORMAL
         self.conversation_area.insert(tk.END, word)
@@ -129,26 +133,26 @@
             self.system_prompt(Greetings.UNPROMPTED_GREETING.value)
         self.mainloop()
 
     def _quit(self) -> None:
         """
         This method is called on exit, and interrupts any currently running activity.
         """
-        self._openai_manager.interrupt()
-        self._text_to_speech.interrupt()
-        self._speech_to_text.interrupt()
+        self._openai_service.interrupt()
+        self._speech_synthesis_service.interrupt()
+        self._speech_recognition_service.interrupt()
         self.quit()
         self.destroy()
 
     def _init_gui(self) -> None:
         """
         Initialize the graphical user interface for the BanterBot application.
         This method sets up the main window, conversation area, input fields, and buttons.
         """
-        self.title(f"BanterBot {self._model.name}")
+        self.title(f"BanterBot {self._model.model}")
         self.configure(bg="black")
         self.geometry("1024x768")
         self._font = ("Cascadia Code", 16)
 
         self.style = ttk.Style()
         self.style.theme_use("clam")
         self.style.configure(".", font=self._font, bg="black", fg="white")
```

### Comparing `BanterBot-0.0.8/banterbot/managers/memory_chain.py` & `BanterBot-0.0.9/banterbot/managers/memory_chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import logging
 import shutil
-from typing import Dict, List, Optional
+from typing import Optional
+
+from typing_extensions import Self
 
 from banterbot import config
+from banterbot.models.memory import Memory
 from banterbot.protos import memory_pb2
-from banterbot.utils.memory import Memory
 from banterbot.utils.nlp import NLP
 
 
 class MemoryChain:
     """
     MemoryChain is a class responsible for managing and handling arrays of memories using Protocol Buffers. It provides
     functionality to save memories to a binary file, load memories from a binary file, and retrieve memories based on
     keywords. The MemoryChain class is designed to efficiently store and retrieve memories based on keywords, allowing
     for quick access to relevant information.
     """
 
     @classmethod
-    def create(cls) -> "MemoryChain":
+    def create(cls) -> Self:
         """
         Generate a new empty set of memories and associated UUID.
 
         Returns:
             MemoryChain: A new instance of MemoryChain with an empty set of memories and a unique UUID.
         """
         uuid = config.generate_uuid().hex
@@ -35,15 +37,15 @@
         with open(config.personae / uuid / config.memory_index, "wb+") as fs:
             fs.write(memory_index.SerializeToString())
 
         logging.debug(f"MemoryChain created new UUID: `{uuid}`")
         return cls(uuid=uuid, memory_index={})
 
     @classmethod
-    def load(cls, uuid: str) -> "MemoryChain":
+    def load(cls, uuid: str) -> Self:
         """
         Load the memories from a binary file using Protocol Buffers deserialization and creates a MemoryChain instance.
         This method is used to load an existing set of memories from a file, allowing for the continuation of a previous
         session or the sharing of memories between different instances.
 
         Args:
             uuid (str): The UUID of the memory files to load.
@@ -70,22 +72,22 @@
         by removing the directory and all its contents, including memory files and the memory index file.
 
         Args:
             uuid (str): The UUID associated with this set of memories.
         """
         shutil.rmtree(config.personae / uuid)
 
-    def __init__(self, uuid: str, memory_index: Dict[str, List[str]]) -> None:
+    def __init__(self, uuid: str, memory_index: dict[str, list[str]]) -> None:
         """
         Initialize a new instance of MemoryChain.
 
         Args:
             uuid (str): The UUID associated with this set of memories.
 
-            memory_index (Dict[str, List[str]]): The dictionary mapping from keyword to list of memory UUIDs. This index
+            memory_index (dict[str, list[str]]): The dictionary mapping from keyword to list of memory UUIDs. This index
             is used to efficiently look up memories based on keywords.
         """
         logging.debug(f"MemoryChain initialized with UUID: `{uuid}`")
         self.uuid = uuid
         self._directory = config.personae / self.uuid / config.memories
         self._index_cache = memory_index
         self._memories = {}
@@ -103,51 +105,51 @@
             memory (Memory): The memory to append.
         """
         self._memories[memory.uuid] = memory
         self._save_memory(memory=memory)
         self._update_index(memory=memory)
         self._save_index()
 
-    def extend(self, memories: List[Memory]) -> None:
+    def extend(self, memories: list[Memory]) -> None:
         """
         Extend the current set of memories with a list of memories. This method is used to add multiple memories to the
         MemoryChain at once, allowing for the storage of new information in bulk. All changes are saved to file as soon
         as they are made.
 
         Args:
-            memories (List[Memory]): The list of memories to append.
+            memories (list[Memory]): The list of memories to append.
         """
         for memory in memories:
             self._memories[memory.uuid] = memory
             self._save_memory(memory=memory)
             self._update_index(memory=memory)
         self._save_index()
 
-    def search(self, keywords: List[str], fuzzy_threshold: Optional[float] = None) -> List[Memory]:
+    def search(self, keywords: list[str], fuzzy_threshold: Optional[float] = None) -> list[Memory]:
         """
-        Look up memories based on keywords. This method is used to retrieve memories that are relevant to the given
+        Look up memories based on keywords. This method is used to retrieve memories that are relevant to the specified
         keywords. It can also perform fuzzy matching, allowing for the retrieval of memories that are similar to the
         given keywords based on a similarity threshold.
 
         Args:
-            keywords (List[str]): The list of keywords to look up.
+            keywords (list[str]): The list of keywords to look up.
 
             fuzzy_threshold (Optional[float]): The threshold for fuzzy matching. If None, only returns exact matches. If
             a value is provided, memories with keywords that have a similarity score greater than or equal to the
             threshold will also be returned.
 
         Returns:
-            List[Memory]: The list of matching memories.
+            list[Memory]: The list of matching memories.
         """
         memory_uuids = set()
         memories = []
         if fuzzy_threshold is not None:
             self._update_similarity_cache(keywords=keywords)
 
-            # Find additional keywords that are similar to the given keywords
+            # Find additional keywords that are similar to the specified keywords
             keywords_extension = []
             cache_filtered = [i for i in self._index_cache.keys() if i not in keywords]
             for keyword in keywords:
                 for keyword_indexed in cache_filtered:
                     if self._similarity_cache[(keyword, keyword_indexed)] >= fuzzy_threshold:
                         keywords_extension.append(keyword_indexed)
             keywords.extend(keywords_extension)
@@ -219,35 +221,35 @@
         Args:
             memory_uuid (str): The UUID of the memory to load.
         """
         filename = memory_uuid + config.protobuf_extension
         with open(self._directory / filename, "rb") as fs:
             self._memories[memory_uuid] = Memory.deserialize(fs.read())
 
-    def _update_token_cache(self, keywords: List[str]) -> None:
+    def _update_token_cache(self, keywords: list[str]) -> None:
         """
         Update the token cache with new keywords. This method is used to keep the token cache up-to-date when new
         keywords are added to the MemoryChain. The token cache allows for efficient computation of similarity scores
         between keywords.
 
         Args:
-            keywords (List[str]): The new keywords to update the cache with.
+            keywords (list[str]): The new keywords to update the cache with.
         """
         new_keywords = [keyword for keyword in keywords if keyword not in self._token_cache.keys()]
         for keyword, token in zip(new_keywords, NLP.tokenize(strings=new_keywords)):
             self._token_cache[keyword] = token
 
-    def _update_similarity_cache(self, keywords: List[str]) -> None:
+    def _update_similarity_cache(self, keywords: list[str]) -> None:
         """
         Update the similarity cache with new keywords. This method is used to keep the similarity cache up-to-date when
         new keywords are added to the MemoryChain. The similarity cache allows for efficient computation of similarity
         scores between keywords, enabling fuzzy matching in the search method.
 
         Args:
-            keywords (List[str]): The new keywords to update the cache with.
+            keywords (list[str]): The new keywords to update the cache with.
         """
         self._update_token_cache(keywords=keywords)
         for keyword_indexed in self._index_cache.keys():
             for keyword in keywords:
                 pair = (keyword, keyword_indexed)
                 if pair not in self._similarity_cache.keys():
                     similarity = self._token_cache[keyword].similarity(self._token_cache[keyword_indexed])
```

### Comparing `BanterBot-0.0.8/banterbot/managers/openai_manager.py` & `BanterBot-0.0.9/banterbot/services/openai_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,102 +1,110 @@
 import datetime
 import logging
 import os
 import time
-from typing import Generator, Iterator, List, Tuple, Union
+from typing import Generator, Iterator, Union
 
 import openai
 
 from banterbot.config import RETRY_LIMIT, RETRY_TIME
 from banterbot.data.enums import EnvVar
-from banterbot.data.openai_models import OpenAIModel
-from banterbot.utils.message import Message
+from banterbot.models.message import Message
+from banterbot.models.openai_model import OpenAIModel
 from banterbot.utils.nlp import NLP
 
 # Set the OpenAI API key
 openai.api_key = os.environ.get(EnvVar.OPENAI_API_KEY.value)
 
 
-class OpenAIManager:
+class OpenAIService:
     """
     A class that handles the interaction with the OpenAI ChatCompletion API. It provides functionality to generate
     responses from the API based on the input messages. It supports generating responses as a whole or as a stream of
     response blocks.
 
-    The main purpose of this class is to facilitate the communication with the OpenAI API and manage the responses
+    The main purpose of this class is to facilitate the communication with the OpenAI API and handle the responses
     generated by the API. It can be used to create chatbots or other applications that require natural language
     processing and generation.
     """
 
     def __init__(self, model: OpenAIModel) -> None:
         """
-        Initializes an OpenAIManager instance for a specific model.
+        Initializes an `OpenAIService` instance for a specific model.
 
         Args:
             model (OpenAIModel): The OpenAI model to be used. This should be an instance of the OpenAIModel class, which
             contains information about the model, such as its name and maximum token limit.
         """
-        logging.debug(f"OpenAIManager initialized")
+        logging.debug(f"OpenAIService initialized")
 
         # The selected model that will be used in OpenAI ChatCompletion prompts.
         self._model = model
 
-        # Indicates whether the current instance of OpenAIManager is streaming.
+        # Indicates whether the current instance of `OpenAIService` is streaming.
         self._streaming = False
 
-        # Set the interruption flag to the current time: if interruptions are raised, this will be updated.
-        self._interrupt: int = time.perf_counter_ns()
+        # Set the interruption flag to zero: if interruptions are raised, this will be updated.
+        self._interrupt: int = 0
 
     def count_tokens(self, string: str) -> int:
         """
         Counts the number of tokens in the provided string.
 
         Args:
             string (str): A string provided by the user where the number of tokens are to be counted.
 
         Returns:
             int: The number of tokens in the string.
         """
         return len(self._model.tokenizer.encode(string))
 
-    def prompt(self, messages: List[Message], split: bool = True, **kwargs) -> Union[Tuple[str], str]:
+    def interrupt(self) -> None:
+        """
+        Interrupts any ongoing streaming processes. This method sets the interrupt flag to the current time, which will
+        cause any streaming processes activated prior to the current time to stop.
+        """
+        self._interrupt: int = time.perf_counter_ns()
+        logging.debug("OpenAIService stream interrupted")
+
+    def prompt(self, messages: list[Message], split: bool = True, **kwargs) -> Union[tuple[str], str]:
         """
         Sends messages to the OpenAI ChatCompletion API and retrieves the response as a list of sentences.
 
         Args:
-            messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
+            messages (list[Message]): A list of messages. Each message should be an instance of the Message class, which
             contains the content and role (user or assistant) of the message.
 
             split (bool): Whether the response should be split into sentences.
 
             **kwargs: Additional parameters for the API request. These can include settings such as temperature, top_p,
             and frequency_penalty.
 
         Returns:
-            Union[List[str], str]: A list of sentences forming the response from the OpenAI API. This can be used to
+            Union[list[str], str]: A list of sentences forming the response from the OpenAI API. This can be used to
             display the generated response to the user or for further processing. If `split` is False, returns a string.
         """
         response = self._request(messages=messages, stream=False, **kwargs)
-        logging.debug(f"OpenAIManager stream processed block: `{response}`")
+        logging.debug(f"OpenAIService stream processed block: `{response}`")
         sentences = NLP.segment_sentences(response) if split else response
         return sentences
 
-    def prompt_stream(self, messages: List[Message], **kwargs) -> Generator[Tuple[str], None, None]:
+    def prompt_stream(self, messages: list[Message], **kwargs) -> Generator[tuple[str], None, None]:
         """
         Sends messages to the OpenAI API and retrieves the response as a stream of blocks of sentences.
 
         Args:
-            messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
+            messages (list[Message]): A list of messages. Each message should be an instance of the Message class, which
             contains the content and role (user or assistant) of the message.
 
             **kwargs: Additional parameters for the API request. These can include settings such as temperature, top_p,
             and frequency_penalty.
 
         Yields:
-            Generator[List[str], None, None]: A stream of blocks of sentences as the response from the OpenAI API. Each
+            Generator[list[str], None, None]: A stream of blocks of sentences as the response from the OpenAI API. Each
             block contains one or more sentences that form a part of the generated response. This can be used to display
             the response to the user in real-time or for further processing.
         """
         # Record the time at which the request was made, in order to account for future interruptions.
         init_time = time.perf_counter_ns()
 
         # Obtain a response from the OpenAI ChatCompletion API
@@ -108,116 +116,117 @@
         # Yield the responses as they are streamed
         for block in self._response_parse_stream(response=response, init_time=init_time):
             yield block
 
         # Reset the streaming flag to False
         self._streaming = False
 
-    def interrupt(self) -> None:
+    @property
+    def model(self) -> OpenAIModel:
         """
-        Interrupts any ongoing streaming processes. This method sets the interrupt flag to the current time, which will
-        cause any streaming processes activated prior to the current time to stop.
+        Return the `OpenAIModel` associated with the current instance.
+
+        Returns:
+            OpenAIModel
         """
-        self._interrupt: int = time.perf_counter_ns()
-        logging.debug("OpenAIManager stream interrupted")
+        return self._model
 
     @property
     def streaming(self) -> bool:
         """
-        If the current instance of OpenAIManager is in the process of streaming, returns True. Otherwise, returns False.
+        If the current instance of OpenAIService is in the process of streaming, returns True. Otherwise, returns False.
 
         Args:
             bool: The streaming state of the current instance.
         """
         return self._streaming
 
-    def _request(self, messages: List[Message], stream: bool, **kwargs) -> Union[Iterator, str]:
+    def _response_parse_stream(self, response: Iterator, init_time: int) -> Generator[list[str], None, None]:
+        """
+        Parses a streaming response from the OpenAI API and yields blocks of text as they are received.
+
+        Args:
+            response (Iterator): A streaming response from the OpenAI ChatCompletion API.
+            init_time (int): The time at which the stream was initialized.
+
+        Yields:
+            Generator[list[str], None, bool]: Lists of sentences as blocks. Each block contains one or more sentences
+            that form a part of the generated response.
+        """
+        text = ""
+        logging.debug("OpenAIService stream started")
+
+        for chunk in response:
+            delta = chunk["choices"][0]["delta"]
+
+            if self._interrupt >= init_time:
+                logging.debug(f"OpenAIService interrupted")
+                break
+
+            if "content" in delta.keys():
+                text += delta["content"]
+
+            if len(sentences := NLP.segment_sentences(text)) > 1:
+                text = sentences[-1]
+                logging.debug(f"OpenAIService yielded sentences: {sentences[:-1]}")
+                yield sentences[:-1]
+        else:
+            sentences = NLP.segment_sentences(text)
+            logging.debug(f"OpenAIService yielded final sentences: {sentences[:-1]}")
+            yield sentences
+
+            logging.debug("OpenAIService stream stopped")
+
+    def _request(self, messages: list[Message], stream: bool, **kwargs) -> Union[Iterator, str]:
         """
-        Sends a request to the OpenAI API and generates a response based on the given parameters.
+        Sends a request to the OpenAI API and generates a response based on the specified parameters.
 
         Args:
-            messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
+            messages (list[Message]): A list of messages. Each message should be an instance of the Message class, which
             contains the content and role (user or assistant) of the message.
 
             stream (bool): Whether the response should be returned as an iterable stream or a complete text.
 
             **kwargs: Additional parameters for the API request. These can include settings such as temperature, top_p,
             and frequency_penalty.
 
         Returns:
             Union[Iterator, str]: The response from the OpenAI API, either as a stream (Iterator) or text (str).
         """
-        kwargs["model"] = self._model.name
+        kwargs["model"] = self._model.model
         kwargs["n"] = 1
         kwargs["stream"] = stream
         kwargs["messages"] = [message() for message in messages]
 
         success = False
         for i in range(RETRY_LIMIT):
             try:
                 response = openai.ChatCompletion.create(**kwargs)
                 success = True
                 break
 
             except openai.error.APIError:
-                retry_time = 0.5
+                retry_time = 0.25
                 retry_timestamp = datetime.datetime.now() + datetime.timedelta(seconds=retry_time)
                 retry_timestamp = retry_timestamp.strptime("%H:%M:%S")
                 error_message = (
-                    f"OpenAIManager encountered an OpenAI API Error - Attempt {i+1}/{RETRY_LIMIT}. Waiting "
+                    f"OpenAIService encountered an OpenAI API Error - Attempt {i+1}/{RETRY_LIMIT}. Waiting "
                     f"{retry_time} seconds until {retry_timestamp} to retry."
                 )
                 logging.info(error_message)
                 time.sleep(retry_time)
 
             except openai.error.RateLimitError:
                 retry_timestamp = datetime.datetime.now() + datetime.timedelta(seconds=RETRY_TIME)
-                retry_timestamp = retry_timestamp.strptime("%H:%M:%S")
+                retry_timestamp = datetime.datetime.strftime(retry_timestamp, "%H:%M:%S")
                 error_message = (
-                    f"OpenAIManager encountered an OpenAI Rate Limiting Error - Attempt {i+1}/{RETRY_LIMIT}. Waiting "
+                    f"OpenAIService encountered an OpenAI Rate Limiting Error - Attempt {i+1}/{RETRY_LIMIT}. Waiting "
                     f"{RETRY_TIME} seconds until {retry_timestamp} to retry."
                 )
                 logging.info(error_message)
                 time.sleep(RETRY_TIME)
 
         if not success:
-            logging.info(f"OpenAIManager encountered too many OpenAI Errors - exiting program.")
+            logging.info(f"OpenAIService encountered too many OpenAI Errors - exiting program.")
             raise openai.error.APIError
 
         return response if stream else response.choices[0].message.content.strip()
-
-    def _response_parse_stream(self, response: Iterator, init_time: int) -> Generator[List[str], None, bool]:
-        """
-        Parses a streaming response from the OpenAI API and yields blocks of text as they are received.
-
-        Args:
-            response (Iterator): A streaming response from the OpenAI ChatCompletion API.
-            init_time (int): The time at which the stream was initialized.
-
-        Yields:
-            Generator[List[str], None, bool]: Lists of sentences as blocks. Each block contains one or more sentences
-            that form a part of the generated response.
-
-        Returns:
-            bool: True if the generator completed its iterations, False otherwise (due to interruption).
-        """
-        text = ""
-        logging.debug("OpenAIManager stream started")
-
-        for chunk in response:
-            delta = chunk["choices"][0]["delta"]
-
-            if self._interrupt >= init_time:
-                return False
-
-            if "content" in delta.keys():
-                text += delta["content"]
-
-            if len(sentences := NLP.segment_sentences(text)) > 1:
-                text = sentences[-1]
-                yield sentences[:-1]
-
-        sentences = NLP.segment_sentences(text)
-        yield sentences
-
-        logging.debug("OpenAIManager stream stopped")
-        return True
```

### Comparing `BanterBot-0.0.8/banterbot/managers/speech_to_text.py` & `BanterBot-0.0.9/banterbot/services/speech_recognition_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,68 +5,73 @@
 import time
 from typing import Generator, Optional, Union
 
 import azure.cognitiveservices.speech as speechsdk
 
 from banterbot.config import DEFAULT_LANGUAGE, soft_interruption_delay
 from banterbot.data.enums import EnvVar
-from banterbot.utils.speech_to_text_output import SpeechToTextOutput
+from banterbot.models.speech_recognition_output import SpeechRecognitionOutput
 
 
-class SpeechToText:
+class SpeechRecognitionService:
     """
-    The SpeechToText class provides an interface to convert spoken language into written text using Azure Cognitive
-    Services. It allows continuous speech recognition and provides real-time results as sentences are recognized.
+    The `SpeechRecognitionService` class provides an interface to convert spoken language into written text using Azure
+    Cognitive Speech Services. It allows continuous speech recognition and provides real-time results as sentences are
+    recognized.
     """
 
     # Create a lock that prevents race conditions when listening
     _listen_lock = threading.Lock()
 
     def __init__(
         self,
         languages: Union[str, list[str]] = None,
         phrase_list: Optional[list[str]] = None,
     ) -> None:
         """
-        Initializes the SpeechToText instance by setting up the Azure Cognitive Services speech configuration and
-        recognizer. Argument `recognition_language` can take one or more values, each representing a language the
-        recognizer can expect to receive as an input. The recognizer will attempt to auto-detect the language if
-        multiple are provided.
+        Initializes the `SpeechRecognitionService` instance by setting up the Azure Cognitive Services speech
+        configuration and recognizer. Argument `recognition_language` can take one or more values, each representing a
+        language the recognizer can expect to receive as an input. The recognizer will attempt to auto-detect the
+        language if multiple are provided.
 
         Args:
             languages (Union[str, list[str]): The language(s) the speech-to-text recognizer expects to hear.
             phrase_list(list[str], optional): Optionally provide the recognizer with context to improve recognition.
         """
-        logging.debug(f"SpeechToText initialized")
+        logging.debug(f"SpeechRecognitionService initialized")
 
         # Initialize the speech configuration with the Azure subscription and region
         self._speech_config = speechsdk.SpeechConfig(
             subscription=os.environ.get(EnvVar.AZURE_SPEECH_KEY.value),
             region=os.environ.get(EnvVar.AZURE_SPEECH_REGION.value),
         )
 
         # Allowing the speech configuration to recognize profane words
         self._speech_config.set_profanity(speechsdk.ProfanityOption.Raw)
 
         # Activate the receipt of data pertaining to word timings
         self._speech_config.request_word_level_timestamps()
 
         # Initialize the output and total length variables
-        self._outputs: list[SpeechToTextOutput] = []
+        self._outputs: list[SpeechRecognitionOutput] = []
 
         # Determine whether language auto-detection should be activated
         self._languages = DEFAULT_LANGUAGE if languages is None else languages
         self._auto_detection = not isinstance(self._languages, str)
 
         # Initialize the speech recognizer with the speech configuration and language settings
         self._recognizer = speechsdk.SpeechRecognizer(speech_config=self._speech_config, **self._language_kwargs())
 
         # Initialize an instance of `PhraseListGrammar` which is used to provide context to improve speech recognition
         self._phrase_list_grammar = speechsdk.PhraseListGrammar.from_recognizer(self._recognizer)
 
+        # Add any phrases in `phrase_list` to the `PhraseListGrammar`.
+        if phrase_list:
+            self.add_phrases(phrase_list)
+
         # Connect the speech recognizer events to their corresponding callbacks
         self._recognizer_events_connect()
 
         # Creating a new instance of Connection class
         self._connection = speechsdk.Connection.from_recognizer(self._recognizer)
 
         # Pre-connecting the speech recognizer for reduced latency
@@ -102,54 +107,53 @@
         self._interrupt: int = shutdown_time if shutdown_time is not None else time.perf_counter_ns()
         # Release any threading.Event instances that the listener may be waiting for.
         self._start_recognition.set()
         self._new_events.set()
         # If a hard interrupt is initiated, interrupt the Event waiting for the recognition to end.
         if not soft:
             self._stop_recognition.set()
-        logging.debug("SpeechToText listener interrupted")
+        logging.debug("SpeechRecognitionService listener interrupted")
 
     def listen(self, init_time: Optional[int] = None) -> Generator[str, None, None]:
         """
         Starts the speech-to-text recognition process and yields sentences as they are recognized.
 
         Yields:
             Generator[str, None, None]: A generator that yields tuples of recognized sentences.
             init_time (Optional[int]): The time at which the listener was activated.
         """
         # Record the time at which the thread was initialized pre-lock, in order to account for future interruptions.
         init_time = init_time if init_time is not None else time.perf_counter_ns()
 
         # Only allow one listener to be active at once.
         with self.__class__._listen_lock:
-
             # Do not run the listener if an interruption was raised after `init_time`.
             if self._interrupt <= init_time:
-
                 # Prepare a list which will contain all the recognized input words.
                 output = []
                 self._outputs.append(output)
 
                 # Set the listening flag to True
                 self._listening = True
 
                 # Monitor the recognition progress in the main thread, yielding sentences as they are processed
                 for block in self._callbacks_process(output=output, init_time=init_time):
-                    logging.debug(f"SpeechToText listener processed block: `{block}`")
+                    logging.debug(f"SpeechRecognitionService listener processed block: `{block}`")
                     yield block
 
-                logging.debug("SpeechToText listener stopped")
+                logging.debug("SpeechRecognitionService listener stopped")
 
                 # Reset all state attributes
                 self._reset()
 
     @property
     def listening(self) -> bool:
         """
-        If the current instance of SpeechToText is in the process of listening, returns True. Otherwise, returns False.
+        If the current instance of `SpeechRecognitionService` is in the process of listening, returns True. Otherwise,
+        returns False.
 
         Returns:
             bool: The listening state of the current instance.
         """
         return self._listening
 
     @property
@@ -160,16 +164,16 @@
         Returns:
             list[str]: The language-country pairs being used by the recognizer.
         """
         return self._languages
 
     def add_phrases(self, phrases: list[str]) -> None:
         """
-        Add a new phrase to the PhraseListGrammar instance, which implements a bias towards the given words/phrases that
-        can help improve speech recognition in circumstances where there may be potential ambiguity.
+        Add a new phrase to the PhraseListGrammar instance, which implements a bias towards the specified words/phrases
+        that can help improve speech recognition in circumstances where there may be potential ambiguity.
 
         Args:
             phrases(list[str]): Provide the recognizer with additional text context to improve recognition.
         """
         for phrase in phrases:
             self._phrase_list_grammar.addPhrase(phrase)
 
@@ -179,15 +183,15 @@
         """
         self._phrase_list_grammar.clear()
 
     def _language_kwargs(self) -> dict:
         """
         Set the language(s) being recognized by the Speech-to-Text recognizer in two modes: if a string is given to
         argument `languages` in the __init__ method, then set the language explicitly in the Azure speech SDK
-        `SpeechRecognizer` object in this `SpeechToText` instance. If a list of languages is given, use the
+        `SpeechRecognizer` object in this `SpeechRecognitionService` instance. If a list of languages is given, use the
         `AutoDetectSourceLanguageConfig` object from the speech SDK to allow the `SpeechRecognizer` to automatically
         choose the input language from one of those provided.
 
         Returns:
             dict: A dictionary of keywords arguments for the Speech Recognizer.
         """
         if self._auto_detection:
@@ -204,15 +208,15 @@
         return kwargs
 
     def _reset(self) -> None:
         """
         Resets the state variables of the speech-to-text recognizer, such as the list of events, the listening flag,
         the soft interruption flag, recognition started flag, recognition stopped flag, and new events flag.
         """
-        self._events: list[SpeechToTextOutput] = []
+        self._events: list[SpeechRecognitionOutput] = []
         self._listening: bool = False
         self._soft_interrupt: bool = False
         self._start_recognition_time = 0
         self._start_recognition.clear()
         self._stop_recognition.clear()
         self._new_events.clear()
 
@@ -246,59 +250,53 @@
         Args:
             event (speechsdk.SessionEventArgs): Event arguments containing information about the recognition started.
         """
         logging.debug("Recognizer connected")
         self._start_recognition_time = time.perf_counter_ns()
         self._start_recognition.set()
 
-    def _callbacks_process(self, output: list[SpeechToTextOutput], init_time: int) -> Generator[str, None, None]:
+    def _callbacks_process(self, output: list[SpeechRecognitionOutput], init_time: int) -> Generator[str, None, None]:
         """
         Processes the recognized speech events and appends them to the output list. Yields sentences as they are
         processed.
 
         Args:
-            output (list[SpeechToTextOutput]): The list in which to store the recognized speech events.
+            output (list[SpeechRecognitionOutput]): The list in which to store the recognized speech events.
             init_time (int): The time at which the listening was initialized.
 
         Yields:
             Generator[str, None, None]: A generator that yields sentences as they are processed.
         """
         # Initialize variables
         idx = 0
 
         # Starting the speech recognizer
         self._recognizer.start_continuous_recognition()
 
-        # Wait until the recognition has started before proceeding
-        self._start_recognition.wait()
+        logging.debug("SpeechRecognitionService listener started")
 
-        t = time.perf_counter_ns()
-        logging.debug("SpeechToText listener started")
+        dt = self._start_recognition_time + 1e3 * soft_interruption_delay.microseconds + self._interrupt - init_time
 
         # Continuously monitor the recognition progress
-        while self._interrupt <= init_time:
-
+        while self._interrupt < init_time:
             self._new_events.wait()
             self._new_events.clear()
 
-            while self._interrupt <= init_time and idx < len(self._events):
+            while self._interrupt < init_time and idx < len(self._events):
                 output.append(self._events[idx])
                 yield str(self._events[idx])
                 idx += 1
 
-        dt = self._start_recognition_time + 1e3 * soft_interruption_delay.microseconds + self._interrupt - init_time
-
         # Stop the recognizer
         self._recognizer.stop_continuous_recognition()
 
         if self._soft_interrupt >= self._interrupt:
             # Prepare a timedelta object indicating how long the listener was active.
             cutoff = datetime.timedelta(microseconds=1e-3 * (self._interrupt - init_time)) + soft_interruption_delay
             for idx in range(idx, len(self._events)):
-
                 if self._events[idx].offset - self._total_offset > cutoff:
                     break
                 elif self._events[idx].offset_end - self._total_offset > cutoff:
                     if (event := self._events[idx].from_cutoff(upper_cutoff=cutoff)) is not None:
                         self._events[idx] = event
 
                 output.append(self._events[idx])
@@ -313,12 +311,12 @@
             event (speechsdk.SpeechRecognitionEventArgs): The recognized speech event.
         """
         if self._start_recognition_time > self._last_total_offset:
             self._last_total_offset = self._start_recognition_time
             self._total_offset = datetime.timedelta(microseconds=event.offset / 10)
 
         self._events.append(
-            SpeechToTextOutput.from_recognition_result(
+            SpeechRecognitionOutput.from_recognition_result(
                 event.result, self._languages if not self._auto_detection else None
             )
         )
         self._new_events.set()
```

### Comparing `BanterBot-0.0.8/banterbot/managers/text_to_speech.py` & `BanterBot-0.0.9/banterbot/services/speech_synthesis_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 import datetime
 import logging
 import os
 import threading
 import time
-from typing import Generator, List, Optional, TypedDict
+from typing import Generator, Optional
 
 import azure.cognitiveservices.speech as speechsdk
 from azure.cognitiveservices.speech import SpeechSynthesisOutputFormat
 
-from banterbot.data.azure_neural_voices import AzureNeuralVoice
 from banterbot.data.enums import EnvVar, SpeechProcessingType, WordCategory
-from banterbot.utils.phrase import Phrase
-from banterbot.utils.text_to_speech_output import TextToSpeechOutput
-from banterbot.utils.word import Word
+from banterbot.models.azure_neural_voice import AzureNeuralVoice
+from banterbot.models.phrase import Phrase
+from banterbot.models.word import Word
+from banterbot.types.timed_event import TimedEvent
 
 
-class TimedEvent(TypedDict):
-    """
-    A specifically typed dictionary which is appended to the list of events in a TextToSpeech instance during speech
-    synthesis in a callback, containing the exact time at which the words in the event should be synthesized.
-    """
-
-    event: speechsdk.SessionEventArgs
-    time: int
-
-
-class TextToSpeech:
+class SpeechSynthesisService:
     """
     A class to handle text-to-speech synthesis utilizing Azure's Cognitive Services.
 
     This class provides an interface to convert text into speech using Azure's Cognitive Services. It supports various
     output formats, voices, and speaking styles. The synthesized speech can be interrupted, and the progress can be
     monitored in real-time.
     """
@@ -38,31 +28,28 @@
     _speech_lock = threading.Lock()
 
     def __init__(
         self,
         output_format: SpeechSynthesisOutputFormat = SpeechSynthesisOutputFormat.Audio16Khz32KBitRateMonoMp3,
     ) -> None:
         """
-        Initializes an instance of the TextToSpeech class with a specified output format.
+        Initializes an instance of the `SpeechSynthesisService` class with a specified output format.
 
         Args:
             output_format (SpeechSynthesisOutputFormat, optional): The desired output format for the synthesized speech.
-                Default is Audio16Khz32KBitRateMonoMp3.
+            Default is Audio16Khz32KBitRateMonoMp3.
         """
-        logging.debug(f"TextToSpeech initialized")
+        logging.debug(f"SpeechSynthesisService initialized")
 
         # Initialize the speech configuration with the Azure subscription and region
         self._speech_config = speechsdk.SpeechConfig(
             subscription=os.environ.get(EnvVar.AZURE_SPEECH_KEY.value),
             region=os.environ.get(EnvVar.AZURE_SPEECH_REGION.value),
         )
 
-        # Initialize the output and total length variables
-        self._outputs: List[TextToSpeechOutput] = []
-
         # Initialize the speech synthesizer with the speech configuration
         self._synthesizer = speechsdk.SpeechSynthesizer(speech_config=self._speech_config)
 
         # Set the speech synthesis output format to the specified output format
         self._speech_config.set_speech_synthesis_output_format(output_format)
 
         # Connect the speech synthesizer events to their corresponding callbacks
@@ -73,48 +60,44 @@
 
         # Preconnecting the speech synthesizer for reduced latency
         self._connection.open(True)
 
         # Set the interruption flag to the current time: if interruptions are raised, this will be updated.
         self._interrupt: int = time.perf_counter_ns()
 
+        # Initialize events.
+        self._start_synthesis: threading.Event = threading.Event()
+        self._stop_synthesis: threading.Event = threading.Event()
+        self._new_events: threading.Event = threading.Event()
+
         # Reset the state variables of the text-to-speech synthesizer
         self._reset()
 
     @property
-    def output(self) -> List[TextToSpeechOutput]:
-        """
-        Getter for the output property, which is a list of TextToSpeechOutput objects.
-
-        Returns:
-            List[TextToSpeechOutput]: The list of synthesized outputs.
-        """
-        return self._outputs
-
-    @property
     def speaking(self) -> bool:
         """
-        If the current instance of TextToSpeech is in the process of speaking, returns True. Otherwise, returns False.
+        If the current instance of `SpeechSynthesisService` is in the process of speaking, returns True. Otherwise,
+        returns False.
 
         Args:
             bool: The speaking state of the current instance.
         """
-        return self._speaking
+        return self._start_synthesis.is_set()
 
     def interrupt(self) -> None:
         """
         Interrupts an ongoing text-to-speech process, if any. This method sets the interrupt flag to the current time,
         which will cause any text-to-speech processes activated prior to the current time to stop.
         """
         self._interrupt: int = time.perf_counter_ns()
-        logging.debug("TextToSpeech synthesizer interrupted")
+        logging.debug("SpeechSynthesisService synthesizer interrupted")
 
-    def speak(self, input_string: str, voice: AzureNeuralVoice, style: str) -> Generator[Word, None, bool]:
+    def speak(self, input_string: str, voice: AzureNeuralVoice, style: str) -> Generator[Word, None, None]:
         """
-        Speaks the given text using the specified voice and style.
+        Speaks the specified text using the specified voice and style.
 
         This method converts the input text into speech using the specified voice and style. It yields the synthesized
         words one by one, along with their contextual information.
 
         Args:
             input_string (str): The input string that is to be converted into speech.
             voice (AzureNeuralVoice): The voice to be used.
@@ -122,46 +105,27 @@
 
         Yields:
             Word: A word with contextual information.
         """
         # Record the time at which the thread was initialized pre-lock, in order to account for future interruptions.
         init_time = time.perf_counter_ns()
 
-        # Create SSML markup for the given input_string, voice, and style
+        # Create SSML markup for the specified input_string, voice, and style
         ssml = self._create_ssml(input_string, voice, style)
 
-        # Create a new thread to handle the speech synthesis
-        speech_thread = threading.Thread(target=self._speak, args=(ssml,), daemon=True)
-
         with self.__class__._speech_lock:
+            # Continuously monitor the synthesis progress in the main thread, yielding words as they are uttered
+            for word in self._callbacks_process(ssml, init_time):
+                logging.debug(f"SpeechSynthesisService synthesizer processed word: `{word}`")
+                yield word
 
-            # Do not run the listener if an interruption was raised after `init_time`.
-            if self._interrupt < init_time:
-
-                # Prepare an instance of TextToSpeechOutput while will receive values iteratively
-                output = TextToSpeechOutput(
-                    input_string=input_string, timestamp=datetime.datetime.now(), voice=voice, style=style
-                )
-                self._outputs.append(output)
-
-                # Starting the speech synthesizer
-                speech_thread.start()
-
-                # Set the speaking flag to True
-                self._speaking = True
-
-                # Continuously monitor the synthesis progress in the main thread, yielding words as they are uttered
-                for word in self._callbacks_process(output, init_time):
-                    logging.debug(f"TextToSpeech synthesizer processed word: `{word}`")
-                    yield word
-
-                # Reset all state attributes
-                self._reset()
+            # Reset all state attributes
+            self._reset()
 
-    def speak_phrases(self, phrases: list[Phrase]) -> Generator[Word, None, bool]:
+    def speak_phrases(self, phrases: list[Phrase]) -> Generator[Word, None, None]:
         """
         Uses instances of class `Phrase` to allow for advanced SSML-based speech.
 
         This method converts the input text into speech using the specified instances of class `Phrase`. It yields the
         synthesized words one by one, along with their contextual information.
 
         Args:
@@ -169,81 +133,62 @@
 
         Yields:
             Word: A word with contextual information.
         """
         # Record the time at which the thread was initialized pre-lock, in order to account for future interruptions.
         init_time = time.perf_counter_ns()
 
-        # Create SSML markup for the given input_string, voice, and style
+        # Create SSML markup for the specified input_string, voice, and style
         ssml = self._create_advanced_ssml(phrases)
 
-        # Create a new thread to handle the speech synthesis
-        speech_thread = threading.Thread(target=self._speak, args=(ssml,), daemon=True)
-
         with self.__class__._speech_lock:
+            # Continuously monitor the synthesis progress in the main thread, yielding words as they are uttered
+            for word in self._callbacks_process(ssml, init_time):
+                logging.debug(f"SpeechSynthesisService synthesizer processed word: `{word}`")
+                yield word
 
-            # Do not run the listener if an interruption was raised after `init_time`.
-            if self._interrupt < init_time:
-
-                # Prepare an instance of TextToSpeechOutput while will receive values iteratively
-                output = TextToSpeechOutput(
-                    input_string=" ",
-                    timestamp=datetime.datetime.now(),
-                )
-                self._outputs.append(output)
-
-                # Starting the speech synthesizer
-                speech_thread.start()
-
-                # Set the speaking flag to True
-                self._speaking = True
-
-                # Continuously monitor the synthesis progress in the main thread, yielding words as they are uttered
-                for word in self._callbacks_process(output, init_time):
-                    logging.debug(f"TextToSpeech synthesizer processed word: `{word}`")
-                    yield word
-
-                # Reset all state attributes
-                self._reset()
+            # Reset all state attributes
+            self._reset()
 
     def _callback_completed(self, event: speechsdk.SessionEventArgs) -> None:
         """
         Callback function for synthesis completed event.
         Sets the synthesis completed flag to True.
 
         Args:
             event (speechsdk.SessionEventArgs): Event arguments containing information about the synthesis completed.
         """
-        self._synthesis_completed = True
+        self._stop_synthesis.set()
 
     def _callback_started(self, event: speechsdk.SessionEventArgs) -> None:
         """
         Callback function for synthesis started event. Signals that the synthesis process has started.
 
         Args:
             event (speechsdk.SessionEventArgs): Event arguments containing information about the synthesis started.
         """
+        self._start_synthesis_time = time.perf_counter_ns()
         self._start_synthesis.set()
 
     def _callback_word_boundary(self, event: speechsdk.SessionEventArgs) -> None:
         """
         Callback function for word boundary event.
         Appends the boundary information to the boundaries list.
 
         Args:
             event (speechsdk.SessionEventArgs): Event arguments containing information about the word boundary.
         """
         # Check if the type is not a sentence boundary
         if event.boundary_type != speechsdk.SpeechSynthesisBoundaryType.Sentence:
-
             # Add the event and timing information to the list of events
             self._events.append(
                 {
                     "event": event,
                     "time": 5e8 + 100 * event.audio_offset + 1e9 * event.duration.total_seconds() / event.word_length,
+                    "word": self._process_event(event=event, first_word=len(self._events) == 0),
                 }
             )
 
     def _callbacks_connect(self) -> None:
         """
         Connects the text-to-speech synthesizer events to their corresponding callbacks.
 
@@ -256,64 +201,54 @@
         # Connect the synthesis_word_boundary event to the _callback_word_boundary method
         self._synthesizer.synthesis_word_boundary.connect(self._callback_word_boundary)
 
         # Connect the synthesis_canceled and synthesis_completed events to the _callback_completed method
         self._synthesizer.synthesis_canceled.connect(self._callback_completed)
         self._synthesizer.synthesis_completed.connect(self._callback_completed)
 
-    def _callbacks_process(self, output: TextToSpeechOutput, init_time: int) -> Generator[Word, None, bool]:
+    def _callbacks_process(self, ssml: str, init_time: int) -> Generator[Word, None, None]:
         """
         Monitors the synthesis progress and updates the output accordingly.
 
-        This method continuously checks the synthesis progress and processes the boundaries. It updates the output
-        object with the processed words and yields them one by one.
+        This method continuously checks the synthesis progress and processes the boundaries. It then yields each
+        processed word one by one.
 
         Args:
-            output (TextToSpeechOutput): The output object to which the processed words will be added.
+            ssml (str): The SSML command to be sent to the Speech Synthesizer.
             init_time (int): The time at which the speech was initialized.
 
         Yields:
             Word: A word with contextual information.
-
-        Returns:
-            bool: True if the process completed successfully, False otherwise.
         """
         # Initialize variables
         idx = 0
-        success = False
 
-        # Wait until the synthesis has started before proceeding
-        self._start_synthesis.wait()
-        start_timer = time.perf_counter_ns()
+        self._synthesizer.speak_ssml_async(ssml)
 
-        logging.debug("TextToSpeech synthesizer started")
+        logging.debug("SpeechSynthesisService synthesizer started")
 
         # Continuously monitor the synthesis progress
-        while self._interrupt < init_time and (not self._synthesis_completed or idx < len(self._events)):
-
-            dt = time.perf_counter_ns() - start_timer
-
-            while self._interrupt < init_time and idx < len(self._events) and dt >= self._events[idx]["time"]:
-                word = self._process_boundary(idx=idx)
-                output.append(word)
+        while self._interrupt < init_time and (not self._stop_synthesis.is_set() or idx < len(self._events)):
+            while (
+                self._interrupt < init_time
+                and idx < len(self._events)
+                and time.perf_counter_ns() - self._start_synthesis_time >= self._events[idx]["time"]
+            ):
+                yield self._events[idx]["word"]
                 idx += 1
-                yield word
-
-        if self._interrupt >= init_time:
-            success = True
+            time.sleep(0.1)
 
         # Stop the synthesizer
         self._synthesizer.stop_speaking()
-        logging.debug("TextToSpeech synthesizer stopped")
-        return success
+        logging.debug("SpeechSynthesisService synthesizer stopped")
 
     @classmethod
     def _create_ssml(cls, text: str, voice: str, style: Optional[str] = None) -> str:
         """
-        Creates an SSML string from the given text, voice, and style.
+        Creates an SSML string from the specified text, voice, and style.
 
         Args:
             text (str): The input string that is to be converted into speech.
             voice (AzureNeuralVoice): The voice to be used.
             style (str, optional): The speaking style to be applied. Default is None.
 
         Returns:
@@ -338,19 +273,19 @@
         # Close the voice and speak tags and return the SSML string
         ssml += "</voice></speak>"
         return ssml
 
     @classmethod
     def _create_advanced_ssml(cls, phrases: list[Phrase]) -> str:
         """
-        Creates a more advanced SSML string from the given list of `Phrase` instances, that customizes the emphasis,
+        Creates a more advanced SSML string from the specified list of `Phrase` instances, that customizes the emphasis,
         style, pitch, and rate of speech on a sub-sentence level, including pitch contouring between phrases.
 
         Args:
-            phrases (List[Phrase]): Instances of class `Phrase` that contain data that can be converted into speech.
+            phrases (list[Phrase]): Instances of class `Phrase` that contain data that can be converted into speech.
 
         Returns:
             str: The SSML string.
         """
         # Start the SSML string with the required header
         ssml = (
             '<speak version="1.0" '
@@ -394,29 +329,29 @@
                 ssml += "</mstts:express-as>"
             ssml += "</voice>"
 
         # Close the voice and speak tags and return the SSML string
         ssml += "</speak>"
         return ssml
 
-    def _process_boundary(self, idx: int) -> Word:
+    def _process_event(self, event: speechsdk.SessionEventArgs, first_word: bool = False) -> Word:
         """
         Processes a synthesis boundary event and returns an instance of class Word.
 
         Args:
-            idx (int): The index of the word relative to the full text.
+            event (speechsdk.SessionEventArgs): An event passed to the WordBoundary handle.
+            first_word (bool): Indicate whether the words is the first in a sentence for correct whitespace handling.
 
         Returns:
             Word: The processed word with contextual information.
         """
-        event = self._events[idx]["event"]
         whitespace = ""
         if event.boundary_type == speechsdk.SpeechSynthesisBoundaryType.Word:
             category = WordCategory.WORD
-            if idx > 0:
+            if not first_word:
                 whitespace = " "
         elif event.boundary_type == speechsdk.SpeechSynthesisBoundaryType.Punctuation:
             category = WordCategory.PUNCTUATION
 
         word = Word(
             word=whitespace + event.text,
             offset=datetime.timedelta(microseconds=event.audio_offset / 10),
@@ -427,14 +362,12 @@
         return word
 
     def _reset(self) -> None:
         """
         Resets the state variables of the text-to-speech synthesizer, such as the list of events, synthesis timer, the
         interrupt flag, the speaking flag, the synthesis completed flag, and synthesis started flag.
         """
-        self._events: List[TimedEvent] = []
-        self._speaking = False
-        self._synthesis_completed = False
-        self._start_synthesis = threading.Event()
-
-    def _speak(self, ssml: str) -> None:
-        self._synthesizer.speak_ssml(ssml)
+        self._events: list[TimedEvent] = []
+        self._start_synthesis_time = 0
+        self._start_synthesis.clear()
+        self._stop_synthesis.clear()
+        self._new_events.clear()
```

### Comparing `BanterBot-0.0.8/banterbot/protos/memory_pb2.py` & `BanterBot-0.0.9/banterbot/protos/memory_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     b"\x03(\t\"6\n\x0bMemoryIndex\x12'\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x16.chat.MemoryIndexEntryb\x06proto3"
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "memory_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     _globals["_MESSAGE"]._serialized_start = 22
     _globals["_MESSAGE"]._serialized_end = 76
     _globals["_MEMORY"]._serialized_start = 78
     _globals["_MEMORY"]._serialized_end = 203
     _globals["_MEMORYINDEXENTRY"]._serialized_start = 205
     _globals["_MEMORYINDEXENTRY"]._serialized_end = 262
```

### Comparing `BanterBot-0.0.8/banterbot/utils/exceptions.py` & `BanterBot-0.0.9/banterbot/exceptions/format_mismatch_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Optional
 
 
 class FormatMismatchError(ValueError):
     """
     Exception raised when the output format from an external API does not match the expected format.
-
     This can be used to signal a mismatch in the expected structure or content type of the data returned from an API
     call.
 
     Args:
 
         expression (Optional[str]): The input expression or API response that caused the error. This is optional and
         used for providing context in the error message.
```

### Comparing `BanterBot-0.0.8/banterbot/utils/nlp.py` & `BanterBot-0.0.9/banterbot/utils/nlp.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.8/banterbot/utils/thread_queue.py` & `BanterBot-0.0.9/banterbot/utils/thread_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,24 @@
 import logging
 import threading
-from typing import List
 
 
 class ThreadQueue:
     """
     A class for managing and executing tasks in separate threads.
 
     This class maintains a queue of tasks to be executed. Each task is a Thread object, which is executed in its own
     thread. If there is a task in the queue that hasn't started executing yet, it will be prevented from running when a
     new task is added unless it is declared unskippable.
     """
 
     def __init__(self):
         logging.debug(f"ThreadQueue initialized")
         self._lock = threading.Lock()
-        self._event_queue: List[threading.Event] = []
-
-    def is_alive(self) -> bool:
-        """
-        Check if the last task in the queue is still running.
-
-        Returns:
-            bool: True if the last task is still running, False otherwise.
-        """
-        if not self._event_queue:
-            return False
-        else:
-            return not self._event_queue[-1].is_set()
+        self._event_queue: list[threading.Event] = []
 
     def add_task(self, thread: threading.Thread, unskippable: bool = False) -> None:
         """
         Add a new task to the queue.
 
         This method adds a new task to the queue and starts a wrapper thread to manage its execution. The wrapper thread
         is responsible for waiting for the previous task to complete, executing the current task if it is unskippable or
@@ -46,14 +33,26 @@
             self._event_queue.append(threading.Event())
 
         wrapper_thread = threading.Thread(
             target=self._thread_wrapper, args=(thread, index, unskippable), daemon=thread.daemon
         )
         wrapper_thread.start()
 
+    def is_alive(self) -> bool:
+        """
+        Check if the last task in the queue is still running.
+
+        Returns:
+            bool: True if the last task is still running, False otherwise.
+        """
+        if not self._event_queue:
+            return False
+        else:
+            return not self._event_queue[-1].is_set()
+
     def _thread_wrapper(self, thread: threading.Thread, index: int, unskippable: bool) -> None:
         """
         A wrapper function for executing threads in the queue.
 
         This function is responsible for waiting for the previous task to complete before starting the current task, and
         setting the event for the next task in the queue. If the current task is skippable and not the last task in the
         queue, it will not be executed.
```

### Comparing `BanterBot-0.0.8/setup.py` & `BanterBot-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 def run_tests():
     test_loader = unittest.TestLoader()
     test_suite = test_loader.discover("tests", pattern="test_*.py")
     return test_suite
 
 
-version = "0.0.8"
+version = "0.0.9"
 setup(
     author="Gabriel S. Cabrera",
     author_email="gabriel.sigurd.cabrera@gmail.com",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
```

