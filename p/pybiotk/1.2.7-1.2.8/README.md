# Comparing `tmp/pybiotk-1.2.7.tar.gz` & `tmp/pybiotk-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybiotk-1.2.7.tar", last modified: Sat Dec 23 08:16:54 2023, max compression
+gzip compressed data, was "pybiotk-1.2.8.tar", last modified: Tue May 14 02:36:59 2024, max compression
```

## Comparing `pybiotk-1.2.7.tar` & `pybiotk-1.2.8.tar`

### file list

```diff
@@ -1,139 +1,140 @@
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:54.000000 pybiotk-1.2.7/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      590 2023-07-28 08:43:54.000000 pybiotk-1.2.7/.coveragerc
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      583 2023-07-28 08:43:54.000000 pybiotk-1.2.7/.gitignore
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      490 2023-07-28 08:43:54.000000 pybiotk-1.2.7/.readthedocs.yml
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       77 2023-07-28 08:43:54.000000 pybiotk-1.2.7/AUTHORS.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      128 2023-07-28 08:43:54.000000 pybiotk-1.2.7/CHANGELOG.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    13815 2023-07-28 08:43:54.000000 pybiotk-1.2.7/CONTRIBUTING.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1079 2023-07-28 08:43:54.000000 pybiotk-1.2.7/LICENSE.txt
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3643 2023-12-23 08:16:46.000000 pybiotk-1.2.7/PKG-INFO
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2932 2023-07-28 08:43:54.000000 pybiotk-1.2.7/README.md
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4004 2023-07-28 08:43:54.000000 pybiotk-1.2.7/README.rst
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:45.000000 pybiotk-1.2.7/docs/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1154 2023-07-28 08:43:54.000000 pybiotk-1.2.7/docs/Makefile
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:45.000000 pybiotk-1.2.7/docs/_static/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       18 2023-07-28 08:43:54.000000 pybiotk-1.2.7/docs/_static/.gitignore
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       41 2023-07-28 08:43:54.000000 pybiotk-1.2.7/docs/authors.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       43 2023-07-28 08:43:54.000000 pybiotk-1.2.7/docs/changelog.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9734 2023-07-28 08:43:54.000000 pybiotk-1.2.7/docs/conf.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       33 2023-07-28 08:43:54.000000 pybiotk-1.2.7/docs/contributing.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2313 2023-07-28 08:43:54.000000 pybiotk-1.2.7/docs/index.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       67 2023-07-28 08:43:54.000000 pybiotk-1.2.7/docs/license.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       39 2023-07-28 08:43:54.000000 pybiotk-1.2.7/docs/readme.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      122 2023-07-28 08:43:54.000000 pybiotk-1.2.7/docs/requirements.txt
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      415 2023-07-28 09:50:57.000000 pybiotk-1.2.7/pyproject.toml
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:45.000000 pybiotk-1.2.7/rscripts/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7058 2023-09-19 12:18:57.000000 pybiotk-1.2.7/rscripts/diff_expr_DESeq2.R
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     5704 2023-09-19 12:18:57.000000 pybiotk-1.2.7/rscripts/diff_expr_edgeR.R
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    16592 2023-11-01 12:39:27.000000 pybiotk-1.2.7/rscripts/diff_expr_plot.R
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3017 2023-09-19 12:18:57.000000 pybiotk-1.2.7/rscripts/peak_anno.R
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3117 2023-09-22 02:34:18.000000 pybiotk-1.2.7/rscripts/plot_FRiPs.R
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2517 2023-09-19 12:18:57.000000 pybiotk-1.2.7/rscripts/plot_bar.R
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     8528 2023-09-22 02:29:27.000000 pybiotk-1.2.7/rscripts/plot_chip_summary.R
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3661 2023-09-19 12:18:57.000000 pybiotk-1.2.7/rscripts/plot_corr.R
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3921 2023-09-19 12:18:57.000000 pybiotk-1.2.7/rscripts/plot_deeptools_fragmentsize.R
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1918 2023-09-19 12:18:57.000000 pybiotk-1.2.7/rscripts/plot_hist.R
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4114 2023-09-19 12:18:57.000000 pybiotk-1.2.7/rscripts/plot_peak_width.R
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3086 2023-09-19 12:18:57.000000 pybiotk-1.2.7/rscripts/plot_rep_cor.R
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2079 2023-09-19 12:18:57.000000 pybiotk-1.2.7/rscripts/plot_venn.R
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:45.000000 pybiotk-1.2.7/scripts/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      196 2023-09-19 12:18:57.000000 pybiotk-1.2.7/scripts/fasta_len.sh
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      147 2023-09-19 12:18:57.000000 pybiotk-1.2.7/scripts/fasta_u2t.sh
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      206 2023-09-19 12:18:57.000000 pybiotk-1.2.7/scripts/fastq_len.sh
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      165 2023-09-19 12:18:57.000000 pybiotk-1.2.7/scripts/get_chrom_length.sh
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1010 2023-09-19 12:18:57.000000 pybiotk-1.2.7/scripts/gtfparser.sh
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      555 2023-09-19 12:18:57.000000 pybiotk-1.2.7/scripts/merge_subseq.sh
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1296 2023-09-19 12:18:57.000000 pybiotk-1.2.7/scripts/remove_duplicates.sh
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2444 2023-12-23 08:16:46.000000 pybiotk-1.2.7/setup.cfg
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1222 2023-07-28 08:43:54.000000 pybiotk-1.2.7/setup.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:45.000000 pybiotk-1.2.7/src/
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:45.000000 pybiotk-1.2.7/src/bx/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7429 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/bx/binBits.c
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      830 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/bx/binBits.h
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     6253 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/bx/bits.c
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1814 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/bx/bits.h
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9273 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/bx/bitset.pyx
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     8110 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/bx/cluster.c
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      905 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/bx/cluster.h
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3795 2023-07-28 09:50:55.000000 pybiotk-1.2.7/src/bx/cluster.pyx
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1508 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/bx/common.c
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      639 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/bx/common.h
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    17210 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/bx/intersection.pyx
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:45.000000 pybiotk-1.2.7/src/pybiotk/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        0 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/__init__.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:45.000000 pybiotk-1.2.7/src/pybiotk/annodb/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       99 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/annodb/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9510 2023-12-23 08:16:00.000000 pybiotk-1.2.7/src/pybiotk/annodb/anno.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    10121 2023-12-23 08:16:00.000000 pybiotk-1.2.7/src/pybiotk/annodb/gene.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    12502 2023-09-19 12:18:57.000000 pybiotk-1.2.7/src/pybiotk/annodb/merged_transcript.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7658 2023-12-23 08:16:00.000000 pybiotk-1.2.7/src/pybiotk/annodb/transcript.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:45.000000 pybiotk-1.2.7/src/pybiotk/convert/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        0 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/convert/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3813 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/convert/bam2fastx.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1149 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/convert/bampe_order_by_name.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1697 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/convert/bed2bedgraph.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      672 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/convert/fa2fastq.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      709 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/convert/fq2fasta.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4691 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/convert/gtf2bed.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:53.000000 pybiotk-1.2.7/src/pybiotk/data/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        0 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/data/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    11177 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/data/hg38.chrom.sizes
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2410 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/data/mm10.chrom.sizes
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:53.000000 pybiotk-1.2.7/src/pybiotk/intervals/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       79 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/intervals/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4842 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/intervals/grange.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2441 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/intervals/merge_bed3.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2642 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/intervals/merge_intervals.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:53.000000 pybiotk-1.2.7/src/pybiotk/io/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      451 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/io/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    10840 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/io/bam.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     6230 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/io/bed.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7678 2023-10-20 09:32:35.000000 pybiotk-1.2.7/src/pybiotk/io/bw.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4795 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/io/fasta.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4505 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/io/fastq.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    19645 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/io/gtf.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:53.000000 pybiotk-1.2.7/src/pybiotk/string/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       44 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/string/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      946 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/string/motif.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      714 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/string/sequence.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:54.000000 pybiotk-1.2.7/src/pybiotk/utils/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       21 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2525 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/bam_random.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2409 2023-12-13 10:16:11.000000 pybiotk-1.2.7/src/pybiotk/utils/ercc_parser.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1230 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/fasta_filter.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     5292 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/fastq_join.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3985 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/fastq_uniq.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1708 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/fastx_rename.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4182 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/fragment_size.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9967 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/genomefetcher.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2936 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/gtf_filter.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     5805 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/merge_row.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2391 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/merge_subseq.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3664 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/normalize.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    11802 2023-12-23 08:16:00.000000 pybiotk-1.2.7/src/pybiotk/utils/pyanno.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3284 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/read_tables.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2234 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/reference_count.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1620 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/reverse_fastx.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3114 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/rmats_filter.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2778 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/seq_random.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4093 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/subseq_analysis.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    14283 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/pybiotk/utils/summary_log.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9620 2023-11-08 08:37:35.000000 pybiotk-1.2.7/src/pybiotk/utils/utils.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:45.000000 pybiotk-1.2.7/src/pybiotk.egg-info/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3643 2023-12-23 08:16:44.000000 pybiotk-1.2.7/src/pybiotk.egg-info/PKG-INFO
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3026 2023-12-23 08:12:22.000000 pybiotk-1.2.7/src/pybiotk.egg-info/SOURCES.txt
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        1 2023-12-23 08:12:22.000000 pybiotk-1.2.7/src/pybiotk.egg-info/dependency_links.txt
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1186 2023-12-23 08:12:22.000000 pybiotk-1.2.7/src/pybiotk.egg-info/entry_points.txt
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        1 2023-07-28 09:09:57.000000 pybiotk-1.2.7/src/pybiotk.egg-info/not-zip-safe
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       93 2023-12-23 08:12:22.000000 pybiotk-1.2.7/src/pybiotk.egg-info/requires.txt
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       15 2023-12-23 08:12:22.000000 pybiotk-1.2.7/src/pybiotk.egg-info/top_level.txt
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:54.000000 pybiotk-1.2.7/src/stream/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       20 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/stream/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    10873 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/stream/pipe.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7886 2023-07-28 08:43:54.000000 pybiotk-1.2.7/src/stream/stream.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:54.000000 pybiotk-1.2.7/tests/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        0 2023-07-28 08:43:54.000000 pybiotk-1.2.7/tests/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      132 2023-07-28 08:43:54.000000 pybiotk-1.2.7/tests/conftest.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-12-23 08:16:54.000000 pybiotk-1.2.7/tests/test_stream/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      195 2023-07-28 08:43:54.000000 pybiotk-1.2.7/tests/test_stream/test_pipe.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2575 2023-07-28 08:43:54.000000 pybiotk-1.2.7/tox.ini
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.639639 pybiotk-1.2.8/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      590 2024-05-06 03:47:28.000000 pybiotk-1.2.8/.coveragerc
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      583 2024-05-06 03:47:28.000000 pybiotk-1.2.8/.gitignore
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      490 2024-05-06 03:47:28.000000 pybiotk-1.2.8/.readthedocs.yml
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       77 2024-05-06 03:47:28.000000 pybiotk-1.2.8/AUTHORS.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      128 2024-05-06 03:47:28.000000 pybiotk-1.2.8/CHANGELOG.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    13815 2024-05-06 03:47:28.000000 pybiotk-1.2.8/CONTRIBUTING.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1079 2024-05-06 03:47:28.000000 pybiotk-1.2.8/LICENSE.txt
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3643 2024-05-14 02:36:59.639639 pybiotk-1.2.8/PKG-INFO
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2932 2024-05-06 03:47:28.000000 pybiotk-1.2.8/README.md
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4004 2024-05-06 03:47:28.000000 pybiotk-1.2.8/README.rst
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.619639 pybiotk-1.2.8/docs/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1154 2024-05-06 03:47:28.000000 pybiotk-1.2.8/docs/Makefile
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.619639 pybiotk-1.2.8/docs/_static/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       18 2024-05-06 03:47:28.000000 pybiotk-1.2.8/docs/_static/.gitignore
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       41 2024-05-06 03:47:28.000000 pybiotk-1.2.8/docs/authors.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       43 2024-05-06 03:47:28.000000 pybiotk-1.2.8/docs/changelog.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     9734 2024-05-06 03:47:28.000000 pybiotk-1.2.8/docs/conf.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       33 2024-05-06 03:47:28.000000 pybiotk-1.2.8/docs/contributing.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2313 2024-05-06 03:47:28.000000 pybiotk-1.2.8/docs/index.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       67 2024-05-06 03:47:28.000000 pybiotk-1.2.8/docs/license.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       39 2024-05-06 03:47:28.000000 pybiotk-1.2.8/docs/readme.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      122 2024-05-06 03:47:28.000000 pybiotk-1.2.8/docs/requirements.txt
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      399 2024-05-08 07:32:50.000000 pybiotk-1.2.8/pyproject.toml
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.619639 pybiotk-1.2.8/rscripts/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     7058 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/diff_expr_DESeq2.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     5704 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/diff_expr_edgeR.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    16592 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/diff_expr_plot.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3017 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/peak_anno.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3117 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/plot_FRiPs.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2517 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/plot_bar.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     8528 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/plot_chip_summary.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3661 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/plot_corr.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3921 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/plot_deeptools_fragmentsize.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1918 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/plot_hist.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4114 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/plot_peak_width.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3086 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/plot_rep_cor.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2079 2024-05-06 03:47:28.000000 pybiotk-1.2.8/rscripts/plot_venn.R
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.619639 pybiotk-1.2.8/scripts/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      196 2024-05-06 03:47:28.000000 pybiotk-1.2.8/scripts/fasta_len.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      147 2024-05-06 03:47:28.000000 pybiotk-1.2.8/scripts/fasta_u2t.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      206 2024-05-06 03:47:28.000000 pybiotk-1.2.8/scripts/fastq_len.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      165 2024-05-06 03:47:28.000000 pybiotk-1.2.8/scripts/get_chrom_length.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1010 2024-05-06 03:47:28.000000 pybiotk-1.2.8/scripts/gtfparser.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      555 2024-05-06 03:47:28.000000 pybiotk-1.2.8/scripts/merge_subseq.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1296 2024-05-06 03:47:28.000000 pybiotk-1.2.8/scripts/remove_duplicates.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2493 2024-05-14 02:36:59.639639 pybiotk-1.2.8/setup.cfg
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1202 2024-05-08 07:29:41.000000 pybiotk-1.2.8/setup.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.609639 pybiotk-1.2.8/src/
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.619639 pybiotk-1.2.8/src/bx/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     7429 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/bx/binBits.c
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      830 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/bx/binBits.h
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     6253 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/bx/bits.c
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1814 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/bx/bits.h
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     9273 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/bx/bitset.pyx
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     8110 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/bx/cluster.c
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      905 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/bx/cluster.h
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3795 2024-05-08 07:21:08.000000 pybiotk-1.2.8/src/bx/cluster.pyx
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1508 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/bx/common.c
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      639 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/bx/common.h
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    17210 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/bx/intersection.pyx
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.619639 pybiotk-1.2.8/src/pybiotk/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)        0 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/__init__.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.619639 pybiotk-1.2.8/src/pybiotk/annodb/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       99 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/annodb/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     9655 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/annodb/anno.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    10121 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/annodb/gene.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    13634 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/annodb/merged_transcript.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     7658 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/annodb/transcript.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.629639 pybiotk-1.2.8/src/pybiotk/convert/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)        0 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/convert/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3813 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/convert/bam2fastx.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1149 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/convert/bampe_order_by_name.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1697 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/convert/bed2bedgraph.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      672 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/convert/fa2fastq.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      709 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/convert/fq2fasta.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4691 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/convert/gtf2bed.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.629639 pybiotk-1.2.8/src/pybiotk/data/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)        0 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/data/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    11177 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/data/hg38.chrom.sizes
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2410 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/data/mm10.chrom.sizes
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.629639 pybiotk-1.2.8/src/pybiotk/intervals/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       79 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/intervals/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4842 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/intervals/grange.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2441 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/intervals/merge_bed3.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2642 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/intervals/merge_intervals.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.629639 pybiotk-1.2.8/src/pybiotk/io/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      451 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/io/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    11443 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/io/bam.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     6230 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/io/bed.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     7678 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/io/bw.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4795 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/io/fasta.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4505 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/io/fastq.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    19645 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/io/gtf.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.629639 pybiotk-1.2.8/src/pybiotk/string/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       44 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/string/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      946 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/string/motif.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      714 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/string/sequence.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.639639 pybiotk-1.2.8/src/pybiotk/utils/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       21 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2525 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/bam_random.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3706 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/bigwigfetcher.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2409 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/ercc_parser.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1230 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/fasta_filter.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     5292 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/fastq_join.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3985 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/fastq_uniq.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1708 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/fastx_rename.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4182 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/fragment_size.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     9967 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/genomefetcher.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2936 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/gtf_filter.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     5805 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/merge_row.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2391 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/merge_subseq.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3664 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/normalize.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    11802 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/pyanno.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3284 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/read_tables.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2234 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/reference_count.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1620 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/reverse_fastx.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3114 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/rmats_filter.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2778 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/seq_random.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4093 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/subseq_analysis.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    14283 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/pybiotk/utils/summary_log.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     9614 2024-05-08 03:51:21.000000 pybiotk-1.2.8/src/pybiotk/utils/utils.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.639639 pybiotk-1.2.8/src/pybiotk.egg-info/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3643 2024-05-14 02:36:59.000000 pybiotk-1.2.8/src/pybiotk.egg-info/PKG-INFO
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3061 2024-05-14 02:36:59.000000 pybiotk-1.2.8/src/pybiotk.egg-info/SOURCES.txt
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)        1 2024-05-14 02:36:59.000000 pybiotk-1.2.8/src/pybiotk.egg-info/dependency_links.txt
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1234 2024-05-14 02:36:59.000000 pybiotk-1.2.8/src/pybiotk.egg-info/entry_points.txt
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)        1 2024-05-08 07:29:57.000000 pybiotk-1.2.8/src/pybiotk.egg-info/not-zip-safe
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       93 2024-05-14 02:36:59.000000 pybiotk-1.2.8/src/pybiotk.egg-info/requires.txt
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       15 2024-05-14 02:36:59.000000 pybiotk-1.2.8/src/pybiotk.egg-info/top_level.txt
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.639639 pybiotk-1.2.8/src/stream/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       20 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/stream/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    10873 2024-05-07 08:30:22.000000 pybiotk-1.2.8/src/stream/pipe.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     7886 2024-05-06 03:47:28.000000 pybiotk-1.2.8/src/stream/stream.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.639639 pybiotk-1.2.8/tests/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)        0 2024-05-06 03:47:28.000000 pybiotk-1.2.8/tests/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      132 2024-05-06 03:47:28.000000 pybiotk-1.2.8/tests/conftest.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2024-05-14 02:36:59.639639 pybiotk-1.2.8/tests/test_stream/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1471 2024-05-08 06:58:29.000000 pybiotk-1.2.8/tests/test_stream/test_pipe.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2575 2024-05-06 03:47:28.000000 pybiotk-1.2.8/tox.ini
```

### Comparing `pybiotk-1.2.7/.coveragerc` & `pybiotk-1.2.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/.gitignore` & `pybiotk-1.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/CONTRIBUTING.rst` & `pybiotk-1.2.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/LICENSE.txt` & `pybiotk-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/PKG-INFO` & `pybiotk-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybiotk
-Version: 1.2.7
+Version: 1.2.8
 Summary: pybiotk: A python toolkit for bioinformatics analysis.
 Home-page: https://github.com/liqiming-whu/pybiotk
 Author: liqiming_whu
 Author-email: liqiming@whu.edu.cn
 License: MIT
 Project-URL: Documentation, https://github.com/liqiming-whu/pybiotk
 Platform: any
