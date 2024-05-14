# Comparing `tmp/wgse_ng-0.0.4a8.tar.gz` & `tmp/wgse_ng-0.0.4a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgse_ng-0.0.4a8.tar", last modified: Tue May 14 11:09:25 2024, max compression
+gzip compressed data, was "wgse_ng-0.0.4a9.tar", last modified: Tue May 14 11:25:36 2024, max compression
```

## Comparing `wgse_ng-0.0.4a8.tar` & `wgse_ng-0.0.4a9.tar`

### file list

```diff
@@ -1,137 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.359851 wgse_ng-0.0.4a8/
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-14 11:09:25.359851 wgse_ng-0.0.4a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.359851 wgse_ng-0.0.4a8/WGSE_NG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-14 11:09:25.000000 wgse_ng-0.0.4a8/WGSE_NG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-14 11:09:25.000000 wgse_ng-0.0.4a8/WGSE_NG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:09:25.000000 wgse_ng-0.0.4a8/WGSE_NG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 11:09:25.000000 wgse_ng-0.0.4a8/WGSE_NG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 11:09:25.000000 wgse_ng-0.0.4a8/WGSE_NG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:09:25.359851 wgse_ng-0.0.4a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.327851 wgse_ng-0.0.4a8/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/test/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/test/test_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/test/test_fasta_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/test/test_microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/test/test_raw_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/test/test_unknown_bases_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.327851 wgse_ng-0.0.4a8/wgse/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.327851 wgse_ng-0.0.4a8/wgse/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/adapters/alignment_map_file_info_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/adapters/alignment_stats_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/adapters/header_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/adapters/index_stats_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.327851 wgse_ng-0.0.4a8/wgse/alignment_map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/alignment_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/alignment_map/alignment_map_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/alignment_map/alignment_map_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/alignment_map/alignment_map_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/alignment_map/alignment_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/alignment_map/depth_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/alignment_map/index_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.331851 wgse_ng-0.0.4a8/wgse/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/alignment_map_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/alignment_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/chromosome_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/mitochondrial_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/mitochondrial_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/mitochondrial_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/read_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/sequence_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/data/tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.331851 wgse_ng-0.0.4a8/wgse/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/experimental/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.331851 wgse_ng-0.0.4a8/wgse/fasta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/fasta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/fasta/fasta_letter_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/fasta/fasta_stats_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/fasta/letter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/fasta/letter_run_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/fasta/letter_run_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/fasta/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.331851 wgse_ng-0.0.4a8/wgse/fastq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/fastq/fastq_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.335851 wgse_ng-0.0.4a8/wgse/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/gui/alignment_statistics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/gui/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/gui/filedrop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/gui/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/gui/header_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/gui/index_statistics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/gui/microarray_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/gui/table_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/gui/ui_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/gui/ui_form.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.339851 wgse_ng-0.0.4a8/wgse/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.351851 wgse_ng-0.0.4a8/wgse/metadata/bed_templates/
--rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/metadata/bed_templates/19_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/metadata/bed_templates/19_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/metadata/bed_templates/38_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/metadata/bed_templates/38_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/metadata/bed_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:20.000000 wgse_ng-0.0.4a8/wgse/metadata/builds.json
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/metadata/mtdna.json
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/metadata/ploidy.txt
--rw-r--r--   0 runner    (1001) docker     (127)  4875881 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/metadata/references.json
--rw-r--r--   0 runner    (1001) docker     (127)    17094 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/metadata/references_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.351851 wgse_ng-0.0.4a8/wgse/metadata/report_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/metadata/report_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/metadata/report_templates/table_macro.html
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/metadata/report_templates/table_simple.html
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/metadata/report_templates/table_tab.html
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/metadata/sequencers.json
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/metadata/sources.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.355851 wgse_ng-0.0.4a8/wgse/microarray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/microarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/microarray/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/microarray/microarray_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/microarray/raw_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.355851 wgse_ng-0.0.4a8/wgse/mtDNA/
--rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/mtDNA/CRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/mtDNA/RSRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/mtDNA/Yoruba.fasta
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/mtDNA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/mtDNA/rCRS.fasta
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.355851 wgse_ng-0.0.4a8/wgse/reference_genome/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/reference_genome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/reference_genome/bgzip_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/reference_genome/decompressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/reference_genome/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/reference_genome/genome_metadata_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/reference_genome/repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.355851 wgse_ng-0.0.4a8/wgse/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/renderers/csv_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/renderers/html_aligned_file_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/renderers/html_simple_table_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:25.359851 wgse_ng-0.0.4a8/wgse/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/utility/check_prerequisites.py
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/utility/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/utility/file_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/utility/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/utility/mt_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/utility/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/utility/sequence_orderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/utility/sequencers.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/utility/unit_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-14 11:09:21.000000 wgse_ng-0.0.4a8/wgse/variant_caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.474474 wgse_ng-0.0.4a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-14 11:25:36.474474 wgse_ng-0.0.4a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.474474 wgse_ng-0.0.4a9/WGSE_NG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-14 11:25:36.000000 wgse_ng-0.0.4a9/WGSE_NG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-14 11:25:36.000000 wgse_ng-0.0.4a9/WGSE_NG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:25:36.000000 wgse_ng-0.0.4a9/WGSE_NG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 11:25:36.000000 wgse_ng-0.0.4a9/WGSE_NG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 11:25:36.000000 wgse_ng-0.0.4a9/WGSE_NG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 11:25:36.000000 wgse_ng-0.0.4a9/WGSE_NG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:25:36.474474 wgse_ng-0.0.4a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.438475 wgse_ng-0.0.4a9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/test/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/test/test_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/test/test_fasta_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/test/test_microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/test/test_raw_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/test/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/test/test_unknown_bases_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.438475 wgse_ng-0.0.4a9/wgse/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.442475 wgse_ng-0.0.4a9/wgse/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/adapters/alignment_map_file_info_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/adapters/alignment_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/adapters/header_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/adapters/index_stats_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.442475 wgse_ng-0.0.4a9/wgse/alignment_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/alignment_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/alignment_map/alignment_map_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/alignment_map/alignment_map_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/alignment_map/alignment_map_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/alignment_map/alignment_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/alignment_map/depth_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/alignment_map/index_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.446475 wgse_ng-0.0.4a9/wgse/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/alignment_map_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/alignment_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/chromosome_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/mitochondrial_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/mitochondrial_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/mitochondrial_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/read_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/sequence_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/data/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.446475 wgse_ng-0.0.4a9/wgse/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/experimental/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.446475 wgse_ng-0.0.4a9/wgse/fasta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/fasta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/fasta/fasta_letter_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/fasta/fasta_stats_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/fasta/letter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/fasta/letter_run_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/fasta/letter_run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/fasta/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.446475 wgse_ng-0.0.4a9/wgse/fastq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/fastq/fastq_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.450475 wgse_ng-0.0.4a9/wgse/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/gui/alignment_statistics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/gui/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/gui/filedrop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/gui/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/gui/header_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/gui/index_statistics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/gui/microarray_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/gui/table_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/gui/ui_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/gui/ui_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.458474 wgse_ng-0.0.4a9/wgse/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.470474 wgse_ng-0.0.4a9/wgse/metadata/bed_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/bed_templates/19_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/bed_templates/19_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/bed_templates/38_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/bed_templates/38_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/bed_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/builds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/mtdna.json
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/ploidy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4875881 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/references.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17094 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/references_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.470474 wgse_ng-0.0.4a9/wgse/metadata/report_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/report_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/report_templates/table_macro.html
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/report_templates/table_simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/report_templates/table_tab.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/sequencers.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/metadata/sources.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.470474 wgse_ng-0.0.4a9/wgse/microarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/microarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/microarray/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/microarray/microarray_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/microarray/raw_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.470474 wgse_ng-0.0.4a9/wgse/mtDNA/
+-rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/mtDNA/CRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/mtDNA/RSRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/mtDNA/Yoruba.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/mtDNA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/mtDNA/rCRS.fasta
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.470474 wgse_ng-0.0.4a9/wgse/reference_genome/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/reference_genome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/reference_genome/bgzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/reference_genome/decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/reference_genome/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/reference_genome/genome_metadata_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/reference_genome/repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.474474 wgse_ng-0.0.4a9/wgse/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/renderers/csv_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/renderers/html_aligned_file_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/renderers/html_simple_table_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:36.474474 wgse_ng-0.0.4a9/wgse/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/utility/check_prerequisites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/utility/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/utility/file_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/utility/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/utility/mt_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/utility/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/utility/sequence_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/utility/sequencers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/utility/unit_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-14 11:25:32.000000 wgse_ng-0.0.4a9/wgse/variant_caller.py
```

### Comparing `wgse_ng-0.0.4a8/PKG-INFO` & `wgse_ng-0.0.4a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 0.0.4a8
+Version: 0.0.4a9
 Summary: Whole Genome Sequencing data manipulation tool
 Home-page: https://github.com/chaplin89/WGSE-NG
 Author: Multiple
 Author-email: 
 Keywords: bioinformatics
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `wgse_ng-0.0.4a8/README.md` & `wgse_ng-0.0.4a9/README.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/WGSE_NG.egg-info/PKG-INFO` & `wgse_ng-0.0.4a9/WGSE_NG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 0.0.4a8
+Version: 0.0.4a9
 Summary: Whole Genome Sequencing data manipulation tool
 Home-page: https://github.com/chaplin89/WGSE-NG
 Author: Multiple
 Author-email: 
 Keywords: bioinformatics
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `wgse_ng-0.0.4a8/WGSE_NG.egg-info/SOURCES.txt` & `wgse_ng-0.0.4a9/WGSE_NG.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 README.md
 setup.py
 WGSE_NG.egg-info/PKG-INFO
 WGSE_NG.egg-info/SOURCES.txt
 WGSE_NG.egg-info/dependency_links.txt
