# Comparing `tmp/ooui-0.7.0.tar.gz` & `tmp/ooui-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooui-0.7.0.tar", last modified: Tue May 14 09:14:19 2024, max compression
+gzip compressed data, was "ooui-0.7.1.tar", last modified: Tue May 14 09:43:04 2024, max compression
```

## Comparing `ooui-0.7.0.tar` & `ooui-0.7.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:19.312034 ooui-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 09:14:05.000000 ooui-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 09:14:05.000000 ooui-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 09:14:19.312034 ooui-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 09:14:05.000000 ooui-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:19.308034 ooui-0.7.0/ooui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:19.312034 ooui-0.7.0/ooui/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9439 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/graph/timerange.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:19.312034 ooui-0.7.0/ooui/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/helpers/conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-14 09:14:05.000000 ooui-0.7.0/ooui/helpers/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:14:19.312034 ooui-0.7.0/ooui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 09:14:19.000000 ooui-0.7.0/ooui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-14 09:14:19.000000 ooui-0.7.0/ooui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:14:19.000000 ooui-0.7.0/ooui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 09:14:19.000000 ooui-0.7.0/ooui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 09:14:19.000000 ooui-0.7.0/ooui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 09:14:05.000000 ooui-0.7.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 09:14:05.000000 ooui-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:14:19.312034 ooui-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-14 09:14:05.000000 ooui-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:43:04.043751 ooui-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 09:42:55.000000 ooui-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 09:42:55.000000 ooui-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 09:43:04.043751 ooui-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 09:42:55.000000 ooui-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:43:04.039751 ooui-0.7.1/ooui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 09:42:55.000000 ooui-0.7.1/ooui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:43:04.043751 ooui-0.7.1/ooui/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-14 09:42:55.000000 ooui-0.7.1/ooui/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-14 09:42:55.000000 ooui-0.7.1/ooui/graph/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-14 09:42:55.000000 ooui-0.7.1/ooui/graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-14 09:42:55.000000 ooui-0.7.1/ooui/graph/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-14 09:42:55.000000 ooui-0.7.1/ooui/graph/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-14 09:42:55.000000 ooui-0.7.1/ooui/graph/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-14 09:42:55.000000 ooui-0.7.1/ooui/graph/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9439 2024-05-14 09:42:55.000000 ooui-0.7.1/ooui/graph/timerange.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:43:04.043751 ooui-0.7.1/ooui/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-14 09:42:55.000000 ooui-0.7.1/ooui/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-14 09:42:55.000000 ooui-0.7.1/ooui/helpers/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-14 09:42:55.000000 ooui-0.7.1/ooui/helpers/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:43:04.043751 ooui-0.7.1/ooui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 09:43:04.000000 ooui-0.7.1/ooui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-14 09:43:04.000000 ooui-0.7.1/ooui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:43:04.000000 ooui-0.7.1/ooui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 09:43:04.000000 ooui-0.7.1/ooui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 09:43:04.000000 ooui-0.7.1/ooui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 09:42:55.000000 ooui-0.7.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 09:42:55.000000 ooui-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:43:04.043751 ooui-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-14 09:42:55.000000 ooui-0.7.1/setup.py
```

### Comparing `ooui-0.7.0/LICENSE` & `ooui-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ooui-0.7.0/ooui/graph/__init__.py` & `ooui-0.7.1/ooui/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.7.0/ooui/graph/axis.py` & `ooui-0.7.1/ooui/graph/axis.py`

 * *Files identical despite different names*

### Comparing `ooui-0.7.0/ooui/graph/base.py` & `ooui-0.7.1/ooui/graph/base.py`

 * *Files identical despite different names*

### Comparing `ooui-0.7.0/ooui/graph/chart.py` & `ooui-0.7.1/ooui/graph/chart.py`

 * *Files identical despite different names*

### Comparing `ooui-0.7.0/ooui/graph/fields.py` & `ooui-0.7.1/ooui/graph/fields.py`

 * *Files identical despite different names*

### Comparing `ooui-0.7.0/ooui/graph/indicator.py` & `ooui-0.7.1/ooui/graph/indicator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         return self._suffix
 
     def process(self, value, total=0):
         res = {
             'value': value,
             'total': total,
         }
+        if self.suffix:
+            res['suffix'] = self.suffix
         if self.show_percent:
             res['percent'] = round_number(value / total * 100)
         if self.color:
             res['color'] = self.color.eval(res)
         if self.icon:
             res['icon'] = self.icon.eval(res)
         return res
```

### Comparing `ooui-0.7.0/ooui/graph/processor.py` & `ooui-0.7.1/ooui/graph/processor.py`

 * *Files identical despite different names*

### Comparing `ooui-0.7.0/ooui/graph/timerange.py` & `ooui-0.7.1/ooui/graph/timerange.py`

 * *Files identical despite different names*

### Comparing `ooui-0.7.0/ooui/helpers/__init__.py` & `ooui-0.7.1/ooui/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.7.0/ooui/helpers/conditions.py` & `ooui-0.7.1/ooui/helpers/conditions.py`

 * *Files identical despite different names*

### Comparing `ooui-0.7.0/ooui/helpers/domain.py` & `ooui-0.7.1/ooui/helpers/domain.py`

 * *Files identical despite different names*

### Comparing `ooui-0.7.0/setup.py` & `ooui-0.7.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setup(
     name='ooui',
     description='Open Object User Interface',
     author='GISCE',
     author_email='devel@gisce.net',
     url='https://github.com/gisce/python-ooui',
-    version='0.7.0',
+    version='0.7.1',
     license='MIT',
     long_description='''Open Object User Interface for GISCE-ERP''',
     provides=['ooui'],
     install_requires=requirements,
     tests_require=requirements_dev,
     packages=find_packages()
 )
```

