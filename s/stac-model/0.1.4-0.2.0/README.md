# Comparing `tmp/stac_model-0.1.4.tar.gz` & `tmp/stac_model-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_model-0.1.4.tar", max compression
+gzip compressed data, was "stac_model-0.2.0.tar", max compression
```

## Comparing `stac_model-0.1.4.tar` & `stac_model-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-05-13 16:59:06.677350 stac_model-0.1.4/LICENSE
--rw-r--r--   0        0        0     3688 2024-05-13 16:59:06.677350 stac_model-0.1.4/README_STAC_MODEL.md
--rw-r--r--   0        0        0     8013 2024-05-13 16:59:06.677350 stac_model-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      265 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/__init__.py
--rw-r--r--   0        0        0     1215 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/__main__.py
--rw-r--r--   0        0        0     3035 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/base.py
--rw-r--r--   0        0        0     7036 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/examples.py
--rw-r--r--   0        0        0     2026 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/input.py
--rw-r--r--   0        0        0     3007 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/output.py
--rw-r--r--   0        0        0     1476 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/runtime.py
--rw-r--r--   0        0        0     9408 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/schema.py
--rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 stac_model-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-14 19:36:29.795580 stac_model-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3679 2024-05-14 19:36:29.795580 stac_model-0.2.0/README_STAC_MODEL.md
+-rw-r--r--   0        0        0     8060 2024-05-14 19:36:29.795580 stac_model-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      265 2024-05-14 19:36:29.795580 stac_model-0.2.0/stac_model/__init__.py
+-rw-r--r--   0        0        0     1215 2024-05-14 19:36:29.795580 stac_model-0.2.0/stac_model/__main__.py
+-rw-r--r--   0        0        0     3038 2024-05-14 19:36:29.795580 stac_model-0.2.0/stac_model/base.py
+-rw-r--r--   0        0        0     7083 2024-05-14 19:36:29.795580 stac_model-0.2.0/stac_model/examples.py
+-rw-r--r--   0        0        0     3838 2024-05-14 19:36:29.795580 stac_model-0.2.0/stac_model/input.py
+-rw-r--r--   0        0        0     3007 2024-05-14 19:36:29.795580 stac_model-0.2.0/stac_model/output.py
+-rw-r--r--   0        0        0     1476 2024-05-14 19:36:29.799581 stac_model-0.2.0/stac_model/runtime.py
+-rw-r--r--   0        0        0     9432 2024-05-14 19:36:29.799581 stac_model-0.2.0/stac_model/schema.py
+-rw-r--r--   0        0        0     5472 1970-01-01 00:00:00.000000 stac_model-0.2.0/PKG-INFO
```

### Comparing `stac_model-0.1.4/LICENSE` & `stac_model-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.4/README_STAC_MODEL.md` & `stac_model-0.2.0/README_STAC_MODEL.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 [![Semantic versions][blic3]][bp5]
 [![Pipelines][bscm6]][bscm7]
 
 _A PydanticV2 and PySTAC validation and serialization library for the STAC ML Model Extension_
 
 </div>
 
-> :warning: <br>
+> ⚠️ <br>
 > FIXME: update description with ML framework connectors (pytorch, scikit-learn, etc.)
 
 ## Installation
 
 ```shell
 pip install -U stac-model
 ```
@@ -45,25 +45,25 @@
 
 ```shell
 stac-model
 ```
 
 This will make [this example item](./examples/item_basic.json) for an example model.
 
-## :chart_with_upwards_trend: Releases
+## 📈 Releases
 
 You can see the list of available releases on the [GitHub Releases][github-releases] page.
 
-## :page_facing_up:  License
+## 📄 License
 [![License][blic1]][blic2]
 
 This project is licenced under the terms of the `Apache Software License 2.0` licence.
 See [LICENSE][blic2] for more details.
 
-## :heartpulse: Credits
+## 💗 Credits
 [![Python project templated from galactipy.][bp6]][bp7]
 
 <!-- Anchors -->
 
 [bp1]: https://img.shields.io/pypi/pyversions/stac-model?style=for-the-badge
 [bp2]: https://pypi.org/project/stac-model/
 [bp3]: https://img.shields.io/pypi/v/stac-model?style=for-the-badge&logo=pypi&color=3775a9
@@ -82,17 +82,17 @@
 [blic1]: https://img.shields.io/github/license/crim-ca/mlm-extension?style=for-the-badge
 [blic2]: https://github.com/crim-ca/mlm-extension/blob/main/LICENSE
 [blic3]: https://img.shields.io/badge/%F0%9F%93%A6-semantic%20versions-4053D6?style=for-the-badge
 
 [github-releases]: https://github.com/crim-ca/mlm-extension/releases
 
 [bscm1]: https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white
