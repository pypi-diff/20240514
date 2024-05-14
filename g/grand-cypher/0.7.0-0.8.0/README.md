# Comparing `tmp/grand-cypher-0.7.0.tar.gz` & `tmp/grand-cypher-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grand-cypher-0.7.0.tar", last modified: Sat May  4 14:00:17 2024, max compression
+gzip compressed data, was "grand-cypher-0.8.0.tar", last modified: Tue May 14 13:03:08 2024, max compression
```

## Comparing `grand-cypher-0.7.0.tar` & `grand-cypher-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-04 14:00:17.204058 grand-cypher-0.7.0/
--rw-r--r--   0 mateljk1   (501) staff       (20)    10173 2024-02-13 16:24:47.000000 grand-cypher-0.7.0/LICENSE
--rw-r--r--   0 mateljk1   (501) staff       (20)     4516 2024-05-04 14:00:17.203883 grand-cypher-0.7.0/PKG-INFO
--rw-r--r--   0 mateljk1   (501) staff       (20)     4125 2024-05-04 13:52:54.000000 grand-cypher-0.7.0/README.md
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-04 14:00:17.202916 grand-cypher-0.7.0/grand_cypher.egg-info/
--rw-r--r--   0 mateljk1   (501) staff       (20)     4516 2024-05-04 14:00:17.000000 grand-cypher-0.7.0/grand_cypher.egg-info/PKG-INFO
--rw-r--r--   0 mateljk1   (501) staff       (20)      284 2024-05-04 14:00:17.000000 grand-cypher-0.7.0/grand_cypher.egg-info/SOURCES.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)        1 2024-05-04 14:00:17.000000 grand-cypher-0.7.0/grand_cypher.egg-info/dependency_links.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)       30 2024-05-04 14:00:17.000000 grand-cypher-0.7.0/grand_cypher.egg-info/requires.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)       12 2024-05-04 14:00:17.000000 grand-cypher-0.7.0/grand_cypher.egg-info/top_level.txt
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-04 14:00:17.203561 grand-cypher-0.7.0/grandcypher/
--rw-r--r--   0 mateljk1   (501) staff       (20)    30112 2024-05-04 13:59:06.000000 grand-cypher-0.7.0/grandcypher/__init__.py
--rw-r--r--   0 mateljk1   (501) staff       (20)      531 2024-02-13 16:24:47.000000 grand-cypher-0.7.0/grandcypher/test_parser.py
--rw-r--r--   0 mateljk1   (501) staff       (20)    40941 2024-05-04 13:52:54.000000 grand-cypher-0.7.0/grandcypher/test_queries.py
--rw-r--r--   0 mateljk1   (501) staff       (20)       38 2024-05-04 14:00:17.204128 grand-cypher-0.7.0/setup.cfg
--rw-r--r--   0 mateljk1   (501) staff       (20)      701 2024-05-04 13:59:22.000000 grand-cypher-0.7.0/setup.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-14 13:03:08.710613 grand-cypher-0.8.0/
+-rw-r--r--   0 mateljk1   (501) staff       (20)    10173 2024-02-13 16:24:47.000000 grand-cypher-0.8.0/LICENSE
+-rw-r--r--   0 mateljk1   (501) staff       (20)     4516 2024-05-14 13:03:08.710500 grand-cypher-0.8.0/PKG-INFO
+-rw-r--r--   0 mateljk1   (501) staff       (20)     4125 2024-05-04 13:52:54.000000 grand-cypher-0.8.0/README.md
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-14 13:03:08.709506 grand-cypher-0.8.0/grand_cypher.egg-info/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     4516 2024-05-14 13:03:08.000000 grand-cypher-0.8.0/grand_cypher.egg-info/PKG-INFO
+-rw-r--r--   0 mateljk1   (501) staff       (20)      284 2024-05-14 13:03:08.000000 grand-cypher-0.8.0/grand_cypher.egg-info/SOURCES.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)        1 2024-05-14 13:03:08.000000 grand-cypher-0.8.0/grand_cypher.egg-info/dependency_links.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)       30 2024-05-14 13:03:08.000000 grand-cypher-0.8.0/grand_cypher.egg-info/requires.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)       12 2024-05-14 13:03:08.000000 grand-cypher-0.8.0/grand_cypher.egg-info/top_level.txt
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-14 13:03:08.710179 grand-cypher-0.8.0/grandcypher/
+-rw-r--r--   0 mateljk1   (501) staff       (20)    33862 2024-05-14 13:01:38.000000 grand-cypher-0.8.0/grandcypher/__init__.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)      531 2024-02-13 16:24:47.000000 grand-cypher-0.8.0/grandcypher/test_parser.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    46192 2024-05-14 13:01:07.000000 grand-cypher-0.8.0/grandcypher/test_queries.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)       38 2024-05-14 13:03:08.710704 grand-cypher-0.8.0/setup.cfg
+-rw-r--r--   0 mateljk1   (501) staff       (20)      701 2024-05-14 13:01:27.000000 grand-cypher-0.8.0/setup.py
```

### Comparing `grand-cypher-0.7.0/LICENSE` & `grand-cypher-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grand-cypher-0.7.0/PKG-INFO` & `grand-cypher-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grand-cypher
-Version: 0.7.0
+Version: 0.8.0
 Summary: Query Grand graphs using Cypher
 Home-page: https://github.com/aplbrain/grandcypher
 Author: Jordan Matelsky
 Author-email: opensource@matelsky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `grand-cypher-0.7.0/README.md` & `grand-cypher-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `grand-cypher-0.7.0/grand_cypher.egg-info/PKG-INFO` & `grand-cypher-0.8.0/grand_cypher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grand-cypher
