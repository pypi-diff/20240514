# Comparing `tmp/libwebarena-0.0.2.tar.gz` & `tmp/libwebarena-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libwebarena-0.0.2.tar", last modified: Tue Mar 12 18:34:44 2024, max compression
+gzip compressed data, was "libwebarena-0.0.3.tar", last modified: Tue May 14 19:49:53 2024, max compression
```

## Comparing `libwebarena-0.0.2.tar` & `libwebarena-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:34:44.559884 libwebarena-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-12 18:34:40.000000 libwebarena-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8935 2024-03-12 18:34:44.559884 libwebarena-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-03-12 18:34:40.000000 libwebarena-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:34:44.555884 libwebarena-0.0.2/agent/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-12 18:34:40.000000 libwebarena-0.0.2/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-03-12 18:34:40.000000 libwebarena-0.0.2/agent/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:34:44.555884 libwebarena-0.0.2/browser_env/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-12 18:34:40.000000 libwebarena-0.0.2/browser_env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53946 2024-03-12 18:34:40.000000 libwebarena-0.0.2/browser_env/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-03-12 18:34:40.000000 libwebarena-0.0.2/browser_env/async_envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-12 18:34:40.000000 libwebarena-0.0.2/browser_env/auto_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-03-12 18:34:40.000000 libwebarena-0.0.2/browser_env/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-12 18:34:40.000000 libwebarena-0.0.2/browser_env/env_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-03-12 18:34:40.000000 libwebarena-0.0.2/browser_env/envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-03-12 18:34:40.000000 libwebarena-0.0.2/browser_env/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26617 2024-03-12 18:34:40.000000 libwebarena-0.0.2/browser_env/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 18:34:40.000000 libwebarena-0.0.2/browser_env/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-12 18:34:40.000000 libwebarena-0.0.2/browser_env/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-12 18:34:40.000000 libwebarena-0.0.2/browser_env/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:34:44.555884 libwebarena-0.0.2/config_files/
--rw-r--r--   0 runner    (1001) docker     (127)   880776 2024-03-12 18:34:40.000000 libwebarena-0.0.2/config_files/test.raw.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:34:44.559884 libwebarena-0.0.2/evaluation_harness/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-12 18:34:40.000000 libwebarena-0.0.2/evaluation_harness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-03-12 18:34:40.000000 libwebarena-0.0.2/evaluation_harness/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-03-12 18:34:40.000000 libwebarena-0.0.2/evaluation_harness/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:34:44.559884 libwebarena-0.0.2/libwebarena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8935 2024-03-12 18:34:44.000000 libwebarena-0.0.2/libwebarena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-12 18:34:44.000000 libwebarena-0.0.2/libwebarena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 18:34:44.000000 libwebarena-0.0.2/libwebarena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-12 18:34:44.000000 libwebarena-0.0.2/libwebarena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-12 18:34:44.000000 libwebarena-0.0.2/libwebarena.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:34:44.559884 libwebarena-0.0.2/llms/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-12 18:34:40.000000 libwebarena-0.0.2/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-12 18:34:40.000000 libwebarena-0.0.2/llms/lm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:34:44.559884 libwebarena-0.0.2/llms/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-12 18:34:40.000000 libwebarena-0.0.2/llms/providers/hf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-03-12 18:34:40.000000 libwebarena-0.0.2/llms/providers/openai_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-12 18:34:40.000000 libwebarena-0.0.2/llms/tokenizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-03-12 18:34:40.000000 libwebarena-0.0.2/llms/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-12 18:34:40.000000 libwebarena-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-12 18:34:40.000000 libwebarena-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 18:34:44.559884 libwebarena-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-12 18:34:40.000000 libwebarena-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:49:53.030132 libwebarena-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:49:49.000000 libwebarena-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-14 19:49:53.030132 libwebarena-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-14 19:49:49.000000 libwebarena-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:49:53.022132 libwebarena-0.0.3/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-14 19:49:49.000000 libwebarena-0.0.3/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-14 19:49:49.000000 libwebarena-0.0.3/agent/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:49:53.026132 libwebarena-0.0.3/browser_env/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-14 19:49:49.000000 libwebarena-0.0.3/browser_env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53946 2024-05-14 19:49:49.000000 libwebarena-0.0.3/browser_env/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-14 19:49:49.000000 libwebarena-0.0.3/browser_env/async_envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-14 19:49:49.000000 libwebarena-0.0.3/browser_env/auto_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-14 19:49:49.000000 libwebarena-0.0.3/browser_env/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-14 19:49:49.000000 libwebarena-0.0.3/browser_env/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-14 19:49:49.000000 libwebarena-0.0.3/browser_env/envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-05-14 19:49:49.000000 libwebarena-0.0.3/browser_env/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26617 2024-05-14 19:49:49.000000 libwebarena-0.0.3/browser_env/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:49:49.000000 libwebarena-0.0.3/browser_env/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-14 19:49:49.000000 libwebarena-0.0.3/browser_env/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-14 19:49:49.000000 libwebarena-0.0.3/browser_env/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:49:53.026132 libwebarena-0.0.3/config_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   880776 2024-05-14 19:49:49.000000 libwebarena-0.0.3/config_files/test.raw.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:49:53.026132 libwebarena-0.0.3/evaluation_harness/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 19:49:49.000000 libwebarena-0.0.3/evaluation_harness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-05-14 19:49:49.000000 libwebarena-0.0.3/evaluation_harness/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-05-14 19:49:49.000000 libwebarena-0.0.3/evaluation_harness/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:49:53.030132 libwebarena-0.0.3/libwebarena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-14 19:49:53.000000 libwebarena-0.0.3/libwebarena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-14 19:49:53.000000 libwebarena-0.0.3/libwebarena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:49:53.000000 libwebarena-0.0.3/libwebarena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 19:49:53.000000 libwebarena-0.0.3/libwebarena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 19:49:53.000000 libwebarena-0.0.3/libwebarena.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:49:53.030132 libwebarena-0.0.3/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-14 19:49:49.000000 libwebarena-0.0.3/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-14 19:49:49.000000 libwebarena-0.0.3/llms/lm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:49:53.030132 libwebarena-0.0.3/llms/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 19:49:49.000000 libwebarena-0.0.3/llms/providers/hf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-05-14 19:49:49.000000 libwebarena-0.0.3/llms/providers/openai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-14 19:49:49.000000 libwebarena-0.0.3/llms/tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-14 19:49:49.000000 libwebarena-0.0.3/llms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-14 19:49:49.000000 libwebarena-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 19:49:49.000000 libwebarena-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:49:53.030132 libwebarena-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 19:49:49.000000 libwebarena-0.0.3/setup.py
```

### Comparing `libwebarena-0.0.2/LICENSE` & `libwebarena-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/agent/agent.py` & `libwebarena-0.0.3/agent/agent.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/browser_env/__init__.py` & `libwebarena-0.0.3/browser_env/__init__.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/browser_env/actions.py` & `libwebarena-0.0.3/browser_env/actions.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/browser_env/async_envs.py` & `libwebarena-0.0.3/browser_env/async_envs.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/browser_env/auto_login.py` & `libwebarena-0.0.3/browser_env/auto_login.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/browser_env/constants.py` & `libwebarena-0.0.3/browser_env/constants.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/browser_env/env_config.py` & `libwebarena-0.0.3/browser_env/env_config.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/browser_env/envs.py` & `libwebarena-0.0.3/browser_env/envs.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/browser_env/helper_functions.py` & `libwebarena-0.0.3/browser_env/helper_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         new_content = f"<h2>New Page</h2>\n"
         new_content += f"<h3 class='url'><a href={state_info['info']['page'].url}>URL: {state_info['info']['page'].url}</a></h3>\n"
         new_content += f"<div class='state_obv'><pre>{text_obs}</pre><div>\n"
 
         if render_screenshot:
             # image observation
             img_obs = observation["image"]
