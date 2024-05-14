# Comparing `tmp/wgse_ng-0.0.4a6.tar.gz` & `tmp/wgse_ng-0.0.4a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgse_ng-0.0.4a6.tar", last modified: Tue May 14 10:41:44 2024, max compression
+gzip compressed data, was "wgse_ng-0.0.4a7.tar", last modified: Tue May 14 10:45:08 2024, max compression
```

## Comparing `wgse_ng-0.0.4a6.tar` & `wgse_ng-0.0.4a7.tar`

### file list

```diff
@@ -1,130 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.541765 wgse_ng-0.0.4a6/
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-14 10:41:44.541765 wgse_ng-0.0.4a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.541765 wgse_ng-0.0.4a6/WGSE_NG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-14 10:41:44.000000 wgse_ng-0.0.4a6/WGSE_NG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-14 10:41:44.000000 wgse_ng-0.0.4a6/WGSE_NG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:41:44.000000 wgse_ng-0.0.4a6/WGSE_NG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 10:41:44.000000 wgse_ng-0.0.4a6/WGSE_NG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 10:41:44.000000 wgse_ng-0.0.4a6/WGSE_NG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:41:44.541765 wgse_ng-0.0.4a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.513765 wgse_ng-0.0.4a6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_fasta_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_raw_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/test/test_unknown_bases_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.513765 wgse_ng-0.0.4a6/wgse/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.517765 wgse_ng-0.0.4a6/wgse/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/adapters/alignment_map_file_info_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/adapters/alignment_stats_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/adapters/header_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/adapters/index_stats_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.517765 wgse_ng-0.0.4a6/wgse/alignment_map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/alignment_map_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/alignment_map_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/alignment_map_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/alignment_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/depth_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/alignment_map/index_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.521765 wgse_ng-0.0.4a6/wgse/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/alignment_map_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/alignment_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/chromosome_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/mitochondrial_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/mitochondrial_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/mitochondrial_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/read_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/sequence_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/data/tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.521765 wgse_ng-0.0.4a6/wgse/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/experimental/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.521765 wgse_ng-0.0.4a6/wgse/fasta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/fasta_letter_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/fasta_stats_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/letter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/letter_run_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/letter_run_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fasta/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.521765 wgse_ng-0.0.4a6/wgse/fastq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/fastq/fastq_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.525765 wgse_ng-0.0.4a6/wgse/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/alignment_statistics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/filedrop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/header_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/index_statistics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/microarray_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/table_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/ui_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/gui/ui_form.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.525765 wgse_ng-0.0.4a6/wgse/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.533765 wgse_ng-0.0.4a6/wgse/metadata/bed_templates/
--rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/bed_templates/19_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/bed_templates/19_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/bed_templates/38_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/bed_templates/38_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/bed_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.537765 wgse_ng-0.0.4a6/wgse/metadata/report_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/report_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/report_templates/table_macro.html
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/report_templates/table_simple.html
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/metadata/report_templates/table_tab.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.537765 wgse_ng-0.0.4a6/wgse/microarray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/microarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/microarray/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/microarray/microarray_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/microarray/raw_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.537765 wgse_ng-0.0.4a6/wgse/mtDNA/
--rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/mtDNA/CRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/mtDNA/RSRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/mtDNA/Yoruba.fasta
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/mtDNA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/mtDNA/rCRS.fasta
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.537765 wgse_ng-0.0.4a6/wgse/reference_genome/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/reference_genome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/reference_genome/bgzip_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/reference_genome/decompressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/reference_genome/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/reference_genome/genome_metadata_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/reference_genome/repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.537765 wgse_ng-0.0.4a6/wgse/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/renderers/csv_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/renderers/html_aligned_file_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/renderers/html_simple_table_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:44.541765 wgse_ng-0.0.4a6/wgse/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/check_prerequisites.py
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/file_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/mt_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/sequence_orderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/sequencers.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/utility/unit_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-14 10:41:40.000000 wgse_ng-0.0.4a6/wgse/variant_caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.053007 wgse_ng-0.0.4a7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-14 10:45:08.053007 wgse_ng-0.0.4a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.053007 wgse_ng-0.0.4a7/WGSE_NG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-14 10:45:08.000000 wgse_ng-0.0.4a7/WGSE_NG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-14 10:45:08.000000 wgse_ng-0.0.4a7/WGSE_NG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:45:08.000000 wgse_ng-0.0.4a7/WGSE_NG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 10:45:08.000000 wgse_ng-0.0.4a7/WGSE_NG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 10:45:08.000000 wgse_ng-0.0.4a7/WGSE_NG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:45:08.053007 wgse_ng-0.0.4a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.021006 wgse_ng-0.0.4a7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/test/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/test/test_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/test/test_fasta_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/test/test_microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/test/test_raw_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/test/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/test/test_unknown_bases_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.021006 wgse_ng-0.0.4a7/wgse/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.021006 wgse_ng-0.0.4a7/wgse/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/adapters/alignment_map_file_info_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/adapters/alignment_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/adapters/header_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/adapters/index_stats_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.021006 wgse_ng-0.0.4a7/wgse/alignment_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/alignment_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/alignment_map/alignment_map_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/alignment_map/alignment_map_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/alignment_map/alignment_map_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/alignment_map/alignment_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/alignment_map/depth_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/alignment_map/index_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.025007 wgse_ng-0.0.4a7/wgse/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/alignment_map_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/alignment_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/chromosome_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/mitochondrial_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/mitochondrial_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/mitochondrial_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/read_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/sequence_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/data/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.025007 wgse_ng-0.0.4a7/wgse/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/experimental/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.025007 wgse_ng-0.0.4a7/wgse/fasta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/fasta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/fasta/fasta_letter_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/fasta/fasta_stats_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/fasta/letter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/fasta/letter_run_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/fasta/letter_run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/fasta/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.025007 wgse_ng-0.0.4a7/wgse/fastq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/fastq/fastq_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.029007 wgse_ng-0.0.4a7/wgse/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/gui/alignment_statistics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/gui/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/gui/filedrop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/gui/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/gui/header_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/gui/index_statistics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/gui/microarray_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/gui/table_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/gui/ui_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/gui/ui_form.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.037007 wgse_ng-0.0.4a7/wgse/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.049007 wgse_ng-0.0.4a7/wgse/metadata/bed_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/bed_templates/19_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/bed_templates/19_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/bed_templates/38_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/bed_templates/38_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/bed_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/builds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/mtdna.json
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/ploidy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4875881 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/references.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17094 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/references_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.049007 wgse_ng-0.0.4a7/wgse/metadata/report_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/report_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/report_templates/table_macro.html
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/report_templates/table_simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/report_templates/table_tab.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/sequencers.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/metadata/sources.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.049007 wgse_ng-0.0.4a7/wgse/microarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/microarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/microarray/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/microarray/microarray_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/microarray/raw_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.049007 wgse_ng-0.0.4a7/wgse/mtDNA/
+-rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/mtDNA/CRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/mtDNA/RSRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/mtDNA/Yoruba.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/mtDNA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/mtDNA/rCRS.fasta
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.049007 wgse_ng-0.0.4a7/wgse/reference_genome/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/reference_genome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/reference_genome/bgzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/reference_genome/decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/reference_genome/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/reference_genome/genome_metadata_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/reference_genome/repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.053007 wgse_ng-0.0.4a7/wgse/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/renderers/csv_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/renderers/html_aligned_file_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/renderers/html_simple_table_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:08.053007 wgse_ng-0.0.4a7/wgse/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/utility/check_prerequisites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/utility/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/utility/file_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/utility/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/utility/mt_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/utility/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/utility/sequence_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/utility/sequencers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/utility/unit_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-14 10:45:01.000000 wgse_ng-0.0.4a7/wgse/variant_caller.py
```

### Comparing `wgse_ng-0.0.4a6/PKG-INFO` & `wgse_ng-0.0.4a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 0.0.4a6
+Version: 0.0.4a7
 Summary: Whole Genome Sequencing data manipulation tool
 Home-page: https://github.com/chaplin89/WGSE-NG
 Author: Multiple
 Author-email: 
 Keywords: bioinformatics
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `wgse_ng-0.0.4a6/README.md` & `wgse_ng-0.0.4a7/README.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/WGSE_NG.egg-info/PKG-INFO` & `wgse_ng-0.0.4a7/WGSE_NG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 0.0.4a6
+Version: 0.0.4a7
 Summary: Whole Genome Sequencing data manipulation tool
 Home-page: https://github.com/chaplin89/WGSE-NG
 Author: Multiple
 Author-email: 
 Keywords: bioinformatics
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `wgse_ng-0.0.4a6/WGSE_NG.egg-info/SOURCES.txt` & `wgse_ng-0.0.4a7/WGSE_NG.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,21 @@
 wgse/gui/index_statistics_dialog.py
 wgse/gui/main.py
 wgse/gui/microarray_format.py
 wgse/gui/table_dialog.py
 wgse/gui/ui_extract.py
 wgse/gui/ui_form.py
 wgse/metadata/__init__.py
