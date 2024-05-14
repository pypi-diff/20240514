# Comparing `tmp/drepr_v2-1.3.1.tar.gz` & `tmp/drepr_v2-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drepr_v2-1.3.1.tar", max compression
+gzip compressed data, was "drepr_v2-1.3.2.tar", max compression
```

## Comparing `drepr_v2-1.3.1.tar` & `drepr_v2-1.3.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1064 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/LICENSE
--rw-r--r--   0        0        0       53 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/README.md
--rw-r--r--   0        0        0        0 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/__init__.py
--rw-r--r--   0        0        0     3754 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/__main__.py
--rw-r--r--   0        0        0     2051 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/main.py
--rw-r--r--   0        0        0        0 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/__init__.py
--rw-r--r--   0        0        0     4710 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/align.py
--rw-r--r--   0        0        0     1263 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/attr.py
--rw-r--r--   0        0        0    18068 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/drepr.py
--rw-r--r--   0        0        0     3416 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/drepr_builder.py
--rw-r--r--   0        0        0       71 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/format.py
--rw-r--r--   0        0        0     8805 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/parse_v1/__init__.py
--rw-r--r--   0        0        0     5815 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/parse_v1/align_parser.py
--rw-r--r--   0        0        0     4520 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/parse_v1/attr_parser.py
--rw-r--r--   0        0        0     5940 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/parse_v1/path_parser.py
--rw-r--r--   0        0        0     5430 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/parse_v1/preprocessing_parser.py
--rw-r--r--   0        0        0     3255 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/parse_v1/resource_parser.py
--rw-r--r--   0        0        0     7107 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/parse_v1/sm_parser.py
--rw-r--r--   0        0        0     9430 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/parse_v2/__init__.py
--rw-r--r--   0        0        0    11569 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/parse_v2/path_parser.py
--rw-r--r--   0        0        0     9359 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/parse_v2/sm_parser.py
--rw-r--r--   0        0        0     6706 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/path.py
--rw-r--r--   0        0        0      326 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/prelude.py
--rw-r--r--   0        0        0     3917 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/preprocessing.py
--rw-r--r--   0        0        0     2200 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/resource.py
--rw-r--r--   0        0        0     9252 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/models/sm.py
--rw-r--r--   0        0        0        0 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/planning/__init__.py
--rw-r--r--   0        0        0    19809 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/planning/class_map_plan.py
--rw-r--r--   0        0        0    17577 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/planning/drepr_model_alignments.py
--rw-r--r--   0        0        0     4783 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/planning/topological_sorting.py
--rw-r--r--   0        0        0        0 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/program_generation/__init__.py
--rw-r--r--   0        0        0    17908 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/program_generation/alignment_fn.py
--rw-r--r--   0        0        0    23969 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/program_generation/main.py
--rw-r--r--   0        0        0     1569 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/program_generation/predefined_fn.py
--rw-r--r--   0        0        0    16794 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/program_generation/preprocessing.py
--rw-r--r--   0        0        0     1458 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/program_generation/program_space.py
--rw-r--r--   0        0        0     4966 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/program_generation/writers.py
--rw-r--r--   0        0        0        0 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/readers/__init__.py
--rw-r--r--   0        0        0      361 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/readers/csv.py
--rw-r--r--   0        0        0      365 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/readers/json.py
--rw-r--r--   0        0        0      145 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/readers/prelude.py
--rw-r--r--   0        0        0      382 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/readers/spreadsheet.py
--rw-r--r--   0        0        0       61 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/utils/__init__.py
--rw-r--r--   0        0        0     6400 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/utils/attr_data.py
--rw-r--r--   0        0        0     2960 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/utils/misc.py
--rw-r--r--   0        0        0      828 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/utils/namespace_mixin.py
--rw-r--r--   0        0        0      443 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/utils/safe.py
--rw-r--r--   0        0        0     4341 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/utils/udf.py
--rw-r--r--   0        0        0     7798 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/utils/validator.py
--rw-r--r--   0        0        0        0 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/writers/__init__.py
--rw-r--r--   0        0        0     3850 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/writers/base.py
--rw-r--r--   0        0        0     3986 2024-05-13 17:11:03.278864 drepr_v2-1.3.1/drepr/writers/rdfgraph_writer.py
--rw-r--r--   0        0        0      605 2024-05-13 17:11:03.282863 drepr_v2-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 drepr_v2-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-14 02:19:51.865225 drepr_v2-1.3.2/LICENSE
+-rw-r--r--   0        0        0       53 2024-05-14 02:19:51.865225 drepr_v2-1.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 02:19:51.865225 drepr_v2-1.3.2/drepr/__init__.py
+-rw-r--r--   0        0        0     3754 2024-05-14 02:19:51.865225 drepr_v2-1.3.2/drepr/__main__.py
+-rw-r--r--   0        0        0     2063 2024-05-14 02:19:51.865225 drepr_v2-1.3.2/drepr/main.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:19:51.865225 drepr_v2-1.3.2/drepr/models/__init__.py
+-rw-r--r--   0        0        0     4710 2024-05-14 02:19:51.865225 drepr_v2-1.3.2/drepr/models/align.py
+-rw-r--r--   0        0        0     1263 2024-05-14 02:19:51.865225 drepr_v2-1.3.2/drepr/models/attr.py
+-rw-r--r--   0        0        0    12290 2024-05-14 02:19:51.865225 drepr_v2-1.3.2/drepr/models/drepr.py
+-rw-r--r--   0        0        0     3416 2024-05-14 02:19:51.865225 drepr_v2-1.3.2/drepr/models/drepr_builder.py
+-rw-r--r--   0        0        0       71 2024-05-14 02:19:51.865225 drepr_v2-1.3.2/drepr/models/format.py
+-rw-r--r--   0        0        0     8805 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/parse_v1/__init__.py
+-rw-r--r--   0        0        0     5815 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/parse_v1/align_parser.py
+-rw-r--r--   0        0        0     4520 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/parse_v1/attr_parser.py
+-rw-r--r--   0        0        0     5940 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/parse_v1/path_parser.py
+-rw-r--r--   0        0        0     5430 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/parse_v1/preprocessing_parser.py
+-rw-r--r--   0        0        0     3255 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/parse_v1/resource_parser.py
+-rw-r--r--   0        0        0     7107 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/parse_v1/sm_parser.py
+-rw-r--r--   0        0        0     9430 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/parse_v2/__init__.py
+-rw-r--r--   0        0        0    11569 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/parse_v2/path_parser.py
+-rw-r--r--   0        0        0     9359 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/parse_v2/sm_parser.py
+-rw-r--r--   0        0        0     6706 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/path.py
+-rw-r--r--   0        0        0      326 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/prelude.py
+-rw-r--r--   0        0        0     3917 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/preprocessing.py
+-rw-r--r--   0        0        0     2200 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/resource.py
+-rw-r--r--   0        0        0     9252 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/models/sm.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/planning/__init__.py
+-rw-r--r--   0        0        0    19809 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/planning/class_map_plan.py
+-rw-r--r--   0        0        0    17577 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/planning/drepr_model_alignments.py
+-rw-r--r--   0        0        0     4783 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/planning/topological_sorting.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/program_generation/__init__.py
+-rw-r--r--   0        0        0    17908 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/program_generation/alignment_fn.py
+-rw-r--r--   0        0        0    23969 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/program_generation/main.py
+-rw-r--r--   0        0        0     1569 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/program_generation/predefined_fn.py
+-rw-r--r--   0        0        0    16794 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/program_generation/preprocessing.py
+-rw-r--r--   0        0        0     1458 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/program_generation/program_space.py
+-rw-r--r--   0        0        0     4966 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/program_generation/writers.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/readers/__init__.py
+-rw-r--r--   0        0        0      361 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/readers/csv.py
+-rw-r--r--   0        0        0      365 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/readers/json.py
+-rw-r--r--   0        0        0      145 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/readers/prelude.py
+-rw-r--r--   0        0        0      382 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/readers/spreadsheet.py
+-rw-r--r--   0        0        0       61 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/utils/__init__.py
+-rw-r--r--   0        0        0     6400 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/utils/attr_data.py
+-rw-r--r--   0        0        0     2960 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/utils/misc.py
+-rw-r--r--   0        0        0      828 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/utils/namespace_mixin.py
+-rw-r--r--   0        0        0      443 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/utils/safe.py
+-rw-r--r--   0        0        0     4341 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/utils/udf.py
+-rw-r--r--   0        0        0     7798 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/utils/validator.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/writers/__init__.py
+-rw-r--r--   0        0        0     3850 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/writers/base.py
+-rw-r--r--   0        0        0     3986 2024-05-14 02:19:51.869225 drepr_v2-1.3.2/drepr/writers/rdfgraph_writer.py
+-rw-r--r--   0        0        0      605 2024-05-14 02:19:51.873226 drepr_v2-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 drepr_v2-1.3.2/PKG-INFO
```

### Comparing `drepr_v2-1.3.1/LICENSE` & `drepr_v2-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/__main__.py` & `drepr_v2-1.3.2/drepr/__main__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/main.py` & `drepr_v2-1.3.2/drepr/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 import importlib.util
 from pathlib import Path
