# Comparing `tmp/flux_local-5.3.0.tar.gz` & `tmp/flux_local-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux_local-5.3.0.tar", last modified: Sun May 12 22:34:29 2024, max compression
+gzip compressed data, was "flux_local-5.3.1.tar", last modified: Tue May 14 04:16:25 2024, max compression
```

## Comparing `flux_local-5.3.0.tar` & `flux_local-5.3.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:34:29.645139 flux_local-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 22:34:25.000000 flux_local-5.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-05-12 22:34:29.645139 flux_local-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-12 22:34:25.000000 flux_local-5.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:34:29.637139 flux_local-5.3.0/flux_local/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27695 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)    22706 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:34:29.641139 flux_local-5.3.0/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    16948 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:34:29.645139 flux_local-5.3.0/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-05-12 22:34:29.000000 flux_local-5.3.0/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-12 22:34:29.000000 flux_local-5.3.0/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 22:34:29.000000 flux_local-5.3.0/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-12 22:34:29.000000 flux_local-5.3.0/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-12 22:34:29.000000 flux_local-5.3.0/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 22:34:29.000000 flux_local-5.3.0/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-12 22:34:25.000000 flux_local-5.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-12 22:34:29.645139 flux_local-5.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-12 22:34:25.000000 flux_local-5.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:34:29.641139 flux_local-5.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16462 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:34:29.645139 flux_local-5.3.0/tests/tool/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_diff_hr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_diff_ks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_get_hr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_get_ks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:16:25.226155 flux_local-5.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 04:16:20.000000 flux_local-5.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-05-14 04:16:25.226155 flux_local-5.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-14 04:16:20.000000 flux_local-5.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:16:25.218155 flux_local-5.3.1/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27695 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22706 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:16:25.222155 flux_local-5.3.1/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/tool/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16948 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/tool/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-14 04:16:20.000000 flux_local-5.3.1/flux_local/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:16:25.226155 flux_local-5.3.1/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-05-14 04:16:25.000000 flux_local-5.3.1/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-14 04:16:25.000000 flux_local-5.3.1/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 04:16:25.000000 flux_local-5.3.1/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 04:16:25.000000 flux_local-5.3.1/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-14 04:16:25.000000 flux_local-5.3.1/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 04:16:25.000000 flux_local-5.3.1/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-14 04:16:20.000000 flux_local-5.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-14 04:16:25.226155 flux_local-5.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 04:16:20.000000 flux_local-5.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:16:25.222155 flux_local-5.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16462 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:16:25.226155 flux_local-5.3.1/tests/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/tool/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/tool/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/tool/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/tool/test_diff_hr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/tool/test_diff_ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/tool/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/tool/test_get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/tool/test_get_hr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/tool/test_get_ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-14 04:16:20.000000 flux_local-5.3.1/tests/tool/test_test.py
```

### Comparing `flux_local-5.3.0/LICENSE` & `flux_local-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/PKG-INFO` & `flux_local-5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 5.3.0
+Version: 5.3.1
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `flux_local-5.3.0/README.md` & `flux_local-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/command.py` & `flux_local-5.3.1/flux_local/command.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/context.py` & `flux_local-5.3.1/flux_local/context.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/exceptions.py` & `flux_local-5.3.1/flux_local/exceptions.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/git_repo.py` & `flux_local-5.3.1/flux_local/git_repo.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/helm.py` & `flux_local-5.3.1/flux_local/helm.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/image.py` & `flux_local-5.3.1/flux_local/image.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/kustomize.py` & `flux_local-5.3.1/flux_local/kustomize.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/manifest.py` & `flux_local-5.3.1/flux_local/manifest.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/tool/build.py` & `flux_local-5.3.1/flux_local/tool/build.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/tool/diagnostics.py` & `flux_local-5.3.1/flux_local/tool/diagnostics.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/tool/diff.py` & `flux_local-5.3.1/flux_local/tool/diff.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/tool/flux_local.py` & `flux_local-5.3.1/flux_local/tool/flux_local.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/tool/format.py` & `flux_local-5.3.1/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/tool/get.py` & `flux_local-5.3.1/flux_local/tool/get.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/tool/selector.py` & `flux_local-5.3.1/flux_local/tool/selector.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/tool/test.py` & `flux_local-5.3.1/flux_local/tool/test.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/tool/visitor.py` & `flux_local-5.3.1/flux_local/tool/visitor.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local/values.py` & `flux_local-5.3.1/flux_local/values.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/flux_local.egg-info/PKG-INFO` & `flux_local-5.3.1/flux_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 5.3.0
+Version: 5.3.1
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `flux_local-5.3.0/flux_local.egg-info/SOURCES.txt` & `flux_local-5.3.1/flux_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/pyproject.toml` & `flux_local-5.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/setup.cfg` & `flux_local-5.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 5.3.0
+version = 5.3.1
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
```

### Comparing `flux_local-5.3.0/tests/test_command.py` & `flux_local-5.3.1/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/test_git_repo.py` & `flux_local-5.3.1/tests/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/test_helm.py` & `flux_local-5.3.1/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/test_image.py` & `flux_local-5.3.1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/test_kustomize.py` & `flux_local-5.3.1/tests/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/test_manifest.py` & `flux_local-5.3.1/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/test_values.py` & `flux_local-5.3.1/tests/test_values.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/tool/test_build.py` & `flux_local-5.3.1/tests/tool/test_build.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/tool/test_diagnostics.py` & `flux_local-5.3.1/tests/tool/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/tool/test_diff.py` & `flux_local-5.3.1/tests/tool/test_diff.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/tool/test_diff_hr.py` & `flux_local-5.3.1/tests/tool/test_diff_hr.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/tool/test_diff_ks.py` & `flux_local-5.3.1/tests/tool/test_diff_ks.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/tool/test_format.py` & `flux_local-5.3.1/tests/tool/test_format.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/tool/test_get_cluster.py` & `flux_local-5.3.1/tests/tool/test_get_cluster.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/tool/test_get_hr.py` & `flux_local-5.3.1/tests/tool/test_get_hr.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/tool/test_get_ks.py` & `flux_local-5.3.1/tests/tool/test_get_ks.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.3.0/tests/tool/test_test.py` & `flux_local-5.3.1/tests/tool/test_test.py`

 * *Files identical despite different names*

