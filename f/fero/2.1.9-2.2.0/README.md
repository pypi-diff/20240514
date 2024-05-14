# Comparing `tmp/fero-2.1.9.tar.gz` & `tmp/fero-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fero-2.1.9.tar", last modified: Mon Sep 18 17:45:21 2023, max compression
+gzip compressed data, was "fero-2.2.0.tar", last modified: Fri Mar 29 14:19:14 2024, max compression
```

## Comparing `fero-2.1.9.tar` & `fero-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-18 17:45:21.277601 fero-2.1.9/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2023-09-18 17:45:06.000000 fero-2.1.9/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18382 2023-09-18 17:45:21.277601 fero-2.1.9/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17660 2023-09-18 17:45:06.000000 fero-2.1.9/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-18 17:45:21.277601 fero-2.1.9/fero/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2023-09-18 17:45:06.000000 fero-2.1.9/fero/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36932 2023-09-18 17:45:06.000000 fero-2.1.9/fero/analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7005 2023-09-18 17:45:06.000000 fero-2.1.9/fero/asset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12046 2023-09-18 17:45:06.000000 fero-2.1.9/fero/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2475 2023-09-18 17:45:06.000000 fero-2.1.9/fero/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9171 2023-09-18 17:45:06.000000 fero-2.1.9/fero/datasource.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-09-18 17:45:06.000000 fero-2.1.9/fero/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14849 2023-09-18 17:45:06.000000 fero-2.1.9/fero/process.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-18 17:45:21.277601 fero-2.1.9/fero.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18382 2023-09-18 17:45:21.000000 fero-2.1.9/fero.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      418 2023-09-18 17:45:21.000000 fero-2.1.9/fero.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-09-18 17:45:21.000000 fero-2.1.9/fero.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2023-09-18 17:45:21.000000 fero-2.1.9/fero.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-09-18 17:45:21.000000 fero-2.1.9/fero.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      280 2023-09-18 17:45:21.281601 fero-2.1.9/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1907 2023-09-18 17:45:06.000000 fero-2.1.9/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-18 17:45:21.277601 fero-2.1.9/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41466 2023-09-18 17:45:06.000000 fero-2.1.9/tests/test_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10345 2023-09-18 17:45:06.000000 fero-2.1.9/tests/test_asset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12385 2023-09-18 17:45:06.000000 fero-2.1.9/tests/test_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2097 2023-09-18 17:45:06.000000 fero-2.1.9/tests/test_datasource.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6792 2023-09-18 17:45:06.000000 fero-2.1.9/tests/test_process.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:19:14.106608 fero-2.2.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2024-03-29 14:18:56.000000 fero-2.2.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19876 2024-03-29 14:19:14.106608 fero-2.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18981 2024-03-29 14:18:56.000000 fero-2.2.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:19:14.102609 fero-2.2.0/fero/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2024-03-29 14:18:56.000000 fero-2.2.0/fero/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    39432 2024-03-29 14:18:56.000000 fero-2.2.0/fero/analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7005 2024-03-29 14:18:56.000000 fero-2.2.0/fero/asset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12898 2024-03-29 14:18:56.000000 fero-2.2.0/fero/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2475 2024-03-29 14:18:56.000000 fero-2.2.0/fero/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9171 2024-03-29 14:18:56.000000 fero-2.2.0/fero/datasource.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-03-29 14:18:56.000000 fero-2.2.0/fero/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16444 2024-03-29 14:18:56.000000 fero-2.2.0/fero/process.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:19:14.106608 fero-2.2.0/fero.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19876 2024-03-29 14:19:14.000000 fero-2.2.0/fero.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      418 2024-03-29 14:19:14.000000 fero-2.2.0/fero.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-29 14:19:14.000000 fero-2.2.0/fero.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2024-03-29 14:19:14.000000 fero-2.2.0/fero.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-03-29 14:19:14.000000 fero-2.2.0/fero.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      280 2024-03-29 14:19:14.106608 fero-2.2.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1909 2024-03-29 14:18:56.000000 fero-2.2.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:19:14.106608 fero-2.2.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43655 2024-03-29 14:18:56.000000 fero-2.2.0/tests/test_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10345 2024-03-29 14:18:56.000000 fero-2.2.0/tests/test_asset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12385 2024-03-29 14:18:56.000000 fero-2.2.0/tests/test_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2097 2024-03-29 14:18:56.000000 fero-2.2.0/tests/test_datasource.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8032 2024-03-29 14:18:56.000000 fero-2.2.0/tests/test_process.py
```

### Comparing `fero-2.1.9/LICENSE` & `fero-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fero-2.1.9/PKG-INFO` & `fero-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: fero
-Version: 2.1.9
+Version: 2.2.0
 Summary: Python client for accessing Fero API
 Home-page: https://github.com/FeroLabs/fero_client
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Source, https://github.com/pypa/sampleproject/
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pandas<1.5.0,>=1.4.4
+Requires-Dist: marshmallow<3.16.0,>=3.8.0
+Requires-Dist: azure-storage-blob
+Requires-Dist: pyarrow<15.0,>=12.0.0
 
 # fero_client
 
 `fero` is a client-side Python library intended to help users interact with [Fero](https://app.ferolabs.com).
 
 ## Quickstart
 
@@ -196,31 +201,67 @@
 constraints = [{"name": "target", "min": 100.0, "max": 200}]
 
 opt = analysis.make_optimization("example_cost_optimization", goal, constraints)
 ```
 
 In both cases, a `Prediction` object is returned, which will provide access to the results of the optimization. By default, the result will be a `DataFrame` but it can also be configured to be a list of dictionaries by specifying `format="record"` in `get_results`.
 
-#### Example
+#### Example 4: Optimize a target subject to combination constriants
+
+Fero also supports combination constraints, which allow us to find optima subject to more complex relationships between different factors and targets. For example, we can find the maximum tensile strength while ensuring that the tensile/yield strength ratio does not exceed some threshold, and that the mass of carbon plus silicon meets some minimum threshold. Provided methods can assist in structuring these constraints.
 
 ```python
+from fero.analysis import (
+  CombinationConstraintOperandType as operands,
+  CombinationConstraintOperator as operators
+)
 goal = {
-  "goal": "minimize",
-  "factor": {"name": "value", "min": 50.0, "max": 100.0}
+  "goal": "maximimze",
+  "factor": {"name": "Tensile Strength", "min": 10000.0, "max": 20000.0}
 }
 
-constraints = [{"name": "target", "min": 100.0, "max": 200}]
+constraints = [
+  {"name": "Carbon", "min": 0.0, "max": 50.0},
+  {"name": "Vanadium", "min": 0.0, "max": 25.0},
+  {"name": "Yield Strength", "min": 1000.0, "max" 5000.0},
+  {"name": "Copper", "min": 10.0, "max": 15.0}
+]
 
-opt = analysis.make_optimization("example_optimization", goal, constraints)
+fixed_factors = {
+  "Product Type": "Type 1",
+  "Product Grade": "Grade B",
+  "Silicon": 14.0,
+  "STRENGTH_RATIO": 12.5,
+  "CARBON_MASS": 12.011,
+  "SILICON_MASS": 28.05,
+  "Iron": 4501.12,
+  "Temperature": 350.1,
+  "test_time": "2024-01-01T00:00"
+}
 
-print(opt.get_results())
-'''
-   value   value2   target (5%)   target (Mean)   target (95%)
-0     60       40           100             150            175
-'''
+combination_constraints = [
+  CombinationConstraint(
+    ("'Tensile Strength' / 'Yield Strength'", operands.FORMULA),
+    operators.LESS_THAN_OR_EQUAL,
+    ("STRENGTH_RATIO", operands.COLUMN)
+  ),
+  CombinationConstraint(
+    ("'CARBON_MASS' * 'CARBON' + 'SILICON_MASS' * 'Silicon'", operands.FORMULA),
+    operators.GREATER_THAN,
+    (134.23, operands.CONSTANT)
+  )
+]
+
+opt = analysis.make_optimization(
+  "example_cost_optimization",
+  goal,
+  constraints,
+  fixed_factors,
+  combination_constraints=combination_constraints
+)
 ```
 
 ## Finding a Fero Asset
 
 The Fero client provides two different methods to find an `Asset`. The first is `Fero.get_asset`, which takes a single unique identifier string (UUID) and attempts to look up the asset matching this ID. The second method is `Fero.search_assets`, which will return an iterator of available `Asset` objects. If no keyword arguments are provided, it will return all assets you have available on the Fero website. Optionally, `name` can be provided to filter to only assets matching that name.
 
 #### Examples
```

### Comparing `fero-2.1.9/README.md` & `fero-2.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -178,31 +178,67 @@
 constraints = [{"name": "target", "min": 100.0, "max": 200}]
 
 opt = analysis.make_optimization("example_cost_optimization", goal, constraints)
 ```
 
 In both cases, a `Prediction` object is returned, which will provide access to the results of the optimization. By default, the result will be a `DataFrame` but it can also be configured to be a list of dictionaries by specifying `format="record"` in `get_results`.
 
-#### Example
+#### Example 4: Optimize a target subject to combination constriants
+
+Fero also supports combination constraints, which allow us to find optima subject to more complex relationships between different factors and targets. For example, we can find the maximum tensile strength while ensuring that the tensile/yield strength ratio does not exceed some threshold, and that the mass of carbon plus silicon meets some minimum threshold. Provided methods can assist in structuring these constraints.
 
 ```python
+from fero.analysis import (
+  CombinationConstraintOperandType as operands,
+  CombinationConstraintOperator as operators
+)
 goal = {
-  "goal": "minimize",
-  "factor": {"name": "value", "min": 50.0, "max": 100.0}
+  "goal": "maximimze",
+  "factor": {"name": "Tensile Strength", "min": 10000.0, "max": 20000.0}
 }
 
-constraints = [{"name": "target", "min": 100.0, "max": 200}]
-
-opt = analysis.make_optimization("example_optimization", goal, constraints)
+constraints = [
+  {"name": "Carbon", "min": 0.0, "max": 50.0},
+  {"name": "Vanadium", "min": 0.0, "max": 25.0},
+  {"name": "Yield Strength", "min": 1000.0, "max" 5000.0},
+  {"name": "Copper", "min": 10.0, "max": 15.0}
+]
+
+fixed_factors = {
+  "Product Type": "Type 1",
+  "Product Grade": "Grade B",
+  "Silicon": 14.0,
+  "STRENGTH_RATIO": 12.5,
+  "CARBON_MASS": 12.011,
+  "SILICON_MASS": 28.05,
+  "Iron": 4501.12,
+  "Temperature": 350.1,
+  "test_time": "2024-01-01T00:00"
+}
 
-print(opt.get_results())
-'''
-   value   value2   target (5%)   target (Mean)   target (95%)
-0     60       40           100             150            175
-'''
+combination_constraints = [
+  CombinationConstraint(
+    ("'Tensile Strength' / 'Yield Strength'", operands.FORMULA),
+    operators.LESS_THAN_OR_EQUAL,
+    ("STRENGTH_RATIO", operands.COLUMN)
+  ),
+  CombinationConstraint(
+    ("'CARBON_MASS' * 'CARBON' + 'SILICON_MASS' * 'Silicon'", operands.FORMULA),
+    operators.GREATER_THAN,
+    (134.23, operands.CONSTANT)
+  )
+]
+
+opt = analysis.make_optimization(
+  "example_cost_optimization",
+  goal,
+  constraints,
+  fixed_factors,
+  combination_constraints=combination_constraints
+)
 ```
 
 ## Finding a Fero Asset
 
 The Fero client provides two different methods to find an `Asset`. The first is `Fero.get_asset`, which takes a single unique identifier string (UUID) and attempts to look up the asset matching this ID. The second method is `Fero.search_assets`, which will return an iterator of available `Asset` objects. If no keyword arguments are provided, it will return all assets you have available on the Fero website. Optionally, `name` can be provided to filter to only assets matching that name.
 
 #### Examples
```

### Comparing `fero-2.1.9/fero/analysis.py` & `fero-2.2.0/fero/analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """This module holds classes related to a fero analysis."""
 
 import time
 import fero
 import uuid
 import io
 import datetime
+from enum import Enum
 from fero import FeroError
 import pandas as pd
 from marshmallow import (
     Schema,
     fields,
     validate,
     validates_schema,
     ValidationError,
     EXCLUDE,
 )
-from typing import Any, Union, List, Optional, IO
+from typing import Any, Union, List, Optional, IO, Tuple
 from .common import FeroObject
 
 
 VALID_GOALS = ["minimize", "maximize"]
 FERO_COST_FUNCTION = "FERO_COST_FUNCTION"
 V1_RESULT_SUFFIXES = ["low", "mid", "high"]
 V2_RESULT_SUFFIXES = ["low90", "low50", "mid", "high50", "high90"]
 BULK_PREDICTION_TYPE = "M"
+VALID_JOINS = ["AND", "OR"]
 
 
 class AnalysisSchema(Schema):
     """A schema to store data related to a fero analysis."""
 
     class Meta:
         """
@@ -182,28 +184,78 @@
 
 class CostOptimizeGoal(BaseGoalSchema):
     """A schema to store data related to a goal to minimize cost in a fero analysis optimization."""
 
     type = fields.String(validate=validate.OneOf(["COST"]), required=True)
     cost_function = fields.Nested(CostSchema, many=True, required=True)
 
-    @validates_schema
-    def max_functions(self, data: dict, **kwargs):
-        """Validate that there are no more than three cost functions in the `data`.
 
-        :raises ValidationError: when there are more than three cost functions specified in `data`
+class CombinationConstraintOperandType(Enum):
+    """An enum listing all valid types of Combination Constraint Operands."""
+
+    FORMULA = "formula"
+    CONSTANT = "constant"
+    COLUMN = "column"
+
+
+class CombinationConstraintOperator(Enum):
+    """An enum listing all valid types of Combination Constraint Operators."""
+
+    GREATER_THAN = ">"
+    GREATER_THAN_OR_EQUAL = ">="
+    LESS_THAN = "<"
+    LESS_THAN_OR_EQUAL = "<="
+    EQUAL = "=="
+    NOT_EQUAL = "!="
+
+
+class CombinationConstraint:
+    """A class to facilitate structuring additional optimization constraints. See README for details."""
+
+    def __init__(
+        self,
+        operand_a: Tuple[Union[str, int, float], CombinationConstraintOperandType],
+        operator: CombinationConstraintOperator,
+        operand_b: Tuple[Union[str, int, float], CombinationConstraintOperandType],
+    ):
         """
-        if len(data["cost_function"]) > 3:
-            raise ValidationError(
-                {
-                    "cost_function": [
-                        "No more than three factors allowed in the cost function."
-                    ]
-                }
-            )
+        Create a `Combination Constraint` with two provided operands and an operator.
+
+        :param operand_a: A tuple with the first operand's value and type. (Left side of operator).
+        :param operator: Enum value indicating which a supported operation for the operands.
+        :param operand_b: A tuple with the second operand's value and type. (Right side of operator).
+        """
+        self._operand_a = operand_a
+        self._operand_b = operand_b
+        self._operator = operator
+
+    def combination_constraint_to_dict(self):
+        """Return valid dictionary representation of this constraint."""
+        a_value, a_kind = self._operand_a
+        b_value, b_kind = self._operand_b
+        return {
+            "kind": "condition",
+            "target": {"kind": a_kind.value, "value": a_value},
+            "operation": {
+                "operator": self._operator.value,
+                "operand": {"kind": b_kind.value, "value": b_value},
+            },
+        }
+
+    def verify_combination_constraint(self, analysis):
+        """Check that literal column references are valid for this analysis.
+
+        Formula verification occurs on Fero's servers. Any errors will be provided in optimization results.
+        """
+        for [value, kind] in [self._operand_a, self._operand_b]:
+            if kind == CombinationConstraintOperandType.COLUMN:
+                if value not in analysis.all_factor_names:
+                    raise FeroError(
+                        f'"{value}" is not a recognized factor in this analysis'
+                    )
 
 
 class Prediction:
     """Represents the results of a prediction submitted to Fero.
 
     Predictions are run asynchrounously by Fero and data will only be available if the `complete` property
     is true.  Attempting to access the data for the prediction before it is complete will result in a `FeroError`
@@ -307,19 +359,19 @@
     """An object for interacting with a specific Analysis on Fero.
 
     The Analysis is the primary way to access a model associated with a data set.
     Once an analysis is created it can be used to perform various actions such as making a prediction
     based on provided data or optimizing certain values based on the Fero model of the data.
     """
 
-    _presentation_data_cache: Union[dict, None] = None
-    _reg_factors: Union[List[dict], None] = None
-    _reg_targets: Union[List[dict], None] = None
-    _factor_names: Union[List[str], None] = None
-    _target_names: Union[List[str], None] = None
+    _presentation_data_cache: Optional[dict] = None
+    _reg_factors: Optional[List[dict]] = None
+    _reg_targets: Optional[List[dict]] = None
+    _factor_names: Optional[List[str]] = None
+    _target_names: Optional[List[str]] = None
 
     schema_class = AnalysisSchema
 
     def __repr__(self) -> str:
         """Represent the `Analysis` by its name."""
         return f"<Analysis name={self.name}>"
 
@@ -339,15 +391,15 @@
         if self._reg_targets is None:
             self._parse_regression_data()
 
         return self._reg_targets
 
     @property
     def factor_names(self) -> Optional[List[str]]:
-        """Get the names of the factors associated with the Analysis."""
+        """Get the names of the factors in the model of the Analysis."""
         if self._factor_names is None:
             self._parse_regression_data()
 
         return self._factor_names
 
     @property
     def target_names(self) -> Optional[List[str]]:
@@ -380,14 +432,19 @@
                 v1_schema = self._client.get(
                     f"/api/data_sources/{self.data_source}/latest_interpreted_schema/"
                 )
             self._schema_cache = v1_schema
 
         return self._schema_cache
 
+    @property
+    def all_factor_names(self):
+        """Get all factor names for any column available to the Analysis."""
+        return [column["name"] for column in self._schema["columns"]]
+
     @staticmethod
     def _make_col_name(col_name: str, cols: List[str]) -> str:
         """Mangle duplicate columns."""
         c = 0
         og_col_name = col_name
         while col_name in cols:
             col_name = f"{og_col_name}.{c}"
@@ -613,17 +670,19 @@
         """Verify provided constraints are in the analysis."""
         use_adaptive = kwargs.get("use_adaptive", False)
         for constraint in constraints:
             constraint_name = constraint["name"]
             constraint_type = (
                 self._get_factor_dtype(constraint_name)
                 if constraint_name in self.factor_names
-                else self._get_target_dtype(constraint_name)
-                if constraint_name in self.target_names
-                else None
+                else (
+                    self._get_target_dtype(constraint_name)
+                    if constraint_name in self.target_names
+                    else None
+                )
             )
             if constraint_type is None:
                 raise FeroError(
                     f'Constraint "{constraint_name}" is not part of this model.'
                 )
             elif constraint_type == "factor_category" and (
                 constraint.get("min", None) is not None
@@ -645,15 +704,20 @@
                 constraint.get("min", None) is None
                 or constraint.get("max", None) is None
             ):
                 raise FeroError(
                     f'Numeric constraint "{constraint_name}" requires a min and max value.'
                 )
 
-    def _cross_verify_optimization(self, goal: dict, constraints: List[dict], **kwargs):
+    def _cross_verify_optimization(
+        self,
+        goal: dict,
+        constraints: List[dict],
+        **kwargs,
+    ):
         """Verify the config has the correct combined targets, costs and factors."""
         is_cost = goal.get("type", None) == "COST"
 
         cost_factors = []
         goal_factor = []
         target_factor = []
         constraint_factors = []
@@ -691,20 +755,29 @@
                 "A maximum of three factors can be specified in an optimization."
             )
         elif use_adaptive and len(constraint_factors + cost_factors + goal_factor) > 5:
             raise FeroError(
                 "A maximum of five factors can be specified in an adaptive optimization."
             )
 
+    def _verify_combination_constraints(
+        self, combination_constraints: Optional[List[CombinationConstraint]]
+    ):
+        if combination_constraints is None or len(combination_constraints) < 1:
+            return
+
+        for constraint in combination_constraints:
+            constraint.verify_combination_constraint(self)
+
     def _verify_fixed_factors(self, fixed_factors: dict):
         """Check that the provided fixed factors are in the analysis."""
-        all_columns = self.target_names + self.factor_names
+        all_columns = self.all_factor_names
         for key in fixed_factors.keys():
             if key not in all_columns:
-                raise FeroError(f'"{key}" is not part of this model.')
+                raise FeroError(f'"{key}" is not part of this analysis.')
 
     def _get_basis_values(self):
         """Get median fixed values from presentation data."""
         reg_data = next(
             d
             for d in self._presentation_data["data"]
             if d["id"] == "regression_simulator"
@@ -722,14 +795,15 @@
     def _build_optimize_request(
         self,
         name,
         goal,
         constraints,
         fixed_factors,
         include_confidence_intervals,
+        combination_constraints,
         **kwargs,
     ) -> dict:
         """Format the content for an optimization request."""
         is_cost = goal.get("type", None) == "COST"
         ci_value = "include" if include_confidence_intervals else "exclude"
         opt_request = {
             "name": name,
@@ -742,18 +816,27 @@
             "version": 1,
             "objectives": [
                 {
                     "factor": FERO_COST_FUNCTION if is_cost else goal["factor"]["name"],
                     "goal": goal["goal"],
                 }
             ],
-            "basisSpecifiedColumns": [],  # These appear to just be, uhm, here
+            "basisSpecifiedColumns": [],
             "linearFunctionDefinitions": {},
             "useAdaptiveGrid": kwargs.get("use_adaptive", False),
         }
+        if combination_constraints is not None and len(combination_constraints) > 0:
+            input_data["combinationConstraints"] = {
+                "conditions": [
+                    constraint.combination_constraint_to_dict()
+                    for constraint in combination_constraints
+                ],
+                "join": "AND",
+                "kind": "clause",
+            }
         basis_values = self._get_basis_values()
         basis_values.update(fixed_factors)
         input_data["basisValues"] = basis_values
 
         factor_bounds = []
         for c in constraints:
             if c["name"] in self.factor_names:
@@ -825,17 +908,19 @@
                 if goal_is_target
                 else self._get_factor_dtype(goal_name)
             )
             goal_bound = {
                 "factor": goal["factor"]["name"],
                 "lowerBound": goal["factor"]["min"],
                 "upperBound": goal["factor"]["max"],
-                "dtype": dtype
-                if dtype is not None
-                else f"{'target' if goal_is_target else 'factor'}_float",
+                "dtype": (
+                    dtype
+                    if dtype is not None
+                    else f"{'target' if goal_is_target else 'factor'}_float"
+                ),
             }
             if goal_is_target:
                 goal_bound["confidenceInterval"] = ci_value
 
             bounds.append(goal_bound)
 
         input_data["bounds"] = bounds
@@ -885,63 +970,37 @@
         self,
         name: str,
         goal: dict,
         constraints: List[dict],
         fixed_factors: Optional[dict] = None,
         include_confidence_intervals: bool = True,
         synchronous: bool = True,
+        combination_constraints: Optional[List[CombinationConstraint]] = None,
         **kwargs,
     ) -> Prediction:
         """Perform an optimization using the most recent model for the analysis.
 
         By default this function will block until the optimization is complete, however specifying `synchonous=False`
         will instead return a prediction object referencing the optimization being made. This prediction will not contain
         results until the `complete` property is true.
 
-        The expected config input looks as follows:
-
-        Example configuration for a standard (without cost) optimization::
-
-            {
-                "goal": "maximize",
-                "factor": {"name": "factor1", "min": 5, "max": 10}
-            }
-
-        Example configuration for a cost optimization:
-        Cost Goal Config
-        ::
-
-            {
-                "type": "COST",
-                "goal": "minimize"
-                "cost_function": [
-                    {"min": 5, "max": 10, "cost": 1000, "name": "factor1"},
-                    {"min": 5, "max": 10, "cost": 500,  "name": "target2"}
-                ]
-            }
-
-        The constraints configuration is a list of factors and their constraints::
-
-            [
-                {"name": "factor2",  "min": 10, "max": 10}
-                {"name": "target1", "min": 100, "max": 500}
-            ]
-
         :param name: Name for this optimization
         :type name: str
         :param goal: A dictionary describing the goal of the optimization
         :type goal: dict
         :param constraints: A dictionary describing the constraints of the optimization
         :type constraints: dict
         :param fixed_factors: Values of factors to stay fixed if not provided the mean values are used, defaults to None
         :type fixed_factors: dict, optional
         :param include_confidence_intervals: Whether the optimization should include the lower 5% and upper 95% prediction levels, defaults to True
         :type include_confidence_intervals: bool, optional
         :param synchronous: Whether the optimization should return only after being complete.  This can take a bit, defaults to True
         :type synchronous: bool, optional
+        :param combination_constraints: A list of additional constraints on the optimization results, typically relating multiple factors or targets.
+        :type combination_constraints: list, optional
         :return: The results of the optimization
         :rtype: Prediction
         """
         if self.blueprint_name == "fault":
             raise FeroError("Fault analysis optimization are not supported")
 
         cost_goal = "type" in goal
@@ -962,19 +1021,21 @@
 
         if cost_goal:
             self._verify_cost_goal(goal)
         else:
             self._verify_standard_goal(goal)
 
         self._verify_constraints(constraints, **kwargs)
+        self._verify_combination_constraints(combination_constraints, **kwargs)
         self._cross_verify_optimization(goal, constraints, **kwargs)
         self._verify_fixed_factors(fixed_factors)
 
         optimize_request = self._build_optimize_request(
             name,
             goal,
             constraints,
             fixed_factors,
             include_confidence_intervals,
+            combination_constraints,
             **kwargs,
         )
         return self._request_prediction(optimize_request, synchronous)
```

### Comparing `fero-2.1.9/fero/asset.py` & `fero-2.2.0/fero/asset.py`

 * *Files identical despite different names*

### Comparing `fero-2.1.9/fero/client.py` & `fero-2.2.0/fero/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         :raises FeroError: Raised if a token cannot be obtained
         """
         self._fero_token = None
         self._fero_conf_content = None
         self._password = None
         self._username = None
         self._verify = verify
+        self._impersonated = None
 
         self._hostname = hostname.rstrip("/")
 
         if fero_token:
             self._fero_token = fero_token
 
         if username and password:
@@ -82,14 +83,19 @@
     def fero_conf_contents(self) -> str:
         """Cache the file content."""
         if self._fero_conf_content is None:
             self._get_fero_conf_contents()
 
         return self._fero_conf_content
 
+    @property
+    def current_user(self) -> str:
+        """Return the username of the current user."""
+        return self._impersonated or self._username
+
     def _get_token_string_from_local(self) -> Union[str, None]:
         """Check the local system for the JWT token string."""
         if "FERO_TOKEN" in os.environ:
             return os.environ.get("FERO_TOKEN")
         jwt_match = re.search(r"FERO_TOKEN=([^\n]+)\n", self.fero_conf_contents)
         return jwt_match.group(1) if jwt_match else None
 
@@ -325,7 +331,27 @@
         return self._handle_response(
             requests.get(
                 url,
                 params=params,
                 verify=self._verify,
             )
         )
+
+    def impersonate(self, username: str):
+        """Impersonate a user.  Only available to admin users.
+
+        :param username: The username to impersonate
+        :type user_id: str
+        :return: None
+        """
+        impersonated_token = self.post(
+            "/api/token/impersonate/", {"user": username}
+        ).get("token")
+        self._admin_token = self._fero_token
+        self._fero_token = impersonated_token
+        self._impersonated = username
+
+    def end_impersonation(self):
+        """Disable client impersonation."""
+        self._fero_token = self._admin_token
+        self._admin_token = None
+        self._impersonated = None
```

### Comparing `fero-2.1.9/fero/common.py` & `fero-2.2.0/fero/common.py`

 * *Files identical despite different names*

### Comparing `fero-2.1.9/fero/datasource.py` & `fero-2.2.0/fero/datasource.py`

 * *Files identical despite different names*

### Comparing `fero-2.1.9/fero/process.py` & `fero-2.2.0/fero/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -347,16 +347,47 @@
         return [
             Tag(self, self._client, tag_data)
             for tag_data in self._client.get(f"/api/processes/{self.api_id}/tags/").get(
                 "tags"
             )
         ]
 
-    def _tag_stage_index(self, tag: Union[Tag, str]) -> Union[int, None]:
+    @property
+    @memoized(maxsize=1)
+    def lims_feeds_batch_id_column_names(self) -> Sequence[Sequence[str]]:
+        """Get batch ids for LIMS-only processes.
+
+        Returns a list of lists of composite batch id
+        column names for each LIMS feed, respects the
+        batch id order as initially specified.  If the
+        process is not LIMS-only, an empty list is returned.
+        """
+        config = self.data_config.get("config", {})
+        config_kind = config.get("kind")
+        initial_feed = config.get("initialFeed", {})
+        lims_data = config.get("limsData", [])
+
+        def _join_these_tag_names(lf):
+            tag_name = lf.get("joinThisTagName")
+            tag_names = lf.get("additionalJoinTheseTagNames", [])
+            if tag_name is not None:
+                tag_names.insert(0, tag_name)
+            return tag_names
+
+        if (
+            self.process_type != FeroProcessTypes.BATCH
+            or config_kind != "BatchDataConfig"
+        ):
+            return []
+        else:
+            if initial_feed.get("kind") != "InitialFeedDescription":
+                lims_data.insert(0, initial_feed)
+            return [_join_these_tag_names(lf) for lf in lims_data]
 
+    def _tag_stage_index(self, tag: Union[Tag, str]) -> Union[int, None]:
         stage_idx = None
         tag_name = Tag.tag_name(tag)
         for idx, s in enumerate(self.stages):
             if tag_name in s.tag_names:
                 stage_idx = idx
                 break
 
@@ -382,26 +413,29 @@
 
         return [] if len(idxs) == 0 else self.stages[: max(idxs) + 1]
 
     def get_data(
         self,
         tags: Sequence[Union[Tag, str]],
         kpis: Optional[Sequence[Union[Tag, str]]] = None,
+        include_batch_id: Optional[bool] = False,
     ) -> pd.DataFrame:
         """Download a pandas data frame with specified process data.
 
         Returns a pandas data frame consisting of the specified tags and bounded by an optional list of kpis.
         For all process types specifying a kpi will remove any tags from stages that are after
         the stage the kpi is assigned to.  For advanced and batch process types not providing a kpi will
         get tags from all stages.  For a continuous process, a kpi must be specified.
 
         :param tags: List of Tags or tag names to include in the data frame
         :type tags: Sequence[Union[Tag, str]]
         :param kpis: List of tags or tag names to use for kpis, defaults to None
         :type kpis: Optional[Sequence[Union[Tag, str]]], optional
+        :param include_batch_id: When true, batch id is returned as index for LIMS-only Processes
+        :type include_batch_id: Optional[bool], optional
         :raises DataRequestError: Raised if data can not be generated
         :return: A data frame of the data generated by the process.
         :rtype: pd.DataFrame
         """
         if self.process_type == FeroProcessTypes.CONTINUOUS and kpis is None:
             raise DataRequestError(
                 "A kpi must be specified to download continuous process data"
@@ -410,15 +444,21 @@
         tag_names = [Tag.tag_name(tag) for tag in tags]
         kpi_names = None
         if kpis:
             kpi_names = [tag if isinstance(tag, str) else tag.name for tag in kpis]
 
         initial_response = self._client.post(
             f"/api/processes/{self.api_id}/download_process_data/",
-            {"request_data": {"tags": tag_names, "kpis": kpi_names}},
+            {
+                "request_data": {
+                    "tags": tag_names,
+                    "kpis": kpi_names,
+                    "include_batch_id": include_batch_id,
+                }
+            },
         )
 
         request_id = initial_response["request_id"]
 
         def get_data():
             return self._client.post(
                 f"/api/processes/{self.api_id}/download_process_data/",
@@ -427,16 +467,17 @@
 
         download_response = poll(get_data, lambda d: d["complete"])
 
         download_data = download_response["data"]
 
         if not download_data["success"]:
             raise DataRequestError(download_data["message"])
-
         # Download the file and write as a stream since it could be large
         req = requests.get(download_data["download_url"], stream=True)
+        req.raise_for_status()
+
         with NamedTemporaryFile() as fp:
             for chunk in req.iter_content(chunk_size=CHUNK_SIZE):
                 fp.write(chunk)
             fp.seek(0)
             df = pd.read_parquet(fp.name)
         return df
```

### Comparing `fero-2.1.9/fero.egg-info/PKG-INFO` & `fero-2.2.0/fero.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: fero
-Version: 2.1.9
+Version: 2.2.0
 Summary: Python client for accessing Fero API
 Home-page: https://github.com/FeroLabs/fero_client
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Source, https://github.com/pypa/sampleproject/
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pandas<1.5.0,>=1.4.4
+Requires-Dist: marshmallow<3.16.0,>=3.8.0
+Requires-Dist: azure-storage-blob
+Requires-Dist: pyarrow<15.0,>=12.0.0
 
 # fero_client
 
 `fero` is a client-side Python library intended to help users interact with [Fero](https://app.ferolabs.com).
 
 ## Quickstart
 
@@ -196,31 +201,67 @@
 constraints = [{"name": "target", "min": 100.0, "max": 200}]
 
 opt = analysis.make_optimization("example_cost_optimization", goal, constraints)
 ```
 
 In both cases, a `Prediction` object is returned, which will provide access to the results of the optimization. By default, the result will be a `DataFrame` but it can also be configured to be a list of dictionaries by specifying `format="record"` in `get_results`.
 
-#### Example
+#### Example 4: Optimize a target subject to combination constriants
+
+Fero also supports combination constraints, which allow us to find optima subject to more complex relationships between different factors and targets. For example, we can find the maximum tensile strength while ensuring that the tensile/yield strength ratio does not exceed some threshold, and that the mass of carbon plus silicon meets some minimum threshold. Provided methods can assist in structuring these constraints.
 
 ```python
+from fero.analysis import (
+  CombinationConstraintOperandType as operands,
+  CombinationConstraintOperator as operators
+)
 goal = {
-  "goal": "minimize",
-  "factor": {"name": "value", "min": 50.0, "max": 100.0}
+  "goal": "maximimze",
+  "factor": {"name": "Tensile Strength", "min": 10000.0, "max": 20000.0}
 }
 
-constraints = [{"name": "target", "min": 100.0, "max": 200}]
+constraints = [
+  {"name": "Carbon", "min": 0.0, "max": 50.0},
+  {"name": "Vanadium", "min": 0.0, "max": 25.0},
+  {"name": "Yield Strength", "min": 1000.0, "max" 5000.0},
+  {"name": "Copper", "min": 10.0, "max": 15.0}
+]
 
-opt = analysis.make_optimization("example_optimization", goal, constraints)
+fixed_factors = {
+  "Product Type": "Type 1",
+  "Product Grade": "Grade B",
+  "Silicon": 14.0,
+  "STRENGTH_RATIO": 12.5,
+  "CARBON_MASS": 12.011,
+  "SILICON_MASS": 28.05,
+  "Iron": 4501.12,
+  "Temperature": 350.1,
+  "test_time": "2024-01-01T00:00"
+}
 
-print(opt.get_results())
-'''
-   value   value2   target (5%)   target (Mean)   target (95%)
-0     60       40           100             150            175
-'''
+combination_constraints = [
+  CombinationConstraint(
+    ("'Tensile Strength' / 'Yield Strength'", operands.FORMULA),
+    operators.LESS_THAN_OR_EQUAL,
+    ("STRENGTH_RATIO", operands.COLUMN)
+  ),
+  CombinationConstraint(
+    ("'CARBON_MASS' * 'CARBON' + 'SILICON_MASS' * 'Silicon'", operands.FORMULA),
+    operators.GREATER_THAN,
+    (134.23, operands.CONSTANT)
+  )
+]
+
+opt = analysis.make_optimization(
+  "example_cost_optimization",
+  goal,
+  constraints,
+  fixed_factors,
+  combination_constraints=combination_constraints
+)
 ```
 
 ## Finding a Fero Asset
 
 The Fero client provides two different methods to find an `Asset`. The first is `Fero.get_asset`, which takes a single unique identifier string (UUID) and attempts to look up the asset matching this ID. The second method is `Fero.search_assets`, which will return an iterator of available `Asset` objects. If no keyword arguments are provided, it will return all assets you have available on the Fero website. Optionally, `name` can be provided to filter to only assets matching that name.
 
 #### Examples
```

### Comparing `fero-2.1.9/setup.py` & `fero-2.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup
 from setuptools.command.install import install
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
-VERSION = "2.1.9"
+VERSION = "2.2.0"
 
 
 class VerifyVersionCommand(install):
     """Custom command to verify that the git tag matches our version."""
 
     description = "verify that the git tag matches our version"
 
@@ -46,18 +46,18 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3 :: Only",
     ],
     packages=["fero"],
     python_requires=">=3.7, <4",
     install_requires=[
         "requests",
-        "pandas>=1.2.0,<1.5.0",
+        "pandas>=1.4.4,<1.5.0",
         "marshmallow>=3.8.0,<3.16.0",
         "azure-storage-blob",
-        "pyarrow>=6.0.0,<7.0",
+        "pyarrow>=12.0.0,<15.0",
     ],
     project_urls={
         "Bug Reports": "https://github.com/pypa/sampleproject/issues",
         "Source": "https://github.com/pypa/sampleproject/",
     },
     cmdclass={
         "verify": VerifyVersionCommand,
```

### Comparing `fero-2.1.9/tests/test_analysis.py` & `fero-2.2.0/tests/test_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 
 import io
 import datetime
 from uuid import uuid4
 import pytest
 from fero import FeroError
 from unittest import mock
-from fero.analysis import Analysis, Prediction
+from fero.analysis import (
+    Analysis,
+    Prediction,
+    CombinationConstraint,
+    CombinationConstraintOperandType as operands,
+    CombinationConstraintOperator as operators,
+)
 import pandas as pd
 from pandas.testing import assert_frame_equal
 
 
 @pytest.fixture
 def test_analysis(
     analysis_data,
@@ -155,14 +161,40 @@
                 },
             ],
         },
     }
 
 
 @pytest.fixture
+def expected_optimization_config_with_combination_constraint(
+    expected_optimization_config,
+):
+    """Add a combination constraint to the sample optimization config."""
+    config = {**expected_optimization_config}
+    config["input_data"]["combinationConstraints"] = {
+        "conditions": [
+            {
+                "kind": "condition",
+                "target": {
+                    "value": "'Factor 1' + 'Factor 2'",
+                    "kind": "formula",
+                },
+                "operation": {
+                    "operator": ">",
+                    "operand": {"kind": "constant", "value": 150.0},
+                },
+            }
+        ],
+        "join": "AND",
+        "kind": "clause",
+    }
+    return config
+
+
+@pytest.fixture
 def prediction_request_response(expected_optimization_config):
     """Get a sample prediction request resopnse using the sample optimization configuration."""
     response = {
         "latest_prediction": {
             "uuid": "01bff6f2-8fb3-469e-813a-9b6cfd93e338",
             "created_by": {"id": 2, "username": "fero"},
             "created": "2020-09-30T12:35:44.897461Z",
@@ -721,35 +753,71 @@
                     {"name": "Category 0", "min": 5.0, "max": 7.0, "cost": 1000},
                 ],
             },
             [{"name": "Target 1", "min": 10, "max": 11}],
         )
 
 
