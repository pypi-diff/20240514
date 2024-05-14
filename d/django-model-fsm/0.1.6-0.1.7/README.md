# Comparing `tmp/django_model_fsm-0.1.6.tar.gz` & `tmp/django_model_fsm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_model_fsm-0.1.6.tar", max compression
+gzip compressed data, was "django_model_fsm-0.1.7.tar", max compression
```

## Comparing `django_model_fsm-0.1.6.tar` & `django_model_fsm-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       70 2024-01-22 17:09:29.487617 django_model_fsm-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-01-22 17:14:09.720271 django_model_fsm-0.1.6/django_model_fsm/__init__.py
--rw-r--r--   0        0        0      183 2024-01-22 17:14:53.736374 django_model_fsm-0.1.6/django_model_fsm/dataclasses/__init__.py
--rw-r--r--   0        0        0      152 2024-02-13 09:58:29.553331 django_model_fsm-0.1.6/django_model_fsm/dataclasses/state_data.py
--rw-r--r--   0        0        0      209 2024-01-22 17:56:38.877399 django_model_fsm-0.1.6/django_model_fsm/dataclasses/trigger_data.py
--rw-r--r--   0        0        0     2251 2024-01-22 17:14:53.736374 django_model_fsm-0.1.6/django_model_fsm/dataclasses/workflow_data.py
--rw-r--r--   0        0        0       84 2024-01-22 17:26:11.273959 django_model_fsm-0.1.6/django_model_fsm/fields/__init__.py
--rw-r--r--   0        0        0      343 2024-01-22 17:27:36.906160 django_model_fsm-0.1.6/django_model_fsm/fields/transition_field.py
--rw-r--r--   0        0        0        0 2024-01-22 17:15:06.000403 django_model_fsm-0.1.6/django_model_fsm/forms/__init__.py
--rw-r--r--   0        0        0       75 2024-02-13 09:57:04.577055 django_model_fsm-0.1.6/django_model_fsm/helpers/__init__.py
--rw-r--r--   0        0        0     3071 2024-02-13 09:56:24.288924 django_model_fsm-0.1.6/django_model_fsm/helpers/draw_workflow.py
--rw-r--r--   0        0        0       87 2024-01-22 17:15:11.508415 django_model_fsm-0.1.6/django_model_fsm/models/__init__.py
--rw-r--r--   0        0        0     4058 2024-02-16 09:42:51.889098 django_model_fsm-0.1.6/django_model_fsm/models/transitions_mixin.py
--rw-r--r--   0        0        0     2207 2024-02-16 09:43:00.129060 django_model_fsm-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 django_model_fsm-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       70 2024-01-22 17:09:29.487617 django_model_fsm-0.1.7/README.md
+-rw-r--r--   0        0        0      215 2024-05-14 19:48:19.786169 django_model_fsm-0.1.7/django_model_fsm/__init__.py
+-rw-r--r--   0        0        0      183 2024-01-22 17:14:53.736374 django_model_fsm-0.1.7/django_model_fsm/dataclasses/__init__.py
+-rw-r--r--   0        0        0      152 2024-02-13 09:58:29.553331 django_model_fsm-0.1.7/django_model_fsm/dataclasses/state_data.py
+-rw-r--r--   0        0        0      209 2024-01-22 17:56:38.877399 django_model_fsm-0.1.7/django_model_fsm/dataclasses/trigger_data.py
+-rw-r--r--   0        0        0     2251 2024-01-22 17:14:53.736374 django_model_fsm-0.1.7/django_model_fsm/dataclasses/workflow_data.py
+-rw-r--r--   0        0        0       84 2024-01-22 17:26:11.273959 django_model_fsm-0.1.7/django_model_fsm/fields/__init__.py
+-rw-r--r--   0        0        0      343 2024-01-22 17:27:36.906160 django_model_fsm-0.1.7/django_model_fsm/fields/transition_field.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:15:06.000403 django_model_fsm-0.1.7/django_model_fsm/forms/__init__.py
+-rw-r--r--   0        0        0       75 2024-02-13 09:57:04.577055 django_model_fsm-0.1.7/django_model_fsm/helpers/__init__.py
+-rw-r--r--   0        0        0     3071 2024-02-13 09:56:24.288924 django_model_fsm-0.1.7/django_model_fsm/helpers/draw_workflow.py
+-rw-r--r--   0        0        0       87 2024-01-22 17:15:11.508415 django_model_fsm-0.1.7/django_model_fsm/models/__init__.py
+-rw-r--r--   0        0        0     4058 2024-02-16 09:42:51.889098 django_model_fsm-0.1.7/django_model_fsm/models/transitions_mixin.py
+-rw-r--r--   0        0        0     2207 2024-05-14 19:50:53.266751 django_model_fsm-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 django_model_fsm-0.1.7/PKG-INFO
```

### Comparing `django_model_fsm-0.1.6/django_model_fsm/dataclasses/workflow_data.py` & `django_model_fsm-0.1.7/django_model_fsm/dataclasses/workflow_data.py`

 * *Files identical despite different names*

### Comparing `django_model_fsm-0.1.6/django_model_fsm/helpers/draw_workflow.py` & `django_model_fsm-0.1.7/django_model_fsm/helpers/draw_workflow.py`

 * *Files identical despite different names*

### Comparing `django_model_fsm-0.1.6/django_model_fsm/models/transitions_mixin.py` & `django_model_fsm-0.1.7/django_model_fsm/models/transitions_mixin.py`

 * *Files identical despite different names*

### Comparing `django_model_fsm-0.1.6/pyproject.toml` & `django_model_fsm-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-model-fsm"
-version = "0.1.6"
+version = "0.1.7"
 description = "A package to use transitions with a Django model."
 authors = ["Alexandre Norman <norman@xael.org>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "django_model_fsm"}]    
 repository = "https://bitbucket.org/hespul/django-model-fsm/"
```

### Comparing `django_model_fsm-0.1.6/PKG-INFO` & `django_model_fsm-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-fsm
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package to use transitions with a Django model.
 Home-page: https://bitbucket.org/hespul/django-model-fsm/
 License: GPLv3
 Author: Alexandre Norman
 Author-email: norman@xael.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

