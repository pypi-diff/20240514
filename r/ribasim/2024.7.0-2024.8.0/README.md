# Comparing `tmp/ribasim-2024.7.0.tar.gz` & `tmp/ribasim-2024.8.0.tar.gz`

## Comparing `ribasim-2024.7.0.tar` & `ribasim-2024.8.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/__init__.py
--rw-r--r--   0        0        0    11099 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/config.py
--rw-r--r--   0        0        0    14581 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/input_base.py
--rw-r--r--   0        0        0    17649 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/py.typed
--rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/schemas.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/utils.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/geometry/__init__.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/geometry/area.py
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/geometry/edge.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/geometry/node.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/basin.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/discrete_control.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/flow_boundary.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/flow_demand.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/fractional_flow.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/level_boundary.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/level_demand.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/linear_resistance.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/manning_resistance.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/outlet.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/pid_control.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/pump.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/tabulated_rating_curve.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/terminal.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ribasim-2024.7.0/ribasim/nodes/user_demand.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 ribasim-2024.7.0/tests/conftest.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 ribasim-2024.7.0/tests/test_edge.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 ribasim-2024.7.0/tests/test_input_base.py
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 ribasim-2024.7.0/tests/test_io.py
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 ribasim-2024.7.0/tests/test_model.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ribasim-2024.7.0/tests/test_schemas.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 ribasim-2024.7.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ribasim-2024.7.0/LICENSE
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ribasim-2024.7.0/README.md
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 ribasim-2024.7.0/pyproject.toml
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 ribasim-2024.7.0/PKG-INFO
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/__init__.py
+-rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/config.py
+-rw-r--r--   0        0        0    14581 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/input_base.py
+-rw-r--r--   0        0        0    17317 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/py.typed
+-rw-r--r--   0        0        0    10740 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/schemas.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/utils.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/geometry/__init__.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/geometry/area.py
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/geometry/edge.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/geometry/node.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/__init__.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/basin.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/discrete_control.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/flow_boundary.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/flow_demand.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/fractional_flow.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/level_boundary.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/level_demand.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/linear_resistance.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/manning_resistance.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/outlet.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/pid_control.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/pump.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/tabulated_rating_curve.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/terminal.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ribasim-2024.8.0/ribasim/nodes/user_demand.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 ribasim-2024.8.0/tests/conftest.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 ribasim-2024.8.0/tests/test_edge.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 ribasim-2024.8.0/tests/test_input_base.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 ribasim-2024.8.0/tests/test_io.py
+-rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 ribasim-2024.8.0/tests/test_model.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ribasim-2024.8.0/tests/test_schemas.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 ribasim-2024.8.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ribasim-2024.8.0/LICENSE
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ribasim-2024.8.0/README.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 ribasim-2024.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 ribasim-2024.8.0/PKG-INFO
```

### Comparing `ribasim-2024.7.0/ribasim/config.py` & `ribasim-2024.8.0/ribasim/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,36 +3,41 @@
 from enum import Enum
 from typing import Any
 
 import numpy as np
 import pandas as pd
 import pydantic
 from geopandas import GeoDataFrame
