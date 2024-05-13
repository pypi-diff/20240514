# Comparing `tmp/elements-3.3.0.tar.gz` & `tmp/elements-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elements-3.3.0.tar", last modified: Fri May 10 22:03:09 2024, max compression
+gzip compressed data, was "elements-3.4.0.tar", last modified: Mon May 13 22:39:43 2024, max compression
```

## Comparing `elements-3.3.0.tar` & `elements-3.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:03:09.573488 elements-3.3.0/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.3.0/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.3.0/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-10 22:03:09.573488 elements-3.3.0/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.3.0/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:03:09.573488 elements-3.3.0/elements/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      541 2024-05-10 22:02:50.000000 elements-3.3.0/elements/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.3.0/elements/agg.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3370 2023-12-10 19:55:19.000000 elements-3.3.0/elements/checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.3.0/elements/config.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.3.0/elements/counter.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.3.0/elements/flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.3.0/elements/fps.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.3.0/elements/logger.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5616 2023-12-10 19:47:00.000000 elements-3.3.0/elements/path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.3.0/elements/plotting.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.3.0/elements/printing.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.3.0/elements/rwlock.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.3.0/elements/timer.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.3.0/elements/tree.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.3.0/elements/usage.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.3.0/elements/utils.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.3.0/elements/uuid.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.3.0/elements/when.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:03:09.573488 elements-3.3.0/elements.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-10 22:03:09.000000 elements-3.3.0/elements.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      654 2024-05-10 22:03:09.000000 elements-3.3.0/elements.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-10 22:03:09.000000 elements-3.3.0/elements.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        6 2024-05-10 22:03:09.000000 elements-3.3.0/elements.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-10 22:03:09.000000 elements-3.3.0/elements.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       80 2023-12-13 02:15:19.000000 elements-3.3.0/requirements-optional.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        6 2023-12-10 19:58:55.000000 elements-3.3.0/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-10 22:03:09.573488 elements-3.3.0/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.3.0/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:03:09.573488 elements-3.3.0/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2023-12-10 20:38:32.000000 elements-3.3.0/tests/test_basics.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.3.0/tests/test_flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1506 2024-05-10 21:58:08.000000 elements-3.3.0/tests/test_path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.3.0/tests/test_tree.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-13 22:39:43.912312 elements-3.4.0/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.4.0/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.4.0/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-13 22:39:43.912312 elements-3.4.0/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.4.0/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-13 22:39:43.908312 elements-3.4.0/elements/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      541 2024-05-13 22:39:29.000000 elements-3.4.0/elements/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.4.0/elements/agg.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3370 2023-12-10 19:55:19.000000 elements-3.4.0/elements/checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.4.0/elements/config.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.4.0/elements/counter.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.4.0/elements/flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.4.0/elements/fps.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.4.0/elements/logger.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6766 2024-05-13 22:38:41.000000 elements-3.4.0/elements/path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.4.0/elements/plotting.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.4.0/elements/printing.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.4.0/elements/rwlock.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.4.0/elements/timer.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.4.0/elements/tree.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.4.0/elements/usage.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.4.0/elements/utils.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.4.0/elements/uuid.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.4.0/elements/when.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-13 22:39:43.912312 elements-3.4.0/elements.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-13 22:39:43.000000 elements-3.4.0/elements.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      654 2024-05-13 22:39:43.000000 elements-3.4.0/elements.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-13 22:39:43.000000 elements-3.4.0/elements.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       39 2024-05-13 22:39:43.000000 elements-3.4.0/elements.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-13 22:39:43.000000 elements-3.4.0/elements.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.4.0/requirements-optional.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       39 2024-05-13 22:39:20.000000 elements-3.4.0/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-13 22:39:43.912312 elements-3.4.0/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.4.0/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-13 22:39:43.912312 elements-3.4.0/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2023-12-10 20:38:32.000000 elements-3.4.0/tests/test_basics.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.4.0/tests/test_flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1506 2024-05-10 21:58:08.000000 elements-3.4.0/tests/test_path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.4.0/tests/test_tree.py
```

### Comparing `elements-3.3.0/LICENSE` & `elements-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/PKG-INFO` & `elements-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.3.0
+Version: 3.4.0
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.3.0/README.md` & `elements-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/__init__.py` & `elements-3.4.0/elements/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.3.0'
+__version__ = '3.4.0'
 
 from .agg import Agg
 from .checkpoint import Checkpoint
 from .config import Config
 from .counter import Counter
 from .flags import Flags
 from .fps import FPS
