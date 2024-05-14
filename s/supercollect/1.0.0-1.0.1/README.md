# Comparing `tmp/supercollect-1.0.0.tar.gz` & `tmp/supercollect-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supercollect-1.0.0.tar", max compression
+gzip compressed data, was "supercollect-1.0.1.tar", max compression
```

## Comparing `supercollect-1.0.0.tar` & `supercollect-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-05-14 17:38:10.400993 supercollect-1.0.0/LICENSE
--rw-r--r--   0        0        0      945 2024-05-14 17:27:58.261104 supercollect-1.0.0/README.md
--rw-r--r--   0        0        0      328 2024-05-14 17:28:14.778275 supercollect-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 13:23:55.140265 supercollect-1.0.0/supercollect/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 13:23:55.140265 supercollect-1.0.0/supercollect/management/__init__.py
--rw-r--r--   0        0        0     2708 2024-05-14 13:23:55.140265 supercollect-1.0.0/supercollect/management/commands/__init__.py
--rw-r--r--   0        0        0     1959 2024-05-14 17:29:03.201495 supercollect-1.0.0/supercollect/management/commands/collectstatic.py
--rw-r--r--   0        0        0      312 2024-05-14 13:38:28.918738 supercollect-1.0.0/supercollect/utils.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 supercollect-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-14 17:38:10.400993 supercollect-1.0.1/LICENSE
+-rw-r--r--   0        0        0      945 2024-05-14 17:27:58.261104 supercollect-1.0.1/README.md
+-rw-r--r--   0        0        0      329 2024-05-14 17:58:36.011282 supercollect-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 13:23:55.140265 supercollect-1.0.1/supercollect/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:23:55.140265 supercollect-1.0.1/supercollect/management/__init__.py
+-rw-r--r--   0        0        0     2708 2024-05-14 13:23:55.140265 supercollect-1.0.1/supercollect/management/commands/__init__.py
+-rw-r--r--   0        0        0     1959 2024-05-14 17:29:03.201495 supercollect-1.0.1/supercollect/management/commands/collectstatic.py
+-rw-r--r--   0        0        0      312 2024-05-14 13:38:28.918738 supercollect-1.0.1/supercollect/utils.py
+-rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 supercollect-1.0.1/PKG-INFO
```

### Comparing `supercollect-1.0.0/LICENSE` & `supercollect-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `supercollect-1.0.0/README.md` & `supercollect-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `supercollect-1.0.0/supercollect/management/commands/__init__.py` & `supercollect-1.0.1/supercollect/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `supercollect-1.0.0/supercollect/management/commands/collectstatic.py` & `supercollect-1.0.1/supercollect/management/commands/collectstatic.py`

 * *Files identical despite different names*

### Comparing `supercollect-1.0.0/PKG-INFO` & `supercollect-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: supercollect
-Version: 1.0.0
+Version: 1.0.1
 Summary: Supercharge collectstatic for remote storages
 Author: mdd
 Author-email: martin.diehl@terreon.de
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (>=4.2)
 Description-Content-Type: text/markdown
 
 # Supercollect
```

