# Comparing `tmp/dvcx-0.78.1.tar.gz` & `tmp/dvcx-0.78.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.78.1.tar", last modified: Fri May 10 02:43:44 2024, max compression
+gzip compressed data, was "dvcx-0.78.2.tar", last modified: Mon May 13 22:08:28 2024, max compression
```

## Comparing `dvcx-0.78.1.tar` & `dvcx-0.78.2.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.694598 dvcx-0.78.1/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-10 02:43:35.000000 dvcx-0.78.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 02:43:35.000000 dvcx-0.78.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.638598 dvcx-0.78.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.638598 dvcx-0.78.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 02:43:35.000000 dvcx-0.78.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 02:43:35.000000 dvcx-0.78.1/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-10 02:43:35.000000 dvcx-0.78.1/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-10 02:43:35.000000 dvcx-0.78.1/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-10 02:43:35.000000 dvcx-0.78.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.642598 dvcx-0.78.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-10 02:43:35.000000 dvcx-0.78.1/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-10 02:43:35.000000 dvcx-0.78.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-10 02:43:35.000000 dvcx-0.78.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-10 02:43:35.000000 dvcx-0.78.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-10 02:43:35.000000 dvcx-0.78.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-10 02:43:35.000000 dvcx-0.78.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.642598 dvcx-0.78.1/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-10 02:43:35.000000 dvcx-0.78.1/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-10 02:43:35.000000 dvcx-0.78.1/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-10 02:43:35.000000 dvcx-0.78.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-10 02:43:35.000000 dvcx-0.78.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-10 02:43:35.000000 dvcx-0.78.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.642598 dvcx-0.78.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-10 02:43:35.000000 dvcx-0.78.1/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-10 02:43:35.000000 dvcx-0.78.1/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-10 02:43:35.000000 dvcx-0.78.1/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-10 02:43:44.694598 dvcx-0.78.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-10 02:43:35.000000 dvcx-0.78.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.642598 dvcx-0.78.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-10 02:43:35.000000 dvcx-0.78.1/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.646598 dvcx-0.78.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/llm-claude-aggregate-query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/llm-claude-simple-query.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/llm-claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.646598 dvcx-0.78.1/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.650598 dvcx-0.78.1/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.650598 dvcx-0.78.1/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-10 02:43:35.000000 dvcx-0.78.1/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-10 02:43:35.000000 dvcx-0.78.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-10 02:43:35.000000 dvcx-0.78.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 02:43:44.694598 dvcx-0.78.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.634598 dvcx-0.78.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.654598 dvcx-0.78.1/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-10 02:43:44.000000 dvcx-0.78.1/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.658598 dvcx-0.78.1/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72305 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/catalog/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    30873 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.658598 dvcx-0.78.1/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11679 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.662598 dvcx-0.78.1/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45621 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30778 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    34860 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.666598 dvcx-0.78.1/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/feature_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/tar_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.670598 dvcx-0.78.1/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    60286 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/query/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.670598 dvcx-0.78.1/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.670598 dvcx-0.78.1/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.670598 dvcx-0.78.1/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.674598 dvcx-0.78.1/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.674598 dvcx-0.78.1/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-10 02:43:35.000000 dvcx-0.78.1/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.686598 dvcx-0.78.1/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-10 02:43:44.000000 dvcx-0.78.1/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-10 02:43:44.000000 dvcx-0.78.1/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 02:43:44.000000 dvcx-0.78.1/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 02:43:44.000000 dvcx-0.78.1/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-10 02:43:44.000000 dvcx-0.78.1/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 02:43:44.000000 dvcx-0.78.1/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.674598 dvcx-0.78.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.674598 dvcx-0.78.1/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14464 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.678598 dvcx-0.78.1/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35673 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   113295 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26674 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/func/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.678598 dvcx-0.78.1/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/scripts/name_len_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/scripts/name_len_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/test_cli_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/test_query_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.682598 dvcx-0.78.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.686598 dvcx-0.78.1/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15017 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/lib/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/lib/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/lib/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.686598 dvcx-0.78.1/tests/unit/sql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:43:44.686598 dvcx-0.78.1/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_catalog_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_dataset_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-10 02:43:35.000000 dvcx-0.78.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.270123 dvcx-0.78.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-13 22:08:22.000000 dvcx-0.78.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 22:08:22.000000 dvcx-0.78.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.226122 dvcx-0.78.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.226122 dvcx-0.78.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.226122 dvcx-0.78.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-13 22:08:22.000000 dvcx-0.78.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-13 22:08:22.000000 dvcx-0.78.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.226122 dvcx-0.78.2/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-13 22:08:22.000000 dvcx-0.78.2/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 22:08:22.000000 dvcx-0.78.2/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-13 22:08:22.000000 dvcx-0.78.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-13 22:08:22.000000 dvcx-0.78.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-13 22:08:22.000000 dvcx-0.78.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.226122 dvcx-0.78.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-13 22:08:22.000000 dvcx-0.78.2/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-13 22:08:22.000000 dvcx-0.78.2/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-13 22:08:22.000000 dvcx-0.78.2/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-13 22:08:28.270123 dvcx-0.78.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-13 22:08:22.000000 dvcx-0.78.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.226122 dvcx-0.78.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-13 22:08:22.000000 dvcx-0.78.2/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.230123 dvcx-0.78.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.230123 dvcx-0.78.2/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.234123 dvcx-0.78.2/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.234123 dvcx-0.78.2/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-13 22:08:22.000000 dvcx-0.78.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-13 22:08:22.000000 dvcx-0.78.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 22:08:28.270123 dvcx-0.78.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.222123 dvcx-0.78.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.238123 dvcx-0.78.2/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.238123 dvcx-0.78.2/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72305 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/catalog/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31034 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.242123 dvcx-0.78.2/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11679 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.242123 dvcx-0.78.2/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45621 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30778 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34860 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.246123 dvcx-0.78.2/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16870 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/tar_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.250123 dvcx-0.78.2/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60449 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.250123 dvcx-0.78.2/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.250123 dvcx-0.78.2/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.250123 dvcx-0.78.2/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.250123 dvcx-0.78.2/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.250123 dvcx-0.78.2/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.266123 dvcx-0.78.2/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.254123 dvcx-0.78.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.254123 dvcx-0.78.2/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.254123 dvcx-0.78.2/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35673 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113286 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26674 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.258123 dvcx-0.78.2/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.262123 dvcx-0.78.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.262123 dvcx-0.78.2/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15017 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.262123 dvcx-0.78.2/tests/unit/sql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.266123 dvcx-0.78.2/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_catalog_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_dataset_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/utils.py
```

### Comparing `dvcx-0.78.1/.cruft.json` & `dvcx-0.78.2/.cruft.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'12bb835c5034be9af72028ae9c5bd06cf571b9d1'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "6925fc738cd3d7086ab4a2efdd1a3ad56af54691",
+    "commit": "12bb835c5034be9af72028ae9c5bd06cf571b9d1",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/iterative/py-template",
             "author": "Dmitry Petrov",
             "copyright_year": "2022",
             "development_status": "Development Status :: 2 - Pre-Alpha",
             "docs": "False",
