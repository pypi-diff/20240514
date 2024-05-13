# Comparing `tmp/ioxplugin-1.0.7.tar.gz` & `tmp/ioxplugin-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioxplugin-1.0.7.tar", last modified: Mon May 13 09:07:25 2024, max compression
+gzip compressed data, was "ioxplugin-1.0.9.tar", last modified: Mon May 13 22:00:12 2024, max compression
```

## Comparing `ioxplugin-1.0.7.tar` & `ioxplugin-1.0.9.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:07:25.038709 ioxplugin-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 09:07:25.038709 ioxplugin-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:07:25.038709 ioxplugin-1.0.7/ioxplugin/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56393 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/ast_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_controller_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_main_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_node_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_node_impl_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_to_modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/main_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/new_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/node_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/nodedef.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3014 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/oauth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/plugin_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/uom.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:07:25.038709 ioxplugin-1.0.7/ioxplugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 09:07:25.000000 ioxplugin-1.0.7/ioxplugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-13 09:07:25.000000 ioxplugin-1.0.7/ioxplugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:07:25.000000 ioxplugin-1.0.7/ioxplugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 09:07:25.000000 ioxplugin-1.0.7/ioxplugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 09:07:25.000000 ioxplugin-1.0.7/ioxplugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:07:25.038709 ioxplugin-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:07:25.038709 ioxplugin-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/tests/test_ioxplugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:12.765927 ioxplugin-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 22:00:12.761927 ioxplugin-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:12.761927 ioxplugin-1.0.9/ioxplugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53706 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/ast_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/iox_controller_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/iox_main_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/iox_node_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/iox_node_impl_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/iox_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/iox_to_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/iox_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/main_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/new_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/node_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/nodedef.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3014 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/oauth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/plugin_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/uom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/ioxplugin/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:12.761927 ioxplugin-1.0.9/ioxplugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 22:00:12.000000 ioxplugin-1.0.9/ioxplugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-13 22:00:12.000000 ioxplugin-1.0.9/ioxplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:00:12.000000 ioxplugin-1.0.9/ioxplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 22:00:12.000000 ioxplugin-1.0.9/ioxplugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 22:00:12.000000 ioxplugin-1.0.9/ioxplugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 22:00:12.765927 ioxplugin-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:00:12.761927 ioxplugin-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/tests/ModbusControllerNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/tests/ModbusDeviceNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/tests/ModbusProtocolHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/tests/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/tests/test_ioxplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 22:00:08.000000 ioxplugin-1.0.9/tests/version.py
```

### Comparing `ioxplugin-1.0.7/PKG-INFO` & `ioxplugin-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 1.0.7
+Version: 1.0.9
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-1.0.7/ioxplugin/__init__.py` & `ioxplugin-1.0.9/ioxplugin/__init__.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/ast_util.py` & `ioxplugin-1.0.9/ioxplugin/ast_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         ast.Expr(value=ast.Call(
             func=ast.Attribute(value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()), attr='subscribe', ctx=ast.Load()),
             args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='START', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='start', ctx=ast.Load())],
             keywords=[]
         )),
         ast.Expr(value=ast.Call(
             func=ast.Attribute(value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()), attr='subscribe', ctx=ast.Load()),
-            args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='CUSTOMPARAMS', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='parameter_handler', ctx=ast.Load())],
+            args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='CUSTOMPARAMS', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='parameterHandler', ctx=ast.Load())],
             keywords=[]
         )),
         ast.Expr(value=ast.Call(
             func=ast.Attribute(value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()), attr='subscribe', ctx=ast.Load()),
             args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='POLL', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poll', ctx=ast.Load())],
             keywords=[]
         )),
@@ -339,14 +339,32 @@
             keywords=[]
         )),
         ast.Expr(value=ast.Call(
             func=ast.Attribute(value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()), attr='subscribe', ctx=ast.Load()),
             args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='CUSTOMDATA', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='customDataHandler', ctx=ast.Load())],
             keywords=[]
         )),
