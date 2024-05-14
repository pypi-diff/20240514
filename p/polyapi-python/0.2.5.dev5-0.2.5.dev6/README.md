# Comparing `tmp/polyapi_python-0.2.5.dev5.tar.gz` & `tmp/polyapi_python-0.2.5.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi_python-0.2.5.dev5.tar", last modified: Tue May 14 17:50:58 2024, max compression
+gzip compressed data, was "polyapi_python-0.2.5.dev6.tar", last modified: Tue May 14 19:35:14 2024, max compression
```

## Comparing `polyapi_python-0.2.5.dev5.tar` & `polyapi_python-0.2.5.dev6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:58.044237 polyapi_python-0.2.5.dev5/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-14 17:50:58.044237 polyapi_python-0.2.5.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:58.040237 polyapi_python-0.2.5.dev5/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/rendered_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:58.044237 polyapi_python-0.2.5.dev5/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-14 17:50:58.000000 polyapi_python-0.2.5.dev5/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-14 17:50:58.000000 polyapi_python-0.2.5.dev5/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:50:58.000000 polyapi_python-0.2.5.dev5/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 17:50:58.000000 polyapi_python-0.2.5.dev5/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 17:50:58.000000 polyapi_python-0.2.5.dev5/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 17:50:58.044237 polyapi_python-0.2.5.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:58.044237 polyapi_python-0.2.5.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/tests/test_rendered_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-14 17:50:53.000000 polyapi_python-0.2.5.dev5/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:14.559930 polyapi_python-0.2.5.dev6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-14 19:35:14.559930 polyapi_python-0.2.5.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:14.555930 polyapi_python-0.2.5.dev6/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/rendered_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:14.559930 polyapi_python-0.2.5.dev6/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-14 19:35:14.000000 polyapi_python-0.2.5.dev6/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-14 19:35:14.000000 polyapi_python-0.2.5.dev6/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:35:14.000000 polyapi_python-0.2.5.dev6/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 19:35:14.000000 polyapi_python-0.2.5.dev6/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 19:35:14.000000 polyapi_python-0.2.5.dev6/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:35:14.559930 polyapi_python-0.2.5.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:35:14.559930 polyapi_python-0.2.5.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/tests/test_rendered_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-14 19:35:10.000000 polyapi_python-0.2.5.dev6/tests/test_variables.py
```

### Comparing `polyapi_python-0.2.5.dev5/LICENSE` & `polyapi_python-0.2.5.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/PKG-INFO` & `polyapi_python-0.2.5.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.5.dev5
+Version: 0.2.5.dev6
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.5.dev5/README.md` & `polyapi_python-0.2.5.dev6/README.md`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/__init__.py` & `polyapi_python-0.2.5.dev6/polyapi/__init__.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/api.py` & `polyapi_python-0.2.5.dev6/polyapi/api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/auth.py` & `polyapi_python-0.2.5.dev6/polyapi/auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/cli.py` & `polyapi_python-0.2.5.dev6/polyapi/cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/client.py` & `polyapi_python-0.2.5.dev6/polyapi/client.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/config.py` & `polyapi_python-0.2.5.dev6/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/constants.py` & `polyapi_python-0.2.5.dev6/polyapi/constants.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/error_handler.py` & `polyapi_python-0.2.5.dev6/polyapi/error_handler.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/execute.py` & `polyapi_python-0.2.5.dev6/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/function_cli.py` & `polyapi_python-0.2.5.dev6/polyapi/function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/generate.py` & `polyapi_python-0.2.5.dev6/polyapi/generate.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/rendered_spec.py` & `polyapi_python-0.2.5.dev6/polyapi/rendered_spec.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     elif spec["type"] == "serverFunction":
         data["customFunctionId"] = spec["id"]
     else:
         raise NotImplementedError("todo")
 
     # use super key on develop-k8s here!
     _, base_url = get_api_key_and_url()
+    if not base_url:
+        # local node server runs on port 8000
+        base_url = "http://localhost:8000"
+
     url = f"{base_url}/functions/rendered-specs"
     headers = {"Authorization": f"Bearer {api_key}"}
     resp = requests.post(url, json=data, headers=headers)
     assert resp.status_code == 201, (resp.text, resp.status_code)
     # this needs to run with something like `kn func run...`
```

### Comparing `polyapi_python-0.2.5.dev5/polyapi/schema.py` & `polyapi_python-0.2.5.dev6/polyapi/schema.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/server.py` & `polyapi_python-0.2.5.dev6/polyapi/server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/typedefs.py` & `polyapi_python-0.2.5.dev6/polyapi/typedefs.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/utils.py` & `polyapi_python-0.2.5.dev6/polyapi/utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/variables.py` & `polyapi_python-0.2.5.dev6/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi/webhook.py` & `polyapi_python-0.2.5.dev6/polyapi/webhook.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/polyapi_python.egg-info/PKG-INFO` & `polyapi_python-0.2.5.dev6/polyapi_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.5.dev5
+Version: 0.2.5.dev6
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.5.dev5/polyapi_python.egg-info/SOURCES.txt` & `polyapi_python-0.2.5.dev6/polyapi_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/pyproject.toml` & `polyapi_python-0.2.5.dev6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.5.dev5"
+version = "0.2.5.dev6"
 description = "The Python Client for PolyAPI, the IPaaS by Developers for Developers"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
     "pydantic==2.6.4",
```

### Comparing `polyapi_python-0.2.5.dev5/tests/test_api.py` & `polyapi_python-0.2.5.dev6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/tests/test_auth.py` & `polyapi_python-0.2.5.dev6/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/tests/test_function_cli.py` & `polyapi_python-0.2.5.dev6/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/tests/test_rendered_spec.py` & `polyapi_python-0.2.5.dev6/tests/test_rendered_spec.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/tests/test_server.py` & `polyapi_python-0.2.5.dev6/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/tests/test_utils.py` & `polyapi_python-0.2.5.dev6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev5/tests/test_variables.py` & `polyapi_python-0.2.5.dev6/tests/test_variables.py`

 * *Files identical despite different names*

