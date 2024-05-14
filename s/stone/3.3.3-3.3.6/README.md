# Comparing `tmp/stone-3.3.3.tar.gz` & `tmp/stone-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stone-3.3.3.tar", last modified: Thu Mar 28 16:48:41 2024, max compression
+gzip compressed data, was "stone-3.3.6.tar", last modified: Tue May 14 19:21:07 2024, max compression
```

## Comparing `stone-3.3.3.tar` & `stone-3.3.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:48:41.225581 stone-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-28 16:48:27.000000 stone-3.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-28 16:48:27.000000 stone-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-03-28 16:48:41.225581 stone-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-03-28 16:48:27.000000 stone-3.3.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-03-28 16:48:27.000000 stone-3.3.3/ez_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 16:48:41.229581 stone-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-03-28 16:48:27.000000 stone-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:48:41.217581 stone-3.3.3/stone/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 16:48:27.000000 stone-3.3.3/stone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19277 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:48:41.221581 stone-3.3.3/stone/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/js_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/js_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/js_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/obj_c.py
--rw-r--r--   0 runner    (1001) docker     (127)    25527 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/obj_c_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12697 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/obj_c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    70757 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/obj_c_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    23654 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/python_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/python_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:48:41.221581 stone-3.3.3/stone/backends/python_rsrc/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/python_rsrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/python_rsrc/stone_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    42584 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/python_rsrc/stone_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    25579 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/python_rsrc/stone_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/python_type_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    18566 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/python_type_stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    50123 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/python_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/swift.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/swift_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/swift_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20578 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/swift_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/tsd_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/tsd_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20714 2024-03-28 16:48:27.000000 stone-3.3.3/stone/backends/tsd_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-03-28 16:48:27.000000 stone-3.3.3/stone/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-03-28 16:48:27.000000 stone-3.3.3/stone/cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-03-28 16:48:27.000000 stone-3.3.3/stone/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:48:41.225581 stone-3.3.3/stone/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 16:48:27.000000 stone-3.3.3/stone/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-03-28 16:48:27.000000 stone-3.3.3/stone/frontend/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-28 16:48:27.000000 stone-3.3.3/stone/frontend/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-28 16:48:27.000000 stone-3.3.3/stone/frontend/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    80039 2024-03-28 16:48:27.000000 stone-3.3.3/stone/frontend/ir_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-03-28 16:48:27.000000 stone-3.3.3/stone/frontend/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27531 2024-03-28 16:48:27.000000 stone-3.3.3/stone/frontend/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:48:41.225581 stone-3.3.3/stone/ir/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-28 16:48:27.000000 stone-3.3.3/stone/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18082 2024-03-28 16:48:27.000000 stone-3.3.3/stone/ir/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    74934 2024-03-28 16:48:27.000000 stone-3.3.3/stone/ir/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 16:48:27.000000 stone-3.3.3/stone/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-28 16:48:27.000000 stone-3.3.3/stone/typing_hacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:48:41.225581 stone-3.3.3/stone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-03-28 16:48:41.000000 stone-3.3.3/stone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-03-28 16:48:41.000000 stone-3.3.3/stone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 16:48:41.000000 stone-3.3.3/stone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-28 16:48:41.000000 stone-3.3.3/stone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 16:48:40.000000 stone-3.3.3/stone.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-28 16:48:41.000000 stone-3.3.3/stone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 16:48:41.000000 stone-3.3.3/stone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:48:41.225581 stone-3.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 16:48:27.000000 stone-3.3.3/test/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    17527 2024-03-28 16:48:27.000000 stone-3.3.3/test/test_backend.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5438 2024-03-28 16:48:27.000000 stone-3.3.3/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-03-28 16:48:27.000000 stone-3.3.3/test/test_js_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-03-28 16:48:27.000000 stone-3.3.3/test/test_python_client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   116400 2024-03-28 16:48:27.000000 stone-3.3.3/test/test_python_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-03-28 16:48:27.000000 stone-3.3.3/test/test_python_type_stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-03-28 16:48:27.000000 stone-3.3.3/test/test_python_types.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   156052 2024-03-28 16:48:27.000000 stone-3.3.3/test/test_stone.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15310 2024-03-28 16:48:27.000000 stone-3.3.3/test/test_stone_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-03-28 16:48:27.000000 stone-3.3.3/test/test_stone_route_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-03-28 16:48:27.000000 stone-3.3.3/test/test_tsd_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14745 2024-03-28 16:48:27.000000 stone-3.3.3/test/test_tsd_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:07.259165 stone-3.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-14 19:20:58.000000 stone-3.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 19:20:58.000000 stone-3.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-05-14 19:21:07.259165 stone-3.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-14 19:20:58.000000 stone-3.3.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-14 19:20:58.000000 stone-3.3.6/ez_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 19:21:07.259165 stone-3.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-14 19:20:58.000000 stone-3.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:07.247165 stone-3.3.6/stone/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:20:58.000000 stone-3.3.6/stone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19277 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:07.251165 stone-3.3.6/stone/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/js_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/js_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/js_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/obj_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25527 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/obj_c_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12697 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/obj_c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70757 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/obj_c_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23654 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/python_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/python_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:07.255165 stone-3.3.6/stone/backends/python_rsrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/python_rsrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/python_rsrc/stone_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42584 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/python_rsrc/stone_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/python_rsrc/stone_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/python_type_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18566 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/python_type_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50123 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/python_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/swift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/swift_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/swift_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20578 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/swift_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/tsd_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/tsd_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20714 2024-05-14 19:20:58.000000 stone-3.3.6/stone/backends/tsd_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-05-14 19:20:58.000000 stone-3.3.6/stone/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-14 19:20:58.000000 stone-3.3.6/stone/cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-14 19:20:58.000000 stone-3.3.6/stone/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:07.255165 stone-3.3.6/stone/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:20:58.000000 stone-3.3.6/stone/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-05-14 19:20:58.000000 stone-3.3.6/stone/frontend/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-14 19:20:58.000000 stone-3.3.6/stone/frontend/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-14 19:20:58.000000 stone-3.3.6/stone/frontend/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80039 2024-05-14 19:20:58.000000 stone-3.3.6/stone/frontend/ir_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-14 19:20:58.000000 stone-3.3.6/stone/frontend/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27531 2024-05-14 19:20:58.000000 stone-3.3.6/stone/frontend/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:07.255165 stone-3.3.6/stone/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 19:20:58.000000 stone-3.3.6/stone/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18082 2024-05-14 19:20:58.000000 stone-3.3.6/stone/ir/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74934 2024-05-14 19:20:58.000000 stone-3.3.6/stone/ir/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:20:58.000000 stone-3.3.6/stone/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-14 19:20:58.000000 stone-3.3.6/stone/typing_hacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:07.259165 stone-3.3.6/stone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-05-14 19:21:07.000000 stone-3.3.6/stone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-14 19:21:07.000000 stone-3.3.6/stone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:21:07.000000 stone-3.3.6/stone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 19:21:07.000000 stone-3.3.6/stone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:21:06.000000 stone-3.3.6/stone.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 19:21:07.000000 stone-3.3.6/stone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 19:21:07.000000 stone-3.3.6/stone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:07.259165 stone-3.3.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 19:20:58.000000 stone-3.3.6/test/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17527 2024-05-14 19:20:58.000000 stone-3.3.6/test/test_backend.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5438 2024-05-14 19:20:58.000000 stone-3.3.6/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-05-14 19:20:58.000000 stone-3.3.6/test/test_js_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-05-14 19:20:58.000000 stone-3.3.6/test/test_python_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   116400 2024-05-14 19:20:58.000000 stone-3.3.6/test/test_python_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-14 19:20:58.000000 stone-3.3.6/test/test_python_type_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-05-14 19:20:58.000000 stone-3.3.6/test/test_python_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   156052 2024-05-14 19:20:58.000000 stone-3.3.6/test/test_stone.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15310 2024-05-14 19:20:58.000000 stone-3.3.6/test/test_stone_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-05-14 19:20:58.000000 stone-3.3.6/test/test_stone_route_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-14 19:20:58.000000 stone-3.3.6/test/test_tsd_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14745 2024-05-14 19:20:58.000000 stone-3.3.6/test/test_tsd_types.py
```

### Comparing `stone-3.3.3/LICENSE` & `stone-3.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/PKG-INFO` & `stone-3.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stone
-Version: 3.3.3
+Version: 3.3.6
 Summary: Stone is an interface description language (IDL) for APIs.
 Home-page: https://github.com/dropbox/stone
 Author: Ken Elkabany
 Author-email: kelkabany@dropbox.com
 Maintainer: Dropbox
 Maintainer-email: api-platform@dropbox.com
 License: MIT License