+wgse/metadata/builds.json
+wgse/metadata/mtdna.json
+wgse/metadata/ploidy.txt
+wgse/metadata/references.json
+wgse/metadata/references_template.json
+wgse/metadata/sequencers.json
+wgse/metadata/sources.json
 wgse/metadata/bed_templates/19_wes.csv
 wgse/metadata/bed_templates/19_y_mt.csv
 wgse/metadata/bed_templates/38_wes.csv
 wgse/metadata/bed_templates/38_y_mt.csv
 wgse/metadata/bed_templates/__init__.py
 wgse/metadata/report_templates/__init__.py
 wgse/metadata/report_templates/table_macro.html
```

### Comparing `wgse_ng-0.0.4a6/setup.py` & `wgse_ng-0.0.4a7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     name="WGSE-NG",
     packages=find_packages(include=["wgse", "wgse.*"]),
     author="Multiple",
     author_email="",
     include_package_data=True,
     package_data={
         "wgse.mtDNA": ["*.*"], 
+        "wgse.metadata": ["*.*"],
         "wgse.metadata.microarray_templates.head": ["*.*"],
         "wgse.metadata.microarray_templates.body": ["*.*"],
         "wgse.metadata.bed_templates": ["*.*"],
         "wgse.metadata.report_templates": ["*.*"],
         },
     description="Whole Genome Sequencing data manipulation tool",
     long_description=open("README.md","r").read(),
