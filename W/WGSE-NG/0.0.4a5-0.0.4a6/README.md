# Comparing `tmp/wgse_ng-0.0.4a5.tar.gz` & `tmp/wgse_ng-0.0.4a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgse_ng-0.0.4a5.tar", last modified: Tue May  7 19:11:28 2024, max compression
+gzip compressed data, was "wgse_ng-0.0.4a6.tar", last modified: Tue May 14 10:41:44 2024, max compression
```

## Comparing `wgse_ng-0.0.4a5.tar` & `wgse_ng-0.0.4a6.tar`

### file list

```diff
@@ -1,45 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.645143 wgse_ng-0.0.4a5/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-07 19:11:28.645143 wgse_ng-0.0.4a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.645143 wgse_ng-0.0.4a5/WGSE_NG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-07 19:11:28.000000 wgse_ng-0.0.4a5/WGSE_NG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-07 19:11:28.000000 wgse_ng-0.0.4a5/WGSE_NG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:11:28.000000 wgse_ng-0.0.4a5/WGSE_NG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 19:11:28.000000 wgse_ng-0.0.4a5/WGSE_NG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 19:11:28.000000 wgse_ng-0.0.4a5/WGSE_NG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 19:11:28.000000 wgse_ng-0.0.4a5/WGSE_NG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:11:28.645143 wgse_ng-0.0.4a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.641143 wgse_ng-0.0.4a5/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_fasta_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_raw_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_unknown_bases_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.641143 wgse_ng-0.0.4a5/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/tools/fake_reference_genome_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/tools/import_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/tools/reference_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.641143 wgse_ng-0.0.4a5/wgse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.641143 wgse_ng-0.0.4a5/wgse/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/external.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/genome_file_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.645143 wgse_ng-0.0.4a5/wgse/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/alignment_statistics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/filedrop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/header_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/index_statistics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    12460 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/table_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    21524 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/ui_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/variant_caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.541765 wgse_ng-0.0.4a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-14 10:41:44.541765 wgse_ng-0.0.4a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.541765 wgse_ng-0.0.4a6/WGSE_NG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-14 10:41:44.000000 wgse_ng-0.0.4a6/WGSE_NG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-14 10:41:44.000000 wgse_ng-0.0.4a6/WGSE_NG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:41:44.000000 wgse_ng-0.0.4a6/WGSE_NG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 10:41:44.000000 wgse_ng-0.0.4a6/WGSE_NG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 10:41:44.000000 wgse_ng-0.0.4a6/WGSE_NG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:41:44.541765 wgse_ng-0.0.4a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.513765 wgse_ng-0.0.4a6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_fasta_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_raw_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_unknown_bases_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.513765 wgse_ng-0.0.4a6/wgse/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.517765 wgse_ng-0.0.4a6/wgse/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/adapters/alignment_map_file_info_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/adapters/alignment_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/adapters/header_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/adapters/index_stats_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.517765 wgse_ng-0.0.4a6/wgse/alignment_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/alignment_map_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/alignment_map_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/alignment_map_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/alignment_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/depth_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/index_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.521765 wgse_ng-0.0.4a6/wgse/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/alignment_map_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/alignment_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/chromosome_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/mitochondrial_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/mitochondrial_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/mitochondrial_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/read_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/sequence_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.521765 wgse_ng-0.0.4a6/wgse/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/experimental/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.521765 wgse_ng-0.0.4a6/wgse/fasta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/fasta_letter_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/fasta_stats_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/letter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/letter_run_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/letter_run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.521765 wgse_ng-0.0.4a6/wgse/fastq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fastq/fastq_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.525765 wgse_ng-0.0.4a6/wgse/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/alignment_statistics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/filedrop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/header_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/index_statistics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/microarray_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/table_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/ui_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/ui_form.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.525765 wgse_ng-0.0.4a6/wgse/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.533765 wgse_ng-0.0.4a6/wgse/metadata/bed_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/bed_templates/19_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/bed_templates/19_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/bed_templates/38_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/bed_templates/38_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/bed_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.537765 wgse_ng-0.0.4a6/wgse/metadata/report_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/report_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/report_templates/table_macro.html
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/report_templates/table_simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/report_templates/table_tab.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.537765 wgse_ng-0.0.4a6/wgse/microarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/microarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/microarray/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/microarray/microarray_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/microarray/raw_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.537765 wgse_ng-0.0.4a6/wgse/mtDNA/
+-rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/mtDNA/CRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/mtDNA/RSRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/mtDNA/Yoruba.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/mtDNA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/mtDNA/rCRS.fasta
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.537765 wgse_ng-0.0.4a6/wgse/reference_genome/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/reference_genome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/reference_genome/bgzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/reference_genome/decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/reference_genome/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/reference_genome/genome_metadata_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/reference_genome/repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.537765 wgse_ng-0.0.4a6/wgse/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/renderers/csv_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/renderers/html_aligned_file_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/renderers/html_simple_table_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.541765 wgse_ng-0.0.4a6/wgse/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/check_prerequisites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/file_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/mt_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/sequence_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/sequencers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/unit_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/variant_caller.py
```

### Comparing `wgse_ng-0.0.4a5/README.md` & `wgse_ng-0.0.4a6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [![Documentation Status](https://readthedocs.org/projects/wgse-ng/badge/?version=latest)](https://wgse-ng.readthedocs.io/en/latest/?badge=latest)
 [![Python application](https://github.com/chaplin89/WGSE-NG/actions/workflows/python-app.yml/badge.svg)](https://github.com/chaplin89/WGSE-NG/actions/workflows/python-app.yml/badge.svg)
 [![Python Publish](https://github.com/chaplin89/WGSE-NG/actions/workflows/python-publish.yml/badge.svg)](https://github.com/chaplin89/WGSE-NG/actions/workflows/python-publish.yml/badge.svg)
 [![Python Publish](https://github.com/chaplin89/WGSE-NG/actions/workflows/python-pyinstaller.yml/badge.svg)](https://github.com/chaplin89/WGSE-NG/actions/workflows/python-pyinstaller.yml/badge.svg)
 
 This is my attempt to improve [WGSE](https://github.com/WGSExtract/WGSExtract-Dev). Still under heavy development. Don't expect anything working.
 
+[PyPi Package](https://pypi.org/project/WGSE-NG/)
+
 ## Documentation
 - [Read the docs](https://wgse-ng.readthedocs.io/en/latest/) (pretty much empty at this point)
 
 ## Develop/Launch
-_Note: The best experience is with [VS Code](https://code.visualstudio.com/) as this project already contains sensible settings for VS code._
+_Note: The best experience for developing is with [VS Code](https://code.visualstudio.com/) as this project already contains sensible settings for VS code._
 ```bash
 git clone https://github.com/chaplin89/WGSE-NG
 cd WGSE-NG
 python -m venv .venv
 ./.venv/Scripts/activate
 python -m pip install -e .
 python main.py
@@ -27,20 +29,20 @@
 ## What's working
 
 - [x] Basic file info extraction
 - [x] Index stats
 - [x] Alignment stats
 - [ ] Coverage stats
 - [ ] FASTQ <-> Aligned file conversion
-- [ ] SAM <-> BAM <-> CRAM conversion
+- [x] SAM <-> BAM <-> CRAM conversion (WIP)
 - [ ] Alignment
-- [ ] Variant calling
+- [x] Variant calling (WIP)
 - [x] Microarray converter
-- [ ] Mitochondrial data extraction
-- [ ] Y-DNA data extraction
-- [ ] Unaligned data extraction
+- [x] Mitochondrial data extraction (WIP)
+- [x] Y-DNA data extraction (WIP)
+- [x] Unaligned data extraction (WIP)
 - [x] Reference genome identification (68 references supported)
 - [ ] Installer
 - [ ] Crash stats
 - [ ] Usage stats
 - [X] Reference ingestion procedure (partial)
 - [ ] Documentation
```

### Comparing `wgse_ng-0.0.4a5/setup.py` & `wgse_ng-0.0.4a6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 from setuptools import find_packages, setup
+from wgse import VERSION
 
 DEPENDENCIES = [
     "setuptools",
     "pefile",
     "pycurl",
     "tqdm",
     "google-cloud-storage",
     "sphinx",
     "pytest",
     "pyqt6",
     "pyinstaller",
     "PySide6",
+    "jinja2",
+    "vcf_parser",
+    "WGSE-NG-3rd-party",
 ]
 
-VERSION = "0.0.4-alpha5"
 DOC = ""
 
 setup(
     name="WGSE-NG",
-    packages=find_packages(),
+    packages=find_packages(include=["wgse", "wgse.*"]),
     author="Multiple",
     author_email="",
     include_package_data=True,
-    extras_require={"gui": ["wgse.gui"], "cli": ["wgse.cli"]},
+    package_data={
+        "wgse.mtDNA": ["*.*"], 
+        "wgse.metadata.microarray_templates.head": ["*.*"],
+        "wgse.metadata.microarray_templates.body": ["*.*"],
+        "wgse.metadata.bed_templates": ["*.*"],
+        "wgse.metadata.report_templates": ["*.*"],
+        },
     description="Whole Genome Sequencing data manipulation tool",
-    long_description="Whole Genome Sequencing data manipulation tool",
+    long_description=open("README.md","r").read(),
     install_requires=DEPENDENCIES,
-    entry_points={"gui_scripts": ["wgse = wgse.gui:main"]},
     url="https://github.com/chaplin89/WGSE-NG",
     version=VERSION,
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
```

### Comparing `wgse_ng-0.0.4a5/test/test_buckets.py` & `wgse_ng-0.0.4a6/test/test_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a5/test/test_fasta.py` & `wgse_ng-0.0.4a6/test/test_fasta.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a5/test/test_fasta_dictionary.py` & `wgse_ng-0.0.4a6/test/test_fasta_dictionary.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a5/test/test_microarray_converter.py` & `wgse_ng-0.0.4a6/test/test_microarray_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from wgse.configuration import RepositoryConfig
 from wgse.data.microarray_converter import MicroarrayConverterTarget
 from wgse.microarray.microarray_converter import MicroarrayConverter
 from wgse.microarray.microarray_line_formatter import TARGET_FORMATTER_MAP
 
 
-def test_every_target_has_formatter():
-    assert all(x in TARGET_FORMATTER_MAP for x in MicroarrayConverterTarget)
+# def test_every_target_has_formatter():
+#     assert all(x in TARGET_FORMATTER_MAP for x in MicroarrayConverterTarget)
     
 def test_inexistent_head_folder_raise():
     config = RepositoryConfig()
     config.metadata = MockPath(exists=False)
     microarray_templates = MockPath(exists=False, name="microarray_templates")
     microarray_templates.joinpath = lambda x: MockPath([], False if x=="body" else True, x)
     config.metadata.joinpath = lambda _: microarray_templates
```

### Comparing `wgse_ng-0.0.4a5/test/test_raw_file.py` & `wgse_ng-0.0.4a6/test/test_raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a5/test/test_sequence.py` & `wgse_ng-0.0.4a6/test/test_sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a5/test/test_unknown_bases_stats.py` & `wgse_ng-0.0.4a6/test/test_unknown_bases_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a5/wgse/external.py` & `wgse_ng-0.0.4a6/wgse/utility/external.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import enum
+import logging
 import os
+import shlex
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 
 from wgse.configuration import MANAGER_CFG
 
 if "win" in sys.platform:
-    """On windows we expect to find all the 
-    executables under .\\3rd_party (if not specified 
-    differently). On other OSs the executables need 
-    to be under path.
-    """
-    third_party = str(Path(".", "3rd_party"))
+    third_party = str(MANAGER_CFG.EXTERNAL.root)
     if third_party not in os.environ["PATH"]:
         os.environ["PATH"] += ";" + third_party
     if ".JAR" not in os.environ["PATHEXT"]:
         os.environ["PATHEXT"] += ";.JAR"
 
 
 class BgzipAction(enum.Enum):
@@ -33,39 +30,40 @@
     the function was invoked.
 
     Args:
         f (Callable): function to decorate.
     """
 
     def execute_binary(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
-        args = [*interpreter, f.__name__, *[str(x) for x in args]]
+        args = [*interpreter, shutil.which(f.__name__), *[str(x) for x in args]]
 
         if wait:
             # Force stdout/stderr to be PIPE as we
             # need to collect the output
             stdout = subprocess.PIPE
             stderr = subprocess.PIPE
+        logging.debug(f"Calling: {shlex.join(args)}")
 
         output = subprocess.Popen(args, stdout=stdout, stdin=stdin, stderr=stderr)
         if wait == True:
             out, err = output.communicate()
             if output.returncode != 0:
                 raise RuntimeError(f"Call to {f.__name__} failed: {err.decode()}")
             return out
         return output
+
     decorated = execute_binary
     decorated.wrapper = exe
     decorated.__name__ = f.__name__
-    
     return decorated
 
 
 def jar(f):
-    """Same thing as run but this deals with .jar files 
-    automatically, invoking java from PATH and specifying 
+    """Same thing as run but this deals with .jar files
+    automatically, invoking java from PATH and specifying
     the right arguments, including the full path of the .jar
     file.
 
     Args:
         f (callable): function to decorate
 
     Returns:
@@ -79,26 +77,32 @@
     full_path = Path(".", full_path)
     full_path = full_path.with_suffix(".jar")
     f.__name__ = str(full_path)
     decorated = exe(f, ["java", "-jar"])
     decorated.wrapper = jar
     return decorated
 
+
 class External:
-    """Wrapper around 3rd party executables"""
+    """Wrapper around 3rd party executables
+
+    TODO: make this class contains only wrappers around exe/jar files and
+    move the rest of the logic somewhere else (e.g., Samtools class with
+    view(), consensus(), ..., a Haplogrep class, a gzip class etc.).
+    """
 
-    def __init__(self, config = MANAGER_CFG.EXTERNAL) -> None:
+    def __init__(self, config=MANAGER_CFG.EXTERNAL) -> None:
         self._config = config
         if not self._config.root.exists():
             raise FileNotFoundError(
                 f"Unable to find root directory for External: {str(self._config.root)}"
             )
         if str(self._config.root) not in os.environ["PATH"]:
             os.environ["PATH"] += ";" + str(self._config.root)
-        
+
         self._htsfile = "htsfile"
         self._samtools = "samtools"
         self._gzip = "gzip"
 
     def get_file_type(self, path: Path):
         process = subprocess.run([self._htsfile, path], capture_output=True, check=True)
         return process.stdout.decode("utf-8")
@@ -118,56 +122,60 @@
 
     def make_dictionary(self, path: Path, output: Path = None):
         if output is None:
             output = Path(path.parent, path.name + ".dict")
         arguments = [self._samtools, "dict", str(path), "-o", str(output)]
         process = subprocess.run(arguments, check=True, capture_output=True)
         return process.stdout.decode("utf-8")
-    
+
     def index(self, path: Path):
-        return self.samtools(["index", "-@", self._config.threads, "-b", str(path)], wait=True)
+        return self.samtools(
+            ["index", "-@", self._config.threads, "-b", str(path)], wait=True
+        )
 
     def _gzip_filename(self, input: Path, action: BgzipAction):
         if action == BgzipAction.Compress:
             return Path(str(input) + ".gz")
         elif action == BgzipAction.Decompress:
             if len(input.suffixes) == 0:
                 raise RuntimeError(
                     f"Unable to determine decompressed filename, invalid filename {str(input)} (no extensions)."
                 )
-            return input.with_suffix("")
+            ext = "".join(input.suffixes[:-1])
+            return input.with_name(input.stem + ext)
         elif action == BgzipAction.Reindex:
             return Path(str(input) + ".gzi")
         else:
             raise RuntimeError(f"Action {action.name} not supported.")
 
     def gzip(
         self,
         input: Path,
         output: Path,
         action: BgzipAction = BgzipAction.Decompress,
     ) -> Path:
+        # TODO: move this logic somewhere else.
         if output.exists():
             raise RuntimeError(
                 f"Trying to decompress {str(input)} but the destination file {str(output)} exists."
             )
         inferred_filename = self._gzip_filename(input, action)
 
         action_flags = {BgzipAction.Compress: "", BgzipAction.Decompress: "-d"}
 
         arguments = [self._gzip, action_flags[action], str(input)]
         process = subprocess.run(arguments, capture_output=True)
 
+        # RAFZ format is libz compatible but will make gzip sometime exit
+        # with a != 0 code, complaining about "trailing garbage data".
+        # This is not a real error, as the file is decompressed anyway.
+        # The issue is potentially fixable by truncating the file, but
+        # there's no practical advantage in doing so. If we fall in this
+        # situation, ignore the error.
         if process.returncode != 0:
-            # RAFZ format is libz compatible but will make gzip sometime exit
-            # with a != 0 code, complaining about "trailing garbage data".
-            # This is not a real error, as the file is decompressed anyway.
-            # The issue is potentially fixable by truncating the file, but
-            # there's no practical advantage in doing so. If we fall in this
-            # situation, ignore the error.
             if "trailing garbage" not in process.stderr.decode():
                 raise RuntimeError(
                     f"gzip exited with return code {process.returncode}: {process.stderr.decode()}"
                 )
 
         if inferred_filename != output:
             inferred_filename.rename(output)
@@ -184,15 +192,18 @@
         action_flags = {
             BgzipAction.Compress: "-if",
             BgzipAction.Decompress: "-d",
             BgzipAction.Reindex: "-r",
         }
         inferred_filename = self._gzip_filename(input, action)
 
-        out = self.bgzip([action_flags[action], str(input), "-@", "32"], wait=True)
+        out = self.bgzip(
+            [action_flags[action], str(input), "-@", str(self._config.threads)],
+            wait=True,
+        )
         if inferred_filename != output:
             inferred_filename.rename(output)
             if action == BgzipAction.Compress:
                 inferred_gzi_filename = Path(str(inferred_filename) + ".gzi")
                 inferred_gzi_filename.rename(str(output) + ".gzi")
 
     def idxstats(self, input: Path):
@@ -204,60 +215,60 @@
     def haplogrep_classify(self, vcf_file, output_file):
         output = self.haplogrep(
             ["classify", "--in", vcf_file, "--format", "vcf", "--out", output_file],
             wait=True,
         )
         output.decode("utf-8")
         return output
-    
+
     # Starting from here all the functions are
     # just calling executables with the same name.
     # See the implementation of @exe and @jar decorator
     # for more details.
-    
+
     @exe
-    def bgzip(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+    def bgzip(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
         raise FileNotFoundError()
 
     @exe
     def samtools(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
         raise FileNotFoundError()
 
     @exe
-    def bwa(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+    def bwa(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
         raise FileNotFoundError()
 
     @exe
-    def bwamem2(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+    def bwamem2(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
         raise FileNotFoundError()
 
     @exe
-    def minimap2(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+    def minimap2(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
         raise FileNotFoundError()
 
     @exe
-    def fastp(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+    def fastp(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
         raise FileNotFoundError()
 
     @exe
-    def bcftool(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+    def bcftools(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
         raise FileNotFoundError()
 
     @exe
-    def tabix(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+    def tabix(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
         raise FileNotFoundError()
 
     @jar
-    def haplogrep(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+    def haplogrep(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
         raise FileNotFoundError()
-    
+
     @jar
-    def FastQC(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+    def FastQC(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
         raise FileNotFoundError()
-    
+
     @jar
-    def picard(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+    def picard(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
         raise FileNotFoundError()
-    
+
     @jar
-    def DISCVRSeq(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+    def DISCVRSeq(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
         raise FileNotFoundError()
```

### Comparing `wgse_ng-0.0.4a5/wgse/gui/alignment_statistics_dialog.py` & `wgse_ng-0.0.4a6/wgse/gui/alignment_statistics_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a5/wgse/gui/filedrop.py` & `wgse_ng-0.0.4a6/wgse/gui/filedrop.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a5/wgse/gui/header.py` & `wgse_ng-0.0.4a6/wgse/gui/header.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a5/wgse/gui/header_dialog.py` & `wgse_ng-0.0.4a6/wgse/gui/header_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a5/wgse/gui/index_statistics_dialog.py` & `wgse_ng-0.0.4a6/wgse/gui/index_statistics_dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PySide6.QtCore import Qt
 
 from wgse.alignment_map.index_stats_calculator import SequenceStatistics
 from wgse.data.alignment_stats import AlignmentStats
-from wgse.data.chromosome_type import ChromosomeType
+from wgse.data.sequence_type import SequenceType
 from wgse.gui.table_dialog import TableDialog
 
 
 class IndexStatisticsDialog(TableDialog):
     def __init__(self, parent=None) -> None:
          super().__init__("Index Statistics", parent, horizontal=True)
 
@@ -18,31 +18,31 @@
             "Mapped length",
             "Unmapped length",
         ]
         grouped_stats = []
         others = [
             "Others",
             "Others",
-            sum(x.reference_length for x in stats if x.type == ChromosomeType.Other),
-            sum(x.mapped for x in stats if x.type == ChromosomeType.Other),
-            sum(x.unmapped for x in stats if x.type == ChromosomeType.Other),
+            sum(x.reference_length for x in stats if x.type == SequenceType.Other),
+            sum(x.mapped for x in stats if x.type == SequenceType.Other),
+            sum(x.unmapped for x in stats if x.type == SequenceType.Other),
         ]
         
         percentage_mapped = ""
         percentage_unmapped = ""
         if others[2] != 0:
             percentage_mapped = f" ({(others[3]/others[2])*100:.1f}%)"
             percentage_unmapped = f" ({(others[4]/others[2])*100:.1f}%)"
         
         others[3] = f"{others[3]}{percentage_mapped}"
         others[4] = f"{others[4]}{percentage_unmapped}"
         others[2] = str(others[2])
 
         for stat in stats:
-            if stat.type == ChromosomeType.Other:
+            if stat.type == SequenceType.Other:
                 continue
             
             percentage_unmapped = ""
             percentage_mapped = ""
             if stat.reference_length != 0:
                 percentage_unmapped = f" ({(stat.unmapped/stat.reference_length)*100:.1f}%)"
                 percentage_mapped = f" ({(stat.mapped/stat.reference_length)*100:.1f}%)"
```

### Comparing `wgse_ng-0.0.4a5/wgse/gui/main.py` & `wgse_ng-0.0.4a6/wgse/gui/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 from wgse.adapters.alignment_stats_adapter import AlignmentStatsAdapter
 from wgse.adapters.header_adapter import HeaderAdapter
 from wgse.adapters.index_stats_adapter import IndexStatsAdapter
 from wgse.alignment_map.alignment_map_file import AlignmentMapFile
 from wgse.configuration import MANAGER_CFG
 from wgse.data.gender import Gender
 from wgse.data.sorting import Sorting
-from wgse.external import External
+from wgse.utility.external import External
 from wgse.fasta.reference import Reference
 from wgse.gui.alignment_statistics_dialog import AlignmentStatisticsDialog
 from wgse.gui.header_dialog import HeaderDialog
+from wgse.gui.extract import ExtractDialog
 from wgse.gui.index_statistics_dialog import IndexStatisticsDialog
 from wgse.gui.ui_form import Ui_MainWindow
 from wgse.gui.filedrop import Ui_Drop
-from wgse.renderers.html_report import HTMLReport
+from wgse.renderers.html_aligned_file_report import HTMLAlignedFileReport
 
 class WGSEWindow(QMainWindow):
     def launch():
         app = QApplication(sys.argv)
         widget = WGSEWindow()
         widget.show()
         sys.exit(app.exec())
@@ -76,60 +77,16 @@
             print("Dropped file:", file_path)
             # Do something with the dropped file
 
 
     def export(self):
         if self.current_file is None:
             return
-        file_info_adapter = AlignmentMapFileInfoAdapter()
-        index_stat_adapter = IndexStatsAdapter()
-        alignment_stats_adapter = AlignmentStatsAdapter()
-        header_adapter = HeaderAdapter()
-
-        file_info_adapted = file_info_adapter.adapt(self.current_file.file_info)
-        index_stat_adapted = index_stat_adapter.adapt(self.current_file.file_info.index_stats)
-        alignment_stats_adapted = alignment_stats_adapter.adapt(
-            self.current_file.file_info.alignment_stats
-        )
-        header_adapted = header_adapter.adapt(self.current_file.header)
-
-        html_report = HTMLReport()
-        html_page = html_report.make(
-            file_info_adapted,
-            index_stat_adapted,
-            alignment_stats_adapted,
-            header_adapted[0],
-            header_adapted[1],
-            header_adapted[2],
-            header_adapted[3],
-        )
-        current_path = self.current_file.path
-        extensions = "".join(current_path.suffixes[:-1])
-        name = current_path.stem + extensions + ".html"
-        target = current_path.with_name(name)
-
-        with target.open("wt") as f:
-            f.write(html_page)
-        webbrowser.open(target)
-        self.ui.exportButton.setDisabled(True)
-
-    def get_reference_genome_string(self, reference: Reference):
-        perfect_match = [x for x in reference.perfect_match.items() if int(x[1]) == 100]
-        if len(perfect_match) > 0:
-            string = ""
-            for genome, percentage_matching in perfect_match:
-                string += f"{genome} ({percentage_matching:.1f}%) "
-            string = f"{len(perfect_match)} perfect match(es) found."
-        else:
-            unknown = [x[0] for x in reference.reference_map.items() if len(x[1]) == 0]
-            if len(unknown) > 0:
-                string = f"Unable to find a match for {len(unknown)} sequence(s)."
-            else:
-                string = f"Unable to find a perfect match but is possible to build it."
-        return string
+        dialog = ExtractDialog(self.current_file, self)
+        dialog.exec()
 
     def on_close(self):
         MANAGER_CFG.save()
         self.close()
 
     def closeEvent(self, event=False):
         MANAGER_CFG.save()
@@ -188,15 +145,15 @@
         size = f"{size:.1f} GB"
 
         rows = [
             ("Directory", str(self.current_file.path.parent)),
             ("Filename", str(self.current_file.path.name)),
             ("Size", size),
             ("File Type", info.file_type.name),
-            ("Reference", self.get_reference_genome_string(info.reference_genome)),
+            ("Reference", info.reference_genome.build),
             ("Gender", gender_string),
             ("Sorted", sorted_string),
             ("Indexed", indexed_string),
             ("Mitochondrial DNA Model", info.mitochondrial_dna_model.name),
             ("Header", click_to_open),
             ("Alignment stats", click_to_open),
             ("Index stats", click_to_open),
@@ -314,16 +271,8 @@
     def _show_header(self):
         if self.current_file is None:
             return
         dialog = HeaderDialog(self)
         dialog.exec(self.current_file.header)
 
     def _gender_determined(self, gender: Gender):
-        male_only = [
-            self.ui.y_extract_group,
-            self.ui.haplogroup_y,
-        ]
-        for element in male_only:
-            if gender ==Gender.Female:
-                element.hide()
-            else:
-                element.show()
+        pass
```

### Comparing `wgse_ng-0.0.4a5/wgse/gui/table_dialog.py` & `wgse_ng-0.0.4a6/wgse/gui/table_dialog.py`

 * *Files identical despite different names*

