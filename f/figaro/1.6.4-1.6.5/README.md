# Comparing `tmp/figaro-1.6.4.tar.gz` & `tmp/figaro-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figaro-1.6.4.tar", last modified: Mon Apr 29 10:57:10 2024, max compression
+gzip compressed data, was "figaro-1.6.5.tar", last modified: Tue May 14 11:24:22 2024, max compression
```

## Comparing `figaro-1.6.4.tar` & `figaro-1.6.5.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.433303 figaro-1.6.4/
--rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.4/LICENSE
--rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.4/MANIFEST.in
--rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-29 10:57:10.433081 figaro-1.6.4/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     4154 2024-02-15 08:23:51.000000 figaro-1.6.4/README.md
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.416997 figaro-1.6.4/docs/
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.422284 figaro-1.6.4/docs/source/
--rw-r--r--   0 rinaldi    (503) staff       (20)      317 2024-02-15 08:23:51.000000 figaro-1.6.4/docs/source/api.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-04-24 14:23:00.000000 figaro-1.6.4/docs/source/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-04-24 14:23:08.000000 figaro-1.6.4/docs/source/figaro.rate.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      293 2024-02-15 08:23:51.000000 figaro-1.6.4/docs/source/figaro.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.utils.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.424393 figaro-1.6.4/docs/source/generated/
--rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.utils.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)     1009 2024-02-15 08:23:51.000000 figaro-1.6.4/docs/source/index.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.430426 figaro-1.6.4/figaro/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.4/figaro/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     5008 2024-04-16 11:57:13.000000 figaro-1.6.4/figaro/_likelihood.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1612 2024-03-15 18:23:44.000000 figaro-1.6.4/figaro/_numba_functions.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.432496 figaro-1.6.4/figaro/_pipelines/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.4/figaro/_pipelines/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    19853 2024-04-23 15:23:17.000000 figaro-1.6.4/figaro/_pipelines/hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    23315 2024-04-26 15:10:23.000000 figaro-1.6.4/figaro/_pipelines/par_hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    10411 2024-04-29 10:56:16.000000 figaro-1.6.4/figaro/_pipelines/par_probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     9221 2024-04-18 07:25:04.000000 figaro-1.6.4/figaro/_pipelines/probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2818 2024-04-18 07:51:37.000000 figaro-1.6.4/figaro/cosmology.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.4/figaro/credible_regions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-04-22 12:27:42.000000 figaro-1.6.4/figaro/cumulative.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1304 2024-04-17 14:55:45.000000 figaro-1.6.4/figaro/decorators.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     8460 2024-02-10 17:20:30.000000 figaro-1.6.4/figaro/diagnostic.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.4/figaro/exceptions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    34199 2024-04-22 14:26:21.000000 figaro-1.6.4/figaro/load.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     6348 2024-04-16 13:52:44.000000 figaro-1.6.4/figaro/marginal.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    55429 2024-04-22 14:27:23.000000 figaro-1.6.4/figaro/mixture.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.4/figaro/montecarlo.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    40563 2024-04-26 15:09:38.000000 figaro-1.6.4/figaro/plot.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-04-23 20:48:47.000000 figaro-1.6.4/figaro/plot_settings.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    12084 2024-04-24 15:08:47.000000 figaro-1.6.4/figaro/rate.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.4/figaro/transform.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    16046 2024-04-17 08:40:42.000000 figaro-1.6.4/figaro/utils.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.432811 figaro-1.6.4/figaro.egg-info/
--rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-29 10:57:10.000000 figaro-1.6.4/figaro.egg-info/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     1789 2024-04-29 10:57:10.000000 figaro-1.6.4/figaro.egg-info/SOURCES.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-04-29 10:57:10.000000 figaro-1.6.4/figaro.egg-info/dependency_links.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-04-29 10:57:10.000000 figaro-1.6.4/figaro.egg-info/entry_points.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-04-29 10:57:10.000000 figaro-1.6.4/figaro.egg-info/requires.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-04-29 10:57:10.000000 figaro-1.6.4/figaro.egg-info/top_level.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-04-29 10:56:50.000000 figaro-1.6.4/pyproject.toml
--rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-04-29 10:57:10.433352 figaro-1.6.4/setup.cfg
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:24:22.878792 figaro-1.6.5/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.5/LICENSE
+-rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.5/MANIFEST.in
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-05-14 11:24:22.878568 figaro-1.6.5/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     4154 2024-02-15 08:23:51.000000 figaro-1.6.5/README.md
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:24:22.858991 figaro-1.6.5/docs/
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:24:22.864366 figaro-1.6.5/docs/source/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      332 2024-05-08 10:09:00.000000 figaro-1.6.5/docs/source/api.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-04-24 14:23:00.000000 figaro-1.6.5/docs/source/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-04-24 14:23:08.000000 figaro-1.6.5/docs/source/figaro.rate.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      308 2024-05-10 07:52:32.000000 figaro-1.6.5/docs/source/figaro.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/figaro.utils.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:24:22.867506 figaro-1.6.5/docs/source/generated/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/generated/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/generated/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/generated/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/generated/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/generated/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/generated/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/generated/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/generated/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/generated/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/generated/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/generated/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.5/docs/source/generated/figaro.utils.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1911 2024-05-13 06:45:07.000000 figaro-1.6.5/docs/source/index.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:24:22.874587 figaro-1.6.5/figaro/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.5/figaro/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     5008 2024-04-16 11:57:13.000000 figaro-1.6.5/figaro/_likelihood.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1612 2024-03-15 18:23:44.000000 figaro-1.6.5/figaro/_numba_functions.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:24:22.877424 figaro-1.6.5/figaro/_pipelines/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.5/figaro/_pipelines/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    20100 2024-05-13 16:05:40.000000 figaro-1.6.5/figaro/_pipelines/hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    23562 2024-05-13 16:05:53.000000 figaro-1.6.5/figaro/_pipelines/par_hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    10988 2024-05-13 16:06:33.000000 figaro-1.6.5/figaro/_pipelines/par_probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     9798 2024-05-13 16:06:51.000000 figaro-1.6.5/figaro/_pipelines/probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2822 2024-05-13 14:47:26.000000 figaro-1.6.5/figaro/cosmology.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.5/figaro/credible_regions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-04-22 12:27:42.000000 figaro-1.6.5/figaro/cumulative.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1364 2024-05-10 09:51:02.000000 figaro-1.6.5/figaro/decorators.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     8460 2024-05-14 11:13:06.000000 figaro-1.6.5/figaro/diagnostic.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.5/figaro/exceptions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    36461 2024-05-14 07:34:00.000000 figaro-1.6.5/figaro/load.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6348 2024-04-16 13:52:44.000000 figaro-1.6.5/figaro/marginal.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    55445 2024-05-14 09:03:30.000000 figaro-1.6.5/figaro/mixture.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.5/figaro/montecarlo.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    40563 2024-04-26 15:09:38.000000 figaro-1.6.5/figaro/plot.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-04-23 20:48:47.000000 figaro-1.6.5/figaro/plot_settings.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    12084 2024-04-24 15:08:47.000000 figaro-1.6.5/figaro/rate.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.5/figaro/transform.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    16046 2024-05-03 13:41:22.000000 figaro-1.6.5/figaro/utils.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:24:22.878258 figaro-1.6.5/figaro.egg-info/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-05-14 11:24:22.000000 figaro-1.6.5/figaro.egg-info/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1809 2024-05-14 11:24:22.000000 figaro-1.6.5/figaro.egg-info/SOURCES.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-05-14 11:24:22.000000 figaro-1.6.5/figaro.egg-info/dependency_links.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-05-14 11:24:22.000000 figaro-1.6.5/figaro.egg-info/entry_points.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-05-14 11:24:22.000000 figaro-1.6.5/figaro.egg-info/requires.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-05-14 11:24:22.000000 figaro-1.6.5/figaro.egg-info/top_level.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-05-14 11:23:57.000000 figaro-1.6.5/pyproject.toml
+-rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-05-14 11:24:22.878842 figaro-1.6.5/setup.cfg
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:24:22.877868 figaro-1.6.5/test/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2577 2024-05-14 09:10:42.000000 figaro-1.6.5/test/test_figaro.py
```

### Comparing `figaro-1.6.4/LICENSE` & `figaro-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/PKG-INFO` & `figaro-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.6.4
+Version: 1.6.5
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `figaro-1.6.4/README.md` & `figaro-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/docs/source/index.rst` & `figaro-1.6.5/docs/source/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -2,27 +2,49 @@
    sphinx-quickstart on Sat Jul 15 21:24:28 2023.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 FIGARO - Fast Inference for GW Astronomy, Research & Observations
 =================================================================
 
-| This page contains the documentation for FIGARO, along with a brief description of how to use it in your research project. Please refer to the `GitHub repository <https://github.com/sterinaldi/FIGARO>`_ for bug reports (extremely appreciated) or issues.
+| This page contains the documentation for FIGARO, along with a brief description of how to use it in your research project. Please refer to the `GitHub repository <https://github.com/sterinaldi/FIGARO>`_ for bug reports (extremely appreciated), issues and contributions.
 | If you're curious about the other projects I'm working on or if you want to get in touch with me, feel free to visit `my website <https://sterinaldi.github.io>`_!
 
