# Comparing `tmp/reasoner_validator-4.1.6.tar.gz` & `tmp/reasoner_validator-4.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.1.6.tar", max compression
+gzip compressed data, was "reasoner_validator-4.1.7.tar", max compression
```

## Comparing `reasoner_validator-4.1.6.tar` & `reasoner_validator-4.1.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1153 2024-05-10 19:15:12.963004 reasoner_validator-4.1.6/LICENSE
--rw-r--r--   0        0        0    13727 2024-05-10 19:15:12.963004 reasoner_validator-4.1.6/README.md
--rw-r--r--   0        0        0      131 2024-05-10 19:15:12.963004 reasoner_validator-4.1.6/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/docs/conf.py
--rw-r--r--   0        0        0    20564 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/docs/index.rst
--rw-r--r--   0        0        0      795 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/docs/make.bat
--rw-r--r--   0        0        0      136 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    43219 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2298 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    94743 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    47100 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/github.py
--rw-r--r--   0        0        0     3973 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/message.py
--rw-r--r--   0        0        0    46754 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    15057 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14745 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    38176 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/validator.py
--rw-r--r--   0        0        0    12127 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      866 2024-05-10 19:15:12.967004 reasoner_validator-4.1.6/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     3601 2024-05-10 19:15:12.971004 reasoner_validator-4.1.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 19:15:12.971004 reasoner_validator-4.1.6/tests/conftest.py
--rw-r--r--   0        0        0   149401 2024-05-10 19:15:12.971004 reasoner_validator-4.1.6/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-05-10 19:15:12.971004 reasoner_validator-4.1.6/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    49059 2024-05-10 19:15:12.971004 reasoner_validator-4.1.6/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-05-10 19:15:12.971004 reasoner_validator-4.1.6/tests/test_semver.py
--rw-r--r--   0        0        0     2351 2024-05-10 19:15:12.971004 reasoner_validator-4.1.6/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    36764 2024-05-10 19:15:12.971004 reasoner_validator-4.1.6/tests/test_validate.py
--rw-r--r--   0        0        0    30423 2024-05-10 19:15:12.971004 reasoner_validator-4.1.6/tests/test_validation_report.py
--rw-r--r--   0        0        0     3421 2024-05-10 19:15:12.971004 reasoner_validator-4.1.6/tests/test_workflows.py
--rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/LICENSE
+-rw-r--r--   0        0        0    13727 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/README.md
+-rw-r--r--   0        0        0      131 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/conf.py
+-rw-r--r--   0        0        0    20564 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    43219 2024-05-14 01:21:43.385422 reasoner_validator-4.1.7/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2298 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    95193 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    47100 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3973 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/message.py
+-rw-r--r--   0        0        0    47007 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    15057 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14745 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    38176 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    12127 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      866 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     3601 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 01:21:43.389422 reasoner_validator-4.1.7/tests/conftest.py
+-rw-r--r--   0        0        0   150844 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    49059 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_semver.py
+-rw-r--r--   0        0        0     2351 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    36764 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_validate.py
+-rw-r--r--   0        0        0    30423 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_validation_report.py
+-rw-r--r--   0        0        0     3421 2024-05-14 01:21:43.393422 reasoner_validator-4.1.7/tests/test_workflows.py
+-rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.7/PKG-INFO
```

### Comparing `reasoner_validator-4.1.6/LICENSE` & `reasoner_validator-4.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/README.md` & `reasoner_validator-4.1.7/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/docs/Makefile` & `reasoner_validator-4.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/docs/conf.py` & `reasoner_validator-4.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/docs/index.rst` & `reasoner_validator-4.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/docs/make.bat` & `reasoner_validator-4.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/docs/validation_codes_dictionary.md` & `reasoner_validator-4.1.7/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/pyproject.toml` & `reasoner_validator-4.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "4.1.6"
+version = "4.1.7"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-4.1.6/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.1.7/reasoner_validator/biolink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,24 +442,27 @@
 
     def validate_element_status(
             self,
             graph_type: TRAPIGraphType,
             context: str,
             identifier: str,
             edge_id: str,
-            source_trail: Optional[str] = None
+            source_trail: Optional[str] = None,
+            ignore_graph_type: bool = False
     ) -> Optional[Element]:
         """
         Detect element missing from Biolink, or is deprecated, abstract or mixin, signalled as a failure or warning.
 
         :param graph_type: TRAPIGraphType, type of TRAPI graph component being validated
         :param context: str, parsing context (e.g. 'Node')
         :param identifier: str, name of the putative Biolink element ('class')
         :param edge_id: str, identifier of enclosing edge containing the element (e.g. the 'edge_id')
         :param source_trail: Optional[str], audit trail of knowledge source provenance for a given Edge, as a string.
+        :param ignore_graph_type: bool, if strict validation is None (not set globally), then
+               only apply graph-type-differential strict validation if 'ignore_graph_type' is False
         :return: Optional[Element], Biolink Element resolved to 'name' if element no validation error; None otherwise.
         """
         element: Optional[Element] = self.bmt.get_element(identifier)
         if not element:
             self.report(
                 code=f"error.{context}.unknown",
                 source_trail=source_trail,
@@ -495,15 +498,15 @@
                     edge_id=edge_id
                 )
 
         elif self.bmt.is_mixin(identifier):
             # A mixin cannot be instantiated ...
             # but can be used in QueryGraphs
             # or when explicitly permitted