```

### Comparing `elements-3.3.0/elements/agg.py` & `elements-3.4.0/elements/agg.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/checkpoint.py` & `elements-3.4.0/elements/checkpoint.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/config.py` & `elements-3.4.0/elements/config.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/counter.py` & `elements-3.4.0/elements/counter.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/flags.py` & `elements-3.4.0/elements/flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/logger.py` & `elements-3.4.0/elements/logger.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/path.py` & `elements-3.4.0/elements/path.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,15 +162,68 @@
     else:
       shutil.copytree(self, type(self)(dest), dirs_exist_ok=True)
 
   def move(self, dest):
     shutil.move(self, dest)
 
 
-class GFilePath(Path):
+class GCSPath(Path):
+
+  __slots__ = ('_path',)
+
+  fs = None
+
+  def __init__(self, path):
+    path = str(path)
+    if not (path.startswith('/') or '://' in path):
+      path = os.path.abspath(os.path.expanduser(path))
+    super().__init__(path)
+    if not type(self).fs:
+      import gcsfs
+      type(self).fs = gcsfs.GCSFileSystem()
+
+  @contextlib.contextmanager
+  def open(self, mode='r'):
+    yield self.fs.open(str(self), mode)
+
+  def absolute(self):
+    return self
+
+  def glob(self, pattern):
+    for path in self.fs.glob(f'{str(self)}/{pattern}'):
+      yield type(self)(path)
+
+  def exists(self):
+    return self.fs.exists(str(self))
+
+  def isfile(self):
+    return self.fs.isfile(str(self))
+
+  def isdir(self):
+    return self.fs.isdir(str(self))
+
+  def mkdirs(self):
+    self.fs.makedirs(str(self), exist_ok=True)
+
+  def remove(self):
+    self.fs.rm(str(self), recursive=False)
+
+  def rmtree(self):
+    self.fs.rm(str(self), recursive=True)
+
+  def copy(self, dest):
+    dest = Path(dest)
+    self.fs.copy(str(self), str(dest), recursive=True)
+
+  def move(self, dest):
+    dest = Path(dest)
+    self.fs.mv(self, str(dest), recursive=True)
+
+
+class TFPath(Path):
 
   __slots__ = ('_path',)
 
   gfile = None
 
   def __init__(self, path):
     path = str(path)
@@ -216,28 +269,27 @@
   def remove(self):
     self.gfile.remove(str(self))
 
   def rmtree(self):
     self.gfile.rmtree(str(self))
 
   def copy(self, dest):
-    dest = type(self)(dest)
+    dest = Path(dest)
     if self.isfile():
       self.gfile.copy(str(self), str(dest), overwrite=True)
     else:
       for folder, subdirs, files in self.gfile.walk(str(self)):
         target = type(self)(folder.replace(str(self), str(dest)))
         target.exists() or target.mkdirs()
         for file in files:
           (type(self)(folder) / file).copy(target / file)
 
   def move(self, dest):
     dest = Path(dest)
-    if dest.isdir():
-      dest.rmtree()
     self.gfile.rename(self, str(dest), overwrite=True)
 
 
 Path.filesystems = [
-    (GFilePath, lambda path: path.startswith('gs://')),
+    (GCSPath, lambda path: path.startswith('gs://')),
+    (TFPath, lambda path: path.startswith('/cns/')),
     (LocalPath, lambda path: True),
 ]
```

### Comparing `elements-3.3.0/elements/plotting.py` & `elements-3.4.0/elements/plotting.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/printing.py` & `elements-3.4.0/elements/printing.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/rwlock.py` & `elements-3.4.0/elements/rwlock.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/timer.py` & `elements-3.4.0/elements/timer.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/tree.py` & `elements-3.4.0/elements/tree.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/usage.py` & `elements-3.4.0/elements/usage.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/uuid.py` & `elements-3.4.0/elements/uuid.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements/when.py` & `elements-3.4.0/elements/when.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/elements.egg-info/PKG-INFO` & `elements-3.4.0/elements.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.3.0
+Version: 3.4.0
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.3.0/elements.egg-info/SOURCES.txt` & `elements-3.4.0/elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/setup.py` & `elements-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/tests/test_basics.py` & `elements-3.4.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/tests/test_flags.py` & `elements-3.4.0/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/tests/test_path.py` & `elements-3.4.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `elements-3.3.0/tests/test_tree.py` & `elements-3.4.0/tests/test_tree.py`

 * *Files identical despite different names*

