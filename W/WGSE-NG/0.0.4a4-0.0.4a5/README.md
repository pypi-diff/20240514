# Comparing `tmp/wgse_ng-0.0.4a4.tar.gz` & `tmp/wgse_ng-0.0.4a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgse_ng-0.0.4a4.tar", last modified: Fri May  3 18:24:28 2024, max compression
+gzip compressed data, was "wgse_ng-0.0.4a5.tar", last modified: Tue May  7 19:11:28 2024, max compression
```

## Comparing `wgse_ng-0.0.4a4.tar` & `wgse_ng-0.0.4a5.tar`

### file list

```diff
@@ -1,77 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:28.829718 wgse_ng-0.0.4a4/
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-03 18:24:28.829718 wgse_ng-0.0.4a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:28.829718 wgse_ng-0.0.4a4/WGSE_NG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-03 18:24:28.000000 wgse_ng-0.0.4a4/WGSE_NG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-03 18:24:28.000000 wgse_ng-0.0.4a4/WGSE_NG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:24:28.000000 wgse_ng-0.0.4a4/WGSE_NG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 18:24:28.000000 wgse_ng-0.0.4a4/WGSE_NG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 18:24:28.000000 wgse_ng-0.0.4a4/WGSE_NG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 18:24:28.000000 wgse_ng-0.0.4a4/WGSE_NG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:24:28.829718 wgse_ng-0.0.4a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:28.821718 wgse_ng-0.0.4a4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/test/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/test/test_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/test/test_fasta_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/test/test_microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/test/test_unknown_bases_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:28.821718 wgse_ng-0.0.4a4/wgse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:28.825718 wgse_ng-0.0.4a4/wgse/alignment_map/
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/alignment_map/alignment_map_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/alignment_map/alignment_map_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/alignment_map/alignment_map_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/alignment_map/alignment_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/alignment_map/depth_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/alignment_map/index_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:28.825718 wgse_ng-0.0.4a4/wgse/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/data/alignment_map_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/data/alignment_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/data/chromosome_type.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/data/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/data/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/data/read_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/data/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/data/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/external.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:28.825718 wgse_ng-0.0.4a4/wgse/fasta/
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/fasta/fasta_letter_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/fasta/fasta_stats_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/fasta/letter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/fasta/letter_run_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/fasta/letter_run_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/fasta/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:28.825718 wgse_ng-0.0.4a4/wgse/fastq/
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/fastq/fastq_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/genome_file_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:28.825718 wgse_ng-0.0.4a4/wgse/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/gui/alignment_statistics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/gui/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/gui/header_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/gui/index_statistics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/gui/table_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/gui/ui_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:28.829718 wgse_ng-0.0.4a4/wgse/microarray/
--rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/microarray/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/microarray/microarray_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/microarray/raw_file.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/prerequisites.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:28.829718 wgse_ng-0.0.4a4/wgse/reference_genome/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/reference_genome/bgzip_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/reference_genome/decompressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/reference_genome/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/reference_genome/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/reference_genome/metadata_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/reference_genome/repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:24:28.829718 wgse_ng-0.0.4a4/wgse/utility/
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/utility/file_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/utility/sequence_orderer.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/utility/sequencers.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/utility/unit_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-03 18:24:21.000000 wgse_ng-0.0.4a4/wgse/variant_caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.645143 wgse_ng-0.0.4a5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-07 19:11:28.645143 wgse_ng-0.0.4a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.645143 wgse_ng-0.0.4a5/WGSE_NG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-07 19:11:28.000000 wgse_ng-0.0.4a5/WGSE_NG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-07 19:11:28.000000 wgse_ng-0.0.4a5/WGSE_NG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:11:28.000000 wgse_ng-0.0.4a5/WGSE_NG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 19:11:28.000000 wgse_ng-0.0.4a5/WGSE_NG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 19:11:28.000000 wgse_ng-0.0.4a5/WGSE_NG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 19:11:28.000000 wgse_ng-0.0.4a5/WGSE_NG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:11:28.645143 wgse_ng-0.0.4a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.641143 wgse_ng-0.0.4a5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_fasta_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_raw_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/test_unknown_bases_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/test/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.641143 wgse_ng-0.0.4a5/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/tools/fake_reference_genome_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/tools/import_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/tools/reference_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.641143 wgse_ng-0.0.4a5/wgse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.641143 wgse_ng-0.0.4a5/wgse/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/genome_file_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:11:28.645143 wgse_ng-0.0.4a5/wgse/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/alignment_statistics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/filedrop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/header_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/index_statistics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12460 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/table_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21524 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/gui/ui_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-07 19:11:19.000000 wgse_ng-0.0.4a5/wgse/variant_caller.py
```

### Comparing `wgse_ng-0.0.4a4/PKG-INFO` & `wgse_ng-0.0.4a5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 0.0.4a4
+Version: 0.0.4a5
 Summary: Whole Genome Sequencing data manipulation tool
 Home-page: https://github.com/chaplin89/WGSE-NG
 Author: Multiple
 Author-email: 
 Keywords: bioinformatics
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -20,9 +20,13 @@
 Requires-Dist: tqdm
 Requires-Dist: google-cloud-storage
 Requires-Dist: sphinx
 Requires-Dist: pytest
 Requires-Dist: pyqt6
 Requires-Dist: pyinstaller
 Requires-Dist: PySide6
