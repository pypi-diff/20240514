# Comparing `tmp/pyrefactoring-0.0.1.1.post1.tar.gz` & `tmp/pyrefactoring-0.0.1.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrefactoring-0.0.1.1.post1.tar", last modified: Thu Apr  4 02:04:46 2024, max compression
+gzip compressed data, was "pyrefactoring-0.0.1.1.post2.tar", last modified: Tue May 14 04:50:57 2024, max compression
```

## Comparing `pyrefactoring-0.0.1.1.post1.tar` & `pyrefactoring-0.0.1.1.post2.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.629231 pyrefactoring-0.0.1.1.post1/
--rw-r--r--   0 hieupth    (501) staff       (20)    11357 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/LICENSE
--rw-r--r--   0 hieupth    (501) staff       (20)      592 2024-04-04 02:04:46.628970 pyrefactoring-0.0.1.1.post1/PKG-INFO
--rw-r--r--   0 hieupth    (501) staff       (20)      332 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/README.md
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.628764 pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/
--rw-r--r--   0 hieupth    (501) staff       (20)      592 2024-04-04 02:04:46.000000 pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/PKG-INFO
--rw-r--r--   0 hieupth    (501) staff       (20)      593 2024-04-04 02:04:46.000000 pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/SOURCES.txt
--rw-r--r--   0 hieupth    (501) staff       (20)        1 2024-04-04 02:04:46.000000 pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/dependency_links.txt
--rw-r--r--   0 hieupth    (501) staff       (20)        9 2024-04-04 02:04:46.000000 pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/top_level.txt
--rw-r--r--   0 hieupth    (501) staff       (20)        1 2024-04-04 02:04:46.000000 pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/zip-safe
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.626443 pyrefactoring-0.0.1.1.post1/refactor/
--rw-r--r--   0 hieupth    (501) staff       (20)        0 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/__init__.py
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.626856 pyrefactoring-0.0.1.1.post1/refactor/common/
--rw-r--r--   0 hieupth    (501) staff       (20)       33 2024-03-05 18:01:45.000000 pyrefactoring-0.0.1.1.post1/refactor/common/__init__.py
--rw-r--r--   0 hieupth    (501) staff       (20)     1874 2024-03-05 18:02:30.000000 pyrefactoring-0.0.1.1.post1/refactor/common/processor.py
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.627134 pyrefactoring-0.0.1.1.post1/refactor/patterns/
--rw-r--r--   0 hieupth    (501) staff       (20)        0 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/patterns/__init__.py
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.627445 pyrefactoring-0.0.1.1.post1/refactor/patterns/creation/
--rw-r--r--   0 hieupth    (501) staff       (20)       33 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/patterns/creation/__init__.py
--rw-r--r--   0 hieupth    (501) staff       (20)     1482 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/patterns/creation/singleton.py
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.627729 pyrefactoring-0.0.1.1.post1/refactor/utils/
--rw-r--r--   0 hieupth    (501) staff       (20)        0 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/utils/__init__.py
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.628234 pyrefactoring-0.0.1.1.post1/refactor/utils/resources/
--rw-r--r--   0 hieupth    (501) staff       (20)       62 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/utils/resources/__init__.py
--rw-r--r--   0 hieupth    (501) staff       (20)     2117 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/utils/resources/abs.py
--rw-r--r--   0 hieupth    (501) staff       (20)     1812 2024-04-03 16:27:03.000000 pyrefactoring-0.0.1.1.post1/refactor/utils/resources/base.py
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.628589 pyrefactoring-0.0.1.1.post1/refactor/utils/versioning/
--rw-r--r--   0 hieupth    (501) staff       (20)       27 2024-04-03 16:27:11.000000 pyrefactoring-0.0.1.1.post1/refactor/utils/versioning/__init__.py
--rw-r--r--   0 hieupth    (501) staff       (20)     1828 2024-04-03 16:27:11.000000 pyrefactoring-0.0.1.1.post1/refactor/utils/versioning/dot.py
--rw-r--r--   0 hieupth    (501) staff       (20)       38 2024-04-04 02:04:46.629285 pyrefactoring-0.0.1.1.post1/setup.cfg
--rw-r--r--   0 hieupth    (501) staff       (20)     2636 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/setup.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-05-14 04:50:57.338788 pyrefactoring-0.0.1.1.post2/
+-rw-r--r--   0 hieupth    (501) staff       (20)    34523 2024-04-25 09:09:05.000000 pyrefactoring-0.0.1.1.post2/LICENSE
+-rw-r--r--   0 hieupth    (501) staff       (20)      592 2024-05-14 04:50:57.338584 pyrefactoring-0.0.1.1.post2/PKG-INFO
+-rw-r--r--   0 hieupth    (501) staff       (20)      296 2024-04-25 09:13:00.000000 pyrefactoring-0.0.1.1.post2/README.md
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-05-14 04:50:57.338398 pyrefactoring-0.0.1.1.post2/pyrefactoring.egg-info/
+-rw-r--r--   0 hieupth    (501) staff       (20)      592 2024-05-14 04:50:57.000000 pyrefactoring-0.0.1.1.post2/pyrefactoring.egg-info/PKG-INFO
+-rw-r--r--   0 hieupth    (501) staff       (20)      660 2024-05-14 04:50:57.000000 pyrefactoring-0.0.1.1.post2/pyrefactoring.egg-info/SOURCES.txt
+-rw-r--r--   0 hieupth    (501) staff       (20)        1 2024-05-14 04:50:57.000000 pyrefactoring-0.0.1.1.post2/pyrefactoring.egg-info/dependency_links.txt
+-rw-r--r--   0 hieupth    (501) staff       (20)        9 2024-05-14 04:50:57.000000 pyrefactoring-0.0.1.1.post2/pyrefactoring.egg-info/top_level.txt
+-rw-r--r--   0 hieupth    (501) staff       (20)        1 2024-04-04 02:04:46.000000 pyrefactoring-0.0.1.1.post2/pyrefactoring.egg-info/zip-safe
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-05-14 04:50:57.335332 pyrefactoring-0.0.1.1.post2/refactor/
+-rw-r--r--   0 hieupth    (501) staff       (20)        0 2024-05-11 07:53:53.000000 pyrefactoring-0.0.1.1.post2/refactor/__init__.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-05-14 04:50:57.335647 pyrefactoring-0.0.1.1.post2/refactor/common/
+-rw-r--r--   0 hieupth    (501) staff       (20)       27 2024-05-14 03:35:10.000000 pyrefactoring-0.0.1.1.post2/refactor/common/__init__.py
+-rw-r--r--   0 hieupth    (501) staff       (20)      487 2024-05-14 04:42:54.000000 pyrefactoring-0.0.1.1.post2/refactor/common/object.py
+-rw-r--r--   0 hieupth    (501) staff       (20)     1874 2024-03-05 18:02:30.000000 pyrefactoring-0.0.1.1.post2/refactor/common/processor.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-05-14 04:50:57.336104 pyrefactoring-0.0.1.1.post2/refactor/patterns/
+-rw-r--r--   0 hieupth    (501) staff       (20)       33 2024-05-11 04:31:59.000000 pyrefactoring-0.0.1.1.post2/refactor/patterns/__init__.py
+-rw-r--r--   0 hieupth    (501) staff       (20)      610 2024-05-11 04:22:06.000000 pyrefactoring-0.0.1.1.post2/refactor/patterns/singleton.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-05-14 04:50:57.336328 pyrefactoring-0.0.1.1.post2/refactor/system/
+-rw-r--r--   0 hieupth    (501) staff       (20)        0 2024-05-13 09:34:17.000000 pyrefactoring-0.0.1.1.post2/refactor/system/__init__.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-05-14 04:50:57.336515 pyrefactoring-0.0.1.1.post2/refactor/system/logging/
+-rw-r--r--   0 hieupth    (501) staff       (20)      168 2024-05-13 10:10:30.000000 pyrefactoring-0.0.1.1.post2/refactor/system/logging/__init__.py
+-rw-r--r--   0 hieupth    (501) staff       (20)     2294 2024-05-14 04:38:32.000000 pyrefactoring-0.0.1.1.post2/refactor/system/logging/stdout.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-05-14 04:50:57.336964 pyrefactoring-0.0.1.1.post2/refactor/utils/
+-rw-r--r--   0 hieupth    (501) staff       (20)        0 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post2/refactor/utils/__init__.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-05-14 04:50:57.337573 pyrefactoring-0.0.1.1.post2/refactor/utils/resource/
+-rw-r--r--   0 hieupth    (501) staff       (20)       27 2024-05-14 04:43:14.000000 pyrefactoring-0.0.1.1.post2/refactor/utils/resource/__init__.py
+-rw-r--r--   0 hieupth    (501) staff       (20)     2681 2024-05-14 04:45:26.000000 pyrefactoring-0.0.1.1.post2/refactor/utils/resource/abs.py
+-rw-r--r--   0 hieupth    (501) staff       (20)     2050 2024-05-14 04:45:26.000000 pyrefactoring-0.0.1.1.post2/refactor/utils/resource/base.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-05-14 04:50:57.338132 pyrefactoring-0.0.1.1.post2/refactor/utils/version/
+-rw-r--r--   0 hieupth    (501) staff       (20)       27 2024-04-03 16:27:11.000000 pyrefactoring-0.0.1.1.post2/refactor/utils/version/__init__.py
+-rw-r--r--   0 hieupth    (501) staff       (20)     1985 2024-05-11 06:56:16.000000 pyrefactoring-0.0.1.1.post2/refactor/utils/version/dot.py
+-rw-r--r--   0 hieupth    (501) staff       (20)       38 2024-05-14 04:50:57.338832 pyrefactoring-0.0.1.1.post2/setup.cfg
+-rw-r--r--   0 hieupth    (501) staff       (20)     2636 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post2/setup.py
```

### Comparing `pyrefactoring-0.0.1.1.post1/PKG-INFO` & `pyrefactoring-0.0.1.1.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrefactoring
-Version: 0.0.1.1.post1
+Version: 0.0.1.1.post2
 Summary: Restructuring existing code from a mess into clean code, simple design and performance application
 Home-page: https://gitlab.com/hieupth/pyrefactor
 Author: Hieu Pham
 Author-email: 64821726+hieupth@users.noreply.github.com
 License: Copyright (c) 2023 Hieu Pham
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/PKG-INFO` & `pyrefactoring-0.0.1.1.post2/pyrefactoring.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrefactoring
-Version: 0.0.1.1.post1
+Version: 0.0.1.1.post2
 Summary: Restructuring existing code from a mess into clean code, simple design and performance application
 Home-page: https://gitlab.com/hieupth/pyrefactor
 Author: Hieu Pham
 Author-email: 64821726+hieupth@users.noreply.github.com
 License: Copyright (c) 2023 Hieu Pham
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/SOURCES.txt` & `pyrefactoring-0.0.1.1.post2/pyrefactoring.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 pyrefactoring.egg-info/PKG-INFO
 pyrefactoring.egg-info/SOURCES.txt
 pyrefactoring.egg-info/dependency_links.txt
 pyrefactoring.egg-info/top_level.txt
 pyrefactoring.egg-info/zip-safe
 refactor/__init__.py
 refactor/common/__init__.py