+WGSE_NG.egg-info/entry_points.txt
 WGSE_NG.egg-info/requires.txt
 WGSE_NG.egg-info/top_level.txt
 test/test_buckets.py
 test/test_fasta.py
 test/test_fasta_dictionary.py
 test/test_microarray_converter.py
 test/test_raw_file.py
 test/test_sequence.py
 test/test_unknown_bases_stats.py
+wgse/VERSION.py
 wgse/__init__.py
 wgse/configuration.py
+wgse/main.py
 wgse/variant_caller.py
 wgse/adapters/__init__.py
 wgse/adapters/alignment_map_file_info_adapter.py
 wgse/adapters/alignment_stats_adapter.py
 wgse/adapters/header_adapter.py
 wgse/adapters/index_stats_adapter.py
 wgse/alignment_map/__init__.py
```

### Comparing `wgse_ng-0.0.4a8/setup.py` & `wgse_ng-0.0.4a9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import find_packages, setup
-from wgse import VERSION
+from wgse.VERSION import VERSION
 
 DEPENDENCIES = [
     "setuptools",
     "pefile",
     "pycurl",
     "tqdm",
     "google-cloud-storage",
@@ -44,9 +44,14 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
+    entry_points={
+        'gui_scripts': [
+            'wgse = wgse.main:main',
+        ]
+    },
     keywords="bioinformatics",
 )
