# Comparing `tmp/polyapi_python-0.2.5.dev3.tar.gz` & `tmp/polyapi_python-0.2.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi_python-0.2.5.dev3.tar", last modified: Thu May  9 16:13:00 2024, max compression
+gzip compressed data, was "polyapi_python-0.2.5.dev4.tar", last modified: Tue May 14 17:26:32 2024, max compression
```

## Comparing `polyapi_python-0.2.5.dev3.tar` & `polyapi_python-0.2.5.dev4.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:00.646603 polyapi_python-0.2.5.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-09 16:13:00.646603 polyapi_python-0.2.5.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:00.642603 polyapi_python-0.2.5.dev3/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/rendered_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:00.646603 polyapi_python-0.2.5.dev3/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-09 16:13:00.000000 polyapi_python-0.2.5.dev3/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-09 16:13:00.000000 polyapi_python-0.2.5.dev3/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:13:00.000000 polyapi_python-0.2.5.dev3/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-09 16:13:00.000000 polyapi_python-0.2.5.dev3/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 16:13:00.000000 polyapi_python-0.2.5.dev3/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 16:13:00.646603 polyapi_python-0.2.5.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:00.646603 polyapi_python-0.2.5.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-09 16:12:51.000000 polyapi_python-0.2.5.dev3/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:26:32.635038 polyapi_python-0.2.5.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-14 17:26:32.635038 polyapi_python-0.2.5.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:26:32.631038 polyapi_python-0.2.5.dev4/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/rendered_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:26:32.635038 polyapi_python-0.2.5.dev4/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-14 17:26:32.000000 polyapi_python-0.2.5.dev4/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-14 17:26:32.000000 polyapi_python-0.2.5.dev4/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:26:32.000000 polyapi_python-0.2.5.dev4/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 17:26:32.000000 polyapi_python-0.2.5.dev4/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 17:26:32.000000 polyapi_python-0.2.5.dev4/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 17:26:32.635038 polyapi_python-0.2.5.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:26:32.635038 polyapi_python-0.2.5.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/tests/test_rendered_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-14 17:26:28.000000 polyapi_python-0.2.5.dev4/tests/test_variables.py
```

### Comparing `polyapi_python-0.2.5.dev3/LICENSE` & `polyapi_python-0.2.5.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/PKG-INFO` & `polyapi_python-0.2.5.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.5.dev3
+Version: 0.2.5.dev4
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.5.dev3/README.md` & `polyapi_python-0.2.5.dev4/README.md`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/__init__.py` & `polyapi_python-0.2.5.dev4/polyapi/__init__.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/api.py` & `polyapi_python-0.2.5.dev4/polyapi/api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/auth.py` & `polyapi_python-0.2.5.dev4/polyapi/auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/cli.py` & `polyapi_python-0.2.5.dev4/polyapi/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import argparse
 
 from polyapi.utils import print_green
 
 from .config import clear_config, set_api_key_and_url
 from .generate import generate, clear
 from .function_cli import function_add_or_update
-from .rendered_spec import save_rendered_specs
+from .rendered_spec import get_and_update_rendered_spec
 
 
-CLI_COMMANDS = ["setup", "generate", "function", "clear", "help", "save_rendered_specs"]
+CLI_COMMANDS = ["setup", "generate", "function", "clear", "help", "update_rendered_spec"]
 
 CLIENT_DESC = """Commands
   python -m polyapi setup                Setup your Poly connection
   python -m polyapi generate             Generates Poly library
   python -m polyapi function <command>   Manages functions
   python -m polyapi clear                Clear current generated Poly library
 """
 
 
-def execute_from_cli():
+def execute_from_cli() -> None:
     parser = argparse.ArgumentParser(
         prog="python -m polyapi", description=CLIENT_DESC, formatter_class=argparse.RawTextHelpFormatter
     )
     parser.add_argument("--context", required=False, default="")
     parser.add_argument("--description", required=False, default="")
     parser.add_argument("--client", action="store_true", help="Pass --client when adding function to add a client function.")
     parser.add_argument("--server", action="store_true", help="Pass --server when adding function to add a server function.")
@@ -39,14 +39,20 @@
         generate()
         print_green("DONE")
     elif command == "setup" and len(args.subcommands) == 2:
         set_api_key_and_url(args.subcommands[1], args.subcommands[0])
     elif command == "setup":
         clear_config()
         generate()
-    elif command == "save_rendered_specs":
-        save_rendered_specs()
+    elif command == "update_rendered_spec":
+        assert len(args.subcommands) == 2
+        updated = get_and_update_rendered_spec(args.subcommands[0], args.subcommands[1])
+        if updated:
+            print("Updated rendered spec!")
+        else:
+            print("Failed to update rendered spec!")
+            exit(1)
     elif command == "clear":
         print("Clearing the generated library...")
         clear()
     elif command == "function":
         function_add_or_update(args.context, args.description, args.client, args.server, args.logs, args.subcommands)
```