```

### Comparing `pybiotk-1.2.7/README.md` & `pybiotk-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/README.rst` & `pybiotk-1.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/docs/Makefile` & `pybiotk-1.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/docs/conf.py` & `pybiotk-1.2.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/docs/index.rst` & `pybiotk-1.2.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/diff_expr_DESeq2.R` & `pybiotk-1.2.8/rscripts/diff_expr_DESeq2.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/diff_expr_edgeR.R` & `pybiotk-1.2.8/rscripts/diff_expr_edgeR.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/diff_expr_plot.R` & `pybiotk-1.2.8/rscripts/diff_expr_plot.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/peak_anno.R` & `pybiotk-1.2.8/rscripts/peak_anno.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/plot_FRiPs.R` & `pybiotk-1.2.8/rscripts/plot_FRiPs.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/plot_bar.R` & `pybiotk-1.2.8/rscripts/plot_bar.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/plot_chip_summary.R` & `pybiotk-1.2.8/rscripts/plot_chip_summary.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/plot_corr.R` & `pybiotk-1.2.8/rscripts/plot_corr.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/plot_deeptools_fragmentsize.R` & `pybiotk-1.2.8/rscripts/plot_deeptools_fragmentsize.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/plot_hist.R` & `pybiotk-1.2.8/rscripts/plot_hist.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/plot_peak_width.R` & `pybiotk-1.2.8/rscripts/plot_peak_width.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/plot_rep_cor.R` & `pybiotk-1.2.8/rscripts/plot_rep_cor.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/rscripts/plot_venn.R` & `pybiotk-1.2.8/rscripts/plot_venn.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/scripts/gtfparser.sh` & `pybiotk-1.2.8/scripts/gtfparser.sh`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/scripts/merge_subseq.sh` & `pybiotk-1.2.8/scripts/merge_subseq.sh`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/scripts/remove_duplicates.sh` & `pybiotk-1.2.8/scripts/remove_duplicates.sh`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/setup.cfg` & `pybiotk-1.2.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pybiotk
-version = 1.2.7
+version = 1.2.8
 description = pybiotk: A python toolkit for bioinformatics analysis.
 author = liqiming_whu
 author_email = liqiming@whu.edu.cn
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -54,14 +54,15 @@
 	bam_random = pybiotk.utils.bam_random:run
 	gtf_filter = pybiotk.utils.gtf_filter:run
 	fasta_filter = pybiotk.utils.fasta_filter:run
 	fastq_uniq = pybiotk.utils.fastq_uniq:run
 	fastq_join = pybiotk.utils.fastq_join:run
 	fastx_rename = pybiotk.utils.fastx_rename:run
 	genomefetcher = pybiotk.utils.genomefetcher:run
+	bigwigfetcher = pybiotk.utils.bigwigfetcher:run
 	reverse_fastx = pybiotk.utils.reverse_fastx:run
 	seq_random = pybiotk.utils.seq_random:run
 	merge_row = pybiotk.utils.merge_row:run
 	read_tables = pybiotk.utils.read_tables:run
 	rmats_filter = pybiotk.utils.rmats_filter:run
 	count_normalize = pybiotk.utils.normalize:run
 	reference_count = pybiotk.utils.reference_count:run
```

