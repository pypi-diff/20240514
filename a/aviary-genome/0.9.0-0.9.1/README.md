# Comparing `tmp/aviary-genome-0.9.0.tar.gz` & `tmp/aviary-genome-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aviary-genome-0.9.0.tar", last modified: Tue Mar 12 03:13:03 2024, max compression
+gzip compressed data, was "aviary-genome-0.9.1.tar", last modified: Tue May 14 02:47:11 2024, max compression
```

## Comparing `aviary-genome-0.9.0.tar` & `aviary-genome-0.9.1.tar`

### file list

```diff
@@ -1,161 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.560391 aviary-genome-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       43 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-03-12 03:13:03.560391 aviary-genome-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.544391 aviary-genome-0.9.0/aviary/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    55763 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/aviary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.544391 aviary-genome-0.9.0/aviary/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.544391 aviary-genome-0.9.0/aviary/envs/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/envs/checkm.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/envs/checkm2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/envs/coverm.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/envs/groopm.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/envs/gtdbtk.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/envs/minimap2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/envs/singlem.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/envs/webpage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.544391 aviary-genome-0.9.0/aviary/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/Snakefile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.544391 aviary-genome-0.9.0/aviary/modules/annotation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/annotation/annotation.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.544391 aviary-genome-0.9.0/aviary/modules/annotation/envs/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/annotation/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/annotation/envs/busco.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       97 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/annotation/envs/eggnog.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.544391 aviary-genome-0.9.0/aviary/modules/annotation/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/annotation/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.548391 aviary-genome-0.9.0/aviary/modules/assembly/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27069 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/assembly.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.548391 aviary-genome-0.9.0/aviary/modules/assembly/envs/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/envs/circlator.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/envs/final_assembly.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/envs/flye.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/envs/medaka.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/envs/megahit.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/envs/mfqe.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/envs/pilon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/envs/polishing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/envs/pysam.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/envs/seqtk.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/envs/spades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/isolate.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.548391 aviary-genome-0.9.0/aviary/modules/assembly/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4636 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/scripts/assemble_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/scripts/assemble_short_reads.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1437 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/scripts/combine_assemblies.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6437 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/scripts/filter_illumina_assembly.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4838 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/scripts/generate_pilon_sort.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7106 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/scripts/get_binned_reads.py
--rw-r--r--   0 runner    (1001) docker     (127)    16701 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/scripts/polish.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/scripts/pool_reads.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2360 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/assembly/scripts/run_flye.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.548391 aviary-genome-0.9.0/aviary/modules/benchmarking/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/benchmarking/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    48774 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/benchmarking/benchmarking.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.548391 aviary-genome-0.9.0/aviary/modules/benchmarking/envs/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/benchmarking/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/benchmarking/envs/magpurify.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.548391 aviary-genome-0.9.0/aviary/modules/benchmarking/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/benchmarking/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.548391 aviary-genome-0.9.0/aviary/modules/binning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32690 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/binning.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.552391 aviary-genome-0.9.0/aviary/modules/binning/envs/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/envs/concoct.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/envs/das_tool.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/envs/maxbin2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/envs/metabat2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/envs/rosella.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/envs/semibin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/envs/vamb.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.552391 aviary-genome-0.9.0/aviary/modules/binning/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/scripts/das_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/scripts/finalise_recovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/scripts/finalise_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/scripts/get_abundances.py
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/scripts/get_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/scripts/make_long_cov.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/scripts/prepare_rosella_input.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13058 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/scripts/rosella_refine.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1833 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/scripts/run_checkm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/binning/scripts/write_vamb_bins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.552391 aviary-genome-0.9.0/aviary/modules/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/cluster/clustering.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.552391 aviary-genome-0.9.0/aviary/modules/cluster/envs/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/cluster/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       93 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/cluster/envs/pggb.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.552391 aviary-genome-0.9.0/aviary/modules/cluster/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/cluster/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26970 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.552391 aviary-genome-0.9.0/aviary/modules/quality_control/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.552391 aviary-genome-0.9.0/aviary/modules/quality_control/envs/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       99 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/envs/chopper.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/envs/fastqc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/envs/nanoplot.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/envs/quast.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     7126 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/qc.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.556391 aviary-genome-0.9.0/aviary/modules/quality_control/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/scripts/filter_read_list.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2824 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/scripts/fraction_recovered.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/scripts/qc_long_reads.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17515 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/scripts/qc_short_reads.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2316 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/quality_control/scripts/run_fastqc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.556391 aviary-genome-0.9.0/aviary/modules/strain_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/strain_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.556391 aviary-genome-0.9.0/aviary/modules/strain_analysis/envs/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/strain_analysis/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       85 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/strain_analysis/envs/lorikeet.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.556391 aviary-genome-0.9.0/aviary/modules/strain_analysis/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/strain_analysis/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1828 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/strain_analysis/scripts/run_lorikeet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/strain_analysis/strain_analysis.smk
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/template_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.556391 aviary-genome-0.9.0/aviary/modules/viral_analysis/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/viral_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.556391 aviary-genome-0.9.0/aviary/modules/viral_analysis/envs/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/viral_analysis/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/viral_analysis/envs/virfinder.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/viral_analysis/envs/virsorter.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.556391 aviary-genome-0.9.0/aviary/modules/viral_analysis/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/viral_analysis/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      622 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/modules/viral_analysis/viral_analysis.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.556391 aviary-genome-0.9.0/aviary/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   211909 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/scripts/create_aviary_webpage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/scripts/process_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/scripts/process_viral_batch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       30 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/scripts/run_busco.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/scripts/run_virfinder.R
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/scripts/singlem_appraise.py
--rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/aviary/scripts/singlem_reads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.556391 aviary-genome-0.9.0/aviary_genome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-03-12 03:13:03.000000 aviary-genome-0.9.0/aviary_genome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-03-12 03:13:03.000000 aviary-genome-0.9.0/aviary_genome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 03:13:03.000000 aviary-genome-0.9.0/aviary_genome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-12 03:13:03.000000 aviary-genome-0.9.0/aviary_genome.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 03:13:03.000000 aviary-genome-0.9.0/aviary_genome.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-12 03:13:03.000000 aviary-genome-0.9.0/aviary_genome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-12 03:13:03.000000 aviary-genome-0.9.0/aviary_genome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 03:13:03.560391 aviary-genome-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:13:03.560391 aviary-genome-0.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/test/test_assemble.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7703 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/test/test_recover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-03-12 03:13:01.000000 aviary-genome-0.9.0/test/test_run_checkm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.684807 aviary-genome-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       43 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-14 02:47:11.684807 aviary-genome-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.664807 aviary-genome-0.9.1/aviary/
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53575 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/aviary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.664807 aviary-genome-0.9.1/aviary/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.668807 aviary-genome-0.9.1/aviary/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/envs/checkm.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/envs/checkm2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/envs/coverm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/envs/groopm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/envs/gtdbtk.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/envs/minimap2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/envs/singlem.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/envs/webpage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.668807 aviary-genome-0.9.1/aviary/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.668807 aviary-genome-0.9.1/aviary/modules/annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/annotation/annotation.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.668807 aviary-genome-0.9.1/aviary/modules/annotation/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/annotation/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/annotation/envs/busco.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       97 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/annotation/envs/eggnog.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.668807 aviary-genome-0.9.1/aviary/modules/annotation/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/annotation/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.668807 aviary-genome-0.9.1/aviary/modules/assembly/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25717 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/assembly.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.672807 aviary-genome-0.9.1/aviary/modules/assembly/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/envs/circlator.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/envs/final_assembly.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/envs/flye.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/envs/medaka.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/envs/megahit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/envs/mfqe.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/envs/pilon.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/envs/polishing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/envs/pysam.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/envs/seqtk.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/envs/spades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/isolate.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.672807 aviary-genome-0.9.1/aviary/modules/assembly/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4636 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/scripts/assemble_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/scripts/assemble_short_reads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1437 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/scripts/combine_assemblies.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6437 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/scripts/filter_illumina_assembly.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4838 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/scripts/generate_pilon_sort.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7106 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/scripts/get_binned_reads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16701 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/scripts/polish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/scripts/pool_reads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2360 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/scripts/run_flye.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/assembly/scripts/spades_assembly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.672807 aviary-genome-0.9.1/aviary/modules/benchmarking/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/benchmarking/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48774 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/benchmarking/benchmarking.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.672807 aviary-genome-0.9.1/aviary/modules/benchmarking/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/benchmarking/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/benchmarking/envs/magpurify.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.672807 aviary-genome-0.9.1/aviary/modules/benchmarking/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/benchmarking/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.672807 aviary-genome-0.9.1/aviary/modules/binning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32690 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/binning.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.676807 aviary-genome-0.9.1/aviary/modules/binning/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/envs/concoct.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/envs/das_tool.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/envs/maxbin2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/envs/metabat2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/envs/rosella.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/envs/semibin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/envs/vamb.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.676807 aviary-genome-0.9.1/aviary/modules/binning/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/scripts/das_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/scripts/finalise_recovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/scripts/finalise_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/scripts/get_abundances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/scripts/get_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/scripts/make_long_cov.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/scripts/prepare_rosella_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13058 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/scripts/rosella_refine.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1833 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/scripts/run_checkm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/binning/scripts/write_vamb_bins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.676807 aviary-genome-0.9.1/aviary/modules/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/cluster/clustering.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.676807 aviary-genome-0.9.1/aviary/modules/cluster/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/cluster/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       93 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/cluster/envs/pggb.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.676807 aviary-genome-0.9.1/aviary/modules/cluster/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/cluster/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27641 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.676807 aviary-genome-0.9.1/aviary/modules/quality_control/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.676807 aviary-genome-0.9.1/aviary/modules/quality_control/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       99 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/envs/chopper.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/envs/fastqc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/envs/nanoplot.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/envs/quast.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7126 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/qc.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.680807 aviary-genome-0.9.1/aviary/modules/quality_control/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/scripts/filter_read_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2824 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/scripts/fraction_recovered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/scripts/qc_long_reads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17515 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/scripts/qc_short_reads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2316 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/quality_control/scripts/run_fastqc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.680807 aviary-genome-0.9.1/aviary/modules/strain_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/strain_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.680807 aviary-genome-0.9.1/aviary/modules/strain_analysis/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/strain_analysis/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       85 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/strain_analysis/envs/lorikeet.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.680807 aviary-genome-0.9.1/aviary/modules/strain_analysis/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/strain_analysis/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1828 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/strain_analysis/scripts/run_lorikeet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/strain_analysis/strain_analysis.smk
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/template_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.680807 aviary-genome-0.9.1/aviary/modules/viral_analysis/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/viral_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.680807 aviary-genome-0.9.1/aviary/modules/viral_analysis/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/viral_analysis/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/viral_analysis/envs/virfinder.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/viral_analysis/envs/virsorter.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.680807 aviary-genome-0.9.1/aviary/modules/viral_analysis/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/viral_analysis/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      622 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/modules/viral_analysis/viral_analysis.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.680807 aviary-genome-0.9.1/aviary/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   211909 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/scripts/create_aviary_webpage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/scripts/process_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/scripts/process_viral_batch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       30 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/scripts/run_busco.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/scripts/run_virfinder.R
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/scripts/singlem_appraise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/aviary/scripts/singlem_reads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.684807 aviary-genome-0.9.1/aviary_genome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-14 02:47:11.000000 aviary-genome-0.9.1/aviary_genome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-14 02:47:11.000000 aviary-genome-0.9.1/aviary_genome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 02:47:11.000000 aviary-genome-0.9.1/aviary_genome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 02:47:11.000000 aviary-genome-0.9.1/aviary_genome.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 02:47:11.000000 aviary-genome-0.9.1/aviary_genome.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 02:47:11.000000 aviary-genome-0.9.1/aviary_genome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 02:47:11.000000 aviary-genome-0.9.1/aviary_genome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 02:47:11.684807 aviary-genome-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:47:11.684807 aviary-genome-0.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/test/test_assemble.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9435 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/test/test_recover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-14 02:47:08.000000 aviary-genome-0.9.1/test/test_run_checkm.py
```

### Comparing `aviary-genome-0.9.0/LICENSE` & `aviary-genome-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/PKG-INFO` & `aviary-genome-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aviary-genome
-Version: 0.9.0
+Version: 0.9.1
 Summary: aviary - metagenomics pipeline using long and short reads
 Home-page: https://github.com/rhysnewell/aviary
 Author: Rhys Newell
 Author-email: rhys.newell94@gmail.com
 License: GPL-3.0
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
```

### Comparing `aviary-genome-0.9.0/README.md` & `aviary-genome-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/aviary.py` & `aviary-genome-0.9.1/aviary/aviary.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #                                                                             #
 # You should have received a copy of the GNU General Public License           #
 # along with this program. If not, see <http://www.gnu.org/licenses/>.        #
 #                                                                             #
 ###############################################################################
 import aviary.config.config as Config
 from aviary.modules.processor import Processor, process_batch