```

### Comparing `dvcx-0.78.1/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.78.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.78.2/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/.github/workflows/benchmarks.yml` & `dvcx-0.78.2/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/.github/workflows/release.yml` & `dvcx-0.78.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/.github/workflows/tests.yml` & `dvcx-0.78.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/.gitignore` & `dvcx-0.78.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/.pre-commit-config.yaml` & `dvcx-0.78.2/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ['--fix=lf']
       - id: sort-simple-yaml
       - id: trailing-whitespace
         exclude: '^LICENSES/'
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.4.2'
+    rev: 'v0.4.4'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.5
     hooks:
```

### Comparing `dvcx-0.78.1/CODE_OF_CONDUCT.rst` & `dvcx-0.78.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/CONTRIBUTING.rst` & `dvcx-0.78.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/LICENSE` & `dvcx-0.78.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/LICENSES/Apache-2.0.txt` & `dvcx-0.78.2/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/LICENSES/BSD-3-Clause.txt` & `dvcx-0.78.2/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/LICENSES/Python-2.0.txt` & `dvcx-0.78.2/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/PKG-INFO` & `dvcx-0.78.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.78.1
+Version: 0.78.2
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.78.1/README.rst` & `dvcx-0.78.2/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/docs/udfs.md` & `dvcx-0.78.2/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/blip2_image_desc_lib.py` & `dvcx-0.78.2/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/common_sql_functions.py` & `dvcx-0.78.2/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/dir_expansion.py` & `dvcx-0.78.2/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/hf_pipeline.py` & `dvcx-0.78.2/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/llava2_image_desc_lib.py` & `dvcx-0.78.2/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/llm-claude-aggregate-query.py` & `dvcx-0.78.2/examples/llm-claude-aggregate-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/llm-claude-simple-query.py` & `dvcx-0.78.2/examples/llm-claude-simple-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/llm-claude.py` & `dvcx-0.78.2/examples/llm-claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/loader.py` & `dvcx-0.78.2/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/neurips/README` & `dvcx-0.78.2/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/neurips/distance_to_query.py` & `dvcx-0.78.2/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/neurips/llm_chat.py` & `dvcx-0.78.2/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/neurips/single_query.py` & `dvcx-0.78.2/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/neurips/text_loaders.py` & `dvcx-0.78.2/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/openai_image_desc_lib.py` & `dvcx-0.78.2/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/openimage-detect.py` & `dvcx-0.78.2/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/pose_detection.py` & `dvcx-0.78.2/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/torch-loader.py` & `dvcx-0.78.2/examples/torch-loader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # pip install Pillow torchvision
 
 import torch
 from torch import nn, optim
 from torch.utils.data import DataLoader
 from torchvision.transforms import v2
 
