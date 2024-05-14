# Comparing `tmp/scwrypts-4.4.2.tar.gz` & `tmp/scwrypts-4.4.3.tar.gz`

## Comparing `scwrypts-4.4.2.tar` & `scwrypts-4.4.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/env.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/data/__init__.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/data/converter.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/data/test_converter.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/fzf/__init__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/fzf/client.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/client.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/conftest.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/test_client.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/directus/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/directus/client.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/directus/collections.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/directus/conftest.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/directus/fields.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/directus/graphql.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/directus/test_client.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/directus/test_graphql.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/discord/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/discord/client.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/discord/conftest.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/discord/send_message.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/discord/test_client.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/discord/test_send_message.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/linear/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/linear/client.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/linear/conftest.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/linear/graphql.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/linear/test_client.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/http/linear/test_graphql.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/io/__init__.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/io/combined_io_stream.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/redis/__init__.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/redis/client.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/scwrypts/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/scwrypts/exceptions.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/scwrypts/execute.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/scwrypts/interactive.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/scwrypts/scwrypts.py
--rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/scwrypts/test_scwrypts.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/test/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/test/character_set.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/test/exceptions.py
--rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/test/generate.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/test/test_generate.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/twilio/__init__.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/twilio/client.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scwrypts-4.4.2/scwrypts/twilio/send_sms.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 scwrypts-4.4.2/.gitignore
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 scwrypts-4.4.2/README.md
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 scwrypts-4.4.2/pyproject.toml
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 scwrypts-4.4.2/PKG-INFO
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/env.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/data/__init__.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/data/converter.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/data/test_converter.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/fzf/__init__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/fzf/client.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/client.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/conftest.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/test_client.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/directus/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/directus/client.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/directus/collections.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/directus/conftest.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/directus/fields.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/directus/graphql.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/directus/test_client.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/directus/test_graphql.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/discord/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/discord/client.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/discord/conftest.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/discord/send_message.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/discord/test_client.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/discord/test_send_message.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/linear/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/linear/client.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/linear/conftest.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/linear/graphql.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/linear/test_client.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/http/linear/test_graphql.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/io/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/io/combined_io_stream.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/redis/__init__.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/redis/client.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/scwrypts/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/scwrypts/exceptions.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/scwrypts/execute.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/scwrypts/interactive.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/scwrypts/scwrypts.py
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/scwrypts/test_scwrypts.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/test/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/test/character_set.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/test/exceptions.py
+-rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/test/generate.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/test/test_generate.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/twilio/__init__.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/twilio/client.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scwrypts-4.4.3/scwrypts/twilio/send_sms.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 scwrypts-4.4.3/.gitignore
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 scwrypts-4.4.3/README.md
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 scwrypts-4.4.3/pyproject.toml
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 scwrypts-4.4.3/PKG-INFO
```

### Comparing `scwrypts-4.4.2/scwrypts/data/converter.py` & `scwrypts-4.4.3/scwrypts/data/converter.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/data/test_converter.py` & `scwrypts-4.4.3/scwrypts/data/test_converter.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/fzf/client.py` & `scwrypts-4.4.3/scwrypts/fzf/client.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/client.py` & `scwrypts-4.4.3/scwrypts/http/client.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/conftest.py` & `scwrypts-4.4.3/scwrypts/http/conftest.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/test_client.py` & `scwrypts-4.4.3/scwrypts/http/test_client.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/directus/__init__.py` & `scwrypts-4.4.3/scwrypts/http/directus/__init__.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/directus/test_client.py` & `scwrypts-4.4.3/scwrypts/http/directus/test_client.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/directus/test_graphql.py` & `scwrypts-4.4.3/scwrypts/http/directus/test_graphql.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/discord/conftest.py` & `scwrypts-4.4.3/scwrypts/http/discord/conftest.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/discord/send_message.py` & `scwrypts-4.4.3/scwrypts/http/discord/send_message.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/discord/test_client.py` & `scwrypts-4.4.3/scwrypts/http/discord/test_client.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/discord/test_send_message.py` & `scwrypts-4.4.3/scwrypts/http/discord/test_send_message.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/linear/conftest.py` & `scwrypts-4.4.3/scwrypts/http/linear/conftest.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/linear/test_client.py` & `scwrypts-4.4.3/scwrypts/http/linear/test_client.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/http/linear/test_graphql.py` & `scwrypts-4.4.3/scwrypts/http/linear/test_graphql.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/io/combined_io_stream.py` & `scwrypts-4.4.3/scwrypts/io/combined_io_stream.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/scwrypts/__init__.py` & `scwrypts-4.4.3/scwrypts/scwrypts/__init__.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/scwrypts/exceptions.py` & `scwrypts-4.4.3/scwrypts/scwrypts/exceptions.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/scwrypts/execute.py` & `scwrypts-4.4.3/scwrypts/scwrypts/execute.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/scwrypts/interactive.py` & `scwrypts-4.4.3/scwrypts/scwrypts/interactive.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/scwrypts/scwrypts.py` & `scwrypts-4.4.3/scwrypts/scwrypts/scwrypts.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/scwrypts/test_scwrypts.py` & `scwrypts-4.4.3/scwrypts/scwrypts/test_scwrypts.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/test/generate.py` & `scwrypts-4.4.3/scwrypts/test/generate.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/test/test_generate.py` & `scwrypts-4.4.3/scwrypts/test/test_generate.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/scwrypts/twilio/send_sms.py` & `scwrypts-4.4.3/scwrypts/twilio/send_sms.py`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/pyproject.toml` & `scwrypts-4.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scwrypts-4.4.2/PKG-INFO` & `scwrypts-4.4.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scwrypts
-Version: 4.4.2
+Version: 4.4.3
 Summary: scwrypts library and invoker
 Project-URL: homepage, https://github.com/wrynegade/scwrypts
 Project-URL: issues, https://github.com/wrynegade/scwrypts/issues
 Author-email: yage <yage@yage.io>
 License-Expression: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