-Version: 0.7.0
+Version: 0.8.0
 Summary: Query Grand graphs using Cypher
 Home-page: https://github.com/aplbrain/grandcypher
 Author: Jordan Matelsky
 Author-email: opensource@matelsky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `grand-cypher-0.7.0/grandcypher/__init__.py` & `grand-cypher-0.8.0/grandcypher/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 You can use this tool to search Python graph data-structures by
 data/attribute or by structure, using the same language you'd use
 to search in a much larger graph database.
 
 """
 
-from typing import Dict, List, Callable, Tuple
+from typing import Dict, List, Callable, Tuple, Union
 from collections import OrderedDict
 import random
 import string
 from functools import lru_cache
 import networkx as nx
 
 import grandiso
@@ -115,15 +115,14 @@
                     | LEFT_ANGLE? "-[" CNAME "*" MIN_HOP  ".." MAX_HOP "]-" RIGHT_ANGLE?
                     | LEFT_ANGLE? "-[" ":" TYPE "*" MIN_HOP "]-" RIGHT_ANGLE?
                     | LEFT_ANGLE? "-[" ":" TYPE "*" MIN_HOP  ".." MAX_HOP "]-" RIGHT_ANGLE?
                     | LEFT_ANGLE? "-[" CNAME ":" TYPE "*" MIN_HOP "]-" RIGHT_ANGLE?
                     | LEFT_ANGLE? "-[" CNAME ":" TYPE "*" MIN_HOP  ".." MAX_HOP "]-" RIGHT_ANGLE?
 
 
-
 LEFT_ANGLE          : "<"
 RIGHT_ANGLE         : ">"
 EQUAL               : "="
 MIN_HOP             : INT
 MAX_HOP             : INT
 TYPE                : CNAME
 
@@ -151,15 +150,15 @@
 COMMENT: "//" /[^\n]/*
 %ignore COMMENT
 
 """,
     start="start",
 )
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 
 _ALPHABET = string.ascii_lowercase + string.digits
 
 
 def shortuuid(k=4) -> str:
     return "".join(random.choices(_ALPHABET, k=k))
@@ -194,48 +193,81 @@
             return False
 
     return True
 
 
 @lru_cache()
 def _is_edge_attr_match(
-    motif_edge_id: Tuple[str, str],
-    host_edge_id: Tuple[str, str],
-    motif: nx.Graph,
-    host: nx.Graph,
+    motif_edge_id: Tuple[str, str, Union[int, str]],
+    host_edge_id: Tuple[str, str, Union[int, str]],
+    motif: Union[nx.Graph, nx.MultiDiGraph],
+    host: Union[nx.Graph, nx.MultiDiGraph],
 ) -> bool:
     """
-    Check if an edge in the host graph matches the attributes in the motif.
-    This also check the __labels__ of edges.
+    Check if an edge in the host graph matches the attributes in the motif,
+    including the special '__labels__' set attribute.
+    This function formats edges into
+    nx.MultiDiGraph format i.e {0: first_relation, 1: ...}.
 
     Arguments:
         motif_edge_id (str): The motif edge ID
         host_edge_id (str): The host edge ID
         motif (nx.Graph): The motif graph
         host (nx.Graph): The host graph
 
     Returns:
         bool: True if the host edge matches the attributes in the motif
-
     """
-    motif_edge = motif.edges[motif_edge_id]
-    host_edge = host.edges[host_edge_id]
+    motif_u, motif_v = motif_edge_id
+    host_u, host_v = host_edge_id
+
+    # Format edges for both DiGraph and MultiDiGraph
+    motif_edges = _get_edge_attributes(motif, motif_u, motif_v)
+    host_edges = _get_edge_attributes(host, host_u, host_v)
+
+    # Aggregate all __labels__ into one set
+    motif_edges = _aggregate_edge_labels(motif_edges)
+    host_edges = _aggregate_edge_labels(host_edges)
 
-    for attr, val in motif_edge.items():
+    for attr, val in motif_edges.items():
         if attr == "__labels__":
-            if val and val - host_edge.get("__labels__", set()):
+            if val and val - host_edges.get("__labels__", set()):
                 return False
             continue
-        if host_edge.get(attr) != val:
+        if host_edges.get(attr) != val:
             return False
 
     return True
 
 
-def _get_entity_from_host(host: nx.DiGraph, entity_name, entity_attribute=None):
+def _get_edge_attributes(graph: Union[nx.Graph, nx.MultiDiGraph], u, v) -> Dict:
+    """
+    Retrieve edge attributes from a graph, handling both Graph and MultiDiGraph.
+    """
+    if isinstance(graph, nx.MultiDiGraph):
+        return graph[u][v]
+    return {0: graph[u][v]}  # Mock single edge for DiGraph
+
+
+def _aggregate_edge_labels(edges: Dict) -> Dict:
+    """
+    Aggregate '__labels__' attributes from edges into a single set.
+    """
+    aggregated = {"__labels__": set()}
+    for edge_id, attrs in edges.items():
+        if "__labels__" in attrs and attrs["__labels__"]:
+            aggregated["__labels__"].update(attrs["__labels__"])
+        elif "__labels__" not in attrs:
+            aggregated[edge_id] = attrs
+    return aggregated
+
+
+def _get_entity_from_host(
+    host: Union[nx.DiGraph, nx.MultiDiGraph], entity_name, entity_attribute=None
+):
     if entity_name in host.nodes():
         # We are looking for a node mapping in the target graph:
         if entity_attribute:
             # Get the correct entity from the target host graph,
             # and then return the attribute:
             return host.nodes[entity_name].get(entity_attribute, None)
         else:
@@ -244,15 +276,18 @@
     else:
         # looking for an edge:
         edge_data = host.get_edge_data(*entity_name)
         if not edge_data:
             return None  # print(f"Nothing found for {entity_name} {entity_attribute}")
         if entity_attribute:
             # looking for edge attribute:
-            return edge_data.get(entity_attribute, None)
+            if isinstance(host, nx.MultiDiGraph):
+                return [r.get(entity_attribute, None) for r in edge_data.values()]
+            else:
+                return edge_data.get(entity_attribute, None)
         else:
             return host.get_edge_data(*entity_name)
 
 
 def _get_edge(host: nx.DiGraph, mapping, match_path, u, v):
     edge_path = match_path[(u, v)]
     return [
@@ -275,26 +310,34 @@
     def inner(match: dict, host: nx.DiGraph, return_endges: list) -> bool:
         return cond_a(match, host, return_endges) or cond_b(match, host, return_endges)
 
     return inner
 
 
 def cond_(should_be, entity_id, operator, value) -> CONDITION:
-    def inner(match: dict, host: nx.DiGraph, return_endges: list) -> bool:
+    def inner(
+        match: dict, host: Union[nx.DiGraph, nx.MultiDiGraph], return_endges: list
+    ) -> bool:
         host_entity_id = entity_id.split(".")
         if host_entity_id[0] in match:
             host_entity_id[0] = match[host_entity_id[0]]
         elif host_entity_id[0] in return_endges:
             # looking for edge...
             edge_mapping = return_endges[host_entity_id[0]]
             host_entity_id[0] = (match[edge_mapping[0]], match[edge_mapping[1]])
         else:
             raise IndexError(f"Entity {host_entity_id} not in graph.")
         try:
-            val = operator(_get_entity_from_host(host, *host_entity_id), value)
+            if isinstance(host, nx.MultiDiGraph):
+                # if any of the relations between nodes satisfies condition, return True
+                r_vals = _get_entity_from_host(host, *host_entity_id)
+                val = any(operator(r_val, value) for r_val in r_vals)
+            else:
+                val = operator(_get_entity_from_host(host, *host_entity_id), value)
+
         except:
             val = False
         if val != should_be:
             return False
         return True
 
     return inner
@@ -319,15 +362,15 @@
 
 
 class _GrandCypherTransformer(Transformer):
     def __init__(self, target_graph: nx.Graph, limit=None):
         self._target_graph = target_graph
         self._paths = []
         self._where_condition: CONDITION = None
-        self._motif = nx.DiGraph()
+        self._motif = nx.MultiDiGraph()
         self._matches = None
         self._matche_paths = None
         self._return_requests = []
         self._return_edges = {}
         self._distinct = False
         self._order_by = None
         self._order_by_attributes = set()
@@ -339,15 +382,19 @@
         if not data_paths:
             return {}
 
         motif_nodes = self._motif.nodes()
 
         for data_path in data_paths:
             entity_name, _ = _data_path_to_entity_name_attribute(data_path)
-            if entity_name not in motif_nodes and entity_name not in self._return_edges and entity_name not in self._paths:
+            if (
+                entity_name not in motif_nodes
+                and entity_name not in self._return_edges
+                and entity_name not in self._paths
+            ):
                 raise NotImplementedError(f"Unknown entity name: {data_path}")
 
         result = {}
         true_matches = self._get_true_matches()
 
         for data_path in data_paths:
             entity_name, entity_attribute = _data_path_to_entity_name_attribute(
@@ -371,63 +418,98 @@
             elif entity_name in self._paths:
                 ret = []
                 for mapping, _ in true_matches:
                     path, nodes = [], list(mapping.values())
                     for x, node in enumerate(nodes):
                         # Edge
                         if x > 0:
-                            path.append(self._target_graph.get_edge_data(nodes[x - 1], node))
+                            path.append(
+                                self._target_graph.get_edge_data(nodes[x - 1], node)
+                            )
 
                         # Node
                         path.append(node)
 
                     ret.append(path)
 
             else:
-                mapping_u, mapping_v = self._return_edges[data_path]
+                mapping_u, mapping_v = self._return_edges[data_path.split(".")[0]]
                 # We are looking for an edge mapping in the target graph:
-                is_hop = self._motif.edges[(mapping_u, mapping_v)]["__is_hop__"]
+                is_hop = self._motif.edges[(mapping_u, mapping_v, 0)]["__is_hop__"]
                 ret = (
                     _get_edge(
                         self._target_graph, mapping, match_path, mapping_u, mapping_v
                     )
                     for mapping, match_path in true_matches
                 )
                 ret = (r[0] if is_hop else r for r in ret)
                 # we keep the original list if len > 2 (edge hop 2+)
 
+                # Get all edge labels from the motif -- this is used to filter the relations for multigraphs
+                motif_edge_labels = set()
+                for edge in self._motif.get_edge_data(mapping_u, mapping_v).values():
+                    if edge.get("__labels__", None):
+                        motif_edge_labels.update(edge["__labels__"])
+
                 if entity_attribute:
                     # Get the correct entity from the target host graph,
                     # and then return the attribute:
-                    ret = (r.get(entity_attribute, None) for r in ret)
+                    if (
+                        isinstance(self._motif, nx.MultiDiGraph)
+                        and len(motif_edge_labels) > 0
+                    ):
+                        # filter the retrieved edge(s) based on the motif edge labels
+                        filtered_ret = []
+                        for r in ret:
+
+                            if any(
+                                [
+                                    i.get("__labels__", None).issubset(
+                                        motif_edge_labels
+                                    )
+                                    for i in r.values()
+                                ]
+                            ):
+                                filtered_ret.append(r)
+
+                        ret = filtered_ret
+
+                    # get the attribute from the retrieved edge(s)
+                    ret_with_attr = []
+                    for r in ret:
+                        r_attr = {}
+                        for i, v in r.items():
+                            r_attr[i] = v.get(entity_attribute, None)
+                        ret_with_attr.append(r_attr)
+
+                    ret = ret_with_attr
 
             result[data_path] = list(ret)[offset_limit]
 
         return result
-    
-    def return_clause(self, clause):        
+
+    def return_clause(self, clause):
         # collect all entity identifiers to be returned
         for item in clause:
             if item:
                 if not isinstance(item, str):
                     item = str(item.value)
                 self._return_requests.append(item)
 
-
     def order_clause(self, order_clause):
         self._order_by = []
         for item in order_clause[0].children:
             field = str(item.children[0])  # assuming the field name is the first child
             # Default to 'ASC' if not specified
-            if len(item.children) > 1 and str(item.children[1].data).lower() != 'desc':
-                direction = 'ASC'
+            if len(item.children) > 1 and str(item.children[1].data).lower() != "desc":
+                direction = "ASC"
             else:
-                direction = 'DESC'
-            
-            self._order_by.append((field, direction))   # [('n.age', 'DESC'), ...]
+                direction = "DESC"
+
+            self._order_by.append((field, direction))  # [('n.age', 'DESC'), ...]
             self._order_by_attributes.add(field)
 
     def distinct_return(self, distinct):
         self._distinct = True
 
     def limit_clause(self, limit):
         limit = int(limit[-1])
@@ -436,83 +518,104 @@
     def skip_clause(self, skip):
         skip = int(skip[-1])
         self._skip = skip
 
     def returns(self, ignore_limit=False):
 
         results = self._lookup(
-            self._return_requests + list(self._order_by_attributes), 
-            offset_limit=slice(0, None)
+            self._return_requests + list(self._order_by_attributes),
+            offset_limit=slice(0, None),
         )
         if self._order_by:
             results = self._apply_order_by(results)
         if self._distinct:
             results = self._apply_distinct(results)
         results = self._apply_pagination(results, ignore_limit)
 
-
         # Exclude order-by-only attributes from the final results
         results = {
-            key: values for key, values in results.items() if key in self._return_requests
+            key: values
+            for key, values in results.items()
+            if key in self._return_requests
         }
 
         return results
-    
+
     def _apply_order_by(self, results):
         if self._order_by:
-            sort_lists = [(results[field], direction) for field, direction in self._order_by if field in results]
+            sort_lists = [
+                (results[field], direction)
+                for field, direction in self._order_by
+                if field in results
+            ]
 
             if sort_lists:
                 # Generate a list of indices sorted by the specified fields
-                indices = range(len(next(iter(results.values()))))  # Safe because all lists are assumed to be of the same length
-                for sort_list, direction in reversed(sort_lists):  # reverse to ensure the first sort key is primary
-                    indices = sorted(indices, key=lambda i: sort_list[i], reverse=(direction == 'DESC'))
+                indices = range(
+                    len(next(iter(results.values())))
+                )  # Safe because all lists are assumed to be of the same length
+                for sort_list, direction in reversed(
+                    sort_lists
+                ):  # reverse to ensure the first sort key is primary
+                    indices = sorted(
+                        indices,
+                        key=lambda i: sort_list[i],
+                        reverse=(direction == "DESC"),
+                    )
 
                 # Reorder all lists in results using sorted indices
                 for key in results:
                     results[key] = [results[key][i] for i in indices]
-        
+
         return results
-    
+
     def _apply_distinct(self, results):
         if self._order_by:
-            assert self._order_by_attributes.issubset(self._return_requests), "In a WITH/RETURN with DISTINCT or an aggregation, it is not possible to access variables declared before the WITH/RETURN"
+            assert self._order_by_attributes.issubset(
+                self._return_requests
+            ), "In a WITH/RETURN with DISTINCT or an aggregation, it is not possible to access variables declared before the WITH/RETURN"
 
         # ordered dict to maintain the first occurrence of each unique tuple based on return requests
         unique_rows = OrderedDict()
-        
+
         # Iterate over each 'row' by index
-        for i in range(len(next(iter(results.values())))):  # assume all columns are of the same length
+        for i in range(
+            len(next(iter(results.values())))
+        ):  # assume all columns are of the same length
             # create a tuple key of all the values from return requests for this row
-            row_key = tuple(results[key][i] for key in self._return_requests if key in results)
-            
+            row_key = tuple(
+                results[key][i] for key in self._return_requests if key in results
+            )
+
             if row_key not in unique_rows:
-                unique_rows[row_key] = i  # store the index of the first occurrence of this unique row
-        
+                unique_rows[row_key] = (
+                    i  # store the index of the first occurrence of this unique row
+                )
+
         # construct the results based on unique indices collected
         distinct_results = {key: [] for key in self._return_requests}
         for row_key, index in unique_rows.items():
             for _, key in enumerate(self._return_requests):
                 distinct_results[key].append(results[key][index])
-        
+
         return distinct_results
-    
+
     def _apply_pagination(self, results, ignore_limit):
         # apply LIMIT and SKIP (if set) after ordering
         if self._limit is not None and not ignore_limit:
             start_index = self._skip
             end_index = start_index + self._limit
             for key in results.keys():
                 results[key] = results[key][start_index:end_index]
         # else just apply SKIP (if set)
         else:
             for key in results.keys():
                 start_index = self._skip
                 results[key] = results[key][start_index:]
-        
+
         return results
 
     def _get_true_matches(self):
         if not self._matches:
             self_matches = []
             self_matche_paths = []
             complete = False
@@ -602,49 +705,49 @@
             # Yield cartesian product
             yield from join
 
     def _is_limit(self, count):
         # Check if limit reached
         return self._limit and count >= (self._limit + self._skip)
 
-    def _edge_hop_motifs(self, motif: nx.DiGraph) -> List[Tuple[nx.Graph, dict]]:
+    def _edge_hop_motifs(self, motif: nx.MultiDiGraph) -> List[Tuple[nx.Graph, dict]]:
         """generate a list of edge-hop-expanded motif with edge-hop-map.
 
         Arguments:
             motif (nx.Graph): The motif graph
 
         Returns:
             List[Tuple[nx.Graph, dict]]: list of motif and edge-hop-map. \
                 edge-hop-map is a mapping from an edge to a real edge path
                 where a real edge path can have more than 2 element (hop >= 2)
                 or it can have 2 same element (hop = 0).
         """
-        new_motif = nx.DiGraph()
+        new_motif = nx.MultiDiGraph()
         for n in motif.nodes:
             if motif.out_degree(n) == 0 and motif.in_degree(n) == 0:
                 new_motif.add_node(n, **motif.nodes[n])
         motifs: List[Tuple[nx.DiGraph, dict]] = [(new_motif, {})]
-        for u, v in motif.edges:
+        for u, v, k in motif.edges:  # OutMultiEdgeView([('a', 'b', 0)])
             new_motifs = []
-            min_hop = motif.edges[u, v]["__min_hop__"]
-            max_hop = motif.edges[u, v]["__max_hop__"]
-            edge_type = motif.edges[u, v]["__labels__"]
+            min_hop = motif.edges[u, v, k]["__min_hop__"]
+            max_hop = motif.edges[u, v, k]["__max_hop__"]
+            edge_type = motif.edges[u, v, k]["__labels__"]
             hops = []
             if min_hop == 0:
-                new_motif = nx.DiGraph()
+                new_motif = nx.MultiDiGraph()
                 new_motif.add_node(u, **motif.nodes[u])
                 new_motifs.append((new_motif, {(u, v): (u, u)}))
             elif min_hop >= 1:
                 for _ in range(1, min_hop):
                     hops.append(shortuuid())
             for _ in range(max(min_hop, 1), max_hop):
                 new_edges = [u] + hops + [v]
-                new_motif = nx.DiGraph()
+                new_motif = nx.MultiDiGraph()
                 new_motif.add_edges_from(
-                    list(zip(new_edges[:-1], new_edges[1:])), __labels__=edge_type
+                    zip(new_edges, new_edges[1:]), __labels__=edge_type
                 )
                 new_motif.add_node(u, **motif.nodes[u])
                 new_motif.add_node(v, **motif.nodes[v])
                 new_motifs.append((new_motif, {(u, v): tuple(new_edges)}))
                 hops.append(shortuuid())
             motifs = self._product_motifs(motifs, new_motifs)
         return motifs
```

