# Comparing `tmp/spinedb_api-0.31.0.tar.gz` & `tmp/spinedb_api-0.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinedb_api-0.31.0.tar", last modified: Tue Apr 30 07:31:12 2024, max compression
+gzip compressed data, was "spinedb_api-0.31.1.tar", last modified: Tue May 14 13:12:11 2024, max compression
```

## Comparing `spinedb_api-0.31.0.tar` & `spinedb_api-0.31.1.tar`

### file list

```diff
@@ -1,195 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.765573 spinedb_api-0.31.0/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.737573 spinedb_api-0.31.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.737573 spinedb_api-0.31.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/.github/workflows/run_unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    32493 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-30 07:31:12.765573 spinedb_api-0.31.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.737573 spinedb_api-0.31.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/benchmarks/datetime_from_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/benchmarks/map_from_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/benchmarks/mapped_item_getitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/benchmarks/update_default_value_to_different_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/benchmarks/update_default_value_to_same_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.737573 spinedb_api-0.31.0/bin/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/bin/build_doc.bat
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/bin/build_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/deploy-key.enc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.737573 spinedb_api-0.31.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.741573 spinedb_api-0.31.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/docs/source/front_matter.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.741573 spinedb_api-0.31.0/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/docs/source/img/spinetoolbox_on_wht.svg
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/docs/source/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12306 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/docs/source/parameter_value_format.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/docs/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.741573 spinedb_api-0.31.0/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    55634 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/fig/eu-emblem-low-res.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:31:12.765573 spinedb_api-0.31.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.745573 spinedb_api-0.31.0/spinedb_api/
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.745573 spinedb_api-0.31.0/spinedb_api/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/README
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.749573 spinedb_api-0.31.0/spinedb_api/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/5385f063bef2_create_superclass_subclass_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/6b7c994c1c61_drop_object_and_relationship_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/8b0eff478bcb_add_active_by_default_to_entity_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/ce9faa82ed59_create_entity_alternative_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    45892 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/db_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    48172 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/db_mapping_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/db_mapping_commit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    63433 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/db_mapping_query_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/export_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.749573 spinedb_api-0.31.0/spinedb_api/export_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/export_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53281 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/export_mapping/export_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/export_mapping/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/export_mapping/group_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/export_mapping/pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/export_mapping/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.749573 spinedb_api-0.31.0/spinedb_api/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/filters/alternative_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/filters/execution_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/filters/renamer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/filters/scenario_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/filters/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/filters/value_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/graph_layout_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    33569 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28826 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/import_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.753573 spinedb_api-0.31.0/spinedb_api/import_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/import_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15737 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/import_mapping/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    39773 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/import_mapping/import_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/import_mapping/import_mapping_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/import_mapping/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    34047 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/mapped_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    60563 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/perfect_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/purge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/server_client_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_db_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28277 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_db_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.753573 spinedb_api-0.31.0/spinedb_api/spine_io/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.753573 spinedb_api-0.31.0/spinedb_api/spine_io/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/exporters/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/exporters/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/exporters/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/exporters/gdx_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/exporters/sql_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/exporters/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/gdx_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.753573 spinedb_api-0.31.0/spinedb_api/spine_io/importers/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/importers/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/importers/datapackage_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/importers/excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/importers/gdx_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/importers/json_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/importers/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/spine_io/importers/sqlalchemy_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/spinedb_api/temp_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-30 07:31:12.000000 spinedb_api-0.31.0/spinedb_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.765573 spinedb_api-0.31.0/spinedb_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-30 07:31:12.000000 spinedb_api-0.31.0/spinedb_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-04-30 07:31:12.000000 spinedb_api-0.31.0/spinedb_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:31:12.000000 spinedb_api-0.31.0/spinedb_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:31:12.000000 spinedb_api-0.31.0/spinedb_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-30 07:31:12.000000 spinedb_api-0.31.0/spinedb_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 07:31:12.000000 spinedb_api-0.31.0/spinedb_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.757573 spinedb_api-0.31.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/custom_db_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.757573 spinedb_api-0.31.0/tests/export_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/export_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77801 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/export_mapping/test_export_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/export_mapping/test_pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/export_mapping/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.761573 spinedb_api-0.31.0/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/filters/test_alternative_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/filters/test_execution_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/filters/test_renamer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27281 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/filters/test_scenario_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/filters/test_tool_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/filters/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/filters/test_value_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.761573 spinedb_api-0.31.0/tests/import_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/import_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/import_mapping/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    87939 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/import_mapping/test_import_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/import_mapping/test_type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.761573 spinedb_api-0.31.0/tests/spine_io/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.761573 spinedb_api-0.31.0/tests/spine_io/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/exporters/test_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/exporters/test_excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15994 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/exporters/test_gdx_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12163 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/exporters/test_sql_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/exporters/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:31:12.765573 spinedb_api-0.31.0/tests/spine_io/importers/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/importers/test_CSVConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/importers/test_GdxConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/importers/test_datapackage_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/importers/test_excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/importers/test_json_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/importers/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/importers/test_sqlalchemy_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/spine_io/test_excel_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)   192142 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/test_DatabaseMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/test_check_integrity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/test_db_mapping_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/test_db_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/test_export_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    77621 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/test_import_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    48629 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/test_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-30 07:31:06.000000 spinedb_api-0.31.0/tests/test_purge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.519268 spinedb_api-0.31.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.487267 spinedb_api-0.31.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.487267 spinedb_api-0.31.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/.github/workflows/run_unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32493 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-14 13:12:11.519268 spinedb_api-0.31.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.487267 spinedb_api-0.31.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/datetime_from_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/map_from_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/mapped_item_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/update_default_value_to_different_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/update_default_value_to_same_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.491267 spinedb_api-0.31.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/bin/build_doc.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/bin/build_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/deploy-key.enc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.491267 spinedb_api-0.31.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.491267 spinedb_api-0.31.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/front_matter.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.491267 spinedb_api-0.31.1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/img/spinetoolbox_on_wht.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12306 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/parameter_value_format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/docs/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.491267 spinedb_api-0.31.1/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)    55634 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/fig/eu-emblem-low-res.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:12:11.519268 spinedb_api-0.31.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.495267 spinedb_api-0.31.1/spinedb_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.499267 spinedb_api-0.31.1/spinedb_api/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/README
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.499267 spinedb_api-0.31.1/spinedb_api/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/5385f063bef2_create_superclass_subclass_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/6b7c994c1c61_drop_object_and_relationship_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/8b0eff478bcb_add_active_by_default_to_entity_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19947 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/ce9faa82ed59_create_entity_alternative_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/e010777927a5_change_active_by_default_server_default_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    10900 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45893 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/db_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48172 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/db_mapping_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/db_mapping_commit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63433 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/db_mapping_query_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.503267 spinedb_api-0.31.1/spinedb_api/export_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52885 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_mapping/export_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_mapping/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_mapping/group_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_mapping/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22267 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/export_mapping/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.503267 spinedb_api-0.31.1/spinedb_api/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/alternative_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/execution_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/renamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/scenario_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/filters/value_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/graph_layout_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28826 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/import_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.503267 spinedb_api-0.31.1/spinedb_api/import_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/import_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15737 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/import_mapping/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39612 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/import_mapping/import_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/import_mapping/import_mapping_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/import_mapping/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34426 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/mapped_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60563 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/perfect_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/purge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/server_client_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28277 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_db_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.503267 spinedb_api-0.31.1/spinedb_api/spine_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.507268 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/gdx_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/sql_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/exporters/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/gdx_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.507268 spinedb_api-0.31.1/spinedb_api/spine_io/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/datapackage_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/gdx_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/spine_io/importers/sqlalchemy_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/spinedb_api/temp_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.515268 spinedb_api-0.31.1/spinedb_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 13:12:11.000000 spinedb_api-0.31.1/spinedb_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.511268 spinedb_api-0.31.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/custom_db_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.511268 spinedb_api-0.31.1/tests/export_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/export_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77130 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/export_mapping/test_export_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/export_mapping/test_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/export_mapping/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.511268 spinedb_api-0.31.1/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_alternative_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_execution_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_renamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27281 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_scenario_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_tool_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/filters/test_value_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.515268 spinedb_api-0.31.1/tests/import_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/import_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27529 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/import_mapping/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87795 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/import_mapping/test_import_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/import_mapping/test_type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.515268 spinedb_api-0.31.1/tests/spine_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.515268 spinedb_api-0.31.1/tests/spine_io/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/exporters/test_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/exporters/test_excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15994 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/exporters/test_gdx_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12163 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/exporters/test_sql_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/exporters/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:12:11.515268 spinedb_api-0.31.1/tests/spine_io/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_CSVConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_GdxConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_datapackage_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/importers/test_sqlalchemy_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/spine_io/test_excel_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)   198916 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_DatabaseMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_check_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_db_mapping_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_db_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_export_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78082 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_import_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48629 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-14 13:12:04.000000 spinedb_api-0.31.1/tests/test_purge.py
```

### Comparing `spinedb_api-0.31.0/.github/workflows/run_unit_tests.yml` & `spinedb_api-0.31.1/.github/workflows/run_unit_tests.yml`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,18 @@
         fetch-depth: 0
     - name: Version from Git tags
       run: git describe --tags
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
+        cache: pip
+        cache-dependency-path: |
+          requirements.txt
+          pyproject.toml
     - name: Display Python version
       run:
          python -c "import sys; print(sys.version)"
     - name: Install unixodbc
       if: runner.os == 'Linux'
       run:
         sudo apt-get install -y unixodbc-dev  # Install to get sql.h headers
@@ -67,14 +71,18 @@
       with:
         repository: spine-tools/Spine-Toolbox
         fetch-depth: 0
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
+        cache: pip
+        cache-dependency-path: |
+          requirements.txt
+          pyproject.toml
     - name: Install additional packages for Linux
       if: runner.os == 'Linux'
       run: |
         sudo apt-get update -y
         sudo apt-get install -y libegl1
     - name: Install dependencies
       env:
@@ -108,14 +116,18 @@
     - uses: actions/checkout@v4
       with:
         repository: spine-tools/Spine-Toolbox
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
+        cache: pip
+        cache-dependency-path: |
+          requirements.txt
+          pyproject.toml
     - name: Install additional packages for Linux
       if: runner.os == 'Linux'
       run: |
         sudo apt-get update -y
         sudo apt-get install -y libegl1
     - name: Install dependencies
       env:
```