+Statement of need
+^^^^^^^^^^^^^^^^^
+| FIGARO is an inference code designed to estimate multivariate probability densities given samples from an unknown distribution using a Dirichlet Process Gaussian Mixture Model (DPGMM) as nonparameteric model, and to perform hierarchical non-parametric inferences: in this case, the model used is (H)DPGMM, described in `Rinaldi & Del Pozzo (2022a) <https://ui.adsabs.harvard.edu/abs/2022MNRAS.509.5454R/abstract>`_.
+| This code, originally developed in the context of black hole population studies using gravitational-wave observations, take as input generic data and therefore it can be applied to a variety of studies beyond gravitational wave populations.
+
+Dependencies
+^^^^^^^^^^^^
+FIGARO has the following dependencies:
+
+* numpy > 1.22
+* scipy
+* matplotlib
+* dill
+* Corner
+* Numba
+* h5py
+* tqdm
+* lalsuite
+* ray
+
 .. toctree::
    :maxdepth: 1
    :caption: Contents:
 
    installation.md
    quickstart.md
-   use_mixture.md
+   use_mixture.ipynb
+   python_script.ipynb
    acknowledgment.md
    api
    figaro
+   
 
 Indices and tables
 ^^^^^^^^^^^^^^^^^^
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `figaro-1.6.4/figaro/_likelihood.py` & `figaro-1.6.5/figaro/_likelihood.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro/_numba_functions.py` & `figaro-1.6.5/figaro/_numba_functions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro/_pipelines/hierarchical_inference.py` & `figaro-1.6.5/figaro/_pipelines/hierarchical_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     parser.add_option("--fraction", dest = "fraction", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
     parser.add_option("--mc_draws", dest = "mc_draws", type = "int", help = "Number of draws for assignment MC integral", default = None)
     parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for LVK sensitivity estimate injections", default = 1.)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options override config options", default = None)
     parser.add_option("--rate", dest = "rate", action = 'store_true', help = "Compute rate", default = False)
     parser.add_option("--include_dvdz", dest = "include_dvdz", action = 'store_true', help = "Include dV/dz*(1+z)^{-1} term in selection effects.", default = False)
+    parser.add_option("-l", "--likelihood", dest = "likelihood", action = 'store_true', help = "Resample posteriors to get likelihood samples (only for GW data)", default = False)
     
     (options, args) = parser.parse_args()
 
     if options.config is not None:
         options = load_options(options, parser)
     # Paths
     if options.input is not None:
@@ -161,18 +162,19 @@
                                                     waveform  = options.wf,
                                                     )
         if np.shape(hier_samples)[-1] == 1:
             hier_samples = hier_samples.flatten()
             
     # Load samples
     events, names = load_data(options.input,
-                              par       = options.par,
-                              n_samples = options.n_samples_dsp,
-                              cosmology = options.cosmology,
-                              waveform  = options.wf,
+                              par        = options.par,
+                              n_samples  = options.n_samples_dsp,
+                              cosmology  = options.cosmology,
+                              waveform   = options.wf,
+                              likelihood = options.likelihood,
                               )
     try:
         dim = np.shape(events[0][0])[-1]
     except IndexError:
         dim = 1
     if options.exclude_points:
         print("Ignoring points outside bounds.")
```