-from typing import Optional
+from typing import Mapping, Optional
 from uuid import uuid4
 
 from drepr.models.prelude import DRepr, OutputFormat, ResourceData
 from drepr.planning.class_map_plan import ClassesMapExecutionPlan
 from drepr.program_generation.main import FileOutput, MemoryOutput, gen_program
 
 
 def convert(
     repr: DRepr | Path,
-    resources: dict[str, Path | ResourceData],
+    resources: Mapping[str, Path | ResourceData],
     progfile: Optional[Path] = None,
     outfile: Optional[Path] = None,
     format: OutputFormat = OutputFormat.TTL,
     tmpdir: Path = Path("/tmp/drepr"),
     debuginfo: bool = False,
     cleanup: bool = True,
 ):
```

### Comparing `drepr_v2-1.3.1/drepr/models/align.py` & `drepr_v2-1.3.2/drepr/models/align.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/attr.py` & `drepr_v2-1.3.2/drepr/models/attr.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/drepr.py` & `drepr_v2-1.3.2/drepr/models/drepr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from __future__ import annotations
+
 from collections import OrderedDict
 from dataclasses import asdict, dataclass
 from enum import Enum
 from io import StringIO
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Optional, Union
 
 import orjson
 from ruamel.yaml import YAML
 
 from drepr.utils.validator import InputError, Validator
 
 from .align import (
@@ -28,27 +30,27 @@
 
 yaml = YAML()
 yaml.Representer.add_representer(OrderedDict, yaml.Representer.represent_dict)
 
 
 @dataclass
 class EngineFormat:
-    model: Dict[str, Any]
-    edges_optional: List[bool]
-    resource_idmap: Dict[str, int]
-    attribute_idmap: Dict[str, int]
-    sm_node_idmap: Dict[str, int]
+    model: dict[str, Any]
+    edges_optional: list[bool]
+    resource_idmap: dict[str, int]
+    attribute_idmap: dict[str, int]
+    sm_node_idmap: dict[str, int]
 
 
 @dataclass
 class DRepr:
-    resources: List[Resource]
-    preprocessing: List[Preprocessing]
-    attrs: List[Attr]
-    aligns: List[Alignment]
+    resources: list[Resource]
+    preprocessing: list[Preprocessing]
+    attrs: list[Attr]
+    aligns: list[Alignment]
     sm: SemanticModel
 
     @staticmethod
     def parse(raw: dict) -> "DRepr":
         Validator.must_have(raw, "version", "Parsing D-REPR configuration")
         if raw["version"] == "1":
             model = ReprV1Parser.parse(raw)
@@ -73,15 +75,15 @@
 
         raise Exception(
             f"Does not supported this file: {fpath}. Only support json or yaml file"
         )
 
     @staticmethod
     def empty() -> "DRepr":
-        return DRepr([], [], [], [], SemanticModel({}, [], {}))
+        return DRepr([], [], [], [], SemanticModel({}, {}, {}))
 
     @staticmethod
     def deserialize(raw: dict) -> "DRepr":
         resources = [Resource.deserialize(o) for o in raw["resources"]]
         preprocessing = [Preprocessing.deserialize(o) for o in raw["preprocessing"]]
         attrs = [Attr.deserialize(o) for o in raw["attrs"]]
         aligns = []
@@ -221,179 +223,14 @@
 
     def to_lang_yml(self, simplify: bool = True, use_json_path: bool = False) -> str:
         model = self.to_lang_format(simplify, use_json_path)
         out = StringIO()
         yaml.dump(model, out)
         return out.getvalue()
 
-    def to_engine_format(self) -> EngineFormat:
-        """
-        Turn this D-REPR configuration into the format that the engine can read
-        :return:
-        """
-        # map string id to incremental numbers (for resource id and attribute id)
-        ridmap = OrderedDict()
-        for resource in self.resources:
-            ridmap[resource.id] = len(ridmap)
-        for pref in self.preprocessing:
-            if pref.value.output is not None:
-                ridmap[pref.value.output] = len(ridmap)
-        aidmap = OrderedDict()
-        for attr in self.attrs:
-            aidmap[attr.id] = len(aidmap)
-
-        resources = []
-        for res in self.resources:
-            resources.append({"type": res.type.value})
-            if isinstance(res.prop, CSVProp):
-                resources[-1]["value"] = {
-                    "resource_id": ridmap[res.id],
-                    "delimiter": res.prop.delimiter,
-                }
-            else:
-                resources[-1]["value"] = ridmap[res.id]
-
-        preprocessing = []
-        for pref in self.preprocessing:
-            prepro = {
-                "type": pref.type.value,
-                "resource_id": ridmap[pref.value.resource_id],
-                "path": pref.value.path.to_engine_format(),
-                "output": (
-                    ridmap[pref.value.output] if pref.value.output is not None else None
-                ),
-            }
-            if isinstance(pref.value, PMap):
-                prepro["code"] = pref.value.code
-                prepro["change_structure"] = pref.value.change_structure
-            elif isinstance(pref.value, (PFilter, PSplit)):
-                prepro["code"] = pref.value.code
-            elif isinstance(pref.value, RMap):
-                prepro["func_id"] = {"t": pref.value.func_id.value}
-            else:
-                raise NotImplementedError()
-            preprocessing.append(prepro)
-
-        attributes = [
-            {
-                "id": aidmap[a.id],
-                "resource_id": ridmap[a.resource_id],
-                "path": a.path.to_engine_format(),
-                "unique": a.unique,
-                "sorted": a.sorted.value,
-                "vtype": a.value_type.value,
-                "missing_values": [
-                    self._serde_engine_value(v) for v in a.missing_values
-                ],
-            }
-            for a in self.attrs
-        ]
-
-        alignments = []
-        for align in self.aligns:
-            if isinstance(align, RangeAlignment):
-                alignments.append(
-                    {
-                        "type": AlignmentType.Range.value,
-                        "source": aidmap[align.source],
-                        "target": aidmap[align.target],
-                        "aligned_dims": [
-                            {"source": ad.source_idx, "target": ad.target_idx}
-                            for ad in align.aligned_steps
-                        ],
-                    }
-                )
-            elif isinstance(align, ValueAlignment):
-                alignments.append(
-                    {
-                        "type": AlignmentType.Value.value,
-                        "source": aidmap[align.source],
-                        "target": aidmap[align.target],
-                    }
-                )
-            else:
-                raise NotImplementedError()
-
-        engine_sm: Dict[str, Any] = {
-            "nodes": [],
-            "edges": [],
-            "prefixes": [(prefix, uri) for prefix, uri in self.sm.prefixes.items()],
-        }
-        nodes = {"cnodes": [], "dnodes": [], "lnodes": []}
-        for node_id, node in self.sm.nodes.items():
-            if isinstance(node, ClassNode):
-                nodes["cnodes"].append(
-                    {
-                        "type": "class_node",
-                        "node_id": node_id,
-                        "rel_label": node.label,
-                        "abs_label": self.sm.get_abs_iri(node.label),
-                    }
-                )
-            elif isinstance(node, DataNode):
-                nodes["dnodes"].append(
-                    {
-                        "type": "data_node",
-                        "node_id": node_id,
-                        "attr_id": aidmap[node.attr_id],
-                        "data_type": (
-                            node.data_type if node.data_type is not None else None
-                        ),
-                    }
-                )
-            elif isinstance(node, LiteralNode):
-                nodes["lnodes"].append(
-                    {
-                        "type": "literal_node",
-                        "node_id": node_id,
-                        "val": self._serde_engine_value(node.value),
-                        "data_type": (
-                            node.data_type if node.data_type is not None else None
-                        ),
-                    }
-                )
-            else:
-                raise NotImplementedError()
-
-        for k in ["cnodes", "dnodes", "lnodes"]:
-            for n in nodes[k]:
-                engine_sm["nodes"].append(n)
-        nidmap = {}
-        for i, n in enumerate(engine_sm["nodes"]):
-            nidmap[n["node_id"]] = i
-            n["node_id"] = i
-
-        for eid, edge in self.sm.edges.items():
-            engine_sm["edges"].append(
-                {
-                    "edge_id": eid,
-                    "source": nidmap[edge.source_id],
-                    "target": nidmap[edge.target_id],
-                    "rel_label": edge.label,
-                    "abs_label": self.sm.get_abs_iri(edge.label),
-                    "is_subject": edge.is_subject,
-                }
-            )
-
-        edges_optional = [not edge.is_required for edge in self.sm.edges.values()]
-
-        return EngineFormat(
-            {
-                "resources": resources,
-                "preprocessing": preprocessing,
-                "attributes": attributes,
-                "alignments": alignments,
-                "semantic_model": engine_sm,
-            },
-            edges_optional,
-            ridmap,
-            aidmap,
-            nidmap,
-        )
-
     def _serde_engine_value(self, value: Any):
         """Serialize a python value to a json representation of the Value struct in the Rust engine"""
         if value is None:
             return {"t": "Null"}
         elif isinstance(value, bool):
             return {"t": "Bool", "c": value}
         elif isinstance(value, int):
@@ -453,28 +290,36 @@
         if idx is None:
             idx = next(
                 i for i in range(len(self.attrs), -1, -1) if self.attrs[i].id == attr_id
             )
 
         self.attrs.pop(idx)
         for i in range(len(self.aligns) - 1, -1, -1):
-            if self.aligns[i].source == attr_id or self.aligns[i].target == attr_id:
-                self.aligns.pop(i)
+            align = self.aligns[i]
+            if not isinstance(align, AutoAlignment):
+                if align.source == attr_id or align.target == attr_id:
+                    self.aligns.pop(i)
 
         for node in self.sm.nodes:
             if isinstance(node, DataNode) and node.attr_id == attr_id:
                 self.sm.remove_node(node.node_id)
 
     def update_attribute(self, attr_id: str, new_attr: Attr):
         for i, attr in enumerate(self.attrs):
             if attr.id == attr_id:
                 self.attrs[i] = new_attr
 
         for align in self.aligns:
-            if align.source == attr_id:
-                align.source = new_attr.id
-            elif align.target == attr_id:
-                align.target = new_attr.id
+            if isinstance(align, AutoAlignment):
+                if align.attrs is not None:
+                    align.attrs = [
+                        new_attr.id if a == attr_id else a for a in align.attrs
+                    ]
+            else:
+                if align.source == attr_id:
+                    align.source = new_attr.id
+                elif align.target == attr_id:
+                    align.target = new_attr.id
 
         for node in self.sm.nodes:
             if isinstance(node, DataNode) and node.attr_id == attr_id:
                 node.attr_id = new_attr.id
```

### Comparing `drepr_v2-1.3.1/drepr/models/drepr_builder.py` & `drepr_v2-1.3.2/drepr/models/drepr_builder.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/parse_v1/__init__.py` & `drepr_v2-1.3.2/drepr/models/parse_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/parse_v1/align_parser.py` & `drepr_v2-1.3.2/drepr/models/parse_v1/align_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/parse_v1/attr_parser.py` & `drepr_v2-1.3.2/drepr/models/parse_v1/attr_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/parse_v1/path_parser.py` & `drepr_v2-1.3.2/drepr/models/parse_v1/path_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/parse_v1/preprocessing_parser.py` & `drepr_v2-1.3.2/drepr/models/parse_v1/preprocessing_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/parse_v1/resource_parser.py` & `drepr_v2-1.3.2/drepr/models/parse_v1/resource_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/parse_v1/sm_parser.py` & `drepr_v2-1.3.2/drepr/models/parse_v1/sm_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/parse_v2/__init__.py` & `drepr_v2-1.3.2/drepr/models/parse_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/parse_v2/path_parser.py` & `drepr_v2-1.3.2/drepr/models/parse_v2/path_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/parse_v2/sm_parser.py` & `drepr_v2-1.3.2/drepr/models/parse_v2/sm_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/path.py` & `drepr_v2-1.3.2/drepr/models/path.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/preprocessing.py` & `drepr_v2-1.3.2/drepr/models/preprocessing.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/resource.py` & `drepr_v2-1.3.2/drepr/models/resource.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/models/sm.py` & `drepr_v2-1.3.2/drepr/models/sm.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/planning/class_map_plan.py` & `drepr_v2-1.3.2/drepr/planning/class_map_plan.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/planning/drepr_model_alignments.py` & `drepr_v2-1.3.2/drepr/planning/drepr_model_alignments.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/planning/topological_sorting.py` & `drepr_v2-1.3.2/drepr/planning/topological_sorting.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/program_generation/alignment_fn.py` & `drepr_v2-1.3.2/drepr/program_generation/alignment_fn.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/program_generation/main.py` & `drepr_v2-1.3.2/drepr/program_generation/main.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/program_generation/predefined_fn.py` & `drepr_v2-1.3.2/drepr/program_generation/predefined_fn.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/program_generation/preprocessing.py` & `drepr_v2-1.3.2/drepr/program_generation/preprocessing.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/program_generation/program_space.py` & `drepr_v2-1.3.2/drepr/program_generation/program_space.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/program_generation/writers.py` & `drepr_v2-1.3.2/drepr/program_generation/writers.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/utils/attr_data.py` & `drepr_v2-1.3.2/drepr/utils/attr_data.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/utils/misc.py` & `drepr_v2-1.3.2/drepr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/utils/namespace_mixin.py` & `drepr_v2-1.3.2/drepr/utils/namespace_mixin.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/utils/udf.py` & `drepr_v2-1.3.2/drepr/utils/udf.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/utils/validator.py` & `drepr_v2-1.3.2/drepr/utils/validator.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/writers/base.py` & `drepr_v2-1.3.2/drepr/writers/base.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/drepr/writers/rdfgraph_writer.py` & `drepr_v2-1.3.2/drepr/writers/rdfgraph_writer.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.1/pyproject.toml` & `drepr_v2-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drepr-v2"
-version = "1.3.1"
+version = "1.3.2"
 description = ""
 authors = ["Binh Vu <binh@toan2.com>"]
 readme = "README.md"
 packages = [{ include = "drepr" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `drepr_v2-1.3.1/PKG-INFO` & `drepr_v2-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drepr-v2
-Version: 1.3.1
+Version: 1.3.2
 Summary: 
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

