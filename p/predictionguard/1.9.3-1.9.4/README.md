# Comparing `tmp/predictionguard-1.9.3.tar.gz` & `tmp/predictionguard-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predictionguard-1.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "predictionguard-1.9.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `predictionguard-1.9.3.tar` & `predictionguard-1.9.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2024-01-02 16:12:43.933648 predictionguard-1.9.3/LICENSE
--rw-r--r--   0        0        0     1878 2024-01-02 16:12:43.933648 predictionguard-1.9.3/README.md
--rw-r--r--   0        0        0     3256 2024-01-02 16:12:43.933648 predictionguard-1.9.3/examples/sentiment.ipynb
--rw-r--r--   0        0        0      188 2024-04-22 20:08:18.083673 predictionguard-1.9.3/predictionguard/__init__.py
--rw-r--r--   0        0        0    19409 2024-04-22 20:08:18.083673 predictionguard-1.9.3/predictionguard/client.py
--rw-r--r--   0        0        0      483 2024-01-02 16:12:43.933648 predictionguard-1.9.3/pyproject.toml
--rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 predictionguard-1.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-02 16:12:43.933648 predictionguard-1.9.4/LICENSE
+-rw-r--r--   0        0        0     1878 2024-01-02 16:12:43.933648 predictionguard-1.9.4/README.md
+-rw-r--r--   0        0        0     3256 2024-01-02 16:12:43.933648 predictionguard-1.9.4/examples/sentiment.ipynb
+-rw-r--r--   0        0        0      188 2024-05-14 13:28:36.671984 predictionguard-1.9.4/predictionguard/__init__.py
+-rw-r--r--   0        0        0    19408 2024-05-14 13:28:54.507699 predictionguard-1.9.4/predictionguard/client.py
+-rw-r--r--   0        0        0      483 2024-01-02 16:12:43.933648 predictionguard-1.9.4/pyproject.toml
+-rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 predictionguard-1.9.4/PKG-INFO
```

### Comparing `predictionguard-1.9.3/LICENSE` & `predictionguard-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `predictionguard-1.9.3/README.md` & `predictionguard-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `predictionguard-1.9.3/examples/sentiment.ipynb` & `predictionguard-1.9.4/examples/sentiment.ipynb`

 * *Files identical despite different names*

### Comparing `predictionguard-1.9.3/predictionguard/client.py` & `predictionguard-1.9.4/predictionguard/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,15 @@
     @classmethod
     def list_models(self) -> List[str]:
         # Commented out parts are there for easier fix when
         # functionality for this call on chat endpoint added
         model_list = [
             "deepseek-coder-6.7b-instruct", 
             "Hermes-2-Pro-Mistral-7B", 
-            "Meta-Llama-3-8B-Instruct", 
+            "Hermes-2-Pro-Llama-3-8B", 
             "Neural-Chat-7B", 
             "Yi-34B-Chat"
             ]
 
         # Make sure we can connect to prediction guard.
         # self._connect()
```

### Comparing `predictionguard-1.9.3/PKG-INFO` & `predictionguard-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictionguard
-Version: 1.9.3
+Version: 1.9.4
 Summary: Create controlled and compliant AI systems with PredictionGuard.
 Author-email: Daniel Whitenack <dan@predictionguard.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: tabulate >=0.8.10
 Requires-Dist: requests >=2.27.1
 Project-URL: Home, https://predictionguard.com
```