### Comparing `figaro-1.6.4/figaro/_pipelines/par_hierarchical_inference.py` & `figaro-1.6.5/figaro/_pipelines/par_hierarchical_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,15 @@
     parser.add_option("--n_parallel", dest = "n_parallel", type = "int", help = "Number of parallel threads", default = 2)
     parser.add_option("--mc_draws", dest = "mc_draws", type = "int", help = "Number of draws for assignment MC integral", default = None)
     parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for LVK sensitivity estimate injections", default = 1.)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options override config options", default = None)
     parser.add_option("--rate", dest = "rate", action = 'store_true', help = "Compute rate", default = False)
     parser.add_option("--include_dvdz", dest = "include_dvdz", action = 'store_true', help = "Include dV/dz*(1+z)^{-1} term in selection effects.", default = False)
+    parser.add_option("-l", "--likelihood", dest = "likelihood", action = 'store_true', help = "Resample posteriors to get likelihood samples (only for GW data)", default = False)
 
     (options, args) = parser.parse_args()
 
     if options.config is not None:
         options = load_options(options, parser)
     # Paths
     if options.input is not None:
@@ -255,18 +256,19 @@
                                                     cosmology = options.cosmology,
                                                     waveform  = options.wf,
                                                     )
         if np.shape(hier_samples)[-1] == 1:
             hier_samples = hier_samples.flatten()
     # Load samples
     events, names = load_data(options.input,
-                              par       = options.par,
-                              n_samples = options.n_samples_dsp,
-                              cosmology = options.cosmology,
-                              waveform  = options.wf,
+                              par        = options.par,
+                              n_samples  = options.n_samples_dsp,
+                              cosmology  = options.cosmology,
+                              waveform   = options.wf,
+                              likelihood = options.likelihood,
                               )
     try:
         dim = np.shape(events[0][0])[-1]
     except IndexError:
         dim = 1
     if options.exclude_points:
         print("Ignoring points outside bounds.")