### Comparing `spinedb_api-0.31.0/.readthedocs.yml` & `spinedb_api-0.31.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/CHANGELOG.md` & `spinedb_api-0.31.1/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,26 @@
 
 ### Removed
 
 ### Deprecated
 
 ### Security
 
+## 0.31.1
+
+### Changed
+
+- The server default of `active_by_default` is now `True`.
+
+### Removed
+
+- `ScenarioActiveFlag` import and export mappings have been removed.
+  While the flag column is still in the database schema, it is not used anywhere,
+  nor is it accessible e.g. in Toolbox.
+
 ## 0.31.0
 
 This is the first release where we keep a Spine-Database-API specific changelog.
 
 The database structure has changed quite a bit.
 Large parts of the API have been rewritten or replaced by new systems.
 We are still keeping many old entry points for backwards compatibility,
```

### Comparing `spinedb_api-0.31.0/COPYING` & `spinedb_api-0.31.1/COPYING`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/COPYING.LESSER` & `spinedb_api-0.31.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/PKG-INFO` & `spinedb_api-0.31.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinedb_api
-Version: 0.31.0
+Version: 0.31.1
 Summary: An API to talk to Spine databases.
 Author-email: Spine Project consortium <spine_info@vtt.fi>
 License: LGPL-3.0-or-later
 Project-URL: Repository, https://github.com/spine-tools/Spine-Database-API
 Keywords: energy system modelling,workflow,optimisation,database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spinedb_api Version: 0.31.0 Summary: An API to talk
+Metadata-Version: 2.1 Name: spinedb_api Version: 0.31.1 Summary: An API to talk
 to Spine databases. Author-email: Spine Project consortium
 vtt.fi> License: LGPL-3.0-or-later Project-URL: Repository, https://github.com/
 spine-tools/Spine-Database-API Keywords: energy system
 modelling,workflow,optimisation,database Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: >=3.8.1 Description-Content-Type: text/markdown License-File: COPYING
```

### Comparing `spinedb_api-0.31.0/README.md` & `spinedb_api-0.31.1/README.md`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/benchmarks/README.md` & `spinedb_api-0.31.1/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/benchmarks/datetime_from_database.py` & `spinedb_api-0.31.1/benchmarks/datetime_from_database.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/benchmarks/map_from_database.py` & `spinedb_api-0.31.1/benchmarks/map_from_database.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/benchmarks/mapped_item_getitem.py` & `spinedb_api-0.31.1/benchmarks/mapped_item_getitem.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/benchmarks/update_default_value_to_different_value.py` & `spinedb_api-0.31.1/benchmarks/update_default_value_to_different_value.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/benchmarks/update_default_value_to_same_value.py` & `spinedb_api-0.31.1/benchmarks/update_default_value_to_same_value.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/benchmarks/utils.py` & `spinedb_api-0.31.1/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/deploy-key.enc` & `spinedb_api-0.31.1/deploy-key.enc`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/docs/Makefile` & `spinedb_api-0.31.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/docs/make.bat` & `spinedb_api-0.31.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/docs/source/conf.py` & `spinedb_api-0.31.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/docs/source/front_matter.rst` & `spinedb_api-0.31.1/docs/source/front_matter.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/docs/source/img/spinetoolbox_on_wht.svg` & `spinedb_api-0.31.1/docs/source/img/spinetoolbox_on_wht.svg`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/docs/source/index.rst` & `spinedb_api-0.31.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/docs/source/metadata.rst` & `spinedb_api-0.31.1/docs/source/metadata.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/docs/source/parameter_value_format.rst` & `spinedb_api-0.31.1/docs/source/parameter_value_format.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/docs/source/tutorial.rst` & `spinedb_api-0.31.1/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/fig/eu-emblem-low-res.jpg` & `spinedb_api-0.31.1/fig/eu-emblem-low-res.jpg`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/pylintrc` & `spinedb_api-0.31.1/pylintrc`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/pyproject.toml` & `spinedb_api-0.31.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -61,8 +61,8 @@
 branch = true
 
 [tool.coverage.report]
 ignore_errors = true
 
 [tool.black]
 line-length = 120
-exclude = '\.git'
+exclude = '\.git|version.py'
```

### Comparing `spinedb_api-0.31.0/spinedb_api/__init__.py` & `spinedb_api-0.31.1/spinedb_api/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/env.py` & `spinedb_api-0.31.1/spinedb_api/alembic/env.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """drop category tables
 
 Revision ID: 070a0eb89e88
 Revises: bba1e2ef5153
 Create Date: 2019-09-20 13:04:52.423483
 
 """
+
 from alembic import op
 import sqlalchemy as sa
 
 
 # revision identifiers, used by Alembic.
 revision = "070a0eb89e88"
 down_revision = "bba1e2ef5153"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Add list_value table
 
 Revision ID: 0c7d199ae915
 Revises: 7d0b467f2f4e
 Create Date: 2022-03-07 14:55:32.802765
 
 """
+
 from alembic import op
 import sqlalchemy as sa
 from sqlalchemy.ext.automap import automap_base
 from sqlalchemy.orm import sessionmaker
 from spinedb_api.helpers import LONGTEXT_LENGTH
 
 # revision identifiers, used by Alembic.
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """create metadata tables
 
 Revision ID: 1892adebc00f
 Revises: defbda3bf2b5
 Create Date: 2020-10-05 14:51:13.787685
 
 """
+
 from alembic import op
 import sqlalchemy as sa
 
 
 # revision identifiers, used by Alembic.
 revision = "1892adebc00f"
 down_revision = "defbda3bf2b5"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # revision identifiers, used by Alembic.
 revision = "1e4997105288"
 down_revision = "fbb540efbf15"
 branch_labels = None
 depends_on = None
 
-LONGTEXT_LENGTH = 2 ** 32 - 1
+LONGTEXT_LENGTH = 2**32 - 1
 
 
 def upgrade():
     conn = op.get_bind()
     Session = sessionmaker(bind=conn)
     session = Session()
     Base = automap_base()
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """add alternatives and scenarios
 
 Revision ID: 39e860a11b05
 Revises: 9da58d2def22
 Create Date: 2020-03-05 14:04:00.854936
 
 """
+
 from datetime import datetime, timezone
 from alembic import op
 import sqlalchemy as sa
 from sqlalchemy.ext.automap import automap_base
 from sqlalchemy.orm import sessionmaker
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Add parameter_tag, parameter_definition_tag, and parameter_value_list
 
 Revision ID: 51fd7b69acf7
 Revises: 8c19c53d5701
 Create Date: 2019-01-25 15:47:05.100028
 
 """
+
 from alembic import op
 import sqlalchemy as sa
 
 
 # revision identifiers, used by Alembic.
 revision = "51fd7b69acf7"
 down_revision = "8c19c53d5701"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/5385f063bef2_create_superclass_subclass_table.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/5385f063bef2_create_superclass_subclass_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """create superclass_subclass table
 
 Revision ID: 5385f063bef2
 Revises: ce9faa82ed59
 Create Date: 2023-10-30 17:11:23.316879
 
 """
+
 from alembic import op
 import sqlalchemy as sa
 
 
 # revision identifiers, used by Alembic.
 revision = "5385f063bef2"
 down_revision = "ce9faa82ed59"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/6b7c994c1c61_drop_object_and_relationship_tables.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/6b7c994c1c61_drop_object_and_relationship_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """drop_object_and_relationship_tables
 
 Revision ID: 6b7c994c1c61
 Revises: 989fccf80441
 Create Date: 2023-02-09 06:48:46.585108
 
 """
+
 from alembic import op
 import sqlalchemy as sa
 from spinedb_api.helpers import naming_convention
 
 # revision identifiers, used by Alembic.
 revision = "6b7c994c1c61"
 down_revision = "989fccf80441"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """fix foreign key constraints in object and relationship tables
 
 Revision ID: 738d494a08ac
 Revises: 1e4997105288
 Create Date: 2022-01-05 09:18:48.858784
 
 """
+
 from alembic import op
 from spinedb_api.helpers import naming_convention
 
 
 # revision identifiers, used by Alembic.
 revision = "738d494a08ac"
 down_revision = "1e4997105288"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """fix foreign key constraints in entity classes
 
 Revision ID: 7d0b467f2f4e
 Revises: fd542cebf699
 Create Date: 2022-02-15 15:41:06.794006
 
 """
+
 from alembic import op
 from spinedb_api.helpers import naming_convention
 
 
 # revision identifiers, used by Alembic.
 revision = "7d0b467f2f4e"
 down_revision = "fd542cebf699"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/8b0eff478bcb_add_active_by_default_to_entity_class.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/8b0eff478bcb_add_active_by_default_to_entity_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """add active_by_default to entity_class
 
 Revision ID: 8b0eff478bcb
 Revises: 5385f063bef2
 Create Date: 2024-01-12 09:55:08.934574
 
 """
