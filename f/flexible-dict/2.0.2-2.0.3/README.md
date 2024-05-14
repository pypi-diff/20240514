# Comparing `tmp/flexible_dict-2.0.2.tar.gz` & `tmp/flexible_dict-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexible_dict-2.0.2.tar", last modified: Fri May 10 09:47:46 2024, max compression
+gzip compressed data, was "flexible_dict-2.0.3.tar", last modified: Tue May 14 10:39:12 2024, max compression
```

## Comparing `flexible_dict-2.0.2.tar` & `flexible_dict-2.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:47:46.866537 flexible_dict-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-10 09:47:46.866537 flexible_dict-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:47:46.866537 flexible_dict-2.0.2/flexible_dict/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/flexible_dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/flexible_dict/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-10 09:47:46.000000 flexible_dict-2.0.2/flexible_dict/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/flexible_dict/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    25169 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/flexible_dict/json_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:47:46.866537 flexible_dict-2.0.2/flexible_dict/script/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/flexible_dict/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/flexible_dict/script/class_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/flexible_dict/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/flexible_dict/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:47:46.866537 flexible_dict-2.0.2/flexible_dict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-10 09:47:46.000000 flexible_dict-2.0.2/flexible_dict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 09:47:46.000000 flexible_dict-2.0.2/flexible_dict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:47:46.000000 flexible_dict-2.0.2/flexible_dict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-10 09:47:46.000000 flexible_dict-2.0.2/flexible_dict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/run_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:47:46.866537 flexible_dict-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-10 09:47:42.000000 flexible_dict-2.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:39:12.784003 flexible_dict-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-14 10:39:12.784003 flexible_dict-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:39:12.784003 flexible_dict-2.0.3/flexible_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-14 10:39:12.000000 flexible_dict-2.0.3/flexible_dict/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26283 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/json_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:39:12.784003 flexible_dict-2.0.3/flexible_dict/script/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/script/class_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/flexible_dict/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:39:12.784003 flexible_dict-2.0.3/flexible_dict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-14 10:39:12.000000 flexible_dict-2.0.3/flexible_dict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-14 10:39:12.000000 flexible_dict-2.0.3/flexible_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:39:12.000000 flexible_dict-2.0.3/flexible_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 10:39:12.000000 flexible_dict-2.0.3/flexible_dict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/run_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:39:12.784003 flexible_dict-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 10:39:07.000000 flexible_dict-2.0.3/tox.ini
```

### Comparing `flexible_dict-2.0.2/PKG-INFO` & `flexible_dict-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_dict
-Version: 2.0.2
+Version: 2.0.3
 Summary: A flexible way to access dict data instead of built-in dict.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/flexible_dict
 Description-Content-Type: text/markdown
 Requires-Dist: dataclasses; python_version < "3.7"
 Requires-Dist: typing_extensions; python_version < "3.8"
```

### Comparing `flexible_dict-2.0.2/README.md` & `flexible_dict-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.2/flexible_dict/__main__.py` & `flexible_dict-2.0.3/flexible_dict/__main__.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.2/flexible_dict/adapter.py` & `flexible_dict-2.0.3/flexible_dict/adapter.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.2/flexible_dict/json_object.py` & `flexible_dict-2.0.3/flexible_dict/json_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,19 +86,27 @@
     name: str = dataclasses.field(init=False, default=None)
     type: Any = dataclasses.field(init=False, default=None)
     _field_type: _FIELD_BASE = dataclasses.field(init=False, default=_FIELD_DICTKEY)
 
     # additional metadata
     metadata: Dict[Any, Any] = dataclasses.field(default_factory=dict)
 
+class DefaultScope:
+    GETTER = 1
+    INIT = 2
+
 @dataclasses.dataclass
 class ProcessorConfig:
     # default value when access an absent key in class scope
     getter_default: Any = MISSING
 
+    # if set a default value but not a field, determine which scope should the value be used
+    # scope can be getter or init, and can all set active
+    default_scopes: int = DefaultScope.GETTER
+
     # auto set encoder and decoder for field
     adapter_detector: AdapterDetector = dataclasses.field(default_factory=AdapterDetector)
 
     # whether to create a new __init__ function
     create_init_func: bool = True
 
     # whether to create a function to iter all field values
@@ -189,15 +197,20 @@
         default = getattr(cls, a_name, MISSING)
         if isinstance(default, Field):
             f = default
         else:
             if isinstance(default, types.MemberDescriptorType):
                 # This is a field in __slots__, so it has no default value.
                 default = MISSING
-            f = Field(init_default=default)
+            getter_default = init_default = MISSING
+            if self.config.default_scopes & DefaultScope.GETTER:
+                getter_default = default
+            if self.config.default_scopes & DefaultScope.INIT:
+                init_default = default
+            f = Field(init_default=init_default, getter_default=getter_default)
 
         # Only at this point do we know the name and the type.  Set them.
         f.name = a_name
         f.type = a_type
 
         # If missing key, set as name.
         if self.is_missing(f.key):
@@ -469,21 +482,32 @@
             f"for {d_name} in {ds_name}:",
             f" {self_name}.update({d_name})",
         ])
 
         # walk fields to update and encode
         for f in fields:
             if f._field_type is _FIELD_DICTKEY:
+                should_encode = callable(f.encoder)
+                if should_encode:
+                    _locals[f'_encoder_{f.name}'] = f.encoder
+
                 # value stored in dict would be correctly encoded by setting with `.`
-                body_lines.extend([
-                    f"if {f.name} is not MISSING:",
-                    f" {self_name}.{f.name} = {f.name}",
-                    f"elif _key_{f.name} in {self_name}:",
-                    f" {self_name}.{f.name} = {self_name}[_key_{f.name}]",
-                ])
+
+                # if value given, stored in the dict
+                body_lines.append(f"if {f.name} is not MISSING:")
+                if should_encode:
+                    body_lines.append(f" {f.name} = _encoder_{f.name}({f.name})")
+                body_lines.append(f" {self_name}[_key_{f.name}] = {f.name}")
+
+                # if value not given but key already in the dict, that means the values is passed in a dict
+                # encode the value if necessary
+                if should_encode:
+                    body_lines.append(f"elif _key_{f.name} in {self_name}:")
+                    body_lines.append(f" {self_name}[_key_{f.name}] = _encoder_{f.name}({self_name}[_key_{f.name}])")
+                    
                 # set default value
                 if not self.is_missing(f.init_default):
                     _locals[f'_default_{f.name}'] = f.init_default
                     body_lines.extend([
                         f"else:",
                         f" {self_name}[_key_{f.name}] = _default_{f.name}",
                     ])
```

### Comparing `flexible_dict-2.0.2/flexible_dict/script/class_builder.py` & `flexible_dict-2.0.3/flexible_dict/script/class_builder.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.2/flexible_dict/utils.py` & `flexible_dict-2.0.3/flexible_dict/utils.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-2.0.2/flexible_dict.egg-info/PKG-INFO` & `flexible_dict-2.0.3/flexible_dict.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_dict
-Version: 2.0.2
+Version: 2.0.3
 Summary: A flexible way to access dict data instead of built-in dict.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/flexible_dict
 Description-Content-Type: text/markdown
 Requires-Dist: dataclasses; python_version < "3.7"
 Requires-Dist: typing_extensions; python_version < "3.8"
```

### Comparing `flexible_dict-2.0.2/pyproject.toml` & `flexible_dict-2.0.3/pyproject.toml`

 * *Files identical despite different names*