```

### Comparing `figaro-1.6.4/figaro/_pipelines/par_probability_density.py` & `figaro-1.6.5/figaro/_pipelines/par_probability_density.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) - single value or n-dim values. If None, it is estimated from samples", default = None)
     parser.add_option("--fraction", dest = "fraction", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
     parser.add_option("--n_parallel", dest = "n_parallel", type = "int", help = "Number of parallel threads", default = 2)
     parser.add_option("--snr_threshold", dest = "snr_threshold", type = "float", help = "SNR threshold for simulated GW datasets", default = None)
     parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for simulated GW datasets", default = None)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options override config options", default = None)
+    parser.add_option("-l", "--likelihood", dest = "likelihood", action = 'store_true', help = "Resample posteriors to get likelihood samples (only for GW data)", default = False)
     
     (options, args) = parser.parse_args()
 
     if options.config is not None:
         options = load_options(options, parser)
     # Paths
     if options.input is not None:
@@ -125,15 +126,23 @@
         print("Ignoring points outside bounds.")
     
     if not options.postprocess:
         ray.init(num_cpus = options.n_parallel)
     
     for i, file in enumerate(files):
         # Load samples
-        samples, name = load_single_event(file, par = options.par, n_samples = options.n_samples_dsp, cosmology = options.cosmology, waveform = options.wf, snr_threshold = options.snr_threshold, far_threshold = options.far_threshold)
+        samples, name = load_single_event(file,
+                                          par           = options.par,
+                                          n_samples     = options.n_samples_dsp,
+                                          cosmology     = options.cosmology,
+                                          waveform      = options.wf,
+                                          snr_threshold = options.snr_threshold,
+                                          far_threshold = options.far_threshold,
+                                          likelihood    = options.likelihood,
+                                          )
         try:
             dim = np.shape(samples)[-1]
         except IndexError:
             dim = 1
         if options.exclude_points:
             samples = samples[np.where((np.prod(options.bounds[:,0] < samples, axis = 1) & np.prod(samples < options.bounds[:,1], axis = 1)))]
         else:
```

### Comparing `figaro-1.6.4/figaro/_pipelines/probability_density.py` & `figaro-1.6.5/figaro/_pipelines/probability_density.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     parser.add_option("--cosmology", type = "choice", dest = "cosmology", help = "Set of cosmological parameters. Default values from Planck (2021)", choices = ['Planck18', 'Planck15'], default = 'Planck18')
     parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) - single value or n-dim values. If None, it is estimated from samples", default = None)
     parser.add_option("--fraction", dest = "fraction", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
     parser.add_option("--snr_threshold", dest = "snr_threshold", type = "float", help = "SNR threshold for simulated GW datasets", default = None)
     parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for simulated GW datasets", default = None)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options override config options", default = None)
+    parser.add_option("-l", "--likelihood", dest = "likelihood", action = 'store_true', help = "Resample posteriors to get likelihood samples (only for GW data)", default = False)
     
     (options, args) = parser.parse_args()
 
     if options.config is not None:
         options = load_options(options, parser)
     # Paths
     if options.input is not None:
@@ -101,15 +102,23 @@
             output_draws.mkdir()
         subfolder = True
     if options.exclude_points:
         print("Ignoring points outside bounds.")
     
     for i, file in enumerate(files):
         # Load samples
-        samples, name = load_single_event(file, par = options.par, n_samples = options.n_samples_dsp, cosmology = options.cosmology, waveform = options.wf, snr_threshold = options.snr_threshold, far_threshold = options.far_threshold)
+        samples, name = load_single_event(file,
+                                          par           = options.par,
+                                          n_samples     = options.n_samples_dsp,
+                                          cosmology     = options.cosmology,
+                                          waveform      = options.wf,
+                                          snr_threshold = options.snr_threshold,
+                                          far_threshold = options.far_threshold,
+                                          likelihood    = options.likelihood,
+                                          )
         try:
             dim = np.shape(samples)[-1]
         except IndexError:
             dim = 1
         if options.exclude_points:
             samples = samples[np.where((np.prod(options.bounds[:,0] < samples, axis = 1) & np.prod(samples < options.bounds[:,1], axis = 1)))]
         else:
