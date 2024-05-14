# Comparing `tmp/compas_dr-0.3.0.tar.gz` & `tmp/compas_dr-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_dr-0.3.0.tar", last modified: Thu Feb 29 22:27:39 2024, max compression
+gzip compressed data, was "compas_dr-0.3.1.tar", last modified: Tue May 14 13:39:03 2024, max compression
```

## Comparing `compas_dr-0.3.0.tar` & `compas_dr-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:27:39.148427 compas_dr-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-29 22:27:27.000000 compas_dr-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-02-29 22:27:39.148427 compas_dr-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-29 22:27:27.000000 compas_dr-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-02-29 22:27:27.000000 compas_dr-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-29 22:27:27.000000 compas_dr-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-29 22:27:27.000000 compas_dr-0.3.0/requirements-hpc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-29 22:27:27.000000 compas_dr-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 22:27:39.148427 compas_dr-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:27:39.140427 compas_dr-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:27:39.144427 compas_dr-0.3.0/src/compas_dr/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:27:39.148427 compas_dr-0.3.0/src/compas_dr/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/constraints/circleconstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/constraints/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/constraints/curveconstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/constraints/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/constraints/lineconstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/constraints/planeconstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/constraints/surfaceconstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:27:39.148427 compas_dr-0.3.0/src/compas_dr/loads/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/loads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/loads/selfweight.py
--rw-r--r--   0 runner    (1001) docker     (127)     9934 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/numdata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:27:39.148427 compas_dr-0.3.0/src/compas_dr/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/solvers/dr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/solvers/dr_constrained_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/solvers/dr_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-29 22:27:27.000000 compas_dr-0.3.0/src/compas_dr/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:27:39.148427 compas_dr-0.3.0/src/compas_dr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-02-29 22:27:39.000000 compas_dr-0.3.0/src/compas_dr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-02-29 22:27:39.000000 compas_dr-0.3.0/src/compas_dr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 22:27:39.000000 compas_dr-0.3.0/src/compas_dr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 22:27:38.000000 compas_dr-0.3.0/src/compas_dr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-29 22:27:39.000000 compas_dr-0.3.0/src/compas_dr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-29 22:27:39.000000 compas_dr-0.3.0/src/compas_dr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:27:39.148427 compas_dr-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-29 22:27:27.000000 compas_dr-0.3.0/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.164856 compas_dr-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 13:38:51.000000 compas_dr-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-14 13:39:03.164856 compas_dr-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-14 13:38:51.000000 compas_dr-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-14 13:38:51.000000 compas_dr-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 13:38:51.000000 compas_dr-0.3.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 13:38:51.000000 compas_dr-0.3.1/requirements-hpc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 13:38:51.000000 compas_dr-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:39:03.164856 compas_dr-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.156856 compas_dr-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.156856 compas_dr-0.3.1/src/compas_dr/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.160856 compas_dr-0.3.1/src/compas_dr/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/constraints/circleconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/constraints/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/constraints/curveconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/constraints/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/constraints/lineconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/constraints/planeconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/constraints/surfaceconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.160856 compas_dr-0.3.1/src/compas_dr/loads/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/loads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/loads/selfweight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9934 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/numdata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.160856 compas_dr-0.3.1/src/compas_dr/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/solvers/dr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/solvers/dr_constrained_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/solvers/dr_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-14 13:38:51.000000 compas_dr-0.3.1/src/compas_dr/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.160856 compas_dr-0.3.1/src/compas_dr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-14 13:39:03.000000 compas_dr-0.3.1/src/compas_dr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-14 13:39:03.000000 compas_dr-0.3.1/src/compas_dr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:39:03.000000 compas_dr-0.3.1/src/compas_dr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:39:02.000000 compas_dr-0.3.1/src/compas_dr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 13:39:03.000000 compas_dr-0.3.1/src/compas_dr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 13:39:03.000000 compas_dr-0.3.1/src/compas_dr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.160856 compas_dr-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 13:38:51.000000 compas_dr-0.3.1/tests/test_placeholder.py
```

### Comparing `compas_dr-0.3.0/LICENSE` & `compas_dr-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_dr-0.3.0/PKG-INFO` & `compas_dr-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_dr
-Version: 0.3.0
+Version: 0.3.1
 Summary: Constrained form finding using the Dynamic Relaxation Method.
 Author-email: tom van mele <tom.v.mele@gmail.com>
 License: MIT License
         
         ETH Zurich - Block Research Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,21 +34,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: compas>=2.0.1