-from .__init__ import __version__
+from .__init__ import __version__, MEDAKA_MODELS, LONG_READ_TYPES
 __author__ = "Rhys Newell"
 __copyright__ = "Copyright 2022"
 __credits__ = ["Rhys Newell"]
 __license__ = "GPL3"
 __maintainer__ = "Rhys Newell"
 __email__ = "rhys.newell near hdr.qut.edu.au"
 __status__ = "Development"
@@ -31,15 +31,14 @@
 ###############################################################################
 # System imports
 import sys
 import argparse
 import logging
 import os
 from datetime import datetime
-import tempfile
 
 # Debug
 debug={1:logging.CRITICAL,
        2:logging.ERROR,
        3:logging.WARNING,
        4:logging.INFO,
        5:logging.DEBUG}
@@ -194,15 +193,15 @@
     )
 
     base_group.add_argument(
         '--tmpdir', '--tempdir', '--tmp-dir', '--tmp_dir', '--tmp', '--temp', '--temp-dir', '--temp_dir',
         help='Path to the location that will be treated used for temporary files. If none is specified, the TMPDIR \n'
              'environment variable will be used. Can be configured within the `configure` subcommand',
         dest='tmpdir',
-        default=tempfile.gettempdir(),
+        default=None,
     )
 
     base_group.add_argument(
         '--default-resources',
         help='Snakemake resources used as is found at: https://snakemake.readthedocs.io/en/stable/snakefiles/rules.html?highlight=resources#standard-resources \n'
              'NOTE: tmpdir is handled by the `tmpdir` command line parameter. ',
         dest='resources',
@@ -474,42 +473,23 @@
     long_read_group.add_argument(
         '-z', '--longread-type', '--longread_type', '--long_read_type', '--long-read-type',
         help='Whether the sequencing platform and technology for the longreads. \n'
              '"rs" for PacBio RSII, "sq" for PacBio Sequel, "ccs" for PacBio CCS, "hifi" for PacBio HiFi \n'
              'reads, "ont" for Oxford Nanopore and "ont_hq" for Oxford Nanopore high quality reads (Guppy5+ or Q20) \n',
         dest='longread_type',
         default="ont",
-        choices=["ont","ont_hq", "rs", "sq", "ccs", "hifi"],
+        choices=LONG_READ_TYPES,
     )
 
     long_read_group.add_argument(
         '--medaka-model', '--medaka_model',
         help='Medaka model to use for polishing long reads. \n',
         dest='medaka_model',
         default="r941_min_hac_g507",
-        choices=[
-            "r103_fast_g507", "r103_fast_snp_g507", "r103_fast_variant_g507", "r103_hac_g507", "r103_hac_snp_g507",
-            "r103_hac_variant_g507", "r103_min_high_g345", "r103_min_high_g360", "r103_prom_high_g360", "r103_prom_snp_g3210",
-            "r103_prom_variant_g3210", "r103_sup_g507", "r103_sup_snp_g507", "r103_sup_variant_g507", "r1041_e82_260bps_fast_g632",
-            "r1041_e82_260bps_fast_variant_g632", "r1041_e82_260bps_hac_g632", "r1041_e82_260bps_hac_variant_g632", "r1041_e82_260bps_sup_g632",
-            "r1041_e82_260bps_sup_variant_g632", "r1041_e82_400bps_fast_g615", "r1041_e82_400bps_fast_g632",
-            "r1041_e82_400bps_fast_variant_g615", "r1041_e82_400bps_fast_variant_g632", "r1041_e82_400bps_hac_g615",
-            "r1041_e82_400bps_hac_g632", "r1041_e82_400bps_hac_variant_g615", "r1041_e82_400bps_hac_variant_g632", "r1041_e82_400bps_sup_g615",
-            "r1041_e82_400bps_sup_variant_g615", "r104_e81_fast_g5015", "r104_e81_fast_variant_g5015", "r104_e81_hac_g5015",
-            "r104_e81_hac_variant_g5015", "r104_e81_sup_g5015", "r104_e81_sup_g610", "r104_e81_sup_variant_g610", "r10_min_high_g303",
-            "r10_min_high_g340", "r941_e81_fast_g514", "r941_e81_fast_variant_g514", "r941_e81_hac_g514", "r941_e81_hac_variant_g514",
-            "r941_e81_sup_g514", "r941_e81_sup_variant_g514", "r941_min_fast_g303", "r941_min_fast_g507", "r941_min_fast_snp_g507",
-            "r941_min_fast_variant_g507", "r941_min_hac_g507", "r941_min_hac_snp_g507", "r941_min_hac_variant_g507", "r941_min_high_g303",
-            "r941_min_high_g330", "r941_min_high_g340_rle", "r941_min_high_g344", "r941_min_high_g351", "r941_min_high_g360", "r941_min_sup_g507",
-            "r941_min_sup_snp_g507", "r941_min_sup_variant_g507", "r941_prom_fast_g303", "r941_prom_fast_g507", "r941_prom_fast_snp_g507",
-            "r941_prom_fast_variant_g507", "r941_prom_hac_g507", "r941_prom_hac_snp_g507", "r941_prom_hac_variant_g507", "r941_prom_high_g303",
-            "r941_prom_high_g330", "r941_prom_high_g344", "r941_prom_high_g360", "r941_prom_high_g4011", "r941_prom_snp_g303", "r941_prom_snp_g322",
-            "r941_prom_snp_g360", "r941_prom_sup_g507", "r941_prom_sup_snp_g507", "r941_prom_sup_variant_g507", "r941_prom_variant_g303",
-            "r941_prom_variant_g322", "r941_prom_variant_g360", "r941_sup_plant_g610", "r941_sup_plant_variant_g610"
-        ]
+        choices=MEDAKA_MODELS
     )
 
     long_read_group.add_argument(
         '--min-percent-read-identity-long', '--min_percent_read_identity_long',
         help='Minimum percent read identity used by CoverM for long-reads'
              'when calculating genome abundances.',
         dest='long_percent_identity',
@@ -1074,22 +1054,22 @@
                                              parents=[qc_group, assemble_group, binning_group, annotation_group, cluster_group, base_group],
                                              epilog=
                                              '''
                                                       ......:::::: BATCH ::::::......
 
                                              aviary batch -f batch_file.tsv -t 32 -o batch_test
                                              
-                                             An example batch file can be found at: 
+                                             An example batch file can be found at: https://rhysnewell.github.io/aviary/examples
 
                                              ''')
 
     batch_options.add_argument(
         '-f', '--batch_file', '--batch-file',
         help='The tab or comma separated batch file containing the input samples to assemble and/or recover MAGs from. \n'
-             'An example batch file can be found at XXX. The heading line is required. \n'
+             'An example batch file can be found at https://rhysnewell.github.io/aviary/examples. The heading line is required. \n'
              'The number of reads provided to each sample is flexible as is the type of assembly being performed (if any). \n'
              'Multiple reads can be supplied by providing a comma-separated list (surrounded by double quotes \"\" if using a \n'
              'comma separated batch file) within the specific read column.',
         dest="batch_file",
         # nargs=1,
         required=True,
     )
@@ -1105,15 +1085,15 @@
     batch_options.add_argument(
         '--cluster',
         help='Cluster final output of all samples using aviary cluster if possible.',
         dest='cluster',
         type=str2bool,
         nargs='?',
         const=True,
-        default=True
+        default=False
     )
 
     batch_options.add_argument(
         '--cluster-ani-values', '--cluster_ani_values', '--ani-values', '--ani_values',
         help='The range of ANI values to perform clustering and dereplication at during aviary cluster.',
         dest='ani_values',
         nargs='*',
@@ -1132,14 +1112,22 @@
         '--min-percent-read-identity-short', '--min_percent_read_identity_short',
         help='Minimum percent read identity used by CoverM for short-reads \n'
              'when calculating genome abundances.',
         dest='short_percent_identity',
         default='95'
     )
 
+    batch_options.add_argument(
+        '--medaka-model', '--medaka_model',
+        help='Medaka model to use for polishing long reads. \n',
+        dest='medaka_model',
+        default="r941_min_hac_g507",
+        choices=MEDAKA_MODELS
+    )
+
     add_workflow_arg(
         batch_options,
         ['get_bam_indices', 'recover_mags', 'annotate', 'lorikeet'],
         help='Main workflow (snakemake target rule) to run for each sample'
     )
 
     ##########################   ~ configure ~  ###########################
@@ -1286,17 +1274,14 @@
     else:
         process_batch(args, prefix)
 
 def manage_env_vars(args):
     if args.conda_prefix is None:
         args.conda_prefix = Config.get_software_db_path('CONDA_ENV_PATH', '--conda-prefix')
 
-    if args.tmpdir is None:
-        args.tmpdir = Config.get_software_db_path('TMPDIR', '--tmpdir')
-
     try:
         if args.gtdb_path is None:
             args.gtdb_path = Config.get_software_db_path('GTDBTK_DATA_PATH', '--gtdb-path')
         if args.eggnog_db_path is None:
             args.eggnog_db_path = Config.get_software_db_path('EGGNOG_DATA_DIR', '--eggnog-db-path')
         if args.checkm2_db_path is None:
             args.checkm2_db_path = Config.get_software_db_path('CHECKM2DB', '--checkm2-db-path')
```

### Comparing `aviary-genome-0.9.0/aviary/config/config.py` & `aviary-genome-0.9.1/aviary/config/config.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/Snakefile` & `aviary-genome-0.9.1/aviary/modules/Snakefile`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/annotation/annotation.smk` & `aviary-genome-0.9.1/aviary/modules/annotation/annotation.smk`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 rule eggnog:
     input:
         mag_folder = config['mag_directory'],
         # mag_extension = config['mag_extension'],
     params:
         mag_extension = config['mag_extension'],
         eggnog_db = config['eggnog_folder'],
-        tmpdir = config["tmpdir"]
+        tmpdir = config["tmpdir"] if config["tmpdir"] else "$TMPDIR",
     output:
         done = 'data/eggnog/done'
     threads:
         config["max_threads"]
     resources:
         mem_mb = lambda wildcards, attempt: min(int(config["max_memory"])*1024, 512*1024*attempt),
         runtime = lambda wildcards, attempt: 24*60*attempt,
```

### Comparing `aviary-genome-0.9.0/aviary/modules/assembly/assembly.smk` & `aviary-genome-0.9.1/aviary/modules/assembly/assembly.smk`

 * *Files 3% similar despite different names*

```diff
@@ -363,39 +363,16 @@
         long_read_type = config["long_read_type"],
         kmer_sizes = " ".join(config["kmer_sizes"]),
         tmpdir = config["tmpdir"]
     conda:
         "envs/spades.yaml"
     benchmark:
         "benchmarks/spades_assembly.benchmark.txt"
-    shell:
-        """
-        rm -rf data/spades_assembly/tmp; 
-        minimumsize=500000;
-        actualsize=$(stat -c%s data/short_reads.filt.fastq.gz);
-        if [ -d "data/spades_assembly/" ]
-        then
-            spades.py --restart-from last --memory {params.max_memory} -t {threads} -o data/spades_assembly -k {params.kmer_sizes} --tmp-dir {params.tmpdir} > {log} 2>&1 && \
-            cp data/spades_assembly/scaffolds.fasta data/spades_assembly.fasta
-        elif [ $actualsize -ge $minimumsize ]
-        then
-            if [ {params.long_read_type} = "ont" ] || [ {params.long_read_type} = "ont_hq" ]
-            then
-                spades.py --checkpoints all --memory {params.max_memory} --meta --nanopore {input.long_reads} --12 {input.fastq} \
-                -o data/spades_assembly -t {threads}  -k {params.kmer_sizes} --tmp-dir {params.tmpdir} >> {log} 2>&1 && \
-                cp data/spades_assembly/scaffolds.fasta data/spades_assembly.fasta
-            else
-                spades.py --checkpoints all --memory {params.max_memory} --meta --pacbio {input.long_reads} --12 {input.fastq} \
-                -o data/spades_assembly -t {threads}  -k {params.kmer_sizes} --tmp-dir {params.tmpdir} >> {log} 2>&1 && \
-                cp data/spades_assembly/scaffolds.fasta data/spades_assembly.fasta
-            fi
-        else
-            mkdir -p {output.spades_folder} && touch {output.fasta}
-        fi 
-        """
+    script:
+        "scripts/spades_assembly.py"        
 
 
 # Perform short read assembly only with no other steps
 rule assemble_short_reads:
     input:
         fastq = "data/short_reads.fastq.gz"
     output:
@@ -454,22 +431,22 @@
         config["max_threads"]
     resources:
         mem_mb = lambda wildcards, attempt: min(int(config["max_memory"])*1024, 512*1024*attempt),
         runtime = lambda wildcards, attempt: 24*60*attempt,
     log:
         "logs/spades_assembly_coverage.log"
     params:
-         tmpdir = config["tmpdir"]
+         tmpdir = f"TMPDIR={config['tmpdir']}" if config["tmpdir"] else ""
     conda:
          "../../envs/coverm.yaml"
     benchmark:
         "benchmarks/spades_assembly_coverage.benchmark.txt"
     shell:
         """
-        TMPDIR={params.tmpdir} coverm contig -m metabat -t {threads} -r {input.fasta} --interleaved {input.fastq} --bam-file-cache-directory data/cached_bams/ > {output.assembly_cov} 2> {log};
+        {params.tmpdir} coverm contig -m metabat -t {threads} -r {input.fasta} --interleaved {input.fastq} --bam-file-cache-directory data/cached_bams/ > {output.assembly_cov} 2> {log};
         mv data/cached_bams/*.bam {output.bam} && samtools index -@ {threads} {output.bam} 2>> {log}
         """
 
 rule metabat_binning_short:
     input:
          assembly_cov = "data/short_read_assembly.cov",
          fasta = "data/spades_assembly.fasta"
```

### Comparing `aviary-genome-0.9.0/aviary/modules/assembly/isolate.smk` & `aviary-genome-0.9.1/aviary/modules/assembly/isolate.smk`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/assembly/scripts/assemble_pools.py` & `aviary-genome-0.9.1/aviary/modules/assembly/scripts/assemble_pools.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/assembly/scripts/assemble_short_reads.py` & `aviary-genome-0.9.1/aviary/modules/assembly/scripts/assemble_short_reads.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,23 @@
     :param coassemble: coassemble or not
     :param threads: number of threads
     :param tmp_dir: temporary directory
     :param kmer_sizes: list of kmer sizes
     :return:
     '''
 
+    if not tmp_dir:
+        try:
+            tmp_dir = os.environ["TMPDIR"]
+        except KeyError:
+            tmp_dir_arg = ""
+
+    if tmp_dir:
+        tmp_dir_arg = f"--tmp-dir {tmp_dir}"
+
     # deal with read sets i.e. are we coassembling? Which assembler are we using?
     # Non co-assembled reads are handled the same for each assembler
     if read_set1 != 'none':
         if not coassemble or len(read_set1) == 1:
             read_set1 = read_set1[0]
             if read_set2 != 'none':
                 read_set2 = read_set2[0]
@@ -82,26 +91,26 @@
     if reference_filter != 'none':
         read_string = f"--12 data/short_reads.fastq.gz"
 
 
     # Run chosen assembler
     if use_megahit:
         max_memory_in_bytes = max_memory * 1024*1024*1024
-        command = f"megahit {read_string} -t {threads} -m {max_memory_in_bytes} -o data/megahit_assembly --tmp-dir {tmp_dir}"
+        command = f"megahit {read_string} -t {threads} -m {max_memory_in_bytes} -o data/megahit_assembly {tmp_dir_arg}"
 
         with open(log, 'a') as logf:
             logf.write(f"Queueing command {command}\n")
             subprocess.run(command.split(), stdout=logf, stderr=subprocess.STDOUT)
         os.makedirs("data/short_read_assembly", exist_ok=True)
         shutil.copyfile("data/megahit_assembly/final.contigs.fa", "data/short_read_assembly/scaffolds.fasta")
 
     else:
         kmers = " ".join(kmer_sizes)
         command = f"spades.py --memory {max_memory} --meta -t {threads} " \
-                f"-o data/short_read_assembly {read_string} -k {kmers} --tmp-dir {tmp_dir}"
+                f"-o data/short_read_assembly {read_string} -k {kmers} {tmp_dir_arg}"
         with open(log, 'a') as logf:
             logf.write(f"Queueing command {command}\n")
             subprocess.run(command.split(), stdout=logf, stderr=subprocess.STDOUT)
 
 
 if __name__ == '__main__':
     read_set1 = snakemake.config['short_reads_1']
```

### Comparing `aviary-genome-0.9.0/aviary/modules/assembly/scripts/combine_assemblies.py` & `aviary-genome-0.9.1/aviary/modules/assembly/scripts/combine_assemblies.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/assembly/scripts/filter_illumina_assembly.py` & `aviary-genome-0.9.1/aviary/modules/assembly/scripts/filter_illumina_assembly.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/assembly/scripts/generate_pilon_sort.py` & `aviary-genome-0.9.1/aviary/modules/assembly/scripts/generate_pilon_sort.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/assembly/scripts/get_binned_reads.py` & `aviary-genome-0.9.1/aviary/modules/assembly/scripts/get_binned_reads.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/assembly/scripts/polish.py` & `aviary-genome-0.9.1/aviary/modules/assembly/scripts/polish.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/assembly/scripts/pool_reads.py` & `aviary-genome-0.9.1/aviary/modules/assembly/scripts/pool_reads.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/assembly/scripts/run_flye.py` & `aviary-genome-0.9.1/aviary/modules/assembly/scripts/run_flye.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/benchmarking/benchmarking.smk` & `aviary-genome-0.9.1/aviary/modules/benchmarking/benchmarking.smk`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/binning/binning.smk` & `aviary-genome-0.9.1/aviary/modules/binning/binning.smk`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/binning/scripts/das_tool.py` & `aviary-genome-0.9.1/aviary/modules/binning/scripts/das_tool.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/binning/scripts/finalise_recovery.py` & `aviary-genome-0.9.1/aviary/modules/binning/scripts/finalise_recovery.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/binning/scripts/finalise_stats.py` & `aviary-genome-0.9.1/aviary/modules/binning/scripts/finalise_stats.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/binning/scripts/get_abundances.py` & `aviary-genome-0.9.1/aviary/modules/binning/scripts/get_abundances.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/binning/scripts/get_coverage.py` & `aviary-genome-0.9.1/aviary/modules/binning/scripts/get_coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     short_reads_2,
     long_read_type: str,
     input_fasta: str,
     tmpdir: str,
     threads: int,
     log: str,
 ):