```

### Comparing `figaro-1.6.4/figaro/cosmology.py` & `figaro-1.6.5/figaro/cosmology.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,16 @@
             def objective(z, self, DL):
                 return DL - self.LuminosityDistance(z)
             return newton(objective,1.0,args=(self, DL))
 
 Planck18 = CosmologicalParameters(0.674, 0.315, 0.685, -1, 0, 0)
 Planck15 = CosmologicalParameters(0.679, 0.3065, 0.6935, -1, 0, 0)
 
-# Interpolants up to z = 2
-z = np.linspace(0,2,1000)
+# Interpolants up to z = 2.5
+z = np.linspace(0,2.5,1000)
 dVdz_approx_planck18 = interp1d(z, Planck18.ComovingVolumeElement(z)/1e9) # In Gpc
 dVdz_approx_planck15 = interp1d(z, Planck15.ComovingVolumeElement(z)/1e9) # In Gpc
 
 def _decorator_dVdz(func, approx, z_index, z_max):
     reg_const = (1+z_max)/approx(z_max)
     def decorated_func(x):
         return func(x)*approx(x[:,z_index])/(1+x[:,z_index]) * reg_const
```

### Comparing `figaro-1.6.4/figaro/credible_regions.py` & `figaro-1.6.5/figaro/credible_regions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro/cumulative.py` & `figaro-1.6.5/figaro/cumulative.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro/decorators.py` & `figaro-1.6.5/figaro/decorators.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 
 def antiprobit(func):
     """
     Transform a point x from probit space to natural space and returns the function evaluated at the natural point y
     """
     def f_transf(ref, x, *args, **kwargs):
         if not ref.probit:
-            return func(ref, x, *args)
+            return func(ref, x, *args, **kwargs)
         y = transform_from_probit(x, ref.bounds)
-        return func(ref, y, *args)
+        return func(ref, y, *args, **kwargs)
     return f_transf
 
 def probit(func):
     """
     Transform a point x from natural space to probit space and returns the function evaluated at the probit point y
     """
     def f_transf(ref, x, *args, **kwargs):
         if not ref.probit:
-            return func(ref, x, *args)
+            return func(ref, x, *args, **kwargs)
         y = transform_to_probit(x, ref.bounds)
-        return func(ref, y, *args)
+        return func(ref, y, *args, **kwargs)
     return f_transf
 
 def from_probit(func):
     """
     Evaluate a function that samples points in probit space and return these points after transforming them to natural space
     """
     def f_transf(ref, *args, **kwargs):
         if not ref.probit:
-            return func(ref, *args)
-        y = func(ref, *args)
+            return func(ref, *args, **kwargs)
+        y = func(ref, *args, **kwargs)
         return transform_from_probit(y, ref.bounds)
     return f_transf
```

### Comparing `figaro-1.6.4/figaro/diagnostic.py` & `figaro-1.6.5/figaro/diagnostic.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro/exceptions.py` & `figaro-1.6.5/figaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro/load.py` & `figaro-1.6.5/figaro/load.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import warnings
 import json
 import dill
 import copy
 import importlib
 from figaro.exceptions import FIGAROException
 from figaro.mixture import mixture
-from figaro.cosmology import Planck18, Planck15
+from figaro.cosmology import Planck18, Planck15, dVdz_approx_planck18, dVdz_approx_planck15
 from pathlib import Path
 from tqdm import tqdm
 
 supported_extensions = ['h5', 'hdf5', 'txt', 'dat', 'csv']
 supported_waveforms  = ['combined', 'imr', 'seob']
 injected_pars        = ['m1', 'm2', 'z', 's1x', 's1y', 's1z', 's2x', 's2y', 's2z', 'ra', 'dec']
 loadable_inj_pars    = injected_pars + ['q', 'chi_eff', 'chi_p', 's1', 's2']
@@ -73,15 +73,15 @@
 
 def available_gw_pars():
     """
     Print a list of available GW parameters
     """
     print(supported_pars)
 
-def load_single_event(event, seed = False, par = None, n_samples = -1, cosmology = 'Planck18', volume = False, waveform = 'combined', snr_threshold = None, far_threshold = None):
+def load_single_event(event, seed = False, par = None, n_samples = -1, cosmology = 'Planck18', volume = False, waveform = 'combined', snr_threshold = None, far_threshold = None, likelihood = False):
     '''
     Loads the data from .txt/.dat files (for simulations) or .h5/.hdf5 files (posteriors from GWTC) for a single event.
     Default cosmological parameters from Planck Collaboration (2021) in a flat Universe (https://www.aanda.org/articles/aa/pdf/2020/09/aa33910-18.pdf)
     Not all GW parameters are implemented: run figaro.load.available_gw_pars() for a list of the available parameters.
     
     Arguments:
         str or Path file:     file with samples
@@ -89,14 +89,15 @@
         list-of-str par:      list with parameter(s) to extract from GW posteriors (m1, m2, mc, z, chi_effective)
         int n_samples:        number of samples for (random) downsampling. Default -1: all samples
         str cosmology:        set of cosmological parameters (Planck18 or Planck15)
         bool volume:          if True, loads RA, dec and Luminosity distance (for skymaps)
         str waveform:         waveform family to be used ('combined', 'seob', 'imr')
         double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
         double far_threshold: FAR threshold for event filtering. For injection analysis only.
+        bool likelihood:      resample to get likelihood samples
         
     Returns:
         np.ndarray: samples
         np.ndarray: name
     '''
     if seed:
         rdstate = np.random.RandomState(seed = 1)