-from dvcx.lib.param import Image, Label
-from dvcx.query import C, DatasetQuery, udf
-from dvcx.sql.types import String
+from dvcx.lib.dataset import C, Dataset
+from dvcx.lib.image import ImageReader
+from dvcx.lib.reader import LabelReader
 
 STORAGE = "gcs://dvcx-datalakes/dogs-and-cats/"
 
 # Define transformation for data preprocessing
 transform = v2.Compose(
     [
         v2.ToTensor(),
@@ -20,19 +20,14 @@
     ]
 )
 
 
 CLASSES = ["cat", "dog"]
 
 
-@udf(params=("name",), output={"label": String})
-def extract_label(name):
-    return (name[:3],)
-
-
 # Define torch model
 class CNN(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv1 = nn.Conv2d(3, 16, kernel_size=3, stride=2, padding=1)
         self.conv2 = nn.Conv2d(16, 32, kernel_size=3, stride=2, padding=1)
         self.conv3 = nn.Conv2d(32, 64, kernel_size=3, stride=2, padding=1)
@@ -46,18 +41,26 @@
         x = x.view(-1, 64 * 8 * 8)
         x = torch.relu(self.fc1(x))
         x = self.fc2(x)
         return x
 
 
 if __name__ == "__main__":
-    q = DatasetQuery(STORAGE).filter(C.name.glob("*.jpg")).add_signals(extract_label)
+    ds = (
+        Dataset(STORAGE)
+        .filter(C.name.glob("*.jpg"))
+        .map(lambda name: (name[:3],), output={"label": str})
+    )
 
     train_loader = DataLoader(
-        q.to_pytorch(Image(), Label("label", CLASSES), cache=True, transform=transform),
+        ds.to_pytorch(
+            ImageReader(),
+            LabelReader(feature="label", classes=CLASSES),
+            transform=transform,
+        ),
         batch_size=16,
         num_workers=2,
     )
 
     model = CNN()
     criterion = nn.CrossEntropyLoss()
     optimizer = optim.Adam(model.parameters(), lr=0.001)
```

### Comparing `dvcx-0.78.1/examples/udfs/batching.py` & `dvcx-0.78.2/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/udfs/image_transformation.py` & `dvcx-0.78.2/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/udfs/parallel.py` & `dvcx-0.78.2/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/udfs/simple.py` & `dvcx-0.78.2/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/udfs/stateful.py` & `dvcx-0.78.2/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/udfs/stateful_similarity.py` & `dvcx-0.78.2/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/unstructured-text.py` & `dvcx-0.78.2/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/wds.py` & `dvcx-0.78.2/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/wds_filtered.py` & `dvcx-0.78.2/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/wds_meta.py` & `dvcx-0.78.2/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/zalando/zalando_clip.py` & `dvcx-0.78.2/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.78.2/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/noxfile.py` & `dvcx-0.78.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/pyproject.toml` & `dvcx-0.78.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/asyn.py` & `dvcx-0.78.2/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/cache.py` & `dvcx-0.78.2/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/catalog/catalog.py` & `dvcx-0.78.2/src/dvcx/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/catalog/datasource.py` & `dvcx-0.78.2/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/catalog/formats.py` & `dvcx-0.78.2/src/dvcx/catalog/formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/catalog/loader.py` & `dvcx-0.78.2/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/cli.py` & `dvcx-0.78.2/src/dvcx/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1032,16 +1032,20 @@
     except BrokenPipeError:
         # Python flushes standard streams on exit; redirect remaining output
         # to devnull to avoid another BrokenPipeError at shutdown
         # See: https://docs.python.org/3/library/signal.html#note-on-sigpipe
         devnull = os.open(os.devnull, os.O_WRONLY)
         os.dup2(devnull, sys.stdout.fileno())
         return 141  # 128 + 13 (SIGPIPE)
-    except Exception as exc:
-        print("Error:", exc, file=sys.stderr)
+    except (KeyboardInterrupt, Exception) as exc:
+        if isinstance(exc, KeyboardInterrupt):
+            msg = "Operation cancelled by the user"
+        else:
+            msg = str(exc)
+        print("Error:", msg, file=sys.stderr)
         if logging_level <= logging.DEBUG:
             traceback.print_exception(
                 type(exc),
                 exc,
                 exc.__traceback__,
                 file=sys.stderr,
             )
```

### Comparing `dvcx-0.78.1/src/dvcx/cli_utils.py` & `dvcx-0.78.2/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/client/azure.py` & `dvcx-0.78.2/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/client/fileslice.py` & `dvcx-0.78.2/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/client/fsspec.py` & `dvcx-0.78.2/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/client/gcs.py` & `dvcx-0.78.2/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/client/local.py` & `dvcx-0.78.2/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/client/s3.py` & `dvcx-0.78.2/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/config.py` & `dvcx-0.78.2/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/data_storage/db_engine.py` & `dvcx-0.78.2/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/data_storage/id_generator.py` & `dvcx-0.78.2/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/data_storage/metastore.py` & `dvcx-0.78.2/src/dvcx/data_storage/metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/data_storage/schema.py` & `dvcx-0.78.2/src/dvcx/data_storage/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/data_storage/serializer.py` & `dvcx-0.78.2/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/data_storage/sqlite.py` & `dvcx-0.78.2/src/dvcx/data_storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/data_storage/warehouse.py` & `dvcx-0.78.2/src/dvcx/data_storage/warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/dataset.py` & `dvcx-0.78.2/src/dvcx/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/error.py` & `dvcx-0.78.2/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/cached_stream.py` & `dvcx-0.78.2/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/claude.py` & `dvcx-0.78.2/src/dvcx/lib/claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/dataset.py` & `dvcx-0.78.2/src/dvcx/lib/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,17 @@
         Example:
         >>> df.map(lambda name: name[:-4] + ".json", output={"json_file": String}) \
         >>>     .save("new_dataset")
         """
 
         self._validate_args("map()", parallel, workers, min_task_size)
 
+        if output:
+            output = {k: Feature._convert_type(v) for k, v in output.items()}
+
         udf_obj = self._udf_to_obj(udf, Mapper, "map()", params, output, cache=cache)
         return self.add_signals(
             udf_obj.to_udf_wrapper(),
             parallel=parallel,
             workers=workers,
             min_task_size=min_task_size,
             cache=cache,
```

### Comparing `dvcx-0.78.1/src/dvcx/lib/feature.py` & `dvcx-0.78.2/src/dvcx/lib/feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     Array,
     Binary,
     Boolean,
     DateTime,
     Float,
     Int,
     NullType,
+    SQLType,
     String,
 )
 
 TYPE_TO_DVCX = {
     int: Int,
     str: String,
     Literal: String,
@@ -101,15 +102,17 @@
     @staticmethod
     def _to_snake_case(name: str) -> str:
         """Convert a CamelCase name to snake_case."""
         s1 = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", name)
         return re.sub("([a-z0-9])([A-Z])", r"\1_\2", s1).lower()
 
     @staticmethod
-    def _convert_type(typ):
+    def _convert_type(typ):  # noqa: PLR0911
+        if inspect.isclass(typ) and issubclass(typ, SQLType):
+            return typ
         res = TYPE_TO_DVCX.get(typ, None)
         if res:
             return res
 
         orig = get_origin(typ)
 
         if orig in (Literal, LiteralEx):
```

### Comparing `dvcx-0.78.1/src/dvcx/lib/feature_types.py` & `dvcx-0.78.2/src/dvcx/lib/feature_types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/feature_udf.py` & `dvcx-0.78.2/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/file.py` & `dvcx-0.78.2/src/dvcx/lib/file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.78.2/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.78.2/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.78.2/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/image.py` & `dvcx-0.78.2/src/dvcx/lib/image.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,36 +16,33 @@
 
 
 def convert_image(
     img: Image.Image,
     mode: str = "RGB",
     size: Optional[tuple[int, int]] = None,
     transform: Optional[Callable] = None,
-    unsqueeze: bool = True,
     open_clip_model: Optional[Any] = None,
 ):
     """
     Resize, transform, and otherwise convert an image.
 
     Args:
         img (Image): PIL.Image object.
         mode (str): PIL.Image mode.
         size (tuple[int, int]): Size in (width, height) pixels for resizing.
         transform (Callable): Torchvision v1 or other transform to apply.
-        unsqueeze (bool): Apply torch unsqueeze operation. Ignored if no transform
-            provided.
         open_clip_model (Any): Encode image using model from open_clip library.
     """
     if mode:
         img = img.convert(mode)
     if size:
         img = img.resize(size)
     if transform:
         img = transform(img)
-        if unsqueeze:
+        if open_clip_model:
             img = img.unsqueeze(0)  # type: ignore
     if open_clip_model:
         method_name = "encode_image"
         if not (
             hasattr(open_clip_model, method_name)
             and inspect.ismethod(getattr(open_clip_model, method_name))
         ):
@@ -59,32 +56,29 @@
 
 class ImageReader(FeatureReader):
     def __init__(
         self,
         mode: str = "RGB",
         size: Optional[tuple[int, int]] = None,
         transform: Optional[Callable] = None,
-        unsqueeze: bool = True,
         open_clip_model: Any = None,
     ):
         """
         Read and optionally transform an image.
 
         All kwargs are passed to `convert_image()`.
         """
         self.mode = mode
         self.size = size
         self.transform = transform
-        self.unsqueeze = unsqueeze
         self.open_clip_model = open_clip_model
         super().__init__(BinaryFile)
 
     def __call__(self, value: bytes):
         img = Image.open(BytesIO(value))
         return convert_image(
             img,
             mode=self.mode,
             size=self.size,
             transform=self.transform,
-            unsqueeze=self.unsqueeze,
             open_clip_model=self.open_clip_model,
         )
```

### Comparing `dvcx-0.78.1/src/dvcx/lib/image_transform.py` & `dvcx-0.78.2/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.78.2/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/pytorch.py` & `dvcx-0.78.2/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/reader.py` & `dvcx-0.78.2/src/dvcx/lib/reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/tar_file.py` & `dvcx-0.78.2/src/dvcx/lib/tar_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/text.py` & `dvcx-0.78.2/src/dvcx/lib/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     tokens = (
         res.input_ids[0] if isinstance(tokenizer, PreTrainedTokenizerBase) else res[0]
     )
     if not open_clip_model:
         return tokens
 
-    return open_clip_model.encode_text(tokens)
+    return open_clip_model.encode_text(tokens.unsqueeze(0))
 
 
 class TextReader(FeatureReader):
     def __init__(
         self,
         fr_class: "FeatureLike" = TextFile,
         tokenizer: Optional[Callable] = None,
```

### Comparing `dvcx-0.78.1/src/dvcx/lib/udf.py` & `dvcx-0.78.2/src/dvcx/lib/udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import inspect
 import types
-from abc import ABC
 from typing import TYPE_CHECKING, Callable
 
 from dvcx.catalog import get_catalog
 from dvcx.query import udf
 from dvcx.query.schema import DatasetRow
 from dvcx.sql.types import Int, String
 
 if TYPE_CHECKING:
     from dvxc.query.udf import UDFWrapper
     from typing_extensions import Self
 
 
-class UDFBase(ABC):
+class UDFBase:
     DEF_OUTPUT_NAME = "result"
     DEF_OUTPUT_TYPE = String
 
     def __init__(self, params=None, output=None, batch=1):
         sign_params, sign_output = self._get_signature(self.process)
 
         self._params = params or sign_params
@@ -56,20 +55,20 @@
     def catalog(self):
         return self._catalog
 
     def to_udf_wrapper(self) -> "UDFWrapper":
         udf_wrapper = udf(params=self.params, output=self.output, batch=self.batch)
         return udf_wrapper(self)
 
-    def bootstrap(self):  # noqa: B027
+    def bootstrap(self):
         """Initialization process executed on each worker before processing begins.
         This is needed for tasks like pre-loading ML models prior to scoring.
         """
 
-    def teardown(self):  # noqa: B027
+    def teardown(self):
         """Teardown process executed on each process/worker after processing ends.
         This is needed for tasks like closing connections to end-points.
         """
 
     def process(self, *args, **kwargs):
         """Abstract processing method that needs to be re-defined in child classes."""
         NotImplementedError(f"UDF processing is not implemented in class {self.name}")
```

### Comparing `dvcx-0.78.1/src/dvcx/lib/unstructured.py` & `dvcx-0.78.2/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/utils.py` & `dvcx-0.78.2/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/webdataset.py` & `dvcx-0.78.2/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.78.2/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.78.2/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/listing.py` & `dvcx-0.78.2/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/node.py` & `dvcx-0.78.2/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/nodes_fetcher.py` & `dvcx-0.78.2/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/nodes_thread_pool.py` & `dvcx-0.78.2/src/dvcx/nodes_thread_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 self.update_progress_bar(progress_bar)
 
             th_pool.shutdown()
 
         return results
 
     def update_progress_bar(self, progress_bar):
-        if progress_bar:
+        if progress_bar is not None:
             with self._thread_lock:
                 if self._thread_counter:
                     progress_bar.update(self._thread_counter)
                     self._thread_counter = 0
 
     def increase_counter(self, value):
         with self._thread_lock:
```

### Comparing `dvcx-0.78.1/src/dvcx/progress.py` & `dvcx-0.78.2/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/query/batch.py` & `dvcx-0.78.2/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/query/builtins.py` & `dvcx-0.78.2/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/query/dataset.py` & `dvcx-0.78.2/src/dvcx/query/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1708,18 +1708,21 @@
     preview: list[dict] = attrs.field(factory=list)
     dataset: Optional[tuple[str, int]] = None
 
 
 def _send_result(
     dataset_query: DatasetQuery, dataset: Optional[tuple[str, int]] = None
 ):
-    def _json_serialize(obj):
-        if isinstance(obj, (datetime.datetime, datetime.date)):
-            return obj.isoformat()
-        return obj
+    class JSONSerialize(json.JSONEncoder):
+        def default(self, obj):
+            if isinstance(obj, (datetime.datetime, datetime.date)):
+                return obj.isoformat()
+            if isinstance(obj, bytes):
+                return [f"{b:02x}" for b in obj[:1024]]
+            return super().default(obj)
 
     try:
         preview_args: dict[str, Any] = json.loads(
             os.getenv("DVCX_QUERY_PREVIEW_ARGS", "")
         )
     except ValueError:
         preview_args = {}
@@ -1735,15 +1738,15 @@
     )
 
     preview = preview_query.to_records()
     result = ExecutionResult(preview, dataset)
     data = attrs.asdict(result)
 
     with open(_get_output_fd_for_write(), mode="w") as f:
-        json.dump(data, f, default=_json_serialize)
+        json.dump(data, f, cls=JSONSerialize)
 
 
 def query_wrapper(dataset_query: DatasetQuery) -> DatasetQuery:
     """
     Wrapper function that wraps the last statement of user query script.
     Last statement MUST be instance of DatasetQuery, otherwise script exits with
     error code 10
```

### Comparing `dvcx-0.78.1/src/dvcx/query/dispatch.py` & `dvcx-0.78.2/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/query/params.py` & `dvcx-0.78.2/src/dvcx/query/params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/query/schema.py` & `dvcx-0.78.2/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/query/session.py` & `dvcx-0.78.2/src/dvcx/query/session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/query/udf.py` & `dvcx-0.78.2/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/remote/studio.py` & `dvcx-0.78.2/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/sql/default/base.py` & `dvcx-0.78.2/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/sql/functions/array.py` & `dvcx-0.78.2/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/sql/functions/path.py` & `dvcx-0.78.2/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/sql/selectable.py` & `dvcx-0.78.2/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/sql/sqlite/base.py` & `dvcx-0.78.2/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/sql/sqlite/types.py` & `dvcx-0.78.2/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/sql/types.py` & `dvcx-0.78.2/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/sql/utils.py` & `dvcx-0.78.2/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/storage.py` & `dvcx-0.78.2/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx/utils.py` & `dvcx-0.78.2/src/dvcx/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.78.2/src/dvcx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.78.1
+Version: 0.78.2
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.78.1/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.78.2/src/dvcx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/src/dvcx.egg-info/requires.txt` & `dvcx-0.78.2/src/dvcx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/benchmarks/conftest.py` & `dvcx-0.78.2/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/conftest.py` & `dvcx-0.78.2/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -365,14 +365,20 @@
         if "all" in skip_missing_remotes or cloud_type in skip_missing_remotes:
             pytest.skip(str(exc))
         raise
 
     return make_cloud_server(src_path, cloud_type, tree)
 
 
+@pytest.fixture()
+def dvcx_job_id(monkeypatch):
+    job_id = uuid.uuid4().hex
+    monkeypatch.setenv("DVCX_JOB_ID", job_id)
+
+
 @pytest.fixture
 def cloud_server_credentials(cloud_server, monkeypatch):
     if cloud_server.kind == "s3":
         cfg = cloud_server.src.fs.client_kwargs
         try:
             monkeypatch.delenv("AWS_PROFILE")
         except KeyError:
```

### Comparing `dvcx-0.78.1/tests/data.py` & `dvcx-0.78.2/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/func/test_catalog.py` & `dvcx-0.78.2/tests/func/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/func/test_client.py` & `dvcx-0.78.2/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/func/test_dataset_query.py` & `dvcx-0.78.2/tests/func/test_dataset_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1025,15 +1025,15 @@
 )
 @pytest.mark.parametrize("batch", [False, True])
 @pytest.mark.parametrize("workers", (1, 2))
 @pytest.mark.skipif(
     "not os.environ.get('DVCX_DISTRIBUTED')",
     reason="Set the DVCX_DISTRIBUTED environment variable to test distributed UDFs",
 )
