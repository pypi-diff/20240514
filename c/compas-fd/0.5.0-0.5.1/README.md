# Comparing `tmp/compas_fd-0.5.0.tar.gz` & `tmp/compas_fd-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_fd-0.5.0.tar", last modified: Thu Feb 29 22:19:41 2024, max compression
+gzip compressed data, was "compas_fd-0.5.1.tar", last modified: Tue May 14 13:39:03 2024, max compression
```

## Comparing `compas_fd-0.5.0.tar` & `compas_fd-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:19:41.210637 compas_fd-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-29 22:19:29.000000 compas_fd-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-29 22:19:41.210637 compas_fd-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-29 22:19:29.000000 compas_fd-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-02-29 22:19:29.000000 compas_fd-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-29 22:19:29.000000 compas_fd-0.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-29 22:19:29.000000 compas_fd-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 22:19:41.210637 compas_fd-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:19:41.202637 compas_fd-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:19:41.202637 compas_fd-0.5.0/src/compas_fd/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:19:41.206637 compas_fd-0.5.0/src/compas_fd/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/constraints/circleconstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/constraints/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/constraints/curveconstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/constraints/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/constraints/frameconstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/constraints/lineconstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/constraints/planeconstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/constraints/surfaceconstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/constraints/vectorconstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:19:41.206637 compas_fd-0.5.0/src/compas_fd/loads/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/loads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/loads/selfweight.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:19:41.210637 compas_fd-0.5.0/src/compas_fd/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/solvers/fd_constrained_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/solvers/fd_numerical_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/solvers/fd_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/solvers/result.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-29 22:19:29.000000 compas_fd-0.5.0/src/compas_fd/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:19:41.210637 compas_fd-0.5.0/src/compas_fd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-29 22:19:41.000000 compas_fd-0.5.0/src/compas_fd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-02-29 22:19:41.000000 compas_fd-0.5.0/src/compas_fd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 22:19:41.000000 compas_fd-0.5.0/src/compas_fd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 22:19:41.000000 compas_fd-0.5.0/src/compas_fd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-29 22:19:41.000000 compas_fd-0.5.0/src/compas_fd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-29 22:19:41.000000 compas_fd-0.5.0/src/compas_fd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:19:41.210637 compas_fd-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-29 22:19:29.000000 compas_fd-0.5.0/tests/test_hypar.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-29 22:19:29.000000 compas_fd-0.5.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-29 22:19:29.000000 compas_fd-0.5.0/tests/test_selfweight.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.184488 compas_fd-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 13:38:53.000000 compas_fd-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-14 13:39:03.184488 compas_fd-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-14 13:38:53.000000 compas_fd-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-14 13:38:53.000000 compas_fd-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 13:38:53.000000 compas_fd-0.5.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 13:38:53.000000 compas_fd-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:39:03.184488 compas_fd-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.176488 compas_fd-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.180488 compas_fd-0.5.1/src/compas_fd/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.180488 compas_fd-0.5.1/src/compas_fd/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/constraints/circleconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/constraints/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/constraints/curveconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/constraints/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/constraints/frameconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/constraints/lineconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/constraints/planeconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/constraints/surfaceconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/constraints/vectorconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.184488 compas_fd-0.5.1/src/compas_fd/loads/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/loads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/loads/selfweight.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.184488 compas_fd-0.5.1/src/compas_fd/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/solvers/fd_constrained_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/solvers/fd_numerical_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/solvers/fd_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/solvers/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-14 13:38:53.000000 compas_fd-0.5.1/src/compas_fd/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.184488 compas_fd-0.5.1/src/compas_fd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-14 13:39:03.000000 compas_fd-0.5.1/src/compas_fd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-14 13:39:03.000000 compas_fd-0.5.1/src/compas_fd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:39:03.000000 compas_fd-0.5.1/src/compas_fd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:39:02.000000 compas_fd-0.5.1/src/compas_fd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 13:39:03.000000 compas_fd-0.5.1/src/compas_fd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 13:39:03.000000 compas_fd-0.5.1/src/compas_fd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:03.184488 compas_fd-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-14 13:38:53.000000 compas_fd-0.5.1/tests/test_hypar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 13:38:53.000000 compas_fd-0.5.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-14 13:38:53.000000 compas_fd-0.5.1/tests/test_selfweight.py
```

### Comparing `compas_fd-0.5.0/LICENSE` & `compas_fd-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/pyproject.toml` & `compas_fd-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 ]
 
 # ============================================================================
 # replace bumpversion.cfg
 # ============================================================================
 
 [tool.bumpversion]
