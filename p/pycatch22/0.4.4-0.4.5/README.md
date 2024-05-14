# Comparing `tmp/pycatch22-0.4.4.tar.gz` & `tmp/pycatch22-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatch22-0.4.4.tar", last modified: Mon Oct 16 02:38:42 2023, max compression
+gzip compressed data, was "pycatch22-0.4.5.tar", last modified: Tue May 14 04:59:33 2024, max compression
```

## Comparing `pycatch22-0.4.4.tar` & `pycatch22-0.4.5.tar`

### file list

```diff
@@ -1,69 +1,68 @@
-drwxr-xr-x   0 benfulcher   (501) staff       (20)        0 2023-10-16 02:38:42.656275 pycatch22-0.4.4/
--rw-r--r--   0 benfulcher   (501) staff       (20)    35147 2018-12-09 23:20:38.000000 pycatch22-0.4.4/LICENSE
--rw-r--r--   0 benfulcher   (501) staff       (20)       10 2022-07-06 02:16:17.000000 pycatch22-0.4.4/MANIFEST.in
--rw-r--r--   0 benfulcher   (501) staff       (20)     5120 2023-10-16 02:38:42.656039 pycatch22-0.4.4/PKG-INFO
--rw-r--r--   0 benfulcher   (501) staff       (20)     4417 2023-10-16 01:32:12.000000 pycatch22-0.4.4/README.md
--rw-r--r--   0 benfulcher   (501) staff       (20)      805 2023-10-16 02:36:54.000000 pycatch22-0.4.4/pyproject.toml
--rw-r--r--   0 benfulcher   (501) staff       (20)       38 2023-10-16 02:38:42.656317 pycatch22-0.4.4/setup.cfg
--rw-r--r--   0 benfulcher   (501) staff       (20)      800 2023-03-10 00:22:35.000000 pycatch22-0.4.4/setup.py
-drwxr-xr-x   0 benfulcher   (501) staff       (20)        0 2023-10-16 02:38:42.646028 pycatch22-0.4.4/src/
--rw-r--r--   0 benfulcher   (501) staff       (20)     6148 2022-07-11 00:17:34.000000 pycatch22-0.4.4/src/.DS_Store
-drwxr-xr-x   0 benfulcher   (501) staff       (20)        0 2023-10-16 02:38:42.653951 pycatch22-0.4.4/src/C/
--rw-r--r--   0 benfulcher   (501) staff       (20)    12945 2022-07-08 06:59:48.000000 pycatch22-0.4.4/src/C/CO_AutoCorr.c
--rw-r--r--   0 benfulcher   (501) staff       (20)     1189 2022-07-08 06:59:48.000000 pycatch22-0.4.4/src/C/CO_AutoCorr.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     2132 2019-08-10 09:05:23.000000 pycatch22-0.4.4/src/C/DN_HistogramMode_10.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      191 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/DN_HistogramMode_10.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     2717 2019-08-10 09:05:23.000000 pycatch22-0.4.4/src/C/DN_HistogramMode_5.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      188 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/DN_HistogramMode_5.h
--rw-r--r--   0 benfulcher   (501) staff       (20)      184 2022-07-08 06:59:48.000000 pycatch22-0.4.4/src/C/DN_Mean.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      187 2022-07-08 06:59:48.000000 pycatch22-0.4.4/src/C/DN_Mean.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     5054 2020-06-17 01:14:39.000000 pycatch22-0.4.4/src/C/DN_OutlierInclude.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      500 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/DN_OutlierInclude.h
--rw-r--r--   0 benfulcher   (501) staff       (20)      271 2022-07-08 06:59:48.000000 pycatch22-0.4.4/src/C/DN_Spread_Std.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      208 2022-07-08 06:59:48.000000 pycatch22-0.4.4/src/C/DN_Spread_Std.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     3772 2019-08-10 09:05:23.000000 pycatch22-0.4.4/src/C/FC_LocalSimple.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      766 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/FC_LocalSimple.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     1273 2019-08-10 09:05:23.000000 pycatch22-0.4.4/src/C/IN_AutoMutualInfoStats.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      381 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/IN_AutoMutualInfoStats.h
--rw-r--r--   0 benfulcher   (501) staff       (20)      715 2019-08-10 09:05:23.000000 pycatch22-0.4.4/src/C/MD_hrv.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      298 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/MD_hrv.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     3651 2019-08-10 09:05:23.000000 pycatch22-0.4.4/src/C/PD_PeriodicityWang.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      348 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/PD_PeriodicityWang.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     1958 2019-08-10 09:05:23.000000 pycatch22-0.4.4/src/C/SB_BinaryStats.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      424 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/SB_BinaryStats.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     1070 2020-06-17 01:14:39.000000 pycatch22-0.4.4/src/C/SB_CoarseGrain.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      301 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/SB_CoarseGrain.h
--rw-r--r--   0 benfulcher   (501) staff       (20)    12842 2022-07-08 06:59:48.000000 pycatch22-0.4.4/src/C/SB_MotifThree.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      325 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/SB_MotifThree.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     3472 2019-08-10 09:05:23.000000 pycatch22-0.4.4/src/C/SB_TransitionMatrix.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      291 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/SB_TransitionMatrix.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     8854 2020-06-17 01:14:39.000000 pycatch22-0.4.4/src/C/SC_FluctAnal.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      413 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/SC_FluctAnal.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     5022 2021-03-23 03:27:21.000000 pycatch22-0.4.4/src/C/SP_Summaries.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      435 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/SP_Summaries.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     7630 2020-06-17 01:14:39.000000 pycatch22-0.4.4/src/C/butterworth.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      288 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/butterworth.h
--rw-r--r--   0 benfulcher   (501) staff       (20)    11538 2022-07-08 06:59:48.000000 pycatch22-0.4.4/src/C/catch22_wrap.c
--rw-r--r--   0 benfulcher   (501) staff       (20)     1473 2021-03-23 03:27:21.000000 pycatch22-0.4.4/src/C/fft.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      646 2020-06-17 01:14:39.000000 pycatch22-0.4.4/src/C/fft.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     4246 2021-03-23 03:27:21.000000 pycatch22-0.4.4/src/C/helper_functions.c
--rw-r--r--   0 benfulcher   (501) staff       (20)     1044 2020-06-17 01:14:39.000000 pycatch22-0.4.4/src/C/helper_functions.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     4335 2020-06-17 01:14:39.000000 pycatch22-0.4.4/src/C/histcounts.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      778 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/histcounts.h
--rw-r--r--   0 benfulcher   (501) staff       (20)    13510 2022-07-08 06:59:48.000000 pycatch22-0.4.4/src/C/main.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      303 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/main.h
--rwxr-xr-x   0 benfulcher   (501) staff       (20)     1708 2022-07-08 06:59:48.000000 pycatch22-0.4.4/src/C/runAllTS.sh
--rw-r--r--   0 benfulcher   (501) staff       (20)    19700 2020-06-17 01:14:39.000000 pycatch22-0.4.4/src/C/splinefit.c
--rw-r--r--   0 benfulcher   (501) staff       (20)      309 2018-12-09 23:20:38.000000 pycatch22-0.4.4/src/C/splinefit.h
--rw-r--r--   0 benfulcher   (501) staff       (20)     5906 2020-06-17 01:14:39.000000 pycatch22-0.4.4/src/C/stats.c
--rw-r--r--   0 benfulcher   (501) staff       (20)     1421 2020-06-17 01:14:39.000000 pycatch22-0.4.4/src/C/stats.h
-drwxr-xr-x   0 benfulcher   (501) staff       (20)        0 2023-10-16 02:38:42.654308 pycatch22-0.4.4/src/pycatch22/
--rw-r--r--   0 benfulcher   (501) staff       (20)       57 2019-01-31 23:04:36.000000 pycatch22-0.4.4/src/pycatch22/__init__.py
--rw-r--r--   0 benfulcher   (501) staff       (20)     2498 2023-10-16 01:31:37.000000 pycatch22-0.4.4/src/pycatch22/catch22.py
-drwxr-xr-x   0 benfulcher   (501) staff       (20)        0 2023-10-16 02:38:42.655447 pycatch22-0.4.4/src/pycatch22.egg-info/
--rw-r--r--   0 benfulcher   (501) staff       (20)     5120 2023-10-16 02:38:42.000000 pycatch22-0.4.4/src/pycatch22.egg-info/PKG-INFO
--rw-r--r--   0 benfulcher   (501) staff       (20)     1310 2023-10-16 02:38:42.000000 pycatch22-0.4.4/src/pycatch22.egg-info/SOURCES.txt
--rw-r--r--   0 benfulcher   (501) staff       (20)        1 2023-10-16 02:38:42.000000 pycatch22-0.4.4/src/pycatch22.egg-info/dependency_links.txt
--rw-r--r--   0 benfulcher   (501) staff       (20)       20 2023-10-16 02:38:42.000000 pycatch22-0.4.4/src/pycatch22.egg-info/top_level.txt
-drwxr-xr-x   0 benfulcher   (501) staff       (20)        0 2023-10-16 02:38:42.655573 pycatch22-0.4.4/tests/
--rw-r--r--   0 benfulcher   (501) staff       (20)      939 2023-10-16 01:31:37.000000 pycatch22-0.4.4/tests/testing.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-14 04:59:33.856344 pycatch22-0.4.5/
+-rw-r--r--   0 joshua     (501) staff       (20)    35147 2024-05-14 01:49:12.000000 pycatch22-0.4.5/LICENSE
+-rw-r--r--   0 joshua     (501) staff       (20)       10 2024-05-14 01:49:12.000000 pycatch22-0.4.5/MANIFEST.in
+-rw-r--r--   0 joshua     (501) staff       (20)     5529 2024-05-14 04:59:33.856070 pycatch22-0.4.5/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     4826 2024-05-14 01:49:12.000000 pycatch22-0.4.5/README.md
+-rw-r--r--   0 joshua     (501) staff       (20)      805 2024-05-14 01:51:01.000000 pycatch22-0.4.5/pyproject.toml
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2024-05-14 04:59:33.856411 pycatch22-0.4.5/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)      896 2024-05-14 04:46:39.000000 pycatch22-0.4.5/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-14 04:59:33.839312 pycatch22-0.4.5/src/
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-14 04:59:33.853779 pycatch22-0.4.5/src/C/
+-rw-r--r--   0 joshua     (501) staff       (20)    12945 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/CO_AutoCorr.c
+-rw-r--r--   0 joshua     (501) staff       (20)     1189 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/CO_AutoCorr.h
+-rw-r--r--   0 joshua     (501) staff       (20)     2132 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/DN_HistogramMode_10.c
+-rw-r--r--   0 joshua     (501) staff       (20)      191 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/DN_HistogramMode_10.h
+-rw-r--r--   0 joshua     (501) staff       (20)     2717 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/DN_HistogramMode_5.c
+-rw-r--r--   0 joshua     (501) staff       (20)      188 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/DN_HistogramMode_5.h
+-rw-r--r--   0 joshua     (501) staff       (20)      184 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/DN_Mean.c
+-rw-r--r--   0 joshua     (501) staff       (20)      187 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/DN_Mean.h
+-rw-r--r--   0 joshua     (501) staff       (20)     5054 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/DN_OutlierInclude.c
+-rw-r--r--   0 joshua     (501) staff       (20)      500 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/DN_OutlierInclude.h
+-rw-r--r--   0 joshua     (501) staff       (20)      271 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/DN_Spread_Std.c
+-rw-r--r--   0 joshua     (501) staff       (20)      208 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/DN_Spread_Std.h
+-rw-r--r--   0 joshua     (501) staff       (20)     3772 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/FC_LocalSimple.c
+-rw-r--r--   0 joshua     (501) staff       (20)      766 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/FC_LocalSimple.h
+-rw-r--r--   0 joshua     (501) staff       (20)     1273 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/IN_AutoMutualInfoStats.c
+-rw-r--r--   0 joshua     (501) staff       (20)      381 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/IN_AutoMutualInfoStats.h
+-rw-r--r--   0 joshua     (501) staff       (20)      715 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/MD_hrv.c
+-rw-r--r--   0 joshua     (501) staff       (20)      298 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/MD_hrv.h
+-rw-r--r--   0 joshua     (501) staff       (20)     3651 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/PD_PeriodicityWang.c
+-rw-r--r--   0 joshua     (501) staff       (20)      348 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/PD_PeriodicityWang.h
+-rw-r--r--   0 joshua     (501) staff       (20)     1958 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/SB_BinaryStats.c
+-rw-r--r--   0 joshua     (501) staff       (20)      424 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/SB_BinaryStats.h
+-rw-r--r--   0 joshua     (501) staff       (20)     1070 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/SB_CoarseGrain.c
+-rw-r--r--   0 joshua     (501) staff       (20)      301 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/SB_CoarseGrain.h
+-rw-r--r--   0 joshua     (501) staff       (20)    12842 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/SB_MotifThree.c
+-rw-r--r--   0 joshua     (501) staff       (20)      325 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/SB_MotifThree.h
+-rw-r--r--   0 joshua     (501) staff       (20)     3472 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/SB_TransitionMatrix.c
+-rw-r--r--   0 joshua     (501) staff       (20)      291 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/SB_TransitionMatrix.h
+-rw-r--r--   0 joshua     (501) staff       (20)     8854 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/SC_FluctAnal.c
+-rw-r--r--   0 joshua     (501) staff       (20)      413 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/SC_FluctAnal.h
+-rw-r--r--   0 joshua     (501) staff       (20)     5022 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/SP_Summaries.c
+-rw-r--r--   0 joshua     (501) staff       (20)      435 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/SP_Summaries.h
+-rw-r--r--   0 joshua     (501) staff       (20)     7630 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/butterworth.c
+-rw-r--r--   0 joshua     (501) staff       (20)      288 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/butterworth.h
+-rw-r--r--   0 joshua     (501) staff       (20)    11538 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/catch22_wrap.c
+-rw-r--r--   0 joshua     (501) staff       (20)     1473 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/fft.c
+-rw-r--r--   0 joshua     (501) staff       (20)      646 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/fft.h
+-rw-r--r--   0 joshua     (501) staff       (20)     4246 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/helper_functions.c
+-rw-r--r--   0 joshua     (501) staff       (20)     1044 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/helper_functions.h
+-rw-r--r--   0 joshua     (501) staff       (20)     4335 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/histcounts.c
+-rw-r--r--   0 joshua     (501) staff       (20)      778 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/histcounts.h
+-rw-r--r--   0 joshua     (501) staff       (20)    13510 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/main.c
+-rw-r--r--   0 joshua     (501) staff       (20)      303 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/main.h
+-rwxr-xr-x   0 joshua     (501) staff       (20)     1708 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/runAllTS.sh
+-rw-r--r--   0 joshua     (501) staff       (20)    19700 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/splinefit.c
+-rw-r--r--   0 joshua     (501) staff       (20)      309 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/splinefit.h
+-rw-r--r--   0 joshua     (501) staff       (20)     5906 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/stats.c
+-rw-r--r--   0 joshua     (501) staff       (20)     1421 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/C/stats.h
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-14 04:59:33.854353 pycatch22-0.4.5/src/pycatch22/
+-rw-r--r--   0 joshua     (501) staff       (20)       57 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/pycatch22/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2498 2024-05-14 01:49:12.000000 pycatch22-0.4.5/src/pycatch22/catch22.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-14 04:59:33.855756 pycatch22-0.4.5/src/pycatch22.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     5529 2024-05-14 04:59:33.000000 pycatch22-0.4.5/src/pycatch22.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     1302 2024-05-14 04:59:33.000000 pycatch22-0.4.5/src/pycatch22.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2024-05-14 04:59:33.000000 pycatch22-0.4.5/src/pycatch22.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       20 2024-05-14 04:59:33.000000 pycatch22-0.4.5/src/pycatch22.egg-info/top_level.txt
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-05-14 04:59:33.855389 pycatch22-0.4.5/tests/
+-rw-r--r--   0 joshua     (501) staff       (20)     4276 2024-05-14 01:49:12.000000 pycatch22-0.4.5/tests/test_features.py
```

### Comparing `pycatch22-0.4.4/LICENSE` & `pycatch22-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/PKG-INFO` & `pycatch22-0.4.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6361  : 2.1.Name: pyca
 00000020: 7463 6832 320a 5665 7273 696f 6e3a 2030  tch22.Version: 0
-00000030: 2e34 2e34 0a53 756d 6d61 7279 3a20 3232  .4.4.Summary: 22
+00000030: 2e34 2e35 0a53 756d 6d61 7279 3a20 3232  .4.5.Summary: 22
 00000040: 2043 416e 6f6e 6963 616c 2054 696d 652d   CAnonical Time-
 00000050: 7365 7269 6573 2046 6561 7475 7265 730a  series Features.
 00000060: 4175 7468 6f72 3a20 4361 726c 2048 204c  Author: Carl H L
 00000070: 7562 6261 0a41 7574 686f 722d 656d 6169  ubba.Author-emai
 00000080: 6c3a 2063 6172 6c2e 6c75 6262 6140 676d  l: carl.lubba@gm
 00000090: 782e 6465 0a4d 6169 6e74 6169 6e65 723a  x.de.Maintainer:
 000000a0: 2042 656e 2044 2046 756c 6368 6572 0a4d   Ben D Fulcher.M
@@ -37,284 +37,310 @@
 00000240: 7220 6c61 7465 7220 2847 504c 7633 2b29  r later (GPLv3+)
 00000250: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
 00000260: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
 00000270: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
 00000280: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
 00000290: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
 000002a0: 6172 6b64 6f77 6e0a 4c69 6365 6e73 652d  arkdown.License-