### Comparing `grand-cypher-0.7.0/grandcypher/test_parser.py` & `grand-cypher-0.8.0/grandcypher/test_parser.py`

 * *Files identical despite different names*

### Comparing `grand-cypher-0.7.0/grandcypher/test_queries.py` & `grand-cypher-0.8.0/grandcypher/test_queries.py`

 * *Files 15% similar despite different names*

```diff
@@ -821,14 +821,137 @@
         MATCH (n)
         RETURN n.name ORDER BY n.age ASC
         """
         res = GrandCypher(host).run(qry)
         assert res["n.name"] == ["Carol", "Alice", "Bob"]
 
 
+class TestMultigraphRelations:
+    def test_query_with_multiple_relations(self):
+        host = nx.MultiDiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_node("c", name="Charlie", age=25)
+        host.add_node("d", name="Diana", age=25)
+
+        # Adding edges with labels for different types of relationship_type
+        host.add_edge("a", "b", __labels__={"friends"})
+        host.add_edge("a", "b", __labels__={"colleagues"})
+        host.add_edge("a", "c", __labels__={"colleagues"})
+        host.add_edge("b", "d", __labels__={"family"})
+        host.add_edge("c", "d", __labels__={"family"})
+        host.add_edge("c", "d", __labels__={"friends"})
+        host.add_edge("d", "a", __labels__={"friends"})
+        host.add_edge("d", "a", __labels__={"colleagues"})
+
+        qry = """
+        MATCH (n)-[r:friends]->(m)
+        RETURN n.name, m.name
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["n.name"] == ['Alice', 'Charlie', 'Diana']
+        assert res["m.name"] == ['Bob', 'Diana', 'Alice']
+
+    def test_multiple_edges_specific_attribute(self):
+        host = nx.MultiDiGraph()
+        host.add_node("a", name="Alice", age=30)
+        host.add_node("b", name="Bob", age=30)
+        host.add_edge("a", "b", __labels__={"colleague"}, years=3)
+        host.add_edge("a", "b", __labels__={"friend"}, years=5)
+        host.add_edge("a", "b", __labels__={"enemy"}, hatred=10)
+
+        qry = """
+        MATCH (a)-[r:friend]->(b)
+        RETURN a.name, b.name, r.years
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["a.name"] == ["Alice"]
+        assert res["b.name"] == ["Bob"]
+        assert res["r.years"] == [{0: 3, 1: 5, 2: None}]   # should return None when attr is missing
+
+    def test_edge_directionality(self):
+        host = nx.MultiDiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_edge("a", "b", __labels__={"friend"}, years=1)
+        host.add_edge("b", "a", __labels__={"colleague"}, years=2)
+        host.add_edge("b", "a", __labels__={"mentor"}, years=4)
+
+        qry = """
+        MATCH (a)-[r]->(b)
+        RETURN a.name, b.name, r.__labels__, r.years
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["a.name"] == ["Alice", "Bob"]
+        assert res["b.name"] == ["Bob", "Alice"]
+        assert res["r.__labels__"] == [{0: {'friend'}}, {0: {'colleague'}, 1: {'mentor'}}]
+        assert res["r.years"] == [{0: 1}, {0: 2, 1: 4}]
+
+
+    def test_query_with_missing_edge_attribute(self):
+        host = nx.MultiDiGraph()
+        host.add_node("a", name="Alice", age=30)
+        host.add_node("b", name="Bob", age=40)
+        host.add_node("c", name="Charlie", age=50)
+        host.add_edge("a", "b", __labels__={"friend"}, years=3)
+        host.add_edge("a", "c", __labels__={"colleague"}, years=10)
+        host.add_edge("b", "c", __labels__={"colleague"}, duration=10)
+        host.add_edge("b", "c", __labels__={"mentor"}, years=2)
+
+        qry = """
+        MATCH (a)-[r:colleague]->(b)
+        RETURN a.name, b.name, r.duration
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["a.name"] == ["Alice", "Bob"]
+        assert res["b.name"] == ["Charlie", "Charlie"]
+        assert res["r.duration"] == [{0: None}, {0: 10, 1: None}]   # should return None when attr is missing
+
+        qry = """
+        MATCH (a)-[r:colleague]->(b)
+        RETURN a.name, b.name, r.years
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["a.name"] == ["Alice", "Bob"]
+        assert res["b.name"] == ["Charlie", "Charlie"]
+        assert res["r.years"] == [{0: 10}, {0: None, 1: 2}]
+
+        qry = """
+        MATCH (a)-[r]->(b)
+        RETURN a.name, b.name, r.__labels__, r.duration
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["a.name"] == ['Alice', 'Alice', 'Bob']
+        assert res["b.name"] == ['Bob', 'Charlie', 'Charlie']
+        assert res["r.__labels__"] == [{0: {'friend'}}, {0: {'colleague'}}, {0: {'colleague'}, 1: {'mentor'}}]
+        assert res["r.duration"] == [{0: None}, {0: None}, {0: 10, 1: None}]
+
+    def test_multigraph_single_edge_where(self):
+        host = nx.MultiDiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_node("c", name="Christine", age=30)
+        host.add_edge("a", "b", __labels__={"friend"}, years=1, friendly="very")
+        host.add_edge("b", "a", __labels__={"colleague"}, years=2)
+        host.add_edge("b", "a", __labels__={"mentor"}, years=4)
+        host.add_edge("b", "c", __labels__={"chef"}, years=12)
+
+        qry = """
+        MATCH (a)-[r]->(b)
+        WHERE r.friendly == "very" OR r.years == 2
+        RETURN a.name, b.name, r.__labels__, r.years, r.friendly
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["a.name"] == ["Alice", "Bob"]
+        assert res["b.name"] == ["Bob", "Alice"]
+        assert res["r.__labels__"] == [{0: {'friend'}}, {0: {'colleague'}, 1: {'mentor'}}]
+        assert res["r.years"] == [{0: 1}, {0: 2, 1: 4}]
+        assert res["r.friendly"] == [{0: 'very'}, {0: None, 1: None}]
+
+
 class TestVariableLengthRelationship:
     def test_single_variable_length_relationship(self):
         host = nx.DiGraph()
         host.add_node("x", foo=12)
         host.add_node("y", foo=13)
         host.add_node("z", foo=16)
         host.add_edge("x", "y", bar="1")
```

### Comparing `grand-cypher-0.7.0/setup.py` & `grand-cypher-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="grand-cypher",
-    version="0.7.0",
+    version="0.8.0",
     author="Jordan Matelsky",
     author_email="opensource@matelsky.com",
     description="Query Grand graphs using Cypher",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aplbrain/grandcypher",
     packages=setuptools.find_packages(),
```