### Comparing `pybiotk-1.2.7/setup.py` & `pybiotk-1.2.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, Extension
 from Cython.Build import cythonize
 from glob import glob
 
 
 ext_modules = [
     Extension("pybiotk.bx.bitset", ["src/bx/bitset.pyx", "src/bx/binBits.c", "src/bx/bits.c", "src/bx/common.c"]),
-    Extension("pybiotk.bx.cluster", ["src/bx/cluster.c", "src/bx/cluster.pyx"]),
+    Extension("pybiotk.bx.cluster", ["src/bx/cluster.pyx"]),
     Extension("pybiotk.bx.intersection", ["src/bx/intersection.pyx"])
 ]
 
 if __name__ == "__main__":
     try:
         setup(use_scm_version={"version_scheme": "no-guess-dev", "local_scheme": "no-local-version"},
               ext_modules=cythonize(ext_modules, build_dir="build"),
```

### Comparing `pybiotk-1.2.7/src/bx/binBits.c` & `pybiotk-1.2.8/src/bx/binBits.c`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/bx/binBits.h` & `pybiotk-1.2.8/src/bx/binBits.h`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/bx/bits.c` & `pybiotk-1.2.8/src/bx/bits.c`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/bx/bits.h` & `pybiotk-1.2.8/src/bx/bits.h`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/bx/bitset.pyx` & `pybiotk-1.2.8/src/bx/bitset.pyx`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/bx/cluster.c` & `pybiotk-1.2.8/src/bx/cluster.c`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/bx/cluster.h` & `pybiotk-1.2.8/src/bx/cluster.h`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/bx/cluster.pyx` & `pybiotk-1.2.8/src/bx/cluster.pyx`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/bx/common.c` & `pybiotk-1.2.8/src/bx/common.c`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/bx/common.h` & `pybiotk-1.2.8/src/bx/common.h`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/bx/intersection.pyx` & `pybiotk-1.2.8/src/bx/intersection.pyx`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/annodb/anno.py` & `pybiotk-1.2.8/src/pybiotk/annodb/anno.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,20 @@
     @abstractmethod
     def tss_region(self, region: Tuple[int, int] = (-1000, 1000)) -> Tuple[int, int]: ...
 
     @abstractmethod
     def downstream(self, down: int = 3000) -> Tuple[int, int]: ...
 
     @abstractmethod
+    def start_condon(self) -> Tuple[int, int]:...
+    
+    @abstractmethod
+    def stop_condon(self) -> Tuple[int, int]:...
+
+    @abstractmethod
     def cds_exons(self) -> List[Tuple[int, int]]: ...
 
     @abstractmethod
     def utr5_exons(self) -> List[Tuple[int, int]]: ...
 
     @abstractmethod
     def utr3_exons(self) -> List[Tuple[int, int]]: ...
```

### Comparing `pybiotk-1.2.7/src/pybiotk/annodb/gene.py` & `pybiotk-1.2.8/src/pybiotk/annodb/gene.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/annodb/merged_transcript.py` & `pybiotk-1.2.8/src/pybiotk/annodb/merged_transcript.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,16 @@
         self.cds_starts = list(cds_starts)
         self.cds_ends = list(cds_ends)
         self._exons = list(exons)
         self._introns = None
         self._cds_exons = None
         self._utr5_exons = None
         self._utr3_exons = None
+        self._start_condon = None
+        self._stop_condon = None
         self.count = count
         self.before = int(before) if before is not None else before
         self.after = int(after) if after is not None else after
 
     def __repr__(self) -> str:
         return f"{self.gene_name}:{self.chrom}:{self.start}-{self.end}({self.strand})"
 
@@ -187,14 +189,28 @@
         return self._exons
 
     def introns(self) -> List[Tuple[int, int]]:
         if self._introns is None:
             self._introns = [self.start, *(self.exons() | flatten), self.end] | window(2, 2) | skip_while(lambda x: x[0] == x[1]) | to_list
         return self._introns
 
+    def tss(self) -> int:
+        if self.strand == '+':
+            tss = self.start
+        else:
+            tss = self.end
+        return tss
+
+    def tes(self) -> int:
+        if self.strand == '+':
+            tes = self.end
+        else:
+            tes = self.start
+        return tes
+
     def tss_region(self, region: Tuple[int, int] = (-1000, 1000)) -> Tuple[int, ...]:
         if self.strand == '+':
             region = tuple(i+self.start for i in region)
         else:
             region = tuple(reversed(tuple(self.end-i for i in region)))
         return region
 
@@ -226,14 +242,33 @@
         return self._utr5_exons
 
     def utr3_exons(self) -> List[Tuple[int, int]]:
         if self._utr3_exons is None:
             self._classify_exons()
         return self._utr3_exons
 
+    def _condon(self):
+        if self.cds_start is not None and self.cds_end is not None:
+            start_condon_region = (self.cds_start, self.cds_start+3)
+            stop_condon_region = (self.cds_end-3, self.cds_end)
+            if self.strand == '-':
+                start_condon_region, stop_condon_region = stop_condon_region, start_condon_region
+            self._start_condon = start_condon_region
+            self._stop_condon = stop_condon_region
+            
+    def start_condon(self) -> Tuple[int, int]:
+        if self._start_condon is None:
+            self._condon()
+        return self._start_condon
+    
+    def stop_condon(self) -> Tuple[int, int]:
+        if self._stop_condon is None:
+            self._condon()
+        return self._stop_condon
+
     def length(self):
         return self.end - self.start
 
 
 def group_overlap_transcripts(iterable: Iterable[Transcript]) -> Iterator[Tuple[Transcript, ...]]:
     a = deque(itertools.islice(iterable, 1))
     max_end = 0
```

### Comparing `pybiotk-1.2.7/src/pybiotk/annodb/transcript.py` & `pybiotk-1.2.8/src/pybiotk/annodb/transcript.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/convert/bam2fastx.py` & `pybiotk-1.2.8/src/pybiotk/convert/bam2fastx.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/convert/bampe_order_by_name.py` & `pybiotk-1.2.8/src/pybiotk/convert/bampe_order_by_name.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/convert/bed2bedgraph.py` & `pybiotk-1.2.8/src/pybiotk/convert/bed2bedgraph.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/convert/fa2fastq.py` & `pybiotk-1.2.8/src/pybiotk/convert/fa2fastq.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/convert/fq2fasta.py` & `pybiotk-1.2.8/src/pybiotk/convert/fq2fasta.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/convert/gtf2bed.py` & `pybiotk-1.2.8/src/pybiotk/convert/gtf2bed.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/data/hg38.chrom.sizes` & `pybiotk-1.2.8/src/pybiotk/data/hg38.chrom.sizes`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/data/mm10.chrom.sizes` & `pybiotk-1.2.8/src/pybiotk/data/mm10.chrom.sizes`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/intervals/grange.py` & `pybiotk-1.2.8/src/pybiotk/intervals/grange.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/intervals/merge_bed3.py` & `pybiotk-1.2.8/src/pybiotk/intervals/merge_bed3.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/intervals/merge_intervals.py` & `pybiotk-1.2.8/src/pybiotk/intervals/merge_intervals.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/io/bam.py` & `pybiotk-1.2.8/src/pybiotk/io/bam.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from typing import (
     AbstractSet,
     Set,
     DefaultDict,
     Literal,
     Tuple,
     Optional,
-    Iterator
+    Union,
+    Iterator,
+    Callable
 )
 
 import pysam
 
 from pybiotk.utils import logging
 
 
@@ -35,17 +37,24 @@
             bamtype = BamType.PE
         else:
             bamtype = BamType.SE
         sys.stderr.write(f"bamtype is {bamtype.value}.\n")
     return bamtype
 
 
-def count_bam_size(filename: str) -> int:
+def count_bam_size(filename: str, read_callback: Union[str, Callable[[pysam.AlignedSegment], bool]] = "all") -> int:
+    """
+    read_callback (string or function) 
+    select a call-back to ignore reads when counting. It can be either a string with the following values:
+        all: skip reads in which any of the following flags are set: BAM_FUNMAP, BAM_FSECONDARY, BAM_FQCFAIL, BAM_FDUP
+        nofilter: uses every single read
+    Alternatively, read_callback can be a function check_read(read) that should return True only for those reads that shall be included in the counting.
+    """
     with pysam.AlignmentFile(filename) as bam:
-        count = bam.count()
+        count = bam.count(read_callback=read_callback)
     return count
 
 
 class BamTypeError(RuntimeError):
     pass
```

### Comparing `pybiotk-1.2.7/src/pybiotk/io/bed.py` & `pybiotk-1.2.8/src/pybiotk/io/bed.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/io/bw.py` & `pybiotk-1.2.8/src/pybiotk/io/bw.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/io/fasta.py` & `pybiotk-1.2.8/src/pybiotk/io/fasta.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/io/fastq.py` & `pybiotk-1.2.8/src/pybiotk/io/fastq.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/io/gtf.py` & `pybiotk-1.2.8/src/pybiotk/io/gtf.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/string/motif.py` & `pybiotk-1.2.8/src/pybiotk/string/motif.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/string/sequence.py` & `pybiotk-1.2.8/src/pybiotk/string/sequence.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/bam_random.py` & `pybiotk-1.2.8/src/pybiotk/utils/bam_random.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/ercc_parser.py` & `pybiotk-1.2.8/src/pybiotk/utils/ercc_parser.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/fasta_filter.py` & `pybiotk-1.2.8/src/pybiotk/utils/fasta_filter.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/fastq_join.py` & `pybiotk-1.2.8/src/pybiotk/utils/fastq_join.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/fastq_uniq.py` & `pybiotk-1.2.8/src/pybiotk/utils/fastq_uniq.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/fastx_rename.py` & `pybiotk-1.2.8/src/pybiotk/utils/fastx_rename.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/fragment_size.py` & `pybiotk-1.2.8/src/pybiotk/utils/fragment_size.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/genomefetcher.py` & `pybiotk-1.2.8/src/pybiotk/utils/genomefetcher.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/gtf_filter.py` & `pybiotk-1.2.8/src/pybiotk/utils/gtf_filter.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/merge_row.py` & `pybiotk-1.2.8/src/pybiotk/utils/merge_row.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/merge_subseq.py` & `pybiotk-1.2.8/src/pybiotk/utils/merge_subseq.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/normalize.py` & `pybiotk-1.2.8/src/pybiotk/utils/normalize.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/pyanno.py` & `pybiotk-1.2.8/src/pybiotk/utils/pyanno.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/read_tables.py` & `pybiotk-1.2.8/src/pybiotk/utils/read_tables.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/reference_count.py` & `pybiotk-1.2.8/src/pybiotk/utils/reference_count.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/reverse_fastx.py` & `pybiotk-1.2.8/src/pybiotk/utils/reverse_fastx.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/rmats_filter.py` & `pybiotk-1.2.8/src/pybiotk/utils/rmats_filter.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/seq_random.py` & `pybiotk-1.2.8/src/pybiotk/utils/seq_random.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/subseq_analysis.py` & `pybiotk-1.2.8/src/pybiotk/utils/subseq_analysis.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/summary_log.py` & `pybiotk-1.2.8/src/pybiotk/utils/summary_log.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/pybiotk/utils/utils.py` & `pybiotk-1.2.8/src/pybiotk/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 import importlib
 import importlib.resources
 import logging
 import os
 import re
+import signal
 import subprocess
 import sys
 import warnings
 from functools import wraps
 from io import TextIOWrapper
 from types import ModuleType
 from typing import List, Dict, Sequence, Tuple, Literal, Iterator, Iterable, Optional, Callable, Union, TextIO
@@ -56,15 +57,15 @@
             if is_overlap(interval1, interval2):
                 return True
     return False
 
 
 def cigar2cigar_tuples(cigar: str) -> List[Tuple[int, int]]:
     code2cigar = "MIDNSHP=XBp"
-    cigar_regex = re.compile("([-\d]+)([MIDNSHP=XBp])")
+    cigar_regex = re.compile("([-0-9]+)([MIDNSHP=XBp])")
     return [(code2cigar.find(x[1]), int(x[0])) for x in re.findall(cigar_regex, cigar)]
 
 
 def cigar_tuples2blocks(start: int, cigartuples: Sequence[Tuple[int, int]], shift: int = 0) -> List[Tuple[int, int]]:
     tmp_abs_start = shift + start
     blocks = []
     for cigar, length in cigartuples:
@@ -210,29 +211,31 @@
         if fragment_strand == "+":
             fragment_strand = "-"
         else:
             fragment_strand = "+"
     return fragment_strand
 
 
+def handler(signum, frame):
+    sys.exit(0)
+
+
 def ignore(func: Callable):
     @wraps(func)
     def wrapper(*args, **kargs):
         try:
+            signal.signal(signal.SIGINT, handler)
             traceback = func(*args, **kargs)
         except BrokenPipeError:
             # https://docs.python.org/3/library/signal.html#note-on-sigpipe
             # Python flushes standard streams on exit; redirect remaining output
             # to devnull to avoid another BrokenPipeError at shutdown
-            devnull = os.open(os.devnull, os.O_WRONLY)
-            os.dup2(devnull, sys.stdout.fileno())
-            sys.exit(0)
-        except KeyboardInterrupt:
-            devnull = os.open(os.devnull, os.O_WRONLY)
-            os.dup2(devnull, sys.stdout.fileno())
+            if not sys.stdout.closed:
+                devnull = os.open(os.devnull, os.O_WRONLY)
+                os.dup2(devnull, sys.stdout.fileno())
             sys.exit(0)
         return traceback
     return wrapper
 
 
 def load_chrom_length_dict(filepath_or_buffer: Union[str, TextIOWrapper]) -> Dict[str, int]:
     if isinstance(filepath_or_buffer, TextIOWrapper):
```

### Comparing `pybiotk-1.2.7/src/pybiotk.egg-info/PKG-INFO` & `pybiotk-1.2.8/src/pybiotk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybiotk
-Version: 1.2.7
+Version: 1.2.8
 Summary: pybiotk: A python toolkit for bioinformatics analysis.
 Home-page: https://github.com/liqiming-whu/pybiotk
 Author: liqiming_whu
 Author-email: liqiming@whu.edu.cn
 License: MIT
 Project-URL: Documentation, https://github.com/liqiming-whu/pybiotk
 Platform: any
```

### Comparing `pybiotk-1.2.7/src/pybiotk.egg-info/SOURCES.txt` & `pybiotk-1.2.8/src/pybiotk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 src/pybiotk/io/fastq.py
 src/pybiotk/io/gtf.py
 src/pybiotk/string/__init__.py
 src/pybiotk/string/motif.py
 src/pybiotk/string/sequence.py
 src/pybiotk/utils/__init__.py
 src/pybiotk/utils/bam_random.py
+src/pybiotk/utils/bigwigfetcher.py
 src/pybiotk/utils/ercc_parser.py
 src/pybiotk/utils/fasta_filter.py
 src/pybiotk/utils/fastq_join.py
 src/pybiotk/utils/fastq_uniq.py
 src/pybiotk/utils/fastx_rename.py
 src/pybiotk/utils/fragment_size.py
 src/pybiotk/utils/genomefetcher.py
```

### Comparing `pybiotk-1.2.7/src/pybiotk.egg-info/entry_points.txt` & `pybiotk-1.2.8/src/pybiotk.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [console_scripts]
 bam2fastx = pybiotk.convert.bam2fastx:run
 bam_random = pybiotk.utils.bam_random:run
 bampe_order_by_name = pybiotk.convert.bampe_order_by_name:run
 bed2bedgraph = pybiotk.convert.bed2bedgraph:run
+bigwigfetcher = pybiotk.utils.bigwigfetcher:run
 count_normalize = pybiotk.utils.normalize:run
 ercc_parser = pybiotk.utils.ercc_parser:run
 fa2fastq = pybiotk.convert.fa2fastq:run
 fasta_filter = pybiotk.utils.fasta_filter:run
 fastq_join = pybiotk.utils.fastq_join:run
 fastq_uniq = pybiotk.utils.fastq_uniq:run
 fastx_rename = pybiotk.utils.fastx_rename:run
```

### Comparing `pybiotk-1.2.7/src/stream/pipe.py` & `pybiotk-1.2.8/src/stream/pipe.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/src/stream/stream.py` & `pybiotk-1.2.8/src/stream/stream.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.7/tox.ini` & `pybiotk-1.2.8/tox.ini`

 * *Files identical despite different names*

