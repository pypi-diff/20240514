# Comparing `tmp/pldag-0.8.1.tar.gz` & `tmp/pldag-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.8.1.tar", max compression
+gzip compressed data, was "pldag-0.8.2.tar", max compression
```

## Comparing `pldag-0.8.1.tar` & `pldag-0.8.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.8.1/LICENSE
--rw-r--r--   0        0        0     2833 2024-05-07 07:16:43.962166 pldag-0.8.1/README.md
--rw-r--r--   0        0        0    36409 2024-05-12 18:13:16.288613 pldag-0.8.1/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.8.1/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.8.1/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-05-12 18:29:15.546030 pldag-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.8.2/LICENSE
+-rw-r--r--   0        0        0     2833 2024-05-07 07:16:43.962166 pldag-0.8.2/README.md
+-rw-r--r--   0        0        0    38933 2024-05-14 12:33:16.562246 pldag-0.8.2/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.8.2/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.8.2/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-05-14 12:33:36.777304 pldag-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.8.2/PKG-INFO
```

### Comparing `pldag-0.8.1/LICENSE` & `pldag-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.8.1/README.md` & `pldag-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.8.1/pldag/__init__.py` & `pldag-0.8.2/pldag/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -322,14 +322,27 @@
                 filter(
                     lambda x: x[1] == id,
                     self._amap.items(),
                 )
             )
         )
     
+    def copy(self) -> "PLDAG":
+        """Copy the model"""
+        model = PLDAG()
+        model._amat = self._amat.copy()
+        model._wmat = self._wmat.copy()
+        model._dvec = self._dvec.copy()
+        model._bvec = self._bvec.copy()
+        model._nvec = self._nvec.copy()
+        model._cvec = self._cvec.copy()
+        model._imap = self._imap.copy()
+        model._amap = self._amap.copy()
+        return model
+    
     def get(self, *id: str) -> np.ndarray:
         """Get the bounds of the given ID(s)"""
         return self._dvec[list(map(self._col, id))]
     
     def delete(self, id: str) -> True:
         """
             Delete the given ID.
@@ -920,24 +933,30 @@
         sub_model = PLDAG()
         sub_model._amat = self._amat[row_idxs][:, col_idxs]
         sub_model._nvec = self._nvec[row_idxs]
         sub_model._dvec = self._dvec[col_idxs]
         sub_model._bvec = self._bvec[row_idxs]
         sub_model._cvec = self._cvec[col_idxs]
         sub_model._imap = dict(map(lambda x: (x[1], x[0]), enumerate(self._col_vars[col_idxs])))
+        sub_model._amap = dict(filter(lambda x: x[1] in sub_model._imap, self._amap.items()))
         return sub_model
     
-    def sub(self, ids: List[str]) -> 'PLDAG':
+    def sub(self, roots: List[str], max_iterations: int = 1000) -> 'PLDAG':
         """
-            Create a sub-PLDAG from the given IDs.
+            Create a sub-PLDAG from the given root IDs.
+            
+            NOTE: This function works recursively to find all roots that eventually will be reached from any of the id's in `ids`. 
+            Therefore we have a maximum number of iterations to avoid infinite loops.
 
             Parameters
             ----------
-            ids : List[str]
-                The IDs to include in the sub PLDAG.
+            roots : List[str]
+                The IDs to use as roots in the new sub PLDAG.
+
+            cuts : List[Dict]
 
             Examples
             --------
             >>> model = PLDAG()
             >>> model.set_primitives("xyz")
             >>> a = model.set_atleast("xyz", 1)
             >>> sub_model = model.sub_pldag(["x", "y"])