-[bscm2]: https://img.shields.io/github/v/release/crim-ca/mlm-extension?style=for-the-badge&logo=semantic-release&color=347d39
-[bscm6]: https://img.shields.io/github/actions/workflow/status/crim-ca/mlm-extension/build.yml?style=for-the-badge&logo=github
-[bscm7]: https://github.com/crim-ca/mlm-extension/actions/workflows/build.yml
+[bscm2]: https://img.shields.io/github/v/release/crim-ca/mlm-extension?filter=stac-model-v*&style=for-the-badge&logo=semantic-release&color=347d39
+[bscm6]: https://img.shields.io/github/actions/workflow/status/crim-ca/mlm-extension/publish.yaml?style=for-the-badge&logo=github
+[bscm7]: https://github.com/crim-ca/mlm-extension/blob/main/.github/workflows/publish.yaml
 
 [hub1]: https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuring-dependabot-version-updates#enabling-dependabot-version-updates
 [hub2]: https://github.com/marketplace/actions/close-stale-issues
 [hub6]: https://docs.github.com/en/code-security/dependabot
 [hub8]: https://github.com/crim-ca/mlm-extension/blob/main/.github/release-drafter.yml
 [hub9]: https://github.com/crim-ca/mlm-extension/blob/main/.github/.stale.yml
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stac_model-0.1.4/pyproject.toml` & `stac_model-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "stac-model"
-version = "0.1.4"
+version = "0.2.0"
 description = "A PydanticV2 validation and serialization libary for the STAC ML Model Extension"
 readme = "README_STAC_MODEL.md"
 authors = [
   "Ryan Avery <ryan@wherobots.com>",
   "Francis Charette-Migneault <francis.charette-migneault@crim.ca>"
 ]
 license = "Apache Software License 2.0"
@@ -91,15 +91,15 @@
 
 [tool.bumpversion]
 # NOTE:
 #   Although these definitions are provided in this 'stac-model' project file,
 #   they are actually intented for versioning the MLM specification itself.
 #   To version 'stac-model', use the 'poetry version' operations.
 #   See also https://github.com/crim-ca/mlm-extension/blob/main/CONTRIBUTING.md#building-and-releasing
-current_version = "1.1.0"
+current_version = "1.2.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = true
 ignore_missing_files = false
@@ -220,14 +220,15 @@
     # isort
     "I",
 ]
 
 [tool.ruff.lint.isort]
 known-local-folder = ["tests", "conftest"]
 known-first-party = ["stac_model"]
+extra-standard-library = ["typing_extensions"]
 
 [tool.mypy]
 # https://github.com/python/mypy
 # https://mypy.readthedocs.io/en/latest/config_file.html#using-a-pyproject-toml-file
 python_version = "3.10"
 pretty = true
 show_traceback = true
```

### Comparing `stac_model-0.1.4/stac_model/__main__.py` & `stac_model-0.2.0/stac_model/__main__.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.4/stac_model/base.py` & `stac_model-0.2.0/stac_model/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,11 +112,11 @@
     "super-resolution",
 ]
 
 
 ModelTask = Union[ModelTaskNames, TaskEnum]
 
 
-class ProcessingExpression(BaseModel):
+class ProcessingExpression(MLMBaseModel):
     # FIXME: should use 'pystac' reference, but 'processing' extension is not implemented yet!
     format: str
     expression: Any