@@ -123,24 +124,24 @@
             raise TypeError("Please provide a list of parameter names you want to load (e.g. ['m1']).")
         # Check that all the parametes are loadable
         if not np.all([p in GW_par.keys() for p in par]):
             wrong_pars = [p for p in par if not p in GW_par.keys()]
             raise FIGAROException("The following parameters are not implemented: "+", ".join(wrong_pars)+". Run figaro.load.available_gw_pars() for a list of available parameters.")
         # If everything is ok, load the samples
         else:
-            out = _unpack_gw_posterior(event, par = par, n_samples = n_samples, cosmology = cosmology, rdstate = rdstate, waveform = waveform, snr_threshold = snr_threshold, far_threshold = far_threshold)
+            out = _unpack_gw_posterior(event, par = par, n_samples = n_samples, cosmology = cosmology, rdstate = rdstate, waveform = waveform, snr_threshold = snr_threshold, far_threshold = far_threshold, likelihood = likelihood)
     
     if out is None:
         return out, name
     
     if len(np.shape(out)) == 1:
         out = np.atleast_2d(out).T
     return out, name
 
-def load_data(path, seed = False, par = None, n_samples = -1, cosmology = 'Planck18', volume = False, waveform = 'combined', snr_threshold = None, far_threshold = None, verbose = True):
+def load_data(path, seed = False, par = None, n_samples = -1, cosmology = 'Planck18', volume = False, waveform = 'combined', snr_threshold = None, far_threshold = None, verbose = True, likelihood = False):
     '''
     Loads the data from .txt files (for simulations) or .h5/.hdf5/.dat files (posteriors from GWTC-x).
     Default cosmological parameters from Planck Collaboration (2021) in a flat Universe (https://www.aanda.org/articles/aa/pdf/2020/09/aa33910-18.pdf)
     Not all GW parameters are implemented: run figaro.load.available_gw_pars() for a list of available parameters.
     
     Arguments:
         str or Path path:     folder with data files
@@ -148,14 +149,15 @@
         list-of-str par:      list with parameter(s) to extract from GW posteriors
         int n_samples:        number of samples for (random) downsampling. Default -1: all samples
         str cosmology:        set of cosmological parameters (Planck18 or Planck15)
         str waveform:         waveform family to be used ('combined', 'seob', 'imr')
         double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
         double far_threshold: FAR threshold for event filtering. For injection analysis only.
         bool verbose:         show progress bar
+        bool likelihood:      resample to get likelihood samples
 
     Returns:
         np.ndarray: samples
         np.ndarray: names
     '''
     folder      = Path(path).resolve()
     event_files = [Path(folder,f) for f in folder.glob('[!.]*')] # Ignores hidden files
@@ -199,28 +201,28 @@
                 raise TypeError("Please provide a list of parameter names you want to load (e.g. ['m1']).")
             # Check that all the parametes are loadable
             if not np.all([p in GW_par.keys() for p in par]):
                 wrong_pars = [p for p in par if not p in GW_par.keys()]
                 raise FIGAROException("The following parameters are not implemented: "+", ".join(wrong_pars)+". Run figaro.load.available_gw_pars() for a list of available parameters.")
             # If everything is ok, load the samples
             else:
-                out = _unpack_gw_posterior(event, par = par, n_samples = n_samples, cosmology = cosmology, rdstate = rdstate, waveform = waveform, snr_threshold = snr_threshold, far_threshold = far_threshold)
+                out = _unpack_gw_posterior(event, par = par, n_samples = n_samples, cosmology = cosmology, rdstate = rdstate, waveform = waveform, snr_threshold = snr_threshold, far_threshold = far_threshold, likelihood = likelihood)
                 if out is not None:
                     if out.shape[-1] == len(par):
                         events.append(out)
                     elif 'snr' in par:
                         removed_snr = True
                         names.remove(name)
                 else:
                     names.remove(name)
     if removed_snr:
         warnings.warn("At least one event does not have SNR samples. These events cannot be loaded for this parameter choices.")
     return (events, np.array(names))
 