```

### Comparing `wgse_ng-0.0.4a8/test/test_buckets.py` & `wgse_ng-0.0.4a9/test/test_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/test/test_fasta.py` & `wgse_ng-0.0.4a9/test/test_fasta.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/test/test_fasta_dictionary.py` & `wgse_ng-0.0.4a9/test/test_fasta_dictionary.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/test/test_microarray_converter.py` & `wgse_ng-0.0.4a9/test/test_microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/test/test_raw_file.py` & `wgse_ng-0.0.4a9/test/test_raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/test/test_sequence.py` & `wgse_ng-0.0.4a9/test/test_sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/test/test_unknown_bases_stats.py` & `wgse_ng-0.0.4a9/test/test_unknown_bases_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/adapters/alignment_map_file_info_adapter.py` & `wgse_ng-0.0.4a9/wgse/adapters/alignment_map_file_info_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/adapters/alignment_stats_adapter.py` & `wgse_ng-0.0.4a9/wgse/adapters/alignment_stats_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/adapters/header_adapter.py` & `wgse_ng-0.0.4a9/wgse/adapters/header_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/adapters/index_stats_adapter.py` & `wgse_ng-0.0.4a9/wgse/adapters/index_stats_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/alignment_map/alignment_map_file.py` & `wgse_ng-0.0.4a9/wgse/alignment_map/alignment_map_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/alignment_map/alignment_map_header.py` & `wgse_ng-0.0.4a9/wgse/alignment_map/alignment_map_header.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/alignment_map/alignment_map_row.py` & `wgse_ng-0.0.4a9/wgse/alignment_map/alignment_map_row.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/alignment_map/alignment_stats_calculator.py` & `wgse_ng-0.0.4a9/wgse/alignment_map/alignment_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/alignment_map/depth_analyzer.py` & `wgse_ng-0.0.4a9/wgse/alignment_map/depth_analyzer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/alignment_map/index_stats_calculator.py` & `wgse_ng-0.0.4a9/wgse/alignment_map/index_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/configuration.py` & `wgse_ng-0.0.4a9/wgse/configuration.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/data/alignment_map_file_info.py` & `wgse_ng-0.0.4a9/wgse/data/alignment_map_file_info.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/data/alignment_stats.py` & `wgse_ng-0.0.4a9/wgse/data/alignment_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/data/microarray_converter.py` & `wgse_ng-0.0.4a9/wgse/data/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/data/mitochondrial_model.py` & `wgse_ng-0.0.4a9/wgse/data/mitochondrial_model.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/data/reference.py` & `wgse_ng-0.0.4a9/wgse/data/reference.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/data/sequence.py` & `wgse_ng-0.0.4a9/wgse/data/sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/fasta/fasta_letter_counter.py` & `wgse_ng-0.0.4a9/wgse/fasta/fasta_letter_counter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/fasta/fasta_stats_files.py` & `wgse_ng-0.0.4a9/wgse/fasta/fasta_stats_files.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/fasta/letter_run_buckets.py` & `wgse_ng-0.0.4a9/wgse/fasta/letter_run_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/fasta/letter_run_collection.py` & `wgse_ng-0.0.4a9/wgse/fasta/letter_run_collection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/fasta/reference.py` & `wgse_ng-0.0.4a9/wgse/fasta/reference.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/fastq/fastq_file.py` & `wgse_ng-0.0.4a9/wgse/fastq/fastq_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/gui/alignment_statistics_dialog.py` & `wgse_ng-0.0.4a9/wgse/gui/alignment_statistics_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/gui/extract.py` & `wgse_ng-0.0.4a9/wgse/gui/extract.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/gui/filedrop.py` & `wgse_ng-0.0.4a9/wgse/gui/filedrop.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/gui/header.py` & `wgse_ng-0.0.4a9/wgse/gui/header.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/gui/header_dialog.py` & `wgse_ng-0.0.4a9/wgse/gui/header_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/gui/index_statistics_dialog.py` & `wgse_ng-0.0.4a9/wgse/gui/index_statistics_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/gui/main.py` & `wgse_ng-0.0.4a9/wgse/gui/main.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/gui/microarray_format.py` & `wgse_ng-0.0.4a9/wgse/gui/microarray_format.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/gui/table_dialog.py` & `wgse_ng-0.0.4a9/wgse/gui/table_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/gui/ui_extract.py` & `wgse_ng-0.0.4a9/wgse/gui/ui_extract.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/gui/ui_form.py` & `wgse_ng-0.0.4a9/wgse/gui/ui_form.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/metadata/bed_templates/19_wes.csv` & `wgse_ng-0.0.4a9/wgse/metadata/bed_templates/19_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/metadata/bed_templates/38_wes.csv` & `wgse_ng-0.0.4a9/wgse/metadata/bed_templates/38_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/metadata/bed_templates/38_y_mt.csv` & `wgse_ng-0.0.4a9/wgse/metadata/bed_templates/38_y_mt.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/metadata/mtdna.json` & `wgse_ng-0.0.4a9/wgse/metadata/mtdna.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/metadata/references.json` & `wgse_ng-0.0.4a9/wgse/metadata/references.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/metadata/references_template.json` & `wgse_ng-0.0.4a9/wgse/metadata/references_template.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/metadata/report_templates/table_macro.html` & `wgse_ng-0.0.4a9/wgse/metadata/report_templates/table_macro.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/metadata/report_templates/table_simple.html` & `wgse_ng-0.0.4a9/wgse/metadata/report_templates/table_simple.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/metadata/report_templates/table_tab.html` & `wgse_ng-0.0.4a9/wgse/metadata/report_templates/table_tab.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/metadata/sequencers.json` & `wgse_ng-0.0.4a9/wgse/metadata/sequencers.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/metadata/sources.json` & `wgse_ng-0.0.4a9/wgse/metadata/sources.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/microarray/microarray_converter.py` & `wgse_ng-0.0.4a9/wgse/microarray/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/microarray/microarray_line_formatter.py` & `wgse_ng-0.0.4a9/wgse/microarray/microarray_line_formatter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/microarray/raw_file.py` & `wgse_ng-0.0.4a9/wgse/microarray/raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/mtDNA/CRS.fasta` & `wgse_ng-0.0.4a9/wgse/mtDNA/CRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/mtDNA/RSRS.fasta` & `wgse_ng-0.0.4a9/wgse/mtDNA/RSRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/mtDNA/Yoruba.fasta` & `wgse_ng-0.0.4a9/wgse/mtDNA/Yoruba.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/mtDNA/rCRS.fasta` & `wgse_ng-0.0.4a9/wgse/mtDNA/rCRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/reference_genome/decompressor.py` & `wgse_ng-0.0.4a9/wgse/reference_genome/decompressor.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/reference_genome/downloader.py` & `wgse_ng-0.0.4a9/wgse/reference_genome/downloader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/reference_genome/genome_metadata_loader.py` & `wgse_ng-0.0.4a9/wgse/reference_genome/genome_metadata_loader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/reference_genome/repository_manager.py` & `wgse_ng-0.0.4a9/wgse/reference_genome/repository_manager.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/renderers/html_aligned_file_report.py` & `wgse_ng-0.0.4a9/wgse/renderers/html_aligned_file_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from wgse.adapters.alignment_stats_adapter import AlignmentStatsAdapter
 from wgse.adapters.header_adapter import HeaderAdapter
 from wgse.adapters.index_stats_adapter import IndexStatsAdapter
 from wgse.alignment_map.alignment_map_file import AlignmentMapFile
 from wgse.alignment_map.alignment_map_header import AlignmentMapHeader
 from wgse.configuration import MANAGER_CFG
 from wgse.data.tabular_data import TabularData