```

### Comparing `stac_model-0.1.4/stac_model/examples.py` & `stac_model-0.2.0/stac_model/examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,18 @@
         404.91978886,
         4.77584468,
         1002.58768311,
         761.30323499,
         1231.58581042,
     ]
     stats = [
-        MLMStatistic(mean=mean, stddev=stddev)
+        MLMStatistic(
+            mean=mean,
+            stddev=stddev,
+        )
         for mean, stddev in zip(stats_mean, stats_stddev)
     ]
     model_input = ModelInput(
         name="13 Band Sentinel-2 Batch",
         bands=band_names,
         input=input_struct,
         norm_by_channel=True,
@@ -78,30 +81,33 @@
             format="python",
             expression="torchgeo.datamodules.eurosat.EuroSATDataModule.collate_fn",
         ),  # noqa: E501
     )
     result_struct = ModelResult(
         shape=[-1, 10],
         dim_order=["batch", "class"],
-        data_type="float32"
+        data_type="float32",
     )
     class_map = {
         "Annual Crop": 0,
         "Forest": 1,
         "Herbaceous Vegetation": 2,
         "Highway": 3,
         "Industrial Buildings": 4,
         "Pasture": 5,
         "Permanent Crop": 6,
         "Residential Buildings": 7,
         "River": 8,
         "SeaLake": 9,
     }
     class_objects = [
-        MLMClassification(value=class_value, name=class_name)
+        MLMClassification(
+            value=class_value,
+            name=class_name,
+        )
         for class_name, class_value in class_map.items()
     ]
     model_output = ModelOutput(
         name="classification",
         tasks={"classification"},
         classes=class_objects,
         result=result_struct,
@@ -115,27 +121,27 @@
                 "imagery with Eurosat landcover labels with torchgeo."
             ),
             href="https://huggingface.co/torchgeo/resnet18_sentinel2_all_moco/resolve/main/resnet18_sentinel2_all_moco-59bfdff9.pth",
             media_type="application/octet-stream; application=pytorch",
             roles=[
                 "mlm:model",
                 "mlm:weights",
-                "data"
-            ]
+                "data",
+            ],
         ),
         "source_code": pystac.Asset(
             title="Model implementation.",
             description="Source code to run the model.",
             href="https://github.com/microsoft/torchgeo/blob/61efd2e2c4df7ebe3bd03002ebbaeaa3cfe9885a/torchgeo/models/resnet.py#L207",
             media_type="text/x-python",
             roles=[
                 "mlm:model",
-                "code"
-            ]
-        )
+                "code",
+            ],
+        ),
     }
 
     ml_model_size = 43000000
     ml_model_meta = MLModelProperties(
         name="Resnet-18 Sentinel-2 ALL MOCO",
         architecture="ResNet-18",
         tasks={"classification"},
@@ -159,31 +165,29 @@
     end_datetime_str = "9999-01-01"  # cannot be None, invalid against STAC Core!
     start_datetime = parse_dt(start_datetime_str).isoformat() + "Z"
     end_datetime = parse_dt(end_datetime_str).isoformat() + "Z"
     bbox = [
         -7.882190080512502,
         37.13739173208318,
         27.911651652899923,
-        58.21798141355221
+        58.21798141355221,
     ]
     geometry = shapely.geometry.Polygon.from_bounds(*bbox).__geo_interface__
     item_name = "item_basic"
     col_name = "ml-model-examples"
     item = pystac.Item(
         id=item_name,
         collection=col_name,
         geometry=geometry,
         bbox=bbox,
         datetime=None,
         properties={
             "start_datetime": start_datetime,
             "end_datetime": end_datetime,
-            "description": (
-                "Sourced from torchgeo python library, identifier is ResNet18_Weights.SENTINEL2_ALL_MOCO"
-            ),
+            "description": "Sourced from torchgeo python library, identifier is ResNet18_Weights.SENTINEL2_ALL_MOCO",
         },
         assets=assets,
     )
 
     # note: cannot use 'item.add_derived_from' since it expects a 'Item' object, but we refer to a 'Collection' here
     # item.add_derived_from("https://earth-search.aws.element84.com/v1/collections/sentinel-2-l2a")
     item.add_link(
@@ -198,22 +202,22 @@
     col = pystac.Collection(
         id=col_name,
         title="Machine Learning Model examples",
         description="Collection of items contained in the Machine Learning Model examples.",
         extent=pystac.Extent(
             temporal=pystac.TemporalExtent([[parse_dt(start_datetime), parse_dt(end_datetime)]]),
             spatial=pystac.SpatialExtent([bbox]),
-        )
+        ),
     )
     col.set_self_href("./examples/collection.json")
     col.add_item(item)
     item.set_self_href(f"./examples/{item_name}.json")
 
     model_asset = cast(
         FileExtension[pystac.Asset],
-        pystac.extensions.file.FileExtension.ext(assets["model"], add_if_missing=True)
+        pystac.extensions.file.FileExtension.ext(assets["model"], add_if_missing=True),
     )
     model_asset.apply(size=ml_model_size)
 
     item_mlm = MLModelExtension.ext(item, add_if_missing=True)
     item_mlm.apply(ml_model_meta.model_dump(by_alias=True, exclude_unset=True, exclude_defaults=True))
     return item_mlm
```

### Comparing `stac_model-0.1.4/stac_model/output.py` & `stac_model-0.2.0/stac_model/output.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.4/stac_model/runtime.py` & `stac_model-0.2.0/stac_model/runtime.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.4/stac_model/schema.py` & `stac_model-0.2.0/stac_model/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "T",
     pystac.Collection,
     pystac.Item,
     pystac.Asset,  # item_assets.AssetDefinition,
 )
 
 SchemaName = Literal["mlm"]
-SCHEMA_URI: str = "https://crim-ca.github.io/mlm-extension/v1.1.0/schema.json"
+SCHEMA_URI: str = "https://crim-ca.github.io/mlm-extension/v1.2.0/schema.json"
 PREFIX = f"{get_args(SchemaName)[0]}:"
 
 
 def mlm_prefix_adder(field_name: str) -> str:
     return "mlm:" + field_name
 
 
@@ -93,23 +93,26 @@
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @overload
     @classmethod
