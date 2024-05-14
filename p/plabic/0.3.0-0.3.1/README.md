# Comparing `tmp/plabic-0.3.0.tar.gz` & `tmp/plabic-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plabic-0.3.0.tar", last modified: Fri Oct  6 15:22:23 2023, max compression
+gzip compressed data, was "plabic-0.3.1.tar", last modified: Tue May 14 21:27:46 2024, max compression
```

## Comparing `plabic-0.3.0.tar` & `plabic-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 15:22:23.566751 plabic-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-06 15:21:36.000000 plabic-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18776 2023-10-06 15:22:23.566751 plabic-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18087 2023-10-06 15:21:36.000000 plabic-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 15:22:23.562751 plabic-0.3.0/plabic/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-10-06 15:21:36.000000 plabic-0.3.0/plabic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42377 2023-10-06 15:21:36.000000 plabic-0.3.0/plabic/ba_permutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2023-10-06 15:21:36.000000 plabic-0.3.0/plabic/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8604 2023-10-06 15:21:36.000000 plabic-0.3.0/plabic/double_wiring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2023-10-06 15:21:36.000000 plabic-0.3.0/plabic/framed_2_disks.py
--rw-r--r--   0 runner    (1001) docker     (127)    31457 2023-10-06 15:21:36.000000 plabic-0.3.0/plabic/le_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)    81228 2023-10-06 15:21:36.000000 plabic-0.3.0/plabic/plabic_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)    13667 2023-10-06 15:21:36.000000 plabic-0.3.0/plabic/planar_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)    15473 2023-10-06 15:21:36.000000 plabic-0.3.0/plabic/triangulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 15:22:23.562751 plabic-0.3.0/plabic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18776 2023-10-06 15:22:23.000000 plabic-0.3.0/plabic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-10-06 15:22:23.000000 plabic-0.3.0/plabic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 15:22:23.000000 plabic-0.3.0/plabic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-06 15:22:23.000000 plabic-0.3.0/plabic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-06 15:21:36.000000 plabic-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 15:22:23.566751 plabic-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 15:22:23.566751 plabic-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12846 2023-10-06 15:21:36.000000 plabic-0.3.0/tests/test_ba_permutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2023-10-06 15:21:36.000000 plabic-0.3.0/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2023-10-06 15:21:36.000000 plabic-0.3.0/tests/test_double_wiring.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-06 15:21:36.000000 plabic-0.3.0/tests/test_framed_2_disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2023-10-06 15:21:36.000000 plabic-0.3.0/tests/test_le.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2023-10-06 15:21:36.000000 plabic-0.3.0/tests/test_plabic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2023-10-06 15:21:36.000000 plabic-0.3.0/tests/test_planar_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2023-10-06 15:21:36.000000 plabic-0.3.0/tests/test_triangulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:27:46.957536 plabic-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 21:27:23.000000 plabic-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19699 2024-05-14 21:27:46.957536 plabic-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19009 2024-05-14 21:27:23.000000 plabic-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:27:46.953536 plabic-0.3.1/plabic/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-14 21:27:23.000000 plabic-0.3.1/plabic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42798 2024-05-14 21:27:23.000000 plabic-0.3.1/plabic/ba_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-14 21:27:23.000000 plabic-0.3.1/plabic/bcfw_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-05-14 21:27:23.000000 plabic-0.3.1/plabic/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-05-14 21:27:24.000000 plabic-0.3.1/plabic/double_wiring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-14 21:27:24.000000 plabic-0.3.1/plabic/framed_2_disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31428 2024-05-14 21:27:24.000000 plabic-0.3.1/plabic/le_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81198 2024-05-14 21:27:24.000000 plabic-0.3.1/plabic/plabic_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13667 2024-05-14 21:27:24.000000 plabic-0.3.1/plabic/planar_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-05-14 21:27:24.000000 plabic-0.3.1/plabic/separated_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-14 21:27:24.000000 plabic-0.3.1/plabic/sym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19104 2024-05-14 21:27:24.000000 plabic-0.3.1/plabic/tnn_grassmannian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15444 2024-05-14 21:27:24.000000 plabic-0.3.1/plabic/triangulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:27:46.957536 plabic-0.3.1/plabic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19699 2024-05-14 21:27:46.000000 plabic-0.3.1/plabic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-14 21:27:46.000000 plabic-0.3.1/plabic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:27:46.000000 plabic-0.3.1/plabic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 21:27:46.000000 plabic-0.3.1/plabic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-14 21:27:24.000000 plabic-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:27:46.957536 plabic-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:27:46.957536 plabic-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-05-14 21:27:24.000000 plabic-0.3.1/tests/test_ba_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 21:27:24.000000 plabic-0.3.1/tests/test_bcfw_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-14 21:27:24.000000 plabic-0.3.1/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-14 21:27:24.000000 plabic-0.3.1/tests/test_double_wiring.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 21:27:24.000000 plabic-0.3.1/tests/test_framed_2_disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-14 21:27:24.000000 plabic-0.3.1/tests/test_le.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-14 21:27:24.000000 plabic-0.3.1/tests/test_plabic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-14 21:27:24.000000 plabic-0.3.1/tests/test_planar_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-14 21:27:24.000000 plabic-0.3.1/tests/test_separated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-14 21:27:24.000000 plabic-0.3.1/tests/test_tnn_grassmannian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-14 21:27:24.000000 plabic-0.3.1/tests/test_triangulation.py
```

### Comparing `plabic-0.3.0/LICENSE` & `plabic-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plabic-0.3.0/PKG-INFO` & `plabic-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: plabic
-Version: 0.3.0
-Summary: A package related to the cluster algebra and geometry related to plabic graphs
-Author-email: Ammar Husain <ammar.s.husain@gmail.com>
-Project-URL: Homepage, https://github.com/Cobord/Plabic
-Project-URL: Bug Tracker, https://github.com/Cobord/Plabic/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Plabic
 Cluster algebraic/geometric structures related to plabic graphs
 
 ## Requirements
 
 matplotlib, networkx, numpy, sympy
 