+Requires-Dist: compas>=2.1
 Provides-Extra: dev
 Requires-Dist: attrs>=17.4; extra == "dev"
 Requires-Dist: black>=22.12.0; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
-Requires-Dist: compas_invocations; extra == "dev"
+Requires-Dist: compas_invocations2; extra == "dev"
 Requires-Dist: compas_notebook; extra == "dev"
+Requires-Dist: compas_viewer; extra == "dev"
 Requires-Dist: invoke>=0.14; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx_compas2_theme; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Provides-Extra: hpc
 Requires-Dist: numba; extra == "hpc"
```

### Comparing `compas_dr-0.3.0/README.md` & `compas_dr-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `compas_dr-0.3.0/pyproject.toml` & `compas_dr-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 ]
 
 # ============================================================================
 # replace bumpversion.cfg
 # ============================================================================
 
 [tool.bumpversion]
-current_version = "0.3.0"
+current_version = "0.3.1"
 message = "Bump version to {new_version}"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "src/compas_dr/__init__.py"
 search = "{current_version}"
@@ -84,18 +84,18 @@
 replace = "[{new_version}] {now:%Y-%m-%d}"
 
 # ============================================================================
 # replace setup.cfg
 # ============================================================================
 
 [tool.black]
-line-length = 119
+line-length = 179
 
 [tool.ruff]
-line-length = 119
+line-length = 179
 indent-width = 4
 target-version = "py39"
 
 [tool.ruff.lint]
 select = ["E", "F", "I"]
 
 [tool.ruff.lint.per-file-ignores]
```