-def test_udf_distributed(cloud_test_catalog_tmpfile, batch, workers):
+def test_udf_distributed(cloud_test_catalog_tmpfile, batch, workers, dvcx_job_id):
     catalog = cloud_test_catalog_tmpfile.catalog
     sources = [cloud_test_catalog_tmpfile.src_uri]
     globs = [s.rstrip("/") + "/*" for s in sources]
     catalog.index(sources)
     catalog.create_dataset_from_sources("animals", globs, recursive=True)
 
     @udf(("name",), {"name_len": Int, "blank": String})
@@ -1075,15 +1075,15 @@
     indirect=True,
 )
 @pytest.mark.parametrize("workers", (1, 2))
 @pytest.mark.skipif(
     "not os.environ.get('DVCX_DISTRIBUTED')",
     reason="Set the DVCX_DISTRIBUTED environment variable to test distributed UDFs",
 )
-def test_udf_distributed_exec_error(cloud_test_catalog_tmpfile, workers):
+def test_udf_distributed_exec_error(cloud_test_catalog_tmpfile, workers, dvcx_job_id):
     catalog = cloud_test_catalog_tmpfile.catalog
     sources = [cloud_test_catalog_tmpfile.src_uri]
     globs = [s.rstrip("/") + "/*" for s in sources]
     catalog.index(sources)
     catalog.create_dataset_from_sources("animals", globs, recursive=True)
 
     @udf((C.name,), {"name_len": Int})