+def test_make_optimization_combination_constraint_unknown_column(
+    test_analysis_with_data,
+):
+    """Test that a combination constraint raises a Fero Error if it references an unknown column."""
+    with pytest.raises(FeroError):
+        test_analysis_with_data.make_optimization(
+            "test optimization",
+            {
+                "goal": "maximize",
+                "factor": {"name": "Factor 2", "min": 70.0, "max": 100.0},
+            },
+            [
+                {"name": "Factor 1", "min": 60.0, "max": 200.0},
+                {"name": "Target 1", "min": 600.0, "max": 700.0},
+            ],
+            include_confidence_intervals=False,
+            combination_constraints=[
+                CombinationConstraint(
+                    ("'Factor 1' + 'Factor 2'", operands.FORMULA),
+                    operators.GREATER_THAN,
+                    ("Unknown Column", operands.COLUMN),
+                )
+            ],
+        )
+
+
 def test_analysis_make_optimization_simple_case(
-    test_analysis_with_data, expected_optimization_config
+    test_analysis_with_data, expected_optimization_config_with_combination_constraint
 ):
     """Test that make_optimzation makes expected requests and returns a prediction."""
     pred = test_analysis_with_data.make_optimization(
         "test optimization",
         {
             "goal": "maximize",
             "factor": {"name": "Factor 2", "min": 70.0, "max": 100.0},
         },
         [
             {"name": "Factor 1", "min": 60.0, "max": 200.0},
             {"name": "Target 1", "min": 600.0, "max": 700.0},
         ],
         include_confidence_intervals=False,
+        combination_constraints=[
+            CombinationConstraint(
+                ("'Factor 1' + 'Factor 2'", operands.FORMULA),
+                operators.GREATER_THAN,
+                (150.0, operands.CONSTANT),
+            )
+        ],
     )
 
     assert pred.result_id == "f0123ab1-c6f4-4bd1-b1a6-02896ba57fc7"
     test_analysis_with_data._client.post.assert_called_with(
         f"/api/analyses/{str(test_analysis_with_data.uuid)}/workspaces/",
-        {"request": expected_optimization_config, "visible": False},
+        {
+            "request": expected_optimization_config_with_combination_constraint,
+            "visible": False,
+        },
     )
     test_analysis_with_data._client.get.assert_called()
 
 
 def test_analysis_make_optimization_simple_case_categorical(
     test_analysis_with_data, expected_optimization_config
 ):
