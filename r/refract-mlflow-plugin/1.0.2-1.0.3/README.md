# Comparing `tmp/refract-mlflow-plugin-1.0.2.tar.gz` & `tmp/refract-mlflow-plugin-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refract-mlflow-plugin-1.0.2.tar", last modified: Mon Oct  9 09:04:28 2023, max compression
+gzip compressed data, was "refract-mlflow-plugin-1.0.3.tar", last modified: Tue May 14 03:05:17 2024, max compression
```

## Comparing `refract-mlflow-plugin-1.0.2.tar` & `refract-mlflow-plugin-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vaibhawbade  (1002) vaibhawbade  (1002)        0 2023-10-09 09:04:28.606769 refract-mlflow-plugin-1.0.2/
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)       42 2023-10-05 10:13:34.000000 refract-mlflow-plugin-1.0.2/LICENSE
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)      316 2023-10-09 09:04:28.606769 refract-mlflow-plugin-1.0.2/PKG-INFO
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)      153 2023-10-05 05:10:35.000000 refract-mlflow-plugin-1.0.2/README.md
-drwxrwxr-x   0 vaibhawbade  (1002) vaibhawbade  (1002)        0 2023-10-09 09:04:28.606769 refract-mlflow-plugin-1.0.2/refract_mlflow_plugin/
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)        0 2023-10-03 10:21:55.000000 refract-mlflow-plugin-1.0.2/refract_mlflow_plugin/__init__.py
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)     2632 2023-10-09 05:53:41.000000 refract-mlflow-plugin-1.0.2/refract_mlflow_plugin/app.py
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)      552 2023-10-03 13:56:30.000000 refract-mlflow-plugin-1.0.2/refract_mlflow_plugin/request_header_provider.py
-drwxrwxr-x   0 vaibhawbade  (1002) vaibhawbade  (1002)        0 2023-10-09 09:04:28.606769 refract-mlflow-plugin-1.0.2/refract_mlflow_plugin.egg-info/
--rw-r--r--   0 vaibhawbade  (1002) vaibhawbade  (1002)      316 2023-10-09 09:04:28.000000 refract-mlflow-plugin-1.0.2/refract_mlflow_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)      410 2023-10-09 09:04:28.000000 refract-mlflow-plugin-1.0.2/refract_mlflow_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)        1 2023-10-09 09:04:28.000000 refract-mlflow-plugin-1.0.2/refract_mlflow_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)      181 2023-10-09 09:04:28.000000 refract-mlflow-plugin-1.0.2/refract_mlflow_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)       14 2023-10-09 09:04:28.000000 refract-mlflow-plugin-1.0.2/refract_mlflow_plugin.egg-info/requires.txt
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)       22 2023-10-09 09:04:28.000000 refract-mlflow-plugin-1.0.2/refract_mlflow_plugin.egg-info/top_level.txt
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)       38 2023-10-09 09:04:28.606769 refract-mlflow-plugin-1.0.2/setup.cfg
--rw-rw-r--   0 vaibhawbade  (1002) vaibhawbade  (1002)      908 2023-10-09 09:01:59.000000 refract-mlflow-plugin-1.0.2/setup.py
+drwxrwxr-x   0 aditya    (1003) aditya    (1003)        0 2024-05-14 03:05:17.617282 refract-mlflow-plugin-1.0.3/
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)       42 2024-05-07 05:14:57.000000 refract-mlflow-plugin-1.0.3/LICENSE
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)      372 2024-05-14 03:05:17.617282 refract-mlflow-plugin-1.0.3/PKG-INFO
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)      153 2024-05-07 05:14:57.000000 refract-mlflow-plugin-1.0.3/README.md
+drwxrwxr-x   0 aditya    (1003) aditya    (1003)        0 2024-05-14 03:05:17.617282 refract-mlflow-plugin-1.0.3/refract_mlflow_plugin/
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)        0 2024-05-07 05:14:57.000000 refract-mlflow-plugin-1.0.3/refract_mlflow_plugin/__init__.py
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)     2632 2024-05-07 05:14:57.000000 refract-mlflow-plugin-1.0.3/refract_mlflow_plugin/app.py
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)      552 2024-05-07 05:14:57.000000 refract-mlflow-plugin-1.0.3/refract_mlflow_plugin/request_header_provider.py
+drwxrwxr-x   0 aditya    (1003) aditya    (1003)        0 2024-05-14 03:05:17.617282 refract-mlflow-plugin-1.0.3/refract_mlflow_plugin.egg-info/
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)      372 2024-05-14 03:05:17.000000 refract-mlflow-plugin-1.0.3/refract_mlflow_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)      410 2024-05-14 03:05:17.000000 refract-mlflow-plugin-1.0.3/refract_mlflow_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)        1 2024-05-14 03:05:17.000000 refract-mlflow-plugin-1.0.3/refract_mlflow_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)      178 2024-05-14 03:05:17.000000 refract-mlflow-plugin-1.0.3/refract_mlflow_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)       15 2024-05-14 03:05:17.000000 refract-mlflow-plugin-1.0.3/refract_mlflow_plugin.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)       22 2024-05-14 03:05:17.000000 refract-mlflow-plugin-1.0.3/refract_mlflow_plugin.egg-info/top_level.txt
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)       38 2024-05-14 03:05:17.617282 refract-mlflow-plugin-1.0.3/setup.cfg
+-rw-rw-r--   0 aditya    (1003) aditya    (1003)      909 2024-05-14 02:59:01.000000 refract-mlflow-plugin-1.0.3/setup.py
```

### Comparing `refract-mlflow-plugin-1.0.2/refract_mlflow_plugin/app.py` & `refract-mlflow-plugin-1.0.3/refract_mlflow_plugin/app.py`

 * *Files identical despite different names*

### Comparing `refract-mlflow-plugin-1.0.2/refract_mlflow_plugin/request_header_provider.py` & `refract-mlflow-plugin-1.0.3/refract_mlflow_plugin/request_header_provider.py`

 * *Files identical despite different names*

### Comparing `refract-mlflow-plugin-1.0.2/setup.py` & `refract-mlflow-plugin-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="refract-mlflow-plugin",
-    version="1.0.2",
+    version="1.0.3",
     description="Refract plugin for MLflow",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=find_packages(),
     # Require MLflow as a dependency of the plugin, so that plugin users can simply install
     # the plugin & then immediately use it with MLflow
-    install_requires=["mlflow==2.6.0"],
+    install_requires=["mlflow==2.10.0"],
     entry_points={
         "mlflow.request_header_provider": "unused=refract_mlflow_plugin.request_header_provider:RefractRequestHeaderProvider",  # pylint: disable=line-too-long
         # Define a custom Mlflow application with name custom_app
         "mlflow.app": "custom_app=refract_mlflow_plugin.app:custom_app"
     },
 )
```

