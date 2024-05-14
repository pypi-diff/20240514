# Comparing `tmp/pyfmtools-5.2.tar.gz` & `tmp/pyfmtools-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfmtools-5.2.tar", last modified: Sun May 12 07:01:57 2024, max compression
+gzip compressed data, was "pyfmtools-5.2.1.tar", last modified: Tue May 14 14:01:55 2024, max compression
```

## Comparing `pyfmtools-5.2.tar` & `pyfmtools-5.2.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-12 07:01:57.307609 pyfmtools-5.2/
--rw-r--r--   0 gleb       (501) staff       (20)     7652 2022-04-26 03:16:57.000000 pyfmtools-5.2/LICENSE.txt
--rw-rw-r--   0 gleb       (501) staff       (20)      239 2024-05-08 11:29:16.000000 pyfmtools-5.2/MANIFEST.in
--rw-r--r--   0 gleb       (501) staff       (20)     5355 2024-05-12 07:01:57.307530 pyfmtools-5.2/PKG-INFO
--rw-rw-r--   0 gleb       (501) staff       (20)     5026 2022-06-20 10:01:16.000000 pyfmtools-5.2/README.md
--rw-r--r--   0 gleb       (501) staff       (20)       38 2024-05-12 07:01:57.308021 pyfmtools-5.2/setup.cfg
--rw-r--r--   0 gleb       (501) staff       (20)      946 2024-05-12 07:01:54.000000 pyfmtools-5.2/setup.py
-drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-12 07:01:57.305339 pyfmtools-5.2/src/
--rw-------   0 gleb       (501) staff       (20)     1933 2021-02-16 05:49:22.000000 pyfmtools-5.2/src/binarylattice.h
--rw-r--r--   0 gleb       (501) staff       (20)    12168 2024-05-11 02:06:23.000000 pyfmtools-5.2/src/buildPyfmtools.py
--rw-------   0 gleb       (501) staff       (20)   103132 2020-04-28 00:59:43.000000 pyfmtools-5.2/src/colamd.c
--rw-r--r--   0 gleb       (501) staff       (20)     9805 2024-04-14 06:20:55.000000 pyfmtools-5.2/src/colamd.h
--rw-r--r--   0 gleb       (501) staff       (20)    19333 2024-04-14 05:56:20.000000 pyfmtools-5.2/src/commonlib.c
--rw-r--r--   0 gleb       (501) staff       (20)     8898 2023-11-18 13:55:16.000000 pyfmtools-5.2/src/commonlib.h
--rw-------   0 gleb       (501) staff       (20)      389 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/declare.h
--rw-r--r--   0 gleb       (501) staff       (20)    26878 2024-04-25 03:30:44.000000 pyfmtools-5.2/src/fmrandom.cpp
--rw-r--r--   0 gleb       (501) staff       (20)     9046 2024-04-25 05:08:55.000000 pyfmtools-5.2/src/fmrandom.h
--rw-r--r--   0 gleb       (501) staff       (20)    53034 2024-05-08 10:01:08.000000 pyfmtools-5.2/src/fmrandomsort.inc
--rw-r--r--   0 gleb       (501) staff       (20)     7328 2023-11-18 13:41:34.000000 pyfmtools-5.2/src/fortify.h
--rw-r--r--   0 gleb       (501) staff       (20)    45535 2024-04-25 07:04:40.000000 pyfmtools-5.2/src/fuzzymeasurefit.cpp
--rw-r--r--   0 gleb       (501) staff       (20)    10737 2024-04-26 08:00:42.000000 pyfmtools-5.2/src/fuzzymeasurefit.h
--rw-r--r--   0 gleb       (501) staff       (20)    57669 2024-05-08 11:02:45.000000 pyfmtools-5.2/src/fuzzymeasurefit3.cpp
--rw-r--r--   0 gleb       (501) staff       (20)    53885 2024-05-11 10:06:35.000000 pyfmtools-5.2/src/fuzzymeasuretools.cpp
--rw-r--r--   0 gleb       (501) staff       (20)    18169 2024-05-02 11:02:46.000000 pyfmtools-5.2/src/fuzzymeasuretools.h
--rw-r--r--   0 gleb       (501) staff       (20)      500 2024-04-25 09:14:22.000000 pyfmtools-5.2/src/gbrealloc.c
--rw-r--r--   0 gleb       (501) staff       (20)     1044 2024-05-11 02:10:05.000000 pyfmtools-5.2/src/generaldefs.h
--rw-------   0 gleb       (501) staff       (20)     2822 2018-03-02 10:06:22.000000 pyfmtools-5.2/src/hbio.h
--rw-------   0 gleb       (501) staff       (20)     1216 2020-09-03 10:46:28.000000 pyfmtools-5.2/src/ini.c
--rw-------   0 gleb       (501) staff       (20)      394 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/ini.h
--rw-------   0 gleb       (501) staff       (20)      496 2020-09-15 01:44:59.000000 pyfmtools-5.2/src/isfixedvar.c
--rw-------   0 gleb       (501) staff       (20)     4588 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_BFP.h
--rw-------   0 gleb       (501) staff       (20)     5569 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_BFP1.h
--rw-r--r--   0 gleb       (501) staff       (20)     4420 2024-04-14 05:45:40.000000 pyfmtools-5.2/src/lp_BFP2.h
--rw-------   0 gleb       (501) staff       (20)     5516 2020-04-28 01:17:20.000000 pyfmtools-5.2/src/lp_Hash.c
--rw-------   0 gleb       (501) staff       (20)     1135 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_Hash.h
--rw-r--r--   0 gleb       (501) staff       (20)    23763 2024-03-24 08:42:10.000000 pyfmtools-5.2/src/lp_LUSOL.c
--rw-r--r--   0 gleb       (501) staff       (20)     2818 2024-03-24 08:42:23.000000 pyfmtools-5.2/src/lp_LUSOL.h
--rw-------   0 gleb       (501) staff       (20)     6986 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_MDO.c
--rw-------   0 gleb       (501) staff       (20)      252 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_MDO.h
--rw-r--r--   0 gleb       (501) staff       (20)    54130 2024-03-24 08:48:14.000000 pyfmtools-5.2/src/lp_MPS.c
--rw-------   0 gleb       (501) staff       (20)      926 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_MPS.h
--rw-------   0 gleb       (501) staff       (20)    40253 2020-04-28 01:17:20.000000 pyfmtools-5.2/src/lp_SOS.c
--rw-------   0 gleb       (501) staff       (20)     4627 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_SOS.h
--rw-------   0 gleb       (501) staff       (20)    12381 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_crash.c
--rw-------   0 gleb       (501) staff       (20)      484 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_crash.h
--rw-------   0 gleb       (501) staff       (20)     3916 2021-02-12 00:36:00.000000 pyfmtools-5.2/src/lp_etaPFI.h
--rw-------   0 gleb       (501) staff       (20)    47660 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_explicit.h
--rw-------   0 gleb       (501) staff       (20)       45 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_fortify.h
--rw-r--r--   0 gleb       (501) staff       (20)   286192 2024-04-14 11:30:55.000000 pyfmtools-5.2/src/lp_lib.c
--rw-------   0 gleb       (501) staff       (20)   118585 2022-05-23 02:33:57.000000 pyfmtools-5.2/src/lp_lib.h
--rw-r--r--   0 gleb       (501) staff       (20)    96482 2024-04-14 05:46:59.000000 pyfmtools-5.2/src/lp_matrix.c
--rw-------   0 gleb       (501) staff       (20)    12184 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_matrix.h
--rw-------   0 gleb       (501) staff       (20)    46309 2021-04-07 03:10:58.000000 pyfmtools-5.2/src/lp_mipbb.c
--rw-------   0 gleb       (501) staff       (20)     2128 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_mipbb.h
--rw-r--r--   0 gleb       (501) staff       (20)    23636 2023-02-01 11:29:49.000000 pyfmtools-5.2/src/lp_params.c
--rw-r--r--   0 gleb       (501) staff       (20)   184288 2023-02-01 11:29:56.000000 pyfmtools-5.2/src/lp_presolve.c
--rw-------   0 gleb       (501) staff       (20)     4190 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_presolve.h
--rw-r--r--   0 gleb       (501) staff       (20)    68814 2024-04-14 05:47:56.000000 pyfmtools-5.2/src/lp_price.c
--rw-------   0 gleb       (501) staff       (20)     5141 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_price.h
--rw-------   0 gleb       (501) staff       (20)    13780 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_pricePSE.c
--rw-------   0 gleb       (501) staff       (20)      712 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_pricePSE.h
--rw-------   0 gleb       (501) staff       (20)    24951 2020-04-28 01:15:06.000000 pyfmtools-5.2/src/lp_report.c
--rw-------   0 gleb       (501) staff       (20)     1436 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_report.h
--rw-------   0 gleb       (501) staff       (20)    51050 2021-02-12 00:36:10.000000 pyfmtools-5.2/src/lp_rlp.h
--rw-r--r--   0 gleb       (501) staff       (20)    29500 2024-04-14 05:49:01.000000 pyfmtools-5.2/src/lp_scale.c
--rw-------   0 gleb       (501) staff       (20)     1008 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_scale.h
--rw-------   0 gleb       (501) staff       (20)    75069 2020-04-28 01:17:20.000000 pyfmtools-5.2/src/lp_simplex.c
--rw-------   0 gleb       (501) staff       (20)     1057 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_simplex.h
--rw-------   0 gleb       (501) staff       (20)     9717 2020-09-08 02:31:35.000000 pyfmtools-5.2/src/lp_types.h
--rw-r--r--   0 gleb       (501) staff       (20)    26898 2024-04-14 05:50:17.000000 pyfmtools-5.2/src/lp_utils.c
--rw-------   0 gleb       (501) staff       (20)     6125 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_utils.h
--rw-r--r--   0 gleb       (501) staff       (20)    11305 2024-03-24 08:48:01.000000 pyfmtools-5.2/src/lp_wlp.c
--rw-------   0 gleb       (501) staff       (20)      294 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lp_wlp.h
--rw-------   0 gleb       (501) staff       (20)     1307 2018-03-02 10:29:08.000000 pyfmtools-5.2/src/lpkit.h
--rw-r--r--   0 gleb       (501) staff       (20)    21901 2024-04-14 05:51:50.000000 pyfmtools-5.2/src/lpslink56.c
--rw-------   0 gleb       (501) staff       (20)      778 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lpsolve.h
--rw-r--r--   0 gleb       (501) staff       (20)    25092 2023-02-01 11:24:58.000000 pyfmtools-5.2/src/lusol.c
--rw-------   0 gleb       (501) staff       (20)    14037 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lusol.h
--rw-r--r--   0 gleb       (501) staff       (20)   135888 2024-04-14 06:11:02.000000 pyfmtools-5.2/src/lusol1.h
--rw-------   0 gleb       (501) staff       (20)     6437 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lusol2.h
--rw-r--r--   0 gleb       (501) staff       (20)    28376 2024-04-14 06:10:22.000000 pyfmtools-5.2/src/lusol6a.h
--rw-r--r--   0 gleb       (501) staff       (20)     4490 2024-04-14 06:09:47.000000 pyfmtools-5.2/src/lusol6l0.h
--rw-r--r--   0 gleb       (501) staff       (20)     4891 2024-04-14 06:11:21.000000 pyfmtools-5.2/src/lusol6u.h
--rw-------   0 gleb       (501) staff       (20)    22181 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lusol7a.h
--rw-------   0 gleb       (501) staff       (20)    11175 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lusol8a.h
--rw-------   0 gleb       (501) staff       (20)     7376 2020-04-28 01:15:38.000000 pyfmtools-5.2/src/lusolio.c
--rw-------   0 gleb       (501) staff       (20)     1014 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/lusolio.h
--rw-------   0 gleb       (501) staff       (20)     7757 2020-12-16 09:23:48.000000 pyfmtools-5.2/src/minimalsplus.h
--rw-r--r--   0 gleb       (501) staff       (20)    13168 2023-02-01 11:25:41.000000 pyfmtools-5.2/src/mmio.c
--rw-------   0 gleb       (501) staff       (20)     4320 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/mmio.h
--rw-r--r--   0 gleb       (501) staff       (20)    19256 2024-04-14 05:52:37.000000 pyfmtools-5.2/src/myblas.c
--rw-------   0 gleb       (501) staff       (20)     5651 2021-02-12 08:29:12.000000 pyfmtools-5.2/src/myblas.h
-drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-12 07:01:57.307268 pyfmtools-5.2/src/pyfmtools.egg-info/
--rw-r--r--   0 gleb       (501) staff       (20)     5355 2024-05-12 07:01:57.000000 pyfmtools-5.2/src/pyfmtools.egg-info/PKG-INFO
--rw-r--r--   0 gleb       (501) staff       (20)     1712 2024-05-12 07:01:57.000000 pyfmtools-5.2/src/pyfmtools.egg-info/SOURCES.txt
--rw-r--r--   0 gleb       (501) staff       (20)        1 2024-05-12 07:01:57.000000 pyfmtools-5.2/src/pyfmtools.egg-info/dependency_links.txt
--rw-r--r--   0 gleb       (501) staff       (20)       12 2024-05-12 07:01:57.000000 pyfmtools-5.2/src/pyfmtools.egg-info/requires.txt
--rw-r--r--   0 gleb       (501) staff       (20)       21 2024-05-12 07:01:57.000000 pyfmtools-5.2/src/pyfmtools.egg-info/top_level.txt
--rw-r--r--   0 gleb       (501) staff       (20)    57619 2024-05-09 01:05:40.000000 pyfmtools-5.2/src/pyfmtools.py
--rw-------   0 gleb       (501) staff       (20)    21684 2021-04-07 03:11:24.000000 pyfmtools-5.2/src/sparselib.c
--rw-------   0 gleb       (501) staff       (20)     2975 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/sparselib.h
--rw-------   0 gleb       (501) staff       (20)      396 2020-04-28 00:33:49.000000 pyfmtools-5.2/src/stdafx.h
--rw-------   0 gleb       (501) staff       (20)     1822 2015-09-18 14:53:52.000000 pyfmtools-5.2/src/ufortify.h
--rw-r--r--   0 gleb       (501) staff       (20)    95171 2024-05-11 09:21:15.000000 pyfmtools-5.2/src/wrapperpy.cpp
--rw-r--r--   0 gleb       (501) staff       (20)    16290 2024-05-05 06:50:06.000000 pyfmtools-5.2/src/wrapperpy.h
--rw-r--r--   0 gleb       (501) staff       (20)    28420 2023-02-01 11:30:06.000000 pyfmtools-5.2/src/yacc_read.c
--rw-------   0 gleb       (501) staff       (20)      918 2017-11-28 12:18:32.000000 pyfmtools-5.2/src/yacc_read.h
-drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-12 07:01:57.306963 pyfmtools-5.2/tests/
--rw-------   0 gleb       (501) staff       (20)     3508 2022-05-24 07:38:34.000000 pyfmtools-5.2/tests/test_no_wrapper.py
--rw-r--r--   0 gleb       (501) staff       (20)    33368 2024-05-11 10:33:11.000000 pyfmtools-5.2/tests/test_wrapper.py
+drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-14 14:01:55.795413 pyfmtools-5.2.1/
+-rw-r--r--   0 gleb       (501) staff       (20)     7652 2022-04-26 03:16:57.000000 pyfmtools-5.2.1/LICENSE.txt
+-rw-rw-r--   0 gleb       (501) staff       (20)      239 2024-05-08 11:29:16.000000 pyfmtools-5.2.1/MANIFEST.in
+-rw-r--r--   0 gleb       (501) staff       (20)     5357 2024-05-14 14:01:55.795346 pyfmtools-5.2.1/PKG-INFO
+-rw-rw-r--   0 gleb       (501) staff       (20)     5026 2022-06-20 10:01:16.000000 pyfmtools-5.2.1/README.md
+-rw-r--r--   0 gleb       (501) staff       (20)       38 2024-05-14 14:01:55.795853 pyfmtools-5.2.1/setup.cfg
+-rw-r--r--   0 gleb       (501) staff       (20)      948 2024-05-14 14:01:46.000000 pyfmtools-5.2.1/setup.py
+drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-14 14:01:55.793108 pyfmtools-5.2.1/src/
+-rw-------   0 gleb       (501) staff       (20)     1933 2021-02-16 05:49:22.000000 pyfmtools-5.2.1/src/binarylattice.h
+-rw-r--r--   0 gleb       (501) staff       (20)    12168 2024-05-11 02:06:23.000000 pyfmtools-5.2.1/src/buildPyfmtools.py
+-rw-------   0 gleb       (501) staff       (20)   103132 2020-04-28 00:59:43.000000 pyfmtools-5.2.1/src/colamd.c
+-rw-r--r--   0 gleb       (501) staff       (20)     9805 2024-04-14 06:20:55.000000 pyfmtools-5.2.1/src/colamd.h
+-rw-r--r--   0 gleb       (501) staff       (20)    19333 2024-04-14 05:56:20.000000 pyfmtools-5.2.1/src/commonlib.c
+-rw-r--r--   0 gleb       (501) staff       (20)     8898 2023-11-18 13:55:16.000000 pyfmtools-5.2.1/src/commonlib.h
+-rw-------   0 gleb       (501) staff       (20)      389 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/declare.h
+-rw-r--r--   0 gleb       (501) staff       (20)    26878 2024-04-25 03:30:44.000000 pyfmtools-5.2.1/src/fmrandom.cpp
+-rw-r--r--   0 gleb       (501) staff       (20)     9046 2024-04-25 05:08:55.000000 pyfmtools-5.2.1/src/fmrandom.h
+-rw-r--r--   0 gleb       (501) staff       (20)    53038 2024-05-14 13:51:32.000000 pyfmtools-5.2.1/src/fmrandomsort.inc
+-rw-r--r--   0 gleb       (501) staff       (20)     7328 2023-11-18 13:41:34.000000 pyfmtools-5.2.1/src/fortify.h
+-rw-r--r--   0 gleb       (501) staff       (20)    45535 2024-04-25 07:04:40.000000 pyfmtools-5.2.1/src/fuzzymeasurefit.cpp
+-rw-r--r--   0 gleb       (501) staff       (20)    10737 2024-04-26 08:00:42.000000 pyfmtools-5.2.1/src/fuzzymeasurefit.h
+-rw-r--r--   0 gleb       (501) staff       (20)    57669 2024-05-08 11:02:45.000000 pyfmtools-5.2.1/src/fuzzymeasurefit3.cpp
+-rw-r--r--   0 gleb       (501) staff       (20)    53885 2024-05-11 10:06:35.000000 pyfmtools-5.2.1/src/fuzzymeasuretools.cpp
+-rw-r--r--   0 gleb       (501) staff       (20)    18169 2024-05-02 11:02:46.000000 pyfmtools-5.2.1/src/fuzzymeasuretools.h
+-rw-r--r--   0 gleb       (501) staff       (20)      500 2024-04-25 09:14:22.000000 pyfmtools-5.2.1/src/gbrealloc.c
+-rw-r--r--   0 gleb       (501) staff       (20)     1044 2024-05-11 02:10:05.000000 pyfmtools-5.2.1/src/generaldefs.h
+-rw-------   0 gleb       (501) staff       (20)     2822 2018-03-02 10:06:22.000000 pyfmtools-5.2.1/src/hbio.h
+-rw-------   0 gleb       (501) staff       (20)     1216 2020-09-03 10:46:28.000000 pyfmtools-5.2.1/src/ini.c
+-rw-------   0 gleb       (501) staff       (20)      394 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/ini.h
+-rw-------   0 gleb       (501) staff       (20)      496 2020-09-15 01:44:59.000000 pyfmtools-5.2.1/src/isfixedvar.c
+-rw-------   0 gleb       (501) staff       (20)     4588 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_BFP.h
+-rw-------   0 gleb       (501) staff       (20)     5569 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_BFP1.h
+-rw-r--r--   0 gleb       (501) staff       (20)     4420 2024-04-14 05:45:40.000000 pyfmtools-5.2.1/src/lp_BFP2.h
+-rw-------   0 gleb       (501) staff       (20)     5516 2020-04-28 01:17:20.000000 pyfmtools-5.2.1/src/lp_Hash.c
+-rw-------   0 gleb       (501) staff       (20)     1135 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_Hash.h
+-rw-r--r--   0 gleb       (501) staff       (20)    23763 2024-03-24 08:42:10.000000 pyfmtools-5.2.1/src/lp_LUSOL.c
+-rw-r--r--   0 gleb       (501) staff       (20)     2818 2024-03-24 08:42:23.000000 pyfmtools-5.2.1/src/lp_LUSOL.h
+-rw-------   0 gleb       (501) staff       (20)     6986 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_MDO.c
+-rw-------   0 gleb       (501) staff       (20)      252 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_MDO.h
+-rw-r--r--   0 gleb       (501) staff       (20)    54130 2024-03-24 08:48:14.000000 pyfmtools-5.2.1/src/lp_MPS.c
+-rw-------   0 gleb       (501) staff       (20)      926 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_MPS.h
+-rw-------   0 gleb       (501) staff       (20)    40253 2020-04-28 01:17:20.000000 pyfmtools-5.2.1/src/lp_SOS.c
+-rw-------   0 gleb       (501) staff       (20)     4627 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_SOS.h
+-rw-------   0 gleb       (501) staff       (20)    12381 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_crash.c
+-rw-------   0 gleb       (501) staff       (20)      484 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_crash.h
+-rw-------   0 gleb       (501) staff       (20)     3916 2021-02-12 00:36:00.000000 pyfmtools-5.2.1/src/lp_etaPFI.h
+-rw-------   0 gleb       (501) staff       (20)    47660 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_explicit.h
+-rw-------   0 gleb       (501) staff       (20)       45 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_fortify.h
+-rw-r--r--   0 gleb       (501) staff       (20)   286192 2024-04-14 11:30:55.000000 pyfmtools-5.2.1/src/lp_lib.c
+-rw-------   0 gleb       (501) staff       (20)   118585 2022-05-23 02:33:57.000000 pyfmtools-5.2.1/src/lp_lib.h
+-rw-r--r--   0 gleb       (501) staff       (20)    96482 2024-04-14 05:46:59.000000 pyfmtools-5.2.1/src/lp_matrix.c
+-rw-------   0 gleb       (501) staff       (20)    12184 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_matrix.h
+-rw-------   0 gleb       (501) staff       (20)    46309 2021-04-07 03:10:58.000000 pyfmtools-5.2.1/src/lp_mipbb.c
+-rw-------   0 gleb       (501) staff       (20)     2128 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_mipbb.h
+-rw-r--r--   0 gleb       (501) staff       (20)    23636 2023-02-01 11:29:49.000000 pyfmtools-5.2.1/src/lp_params.c
+-rw-r--r--   0 gleb       (501) staff       (20)   184288 2023-02-01 11:29:56.000000 pyfmtools-5.2.1/src/lp_presolve.c
+-rw-------   0 gleb       (501) staff       (20)     4190 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_presolve.h
+-rw-r--r--   0 gleb       (501) staff       (20)    68814 2024-04-14 05:47:56.000000 pyfmtools-5.2.1/src/lp_price.c
+-rw-------   0 gleb       (501) staff       (20)     5141 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_price.h
+-rw-------   0 gleb       (501) staff       (20)    13780 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_pricePSE.c
+-rw-------   0 gleb       (501) staff       (20)      712 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_pricePSE.h
+-rw-------   0 gleb       (501) staff       (20)    24951 2020-04-28 01:15:06.000000 pyfmtools-5.2.1/src/lp_report.c
+-rw-------   0 gleb       (501) staff       (20)     1436 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_report.h
+-rw-------   0 gleb       (501) staff       (20)    51050 2021-02-12 00:36:10.000000 pyfmtools-5.2.1/src/lp_rlp.h
+-rw-r--r--   0 gleb       (501) staff       (20)    29500 2024-04-14 05:49:01.000000 pyfmtools-5.2.1/src/lp_scale.c
+-rw-------   0 gleb       (501) staff       (20)     1008 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_scale.h
+-rw-------   0 gleb       (501) staff       (20)    75069 2020-04-28 01:17:20.000000 pyfmtools-5.2.1/src/lp_simplex.c
+-rw-------   0 gleb       (501) staff       (20)     1057 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_simplex.h
+-rw-------   0 gleb       (501) staff       (20)     9717 2020-09-08 02:31:35.000000 pyfmtools-5.2.1/src/lp_types.h
+-rw-r--r--   0 gleb       (501) staff       (20)    26898 2024-04-14 05:50:17.000000 pyfmtools-5.2.1/src/lp_utils.c
+-rw-------   0 gleb       (501) staff       (20)     6125 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_utils.h
+-rw-r--r--   0 gleb       (501) staff       (20)    11305 2024-03-24 08:48:01.000000 pyfmtools-5.2.1/src/lp_wlp.c
+-rw-------   0 gleb       (501) staff       (20)      294 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lp_wlp.h
+-rw-------   0 gleb       (501) staff       (20)     1307 2018-03-02 10:29:08.000000 pyfmtools-5.2.1/src/lpkit.h
+-rw-r--r--   0 gleb       (501) staff       (20)    21901 2024-04-14 05:51:50.000000 pyfmtools-5.2.1/src/lpslink56.c
+-rw-------   0 gleb       (501) staff       (20)      778 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lpsolve.h
+-rw-r--r--   0 gleb       (501) staff       (20)    25092 2023-02-01 11:24:58.000000 pyfmtools-5.2.1/src/lusol.c
+-rw-------   0 gleb       (501) staff       (20)    14037 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lusol.h
+-rw-r--r--   0 gleb       (501) staff       (20)   135888 2024-04-14 06:11:02.000000 pyfmtools-5.2.1/src/lusol1.h
+-rw-------   0 gleb       (501) staff       (20)     6437 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lusol2.h
+-rw-r--r--   0 gleb       (501) staff       (20)    28376 2024-04-14 06:10:22.000000 pyfmtools-5.2.1/src/lusol6a.h
+-rw-r--r--   0 gleb       (501) staff       (20)     4490 2024-04-14 06:09:47.000000 pyfmtools-5.2.1/src/lusol6l0.h
+-rw-r--r--   0 gleb       (501) staff       (20)     4891 2024-04-14 06:11:21.000000 pyfmtools-5.2.1/src/lusol6u.h
+-rw-------   0 gleb       (501) staff       (20)    22181 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lusol7a.h
+-rw-------   0 gleb       (501) staff       (20)    11175 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lusol8a.h
+-rw-------   0 gleb       (501) staff       (20)     7376 2020-04-28 01:15:38.000000 pyfmtools-5.2.1/src/lusolio.c
+-rw-------   0 gleb       (501) staff       (20)     1014 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/lusolio.h
+-rw-------   0 gleb       (501) staff       (20)     7757 2020-12-16 09:23:48.000000 pyfmtools-5.2.1/src/minimalsplus.h
+-rw-r--r--   0 gleb       (501) staff       (20)    13168 2023-02-01 11:25:41.000000 pyfmtools-5.2.1/src/mmio.c
+-rw-------   0 gleb       (501) staff       (20)     4320 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/mmio.h
+-rw-r--r--   0 gleb       (501) staff       (20)    19256 2024-04-14 05:52:37.000000 pyfmtools-5.2.1/src/myblas.c
+-rw-------   0 gleb       (501) staff       (20)     5651 2021-02-12 08:29:12.000000 pyfmtools-5.2.1/src/myblas.h
+drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-14 14:01:55.795069 pyfmtools-5.2.1/src/pyfmtools.egg-info/
+-rw-r--r--   0 gleb       (501) staff       (20)     5357 2024-05-14 14:01:55.000000 pyfmtools-5.2.1/src/pyfmtools.egg-info/PKG-INFO
+-rw-r--r--   0 gleb       (501) staff       (20)     1712 2024-05-14 14:01:55.000000 pyfmtools-5.2.1/src/pyfmtools.egg-info/SOURCES.txt
+-rw-r--r--   0 gleb       (501) staff       (20)        1 2024-05-14 14:01:55.000000 pyfmtools-5.2.1/src/pyfmtools.egg-info/dependency_links.txt
+-rw-r--r--   0 gleb       (501) staff       (20)       12 2024-05-14 14:01:55.000000 pyfmtools-5.2.1/src/pyfmtools.egg-info/requires.txt
+-rw-r--r--   0 gleb       (501) staff       (20)       21 2024-05-14 14:01:55.000000 pyfmtools-5.2.1/src/pyfmtools.egg-info/top_level.txt
+-rw-r--r--   0 gleb       (501) staff       (20)    57619 2024-05-09 01:05:40.000000 pyfmtools-5.2.1/src/pyfmtools.py
+-rw-------   0 gleb       (501) staff       (20)    21684 2021-04-07 03:11:24.000000 pyfmtools-5.2.1/src/sparselib.c
+-rw-------   0 gleb       (501) staff       (20)     2975 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/sparselib.h
+-rw-------   0 gleb       (501) staff       (20)      396 2020-04-28 00:33:49.000000 pyfmtools-5.2.1/src/stdafx.h
+-rw-------   0 gleb       (501) staff       (20)     1822 2015-09-18 14:53:52.000000 pyfmtools-5.2.1/src/ufortify.h
+-rw-r--r--   0 gleb       (501) staff       (20)    95755 2024-05-11 13:48:58.000000 pyfmtools-5.2.1/src/wrapperpy.cpp
+-rw-r--r--   0 gleb       (501) staff       (20)    16290 2024-05-05 06:50:06.000000 pyfmtools-5.2.1/src/wrapperpy.h
+-rw-r--r--   0 gleb       (501) staff       (20)    28420 2023-02-01 11:30:06.000000 pyfmtools-5.2.1/src/yacc_read.c
+-rw-------   0 gleb       (501) staff       (20)      918 2017-11-28 12:18:32.000000 pyfmtools-5.2.1/src/yacc_read.h
+drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-14 14:01:55.794749 pyfmtools-5.2.1/tests/
+-rw-------   0 gleb       (501) staff       (20)     3508 2022-05-24 07:38:34.000000 pyfmtools-5.2.1/tests/test_no_wrapper.py
+-rw-r--r--   0 gleb       (501) staff       (20)    33368 2024-05-11 10:33:11.000000 pyfmtools-5.2.1/tests/test_wrapper.py
```

### Comparing `pyfmtools-5.2/LICENSE.txt` & `pyfmtools-5.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/PKG-INFO` & `pyfmtools-5.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmtools
-Version: 5.2
+Version: 5.2.1
 Summary: Library for handling and fitting fuzzy measures
 Home-page: 
 Author: Gleb Beliakov, Norbert Henseler
 Author-email: gleb.beliakov@deakin.edu.au, norbert.henseler@deakin.edu.au
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: cffi>=1.0.0
```

### Comparing `pyfmtools-5.2/README.md` & `pyfmtools-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/setup.py` & `pyfmtools-5.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup( 
     name="pyfmtools",
-    version="5.2",
+    version="5.2.1",
     description="Library for handling and fitting fuzzy measures",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="",
     author='Gleb Beliakov, Norbert Henseler',
     author_email='gleb.beliakov@deakin.edu.au, norbert.henseler@deakin.edu.au',
     license_file='LICENSE.txt',
```

### Comparing `pyfmtools-5.2/src/binarylattice.h` & `pyfmtools-5.2.1/src/binarylattice.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/buildPyfmtools.py` & `pyfmtools-5.2.1/src/buildPyfmtools.py`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/colamd.c` & `pyfmtools-5.2.1/src/colamd.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/colamd.h` & `pyfmtools-5.2.1/src/colamd.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/commonlib.c` & `pyfmtools-5.2.1/src/commonlib.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/commonlib.h` & `pyfmtools-5.2.1/src/commonlib.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/fmrandom.cpp` & `pyfmtools-5.2.1/src/fmrandom.cpp`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/fmrandom.h` & `pyfmtools-5.2.1/src/fmrandom.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/fmrandomsort.inc` & `pyfmtools-5.2.1/src/fmrandomsort.inc`

 * *Files 0% similar despite different names*

```diff
@@ -1225,19 +1225,19 @@
 {
 	if (kadd < n - 1)
 		*length = fm_arraysize_kadd(n, kadd);
 	else *length = 0x1ULL << n; 
 
 	vector<double> v1(*length);
 	for (int_64 k = 0; k < num; k++) {
-		GenerateBeliefMob(n, *length, v1); // in Mobius! with no 0
+		GenerateBeliefMob(n, *length-1, v1); // in Mobius! with no 0
 		
 		vv[0+ (*length)*k] = 0;
 
-		for (int i = 0; i < *length; i++)
+		for (int i = 0; i < *length-1; i++)
 			vv[i + 1 + (*length) * k] = v1[i]; // last one?
 	}
 	return 1;
 }
 
 LIBDLL_API int generate_fm_balanced(int_64 num, int n, double* vv)
 {
```

### Comparing `pyfmtools-5.2/src/fortify.h` & `pyfmtools-5.2.1/src/fortify.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/fuzzymeasurefit.cpp` & `pyfmtools-5.2.1/src/fuzzymeasurefit.cpp`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/fuzzymeasurefit.h` & `pyfmtools-5.2.1/src/fuzzymeasurefit.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/fuzzymeasurefit3.cpp` & `pyfmtools-5.2.1/src/fuzzymeasurefit3.cpp`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/fuzzymeasuretools.cpp` & `pyfmtools-5.2.1/src/fuzzymeasuretools.cpp`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/fuzzymeasuretools.h` & `pyfmtools-5.2.1/src/fuzzymeasuretools.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/generaldefs.h` & `pyfmtools-5.2.1/src/generaldefs.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/hbio.h` & `pyfmtools-5.2.1/src/hbio.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/ini.c` & `pyfmtools-5.2.1/src/ini.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_BFP.h` & `pyfmtools-5.2.1/src/lp_BFP.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_BFP1.h` & `pyfmtools-5.2.1/src/lp_BFP1.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_BFP2.h` & `pyfmtools-5.2.1/src/lp_BFP2.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_Hash.c` & `pyfmtools-5.2.1/src/lp_Hash.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_Hash.h` & `pyfmtools-5.2.1/src/lp_Hash.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_LUSOL.c` & `pyfmtools-5.2.1/src/lp_LUSOL.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_LUSOL.h` & `pyfmtools-5.2.1/src/lp_LUSOL.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_MDO.c` & `pyfmtools-5.2.1/src/lp_MDO.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_MPS.c` & `pyfmtools-5.2.1/src/lp_MPS.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_MPS.h` & `pyfmtools-5.2.1/src/lp_MPS.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_SOS.c` & `pyfmtools-5.2.1/src/lp_SOS.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_SOS.h` & `pyfmtools-5.2.1/src/lp_SOS.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_crash.c` & `pyfmtools-5.2.1/src/lp_crash.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_etaPFI.h` & `pyfmtools-5.2.1/src/lp_etaPFI.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_explicit.h` & `pyfmtools-5.2.1/src/lp_explicit.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_lib.c` & `pyfmtools-5.2.1/src/lp_lib.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_lib.h` & `pyfmtools-5.2.1/src/lp_lib.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_matrix.c` & `pyfmtools-5.2.1/src/lp_matrix.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_matrix.h` & `pyfmtools-5.2.1/src/lp_matrix.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_mipbb.c` & `pyfmtools-5.2.1/src/lp_mipbb.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_mipbb.h` & `pyfmtools-5.2.1/src/lp_mipbb.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_params.c` & `pyfmtools-5.2.1/src/lp_params.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_presolve.c` & `pyfmtools-5.2.1/src/lp_presolve.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_presolve.h` & `pyfmtools-5.2.1/src/lp_presolve.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_price.c` & `pyfmtools-5.2.1/src/lp_price.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_price.h` & `pyfmtools-5.2.1/src/lp_price.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_pricePSE.c` & `pyfmtools-5.2.1/src/lp_pricePSE.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_pricePSE.h` & `pyfmtools-5.2.1/src/lp_pricePSE.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_report.c` & `pyfmtools-5.2.1/src/lp_report.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_report.h` & `pyfmtools-5.2.1/src/lp_report.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_rlp.h` & `pyfmtools-5.2.1/src/lp_rlp.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_scale.c` & `pyfmtools-5.2.1/src/lp_scale.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_scale.h` & `pyfmtools-5.2.1/src/lp_scale.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_simplex.c` & `pyfmtools-5.2.1/src/lp_simplex.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_simplex.h` & `pyfmtools-5.2.1/src/lp_simplex.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_types.h` & `pyfmtools-5.2.1/src/lp_types.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_utils.c` & `pyfmtools-5.2.1/src/lp_utils.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_utils.h` & `pyfmtools-5.2.1/src/lp_utils.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lp_wlp.c` & `pyfmtools-5.2.1/src/lp_wlp.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lpkit.h` & `pyfmtools-5.2.1/src/lpkit.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lpslink56.c` & `pyfmtools-5.2.1/src/lpslink56.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lpsolve.h` & `pyfmtools-5.2.1/src/lpsolve.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lusol.c` & `pyfmtools-5.2.1/src/lusol.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lusol.h` & `pyfmtools-5.2.1/src/lusol.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lusol1.h` & `pyfmtools-5.2.1/src/lusol1.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lusol2.h` & `pyfmtools-5.2.1/src/lusol2.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lusol6a.h` & `pyfmtools-5.2.1/src/lusol6a.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lusol6l0.h` & `pyfmtools-5.2.1/src/lusol6l0.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lusol6u.h` & `pyfmtools-5.2.1/src/lusol6u.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lusol7a.h` & `pyfmtools-5.2.1/src/lusol7a.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lusol8a.h` & `pyfmtools-5.2.1/src/lusol8a.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lusolio.c` & `pyfmtools-5.2.1/src/lusolio.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/lusolio.h` & `pyfmtools-5.2.1/src/lusolio.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/minimalsplus.h` & `pyfmtools-5.2.1/src/minimalsplus.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/mmio.c` & `pyfmtools-5.2.1/src/mmio.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/mmio.h` & `pyfmtools-5.2.1/src/mmio.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/myblas.c` & `pyfmtools-5.2.1/src/myblas.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/myblas.h` & `pyfmtools-5.2.1/src/myblas.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/pyfmtools.egg-info/PKG-INFO` & `pyfmtools-5.2.1/src/pyfmtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmtools
-Version: 5.2
+Version: 5.2.1
 Summary: Library for handling and fitting fuzzy measures
 Home-page: 
 Author: Gleb Beliakov, Norbert Henseler
 Author-email: gleb.beliakov@deakin.edu.au, norbert.henseler@deakin.edu.au
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: cffi>=1.0.0
```

### Comparing `pyfmtools-5.2/src/pyfmtools.egg-info/SOURCES.txt` & `pyfmtools-5.2.1/src/pyfmtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/pyfmtools.py` & `pyfmtools-5.2.1/src/pyfmtools.py`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/sparselib.c` & `pyfmtools-5.2.1/src/sparselib.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/sparselib.h` & `pyfmtools-5.2.1/src/sparselib.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/ufortify.h` & `pyfmtools-5.2.1/src/ufortify.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/wrapperpy.cpp` & `pyfmtools-5.2.1/src/wrapperpy.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,19 @@
     return static_cast<MyDerivedClass &>(*vectorPtr).assignnullarray();		
  //  vectorPtr->__begin_ = vectorPtr->__end_ =  vectorPtr->__end_cap()= NULL;
 }
 */
 #endif
 
 #else
+	
+#if ( _MSC_VER>1)
+#include <crtversion.h>
+#endif
+#if (_VC_CRT_MAJOR_VERSION<13)
 
 template <class T>
 void wrapArrayInVector( T *sourceArray, size_t arraySize, std::vector<T,  std::allocator<T> > volatile &targetVector ) {
   typename std::_Vector_base<T, std::allocator<T> >::_Vector_impl *vectorPtr =
     (typename std::_Vector_base<T, std::allocator<T> >::_Vector_impl *)((void *) &targetVector);
   vectorPtr->_M_start = sourceArray;
   vectorPtr->_M_finish = vectorPtr->_M_end_of_storage = vectorPtr->_M_start + arraySize;
@@ -169,14 +174,31 @@
 
 template <class T>
 void releaseVectorWrapper( std::vector<T,  std::allocator<T> > volatile &targetVector ) {
   typename std::_Vector_base<T, std::allocator<T> >::_Vector_impl *vectorPtr =
         (typename std::_Vector_base<T, std::allocator<T> >::_Vector_impl *)((void *) &targetVector);
   vectorPtr->_M_start = vectorPtr->_M_finish = vectorPtr->_M_end_of_storage = NULL;
 }
+#else
+	// just copy
+template <class T>
+void wrapArrayInVector( T *sourceArray, size_t arraySize, std::vector<T,  std::allocator<T> > volatile &targetVector ) {
+  typename std::vector<T, std::allocator<T> > *vectorPtr =
+    (typename std::vector<T, std::allocator<T> > *)((void *) &targetVector);
+	
+	vectorPtr->assign(sourceArray, sourceArray+ arraySize);
+}
+template <class T>
+void releaseVectorWrapper( std::vector<T,  std::allocator<T> > volatile &targetVector )
+{
+	// do nothing 
+	return ;
+}
+#endif
+
 #endif
 
 #endif
 
 //#undef PYTHON_
 
 extern "C" {
```

### Comparing `pyfmtools-5.2/src/wrapperpy.h` & `pyfmtools-5.2.1/src/wrapperpy.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/yacc_read.c` & `pyfmtools-5.2.1/src/yacc_read.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/src/yacc_read.h` & `pyfmtools-5.2.1/src/yacc_read.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/tests/test_no_wrapper.py` & `pyfmtools-5.2.1/tests/test_no_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyfmtools-5.2/tests/test_wrapper.py` & `pyfmtools-5.2.1/tests/test_wrapper.py`

 * *Files identical despite different names*