-    os.environ["TMPDIR"] = tmpdir
+    if tmpdir: os.environ["TMPDIR"] = tmpdir
+
     if long_reads != "none" and not os.path.exists("data/long_cov.tsv"):
         if long_read_type in ["ont", "ont_hq"]:
             coverm_cmd = f"coverm contig -t {threads} -r {input_fasta} --single {' '.join(long_reads)} -p minimap2-ont -m length trimmed_mean variance --bam-file-cache-directory data/binning_bams/ --discard-unmapped --min-read-percent-identity 0.85 --output-file data/long_cov.tsv".split()
             with open(log, "a") as logf:
                 run(coverm_cmd, stdout=logf, stderr=STDOUT)
 
         elif long_read_type in ["rs", "sq", "ccs", "hifi"]:
```

### Comparing `aviary-genome-0.9.0/aviary/modules/binning/scripts/make_long_cov.py` & `aviary-genome-0.9.1/aviary/modules/binning/scripts/make_long_cov.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/binning/scripts/rosella_refine.py` & `aviary-genome-0.9.1/aviary/modules/binning/scripts/rosella_refine.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/binning/scripts/run_checkm.py` & `aviary-genome-0.9.1/aviary/modules/binning/scripts/run_checkm.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/binning/scripts/write_vamb_bins.py` & `aviary-genome-0.9.1/aviary/modules/binning/scripts/write_vamb_bins.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/cluster/clustering.smk` & `aviary-genome-0.9.1/aviary/modules/cluster/clustering.smk`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/processor.py` & `aviary-genome-0.9.1/aviary/modules/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,25 @@
 
 ###############################################################################
 # System imports
 import sys
 import logging
 import os
 import subprocess
+import copy
 from pathlib import Path
 from glob import glob
 
 # Local imports
 from snakemake import utils
 from snakemake.io import load_configfile
 from ruamel.yaml import YAML  # used for yaml reading with comments
+from aviary import LONG_READ_TYPES
+
+BATCH_HEADER=['sample', 'short_reads_1', 'short_reads_2', 'long_reads', 'long_read_type', 'assembly', 'coassemble']
 
 # Debug
 debug={1:logging.CRITICAL,
        2:logging.ERROR,
        3:logging.WARNING,
        4:logging.INFO,
        5:logging.DEBUG}
@@ -86,15 +90,15 @@
     def __init__(self,
                  args,
                  # conda_prefix=Config.get_software_db_path('CONDA_ENV_PATH', '--conda-prefix'),
                  ):
 
 
         self.conda_prefix = args.conda_prefix
-        self.tmpdir = os.path.abspath(args.tmpdir)
+        self.tmpdir = os.path.abspath(args.tmpdir) if args.tmpdir else None
         self.resources = args.resources
         self.output = os.path.abspath(args.output)
         self.threads = args.max_threads
         self.max_memory = args.max_memory
         self.pplacer_threads = min(int(self.threads), 48)
         self.workflows = args.workflow
         self.request_gpu = args.request_gpu
@@ -438,15 +442,16 @@
         if not os.path.exists(self.config):
             logging.critical(f"config-file not found: {self.config}\n")
             sys.exit(1)
 
         self._validate_config()
 
         cores = max(int(self.threads), cores)
-        os.environ["TMPDIR"] = self.tmpdir
+        if self.tmpdir is not None:
+            os.environ["TMPDIR"] = self.tmpdir
         for workflow in self.workflows:
             cmd = (
                 "snakemake --snakefile {snakefile} --directory {working_dir} "
                 "{jobs} --rerun-incomplete --keep-going {args} {rerun_triggers} "
                 "--configfile {config_file} --nolock "
                 "{profile} {retries} {conda_frontend} {resources} --use-conda {conda_prefix} "
                 "{dryrun} {notemp} "
@@ -464,14 +469,16 @@
                 args=snakemake_args,
                 target_rule=workflow if workflow != "None" else "",
                 conda_prefix="--conda-prefix " + self.conda_prefix,
                 conda_frontend="--conda-frontend " + conda_frontend,
                 resources=f"--resources mem_mb={int(self.max_memory)*1024} {self.resources}" if not dryrun else ""
             )
 
+            logging.debug(f"Command: {cmd}")
+
             if write_to_script is not None:
                 write_to_script.append(cmd)
                 continue
 
             try:
                 logging.info("Executing: %s" % cmd)
                 subprocess.run(cmd.split(), check=True)
@@ -491,28 +498,36 @@
 
     If the user wishes, the results are then clustered.
     '''
     import pandas as pd
 
     logging.info(f"Reading batch file: {args.batch_file}")
 
-    header=0
+    header=None
+    separator=' '
     with open(args.batch_file, mode='r') as check_batch:
         for line in check_batch.readlines():
-            if "sample\tshort_reads_1\tshort_reads_2\tlong_reads\tlong_read_type\tassembly\tcoassemble" in line \
-                or "sample,short_reads_1,short_reads_2,long_reads,long_read_type,assembly,coassemble" in line \
-                or "sample  short_reads_1   short_reads_2   long_reads      long_read_type  assembly        coassemble" in line \
-                or "sample short_reads_1 short_reads_2 long_reads long_read_type assembly coassemble" in line:
-               header=1
-               logging.debug("Inferred header")
-            else:
-                logging.debug("No heading inferred.")
+            line = line.strip()
+            for sep in ['\t', ',', ' ']:
+                separated = line.split(sep)
+                if separated == BATCH_HEADER:
+                    header=0
+                    separator=sep
+                    logging.debug("Inferred header")
+                    break
+                elif len(separated) >= 7:
+                    header=None
+                    separator=sep
+                    logging.debug("Inferred no header")
+                    break
+            if header is None:
+                logging.debug("No header found")
             break
 
-    batch = pd.read_csv(args.batch_file, sep=None, engine='python', skiprows=header)
+    batch = pd.read_csv(args.batch_file, sep=separator, engine='python', names=BATCH_HEADER, header=header)
     if len(batch.columns) != 7:
         logging.critical(f"Batch file contains incorrect number of columns ({len(batch.columns)}). Should contain 7.")
         logging.critical(f"Current columns: {batch.columns}")
         sys.exit()
 
     if args.build:
         try:
@@ -521,60 +536,67 @@
             args.cmds = '--conda-create-envs-only '
 
     if args.use_unicycler:
         args.workflow.insert(0, "combine_assemblies")
 
     try:
         script_file = args.write_script
-        write_to_script = []
     except AttributeError:
         script_file = None
-        write_to_script = None
+    
+    write_to_script = None
+    if script_file is not None:
+        write_to_script = []
 
     runs = []
     args.interleaved = "none" # hacky solution to skip attribute error
     args.coupled = "none"
     for i in range(batch.shape[0]):
         # process the batch line
         sample = check_batch_input(batch.iloc[i, 0], f"sample_{i}", split=False)
         logging.info(f"Processing {sample}")
         s1 = check_batch_input(batch.iloc[i, 1], "none", split=True)
         s2 = check_batch_input(batch.iloc[i, 2], "none", split=True)
         l = check_batch_input(batch.iloc[i, 3], "none", split=True)
         l_type = check_batch_input(batch.iloc[i, 4], "ont", split=False)
+        if l_type not in LONG_READ_TYPES:
+            logging.error(f"Unknown long read type {l_type} specified.")
+            logging.error(f"Valid long read types: {LONG_READ_TYPES}")
+            sys.exit(1)
         assembly = check_batch_input(batch.iloc[i, 5], None, split=False)
         coassemble = check_batch_input(batch.iloc[i, 6], False, split=False)
-
+        
+        new_args = copy.deepcopy(args)
         # update the value of args
-        args.output = f"{prefix}/{sample}"
-        runs.append(args.output)
-        args.pe1 = s1
-        args.pe2 = s2
-
-        args.longreads = l
-        args.longread_type = l_type
-        args.assembly = assembly
-        args.coassemble = coassemble
+        new_args.output = f"{prefix}/{sample}"
+        runs.append(new_args.output)
+        new_args.pe1 = s1
+        new_args.pe2 = s2
+
+        new_args.longreads = l
+        new_args.longread_type = l_type
+        new_args.assembly = assembly
+        new_args.coassemble = coassemble
 
         # ensure output folder exists
-        if not os.path.exists(args.output):
-            os.makedirs(args.output)
+        if not os.path.exists(new_args.output):
+            os.makedirs(new_args.output)
 
         # setup processor for this line
-        processor = Processor(args)
+        processor = Processor(new_args)
         processor.make_config()
 
-        processor.run_workflow(cores=int(args.n_cores),
-                               dryrun=args.dryrun,
-                               clean=args.clean,
-                               conda_frontend=args.conda_frontend,
-                               snakemake_args=args.cmds,
-                               rerun_triggers=args.rerun_triggers,
-                               profile=args.snakemake_profile,
-                               cluster_retries=args.cluster_retries,
+        processor.run_workflow(cores=int(new_args.n_cores),
+                               dryrun=new_args.dryrun,
+                               clean=new_args.clean,
+                               conda_frontend=new_args.conda_frontend,
+                               snakemake_args=new_args.cmds,
+                               rerun_triggers=new_args.rerun_triggers,
+                               profile=new_args.snakemake_profile,
+                               cluster_retries=new_args.cluster_retries,
                                write_to_script=write_to_script)
 
     if args.cluster:
         logging.info(f"Beginning clustering of {len(runs)} previous Aviary runs with ANI values: {args.ani_values}...")
 
         for ani in args.ani_values:
             args.previous_runs = runs
```