-from pydantic import ConfigDict, Field, model_validator
+from pydantic import ConfigDict, Field, NonNegativeInt, model_validator
 from shapely.geometry import Point
 
 from ribasim.geometry import BasinAreaSchema, NodeTable
 from ribasim.geometry.edge import NodeData
 from ribasim.input_base import ChildModel, NodeModel, SpatialTableModel, TableModel
 
 # These schemas are autogenerated
 from ribasim.schemas import (
+    BasinConcentrationExternalSchema,
+    BasinConcentrationSchema,
+    BasinConcentrationStateSchema,
     BasinProfileSchema,
     BasinStateSchema,
     BasinStaticSchema,
     BasinSubgridSchema,
     BasinTimeSchema,
     DiscreteControlConditionSchema,
     DiscreteControlLogicSchema,
     DiscreteControlVariableSchema,
+    FlowBoundaryConcentrationSchema,
     FlowBoundaryStaticSchema,
     FlowBoundaryTimeSchema,
     FlowDemandStaticSchema,
     FlowDemandTimeSchema,
     FractionalFlowStaticSchema,
+    LevelBoundaryConcentrationSchema,
     LevelBoundaryStaticSchema,
     LevelBoundaryTimeSchema,
     LevelDemandStaticSchema,
     LevelDemandTimeSchema,
     LinearResistanceStaticSchema,
     ManningResistanceStaticSchema,
     OutletStaticSchema,
@@ -83,15 +88,15 @@
 
 class Logging(ChildModel):
     verbosity: Verbosity = Verbosity.info
     timing: bool = False
 
 
 class Node(pydantic.BaseModel):
-    node_id: int
+    node_id: NonNegativeInt
     geometry: Point
     name: str = ""
     subnetwork_id: int | None = None
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     def __init__(self, node_id: int, geometry: Point, **kwargs) -> None:
@@ -185,14 +190,18 @@
         default_factory=TableModel[LevelBoundaryStaticSchema],
         json_schema_extra={"sort_keys": ["node_id"]},
     )
     time: TableModel[LevelBoundaryTimeSchema] = Field(
         default_factory=TableModel[LevelBoundaryTimeSchema],
         json_schema_extra={"sort_keys": ["node_id", "time"]},
     )
+    concentration: TableModel[LevelBoundaryConcentrationSchema] = Field(
+        default_factory=TableModel[LevelBoundaryConcentrationSchema],
+        json_schema_extra={"sort_keys": ["node_id", "substance", "time"]},
+    )
 
 
 class Pump(MultiNodeModel):
     static: TableModel[PumpStaticSchema] = Field(
         default_factory=TableModel[PumpStaticSchema],
         json_schema_extra={"sort_keys": ["node_id", "control_state"]},
     )
@@ -236,14 +245,18 @@
         default_factory=TableModel[FlowBoundaryStaticSchema],
         json_schema_extra={"sort_keys": ["node_id"]},
     )
     time: TableModel[FlowBoundaryTimeSchema] = Field(
         default_factory=TableModel[FlowBoundaryTimeSchema],
         json_schema_extra={"sort_keys": ["node_id", "time"]},
     )
+    concentration: TableModel[FlowBoundaryConcentrationSchema] = Field(
+        default_factory=TableModel[FlowBoundaryConcentrationSchema],
+        json_schema_extra={"sort_keys": ["node_id", "substance", "time"]},
+    )
 
 
 class FlowDemand(MultiNodeModel):
     static: TableModel[FlowDemandStaticSchema] = Field(
         default_factory=TableModel[FlowDemandStaticSchema],
         json_schema_extra={"sort_keys": ["node_id"]},
     )
@@ -274,14 +287,26 @@
         default_factory=TableModel[BasinSubgridSchema],
         json_schema_extra={"sort_keys": ["subgrid_id", "basin_level"]},
     )
     area: SpatialTableModel[BasinAreaSchema] = Field(
         default_factory=SpatialTableModel[BasinAreaSchema],
         json_schema_extra={"sort_keys": ["node_id"]},
     )
+    concentration: TableModel[BasinConcentrationSchema] = Field(
+        default_factory=TableModel[BasinConcentrationSchema],
+        json_schema_extra={"sort_keys": ["node_id", "substance", "time"]},
+    )
+    concentration_external: TableModel[BasinConcentrationExternalSchema] = Field(
+        default_factory=TableModel[BasinConcentrationExternalSchema],
+        json_schema_extra={"sort_keys": ["node_id", "substance", "time"]},
+    )
+    concentration_state: TableModel[BasinConcentrationStateSchema] = Field(
+        default_factory=TableModel[BasinConcentrationStateSchema],
+        json_schema_extra={"sort_keys": ["node_id", "substance"]},
+    )
 
 
 class ManningResistance(MultiNodeModel):
     static: TableModel[ManningResistanceStaticSchema] = Field(
         default_factory=TableModel[ManningResistanceStaticSchema],
         json_schema_extra={"sort_keys": ["node_id", "control_state"]},
     )
