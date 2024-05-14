# Comparing `tmp/clams_python-1.2.1.tar.gz` & `tmp/clams_python-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams_python-1.2.1.tar", last modified: Sun Apr 21 22:13:16 2024, max compression
+gzip compressed data, was "clams_python-1.2.2.tar", last modified: Tue May 14 20:12:07 2024, max compression
```

## Comparing `clams_python-1.2.1.tar` & `clams_python-1.2.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.213550 clams_python-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-21 22:12:50.000000 clams_python-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-21 22:12:50.000000 clams_python-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-21 22:13:16.213550 clams_python-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-21 22:12:50.000000 clams_python-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 22:12:50.000000 clams_python-1.2.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.205550 clams_python-1.2.1/clams/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.205550 clams_python-1.2.1/clams/app/
--rw-r--r--   0 runner    (1001) docker     (127)    19005 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.205550 clams_python-1.2.1/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (127)    21677 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.205550 clams_python-1.2.1/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.205550 clams_python-1.2.1/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/.dockerignore.template
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/.gitignore.template
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/Containerfile.template
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/LICENSE.template
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/README.md.template
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/app.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/metadata.py.template
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/requirements.txt.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/develop/templates/gha/
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/gha/for-clams-team.md.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/develop/templates/gha/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/gha/workflows/issue-assign.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/gha/workflows/issue-close.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/gha/workflows/publish.yml.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/mmif_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/mmif_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/mmif_utils/rewind.py
--rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/mmif_utils/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 22:12:50.000000 clams_python-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:13:16.213550 clams_python-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-21 22:12:50.000000 clams_python-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    23502 2024-04-21 22:12:50.000000 clams_python-1.2.1/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-21 22:12:50.000000 clams_python-1.2.1/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.194347 clams_python-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-14 20:11:42.000000 clams_python-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 20:11:42.000000 clams_python-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-14 20:12:07.194347 clams_python-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-14 20:11:42.000000 clams_python-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 20:11:42.000000 clams_python-1.2.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.190346 clams_python-1.2.2/clams/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.190346 clams_python-1.2.2/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    20238 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.190346 clams_python-1.2.2/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    21677 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.190346 clams_python-1.2.2/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.186346 clams_python-1.2.2/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.190346 clams_python-1.2.2/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/app/.dockerignore.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/app/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/app/Containerfile.template
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/app/LICENSE.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/app/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/app/app.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/app/metadata.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/app/requirements.txt.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.190346 clams_python-1.2.2/clams/develop/templates/gha/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/gha/for-clams-team.md.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.190346 clams_python-1.2.2/clams/develop/templates/gha/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/gha/workflows/issue-assign.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/gha/workflows/issue-close.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/develop/templates/gha/workflows/publish.yml.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.190346 clams_python-1.2.2/clams/mmif_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/mmif_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/mmif_utils/rewind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/mmif_utils/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.190346 clams_python-1.2.2/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.194347 clams_python-1.2.2/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-14 20:11:42.000000 clams_python-1.2.2/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.194347 clams_python-1.2.2/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 20:12:07.000000 clams_python-1.2.2/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.194347 clams_python-1.2.2/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-14 20:12:07.000000 clams_python-1.2.2/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-14 20:12:07.000000 clams_python-1.2.2/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:12:07.000000 clams_python-1.2.2/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 20:12:07.000000 clams_python-1.2.2/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 20:12:07.000000 clams_python-1.2.2/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 20:12:07.000000 clams_python-1.2.2/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 20:11:42.000000 clams_python-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:12:07.194347 clams_python-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-14 20:11:42.000000 clams_python-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:12:07.194347 clams_python-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    24769 2024-05-14 20:11:42.000000 clams_python-1.2.2/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-14 20:11:42.000000 clams_python-1.2.2/tests/test_clamscli.py
```

### Comparing `clams_python-1.2.1/LICENSE` & `clams_python-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/PKG-INFO` & `clams_python-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.2.1
+Version: 1.2.2
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers 
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mmif-python==1.0.13
+Requires-Dist: mmif-python==1.0.14
 Requires-Dist: Flask>=2
 Requires-Dist: Flask-RESTful>=0.3.9
 Requires-Dist: gunicorn>=20
 Requires-Dist: lapps>=0.0.2
 Requires-Dist: pydantic<2,>=1.8
 Requires-Dist: jsonschema>=3