### Comparing `aviary-genome-0.9.0/aviary/modules/quality_control/qc.smk` & `aviary-genome-0.9.1/aviary/modules/quality_control/qc.smk`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/quality_control/scripts/filter_read_list.py` & `aviary-genome-0.9.1/aviary/modules/quality_control/scripts/filter_read_list.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/quality_control/scripts/fraction_recovered.py` & `aviary-genome-0.9.1/aviary/modules/quality_control/scripts/fraction_recovered.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/quality_control/scripts/qc_long_reads.py` & `aviary-genome-0.9.1/aviary/modules/quality_control/scripts/qc_long_reads.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/quality_control/scripts/qc_short_reads.py` & `aviary-genome-0.9.1/aviary/modules/quality_control/scripts/qc_short_reads.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/quality_control/scripts/run_fastqc.py` & `aviary-genome-0.9.1/aviary/modules/quality_control/scripts/run_fastqc.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/strain_analysis/scripts/run_lorikeet.py` & `aviary-genome-0.9.1/aviary/modules/strain_analysis/scripts/run_lorikeet.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/strain_analysis/strain_analysis.smk` & `aviary-genome-0.9.1/aviary/modules/strain_analysis/strain_analysis.smk`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,13 @@
     output:
          output_directory = directory("strain_diversity/")
     conda:
         "envs/lorikeet.yaml"
     params:
         mag_extension = config['mag_extension'],
         parallel_genomes = 8,
