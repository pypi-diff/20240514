# Comparing `tmp/gen_wrappers-0.3.3.tar.gz` & `tmp/gen_wrappers-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.3.3.tar", last modified: Tue May 14 12:45:46 2024, max compression
+gzip compressed data, was "gen_wrappers-0.3.4.tar", last modified: Tue May 14 13:55:14 2024, max compression
```

## Comparing `gen_wrappers-0.3.3.tar` & `gen_wrappers-0.3.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.680182 gen_wrappers-0.3.3/
--rw-rw-rw-   0        0        0      847 2024-05-14 12:45:46.679182 gen_wrappers-0.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.533172 gen_wrappers-0.3.3/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.3/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.561246 gen_wrappers-0.3.3/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.3/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     6625 2024-05-11 17:01:23.000000 gen_wrappers-0.3.3/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.3.3/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.3/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.593377 gen_wrappers-0.3.3/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.3/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.3.3/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.3/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.3/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.3/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.618538 gen_wrappers-0.3.3/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.3/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9561 2024-05-11 17:02:29.000000 gen_wrappers-0.3.3/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     9193 2024-05-11 14:41:07.000000 gen_wrappers-0.3.3/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.3/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.646154 gen_wrappers-0.3.3/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.3/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6345 2024-05-11 17:04:12.000000 gen_wrappers-0.3.3/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.3/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.3/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.656666 gen_wrappers-0.3.3/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.3/creator/util/__init__.py
--rw-rw-rw-   0        0        0     6060 2024-05-13 20:04:32.000000 gen_wrappers-0.3.3/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:45:46.677201 gen_wrappers-0.3.3/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-14 12:45:46.000000 gen_wrappers-0.3.3/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-14 12:45:46.000000 gen_wrappers-0.3.3/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 12:45:46.000000 gen_wrappers-0.3.3/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-14 12:45:46.000000 gen_wrappers-0.3.3/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 12:45:46.000000 gen_wrappers-0.3.3/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 12:45:46.680182 gen_wrappers-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-14 12:45:33.000000 gen_wrappers-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.537770 gen_wrappers-0.3.4/
+-rw-rw-rw-   0        0        0      847 2024-05-14 13:55:14.536771 gen_wrappers-0.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.496246 gen_wrappers-0.3.4/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.4/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.501279 gen_wrappers-0.3.4/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.4/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     6625 2024-05-11 17:01:23.000000 gen_wrappers-0.3.4/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.3.4/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.4/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.505252 gen_wrappers-0.3.4/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.4/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.3.4/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.4/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.4/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.4/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.509252 gen_wrappers-0.3.4/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.4/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9561 2024-05-11 17:02:29.000000 gen_wrappers-0.3.4/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     9193 2024-05-11 14:41:07.000000 gen_wrappers-0.3.4/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.4/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.513770 gen_wrappers-0.3.4/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.4/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6345 2024-05-11 17:04:12.000000 gen_wrappers-0.3.4/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.4/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.4/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.515772 gen_wrappers-0.3.4/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.4/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.3.4/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:55:14.534770 gen_wrappers-0.3.4/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-14 13:55:14.000000 gen_wrappers-0.3.4/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-14 13:55:14.000000 gen_wrappers-0.3.4/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 13:55:14.000000 gen_wrappers-0.3.4/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-14 13:55:14.000000 gen_wrappers-0.3.4/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 13:55:14.000000 gen_wrappers-0.3.4/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 13:55:14.537770 gen_wrappers-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-14 13:55:01.000000 gen_wrappers-0.3.4/setup.py
```

### Comparing `gen_wrappers-0.3.3/PKG-INFO` & `gen_wrappers-0.3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.3.3
+Version: 0.3.4
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.3/creator/auto/creator_auto.py` & `gen_wrappers-0.3.4/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.3/creator/auto/request_auto.py` & `gen_wrappers-0.3.4/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.3/creator/auto/response_auto.py` & `gen_wrappers-0.3.4/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.3/creator/base/base_app.py` & `gen_wrappers-0.3.4/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.3/creator/base/base_request.py` & `gen_wrappers-0.3.4/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.3/creator/base/base_response.py` & `gen_wrappers-0.3.4/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.3/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.3.4/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.3/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.3.4/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.3/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.3.4/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.3/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.3.4/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.3/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.3.4/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.3/creator/util/helper.py` & `gen_wrappers-0.3.4/creator/util/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -102,34 +102,18 @@
             openapi_examples[method] = {
                 "summary": f"{method}",
                 "value": method
             }
     return examples if not openapi_output else openapi_examples
 
 
-def get_use_case(app_name: str, method: str, debug=False) -> Union[None, Type[BaseRequest]]:
-    package = sys.modules['creator']  # Make sure 'src.sb_api.creator' is the correct package path
-
-    for importer, modname, ispkg in pkgutil.walk_packages(package.__path__, package.__name__ + '.'):
-        # Filter out unwanted modules
-        if "creator_" not in modname or "base" in modname:
-            continue
-
-        # Try to import the module
-        try:
-            module = importlib.import_module(modname)
-            # Find all subclasses of BaseApp in the imported module
-            for name, obj in vars(module).items():
-                if isinstance(obj, type) and issubclass(obj, BaseApp) and obj is not BaseApp:
-                    base_app_name = obj.__name__.replace("App", "")
-                    base_app_name = ''.join(['_' + i.lower() if i.isupper() else i for i in base_app_name]).lstrip('_')
-                    if base_app_name != app_name:
-                        continue
-                    params = getattr(obj, "param_classes", [])
-                    for param in params:
-                        # Compare the method name to the base name of the param class
-                        param_base_name = param.__name__.split("_")[-1]
-                        if param_base_name == method:
-                            return param
-        except Exception as e:
-            print(f"Error importing {modname}: {e}")
+def get_use_case(app_name: str, method: str) -> Union[None, Type[BaseRequest]]:
+    use_cases = get_use_cases(True, False)
+    method = method.replace("_async", "")
+    # Convert app_name to CamelCase
+    app_name = ''.join([i.capitalize() for i in app_name.split('_')])
+    app_name = f"App{app_name}"
+    use_case_list = use_cases.get(app_name, [])
+    for use_case in use_case_list:
+        if use_case.__name__.split("_")[-1] == method:
+            return use_case
     return None
```

### Comparing `gen_wrappers-0.3.3/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.3.4/gen_wrappers.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.3.3
+Version: 0.3.4
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.3/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.3.4/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.3/setup.py` & `gen_wrappers-0.3.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.3.3',
+    version='0.3.4',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

