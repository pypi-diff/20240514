# Comparing `tmp/maxray-0.1.1.tar.gz` & `tmp/maxray-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxray-0.1.1.tar", max compression
+gzip compressed data, was "maxray-0.2.0.tar", max compression
```

## Comparing `maxray-0.1.1.tar` & `maxray-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1365 2024-05-04 02:53:18.136745 maxray-0.1.1/README.md
--rw-r--r--   0        0        0     9335 2024-05-04 02:53:18.136745 maxray-0.1.1/maxray/__init__.py
--rw-r--r--   0        0        0    18316 2024-05-04 02:53:18.136745 maxray-0.1.1/maxray/transforms.py
--rw-r--r--   0        0        0      191 2024-05-04 02:53:18.136745 maxray-0.1.1/maxray/walkers.py
--rw-r--r--   0        0        0      831 2024-05-04 02:53:26.620804 maxray-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 maxray-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1365 2024-05-14 10:28:54.697608 maxray-0.2.0/README.md
+-rw-r--r--   0        0        0     9387 2024-05-14 10:28:54.697608 maxray-0.2.0/maxray/__init__.py
+-rw-r--r--   0        0        0    21807 2024-05-14 10:28:54.697608 maxray-0.2.0/maxray/transforms.py
+-rw-r--r--   0        0        0      191 2024-05-14 10:28:54.697608 maxray-0.2.0/maxray/walkers.py
+-rw-r--r--   0        0        0      819 2024-05-14 10:29:02.017620 maxray-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 maxray-0.2.0/PKG-INFO
```

### Comparing `maxray-0.1.1/README.md` & `maxray-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `maxray-0.1.1/maxray/__init__.py` & `maxray-0.2.0/maxray/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,19 +22,19 @@
             case Err(err):
                 logger.error(err)
                 return fn
 
     return inner
 
 
-def xray(walker):
+def xray(walker, **kwargs):
     """
     Immutable version of `maxray` - expressions are passed to `walker` but its return value is ignored and the original code execution is left unchanged.
     """
-    return maxray(walker, mutable=False)
+    return maxray(walker, **kwargs, mutable=False)
 
 
 _GLOBAL_SKIP_MODULES = {
     "abc",  # excessive inheritance and super calls in scikit-learn
     "inspect",  # don't want to screw this module up
     "pathlib",  # internally used in transform for checking source file exists
     "re",  # internals of regexp have a lot of uninteresting step methods
@@ -61,27 +61,30 @@
 _GLOBAL_WRITER_ACTIVE_FLAG = ContextVar("writer_active (global)", default=False)
 
 # We don't want to recompile the same function over and over - so our cache needs to be global
 _MAXRAY_FN_CACHE = dict()
 
 
 def callable_allowed_for_transform(x, ctx: NodeContext):
+    if getattr(x, "__module__", None) in _GLOBAL_SKIP_MODULES:
+        return False
+
     module_path = ctx.fn_context.module.split(".")
     if module_path[0] in _GLOBAL_SKIP_MODULES:
         return False
     # TODO: deal with nonhashable objects and callables and other exotic types properly
     return (
         not hasattr(x, "_MAXRAY_TRANSFORMED")
         and callable(x)
         and callable(getattr(x, "__hash__", None))
         and getattr(type(x), "__module__", None) not in {"ctypes"}
     )
 
 
-def _maxray_walker_handler(x, ctx):
+def _maxray_walker_handler(x, ctx: NodeContext):
     # We ignore writer calls triggered by code execution in other writers to prevent easily getting stuck in recursive hell
     if _GLOBAL_WRITER_ACTIVE_FLAG.get():
         return x
 
     # 1. logic to recursively patch callables
     if callable_allowed_for_transform(x, ctx):
         # TODO: don't cache objects w/ __call__
@@ -151,15 +154,19 @@
     finally:
         _GLOBAL_WRITER_ACTIVE_FLAG.reset(global_write_active_token)
 
     return x
 
 
 def maxray(
-    writer: Callable[[Any, NodeContext], Any], skip_modules=frozenset(), *, mutable=True
+    writer: Callable[[Any, NodeContext], Any],
+    skip_modules=frozenset(),
+    *,
+    mutable=True,
+    pass_scope=False,
 ):
     """
     A transform that recursively hooks into all further calls made within the function, so that `writer` will (in theory) observe every single expression evaluated by the Python interpreter occurring as part of the decorated function call.
 
     There are some limitations to be aware of:
     - Be careful to avoid infinite recursion: the source code of the writer will not be transformed but it may call methods that have been monkey-patched that result in more calls to the writer function.
     - Objects that are not yet fully initialised may not behave as expected - e.g. repr may throw an error because of a missing property
@@ -175,14 +182,15 @@
     # except Exception as e:
     #     logger.exception(e)
     #     logger.error("Couldn't get locals")
     #     caller_locals = {}
     # finally:
     #     del frame
 
+    # TODO: allow configuring injection of variables into exec scope
     caller_locals = {}
 
     def recursive_transform(fn):
         _MAXRAY_REGISTERED_HOOKS.append(
             W_erHook(
                 writer,
                 ACTIVE_FLAG,
@@ -193,48 +201,43 @@
         )
 
         # Fixes `test_double_decorators_with_locals`: repeated transforms are broken because stuffing closures into locals doesn't work the second time around
         if hasattr(fn, "_MAXRAY_TRANSFORMED"):
             fn_transform = fn
         else:
             match recompile_fn_with_transform(
-                fn, _maxray_walker_handler, initial_scope=caller_locals
+                fn,
+                _maxray_walker_handler,
+                initial_scope=caller_locals,
+                pass_scope=pass_scope,
             ):
                 case Ok(fn_transform):
                     pass
                 case Err(err):
                     # Errors are only displayed at top-level, when the user has manually annotated a function with @xray or the like
                     logger.error(err)
                     return fn
 
         # BUG: We can't do @wraps if it's a callable instance, right?
         if inspect.iscoroutinefunction(fn):
 
             @wraps(fn)
             async def fn_with_context_update(*args, **kwargs):
-                # already active on stack
-                if ACTIVE_FLAG.get():
-                    return await fn_transform(*args, **kwargs)
-
-                ACTIVE_FLAG.set(True)
+                prev_token = ACTIVE_FLAG.set(True)
                 try:
                     return await fn_transform(*args, **kwargs)
                 finally:
-                    ACTIVE_FLAG.set(False)
+                    ACTIVE_FLAG.reset(prev_token)
         else:
 
             @wraps(fn)
             def fn_with_context_update(*args, **kwargs):
-                # already active on stack
-                if ACTIVE_FLAG.get():
-                    return fn_transform(*args, **kwargs)
-
-                ACTIVE_FLAG.set(True)
+                prev_token = ACTIVE_FLAG.set(True)
                 try:
                     return fn_transform(*args, **kwargs)
                 finally:
-                    ACTIVE_FLAG.set(False)
+                    ACTIVE_FLAG.reset(prev_token)
 
         fn_with_context_update._MAXRAY_TRANSFORMED = True
         return fn_with_context_update
 
     return recursive_transform
```