+        ast.Assign(
+            targets=[
+                ast.Attribute(
+                    value=ast.Name(id='self', ctx=ast.Load()),
+                    attr='configDone',
+                    ctx=ast.Store()
+                )
+            ],
+            value=ast.Call(
+                func=ast.Attribute(
+                    value=ast.Name(id='threading', ctx=ast.Load()),
+                    attr='Condition',
+                    ctx=ast.Load()
+                ),
+                args=[],
+                keywords=[]
+            )
+        ),
         ast.Expr(value=ast.Call(
             func=ast.Attribute(
                 value=ast.Name(id='self', ctx=ast.Load()),
                 attr='initOAuth',
                 ctx=ast.Load()
             ),
             args=[],  # No arguments are passed to the function
@@ -433,110 +451,14 @@
         body=init_body,
         decorator_list=[],
         returns=None
     )
 
     return function_def
 
-def astControllerBody(): 
-    # Create an AST node for the assignment to self.Parameters
-    assignment = ast.Assign(
-        targets=[ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='Parameters', ctx=ast.Store())],
-        value=ast.Call(
-            func=ast.Name(id='Custom', ctx=ast.Load()),
-            args=[
-                ast.Name(id='polyglot', ctx=ast.Load()),
-                ast.Str(s='customparams')
-            ],
-            keywords=[]
-        )
-    )
-    
-    valid_config = ast.Assign(
-                targets=[ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='valid_configuration', ctx=ast.Store())],
-                value=ast.Constant(value=False)
-    )
-
-    # Create a list to store method calls
-    method_calls = []
-
-    # Subscribing to various events
-    events = ['START', 'CUSTOMPARAMS', 'POLL', 'STOP', 'CONFIG']
-    methods = ['start', 'parameter_handler', 'poll', 'stop', 'config']
-    for event, method in zip(events, methods):
-        subscribe_call = ast.Expr(value=ast.Call(
-            func=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()),
-            args=[
-                ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr=event, ctx=ast.Load()),
-                ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr=method, ctx=ast.Load())
-            ],
-            keywords=[]
-        ))
-        method_calls.append(subscribe_call)
-
-    # Adding self.poly.ready() and self.addAllNodes() calls
-    ready_call = ast.Expr(value=ast.Call(
-        func=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly.ready', ctx=ast.Load()),
-        args=[],
-        keywords=[]
-    ))
-    method_calls.append(ready_call)
-
-    add_all_nodes_call = ast.Expr(value=ast.Call(
-        func=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='addAllNodes', ctx=ast.Load()),
-        args=[],
-        keywords=[]
-    ))
-    method_calls.append(add_all_nodes_call)
-
-    return [assignment, valid_config] + method_calls
-
-def astParamHandlerFunc():
-    # Create AST nodes for each statement in the function body
-    clear_notices = ast.Expr(value=ast.Call(
-    func=ast.Attribute(
-            value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()),
-            attr='Notices.clear',
-            ctx=ast.Load()
-    ),
-    args=[],
-    keywords=[]
-    ))
-
-    load_parameters = ast.Expr(value=ast.Call(
-    func=ast.Attribute(
-            value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='Parameters', ctx=ast.Load()),
-            attr='load',
-            ctx=ast.Load()
-    ),
-    args=[ast.Name(id='params', ctx=ast.Load())],
-    keywords=[]
-    ))
-
-    return_true = ast.Return(value=ast.Constant(value=True))
-
-    # Function definition
-    function_def = ast.FunctionDef(
-    name='parameter_handler',
-    args=ast.arguments(
-            posonlyargs=[],
-            args=[ast.arg(arg='self'), ast.arg(arg='params')],
-            kwonlyargs=[],
-            kw_defaults=[],
-            defaults=[]
-    ),
-    body=[clear_notices, load_parameters, return_true],
-    decorator_list=[],
-    returns=None
-    )
- 
-    return function_def
-
-import ast
-
 def astStartFunc():
     log_info = astLogger('info', 'Starting ... ', False)
     function_def = ast.FunctionDef(
         name='start',
         args=ast.arguments(
             posonlyargs=[],
             args=[ast.arg(arg='self')],
```

### Comparing `ioxplugin-1.0.7/ioxplugin/commands.py` & `ioxplugin-1.0.9/ioxplugin/commands.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/editor.py` & `ioxplugin-1.0.9/ioxplugin/editor.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/iox_controller_template.py` & `ioxplugin-1.0.9/ioxplugin/iox_controller_template.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,20 @@
 CONTROLLER_TEMPLATE_HEADER='''
-import udi_interface, os, sys, json, time
+import udi_interface, os, shutil, sys, json, time, threading
 from udi_interface import OAuth
 LOGGER = udi_interface.LOGGER
 Custom = udi_interface.Custom
 from ioxplugin import Plugin, OAuthService
 
 DATA_PATH='./data'
 '''
 
-#
-#from ModbusDeviceNode import ModbusDeviceNode
-#class ModbusControllerNode(udi_interface.Node):
-#   id = 'modbuscontroll'
-#    """This is a list of properties that were defined in the nodedef"""
-#    drivers = [{'driver': 'ST', 'value': 0, 'uom': 2, 'name': 'Status'}]
-#    children = [{'node_class': 'ModbusDeviceNode', 'id': 'modbus', 'name':
-#        'ModbusDevice', 'parent': 'modbuscontroll'}]
-
-#    def __init__(self, polyglot, protocolHandler, controller=
-#        'modbuscontroll', address='modbuscontroll', name='Modbus Controller'):
-#        super().__init__(polyglot, controller, address, name)
-#        self.protocolHandler = protocolHandler
-#        self.Parameters = Custom(polyglot, 'customparams')
-#        self.valid_configuration = False
-#        self.started = False
-#        self.poly.subscribe(polyglot.START, self.start)
-#        self.poly.subscribe(polyglot.CUSTOMPARAMS, self.parameter_handler)
-#        self.poly.subscribe(polyglot.POLL, self.poll)
-#        self.poly.subscribe(polyglot.STOP, self.stop)
-#        self.poly.subscribe(polyglot.CONFIG, self.config)
-
 CONTROLLER_TEMPLATE_BODY='''
 
-    def setProtocolHandler(self, protocolHandler):
+     def setProtocolHandler(self, protocolHandler):
         self.protocolHandler = protocolHandler
 
     def initOAuth(self):
         if self.protocolHandler and self.protocolHandler.plugin and self.protocolHandler.plugin.meta and self.protocolHandler.plugin.meta.getEnableOAUTH2():
             self.oauthService = OAuthService(self.polyglot)
 
     def parameter_handler(self, params):
@@ -53,21 +31,37 @@
             LOGGER.warn(str(ex))
 
         self.protocolHandler.configChanged(param)
         return True
 
     def start(self):
         LOGGER.info(f'Starting... ')
-        self.poly.addNode(self)
-        self.addAllNodes()
-        self.poly.updateProfile()
-        self.poly.setCustomParamsDoc()
-        self.updateStatus(1 if self.protocolHandler.start() else 0, True)
-        self.poly.ready()
-        return True
+        try:
+            self.poly.addNode(self)
+            self.poly.setCustomParamsDoc()
+            self.poly.ready()
+            with self.configDone:
+                result = self.configDone.wait(timeout=10)
+                if not result:
+                    #timedout
+                    LOGGER.info("timed out while waiting for configDone")
+                    self.updateStatus(0, True) 
+                    return False
+                if self.protocolHandler.start():
+                    self.addAllNodes()
+                    self.poly.updateProfile()
+                    self.updateStatus(1, True) 
+                    return True
+                else:
+                    LOGGER.info("protocol handler failed processing config ...")
+                    self.updateStatus(0, True) 
+                    return False
+        except Exception as ex:
+            LOGGER.error(str(ex))
+            return False
 
     def stop(self):
         LOGGER.info(f'Stopping ... ')
         self.protocolHandler.stop()
         self.updateStatus(0)
         return True
 
@@ -113,33 +107,40 @@
                 return False
         except Exception as ex:
             LOGGER.error(str(ex))
             return False
 
     def addNodeDoneHandler(self, node):
         try:
+            if node['nodeDefId'] == self.id:
+                return True
             return self.protocolHandler.addNodeDone(node)
 
         except ValueError as err:
             LOGGER.error(str(x))
             return False
 
     def configDoneHandler(self):
-        if not self.oauthService:
-            return 
-        # First check if user has authenticated
-        try:
-            self.oauthService.getAccessToken()
-            # If getAccessToken did raise an exception, then proceed with device discovery
-            return self.protocolHandler.configDone()
+        rc = False
+        if self.oauthService:
+            # First check if user has authenticated
+            try:
+                self.oauthService.getAccessToken()
+                # If getAccessToken did raise an exception, then proceed with device discovery
+                rc = self.protocolHandler.configDone()
+
+            except ValueError as err:
+                LOGGER.warning('Access token is not yet available. Please authenticate.')
+                polyglot.Notices['auth'] = 'Please initiate authentication using the Authenticate Buttion'
+                return False
+        with self.configDone:
+            self.configDone.notifyAll()
+        return rc
+
 
-        except ValueError as err:
-            LOGGER.warning('Access token is not yet available. Please authenticate.')
-            polyglot.Notices['auth'] = 'Please initiate authentication using the Authenticate Buttion'
-            return False
 
     def customNSHandler(self, key, data):
         if not self.oauthService:
             return 
         # This provides the oAuth config (key='oauth') and saved oAuth tokens (key='oauthTokens))
         try:
             self.oauthService.customNsHandler(key, data)
@@ -187,8 +188,9 @@
             else:
                 node.queryAll()
 
     ###
     # This is a list of commands that were defined in the nodedef
     ###
     commands = {'discover': Discover, 'query': Query}
+
 '''
```

### Comparing `ioxplugin-1.0.7/ioxplugin/iox_main_template.py` & `ioxplugin-1.0.9/ioxplugin/iox_main_template.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/iox_node_gen.py` & `ioxplugin-1.0.9/ioxplugin/iox_node_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,14 @@
 
         defaults=[self.nodedef.parent if self.nodedef.parent else self.nodedef.id,  self.nodedef.id,  self.nodedef.name]
         class_def.body.append(ast_util.astAddClassInit(self.nodedef.isController, defaults, None))
         if self.nodedef.isController:
             pass
             #set protocol handler
             #class_def.body.append(ast_util.astSetPluginFunc())
-            #class_def.body.append(ast_util.astParamHandlerFunc())
             #class_def.body.append(ast_util.astConfigFunc())
             #class_def.body.append(ast_util.astStartFunc())
             #class_def.body.append(ast_util.astStopFunc())
             #class_def.body.append(ast_util.astPollFunc())
             #class_def.body.append(ast_util.astAddAllNodesFunc())
             #class_def.body.append(ast_util.astAddNodeFunc())
         else:
```

### Comparing `ioxplugin-1.0.7/ioxplugin/iox_node_impl_gen.py` & `ioxplugin-1.0.9/ioxplugin/iox_node_impl_gen.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/iox_profile.py` & `ioxplugin-1.0.9/ioxplugin/iox_profile.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/iox_to_modbus.py` & `ioxplugin-1.0.9/ioxplugin/iox_to_modbus.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/iox_transport.py` & `ioxplugin-1.0.9/ioxplugin/iox_transport.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/log.py` & `ioxplugin-1.0.9/ioxplugin/log.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/main_gen.py` & `ioxplugin-1.0.9/ioxplugin/main_gen.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/new_project.py` & `ioxplugin-1.0.9/ioxplugin/new_project.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/node_properties.py` & `ioxplugin-1.0.9/ioxplugin/node_properties.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/nodedef.py` & `ioxplugin-1.0.9/ioxplugin/nodedef.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/oauth_service.py` & `ioxplugin-1.0.9/ioxplugin/oauth_service.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/plugin.py` & `ioxplugin-1.0.9/ioxplugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 
 
 class Plugin:
 
     def __init__(self, plugin_file, path:str=None, schema=PLUGIN_SCHEMA_FILE):
         self.path = os.path.dirname(plugin_file) if path == None else path
+        self.path = './' if self.path == '' else self.path
         init_ext_logging(self.path)
         self.meta = None
         self.editors=Editors()
         self.nodedefs:NodeDefs = None
         self.protocol:Protocol = None
         
         self.isValid = False
```

### Comparing `ioxplugin-1.0.7/ioxplugin/plugin_meta.py` & `ioxplugin-1.0.9/ioxplugin/plugin_meta.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/properties.py` & `ioxplugin-1.0.9/ioxplugin/properties.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/protocol.py` & `ioxplugin-1.0.9/ioxplugin/protocol.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/uom.py` & `ioxplugin-1.0.9/ioxplugin/uom.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin/validator.py` & `ioxplugin-1.0.9/ioxplugin/validator.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.7/ioxplugin.egg-info/PKG-INFO` & `ioxplugin-1.0.9/ioxplugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 1.0.7
+Version: 1.0.9
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-1.0.7/ioxplugin.egg-info/SOURCES.txt` & `ioxplugin-1.0.9/ioxplugin.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -25,9 +25,14 @@
 ioxplugin/uom.py
 ioxplugin/validator.py
 ioxplugin.egg-info/PKG-INFO
 ioxplugin.egg-info/SOURCES.txt
 ioxplugin.egg-info/dependency_links.txt
 ioxplugin.egg-info/requires.txt
 ioxplugin.egg-info/top_level.txt
+tests/ModbusControllerNode.py
+tests/ModbusDeviceNode.py
+tests/ModbusProtocolHandler.py
 tests/__init__.py
-tests/test_ioxplugin.py
+tests/modbus.py
+tests/test_ioxplugin.py
+tests/version.py
```

### Comparing `ioxplugin-1.0.7/setup.py` & `ioxplugin-1.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ioxplugin',
-    version='1.0.7',
+    version='1.0.9',
     packages=find_packages(),
     description='IoX Plugin Helper Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Michel Kohanim',
     author_email='support@universal-devices.com',
     url='https://github.com/universaldevices/ioxplugin.git',
```