```

### Comparing `ribasim-2024.7.0/ribasim/input_base.py` & `ribasim-2024.8.0/ribasim/input_base.py`

 * *Files identical despite different names*

### Comparing `ribasim-2024.7.0/ribasim/model.py` & `ribasim-2024.8.0/ribasim/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -166,14 +166,15 @@
         db_path = directory / input_dir / "database.gpkg"
         db_path.parent.mkdir(parents=True, exist_ok=True)
         db_path.unlink(missing_ok=True)
         context_file_loading.get()["database"] = db_path
         self.edge._save(directory, input_dir)
 
         node = self.node_table()
+        assert node.df is not None
         # Temporarily require unique node_id for #1262
         # and copy them to the fid for #1306.
         if not node.df["node_id"].is_unique:
             raise ValueError("node_id must be unique")
         node.df.set_index("node_id", drop=False, inplace=True)
         node.df.index.name = "fid"
         node.df.sort_index(inplace=True)
@@ -199,18 +200,19 @@
             for table in sub._tables():
                 if isinstance(table, SpatialTableModel) and table.df is not None:
                     table.df = getattr(table.df, function_name)(crs)
         self.crs = crs
 
     def node_table(self) -> NodeTable:
         """Compute the full NodeTable from all node types."""
-        df_chunks = [node.node.df.set_crs(self.crs) for node in self._nodes()]
+        df_chunks = [node.node.df.set_crs(self.crs) for node in self._nodes()]  # type: ignore
         df = pd.concat(df_chunks, ignore_index=True)
         node_table = NodeTable(df=df)
         node_table.sort()
+        assert node_table.df is not None
         node_table.df.index.name = "fid"
         return node_table
 
     def _nodes(self) -> Generator[MultiNodeModel, Any, None]:
         """Return all non-empty MultiNodeModel instances."""
         for key in self.model_fields.keys():
             attr = getattr(self, key)
@@ -225,31 +227,14 @@
     def _children(self):
         return {
             k: getattr(self, k)
             for k in self.model_fields.keys()
             if isinstance(getattr(self, k), ChildModel)
         }
 