-000002b0: 4669 6c65 3a20 4c49 4345 4e53 450a 0a23  File: LICENSE..#
-000002c0: 205f 7079 6361 7463 6832 325f 202d 2043   _pycatch22_ - C
-000002d0: 416e 6f6e 6963 616c 2054 696d 652d 7365  Anonical Time-se
-000002e0: 7269 6573 2043 4861 7261 6374 6572 6973  ries CHaracteris
-000002f0: 7469 6373 2069 6e20 7079 7468 6f6e 0a0a  tics in python..
-00000300: 3c69 6d67 2073 7263 3d22 696d 672f 6361  <img src="img/ca
-00000310: 7463 6832 325f 6c6f 676f 5f73 7175 6172  tch22_logo_squar
-00000320: 652e 706e 6722 2077 6964 7468 3d22 3235  e.png" width="25
-00000330: 3022 2068 6569 6768 743d 2232 3530 222f  0" height="250"/
-00000340: 3e0a 0a23 2320 4162 6f75 740a 0a5b 5f63  >..## About..[_c
-00000350: 6174 6368 3232 5f5d 2868 7474 7073 3a2f  atch22_](https:/
-00000360: 2f67 6974 6875 622e 636f 6d2f 4479 6e61  /github.com/Dyna
-00000370: 6d69 6373 416e 644e 6575 7261 6c53 7973  micsAndNeuralSys
-00000380: 7465 6d73 2f63 6174 6368 3232 2920 6973  tems/catch22) is
-00000390: 2061 2063 6f6c 6c65 6374 696f 6e20 6f66   a collection of
-000003a0: 2032 3220 7469 6d65 2d73 6572 6965 7320   22 time-series 
-000003b0: 6665 6174 7572 6573 2063 6f64 6564 2069  features coded i
-000003c0: 6e20 4320 7468 6174 2063 616e 2062 6520  n C that can be 
-000003d0: 7275 6e20 6672 6f6d 2050 7974 686f 6e2c  run from Python,
-000003e0: 2061 7320 7765 6c6c 2061 7320 5b52 5d28   as well as [R](
-000003f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000400: 6f6d 2f68 656e 6465 7273 6f6e 7472 656e  om/hendersontren
-00000410: 742f 5263 6174 6368 3232 292c 205b 4d61  t/Rcatch22), [Ma
-00000420: 746c 6162 5d28 6874 7470 733a 2f2f 6769  tlab](https://gi
-00000430: 7468 7562 2e63 6f6d 2f44 796e 616d 6963  thub.com/Dynamic
-00000440: 7341 6e64 4e65 7572 616c 5379 7374 656d  sAndNeuralSystem
-00000450: 732f 6361 7463 6832 3229 2c20 616e 6420  s/catch22), and 
-00000460: 5b4a 756c 6961 5d28 6874 7470 733a 2f2f  [Julia](https://
-00000470: 6769 7468 7562 2e63 6f6d 2f62 7265 6e64  github.com/brend
-00000480: 616e 6a6f 686e 6861 7272 6973 2f43 6174  anjohnharris/Cat
-00000490: 6368 3232 2e6a 6c29 2e0a 0a54 6869 7320  ch22.jl)...This 
-000004a0: 7061 636b 6167 6520 7072 6f76 6964 6573  package provides
-000004b0: 2061 2070 7974 686f 6e20 696d 706c 656d   a python implem
-000004c0: 656e 7461 7469 6f6e 2061 7320 7468 6520  entation as the 
-000004d0: 6d6f 6475 6c65 205f 7079 6361 7463 6832  module _pycatch2
-000004e0: 325f 2c20 6c69 6365 6e73 6564 2075 6e64  2_, licensed und
-000004f0: 6572 2074 6865 205b 474e 5520 4750 4c20  er the [GNU GPL 
-00000500: 7633 206c 6963 656e 7365 5d28 6874 7470  v3 license](http
-00000510: 3a2f 2f77 7777 2e67 6e75 2e6f 7267 2f6c  ://www.gnu.org/l
-00000520: 6963 656e 7365 732f 6770 6c2d 332e 302e  icenses/gpl-3.0.
-00000530: 6874 6d6c 2920 286f 7220 6c61 7465 7229  html) (or later)
-00000540: 2e0a 0a23 2323 2057 6861 7420 646f 2074  ...### What do t
-00000550: 6865 2066 6561 7475 7265 7320 646f 3f0a  he features do?.
-00000560: 0a54 6869 7320 5b47 6974 426f 6f6b 7320  .This [GitBooks 
-00000570: 7765 6273 6974 655d 2868 7474 7073 3a2f  website](https:/
-00000580: 2f66 6561 7475 7265 2d62 6173 6564 2d74  /feature-based-t
-00000590: 696d 652d 7365 7269 6573 2d61 6e61 6c79  ime-series-analy
-000005a0: 732e 6769 7462 6f6f 6b2e 696f 2f63 6174  s.gitbook.io/cat
-000005b0: 6368 3232 2d66 6561 7475 7265 732f 2920  ch22-features/) 
-000005c0: 6973 2064 6564 6963 6174 6564 2074 6f20  is dedicated to 
-000005d0: 6465 7363 7269 6269 6e67 2074 6865 2066  describing the f
-000005e0: 6561 7475 7265 732e 0a46 6f72 2074 6865  eatures..For the
-000005f0: 6972 2069 6d70 6c65 6d65 6e74 6174 696f  ir implementatio
-00000600: 6e20 696e 2063 6f64 652c 2073 6565 2074  n in code, see t
-00000610: 6865 205b 6d61 696e 205f 6361 7463 6832  he [main _catch2
-00000620: 325f 2072 6570 6f73 6974 6f72 795d 2868  2_ repository](h
-00000630: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000640: 6d2f 4479 6e61 6d69 6373 416e 644e 6575  m/DynamicsAndNeu
-00000650: 7261 6c53 7973 7465 6d73 2f63 6174 6368  ralSystems/catch
-00000660: 3232 292e 0a54 6865 7265 2069 7320 616c  22)..There is al
-00000670: 736f 2069 6e66 6f72 6d61 7469 6f6e 2069  so information i
-00000680: 6e20 7468 6520 6173 736f 6369 6174 6564  n the associated
-00000690: 2070 6170 6572 205b 2623 7831 4634 4437   paper [&#x1F4D7
-000006a0: 3b20 4c75 6262 6120 6574 2061 6c2e 2028  ; Lubba et al. (
-000006b0: 3230 3139 292e 5d28 6874 7470 733a 2f2f  2019).](https://
-000006c0: 646f 692e 6f72 672f 3130 2e31 3030 372f  doi.org/10.1007/
-000006d0: 7331 3036 3138 2d30 3139 2d30 3036 3437  s10618-019-00647
-000006e0: 2d78 292e 0a0a 2323 2320 4163 6b6e 6f77  -x)...### Acknow
-000006f0: 6c65 6467 656d 656e 7420 3a2b 313a 0a0a  ledgement :+1:..
-00000700: 4966 2079 6f75 2075 7365 2074 6869 7320  If you use this 
-00000710: 736f 6674 7761 7265 2c20 706c 6561 7365  software, please
-00000720: 2072 6561 6420 616e 6420 6369 7465 2074   read and cite t
-00000730: 6869 7320 6f70 656e 2d61 6363 6573 7320  his open-access 
-00000740: 6172 7469 636c 653a 0a0a 2d20 2623 7831  article:..- &#x1
-00000750: 4634 4437 3b20 4c75 6262 6120 6574 2061  F4D7; Lubba et a
-00000760: 6c2e 205b 5f63 6174 6368 3232 5f3a 2043  l. [_catch22_: C
-00000770: 416e 6f6e 6963 616c 2054 696d 652d 7365  Anonical Time-se
-00000780: 7269 6573 2043 4861 7261 6374 6572 6973  ries CHaracteris
-00000790: 7469 6373 5d28 6874 7470 733a 2f2f 646f  tics](https://do
-000007a0: 692e 6f72 672f 3130 2e31 3030 372f 7331  i.org/10.1007/s1
-000007b0: 3036 3138 2d30 3139 2d30 3036 3437 2d78  0618-019-00647-x
-000007c0: 292c 205f 4461 7461 204d 696e 204b 6e6f  ), _Data Min Kno
-000007d0: 776c 2044 6973 635f 205f 5f33 335f 5f2c  wl Disc_ __33__,
-000007e0: 2031 3832 3120 2832 3031 3929 2e0a 0a23   1821 (2019)...#
-000007f0: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
-00000800: 5573 696e 6720 6070 6970 6020 666f 7220  Using `pip` for 
-00000810: 5b60 7079 6361 7463 6832 3260 5d28 6874  [`pycatch22`](ht
-00000820: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000830: 726f 6a65 6374 2f70 7963 6174 6368 3232  roject/pycatch22
-00000840: 2f29 3a0a 0a60 6060 0a70 6970 2069 6e73  /):..```.pip ins
-00000850: 7461 6c6c 2070 7963 6174 6368 3232 0a60  tall pycatch22.`
-00000860: 6060 0a0a 4966 2074 6869 7320 646f 6573  ``..If this does
-00000870: 6e27 7420 776f 726b 2c20 6d61 6b65 2073  n't work, make s
-00000880: 7572 6520 796f 7520 6172 6520 7573 696e  ure you are usin
-00000890: 6720 7468 6520 6c61 7465 7374 2060 7365  g the latest `se
-000008a0: 7475 7074 6f6f 6c73 603a 2060 7069 7020  tuptools`: `pip 
-000008b0: 696e 7374 616c 6c20 7365 7475 7074 6f6f  install setuptoo
-000008c0: 6c73 202d 2d75 7067 7261 6465 602e 0a0a  ls --upgrade`...
-000008d0: 4966 2079 6f75 2063 6f6d 6520 6163 726f  If you come acro
-000008e0: 7373 2065 7272 6f72 7320 7769 7468 2076  ss errors with v
-000008f0: 6572 7369 6f6e 2072 6573 6f6c 7574 696f  ersion resolutio
-00000900: 6e2c 2079 6f75 2073 686f 756c 6420 7472  n, you should tr
-00000910: 7920 736f 6d65 7468 696e 6720 6c69 6b65  y something like
-00000920: 3a20 6070 6970 2069 6e73 7461 6c6c 2070  : `pip install p
-00000930: 7963 6174 6368 3232 3d3d 302e 342e 3220  ycatch22==0.4.2 
-00000940: 2d2d 7573 652d 6465 7072 6563 6174 6564  --use-deprecated
-00000950: 3d6c 6567 6163 792d 7265 736f 6c76 6572  =legacy-resolver
-00000960: 602e 0a0a 4974 2069 7320 616c 736f 2061  `...It is also a
-00000970: 205b 7061 636b 6167 6520 6f6e 2061 6e61   [package on ana
-00000980: 636f 6e64 615d 2868 7474 7073 3a2f 2f61  conda](https://a
-00000990: 6e61 636f 6e64 612e 6f72 672f 636f 6e64  naconda.org/cond
-000009a0: 612d 666f 7267 652f 7079 6361 7463 6832  a-forge/pycatch2
-000009b0: 3229 2074 6861 6e6b 7320 746f 205b 4072  2) thanks to [@r
-000009c0: 7061 6e61 695d 2868 7474 7073 3a2f 2f67  panai](https://g
-000009d0: 6974 6875 622e 636f 6d2f 7270 616e 6169  ithub.com/rpanai
-000009e0: 292c 2077 6869 6368 2079 6f75 2063 616e  ), which you can
-000009f0: 2069 6e73 7461 6c6c 2076 6961 2060 636f   install via `co
-00000a00: 6e64 6160 3a0a 0a60 6060 0a63 6f6e 6461  nda`:..```.conda
-00000a10: 2069 6e73 7461 6c6c 202d 6320 636f 6e64   install -c cond
-00000a20: 612d 666f 7267 6520 7079 6361 7463 6832  a-forge pycatch2
-00000a30: 320a 6060 600a 0a6f 7220 606d 616d 6261  2.```..or `mamba
-00000a40: 603a 0a0a 6060 600a 6d61 6d62 6120 696e  `:..```.mamba in
-00000a50: 7374 616c 6c20 2d63 2063 6f6e 6461 2d66  stall -c conda-f
-00000a60: 6f72 6765 2070 7963 6174 6368 3232 0a60  orge pycatch22.`
-00000a70: 6060 0a0a 5b41 206d 616e 7561 6c20 696e  ``..[A manual in
-00000a80: 7374 616c 6c20 2862 6f74 746f 6d20 6f66  stall (bottom of
-00000a90: 2074 6869 7320 7061 6765 2920 6973 2061   this page) is a
-00000aa0: 206c 6173 7420 7265 736f 7274 2e5d 0a0a   last resort.]..
-00000ab0: 2323 2055 7361 6765 0a0a 4561 6368 2066  ## Usage..Each f
-00000ac0: 6561 7475 7265 2066 756e 6374 696f 6e20  eature function 
-00000ad0: 6361 6e20 6265 2061 6363 6573 7365 6420  can be accessed 
-00000ae0: 696e 6469 7669 6475 616c 6c79 2061 6e64  individually and
-00000af0: 2074 616b 6573 2061 7272 6179 7320 6173   takes arrays as
-00000b00: 2074 7570 6c65 206f 7220 6c69 7374 7320   tuple or lists 
-00000b10: 286e 6f74 2060 6e75 6d70 7960 2061 7272  (not `numpy` arr
-00000b20: 6179 7329 2e0a 466f 7220 6578 616d 706c  ays)..For exampl
-00000b30: 652c 2066 6f72 206c 6f61 6465 6420 6461  e, for loaded da
-00000b40: 7461 2060 7473 4461 7461 6020 696e 2050  ta `tsData` in P
-00000b50: 7974 686f 6e3a 0a0a 6060 6070 7974 686f  ython:..```pytho
-00000b60: 6e33 0a69 6d70 6f72 7420 7079 6361 7463  n3.import pycatc
-00000b70: 6832 320a 7473 4461 7461 203d 205b 312c  h22.tsData = [1,
-00000b80: 322c 342c 335d 2023 2028 6f72 206d 6f72  2,4,3] # (or mor
-00000b90: 6520 696e 7465 7265 7374 696e 6720 6461  e interesting da
-00000ba0: 7461 2129 0a70 7963 6174 6368 3232 2e43  ta!).pycatch22.C
-00000bb0: 4f5f 6631 6563 6163 2874 7344 6174 6129  O_f1ecac(tsData)
-00000bc0: 0a60 6060 0a0a 416c 6c20 6665 6174 7572  .```..All featur
-00000bd0: 6573 2061 7265 2062 756e 646c 6564 2069  es are bundled i
-00000be0: 6e20 7468 6520 6d65 7468 6f64 2060 6361  n the method `ca
-00000bf0: 7463 6832 325f 616c 6c60 2c20 7768 6963  tch22_all`, whic
-00000c00: 6820 616c 736f 2061 6363 6570 7473 2060  h also accepts `
-00000c10: 6e75 6d70 7960 2061 7272 6179 7320 616e  numpy` arrays an
-00000c20: 6420 6769 7665 7320 6261 636b 2061 2064  d gives back a d
-00000c30: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
-00000c40: 6e69 6e67 2074 6865 2065 6e74 7269 6573  ning the entries
-00000c50: 2060 6361 7463 6832 325f 616c 6c5b 276e   `catch22_all['n
-00000c60: 616d 6573 275d 6020 666f 7220 6665 6174  ames']` for feat
-00000c70: 7572 6520 6e61 6d65 7320 616e 6420 6063  ure names and `c
-00000c80: 6174 6368 3232 5f61 6c6c 5b27 7661 6c75  atch22_all['valu
-00000c90: 6573 275d 6020 666f 7220 6665 6174 7572  es']` for featur
-00000ca0: 6520 6f75 7470 7574 732e 0a0a 5573 6167  e outputs...Usag
-00000cb0: 6520 2863 6f6d 7075 7469 6e67 2032 3220  e (computing 22 
-00000cc0: 6665 6174 7572 6573 3a20 5f63 6174 6368  features: _catch
-00000cd0: 3232 5f29 3a0a 0a60 6060 7079 7468 6f6e  22_):..```python
-00000ce0: 330a 7079 6361 7463 6832 322e 6361 7463  3.pycatch22.catc
-00000cf0: 6832 325f 616c 6c28 7473 4461 7461 290a  h22_all(tsData).
-00000d00: 6060 600a 0a55 7361 6765 2028 636f 6d70  ```..Usage (comp
-00000d10: 7574 696e 6720 3234 2066 6561 7475 7265  uting 24 feature
-00000d20: 733a 205f 6361 7463 6832 345f 203d 205f  s: _catch24_ = _
-00000d30: 6361 7463 6832 325f 202b 206d 6561 6e20  catch22_ + mean 
-00000d40: 2b20 7374 616e 6461 7264 2064 6576 6961  + standard devia
-00000d50: 7469 6f6e 293a 0a0a 6060 6070 7974 686f  tion):..```pytho
-00000d60: 6e33 0a70 7963 6174 6368 3232 2e63 6174  n3.pycatch22.cat
-00000d70: 6368 3232 5f61 6c6c 2874 7344 6174 612c  ch22_all(tsData,
-00000d80: 6361 7463 6832 343d 5472 7565 290a 6060  catch24=True).``
-00000d90: 600a 0a57 6520 616c 736f 2069 6e63 6c75  `..We also inclu
-00000da0: 6465 2061 2027 7368 6f72 7420 6e61 6d65  de a 'short name
-00000db0: 2720 666f 7220 6561 6368 2066 6561 7475  ' for each featu
-00000dc0: 7265 2066 6f72 2065 6173 6965 7220 7265  re for easier re
-00000dd0: 6665 7265 6e63 6520 2861 7320 6f75 746c  ference (as outl
-00000de0: 696e 6564 2069 6e20 7468 6520 4769 7442  ined in the GitB
-00000df0: 6f6f 6b20 5b46 6561 7475 7265 206f 7665  ook [Feature ove
-00000e00: 7276 6965 7720 7461 626c 655d 2868 7474  rview table](htt
-00000e10: 7073 3a2f 2f61 7070 2e67 6974 626f 6f6b  ps://app.gitbook
-00000e20: 2e63 6f6d 2f6f 2f2d 4d66 6568 5a71 6143  .com/o/-MfehZqaC
-00000e30: 576e 7353 5244 4964 5547 382f 732f 2d4d  WnsSRDIdUG8/s/-M
-00000e40: 6648 4659 346c 767a 4f7a 3349 5061 4133  fHFY4lvzOz3IPaA3
-00000e50: 776d 2f66 6561 7475 7265 2d6f 7665 7276  wm/feature-overv
-00000e60: 6965 772d 7461 626c 6529 292e 0a54 6865  iew-table))..The
-00000e70: 7365 2073 686f 7274 206e 616d 6573 2063  se short names c
-00000e80: 616e 2062 6520 696e 636c 7564 6564 2069  an be included i
-00000e90: 6e20 7468 6520 6f75 7470 7574 2066 726f  n the output fro
-00000ea0: 6d20 6063 6174 6368 3232 5f61 6c6c 2829  m `catch22_all()
-00000eb0: 6020 6279 2073 6574 7469 6e67 2060 7368  ` by setting `sh
-00000ec0: 6f72 745f 6e61 6d65 733d 5472 7565 6020  ort_names=True` 
-00000ed0: 6173 2066 6f6c 6c6f 7773 3a0a 0a60 6060  as follows:..```
-00000ee0: 7079 7468 6f6e 330a 7079 6361 7463 6832  python3.pycatch2
-00000ef0: 322e 6361 7463 6832 325f 616c 6c28 7473  2.catch22_all(ts
-00000f00: 4461 7461 2c63 6174 6368 3234 3d54 7275  Data,catch24=Tru
-00000f10: 652c 7368 6f72 745f 6e61 6d65 733d 5472  e,short_names=Tr
-00000f20: 7565 290a 6060 600a 0a23 2323 2054 656d  ue).```..### Tem
-00000f30: 706c 6174 6520 616e 616c 7973 6973 2073  plate analysis s
-00000f40: 6372 6970 740a 0a54 6861 6e6b 7320 746f  cript..Thanks to
-00000f50: 205b 406a 6d6f 6f32 3838 305d 2868 7474   [@jmoo2880](htt
-00000f60: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000f70: 6a6d 6f6f 3238 3830 2920 666f 7220 7075  jmoo2880) for pu
-00000f80: 7474 696e 6720 746f 6765 7468 6572 2061  tting together a
-00000f90: 205b 6465 6d6f 6e73 7472 6174 696f 6e20   [demonstration 
-00000fa0: 6e6f 7465 626f 6f6b 5d28 6874 7470 733a  notebook](https:
-00000fb0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6d6f  //github.com/jmo
-00000fc0: 6f32 3838 302f 6332 322d 7573 6167 652d  o2880/c22-usage-
-00000fd0: 6578 616d 706c 6573 2f29 2066 6f72 2075  examples/) for u
-00000fe0: 7369 6e67 2070 7963 6174 6368 3232 2074  sing pycatch22 t
-00000ff0: 6f20 6578 7472 6163 7420 6665 6174 7572  o extract featur
-00001000: 6573 2066 726f 6d20 6120 7469 6d65 2d73  es from a time-s
-00001010: 6572 6965 7320 6461 7461 7365 742e 0a0a  eries dataset...
-00001020: 2323 2320 5573 6167 6520 6e6f 7465 730a  ### Usage notes.
-00001030: 0a2d 2057 6865 6e20 7072 6573 656e 7469  .- When presenti
-00001040: 6e67 2072 6573 756c 7473 2075 7369 6e67  ng results using
-00001050: 205f 6361 7463 6832 325f 2c20 796f 7520   _catch22_, you 
-00001060: 6d75 7374 2069 6465 6e74 6966 7920 7468  must identify th
-00001070: 6520 7665 7273 696f 6e20 7573 6564 2074  e version used t
-00001080: 6f20 616c 6c6f 7720 636c 6561 7220 7265  o allow clear re
-00001090: 7072 6f64 7563 7469 6f6e 206f 6620 796f  production of yo
-000010a0: 7572 2072 6573 756c 7473 2e20 466f 7220  ur results. For 
-000010b0: 6578 616d 706c 652c 2060 434f 5f66 3165  example, `CO_f1e
-000010c0: 6361 6360 2077 6173 2061 6c74 6572 6564  cac` was altered
-000010d0: 2066 726f 6d20 616e 2069 6e74 6567 6572   from an integer
-000010e0: 2d76 616c 7565 6420 6f75 7470 7574 2074  -valued output t
-000010f0: 6f20 6120 6c69 6e65 6172 6c79 2069 6e74  o a linearly int
-00001100: 6572 706f 6c61 7465 6420 7265 616c 2d76  erpolated real-v
-00001110: 616c 7565 6420 6f75 7470 7574 2066 726f  alued output fro
-00001120: 6d20 7630 2e33 2e0a 2d20 5f5f 496d 706f  m v0.3..- __Impo
-00001130: 7274 616e 7420 4e6f 7465 3a5f 5f20 5f63  rtant Note:__ _c
-00001140: 6174 6368 3232 5f20 6665 6174 7572 6573  atch22_ features
-00001150: 206f 6e6c 7920 6576 616c 7561 7465 205f   only evaluate _
-00001160: 6479 6e61 6d69 6361 6c5f 2070 726f 7065  dynamical_ prope
-00001170: 7274 6965 7320 6f66 2074 696d 6520 7365  rties of time se
-00001180: 7269 6573 2061 6e64 2064 6f20 6e6f 7420  ries and do not 
-00001190: 7265 7370 6f6e 6420 746f 2062 6173 6963  respond to basic
-000011a0: 2064 6966 6665 7265 6e63 6573 2069 6e20   differences in 
-000011b0: 7468 6520 6c6f 6361 7469 6f6e 2028 652e  the location (e.
-000011c0: 672e 2c20 6d65 616e 2920 6f72 2073 7072  g., mean) or spr
-000011d0: 6561 6420 2865 2e67 2e2c 2076 6172 6961  ead (e.g., varia
-000011e0: 6e63 6529 2e0a 2020 2d20 4672 6f6d 205f  nce)..  - From _
-000011f0: 6361 7463 6832 325f 2076 302e 332c 2049  catch22_ v0.3, I
-00001200: 6620 7468 6520 6c6f 6361 7469 6f6e 2061  f the location a
-00001210: 6e64 2073 7072 6561 6420 6f66 2074 6865  nd spread of the
-00001220: 2072 6177 2074 696d 652d 7365 7269 6573   raw time-series
-00001230: 2064 6973 7472 6962 7574 696f 6e20 6d61   distribution ma
-00001240: 7920 6265 2069 6d70 6f72 7461 6e74 2066  y be important f
-00001250: 6f72 2079 6f75 7220 6170 706c 6963 6174  or your applicat
-00001260: 696f 6e2c 2077 6520 7375 6767 6573 7420  ion, we suggest 
-00001270: 6170 706c 7969 6e67 2074 6865 2066 756e  applying the fun
-00001280: 6374 696f 6e20 6172 6775 6d65 6e74 2060  ction argument `
-00001290: 6361 7463 6832 3420 3d20 5472 7565 6020  catch24 = True` 
-000012a0: 746f 2079 6f75 7220 6361 6c6c 2074 6f20  to your call to 
-000012b0: 7468 6520 5f63 6174 6368 3232 5f20 6675  the _catch22_ fu
-000012c0: 6e63 7469 6f6e 2069 6e20 7468 6520 6c61  nction in the la
-000012d0: 6e67 7561 6765 206f 6620 796f 7572 2063  nguage of your c
-000012e0: 686f 6963 652e 0a20 2054 6869 7320 7769  hoice..  This wi
-000012f0: 6c6c 2072 6573 756c 7420 696e 2032 3420  ll result in 24 
-00001300: 6665 6174 7572 6573 2062 6569 6e67 2063  features being c
-00001310: 616c 6375 6c61 7465 643a 2074 6865 205f  alculated: the _
-00001320: 6361 7463 6832 325f 2066 6561 7475 7265  catch22_ feature
-00001330: 7320 696e 2061 6464 6974 696f 6e20 746f  s in addition to
-00001340: 206d 6561 6e20 616e 6420 7374 616e 6461   mean and standa
-00001350: 7264 2064 6576 6961 7469 6f6e 2e0a 0a23  rd deviation...#
-00001360: 2323 204d 616e 7561 6c20 696e 7374 616c  ## Manual instal
-00001370: 6c0a 0a49 6620 796f 7520 6669 6e64 2069  l..If you find i
-00001380: 7373 7565 7320 7769 7468 2074 6865 2060  ssues with the `
-00001390: 7069 7060 2069 6e73 7461 6c6c 2c20 796f  pip` install, yo
-000013a0: 7520 6361 6e20 616c 736f 2069 6e73 7461  u can also insta
-000013b0: 6c6c 2075 7369 6e67 2060 7365 7475 7074  ll using `setupt
-000013c0: 6f6f 6c73 603a 0a0a 6060 600a 7079 7468  ools`:..```.pyth
-000013d0: 6f6e 3320 7365 7475 702e 7079 2062 7569  on3 setup.py bui
-000013e0: 6c64 0a70 7974 686f 6e33 2073 6574 7570  ld.python3 setup
-000013f0: 2e70 7920 696e 7374 616c 6c0a 6060 600a  .py install.```.
+000002b0: 4669 6c65 3a20 4c49 4345 4e53 450a 0a3c  File: LICENSE..<
+000002c0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+000002d0: 3e3c 696d 6720 7372 633d 2269 6d67 2f63  ><img src="img/c
+000002e0: 6174 6368 3232 5f6c 6f67 6f5f 7371 7561  atch22_logo_squa
+000002f0: 7265 2e70 6e67 2220 616c 743d 2263 6174  re.png" alt="cat
+00000300: 6368 3232 206c 6f67 6f22 2068 6569 6768  ch22 logo" heigh
+00000310: 743d 2232 3230 222f 3e3c 2f70 3e0a 0a3c  t="220"/></p>..<
+00000320: 6831 2061 6c69 676e 3d22 6365 6e74 6572  h1 align="center
+00000330: 223e 3c65 6d3e 7079 6361 7463 6832 323c  "><em>pycatch22<
+00000340: 2f65 6d3e 3a20 4341 6e6f 6e69 6361 6c20  /em>: CAnonical 
+00000350: 5469 6d65 2d73 6572 6965 7320 4348 6172  Time-series CHar
+00000360: 6163 7465 7269 7374 6963 7320 696e 2070  acteristics in p
+00000370: 7974 686f 6e3c 2f68 313e 0a0a 3c70 2061  ython</h1>..<p a
+00000380: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+00000390: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+000003a0: 733a 2f2f 7777 772e 676e 752e 6f72 672f  s://www.gnu.org/
+000003b0: 6c69 6365 6e73 6573 2f67 706c 2d33 2e30  licenses/gpl-3.0
+000003c0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+000003d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000003e0: 696f 2f62 6164 6765 2f4c 6963 656e 7365  io/badge/License
+000003f0: 2d47 504c 7633 2d62 6c75 652e 7376 6722  -GPLv3-blue.svg"
+00000400: 2068 6569 6768 743d 2232 3022 2f3e 3c2f   height="20"/></
+00000410: 613e 0a20 0920 203c 6120 6872 6566 3d22  a>. .  <a href="
+00000420: 6874 7470 733a 2f2f 7477 6974 7465 722e  https://twitter.
+00000430: 636f 6d2f 636f 6d70 5469 6d65 5365 7269  com/compTimeSeri
+00000440: 6573 223e 3c69 6d67 2073 7263 3d22 6874  es"><img src="ht
+00000450: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000460: 732e 696f 2f74 7769 7474 6572 2f75 726c  s.io/twitter/url
+00000470: 2f68 7474 7073 2f74 7769 7474 6572 2e63  /https/twitter.c
+00000480: 6f6d 2f63 6f6d 7054 696d 6553 6572 6965  om/compTimeSerie
+00000490: 732e 7376 673f 7374 796c 653d 736f 6369  s.svg?style=soci
+000004a0: 616c 266c 6162 656c 3d46 6f6c 6c6f 7725  al&label=Follow%
+000004b0: 3230 2534 3063 6f6d 7054 696d 6553 6572  20%40compTimeSer
+000004c0: 6965 7322 2068 6569 6768 743d 2232 3022  ies" height="20"
+000004d0: 2f3e 3c2f 613e 0a3c 2f70 3e0a 0a0a 2323  /></a>.</p>...##
+000004e0: 2041 626f 7574 0a0a 5b5f 6361 7463 6832   About..[_catch2
+000004f0: 325f 5d28 6874 7470 733a 2f2f 6769 7468  2_](https://gith
+00000500: 7562 2e63 6f6d 2f44 796e 616d 6963 7341  ub.com/DynamicsA
+00000510: 6e64 4e65 7572 616c 5379 7374 656d 732f  ndNeuralSystems/
+00000520: 6361 7463 6832 3229 2069 7320 6120 636f  catch22) is a co
+00000530: 6c6c 6563 7469 6f6e 206f 6620 3232 2074  llection of 22 t
+00000540: 696d 652d 7365 7269 6573 2066 6561 7475  ime-series featu
+00000550: 7265 7320 636f 6465 6420 696e 2043 2074  res coded in C t
+00000560: 6861 7420 6361 6e20 6265 2072 756e 2066  hat can be run f
+00000570: 726f 6d20 5079 7468 6f6e 2c20 6173 2077  rom Python, as w
+00000580: 656c 6c20 6173 205b 525d 2868 7474 7073  ell as [R](https
+00000590: 3a2f 2f67 6974 6875 622e 636f 6d2f 6865  ://github.com/he
+000005a0: 6e64 6572 736f 6e74 7265 6e74 2f52 6361  ndersontrent/Rca
+000005b0: 7463 6832 3229 2c20 5b4d 6174 6c61 625d  tch22), [Matlab]
+000005c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000005d0: 636f 6d2f 4479 6e61 6d69 6373 416e 644e  com/DynamicsAndN
+000005e0: 6575 7261 6c53 7973 7465 6d73 2f63 6174  euralSystems/cat
+000005f0: 6368 3232 292c 2061 6e64 205b 4a75 6c69  ch22), and [Juli
+00000600: 615d 2868 7474 7073 3a2f 2f67 6974 6875  a](https://githu
+00000610: 622e 636f 6d2f 6272 656e 6461 6e6a 6f68  b.com/brendanjoh
+00000620: 6e68 6172 7269 732f 4361 7463 6832 322e  nharris/Catch22.
+00000630: 6a6c 292e 0a0a 5468 6973 2070 6163 6b61  jl)...This packa
+00000640: 6765 2070 726f 7669 6465 7320 6120 7079  ge provides a py
+00000650: 7468 6f6e 2069 6d70 6c65 6d65 6e74 6174  thon implementat
+00000660: 696f 6e20 6173 2074 6865 206d 6f64 756c  ion as the modul
+00000670: 6520 5f70 7963 6174 6368 3232 5f2c 206c  e _pycatch22_, l
+00000680: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
+00000690: 6520 5b47 4e55 2047 504c 2076 3320 6c69  e [GNU GPL v3 li
+000006a0: 6365 6e73 655d 2868 7474 703a 2f2f 7777  cense](http://ww
+000006b0: 772e 676e 752e 6f72 672f 6c69 6365 6e73  w.gnu.org/licens
+000006c0: 6573 2f67 706c 2d33 2e30 2e68 746d 6c29  es/gpl-3.0.html)
+000006d0: 2028 6f72 206c 6174 6572 292e 0a0a 2323   (or later)...##
+000006e0: 2320 5768 6174 2064 6f20 7468 6520 6665  # What do the fe
+000006f0: 6174 7572 6573 2064 6f3f 0a0a 5468 6973  atures do?..This
+00000700: 205b 4769 7442 6f6f 6b73 2077 6562 7369   [GitBooks websi
+00000710: 7465 5d28 6874 7470 733a 2f2f 7469 6d65  te](https://time
+00000720: 2d73 6572 6965 732d 6665 6174 7572 6573  -series-features
+00000730: 2e67 6974 626f 6f6b 2e69 6f2f 6361 7463  .gitbook.io/catc
+00000740: 6832 322f 6665 6174 7572 652d 6465 7363  h22/feature-desc
+00000750: 7269 7074 696f 6e73 2920 6973 2064 6564  riptions) is ded
+00000760: 6963 6174 6564 2074 6f20 6465 7363 7269  icated to descri
+00000770: 6269 6e67 2074 6865 2066 6561 7475 7265  bing the feature
+00000780: 732e 0a46 6f72 2074 6865 6972 2069 6d70  s..For their imp
+00000790: 6c65 6d65 6e74 6174 696f 6e20 696e 2063  lementation in c
+000007a0: 6f64 652c 2073 6565 2074 6865 205b 6d61  ode, see the [ma
+000007b0: 696e 205f 6361 7463 6832 325f 2072 6570  in _catch22_ rep
+000007c0: 6f73 6974 6f72 795d 2868 7474 7073 3a2f  ository](https:/
+000007d0: 2f67 6974 6875 622e 636f 6d2f 4479 6e61  /github.com/Dyna
+000007e0: 6d69 6373 416e 644e 6575 7261 6c53 7973  micsAndNeuralSys
+000007f0: 7465 6d73 2f63 6174 6368 3232 292e 0a54  tems/catch22)..T
+00000800: 6865 7265 2069 7320 616c 736f 2069 6e66  here is also inf
+00000810: 6f72 6d61 7469 6f6e 2069 6e20 7468 6520  ormation in the 
+00000820: 6173 736f 6369 6174 6564 2070 6170 6572  associated paper
+00000830: 205b 2623 7831 4634 4437 3b20 4c75 6262   [&#x1F4D7; Lubb
+00000840: 6120 6574 2061 6c2e 2028 3230 3139 292e  a et al. (2019).
+00000850: 5d28 6874 7470 733a 2f2f 646f 692e 6f72  ](https://doi.or
+00000860: 672f 3130 2e31 3030 372f 7331 3036 3138  g/10.1007/s10618
+00000870: 2d30 3139 2d30 3036 3437 2d78 292e 0a0a  -019-00647-x)...
+00000880: 2323 2320 4163 6b6e 6f77 6c65 6467 656d  ### Acknowledgem
+00000890: 656e 7420 3a2b 313a 0a0a 4966 2079 6f75  ent :+1:..If you
+000008a0: 2075 7365 2074 6869 7320 736f 6674 7761   use this softwa
+000008b0: 7265 2c20 706c 6561 7365 2072 6561 6420  re, please read 
+000008c0: 616e 6420 6369 7465 2074 6869 7320 6f70  and cite this op
+000008d0: 656e 2d61 6363 6573 7320 6172 7469 636c  en-access articl
+000008e0: 653a 0a0a 2d20 2623 7831 4634 4437 3b20  e:..- &#x1F4D7; 
+000008f0: 4c75 6262 6120 6574 2061 6c2e 205b 5f63  Lubba et al. [_c
+00000900: 6174 6368 3232 5f3a 2043 416e 6f6e 6963  atch22_: CAnonic
+00000910: 616c 2054 696d 652d 7365 7269 6573 2043  al Time-series C
+00000920: 4861 7261 6374 6572 6973 7469 6373 5d28  Haracteristics](
+00000930: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
+00000940: 3130 2e31 3030 372f 7331 3036 3138 2d30  10.1007/s10618-0
+00000950: 3139 2d30 3036 3437 2d78 292c 205f 4461  19-00647-x), _Da
+00000960: 7461 204d 696e 204b 6e6f 776c 2044 6973  ta Min Knowl Dis
+00000970: 635f 205f 5f33 335f 5f2c 2031 3832 3120  c_ __33__, 1821 
+00000980: 2832 3031 3929 2e0a 0a23 2320 496e 7374  (2019)...## Inst
+00000990: 616c 6c61 7469 6f6e 0a0a 5573 696e 6720  allation..Using 
+000009a0: 6070 6970 6020 666f 7220 5b60 7079 6361  `pip` for [`pyca
+000009b0: 7463 6832 3260 5d28 6874 7470 733a 2f2f  tch22`](https://
+000009c0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000009d0: 2f70 7963 6174 6368 3232 2f29 3a0a 0a60  /pycatch22/):..`
+000009e0: 6060 0a70 6970 2069 6e73 7461 6c6c 2070  ``.pip install p
+000009f0: 7963 6174 6368 3232 0a60 6060 0a0a 4966  ycatch22.```..If
+00000a00: 2074 6869 7320 646f 6573 6e27 7420 776f   this doesn't wo
+00000a10: 726b 2c20 6d61 6b65 2073 7572 6520 796f  rk, make sure yo
+00000a20: 7520 6172 6520 7573 696e 6720 7468 6520  u are using the 
+00000a30: 6c61 7465 7374 2060 7365 7475 7074 6f6f  latest `setuptoo
+00000a40: 6c73 603a 2060 7069 7020 696e 7374 616c  ls`: `pip instal
+00000a50: 6c20 7365 7475 7074 6f6f 6c73 202d 2d75  l setuptools --u
+00000a60: 7067 7261 6465 602e 0a0a 4966 2079 6f75  pgrade`...If you
+00000a70: 2063 6f6d 6520 6163 726f 7373 2065 7272   come across err
+00000a80: 6f72 7320 7769 7468 2076 6572 7369 6f6e  ors with version
+00000a90: 2072 6573 6f6c 7574 696f 6e2c 2079 6f75   resolution, you
+00000aa0: 2073 686f 756c 6420 7472 7920 736f 6d65   should try some
+00000ab0: 7468 696e 6720 6c69 6b65 3a20 6070 6970  thing like: `pip
+00000ac0: 2069 6e73 7461 6c6c 2070 7963 6174 6368   install pycatch
+00000ad0: 3232 3d3d 302e 342e 3220 2d2d 7573 652d  22==0.4.2 --use-
+00000ae0: 6465 7072 6563 6174 6564 3d6c 6567 6163  deprecated=legac
+00000af0: 792d 7265 736f 6c76 6572 602e 0a0a 4974  y-resolver`...It
+00000b00: 2069 7320 616c 736f 2061 205b 7061 636b   is also a [pack
+00000b10: 6167 6520 6f6e 2061 6e61 636f 6e64 615d  age on anaconda]
+00000b20: 2868 7474 7073 3a2f 2f61 6e61 636f 6e64  (https://anacond
+00000b30: 612e 6f72 672f 636f 6e64 612d 666f 7267  a.org/conda-forg
+00000b40: 652f 7079 6361 7463 6832 3229 2074 6861  e/pycatch22) tha
+00000b50: 6e6b 7320 746f 205b 4072 7061 6e61 695d  nks to [@rpanai]
+00000b60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000b70: 636f 6d2f 7270 616e 6169 292c 2077 6869  com/rpanai), whi
+00000b80: 6368 2079 6f75 2063 616e 2069 6e73 7461  ch you can insta
+00000b90: 6c6c 2076 6961 2060 636f 6e64 6160 3a0a  ll via `conda`:.
+00000ba0: 0a60 6060 0a63 6f6e 6461 2069 6e73 7461  .```.conda insta
+00000bb0: 6c6c 202d 6320 636f 6e64 612d 666f 7267  ll -c conda-forg
+00000bc0: 6520 7079 6361 7463 6832 320a 6060 600a  e pycatch22.```.
+00000bd0: 0a6f 7220 606d 616d 6261 603a 0a0a 6060  .or `mamba`:..``
+00000be0: 600a 6d61 6d62 6120 696e 7374 616c 6c20  `.mamba install 
+00000bf0: 2d63 2063 6f6e 6461 2d66 6f72 6765 2070  -c conda-forge p
+00000c00: 7963 6174 6368 3232 0a60 6060 0a0a 5b41  ycatch22.```..[A
+00000c10: 206d 616e 7561 6c20 696e 7374 616c 6c20   manual install 
+00000c20: 2862 6f74 746f 6d20 6f66 2074 6869 7320  (bottom of this 
+00000c30: 7061 6765 2920 6973 2061 206c 6173 7420  page) is a last 
+00000c40: 7265 736f 7274 2e5d 0a0a 2323 2055 7361  resort.]..## Usa
+00000c50: 6765 0a0a 4561 6368 2066 6561 7475 7265  ge..Each feature
+00000c60: 2066 756e 6374 696f 6e20 6361 6e20 6265   function can be
+00000c70: 2061 6363 6573 7365 6420 696e 6469 7669   accessed indivi
+00000c80: 6475 616c 6c79 2061 6e64 2074 616b 6573  dually and takes
+00000c90: 2061 7272 6179 7320 6173 2074 7570 6c65   arrays as tuple
+00000ca0: 206f 7220 6c69 7374 7320 286e 6f74 2060   or lists (not `
+00000cb0: 6e75 6d70 7960 2061 7272 6179 7329 2e0a  numpy` arrays)..
+00000cc0: 466f 7220 6578 616d 706c 652c 2066 6f72  For example, for
+00000cd0: 206c 6f61 6465 6420 6461 7461 2060 7473   loaded data `ts
+00000ce0: 4461 7461 6020 696e 2050 7974 686f 6e3a  Data` in Python:
+00000cf0: 0a0a 6060 6070 7974 686f 6e33 0a69 6d70  ..```python3.imp
+00000d00: 6f72 7420 7079 6361 7463 6832 320a 7473  ort pycatch22.ts
+00000d10: 4461 7461 203d 205b 312c 322c 342c 335d  Data = [1,2,4,3]
+00000d20: 2023 2028 6f72 206d 6f72 6520 696e 7465   # (or more inte
+00000d30: 7265 7374 696e 6720 6461 7461 2129 0a70  resting data!).p
+00000d40: 7963 6174 6368 3232 2e43 4f5f 6631 6563  ycatch22.CO_f1ec
+00000d50: 6163 2874 7344 6174 6129 0a60 6060 0a0a  ac(tsData).```..
+00000d60: 416c 6c20 6665 6174 7572 6573 2061 7265  All features are
+00000d70: 2062 756e 646c 6564 2069 6e20 7468 6520   bundled in the 
+00000d80: 6d65 7468 6f64 2060 6361 7463 6832 325f  method `catch22_
+00000d90: 616c 6c60 2c20 7768 6963 6820 616c 736f  all`, which also
+00000da0: 2061 6363 6570 7473 2060 6e75 6d70 7960   accepts `numpy`
+00000db0: 2061 7272 6179 7320 616e 6420 6769 7665   arrays and give
+00000dc0: 7320 6261 636b 2061 2064 6963 7469 6f6e  s back a diction
+00000dd0: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
+00000de0: 6865 2065 6e74 7269 6573 2060 6361 7463  he entries `catc
+00000df0: 6832 325f 616c 6c5b 276e 616d 6573 275d  h22_all['names']
+00000e00: 6020 666f 7220 6665 6174 7572 6520 6e61  ` for feature na
+00000e10: 6d65 7320 616e 6420 6063 6174 6368 3232  mes and `catch22
+00000e20: 5f61 6c6c 5b27 7661 6c75 6573 275d 6020  _all['values']` 
+00000e30: 666f 7220 6665 6174 7572 6520 6f75 7470  for feature outp
+00000e40: 7574 732e 0a0a 5573 6167 6520 2863 6f6d  uts...Usage (com
+00000e50: 7075 7469 6e67 2032 3220 6665 6174 7572  puting 22 featur
+00000e60: 6573 3a20 5f63 6174 6368 3232 5f29 3a0a  es: _catch22_):.
+00000e70: 0a60 6060 7079 7468 6f6e 330a 7079 6361  .```python3.pyca
+00000e80: 7463 6832 322e 6361 7463 6832 325f 616c  tch22.catch22_al
+00000e90: 6c28 7473 4461 7461 290a 6060 600a 0a55  l(tsData).```..U
+00000ea0: 7361 6765 2028 636f 6d70 7574 696e 6720  sage (computing 
+00000eb0: 3234 2066 6561 7475 7265 733a 205f 6361  24 features: _ca
+00000ec0: 7463 6832 345f 203d 205f 6361 7463 6832  tch24_ = _catch2
+00000ed0: 325f 202b 206d 6561 6e20 2b20 7374 616e  2_ + mean + stan
+00000ee0: 6461 7264 2064 6576 6961 7469 6f6e 293a  dard deviation):
+00000ef0: 0a0a 6060 6070 7974 686f 6e33 0a70 7963  ..```python3.pyc
+00000f00: 6174 6368 3232 2e63 6174 6368 3232 5f61  atch22.catch22_a
+00000f10: 6c6c 2874 7344 6174 612c 6361 7463 6832  ll(tsData,catch2
+00000f20: 343d 5472 7565 290a 6060 600a 0a57 6520  4=True).```..We 
+00000f30: 616c 736f 2069 6e63 6c75 6465 2061 2027  also include a '
+00000f40: 7368 6f72 7420 6e61 6d65 2720 666f 7220  short name' for 
+00000f50: 6561 6368 2066 6561 7475 7265 2066 6f72  each feature for
+00000f60: 2065 6173 6965 7220 7265 6665 7265 6e63   easier referenc
+00000f70: 6520 2861 7320 6f75 746c 696e 6564 2069  e (as outlined i
+00000f80: 6e20 7468 6520 4769 7442 6f6f 6b20 5b46  n the GitBook [F
+00000f90: 6561 7475 7265 206f 7665 7276 6965 7720  eature overview 
+00000fa0: 7461 626c 655d 2868 7474 7073 3a2f 2f74  table](https://t
+00000fb0: 696d 652d 7365 7269 6573 2d66 6561 7475  ime-series-featu
+00000fc0: 7265 732e 6769 7462 6f6f 6b2e 696f 2f63  res.gitbook.io/c
+00000fd0: 6174 6368 3232 2f66 6561 7475 7265 2d64  atch22/feature-d
+00000fe0: 6573 6372 6970 7469 6f6e 732f 6665 6174  escriptions/feat
+00000ff0: 7572 652d 6f76 6572 7669 6577 2d74 6162  ure-overview-tab
+00001000: 6c65 2929 2e0a 5468 6573 6520 7368 6f72  le))..These shor
+00001010: 7420 6e61 6d65 7320 6361 6e20 6265 2069  t names can be i
+00001020: 6e63 6c75 6465 6420 696e 2074 6865 206f  ncluded in the o
+00001030: 7574 7075 7420 6672 6f6d 2060 6361 7463  utput from `catc
+00001040: 6832 325f 616c 6c28 2960 2062 7920 7365  h22_all()` by se
+00001050: 7474 696e 6720 6073 686f 7274 5f6e 616d  tting `short_nam
+00001060: 6573 3d54 7275 6560 2061 7320 666f 6c6c  es=True` as foll
+00001070: 6f77 733a 0a0a 6060 6070 7974 686f 6e33  ows:..```python3
+00001080: 0a70 7963 6174 6368 3232 2e63 6174 6368  .pycatch22.catch
+00001090: 3232 5f61 6c6c 2874 7344 6174 612c 6361  22_all(tsData,ca
+000010a0: 7463 6832 343d 5472 7565 2c73 686f 7274  tch24=True,short
+000010b0: 5f6e 616d 6573 3d54 7275 6529 0a60 6060  _names=True).```
+000010c0: 0a0a 2323 2320 5465 6d70 6c61 7465 2061  ..### Template a
+000010d0: 6e61 6c79 7369 7320 7363 7269 7074 0a0a  nalysis script..
+000010e0: 5468 616e 6b73 2074 6f20 5b40 6a6d 6f6f  Thanks to [@jmoo
+000010f0: 3238 3830 5d28 6874 7470 733a 2f2f 6769  2880](https://gi
+00001100: 7468 7562 2e63 6f6d 2f6a 6d6f 6f32 3838  thub.com/jmoo288
+00001110: 3029 2066 6f72 2070 7574 7469 6e67 2074  0) for putting t
+00001120: 6f67 6574 6865 7220 6120 5b64 656d 6f6e  ogether a [demon
+00001130: 7374 7261 7469 6f6e 206e 6f74 6562 6f6f  stration noteboo
+00001140: 6b5d 2868 7474 7073 3a2f 2f67 6974 6875  k](https://githu
+00001150: 622e 636f 6d2f 6a6d 6f6f 3238 3830 2f63  b.com/jmoo2880/c
+00001160: 3232 2d75 7361 6765 2d65 7861 6d70 6c65  22-usage-example
+00001170: 732f 2920 666f 7220 7573 696e 6720 7079  s/) for using py
+00001180: 6361 7463 6832 3220 746f 2065 7874 7261  catch22 to extra
+00001190: 6374 2066 6561 7475 7265 7320 6672 6f6d  ct features from
+000011a0: 2061 2074 696d 652d 7365 7269 6573 2064   a time-series d
+000011b0: 6174 6173 6574 2e0a 0a23 2323 2055 7361  ataset...### Usa
+000011c0: 6765 206e 6f74 6573 0a0a 2d20 5768 656e  ge notes..- When
+000011d0: 2070 7265 7365 6e74 696e 6720 7265 7375   presenting resu
+000011e0: 6c74 7320 7573 696e 6720 5f63 6174 6368  lts using _catch
+000011f0: 3232 5f2c 2079 6f75 206d 7573 7420 6964  22_, you must id
+00001200: 656e 7469 6679 2074 6865 2076 6572 7369  entify the versi
+00001210: 6f6e 2075 7365 6420 746f 2061 6c6c 6f77  on used to allow
+00001220: 2063 6c65 6172 2072 6570 726f 6475 6374   clear reproduct
+00001230: 696f 6e20 6f66 2079 6f75 7220 7265 7375  ion of your resu
+00001240: 6c74 732e 2046 6f72 2065 7861 6d70 6c65  lts. For example
+00001250: 2c20 6043 4f5f 6631 6563 6163 6020 7761  , `CO_f1ecac` wa
+00001260: 7320 616c 7465 7265 6420 6672 6f6d 2061  s altered from a
+00001270: 6e20 696e 7465 6765 722d 7661 6c75 6564  n integer-valued
+00001280: 206f 7574 7075 7420 746f 2061 206c 696e   output to a lin
+00001290: 6561 726c 7920 696e 7465 7270 6f6c 6174  early interpolat
+000012a0: 6564 2072 6561 6c2d 7661 6c75 6564 206f  ed real-valued o
+000012b0: 7574 7075 7420 6672 6f6d 2076 302e 332e  utput from v0.3.
+000012c0: 0a2d 205f 5f49 6d70 6f72 7461 6e74 204e  .- __Important N
+000012d0: 6f74 653a 5f5f 205f 6361 7463 6832 325f  ote:__ _catch22_
+000012e0: 2066 6561 7475 7265 7320 6f6e 6c79 2065   features only e
+000012f0: 7661 6c75 6174 6520 5f64 796e 616d 6963  valuate _dynamic
+00001300: 616c 5f20 7072 6f70 6572 7469 6573 206f  al_ properties o
+00001310: 6620 7469 6d65 2073 6572 6965 7320 616e  f time series an
+00001320: 6420 646f 206e 6f74 2072 6573 706f 6e64  d do not respond
+00001330: 2074 6f20 6261 7369 6320 6469 6666 6572   to basic differ
+00001340: 656e 6365 7320 696e 2074 6865 206c 6f63  ences in the loc
+00001350: 6174 696f 6e20 2865 2e67 2e2c 206d 6561  ation (e.g., mea
+00001360: 6e29 206f 7220 7370 7265 6164 2028 652e  n) or spread (e.
+00001370: 672e 2c20 7661 7269 616e 6365 292e 0a20  g., variance).. 
+00001380: 202d 2046 726f 6d20 5f63 6174 6368 3232   - From _catch22
+00001390: 5f20 7630 2e33 2c20 4966 2074 6865 206c  _ v0.3, If the l
+000013a0: 6f63 6174 696f 6e20 616e 6420 7370 7265  ocation and spre
+000013b0: 6164 206f 6620 7468 6520 7261 7720 7469  ad of the raw ti
+000013c0: 6d65 2d73 6572 6965 7320 6469 7374 7269  me-series distri
+000013d0: 6275 7469 6f6e 206d 6179 2062 6520 696d  bution may be im
+000013e0: 706f 7274 616e 7420 666f 7220 796f 7572  portant for your
+000013f0: 2061 7070 6c69 6361 7469 6f6e 2c20 7765   application, we
+00001400: 2073 7567 6765 7374 2061 7070 6c79 696e   suggest applyin
+00001410: 6720 7468 6520 6675 6e63 7469 6f6e 2061  g the function a
+00001420: 7267 756d 656e 7420 6063 6174 6368 3234  rgument `catch24
+00001430: 203d 2054 7275 6560 2074 6f20 796f 7572   = True` to your
+00001440: 2063 616c 6c20 746f 2074 6865 205f 6361   call to the _ca
+00001450: 7463 6832 325f 2066 756e 6374 696f 6e20  tch22_ function 
+00001460: 696e 2074 6865 206c 616e 6775 6167 6520  in the language 
+00001470: 6f66 2079 6f75 7220 6368 6f69 6365 2e0a  of your choice..
+00001480: 2020 5468 6973 2077 696c 6c20 7265 7375    This will resu
+00001490: 6c74 2069 6e20 3234 2066 6561 7475 7265  lt in 24 feature
+000014a0: 7320 6265 696e 6720 6361 6c63 756c 6174  s being calculat
+000014b0: 6564 3a20 7468 6520 5f63 6174 6368 3232  ed: the _catch22
+000014c0: 5f20 6665 6174 7572 6573 2069 6e20 6164  _ features in ad
+000014d0: 6469 7469 6f6e 2074 6f20 6d65 616e 2061  dition to mean a
+000014e0: 6e64 2073 7461 6e64 6172 6420 6465 7669  nd standard devi
+000014f0: 6174 696f 6e2e 0a0a 2323 2320 4d61 6e75  ation...### Manu
+00001500: 616c 2069 6e73 7461 6c6c 0a0a 4966 2079  al install..If y
+00001510: 6f75 2066 696e 6420 6973 7375 6573 2077  ou find issues w
+00001520: 6974 6820 7468 6520 6070 6970 6020 696e  ith the `pip` in
+00001530: 7374 616c 6c2c 2079 6f75 2063 616e 2061  stall, you can a
+00001540: 6c73 6f20 696e 7374 616c 6c20 7573 696e  lso install usin
+00001550: 6720 6073 6574 7570 746f 6f6c 7360 3a0a  g `setuptools`:.
+00001560: 0a60 6060 0a70 7974 686f 6e33 2073 6574  .```.python3 set
+00001570: 7570 2e70 7920 6275 696c 640a 7079 7468  up.py build.pyth
+00001580: 6f6e 3320 7365 7475 702e 7079 2069 6e73  on3 setup.py ins
+00001590: 7461 6c6c 0a60 6060 0a                   tall.```.
```

### Comparing `pycatch22-0.4.4/README.md` & `pycatch22-0.4.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,277 +1,302 @@
-00000000: 2320 5f70 7963 6174 6368 3232 5f20 2d20  # _pycatch22_ - 
-00000010: 4341 6e6f 6e69 6361 6c20 5469 6d65 2d73  CAnonical Time-s
-00000020: 6572 6965 7320 4348 6172 6163 7465 7269  eries CHaracteri
-00000030: 7374 6963 7320 696e 2070 7974 686f 6e0a  stics in python.
-00000040: 0a3c 696d 6720 7372 633d 2269 6d67 2f63  .<img src="img/c
-00000050: 6174 6368 3232 5f6c 6f67 6f5f 7371 7561  atch22_logo_squa
-00000060: 7265 2e70 6e67 2220 7769 6474 683d 2232  re.png" width="2
-00000070: 3530 2220 6865 6967 6874 3d22 3235 3022  50" height="250"
-00000080: 2f3e 0a0a 2323 2041 626f 7574 0a0a 5b5f  />..## About..[_
-00000090: 6361 7463 6832 325f 5d28 6874 7470 733a  catch22_](https:
-000000a0: 2f2f 6769 7468 7562 2e63 6f6d 2f44 796e  //github.com/Dyn
-000000b0: 616d 6963 7341 6e64 4e65 7572 616c 5379  amicsAndNeuralSy
-000000c0: 7374 656d 732f 6361 7463 6832 3229 2069  stems/catch22) i
-000000d0: 7320 6120 636f 6c6c 6563 7469 6f6e 206f  s a collection o
-000000e0: 6620 3232 2074 696d 652d 7365 7269 6573  f 22 time-series
-000000f0: 2066 6561 7475 7265 7320 636f 6465 6420   features coded 
-00000100: 696e 2043 2074 6861 7420 6361 6e20 6265  in C that can be
-00000110: 2072 756e 2066 726f 6d20 5079 7468 6f6e   run from Python
-00000120: 2c20 6173 2077 656c 6c20 6173 205b 525d  , as well as [R]
-00000130: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000140: 636f 6d2f 6865 6e64 6572 736f 6e74 7265  com/hendersontre
-00000150: 6e74 2f52 6361 7463 6832 3229 2c20 5b4d  nt/Rcatch22), [M
-00000160: 6174 6c61 625d 2868 7474 7073 3a2f 2f67  atlab](https://g
-00000170: 6974 6875 622e 636f 6d2f 4479 6e61 6d69  ithub.com/Dynami
-00000180: 6373 416e 644e 6575 7261 6c53 7973 7465  csAndNeuralSyste
-00000190: 6d73 2f63 6174 6368 3232 292c 2061 6e64  ms/catch22), and
-000001a0: 205b 4a75 6c69 615d 2868 7474 7073 3a2f   [Julia](https:/
-000001b0: 2f67 6974 6875 622e 636f 6d2f 6272 656e  /github.com/bren
-000001c0: 6461 6e6a 6f68 6e68 6172 7269 732f 4361  danjohnharris/Ca
-000001d0: 7463 6832 322e 6a6c 292e 0a0a 5468 6973  tch22.jl)...This
-000001e0: 2070 6163 6b61 6765 2070 726f 7669 6465   package provide
-000001f0: 7320 6120 7079 7468 6f6e 2069 6d70 6c65  s a python imple
-00000200: 6d65 6e74 6174 696f 6e20 6173 2074 6865  mentation as the
-00000210: 206d 6f64 756c 6520 5f70 7963 6174 6368   module _pycatch
-00000220: 3232 5f2c 206c 6963 656e 7365 6420 756e  22_, licensed un
-00000230: 6465 7220 7468 6520 5b47 4e55 2047 504c  der the [GNU GPL
-00000240: 2076 3320 6c69 6365 6e73 655d 2868 7474   v3 license](htt
-00000250: 703a 2f2f 7777 772e 676e 752e 6f72 672f  p://www.gnu.org/
-00000260: 6c69 6365 6e73 6573 2f67 706c 2d33 2e30  licenses/gpl-3.0
-00000270: 2e68 746d 6c29 2028 6f72 206c 6174 6572  .html) (or later
-00000280: 292e 0a0a 2323 2320 5768 6174 2064 6f20  )...### What do 
-00000290: 7468 6520 6665 6174 7572 6573 2064 6f3f  the features do?
-000002a0: 0a0a 5468 6973 205b 4769 7442 6f6f 6b73  ..This [GitBooks
-000002b0: 2077 6562 7369 7465 5d28 6874 7470 733a   website](https:
-000002c0: 2f2f 6665 6174 7572 652d 6261 7365 642d  //feature-based-
-000002d0: 7469 6d65 2d73 6572 6965 732d 616e 616c  time-series-anal
-000002e0: 7973 2e67 6974 626f 6f6b 2e69 6f2f 6361  ys.gitbook.io/ca
-000002f0: 7463 6832 322d 6665 6174 7572 6573 2f29  tch22-features/)
-00000300: 2069 7320 6465 6469 6361 7465 6420 746f   is dedicated to
-00000310: 2064 6573 6372 6962 696e 6720 7468 6520   describing the 
-00000320: 6665 6174 7572 6573 2e0a 466f 7220 7468  features..For th
-00000330: 6569 7220 696d 706c 656d 656e 7461 7469  eir implementati
-00000340: 6f6e 2069 6e20 636f 6465 2c20 7365 6520  on in code, see 
-00000350: 7468 6520 5b6d 6169 6e20 5f63 6174 6368  the [main _catch
-00000360: 3232 5f20 7265 706f 7369 746f 7279 5d28  22_ repository](
-00000370: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000380: 6f6d 2f44 796e 616d 6963 7341 6e64 4e65  om/DynamicsAndNe
-00000390: 7572 616c 5379 7374 656d 732f 6361 7463  uralSystems/catc
-000003a0: 6832 3229 2e0a 5468 6572 6520 6973 2061  h22)..There is a
-000003b0: 6c73 6f20 696e 666f 726d 6174 696f 6e20  lso information 
-000003c0: 696e 2074 6865 2061 7373 6f63 6961 7465  in the associate
-000003d0: 6420 7061 7065 7220 5b26 2378 3146 3444  d paper [&#x1F4D
-000003e0: 373b 204c 7562 6261 2065 7420 616c 2e20  7; Lubba et al. 
-000003f0: 2832 3031 3929 2e5d 2868 7474 7073 3a2f  (2019).](https:/
-00000400: 2f64 6f69 2e6f 7267 2f31 302e 3130 3037  /doi.org/10.1007
-00000410: 2f73 3130 3631 382d 3031 392d 3030 3634  /s10618-019-0064
-00000420: 372d 7829 2e0a 0a23 2323 2041 636b 6e6f  7-x)...### Ackno
-00000430: 776c 6564 6765 6d65 6e74 203a 2b31 3a0a  wledgement :+1:.
-00000440: 0a49 6620 796f 7520 7573 6520 7468 6973  .If you use this
-00000450: 2073 6f66 7477 6172 652c 2070 6c65 6173   software, pleas
-00000460: 6520 7265 6164 2061 6e64 2063 6974 6520  e read and cite 
-00000470: 7468 6973 206f 7065 6e2d 6163 6365 7373  this open-access
-00000480: 2061 7274 6963 6c65 3a0a 0a2d 2026 2378   article:..- &#x
-00000490: 3146 3444 373b 204c 7562 6261 2065 7420  1F4D7; Lubba et 
-000004a0: 616c 2e20 5b5f 6361 7463 6832 325f 3a20  al. [_catch22_: 
-000004b0: 4341 6e6f 6e69 6361 6c20 5469 6d65 2d73  CAnonical Time-s
-000004c0: 6572 6965 7320 4348 6172 6163 7465 7269  eries CHaracteri
-000004d0: 7374 6963 735d 2868 7474 7073 3a2f 2f64  stics](https://d
-000004e0: 6f69 2e6f 7267 2f31 302e 3130 3037 2f73  oi.org/10.1007/s
-000004f0: 3130 3631 382d 3031 392d 3030 3634 372d  10618-019-00647-
-00000500: 7829 2c20 5f44 6174 6120 4d69 6e20 4b6e  x), _Data Min Kn
-00000510: 6f77 6c20 4469 7363 5f20 5f5f 3333 5f5f  owl Disc_ __33__
-00000520: 2c20 3138 3231 2028 3230 3139 292e 0a0a  , 1821 (2019)...
-00000530: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
-00000540: 0a55 7369 6e67 2060 7069 7060 2066 6f72  .Using `pip` for
-00000550: 205b 6070 7963 6174 6368 3232 605d 2868   [`pycatch22`](h
-00000560: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000570: 7072 6f6a 6563 742f 7079 6361 7463 6832  project/pycatch2
-00000580: 322f 293a 0a0a 6060 600a 7069 7020 696e  2/):..```.pip in
-00000590: 7374 616c 6c20 7079 6361 7463 6832 320a  stall pycatch22.
-000005a0: 6060 600a 0a49 6620 7468 6973 2064 6f65  ```..If this doe
-000005b0: 736e 2774 2077 6f72 6b2c 206d 616b 6520  sn't work, make 
-000005c0: 7375 7265 2079 6f75 2061 7265 2075 7369  sure you are usi
-000005d0: 6e67 2074 6865 206c 6174 6573 7420 6073  ng the latest `s
-000005e0: 6574 7570 746f 6f6c 7360 3a20 6070 6970  etuptools`: `pip
-000005f0: 2069 6e73 7461 6c6c 2073 6574 7570 746f   install setupto
-00000600: 6f6c 7320 2d2d 7570 6772 6164 6560 2e0a  ols --upgrade`..
-00000610: 0a49 6620 796f 7520 636f 6d65 2061 6372  .If you come acr
-00000620: 6f73 7320 6572 726f 7273 2077 6974 6820  oss errors with 
-00000630: 7665 7273 696f 6e20 7265 736f 6c75 7469  version resoluti
-00000640: 6f6e 2c20 796f 7520 7368 6f75 6c64 2074  on, you should t
-00000650: 7279 2073 6f6d 6574 6869 6e67 206c 696b  ry something lik
-00000660: 653a 2060 7069 7020 696e 7374 616c 6c20  e: `pip install 
-00000670: 7079 6361 7463 6832 323d 3d30 2e34 2e32  pycatch22==0.4.2
-00000680: 202d 2d75 7365 2d64 6570 7265 6361 7465   --use-deprecate
-00000690: 643d 6c65 6761 6379 2d72 6573 6f6c 7665  d=legacy-resolve
-000006a0: 7260 2e0a 0a49 7420 6973 2061 6c73 6f20  r`...It is also 
-000006b0: 6120 5b70 6163 6b61 6765 206f 6e20 616e  a [package on an
-000006c0: 6163 6f6e 6461 5d28 6874 7470 733a 2f2f  aconda](https://
-000006d0: 616e 6163 6f6e 6461 2e6f 7267 2f63 6f6e  anaconda.org/con
-000006e0: 6461 2d66 6f72 6765 2f70 7963 6174 6368  da-forge/pycatch
-000006f0: 3232 2920 7468 616e 6b73 2074 6f20 5b40  22) thanks to [@
-00000700: 7270 616e 6169 5d28 6874 7470 733a 2f2f  rpanai](https://
-00000710: 6769 7468 7562 2e63 6f6d 2f72 7061 6e61  github.com/rpana
-00000720: 6929 2c20 7768 6963 6820 796f 7520 6361  i), which you ca
-00000730: 6e20 696e 7374 616c 6c20 7669 6120 6063  n install via `c
-00000740: 6f6e 6461 603a 0a0a 6060 600a 636f 6e64  onda`:..```.cond
-00000750: 6120 696e 7374 616c 6c20 2d63 2063 6f6e  a install -c con
-00000760: 6461 2d66 6f72 6765 2070 7963 6174 6368  da-forge pycatch
-00000770: 3232 0a60 6060 0a0a 6f72 2060 6d61 6d62  22.```..or `mamb
-00000780: 6160 3a0a 0a60 6060 0a6d 616d 6261 2069  a`:..```.mamba i
-00000790: 6e73 7461 6c6c 202d 6320 636f 6e64 612d  nstall -c conda-
-000007a0: 666f 7267 6520 7079 6361 7463 6832 320a  forge pycatch22.
-000007b0: 6060 600a 0a5b 4120 6d61 6e75 616c 2069  ```..[A manual i
-000007c0: 6e73 7461 6c6c 2028 626f 7474 6f6d 206f  nstall (bottom o
-000007d0: 6620 7468 6973 2070 6167 6529 2069 7320  f this page) is 
-000007e0: 6120 6c61 7374 2072 6573 6f72 742e 5d0a  a last resort.].
-000007f0: 0a23 2320 5573 6167 650a 0a45 6163 6820  .## Usage..Each 
-00000800: 6665 6174 7572 6520 6675 6e63 7469 6f6e  feature function
-00000810: 2063 616e 2062 6520 6163 6365 7373 6564   can be accessed
-00000820: 2069 6e64 6976 6964 7561 6c6c 7920 616e   individually an
-00000830: 6420 7461 6b65 7320 6172 7261 7973 2061  d takes arrays a
-00000840: 7320 7475 706c 6520 6f72 206c 6973 7473  s tuple or lists
-00000850: 2028 6e6f 7420 606e 756d 7079 6020 6172   (not `numpy` ar
-00000860: 7261 7973 292e 0a46 6f72 2065 7861 6d70  rays)..For examp
-00000870: 6c65 2c20 666f 7220 6c6f 6164 6564 2064  le, for loaded d
-00000880: 6174 6120 6074 7344 6174 6160 2069 6e20  ata `tsData` in 
-00000890: 5079 7468 6f6e 3a0a 0a60 6060 7079 7468  Python:..```pyth
-000008a0: 6f6e 330a 696d 706f 7274 2070 7963 6174  on3.import pycat
-000008b0: 6368 3232 0a74 7344 6174 6120 3d20 5b31  ch22.tsData = [1
-000008c0: 2c32 2c34 2c33 5d20 2320 286f 7220 6d6f  ,2,4,3] # (or mo
-000008d0: 7265 2069 6e74 6572 6573 7469 6e67 2064  re interesting d
-000008e0: 6174 6121 290a 7079 6361 7463 6832 322e  ata!).pycatch22.
-000008f0: 434f 5f66 3165 6361 6328 7473 4461 7461  CO_f1ecac(tsData
-00000900: 290a 6060 600a 0a41 6c6c 2066 6561 7475  ).```..All featu
-00000910: 7265 7320 6172 6520 6275 6e64 6c65 6420  res are bundled 
-00000920: 696e 2074 6865 206d 6574 686f 6420 6063  in the method `c
-00000930: 6174 6368 3232 5f61 6c6c 602c 2077 6869  atch22_all`, whi
-00000940: 6368 2061 6c73 6f20 6163 6365 7074 7320  ch also accepts 
-00000950: 606e 756d 7079 6020 6172 7261 7973 2061  `numpy` arrays a
-00000960: 6e64 2067 6976 6573 2062 6163 6b20 6120  nd gives back a 
-00000970: 6469 6374 696f 6e61 7279 2063 6f6e 7461  dictionary conta
-00000980: 696e 696e 6720 7468 6520 656e 7472 6965  ining the entrie
-00000990: 7320 6063 6174 6368 3232 5f61 6c6c 5b27  s `catch22_all['
-000009a0: 6e61 6d65 7327 5d60 2066 6f72 2066 6561  names']` for fea
-000009b0: 7475 7265 206e 616d 6573 2061 6e64 2060  ture names and `
-000009c0: 6361 7463 6832 325f 616c 6c5b 2776 616c  catch22_all['val
-000009d0: 7565 7327 5d60 2066 6f72 2066 6561 7475  ues']` for featu
-000009e0: 7265 206f 7574 7075 7473 2e0a 0a55 7361  re outputs...Usa
-000009f0: 6765 2028 636f 6d70 7574 696e 6720 3232  ge (computing 22
-00000a00: 2066 6561 7475 7265 733a 205f 6361 7463   features: _catc
-00000a10: 6832 325f 293a 0a0a 6060 6070 7974 686f  h22_):..```pytho
-00000a20: 6e33 0a70 7963 6174 6368 3232 2e63 6174  n3.pycatch22.cat
-00000a30: 6368 3232 5f61 6c6c 2874 7344 6174 6129  ch22_all(tsData)
-00000a40: 0a60 6060 0a0a 5573 6167 6520 2863 6f6d  .```..Usage (com
-00000a50: 7075 7469 6e67 2032 3420 6665 6174 7572  puting 24 featur
-00000a60: 6573 3a20 5f63 6174 6368 3234 5f20 3d20  es: _catch24_ = 
-00000a70: 5f63 6174 6368 3232 5f20 2b20 6d65 616e  _catch22_ + mean
-00000a80: 202b 2073 7461 6e64 6172 6420 6465 7669   + standard devi
-00000a90: 6174 696f 6e29 3a0a 0a60 6060 7079 7468  ation):..```pyth
-00000aa0: 6f6e 330a 7079 6361 7463 6832 322e 6361  on3.pycatch22.ca
-00000ab0: 7463 6832 325f 616c 6c28 7473 4461 7461  tch22_all(tsData
-00000ac0: 2c63 6174 6368 3234 3d54 7275 6529 0a60  ,catch24=True).`
-00000ad0: 6060 0a0a 5765 2061 6c73 6f20 696e 636c  ``..We also incl
-00000ae0: 7564 6520 6120 2773 686f 7274 206e 616d  ude a 'short nam
-00000af0: 6527 2066 6f72 2065 6163 6820 6665 6174  e' for each feat
-00000b00: 7572 6520 666f 7220 6561 7369 6572 2072  ure for easier r
-00000b10: 6566 6572 656e 6365 2028 6173 206f 7574  eference (as out
-00000b20: 6c69 6e65 6420 696e 2074 6865 2047 6974  lined in the Git
-00000b30: 426f 6f6b 205b 4665 6174 7572 6520 6f76  Book [Feature ov
-00000b40: 6572 7669 6577 2074 6162 6c65 5d28 6874  erview table](ht
-00000b50: 7470 733a 2f2f 6170 702e 6769 7462 6f6f  tps://app.gitboo
-00000b60: 6b2e 636f 6d2f 6f2f 2d4d 6665 685a 7161  k.com/o/-MfehZqa
-00000b70: 4357 6e73 5352 4449 6455 4738 2f73 2f2d  CWnsSRDIdUG8/s/-
-00000b80: 4d66 4846 5934 6c76 7a4f 7a33 4950 6141  MfHFY4lvzOz3IPaA
-00000b90: 3377 6d2f 6665 6174 7572 652d 6f76 6572  3wm/feature-over
-00000ba0: 7669 6577 2d74 6162 6c65 2929 2e0a 5468  view-table))..Th
-00000bb0: 6573 6520 7368 6f72 7420 6e61 6d65 7320  ese short names 
-00000bc0: 6361 6e20 6265 2069 6e63 6c75 6465 6420  can be included 
-00000bd0: 696e 2074 6865 206f 7574 7075 7420 6672  in the output fr
-00000be0: 6f6d 2060 6361 7463 6832 325f 616c 6c28  om `catch22_all(
-00000bf0: 2960 2062 7920 7365 7474 696e 6720 6073  )` by setting `s
-00000c00: 686f 7274 5f6e 616d 6573 3d54 7275 6560  hort_names=True`
-00000c10: 2061 7320 666f 6c6c 6f77 733a 0a0a 6060   as follows:..``
-00000c20: 6070 7974 686f 6e33 0a70 7963 6174 6368  `python3.pycatch
-00000c30: 3232 2e63 6174 6368 3232 5f61 6c6c 2874  22.catch22_all(t
-00000c40: 7344 6174 612c 6361 7463 6832 343d 5472  sData,catch24=Tr
-00000c50: 7565 2c73 686f 7274 5f6e 616d 6573 3d54  ue,short_names=T
-00000c60: 7275 6529 0a60 6060 0a0a 2323 2320 5465  rue).```..### Te
-00000c70: 6d70 6c61 7465 2061 6e61 6c79 7369 7320  mplate analysis 
-00000c80: 7363 7269 7074 0a0a 5468 616e 6b73 2074  script..Thanks t
-00000c90: 6f20 5b40 6a6d 6f6f 3238 3830 5d28 6874  o [@jmoo2880](ht
-00000ca0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000cb0: 2f6a 6d6f 6f32 3838 3029 2066 6f72 2070  /jmoo2880) for p
-00000cc0: 7574 7469 6e67 2074 6f67 6574 6865 7220  utting together 
-00000cd0: 6120 5b64 656d 6f6e 7374 7261 7469 6f6e  a [demonstration
-00000ce0: 206e 6f74 6562 6f6f 6b5d 2868 7474 7073   notebook](https
-00000cf0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a6d  ://github.com/jm
-00000d00: 6f6f 3238 3830 2f63 3232 2d75 7361 6765  oo2880/c22-usage
-00000d10: 2d65 7861 6d70 6c65 732f 2920 666f 7220  -examples/) for 
-00000d20: 7573 696e 6720 7079 6361 7463 6832 3220  using pycatch22 
-00000d30: 746f 2065 7874 7261 6374 2066 6561 7475  to extract featu
-00000d40: 7265 7320 6672 6f6d 2061 2074 696d 652d  res from a time-
-00000d50: 7365 7269 6573 2064 6174 6173 6574 2e0a  series dataset..
-00000d60: 0a23 2323 2055 7361 6765 206e 6f74 6573  .### Usage notes
-00000d70: 0a0a 2d20 5768 656e 2070 7265 7365 6e74  ..- When present
-00000d80: 696e 6720 7265 7375 6c74 7320 7573 696e  ing results usin
-00000d90: 6720 5f63 6174 6368 3232 5f2c 2079 6f75  g _catch22_, you
-00000da0: 206d 7573 7420 6964 656e 7469 6679 2074   must identify t
-00000db0: 6865 2076 6572 7369 6f6e 2075 7365 6420  he version used 
-00000dc0: 746f 2061 6c6c 6f77 2063 6c65 6172 2072  to allow clear r
-00000dd0: 6570 726f 6475 6374 696f 6e20 6f66 2079  eproduction of y
-00000de0: 6f75 7220 7265 7375 6c74 732e 2046 6f72  our results. For
-00000df0: 2065 7861 6d70 6c65 2c20 6043 4f5f 6631   example, `CO_f1
-00000e00: 6563 6163 6020 7761 7320 616c 7465 7265  ecac` was altere
-00000e10: 6420 6672 6f6d 2061 6e20 696e 7465 6765  d from an intege
-00000e20: 722d 7661 6c75 6564 206f 7574 7075 7420  r-valued output 
-00000e30: 746f 2061 206c 696e 6561 726c 7920 696e  to a linearly in
-00000e40: 7465 7270 6f6c 6174 6564 2072 6561 6c2d  terpolated real-
-00000e50: 7661 6c75 6564 206f 7574 7075 7420 6672  valued output fr
-00000e60: 6f6d 2076 302e 332e 0a2d 205f 5f49 6d70  om v0.3..- __Imp
-00000e70: 6f72 7461 6e74 204e 6f74 653a 5f5f 205f  ortant Note:__ _
-00000e80: 6361 7463 6832 325f 2066 6561 7475 7265  catch22_ feature
-00000e90: 7320 6f6e 6c79 2065 7661 6c75 6174 6520  s only evaluate 
-00000ea0: 5f64 796e 616d 6963 616c 5f20 7072 6f70  _dynamical_ prop
-00000eb0: 6572 7469 6573 206f 6620 7469 6d65 2073  erties of time s
-00000ec0: 6572 6965 7320 616e 6420 646f 206e 6f74  eries and do not
-00000ed0: 2072 6573 706f 6e64 2074 6f20 6261 7369   respond to basi
-00000ee0: 6320 6469 6666 6572 656e 6365 7320 696e  c differences in
-00000ef0: 2074 6865 206c 6f63 6174 696f 6e20 2865   the location (e
-00000f00: 2e67 2e2c 206d 6561 6e29 206f 7220 7370  .g., mean) or sp
-00000f10: 7265 6164 2028 652e 672e 2c20 7661 7269  read (e.g., vari
-00000f20: 616e 6365 292e 0a20 202d 2046 726f 6d20  ance)..  - From 
-00000f30: 5f63 6174 6368 3232 5f20 7630 2e33 2c20  _catch22_ v0.3, 
-00000f40: 4966 2074 6865 206c 6f63 6174 696f 6e20  If the location 
-00000f50: 616e 6420 7370 7265 6164 206f 6620 7468  and spread of th
-00000f60: 6520 7261 7720 7469 6d65 2d73 6572 6965  e raw time-serie
-00000f70: 7320 6469 7374 7269 6275 7469 6f6e 206d  s distribution m
-00000f80: 6179 2062 6520 696d 706f 7274 616e 7420  ay be important 
-00000f90: 666f 7220 796f 7572 2061 7070 6c69 6361  for your applica
-00000fa0: 7469 6f6e 2c20 7765 2073 7567 6765 7374  tion, we suggest
-00000fb0: 2061 7070 6c79 696e 6720 7468 6520 6675   applying the fu
-00000fc0: 6e63 7469 6f6e 2061 7267 756d 656e 7420  nction argument 
-00000fd0: 6063 6174 6368 3234 203d 2054 7275 6560  `catch24 = True`
-00000fe0: 2074 6f20 796f 7572 2063 616c 6c20 746f   to your call to
-00000ff0: 2074 6865 205f 6361 7463 6832 325f 2066   the _catch22_ f
-00001000: 756e 6374 696f 6e20 696e 2074 6865 206c  unction in the l
-00001010: 616e 6775 6167 6520 6f66 2079 6f75 7220  anguage of your 
-00001020: 6368 6f69 6365 2e0a 2020 5468 6973 2077  choice..  This w
-00001030: 696c 6c20 7265 7375 6c74 2069 6e20 3234  ill result in 24
-00001040: 2066 6561 7475 7265 7320 6265 696e 6720   features being 
-00001050: 6361 6c63 756c 6174 6564 3a20 7468 6520  calculated: the 
-00001060: 5f63 6174 6368 3232 5f20 6665 6174 7572  _catch22_ featur
-00001070: 6573 2069 6e20 6164 6469 7469 6f6e 2074  es in addition t
-00001080: 6f20 6d65 616e 2061 6e64 2073 7461 6e64  o mean and stand
-00001090: 6172 6420 6465 7669 6174 696f 6e2e 0a0a  ard deviation...
-000010a0: 2323 2320 4d61 6e75 616c 2069 6e73 7461  ### Manual insta
-000010b0: 6c6c 0a0a 4966 2079 6f75 2066 696e 6420  ll..If you find 
-000010c0: 6973 7375 6573 2077 6974 6820 7468 6520  issues with the 
-000010d0: 6070 6970 6020 696e 7374 616c 6c2c 2079  `pip` install, y
-000010e0: 6f75 2063 616e 2061 6c73 6f20 696e 7374  ou can also inst
-000010f0: 616c 6c20 7573 696e 6720 6073 6574 7570  all using `setup
-00001100: 746f 6f6c 7360 3a0a 0a60 6060 0a70 7974  tools`:..```.pyt
-00001110: 686f 6e33 2073 6574 7570 2e70 7920 6275  hon3 setup.py bu
-00001120: 696c 640a 7079 7468 6f6e 3320 7365 7475  ild.python3 setu
-00001130: 702e 7079 2069 6e73 7461 6c6c 0a60 6060  p.py install.```
-00001140: 0a                                       .
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 3c69 6d67 2073 7263 3d22 696d 672f  "><img src="img/
+00000020: 6361 7463 6832 325f 6c6f 676f 5f73 7175  catch22_logo_squ
+00000030: 6172 652e 706e 6722 2061 6c74 3d22 6361  are.png" alt="ca
+00000040: 7463 6832 3220 6c6f 676f 2220 6865 6967  tch22 logo" heig
+00000050: 6874 3d22 3232 3022 2f3e 3c2f 703e 0a0a  ht="220"/></p>..
+00000060: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00000070: 7222 3e3c 656d 3e70 7963 6174 6368 3232  r"><em>pycatch22
+00000080: 3c2f 656d 3e3a 2043 416e 6f6e 6963 616c  </em>: CAnonical
+00000090: 2054 696d 652d 7365 7269 6573 2043 4861   Time-series CHa
+000000a0: 7261 6374 6572 6973 7469 6373 2069 6e20  racteristics in 
+000000b0: 7079 7468 6f6e 3c2f 6831 3e0a 0a3c 7020  python</h1>..<p 
+000000c0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+000000d0: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+000000e0: 7073 3a2f 2f77 7777 2e67 6e75 2e6f 7267  ps://www.gnu.org
+000000f0: 2f6c 6963 656e 7365 732f 6770 6c2d 332e  /licenses/gpl-3.
+00000100: 3022 3e3c 696d 6720 7372 633d 2268 7474  0"><img src="htt
+00000110: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000120: 2e69 6f2f 6261 6467 652f 4c69 6365 6e73  .io/badge/Licens
+00000130: 652d 4750 4c76 332d 626c 7565 2e73 7667  e-GPLv3-blue.svg
+00000140: 2220 6865 6967 6874 3d22 3230 222f 3e3c  " height="20"/><
+00000150: 2f61 3e0a 2009 2020 3c61 2068 7265 663d  /a>. .  <a href=
+00000160: 2268 7474 7073 3a2f 2f74 7769 7474 6572  "https://twitter
+00000170: 2e63 6f6d 2f63 6f6d 7054 696d 6553 6572  .com/compTimeSer
+00000180: 6965 7322 3e3c 696d 6720 7372 633d 2268  ies"><img src="h
+00000190: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000001a0: 6473 2e69 6f2f 7477 6974 7465 722f 7572  ds.io/twitter/ur
+000001b0: 6c2f 6874 7470 732f 7477 6974 7465 722e  l/https/twitter.
+000001c0: 636f 6d2f 636f 6d70 5469 6d65 5365 7269  com/compTimeSeri
+000001d0: 6573 2e73 7667 3f73 7479 6c65 3d73 6f63  es.svg?style=soc
+000001e0: 6961 6c26 6c61 6265 6c3d 466f 6c6c 6f77  ial&label=Follow
+000001f0: 2532 3025 3430 636f 6d70 5469 6d65 5365  %20%40compTimeSe
+00000200: 7269 6573 2220 6865 6967 6874 3d22 3230  ries" height="20
+00000210: 222f 3e3c 2f61 3e0a 3c2f 703e 0a0a 0a23  "/></a>.</p>...#
+00000220: 2320 4162 6f75 740a 0a5b 5f63 6174 6368  # About..[_catch
+00000230: 3232 5f5d 2868 7474 7073 3a2f 2f67 6974  22_](https://git
+00000240: 6875 622e 636f 6d2f 4479 6e61 6d69 6373  hub.com/Dynamics
+00000250: 416e 644e 6575 7261 6c53 7973 7465 6d73  AndNeuralSystems
+00000260: 2f63 6174 6368 3232 2920 6973 2061 2063  /catch22) is a c
+00000270: 6f6c 6c65 6374 696f 6e20 6f66 2032 3220  ollection of 22 
+00000280: 7469 6d65 2d73 6572 6965 7320 6665 6174  time-series feat
+00000290: 7572 6573 2063 6f64 6564 2069 6e20 4320  ures coded in C 
+000002a0: 7468 6174 2063 616e 2062 6520 7275 6e20  that can be run 
+000002b0: 6672 6f6d 2050 7974 686f 6e2c 2061 7320  from Python, as 
+000002c0: 7765 6c6c 2061 7320 5b52 5d28 6874 7470  well as [R](http
+000002d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
+000002e0: 656e 6465 7273 6f6e 7472 656e 742f 5263  endersontrent/Rc
+000002f0: 6174 6368 3232 292c 205b 4d61 746c 6162  atch22), [Matlab
+00000300: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000310: 2e63 6f6d 2f44 796e 616d 6963 7341 6e64  .com/DynamicsAnd
+00000320: 4e65 7572 616c 5379 7374 656d 732f 6361  NeuralSystems/ca
+00000330: 7463 6832 3229 2c20 616e 6420 5b4a 756c  tch22), and [Jul
+00000340: 6961 5d28 6874 7470 733a 2f2f 6769 7468  ia](https://gith
+00000350: 7562 2e63 6f6d 2f62 7265 6e64 616e 6a6f  ub.com/brendanjo
+00000360: 686e 6861 7272 6973 2f43 6174 6368 3232  hnharris/Catch22
+00000370: 2e6a 6c29 2e0a 0a54 6869 7320 7061 636b  .jl)...This pack
+00000380: 6167 6520 7072 6f76 6964 6573 2061 2070  age provides a p
+00000390: 7974 686f 6e20 696d 706c 656d 656e 7461  ython implementa
+000003a0: 7469 6f6e 2061 7320 7468 6520 6d6f 6475  tion as the modu
+000003b0: 6c65 205f 7079 6361 7463 6832 325f 2c20  le _pycatch22_, 
+000003c0: 6c69 6365 6e73 6564 2075 6e64 6572 2074  licensed under t
+000003d0: 6865 205b 474e 5520 4750 4c20 7633 206c  he [GNU GPL v3 l
+000003e0: 6963 656e 7365 5d28 6874 7470 3a2f 2f77  icense](http://w
+000003f0: 7777 2e67 6e75 2e6f 7267 2f6c 6963 656e  ww.gnu.org/licen
+00000400: 7365 732f 6770 6c2d 332e 302e 6874 6d6c  ses/gpl-3.0.html
+00000410: 2920 286f 7220 6c61 7465 7229 2e0a 0a23  ) (or later)...#
+00000420: 2323 2057 6861 7420 646f 2074 6865 2066  ## What do the f
+00000430: 6561 7475 7265 7320 646f 3f0a 0a54 6869  eatures do?..Thi
+00000440: 7320 5b47 6974 426f 6f6b 7320 7765 6273  s [GitBooks webs
+00000450: 6974 655d 2868 7474 7073 3a2f 2f74 696d  ite](https://tim
+00000460: 652d 7365 7269 6573 2d66 6561 7475 7265  e-series-feature
+00000470: 732e 6769 7462 6f6f 6b2e 696f 2f63 6174  s.gitbook.io/cat
+00000480: 6368 3232 2f66 6561 7475 7265 2d64 6573  ch22/feature-des
+00000490: 6372 6970 7469 6f6e 7329 2069 7320 6465  criptions) is de
+000004a0: 6469 6361 7465 6420 746f 2064 6573 6372  dicated to descr
+000004b0: 6962 696e 6720 7468 6520 6665 6174 7572  ibing the featur
+000004c0: 6573 2e0a 466f 7220 7468 6569 7220 696d  es..For their im
+000004d0: 706c 656d 656e 7461 7469 6f6e 2069 6e20  plementation in 
+000004e0: 636f 6465 2c20 7365 6520 7468 6520 5b6d  code, see the [m
+000004f0: 6169 6e20 5f63 6174 6368 3232 5f20 7265  ain _catch22_ re
+00000500: 706f 7369 746f 7279 5d28 6874 7470 733a  pository](https:
+00000510: 2f2f 6769 7468 7562 2e63 6f6d 2f44 796e  //github.com/Dyn
+00000520: 616d 6963 7341 6e64 4e65 7572 616c 5379  amicsAndNeuralSy
+00000530: 7374 656d 732f 6361 7463 6832 3229 2e0a  stems/catch22)..
+00000540: 5468 6572 6520 6973 2061 6c73 6f20 696e  There is also in
+00000550: 666f 726d 6174 696f 6e20 696e 2074 6865  formation in the
+00000560: 2061 7373 6f63 6961 7465 6420 7061 7065   associated pape
+00000570: 7220 5b26 2378 3146 3444 373b 204c 7562  r [&#x1F4D7; Lub
+00000580: 6261 2065 7420 616c 2e20 2832 3031 3929  ba et al. (2019)
+00000590: 2e5d 2868 7474 7073 3a2f 2f64 6f69 2e6f  .](https://doi.o
+000005a0: 7267 2f31 302e 3130 3037 2f73 3130 3631  rg/10.1007/s1061
+000005b0: 382d 3031 392d 3030 3634 372d 7829 2e0a  8-019-00647-x)..
+000005c0: 0a23 2323 2041 636b 6e6f 776c 6564 6765  .### Acknowledge
+000005d0: 6d65 6e74 203a 2b31 3a0a 0a49 6620 796f  ment :+1:..If yo
+000005e0: 7520 7573 6520 7468 6973 2073 6f66 7477  u use this softw
+000005f0: 6172 652c 2070 6c65 6173 6520 7265 6164  are, please read
+00000600: 2061 6e64 2063 6974 6520 7468 6973 206f   and cite this o
+00000610: 7065 6e2d 6163 6365 7373 2061 7274 6963  pen-access artic
+00000620: 6c65 3a0a 0a2d 2026 2378 3146 3444 373b  le:..- &#x1F4D7;
+00000630: 204c 7562 6261 2065 7420 616c 2e20 5b5f   Lubba et al. [_
+00000640: 6361 7463 6832 325f 3a20 4341 6e6f 6e69  catch22_: CAnoni
+00000650: 6361 6c20 5469 6d65 2d73 6572 6965 7320  cal Time-series 
+00000660: 4348 6172 6163 7465 7269 7374 6963 735d  CHaracteristics]
+00000670: 2868 7474 7073 3a2f 2f64 6f69 2e6f 7267  (https://doi.org
+00000680: 2f31 302e 3130 3037 2f73 3130 3631 382d  /10.1007/s10618-
+00000690: 3031 392d 3030 3634 372d 7829 2c20 5f44  019-00647-x), _D
+000006a0: 6174 6120 4d69 6e20 4b6e 6f77 6c20 4469  ata Min Knowl Di
+000006b0: 7363 5f20 5f5f 3333 5f5f 2c20 3138 3231  sc_ __33__, 1821
+000006c0: 2028 3230 3139 292e 0a0a 2323 2049 6e73   (2019)...## Ins
+000006d0: 7461 6c6c 6174 696f 6e0a 0a55 7369 6e67  tallation..Using
+000006e0: 2060 7069 7060 2066 6f72 205b 6070 7963   `pip` for [`pyc
+000006f0: 6174 6368 3232 605d 2868 7474 7073 3a2f  atch22`](https:/
+00000700: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000710: 742f 7079 6361 7463 6832 322f 293a 0a0a  t/pycatch22/):..
+00000720: 6060 600a 7069 7020 696e 7374 616c 6c20  ```.pip install 
+00000730: 7079 6361 7463 6832 320a 6060 600a 0a49  pycatch22.```..I
+00000740: 6620 7468 6973 2064 6f65 736e 2774 2077  f this doesn't w
+00000750: 6f72 6b2c 206d 616b 6520 7375 7265 2079  ork, make sure y
+00000760: 6f75 2061 7265 2075 7369 6e67 2074 6865  ou are using the
+00000770: 206c 6174 6573 7420 6073 6574 7570 746f   latest `setupto
+00000780: 6f6c 7360 3a20 6070 6970 2069 6e73 7461  ols`: `pip insta
+00000790: 6c6c 2073 6574 7570 746f 6f6c 7320 2d2d  ll setuptools --
+000007a0: 7570 6772 6164 6560 2e0a 0a49 6620 796f  upgrade`...If yo
+000007b0: 7520 636f 6d65 2061 6372 6f73 7320 6572  u come across er
+000007c0: 726f 7273 2077 6974 6820 7665 7273 696f  rors with versio
+000007d0: 6e20 7265 736f 6c75 7469 6f6e 2c20 796f  n resolution, yo
+000007e0: 7520 7368 6f75 6c64 2074 7279 2073 6f6d  u should try som
+000007f0: 6574 6869 6e67 206c 696b 653a 2060 7069  ething like: `pi
+00000800: 7020 696e 7374 616c 6c20 7079 6361 7463  p install pycatc
+00000810: 6832 323d 3d30 2e34 2e32 202d 2d75 7365  h22==0.4.2 --use
+00000820: 2d64 6570 7265 6361 7465 643d 6c65 6761  -deprecated=lega
+00000830: 6379 2d72 6573 6f6c 7665 7260 2e0a 0a49  cy-resolver`...I
+00000840: 7420 6973 2061 6c73 6f20 6120 5b70 6163  t is also a [pac
+00000850: 6b61 6765 206f 6e20 616e 6163 6f6e 6461  kage on anaconda
+00000860: 5d28 6874 7470 733a 2f2f 616e 6163 6f6e  ](https://anacon
+00000870: 6461 2e6f 7267 2f63 6f6e 6461 2d66 6f72  da.org/conda-for
+00000880: 6765 2f70 7963 6174 6368 3232 2920 7468  ge/pycatch22) th
+00000890: 616e 6b73 2074 6f20 5b40 7270 616e 6169  anks to [@rpanai
+000008a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000008b0: 2e63 6f6d 2f72 7061 6e61 6929 2c20 7768  .com/rpanai), wh
+000008c0: 6963 6820 796f 7520 6361 6e20 696e 7374  ich you can inst
+000008d0: 616c 6c20 7669 6120 6063 6f6e 6461 603a  all via `conda`:
+000008e0: 0a0a 6060 600a 636f 6e64 6120 696e 7374  ..```.conda inst
+000008f0: 616c 6c20 2d63 2063 6f6e 6461 2d66 6f72  all -c conda-for
+00000900: 6765 2070 7963 6174 6368 3232 0a60 6060  ge pycatch22.```
+00000910: 0a0a 6f72 2060 6d61 6d62 6160 3a0a 0a60  ..or `mamba`:..`
+00000920: 6060 0a6d 616d 6261 2069 6e73 7461 6c6c  ``.mamba install
+00000930: 202d 6320 636f 6e64 612d 666f 7267 6520   -c conda-forge 
+00000940: 7079 6361 7463 6832 320a 6060 600a 0a5b  pycatch22.```..[
+00000950: 4120 6d61 6e75 616c 2069 6e73 7461 6c6c  A manual install
+00000960: 2028 626f 7474 6f6d 206f 6620 7468 6973   (bottom of this
+00000970: 2070 6167 6529 2069 7320 6120 6c61 7374   page) is a last
+00000980: 2072 6573 6f72 742e 5d0a 0a23 2320 5573   resort.]..## Us
+00000990: 6167 650a 0a45 6163 6820 6665 6174 7572  age..Each featur
+000009a0: 6520 6675 6e63 7469 6f6e 2063 616e 2062  e function can b
+000009b0: 6520 6163 6365 7373 6564 2069 6e64 6976  e accessed indiv
+000009c0: 6964 7561 6c6c 7920 616e 6420 7461 6b65  idually and take
+000009d0: 7320 6172 7261 7973 2061 7320 7475 706c  s arrays as tupl
+000009e0: 6520 6f72 206c 6973 7473 2028 6e6f 7420  e or lists (not 
+000009f0: 606e 756d 7079 6020 6172 7261 7973 292e  `numpy` arrays).
+00000a00: 0a46 6f72 2065 7861 6d70 6c65 2c20 666f  .For example, fo
+00000a10: 7220 6c6f 6164 6564 2064 6174 6120 6074  r loaded data `t
+00000a20: 7344 6174 6160 2069 6e20 5079 7468 6f6e  sData` in Python
+00000a30: 3a0a 0a60 6060 7079 7468 6f6e 330a 696d  :..```python3.im
+00000a40: 706f 7274 2070 7963 6174 6368 3232 0a74  port pycatch22.t
+00000a50: 7344 6174 6120 3d20 5b31 2c32 2c34 2c33  sData = [1,2,4,3
+00000a60: 5d20 2320 286f 7220 6d6f 7265 2069 6e74  ] # (or more int
+00000a70: 6572 6573 7469 6e67 2064 6174 6121 290a  eresting data!).
+00000a80: 7079 6361 7463 6832 322e 434f 5f66 3165  pycatch22.CO_f1e
+00000a90: 6361 6328 7473 4461 7461 290a 6060 600a  cac(tsData).```.
+00000aa0: 0a41 6c6c 2066 6561 7475 7265 7320 6172  .All features ar
+00000ab0: 6520 6275 6e64 6c65 6420 696e 2074 6865  e bundled in the
+00000ac0: 206d 6574 686f 6420 6063 6174 6368 3232   method `catch22
+00000ad0: 5f61 6c6c 602c 2077 6869 6368 2061 6c73  _all`, which als
+00000ae0: 6f20 6163 6365 7074 7320 606e 756d 7079  o accepts `numpy
+00000af0: 6020 6172 7261 7973 2061 6e64 2067 6976  ` arrays and giv
+00000b00: 6573 2062 6163 6b20 6120 6469 6374 696f  es back a dictio
+00000b10: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+00000b20: 7468 6520 656e 7472 6965 7320 6063 6174  the entries `cat
+00000b30: 6368 3232 5f61 6c6c 5b27 6e61 6d65 7327  ch22_all['names'
+00000b40: 5d60 2066 6f72 2066 6561 7475 7265 206e  ]` for feature n
+00000b50: 616d 6573 2061 6e64 2060 6361 7463 6832  ames and `catch2
+00000b60: 325f 616c 6c5b 2776 616c 7565 7327 5d60  2_all['values']`
+00000b70: 2066 6f72 2066 6561 7475 7265 206f 7574   for feature out
+00000b80: 7075 7473 2e0a 0a55 7361 6765 2028 636f  puts...Usage (co
+00000b90: 6d70 7574 696e 6720 3232 2066 6561 7475  mputing 22 featu
+00000ba0: 7265 733a 205f 6361 7463 6832 325f 293a  res: _catch22_):
+00000bb0: 0a0a 6060 6070 7974 686f 6e33 0a70 7963  ..```python3.pyc
+00000bc0: 6174 6368 3232 2e63 6174 6368 3232 5f61  atch22.catch22_a
+00000bd0: 6c6c 2874 7344 6174 6129 0a60 6060 0a0a  ll(tsData).```..
+00000be0: 5573 6167 6520 2863 6f6d 7075 7469 6e67  Usage (computing
+00000bf0: 2032 3420 6665 6174 7572 6573 3a20 5f63   24 features: _c
+00000c00: 6174 6368 3234 5f20 3d20 5f63 6174 6368  atch24_ = _catch
+00000c10: 3232 5f20 2b20 6d65 616e 202b 2073 7461  22_ + mean + sta
+00000c20: 6e64 6172 6420 6465 7669 6174 696f 6e29  ndard deviation)
+00000c30: 3a0a 0a60 6060 7079 7468 6f6e 330a 7079  :..```python3.py
+00000c40: 6361 7463 6832 322e 6361 7463 6832 325f  catch22.catch22_
+00000c50: 616c 6c28 7473 4461 7461 2c63 6174 6368  all(tsData,catch
+00000c60: 3234 3d54 7275 6529 0a60 6060 0a0a 5765  24=True).```..We
+00000c70: 2061 6c73 6f20 696e 636c 7564 6520 6120   also include a 
+00000c80: 2773 686f 7274 206e 616d 6527 2066 6f72  'short name' for
+00000c90: 2065 6163 6820 6665 6174 7572 6520 666f   each feature fo
+00000ca0: 7220 6561 7369 6572 2072 6566 6572 656e  r easier referen
+00000cb0: 6365 2028 6173 206f 7574 6c69 6e65 6420  ce (as outlined 
+00000cc0: 696e 2074 6865 2047 6974 426f 6f6b 205b  in the GitBook [
+00000cd0: 4665 6174 7572 6520 6f76 6572 7669 6577  Feature overview
+00000ce0: 2074 6162 6c65 5d28 6874 7470 733a 2f2f   table](https://
+00000cf0: 7469 6d65 2d73 6572 6965 732d 6665 6174  time-series-feat
+00000d00: 7572 6573 2e67 6974 626f 6f6b 2e69 6f2f  ures.gitbook.io/
+00000d10: 6361 7463 6832 322f 6665 6174 7572 652d  catch22/feature-
+00000d20: 6465 7363 7269 7074 696f 6e73 2f66 6561  descriptions/fea
+00000d30: 7475 7265 2d6f 7665 7276 6965 772d 7461  ture-overview-ta
+00000d40: 626c 6529 292e 0a54 6865 7365 2073 686f  ble))..These sho
+00000d50: 7274 206e 616d 6573 2063 616e 2062 6520  rt names can be 
+00000d60: 696e 636c 7564 6564 2069 6e20 7468 6520  included in the 
+00000d70: 6f75 7470 7574 2066 726f 6d20 6063 6174  output from `cat
+00000d80: 6368 3232 5f61 6c6c 2829 6020 6279 2073  ch22_all()` by s
+00000d90: 6574 7469 6e67 2060 7368 6f72 745f 6e61  etting `short_na
+00000da0: 6d65 733d 5472 7565 6020 6173 2066 6f6c  mes=True` as fol
+00000db0: 6c6f 7773 3a0a 0a60 6060 7079 7468 6f6e  lows:..```python
+00000dc0: 330a 7079 6361 7463 6832 322e 6361 7463  3.pycatch22.catc
+00000dd0: 6832 325f 616c 6c28 7473 4461 7461 2c63  h22_all(tsData,c
+00000de0: 6174 6368 3234 3d54 7275 652c 7368 6f72  atch24=True,shor
+00000df0: 745f 6e61 6d65 733d 5472 7565 290a 6060  t_names=True).``
+00000e00: 600a 0a23 2323 2054 656d 706c 6174 6520  `..### Template 
+00000e10: 616e 616c 7973 6973 2073 6372 6970 740a  analysis script.
+00000e20: 0a54 6861 6e6b 7320 746f 205b 406a 6d6f  .Thanks to [@jmo
+00000e30: 6f32 3838 305d 2868 7474 7073 3a2f 2f67  o2880](https://g
+00000e40: 6974 6875 622e 636f 6d2f 6a6d 6f6f 3238  ithub.com/jmoo28
+00000e50: 3830 2920 666f 7220 7075 7474 696e 6720  80) for putting 
+00000e60: 746f 6765 7468 6572 2061 205b 6465 6d6f  together a [demo
+00000e70: 6e73 7472 6174 696f 6e20 6e6f 7465 626f  nstration notebo
+00000e80: 6f6b 5d28 6874 7470 733a 2f2f 6769 7468  ok](https://gith
+00000e90: 7562 2e63 6f6d 2f6a 6d6f 6f32 3838 302f  ub.com/jmoo2880/
+00000ea0: 6332 322d 7573 6167 652d 6578 616d 706c  c22-usage-exampl
+00000eb0: 6573 2f29 2066 6f72 2075 7369 6e67 2070  es/) for using p
+00000ec0: 7963 6174 6368 3232 2074 6f20 6578 7472  ycatch22 to extr
+00000ed0: 6163 7420 6665 6174 7572 6573 2066 726f  act features fro
+00000ee0: 6d20 6120 7469 6d65 2d73 6572 6965 7320  m a time-series 
+00000ef0: 6461 7461 7365 742e 0a0a 2323 2320 5573  dataset...### Us
+00000f00: 6167 6520 6e6f 7465 730a 0a2d 2057 6865  age notes..- Whe
+00000f10: 6e20 7072 6573 656e 7469 6e67 2072 6573  n presenting res
+00000f20: 756c 7473 2075 7369 6e67 205f 6361 7463  ults using _catc
+00000f30: 6832 325f 2c20 796f 7520 6d75 7374 2069  h22_, you must i
+00000f40: 6465 6e74 6966 7920 7468 6520 7665 7273  dentify the vers
+00000f50: 696f 6e20 7573 6564 2074 6f20 616c 6c6f  ion used to allo
+00000f60: 7720 636c 6561 7220 7265 7072 6f64 7563  w clear reproduc
+00000f70: 7469 6f6e 206f 6620 796f 7572 2072 6573  tion of your res
+00000f80: 756c 7473 2e20 466f 7220 6578 616d 706c  ults. For exampl
+00000f90: 652c 2060 434f 5f66 3165 6361 6360 2077  e, `CO_f1ecac` w
+00000fa0: 6173 2061 6c74 6572 6564 2066 726f 6d20  as altered from 
+00000fb0: 616e 2069 6e74 6567 6572 2d76 616c 7565  an integer-value
+00000fc0: 6420 6f75 7470 7574 2074 6f20 6120 6c69  d output to a li
+00000fd0: 6e65 6172 6c79 2069 6e74 6572 706f 6c61  nearly interpola
+00000fe0: 7465 6420 7265 616c 2d76 616c 7565 6420  ted real-valued 
+00000ff0: 6f75 7470 7574 2066 726f 6d20 7630 2e33  output from v0.3
+00001000: 2e0a 2d20 5f5f 496d 706f 7274 616e 7420  ..- __Important 
+00001010: 4e6f 7465 3a5f 5f20 5f63 6174 6368 3232  Note:__ _catch22
+00001020: 5f20 6665 6174 7572 6573 206f 6e6c 7920  _ features only 
+00001030: 6576 616c 7561 7465 205f 6479 6e61 6d69  evaluate _dynami
+00001040: 6361 6c5f 2070 726f 7065 7274 6965 7320  cal_ properties 
+00001050: 6f66 2074 696d 6520 7365 7269 6573 2061  of time series a
+00001060: 6e64 2064 6f20 6e6f 7420 7265 7370 6f6e  nd do not respon
+00001070: 6420 746f 2062 6173 6963 2064 6966 6665  d to basic diffe
+00001080: 7265 6e63 6573 2069 6e20 7468 6520 6c6f  rences in the lo
+00001090: 6361 7469 6f6e 2028 652e 672e 2c20 6d65  cation (e.g., me
+000010a0: 616e 2920 6f72 2073 7072 6561 6420 2865  an) or spread (e
+000010b0: 2e67 2e2c 2076 6172 6961 6e63 6529 2e0a  .g., variance)..
+000010c0: 2020 2d20 4672 6f6d 205f 6361 7463 6832    - From _catch2
+000010d0: 325f 2076 302e 332c 2049 6620 7468 6520  2_ v0.3, If the 
+000010e0: 6c6f 6361 7469 6f6e 2061 6e64 2073 7072  location and spr
+000010f0: 6561 6420 6f66 2074 6865 2072 6177 2074  ead of the raw t
+00001100: 696d 652d 7365 7269 6573 2064 6973 7472  ime-series distr
+00001110: 6962 7574 696f 6e20 6d61 7920 6265 2069  ibution may be i
+00001120: 6d70 6f72 7461 6e74 2066 6f72 2079 6f75  mportant for you
+00001130: 7220 6170 706c 6963 6174 696f 6e2c 2077  r application, w
+00001140: 6520 7375 6767 6573 7420 6170 706c 7969  e suggest applyi
+00001150: 6e67 2074 6865 2066 756e 6374 696f 6e20  ng the function 
+00001160: 6172 6775 6d65 6e74 2060 6361 7463 6832  argument `catch2
+00001170: 3420 3d20 5472 7565 6020 746f 2079 6f75  4 = True` to you
+00001180: 7220 6361 6c6c 2074 6f20 7468 6520 5f63  r call to the _c
+00001190: 6174 6368 3232 5f20 6675 6e63 7469 6f6e  atch22_ function
+000011a0: 2069 6e20 7468 6520 6c61 6e67 7561 6765   in the language
+000011b0: 206f 6620 796f 7572 2063 686f 6963 652e   of your choice.
+000011c0: 0a20 2054 6869 7320 7769 6c6c 2072 6573  .  This will res
+000011d0: 756c 7420 696e 2032 3420 6665 6174 7572  ult in 24 featur
+000011e0: 6573 2062 6569 6e67 2063 616c 6375 6c61  es being calcula
+000011f0: 7465 643a 2074 6865 205f 6361 7463 6832  ted: the _catch2
+00001200: 325f 2066 6561 7475 7265 7320 696e 2061  2_ features in a
+00001210: 6464 6974 696f 6e20 746f 206d 6561 6e20  ddition to mean 
+00001220: 616e 6420 7374 616e 6461 7264 2064 6576  and standard dev
+00001230: 6961 7469 6f6e 2e0a 0a23 2323 204d 616e  iation...### Man
+00001240: 7561 6c20 696e 7374 616c 6c0a 0a49 6620  ual install..If 
+00001250: 796f 7520 6669 6e64 2069 7373 7565 7320  you find issues 
+00001260: 7769 7468 2074 6865 2060 7069 7060 2069  with the `pip` i
+00001270: 6e73 7461 6c6c 2c20 796f 7520 6361 6e20  nstall, you can 
+00001280: 616c 736f 2069 6e73 7461 6c6c 2075 7369  also install usi
+00001290: 6e67 2060 7365 7475 7074 6f6f 6c73 603a  ng `setuptools`:
+000012a0: 0a0a 6060 600a 7079 7468 6f6e 3320 7365  ..```.python3 se
+000012b0: 7475 702e 7079 2062 7569 6c64 0a70 7974  tup.py build.pyt
+000012c0: 686f 6e33 2073 6574 7570 2e70 7920 696e  hon3 setup.py in
+000012d0: 7374 616c 6c0a 6060 600a                 stall.```.
```

### Comparing `pycatch22-0.4.4/pyproject.toml` & `pycatch22-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pycatch22"
-version = "0.4.4"
+version = "0.4.5"
 authors = [
     {name = "Carl H Lubba"},
     {email = "carl.lubba@gmx.de"},
 ]
 maintainers = [
     {name = "Ben D Fulcher"},
     {email = "ben.fulcher@sydney.edu.au"},
```

### Comparing `pycatch22-0.4.4/setup.py` & `pycatch22-0.4.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,22 +4,27 @@
 
 sourceDir = os.path.join("src", "C");
 
 sourceFileList = [os.path.join(sourceDir, file) for file in os.listdir(sourceDir) if file.endswith(
     ".c") and not 'main' in file]
     # and not (file == "sampen.c" or file == "run_features.c")]
 
-extra_compile_args = sysconfig.get_config_var('CFLAGS').split()
+cflags = sysconfig.get_config_var('CFLAGS')
+if cflags is not None:
+    extra_compile_args = cflags.split()
+else: # Windows system
+    extra_compile_args = []
+
 extra_compile_args += ["-std=c99"]
 
 # The c++ extension module:
 extension_mod = Extension(name = "catch22_C",
     sources = sourceFileList,
     include_dirs = [sourceDir],
     extra_compile_args = extra_compile_args)  # Header files are here
 
 setup(
     packages = find_packages(where = "src",
                             include = ["pycatch22"]),
     package_dir = {"": "src"},
-    ext_modules = [extension_mod]
+    ext_modules = [extension_mod],
 )
```

### Comparing `pycatch22-0.4.4/src/C/CO_AutoCorr.c` & `pycatch22-0.4.5/src/C/CO_AutoCorr.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/CO_AutoCorr.h` & `pycatch22-0.4.5/src/C/CO_AutoCorr.h`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/DN_HistogramMode_10.c` & `pycatch22-0.4.5/src/C/DN_HistogramMode_10.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/DN_HistogramMode_5.c` & `pycatch22-0.4.5/src/C/DN_HistogramMode_5.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/DN_OutlierInclude.c` & `pycatch22-0.4.5/src/C/DN_OutlierInclude.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/FC_LocalSimple.c` & `pycatch22-0.4.5/src/C/FC_LocalSimple.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/FC_LocalSimple.h` & `pycatch22-0.4.5/src/C/FC_LocalSimple.h`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/IN_AutoMutualInfoStats.c` & `pycatch22-0.4.5/src/C/IN_AutoMutualInfoStats.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/MD_hrv.c` & `pycatch22-0.4.5/src/C/MD_hrv.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/PD_PeriodicityWang.c` & `pycatch22-0.4.5/src/C/PD_PeriodicityWang.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/SB_BinaryStats.c` & `pycatch22-0.4.5/src/C/SB_BinaryStats.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/SB_CoarseGrain.c` & `pycatch22-0.4.5/src/C/SB_CoarseGrain.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/SB_MotifThree.c` & `pycatch22-0.4.5/src/C/SB_MotifThree.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/SB_TransitionMatrix.c` & `pycatch22-0.4.5/src/C/SB_TransitionMatrix.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/SC_FluctAnal.c` & `pycatch22-0.4.5/src/C/SC_FluctAnal.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/SP_Summaries.c` & `pycatch22-0.4.5/src/C/SP_Summaries.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/butterworth.c` & `pycatch22-0.4.5/src/C/butterworth.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/catch22_wrap.c` & `pycatch22-0.4.5/src/C/catch22_wrap.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/fft.c` & `pycatch22-0.4.5/src/C/fft.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/fft.h` & `pycatch22-0.4.5/src/C/fft.h`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/helper_functions.c` & `pycatch22-0.4.5/src/C/helper_functions.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/helper_functions.h` & `pycatch22-0.4.5/src/C/helper_functions.h`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/histcounts.c` & `pycatch22-0.4.5/src/C/histcounts.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/histcounts.h` & `pycatch22-0.4.5/src/C/histcounts.h`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/main.c` & `pycatch22-0.4.5/src/C/main.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/runAllTS.sh` & `pycatch22-0.4.5/src/C/runAllTS.sh`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/splinefit.c` & `pycatch22-0.4.5/src/C/splinefit.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/stats.c` & `pycatch22-0.4.5/src/C/stats.c`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/C/stats.h` & `pycatch22-0.4.5/src/C/stats.h`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/pycatch22/catch22.py` & `pycatch22-0.4.5/src/pycatch22/catch22.py`

 * *Files identical despite different names*

### Comparing `pycatch22-0.4.4/src/pycatch22.egg-info/PKG-INFO` & `pycatch22-0.4.5/src/pycatch22.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6361  : 2.1.Name: pyca
 00000020: 7463 6832 320a 5665 7273 696f 6e3a 2030  tch22.Version: 0
-00000030: 2e34 2e34 0a53 756d 6d61 7279 3a20 3232  .4.4.Summary: 22
+00000030: 2e34 2e35 0a53 756d 6d61 7279 3a20 3232  .4.5.Summary: 22
 00000040: 2043 416e 6f6e 6963 616c 2054 696d 652d   CAnonical Time-
 00000050: 7365 7269 6573 2046 6561 7475 7265 730a  series Features.
 00000060: 4175 7468 6f72 3a20 4361 726c 2048 204c  Author: Carl H L
 00000070: 7562 6261 0a41 7574 686f 722d 656d 6169  ubba.Author-emai
 00000080: 6c3a 2063 6172 6c2e 6c75 6262 6140 676d  l: carl.lubba@gm
 00000090: 782e 6465 0a4d 6169 6e74 6169 6e65 723a  x.de.Maintainer:
 000000a0: 2042 656e 2044 2046 756c 6368 6572 0a4d   Ben D Fulcher.M
@@ -37,284 +37,310 @@
 00000240: 7220 6c61 7465 7220 2847 504c 7633 2b29  r later (GPLv3+)
 00000250: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
 00000260: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
 00000270: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
 00000280: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
 00000290: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
 000002a0: 6172 6b64 6f77 6e0a 4c69 6365 6e73 652d  arkdown.License-
-000002b0: 4669 6c65 3a20 4c49 4345 4e53 450a 0a23  File: LICENSE..#
-000002c0: 205f 7079 6361 7463 6832 325f 202d 2043   _pycatch22_ - C
-000002d0: 416e 6f6e 6963 616c 2054 696d 652d 7365  Anonical Time-se
-000002e0: 7269 6573 2043 4861 7261 6374 6572 6973  ries CHaracteris
-000002f0: 7469 6373 2069 6e20 7079 7468 6f6e 0a0a  tics in python..
-00000300: 3c69 6d67 2073 7263 3d22 696d 672f 6361  <img src="img/ca
-00000310: 7463 6832 325f 6c6f 676f 5f73 7175 6172  tch22_logo_squar
-00000320: 652e 706e 6722 2077 6964 7468 3d22 3235  e.png" width="25
-00000330: 3022 2068 6569 6768 743d 2232 3530 222f  0" height="250"/
-00000340: 3e0a 0a23 2320 4162 6f75 740a 0a5b 5f63  >..## About..[_c
-00000350: 6174 6368 3232 5f5d 2868 7474 7073 3a2f  atch22_](https:/
-00000360: 2f67 6974 6875 622e 636f 6d2f 4479 6e61  /github.com/Dyna
-00000370: 6d69 6373 416e 644e 6575 7261 6c53 7973  micsAndNeuralSys
-00000380: 7465 6d73 2f63 6174 6368 3232 2920 6973  tems/catch22) is
-00000390: 2061 2063 6f6c 6c65 6374 696f 6e20 6f66   a collection of
-000003a0: 2032 3220 7469 6d65 2d73 6572 6965 7320   22 time-series 
-000003b0: 6665 6174 7572 6573 2063 6f64 6564 2069  features coded i
-000003c0: 6e20 4320 7468 6174 2063 616e 2062 6520  n C that can be 
-000003d0: 7275 6e20 6672 6f6d 2050 7974 686f 6e2c  run from Python,
-000003e0: 2061 7320 7765 6c6c 2061 7320 5b52 5d28   as well as [R](
-000003f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000400: 6f6d 2f68 656e 6465 7273 6f6e 7472 656e  om/hendersontren
-00000410: 742f 5263 6174 6368 3232 292c 205b 4d61  t/Rcatch22), [Ma
-00000420: 746c 6162 5d28 6874 7470 733a 2f2f 6769  tlab](https://gi
-00000430: 7468 7562 2e63 6f6d 2f44 796e 616d 6963  thub.com/Dynamic
-00000440: 7341 6e64 4e65 7572 616c 5379 7374 656d  sAndNeuralSystem
-00000450: 732f 6361 7463 6832 3229 2c20 616e 6420  s/catch22), and 
-00000460: 5b4a 756c 6961 5d28 6874 7470 733a 2f2f  [Julia](https://
-00000470: 6769 7468 7562 2e63 6f6d 2f62 7265 6e64  github.com/brend
-00000480: 616e 6a6f 686e 6861 7272 6973 2f43 6174  anjohnharris/Cat
-00000490: 6368 3232 2e6a 6c29 2e0a 0a54 6869 7320  ch22.jl)...This 
-000004a0: 7061 636b 6167 6520 7072 6f76 6964 6573  package provides
-000004b0: 2061 2070 7974 686f 6e20 696d 706c 656d   a python implem
-000004c0: 656e 7461 7469 6f6e 2061 7320 7468 6520  entation as the 
-000004d0: 6d6f 6475 6c65 205f 7079 6361 7463 6832  module _pycatch2
-000004e0: 325f 2c20 6c69 6365 6e73 6564 2075 6e64  2_, licensed und
-000004f0: 6572 2074 6865 205b 474e 5520 4750 4c20  er the [GNU GPL 
-00000500: 7633 206c 6963 656e 7365 5d28 6874 7470  v3 license](http
-00000510: 3a2f 2f77 7777 2e67 6e75 2e6f 7267 2f6c  ://www.gnu.org/l
-00000520: 6963 656e 7365 732f 6770 6c2d 332e 302e  icenses/gpl-3.0.
-00000530: 6874 6d6c 2920 286f 7220 6c61 7465 7229  html) (or later)
-00000540: 2e0a 0a23 2323 2057 6861 7420 646f 2074  ...### What do t
-00000550: 6865 2066 6561 7475 7265 7320 646f 3f0a  he features do?.
-00000560: 0a54 6869 7320 5b47 6974 426f 6f6b 7320  .This [GitBooks 
-00000570: 7765 6273 6974 655d 2868 7474 7073 3a2f  website](https:/
-00000580: 2f66 6561 7475 7265 2d62 6173 6564 2d74  /feature-based-t
-00000590: 696d 652d 7365 7269 6573 2d61 6e61 6c79  ime-series-analy
-000005a0: 732e 6769 7462 6f6f 6b2e 696f 2f63 6174  s.gitbook.io/cat
-000005b0: 6368 3232 2d66 6561 7475 7265 732f 2920  ch22-features/) 
-000005c0: 6973 2064 6564 6963 6174 6564 2074 6f20  is dedicated to 
-000005d0: 6465 7363 7269 6269 6e67 2074 6865 2066  describing the f
-000005e0: 6561 7475 7265 732e 0a46 6f72 2074 6865  eatures..For the
-000005f0: 6972 2069 6d70 6c65 6d65 6e74 6174 696f  ir implementatio
-00000600: 6e20 696e 2063 6f64 652c 2073 6565 2074  n in code, see t
-00000610: 6865 205b 6d61 696e 205f 6361 7463 6832  he [main _catch2
-00000620: 325f 2072 6570 6f73 6974 6f72 795d 2868  2_ repository](h
-00000630: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000640: 6d2f 4479 6e61 6d69 6373 416e 644e 6575  m/DynamicsAndNeu
-00000650: 7261 6c53 7973 7465 6d73 2f63 6174 6368  ralSystems/catch
-00000660: 3232 292e 0a54 6865 7265 2069 7320 616c  22)..There is al
-00000670: 736f 2069 6e66 6f72 6d61 7469 6f6e 2069  so information i
-00000680: 6e20 7468 6520 6173 736f 6369 6174 6564  n the associated
-00000690: 2070 6170 6572 205b 2623 7831 4634 4437   paper [&#x1F4D7
-000006a0: 3b20 4c75 6262 6120 6574 2061 6c2e 2028  ; Lubba et al. (
-000006b0: 3230 3139 292e 5d28 6874 7470 733a 2f2f  2019).](https://
-000006c0: 646f 692e 6f72 672f 3130 2e31 3030 372f  doi.org/10.1007/
-000006d0: 7331 3036 3138 2d30 3139 2d30 3036 3437  s10618-019-00647
-000006e0: 2d78 292e 0a0a 2323 2320 4163 6b6e 6f77  -x)...### Acknow
-000006f0: 6c65 6467 656d 656e 7420 3a2b 313a 0a0a  ledgement :+1:..
-00000700: 4966 2079 6f75 2075 7365 2074 6869 7320  If you use this 
-00000710: 736f 6674 7761 7265 2c20 706c 6561 7365  software, please
-00000720: 2072 6561 6420 616e 6420 6369 7465 2074   read and cite t
-00000730: 6869 7320 6f70 656e 2d61 6363 6573 7320  his open-access 
-00000740: 6172 7469 636c 653a 0a0a 2d20 2623 7831  article:..- &#x1
-00000750: 4634 4437 3b20 4c75 6262 6120 6574 2061  F4D7; Lubba et a
-00000760: 6c2e 205b 5f63 6174 6368 3232 5f3a 2043  l. [_catch22_: C
-00000770: 416e 6f6e 6963 616c 2054 696d 652d 7365  Anonical Time-se
-00000780: 7269 6573 2043 4861 7261 6374 6572 6973  ries CHaracteris
-00000790: 7469 6373 5d28 6874 7470 733a 2f2f 646f  tics](https://do
-000007a0: 692e 6f72 672f 3130 2e31 3030 372f 7331  i.org/10.1007/s1
-000007b0: 3036 3138 2d30 3139 2d30 3036 3437 2d78  0618-019-00647-x
-000007c0: 292c 205f 4461 7461 204d 696e 204b 6e6f  ), _Data Min Kno
-000007d0: 776c 2044 6973 635f 205f 5f33 335f 5f2c  wl Disc_ __33__,
-000007e0: 2031 3832 3120 2832 3031 3929 2e0a 0a23   1821 (2019)...#
-000007f0: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
-00000800: 5573 696e 6720 6070 6970 6020 666f 7220  Using `pip` for 
-00000810: 5b60 7079 6361 7463 6832 3260 5d28 6874  [`pycatch22`](ht
-00000820: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000830: 726f 6a65 6374 2f70 7963 6174 6368 3232  roject/pycatch22
-00000840: 2f29 3a0a 0a60 6060 0a70 6970 2069 6e73  /):..```.pip ins
-00000850: 7461 6c6c 2070 7963 6174 6368 3232 0a60  tall pycatch22.`
-00000860: 6060 0a0a 4966 2074 6869 7320 646f 6573  ``..If this does
-00000870: 6e27 7420 776f 726b 2c20 6d61 6b65 2073  n't work, make s
-00000880: 7572 6520 796f 7520 6172 6520 7573 696e  ure you are usin
-00000890: 6720 7468 6520 6c61 7465 7374 2060 7365  g the latest `se
-000008a0: 7475 7074 6f6f 6c73 603a 2060 7069 7020  tuptools`: `pip 
-000008b0: 696e 7374 616c 6c20 7365 7475 7074 6f6f  install setuptoo
-000008c0: 6c73 202d 2d75 7067 7261 6465 602e 0a0a  ls --upgrade`...
-000008d0: 4966 2079 6f75 2063 6f6d 6520 6163 726f  If you come acro
-000008e0: 7373 2065 7272 6f72 7320 7769 7468 2076  ss errors with v
-000008f0: 6572 7369 6f6e 2072 6573 6f6c 7574 696f  ersion resolutio
-00000900: 6e2c 2079 6f75 2073 686f 756c 6420 7472  n, you should tr
-00000910: 7920 736f 6d65 7468 696e 6720 6c69 6b65  y something like
-00000920: 3a20 6070 6970 2069 6e73 7461 6c6c 2070  : `pip install p
-00000930: 7963 6174 6368 3232 3d3d 302e 342e 3220  ycatch22==0.4.2 
-00000940: 2d2d 7573 652d 6465 7072 6563 6174 6564  --use-deprecated
-00000950: 3d6c 6567 6163 792d 7265 736f 6c76 6572  =legacy-resolver
-00000960: 602e 0a0a 4974 2069 7320 616c 736f 2061  `...It is also a
-00000970: 205b 7061 636b 6167 6520 6f6e 2061 6e61   [package on ana
-00000980: 636f 6e64 615d 2868 7474 7073 3a2f 2f61  conda](https://a
-00000990: 6e61 636f 6e64 612e 6f72 672f 636f 6e64  naconda.org/cond
-000009a0: 612d 666f 7267 652f 7079 6361 7463 6832  a-forge/pycatch2
-000009b0: 3229 2074 6861 6e6b 7320 746f 205b 4072  2) thanks to [@r
-000009c0: 7061 6e61 695d 2868 7474 7073 3a2f 2f67  panai](https://g
-000009d0: 6974 6875 622e 636f 6d2f 7270 616e 6169  ithub.com/rpanai
-000009e0: 292c 2077 6869 6368 2079 6f75 2063 616e  ), which you can
-000009f0: 2069 6e73 7461 6c6c 2076 6961 2060 636f   install via `co
-00000a00: 6e64 6160 3a0a 0a60 6060 0a63 6f6e 6461  nda`:..```.conda
-00000a10: 2069 6e73 7461 6c6c 202d 6320 636f 6e64   install -c cond
-00000a20: 612d 666f 7267 6520 7079 6361 7463 6832  a-forge pycatch2
-00000a30: 320a 6060 600a 0a6f 7220 606d 616d 6261  2.```..or `mamba
-00000a40: 603a 0a0a 6060 600a 6d61 6d62 6120 696e  `:..```.mamba in
-00000a50: 7374 616c 6c20 2d63 2063 6f6e 6461 2d66  stall -c conda-f
-00000a60: 6f72 6765 2070 7963 6174 6368 3232 0a60  orge pycatch22.`
-00000a70: 6060 0a0a 5b41 206d 616e 7561 6c20 696e  ``..[A manual in
-00000a80: 7374 616c 6c20 2862 6f74 746f 6d20 6f66  stall (bottom of
-00000a90: 2074 6869 7320 7061 6765 2920 6973 2061   this page) is a
-00000aa0: 206c 6173 7420 7265 736f 7274 2e5d 0a0a   last resort.]..
-00000ab0: 2323 2055 7361 6765 0a0a 4561 6368 2066  ## Usage..Each f
-00000ac0: 6561 7475 7265 2066 756e 6374 696f 6e20  eature function 
-00000ad0: 6361 6e20 6265 2061 6363 6573 7365 6420  can be accessed 
-00000ae0: 696e 6469 7669 6475 616c 6c79 2061 6e64  individually and
-00000af0: 2074 616b 6573 2061 7272 6179 7320 6173   takes arrays as
-00000b00: 2074 7570 6c65 206f 7220 6c69 7374 7320   tuple or lists 
-00000b10: 286e 6f74 2060 6e75 6d70 7960 2061 7272  (not `numpy` arr
-00000b20: 6179 7329 2e0a 466f 7220 6578 616d 706c  ays)..For exampl
-00000b30: 652c 2066 6f72 206c 6f61 6465 6420 6461  e, for loaded da
-00000b40: 7461 2060 7473 4461 7461 6020 696e 2050  ta `tsData` in P
-00000b50: 7974 686f 6e3a 0a0a 6060 6070 7974 686f  ython:..```pytho
-00000b60: 6e33 0a69 6d70 6f72 7420 7079 6361 7463  n3.import pycatc
-00000b70: 6832 320a 7473 4461 7461 203d 205b 312c  h22.tsData = [1,
-00000b80: 322c 342c 335d 2023 2028 6f72 206d 6f72  2,4,3] # (or mor
-00000b90: 6520 696e 7465 7265 7374 696e 6720 6461  e interesting da
-00000ba0: 7461 2129 0a70 7963 6174 6368 3232 2e43  ta!).pycatch22.C
-00000bb0: 4f5f 6631 6563 6163 2874 7344 6174 6129  O_f1ecac(tsData)
-00000bc0: 0a60 6060 0a0a 416c 6c20 6665 6174 7572  .```..All featur
-00000bd0: 6573 2061 7265 2062 756e 646c 6564 2069  es are bundled i
-00000be0: 6e20 7468 6520 6d65 7468 6f64 2060 6361  n the method `ca
-00000bf0: 7463 6832 325f 616c 6c60 2c20 7768 6963  tch22_all`, whic
-00000c00: 6820 616c 736f 2061 6363 6570 7473 2060  h also accepts `
-00000c10: 6e75 6d70 7960 2061 7272 6179 7320 616e  numpy` arrays an
-00000c20: 6420 6769 7665 7320 6261 636b 2061 2064  d gives back a d
-00000c30: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
-00000c40: 6e69 6e67 2074 6865 2065 6e74 7269 6573  ning the entries
-00000c50: 2060 6361 7463 6832 325f 616c 6c5b 276e   `catch22_all['n
-00000c60: 616d 6573 275d 6020 666f 7220 6665 6174  ames']` for feat
-00000c70: 7572 6520 6e61 6d65 7320 616e 6420 6063  ure names and `c
-00000c80: 6174 6368 3232 5f61 6c6c 5b27 7661 6c75  atch22_all['valu
-00000c90: 6573 275d 6020 666f 7220 6665 6174 7572  es']` for featur
-00000ca0: 6520 6f75 7470 7574 732e 0a0a 5573 6167  e outputs...Usag
-00000cb0: 6520 2863 6f6d 7075 7469 6e67 2032 3220  e (computing 22 
-00000cc0: 6665 6174 7572 6573 3a20 5f63 6174 6368  features: _catch
-00000cd0: 3232 5f29 3a0a 0a60 6060 7079 7468 6f6e  22_):..```python
-00000ce0: 330a 7079 6361 7463 6832 322e 6361 7463  3.pycatch22.catc
-00000cf0: 6832 325f 616c 6c28 7473 4461 7461 290a  h22_all(tsData).
-00000d00: 6060 600a 0a55 7361 6765 2028 636f 6d70  ```..Usage (comp
-00000d10: 7574 696e 6720 3234 2066 6561 7475 7265  uting 24 feature
-00000d20: 733a 205f 6361 7463 6832 345f 203d 205f  s: _catch24_ = _
-00000d30: 6361 7463 6832 325f 202b 206d 6561 6e20  catch22_ + mean 
-00000d40: 2b20 7374 616e 6461 7264 2064 6576 6961  + standard devia
-00000d50: 7469 6f6e 293a 0a0a 6060 6070 7974 686f  tion):..```pytho
-00000d60: 6e33 0a70 7963 6174 6368 3232 2e63 6174  n3.pycatch22.cat
-00000d70: 6368 3232 5f61 6c6c 2874 7344 6174 612c  ch22_all(tsData,
-00000d80: 6361 7463 6832 343d 5472 7565 290a 6060  catch24=True).``
-00000d90: 600a 0a57 6520 616c 736f 2069 6e63 6c75  `..We also inclu
-00000da0: 6465 2061 2027 7368 6f72 7420 6e61 6d65  de a 'short name
-00000db0: 2720 666f 7220 6561 6368 2066 6561 7475  ' for each featu
-00000dc0: 7265 2066 6f72 2065 6173 6965 7220 7265  re for easier re
-00000dd0: 6665 7265 6e63 6520 2861 7320 6f75 746c  ference (as outl
-00000de0: 696e 6564 2069 6e20 7468 6520 4769 7442  ined in the GitB
-00000df0: 6f6f 6b20 5b46 6561 7475 7265 206f 7665  ook [Feature ove
-00000e00: 7276 6965 7720 7461 626c 655d 2868 7474  rview table](htt
-00000e10: 7073 3a2f 2f61 7070 2e67 6974 626f 6f6b  ps://app.gitbook
-00000e20: 2e63 6f6d 2f6f 2f2d 4d66 6568 5a71 6143  .com/o/-MfehZqaC
-00000e30: 576e 7353 5244 4964 5547 382f 732f 2d4d  WnsSRDIdUG8/s/-M
-00000e40: 6648 4659 346c 767a 4f7a 3349 5061 4133  fHFY4lvzOz3IPaA3
-00000e50: 776d 2f66 6561 7475 7265 2d6f 7665 7276  wm/feature-overv
-00000e60: 6965 772d 7461 626c 6529 292e 0a54 6865  iew-table))..The
-00000e70: 7365 2073 686f 7274 206e 616d 6573 2063  se short names c
-00000e80: 616e 2062 6520 696e 636c 7564 6564 2069  an be included i
-00000e90: 6e20 7468 6520 6f75 7470 7574 2066 726f  n the output fro
-00000ea0: 6d20 6063 6174 6368 3232 5f61 6c6c 2829  m `catch22_all()
-00000eb0: 6020 6279 2073 6574 7469 6e67 2060 7368  ` by setting `sh
-00000ec0: 6f72 745f 6e61 6d65 733d 5472 7565 6020  ort_names=True` 
-00000ed0: 6173 2066 6f6c 6c6f 7773 3a0a 0a60 6060  as follows:..```
-00000ee0: 7079 7468 6f6e 330a 7079 6361 7463 6832  python3.pycatch2
-00000ef0: 322e 6361 7463 6832 325f 616c 6c28 7473  2.catch22_all(ts
-00000f00: 4461 7461 2c63 6174 6368 3234 3d54 7275  Data,catch24=Tru
-00000f10: 652c 7368 6f72 745f 6e61 6d65 733d 5472  e,short_names=Tr
-00000f20: 7565 290a 6060 600a 0a23 2323 2054 656d  ue).```..### Tem
-00000f30: 706c 6174 6520 616e 616c 7973 6973 2073  plate analysis s
-00000f40: 6372 6970 740a 0a54 6861 6e6b 7320 746f  cript..Thanks to
-00000f50: 205b 406a 6d6f 6f32 3838 305d 2868 7474   [@jmoo2880](htt
-00000f60: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000f70: 6a6d 6f6f 3238 3830 2920 666f 7220 7075  jmoo2880) for pu
-00000f80: 7474 696e 6720 746f 6765 7468 6572 2061  tting together a
-00000f90: 205b 6465 6d6f 6e73 7472 6174 696f 6e20   [demonstration 
-00000fa0: 6e6f 7465 626f 6f6b 5d28 6874 7470 733a  notebook](https:
-00000fb0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6d6f  //github.com/jmo
-00000fc0: 6f32 3838 302f 6332 322d 7573 6167 652d  o2880/c22-usage-
-00000fd0: 6578 616d 706c 6573 2f29 2066 6f72 2075  examples/) for u
-00000fe0: 7369 6e67 2070 7963 6174 6368 3232 2074  sing pycatch22 t
-00000ff0: 6f20 6578 7472 6163 7420 6665 6174 7572  o extract featur
-00001000: 6573 2066 726f 6d20 6120 7469 6d65 2d73  es from a time-s
-00001010: 6572 6965 7320 6461 7461 7365 742e 0a0a  eries dataset...
-00001020: 2323 2320 5573 6167 6520 6e6f 7465 730a  ### Usage notes.
-00001030: 0a2d 2057 6865 6e20 7072 6573 656e 7469  .- When presenti
-00001040: 6e67 2072 6573 756c 7473 2075 7369 6e67  ng results using
-00001050: 205f 6361 7463 6832 325f 2c20 796f 7520   _catch22_, you 
-00001060: 6d75 7374 2069 6465 6e74 6966 7920 7468  must identify th
-00001070: 6520 7665 7273 696f 6e20 7573 6564 2074  e version used t
-00001080: 6f20 616c 6c6f 7720 636c 6561 7220 7265  o allow clear re
-00001090: 7072 6f64 7563 7469 6f6e 206f 6620 796f  production of yo
-000010a0: 7572 2072 6573 756c 7473 2e20 466f 7220  ur results. For 
-000010b0: 6578 616d 706c 652c 2060 434f 5f66 3165  example, `CO_f1e
-000010c0: 6361 6360 2077 6173 2061 6c74 6572 6564  cac` was altered
-000010d0: 2066 726f 6d20 616e 2069 6e74 6567 6572   from an integer
-000010e0: 2d76 616c 7565 6420 6f75 7470 7574 2074  -valued output t
-000010f0: 6f20 6120 6c69 6e65 6172 6c79 2069 6e74  o a linearly int
-00001100: 6572 706f 6c61 7465 6420 7265 616c 2d76  erpolated real-v
-00001110: 616c 7565 6420 6f75 7470 7574 2066 726f  alued output fro
-00001120: 6d20 7630 2e33 2e0a 2d20 5f5f 496d 706f  m v0.3..- __Impo
-00001130: 7274 616e 7420 4e6f 7465 3a5f 5f20 5f63  rtant Note:__ _c
-00001140: 6174 6368 3232 5f20 6665 6174 7572 6573  atch22_ features
-00001150: 206f 6e6c 7920 6576 616c 7561 7465 205f   only evaluate _
-00001160: 6479 6e61 6d69 6361 6c5f 2070 726f 7065  dynamical_ prope
-00001170: 7274 6965 7320 6f66 2074 696d 6520 7365  rties of time se
-00001180: 7269 6573 2061 6e64 2064 6f20 6e6f 7420  ries and do not 
-00001190: 7265 7370 6f6e 6420 746f 2062 6173 6963  respond to basic
-000011a0: 2064 6966 6665 7265 6e63 6573 2069 6e20   differences in 
-000011b0: 7468 6520 6c6f 6361 7469 6f6e 2028 652e  the location (e.
-000011c0: 672e 2c20 6d65 616e 2920 6f72 2073 7072  g., mean) or spr
-000011d0: 6561 6420 2865 2e67 2e2c 2076 6172 6961  ead (e.g., varia
-000011e0: 6e63 6529 2e0a 2020 2d20 4672 6f6d 205f  nce)..  - From _
-000011f0: 6361 7463 6832 325f 2076 302e 332c 2049  catch22_ v0.3, I
-00001200: 6620 7468 6520 6c6f 6361 7469 6f6e 2061  f the location a
-00001210: 6e64 2073 7072 6561 6420 6f66 2074 6865  nd spread of the
-00001220: 2072 6177 2074 696d 652d 7365 7269 6573   raw time-series
-00001230: 2064 6973 7472 6962 7574 696f 6e20 6d61   distribution ma
-00001240: 7920 6265 2069 6d70 6f72 7461 6e74 2066  y be important f
-00001250: 6f72 2079 6f75 7220 6170 706c 6963 6174  or your applicat
-00001260: 696f 6e2c 2077 6520 7375 6767 6573 7420  ion, we suggest 
-00001270: 6170 706c 7969 6e67 2074 6865 2066 756e  applying the fun
-00001280: 6374 696f 6e20 6172 6775 6d65 6e74 2060  ction argument `
-00001290: 6361 7463 6832 3420 3d20 5472 7565 6020  catch24 = True` 
-000012a0: 746f 2079 6f75 7220 6361 6c6c 2074 6f20  to your call to 
-000012b0: 7468 6520 5f63 6174 6368 3232 5f20 6675  the _catch22_ fu
-000012c0: 6e63 7469 6f6e 2069 6e20 7468 6520 6c61  nction in the la
-000012d0: 6e67 7561 6765 206f 6620 796f 7572 2063  nguage of your c
-000012e0: 686f 6963 652e 0a20 2054 6869 7320 7769  hoice..  This wi
-000012f0: 6c6c 2072 6573 756c 7420 696e 2032 3420  ll result in 24 
-00001300: 6665 6174 7572 6573 2062 6569 6e67 2063  features being c
-00001310: 616c 6375 6c61 7465 643a 2074 6865 205f  alculated: the _
-00001320: 6361 7463 6832 325f 2066 6561 7475 7265  catch22_ feature
-00001330: 7320 696e 2061 6464 6974 696f 6e20 746f  s in addition to
-00001340: 206d 6561 6e20 616e 6420 7374 616e 6461   mean and standa
-00001350: 7264 2064 6576 6961 7469 6f6e 2e0a 0a23  rd deviation...#
-00001360: 2323 204d 616e 7561 6c20 696e 7374 616c  ## Manual instal
-00001370: 6c0a 0a49 6620 796f 7520 6669 6e64 2069  l..If you find i
-00001380: 7373 7565 7320 7769 7468 2074 6865 2060  ssues with the `
-00001390: 7069 7060 2069 6e73 7461 6c6c 2c20 796f  pip` install, yo
-000013a0: 7520 6361 6e20 616c 736f 2069 6e73 7461  u can also insta
-000013b0: 6c6c 2075 7369 6e67 2060 7365 7475 7074  ll using `setupt
-000013c0: 6f6f 6c73 603a 0a0a 6060 600a 7079 7468  ools`:..```.pyth
-000013d0: 6f6e 3320 7365 7475 702e 7079 2062 7569  on3 setup.py bui
-000013e0: 6c64 0a70 7974 686f 6e33 2073 6574 7570  ld.python3 setup
-000013f0: 2e70 7920 696e 7374 616c 6c0a 6060 600a  .py install.```.
+000002b0: 4669 6c65 3a20 4c49 4345 4e53 450a 0a3c  File: LICENSE..<
+000002c0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+000002d0: 3e3c 696d 6720 7372 633d 2269 6d67 2f63  ><img src="img/c
+000002e0: 6174 6368 3232 5f6c 6f67 6f5f 7371 7561  atch22_logo_squa
+000002f0: 7265 2e70 6e67 2220 616c 743d 2263 6174  re.png" alt="cat
+00000300: 6368 3232 206c 6f67 6f22 2068 6569 6768  ch22 logo" heigh
+00000310: 743d 2232 3230 222f 3e3c 2f70 3e0a 0a3c  t="220"/></p>..<
+00000320: 6831 2061 6c69 676e 3d22 6365 6e74 6572  h1 align="center
+00000330: 223e 3c65 6d3e 7079 6361 7463 6832 323c  "><em>pycatch22<
+00000340: 2f65 6d3e 3a20 4341 6e6f 6e69 6361 6c20  /em>: CAnonical 
+00000350: 5469 6d65 2d73 6572 6965 7320 4348 6172  Time-series CHar
+00000360: 6163 7465 7269 7374 6963 7320 696e 2070  acteristics in p
+00000370: 7974 686f 6e3c 2f68 313e 0a0a 3c70 2061  ython</h1>..<p a
+00000380: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+00000390: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+000003a0: 733a 2f2f 7777 772e 676e 752e 6f72 672f  s://www.gnu.org/
+000003b0: 6c69 6365 6e73 6573 2f67 706c 2d33 2e30  licenses/gpl-3.0
+000003c0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+000003d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000003e0: 696f 2f62 6164 6765 2f4c 6963 656e 7365  io/badge/License
+000003f0: 2d47 504c 7633 2d62 6c75 652e 7376 6722  -GPLv3-blue.svg"
+00000400: 2068 6569 6768 743d 2232 3022 2f3e 3c2f   height="20"/></
+00000410: 613e 0a20 0920 203c 6120 6872 6566 3d22  a>. .  <a href="
+00000420: 6874 7470 733a 2f2f 7477 6974 7465 722e  https://twitter.
+00000430: 636f 6d2f 636f 6d70 5469 6d65 5365 7269  com/compTimeSeri
+00000440: 6573 223e 3c69 6d67 2073 7263 3d22 6874  es"><img src="ht
+00000450: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000460: 732e 696f 2f74 7769 7474 6572 2f75 726c  s.io/twitter/url
+00000470: 2f68 7474 7073 2f74 7769 7474 6572 2e63  /https/twitter.c
+00000480: 6f6d 2f63 6f6d 7054 696d 6553 6572 6965  om/compTimeSerie
+00000490: 732e 7376 673f 7374 796c 653d 736f 6369  s.svg?style=soci
+000004a0: 616c 266c 6162 656c 3d46 6f6c 6c6f 7725  al&label=Follow%
+000004b0: 3230 2534 3063 6f6d 7054 696d 6553 6572  20%40compTimeSer
+000004c0: 6965 7322 2068 6569 6768 743d 2232 3022  ies" height="20"
+000004d0: 2f3e 3c2f 613e 0a3c 2f70 3e0a 0a0a 2323  /></a>.</p>...##
+000004e0: 2041 626f 7574 0a0a 5b5f 6361 7463 6832   About..[_catch2
+000004f0: 325f 5d28 6874 7470 733a 2f2f 6769 7468  2_](https://gith
+00000500: 7562 2e63 6f6d 2f44 796e 616d 6963 7341  ub.com/DynamicsA
+00000510: 6e64 4e65 7572 616c 5379 7374 656d 732f  ndNeuralSystems/
+00000520: 6361 7463 6832 3229 2069 7320 6120 636f  catch22) is a co
+00000530: 6c6c 6563 7469 6f6e 206f 6620 3232 2074  llection of 22 t
+00000540: 696d 652d 7365 7269 6573 2066 6561 7475  ime-series featu
+00000550: 7265 7320 636f 6465 6420 696e 2043 2074  res coded in C t
+00000560: 6861 7420 6361 6e20 6265 2072 756e 2066  hat can be run f
+00000570: 726f 6d20 5079 7468 6f6e 2c20 6173 2077  rom Python, as w
+00000580: 656c 6c20 6173 205b 525d 2868 7474 7073  ell as [R](https
+00000590: 3a2f 2f67 6974 6875 622e 636f 6d2f 6865  ://github.com/he
+000005a0: 6e64 6572 736f 6e74 7265 6e74 2f52 6361  ndersontrent/Rca
+000005b0: 7463 6832 3229 2c20 5b4d 6174 6c61 625d  tch22), [Matlab]
+000005c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000005d0: 636f 6d2f 4479 6e61 6d69 6373 416e 644e  com/DynamicsAndN
+000005e0: 6575 7261 6c53 7973 7465 6d73 2f63 6174  euralSystems/cat
+000005f0: 6368 3232 292c 2061 6e64 205b 4a75 6c69  ch22), and [Juli
+00000600: 615d 2868 7474 7073 3a2f 2f67 6974 6875  a](https://githu
+00000610: 622e 636f 6d2f 6272 656e 6461 6e6a 6f68  b.com/brendanjoh
+00000620: 6e68 6172 7269 732f 4361 7463 6832 322e  nharris/Catch22.
+00000630: 6a6c 292e 0a0a 5468 6973 2070 6163 6b61  jl)...This packa
+00000640: 6765 2070 726f 7669 6465 7320 6120 7079  ge provides a py
+00000650: 7468 6f6e 2069 6d70 6c65 6d65 6e74 6174  thon implementat
+00000660: 696f 6e20 6173 2074 6865 206d 6f64 756c  ion as the modul
+00000670: 6520 5f70 7963 6174 6368 3232 5f2c 206c  e _pycatch22_, l
+00000680: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
+00000690: 6520 5b47 4e55 2047 504c 2076 3320 6c69  e [GNU GPL v3 li
+000006a0: 6365 6e73 655d 2868 7474 703a 2f2f 7777  cense](http://ww
+000006b0: 772e 676e 752e 6f72 672f 6c69 6365 6e73  w.gnu.org/licens
+000006c0: 6573 2f67 706c 2d33 2e30 2e68 746d 6c29  es/gpl-3.0.html)
+000006d0: 2028 6f72 206c 6174 6572 292e 0a0a 2323   (or later)...##
+000006e0: 2320 5768 6174 2064 6f20 7468 6520 6665  # What do the fe
+000006f0: 6174 7572 6573 2064 6f3f 0a0a 5468 6973  atures do?..This
+00000700: 205b 4769 7442 6f6f 6b73 2077 6562 7369   [GitBooks websi
+00000710: 7465 5d28 6874 7470 733a 2f2f 7469 6d65  te](https://time
+00000720: 2d73 6572 6965 732d 6665 6174 7572 6573  -series-features
+00000730: 2e67 6974 626f 6f6b 2e69 6f2f 6361 7463  .gitbook.io/catc
+00000740: 6832 322f 6665 6174 7572 652d 6465 7363  h22/feature-desc
+00000750: 7269 7074 696f 6e73 2920 6973 2064 6564  riptions) is ded
+00000760: 6963 6174 6564 2074 6f20 6465 7363 7269  icated to descri
+00000770: 6269 6e67 2074 6865 2066 6561 7475 7265  bing the feature
+00000780: 732e 0a46 6f72 2074 6865 6972 2069 6d70  s..For their imp
+00000790: 6c65 6d65 6e74 6174 696f 6e20 696e 2063  lementation in c
+000007a0: 6f64 652c 2073 6565 2074 6865 205b 6d61  ode, see the [ma
+000007b0: 696e 205f 6361 7463 6832 325f 2072 6570  in _catch22_ rep
+000007c0: 6f73 6974 6f72 795d 2868 7474 7073 3a2f  ository](https:/
+000007d0: 2f67 6974 6875 622e 636f 6d2f 4479 6e61  /github.com/Dyna
+000007e0: 6d69 6373 416e 644e 6575 7261 6c53 7973  micsAndNeuralSys
+000007f0: 7465 6d73 2f63 6174 6368 3232 292e 0a54  tems/catch22)..T
+00000800: 6865 7265 2069 7320 616c 736f 2069 6e66  here is also inf
+00000810: 6f72 6d61 7469 6f6e 2069 6e20 7468 6520  ormation in the 
+00000820: 6173 736f 6369 6174 6564 2070 6170 6572  associated paper
+00000830: 205b 2623 7831 4634 4437 3b20 4c75 6262   [&#x1F4D7; Lubb
+00000840: 6120 6574 2061 6c2e 2028 3230 3139 292e  a et al. (2019).
+00000850: 5d28 6874 7470 733a 2f2f 646f 692e 6f72  ](https://doi.or
+00000860: 672f 3130 2e31 3030 372f 7331 3036 3138  g/10.1007/s10618
+00000870: 2d30 3139 2d30 3036 3437 2d78 292e 0a0a  -019-00647-x)...
+00000880: 2323 2320 4163 6b6e 6f77 6c65 6467 656d  ### Acknowledgem
+00000890: 656e 7420 3a2b 313a 0a0a 4966 2079 6f75  ent :+1:..If you
+000008a0: 2075 7365 2074 6869 7320 736f 6674 7761   use this softwa
+000008b0: 7265 2c20 706c 6561 7365 2072 6561 6420  re, please read 
+000008c0: 616e 6420 6369 7465 2074 6869 7320 6f70  and cite this op
+000008d0: 656e 2d61 6363 6573 7320 6172 7469 636c  en-access articl
+000008e0: 653a 0a0a 2d20 2623 7831 4634 4437 3b20  e:..- &#x1F4D7; 
+000008f0: 4c75 6262 6120 6574 2061 6c2e 205b 5f63  Lubba et al. [_c
+00000900: 6174 6368 3232 5f3a 2043 416e 6f6e 6963  atch22_: CAnonic
+00000910: 616c 2054 696d 652d 7365 7269 6573 2043  al Time-series C
+00000920: 4861 7261 6374 6572 6973 7469 6373 5d28  Haracteristics](
+00000930: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
+00000940: 3130 2e31 3030 372f 7331 3036 3138 2d30  10.1007/s10618-0
+00000950: 3139 2d30 3036 3437 2d78 292c 205f 4461  19-00647-x), _Da
+00000960: 7461 204d 696e 204b 6e6f 776c 2044 6973  ta Min Knowl Dis
+00000970: 635f 205f 5f33 335f 5f2c 2031 3832 3120  c_ __33__, 1821 
+00000980: 2832 3031 3929 2e0a 0a23 2320 496e 7374  (2019)...## Inst
+00000990: 616c 6c61 7469 6f6e 0a0a 5573 696e 6720  allation..Using 
+000009a0: 6070 6970 6020 666f 7220 5b60 7079 6361  `pip` for [`pyca
+000009b0: 7463 6832 3260 5d28 6874 7470 733a 2f2f  tch22`](https://
+000009c0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000009d0: 2f70 7963 6174 6368 3232 2f29 3a0a 0a60  /pycatch22/):..`
+000009e0: 6060 0a70 6970 2069 6e73 7461 6c6c 2070  ``.pip install p
+000009f0: 7963 6174 6368 3232 0a60 6060 0a0a 4966  ycatch22.```..If
+00000a00: 2074 6869 7320 646f 6573 6e27 7420 776f   this doesn't wo
+00000a10: 726b 2c20 6d61 6b65 2073 7572 6520 796f  rk, make sure yo
+00000a20: 7520 6172 6520 7573 696e 6720 7468 6520  u are using the 
+00000a30: 6c61 7465 7374 2060 7365 7475 7074 6f6f  latest `setuptoo
+00000a40: 6c73 603a 2060 7069 7020 696e 7374 616c  ls`: `pip instal
+00000a50: 6c20 7365 7475 7074 6f6f 6c73 202d 2d75  l setuptools --u
+00000a60: 7067 7261 6465 602e 0a0a 4966 2079 6f75  pgrade`...If you
+00000a70: 2063 6f6d 6520 6163 726f 7373 2065 7272   come across err
+00000a80: 6f72 7320 7769 7468 2076 6572 7369 6f6e  ors with version
+00000a90: 2072 6573 6f6c 7574 696f 6e2c 2079 6f75   resolution, you
+00000aa0: 2073 686f 756c 6420 7472 7920 736f 6d65   should try some
+00000ab0: 7468 696e 6720 6c69 6b65 3a20 6070 6970  thing like: `pip
+00000ac0: 2069 6e73 7461 6c6c 2070 7963 6174 6368   install pycatch
+00000ad0: 3232 3d3d 302e 342e 3220 2d2d 7573 652d  22==0.4.2 --use-
+00000ae0: 6465 7072 6563 6174 6564 3d6c 6567 6163  deprecated=legac
+00000af0: 792d 7265 736f 6c76 6572 602e 0a0a 4974  y-resolver`...It
+00000b00: 2069 7320 616c 736f 2061 205b 7061 636b   is also a [pack
+00000b10: 6167 6520 6f6e 2061 6e61 636f 6e64 615d  age on anaconda]
+00000b20: 2868 7474 7073 3a2f 2f61 6e61 636f 6e64  (https://anacond
+00000b30: 612e 6f72 672f 636f 6e64 612d 666f 7267  a.org/conda-forg
+00000b40: 652f 7079 6361 7463 6832 3229 2074 6861  e/pycatch22) tha
+00000b50: 6e6b 7320 746f 205b 4072 7061 6e61 695d  nks to [@rpanai]
+00000b60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000b70: 636f 6d2f 7270 616e 6169 292c 2077 6869  com/rpanai), whi
+00000b80: 6368 2079 6f75 2063 616e 2069 6e73 7461  ch you can insta
+00000b90: 6c6c 2076 6961 2060 636f 6e64 6160 3a0a  ll via `conda`:.
+00000ba0: 0a60 6060 0a63 6f6e 6461 2069 6e73 7461  .```.conda insta
+00000bb0: 6c6c 202d 6320 636f 6e64 612d 666f 7267  ll -c conda-forg
+00000bc0: 6520 7079 6361 7463 6832 320a 6060 600a  e pycatch22.```.
+00000bd0: 0a6f 7220 606d 616d 6261 603a 0a0a 6060  .or `mamba`:..``
+00000be0: 600a 6d61 6d62 6120 696e 7374 616c 6c20  `.mamba install 
+00000bf0: 2d63 2063 6f6e 6461 2d66 6f72 6765 2070  -c conda-forge p
+00000c00: 7963 6174 6368 3232 0a60 6060 0a0a 5b41  ycatch22.```..[A
+00000c10: 206d 616e 7561 6c20 696e 7374 616c 6c20   manual install 
+00000c20: 2862 6f74 746f 6d20 6f66 2074 6869 7320  (bottom of this 
+00000c30: 7061 6765 2920 6973 2061 206c 6173 7420  page) is a last 
+00000c40: 7265 736f 7274 2e5d 0a0a 2323 2055 7361  resort.]..## Usa
+00000c50: 6765 0a0a 4561 6368 2066 6561 7475 7265  ge..Each feature
+00000c60: 2066 756e 6374 696f 6e20 6361 6e20 6265   function can be
+00000c70: 2061 6363 6573 7365 6420 696e 6469 7669   accessed indivi
+00000c80: 6475 616c 6c79 2061 6e64 2074 616b 6573  dually and takes
+00000c90: 2061 7272 6179 7320 6173 2074 7570 6c65   arrays as tuple
+00000ca0: 206f 7220 6c69 7374 7320 286e 6f74 2060   or lists (not `
+00000cb0: 6e75 6d70 7960 2061 7272 6179 7329 2e0a  numpy` arrays)..
+00000cc0: 466f 7220 6578 616d 706c 652c 2066 6f72  For example, for
+00000cd0: 206c 6f61 6465 6420 6461 7461 2060 7473   loaded data `ts
+00000ce0: 4461 7461 6020 696e 2050 7974 686f 6e3a  Data` in Python:
+00000cf0: 0a0a 6060 6070 7974 686f 6e33 0a69 6d70  ..```python3.imp
+00000d00: 6f72 7420 7079 6361 7463 6832 320a 7473  ort pycatch22.ts
+00000d10: 4461 7461 203d 205b 312c 322c 342c 335d  Data = [1,2,4,3]
+00000d20: 2023 2028 6f72 206d 6f72 6520 696e 7465   # (or more inte
+00000d30: 7265 7374 696e 6720 6461 7461 2129 0a70  resting data!).p
+00000d40: 7963 6174 6368 3232 2e43 4f5f 6631 6563  ycatch22.CO_f1ec
+00000d50: 6163 2874 7344 6174 6129 0a60 6060 0a0a  ac(tsData).```..
+00000d60: 416c 6c20 6665 6174 7572 6573 2061 7265  All features are
+00000d70: 2062 756e 646c 6564 2069 6e20 7468 6520   bundled in the 
+00000d80: 6d65 7468 6f64 2060 6361 7463 6832 325f  method `catch22_
+00000d90: 616c 6c60 2c20 7768 6963 6820 616c 736f  all`, which also
+00000da0: 2061 6363 6570 7473 2060 6e75 6d70 7960   accepts `numpy`
+00000db0: 2061 7272 6179 7320 616e 6420 6769 7665   arrays and give
+00000dc0: 7320 6261 636b 2061 2064 6963 7469 6f6e  s back a diction
+00000dd0: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
+00000de0: 6865 2065 6e74 7269 6573 2060 6361 7463  he entries `catc
+00000df0: 6832 325f 616c 6c5b 276e 616d 6573 275d  h22_all['names']
+00000e00: 6020 666f 7220 6665 6174 7572 6520 6e61  ` for feature na
+00000e10: 6d65 7320 616e 6420 6063 6174 6368 3232  mes and `catch22
+00000e20: 5f61 6c6c 5b27 7661 6c75 6573 275d 6020  _all['values']` 
+00000e30: 666f 7220 6665 6174 7572 6520 6f75 7470  for feature outp
+00000e40: 7574 732e 0a0a 5573 6167 6520 2863 6f6d  uts...Usage (com
+00000e50: 7075 7469 6e67 2032 3220 6665 6174 7572  puting 22 featur
+00000e60: 6573 3a20 5f63 6174 6368 3232 5f29 3a0a  es: _catch22_):.
+00000e70: 0a60 6060 7079 7468 6f6e 330a 7079 6361  .```python3.pyca
+00000e80: 7463 6832 322e 6361 7463 6832 325f 616c  tch22.catch22_al
+00000e90: 6c28 7473 4461 7461 290a 6060 600a 0a55  l(tsData).```..U
+00000ea0: 7361 6765 2028 636f 6d70 7574 696e 6720  sage (computing 
+00000eb0: 3234 2066 6561 7475 7265 733a 205f 6361  24 features: _ca
+00000ec0: 7463 6832 345f 203d 205f 6361 7463 6832  tch24_ = _catch2
+00000ed0: 325f 202b 206d 6561 6e20 2b20 7374 616e  2_ + mean + stan
+00000ee0: 6461 7264 2064 6576 6961 7469 6f6e 293a  dard deviation):
+00000ef0: 0a0a 6060 6070 7974 686f 6e33 0a70 7963  ..```python3.pyc
+00000f00: 6174 6368 3232 2e63 6174 6368 3232 5f61  atch22.catch22_a
+00000f10: 6c6c 2874 7344 6174 612c 6361 7463 6832  ll(tsData,catch2
+00000f20: 343d 5472 7565 290a 6060 600a 0a57 6520  4=True).```..We 
+00000f30: 616c 736f 2069 6e63 6c75 6465 2061 2027  also include a '
+00000f40: 7368 6f72 7420 6e61 6d65 2720 666f 7220  short name' for 
+00000f50: 6561 6368 2066 6561 7475 7265 2066 6f72  each feature for
+00000f60: 2065 6173 6965 7220 7265 6665 7265 6e63   easier referenc
+00000f70: 6520 2861 7320 6f75 746c 696e 6564 2069  e (as outlined i
+00000f80: 6e20 7468 6520 4769 7442 6f6f 6b20 5b46  n the GitBook [F
+00000f90: 6561 7475 7265 206f 7665 7276 6965 7720  eature overview 
+00000fa0: 7461 626c 655d 2868 7474 7073 3a2f 2f74  table](https://t
+00000fb0: 696d 652d 7365 7269 6573 2d66 6561 7475  ime-series-featu
+00000fc0: 7265 732e 6769 7462 6f6f 6b2e 696f 2f63  res.gitbook.io/c
+00000fd0: 6174 6368 3232 2f66 6561 7475 7265 2d64  atch22/feature-d
+00000fe0: 6573 6372 6970 7469 6f6e 732f 6665 6174  escriptions/feat
+00000ff0: 7572 652d 6f76 6572 7669 6577 2d74 6162  ure-overview-tab
+00001000: 6c65 2929 2e0a 5468 6573 6520 7368 6f72  le))..These shor
+00001010: 7420 6e61 6d65 7320 6361 6e20 6265 2069  t names can be i
+00001020: 6e63 6c75 6465 6420 696e 2074 6865 206f  ncluded in the o
+00001030: 7574 7075 7420 6672 6f6d 2060 6361 7463  utput from `catc
+00001040: 6832 325f 616c 6c28 2960 2062 7920 7365  h22_all()` by se
+00001050: 7474 696e 6720 6073 686f 7274 5f6e 616d  tting `short_nam
+00001060: 6573 3d54 7275 6560 2061 7320 666f 6c6c  es=True` as foll
+00001070: 6f77 733a 0a0a 6060 6070 7974 686f 6e33  ows:..```python3
+00001080: 0a70 7963 6174 6368 3232 2e63 6174 6368  .pycatch22.catch
+00001090: 3232 5f61 6c6c 2874 7344 6174 612c 6361  22_all(tsData,ca
+000010a0: 7463 6832 343d 5472 7565 2c73 686f 7274  tch24=True,short
+000010b0: 5f6e 616d 6573 3d54 7275 6529 0a60 6060  _names=True).```
+000010c0: 0a0a 2323 2320 5465 6d70 6c61 7465 2061  ..### Template a
+000010d0: 6e61 6c79 7369 7320 7363 7269 7074 0a0a  nalysis script..
+000010e0: 5468 616e 6b73 2074 6f20 5b40 6a6d 6f6f  Thanks to [@jmoo
+000010f0: 3238 3830 5d28 6874 7470 733a 2f2f 6769  2880](https://gi
+00001100: 7468 7562 2e63 6f6d 2f6a 6d6f 6f32 3838  thub.com/jmoo288
+00001110: 3029 2066 6f72 2070 7574 7469 6e67 2074  0) for putting t
+00001120: 6f67 6574 6865 7220 6120 5b64 656d 6f6e  ogether a [demon
+00001130: 7374 7261 7469 6f6e 206e 6f74 6562 6f6f  stration noteboo
+00001140: 6b5d 2868 7474 7073 3a2f 2f67 6974 6875  k](https://githu
+00001150: 622e 636f 6d2f 6a6d 6f6f 3238 3830 2f63  b.com/jmoo2880/c
+00001160: 3232 2d75 7361 6765 2d65 7861 6d70 6c65  22-usage-example
+00001170: 732f 2920 666f 7220 7573 696e 6720 7079  s/) for using py
+00001180: 6361 7463 6832 3220 746f 2065 7874 7261  catch22 to extra
+00001190: 6374 2066 6561 7475 7265 7320 6672 6f6d  ct features from
+000011a0: 2061 2074 696d 652d 7365 7269 6573 2064   a time-series d
+000011b0: 6174 6173 6574 2e0a 0a23 2323 2055 7361  ataset...### Usa
+000011c0: 6765 206e 6f74 6573 0a0a 2d20 5768 656e  ge notes..- When
+000011d0: 2070 7265 7365 6e74 696e 6720 7265 7375   presenting resu
+000011e0: 6c74 7320 7573 696e 6720 5f63 6174 6368  lts using _catch
+000011f0: 3232 5f2c 2079 6f75 206d 7573 7420 6964  22_, you must id
+00001200: 656e 7469 6679 2074 6865 2076 6572 7369  entify the versi
+00001210: 6f6e 2075 7365 6420 746f 2061 6c6c 6f77  on used to allow
+00001220: 2063 6c65 6172 2072 6570 726f 6475 6374   clear reproduct
+00001230: 696f 6e20 6f66 2079 6f75 7220 7265 7375  ion of your resu
+00001240: 6c74 732e 2046 6f72 2065 7861 6d70 6c65  lts. For example
+00001250: 2c20 6043 4f5f 6631 6563 6163 6020 7761  , `CO_f1ecac` wa
+00001260: 7320 616c 7465 7265 6420 6672 6f6d 2061  s altered from a
+00001270: 6e20 696e 7465 6765 722d 7661 6c75 6564  n integer-valued
+00001280: 206f 7574 7075 7420 746f 2061 206c 696e   output to a lin
+00001290: 6561 726c 7920 696e 7465 7270 6f6c 6174  early interpolat
+000012a0: 6564 2072 6561 6c2d 7661 6c75 6564 206f  ed real-valued o
+000012b0: 7574 7075 7420 6672 6f6d 2076 302e 332e  utput from v0.3.
+000012c0: 0a2d 205f 5f49 6d70 6f72 7461 6e74 204e  .- __Important N
+000012d0: 6f74 653a 5f5f 205f 6361 7463 6832 325f  ote:__ _catch22_
+000012e0: 2066 6561 7475 7265 7320 6f6e 6c79 2065   features only e
+000012f0: 7661 6c75 6174 6520 5f64 796e 616d 6963  valuate _dynamic
+00001300: 616c 5f20 7072 6f70 6572 7469 6573 206f  al_ properties o
+00001310: 6620 7469 6d65 2073 6572 6965 7320 616e  f time series an
+00001320: 6420 646f 206e 6f74 2072 6573 706f 6e64  d do not respond
+00001330: 2074 6f20 6261 7369 6320 6469 6666 6572   to basic differ
+00001340: 656e 6365 7320 696e 2074 6865 206c 6f63  ences in the loc
+00001350: 6174 696f 6e20 2865 2e67 2e2c 206d 6561  ation (e.g., mea
+00001360: 6e29 206f 7220 7370 7265 6164 2028 652e  n) or spread (e.
+00001370: 672e 2c20 7661 7269 616e 6365 292e 0a20  g., variance).. 
+00001380: 202d 2046 726f 6d20 5f63 6174 6368 3232   - From _catch22
+00001390: 5f20 7630 2e33 2c20 4966 2074 6865 206c  _ v0.3, If the l
+000013a0: 6f63 6174 696f 6e20 616e 6420 7370 7265  ocation and spre
+000013b0: 6164 206f 6620 7468 6520 7261 7720 7469  ad of the raw ti
+000013c0: 6d65 2d73 6572 6965 7320 6469 7374 7269  me-series distri
+000013d0: 6275 7469 6f6e 206d 6179 2062 6520 696d  bution may be im
+000013e0: 706f 7274 616e 7420 666f 7220 796f 7572  portant for your
+000013f0: 2061 7070 6c69 6361 7469 6f6e 2c20 7765   application, we
+00001400: 2073 7567 6765 7374 2061 7070 6c79 696e   suggest applyin
+00001410: 6720 7468 6520 6675 6e63 7469 6f6e 2061  g the function a
+00001420: 7267 756d 656e 7420 6063 6174 6368 3234  rgument `catch24
+00001430: 203d 2054 7275 6560 2074 6f20 796f 7572   = True` to your
+00001440: 2063 616c 6c20 746f 2074 6865 205f 6361   call to the _ca
+00001450: 7463 6832 325f 2066 756e 6374 696f 6e20  tch22_ function 
+00001460: 696e 2074 6865 206c 616e 6775 6167 6520  in the language 
+00001470: 6f66 2079 6f75 7220 6368 6f69 6365 2e0a  of your choice..
+00001480: 2020 5468 6973 2077 696c 6c20 7265 7375    This will resu
+00001490: 6c74 2069 6e20 3234 2066 6561 7475 7265  lt in 24 feature
+000014a0: 7320 6265 696e 6720 6361 6c63 756c 6174  s being calculat
+000014b0: 6564 3a20 7468 6520 5f63 6174 6368 3232  ed: the _catch22
+000014c0: 5f20 6665 6174 7572 6573 2069 6e20 6164  _ features in ad
+000014d0: 6469 7469 6f6e 2074 6f20 6d65 616e 2061  dition to mean a
+000014e0: 6e64 2073 7461 6e64 6172 6420 6465 7669  nd standard devi
+000014f0: 6174 696f 6e2e 0a0a 2323 2320 4d61 6e75  ation...### Manu
+00001500: 616c 2069 6e73 7461 6c6c 0a0a 4966 2079  al install..If y
+00001510: 6f75 2066 696e 6420 6973 7375 6573 2077  ou find issues w
+00001520: 6974 6820 7468 6520 6070 6970 6020 696e  ith the `pip` in
+00001530: 7374 616c 6c2c 2079 6f75 2063 616e 2061  stall, you can a
+00001540: 6c73 6f20 696e 7374 616c 6c20 7573 696e  lso install usin
+00001550: 6720 6073 6574 7570 746f 6f6c 7360 3a0a  g `setuptools`:.
+00001560: 0a60 6060 0a70 7974 686f 6e33 2073 6574  .```.python3 set
+00001570: 7570 2e70 7920 6275 696c 640a 7079 7468  up.py build.pyth
+00001580: 6f6e 3320 7365 7475 702e 7079 2069 6e73  on3 setup.py ins
+00001590: 7461 6c6c 0a60 6060 0a                   tall.```.
```

### Comparing `pycatch22-0.4.4/src/pycatch22.egg-info/SOURCES.txt` & `pycatch22-0.4.5/src/pycatch22.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-src/.DS_Store
 src/C/CO_AutoCorr.c
 src/C/CO_AutoCorr.h
 src/C/DN_HistogramMode_10.c
 src/C/DN_HistogramMode_10.h
 src/C/DN_HistogramMode_5.c
 src/C/DN_HistogramMode_5.h
 src/C/DN_Mean.c
@@ -54,8 +53,8 @@
 src/C/stats.h
 src/pycatch22/__init__.py
 src/pycatch22/catch22.py
 src/pycatch22.egg-info/PKG-INFO
 src/pycatch22.egg-info/SOURCES.txt
 src/pycatch22.egg-info/dependency_links.txt
 src/pycatch22.egg-info/top_level.txt
-tests/testing.py
+tests/test_features.py
```