```

### Comparing `clams_python-1.2.1/README.md` & `clams_python-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/__init__.py` & `clams_python-1.2.2/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/app/__init__.py` & `clams_python-1.2.2/clams/app/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,15 +174,22 @@
         casted = self.annotate_param_caster.cast(runtime_params)
         for parameter in self.metadata.parameters:
             if parameter.name in casted:
                 if parameter.choices and casted[parameter.name] not in parameter.choices:
                     raise ValueError(f"Value for parameter \"{parameter.name}\" must be one of {parameter.choices}.")
                 refined[parameter.name] = casted[parameter.name]
             elif parameter.default is not None:
-                refined[parameter.name] = parameter.default
+                # have to cast the default values as well, since 
+                # 1. `map` type default values are not actually expected as a map (dict)
+                # 2. developers can use data type not matching the spec
+                if isinstance(parameter.default, list):
+                    casted_default = self.annotate_param_caster.cast({parameter.name: list(map(str, parameter.default))})
+                else:
+                    casted_default = self.annotate_param_caster.cast({parameter.name: [str(parameter.default)]})
+                refined.update(casted_default)
             else:
                 raise ValueError(f"Cannot find configuration for a required parameter \"{parameter.name}\".")
         # raw input params are hidden under a special key
         refined[self._RAW_PARAMS_KEY] = runtime_params
         return refined
     
     def get_configuration(self, **runtime_params):
@@ -334,16 +341,16 @@
                  structures, but that is not in the scope of this Caster class. 
         """
         casted = {}
         for k, vs in args.items():
             assert isinstance(vs, list), f"Expected a list of values for key {k}, but got {vs} of type {type(vs)}"
             assert all(isinstance(v, str) for v in vs), f"Expected a list of strings for key {k}, but got {vs} of types {[type(v) for v in vs]}"
             if k in self.param_spec:
+                valuetype, multivalued = self.param_spec[k]
                 for v in vs:
-                    valuetype, multivalued = self.param_spec[k]
                     if multivalued or k not in casted:  # effectively only keeps the first value for non-multi params
                         if valuetype == bool:
                             v = self.bool_param(v)
                         elif valuetype == float:
                             v = self.float_param(v)
                         elif valuetype == int:
                             v = self.int_param(v)
@@ -354,19 +361,30 @@
                         if multivalued:
                             if valuetype == dict:
                                 casted.setdefault(k, {}).update(v)
                             else:
                                 casted.setdefault(k, []).append(v)
                         else: 
                             casted[k] = v
+                # when an empty value is passed (usually as a default value)
+                # just add an empty list or dict as a placeholder
+                # explicit check for `len == 0` is required to prevent 
+                # empty values are set for params that don't have default values
+                if multivalued and len(vs) == 0:
+                    if valuetype == dict:
+                        casted.setdefault(k, {})
+                    else:
+                        casted.setdefault(k, [])
             else:
-                if len(vs) > 1:
-                    casted[k] = vs
-                else:
+                # if the parameter is not defined in the spec, there's no easy way to figure out 
+                # the user's intention whether it should be a list (multivalued) or a single value.
+                if len(vs) == 1:
                     casted[k] = vs[0]
+                else:
+                    casted[k] = vs
         return casted  # pytype: disable=bad-return-type
 
     @staticmethod
     def bool_param(value) -> bool:
         """
         Helper function to convert string values to bool type.
         """
```

### Comparing `clams_python-1.2.1/clams/appmetadata/__init__.py` & `clams_python-1.2.2/clams/appmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/develop/__init__.py` & `clams_python-1.2.2/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/develop/templates/app/.gitignore.template` & `clams_python-1.2.2/clams/develop/templates/app/.gitignore.template`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/develop/templates/app/Containerfile.template` & `clams_python-1.2.2/clams/develop/templates/app/Containerfile.template`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/develop/templates/app/README.md.template` & `clams_python-1.2.2/clams/develop/templates/app/README.md.template`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/develop/templates/app/app.py.template` & `clams_python-1.2.2/clams/develop/templates/app/app.py.template`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/develop/templates/app/metadata.py.template` & `clams_python-1.2.2/clams/develop/templates/app/metadata.py.template`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/develop/templates/gha/for-clams-team.md.template` & `clams_python-1.2.2/clams/develop/templates/gha/for-clams-team.md.template`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/develop/templates/gha/workflows/publish.yml.template` & `clams_python-1.2.2/clams/develop/templates/gha/workflows/publish.yml.template`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/mmif_utils/rewind.py` & `clams_python-1.2.2/clams/mmif_utils/rewind.py`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/mmif_utils/source.py` & `clams_python-1.2.2/clams/mmif_utils/source.py`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/clams/restify/__init__.py` & `clams_python-1.2.2/clams/restify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,17 @@
 
     def get(self) -> Response:
         """
         Maps HTTP GET verb to :meth:`~clams.app.ClamsApp.appmetadata`.
 
         :return: Returns app metadata in a HTTP response.
         """
-        return self.json_to_response(self.cla.appmetadata(**request.args))
+        # this will catch duplicate arguments with different values into a list under the key
+        raw_params = request.args.to_dict(flat=False)
+        return self.json_to_response(self.cla.appmetadata(**raw_params))
 
     def post(self) -> Response:
         """
         Maps HTTP POST verb to :meth:`~clams.app.ClamsApp.annotate`.
         Note that for now HTTP PUT verbs is also mapped to :meth:`~clams.app.ClamsApp.annotate`.
 
         :return: Returns MMIF output from a ClamsApp in a HTTP response.