-            if self.is_strict_validation(graph_type):
+            if self.is_strict_validation(graph_type, ignore_graph_type=ignore_graph_type):
                 self.report(
                     code=f"error.{context}.mixin",
                     source_trail=source_trail,
                     identifier=identifier,
                     edge_id=edge_id
                 )
                 return None
@@ -1418,15 +1421,19 @@
             # *not* being abstract, deprecated or
             # a mixin (for Biolink Model release >= 4.2.1?)
             biolink_class = self.validate_element_status(
                 graph_type=graph_type,
                 context=context,
                 identifier=predicate,
                 edge_id=edge_id,
-                source_trail=source_trail
+                source_trail=source_trail,
+
+                # validation of 'predicates' can ignore graph type
+                # unless strict validation is globally overridden
+                ignore_graph_type=True
             )
             if biolink_class:
                 if not self.bmt.is_predicate(predicate):
                     self.report(
                         code=f"error.{context}.invalid",
                         source_trail=source_trail,
                         identifier=predicate,
```

### Comparing `reasoner_validator-4.1.6/reasoner_validator/codes.yaml` & `reasoner_validator-4.1.7/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/reasoner_validator/github.py` & `reasoner_validator-4.1.7/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/reasoner_validator/message.py` & `reasoner_validator-4.1.7/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/reasoner_validator/report.py` & `reasoner_validator-4.1.7/reasoner_validator/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,25 +106,27 @@
     def get_default_target(self) -> str:
         """
         Returns the current target of the ValidationReporter.
         :return: str, current target
         """
         return self.default_target
 
-    def is_strict_validation(self, graph_type: TRAPIGraphType) -> bool:
+    def is_strict_validation(self, graph_type: TRAPIGraphType, ignore_graph_type: bool = False) -> bool:
         """
         Predicate to test if strict validation is to be applied. If the internal
         'strict_validation' flag is not set (i.e. None), then graph_type is
         to resolve strictness based on TRAPI graph type context.
 
         :param graph_type: TRAPIGraphType, type of TRAPI graph component being validated
+        :param ignore_graph_type: bool, if strict validation is None (not set globally), then
+               only apply graph-type-differential strict validation if 'ignore_graph_type' is False
         :return: bool, value of validation strictness set in the ValidationReporter.
         """
         if self.strict_validation is None:
-            if graph_type == TRAPIGraphType.Knowledge_Graph:
+            if not ignore_graph_type and graph_type == TRAPIGraphType.Knowledge_Graph:
                 return True
             else:
                 return False
         else:
             return self.strict_validation
 
     def get_messages_by_target(self, target: Optional[str] = None) -> MESSAGES_BY_TEST:
```

### Comparing `reasoner_validator-4.1.6/reasoner_validator/sri/util.py` & `reasoner_validator-4.1.7/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.1.7/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.1.7/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/reasoner_validator/validation_codes.py` & `reasoner_validator-4.1.7/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/reasoner_validator/validator.py` & `reasoner_validator-4.1.7/reasoner_validator/validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/reasoner_validator/versioning.py` & `reasoner_validator-4.1.7/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/reasoner_validator/versions.yaml` & `reasoner_validator-4.1.7/reasoner_validator/versions.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/tests/__init__.py` & `reasoner_validator-4.1.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.1.7/tests/test_biolink_compliance_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -409,15 +409,18 @@
             "info.input_edge.predicate.mixin"
         )
     ]
 )
 def test_check_biolink_model_non_strict_compliance_of_input_edge(
         biolink_version: str, edge: Dict, validation_code: str
 ):
