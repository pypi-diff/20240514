# Comparing `tmp/deriva-1.7.0.tar.gz` & `tmp/deriva-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deriva-1.7.0.tar", last modified: Fri Mar 15 22:05:46 2024, max compression
+gzip compressed data, was "deriva-1.7.1.tar", last modified: Tue May 14 20:16:44 2024, max compression
```

## Comparing `deriva-1.7.0.tar` & `deriva-1.7.1.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.187076 deriva-1.7.0/
--rw-rw-rw-   0        0        0     1087 2024-02-21 06:15:46.000000 deriva-1.7.0/.gitignore
--rw-rw-rw-   0        0        0      415 2024-02-21 06:15:46.000000 deriva-1.7.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    11357 2024-02-21 06:15:46.000000 deriva-1.7.0/LICENSE
--rw-rw-rw-   0        0        0     1616 2024-03-15 22:05:46.187076 deriva-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1847 2024-02-21 06:15:46.000000 deriva-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.016795 deriva-1.7.0/deriva/
--rw-rw-rw-   0        0        0       64 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.040743 deriva-1.7.0/deriva/config/
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/config/__init__.py
--rw-rw-rw-   0        0        0    23946 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/config/acl_config.py
--rw-rw-rw-   0        0        0    11732 2024-03-14 22:27:48.000000 deriva-1.7.0/deriva/config/annotation_config.py
--rw-rw-rw-   0        0        0     5228 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/config/annotation_validate.py
--rw-rw-rw-   0        0        0    20724 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/config/base_config.py
--rw-rw-rw-   0        0        0     9362 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/config/dump_catalog_annotations.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.042891 deriva-1.7.0/deriva/config/examples/
--rw-rw-rw-   0        0        0     2408 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/config/examples/group_owner_policy.json
--rw-rw-rw-   0        0        0     1676 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/config/examples/self_serve_policy.json
--rw-rw-rw-   0        0        0     3020 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/config/rollback_annotation.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.058730 deriva-1.7.0/deriva/core/
--rw-rw-rw-   0        0        0     4945 2024-03-15 21:04:26.000000 deriva-1.7.0/deriva/core/__init__.py
--rw-rw-rw-   0        0        0    13432 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/annotation.py
--rw-rw-rw-   0        0        0     2681 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/base_cli.py
--rw-rw-rw-   0        0        0    21253 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/catalog_cli.py
--rw-rw-rw-   0        0        0    67548 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/datapath.py
--rw-rw-rw-   0        0        0    12970 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/deriva_binding.py
--rw-rw-rw-   0        0        0      200 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/deriva_server.py
--rw-rw-rw-   0        0        0    50817 2024-03-14 22:27:48.000000 deriva-1.7.0/deriva/core/ermrest_catalog.py
--rw-rw-rw-   0        0        0    85916 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/ermrest_model.py
--rw-rw-rw-   0        0        0    14522 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/hatrac_cli.py
--rw-rw-rw-   0        0        0    22582 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/hatrac_store.py
--rw-rw-rw-   0        0        0    10351 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/polling_ermrest_catalog.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.075704 deriva-1.7.0/deriva/core/schemas/
--rw-rw-rw-   0        0        0      954 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/app_links.schema.json
--rw-rw-rw-   0        0        0     1287 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/asset.schema.json
--rw-rw-rw-   0        0        0     7387 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/bulk_upload.schema.json
--rw-rw-rw-   0        0        0      363 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/chaise_config.schema.json
--rw-rw-rw-   0        0        0     1023 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/citation.schema.json
--rw-rw-rw-   0        0        0     1720 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/column_display.schema.json
--rw-rw-rw-   0        0        0     1461 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/display.schema.json
--rw-rw-rw-   0        0        0     2147 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/export.schema.json
--rw-rw-rw-   0        0        0      623 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/export_2019.schema.json
--rw-rw-rw-   0        0        0     1550 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/foreign_key.schema.json
--rw-rw-rw-   0        0        0      324 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/generated.schema.json
--rw-rw-rw-   0        0        0      324 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/immutable.schema.json
--rw-rw-rw-   0        0        0      546 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/indexing_preferences.schema.json
--rw-rw-rw-   0        0        0     1017 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/key_display.schema.json
--rw-rw-rw-   0        0        0      267 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/non_deletable.schema.json
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/required.schema.json
--rw-rw-rw-   0        0        0     8590 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/source_definitions.schema.json
--rw-rw-rw-   0        0        0      708 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/table_alternatives.schema.json
--rw-rw-rw-   0        0        0     1617 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/table_display.schema.json
--rw-rw-rw-   0        0        0     6500 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/visible_columns.schema.json
--rw-rw-rw-   0        0        0     3364 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/schemas/visible_foreign_keys.schema.json
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.076753 deriva-1.7.0/deriva/core/tests/
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.083082 deriva-1.7.0/deriva/core/utils/
--rw-rw-rw-   0        0        0      124 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/utils/__init__.py
--rw-rw-rw-   0        0        0    19500 2024-03-14 22:27:48.000000 deriva-1.7.0/deriva/core/utils/core_utils.py
--rw-rw-rw-   0        0        0    55601 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/utils/globus_auth_utils.py
--rw-rw-rw-   0        0        0     2299 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/utils/hash_utils.py
--rw-rw-rw-   0        0        0     1128 2024-03-14 22:27:48.000000 deriva-1.7.0/deriva/core/utils/mime_utils.py
--rw-rw-rw-   0        0        0     2954 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/utils/version_utils.py
--rw-rw-rw-   0        0        0     3809 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/core/utils/webauthn_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.086245 deriva-1.7.0/deriva/seo/
--rw-rw-rw-   0        0        0     2134 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/seo/README.md
--rw-rw-rw-   0        0        0       54 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/seo/__init__.py
--rw-rw-rw-   0        0        0    13948 2024-03-14 22:27:48.000000 deriva-1.7.0/deriva/seo/sitemap_builder.py
--rw-rw-rw-   0        0        0     2654 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/seo/sitemap_cli.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.087295 deriva-1.7.0/deriva/transfer/
--rw-rw-rw-   0        0        0     1099 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.090574 deriva-1.7.0/deriva/transfer/backup/
--rw-rw-rw-   0        0        0      465 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/backup/__init__.py
--rw-rw-rw-   0        0        0      361 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/backup/__main__.py
--rw-rw-rw-   0        0        0     5228 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/backup/deriva_backup.py
--rw-rw-rw-   0        0        0     2157 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/backup/deriva_backup_cli.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.093726 deriva-1.7.0/deriva/transfer/download/
--rw-rw-rw-   0        0        0      294 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/__init__.py
--rw-rw-rw-   0        0        0      363 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/__main__.py
--rw-rw-rw-   0        0        0    16201 2024-03-04 23:18:12.000000 deriva-1.7.0/deriva/transfer/download/deriva_download.py
--rw-rw-rw-   0        0        0     3878 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/deriva_download_cli.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.095911 deriva-1.7.0/deriva/transfer/download/processors/
--rw-rw-rw-   0        0        0     4507 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/__init__.py
--rw-rw-rw-   0        0        0     3837 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/base_processor.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.099012 deriva-1.7.0/deriva/transfer/download/processors/postprocess/
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/postprocess/__init__.py
--rw-rw-rw-   0        0        0     5370 2024-03-07 07:07:18.000000 deriva-1.7.0/deriva/transfer/download/processors/postprocess/identifier_post_processor.py
--rw-rw-rw-   0        0        0     7828 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/postprocess/transfer_post_processor.py
--rw-rw-rw-   0        0        0     2745 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/postprocess/url_post_processor.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.103267 deriva-1.7.0/deriva/transfer/download/processors/query/
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/query/__init__.py
--rw-rw-rw-   0        0        0     5645 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/query/bag_fetch_query_processor.py
--rw-rw-rw-   0        0        0    10192 2024-03-07 06:48:41.000000 deriva-1.7.0/deriva/transfer/download/processors/query/base_query_processor.py
--rw-rw-rw-   0        0        0     7257 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/query/file_download_query_processor.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.109577 deriva-1.7.0/deriva/transfer/download/processors/transform/
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/transform/__init__.py
--rw-rw-rw-   0        0        0     4109 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/transform/base_transform_processor.py
--rw-rw-rw-   0        0        0     2627 2024-03-14 22:29:14.000000 deriva-1.7.0/deriva/transfer/download/processors/transform/column_transform_processor.py
--rw-rw-rw-   0        0        0     2387 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/transform/fasta_transform_processor.py
--rw-rw-rw-   0        0        0     1790 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/transform/format_transform_processor.py
--rw-rw-rw-   0        0        0    52965 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/transform/geo_transform_processor.py
--rw-rw-rw-   0        0        0     4165 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/processors/transform/string_transform_processor.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.125408 deriva-1.7.0/deriva/transfer/download/tests/
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/__init__.py
--rw-rw-rw-   0        0        0     1371 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test1.json
--rw-rw-rw-   0        0        0     1663 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test10.json
--rw-rw-rw-   0        0        0      740 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test11.json
--rw-rw-rw-   0        0        0     1353 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test12.json
--rw-rw-rw-   0        0        0     1297 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test13.json
--rw-rw-rw-   0        0        0     1597 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test14.json
--rw-rw-rw-   0        0        0     1572 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test15.json
--rw-rw-rw-   0        0        0     1601 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test16.json
--rw-rw-rw-   0        0        0    11080 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test19.json
--rw-rw-rw-   0        0        0      925 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test2.json
--rw-rw-rw-   0        0        0     7695 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test20.json
--rw-rw-rw-   0        0        0     3182 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test3.json
--rw-rw-rw-   0        0        0     1560 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test4.json
--rw-rw-rw-   0        0        0      769 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test5.json
--rw-rw-rw-   0        0        0      823 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test6.json
--rw-rw-rw-   0        0        0     1744 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test7.json
--rw-rw-rw-   0        0        0     4456 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test8.json
--rw-rw-rw-   0        0        0     2506 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/download/tests/test9.json
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.128875 deriva-1.7.0/deriva/transfer/restore/
--rw-rw-rw-   0        0        0      234 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/restore/__init__.py
--rw-rw-rw-   0        0        0      364 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/restore/__main__.py
--rw-rw-rw-   0        0        0    30298 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/restore/deriva_restore.py
--rw-rw-rw-   0        0        0     5603 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/restore/deriva_restore_cli.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.133049 deriva-1.7.0/deriva/transfer/upload/
--rw-rw-rw-   0        0        0      239 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/upload/__init__.py
--rw-rw-rw-   0        0        0      340 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/upload/__main__.py
--rw-rw-rw-   0        0        0    60075 2024-03-14 22:27:48.000000 deriva-1.7.0/deriva/transfer/upload/deriva_upload.py
--rw-rw-rw-   0        0        0     5016 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/upload/deriva_upload_cli.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.138481 deriva-1.7.0/deriva/transfer/upload/processors/
--rw-rw-rw-   0        0        0     2481 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/upload/processors/__init__.py
--rw-rw-rw-   0        0        0     2015 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/upload/processors/archive_processor.py
--rw-rw-rw-   0        0        0      666 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/upload/processors/base_processor.py
--rw-rw-rw-   0        0        0      844 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/upload/processors/logging_processor.py
--rw-rw-rw-   0        0        0     1126 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/upload/processors/metadata_update_processor.py
--rw-rw-rw-   0        0        0     2423 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/upload/processors/rename_processor.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.139572 deriva-1.7.0/deriva/transfer/upload/tests/
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/transfer/upload/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.140630 deriva-1.7.0/deriva/utils/
--rw-rw-rw-   0        0        0       65 2024-02-21 06:15:46.000000 deriva-1.7.0/deriva/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.186015 deriva-1.7.0/deriva.egg-info/
--rw-rw-rw-   0        0        0     1616 2024-03-15 22:05:45.000000 deriva-1.7.0/deriva.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6635 2024-03-15 22:05:45.000000 deriva-1.7.0/deriva.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 22:05:45.000000 deriva-1.7.0/deriva.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      786 2024-03-15 22:05:45.000000 deriva-1.7.0/deriva.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      172 2024-03-15 22:05:45.000000 deriva-1.7.0/deriva.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-15 22:05:45.000000 deriva-1.7.0/deriva.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.153276 deriva-1.7.0/docs/
--rw-rw-rw-   0        0        0     2002 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/BUILD.md
--rw-rw-rw-   0        0        0      606 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/Makefile
--rw-rw-rw-   0        0        0    17368 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/README.md
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.154278 deriva-1.7.0/docs/_static/
--rw-rw-rw-   0        0        0       56 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/_static/README.txt
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.166527 deriva-1.7.0/docs/api/
--rw-rw-rw-   0        0        0      921 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.config.rst
--rw-rw-rw-   0        0        0     3308 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.core.rst
--rw-rw-rw-   0        0        0     1112 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.core.utils.rst
--rw-rw-rw-   0        0        0      292 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.rst
--rw-rw-rw-   0        0        0      240 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.seo.rst
--rw-rw-rw-   0        0        0      644 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.transfer.backup.rst
--rw-rw-rw-   0        0        0     1227 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.transfer.download.processors.postprocess.rst
--rw-rw-rw-   0        0        0     1166 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.transfer.download.processors.query.rst
--rw-rw-rw-   0        0        0      687 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.transfer.download.processors.rst
--rw-rw-rw-   0        0        0      261 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.transfer.download.processors.transform.rst
--rw-rw-rw-   0        0        0      744 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.transfer.download.rst
--rw-rw-rw-   0        0        0      643 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.transfer.restore.rst
--rw-rw-rw-   0        0        0      322 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.transfer.rst
--rw-rw-rw-   0        0        0      633 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/api/deriva.transfer.upload.rst
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.179228 deriva-1.7.0/docs/cli/
--rw-rw-rw-   0        0        0      959 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/cli/commands.md
--rw-rw-rw-   0        0        0    13695 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/cli/deriva-acl-config.md
--rw-rw-rw-   0        0        0     8021 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/cli/deriva-annotation-config.md
--rw-rw-rw-   0        0        0     7899 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/cli/deriva-annotation-validate.md
--rw-rw-rw-   0        0        0     4780 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/cli/deriva-backup-cli.md
--rw-rw-rw-   0        0        0    24112 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/cli/deriva-download-cli.md
--rw-rw-rw-   0        0        0     3746 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/cli/deriva-hatrac-cli.md
--rw-rw-rw-   0        0        0     7228 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/cli/deriva-restore-cli.md
--rw-rw-rw-   0        0        0     2009 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/cli/deriva-sitemap-cli.md
--rw-rw-rw-   0        0        0     5904 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/conf.py
--rw-rw-rw-   0        0        0     6549 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/derivapy-catalog-snapshot.ipynb
--rw-rw-rw-   0        0        0     3143 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/derivapy-catalog.ipynb
--rw-rw-rw-   0        0        0     8929 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/derivapy-datapath-example-1.ipynb
--rw-rw-rw-   0        0        0    19838 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/derivapy-datapath-example-2.ipynb
--rw-rw-rw-   0        0        0    17351 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/derivapy-datapath-example-3.ipynb
--rw-rw-rw-   0        0        0   104075 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/derivapy-datapath-example-4.ipynb
--rw-rw-rw-   0        0        0    11326 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/derivapy-datapath-update.ipynb
--rw-rw-rw-   0        0        0     2491 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/get-started.ipynb
--rw-rw-rw-   0        0        0      490 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/index.rst
--rw-rw-rw-   0        0        0      776 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/install.md
--rwxrwxrwx   0        0        0      777 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/make.bat
--rw-rw-rw-   0        0        0    27593 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/project-tutorial.md
--rw-rw-rw-   0        0        0     3671 2024-02-21 06:15:46.000000 deriva-1.7.0/docs/using-r.md
--rw-rw-rw-   0        0        0      124 2024-02-21 06:15:46.000000 deriva-1.7.0/requirements_dev.txt
--rw-rw-rw-   0        0        0      110 2024-03-15 22:05:46.188136 deriva-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     3286 2024-03-15 17:34:39.000000 deriva-1.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.180340 deriva-1.7.0/tests/
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.181514 deriva-1.7.0/tests/deriva/
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.0/tests/deriva/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 22:05:46.183867 deriva-1.7.0/tests/deriva/core/
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.0/tests/deriva/core/__init__.py
--rw-rw-rw-   0        0        0    36023 2024-03-14 22:27:48.000000 deriva-1.7.0/tests/deriva/core/test_datapath.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:44.097725 deriva-1.7.1/
+-rw-rw-rw-   0        0        0     1087 2024-02-21 06:15:46.000000 deriva-1.7.1/.gitignore
+-rw-rw-rw-   0        0        0     1208 2024-04-16 01:40:25.000000 deriva-1.7.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0    11357 2024-02-21 06:15:46.000000 deriva-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0     1616 2024-05-14 20:16:44.097725 deriva-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1847 2024-02-21 06:15:46.000000 deriva-1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.740099 deriva-1.7.1/deriva/
+-rw-rw-rw-   0        0        0       64 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.763848 deriva-1.7.1/deriva/config/
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/config/__init__.py
+-rw-rw-rw-   0        0        0    23946 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/config/acl_config.py
+-rw-rw-rw-   0        0        0    11732 2024-03-14 22:27:48.000000 deriva-1.7.1/deriva/config/annotation_config.py
+-rw-rw-rw-   0        0        0     5228 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/config/annotation_validate.py
+-rw-rw-rw-   0        0        0    20724 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/config/base_config.py
+-rw-rw-rw-   0        0        0     9362 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/config/dump_catalog_annotations.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.763848 deriva-1.7.1/deriva/config/examples/
+-rw-rw-rw-   0        0        0     2408 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/config/examples/group_owner_policy.json
+-rw-rw-rw-   0        0        0     1676 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/config/examples/self_serve_policy.json
+-rw-rw-rw-   0        0        0     3020 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/config/rollback_annotation.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.795492 deriva-1.7.1/deriva/core/
+-rw-rw-rw-   0        0        0     4945 2024-04-16 01:40:25.000000 deriva-1.7.1/deriva/core/__init__.py
+-rw-rw-rw-   0        0        0    13432 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/annotation.py
+-rw-rw-rw-   0        0        0     2681 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/base_cli.py
+-rw-rw-rw-   0        0        0    23273 2024-04-16 01:53:59.000000 deriva-1.7.1/deriva/core/catalog_cli.py
+-rw-rw-rw-   0        0        0    81306 2024-04-16 01:40:25.000000 deriva-1.7.1/deriva/core/datapath.py
+-rw-rw-rw-   0        0        0    12970 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/deriva_binding.py
+-rw-rw-rw-   0        0        0      200 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/deriva_server.py
+-rw-rw-rw-   0        0        0    50817 2024-03-14 22:27:48.000000 deriva-1.7.1/deriva/core/ermrest_catalog.py
+-rw-rw-rw-   0        0        0    85916 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/ermrest_model.py
+-rw-rw-rw-   0        0        0    14522 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/hatrac_cli.py
+-rw-rw-rw-   0        0        0    22582 2024-04-25 18:40:23.000000 deriva-1.7.1/deriva/core/hatrac_store.py
+-rw-rw-rw-   0        0        0    10351 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/polling_ermrest_catalog.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.826829 deriva-1.7.1/deriva/core/schemas/
+-rw-rw-rw-   0        0        0      954 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/app_links.schema.json
+-rw-rw-rw-   0        0        0     1287 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/asset.schema.json
+-rw-rw-rw-   0        0        0     7387 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/bulk_upload.schema.json
+-rw-rw-rw-   0        0        0      363 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/chaise_config.schema.json
+-rw-rw-rw-   0        0        0     1023 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/citation.schema.json
+-rw-rw-rw-   0        0        0     1720 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/column_display.schema.json
+-rw-rw-rw-   0        0        0     1461 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/display.schema.json
+-rw-rw-rw-   0        0        0     2147 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/export.schema.json
+-rw-rw-rw-   0        0        0      623 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/export_2019.schema.json
+-rw-rw-rw-   0        0        0     1550 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/foreign_key.schema.json
+-rw-rw-rw-   0        0        0      324 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/generated.schema.json
+-rw-rw-rw-   0        0        0      324 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/immutable.schema.json
+-rw-rw-rw-   0        0        0      546 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/indexing_preferences.schema.json
+-rw-rw-rw-   0        0        0     1017 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/key_display.schema.json
+-rw-rw-rw-   0        0        0      267 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/non_deletable.schema.json
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/required.schema.json
+-rw-rw-rw-   0        0        0     8590 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/source_definitions.schema.json
+-rw-rw-rw-   0        0        0      708 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/table_alternatives.schema.json
+-rw-rw-rw-   0        0        0     1617 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/table_display.schema.json
+-rw-rw-rw-   0        0        0     6500 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/visible_columns.schema.json
+-rw-rw-rw-   0        0        0     3364 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/schemas/visible_foreign_keys.schema.json
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.836869 deriva-1.7.1/deriva/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.843762 deriva-1.7.1/deriva/core/utils/
+-rw-rw-rw-   0        0        0      124 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/utils/__init__.py
+-rw-rw-rw-   0        0        0    19500 2024-03-14 22:27:48.000000 deriva-1.7.1/deriva/core/utils/core_utils.py
+-rw-rw-rw-   0        0        0    55601 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/utils/globus_auth_utils.py
+-rw-rw-rw-   0        0        0     2299 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/utils/hash_utils.py
+-rw-rw-rw-   0        0        0     1128 2024-03-14 22:27:48.000000 deriva-1.7.1/deriva/core/utils/mime_utils.py
+-rw-rw-rw-   0        0        0     2954 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/utils/version_utils.py
+-rw-rw-rw-   0        0        0     3809 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/core/utils/webauthn_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.858788 deriva-1.7.1/deriva/seo/
+-rw-rw-rw-   0        0        0     2134 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/seo/README.md
+-rw-rw-rw-   0        0        0       54 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/seo/__init__.py
+-rw-rw-rw-   0        0        0    13948 2024-03-14 22:27:48.000000 deriva-1.7.1/deriva/seo/sitemap_builder.py
+-rw-rw-rw-   0        0        0     2654 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/seo/sitemap_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.859683 deriva-1.7.1/deriva/transfer/
+-rw-rw-rw-   0        0        0     1172 2024-05-14 20:14:05.000000 deriva-1.7.1/deriva/transfer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.859683 deriva-1.7.1/deriva/transfer/backup/
+-rw-rw-rw-   0        0        0      465 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/backup/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/backup/__main__.py
+-rw-rw-rw-   0        0        0     5228 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/backup/deriva_backup.py
+-rw-rw-rw-   0        0        0     2157 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/backup/deriva_backup_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.874697 deriva-1.7.1/deriva/transfer/download/
+-rw-rw-rw-   0        0        0      350 2024-05-14 18:34:21.000000 deriva-1.7.1/deriva/transfer/download/__init__.py
+-rw-rw-rw-   0        0        0      363 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/__main__.py
+-rw-rw-rw-   0        0        0    17145 2024-05-14 18:48:42.000000 deriva-1.7.1/deriva/transfer/download/deriva_download.py
+-rw-rw-rw-   0        0        0     3940 2024-05-14 18:38:27.000000 deriva-1.7.1/deriva/transfer/download/deriva_download_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.874697 deriva-1.7.1/deriva/transfer/download/processors/
+-rw-rw-rw-   0        0        0     4507 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/__init__.py
+-rw-rw-rw-   0        0        0     3837 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/base_processor.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.890348 deriva-1.7.1/deriva/transfer/download/processors/postprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     5370 2024-03-07 07:07:18.000000 deriva-1.7.1/deriva/transfer/download/processors/postprocess/identifier_post_processor.py
+-rw-rw-rw-   0        0        0     7828 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/postprocess/transfer_post_processor.py
+-rw-rw-rw-   0        0        0     2745 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/postprocess/url_post_processor.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.891363 deriva-1.7.1/deriva/transfer/download/processors/query/
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/query/__init__.py
+-rw-rw-rw-   0        0        0     5645 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/query/bag_fetch_query_processor.py
+-rw-rw-rw-   0        0        0    10327 2024-05-14 18:15:33.000000 deriva-1.7.1/deriva/transfer/download/processors/query/base_query_processor.py
+-rw-rw-rw-   0        0        0     7257 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/query/file_download_query_processor.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.907511 deriva-1.7.1/deriva/transfer/download/processors/transform/
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/transform/__init__.py
+-rw-rw-rw-   0        0        0     4109 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/transform/base_transform_processor.py
+-rw-rw-rw-   0        0        0     2627 2024-03-14 22:29:14.000000 deriva-1.7.1/deriva/transfer/download/processors/transform/column_transform_processor.py
+-rw-rw-rw-   0        0        0     2387 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/transform/fasta_transform_processor.py
+-rw-rw-rw-   0        0        0     1790 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/transform/format_transform_processor.py
+-rw-rw-rw-   0        0        0    52965 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/transform/geo_transform_processor.py
+-rw-rw-rw-   0        0        0     4165 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/processors/transform/string_transform_processor.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.954113 deriva-1.7.1/deriva/transfer/download/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/__init__.py
+-rw-rw-rw-   0        0        0     1371 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test1.json
+-rw-rw-rw-   0        0        0     1663 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test10.json
+-rw-rw-rw-   0        0        0      740 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test11.json
+-rw-rw-rw-   0        0        0     1353 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test12.json
+-rw-rw-rw-   0        0        0     1297 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test13.json
+-rw-rw-rw-   0        0        0     1597 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test14.json
+-rw-rw-rw-   0        0        0     1572 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test15.json
+-rw-rw-rw-   0        0        0     1601 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test16.json
+-rw-rw-rw-   0        0        0    11080 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test19.json
+-rw-rw-rw-   0        0        0      925 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test2.json
+-rw-rw-rw-   0        0        0     7695 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test20.json
+-rw-rw-rw-   0        0        0     3182 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test3.json
+-rw-rw-rw-   0        0        0     1560 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test4.json
+-rw-rw-rw-   0        0        0      769 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test5.json
+-rw-rw-rw-   0        0        0      823 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test6.json
+-rw-rw-rw-   0        0        0     1744 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test7.json
+-rw-rw-rw-   0        0        0     4456 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test8.json
+-rw-rw-rw-   0        0        0     2506 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/download/tests/test9.json
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.954113 deriva-1.7.1/deriva/transfer/restore/
+-rw-rw-rw-   0        0        0      234 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/restore/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/restore/__main__.py
+-rw-rw-rw-   0        0        0    30298 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/restore/deriva_restore.py
+-rw-rw-rw-   0        0        0     5603 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/restore/deriva_restore_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.969778 deriva-1.7.1/deriva/transfer/upload/
+-rw-rw-rw-   0        0        0      304 2024-05-14 19:00:30.000000 deriva-1.7.1/deriva/transfer/upload/__init__.py
+-rw-rw-rw-   0        0        0      340 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/upload/__main__.py
+-rw-rw-rw-   0        0        0    60376 2024-05-14 19:00:30.000000 deriva-1.7.1/deriva/transfer/upload/deriva_upload.py
+-rw-rw-rw-   0        0        0     5082 2024-05-14 19:08:40.000000 deriva-1.7.1/deriva/transfer/upload/deriva_upload_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.985819 deriva-1.7.1/deriva/transfer/upload/processors/
+-rw-rw-rw-   0        0        0     2481 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/upload/processors/__init__.py
+-rw-rw-rw-   0        0        0     2015 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/upload/processors/archive_processor.py
+-rw-rw-rw-   0        0        0      666 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/upload/processors/base_processor.py
+-rw-rw-rw-   0        0        0      844 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/upload/processors/logging_processor.py
+-rw-rw-rw-   0        0        0     1126 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/upload/processors/metadata_update_processor.py
+-rw-rw-rw-   0        0        0     2423 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/upload/processors/rename_processor.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.985819 deriva-1.7.1/deriva/transfer/upload/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/transfer/upload/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:43.985819 deriva-1.7.1/deriva/utils/
+-rw-rw-rw-   0        0        0       65 2024-02-21 06:15:46.000000 deriva-1.7.1/deriva/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:44.082073 deriva-1.7.1/deriva.egg-info/
+-rw-rw-rw-   0        0        0     1616 2024-05-14 20:16:43.000000 deriva-1.7.1/deriva.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6635 2024-05-14 20:16:43.000000 deriva-1.7.1/deriva.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 20:16:43.000000 deriva-1.7.1/deriva.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      786 2024-05-14 20:16:43.000000 deriva-1.7.1/deriva.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      172 2024-05-14 20:16:43.000000 deriva-1.7.1/deriva.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-14 20:16:43.000000 deriva-1.7.1/deriva.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:44.040459 deriva-1.7.1/docs/
+-rw-rw-rw-   0        0        0     2002 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/BUILD.md
+-rw-rw-rw-   0        0        0      606 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/Makefile
+-rw-rw-rw-   0        0        0    17368 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:44.040459 deriva-1.7.1/docs/_static/
+-rw-rw-rw-   0        0        0       56 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/_static/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:44.066019 deriva-1.7.1/docs/api/
+-rw-rw-rw-   0        0        0      921 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.config.rst
+-rw-rw-rw-   0        0        0     3308 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.core.rst
+-rw-rw-rw-   0        0        0     1112 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.core.utils.rst
+-rw-rw-rw-   0        0        0      292 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.rst
+-rw-rw-rw-   0        0        0      240 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.seo.rst
+-rw-rw-rw-   0        0        0      644 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.transfer.backup.rst
+-rw-rw-rw-   0        0        0     1227 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.transfer.download.processors.postprocess.rst
+-rw-rw-rw-   0        0        0     1166 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.transfer.download.processors.query.rst
+-rw-rw-rw-   0        0        0      687 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.transfer.download.processors.rst
+-rw-rw-rw-   0        0        0      261 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.transfer.download.processors.transform.rst
+-rw-rw-rw-   0        0        0      744 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.transfer.download.rst
+-rw-rw-rw-   0        0        0      643 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.transfer.restore.rst
+-rw-rw-rw-   0        0        0      322 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.transfer.rst
+-rw-rw-rw-   0        0        0      633 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/api/deriva.transfer.upload.rst
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:44.082073 deriva-1.7.1/docs/cli/
+-rw-rw-rw-   0        0        0      959 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/cli/commands.md
+-rw-rw-rw-   0        0        0    13695 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/cli/deriva-acl-config.md
+-rw-rw-rw-   0        0        0     8021 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/cli/deriva-annotation-config.md
+-rw-rw-rw-   0        0        0     7899 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/cli/deriva-annotation-validate.md
+-rw-rw-rw-   0        0        0     4780 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/cli/deriva-backup-cli.md
+-rw-rw-rw-   0        0        0    24112 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/cli/deriva-download-cli.md
+-rw-rw-rw-   0        0        0     3746 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/cli/deriva-hatrac-cli.md
+-rw-rw-rw-   0        0        0     7228 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/cli/deriva-restore-cli.md
+-rw-rw-rw-   0        0        0     2009 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/cli/deriva-sitemap-cli.md
+-rw-rw-rw-   0        0        0     5904 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/conf.py
+-rw-rw-rw-   0        0        0     6549 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/derivapy-catalog-snapshot.ipynb
+-rw-rw-rw-   0        0        0     3143 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/derivapy-catalog.ipynb
+-rw-rw-rw-   0        0        0     8929 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/derivapy-datapath-example-1.ipynb
+-rw-rw-rw-   0        0        0    19838 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/derivapy-datapath-example-2.ipynb
+-rw-rw-rw-   0        0        0    17351 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/derivapy-datapath-example-3.ipynb
+-rw-rw-rw-   0        0        0   104075 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/derivapy-datapath-example-4.ipynb
+-rw-rw-rw-   0        0        0    11326 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/derivapy-datapath-update.ipynb
+-rw-rw-rw-   0        0        0     2491 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/get-started.ipynb
+-rw-rw-rw-   0        0        0      490 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/index.rst
+-rw-rw-rw-   0        0        0      776 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/install.md
+-rwxrwxrwx   0        0        0      777 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/make.bat
+-rw-rw-rw-   0        0        0    27593 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/project-tutorial.md
+-rw-rw-rw-   0        0        0     3671 2024-02-21 06:15:46.000000 deriva-1.7.1/docs/using-r.md
+-rw-rw-rw-   0        0        0      124 2024-02-21 06:15:46.000000 deriva-1.7.1/requirements_dev.txt
+-rw-rw-rw-   0        0        0      110 2024-05-14 20:16:44.097725 deriva-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     3286 2024-05-14 19:14:56.000000 deriva-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:44.082073 deriva-1.7.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:44.082073 deriva-1.7.1/tests/deriva/
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.1/tests/deriva/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:16:44.082073 deriva-1.7.1/tests/deriva/core/
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:46.000000 deriva-1.7.1/tests/deriva/core/__init__.py
+-rw-rw-rw-   0        0        0    37308 2024-04-16 01:40:25.000000 deriva-1.7.1/tests/deriva/core/test_datapath.py
```

### Comparing `deriva-1.7.0/.gitignore` & `deriva-1.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/LICENSE` & `deriva-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/PKG-INFO` & `deriva-1.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deriva
-Version: 1.7.0
+Version: 1.7.1
 Summary: Python APIs and CLIs (Command-Line Interfaces) for the DERIVA platform.
 Home-page: https://github.com/informatics-isi-edu/deriva-py
 Author: USC Information Sciences Institute, Informatics Systems Research Division
 Author-email: isrd-support@isi.edu
 Maintainer: USC Information Sciences Institute, Informatics Systems Research Division
 Maintainer-email: isrd-support@isi.edu
 License: Apache 2.0
