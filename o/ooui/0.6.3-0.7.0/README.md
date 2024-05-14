# Comparing `tmp/ooui-0.6.3.tar.gz` & `tmp/ooui-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooui-0.6.3.tar", last modified: Mon May 13 15:49:32 2024, max compression
+gzip compressed data, was "ooui-0.7.0.tar", last modified: Tue May 14 09:14:19 2024, max compression
```

## Comparing `ooui-0.6.3.tar` & `ooui-0.7.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:49:32.247209 ooui-0.6.3/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1065 2024-05-06 16:18:58.000000 ooui-0.6.3/LICENSE
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-13 15:49:32.247209 ooui-0.6.3/PKG-INFO
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       40 2024-05-06 16:18:58.000000 ooui-0.6.3/README.md
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:49:32.247209 ooui-0.6.3/ooui/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-06 16:22:58.000000 ooui-0.6.3/ooui/__init__.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:49:32.247209 ooui-0.6.3/ooui/graph/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      779 2024-05-10 12:16:14.000000 ooui-0.6.3/ooui/graph/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2599 2024-05-08 10:59:34.000000 ooui-0.6.3/ooui/graph/axis.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      783 2024-05-10 12:49:23.000000 ooui-0.6.3/ooui/graph/base.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     5632 2024-05-10 12:48:45.000000 ooui-0.6.3/ooui/graph/chart.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     3305 2024-05-10 12:09:54.000000 ooui-0.6.3/ooui/graph/fields.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2839 2024-05-13 15:48:33.000000 ooui-0.6.3/ooui/graph/indicator.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2996 2024-05-13 15:00:24.000000 ooui-0.6.3/ooui/graph/processor.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     9439 2024-05-08 12:28:50.000000 ooui-0.6.3/ooui/graph/timerange.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:49:32.247209 ooui-0.6.3/ooui/helpers/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      526 2024-05-06 17:19:46.000000 ooui-0.6.3/ooui/helpers/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1407 2024-05-13 14:13:20.000000 ooui-0.6.3/ooui/helpers/conditions.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1088 2024-05-13 15:37:47.000000 ooui-0.6.3/ooui/helpers/domain.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-13 15:49:32.247209 ooui-0.6.3/ooui.egg-info/
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-13 15:49:32.000000 ooui-0.6.3/ooui.egg-info/PKG-INFO
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      431 2024-05-13 15:49:32.000000 ooui-0.6.3/ooui.egg-info/SOURCES.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2024-05-13 15:49:32.000000 ooui-0.6.3/ooui.egg-info/dependency_links.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       43 2024-05-13 15:49:32.000000 ooui-0.6.3/ooui.egg-info/requires.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        5 2024-05-13 15:49:32.000000 ooui-0.6.3/ooui.egg-info/top_level.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2024-05-13 15:49:32.247209 ooui-0.6.3/setup.cfg
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      562 2024-05-13 15:48:57.000000 ooui-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:19.312034 ooui-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 09:14:05.000000 ooui-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 09:14:05.000000 ooui-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 09:14:19.312034 ooui-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 09:14:05.000000 ooui-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:19.308034 ooui-0.7.0/ooui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:19.312034 ooui-0.7.0/ooui/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9439 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/timerange.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:19.312034 ooui-0.7.0/ooui/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/helpers/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/helpers/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:19.312034 ooui-0.7.0/ooui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 09:14:19.000000 ooui-0.7.0/ooui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-14 09:14:19.000000 ooui-0.7.0/ooui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:14:19.000000 ooui-0.7.0/ooui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 09:14:19.000000 ooui-0.7.0/ooui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 09:14:19.000000 ooui-0.7.0/ooui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 09:14:05.000000 ooui-0.7.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 09:14:05.000000 ooui-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:14:19.312034 ooui-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-14 09:14:05.000000 ooui-0.7.0/setup.py
```

### Comparing `ooui-0.6.3/LICENSE` & `ooui-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ooui-0.6.3/ooui/graph/__init__.py` & `ooui-0.7.0/ooui/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.3/ooui/graph/axis.py` & `ooui-0.7.0/ooui/graph/axis.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.3/ooui/graph/base.py` & `ooui-0.7.0/ooui/graph/base.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.3/ooui/graph/chart.py` & `ooui-0.7.0/ooui/graph/chart.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.3/ooui/graph/fields.py` & `ooui-0.7.0/ooui/graph/fields.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.3/ooui/graph/indicator.py` & `ooui-0.7.0/ooui/graph/indicator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import division
 from ooui.graph.base import Graph
-from ooui.helpers import parse_bool_attribute, replace_entities
-from ooui.helpers.conditions import ConditionParser
-from ooui.helpers.domain import Domain
+from ooui.helpers import (
+    parse_bool_attribute, replace_entities, ConditionParser, Domain
+)
 from ooui.graph.fields import get_value_for_operator, round_number
 
 
 class GraphIndicator(Graph):
     def __init__(self, graph_type, element):
         # Inicia la classe base Graph
         super(GraphIndicator, self).__init__(element)
```

### Comparing `ooui-0.6.3/ooui/graph/processor.py` & `ooui-0.7.0/ooui/graph/processor.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.3/ooui/graph/timerange.py` & `ooui-0.7.0/ooui/graph/timerange.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.3/ooui/helpers/__init__.py` & `ooui-0.7.0/ooui/helpers/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from __future__ import absolute_import
 import six
+from .conditions import ConditionParser
+from .domain import Domain
 
 
 def parse_bool_attribute(attribute):
     """
     Parse a boolean attribute.
     :param attribute:
     :return: bool
```

### Comparing `ooui-0.6.3/ooui/helpers/conditions.py` & `ooui-0.7.0/ooui/helpers/conditions.py`

 * *Files identical despite different names*

### Comparing `ooui-0.6.3/ooui/helpers/domain.py` & `ooui-0.7.0/ooui/helpers/domain.py`

 * *Files identical despite different names*