+
 from alembic import op
 import sqlalchemy as sa
 import sqlalchemy.orm
 
 from spinedb_api.compatibility import convert_tool_feature_method_to_active_by_default
 
 # revision identifiers, used by Alembic.
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """rename parameter to parameter_definition
 
 Revision ID: 8c19c53d5701
 Revises:
 Create Date: 2019-01-24 16:47:21.493240
 
 """
+
 from alembic import op
 import sqlalchemy as sa
 
 naming_convention = {
     "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
     "uq": "uq_%(table_name)s_%(column_0N_name)s",
 }
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Replace values with reference to list values
 
 Revision ID: 989fccf80441
 Revises: 0c7d199ae915
 Create Date: 2022-03-14 11:33:13.777028
 
 """
+
 from alembic import op
 from sqlalchemy import MetaData
 from sqlalchemy.sql.expression import bindparam
 from sqlalchemy.orm import sessionmaker
 from spinedb_api.parameter_value import dump_db_value, from_database, ParameterValueFormatError
 from spinedb_api.helpers import group_concat
 from spinedb_api.exception import SpineIntegrityError
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """create entity_group_table
 
 Revision ID: 9da58d2def22
 Revises: 070a0eb89e88
 Create Date: 2020-06-09 21:31:07.912724
 
 """
+
 from alembic import op
 import sqlalchemy as sa
 
 
 # revision identifiers, used by Alembic.
 revision = "9da58d2def22"
 down_revision = "070a0eb89e88"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """move to entity based design
 
 Revision ID: bba1e2ef5153
 Revises: bf255c179bce
 Create Date: 2019-09-17 13:38:53.437119
 
 """
+
 from datetime import datetime
 from alembic import op
 import sqlalchemy as sa
 
 
 # revision identifiers, used by Alembic.
 revision = "bba1e2ef5153"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """get rid of unused fields in parameter tables and update unique constraints
 
 Revision ID: bf255c179bce
 Revises: 51fd7b69acf7
 Create Date: 2019-03-26 15:34:26.550171
 
 """
+
 from alembic import op
 import sqlalchemy as sa
 
 naming_convention = {
     "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
     "uq": "uq_%(table_name)s_%(column_0N_name)s",
 }
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/ce9faa82ed59_create_entity_alternative_table.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/ce9faa82ed59_create_entity_alternative_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """create entity_alternative table
 
 Revision ID: ce9faa82ed59
 Revises: 6b7c994c1c61
 Create Date: 2023-09-21 14:35:28.867803
 
 """
+
 from alembic import op
 import sqlalchemy as sa
 from spinedb_api.compatibility import convert_tool_feature_method_to_entity_alternative
 
 
 # revision identifiers, used by Alembic.
 revision = "ce9faa82ed59"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """add tool feature tables
 
 Revision ID: defbda3bf2b5
 Revises: 39e860a11b05
 Create Date: 2020-09-01 20:12:57.300147
 
 """
+
 from alembic import op
 import sqlalchemy as sa
 
 
 # revision identifiers, used by Alembic.
 revision = "defbda3bf2b5"
 down_revision = "39e860a11b05"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """add support for mysql
 
 Revision ID: fbb540efbf15
 Revises: 1892adebc00f
 Create Date: 2021-01-05 10:40:16.720937
 
 """
+
 from alembic import op
 from sqlalchemy import Text
 from spinedb_api.helpers import LONGTEXT_LENGTH, naming_convention
 
 
 # revision identifiers, used by Alembic.
 revision = "fbb540efbf15"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py` & `spinedb_api-0.31.1/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """drop on update clauses from object and relationship foreign key constraints
 
 Revision ID: fd542cebf699
 Revises: 738d494a08ac
 Create Date: 2022-01-05 11:00:31.154790
 
 """
+
 from alembic import op
 from spinedb_api.helpers import naming_convention
 
 
 # revision identifiers, used by Alembic.
 revision = "fd542cebf699"
 down_revision = "738d494a08ac"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/alembic.ini` & `spinedb_api-0.31.1/spinedb_api/alembic.ini`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/compatibility.py` & `spinedb_api-0.31.1/spinedb_api/compatibility.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,38 +77,30 @@
             ).where(pd_table.c.id.in_(lv_id_by_pdef_id))
         )
     ]
     # Compute new active_by_default values from 'is_active' default values,
     # where active_by_default is True if the value of 'is_active' is the one from the tool_feature_method specification
     entity_class_items_to_update = {
         x["entity_class_id"]: {
-            "active_by_default": False
-            if x["list_value_id"] is None
-            else x["list_value_id"] == lv_id_by_pdef_id[x["parameter_definition_id"]],
+            "active_by_default": (
+                False
+                if x["list_value_id"] is None
+                else x["list_value_id"] == lv_id_by_pdef_id[x["parameter_definition_id"]]
+            ),
         }
         for x in is_active_default_vals
     }
     updated_items = []
     entity_class_table = meta.tables["entity_class"]
     update_statement = entity_class_table.update()
     for class_id, update in entity_class_items_to_update.items():
         if apply:
             conn.execute(update_statement.where(entity_class_table.c.id == class_id), update)
         update["id"] = class_id
         updated_items.append(update)
-    parameter_definitions_to_update = (
-        x["parameter_definition_id"] for x in is_active_default_vals if x["list_value_id"] is not None
-    )
-    update_statement = pd_table.update()
-    for definition_id in parameter_definitions_to_update:
-        update = {"default_value": None, "default_type": None}
-        if apply:
-            conn.execute(update_statement.where(pd_table.c.id == definition_id), update)
-        update["id"] = definition_id
-        updated_items.append(update)
     return [], updated_items, []
 
 
 def convert_tool_feature_method_to_entity_alternative(conn, use_existing_tool_feature_method, apply):
     """Transforms parameter_value rows into entity_alternative rows, whenever the former are used in a tool filter
     to control entity activity.
```

### Comparing `spinedb_api-0.31.0/spinedb_api/db_mapping.py` & `spinedb_api-0.31.1/spinedb_api/db_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -873,14 +873,15 @@
     setattr(DatabaseMapping, "get_" + it + "_items", partialmethod(DatabaseMapping.get_items, it))
     setattr(DatabaseMapping, "add_" + it + "_item", partialmethod(DatabaseMapping.add_item, it))
     setattr(DatabaseMapping, "update_" + it + "_item", partialmethod(DatabaseMapping.update_item, it))
     setattr(DatabaseMapping, "add_update_" + it + "_item", partialmethod(DatabaseMapping.add_update_item, it))
     setattr(DatabaseMapping, "remove_" + it + "_item", partialmethod(DatabaseMapping.remove_item, it))
     setattr(DatabaseMapping, "restore_" + it + "_item", partialmethod(DatabaseMapping.restore_item, it))
 
+
 # Astroid transform so DatabaseMapping looks like it has the convenience methods defined above
 def _add_convenience_methods(node):
     if node.name != "DatabaseMapping":
         return node
 
     def _a(item_type):
         return "an" if any(item_type.lower().startswith(x) for x in "aeiou") else "a"
```

### Comparing `spinedb_api-0.31.0/spinedb_api/db_mapping_base.py` & `spinedb_api-0.31.1/spinedb_api/db_mapping_base.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/db_mapping_commit_mixin.py` & `spinedb_api-0.31.1/spinedb_api/db_mapping_commit_mixin.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/db_mapping_query_mixin.py` & `spinedb_api-0.31.1/spinedb_api/db_mapping_query_mixin.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/exception.py` & `spinedb_api-0.31.1/spinedb_api/exception.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/export_functions.py` & `spinedb_api-0.31.1/spinedb_api/export_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/export_mapping/__init__.py` & `spinedb_api-0.31.1/spinedb_api/export_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/export_mapping/export_mapping.py` & `spinedb_api-0.31.1/spinedb_api/export_mapping/export_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1316,34 +1316,14 @@
         return "scenario_name"
 
     @staticmethod
     def id_field():
         return "scenario_id"
 
 
-class ScenarioActiveFlagMapping(ExportMapping):
-    """Maps scenario active flags.
-
-    Cannot be used as the topmost mapping; must have a :class:`ScenarioMapping` as parent.
-    """
-
-    MAP_TYPE = "ScenarioActiveFlag"
-
-    def add_query_columns(self, db_map, query):
-        return query.add_columns(db_map.scenario_sq.c.active)
-
-    @staticmethod
-    def name_field():
-        return "active"
-
-    @staticmethod
-    def id_field():
-        return "active"
-
-
 class ScenarioAlternativeMapping(ExportMapping):
     """Maps scenario alternatives.
 
     Cannot be used as the topmost mapping; must have a :class:`ScenarioMapping` as parent.
     """
 
     MAP_TYPE = "ScenarioAlternative"
@@ -1553,16 +1533,14 @@
             ParameterDefaultValueTypeMapping,
             ParameterDefinitionMapping,
             ParameterValueIndexMapping,
             ParameterValueListMapping,
             ParameterValueListValueMapping,
             ParameterValueMapping,
             ParameterValueTypeMapping,
-            ScenarioActiveFlagMapping,
-            ScenarioAlternativeMapping,
             ScenarioBeforeAlternativeMapping,
             ScenarioDescriptionMapping,
             ScenarioMapping,
             # FIXME
             # FeatureEntityClassMapping,
             # FeatureParameterDefinitionMapping,
             # ToolMapping,