@@ -946,33 +965,83 @@
 
             Returns
             -------
             PLDAG
                 The sub-PLDAG.
         """
 
-        col_vars = self._col_vars.tolist()
-        row_vars = self._row_vars.tolist()
-
-        def incoming_edges(idlist: List[int]) -> Set[int]:
-            return set(self._col_vars[np.argwhere(self._amat[list(map(row_vars.index, filter(lambda v: v in row_vars, idlist)))]).T[1]].tolist())
-        
         # First find all variables (columns and rows)
-        # that eventually reaches any of the id's in `ids`
-        max_iterations: int = 100
-        matching_variables = incoming_edges(set(ids)).union(set(ids))
+        # that eventually reaches any of the roots
+        adj = self.adjacency_matrix
+        idxs = list(map(self._col, filter(lambda id: id in self._imap, roots)))
+        
+        # Init by setting the given nodes
+        match_vector = np.isin(range(adj.shape[1]), idxs)
+        match_vector[idxs] = True
+
+        # Find what nodes that are connected to the given nodes
+        previous_match_vector = (adj[match_vector] != 0).any(axis=0)
+
         for _ in range(max_iterations):
-            new_matching_variables = incoming_edges(matching_variables)
-            if new_matching_variables.issubset(matching_variables):
+
+            # Extend the match vector with new variables found
+            match_vector |= previous_match_vector
+            
+            # Query for new variables
+            previous_match_vector = (adj[previous_match_vector] != 0).any(axis=0)
+            
+            # If no new variables are found, this is the last root
+            if (~previous_match_vector).all():
                 break
-            matching_variables.update(new_matching_variables)
 
-        col_idxs = np.array(sorted(list(map(col_vars.index, matching_variables))))
-        row_idxs = np.array(sorted(list(map(row_vars.index, filter(lambda v: v in self._row_vars, matching_variables)))))
-        return self._from_indices(row_idxs, col_idxs)
+        return self._from_indices(
+            list(map(self._row, filter(lambda x: x in self.composites, self.columns[match_vector]))), 
+            np.argwhere(match_vector).T[0]
+        )
+    
+    def cut(self, cuts: Dict[str, str]) -> "PLDAG":
+
+        """
+            Cuts graph on given nodes in `cuts`. The key in cuts is what node to cut,
+            the value is the new ID of the node (since it will go from a composite to a primitive).
+
+            Note. Only connections to the given nodes in cuts will be cut. If the child nodes has
+            other connections to the graph, they will still be part of the graph.
+
+            Parameters
+            ----------
+            cuts : Dict[str, str]
+                A mapping of nodes to cut to their new IDs.
+
+            Returns
+            -------
+            PLDAG
+                The cut PLDAG.
+        """
+        ids = list(filter(lambda id: id in self.rows, cuts.keys()))
+        if len(ids) == 0:
+            return self.copy()
+        ex_roots = (self._amat == 0).all(axis=0)
+        idxs = list(map(self._row, ids))
+        a = self._amat.copy()
+        a[idxs] = 0
+        sub = self._from_indices(
+            col_idxs=np.argwhere((a != 0).any(axis=0) | ex_roots).T[0],
+            row_idxs=np.argwhere((a != 0).any(axis=1)).T[0],
+        )
+        sub._cvec[list(map(sub._col, ids))] = False
+        sub._amap = dict(filter(lambda x: x[1] not in ids, sub._amap.items()))
+        sub._imap = dict(map(lambda x: (cuts.get(x[0], x[0]), x[1]), sub._imap.items()))
+        return sub
+    
+    def cut_sub(self, cuts: Dict[str, str], roots: List[str]) -> "PLDAG":
+        """
+            Cuts graph on given nodes in `cuts` and then creates a sub graph from the given root IDs.
+        """
+        return self.cut(cuts).sub(roots)
     
     def solve(self, objectives: List[Dict[str, int]], assume: Dict[str, complex], solver: Solver) -> List[Dict[str, complex]]:
         """
             Solves the model with the given objectives.
 
             Parameters
             ----------
```

### Comparing `pldag-0.8.1/pldag/solver/glpk_solver.py` & `pldag-0.8.2/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.8.1/PKG-INFO` & `pldag-0.8.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.8.1
+Version: 0.8.2
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