### Comparing `polyapi_python-0.2.5.dev3/polyapi/client.py` & `polyapi_python-0.2.5.dev4/polyapi/client.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/config.py` & `polyapi_python-0.2.5.dev4/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/constants.py` & `polyapi_python-0.2.5.dev4/polyapi/constants.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/error_handler.py` & `polyapi_python-0.2.5.dev4/polyapi/error_handler.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/execute.py` & `polyapi_python-0.2.5.dev4/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/function_cli.py` & `polyapi_python-0.2.5.dev4/polyapi/function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/generate.py` & `polyapi_python-0.2.5.dev4/polyapi/generate.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/rendered_spec.py` & `polyapi_python-0.2.5.dev4/polyapi/rendered_spec.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from typing import Dict
+from typing import Dict, Optional
+
+import requests
+from polyapi.config import get_api_key_and_url
 from polyapi.generate import read_cached_specs, render_spec
 from polyapi.execute import execute_post
 from polyapi.typedefs import SpecificationDto
 
 
 def update_rendered_spec(spec: SpecificationDto):
     print("Updating rendered spec...")
@@ -15,19 +18,43 @@
     if spec["type"] == "apiFunction":
         data["apiFunctionId"] = spec["id"]
     elif spec["type"] == "serverFunction":
         data["customFunctionId"] = spec["id"]
     else:
         raise NotImplementedError("todo")
 
+    # use super key on develop-k8s here!
     resp = execute_post("/functions/rendered-specs", data)
     assert resp.status_code == 201, (resp.text, resp.status_code)
     # this needs to run with something like `kn func run...`
 
 
+def _get_spec(api_key: str, spec_id: str) -> Optional[SpecificationDto]:
+    _, base_url = get_api_key_and_url()
+    url = f"{base_url}/specs"
+    headers = {"Authorization": f"Bearer {api_key}"}
+    resp = requests.get(url, headers=headers)
+    if resp.status_code == 200:
+        specs = resp.json()
+        for spec in specs:
+            if spec['id'] == spec_id:
+                return spec
+        return None
+    else:
+        raise NotImplementedError(resp.content)
+
+
+def get_and_update_rendered_spec(api_key: str, spec_id: str) -> bool:
+    spec = _get_spec(api_key, spec_id)
+    if spec:
+        update_rendered_spec(spec)
+        return True
+    return False
+
+
 def save_rendered_specs() -> None:
     specs = read_cached_specs()
     # right now we just support rendered apiFunctions
     api_specs = [spec for spec in specs if spec["type"] == "apiFunction"]
     for spec in api_specs:
         assert spec["function"]
         print("adding", spec["context"], spec["name"])
```

### Comparing `polyapi_python-0.2.5.dev3/polyapi/schema.py` & `polyapi_python-0.2.5.dev4/polyapi/schema.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/server.py` & `polyapi_python-0.2.5.dev4/polyapi/server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/typedefs.py` & `polyapi_python-0.2.5.dev4/polyapi/typedefs.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/utils.py` & `polyapi_python-0.2.5.dev4/polyapi/utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/variables.py` & `polyapi_python-0.2.5.dev4/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi/webhook.py` & `polyapi_python-0.2.5.dev4/polyapi/webhook.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/polyapi_python.egg-info/PKG-INFO` & `polyapi_python-0.2.5.dev4/polyapi_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.5.dev3
+Version: 0.2.5.dev4
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.5.dev3/polyapi_python.egg-info/SOURCES.txt` & `polyapi_python-0.2.5.dev4/polyapi_python.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,10 +26,12 @@
 polyapi_python.egg-info/SOURCES.txt
 polyapi_python.egg-info/dependency_links.txt
 polyapi_python.egg-info/requires.txt
 polyapi_python.egg-info/top_level.txt
 tests/test_api.py
 tests/test_auth.py
 tests/test_function_cli.py
+tests/test_rendered_spec.py
+tests/test_schema.py
 tests/test_server.py
 tests/test_utils.py
 tests/test_variables.py
```

### Comparing `polyapi_python-0.2.5.dev3/pyproject.toml` & `polyapi_python-0.2.5.dev4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.5.dev3"
+version = "0.2.5.dev4"
 description = "The Python Client for PolyAPI, the IPaaS by Developers for Developers"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
     "pydantic==2.6.4",
```

### Comparing `polyapi_python-0.2.5.dev3/tests/test_api.py` & `polyapi_python-0.2.5.dev4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/tests/test_auth.py` & `polyapi_python-0.2.5.dev4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/tests/test_function_cli.py` & `polyapi_python-0.2.5.dev4/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/tests/test_server.py` & `polyapi_python-0.2.5.dev4/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/tests/test_utils.py` & `polyapi_python-0.2.5.dev4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev3/tests/test_variables.py` & `polyapi_python-0.2.5.dev4/tests/test_variables.py`

 * *Files identical despite different names*

