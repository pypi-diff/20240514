# Comparing `tmp/starsim-0.3.4.tar.gz` & `tmp/starsim-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starsim-0.3.4.tar", last modified: Thu Apr 18 08:31:58 2024, max compression
+gzip compressed data, was "starsim-0.5.0.tar", last modified: Tue May 14 13:51:49 2024, max compression
```

## Comparing `starsim-0.3.4.tar` & `starsim-0.5.0.tar`

### file list

```diff
@@ -1,54 +1,60 @@
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 08:31:58.843789 starsim-0.3.4/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1088 2024-03-30 07:25:13.000000 starsim-0.3.4/LICENSE
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3619 2024-04-18 08:31:58.843789 starsim-0.3.4/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2714 2024-04-18 06:06:16.000000 starsim-0.3.4/README.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2024-04-18 08:31:58.843789 starsim-0.3.4/setup.cfg
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1619 2024-04-03 13:56:26.000000 starsim-0.3.4/setup.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 08:31:58.839789 starsim-0.3.4/starsim/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1046 2024-04-13 20:12:05.000000 starsim-0.3.4/starsim/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1191 2024-04-13 20:12:05.000000 starsim-0.3.4/starsim/connectors.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       37 2024-04-13 20:12:05.000000 starsim-0.3.4/starsim/demo.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19988 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/demographics.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    16370 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/disease.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 08:31:58.843789 starsim-0.3.4/starsim/diseases/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      285 2024-04-13 20:12:07.000000 starsim-0.3.4/starsim/diseases/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8863 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/diseases/cholera.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5839 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/ebola.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3385 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/gonorrhea.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4668 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/hiv.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3283 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/measles.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3423 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/ncd.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5895 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/sir.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14752 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/diseases/syphilis.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    29246 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/distributions.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22026 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/interventions.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6688 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/modules.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    33433 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/network.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3979 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/parameters.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15132 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/people.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5869 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/products.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2080 2024-04-13 20:12:05.000000 starsim-0.3.4/starsim/results.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15346 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/run.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13972 2024-04-13 20:12:05.000000 starsim-0.3.4/starsim/samples.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7750 2024-04-18 05:47:32.000000 starsim-0.3.4/starsim/settings.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    45922 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/sim.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    24451 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/states.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13010 2024-04-17 05:34:13.000000 starsim-0.3.4/starsim/utils.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      239 2024-04-18 06:07:15.000000 starsim-0.3.4/starsim/version.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 08:31:58.843789 starsim-0.3.4/starsim.egg-info/
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)     3619 2024-04-18 08:31:58.000000 starsim-0.3.4/starsim.egg-info/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1030 2024-04-18 08:31:58.000000 starsim-0.3.4/starsim.egg-info/SOURCES.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2024-04-18 08:31:58.000000 starsim-0.3.4/starsim.egg-info/dependency_links.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       66 2024-04-18 08:31:58.000000 starsim-0.3.4/starsim.egg-info/requires.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        8 2024-04-18 08:31:58.000000 starsim-0.3.4/starsim.egg-info/top_level.txt
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-18 08:31:58.843789 starsim-0.3.4/tests/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3358 2024-04-18 05:47:32.000000 starsim-0.3.4/tests/test_base.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5666 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_baselines.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      973 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_dcp.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5702 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_demographics.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3274 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_diseases.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7721 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_dist.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5914 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_dists.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1420 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_samples.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5576 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_simple.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6159 2024-04-13 20:12:03.000000 starsim-0.3.4/tests/test_syphilis.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-05-14 13:51:49.821274 starsim-0.5.0/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1088 2024-03-30 07:25:13.000000 starsim-0.5.0/LICENSE
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3619 2024-05-14 13:51:49.821274 starsim-0.5.0/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2714 2024-04-19 05:58:15.000000 starsim-0.5.0/README.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2024-05-14 13:51:49.821274 starsim-0.5.0/setup.cfg
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1619 2024-04-03 13:56:26.000000 starsim-0.5.0/setup.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-05-14 13:51:49.821274 starsim-0.5.0/starsim/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1017 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       37 2024-05-06 03:47:36.000000 starsim-0.5.0/starsim/demo.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    20147 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/demographics.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15578 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/disease.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-05-14 13:51:49.821274 starsim-0.5.0/starsim/diseases/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      285 2024-05-06 03:47:27.000000 starsim-0.5.0/starsim/diseases/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8440 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/diseases/cholera.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5430 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/diseases/ebola.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3027 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/diseases/gonorrhea.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4287 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/diseases/hiv.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3126 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/diseases/measles.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3226 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/diseases/ncd.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5564 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/diseases/sir.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14383 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/diseases/syphilis.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    32460 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/distributions.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22474 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/interventions.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8719 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/modules.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    30557 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/network.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    18854 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/parameters.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13057 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/people.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6123 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/products.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2086 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/results.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15362 2024-05-06 03:47:36.000000 starsim-0.5.0/starsim/run.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13998 2024-05-06 03:47:36.000000 starsim-0.5.0/starsim/samples.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7552 2024-05-06 03:47:36.000000 starsim-0.5.0/starsim/settings.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    33629 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/sim.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    16124 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/states.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      857 2024-05-09 04:41:14.000000 starsim-0.5.0/starsim/untitled0.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1165 2024-05-06 03:47:36.000000 starsim-0.5.0/starsim/untitled13.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1501 2024-05-06 03:47:36.000000 starsim-0.5.0/starsim/untitled14.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1588 2024-05-06 03:47:36.000000 starsim-0.5.0/starsim/untitled16.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1654 2024-05-06 03:47:36.000000 starsim-0.5.0/starsim/untitled17.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      786 2024-05-11 23:02:25.000000 starsim-0.5.0/starsim/untitled5.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       75 2024-05-11 21:31:45.000000 starsim-0.5.0/starsim/untitled8.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    10204 2024-05-14 13:50:27.000000 starsim-0.5.0/starsim/utils.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      239 2024-05-14 13:51:13.000000 starsim-0.5.0/starsim/version.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-05-14 13:51:49.821274 starsim-0.5.0/starsim.egg-info/
+-rw-r--r--   0 cliffk    (1000) cliffk    (1000)     3619 2024-05-14 13:51:49.000000 starsim-0.5.0/starsim.egg-info/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1166 2024-05-14 13:51:49.000000 starsim-0.5.0/starsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2024-05-14 13:51:49.000000 starsim-0.5.0/starsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       66 2024-05-14 13:51:49.000000 starsim-0.5.0/starsim.egg-info/requires.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        8 2024-05-14 13:51:49.000000 starsim-0.5.0/starsim.egg-info/top_level.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-05-14 13:51:49.821274 starsim-0.5.0/tests/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5675 2024-05-14 13:50:27.000000 starsim-0.5.0/tests/test_baselines.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7429 2024-05-14 13:50:27.000000 starsim-0.5.0/tests/test_demographics.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5475 2024-05-14 13:50:27.000000 starsim-0.5.0/tests/test_diseases.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8115 2024-05-14 13:50:27.000000 starsim-0.5.0/tests/test_dist.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5278 2024-05-14 13:50:27.000000 starsim-0.5.0/tests/test_other.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5664 2024-05-14 13:50:27.000000 starsim-0.5.0/tests/test_plugins.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8325 2024-05-14 13:50:27.000000 starsim-0.5.0/tests/test_randomness.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1420 2024-04-13 20:12:03.000000 starsim-0.5.0/tests/test_samples.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9629 2024-05-14 13:50:27.000000 starsim-0.5.0/tests/test_sim.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6168 2024-05-01 15:26:23.000000 starsim-0.5.0/tests/test_syphilis.py
```

### Comparing `starsim-0.3.4/LICENSE` & `starsim-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starsim-0.3.4/PKG-INFO` & `starsim-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starsim
-Version: 0.3.4
+Version: 0.5.0
 Summary: Starsim
 Author: Robyn Stuart, Cliff Kerr, Romesh Abeysuriya, Paula Sanz-Leon, Jamie Cohen, and Daniel Klein on behalf of the Starsim Collective
 Keywords: agent-based model,simulation,disease,epidemiology
 Platform: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
```

### Comparing `starsim-0.3.4/README.rst` & `starsim-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `starsim-0.3.4/setup.py` & `starsim-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.4/starsim/__init__.py` & `starsim-0.5.0/starsim/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from .version import __version__, __versiondate__, __license__
 from .settings      import *
-from .parameters    import *
 from .utils         import *
+from .parameters    import *
 from .distributions import *
 from .states        import *
 from .people        import *
 from .modules       import *
 from .network       import *
 from .results       import *
 from .demographics  import *
 from .products      import *
 from .interventions import *
 from .demographics  import *
-from .connectors    import *
 from .disease       import *
 from .diseases      import *
 from .sim           import *
 from .run           import *
 from .samples       import *
 
 # Assign the root folder
```

### Comparing `starsim-0.3.4/starsim/demographics.py` & `starsim-0.5.0/starsim/demographics.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,113 +7,124 @@
 import sciris as sc
 import pandas as pd
 
 __all__ = ['Demographics', 'Births', 'Deaths', 'Pregnancy']
 
 
 class Demographics(ss.Module):
-    # A demographic module typically handles births/deaths/migration and takes
-    # place at the start of the timestep, before networks are updated and before
-    # any disease modules are executed
-
+    """
+    A demographic module typically handles births/deaths/migration and takes
+    place at the start of the timestep, before networks are updated and before
+    any disease modules are executed.
+    """
     def initialize(self, sim):
         super().initialize(sim)
-        self.init_results(sim)
+        self.init_results()
         return
 
-    def init_results(self, sim):
+    def init_results(self):
+        pass
+
+    def update(self):
         pass
 
-    def update(self, sim):
-        # Note that for demographic modules, any result updates should be
-        # carried out inside this function
+    def update_results(self):
         pass
 
 
 class Births(Demographics):
+    """ Create births based on rates, rather than based on pregnancy """
     def __init__(self, pars=None, metadata=None, **kwargs):