-def _unpack_gw_posterior(event, par, cosmology, rdstate, n_samples = -1, waveform = 'combined', snr_threshold = None, far_threshold = None):
+def _unpack_gw_posterior(event, par, cosmology, rdstate, n_samples = -1, waveform = 'combined', snr_threshold = None, far_threshold = None, likelihood = False):
     '''
     Reads data from .h5/.hdf5 GW posterior files.
     For GWTC-3 data release, it uses by default the Mixed posterior samples.
     Not all parameters are implemented: run figaro.load.available_gw_pars() for a list of available parameters.
     The waveform argument allows the user to select a waveform family. The default value, 'combined' uses samples from both imr and seob waveforms.
     For SEOB waveforms, the following waveform models are used (in descending priority order):
         * SEOBNRv4PHM
@@ -228,21 +230,23 @@
         * SEOBNRv4
     For IMR waveforms, in descending order:
         * IMRPhenomXPHM
         * IMRPhenomPv2
         * IMRPhenomPv3HM
     
     Arguments:
-        str event:            file to read
-        str par:              parameter to extract
-        tuple cosmology:      cosmological parameters (h, om, ol)
-        int n_samples:        number of samples for (random) downsampling. Default -1: all samples
-        str waveform:         waveform family to be used ('combined', 'imr', 'seob')
-        double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
-        double far_threshold: FAR threshold for event filtering. For injection analysis only.
+        str event:                 file to read
+        list-of-str par:           parameter to extract
+        str cosmology:             set of cosmological parameters to use.
+        np.random.rdstate rdstate: state for random number generation
+        int n_samples:             number of samples for (random) downsampling. Default -1: all samples
+        str waveform:              waveform family to be used ('combined', 'imr', 'seob')
+        double snr_threhsold:      SNR threshold for event filtering. For injection analysis only.
+        double far_threshold:      FAR threshold for event filtering. For injection analysis only.
+        bool likelihood:           resample to get likelihood samples
     
     Returns:
         np.ndarray: samples
     '''
     if cosmology == 'Planck18':
         omega = Planck18
     elif cosmology == 'Planck15':
@@ -395,14 +399,18 @@
                 samples = np.array(samples)
                 if flag_filter:
                     if far_threshold is not None:
                         samples = samples[:, np.where((far < far_threshold) & (far > 0))[0]]
                     if snr_threshold is not None:
                         samples = samples[:, np.where(snr > snr_threshold)[0]]
                 samples = samples.T
+            if likelihood:
+                inv_prior = 1./_prior_gw(par, data, cosmology)
+                h         = np.random.uniform(0,1, len(samples))
+                samples   = samples[h < inv_prior/np.max(inv_prior)]
             if n_samples > -1:
                 s = int(min([n_samples, len(samples)]))
                 return samples[rdstate.choice(np.arange(len(samples)), size = s, replace = False)]
             else:
                 return samples
 
         # GWTC-1
@@ -464,20 +472,59 @@
                 samples_loaded = np.array(samples)
                 samples = []
                 for pi in par:
                     if not (pi == 'snr' or pi == 'far'):
                         samples.append(samples_loaded[np.where(loaded_pars == pi)[0]].flatten())
                 samples = np.array(samples)
                 samples = samples.T
+            if likelihood:
+                inv_prior = 1./_prior_gw(par, ss, cosmology)
+                h         = np.random.uniform(0,1, len(samples))
+                samples   = samples[h < inv_prior/np.max(inv_prior)]
             if n_samples > -1:
                 s = int(min([n_samples, len(samples)]))
                 return samples[rdstate.choice(np.arange(len(samples)), size = s, replace = False)]
             else:
                 return samples
 
