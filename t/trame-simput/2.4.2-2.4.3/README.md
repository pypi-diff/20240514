# Comparing `tmp/trame-simput-2.4.2.tar.gz` & `tmp/trame-simput-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-simput-2.4.2.tar", last modified: Mon May  6 14:27:00 2024, max compression
+gzip compressed data, was "trame-simput-2.4.3.tar", last modified: Tue May 14 15:54:58 2024, max compression
```

## Comparing `trame-simput-2.4.2.tar` & `trame-simput-2.4.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.057639 trame-simput-2.4.2/
--rw-r--r--   0 root         (0) root         (0)      583 2024-05-06 14:26:23.000000 trame-simput-2.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       32 2024-05-06 14:26:23.000000 trame-simput-2.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4666 2024-05-06 14:27:00.057639 trame-simput-2.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3894 2024-05-06 14:26:23.000000 trame-simput-2.4.2/README.rst
--rw-r--r--   0 root         (0) root         (0)      923 2024-05-06 14:27:00.057639 trame-simput-2.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 14:26:23.000000 trame-simput-2.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.045639 trame-simput-2.4.2/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       34 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame/modules/simput.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame/widgets/simput.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame_simput/
--rw-r--r--   0 root         (0) root         (0)      192 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame_simput/core/
--rw-r--r--   0 root         (0) root         (0)       81 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9142 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/domains.py
--rw-r--r--   0 root         (0) root         (0)      648 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/factory.py
--rw-r--r--   0 root         (0) root         (0)     1985 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/mapping.py
--rw-r--r--   0 root         (0) root         (0)    29212 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame_simput/core/ui/
--rw-r--r--   0 root         (0) root         (0)      133 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4685 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/ui/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame_simput/core/ui/resolvers/
--rw-r--r--   0 root         (0) root         (0)       75 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/ui/resolvers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4997 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/ui/resolvers/vuetify.py
--rw-r--r--   0 root         (0) root         (0)     1810 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/ui/utils.py
--rw-r--r--   0 root         (0) root         (0)      672 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.053639 trame-simput-2.4.2/trame_simput/module/
--rw-r--r--   0 root         (0) root         (0)      979 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8342 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/module/core.py
--rw-r--r--   0 root         (0) root         (0)     3257 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/module/protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.057639 trame-simput-2.4.2/trame_simput/module/serve/
--rw-r--r--   0 root         (0) root         (0)      208 2024-05-06 14:26:49.000000 trame-simput-2.4.2/trame_simput/module/serve/demo.html
--rw-r--r--   0 root         (0) root         (0)   326277 2024-05-06 14:26:49.000000 trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.common.js
--rw-r--r--   0 root         (0) root         (0)   450349 2024-05-06 14:26:49.000000 trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.common.js.map
--rw-r--r--   0 root         (0) root         (0)   326677 2024-05-06 14:26:49.000000 trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.js
--rw-r--r--   0 root         (0) root         (0)   450910 2024-05-06 14:26:49.000000 trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.js.map
--rw-r--r--   0 root         (0) root         (0)   113788 2024-05-06 14:26:50.000000 trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.min.js
--rw-r--r--   0 root         (0) root         (0)   482718 2024-05-06 14:26:50.000000 trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.min.js.map
--rw-r--r--   0 root         (0) root         (0)    79047 2024-05-06 14:26:56.000000 trame-simput-2.4.2/trame_simput/module/serve/vue3-trame_simput.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.057639 trame-simput-2.4.2/trame_simput/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4997 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/widgets/simput.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame_simput.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4666 2024-05-06 14:27:00.000000 trame-simput-2.4.2/trame_simput.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1291 2024-05-06 14:27:00.000000 trame-simput-2.4.2/trame_simput.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 14:27:00.000000 trame-simput-2.4.2/trame_simput.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-06 14:27:00.000000 trame-simput-2.4.2/trame_simput.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-06 14:27:00.000000 trame-simput-2.4.2/trame_simput.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:58.381497 trame-simput-2.4.3/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-14 15:54:22.000000 trame-simput-2.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-14 15:54:22.000000 trame-simput-2.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4666 2024-05-14 15:54:58.381497 trame-simput-2.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3894 2024-05-14 15:54:22.000000 trame-simput-2.4.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)      923 2024-05-14 15:54:58.385497 trame-simput-2.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 15:54:22.000000 trame-simput-2.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:58.373497 trame-simput-2.4.3/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:58.373497 trame-simput-2.4.3/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame/modules/simput.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:58.373497 trame-simput-2.4.3/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame/widgets/simput.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:58.373497 trame-simput-2.4.3/trame_simput/
+-rw-r--r--   0 root         (0) root         (0)      192 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:58.377497 trame-simput-2.4.3/trame_simput/core/
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9142 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/core/domains.py
+-rw-r--r--   0 root         (0) root         (0)      648 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/core/factory.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/core/mapping.py
+-rw-r--r--   0 root         (0) root         (0)    29238 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/core/proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:58.377497 trame-simput-2.4.3/trame_simput/core/ui/
+-rw-r--r--   0 root         (0) root         (0)      133 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/core/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4685 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/core/ui/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:58.377497 trame-simput-2.4.3/trame_simput/core/ui/resolvers/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/core/ui/resolvers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4997 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/core/ui/resolvers/vuetify.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/core/ui/utils.py
+-rw-r--r--   0 root         (0) root         (0)      672 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:58.377497 trame-simput-2.4.3/trame_simput/module/
+-rw-r--r--   0 root         (0) root         (0)      979 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8342 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/module/core.py
+-rw-r--r--   0 root         (0) root         (0)     3257 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/module/protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:58.381497 trame-simput-2.4.3/trame_simput/module/serve/
+-rw-r--r--   0 root         (0) root         (0)      208 2024-05-14 15:54:48.000000 trame-simput-2.4.3/trame_simput/module/serve/demo.html
+-rw-r--r--   0 root         (0) root         (0)   326277 2024-05-14 15:54:48.000000 trame-simput-2.4.3/trame_simput/module/serve/vue-trame_simput.common.js
+-rw-r--r--   0 root         (0) root         (0)   450349 2024-05-14 15:54:48.000000 trame-simput-2.4.3/trame_simput/module/serve/vue-trame_simput.common.js.map
+-rw-r--r--   0 root         (0) root         (0)   326677 2024-05-14 15:54:48.000000 trame-simput-2.4.3/trame_simput/module/serve/vue-trame_simput.umd.js
+-rw-r--r--   0 root         (0) root         (0)   450910 2024-05-14 15:54:48.000000 trame-simput-2.4.3/trame_simput/module/serve/vue-trame_simput.umd.js.map
+-rw-r--r--   0 root         (0) root         (0)   113788 2024-05-14 15:54:49.000000 trame-simput-2.4.3/trame_simput/module/serve/vue-trame_simput.umd.min.js
+-rw-r--r--   0 root         (0) root         (0)   482718 2024-05-14 15:54:49.000000 trame-simput-2.4.3/trame_simput/module/serve/vue-trame_simput.umd.min.js.map
+-rw-r--r--   0 root         (0) root         (0)    79047 2024-05-14 15:54:55.000000 trame-simput-2.4.3/trame_simput/module/serve/vue3-trame_simput.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:58.381497 trame-simput-2.4.3/trame_simput/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4997 2024-05-14 15:54:22.000000 trame-simput-2.4.3/trame_simput/widgets/simput.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:58.373497 trame-simput-2.4.3/trame_simput.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4666 2024-05-14 15:54:58.000000 trame-simput-2.4.3/trame_simput.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-05-14 15:54:58.000000 trame-simput-2.4.3/trame_simput.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 15:54:58.000000 trame-simput-2.4.3/trame_simput.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-14 15:54:58.000000 trame-simput-2.4.3/trame_simput.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-14 15:54:58.000000 trame-simput-2.4.3/trame_simput.egg-info/top_level.txt
```

### Comparing `trame-simput-2.4.2/LICENSE` & `trame-simput-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/PKG-INFO` & `trame-simput-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-simput
-Version: 2.4.2
+Version: 2.4.3
 Summary: Simput implementation for trame
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-simput-2.4.2/README.rst` & `trame-simput-2.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/setup.cfg` & `trame-simput-2.4.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-simput
-version = 2.4.2
+version = 2.4.3
 description = Simput implementation for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-simput-2.4.2/trame_simput/core/domains.py` & `trame-simput-2.4.3/trame_simput/core/domains.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/core/factory.py` & `trame-simput-2.4.3/trame_simput/core/factory.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/core/mapping.py` & `trame-simput-2.4.3/trame_simput/core/mapping.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/core/proxy.py` & `trame-simput-2.4.3/trame_simput/core/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -853,14 +853,16 @@
             file_content=file_content,
             data=data,
             new_ids=_new_ids,
             id_remap=_id_remap,
         )
         self._emit("created", ids=_new_ids)
 