-from wgse import VERSION
+from wgse.VERSION import VERSION
 
 
 class HTMLAlignedFileReport:
     def __init__(self, config=MANAGER_CFG.REPOSITORY) -> None:
         self._templates_folder = config.metadata.joinpath("report_templates")
 
     def from_aligned_file(file=AlignmentMapFile):
```

### Comparing `wgse_ng-0.0.4a8/wgse/renderers/html_simple_table_report.py` & `wgse_ng-0.0.4a9/wgse/renderers/html_simple_table_report.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/utility/check_prerequisites.py` & `wgse_ng-0.0.4a9/wgse/utility/check_prerequisites.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/utility/external.py` & `wgse_ng-0.0.4a9/wgse/utility/external.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/utility/file_type_checker.py` & `wgse_ng-0.0.4a9/wgse/utility/file_type_checker.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/utility/mt_dna.py` & `wgse_ng-0.0.4a9/wgse/utility/mt_dna.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/utility/regions.py` & `wgse_ng-0.0.4a9/wgse/utility/regions.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/utility/sequence_orderer.py` & `wgse_ng-0.0.4a9/wgse/utility/sequence_orderer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/utility/sequencers.py` & `wgse_ng-0.0.4a9/wgse/utility/sequencers.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a8/wgse/variant_caller.py` & `wgse_ng-0.0.4a9/wgse/variant_caller.py`

 * *Files identical despite different names*