### Comparing `maxray-0.1.1/maxray/transforms.py` & `maxray-0.2.0/maxray/transforms.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import sys
 
 from textwrap import dedent
 from pathlib import Path
 from dataclasses import dataclass
 from copy import deepcopy
 from result import Result, Ok, Err
+from contextvars import ContextVar
+from functools import wraps
 
 from typing import Any, Callable
 
 from loguru import logger
 
 
 _METHOD_MANGLE_NAME = "vdxivosjdovs_method"
@@ -27,15 +29,19 @@
 @dataclass
 class FnContext:
     impl_fn: Callable
     name: str
     module: str
     source: str
     source_file: str
-    # TODO: add location as well
+    call_count: ContextVar[int]
+
+    def __repr__(self):
+        # Call count not included in repr so the same source location can be "grouped by" over multiple calls
+        return f"{self.module}/{self.name}"
 
 
 @dataclass
 class NodeContext:
     id: str
     """
     Identifier for the type of syntax node this event came from. For example:
@@ -48,35 +54,41 @@
     fn_context: FnContext
     """
     Properties of the function containing this node.
     """
 
     location: tuple[int, int, int, int]
 
+    local_scope: Any = None
+
     def __repr__(self):
-        return f"{self.fn_context.module}/{self.fn_context.name}/{self.id}"
+        return f"{self.fn_context}/{self.id}"
 
 
 class FnRewriter(ast.NodeTransformer):
     def __init__(
         self,
         transform_fn,
         fn_context: FnContext,
         *,
         instance_type: str | None,
         dedent_chars: int = 0,
+        record_call_counts: bool = True,
+        pass_locals_on_return: bool = False,
     ):
         """
         If we're transforming a method, instance type should be the __name__ of the class. Otherwise, None.
         """
 
         self.transform_fn = transform_fn
         self.fn_context = fn_context
         self.instance_type = instance_type
         self.dedent_chars = dedent_chars
+        self.record_call_counts = record_call_counts
+        self.pass_locals_on_return = pass_locals_on_return
 
         # the first `def` we encounter is the one that we're transforming. Subsequent ones will be nested/within class definitions.
         self.fn_count = 0
 
     def is_method(self):
         return self.instance_type is not None
 
@@ -85,52 +97,67 @@
         # workaround for https://github.com/python/cpython/issues/108469 (fixed in python 3.12)
         try:
             return ast.unparse(node)
         except ValueError as e:
             return "<UNUNPARSEABLE>"
 
     @staticmethod
+    def safe_show_ast(node):
+        return ast.dump(node, indent=4)
+
+    @staticmethod
     def is_private_class_name(identifier_name: str):
         return (
             identifier_name.startswith("__")
             and not identifier_name.endswith("__")
             and identifier_name.strip("_")
         )
 
     def recover_source(self, pre_node):
         segment = ast.get_source_segment(self.fn_context.source, pre_node, padded=False)
         if segment is None:
             return self.safe_unparse(pre_node)
         return segment
 
-    def build_transform_node(self, node, label, node_source=None):
+    def build_transform_node(self, node, label, node_source=None, pass_locals=False):
         """
         Builds the "inspection" node that wraps the original source node - passing the (value, context) pair to `transform_fn`.
         """
         if node_source is None:
             node_source = self.safe_unparse(node)
 
         line_offset = self.fn_context.impl_fn.__code__.co_firstlineno - 2
         col_offset = self.dedent_chars
+
+        context_args = [
+            ast.Constant(label),
+            ast.Constant(node_source),
+            # Name is injected into the exec scope by `recompile_fn_with_transform`
+            ast.Name(id="_MAXRAY_FN_CONTEXT", ctx=ast.Load()),
+            ast.Constant(
+                (
+                    line_offset + node.lineno,
+                    line_offset + node.end_lineno,
+                    node.col_offset + col_offset,
+                    node.end_col_offset + col_offset,
+                )
+            ),
+        ]
+
+        if pass_locals:
+            context_args.append(
+                ast.Call(
+                    func=ast.Name(id="_MAXRAY_BUILTINS_LOCALS", ctx=ast.Load()),
+                    args=[],
+                    keywords=[],
+                ),
+            )
         context_node = ast.Call(
             func=ast.Name(id=NodeContext.__name__, ctx=ast.Load()),
-            args=[
-                ast.Constant(label),
-                ast.Constant(node_source),
-                # Name is injected into the exec scope by `recompile_fn_with_transform`
-                ast.Name(id="_MAXRAY_FN_CONTEXT", ctx=ast.Load()),
-                ast.Constant(
-                    (
-                        line_offset + node.lineno,
-                        line_offset + node.end_lineno,
-                        node.col_offset + col_offset,
-                        node.end_col_offset + col_offset,
-                    )
-                ),
-            ],
+            args=context_args,
             keywords=[],
         )
 
         return ast.Call(
             func=ast.Name(id=self.transform_fn.__name__, ctx=ast.Load()),
             args=[node, context_node],
             keywords=[],
@@ -181,30 +208,44 @@
     def visit_Assign(self, node: ast.Assign) -> Any:
         new_node = self.generic_visit(node)
         assert isinstance(new_node, ast.Assign)
         # node = new_node
         # node.value = self.build_transform_node(new_node, f"assign/(multiple)")
         return node
 
+    def visit_Return(self, node: ast.Return) -> Any:
+        node_pre = deepcopy(node)
+
+        if node.value is None:
+            node.value = ast.Constant(None)
+
+        # Note: For a plain `return` statement, there's no source for a thing that *isn't* returned
+        value_source_pre = self.recover_source(node.value)
+
+        node = self.generic_visit(node)
+
+        # TODO: Check source locations are correct here
+        ast.fix_missing_locations(node)
+        node.value = self.build_transform_node(
+            node.value,
+            f"return/{value_source_pre}",
+            node_source=value_source_pre,
+            pass_locals=self.pass_locals_on_return,
+        )
+
+        return ast.copy_location(node, node_pre)
+
     def visit_Call(self, node):
         source_pre = self.recover_source(node)
 
         node_pre = deepcopy(node)
 
         node = self.generic_visit(node)  # mutates
 
         # the function/callable instance itself is observed by Name/Attribute/... nodes
-
-        target = node.func
-        match target:
-            case ast.Name():
-                logger.debug(f"Visiting call to function {target.id}")
-            case ast.Attribute():
-                logger.debug(f"Visiting call to attribute {target.attr}")
-
         return ast.copy_location(
             self.build_transform_node(
                 node, f"call/{source_pre}", node_source=source_pre
             ),
             node_pre,
         )
 
@@ -239,19 +280,36 @@
             logger.info(
                 f"Wiped decorators at level {self.fn_count} for {self.fn_context.impl_fn}: {node.decorator_list}"
             )
             # If we didn't clear, decorators would be applied twice - screwing up routing handling in libraries like `quart`: `@app.post("/generate")`
             node.decorator_list = []
 
         # Removes type annotations from the call for safety as they're evaluated at definition-time rather than call-time
-        # This may not be needed now that locals are (usually) captured properly
+        # Necessary because some packages do `if typing.TYPE_CHECKING` imports
         for arg in node.args.args:
             arg.annotation = None
 
+        for arg in node.args.kwonlyargs:
+            arg.annotation = None
+
+        node.returns = None
+
         out = ast.copy_location(self.generic_visit(node), pre_node)
+
+        # Add statements after visiting so that walk handlers aren't called on this internal code
+        if self.fn_count == 1 and self.record_call_counts:
+            # has to be applied as a decorator so that inner recursive calls of the fn are tracked properly
+            node.decorator_list.append(
+                ast.Call(
+                    func=ast.Name(id="_MAXRAY_DECORATE_WITH_COUNTER", ctx=ast.Load()),
+                    args=[ast.Name(id="_MAXRAY_CALL_COUNTER", ctx=ast.Load())],
+                    keywords=[],
+                )
+            )
+
         return out
 
     def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef) -> Any:
         """
         Copied directly from FunctionDef
         TODO: FIX OR REFACTOR
         """
@@ -306,14 +364,15 @@
 
 def recompile_fn_with_transform(
     source_fn,
     transform_fn,
     ast_pre_callback=None,
     ast_post_callback=None,
     initial_scope={},
+    pass_scope=False,
 ) -> Result[Callable, str]:
     """
     Recompiles `source_fn` so that essentially every node of its AST tree is wrapped by a call to `transform_fn` with the evaluated value along with context information about the source code.
     """
     # handle `functools.wraps`
     if hasattr(source_fn, "__wrapped__"):
         # SOUNDNESS: failure when decorators aren't applied at the definition site (will look for the original definition, ignoring any transformations that have been applied before the wrap but after definition)
@@ -375,32 +434,42 @@
             case type():
                 # Descriptor
                 parent_cls = source_fn.__self__
             case _:
                 # Bound method
                 parent_cls = type(source_fn.__self__)
 
+    fn_call_counter = ContextVar("maxray_call_counter", default=0)
     fn_context = FnContext(
-        source_fn, source_fn.__name__, module.__name__, source, sourcefile
+        source_fn,
+        source_fn.__name__,
+        module.__name__,
+        source,
+        sourcefile,
+        fn_call_counter,
     )
     transformed_fn_ast = FnRewriter(
         transform_fn,
         fn_context,
         instance_type=parent_cls.__name__ if fn_is_method else None,
         dedent_chars=dedent_chars,
+        pass_locals_on_return=pass_scope,
     ).visit(fn_ast)
     ast.fix_missing_locations(transformed_fn_ast)
 
     if ast_post_callback is not None:
         ast_post_callback(transformed_fn_ast)
 
     scope = {
         transform_fn.__name__: transform_fn,
         NodeContext.__name__: NodeContext,
         "_MAXRAY_FN_CONTEXT": fn_context,
+        "_MAXRAY_CALL_COUNTER": fn_call_counter,
+        "_MAXRAY_DECORATE_WITH_COUNTER": count_calls_with,
+        "_MAXRAY_BUILTINS_LOCALS": locals,
     }
     scope.update(initial_scope)
 
     # Add class-private names to scope (though only should be usable as a default argument)
     # TODO: should apply to all definitions within a class scope - so @staticmethod descriptors as well...
     if fn_is_method:
         scope.update(
@@ -446,15 +515,20 @@
             ),
             scope,
             scope,
         )
     except Exception as e:
         logger.exception(e)
         logger.error(
-            f"Failed to compile function {source_fn.__name__} in its module {module}"
+            f"Failed to compile function `{source_fn.__name__}` at '{sourcefile}' in its module {module}"
+        )
+        logger.debug(f"Relevant original source code:\n{source}")
+        logger.debug(f"Corresponding AST:\n{FnRewriter.safe_show_ast(fn_ast)}")
+        logger.debug(
+            f"Transformed code we attempted to compile:\n{FnRewriter.safe_unparse(transformed_fn_ast)}"
         )
 
         # FALLBACK: in numpy.core.numeric, they define `@set_module` that rewrites __module__ so inspect gives us the wrong module to correctly re-execute the def in
         # sourcefile is still correct so let's try use `sys.modules`
 
         file_to_modules = {
             getattr(mod, "__file__", None): mod for mod in sys.modules.values()
@@ -466,15 +540,14 @@
                     compile(
                         transformed_fn_ast,
                         filename=f"<{source_fn.__name__}>",
                         mode="exec",
                     ),
                     scope,
                     scope,
-                    # closure=fn.__closure__,
                 )
             except Exception as e:
                 logger.exception(e)
                 return Err(
                     f"Re-def of function {get_fn_name(source_fn)} in its source file module at {sourcefile} also failed"
                 )
         else:
@@ -498,7 +571,40 @@
     # unmangle the name again - it's possible some packages might use __name__ internally for registries and whatnot
     transformed_fn.__name__ = source_fn.__name__
 
     # way to keep track of which functions we've already transformed
     transformed_fn._MAXRAY_TRANSFORMED = True
 
     return Ok(transformed_fn)
+
+
+def count_calls_with(counter: ContextVar):
+    def inner(fn):
+        # TODO: synchronisation/context?
+        total_calls_count = 0
+
+        if inspect.iscoroutinefunction(fn):
+
+            @wraps(fn)
+            async def fn_with_counter(*args, **kwargs):
+                nonlocal total_calls_count
+                total_calls_count += 1
+                reset_call = counter.set(total_calls_count)
+                try:
+                    return await fn(*args, **kwargs)
+                finally:
+                    counter.reset(reset_call)
+        else:
+
+            @wraps(fn)
+            def fn_with_counter(*args, **kwargs):
+                nonlocal total_calls_count
+                total_calls_count += 1
+                reset_call = counter.set(total_calls_count)
+                try:
+                    return fn(*args, **kwargs)
+                finally:
+                    counter.reset(reset_call)
+
+        return fn_with_counter
+
+    return inner
```

### Comparing `maxray-0.1.1/PKG-INFO` & `maxray-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxray
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 Author: blepabyte
 Author-email: 255@blepabyte.me
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