-        tmpdir = config['tmpdir']
     resources:
         mem_mb=int(config["max_memory"])*512
     threads:
         config["max_threads"]
     script:
         "scripts/run_lorikeet.py"
```

### Comparing `aviary-genome-0.9.0/aviary/modules/template_config.yaml` & `aviary-genome-0.9.1/aviary/modules/template_config.yaml`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/modules/viral_analysis/viral_analysis.smk` & `aviary-genome-0.9.1/aviary/modules/viral_analysis/viral_analysis.smk`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/scripts/create_aviary_webpage.py` & `aviary-genome-0.9.1/aviary/scripts/create_aviary_webpage.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/scripts/process_batch.py` & `aviary-genome-0.9.1/aviary/scripts/process_batch.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/scripts/process_viral_batch.py` & `aviary-genome-0.9.1/aviary/scripts/process_viral_batch.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/scripts/singlem_appraise.py` & `aviary-genome-0.9.1/aviary/scripts/singlem_appraise.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary/scripts/singlem_reads.py` & `aviary-genome-0.9.1/aviary/scripts/singlem_reads.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/aviary_genome.egg-info/PKG-INFO` & `aviary-genome-0.9.1/aviary_genome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aviary-genome
-Version: 0.9.0
+Version: 0.9.1
 Summary: aviary - metagenomics pipeline using long and short reads
 Home-page: https://github.com/rhysnewell/aviary
 Author: Rhys Newell
 Author-email: rhys.newell94@gmail.com
 License: GPL-3.0
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
```

### Comparing `aviary-genome-0.9.0/aviary_genome.egg-info/SOURCES.txt` & `aviary-genome-0.9.1/aviary_genome.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 aviary/modules/assembly/scripts/combine_assemblies.py
 aviary/modules/assembly/scripts/filter_illumina_assembly.py
 aviary/modules/assembly/scripts/generate_pilon_sort.py
 aviary/modules/assembly/scripts/get_binned_reads.py
 aviary/modules/assembly/scripts/polish.py
 aviary/modules/assembly/scripts/pool_reads.py
 aviary/modules/assembly/scripts/run_flye.py
