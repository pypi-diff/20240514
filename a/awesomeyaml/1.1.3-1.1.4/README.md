# Comparing `tmp/awesomeyaml-1.1.3.tar.gz` & `tmp/awesomeyaml-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awesomeyaml-1.1.3.tar", last modified: Wed Mar  6 10:02:53 2024, max compression
+gzip compressed data, was "awesomeyaml-1.1.4.tar", last modified: Tue May 14 18:36:47 2024, max compression
```

## Comparing `awesomeyaml-1.1.3.tar` & `awesomeyaml-1.1.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 l.dudziak (966277671) l.dudziak (966277671)        0 2024-03-06 10:02:53.872594 awesomeyaml-1.1.3/
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    11357 2024-03-06 09:38:56.443964 awesomeyaml-1.1.3/LICENSE
--rw-r--r--   0 l.dudziak (966277671) l.dudziak (966277671)    30757 2024-03-06 10:02:53.872594 awesomeyaml-1.1.3/PKG-INFO
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    30370 2024-03-06 10:00:00.462036 awesomeyaml-1.1.3/README.md
-drwxrwxr-x   0 l.dudziak (966277671) l.dudziak (966277671)        0 2024-03-06 10:02:53.872594 awesomeyaml-1.1.3/awesomeyaml/
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1795 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/__init__.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)      138 2024-03-06 10:02:53.868594 awesomeyaml-1.1.3/awesomeyaml/_dist_info.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    18899 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/builder.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    12488 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/config.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     5009 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/errors.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     8880 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/eval_context.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     7824 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/namespace.py
-drwxrwxr-x   0 l.dudziak (966277671) l.dudziak (966277671)        0 2024-03-06 10:02:53.872594 awesomeyaml-1.1.3/awesomeyaml/nodes/
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)      681 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/__init__.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     2089 2024-03-06 09:42:45.727430 awesomeyaml-1.1.3/awesomeyaml/nodes/append.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     4582 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/bind.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     3213 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/call.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1304 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/clear.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    20454 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/composed.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     4836 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/dict.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    13420 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/eval.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     2193 2024-03-06 09:52:39.171627 awesomeyaml-1.1.3/awesomeyaml/nodes/extend.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1943 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/fstr.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     4589 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/function.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1734 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/import.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     5482 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/include.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     6668 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/list.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    21453 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/node.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     4680 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/node_path.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     6208 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/path.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1148 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/prev.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1305 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/required.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     6634 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/scalar.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1189 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/stream.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     3288 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/tuple.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1502 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/nodes/xref.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    10567 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/awesomeyaml/utils.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1997 2024-03-06 10:01:11.763077 awesomeyaml-1.1.3/awesomeyaml/version.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    25371 2024-03-06 10:00:44.142674 awesomeyaml-1.1.3/awesomeyaml/yaml.py
--rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     3365 2024-03-06 09:38:56.447964 awesomeyaml-1.1.3/setup.py
+drwxrwxr-x   0 l.dudziak (966277671) l.dudziak (966277671)        0 2024-05-14 18:36:47.548002 awesomeyaml-1.1.4/
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    11357 2024-03-06 09:38:56.443964 awesomeyaml-1.1.4/LICENSE
+-rw-r--r--   0 l.dudziak (966277671) l.dudziak (966277671)    30757 2024-05-14 18:36:47.548002 awesomeyaml-1.1.4/PKG-INFO
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    30370 2024-03-06 10:00:00.462036 awesomeyaml-1.1.4/README.md
+drwxrwxr-x   0 l.dudziak (966277671) l.dudziak (966277671)        0 2024-05-14 18:36:47.548002 awesomeyaml-1.1.4/awesomeyaml/
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1795 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/__init__.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)      138 2024-05-14 18:36:47.540002 awesomeyaml-1.1.4/awesomeyaml/_dist_info.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    18905 2024-05-14 18:06:49.330907 awesomeyaml-1.1.4/awesomeyaml/builder.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    12488 2024-05-14 17:49:18.317041 awesomeyaml-1.1.4/awesomeyaml/config.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     5015 2024-05-14 18:28:04.598324 awesomeyaml-1.1.4/awesomeyaml/errors.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     8578 2024-05-14 18:21:11.982614 awesomeyaml-1.1.4/awesomeyaml/eval_context.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     7824 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/namespace.py
+drwxrwxr-x   0 l.dudziak (966277671) l.dudziak (966277671)        0 2024-05-14 18:36:47.548002 awesomeyaml-1.1.4/awesomeyaml/nodes/
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)      681 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/__init__.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     2089 2024-03-06 09:42:45.727430 awesomeyaml-1.1.4/awesomeyaml/nodes/append.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     4582 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/bind.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     3213 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/call.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1304 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/clear.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    20454 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/composed.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     4836 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/dict.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    13420 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/eval.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     2193 2024-03-06 09:52:39.171627 awesomeyaml-1.1.4/awesomeyaml/nodes/extend.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1943 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/fstr.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     4589 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/function.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1734 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/import.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     5482 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/include.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     6668 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/list.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    21459 2024-05-14 18:06:58.499095 awesomeyaml-1.1.4/awesomeyaml/nodes/node.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     4680 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/node_path.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     6208 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/path.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1148 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/prev.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     4043 2024-05-14 18:23:49.849610 awesomeyaml-1.1.4/awesomeyaml/nodes/recurse.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1305 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/required.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     6634 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/scalar.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1189 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/stream.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     3288 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/tuple.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1502 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/nodes/xref.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    10567 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/awesomeyaml/utils.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     1997 2024-05-14 18:30:06.464597 awesomeyaml-1.1.4/awesomeyaml/version.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)    25951 2024-05-14 18:06:54.563014 awesomeyaml-1.1.4/awesomeyaml/yaml.py
+-rw-rw-r--   0 l.dudziak (966277671) l.dudziak (966277671)     3365 2024-03-06 09:38:56.447964 awesomeyaml-1.1.4/setup.py
```

### Comparing `awesomeyaml-1.1.3/LICENSE` & `awesomeyaml-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/PKG-INFO` & `awesomeyaml-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awesomeyaml
-Version: 1.1.3
+Version: 1.1.4
 Summary: Config-building utilities using YAML
 Home-page: https://github.com/SamsungLabs/awesomeyaml
 Download-URL: https://github.com/SamsungLabs/awesomeyaml
 Author: Łukasz Dudziak
 Author-email: l.dudziak@samsung.com
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `awesomeyaml-1.1.3/README.md` & `awesomeyaml-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/__init__.py` & `awesomeyaml-1.1.4/awesomeyaml/__init__.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/builder.py` & `awesomeyaml-1.1.4/awesomeyaml/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
         new_stage = self.stages[0].ayns.premerge(None)
         if new_stage is not self.stages[0]:
             try:
                 self.stages[0:1] = new_stage.stages
             except AttributeError:
                 self.stages[0] = new_stage
 
-        with errors.rethrow(errors.MergeError, self.stages[0], None, None):
+        with errors.rethrow_point(errors.MergeError, self.stages[0], None, None):
             self.stages[0].ayns._require_all_new([], 'the node comes from the first config tree in a merging sequence and the current config is empty')
         if len(self.stages) < 2:
             return
 
         root = self.stages[0]
         for i in range(1, len(self.stages)):
             root = root.ayns.merge(self.stages[i])
```

