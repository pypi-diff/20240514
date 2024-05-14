# Comparing `tmp/ooui-0.6.2.tar.gz` & `tmp/ooui-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooui-0.6.2.tar", last modified: Mon May 13 15:38:30 2024, max compression
+gzip compressed data, was "ooui-0.6.3.tar", last modified: Mon May 13 15:49:32 2024, max compression
```

## Comparing `ooui-0.6.2.tar` & `ooui-0.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:38:30.162073 ooui-0.6.2/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1065 2024-05-06 16:18:58.000000 ooui-0.6.2/LICENSE
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-13 15:38:30.162073 ooui-0.6.2/PKG-INFO
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       40 2024-05-06 16:18:58.000000 ooui-0.6.2/README.md
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:38:30.158073 ooui-0.6.2/ooui/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-06 16:22:58.000000 ooui-0.6.2/ooui/__init__.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:38:30.162073 ooui-0.6.2/ooui/graph/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      779 2024-05-10 12:16:14.000000 ooui-0.6.2/ooui/graph/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2599 2024-05-08 10:59:34.000000 ooui-0.6.2/ooui/graph/axis.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      783 2024-05-10 12:49:23.000000 ooui-0.6.2/ooui/graph/base.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     5632 2024-05-10 12:48:45.000000 ooui-0.6.2/ooui/graph/chart.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     3305 2024-05-10 12:09:54.000000 ooui-0.6.2/ooui/graph/fields.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2696 2024-05-13 15:27:59.000000 ooui-0.6.2/ooui/graph/indicator.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2996 2024-05-13 15:00:24.000000 ooui-0.6.2/ooui/graph/processor.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     9439 2024-05-08 12:28:50.000000 ooui-0.6.2/ooui/graph/timerange.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:38:30.162073 ooui-0.6.2/ooui/helpers/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      526 2024-05-06 17:19:46.000000 ooui-0.6.2/ooui/helpers/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1407 2024-05-13 14:13:20.000000 ooui-0.6.2/ooui/helpers/conditions.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1088 2024-05-13 15:37:47.000000 ooui-0.6.2/ooui/helpers/domain.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:38:30.162073 ooui-0.6.2/ooui.egg-info/
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-13 15:38:30.000000 ooui-0.6.2/ooui.egg-info/PKG-INFO
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      431 2024-05-13 15:38:30.000000 ooui-0.6.2/ooui.egg-info/SOURCES.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2024-05-13 15:38:30.000000 ooui-0.6.2/ooui.egg-info/dependency_links.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       43 2024-05-13 15:38:30.000000 ooui-0.6.2/ooui.egg-info/requires.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        5 2024-05-13 15:38:30.000000 ooui-0.6.2/ooui.egg-info/top_level.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2024-05-13 15:38:30.162073 ooui-0.6.2/setup.cfg
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      562 2024-05-13 15:38:02.000000 ooui-0.6.2/setup.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:49:32.247209 ooui-0.6.3/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1065 2024-05-06 16:18:58.000000 ooui-0.6.3/LICENSE
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-13 15:49:32.247209 ooui-0.6.3/PKG-INFO
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       40 2024-05-06 16:18:58.000000 ooui-0.6.3/README.md
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:49:32.247209 ooui-0.6.3/ooui/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-06 16:22:58.000000 ooui-0.6.3/ooui/__init__.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:49:32.247209 ooui-0.6.3/ooui/graph/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      779 2024-05-10 12:16:14.000000 ooui-0.6.3/ooui/graph/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2599 2024-05-08 10:59:34.000000 ooui-0.6.3/ooui/graph/axis.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      783 2024-05-10 12:49:23.000000 ooui-0.6.3/ooui/graph/base.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     5632 2024-05-10 12:48:45.000000 ooui-0.6.3/ooui/graph/chart.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     3305 2024-05-10 12:09:54.000000 ooui-0.6.3/ooui/graph/fields.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2839 2024-05-13 15:48:33.000000 ooui-0.6.3/ooui/graph/indicator.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2996 2024-05-13 15:00:24.000000 ooui-0.6.3/ooui/graph/processor.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     9439 2024-05-08 12:28:50.000000 ooui-0.6.3/ooui/graph/timerange.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:49:32.247209 ooui-0.6.3/ooui/helpers/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      526 2024-05-06 17:19:46.000000 ooui-0.6.3/ooui/helpers/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1407 2024-05-13 14:13:20.000000 ooui-0.6.3/ooui/helpers/conditions.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1088 2024-05-13 15:37:47.000000 ooui-0.6.3/ooui/helpers/domain.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:49:32.247209 ooui-0.6.3/ooui.egg-info/
+-rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-13 15:49:32.000000 ooui-0.6.3/ooui.egg-info/PKG-INFO
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      431 2024-05-13 15:49:32.000000 ooui-0.6.3/ooui.egg-info/SOURCES.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2024-05-13 15:49:32.000000 ooui-0.6.3/ooui.egg-info/dependency_links.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       43 2024-05-13 15:49:32.000000 ooui-0.6.3/ooui.egg-info/requires.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        5 2024-05-13 15:49:32.000000 ooui-0.6.3/ooui.egg-info/top_level.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2024-05-13 15:49:32.247209 ooui-0.6.3/setup.cfg
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      562 2024-05-13 15:48:57.000000 ooui-0.6.3/setup.py
```

### Comparing `ooui-0.6.2/LICENSE` & `ooui-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ooui-0.6.2/ooui/graph/__init__.py` & `ooui-0.6.3/ooui/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.2/ooui/graph/axis.py` & `ooui-0.6.3/ooui/graph/axis.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.2/ooui/graph/base.py` & `ooui-0.6.3/ooui/graph/base.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.2/ooui/graph/chart.py` & `ooui-0.6.3/ooui/graph/chart.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.2/ooui/graph/fields.py` & `ooui-0.6.3/ooui/graph/fields.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.2/ooui/graph/indicator.py` & `ooui-0.6.3/ooui/graph/indicator.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,17 @@
         self._color = ConditionParser(replace_entities(element.get('color'))) if element.get(
             'color') else None
         self._icon = ConditionParser(replace_entities(element.get('icon'))) if element.get(
             'icon') else None
         self._suffix = element.get('suffix') if element.get('suffix') else None
         self._total_domain = Domain(replace_entities(
             element.get('totalDomain')) if element.get('totalDomain') else None)
+        self._total_domain = element.get('totalDomain') and Domain(
+            replace_entities(element.get('totalDomain'))
+        ) or None
         self._show_percent = parse_bool_attribute(
             element.get('showPercent')) if element.get('showPercent') else False
         self.domain_parse_values = {}
 
     @property
     def color(self):
         return self._color
```

### Comparing `ooui-0.6.2/ooui/graph/processor.py` & `ooui-0.6.3/ooui/graph/processor.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.2/ooui/graph/timerange.py` & `ooui-0.6.3/ooui/graph/timerange.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.2/ooui/helpers/__init__.py` & `ooui-0.6.3/ooui/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.2/ooui/helpers/conditions.py` & `ooui-0.6.3/ooui/helpers/conditions.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.2/ooui/helpers/domain.py` & `ooui-0.6.3/ooui/helpers/domain.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.2/setup.py` & `ooui-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name='ooui',
     description='Open Object User Interface',
     author='GISCE',
     author_email='devel@gisce.net',
     url='https://github.com/gisce/python-ooui',
-    version='0.6.2',
+    version='0.6.3',
     license='MIT',
     long_description='''Open Object User Interface for GISCE-ERP''',
     provides=['ooui'],
     install_requires=[
         'lxml',
         'python-dateutil',
         'six',
```