-current_version = "0.5.0"
+current_version = "0.5.1"
 message = "Bump version to {new_version}"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "src/compas_fd/__init__.py"
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

### Comparing `compas_fd-0.5.0/src/compas_fd/__init__.py` & `compas_fd-0.5.1/src/compas_fd/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import compas
 
 
 __author__ = ["tom van mele <tom.v.mele@gmail.com>"]
 __copyright__ = "Block Research Group - ETH Zurich"
 __license__ = "MIT License"
 __email__ = "tom.v.mele@gmail.com"
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 get = compas.get
 
 
 HERE = os.path.dirname(__file__)
```

### Comparing `compas_fd-0.5.0/src/compas_fd/constraints/__init__.py` & `compas_fd-0.5.1/src/compas_fd/constraints/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""This package defines geometric constraints that can be applied to the fixed vertices of a mesh/cable-mesh.
-"""
+"""This package defines geometric constraints that can be applied to the fixed vertices of a mesh/cable-mesh."""
 
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
 
 from compas.geometry import Vector
 from compas.geometry import Frame
```

### Comparing `compas_fd-0.5.0/src/compas_fd/constraints/circleconstraint.py` & `compas_fd-0.5.1/src/compas_fd/constraints/circleconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/src/compas_fd/constraints/constraint.py` & `compas_fd-0.5.1/src/compas_fd/constraints/constraint.py`

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

### Comparing `compas_fd-0.5.0/src/compas_fd/constraints/curveconstraint.py` & `compas_fd-0.5.1/src/compas_fd/constraints/curveconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/src/compas_fd/constraints/frameconstraint.py` & `compas_fd-0.5.1/src/compas_fd/constraints/frameconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/src/compas_fd/constraints/lineconstraint.py` & `compas_fd-0.5.1/src/compas_fd/constraints/lineconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/src/compas_fd/constraints/planeconstraint.py` & `compas_fd-0.5.1/src/compas_fd/constraints/planeconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/src/compas_fd/constraints/surfaceconstraint.py` & `compas_fd-0.5.1/src/compas_fd/constraints/surfaceconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/src/compas_fd/constraints/vectorconstraint.py` & `compas_fd-0.5.1/src/compas_fd/constraints/vectorconstraint.py`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/src/compas_fd/loads/selfweight.py` & `compas_fd-0.5.1/src/compas_fd/loads/selfweight.py`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/src/compas_fd/solvers/__init__.py` & `compas_fd-0.5.1/src/compas_fd/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/src/compas_fd/solvers/fd_constrained_numpy.py` & `compas_fd-0.5.1/src/compas_fd/solvers/fd_constrained_numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,15 @@
         _solve_fd(numdata, selfweight)
         # this needs to be turned inside out
         # - associate vertices with constraint
         # - compute all projections in one step
         # - vectorize the computation of residuals
         # -
         _update_constraints(numdata, constraints, damping)
-        if _is_converged_residuals(numdata.tangent_residuals, tol_res) and _is_converged_disp(
-            xyz_prev, numdata.xyz, tol_disp
-        ):
+        if _is_converged_residuals(numdata.tangent_residuals, tol_res) and _is_converged_disp(xyz_prev, numdata.xyz, tol_disp):
             break
 
     _post_process_fd(numdata)
     return numdata.to_result()
 
 
 def _solve_fd(numdata: FDNumericalData, selfweight: Callable = None) -> None:
```

### Comparing `compas_fd-0.5.0/src/compas_fd/solvers/fd_numerical_data.py` & `compas_fd-0.5.1/src/compas_fd/solvers/fd_numerical_data.py`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/src/compas_fd/solvers/fd_numpy.py` & `compas_fd-0.5.1/src/compas_fd/solvers/fd_numpy.py`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/src/compas_fd/types.py` & `compas_fd-0.5.1/src/compas_fd/types.py`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/src/compas_fd.egg-info/SOURCES.txt` & `compas_fd-0.5.1/src/compas_fd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compas_fd-0.5.0/tests/test_selfweight.py` & `compas_fd-0.5.1/tests/test_selfweight.py`

 * *Files identical despite different names*

