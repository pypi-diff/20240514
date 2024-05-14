# Comparing `tmp/openai_priority_loadbalancer-0.0.3.tar.gz` & `tmp/openai_priority_loadbalancer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_priority_loadbalancer-0.0.3.tar", last modified: Tue May 14 03:46:31 2024, max compression
+gzip compressed data, was "openai_priority_loadbalancer-0.0.4.tar", last modified: Tue May 14 03:56:50 2024, max compression
```

## Comparing `openai_priority_loadbalancer-0.0.3.tar` & `openai_priority_loadbalancer-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 03:46:31.649922 openai_priority_loadbalancer-0.0.3/
--rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    11484 2024-05-14 03:45:16.000000 openai_priority_loadbalancer-0.0.3/PACKAGE_README.md
--rw-rw-rw-   0        0        0    12284 2024-05-14 03:46:31.641764 openai_priority_loadbalancer-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    12280 2024-05-14 03:01:51.000000 openai_priority_loadbalancer-0.0.3/README.md
--rw-rw-rw-   0        0        0      670 2024-05-14 03:45:23.000000 openai_priority_loadbalancer-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 03:46:31.651153 openai_priority_loadbalancer-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 03:46:31.565961 openai_priority_loadbalancer-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 03:46:31.588199 openai_priority_loadbalancer-0.0.3/src/openai_loadbalancer_simon_kurtz/
--rw-rw-rw-   0        0        0       36 2024-05-14 02:47:44.000000 openai_priority_loadbalancer-0.0.3/src/openai_loadbalancer_simon_kurtz/__init__.py
--rw-rw-rw-   0        0        0    10300 2024-05-13 20:56:00.000000 openai_priority_loadbalancer-0.0.3/src/openai_loadbalancer_simon_kurtz/openai_load_balancer.py
-drwxrwxrwx   0        0        0        0 2024-05-14 03:46:31.638424 openai_priority_loadbalancer-0.0.3/src/openai_priority_loadbalancer.egg-info/
--rw-rw-rw-   0        0        0    12284 2024-05-14 03:46:31.000000 openai_priority_loadbalancer-0.0.3/src/openai_priority_loadbalancer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2024-05-14 03:46:31.000000 openai_priority_loadbalancer-0.0.3/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 03:46:31.000000 openai_priority_loadbalancer-0.0.3/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-14 03:46:31.000000 openai_priority_loadbalancer-0.0.3/src/openai_priority_loadbalancer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 03:56:50.550350 openai_priority_loadbalancer-0.0.4/
+-rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    11484 2024-05-14 03:45:16.000000 openai_priority_loadbalancer-0.0.4/PACKAGE_README.md
+-rw-rw-rw-   0        0        0    12284 2024-05-14 03:56:50.520193 openai_priority_loadbalancer-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12280 2024-05-14 03:01:51.000000 openai_priority_loadbalancer-0.0.4/README.md
+-rw-rw-rw-   0        0        0      670 2024-05-14 03:56:29.000000 openai_priority_loadbalancer-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 03:56:50.551353 openai_priority_loadbalancer-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 03:56:49.947544 openai_priority_loadbalancer-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 03:56:50.038370 openai_priority_loadbalancer-0.0.4/src/openai_priority_loadbalancer/
+-rw-rw-rw-   0        0        0       35 2024-05-14 03:55:49.000000 openai_priority_loadbalancer-0.0.4/src/openai_priority_loadbalancer/__init__.py
+-rw-rw-rw-   0        0        0    10300 2024-05-13 20:56:00.000000 openai_priority_loadbalancer-0.0.4/src/openai_priority_loadbalancer/openai_loadbalancer.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:56:50.478228 openai_priority_loadbalancer-0.0.4/src/openai_priority_loadbalancer.egg-info/
+-rw-rw-rw-   0        0        0    12284 2024-05-14 03:56:49.000000 openai_priority_loadbalancer-0.0.4/src/openai_priority_loadbalancer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2024-05-14 03:56:49.000000 openai_priority_loadbalancer-0.0.4/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 03:56:49.000000 openai_priority_loadbalancer-0.0.4/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-14 03:56:49.000000 openai_priority_loadbalancer-0.0.4/src/openai_priority_loadbalancer.egg-info/top_level.txt
```

### Comparing `openai_priority_loadbalancer-0.0.3/LICENSE` & `openai_priority_loadbalancer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-0.0.3/PACKAGE_README.md` & `openai_priority_loadbalancer-0.0.4/PACKAGE_README.md`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-0.0.3/PKG-INFO` & `openai_priority_loadbalancer-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 0.0.3
+Version: 0.0.4
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_priority_loadbalancer-0.0.3/README.md` & `openai_priority_loadbalancer-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-0.0.3/pyproject.toml` & `openai_priority_loadbalancer-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openai_priority_loadbalancer"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Simon Kurtz", email="simonkurtz@gmail.com" },
 ]
 description = "A multi-backend, prioritization load balancer for OpenAI"
 readme = "PACKAGE_README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `openai_priority_loadbalancer-0.0.3/src/openai_loadbalancer_simon_kurtz/openai_load_balancer.py` & `openai_priority_loadbalancer-0.0.4/src/openai_priority_loadbalancer/openai_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-0.0.3/src/openai_priority_loadbalancer.egg-info/PKG-INFO` & `openai_priority_loadbalancer-0.0.4/src/openai_priority_loadbalancer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 0.0.3
+Version: 0.0.4
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

