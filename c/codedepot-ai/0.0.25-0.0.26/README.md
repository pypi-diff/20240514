# Comparing `tmp/codedepot_ai-0.0.25.tar.gz` & `tmp/codedepot_ai-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_ai-0.0.25.tar", last modified: Tue May 14 10:13:36 2024, max compression
+gzip compressed data, was "codedepot_ai-0.0.26.tar", last modified: Tue May 14 16:48:34 2024, max compression
```

## Comparing `codedepot_ai-0.0.25.tar` & `codedepot_ai-0.0.26.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       48 2024-05-13 13:26:24.698707 codedepot_ai-0.0.25/README.md
--rw-r--r--   0        0        0        0 2024-05-13 13:14:58.280759 codedepot_ai-0.0.25/ai/__init__.py
--rw-r--r--   0        0        0    15091 2024-05-13 14:01:29.258676 codedepot_ai-0.0.25/ai/api.py
--rw-r--r--   0        0        0      624 2024-05-13 13:14:58.281422 codedepot_ai-0.0.25/ai/cluster_spec.py
--rw-r--r--   0        0        0     3947 2024-05-13 13:28:42.697260 codedepot_ai-0.0.25/ai/config.py
--rw-r--r--   0        0        0      507 2024-05-13 13:14:58.282241 codedepot_ai-0.0.25/ai/jobfile.py
--rw-r--r--   0        0        0     5553 2024-05-14 10:13:19.935270 codedepot_ai-0.0.25/ai/main.py
--rw-r--r--   0        0        0      616 2024-05-13 13:14:58.283186 codedepot_ai-0.0.25/ai/provider_spec.py
--rw-r--r--   0        0        0      771 2024-05-14 10:13:36.846414 codedepot_ai-0.0.25/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 13:14:58.284442 codedepot_ai-0.0.25/test/__init__.py
--rw-r--r--   0        0        0       86 2024-05-13 13:14:58.284960 codedepot_ai-0.0.25/test/resources/cluster_test.yaml
--rw-r--r--   0        0        0       87 2024-05-13 13:14:58.285531 codedepot_ai-0.0.25/test/resources/config.json
--rw-r--r--   0        0        0       80 2024-05-13 13:14:58.285845 codedepot_ai-0.0.25/test/resources/local_cred.json
--rw-r--r--   0        0        0       94 2024-05-13 13:30:47.773285 codedepot_ai-0.0.25/test/resources/provider_test.yaml
--rw-r--r--   0        0        0        0 2024-05-13 13:14:58.286084 codedepot_ai-0.0.25/test/test_client.py
--rw-r--r--   0        0        0      405 2024-05-13 13:25:27.013607 codedepot_ai-0.0.25/test/test_provider.py
--rw-r--r--   0        0        0      654 2024-05-13 13:28:42.702562 codedepot_ai-0.0.25/test/utils.py
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 codedepot_ai-0.0.25/PKG-INFO
+-rw-r--r--   0        0        0       48 2024-05-13 13:26:24.698707 codedepot_ai-0.0.26/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 13:14:58.280759 codedepot_ai-0.0.26/ai/__init__.py
+-rw-r--r--   0        0        0    15093 2024-05-14 16:47:35.661693 codedepot_ai-0.0.26/ai/api.py
+-rw-r--r--   0        0        0      624 2024-05-13 13:14:58.281422 codedepot_ai-0.0.26/ai/cluster_spec.py
+-rw-r--r--   0        0        0     3947 2024-05-13 13:28:42.697260 codedepot_ai-0.0.26/ai/config.py
+-rw-r--r--   0        0        0      507 2024-05-13 13:14:58.282241 codedepot_ai-0.0.26/ai/jobfile.py
+-rw-r--r--   0        0        0     5553 2024-05-14 16:47:55.946487 codedepot_ai-0.0.26/ai/main.py
+-rw-r--r--   0        0        0      616 2024-05-13 13:14:58.283186 codedepot_ai-0.0.26/ai/provider_spec.py
+-rw-r--r--   0        0        0      771 2024-05-14 16:48:34.507972 codedepot_ai-0.0.26/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 13:14:58.284442 codedepot_ai-0.0.26/test/__init__.py
+-rw-r--r--   0        0        0       86 2024-05-13 13:14:58.284960 codedepot_ai-0.0.26/test/resources/cluster_test.yaml
+-rw-r--r--   0        0        0       87 2024-05-13 13:14:58.285531 codedepot_ai-0.0.26/test/resources/config.json
+-rw-r--r--   0        0        0       80 2024-05-13 13:14:58.285845 codedepot_ai-0.0.26/test/resources/local_cred.json
+-rw-r--r--   0        0        0       94 2024-05-13 13:30:47.773285 codedepot_ai-0.0.26/test/resources/provider_test.yaml
+-rw-r--r--   0        0        0        0 2024-05-13 13:14:58.286084 codedepot_ai-0.0.26/test/test_client.py
+-rw-r--r--   0        0        0      405 2024-05-13 13:25:27.013607 codedepot_ai-0.0.26/test/test_provider.py
+-rw-r--r--   0        0        0      654 2024-05-13 13:28:42.702562 codedepot_ai-0.0.26/test/utils.py
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 codedepot_ai-0.0.26/PKG-INFO
```

### Comparing `codedepot_ai-0.0.25/ai/api.py` & `codedepot_ai-0.0.26/ai/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     print(table)
 
 
 def list_jobs(config: AIConfig):
     response = config.api().list_job_instances_job_instances_get()
     table = PrettyTable()
     table.field_names = ['Name', 'Status', 'Repository', 'Cluster']
-    table._max_width = {"Name": 10, "Repository": 20}
+    # table._max_width = {"Name": 10, "Repository": 20}
     for job in response:
         table.add_row([job.name, job.status,
                       job.repository_url, job.cluster_name])
     print(table)
 
 
 def stop_job(config: AIConfig, job_name: str):
```

### Comparing `codedepot_ai-0.0.25/ai/cluster_spec.py` & `codedepot_ai-0.0.26/ai/cluster_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.0.25/ai/config.py` & `codedepot_ai-0.0.26/ai/config.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.0.25/ai/main.py` & `codedepot_ai-0.0.26/ai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     return parser.parse_args()
 
 
 
 def main():
     args = parse_args()
     if args.version:
-        print("0.0.25")
+        print("0.0.26")
         return
 
     if args.command == 'login':
         AIConfig.create()
         return
 
     config = AIConfig.default()
```

### Comparing `codedepot_ai-0.0.25/ai/provider_spec.py` & `codedepot_ai-0.0.26/ai/provider_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.0.25/pyproject.toml` & `codedepot_ai-0.0.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "codedepot-ai"
-version = "0.0.25"
+version = "0.0.26"
 description = "Job run support for Git AI"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `codedepot_ai-0.0.25/test/utils.py` & `codedepot_ai-0.0.26/test/utils.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.0.25/PKG-INFO` & `codedepot_ai-0.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-ai
-Version: 0.0.25
+Version: 0.0.26
 Summary: Job run support for Git AI
 Author-Email: CodeDepot <contact@codedepot.ai>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Requires-Python: >=3.10
```