```

### Comparing `fero-2.1.9/tests/test_asset.py` & `fero-2.2.0/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `fero-2.1.9/tests/test_client.py` & `fero-2.2.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `fero-2.1.9/tests/test_datasource.py` & `fero-2.2.0/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `fero-2.1.9/tests/test_process.py` & `fero-2.2.0/tests/test_process.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """A module to test `Process` and related classes."""
 
 import pytest
+import requests
 import pandas as pd
 from pandas.testing import assert_frame_equal
 from unittest import mock
 from fero.process import Process, Stage, Tag, DataRequestError
 from io import BytesIO
 
 
@@ -138,15 +139,21 @@
     test_file.close()
     assert_frame_equal(test_df, df)
 
     patched_fero_client.post.assert_has_calls(
         [
             mock.call(
                 f"/api/processes/{process_with_loaded_data.api_id}/download_process_data/",
-                {"request_data": {"tags": ["s1_factor1", "s3_factor1"], "kpis": None}},
+                {
+                    "request_data": {
+                        "tags": ["s1_factor1", "s3_factor1"],
+                        "kpis": None,
+                        "include_batch_id": False,
+                    }
+                },
             ),
             mock.call(
                 f"/api/processes/{process_with_loaded_data.api_id}/download_process_data/",
                 {"request_id": "abcd-1234"},
             ),
         ]
     )
@@ -179,15 +186,48 @@
         process_with_loaded_data.get_data(["s1_factor1", "s3_factor1"])
         assert exc.message == "something bad happened!"
 
     patched_fero_client.post.assert_has_calls(
         [
             mock.call(
                 f"/api/processes/{process_with_loaded_data.api_id}/download_process_data/",
-                {"request_data": {"tags": ["s1_factor1", "s3_factor1"], "kpis": None}},
+                {
+                    "request_data": {
+                        "tags": ["s1_factor1", "s3_factor1"],
+                        "kpis": None,
+                        "include_batch_id": False,
+                    }
+                },
             ),
             mock.call(
                 f"/api/processes/{process_with_loaded_data.api_id}/download_process_data/",
                 {"request_id": "abcd-1234"},
             ),
         ]
     )
+
+
+def test_get_data_raises_bad_status(
+    monkeypatch, process_with_loaded_data, patched_fero_client
+):
+    """Test that an exception is raised for non-2xx status codes."""
+
+    class MockResponse:
+        status_code = 404
+
+        def raise_for_status(self):
+            if 400 <= self.status_code < 600:
+                raise requests.exceptions.HTTPError(response=self)
+
+    def mock_get(*args, **kwargs):
+        return MockResponse()
+
+    def mock_raise_for_status(*args, **kwargs):
+        mock_response.raise_for_status()
+
+    monkeypatch.setattr(requests, "get", mock_get)
+    monkeypatch.setattr(requests.Response, "raise_for_status", mock_raise_for_status)
+    mock_response = MockResponse()
+
+    with pytest.raises(requests.exceptions.HTTPError) as exc:
+        process_with_loaded_data.get_data(["s1_factor1", "s3_factor1"])
+        assert exc.value.response.status_code in range(400, 500)
```