```

### Comparing `stone-3.3.3/README.rst` & `stone-3.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/ez_setup.py` & `stone-3.3.6/ez_setup.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/setup.py` & `stone-3.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     test_reqs += f.read().splitlines()
 
 with open('README.rst') as f:  # pylint: disable=W1514
     README = f.read()
 
 dist = setup(
     name='stone',
-    version='3.3.3',
+    version='3.3.6',
     install_requires=install_reqs,
     setup_requires=setup_requires,
     tests_require=test_reqs,
     entry_points={
         'console_scripts': ['stone=stone.cli:main'],
     },
     packages=[
```

### Comparing `stone-3.3.3/stone/backend.py` & `stone-3.3.6/stone/backend.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/helpers.py` & `stone-3.3.6/stone/backends/helpers.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/js_client.py` & `stone-3.3.6/stone/backends/js_client.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/js_helpers.py` & `stone-3.3.6/stone/backends/js_helpers.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/js_types.py` & `stone-3.3.6/stone/backends/js_types.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/obj_c.py` & `stone-3.3.6/stone/backends/obj_c.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/obj_c_client.py` & `stone-3.3.6/stone/backends/obj_c_client.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/obj_c_helpers.py` & `stone-3.3.6/stone/backends/obj_c_helpers.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/obj_c_types.py` & `stone-3.3.6/stone/backends/obj_c_types.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/python_client.py` & `stone-3.3.6/stone/backends/python_client.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/python_helpers.py` & `stone-3.3.6/stone/backends/python_helpers.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/python_rsrc/stone_base.py` & `stone-3.3.6/stone/backends/python_rsrc/stone_base.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/python_rsrc/stone_serializers.py` & `stone-3.3.6/stone/backends/python_rsrc/stone_serializers.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/python_rsrc/stone_validators.py` & `stone-3.3.6/stone/backends/python_rsrc/stone_validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,25 @@
         return 'string'
     elif v is None:
         return 'null'
     else:
         return type_name_with_module(type(v))
 
 
+def get_value_string(v, max_length=1000):
+    # type: (typing.Any, int) -> str
+    """Return a truncated version of the input string.  If the input string is longer than
+       1000 characters, this will return the first 1000 characters and append with '[The
+       string has been truncated due to its length]' to indicate that it has been truncated."""
+    v_str = str(v)
+    if len(v_str) > max_length:
+        return v_str[:max_length] + ' [The string has been truncated due to its length]'
+    return v_str
+
+
 class Validator(metaclass=ABCMeta):
     """All primitive and composite data types should be a subclass of this."""
     __slots__ = ("_redact",)
 
     @abstractmethod
     def validate(self, val):
         """Validates that val is of this data type.
@@ -318,31 +329,35 @@
         """
         A unicode string of the correct length and pattern will pass validation.
         In PY2, we enforce that a str type must be valid utf-8, and a unicode
         string will be returned.
         """
         if not isinstance(val, str):
             raise ValidationError("'%s' expected to be a string, got %s"
-                                  % (val, generic_type_name(val)))
+                                  % (get_value_string(val), generic_type_name(val)))
         if not six.PY3 and isinstance(val, str):
             try:
                 val = val.decode('utf-8')
             except UnicodeDecodeError:
                 raise ValidationError("'%s' was not valid utf-8")
 
         if self.max_length is not None and len(val) > self.max_length:
             raise ValidationError("'%s' must be at most %d characters, got %d"
-                                  % (val, self.max_length, len(val)))
+                                  % (get_value_string(val), self.max_length, len(val)))
         if self.min_length is not None and len(val) < self.min_length:
             raise ValidationError("'%s' must be at least %d characters, got %d"
-                                  % (val, self.min_length, len(val)))
+                                  % (get_value_string(val), self.min_length, len(val)))
 
         if self.pattern and not self.pattern_re.match(val):
+            # Detect if pattern is matching an email address and return redacted error message.
+            if self.pattern == "^['#&A-Za-z0-9._%+-]+@[A-Za-z0-9-][A-Za-z0-9.-]*\\.[A-Za-z]{2,15}$":
+                val = "*****"
+
             raise ValidationError("'%s' did not match pattern '%s'"
-                                  % (val, self.pattern))
+                                  % (get_value_string(val), self.pattern))
         return val
 
 
 class Bytes(Primitive):
     __slots__ = ("min_length", "max_length")
 
     def __init__(self, min_length=None, max_length=None):
@@ -362,18 +377,18 @@
 
     def validate(self, val):
         if not isinstance(val, _binary_types):
             raise ValidationError("expected bytes type, got %s"
                                   % generic_type_name(val))
         elif self.max_length is not None and len(val) > self.max_length:
             raise ValidationError("'%s' must have at most %d bytes, got %d"
-                                  % (val, self.max_length, len(val)))
+                                  % (get_value_string(val), self.max_length, len(val)))
         elif self.min_length is not None and len(val) < self.min_length:
             raise ValidationError("'%s' has fewer than %d bytes, got %d"
-                                  % (val, self.min_length, len(val)))
+                                  % (get_value_string(val), self.min_length, len(val)))
         return val
 
 
 class Timestamp(Primitive):
     """Note that while a format is specified, it isn't used in validation
     since a native Python datetime object is preferred. The format, however,
     can and should be used by serializers."""
@@ -421,21 +436,21 @@
             assert max_items >= min_items, 'max_items must be >= min_items'
 
         self.min_items = min_items
         self.max_items = max_items
 
     def validate(self, val):
         if not isinstance(val, (tuple, list)):
-            raise ValidationError('%r is not a valid list' % val)
+            raise ValidationError('%r is not a valid list' % get_value_string(val))
         elif self.max_items is not None and len(val) > self.max_items:
             raise ValidationError('%r has more than %s items'
-                                  % (val, self.max_items))
+                                  % (get_value_string(val), self.max_items))
         elif self.min_items is not None and len(val) < self.min_items:
             raise ValidationError('%r has fewer than %s items'
-                                  % (val, self.min_items))
+                                  % (get_value_string(val), self.min_items))
         return [self.item_validator.validate(item) for item in val]
 
 
 class Map(Composite):
     """Assumes map keys and values are homogeneous with respect to types."""
     __slots__ = ("key_validator", "value_validator")
 
@@ -445,15 +460,15 @@
         key validators must be a subclass of a String validator
         """
         self.key_validator = key_validator
         self.value_validator = value_validator
 
     def validate(self, val):
         if not isinstance(val, dict):
-            raise ValidationError('%r is not a valid dict' % val)
+            raise ValidationError('%r is not a valid dict' % get_value_string(val))
         return {
             self.key_validator.validate(key):
                 self.value_validator.validate(value) for key, value in val.items()
         }
 
 
 class Struct(Composite):
```

### Comparing `stone-3.3.3/stone/backends/python_type_mapping.py` & `stone-3.3.6/stone/backends/python_type_mapping.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/python_type_stubs.py` & `stone-3.3.6/stone/backends/python_type_stubs.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/python_types.py` & `stone-3.3.6/stone/backends/python_types.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/swift.py` & `stone-3.3.6/stone/backends/swift.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/swift_client.py` & `stone-3.3.6/stone/backends/swift_client.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/swift_helpers.py` & `stone-3.3.6/stone/backends/swift_helpers.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/swift_types.py` & `stone-3.3.6/stone/backends/swift_types.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/tsd_client.py` & `stone-3.3.6/stone/backends/tsd_client.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/tsd_helpers.py` & `stone-3.3.6/stone/backends/tsd_helpers.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/backends/tsd_types.py` & `stone-3.3.6/stone/backends/tsd_types.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/cli.py` & `stone-3.3.6/stone/cli.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/cli_helpers.py` & `stone-3.3.6/stone/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/compiler.py` & `stone-3.3.6/stone/compiler.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/frontend/ast.py` & `stone-3.3.6/stone/frontend/ast.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/frontend/exception.py` & `stone-3.3.6/stone/frontend/exception.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/frontend/frontend.py` & `stone-3.3.6/stone/frontend/frontend.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/frontend/ir_generator.py` & `stone-3.3.6/stone/frontend/ir_generator.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/frontend/lexer.py` & `stone-3.3.6/stone/frontend/lexer.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/frontend/parser.py` & `stone-3.3.6/stone/frontend/parser.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/ir/api.py` & `stone-3.3.6/stone/ir/api.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone/ir/data_types.py` & `stone-3.3.6/stone/ir/data_types.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/stone.egg-info/PKG-INFO` & `stone-3.3.6/stone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stone
-Version: 3.3.3
+Version: 3.3.6
 Summary: Stone is an interface description language (IDL) for APIs.
 Home-page: https://github.com/dropbox/stone
 Author: Ken Elkabany
 Author-email: kelkabany@dropbox.com
 Maintainer: Dropbox
 Maintainer-email: api-platform@dropbox.com
 License: MIT License
```

### Comparing `stone-3.3.3/stone.egg-info/SOURCES.txt` & `stone-3.3.6/stone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/test/test_backend.py` & `stone-3.3.6/test/test_backend.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/test/test_cli.py` & `stone-3.3.6/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/test/test_js_client.py` & `stone-3.3.6/test/test_js_client.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/test/test_python_client.py` & `stone-3.3.6/test/test_python_client.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/test/test_python_gen.py` & `stone-3.3.6/test/test_python_gen.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/test/test_python_type_stubs.py` & `stone-3.3.6/test/test_python_type_stubs.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/test/test_python_types.py` & `stone-3.3.6/test/test_python_types.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/test/test_stone.py` & `stone-3.3.6/test/test_stone.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/test/test_stone_internal.py` & `stone-3.3.6/test/test_stone_internal.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/test/test_stone_route_whitelist.py` & `stone-3.3.6/test/test_stone_route_whitelist.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/test/test_tsd_client.py` & `stone-3.3.6/test/test_tsd_client.py`

 * *Files identical despite different names*

### Comparing `stone-3.3.3/test/test_tsd_types.py` & `stone-3.3.6/test/test_tsd_types.py`

 * *Files identical despite different names*