+        return _id_remap
+
     # -------------------------------------------------------------------------
     # Commit / Reset
     # -------------------------------------------------------------------------
 
     def commit_all(self):
         """Commit all dirty proxies"""
         proxy_ids = list(self.dirty_proxy_data)
```

### Comparing `trame-simput-2.4.2/trame_simput/core/ui/manager.py` & `trame-simput-2.4.3/trame_simput/core/ui/manager.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/core/ui/resolvers/vuetify.py` & `trame-simput-2.4.3/trame_simput/core/ui/resolvers/vuetify.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/core/ui/utils.py` & `trame-simput-2.4.3/trame_simput/core/ui/utils.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/core/utils.py` & `trame-simput-2.4.3/trame_simput/core/utils.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/module/__init__.py` & `trame-simput-2.4.3/trame_simput/module/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/module/core.py` & `trame-simput-2.4.3/trame_simput/module/core.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/module/protocol.py` & `trame-simput-2.4.3/trame_simput/module/protocol.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.common.js` & `trame-simput-2.4.3/trame_simput/module/serve/vue-trame_simput.common.js`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.common.js.map` & `trame-simput-2.4.3/trame_simput/module/serve/vue-trame_simput.common.js.map`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.js` & `trame-simput-2.4.3/trame_simput/module/serve/vue-trame_simput.umd.js`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.js.map` & `trame-simput-2.4.3/trame_simput/module/serve/vue-trame_simput.umd.js.map`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.min.js` & `trame-simput-2.4.3/trame_simput/module/serve/vue-trame_simput.umd.min.js`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.min.js.map` & `trame-simput-2.4.3/trame_simput/module/serve/vue-trame_simput.umd.min.js.map`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/module/serve/vue3-trame_simput.umd.js` & `trame-simput-2.4.3/trame_simput/module/serve/vue3-trame_simput.umd.js`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput/widgets/simput.py` & `trame-simput-2.4.3/trame_simput/widgets/simput.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.2/trame_simput.egg-info/PKG-INFO` & `trame-simput-2.4.3/trame_simput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-simput
-Version: 2.4.2
+Version: 2.4.3
 Summary: Simput implementation for trame
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-simput-2.4.2/trame_simput.egg-info/SOURCES.txt` & `trame-simput-2.4.3/trame_simput.egg-info/SOURCES.txt`

 * *Files identical despite different names*

