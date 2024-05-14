# Comparing `tmp/hicstuff-3.2.2.tar.gz` & `tmp/hicstuff-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hicstuff-3.2.2.tar", last modified: Thu Feb 15 09:32:21 2024, max compression
+gzip compressed data, was "hicstuff-3.2.3.tar", last modified: Tue May 14 07:26:05 2024, max compression
```

## Comparing `hicstuff-3.2.2.tar` & `hicstuff-3.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:32:21.881721 hicstuff-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-02-15 09:32:12.000000 hicstuff-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-15 09:32:12.000000 hicstuff-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23608 2024-02-15 09:32:21.881721 hicstuff-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-02-15 09:32:12.000000 hicstuff-3.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:32:21.881721 hicstuff-3.2.2/hicstuff/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77570 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/cutsite.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17135 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/digest.py
--rw-r--r--   0 runner    (1001) docker     (127)    32517 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/distance_law.py
--rw-r--r--   0 runner    (1001) docker     (127)    18713 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    67774 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/hicstuff.py
--rw-r--r--   0 runner    (1001) docker     (127)    46245 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/io.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11000 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/iteralign.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    44318 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-15 09:32:21.000000 hicstuff-3.2.2/hicstuff/version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5542 2024-02-15 09:32:12.000000 hicstuff-3.2.2/hicstuff/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:32:21.881721 hicstuff-3.2.2/hicstuff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23608 2024-02-15 09:32:21.000000 hicstuff-3.2.2/hicstuff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-15 09:32:21.000000 hicstuff-3.2.2/hicstuff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 09:32:21.000000 hicstuff-3.2.2/hicstuff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-15 09:32:21.000000 hicstuff-3.2.2/hicstuff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-15 09:32:21.000000 hicstuff-3.2.2/hicstuff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-15 09:32:21.000000 hicstuff-3.2.2/hicstuff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-15 09:32:12.000000 hicstuff-3.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-15 09:32:21.881721 hicstuff-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-02-15 09:32:12.000000 hicstuff-3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:26:05.961964 hicstuff-3.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-14 07:25:56.000000 hicstuff-3.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 07:25:56.000000 hicstuff-3.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23608 2024-05-14 07:26:05.961964 hicstuff-3.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-05-14 07:25:56.000000 hicstuff-3.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:26:05.961964 hicstuff-3.2.3/hicstuff/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77987 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/cutsite.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17135 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32517 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/distance_law.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18713 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    67774 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/hicstuff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46245 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/io.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11000 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/iteralign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44540 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 07:26:05.000000 hicstuff-3.2.3/hicstuff/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5542 2024-05-14 07:25:56.000000 hicstuff-3.2.3/hicstuff/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:26:05.961964 hicstuff-3.2.3/hicstuff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23608 2024-05-14 07:26:05.000000 hicstuff-3.2.3/hicstuff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-14 07:26:05.000000 hicstuff-3.2.3/hicstuff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:26:05.000000 hicstuff-3.2.3/hicstuff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 07:26:05.000000 hicstuff-3.2.3/hicstuff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 07:26:05.000000 hicstuff-3.2.3/hicstuff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 07:26:05.000000 hicstuff-3.2.3/hicstuff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 07:25:56.000000 hicstuff-3.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 07:26:05.961964 hicstuff-3.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-14 07:25:56.000000 hicstuff-3.2.3/setup.py
```

### Comparing `hicstuff-3.2.2/LICENSE` & `hicstuff-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/PKG-INFO` & `hicstuff-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hicstuff
-Version: 3.2.2
+Version: 3.2.3
 Summary: General purpose stuff to generate and handle Hi-C data in its simplest form.
 Home-page: https://github.com/koszullab/hicstuff
 Author: cyril.matthey-doret@pasteur.fr
 License: BSD-3-Clause
 Description: # hicstuff
         
         [![PyPI version](https://badge.fury.io/py/hicstuff.svg)](https://badge.fury.io/py/hicstuff)
```

### Comparing `hicstuff-3.2.2/README.md` & `hicstuff-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/hicstuff/__init__.py` & `hicstuff-3.2.3/hicstuff/__init__.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/hicstuff/commands.py` & `hicstuff-3.2.3/hicstuff/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     -digest (genome chunking)
     -cutsite (preprocess fastq by cutting reads into digestion products)
     -filter (Hi-C 'event' sorting: loops, uncuts, weird
      and 'true contacts')
     -view (map visualization)
     -pipeline (whole contact map generation)
     -distancelaw (Analysis tool and plot for the distance law)
+    -stats (Extract stats from log)
 
 Running 'pipeline' implies running 'digest', but not
-iteralign or filter unless specified, because they can
+'iteralign' or 'filter' unless specified, because they can
 take up a lot of time for dimnishing returns.
 
 Note
 ----
 Structure based on Rémy Greinhofer (rgreinho) tutorial on subcommands in
 docopt : https://github.com/rgreinho/docopt-subcommands-example
 cmdoret, 20181412
@@ -34,15 +35,15 @@
     Will be raised if an incorrect chunking method (e.g.
     not an enzyme or number or invalid range view is
     specified.
 """
 import re
 import sys, os, shutil
 import tempfile
-from os.path import join, dirname
+from os.path import join, dirname, basename
 from matplotlib import pyplot as plt
 from matplotlib import cm
 from docopt import docopt
 import pandas as pd
 import numpy as np
 import pysam as ps
 import glob
@@ -50,14 +51,15 @@
 from Bio import SeqIO
 import hicstuff.view as hcv
 import hicstuff.hicstuff as hcs
 import hicstuff.cutsite as hcc
 import hicstuff.digest as hcd
 import hicstuff.iteralign as hci
 import hicstuff.filter as hcf
+import hicstuff.stats as hcs
 from hicstuff.version import __version__
 import hicstuff.io as hio
 from hicstuff.log import logger
 import hicstuff.pipeline as hpi
 import hicstuff.distance_law as hcdl
 
 DIVERGENT_CMAPS = [
@@ -1652,14 +1654,28 @@
             ),
             dpi=600,
             vmax=2,
             cmap="Greys",
         )
         logger.info("Output image saved at %s.", out)
 
+class Stats(AbstractCommand):
+    """Extract stats from a hicstuff log file.
+
+    usage:
+        stats <log>
+
+    arguments:
+        log               Path to a hicstuff log file.
+    """
+
+    def execute(self):
+        log_file = self.args["<log>"]
+        stats = hcs.get_pipeline_stats(log_file)
+        hcs.print_pipeline_stats(stats)
 
 def parse_bin_str(bin_str):
     """Bin string parsing
 
     Take a basepair binning string as input and converts it into
     corresponding basepair values.
 
@@ -1692,15 +1708,14 @@
         unit_pos = re.search(r"[KMG]?$", bin_str).start()
         bp_unit = bin_str[unit_pos:]
         # Extract unit and multiply accordingly for fixed bp binning
         binning = int(float(bin_str[:unit_pos]) * binsuffix[bp_unit[0]])
 
     return binning
 
-
 def parse_ucsc(ucsc_str, bins):
     """
     Take a UCSC region in UCSC notation and a list of bin chromosomes and
     positions (in basepair) and converts it to range of bins.
 
     Parameters
     ----------
```

### Comparing `hicstuff-3.2.2/hicstuff/cutsite.py` & `hicstuff-3.2.3/hicstuff/cutsite.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/hicstuff/digest.py` & `hicstuff-3.2.3/hicstuff/digest.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/hicstuff/distance_law.py` & `hicstuff-3.2.3/hicstuff/distance_law.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/hicstuff/filter.py` & `hicstuff-3.2.3/hicstuff/filter.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/hicstuff/hicstuff.py` & `hicstuff-3.2.3/hicstuff/hicstuff.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/hicstuff/io.py` & `hicstuff-3.2.3/hicstuff/io.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/hicstuff/iteralign.py` & `hicstuff-3.2.3/hicstuff/iteralign.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/hicstuff/log.py` & `hicstuff-3.2.3/hicstuff/log.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/hicstuff/main.py` & `hicstuff-3.2.3/hicstuff/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     digest          Digest genome into a list of fragments.
     cutsite         Preprocess fastq files by digesting reads at religation site.
     distancelaw     Analyse and plot distance law.
     filter          Filters Hi-C pairs to exclude spurious events.
     iteralign       Iteratively aligns reads to a reference genome.
     missview        Preview missing Hi-C bins in based on the genome and read length.
     pipeline        Hi-C pipeline to generate contact matrix from fastq files.
+    stats           Extract mapping statistics from a hicstuff pipeline log file.
     rebin           Bin the matrix and regenerate files accordingly.
     subsample       Bootstrap subsampling of contacts from a Hi-C map.
     view            Visualize a Hi-C matrix.    
 """
 
 from docopt import docopt
 from docopt import DocoptExit
```

### Comparing `hicstuff-3.2.2/hicstuff/pipeline.py` & `hicstuff-3.2.3/hicstuff/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 import hicstuff.filter as hcf
 import hicstuff.io as hio
 import hicstuff.distance_law as hcdl
 import hicstuff.cutsite as hcc
 import hicstuff.stats as hcs
 import matplotlib
 import pathlib
+import pairtools
+from packaging.version import Version
 from hicstuff.version import __version__
 import hicstuff.log as hcl
 from hicstuff.log import logger
 
 
 def align_reads(
     reads,
@@ -1136,15 +1138,16 @@
             threads=threads,
             tmp_dir=tmp_dir,
         )
 
     # Get stats on the pipeline
     try:
         logger.info("Fetching mapping and pairing stats")
-        hcs.get_pipeline_stats(prefix, out_dir, log_file)
+        stats = hcs.get_pipeline_stats(log_file)
+        logger.info(stats)
     except IndexError: 
         logger.warning("IndexError. Stats not compiled.")
         pass 
     
     # Move final pairs file to main dir. 
     p = pathlib.Path(use_pairs).absolute()
     pairsf = p.parents[1] / p.name
@@ -1152,14 +1155,16 @@
     
     # Sort and compress final pairs file
     pairstools_cmd = "pairtools sort".split(" ")
     sorted_pairsf = str(pairsf) + ".gz"
     sort_args = "--output {out} --tmpdir {tmp_dir}".format(
         out = sorted_pairsf, tmp_dir = tmp_dir
     )
+    if (Version(pairtools.__version__) >= Version('1.1.0')): 
+        sort_args = sort_args + " --c1 chr1 --c2 chr2 --p1 pos1 --p2 pos2 --pt frag1" 
     sp.call(pairstools_cmd + sort_args.split(" ") + [pairsf], shell=False)
     os.remove(pairsf)
     
     # Clean temporary files
     if not no_cleanup:
         tempfiles = [
             pairs,
```

### Comparing `hicstuff-3.2.2/hicstuff/stats.py` & `hicstuff-3.2.3/hicstuff/stats.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import re 
-from os.path import join
+import os 
+from os.path import basename
+from os.path import splitext
 import json
 
-def get_pipeline_stats(prefix, out_dir, log_file):
+def get_pipeline_stats(log_file):
     """Get stats after pipeline execution.
 
     Parameters
     ----------
-    prefix : str
-        The prefix used to create output files by the pipeline.
-    out_dir : str
-        The prefix used to create output files by the pipeline.
     log_file : str
         Path to hicstuff log file.
 
     Returns
     -------
-    txt file:
-        A single text file containing stats about hicstuff pipeline execution: 
+    list:
+        A single list containing stats about hicstuff pipeline execution: 
         - Number of sequenced pairs from fastqs
         - Number (% of total reads) of unmapped reads 
         - Number (% of total reads) of mapped reads 
         - Number (% of total reads) of pairs 
         - Number (% of total pairs) of filtered pairs 
             - Number (% of total pairs) of loops
             - Number (% of total pairs) of uncuts
@@ -36,34 +34,31 @@
             - Trans ratio
     """
 
     with open(log_file) as file:
         log_lines = [line.rstrip() for line in file]
 
     # 1. Number of sequenced pairs from fastqs
-    fastq_pairs = [s for s in log_lines if re.search("reads found in eajch fastq file.", s)][0]
+    fastq_pairs = [s for s in log_lines if re.search("reads found in each", s)][0]
     fastq_pairs = re.sub(".*INFO :: ", "", fastq_pairs)
-    fastq_pairs = re.sub(" reads found in each fastq file.*", "", fastq_pairs)
+    fastq_pairs = re.sub(" reads found in each.*", "", fastq_pairs)
     fastq_pairs = int(float(fastq_pairs))
     
     # 2. Number (% of total) of (un)mapped reads
     tot_mapped = [s for s in log_lines if re.search("mapped with Q ", s)][0]
     tot_mapped = re.sub(".*Q >= 30 \(", "", tot_mapped)
     tot_mapped = re.sub("/.*", "", tot_mapped)
     tot_mapped = int(float(tot_mapped))
     tot_unmapped = fastq_pairs*2 - tot_mapped
-    pct_mapped = round(tot_mapped/(fastq_pairs*2)*100, 2)
-    pct_unmapped = round(tot_unmapped/(fastq_pairs*2)*100, 2)
 
     # 3. Number (% of total) of pairs
     tot_pairs = [s for s in log_lines if re.search("pairs successfully mapped", s)][0]
     tot_pairs = re.sub(".*INFO :: ", "", tot_pairs)
     tot_pairs = re.sub(" pairs successfully.*", "", tot_pairs)
     tot_pairs = int(float(tot_pairs))
-    pct_pairs = round(tot_pairs/fastq_pairs*100, 2)
     
     # 4. Number (% of total) of filtered pairs
     filtered_pairs = [s for s in log_lines if re.search("pairs discarded:", s)]
     if (len(filtered_pairs) > 0): 
         filtered_pairs = filtered_pairs[0]
         loops_pairs = re.sub(".*Loops: ", "", filtered_pairs)
         loops_pairs = re.sub(", Uncuts:.*", "", loops_pairs)
@@ -77,78 +72,114 @@
         filtered_pairs = re.sub(" pairs discarded.*", "", filtered_pairs)
         filtered_pairs = int(float(filtered_pairs))
     else: 
         loops_pairs=0
         uncuts_pairs=0
         abnormal_pairs=0
         filtered_pairs=0
-    pct_filtered = round(filtered_pairs/tot_pairs*100, 2)
-    pct_loops_pairs = round(loops_pairs/tot_pairs*100, 2)
-    pct_uncuts_pairs = round(uncuts_pairs/tot_pairs*100, 2)
-    pct_abnormal_pairs = round(abnormal_pairs/tot_pairs*100, 2)
 
-    # 5. Number (% of total) of PCR dups pairs
-    PCR_pairs = [s for s in log_lines if re.search("PCR duplicates have been filtered", s)]
-    if (len(PCR_pairs) > 0): 
-        PCR_pairs = PCR_pairs[0]
-        PCR_pairs = re.sub(".*have been filtered out \(", "", PCR_pairs)
-        PCR_pairs = re.sub(" / .*", "", PCR_pairs)
-        PCR_pairs = int(float(PCR_pairs))
+    # 5. Number (% of total) of PCR duplicates pairs
+    pcr_pairs = [s for s in log_lines if re.search("PCR duplicates have been filtered", s)]
+    if (len(pcr_pairs) > 0): 
+        pcr_pairs = pcr_pairs[0]
+        pcr_pairs = re.sub(".*have been filtered out \(", "", pcr_pairs)
+        pcr_pairs = re.sub(" / .*", "", pcr_pairs)
+        pcr_pairs = int(float(pcr_pairs))
     else: 
-        PCR_pairs = 0
-    pct_PCR = round(PCR_pairs/tot_pairs*100, 2)
+        pcr_pairs = 0
 
     # 6. Number (%) of final pairs
-    kept_pairs=tot_pairs-filtered_pairs-PCR_pairs
-    pct_kept = round(kept_pairs/tot_pairs*100, 2)
-
-    # Open the log file and read its contents
-    stats_file_path = join(out_dir, prefix + ".stats.txt")
-    with open(stats_file_path, 'w') as stats_file:
-        stats_file.write("Sample:             {prefix}\n".format(prefix = prefix))
-        stats_file.write("Total read pairs:   {reads}\n".format(reads = "{:,}".format(fastq_pairs)))
-        stats_file.write("Mapped reads:       {tot_mapped} ({pct_mapped}%  of all reads)\n".format(
-                tot_mapped = "{:,}".format(tot_mapped), 
-                pct_mapped = pct_mapped
-            )
-        )
-        stats_file.write("Unmapped reads:     {tot_unmapped} ({pct_unmapped}%  of all reads)\n".format(
-            tot_unmapped = "{:,}".format(tot_unmapped), pct_unmapped = pct_unmapped
-        ))
-        stats_file.write("Recovered contacts: {tot_pairs} ({pct_pairs}%  of all read pairs)\n".format(
-            tot_pairs = "{:,}".format(tot_pairs), pct_pairs = pct_pairs
-        ))
-        stats_file.write("Final contacts:     {kept_pairs} ({pct_kept}% of all contacts)\n".format(
-            kept_pairs = "{:,}".format(kept_pairs), pct_kept = pct_kept
-        ))
-        stats_file.write("  Filtered out:     {filtered_pairs} ({pct_filtered}% of all contacts)\n".format(
-            filtered_pairs = "{:,}".format(filtered_pairs), pct_filtered = pct_filtered
-        ))
-        stats_file.write("    Loops:          {loops_pairs} ({pct_loops_pairs}% of all contacts)\n".format(
-            loops_pairs = "{:,}".format(loops_pairs), pct_loops_pairs = pct_loops_pairs
-        ))
-        stats_file.write("    Uncuts:         {uncuts_pairs} ({pct_uncuts_pairs}% of all contacts)\n".format(
-            uncuts_pairs = "{:,}".format(uncuts_pairs), pct_uncuts_pairs = pct_uncuts_pairs
-        ))
-        stats_file.write("    Weirds:         {abnormal_pairs} ({pct_abnormal_pairs}% of all contacts)\n".format(
-            abnormal_pairs = "{:,}".format(abnormal_pairs), pct_abnormal_pairs = pct_abnormal_pairs
-        ))
-        stats_file.write("  PCR duplicates:   {PCR_pairs} ({pct_PCR}% of all contacts)\n".format(
-            PCR_pairs = "{:,}".format(PCR_pairs), pct_PCR = pct_PCR
-        ))
-
+    removed_pairs=filtered_pairs+pcr_pairs
+    final_pairs=tot_pairs-removed_pairs
+    
+    # 7. Final stats
     stats = {
+        'Sample': re.sub(".hicstuff.*", "", basename(log_file)),
         'Total read pairs': fastq_pairs,
         'Mapped reads': tot_mapped,
         'Unmapped reads': tot_unmapped,
         'Recovered contacts': tot_pairs,
-        'Final contacts': kept_pairs,
+        'Final contacts': final_pairs,
+        'Removed contacts': removed_pairs,
         'Filtered out': filtered_pairs,
         'Loops': loops_pairs,
         'Uncuts': uncuts_pairs,
         'Weirds': abnormal_pairs,
-        'PCR duplicates': PCR_pairs
+        'PCR duplicates': pcr_pairs
     }
-    stats_json_path = join(out_dir, prefix + ".stats.json")
-    with open(stats_json_path, 'w') as json_file:
-        json.dump(stats, json_file, indent=4)
 
+    return(stats)
+
+def write_pipeline_stats(stats, out_file): 
+    prefix = stats['Sample']
+    fastq_pairs=stats['Total read pairs']
+    tot_mapped=stats['Mapped reads']
+    tot_unmapped=stats['Unmapped reads']
+    tot_pairs=stats['Recovered contacts']
+    final_pairs=stats['Final contacts']
+    removed_pairs=stats['Removed contacts']
+    filtered_pairs=stats['Filtered out']
+    loops_pairs=stats['Loops']
+    uncuts_pairs=stats['Uncuts']
+    abnormal_pairs=stats['Weirds']
+    pcr_pairs=stats['PCR duplicates']
+    pct_pairs = round(tot_pairs/fastq_pairs*100, 2)
+    pct_mapped = round(tot_mapped/(fastq_pairs*2)*100, 2)
+    pct_unmapped = round(tot_unmapped/(fastq_pairs*2)*100, 2)
+    pct_filtered = round(filtered_pairs/tot_pairs*100, 2)
+    pct_loops_pairs = round(loops_pairs/tot_pairs*100, 2)
+    pct_uncuts_pairs = round(uncuts_pairs/tot_pairs*100, 2)
+    pct_abnormal_pairs = round(abnormal_pairs/tot_pairs*100, 2)
+    pct_pcr = round(pcr_pairs/tot_pairs*100, 2)
+    pct_removed=round(removed_pairs/tot_pairs*100, 2)
+    pct_final = round(final_pairs/tot_pairs*100, 2)
+
+    # Open the log file and read its contents
+    _, file_extension = splitext(out_file)
+    if (file_extension == '.json'):
+        with open(out_file, 'w') as json_file:
+            json.dump(stats, json_file, indent=4)
+    else:
+        with open(out_file, 'w') as stats_file:
+            stats_file.write("Sample:             {prefix}\n".format(prefix = prefix))
+            stats_file.write("Total read pairs:   {reads}\n".format(reads = "{:,}".format(fastq_pairs)))
+            stats_file.write("Mapped reads:       {tot_mapped} ({pct_mapped}%  of all reads)\n".format(
+                    tot_mapped = "{:,}".format(tot_mapped), 
+                    pct_mapped = pct_mapped
+                )
+            )
+            stats_file.write("Unmapped reads:     {tot_unmapped} ({pct_unmapped}%  of all reads)\n".format(
+                tot_unmapped = "{:,}".format(tot_unmapped), pct_unmapped = pct_unmapped
+            ))
+            stats_file.write("Recovered contacts: {tot_pairs} ({pct_pairs}%  of all read pairs)\n".format(
+                tot_pairs = "{:,}".format(tot_pairs), pct_pairs = pct_pairs
+            ))
+            stats_file.write("Removed contacts:   {removed_pairs} ({pct_removed}% of all contacts)\n".format(
+                removed_pairs = "{:,}".format(removed_pairs), pct_removed = pct_removed
+            ))
+            stats_file.write("  Filtered out:     {filtered_pairs} ({pct_filtered}% of all contacts)\n".format(
+                filtered_pairs = "{:,}".format(filtered_pairs), pct_filtered = pct_filtered
+            ))
+            stats_file.write("    Loops:          {loops_pairs} ({pct_loops_pairs}% of all contacts)\n".format(
+                loops_pairs = "{:,}".format(loops_pairs), pct_loops_pairs = pct_loops_pairs
+            ))
+            stats_file.write("    Uncuts:         {uncuts_pairs} ({pct_uncuts_pairs}% of all contacts)\n".format(
+                uncuts_pairs = "{:,}".format(uncuts_pairs), pct_uncuts_pairs = pct_uncuts_pairs
+            ))
+            stats_file.write("    Weirds:         {abnormal_pairs} ({pct_abnormal_pairs}% of all contacts)\n".format(
+                abnormal_pairs = "{:,}".format(abnormal_pairs), pct_abnormal_pairs = pct_abnormal_pairs
+            ))
+            stats_file.write("  PCR duplicates:   {pcr_pairs} ({pct_pcr}% of all contacts)\n".format(
+                pcr_pairs = "{:,}".format(pcr_pairs), pct_pcr = pct_pcr
+            ))
+            stats_file.write("Final contacts:     {final_pairs} ({pct_final}% of all contacts)\n".format(
+            final_pairs = "{:,}".format(final_pairs), pct_final = pct_final
+        ))
+
+def print_pipeline_stats(stats): 
+    tmp = '.'+stats['Sample']+'.txt'
+    write_pipeline_stats(stats, tmp)
+    with open(tmp, 'r') as file: 
+        lines = [line for line in file]
+        print(''.join(lines))
+    os.unlink(tmp)
+
```

### Comparing `hicstuff-3.2.2/hicstuff/view.py` & `hicstuff-3.2.3/hicstuff/view.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/hicstuff.egg-info/PKG-INFO` & `hicstuff-3.2.3/hicstuff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hicstuff
-Version: 3.2.2
+Version: 3.2.3
 Summary: General purpose stuff to generate and handle Hi-C data in its simplest form.
 Home-page: https://github.com/koszullab/hicstuff
 Author: cyril.matthey-doret@pasteur.fr
 License: BSD-3-Clause
 Description: # hicstuff
         
         [![PyPI version](https://badge.fury.io/py/hicstuff.svg)](https://badge.fury.io/py/hicstuff)
```

### Comparing `hicstuff-3.2.2/hicstuff.egg-info/SOURCES.txt` & `hicstuff-3.2.3/hicstuff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hicstuff-3.2.2/setup.py` & `hicstuff-3.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Operating System :: MacOS",
 ]
 
 name = "hicstuff"
 
 MAJOR = 3
 MINOR = 2
-MAINTENANCE = 2
+MAINTENANCE = 3
 VERSION = "{}.{}.{}".format(MAJOR, MINOR, MAINTENANCE)
 
 LICENSE = "BSD-3-Clause"
 URL = "https://github.com/koszullab/hicstuff"
 
 DESCRIPTION = __doc__.strip("\n")
```

