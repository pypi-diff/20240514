# Comparing `tmp/codedepot_ai-0.0.23.tar.gz` & `tmp/codedepot_ai-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_ai-0.0.23.tar", last modified: Tue May 14 09:47:48 2024, max compression
+gzip compressed data, was "codedepot_ai-0.0.24.tar", last modified: Tue May 14 10:11:40 2024, max compression
```

## Comparing `codedepot_ai-0.0.23.tar` & `codedepot_ai-0.0.24.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       48 2024-05-13 13:26:24.698707 codedepot_ai-0.0.23/README.md
--rw-r--r--   0        0        0        0 2024-05-13 13:14:58.280759 codedepot_ai-0.0.23/ai/__init__.py
--rw-r--r--   0        0        0    15091 2024-05-13 14:01:29.258676 codedepot_ai-0.0.23/ai/api.py
--rw-r--r--   0        0        0      624 2024-05-13 13:14:58.281422 codedepot_ai-0.0.23/ai/cluster_spec.py
--rw-r--r--   0        0        0     3947 2024-05-13 13:28:42.697260 codedepot_ai-0.0.23/ai/config.py
--rw-r--r--   0        0        0      507 2024-05-13 13:14:58.282241 codedepot_ai-0.0.23/ai/jobfile.py
--rw-r--r--   0        0        0     5553 2024-05-13 13:52:54.978959 codedepot_ai-0.0.23/ai/main.py
--rw-r--r--   0        0        0      616 2024-05-13 13:14:58.283186 codedepot_ai-0.0.23/ai/provider_spec.py
--rw-r--r--   0        0        0      761 2024-05-14 09:47:48.443878 codedepot_ai-0.0.23/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 13:14:58.284442 codedepot_ai-0.0.23/test/__init__.py
--rw-r--r--   0        0        0       86 2024-05-13 13:14:58.284960 codedepot_ai-0.0.23/test/resources/cluster_test.yaml
--rw-r--r--   0        0        0       87 2024-05-13 13:14:58.285531 codedepot_ai-0.0.23/test/resources/config.json
--rw-r--r--   0        0        0       80 2024-05-13 13:14:58.285845 codedepot_ai-0.0.23/test/resources/local_cred.json
--rw-r--r--   0        0        0       94 2024-05-13 13:30:47.773285 codedepot_ai-0.0.23/test/resources/provider_test.yaml
--rw-r--r--   0        0        0        0 2024-05-13 13:14:58.286084 codedepot_ai-0.0.23/test/test_client.py
--rw-r--r--   0        0        0      405 2024-05-13 13:25:27.013607 codedepot_ai-0.0.23/test/test_provider.py
--rw-r--r--   0        0        0      654 2024-05-13 13:28:42.702562 codedepot_ai-0.0.23/test/utils.py
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 codedepot_ai-0.0.23/PKG-INFO
+-rw-r--r--   0        0        0       48 2024-05-13 13:26:24.698707 codedepot_ai-0.0.24/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 13:14:58.280759 codedepot_ai-0.0.24/ai/__init__.py
+-rw-r--r--   0        0        0    15091 2024-05-13 14:01:29.258676 codedepot_ai-0.0.24/ai/api.py
+-rw-r--r--   0        0        0      624 2024-05-13 13:14:58.281422 codedepot_ai-0.0.24/ai/cluster_spec.py
+-rw-r--r--   0        0        0     3947 2024-05-13 13:28:42.697260 codedepot_ai-0.0.24/ai/config.py
+-rw-r--r--   0        0        0      507 2024-05-13 13:14:58.282241 codedepot_ai-0.0.24/ai/jobfile.py
+-rw-r--r--   0        0        0     5553 2024-05-14 10:11:08.702294 codedepot_ai-0.0.24/ai/main.py
+-rw-r--r--   0        0        0      616 2024-05-13 13:14:58.283186 codedepot_ai-0.0.24/ai/provider_spec.py
+-rw-r--r--   0        0        0      792 2024-05-14 10:11:40.818212 codedepot_ai-0.0.24/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 13:14:58.284442 codedepot_ai-0.0.24/test/__init__.py
+-rw-r--r--   0        0        0       86 2024-05-13 13:14:58.284960 codedepot_ai-0.0.24/test/resources/cluster_test.yaml
+-rw-r--r--   0        0        0       87 2024-05-13 13:14:58.285531 codedepot_ai-0.0.24/test/resources/config.json
+-rw-r--r--   0        0        0       80 2024-05-13 13:14:58.285845 codedepot_ai-0.0.24/test/resources/local_cred.json
+-rw-r--r--   0        0        0       94 2024-05-13 13:30:47.773285 codedepot_ai-0.0.24/test/resources/provider_test.yaml
+-rw-r--r--   0        0        0        0 2024-05-13 13:14:58.286084 codedepot_ai-0.0.24/test/test_client.py
+-rw-r--r--   0        0        0      405 2024-05-13 13:25:27.013607 codedepot_ai-0.0.24/test/test_provider.py
+-rw-r--r--   0        0        0      654 2024-05-13 13:28:42.702562 codedepot_ai-0.0.24/test/utils.py
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 codedepot_ai-0.0.24/PKG-INFO
```

### Comparing `codedepot_ai-0.0.23/ai/api.py` & `codedepot_ai-0.0.24/ai/api.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.0.23/ai/cluster_spec.py` & `codedepot_ai-0.0.24/ai/cluster_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.0.23/ai/config.py` & `codedepot_ai-0.0.24/ai/config.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.0.23/ai/main.py` & `codedepot_ai-0.0.24/ai/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     return parser.parse_args()
 
 
 
 def main():
     args = parse_args()
     if args.version:
-        print("0.0.23")
+        print("0.0.24")
         return
 
     if args.command == 'login':
         AIConfig.create()
         return
 
     config = AIConfig.default()
```

### Comparing `codedepot_ai-0.0.23/ai/provider_spec.py` & `codedepot_ai-0.0.24/ai/provider_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.0.23/pyproject.toml` & `codedepot_ai-0.0.24/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "codedepot-ai"
-version = "0.0.23"
+version = "0.0.24"
 description = "Job run support for Git AI"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -21,14 +21,15 @@
     "pyaml",
     "pydantic",
     "pygit2",
     "requests",
     "inquirer",
     "codedepot-git-ai>=0.0.25",
     "ai_api>=1.0.9",
+    "codedepot-ai-api>=1.0.9",
 ]
 
 [project.urls]
 Homepage = "https://github.com/codedepotai/git-ai"
 
 [project.scripts]
 ai = "ai.main:main"
```

### Comparing `codedepot_ai-0.0.23/test/utils.py` & `codedepot_ai-0.0.24/test/utils.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.0.23/PKG-INFO` & `codedepot_ai-0.0.24/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-ai
-Version: 0.0.23
+Version: 0.0.24
 Summary: Job run support for Git AI
 Author-Email: CodeDepot <contact@codedepot.ai>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Requires-Python: >=3.10
@@ -14,12 +14,13 @@
 Requires-Dist: pyaml
 Requires-Dist: pydantic
 Requires-Dist: pygit2
 Requires-Dist: requests
 Requires-Dist: inquirer
 Requires-Dist: codedepot-git-ai>=0.0.25
 Requires-Dist: ai_api>=1.0.9
+Requires-Dist: codedepot-ai-api>=1.0.9
 Description-Content-Type: text/markdown
 
 # AI
 
 This is the ai client. More docs to come.
```