### Comparing `awesomeyaml-1.1.3/awesomeyaml/config.py` & `awesomeyaml-1.1.4/awesomeyaml/config.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/errors.py` & `awesomeyaml-1.1.4/awesomeyaml/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
 
 class UnsafeError(EvalError):
     base_msg = 'Avoiding execution of an !unsafe {} node under path: {}'
 
 
 @contextlib.contextmanager
-def rethrow(error_type, self, path, other):
+def rethrow_point(error_type, self, path, other):
     try:
         yield
     except error_type as e:
         if shorten_traceback:
             raise
         else:
             raise error_type(error_msg=None, node=self, path=path, extra_node=other) from e
```

### Comparing `awesomeyaml-1.1.3/awesomeyaml/eval_context.py` & `awesomeyaml-1.1.4/awesomeyaml/eval_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,22 +117,14 @@
 
     def get_node(self, *path, **kwargs):
         path = NodePath.get_list_path(*path)
         if str(path) in self._eval_cache:
             return self._eval_cache[str(path)]
         return self.cfg.ayns.get_node(path, **kwargs)
 
-    def get_evaluated_node(self, nodepath):
-        nodepath = NodePath.get_list_path(nodepath, check_types=False) or NodePath()
-        node = self.ayns.get_node(nodepath)
-        if str(nodepath) in self._eval_cache:
-            return node
-
-        return self.evaluate_node(node, prefix=nodepath)
-
     @errors.api_entry
     def evaluate_node(self, cfgobj, prefix=None):
         if not isinstance(cfgobj, ConfigNode):
             return cfgobj
 
         self._eval_stack.append(prefix)
         prefix = NodePath.get_list_path(prefix, check_types=False) or NodePath()