@@ -1106,15 +1106,15 @@
     [("s3", True)],
     indirect=True,
 )
 @pytest.mark.skipif(
     "not os.environ.get('DVCX_DISTRIBUTED')",
     reason="Set the DVCX_DISTRIBUTED environment variable to test distributed UDFs",
 )
-def test_udf_distributed_interrupt(cloud_test_catalog_tmpfile, capfd):
+def test_udf_distributed_interrupt(cloud_test_catalog_tmpfile, capfd, dvcx_job_id):
     catalog = cloud_test_catalog_tmpfile.catalog
     sources = [cloud_test_catalog_tmpfile.src_uri]
     globs = [s.rstrip("/") + "/*" for s in sources]
     catalog.index(sources)
     catalog.create_dataset_from_sources("animals", globs, recursive=True)
 
     @udf(("name",), {"name_len": Int})
@@ -1140,37 +1140,36 @@
     [("s3", True)],
     indirect=True,
 )
 @pytest.mark.skipif(
     "not os.environ.get('DVCX_DISTRIBUTED')",
     reason="Set the DVCX_DISTRIBUTED environment variable to test distributed UDFs",
 )
-def test_udf_distributed_cancel(cloud_test_catalog_tmpfile, capfd, monkeypatch):
+def test_udf_distributed_cancel(cloud_test_catalog_tmpfile, capfd, dvcx_job_id):
     catalog = cloud_test_catalog_tmpfile.catalog
     metastore = catalog.metastore
     sources = [cloud_test_catalog_tmpfile.src_uri]
     globs = [s.rstrip("/") + "/*" for s in sources]
     catalog.index(sources)
     catalog.create_dataset_from_sources("animals", globs, recursive=True)
 