-    def validate_model_node_field_ids(self):
-        raise NotImplementedError()
-
-    def validate_model_node_ids(self):
-        raise NotImplementedError()
-
-    def validate_model(self):
-        """Validate the model.
-
-        Checks:
-        - Whether the node IDs of the node_type fields are valid
-        - Whether the node IDs in the node field correspond to the node IDs on the node type fields
-        """
-
-        self.validate_model_node_field_ids()
-        self.validate_model_node_ids()
-
     @classmethod
     def read(cls, filepath: str | PathLike[str]) -> "Model":
         """Read model from TOML file."""
         return cls(filepath=filepath)  # type: ignore
 
     def write(self, filepath: str | PathLike[str]) -> Path:
         """
@@ -399,21 +384,23 @@
         """
         Convert the network and results to a `xugrid.UgridDataset`.
         To get the network only, set `add_results=False`.
         This method will throw `ImportError`,
         if the optional dependency `xugrid` isn't installed.
         """
         node_df = self.node_table().df
+        assert node_df is not None
 
         # This will need to be adopted for locally unique node IDs,
         # otherwise the `node_lookup` with `argsort` is not correct.
         if not node_df.node_id.is_unique:
             raise ValueError("node_id must be unique")
         node_df.sort_values("node_id", inplace=True)
 
+        assert self.edge.df is not None
         edge_df = self.edge.df.copy()
         # We assume only the flow network is of interest.
         edge_df = edge_df[edge_df.edge_type == "flow"]
 
         node_id = node_df.node_id.to_numpy()
         edge_id = edge_df.index.to_numpy()
         from_node_id = edge_df.from_node_id.to_numpy()
```

### Comparing `ribasim-2024.7.0/ribasim/schemas.py` & `ribasim-2024.8.0/ribasim/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,35 @@
 
 class _BaseSchema(pa.DataFrameModel):
     class Config:
         add_missing_columns = True
         coerce = True
 
 
+class BasinConcentrationExternalSchema(_BaseSchema):
+    node_id: Series[Int32] = pa.Field(nullable=False, default=0)
+    time: Series[Timestamp] = pa.Field(nullable=False)
+    substance: Series[str] = pa.Field(nullable=False)
+    concentration: Series[float] = pa.Field(nullable=True)
+
+
+class BasinConcentrationStateSchema(_BaseSchema):
+    node_id: Series[Int32] = pa.Field(nullable=False, default=0)
+    substance: Series[str] = pa.Field(nullable=False)
+    concentration: Series[float] = pa.Field(nullable=True)
+
+
+class BasinConcentrationSchema(_BaseSchema):
+    node_id: Series[Int32] = pa.Field(nullable=False, default=0)
+    time: Series[Timestamp] = pa.Field(nullable=False)
+    substance: Series[str] = pa.Field(nullable=False)
+    drainage: Series[float] = pa.Field(nullable=True)
+    precipitation: Series[float] = pa.Field(nullable=True)
+
+
 class BasinProfileSchema(_BaseSchema):
     node_id: Series[Int32] = pa.Field(nullable=False, default=0)
     area: Series[float] = pa.Field(nullable=False)
     level: Series[float] = pa.Field(nullable=False)
 
 
 class BasinStateSchema(_BaseSchema):
@@ -66,14 +87,21 @@
     listen_node_type: Series[str] = pa.Field(nullable=False)
     listen_node_id: Series[Int32] = pa.Field(nullable=False, default=0)
     variable: Series[str] = pa.Field(nullable=False)
     weight: Series[float] = pa.Field(nullable=True)
     look_ahead: Series[float] = pa.Field(nullable=True)
 
 
+class FlowBoundaryConcentrationSchema(_BaseSchema):
+    node_id: Series[Int32] = pa.Field(nullable=False, default=0)
+    time: Series[Timestamp] = pa.Field(nullable=False)
+    substance: Series[str] = pa.Field(nullable=False)
+    concentration: Series[float] = pa.Field(nullable=False)
+
+
 class FlowBoundaryStaticSchema(_BaseSchema):
     node_id: Series[Int32] = pa.Field(nullable=False, default=0)
     active: Series[pa.BOOL] = pa.Field(nullable=True)
     flow_rate: Series[float] = pa.Field(nullable=False)
 
 
 class FlowBoundaryTimeSchema(_BaseSchema):
@@ -97,38 +125,45 @@
 
 class FractionalFlowStaticSchema(_BaseSchema):
     node_id: Series[Int32] = pa.Field(nullable=False, default=0)
     fraction: Series[float] = pa.Field(nullable=False)
     control_state: Series[str] = pa.Field(nullable=True)
 
 
+class LevelBoundaryConcentrationSchema(_BaseSchema):
+    node_id: Series[Int32] = pa.Field(nullable=False, default=0)
+    time: Series[Timestamp] = pa.Field(nullable=False)
+    substance: Series[str] = pa.Field(nullable=False)
+    concentration: Series[float] = pa.Field(nullable=False)
+
+
 class LevelBoundaryStaticSchema(_BaseSchema):
     node_id: Series[Int32] = pa.Field(nullable=False, default=0)
     active: Series[pa.BOOL] = pa.Field(nullable=True)
     level: Series[float] = pa.Field(nullable=False)
 
 
 class LevelBoundaryTimeSchema(_BaseSchema):
     node_id: Series[Int32] = pa.Field(nullable=False, default=0)
     time: Series[Timestamp] = pa.Field(nullable=False)
     level: Series[float] = pa.Field(nullable=False)
 
 
 class LevelDemandStaticSchema(_BaseSchema):
     node_id: Series[Int32] = pa.Field(nullable=False, default=0)
-    min_level: Series[float] = pa.Field(nullable=False)
-    max_level: Series[float] = pa.Field(nullable=False)
+    min_level: Series[float] = pa.Field(nullable=True)
+    max_level: Series[float] = pa.Field(nullable=True)
     priority: Series[Int32] = pa.Field(nullable=False, default=0)
 
 
 class LevelDemandTimeSchema(_BaseSchema):
     node_id: Series[Int32] = pa.Field(nullable=False, default=0)
     time: Series[Timestamp] = pa.Field(nullable=False)
-    min_level: Series[float] = pa.Field(nullable=False)
-    max_level: Series[float] = pa.Field(nullable=False)
+    min_level: Series[float] = pa.Field(nullable=True)
+    max_level: Series[float] = pa.Field(nullable=True)
     priority: Series[Int32] = pa.Field(nullable=False, default=0)
 
 
 class LinearResistanceStaticSchema(_BaseSchema):
     node_id: Series[Int32] = pa.Field(nullable=False, default=0)
     active: Series[pa.BOOL] = pa.Field(nullable=True)
     resistance: Series[float] = pa.Field(nullable=False)
```

### Comparing `ribasim-2024.7.0/ribasim/geometry/edge.py` & `ribasim-2024.8.0/ribasim/geometry/edge.py`

 * *Files identical despite different names*

### Comparing `ribasim-2024.7.0/ribasim/geometry/node.py` & `ribasim-2024.8.0/ribasim/geometry/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from ribasim.input_base import SpatialTableModel
 
 __all__ = ("NodeTable",)
 
 
 class NodeSchema(pa.SchemaModel):
-    node_id: Series[Int32]
+    node_id: Series[Int32] = pa.Field(ge=0)
     name: Series[str] = pa.Field(default="")
     node_type: Series[str] = pa.Field(default="")
     subnetwork_id: Series[pd.Int32Dtype] = pa.Field(
         default=pd.NA, nullable=True, coerce=True
     )
     geometry: GeoSeries[Any] = pa.Field(default=None, nullable=True)
```

### Comparing `ribasim-2024.7.0/ribasim/nodes/__init__.py` & `ribasim-2024.8.0/ribasim/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `ribasim-2024.7.0/ribasim/nodes/basin.py` & `ribasim-2024.8.0/ribasim/nodes/basin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 from geopandas import GeoDataFrame
 from pandas import DataFrame
 
 from ribasim.geometry.area import BasinAreaSchema
 from ribasim.input_base import TableModel
 from ribasim.schemas import (
+    BasinConcentrationExternalSchema,
+    BasinConcentrationSchema,
+    BasinConcentrationStateSchema,
     BasinProfileSchema,
     BasinStateSchema,
     BasinStaticSchema,
     BasinSubgridSchema,
     BasinTimeSchema,
 )
 
-__all__ = ["Static", "Time", "State", "Profile", "Subgrid", "Area"]
+__all__ = [
+    "Static",
+    "Time",
+    "State",
+    "Profile",
+    "Subgrid",
+    "Area",
+    "Concentration",
+]
 
 
 class Static(TableModel[BasinStaticSchema]):
     def __init__(self, **kwargs):
         super().__init__(df=DataFrame(dict(**kwargs)))
 
 
@@ -38,7 +49,22 @@
     def __init__(self, **kwargs):
         super().__init__(df=DataFrame(dict(**kwargs)))
 
 
 class Area(TableModel[BasinAreaSchema]):
     def __init__(self, **kwargs):
         super().__init__(df=GeoDataFrame(dict(**kwargs)))
+
+
+class Concentration(TableModel[BasinConcentrationSchema]):
+    def __init__(self, **kwargs):
+        super().__init__(df=GeoDataFrame(dict(**kwargs)))
+
+
+class ConcentrationExternal(TableModel[BasinConcentrationExternalSchema]):
+    def __init__(self, **kwargs):
+        super().__init__(df=GeoDataFrame(dict(**kwargs)))
+
+
+class ConcentrationState(TableModel[BasinConcentrationStateSchema]):
+    def __init__(self, **kwargs):
+        super().__init__(df=GeoDataFrame(dict(**kwargs)))
```

### Comparing `ribasim-2024.7.0/ribasim/nodes/discrete_control.py` & `ribasim-2024.8.0/ribasim/nodes/discrete_control.py`

 * *Files identical despite different names*

### Comparing `ribasim-2024.7.0/tests/conftest.py` & `ribasim-2024.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ribasim-2024.7.0/tests/test_edge.py` & `ribasim-2024.8.0/tests/test_edge.py`

 * *Files identical despite different names*

### Comparing `ribasim-2024.7.0/tests/test_io.py` & `ribasim-2024.8.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `ribasim-2024.7.0/tests/test_model.py` & `ribasim-2024.8.0/tests/test_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 import xugrid
 from pydantic import ValidationError
 from pyproj import CRS
+from ribasim import Node
 from ribasim.config import Solver
 from ribasim.geometry.edge import NodeData
 from ribasim.input_base import esc_id
 from ribasim.model import Model
 from shapely import Point
 
 
@@ -61,32 +62,20 @@
     model = basic
     model.solver.saveat = 86400.0
     d = model.model_dump(exclude_unset=True, exclude_none=True, by_alias=True)
     assert "solver" in d
     assert d["solver"]["saveat"] == 86400.0
 
 
-@pytest.mark.xfail(reason="Needs implementation")
-def test_invalid_node_id(basic):
-    model = basic
-
-    # Add entry with invalid node ID
-    df = model.pump.static.df._append(
-        {"flow_rate": 1, "node_id": -1, "active": True},
-        ignore_index=True,
-    )
-    # Currently can't handle mixed NaN and None in a DataFrame
-    df = df.where(pd.notna(df), None)
-    model.pump.static.df = df
-
+def test_invalid_node_id():
     with pytest.raises(
         ValueError,
-        match=re.escape("Node IDs must be non-negative integers, got [-1]."),
+        match=r".* Input should be greater than or equal to 0 .*",
     ):
-        model.validate_model_node_field_ids()
+        Node(-1, Point(7.0, 7.0))
 
 
 @pytest.mark.xfail(reason="Should be reimplemented by the .add() API.")
 def test_node_id_duplicate(basic):
     model = basic
 
     # Add duplicate node ID
```

### Comparing `ribasim-2024.7.0/.gitignore` & `ribasim-2024.8.0/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # Files generated by invoking Julia with --code-coverage
 *.jl.cov
 *.jl.*.cov
 
 # Files generated by invoking Julia with --track-allocation
 *.jl.mem
 
-# Build artifacts for creating documentation generated by the Documenter package
-docs/build/
-docs/site/
-
 /generated_testmodels
-build/ribasim_cli/
-build/libribasim/
+build/ribasim/
+build/cli/target
 
 JuliaSysimage.dll
 LocalPreferences.toml
 .ipynb_checkpoints
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
```

### Comparing `ribasim-2024.7.0/LICENSE` & `ribasim-2024.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ribasim-2024.7.0/README.md` & `ribasim-2024.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ribasim-2024.7.0/pyproject.toml` & `ribasim-2024.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 requires-python = ">=3.10"
 dependencies = [
     "geopandas",
     "matplotlib",
     "numpy",
     "pandas",
-    "pandera != 0.16.0",
+    "pandera >= 0.18",
     "pyarrow",
     "pydantic ~= 2.0",
     "pyogrio",
     "shapely >= 2.0",
     "tomli",
     "tomli-w",
 ]
```

### Comparing `ribasim-2024.7.0/PKG-INFO` & `ribasim-2024.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.3
 Name: ribasim
-Version: 2024.7.0
+Version: 2024.8.0
 Summary: Pre- and post-process Ribasim
 Project-URL: Documentation, https://deltares.github.io/Ribasim
 Project-URL: Source, https://github.com/Deltares/Ribasim
 Author-email: Deltares and contributors <ribasim.info@deltares.nl>
 License: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.10
 Requires-Dist: geopandas
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: pandera!=0.16.0
+Requires-Dist: pandera>=0.18
 Requires-Dist: pyarrow
 Requires-Dist: pydantic~=2.0
 Requires-Dist: pyogrio
 Requires-Dist: shapely>=2.0
 Requires-Dist: tomli
 Requires-Dist: tomli-w
 Provides-Extra: tests
```