```

### Comparing `awesomeyaml-1.1.3/awesomeyaml/namespace.py` & `awesomeyaml-1.1.4/awesomeyaml/namespace.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/__init__.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/append.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/append.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/bind.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/bind.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/call.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/call.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/clear.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/clear.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/composed.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/composed.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/dict.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/dict.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/eval.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/eval.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/extend.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/extend.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/fstr.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/fstr.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/function.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/function.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/import.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/import.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/include.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/include.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/list.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/list.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/node.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def decorator(func):
         def impl(*args, **kwargs):
             self = args[0]
             path = args[1] if len(args) > 1 else kwargs['path']
             other = args[2] if len(args) > 2 else kwargs.get('other', None)
             if not isinstance(other, ConfigNode):
                 other = None
-            with errors.rethrow(error_type, self, path, other):
+            with errors.rethrow_point(error_type, self, path, other):
                 return func(*args, **kwargs)
 
         return impl
     return decorator
 
 
 rethrow_as_preprocess_error = decorator_factory(errors.PreprocessError)
```

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/node_path.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/node_path.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/path.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/path.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/prev.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/prev.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/required.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/required.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/scalar.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/scalar.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/stream.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/stream.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/tuple.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/tuple.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/nodes/xref.py` & `awesomeyaml-1.1.4/awesomeyaml/nodes/xref.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/utils.py` & `awesomeyaml-1.1.4/awesomeyaml/utils.py`

 * *Files identical despite different names*

### Comparing `awesomeyaml-1.1.3/awesomeyaml/version.py` & `awesomeyaml-1.1.4/awesomeyaml/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-version = '1.1.3'
+version = '1.1.4'
 repo = 'unknown'
 commit = 'unknown'
 has_repo = False
 
 try:
     import git
     from pathlib import Path
```

### Comparing `awesomeyaml-1.1.3/awesomeyaml/yaml.py` & `awesomeyaml-1.1.4/awesomeyaml/yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     yaml.add_multi_representer(data_type, representer, Dumper=AwesomeyamlDumper)
 
 
 def rethrow_as_parsing_error(func):
     @functools.wraps(func)
     def impl(*args, **kwargs):
         node = args[2] if len(args) > 2 else args[1]
-        with errors.rethrow(errors.ParsingError, node, None, None):
+        with errors.rethrow_point(errors.ParsingError, node, None, None):
             return func(*args, **kwargs)
 
     return impl
 
 
 @contextlib.contextmanager
 def global_ctx(filename):
@@ -466,14 +466,27 @@
 @rethrow_as_parsing_error
 def _extend_constructor_md(loader, tag_suffix, node):
     from .nodes.extend import ExtendNode
     kwargs = _decode_metadata(tag_suffix)
     return _make_node(loader, node, kwargs=kwargs, node_type=ExtendNode)
 
 
+@rethrow_as_parsing_error
+def _rec_constructor(loader, node):
+    from .nodes.recurse import RecurseNode
+    return _make_node(loader, node, node_type=RecurseNode, dict_is_data=False, parse_scalars=False)
+
+
+@rethrow_as_parsing_error
+def _rec_constructor_md(loader, tag_suffix, node):
+    from .nodes.recurse import RecurseNode
+    kwargs = _decode_metadata(tag_suffix)
+    return _make_node(loader, node, kwargs=kwargs, node_type=RecurseNode, dict_is_data=False, parse_scalars=False)
+
+
 add_constructor('!del', _del_constructor)
 add_constructor('!weak', _weak_constructor)
 add_constructor('!force', _force_constructor)
 add_constructor('!merge', _merge_constructor)
 add_constructor('!append', _append_constructor)
 add_multi_constructor('!metadata:', _metadata_constructor)
 add_constructor('!include', _include_constructor)
@@ -500,14 +513,16 @@
 add_constructor('!new', _new_constructor)
 add_constructor('!notnew', _notnew_constructor)
 add_constructor('!unsafe', _unsafe_constructor)
 add_constructor('!clear', _clear_constructor)
 add_multi_constructor('!clear:', _clear_constructor_md)
 add_constructor('!extend', _extend_constructor)
 add_multi_constructor('!extend:', _extend_constructor_md)
+add_constructor('!rec', _rec_constructor)
+add_constructor('!rec:', _rec_constructor_md)
 
 
 def _node_representer(dumper, node):
     from .nodes.bind import BindNode
     tag, metadata, data = node.ayns.represent()
     if data is None:
         assert not tag
```

### Comparing `awesomeyaml-1.1.3/setup.py` & `awesomeyaml-1.1.4/setup.py`

 * *Files identical despite different names*