+aviary/modules/assembly/scripts/spades_assembly.py
 aviary/modules/benchmarking/__init__.py
 aviary/modules/benchmarking/benchmarking.smk
 aviary/modules/benchmarking/envs/__init__.py
 aviary/modules/benchmarking/envs/magpurify.yaml
 aviary/modules/benchmarking/scripts/__init__.py
 aviary/modules/binning/__init__.py
 aviary/modules/binning/binning.smk
```

### Comparing `aviary-genome-0.9.0/setup.py` & `aviary-genome-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/test/test_assemble.py` & `aviary-genome-0.9.1/test/test_assemble.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/test/test_integration.py` & `aviary-genome-0.9.1/test/test_integration.py`

 * *Files 19% similar despite different names*

```diff
@@ -158,15 +158,14 @@
 
     def test_short_read_recovery_queue_submission(self):
         output_dir = os.path.join("example", "test_short_read_recovery_queue_submission")
         self.setup_output_dir(output_dir)
 
         cmd = (
             f"aviary recover "
-            f"--output {output_dir} "
             f"-o {output_dir}/aviary_out "
             f"-1 {data}/wgsim.1.fq.gz "
             f"-2 {data}/wgsim.2.fq.gz "
             f"--conda-prefix {path_to_conda} "
             f"-n 32 -t 32 "
             f"--snakemake-profile mqsub --cluster-retries 3 "
         )