@@ -1585,14 +1563,17 @@
         "RelationshipObject": ElementMapping,
         "RelationshipClassObjectHighlightingMapping": EntityClassMapping,
         "RelationshipObjectHighlightingMapping": ElementMapping,
     }
     mappings.update(legacy_mappings)
     flattened = list()
     for mapping_dict in serialized:
+        if mapping_dict["map_type"] == "ScenarioActiveFlag":
+            # We don't support active flag exporting anymore.
+            continue
         if (highlight_position := mapping_dict.get("highlight_dimension")) is not None:
             # legacy
             mapping_dict["highlight_position"] = highlight_position
         position = mapping_dict["position"]
         if isinstance(position, str):
             position = Position(position)
         ignorable = mapping_dict.get("ignorable", False)
```

### Comparing `spinedb_api-0.31.0/spinedb_api/export_mapping/generator.py` & `spinedb_api-0.31.1/spinedb_api/export_mapping/generator.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/export_mapping/group_functions.py` & `spinedb_api-0.31.1/spinedb_api/export_mapping/group_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/export_mapping/pivot.py` & `spinedb_api-0.31.1/spinedb_api/export_mapping/pivot.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/export_mapping/settings.py` & `spinedb_api-0.31.1/spinedb_api/export_mapping/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 # Spine Database API is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser
 # General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
 # option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-"""
-Contains convenience functions to set up different database export schemes.
-
-"""
+""" Contains convenience functions to set up different database export schemes. """
 from itertools import takewhile
 
 from .export_mapping import (
     AlternativeMapping,
     AlternativeDescriptionMapping,
     DimensionMapping,
     ElementMapping,
@@ -31,15 +28,14 @@
     ParameterDefinitionMapping,
     ParameterValueIndexMapping,
     ParameterValueListMapping,
     ParameterValueListValueMapping,
     ParameterValueMapping,
     ParameterValueTypeMapping,
     Position,
-    ScenarioActiveFlagMapping,
     ScenarioAlternativeMapping,
     ScenarioBeforeAlternativeMapping,
     ScenarioMapping,
     ScenarioDescriptionMapping,
     IndexNameMapping,
     DefaultValueIndexNameMapping,
     ParameterDefaultValueTypeMapping,
@@ -317,31 +313,28 @@
     alt_mapping = AlternativeMapping(alternative_position)
     alt_mapping.child = AlternativeDescriptionMapping(alternative_description_position)
     return alt_mapping
 
 
 def scenario_export(
     scenario_position=Position.hidden,
-    scenario_active_flag_position=Position.hidden,
     scenario_description_position=Position.hidden,
 ):
     """
     Sets up export mappings for exporting scenarios.
 
     Args:
         scenario_position (int or Position): position of scenarios
-        scenario_active_flag_position (int or Position): position of scenario active flags
         scenario_description_position (int or Position): position of descriptions
 
     Returns:
         Mapping: root mapping
     """
     scenario_mapping = ScenarioMapping(scenario_position)
-    active_flag_mapping = scenario_mapping.child = ScenarioActiveFlagMapping(scenario_active_flag_position)
-    active_flag_mapping.child = ScenarioDescriptionMapping(scenario_description_position)
+    scenario_mapping.child = ScenarioDescriptionMapping(scenario_description_position)
     return scenario_mapping
 
 
 def scenario_alternative_export(
     scenario_position=Position.hidden, alternative_position=Position.hidden, before_alternative_position=Position.hidden
 ):
     """
```

### Comparing `spinedb_api-0.31.0/spinedb_api/filters/__init__.py` & `spinedb_api-0.31.1/spinedb_api/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/filters/alternative_filter.py` & `spinedb_api-0.31.1/spinedb_api/filters/alternative_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/filters/execution_filter.py` & `spinedb_api-0.31.1/spinedb_api/filters/execution_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/filters/renamer.py` & `spinedb_api-0.31.1/spinedb_api/filters/renamer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/filters/scenario_filter.py` & `spinedb_api-0.31.1/spinedb_api/filters/scenario_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/filters/tools.py` & `spinedb_api-0.31.1/spinedb_api/filters/tools.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/filters/value_transformer.py` & `spinedb_api-0.31.1/spinedb_api/filters/value_transformer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/graph_layout_generator.py` & `spinedb_api-0.31.1/spinedb_api/graph_layout_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         for ind, pos in self.heavy_positions.items():
             heavy_ind_list.append(ind)
             heavy_pos_list.append([pos["x"], pos["y"]])
         heavy_ind = arr(heavy_ind_list)
         heavy_pos = arr(heavy_pos_list)
         if heavy_ind.any():
             layout[heavy_ind, :] = heavy_pos
-        weights = matrix ** self.weight_exp  # bus-pair weights (lower for distant buses)
+        weights = matrix**self.weight_exp  # bus-pair weights (lower for distant buses)
         maxstep = 1 / np.min(weights[mask])
         minstep = 1 / np.max(weights[mask])
         lambda_ = np.log(minstep / maxstep) / (self.max_iters - 1)  # exponential decay of allowed adjustment
         sets = self.sets()  # construct sets of bus pairs
         self._layout_progressed(2)
         for iteration in range(self.max_iters):
             if self._is_stopped():
```

### Comparing `spinedb_api-0.31.0/spinedb_api/helpers.py` & `spinedb_api-0.31.1/spinedb_api/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
     "uq": "uq_%(table_name)s_%(column_0N_name)s",
     "ck": "ck_%(table_name)s_%(constraint_name)s",
 }
 
 model_meta = MetaData(naming_convention=naming_convention)
 
-LONGTEXT_LENGTH = 2 ** 32 - 1
+LONGTEXT_LENGTH = 2**32 - 1
 
 
 def name_from_elements(elements):
     """Creates an entity name by combining element names.
 
     Args:
         elements (Sequence of str): element names
@@ -375,15 +375,15 @@
         meta,
         Column("id", Integer, primary_key=True),
         Column("name", String(255), nullable=False),
         Column("description", Text(), server_default=null()),
         Column("display_order", Integer, server_default="99"),
         Column("display_icon", BigInteger, server_default=null()),
         Column("hidden", Integer, server_default="0"),
-        Column("active_by_default", Boolean(name="active_by_default"), server_default=false(), nullable=False),
+        Column("active_by_default", Boolean(name="active_by_default"), server_default=true(), nullable=False),
     )
     Table(
         "superclass_subclass",
         meta,
         Column("id", Integer, primary_key=True),
         Column(
             "superclass_id",
```

### Comparing `spinedb_api-0.31.0/spinedb_api/import_functions.py` & `spinedb_api-0.31.1/spinedb_api/import_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/import_mapping/__init__.py` & `spinedb_api-0.31.1/spinedb_api/import_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/import_mapping/generator.py` & `spinedb_api-0.31.1/spinedb_api/import_mapping/generator.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/import_mapping/import_mapping.py` & `spinedb_api-0.31.1/spinedb_api/import_mapping/import_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,19 +450,22 @@
 
     Cannot be used as the topmost mapping; one of the parents must be :class:`EntityClassMapping`.
     """
 
     MAP_TYPE = "Dimension"
 
     def _import_row(self, source_data, state, mapped_data):
-        _ = state[ImportKey.ENTITY_CLASS_NAME]
-        dimension_name = str(source_data)
-        state[ImportKey.DIMENSION_NAMES].append(dimension_name)
+        if ImportKey.ENTITY_CLASS_NAME not in state:
+            raise KeyError(ImportKey.ENTITY_CLASS_NAME)
         dimension_names = state[ImportKey.DIMENSION_NAMES]
         if len(dimension_names) == state[ImportKey.DIMENSION_COUNT]:
+            return
+        dimension_name = str(source_data)
+        dimension_names.append(dimension_name)
+        if len(dimension_names) == state[ImportKey.DIMENSION_COUNT]:
             raise KeyFix(ImportKey.DIMENSION_NAMES)
 
 
 class ElementMapping(ImportEntitiesMixin, ImportMapping):
     """Maps elements.
 
     Cannot be used as the topmost mapping; must have :class:`EntityClassMapping` and :class:`EntityMapping`
@@ -792,29 +795,18 @@
 
     Can be used as the topmost mapping.
     """
 
     MAP_TYPE = "Scenario"
 
     def _import_row(self, source_data, state, mapped_data):
-        state[ImportKey.SCENARIO_NAME] = str(source_data)
-
-
-class ScenarioActiveFlagMapping(ImportMapping):
-    """Maps scenario active flags.
-
-    Cannot be used as the topmost mapping; must have a :class:`ScenarioMapping` as parent.
-    """
-
-    MAP_TYPE = "ScenarioActiveFlag"
-
-    def _import_row(self, source_data, state, mapped_data):
-        scenario = state[ImportKey.SCENARIO_NAME]
-        active = string_to_bool(str(source_data))
-        mapped_data.setdefault("scenarios", set()).add((scenario, active))
+        scenario = str(source_data)
+        state[ImportKey.SCENARIO_NAME] = scenario
+        if self._child is None:
+            mapped_data.setdefault("scenarios", set()).add((scenario,))
 
 
 class ScenarioAlternativeMapping(ImportMapping):
     """Maps scenario alternatives.
 
     Cannot be used as the topmost mapping; must have a :class:`ScenarioMapping` as parent.
     """
@@ -903,15 +895,14 @@
 def _default_scenario_mapping():
     """Creates default scenario mappings.
 
     Returns:
         ScenarioMapping: root mapping
     """
     root_mapping = ScenarioMapping(Position.hidden)