+Provides-Extra: gui
+Requires-Dist: wgse.gui; extra == "gui"
+Provides-Extra: cli
+Requires-Dist: wgse.cli; extra == "cli"
 
 Whole Genome Sequencing data manipulation tool
```

### Comparing `wgse_ng-0.0.4a4/README.md` & `wgse_ng-0.0.4a5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ## Develop/Launch
 _Note: The best experience is with [VS Code](https://code.visualstudio.com/) as this project already contains sensible settings for VS code._
 ```bash
 git clone https://github.com/chaplin89/WGSE-NG
 cd WGSE-NG
 python -m venv .venv
 ./.venv/Scripts/activate
-python -m pip install -r requirements.txt
 python -m pip install -e .
 python main.py
+sudo apt install libegl1 libgl1 libxkbcommon0 libfontconfig1 -y
 # If this is run from the terminal of an IDE, 
 # at this point you should restart the IDE as
 # there are some executables that are installed
 # by pip that otherwise won't be found by the IDE.
 ```
 
 ## What's working
```

### Comparing `wgse_ng-0.0.4a4/WGSE_NG.egg-info/PKG-INFO` & `wgse_ng-0.0.4a5/WGSE_NG.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 0.0.4a4
+Version: 0.0.4a5
 Summary: Whole Genome Sequencing data manipulation tool
 Home-page: https://github.com/chaplin89/WGSE-NG
 Author: Multiple
 Author-email: 
 Keywords: bioinformatics
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -20,9 +20,13 @@
 Requires-Dist: tqdm
 Requires-Dist: google-cloud-storage
 Requires-Dist: sphinx
 Requires-Dist: pytest
 Requires-Dist: pyqt6
 Requires-Dist: pyinstaller
 Requires-Dist: PySide6
+Provides-Extra: gui
+Requires-Dist: wgse.gui; extra == "gui"
+Provides-Extra: cli
+Requires-Dist: wgse.cli; extra == "cli"
 
 Whole Genome Sequencing data manipulation tool
```

### Comparing `wgse_ng-0.0.4a4/setup.py` & `wgse_ng-0.0.4a5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,36 @@
-from setuptools import setup
+from setuptools import find_packages, setup
 
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
 ]
 
