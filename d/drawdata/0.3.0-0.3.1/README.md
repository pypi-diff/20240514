# Comparing `tmp/drawdata-0.3.0.tar.gz` & `tmp/drawdata-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drawdata-0.3.0.tar", last modified: Sat Feb 24 12:37:26 2024, max compression
+gzip compressed data, was "drawdata-0.3.1.tar", last modified: Tue May 14 13:12:54 2024, max compression
```

## Comparing `drawdata-0.3.0.tar` & `drawdata-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-02-24 12:37:26.424522 drawdata-0.3.0/
--rw-r--r--   0 vincent    (501) staff       (20)     1077 2024-02-14 10:06:31.000000 drawdata-0.3.0/LICENSE
--rw-r--r--   0 vincent    (501) staff       (20)     3000 2024-02-24 12:37:26.424412 drawdata-0.3.0/PKG-INFO
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-02-24 12:37:26.423034 drawdata-0.3.0/drawdata/
--rw-r--r--   0 vincent    (501) staff       (20)     1237 2024-02-24 12:36:19.000000 drawdata-0.3.0/drawdata/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-02-24 12:37:26.423756 drawdata-0.3.0/drawdata/static/
--rw-r--r--   0 vincent    (501) staff       (20)      390 2024-02-24 12:36:19.000000 drawdata-0.3.0/drawdata/static/scatter_widget.css
--rw-r--r--   0 vincent    (501) staff       (20)   476692 2024-02-24 12:36:19.000000 drawdata-0.3.0/drawdata/static/scatter_widget.js
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-02-24 12:37:26.423550 drawdata-0.3.0/drawdata.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)     3000 2024-02-24 12:37:26.000000 drawdata-0.3.0/drawdata.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      265 2024-02-24 12:37:26.000000 drawdata-0.3.0/drawdata.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2024-02-24 12:37:26.000000 drawdata-0.3.0/drawdata.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)       51 2024-02-24 12:37:26.000000 drawdata-0.3.0/drawdata.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)        9 2024-02-24 12:37:26.000000 drawdata-0.3.0/drawdata.egg-info/top_level.txt
--rw-r--r--   0 vincent    (501) staff       (20)       38 2024-02-24 12:37:26.424557 drawdata-0.3.0/setup.cfg
--rw-r--r--   0 vincent    (501) staff       (20)     1148 2024-02-24 12:36:19.000000 drawdata-0.3.0/setup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-14 13:12:54.042003 drawdata-0.3.1/
+-rw-r--r--   0 vincent    (501) staff       (20)     1077 2024-02-14 10:06:31.000000 drawdata-0.3.1/LICENSE
+-rw-r--r--   0 vincent    (501) staff       (20)     3000 2024-05-14 13:12:54.041877 drawdata-0.3.1/PKG-INFO
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-14 13:12:54.039680 drawdata-0.3.1/drawdata/
+-rw-r--r--   0 vincent    (501) staff       (20)     1690 2024-05-14 13:08:39.000000 drawdata-0.3.1/drawdata/__init__.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-14 13:12:54.040641 drawdata-0.3.1/drawdata/static/
+-rw-r--r--   0 vincent    (501) staff       (20)      390 2024-02-24 12:36:19.000000 drawdata-0.3.1/drawdata/static/scatter_widget.css
+-rw-r--r--   0 vincent    (501) staff       (20)   476692 2024-02-24 12:36:19.000000 drawdata-0.3.1/drawdata/static/scatter_widget.js
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-14 13:12:54.040324 drawdata-0.3.1/drawdata.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)     3000 2024-05-14 13:12:54.000000 drawdata-0.3.1/drawdata.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      265 2024-05-14 13:12:54.000000 drawdata-0.3.1/drawdata.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2024-05-14 13:12:54.000000 drawdata-0.3.1/drawdata.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       51 2024-05-14 13:12:54.000000 drawdata-0.3.1/drawdata.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        9 2024-05-14 13:12:54.000000 drawdata-0.3.1/drawdata.egg-info/top_level.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2024-05-14 13:12:54.042045 drawdata-0.3.1/setup.cfg
+-rw-r--r--   0 vincent    (501) staff       (20)     1148 2024-05-14 12:58:46.000000 drawdata-0.3.1/setup.py
```

### Comparing `drawdata-0.3.0/LICENSE` & `drawdata-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drawdata-0.3.0/PKG-INFO` & `drawdata-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drawdata
-Version: 0.3.0
+Version: 0.3.1
 Summary: draw a dataset from inside Jupyter
 Author: Vincent D. Warmerdam
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `drawdata-0.3.0/drawdata/__init__.py` & `drawdata-0.3.1/drawdata/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,7 +35,20 @@
         import pandas as pd 
         return pd.DataFrame(self.data)
 
     @property
     def data_as_polars(self):
         import polars as pl
         return pl.DataFrame(self.data)
+
+    @property
+    def data_as_X_y(self, kind='classification'):
+        import numpy as np
+
+        colors = [_['label'] for _ in self.data]
+        if np.unique(colors).shape[0] == 1:
+            X = np.array([[_['x']] for _ in self.data])
+            y = np.array([_['y'] for _ in self.data])
+            return X, y
+        X = np.array([[_['x'], _['y']] for _ in self.data])
+        y = np.array([_['label'] for _ in self.data])
+        return X, y
```

### Comparing `drawdata-0.3.0/drawdata/static/scatter_widget.js` & `drawdata-0.3.1/drawdata/static/scatter_widget.js`

 * *Files identical despite different names*

### Comparing `drawdata-0.3.0/drawdata.egg-info/PKG-INFO` & `drawdata-0.3.1/drawdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drawdata
-Version: 0.3.0
+Version: 0.3.1
 Summary: draw a dataset from inside Jupyter
 Author: Vincent D. Warmerdam
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `drawdata-0.3.0/setup.py` & `drawdata-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="drawdata",
-    version="0.3.0",
+    version="0.3.1",
     description="draw a dataset from inside Jupyter",
     author="Vincent D. Warmerdam",
     packages=find_packages(exclude=["notebooks"]),
     package_data={"drawdata": ["static/*.js", "static/*.css"]},
     long_description=read("readme.md"),
     long_description_content_type="text/markdown",
     install_requires=base_packages,
```