-    root_mapping.child = ScenarioActiveFlagMapping(Position.hidden)
     return root_mapping
 
 
 def _default_scenario_alternative_mapping():
     """Creates default scenario alternative mappings.
 
     Returns:
@@ -976,15 +967,14 @@
             IndexNameMapping,
             ParameterValueIndexMapping,
             ExpandedParameterValueMapping,
             ParameterValueListMapping,
             ParameterValueListValueMapping,
             AlternativeMapping,
             ScenarioMapping,
-            ScenarioActiveFlagMapping,
             ScenarioAlternativeMapping,
             ScenarioBeforeAlternativeMapping,
             ToolMapping,
             # FIXME
             # FeatureEntityClassMapping,
             # FeatureParameterDefinitionMapping,
             # ToolFeatureEntityClassMapping,
@@ -1006,14 +996,17 @@
         "Relationship": EntityMapping,
         "RelationshipObject": ElementMapping,
         "RelationshipMetadata": EntityMetadataMapping,
     }
     mappings.update(legacy_mappings)
     flattened = []
     for mapping_dict in serialized:
+        if mapping_dict["map_type"] == "ScenarioActiveFlag":
+            # We don't have active flag mapping anymore.
+            continue
         position = mapping_dict["position"]
         value = mapping_dict.get("value")
         skip_columns = mapping_dict.get("skip_columns")
         read_start_row = mapping_dict.get("read_start_row", 0)
         filter_re = mapping_dict.get("filter_re", "")
         if isinstance(position, str):
             position = Position(position)
```

### Comparing `spinedb_api-0.31.0/spinedb_api/import_mapping/import_mapping_compat.py` & `spinedb_api-0.31.1/spinedb_api/import_mapping/import_mapping_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     ParameterValueMapping,
     ParameterValueTypeMapping,
     ParameterValueMetadataMapping,
     ParameterValueIndexMapping,
     ExpandedParameterValueMapping,
     AlternativeMapping,
     ScenarioMapping,
-    ScenarioActiveFlagMapping,
     ScenarioAlternativeMapping,
     ScenarioBeforeAlternativeMapping,
     EntityGroupMapping,
     ParameterValueListMapping,
     ParameterValueListValueMapping,
     from_dict as mapping_from_dict,
     IndexNameMapping,
@@ -106,17 +105,15 @@
     return root_mapping
 
 
 def _scenario_mapping_from_dict(map_dict):
     name = map_dict.get("name")
     skip_columns = map_dict.get("skip_columns", [])
     read_start_row = map_dict.get("read_start_row", 0)
-    active = map_dict.get("active", "false")
     root_mapping = ScenarioMapping(*_pos_and_val(name), skip_columns=skip_columns, read_start_row=read_start_row)
-    root_mapping.child = ScenarioActiveFlagMapping(*_pos_and_val(active))
     return root_mapping
 
 
 def _scenario_alternative_mapping_from_dict(map_dict):
     scenario_name = map_dict.get("scenario_name")
     alternative_name = map_dict.get("alternative_name")
     before_alternative_name = map_dict.get("before_alternative_name")
```

### Comparing `spinedb_api-0.31.0/spinedb_api/import_mapping/type_conversion.py` & `spinedb_api-0.31.1/spinedb_api/import_mapping/type_conversion.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/mapped_items.py` & `spinedb_api-0.31.1/spinedb_api/mapped_items.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         return super().__getitem__(key)
 
     def polish(self):
         error = super().polish()
         if error:
             return error
         if "active_by_default" not in self:
-            self["active_by_default"] = bool(dict.get(self, "dimension_id_list"))
+            self["active_by_default"] = True
 
     def merge(self, other):
         dimension_id_list = other.pop("dimension_id_list", None)
         error = (
             "can't modify dimensions of an entity class"
             if dimension_id_list is not None and dimension_id_list != self["dimension_id_list"]
             else ""
@@ -160,15 +160,15 @@
         if isinstance(element_id_list, str):
             element_id_list = (int(id_) for id_ in element_id_list.split(","))
         kwargs["element_id_list"] = tuple(element_id_list)
         super().__init__(*args, **kwargs)
 
     @classmethod
     def unique_values_for_item(cls, item, skip_keys=()):
-        """Overriden to also yield unique values for the superclass."""
+        """Overridden to also yield unique values for the superclass."""
         for key, value in super().unique_values_for_item(item, skip_keys=skip_keys):
             yield key, value
             sc_value = tuple(item.get("superclass_name" if k == "entity_class_name" else k) for k in key)
             if None not in sc_value:
                 yield (key, sc_value)
 
     def _byname_iter(self, entity):
@@ -378,15 +378,15 @@
         if key == "parsed_value":
             return self.parsed_value
         return super().__getitem__(key)
 
     def _something_to_update(self, other):
         if self._value_key in other and self._type_key in other:
             other_value_type = other[self._type_key]
-            if self.type != other_value_type:
+            if self[self._type_key] != other_value_type:
                 return True
             other_value = other[self._value_key]
             if self.value != other_value:
                 try:
                     other_parsed_value = from_database(other_value, other_value_type)
                     if self.parsed_value != other_parsed_value:
                         return True
@@ -430,15 +430,20 @@
         error = super().polish()
         if error:
             return error
         list_name = self["parameter_value_list_name"]
         if list_name is None:
             self["list_value_id"] = None
             return
-        type_ = super().__getitem__(self._type_key)
+        try:
+            type_ = super().__getitem__(self._type_key)
+        except KeyError:
+            if isinstance(self, ParameterValueItem):
+                return f"parameter value {self['parameter_definition_name']} for class {self['entity_class_name']}, entity {self['entity_byname']}, alternative {self['alternative_name']} has no list value"
+            return f"parameter {self['name']} for class {self['entity_class_name']} has no list value"
         if type_ == "list_value_ref":
             return
         value = super().__getitem__(self._value_key)
         parsed_value = from_database(value, type_)
         if parsed_value is None:
             return
         list_value_id = self._db_map.get_item(
```

### Comparing `spinedb_api-0.31.0/spinedb_api/mapping.py` & `spinedb_api-0.31.1/spinedb_api/mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/parameter_value.py` & `spinedb_api-0.31.1/spinedb_api/parameter_value.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/perfect_split.py` & `spinedb_api-0.31.1/spinedb_api/perfect_split.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/purge.py` & `spinedb_api-0.31.1/spinedb_api/purge.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/query.py` & `spinedb_api-0.31.1/spinedb_api/query.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/server_client_helpers.py` & `spinedb_api-0.31.1/spinedb_api/server_client_helpers.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_db_client.py` & `spinedb_api-0.31.1/spinedb_api/spine_db_client.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_db_server.py` & `spinedb_api-0.31.1/spinedb_api/spine_db_server.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/__init__.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/exporters/__init__.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/exporters/csv_writer.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/csv_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/exporters/excel.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/excel.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/exporters/excel_writer.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/excel_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/exporters/gdx_writer.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/gdx_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/exporters/sql_writer.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/sql_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/exporters/writer.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/exporters/writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/gdx_utils.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/gdx_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     import winreg
 
 
 def _python_interpreter_bitness():
     """Returns 64 for 64bit Python interpreter or 32 for 32bit interpreter."""
     # As recommended in Python's docs:
     # https://docs.python.org/3/library/platform.html#cross-platform
-    return 64 if sys.maxsize > 2 ** 32 else 32
+    return 64 if sys.maxsize > 2**32 else 32
 
 
 def _windows_dlls_exist(gams_path):
     """Returns True if requred DLL files exist in given GAMS installation path."""
     bitness = _python_interpreter_bitness()
     # This DLL must exist on Windows installation
     dll_name = "gdxdclib{}.dll".format(bitness)
```

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/importers/__init__.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/importers/csv_reader.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/importers/csv_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/importers/datapackage_reader.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/importers/datapackage_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/importers/excel_reader.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/importers/excel_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/importers/gdx_connector.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/importers/gdx_connector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/importers/json_reader.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/importers/json_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/importers/reader.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/importers/reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/spine_io/importers/sqlalchemy_connector.py` & `spinedb_api-0.31.1/spinedb_api/spine_io/importers/sqlalchemy_connector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api/temp_id.py` & `spinedb_api-0.31.1/spinedb_api/temp_id.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/spinedb_api.egg-info/PKG-INFO` & `spinedb_api-0.31.1/spinedb_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinedb_api
-Version: 0.31.0
+Version: 0.31.1
 Summary: An API to talk to Spine databases.
 Author-email: Spine Project consortium <spine_info@vtt.fi>
 License: LGPL-3.0-or-later
 Project-URL: Repository, https://github.com/spine-tools/Spine-Database-API
 Keywords: energy system modelling,workflow,optimisation,database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spinedb_api Version: 0.31.0 Summary: An API to talk
+Metadata-Version: 2.1 Name: spinedb_api Version: 0.31.1 Summary: An API to talk
 to Spine databases. Author-email: Spine Project consortium
 vtt.fi> License: LGPL-3.0-or-later Project-URL: Repository, https://github.com/
 spine-tools/Spine-Database-API Keywords: energy system
 modelling,workflow,optimisation,database Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: >=3.8.1 Description-Content-Type: text/markdown License-File: COPYING
```

### Comparing `spinedb_api-0.31.0/spinedb_api.egg-info/SOURCES.txt` & `spinedb_api-0.31.1/spinedb_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py
 spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py
 spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py
 spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py
 spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py
 spinedb_api/alembic/versions/ce9faa82ed59_create_entity_alternative_table.py
 spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py
+spinedb_api/alembic/versions/e010777927a5_change_active_by_default_server_default_.py
 spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py
 spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py
 spinedb_api/export_mapping/__init__.py
 spinedb_api/export_mapping/export_mapping.py
 spinedb_api/export_mapping/generator.py
 spinedb_api/export_mapping/group_functions.py
 spinedb_api/export_mapping/pivot.py
```

### Comparing `spinedb_api-0.31.0/tests/__init__.py` & `spinedb_api-0.31.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/custom_db_mapping.py` & `spinedb_api-0.31.1/tests/custom_db_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/export_mapping/__init__.py` & `spinedb_api-0.31.1/tests/export_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/export_mapping/test_export_mapping.py` & `spinedb_api-0.31.1/tests/export_mapping/test_export_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     ParameterValueIndexMapping,
     ParameterValueListMapping,
     ParameterValueListValueMapping,
     ParameterValueMapping,
     ParameterValueTypeMapping,
     DimensionMapping,
     ElementMapping,
-    ScenarioActiveFlagMapping,
     ScenarioAlternativeMapping,
     ScenarioDescriptionMapping,
     ScenarioMapping,
 )
 from spinedb_api.mapping import unflatten
 
 
@@ -959,27 +958,14 @@
         scenario_mapping = ScenarioMapping(0)
         tables = dict()
         for title, title_key in titles(scenario_mapping, db_map):
             tables[title] = list(rows(scenario_mapping, db_map, title_key))
         self.assertEqual(tables, {None: [["s1"], ["s2"]]})
         db_map.close()
 
-    def test_scenario_active_flag_mapping(self):
-        db_map = DatabaseMapping("sqlite://", create=True)
-        import_scenarios(db_map, (("s1", True), ("s2", False)))
-        db_map.commit_session("Add test data.")
-        scenario_mapping = ScenarioMapping(0)
-        active_flag_mapping = ScenarioActiveFlagMapping(1)
-        scenario_mapping.child = active_flag_mapping
-        tables = dict()
-        for title, title_key in titles(scenario_mapping, db_map):
-            tables[title] = list(rows(scenario_mapping, db_map, title_key))
-        self.assertEqual(tables, {None: [["s1", True], ["s2", False]]})
-        db_map.close()
-
     def test_scenario_alternative_mapping(self):
         db_map = DatabaseMapping("sqlite://", create=True)
         import_alternatives(db_map, ("a1", "a2", "a3"))
         import_scenarios(db_map, ("s1", "s2", "empty"))
         import_scenario_alternatives(db_map, (("s1", "a2"), ("s1", "a1", "a2"), ("s2", "a2"), ("s2", "a3", "a2")))
         db_map.commit_session("Add test data.")
         scenario_mapping = ScenarioMapping(0)
```

### Comparing `spinedb_api-0.31.0/tests/export_mapping/test_pivot.py` & `spinedb_api-0.31.1/tests/export_mapping/test_pivot.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/export_mapping/test_settings.py` & `spinedb_api-0.31.1/tests/export_mapping/test_settings.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/filters/__init__.py` & `spinedb_api-0.31.1/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/filters/test_alternative_filter.py` & `spinedb_api-0.31.1/tests/filters/test_alternative_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/filters/test_execution_filter.py` & `spinedb_api-0.31.1/tests/filters/test_execution_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/filters/test_renamer.py` & `spinedb_api-0.31.1/tests/filters/test_renamer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/filters/test_scenario_filter.py` & `spinedb_api-0.31.1/tests/filters/test_scenario_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/filters/test_tool_filter.py` & `spinedb_api-0.31.1/tests/filters/test_tool_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/filters/test_tools.py` & `spinedb_api-0.31.1/tests/filters/test_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,38 +97,38 @@
         db_map.close()
 
     def test_empty_stack(self):
         db_map = DatabaseMapping(self._db_url)
         try:
             apply_filter_stack(db_map, [])
             object_classes = export_entity_classes(db_map)
-            self.assertEqual(object_classes, [("object_class", (), None, None, False)])
+            self.assertEqual(object_classes, [("object_class", (), None, None, True)])
         finally:
             db_map.close()
 
     def test_single_renaming_filter(self):
         db_map = DatabaseMapping(self._db_url)
         try:
             stack = [entity_class_renamer_config(object_class="renamed_once")]
             apply_filter_stack(db_map, stack)
             object_classes = export_entity_classes(db_map)
-            self.assertEqual(object_classes, [("renamed_once", (), None, None, False)])
+            self.assertEqual(object_classes, [("renamed_once", (), None, None, True)])
         finally:
             db_map.close()
 
     def test_two_renaming_filters(self):
         db_map = DatabaseMapping(self._db_url)
         try:
             stack = [
                 entity_class_renamer_config(object_class="renamed_once"),
                 entity_class_renamer_config(renamed_once="renamed_twice"),
             ]
             apply_filter_stack(db_map, stack)
             object_classes = export_entity_classes(db_map)
-            self.assertEqual(object_classes, [("renamed_twice", (), None, None, False)])
+            self.assertEqual(object_classes, [("renamed_twice", (), None, None, True)])
         finally:
             db_map.close()
 
 
 class TestFilteredDatabaseMap(unittest.TestCase):
     _db_url = URL("sqlite")
     _dir = None
@@ -143,27 +143,27 @@
         db_map.commit_session("Add test data.")
         db_map.close()
 
     def test_without_filters(self):
         db_map = DatabaseMapping(self._db_url, self._engine)
         try:
             object_classes = export_entity_classes(db_map)
-            self.assertEqual(object_classes, [("object_class", (), None, None, False)])
+            self.assertEqual(object_classes, [("object_class", (), None, None, True)])
         finally:
             db_map.close()
 
     def test_single_renaming_filter(self):
         path = os.path.join(self._dir.name, "config.json")
         with open(path, "w") as out_file:
             store_filter(entity_class_renamer_config(object_class="renamed_once"), out_file)
         url = append_filter_config(str(self._db_url), path)
         db_map = DatabaseMapping(url, self._engine)
         try:
             object_classes = export_entity_classes(db_map)
-            self.assertEqual(object_classes, [("renamed_once", (), None, None, False)])
+            self.assertEqual(object_classes, [("renamed_once", (), None, None, True)])
         finally:
             db_map.close()
 
     def test_two_renaming_filters(self):
         path1 = os.path.join(self._dir.name, "config1.json")
         with open(path1, "w") as out_file:
             store_filter(entity_class_renamer_config(object_class="renamed_once"), out_file)
@@ -171,25 +171,25 @@
         path2 = os.path.join(self._dir.name, "config2.json")
         with open(path2, "w") as out_file:
             store_filter(entity_class_renamer_config(renamed_once="renamed_twice"), out_file)
         url = append_filter_config(url, path2)
         db_map = DatabaseMapping(url, self._engine)
         try:
             object_classes = export_entity_classes(db_map)
-            self.assertEqual(object_classes, [("renamed_twice", (), None, None, False)])
+            self.assertEqual(object_classes, [("renamed_twice", (), None, None, True)])
         finally:
             db_map.close()
 
     def test_config_embedded_to_url(self):
         config = entity_class_renamer_config(object_class="renamed_once")
         url = append_filter_config(str(self._db_url), config)
         db_map = DatabaseMapping(url, self._engine)
         try:
             object_classes = export_entity_classes(db_map)
-            self.assertEqual(object_classes, [("renamed_once", (), None, None, False)])
+            self.assertEqual(object_classes, [("renamed_once", (), None, None, True)])
         finally:
             db_map.close()
 
 
 class TestAppendFilterConfig(unittest.TestCase):
     def test_append_to_simple_url(self):
         url = append_filter_config(r"sqlite:///C:\dbs\database.sqlite", r"F:\fltr\a.json")
```

### Comparing `spinedb_api-0.31.0/tests/filters/test_value_transformer.py` & `spinedb_api-0.31.1/tests/filters/test_value_transformer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/import_mapping/__init__.py` & `spinedb_api-0.31.1/tests/import_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/import_mapping/test_generator.py` & `spinedb_api-0.31.1/tests/import_mapping/test_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -438,10 +438,81 @@
                     ["Data", "d2", "parameter2", 2.3, "Base"],
                 ],
                 "parameter_definitions": [("Data", "parameter1"), ("Data", "parameter2")],
                 "entities": [("Data", "d1"), ("Data", "d2")],
             },
         )
 
+    def test_import_scenario(self):
+        data_source = iter([["scen1"]])
+        mappings = [
+            [
+                {"map_type": "Scenario", "position": 0},
+            ]
+        ]
+        convert_function_specs = {0: "string"}
+        convert_functions = {column: value_to_convert_spec(spec) for column, spec in convert_function_specs.items()}
+        mapped_data, errors = get_mapped_data(data_source, mappings, column_convert_fns=convert_functions)
+        self.assertEqual(errors, [])
+        self.assertEqual(
+            mapped_data,
+            {"scenarios": {("scen1",)}},
+        )
+
+    def test_importing_multidimensional_class_when_there_is_an_extra_column(self):
+        header = ["3D entity class", "unit", "node", "node", "parameter", "alternative", "value", None]
+        data_source = iter(
+            [
+                ["unit__node__node", "Dyson sphere", "Gamma Ceti", "Ring world", "flow", "Base", 23.3, None],
+                7 * [None] + ["aa"],
+            ]
+        )
+        mappings = [
+            [
+                {"map_type": "EntityClass", "position": 0},
+                {"map_type": "Dimension", "position": "header", "value": 1},
+                {"map_type": "Dimension", "position": "header", "value": 2},
+                {"map_type": "Dimension", "position": "header", "value": 3},
+                {"map_type": "Entity", "position": "hidden"},
+                {"map_type": "Element", "position": 1, "import_entities": True},
+                {"map_type": "Element", "position": 2, "import_entities": True},
+                {"map_type": "Element", "position": 3, "import_entities": True},
+                {"map_type": "EntityMetadata", "position": "hidden"},
+                {"map_type": "ParameterDefinition", "position": 4},
+                {"map_type": "Alternative", "position": 5},
+                {"map_type": "ParameterValueMetadata", "position": "hidden"},
+                {"map_type": "ParameterValue", "position": 6},
+            ]
+        ]
+        convert_function_specs = {
+            0: "string",
+            1: "string",
+            2: "string",
+            3: "string",
+            4: "string",
+            5: "string",
+            6: "float",
+        }
+        convert_functions = {column: value_to_convert_spec(spec) for column, spec in convert_function_specs.items()}
+        mapped_data, errors = get_mapped_data(data_source, mappings, header, column_convert_fns=convert_functions)
+        self.assertEqual(errors, [])
+        self.assertEqual(
+            mapped_data,
+            {
+                "alternatives": {"Base"},
+                "entities": [
+                    ("unit", "Dyson sphere"),
+                    ("node", "Gamma Ceti"),
+                    ("node", "Ring world"),
+                    ("unit__node__node", ("Dyson sphere", "Gamma Ceti", "Ring world")),
+                ],
+                "entity_classes": [("unit",), ("node",), ("unit__node__node", ("unit", "node", "node"))],
+                "parameter_definitions": [("unit__node__node", "flow")],
+                "parameter_values": [
+                    ["unit__node__node", ("Dyson sphere", "Gamma Ceti", "Ring world"), "flow", 23.3, "Base"]
+                ],
+            },
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `spinedb_api-0.31.0/tests/import_mapping/test_import_mapping.py` & `spinedb_api-0.31.1/tests/import_mapping/test_import_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         expected = ["Alternative"]
         self.assertEqual(types, expected)
 
     def test_scenario_mapping(self):
         mapping = import_mapping_from_dict({"map_type": "Scenario"})
         d = mapping_to_dict(mapping)
         types = [m["map_type"] for m in d]
-        expected = ["Scenario", "ScenarioActiveFlag"]
+        expected = ["Scenario"]
         self.assertEqual(types, expected)
 
     def test_scenario_alternative_mapping(self):
         mapping = import_mapping_from_dict({"map_type": "ScenarioAlternative"})
         d = mapping_to_dict(mapping)
         types = [m["map_type"] for m in d]
         expected = ["Scenario", "ScenarioAlternative", "ScenarioBeforeAlternative"]
@@ -401,15 +401,14 @@
 
     def test_Scenario_to_dict_from_dict(self):
         mapping = {"map_type": "Scenario", "name": 0}
         mapping = import_mapping_from_dict(mapping)
         out = mapping_to_dict(mapping)
         expected = [
             {"map_type": "Scenario", "position": 0},
-            {"map_type": "ScenarioActiveFlag", "position": "hidden", "value": "false"},
         ]
         self.assertEqual(out, expected)
 
     def test_ScenarioAlternative_to_dict_from_dict(self):
         mapping = {
             "map_type": "ScenarioAlternative",
             "scenario_name": 0,
@@ -1644,25 +1643,25 @@
 
     def test_read_scenario(self):
         input_data = [["Scenarios"], ["scenario1"], ["second_scenario"], ["last_one"]]
         data = iter(input_data)
         data_header = next(data)
         mapping = {"map_type": "Scenario", "name": 0}
         out, errors = get_mapped_data(data, [mapping], data_header)
-        expected = {"scenarios": {("scenario1", False), ("second_scenario", False), ("last_one", False)}}
+        expected = {"scenarios": {("scenario1",), ("second_scenario",), ("last_one",)}}
         self.assertFalse(errors)
         self.assertEqual(out, expected)
 
     def test_read_scenario_with_active_flags(self):
         input_data = [["Scenarios", "Active"], ["scenario1", 1], ["second_scenario", "f"], ["last_one", "true"]]
         data = iter(input_data)
         data_header = next(data)
         mapping = {"map_type": "Scenario", "name": 0, "active": 1}
         out, errors = get_mapped_data(data, [mapping], data_header)
-        expected = {"scenarios": {("scenario1", True), ("second_scenario", False), ("last_one", True)}}
+        expected = {"scenarios": {("scenario1",), ("second_scenario",), ("last_one",)}}
         self.assertFalse(errors)
         self.assertEqual(out, expected)
 
     def test_read_scenario_alternative(self):
         input_data = [
             ["Scenario", "Alternative", "Before alternative"],
             ["scenario_A", "alternative1", "second_alternative"],
```

### Comparing `spinedb_api-0.31.0/tests/import_mapping/test_type_conversion.py` & `spinedb_api-0.31.1/tests/import_mapping/test_type_conversion.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/__init__.py` & `spinedb_api-0.31.1/tests/spine_io/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/exporters/__init__.py` & `spinedb_api-0.31.1/tests/spine_io/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/exporters/test_csv_writer.py` & `spinedb_api-0.31.1/tests/spine_io/exporters/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/exporters/test_excel_writer.py` & `spinedb_api-0.31.1/tests/spine_io/exporters/test_excel_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/exporters/test_gdx_writer.py` & `spinedb_api-0.31.1/tests/spine_io/exporters/test_gdx_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/exporters/test_sql_writer.py` & `spinedb_api-0.31.1/tests/spine_io/exporters/test_sql_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/exporters/test_writer.py` & `spinedb_api-0.31.1/tests/spine_io/exporters/test_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/importers/__init__.py` & `spinedb_api-0.31.1/tests/spine_io/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/importers/test_CSVConnector.py` & `spinedb_api-0.31.1/tests/spine_io/importers/test_CSVConnector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/importers/test_GdxConnector.py` & `spinedb_api-0.31.1/tests/spine_io/importers/test_GdxConnector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/importers/test_datapackage_reader.py` & `spinedb_api-0.31.1/tests/spine_io/importers/test_datapackage_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/importers/test_excel_reader.py` & `spinedb_api-0.31.1/tests/spine_io/importers/test_excel_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/importers/test_json_reader.py` & `spinedb_api-0.31.1/tests/spine_io/importers/test_json_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/importers/test_reader.py` & `spinedb_api-0.31.1/tests/spine_io/importers/test_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/importers/test_sqlalchemy_connector.py` & `spinedb_api-0.31.1/tests/spine_io/importers/test_sqlalchemy_connector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/spine_io/test_excel_integration.py` & `spinedb_api-0.31.1/tests/spine_io/test_excel_integration.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/test_DatabaseMapping.py` & `spinedb_api-0.31.1/tests/test_DatabaseMapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,18 +89,18 @@
     def _assert_success(self, result):
         item, error = result
         self.assertIsNone(error)
         return item
 
 
 class TestDatabaseMapping(AssertSuccessTestCase):
-    def test_active_by_default_is_initially_false_for_zero_dimensional_entity_class(self):
+    def test_active_by_default_is_initially_true_for_zero_dimensional_entity_class(self):
         with DatabaseMapping("sqlite://", create=True) as db_map:
             item = self._assert_success(db_map.add_entity_class_item(name="Entity"))
-            self.assertFalse(item["active_by_default"])
+            self.assertTrue(item["active_by_default"])
 
     def test_active_by_default_is_initially_false_for_multi_dimensional_entity_class(self):
         with DatabaseMapping("sqlite://", create=True) as db_map:
             db_map.add_entity_class_item(name="Dimension")
             item = self._assert_success(db_map.add_entity_class_item(name="Entity", dimension_name_list=("Dimension",)))
             self.assertTrue(item["active_by_default"])
 
@@ -670,15 +670,15 @@
                 for entity_class in db_map.query(db_map.wide_entity_class_sq)
             }
             self.assertEqual(active_by_defaults, {"Widget": True, "Gadget": True, "NoIsActiveDefault": False})
             defaults = [
                 from_database(definition["default_value"], definition["default_type"])
                 for definition in db_map.query(db_map.parameter_definition_sq)
             ]
-            self.assertEqual(defaults, 3 * [None])
+            self.assertEqual(defaults, [True, True, None])
 
     def test_remove_items_by_asterisk(self):
         with DatabaseMapping("sqlite://", create=True) as db_map:
             self._assert_success(db_map.add_alternative_item(name="alt_1"))
             self._assert_success(db_map.add_alternative_item(name="alt_2"))
             db_map.commit_session("Add alternatives.")
             alternatives = db_map.get_alternative_items()
@@ -717,14 +717,151 @@
             entity_class.remove()
             self.assertFalse(entity.is_valid())
             entity.restore()
             self.assertFalse(entity.is_valid())
             entity_class.restore()
             self.assertTrue(entity.is_valid())
 
+    def test_get_parameter_value_from_wrong_alternative_fails_graciously(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            self._assert_success(db_map.add_alternative_item(name="extra alternative"))
+            self._assert_success(db_map.add_entity_class_item(name="Object"))
+            self._assert_success(db_map.add_entity_item(name="knife", entity_class_name="Object"))
+            self._assert_success(db_map.add_parameter_definition_item(entity_class_name="Object", name="x"))
+            db_value, value_type = to_database(2.3)
+            self._assert_success(
+                db_map.add_parameter_value_item(
+                    entity_class_name="Object",
+                    entity_byname=("knife",),
+                    parameter_definition_name="x",
+                    alternative_name="Base",
+                    value=db_value,
+                    type=value_type,
+                )
+            )
+            gotten_value = db_map.get_parameter_value_item(
+                entity_class_name="Object",
+                entity_byname=("knife",),
+                parameter_definition_name="x",
+                alternative_name="extra alternative",
+            )
+            self.assertEqual(gotten_value, {})
+
+    def test_get_parameter_value_with_list_value(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            self._assert_success(db_map.add_parameter_value_list_item(name="Enumeration"))
+            db_value, value_type = to_database(2.3)
+            self._assert_success(
+                db_map.add_list_value_item(
+                    parameter_value_list_name="Enumeration", value=db_value, type=value_type, index=0
+                )
+            )
+            self._assert_success(db_map.add_entity_class_item(name="Object"))
+            self._assert_success(db_map.add_entity_item(name="knife", entity_class_name="Object"))
+            self._assert_success(
+                db_map.add_parameter_definition_item(
+                    entity_class_name="Object", name="x", parameter_value_list_name="Enumeration"
+                )
+            )
+            self._assert_success(
+                db_map.add_parameter_value_item(
+                    entity_class_name="Object",
+                    entity_byname=("knife",),
+                    parameter_definition_name="x",
+                    alternative_name="Base",
+                    value=db_value,
+                    type=value_type,
+                )
+            )
+            gotten_value = db_map.get_parameter_value_item(
+                entity_class_name="Object",
+                entity_byname=("knife",),
+                parameter_definition_name="x",
+                alternative_name="Base",
+            )
+            self.assertEqual(gotten_value["parsed_value"], 2.3)
+
+    def test_get_parameter_value_with_list_value_from_disk(self):
+        with TemporaryDirectory() as temp_dir:
+            url = "sqlite:///" + os.path.join(temp_dir, "db.sqlite")
+            with DatabaseMapping(url, create=True) as db_map:
+                self._assert_success(db_map.add_parameter_value_list_item(name="Enumeration"))
+                value, value_type = to_database(2.3)
+                self._assert_success(
+                    db_map.add_list_value_item(
+                        parameter_value_list_name="Enumeration", value=value, type=value_type, index=0
+                    )
+                )
+                self._assert_success(db_map.add_entity_class_item(name="Object"))
+                self._assert_success(db_map.add_entity_item(name="knife", entity_class_name="Object"))
+                self._assert_success(
+                    db_map.add_parameter_definition_item(
+                        entity_class_name="Object", name="x", parameter_value_list_name="Enumeration"
+                    )
+                )
+                self._assert_success(
+                    db_map.add_parameter_value_item(
+                        entity_class_name="Object",
+                        entity_byname=("knife",),
+                        parameter_definition_name="x",
+                        alternative_name="Base",
+                        value=value,
+                        type=value_type,
+                    )
+                )
+                db_map.commit_session("Add parameter value.")
+            with DatabaseMapping(url) as db_map:
+                value = db_map.get_parameter_value_item(
+                    entity_class_name="Object",
+                    entity_byname=("knife",),
+                    parameter_definition_name="x",
+                    alternative_name="Base",
+                )
+                self.assertNotEqual(value, {})
+                self.assertEqual(value["parsed_value"], 2.3)
+
+    def test_nonexistent_parameter_value_with_list_value_does_not_traceback(self):
+        with TemporaryDirectory() as temp_dir:
+            url = "sqlite:///" + os.path.join(temp_dir, "db.sqlite")
+            with DatabaseMapping(url, create=True) as db_map:
+                self._assert_success(db_map.add_alternative_item(name="extra alternative"))
+                self._assert_success(db_map.add_parameter_value_list_item(name="Enumeration"))
+                value, value_type = to_database(2.3)
+                self._assert_success(
+                    db_map.add_list_value_item(
+                        parameter_value_list_name="Enumeration", value=value, type=value_type, index=0
+                    )
+                )
+                self._assert_success(db_map.add_entity_class_item(name="Object"))
+                self._assert_success(db_map.add_entity_item(name="knife", entity_class_name="Object"))
+                self._assert_success(
+                    db_map.add_parameter_definition_item(
+                        entity_class_name="Object", name="x", parameter_value_list_name="Enumeration"
+                    )
+                )
+                self._assert_success(
+                    db_map.add_parameter_value_item(
+                        entity_class_name="Object",
+                        entity_byname=("knife",),
+                        parameter_definition_name="x",
+                        alternative_name="Base",
+                        value=value,
+                        type=value_type,
+                    )
+                )
+                db_map.commit_session("Add parameter value.")
+            with DatabaseMapping(url) as db_map:
+                value = db_map.get_parameter_value_item(
+                    entity_class_name="Object",
+                    entity_byname=("knife",),
+                    parameter_definition_name="x",
+                    alternative_name="extra alternative",
+                )
+                self.assertEqual(value, {})
+
 
 class TestDatabaseMappingLegacy(unittest.TestCase):
     """'Backward compatibility' tests, i.e. pre-entity tests converted to work with the entity structure."""
 
     _db_map = None
 
     @classmethod
```

### Comparing `spinedb_api-0.31.0/tests/test_check_integrity.py` & `spinedb_api-0.31.1/tests/test_check_integrity.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/test_db_mapping_base.py` & `spinedb_api-0.31.1/tests/test_db_mapping_base.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/test_db_server.py` & `spinedb_api-0.31.1/tests/test_db_server.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/test_export_functions.py` & `spinedb_api-0.31.1/tests/test_export_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     def test_export_entity_classes(self):
         with DatabaseMapping("sqlite://", username="UnitTest", create=True) as db_map:
             self._assert_addition_success(db_map.add_entity_class_item(name="Object"))
             self._assert_addition_success(
                 db_map.add_entity_class_item(name="Relation", dimension_name_list=("Object",))
             )
             exported = export_entity_classes(db_map)
-            expected = (("Object", (), None, None, False), ("Relation", ("Object",), None, None, True))
+            expected = (("Object", (), None, None, True), ("Relation", ("Object",), None, None, True))
             self.assertCountEqual(exported, expected)
 
     def test_export_data(self):
         with DatabaseMapping("sqlite://", username="UnitTest", create=True) as db_map:
             self._assert_import_success(import_object_classes(db_map, ["object_class"]))
             self._assert_import_success(import_object_parameters(db_map, [("object_class", "object_parameter")]))
             self._assert_import_success(import_objects(db_map, [("object_class", "object")]))
@@ -112,15 +112,15 @@
             self._assert_import_success(import_scenarios(db_map, ["scenario"]))
             self._assert_import_success(import_scenario_alternatives(db_map, [("scenario", "alternative")]))
             exported = export_data(db_map)
             self.assertEqual(len(exported), 8)
             self.assertIn("entity_classes", exported)
             self.assertEqual(
                 exported["entity_classes"],
-                [("object_class", (), None, None, False), ("relationship_class", ("object_class",), None, None, True)],
+                [("object_class", (), None, None, True), ("relationship_class", ("object_class",), None, None, True)],
             )
             self.assertIn("parameter_definitions", exported)
             self.assertEqual(
                 exported["parameter_definitions"],
                 [
                     ("object_class", "object_parameter", None, None, None),
                     ("relationship_class", "relationship_parameter", None, None, None),
```

### Comparing `spinedb_api-0.31.0/tests/test_helpers.py` & `spinedb_api-0.31.1/tests/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         sanitized = remove_credentials_from_url(url)
         self.assertEqual(sanitized, "mysql://example.com/db")
 
 
 class TestGetHeadAlembicVersion(unittest.TestCase):
     def test_returns_latest_version(self):
         # This test must be updated each time new migration script is added.
-        self.assertEqual(get_head_alembic_version(), "8b0eff478bcb")
+        self.assertEqual(get_head_alembic_version(), "e010777927a5")
 
 
 class TestStringToBool(unittest.TestCase):
     def test_truths(self):
         self.assertTrue(string_to_bool("yes"))
         self.assertTrue(string_to_bool("YES"))
         self.assertTrue(string_to_bool("y"))
```

### Comparing `spinedb_api-0.31.0/tests/test_import_functions.py` & `spinedb_api-0.31.1/tests/test_import_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1264,14 +1264,23 @@
         self.assertEqual(count, 1)
         self.assertFalse(errors)
         db_map.commit_session("test")
         scenarios = {s.name: s.description for s in db_map.query(db_map.scenario_sq)}
         self.assertEqual(scenarios, {"scenario": None})
         db_map.close()
 
+    def test_import_single_scenario_as_tuple(self):
+        with DatabaseMapping("sqlite://", create=True) as db_map:
+            count, errors = import_scenarios(db_map, [("scenario",)])
+            self.assertEqual(errors, [])
+            self.assertEqual(count, 1)
+            db_map.commit_session("test")
+            scenarios = {s.name: s.description for s in db_map.query(db_map.scenario_sq)}
+            self.assertEqual(scenarios, {"scenario": None})
+
     def test_scenario_with_description(self):
         db_map = create_db_map()
         count, errors = import_scenarios(db_map, [["scenario", False, "description"]])
         self.assertEqual(count, 1)
         self.assertFalse(errors)
         db_map.commit_session("test")
         scenarios = {s.name: s.description for s in db_map.query(db_map.scenario_sq)}
```

### Comparing `spinedb_api-0.31.0/tests/test_mapping.py` & `spinedb_api-0.31.1/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/test_migration.py` & `spinedb_api-0.31.1/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/test_parameter_value.py` & `spinedb_api-0.31.1/tests/test_parameter_value.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.31.0/tests/test_purge.py` & `spinedb_api-0.31.1/tests/test_purge.py`

 * *Files identical despite different names*