```

### Comparing `wgse_ng-0.0.4a6/test/test_buckets.py` & `wgse_ng-0.0.4a7/test/test_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/test/test_fasta.py` & `wgse_ng-0.0.4a7/test/test_fasta.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/test/test_fasta_dictionary.py` & `wgse_ng-0.0.4a7/test/test_fasta_dictionary.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/test/test_microarray_converter.py` & `wgse_ng-0.0.4a7/test/test_microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/test/test_raw_file.py` & `wgse_ng-0.0.4a7/test/test_raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/test/test_sequence.py` & `wgse_ng-0.0.4a7/test/test_sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/test/test_unknown_bases_stats.py` & `wgse_ng-0.0.4a7/test/test_unknown_bases_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/__init__.py` & `wgse_ng-0.0.4a7/wgse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION="v0.0.4alpha6"
+VERSION="v0.0.4alpha7"
 
 # pkgutil shenanigans to make python load wgse.third_party from site-packages
 #
 # tl;dr wgse.third_party contains some executables for windows and is installed
 # from another pypi package (wgse-ng-3rd-party).
 # When importing wgse.third_party from any files inside WGSE, python will expect
 # to find wgse.third_party INSIDE this package and not in site-packages. Code
```

### Comparing `wgse_ng-0.0.4a6/wgse/adapters/alignment_map_file_info_adapter.py` & `wgse_ng-0.0.4a7/wgse/adapters/alignment_map_file_info_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/adapters/alignment_stats_adapter.py` & `wgse_ng-0.0.4a7/wgse/adapters/alignment_stats_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/adapters/header_adapter.py` & `wgse_ng-0.0.4a7/wgse/adapters/header_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/adapters/index_stats_adapter.py` & `wgse_ng-0.0.4a7/wgse/adapters/index_stats_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/alignment_map/alignment_map_file.py` & `wgse_ng-0.0.4a7/wgse/alignment_map/alignment_map_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/alignment_map/alignment_map_header.py` & `wgse_ng-0.0.4a7/wgse/alignment_map/alignment_map_header.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/alignment_map/alignment_map_row.py` & `wgse_ng-0.0.4a7/wgse/alignment_map/alignment_map_row.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/alignment_map/alignment_stats_calculator.py` & `wgse_ng-0.0.4a7/wgse/alignment_map/alignment_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/alignment_map/depth_analyzer.py` & `wgse_ng-0.0.4a7/wgse/alignment_map/depth_analyzer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/alignment_map/index_stats_calculator.py` & `wgse_ng-0.0.4a7/wgse/alignment_map/index_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/configuration.py` & `wgse_ng-0.0.4a7/wgse/configuration.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/data/alignment_map_file_info.py` & `wgse_ng-0.0.4a7/wgse/data/alignment_map_file_info.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/data/alignment_stats.py` & `wgse_ng-0.0.4a7/wgse/data/alignment_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/data/microarray_converter.py` & `wgse_ng-0.0.4a7/wgse/data/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/data/mitochondrial_model.py` & `wgse_ng-0.0.4a7/wgse/data/mitochondrial_model.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/data/reference.py` & `wgse_ng-0.0.4a7/wgse/data/reference.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/data/sequence.py` & `wgse_ng-0.0.4a7/wgse/data/sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/fasta/fasta_letter_counter.py` & `wgse_ng-0.0.4a7/wgse/fasta/fasta_letter_counter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/fasta/fasta_stats_files.py` & `wgse_ng-0.0.4a7/wgse/fasta/fasta_stats_files.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/fasta/letter_run_buckets.py` & `wgse_ng-0.0.4a7/wgse/fasta/letter_run_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/fasta/letter_run_collection.py` & `wgse_ng-0.0.4a7/wgse/fasta/letter_run_collection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/fasta/reference.py` & `wgse_ng-0.0.4a7/wgse/fasta/reference.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/fastq/fastq_file.py` & `wgse_ng-0.0.4a7/wgse/fastq/fastq_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/gui/alignment_statistics_dialog.py` & `wgse_ng-0.0.4a7/wgse/gui/alignment_statistics_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/gui/extract.py` & `wgse_ng-0.0.4a7/wgse/gui/extract.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/gui/filedrop.py` & `wgse_ng-0.0.4a7/wgse/gui/filedrop.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/gui/header.py` & `wgse_ng-0.0.4a7/wgse/gui/header.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/gui/header_dialog.py` & `wgse_ng-0.0.4a7/wgse/gui/header_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/gui/index_statistics_dialog.py` & `wgse_ng-0.0.4a7/wgse/gui/index_statistics_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/gui/main.py` & `wgse_ng-0.0.4a7/wgse/gui/main.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/gui/microarray_format.py` & `wgse_ng-0.0.4a7/wgse/gui/microarray_format.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/gui/table_dialog.py` & `wgse_ng-0.0.4a7/wgse/gui/table_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/gui/ui_extract.py` & `wgse_ng-0.0.4a7/wgse/gui/ui_extract.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/gui/ui_form.py` & `wgse_ng-0.0.4a7/wgse/gui/ui_form.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/metadata/bed_templates/19_wes.csv` & `wgse_ng-0.0.4a7/wgse/metadata/bed_templates/19_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/metadata/bed_templates/38_wes.csv` & `wgse_ng-0.0.4a7/wgse/metadata/bed_templates/38_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/metadata/bed_templates/38_y_mt.csv` & `wgse_ng-0.0.4a7/wgse/metadata/bed_templates/38_y_mt.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/metadata/report_templates/table_macro.html` & `wgse_ng-0.0.4a7/wgse/metadata/report_templates/table_macro.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/metadata/report_templates/table_simple.html` & `wgse_ng-0.0.4a7/wgse/metadata/report_templates/table_simple.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/metadata/report_templates/table_tab.html` & `wgse_ng-0.0.4a7/wgse/metadata/report_templates/table_tab.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/microarray/microarray_converter.py` & `wgse_ng-0.0.4a7/wgse/microarray/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/microarray/microarray_line_formatter.py` & `wgse_ng-0.0.4a7/wgse/microarray/microarray_line_formatter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/microarray/raw_file.py` & `wgse_ng-0.0.4a7/wgse/microarray/raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/mtDNA/CRS.fasta` & `wgse_ng-0.0.4a7/wgse/mtDNA/CRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/mtDNA/RSRS.fasta` & `wgse_ng-0.0.4a7/wgse/mtDNA/RSRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/mtDNA/Yoruba.fasta` & `wgse_ng-0.0.4a7/wgse/mtDNA/Yoruba.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/mtDNA/rCRS.fasta` & `wgse_ng-0.0.4a7/wgse/mtDNA/rCRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/reference_genome/decompressor.py` & `wgse_ng-0.0.4a7/wgse/reference_genome/decompressor.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/reference_genome/downloader.py` & `wgse_ng-0.0.4a7/wgse/reference_genome/downloader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/reference_genome/genome_metadata_loader.py` & `wgse_ng-0.0.4a7/wgse/reference_genome/genome_metadata_loader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/reference_genome/repository_manager.py` & `wgse_ng-0.0.4a7/wgse/reference_genome/repository_manager.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/renderers/html_aligned_file_report.py` & `wgse_ng-0.0.4a7/wgse/renderers/html_aligned_file_report.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/renderers/html_simple_table_report.py` & `wgse_ng-0.0.4a7/wgse/renderers/html_simple_table_report.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/utility/check_prerequisites.py` & `wgse_ng-0.0.4a7/wgse/utility/check_prerequisites.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/utility/external.py` & `wgse_ng-0.0.4a7/wgse/utility/external.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/utility/file_type_checker.py` & `wgse_ng-0.0.4a7/wgse/utility/file_type_checker.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/utility/mt_dna.py` & `wgse_ng-0.0.4a7/wgse/utility/mt_dna.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/utility/regions.py` & `wgse_ng-0.0.4a7/wgse/utility/regions.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/utility/sequence_orderer.py` & `wgse_ng-0.0.4a7/wgse/utility/sequence_orderer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/utility/sequencers.py` & `wgse_ng-0.0.4a7/wgse/utility/sequencers.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a6/wgse/variant_caller.py` & `wgse_ng-0.0.4a7/wgse/variant_caller.py`

 * *Files identical despite different names*