+refactor/common/object.py
 refactor/common/processor.py
 refactor/patterns/__init__.py
-refactor/patterns/creation/__init__.py
-refactor/patterns/creation/singleton.py
+refactor/patterns/singleton.py
+refactor/system/__init__.py
+refactor/system/logging/__init__.py
+refactor/system/logging/stdout.py
 refactor/utils/__init__.py
-refactor/utils/resources/__init__.py
-refactor/utils/resources/abs.py
-refactor/utils/resources/base.py
-refactor/utils/versioning/__init__.py
-refactor/utils/versioning/dot.py
+refactor/utils/resource/__init__.py
+refactor/utils/resource/abs.py
+refactor/utils/resource/base.py
+refactor/utils/version/__init__.py
+refactor/utils/version/dot.py
```

### Comparing `pyrefactoring-0.0.1.1.post1/refactor/common/processor.py` & `pyrefactoring-0.0.1.1.post2/refactor/common/processor.py`

 * *Files identical despite different names*

### Comparing `pyrefactoring-0.0.1.1.post1/refactor/utils/versioning/dot.py` & `pyrefactoring-0.0.1.1.post2/refactor/utils/version/dot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-class DotVersion:
+class DotVer:
   """
   A version patterns use numbers and dot as separator such as x.y.z
   """
 
   @property
   def numbers(self):
     """
@@ -23,42 +23,49 @@
   def precedence(self, other, *args, **kwds) -> int:
     """
     Precedence when compare to another.
     :param other:   other dot version.
     :param args:    additional arguments.
     :param kwds:    additional keyword arguments.
     """
-    if not isinstance(other, DotVersion):
+    if not isinstance(other, DotVer):
       c1 = self.__class__.__name__
       c2 = other.__class__.__name__
       raise TypeError(f'{c1} cannot be compared to {c2}')
     # Calculate precedence.
     l1, l2 = len(self.numbers), len(other.numbers)
     for i in range(min(l1, l2)):
       x1, x2 = self.numbers[i], other.numbers[i]
       if x1 == x2:
         continue
       else:
         return -1 if x1 < x2 else 1
     # Longer is langer.
     return -1 if l1 < l2 else 1 if l1 > l2 else 0
 
+  # Convert to a string.
   def __str__(self):
     return '.'.join(self._numbers)
   
+  # Compare equal.
   def __eq__(self, __value: object) -> bool:
     return self.precedence(__value) == 0
   
+  # Compare not equal.
   def __ne__(self, __value: object) -> bool:
     return self.precedence(__value) != 0
   
+  # Compare greater.
   def __gt__(self, __value: object) -> bool:
     return self.precedence(__value) > 0
   
+  # Compare greater and equal.
   def __ge__(self, __value: object) -> bool:
     return self.precedence(__value) >= 0
   
+  # Compare less.
   def __lt__(self, __value: object) -> bool:
     return self.precedence(__value) < 0
   
+  # Compare less and equal.
   def __le__(self, __value: object) -> bool:
     return self.precedence(__value) <= 0
```

### Comparing `pyrefactoring-0.0.1.1.post1/setup.py` & `pyrefactoring-0.0.1.1.post2/setup.py`

 * *Files identical despite different names*