-    def ext(cls, obj: pystac.Asset, add_if_missing: bool = False) -> "AssetMLModelExtension": ...
+    def ext(cls, obj: pystac.Asset, add_if_missing: bool = False) -> "AssetMLModelExtension":
+        ...
 
     @overload
     @classmethod
-    def ext(cls, obj: pystac.Item, add_if_missing: bool = False) -> "ItemMLModelExtension": ...
+    def ext(cls, obj: pystac.Item, add_if_missing: bool = False) -> "ItemMLModelExtension":
+        ...
 
     @overload
     @classmethod
-    def ext(cls, obj: pystac.Collection, add_if_missing: bool = False) -> "CollectionMLModelExtension": ...
+    def ext(cls, obj: pystac.Collection, add_if_missing: bool = False) -> "CollectionMLModelExtension":
+        ...
 
     # @overload
     # @classmethod
     # def ext(cls, obj: item_assets.AssetDefinition, add_if_missing: bool = False) -> "ItemAssetsMLModelExtension":
     #     ...
 
     @classmethod
```

### Comparing `stac_model-0.1.4/PKG-INFO` & `stac_model-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-model
-Version: 0.1.4
+Version: 0.2.0
 Summary: A PydanticV2 validation and serialization libary for the STAC ML Model Extension
 Home-page: https://github.com/crim-ca/mlm-extension/blob/main/README_STAC_MODEL.md
 License: Apache Software License 2.0
 Author: Ryan Avery
 Author-email: ryan@wherobots.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -56,15 +56,15 @@
 [![Semantic versions][blic3]][bp5]
 [![Pipelines][bscm6]][bscm7]
 
 _A PydanticV2 and PySTAC validation and serialization library for the STAC ML Model Extension_
 
 </div>
 
-> :warning: <br>
+> ⚠️ <br>
 > FIXME: update description with ML framework connectors (pytorch, scikit-learn, etc.)
 
 ## Installation
 
 ```shell
 pip install -U stac-model
 ```
@@ -84,25 +84,25 @@
 
 ```shell
 stac-model
 ```
 
 This will make [this example item](./examples/item_basic.json) for an example model.
 
-## :chart_with_upwards_trend: Releases
+## 📈 Releases
 
 You can see the list of available releases on the [GitHub Releases][github-releases] page.
 
-## :page_facing_up:  License
+## 📄 License
 [![License][blic1]][blic2]
 
 This project is licenced under the terms of the `Apache Software License 2.0` licence.
 See [LICENSE][blic2] for more details.
 
-## :heartpulse: Credits
+## 💗 Credits
 [![Python project templated from galactipy.][bp6]][bp7]
 
 <!-- Anchors -->
 
 [bp1]: https://img.shields.io/pypi/pyversions/stac-model?style=for-the-badge
 [bp2]: https://pypi.org/project/stac-model/
 [bp3]: https://img.shields.io/pypi/v/stac-model?style=for-the-badge&logo=pypi&color=3775a9
@@ -121,17 +121,17 @@
 [blic1]: https://img.shields.io/github/license/crim-ca/mlm-extension?style=for-the-badge
 [blic2]: https://github.com/crim-ca/mlm-extension/blob/main/LICENSE
 [blic3]: https://img.shields.io/badge/%F0%9F%93%A6-semantic%20versions-4053D6?style=for-the-badge
 
 [github-releases]: https://github.com/crim-ca/mlm-extension/releases
 
 [bscm1]: https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white
-[bscm2]: https://img.shields.io/github/v/release/crim-ca/mlm-extension?style=for-the-badge&logo=semantic-release&color=347d39
-[bscm6]: https://img.shields.io/github/actions/workflow/status/crim-ca/mlm-extension/build.yml?style=for-the-badge&logo=github
-[bscm7]: https://github.com/crim-ca/mlm-extension/actions/workflows/build.yml
+[bscm2]: https://img.shields.io/github/v/release/crim-ca/mlm-extension?filter=stac-model-v*&style=for-the-badge&logo=semantic-release&color=347d39
+[bscm6]: https://img.shields.io/github/actions/workflow/status/crim-ca/mlm-extension/publish.yaml?style=for-the-badge&logo=github
+[bscm7]: https://github.com/crim-ca/mlm-extension/blob/main/.github/workflows/publish.yaml
 
 [hub1]: https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuring-dependabot-version-updates#enabling-dependabot-version-updates
 [hub2]: https://github.com/marketplace/actions/close-stale-issues
 [hub6]: https://docs.github.com/en/code-security/dependabot
 [hub8]: https://github.com/crim-ca/mlm-extension/blob/main/.github/release-drafter.yml
 [hub9]: https://github.com/crim-ca/mlm-extension/blob/main/.github/.stale.yml
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