-    job_id = "a53bb062dfdf437baf6003795a62d17d"
+    job_id = os.environ.get("DVCX_JOB_ID")
 
     # A job is required for query script cancellation (not using a KeyboardInterrupt)
     metastore.db.execute(
         metastore._jobs_insert().values(
             id=job_id,
             status=7,  # CANCELING
             celery_task_id="",
             name="Test Cancel Job",
             workers=2,
             team_id=metastore.team_id,
             created_at=datetime.now(timezone.utc),
         ),
     )
-    monkeypatch.setenv("DVCX_JOB_ID", job_id)
 
     @udf(("name",), {"name_len": Int})
     def name_len_slow(name):
         # A very simple udf, that processes slowly to emulate being stuck.
         from time import sleep
 
         sleep(10)
@@ -3279,14 +3278,15 @@
 
     if method == "to_records":
 
         def get_result(query):
             result = [(r["name"], r["name_len"]) for r in query.to_records()]
             result.sort()
             return result
+
     elif method == "extract":
 
         def get_result(query):
             result = list(query.extract("name", "name_len"))
             result.sort()
             return result
 
@@ -3344,14 +3344,15 @@
 
     if method == "to_records":
 
         def get_result(query):
             result = [(r["name"], r["x"], r["name_len"]) for r in query.to_records()]
             result.sort()
             return result