-    validator: BiolinkValidator = BiolinkValidator(biolink_version=biolink_version, strict_validation=False)
+    validator: BiolinkValidator = BiolinkValidator(
+        biolink_version=biolink_version,
+        strict_validation=False
+    )
     validator.check_biolink_model_compliance_of_input_edge(edge=edge)
     check_messages(validator, validation_code)
 
 
 @pytest.mark.parametrize(
     "biolink_version,graph",
     [
@@ -1155,15 +1158,61 @@
     ]
 )
 def test_check_biolink_model_non_strict_compliance_of_query_graph(
     query_graph: Dict,
     biolink_version: str,
     validation_code: str
 ):
-    validator: BiolinkValidator = BiolinkValidator(biolink_version=biolink_version, strict_validation=False)
+    validator: BiolinkValidator = BiolinkValidator(
+        biolink_version=biolink_version,
+        strict_validation=False
+    )
+    validator.check_biolink_model_compliance(
+        graph=query_graph,
+        graph_type=TRAPIGraphType.Query_Graph
+    )
+    check_messages(validator, validation_code)
+
+
+@pytest.mark.parametrize(
+    "biolink_version,query_graph,validation_code",
+    [
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+            # Query 0: Query edge predicate is a mixin, normally now
+            #          allowed in both QueryGraph and Knowledge Graphs but
+            #          caller here explicitly specifies strict validation
+            {
+                "nodes": {
+                    "IRS1": {"ids": ["HGNC:6125"], "categories": ["biolink:Gene"]},
+                    "drug": {
+                        "categories": ["biolink:Drug"]
+                    }
+                },
+                "edges": {
+                    "treats": {
+                        "subject": "drug",
+                        "predicates": ["biolink:increases_amount_or_activity_of"],
+                        "object": "IRS1"
+                    }
+                }
+            },
+            "error.query_graph.edge.predicate.mixin"
+        )
+    ]
+)
+def test_check_biolink_model_strict_compliance_of_query_graph(
+    query_graph: Dict,
+    biolink_version: str,
+    validation_code: str
+):
+    validator: BiolinkValidator = BiolinkValidator(
+        biolink_version=biolink_version,
+        strict_validation=True
+    )
     validator.check_biolink_model_compliance(
         graph=query_graph,
         graph_type=TRAPIGraphType.Query_Graph
     )
     check_messages(validator, validation_code)
 
 
@@ -3084,15 +3133,15 @@
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
-            "error.knowledge_graph.edge.predicate.mixin"
+            "info.knowledge_graph.edge.predicate.mixin"
         ),
         (
             "4.1.6",
             # Query 20: predicate is a mixin - not allowed in Knowledge Graphs, but "biolink:interacts_with"
             #           is tagged as an exception (see https://github.com/NCATSTranslator/reasoner-validator/issues/97)
             #           for Biolink Model releases < 4.2.0
             {
```

### Comparing `reasoner_validator-4.1.6/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.1.7/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/tests/test_response_validator.py` & `reasoner_validator-4.1.7/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/tests/test_semver.py` & `reasoner_validator-4.1.7/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/tests/test_trapi_versioning.py` & `reasoner_validator-4.1.7/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/tests/test_validate.py` & `reasoner_validator-4.1.7/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/tests/test_validation_report.py` & `reasoner_validator-4.1.7/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/tests/test_workflows.py` & `reasoner_validator-4.1.7/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.6/PKG-INFO` & `reasoner_validator-4.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.1.6
+Version: 4.1.7
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