### Comparing `compas_dr-0.3.0/src/compas_dr/__init__.py` & `compas_dr-0.3.1/src/compas_dr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 
 __author__ = ["tom van mele"]
 __copyright__ = "ETH Zurich - Block Research Group"
 __license__ = "MIT License"
 __email__ = "tom.v.mele@gmail.com"
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
```

### Comparing `compas_dr-0.3.0/src/compas_dr/constraints/__init__.py` & `compas_dr-0.3.1/src/compas_dr/constraints/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""This package defines geometric constraints that can be applied to the fixed vertices of a mesh/cable-mesh.
-"""
+"""This package defines geometric constraints that can be applied to the fixed vertices of a mesh/cable-mesh."""
 
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
 
 from compas.geometry import Line
 from compas.geometry import Plane
```

### Comparing `compas_dr-0.3.0/src/compas_dr/constraints/circleconstraint.py` & `compas_dr-0.3.1/src/compas_dr/constraints/circleconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_dr-0.3.0/src/compas_dr/constraints/constraint.py` & `compas_dr-0.3.1/src/compas_dr/constraints/constraint.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,17 +64,15 @@
         gtype = type(geometry)
         cls = None
         for type_ in inspect.getmro(gtype):
             cls = Constraint.GEOMETRY_CONSTRAINT.get(type_)
             if cls is not None:
                 break
         if cls is None:
-            raise GeometryNotRegisteredAsConstraint(
-                "No constraint is registered for this geometry type: {}".format(gtype)
-            )
+            raise GeometryNotRegisteredAsConstraint("No constraint is registered for this geometry type: {}".format(gtype))
         return cls
 
     def __new__(cls, *args, **kwargs):
         geometry = args[0]
         cls = Constraint.get_constraint_cls(geometry)
         return super(Constraint, cls).__new__(cls)
```

### Comparing `compas_dr-0.3.0/src/compas_dr/constraints/curveconstraint.py` & `compas_dr-0.3.1/src/compas_dr/constraints/curveconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_dr-0.3.0/src/compas_dr/constraints/lineconstraint.py` & `compas_dr-0.3.1/src/compas_dr/constraints/lineconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_dr-0.3.0/src/compas_dr/constraints/planeconstraint.py` & `compas_dr-0.3.1/src/compas_dr/constraints/planeconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_dr-0.3.0/src/compas_dr/constraints/surfaceconstraint.py` & `compas_dr-0.3.1/src/compas_dr/constraints/surfaceconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_dr-0.3.0/src/compas_dr/loads/selfweight.py` & `compas_dr-0.3.1/src/compas_dr/loads/selfweight.py`

 * *Files identical despite different names*

### Comparing `compas_dr-0.3.0/src/compas_dr/numdata.py` & `compas_dr-0.3.1/src/compas_dr/numdata.py`

 * *Files identical despite different names*

### Comparing `compas_dr-0.3.0/src/compas_dr/solvers/dr.py` & `compas_dr-0.3.1/src/compas_dr/solvers/dr.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,38 +251,23 @@
             a1 = a(
                 K[1][0] * dt,
                 [[V0[i][axis] + K[1][1] * k0[i][axis] for axis in (0, 1, 2)] for i in range(n)],
             )
             k1 = [[dt * a1[i][axis] for axis in (0, 1, 2)] for i in range(n)]
             a2 = a(
                 K[2][0] * dt,
-                [
-                    [V0[i][axis] + K[2][1] * k0[i][axis] + K[2][2] * k1[i][axis] for axis in (0, 1, 2)]
-                    for i in range(n)
-                ],
+                [[V0[i][axis] + K[2][1] * k0[i][axis] + K[2][2] * k1[i][axis] for axis in (0, 1, 2)] for i in range(n)],
             )
             k2 = [[dt * a2[i][axis] for axis in (0, 1, 2)] for i in range(n)]
             a3 = a(
                 K[3][0] * dt,
-                [
-                    [
-                        V0[i][axis] + K[3][1] * k0[i][axis] + K[3][2] * k1[i][axis] + K[3][3] * k2[i][axis]
-                        for axis in (0, 1, 2)
-                    ]
-                    for i in range(n)
-                ],
+                [[V0[i][axis] + K[3][1] * k0[i][axis] + K[3][2] * k1[i][axis] + K[3][3] * k2[i][axis] for axis in (0, 1, 2)] for i in range(n)],
             )
             k3 = [[dt * a3[i][axis] for axis in (0, 1, 2)] for i in range(n)]
-            return [
-                [
-                    B[0] * k0[i][axis] + B[1] * k1[i][axis] + B[2] * k2[i][axis] + B[3] * k3[i][axis]
-                    for axis in (0, 1, 2)
-                ]
-                for i in range(n)
-            ]
+            return [[B[0] * k0[i][axis] + B[1] * k1[i][axis] + B[2] * k2[i][axis] + B[3] * k3[i][axis] for axis in (0, 1, 2)] for i in range(n)]
 
         raise NotImplementedError
 
     # --------------------------------------------------------------------------
     # start iterating
     # --------------------------------------------------------------------------
```

### Comparing `compas_dr-0.3.0/src/compas_dr/solvers/dr_constrained_numpy.py` & `compas_dr-0.3.1/src/compas_dr/solvers/dr_constrained_numpy.py`

 * *Files identical despite different names*

### Comparing `compas_dr-0.3.0/src/compas_dr/solvers/dr_numpy.py` & `compas_dr-0.3.1/src/compas_dr/solvers/dr_numpy.py`

 * *Files identical despite different names*

### Comparing `compas_dr-0.3.0/src/compas_dr/types.py` & `compas_dr-0.3.1/src/compas_dr/types.py`

 * *Files identical despite different names*

### Comparing `compas_dr-0.3.0/src/compas_dr.egg-info/PKG-INFO` & `compas_dr-0.3.1/src/compas_dr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_dr
-Version: 0.3.0
+Version: 0.3.1
 Summary: Constrained form finding using the Dynamic Relaxation Method.
 Author-email: tom van mele <tom.v.mele@gmail.com>
 License: MIT License
         
         ETH Zurich - Block Research Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,21 +34,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: compas>=2.0.1
+Requires-Dist: compas>=2.1
 Provides-Extra: dev
 Requires-Dist: attrs>=17.4; extra == "dev"
 Requires-Dist: black>=22.12.0; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
-Requires-Dist: compas_invocations; extra == "dev"
+Requires-Dist: compas_invocations2; extra == "dev"
 Requires-Dist: compas_notebook; extra == "dev"
+Requires-Dist: compas_viewer; extra == "dev"
 Requires-Dist: invoke>=0.14; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx_compas2_theme; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Provides-Extra: hpc
 Requires-Dist: numba; extra == "hpc"
```

### Comparing `compas_dr-0.3.0/src/compas_dr.egg-info/SOURCES.txt` & `compas_dr-0.3.1/src/compas_dr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