@@ -176,10 +175,45 @@
 
         bin_info_path = f"{output_dir}/aviary_out/bins/bin_info.tsv"
         self.assertTrue(os.path.isfile(bin_info_path))
         with open(bin_info_path) as f:
             num_lines = sum(1 for _ in f)
         self.assertEqual(num_lines, 3)
 
+    def test_batch_recovery(self):
+        output_dir = os.path.join("example", "test_batch_recovery")
+        self.setup_output_dir(output_dir)
+        cmd = (
+            f"aviary batch "
+            f"-o {output_dir}/aviary_out "
+            f"-f {data}/example_batch.tsv "
+            f"--conda-prefix {path_to_conda} "
+            f"--skip-binners rosella vamb metabat "
+            f"--skip-qc "
+            f"--refinery-max-iterations 0 "
+            f"--min-read-size 10 --min-mean-q 1 "
+            f"-n 32 -t 32 "
+        )
+        subprocess.run(cmd, shell=True, check=True)
+
+        self.assertTrue(os.path.isfile(f"{output_dir}/aviary_out/sample_1/data/final_contigs.fasta"))
+        self.assertTrue(os.path.isfile(f"{output_dir}/aviary_out/sample_2/data/final_contigs.fasta"))
+
+        bin_info_path_1 = f"{output_dir}/aviary_out/sample_1/bins/bin_info.tsv"
+        bin_info_path_2 = f"{output_dir}/aviary_out/sample_2/bins/bin_info.tsv"
+        self.assertTrue(os.path.isfile(bin_info_path_1))
+        self.assertTrue(os.path.isfile(bin_info_path_2))
+        with open(bin_info_path_1) as f:
+            num_lines = sum(1 for _ in f)
+        self.assertEqual(num_lines, 3)
+
+        self.assertTrue(os.path.isdir(f"{output_dir}/aviary_out/aviary_cluster_ani_0.95"))
+        self.assertTrue(os.path.isdir(f"{output_dir}/aviary_out/aviary_cluster_ani_0.97"))
+        self.assertTrue(os.path.isdir(f"{output_dir}/aviary_out/aviary_cluster_ani_0.99"))
+
+        self.assertTrue(os.path.isdir(f"{output_dir}/aviary_out/aviary_cluster_ani_0.95/pangenomes"))
+        self.assertTrue(os.path.isdir(f"{output_dir}/aviary_out/aviary_cluster_ani_0.97/pangenomes"))
+        self.assertTrue(os.path.isdir(f"{output_dir}/aviary_out/aviary_cluster_ani_0.99/pangenomes"))
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aviary-genome-0.9.0/test/test_recover.py` & `aviary-genome-0.9.1/test/test_recover.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.9.0/test/test_run_checkm.py` & `aviary-genome-0.9.1/test/test_run_checkm.py`

 * *Files identical despite different names*