-        super().__init__(pars, **kwargs)
-
-        # Set defaults
-        self.pars = ss.omergeleft(self.pars,
+        super().__init__()
+        self.default_pars(
             birth_rate = 0,
             rel_birth = 1,
             units = 1e-3,  # assumes birth rates are per 1000. If using percentages, switch this to 1
         )
+        self.update_pars(pars, **kwargs)
 
         # Process metadata. Defaults here are the labels used by UN data
-        self.metadata = ss.omergeleft(metadata,
-            data_cols = dict(year='Year', cbr='CBR'),
+        self.metadata = sc.mergedicts(
+            sc.objdict(data_cols=dict(year='Year', cbr='CBR')),
+            metadata,
         )
 
         # Process data, which may be provided as a number, dict, dataframe, or series
         # If it's a number it's left as-is; otherwise it's converted to a dataframe
         self.pars.birth_rate = self.standardize_birth_data()
+        self.n_births = 0 # For results tracking
         return
 
     def initialize(self, sim):
         """ Initialize with sim information """
         super().initialize(sim)
         if isinstance(self.pars.birth_rate, pd.DataFrame):
             br_year = self.pars.birth_rate[self.metadata.data_cols['year']]
             br_val = self.pars.birth_rate[self.metadata.data_cols['cbr']]
             all_birth_rates = np.interp(sim.yearvec, br_year, br_val)
             self.pars.birth_rate = all_birth_rates
+        return
 
     def standardize_birth_data(self):
         """ Standardize/validate birth rates - handled in an external file due to shared functionality """
         birth_rate = ss.standardize_data(data=self.pars.birth_rate, metadata=self.metadata)
         return birth_rate
 
-    def init_results(self, sim):
+    def init_results(self):
+        npts = self.sim.npts
         self.results += [
-            ss.Result(self.name, 'new', sim.npts, dtype=int, scale=True),
-            ss.Result(self.name, 'cumulative', sim.npts, dtype=int, scale=True),
-            ss.Result(self.name, 'cbr', sim.npts, dtype=int, scale=False),
+            ss.Result(self.name, 'new', npts, dtype=int, scale=True),
+            ss.Result(self.name, 'cumulative', npts, dtype=int, scale=True),
+            ss.Result(self.name, 'cbr', npts, dtype=int, scale=False),
         ]
         return
 
-    def update(self, sim):
-        new_uids = self.add_births(sim)
-        self.update_results(len(new_uids), sim)
+    def update(self):
+        new_uids = self.add_births()
+        self.n_births = len(new_uids)
         return new_uids
 
-    def get_births(self, sim):
+    def get_births(self):
         """
         Extract the right birth rates to use and translate it into a number of people to add.
         """
+        sim = self.sim
         p = self.pars
         if sc.isnumber(p.birth_rate):
             this_birth_rate = p.birth_rate
         elif sc.checktype(p.birth_rate, 'arraylike'):
             this_birth_rate = p.birth_rate[sim.ti]
 
         scaled_birth_prob = this_birth_rate * p.units * p.rel_birth * sim.pars.dt
         scaled_birth_prob = np.clip(scaled_birth_prob, a_min=0, a_max=1)
         n_new = int(np.floor(sim.people.alive.count() * scaled_birth_prob))
         return n_new
 
-    def add_births(self, sim):
-        # Add n_new births to each state in the sim
-        n_new = self.get_births(sim)
-        new_uids = sim.people.grow(n_new)
-        sim.people.age[new_uids] = 0
+    def add_births(self):
+        """ Add n_new births to each state in the sim """
+        people = self.sim.people
+        n_new = self.get_births()
+        new_uids = people.grow(n_new)
+        people.age[new_uids] = 0
         return new_uids
 
-    def update_results(self, n_new, sim):
-        self.results['new'][sim.ti] = n_new
+    def update_results(self):
+        self.results['new'][self.sim.ti] = self.n_births
+        return
 
-    def finalize(self, sim):
-        super().finalize(sim)
-        self.results['cumulative'] = np.cumsum(self.results['new'])
-        self.results['cbr'] = 1/self.pars.units*np.divide(self.results['new'] / sim.dt, sim.results['n_alive'], where=sim.results['n_alive']>0)
+    def finalize(self):
+        super().finalize()
+        res = self.sim.results
+        self.results.cumulative = np.cumsum(self.results.new)
+        self.results.cbr = 1/self.pars.units*np.divide(self.results.new/self.sim.dt, res.n_alive, where=res.n_alive>0)
+        return
 
 
 class Deaths(Demographics):
-    def __init__(self, pars=None, par_dists=None, metadata=None, **kwargs):
+    def __init__(self, pars=None, metadata=None, **kwargs):
         """
         Configure disease-independent "background" deaths.
 
         The probability of death for each agent on each timestep is determined
         by the `death_rate` parameter and the time step. The default value of
         this parameter is 0.02, indicating that all agents will
         face a 2% chance of death per year.
@@ -129,343 +140,341 @@
 
         Args:
             pars: dict with arguments including:
                 rel_death: constant used to scale all death rates
                 death_rate: float, dict, or pandas dataframe/series containing mortality data
                 units: units for death rates (see in-line comment on par dict below)
 
-            par_dists: dict
-
             metadata: data about the data contained within the data input.
                 "data_cols" is is a dictionary mapping standard keys, like "year" to the
                 corresponding column name in data. Similar for "sex_keys". Finally,
         """
-        super().__init__(pars, **kwargs)
-
-        self.pars = ss.omergeleft(self.pars,
+        super().__init__()
+        self.default_pars(
             rel_death = 1,
             death_rate = 20,  # Default = a fixed rate of 2%/year, overwritten if data provided
             units = 1e-3,  # assumes death rates are per 1000. If using percentages, switch this to 1
         )
-
-        self.par_dists = ss.omergeleft(par_dists,
-            death_rate = ss.bernoulli
-        )
+        self.update_pars(pars, **kwargs)
 
         # Process metadata. Defaults here are the labels used by UN data
-        self.metadata = ss.omergeleft(metadata,
-            data_cols = dict(year='Time', sex='Sex', age='AgeGrpStart', value='mx'),
-            sex_keys = dict(f='Female', m='Male'),
+        self.metadata = sc.mergedicts(
+            sc.objdict(
+                data_cols = dict(year='Time', sex='Sex', age='AgeGrpStart', value='mx'),
+                sex_keys = dict(f='Female', m='Male'),
+            ),
+            metadata
         )
 
         # Process data, which may be provided as a number, dict, dataframe, or series
         # If it's a number it's left as-is; otherwise it's converted to a dataframe
-        self.death_rate_data = self.standardize_death_data()
-        self.pars.death_rate = self.make_death_prob_fn
-
+        self.death_rate_data = self.standardize_death_data() # TODO: refactor
+        self.pars.death_rate = ss.bernoulli(p=self.make_death_prob_fn)
+        self.n_deaths = 0 # For results tracking
         return
+    
+    def standardize_death_data(self):
+        """ Standardize/validate death rates - handled in an external file due to shared functionality """
+        death_rate = ss.standardize_data(data=self.pars.death_rate, metadata=self.metadata)
+        return death_rate
 
-    @staticmethod
-    def make_death_prob_fn(module, sim, uids):
+    @staticmethod # Needs to be static since called externally, although it sure looks like a class method!
+    def make_death_prob_fn(self, sim, uids):
         """ Take in the module, sim, and uids, and return the probability of death for each UID on this timestep """
 
-        if sc.isnumber(module.death_rate_data):
-            death_rate = module.death_rate_data
+        drd = self.death_rate_data
+        if sc.isnumber(drd) or isinstance(drd, ss.Dist):
+            death_rate = drd
 
         else:
-            data_cols = sc.objdict(module.metadata.data_cols)
+            ppl = sim.people
+            data_cols = sc.objdict(self.metadata.data_cols)
             year_label = data_cols.year
             age_label  = data_cols.age
             sex_label  = data_cols.sex
             val_label  = data_cols.value
-            sex_keys = module.metadata.sex_keys
+            sex_keys = self.metadata.sex_keys
 
-            available_years = module.death_rate_data[year_label].unique()
+            available_years = self.death_rate_data[year_label].unique()
             year_ind = sc.findnearest(available_years, sim.year)
             nearest_year = available_years[year_ind]
 
-            df = module.death_rate_data.loc[module.death_rate_data[year_label] == nearest_year]
+            df = self.death_rate_data.loc[self.death_rate_data[year_label] == nearest_year]
             age_bins = df[age_label].unique()
-            age_inds = np.digitize(sim.people.age[uids], age_bins) - 1
 
             f_arr = df[val_label].loc[df[sex_label] == sex_keys['f']].values
             m_arr = df[val_label].loc[df[sex_label] == sex_keys['m']].values
 
             # Initialize
             death_rate_df = pd.Series(index=uids)
-            death_rate_df[uids[sim.people.female[uids]]] = f_arr[age_inds[sim.people.female[uids]]] # TODO: avoid double indexing
-            death_rate_df[uids[sim.people.male[uids]]] = m_arr[age_inds[sim.people.male[uids]]]
-            death_rate_df[uids[sim.people.age[uids] < 0]] = 0  # Don't use background death rates for unborn babies
+            f_uids = uids.intersect(ppl.female.uids) # TODO: reduce duplication
+            m_uids = uids.intersect(ppl.male.uids)
+            f_age_inds = np.digitize(ppl.age[f_uids], age_bins) - 1
+            m_age_inds = np.digitize(ppl.age[m_uids], age_bins) - 1
+            death_rate_df[f_uids] = f_arr[f_age_inds]
+            death_rate_df[m_uids] = m_arr[m_age_inds]
+            unborn_inds = uids.intersect((sim.people.age < 0).uids)
+            death_rate_df[unborn_inds] = 0  # Don't use background death rates for unborn babies
 
             death_rate = death_rate_df.values
 
         # Scale from rate to probability. Consider an exponential here.
-        death_prob = death_rate * (module.pars.units * module.pars.rel_death * sim.pars.dt)
+        death_prob = death_rate * (self.pars.units * self.pars.rel_death * sim.pars.dt)
         death_prob = np.clip(death_prob, a_min=0, a_max=1)
 
         return death_prob
 
-    def standardize_death_data(self):
-        """ Standardize/validate death rates - handled in an external file due to shared functionality """
-        death_rate = ss.standardize_data(data=self.pars.death_rate, metadata=self.metadata)
-        return death_rate
-
-    def init_results(self, sim):
+    def init_results(self):
+        npts = self.sim.npts
         self.results += [
-            ss.Result(self.name, 'new', sim.npts, dtype=int, scale=True),
-            ss.Result(self.name, 'cumulative', sim.npts, dtype=int, scale=True),
-            ss.Result(self.name, 'cmr', sim.npts, dtype=int, scale=False),
+            ss.Result(self.name, 'new', npts, dtype=int, scale=True),
+            ss.Result(self.name, 'cumulative', npts, dtype=int, scale=True),
+            ss.Result(self.name, 'cmr', npts, dtype=int, scale=False),
         ]
         return
 
-    def update(self, sim):
-        n_deaths = self.apply_deaths(sim)
-        self.update_results(n_deaths, sim)
+    def update(self):
+        self.n_deaths = self.apply_deaths()
         return
 
-    def apply_deaths(self, sim):
+    def apply_deaths(self):
         """ Select people to die """
-        alive_uids = ss.true(sim.people.alive)
-        death_uids = self.pars.death_rate.filter(alive_uids)
-        sim.people.request_death(death_uids)
+        death_uids = self.pars.death_rate.filter()
+        self.sim.people.request_death(death_uids)
         return len(death_uids)
 
-    def update_results(self, n_deaths, sim):
-        self.results['new'][sim.ti] = n_deaths
+    def update_results(self):
+        self.results['new'][self.sim.ti] = self.n_deaths
         return
 
-    def finalize(self, sim):
-        super().finalize(sim)
-        self.results['cumulative'] = np.cumsum(self.results['new'])
-        self.results['cmr'] = 1/self.pars.units*np.divide(self.results['new'] / sim.dt, sim.results['n_alive'], where=sim.results['n_alive']>0)
+    def finalize(self):
+        super().finalize()
+        n_alive = self.sim.results.n_alive
+        self.results.cumulative = np.cumsum(self.results.new)
+        self.results.cmr = 1/self.pars.units*np.divide(self.results.new / self.sim.dt, n_alive, where=n_alive>0)
         return
 
 
 class Pregnancy(Demographics):
-
-    def __init__(self, pars=None, par_dists=None, metadata=None, **kwargs):
-        super().__init__(pars, **kwargs)
-
-        # Other, e.g. postpartum, on contraception...
-        self.add_states(
-            ss.State('infertile', bool, False),  # Applies to girls and women outside the fertility window
-            ss.State('fecund', bool, True),  # Applies to girls and women inside the fertility window
-            ss.State('pregnant', bool, False),  # Currently pregnant
-            ss.State('postpartum', bool, False),  # Currently post-partum
-            ss.State('ti_pregnant', int, ss.INT_NAN),  # Time pregnancy begins
-            ss.State('ti_delivery', int, ss.INT_NAN),  # Time of delivery
-            ss.State('ti_postpartum', int, ss.INT_NAN),  # Time postpartum ends
-            ss.State('ti_dead', int, ss.INT_NAN),  # Maternal mortality
-        )
-
-        self.pars = ss.omergeleft(self.pars,
+    """ Create births via pregnancies """
+    def __init__(self, pars=None, metadata=None, **kwargs):
+        super().__init__()
+        self.default_pars(
             dur_pregnancy = 0.75,
             dur_postpartum = 0.5,
-            fertility_rate = 0,    # Usually this will be provided in CSV format
+            fertility_rate = 0, # See make_fertility_prob_function
             rel_fertility = 1,
-            maternal_death_rate = 0,
-            sex_ratio = 0.5,       # Ratio of babies born female
-            units = 1e-3,          # Assumes fertility rates are per 1000. If using percentages, switch this to 1
+            maternal_death_prob = ss.bernoulli(0),
+            sex_ratio = ss.bernoulli(0.5), # Ratio of babies born female
+            units = 1e-3, # Assumes fertility rates are per 1000. If using percentages, switch this to 1
         )
-
-        self.par_dists = ss.omergeleft(par_dists,
-            fertility_rate = ss.bernoulli,
-            maternal_death_rate = ss.bernoulli,
-            sex_ratio = ss.bernoulli
+        self.update_pars(pars, **kwargs)
+        
+        # Other, e.g. postpartum, on contraception...
+        self.add_states(
+            ss.BoolArr('infertile'),  # Applies to girls and women outside the fertility window
+            ss.BoolArr('fecund', default=True),  # Applies to girls and women inside the fertility window
+            ss.BoolArr('pregnant'),  # Currently pregnant
+            ss.BoolArr('postpartum'),  # Currently post-partum
+            ss.FloatArr('ti_pregnant'),  # Time pregnancy begins
+            ss.FloatArr('ti_delivery'),  # Time of delivery
+            ss.FloatArr('ti_postpartum'),  # Time postpartum ends
+            ss.FloatArr('ti_dead'),  # Maternal mortality
         )
 
         # Process metadata. Defaults here are the labels used by UN data
-        self.metadata = ss.omergeleft(metadata,
-            data_cols = dict(year='Time', age='AgeGrp', value='ASFR'),
+        self.metadata = sc.mergedicts(
+            sc.objdict(data_cols=dict(year='Time', age='AgeGrp', value='ASFR')),
+            metadata,
         )
-
-        self.choose_slots = ss.randint() # Low and high will be reset upon initialization
+        self.choose_slots = None # Distribution for choosing slots; set in self.initialize()
 
         # Process data, which may be provided as a number, dict, dataframe, or series
         # If it's a number it's left as-is; otherwise it's converted to a dataframe
         self.fertility_rate_data = self.standardize_fertility_data()
-        self.pars.fertility_rate = self.make_fertility_prob_fn
+        self.pars.fertility_rate = ss.bernoulli(self.make_fertility_prob_fn)
 
+        # For results tracking
+        self.n_pregnancies = 0
+        self.n_births = 0
         return
 
     @staticmethod
-    def make_fertility_prob_fn(module, sim, uids):
+    def make_fertility_prob_fn(self, sim, uids):
         """ Take in the module, sim, and uids, and return the conception probability for each UID on this timestep """
 
-        if sc.isnumber(module.fertility_rate_data):
-            fertility_rate = module.fertility_rate_data
+        if sc.isnumber(self.fertility_rate_data):
+            fertility_rate = self.fertility_rate_data
 
         else:
             # Abbreviate key variables
-            data_cols = sc.objdict(module.metadata.data_cols)
+            data_cols = sc.objdict(self.metadata.data_cols)
             year_label = data_cols.year
             age_label  = data_cols.age
             val_label  = data_cols.value
 
-            available_years = module.fertility_rate_data[year_label].unique()
-            year_ind = sc.findnearest(available_years, sim.year-module.pars.dur_pregnancy)
+            available_years = self.fertility_rate_data[year_label].unique()
+            year_ind = sc.findnearest(available_years, sim.year-self.pars.dur_pregnancy)
             nearest_year = available_years[year_ind]
 
-            df = module.fertility_rate_data.loc[module.fertility_rate_data[year_label] == nearest_year]
+            df = self.fertility_rate_data.loc[self.fertility_rate_data[year_label] == nearest_year]
             df_arr = df[val_label].values  # Pull out dataframe values
             df_arr = np.append(df_arr, 0)  # Add zeros for those outside data range
 
             # Process age data
             age_bins = df[age_label].unique()
             age_bins = np.append(age_bins, age_bins[-1]+1) # WARNING: Assumes one year age bins! TODO: More robust handling.
             age_inds = np.digitize(sim.people.age[uids], age_bins) - 1
             age_inds[age_inds == len(age_bins)-1] = -1  # This ensures women outside the data range will get a value of 0
 
             # Adjust rates: rates are based on the entire population, but we need to remove
             # anyone already pregnant and then inflate the rates for the remainder
-            pregnant_uids = ss.true(module.pregnant[uids])  # Find agents who are already pregnant
+            pregnant_uids = self.pregnant.uids # Find agents who are already pregnant
             pregnant_age_counts, _ = np.histogram(sim.people.age[pregnant_uids], age_bins)  # Count them by age
             age_counts, _ = np.histogram(sim.people.age[uids], age_bins)  # Count overall number per age bin
             new_denom = age_counts - pregnant_age_counts  # New denominator for rates
             num_to_make = df_arr[:-1]*age_counts  # Number that we need to make pregnant
             new_percent = sc.dcp(df_arr)  # Initialize array with new rates
             inds_to_rescale = new_denom > 0  # Rescale any non-zero age bins
             new_percent[:-1][inds_to_rescale] = num_to_make[inds_to_rescale] / new_denom[inds_to_rescale]  # New rates
 
             # Make array of fertility rates
             fertility_rate = pd.Series(index=uids)
             fertility_rate[uids] = new_percent[age_inds]
             fertility_rate[pregnant_uids] = 0
 
         # Scale from rate to probability. Consider an exponential here.
-        fertility_prob = fertility_rate * (module.pars.units * module.pars.rel_fertility * sim.pars.dt)
+        fertility_prob = fertility_rate * (self.pars.units * self.pars.rel_fertility * sim.pars.dt)
         fertility_prob = np.clip(fertility_prob, a_min=0, a_max=1)
 
         return fertility_prob
 
     def standardize_fertility_data(self):
         """ Standardize/validate fertility rates - handled in an external file due to shared functionality """
         fertility_rate = ss.standardize_data(data=self.pars.fertility_rate, metadata=self.metadata)
         return fertility_rate
 
     def initialize(self, sim):
         super().initialize(sim)
         low = sim.pars.n_agents + 1
         high = int(sim.pars.slot_scale*sim.pars.n_agents)
-        self.choose_slots.set(low=low, high=high)
+        self.choose_slots = ss.randint(low=low, high=high, sim=sim, module=self)
         return
 
-    def init_results(self, sim):
+    def init_results(self):
         """
         Results could include a range of birth outcomes e.g. LGA, stillbirths, etc.
         Still unclear whether this logic should live in the pregnancy module, the
         individual disease modules, the connectors, or the sim.
         """
+        npts = self.sim.npts
         self.results += [
-            ss.Result(self.name, 'pregnancies', sim.npts, dtype=int, scale=True),
-            ss.Result(self.name, 'births', sim.npts, dtype=int, scale=True),
-            ss.Result(self.name, 'cbr', sim.npts, dtype=int, scale=False),
+            ss.Result(self.name, 'pregnancies', npts, dtype=int, scale=True),
+            ss.Result(self.name, 'births', npts, dtype=int, scale=True),
+            ss.Result(self.name, 'cbr', npts, dtype=int, scale=False),
         ]
         return
 
-    def update(self, sim):
-        """
-        Perform all updates
-        """
-        self.update_states(sim)
-        conceive_uids = self.make_pregnancies(sim)
-        self.make_embryos(sim, conceive_uids)
-        self.update_results(sim)
+    def update(self):
+        """ Perform all updates """
+        self.update_states()
+        conceive_uids = self.make_pregnancies()
+        self.n_pregnancies = len(conceive_uids)
+        self.make_embryos(conceive_uids)
         return
 
-    def update_states(self, sim):
-        """
-        Update states
-        """
-
+    def update_states(self):
+        """ Update states """
         # Check for new deliveries
-        deliveries = self.pregnant & (self.ti_delivery <= sim.ti)
+        ti = self.sim.ti
+        deliveries = self.pregnant & (self.ti_delivery <= ti)
+        self.n_births = np.count_nonzero(deliveries)
         self.pregnant[deliveries] = False
         self.postpartum[deliveries] = True
         self.fecund[deliveries] = False
 
         # Check for new women emerging from post-partum
-        postpartum = ~self.pregnant & (self.ti_postpartum <= sim.ti)
+        postpartum = ~self.pregnant & (self.ti_postpartum <= ti)
         self.postpartum[postpartum] = False
         self.fecund[postpartum] = True
 
         # Maternal deaths
-        maternal_deaths = ss.true(self.ti_dead <= sim.ti)
-        sim.people.request_death(maternal_deaths)
-
+        maternal_deaths = (self.ti_dead <= ti).uids
+        self.sim.people.request_death(maternal_deaths)
         return
 
-    def make_pregnancies(self, sim):
-        """
-        Select people to make pregnant using incidence data
-        """
-        # Abbreviate
-        ppl = sim.people
-
+    def make_pregnancies(self):
+        """ Select people to make pregnant using incidence data """
         # People eligible to become pregnant. We don't remove pregnant people here, these
         # are instead handled in the fertility_dist logic as the rates need to be adjusted
-        denom_conds = ppl.female & ppl.alive
-        inds_to_choose_from = ss.true(denom_conds)
-        conceive_uids = self.pars.fertility_rate.filter(inds_to_choose_from)
+        eligible_uids = self.sim.people.female.uids
+        conceive_uids = self.pars.fertility_rate.filter(eligible_uids)
 
         # Set prognoses for the pregnancies
         if len(conceive_uids) > 0:
-            self.set_prognoses(sim, conceive_uids)
-
+            self.set_prognoses(conceive_uids)
         return conceive_uids
 
-    def make_embryos(self, sim, conceive_uids):
+    def make_embryos(self, conceive_uids):
         """ Add properties for the just-conceived """
-        n_unborn_agents = len(conceive_uids)
-        if n_unborn_agents > 0:
+        people = self.sim.people
+        n_unborn = len(conceive_uids)
+        if n_unborn == 0:
+            new_uids = ss.uids()
+        else:
 
             # Choose slots for the unborn agents
             new_slots = self.choose_slots.rvs(conceive_uids)
 
             # Grow the arrays and set properties for the unborn agents
-            new_uids = sim.people.grow(len(new_slots), new_slots)
-            sim.people.age[new_uids] = -self.pars.dur_pregnancy
-            sim.people.slot[new_uids] = new_slots  # Before sampling female_dist
-            sim.people.female[new_uids] = self.pars.sex_ratio.rvs(new_uids)
+            new_uids = people.grow(len(new_slots), new_slots)
+            people.age[new_uids] = -self.pars.dur_pregnancy
+            people.slot[new_uids] = new_slots  # Before sampling female_dist
+            people.female[new_uids] = self.pars.sex_ratio.rvs(conceive_uids)
 
             # Add connections to any vertical transmission layers
             # Placeholder code to be moved / refactored. The maternal network may need to be
             # handled separately to the sexual networks, TBC how to handle this most elegantly
-            for lkey, layer in sim.networks.items():
+            for lkey, layer in self.sim.networks.items():
                 if layer.vertical:  # What happens if there's more than one vertical layer?
-                    durs = np.full(n_unborn_agents, fill_value=self.pars.dur_pregnancy + self.pars.dur_postpartum)
+                    durs = np.full(n_unborn, fill_value=self.pars.dur_pregnancy + self.pars.dur_postpartum)
                     layer.add_pairs(conceive_uids, new_uids, dur=durs)
 
-        return
+        return new_uids
 
-    def set_prognoses(self, sim, uids):
+    def set_prognoses(self, uids):
         """
         Make pregnancies
         Add miscarriage/termination logic here
         Also reconciliation with birth rates
         Q, is this also a good place to check for other conditions and set prognoses for the fetus?
         """
 
         # Change states for the newly pregnant woman
+        ti = self.sim.ti
+        dt = self.sim.dt
         self.fecund[uids] = False
         self.pregnant[uids] = True
-        self.ti_pregnant[uids] = sim.ti
+        self.ti_pregnant[uids] = ti
 
         # Outcomes for pregnancies
-        dur_preg = np.full(len(uids), self.pars.dur_pregnancy / sim.dt)
-        dur_postpartum = np.full(len(uids), self.pars.dur_postpartum / sim.dt)
-        dead = self.pars.maternal_death_rate.rvs(uids)
-        self.ti_delivery[uids] = sim.ti + dur_preg # Currently assumes maternal deaths still result in a live baby
-        self.ti_postpartum[uids] = sim.ti + dur_preg + dur_postpartum
+        dur_preg = np.full(len(uids), self.pars.dur_pregnancy / dt)
+        dur_postpartum = np.full(len(uids), self.pars.dur_postpartum / dt)
+        dead = self.pars.maternal_death_prob.rvs(uids)
+        self.ti_delivery[uids] = ti + dur_preg # Currently assumes maternal deaths still result in a live baby
+        self.ti_postpartum[uids] = ti + dur_preg + dur_postpartum
 
         if np.any(dead): # NB: 100x faster than np.sum(), 10x faster than np.count_nonzero()
-            self.ti_dead[uids[dead]] = sim.ti + dur_preg[dead]
+            self.ti_dead[uids[dead]] = ti + dur_preg[dead]
         return
 
-    def update_results(self, sim):
-        self.results['pregnancies'][sim.ti] = np.count_nonzero(self.ti_pregnant == sim.ti)
-        self.results['births'][sim.ti] = np.count_nonzero(self.ti_delivery == sim.ti)
+    def update_results(self):
+        ti = self.sim.ti
+        self.results['pregnancies'][ti] = self.n_pregnancies
+        self.results['births'][ti] = self.n_births
         return
 
-    def finalize(self, sim):
-        super().finalize(sim)
-        self.results['cbr'] = 1/self.pars.units * np.divide(self.results['births'] / sim.dt, sim.results['n_alive'], where=sim.results['n_alive']>0)
+    def finalize(self):
+        super().finalize()
+        n_alive = self.sim.results.n_alive
+        self.results['cbr'] = 1/self.pars.units * np.divide(self.results['births'] / self.sim.dt, n_alive, where=n_alive>0)
+        return
```

### Comparing `starsim-0.3.4/starsim/disease.py` & `starsim-0.5.0/starsim/disease.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 __all__ = ['Disease', 'Infection', 'InfectionLog']
 
 
 class Disease(ss.Module):
     """ Base module class for diseases """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self):
+        super().__init__()
         self.results = ss.Results(self.name)
         self.log = InfectionLog()  # See below for definition
         return
 
     @property
     def _boolean_states(self):
         """
@@ -32,78 +32,36 @@
         for state in self.states:
             if state.dtype == bool:
                 yield state
         return
 
     def initialize(self, sim):
         super().initialize(sim)
-        self.validate_pars(sim)
-        self.init_results(sim)
-        self.set_initial_states(sim)
+        self.init_results()
         return
 
-    def finalize(self, sim):
-        super().finalize(sim)
-        return
-
-    def validate_pars(self, sim):
-        """
-        Perform any parameter validation
-        """
-        if sim.networks is not None and len(sim.networks) > 0:
-
-            # If there's no beta, make a default one
-            if 'beta' not in self.pars or self.pars.beta is None:
-                self.pars.beta = sc.objdict({k: [1, 1] for k in sim.networks})
-                msg = f'Beta not supplied for disease "{self.name}"; defaulting to 1'
-                ss.warn(msg)
-
-            # If beta is a scalar, apply this bi-directionally to all networks
-            if sc.isnumber(self.pars.beta):
-                orig_beta = self.pars.beta
-                self.pars.beta = sc.objdict({k: [orig_beta] * 2 for k in sim.networks})
-
-            # If beta is a dict, check all entries are bi-directional
-            elif isinstance(self.pars.beta, dict):
-                for k, v in self.pars.beta.items():
-                    if sc.isnumber(v):
-                        self.pars.beta[k] = [v, v]
-        return
-
-    def set_initial_states(self, sim):
-        """
-        Set initial values for states
-
-        This could involve passing in a full set of initial conditions,
-        or using init_prev, or other. Note that this is different to initialization of the State objects
-        i.e., creating their dynamic array, linking them to a People instance. That should have already
-        taken place by the time this method is called. This method is about supplying initial values
-        for the states (e.g., seeding initial infections)
-        """
-        pass
-
-    def init_results(self, sim):
+    def init_results(self):
         """
         Initialize results
 
         By default, diseases all report on counts for any boolean states e.g., if
         a disease contains a boolean state 'susceptible' it will automatically contain a
         Result for 'n_susceptible'
         """
         for state in self._boolean_states:
-            self.results += ss.Result(self.name, f'n_{state.name}', sim.npts, dtype=int, scale=True)
+            self.results += ss.Result(self.name, f'n_{state.name}', self.sim.npts, dtype=int, scale=True)
         return
 
-    def update_pre(self, sim):
+    def update_pre(self):
         """
         Carry out autonomous updates at the start of the timestep (prior to transmission)
         """
         pass
 
-    def update_death(self, sim, uids):
+    def update_death(self, uids):
         """
         Carry out state changes upon death
 
         This function is triggered after deaths are resolved, and before analyzers are run.
         See the SIR example model for a typical use case - deaths are requested as an autonomous
         update, to take effect after transmission on the same timestep. State changes that occur
         upon death (e.g., clearing an `infected` flag) are executed in this function. That also
@@ -112,29 +70,29 @@
         function if the death actually occurs).
 
         Depending on the module and the results it produces, it may or may not be necessary
         to implement this.
         """
         pass
 
-    def make_new_cases(self, sim):
+    def make_new_cases(self):
         """
         Add new cases of the disease
 
         This method is agnostic as to the mechanism by which new cases occur. This
         could be through transmission (parametrized in different ways, which may or
         may not use the contact networks) or it may be based on risk factors/seeding,
         as may be the case for non-communicable diseases.
 
         It is expected that this method will internally call Disease.set_prognoses()
         at some point.
         """
         pass
 
-    def set_prognoses(self, sim, target_uids, source_uids=None):
+    def set_prognoses(self, target_uids, source_uids=None):
         """
         Set prognoses upon infection/acquisition
 
         This function assigns state values upon infection or acquisition of
         the disease. It would normally be called somewhere towards the end of
         `Disease.make_new_cases()`. Infections will automatically be added to
         the log as part of this operation.
@@ -143,104 +101,134 @@
         as `None` for NCDs.
 
         Args:
             sim (Sim): the STarsim simulation object
             uids (array): UIDs for agents to assign disease progoses to
             from_uids (array): Optionally specify the infecting agent
         """
+        sim = self.sim
         if source_uids is None:
             for target in target_uids:
                 self.log.append(np.nan, target, sim.year)
         else:
             for target, source in zip(target_uids, source_uids):
                 self.log.append(source, target, sim.year)
         return
 
-    def update_results(self, sim):
+    def update_results(self):
         """
         Update results
 
         This function is executed after transmission in all modules has been resolved.
         This allows result updates at this point to capture outcomes dependent on multiple
         modules, where relevant.
         """
+        sim = self.sim
         for state in self._boolean_states:
             self.results[f'n_{state.name}'][sim.ti] = np.count_nonzero(state & sim.people.alive)
         return
 
 
 class Infection(Disease):
     """
     Base class for infectious diseases used in Starsim
 
     This class contains specializations for infectious transmission (i.e., implements network-based
     transmission with directional beta values) and defines attributes that connectors
     operate on to capture co-infection
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self):
+        super().__init__()
         self.add_states(
-            ss.State('susceptible', bool, True),
-            ss.State('infected', bool, False),
-            ss.State('rel_sus', float, 1.0),
-            ss.State('rel_trans', float, 1.0),
-            ss.State('ti_infected', int, ss.INT_NAN),
+            ss.BoolArr('susceptible', default=True),
+            ss.BoolArr('infected'),
+            ss.FloatArr('rel_sus', default=1.0),
+            ss.FloatArr('rel_trans', default=1.0),
+            ss.FloatArr('ti_infected'),
         )
 
+        # Define random number generators for make_new_cases
         self.rng_target = ss.random(name='target')
         self.rng_source = ss.random(name='source')
+        return
+    
+    def initialize(self, sim):
+        super().initialize(sim)
+        self.validate_beta()
+        return
+    
+    def validate_beta(self):
+        """
+        Perform any parameter validation
+        """
+        networks = self.sim.networks
+        if networks is not None and len(networks) > 0:
+            
+            if 'beta' not in self.pars:
+                errormsg = f'Disease {self.name} is missing beta; pars are: {sc.strjoin(self.pars.keys())}'
+                raise sc.KeyNotFoundError(errormsg)
 
+            # If beta is a scalar, apply this bi-directionally to all networks
+            if sc.isnumber(self.pars.beta):
+                β = self.pars.beta
+                self.pars.beta = sc.objdict({k:[β,β] for k in networks.keys()})
+
+            # If beta is a dict, check all entries are bi-directional
+            elif isinstance(self.pars.beta, dict):
+                for k,β in self.pars.beta.items():
+                    if sc.isnumber(β):
+                        self.pars.beta[k] = [β,β]
         return
 
     @property
     def infectious(self):
         """
         Generally defined as an alias for infected, although these may differ in some diseases.
         Transmission comes from infectious people; prevalence estimates may include infected people who don't transmit
         """
         return self.infected
 
-    def set_initial_states(self, sim):
+    def init_vals(self):
         """
         Set initial values for states. This could involve passing in a full set of initial conditions,
-        or using init_prev, or other. Note that this is different to initialization of the State objects
+        or using init_prev, or other. Note that this is different to initialization of the Arr objects
         i.e., creating their dynamic array, linking them to a People instance. That should have already
         taken place by the time this method is called.
         """
         if self.pars.init_prev is None:
             return
 
-        alive_uids = ss.true(sim.people.alive)  # Maybe just sim.people.uid?
-        initial_cases = self.pars.init_prev.filter(alive_uids)
-        self.set_prognoses(sim, initial_cases)  # TODO: sentinel value to indicate seeds?
+        initial_cases = self.pars.init_prev.filter()
+        self.set_prognoses(initial_cases)  # TODO: sentinel value to indicate seeds?
         return
 
-    def init_results(self, sim):
+    def init_results(self):
         """
         Initialize results
         """
-        super().init_results(sim)
+        super().init_results()
+        sim = self.sim
         self.results += [
-            ss.Result(self.name, 'prevalence', sim.npts, dtype=float, scale=False),
+            ss.Result(self.name, 'prevalence',     sim.npts, dtype=float, scale=False),
             ss.Result(self.name, 'new_infections', sim.npts, dtype=int, scale=True),
             ss.Result(self.name, 'cum_infections', sim.npts, dtype=int, scale=True),
         ]
         return
 
-    def _check_betas(self, sim):
+    def _check_betas(self):
         """ Check that there's a network for each beta key """
         # Ensure keys are lowercase
         if isinstance(self.pars.beta, dict): # TODO: check if needed
             self.pars.beta = {k.lower(): v for k, v in self.pars.beta.items()}
 
         # Create a mapping between beta and networks, and populate it
         betapars = self.pars.beta
         betamap = sc.objdict()
-        netkeys = list(sim.networks.keys())
+        netkeys = list(self.sim.networks.keys())
         if netkeys: # Skip if no networks
             for bkey in betapars.keys():
                 orig_bkey = bkey[:]
                 if bkey in netkeys: # TODO: CK: could tidy up logic
                     betamap[bkey] = betapars[orig_bkey]
                 else:
                     if 'net' not in bkey:
@@ -248,44 +236,44 @@
                     if bkey in netkeys:
                         betamap[bkey] = betapars[orig_bkey]
                     else:
                         errormsg = f'No network for beta parameter "{bkey}"; your beta should match network keys:\n{sc.newlinejoin(netkeys)}'
                         raise ValueError(errormsg)
         return betamap
 
-    def make_new_cases(self, sim):
+    def make_new_cases(self):
         """
         Add new cases of module, through transmission, incidence, etc.
         
         Common-random-number-safe transmission code works by mapping edges onto
         slots.
         """
         new_cases = []
         sources = []
-        people = sim.people
-        betamap = self._check_betas(sim)
+        betamap = self._check_betas()
 
-        for nkey,net in sim.networks.items():
+        for nkey,net in self.sim.networks.items():
             if not len(net):
                 break
 
             nbetas = betamap[nkey]
             contacts = net.contacts
-            rel_trans = (self.infectious & people.alive) * self.rel_trans
-            rel_sus = (self.susceptible & people.alive) * self.rel_sus
+
+            rel_trans = self.rel_trans.asnew(self.infectious * self.rel_trans)
+            rel_sus   = self.rel_sus.asnew(self.susceptible * self.rel_sus)
             p1p2b0 = [contacts.p1, contacts.p2, nbetas[0]]
             p2p1b1 = [contacts.p2, contacts.p1, nbetas[1]]
             for src, trg, beta in [p1p2b0, p2p1b1]:
 
                 # Skip networks with no transmission
                 if beta == 0:
                     continue
 
                 # Calculate probability of a->b transmission.
-                beta_per_dt = net.beta_per_dt(disease_beta=beta, dt=people.dt) # TODO: should this be sim.dt?
+                beta_per_dt = net.beta_per_dt(disease_beta=beta, dt=self.sim.dt)
                 p_transmit = rel_trans[src] * rel_sus[trg] * beta_per_dt
 
                 # Generate a new random number based on the two other random numbers -- 3x faster than `rvs = np.remainder(rvs_s + rvs_t, 1)`
                 rvs_s = self.rng_source.rvs(src)
                 rvs_t = self.rng_target.rvs(trg)
                 rvs = rvs_s + rvs_t
                 inds = np.where(rvs>1.0)[0]
@@ -293,42 +281,43 @@
                 
                 new_cases_bool = rvs < p_transmit
                 new_cases.append(trg[new_cases_bool])
                 sources.append(src[new_cases_bool])
                 
         # Tidy up
         if len(new_cases) and len(sources):
-            new_cases = np.concatenate(new_cases)
-            sources = np.concatenate(sources)
+            new_cases = ss.uids.cat(new_cases)
+            sources = ss.uids.cat(sources)
         else:
             new_cases = np.empty(0, dtype=int)
             sources = np.empty(0, dtype=int)
             
         if len(new_cases):
-            self._set_cases(sim, new_cases, sources)
+            self._set_cases(new_cases, sources)
             
         return new_cases, sources
 
-    def _set_cases(self, sim, target_uids, source_uids=None):
+    def _set_cases(self, target_uids, source_uids=None):
+        sim = self.sim
         congenital = sim.people.age[target_uids] <= 0
-        if len(ss.true(congenital)) > 0:
+        if np.count_nonzero(congenital):
             src_c = source_uids[congenital] if source_uids is not None else None
-            self.set_congenital(sim, target_uids[congenital], src_c)
+            self.set_congenital(target_uids[congenital], src_c)
         src_p = source_uids[~congenital] if source_uids is not None else None
-        self.set_prognoses(sim, target_uids[~congenital], src_p)
+        self.set_prognoses(target_uids[~congenital], src_p)
         return
 
-    def set_congenital(self, sim, target_uids, source_uids=None):
+    def set_congenital(self, target_uids, source_uids=None):
         pass
 
-    def update_results(self, sim):
-        super().update_results(sim)
+    def update_results(self):
+        super().update_results()
         res = self.results
-        ti = sim.ti
-        res.prevalence[ti] = res.n_infected[ti] / np.count_nonzero(sim.people.alive)
+        ti = self.sim.ti
+        res.prevalence[ti] = res.n_infected[ti] / np.count_nonzero(self.sim.people.alive)
         res.new_infections[ti] = np.count_nonzero(self.ti_infected == ti)
         res.cum_infections[ti] = np.sum(res['new_infections'][:ti+1])
         return
 
 
 class InfectionLog(nx.MultiDiGraph):
     """
@@ -373,16 +362,19 @@
         :param kwargs: Remaining arguments are stored as edge data
         """
         for uid in sc.promotetoarray(uids):
             source, target, key = max(self.in_edges(uid, keys=True),
                                       key=itemgetter(2, 0))  # itemgetter twice as fast as lambda apparently
             self[source][target][key].update(**kwargs)
 
+        return
+
     def append(self, source, target, t, **kwargs):
         self.add_edge(source, target, key=t, **kwargs)
+        return
 
     @property
     def line_list(self):
         """
         Return a tabular representation of the log
 
         This function returns a dataframe containing columns for all quantities
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `starsim-0.3.4/starsim/diseases/cholera.py` & `starsim-0.5.0/starsim/diseases/cholera.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,188 +10,179 @@
 __all__ = ['Cholera']
 
 
 class Cholera(ss.Infection):
     """
     Cholera
     """
-    def __init__(self, pars=None, par_dists=None, *args, **kwargs):
+    def __init__(self, pars=None, *args, **kwargs):
         """ Initialize with parameters """
-
-        pars = ss.omergeleft(pars,
-            # Natural history parameters, all specified in days
-            dur_exp2inf = ss.lognorm_ex(mean=2.772, stdev=4.737),  # Calculated from Azman et al. estimates https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3677557/
-            dur_asymp2rec = ss.uniform(low=1, high=10),    # From WHO cholera fact sheet, asymptomatic individuals shed bacteria for 1-10 days (https://www.who.int/news-room/fact-sheets/detail/cholera)
-            dur_symp2rec = ss.lognorm_ex(mean=5, stdev=1.8),    # According to Fung most modelling studies assume 5 days of symptoms (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3926264/), but found a range of 2.9-14 days. Distribution approximately fit to these values
-            dur_symp2dead = ss.lognorm_ex(mean=1, stdev=0.5),   # There does not appear to be differences in timing/duration of mild vs severe disease, but death from severe disease happens rapidly https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5767916/
-            p_death = 0.005,   # Probability of death is typically less than 1% when treated
-            p_symp = 0.5,   # Proportion of infected which are symptomatic, mid range of ~25% and 57% estimates from Jaclson et al (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3795095/) and Nelson et al (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3842031/), respectively
-            asymp_trans = 0.01,    # Reduction in transmission probability for asymptomatic infection, asymptomatic carriers shed 100-1000 times less bacteria than symptomatic carriers (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3084143/ and https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3842031/). Previous models assume a 10% relative transmissibility (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4238032/)
-
+        super().__init__()
+        self.default_pars(
             # Initial conditions and beta
-            init_prev = 0.005,
-            beta = None,
+            beta = 1.0, # Placeholder value
+            init_prev = ss.bernoulli(0.005),
+            
+            # Natural history parameters, all specified in days
+            dur_exp2inf   = ss.lognorm_ex(mean=2.772, stdev=4.737), # Calculated from Azman et al. estimates https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3677557/
+            dur_asymp2rec = ss.uniform(low=1, high=10), # From WHO cholera fact sheet, asymptomatic individuals shed bacteria for 1-10 days (https://www.who.int/news-room/fact-sheets/detail/cholera)
+            dur_symp2rec  = ss.lognorm_ex(mean=5, stdev=1.8), # According to Fung most modelling studies assume 5 days of symptoms (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3926264/), but found a range of 2.9-14 days. Distribution approximately fit to these values
+            dur_symp2dead = ss.lognorm_ex(mean=1, stdev=0.5), # There does not appear to be differences in timing/duration of mild vs severe disease, but death from severe disease happens rapidly https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5767916/
+            p_death       = ss.bernoulli(p=0.005), # Probability of death is typically less than 1% when treated
+            p_symp        = ss.bernoulli(p=0.5), # Proportion of infected which are symptomatic, mid range of ~25% and 57% estimates from Jaclson et al (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3795095/) and Nelson et al (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3842031/), respectively
+            asymp_trans   = 0.01, # Reduction in transmission probability for asymptomatic infection, asymptomatic carriers shed 100-1000 times less bacteria than symptomatic carriers (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3084143/ and https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3842031/). Previous models assume a 10% relative transmissibility (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4238032/)
 
             # Environmental parameters
-            beta_env = 0.5 / 3,  # Scaling factor for transmission from environment,
-            half_sat_rate = 1000000,   # Infectious dose in water sufficient to produce infection in 50% of  exposed, from Mukandavire et al. (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3102413/)
-            shedding_rate = 10,    # Rate at which infectious people shed bacteria to the environment (per day), from Mukandavire et al. (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3102413/)
-            decay_rate = 0.033,    # Rate at which bacteria in the environment dies (per day), from Chao et al. and Mukandavire et al. citing https://pubmed.ncbi.nlm.nih.gov/8882180/
-            p_env_transmit = 0,    # Probability of environmental transmission - filled out later
-        )
-
-        par_dists = ss.omergeleft(par_dists,
-            dur_exp2inf    = ss.lognorm_ex,
-            dur_asymp2rec  = ss.uniform,
-            dur_symp2rec   = ss.lognorm_ex,
-            dur_symp2dead  = ss.lognorm_ex,
-            init_prev      = ss.bernoulli,
-            p_death        = ss.bernoulli,
-            p_symp         = ss.bernoulli,
-            p_env_transmit = ss.bernoulli,
+            beta_env = 0.5 / 3, # Scaling factor for transmission from environment,
+            half_sat_rate = 1_000_000, # Infectious dose in water sufficient to produce infection in 50% of  exposed, from Mukandavire et al. (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3102413/)
+            shedding_rate = 10, # Rate at which infectious people shed bacteria to the environment (per day), from Mukandavire et al. (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3102413/)
+            decay_rate = 0.033, # Rate at which bacteria in the environment dies (per day), from Chao et al. and Mukandavire et al. citing https://pubmed.ncbi.nlm.nih.gov/8882180/
+            p_env_transmit = ss.bernoulli(p=0), # Probability of environmental transmission - filled out later
         )
-
-        super().__init__(pars=pars, par_dists=par_dists, *args, **kwargs)
+        self.update_pars(pars, **kwargs)
 
         # Boolean states
-        
         self.add_states(
             # Susceptible & infected are added automatically, here we add the rest
-            ss.State('exposed', bool, False),
-            ss.State('symptomatic', bool, False),
-            ss.State('recovered', bool, False),
+            ss.BoolArr('exposed'),
+            ss.BoolArr('symptomatic'),
+            ss.BoolArr('recovered'),
     
             # Timepoint states
-            ss.State('ti_exposed', float, np.nan),
-            ss.State('ti_symptomatic', float, np.nan),
-            ss.State('ti_recovered', float, np.nan),
-            ss.State('ti_dead', float, np.nan),
+            ss.FloatArr('ti_exposed'),
+            ss.FloatArr('ti_symptomatic'),
+            ss.FloatArr('ti_recovered'),
+            ss.FloatArr('ti_dead'),
         )
-
         return
 
     @property
     def infectious(self):
         return self.infected | self.exposed
 
     @property
     def asymptomatic(self):
         return self.infected & ~self.symptomatic
 
-    def init_results(self, sim):
+    def init_results(self):
         """
         Initialize results
         """
-        super().init_results(sim)
+        super().init_results()
+        npts = self.sim.npts
         self.results += [
-            ss.Result(self.name, 'new_deaths', sim.npts, dtype=int),
-            ss.Result(self.name, 'cum_deaths', sim.npts, dtype=int),
-            ss.Result(self.name, 'env_prev', sim.npts, dtype=float),
-            ss.Result(self.name, 'env_conc', sim.npts, dtype=float),
+            ss.Result(self.name, 'new_deaths', npts, dtype=int),
+            ss.Result(self.name, 'cum_deaths', npts, dtype=int),
+            ss.Result(self.name, 'env_prev', npts, dtype=float),
+            ss.Result(self.name, 'env_conc', npts, dtype=float),
         ]
         return
 
-    def update_pre(self, sim):
+    def update_pre(self):
         """
         Adapted from https://github.com/optimamodel/gavi-outbreaks/blob/main/stisim/gavi/cholera.py
         Original version by Dom Delport
         """
-
         # Progress exposed -> infected
-        infected = ss.true(self.exposed & (self.ti_infected <= sim.ti))
+        ti = self.sim.ti
+        infected = (self.exposed & (self.ti_infected <= ti)).uids
         self.infected[infected] = True
 
         # Progress infected -> symptomatic
-        symptomatic = ss.true(self.infected & (self.ti_symptomatic <= sim.ti))
+        symptomatic = (self.infected & (self.ti_symptomatic <= ti)).uids
         self.symptomatic[symptomatic] = True
 
         # Progress symptomatic -> recovered
-        recovered = ss.true(self.infectious & (self.ti_recovered <= sim.ti))
+        recovered = (self.infectious & (self.ti_recovered <= ti)).uids
+        self.exposed[recovered] = False
         self.infected[recovered] = False
-        self.infectious[recovered] = False
         self.symptomatic[recovered] = False
         self.recovered[recovered] = True
 
         # Trigger deaths
-        deaths = ss.true(self.ti_dead <= sim.ti)
+        deaths = (self.ti_dead <= ti).uids
         if len(deaths):
-            sim.people.request_death(deaths)
+            self.sim.people.request_death(deaths)
 
         # Update today's environmental prevalence
-        self.calc_environmental_prev(sim)
+        self.calc_environmental_prev()
 
-    def calc_environmental_prev(self, sim):
+        return
+
+    def calc_environmental_prev(self):
         """
         Calculate environmental prevalence
         """
         p = self.pars
         r = self.results
+        ti = self.sim.ti
 
-        n_symptomatic = len(ss.true(self.symptomatic))
-        n_asymptomatic = len(ss.true(self.asymptomatic))
-        old_prev = self.results.env_prev[sim.ti-1]
+        n_symptomatic = self.symptomatic.sum()
+        n_asymptomatic = self.asymptomatic.sum()
+        old_prev = self.results.env_prev[ti-1]
 
         new_bacteria = p.shedding_rate * (n_symptomatic + p.asymp_trans * n_asymptomatic)
         old_bacteria = old_prev * (1 - p.decay_rate)
 
-        r.env_prev[sim.ti] = new_bacteria + old_bacteria
-        r.env_conc[sim.ti] = r.env_prev[sim.ti] / (r.env_prev[sim.ti] + p.half_sat_rate)
+        r.env_prev[ti] = new_bacteria + old_bacteria
+        r.env_conc[ti] = r.env_prev[ti] / (r.env_prev[ti] + p.half_sat_rate)
+        return
 
-    def set_prognoses(self, sim, uids, source_uids=None):
+    def set_prognoses(self, uids, source_uids=None):
         """ Set prognoses for those who get infected """
-        super().set_prognoses(sim, uids, source_uids)
+        super().set_prognoses(uids, source_uids)
+        ti = self.sim.ti
+        dt = self.sim.dt
 
         self.susceptible[uids] = False
         self.exposed[uids] = True
-        self.ti_exposed[uids] = sim.ti
+        self.ti_exposed[uids] = ti
 
         p = self.pars
 
         # Determine when exposed become infected
-        self.ti_infected[uids] = sim.ti + p.dur_exp2inf.rvs(uids) / sim.dt
+        self.ti_infected[uids] = ti + p.dur_exp2inf.rvs(uids) / dt
 
         # Determine who becomes symptomatic and when
         symp_uids = p.p_symp.filter(uids)
         self.ti_symptomatic[symp_uids] = self.ti_infected[symp_uids]
 
         # Determine who dies and when
         dead_uids = p.p_death.filter(symp_uids)
-        self.ti_dead[dead_uids] = self.ti_symptomatic[dead_uids] + p.dur_symp2dead.rvs(dead_uids) / sim.dt
+        self.ti_dead[dead_uids] = self.ti_symptomatic[dead_uids] + p.dur_symp2dead.rvs(dead_uids) / dt
         symp_rev_uids = np.setdiff1d(symp_uids, dead_uids)
         asymp_uids = np.setdiff1d(uids, symp_uids)
 
         # Determine when agents recover
-        self.ti_recovered[symp_rev_uids] = self.ti_exposed[symp_rev_uids] + p.dur_symp2rec.rvs(symp_rev_uids) / sim.dt
-        self.ti_recovered[asymp_uids] = self.ti_exposed[asymp_uids] + p.dur_asymp2rec.rvs(asymp_uids) / sim.dt
+        self.ti_recovered[symp_rev_uids] = self.ti_exposed[symp_rev_uids] + p.dur_symp2rec.rvs(symp_rev_uids) / dt
+        self.ti_recovered[asymp_uids] = self.ti_exposed[asymp_uids] + p.dur_asymp2rec.rvs(asymp_uids) / dt
 
         return
 
-    def make_new_cases(self, sim):
+    def make_new_cases(self):
         """ Add indirect transmission """
-
-        pars = self.pars
-        res = self.results
-
         # Make new cases via direct transmission
-        super().make_new_cases(sim)
-
+        super().make_new_cases()
+        
         # Make new cases via indirect transmission
-        p_transmit = res.env_conc[sim.ti] * pars.beta_env
+        pars = self.pars
+        res = self.results
+        p_transmit = res.env_conc[self.sim.ti] * pars.beta_env
         pars.p_env_transmit.set(p=p_transmit)
-        new_cases = pars.p_env_transmit.filter(sim.people.uid[self.susceptible]) # TODO: make syntax nicer
+        new_cases = pars.p_env_transmit.filter(self.sim.people.uid[self.susceptible]) # TODO: make syntax nicer
         if new_cases.any():
-            self.set_prognoses(sim, new_cases, source_uids=None)
+            self.set_prognoses(new_cases, source_uids=None)
         return
 
-    def update_death(self, sim, uids):
+    def update_death(self, uids):
         """ Reset infected/recovered flags for dead agents """
         for state in ['susceptible', 'exposed', 'infected', 'symptomatic', 'recovered']:
             self.statesdict[state][uids] = False
         return
 
-    def update_results(self, sim):
-        super().update_results(sim)
+    def update_results(self):
+        super().update_results()
         res = self.results
-        ti = sim.ti
+        ti = self.sim.ti
         res.new_deaths[ti] = np.count_nonzero(self.ti_dead == ti)
         res.cum_deaths[ti] = np.sum(res.new_deaths[:ti+1])
         return
```

### Comparing `starsim-0.3.4/starsim/diseases/ebola.py` & `starsim-0.5.0/starsim/diseases/ebola.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,144 +9,130 @@
 from starsim.diseases.sir import SIR
 
 __all__ = ['Ebola']
 
 
 class Ebola(SIR):
 
-    def __init__(self, pars=None, par_dists=None, *args, **kwargs):
+    def __init__(self, pars=None, *args, **kwargs):
         """ Initialize with parameters """
-
-        pars = ss.omergeleft(pars,
-            # Natural history parameters, all specified in days
-            dur_exp2symp = 12.7, # Add source
-            dur_symp2sev =    6, # Add source
-            dur_sev2dead =  1.5, # Add source
-            dur_dead2buried = 2, # Add source
-            dur_symp2rec =   10, # Add source
-            dur_sev2rec =  10.4, # Add source
-            p_sev =         0.7, # Add source
-            p_death =      0.55, # Add source
-            p_safe_bury =  0.25, # Probability of a safe burial - should be linked to diagnoses
-
+        super().__init__()
+        self.default_pars(
             # Initial conditions and beta
-            init_prev = 0.005,
-            beta = None,
-            sev_factor = 2.2,
+            init_prev       = ss.bernoulli(p=0.005),
+            beta            = 1.0, # Placeholder value
+            sev_factor      = 2.2,
             unburied_factor = 2.1,
+            
+            # Natural history parameters, all specified in days
+            dur_exp2symp    = ss.lognorm_ex(mean=12.7), # Add source
+            dur_symp2sev    = ss.lognorm_ex(mean=6), # Add source
+            dur_sev2dead    = ss.lognorm_ex(mean=1.5), # Add source
+            dur_dead2buried = ss.lognorm_ex(mean=2), # Add source
+            dur_symp2rec    = ss.lognorm_ex(mean=10), # Add source
+            dur_sev2rec     = ss.lognorm_ex(mean=10.4), # Add source
+            p_sev           = ss.bernoulli(p=0.7), # Add source
+            p_death         = ss.bernoulli(p=0.55), # Add source
+            p_safe_bury     = ss.bernoulli(p=0.25), # Probability of a safe burial - should be linked to diagnoses
         )
-
-        par_dists = ss.omergeleft(par_dists,
-            dur_exp2symp    = ss.lognorm_ex,
-            dur_symp2sev    = ss.lognorm_ex,
-            dur_sev2dead    = ss.lognorm_ex,
-            dur_dead2buried = ss.lognorm_ex,
-            dur_symp2rec    = ss.lognorm_ex,
-            dur_sev2rec     = ss.lognorm_ex,
-            p_sev           = ss.bernoulli,
-            p_death         = ss.bernoulli,
-            p_safe_bury     = ss.bernoulli,
-            init_prev       = ss.bernoulli,
-        )
-
-        super().__init__(pars=pars, par_dists=par_dists, *args, **kwargs)
-
-        # Boolean states
+        self.update_pars(pars=pars, **kwargs)
         
+        # Boolean states
         self.add_states(
             # SIR are added automatically, here we add E
-            ss.State('exposed', bool, False),
-            ss.State('severe', bool, False),
-            ss.State('recovered', bool, False),
-            ss.State('buried', bool, False),
+            ss.BoolArr('exposed'),
+            ss.BoolArr('severe'),
+            ss.BoolArr('recovered'),
+            ss.BoolArr('buried'),
     
             # Timepoint states
-            ss.State('ti_exposed', float, np.nan),
-            ss.State('ti_severe', float, np.nan),
-            ss.State('ti_recovered', float, np.nan),
-            ss.State('ti_dead', float, np.nan),
-            ss.State('ti_buried', float, np.nan),
+            ss.FloatArr('ti_exposed'),
+            ss.FloatArr('ti_severe'),
+            ss.FloatArr('ti_recovered'),
+            ss.FloatArr('ti_dead'),
+            ss.FloatArr('ti_buried'),
         )
-
         return
 
     @property
     def infectious(self):
         return self.infected | self.exposed
 
-    def update_pre(self, sim):
+    def update_pre(self):
 
         # Progress exposed -> infected
-        infected = ss.true(self.exposed & (self.ti_infected <= sim.ti))
+        ti = self.sim.ti
+        infected = (self.exposed & (self.ti_infected <= ti)).uids
         self.exposed[infected] = False
         self.infected[infected] = True
 
         # Progress infectious -> severe
-        severe = ss.true(self.infected & (self.ti_severe <= sim.ti))
+        severe = (self.infected & (self.ti_severe <= ti)).uids
         self.severe[severe] = True
 
         # Progress infected -> recovered
-        recovered = ss.true(self.infected & (self.ti_recovered <= sim.ti))
+        recovered = (self.infected & (self.ti_recovered <= ti)).uids
         self.infected[recovered] = False
         self.recovered[recovered] = True
 
         # Progress severe -> recovered
-        recovered_sev = ss.true(self.severe & (self.ti_recovered <= sim.ti))
+        recovered_sev = (self.severe & (self.ti_recovered <= ti)).uids
         self.severe[recovered_sev] = False
         self.recovered[recovered_sev] = True
 
         # Trigger deaths
-        deaths = ss.true(self.ti_dead <= sim.ti)
+        deaths = (self.ti_dead <= ti).uids
         if len(deaths):
-            sim.people.request_death(deaths)
+            self.sim.people.request_death(deaths)
 
         # Progress dead -> buried
-        buried = ss.true(self.ti_buried <= sim.ti)
+        buried = (self.ti_buried <= ti).uids
         self.buried[buried] = True
         
         return
 
-    def set_prognoses(self, sim, uids, source_uids=None):
+    def set_prognoses(self, uids, source_uids=None):
         """ Set prognoses for those who get infected """
         # Do not call set_prognoses on the parent
         #super().set_prognoses(sim, uids, source_uids)
 
+        ti = self.sim.ti
+        dt = self.sim.dt
         self.susceptible[uids] = False
         self.exposed[uids] = True
-        self.ti_exposed[uids] = sim.ti
+        self.ti_exposed[uids] = ti
 
         p = self.pars
 
         # Determine when exposed become infected
-        self.ti_infected[uids] = sim.ti + p.dur_exp2symp.rvs(uids) / sim.dt
+        self.ti_infected[uids] = ti + p.dur_exp2symp.rvs(uids) / dt
 
         # Determine who progresses to sever and when
         sev_uids = p.p_sev.filter(uids)
-        self.ti_severe[sev_uids] = self.ti_infected[sev_uids] + p.dur_symp2sev.rvs(sev_uids) / sim.dt
+        self.ti_severe[sev_uids] = self.ti_infected[sev_uids] + p.dur_symp2sev.rvs(sev_uids) / dt
 
         # Determine who dies and who recovers and when
         dead_uids = p.p_death.filter(sev_uids)
-        self.ti_dead[dead_uids] = self.ti_severe[dead_uids] + p.dur_sev2dead.rvs(dead_uids) / sim.dt
+        self.ti_dead[dead_uids] = self.ti_severe[dead_uids] + p.dur_sev2dead.rvs(dead_uids) / dt
         rec_sev_uids = np.setdiff1d(sev_uids, dead_uids)
-        self.ti_recovered[rec_sev_uids] = self.ti_severe[rec_sev_uids] + p.dur_sev2rec.rvs(rec_sev_uids) / sim.dt
+        self.ti_recovered[rec_sev_uids] = self.ti_severe[rec_sev_uids] + p.dur_sev2rec.rvs(rec_sev_uids) / dt
         rec_symp_uids = np.setdiff1d(uids, sev_uids)
-        self.ti_recovered[rec_symp_uids] = self.ti_infected[rec_symp_uids] + p.dur_symp2rec.rvs(rec_symp_uids) / sim.dt
+        self.ti_recovered[rec_symp_uids] = self.ti_infected[rec_symp_uids] + p.dur_symp2rec.rvs(rec_symp_uids) / dt
 
         # Determine time of burial - either immediate (safe burials) or after a delay (unsafe)
         safe_buried = p.p_safe_bury.filter(dead_uids)
         unsafe_buried = np.setdiff1d(dead_uids, safe_buried)
         self.ti_buried[safe_buried] = self.ti_dead[safe_buried]
-        self.ti_buried[unsafe_buried] = self.ti_dead[unsafe_buried] + p.dur_dead2buried.rvs(unsafe_buried) / sim.dt
+        self.ti_buried[unsafe_buried] = self.ti_dead[unsafe_buried] + p.dur_dead2buried.rvs(unsafe_buried) / dt
 
         # Change rel_trans values
         self.rel_trans[self.infectious] = 1
         self.rel_trans[self.severe] = self.pars['sev_factor']  # Change for severe
-        unburied_uids = ss.true((self.ti_dead <= sim.ti) & (self.ti_buried > sim.ti))
+        unburied_uids = ((self.ti_dead <= ti) & (self.ti_buried > ti)).uids
         self.rel_trans[unburied_uids] = self.pars['unburied_factor']  # Change for unburied
-
         return
 
-    def update_death(self, sim, uids):
+    def update_death(self, uids):
         # Reset infected/recovered flags for dead agents
         for state in ['susceptible', 'exposed', 'infected', 'severe', 'recovered']:
             self.statesdict[state][uids] = False
         return
```

### Comparing `starsim-0.3.4/starsim/diseases/gonorrhea.py` & `starsim-0.5.0/starsim/diseases/gonorrhea.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,96 +1,84 @@
 """
 Define default gonorrhea disease module and related interventions
 """
 
 import numpy as np
 import starsim as ss
 
+
 __all__ = ['Gonorrhea']
 
 class Gonorrhea(ss.Infection):
 
-    def __init__(self, pars=None, par_dists=None, *args, **kwargs):
-
+    def __init__(self, pars=None, *args, **kwargs):
+        # Parameters
+        super().__init__()
+        self.default_pars(
+            beta = 1.0, # Placeholder value
+            dur_inf_in_days = ss.lognorm_ex(mean=10, stdev=0.6),  # median of 10 days (IQR 7–15 days) https://sti.bmj.com/content/96/8/556
+            p_symp    = ss.bernoulli(p=0.5),  # Share of infections that are symptomatic. Placeholder value
+            p_clear   = ss.bernoulli(p=0.2),  # Share of infections that spontaneously clear: https://sti.bmj.com/content/96/8/556
+            init_prev = ss.bernoulli(p=0.1),
+        )
+        self.update_pars(pars=pars, **kwargs)
+        
         # States additional to the default disease states (see base class)
         # Additional states dependent on parameter values, e.g. self.p_symp?
         # These might be useful for connectors to target, e.g. if HIV reduces p_clear
         self.add_states(
-            ss.State('symptomatic', bool, False),
-            ss.State('ti_clearance', int, ss.INT_NAN),
-            ss.State('p_symp', float, 1),
-        )
-
-        # Parameters
-        pars = ss.omergeleft(pars,
-            dur_inf_in_days = ss.lognorm_ex(mean=10, stdev=0.6),  # median of 10 days (IQR 7–15 days) https://sti.bmj.com/content/96/8/556
-            p_symp = 0.5,  # Share of infections that are symptomatic. Placeholder value
-            p_clear = 0.2,  # Share of infections that spontaneously clear: https://sti.bmj.com/content/96/8/556
-            init_prev = 0.1,
-        )
-
-        par_dists = ss.omergeleft(par_dists,
-            dur_inf_in_days = ss.lognorm_ex,
-            p_symp          = ss.bernoulli,
-            p_clear         = ss.bernoulli,
-            init_prev       = ss.bernoulli,
+            ss.BoolArr('symptomatic'),
+            ss.FloatArr('ti_clearance'),
+            ss.FloatArr('p_symp', default=1),
         )
-
-        super().__init__(pars=pars, par_dists=par_dists, *args, **kwargs)
+        
         return
 
-    def init_results(self, sim):
+    def init_results(self):
         """
         Initialize results
         """
-        super().init_results(sim)
-        self.results += ss.Result(self.name, 'new_clearances', sim.npts, dtype=int)
+        super().init_results()
+        self.results += ss.Result(self.name, 'new_clearances', self.sim.npts, dtype=int)
         return
 
-    def update_results(self, sim):
-        ti = sim.ti
-        super(Gonorrhea, self).update_results(sim)
+    def update_results(self):
+        super().update_results()
+        ti = self.sim.ti
         self.results.n_symptomatic[ti] = self.symptomatic.count()
         self.results.new_clearances[ti] = np.count_nonzero(self.ti_clearance == ti)
         return
 
-    def update_pre(self, sim):
+    def update_pre(self):
         # What if something in here should depend on another module?
         # I guess we could just check for it e.g., 'if HIV in sim.modules' or
         # 'if 'hiv' in sim.people' or something
         # Natural clearance
-        clearances = self.ti_clearance <= sim.ti
+        clearances = self.ti_clearance <= self.sim.ti
         self.susceptible[clearances] = True
         self.infected[clearances] = False
         self.symptomatic[clearances] = False
-        self.ti_clearance[clearances] = sim.ti
+        self.ti_clearance[clearances] = self.sim.ti
 
         return
-    
-    def make_new_cases(self, sim):
-        super(Gonorrhea, self).make_new_cases(sim)
-        return
 
-    def set_prognoses(self, sim, target_uids, source_uids=None):
+    def set_prognoses(self, target_uids, source_uids=None):
         """
         Natural history of gonorrhea for adult infection
         """
-        super().set_prognoses(sim, target_uids, source_uids)
+        super().set_prognoses(target_uids, source_uids)
+        ti = self.sim.ti
 
         # Set infection status
         self.susceptible[target_uids] = False
         self.infected[target_uids] = True
-        self.ti_infected[target_uids] = sim.ti
+        self.ti_infected[target_uids] = ti
 
         # Set infection status
         symp_uids = self.pars.p_symp.filter(target_uids)
         self.symptomatic[symp_uids] = True
 
         # Set natural clearance
         clear_uids = self.pars.p_clear.filter(target_uids)
-        dur = sim.ti + self.pars.dur_inf_in_days.rvs(clear_uids)/365/sim.dt # Convert from days to years and then adjust for dt
+        dur = ti + self.pars.dur_inf_in_days.rvs(clear_uids)/365/self.sim.dt # Convert from days to years and then adjust for dt
         self.ti_clearance[clear_uids] = dur
-
-        return
-
-    def set_congenital(self, sim, target_uids, source_uids=None):
-        pass
+        return
```

### Comparing `starsim-0.3.4/starsim/diseases/hiv.py` & `starsim-0.5.0/starsim/diseases/hiv.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,98 +2,86 @@
 Define default HIV disease module and related interventions
 """
 
 import numpy as np
 import sciris as sc
 import starsim as ss
 
+
 __all__ = ['HIV', 'ART', 'CD4_analyzer']
 
 class HIV(ss.Infection):
 
-    def __init__(self, pars=None, par_dists=None, *args, **kwargs):
-
-        # States
-        self.add_states(
-            ss.State('on_art', bool, False),
-            ss.State('ti_art', int, ss.INT_NAN),
-            ss.State('cd4', float, 500),
-            ss.State('ti_dead', int, ss.INT_NAN), # Time of HIV-cause death
-        )
-
-        pars = ss.omergeleft(pars,
+    def __init__(self, pars=None, *args, **kwargs):
+        super().__init__()
+        self.default_pars(
+            beta = 1.0, # Placeholder value
             cd4_min = 100,
             cd4_max = 500,
             cd4_rate = 5,
-            init_prev = 0.05,
             eff_condoms = 0.7,
             art_efficacy = 0.96,
-            death_prob = 0.05,
+            init_prev = ss.bernoulli(p=0.05),
+            death_dist = ss.bernoulli(p=self.death_prob_func), # Uses p_death by default, modulated by CD4
+            p_death = 0.05,
         )
+        self.update_pars(pars=pars, **kwargs)
 
-        par_dists = ss.omergeleft(par_dists,
-            init_prev  = ss.bernoulli,
-            death_prob = ss.bernoulli,
+        # States
+        self.add_states(
+            ss.BoolArr('on_art'),
+            ss.FloatArr('ti_art'),
+            ss.FloatArr('ti_dead'), # Time of HIV-cause death
+            ss.FloatArr('cd4', default=500),
         )
-
-        super().__init__(pars=pars, par_dists=par_dists, *args, **kwargs)
-        self.death_prob_data = sc.dcp(self.pars.death_prob)
-        self.pars.death_prob = self.make_death_prob
-
         return
 
     @staticmethod
-    def make_death_prob(module, sim, uids):
+    def death_prob_func(module, sim, uids):
         p = module.pars
-        out = sim.dt * module.death_prob_data / (p.cd4_min - p.cd4_max)**2 *  (module.cd4[uids] - p.cd4_max)**2
+        out = sim.dt * p.p_death / (p.cd4_min - p.cd4_max)**2 *  (module.cd4[uids] - p.cd4_max)**2
         out = np.array(out)
         return out
 
-    def update_pre(self, sim):
+    def update_pre(self):
         """ Update CD4 """
-        self.cd4[sim.people.alive & self.infected & self.on_art] += (self.pars.cd4_max - self.cd4[sim.people.alive & self.infected & self.on_art])/self.pars.cd4_rate
-        self.cd4[sim.people.alive & self.infected & ~self.on_art] += (self.pars.cd4_min - self.cd4[sim.people.alive & self.infected & ~self.on_art])/self.pars.cd4_rate
+        people = self.sim.people
+        self.cd4[people.alive & self.infected & self.on_art] += (self.pars.cd4_max - self.cd4[people.alive & self.infected & self.on_art])/self.pars.cd4_rate
+        self.cd4[people.alive & self.infected & ~self.on_art] += (self.pars.cd4_min - self.cd4[people.alive & self.infected & ~self.on_art])/self.pars.cd4_rate
 
-        self.rel_trans[sim.people.alive & self.infected & self.on_art] = 1 - self.pars['art_efficacy']
+        self.rel_trans[people.alive & self.infected & self.on_art] = 1 - self.pars['art_efficacy']
 
-        can_die = ss.true(sim.people.alive & sim.people.hiv.infected)
-        hiv_deaths = self.pars.death_prob.filter(can_die)
+        can_die = people.hiv.infected.uids
+        hiv_deaths = self.pars.death_dist.filter(can_die)
         
-        sim.people.request_death(hiv_deaths)
-        self.ti_dead[hiv_deaths] = sim.ti
+        people.request_death(hiv_deaths)
+        self.ti_dead[hiv_deaths] = self.sim.ti
         return
 
-    def init_results(self, sim):
-        """
-        Initialize results
-        """
-        super().init_results(sim)
-        self.results += ss.Result(self.name, 'new_deaths', sim.npts, dtype=int)
+    def init_results(self):
+        """ Initialize results """
+        super().init_results()
+        self.results += ss.Result(self.name, 'new_deaths', self.sim.npts, dtype=int)
         return
 
-    def update_results(self, sim):
-        super().update_results(sim)
-        self.results['new_deaths'][sim.ti] = np.count_nonzero(self.ti_dead == sim.ti)
+    def update_results(self):
+        super().update_results()
+        ti = self.sim.ti
+        self.results['new_deaths'][ti] = np.count_nonzero(self.ti_dead == ti)
         return 
 
-    def make_new_cases(self, sim):
-        # eff_condoms = sim.pars[self.name]['eff_condoms'] # TODO figure out how to add this
-        super().make_new_cases(sim)
-        return
-
-    def set_prognoses(self, sim, uids, source_uids=None):
-        super().set_prognoses(sim, uids, source_uids)
-
+    def set_prognoses(self, uids, source_uids=None):
+        super().set_prognoses(uids, source_uids)
         self.susceptible[uids] = False
         self.infected[uids] = True
-        self.ti_infected[uids] = sim.ti
+        self.ti_infected[uids] = self.sim.ti
         return
 
-    def set_congenital(self, sim, target_uids, source_uids):
-        return self.set_prognoses(sim, target_uids, source_uids)
+    def set_congenital(self, target_uids, source_uids):
+        return self.set_prognoses(target_uids, source_uids)
 
 
 # %% HIV-related interventions
 
 class ART(ss.Intervention):
 
     def __init__(self, year: np.array, coverage: np.array, **kwargs):
```

### Comparing `starsim-0.3.4/starsim/diseases/measles.py` & `starsim-0.5.0/starsim/diseases/measles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,94 @@
 """
 Define measles model.
 Adapted from https://github.com/optimamodel/gavi-outbreaks/blob/main/stisim/gavi/measles.py
 Original version by @alina-muellenmeister, @domdelport, and @RomeshA
 """
 
-import numpy as np
 import starsim as ss
 from starsim.diseases.sir import SIR
 
 __all__ = ['Measles']
 
 
 class Measles(SIR):
 
-    def __init__(self, pars=None, par_dists=None, *args, **kwargs):
+    def __init__(self, pars=None, *args, **kwargs):
         """ Initialize with parameters """
-
-        pars = ss.omergeleft(pars,
-            # Natural history parameters, all specified in days
-            dur_exp = 8,       # (days) - source: US CDC
-            dur_inf = 11,      # (days) - source: US CDC
-            p_death = 0.005,   # Probability of death
-
+        super().__init__()
+        self.default_pars(
             # Initial conditions and beta
-            init_prev = 0.005,
-            beta = None,
-        )
-
-        par_dists = ss.omergeleft(par_dists,
-            dur_exp   = ss.normal,
-            dur_inf   = ss.normal,
-            init_prev = ss.bernoulli,
-            p_death   = ss.bernoulli,
+            beta = 1.0, # Placeholder value
+            init_prev = ss.bernoulli(p=0.005),
+            
+            # Natural history parameters, all specified in days
+            dur_exp = ss.normal(loc=8),        # (days) - source: US CDC
+            dur_inf = ss.normal(loc=11),       # (days) - source: US CDC
+            p_death = ss.bernoulli(p=0.005), # Probability of death
         )
-
-        super().__init__(pars=pars, par_dists=par_dists, *args, **kwargs)
+        self.update_pars(pars=pars, **kwargs)
 
         # SIR are added automatically, here we add E
         self.add_states(
-            ss.State('exposed', bool, False),
-            ss.State('ti_exposed', float, np.nan),
+            ss.BoolArr('exposed'),
+            ss.FloatArr('ti_exposed'),
         )
 
         return
 
     @property
     def infectious(self):
         return self.infected | self.exposed
 
-    def update_pre(self, sim):
+    def update_pre(self):
         # Progress exposed -> infected
-        infected = ss.true(self.exposed & (self.ti_infected <= sim.ti))
+        ti = self.sim.ti
+        infected = (self.exposed & (self.ti_infected <= ti)).uids
         self.exposed[infected] = False
         self.infected[infected] = True
 
         # Progress infected -> recovered
-        recovered = ss.true(self.infected & (self.ti_recovered <= sim.ti))
+        recovered = (self.infected & (self.ti_recovered <= ti)).uids
         self.infected[recovered] = False
         self.recovered[recovered] = True
 
         # Trigger deaths
-        deaths = ss.true(self.ti_dead <= sim.ti)
+        deaths = (self.ti_dead <= ti).uids
         if len(deaths):
-            sim.people.request_death(deaths)
+            self.sim.people.request_death(deaths)
         return
 
-    def set_prognoses(self, sim, uids, source_uids=None):
+    def set_prognoses(self, uids, source_uids=None):
         """ Set prognoses for those who get infected """
         # Do not call set_prognosis on parent
         # super().set_prognoses(sim, uids, source_uids)
+        ti = self.sim.ti
+        dt = self.sim.dt
 
         self.susceptible[uids] = False
         self.exposed[uids] = True
-        self.ti_exposed[uids] = sim.ti
+        self.ti_exposed[uids] = ti
 
         p = self.pars
 
         # Determine when exposed become infected
-        self.ti_infected[uids] = sim.ti + p.dur_exp.rvs(uids) / sim.dt
+        self.ti_infected[uids] = ti + p.dur_exp.rvs(uids) / dt
 
         # Sample duration of infection, being careful to only sample from the
         # distribution once per timestep.
         dur_inf = p.dur_inf.rvs(uids)
 
         # Determine who dies and who recovers and when
         will_die = p.p_death.rvs(uids)
         dead_uids = uids[will_die]
         rec_uids = uids[~will_die]
-        self.ti_dead[dead_uids] = self.ti_infected[dead_uids] + dur_inf[will_die] / sim.dt
-        self.ti_recovered[rec_uids] = self.ti_infected[rec_uids] + dur_inf[~will_die] / sim.dt
+        self.ti_dead[dead_uids] = self.ti_infected[dead_uids] + dur_inf[will_die] / dt
+        self.ti_recovered[rec_uids] = self.ti_infected[rec_uids] + dur_inf[~will_die] / dt
 
         return
 
-    def update_death(self, sim, uids):
+    def update_death(self, uids):
         # Reset infected/recovered flags for dead agents
         for state in ['susceptible', 'exposed', 'infected', 'recovered']:
             self.statesdict[state][uids] = False
         return
```

### Comparing `starsim-0.3.4/starsim/diseases/ncd.py` & `starsim-0.5.0/starsim/diseases/ncd.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,86 +2,89 @@
 Define non-communicable disease (NCD) model
 """
 
 import numpy as np
 import starsim as ss
 import sciris as sc
 
+
 __all__ = ['NCD']
 
 class NCD(ss.Disease):
     """
     Example non-communicable disease
 
     This class implements a basic NCD model with risk of developing a condition
     (e.g., hypertension, diabetes), a state for having the condition, and associated
     mortality.
     """
-    def __init__(self, pars=None):
-        default_pars = dict(
+    def __init__(self, pars=None, **kwargs):
+        super().__init__()
+        self.default_pars(
             initial_risk = ss.bernoulli(p=0.3), # Initial prevalence of risk factors
-            #'affection_rate': ss.rate(p=0.1), # Instantaneous rate of acquisition applied to those at risk (units are acquisitions / year)
             dur_risk = ss.expon(scale=10),
             prognosis = ss.weibull(c=2, scale=5), # Time in years between first becoming affected and death
         )
-
-        super().__init__(ss.omerge(default_pars, pars))
+        self.update_pars(pars=pars, **kwargs)
+        
         self.add_states(
-            ss.State('at_risk', bool, False),
-            ss.State('affected', bool, False),
-            ss.State('ti_affected', int, ss.INT_NAN),
-            ss.State('ti_dead', int, ss.INT_NAN),
+            ss.BoolArr('at_risk'),
+            ss.BoolArr('affected'),
+            ss.FloatArr('ti_affected'),
+            ss.FloatArr('ti_dead'),
         )
         return
 
     @property
     def not_at_risk(self):
         return ~self.at_risk
 
-    def set_initial_states(self, sim):
+    def init_vals(self):
         """
         Set initial values for states. This could involve passing in a full set of initial conditions,
         or using init_prev, or other. Note that this is different to initialization of the State objects
         i.e., creating their dynamic array, linking them to a People instance. That should have already
         taken place by the time this method is called.
         """
-        alive_uids = ss.true(sim.people.alive)
-        initial_risk = self.pars['initial_risk'].filter(alive_uids)
+        super().init_vals()
+        initial_risk = self.pars['initial_risk'].filter()
         self.at_risk[initial_risk] = True
-        self.ti_affected[initial_risk] = sim.ti + sc.randround(self.pars['dur_risk'].rvs(initial_risk) / sim.dt)
+        self.ti_affected[initial_risk] = self.sim.ti + sc.randround(self.pars['dur_risk'].rvs(initial_risk) / self.sim.dt)
         return initial_risk
 
-    def update_pre(self, sim):
-        deaths = ss.true(self.ti_dead == sim.ti)
-        sim.people.request_death(deaths)
+    def update_pre(self):
+        ti = self.sim.ti
+        deaths = (self.ti_dead == ti).uids
+        self.sim.people.request_death(deaths)
         self.log.add_data(deaths, died=True)
-        self.results.new_deaths[sim.ti] = len(deaths) # Log deaths attributable to this module
+        self.results.new_deaths[ti] = len(deaths) # Log deaths attributable to this module
         return
 
-    def make_new_cases(self, sim):
-        new_cases = ss.true(self.ti_affected == sim.ti)
+    def make_new_cases(self):
+        ti = self.sim.ti
+        new_cases = (self.ti_affected == ti).uids
         self.affected[new_cases] = True
         prog_years = self.pars.prognosis.rvs(new_cases)
-        self.ti_dead[new_cases] = sim.ti + sc.randround(prog_years / sim.dt)
-        super().set_prognoses(sim, new_cases)
+        self.ti_dead[new_cases] = ti + sc.randround(prog_years / self.sim.dt)
+        super().set_prognoses(new_cases)
         return new_cases
 
-    def init_results(self, sim):
+    def init_results(self):
         """
         Initialize results
         """
-        super().init_results(sim)
+        super().init_results()
+        npts = self.sim.npts
         self.results += [
-            ss.Result(self.name, 'n_not_at_risk', sim.npts, dtype=int),
-            ss.Result(self.name, 'prevalence', sim.npts, dtype=float),
-            ss.Result(self.name, 'new_deaths', sim.npts, dtype=int),
+            ss.Result(self.name, 'n_not_at_risk', npts, dtype=int),
+            ss.Result(self.name, 'prevalence', npts, dtype=float),
+            ss.Result(self.name, 'new_deaths', npts, dtype=int),
         ]
         return
 
-    def update_results(self, sim):
-        super().update_results(sim)
-        ti = sim.ti
-        alive = sim.people.alive
-        self.results.n_not_at_risk[ti] = np.count_nonzero(self.not_at_risk & alive)
-        self.results.prevalence[ti]    = np.count_nonzero(self.affected & alive)/alive.count()
+    def update_results(self):
+        super().update_results()
+        ti = self.sim.ti
+        self.results.n_not_at_risk[ti] = np.count_nonzero(self.not_at_risk)
+        self.results.prevalence[ti]    = np.count_nonzero(self.affected)/len(self.sim.people)
         self.results.new_deaths[ti]    = np.count_nonzero(self.ti_dead == ti)
         return
```

### Comparing `starsim-0.3.4/starsim/diseases/sir.py` & `starsim-0.5.0/starsim/diseases/sir.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,82 +2,79 @@
 Define SIR and SIS disease modules
 """
 
 import numpy as np
 import matplotlib.pyplot as pl
 import starsim as ss
 
+
 __all__ = ['SIR', 'SIS']
 
 class SIR(ss.Infection):
     """
     Example SIR model
 
     This class implements a basic SIR model with states for susceptible,
     infected/infectious, and recovered. It also includes deaths, and basic
     results.
     """
-
-    def __init__(self, pars=None, par_dists=None, *args, **kwargs):
-        pars = ss.omergeleft(pars,
-            dur_inf = 6,
-            init_prev = 0.01,
-            p_death = 0.01,
+    def __init__(self, pars=None, **kwargs):
+        super().__init__()
+        self.default_pars(
             beta = 0.5,
+            init_prev = ss.bernoulli(p=0.01),
+            dur_inf = ss.lognorm_ex(mean=6),
+            p_death = ss.bernoulli(p=0.01),
         )
-
-        par_dists = ss.omergeleft(par_dists,
-            dur_inf   = ss.lognorm_ex,
-            init_prev = ss.bernoulli,
-            p_death   = ss.bernoulli,
-        )
-
-        super().__init__(pars=pars, par_dists=par_dists, *args, **kwargs)
+        self.update_pars(pars, **kwargs)
 
         self.add_states(
-            ss.State('recovered', bool, False),
-            ss.State('ti_recovered', int, ss.INT_NAN),
-            ss.State('ti_dead', int, ss.INT_NAN),
+            ss.BoolArr('recovered'),
+            ss.FloatArr('ti_recovered'),
+            ss.FloatArr('ti_dead'),
         )
         return
 
-    def update_pre(self, sim):
+    def update_pre(self):
         # Progress infectious -> recovered
-        recovered = ss.true(self.infected & (self.ti_recovered <= sim.ti))
+        sim = self.sim
+        recovered = (self.infected & (self.ti_recovered <= sim.ti)).uids
         self.infected[recovered] = False
         self.recovered[recovered] = True
 
         # Trigger deaths
-        deaths = ss.true(self.ti_dead <= sim.ti)
+        deaths = (self.ti_dead <= sim.ti).uids
         if len(deaths):
             sim.people.request_death(deaths)
         return
 
-    def set_prognoses(self, sim, uids, source_uids=None):
+    def set_prognoses(self, uids, source_uids=None):
         """ Set prognoses """
+        ti = self.sim.ti
+        dt = self.sim.dt
         self.susceptible[uids] = False
         self.infected[uids] = True
-        self.ti_infected[uids] = sim.ti
+        self.ti_infected[uids] = ti
 
         p = self.pars
 
         # Sample duration of infection, being careful to only sample from the
         # distribution once per timestep.
         dur_inf = p.dur_inf.rvs(uids)
 
         # Determine who dies and who recovers and when
         will_die = p.p_death.rvs(uids)
         dead_uids = uids[will_die]
         rec_uids = uids[~will_die]
-        self.ti_dead[dead_uids] = sim.ti + dur_inf[will_die] / sim.dt # Consider rand round, but not CRN safe
-        self.ti_recovered[rec_uids] = sim.ti + dur_inf[~will_die] / sim.dt
+        self.ti_dead[dead_uids] = ti + dur_inf[will_die] / dt # Consider rand round, but not CRN safe
+        self.ti_recovered[rec_uids] = ti + dur_inf[~will_die] / dt
 
         return
 
-    def update_death(self, sim, uids):
+    def update_death(self, uids):
         """ Reset infected/recovered flags for dead agents """
         self.susceptible[uids] = False
         self.infected[uids] = False
         self.recovered[uids] = False
         return
 
     def plot(self):
@@ -93,99 +90,91 @@
     """
     Example SIS model
 
     This class implements a basic SIS model with states for susceptible,
     infected/infectious, and back to susceptible based on waning immunity. There
     is no death in this case.
     """
-    def __init__(self, pars=None, par_dists=None, *args, **kwargs):
-        pars = ss.omergeleft(pars,
-            dur_inf = 10,
-            init_prev = 0.01,
+    def __init__(self, pars=None, *args, **kwargs):
+        super().__init__()
+        self.default_pars(
             beta = 0.05,
+            init_prev = ss.bernoulli(p=0.01),
+            dur_inf = ss.lognorm_ex(mean=10),
             waning = 0.05,
             imm_boost = 1.0,
         )
+        self.update_pars(pars=pars, *args, **kwargs)
 
-        par_dists = ss.omergeleft(par_dists,
-            dur_inf   = ss.lognorm_ex,
-            init_prev = ss.bernoulli,
-        )
-        
         self.add_states(
-            ss.State('ti_recovered', int, ss.INT_NAN),
-            ss.State('immunity', float, 0.0),
+            ss.FloatArr('ti_recovered'),
+            ss.FloatArr('immunity', default=0.0),
         )
-
-        super().__init__(pars=pars, par_dists=par_dists, *args, **kwargs)
         return
 
-    def update_pre(self, sim):
+    def update_pre(self):
         """ Progress infectious -> recovered """
-        recovered = ss.true(self.infected & (self.ti_recovered <= sim.ti))
+        recovered = (self.infected & (self.ti_recovered <= self.sim.ti)).uids
         self.infected[recovered] = False
         self.susceptible[recovered] = True
-        self.update_immunity(sim)
+        self.update_immunity()
         return
     
-    def update_immunity(self, sim):
-        uids = ss.true(self.immunity > 0)
-        self.immunity[uids] = (self.immunity[uids])*(1 - self.pars.waning*sim.dt)
-        self.rel_sus[uids] = np.maximum(0, 1 - self.immunity[uids])
+    def update_immunity(self):
+        has_imm = (self.immunity > 0).uids
+        self.immunity[has_imm] = (self.immunity[has_imm])*(1 - self.pars.waning*self.sim.dt)
+        self.rel_sus[has_imm] = np.maximum(0, 1 - self.immunity[has_imm])
         return
 
-    def set_prognoses(self, sim, uids, source_uids=None):
+    def set_prognoses(self, uids, source_uids=None):
         """ Set prognoses """
         self.susceptible[uids] = False
         self.infected[uids] = True
-        self.ti_infected[uids] = sim.ti
+        self.ti_infected[uids] = self.sim.ti
         self.immunity[uids] += self.pars.imm_boost
 
         # Sample duration of infection
         dur_inf = self.pars.dur_inf.rvs(uids)
 
         # Determine when people recover
-        self.ti_recovered[uids] = sim.ti + dur_inf / sim.dt
+        self.ti_recovered[uids] = self.sim.ti + dur_inf / self.sim.dt
 
         return
     
-    def init_results(self, sim):
+    def init_results(self):
         """ Initialize results """
-        super().init_results(sim)
-        self.results += ss.Result(self.name, 'rel_sus', sim.npts, dtype=float)
+        super().init_results()
+        self.results += ss.Result(self.name, 'rel_sus', self.sim.npts, dtype=float)
         return
 
-    def update_results(self, sim):
+    def update_results(self):
         """ Store the population immunity (susceptibility) """
-        super().update_results(sim)
-        self.results['rel_sus'][sim.ti] = self.rel_sus.mean()
+        super().update_results()
+        self.results['rel_sus'][self.sim.ti] = self.rel_sus.mean()
         return 
 
     def plot(self):
         """ Default plot for SIS model """
         fig = pl.figure()
         for rkey in ['susceptible', 'infected']:
             pl.plot(self.results['n_'+rkey], label=rkey.title())
         pl.legend()
         return fig
 
 
 # %% Interventions
-__all__ += ['sir_vaccine']
 
+__all__ += ['sir_vaccine']
 
 class sir_vaccine(ss.Vx):
     """
     Create a vaccine product that changes susceptible people to recovered (i.e., perfect immunity)
     """
-    def __init__(self, pars=None, par_dists=None, *args, **kwargs):
-        pars = ss.omerge({
-            'efficacy': 0.9,
-        }, pars)
-
-        super().__init__(pars=pars, *args, **kwargs)
-
+    def __init__(self, pars=None, *args, **kwargs):
+        super().__init__()
+        self.default_pars(efficacy=0.9)
+        self.update_pars(pars, **kwargs)
         return
 
     def administer(self, people, uids):
         people.sir.rel_sus[uids] *= 1-self.pars.efficacy
         return
```

### Comparing `starsim-0.3.4/starsim/diseases/syphilis.py` & `starsim-0.5.0/starsim/diseases/syphilis.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,51 +3,27 @@
 """
 
 import numpy as np
 import sciris as sc
 from sciris import randround as rr # Since used frequently
 import starsim as ss
 
+
 __all__ = ['Syphilis']
 
 class Syphilis(ss.Infection):
 
-    def __init__(self, pars=None):
-        super().__init__(pars)
-
-        self.add_states(
-            # Adult syphilis states
-            ss.State('exposed', bool, False),  # AKA incubating. Free of symptoms, not transmissible
-            ss.State('primary', bool, False),  # Primary chancres
-            ss.State('secondary', bool, False),  # Inclusive of those who may still have primary chancres
-            ss.State('latent_temp', bool, False),  # Relapses to secondary (~1y)
-            ss.State('latent_long', bool, False),  # Can progress to tertiary or remain here
-            ss.State('tertiary', bool, False),  # Includes complications (cardio/neuro/disfigurement)
-            ss.State('immune', bool, False),  # After effective treatment people may acquire temp immunity
-            ss.State('ever_exposed', bool, False),  # Anyone ever exposed - stays true after treatment
-    
-            # Congenital syphilis states
-            ss.State('congenital', bool, False),
-    
-            # Timestep of state changes
-            ss.State('ti_exposed', int, ss.INT_NAN),
-            ss.State('ti_primary', int, ss.INT_NAN),
-            ss.State('ti_secondary', int, ss.INT_NAN),
-            ss.State('ti_latent_temp', int, ss.INT_NAN),
-            ss.State('ti_latent_long', int, ss.INT_NAN),
-            ss.State('ti_tertiary', int, ss.INT_NAN),
-            ss.State('ti_immune', int, ss.INT_NAN),
-            ss.State('ti_miscarriage', int, ss.INT_NAN),
-            ss.State('ti_nnd', int, ss.INT_NAN),
-            ss.State('ti_stillborn', int, ss.INT_NAN),
-            ss.State('ti_congenital', int, ss.INT_NAN),
-        )
-
+    def __init__(self, pars=None, **kwargs):
         # Parameters
-        default_pars = dict(
+        super().__init__()
+        self.default_pars(
+            # Initial conditions
+            beta = 1.0, # Placeholder
+            init_prev = ss.bernoulli(p=0.03),
+            
             # Adult syphilis natural history, all specified in years
             dur_exposed = ss.lognorm_ex(mean=1 / 12, stdev=1 / 36),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
             dur_primary = ss.lognorm_ex(mean=1.5 / 12, stdev=1 / 36),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
             dur_secondary = ss.normal(loc=3.6 / 12, scale=1.5 / 12),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
             dur_latent_temp = ss.lognorm_ex(mean=1, stdev=6 / 12),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
             dur_latent_long = ss.lognorm_ex(mean=20, stdev=8),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
             p_latent_temp = ss.bernoulli(p=0.25),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
@@ -66,24 +42,47 @@
             # Congenital syphilis outcomes
             # Birth outcomes coded as:
             #   0: Neonatal death
             #   1: Stillborn
             #   2: Congenital syphilis
             #   3: Live birth without syphilis-related complications
             # Source: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5973824/)
-            birth_outcomes=sc.objdict(
+            birth_outcomes = sc.objdict(
                 active = ss.choice(a=5, p=np.array([0.125, 0.125, 0.20, 0.35, 0.200])), # Probabilities of active by birth outcome
                 latent = ss.choice(a=5, p=np.array([0.050, 0.075, 0.10, 0.05, 0.725])), # Probabilities of latent
             ),
-            birth_outcome_keys=['miscarriage', 'nnd', 'stillborn', 'congenital'],
+            birth_outcome_keys = ['miscarriage', 'nnd', 'stillborn', 'congenital'],
+        )
+        self.update_pars(pars, **kwargs)
 
-            # Initial conditions
-            init_prev=ss.bernoulli(p=0.03),
+        self.add_states(
+            # Adult syphilis states
+            ss.BoolArr('exposed'),  # AKA incubating. Free of symptoms, not transmissible
+            ss.BoolArr('primary'),  # Primary chancres
+            ss.BoolArr('secondary'),  # Inclusive of those who may still have primary chancres
+            ss.BoolArr('latent_temp'),  # Relapses to secondary (~1y)
+            ss.BoolArr('latent_long'),  # Can progress to tertiary or remain here
+            ss.BoolArr('tertiary'),  # Includes complications (cardio/neuro/disfigurement)
+            ss.BoolArr('immune'),  # After effective treatment people may acquire temp immunity
+            ss.BoolArr('ever_exposed'),  # Anyone ever exposed - stays true after treatment
+            ss.BoolArr('congenital'),  # Congenital syphilis states
+    
+            # Timestep of state changes
+            ss.FloatArr('ti_exposed'),
+            ss.FloatArr('ti_primary'),
+            ss.FloatArr('ti_secondary'),
+            ss.FloatArr('ti_latent_temp'),
+            ss.FloatArr('ti_latent_long'),
+            ss.FloatArr('ti_tertiary'),
+            ss.FloatArr('ti_immune'),
+            ss.FloatArr('ti_miscarriage'),
+            ss.FloatArr('ti_nnd'),
+            ss.FloatArr('ti_stillborn'),
+            ss.FloatArr('ti_congenital'),
         )
-        self.pars = ss.omerge(default_pars, self.pars) # NB: regular omerge rather than omergeleft
 
         return
 
     @property
     def naive(self):
         """ Never exposed """
         return ~self.ever_exposed
@@ -104,187 +103,187 @@
         return self.latent_temp | self.latent_long
 
     @property
     def infectious(self):
         """ Infectious """
         return self.active | self.latent | self.exposed
 
-    def init_results(self, sim):
+    def init_results(self):
         """ Initialize results """
-        super().init_results(sim)
+        super().init_results()
+        npts = self.sim.npts
         self.results += [
-            ss.Result(self.name, 'new_nnds',       sim.npts, dtype=int, scale=True),
-            ss.Result(self.name, 'new_stillborns', sim.npts, dtype=int, scale=True),
-            ss.Result(self.name, 'new_congenital', sim.npts, dtype=int, scale=True),
+            ss.Result(self.name, 'new_nnds',       npts, dtype=int, scale=True),
+            ss.Result(self.name, 'new_stillborns', npts, dtype=int, scale=True),
+            ss.Result(self.name, 'new_congenital', npts, dtype=int, scale=True),
         ]
         return
 
-    def update_pre(self, sim):
+    def update_pre(self):
         """ Updates prior to interventions """
 
         # Primary
-        primary = self.exposed & (self.ti_primary <= sim.ti)
+        ti = self.sim.ti
+        primary = self.exposed & (self.ti_primary <= ti)
         self.primary[primary] = True
         self.exposed[primary] = False
         self.rel_trans[primary] = self.pars.rel_trans['primary']
 
         # Secondary from primary
-        secondary_from_primary = self.primary & (self.ti_secondary <= sim.ti)
-        if len(ss.true(secondary_from_primary)) > 0:
+        secondary_from_primary = (self.primary & (self.ti_secondary <= ti)).uids
+        if len(secondary_from_primary) > 0:
             self.secondary[secondary_from_primary] = True
             self.primary[secondary_from_primary] = False
-            self.set_secondary_prognoses(sim, ss.true(secondary_from_primary))
+            self.set_secondary_prognoses(secondary_from_primary)
             self.rel_trans[secondary_from_primary] = self.pars.rel_trans['secondary']
 
         # Hack to reset the MultiRNGs in set_secondary_prognoses so that they can be called again in this timestep. TODO: Refactor
-        self.pars.p_latent_temp.jump(sim.ti+1)
-        self.pars.dur_secondary.jump(sim.ti+1)
+        self.pars.p_latent_temp.jump(ti+1)
+        self.pars.dur_secondary.jump(ti+1)
 
         # Secondary reactivation from latent
-        secondary_from_latent = self.latent_temp & (self.ti_secondary <= sim.ti)
-        if len(ss.true(secondary_from_latent)) > 0:
+        secondary_from_latent = (self.latent_temp & (self.ti_secondary <= ti)).uids
+        if len(secondary_from_latent) > 0:
             self.secondary[secondary_from_latent] = True
             self.latent_temp[secondary_from_latent] = False
-            self.set_secondary_prognoses(sim, ss.true(secondary_from_latent))
+            self.set_secondary_prognoses(secondary_from_latent)
             self.rel_trans[secondary_from_latent] = self.pars.rel_trans['secondary']
 
         # Latent
-        latent_temp = self.secondary & (self.ti_latent_temp <= sim.ti)
-        if len(ss.true(latent_temp)) > 0:
+        latent_temp = (self.secondary & (self.ti_latent_temp <= ti)).uids
+        if len(latent_temp) > 0:
             self.latent_temp[latent_temp] = True
             self.secondary[latent_temp] = False
-            self.set_latent_temp_prognoses(sim, ss.true(latent_temp))
+            self.set_latent_temp_prognoses(latent_temp)
             self.rel_trans[latent_temp] = self.pars.rel_trans['latent_temp']
 
         # Latent long
-        latent_long = self.secondary & (self.ti_latent_long <= sim.ti)
-        if len(ss.true(latent_long)) > 0:
+        latent_long = (self.secondary & (self.ti_latent_long <= ti)).uids
+        if len(latent_long) > 0:
             self.latent_long[latent_long] = True
             self.secondary[latent_long] = False
-            self.set_latent_long_prognoses(sim, ss.true(latent_long))
+            self.set_latent_long_prognoses(latent_long)
             self.rel_trans[latent_long] = self.pars.rel_trans['latent_long']
 
         # Tertiary
-        tertiary = self.latent_long & (self.ti_tertiary <= sim.ti)
+        tertiary = (self.latent_long & (self.ti_tertiary <= ti)).uids
         self.tertiary[tertiary] = True
         self.latent_long[tertiary] = False
         self.rel_trans[tertiary] = self.pars.rel_trans['tertiary']
 
         # Congenital syphilis deaths
-        nnd = self.ti_nnd == sim.ti
-        stillborn = self.ti_stillborn == sim.ti
-        sim.people.request_death(nnd)
-        sim.people.request_death(stillborn)
+        nnd = (self.ti_nnd == ti).uids
+        stillborn = (self.ti_stillborn == ti).uids
+        self.sim.people.request_death(nnd)
+        self.sim.people.request_death(stillborn)
 
         # Congenital syphilis transmission outcomes
-        congenital = self.ti_congenital == sim.ti
+        congenital = self.ti_congenital == ti
         self.congenital[congenital] = True
         self.susceptible[congenital] = False
 
         return
 
-    def update_results(self, sim):
-        super(Syphilis, self).update_results(sim)
-        ti = sim.ti
+    def update_results(self):
+        super().update_results()
+        ti = self.sim.ti
         self.results.new_nnds[ti]       = np.count_nonzero(self.ti_nnd == ti)
         self.results.new_stillborns[ti] = np.count_nonzero(self.ti_stillborn == ti)
         self.results.new_congenital[ti] = np.count_nonzero(self.ti_congenital == ti)
         return
 
-    def make_new_cases(self, sim):
-        super(Syphilis, self).make_new_cases(sim)
-        return
-
-    def set_prognoses(self, sim, uids, source_uids=None):
+    def set_prognoses(self, uids, source_uids=None):
         """
         Set initial prognoses for adults newly infected with syphilis
         """
+        
+        ti = self.sim.ti
+        dt = self.sim.dt
 
         self.susceptible[uids] = False
         self.ever_exposed[uids] = True
         self.exposed[uids] = True
         self.infected[uids] = True
-        self.ti_exposed[uids] = sim.ti
-        self.ti_infected[uids] = sim.ti
+        self.ti_exposed[uids] = ti
+        self.ti_infected[uids] = ti
 
         # Set future dates and probabilities
         # Exposed to primary
         dur_exposed = self.pars.dur_exposed.rvs(uids)
-        self.ti_primary[uids] = sim.ti + rr(dur_exposed / sim.dt)
+        self.ti_primary[uids] = ti + rr(dur_exposed / dt)
 
         # Primary to secondary
         dur_primary = self.pars.dur_primary.rvs(uids)
-        self.ti_secondary[uids] = self.ti_primary[uids] + rr(dur_primary / sim.dt)
-
+        self.ti_secondary[uids] = self.ti_primary[uids] + rr(dur_primary / dt)
         return
 
-    def set_secondary_prognoses(self, sim, uids):
+    def set_secondary_prognoses(self, uids):
         """ Set prognoses for people who have just progressed to secondary infection """
 
+        dt = self.sim.dt
         dur_secondary = self.pars.dur_secondary.rvs(uids)
 
         # Secondary to latent_temp or latent_long
         latent_temp = self.pars.p_latent_temp.rvs(uids)
         latent_temp_uids = uids[latent_temp]
         latent_long_uids = uids[~latent_temp]
 
         dur_secondary_temp = dur_secondary[latent_temp]
-        self.ti_latent_temp[latent_temp_uids] = self.ti_secondary[latent_temp_uids] + rr(dur_secondary_temp / sim.dt)
+        self.ti_latent_temp[latent_temp_uids] = self.ti_secondary[latent_temp_uids] + rr(dur_secondary_temp / dt)
 
         dur_secondary_long = dur_secondary[~latent_temp]
-        self.ti_latent_long[latent_long_uids] = self.ti_secondary[latent_long_uids] + rr(dur_secondary_long / sim.dt)
+        self.ti_latent_long[latent_long_uids] = self.ti_secondary[latent_long_uids] + rr(dur_secondary_long / dt)
 
         return
 
-    def set_latent_temp_prognoses(self, sim, uids):
+    def set_latent_temp_prognoses(self, uids):
         # Primary to secondary
         dur_latent_temp = self.pars.dur_latent_temp.rvs(uids)
-        self.ti_secondary[uids] = self.ti_latent_temp[uids] + rr(dur_latent_temp / sim.dt)
+        self.ti_secondary[uids] = self.ti_latent_temp[uids] + rr(dur_latent_temp / self.sim.dt)
         return
 
-    def set_latent_long_prognoses(self, sim, uids):
-
+    def set_latent_long_prognoses(self, uids):
+        dt = self.sim.dt
         dur_latent = self.pars.dur_latent_long.rvs(uids)
 
         # Primary to secondary
         dur_latent_long = dur_latent
-        self.ti_secondary[uids] = self.ti_latent_temp[uids] + rr(dur_latent_long / sim.dt)
+        self.ti_secondary[uids] = self.ti_latent_temp[uids] + rr(dur_latent_long / dt)
 
         # Latent_long to tertiary
         tertiary = self.pars.p_tertiary.rvs(uids)
         tertiary_uids = uids[tertiary]
-        self.ti_tertiary[tertiary_uids] = self.ti_latent_long[tertiary_uids] + rr(dur_latent_long[tertiary] / sim.dt)
+        self.ti_tertiary[tertiary_uids] = self.ti_latent_long[tertiary_uids] + rr(dur_latent_long[tertiary] / dt)
 
         return
 
-    def set_congenital(self, sim, target_uids, source_uids=None):
-        """
-        Natural history of syphilis for congenital infection
-        """
+    def set_congenital(self, target_uids, source_uids=None):
+        """ Natural history of syphilis for congenital infection """
+        sim = self.sim
 
         # Determine outcomes
         for state in ['active', 'latent']:
 
-            source_state_inds = getattr(self, state)[source_uids].values.nonzero()[-1]
+            source_state_inds = getattr(self, state)[source_uids].nonzero()[0]
             uids = target_uids[source_state_inds]
 
             if len(uids) > 0:
 
                 # Birth outcomes must be modified to add probability of susceptible birth
                 birth_outcomes = self.pars.birth_outcomes[state]
                 assigned_outcomes = birth_outcomes.rvs(len(uids))
-                time_to_birth = -sim.people.age
+                time_to_birth = -sim.people.age.raw # TODO: make nicer
 
                 # Schedule events
                 for oi, outcome in enumerate(self.pars.birth_outcome_keys):
                     o_uids = uids[assigned_outcomes == oi]
                     if len(o_uids) > 0:
                         ti_outcome = f'ti_{outcome}'
                         vals = getattr(self, ti_outcome)
-                        vals[o_uids] = sim.ti + rr(time_to_birth[o_uids].values / sim.dt)
+                        vals[o_uids] = sim.ti + rr(time_to_birth[o_uids] / sim.dt)
                         setattr(self, ti_outcome, vals)
 
         return
 
 
 # %% Syphilis-related interventions
 
@@ -338,15 +337,15 @@
         """
         Return an array of indices of agents eligible for screening at time t, i.e. sexually active
         females in age range, plus any additional user-defined eligibility
         """
         if self.eligibility is not None:
             is_eligible = self.eligibility(sim)
         else:
-            is_eligible = sim.people.alive  # Probably not required
+            is_eligible = sim.people.auids  # Probably not required
         return is_eligible
 
     def initialize(self, sim):
         super().initialize(sim)
         self.results += [
             ss.Result('syphilis', 'n_screened', sim.npts, dtype=int, scale=True),
             ss.Result('syphilis', 'n_dx', sim.npts, dtype=int, scale=True),
@@ -374,9 +373,7 @@
         self.results += ss.Result('syphilis', 'n_tx', sim.npts, dtype=int, scale=True)
         return
 
     def apply(self, sim):
         treat_inds = super().apply(sim)
         sim.people.syphilis.infected[treat_inds] = False
         self.results['n_tx'][sim.ti] += len(treat_inds)
-
-
```

### Comparing `starsim-0.3.4/starsim/distributions.py` & `starsim-0.5.0/starsim/distributions.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,63 +4,95 @@
 
 import numpy as np
 import sciris as sc
 import scipy.stats as sps
 import starsim as ss
 import matplotlib.pyplot as pl
 
-__all__ = ['find_dists', 'dist_list', 'Dists', 'Dist']
+__all__ = ['find_dists', 'link_dists', 'make_dist', 'dist_list', 'Dists', 'Dist']
 
 
 def str2int(string, modulo=1_000_000):
     """
     Convert a string to an int
     
     Cannot use Python's built-in hash() since it's randomized for strings, but
     this is almost as fast (and 5x faster than hashlib).
     """
     return int.from_bytes(string.encode(), byteorder='big') % modulo
 
 
-def find_dists(obj, verbose=False):
+def find_dists(obj, verbose=False, **kwargs):
     """ Find all Dist objects in a parent object """
     out = sc.objdict()
-    tree = sc.iterobj(obj, depthfirst=False, flatten=True)
+    tree = sc.iterobj(obj, depthfirst=False, flatten=True, **kwargs)
     if verbose: print(f'Found {len(tree)} objects')
     for trace,val in tree.items():
         if isinstance(val, Dist):
             out[trace] = val
             if verbose: print(f'  {trace} is a dist ({len(out)})')
     return out
 
 
+def link_dists(obj, sim, module=None, overwrite=False, init=False, **kwargs):
+    """ Link distributions to the sim and the module; used in module.initialize() and people.initialize() """
+    if module is None and isinstance(obj, ss.Module):
+        module = obj
+    dists = ss.find_dists(obj, **kwargs) # Important that this comes first, before the sim is linked to the dist!
+    for key,val in dists.items():
+        if isinstance(val, ss.Dist):
+            val.link_sim(sim, overwrite=overwrite)
+            val.link_module(module, overwrite=overwrite)
+            if init: # Usually this is false since usually these are initialized centrally by the sim
+                val.initialize()
+    return
+
+
+def make_dist(pars=None, **kwargs):
+    """ Make a distribution from a dictionary """
+    pars = sc.mergedicts(pars, kwargs)
+    if 'type' not in pars:
+        errormsg = 'To make a distribution from a dict, one of the keys must be "type" to specify the distribution'
+        raise ValueError(errormsg)
+    dist_type = pars.pop('type')
+    if dist_type not in dist_list:
+        errormsg = f'"{dist_type}" is not a valid distribution; valid types are {dist_list}'
+        raise AttributeError(errormsg)
+    dist_class = getattr(ss, dist_type)
+    dist = dist_class(**pars) # Actually create the distribution
+    return dist
+
+
 class Dists(sc.prettyobj):
     """ Class for managing a collection of Dist objects """
-
     def __init__(self, obj=None, *args, base_seed=None, sim=None):
         if len(args): obj = [obj] + list(args)
         self.obj = obj
         self.dists = None
         self.base_seed = base_seed
+        if sim is None and obj is not None and isinstance(obj, ss.Sim):
+            sim = obj
         self.sim = sim
         self.initialized = False
-        if self.obj is not None:
-            self.initialize()
         return
 
     def initialize(self, obj=None, base_seed=None, sim=None, force=False):
         """
         Set the base seed, find and initialize all distributions in an object
         
         In practice, the object is usually a Sim, but can be anything.
         """
         if base_seed:
             self.base_seed = base_seed
         sim = sim if (sim is not None) else self.sim
         obj = obj if (obj is not None) else self.obj
+        if sim is None and obj is not None and isinstance(obj, ss.Sim):
+            sim = obj
+        if obj is None and sim is not None:
+            obj = sim
         if obj is None:
             errormsg = 'Must supply a container that contains one or more Dist objects, typically the sim'
             raise ValueError(errormsg)
         self.dists = find_dists(obj)
         for trace,dist in self.dists.items():
             if not dist.initialized or force:
                 dist.initialize(trace=trace, seed=base_seed, sim=sim, force=force)
@@ -95,15 +127,15 @@
         """ Reset each RNG """
         out = sc.autolist()
         for dist in self.dists.values():
             out += dist.reset()
         return out
 
 
-class Dist: # TODO: figure out why subclassing sc.prettyobj breaks isinstance
+class Dist:
     """
     Base class for tracking one random number generator associated with one distribution,
     i.e. one decision per timestep.
     
     See ss.dist_list for a full list of supported distributions.
     
     Although it's possible in theory to define a custom distribution (i.e., not
@@ -207,19 +239,27 @@
             print(s)
             return
     
     def __call__(self, n=1):
         """ Alias to self.rvs() """
         return self.rvs(n=n)
     
-    def set(self, dist=None, **kwargs):
+    def set(self, *args, dist=None, **kwargs):
         """ Set (change) the distribution type, or one or more parameters of the distribution """
         if dist:
             self.dist = dist
             self.process_dist()
+        if args:
+            if kwargs:
+                errormsg = f'You can supply args or kwargs, but not both (args={len(args)}, kwargs={len(kwargs)})'
+                raise ValueError(errormsg)
+            else: # Convert from args to kwargs
+                parkeys = list(self.pars.keys())
+                for i,arg in enumerate(args):
+                    kwargs[parkeys[i]] = arg
         if kwargs:
             self.pars.update(kwargs)
             self.process_pars(call=False)
         return
 
     @property
     def bitgen(self):
@@ -302,35 +342,52 @@
         if ss.options._centralized:
             self.rng = np.random.mtrand._rand # If _centralized, return the centralized numpy random number instance
         else:
             self.rng = np.random.default_rng(seed=self.seed)
         self.make_history(reset=True)
         
         # Handle the sim, module, and slots
-        self.sim = sim if (sim is not None) else self.sim
-        self.module = module if (module is not None) else self.module
+        self.link_sim(sim)
+        self.link_module(module)
         if slots is None and self.sim is not None:
             try:
                 slots = self.sim.people.slot
             except Exception as E:
                 warnmsg = f'Could not extract slots from sim object, is this an error?\n{E}'
                 ss.warn(warnmsg)
         if slots is not None:
             self.slots = slots
             
         # Initialize the distribution and finalize
         self.process_dist()
         self.process_pars(call=False)
         self.ready = True
-        if self.trace is None or self.sim is None or self.slots is None:
-            self.initialized = 'partial' # Initialized enough to produce random numbers, but not fully initialized
+        none_dict = dict(trace=self.trace, sim=self.sim, slots=self.slots)
+        none_dict = {k:v for k,v in none_dict.items() if v is None}
+        if len(none_dict):
+            self.initialized = 'partial'
+            if self.strict:
+                errormsg = f'Distribution {self} is not fully initialized, the following inputs are None:\n{none_dict.keys()}\nThis distribution may not produce valid random numbers.'
+                raise RuntimeError(errormsg)
         else:
             self.initialized = True
         return self
     
+    def link_sim(self, sim=None, overwrite=False):
+        """ Shortcut for linking the sim, only overwriting an existing one if overwrite=True """
+        if (not self.sim or overwrite) and sim is not None:
+            self.sim = sim
+        return
+    
+    def link_module(self, module=None, overwrite=False):
+        """ Shortcut for linking the module """
+        if (not self.module or overwrite) and module is not None:
+            self.module = module
+        return
+    
     def process_seed(self, trace=None, seed=None):
         """ Obtain the seed offset by hashing the path to this distribution; called automatically """
         unique_name = trace or self.trace or self.name
         if unique_name:
             if not self.name:
                 self.name = unique_name
             self.trace = unique_name
@@ -368,15 +425,15 @@
     def process_size(self, n=1):
         """ Handle an input of either size or UIDs and calculate size, UIDs, and slots """
         if np.isscalar(n) or isinstance(n, tuple):  # If passing a non-scalar size, interpret as dimension rather than UIDs iff a tuple
             uids = None
             slots = None
             size = n
         else:
-            uids = np.asarray(n)
+            uids = ss.uids(n)
             if len(uids):
                 slots = self.slots[uids]
                 if len(slots): # Handle case where uids is boolean
                     size = slots.max() + 1
                 else:
                     size = 0
             else:
@@ -455,34 +512,37 @@
     
     def rvs(self, n=1, reset=False):
         """
         Get random variables
         
         Args:
             n (int/tuple/arr): if an int or tuple, return this many random variables; if an array, treat as UIDs
+            reset (bool): whether to automatically reset the random number distribution state after being called
         """
         # Check for readiness
         if not self.initialized:
             raise DistNotInitializedError(self)
         if not self.ready and self.strict and not ss.options._centralized:
             raise DistNotReadyError(self)
         
         # Figure out size, UIDs, and slots
         size, slots = self.process_size(n)
         
         # Check if size is 0, then we can return
         if size == 0:
             return np.array([], dtype=int) # int dtype allows use as index, e.g. when filtering
+        elif isinstance(size, ss.uids) and self.initialized == 'partial': # This point can be reached if and only if strict=False and UIDs are used as input
+            errormsg = f'Distribution {self} is only partially initialized; cannot generate random numbers to match UIDs'
+            raise ValueError(errormsg)
         
         # Store the state
         self.make_history() # Store the pre-call state
         
         # Check if any keywords are callable -- parameters shouldn't need to be reprocessed otherwise
-        if True: # self.dynamic_pars: # TODO: fix!!!!
-            self.process_pars()
+        self.process_pars()
         
         # Actually get the random numbers
         if self.dynamic_pars:
             rands = self.rand(size)[slots] # Get random values 
             rvs = self.ppf(rands) # Convert to actual values via the PPF
         else:
             rvs = self.make_rvs() # Or, just get regular values
@@ -696,22 +756,28 @@
         rvs = self.rng.random(self._size) < self._pars.p # 3x faster than using rng.binomial(1, p, size)
         return rvs
     
     def ppf(self, rands):
         rvs = rands < self._pars.p
         return rvs
     
-    def filter(self, uids, both=False):
+    def filter(self, uids=None, both=False):
         """ Return UIDs that correspond to True, or optionally return both True and False """
+        if uids is None:
+            uids = self.sim.people.auids # All active UIDs
         bools = self.rvs(uids)
         if both:
             return uids[bools], uids[~bools]
         else:
             return uids[bools]
 
+    def split(self, uids=None):
+        """ Alias to filter(uids, both=True) """
+        return self.filter(uids=uids, both=True)
+
 
 class choice(Dist):
     """
     Random choice between discrete options
     
     **Examples**::
         
@@ -740,19 +806,24 @@
 #%% Dist exceptions
 
 class DistNotInitializedError(RuntimeError):
     """ Raised when Dist object is called when not initialized. """
     def __init__(self, dist):
         msg = f'{dist} has not been initialized; please call dist.initialize()'
         super().__init__(msg)
+        return
+
 
 class DistNotReadyError(RuntimeError):
     """ Raised when a Dist object is called without being ready. """
     def __init__(self, dist):
         msg = f'{dist} is not ready. This is likely caused by calling a distribution multiple times in a single step. Call dist.jump() to reset.'
         super().__init__(msg)
-        
+        return
+
+
 class DistSeedRepeatError(RuntimeError):
     """ Raised when a Dist object shares a seed with another """
     def __init__(self, dist1, dist2):
         msg = f'A common seed was found between {dist1} and {dist2}. This is likely caused by incorrect initialization of the parent Dists object.'
         super().__init__(msg)
+        return
```

### Comparing `starsim-0.3.4/starsim/interventions.py` & `starsim-0.5.0/starsim/interventions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,67 +2,71 @@
 Define interventions (and analyzers)
 """
 
 import starsim as ss
 import sciris as sc
 import numpy as np
 
-__all__ = ['Analyzer', 'Intervention']
+__all__ = ['Plugin', 'Analyzer', 'Intervention']
 
 
-class Analyzer(ss.Module):
-    """
-    Base class for analyzers. Analyzers are used to provide more detailed information 
-    about a simulation than is available by default -- for example, pulling states 
-    out of sim.people on a particular timestep before they get updated on the next step.
-    
-    The key method of the analyzer is ``apply()``, which is called with the sim
-    on each timestep.
+class Plugin(ss.Module):
+    """ Base class for interventions and analyzers """
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        return
     
-    To retrieve a particular analyzer from a sim, use sim.get_analyzer().
-    """
-
     def __call__(self, *args, **kwargs):
         return self.apply(*args, **kwargs)
     
     def initialize(self, sim):
         return super().initialize(sim)
     
     def apply(self, sim):
         pass
 
-    def finalize(self, sim):
-        return super().finalize(sim)
+    def finalize(self):
+        return super().finalize()
+    
+    @classmethod
+    def from_func(cls, func):
+        """ Create an intervention or analyzer from a function """
+        name = func.__name__
+        new = cls(name=name)
+        new.apply = func
+        return new
 
 
-class Intervention(ss.Module):
+class Analyzer(Plugin):
+    """
+    Base class for analyzers. Analyzers are used to provide more detailed information 
+    about a simulation than is available by default -- for example, pulling states 
+    out of sim.people on a particular timestep before they get updated on the next step.
+    
+    The key method of the analyzer is ``apply()``, which is called with the sim
+    on each timestep.
+    
+    To retrieve a particular analyzer from a sim, use sim.get_analyzer().
+    """
+    pass
+
+
+class Intervention(Plugin):
     """
     Base class for interventions.
     
     The key method of the intervention is ``apply()``, which is called with the sim
     on each timestep.
     """
 
     def __init__(self, eligibility=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.eligibility = eligibility
         return
 
-    def __call__(self, *args, **kwargs):
-        return self.apply(*args, **kwargs)
-    
-    def initialize(self, sim):
-        return super().initialize(sim)
-    
-    def apply(self, sim, *args, **kwargs):
-        raise NotImplementedError
-
-    def finalize(self, sim):
-        return super().finalize(sim)
-
     def _parse_product(self, product):
         """
         Parse the product input
         """
         if isinstance(product, ss.Product):  # No need to do anything
             self.product = product
         elif isinstance(product, str):
@@ -77,20 +81,27 @@
 
     def check_eligibility(self, sim):
         """
         Return an array of indices of agents eligible for screening at time t
         """
         if self.eligibility is not None:
             is_eligible = self.eligibility(sim)
+            if is_eligible is not None and len(is_eligible): # Only worry if non-None/nonzero length
+                if isinstance(is_eligible, ss.BoolArr):
+                    is_eligible = is_eligible.uids
+                if not isinstance(is_eligible, ss.uids):
+                    errormsg = f'Eligibility function must return BoolArr or UIDs, not {type(is_eligible)} {is_eligible}'
+                    raise TypeError(errormsg)
         else:
-            is_eligible = sim.people.alive  # Probably not required
+            is_eligible = sim.people.auids # Everyone
         return is_eligible
 
 
 # %% Template classes for routine and campaign delivery
+
 __all__ += ['RoutineDelivery', 'CampaignDelivery']
 
 class RoutineDelivery(Intervention):
     """
     Base class for any intervention that uses routine delivery; handles interpolation of input years.
     """
 
@@ -173,18 +184,18 @@
             errormsg = f'Length of years incompatible with length of probabilities: {len(self.years)} vs {len(self.prob)}'
             raise ValueError(errormsg)
 
         return
 
 
 # %% Screening and triage
+
 __all__ += ['BaseTest', 'BaseScreening', 'routine_screening', 'campaign_screening', 'BaseTriage', 'routine_triage',
             'campaign_triage']
 
-
 class BaseTest(Intervention):
     """
     Base class for screening and triage.
 
     Args:
          product        (Product)       : the diagnostic to use
          prob           (float/arr)     : annual probability of eligible people receiving the diagnostic
@@ -193,33 +204,33 @@
     """
 
     def __init__(self, product=None, prob=None, eligibility=None, **kwargs):
         super().__init__(**kwargs)
         self.prob = sc.promotetoarray(prob)
         self.eligibility = eligibility
         self._parse_product(product)
-        self.screened = ss.State('screened', bool, False)
-        self.screens = ss.State('screens', int, 0)
-        self.ti_screened = ss.State('ti_screened', int, ss.INT_NAN)
+        self.screened = ss.BoolArr('screened')
+        self.screens = ss.FloatArr('screens', default=0)
+        self.ti_screened = ss.FloatArr('ti_screened')
         return
 
     def initialize(self, sim):
         Intervention.initialize(self, sim)
         self.outcomes = {k: np.array([], dtype=int) for k in self.product.hierarchy}
         return
 
     def deliver(self, sim):
         """
         Deliver the diagnostics by finding who's eligible, finding who accepts, and applying the product.
         """
         ti = sc.findinds(self.timepoints, sim.ti)[0]
         prob = self.prob[ti]  # Get the proportion of people who will be tested this timestep
-        is_eligible = self.check_eligibility(sim)  # Check eligibility
+        eligible_uids = self.check_eligibility(sim)  # Check eligibility
         self.coverage_dist.set(p=prob)
-        accept_uids = self.coverage_dist.filter(ss.true(is_eligible))
+        accept_uids = self.coverage_dist.filter(eligible_uids)
         if len(accept_uids):
             self.outcomes = self.product.administer(sim, accept_uids)  # Actually administer the diagnostic
         return accept_uids
 
     def check_eligibility(self, sim):
         raise NotImplementedError
 
@@ -236,15 +247,15 @@
         """
         raise NotImplementedError
 
     def apply(self, sim, module=None):
         """
         Perform screening by finding who's eligible, finding who accepts, and applying the product.
         """
-        accept_uids = np.array([])
+        accept_uids = ss.uids()
         if sim.ti in self.timepoints:
             accept_uids = self.deliver(sim)
             self.screened[accept_uids] = True
             self.screens[accept_uids] += 1
             self.ti_screened[accept_uids] = sim.ti
             self.results['n_screened'][sim.ti] = len(accept_uids)
             self.results['n_dx'][sim.ti] = len(self.outcomes['positive'])
@@ -259,15 +270,15 @@
         kwargs (dict): passed to BaseTest
     """
     def check_eligibility(self, sim):
         return sc.promotetoarray(self.eligibility(sim))
 
     def apply(self, sim):
         self.outcomes = {k: np.array([], dtype=int) for k in self.product.hierarchy}
-        accept_inds = np.array([])
+        accept_inds = ss.uids()
         if sim.t in self.timepoints: accept_inds = self.deliver(sim)
         return accept_inds
 
 
 class routine_screening(BaseScreening, RoutineDelivery):
     """
     Routine screening - an instance of base screening combined with routine delivery.
@@ -358,16 +369,16 @@
     def initialize(self, sim):
         CampaignDelivery.initialize(self, sim)
         BaseTriage.initialize(self, sim)
         return
 
 
 #%% Treatment interventions
-__all__ += ['BaseTreatment', 'treat_num']
 
+__all__ += ['BaseTreatment', 'treat_num']
 
 class BaseTreatment(Intervention):
     """
     Base treatment class.
 
     Args:
          product        (str/Product)   : the treatment product to use
@@ -388,15 +399,15 @@
         self.outcomes = {k: np.array([], dtype=int) for k in ['unsuccessful', 'successful']} # Store outcomes on each timestep
         return
 
     def get_accept_inds(self, sim):
         """
         Get indices of people who will acccept treatment; these people are then added to a queue or scheduled for receiving treatment
         """
-        accept_uids = np.array([], dtype=int)
+        accept_uids = ss.uids()
         eligible_uids = self.check_eligibility(sim)  # Apply eligiblity
         if len(eligible_uids):
             self.coverage_dist.set(p=self.prob[0])
             accept_uids = self.coverage_dist.filter(eligible_uids)
         return accept_uids
 
     def get_candidates(self, sim):
@@ -408,15 +419,15 @@
     def apply(self, sim):
         """
         Perform treatment by getting candidates, checking their eligibility, and then treating them.
         """
         # Get indices of who will get treated
         treat_candidates = self.get_candidates(sim)  # NB, this needs to be implemented by derived classes
         still_eligible = self.check_eligibility(sim)
-        treat_uids = np.intersect1d(treat_candidates, still_eligible)
+        treat_uids = treat_candidates.intersect(still_eligible)
         if len(treat_uids):
             self.outcomes = self.product.administer(sim, treat_uids)
         return treat_uids
 
 
 class treat_num(BaseTreatment):
     """
@@ -445,34 +456,31 @@
         """
         treat_candidates = np.array([], dtype=int)
         if len(self.queue):
             if self.max_capacity is None or (self.max_capacity > len(self.queue)):
                 treat_candidates = self.queue[:]
             else:
                 treat_candidates = self.queue[:self.max_capacity]
-        return sc.promotetoarray(treat_candidates)
+        return ss.uids(treat_candidates) # TODO: Check
 
     def apply(self, sim):
         """
         Apply treatment. On each timestep, this method will add eligible people who are willing to accept treatment to a
         queue, and then will treat as many people in the queue as there is capacity for.
         """
         self.add_to_queue(sim)
         treat_inds = BaseTreatment.apply(self, sim) # Apply method from BaseTreatment class
         self.queue = [e for e in self.queue if e not in treat_inds] # Recreate the queue, removing people who were treated
         return treat_inds
 
 
-
 #%% Vaccination
 
-
 __all__ += ['BaseVaccination', 'routine_vx', 'campaign_vx']
 
-
 class BaseVaccination(Intervention):
     """
     Base vaccination class for determining who will receive a vaccine.
 
     Args:
          product        (str/Product)   : the vaccine to use
          prob           (float/arr)     : annual probability of eligible population getting vaccinated
@@ -481,32 +489,32 @@
          kwargs         (dict)          : passed to Intervention()
     """
     def __init__(self, product=None, prob=None, label=None, **kwargs):
         Intervention.__init__(self, **kwargs)
         self.prob = sc.promotetoarray(prob)
         self.label = label
         self._parse_product(product)
-        self.vaccinated = ss.State('vaccinated', bool, False)
-        self.n_doses = ss.State('doses', int, 0)
-        self.ti_vaccinated = ss.State('ti_vaccinated', int, ss.INT_NAN)
+        self.vaccinated = ss.BoolArr('vaccinated')
+        self.n_doses = ss.FloatArr('doses', default=0)
+        self.ti_vaccinated = ss.FloatArr('ti_vaccinated')
         self.coverage_dist = ss.bernoulli(p=0)  # Placeholder
         return
 
     def apply(self, sim):
         """
         Deliver the diagnostics by finding who's eligible, finding who accepts, and applying the product.
         """
         accept_uids = np.array([])
         if sim.ti in self.timepoints:
 
             ti = sc.findinds(self.timepoints, sim.ti)[0]
             prob = self.prob[ti]  # Get the proportion of people who will be tested this timestep
             is_eligible = self.check_eligibility(sim)  # Check eligibility
             self.coverage_dist.set(p=prob)
-            accept_uids = self.coverage_dist.filter(ss.true(is_eligible))
+            accept_uids = self.coverage_dist.filter(is_eligible)
 
             if len(accept_uids):
                 self.product.administer(sim.people, accept_uids)
 
                 # Update people's state and dates
                 self.vaccinated[accept_uids] = True
                 self.ti_vaccinated[accept_uids] = sim.ti
@@ -547,9 +555,7 @@
         CampaignDelivery.__init__(self, prob=prob, years=years, interpolate=interpolate)
         return
 
     def initialize(self, sim):
         CampaignDelivery.initialize(self, sim) # Initialize this first, as it ensures that prob is interpolated properly
         BaseVaccination.initialize(self, sim) # Initialize this next
         return
-
-
```

### Comparing `starsim-0.3.4/starsim/network.py` & `starsim-0.5.0/starsim/network.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 import scipy.optimize as spo
 import scipy.spatial as spsp
 
 # CK: need to remove this, but slows down the code otherwise
 ss_float_ = ss.dtypes.float
 ss_int_ = ss.dtypes.int
 
-# Specify all externally visible functions this file defines; see also more definitions below
-__all__ = ['Network', 'Networks', 'DynamicNetwork', 'SexualNetwork']
 
+# Specify all externally visible functions this file defines; see also more definitions below
+__all__ = ['Network', 'DynamicNetwork', 'SexualNetwork']
 
 # %% General network classes
 
 class Network(ss.Module):
     """
     A class holding a single network of contact edges (connections) between people
     as well as methods for updating these.
@@ -56,56 +56,57 @@
 
         # Convert one network to another with extra columns
         index = np.arange(n)
         self_conn = p1 == p2
         network2 = ss.Network(**network, index=index, self_conn=self_conn, label=network.label)
     """
 
-    def __init__(self, pars=None, key_dict=None, vertical=False, *args, **kwargs):
-
+    def __init__(self, key_dict=None, vertical=False, name=None, label=None, requires=None, **kwargs):
         # Initialize as a module
-        super().__init__(pars, *args, **kwargs)
+        super().__init__(name=name, label=label, requires=requires)
 
         # Each relationship is characterized by these default set of keys, plus any user- or network-supplied ones
-        default_keys = dict(
+        default_keys = sc.objdict(
             p1 = ss_int_,
             p2 = ss_int_,
             beta = ss_float_,
         )
-        self.meta = ss.omerge(default_keys, key_dict)
+        self.meta = sc.mergedicts(default_keys, key_dict)
         self.vertical = vertical  # Whether transmission is bidirectional
 
         # Initialize the keys of the network
         self.contacts = sc.objdict()
         for key, dtype in self.meta.items():
             self.contacts[key] = np.empty((0,), dtype=dtype)
 
         # Set data, if provided
         for key, value in kwargs.items():
-            self.contacts[key] = np.array(value, dtype=self.meta.get(key))
+            self.contacts[key] = np.array(value, dtype=self.meta.get(key)) # Overwrite dtype if supplied, else keep original
             self.initialized = True
 
         # Define states using placeholder values
-        self.participant = ss.State('participant', bool, default=False)
+        self.participant = ss.BoolArr('participant')
+        self.validate_uids()
         return
     
     @property
     def p1(self):
         return self.contacts['p1'] if 'p1' in self.contacts else None
     
     @property
     def p2(self):
         return self.contacts['p2'] if 'p2' in self.contacts else None
 
     @property
     def beta(self):
         return self.contacts['beta'] if 'beta' in self.contacts else None
 
-    def initialize(self, sim):
-        super().initialize(sim)
+    def init_vals(self, add_pairs=True):
+        super().init_vals()
+        if add_pairs: self.add_pairs()
         return
 
     def __len__(self):
         try:
             return len(self.contacts.p1)
         except:  # pragma: no cover
             return 0
@@ -124,33 +125,43 @@
         Check if a person is present in a network
 
         Args:
             item: Person index
 
         Returns: True if person index appears in any interactions
         """
-        return (item in self.contacts.p1) or (item in self.contacts.p2)
+        return (item in self.contacts.p1) or (item in self.contacts.p2) # TODO: chek if (item in self.members) is faster
 
     @property
     def members(self):
         """ Return sorted array of all members """
-        return np.unique([self.contacts.p1, self.contacts.p2])
+        return np.unique([self.contacts.p1, self.contacts.p2]).view(ss.uids)
 
     def meta_keys(self):
         """ Return the keys for the network's meta information """
         return self.meta.keys()
 
     def set_network_states(self, people):
         """
         Many network states depend on properties of people -- e.g. MSM depends on being male,
         age of debut varies by sex and over time, and participation rates vary by age.
         Each time states are dynamically grown, this function should be called to set the network
         states that depend on other states.
         """
         pass
+    
+    def validate_uids(self):
+        """ Ensure that p1, p2 are both UID arrays """
+        contacts = self.contacts
+        for key in ['p1', 'p2']:
+            if key in contacts:
+                arr = contacts[key]
+                if not isinstance(arr, ss.uids):
+                    self.contacts[key] = ss.uids(arr)
+        return
 
     def validate(self, force=True):
         """
         Check the integrity of the network: right types, right lengths.
 
         If dtype is incorrect, try to convert automatically; if length is incorrect,
         do not.
@@ -162,55 +173,60 @@
                 expected = dtype
                 if actual != expected:
                     self.contacts[key] = np.array(self.contacts[key], dtype=expected)  # Try to convert to correct type
             actual_n = len(self.contacts[key])
             if n != actual_n:
                 errormsg = f'Expecting length {n} for network key "{key}"; got {actual_n}'  # Report length mismatches
                 raise TypeError(errormsg)
+        self.validate_uids()
         return
 
     def get_inds(self, inds, remove=False):
         """
         Get the specified indices from the edgelist and return them as a dict.
         Args:
             inds (int, array, slice): the indices to find
             remove (bool): whether to remove the indices
         """
         output = {}
         for key in self.meta_keys():
             output[key] = self.contacts[key][inds]  # Copy to the output object
             if remove:
                 self.contacts[key] = np.delete(self.contacts[key], inds)  # Remove from the original
+                self.validate_uids()
         return output
 
     def pop_inds(self, inds):
         """
         "Pop" the specified indices from the edgelist and return them as a dict.
         Returns arguments in the right format to be used with network.append().
 
         Args:
             inds (int, array, slice): the indices to be removed
         """
         popped_inds = self.get_inds(inds, remove=True)
         return popped_inds
 
-    def append(self, contacts):
+    def append(self, contacts=None, **kwargs):
         """
         Append contacts to the current network.
 
         Args:
             contacts (dict): a dictionary of arrays with keys p1,p2,beta, as returned from network.pop_inds()
         """
+        contacts = sc.mergedicts(contacts, kwargs)
         for key in self.meta_keys():
-            new_arr = contacts[key]
-            n_curr = len(self.contacts[key])  # Current number of contacts
-            n_new = len(new_arr)  # New contacts to add
-            n_total = n_curr + n_new  # New size
-            self.contacts[key] = np.resize(self.contacts[key], n_total)  # Resize to make room, preserving dtype
-            self.contacts[key][n_curr:] = new_arr  # Copy contacts into the network
+            curr_arr = self.contacts[key]
+            try:
+                new_arr = contacts[key]
+            except KeyError:
+                errormsg = f'Cannot append contacts since required key "{key}" is missing'
+                raise KeyError(errormsg)
+            self.contacts[key] = np.concatenate([curr_arr, new_arr])  # Resize to make room, preserving dtype
+        self.validate_uids()
         return
 
     def to_dict(self):
         """ Convert to dictionary """
         d = {k: self.contacts[k] for k in self.meta_keys()}
         return d
 
@@ -267,205 +283,197 @@
 
         return contact_inds
 
     def add_pairs(self):
         """ Define how pairs of people are formed """
         pass
 
-    def update(self, people):
+    def update(self):
         """ Define how pairs/connections evolve (in time) """
         pass
 
     def remove_uids(self, uids):
         """
         Remove interactions involving specified UIDs
         This method is typically called via `People.remove()` and
         is specifically used when removing agents from the simulation.
         """
         keep = ~(np.isin(self.contacts.p1, uids) | np.isin(self.contacts.p2, uids))
         for k in self.meta_keys():
             self.contacts[k] = self.contacts[k][keep]
 
+        return
+
     def beta_per_dt(self, disease_beta=None, dt=None, uids=None):
         if uids is None: uids = Ellipsis
         return self.contacts.beta[uids] * disease_beta * dt
 
 
-class Networks(ss.ndict):
-    """
-    Container for networks
-    """
-    def __init__(self, *args, type=Network, connectors=None, **kwargs):
-        self.setattribute('_connectors', ss.ndict(connectors))
-        super().__init__(*args, type=type, **kwargs)
-        return
-
-    def initialize(self, sim):
-        for nw in self.values():
-            nw.initialize(sim)
-        for cn in self._connectors.values():
-            cn.initialize(sim)
-        return
-
-    def update(self, people):
-        for nw in self.values():
-            nw.update(people)
-        for cn in self._connectors.values():
-            cn.update(people)
-        return
-
-
 class DynamicNetwork(Network):
     """ A network where partnerships update dynamically """
-    def __init__(self, pars=None, key_dict=None, **kwargs):
-        key_dict = ss.omerge({'dur': ss_float_}, key_dict)
-        super().__init__(pars, key_dict=key_dict, **kwargs)
+    def __init__(self, key_dict=None, **kwargs):
+        key_dict = sc.mergedicts({'dur': ss_float_}, key_dict)
+        super().__init__(key_dict=key_dict, **kwargs)
         return
 
-    def end_pairs(self, people):
-        dt = people.dt
-        self.contacts.dur = self.contacts.dur - dt
+    def end_pairs(self):
+        people = self.sim.people
+        self.contacts.dur = self.contacts.dur - self.sim.dt
 
         # Non-alive agents are removed
         active = (self.contacts.dur > 0) & people.alive[self.contacts.p1] & people.alive[self.contacts.p2]
         for k in self.meta_keys():
             self.contacts[k] = self.contacts[k][active]
-        return
+        return len(active)
 
 
-class SexualNetwork(Network):
+class SexualNetwork(DynamicNetwork):
     """ Base class for all sexual networks """
-    def __init__(self, pars=None, key_dict=None, **kwargs):
-        key_dict = ss.omerge({'acts': ss_int_}, key_dict)
-        super().__init__(pars, key_dict=key_dict, **kwargs)
-        self.debut = ss.State('debut', float, default=0)
+    def __init__(self, key_dict=None, **kwargs):
+        key_dict = sc.mergedicts({'acts': ss_int_}, key_dict)
+        super().__init__(key_dict=key_dict, **kwargs)
+        self.debut = ss.FloatArr('debut', default=0)
         return
 
     def active(self, people):
         # Exclude people who are not alive
-        return self.participant & (people.age > self.debut) & people.alive
+        valid_age = people.age > self.debut
+        active = self.participant & valid_age & people.alive
+        return active
 
     def available(self, people, sex):
         # Currently assumes unpartnered people are available
         # Could modify this to account for concurrency
         # This property could also be overwritten by a NetworkConnector
         # which could incorporate information about membership in other
         # contact networks
-        return np.setdiff1d(ss.true(people[sex] & self.active(people)), self.members) # ss.true instead of people.uid[]?
+        right_sex = people[sex]
+        is_active = self.active(people)
+        is_available = (right_sex & is_active).uids
+        still_available = is_available.remove(self.members)
+        return still_available
 
     def beta_per_dt(self, disease_beta=None, dt=None, uids=None):
         if uids is None: uids = Ellipsis
         return self.contacts.beta[uids] * (1 - (1 - disease_beta) ** (self.contacts.acts[uids] * dt))
 
 
 # %% Specific instances of networks
-__all__ += ['StaticNet', 'RandomNet', 'MFNet', 'MSMNet', 'EmbeddingNet', 'MaternalNet']
+__all__ += ['StaticNet', 'RandomNet', 'NullNet', 'MFNet', 'MSMNet', 'EmbeddingNet', 'MaternalNet']
 
 
 class StaticNet(Network):
     """
     A network class of static partnerships converted from a networkx graph. There's no formation of new partnerships
     and initialized partnerships only end when one of the partners dies. The networkx graph can be created outside Starsim
     if population size is known. Or the graph can be created by passing a networkx generator function to Starsim.
 
-    If "seed=True" is passed as a parameter, it is replaced with the built-in RNG.
+    If "seed=True" is passed as a keyword argument or a parameter in pars, it is replaced with the built-in RNG.
     The parameter "n" is supplied automatically to be equal to n_agents.
-    
-    **Examples**::
 
+    **Examples**::
         # Generate a networkx graph and pass to Starsim
         import networkx as nx
         import starsim as ss
         g = nx.scale_free_graph(n=10000)
         ss.StaticNet(graph=g)
 
         # Pass a networkx graph generator to Starsim
         ss.StaticNet(graph=nx.erdos_renyi_graph, p=0.0001, seed=True)
-        
+
         # Just create a default graph
     """
 
     def __init__(self, graph=None, pars=None, **kwargs):
-        super().__init__(**kwargs)
+        super().__init__()
         self.graph = graph
-        self.pars = ss.omerge(dict(seed=True), pars)
-        self.dist = ss.Dist(name='StaticNet').initialize()
+        self.default_pars(seed=True)
+        self.update_pars(pars, **kwargs)
+        self.dist = ss.Dist(name='StaticNet')
         return
 
     def initialize(self, sim):
-        n_agents = sim.pars.n_agents
+        super().initialize(sim)
+        self.n_agents = sim.pars.n_agents
         if self.graph is None:
             self.graph = nx.fast_gnp_random_graph # Fast random (Erdos-Renyi) graph creator
             if 'p' not in self.pars and 'n_contacts' not in self.pars: # TODO: refactor
                 self.pars.n_contacts = 10
         if 'n_contacts' in self.pars: # Convert from n_contacts to probability
-            self.pars.p = self.pars.pop('n_contacts')/n_agents
+            self.pars.p = self.pars.pop('n_contacts')/self.n_agents
+        return
+    
+    def init_vals(self):
+        super().init_vals()
         if 'seed' in self.pars and self.pars.seed is True:
             self.pars.seed = self.dist.rng
         if callable(self.graph):
-            self.graph = self.graph(n=n_agents, **self.pars)
-        self.validate_pop(n_agents)
-        super().initialize(sim)
+            try:
+                self.graph = self.graph(n=self.n_agents, **self.pars)
+            except TypeError as e:
+                print(f"{str(e)}: networkx {self.graph.name} not supported. Try using ss.NullNet().")
+                raise e
+        self.validate_pop(self.n_agents)
         self.get_contacts()
         return
 
-    def validate_pop(self, popsize):
+    def validate_pop(self, n_agents):
         n_nodes = self.graph.number_of_nodes()
-        if n_nodes > popsize:
-            errormsg = f'Please ensure the number of nodes in graph {n_nodes} is smaller than population size {popsize}.'
-            raise ValueError(errormsg)
+        if n_nodes > n_agents:
+            errmsg = (f"Please ensure the number of nodes in graph ({n_nodes}) is less than "
+                      f"or equal to (<=) the agent population size ({n_agents}).")
+            raise ValueError(errmsg)
+
+        if not self.graph.number_of_edges():
+            errmsg = f"The nx generator {self.graph.name} produced a graph with no edges"
+            raise ValueError(errmsg)
 
     def get_contacts(self):
         p1s = []
         p2s = []
         for edge in self.graph.edges():
             p1, p2 = edge
             p1s.append(p1)
             p2s.append(p2)
-        self.contacts.p1 = np.concatenate([self.contacts.p1, p1s])
-        self.contacts.p2 = np.concatenate([self.contacts.p2, p2s])
-        self.contacts.beta = np.concatenate([self.contacts.beta, np.ones_like(p1s)])
+        contacts = dict(p1=p1s, p2=p2s, beta=np.ones_like(p1s))
+        self.append(contacts)
         return
 
 
 class RandomNet(DynamicNetwork):
     """ Random connectivity between agents """
 
-    def __init__(self, pars=None, par_dists=None, key_dict=None, **kwargs):
+    def __init__(self, pars=None, key_dict=None, **kwargs):
         """ Initialize """
-        pars = ss.omerge({
-            'n_contacts': 10,  # Distribution or int. If int, interpreted as the mean of the dist listed in par_dists
-            'dur': 0,
-        }, pars)
-
-        super().__init__(pars=pars, key_dict=key_dict, **kwargs)
-        
-        # Default RNG
-        self.dist = ss.Dist(distname='RandomNet')
-
+        super().__init__(key_dict=key_dict)
+        self.default_pars(
+            n_contacts = ss.delta(10),
+            dur = 0,
+        )
+        self.update_pars(pars, **kwargs)
+        self.dist = ss.Dist(distname='RandomNet') # Default RNG
         return
 
-    def initialize(self, sim):
-        super().initialize(sim)
-        self.add_pairs(sim.people)
+    def init_vals(self):
+        self.add_pairs()
         return
 
     @staticmethod
     @nb.njit(cache=True)
     def get_source(inds, n_contacts):
         """ Optimized helper function for getting contacts """
         total_number_of_half_edges = np.sum(n_contacts)
         count = 0
         source = np.zeros((total_number_of_half_edges,), dtype=ss_int_)
         for i, person_id in enumerate(inds):
             n = n_contacts[i]
             source[count: count + n] = person_id
             count += n
         return source
-    
+
     def get_contacts(self, inds, n_contacts):
         """
         Efficiently generate contacts
 
         Note that because of the shuffling operation, each person is assigned 2N contacts
         (i.e. if a person has 5 contacts, they appear 5 times in the 'source' array and 5
         times in the 'target' array). Therefore, the `number_of_contacts` argument to this
@@ -485,99 +493,129 @@
         Returns: Two arrays, for source and target
         """
         source = self.get_source(inds, n_contacts)
         target = self.dist.rng.permutation(source)
         self.dist.jump() # Reset the RNG manually # TODO, think if there's a better way
         return source, target
 
-    def update(self, people, dt=None):
-        self.end_pairs(people)
-        self.add_pairs(people)
+    def update(self):
+        self.end_pairs()
+        self.add_pairs()
         return
 
-    def add_pairs(self, people):
+    def add_pairs(self):
         """ Generate contacts """
+        people = self.sim.people
         if isinstance(self.pars.n_contacts, ss.Dist):
             number_of_contacts = self.pars.n_contacts.rvs(people.uid[people.alive])  # or people.uid?
         else:
             number_of_contacts = np.full(len(people), self.pars.n_contacts)
 
         number_of_contacts = np.round(number_of_contacts / 2).astype(ss_int_)  # One-way contacts
 
         p1, p2 = self.get_contacts(people.uid.__array__(), number_of_contacts)
         beta = np.ones(len(p1), dtype=ss_float_)
 
         if isinstance(self.pars.dur, ss.Dist):
             dur = self.pars.dur.rvs(p1)
         else:
             dur = np.full(len(p1), self.pars.dur)
+        
+        self.append(p1=p1, p2=p2, beta=beta, dur=dur)
+        return
 
-        self.contacts.p1 = np.concatenate([self.contacts.p1, p1])
-        self.contacts.p2 = np.concatenate([self.contacts.p2, p2])
-        self.contacts.beta = np.concatenate([self.contacts.beta, beta])
-        self.contacts.dur = np.concatenate([self.contacts.dur, dur])
 
+class NullNet(Network):
+    """
+    A convenience class for a network of size n that only has self-connections with a weight of 0.
+    This network can be useful for debugging purposes or as a placeholder network during development
+    for conditions that require more complex network mechanisms.
+
+    Guarantees there's one (1) contact per agent (themselves), and that their connection weight is zero.
+
+    For an empty network (ie, no contacts) use
+    >> import starsim as ss
+    >> import networkx as nx
+    >> empty_net_static = ss.StaticNet(nx.empty_graph)
+    >> empty_net_rand = ss.RandomNet(n_contacts=0)
+
+    """
+
+    def __init__(self, n_people=None, **kwargs):
+        self.n = n_people
+        super().__init__(**kwargs)
+        return
+
+    def initialize(self, sim):
+        super().initialize(sim)
+        popsize = sim.pars['n_agents']
+        if self.n is None:
+            self.n = popsize
+        else:
+            if self.n > popsize:
+                errormsg = f'Please ensure the size of the network ({self.n} is less than or equal to the population size ({popsize}).'
+                raise ValueError(errormsg)
+        self.get_contacts()
+        return
+
+    def get_contacts(self):
+        indices = np.arange(self.n)
+        self.append(dict(p1=indices, p2=indices, beta=np.zeros_like(indices)))
         return
 
 
-class MFNet(SexualNetwork, DynamicNetwork):
+class MFNet(SexualNetwork):
     """
     This network is built by **randomly pairing** males and female with variable
     relationship durations.
     """
-
-    def __init__(self, pars=None, par_dists=None, key_dict=None, **kwargs):
-        pars = ss.omergeleft(pars,
-            duration = 15,  # Can vary by age, year, and individual pair. Set scale=exp(mu) and s=sigma where mu,sigma are of the underlying normal distribution.
-            participation = 0.9,  # Probability of participating in this network - can vary by individual properties (age, sex, ...) using callable parameter values
-            debut = 16,  # Age of debut can vary by using callable parameter values
-            acts = 80,
+    def __init__(self, pars=None, key_dict=None, **kwargs):
+        super().__init__(key_dict=key_dict)
+        self.default_pars(
+            duration = ss.lognorm_ex(mean=15),  # Can vary by age, year, and individual pair. Set scale=exp(mu) and s=sigma where mu,sigma are of the underlying normal distribution.
+            participation = ss.bernoulli(p=0.9),  # Probability of participating in this network - can vary by individual properties (age, sex, ...) using callable parameter values
+            debut = ss.normal(loc=16),  # Age of debut can vary by using callable parameter values
+            acts = ss.poisson(lam=80),
             rel_part_rates = 1.0,
         )
+        self.update_pars(pars=pars, **kwargs)
 
-        par_dists = ss.omergeleft(par_dists,
-            duration      = ss.lognorm_ex,
-            participation = ss.bernoulli,
-            debut         = ss.normal,
-            acts          = ss.poisson,
-        )
-
-        DynamicNetwork.__init__(self, key_dict=key_dict, **kwargs)
-        SexualNetwork.__init__(self, pars, key_dict=key_dict, **kwargs)
-
+        # Finish initialization
         self.dist = ss.choice(name='MFNet', replace=False) # Set the array later
-        self.par_dists = par_dists
-
         return
 
-    def initialize(self, sim):
-        super().initialize(sim)
-        self.set_network_states(sim.people)
-        self.add_pairs(sim.people, ti=0)
+    def init_vals(self):
+        self.set_network_states()
+        self.add_pairs()
         return
 
-    def set_network_states(self, people, upper_age=None):
+    def set_network_states(self, upper_age=None):
         """ Set network states including age of entry into network and participation rates """
-        self.set_debut(people, upper_age=upper_age)
-        self.set_participation(people, upper_age=upper_age)
+        self.set_debut(upper_age=upper_age)
+        self.set_participation(upper_age=upper_age)
+        return
 
-    def set_participation(self, people, upper_age=None):
-        # Set people who will participate in the network at some point
-        if upper_age is None: uids = people.uid
-        else: uids = people.uid[(people.age < upper_age)]
+    def set_participation(self, upper_age=None):
+        """ Set people who will participate in the network at some point """
+        people = self.sim.people
+        if upper_age is None: uids = people.auids
+        else: uids = (people.age < upper_age).uids
         self.participant[uids] = self.pars.participation.rvs(uids)
+        return
 
-    def set_debut(self, people, upper_age=None):
-        # Set debut age
-        if upper_age is None: uids = people.uid
-        else: uids = people.uid[(people.age < upper_age)]
+    def set_debut(self, upper_age=None):
+        """ Set debut age """
+        people = self.sim.people
+        if upper_age is None: uids = people.auids
+        else: uids = (people.age < upper_age).uids
         self.debut[uids] = self.pars.debut.rvs(uids)
         return
 
-    def add_pairs(self, people, ti=None):
+    def add_pairs(self):
+        people = self.sim.people
         available_m = self.available(people, 'male')
         available_f = self.available(people, 'female')
 
         # random.choice is not common-random-number safe, and therefore we do
         # not try to Stream-ify the following draws at this time.
         if len(available_m) <= len(available_f):
             self.dist.set(a=available_f)
@@ -592,54 +630,48 @@
         beta = np.ones_like(p1)
 
         # Figure out durations and acts
         if (len(p1) == len(np.unique(p1))):
             # No duplicates and user has enabled multirng, so use slotting based on p1
             dur_vals = self.pars.duration.rvs(p1)
             act_vals = self.pars.acts.rvs(p1)
-        else:
+        else: # TODO: rethink explanation without multirng
             # If multirng is enabled, we're here because some individuals in p1
             # are starting multiple relationships on this timestep. If using
             # slotted draws, as above, repeated relationships will get the same
             # duration and act rates, which is scientifically undesirable.
             # Instead, we fall back to a not-CRN safe approach:
             dur_vals = self.pars.duration.rvs(len(p1))  # Just use len(p1) to say how many draws are needed
             act_vals = self.pars.acts.rvs(len(p1))
 
-        self.contacts.p1 = np.concatenate([self.contacts.p1, p1])
-        self.contacts.p2 = np.concatenate([self.contacts.p2, p2])
-        self.contacts.beta = np.concatenate([self.contacts.beta, beta])
-        self.contacts.dur = np.concatenate([self.contacts.dur, dur_vals])
-        self.contacts.acts = np.concatenate([self.contacts.acts, act_vals])
+        self.append(p1=p1, p2=p2, beta=beta, dur=dur_vals, acts=act_vals)
 
         return len(p1)
 
-    def update(self, people, dt=None):
-        self.end_pairs(people)
-        self.set_network_states(people, upper_age=people.dt)
-        self.add_pairs(people)
+    def update(self):
+        self.end_pairs()
+        self.set_network_states(upper_age=self.sim.dt) # TODO: looks wrong
+        self.add_pairs()
         return
 
 
-class MSMNet(SexualNetwork, DynamicNetwork):
+class MSMNet(SexualNetwork):
     """
     A network that randomly pairs males
     """
 
     def __init__(self, pars=None, key_dict=None, **kwargs):
-        pars = ss.omergeleft(pars,
-            duration_dist = ss.lognorm_ex(mean=15, stdev=15),
-            participation_dist = ss.bernoulli(p=0.1),  # Probability of participating in this network - can vary by individual properties (age, sex, ...) using callable parameter values
-            debut_dist = ss.normal(loc=16, scale=2),
+        super().__init__(key_dict=key_dict)
+        self.default_pars(
+            duration = ss.lognorm_ex(mean=15, stdev=15),
+            debut = ss.normal(loc=16, scale=2),
             acts = ss.lognorm_ex(mean=80, stdev=20),
-            rel_part_rates = 1.0,
+            participation = ss.bernoulli(p=0.1),
         )
-        DynamicNetwork.__init__(self, key_dict, **kwargs)
-        SexualNetwork.__init__(self, pars, key_dict)
-        self.dist = ss.bernoulli(name='MSMNet')
+        self.update_pars(pars, **kwargs)
         return
 
     def initialize(self, sim):
         # Add more here in line with MF network, e.g. age of debut
         # Or if too much replication then perhaps both these networks
         # should be subclasss of a specific network type (ask LY/DK)
         super().initialize(sim)
@@ -650,111 +682,101 @@
     def set_network_states(self, people, upper_age=None):
         """ Set network states including age of entry into network and participation rates """
         if upper_age is None: uids = people.uid[people.male]
         else: uids = people.uid[people.male & (people.age < upper_age)]
 
         # Participation
         self.participant[people.female] = False
-        pr = self.pars.rel_part_rates
-        self.dist.set(p=pr)
-        self.participant[uids] = self.dist.rvs(uids) # Should be CRN safe?
+        self.participant[uids] = self.participation.rvs(uids) # Should be CRN safe?
 
         # Debut
-        self.debut[uids] = self.pars.debut_dist.rvs(len(uids)) # Just pass len(uids) as this network is not crn safe anyway
+        self.debut[uids] = self.pars.debut.rvs(len(uids)) # Just pass len(uids) as this network is not crn safe anyway
         return
 
-    def add_pairs(self, people, ti=None):
-        # Pair all unpartnered MSM
-        available_m = self.available(people, 'm')
+    def add_pairs(self):
+        """ Pair all unpartnered MSM """
+        available_m = self.available(self.sim.people, 'm')
         n_pairs = int(len(available_m)/2)
         p1 = available_m[:n_pairs]
         p2 = available_m[n_pairs:n_pairs*2]
 
         # Figure out durations
         if (len(p1) == len(np.unique(p1))):
             # No duplicates, so use slotting based on p1
             dur = self.pars.duration.rvs(p1)
             act_vals = self.pars.acts.rvs(p1)
         else:
             dur = self.pars.duration.rvs(len(p1)) # Just use len(p1) to say how many draws are needed
             act_vals = self.pars.acts.rvs(len(p1))
 
-        self.contacts.p1 = np.concatenate([self.contacts.p1, p1])
-        self.contacts.p2 = np.concatenate([self.contacts.p2, p2])
-        self.contacts.beta = np.concatenate([self.contacts.beta, np.ones_like(p1)])
-        self.contacts.dur = np.concatenate([self.contacts.dur, dur])
-        self.contacts.acts = np.concatenate([self.contacts.acts, act_vals])
+        self.append(p1=p1, p2=p2, beta=np.ones_like(p1), dur=dur, acts=act_vals)
+        
         return len(p1)
 
-    def update(self, people, dt=None):
-        self.end_pairs(people)
-        self.set_network_states(people, upper_age=people.dt)
-        self.add_pairs(people)
+    def update(self):
+        self.end_pairs(self.sim)
+        self.set_network_states(self.sim.people, upper_age=self.sim.dt)
+        self.add_pairs(self.sim)
         return
 
 
 class EmbeddingNet(MFNet):
     """
     Heterosexual age-assortative network based on a one-dimensional embedding. Could be made more generic.
     """
 
     def __init__(self, pars=None, **kwargs):
         """
         Create a sexual network from a 1D embedding based on age
 
-        male_shift is the average age that males are older than females in partnerships
-        std is the standard deviation of noise added to the age of each individual when seeking a pair. Larger values will created more diversity in age gaps.
-        
+        Args:
+            male_shift is the average age that males are older than females in partnerships
         """
-        pars = ss.omerge({
-            'embedding_func': ss.normal(name='EmbeddingNet', loc=self.embedding_loc, scale=2),
-            'male_shift': 5,
-        }, pars)
-        super().__init__(pars, **kwargs)
+        super().__init__()
+        self.default_pars(
+            inherit = True, # The MFNet already comes with pars, we want to keep those
+            embedding_func = ss.normal(name='EmbeddingNet', loc=self.embedding_loc, scale=2),
+            male_shift = 5,
+        )
+        self.update_pars(pars, **kwargs)
         return
 
     @staticmethod
     def embedding_loc(module, sim, uids):
-        loc = sim.people.age[uids].values
+        loc = sim.people.age[uids]
         loc[sim.people.female[uids]] += module.pars.male_shift  # Shift females so they will be paired with older men
         return loc
 
-    def add_pairs(self, people, ti=None):
+    def add_pairs(self):
+        people = self.sim.people
         available_m = self.available(people, 'male')
         available_f = self.available(people, 'female')
 
         if not len(available_m) or not len(available_f):
             if ss.options.verbose > 1:
                 print('No pairs to add')
             return 0
 
-        available = np.concatenate((available_m, available_f))
+        available = ss.uids.cat(available_m, available_f)
         loc = self.pars.embedding_func.rvs(available)
         loc_f = loc[people.female[available]]
         loc_m = loc[~people.female[available]]
 
         dist_mat = spsp.distance_matrix(loc_m[:, np.newaxis], loc_f[:, np.newaxis])
-
         ind_m, ind_f = spo.linear_sum_assignment(dist_mat)
-        # loc_f[ind_f[0]] is close to loc_m[ind_m[0]]
-
         n_pairs = len(ind_f)
 
-        beta = np.ones(n_pairs)
-
-        # Figure out durations
+        # Finalize pairs
         p1 = available_m[ind_m]
+        p2 = available_f[ind_f]
+        beta = np.ones(n_pairs) # TODO: Allow custom beta
         dur_vals = self.pars.duration.rvs(p1)
         act_vals = self.pars.acts.rvs(p1)
 
-        self.contacts.p1 = np.concatenate([self.contacts.p1, p1])
-        self.contacts.p2 = np.concatenate([self.contacts.p2, available_f[ind_f]])
-        self.contacts.beta = np.concatenate([self.contacts.beta, beta])
-        self.contacts.dur = np.concatenate([self.contacts.dur, dur_vals])
-        self.contacts.acts = np.concatenate([self.contacts.acts, act_vals])
+        self.append(p1=p1, p2=p2, beta=beta, dur=dur_vals, acts=act_vals)
         return len(beta)
 
 
 class MaternalNet(Network):
     """
     Vertical (birth-related) transmission network
     """
@@ -762,108 +784,27 @@
         """
         Initialized empty and filled with pregnancies throughout the simulation
         """
         key_dict = sc.mergedicts({'dur': ss_float_}, key_dict)
         super().__init__(key_dict=key_dict, vertical=vertical, **kwargs)
         return
 
-    def update(self, people, dt=None):
-        if dt is None: dt = people.dt
-        # Set beta to 0 for women who complete post-partum period
-        # Keep connections for now, might want to consider removing
+    def update(self):
+        """
+        Set beta to 0 for women who complete post-partum period
+        Keep connections for now, might want to consider removing
+        """
+        dt = self.sim.dt
         self.contacts.dur = self.contacts.dur - dt
         inactive = self.contacts.dur <= 0
         self.contacts.beta[inactive] = 0
         return
 
-    def initialize(self, sim):
-        """ No pairs added upon initialization """
-        pass
-
-    def add_pairs(self, mother_inds, unborn_inds, dur):
-        """
-        Add connections between pregnant women and their as-yet-unborn babies
-        """
-        beta = np.ones_like(mother_inds)
-        self.contacts.p1 = np.concatenate([self.contacts.p1, mother_inds])
-        self.contacts.p2 = np.concatenate([self.contacts.p2, unborn_inds])
-        self.contacts.beta = np.concatenate([self.contacts.beta, beta])
-        self.contacts.dur = np.concatenate([self.contacts.dur, dur])
-        return len(mother_inds)
-
-
-# %% Network connectors
-__all__ += ['NetworkConnector', 'MF_MSM']
-
-class NetworkConnector(ss.Module):
-    """
-    Template for a connector between networks.
-    """
-    def __init__(self, *args, networks=None, pars=None, **kwargs):
-        super().__init__(pars, requires=networks, *args, **kwargs)
-        return
-
-    def set_participation(self, people, upper_age=None):
-        pass
-
-    def update(self, people):
-        pass
-
-
-class MF_MSM(NetworkConnector):
-    """ Combines the MF and MSM networks """
-    def __init__(self, pars=None):
-        networks = [ss.MFNet, ss.MSMNet]
-        pars = ss.omergeleft(pars,
-            prop_bi = 0.5,  # Could vary over time -- but not by age or sex or individual
-        )
-        super().__init__(networks=networks, pars=pars)
-
-        self.bi_dist = ss.bernoulli(p=self.pars.prop_bi)
-        return
-
-    def initialize(self, sim):
-        super().initialize(sim)
-        self.set_participation(sim.people)
-        return
-
-    def set_participation(self, people, upper_age=None):
-        if upper_age is None:
-            uids = people.uid
+    def add_pairs(self, mother_inds=None, unborn_inds=None, dur=None):
+        """ Add connections between pregnant women and their as-yet-unborn babies """
+        if mother_inds is None:
+            return 0
         else:
-            uids = people.uid[(people.age < upper_age)]
-        uids = ss.true(people.male[uids])
-
-        # Get networks and overwrite default participation
-        mf = people.networks.mf
-        msm = people.networks.msm
-        mf.participant[uids] = False
-        msm.participant[uids] = False
-
-        # Male participation rate uses info about cross-network participation.
-        # First, we determine who's participating in the MSM network
-        pr = msm.pars.part_rates
-        dist = ss.bernoulli.rvs(p=pr, size=len(uids))
-        msm.participant[uids] = dist
-
-        # Now we take the MSM participants and determine which are also in the MF network
-        msm_uids = ss.true(msm.participant[uids])  # Males in the MSM network
-        bi_uids = self.bi_dist.filter(msm_uids)  # Males in both MSM and MF networks
-        mf_excl_set = np.setdiff1d(uids, msm_uids)  # Set of males who aren't in the MSM network
-
-        # What remaining share to we need?
-        mf_df = mf.pars.part_rates.loc[mf.pars.part_rates.sex == 'm']  # Male participation in the MF network
-        mf_pr = np.interp(people.year, mf_df['year'], mf_df['part_rates']) * mf.pars.rel_part_rates
-        remaining_pr = max(mf_pr*len(uids)-len(bi_uids), 0)/len(mf_excl_set)
-
-        # Don't love the following new syntax:
-        mf_excl_uids = mf_excl_set[ss.random().rvs(size=len(mf_excl_set)) < remaining_pr] # TODO: not RNG safe and yes ugly!
-
-        mf.participant[bi_uids] = True
-        mf.participant[mf_excl_uids] = True
-        return
-
-    def update(self, people):
-        self.set_participation(people, upper_age=people.dt)
-        return
-
-
+            n = len(mother_inds)
+            beta = np.ones(n)
+            self.append(p1=mother_inds, p2=unborn_inds, beta=beta, dur=dur)
+            return n
```

### Comparing `starsim-0.3.4/starsim/people.py` & `starsim-0.5.0/starsim/people.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,208 +4,78 @@
 
 # %% Imports
 import numpy as np
 import pandas as pd
 import sciris as sc
 import starsim as ss
 
-__all__ = ['BasePeople', 'People']
+__all__ = ['People', 'Person']
 
-# %% Main people class
-class BasePeople(sc.prettyobj):
-    """
-    A class to handle all the boilerplate for people -- everything interesting 
-    happens in the People class, whereas this class exists to handle the less 
-    interesting implementation details.
-    """
-
-    def __init__(self, n_agents):
-
-        self.initialized = False
-        self._uid_map = ss.ArrayView(int, default=ss.INT_NAN)  # This variable tracks all UIDs ever created
-        self.uid = ss.ArrayView(int, default=ss.INT_NAN)  # This variable tracks all UIDs currently in use
-
-        n = int(n_agents)
-
-        self._uid_map.grow(n)
-        self._uid_map[:] = np.arange(0, n)
-        self.uid.grow(n)
-        self.uid[:] = np.arange(0, n)
-
-        # A slot is a special state managed internally by BasePeople
-        # This is because it needs to be updated separately from any other states, as other states
-        # might have fill_values that depend on the slot
-        self.slot = ss.State('slot', int, ss.INT_NAN)
-
-        self.ti = None  # Track simulation time index
-        self.dt = np.nan  # Track simulation time step
-
-        # User-facing collection of states
-        self.states = ss.ndict(type=ss.State)
-
-        # We also internally store states in a dict keyed by the memory ID of the state, so that we can have colliding names
-        # e.g., across modules, but we will never change the size of a State multiple times in the same iteration over
-        # _states. This is a hidden variable because it is internally used to synchronize the size of all States contained
-        # within the sim, regardless of where they are. In contrast, `People.states` offers a more user-friendly way to access
-        # a selection of the states e.g., module states could be added in there, while intervention states might not
-        self._states = {}
-
-    def __len__(self):
-        """ Length of people """
-        return len(self.uid)
-
-    def register_state(self, state, die=True):
-        """
-        Register a state with the People instance for dynamic resizing
-
-        All states should be registered by this function for the purpose of connecting them to the
-        People's UIDs and to have them be automatically resized when the number of agents changes.
-        This operation is normally triggered as part of initializing the state (via `State.initialize()`)
-        """
-        if id(state) not in self._states:
-            self._states[id(state)] = state
-        elif die:
-            errormsg = f'Cannot add state {state} since already added'
-            raise ValueError(errormsg)
-        return
-
-    def grow(self, n, new_slots=None):
-        """
-        Increase the number of agents
-
-        :param n: Integer number of agents to add
-        :param new_slots: Optionally specify the slots to assign for the new agents. Otherwise, it will default to the new UIDs
-        """
-
-        if n == 0:
-            return np.array([], dtype=ss.dtypes.int)
-
-        start_uid = len(self._uid_map)
-        start_idx = len(self.uid)
-
-        new_uids = np.arange(start_uid, start_uid + n)
-        new_inds = np.arange(start_idx, start_idx + n)
-
-        self._uid_map.grow(n)
-        self._uid_map[new_uids] = new_inds
-
-        self.uid.grow(n)
-        self.uid[new_inds] = new_uids
-
-        # We need to grow the slots as well
-        self.slot.grow(new_uids)
-        self.slot[new_uids] = new_slots if new_slots is not None else new_uids
-
-        for state in self._states.values():
-            state.grow(new_uids)
-
-        return new_uids
 
-    def remove(self, uids_to_remove):
-        """
-        Reduce the number of agents
-
-        :param uids_to_remove: An int/list/array containing the UID(s) to remove
-        """
-
-        # Calculate the *indices* to keep
-        keep_uids = self.uid[~np.in1d(self.uid, uids_to_remove)]  # Calculate UIDs to keep
-        keep_inds = self._uid_map[keep_uids]  # Calculate indices to keep
-
-        # Trim the UIDs and states
-        self.uid._trim(keep_inds)
-        for state in self._states.values(): # includes self.slot
-            state._trim(keep_inds)
-
-        # Update the UID map
-        self._uid_map[:] = ss.INT_NAN  # Clear out all previously used UIDs
-        self._uid_map[keep_uids] = np.arange(0, len(keep_uids))  # Assign the array indices for all of the current UIDs
-
-        return
-
-    def __getitem__(self, key):
-        """
-        Allow people['attr'] instead of getattr(people, 'attr')
-        If the key is an integer, alias `people.person()` to return a `Person` instance
-        """
-        if isinstance(key, int):
-            return self.person(key)  # TODO: need to re-implement
-        else:
-            return self.__getattribute__(key)
-
-    def __setitem__(self, key, value):
-        """ Ditto """
-        return self.__setattr__(key, value)
-
-    def __iter__(self):
-        """ Iterate over people """
-        for i in range(len(self)):
-            yield self[i]
-
-    def __setstate__(self, state):
-        """
-        Set the state upon unpickling/deepcopying
-
-        If a People instance is copied (by any mechanism) then the keys in the `_states`
-        registry will no longer match the memory addresses of the new copied states. Therefore,
-        after copying, we need to re-create the states registry with the new object IDs
-        """
-        state['_states'] =  {id(v):v for v in state['_states'].values()}
-        self.__dict__ = state
-
-
-class People(BasePeople):
+class People(sc.prettyobj):
     """
     A class to perform all the operations on the people
     This class is usually created automatically by the sim. The only required input
     argument is the population size, but typically the full parameters dictionary
     will get passed instead since it will be needed before the People object is
     initialized.
 
     Note that this class handles the mechanics of updating the actual people, while
     ``ss.BasePeople`` takes care of housekeeping (saving, loading, exporting, etc.).
     Please see the BasePeople class for additional methods.
 
     Args:
         pars (dict): the sim parameters, e.g. sim.pars -- alternatively, if a number, interpreted as n_agents
-        strict (bool): whether to only create keys that are already in self.meta.person; otherwise, let any key be set
-        pop_trend (dataframe): a dataframe of years and population sizes, if available
-        kwargs (dict): the actual data, e.g. from a popdict, being specified
+        age_data (dataframe): a dataframe of years and population sizes, if available
+        extra_states (list): non-default states to initialize
 
     **Examples**::
         ppl = ss.People(2000)
     """
 
-    def __init__(self, n_agents, age_data=None, extra_states=None, rand_seed=0):
+    def __init__(self, n_agents, age_data=None, extra_states=None):
         """ Initialize """
-
-        super().__init__(n_agents)
-
-        self.initialized = False
+        
+        # We internally store states in a dict keyed by the memory ID of the state, so that we can have colliding names
+        # e.g., across modules, but we will never change the size of a State multiple times in the same iteration over
+        # _states. This is a hidden variable because it is internally used to synchronize the size of all States contained
+        # within the sim, regardless of where they are. In contrast, `People.states` offers a more user-friendly way to access
+        # a selection of the states e.g., module states could be added in there, while intervention states might not
+        self._states = {}
         self.version = ss.__version__  # Store version info
+        self.initialized = False
 
-        # Handle states
+        # Handle the three fundamental arrays: UIDs for tracking agents, slots for 
+        # tracking random numbers, and AUIDs for tracking alive agents
+        n = int(n_agents)
+        uids = ss.uids(np.arange(n))
+        self.auids = uids.copy() # This tracks all active UIDs (in practice, agents who are alive)
+        self.uid = ss.IndexArr('uid')  # This variable tracks all UIDs
+        self.slot = ss.IndexArr('slot') # A slot is a special state managed internally
+        self.uid.grow(new_vals=uids)
+        self.slot.grow(new_vals=uids)
+        for state in [self.uid, self.slot]:
+            state.people = self # Manually link to people since we don't want to link to states
+        
+        # Handle additional states
+        extra_states = sc.promotetolist(extra_states)
         states = [
-            ss.State('age', float, np.nan), # NaN until conceived
-            ss.State('female', bool, ss.bernoulli(name='female', p=0.5)),
-            ss.State('ti_dead', int, ss.INT_NAN),  # Time index for death
-            ss.State('alive', bool, True),  # Time index for death
-            ss.State('scale', float, 1.0),
+            ss.BoolArr('alive', default=True),  # Time index for death
+            ss.BoolArr('female', default=ss.bernoulli(name='female', p=0.5)),
+            ss.FloatArr('age', default=self.get_age_dist(age_data)), # NaN until conceived
+            ss.FloatArr('ti_dead'),  # Time index for death
+            ss.FloatArr('scale', default=1.0), # The scale factor for the agents (multiplied for making results)
         ]
-        states.extend(sc.promotetolist(extra_states))
-
-        # Expose states with their original names directly as people attributes (e.g., `People.age`) and nested under states
-        # (e.g., `People.states.age`)
+        states.extend(extra_states)
+        self.states = ss.ndict(type=ss.Arr)
         for state in states:
             self.states.append(state, overwrite=False)
             setattr(self, state.name, state)
-
-        # Set initial age distribution - likely move this somewhere else later
-        self.age_data_dist = self.get_age_dist(age_data)
-
+            state.link_people(self)
+            
         return
 
     @staticmethod
     def get_age_dist(age_data):
         """ Return an age distribution based on provided data """
         if age_data is None:
             dist = ss.uniform(low=0, high=100, name='Age distribution')
@@ -213,153 +83,163 @@
 
         if sc.checktype(age_data, pd.DataFrame):
             age_bins = age_data['age'].values
             age_props = age_data['value'].values
             age_props = age_props / age_props.sum()
             return ss.choice(a=age_bins, p=age_props)
 
-
-    def initialize(self, sim):
+    def link_sim(self, sim):
         """ Initialization """
-
         if self.initialized:
-            return
-        else:
-            self.initialized = True # Expected by state.initialize()
-        
-        # For People initialization, first initialize slots, then initialize RNGs, then initialize remaining states
-        # This is because some states may depend on RNGs being initialized to generate initial values
-        self.slot.initialize(sim)
-        self.slot[:] = self.uid
-
-        # Initialize states
-        # Age is handled separately because the default value for new agents is NaN until they are concieved/born whereas
-        # the initial values need to depend on the current age distribution for the setting. In contrast, the sex for new
-        # agents can be sampled from the same distribution used to initialize the population
-        for state in self.states.values():
-            state.initialize(sim)
-
-        # Assign initial ages based on the current age distribution
-        self.age_data_dist.initialize(module=self, sim=sim)
-        self.age[:] = self.age_data_dist.rvs(self.uid)
+            errormsg = 'Cannot re-initialize a People object directly; use sim.initialize(reset=True)'
+            raise RuntimeError(errormsg)
+        self.sim = sim # Store the sim
+        ss.link_dists(obj=self.states, sim=sim, module=self, skip=[ss.Sim, ss.Module])
         return
-
+    
     def add_module(self, module, force=False):
         """
         Add a Module to the People instance
 
         This method is used to add a module to the People. It will register any module states with this
         people instance for dynamic resizing, and expose the states contained in the module to the user
         via `People.states.<module_name>.<state_name>`
-        :param module:
-        :param force:
-        :return:
+        
+        The entries created below make it possible to do `sim.people.hiv.susceptible` or
+        `sim.people.states['hiv.susceptible']` and have both of them work
         """
         # Map the module's states into the People state ndict
         if hasattr(self, module.name) and not force:
             raise Exception(f'Module {module.name} already added')
-        self.__setattr__(module.name, sc.objdict())
 
-        # The entries created below make it possible to do `sim.people.hiv.susceptible` or
-        # `sim.people.states['hiv.susceptible']` and have both of them work
+        if len(module.states):
+            module_states = sc.objdict()
+            setattr(self, module.name, module_states)
+            for state in module.states:
+                state.link_people(self)
+                combined_name = module.name + '.' + state.name  # We will have to resolve how this works with multiple instances of the same module (e.g., for strains). The underlying machinery should be fine though, with People._states being flat and keyed by ID
+                self.states[combined_name] = state # Register the state on the user-facing side using the combined name. Within the original module, it can still be referenced by its original name
+                module_states[state.name] = state
+        return
+    
+    def init_vals(self):
+        """ Populate states with initial values, the final step of initialization """
+        for state in self.states():
+            if not state.initialized:
+                state.init_vals()
+        self.initialized = True
+        return
+    
+    def __bool__(self):
+        """ Ensure that zero-length people are still truthy """
+        return True
+    
+    def __len__(self):
+        """ Length of people """
+        return len(self.auids)
+    
+    @property
+    def n_uids(self):
+        return self.uid.len_used
+    
+    def _link_state(self, state, die=True):
+        """
+        Link a state with the People instance for dynamic resizing; usually called by
+        state.link_people()
 
-        module_states = sc.objdict()
-        setattr(self, module.name, module_states)
-        self._register_module_states(module, module_states)
+        All states should be registered by this function for the purpose of connecting them to the
+        People's UIDs and to have them be automatically resized when the number of agents changes.
+        This operation is normally triggered as part of initializing the state (via `State.initialize()`)
+        """
+        if id(state) not in self._states:
+            self._states[id(state)] = state
+        elif die:
+            errormsg = f'Cannot add state {state} since already added'
+            raise ValueError(errormsg)
         return
 
-    def _register_module_states(self, module, module_states):
-        """Enable dot notation for module specific states:
-         - `sim.people.hiv.susceptible` or
-         - `sim.people.states['hiv.susceptible']`
+    def grow(self, n=None, new_slots=None):
         """
+        Increase the number of agents
 
-        for state in module.states:
-            combined_name = module.name + '.' + state.name  # We will have to resolve how this works with multiple instances of the same module (e.g., for strains). The underlying machinery should be fine though, with People._states being flat and keyed by ID
-            self.states[combined_name] = state  # Register the state on the user-facing side using the combined name. Within the original module, it can still be referenced by its original name
-            pre, _, post = combined_name.rpartition('.')
-            setattr(module_states, state.name, state)
+        Args:
+            n: Integer number of agents to add
+            new_slots: Optionally specify the slots to assign for the new agents. Otherwise, it will default to the new UIDs
+        """
+        if n is None:
+            if new_slots is None:
+                errormsg = 'Must supply either n or new_slots'
+                raise ValueError(errormsg)
+            else:
+                n = len(new_slots)
 
-        return
+        if n == 0:
+            return np.array([], dtype=ss.dtypes.int)
 
-    def scale_flows(self, inds):
-        """
-        Return the scaled versions of the flows -- replacement for len(inds)
-        followed by scale factor multiplication
-        """
-        return self.scale[inds].sum()
+        start_uid = self.uid.len_used
+        stop_uid = start_uid + n
+        new_uids = ss.uids(np.arange(start_uid, stop_uid))
+        self.uid.grow(new_uids, new_vals=new_uids)
 
-    def remove_dead(self, sim):
+        # We need to grow the slots as well
+        new_slots = new_slots if new_slots is not None else new_uids
+        self.slot.grow(new_uids, new_vals=new_slots)
+
+        # Grow the states
+        for state in self._states.values():
+            state.grow(new_uids)
+            
+        # Finally, update the alive indices
+        self.auids = self.auids.concat(new_uids)
+        return new_uids
+
+    def __getitem__(self, key):
         """
-        Remove dead agents
+        Allow people['attr'] instead of getattr(people, 'attr')
+        If the key is an integer, alias `people.person()` to return a `Person` instance
         """
-        uids_to_remove = ss.true(self.dead)
-        if len(uids_to_remove):
-            self.remove(uids_to_remove)
-
-        # Remove the UIDs from the network too
-        for network in sim.networks.values():
-            network.remove_uids(uids_to_remove)
+        if isinstance(key, int):
+            return self.person(key)
+        else:
+            return getattr(self, key)
 
-        return
+    def __setitem__(self, key, value):
+        """ Ditto """
+        return setattr(self, key, value)
 
-    def update_post(self, sim):
+    def __iter__(self):
+        """ Iterate over people """
+        for i in range(len(self)):
+            yield self[i]
+
+    def __setstate__(self, state):
         """
-        Final updates at the very end of the timestep
+        Set the state upon unpickling/deepcopying
 
-        :param sim:
-        :return:
+        If a People instance is copied (by any mechanism) then the keys in the `_states`
+        registry will no longer match the memory addresses of the new copied states. Therefore,
+        after copying, we need to re-create the states registry with the new object IDs
         """
-        self.age[self.alive] += self.dt
+        state['_states'] =  {id(v):v for v in state['_states'].values()}
+        self.__dict__ = state
+        
         return
 
-    def resolve_deaths(self):
+    def scale_flows(self, inds):
         """
-        Carry out any deaths that took place this timestep
-
-        :return:
+        Return the scaled versions of the flows -- replacement for len(inds)
+        followed by scale factor multiplication
         """
-        death_uids = ss.true(self.ti_dead <= self.ti)
-        self.alive[death_uids] = False
-        return death_uids
-
-
-    @property
-    def dead(self):
-        """ Dead boolean """
-        return ~self.alive
-
-    @property
-    def male(self):
-        """ Male boolean """
-        return ~self.female
-
-    @property
-    def f(self):
-        """ Shorthand for female """
-        return self.female
-
-    @property
-    def m(self):
-        """ Shorthand for male """
-        return self.male
-
-    def init_results(self, sim):
-        sim.results += [
-            ss.Result(None, 'n_alive', sim.npts, ss.dtypes.int, scale=True),
-            ss.Result(None, 'new_deaths', sim.npts, ss.dtypes.int, scale=True),
-            ss.Result(None, 'cum_deaths', sim.npts, ss.dtypes.int, scale=True),
-        ]
-        return
+        return self.scale[inds].sum()
 
-    def update_results(self, sim):
-        res = sim.results
-        res.n_alive[self.ti] = np.count_nonzero(self.alive)
-        res.new_deaths[self.ti] = np.count_nonzero(self.ti_dead == self.ti)
-        res.cum_deaths[self.ti] = np.sum(res.new_deaths[:sim.ti])
+    def update_post(self):
+        """ Final updates at the very end of the timestep """
+        sim = self.sim
+        if sim.pars.use_aging:
+            self.age[self.alive.uids] += sim.dt
         return
 
     def request_death(self, uids):
         """
         External-facing function to request an agent die at the current timestep
 
         In general, users should not directly interact with `People.ti_dead` to minimize
@@ -379,14 +259,67 @@
         **WARNING** - this function allows multiple modules to each independently carry out and
         record state changes associated with death. It is therefore important that they can
         guarantee that after requesting death, the death is guaranteed to occur.
 
         :param uids: Agent IDs to request deaths for
         :return: UIDs of agents that have been scheduled to die on this timestep
         """
+        self.ti_dead[uids] = self.sim.ti
+        return
+
+    def resolve_deaths(self):
+        """ Carry out any deaths that took place this timestep """
+        death_uids = (self.ti_dead <= self.sim.ti).uids
+        self.alive[death_uids] = False
+        return death_uids
+    
+    def remove_dead(self):
+        """
+        Remove dead agents
+        """
+        uids = self.dead.uids
+        if len(uids):
+            
+            # Remove the UIDs from the networks too
+            for network in self.sim.networks.values():
+                network.remove_uids(uids) # TODO: only run once every nth timestep
+                
+            # Calculate the indices to keep
+            self.auids = self.auids.remove(uids)
 
-        # Only update the time of death for agents that are currently alive. This way modules cannot
-        # modify the time of death for agents that have already died. Noting that if remove_people is
-        # enabled then often such agents would not be present in the simulation anyway
-        uids = ss.true(self.alive[uids])
-        self.ti_dead[uids] = self.ti
         return
+    
+    @property
+    def dead(self):
+        """ Dead boolean """
+        return ~self.alive
+
+    @property
+    def male(self):
+        """ Male boolean """
+        return ~self.female
+
+    def update_results(self):
+        ti = self.sim.ti
+        res = self.sim.results
+        res.n_alive[ti] = np.count_nonzero(self.alive)
+        res.new_deaths[ti] = np.count_nonzero(self.ti_dead == ti)
+        res.cum_deaths[ti] = np.sum(res.new_deaths[:ti]) # TODO: inefficient to compute the cumulative sum on every timestep!
+        return
+    
+    def person(self, ind):
+        """ Get all the properties for a single person """
+        person = Person()
+        for key in ['uid', 'slot']:
+            person[key] = self[key][ind]
+        for key in self.states.keys():
+            person[key] = self.states[key][ind]
+        return person
+            
+
+class Person(sc.objdict):
+    """ A simple class to hold all attributes of a person """
+    def to_df(self):
+        """ Convert to a dataframe """
+        df = sc.dataframe.from_dict(self, orient='index', columns='value')
+        df.index.name = 'key'
+        return df
```

### Comparing `starsim-0.3.4/starsim/products.py` & `starsim-0.5.0/starsim/products.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 
 
 __all__ = ['Product', 'Dx', 'Tx', 'Vx']
 
 
 class Product(ss.Module):
     """ Generic product implementation """
+    def initialize(self, sim):
+        if not self.initialized:
+            super().initialize(sim)
+        else:
+            return
 
     def administer(self, people, inds):
         """ Adminster a Product - implemented by derived classes """
         raise NotImplementedError
 
 
 class Dx(Product):
@@ -55,25 +60,26 @@
 
         # Pre-fill with the default value, which is set to be the last value in the hierarchy
         results = sc.dataframe({'uids': uids, 'result': self.default_value})
 
         for disease in self.diseases:
             for state in self.health_states:
                 this_state = getattr(sim.diseases[disease], state)
-                these_uids = ss.true(this_state[uids])
+                true_uids = this_state.uids # Find people for which this state is true
+                these_uids = true_uids.intersect(uids) # Find intersection of people in this state and the supplied UIDs
 
                 # Filter the dataframe to extract test results for people in this state
                 df_filter = (self.df.state == state) & (self.df.disease == disease)
                 thisdf = self.df[df_filter]  # apply filter to get the results for this state & genotype
                 probs = [thisdf[thisdf.result == result].probability.values[0] for result in self.hierarchy]
                 self.result_dist.pk = probs  # Overwrite distribution probabilities
 
                 # Sort people into one of the possible result states and then update their overall results
-                this_result = self.result_dist.rvs(these_uids)-these_uids # TODO: check!
-                row_inds = results.uids.isin(these_uids)
+                this_result = self.result_dist.rvs(these_uids)
+                row_inds = sc.findinds(results.uids.isin(these_uids))
                 results.loc[row_inds, 'result'] = np.minimum(this_result, results.loc[row_inds, 'result'])
 
             if return_format == 'dict':
                 output = {self.hierarchy[i]: results[results.result == i].uids.values for i in range(len(self.hierarchy))}
             elif return_format == 'array':
                 output = results
 
@@ -102,15 +108,16 @@
         for disease_name in self.diseases:
 
             disease = sim.diseases[disease_name]
 
             for state in self.health_states:
 
                 pre_tx_state = getattr(disease, state)
-                these_uids = ss.true(pre_tx_state[uids])
+                true_uids = pre_tx_state.uids # People in this state
+                these_uids = true_uids.intersect(uids)
 
                 if len(these_uids):
 
                     df_filter = (self.df.state == state) & (self.df.disease == disease_name)  # Filter by state
                     thisdf = self.df[df_filter]  # apply filter to get the results for this state & genotype
 
                     # Determine whether treatment is successful
@@ -136,16 +143,15 @@
             output = tx_successful
 
         return output
 
 
 class Vx(Product):
     """ Vaccine product """
-    def __init__(self, diseases=None, pars=None, par_dists=None, *args, **kwargs):
-        pars = ss.omerge({}, pars)
-        par_dists = ss.omerge({}, par_dists)
-        super().__init__(pars, par_dists, *args, **kwargs)
+    def __init__(self, diseases=None, pars=None, *args, **kwargs):
+        super().__init__(pars, *args, **kwargs)
         self.diseases = sc.tolist(diseases)
+        return
 
     def administer(self, people, uids):
         """ Apply the vaccine to the requested uids. """
         pass
```

### Comparing `starsim-0.3.4/starsim/results.py` & `starsim-0.5.0/starsim/results.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,17 @@
         arrstr = super().__repr__().removeprefix(cls_name)
         out = f'{cls_name}({modulestr}{self.name}):\narray{arrstr}'
         return out
 
     def __array_finalize__(self, obj):
         if obj is None:
             return
-        self.name = getattr(obj, 'name', None)
+        self.name   = getattr(obj, 'name',   None)
         self.module = getattr(obj, 'module', None)
-        self.scale = getattr(obj, 'scale', None)
+        self.scale  = getattr(obj, 'scale',  None)
         return
 
     def __array_wrap__(self, obj, **kwargs):
         if obj.shape == ():
             return obj[()]
         else:
             return super().__array_wrap__(obj, **kwargs)
```

### Comparing `starsim-0.3.4/starsim/run.py` & `starsim-0.5.0/starsim/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,16 +390,15 @@
             this_iter.update(kwargs)  # Merge with the kwargs
             this_iter['sim'] = this_iter[
                 'sim'].copy()  # Ensure we have a fresh sim; this happens implicitly on pickling with multiprocessing
             sim = single_run(**this_iter)  # Run in series
             sims.append(sim)
 
     return sims
-
-
+                  
 def parallel(*args, **kwargs):
     """
     A shortcut to ``ss.MultiSim()``, allowing the quick running of multiple simulations
     at once.
 
     Args:
         args (list): The simulations to run
@@ -413,8 +412,7 @@
         s1 = ss.Sim(beta=0.01, label='Low')
         s2 = ss.Sim(beta=0.02, label='High')
         ss.parallel(s1, s2).plot()
         msim = ss.parallel([s1, s2], keep_people=True)
     """
     sims = sc.mergelists(*args)
     return MultiSim(sims=sims).run(**kwargs)
-
```

### Comparing `starsim-0.3.4/starsim/samples.py` & `starsim-0.5.0/starsim/samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 - dataset: collection of samples (with different parameters)
 """
 
 import io
 import zipfile
 import sciris as sc
 
+
 __all__ = ['Dataset', 'Samples']
 
 class Dataset:
     def __init__(self, folder=None, results=None, *args, **kwargs):
         # Note that results are not deep copied, to save memory
         if folder is not None:
             self.results = sc.odict()
@@ -88,14 +89,15 @@
             raise KeyError("Multiple results matched the requested criteria")
         else:
             return ds[0]
 
 identifiers_file = 'identifiers.txt'
 summary_file = 'summary.csv'
 
+
 class Samples:
     """
     Stores CSV outputs and summary dataframes
 
     To construct, use ``Samples.new()``. To read an existing one, use ``Samples(fname)``.
     The sample files are just ZIP archives with plain text CSV and TXT files so they
     can be easily accessed externally as well.
@@ -139,14 +141,16 @@
             self.summary = self.summary.sort_index()
 
         self._cache = {}  # Cache the dataframes
 
         if preload:
             self.preload()
 
+        return
+        
     def copy(self):
         """
         Shallow copy - shared cache, copied summary
 
         This allows efficient filtering of seeds within runs by removing rows from
         the copy's summary, while not reloading or duplicating any of the dataframes
         in memory
```

### Comparing `starsim-0.3.4/starsim/settings.py` & `starsim-0.5.0/starsim/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,25 @@
     ss.options(verbose=False)
 """
 
 import os
 import numpy as np
 import sciris as sc
 
-
-__all__ = ['INT_NAN', 'dtypes', 'options']
-
-INT_NAN = 2147483647 # From np.iinfo(np.int32).max: value to use to flag invalid content (i.e., an integer value we are treating like NaN, since NaN can't be stored in an integer array)
+__all__ = ['dtypes', 'options']
 
 # Define Starsim-default data types
 dtypes = sc.objdict(
     bool = bool,
     int = np.int64,
     float = np.float64,
     result_float = np.float64,
 )
 
+
 # Not public to avoid confusion with ss.options
 class Options(sc.objdict):
     """
     Set options for Starsim.
 
     Use ``ss.options.set('defaults')`` to reset all values to default, or ``ss.options.set(dpi='default')``
     to reset one parameter to default. See ``ss.options.help(detailed=True)`` for
```

### Comparing `starsim-0.3.4/starsim/sim.py` & `starsim-0.5.0/starsim/sim.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,524 +1,235 @@
 """
 Define core Sim classes
 """
 
 # Imports
+import itertools
 import numpy as np
 import sciris as sc
 import starsim as ss
-import itertools
 import matplotlib.pyplot as pl
 
-__all__ = ['Sim', 'AlreadyRunError', 'demo', 'diff_sims']
+__all__ = ['Sim', 'AlreadyRunError', 'demo', 'diff_sims', 'check_sims_match']
 
 
 class Sim(sc.prettyobj):
 
     def __init__(self, pars=None, label=None, people=None, demographics=None, diseases=None, networks=None,
-                 connectors=None, interventions=None, analyzers=None, **kwargs):
+                 interventions=None, analyzers=None, connectors=None, copy_inputs=True, **kwargs):
 
+        # Make default parameters (using values from parameters.py)
+        self.pars = ss.make_pars() # Start with default pars
+        args = dict(label=label, people=people, demographics=demographics, diseases=diseases, networks=networks, 
+                    interventions=interventions, analyzers=analyzers, connectors=connectors)
+        args = {key:val for key,val in args.items() if val is not None} # Remove None inputs
+        self.pars.update(sc.mergedicts(pars, args, kwargs, _copy=copy_inputs))  # Update the parameters
+        
         # Set attributes
-        self.label = label  # The label/name of the simulation
-        self.created = None  # The datetime the sim was created
-        self.people = people  # People object
-        self.results = ss.Results(module='sim')  # For storing results
-        self.summary = None  # For storing a summary of the results
+        self.label = label # Usually overwritten during initialization by the parameters
+        self.created = sc.now()  # The datetime the sim was created
         self.initialized = False  # Whether initialization is complete
         self.complete = False  # Whether a simulation has completed running # TODO: replace with finalized?
         self.results_ready = False  # Whether results are ready
-        self.filename = None
-
-        # Time indexing
-        self.ti = None  # The time index, e.g. 0, 1, 2 # TODO: do we need all of these?
-        self.yearvec = None
-        self.tivec = None
-        self.npts = None
-
-        # Make default parameters (using values from parameters.py)
-        self.pars = ss.make_pars()  # Start with default pars
-        self.pars.update_pars(sc.mergedicts(pars, kwargs))  # Update the parameters
-
-        # Placeholders for plug-ins: demographics, diseases, connectors, analyzers, and interventions
-        # Products are not here because they are stored within interventions
-        if demographics == True: demographics = [ss.Births(), ss.Deaths()]  # Use default assumptions for demographics
-        self.demographics  = ss.ndict(demographics, type=ss.Demographics)
-        self.diseases      = ss.ndict(diseases, type=ss.Disease)
-        self.networks      = ss.ndict(networks, type=ss.Network)
-        self.connectors    = ss.ndict(connectors, type=ss.Connector)
-        self.interventions = ss.ndict(interventions, type=ss.Intervention, strict=False) # strict=False since can be a function
-        self.analyzers     = ss.ndict(analyzers, type=ss.Analyzer, strict=False)
-
-        # Initialize the random number generator container
-        self.dists = ss.Dists(obj=self)
-
+        self.dists = ss.Dists(obj=self) # Initialize the random number generator container
+        self.results = ss.Results(module='sim')  # For storing results
+        self.summary = None  # For storing a summary of the results
+        self.filename = None # Store the filename, if saved
         return
-
-    @property
-    def dt(self):
-        if 'dt' in self.pars:
-            return self.pars['dt']
-        else:
-            return np.nan
-
-    @property
-    def year(self):
-        try:
-            return self.yearvec[self.ti]
-        except:
-            return np.nan
-
-    @property
-    def modules(self):
-        # Return iterator over all Module instances (stored in standard places) in the Sim
-        products = [intv.product for intv in self.interventions.values() if
-                    hasattr(intv, 'product') and isinstance(intv.product, ss.Product)]
-        return itertools.chain(
-            self.demographics.values(),
-            self.networks.values(),
-            self.diseases.values(),
-            self.connectors.values(),
-            self.interventions.values(),
-            products,
-            self.analyzers.values(),
-        )
-
-    def initialize(self, reset=False, **kwargs):
-        """
-        Perform all initializations on the sim.
-        """
+    
+    def __getitem__(self, key):
+        """ Allow dict-like access, e.g. sim['diseases'] """
+        return getattr(self, key)
+    
+    def __setitem__(self, key, value):
+        """ Allow dict-like access, e.g. sim['created'] = sc.now() """
+        return setattr(self, key, value)
+    
+    def initialize(self, **kwargs):
+        """ Perform all initializations for the sim; most heavy lifting is done by the parameters """
         # Validation and initialization
-        self.ti = 0  # The current time index
-        self.validate_pars()  # Ensure parameters have valid values
-        self.validate_dt()
-        self.init_time_vecs()  # Initialize time vecs
-        ss.set_seed(self.pars.rand_seed)  # Reset the seed before the population is created -- shouldn't matter if only using Dist objects
-
-        # Initialize the core sim components
-        self.init_people(reset=reset, **kwargs)  # Create all the people (the heaviest step)
-
-        # Initialize plug-ins
-        self.init_demographics()
-        self.init_networks()
-        self.init_diseases()
-        self.init_connectors()
-        self.init_interventions()
-        self.init_analyzers()
+        ss.set_seed(self.pars.rand_seed) # Reset the seed before the population is created -- shouldn't matter if only using Dist objects
+        
+        # Validate parameters
+        self.pars.validate()
 
-        # Initialize all distributions now that everything else is in place
+        # Initialize time
+        self.init_time_attrs()
+        
+        # Initialize the people
+        self.init_people(**kwargs)  # Create all the people
+        
+        # # Initialize the modules within the parameters
+        # self.pars.validate_modules(self)
+        
+        # Move initialized modules to the sim
+        keys = ['label', 'demographics', 'networks', 'diseases', 'interventions', 'analyzers', 'connectors']
+        for key in keys:
+            setattr(self, key, self.pars.pop(key))
+            
+        # Initialize all the modules with the sim
+        for mod in self.modules:
+            mod.initialize(self)
+                
+        # Initialize products # TODO: think about simplifying
+        for mod in self.interventions:
+            if hasattr(mod, 'product') and isinstance(mod.product, ss.Product):
+                mod.product.initialize(self)
+        
+        # Initialize all distributions now that everything else is in place, then set states
         self.dists.initialize(obj=self, base_seed=self.pars.rand_seed, force=True)
+        
+        # Initialize the values in all of the states and networks
+        self.init_vals()
+        
+        # Initialize the results
+        self.init_results()
 
-        # Final steps
+        # It's initialized
         self.initialized = True
-        self.complete = False
-        self.results_ready = False
-
         return self
-
-    def validate_dt(self):
-        """
-        Check that 1/dt is an integer value, otherwise results and time vectors will have mismatching shapes.
-        init_results explicitly makes this assumption by casting resfrequency = int(1/dt).
-        """
-        dt = self.dt
-        reciprocal = 1.0 / dt  # Compute the reciprocal of dt
-        if not reciprocal.is_integer():  # Check if reciprocal is not a whole (integer) number
-            # Round the reciprocal
-            reciprocal = int(reciprocal)
-            rounded_dt = 1.0 / reciprocal
-            self.pars.dt = rounded_dt
-            if self.pars.verbose:
-                warnmsg = f"Warning: Provided time step dt: {dt} resulted in a non-integer number of steps per year. Rounded to {rounded_dt}."
-                print(warnmsg)
-        return
-
-    def validate_pars(self):
-        """
-        Some parameters can take multiple types; this makes them consistent.
-        """
-        # Handle n_agents
-        if self.people is not None:
-            self.pars.n_agents = len(self.people)
-        # elif self.popdict is not None: # Starsim does not currenlty support self.popdict
-        # self.pars.n_agents = len(self.popdict)
-        elif self.pars.n_agents is not None:
-            self.pars.n_agents = int(self.pars.n_agents)
-        else:
-            errormsg = 'Must supply n_agents, a people object, or a popdict'
-            raise ValueError(errormsg)
-
-        # Handle end and n_years
-        if self.pars.end:
-            self.pars.n_years = self.pars.end - self.pars.start
-            if self.pars.n_years <= 0:
-                errormsg = f"Number of years must be >0, but you supplied start={str(self.pars.start)} and " \
-                           f"end={str(self.pars.end)}, which gives n_years={self.pars.n_years}"
-                raise ValueError(errormsg)
-        else:
-            if self.pars.n_years:
-                self.pars.end = self.pars.start + self.pars.n_years
-            else:
-                errormsg = 'You must supply one of n_years and end."'
-                raise ValueError(errormsg)
-
-        # Handle verbose
-        if self.pars.verbose == 'brief':
-            self.pars.verbose = -1
-        if not sc.isnumber(self.pars.verbose):  # pragma: no cover
-            errormsg = f'Verbose argument should be either "brief", -1, or a float, not {type(self.par.verbose)} "{self.par.verbose}"'
-            raise ValueError(errormsg)
-
-        return
-
-    def init_time_vecs(self):
-        """
-        Construct vectors things that keep track of time
-        """
-        self.yearvec = np.arange(start=self.pars.start, stop=self.pars.end + self.pars.dt, step=self.pars.dt)
-        self.npts = len(self.yearvec)
-        self.tivec = np.arange(self.npts)
+    
+    def init_time_attrs(self):
+        """ Time indexing; derived values live in the sim rather than in the pars """
+        self.dt = self.pars.dt # Shortcut to dt since used a lot
+        self.yearvec = np.arange(start=self.pars.start, stop=self.pars.end + self.pars.dt, step=self.pars.dt) # The time points of the sim
+        self.results.yearvec = self.yearvec # Store the yearvec in the results for plotting
+        self.npts = len(self.yearvec) # The number of points in the sim
+        self.tivec = np.arange(self.npts) # The vector of time indices
+        self.ti = 0  # The time index, e.g. 0, 1, 2
         return
 
-    def init_people(self, reset=False, verbose=None, **kwargs):
+    def init_people(self, verbose=None, **kwargs):
         """
         Initialize people within the sim
         Sometimes the people are provided, in which case this just adds a few sim properties to them.
         Other time people are not provided and this method makes them.
+        
         Args:
-            reset           (bool): whether to regenerate the people even if they already exist
-            verbose         (int):  detail to print
-            kwargs          (dict): passed to ss.make_people()
+            verbose (int):  detail to print
+            kwargs  (dict): passed to ss.make_people()
         """
-
         # Handle inputs
-        if verbose is None:
-            verbose = self.pars.verbose
+        people = self.pars.pop('people')
+        n_agents = self.pars.n_agents
+        verbose = sc.ifelse(verbose, self.pars.verbose)
         if verbose > 0:
-            resetstr = ''
-            if self.people and reset:
-                resetstr = ' (resetting people)'
-            print(f'Initializing sim{resetstr} with {self.pars["n_agents"]:0n} agents')
-
-        # If people have not been supplied, make them
-        if self.people is None or reset:
-            self.people = ss.People(n_agents=self.pars.n_agents, **kwargs)  # This just assigns UIDs and length
-
-        # If a popdict has not been supplied, we can make one from location data
-        if self.pars.location is not None:
-            # Check where to get total_pop from
-            if self.pars.total_pop is not None:  # If no pop_scale has been provided, try to get it from the location
-                errormsg = 'You can either define total_pop explicitly or via the location, but not both'
-                raise ValueError(errormsg)
-
-        else:
-            if self.pars.total_pop is not None:  # If no pop_scale has been provided, try to get it from the location
-                total_pop = self.pars.total_pop
-            else:
-                if self.pars.pop_scale is not None:
-                    total_pop = self.pars.pop_scale * self.pars.n_agents
-                else:
-                    total_pop = self.pars.n_agents
-
-        self.pars.total_pop = total_pop
-        if self.pars.pop_scale is None:
-            self.pars.pop_scale = total_pop / self.pars.n_agents
-
-        # Any other initialization
-        if not self.people.initialized:
-            self.people.initialize(self)
-
-        # Set time attributes
-        self.people.ti = self.ti
-        self.people.dt = self.dt
-        self.people.year = self.year
-        self.people.init_results(self)
-        return self
-
-    def convert_plugins(self, plugin_class, plugin_name=None):
-        """
-        Common logic for converting plug-ins to a standard format
-        Used for networks, demographics, diseases, connectors, analyzers, and interventions
-        Args:
-            plugin: class
-        """
-
-        if plugin_name is None: plugin_name = plugin_class.__name__.lower()
-
-        # Get lower-case names of all subclasses
-        known_plugins = {n.__name__.lower():n for n in ss.all_subclasses(plugin_class)}
-        if plugin_name == 'networks': # Allow "msm" or "msmnet"
-            known_plugins.update({k.removesuffix('net'):v for k,v in known_plugins.items()})
-
-        # Figure out if it's in the sim pars or provided directly
-        attr_plugins = getattr(self, plugin_name)  # Get any plugins that have been provided directly
-
-        # See if they've been provided in the pars dict
-        if self.pars.get(plugin_name):
-
-            par_plug = self.pars[plugin_name]
-
-            # String: convert to ndict
-            if isinstance(par_plug, str):
-                plugins = ss.ndict(dict(name=par_plug))
-
-            # List or dict: convert to ndict
-            elif sc.isiterable(par_plug) and len(par_plug):
-                if isinstance(par_plug, dict) and 'type' in par_plug and 'name' not in par_plug:
-                    par_plug['name'] = par_plug['type'] # TODO: simplify/remove this
-                plugins = ss.ndict(par_plug)
-
-        else:  # Not provided directly or in pars
-            plugins = {}
-
-        # Check that we don't have two copies
-        for attr_key in attr_plugins.keys():
-            if plugins.get(attr_key):
-                errormsg = f'Sim was created with {attr_key} module, cannot create another through the pars dict.'
-                raise ValueError(errormsg)
-
-        plugins = sc.mergedicts(plugins, attr_plugins)
-
-        # Process
-        processed_plugins = sc.autolist()
-        for plugin in plugins.values():
-
-            if not isinstance(plugin, plugin_class):
-
-                if isinstance(plugin, dict):
-                    ptype = (plugin.get('type') or plugin.get('name') or '').lower()
-                    name = plugin.get('name') or ptype
-                    if ptype in known_plugins:
-                        # Make an instance of the requested plugin
-                        plugin_pars = {k: v for k, v in plugin.items() if k not in ['type', 'name']}
-                        pclass = known_plugins[ptype]
-                        plugin = pclass(name=name, pars=plugin_pars) # TODO: does this handle par_dists, etc?
-                    else:
-                        errormsg = (f'Could not convert {plugin} to an instance of class {plugin_name}.'
-                                    f'Try specifying it directly rather than as a dictionary.')
-                        raise ValueError(errormsg)
-                elif plugin_name in ['analyzers', 'interventions'] and callable(plugin):
-                    pass # This is ok, it's a function instead of an Intervention object
-                else:
-                    errormsg = (
-                        f'{plugin_name.capitalize()} must be provided as either class instances or dictionaries with a '
-                        f'"name" key corresponding to one of these known subclasses: {known_plugins}.')
-                    raise ValueError(errormsg)
-
-            processed_plugins += plugin
-
-        return processed_plugins
-
-    def init_demographics(self):
-        """ Initialize demographics """
-
-        # Demographics can be provided via sim.demographics or sim.pars - this methods reconciles them
-        demographics = self.convert_plugins(ss.Demographics, plugin_name='demographics')
-
-        # We also allow users to add vital dynamics by entering birth_rate and death_rate parameters directly to the sim
-        if self.pars.birth_rate is not None:
-            births = ss.Births(pars={'birth_rate': self.pars.birth_rate})
-            demographics += births
-        if self.pars.death_rate is not None:
-            background_deaths = ss.Deaths(pars={'death_rate': self.pars.death_rate})
-            demographics += background_deaths
-
-        # Iterate over demographic modules and initialize them
-        for dem_mod in demographics:
-            dem_mod.initialize(self)
-            self.results[dem_mod.name] = dem_mod.results
-
-        # Count how many of each kind of demographic module we have
-        demdict = {'births': ss.Births, 'pregnancy': ss.Pregnancy, 'deaths': ss.Deaths}
-        mod_names = dict()
-        for demname, demtype in demdict.items():
-            mod_names[demname] = [d.name for d in demographics if isinstance(d, demtype)]
-
-            # Validation
-            if len(mod_names[demname]) > 1:
-                if len(mod_names[demname]) == len(set(mod_names[demname])):  # No duplicate names, raise warning
-                    ss.warn(f'Two instances of {demname} module added to the sim; was this intentional?')
-                else:
-                    errormsg = (f'Cannot add two identically-named {demname} modules to a sim.\n '
-                                f'Demographic modules are: \n{sc.newlinejoin(mod_names[demname])}.\n'
-                                f'Tip: if using demographic modules, do not use birth and death rates in the sim pars.')
-                    raise ValueError(errormsg)
-
-        # Ensure they're stored at the sim level
-        self.demographics = ss.ndict(*demographics)
-
-    def init_diseases(self):
-        """ Initialize diseases """
-
-        # Diseases can be provided in sim.demographics or sim.pars
-        diseases = self.convert_plugins(ss.Disease, plugin_name='diseases')
-
-        # Interate over diseases and initialize them
-        for disease in diseases:
-            disease.initialize(self)
-
-            # Add the disease's parameters and results into the Sim's dicts
-            self.pars[disease.name] = disease.pars
-            self.results[disease.name] = disease.results
-
-            # Add disease states to the People's dicts
-            self.people.add_module(disease)
-
-        # Store diseases in the sim
-        self.diseases = ss.ndict(*diseases)
-
-        return
-
-    def init_connectors(self):
-        for connector in self.connectors.values():
-            connector.initialize(self)
-
-    def init_networks(self):
-        """ Initialize networks if these have been provided separately from the people """
-
-        processed_networks = self.convert_plugins(ss.Network, plugin_name='networks')
-
-        # Now store the networks in a Networks object, which also allows for connectors between networks
-        if not isinstance(processed_networks, ss.Networks):
-            self.networks = ss.Networks(*processed_networks)
-        self.networks.initialize(self)
-
-        return
-
-    def init_interventions(self):
-        """ Initialize and validate the interventions """
-
-        interventions = self.convert_plugins(ss.Intervention, plugin_name='interventions')
-
-        # Translate the intervention specs into actual interventions
-        for i, intervention in enumerate(interventions):
-            if isinstance(intervention, type) and issubclass(intervention, ss.Intervention):
-                intervention = intervention()  # Convert from a class to an instance of a class
-            if isinstance(intervention, ss.Intervention):
-                intervention.initialize(self)
-            elif callable(intervention):
-                intv_func = intervention
-                intervention = ss.Intervention(name=f'intervention_func_{i}')
-                intervention.apply = intv_func # Monkey-patch together an intervention from a function
-            else:
-                errormsg = f'Intervention {intervention} does not seem to be a valid intervention: must be a function or Intervention subclass'
-                raise TypeError(errormsg)
-            
-            if intervention.name not in self.interventions:
-                self.interventions += intervention
-
-            # Add the intervention parameters and results into the Sim's dicts
-            self.pars[intervention.name] = intervention.pars
-            self.results[intervention.name] = intervention.results
+            labelstr = f' "{self.label}"' if self.label else ''
+            print(f'Initializing sim{labelstr} with {n_agents:0n} agents')
 
-            # Add intervention states to the People's dicts
-            self.people.add_module(intervention)
-
-            # If there's a product module present, initialize and add it
-            if hasattr(intervention, 'product') and isinstance(intervention.product, ss.Product):
-                intervention.product.initialize(self)
-
-                self.people.add_module(intervention.product)
+        # If people have not been supplied, make them -- typical use case
+        if people is None:
+            people = ss.People(n_agents=n_agents, **kwargs)  # This just assigns UIDs and length
+
+        # Finish up (NB: the People object is not yet initialized)
+        self.people = people
+        self.people.link_sim(self)
+        return self.people
+    
+    def init_vals(self):
+        """ Initialize the states and other objects with values """
         
-        # TODO: combine this with the code above
-        for k,intervention in self.interventions.items():
-            if not isinstance(intervention, ss.Intervention):
-                intv_func = intervention
-                intervention = ss.Intervention(name=f'intervention_func_{k}')
-                intervention.apply = intv_func # Monkey-patch together an intervention from a function
-                self.interventions[k] = intervention
-
-        return
-
-    def init_analyzers(self):
-        """ Initialize the analyzers """
+        # Initialize values in people
+        self.people.init_vals()
         
-        analyzers = self.pars.analyzers
-        if not np.iterable(analyzers):
-            analyzers = sc.tolist(analyzers)
-
-        # Interpret analyzers
-        for ai, analyzer in enumerate(analyzers):
-            if isinstance(analyzer, type) and issubclass(analyzer, ss.Analyzer):
-                analyzer = analyzer()  # Convert from a class to an instance of a class
-            if not (isinstance(analyzer, ss.Analyzer) or callable(analyzer)):
-                errormsg = f'Analyzer {analyzer} does not seem to be a valid analyzer: must be a function or Analyzer subclass'
-                raise TypeError(errormsg)
-            self.analyzers += analyzer  # Add it in
-
-        # TODO: should tidy/remove this code
-        for k,analyzer in self.analyzers.items():
-            if not isinstance(analyzer, ss.Analyzer) and callable(analyzer):
-                ana_func = analyzer
-                analyzer = ss.Analyzer(name=f'analyzer_func_{k}')
-                analyzer.apply = ana_func # Monkey-patch together an intervention from a function
-                self.analyzers[k] = analyzer
-            if isinstance(analyzer, ss.Analyzer):
-                analyzer.initialize(self)
-
+        # Initialize values in other modules, including networks
+        for mod in self.modules:
+            mod.init_vals()
+        return
+    
+    def init_results(self):
+        """ Create initial results that are present in all simulations """
+        self.results += [ # TODO: refactor with self.add_results()
+            ss.Result(None, 'n_alive',    self.npts, ss.dtypes.int, scale=True),
+            ss.Result(None, 'new_deaths', self.npts, ss.dtypes.int, scale=True),
+            ss.Result(None, 'cum_deaths', self.npts, ss.dtypes.int, scale=True),
+        ]
         return
 
+    @property
+    def modules(self):
+        # Return iterator over all Module instances (stored in standard places) in the Sim
+        products = [intv.product for intv in self.interventions.values() if
+                    hasattr(intv, 'product') and isinstance(intv.product, ss.Product)]
+        return itertools.chain(
+            self.demographics.values(),
+            self.networks.values(),
+            self.diseases.values(),
+            self.connectors.values(),
+            self.interventions.values(),
+            products,
+            self.analyzers.values(),
+        )
+    
+    @property
+    def year(self):
+        return self.yearvec[self.ti]
+
     def step(self):
         """ Step through time and update values """
 
         # Set the time and if we have reached the end of the simulation, then do nothing
         if self.complete:
             raise AlreadyRunError('Simulation already complete (call sim.initialize() to re-run)')
 
         # Advance random number generators forward to prepare for any random number calls that may be necessary on this step
         self.dists.jump(to=self.ti+1)  # +1 offset because ti=0 is used on initialization
 
-        # Clean up dead agents, if removing agents is enabled
-        if self.pars.remove_dead and (self.ti % self.pars.remove_dead == 0):
-            self.people.remove_dead(self)
-
         # Update demographic modules (create new agents from births/immigration, schedule non-disease deaths and emigration)
-        for dem_mod in self.demographics.values():
-            dem_mod.update(self)
+        for dem_mod in self.demographics():
+            dem_mod.update()
 
         # Carry out autonomous state changes in the disease modules. This allows autonomous state changes/initializations
         # to be applied to newly created agents
-        for disease in self.diseases.values():
-            disease.update_pre(self)
+        for disease in self.diseases():
+            disease.update_pre()
 
         # Update connectors -- TBC where this appears in the ordering
-        for connector in self.connectors.values():
-            connector.update(self)
+        for connector in self.connectors():
+            connector.update()
 
         # Update networks - this takes place here in case autonomous state changes at this timestep
+        for network in self.networks():
         # affect eligibility for contacts
-        self.networks.update(self.people)
+            network.update()
 
         # Apply interventions - new changes to contacts will be visible and so the final networks can be customized by
         # interventions, by running them at this point
-        for intervention in self.interventions.values():
+        for intervention in self.interventions():
             intervention(self)
 
         # Carry out transmission/new cases
-        for disease in self.diseases.values():
-            disease.make_new_cases(self)
+        for disease in self.diseases():
+            disease.make_new_cases()
 
         # Execute deaths that took place this timestep (i.e., changing the `alive` state of the agents). This is executed
         # before analyzers have run so that analyzers are able to inspect and record outcomes for agents that died this timestep
         uids = self.people.resolve_deaths()
-        for disease in self.diseases.values():
-            disease.update_death(self, uids)
+        for disease in self.diseases():
+            disease.update_death(uids)
 
         # Update results
-        self.people.update_results(self)
+        self.people.update_results()
 
-        for disease in self.diseases.values():
-            disease.update_results(self)
+        for dem_mod in self.demographics():
+            dem_mod.update_results()
 
-        for analyzer in self.analyzers.values():
+        for disease in self.diseases():
+            disease.update_results()
+
+        for analyzer in self.analyzers():
             analyzer(self)
+            
+        # Clean up dead agents
+        self.people.remove_dead()
 
         # Tidy up
         self.ti += 1
         self.people.ti = self.ti
-        self.people.update_post(self)
+        self.people.update_post()
 
         if self.ti == self.npts:
             self.complete = True
 
         return
 
     def run(self, until=None, verbose=None):
@@ -581,15 +292,15 @@
 
         # Scale the results
         for reskey, res in self.results.items():
             if isinstance(res, ss.Result) and res.scale:
                 self.results[reskey] = self.results[reskey] * self.pars.pop_scale
 
         for module in self.modules:
-            module.finalize(self)
+            module.finalize()
 
         self.summarize()
         self.results_ready = True  # Set this first so self.summary() knows to print the results
         self.ti -= 1  # During the run, this keeps track of the next step; restore this be the final day of the sim
         return
 
     def summarize(self, how='default'):
@@ -641,14 +352,15 @@
                 entry = f'N/A {E}'
             summary[key] = entry
         self.summary = summary
         return summary
     
     def disp(self):
         print(self.summary)
+        return
     
     def shrink(self, skip_attrs=None, in_place=True):
         """
         "Shrinks" the simulation by removing the people and other memory-intensive
         attributes (e.g., some interventions and analyzers), and returns a copy of
         the "shrunken" simulation. Used to reduce the memory required for RAM or
         for saved files.
@@ -854,21 +566,26 @@
             args (list): passed to savejson()
             kwargs (dict): passed to savejson()
 
         Returns:
             pardict (dict): a dictionary containing all the parameter values
         '''
         pardict = {}
-        for key in self.pars.keys():
-            if key == 'interventions':
-                pardict[key] = [intervention.to_json() for intervention in self.pars[key]]
-            elif key == 'start_day':
-                pardict[key] = str(self.pars[key])
-            else:
-                pardict[key] = self.pars[key]
+        for key,item in self.pars.items():
+            if key in ss.module_map().keys():
+                if np.iterable(item):
+                    item = [mod.to_json() for mod in item]
+                else:
+                    try:
+                        item = item.to_json()
+                    except:
+                        pass
+            elif key == 'people':
+                continue
+            pardict[key] = item
         if filename is not None:
             sc.savejson(filename=filename, obj=pardict, indent=indent, *args, **kwargs)
         return pardict
 
     def to_json(self, filename=None, keys=None, tostring=False, indent=2, verbose=False, *args, **kwargs):
         '''
         Export results and parameters as JSON.
@@ -930,20 +647,23 @@
         if filename is None:
             output = sc.jsonify(d, tostring=tostring, indent=indent, verbose=verbose, *args, **kwargs)
         else:
             output = sc.savejson(filename=filename, obj=d, indent=indent, *args, **kwargs)
 
         return output
 
-    def plot(self):
+    def plot(self, key=None):
         with sc.options.with_style('fancy'):
             flat = sc.flattendict(self.results, sep=': ')
+            yearvec = flat.pop('yearvec')
+            if key is not None:
+                flat = {k:v for k,v in flat.items() if k.startswith(key)}
             fig, axs = sc.getrowscols(len(flat), make=True)
             for ax, (k, v) in zip(axs.flatten(), flat.items()):
-                ax.plot(self.yearvec, v)
+                ax.plot(yearvec, v)
                 ax.set_title(k)
                 ax.set_xlabel('Year')
         return fig
 
 
 class AlreadyRunError(RuntimeError):
     """
@@ -1107,11 +827,26 @@
     if mismatchmsg:  # pragma: no cover
         if die and n_mismatch: # To catch full=True case
             raise ValueError(mismatchmsg)
         elif output:
             return df
         else:
             print(mismatchmsg)
+            return True
     else:
         if not output:
             print('Sims match')
-    return
+        return False
+
+
+def check_sims_match(*args, full=False):
+    """ Shortcut to using ss.diff_sims() to check if multiple sims match """
+    s1 = args[0]
+    matches = []
+    for s2 in args[1:]:
+        diff = diff_sims(s1, s2, full=False, output=False, die=False)
+        matches.append(not(diff)) # Return the opposite of the diff
+    if full:
+        return matches
+    else:
+        return all(matches)
+
```

### Comparing `starsim-0.3.4/starsim/utils.py` & `starsim-0.5.0/starsim/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import starsim as ss
 import numba as nb
 import pandas as pd
 
 # %% Helper functions
 
 # What functions are externally visible -- note, this gets populated in each section below
-__all__ = ['ndict', 'omerge', 'omergeleft', 'warn', 'unique', 'find_contacts', 'get_subclasses', 'all_subclasses']
+__all__ = ['ndict', 'warn', 'unique', 'find_contacts']
 
 
 class ndict(sc.objdict):
     """
     A dictionary-like class that provides additional functionalities for handling named items.
 
     Args:
@@ -36,14 +36,18 @@
         super().__init__()
         self.setattribute('_nameattr', nameattr)  # Since otherwise treated as keys
         self.setattribute('_type', type)
         self.setattribute('_strict', strict)
         self.setattribute('_overwrite', overwrite)
         self.extend(*args, **kwargs)
         return
+    
+    def __call__(self):
+        """ Shortcut for returning values """
+        return self.values()
 
     def append(self, arg, key=None, overwrite=None):
         valid = False
         if arg is None:
             return  # Nothing to do
         elif hasattr(arg, self._nameattr):
             key = key or getattr(arg, self._nameattr)
@@ -121,33 +125,14 @@
         if isinstance(dict2, list):
             self.extend(dict2)
         else:
             self.append(dict2)
         return self
 
 
-def omerge(*args, **kwargs):
-    """ Merge things into an objdict, using standard order """
-    return sc.objdict(sc.mergedicts(*args, **kwargs))
-
-
-def omergeleft(*args, **kwargs):
-    """ Merge things into an odict, using opposite order to allow defaults to be supplied second """
-    if len(args) == 1 and len(kwargs):
-        new = args[0]
-        default = kwargs
-    elif len(args) == 2 and len(kwargs) == 0:
-        new = args[0]
-        default = args[1]
-    else:
-        errormsg = 'Expecting either two arguments, or one argument and kwargs; for any other arrangement, use ss.omerge()'
-        raise ValueError(errormsg)
-    return sc.objdict(sc.mergedicts(default, new))
-
-
 def warn(msg, category=None, verbose=None, die=None):
     """ Helper function to handle warnings -- shortcut to warnings.warn """
 
     # Handle inputs
     warnopt = ss.options.warnings if not die else 'error'
     if category is None:
         category = RuntimeWarning
@@ -200,24 +185,14 @@
         if p1[i] in inds:
             pairing_partners.add(p2[i])
         if p2[i] in inds:
             pairing_partners.add(p1[i])
     return pairing_partners
 
 
-def get_subclasses(cls):
-    for subclass in cls.__subclasses__():
-        yield from get_subclasses(subclass)
-        yield subclass
-
-def all_subclasses(cls):
-    """ As above but also returns subsubclases """
-    return set(cls.__subclasses__()).union(
-        [s for c in cls.__subclasses__() for s in all_subclasses(c)])
-
 # %% Seed methods
 
 __all__ += ['set_seed']
 
 def set_seed(seed=None):
     '''
     Reset the random seed -- complicated because of Numba, which requires special
@@ -243,105 +218,14 @@
     if seed is None:  # Numba can't accept a None seed, so use our just-reinitialized Numpy stream to generate one
         seed = np.random.randint(1e9)
     set_seed_numba(seed)
 
     return
 
 
-# %% Simple array operations
-
-__all__ += ['true', 'false', 'defined', 'undefined']
-
-
-@nb.njit(cache=True)
-def _true(uids, values):
-    """
-    Returns the UIDs for indices where the value evaluates as True
-    """
-    out = np.empty(len(uids), dtype=uids.dtype)
-    j = 0
-    for i in range(len(values)):
-        out[j] = uids[i]
-        if values[i]:
-            j += 1
-    out = out[0:j]
-    return out
-
-
-@nb.njit(cache=True)
-def _false(uids, values):
-    """
-    Returns the UIDs for indices where the value evaluates as False
-    """
-    out = np.empty(len(uids), dtype=uids.dtype)
-    j = 0
-    for i in range(len(values)):
-        out[j] = uids[i]
-        if not values[i]:
-            j += 1
-    out = out[0:j]
-    return out
-
-
-def true(state):
-    """
-    Returns the UIDs of the values of the array that are true
-
-    Args:
-        state (State, UIDArray)
-
-    **Example**::
-
-        inds = ss.true(people.alive) # Returns array of UIDs of alive agents
-    """
-    return _true(state.uid.__array__(), state.__array__())
-
-
-def false(state):
-    """
-    Returns the indices of the values of the array that are false.
-
-    Args:
-        state (State, UIDArray)
-
-    **Example**::
-
-        inds = ss.false(people.alive) # Returns array of UIDs of dead agents
-    """
-    return _false(state.uid.__array__(), state.__array__())
-
-
-def defined(arr):
-    """
-    Returns the indices of the values of the array that are not-nan.
-
-    Args:
-        arr (array): any array
-
-    **Example**::
-
-        inds = ss.defined(np.array([1,np.nan,0,np.nan,1,0,1]))
-    """
-    return (~np.isnan(arr)).nonzero()[-1]
-
-
-def undefined(arr):
-    """
-    Returns the indices of the values of the array that are not-nan.
-
-    Args:
-        arr (array): any array
-
-    **Example**::
-
-        inds = ss.defined(np.array([1,np.nan,0,np.nan,1,0,1]))
-    """
-    return np.isnan(arr).nonzero()[-1]
-
-
 # %% Data cleaning and processing
 
 __all__ += ['standardize_data']
 
 
 def standardize_data(data=None, metadata=None, max_age=120, min_year=1800):
     """
@@ -399,15 +283,15 @@
             errormsg = 'Please ensure the keys of the data dict match the values in metadata.data_cols.'
             raise ValueError(errormsg)
         new_data = dict()
         for sim_name, col_name in metadata.data_cols.items():
             new_data[sim_name] = sc.tolist(data[col_name])
         df = sc.dataframe(new_data)
 
-    elif sc.isnumber(data):
+    elif sc.isnumber(data) or isinstance(data, ss.Dist):
         df = data  # Just return it as-is
 
     else:
         errormsg = f'Data type {type(data)} not understood.'
         raise ValueError(errormsg)
-
+        
     return df
```

### Comparing `starsim-0.3.4/starsim.egg-info/PKG-INFO` & `starsim-0.5.0/starsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starsim
-Version: 0.3.4
+Version: 0.5.0
 Summary: Starsim
 Author: Robyn Stuart, Cliff Kerr, Romesh Abeysuriya, Paula Sanz-Leon, Jamie Cohen, and Daniel Klein on behalf of the Starsim Collective
 Keywords: agent-based model,simulation,disease,epidemiology
 Platform: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
```

### Comparing `starsim-0.3.4/tests/test_baselines.py` & `starsim-0.5.0/tests/test_baselines.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,32 +26,32 @@
 def make_people():
     ss.set_seed(pars.rand_seed)
     n_agents = int(10e3)
     ppl = ss.People(n_agents=n_agents)
     return ppl
 
 
-def make_sim(ppl=None, do_plot=False, **kwargs):
+def make_sim(ppl=None, do_run=False, **kwargs):
     '''
     Define a default simulation for testing the baseline, including
     interventions to increase coverage. If run directly (not via pytest), also
     plot the sim by default.
     '''
 
     if ppl is None:
         ppl = make_people()
 
     # Make the sim
     hiv = ss.HIV()
     hiv.pars.beta = {'mf': [0.15, 0.10], 'maternal': [0.2, 0]}
     networks = [ss.MFNet(), ss.MaternalNet()]
     sim = ss.Sim(pars=pars, people=ppl, networks=networks, demographics=ss.Pregnancy(), diseases=hiv)
-
-    # Optionally plot
-    if do_plot:
+    
+    # Optionally run and plot
+    if do_run:
         sim.run()
         sim.plot()
 
     return sim
 
 
 def save_baseline():
@@ -205,12 +205,12 @@
 
     # Start timing and optionally enable interactive plotting
     sc.options(interactive=do_plot)
     T = sc.tic()
 
     json = test_benchmark(do_save=do_save, repeats=5) # Run this first so benchmarking is available even if results are different
     new  = test_baseline()
-    sim = make_sim(do_plot=do_plot)
+    sim = make_sim(do_run=do_plot)
 
     print('\n'*2)
     sc.toc(T)
     print('Done.')
```

### Comparing `starsim-0.3.4/tests/test_demographics.py` & `starsim-0.5.0/tests/test_demographics.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as np
 import sciris as sc
 import pytest
 
 
-do_plot = True
 sc.options(interactive=False) # Assume not running interactively
 
 
-def test_nigeria(which='births', dt=1, start=1995, n_years=15, plot_init=False, do_plot=True):
+def test_nigeria(which='births', dt=1, start=1995, n_years=15, do_plot=False):
     """
     Make a Nigeria sim with demographic modules
     Switch between which='births' or 'pregnancy' to determine which demographic module to use
     """
+    sc.heading('Testing Nigeria demographics')
 
     # Make demographic modules
     demographics = sc.autolist()
 
     if which == 'births':
         birth_rates = pd.read_csv(ss.root / 'tests/test_data/nigeria_births.csv')
         births = ss.Births(pars={'birth_rate': birth_rates})
@@ -49,15 +49,15 @@
         total_pop=nga_pop_1995,
         start=start,
         n_years=n_years,
         people=ppl,
         demographics=demographics,
     )
 
-    if plot_init:
+    if do_plot:
         sim.initialize()
         # Plot histograms of the age distributions - simulated vs data
         bins = np.arange(0, 101, 1)
         init_scale = nga_pop_1995 / n_agents
         counts, bins = np.histogram(sim.people.age, bins)
         plt.bar(bins[:-1], counts * init_scale, alpha=0.5, label='Simulated')
         plt.bar(bins, age_data.value.values * 1000, alpha=0.5, color='r', label='Data')
@@ -119,35 +119,75 @@
             ax[3].legend()
 
         fig.tight_layout()
 
     return sim
 
 
-def test_constant_pop():
-    # Test pars for constant pop size
+def test_constant_pop(do_plot=False):
+    """ Test pars for constant pop size """
+    sc.heading('Testing constant population size')
     sim = ss.Sim(n_agents=10e3, birth_rate=10, death_rate=10/1010*1000, n_years=200, rand_seed=1).run()
     print("Check final pop size within 5% of starting pop")
     assert np.isclose(sim.results.n_alive[0], sim.results.n_alive[-1], rtol=0.05)
     print(f'✓ (final pop / starting pop={sim.results.n_alive[-1] / sim.results.n_alive[0]:.2f})')
 
     # Plots
     if do_plot:
         sim.plot()
     return sim
 
 
 def test_module_adding():
+    """ Test that modules can't be added twice """
+    sc.heading('Testing module duplication')
     births = ss.Births(pars={'birth_rate': 10})
     deaths = ss.Deaths(pars={'death_rate': 10})
     demographics = [births, deaths]
     with pytest.raises(Exception): # CK: should be ValueError, but that fails for now, and this is OK
         ss.Sim(n_agents=1e3, demographics=demographics, birth_rate=10, death_rate=10).run()
     return demographics
 
 
+def test_aging():
+    """ Test that aging is configured properly """
+    sc.heading('Testing aging')
+    n_agents = int(1e3)
+    
+    # With no demograhpics, people shouldn't age
+    s1 = ss.Sim(n_agents=n_agents).initialize()
+    orig_ages = s1.people.age.raw.copy()
+    orig_age = orig_ages.mean()
+    s1.run()
+    end_age = s1.people.age.mean()
+    assert orig_age == end_age, f'By default there should be no aging, but {orig_age} != {end_age}'
+    
+    # We should be able to manually turn on aging
+    s2 = ss.Sim(n_agents=n_agents, use_aging=True).run()
+    age2 = s2.people.age.mean()
+    assert orig_age < age2, f'With aging, start age {orig_age} should be less than end age {age2}'
+    
+    # Aging should turn on automatically if we add demographics
+    s3 = ss.Sim(n_agents=n_agents, demographics=True).run()
+    agent = s3.people.auids[0] # Find first alive agent
+    orig_agent_age = orig_ages[agent]
+    age3 = s3.people.age[ss.uids(agent)]
+    assert orig_agent_age < age3, f'With demographics, original agent age {orig_agent_age} should be less than end age {age3}'
+    
+    # ...but can be turned off manually
+    s4 = ss.Sim(n_agents=n_agents, demographics=True, use_aging=False).run()
+    agent = s4.people.auids[0] # Find first alive agent
+    orig_agent_age = orig_ages[agent]
+    age4 = s4.people.age[ss.uids(agent)]
+    assert orig_agent_age == age4, f'With aging turned off, original agent age {orig_agent_age} should match end age {age4}'
+
+    return s3 # Most interesting sim
+
+
 if __name__ == '__main__':
+    do_plot = True
     sc.options(interactive=do_plot)
-    s1 = test_nigeria(dt=1, which='pregnancy', n_years=15, plot_init=True, do_plot=do_plot)
-    s2 = test_constant_pop()
+    s1 = test_nigeria(do_plot=do_plot)
+    s2 = test_constant_pop(do_plot=do_plot)
     s3 = test_module_adding()
+    s4 = test_aging()
     plt.show()
```

### Comparing `starsim-0.3.4/tests/test_dist.py` & `starsim-0.5.0/tests/test_dist.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,37 +23,43 @@
         title = times[name] if times else name
         pl.title(title)
         sc.commaticks()
     sc.figlayout()
     return fig
 
 
+def make_sim():
+    """ Make a tiny sim for initializing the distributions """
+    sim = ss.Sim(n_agents=100).initialize() # Need an empty sim to initialize properly
+    return sim
+
+
 # %% Define the tests
 def test_dist(m=m):
     """ Test the Dist class """
     sc.heading('Testing the basic Dist call')
-    dist = ss.Dist(distname='random', name='test')
+    dist = ss.Dist(distname='random', name='test', strict=False)
     dist.initialize()
     rvs = dist(m)
     print(rvs)
     assert 0 < rvs.min() < 1, 'Values should be between 0 and 1'
     return rvs
 
 
 def test_custom_dists(n=n, do_plot=False):
     """ Test all custom dists """
     sc.heading('Testing all custom distributions')
     
-    o = sc.objdict()
+    o     = sc.objdict()
     dists = sc.objdict()
-    rvs = sc.objdict()
+    rvs   = sc.objdict()
     times = sc.objdict()
     for name in ss.dist_list:
         func = getattr(ss, name)
-        dist = func(name='test')
+        dist = func(name='test', strict=False)
         dist.initialize()
         dists[name] = dist
         sc.tic()
         rvs[name] = dist.rvs(n)
         times[name] = sc.toc(name, unit='ms', output='message')
         print(f'{name:10s}: mean = {rvs[name].mean():n}')
     
@@ -75,15 +81,15 @@
     for i in range(2):
         
         # Create a complex object containing various distributions
         obj = sc.prettyobj()
         obj.a = sc.objdict()
         obj.a.mylist = [ss.random(), ss.Dist(distname='uniform', low=2, high=3)]
         obj.b = dict(d3=ss.weibull(c=2), d4=ss.delta(v=0.3))
-        dists = ss.Dists(obj)
+        dists = ss.Dists(obj).initialize(sim=make_sim())
         
         # Call each distribution twice
         for j in range(2):
             rvs = sc.objdict()
             for key,dist in dists.dists.items():
                 rvs[str(dist)] = dist(n)
                 dist.jump() # Reset
@@ -104,16 +110,16 @@
 
 
 def test_scipy(m=m):
     """ Test that SciPy distributions also work """
     sc.heading('Testing SciPy distributions')
     
     # Make SciPy distributions in two different ways
-    dist1 = ss.Dist(dist=sps.expon, name='scipy', scale=2).initialize() # Version 1: callable
-    dist2 = ss.Dist(dist=sps.expon(scale=2), name='scipy').initialize() # Version 2: frozen
+    dist1 = ss.Dist(dist=sps.expon, name='scipy', scale=2, strict=False).initialize() # Version 1: callable
+    dist2 = ss.Dist(dist=sps.expon(scale=2), name='scipy', strict=False).initialize() # Version 2: frozen
     rvs1 = dist1(m)
     rvs2 = dist2(m)
     
     # Check that they match
     print(rvs1)
     assert np.array_equal(rvs1, rvs2), 'Arrays should match'
     
@@ -126,21 +132,22 @@
     
     # Create a strict distribution
     dist = ss.random(strict=True, auto=False)
     with pytest.raises(ss.distributions.DistNotInitializedError):
         dist(m) # Check that we can't call an uninitialized
     
     # Initialize and check we can't call repeatedly
-    dist.initialize()
+    dist.initialize(trace='test', sim=make_sim())
     rvs = dist(m)
     with pytest.raises(ss.distributions.DistNotReadyError):
         dist(m) # Check that we can't call an already-used distribution
     
     # Check that we can with a non-strict Dist
     dist2 = ss.random(strict=False)
+    dist2.initialize(trace='test')
     rvs2 = sc.autolist()
     for i in range(2):
         rvs2 += dist2(m) # We should be able to call multiple times with no problem
     
     print(rvs)
     print(rvs2)
     assert np.array_equal(rvs, rvs2[0]), 'Separate dists should match'
@@ -150,15 +157,15 @@
     
 
 def test_reset(m=m):
     """ Check that reset works as expected """
     sc.heading('Testing reset')
     
     # Create and draw two sets of random numbers
-    dist = ss.random(seed=533).initialize()
+    dist = ss.random(seed=533, strict=False).initialize()
     r1 = dist.rvs(m)
     r2 = dist.rvs(m)
     assert all(r1 != r2)
     
     # Reset to the most recent state
     dist.reset(-1)
     r3 = dist.rvs(m)
@@ -189,15 +196,15 @@
 
     # Define a parameter as a function
     def custom_loc(module, sim, uids):
         out = sim.people.age[uids]
         return out
     
     scale = 1
-    d = ss.normal(loc=custom_loc, scale=scale).initialize(sim=sim)
+    d = ss.normal(name='callable', loc=custom_loc, scale=scale).initialize(sim=sim)
 
     uids = np.array([1, 3, 7, 9])
     draws = d.rvs(uids)
     print(f'Input ages were: {sim.people.age[uids]}')
     print(f'Output samples were: {draws}')
 
     meandiff = np.abs(sim.people.age[uids] - draws).mean()
@@ -209,15 +216,15 @@
     """ Test array parameters """
     sc.heading('Testing uniform with a array parameters')
 
     uids = np.array([1, 3])
     low  = np.array([1, 100]) # Low
     high = np.array([3, 125]) # High
 
-    d = ss.uniform(low=low, high=high).initialize(slots=np.arange(uids.max()+1))
+    d = ss.uniform(low=low, high=high, strict=False).initialize(slots=np.arange(uids.max()+1))
     draws = d.rvs(uids)
     print(f'Uniform sample for uids {uids} returned {draws}')
 
     assert len(draws) == len(uids)
     for i in range(len(uids)):
         assert low[i] < draws[i] < low[i] + high[i], 'Invalid value'
     return draws
@@ -231,15 +238,15 @@
     slots = np.array([4,2,3,2,2,3])
     n = len(slots)
     uids = np.arange(n)
     low = np.arange(n)
     high = low + 1
 
     # Draw values
-    d = ss.uniform(low=low, high=high).initialize(slots=slots)
+    d = ss.uniform(low=low, high=high, strict=False).initialize(slots=slots)
     draws = d.rvs(uids)
     
     # Print and test
     print(f'Uniform sample for slots {slots} returned {draws}')
     assert len(draws) == len(slots)
 
     unique_slots = np.unique(slots)
```

### Comparing `starsim-0.3.4/tests/test_dists.py` & `starsim-0.5.0/tests/test_randomness.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 def make_dist(name='test', **kwargs):
     """ Make a default Dist for testing """
     dist = ss.random(name=name, **kwargs)
     return dist
 
 def make_dists(**kwargs):
     """ Make a Dists object with two distributions in it """
+    sim = ss.Sim(n_agents=100).initialize() # Need an empty sim to initialize properly
     distlist = [make_dist(), make_dist()]
     dists = ss.Dists(distlist)
-    dists.initialize()
+    dists.initialize(sim=sim)
     return dists
 
 
 # %% Define the tests
 
 def test_seed():
     """ Test assignment of seeds """
@@ -118,27 +119,29 @@
     def apply(self, sim):
         self.arr[sim.ti, :] = np.array(sim.diseases.sir.infected)[:self.n_agents]
         return
 
 
 class OneMore(ss.Intervention):
     """ Add one additional agent and infection """
-    def apply(self, sim):
-        if sim.ti == 0:
-            # Create an extra agent
-            preg = ss.Pregnancy(rel_fertility=0) # Ensure no default births
-            preg.initialize(sim)
-            new_uids = np.array([len(sim.people)]) # Hack since make_embryos doesn't return UIDs
-            preg.make_embryos(sim, np.array([0])) # Assign 0th agent to be the "mother"
-            assert len(new_uids) == 1
+    def initialize(self, sim):
+        one_birth = ss.Pregnancy(name='one_birth', rel_fertility=0) # Ensure no default births
+        one_birth.initialize(sim)
+        self.one_birth = one_birth
+        return
+    
+    def apply(self, sim, ti=10):
+        """ Create an extra agent """
+        if sim.ti == ti:
+            new_uids = self.one_birth.make_embryos(ss.uids(0)) # Assign 0th agent to be the "mother"
             sim.people.age[new_uids] = -100 # Set to a very low number to never reach debut age
             
-            # Infect that agent
+            # Infect that agent and immediately recover
             sir = sim.diseases.sir
-            sir.set_prognoses(sim, new_uids)
+            sir.set_prognoses(new_uids)
             sir.ti_recovered[new_uids] = sim.ti + 1 # Reset recovery time to next timestep
             
             # Reset the random states
             p = sir.pars
             for dist in [p.dur_inf, p.p_death]:
                 dist.jump(sim.ti+1)
 
@@ -166,14 +169,16 @@
     pl.title('Difference')
     
     sc.figlayout()
     return fig
 
 
 def test_worlds(do_plot=False):
+    """ Test that one extra birth leads to one extra infection """
+    sc.heading('Testing worlds...')
     
     res = sc.objdict()
     
     pars = dict(
         start = 2000,
         end = 2100,
         n_agents = 200,
@@ -202,26 +207,96 @@
     res.sum2 = sum2
     
     if do_plot:
         s1.plot()
         plot_infs(s1, s2)
         pl.show()
     
-    assert len(s2.people) == len(s1.people) + 1
-    assert sum2.sir_cum_infections == sum1.sir_cum_infections + 1
-    assert (s1.interventions.countinf.arr != s2.interventions.countinf.arr).sum() == 0
+    l1 = len(s1.people)
+    l2 = len(s2.people)
+    i1 = sum1.sir_cum_infections
+    i2 = sum2.sir_cum_infections
+    a1 = s1.interventions.countinf.arr
+    a2 = s2.interventions.countinf.arr
+    assert l2 == l1 + 1, f'Expected one more person in s2 ({l2}) than s1 ({l1})'
+    assert i2 == i1 + 1, f'Expected one more infection in s2 ({i2}) than s1 ({i1})'
+    assert (a1 != a2).sum() == 0, f'Expected infection arrays to match:\n{a1}\n{a2}'
         
     return res
 
 
+def test_independence(do_plot=False, thresh=0.1):
+    """ Test that when variables are created, they are uncorrelated """
+    sc.heading('Testing independence...')
+    
+    # Create the sim and initialize (do not run)
+    sim = ss.Sim(
+        n_agents = 1000,
+        diseases = [
+            dict(type='sir', init_prev=0.1),
+            dict(type='sis', init_prev=0.1),
+            dict(type='hiv', init_prev=0.1),
+        ],
+        networks = [
+            dict(type='random', n_contacts=ss.poisson(8)),
+            dict(type='mf', debut=ss.delta(0), participation=0.5), # To avoid age correlations
+        ]
+    )
+    sim.initialize()
+    
+    # Assemble measures
+    st = sim.people.states
+    arrs = sc.objdict()
+    arrs.age = st.age.values
+    arrs.sex = st.female.values
+    for key,disease in sim.diseases.items():
+        arrs[f'{key}_init'] = disease.infected.values
+    for key,network in sim.networks.items():
+        data = np.zeros(len(sim.people))
+        for p in ['p1', 'p2']:
+            for uid in network.contacts[p]:
+                data[uid] += 1 # Could also use a histogram
+        arrs[key] = data
+    
+    # Compute the correlations
+    n = len(arrs)
+    stats = np.zeros((n,n))
+    for i,arr1 in arrs.enumvals():
+        for j,arr2 in arrs.enumvals():
+            if i != j:
+                stats[i,j] = np.corrcoef(arr1, arr2)[0,1]
+                
+    # Optionally plot
+    if do_plot:
+        pl.figure()
+        pl.imshow(stats)
+        ticks = np.arange(n)
+        labels = arrs.keys()
+        pl.xticks(ticks, labels)
+        pl.yticks(ticks, labels)
+        pl.xticks(rotation=15)
+        pl.colorbar()
+        sc.figlayout()
+        pl.show()
+            
+    # Test that everything is independent
+    max_corr = abs(stats).max()
+    assert max_corr < thresh, f'The maximum correlation between variables was {max_corr}, above the threshold {thresh}'
+    
+    return sim
+    
+
+
 # %% Run as a script
 if __name__ == '__main__':
     T = sc.timer()
     do_plot = True
 
     o1 = test_seed()
     o2 = test_reset(n)
     o3 = test_jump(n)
     o4 = test_order(n)
     o5 = test_worlds(do_plot=do_plot)
+    o6 = test_independence(do_plot=do_plot)
 
     T.toc()
+
```

### Comparing `starsim-0.3.4/tests/test_samples.py` & `starsim-0.5.0/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.4/tests/test_syphilis.py` & `starsim-0.5.0/tests/test_syphilis.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         product='rpr',
         prob=0.99,
         eligibility=screen_eligible,
         start_year=2020,
         label='syph_screening',
     )
 
-    treat_eligible = lambda sim: sim.get_intervention('syph_screening').outcomes['positive']
+    treat_eligible = lambda sim: ss.uids(sim.get_intervention('syph_screening').outcomes['positive'])
     bpg = ss.syph_treatment(
         prob=0.9,
         product='bpg',
         eligibility=treat_eligible,
         label='bpg'
     )
```