-            image = Image.fromarray(img_obs)
+            image = Image.fromarray(img_obs)  # type:ignore
             byte_io = io.BytesIO()
             image.save(byte_io, format="PNG")
             byte_io.seek(0)
             image_bytes = base64.b64encode(byte_io.read())
             image_str = image_bytes.decode("utf-8")
             new_content += f"<img src='data:image/png;base64,{image_str}' style='width:50vw; height:auto;'/>\n"
```

### Comparing `libwebarena-0.0.2/browser_env/processors.py` & `libwebarena-0.0.3/browser_env/processors.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/browser_env/utils.py` & `libwebarena-0.0.3/browser_env/utils.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/config_files/test.raw.json` & `libwebarena-0.0.3/config_files/test.raw.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998588875205255%*

 * *Differences: {'240': "{'instantiation_dict': {'product_category': 'competitive swimwear'}, 'intent': 'I am "*

 * *        'doing a market survey for one stop market, show me the most expensive product from '*

 * *        "competitive swimwear category'}",*

 * * '353': "{'instantiation_dict': {'product_category': 'competitive swimwear'}, 'intent': 'List "*

 * *        "products from competitive swimwear category by ascending price'}"}*

```diff
@@ -7636,17 +7636,17 @@
             "program_html": [],
             "reference_answers": null,
             "reference_url": "__SHOPPING__/women-cross-flower-beachwear-tankini-bandeau-bandage-bikini-set-push-up-swimwear-bathing-suit-two-pieces-swimsuits.html",
             "url_note": "GOLD in PRED"
         },
         "geolocation": null,
         "instantiation_dict": {
-            "product_category": "competative swimwear"
+            "product_category": "competitive swimwear"
         },
-        "intent": "I am doing a market survey for one stop market, show me the most expensive product from competative swimwear category",
+        "intent": "I am doing a market survey for one stop market, show me the most expensive product from competitive swimwear category",
         "intent_template": "I am doing a market survey for one stop market, show me the most expensive product from {{product_category}} category",
         "intent_template_id": 138,
         "require_login": true,
         "require_reset": false,
         "sites": [
             "shopping"
         ],
@@ -10985,17 +10985,17 @@
             "reference_answers": null,
             "reference_url": "__SHOPPING__/clothing-shoes-jewelry/sport-specific-clothing/competitive-swimwear.html?product_list_order=price",
             "url_note": "GOLD in PRED"
         },
         "geolocation": null,
         "instantiation_dict": {
             "order": "ascending",
-            "product_category": "competative swimwear"
+            "product_category": "competitive swimwear"
         },
-        "intent": "List products from competative swimwear category by ascending price",
+        "intent": "List products from competitive swimwear category by ascending price",
         "intent_template": "List products from {{product_category}} category by {{order}} price",
         "intent_template_id": 137,
         "require_login": true,
         "require_reset": false,
         "sites": [
             "shopping"
         ],
```

### Comparing `libwebarena-0.0.2/evaluation_harness/evaluators.py` & `libwebarena-0.0.3/evaluation_harness/evaluators.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/evaluation_harness/helper_functions.py` & `libwebarena-0.0.3/evaluation_harness/helper_functions.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/libwebarena.egg-info/SOURCES.txt` & `libwebarena-0.0.3/libwebarena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/llms/lm_config.py` & `libwebarena-0.0.3/llms/lm_config.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/llms/providers/hf_utils.py` & `libwebarena-0.0.3/llms/providers/hf_utils.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/llms/providers/openai_utils.py` & `libwebarena-0.0.3/llms/providers/openai_utils.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/llms/tokenizers.py` & `libwebarena-0.0.3/llms/tokenizers.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/llms/utils.py` & `libwebarena-0.0.3/llms/utils.py`

 * *Files identical despite different names*

### Comparing `libwebarena-0.0.2/pyproject.toml` & `libwebarena-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "libwebarena"
-version = "0.0.2"
+version = "0.0.3"
 description = "This is an unofficial, use-at-your-own risks port of the webarena benchmark, for use as a standalone library package."
 readme = "README.md"
 requires-python = ">=3.7, <4"
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

