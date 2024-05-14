# Comparing `tmp/continuedfractions-0.12.0.tar.gz` & `tmp/continuedfractions-0.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuedfractions-0.12.0.tar", last modified: Tue May 14 16:34:51 2024, max compression
+gzip compressed data, was "continuedfractions-0.12.1.tar", last modified: Tue May 14 17:14:45 2024, max compression
```

## Comparing `continuedfractions-0.12.0.tar` & `continuedfractions-0.12.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.0/LICENSE
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.0/LICENSE
--rw-r--r--   0        0        0     3162 2024-05-14 16:22:41.742134 continuedfractions-0.12.0/README.md
--rw-r--r--   0        0        0     3162 2024-05-14 16:22:41.742134 continuedfractions-0.12.0/README.md
--rw-r--r--   0        0        0     3506 2024-05-14 16:34:51.929492 continuedfractions-0.12.0/pyproject.toml
--rw-r--r--   0        0        0    31312 2024-03-28 15:58:08.840824 continuedfractions-0.12.0/src/continuedfractions/continuedfraction.py
--rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.0/src/continuedfractions/lib.py
--rw-r--r--   0        0        0    40644 2024-05-14 15:35:07.292234 continuedfractions-0.12.0/src/continuedfractions/sequences.py
--rw-r--r--   0        0        0     2077 2024-04-15 22:05:26.859297 continuedfractions-0.12.0/src/continuedfractions/utils.py
--rw-r--r--   0        0        0       23 2024-04-12 12:56:49.382276 continuedfractions-0.12.0/src/continuedfractions/version.py
--rw-r--r--   0        0        0    24146 1970-01-01 00:00:00.000000 continuedfractions-0.12.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.1/LICENSE
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.1/LICENSE
+-rw-r--r--   0        0        0     3162 2024-05-14 16:54:10.646159 continuedfractions-0.12.1/README.md
+-rw-r--r--   0        0        0     3162 2024-05-14 16:54:10.646159 continuedfractions-0.12.1/README.md
+-rw-r--r--   0        0        0     3506 2024-05-14 17:14:45.815444 continuedfractions-0.12.1/pyproject.toml
+-rw-r--r--   0        0        0    31312 2024-03-28 15:58:08.840824 continuedfractions-0.12.1/src/continuedfractions/continuedfraction.py
+-rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.1/src/continuedfractions/lib.py
+-rw-r--r--   0        0        0    40513 2024-05-14 17:09:06.012944 continuedfractions-0.12.1/src/continuedfractions/sequences.py
+-rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.1/src/continuedfractions/utils.py
+-rw-r--r--   0        0        0       23 2024-05-14 17:08:51.169656 continuedfractions-0.12.1/src/continuedfractions/version.py
+-rw-r--r--   0        0        0    24146 1970-01-01 00:00:00.000000 continuedfractions-0.12.1/PKG-INFO
```

### Comparing `continuedfractions-0.12.0/LICENSE` & `continuedfractions-0.12.1/LICENSE`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.0/README.md` & `continuedfractions-0.12.1/README.md`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.0/pyproject.toml` & `continuedfractions-0.12.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
-version = "0.12.0"
+version = "0.12.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 user = [
     "jupyter",
```

### Comparing `continuedfractions-0.12.0/src/continuedfractions/continuedfraction.py` & `continuedfractions-0.12.1/src/continuedfractions/continuedfraction.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.0/src/continuedfractions/lib.py` & `continuedfractions-0.12.1/src/continuedfractions/lib.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.0/src/continuedfractions/sequences.py` & `continuedfractions-0.12.1/src/continuedfractions/sequences.py`

 * *Files 1% similar despite different names*

```diff
@@ -805,20 +805,16 @@
         yield 1, 1
 
         if n == 2:
             yield 2, 1
         elif n > 1:
             yield from self.search_root(n - 1, self.roots[0])
 
-        if n > 2 and n % 2 == 0:
-            yield from self.search_root(n - 1, self.roots[1])
-        elif n > 2 and n % 2 == 1:
-            yield from self.search_root(n - 1, self.roots[1])
-
         if n > 2:
+            yield from self.search_root(n - 1, self.roots[1])
             yield from tuple(product([n], coprime_integers(n)))
 
 
 @functools.cache
 def coprime_pairs(n: int, /) -> tuple[KSRMNode]:
     """A function wrapper to return a sequence (tuple) of all pairs of (positive) coprime integers :math:`<= n`.
```

### Comparing `continuedfractions-0.12.0/src/continuedfractions/utils.py` & `continuedfractions-0.12.1/src/continuedfractions/utils.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.0/PKG-INFO` & `continuedfractions-0.12.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuedfractions
-Version: 0.12.0
+Version: 0.12.1
 Summary: Object-oriented continued fractions with Python.
 Keywords: computational number theory,coprime integers,continued fractions,farey sequences,irrational numbers,mediants,number theory,rational approximation,rational numbers,real numbers
 Author-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 Maintainer-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 License: Mozilla Public License Version 2.0
         ==================================
```