+def _prior_gw(par, samples, cosmology = 'Planck18'):
+    """
+    GW prior parameters, following https://docs.ligo.org/RatesAndPopulations/gwpopulation_pipe/_modules/gwpopulation_pipe/data_collection.html#evaluate_prior
+    
+    Arguments:
+        np.ndarray samples: posterior samples
+        list-of-str par:    parameter(s)
+        str cosmology:      cosmological parameters.
+    
+    Returns:
+        np.ndarray: prior values
+    """
+    if cosmology == 'Planck18':
+        omega = Planck18
+        dVdz  = dVdz_approx_planck18
+    elif cosmology == 'Planck15':
+        omega = Planck15
+        dVdz  = dVdz_approx_planck15
+    else:
+        raise FIGAROException("Cosmology not supported")
+    vol   = omega.ComovingVolume(2.5)/1e9
+    prior = np.ones(len(samples))
+    # Redshift prior (uniform in comoving source frame)
+    if 'z' in par:
+        prior *= dVdz(samples[GW_par['z']])/((1.+samples[GW_par['z']])*vol)
+    # Mass prior (uniform in detector-frame component masses)
+    n_mass_pars = np.sum([item in par for item in ['m1','m2','mc','q']])
+    if n_mass_pars > 0:
+        prior *= (1+samples[GW_par['z']])**np.min([n_mass_pars, 2])
+    if 'q' in par:
+        prior *= samples[GW_par['m1']]
+    if ('mc' in par or 'mc_detect' in par):
+        prior *= (1 + samples[GW_par['q']]) ** 0.2 / samples[GW_par['q']] ** 0.6
+    return prior
+    
 def save_density(draws, folder = '.', name = 'density', ext = 'json'):
     """
     Exports a list of figaro.mixture instances to file
 
     Arguments:
         list draws:         list of mixtures to be saved
         str or Path folder: folder in which the output file will be saved
```

### Comparing `figaro-1.6.4/figaro/marginal.py` & `figaro-1.6.5/figaro/marginal.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro/mixture.py` & `figaro-1.6.5/figaro/mixture.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,28 +546,28 @@
         
         Arguments:
             np.ndarray x: point(s) to evaluate the mixture at
         
         Returns:
             np.ndarray: mixture.cdf(x)
         """
-        return np.sum(np.array([w*norm(mean[0], cov[0,0]).cdf(x) for mean, cov, w in zip(self.means, np.sqrt(self.covs), self.w)]), axis = 0)
+        return np.sum(np.array([w*norm(mean[0], cov[0,0]).cdf(x) for mean, cov, w in zip(self.means, np.sqrt(self.covs), self.w)]), axis = 0).flatten()
 
     @probit
     def _logcdf(self, x):
         """
         Evaluate mixture log cdf at point(s) x
         
         Arguments:
             np.ndarray x: point(s) to evaluate the mixture at
         
         Returns:
             np.ndarray: mixture.logcdf(x)
         """
-        return logsumexp(np.array([w + norm(mean[0], cov[0,0]).logcdf(x) for mean, cov, w in zip(self.means, np.sqrt(self.covs), self.log_w)]), axis = 0)
+        return logsumexp(np.array([w + norm(mean[0], cov[0,0]).logcdf(x) for mean, cov, w in zip(self.means, np.sqrt(self.covs), self.log_w)]), axis = 0).flatten()
 
     @from_probit
     def rvs(self, size = 1):
         """
         Draw samples from mixture
         
         Arguments:
@@ -575,15 +575,15 @@
         
         Returns:
             np.ndarray: samples
         """
         if self.n_cl == 0:
             raise FIGAROException("You are trying to draw samples from an empty mixture.\n If you are using the density_from_samples() method, you may want to draw samples from the output of that method.")
         return self._rvs_probit(size)
-        
+    
     def _rvs_probit(self, size = 1):
         """
         Draw samples from mixture in probit space
         
         Arguments:
             int size: number of samples to draw
```

### Comparing `figaro-1.6.4/figaro/montecarlo.py` & `figaro-1.6.5/figaro/montecarlo.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro/plot.py` & `figaro-1.6.5/figaro/plot.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro/plot_settings.py` & `figaro-1.6.5/figaro/plot_settings.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro/rate.py` & `figaro-1.6.5/figaro/rate.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro/transform.py` & `figaro-1.6.5/figaro/transform.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro/utils.py` & `figaro-1.6.5/figaro/utils.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.4/figaro.egg-info/PKG-INFO` & `figaro-1.6.5/figaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.6.4
+Version: 1.6.5
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `figaro-1.6.4/figaro.egg-info/SOURCES.txt` & `figaro-1.6.5/figaro.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,8 +54,9 @@
 figaro.egg-info/entry_points.txt
 figaro.egg-info/requires.txt
 figaro.egg-info/top_level.txt
 figaro/_pipelines/__init__.py
 figaro/_pipelines/hierarchical_inference.py
 figaro/_pipelines/par_hierarchical_inference.py
 figaro/_pipelines/par_probability_density.py
-figaro/_pipelines/probability_density.py
+figaro/_pipelines/probability_density.py
+test/test_figaro.py
```

### Comparing `figaro-1.6.4/pyproject.toml` & `figaro-1.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.setuptools]
 packages = ['figaro', 'figaro._pipelines']
 
 [project]
 name = 'figaro'
 description = 'FIGARO: Fast Inference for GW Astronomy, Research & Observations'
-version = '1.6.4'
+version = '1.6.5'
 requires-python = '< 3.12'
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ['DPGMM', 'figaro', 'hierarchical', 'inference', 'HDPGMM']
 authors = [
   {name = "Stefano Rinaldi", email = "stefano.rinaldi@uni-heidelberg.de"},
   {name = "Walter Del Pozzo", email = "walter.delpozzo@unipi.it"},
```