+
     elif method == "extract":
 
         def get_result(query):
             return sorted(query.extract("name", "x", "name_len"))
 
     q = q1.union(q2).add_signals(name_len)
     result1 = get_result(q)
@@ -3412,14 +3413,15 @@
         def get_result(query):
             return (
                 query.limit(100)
                 .add_signals(name_int)
                 .select("name", "name_int")
                 .to_records()
             )
+
     elif method == "extract":
 
         def get_result(query):
             data = query.limit(100).add_signals(name_int).extract("name", "name_int")
             return [{"name": name, "name_int": name_int} for name, name_int in data]
 
     expected = [{"name": f"{i:06d}", "name_int": i} for i in range(100)]
```

### Comparing `dvcx-0.78.1/tests/func/test_datasets.py` & `dvcx-0.78.2/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/func/test_ls.py` & `dvcx-0.78.2/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/func/test_pull.py` & `dvcx-0.78.2/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/func/test_pytorch.py` & `dvcx-0.78.2/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/func/test_query.py` & `dvcx-0.78.2/tests/func/test_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/scripts/name_len_normal.py` & `dvcx-0.78.2/tests/scripts/name_len_normal.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/scripts/name_len_slow.py` & `dvcx-0.78.2/tests/scripts/name_len_slow.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/test_cli_e2e.py` & `dvcx-0.78.2/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/test_query_e2e.py` & `dvcx-0.78.2/tests/test_query_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/lib/test_cached_stream.py` & `dvcx-0.78.2/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/lib/test_feature.py` & `dvcx-0.78.2/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/lib/test_feature_udf.py` & `dvcx-0.78.2/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/lib/test_file.py` & `dvcx-0.78.2/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/lib/test_image.py` & `dvcx-0.78.2/tests/unit/lib/test_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     img.save(file_path)
 
     converted_img = convert_image(
         img,
         mode="RGBA",
         size=(32, 32),
         transform=ToTensor(),
-        unsqueeze=False,
     )
     assert isinstance(converted_img, Tensor)
     assert converted_img.size() == (4, 32, 32)
 
 
 def test_image_file_reader(tmp_path, catalog, mocker):
     file_name = "img.jpg"