```

### Comparing `clams_python-1.2.1/clams_python.egg-info/PKG-INFO` & `clams_python-1.2.2/clams_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.2.1
+Version: 1.2.2
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers 
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mmif-python==1.0.13
+Requires-Dist: mmif-python==1.0.14
 Requires-Dist: Flask>=2
 Requires-Dist: Flask-RESTful>=0.3.9
 Requires-Dist: gunicorn>=20
 Requires-Dist: lapps>=0.0.2
 Requires-Dist: pydantic<2,>=1.8
 Requires-Dist: jsonschema>=3
```

### Comparing `clams_python-1.2.1/clams_python.egg-info/SOURCES.txt` & `clams_python-1.2.2/clams_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/setup.py` & `clams_python-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `clams_python-1.2.1/tests/test_clamsapp.py` & `clams_python-1.2.2/tests/test_clamsapp.py`

 * *Files 3% similar despite different names*

```diff
@@ -232,25 +232,39 @@
     def test_sign_view(self):
         m = Mmif(self.in_mmif)
         v1 = m.new_view()
         self.app.sign_view(v1, {})
         self.assertEqual(v1.metadata.app, self.app.metadata.identifier)
         self.assertEqual(len(v1.metadata.parameters), 0)
         v2 = m.new_view()
-        raw_query_string_arguments = {'undefined_param1': ['value1']}  # values are lists as our restifier uses `to_dict(flat=False)`
-        self.app.sign_view(v2, self.app._refine_params(**raw_query_string_arguments))
+        args2 = {'undefined_param1': ['value1']}  # values are lists as our restifier uses `to_dict(flat=False)`
+        self.app.sign_view(v2, self.app._refine_params(**args2))
         self.assertEqual(v2.metadata.app, self.app.metadata.identifier)
         self.assertEqual(len(v2.metadata.parameters), 1)
         self.assertFalse(clams.ClamsApp._RAW_PARAMS_KEY in v2.metadata.appConfiguration)
         for param in self.app.metadata.parameters:
             # any parameter with defaults should be recorded
             if param.default is not None:
                 self.assertTrue(param.name in v2.metadata.appConfiguration)
-            elif param.name not in raw_query_string_arguments:
+            elif param.name not in args2:
                 self.assertFalse(param.name in v2.metadata.appConfiguration)
+        v3 = m.new_view()
+        self.app.metadata.add_parameter('multivalued_param', 'dummy parameter with multivalues', type='string', multivalued=True, default=[])
+        args3 = {'undefined_param1': ['value1']} 
+        self.app.sign_view(v3, self.app._refine_params(**args3))
+        self.assertEqual(len(v3.metadata.parameters), 1)
+        self.assertEqual(len(v3.metadata.appConfiguration), 3)  # universal (pretty) + `raise_error` in metadata.py + `multivalued_param`
+        self.assertEqual(v3.metadata.appConfiguration['multivalued_param'], [])
+        v4 = m.new_view()
+        multiple_values = ['value1', 'value2']
+        args4 = {'multivalued_param': multiple_values}
+        self.app.sign_view(v4, self.app._refine_params(**args4))
+        self.assertEqual(len(v4.metadata.parameters), 1)
+        self.assertEqual(len(v4.metadata.appConfiguration), 3)
+        self.assertEqual(len(v4.metadata.parameters['multivalued_param']), len(str(multiple_values)))
 
     def test_annotate(self):
         # The example app is hard-coded to **always** emit version mismatch warning
         out_mmif = self.app.annotate(self.in_mmif)
         # TODO (krim @ 9/3/19): more robust test cases
         self.assertIsNotNone(out_mmif)
         out_mmif = Mmif(out_mmif)
@@ -303,14 +317,18 @@
                                         description='int +def +choices')
         self.app.metadata.add_parameter('param5', type='number', default=0.5,
                                         description='float +def')
         self.app.metadata.add_parameter('param6', type='number', multivalued=True, default=[0.5],
                                         description='float +def +mv')
         self.app.metadata.add_parameter('param7', type='number', default=[], multivalued=True,
                                         description='float +def +empty +mv')
+        # need to manually rebuild caster object, because the metadata has updated after the app is initialized
+        for param_spec in self.app.metadata.parameters:
+            self.app.annotate_param_spec[param_spec.name] = (param_spec.type, param_spec.multivalued)
+        self.app.annotate_param_caster = ParameterCaster(self.app.annotate_param_spec)
         with self.assertRaises(ValueError):
             self.app._refine_params(**{})  # param1 is required, but not passed
         dummy_params = {'param1': ['okay'], 'non_parameter': ['should be ignored']}
         conf = self.app._refine_params(**dummy_params)
         # should not refine what's already refined
         double_refine = self.app._refine_params(**conf)
         self.assertTrue(clams.ClamsApp._RAW_PARAMS_KEY in double_refine)
@@ -371,15 +389,15 @@
         put = self.app.put('/', data=ExampleInputMMIF.get_mmif())
         print(put.get_data(as_text=True))
         self.assertIsNotNone(put)
 
     def test_can_put_as_json(self):
         put = self.app.put('/', data=ExampleInputMMIF.get_mmif(), headers={"Content-Type": "Application/json"})
         self.assertIsNotNone(put)
-        self.assertEqual(put.status_code, 200)
+        self.assertEqual(200, put.status_code)
         self.assertIsNotNone(Mmif(put.get_data(as_text=True)))
 
     def test_can_pass_params(self):
         mmif = ExampleInputMMIF.get_mmif()
         headers = {"Content-Type": "Application/json"}
         query_string = {'pretty': True}
         pretty_res = self.app.put('/', data=mmif, headers=headers, query_string=query_string)
```

### Comparing `clams_python-1.2.1/tests/test_clamscli.py` & `clams_python-1.2.2/tests/test_clamscli.py`

 * *Files identical despite different names*

