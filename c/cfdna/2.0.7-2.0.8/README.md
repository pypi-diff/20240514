# Comparing `tmp/cfdna-2.0.7.tar.gz` & `tmp/cfdna-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfdna-2.0.7.tar", max compression
+gzip compressed data, was "cfdna-2.0.8.tar", max compression
```

## Comparing `cfdna-2.0.7.tar` & `cfdna-2.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rwxr-xr-x   0        0        0    17895 2022-07-20 16:09:08.000000 cfdna-2.0.7/LICENSE.md
--rwxr-xr-x   0        0        0     1341 2023-11-21 14:09:42.209706 cfdna-2.0.7/README.md
--rw-r--r--   0        0        0     8196 2024-04-15 19:39:52.737913 cfdna-2.0.7/cfdna/.DS_Store
--rwxr-xr-x   0        0        0      638 2024-04-16 03:46:52.824792 cfdna-2.0.7/cfdna/__init__.py
--rwxr-xr-x   0        0        0     4486 2024-04-16 02:05:12.659608 cfdna-2.0.7/cfdna/__main__.py
--rwxr-xr-x   0        0        0       69 2022-07-20 16:09:08.000000 cfdna-2.0.7/cfdna/commandline/__init__.py
--rwxr-xr-x   0        0        0     8267 2024-04-16 03:13:23.158743 cfdna-2.0.7/cfdna/commandline/commands.py
--rwxr-xr-x   0        0        0       64 2022-08-30 19:13:58.000000 cfdna-2.0.7/cfdna/core/__init__.py
--rwxr-xr-x   0        0        0     2918 2023-11-06 18:52:38.951861 cfdna-2.0.7/cfdna/core/core.py
--rw-r--r--   0        0        0     6148 2023-11-06 14:19:28.230169 cfdna-2.0.7/cfdna/io/.DS_Store
--rwxr-xr-x   0        0        0      281 2022-07-20 16:09:09.000000 cfdna-2.0.7/cfdna/io/__init__.py
--rwxr-xr-x   0        0        0      184 2022-07-20 16:09:09.000000 cfdna-2.0.7/cfdna/io/read/__init__.py
--rwxr-xr-x   0        0        0     1762 2023-02-03 15:34:27.663648 cfdna-2.0.7/cfdna/io/read/read_bam.py
--rwxr-xr-x   0        0        0      491 2023-11-06 18:42:33.912191 cfdna-2.0.7/cfdna/io/read/read_h5.py
--rwxr-xr-x   0        0        0      190 2022-07-20 16:09:09.000000 cfdna-2.0.7/cfdna/io/write/__init__.py
--rwxr-xr-x   0        0        0      511 2023-11-06 18:43:44.583371 cfdna-2.0.7/cfdna/io/write/write_h5.py
--rwxr-xr-x   0        0        0      849 2022-07-20 16:09:09.000000 cfdna-2.0.7/cfdna/io/write/write_text.py
--rwxr-xr-x   0        0        0       67 2022-07-20 16:09:08.000000 cfdna-2.0.7/cfdna/plot/__init__.py
--rwxr-xr-x   0        0        0     7663 2022-07-20 16:09:09.000000 cfdna-2.0.7/cfdna/plot/plot_bokeh.py
--rwxr-xr-x   0        0        0      990 2023-11-07 16:01:23.498388 cfdna-2.0.7/cfdna/plot/plot_plt.py
--rwxr-xr-x   0        0        0      391 2022-10-05 14:16:05.000000 cfdna-2.0.7/cfdna/tools/__init__.py
--rwxr-xr-x   0        0        0      167 2023-11-06 18:36:25.971444 cfdna-2.0.7/cfdna/tools/cnv/__init__.py
--rwxr-xr-x   0        0        0     3563 2023-11-06 18:44:12.544286 cfdna-2.0.7/cfdna/tools/cnv/segmentation.py
--rw-r--r--   0        0        0     1334 2024-03-21 21:01:17.622900 cfdna-2.0.7/cfdna/tools/coverage/gene_activity.py
--rwxr-xr-x   0        0        0      165 2022-07-20 16:09:08.000000 cfdna-2.0.7/cfdna/tools/fragmentation/__init__.py
--rwxr-xr-x   0        0        0     2418 2022-08-30 16:29:27.000000 cfdna-2.0.7/cfdna/tools/fragmentation/frag_pattern.py
--rwxr-xr-x   0        0        0      175 2022-07-20 16:09:08.000000 cfdna-2.0.7/cfdna/tools/nucleosome/__init__.py
--rw-r--r--   0        0        0     4281 2022-10-20 20:27:47.000000 cfdna-2.0.7/cfdna/tools/nucleosome/gene_activity.py
--rwxr-xr-x   0        0        0     8696 2022-08-30 16:32:05.000000 cfdna-2.0.7/cfdna/tools/nucleosome/nfr.py
--rw-r--r--   0        0        0     5375 2022-10-21 19:39:37.000000 cfdna-2.0.7/cfdna/tools/nucleosome/relative_window.py
--rwxr-xr-x   0        0        0     4302 2022-10-05 14:44:52.000000 cfdna-2.0.7/cfdna/tools/nucleosome/wps.py
--rw-r--r--   0        0        0     7053 2022-10-05 14:45:53.000000 cfdna-2.0.7/cfdna/tools/nucleosome/wps_functions.py
--rwxr-xr-x   0        0        0      162 2022-07-20 16:09:08.000000 cfdna-2.0.7/cfdna/tools/summarize/__init__.py
--rw-r--r--   0        0        0     3551 2022-08-30 19:26:15.000000 cfdna-2.0.7/cfdna/tools/summarize/multi_sample.py
--rwxr-xr-x   0        0        0     3417 2023-11-06 18:46:14.639312 cfdna-2.0.7/cfdna/tools/summarize/summarize.py
--rwxr-xr-x   0        0        0      143 2022-07-20 16:09:09.000000 cfdna-2.0.7/cfdna/utilities/__init__.py
--rwxr-xr-x   0        0        0     4289 2022-08-30 19:22:16.000000 cfdna-2.0.7/cfdna/utilities/h5_utilities.py
--rw-r--r--   0        0        0     2478 2024-04-16 03:48:10.613356 cfdna-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 cfdna-2.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2022-07-20 16:09:08.000000 cfdna-2.0.8/LICENSE.md
+-rwxr-xr-x   0        0        0     1341 2023-11-21 14:09:42.209706 cfdna-2.0.8/README.md
+-rw-r--r--   0        0        0     8196 2024-05-08 14:42:10.009834 cfdna-2.0.8/cfdna/.DS_Store
+-rwxr-xr-x   0        0        0      638 2024-05-08 14:59:14.786741 cfdna-2.0.8/cfdna/__init__.py
+-rwxr-xr-x   0        0        0     4486 2024-04-16 02:05:12.659608 cfdna-2.0.8/cfdna/__main__.py
+-rwxr-xr-x   0        0        0       69 2022-07-20 16:09:08.000000 cfdna-2.0.8/cfdna/commandline/__init__.py
+-rwxr-xr-x   0        0        0     8737 2024-05-08 15:14:26.771522 cfdna-2.0.8/cfdna/commandline/commands.py
+-rwxr-xr-x   0        0        0       64 2022-08-30 19:13:58.000000 cfdna-2.0.8/cfdna/core/__init__.py
+-rwxr-xr-x   0        0        0     2918 2023-11-06 18:52:38.951861 cfdna-2.0.8/cfdna/core/core.py
+-rw-r--r--   0        0        0     6148 2023-11-06 14:19:28.230169 cfdna-2.0.8/cfdna/io/.DS_Store
+-rwxr-xr-x   0        0        0      281 2022-07-20 16:09:09.000000 cfdna-2.0.8/cfdna/io/__init__.py
+-rwxr-xr-x   0        0        0      184 2022-07-20 16:09:09.000000 cfdna-2.0.8/cfdna/io/read/__init__.py
+-rwxr-xr-x   0        0        0     1762 2023-02-03 15:34:27.663648 cfdna-2.0.8/cfdna/io/read/read_bam.py
+-rwxr-xr-x   0        0        0      491 2023-11-06 18:42:33.912191 cfdna-2.0.8/cfdna/io/read/read_h5.py
+-rwxr-xr-x   0        0        0      190 2022-07-20 16:09:09.000000 cfdna-2.0.8/cfdna/io/write/__init__.py
+-rwxr-xr-x   0        0        0      511 2023-11-06 18:43:44.583371 cfdna-2.0.8/cfdna/io/write/write_h5.py
+-rwxr-xr-x   0        0        0      849 2022-07-20 16:09:09.000000 cfdna-2.0.8/cfdna/io/write/write_text.py
+-rwxr-xr-x   0        0        0       67 2022-07-20 16:09:08.000000 cfdna-2.0.8/cfdna/plot/__init__.py
+-rwxr-xr-x   0        0        0     7663 2022-07-20 16:09:09.000000 cfdna-2.0.8/cfdna/plot/plot_bokeh.py
+-rwxr-xr-x   0        0        0      990 2023-11-07 16:01:23.498388 cfdna-2.0.8/cfdna/plot/plot_plt.py
+-rwxr-xr-x   0        0        0      391 2022-10-05 14:16:05.000000 cfdna-2.0.8/cfdna/tools/__init__.py
+-rwxr-xr-x   0        0        0      167 2023-11-06 18:36:25.971444 cfdna-2.0.8/cfdna/tools/cnv/__init__.py
+-rwxr-xr-x   0        0        0     3563 2023-11-06 18:44:12.544286 cfdna-2.0.8/cfdna/tools/cnv/segmentation.py
+-rw-r--r--   0        0        0     1334 2024-03-21 21:01:17.622900 cfdna-2.0.8/cfdna/tools/coverage/gene_activity.py
+-rwxr-xr-x   0        0        0      165 2022-07-20 16:09:08.000000 cfdna-2.0.8/cfdna/tools/fragmentation/__init__.py
+-rwxr-xr-x   0        0        0     2418 2022-08-30 16:29:27.000000 cfdna-2.0.8/cfdna/tools/fragmentation/frag_pattern.py
+-rwxr-xr-x   0        0        0      175 2022-07-20 16:09:08.000000 cfdna-2.0.8/cfdna/tools/nucleosome/__init__.py
+-rw-r--r--   0        0        0     4281 2022-10-20 20:27:47.000000 cfdna-2.0.8/cfdna/tools/nucleosome/gene_activity.py
+-rwxr-xr-x   0        0        0     8696 2022-08-30 16:32:05.000000 cfdna-2.0.8/cfdna/tools/nucleosome/nfr.py
+-rw-r--r--   0        0        0     5375 2022-10-21 19:39:37.000000 cfdna-2.0.8/cfdna/tools/nucleosome/relative_window.py
+-rwxr-xr-x   0        0        0     8490 2024-05-09 17:45:05.523659 cfdna-2.0.8/cfdna/tools/nucleosome/wps.py
+-rw-r--r--   0        0        0     7053 2022-10-05 14:45:53.000000 cfdna-2.0.8/cfdna/tools/nucleosome/wps_functions.py
+-rwxr-xr-x   0        0        0      162 2022-07-20 16:09:08.000000 cfdna-2.0.8/cfdna/tools/summarize/__init__.py
+-rw-r--r--   0        0        0     3551 2022-08-30 19:26:15.000000 cfdna-2.0.8/cfdna/tools/summarize/multi_sample.py
+-rwxr-xr-x   0        0        0     3417 2023-11-06 18:46:14.639312 cfdna-2.0.8/cfdna/tools/summarize/summarize.py
+-rwxr-xr-x   0        0        0      143 2022-07-20 16:09:09.000000 cfdna-2.0.8/cfdna/utilities/__init__.py
+-rwxr-xr-x   0        0        0     4289 2022-08-30 19:22:16.000000 cfdna-2.0.8/cfdna/utilities/h5_utilities.py
+-rw-r--r--   0        0        0     2474 2024-05-14 14:31:10.040759 cfdna-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3553 1970-01-01 00:00:00.000000 cfdna-2.0.8/PKG-INFO
```

### Comparing `cfdna-2.0.7/LICENSE.md` & `cfdna-2.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/README.md` & `cfdna-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/.DS_Store` & `cfdna-2.0.8/cfdna/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 00001030: 00b8 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
 00001040: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
 00001050: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
 00001060: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 00001070: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 00001080: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00001090: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