@@ -25,14 +25,14 @@
 License-File: LICENSE
 Requires-Dist: packaging
 Requires-Dist: requests
 Requires-Dist: certifi
 Requires-Dist: pika
 Requires-Dist: urllib3<3,>=1.26
 Requires-Dist: portalocker>=1.2.1
-Requires-Dist: bdbag>=1.7.2
+Requires-Dist: bdbag>=1.7.3
 Requires-Dist: globus_sdk<4,>=3
 Requires-Dist: fair-research-login>=0.3.1
 Requires-Dist: fair-identifiers-client>=0.5.1
 Requires-Dist: jsonschema>=3.1
 
 For further information, visit the project [homepage](https://github.com/informatics-isi-edu/deriva-py).
```

### Comparing `deriva-1.7.0/README.md` & `deriva-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/config/acl_config.py` & `deriva-1.7.1/deriva/config/acl_config.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/config/annotation_config.py` & `deriva-1.7.1/deriva/config/annotation_config.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/config/annotation_validate.py` & `deriva-1.7.1/deriva/config/annotation_validate.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/config/base_config.py` & `deriva-1.7.1/deriva/config/base_config.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/config/dump_catalog_annotations.py` & `deriva-1.7.1/deriva/config/dump_catalog_annotations.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/config/examples/group_owner_policy.json` & `deriva-1.7.1/deriva/config/examples/group_owner_policy.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/config/examples/self_serve_policy.json` & `deriva-1.7.1/deriva/config/examples/self_serve_policy.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/config/rollback_annotation.py` & `deriva-1.7.1/deriva/config/rollback_annotation.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/__init__.py` & `deriva-1.7.1/deriva/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.7.0"
+__version__ = "1.7.1"
 
 from deriva.core.utils.core_utils import *
 from deriva.core.base_cli import BaseCLI, KeyValuePairArgs
 from deriva.core.deriva_binding import DerivaBinding, DerivaPathError, DerivaClientContext
 from deriva.core.deriva_server import DerivaServer
 from deriva.core.ermrest_catalog import ErmrestCatalog, ErmrestSnapshot, ErmrestCatalogMutationError, ErmrestAlias
 from deriva.core.polling_ermrest_catalog import PollingErmrestCatalog
```

### Comparing `deriva-1.7.0/deriva/core/annotation.py` & `deriva-1.7.1/deriva/core/annotation.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/base_cli.py` & `deriva-1.7.1/deriva/core/base_cli.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/catalog_cli.py` & `deriva-1.7.1/deriva/core/catalog_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,98 +51,103 @@
         self.args = None
         self.host = None
         self.protocol = None
         self.catalog = None
 
         # parent arg parser
         self.remove_options(['--config-file', '--credential-file'])
-        self.parser.add_argument("--protocol", choices=["http", "https"], default='https',
+        self.parser.add_argument("-p", "--protocol", choices=["http", "https"], default='https',
                                  help="transport protocol: 'http' or 'https'")
         subparsers = self.parser.add_subparsers(title='sub-commands', dest='subcmd')
 
         # exists parser
         exists_parser = subparsers.add_parser('exists', help="Check if catalog exists.")
-        exists_parser.add_argument("id", metavar="<id>", type=str, help="catalog id")
+        exists_parser.add_argument("id", metavar="<id>", type=str, help="Catalog ID")
         exists_parser.set_defaults(func=self.catalog_exists)
 
         # create parser
         create_parser = subparsers.add_parser('create', help="Create a new catalog.")
-        create_parser.add_argument("--id", metavar="<id>", type=str, help="catalog id")
-        create_parser.add_argument("--owner", metavar="<owner> <owner> ...",
+        create_parser.add_argument("--id", metavar="<id>", type=str, help="Catalog ID")
+        create_parser.add_argument("-o", "--owner", metavar="<owner> <owner> ...",
                                    nargs="+", help="List of quoted user or group identifier strings.")
-        create_parser.add_argument("--auto-configure", action="store_true",
+        create_parser.add_argument("-a", "--auto-configure", action="store_true",
                                    help="Configure the new catalog with a set of baseline defaults")
         create_parser.add_argument("--configure-args", metavar="[key=value key=value ...]",
                                    nargs='+', action=KeyValuePairArgs, default={},
                                    help="Variable length of whitespace-delimited key=value pair arguments used for "
                                         "controlling automatic catalog configuration settings. "
                                         "For example: --configure-args key1=value1 key2=value2")
         create_parser.set_defaults(func=self.catalog_create)
 
         # get parser
         get_parser = subparsers.add_parser('get', help="Send a HTTP GET request to the catalog.")
-        get_parser.add_argument("id", metavar="<id>", type=str, help="catalog id")
+        get_parser.add_argument("id", metavar="<id>", type=str, help="Catalog ID")
         get_parser.add_argument("path", metavar="<request-path>", help="The ERMRest API path.")
-        get_parser.add_argument("--output-file", metavar="<output file path>", help="Path to output file.")
-        get_parser.add_argument("--output-format", choices=["json", "json-stream", "csv"], default="json")
-        get_parser.add_argument("--auto-delete", action="store_true",
+        get_parser.add_argument("-o", "--output-file", metavar="<output file path>", help="Path to output file.")
+        get_parser.add_argument("-f", "--output-format", choices=["json", "json-stream", "csv"], default="json",
+                                help="The output file format. Defaults to 'json'")
+        get_parser.add_argument("-a", "--auto-delete", action="store_true",
                                 help="Automatically delete output file if no results are returned.")
         get_parser.add_argument("--headers", metavar="[key=value key=value ...]",
                                 nargs='+', action=KeyValuePairArgs, default={},
                                 help="Variable length of whitespace-delimited key=value pair arguments used for "
                                      "specifying or overriding HTTP Request Headers. "
                                      "For example: --headers key1=value1 key2=value2")
         get_parser.set_defaults(func=self.catalog_get)
 
         # put parser
         put_parser = subparsers.add_parser('put', help="Send a HTTP PUT request to the catalog.")
-        put_parser.add_argument("id", metavar="<id>", type=str, help="catalog id")
+        put_parser.add_argument("id", metavar="<id>", type=str, help="Catalog ID")
         put_parser.add_argument("path", metavar="<request-path>", help="The ERMRest API path.")
-        put_parser.add_argument("--input-file", metavar="<output file path>", help="Path to input file.")
-        put_parser.add_argument("--input-format", choices=["json", "json-stream", "csv"], default="json")
+        put_parser.add_argument("input-file", metavar="<input file path>",
+                                help="Path to an input file containing the request message body.")
+        put_parser.add_argument("-f", "--input-format", choices=["json", "json-stream", "csv"], default="json",
+                                help="The input file format. Defaults to 'json'")
         put_parser.add_argument("--headers", metavar="[key=value key=value ...]",
                                 nargs='+', action=KeyValuePairArgs, default={},
                                 help="Variable length of whitespace-delimited key=value pair arguments used for "
                                      "specifying or overriding HTTP Request Headers. "
                                      "For example: --headers key1=value1 key2=value2")
         put_parser.set_defaults(func=self.catalog_put)
 
         # post parser
         post_parser = subparsers.add_parser('post', help="Send a HTTP POST request to the catalog.")
-        post_parser.add_argument("id", metavar="<id>", type=str, help="catalog id")
+        post_parser.add_argument("id", metavar="<id>", type=str, help="Catalog ID")
         post_parser.add_argument("path", metavar="<request-path>", help="The ERMRest API path.")
-        post_parser.add_argument("--input-file", metavar="<input file path>", help="Path to input file.")
-        post_parser.add_argument("--input-format", choices=["json", "json-stream", "csv"], default="json")
+        post_parser.add_argument("input-file", metavar="<input file path>",
+                                 help="Path to an input file containing the request message body.")
+        post_parser.add_argument("-f", "--input-format", choices=["json", "json-stream", "csv"], default="json",
+                                 help="The input file format. Defaults to 'json'")
         post_parser.add_argument("--headers", metavar="[key=value key=value ...]",
                                  nargs='+', action=KeyValuePairArgs, default={},
                                  help="Variable length of whitespace-delimited key=value pair arguments used for "
                                       "specifying or overriding HTTP Request Headers. "
                                       "For example: --headers key1=value1 key2=value2")
         post_parser.set_defaults(func=self.catalog_post)
 
         # delete parser
         del_parser = subparsers.add_parser('delete', help="Send a HTTP DELETE request to the catalog. "
                                                           "Use the 'drop' command to delete the entire catalog.")
-        del_parser.add_argument("id", metavar="<id>", type=str, help="catalog id")
+        del_parser.add_argument("id", metavar="<id>", type=str, help="Catalog ID")
         del_parser.add_argument("path", metavar="<request-path>", help="The ERMRest API path.")
         del_parser.add_argument("--headers", metavar="[key=value key=value ...]",
                                 nargs='+', action=KeyValuePairArgs, default={},
                                 help="Variable length of whitespace-delimited key=value pair arguments used for "
                                      "specifying or overriding HTTP Request Headers. "
                                      "For example: --headers key1=value1 key2=value2")
         del_parser.set_defaults(func=self.catalog_delete)
 
         # drop parser
         drop_parser = subparsers.add_parser('drop', help="Delete a catalog.")
-        drop_parser.add_argument("id", metavar="<id>", type=str, help="catalog id")
+        drop_parser.add_argument("id", metavar="<id>", type=str, help="Catalog ID")
         drop_parser.set_defaults(func=self.catalog_drop)
 
         # clone parser
         clone_parser = subparsers.add_parser('clone', help="Clone a source catalog to a new destination catalog.")
-        clone_parser.add_argument("id", metavar="<id>", type=str, help="catalog id")
+        clone_parser.add_argument("id", metavar="<id>", type=str, help="Catalog ID")
         clone_parser.add_argument("--no-copy-data", action="store_false",
                                   help="Do not copy table contents.")
         clone_parser.add_argument("--no-copy-annotations", action="store_false",
                                   help="Do not copy annotations.")
         clone_parser.add_argument("--no-copy-policy", action="store_false",
                                   help="Do not copy ACL (Access Control List) policies.")
         clone_parser.add_argument("--no-truncate-after", action="store_false",
@@ -150,31 +155,31 @@
         clone_parser.add_argument("--exclude-schemas", metavar="<schema-name> <schema-name> ...",
                                   nargs="+", help="List of schema names to exclude from the cloning process.")
         clone_parser.set_defaults(func=self.catalog_clone)
 
         # create_alias parser
         create_alias_parser = subparsers.add_parser('create-alias', help="Create a new catalog alias")
         create_alias_parser.add_argument("--id", metavar="<id>", type=str, help="The alias id.")
-        create_alias_parser.add_argument("--alias-target", metavar="<alias>", help="The target catalog id.")
-        create_alias_parser.add_argument("--owner", metavar="<owner> <owner> ...",
+        create_alias_parser.add_argument("-t", "--alias-target", metavar="<alias>", help="The target catalog id.")
+        create_alias_parser.add_argument("-o", "--owner", metavar="<owner> <owner> ...",
                                          nargs="+", help="List of quoted user or group identifier strings.")
         create_alias_parser.set_defaults(func=self.catalog_alias_create)
 
         # get_alias parser
         get_alias_parser = subparsers.add_parser('get-alias', help="Get catalog alias metadata")
         get_alias_parser.add_argument("id", metavar="<id>", type=str, help="The alias id.")
         get_alias_parser.set_defaults(func=self.catalog_alias_get)
 
         # update_alias parser
         update_alias_parser = subparsers.add_parser('update-alias', help="Update an existing catalog alias")
         update_alias_parser.add_argument("--id", metavar="<id>", type=str, help="The alias id.")
-        update_alias_parser.add_argument("--alias-target", metavar="<alias>", nargs='?', default=nochange, const=None,
+        update_alias_parser.add_argument("-t", "--alias-target", metavar="<alias>", nargs='?', default=nochange, const=None,
                                          help="The target catalog id. If specified without a catalog id as an argument "
                                               "value, the existing alias target will be cleared ")
-        update_alias_parser.add_argument("--owner", metavar="<owner> <owner> ...", nargs='+', default=nochange,
+        update_alias_parser.add_argument("-o", "--owner", metavar="<owner> <owner> ...", nargs='+', default=nochange,
                                          help="List of quoted user or group identifier strings.")
         update_alias_parser.set_defaults(func=self.catalog_alias_update)
 
         # delete_alias parser
         del_alias_parser = subparsers.add_parser('delete-alias', help="Delete a catalog alias.")
         del_alias_parser.add_argument("id", metavar="<id>", type=str, help="The alias id.")
         del_alias_parser.set_defaults(func=self.catalog_alias_delete)
@@ -190,17 +195,37 @@
         """Shared initialization for all sub-commands.
         """
         self.host = args.host if args.host else 'localhost'
         self.protocol = args.protocol
         self.id = args.id
         self.server = DerivaServer(self.protocol,
                                    args.host,
-                                   credentials=DerivaCatalogCLI._get_credential(self.host,
-                                                                                token=args.token,
-                                                                                oauth2_token=args.oauth2_token))
+                                   credentials=DerivaCatalogCLI._get_credential(
+                                       self.host,
+                                       token=args.token,
+                                       oauth2_token=args.oauth2_token))
+
+    @staticmethod
+    def _decorate_headers(headers, file_format, method="get"):
+
+        header_format_map = {
+            "json": "application/json",
+            "json-stream": "application/x-json-stream",
+            "csv": "text/csv"
+        }
+
+        format_type = header_format_map.get(file_format)
+        if format_type is None:
+            raise UsageException("Unsupported format: %s" % file_format)
+        if str(method).lower() in ["get", "head"]:
+            headers["accept"] = format_type
+        elif str(method).lower() in ["post", "put"]:
+            headers["content-type"] = format_type
+        else:
+            raise UsageException("Unsupported method: %s" % method)
 
     def catalog_exists(self, args):
         """Implements the catalog_exists sub-command.
         """
         catalog = self.server.connect_ermrest(self.id)
         pp(catalog.exists())
 
@@ -246,24 +271,15 @@
                 raise e
 
     def catalog_get(self, args):
         """Implements the catalog_get sub-command.
         """
         headers = DEFAULT_HEADERS.copy()
         headers.update(args.headers)
-
-        if args.output_format == "json":
-            headers["accept"] = "application/json"
-        elif args.output_format == "json-stream":
-            headers["accept"] = "application/x-json-stream"
-        elif args.output_format == "csv":
-            headers["accept"] = "text/csv"
-        else:
-            raise UsageException("Unsupported output format: %s" % args.output_format)
-
+        self._decorate_headers(headers, args.output_format)
         catalog = self.server.connect_ermrest(args.id)
         try:
             if args.output_file:
                 catalog.getAsFile(args.path,
                                   destfilename=args.output_file,
                                   headers=headers,
                                   delete_if_empty=args.auto_delete)
@@ -274,21 +290,49 @@
                 raise ResourceException('Catalog not found', e)
         except:
             if args.output_file and os.path.isfile(args.output_file):
                 logging.info("Deleting empty file: %s" % args.output_file)
                 os.remove(args.output_file)
             raise
 
-    # TODO: implement PUT at some point
     def catalog_put(self, args):
-        raise NotImplementedError
+        """Implements the catalog_put sub-command.
+        """
+        headers = DEFAULT_HEADERS.copy()
+        headers.update(args.headers)
+        self._decorate_headers(headers, args.input_format, "put")
+        try:
+            catalog = self.server.connect_ermrest(args.id)
+            with open(args.input_file, "rb") as input_file:
+                resp = catalog.put(args.path, data=input_file, headers=headers)
+                if not args.quiet:
+                    pp(resp.json())
+        except HTTPError as e:
+            if e.response.status_code == requests.codes.not_found:
+                raise ResourceException('Catalog not found', e)
+            else:
+                raise e
 
-    # TODO: implement POST at some point
     def catalog_post(self, args):
-        raise NotImplementedError
+        """Implements the catalog_post sub-command.
+        """
+        headers = DEFAULT_HEADERS.copy()
+        headers.update(args.headers)
+        self._decorate_headers(headers, args.input_format, "post")
+        try:
+            catalog = self.server.connect_ermrest(args.id)
+            with open(args.input_file, "rb") as input_file:
+                resp = catalog.post(args.path, data=input_file, headers=headers)
+                if not args.quiet:
+                    pp(resp.json())
+        except HTTPError as e:
+            if e.response.status_code == requests.codes.not_found:
+                raise ResourceException('Catalog not found', e)
+            else:
+                raise e
 
     def catalog_delete(self, args):
         """Implements the catalog_delete sub-command.
         """
         headers = DEFAULT_HEADERS.copy()
         headers.update(args.headers)
         try:
```

### Comparing `deriva-1.7.0/deriva/core/datapath.py` & `deriva-1.7.1/deriva/core/datapath.py`

 * *Files 24% similar despite different names*

```diff
@@ -391,15 +391,16 @@
         # let fk be a foreign key object from table A to table B (or from table B to table A)
         path = A.link(B, on=fk)
         ```
 
         By default links use inner join semantics on the foreign key / key equality comparison. The `join_type`
         parameter can be used to specify `left`, `right`, or `full` outer join semantics.
 
-        :param right: the right hand table of the link expression
+        :param right: the right hand table of the link expression; if the table or alias name is in use, an incremental
+        number will be used to disambiguate tables instances of the same original name.
         :param on: an equality comparison between key and foreign key columns, a conjunction of such comparisons, or a foreign key object
         :param join_type: the join type of this link which may be 'left', 'right', 'full' outer joins or '' for inner
         join link by default.
         :return: self
         """
         if not isinstance(right, _TableWrapper):
             raise TypeError("'right' must be a '_TableWrapper' instance")
@@ -409,15 +410,15 @@
             isinstance(on, _erm.ForeignKey)
         ):
             raise TypeError("'on' must be a comparison, conjuction of comparisons, or foreign key object")
         if join_type and on is None:
             raise ValueError("'on' must be specified for outer joins")
         if right._schema._catalog != self._root._schema._catalog:
             raise ValueError("'right' is from a different catalog. Cannot link across catalogs.")
-        if isinstance(right, _TableAlias) and right._name in self._table_instances:
+        if isinstance(right, _TableAlias) and right._parent == self:
             raise ValueError("'right' is a table alias that has already been used.")
         else:
             # Generate an unused alias name for the table
             table_name = right._name
             alias_name = table_name
             counter = 1
             while alias_name in self._table_instances:
@@ -602,14 +603,26 @@
                 self._bind_table_instance(copy.deepcopy(path._table_instances[alias]))
 
         # set the context
         self._context = self._table_instances[path._context._name]
 
         return self
 
+    def denormalize(self, context_name=None, heuristic=None, groupkey_name='RID'):
+        """Denormalizes a path based on a visible-columns annotation 'context' or a heuristic approach.
+
+        This method does not mutate this object. It returns a result set representing the denormalization of the path.
+
+        :param context_name: name of the visible-columns context or if none given, will attempt apply heuristics
+        :param heuristic: heuristic to apply if no context name specified
+        :param groupkey_name: column name for the group by key of the generated query expression (default: 'RID')
+        :return: a results set.
+        """
+        return _datapath_denormalize(self, context_name=context_name, heuristic=heuristic, groupkey_name=groupkey_name)
+
 
 class _ResultSet (object):
     """A set of results for various queries or data manipulations.
 
     The result set is produced by a path. The results may be explicitly fetched. The result set behaves like a
     container. If the result set has not been fetched explicitly, on first use of container operations, it will
     be implicitly fetched from the catalog.
@@ -619,14 +632,15 @@
         :param uri: the uri for the entity set in the catalog.
         :param fetcher_fn: a function that fetches the entities from the catalog.
         """
         assert fetcher_fn is not None
         self._fetcher_fn = fetcher_fn
         self._results_doc = None
         self._sort_keys = None
+        self._limit = None
         self.uri = uri
 
     @property
     def _results(self):
         if self._results_doc is None:
             self.fetch()
         return self._results_doc
@@ -652,22 +666,35 @@
         if not all(isinstance(a, _ColumnWrapper) or isinstance(a, _ColumnAlias) or isinstance(a, _AggregateFunctionAlias)
                    or isinstance(a, _SortDescending) for a in attributes):
             raise TypeError("Sort keys must be column, column alias, or aggregate function alias")
         self._sort_keys = attributes
         self._results_doc = None
         return self
 
+    def limit(self, n):
+        """Set a limit on the number of results to be returned.
+
+        :param n: integer or None.
+        :return: self
+        """
+        try:
+            self._limit = None if n is None else int(n)
+            self._results_doc = None
+            return self
+        except ValueError:
+            raise ValueError('limit argument "n" must be an integer or None')
+
     def fetch(self, limit=None, headers=DEFAULT_HEADERS):
         """Fetches the results from the catalog.
 
         :param limit: maximum number of results to fetch from the catalog.
         :param headers: headers to send in request to server
         :return: self
         """
-        limit = int(limit) if limit else None
+        limit = int(limit) if limit else self._limit
         self._results_doc = self._fetcher_fn(limit, self._sort_keys, headers)
         logger.debug("Fetched %d entities" % len(self._results_doc))
         return self
 
 
 class _TableWrapper (object):
     """Wraps a Table for datapath expressions.
@@ -793,14 +820,26 @@
     def groupby(self, *keys):
         """Returns an attribute group object.
 
         See the docs for this method in `DataPath` for more information.
         """
         return _AttributeGroup(self, self._query, keys)
 
+    def denormalize(self, context_name=None, heuristic=None, groupkey_name='RID'):
+        """Denormalizes a path based on a visible-columns annotation 'context' or a heuristic approach.
+
+        This method does not mutate this object. It returns a result set representing the denormalization of the path.
+
+        :param context_name: name of the visible-columns context or if none given, will attempt apply heuristics
+        :param heuristic: heuristic to apply if no context name specified
+        :param groupkey_name: column name for the group by key of the generated query expression (default: 'RID')
+        :return: a results set.
+        """
+        return self.path.denormalize(context_name=context_name, heuristic=heuristic, groupkey_name=groupkey_name)
+
     def insert(self, entities, defaults=set(), nondefaults=set(), add_system_defaults=True, on_conflict_skip=False):
         """Inserts entities into the table.
 
         :param entities: an iterable collection of entities (i.e., rows) to be inserted into the table.
         :param defaults: optional, set of column names to be assigned the default expression value.
         :param nondefaults: optional, set of columns names to override implicit system defaults
         :param add_system_defaults: flag to add system columns to the set of default columns.
@@ -1756,7 +1795,279 @@
                     aggrs.append(Max(bin._arg).alias('maxval'))
                 if aggrs:
                     result = self._source.aggregates(*aggrs)[0]
                     bin.minval = result.get('minval', bin.minval)
                     bin.maxval = result.get('maxval', bin.maxval)
                     if (bin.minval is None) or (bin.maxval is None):
                         raise ValueError('Automatic determination of binning bounds failed.')
+
+##
+## UTILITIES FOR DENORMALIZATION ##############################################
+##
+
+def _datapath_left_outer_join_by_fkey(path, fk, alias_name=None):
+    """Link a table to the path based on a foreign key reference.
+
+    :param path: a DataPath object
+    :param fk: an ermrest_model.ForeignKey object
+    :param alias_name: an optional 'alias' name to use for the foreign table
+    """
+    assert isinstance(path, DataPath)
+    assert isinstance(fk, _erm.ForeignKey)
+    catalog = path._root._schema._catalog
+
+    # determine 'direction' -- inbound or outbound
+    path_context_table = path.context._base_table._wrapped_table
+    if (path_context_table.schema.name, path_context_table.name) == (fk.table.schema.name, fk.table.name):
+        right = catalog.schemas[fk.pk_table.schema.name].tables[fk.pk_table.name]
+        fkcols = zip(fk.foreign_key_columns, fk.referenced_columns)
+    elif (path_context_table.schema.name, path_context_table.name) == (fk.pk_table.schema.name, fk.pk_table.name):
+        right = catalog.schemas[fk.table.schema.name].tables[fk.table.name]
+        fkcols = zip(fk.referenced_columns, fk.foreign_key_columns)
+    else:
+        raise ValueError('Context table "%s" not referenced by foreign key "%s"' % (path_context_table.name, fk.constraint_name))
+
+    # compose join condition
+    on = None
+    for lcol, rcol in fkcols:
+        lcol = catalog.schemas[lcol.table.schema.name].tables[lcol.table.name].columns[lcol.name]
+        rcol = catalog.schemas[rcol.table.schema.name].tables[rcol.table.name].columns[rcol.name]
+        if on:
+            on = on & (lcol == rcol)
+        else:
+            on = lcol == rcol
+
+    # link
+    path.link(right.alias(alias_name) if alias_name else right, on=on, join_type='left')
+
+
+def _datapath_deserialize_vizcolumn(path, vizcol, sources=None):
+    """Deserializes a visual column specification.
+
+    If the visible column specifies a foreign key path, the datapath object
+    will be changed by linking the foreign keys in the path.
+
+    :param path: a datapath object
+    :param vizcol: a visible column specification
+    :return: the element to be projected from the datapath or None
+    """
+    assert isinstance(path, DataPath)
+    sources = sources if sources else {}
+    context = path.context
+    table = context._wrapped_table
+    model = table.schema.model
+
+    if isinstance(vizcol, str):
+        # column name specification
+        return context.columns[vizcol]
+    elif isinstance(vizcol, list):
+        # constraint specification
+        try:
+            fk = model.fkey(vizcol)
+            _datapath_left_outer_join_by_fkey(path, fk, alias_name='F')
+            return ArrayD(path.context).alias(path.context._name)  # project all attributes
+        except KeyError as e:
+            raise ValueError('Invalid foreign key constraint name: %s. If this is a key constraint name, note that keys are not supported at this time.' % str(e))
+    elif isinstance(vizcol, dict):
+        # resolve visible column
+        while 'sourcekey' in vizcol:
+            temp = sources.get(vizcol['sourcekey'], {})
+            if temp == vizcol:
+                raise ValueError('Visible column self reference for sourcekey "%s"' % vizcol['sourcekey'])
+            vizcol = temp
+        # deserialize source definition
+        source = vizcol.get('source')
+        if not source:
+            # case: none
+            raise ValueError('Could not resolve source definition for visible column')
+        elif isinstance(source, str):
+            # case: column name
+            return context.columns[source]
+        elif isinstance(source, list):
+            # case: path expression
+            # ...validate syntax
+            if not all(isinstance(obj, dict) for obj in source[:-1]):
+                raise ValueError('Source path element must be a foreign key dict')
+            if not isinstance(source[-1], str):
+                raise ValueError('Source path must terminate in a column name string')
+            # link path elements by fkey; and track whether path is outbound only fkeys
+            outbound_only = True
+            for path_elem in source[:-1]:
+                try:
+                    fk = model.fkey(path_elem.get('inbound', path_elem.get('outbound')))
+                    _datapath_left_outer_join_by_fkey(path, fk, alias_name='F')
+                    outbound_only = outbound_only and 'outbound' in path_elem
+                except KeyError as e:
+                    raise ValueError('Invalid foreign key constraint name: %s' % str(e))
+            # return terminating column or entity
+            # ...get terminal name
+            terminal = source[-1]
+            # ...get alias name
+            alias = vizcol.get('markdown_name', vizcol.get('name', path.context._name + '_' + terminal))
+            # ...get aggregate function
+            aggregate = {
+                'min': Min,
+                'max': Max,
+                'cnt': Cnt,
+                'cnd_d': CntD,
+                'array': Array,
+                'array_d': ArrayD
+            }.get(vizcol.get('aggregate'), ArrayD)
+            # ...determine projection mode
+            if vizcol.get('entity', True):
+                # case: whole entities
+                return aggregate(path.context).alias(alias)
+            else:
+                # case: specified attribute value(s)
+                if outbound_only:
+                    # for outbound only paths, we can project a single value
+                    return path.context.columns[terminal].alias(alias)
+                else:
+                    # otherwise, we need to use aggregate the values
+                    return aggregate(path.context.columns[terminal]).alias(alias)
+        else:
+            raise ValueError('Malformed source: %s' % str(source))
+    else:
+        raise ValueError('Malformed visible column: %s' % str(vizcol))
+
+
+def _datapath_contextualize(path, context_name='*', context_body=None, groupkey_name='RID'):
+    """Contextualizes a data path to a named visible columns context.
+
+    :param path: a datapath object
+    :param context_name: name of the context within the path's terminating table's "visible columns" annotations
+    :param context_body: a list of visible column definitions, if given, the `context_name` will be ignored
+    :param groupkey_name: column name for the group by key of the generated query expression (default: 'RID')
+    :return: a 'contextualized' attribute group query object
+    """
+    assert isinstance(path, DataPath)
+    path = copy.deepcopy(path)
+    context = path.context
+    table = context._wrapped_table
+    sources = table.annotations.get(_erm.tag.source_definitions, {}).get('sources')
+    vizcols = context_body if context_body else table.annotations.get(_erm.tag.visible_columns, {}).get(context_name, [])
+    if not vizcols:
+        raise ValueError('Visible columns context "%s" not found for table %s:%s' % (context_name, table.schema.name, table.name))
+    groupkey = context.columns[groupkey_name]
+    projection = []
+
+    for vizcol in vizcols:
+        try:
+            projection.append(_datapath_deserialize_vizcolumn(path, vizcol, sources=sources))
+            path.context = context
+        except ValueError as e:
+            logger.warning(str(e))
+
+    def not_same_as_group_key(x):
+        assert isinstance(groupkey, _ColumnWrapper)
+        if not isinstance(x, _ColumnWrapper):
+            return True
+        return groupkey._wrapped_column != x._wrapped_column
+
+    projection = filter(not_same_as_group_key, projection)  # project groupkey only once
+    query = path.groupby(groupkey).attributes(*projection)
+    return query
+
+
+def _datapath_generate_simple_denormalization(path, include_whole_entities=False):
+    """Generates a denormalized form of the table expressed in a visible columns specification.
+
+    :param path: a datapath object
+    :param include_whole_entities: if a denormalization cannot find a 'name' like terminal, include the whole entity (i.e., all attributes), else return just the 'RID'
+    :return: a generated visible columns specification based on a denormalization heuristic
+    """
+    assert isinstance(path, DataPath)
+    context = path.context
+    table = context._wrapped_table
+
+    fkeys = list(table.foreign_keys)
+    single_column_fkeys = {
+        fkey.foreign_key_columns[0].name: fkey
+        for fkey in table.foreign_keys if len(fkey.foreign_key_columns) == 1
+    }
+
+    def _fkey_to_vizcol(name, fk, inbound=None):
+        # name columns to look for in related tables
+        name_candidates = [
+            'displayname',
+            'preferredname',
+            'fullname',
+            'name',
+            'title',
+            'label'
+        ]
+
+        # determine terminal column
+        terminal = 'RID'
+        for candidate_col in fk.pk_table.columns:
+            if candidate_col.name.lower().replace(' ', '').replace('_', '') in name_candidates:
+                terminal = candidate_col.name
+                break
+
+        # define source path
+        source = [{'outbound': fk.names[0]}, terminal]
+        if inbound:
+            source = [{'inbound': inbound.names[0]}] + source
+
+        # return vizcol spec
+        return {
+            'markdown_name': name,
+            'source': source,
+            'entity': include_whole_entities and terminal == 'RID'
+        }
+
+    # assemble the visible column:
+    #  1. column or single column fkeys
+    #  2. all other (outbound fkey) related tables
+    #  3. all associated tables
+    vizcols = []
+    for col in table.column_definitions:
+        if col.name in single_column_fkeys:
+            fkey = single_column_fkeys[col.name]
+            vizcols.append(_fkey_to_vizcol(col.name, fkey))
+            del single_column_fkeys[col.name]
+            fkeys.remove(fkey)
+        else:
+            vizcols.append(col.name)
+
+    for outbound_fkey in fkeys:
+        vizcols.append(_fkey_to_vizcol(outbound_fkey.constraint_name, outbound_fkey))
+
+    for inbound_fkey in table.referenced_by:
+        if inbound_fkey.table.is_association():
+            vizcols.append(
+                _fkey_to_vizcol(
+                    inbound_fkey.table.name,
+                    inbound_fkey.table.foreign_keys[0] if inbound_fkey != inbound_fkey.table.foreign_keys[0] else inbound_fkey.table.foreign_keys[1],
+                    inbound=inbound_fkey
+                )
+            )
+
+    return vizcols
+
+def simple_denormalization(path):
+    """A simple heuristic denormalization."""
+    return _datapath_generate_simple_denormalization(path)
+
+def simple_denormalization_with_whole_entities(path):
+    """A simple heuristic denormalization with related and associated entities."""
+    return _datapath_generate_simple_denormalization(path, include_whole_entities=True)
+
+def _datapath_denormalize(path, context_name=None, heuristic=None, groupkey_name='RID'):
+    """Denormalizes a path based on annotations or heuristics.
+
+    :param path: a DataPath object
+    :param context_name: name of the visible-columns context or if none given, will attempt apply heuristics
+    :param heuristic: heuristic to apply if no context name specified
+    :param groupkey_name: column name for the group by key of the generated query expression (default: 'RID')
+    """
+    assert isinstance(path, DataPath)
+    assert context_name is None or isinstance(context_name, str)
+    assert isinstance(groupkey_name, str)
+    heuristic = heuristic or simple_denormalization
+    assert callable(heuristic)
+    return _datapath_contextualize(
+        path,
+        context_name=context_name,
+        context_body=None if context_name else heuristic(path),
+        groupkey_name=groupkey_name
+    )
```

### Comparing `deriva-1.7.0/deriva/core/deriva_binding.py` & `deriva-1.7.1/deriva/core/deriva_binding.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/ermrest_catalog.py` & `deriva-1.7.1/deriva/core/ermrest_catalog.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/ermrest_model.py` & `deriva-1.7.1/deriva/core/ermrest_model.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/hatrac_cli.py` & `deriva-1.7.1/deriva/core/hatrac_cli.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/hatrac_store.py` & `deriva-1.7.1/deriva/core/hatrac_store.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/polling_ermrest_catalog.py` & `deriva-1.7.1/deriva/core/polling_ermrest_catalog.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/app_links.schema.json` & `deriva-1.7.1/deriva/core/schemas/app_links.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/asset.schema.json` & `deriva-1.7.1/deriva/core/schemas/asset.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/bulk_upload.schema.json` & `deriva-1.7.1/deriva/core/schemas/bulk_upload.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/citation.schema.json` & `deriva-1.7.1/deriva/core/schemas/citation.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/column_display.schema.json` & `deriva-1.7.1/deriva/core/schemas/column_display.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/display.schema.json` & `deriva-1.7.1/deriva/core/schemas/display.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/export.schema.json` & `deriva-1.7.1/deriva/core/schemas/export.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/export_2019.schema.json` & `deriva-1.7.1/deriva/core/schemas/export_2019.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/foreign_key.schema.json` & `deriva-1.7.1/deriva/core/schemas/foreign_key.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/indexing_preferences.schema.json` & `deriva-1.7.1/deriva/core/schemas/indexing_preferences.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/key_display.schema.json` & `deriva-1.7.1/deriva/core/schemas/key_display.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/source_definitions.schema.json` & `deriva-1.7.1/deriva/core/schemas/source_definitions.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/table_alternatives.schema.json` & `deriva-1.7.1/deriva/core/schemas/table_alternatives.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/table_display.schema.json` & `deriva-1.7.1/deriva/core/schemas/table_display.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/visible_columns.schema.json` & `deriva-1.7.1/deriva/core/schemas/visible_columns.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/schemas/visible_foreign_keys.schema.json` & `deriva-1.7.1/deriva/core/schemas/visible_foreign_keys.schema.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/utils/core_utils.py` & `deriva-1.7.1/deriva/core/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/utils/globus_auth_utils.py` & `deriva-1.7.1/deriva/core/utils/globus_auth_utils.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/utils/hash_utils.py` & `deriva-1.7.1/deriva/core/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/utils/mime_utils.py` & `deriva-1.7.1/deriva/core/utils/mime_utils.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/utils/version_utils.py` & `deriva-1.7.1/deriva/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/core/utils/webauthn_utils.py` & `deriva-1.7.1/deriva/core/utils/webauthn_utils.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/seo/README.md` & `deriva-1.7.1/deriva/seo/README.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/seo/sitemap_builder.py` & `deriva-1.7.1/deriva/seo/sitemap_builder.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/seo/sitemap_cli.py` & `deriva-1.7.1/deriva/seo/sitemap_cli.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/__init__.py` & `deriva-1.7.1/deriva/transfer/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from deriva.transfer.download.deriva_download import DerivaDownload, GenericDownloader, DerivaDownloadError, \
-    DerivaDownloadConfigurationError, DerivaDownloadAuthenticationError, DerivaDownloadAuthorizationError
+    DerivaDownloadConfigurationError, DerivaDownloadAuthenticationError, DerivaDownloadAuthorizationError, \
+    DerivaDownloadBaggingError
 from deriva.transfer.download.deriva_download_cli import DerivaDownloadCLI
 
 from deriva.transfer.upload.deriva_upload import DerivaUpload, GenericUploader, DerivaUploadError, DerivaUploadError, \
-    DerivaUploadConfigurationError, DerivaUploadCatalogCreateError, DerivaUploadCatalogUpdateError
+    DerivaUploadConfigurationError, DerivaUploadCatalogCreateError, DerivaUploadCatalogUpdateError, \
+    DerivaUploadAuthenticationError
 from deriva.transfer.upload.deriva_upload_cli import DerivaUploadCLI
 
 from deriva.transfer.backup.deriva_backup import DerivaBackup, DerivaBackupAuthenticationError, \
     DerivaBackupAuthorizationError, DerivaBackupConfigurationError, DerivaBackupError
 from deriva.transfer.backup.deriva_backup_cli import DerivaBackupCLI
 
 from deriva.transfer.restore.deriva_restore import DerivaRestore, DerivaRestoreAuthenticationError, \
```

### Comparing `deriva-1.7.0/deriva/transfer/backup/deriva_backup.py` & `deriva-1.7.1/deriva/transfer/backup/deriva_backup.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/backup/deriva_backup_cli.py` & `deriva-1.7.1/deriva/transfer/backup/deriva_backup_cli.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/deriva_download.py` & `deriva-1.7.1/deriva/transfer/download/deriva_download.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,27 @@
 import datetime
 import uuid
 import logging
 import platform
 import requests
 from requests.exceptions import HTTPError
 from bdbag import bdbag_api as bdb, bdbag_ro as ro, BAG_PROFILE_TAG, BDBAG_RO_PROFILE_ID
+from bdbag.bdbagit import BagValidationError
 from deriva.core import ErmrestCatalog, HatracStore, format_exception, get_credential, format_credential, read_config, \
     stob, Megabyte, __version__ as VERSION
 from deriva.core.utils.version_utils import get_installed_version
 from deriva.transfer.download.processors import find_query_processor, find_transform_processor, find_post_processor
 from deriva.transfer.download.processors.base_processor import LOCAL_PATH_KEY, REMOTE_PATHS_KEY, SERVICE_URL_KEY, \
     FILE_SIZE_KEY
 from deriva.transfer.download import DerivaDownloadError, DerivaDownloadConfigurationError, \
-    DerivaDownloadAuthenticationError, DerivaDownloadAuthorizationError, DerivaDownloadTimeoutError
+    DerivaDownloadAuthenticationError, DerivaDownloadAuthorizationError, DerivaDownloadTimeoutError, \
+    DerivaDownloadBaggingError
+
+
+logger = logging.getLogger(__name__)
 
 
 class DerivaDownload(object):
     """
 
     """
     def __init__(self, server, **kwargs):
@@ -39,15 +44,15 @@
         self.max_payload_size_mb = int(kwargs.get("max_payload_size_mb", 0) or 0)
         self.timeout_secs = int(kwargs.get("timeout", 0) or 0)
         self.timeout = None
 
         info = "%s v%s [Python %s, %s]" % (
             self.__class__.__name__, get_installed_version(VERSION),
             platform.python_version(), platform.platform(aliased=True))
-        logging.info("Initializing downloader: %s" % info)
+        logger.info("Initializing downloader: %s" % info)
 
         if not self.server:
             raise DerivaDownloadConfigurationError("Server not specified!")
 
         # server variable initialization
         self.hostname = self.server.get('host', '')
         if not self.hostname:
@@ -141,41 +146,43 @@
 
         # 1. If we don't have a client identity, we need to authenticate
         identity = kwargs.get("identity")
         if not identity:
             try:
                 if not self.credentials:
                     self.set_credentials(get_credential(self.hostname))
-                logging.info("Validating credentials for host: %s" % self.hostname)
+                logger.info("Validating credentials for host: %s" % self.hostname)
                 attributes = self.catalog.get_authn_session().json()
                 identity = attributes["client"]
             except HTTPError as he:
                 if he.response.status_code == 404:
-                    logging.info("No existing login session found for host: %s" % self.hostname)
+                    logger.info("No existing login session found for host: %s" % self.hostname)
             except Exception as e:
                 raise DerivaDownloadAuthenticationError("Unable to validate credentials: %s" % format_exception(e))
         wallet = kwargs.get("wallet", {})
 
         # 2. Check for bagging config and initialize bag related variables
         bag_path = None
         bag_archiver = None
         bag_algorithms = None
         bag_idempotent = False
+        bag_strict = True
         bag_config = self.config.get('bag')
         create_bag = True if bag_config else False
         if create_bag:
             bag_name = bag_config.get(
                 'bag_name', ''.join(["deriva_bag", '_', time.strftime("%Y-%m-%d_%H.%M.%S")])).format(**self.envars)
             bag_path = os.path.abspath(os.path.join(self.output_dir, bag_name))
             bag_archiver = bag_config.get('bag_archiver')
             bag_algorithms = bag_config.get('bag_algorithms', ['sha256'])
             bag_idempotent = stob(bag_config.get('bag_idempotent', False))
             bag_metadata = bag_config.get('bag_metadata', {"Internal-Sender-Identifier":
                                                            "deriva@%s" % self.server_url})
-            bag_ro = create_bag and not bag_idempotent and stob(bag_config.get('bag_ro', "True"))
+            bag_ro = create_bag and not bag_idempotent and stob(bag_config.get('bag_ro', True))
+            bag_strict = stob(bag_config.get('bag_strict', True))
             if create_bag:
                 bdb.ensure_bag_path_exists(bag_path)
                 bag = bdb.make_bag(bag_path, algs=bag_algorithms, metadata=bag_metadata, idempotent=bag_idempotent)
                 if bag_ro:
                     ro_author_name = bag.info.get("Contact-Name",
                                                   None if not identity else
                                                   identity.get('full_name',
@@ -207,20 +214,21 @@
                                             ro_author_name=ro_author_name,
                                             ro_author_orcid=ro_author_orcid,
                                             identity=identity,
                                             wallet=wallet,
                                             allow_anonymous=self.allow_anonymous,
                                             timeout=self.timeout)
                 outputs = processor.process()
+                assert outputs is not None
                 if processor.should_abort():
                     raise DerivaDownloadTimeoutError("Timeout (%s seconds) waiting for processor [%s] to complete." %
                                                      (self.timeout_secs, processor_name))
                 self.check_payload_size(outputs)
             except Exception as e:
-                logging.error(format_exception(e))
+                logger.error(format_exception(e))
                 if create_bag:
                     bdb.cleanup_bag(bag_path)
                     if remote_file_manifest and os.path.isfile(remote_file_manifest):
                         os.remove(remote_file_manifest)
                 raise
 
         # 4. Execute anything in the transform processing pipeline, if configured
@@ -266,35 +274,47 @@
                 if not os.path.isfile(remote_file_manifest):
                     remote_file_manifest = None
                 bdb.make_bag(bag_path,
                              algs=bag_algorithms,
                              remote_file_manifest=remote_file_manifest
                              if (remote_file_manifest and os.path.getsize(remote_file_manifest) > 0) else None,
                              update=True,
-                             idempotent=bag_idempotent)
+                             idempotent=bag_idempotent,
+                             strict=bag_strict)
+            except BagValidationError as bve:
+                msg = "Unable to validate bag.%s Error: %s" % (
+                    "" if not bag_strict else
+                    " Strict checking has been enabled, which most likely means that this bag "
+                    "is empty (has no payload files or fetch references) and therefore invalid.",
+                    format_exception(bve))
+                logger.error(msg)
+                bdb.cleanup_bag(bag_path)
+                raise DerivaDownloadBaggingError(msg)
             except Exception as e:
-                logging.fatal("Exception while updating bag manifests: %s" % format_exception(e))
+                msg = "Unhandled exception while updating bag manifests: %s" % format_exception(e)
+                logger.error(msg)
                 bdb.cleanup_bag(bag_path)
-                raise
+                raise DerivaDownloadBaggingError(msg)
             finally:
                 if remote_file_manifest and os.path.isfile(remote_file_manifest):
                     os.remove(remote_file_manifest)
 
-            logging.info('Created bag: %s' % bag_path)
+            logger.info('Created bag: %s' % bag_path)
 
             if bag_archiver is not None:
                 try:
                     archive = bdb.archive_bag(bag_path,
                                               bag_archiver.lower(),
                                               idempotent=bag_idempotent)
                     bdb.cleanup_bag(bag_path)
                     outputs = {os.path.basename(archive): {LOCAL_PATH_KEY: archive}}
                 except Exception as e:
-                    logging.error("Exception while creating data bag archive: %s" % format_exception(e))
-                    raise
+                    msg = "Exception while creating data bag archive: %s" % format_exception(e)
+                    logger.error(msg)
+                    raise DerivaDownloadBaggingError(msg)
             else:
                 outputs = {os.path.basename(bag_path): {LOCAL_PATH_KEY: bag_path}}
 
         # 6. Execute anything in the post processing pipeline, if configured
         post_processors = self.config.get('post_processors', [])
         if post_processors:
             for processor in post_processors:
@@ -314,15 +334,15 @@
                     outputs = processor.process()
                     if processor.should_abort():
                         raise DerivaDownloadTimeoutError(
                             "Timeout (%s seconds) waiting for processor [%s] to complete." %
                             (self.timeout_secs, processor_name))
                     self.check_payload_size(outputs)
                 except Exception as e:
-                    logging.error(format_exception(e))
+                    logger.error(format_exception(e))
                     raise
 
         return outputs
 
     def __del__(self):
         for session in self.sessions.values():
             session.close()
```

### Comparing `deriva-1.7.0/deriva/transfer/download/deriva_download_cli.py` & `deriva-1.7.1/deriva/transfer/download/deriva_download_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import json
 import traceback
 import argparse
 import requests
 from requests.exceptions import HTTPError, ConnectionError
 from deriva.transfer import GenericDownloader
 from deriva.transfer.download import DerivaDownloadError, DerivaDownloadConfigurationError, \
-    DerivaDownloadAuthenticationError, DerivaDownloadAuthorizationError, DerivaDownloadTimeoutError
+    DerivaDownloadAuthenticationError, DerivaDownloadAuthorizationError, DerivaDownloadTimeoutError, \
+    DerivaDownloadBaggingError
 from deriva.core import BaseCLI, KeyValuePairArgs, format_credential, format_exception, urlparse
 
 
 class DerivaDownloadCLI(BaseCLI):
     def __init__(self, description, epilog, **kwargs):
 
         BaseCLI.__init__(self, description, epilog, **kwargs)
@@ -67,15 +68,15 @@
                     raise DerivaDownloadAuthenticationError(
                         "The requested service requires authentication and a valid login session could "
                         "not be found for the specified host. Server responded: %s" % e)
                 elif e.response.status_code == requests.codes.forbidden:
                     raise DerivaDownloadAuthorizationError(
                         "A requested operation was forbidden. Server responded: %s" % e)
         except (DerivaDownloadError, DerivaDownloadConfigurationError, DerivaDownloadAuthenticationError,
-                DerivaDownloadAuthorizationError, DerivaDownloadTimeoutError) as e:
+                DerivaDownloadAuthorizationError, DerivaDownloadTimeoutError, DerivaDownloadBaggingError) as e:
             sys.stderr.write(("\n" if not args.quiet else "") + format_exception(e))
             if args.debug:
                 traceback.print_exc()
             return 1
         except:
             sys.stderr.write("An unexpected error occurred.")
             traceback.print_exc()
```

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/__init__.py` & `deriva-1.7.1/deriva/transfer/download/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/base_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/base_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/postprocess/identifier_post_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/postprocess/identifier_post_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/postprocess/transfer_post_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/postprocess/transfer_post_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/postprocess/url_post_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/postprocess/url_post_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/query/bag_fetch_query_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/query/bag_fetch_query_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/query/base_query_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/query/base_query_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     HEADERS = {'Connection': 'keep-alive'}
 
     def __init__(self, envars=None, **kwargs):
         super(BaseQueryProcessor, self).__init__(envars, **kwargs)
         self.catalog = kwargs["catalog"]
         self.store = kwargs["store"]
         self.base_path = kwargs["base_path"]
-        self.query = self.parameters["query_path"]
-        if self.envars:
+        self.query = self.parameters.get("query_path", "")
+        if self.query and self.envars:
             self.query = self.query.format(**self.envars)
         self.sub_path = self.parameters.get("output_path")
         self.output_filename = self.parameters.get("output_filename")
         self.store_base = kwargs.get("store_base", "/hatrac/")
         self.is_bag = kwargs.get("bag", False)
         self.sessions = kwargs.get("sessions", dict())
         self.content_type = "application/octet-stream"
@@ -55,14 +55,17 @@
                                      bundled_as=ro.make_bundled_as())
             self.outputs.update({self.output_relpath: {LOCAL_PATH_KEY: self.output_abspath,
                                                        FILE_SIZE_KEY: os.path.getsize(self.output_abspath),
                                                        SOURCE_URL_KEY: self.url}})
         return self.outputs
 
     def catalogQuery(self, headers=None, as_file=True):
+        if not self.query:
+            return {}
+
         if not headers:
             headers = self.HEADERS.copy()
         else:
             headers.update(self.HEADERS)
 
         if as_file:
             output_dir = os.path.dirname(self.output_abspath)
@@ -171,16 +174,17 @@
                                                                      sub_path=self.sub_path,
                                                                      filename=self.output_filename,
                                                                      ext=self.ext,
                                                                      is_bag=self.is_bag,
                                                                      envars=self.envars)
 
     def __del__(self):
-        for session in self.sessions.values():
-            session.close()
+        if self.sessions:
+            for session in self.sessions.values():
+                session.close()
 
 
 class CSVQueryProcessor(BaseQueryProcessor):
     def __init__(self, envars=None, **kwargs):
         super(CSVQueryProcessor, self).__init__(envars, **kwargs)
         self.ext = ".csv"
         self.content_type = "text/csv"
@@ -228,7 +232,8 @@
         self.ext = ""
 
     def process(self):
         super(CreateDirProcessor, self).process()
         self.create_default_paths()
         make_dirs(self.output_abspath)
 
+        return self.outputs
```

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/query/file_download_query_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/query/file_download_query_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/transform/base_transform_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/transform/base_transform_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/transform/column_transform_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/transform/column_transform_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/transform/fasta_transform_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/transform/fasta_transform_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/transform/format_transform_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/transform/format_transform_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/transform/geo_transform_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/transform/geo_transform_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/processors/transform/string_transform_processor.py` & `deriva-1.7.1/deriva/transfer/download/processors/transform/string_transform_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test1.json` & `deriva-1.7.1/deriva/transfer/download/tests/test1.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test10.json` & `deriva-1.7.1/deriva/transfer/download/tests/test10.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test11.json` & `deriva-1.7.1/deriva/transfer/download/tests/test11.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test12.json` & `deriva-1.7.1/deriva/transfer/download/tests/test12.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test13.json` & `deriva-1.7.1/deriva/transfer/download/tests/test13.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test14.json` & `deriva-1.7.1/deriva/transfer/download/tests/test14.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test15.json` & `deriva-1.7.1/deriva/transfer/download/tests/test15.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test16.json` & `deriva-1.7.1/deriva/transfer/download/tests/test16.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test19.json` & `deriva-1.7.1/deriva/transfer/download/tests/test19.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test2.json` & `deriva-1.7.1/deriva/transfer/download/tests/test2.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test20.json` & `deriva-1.7.1/deriva/transfer/download/tests/test20.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test3.json` & `deriva-1.7.1/deriva/transfer/download/tests/test3.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test4.json` & `deriva-1.7.1/deriva/transfer/download/tests/test4.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test5.json` & `deriva-1.7.1/deriva/transfer/download/tests/test5.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test6.json` & `deriva-1.7.1/deriva/transfer/download/tests/test6.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test7.json` & `deriva-1.7.1/deriva/transfer/download/tests/test7.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test8.json` & `deriva-1.7.1/deriva/transfer/download/tests/test8.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/download/tests/test9.json` & `deriva-1.7.1/deriva/transfer/download/tests/test9.json`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/restore/deriva_restore.py` & `deriva-1.7.1/deriva/transfer/restore/deriva_restore.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/restore/deriva_restore_cli.py` & `deriva-1.7.1/deriva/transfer/restore/deriva_restore_cli.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/upload/deriva_upload.py` & `deriva-1.7.1/deriva/transfer/upload/deriva_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,14 +553,18 @@
                 groupdict.update(match.groupdict())
 
             return asset_group, asset_type, groupdict
 
         return None, None, None
 
     def uploadFiles(self, status_callback=None, file_callback=None):
+        if not self.identity:
+            raise DerivaUploadAuthenticationError("Unable to determine user identity for %s. "
+                                                  "Please ensure that you are authenticated successfully." %
+                                                  self.server_url)
         completed = 0
         for group, assets in self.file_list.items():
             if self.cancelled:
                 break
             for entry in assets.values():
                 if self.cancelled:
                     self.file_status[entry.path] = FileUploadState(UploadState.Cancelled, "Cancelled by user").asdict()
```

### Comparing `deriva-1.7.0/deriva/transfer/upload/deriva_upload_cli.py` & `deriva-1.7.1/deriva/transfer/upload/deriva_upload_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 import json
 import traceback
 from deriva.transfer import DerivaUpload, DerivaUploadError, DerivaUploadConfigurationError, \
-    DerivaUploadCatalogCreateError, DerivaUploadCatalogUpdateError
+    DerivaUploadCatalogCreateError, DerivaUploadCatalogUpdateError, DerivaUploadAuthenticationError
 from deriva.core import BaseCLI, write_config, format_credential, format_exception, urlparse
 
 
 class DerivaUploadCLI(BaseCLI):
     def __init__(self, uploader, description, epilog):
         if not issubclass(uploader, DerivaUpload):
             raise TypeError("DerivaUpload subclass required")
@@ -91,15 +91,15 @@
                                    args.config_file,
                                    args.credential_file,
                                    args.no_config_update,
                                    args.purge_state,
                                    args.dry_run,
                                    args.output_file)
         except (RuntimeError, FileNotFoundError, DerivaUploadError, DerivaUploadConfigurationError,
-                DerivaUploadCatalogCreateError, DerivaUploadCatalogUpdateError) as e:
+                DerivaUploadCatalogCreateError, DerivaUploadCatalogUpdateError, DerivaUploadAuthenticationError) as e:
             sys.stderr.write(("\n" if not args.quiet else "") + format_exception(e))
             if args.debug:
                 traceback.print_exc()
             return 1
         except:
             traceback.print_exc()
             return 1
```

### Comparing `deriva-1.7.0/deriva/transfer/upload/processors/__init__.py` & `deriva-1.7.1/deriva/transfer/upload/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/upload/processors/archive_processor.py` & `deriva-1.7.1/deriva/transfer/upload/processors/archive_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/upload/processors/base_processor.py` & `deriva-1.7.1/deriva/transfer/upload/processors/base_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/upload/processors/logging_processor.py` & `deriva-1.7.1/deriva/transfer/upload/processors/logging_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/upload/processors/metadata_update_processor.py` & `deriva-1.7.1/deriva/transfer/upload/processors/metadata_update_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva/transfer/upload/processors/rename_processor.py` & `deriva-1.7.1/deriva/transfer/upload/processors/rename_processor.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva.egg-info/PKG-INFO` & `deriva-1.7.1/deriva.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deriva
-Version: 1.7.0
+Version: 1.7.1
 Summary: Python APIs and CLIs (Command-Line Interfaces) for the DERIVA platform.
 Home-page: https://github.com/informatics-isi-edu/deriva-py
 Author: USC Information Sciences Institute, Informatics Systems Research Division
 Author-email: isrd-support@isi.edu
 Maintainer: USC Information Sciences Institute, Informatics Systems Research Division
 Maintainer-email: isrd-support@isi.edu
 License: Apache 2.0
@@ -25,14 +25,14 @@
 License-File: LICENSE
 Requires-Dist: packaging
 Requires-Dist: requests
 Requires-Dist: certifi
 Requires-Dist: pika
 Requires-Dist: urllib3<3,>=1.26
 Requires-Dist: portalocker>=1.2.1
-Requires-Dist: bdbag>=1.7.2
+Requires-Dist: bdbag>=1.7.3
 Requires-Dist: globus_sdk<4,>=3
 Requires-Dist: fair-research-login>=0.3.1
 Requires-Dist: fair-identifiers-client>=0.5.1
 Requires-Dist: jsonschema>=3.1
 
 For further information, visit the project [homepage](https://github.com/informatics-isi-edu/deriva-py).
```

### Comparing `deriva-1.7.0/deriva.egg-info/SOURCES.txt` & `deriva-1.7.1/deriva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/deriva.egg-info/entry_points.txt` & `deriva-1.7.1/deriva.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/BUILD.md` & `deriva-1.7.1/docs/BUILD.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/Makefile` & `deriva-1.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/README.md` & `deriva-1.7.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/api/deriva.config.rst` & `deriva-1.7.1/docs/api/deriva.config.rst`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/api/deriva.core.rst` & `deriva-1.7.1/docs/api/deriva.core.rst`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/api/deriva.core.utils.rst` & `deriva-1.7.1/docs/api/deriva.core.utils.rst`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/api/deriva.transfer.backup.rst` & `deriva-1.7.1/docs/api/deriva.transfer.backup.rst`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/api/deriva.transfer.download.processors.postprocess.rst` & `deriva-1.7.1/docs/api/deriva.transfer.download.processors.postprocess.rst`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/api/deriva.transfer.download.processors.query.rst` & `deriva-1.7.1/docs/api/deriva.transfer.download.processors.query.rst`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/api/deriva.transfer.download.processors.rst` & `deriva-1.7.1/docs/api/deriva.transfer.download.processors.rst`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/api/deriva.transfer.download.rst` & `deriva-1.7.1/docs/api/deriva.transfer.download.rst`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/api/deriva.transfer.restore.rst` & `deriva-1.7.1/docs/api/deriva.transfer.restore.rst`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/api/deriva.transfer.upload.rst` & `deriva-1.7.1/docs/api/deriva.transfer.upload.rst`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/cli/commands.md` & `deriva-1.7.1/docs/cli/commands.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/cli/deriva-acl-config.md` & `deriva-1.7.1/docs/cli/deriva-acl-config.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/cli/deriva-annotation-config.md` & `deriva-1.7.1/docs/cli/deriva-annotation-config.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/cli/deriva-annotation-validate.md` & `deriva-1.7.1/docs/cli/deriva-annotation-validate.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/cli/deriva-backup-cli.md` & `deriva-1.7.1/docs/cli/deriva-backup-cli.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/cli/deriva-download-cli.md` & `deriva-1.7.1/docs/cli/deriva-download-cli.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/cli/deriva-hatrac-cli.md` & `deriva-1.7.1/docs/cli/deriva-hatrac-cli.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/cli/deriva-restore-cli.md` & `deriva-1.7.1/docs/cli/deriva-restore-cli.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/cli/deriva-sitemap-cli.md` & `deriva-1.7.1/docs/cli/deriva-sitemap-cli.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/conf.py` & `deriva-1.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/derivapy-catalog-snapshot.ipynb` & `deriva-1.7.1/docs/derivapy-catalog-snapshot.ipynb`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/derivapy-catalog.ipynb` & `deriva-1.7.1/docs/derivapy-catalog.ipynb`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/derivapy-datapath-example-1.ipynb` & `deriva-1.7.1/docs/derivapy-datapath-example-1.ipynb`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/derivapy-datapath-example-2.ipynb` & `deriva-1.7.1/docs/derivapy-datapath-example-2.ipynb`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/derivapy-datapath-example-3.ipynb` & `deriva-1.7.1/docs/derivapy-datapath-example-3.ipynb`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/derivapy-datapath-example-4.ipynb` & `deriva-1.7.1/docs/derivapy-datapath-example-4.ipynb`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/derivapy-datapath-update.ipynb` & `deriva-1.7.1/docs/derivapy-datapath-update.ipynb`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/get-started.ipynb` & `deriva-1.7.1/docs/get-started.ipynb`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/install.md` & `deriva-1.7.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/make.bat` & `deriva-1.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/project-tutorial.md` & `deriva-1.7.1/docs/project-tutorial.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/docs/using-r.md` & `deriva-1.7.1/docs/using-r.md`

 * *Files identical despite different names*

### Comparing `deriva-1.7.0/setup.py` & `deriva-1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     install_requires=[
         'packaging',
         'requests',
         'certifi',
         'pika',
         'urllib3>=1.26,<3',
         'portalocker>=1.2.1',
-        'bdbag>=1.7.2',
+        'bdbag>=1.7.3',
         'globus_sdk>=3,<4',
         'fair-research-login>=0.3.1',
         'fair-identifiers-client>=0.5.1',
         'jsonschema>=3.1'
     ],
     license='Apache 2.0',
     classifiers=[
```

### Comparing `deriva-1.7.0/tests/deriva/core/test_datapath.py` & `deriva-1.7.1/tests/deriva/core/test_datapath.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from copy import deepcopy
 import logging
 from operator import itemgetter
 import os
 import unittest
 import sys
 from deriva.core import DerivaServer, get_credential, ermrest_model as _em, __version__
-from deriva.core.datapath import DataPathException, Min, Max, Sum, Avg, Cnt, CntD, Array, ArrayD, Bin
+from deriva.core.datapath import DataPathException, Min, Max, Sum, Avg, Cnt, CntD, Array, ArrayD, Bin, \
+    simple_denormalization_with_whole_entities
 
 try:
     from pandas import DataFrame
     HAS_PANDAS = True
 except ImportError:
     HAS_PANDAS = False
 
@@ -125,19 +126,20 @@
     ]
 
 
 def populate_test_catalog(catalog):
     """Populate the test catalog."""
     paths = catalog.getPathBuilder()
     logger.debug("Inserting project...")
-    logger.debug("Inserting experiment types...")
     proj_table = paths.schemas[SNAME_ISA].tables[TNAME_PROJECT]
+    logger.debug("Inserting investigators...")
     proj_table.insert([
         {"Investigator": TEST_PROJ_INVESTIGATOR, "Num": TEST_PROJ_NUM}
     ])
+    logger.debug("Inserting experiment types...")
     type_table = paths.schemas[SNAME_VOCAB].tables[TNAME_EXPERIMENT_TYPE]
     types = type_table.insert([
         {"Name": "{}".format(name), "Description": "NA"} for name in range(TEST_EXPTYPE_MAX)
     ], defaults=['ID', 'URI'])
     logger.debug("Inserting experiments...")
     exp = paths.schemas[SNAME_ISA].tables[TNAME_EXPERIMENT]
     exp.insert(_generate_experiment_entities(types, TEST_EXP_MAX))
@@ -802,10 +804,30 @@
         self.assertNotEqual(path, path1, "Compose should have copied the first path rather than mutate it")
         self.assertNotEqual(path.uri, path1.uri, "Composed path URI should not match the first path URI")
         self.assertEqual(path1.uri, original_uri, "First path was changed")
         self.assertNotEqual(path.uri, original_uri, "Merged path's URI should have changed from its original URI")
         self.assertEqual(path.context._name, path3.context._name, "Context of composed paths should equal far right-hand path's context")
         self.assertGreater(len(path.Experiment.entities()), 0, "Should have returned results")
 
+    def test_simple_denormalization(self):
+        entities = self.experiment.entities()
+        results = self.experiment.denormalize()
+        self.assertEqual(len(entities), len(results))
+        self.assertNotEqual(entities[0].keys(), results[0].keys())
+        self.assertIn('Type', results[0])
+        self.assertTrue(entities[0]['Type'].startswith('TEST:'))
+        self.assertTrue(results[0]['Type'])
+        self.assertFalse(results[0]['Type'].startswith('TEST:'))
+
+    def test_simple_denormalization_w_entities(self):
+        entities = self.experiment.entities()
+        results = self.experiment.denormalize(heuristic=simple_denormalization_with_whole_entities)
+        self.assertEqual(len(entities), len(results))
+        self.assertLess(len(entities[0].keys()), len(results[0].keys()))
+        self.assertIn('Experiment_Project Investigator_Project_Num_fkey', results[0])
+        self.assertIsInstance(results[0]['Experiment_Project Investigator_Project_Num_fkey'], list)
+        self.assertIsInstance(results[0]['Experiment_Project Investigator_Project_Num_fkey'][0], dict)
+        self.assertIn('RID', results[0]['Experiment_Project Investigator_Project_Num_fkey'][0])
+
 
 if __name__ == '__main__':
     sys.exit(unittest.main())
```