@@ -286,7 +270,23 @@
 
 In order to mutate specify the name of the vertex you wish to mutate at. The object changes my_quiver and cluster variables (simply called cluster) appropriately. The cluster variables are given as a dictionary
 so we can easily pick out the one corresponding to each vertex of the quiver.
 
 cluster_same compares the two clusters and can also be given an additional function which can do more simplification. This will be needed only if the simplifier in the Cluster initialization was too weak. 
 
 The draw method simply draws the underlying quiver.
+
+# TNN Grassmannian
+
+MinorSignConstraints allows one to specify which minors of a matrix are 0, positive, negative, etc.
+The minors are specified as which columns are selected from the matrix. The total number of columns is not fixed,
+just that it has to be at least some value for all the constraints to make sense.
+You can change the number of columns in your example, and the additional columns will be unconstrained.
+
+TNNGrassChart is where you actually work with the symbolic matrix representing a R_>0^d chart in Mat(k,n)
+You specify the names of the variables which are all treated as ranging over positive reals
+The constraints are imposed and we can enforce that all the sign constraints on minors are manifestly satisfied 
+
+# BCFW Cells
+
+[As described in this paper](https://arxiv.org/pdf/2402.15568.pdf "A cluster of results on amplitudehedron tiles")
+Uses the operad composition for the BCFW product operation.
```

### Comparing `plabic-0.3.0/README.md` & `plabic-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: plabic
+Version: 0.3.1
+Summary: A package related to the cluster algebra and geometry related to plabic graphs
+Author-email: Ammar Husain <ammar.s.husain@gmail.com>
+Project-URL: Homepage, https://github.com/Cobord/Plabic
+Project-URL: Bug Tracker, https://github.com/Cobord/Plabic/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Plabic
 Cluster algebraic/geometric structures related to plabic graphs
 
 ## Requirements
 
 matplotlib, networkx, numpy, sympy
 
@@ -270,7 +286,23 @@
 
 In order to mutate specify the name of the vertex you wish to mutate at. The object changes my_quiver and cluster variables (simply called cluster) appropriately. The cluster variables are given as a dictionary
 so we can easily pick out the one corresponding to each vertex of the quiver.
 
 cluster_same compares the two clusters and can also be given an additional function which can do more simplification. This will be needed only if the simplifier in the Cluster initialization was too weak. 
 
 The draw method simply draws the underlying quiver.
+
+# TNN Grassmannian
+
+MinorSignConstraints allows one to specify which minors of a matrix are 0, positive, negative, etc.
+The minors are specified as which columns are selected from the matrix. The total number of columns is not fixed,
+just that it has to be at least some value for all the constraints to make sense.
+You can change the number of columns in your example, and the additional columns will be unconstrained.
+
+TNNGrassChart is where you actually work with the symbolic matrix representing a R_>0^d chart in Mat(k,n)
+You specify the names of the variables which are all treated as ranging over positive reals
+The constraints are imposed and we can enforce that all the sign constraints on minors are manifestly satisfied 
+
+# BCFW Cells
+
+[As described in this paper](https://arxiv.org/pdf/2402.15568.pdf "A cluster of results on amplitudehedron tiles")
+Uses the operad composition for the BCFW product operation.
```

### Comparing `plabic-0.3.0/plabic/__init__.py` & `plabic-0.3.1/plabic/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 the relevant classes for external use 
 """
-#pylint:disable=import-error
 from .planar_diagram import PlanarNetwork,ChipType,determinant
 from .framed_2_disks import FramedDiskConfig
 from .plabic_diagram import BiColor,PlabicGraphBuilder,PlabicGraph,ExtraData
 from .le_diagram import LeDiagram
 from .double_wiring import WiringDiagram
 from .triangulation import Triangulation
 from .ba_permutation import AffinePermutation, BoundedAffinePermutation, ShiftEquivariantZBijection
 from .cluster import Cluster,cluster_same
+from .tnn_grassmannian import MinorSignConstraints,TNNGrassChart,ConvexHull
+from .bcfw_cell import BCFWCell, ButterflyData
```

### Comparing `plabic-0.3.0/plabic/ba_permutation.py` & `plabic-0.3.1/plabic/ba_permutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     return abs(a*b) // gcd(a, b)
 
 class ShiftEquivariantZBijection:
     """
     Common to all bijections of Z
     satisfying f(k+n) = f(k)+n for all k
     for some n
+    One can also think of these as
+    the invertible Hom(N,N) in the paracyclic category
+    N is either n,n+1 depending on notation
     """
     my_n : int
     my_f : Dict[int,int]
     is_lift_from_sn : bool
 
     # pylint:disable=too-many-locals
     def __init__(self,*,
@@ -694,24 +697,28 @@
 
         # check the condition on ij jumping self[i,j]<=other[i,j] for all i,j
         # on some pairs i,j
         for try_i,try_j in itertools.permutations(range(1,self.my_n+1),2):
             if len(self.ij_jumpers(try_i,try_j))>len(other.ij_jumpers(try_i,try_j)):
                 return False
         if self.is_lift_from_sn and other.is_lift_from_sn:
+            # the above pair check is conclusive for lifts from Sn
+            # so we can definitively conclude true in this case
             if known_leq_other is not None:
                 known_leq_other.add(self)
             if known_geq_self is not None:
                 known_geq_self.add(other)
             return True
         # couldn't prove not leq with the limited set of ij pairs we tried
-        # we need to work harder
+        # and it wasn't from Sn so that was not a conclusive yes they are leq
         if len(reduced_self)+1==len(reduced_other):
+            # try omitting a letter from reduced_other one by one
             raise NotImplementedError
 
+        # none of the easy strategies worked
         raise NotImplementedError
 
     def quot_to_sn(self) -> List[int]:
         """
         Forget down to the residues modulo self.my_n
         """
         return self.my_underlying.quot_to_sn()
```

### Comparing `plabic-0.3.0/plabic/cluster.py` & `plabic-0.3.1/plabic/cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from __future__ import annotations
 from typing import Callable, Optional, TypeVar,Protocol,\
     Generic,List,Dict,Tuple,Set
 from functools import reduce
 import networkx as nx
 import matplotlib.pyplot as plt
+from sympy import Expr, Integer, symbols
 
 T = TypeVar("T")
 
 class Arithmetic(Protocol):
     """
     can be multiplied, added, divided and powered
     that is enough to do all the cluster
@@ -164,7 +165,29 @@
         if not isinstance(other,Cluster):
             return False
         if list(self.my_quiver.nodes()) != list(other.my_quiver.nodes()):
             return False
         if not cluster_same(self.cluster,other.cluster):
             return False
         return self.my_antisymmetric() == other.my_antisymmetric()
+
+    @staticmethod
+    def make_type_an_cluster(my_n : int) -> Tuple[List[Expr],Cluster[Expr]]:
+        """
+        make the cluster for type An with sympy variables
+        """
+        if my_n<=0:
+            raise TypeError("n must be a natural number greater than 0")
+        variable_pool = ["a","b","c","d","x","y","z","w","v",
+                         "f","g","h","l","m","n","o",
+                         "p","q","r","s","t","u"]
+        if my_n>len(variable_pool):
+            raise ValueError(f"Only have {len(variable_pool)} variables available")
+        variables_used = variable_pool[0:my_n]
+        variable_list = list(symbols(",".join(variables_used),commutative=True))
+        my_an_quiver = nx.MultiDiGraph()
+        for cur_node in range(1,my_n+1):
+            my_an_quiver.add_node(str(cur_node))
+        for cur_node in range(1,my_n):
+            my_an_quiver.add_edge(str(cur_node),str(cur_node+1))
+        return_cluster = Cluster[Expr](my_an_quiver,variable_list,Integer(1),lambda z: z.simplify())
+        return variable_list, return_cluster
```

### Comparing `plabic-0.3.0/plabic/double_wiring.py` & `plabic-0.3.1/plabic/double_wiring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 double wiring diagram
 also include single wiring diagram
 """
 from __future__ import annotations
 from functools import reduce
 from typing import Tuple,List,Dict,Iterator,Set,Any,cast
-#pylint:disable=import-error
 from .plabic_diagram import PlabicGraph, BiColor
 from .ba_permutation import AffinePermutation
 
 Point = Tuple[float,float]
 
 class WiringDiagram:
     """
```

### Comparing `plabic-0.3.0/plabic/framed_2_disks.py` & `plabic-0.3.1/plabic/framed_2_disks.py`

 * *Files identical despite different names*

### Comparing `plabic-0.3.0/plabic/le_diagram.py` & `plabic-0.3.1/plabic/le_diagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Le Diagram
 """
 
 from enum import Enum, auto
 from typing import List, Optional, Tuple, Set, Iterable, Union, TypeVar, Dict, cast, Iterator
 import itertools
 
-#pylint:disable=import-error
 from .plabic_diagram import BiColor, ExtraData, PlabicGraph
 from .ba_permutation import AffinePermutation, BruhatInterval
 
 #pylint:disable=too-many-locals,too-many-statements,too-many-branches,too-many-return-statements,too-many-instance-attributes
 
 Point = Tuple[float, float]
```

### Comparing `plabic-0.3.0/plabic/plabic_diagram.py` & `plabic-0.3.1/plabic/plabic_diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import functools
 import numbers
 from math import sqrt
 from typing import Tuple, Optional, List, Dict, cast, Any, Callable, Set, Iterator
 import itertools
 import networkx as nx
 import matplotlib.pyplot as plt
-# pylint:disable=import-error
 from .framed_2_disks import FramedDiskConfig
 
 Point = Tuple[float,float]
 
 class BiColor(Enum):
     """
     the two colors for internal vertices
```

### Comparing `plabic-0.3.0/plabic/planar_diagram.py` & `plabic-0.3.1/plabic/planar_diagram.py`

 * *Files identical despite different names*

### Comparing `plabic-0.3.0/plabic/triangulation.py` & `plabic-0.3.1/plabic/triangulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Triangulation of convex m-gon
 """
 
 from typing import Tuple,Set,List,Union,cast,Dict,Any
 from functools import reduce
 import itertools
 from math import sin, cos, pi as PI, atan2, sqrt
-#pylint:disable=import-error
 from .plabic_diagram import PlabicGraph, BiColor
 from .framed_2_disks import FramedDiskConfig
 
 Point = Tuple[float,float]
 
 class Triangulation:
     """
```

### Comparing `plabic-0.3.0/plabic.egg-info/PKG-INFO` & `plabic-0.3.1/plabic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plabic
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package related to the cluster algebra and geometry related to plabic graphs
 Author-email: Ammar Husain <ammar.s.husain@gmail.com>
 Project-URL: Homepage, https://github.com/Cobord/Plabic
 Project-URL: Bug Tracker, https://github.com/Cobord/Plabic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -286,7 +286,23 @@
 
 In order to mutate specify the name of the vertex you wish to mutate at. The object changes my_quiver and cluster variables (simply called cluster) appropriately. The cluster variables are given as a dictionary
 so we can easily pick out the one corresponding to each vertex of the quiver.
 
 cluster_same compares the two clusters and can also be given an additional function which can do more simplification. This will be needed only if the simplifier in the Cluster initialization was too weak. 
 
 The draw method simply draws the underlying quiver.
+
+# TNN Grassmannian
+
+MinorSignConstraints allows one to specify which minors of a matrix are 0, positive, negative, etc.
+The minors are specified as which columns are selected from the matrix. The total number of columns is not fixed,
+just that it has to be at least some value for all the constraints to make sense.
+You can change the number of columns in your example, and the additional columns will be unconstrained.
+
+TNNGrassChart is where you actually work with the symbolic matrix representing a R_>0^d chart in Mat(k,n)
+You specify the names of the variables which are all treated as ranging over positive reals
+The constraints are imposed and we can enforce that all the sign constraints on minors are manifestly satisfied 
+
+# BCFW Cells
+
+[As described in this paper](https://arxiv.org/pdf/2402.15568.pdf "A cluster of results on amplitudehedron tiles")
+Uses the operad composition for the BCFW product operation.
```

### Comparing `plabic-0.3.0/plabic.egg-info/SOURCES.txt` & `plabic-0.3.1/plabic.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 LICENSE
 README.md
 pyproject.toml
 plabic/__init__.py
 plabic/ba_permutation.py
+plabic/bcfw_cell.py
 plabic/cluster.py
 plabic/double_wiring.py
 plabic/framed_2_disks.py
 plabic/le_diagram.py
 plabic/plabic_diagram.py
 plabic/planar_diagram.py
+plabic/separated_sets.py
+plabic/sym_utils.py
+plabic/tnn_grassmannian.py
 plabic/triangulation.py
 plabic.egg-info/PKG-INFO
 plabic.egg-info/SOURCES.txt
 plabic.egg-info/dependency_links.txt
 plabic.egg-info/top_level.txt
 tests/test_ba_permutation.py
+tests/test_bcfw_cell.py
 tests/test_cluster.py
 tests/test_double_wiring.py
 tests/test_framed_2_disks.py
 tests/test_le.py
 tests/test_plabic.py
 tests/test_planar_diagram.py
+tests/test_separated.py
+tests/test_tnn_grassmannian.py
 tests/test_triangulation.py
```

### Comparing `plabic-0.3.0/pyproject.toml` & `plabic-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "plabic"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Ammar Husain", email="ammar.s.husain@gmail.com" },
 ]
 description = "A package related to the cluster algebra and geometry related to plabic graphs"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `plabic-0.3.0/tests/test_ba_permutation.py` & `plabic-0.3.1/tests/test_ba_permutation.py`

 * *Files identical despite different names*

### Comparing `plabic-0.3.0/tests/test_cluster.py` & `plabic-0.3.1/tests/test_cluster.py`

 * *Files 23% similar despite different names*

```diff
@@ -41,14 +41,38 @@
     assert my_cluster_same(c.cluster,{"1":(B+1)/A,"2":(1+A+B)/(A*B)})
     c.mutate("1")
     c.mutate("2")
     c.mutate("1")
     assert np.array_equal(c.my_antisymmetric(),[[0,-1],[1,0]])
     assert my_cluster_same(c.cluster,{"1":B,"2":A})
 
+def test_make_a2():
+    """
+    a2 quiver with static method
+    """
+    #pylint:disable=invalid-name
+    ([A,B],c) = Cluster.make_type_an_cluster(2)
+    assert np.array_equal(c.my_antisymmetric(),[[0,1],[-1,0]])
+    assert my_cluster_same(c.cluster,{"1":A,"2":B})
+    c.mutate("1")
+    assert np.array_equal(c.my_antisymmetric(),[[0,-1],[1,0]])
+    assert my_cluster_same(c.cluster,{"1":(B+1)/A,"2":B})
+    c.mutate("1")
+    assert np.array_equal(c.my_antisymmetric(),[[0,1],[-1,0]])
+    assert my_cluster_same(c.cluster,{"1":A,"2":B})
+    c.mutate("1")
+    c.mutate("2")
+    assert np.array_equal(c.my_antisymmetric(),[[0,1],[-1,0]])
+    assert my_cluster_same(c.cluster,{"1":(B+1)/A,"2":(1+A+B)/(A*B)})
+    c.mutate("1")
+    c.mutate("2")
+    c.mutate("1")
+    assert np.array_equal(c.my_antisymmetric(),[[0,-1],[1,0]])
+    assert my_cluster_same(c.cluster,{"1":B,"2":A})
+
 def test_square():
     """
     affine a3 quiver
     """
     #pylint:disable=invalid-name
     A,B,C,D = symbols("a,b,c,d",commutative=True)
     my_aa3_quiver = nx.MultiDiGraph()
```

### Comparing `plabic-0.3.0/tests/test_double_wiring.py` & `plabic-0.3.1/tests/test_double_wiring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 test for double wiring diagrams
 """
-#pylint:disable=invalid-name,import-error
+#pylint:disable=invalid-name
 from typing import List
 from plabic import WiringDiagram
 
 def test_dw1() -> None:
     """
     sbar_2 s_1 s2 sbar_1 sbar_2 s1
     """
```

### Comparing `plabic-0.3.0/tests/test_le.py` & `plabic-0.3.1/tests/test_le.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 test Le diagrams
 """
 
-#pylint:disable=invalid-name,import-error
+#pylint:disable=invalid-name
 from typing import Set
 from plabic import LeDiagram
 
 def test_empty() -> None:
     """
     partition should be of positive number
     """
```

### Comparing `plabic-0.3.0/tests/test_plabic.py` & `plabic-0.3.1/tests/test_plabic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 test Plabic graphs
 """
-#pylint:disable=import-error,too-many-locals
+#pylint:disable=too-many-locals
 from typing import List,Dict
 from plabic import PlabicGraph,BiColor,PlabicGraphBuilder
 
 def test_plabic() -> None:
     """
     example from figure 7.1 of https://arxiv.org/pdf/2106.02160.pdf
     black there -> red here
```

### Comparing `plabic-0.3.0/tests/test_planar_diagram.py` & `plabic-0.3.1/tests/test_planar_diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 test planar diagrams
 """
-#pylint:disable=import-error,invalid-name,too-many-locals
+#pylint:disable=invalid-name,too-many-locals
 from typing import cast,List,Tuple
 from sympy import symbols, Symbol, Expr, Add, Mul, Pow, Integer, Rational, UnevaluatedExpr
 from plabic import PlanarNetwork, determinant, ChipType
 
 def test_planar() -> None:
     """
     example is taken from https://arxiv.org/pdf/math/9912128.pdf figure 1
```

### Comparing `plabic-0.3.0/tests/test_triangulation.py` & `plabic-0.3.1/tests/test_triangulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 test triangulations of convex m-gons
 """
-#pylint:disable=import-error,invalid-name,R0801
+#pylint:disable=invalid-name,R0801
 from math import pi as PI,sin,cos
 from plabic import Triangulation
 
 def test_octagon() -> None:
     """
     a triangulation of an octagon
     """
```