-000010a0: 095f 1018 7b7b 3335 372c 2034 3330 7d2c  ._..{{357, 430},
+000010a0: 095f 1018 7b7b 3434 322c 2032 3736 7d2c  ._..{{442, 276},
 000010b0: 207b 3932 302c 2034 3336 7d7d 0908 1523   {920, 436}}...#
 000010c0: 2f3b 525f 6b6c 6d6e 6f8a 0000 0000 0000  /;R_klmno.......
 000010d0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
 000010e0: 0000 0000 0000 0000 008b 0000 000b 0063  ...............c
 000010f0: 006f 006d 006d 0061 006e 0064 006c 0069  .o.m.m.a.n.d.l.i
 00001100: 006e 0065 7653 726e 6c6f 6e67 0000 0001  .n.evSrnlong....
 00001110: 0000 0004 0063 006f 0072 0065 6277 7370  .....c.o.r.ebwsp
@@ -318,16 +318,16 @@
 000013d0: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
 000013e0: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
 000013f0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00001400: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 00001410: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 00001420: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 00001430: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00001440: 6261 7208 0908 095f 1018 7b7b 3135 352c  bar...._..{{155,
-00001450: 2033 3634 7d2c 207b 3932 302c 2034 3336   364}, {920, 436
+00001440: 6261 7208 0908 095f 1018 7b7b 3235 302c  bar...._..{{250,
+00001450: 2033 3336 7d2c 207b 3932 302c 2034 3336   336}, {920, 436
 00001460: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
 00001470: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 00001480: 0000 0000 0000 0000 0000 0000 0000 008b  ................
 00001490: 0000 0005 0074 006f 006f 006c 0073 7653  .....t.o.o.l.svS
 000014a0: 726e 6c6f 6e67 0000 0001 0000 0009 0075  rnlong.........u
 000014b0: 0074 0069 006c 0069 0074 0069 0065 0073  .t.i.l.i.t.i.e.s
 000014c0: 6277 7370 626c 6f62 0000 00b7 6270 6c69  bwspblob....bpli
```

### Comparing `cfdna-2.0.7/cfdna/__init__.py` & `cfdna-2.0.8/cfdna/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from . import commandline as cmd
 from . import tools as tl
 
 from ngsfragments import Fragments
 
 
 # This is extracted automatically by the top-level setup.py.
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 
 __author__ = "Kyle S. Smith"
 
 __doc__ = """\
 
 API
 ======
```

### Comparing `cfdna-2.0.7/cfdna/__main__.py` & `cfdna-2.0.8/cfdna/__main__.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/commandline/commands.py` & `cfdna-2.0.8/cfdna/commandline/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,28 +55,32 @@
                                                                 hmm_binsize=args.hmm_bin_size,
                                                                 nthreads = nthreads,
                                                                 use_normal = args.use_normal,
                                                                 keep_sex_chroms = args.add_sex,
                                                                 normal = [0.1, 0.25, 0.5, 0.75, 0.9],
                                                                 ploidy = [1,2,3],
                                                                 estimatePloidy = True,
-                                                                scStates = [1, 3])
+                                                                scStates = [1, 3],
+                                                                minSegmentBins = 50,
+                                                                maxCN = 5)
             else:
                 cfdna_object = ngs.segment.cnv_pipeline.call_cnv_pipeline(cfdna_object,
                                                             frags,
                                                             genome_version=args.genome,
                                                             cnv_binsize=args.bin_size,
                                                             hmm_binsize=args.hmm_bin_size,
                                                             nthreads = nthreads,
                                                             use_normal = args.use_normal,
                                                             keep_sex_chroms = args.add_sex,
                                                             normal = [0.1, 0.25, 0.5, 0.75, 0.9],
                                                             ploidy = [1,2,3],
                                                             estimatePloidy = True,
-                                                            scStates = None)
+                                                            scStates = None,
+                                                            minSegmentBins = 50,
+                                                            maxCN = 5)
             
             # Add WPS
             if args.add_wps:
                 scores = ngs.metrics.wps_windows(frags,
                                                 protection = 120,
                                                 min_length = args.min_length,
                                                 max_length = args.max_length,
@@ -105,20 +109,23 @@
 
         # Write annotations
         if args.anno_file:
             cfdna_object.anno.engine.df.to_csv(prefix+"_metrics.txt", header=True, index=True, sep="\t")
         
         # Write seg annotations
         if args.anno_segs:
+            sample = os.path.split(prefix)[-1]
             df = cfdna_object.obs_intervals[sample]["cnv_segments"].df
             df.loc[:,"chrom"] = cfdna_object.obs_intervals[sample]["cnv_segments"].index.labels
             df.loc[:,"start"] = cfdna_object.obs_intervals[sample]["cnv_segments"].index.starts
             df.loc[:,"end"] = cfdna_object.obs_intervals[sample]["cnv_segments"].index.ends
-            df = df.loc[:,['chrom', 'start', 'end', 'median', 'copy_number', 'event', 'subclone_status',
-                           'logR_Copy_Number', 'Corrected_Copy_Number', 'Corrected_Call', 'var']]
+            df.loc[:,"sample"] = sample
+            df.loc[:,"bin_size"] = args.bin_size
+            df = df.loc[:,['sample', 'chrom', 'start', 'end', 'median', 'copy_number', 'event', 'subclone_status',
+                           'logR_Copy_Number', 'Corrected_Copy_Number', 'Corrected_Call', 'var', 'bin_size']]
             df.to_csv(prefix+"_seg_annotations.txt", header=True, index=False, sep="\t")
 
             # Drop columns
             df.drop(columns=["chrom", "start", "end"], inplace=True)
 
 
 def GeneActivity(args):
```

### Comparing `cfdna-2.0.7/cfdna/core/core.py` & `cfdna-2.0.8/cfdna/core/core.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/io/.DS_Store` & `cfdna-2.0.8/cfdna/io/.DS_Store`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/io/read/read_bam.py` & `cfdna-2.0.8/cfdna/io/read/read_bam.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/io/write/write_text.py` & `cfdna-2.0.8/cfdna/io/write/write_text.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/plot/plot_bokeh.py` & `cfdna-2.0.8/cfdna/plot/plot_bokeh.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/plot/plot_plt.py` & `cfdna-2.0.8/cfdna/plot/plot_plt.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/tools/cnv/segmentation.py` & `cfdna-2.0.8/cfdna/tools/cnv/segmentation.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/tools/coverage/gene_activity.py` & `cfdna-2.0.8/cfdna/tools/coverage/gene_activity.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/tools/fragmentation/frag_pattern.py` & `cfdna-2.0.8/cfdna/tools/fragmentation/frag_pattern.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/tools/nucleosome/gene_activity.py` & `cfdna-2.0.8/cfdna/tools/nucleosome/gene_activity.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/tools/nucleosome/nfr.py` & `cfdna-2.0.8/cfdna/tools/nucleosome/nfr.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/tools/nucleosome/relative_window.py` & `cfdna-2.0.8/cfdna/tools/nucleosome/relative_window.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/tools/nucleosome/wps_functions.py` & `cfdna-2.0.8/cfdna/tools/nucleosome/wps_functions.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/tools/summarize/multi_sample.py` & `cfdna-2.0.8/cfdna/tools/summarize/multi_sample.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/tools/summarize/summarize.py` & `cfdna-2.0.8/cfdna/tools/summarize/summarize.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/cfdna/utilities/h5_utilities.py` & `cfdna-2.0.8/cfdna/utilities/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.0.7/pyproject.toml` & `cfdna-2.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cfdna"
-version = "2.0.7"
+version = "2.0.8"
 description = "Python package for fragment manipulation for cfDNA"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/cfdna"
 documentation = "https://www.biosciencestack.com/static/cfdna/docs/index.html"
 keywords = ["cython", "interval", "cfdna", "c"]
 readme = 'README.md'
@@ -25,45 +25,45 @@
                     "Topic :: Scientific/Engineering :: Bio-Informatics"
                   ]
 packages = [{ include = "cfdna" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.23.5"
-cython = "^0.29.32"
-pandas = "^1.5.2"
-ailist = "^2.1.2"
+cython = "^3.0.0"
+pandas = "^2.0.0"
+ailist = "^2.1.3"
 linear_segment = "^1.1.0"
 pysam = "^0.21.0"
 intervalframe = "^1.1.5"
 matplotlib = "^3.7.1"
 bokeh = "^3.1.0"
 scipy = "^1.9.1"
 statsmodels = "^0.13.5"
 seaborn = "^0.12.2"
 projectframe = "^1.0.0"
 hmmCNV = "^1.0.1"
 scikit-learn = "^1.2.2"
-ngsfragments = "^2.1.5"
+ngsfragments = "^2.1.8"
 genome_info = "^1.0.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0",
-            "cython>=0.29.32",
+            "cython>=3.0.0",
             "numpy>=1.23.5",
-            "pandas>=1.5.2",
+            "pandas>=2.0.0",
             "setuptools>=65.5.0",
-            "ailist>=2.1.2",
-            "pysam>=0.20.0",
+            "ailist>=2.1.3",
+            "pysam>=0.21.0",
             "genome_info>=1.0.4",
             "intervalframe>=1.1.5",
-            "ngsfragments>=2.1.5"]
+            "ngsfragments>=2.1.8"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.build]
 generate-setup-file = false
 #script = "build.py"
 
 [tool.cibuildwheel]
```

### Comparing `cfdna-2.0.7/PKG-INFO` & `cfdna-2.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdna
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python package for fragment manipulation for cfDNA
 Home-page: https://github.com/kylessmith/cfdna
 License: GPL-2.0-or-later
 Keywords: cython,interval,cfdna,c
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
@@ -24,25 +24,25 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: ailist (>=2.1.2,<3.0.0)
+Requires-Dist: ailist (>=2.1.3,<3.0.0)
 Requires-Dist: bokeh (>=3.1.0,<4.0.0)
-Requires-Dist: cython (>=0.29.32,<0.30.0)
+Requires-Dist: cython (>=3.0.0,<4.0.0)
 Requires-Dist: genome_info (>=1.0.4,<2.0.0)
 Requires-Dist: hmmCNV (>=1.0.1,<2.0.0)
 Requires-Dist: intervalframe (>=1.1.5,<2.0.0)
 Requires-Dist: linear_segment (>=1.1.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: ngsfragments (>=2.1.5,<3.0.0)
+Requires-Dist: ngsfragments (>=2.1.8,<3.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: projectframe (>=1.0.0,<2.0.0)
 Requires-Dist: pysam (>=0.21.0,<0.22.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: statsmodels (>=0.13.5,<0.14.0)
 Project-URL: Documentation, https://www.biosciencestack.com/static/cfdna/docs/index.html
```