@@ -31,15 +30,14 @@
     img = Image.new(mode="RGB", size=(64, 64))
     img.save(file_path)
 
     kwargs = {
         "mode": "RGBA",
         "size": (32, 32),
         "transform": ToTensor(),
-        "unsqueeze": False,
         "open_clip_model": None,
     }
     reader = ImageReader(**kwargs)
     file = File(name=file_name, source=f"file://{tmp_path}")
     file.set_catalog(catalog)
 
     convert_image = mocker.patch("dvcx.lib.image.convert_image")
```

### Comparing `dvcx-0.78.1/tests/unit/lib/test_reader.py` & `dvcx-0.78.2/tests/unit/lib/test_reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/lib/test_text.py` & `dvcx-0.78.2/tests/unit/lib/test_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/lib/test_webdataset.py` & `dvcx-0.78.2/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.78.2/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/sql/test_array.py` & `dvcx-0.78.2/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/sql/test_conditional.py` & `dvcx-0.78.2/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/sql/test_path.py` & `dvcx-0.78.2/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/sql/test_selectable.py` & `dvcx-0.78.2/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/sql/test_string.py` & `dvcx-0.78.2/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_asyn.py` & `dvcx-0.78.2/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_cache.py` & `dvcx-0.78.2/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_catalog.py` & `dvcx-0.78.2/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_catalog_formats.py` & `dvcx-0.78.2/tests/unit/test_catalog_formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_catalog_loader.py` & `dvcx-0.78.2/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_cli_parsing.py` & `dvcx-0.78.2/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_client.py` & `dvcx-0.78.2/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_client_s3.py` & `dvcx-0.78.2/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_data_storage.py` & `dvcx-0.78.2/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_database_engine.py` & `dvcx-0.78.2/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_dataset.py` & `dvcx-0.78.2/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_dataset_row.py` & `dvcx-0.78.2/tests/unit/test_dataset_row.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_dispatch.py` & `dvcx-0.78.2/tests/unit/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_fileslice.py` & `dvcx-0.78.2/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_id_generator.py` & `dvcx-0.78.2/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_listing.py` & `dvcx-0.78.2/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_metastore.py` & `dvcx-0.78.2/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_query_params.py` & `dvcx-0.78.2/tests/unit/test_query_params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_serializer.py` & `dvcx-0.78.2/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_session.py` & `dvcx-0.78.2/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_storage.py` & `dvcx-0.78.2/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_udf.py` & `dvcx-0.78.2/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_utils.py` & `dvcx-0.78.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/unit/test_warehouse.py` & `dvcx-0.78.2/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.1/tests/utils.py` & `dvcx-0.78.2/tests/utils.py`

 * *Files identical despite different names*