-VERSION = "0.0.4-alpha4"
+VERSION = "0.0.4-alpha5"
 DOC = ""
 
 setup(
     name="WGSE-NG",
-    packages=[
-        "wgse",
-        "wgse.alignment_map",
-        "wgse.data",
-        "wgse.fasta",
-        "wgse.fastq",
-        "wgse.gui",
-        "wgse.microarray",
-        "wgse.reference_genome",
-        "wgse.utility",
-    ],
+    packages=find_packages(),
     author="Multiple",
     author_email="",
+    include_package_data=True,
+    extras_require={"gui": ["wgse.gui"], "cli": ["wgse.cli"]},
     description="Whole Genome Sequencing data manipulation tool",
     long_description="Whole Genome Sequencing data manipulation tool",
     install_requires=DEPENDENCIES,
-    entry_points={"gui_scripts": ["wgse = wgse:gui"]},
+    entry_points={"gui_scripts": ["wgse = wgse.gui:main"]},
     url="https://github.com/chaplin89/WGSE-NG",
     version=VERSION,
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
```

### Comparing `wgse_ng-0.0.4a4/test/test_buckets.py` & `wgse_ng-0.0.4a5/test/test_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a4/test/test_fasta_dictionary.py` & `wgse_ng-0.0.4a5/test/test_fasta_dictionary.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a4/test/test_sequence.py` & `wgse_ng-0.0.4a5/test/test_sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a4/test/test_unknown_bases_stats.py` & `wgse_ng-0.0.4a5/test/test_unknown_bases_stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,14 @@
+from test.utility import MockFile, MockPath
+
 import pytest
 
 from wgse.fasta.fasta_letter_counter import FASTALetterCounter
 
 
-class MockFile:
-    def __init__(self, lines) -> None:
-        self.lines = lines
-
-    def __enter__(self):
-        return self.lines
-
-    def __exit__(self, _1, _2, _3):
-        return
-
-
-class MockPath:
-    def __init__(self, lines) -> None:
-        self.lines = lines
-        self.name = "foo.fa.gz"
-        self.stem = "foo.fa"
-
-    def open(self, *_1):
-        return MockFile(self.lines)
-
-    def exists(self):
-        return True
-
-
 class MockGenome:
     def __init__(self, fasta_lines, dictionary_lines) -> None:
         self.fasta = MockPath(fasta_lines)
         self.dict = MockPath(dictionary_lines)
 
 
 def gzip_open(path, mode):
```

### Comparing `wgse_ng-0.0.4a4/wgse/configuration.py` & `wgse_ng-0.0.4a5/wgse/configuration.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import configparser
 import logging
 import multiprocessing
 from pathlib import Path
 
 import wgse
 
+logging.getLogger().setLevel(logging.DEBUG)
+
 
 class WGSEDefaults:
     """Specify some directory where to find configuration files."""
 
     WGSE_FOLDER = Path(wgse.__file__).parents[1]
-    PROGRAM_CONFIG = Path(WGSE_FOLDER, "configuration", "main.ini")
-    RELEASE_CONFIG = Path(Path.home(), ".wgse", "main.ini")
+    LOCAL_CONFIG = Path(WGSE_FOLDER, "configuration", "main.ini")
+    GLOBAL_CONFIG = Path(Path.home(), ".wgse", "main.ini")
 
 
 class GeneralConfig:
     def __init__(self) -> None:
         self.last_path: Path = Path.home()
+        self.log_level: str = "DEBUG"
 
 
 class ExternalConfig:
     def __init__(self) -> None:
         self.root: Path = Path(WGSEDefaults.WGSE_FOLDER, "3rd_party")
         self.threads: int = multiprocessing.cpu_count()
 
@@ -34,59 +37,80 @@
 
 class AlignmentStatsConfig:
     def __init__(self) -> None:
         self.skip: int = 40000
         self.samples: int = 20000
 
 
-EXTERNAL_CFG: ExternalConfig = None
-REPOSITORY_CFG: RepositoryConfig = None
-GENERAL_CFG: GeneralConfig = None
-ALIGNMENT_STATS_CFG: AlignmentStatsConfig = None
-
-
 class ConfigurationManager:
+    GENERAL: GeneralConfig = GeneralConfig()
+    EXTERNAL: ExternalConfig = ExternalConfig()
+    REPOSITORY: RepositoryConfig = RepositoryConfig()
+    ALIGNMENT_STATS: AlignmentStatsConfig = AlignmentStatsConfig()
+
     def __init__(self) -> None:
-        self._section_map = {
-            "general": ("GENERAL_CFG", GeneralConfig),
-            "external": ("EXTERNAL_CFG", ExternalConfig),
-            "repository": ("REPOSITORY_CFG", RepositoryConfig),
-            "alignment_stats": ("ALIGNMENT_STATS_CFG", AlignmentStatsConfig),
-        }
         self.load()
 
     def load(self) -> None:
         self._parser = configparser.ConfigParser()
-        self._parser.read(WGSEDefaults.PROGRAM_CONFIG)
-        self._parser.read(WGSEDefaults.RELEASE_CONFIG)
+        logging.info(
+            f"Found file {WGSEDefaults.LOCAL_CONFIG}: {WGSEDefaults.LOCAL_CONFIG.exists()}"
+        )
+        logging.info(
+            f"Found file {WGSEDefaults.GLOBAL_CONFIG}: {WGSEDefaults.GLOBAL_CONFIG.exists()}"
+        )
+        self._parser.read(WGSEDefaults.LOCAL_CONFIG)
+        self._parser.read(WGSEDefaults.GLOBAL_CONFIG)
 
-        for section, value in self._section_map.items():
-            (var, class_name) = value
-            globals()[var] = class_name()
+        for var_name, var_value in ConfigurationManager.__dict__.items():
+            if var_name.startswith("__"):
+                continue
+            if getattr(var_value, "__dict__") == None:
+                continue
+            if type(var_value) == type(ConfigurationManager.load):
+                continue
+
+            section = var_name.lower()
             if section not in self._parser:
                 continue
             for key, value in self._parser[section].items():
-                if key not in globals()[var].__dict__:
+                if key not in var_value.__dict__:
                     logging.warning(f"Configuration {section}.{key} not known")
                     continue
                 if value is None:
                     continue
-                var_type = type(globals()[var].__dict__[key])
-                globals()[var].__dict__[key] = var_type(value)
+                var_type = type(var_value.__dict__[key])
+                var_value.__dict__[key] = var_type(value)
+
+    def save(self, save_defaults=False):
+        for var_name, var_value in ConfigurationManager.__dict__.items():
+            if var_name.startswith("__"):
+                continue
+            if getattr(var_value, "__dict__") == None:
+                continue
+            if type(var_value) == type(ConfigurationManager.load):
+                continue
 
-    def save(self):
-        for section, value in self._section_map.items():
-            (var, _) = value
-            for key, value in globals()[var].__dict__.items():
-                if section not in self._parser:
-                    self._parser.add_section(section)
-                self._parser[section][key] = str(value)
-        for config in [WGSEDefaults.RELEASE_CONFIG, WGSEDefaults.PROGRAM_CONFIG]:
+            default_item = type(var_value)()
+            section = var_name.lower()
+            if section not in self._parser:
+                self._parser.add_section(section)
+            for key, value in var_value.__dict__.items():
+                if default_item.__dict__[key] != value or save_defaults:
+                    self._parser[section][key] = str(value)
+            if len(self._parser[section]) == 0 and not save_defaults:
+                self._parser.remove_section(section)
+        ordered_config_paths = [WGSEDefaults.GLOBAL_CONFIG, WGSEDefaults.LOCAL_CONFIG]
+        if not any([x.exists() for x in ordered_config_paths]):
+            with ordered_config_paths[1].open("wt") as f:
+                pass
+        for config in ordered_config_paths:
             if not config.exists():
                 continue
             with config.open("wt") as f:
                 self._parser.write(f)
+            break
 
 
 MANAGER_CFG = None
 if MANAGER_CFG is None:
     MANAGER_CFG = ConfigurationManager()
```

### Comparing `wgse_ng-0.0.4a4/wgse/external.py` & `wgse_ng-0.0.4a5/wgse/external.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import enum
 import os
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 
-from wgse import configuration
+from wgse.configuration import MANAGER_CFG
 
 if "win" in sys.platform:
     """On windows we expect to find all the 
     executables under .\\3rd_party (if not specified 
     differently). On other OSs the executables need 
     to be under path.
     """
@@ -48,16 +48,19 @@
         output = subprocess.Popen(args, stdout=stdout, stdin=stdin, stderr=stderr)
         if wait == True:
             out, err = output.communicate()
             if output.returncode != 0:
                 raise RuntimeError(f"Call to {f.__name__} failed: {err.decode()}")
             return out
         return output
-
-    return execute_binary
+    decorated = execute_binary
+    decorated.wrapper = exe
+    decorated.__name__ = f.__name__
+    
+    return decorated
 
 
 def jar(f):
     """Same thing as run but this deals with .jar files 
     automatically, invoking java from PATH and specifying 
     the right arguments, including the full path of the .jar
     file.
@@ -66,25 +69,28 @@
         f (callable): function to decorate
 
     Returns:
         callable: Decorated function
     """
     full_path = shutil.which(f.__name__)
     if full_path is None:
+        # Should raise NotImplementedError
+        f.wrapper = jar
         return f
     full_path = Path(".", full_path)
     full_path = full_path.with_suffix(".jar")
     f.__name__ = str(full_path)
-    return exe(f, ["java", "-jar"])
-
+    decorated = exe(f, ["java", "-jar"])
+    decorated.wrapper = jar
+    return decorated
 
 class External:
     """Wrapper around 3rd party executables"""
 
-    def __init__(self, config: configuration.ExternalConfig = configuration.EXTERNAL_CFG) -> None:
+    def __init__(self, config = MANAGER_CFG.EXTERNAL) -> None:
         self._config = config
         if not self._config.root.exists():
             raise FileNotFoundError(
                 f"Unable to find root directory for External: {str(self._config.root)}"
             )
         if str(self._config.root) not in os.environ["PATH"]:
             os.environ["PATH"] += ";" + str(self._config.root)
@@ -205,53 +211,53 @@
     
     # Starting from here all the functions are
     # just calling executables with the same name.
     # See the implementation of @exe and @jar decorator
     # for more details.
     
     @exe
-    def bgzip(self, args=[], stdout=None, stdin=None, wait=False):
-        pass
+    def bgzip(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+        raise FileNotFoundError()
 
     @exe
-    def samtools(self, args=[], stdout=None, stdin=None, wait=False):
-        pass
+    def samtools(self, args=[], stdout=None, stdin=None, stderr=None, wait=False):
+        raise FileNotFoundError()
 
     @exe
-    def bwa(self, args=[], stdout=None, stdin=None, wait=False):
-        pass
+    def bwa(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+        raise FileNotFoundError()
 
     @exe
-    def bwamem2(self, args=[], stdout=None, stdin=None, wait=False):
-        pass
+    def bwamem2(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+        raise FileNotFoundError()
 
     @exe
-    def minimap2(self, args=[], stdout=None, stdin=None, wait=False):
-        pass
+    def minimap2(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+        raise FileNotFoundError()
 
     @exe
-    def fastp(self, args=[], stdout=None, stdin=None, wait=False):
-        pass
+    def fastp(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+        raise FileNotFoundError()
 
     @exe
-    def bcftool(self, args=[], stdout=None, stdin=None, wait=False):
-        pass
+    def bcftool(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+        raise FileNotFoundError()
 
     @exe
-    def tabix(self, args=[], stdout=None, stdin=None, wait=False):
-        pass
+    def tabix(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+        raise FileNotFoundError()
 
     @jar
-    def haplogrep(self, args=[], stdout=None, stdin=None, wait=False):
-        pass
+    def haplogrep(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+        raise FileNotFoundError()
     
     @jar
-    def FastQC(self, args=[], stdout=None, stdin=None, wait=False):
-        pass
+    def FastQC(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+        raise FileNotFoundError()
     
     @jar
-    def picard(self, args=[], stdout=None, stdin=None, wait=False):
-        pass
+    def picard(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+        raise FileNotFoundError()
     
     @jar
-    def DISCVRSeq(self, args=[], stdout=None, stdin=None, wait=False):
-        pass
+    def DISCVRSeq(self, args=[], stdout=None, stdin=None, stderr=None,wait=False):
+        raise FileNotFoundError()
```

### Comparing `wgse_ng-0.0.4a4/wgse/genome_file_finder.py` & `wgse_ng-0.0.4a5/wgse/genome_file_finder.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a4/wgse/gui/alignment_statistics_dialog.py` & `wgse_ng-0.0.4a5/wgse/gui/alignment_statistics_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a4/wgse/gui/header.py` & `wgse_ng-0.0.4a5/wgse/gui/header.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a4/wgse/gui/header_dialog.py` & `wgse_ng-0.0.4a5/wgse/gui/header_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a4/wgse/gui/index_statistics_dialog.py` & `wgse_ng-0.0.4a5/wgse/gui/index_statistics_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a4/wgse/gui/table_dialog.py` & `wgse_ng-0.0.4a5/wgse/gui/table_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a4/wgse/variant_caller.py` & `wgse_ng-0.0.4a5/wgse/variant_caller.py`

 * *Files identical despite different names*

