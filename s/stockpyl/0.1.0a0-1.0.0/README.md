# Comparing `tmp/stockpyl-0.1.0a0.tar.gz` & `tmp/stockpyl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stockpyl-0.1.0a0.tar", last modified: Tue Feb 22 21:42:56 2022, max compression
+gzip compressed data, was "stockpyl-1.0.0.tar", last modified: Tue May 14 11:48:33 2024, max compression
```

## Comparing `stockpyl-0.1.0a0.tar` & `stockpyl-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,71 @@
-drwxr-xr-x   0 larry      (501) staff       (20)        0 2022-02-22 21:42:56.000000 stockpyl-0.1.0a0/
--rw-r--r--   0 larry      (501) staff       (20)      672 2022-02-22 21:42:56.000000 stockpyl-0.1.0a0/PKG-INFO
-drwxr-xr-x   0 larry      (501) staff       (20)        0 2022-02-22 21:42:56.000000 stockpyl-0.1.0a0/stockpyl/
--rw-r--r--   0 larry      (501) staff       (20)    37715 2022-02-02 22:37:31.000000 stockpyl-0.1.0a0/stockpyl/loss_functions.py
--rw-r--r--   0 larry      (501) staff       (20)    21742 2022-02-03 01:27:15.000000 stockpyl-0.1.0a0/stockpyl/sim.py
--rw-r--r--   0 larry      (501) staff       (20)    30260 2022-02-03 00:53:04.000000 stockpyl-0.1.0a0/stockpyl/newsvendor.py
--rw-r--r--   0 larry      (501) staff       (20)     6942 2022-02-22 21:39:52.000000 stockpyl-0.1.0a0/stockpyl/instances.py
--rw-r--r--   0 larry      (501) staff       (20)    29577 2022-02-03 23:51:36.000000 stockpyl-0.1.0a0/stockpyl/finite_horizon.py
--rw-r--r--   0 larry      (501) staff       (20)    12902 2022-02-22 21:39:52.000000 stockpyl-0.1.0a0/stockpyl/policy.py
--rw-r--r--   0 larry      (501) staff       (20)     2628 2022-02-02 22:37:15.000000 stockpyl-0.1.0a0/stockpyl/optimization.py
--rw-r--r--   0 larry      (501) staff       (20)    21860 2022-02-03 00:53:02.000000 stockpyl-0.1.0a0/stockpyl/rq.py
--rw-r--r--   0 larry      (501) staff       (20)        0 2022-02-02 22:29:23.000000 stockpyl-0.1.0a0/stockpyl/__init__.py
--rw-r--r--   0 larry      (501) staff       (20)     3419 2022-02-02 22:29:23.000000 stockpyl-0.1.0a0/stockpyl/gsm_tree_willems_data.py
--rw-r--r--   0 larry      (501) staff       (20)    23899 2022-02-02 22:29:23.000000 stockpyl-0.1.0a0/stockpyl/meio.py
--rw-r--r--   0 larry      (501) staff       (20)    30665 2022-02-22 21:39:52.000000 stockpyl-0.1.0a0/stockpyl/supply_chain_node.py
--rw-r--r--   0 larry      (501) staff       (20)    22267 2022-02-03 00:31:56.000000 stockpyl-0.1.0a0/stockpyl/supply_uncertainty.py
--rw-r--r--   0 larry      (501) staff       (20)    41841 2022-02-22 21:39:52.000000 stockpyl-0.1.0a0/stockpyl/supply_chain_network.py
--rw-r--r--   0 larry      (501) staff       (20)     6639 2022-02-22 21:39:52.000000 stockpyl-0.1.0a0/stockpyl/gsm_tree_helpers.py
--rw-r--r--   0 larry      (501) staff       (20)     5829 2022-02-02 22:36:57.000000 stockpyl-0.1.0a0/stockpyl/sim_io.py
--rw-r--r--   0 larry      (501) staff       (20)    13132 2022-02-22 21:39:52.000000 stockpyl-0.1.0a0/stockpyl/demand_source.py
--rw-r--r--   0 larry      (501) staff       (20)    13284 2022-02-03 00:53:00.000000 stockpyl-0.1.0a0/stockpyl/ss.py
--rw-r--r--   0 larry      (501) staff       (20)    12202 2022-02-03 00:53:07.000000 stockpyl-0.1.0a0/stockpyl/eoq.py
--rw-r--r--   0 larry      (501) staff       (20)    19862 2022-02-22 21:39:52.000000 stockpyl-0.1.0a0/stockpyl/helpers.py
--rw-r--r--   0 larry      (501) staff       (20)    33474 2022-02-22 21:39:52.000000 stockpyl-0.1.0a0/stockpyl/gsm_tree.py
--rw-r--r--   0 larry      (501) staff       (20)    34451 2022-02-22 21:39:52.000000 stockpyl-0.1.0a0/stockpyl/ssm_serial.py
--rw-r--r--   0 larry      (501) staff       (20)     8915 2022-02-03 00:52:56.000000 stockpyl-0.1.0a0/stockpyl/wagner_whitin.py
-drwxr-xr-x   0 larry      (501) staff       (20)        0 2022-02-22 21:42:56.000000 stockpyl-0.1.0a0/datasets/
--rw-r--r--   0 larry      (501) staff       (20)    76429 2022-02-22 21:39:52.000000 stockpyl-0.1.0a0/datasets/stockpyl_instances.json
-drwxr-xr-x   0 larry      (501) staff       (20)        0 2022-02-22 21:42:56.000000 stockpyl-0.1.0a0/stockpyl.egg-info/
--rw-r--r--   0 larry      (501) staff       (20)      672 2022-02-22 21:42:55.000000 stockpyl-0.1.0a0/stockpyl.egg-info/PKG-INFO
--rw-r--r--   0 larry      (501) staff       (20)        1 2022-02-22 21:32:16.000000 stockpyl-0.1.0a0/stockpyl.egg-info/not-zip-safe
--rw-r--r--   0 larry      (501) staff       (20)      788 2022-02-22 21:42:55.000000 stockpyl-0.1.0a0/stockpyl.egg-info/SOURCES.txt
--rw-r--r--   0 larry      (501) staff       (20)      100 2022-02-22 21:42:55.000000 stockpyl-0.1.0a0/stockpyl.egg-info/requires.txt
--rw-r--r--   0 larry      (501) staff       (20)        9 2022-02-22 21:42:55.000000 stockpyl-0.1.0a0/stockpyl.egg-info/top_level.txt
--rw-r--r--   0 larry      (501) staff       (20)        1 2022-02-22 21:42:55.000000 stockpyl-0.1.0a0/stockpyl.egg-info/dependency_links.txt
--rw-r--r--   0 larry      (501) staff       (20)       17 2022-02-22 21:39:52.000000 stockpyl-0.1.0a0/MANIFEST.in
--rw-r--r--   0 larry      (501) staff       (20)       41 2022-02-02 22:29:23.000000 stockpyl-0.1.0a0/README.md
--rw-r--r--   0 larry      (501) staff       (20)     1006 2022-02-22 21:42:39.000000 stockpyl-0.1.0a0/setup.py
--rw-r--r--   0 larry      (501) staff       (20)       38 2022-02-22 21:42:56.000000 stockpyl-0.1.0a0/setup.cfg
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2024-05-14 11:48:33.510002 stockpyl-1.0.0/
+-rw-r--r--   0 larry      (502) staff       (20)    35149 2022-06-15 01:54:09.000000 stockpyl-1.0.0/LICENSE
+-rw-r--r--   0 larry      (502) staff       (20)       79 2022-06-28 22:13:53.000000 stockpyl-1.0.0/MANIFEST.in
+-rw-r--r--   0 larry      (502) staff       (20)     5214 2024-05-14 11:48:33.509922 stockpyl-1.0.0/PKG-INFO
+-rw-r--r--   0 larry      (502) staff       (20)     4139 2023-11-11 19:13:12.000000 stockpyl-1.0.0/README.md
+-rw-r--r--   0 larry      (502) staff       (20)       99 2022-06-15 01:54:09.000000 stockpyl-1.0.0/pyproject.toml
+-rw-r--r--   0 larry      (502) staff       (20)     1339 2024-05-14 11:48:33.510508 stockpyl-1.0.0/setup.cfg
+-rw-r--r--   0 larry      (502) staff       (20)       66 2022-06-15 01:54:09.000000 stockpyl-1.0.0/setup.py
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2024-05-14 11:48:33.495492 stockpyl-1.0.0/src/
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2024-05-14 11:48:33.501939 stockpyl-1.0.0/src/stockpyl/
+-rw-r--r--   0 larry      (502) staff       (20)        0 2022-06-02 12:18:00.000000 stockpyl-1.0.0/src/stockpyl/__init__.py
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2024-05-14 11:48:33.503622 stockpyl-1.0.0/src/stockpyl/datasets/
+-rw-r--r--   0 larry      (502) staff       (20)   410251 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/datasets/stockpyl_instances.json
+-rw-r--r--   0 larry      (502) staff       (20)    22506 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/demand_source.py
+-rw-r--r--   0 larry      (502) staff       (20)    14943 2022-07-15 21:43:50.000000 stockpyl-1.0.0/src/stockpyl/disruption_process.py
+-rw-r--r--   0 larry      (502) staff       (20)    12320 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/eoq.py
+-rw-r--r--   0 larry      (502) staff       (20)    31671 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/finite_horizon.py
+-rw-r--r--   0 larry      (502) staff       (20)    10257 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/gsm_helpers.py
+-rw-r--r--   0 larry      (502) staff       (20)    10622 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/gsm_serial.py
+-rw-r--r--   0 larry      (502) staff       (20)    35951 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/gsm_tree.py
+-rw-r--r--   0 larry      (502) staff       (20)    36037 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/helpers.py
+-rw-r--r--   0 larry      (502) staff       (20)     9292 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/instances.py
+-rw-r--r--   0 larry      (502) staff       (20)    39022 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/loss_functions.py
+-rw-r--r--   0 larry      (502) staff       (20)    20537 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/meio_general.py
+-rw-r--r--   0 larry      (502) staff       (20)    33042 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/newsvendor.py
+-rw-r--r--   0 larry      (502) staff       (20)    67625 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/node_state_vars.py
+-rw-r--r--   0 larry      (502) staff       (20)     2673 2022-06-25 17:25:02.000000 stockpyl-1.0.0/src/stockpyl/optimization.py
+-rw-r--r--   0 larry      (502) staff       (20)    22003 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/policy.py
+-rw-r--r--   0 larry      (502) staff       (20)    22756 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/rq.py
+-rw-r--r--   0 larry      (502) staff       (20)    47979 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/sim.py
+-rw-r--r--   0 larry      (502) staff       (20)    16235 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/sim_io.py
+-rw-r--r--   0 larry      (502) staff       (20)    13675 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/ss.py
+-rw-r--r--   0 larry      (502) staff       (20)    37084 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/ssm_serial.py
+-rw-r--r--   0 larry      (502) staff       (20)    59429 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/supply_chain_network.py
+-rw-r--r--   0 larry      (502) staff       (20)    79931 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/supply_chain_node.py
+-rw-r--r--   0 larry      (502) staff       (20)    23210 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/supply_chain_product.py
+-rw-r--r--   0 larry      (502) staff       (20)    22457 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/supply_uncertainty.py
+-rw-r--r--   0 larry      (502) staff       (20)     4886 2024-05-14 11:09:59.000000 stockpyl-1.0.0/src/stockpyl/wagner_whitin.py
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2024-05-14 11:48:33.509554 stockpyl-1.0.0/src/stockpyl.egg-info/
+-rw-r--r--   0 larry      (502) staff       (20)     5214 2024-05-14 11:48:33.000000 stockpyl-1.0.0/src/stockpyl.egg-info/PKG-INFO
+-rw-r--r--   0 larry      (502) staff       (20)     1694 2024-05-14 11:48:33.000000 stockpyl-1.0.0/src/stockpyl.egg-info/SOURCES.txt
+-rw-r--r--   0 larry      (502) staff       (20)        1 2024-05-14 11:48:33.000000 stockpyl-1.0.0/src/stockpyl.egg-info/dependency_links.txt
+-rw-r--r--   0 larry      (502) staff       (20)        1 2022-06-02 14:15:38.000000 stockpyl-1.0.0/src/stockpyl.egg-info/not-zip-safe
+-rw-r--r--   0 larry      (502) staff       (20)      189 2024-05-14 11:48:33.000000 stockpyl-1.0.0/src/stockpyl.egg-info/requires.txt
+-rw-r--r--   0 larry      (502) staff       (20)        9 2024-05-14 11:48:33.000000 stockpyl-1.0.0/src/stockpyl.egg-info/top_level.txt
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2024-05-14 11:48:33.509314 stockpyl-1.0.0/tests/
+-rw-r--r--   0 larry      (502) staff       (20)    37762 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_demand_source.py
+-rw-r--r--   0 larry      (502) staff       (20)    19210 2024-04-22 02:22:27.000000 stockpyl-1.0.0/tests/test_disruption_process.py
+-rw-r--r--   0 larry      (502) staff       (20)    15590 2022-07-14 01:33:46.000000 stockpyl-1.0.0/tests/test_eoq.py
+-rw-r--r--   0 larry      (502) staff       (20)    17638 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_finite_horizon.py
+-rw-r--r--   0 larry      (502) staff       (20)    17900 2022-07-17 13:54:47.000000 stockpyl-1.0.0/tests/test_gsm_helpers.py
+-rw-r--r--   0 larry      (502) staff       (20)     5406 2022-07-18 01:14:44.000000 stockpyl-1.0.0/tests/test_gsm_serial.py
+-rw-r--r--   0 larry      (502) staff       (20)    76136 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_gsm_tree.py
+-rw-r--r--   0 larry      (502) staff       (20)    42318 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_helpers.py
+-rw-r--r--   0 larry      (502) staff       (20)    15147 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_instances.py
+-rw-r--r--   0 larry      (502) staff       (20)    46866 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_loss_functions.py
+-rw-r--r--   0 larry      (502) staff       (20)    16417 2024-03-11 01:38:31.000000 stockpyl-1.0.0/tests/test_meio_general.py
+-rw-r--r--   0 larry      (502) staff       (20)    40360 2024-03-11 01:36:09.000000 stockpyl-1.0.0/tests/test_newsvendor.py
+-rw-r--r--   0 larry      (502) staff       (20)    43809 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_node_state_vars.py
+-rw-r--r--   0 larry      (502) staff       (20)     2604 2023-05-23 14:09:59.000000 stockpyl-1.0.0/tests/test_optimization.py
+-rw-r--r--   0 larry      (502) staff       (20)    15946 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_policy.py
+-rw-r--r--   0 larry      (502) staff       (20)    19461 2024-03-11 01:45:08.000000 stockpyl-1.0.0/tests/test_rq.py
+-rw-r--r--   0 larry      (502) staff       (20)    74063 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_sim.py
+-rw-r--r--   0 larry      (502) staff       (20)    25537 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_sim_io.py
+-rw-r--r--   0 larry      (502) staff       (20)     8408 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_ss.py
+-rw-r--r--   0 larry      (502) staff       (20)    43246 2023-05-23 14:17:13.000000 stockpyl-1.0.0/tests/test_ssm_serial.py
+-rw-r--r--   0 larry      (502) staff       (20)    74433 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_supply_chain_network.py
+-rw-r--r--   0 larry      (502) staff       (20)   159279 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_supply_chain_node.py
+-rw-r--r--   0 larry      (502) staff       (20)    19452 2024-05-14 11:09:59.000000 stockpyl-1.0.0/tests/test_supply_chain_product.py
+-rw-r--r--   0 larry      (502) staff       (20)    19130 2022-07-14 01:33:47.000000 stockpyl-1.0.0/tests/test_supply_uncertainty.py
+-rw-r--r--   0 larry      (502) staff       (20)     5342 2022-07-14 01:33:47.000000 stockpyl-1.0.0/tests/test_wagner_whitin.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `stockpyl-0.1.0a0/stockpyl/loss_functions.py` & `stockpyl-1.0.0/src/stockpyl/loss_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 # ===============================================================================
 # stockpyl - loss_functions Module
 # -------------------------------------------------------------------------------
-# Version: 0.0.0
-# Updated: 01-31-2022
 # Author: Larry Snyder
 # License: GPLv3
 # ===============================================================================
 
-"""The :mod:`loss_functions` module contains code for calculating loss functions.
+"""
+.. include:: ../../globals.inc
+
+Overview 
+--------
+
+The |mod_loss_functions| module contains code for calculating loss functions.
 
 For a random variable :math:`X`, the loss function, :math:`n(x)`, and the
 complementary loss function, :math:`\\bar{n}(x)`, are defined as:
 
 	* :math:`n(x) = E[(X-x)^+]`
 	* :math:`\\bar{n}(x) = E[(X-x)^-]`,
 
 where :math:`x^+ = \\max\\{x,0\\}` and :math:`x^- = |\\min\\{x,0\\}|`. The second-order
 loss function, :math:`n^{(2)}(x)`, and the second-order complementary loss function,
 :math:`\\bar{n}^{(2)}(x)`, are defined as:
 
 	* :math:`n^{(2)}(x) = \\frac{1}{2}E\\left[\\left([X-x]^+\\right)^2\\right]`
 	* :math:`\\bar{n}^{(2)}(x) = \\frac{1}{2}E\\left[\\left([X-x]^-\\right)^2\\right]`
 
-Equation and section numbers refer to Snyder and Shen, "Fundamentals of Supply
-Chain Theory", Wiley, 2019, 2nd ed., except as noted.
+.. note:: |fosct_notation|
 
-(c) Lawrence V. Snyder
-Lehigh University
+
+API Reference
+-------------
 
 """
 
 import numpy as np
 from scipy.stats import norm
 from scipy.stats import poisson
 from scipy.stats import nbinom
 from scipy.stats import gamma
 #from scipy.integrate import quad
 from types import *
-from numbers import Number
-from numbers import Integral
+import math
 
 from stockpyl.helpers import *
 
 
 ####################################################
 # CONTINUOUS DISTRIBUTIONS
 ####################################################
@@ -251,14 +254,62 @@
 	L2, L2_bar = standard_normal_second_loss(z)
 	n = sd**2 * L2
 	n_bar = sd**2 * L2_bar
 
 	return n, n_bar
 
 
+def standard_normal_loss_dict(start=-4, stop=4, step=0.01, complementary=False):
+	"""Return a dictionary whose keys range from ``start`` to ``stop`` in intervals of ``step``, 
+	and whose values are the standard normal loss function
+	values corresponding to those keys. If going from ``start`` in increments of ``step``
+	overshoots ``stop``, ends at the largest value before ``stop``. If ``complementary`` is ``False``,
+	the dictionary values are the standard normal complementary loss function.
+	
+	Default values return :math:`\\mathscr{L}^{(2)}(z)`
+	for :math:`z = -4.00, -3.99, -3.98, \ldots, 3.98, 3.99, 4.00`.
+
+	**Note:** Because of how floating point arithmetic works, the dictionary keys will not
+	precisely equal the desired values. Therefore, the resulting dictionary is difficult to 
+	use by calling it directly. For example, 0.55 is unlikely to be a key in the dictionary 
+	returned, even if the input parameters suggest that it should; instead, the key might be
+	represented as, say, 0.5499999999999593. Therefore, to determine the value of the loss function
+	for 0.55, you must generally search for the nearest key to 0.55 and take the corresponding value.
+	(The ``helpers.nearest_dict_value()`` function does just that.)
+
+	Parameters
+	----------
+	start : float, optional
+		The start value to calculate the loss function for, by default -4
+	stop : float, optional
+		The start value to calculate the loss function for, by default 4
+	step : float, optional
+		The interval between values to calculate the loss function for, by default 0.01
+	complementary : bool, optional
+		Set to ``True`` to return the complementary loss function, by default ``False``
+
+	Returns
+	-------
+	dict
+		Dictoinary whose keys range from ``start`` to ``stop`` in intervals of ``step``, 
+		and whose values are the standard normal loss function
+		values corresponding to those keys.
+	"""
+	
+	# Build list of z values.
+	z = start
+	z_list = []
+	while z < stop:
+		z_list.append(z)
+		z += step
+	
+	# Build and return dictionary.
+	return {z: standard_normal_loss(z)[1 if complementary else 0] for z in z_list}
+
+	
 def lognormal_loss(x, mu, sigma):
 	"""
 	Return lognormal loss and complementary loss functions for :math:`\\text{lognormal}(\\mu,\\sigma)`
 	distribution.
 
 	Parameters
 	----------
@@ -296,30 +347,27 @@
 
 	.. doctest::
 
 		>>> lognormal_loss(10, 2, 0.3)
 		(0.28364973888106326, 2.5544912009711833)
 	"""
 	# Calculate E[X].
-	E = np.exp(mu + sigma**2/2)
+	E = math.exp(mu + sigma**2/2)
 
 	if x > 0:
-		n = E * norm.cdf((mu + sigma**2 - np.log(x)) / sigma) \
-			- x * (1 - norm.cdf((np.log(x) - mu) / sigma))
+		n = E * norm.cdf((mu + sigma**2 - math.log(x)) / sigma) \
+			- x * (1 - norm.cdf((math.log(x) - mu) / sigma))
 		n_bar = x - E + n
 	else:
 		n = E - x
 		n_bar = 0
 
 	return n, n_bar
 
 
-# TODO: lognormal second loss
-
-
 def exponential_loss(x, mu):
 	"""
 	Return exponential loss and complementary loss functions for :math:`\\text{exp}(\\mu)`
 	distribution.
 
 	Parameters
 	----------
@@ -371,15 +419,15 @@
 	# Check that x >= 0.
 	if x < 0:
 		raise ValueError("x must be >= 0.")
 
 	# Calculate E[X].
 	E = 1.0 / mu
 
-	n = np.exp(-mu * x) / mu
+	n = math.exp(-mu * x) / mu
 	n_bar = x - E + n
 
 	return n, n_bar
 
 
 def exponential_second_loss(x, mu):
 	"""
@@ -439,15 +487,15 @@
 	if x < 0:
 		raise ValueError("x must be >= 0.")
 
 	# Calculate E[X] and Var[X].
 	E = 1.0 / mu
 	V = 1.0 / mu**2
 
-	n = np.exp(-mu * x) / mu**2
+	n = math.exp(-mu * x) / mu**2
 	n_bar = 0.5 * ((x - E)**2 + V) - n
 
 	return n, n_bar
 
 
 def gamma_loss(x, a, b):
 	"""
@@ -627,15 +675,14 @@
 	n_bar : float
 		Complementary loss function. [:math:`\\bar{n}(x)`]
 
 	Raises
 	------
 	ValueError
 		If ``x`` < ``a`` or > ``b``.
-		# TODO: actually this is OK, just figure out what function equals in this case
 
 
 	**Equations Used:**
 
 	.. math::
 
 		n(x) = \\frac{(b-x)^2}{2(b-a)}
@@ -686,15 +733,14 @@
 	n2_bar : float
 		Complementary second-order loss function. [:math:`\\bar{n}^{(n)}(x)`]
 
 	Raises
 	------
 	ValueError
 		If ``x`` < ``a`` or > ``b``.
-		# TODO: actually this is OK, just figure out what function equals in this case
 
 
 	**Equations Used:**
 
 	.. math::
 
 		n^{(2)}(x) = \\frac{(b-x)^3}{6(b-a)}
@@ -725,16 +771,14 @@
 
 
 def continuous_loss(x, distrib):
 	"""
 	Return loss and complementary loss functions for an arbitrary continuous
 	distribution, using numerical integration.
 
-	TODO: handle distribution supplied as pdf function
-
 	Parameters
 	----------
 	x : float
 		Argument of loss function.
 	distrib : rv_continuous
 		Desired distribution.
 
@@ -809,16 +853,14 @@
 
 
 def continuous_second_loss(x, distrib):
 	"""
 	Return second-order loss and complementary loss functions for an arbitrary continuous
 	distribution, using numerical integration.
 
-	TODO: handle distribution supplied as pdf function
-
 	Parameters
 	----------
 	x : float
 		Argument of loss function.
 	distrib : rv_continuous
 		Desired distribution.
 
@@ -880,16 +922,14 @@
 	# (These will be the ranges for integration.)
 	lb = distrib.ppf(1.0e-10)
 	ub = distrib.ppf(1.0 - 1.0e-10)
 
 	# Find E[X] and Var[X].
 #	E, V = distrib.stats(moments='mv')
 
-	# TODO: allow different methods of computation
-
 	# Calculate loss functions.
 	n2 = 0.5 * distrib.expect(lambda y: max(y - x, 0)**2, lb=x, ub=ub)
 	n2_bar = 0.5 * distrib.expect(lambda y: max(x - y, 0)**2, lb=lb, ub=x)
 	#n2_bar = 0.5 * ((x - E)**2 + V) - n2
 
 	# Original version; the new version seems to be more accurate (and maybe
 	# faster).
@@ -928,19 +968,19 @@
 		If ``x`` is not an integer.
 
 
 	**Equations Used** (equations (C.41) and (C.42)):
 
 	.. math::
 
-		n(x) = -(x - \\mu)(1-F(x)) + \\mu * f(x)
+		n(x) = -(x - \\mu)(1-F(x)) + \\mu f(x)
 
 	.. math::
 
-		\\bar{n}(x) = (x - \\mu) * F(x) + \\mu * f(x)
+		\\bar{n}(x) = (x - \\mu) F(x) + \\mu f(x)
 
 
 	**Example**:
 
 	.. testsetup:: *
 
 		from stockpyl.loss_functions import *
@@ -1260,17 +1300,17 @@
 	.. testsetup:: *
 
 		from stockpyl.loss_functions import *
 
 	.. doctest::
 
 		>>> negative_binomial_loss(14, 4, 0.2)
-		(4.447304632028365, 2.4473046320283647)
+		(4.447304632028364, 2.447304632028364)
 		>>> negative_binomial_loss(14, mean=23, sd=8)
-		(9.326459980156917, 0.32645998015691724)
+		(9.326459980156931, 0.32645998015693145)
 	"""
 
 	# Check for integer x.
 	if not is_integer(x):
 		raise ValueError("x must be an integer")
 
 	# Check that correct parameters have been provided.
@@ -1279,32 +1319,28 @@
 
 	# Calculate mean and sd from r and p, or vice-versa.
 	if r is None or p is None:
 		r = 1.0 * mean ** 2 / (sd ** 2 - mean)
 		p = 1 - (sd ** 2 - mean) / (sd ** 2)
 	else:
 		mean = (1 - p) * r / p
-		sd = np.sqrt((1 - p) * r) / p
+		sd = math.sqrt((1 - p) * r) / p
 
 	# Check that mean < sigma^2.
 	if not mean < sd ** 2:
 		raise ValueError("mean must be less than variance")
 
 	beta = (1 - p) / p
 
 	# Calculate f(x) and F(x).
 	f = nbinom.pmf(x, r, p)
 	F = nbinom.cdf(x, r, p)
 
 	n = -(x - r * beta) * (1 - F) + (x + r) * beta * f
 	n_bar = x - mean + n
-	# formula above does not seem to be working (e.g., if r = 6, p = 0.4, then
-	# returns negative value for n(10). So for now, using generic function:
-#	n, n_bar = discrete_loss(x, nbinom(r, p))
-	# TODO: what's going on above?
 
 	return n, n_bar
 
 
 def negative_binomial_second_loss(x, r=None, p=None, mean=None, sd=None):
 	"""
 	Return :math:`n^{(2)}(x)` and :math:`\\bar{n}^{(2)}(x)``, the second-order
@@ -1389,15 +1425,15 @@
 		from stockpyl.loss_functions import *
 
 	.. doctest::
 
 		>>> negative_binomial_second_loss(14, 4, 0.2)
 		(30.877804945158942, 10.122195054841043)
 		>>> negative_binomial_second_loss(14, mean=23, sd=8)
-		(67.10108087745225, 0.8989191225477526)
+		(67.10108087745232, 0.8989191225476816)
 
 	"""
 	# Check for integer x.
 	if not is_integer(x):
 		raise ValueError("x must be an integer")
 
 	# Check that correct parameters have been provided.
@@ -1406,15 +1442,15 @@
 
 	# Calculate mean and sd from r and p, or vice-versa.
 	if r is None or p is None:
 		r = 1.0 * mean ** 2 / (sd ** 2 - mean)
 		p = 1 - (sd ** 2 - mean) / (sd ** 2)
 	else:
 		mean = (1 - p) * r / p
-		sd = np.sqrt((1 - p) * r) / p
+		sd = math.sqrt((1 - p) * r) / p
 
 	# Check that mean < sigma^2.
 	if not mean < sd ** 2:
 		raise ValueError("mean must be less than variance")
 
 	beta = (1 - p) / p
 
@@ -1507,15 +1543,15 @@
 
 	# Check that either distribution or pmf have been supplied.
 	if (distrib is None) and (pmf is None):
 		raise ValueError("must provide distrib or pmf")
 
 	if distrib is not None:
 		# rv_discrete object has been provided.
-		n_bar = np.sum([distrib.cdf(range(int(x)))])
+		n_bar = float(np.sum([distrib.cdf(range(int(x)))]))
 		n = n_bar - x + distrib.mean()
 
 		# Old (slower) method:
 		# n = 0.0
 		# y = x
 		# comp_cdf = 1 - distrib.cdf(y)
 		# while comp_cdf > 1.0e-12:
@@ -1526,17 +1562,16 @@
 		# n_bar = 0.0
 		# for y in range(0, int(x)):
 		# 	n_bar += distrib.cdf(y)
 	else:
 		# pmf dict has been provided.
 		x_values = list(pmf.keys())
 		x_values.sort()
-		# TODO: vectorize this?
-		n = np.sum([(y - x) * pmf[y] for y in x_values if y >= x])
-		n_bar = np.sum([(x - y) * pmf[y] for y in x_values if y <= x])
+		n = float(np.sum([(y - x) * pmf[y] for y in x_values if y >= x]))
+		n_bar = float(np.sum([(x - y) * pmf[y] for y in x_values if y <= x]))
 
 	return n, n_bar
 
 
 def discrete_second_loss(x, distrib=None, pmf=None):
 	"""
 	Return second-order loss and complementary loss function for an arbitrary discrete
@@ -1624,23 +1659,21 @@
 	if distrib is not None:
 		# rv_discrete object has been provided.
 
 		# Calculate E[X] and Var[x].
 		E, V = distrib.stats(moments='mv')
 
 		# Calculate loss functions.
-		n2_bar = np.dot([np.subtract(x, range(int(x)))], distrib.cdf(range(int(x))))
+		n2_bar = float(np.dot([np.subtract(x, range(int(x)))], distrib.cdf(range(int(x)))))
 		n2 = 0.5 * ((x - E)**2 + (x - E) + V) - n2_bar
 
 	else:
 		# pmf dict has been provided.
 		x_values = list(pmf.keys())
 		x_values.sort()
-		# TODO: vectorize this?
-		n2 = 0.5 * np.sum([(y - x) * (y - x - 1) * pmf[y] for y in x_values if y >= x])
-		n2_bar = 0.5 * np.sum([(x - y) * (x + 1 - y) * pmf[y] for y in x_values if y <= x])
+		n2 = 0.5 * float(np.sum([(y - x) * (y - x - 1) * pmf[y] for y in x_values if y >= x]))
+		n2_bar = 0.5 * float(np.sum([(x - y) * (x + 1 - y) * pmf[y] for y in x_values if y <= x]))
 
-	# .item() removes singleton from ndarray.
-	return n2.item(), n2_bar.item()
+	return n2, n2_bar
```

### Comparing `stockpyl-0.1.0a0/stockpyl/newsvendor.py` & `stockpyl-1.0.0/src/stockpyl/newsvendor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 # ===============================================================================
 # stockpyl - newsvendor Module
 # -------------------------------------------------------------------------------
-# Version: 0.0.0
-# Updated: 01-30-2022
 # Author: Larry Snyder
 # License: GPLv3
 # ===============================================================================
 
-"""The :mod:`newsvendor` module contains code for solving the newsvendor
+"""
+.. include:: ../../globals.inc
+
+
+Overview 
+--------
+
+
+The |mod_newsvendor| module contains code for solving the newsvendor
 problem and some of its variants.
 
-The notation and references (equations, sections, examples, etc.) used below
-refer to Snyder and Shen, *Fundamentals of Supply Chain Theory*, 2nd edition
-(2019).
+.. note:: |fosct_notation|
+
+.. seealso::
+
+	For an overview of single-echelon inventory optimization in |sp|,
+	see the :ref:`tutorial page for single-echelon inventory optimization<tutorial_seio_page>`.
 
+
+API Reference
+-------------
 """
 
 
-from multiprocessing.sharedctypes import Value
 from scipy import stats
 from scipy.optimize import brentq
 import numpy as np
 
 import stockpyl.loss_functions as lf
 from stockpyl.helpers import *
 
@@ -100,15 +111,15 @@
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if demand_mean <= 0: raise ValueError("mean must be positive")
 	if demand_sd <= 0: raise ValueError("demand_sd must be positive")
 
 	# Calculate lead-time demand parameters.
 	ltd_mean = demand_mean * (lead_time + 1)
-	ltd_sd = demand_sd * np.sqrt(lead_time + 1)
+	ltd_sd = demand_sd * math.sqrt(lead_time + 1)
 
 	# Is S provided?
 	if base_stock_level is None:
 		# Calculate alpha.
 		alpha = stockout_cost / (stockout_cost + holding_cost)
 
 		# Calculate optimal order quantity and cost.
@@ -175,25 +186,23 @@
 	.. doctest::
 
 		>>> newsvendor_normal_cost(60, 0.18, 0.70, 50, 8)
 		2.156131552870387
 
 	"""
 
-	# TODO: delete this function since newsvendor_normal subsumes it?
-
 	# Check that parameters are positive.
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if demand_mean <= 0: raise ValueError("mean must be positive")
 	if demand_sd <= 0: raise ValueError("demand_sd must be positive")
 
 	# Calculate lead-time demand parameters.
 	ltd_mean = demand_mean * (lead_time + 1)
-	ltd_sd = demand_sd * np.sqrt(lead_time + 1)
+	ltd_sd = demand_sd * math.sqrt(lead_time + 1)
 
 	# Calculate loss functions.
 	n, n_bar = lf.normal_loss(base_stock_level, ltd_mean, ltd_sd)
 
 	# Calculate cost.
 	cost = holding_cost * n_bar + stockout_cost * n
 
@@ -268,16 +277,14 @@
 	# Check that parameters are positive.
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if demand_mean <= 0: raise ValueError("mean must be positive")
 	if base_stock_level is not None and not is_integer(base_stock_level):
 		raise ValueError("base_stock_level must be an integer (or None)")
 
-	# TODO: handle lead time
-
 	# Is S provided?
 	if base_stock_level is None:
 		# Calculate alpha.
 		alpha = stockout_cost / (stockout_cost + holding_cost)
 
 		# Calculate optimal order quantity and cost.
 		base_stock_level = stats.poisson.ppf(alpha, demand_mean)
@@ -343,24 +350,20 @@
 	.. doctest::
 
 		>>> newsvendor_poisson_cost(56, 0.18, 0.70, 50)
 		1.797235211809178
 
 	"""
 
-	# TODO: delete this function since newsvendor_poisson() subsumes it?
-
 	# Check that parameters are positive.
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if demand_mean <= 0: raise ValueError("mean must be positive")
 	if not is_integer(base_stock_level): raise ValueError("base_stock_level must be an integer")
 
-	# TODO: handle lead time
-
 	# Calculate loss functions.
 	n, n_bar = lf.poisson_loss(base_stock_level, demand_mean)
 
 	# Calculate cost.
 	cost = holding_cost * n_bar + stockout_cost * n
 
 	return cost
@@ -445,17 +448,14 @@
 	# Check that parameters are positive.
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 
 	# Check that either distribution or pmf have been supplied.
 	if demand_distrib is None and demand_pdf is None: raise ValueError("must provide demand_distrib or demand_pdf")
 
-	# TODO: handle lead time
-	# TODO: handle demand_pdf as function
-
 	# For now, raise error if only demand_pdf is provided. TODO: (Need to add this
 	# capability.)
 	assert demand_distrib is not None, "newsvendor_continuous() does not yet support demand distributions passed as pdf functions"
 
 	# Is S provided?
 	if base_stock_level is None:
 		# Calculate alpha.
@@ -533,20 +533,20 @@
 
 	.. testsetup:: *
 
 		from stockpyl.newsvendor import *
 
 	.. doctest::
 
-		>>> from scipy.stats import poisson
-		>>> demand_distrib = poisson(6)
-		>>> newsvendor_discrete(1, 4, demand_distrib)
-		(8.0, 3.5701069457709416)
-		>>> newsvendor_discrete(1, 4, demand_distrib, base_stock_level=5)
-		(5, 6.590296024616343)
+			>>> from scipy.stats import poisson
+			>>> demand_distrib = poisson(6)
+			>>> newsvendor_discrete(1, 4, demand_distrib)
+			(8.0, 3.5701069457709416)
+			>>> newsvendor_discrete(1, 4, demand_distrib, base_stock_level=5)
+			(5, 6.590296024616343)
 
 	.. doctest::
 
 		>>> from scipy.stats import poisson
 		>>> d = range(0, 41)
 		>>> f = [poisson.pmf(d_val, 6) for d_val in d]
 		>>> demand_pmf = dict(zip(d, f))
@@ -558,30 +558,28 @@
 	# Check that parameters are positive.
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost < 0: raise ValueError("stockout_cost must be non-negative")
 
 	# Check that either distribution or pmf have been supplied.
 	if demand_distrib is None and demand_pmf is None: raise ValueError("must provide demand_distrib or demand_pmf")
 
-	# TODO: handle lead time
-
 	# Is S provided?
 	if base_stock_level is None:
 		# Calculate alpha.
 		alpha = stockout_cost / (stockout_cost + holding_cost)
 
 		# Was distribution provided?
 		if demand_distrib is not None:
 			# Use built-in ppf (F-inverse) function.
 			base_stock_level = demand_distrib.ppf(alpha)
 		else:
 			# Build sorted list of demand values.
 			demand_values = list(demand_pmf.keys())
 			demand_values.sort()
-			# Loop through demand_list until cdf exceeds alpha.
+			# Loop through demands until cdf exceeds alpha.
 			i = 0
 			F = 0
 			while F < alpha:
 				F += demand_pmf[demand_values[i]]
 				i += 1
 				if i >= len(demand_pmf):
 					break
@@ -609,16 +607,16 @@
 		demand_sd,
 		discount_factor=1.0,
 		base_stock_level=None):
 	"""Find the optimizer of the myopic cost function, or (if ``base_stock_level``
 	is supplied) calculate the cost of given solution. Assumes demand is normally distributed.
 
 	The myopic cost function is denoted :math:`G_i(y)` in Veinott (1966) and
-	as :math:`C^+(t,y)` in Zipkin (2000). It is not used in Snyder and Shen
-	(2019), but the function is given in terms of Snyder-Shen notation below.
+	as :math:`C^+(t,y)` in Zipkin (2000). It is not used in |fosct|, 
+	but the function is given in terms of Snyder-Shen notation below.
 
 	Parameters are singleton values for the current period, not arrays.
 
 	Parameters
 	----------
 	holding_cost : float
 		Holding cost in the current period. [:math:`h`]
@@ -684,16 +682,14 @@
 		>>> myopic(0.18, 0.70, 0.3, 0.35, 50, 8, 0.98)
 		(58.09891883213067, 16.682411764618777)
 		>>> myopic(0.18, 0.70, 0.3, 0.35, 50, 8, 0.98, base_stock_level=62)
 		(62, 16.850319828088736)
 
 	"""
 
-# TODO: handle non-normal demand
-
 	# Calculate c_plus.
 	c_plus = purchase_cost - discount_factor * purchase_cost_next_per
 
 	# Validate c_plus.
 	if c_plus < -holding_cost or c_plus > stockout_cost:
 		raise ValueError("myopic() requires -h_t <= c_t - gamma * c_{t+1} <= p_t")
 
@@ -721,16 +717,16 @@
 		purchase_cost_next_per,
 		demand_mean,
 		demand_sd,
 		discount_factor=1.0):
 	"""Calculate "myopic" cost function. Assumes demand is normally distributed.
 
 	The myopic cost function is denoted :math:`G_i(y)` in Veinott (1966) and
-	as :math:`C^+(t,y)` in Zipkin (2000). It is not used in Snyder and Shen
-	(2019), but the function is given in terms of Snyder-Shen notation below.
+	as :math:`C^+(t,y)` in Zipkin (2000). It is not used in |fosct|, 
+	but the function is given in terms of Snyder-Shen notation below.
 
 	Parameters are singleton values for the current period, not arrays.
 
 	Parameters
 	----------
 	base_stock_level : float
 		Base-stock level to calculate cost for. [:math:`S`]
@@ -782,16 +778,14 @@
 	.. doctest::
 
 		>>> myopic_cost(60, 0.18, 0.70, 0.3, 0.35, 50, 8, 0.98)
 		16.726131552870388
 
 	"""
 
-# TODO: handle non-normal demand
-
 	# Calculate newsvendor cost.
 	g = newsvendor_normal_cost(base_stock_level, holding_cost, stockout_cost,
 			demand_mean, demand_sd)
 
 	return purchase_cost * base_stock_level + g \
 		- discount_factor * purchase_cost_next_per * (base_stock_level - demand_mean)
 
@@ -865,16 +859,14 @@
 		>>> set_myopic_cost_to(18, 0.18, 0.70, 0.3, 0.35, 50, 8, 0.98, left_half=False)
 		71.84861989932769
 		>>> myopic_cost(71.84861989932769, 0.18, 0.70, 0.3, 0.35, 50, 8, 0.98)
 		18.0
 
 	"""
 
-	# TODO: handle non-normal demand
-
 	# Calculate c_plus.
 	c_plus = purchase_cost - discount_factor * purchase_cost_next_per
 
 	# Validate c_plus.
 	if c_plus < -holding_cost or c_plus > stockout_cost:
 		raise ValueError("set_myopic_cost_to() requires -h_t <= c_t - gamma * c_{t+1} <= p_t")
 
@@ -917,44 +909,42 @@
 
 	# Use Brent method to find zero of G_t(y) - cost.
 	base_stock_level = brentq(fun, a, b)
 
 	return base_stock_level
 
 
-def newsvendor_normal_explicit(selling_revenue, purchase_cost, salvage_value,
-							   holding_cost, stockout_cost, demand_mean, demand_sd,
+def newsvendor_normal_explicit(revenue, purchase_cost, salvage_value,
+							   demand_mean, demand_sd, holding_cost=0, stockout_cost=0, 
 					  		   lead_time=0, base_stock_level=None):
 	"""Solve the "explicit", profit-maximization version of the newsvendor
 	problem with normal distribution, or (if ``base_stock_level`` is supplied)
 	calculate profit of given solution.
 
-	Assumes ``salvage_value`` < ``purchase_cost`` < ``selling_revenue``
+	Assumes ``salvage_value`` < ``purchase_cost`` < ``revenue``
 	(otherwise the solution is not well-defined).
 
-	# TODO: handle non-normal demand
-
 	Parameters
 	----------
-	selling_revenue : float
+	revenue : float
 		Revenue per unit sold. [:math:`r`]
 	purchase_cost : float
 		Cost per unit purchased. [:math:`c`]
 	salvage_value : float
 		Revenue per unit unsold. [:math:`v`]
-	holding_cost : float
-		Holding cost per item per period, excluding costs and revenues from
-		buying, selling, or salvaging items. [:math:`h`]
-	stockout_cost : float
-		Stockout cost per item per period, excluding costs and revenues from
-		buying, selling, or salvaging items. [:math:`p`]
 	demand_mean : float
 		Mean demand per period. [:math:`\\mu`]
 	demand_sd : float
 		Standard deviation of demand per period. [:math:`\\sigma`]
+	holding_cost : float, optional
+		Holding cost per item per period, over and above any costs and revenues from
+		buying, selling, or salvaging items. [:math:`h`]
+	stockout_cost : float, optional
+		Stockout cost per item per period, over and above any costs and revenues from
+		buying, selling, or salvaging items. [:math:`p`]
 	lead_time : int, optional
 		Lead time. Default = 0. [:math:`L`]
 	base_stock_level : float, optional
 		Base-stock level for profit evaluation. If supplied, no
 		optimization will be performed. [:math:`S`]
 
 	Returns
@@ -992,47 +982,148 @@
 
 	.. testsetup:: *
 
 		from stockpyl.newsvendor import *
 
 	.. doctest::
 
-		>>> newsvendor_normal_explicit(1, 0.3, 0.12, 0, 0, 50, 8)
+		>>> newsvendor_normal_explicit(1, 0.3, 0.12, 50, 8)
 		(56.60395592743389, 33.002394806823354)
 
 	"""
 
 	# Check that parameters are positive/non-negative.
 	if holding_cost < 0: raise ValueError("holding_cost must be non-negative")
 	if stockout_cost < 0: raise ValueError("stockout_cost must be non-negative")
 	if demand_mean <= 0: raise ValueError("mean must be positive")
 	if demand_sd <= 0: raise ValueError("demand_sd must be positive")
-	if selling_revenue <= purchase_cost: raise ValueError("selling_revenue must be > purchase_cost")
+	if revenue <= purchase_cost: raise ValueError("revenue must be > purchase_cost")
 	if purchase_cost <= salvage_value: raise ValueError("purchase_cost must be > salvage_value")
 
 	# Calculate lead-time demand parameters.
 	ltd_mean = demand_mean * (lead_time + 1)
-	ltd_sd = demand_sd * np.sqrt(lead_time + 1)
+	ltd_sd = demand_sd * math.sqrt(lead_time + 1)
 
 	# Is S provided?
 	if base_stock_level is None:
 		# Calculate alpha.
-		alpha = (stockout_cost + selling_revenue - purchase_cost) \
-				/ (stockout_cost + holding_cost + selling_revenue - salvage_value)
+		alpha = (stockout_cost + revenue - purchase_cost) \
+				/ (stockout_cost + holding_cost + revenue - salvage_value)
 
 		# Calculate optimal order quantity and cost.
 		base_stock_level = stats.norm.ppf(alpha, ltd_mean, ltd_sd)
-		profit = (selling_revenue - purchase_cost) * ltd_mean \
-			- (selling_revenue - salvage_value + holding_cost + stockout_cost) \
+		profit = (revenue - purchase_cost) * ltd_mean \
+			- (revenue - salvage_value + holding_cost + stockout_cost) \
 			   * stats.norm.pdf(stats.norm.ppf(alpha, 0, 1)) * ltd_sd
 	else:
 		# Calculate loss functions.
 		_, n_bar = lf.normal_loss(base_stock_level, ltd_mean, ltd_sd)
 
 		# Calculate profit.
-		profit = (selling_revenue - purchase_cost + stockout_cost) * base_stock_level \
+		profit = (revenue - purchase_cost + stockout_cost) * base_stock_level \
 			- stockout_cost * ltd_mean \
-			+ (salvage_value - selling_revenue - holding_cost - stockout_cost) * n_bar
+			+ (salvage_value - revenue - holding_cost - stockout_cost) * n_bar
+
+	return base_stock_level, profit
+
+
+def newsvendor_poisson_explicit(revenue, purchase_cost, salvage_value,
+							   demand_mean, holding_cost=0, stockout_cost=0, 
+					  		   lead_time=0, base_stock_level=None):
+	"""Solve the "explicit", profit-maximization version of the newsvendor
+	problem with Poisson distribution, or (if ``base_stock_level`` is supplied)
+	calculate profit of given solution.
+
+	Assumes ``salvage_value`` < ``purchase_cost`` < ``revenue``
+	(otherwise the solution is not well-defined).
+
+	Parameters
+	----------
+	revenue : float
+		Revenue per unit sold. [:math:`r`]
+	purchase_cost : float
+		Cost per unit purchased. [:math:`c`]
+	salvage_value : float
+		Revenue per unit unsold. [:math:`v`]
+	demand_mean : float
+		Mean demand per period. [:math:`\\mu`]
+	holding_cost : float, optional
+		Holding cost per item per period, over and above any costs and revenues from
+		buying, selling, or salvaging items. [:math:`h`]
+	stockout_cost : float, optional
+		Stockout cost per item per period, over and above any costs and revenues from
+		buying, selling, or salvaging items. [:math:`p`]
+	lead_time : int, optional
+		Lead time. Default = 0. [:math:`L`]
+	base_stock_level : float, optional
+		Base-stock level for profit evaluation. If supplied, no
+		optimization will be performed. [:math:`S`]
+
+	Returns
+	-------
+	base_stock_level : float
+		Optimal base-stock level (or base-stock level supplied). [:math:`S^*`]
+	profit : float
+		Profit per period attained by ``base_stock_level``. [:math:`\\pi^*`]
+
+	Raises
+	------
+	ValueError
+		If ``r`` < ``c`` or ``c`` < ``v``.
+	ValueError
+		If ``holding_cost`` < 0 or ``stockout_cost`` < 0.
+
+
+	**Equations Used**:
+
+	.. math::
+
+		S^* = \\text{smallest } S \\text{ such that } F(S) \\ge \\frac{p+r-c}{h+p+r-v}
+
+		\\pi(S) = (r-c+p)S - p\\mu + (v-r-h-p)\\bar{n}(S),
+
+	where :math:`\\mu` is the lead-time demand mean
+	and :math:`\\bar{n}(\\cdot)` is the Poisson complementary loss function.
+
+	**Example** (Example 4.2 but with Poisson demand):
+
+	.. testsetup:: *
+
+		from stockpyl.newsvendor import *
+
+	.. doctest::
+
+		>>> newsvendor_poisson_explicit(1, 0.3, 0.12, 50)
+		(56.0, 33.20276478819082)
+
+	"""
+
+	# Check that parameters are positive/non-negative.
+	if holding_cost < 0: raise ValueError("holding_cost must be non-negative")
+	if stockout_cost < 0: raise ValueError("stockout_cost must be non-negative")
+	if demand_mean <= 0: raise ValueError("mean must be positive")
+	if revenue <= purchase_cost: raise ValueError("revenue must be > purchase_cost")
+	if purchase_cost <= salvage_value: raise ValueError("purchase_cost must be > salvage_value")
+
+	# Calculate lead-time demand parameters.
+	ltd_mean = demand_mean * (lead_time + 1)
+
+	# Is S provided?
+	if base_stock_level is None:
+		# Calculate alpha.
+		alpha = (stockout_cost + revenue - purchase_cost) \
+				/ (stockout_cost + holding_cost + revenue - salvage_value)
+
+		# Calculate optimal order quantity.
+		base_stock_level = stats.poisson.ppf(alpha, ltd_mean)
+
+	# Calculate loss functions.
+	_, n_bar = lf.poisson_loss(base_stock_level, ltd_mean)
+
+	# Calculate profit.
+	profit = (revenue - purchase_cost + stockout_cost) * base_stock_level \
+		- stockout_cost * ltd_mean \
+		+ (salvage_value - revenue - holding_cost - stockout_cost) * n_bar
 
 	return base_stock_level, profit
```

### Comparing `stockpyl-0.1.0a0/stockpyl/instances.py` & `stockpyl-1.0.0/src/stockpyl/instances.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,133 +1,199 @@
 # ===============================================================================
 # stockpyl - instances Module
 # -------------------------------------------------------------------------------
-# Version: 0.0.0
-# Updated: 02-03-2022
 # Author: Larry Snyder
 # License: GPLv3
 # ===============================================================================
 
-"""The :mod:`instances` module contains code for loading and saving problem instances.
-Unless otherwise noted, instances are taken from Snyder and Shen, *Fundamentals of Supply Chain Theory*, 2nd edition
-(2019).
-
-.. csv-table:: Named Instances
-   :file: ../docs/aux_files/temp.csv
-   :widths: 30, 70
-   :header-rows: 1
+"""
+.. include:: ../../globals.inc
+
+Overview 
+--------
+
+The |mod_instances| module contains code for loading and saving problem instances.
+
+.. note:: |fosct_notation| 
+
+	The abbreviation *SCMO* below refers to the textbook
+	*Supply Chain Modeling and Optimization* by Snyder, Smilowitz, and Shen, forthcoming.
+
+|sp| has a number of built-in instances, most (but not all) of which are taken from |fosct|.
+These can be loaded using the :func:`~load_instance` function by providing the instance name. 
+A list of the built-in instances is provided below.
+
+
+.. include:: ../../../src/stockpyl/aux_files/stockpyl_instances_metadata.rst
+
+
+|
+
+API Reference
+-------------
+
 """
 
-#import copy
 import os
 import json
 import warnings
 import datetime
 import jsonpickle
 import csv
+from copy import deepcopy
+import inspect
 
 from stockpyl.supply_chain_network import *
 from stockpyl.supply_chain_node import *
 
-DEFAULT_JSON_FILEPATH = 'datasets/stockpyl_instances.json'
-
-
-def load_instance(instance_name, filepath=DEFAULT_JSON_FILEPATH):
+def load_instance(instance_name, filepath=None, ignore_state_vars=True):
 	"""Load an instance from a JSON file. 
 
-	If the instance was originally specified as a ``SupplyChainNetwork`` object, returns the
+	If the instance was originally specified as a |class_network| object, returns the
 	object; otherwise, returns the instance in a dictionary.
 
 	Parameters
 	----------
 	instance_name : str
 		The name of the instance.
 	filepath : str, optional
-		Path to the JSON file. If ``None``, ``../datasets/stockpyl_instances.json`` is used.
+		Path to the JSON file. If ``None``, the function determines the path to 
+		``datasets/stockpyl_instances.json``.
+	ignore_state_vars : bool, optional
+		If ``True``, function will ignore any saved state variables in the nodes.
 
 	Returns
 	-------
-	dict or SupplyChainNetwork
-		The loaded instance. If the instance was originally specified as a ``SupplyChainNetwork``
+	dict or |class_network|
+		The loaded instance. If the instance was originally specified as a |class_network|
 		object, returns the object; otherwise, returns the instance in a dictionary in which
 		the keys equal the parameter names (e.g., "holding_cost") and the values equal the parameter
 		values (e.g., 0.5).
 
 	Raises
 	------
 	ValueError
 		If the JSON file does not exist or the instance cannot be found in the JSON file.
 	"""
-	# TODO: unit tests
-	
+
+	# Determine filepath.
+	if filepath is None:
+		filepath = _stockpyl_instances_json_path()
+
 	# Does JSON file exist?
 	if os.path.exists(filepath):
-		# Load data from JSON.
-		with open(filepath) as f:
-			json_contents = json.load(f)
+		# Use this path.
+		new_path = filepath
 	else:
-		raise FileNotFoundError("The specified JSON file was not found")
-	
+		# Try changing working directory to project root (stockpyl/). This is mainly a workaround for
+		# when this function is called from doctests.
+		one_level_up = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+		new_path = os.path.join(one_level_up, filepath)
+		if not os.path.exists(new_path):
+			raise FileNotFoundError(f"The JSON file {os.path.abspath(filepath)} was not found")
+
+	# Load data from JSON.
+	with open(new_path) as f:
+		json_contents = json.load(f)
+
 	# Look for instance. (https://stackoverflow.com/a/8653568/3453768)
 	instance_index = next((i for i, item in enumerate(json_contents["instances"]) \
 		if item["name"] == instance_name), None)
 	# Was instance found?
 	if instance_index is None:
 		raise KeyError("The speficied instance name was not found")
 
-	# Get instance (in case it was jsonpickled).
+	# Get instance.
 	instance = json_contents["instances"][instance_index]["data"]
+	instance_type = json_contents["instances"][instance_index]["type"]
 
-	# Try to decode instance using jsonpickle. This will fail if the
-	# instance is a regular dict, in which case we'll just return the dict.
-	try:
-		return jsonpickle.decode(instance)
-	except:
+	# Was instance saved as a dict or a network?
+	if instance_type == "network":
+		# As a network.
+		instance = SupplyChainNetwork.from_dict(instance)
+
+		# Delete the state variables and replace with initialized version, 
+		# if ignore_state_variables = True.
+		if ignore_state_vars:
+			for n in instance.nodes:
+				n.state_vars = []
+
+		# Ensure that all nodes have dummy product fields set correctly. This is to maintain backward
+		# compatitbility with earlier versions, which did not save product info (including dummy products).
+		for n in instance.nodes:
+			# Does node already have dummy product?
+			if n._dummy_product is None:
+				# Add a dummy product, whether or not it needs one (mainly to assign the index).
+				n._add_dummy_product()
+			# Assign external supplier dummy product.
+			n._external_supplier_dummy_product = SupplyChainProduct(n._dummy_product.index - 1, is_dummy=True)
+			# Does node have "real" products? (This will probably never happen, since products were introduced
+			# in the same version as dummy products--so if a node has products, it probably has dummy products
+			# correctly handled already.)
+			if len(n.products_by_index) > 1:
+				# Remove dummy product.
+				n._remove_dummy_product()
+	else:
+		# As a dict. Leave in place. But:
 		# If the instance contains any dicts with integer keys, they will have
 		# been saved as strings when the JSON was saved. Convert them back to integers here.
 		# Currently, only demand_pmf has this issue.
 		if 'demand_pmf' in instance.keys():
 			instance['demand_pmf'] = {int(k): v for k, v in instance['demand_pmf'].items()}
+ 
+	return instance
 
-		return instance
-
-
-def save_instance(instance_name, instance_data, instance_description='', filepath=DEFAULT_JSON_FILEPATH, replace=True, create_if_none=True):
+def save_instance(instance_name, instance_data, instance_description='', filepath=None, 
+	replace=True, create_if_none=True, delete_if_exists=False, omit_state_vars=True):
 	"""Save an instance to a JSON file. 
 	
-	Appends the instance; does not check to see whether the instance is already in the file. 
-	(To update an existing instance, use :func:`update_instance`.)
-
 	Parameters
 	----------
 	instance_name : str
 		The name of the instance. This will be used later for retreving the instance.
 	instance_data : dict or SupplyChainNetwork
 		The instance data as a dictionary (with keys equal to parameter names (e.g., "holding_cost")
-		and values equal to parameter values (e.g., 0.5)) or as a ``SupplyChainNetwork`` object 
+		and values equal to parameter values (e.g., 0.5)) or as a |class_network| object 
 		(in which case the instance is serialized using :mod:`jsonpickle`).
 	instance_description : str, optional
 		A longer descrtiption of the instance.
 	filepath : str, optional
-		Path to the JSON file. If ``None``, ``../datasets/stockpyl_instances.json`` is used.
+		Path to the JSON file. If ``None``, the function determines the path to 
+		``datasets/stockpyl_instances.json``.
 	replace : bool, optional
 		If an instance with the same ``instance_name`` is already in the file, the function
 		will replace it if ``True`` and will ignore it (and write nothing) if ``False``.
 	create_if_none : bool, optional
 		If the file does not already exist, the function will create a new file if ``True``; 
 		otherwise, it will not do anything and issue a warning.
+	delete_if_exists : bool, optional
+		If the file already exists, the function will delete it first if ``True``; 
+		otherwise, it will modify the existing file.
+	omit_state_vars : bool, optional
+		If ``True``, the function will not save state variables as part of the nodes,
+		even if they are present in the instance.
 	"""
 
-	# TODO: unit tests
-	
+	# Determine filepath.
+	if filepath is None:
+		filepath = _stockpyl_instances_json_path()
+
 	# Does JSON file exist?
 	if os.path.exists(filepath):
-		# Load data from JSON.
-		with open(filepath) as f:
-			json_contents = json.load(f)
+		if delete_if_exists:
+			os.remove(filepath)
+			json_contents = {
+				"_id": "",
+				"instances": [],
+				"last_updated": ""
+			}
+		else:
+			# Load data from JSON.
+			with open(filepath) as f:
+				json_contents = json.load(f)
 	else:
 		# Should we create it?
 		if create_if_none:
 			json_contents = {
 				"_id": "",
 				"instances": [],
 				"last_updated": ""
@@ -140,70 +206,71 @@
 	instance_index = next((i for i, item in enumerate(json_contents["instances"]) \
 		if item["name"] == instance_name), None)
 	# Was instance found?
 	if instance_index is not None:
 		if not replace:
 			return
 
+	# Make local copy of network.
+	local_copy = deepcopy(instance_data)
+
 	# Was data provided as dict or SupplyChainNetwork?
-	if isinstance(instance_data, dict):
-		data = instance_data
+	if isinstance(local_copy, dict):
+		data = local_copy
+		instance_type = "dict"
 	else:
 		# Assume SupplyChainNetwork.
-		data = jsonpickle.encode(instance_data)
+		# Omit state variables, if requested.
+		if omit_state_vars:
+			for n in local_copy.nodes:
+				n.state_vars = None
+		# Convert to dict and JSONify.
+		data = local_copy.to_dict()
+		instance_type = "network"
 
 	# Create dictionary with instance metadata and data.
 	instance_dict = {
 		"name": instance_name,
 		"description": instance_description,
-		"data": data
+		"data": data,
+		"type": instance_type
 	}
 
 	# Add (or replace) instance.
-	if instance_index:
+	if instance_index is not None:
 		# We already know replace is True, otherwise we would have exited already.
 		json_contents["instances"][instance_index] = instance_dict
 	else:
 		json_contents["instances"].append(instance_dict)
 	json_contents["last_updated"] = f"{datetime.datetime.now()}"
 
 	# If the instance contains any dicts with integer keys, they will be
 	# saved as strings when the JSON is saved. load_instance() converts them back to integers.
 	# Currently, only demand_pmf has this issue.
 
+	# Make sure path exists; if not, create it.
+	os.makedirs(os.path.dirname(filepath), exist_ok=True)
+	
 	# Write all instances to JSON.
 	with open(filepath, 'w') as f:
 		json.dump(json_contents, f)
 
 	# Close file.
 	f.close()
 
 
-def save_summary_to_csv(save_filepath, json_filepath=DEFAULT_JSON_FILEPATH):
-	"""Save a CSV file with a summary of the instances in a JSON file.
-
-	Main purpose of this method is to build the CSV file that populates the table
-	at the top of this page.
 
-	Parameters
-	----------
-	save_filepath : str
-		Path to the CSV file to create.
-	json_filepath : str, optional
-		Path to the JSON file. If ``None``, ``../datasets/stockpyl_instances.json`` is used.
-	"""
+def _stockpyl_instances_json_path():
+	"""Determine the path to the JSON file containing the instances. 
 
-	# Load JSON file.
-	with open(json_filepath) as f:
-		json_contents = json.load(f)
+	See discussion at https://github.com/LarrySnyder/stockpyl/issues/85.
 
-	# Write to CSV.
-	with open(save_filepath, 'w', newline='') as csvfile:
-		instance_writer = csv.writer(csvfile, delimiter=',', quotechar='"', quoting=csv.QUOTE_MINIMAL)
-
-		instance_writer.writerow(['Name', 'Description'])
-		for instance in json_contents['instances']:
-			instance_writer.writerow([instance['name'], instance['description']])
-
-	f.close()
-	csvfile.close()
+	Returns
+	-------
+	str
+		The absolute path, including the filename itself.
+	"""
+	code_file = os.path.abspath(inspect.getsourcefile(_stockpyl_instances_json_path))
+	rtn = os.path.join(os.path.dirname(code_file), "datasets", "stockpyl_instances.json")
+	assert os.path.exists(rtn) and os.path.isfile(rtn)
+	return rtn
```

### Comparing `stockpyl-0.1.0a0/stockpyl/finite_horizon.py` & `stockpyl-1.0.0/src/stockpyl/finite_horizon.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 # ===============================================================================
 # stockpyl - finite_horizon Module
 # -------------------------------------------------------------------------------
-# Version: 0.0.0
-# Updated: 01-30-2020
 # Author: Larry Snyder
 # License: GPLv3
 # ===============================================================================
 
-"""The :mod:`finite_horizon` module contains code for solving finite-horizon
-inventory optimization problems using dynamic programming.
+"""
+.. include:: ../../globals.inc
+
+Overview 
+--------
+
+The |mod_finite_horizon| module contains code for solving finite-horizon, stochastic
+inventory optimization problems, with or without fixed costs, using dynamic programming (DP).
+
+.. note:: |fosct_notation|
+
+.. seealso::
 
-The notation and references (equations, sections, examples, etc.) used below
-refer to Snyder and Shen, *Fundamentals of Supply Chain Theory*, 2nd edition
-(2019).
+	For an overview of single-echelon inventory optimization in |sp|,
+	see the :ref:`tutorial page for single-echelon inventory optimization<tutorial_seio_page>`.
 
+
+API Reference
+-------------
 """
 
 import numpy as np
 from scipy.stats import norm
-#from scipy.optimize import brentq
 import warnings
-from tabulate import tabulate
 
 from stockpyl.helpers import *
 from stockpyl.newsvendor import *
 from stockpyl.eoq import *
 import stockpyl.loss_functions as lf
 from stockpyl.instances import *
 
@@ -33,27 +41,30 @@
 		num_periods,
 		holding_cost,
 		stockout_cost,
 		terminal_holding_cost,
 		terminal_stockout_cost,
 		purchase_cost,
 		fixed_cost,
-		demand_mean,
-		demand_sd,
+		demand_mean=None,
+		demand_sd=None,
+		demand_source=None,
 		discount_factor=1.0,
 		initial_inventory_level=0.0,
 		trunc_tol=0.02,
 		d_spread=4,
-		s_spread=5):
+		s_spread=5,
+		oul_matrix=None,
+		x_range=None):
 	"""
 	Solve the finite-horizon inventory optimization problem, with or without
 	fixed costs, minimizing the expected discounted cost over the time horizon,
 	using dynamic programming (DP).
 
-	See Sections 4.3.3 and 4.4.3 of Snyder and Shen (2019) for discussion and
+	See Sections 4.3.3 and 4.4.3 of |fosct| for discussion and
 	notation.
 
 	Returns :math:`s^*_t` and :math:`S^*_t` in the output lists ``reorder_points``
 	and ``order_up_to_levels``, respectively. If ``fixed_cost`` = 0,
 	then ``reorder_points[t]`` = ``order_up_to_levels[t]`` for all ``t``.
 
 	Also returns the optimal cost and action matrices. The optimal total
@@ -69,15 +80,18 @@
 
 		\\theta_{T+1}(x) = h_T x^+ + p_T x^-,
 
 	where :math:`h_T` = ``terminal_holding_cost``, :math:`p_T` =
 	``terminal_stockout_cost``, :math:`x^+ = \\max\\{x,0\\}`, and
 	:math:`x^- = \\max\\{-x,0\\}`.
 
-	Demands are assumed to be normally distributed.
+	Either ``demand_mean`` and ``demand_sd`` must be
+	provided (in which case the demand will be assumed to be normally distributed),
+	or ``demand_source`` must be provided (in which case the demand will follow the
+	distribution specified in ``demand_source``).
 
 	Most parameters may be given as a singleton or a list. If given as a
 	singleton, the parameter will be assumed to be the same in every time
 	period. If given as a list, the list must be of length ``num_periods`` or
 	``num_periods``\+1.
 
 	*	In the former case, the list is assumed to contain values for periods
@@ -87,27 +101,31 @@
 		0th element is ignored.
 
 	The parameters may be mixed, some scalars and some lists.
 
 	Output arrays are all 1-indexed; for example, ``reorder_point[5]`` gives
 	:math:`s^*_5`, the reorder point for period 5.
 
-	Discretization is done at the integer level, i.e., all demand_list and
+	Discretization is done at the integer level, i.e., all demands and
 	inventory positions are rounded to the nearest integer. The state space
 	(range of possible inventory positions) is truncated using settings
 	specified in the code.
 
 	Raises warnings if the discretization and truncation settings are likely to
 	lead to suboptimal results. (See details in the code.)
-
-	Executes faster than straightforward implementation because it calculates
-	:math:`H_t(y)` (as defined in (4.87)) for each :math:`t` and :math:`y`,
-	and then uses this when calculating :math:`\\theta_t(x)` for each :math:`x`.
-	This avoids having to recalculate the terms that don't depend on :math:`x`
-	(which are computationally expensive).
+		
+	If ``oul_matrix`` is provided as an input, the function uses it (with discretization 
+	specified by ``x_range`` input) instead of optimizing over the order-up-to levels.
+	If ``oul_matrix`` is provided, then ``x_range`` must be provided as well.
+
+	.. note:: This function executes faster than straightforward implementation because it calculates
+		:math:`H_t(y)` (as defined in (4.87)) for each :math:`t` and :math:`y`,
+		and then uses this when calculating :math:`\\theta_t(x)` for each :math:`x`.
+		This avoids having to recalculate the terms that don't depend on :math:`x`
+		(which are computationally expensive).
 
 	Parameters
 	----------
 	num_periods : int
 		Number of periods in time horizon. [:math:`T`]
 	holding_cost : float or list
 		Holding cost per item per period. [:math:`h`]
@@ -117,31 +135,41 @@
 		Terminal holding cost per item. [:math:`h_T`]
 	terminal_stockout_cost : float
 		Terminal stockout cost per item. [:math:`p_T`]
 	purchase_cost : float or list
 		Purchase cost per item. [:math:`c`]
 	fixed_cost : float or list
 		Fixed cost per order. [:math:`K`]
-	demand_mean : float or list
-		Demand mean per period. [:math:`\\mu`]
-	demand_sd : float or list
-		Demand standard deviation per period. [:math:`\\sigma`]
+	demand_mean : float or list, optional
+		Demand mean per period. Ignored if ``demand_source`` is not ``None``. [:math:`\\mu`]
+	demand_sd : float or list, optional
+		Demand standard deviation per period. Ignored if ``demand_source`` is not ``None``. [:math:`\\sigma`]
+	demand_source : |class_demand_source|, optional
+		A |class_demand_source| object describing the demand distribution. Required if
+		``demand_mean`` and ``demand_standard_deviation`` are ``None``.
 	discount_factor : float or list
 		Discount factor, in :math:`(0,1]`. Default = 1. [:math:`\\gamma`]
 	initial_inventory_level : float
 		Initial inventory level at the start of period 1. [:math:`x_1`]
 	trunc_tol : float
 		Truncation tolerance; a warning is raised if *either* total probability of 
 		demand outside of ``d_range`` > ``trunc_tol`` for any time period, *or*
 		:math:`P(s_t - D < x_{min})` > ``trunc_tol``, where :math:`x_{min}` is the 
 		minimum value of :math:`x` after truncation.
 	d_spread : float
 		Number of standard deviations around mean to consider for demand truncation.
 	s_spread : float
 		Number of (demand) standard deviations around :math:`(s,S)` estimates to consider.
+	oul_matrix : ndarray, optional
+		User-specified matrix of order-up-to levels; ``oul_matrix[t,x]`` = optimal
+		order-up-to level in period :math:`t` if we begin period :math:`t`
+		with :math:`IL_t = x`. ``t=0`` is ignored. If provided, then ``x_range`` must also be provided.
+	x_range : ndarray, optional
+		User-specified list of :math:`x`-values used in the discretization, i.e.,
+		indices of the columns of ``cost_matrix`` and ``oul_matrix``. 
 
 	Returns
 	-------
 	reorder_points : list
 		List of reorder points in each time period. [:math:`s^*_t`]
 	order_up_to_levels : list
 		List of order-up-to levels in each time period. [:math:`S^*_t`]
@@ -151,30 +179,36 @@
 	cost_matrix : ndarray
 		Matrix of DP costs; ``cost_matrix[t,x]`` = optimal expected cost
 		in periods :math:`t,\\ldots,T` if we begin period :math:`t` with
 		:math:`IL_t = x` (and act optimally thereafter). [:math:`\\theta_t(x)`]
 	oul_matrix : ndarray
 		Matrix of order-up-to levels; ``oul_matrix[t,x]`` = optimal
 		order-up-to level in period :math:`t` if we begin period :math:`t`
-		with :math:`IL_t = x`.
+		with :math:`IL_t = x`. ``t=0`` is ignored.
 	x_range : list
-		Vector of :math:`x`-values used in the discretization, i.e.,
+		List of :math:`x`-values used in the discretization, i.e.,
 		indices of the columns of ``cost_matrix`` and ``oul_matrix``.
 
 	Raises
 	------
 	ValueError
 		If ``num_periods`` <= 0 or is non-integer.
 	ValueError
 		If ``holding_cost``, ``stockout_cost``, ``purchase_cost``, ``fixed_cost``,
 		``demand_mean``, or ``demand_sd`` < 0 for any time period.
 	ValueError
+		If ``demand_mean`` or ``demand_standard_deviation`` is ``None`` and 
+		``demand_source`` is ``None``.
+	ValueError
 		If ``discount_factor`` <= 0 or > 1 for any time period.
 	ValueError
 		If ``terminal_holding_cost`` < 0 or ``terminal_stockout_cost`` < 0.
+	ValueError
+		If ``oul_matrix`` is provided but ``x_range`` is not, or ``x_range`` does not contain all
+		values in ``oul_matrix``.
 
 
 	**Equation Used** (equation (4.66)):
 
 	.. math::
 
 		\\theta_t(x) = \\min_{y \\ge x} \\{K\\delta(y-x) + c(y-x) + g(y) +
@@ -233,110 +267,138 @@
 
 		>>> s, S, cost, _, _, _ = finite_horizon_dp(5, 1, 20, 1, 20, 2, 50, 100, 20)
 		>>> s
 		[0, 110, 110, 110, 110, 111]
 		>>> S
 		[0, 133.0, 133.0, 133.0, 133.0, 126.0]
 		>>> cost
-		1558.6946467384014
+		1558.6946467384012
 	"""
 
-	# TODO: handle non-normal demand_list
-	# TODO: handle arbitrary discretizations
-
 	# Validate singleton parameters.
 	if num_periods <= 0 or not is_integer(num_periods): raise ValueError("num_periods must be a positive integer")
 	if terminal_holding_cost < 0: raise ValueError("terminal_holding_cost must be non-negative")
 	if terminal_stockout_cost < 0: raise ValueError("terminal_stockout_cost must be non-negative")
 
 	# Replace scalar parameters with lists (multiple copies of scalar).
 	holding_cost = np.array(ensure_list_for_time_periods(holding_cost, num_periods, var_name="holding_cost"))
 	stockout_cost = np.array(ensure_list_for_time_periods(stockout_cost, num_periods, var_name="stockout_cost"))
 	purchase_cost = np.array(ensure_list_for_time_periods(purchase_cost, num_periods, var_name="purchase_cost"))
 	fixed_cost = np.array(ensure_list_for_time_periods(fixed_cost, num_periods, var_name="fixed_cost"))
 	discount_factor = np.array(ensure_list_for_time_periods(discount_factor, num_periods, var_name="discount_factor"))
 	demand_mean = np.array(ensure_list_for_time_periods(demand_mean, num_periods, var_name="mean"))
 	demand_sd = np.array(ensure_list_for_time_periods(demand_sd, num_periods, var_name="demand_sd"))
+	demand_source = np.array(ensure_list_for_time_periods(demand_source, num_periods, var_name="demand_source"))
+
+	# Build demand_source, if not provided; and get mean and SD, if demand_source is provided.
+	# After this step, demand_mean[t], demand_sd[t], and demand_source[t] will be reliably set for all t.
+	for t in range(1, num_periods + 1):
+		if demand_source[t] is None:
+			demand_source[t] = DemandSource(type='N', mean=demand_mean[t], standard_deviation=demand_sd[t])
+		else:
+			demand_mean[t] = demand_source[t].mean or demand_source[t].demand_distribution.mean()
+			demand_sd[t] = demand_source[t].standard_deviation or demand_source[t].demand_distribution.std()
 
 	# Validate other parameters.
 	if not np.all(np.array(holding_cost[1:]) >= 0): raise ValueError("holding_cost must be non-negative")
 	if not np.all(np.array(stockout_cost[1:]) >= 0): raise ValueError("stockout_cost must be non-negative")
 	if not np.all(np.array(purchase_cost[1:]) >= 0): raise ValueError("purchase_cost must be non-negative")
 	if not np.all(np.array(fixed_cost[1:]) >= 0): raise ValueError("fixed_cost must be non-negative")
 	if not np.all(np.array(discount_factor[1:]) > 0) or \
 		not np.all(np.array(discount_factor[1:]) <= 1): raise ValueError("discount_factor must be <0 and <=1")
-	if not np.all(np.array(demand_mean[1:]) >= 0): raise ValueError("mean must be non-negative")
+	if not np.all(np.array(demand_mean[1:]) >= 0): raise ValueError("demand_mean must be non-negative")
 	if not np.all(np.array(demand_sd[1:]) >= 0): raise ValueError("demand_sd must be non-negative")
-
+	if (demand_mean is None or demand_sd is None) and demand_source is None:
+		raise ValueError("You must provide either demand_mean and demand_standard_deviation, or demand_source")
+	
 	# Determine truncation for D: mu +/- d_spread * sigma (but no negative values)
 	# (accounting appropriately for variations among periods)
 	d_min = int(max(0, round(np.min(demand_mean[1:]) - d_spread * np.max(demand_sd[1:]))))
 	d_max = int(round(np.max(demand_mean[1:]) + d_spread * np.max(demand_sd[1:])))
 	d_range = np.array(range(d_min, d_max + 1))
 
 	# Calculate total probability of demand outside d_range for each t, and
 	# raise warning if > trunc_tol for any t. (prob is an array.)
 	# Ignore entry 0 (o/w divide-by-0) but then add back an entry for 0 to keep
 	# things consistent.
-	prob = norm.cdf(d_min, demand_mean[1:], demand_sd[1:]) + \
-		   (1 - norm.cdf(d_max, demand_mean[1:], demand_sd[1:]))
+	prob = [demand_source[t].demand_distribution.cdf(d_min) + \
+		    (1 - demand_source[t].demand_distribution.cdf(d_max)) for t in range(1, num_periods + 1)]
+	# prob = norm.cdf(d_min, demand_mean[1:], demand_sd[1:]) + \
+	# 	   (1 - norm.cdf(d_max, demand_mean[1:], demand_sd[1:]))
 	prob = np.append([0], prob)
 	if np.any(prob > trunc_tol):
-		warnings.warn("Total probability of demand outside demand-truncation range exceeds trunc_tol for at least one "
-					  "period.")
+		warnings.warn("Total probability of demand outside demand-truncation range exceeds trunc_tol for at least one period.")
 
 	# Calculate alpha (= p/(p+h)) in each period.
 	alpha = np.zeros(num_periods+1)
 	alpha[0] = 0
 	alpha[1:num_periods] = np.divide(stockout_cost[1:num_periods],
 									 (stockout_cost[1:num_periods] + holding_cost[1:num_periods]))
 	# Include terminal costs in alpha[T].
 	alpha[num_periods] = \
 		np.divide((stockout_cost[num_periods] + terminal_stockout_cost),
 				  (stockout_cost[num_periods] + terminal_stockout_cost +
 				   holding_cost[num_periods] + terminal_holding_cost))
 
 	# Calculate newsvendor solution for each period, or use mu if sigma = 0.
-	# TODO: MATLAB code just uses mu in every case; why?
 	nv = np.zeros(num_periods+1)
 	for t in range(1, num_periods+1):
 		nv[t] = demand_mean[t]
 #		if demand_sd[t] == 0:
 #			nv[t] = mean[t]
 #		else:
 #			nv[t] = norm.ppf(alpha[t], mean[t], demand_sd[t])
 
 	# Calculate EOQB.
 	Q = [economic_order_quantity_with_backorders(fixed_cost[t], holding_cost[t],
 			stockout_cost[t], demand_mean[t])[0] for t in range(1, num_periods+1)]
 
-	# Determine initial truncation for x:
-	# - estimate s = newsvendor solution, S = s + EOQB
-	# - then subtract s_spread * sigma from s and add s_spread * sigma to S
-	# - then, subtract mu + d_spread * sigma from s to account for demand
-	# (accounting appropriately for variations among periods, and adjusting
-	# period T to include terminal costs)
-	x_min = int(round(np.min(nv[1:]) - np.max(demand_mean[1:]) - np.max(demand_sd[1:]) * (s_spread + d_spread)))
-	x_max = int(round(np.max(nv[1:]) + np.max(Q[1:]) + np.max(demand_sd[1:]) * s_spread))
-	x_range = np.array(range(x_min, x_max+1))
+	# Determine initial truncation for x.
+	# Did user specify oul_matrix?
+	if oul_matrix is not None:
+		user_provided_oul_matrix = True
+		# Make sure x_range is also provided and contains all OULs.
+		if x_range is None:
+			raise ValueError('If oul_matrix is provided, then x_range must also be provided.')
+		elif (np.amax(np.amax(oul_matrix)) not in x_range) or \
+			(np.amin(np.amin(oul_matrix)) not in x_range):
+			raise ValueError('x_range must contain all oul_matrix values.')
+		else:
+			x_min = int(np.amin(x_range))
+			x_max = int(np.amax(x_range))
+	elif x_range is not None:
+		user_provided_oul_matrix = False
+		x_min = int(np.amin(x_range))
+		x_max = int(np.amax(x_range))
+	else:
+		user_provided_oul_matrix = False
+		# - estimate s = newsvendor solution, S = s + EOQB
+		# - then subtract s_spread * sigma from s and add s_spread * sigma to S
+		# - then, subtract mu + d_spread * sigma from s to account for demand
+		# (accounting appropriately for variations among periods, and adjusting
+		# period T to include terminal costs)
+		x_min = int(round(np.min(nv[1:]) - np.max(demand_mean[1:]) - np.max(demand_sd[1:]) * (s_spread + d_spread)))
+		x_max = int(round(np.max(nv[1:]) + np.max(Q[1:]) + np.max(demand_sd[1:]) * s_spread))
+		x_range = np.array(range(x_min, x_max+1))
 
 	# Note:
 	# - to get x value from index i, use x_range[i]
 	# - to get index from x value, use x - x_min
 	# Example: x_range = 10:20; then x_range[3] = 13 and 13 - x_min = 3.
 
 	# Start with initial truncation range; abort, expand, and re-try if necessary.
 	done = False
 	while not done:
 
 		# Allocate arrays.
 		reorder_points = [0] * (num_periods+1)
 		order_up_to_levels = [0] * (num_periods+1)
 		cost_matrix = np.zeros((num_periods+2, len(x_range)))
-		oul_matrix = np.zeros((num_periods+1, len(x_range)))
+		if not user_provided_oul_matrix:
+			oul_matrix = np.zeros((num_periods+1, len(x_range)))
 		H = np.zeros((num_periods+1, len(x_range)))
 
 		# Initialize abort (will be set to true if range is not large enough)
 		abort = False
 
 		# Initialize warning flags (will be set to True when warnings are
 		# issued to avoid duplication).
@@ -347,38 +409,42 @@
 			= terminal_holding_cost * np.maximum(x_range, 0) + \
 			  terminal_stockout_cost * np.maximum(-x_range, 0)
 
 		# Loop backwards through periods.
 		for t in range(num_periods, 0, -1):
 
 			# Calculate probability vector for demand.
-			prob = norm.cdf(d_range + 0.5, demand_mean[t], demand_sd[t]) - \
-				   norm.cdf(d_range - 0.5, demand_mean[t], demand_sd[t])
+			if demand_source[t].is_discrete:
+				prob = [demand_source[t].demand_distribution.pmf(d) for d in d_range]
+			else:
+				prob = [demand_source[t].demand_distribution.cdf(d + 0.5) - \
+						demand_source[t].demand_distribution.cdf(d - 0.5) for d in d_range]
+			# prob = norm.cdf(d_range + 0.5, demand_mean[t], demand_sd[t]) - \
+			# 	   norm.cdf(d_range - 0.5, demand_mean[t], demand_sd[t])
 
 			# Calculate H_t(y).
 			for y in range(x_min, x_max + 1):
 
 				# Initialize cost.
 				cost = 0.0
 
-				# Calculate n(y) and \bar{n}(y).
+				# Calculate n(y) and \bar{n}(y). 
 				n, n_bar = lf.normal_loss(y, demand_mean[t], demand_sd[t])
 
 				# Calculate current-period (newsvendor) cost.
-				cost += holding_cost[t] * n_bar + stockout_cost[t] * n;
+				cost += holding_cost[t] * n_bar + stockout_cost[t] * n
 
 				# Truncate demand range to avoid y-d exceeding x bounds.
 				# Need x_min <= y - d <= x_max.
 				# Therefore d_eff (d effective) must be between y - x_max
 				# and y - x_min.
 				d_eff = np.maximum(np.minimum(d_range, y - x_min), y - x_max)
 
 				# Calculate amount of demand probability that was truncated
 				# and issue warning if truncprob > trunc_tol
-				# TODO: fix this -- generates too many warnings
 				#truncprob = np.dot(prob, d_range != d_eff)
 				#if truncprob > trunc_tol:
 				#	warnings.warn('Total probability of truncated demand exceeds trunc_tol: t = {:d}, y = {:d}, truncprob = {:f}'.format(t, y, truncprob))
 
 				# Calculate future cost for this y.
 				future_cost = discount_factor[t] * np.dot(prob,
 								cost_matrix[t+1, y - d_eff - x_min])
@@ -392,41 +458,53 @@
 			# Loop through possible x values.
 			for x in range(x_min, x_max + 1):
 
 				# Initialize best_cost to something big (keeps track of best
 				# cost found for this t and x).
 				best_cost = float("inf")
 
+				# Did user provide oul_matrix? 
+				if user_provided_oul_matrix:
+					# Only consider y equal to value specified in oul_matrix.
+					y_range = [oul_matrix[t, x - x_min]]
+				else:
+					# Consider y = x, ..., x_max.
+					y_range = list(range(x, x_max + 1))
+
 				# Loop through possible y values.
-				for y in range(x, x_max + 1):
+				for y in y_range:
 
 					# Initialize cost.
 					cost = 0.0
 
 					# Calculate ordering cost.
 					if y > x:
 						cost += purchase_cost[t] * (y - x) + fixed_cost[t]
 
 					# Add H_t(y).
-					cost += H[t, y - x_min]
+					cost += H[t, int(y - x_min)]
 
 					# Compare cost to current best.
 					if cost < best_cost:
 						best_cost = cost
 						best_y = y
 
 						# If this is the largest y in range (and range has more
 						# than one element), abort and increase upper range.
 						if y == x_max and x < x_max:
-							warnings.warn('Cost is still decreasing at upper end of y range; increasing upper range '
-										  'and retrying: t = {:d}, x = {:d}, y = {:d}.'.format(t, x, y))
-							abort = True
-							x_max = x_max * 2
-							x_range = np.array(range(x_min, x_max + 1))
-							break
+							if user_provided_oul_matrix:
+								warnings.warn('Cost is still decreasing at upper end of y range; did not increase upper range '
+					 						'because oul_matrix was provided: t = {:d}, x = {:d}, y = {:d}.'.format(t, x, y))
+							else:
+								warnings.warn('Cost is still decreasing at upper end of y range; increasing upper range '
+											'and retrying: t = {:d}, x = {:d}, y = {:d}.'.format(t, x, y))
+								abort = True
+								x_max = x_max * 2
+								x_range = np.array(range(x_min, x_max + 1))
+								break
 
 				# If abort flag was set in for-y loop, exit for-x loop.
 				if abort:
 					break
 
 				# Store best cost and best action for this t, x.
 				cost_matrix[t, x - x_min] = best_cost
@@ -446,15 +524,17 @@
 					reorder_points[t] += 1
 
 			# Raise warning if truncation makes it so that probability of
 			# demand bringing IL below x_range > trunc_tol (i.e., if
 			# P(s - D < x_min) > trunc_tol). (Issue warning in each period
 			# in which there is a violation.)
 			prob_demand_below_range = 1 - \
-				norm.cdf(reorder_points[t] - x_min, demand_mean[t], demand_sd[t])
+				demand_source[t].demand_distribution.cdf(reorder_points[t] - x_min)
+			# prob_demand_below_range = 1 - \
+			# 	norm.cdf(reorder_points[t] - x_min, demand_mean[t], demand_sd[t])
 			if prob_demand_below_range > trunc_tol:
 				warnings.warn('Probability that demand brings IL below x-truncation range exceeds trunc_tol: t = {:d}, prob = {:f}'.format(t, prob_demand_below_range))
 
 		# If made it through all t without abort flag, set done = True.
 		if not abort:
 			done = True
 
@@ -475,22 +555,22 @@
 		demand_mean,
 		demand_sd,
 		discount_factor=1.0):
 	"""
 	Calculate the "myopic" bounds for the finite-horizon inventory optimization problem,
 	with or without fixed costs. 
 
-	See Sections 4.3.3 and 4.4.3 of Snyder and Shen (2019) for discussion and
+	See Sections 4.3.3 and 4.4.3 of |fosct| for discussion and
 	notation.
 
 	The myopic bounds :math:`\\bar{s}_t`, :math:`\\underline{S}_t`,
 	and :math:`\\bar{S}_t` are denoted :math:`r^+(t)`, :math:`s^+(t)`, and :math:`s^++(t)`,
 	respectively, in Zipkin (2000). (Zipkin does not have an analogous quantity
-	to :math:`\\underline{s}_t`.) They are not used in Snyder and Shen
-	(2019), but the bounds are given in terms of Snyder-Shen notation below.
+	to :math:`\\underline{s}_t`.) They are not used in |fosct|, 
+	but the bounds are given in terms of |fosct| notation below.
 
 	Demands are assumed to be normally distributed.
 
 	Most parameters may be given as a singleton or a list. If given as a
 	singleton, the parameter will be assumed to be the same in every time
 	period. If given as a list, the list must be of length ``num_periods`` or
 	``num_periods``\+1.
@@ -573,15 +653,15 @@
 
 	.. math::
 
 		\\bar{s}_t = \\text{the value of } y \\le \\underline{S}_t \\text{ such that } G_t(y) = G_t(\\underline{S}_t) + K_t - \\gamma_tK_{t+1},
 
 	where :math:`G_t(y)` is the myopic newsvendor cost function in period :math:`t`,
 	denoted :math:`G_i(y)` in Veinott (1966) and
-	as :math:`C^+(t,y)` in Zipkin (2000), and is implemented in ``stockpyl.newsvendor.myopic()``.)
+	as :math:`C^+(t,y)` in Zipkin (2000), and is implemented in :func:`stockpyl.newsvendor.myopic`.)
 
 	In the fourth equation, if :math:`K_t - \\gamma_tK_{t+1} < 0`, then :math:`\\bar{s}_t` is invalid and
 	``s_overbar[t]`` is set to ``None``.
 
 
 	References
 	----------
@@ -601,16 +681,14 @@
 
 		>>> S_underbar, S_overbar, s_underbar, s_overbar = myopic_bounds(5, 1, 20, 1, 20, 2, 50, 100, 20)
 		>>> S_underbar[1], S_overbar[1], s_underbar[1], s_overbar[1]
 		(133.36782387894158, 191.66022942788436, 110.26036848597217, 133.36782387894158)
 
 	"""
 
-	# TODO: unit tests
-
 	# Validate singleton parameters.
 	assert num_periods > 0 and is_integer(num_periods), "num_periods must be a positive integer."
 	assert terminal_holding_cost >= 0, "terminal_holding_cost must be non-negative"
 	assert terminal_stockout_cost >= 0, "terminal_stockout_cost must be non-negative"
 
 	# Replace scalar parameters with lists (multiple copies of scalar).
 	holding_cost = np.array(ensure_list_for_time_periods(holding_cost, num_periods, var_name="holding_cost"))
@@ -681,66 +759,7 @@
 											  h[t], p[t], c[t], c[t+1], demand_mean[t],
 											  demand_sd[t], discount_factor[t], left_half=True)
 		else:
 			s_overbar[t] = None
 
 	return S_underbar, S_overbar, s_underbar, s_overbar
 
-
-# TODO: delete or move this
-
-if __name__ == "__main__":
-
-	instance = load_instance("problem_4_29")
-
-	# num_periods = 6
-	# holding_cost = [1, 1, 1, 1, 2, 2]
-	# stockout_cost = [20, 20, 10, 15, 10, 10]
-	# terminal_holding_cost = 4
-	# terminal_stockout_cost = 50
-	# purchase_cost = [0.2, 0.8, 0.5, 0.5, 0.2, 0.8]
-	# fixed_cost = 100
-	# demand_mean = [20, 60, 110, 200, 200, 40]
-	# demand_sd = [4.6000, 11.9000, 26.4000, 32.8000, 1.8000, 8.5000]
-	# discount_factor = 0.98
-	# initial_inventory_level = 0
-
-	S_underbar, S_overbar, s_underbar, s_overbar = myopic_bounds(
-				instance['num_periods'], 
-				instance['holding_cost'], 
-				instance['stockout_cost'], 
-				instance['terminal_holding_cost'], 
-				instance['terminal_stockout_cost'], 
-				instance['purchase_cost'], 
-				instance['fixed_cost'], 
-				instance['demand_mean'], 
-				instance['demand_sd'], 
-				instance['discount_factor']
-		)
-
-	# Solve problem.
-	reorder_points, order_up_to_levels, total_cost, cost_matrix, oul_matrix, \
-		x_range = finite_horizon_dp(				
-				instance['num_periods'], 
-				instance['holding_cost'], 
-				instance['stockout_cost'], 
-				instance['terminal_holding_cost'], 
-				instance['terminal_stockout_cost'], 
-				instance['purchase_cost'], 
-				instance['fixed_cost'], 
-				instance['demand_mean'], 
-				instance['demand_sd'], 
-				instance['discount_factor'], 
-				instance['initial_inventory_level']
-		)
-
-	results = []
-	for t in range(1, num_periods+1):
-		results.append([t, reorder_points[t], order_up_to_levels[t], S_underbar[t], S_overbar[t],
-					   s_underbar[t], s_overbar[t]])
-
-	print(tabulate(results, headers=["t", "s", "S", "S_underbar", "S_overbar", "s_underbar", "s_overbar"]))
-
-	print(S_underbar, S_overbar, s_underbar, s_overbar)
-
-	# S_underbar, S_overbar, s_underbar, s_overbar = myopic_bounds(5, 1, 20, 1, 20, 2, 50, 100, 20)
-	# print(S_underbar[1], S_overbar[1], s_underbar[1], s_overbar[1])
```

### Comparing `stockpyl-0.1.0a0/stockpyl/optimization.py` & `stockpyl-1.0.0/src/stockpyl/optimization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 # ===============================================================================
 # stockpyl - optimization Module
 # -------------------------------------------------------------------------------
-# Version: 0.0.0
-# Updated: 01-30-2022
 # Author: Larry Snyder
 # License: GPLv3
 # ===============================================================================
 
-"""The :mod:`optimization` module contains optimization-related code used in other
+"""
+.. include:: ../../globals.inc
+
+Overview 
+--------
+
+The |mod_optimization| module contains optimization-related code used in other
 modules.
 
+API Reference
+-------------
+
+
 """
 
 
 import math
 
 
 def golden_section_search(f, a, b, tol=1e-5, verbose=False):
 	"""Golden-section search. Adapted from https://en.wikipedia.org/wiki/Golden-section_search.
 	This implementation reuses function evaluations, saving 1/2 of the evaluations
 	per iteration, and returns a bounding interval.
 
-	Given a function ``f`` with a single local minimum in the interval [``a``,``b``],
+	Given a function ``f`` with a single local minimum in the interval [``a``, ``b``],
 	returns a point within ``tol`` of the minimizer.
 
 	**Example**:
 
 	.. testsetup:: *
 
 		from stockpyl.optimization import *
 
 	.. doctest::
 
 		>>> f = lambda x: (x-2)**2
 		>>> a = 1
 		>>> b = 5
 		>>> tol = 1e-5
-		>>> x = golden_section_search(f, a, b, tol)
-		>>> print(x)
-		2.0000005374905
+		>>> x, fx = golden_section_search(f, a, b, tol)
+		>>> x
+		2.0000005374905 
+		>>> fx
+		2.888960377059731e-13
 
 	Parameters
 	----------
 	f : function
 		Function to optimize.
 	a : float
 		Lower end of interval to optimize over.
@@ -58,16 +68,14 @@
 	-------
 	x_star : float
 		Optimizer of ``f``.
 	f_star : float
 		Optimal value of ``f``.
 
 	"""
-	# TODO: comment this better
-
 	# Calculate golden-section quantities.
 	invphi = (math.sqrt(5) - 1) / 2  # 1 / phi
 	invphi2 = (3 - math.sqrt(5)) / 2  # 1 / phi^2
 
 	(a, b) = (min(a, b), max(a, b))
 	h = b - a
 	if h <= tol:
```

### Comparing `stockpyl-0.1.0a0/stockpyl/rq.py` & `stockpyl-1.0.0/src/stockpyl/rq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 # ===============================================================================
 # stockpyl - rq Module
 # -------------------------------------------------------------------------------
-# Version: 0.0.0
-# Updated: 01-30-2022
 # Author: Larry Snyder
 # License: GPLv3
 # ===============================================================================
 
-"""The :mod:`rq` module contains code for solving the :math:`(r,Q)` problem.
+"""
+.. include:: ../../globals.inc
+
+Overview 
+--------
+
+The |mod_rq| module contains code for solving the |rq| optimization problem, 
+including a number of approximations.
+
+.. note:: |fosct_notation|
 
-The notation and references (equations, sections, examples, etc.) used below
-refer to Snyder and Shen, *Fundamentals of Supply Chain Theory*, 2nd edition
-(2019).
+.. seealso::
 
+	For an overview of single-echelon inventory optimization in |sp|,
+	see the :ref:`tutorial page for single-echelon inventory optimization<tutorial_seio_page>`.
+
+API Reference
+-------------
 """
 
 from scipy import integrate
 from scipy.stats import norm
 from scipy.stats import poisson
 from scipy.optimize import fsolve
 
 from stockpyl.newsvendor import *
 from stockpyl.eoq import *
 import stockpyl.loss_functions as lf
 
 
 def r_q_cost(reorder_point, order_quantity, holding_cost, stockout_cost,
 			 fixed_cost, demand_mean, demand_sd, lead_time):
-	"""Calculate the exact cost of the given solution for an :math:`(r,Q)`
+	"""Calculate the exact cost of the given solution for an |rq|
 	policy with given parameters. Assumes demand is normally distributed.
 
 	Parameters
 	----------
 	reorder_point : float
 		Reorder point. [:math:`r`]
 	order_quantity : float
@@ -79,28 +89,26 @@
 	.. doctest::
 
 		>>> r_q_cost(126.8, 328.5, 0.225, 7.5, 8, 1300, 150, 1/12)
 		78.07116250928294
 
 	"""
 
-	# TODO handle non-normal demand
-
 	# Check that parameters are positive/non-negative.
 	if order_quantity <= 0: raise ValueError("order_quantity must be positive")
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if fixed_cost <= 0: raise ValueError("fixed_cost must be positive")
 	if demand_mean < 0: raise ValueError("mean must be non-negative")
 	if demand_sd < 0: raise ValueError("demand_sd must be non-negative")
 	if lead_time < 0: raise ValueError("lead_time must be non-negative")
 
 	# Calculate mu and sigma (mean and SD of lead-time demand).
 	mu = demand_mean * lead_time
-	sigma = demand_sd * np.sqrt(lead_time)
+	sigma = demand_sd * math.sqrt(lead_time)
 
 	# Build newsvendor cost function. (Note: lead_time=0 in newsvendor even
 	# though LT in (r,Q) <> 0.)
 	newsvendor_cost = lambda S: newsvendor_normal_cost(S, holding_cost, stockout_cost,
 												  mu, sigma, lead_time=0)
 
 	# Calculate integral of g(.) function.
@@ -168,33 +176,31 @@
 	.. doctest::
 
 		>>> r_q_optimal_r_for_q(300, 0.225, 7.5, 1300, 150, 1/12)
 		129.4272799263067
 
 	"""
 
-	# TODO handle non-normal demand
-
 	# Check that parameters are positive/non-negative.
 	if order_quantity <= 0: raise ValueError("order_quantity must be positive")
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if demand_mean < 0: raise ValueError("mean must be non-negative")
 	if demand_sd < 0: raise ValueError("demand_sd must be non-negative")
 	if lead_time < 0: raise ValueError("lead_time must be non-negative")
 
 	# Calculate mu and sigma (mean and SD of lead-time demand).
 	mu = demand_mean * lead_time
-	sigma = demand_sd * np.sqrt(lead_time)
+	sigma = demand_sd * math.sqrt(lead_time)
 
 	# Find S^* (= minimizer of g(.)).
 	S, _ = newsvendor_normal(holding_cost, stockout_cost, mu, sigma)
 
 	# Initialize bounds and midpoint for bisection search.
-	r_lo = S - 5 * order_quantity  # TODO: better way to do this?
+	r_lo = S - 5 * order_quantity  
 	r_hi = S
 	r = (r_lo + r_hi) / 2
 
 	# Calculate g(r) and g(r+Q).
 	gr = newsvendor_normal_cost(r, holding_cost, stockout_cost, mu, sigma)
 	grQ = newsvendor_normal_cost(r+order_quantity, holding_cost, stockout_cost, mu, sigma)
 
@@ -219,14 +225,17 @@
 
 def r_q_eil_approximation(holding_cost, stockout_cost, fixed_cost,
 						  demand_mean, demand_sd,
 						  lead_time, tol=1e-6):
 	"""Determine :math:`r` and :math:`Q` using the "expected-inventory-level" (EIL)
 	approximation. Assumes demand is normally distributed.
 
+	The EIL approximation is one of the oldest and most widely known approximations for
+	the |rq| optimization problem, dating back to Whitin (1953) and Hadley and Whitin (1963).
+
 	Parameters
 	----------
 	holding_cost : float
 		Holding cost per item per unit time. [:math:`h`]
 	stockout_cost : float
 		Stockout cost per item per unit time. [:math:`p`]
 	fixed_cost : float
@@ -265,42 +274,48 @@
 
 		r = F^{-1}\\left(1 - \\frac{Qh}{p\\lambda}\\right)
 
 		Q = \\sqrt{\\frac{2\\lambda[K + pn(r)]}{h}}
 
 		g(r,Q) = h\\left(r - \\lambda L + \\frac{Q}{2}\\right) + \\frac{K\\lambda}{Q} + \\frac{p\\lambda n(r)}{Q}
 
-	**Algorithm Used:** Iterative algorithm for EIL approximation for :math:`(r,Q)` policy (Algorithm 5.1)
+	**Algorithm Used:** Iterative algorithm for EIL approximation for |rq| policy (Algorithm 5.1)
+
+
+	References
+	----------
+	T. M. Whitin, *The Theory of Inventory Management*, Princeton University Press, Princeton, NJ, 1953.
+
+	G. Hadley and T. M. Whitin, *Analysis of Inventory Systems*, Prentice-Hall, Englewood Cliffs, NJ, 1963.
+
 
 	**Example** (Example 5.2):
 
 	.. testsetup:: *
 
 		from stockpyl.rq import *
 
 	.. doctest::
 
 		>>> r_q_eil_approximation(0.225, 7.5, 8, 1300, 150, 1/12)
 		(213.97044213580244, 318.5901810768729, 95.45114022285196)
 
 	"""
 
-	# TODO handle non-normal demand
-
 	# Check that parameters are positive/non-negative.
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if fixed_cost <= 0: raise ValueError("fixed_cost must be positive")
 	if demand_mean < 0: raise ValueError("mean must be non-negative")
 	if demand_sd < 0: raise ValueError("demand_sd must be non-negative")
 	if lead_time < 0: raise ValueError("lead_time must be non-negative")
 
 	# Calculate mu and sigma (mean and SD of lead-time demand).
 	mu = demand_mean * lead_time
-	sigma = demand_sd * np.sqrt(lead_time)
+	sigma = demand_sd * math.sqrt(lead_time)
 
 	# Initialize: Q = EOQ, r = 0.
 	Q, _ = economic_order_quantity(fixed_cost, holding_cost, demand_mean)
 	r = 0
 	Q_prev = float("inf")
 	r_prev = float("inf")
 
@@ -313,29 +328,31 @@
 
 		# Solve for r.
 		r = norm.ppf(1 - Q * holding_cost / (stockout_cost * demand_mean),
 					 mu, sigma)
 
 		# Solve for Q.
 		loss, _ = lf.normal_loss(r, mu, sigma)
-		Q = np.sqrt(2 * demand_mean * (fixed_cost + stockout_cost * loss) / holding_cost)
+		Q = math.sqrt(2 * demand_mean * (fixed_cost + stockout_cost * loss) / holding_cost)
 
 	# Calculate approximate expected cost per unit time.
 	loss, _ = lf.normal_loss(r, mu, sigma)
 	cost = holding_cost * (r - mu + Q/2) + fixed_cost * demand_mean / Q \
 		   + stockout_cost * demand_mean * loss / Q
 
 	return r, Q, cost
 
 
 def r_q_eoqb_approximation(holding_cost, stockout_cost, fixed_cost,
 						   demand_mean, demand_sd, lead_time):
 	"""Determine :math:`r` and :math:`Q` using the "EOQ with backorders" (EOQB)
 	approximation. Assumes demand is normally distributed.
 
+	See Zheng (1992) for a thorough exploration of the EOQB approximation.
+
 	Parameters
 	----------
 	holding_cost : float
 		Holding cost per item per unit time. [:math:`h`]
 	stockout_cost : float
 		Stockout cost per item per unit time. [:math:`p`]
 	fixed_cost : float
@@ -368,29 +385,34 @@
 
 		Q^* = \\sqrt{\\frac{2K\\lambda(h+p)}{hp}}
 
 		g(r) = g(r+Q)
 
 	where :math:`g(y)` is the newsvendor cost function.
 
+
+	References
+	----------
+	Y.-S. Zheng, On Properties of Stochastic Inventory Systems, *Management Science*
+	38(1), 87-103 (1992).
+
+
 	**Example** (Example 5.2):
 
 	.. testsetup:: *
 
 		from stockpyl.rq import *
 
 	.. doctest::
 
 		>>> r_q_eoqb_approximation(0.225, 7.5, 8, 1300, 150, 1/12)
 		(128.63781442427097, 308.5737801203754)
 
 	"""
 
-	# TODO handle non-normal demand
-
 	# Check that parameters are positive/non-negative.
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if fixed_cost <= 0: raise ValueError("fixed_cost must be positive")
 	if demand_mean < 0: raise ValueError("mean must be non-negative")
 	if demand_sd < 0: raise ValueError("demand_sd must be non-negative")
 	if lead_time < 0: raise ValueError("lead_time must be non-negative")
@@ -460,27 +482,25 @@
 	.. doctest::
 
 		>>> r_q_eoqss_approximation(0.225, 7.5, 8, 1300, 150, 1/12)
 		(190.3369965715624, 304.0467800264368)
 
 	"""
 
-	# TODO handle non-normal demand
-
 	# Check that parameters are positive/non-negative.
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if fixed_cost <= 0: raise ValueError("fixed_cost must be positive")
 	if demand_mean < 0: raise ValueError("mean must be non-negative")
 	if demand_sd < 0: raise ValueError("demand_sd must be non-negative")
 	if lead_time < 0: raise ValueError("lead_time must be non-negative")
 
 	# Calculate mu and sigma (mean and SD of lead-time demand).
 	mu = demand_mean * lead_time
-	sigma = demand_sd * np.sqrt(lead_time)
+	sigma = demand_sd * math.sqrt(lead_time)
 
 	# Calculate EOQ.
 	Q, _ = economic_order_quantity(fixed_cost, holding_cost, demand_mean)
 
 	# Calculate r(Q).
 	r, _ = newsvendor_normal(holding_cost, stockout_cost, mu, sigma)
 
@@ -488,14 +508,16 @@
 
 
 def r_q_loss_function_approximation(holding_cost, stockout_cost, fixed_cost,
 									demand_mean, demand_sd, lead_time, tol=1e-6):
 	"""Determine :math:`r` and :math:`Q` using the "loss function"
 	approximation. Assumes demand is normally distributed.
 
+	This approximation is due to Hadley and Whitin (1963).
+
 	Parameters
 	----------
 	holding_cost : float
 		Holding cost per item per unit time. [:math:`h`]
 	stockout_cost : float
 		Stockout cost per item per unit time. [:math:`p`]
 	fixed_cost : float
@@ -533,40 +555,44 @@
 		Q = \\sqrt{\\frac{2\\left[K\\lambda + (h+p)n^{(2)}(r)\\right]}{h}}
 
 		n(r) = \\frac{hQ}{h+p}
 
 	where :math:`n(\\cdot)` and :math:`n^{(2)}(\\cdot)` are the first- and
 	second-order loss functions for the lead-time demand distribution.
 
+
+	References
+	----------
+	G. Hadley and T. M. Whitin, *Analysis of Inventory Systems*, Prentice-Hall, Englewood Cliffs, NJ, 1963.
+
+
 	**Example** (Example 5.6):
 
 	.. testsetup:: *
 
 		from stockpyl.rq import *
 
 	.. doctest::
 
 		>>> r_q_loss_function_approximation(0.225, 7.5, 8, 1300, 150, 1/12)
 		(126.8670634479628, 328.4491421980451)
 
 	"""
 
-	# TODO handle non-normal demand
-
 	# Check that parameters are positive/non-negative.
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if fixed_cost <= 0: raise ValueError("fixed_cost must be positive")
 	if demand_mean < 0: raise ValueError("mean must be non-negative")
 	if demand_sd < 0: raise ValueError("demand_sd must be non-negative")
 	if lead_time < 0: raise ValueError("lead_time must be non-negative")
 
 	# Calculate mu and sigma (mean and SD of lead-time demand).
 	mu = demand_mean * lead_time
-	sigma = demand_sd * np.sqrt(lead_time)
+	sigma = demand_sd * math.sqrt(lead_time)
 
 	# Initialize: Q = EOQ, r = 0.
 	Q, _ = economic_order_quantity(fixed_cost, holding_cost, demand_mean)
 	r = 0
 	Q_prev = float("inf")
 	r_prev = float("inf")
 
@@ -580,23 +606,23 @@
 		# Solve for r.
 		rhs = holding_cost * Q / (holding_cost + stockout_cost)
 		fun = lambda y: lf.normal_loss(y, mu, sigma)[0] - rhs
 		r = fsolve(fun, r_prev)[0]
 
 		# Solve for Q.
 		loss2, _ = lf.normal_second_loss(r, mu, sigma)
-		Q = np.sqrt(2 * (fixed_cost * demand_mean +
+		Q = math.sqrt(2 * (fixed_cost * demand_mean +
 						 (holding_cost + stockout_cost) * loss2) / holding_cost)
 
 	return r, Q
 
 
 def r_q_cost_poisson(reorder_point, order_quantity, holding_cost, stockout_cost,
 					 fixed_cost, demand_mean, lead_time):
-	"""Calculate the exact cost of the given solution for an :math:`(r,Q)`
+	"""Calculate the exact cost of the given solution for an |rq|
 	policy with given parameters under Poisson demand.
 
 	Parameters
 	----------
 	reorder_point : float
 		Reorder point. [:math:`r`]
 	order_quantity : float
@@ -672,15 +698,15 @@
 	cost /= order_quantity
 
 	return cost
 
 
 def r_q_poisson_exact(holding_cost, stockout_cost, fixed_cost,
 					  demand_mean, lead_time):
-	"""Determine optimal :math:`r` and :math:`Q` for Poisson demand_list, using
+	"""Determine optimal :math:`r` and :math:`Q` for Poisson demands, using the
 	algorithm by Federgruen and Zheng (1992).
 
 	Parameters
 	----------
 	holding_cost : float
 		Holding cost per item per unit time. [:math:`h`]
 	stockout_cost : float
@@ -711,15 +737,23 @@
 
 	**Equations Used** (equation (5.48)):
 
 	.. math::
 
 		g(r,Q) = \\frac{K\\lambda + \\sum_{y=r+1}^{r+Q} g(y)}{Q}
 
-	where :math:`g(y)` is the newsvendor cost function for Poisson demand_list.
+	where :math:`g(y)` is the newsvendor cost function for Poisson demands.
+
+
+	References
+	----------
+	A. Federgruen and Y.-S. Zheng, An Efficient Algorithm for Computing an Optimal
+	|rq| Policy in Continuous Review Stochastic Inventory Systems, *Operations Research*
+	40(4), 808-813 (1992).
+
 
 	**Example** (Example 5.8):
 
 	.. testsetup:: *
 
 		from stockpyl.rq import *
```

### Comparing `stockpyl-0.1.0a0/stockpyl/meio.py` & `stockpyl-1.0.0/src/stockpyl/meio_general.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,37 @@
-"""Code for optimizing multi-echelon inventory systems using a variety of
-generic methods.
-# TODO: rename to meio_generic?
+# ===============================================================================
+# stockpyl - meio_general Module
+# -------------------------------------------------------------------------------
+# Author: Larry Snyder
+# License: GPLv3
+# ===============================================================================
 
-'node' and 'stage' are used interchangeably in the documentation.
+"""
+.. include:: ../../globals.inc
+
+Overview 
+--------
+
+For MEIO systems with arbitrary topology (not necessarily serial or tree systems),
+the |mod_meio_general| module can optimize base-stock levels approximately using
+relatively brute-force approaches—either coordinate descent or enumeration. These
+heuristics tend to be quite slow and not particularly accurate, but they are sometimes
+the best methods available for complex systems that are not well solved in the literature.
+
+.. note:: |node_stage|
+
+.. note:: |fosct_notation|
 
-The primary data object is the ``SupplyChainNetwork`` and the ``SupplyChainNode``s
-that it contains, which contains all of the data for the optimization instance.
+.. seealso::
 
-(c) Lawrence V. Snyder
-Lehigh University
+	For an overview of multi-echelon inventory optimization in |sp|,
+	see the :ref:`tutorial page for multi-echelon inventory optimization<tutorial_meio_page>`.
 
+API Reference
+-------------
 """
 
 import numpy as np
 from itertools import product
 from tqdm import tqdm				# progress bar
 
 from stockpyl.supply_chain_network import *
@@ -22,192 +40,28 @@
 from stockpyl.ssm_serial import *
 from stockpyl.instances import *
 import stockpyl.optimization as optimization
 
 
 # -------------------
 
-# HELPER FUNCTIONS
-
-def truncate_and_discretize(node_indices, values=None, truncation_lo=None,
-						truncation_hi=None, discretization_step=None,
-						discretization_num=None):
-	"""Determine truncated and discretized set of values for each node in network.
-
-	* If ``values`` is provided, it is assumed to be a dictionary of truncated
-	and discretized values, and it is returned without modification.
-	* If ``truncation_lo``, ``truncation_hi``, and ``discretization_step`` or
-	``discretization_num`` are provided, these are used to determine the set of values.
-	* ``truncation_lo``, ``truncation_hi``, ``discretization_step``, and
-	``discretization_num`` may each either be a dictionary (with keys equal to
-	node indices) or a singleton. If a singleton, the same value will be used for all nodes.
-	* If any or all of ``truncation_lo``, ``truncation_hi``, ``discretization_step``,
-	and ``discretization_num`` are omitted, they will be set automatically:
-		- ``truncation_lo'' is set to 0.
-		- ``truncation_hi`` is set to 100.
-		- ``discretization_step`` is set to 1 and ``discretization_num`` is set to
-		(``truncation_hi`` - ``truncation_lo``) / ``discretization_step``.
-		# TODO: use demand distribution to set lo and hi, even at upstream nodes
-
-	Parameters
-	----------
-	node_indices : list
-		List of indices of all nodes in the network.
-	values : dict, optional
-		Dictionary in which keys are node indices and values are lists of
-		truncated, discretized values; if provided, it is returned without modification.
-	truncation_lo : float or dict, optional
-		A float or dictionary indicating, for each node index, the low end of the
-		truncation range for values to test for that node. If float,
-		the same value is used for every node. If omitted, it is set automatically.
-	truncation_hi : float or dict, optional
-		A dictionary indicating, for each node index, the high end of the
-		truncation range for values levels to test for that node. If float,
-		the same value is used for every node. If omitted, it is set automatically.
-	discretization_step : float or dict, optional
-		A dictionary indicating, for each node index, the interval width to use
-		for discretization of the values to test for that node. If float,
-		the same value is used for every node. If omitted, it is set automatically.
-	discretization_num : int or dict, optional
-		A dictionary indicating, for each node index, the number of intervals to use
-		for discretization of the values to test for that node. If int,
-		the same value is used for every node. If omitted, it is set automatically.
-		Ignored if ``discretization_step`` is provided.
-
-	Returns
-	-------
-	truncated_discretized_values : dict
-		Dictionary indicating a list of truncated, discretized values for each
-		node index.
-	"""
-
-	# Define constants for default truncation and discretization settings.
-	DEFAULT_LO = 0
-	DEFAULT_HI = 100
-	DEFAULT_STEP = 1
-
-	# Were values already provided?
-	if values is None:
-		values_provided = False
-	else:
-		values_provided = False
-		for v in values.values():
-			if v is not None:
-				values_provided = True
-
-	if values_provided:
-		truncated_discretized_values = values
-	else:
-		# Determine lo, hi, step, and num.
-		lo_dict = ensure_dict_for_nodes(truncation_lo, node_indices)
-		hi_dict = ensure_dict_for_nodes(truncation_hi, node_indices)
-		step_dict = ensure_dict_for_nodes(discretization_step, node_indices)
-		num_dict = ensure_dict_for_nodes(discretization_num, node_indices)
-
-		# Initialize output dict.
-		truncated_discretized_values = {}
-
-		# Loop through nodes.
-		for n_ind in node_indices:
-
-			# Determine lo, hi, step/num for each node. If not provided,
-			# use default settings.
-			# TODO: what if lead_time_demand_distribution is not provided by demand_source object?
-			lo = lo_dict[n_ind] or DEFAULT_LO
-			hi = hi_dict[n_ind] or DEFAULT_HI
-			if step_dict[n_ind] is not None:
-				step = step_dict[n_ind]
-			elif num_dict[n_ind] is not None:
-				num = num_dict[n_ind]
-				step = (hi - lo) / (num - 1)
-			else:
-				step = DEFAULT_STEP
-
-			truncated_discretized_values[n_ind] = np.arange(lo, hi+1, step).tolist()
-
-	return truncated_discretized_values
-
-
-def base_stock_group_assignments(node_indices, groups=None):
-	"""Build dict indicating, for each node index, the group that the node is
-	assigned to for the purposes of base-stock-level optimization.
-
-	Grouping nodes that should have the same base-stock level speeds the optimization
-	since the base-stock levels for the nodes in a given group do not have to be
-	optimized individually.
-
-	Group indices will not be consecutive; some group indices will have no members.
-
-	Parameters
-	----------
-	node_indices : list
-		List of indices of all nodes in the network.
-	groups : list of sets, optional
-		A list of sets, each of which contains indices of nodes that should have the
-		same base-stock level. Any nodes not contained in any set in the list are
-		optimized individually. If omitted, all nodes are optimized individually.
-
-	Returns
-	-------
-	opt_group : dict
-		A dict in which each key is the index of a node in ``network`` and each
-		value is the index of the optimization group the node is assigned to.
-	group_list : list
-		A list in which each item is a list of node indices corresponding to one
-		group. This is the same as the ``groups`` list provided, but with
-		singletons filled in.
-	"""
-
-	# Initialize dict.
-	opt_group = {}
-
-	# Were any groups provided?
-	if groups is None:
-		opt_group = {n_ind: n_ind for n_ind in node_indices}
-	else:
-		# For each node, look for it in a group.
-		for n_ind in node_indices:
-			for node_set in groups:
-				if n_ind in node_set:
-					# Assign group in dict.
-					opt_group[n_ind] = min(node_set)
-
-			# Check whether we already assigned node; if not, assign it to its own
-			# group.
-			if n_ind not in opt_group:
-				opt_group[n_ind] = n_ind
-
-	# Build group_list.
-	group_list = []
-	for i in node_indices:
-		g = [n_ind for n_ind in node_indices if opt_group[n_ind] == i]
-		if g:
-			group_list.append(g)
-
-	return opt_group, group_list
-
-
-# -------------------
-
 # ENUMERATION
 
 def meio_by_enumeration(network, base_stock_levels=None, truncation_lo=None,
 						truncation_hi=None, discretization_step=None,
 						discretization_num=None, groups=None, objective_function=None,
 						sim_num_trials=10, sim_num_periods=1000, sim_rand_seed=None,
 						progress_bar=True, print_solutions=False):
 	"""Optimize the MEIO instance by enumerating the combinations of values of the
 	base-stock levels. Evaluate each combination using the provided objective
 	function, or simulation if not provided.
 
-	# TODO: generalize to allow parameters other than BSL
-
 	Parameters
 	----------
-	network : SupplyChainNetwork
+	network : |class_network|
 		The network to optimize.
 	base_stock_levels : dict, optional
 		A dictionary indicating, for each node index, the base-stock levels to
 		test in the enumeration. Example: {0: [0, 5, 10, 15], 1: [0, 2, 4, 6]}.
 	truncation_lo : float or dict, optional
 		A float or dictionary indicating, for each node index, the low end of the
 		truncation range for values to test for that node. If float,
@@ -236,20 +90,20 @@
 		a single argument, the dictionary of base-stock levels, and return a
 		single output, the expected cost per period. If omitted, simulation
 		will be used.
 	sim_num_trials : int, optional
 		Number of trials to run in each simulation. Ignored if ``objective_function``
 		is provided.
 	sim_num_periods : int, optional
-		Number of periods per trial in each simulation. Ignored if ``objective_function''
+		Number of periods per trial in each simulation. Ignored if ``objective_function``
 		is provided.
 	sim_rand_seed : int, optional
-		Rand seed to use for simulation. Ignored if ``objective_function'' is provided.
+		Rand seed to use for simulation. Ignored if ``objective_function`` is provided.
 	progress_bar : bool, optional
-		Display a progress bar? Ignored if ``print_solutions`` is True.
+		Display a progress bar? Ignored if ``print_solutions`` is ``True``.
 	print_solutions : bool, optional
 		Print each solution and its cost?
 
 	Returns
 	-------
 	best_S : dict
 		Dict of best base-stock levels found.
@@ -257,22 +111,21 @@
 		Best cost found.
 
 	"""
 
 	# Build dictionary indicating which optimization group each node is assigned to.
 	# (Group indices will not be consecutive; some will be empty.)
 	# Note that every set contains a node with the same index as the set.
-	opt_group, _ = base_stock_group_assignments(network.node_indices, groups=groups)
+	opt_group, _ = _base_stock_group_assignments(network.node_indices, groups=groups)
 
 	# Determine list of nodes to optimize, based on groups. Nodes that are not
 	# in the list will have their base-stock level set to the level from their group.
 	nodes_to_optimize = {opt_group[n_ind] for n_ind in network.node_indices}
 
 	# Build lists needed for truncation and discretization, based on nodes_to_optimize.
-	# TODO: wrap this in a separate function
 	dict_base_stock_levels = ensure_dict_for_nodes(base_stock_levels, network.node_indices)
 	dict_truncation_lo = ensure_dict_for_nodes(truncation_lo, network.node_indices)
 	dict_truncation_hi = ensure_dict_for_nodes(truncation_hi, network.node_indices)
 	dict_discretization_step = ensure_dict_for_nodes(discretization_step, network.node_indices)
 	dict_discretization_num = ensure_dict_for_nodes(discretization_num, network.node_indices)
 	nto_base_stock_levels = {n_ind: dict_base_stock_levels[n_ind] for n_ind in nodes_to_optimize}
 	nto_truncation_lo = {n_ind: dict_truncation_lo[n_ind] for n_ind in nodes_to_optimize}
@@ -326,15 +179,14 @@
 				else:
 					n.inventory_policy.local_base_stock_level = S_complete[n.index]
 			# Run multiple trials of simulation to evaluate solution.
 			mean_cost, _ = run_multiple_trials(network, sim_num_trials, sim_num_periods,
 											   sim_rand_seed, progress_bar=False)
 
 		# Compare to best solution found so far.
-		# TODO: do something with sem?
 		if mean_cost < best_cost:
 			best_cost = mean_cost
 			best_S = S_complete
 
 		# Print solution, if requested.
 		if print_solutions:
 			print_str = "S = {} cost = {}".format(S_complete, mean_cost)
@@ -348,83 +200,26 @@
 	return best_S, best_cost
 
 
 # -------------------
 
 # COORDINATE DESCENT
 
-def base_stock_level_bisection_search(network, node_to_optimize, lo=None, hi=None,
-						objective_function=None,
-						sim_num_trials=10, sim_num_periods=1000, sim_rand_seed=None,
-						tolerance=1e-2):
-	"""Optimize the base-stock level for one node using bisection search.
-	Evaluate each solution using the provided objective function, or simulation if not provided.
-
-	Parameters
-	----------
-	network : SupplyChainNetwork
-		The supply chain network.
-	node_to_optimize : SupplyChainNode
-		The supply chain node to optimize.
-	lo : float, optional
-		The low end of the search range. If omitted, it is set automatically.
-	hi : float, optional
-		The high end of the search range. If omitted, it is set automatically.
-	objective_function : function, optional
-		The function to use to evaluate a given solution. If omitted, simulation
-		will be used.
-	sim_num_trials : int, optional
-		Number of trials to run in each simulation. Ignored if ``objective_function``
-		is provided.
-	sim_num_periods : int, optional
-		Number of periods per trial in each simulation. Ignored if ``objective_function''
-		is provided.
-	sim_rand_seed : int, optional
-		Rand seed to use for simulation. Ignored if ``objective_function'' is provided.
-	tolerance : float, optional
-		Absolute tolerance to use for convergence. The algorithm terminates when
-		the absolute difference between the current bounds is less than the tolerance.
-
-	Returns
-	-------
-	base_stock_level : float
-		Best base-stock level found for the node.
-	cost : float
-		Cost of best solution found.
-	"""
-
-	# Determine bounds, if not provided.
-	# TODO: do this better
-	if lo is None:
-		lo = 0
-	if hi is None:
-		hi = 3 * np.sum([s.demand_source.mean for s in network.sink_nodes])
-
-	# Determine initial lo, hi, and midpoint for bisection search.
-	S_lo = lo
-	S_hi = hi
-	S = (S_lo + S_hi) / 2
-
-	# Calculate cost at
-
-
 def meio_by_coordinate_descent(network, initial_solution=None,
 							   search_lo=None, search_hi=None,
 							   groups=None, objective_function=None,
 							   sim_num_trials=10, sim_num_periods=1000, sim_rand_seed=None,
 							   tol=1e-2, line_search_tol=1e-4, verbose=False):
 	"""Optimize the MEIO instance by coordinate descent on the
 	base-stock levels. Evaluate each solution using the provided objective
 	function, or simulation if not provided.
 
-	# TODO: generalize to allow parameters other than BSL
-
 	Parameters
 	----------
-	network : SupplyChainNetwork
+	network : |class_network|
 		The network to optimize.
 	initial_solution : dict, optional
 		The starting solution, as a dict. If omitted, initial solution will be set
 		automatically.
 	search_lo : float or dict, optional
 		A float or dictionary indicating, for each node index, the low end of the
 		search range for that node. If float, the same value is used for every node.
@@ -442,62 +237,61 @@
 	objective_function : function, optional
 		The function to use to evaluate a given solution. If omitted, simulation
 		will be used.
 	sim_num_trials : int, optional
 		Number of trials to run in each simulation. Ignored if ``objective_function``
 		is provided.
 	sim_num_periods : int, optional
-		Number of periods per trial in each simulation. Ignored if ``objective_function''
+		Number of periods per trial in each simulation. Ignored if ``objective_function``
 		is provided.
 	sim_rand_seed : int, optional
-		Rand seed to use for simulation. Ignored if ``objective_function'' is provided.
+		Rand seed to use for simulation. Ignored if ``objective_function`` is provided.
 	tol : float, optional
 		Algorithm terminates when iteration fails to improve objective function by
 		more than tol.
 	line_search_tol : float, optional
 		Tolerance to use for line search (golden section search) component of algorithm.
 	verbose: bool, optional
 		Set to True to print messages at each iteration.
+		
 	Returns
 	-------
 	best_S : dict
 		Dict of best base-stock levels found.
 	best_cost : float
 		Best cost found.
 
 	"""
 
 	# Build dictionary indicating which optimization group each node is assigned to.
 	# (Group indices will not be consecutive; some will be empty.)
 	# Note that every set contains a node with the same index as the set.
-	opt_group, group_list = base_stock_group_assignments(network.node_indices, groups=groups)
+	opt_group, group_list = _base_stock_group_assignments(network.node_indices, groups=groups)
 
 	# Determine list of nodes to optimize, based on groups. Nodes that are not
 	# in the list will have their base-stock level set to the level from their group.
 	nodes_to_optimize = {opt_group[n_ind] for n_ind in network.node_indices}
 
 	# Determine bounds for search, if not provided, based on nodes_to_optimize.
 	dict_lo = ensure_dict_for_nodes(search_lo, network.node_indices)
 	dict_hi = ensure_dict_for_nodes(search_hi, network.node_indices)
 	nto_lo = {n_ind: dict_lo[n_ind] for n_ind in nodes_to_optimize}
 	nto_hi = {n_ind: dict_hi[n_ind] for n_ind in nodes_to_optimize}
-	# TODO: do this better
 	for n_ind in nodes_to_optimize:
 		if nto_lo[n_ind] is None:
 			nto_lo[n_ind] = 0
 		if nto_hi[n_ind] is None:
 			n = network.get_node_from_index(n_ind)
-			nto_hi[n_ind] = 3 * n.lead_time * np.sum([s.demand_source.mean for s in network.sink_nodes])
+			nto_hi[n_ind] = 3 * n.lead_time * float(np.sum([s.demand_source.mean for s in network.sink_nodes]))
 
 	# Determine initial solution.
 	if initial_solution is None:
-		# TODO: do this better -- set to mean implied demand
 		nto_initial_solution = {}
 		for n in nodes_to_optimize:
-			nto_initial_solution[n] = np.sum([s.demand_source.mean for s in network.sink_nodes])
+			nto_initial_solution[n] = float(np.sum([s.demand_source.mean for s in network.sink_nodes]))
 	else:
 		nto_initial_solution = {n_ind: initial_solution[n_ind] for n_ind in nodes_to_optimize}
 
 	# Shortcut to objective function.
 	def obj_fcn(S):
 		if objective_function is not None:
 			return objective_function(S)
@@ -555,49 +349,170 @@
 		else:
 			current_cost = best_cost
 			t += 1
 
 	return current_soln_complete, best_cost
 
 
-#
-# network = get_named_instance("example_6_1")
-#
-# # reindex nodes N, ..., 1 (ssm_serial.expected_cost() requires it)
-# network.reindex_nodes({0: 1, 1: 2, 2: 3})
-# obj_fcn = lambda S: expected_cost(network, local_to_echelon_base_stock_levels(network, S), x_num=100, d_num=10)
-# best_S, best_cost = meio_by_coordinate_descent(network,
-# 										initial_solution=echelon_to_local_base_stock_levels(network, {1: 6.49, 2: 12.02, 3: 22.71}),
-# 										objective_function=obj_fcn, verbose=True)
-# best_S, best_cost = meio_by_enumeration(network,
-# 										truncation_lo={1: 5, 2: 4, 3: 10},
-#  										truncation_hi={1: 7, 2: 7, 3: 12},
-# 										objective_function=obj_fcn)
-
-#
-# # T = 1000
-# # total_cost = simulation(network, T)
-# # print(total_cost / T)
-# #
-# network = get_named_instance("rong_atan_snyder_figure_1a")
-#
-# best_S, best_cost = meio_by_enumeration(network, groups=[{0}, {1, 2}, {3, 4, 5, 6}],
-# 										truncation_lo={0: 35, 1: 22, 3: 10},
-# 										truncation_hi={0: 50, 1: 31, 3: 14},
-# 										discretization_step={0: 5, 1: 3, 3: 1},
-# 										sim_num_trials=5, sim_num_periods=100, sim_rand_seed=762,
-# 										progress_bar=False,
-# 										print_solutions=True)
-# best_S, best_cost = meio_by_coordinate_descent(network, groups=[{0}, {1, 2}, {3, 4, 5, 6}],
-# 													search_lo={0: 35, 1: 22, 3: 10}, search_hi={0: 50, 1: 31, 3: 14},
-# 													sim_num_trials=1, sim_num_periods=50, sim_rand_seed=762,
-# 													verbose=True)
-#
-# # network = get_named_instance("example_4_1_network")
-# #
-# # best_S, best_cost = meio_by_enumeration(network, truncation_lo=55, truncation_hi=58, discretization_step=0.1,
-# # 											 sim_num_trials=5, sim_num_periods=500, sim_rand_seed=762,
-# # 											 progress_bar=False,
-# # 											 print_solutions=True)
-#
-#
-# print("best_S = {}, best_cost = {}".format(best_S, best_cost))
+# -------------------
+
+# HELPER FUNCTIONS
+
+def truncate_and_discretize(node_indices, values=None, truncation_lo=None,
+						truncation_hi=None, discretization_step=None,
+						discretization_num=None):
+	"""Determine truncated and discretized set of values for each node in network.
+
+	* If ``values`` is provided, it is assumed to be a dictionary of truncated
+	  and discretized values, and it is returned without modification.
+	* If ``truncation_lo``, ``truncation_hi``, and ``discretization_step`` or
+	  ``discretization_num`` are provided, these are used to determine the set of values.
+	* ``truncation_lo``, ``truncation_hi``, ``discretization_step``, and
+	  ``discretization_num`` may each either be a dictionary (with keys equal to
+	  node indices) or a singleton. If a singleton, the same value will be used for all nodes.
+	* If any or all of ``truncation_lo``, ``truncation_hi``, ``discretization_step``,
+	  and ``discretization_num`` are omitted, they will be set automatically:
+
+		- ``truncation_lo`` is set to 0.
+		- ``truncation_hi`` is set to 100.
+		- ``discretization_step`` is set to 1 and ``discretization_num`` is set to
+		  (``truncation_hi`` - ``truncation_lo``) / ``discretization_step``.
+		
+	Parameters
+	----------
+	node_indices : list
+		List of indices of all nodes in the network.
+	values : dict, optional
+		Dictionary in which keys are node indices and values are lists of
+		truncated, discretized values; if provided, it is returned without modification.
+	truncation_lo : float or dict, optional
+		A float or dictionary indicating, for each node index, the low end of the
+		truncation range for values to test for that node. If float,
+		the same value is used for every node. If omitted, it is set automatically.
+	truncation_hi : float or dict, optional
+		A dictionary indicating, for each node index, the high end of the
+		truncation range for values levels to test for that node. If float,
+		the same value is used for every node. If omitted, it is set automatically.
+	discretization_step : float or dict, optional
+		A dictionary indicating, for each node index, the interval width to use
+		for discretization of the values to test for that node. If float,
+		the same value is used for every node. If omitted, it is set automatically.
+	discretization_num : int or dict, optional
+		A dictionary indicating, for each node index, the number of intervals to use
+		for discretization of the values to test for that node. If int,
+		the same value is used for every node. If omitted, it is set automatically.
+		Ignored if ``discretization_step`` is provided.
+
+	Returns
+	-------
+	truncated_discretized_values : dict
+		Dictionary indicating a list of truncated, discretized values for each
+		node index.
+	"""
+
+	# Define constants for default truncation and discretization settings.
+	DEFAULT_LO = int()
+	DEFAULT_HI = int(100)
+	DEFAULT_STEP = int(1)
+
+	# Were values already provided?
+	if values is None:
+		values_provided = False
+	else:
+		values_provided = False
+		for v in values.values():
+			if v is not None:
+				values_provided = True
+
+	if values_provided:
+		truncated_discretized_values = values
+	else:
+		# Determine lo, hi, step, and num.
+		lo_dict = ensure_dict_for_nodes(truncation_lo, node_indices)
+		hi_dict = ensure_dict_for_nodes(truncation_hi, node_indices)
+		step_dict = ensure_dict_for_nodes(discretization_step, node_indices)
+		num_dict = ensure_dict_for_nodes(discretization_num, node_indices)
+
+		# Initialize output dict.
+		truncated_discretized_values = {}
+
+		# Loop through nodes.
+		for n_ind in node_indices:
+
+			# Determine lo, hi, step/num for each node. If not provided,
+			# use default settings.
+			lo = lo_dict[n_ind] or DEFAULT_LO
+			hi = hi_dict[n_ind] or DEFAULT_HI
+			if step_dict[n_ind] is not None:
+				step = step_dict[n_ind]
+				num  = int((hi-lo)/step)
+			elif num_dict[n_ind] is not None:
+				num  = num_dict[n_ind]
+				step = (hi-lo)/num if num and hi > lo else int(1)
+			else:
+				step = DEFAULT_STEP
+				num  = int((hi-lo)/step)
+
+			truncated_discretized_values[n_ind] = [ind*step+lo for ind in range(num+1)]
+
+	return truncated_discretized_values
+
+
+def _base_stock_group_assignments(node_indices, groups=None):
+	"""Build dict indicating, for each node index, the group that the node is
+	assigned to for the purposes of base-stock-level optimization.
+
+	Grouping nodes that should have the same base-stock level speeds the optimization
+	since the base-stock levels for the nodes in a given group do not have to be
+	optimized individually.
+
+	Group indices will not be consecutive; some group indices will have no members.
+
+	Parameters
+	----------
+	node_indices : list
+		List of indices of all nodes in the network.
+	groups : list of sets, optional
+		A list of sets, each of which contains indices of nodes that should have the
+		same base-stock level. Any nodes not contained in any set in the list are
+		optimized individually. If omitted, all nodes are optimized individually.
+
+	Returns
+	-------
+	opt_group : dict
+		A dict in which each key is the index of a node in ``network`` and each
+		value is the index of the optimization group the node is assigned to.
+	group_list : list
+		A list in which each item is a list of node indices corresponding to one
+		group. This is the same as the ``groups`` list provided, but with
+		singletons filled in.
+	"""
+
+	# Initialize dict.
+	opt_group = {}
+
+	# Were any groups provided?
+	if groups is None:
+		opt_group = {n_ind: n_ind for n_ind in node_indices}
+	else:
+		# For each node, look for it in a group.
+		for n_ind in node_indices:
+			for node_set in groups:
+				if n_ind in node_set:
+					# Assign group in dict.
+					opt_group[n_ind] = min(node_set)
+
+			# Check whether we already assigned node; if not, assign it to its own
+			# group.
+			if n_ind not in opt_group:
+				opt_group[n_ind] = n_ind
+
+	# Build group_list.
+	group_list = []
+	for i in node_indices:
+		g = [n_ind for n_ind in node_indices if opt_group[n_ind] == i]
+		if g:
+			group_list.append(g)
+
+	return opt_group, group_list
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stockpyl-0.1.0a0/stockpyl/supply_uncertainty.py` & `stockpyl-1.0.0/src/stockpyl/supply_uncertainty.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 # ===============================================================================
 # stockpyl - supply_uncertainty Module
 # -------------------------------------------------------------------------------
-# Version: 0.0.0
-# Updated: 01-31-2022
 # Author: Larry Snyder
 # License: GPLv3
 # ===============================================================================
 
-"""The :mod:`supply_uncertainty` module contains code for solving inventory
-problems with supply uncertainty.
+"""
+.. include:: ../../globals.inc
 
-The notation and references (equations, sections, examples, etc.) used below
-refer to Snyder and Shen, *Fundamentals of Supply Chain Theory*, 2nd edition
-(2019).
+Overview 
+--------
 
-"""
+|sp| contains code to solve the following types of single-echelon inventory optimization problems
+in the |mod_supply_uncertainty| module:
+
+* Economic order quantity (EOQ)-based models
+	- with disruptions
+	- with yield uncertainty
+* Newsvendor-based models
+	- with disruptions
+	- with yield uncertainty
+
+.. note:: |fosct_notation|
+
+.. seealso::
+
+	For an overview of supply uncertainty in |sp|,
+	see the :ref:`tutorial page for supply uncertainty<tutorial_su_page>`.
 
-# TODO: add Dada
 
-from multiprocessing.sharedctypes import Value
+
+API Reference
+-------------
+
+"""
+
 import numpy as np
 from math import log
 from scipy.stats import *
 
 from stockpyl.optimization import golden_section_search
 from stockpyl.loss_functions import *
 from stockpyl.helpers import is_discrete_distribution
@@ -105,15 +121,15 @@
 	----------
 	M. Parlar and D. Berkin. Future supply uncertainty in EOQ models. *Naval Research Logistics*, 38 (1):107–121, 1991.
 
 	E. Berk and A. Arreola-Risa. Note on “Future supply uncertainty in EOQ models”. *Naval Research Logistics*, 41(1):129–132, 1994.
 
 	L. V. Snyder. A tight approximation for a continuousreview inventory model with supplier disruptions. *International Journal of Production Economics*, 155:91–108, 2014.
 
-	**Example** (Example 3.1):
+	**Example** (Example 9.1-9.2):
 
 	.. testsetup:: *
 
 		from stockpyl.supply_uncertainty import *
 
 	.. doctest::
 
@@ -134,15 +150,15 @@
 	if recovery_rate <= 0: raise ValueError("recovery_rate must be positive")
 
 	# Calculate approximate order quantity. Even if exact order quantity is
 	# requested, approximate quantity will be used for search bounds.
 	psi_approx = (disruption_rate / (disruption_rate + recovery_rate))
 
 	# Calculate approximate Q^*.
-	order_quantity_approx = (np.sqrt((psi_approx * demand_rate * holding_cost) ** 2 + 2 * holding_cost * recovery_rate * (
+	order_quantity_approx = (math.sqrt((psi_approx * demand_rate * holding_cost) ** 2 + 2 * holding_cost * recovery_rate * (
 				fixed_cost * demand_rate * recovery_rate + demand_rate ** 2 * stockout_cost * psi_approx)) - psi_approx * demand_rate * holding_cost) / (
 								 holding_cost * recovery_rate)
 
 	# Approximate?
 	if approximate:
 
 		# Set Q.
@@ -464,15 +480,15 @@
 	if fixed_cost < 0: raise ValueError("fixed_cost must be non-negative")
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if demand_rate < 0: raise ValueError("demand_rate must be non-negative")
 	if yield_sd < 0: raise ValueError("yield_sd must be non-negative")
 
 	# Is Q provided?
 	if order_quantity is None:
-		order_quantity = np.sqrt((2 * fixed_cost * demand_rate / holding_cost) + yield_sd**2) - yield_mean
+		order_quantity = math.sqrt((2 * fixed_cost * demand_rate / holding_cost) + yield_sd**2) - yield_mean
 
 	# Calculate cost.
 	term1 = (2 * fixed_cost * demand_rate + holding_cost * yield_sd**2) / (2 * (order_quantity + yield_mean))
 	term2 = holding_cost * (order_quantity + yield_mean) / 2
 	cost = term1 + term2
 
 	return order_quantity, cost
@@ -523,37 +539,37 @@
 
 		Q^* = \\sqrt{\\frac{2Kd}{h(\\text{Var}[Z] + E[Z]^2)}}
 
 	.. math::
 
 		g(Q) = \\frac{Kd}{QE[Z]} + \\frac{hQ(\\text{Var}[Z] + E[Z]^2)}{2E[Z]}
 
-	**Example** (Example 9.4):
+	**Example** (Example 9.5):
 
 	.. testsetup:: *
 
 		from stockpyl.supply_uncertainty import *
 
 	.. doctest::
 
-		>>> eoq_with_multiplicative_yield_uncertainty(18500, 0.06, 75000, 0.8333, np.sqrt(0.0198))
+		>>> eoq_with_multiplicative_yield_uncertainty(18500, 0.06, 75000, 0.8333, math.sqrt(0.0198))
 		(254477.46130342316, 13086.16169098594)
-		>>> eoq_with_multiplicative_yield_uncertainty(18500, 0.06, 75000, 0.8333, np.sqrt(0.0198), order_quantity=300000)
+		>>> eoq_with_multiplicative_yield_uncertainty(18500, 0.06, 75000, 0.8333, math.sqrt(0.0198), order_quantity=300000)
 		(300000, 13263.770562822512)
 	"""
 
 	# Check parameters.
 	if fixed_cost < 0: raise ValueError("fixed_cost must be non-negative")
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if demand_rate < 0: raise ValueError("demand_rate must be non-negative")
 	if yield_sd < 0: raise ValueError("yield_sd must be non-negative")
 
 	# Is Q provided?
 	if order_quantity is None:
-		order_quantity = np.sqrt((2 * fixed_cost * demand_rate) / (holding_cost * (yield_sd**2 + yield_mean**2)))
+		order_quantity = math.sqrt((2 * fixed_cost * demand_rate) / (holding_cost * (yield_sd**2 + yield_mean**2)))
 
 	# Calculate cost.
 	term1 = fixed_cost * demand_rate / (order_quantity * yield_mean)
 	term2 = holding_cost * order_quantity * (yield_sd**2 + yield_mean**2) / (2 * yield_mean)
 	cost = term1 + term2
 
 	return order_quantity, cost
@@ -583,15 +599,15 @@
 	yield_mean : float, optional
 		Mean of yield distribution. [:math:`E[Y]`]
 	yield_sd : float, optional
 		Standard deviation of yield distribution. [:math:`\\text{SD}[Y]`]
 	yield_distribution : rv_continuous or rv_discrete, optional
 		Yield distribution. Required if ``yield_mean`` or ``yield_sd`` is ``None``.
 	loss_function : function, optional
-		Function that takes a single argument and returns the a tuple consisting
+		Function that takes a single argument and returns a tuple consisting
 		of the loss function and complementary loss function value of that argument.
 		Ignored if ``yield_distribution`` is ``None``.
 	base_stock_level : float, optional
 		Base-stock level for cost evaluation. If supplied, no
 		optimization will be performed. [:math:`S`]
 
 	Returns
@@ -616,15 +632,15 @@
 
 	.. math::
 
 		S^* = d - F_Y^{-1}\\left(\\frac{h}{h+p}\\right)
 
 	.. math::
 
-		g(S) = p\\bar{n}(S) + hn(S),
+		g(S) = p\\bar{n}(d-S) + hn(d-S),
 
 	where :math:`n(\\cdot)` and :math:`\\bar{n}(\\cdot)` are the loss function
 	and complementary loss function, respectively, of the yield distribution.
 
 	**Example** (Example 9.6):
 
 	.. testsetup:: *
@@ -649,15 +665,15 @@
 		(1833333.3333333335, 6250000.000000001)
 	"""
 
 	# Check parameters.
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if demand <= 0: raise ValueError("demand must be positive")
-	if yield_sd or 0 < 0: raise ValueError("yield_sd must be non-negative")
+	if (yield_sd or 0) < 0: raise ValueError("yield_sd must be non-negative")
 	if (yield_mean is None or yield_sd is None) and yield_distribution is None: \
 		raise ValueError("Must provide either yield_mean and yield_sd or yield_distribution")
 
 	# Is S provided?
 	if base_stock_level is None:
 		# Calculate critical ratio.
 		crit_ratio = holding_cost / (holding_cost + stockout_cost)
@@ -687,8 +703,7 @@
 					n, n_bar = continuous_loss(R, yield_distribution)
 
 	# Calculate cost.
 	cost = stockout_cost * n_bar + holding_cost * n
 
 	return base_stock_level, cost
 
-
```

### Comparing `stockpyl-0.1.0a0/stockpyl/ss.py` & `stockpyl-1.0.0/src/stockpyl/ss.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 # ===============================================================================
 # stockpyl - ss Module
 # -------------------------------------------------------------------------------
-# Version: 0.0.0
-# Updated: 01-30-2022
 # Author: Larry Snyder
 # License: GPLv3
 # ===============================================================================
 
-"""The :mod:`ss` module contains code for solving the :math:`(s,S)` problem.
+"""
+.. include:: ../../globals.inc
+
+Overview 
+--------
+
+The |mod_ss| module contains code for solving the |ss| optimization problem.
+
+.. note:: |fosct_notation|
+
+.. seealso::
+
+	For an overview of single-echelon inventory optimization in |sp|,
+	see the :ref:`tutorial page for single-echelon inventory optimization<tutorial_seio_page>`.
 
-The notation and references (equations, sections, examples, etc.) used below
-refer to Snyder and Shen, *Fundamentals of Supply Chain Theory*, 2nd edition
-(2019).
+
+API Reference
+-------------
 
 """
 
 from scipy import integrate
 from scipy.stats import norm
 from scipy.stats import poisson
 from scipy.optimize import fsolve
@@ -24,33 +35,33 @@
 from stockpyl.eoq import *
 #import stockpyl.loss_functions as lf
 
 
 def s_s_cost_discrete(reorder_point, order_up_to_level, holding_cost,
 					  stockout_cost, fixed_cost, use_poisson, demand_mean=None,
 					  demand_hi=None, demand_pmf=None):
-	"""Calculate the exact cost of the given solution for an :math:`(s,S)`
+	"""Calculate the exact cost of the given solution for an |ss|
 	policy with given parameters under a discrete (Poisson or custom) demand
 	distribution.
 
-	Uses method described in Zheng and Federgruen (1991).
+	Uses method introduced in Zheng and Federgruen (1991).
 
 	Parameters
 	----------
 	reorder_point : float
 		Reorder point. [:math:`s`]
 	order_up_to_level : float
 		Order-up-to level. [:math:`S`]
 	holding_cost : float
 		Holding cost per item per period. [:math:`h`]
 	stockout_cost : float
 		Stockout cost per item per period. [:math:`p`]
 	fixed_cost : float
 		Fixed cost per order. [:math:`K`]
-	poisson_dist : bool
+	use_poisson : bool
 		Set to ``True`` to use Poisson distribution, ``False`` to use custom
 		discrete distribution. If ``True``, then ``mean`` must be
 		provided; if ``False``, then ``hi`` and ``demand_pdf`` must
 		be provied.
 	demand_mean : float, optional
 		Mean demand per period. Required if ``use_poisson`` is ``True``,
 		ignored otherwise. [:math:`\\mu`]
@@ -83,29 +94,34 @@
 	.. math::
 
 		g(s,S) = \\frac{K + \\sum_{d=0}^{S-s-1} m(d)g(S-d)}{M(S-s)},
 
 	where :math:`g(\cdot)` is the newsvendor cost function and :math:`M(\\cdot)`
 	and :math:`m(\\cdot)` are as described in equations (4.71)--(4.75).
 
+
+	References
+	----------
+	Y.-S. Zheng and A. Federgruen, Finding Optimal |ss| Policies is About as Simple
+	as Evaluating a Single Policy, *Operations Research* 39(4), 654-665 (1991).
+
+
 	**Example** (Example 4.7):
 
 	.. testsetup:: *
 
 		from stockpyl.ss import *
 
 	.. doctest::
 
 		>>> s_s_cost_discrete(4, 10, 1, 4, 5, True, 6)
 		8.034111561471642
 
 	"""
 
-	# TODO: improve performance
-
 	# Check parameters.
 	if not is_integer(reorder_point): raise ValueError("reorder_point must be an integer")
 	if not is_integer(order_up_to_level): raise ValueError("order_up_to_level must be an integer")
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if fixed_cost <= 0: raise ValueError("fixed_cost must be positive")
 	if demand_mean is not None and demand_mean < 0: raise ValueError("demand_mean must be non-negative (or None)")
@@ -154,40 +170,40 @@
 	cost /= M[int(order_up_to_level)-int(reorder_point)]
 
 	return cost
 
 
 def s_s_discrete_exact(holding_cost, stockout_cost, fixed_cost, use_poisson,
 					   demand_mean=None, demand_hi=None, demand_pmf=None):
-	"""Determine optimal :math:`s` and :math:`S` for an :math:`(s,S)`
+	"""Determine optimal :math:`s` and :math:`S` for an |ss|
 	policy under a discrete (Poisson or custom) demand distribution.
 
-	Uses method described in Zheng and Federgruen (1991).
+	Uses method introduced in Zheng and Federgruen (1991).
 
 	Parameters
 	----------
 	holding_cost : float
 		Holding cost per item per period. [:math:`h`]
 	stockout_cost : float
 		Stockout cost per item per period. [:math:`p`]
 	fixed_cost : float
 		Fixed cost per order. [:math:`K`]
-	poisson_dist : bool
+	use_poisson : bool
 		Set to ``True`` to use Poisson distribution, ``False`` to use custom
-		discrete distribution. If ``True``, then ``mean`` must be
-		provided; if ``False``, then ``hi`` and ``demand_pdf`` must
+		discrete distribution. If ``True``, then ``demand_mean`` must be
+		provided; if ``False``, then ``demand_hi`` and ``demand_pdf`` must
 		be provied.
 	demand_mean : float, optional
 		Mean demand per period. Required if ``use_poisson`` is ``True``,
 		ignored otherwise. [:math:`\\mu`]
 	demand_hi : int, optional
 		Upper limit of support of demand per period (lower limit is assumed to
 		be 0). Required if ``use_poisson`` is ``False``, ignored otherwise.
 	demand_pmf : list, optional
-		List of pmf values for demand values 0, ..., ``hi``. Required
+		List of pmf values for demand values 0, ..., ``demand_hi``. Required
 		if ``use_poisson`` is ``False``, ignored otherwise.
 
 	Returns
 	-------
 	reorder_point : float
 		Reorder point. [:math:`s`]
 	order_up_to_level : float
@@ -201,32 +217,37 @@
 		If ``holding_cost``, ``stockout_cost``, or ``fixed_cost`` <= 0.
 	ValueError
 		If ``demand_mean`` < 0, or if ``demand_hi`` is not a non-negative integer.
 	ValueError
 		If ``demand_pmf`` is not a list of length ``demand_hi`` + 1.
 
 
-	**Algorithm Used:** Exact algorithm for periodic-review :math:`(s,S)`
+	**Algorithm Used:** Exact algorithm for periodic-review |ss|
 	policies with discrete demand distribution (Algorithm 4.2)
 
+
+	References
+	----------
+	Y.-S. Zheng and A. Federgruen, Finding Optimal |ss| Policies is About as Simple
+	as Evaluating a Single Policy, *Operations Research* 39(4), 654-665 (1991).
+
+
 	**Example** (Example 4.7):
 
 	.. testsetup:: *
 
 		from stockpyl.ss import *
 
 	.. doctest::
 
 		>>> s_s_discrete_exact(1, 4, 5, True, 6)
 		(4.0, 10.0, 8.034111561471642)
 
 	"""
 
-	# TODO: improve performance
-
 	# Check parameters.
 	if holding_cost <= 0: raise ValueError("holding_cost must be positive")
 	if stockout_cost <= 0: raise ValueError("stockout_cost must be positive")
 	if fixed_cost <= 0: raise ValueError("fixed_cost must be positive")
 	if demand_mean is not None and demand_mean < 0: raise ValueError("demand_mean must be non-negative (or None)")
 	if demand_hi is not None and (demand_hi < 0 or not is_integer(demand_hi)):
 		raise ValueError("demand_hi must be a non-negative integer (or None)")
@@ -250,15 +271,14 @@
 	# Find s(S0).
 	done = False
 	while not done:
 		s -= 1
 		if use_poisson:
 			gs = newsvendor_poisson_cost(s, holding_cost, stockout_cost, demand_mean)
 		else:
-			# TODO: build newsvendor_discrete_cost function
 			gs = newsvendor_discrete(holding_cost, stockout_cost,
 									 demand_pmf=demand_pmf_dict,
 									 base_stock_level=s)[1]
 		gsS0 = s_s_cost_discrete(s, S0, holding_cost, stockout_cost, fixed_cost,
 							 use_poisson, demand_mean, demand_hi, demand_pmf)
 		if gsS0 <= gs:
 			done = True
@@ -266,16 +286,16 @@
 	# Set s0.
 	s0 = s
 
 	# Initialize incumbent and cost.
 	S_hat = S0
 	s_hat = s0
 	g_hat = s_s_cost_discrete(s_hat, S_hat, holding_cost, stockout_cost,
-							  fixed_cost, use_poisson, demand_mean,
-							  demand_pmf_dict)
+							  fixed_cost, use_poisson, demand_mean, demand_hi,
+							  demand_pmf)
 
 	# Choose next order-up-to level to consider.
 	S = S_hat + 1
 
 	# Loop through S values.
 	if use_poisson:
 		gS = newsvendor_poisson_cost(S, holding_cost, stockout_cost, demand_mean)
@@ -332,17 +352,19 @@
 	g = g_hat
 
 	return s, S, g
 
 
 def s_s_power_approximation(holding_cost, stockout_cost, fixed_cost,
 					   demand_mean, demand_sd):
-	"""Determine heuristic :math:`s` and :math:`S` for an :math:`(s,S)`
+	"""Determine heuristic :math:`s` and :math:`S` for an |ss|
 	policy under a normal demand distribution.
 
+	Uses the power approximation by Ehrhardt and Mosier (1984).
+
 	Parameters
 	----------
 	holding_cost : float
 		Holding cost per item per period. [:math:`h`]
 	stockout_cost : float
 		Stockout cost per item per period. [:math:`p`]
 	fixed_cost : float
@@ -366,15 +388,15 @@
 	ValueError
 		If ``demand_mean`` or ``demand_sd`` < 0.
 
 
 	References
 	----------
 	R. Ehrhardt and C. Mosier, A Revision of the Power Approximation for
-	Computing :math:`(s, S)` Policies, *Management Science* 30, 618-622 (1984).
+	Computing |ss| Policies, *Management Science* 30, 618-622 (1984).
 
 
 	**Equations Used** (equations (4.77)-(4.80)):
 
 	.. math::
 
 		Q  = 1.30 \\mu^{0.494} \\left(\\frac{K}{h}\\right)^{0.506} \\left(1 + \\frac{\\sigma_L^2}{\\mu^2}\\right)^{
@@ -408,14 +430,14 @@
 	if fixed_cost <= 0: raise ValueError("fixed_cost must be positive")
 	if demand_mean < 0: raise ValueError("mean must be non-negative")
 	if demand_sd < 0: raise ValueError("demand_sd must be non-negative")
 
 	# Calculate Q and z.
 	Q = 1.30 * (demand_mean**0.494) * (fixed_cost / holding_cost)**0.506 \
 		* (1 + (demand_sd / demand_mean)**2)**0.116
-	z = np.sqrt((Q / demand_sd) * (holding_cost / stockout_cost))
+	z = math.sqrt((Q / demand_sd) * (holding_cost / stockout_cost))
 
 	# Calculate s and S.
 	s = 0.973 * demand_mean + demand_sd * ((0.183 / z) + 1.063 - 2.192*z)
 	S = s + Q
 
 	return s, S
```

### Comparing `stockpyl-0.1.0a0/stockpyl/eoq.py` & `stockpyl-1.0.0/src/stockpyl/eoq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 # ===============================================================================
 # stockpyl - eoq Module
 # -------------------------------------------------------------------------------
-# Version: 0.0.0
-# Updated: 01-30-2022
 # Author: Larry Snyder
 # License: GPLv3
 # ===============================================================================
 
-"""The :mod:`eoq` module contains code for solving the economic order quantity
+"""
+.. include:: ../../globals.inc
+
+Overview 
+--------
+
+The |mod_eoq| module contains code for solving the economic order quantity
 (EOQ) problem and some of its variants.
 
-The notation and references (equations, sections, examples, etc.) used below
-refer to Snyder and Shen, *Fundamentals of Supply Chain Theory*, 2nd edition
-(2019).
+.. note:: |fosct_notation|
+
+.. seealso::
+
+	For an overview of single-echelon inventory optimization in |sp|,
+	see the :ref:`tutorial page for single-echelon inventory optimization<tutorial_seio_page>`.
+
 
+API Reference
+-------------
 """
 
 import numpy as np
+import math
 
 
 def economic_order_quantity(fixed_cost, holding_cost, demand_rate, order_quantity=None):
 	"""Solve the economic order quantity (EOQ) problem, or (if
 	``order_quantity`` is supplied) calculate cost of given solution.
 
 	Parameters
@@ -75,15 +86,15 @@
 	if holding_cost <= 0: raise ValueError( "holding_cost must be positive.")
 	if demand_rate < 0: raise ValueError( "demand_rate must be non-negative.")
 	if order_quantity is not None and order_quantity <= 0: raise ValueError("order_quantity must be positive.")
 
 	# Is Q provided?
 	if order_quantity is None:
 		# Calculate optimal order quantity and cost.
-		order_quantity = np.sqrt(2 * fixed_cost * demand_rate / holding_cost)
+		order_quantity = math.sqrt(2 * fixed_cost * demand_rate / holding_cost)
 		cost = order_quantity * holding_cost
 	else:
 		# Calculate cost.
 		cost = fixed_cost * demand_rate / order_quantity + holding_cost * order_quantity / 2
 
 	return order_quantity, cost
 
@@ -157,15 +168,15 @@
 
 	# Check that both or neither order_quantity and stockout_fraction are  provided.
 	if (order_quantity is None and stockout_fraction is not None) or (order_quantity is not None and stockout_fraction is None): raise ValueError("You must provide both order_quantity and stockout_fraction or neither.")
 
 	# Is Q provided?
 	if order_quantity is None:
 		# Calculate optimal order quantity, stockout fraction, and cost.
-		order_quantity = np.sqrt(2 * fixed_cost * demand_rate * (holding_cost + stockout_cost)
+		order_quantity = math.sqrt(2 * fixed_cost * demand_rate * (holding_cost + stockout_cost)
 									/ (holding_cost * stockout_cost))
 		stockout_fraction = holding_cost / (holding_cost + stockout_cost)
 		cost = order_quantity * (holding_cost * stockout_cost) / (holding_cost + stockout_cost)
 	else:
 		# Caclulate cost.
 		cost = holding_cost * order_quantity * (1 - stockout_fraction) ** 2 / 2 \
 			+ stockout_cost * order_quantity * stockout_fraction ** 2 / 2 \
@@ -239,15 +250,15 @@
 
 	# Calculate rho.
 	rho = demand_rate / production_rate
 
 	# Is Q provided?
 	if order_quantity is None:
 		# Calculate optimal order quantity and cost.
-		order_quantity = np.sqrt(
+		order_quantity = math.sqrt(
 			2 * fixed_cost * demand_rate / (holding_cost * (1 - rho)))
 		cost = order_quantity * holding_cost * (1 - rho)
 	else:
 		# Calculate cost.
 		cost = fixed_cost * demand_rate / order_quantity + holding_cost * (1 - rho) * order_quantity / 2
 
 	return order_quantity, cost
@@ -337,27 +348,27 @@
 	# Calculate order frequencies.
 	order_multiples = []
 	for n in range(num_prod):
 
 		if n == min_ratio_prod:
 			m = 1
 		else:
-			m = np.sqrt((individual_fixed_costs[n] / (holding_costs[n] * demand_rates[n])) * const)
+			m = math.sqrt((individual_fixed_costs[n] / (holding_costs[n] * demand_rates[n])) * const)
 			m = max(1, int(round(m)))
 
 		order_multiples.append(m)
 
 	# Calculate a few terms we'll need below.
-	term1 = shared_fixed_cost + np.sum(np.divide(individual_fixed_costs, order_multiples))
-	term2 = np.sum([holding_costs[n] * order_multiples[n] * demand_rates[n] for n in range(num_prod)])
+	term1 = shared_fixed_cost + float(np.sum(np.divide(individual_fixed_costs, order_multiples)))
+	term2 = float(np.sum([holding_costs[n] * order_multiples[n] * demand_rates[n] for n in range(num_prod)]))
 
 	# Calculate base cycle time.
 	numer = 2 * term1
 	denom = term2
-	base_cycle_time = np.sqrt(numer / denom)
+	base_cycle_time = math.sqrt(numer / denom)
 
 	# Calculate order quantities.
 	order_quantities = [base_cycle_time * order_multiples[n] * demand_rates[n] for n in range(num_prod)]
 
 	# Calculate average cost.
 	avg_fixed_cost = term1 / base_cycle_time
 	avg_holding_cost = (base_cycle_time / 2) * term2
```

### Comparing `stockpyl-0.1.0a0/stockpyl/helpers.py` & `stockpyl-1.0.0/src/stockpyl/demand_source.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,759 +1,730 @@
-"""Helper functions for stockpyl package.
-
-(c) Lawrence V. Snyder
-Lehigh University
+# ===============================================================================
+# stockpyl - DemandSource Class
+# -------------------------------------------------------------------------------
+# Author: Larry Snyder
+# License: GPLv3
+# ===============================================================================
 
 """
+.. include:: ../../globals.inc
 
-import math
-from scipy import stats
-from scipy.special import comb
-from scipy.stats import uniform
-from scipy.stats import rv_discrete, rv_continuous
-from math import factorial
-import numpy as np
-
-#from datatypes import *
-
-
-### CONSTANTS ###
-
-BIG_INT = 1e100
-BIG_FLOAT = 1.0e100
+Overview 
+--------
 
+This module contains the |class_demand_source| class. A |class_demand_source|
+object represents external demand observed by a node.
+The demand can be random or deterministic. Attributes specify the type of demand
+distribution and its parameters. The object can generate demands from the specified distribution.
 
-### UTILITY FUNCTIONS ###
+.. note:: |fosct_notation|
 
-def min_of_dict(d):
-	"""Determine min value of dict and return min and argmin (key).
+**Example:** Create a |class_demand_source| object representing demand that has a normal
+distribution with a mean of 50 and a standard deviation of 10. Generate a random demand from the distribution.
 
-	Values must be numeric.
-
-	Parameters
-	----------
-	d : dict
-		The dict.
-
-	Returns
-	-------
-	min_value : float
-		Minimum value in dict.
-	min_key
-		Key that attains minimum value.
-
-	Raises
-	------
-	TypeError
-		If dict contains a non-numeric value.
-	"""
-	min_key = min(d, key=d.get)
-	min_value = d[min_key]
+	.. testsetup:: *
 
-	return min_value, min_key
+		from stockpyl.demand_source import *
 
+	.. doctest::
 
-def dict_match(d1, d2, require_presence=False, rel_tol=1e-9, abs_tol=0.0):
-	"""Check whether two dicts have equal keys and values.
+		>>> ds = DemandSource(type='N', mean=50, standard_deviation=10)
+		>>> ds.generate_demand()	# doctest: +SKIP
+		46.75370030596123
+		>>> # Tell object to round demands to integers.
+		>>> ds.round_to_int = True
+		>>> ds.generate_demand()	# doctest: +SKIP
+		63
 
-	A missing key is treated as 0 if the key is present in the other dict,
-	unless require_presence is True, in which case the dict must have the
-	key to count as a match.
+API Reference
+-------------
 
-	Parameters
-	----------
-	d1 : node
-		First dict for comparison.
-	d2 : node
-		Second dict for comparison.
-	require_presence : bool, optional
-		Set to True to require dicts to have the same keys, or False
-		(default) to treat missing keys as 0s.
-	rel_tol : float
-		Relative tolerance.
-	abs_tol : float
-		Absolute tolerance.
-	"""
+"""
 
-	match = True
 
-	# Check d1 against d2.
-	for key in d1.keys():
-		if key in d2:
-			if not math.isclose(d1[key], d2[key], rel_tol=rel_tol, abs_tol=abs_tol):
-				match = False
-		else:
-			if not math.isclose(d1[key], 0, rel_tol=rel_tol, abs_tol=abs_tol) \
-					or require_presence:
-				match = False
-
-	# Check d2 against d1.
-	for key in d2.keys():
-		if key in d2:
-			# We already checked in this case.
-			pass
-		else:
-			if not math.isclose(d2[key], 0, rel_tol=rel_tol, abs_tol=abs_tol) \
-					or require_presence:
-				match = False
+# ===============================================================================
+# Imports
+# ===============================================================================
 
-	return match
+import numpy as np
+import scipy.stats 
 
+from stockpyl.helpers import *
 
-def is_iterable(x):
-	"""Determine whether x is an iterable or a singleton.
+# ===============================================================================
+# DemandSource Class
+# ===============================================================================
+
+ALLOWABLE_TYPES = ('N', 'P', 'UD', 'UC', 'NB', 'D', 'CD', None)
+class DemandSource(object):
+	"""
+	A |class_demand_source| object represents external demand observed by a node.
+	The demand can be random or deterministic. Attributes specify the type of demand
+	distribution and its parameters. The object can generate demands from the specified distribution.
 
 	Parameters
 	----------
-	x
-		Object to test for iterable vs. singleton.
+	**kwargs 
+		Keyword arguments specifying values of one or more attributes of the |class_demand_source|, 
+		e.g., ``type='N'``.
+
+	Attributes
+	----------
+	type : str
+		The demand type, as a string. Currently supported strings are:
+
+			* None
+			* 'N' (normal)
+			* 'P' (Poisson)
+			* 'UD' (uniform discrete)
+			* 'UC' (uniform continuous)
+			* 'NB' (negative binomial)
+			* 'D' (deterministic)
+			* 'CD' (custom discrete)
+			
+	round_to_int : bool
+		Round demand to nearest integer?
+	demand_list : list, optional
+		List of demands, one per period (for deterministic demand types), or list
+		of possible demand values (for custom discrete demand types). For deterministic
+		demand types, if demand is required in a period beyond the length of the list,
+		the list is restarted at the beginning. This also allows ``demand_list`` to be
+		a singleton, in which case it is used in every period.
+		Required if ``type`` == 'D' or 'CD'. [:math:`d`]
+	probabilities : list, optional
+		List of probabilities of each demand value (for custom discrete demand types).
+		Required if ``type`` == 'CD'.
+	lo : float, optional
+		Low value of demand range (for uniform demand types). Required if
+		``type`` == 'UD' or 'UC'.
+	hi : float, optional
+		High value of demand range (for uniform demand types). Required if
+		``type`` == 'UD' or 'UC'.
+	n : int, optional
+		Parameter for negative binomial distribution indicating number of trial successes. 
+		Required if ``type`` == 'NB'. [:math:`n`]
+	p : float, optional
+		Parameter for negative binomial distribution indicating probability of success for each trial. 
+		Required if ``type`` == 'NB'. [:math:`p`]
+	"""
+
+	def __init__(self, **kwargs):
+		"""DemandSource constructor method.
+
+		Parameters
+		----------
+		kwargs : optional
+			Optional keyword arguments to specify |class_demand_source| attributes.
+
+		Raises
+		------
+		AttributeError
+			If an optional keyword argument does not match class_demand_source| attribute.
+		"""
+		# Initialize parameters.
+		self.initialize()
+
+		# Set attributes specified by kwargs.
+		for key, value in kwargs.items():
+			if key in vars(self):
+				vars(self)[key] = value
+			elif f"_{key}" in vars(self):
+				vars(self)[f"_{key}"] = value
+			else:
+				raise AttributeError(f"{key} is not an attribute of DemandSource")
 
-	Returns
-	-------
-	True if x is iterable, False if it is a singleton.
+	_DEFAULT_VALUES = {
+		'_type': None,
+		'_mean': None,
+		'_standard_deviation': None,
+		'_demand_list': None,
+		'_probabilities': None,
+		'_lo': None,
+		'_hi': None,
+		'_n': None,
+		'_p': None,
+		'_round_to_int': None
+	}
+
+	# SPECIAL METHODS
+
+	def __eq__(self, other):
+		"""Determine whether ``other`` is equal to this demand source object. 
+		Two demand source objects are considered equal if all of their attributes 
+		are equal.
+
+		Parameters
+		----------
+		other : |class_demand_source|
+			The demand source object to compare to.
+
+		Returns
+		-------
+		bool
+			True if the demand source objects are equal, False otherwise.
 
-	"""
-	# First check whether x is a string (because strings act like iterables).
-	if isinstance(x, str):
-		return False
-	else:
-		try:
-			_ = iter(x)
-	#		_ = (y for y in x)
-		except TypeError:
+		"""
+		if other is None:
 			return False
 		else:
+			for attr in self._DEFAULT_VALUES.keys():
+				if getattr(self, attr) != getattr(other, attr):
+					return False
 			return True
 
-
-def is_list(x):
-	"""Determine whether x is a list.
-
-	Parameters
-	----------
-	x
-		Object to test for list-ness.
-
-	Returns
-	-------
-	True if x is a list, False otherwise.
-
-	"""
-	return isinstance(x, list)
-
-
-def is_integer(x):
-	"""Determine whether x is an integer. Return False if x is not a float,
-	or is a non-integer float, or is an int.
-
-	Parameters
-	----------
-	x : float
-		Number to check for integrality.
-
-	Returns
-	-------
-	is_int : bool
-		True if x is an integer, False otherwise.
-
-	"""
-	# Check whether x is an int.
-	if isinstance(x, int):
-		return True
-	# Check whether x is a float.
-	elif isinstance(x, float):
-		# Check whether x is an integer.
-		if x.is_integer():
-			return True
+	def __ne__(self, other):
+		"""Determine whether ``other`` is not equal to this demand source object. 
+		Two demand source objects are considered equal if all of their attributes 
+		are equal.
+
+		Parameters
+		----------
+		other : |class_demand_source|
+			The demand source object to compare to.
+
+		Returns
+		-------
+		bool
+			True if the demand source objects are not equal, False otherwise.
+		"""
+		return not self.__eq__(other)
+
+	# PROPERTY GETTERS AND SETTERS
+
+	@property
+	def type(self):
+		return self._type
+
+	@type.setter
+	def type(self, value):
+		self._type = value
+
+	@property
+	def mean(self):
+		"""Return mean set by user, if any; or, for distributions whose mean is not
+		set but is calculated from other parameters, returns the calculated mean.
+		If neither is true, return ``None``.
+		"""
+		if self._mean is not None:
+			return self._mean
+		elif self.type in ('UC', 'UD', 'NB', 'CD'):
+			return self.demand_distribution.mean()
 		else:
-			return False
-	else:
-		return False
+			return None
 
-
-def is_discrete_distribution(distribution):
-	"""Check whether the given distribution object is discrete.
-
-	Works both for ``rv_frozen`` objects (i.e., `frozen distributions
-	<https://docs.scipy.org/doc/scipy/reference/tutorial/stats.html#freezing-a
-	-distribution>`_) and for custom distribution (i.e., subclasses of
-	``rv_continuous`` and ``rv_discrete``).
-
-	See https://stackoverflow.com/a/61530461/3453768.
-
-	Parameters
-	----------
-	distribution : rv_frozen, rv_continuous, or rv_discrete
-		The distribution object to check.
-
-	Returns
-	-------
-	``True`` if the distribution is discrete, ``False`` otherwise.
-
-	Notes
-	-----
-	Not reliable if ``distribution`` is not an ``rv_frozen``, ``rv_discrete``,
-	or ``rv_continuous`` object.
-
-	"""
-	# First check whether distribution is a frozen distribution (in which case
-	# it has a .dist attribute which must be checked).
-	if hasattr(distribution, 'dist'):
-		# Check .dist attribute to determine type.
-		return isinstance(distribution.dist, rv_discrete)
-	else:
-		# Check the object itself for type.
-		return isinstance(distribution, rv_discrete)
-
-
-def is_continuous_distribution(distribution):
-	"""Check whether the given distribution object is continuous.
-
-	Works both for ``rv_frozen`` objects (i.e., `frozen distributions
-	<https://docs.scipy.org/doc/scipy/reference/tutorial/stats.html#freezing-a
-	-distribution>`_) and for custom distribution (i.e., subclasses of
-	``rv_continuous`` and ``rv_discrete``).
-
-	See https://stackoverflow.com/a/61530461/3453768.
-
-	Parameters
-	----------
-	distribution : rv_frozen, rv_continuous, or rv_discrete
-		The distribution object to check.
-
-	Returns
-	-------
-	``True`` if the distribution is continuous, ``False`` otherwise.
-
-	Notes
-	-----
-	Not reliable if ``distribution`` is not an ``rv_frozen``, ``rv_discrete``,
-	or ``rv_continuous`` object.
-
-	"""
-	# First check whether distribution is a frozen distribution (in which case
-	# it has a .dist attribute which must be checked).
-	if hasattr(distribution, 'dist'):
-		# Check .dist attribute to determine type.
-		return isinstance(distribution.dist, rv_continuous)
-	else:
-		# Check the object itself for type.
-		return isinstance(distribution, rv_continuous)
-
-
-def find_nearest(array, values, sorted=False):
-	"""Determine entries in ``array` that are closest to each of the
-	entries in ``values`` and return their indices. Neither array needs to be sorted,
-	but if ``array`` is sorted and ``sorted`` is set to ``True``, execution will be faster.
-	``array`` and ``values`` need not be the same length.
-
-	Parameters
-	----------
-	array : ndarray
-		The array to search for values in.
-	values : ndarray
-		The array whose values should be searched for in the other array.
-	sorted : Boolean
-		If ``True``, treats array as sorted, which will make the function execute
-		faster.
-
-	Returns
-	-------
-	ind : ndarray
-		Array of indices.
-	"""
-	array = np.asarray(array)
-	values = np.array(values, ndmin=1, copy=False)
-	ind = np.zeros(values.shape)
-	for v in range(values.size):
-		if sorted:
-			# https://stackoverflow.com/a/26026189/3453768
-			idx = np.searchsorted(array, values[v], side="left")
-			if idx > 0 and (idx == len(array) or math.fabs(values[v] - array[idx-1])
-					< math.fabs(values[v] - array[idx])):
-				ind[v] = idx-1
-			else:
-				ind[v] = idx
+	@mean.setter
+	def mean(self, value):
+		self._mean = value
+
+	@property
+	def standard_deviation(self):
+		"""Return standard deviation set by user, if any; or, for distributions whose standard deviation is not
+		set but is calculated from other parameters, returns the calculated standard deviation.
+		If neither is true, return ``None``.
+		"""
+		if self._standard_deviation is not None:
+			return self._standard_deviation
+		elif self.type in ('P', 'UC', 'UD', 'NB', 'CD'):
+			return self.demand_distribution.std()
 		else:
-			# https://stackoverflow.com/a/2566508/3453768
-			idx = (np.abs(array - values[v])).argmin()
-			ind[v] = idx
-
-	return ind.astype(int)
-
-
-### LIST-HANDLING FUNCTIONS ###
-
-def check_iterable_sizes(iterable_list):
-	"""Check whether `iterable_list` is a list in which every item is an iterable of the
-	same size _or_ a singleton.
-
-	Examples:
-		- ensure_iterable_sizes([[5, 3, 1], ('a', 'b', 'c'), 7]) returns True
-		- ensure_iterable_sizes([[5, 3, 1], ('a, 'b'), 7]) returns False
-
-	Parameters
-	----------
-	iterable_list : list
-		List to check.
+			return None
 
-	Returns
-	-------
-	True if `iterable_list` is a list in which every item is an iterable of the
-	same size _or_ a singleton, False otherwise.
-	"""
-	# Build set of lengths of items in list, excluding singletons.
-	lengths = {len(i) for i in iterable_list if is_iterable(i) and len(i) != 1}
-
-	# Check whether lengths contains at most one element.
-	return len(lengths) <= 1
-
-
-def ensure_list_for_time_periods(x, num_periods, var_name=None):
-	"""Ensure that `x` is a list suitable for time-period indexing; if not, create
-	such a list and return it.
-
-	"Suitable for time-period indexing" means that it has length num_periods+1,
-	and element [0] is ignored.
-
-	If x is a singleton, return a list consisting of `num_periods` copies of x.
-	If x is a list of length `num_periods`, return x.
-	If x is a list of length `num_periods`-1, shift elements to the right by 1 slot,
-		fill [0] element with 0, and return new list.
-	Otherwise, raise a ValueError.
-
-	Examples:
-		- ensure_list_for_time_periods(5, 3) returns [5, 5, 5]
-		- ensure_list_for_time_periods([0, 5, 2, 1], 4) returns [0, 5, 2, 1]
-		- ensure_list_for_time_periods([5, 2, 1], 4) returns [0, 5, 2, 1]
-		- ensure_list_for_time_periods([0, 5, 2, 1], 3) raises a ValueError.
-
-	Parameters
-	----------
-	x : float or list
-		Object to time-period-ify.
-	num_periods : int
-		Number of time periods.
-	var_name : str, optional
-		Variable name to use in generating error messages, if desired.
-		Useful for offloading the type-checking to this function rather than
-		doing it in the calling function.
-
-	Returns
-	-------
-	x_new : list
-		Time-period-ified list.
-	"""
-	# Determine whether x is singleton or iterable.
-	if is_iterable(x):
-		if len(x) == num_periods+1:
-			return x
-		elif len(x) == num_periods:
-			return [0] + x
+	@standard_deviation.setter
+	def standard_deviation(self, value):
+		self._standard_deviation = value
+
+	@property
+	def demand_list(self):
+		return self._demand_list
+
+	@demand_list.setter
+	def demand_list(self, value):
+		self._demand_list = value
+
+	@property
+	def probabilities(self):
+		return self._probabilities
+
+	@probabilities.setter
+	def probabilities(self, value):
+		self._probabilities = value
+
+	@property
+	def lo(self):
+		return self._lo
+
+	@lo.setter
+	def lo(self, value):
+		self._lo = value
+
+	@property
+	def hi(self):
+		return self._hi
+
+	@hi.setter
+	def hi(self, value):
+		self._hi = value
+
+	@property
+	def n(self):
+		return self._n
+
+	@n.setter
+	def n(self, value):
+		self._n = value
+
+	@property
+	def p(self):
+		return self._p
+
+	@p.setter
+	def p(self, value):
+		self._p = value
+
+	@property
+	def round_to_int(self):
+		return self._round_to_int
+
+	@round_to_int.setter
+	def round_to_int(self, value):
+		self._round_to_int = value
+
+	# READ-ONLY PROPERTIES
+	@property
+	def demand_distribution(self):
+		"""Demand distribution, as a ``scipy.stats.rv_continuous`` or
+		``scipy.stats.rv_discrete`` object. Returns ``None`` if demand source ``type`` is ``'D'``.
+		Read only.
+		"""
+		# Check that the appropriate parameters have been set. If not, raise an exception.
+		self.validate_parameters()
+
+		if self.type is None:
+			distribution = None
+		elif self.type == 'N':
+			distribution = scipy.stats.norm(self.mean, self.standard_deviation)
+		elif self.type == 'P':
+			distribution = scipy.stats.poisson(self.mean)
+		elif self.type == 'UD':
+			distribution = scipy.stats.randint(self.lo, self.hi+1)
+		elif self.type == 'UC':
+			distribution = scipy.stats.uniform(self.lo, self.hi - self.lo)
+		elif self.type == 'NB':
+			distribution = scipy.stats.nbinom(self.n, self.p)
+		elif self.type == 'CD':
+			distribution = scipy.stats.rv_discrete(name='custom',
+												   values=(self.demand_list, self.probabilities))
 		else:
-			if var_name is None:
-				vname = 'x'
-			else:
-				vname = var_name
-			raise ValueError('{:s} must be a singleton or a list of length num_periods or num_periods+1'.format(vname))
-	else:
-		return [0] + [x] * num_periods
-
-
-def ensure_list_for_nodes(x, num_nodes, default=None):
-	"""Ensure that x is a list suitable for node indexing; if not, create
-	such a list and return it.
-
-	"Suitable for node indexing" means that it has length num_nodes.
-
-	If x is a singleton, return a list consisting of `num_nodes` copies of x.
-	If x is a list of length `num_nodes`, return x.
-	If x is None and `default` is provided, return a list consisting of
-		`num_nodes` copies of `default`.
-	If x is None and `default` is not provided, a list consisting of
-	 	`num_nodes` copies of None.
-	Otherwise, raise a ValueError.
-
-	Examples:
-		- ensure_list_for_nodes(5, 3) returns [5, 5, 5]
-		- ensure_list_for_nodes([0, 5, 2, 1], 4) returns [0, 5, 2, 1]
-		- ensure_list_for_nodes([0, 5, 2, 1], 3) raises a ValueError.
+			distribution = None
 
-	Parameters
-	----------
-	x : float or list
-		Object to node-ify.
-	num_nodes : int
-		Number of nodes.
-	default : float, optional
-		Value to use if x is None.
-
-	Returns
-	-------
-	x_new : list
-		Node-ified list.
-	"""
-	# Is x None?
-	if x is None:
-		return [default] * num_nodes
-	else:
-		# Determine whether x is singleton or iterable.
-		if is_iterable(x):
-			if len(list(x)) == num_nodes:
-				return list(x)
+		return distribution
+	
+	@property
+	def is_discrete(self):
+		"""``True`` if the distribution is discrete, ``False`` if it is continuous. Read only.
+
+		The distribution is discrete if ``self.type`` is 'P', 'UD', 'CD', 'NB', or 'D'.
+
+		Returns
+		-------
+		bool
+			``True`` if the distribution is discrete, ``False`` if it is continuous.
+		"""
+		return self.type in ('P', 'UD', 'CD', 'NB', 'D')
+	
+
+	# SPECIAL MEMBERS
+
+	def __repr__(self):
+		"""
+		Return a string representation of the |class_demand_source| instance.
+
+		Returns
+		-------
+			A string representation of the |class_demand_source| instance.
+
+		"""
+		# Build string of parameters.
+		if self.type is None:
+			return "DemandSource(None)"
+		elif self.type == 'N':
+			param_str = "mean={:.2f}, standard_deviation={:.2f}".format(
+				self.mean, self.standard_deviation)
+		elif self.type == 'P':
+			param_str = "mean={:.2f}".format(self.mean)
+		elif self.type in ('UD', 'UC'):
+			param_str = "lo={:.2f}, hi={:.2f}".format(
+				self.lo, self.hi)
+		elif self.type == 'D':
+			if not is_list(self.demand_list) or len(self.demand_list) <= 8:
+				param_str = "demand_list={}".format(self.demand_list)
 			else:
-				raise ValueError('x must be a singleton or a list of length num_nodes')
-		else:
-			return [x] * num_nodes
-
-
-def ensure_dict_for_nodes(x, node_indices, default=None):
-	"""Ensure that x is a dict suitable with node indices as keys(); if not, create
-	such a dict and return it.
-
-	If ``x`` is a dict, return ``x``.
-	If ``x`` is a singleton, return a dict with keys equal to ``node_indices``
-		and values all equal to ``x``.
-	If ``x`` is a list with the same length as ``node_indices``, return a dict
-		with keys equal to ``node_indices`` and values equal to ``x``.
-	If ``x`` is ``None`` and ``default`` is provided, return a dict with keys
-		equal to ``node_indices`` and values all equal to ``default``.
-	If ``x`` is ``None`` and ``default`` is not provided, return a dict with
-		keys equal to ``node_indices`` and values all equal to ``None``.
-	Otherwise, raise a ``ValueError``.
-
-	Examples:
-		- ensure_dict_for_nodes(5, [0, 1, 2]) returns {0: 5, 1: 5, 2:5}.
-		- ensure_dict_for_nodes([0, 5, 2], [0, 1, 2]) returns {0: 0, 1: 5, 2: 2}.
-		- ensure_list_for_nodes([0, 5, 2, 1], [0, 1, 2]) raises a ValueError.
-
-	Parameters
-	----------
-	x : dict, float, or list
-		Object to node-ify.
-	node_indices : list
-		List of node indices.
-	default : float, optional
-		Value to use if ``x`` is ``None``.
-
-	Returns
-	-------
-	x_new : dict
-		Node-ified dict.
-	"""
-	# Is x None?
-	if type(x) == dict:
-		return x
-	elif x is None:
-		return {n_ind: default for n_ind in node_indices}
-	else:
-		# Determine whether x is singleton or iterable.
-		if is_iterable(x):
-			if len(list(x)) == len(node_indices):
-				return {node_indices[i]: x[i] for i in range(len(x))}
+				param_str = "demand_list={}...".format(self.demand_list[0:8])
+		elif self.type == 'NB':
+			param_str = "n={:d}, p={:.2f}".format(self.n, self.p)
+		elif self.type == 'CD':
+			if len(self.demand_list) <= 8:
+				param_str = "demand_list={}, probabilities={}".format(
+					self.demand_list, self.probabilities)
 			else:
-				raise ValueError('x must be a singleton, dict, or list with the same length as node_indices')
+				param_str = "demand_list={}..., probabilities={}...".format(
+					self.demand_list[0:8], self.probabilities[0:8])
 		else:
-			return {node_indices[i]: x for i in range(len(node_indices))}
-
-
-def sort_dict_by_keys(d, ascending=True, return_values=True):
-	"""Sort dict by keys and return sorted list of values or keys, depending
-	on the value of ``return_values``.
-	Special handling is included to handle keys that might be ``None``.
-	(``None`` is assumed to come before any other element when sorting in
-	ascending order.)
-
-	Parameters
-	----------
-	d : dict
-		The dict to sort.
-	ascending : bool, optional
-		Sort order.
-	return_values : bool, optional
-		Set to ``True`` to return a list of the dict's values, ``False`` to
-		return its keys.
-
-	Returns
-	-------
-	return_list : list
-		List of values or keys of ``d``, sorted in order of keys of ``d``.
-
-	"""
-	# Create dict equal to d but without None key.
-	dict_without_none = {key: d[key] for key in d.keys() if key is not None}
-
-	if return_values:
-		# Build sorted list of values in dict_without_none.
-		return_list = [value for _, value in sorted(dict_without_none.items(), reverse=not ascending)]
-
-		# If original dict had None key, add it back.
-		if None in d.keys():
-			if ascending:
-				return_list.insert(0, d[None])
-			else:
-				return_list.append(d[None])
-	else:
-		# Build sorted list of keys in dict_without_none.
-		return_list = [key for key, _ in sorted(dict_without_none.items(), reverse=not ascending)]
-
-		# If original dict had None key, add it back.
-		if None in d.keys():
-			if ascending:
-				return_list.insert(0, None)
-			else:
-				return_list.append(None)
-
-	return return_list
-
-
-def change_dict_key(dict_to_change, old_key, new_key):
-	"""Change ``old_key`` to ``new_key`` in ``dict_to_change`` (in place).
-	New key/value pair will appear at end of dict.
-
-	Parameters
-	----------
-	dict_to_change : dict
-		The dict.
-	old_key :
-		The key to be changed.
-	new_key :
-		The key to change to.
-
-	Raises
-	------
-	KeyError : if dict_to_change[old_key] is undefined.
-	"""
-	# Change key.
-	# See https://stackoverflow.com/a/4406521/3453768.
-	dict_to_change[new_key] = dict_to_change.pop(old_key)
-
-
-### STATS FUNCTIONS ###
-
-def convolve_many(arrays):
-	"""Convolve a list of 1-dimensional float arrays together, using FFTs.
-	The arrays need not have the same length, but each array should
-	have length at least 1.
-
-	If the arrays represent pmfs of discrete random variables
-	:math:`X_1,\\ldots,X_n`, then the output represents the pmf of
-	:math:`X_1+\\cdots+X_n`. Assuming the possible values of all of the random
-	variables are equally spaced with spacing :math:`s`, the possible values of
-	:math:`X_1+\\cdots+X_n` corresponding to the output are
-	:math:`\\min_i\\{\\min X_i\\},\\ldots,\\sum_i \\max X_i`, with spacing :math:`s`.
-
-	Code is adapted from https://stackoverflow.com/a/29236193/3453768.
-
-	Parameters
-	----------
-	arrays : list of 1-dimensional float arrays
-		The arrays to convolve.
-
-	Returns
-	-------
-	convolution : array
-		Array of elements in the convolution.
-
-	**Example**
-	Let :math:`X_1 = \\{0, 1, 2\\}` with probabilities :math:`[0.6, 0.3, 0.1]`,
-	:math:`X_2 = \\{0, 1, 2\\}` with probabilities :math:`[0.5, 0.4, 0.1]`,
-	:math:`X_3 = \\{0, 1\\}` with probabilities :math:`[0.3, 0.7]`, and
-	:math:`X_4 = 0` with probability :math:`1`.
-
-	.. testsetup:: *
-
-		from stockpyl.helpers import *
-
-	.. doctest::
-
-		>>> convolve_many([[0.6, 0.3, 0.1], [0.5, 0.4, 0.1], [0.3, 0.7], [1.0]])
-		array([0.09 , 0.327, 0.342, 0.182, 0.052, 0.007])
-
-	In other words, :math:`X_1+\\cdots+X_4 = \\{0, 1, \\ldots, 5\\}`: with
-	probabilities :math:`[0.09 , 0.327, 0.342, 0.182, 0.052, 0.007]`.
-
-	"""
-	result_length = 1 + sum((len(a) - 1) for a in arrays)
-
-	# Copy each array into a 2d array of the appropriate shape.
-	rows = np.zeros((len(arrays), result_length))
-	for i, a in enumerate(arrays):
-		rows[i, :len(a)] = a
+			param_str = ""
 
-	# Transform, take the product, and do the inverse transform
-	# to get the convolution.
-	fft_of_rows = np.fft.fft(rows)
-	fft_of_convolution = fft_of_rows.prod(axis=0)
-	convolution = np.fft.ifft(fft_of_convolution)
+		return "DemandSource({:s}: {:s})".format(self.type, param_str)
 
-	# Assuming real inputs, the imaginary part of the output can be ignored.
-	return convolution.real
-
-
-def irwin_hall_cdf(x, n):
-	"""Return cdf of Irwin-Hall distribution, i.e., distribution of sum of ``n``
-	U[0,1] random variables.
-
-	See https://en.wikipedia.org/wiki/Irwin%E2%80%93Hall_distribution.
-
-	Parameters
-	----------
-	x : float
-		Argument of cdf function.
-	n : int
-		Number of U[0,1] random variables in the sum.
-
-	Returns
-	-------
-	F : float
-		The cdf of ``x``.
-	"""
-
-	# TODO vectorize this
-	F = 0
-	for k in range(int(np.floor(x)) + 1):
-		F += ((-1) ** k) * comb(n, k) * (x - k) ** n
-	F /= factorial(n)
-
-	return F
-
-
-def sum_of_uniforms_distribution(n, lo=0, hi=1):
-	"""Return distribution of sum of ``n`` identical uniform random variables as
-	``rv_continuous`` object.
-
-	If ``lo`` = 0 and ``hi`` = 1, this distribution is the Irwin-Hall
-	distribution.
-
-	Parameters
-	----------
-	n : int
-		Number of uniform random variables in the sum.
-	lo : float, optional
-		Lower bound of uniform distribution. Default = 0.
-	hi : float, optional
-		Upper bound of uniform distribution. Default = 1.
+	def __str__(self):
+		"""
+		Return the full name of the |class_demand_source| instance.
+
+		Returns
+		-------
+			The demand_source name.
+
+		"""
+		return self.__repr__()
+
+	# ATTRIBUTE HANDLING
+
+	def initialize(self):
+		"""Initialize the parameters in the object to their default values. 
+		"""
+		for attr in self._DEFAULT_VALUES.keys():
+			setattr(self, attr, self._DEFAULT_VALUES[attr])
+
+	def validate_parameters(self):
+		"""Check that appropriate parameters have been provided for the given
+		demand type. Raise an exception if not.
+		"""
+		if self.type not in ALLOWABLE_TYPES: raise AttributeError(f"Valid type in {ALLOWABLE_TYPES} must be provided")
+
+		# Note: Importane to use the '_' attributes here, rather than associated properties,
+		# to avoid infinite recursion. (For example, if self._mean is None, calling self.mean calls
+  		# self.demand_distribution(), which calls self.mean.) Plus, these attributes have to be set by
+		# user, not just calculated.
+		if self.type == 'N':
+			if self._mean is None: raise AttributeError("For 'N' (normal) demand, mean must be provided")
+			if self._mean < 0: raise AttributeError("For 'N' (normal) demand, mean must be non-negative")
+			if self._standard_deviation is None: raise AttributeError("For 'N' (normal) demand, standard_deviation must be provided")
+			if self._standard_deviation < 0: raise AttributeError("For 'N' (normal) demand, standard_deviation must be non-negative")
+		elif self.type == 'P':
+			if self._mean is None: raise AttributeError("For 'P' (Poisson) demand, mean must be provided")
+			if self._mean < 0: raise AttributeError("For 'P' (Poisson) demand, mean must be non-negative")
+		elif self.type == 'UD':
+			if self._lo is None: raise AttributeError("For 'UD' (uniform discrete) demand, lo must be provided")
+			if self._lo < 0 or not is_integer(self._lo): raise AttributeError("For 'UD' (uniform discrete) demand, lo must be a non-negative integer")
+			if self._hi is  None: raise AttributeError("For 'UD' (uniform discrete) demand, hi must be provided")
+			if self._hi < 0 or not is_integer(self._hi): raise AttributeError("For 'UD' (uniform discrete) demand, hi must be a non-negative integer")
+			if self._lo > self._hi: raise AttributeError("For 'UD' (uniform discrete) demand, lo must be <= hi")
+		elif self.type == 'UC':
+			if self._lo is None: raise AttributeError("For 'UC' (uniform continuous) demand, lo must be provided")
+			if self._lo < 0: raise AttributeError("For 'UC' (uniform continuous) demand, lo must be non-negative")
+			if self._hi is None: raise AttributeError("For 'UC' (uniform continuous) demand, hi must be provided")
+			if self._hi < 0: raise AttributeError("For 'UC' (uniform continuous) demand, hi must be non-negative")
+			if self._lo > self._hi: raise AttributeError("For 'UC' (uniform continuous) demand, lo must be <= hi")
+		elif self.type == 'NB':
+			if self._n is None: raise AttributeError("For 'NB' (negative binomial) demand, n must be provided")
+			if self._n <= 0: raise AttributeError("For 'NB' (negative binomial) demand, n must be positive")
+			if self._p is None: raise AttributeError("For 'NB' (negative binomial) demand, p must be provided")
+			if self._p < 0 or self._p > 1: raise AttributeError("For 'NB' (negative binomial) demand, p must be in [0, 1]")
+		elif self.type == 'D':
+			if self._demand_list is None: raise AttributeError("For 'D' (deterministic) demand, demand_list must be provided")
+		elif self.type == 'CD':
+			if self._demand_list is None: raise AttributeError("For 'CD' (custom discrete) demand, demand_list must be provided")
+			if self._probabilities is None: raise AttributeError("For 'CD' (custom discrete) demand, probabilities must be provided")
+			if len(self._demand_list) != len(self._probabilities): raise AttributeError("For 'CD' (custom discrete) demand, demand_list and probabilities must have equal lengths")
+			if np.sum(self._probabilities) != 1: raise AttributeError("For 'CD' (custom discrete) demand, probabilities must sum to 1")
+
+	# CONVERSION TO/FROM DICTS
+
+	def to_dict(self):
+		"""Convert the |class_demand_source| object to a dict. List attributes
+		(``demand_list``, ``probabilities``) are deep-copied so changes to the original
+		object do not get propagated to the dict.
+
+		Returns
+		-------
+		dict
+			The dict representation of the object.
+		"""
+		# Initialize dict.
+		ds_dict = {}
+
+		# Attributes.
+		for attr in self._DEFAULT_VALUES.keys():
+			# Remove leading '_' to get property names.
+			prop = attr[1:] if attr[0] == '_' else attr
+			ds_dict[prop] = getattr(self, prop)
+
+		return ds_dict
+
+	@classmethod
+	def from_dict(cls, the_dict):
+		"""Return a new |class_demand_source| object with attributes copied from the
+		values in ``the_dict``. List attributes (``demand_list``, ``probabilities``) 
+		are deep-copied so changes to the original dict do not get propagated to the object.
+		Any missing attributes are set to their default values.
+
+		Parameters
+		----------
+		the_dict : dict
+			Dict representation of a |class_demand_source|, typically created using ``to_dict()``.
+
+		Returns
+		-------
+		DemandSource
+			The object converted from the dict.
+		"""
+		if the_dict is None:
+			ds = cls()
+		else:
+			# Build empty DemandSource.
+			ds = cls()
+			# Fill attributes.
+			for attr in cls._DEFAULT_VALUES.keys():
+				# Remove leading '_' to get property names.
+				prop = attr[1:] if attr[0] == '_' else attr
+
+				# Some attributes require special handling.
+				if prop == 'demand_list':
+					if prop not in the_dict or the_dict[prop] is None:
+						value = None
+					elif the_dict[prop] is not None:
+						# If elements of demand_list are dicts (keys = products, values = demands),
+	  					# replace string keys with integers.
+						value = [{int(k): v for k, v in d.items()} if is_dict(d) else d for d in the_dict[prop]]
+				else:
+					if prop in the_dict:
+						value = the_dict[prop]
+					else:
+						value = cls._DEFAULT_VALUES[attr]
+
+				# Set the property/attribute.
+				setattr(ds, prop, value)
+	
+		return ds
+
+	# DEMAND GENERATION
+
+	def generate_demand(self, period=None):
+		"""Generate a demand value using the demand type specified in ``type``.
+		If ``type`` is ``None``, returns ``None``.
+
+		Parameters
+		----------
+		period : int, optional
+			The period to generate a demand value for. If ``type`` = 'D' (deterministic),
+			this is required if ``demand_list`` is a list of demands, one per period. If omitted,
+			will return first (or only) demand in list.
+
+		Returns
+		-------
+		demand : float
+			The demand value.
+
+		"""
+
+		if self.type is None:
+			return None
+		if self.type == 'N':
+			demand = self._generate_demand_normal()
+		elif self.type == 'P':
+			demand = self._generate_demand_poisson()
+		elif self.type == 'UD':
+			demand = self._generate_demand_uniform_discrete()
+		elif self.type == 'UC':
+			demand = self._generate_demand_uniform_continuous()
+		elif self.type == 'NB':
+			demand = self._generate_demand_negative_binomial()
+		elif self.type == 'D':
+			demand = self._generate_demand_deterministic(period)
+		elif self.type == 'CD':
+			demand = self._generate_demand_custom_discrete()
+		else:
+			demand = None
 
-	Returns
-	-------
-	distribution : rv_continuous
-		The rv_continuous object.
+		if self.round_to_int:
+			demand = int(np.round(demand))
 
-	"""
+		return demand
 
-	class sum_of_uniforms_rv(stats.rv_continuous):
-		def _cdf(self, x):
-			# P(X <= x) = P(Y <= (y - n * lo) / (hi - lo)), where Y is the sum of
-			# n U[0,1] r.v.s and therefore has an Irwin-Hall distribution.
-			if x < n * lo:
-				return 0
-			elif x > n * hi:
-				return 1
+	def _generate_demand_normal(self):
+		"""Generate demand from normal distribution.
+
+		Returns
+		-------
+		demand : float
+			The demand value.
+
+		"""
+		return max(0, float(np.random.normal(self.mean, self.standard_deviation)))
+
+	def _generate_demand_poisson(self):
+		"""Generate demand from Poisson distribution.
+
+		Returns
+		-------
+		demand : int
+			The demand value.
+
+		"""
+		return int(np.random.poisson(self.mean))
+
+	def _generate_demand_uniform_discrete(self):
+		"""Generate demand from discrete uniform distribution.
+
+		Returns
+		-------
+		demand : float
+			The demand value.
+
+		"""
+		return int(np.random.randint(int(self.lo), int(self.hi) + 1))
+
+	def _generate_demand_uniform_continuous(self):
+		"""Generate demand from continuous uniform distribution.
+
+		Returns
+		-------
+		demand : float
+			The demand value.
+
+		"""
+		return float(np.random.uniform(self.lo, self.hi - self.lo))
+
+	def _generate_demand_negative_binomial(self):
+		"""Generate demand from negative binomial distribution.
+
+		Returns
+		-------
+		demand : int
+			The demand value.
+
+		"""
+		return float(np.random.negative_binomial(self.n, self.p))
+	
+	def _generate_demand_deterministic(self, period=None):
+		"""Generate deterministic demand.
+
+		Parameters
+		----------
+		period : int, optional
+			The period to generate a demand value for. This is required if ``demand_list`` is a 
+			list of demands, one per period. If omitted, will return first (or only) demand in list.
+
+		Returns
+		-------
+		demand : float
+			The demand value.
+
+		"""
+		if is_iterable(self.demand_list):
+			if period is None:
+				# Return first demand in demand_list list.
+				return self.demand_list[0]
 			else:
-				return irwin_hall_cdf((x - n * lo) / (hi - lo), n)
-
-	distribution = sum_of_uniforms_rv()
-
-	return distribution
-
-
-def sum_of_discretes_distribution(n, lo, hi, p):
-	"""Return distribution of convolution of ``n`` identical discrete random variables as
-	``rv_discrete`` object.
-
-	The random variables must have support ``lo``, ``lo``+1, ..., ``hi``.
-	(The convolution will have support ``n * lo``, ``n * lo``+1, ..., ``n * hi``.
-
-
-	Parameters
-	----------
-	n : int
-		Number of uniform random variables in the sum.
-	lo : int
-		Smallest value of the support of the random variable.
-	hi : int
-		Largest value of the support of the random variable.
-	p : list
-		Probabilities of each of the values.
-
-	Returns
-	-------
-	distribution : rv_discrete
-		The rv_discrete object.
-
-	"""
-
-	xk = np.arange(n * lo, n * hi + 1)
-	pk = convolve_many([p for _ in range(n)])
-
-	distribution = stats.rv_discrete(name='sum_of_discretes', values=(xk, pk))
-
-	return distribution
-
-
-def run_irwin_hall_cdf_test():
-	"""Test ``helpers.irwin_hall_cdf()``. This is not a unit test; it must be
-	run manually. It simulates many sums of uniform distributions and plots
-	their empirical cdf against the calculated cdf.
+				# Get demand for period mod (# periods in demand_list list), i.e.,
+				# if we are past the end of the demand_list list, loop back to the beginning.
+				return self.demand_list[period % len(self.demand_list)]
+		else:
+			# Return demand_list singleton.
+			return self.demand_list
 
-	"""
+	def _generate_demand_custom_discrete(self):
+		"""Generate demand from custom discrete distribution.
 
-	n = 4
-	T = 100000
-	nbins = 100
-
-	sums = []
-	for t in range(T):
-		sums.append(np.sum(uniform.rvs(size=n)))
-
-	x = np.arange(0, n, n * 1.0/nbins)
-	F_empirical = np.zeros(np.size(x))
-	F_calc = np.zeros(np.size(x))
-	for b in range(nbins):
-		F_empirical[b] = np.sum(1 if sums[t] < x[b] else 0 for t in range(T)) / T
-		F_calc[b] = irwin_hall_cdf(x[b], n)
-
-	import matplotlib.pyplot as plt
-
-	plt.plot(x, F_empirical, 'r')
-	plt.plot(x, F_calc, 'b')
-	plt.show()
-
-
-def run_sum_of_uniforms_distribution_test():
-	"""Test ``helpers.sum_of_uniforms_distribution()``. This is not a unit test;
-	it must be run manually. It simulates many sums of uniform distributions and
-	plots their empirical cdf against the calculated cdf.
+		Returns
+		-------
+		demand : float
+			The demand value.
 
-	"""
+		"""
+		return np.random.choice(self.demand_list, p=self.probabilities)
 
-	n = 4
-	lo = 20
-	hi = 60
-	T = 10000
-	nbins = 100
+	# OTHER METHODS
 
-	sums = []
-	for t in range(T):
-		sums.append(np.sum(uniform.rvs(lo, hi-lo, size=n)))
+	def cdf(self, x):
+		"""Cumulative distribution function of demand distribution.
 
-	dist = sum_of_uniforms_distribution(n, lo, hi)
+		In some cases, this is just a wrapper around ``cdf()`` function
+		of ``scipy.stats.rv_continuous`` or ``scipy.stats.rv_discrete`` object.
 
-	x = np.arange(n*lo, n*hi, n * (hi-lo)/nbins)
-	F_empirical = np.zeros(np.size(x))
-	F_calc = np.zeros(np.size(x))
-	for b in range(nbins):
-		F_empirical[b] = np.sum(1 if sums[t] < x[b] else 0 for t in range(T)) / T
-		F_calc[b] = dist.cdf(x[b])
+		Parameters
+		----------
+		x : float
+			Value to calculate cdf for.
 
-	import matplotlib.pyplot as plt
+		Returns
+		-------
+		F : float
+			cdf of ``x``.
 
-	plt.plot(x, F_empirical, 'r')
-	plt.plot(x, F_calc, 'b')
-	plt.show()
+		"""
 
+		if self.type in (None, 'D'):
+			return None
+		else:
+			distribution = self.demand_distribution
+			return distribution.cdf(x)
 
 
-#test_irwin_hall_cdf()
-#test_sum_of_uniforms_distribution()
+	def lead_time_demand_distribution(self, lead_time):
+		"""Return lead-time demand distribution, as a
+		``scipy.stats.rv_continuous`` or ``scipy.stats.rv_discrete`` object.
+
+		.. note:: For 'UC', 'UD', 'NB', and 'CD' demands, this method calculates the lead-time
+			demand distribution as the sum of ``lead_time`` independent random variables.
+			Therefore, the method requires ``lead_time`` to be an integer for these
+			distributions. If it is not, it raises a ``ValueError``.
+
+		Parameters
+		----------
+		lead_time : float or int
+			The lead time. [:math:`L`]
+
+		Returns
+		-------
+		distribution : rv_continuous or rv_discrete
+			The lead-time demand distribution object.
+
+		Raises
+		------
+		ValueError
+			If ``type`` is 'UC', 'UD', 'NB', or 'CD' and ``lead_time`` is not an integer.
+		"""
+
+		# Check whether lead_time is an integer.
+		if self.type in ('UC', 'UD', 'NB', 'CD') and not is_integer(lead_time):
+			raise ValueError("lead_time must be an integer for 'UC', 'UD', 'NB', or 'CD' demand")
+
+		# Get distribution object.
+		if self.type == 'N':
+			return scipy.stats.norm(self.mean * lead_time, self.standard_deviation * math.sqrt(lead_time))
+		elif self.type == 'P':
+			return scipy.stats.poisson(self.mean * lead_time)
+		elif self.type == 'UC':
+			distribution = sum_of_continuous_uniforms_distribution(lead_time, self.lo, self.hi)
+		elif self.type == 'UD':
+			distribution = sum_of_discrete_uniforms_distribution(lead_time, self.lo, self.hi)
+		elif self.type == 'NB':
+			# Build probability list.
+			min_demand = 0
+			max_demand = int(self.demand_distribution.ppf(0.9999))
+			prob = [self.demand_distribution.pmf(d) for d in range(min_demand, max_demand + 1)]
+			prob = [prob[d] / sum(prob) for d in range(min_demand, max_demand + 1)]
+			distribution = sum_of_discretes_distribution(lead_time, min_demand, max_demand, prob)
+		elif self.type == 'CD':
+			# Convert probability list to a list with 0 values for x values not in support.
+			min_demand = min(self.demand_list)
+			max_demand = max(self.demand_list)
+			prob = []
+			for x in range(min_demand, max_demand + 1):
+				if x in self.demand_list:
+					prob.append(self.probabilities[self.demand_list.index(x)])
+				else:
+					prob.append(0)
+			distribution = sum_of_discretes_distribution(lead_time, min_demand, max_demand, prob)
+		else:
+			return None
 
+		return distribution
```

### Comparing `stockpyl-0.1.0a0/stockpyl/gsm_tree.py` & `stockpyl-1.0.0/src/stockpyl/gsm_tree.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,967 +1,1005 @@
 # ===============================================================================
 # stockpyl - gsm_tree Module
 # -------------------------------------------------------------------------------
-# Version: 0.0.0
-# Updated: 01-30-2022
 # Author: Larry Snyder
 # License: GPLv3
 # ===============================================================================
 
-"""Code to implement dynamic programming (DP) algorithm for guaranteed-service model (GSM)
-for multi-echelon inventory systems with tree structures by Graves and Willems (2000).
-
-'node' and 'stage' are used interchangeably in the documentation.
-
-The primary data object is the NetworkX DiGraph, which contains all of the data
-for the GSM instance.
-
-The following attributes are used to specify input data:
-	* Node-level attributes
-		- processing_time [T]
-		- external_inbound_cst [si]
-		- external_outbound_cst [s]
-		- holding_cost [h]
-		- demand_bound_constant [z_alpha]
-		- external_demand_mean [mu]
-		- external_demand_standard_deviation [sigma]
-	* Edge-level attributes
-		- units_required (e.g., on edge i->j, units_required units of item i are
-	required to make 1 unit of item j)
-
-The following attributes are used to store outputs and intermediate values:
-	* Graph-level attributes
-		- max_max_replenishment_time
-	* Node-level attributes:
-		- original_label
-		- net_demand_standard_deviation (standard deviation of combined demand
-		stream consisting of external demand and downstream demand)
-		- larger_adjacent_node [p]
-		- larger_adjacent_node_is_downstream
-		- max_replenishment_time [M]
-
-(c) Lawrence V. Snyder
-Lehigh University
-
 """
+.. include:: ../../globals.inc
 
-import networkx as nx
-
-from stockpyl.gsm_tree_helpers import *
-from stockpyl.helpers import *
-
-# TODO: add instances to instance JSON
-
-### GRAPH MANIPULATION ###
-
-def preprocess_tree(tree):
-	"""Preprocess the GSM tree. Returns an independent copy.
-
-	If tree is already correctly labeled, does not relabel it.
-
-	Fill node-level attributes: original_label, net_demand_mean,
-	net_demand_standard_deviation, larger_adjacent_node,
-	max_replenishment_time.
-	Fill missing data for demand_bound_constant, external_inbound_cst, and
-	external_outbound_cst attributes.
-
-	Fill max_max_replenishment_time graph-level attribute.
-
-	Parameters
-	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
-		Current node labels are ignored and may be anything.
-	start_index : int, optional
-		Integer to use as starting (smallest) node label.
-
-	Returns
-	-------
-	new_tree : graph
-		Pre-processed multi-echelon tree network.
-
-	"""
-
-	new_tree = tree.copy()
-
-	# Fill external inbound and outbound CST parameters, if not provided.
-	# Default value of external outbound CST = BIG_INT.
-	# Default value of external inbound CST = 0. (Not strictly necessary,
-	# but cleaner.)
-	for k in new_tree.nodes:
-		if 'external_inbound_cst' not in new_tree.nodes[k]:
-			new_tree.nodes[k]['external_inbound_cst'] = 0
-		if 'external_outbound_cst' not in new_tree.nodes[k]:
-			new_tree.nodes[k]['external_outbound_cst'] = BIG_INT
-
-	# Fill demand bound constant parameters, if not provided.
-	# Set equal to demand bound constant of sink node. If more than one sink node,
-	# one is chosen arbitrarily. If no sink nodes have demand bound constant,
-	# constant is set to 1.
-	sinks_with_dbc = [k for k in new_tree.nodes if new_tree.out_degree(k) == 0
-					  and 'demand_bound_constant' in new_tree.nodes[k]]
-	for k in new_tree.nodes:
-		if 'demand_bound_constant' not in new_tree.nodes[k]:
-			if sinks_with_dbc == []:
-				new_tree.nodes[k]['demand_bound_constant'] = 1
-			else:
-				new_tree.nodes[k]['demand_bound_constant'] = \
-					new_tree.nodes[sinks_with_dbc[0]]['demand_bound_constant']
-
-	# Calculate net demand parameters.
-	net_demand_means, net_demand_standard_deviations = net_demand(new_tree)
-	nx.set_node_attributes(new_tree, net_demand_means, 'net_demand_mean')
-	nx.set_node_attributes(new_tree, net_demand_standard_deviations,
-						   'net_demand_standard_deviation')
-
-	# Calculate max replenishment times.
-	max_replenishment_times = longest_paths(new_tree)
-	nx.set_node_attributes(new_tree, max_replenishment_times, 'max_replenishment_time')
-
-	# Calculate maximum value of max_replenishment_time.
-	new_tree.graph['max_max_replenishment_time'] = \
-		np.max(list(nx.get_node_attributes(new_tree,
-										   'max_replenishment_time').values()))
-
-	return new_tree
-
-
-def relabel_nodes(tree, start_index=0, force_relabel=False):
-	"""Perform the node-labeling algorithm described in Section 5 of Graves and
-	Willems (2000).
-
-	If tree is already correctly labeled, returns the original tree,
-	unless force_relabel is True, in which case performs the relabeling.
-
-	Does not modify the input tree. Fills 'original_label',
-	'larger_adjacent_node', and 'larger_adjacent_node_is_downstream' attributes
-	of nodes in new tree, whether or not original tree was already
-	correctly labeled.
-
-	Parameters
-	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
-		Current node labels are ignored (unless the tree is already correctly
-		labeled) and may be anything.
-	start_index : int, optional
-		Integer to use as starting (smallest) node label.
-	force_relabel : bool, optional
-		If True, function will relabel nodes even if original tree is correctly
-		labeled.
-
-	Returns
-	-------
-	relabeled_tree : graph
-		NetworkX directed graph representing the relabeled tree network.
-
-	"""
-
-	# Check whether tree is already correctly labeled.
-	is_correct = is_correctly_labeled(tree)
-
-	# Do relabel?
-	if is_correct and not force_relabel:
-		relabeled_tree = tree.copy()
-		new_labels = {k: k for k in tree.nodes}
-	else:
-
-		# Initialize all nodes to "unlabeled", and initialize list of new labels.
-		labeled = {i: False for i in tree.nodes()}
-		new_labels = {}
-
-		# Find nodes that are adjacent to at most 1 unlabeled node and label them.
-		for k in range(start_index, start_index+nx.number_of_nodes(tree)):
-
-			# Find a node for labeling.
-			for i in tree.nodes():
-
-				# Make sure i is unlabeled.
-				if not labeled[i]:
-					# Count unlabeled nodes that are adjacent to node i.
-					num_adj = len([j for j in nx.all_neighbors(tree, i) if not labeled[j]])
-
-					# If i is adjacent to at most 1 unlabeled node, label it.
-					if num_adj <= 1:
-						# Change i's label to k.
-						new_labels[i] = k
-						# Mark i as labeled.
-						labeled[i] = True
-						# Break out of 'for i' loop
-						break
-
-		# Relabel the nodes
-		relabeled_tree = nx.relabel_nodes(tree, new_labels)
-
-	# Fill original_label attribute of relabeled tree.
-	original_labels = {new_labels[k]: k for k in tree.nodes}
-	nx.set_node_attributes(relabeled_tree, original_labels, 'original_label')
-
-	# Fill larger-adjacent-node attributes.
-	larger_adjacent, downstream = find_larger_adjacent_nodes(relabeled_tree)
-	nx.set_node_attributes(relabeled_tree, larger_adjacent, 'larger_adjacent_node')
-	nx.set_node_attributes(relabeled_tree, downstream, 'larger_adjacent_node_is_downstream')
-
-	return relabeled_tree
-
-
-def is_correctly_labeled(tree):
-	"""Determine whether tree is already correctly labeled.
-
-	Tree is correctly labeled if all labels are integers, the integers are
-	consecutive, and every stage (other than the highest-indexed one) has
-	exactly one adjacent stage with a greater index.
-
-	Parameters
-	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
+Overview 
+--------
 
-	Returns
-	-------
-	True if tree is already correctly labeled.
-	"""
+The |mod_gsm_tree| module implements Graves and Willems's (2000, 2003) dynamic programming (DP)
+algorithm for multi-echelon inventory systems with tree structures. 
 
-	# Get indices.
-	ind = list(tree.nodes)
+.. note:: |node_stage|
 
-	# Check whether every label is a non-negative integer.
-	if not np.all([str(k).isdigit() for k in ind]):
-		is_correct = False
-	else:
-		# Check whether labels are consecutive integers starting at min_index.
-		min_index = np.min(ind)
-		if set(ind) != set(range(min_index, min_index + len(ind))):
-			is_correct = False
-		else:
-			# Check whether every node as exactly one adjacent stage with
-			# greater index.
-			is_correct = True
-			for k in tree.nodes:
-				if k < np.max(ind):
-					greater_indexed_neighbors = \
-						{i for i in tree.predecessors(k) if i > k}.union(
-							{i for i in tree.successors(k) if i > k}
-						)
-					if len(greater_indexed_neighbors) != 1:
-						is_correct = False
-
-	return is_correct
-
-
-def find_larger_adjacent_nodes(tree):
-	"""Find larger-indexed adjacent node, for each node in tree.
-
-	After the nodes are relabeled by relabel_nodes(), each node (except the
-	node with the largest index) is adjacent to exactly one node with a
-	larger index. Node k's neighbor with larger index is denoted p(k) in
-	Graves and Willems (2000). This function finds p(k) for all k and also
-	indicates whether p(k) is upstream or downstream from k.
-
-	Parameters
-	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
-		Nodes are assumed to have been relabeled using relabel_nodes().
-
-	Returns
-	-------
-	larger_adjacent: dict
-		Dict containing index of each node's larger-indexed adjacent node,
-		for all nodes except the largest-indexed node.
-	downstream: dict
-		Dict containing, for each node, True if the larger-indexed adjacent
-		node is downstream from the node, False if it is upstream, for all
-		nodes except the largest-indexed node.
-	"""
-
-	# Initialize dicts.
-	larger_adjacent = {}
-	downstream = {}
-
-	# Loop through nodes.
-	for k in tree.nodes:
-		if k < np.max(list(tree.nodes)):
-			# Get list of nodes that are adjacent to k and have a larger index,
-			# but the list will only contain a single item; set larger_adjacent[k] to it.
-			larger_adjacent_list = [i for i in nx.all_neighbors(tree, k) if i > k]
-			larger_adjacent[k] = larger_adjacent_list[0]
-
-			# Set downstream flag.
-			if larger_adjacent[k] in tree.successors(k):
-				downstream[k] = True
-			else:
-				downstream[k] = False
-
-	return larger_adjacent, downstream
-
-
-def longest_paths(tree):
-	"""Determine the length of the longest path from any source node to to each
-	node k.
-
-	Arc lengths are determined by processing times. External inbound CSTs are
-	considered source nodes, so having an external inbound CST at node i of 5 is
-	like having another node that serves node i with a processing time of 5.
-
-	Parameters
-	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
-		Nodes are assumed to have been relabeled using relabel_nodes().
-
-	Returns
-	-------
-	longest_lengths : dict
-		Dict of longest paths to each node (M_k).
-
-	"""
-
-	# Get dict of external inbound CSTs. (Some nodes may have no entry.)
-	external_inbound_cst = nx.get_node_attributes(tree, 'external_inbound_cst')
+The primary data object is the |class_network|, which contains all of the data
+for the GSM instance.
 
-	# Copy the tree. Set the weight of each edge into a given node k to the processing
-	# time of node k. If node k is a source node and/or it has an external inbound CST,
-	# add a dummy node before node k and set weight of edge from dummy node to node k
-	# equal to processing time of node k + external inbound CST for node k.
-	temp_tree = tree.copy()
-	for k in tree.nodes:
-		for p in tree.predecessors(k):
-			temp_tree[p][k]['weight'] = tree.nodes[k]['processing_time']
-		if tree.in_degree(k) == 0 or external_inbound_cst.get(k, 0) > 0:
-			temp_tree.add_edge('dummy_' + str(k), k,
-							   weight=tree.nodes[k]['processing_time'] + external_inbound_cst.get(k, 0))
+.. note:: |fosct_notation|
 
-	# Determine shortest path between every pair of nodes.
-	# (Really there's only one path, but shortest path is the
-	# most straightforward algorithm to use here.)
-	path_lengths = dict(nx.shortest_path_length(temp_tree, weight='weight'))
+.. seealso::
 
-	# Determine longest shortest path to each node k, among all
-	# source nodes that are ancestors to k.
-	longest_lengths = {}
-	for k in tree.nodes:
-		longest_lengths[k] = max([path_lengths[i][k] for i in
-								  nx.ancestors(temp_tree, k)], default=0)
+	For an overview of multi-echelon inventory optimization in |sp|,
+	see the :ref:`tutorial page for multi-echelon inventory optimization<tutorial_meio_page>`.
 
-	return longest_lengths
 
+References
+----------
+S. C. Graves and S. P. Willems. Optimizing strategic safety stock placement in supply chains. 
+*Manufacturing and Service Operations Management*, 2(1):68-83, 2000.
 
-def net_demand(tree):
-	"""Calculate net demand mean and standard deviation for all nodes in tree.
+S. C. Graves and S. P. Willems. Erratum: Optimizing strategic safety stock placement in supply chains. 
+*Manufacturing and Service Operations Management*, 5(2):176-177, 2003.
 
-	Net demand is the demand stream consisting of the external demand for the
-	node plus all downstream demand.
 
-	Parameters
-	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
-
-	Returns
-	-------
-	net_means : dict
-		Dict of net mean for each node.
+API Reference
+-------------
+"""
 
-	net_standard_deviations : dict
-		Dict of net standard deviation for each node.
+import networkx as nx
+import copy
 
-	"""
+from stockpyl.gsm_helpers import *
+from stockpyl.helpers import *
+from stockpyl.supply_chain_network import SupplyChainNetwork
+from stockpyl.supply_chain_node import SupplyChainNode
 
-	# Initialize net_mean and net_variances using each node's external demand.
-	net_means = {k: tree.nodes[k].get('external_demand_mean', 0) for k in
-				tree.nodes}
-	net_variances = {k: tree.nodes[k].get('external_demand_standard_deviation', 0)**2
-				for k in tree.nodes}
 
-	# Make temp copy of tree.
-	temp_tree = tree.copy()
 
-	# Loop through temp_tree. At each iteration, handle leaf nodes (nodes with
-	# no _successors), adding their net_means and net_variances to those of their
-	# _predecessors. Then remove the leaf nodes and iterate.
-	while temp_tree.number_of_nodes() > 0:
-		leaf_nodes = [k for k in temp_tree.nodes if temp_tree.out_degree(k) == 0]
-		for k in leaf_nodes:
-			for i in temp_tree.predecessors(k):
-				net_means[i] += net_means[k]
-				net_variances[i] += net_variances[k]
-			temp_tree.remove_node(k)
+### OPTIMIZATION ###
 
-	net_standard_deviations = {k: np.sqrt(net_variances[k]) for k in tree.nodes}
-	return net_means, net_standard_deviations
+def optimize_committed_service_times(tree):
+	"""Optimize committed service times using the dynamic programming (DP) algorithm of
+	Graves and Willems (2000, 2003).
 
+	``tree`` is the |class_network| containing the instance. The tree need not already have been
+	pre-processed using :func:`preprocess_tree` or :func:`relabel_nodes`; this function will do so. 
 
-def connected_subgraph_nodes(tree):
-	"""Determine nodes connected to k in subgraph on {min_k,...,k}, for each k,
-	where min_k is smallest index in graph. [N_k]
+	Output parameters are expressed using the original labeling of tree, even if the nodes
+	are relabeled internally.
 
-	Connected does not necessarily mean adjacent.
+	Demands are assumed to be normally distributed. 
 
 	Parameters
 	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
+	tree : |class_network|
+		The multi-echelon tree network. Current node labels are ignored and may be anything.
 
 	Returns
 	-------
-	connected_nodes : dict
-		Dict of set of connected subgraph nodes for each node.
+	opt_cst : dict
+		Dict of optimal CSTs, with node indices as keys and CSTs as values.
+	opt_cost : float
+		Optimal expected cost of system.
+	
+	Raises
+	------
+	ValueError
+		If any sink node (node with no successors) has no demand mean or standard devation provided.
 
-	"""
 
-	# Intiailize output dict.
-	connected_nodes = {}
+	**Example** (Example 6.5):
 
-	# Loop through nodes.
-	for k in tree.nodes:
-		# Build subgraph on {min_k,...,k}.
-		subgraph = tree.to_undirected().subgraph(range(np.min(tree.nodes), k+1))
-		# Build set of connected nodes.
-		connected_nodes[k] = set(i for i in subgraph.nodes if
-							  nx.has_path(subgraph, i, k))
+	.. testsetup:: *
 
-	return connected_nodes
+		from stockpyl.gsm_tree import *
 
+	.. doctest::
 
-def GSM_to_SSM(tree, p=None):
-	"""Convert GSM tree to SSM tree:
-		- Convert local to echelon holding costs.
-		- Convert processing times to lead times.
-		- Include stockout cost at demand nodes (if provided).
+		>>> from stockpyl.instances import load_instance
+		>>> tree = load_instance("example_6_5")
+		>>> opt_cst, opt_cost = optimize_committed_service_times(tree)
+		>>> opt_cst
+		{1: 0, 3: 0, 2: 0, 4: 1}
+		>>> opt_cost
+		8.277916867529369
 
-	Tree must be pre-processed before calling.
 
-	Parameters
+	References
 	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
-	p : float, optional
-		Stockout cost to use at demand nodes. If None, copies stockout_cost
-		field from tree for nodes that have it, and does not fill stockout_cost
-		for nodes that do not.
-		# TODO: allow different p values at different demand nodes
+	S. C. Graves and S. P. Willems. Optimizing strategic safety stock placement in supply chains. 
+	*Manufacturing and Service Operations Management*, 2(1):68-83, 2000.
 
-	Returns
-	-------
-	SSM_tree : graph
-		SSM representation of tree.
+	S. C. Graves and S. P. Willems. Erratum: Optimizing strategic safety stock placement in supply chains. 
+	*Manufacturing and Service Operations Management*, 5(2):176-177, 2003.
 	"""
+ 
+	# Validate parameters.
+	for n in tree.sink_nodes:
+		if n.demand_source.mean is None:
+			raise ValueError(f'All sink nodes must have demand_source.mean (node {n.index} does not).')
+		if n.demand_source.standard_deviation is None:
+			raise ValueError(f'All sink nodes must have demand_source.standard_deviation (node {n.index} does not).')
 
-	# Build new graph.
-	SSM_tree = nx.DiGraph()
-
-	# Add nodes.
-	for n in tree.nodes:
-		upstream_h = np.sum([tree.nodes[k]['holding_cost'] for k in
-							 tree.predecessors(n)])
-		SSM_tree.add_node(n,
-			lead_time=tree.nodes[n]['processing_time']+tree.nodes[n]['external_inbound_cst'],
-			echelon_holding_cost=tree.nodes[n]['holding_cost'] - upstream_h)
-		if 'external_demand_mean' in tree.nodes[n]:
-			SSM_tree.nodes[n]['mean'] = \
-				tree.nodes[n]['external_demand_mean']
-		if 'external_demand_standard_deviation' in tree.nodes[n]:
-			SSM_tree.nodes[n]['standard_deviation'] = \
-				tree.nodes[n]['external_demand_standard_deviation']
-		if p is not None:
-			if tree.nodes[n]['external_demand_mean'] > 0 or \
-				tree.nodes[n]['external_demand_standard_deviation'] > 0:
-				SSM_tree.nodes[n]['stockout_cost'] = p
-		else:
-			if 'stockout_cost' in tree.nodes[n]:
-				SSM_tree.nodes[n]['stockout_cost'] = tree.nodes[n]['stockout_cost']
-
-	# Add edges.
-	SSM_tree.add_edges_from(tree.edges)
-
-	return SSM_tree
-
-
-### OPTIMIZATION ###
-
-def optimize_committed_service_times(tree):
-	"""Optimize committed service times.
-
-	Optimization is performed using the dynamic programming (DP) algorithm of
-	Graves and Willems (2000).
-
-	tree is the DiGraph containing the instance. The tree must already have been
-	pre-processed using preprocess_tree(), but it need not have had its nodes
-	relabeled using relabel_nodes().
-
-	Output parameters are expressed using the original labeling of tree.
-
-	Parameters
-	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
-		Current node labels are ignored and may be anything.
-
-	Returns
-	-------
-	opt_cost : float
-		Optimal expected cost of system.
-	opt_cst : dict
-		Dict of optimal CSTs.
-
-	"""
+	# Preprocess tree.
+	tree = preprocess_tree(tree)
 
 	# Relabel nodes.
 	tree = relabel_nodes(tree)
 
 	# Solve.
-	opt_cost, opt_cst_relabeled = cst_dp(tree)
+	opt_cst_relabeled, opt_cost = _cst_dp_tree(tree)
 
 	# Prepare optimal solution in terms of original labels.
-	opt_cst = {tree.nodes[k]['original_label']: opt_cst_relabeled[k]
-			   for k in tree.nodes}
+	opt_cst = {k.original_label: opt_cst_relabeled[k.index] for k in tree.nodes}
 
-	return opt_cost, opt_cst
+	return opt_cst, opt_cost
 
 
-def cst_dp(tree):
+def _cst_dp_tree(tree):
 	"""Optimize committed service times on pre-processed tree.
 
 	Optimization is performed using the dynamic programming (DP) algorithm of
 	Graves and Willems (2000).
 
-	tree is the DiGraph containing the instance. It must be pre-processed
+	``tree`` is the |class_network| containing the instance. It must be pre-processed
 	before calling this function.
 
+	Assumes demand bound over tau periods is of the form
+	:math:`z_\\alpha\\sigma\\sqrt{\\tau}`.
+
 	Parameters
 	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
-		Current node labels are ignored and may be anything.
+	tree : |class_network|
+		The multi-echelon tree network. Current node labels are ignored and may be anything.
 
 	Returns
 	-------
+	opt_cst : dict
+		Dict of optimal CSTs, with node indices as keys and CSTs as values.
 	opt_cost : float
 		Optimal expected cost of system.
-	opt_cst : dict
-		Dict of optimal CSTs.
 
 	"""
 
-
 	# Initialize dicts to store values of theta_in(.) and theta_out(.) functions
 	# (called f(.) and g(.) in Graves and Willems).
-	theta_in = {k: {} for k in tree.nodes}
-	theta_out = {k: {} for k in tree.nodes}
+	theta_in = {k_index: {} for k_index in tree.node_indices}
+	theta_out = {k_index: {} for k_index in tree.node_indices}
 
 	# Get min and max node indices (for convenience).
-	min_k = np.min(list(tree.nodes))
-	max_k = np.max(list(tree.nodes))
+	min_k_index = int(np.min(tree.node_indices))
+	max_k_index = int(np.max(tree.node_indices))
 
 	# Initialize best_cst_adjacent.
-	# best_cst_adjacent[k][S][i] = CST chosen for stage i when calculating
+	# best_cst_adjacent[k_index][S][i] = CST chosen for stage i when calculating
 	# theta_out(S) or theta_in(SI) for stage k.
-	best_cst_adjacent = {k: {S: {} for S in
-		range(tree.nodes[k]['max_replenishment_time']+1)} for k in tree.nodes}
+	best_cst_adjacent = {k.index: {S: {} for S in
+		range(k.max_replenishment_time+1)} for k in tree.nodes}
 
 	# Loop through stages.
-	for k in range(min_k, max_k + 1):
+	for k_index in range(min_k_index, max_k_index + 1):
 
 		# Get shortcuts to some parameters (for convenience).
-		max_replen_time = tree.nodes[k]['max_replenishment_time']
-		proc_time = tree.nodes[k]['processing_time']
+		k = tree.get_node_from_index(k_index)
+		max_replen_time = k.max_replenishment_time
+		proc_time = k.processing_time
+
+		# Evaluate theta_out(k_index, S) if p(k_index) is downstream from k_index and
+		# and k_index < final k_index, evaluate theta_in(k_index, SI) otherwise.
+		if k_index < max_k_index and k.larger_adjacent_node_is_downstream:
 
-		# Evaluate theta_out(k, S) if p(k) is downstream from k and
-		# and k < final k, evaluate theta_in(k, SI) otherwise.
-		if k < max_k and tree.nodes[k]['larger_adjacent_node_is_downstream']:
-
-			# p(k) is downstream from k -- evaluate theta_out(k, S).
+			# p(k_index) is downstream from k_index -- evaluate theta_out(k_index, S).
 			for S in range(max_replen_time+1):
 				# Calculate theta_out.
-				theta_out[k][S], temp_best_cst_adjacent = \
-					calculate_theta_out(tree, k, S, theta_in, theta_out)
+				theta_out[k_index][S], temp_best_cst_adjacent = \
+					_calculate_theta_out(tree, k_index, S, theta_in, theta_out)
 				# Copy temp_best_cst_adjacent to best_cst_adjacent.
-				best_cst_adjacent[k][S] = {i: temp_best_cst_adjacent[i]
+				best_cst_adjacent[k_index][S] = {i: temp_best_cst_adjacent[i]
 										   for i in temp_best_cst_adjacent}
 
 			# Set values of theta_out and best_cst_adjacent for
 			# max_replenishment_time+1 to max_max_replenishment_time to
 			# theta_out(max_replenishment_time).
 			# Needed so that stages with larger max_replenishment_time don't
 			# encounter undefined values of theta_out.
 			for S in range(max_replen_time+1,
-						   tree.graph['max_max_replenishment_time'] + 1):
-				theta_out[k][S] = theta_out[k][max_replen_time]
-				best_cst_adjacent[k][S] = best_cst_adjacent[k][max_replen_time]
+						   tree.max_max_replenishment_time + 1):
+				theta_out[k_index][S] = theta_out[k_index][max_replen_time]
+				best_cst_adjacent[k_index][S] = best_cst_adjacent[k_index][max_replen_time]
 
 		else:
 
-			# p(k) is upstream from k -- evaluate theta_in(k, SI).
+			# p(k_index) is upstream from k_index -- evaluate theta_in(k_index, SI).
 			for SI in range(max_replen_time - proc_time + 1):
 				# Calculate theta_in.
-				theta_in[k][SI], temp_best_cst_adjacent = \
-					calculate_theta_in(tree, k, SI, theta_in, theta_out)
+				theta_in[k_index][SI], temp_best_cst_adjacent = \
+					_calculate_theta_in(tree, k_index, SI, theta_in, theta_out)
 				# Copy temp_best_cst_adjacent to best_cst_adjacent.
-				best_cst_adjacent[k][SI] = {i: temp_best_cst_adjacent[i]
+				best_cst_adjacent[k_index][SI] = {i: temp_best_cst_adjacent[i]
 											for i in temp_best_cst_adjacent}
 
 			# Set values of theta_in and best_cst_adjacent for
 			# max_replenishment_time+1 to max_max_replenishment_time to
 			# theta_in(max_replenishment_time - processing_time).
 			# Needed so that stages with larger max_replenishment_time don't
 			# encounter undefined values of theta_in.
 			for SI in range(max_replen_time - proc_time + 1,
-							tree.graph['max_max_replenishment_time'] + 1):
-				theta_in[k][SI] = theta_in[k][max_replen_time - proc_time]
-				best_cst_adjacent[k][SI] = \
-					best_cst_adjacent[k][max_replen_time - proc_time]
+							tree.max_max_replenishment_time + 1):
+				theta_in[k_index][SI] = theta_in[k_index][max_replen_time - proc_time]
+				best_cst_adjacent[k_index][SI] = \
+					best_cst_adjacent[k_index][max_replen_time - proc_time]
 
 	# Determine best value of SI for final stage.
-	SI_dict = {SI: theta_in[max_k][SI] for SI in
-			   range(tree.nodes[max_k]['max_replenishment_time'] -
-					 tree.nodes[max_k]['processing_time'] + 1)} # smaller range of SI
+	max_k_node = tree.get_node_from_index(max_k_index)
+	SI_dict = {SI: theta_in[max_k_index][SI] for SI in
+			   range(max_k_node.max_replenishment_time -
+					 max_k_node.processing_time + 1)} # smaller range of SI
 	best_theta_in, best_SI = min_of_dict(SI_dict)
 
 	# Initialize dict of optimal CSTs and optimal inbound CSTs.
 	opt_cst = {}
 	opt_in_cst = {}
 
-	# Backtrack to find optimal CSTs: Loop backwards through stages k;
-	# if p(k) is downstream from k, then set k's outbound CST to p(k)'s
-	# optimal inbound CST (which we get from best_cst_adjacent[p(k)][CST(p(k))]);
-	# if p(k) is upstream from k, then set k's inbound CST to p(k)'s optimal
-	# outbound CST and set k's outbound CST to the optimal for that inbound
-	# CST (from best_cst_adjacent[p(k)][CST(p(k))]).
+	# Backtrack to find optimal CSTs: Loop backwards through stages k_index;
+	# if p(k_index) is downstream from k_index, then set k_index's outbound CST to p(k_index)'s
+	# optimal inbound CST (which we get from best_cst_adjacent[p(k_index)][CST(p(k_index))]);
+	# if p(k_index) is upstream from k_index, then set k_index's inbound CST to p(k_index)'s optimal
+	# outbound CST and set k_index's outbound CST to the optimal for that inbound
+	# CST (from best_cst_adjacent[p(k_index)][CST(p(k_index))]).
 	# For each stage, remember optimal outbound _and_ inbound CSTs.
-	for k in range(max_k, min_k-1, -1):
+	for k_index in range(max_k_index, min_k_index-1, -1):
+
+		# Get node k.
+		k = tree.get_node_from_index(k_index)
 
-		# Get p(k), and determine whether p(k) and p(p(k)) are upstream or
+		# Get p(k_index), and determine whether p(k_index) and p(p(k_index)) are upstream or
 		# downstream (for convenience).
-		if k < max_k:
-			pk = tree.nodes[k]['larger_adjacent_node']
-			pk_is_downstream = tree.nodes[k]['larger_adjacent_node_is_downstream']
-			if pk < max_k:
-				ppk_is_downstream = tree.nodes[pk]['larger_adjacent_node_is_downstream']
+		if k_index < max_k_index:
+			pk = k.larger_adjacent_node
+			pk_is_downstream = k.larger_adjacent_node_is_downstream
+			if pk < max_k_index:
+				ppk_is_downstream = tree.get_node_from_index(pk).larger_adjacent_node_is_downstream
 
-		# Where is p(k)?
-		if k == max_k:
+		# Where is p(k_index)?
+		if k_index == max_k_index:
 			# This is final stage.
-			opt_cst[k] = best_cst_adjacent[k][best_SI][k]
-			opt_in_cst[k] = best_SI
+			opt_cst[k_index] = best_cst_adjacent[k_index][best_SI][k_index]
+			opt_in_cst[k_index] = best_SI
 		elif pk_is_downstream:
-			# p(k) is downstream from k. Is p(p(k)) upstream or downstream from p(k)?
-			if pk != max_k and ppk_is_downstream:
-				# p(p(k)) is downstream from p(k) -- that means that optimal
+			# p(k_index) is downstream from k. Is p(p(k_index)) upstream or downstream from p(k_index)?
+			if pk != max_k_index and ppk_is_downstream:
+				# p(p(k_index)) is downstream from p(k_index) -- that means that optimal
 				# CST values are stored in best_cst_adjacent[pk][opt_cst[pk]][.].
-				opt_cst[k] = best_cst_adjacent[pk][opt_cst[pk]][k]
+				opt_cst[k_index] = best_cst_adjacent[pk][opt_cst[pk]][k_index]
 			else:
-				# p(p(k)) is upstream from p(k) (or it's the final node) --
+				# p(p(k_index)) is upstream from p(k_index) (or it's the final node) --
 				# that means that optimal CST values are stored in
 				# best_cst_adjacent[pk][opt_in_cst[ppk]][.].
-				# TODO: best_cst_adjacent[pk][opt_in_cst[pk]][.] ???
-				opt_cst[k] = best_cst_adjacent[pk][opt_in_cst[pk]][k]
-			opt_in_cst[k] = best_cst_adjacent[k][opt_cst[k]][k]
+				opt_cst[k_index] = best_cst_adjacent[pk][opt_in_cst[pk]][k_index]
+			opt_in_cst[k_index] = best_cst_adjacent[k_index][opt_cst[k_index]][k_index]
 		else:
-			# p(k) is upstream from k. Is p(p(k)) upstream or downstream from p(k)?
-			if pk != max_k and ppk_is_downstream:
-				# p(p(k)) is downstream from p(k) -- that means that optimal
+			# p(k_index) is upstream from k. Is p(p(k_index)) upstream or downstream from p(k_index)?
+			if pk != max_k_index and ppk_is_downstream:
+				# p(p(k_index)) is downstream from p(k_index) -- that means that optimal
 				# inbound CST values are stored in
 				# best_cst_adjacent[pk][opt_cst[pk]][.].
-				opt_in_cst[k] = best_cst_adjacent[pk][opt_cst[pk]][k]
+				opt_in_cst[k_index] = best_cst_adjacent[pk][opt_cst[pk]][k_index]
 			else:
-				# p(p(k)) is upstream from p(k) (or it's the final node) --
+				# p(p(k_index)) is upstream from p(k_index) (or it's the final node) --
 				# that means that optimal inbound CST values are stored in
 				# best_cst_adjacent[pk][opt_in_cst[pk]][.].
-				opt_in_cst[k] = best_cst_adjacent[pk][opt_in_cst[pk]][k]
-			opt_cst[k] = best_cst_adjacent[k][opt_in_cst[k]][k]
+				opt_in_cst[k_index] = best_cst_adjacent[pk][opt_in_cst[pk]][k_index]
+			opt_cst[k_index] = best_cst_adjacent[k_index][opt_in_cst[k_index]][k_index]
 
-		# If outbound CST for k is greater than k's external outbound CST,
+		# If outbound CST for k_index is greater than k_index's external outbound CST,
 		# reset it.
-		opt_cst[k] = min(opt_cst[k], tree.nodes[k]['external_outbound_cst'])
+		opt_cst[k_index] = min(opt_cst[k_index], k.external_outbound_cst)
 
 	# Get optimal cost.
 	opt_cost = best_theta_in
 
-	return opt_cost, opt_cst
+	return opt_cst, opt_cost
 
 
-def calculate_theta_out(tree, k, S, theta_in_partial, theta_out_partial):
-	"""Calculate the function theta_out(k, S) as described in Section 6.3.6.2 of
-	Snyder and Shen (2019) [function f_i(S) in Section 5 of Graves and Willems
+def _calculate_theta_out(tree, k_index, S, theta_in_partial, theta_out_partial):
+	"""Calculate the function :math:`\\theta^o_k(S)` as described in Section 6.3.6.2 of
+	|fosct| [function :math:`f_i(S)` in Section 5 of Graves and Willems
 	(2003)].
 
 	Original function is modified in the following ways:
-	1. If S is greater than the external outbound CST for stage k,
-	theta_out(k, S) is calculated as though S = external outbound CST. (If k is a sink
-	stage, theta_out(k,.) will never be calculated [theta_in(k,.) will be], but
-	k might have non-zero external outbound CST even if it is not a sink stage.)
-	2. The range of values of SI for which c_k(S,SI) is evaluated begins at
-	max(external_inbound_cst, S - T_k), not max(0, S - T_k).
-	3. The demand bound demand bound over tau periods is assumed to be of the form
-	z_alpha * sigma * sqrt(tau).
-	4. When calculating c_k(S, SI), upstream nodes are allowed to use outbound
-	CSTs greater than SI, and downstream nodes are allowed to use inbound
-	CSTs greater than S. In effect, this allows multiple inbound/outbound
-	CSTs for a single nodes.
+	1. If :math:`S` is greater than the external outbound CST for stage :math:`k`,
+	:math:`\\theta^o_k(S)` is calculated as though :math:`S` = external outbound CST. (If :math:`k` is a sink
+	stage, :math:`\\theta^o_k(\\cdot)` will never be calculated [:math:`\\theta^i_k(\\cdot)` will be], but
+	:math:`k` might have non-zero external outbound CST even if it is not a sink stage.)
+	2. The range of values of :math:`SI` for which :math:`c_k(S,SI)` is evaluated begins at
+	:math:`\\max\\{\\text{external_inbound_cst}, S - T_k\\}`, not :math:`\\max\\{0, S - T_k\\}`.
+	3. The demand bound demand bound over :math:`\\tau` periods is assumed to be of the form
+	:math:`z_\\alpha\\sigma\\sqrt{\\tau}`.
+	4. When calculating :math:`c_k(S, SI)`, upstream nodes are allowed to use outbound
+	CSTs greater than :math:`SI`, and downstream nodes are allowed to use inbound
+	CSTs greater than :math:`S`. In effect, this allows multiple inbound/outbound
+	CSTs for a single node.
 
 	Parameters
 	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
-		Tree must be pre-processed already.
-	k : int
+	tree : |class_network|
+		The multi-echelon tree network. Tree must be pre-processed already.
+	k_index : int
 		Index of node.
 	S : int
 		Outbound committed service time.
 	theta_in_partial : dict
 		Dict of values of theta_in function that have been calculated so far
-		(i.e., for i < k).
+		(i.e., for ``i`` < ``k_index``).
 	theta_out_partial : dict
 		Dict of values of theta_out function that have been calculated so far
-		(i.e., for i < k).
+		(i.e., for ``i`` < ``k_index``).
 
 	Returns
 	-------
 	theta_out_k_S : float
-		The value of theta_out(k, S).
+		The value of :math:`\\theta^o_k(S)`.
 	best_cst_adjacent : dict
-		Dict indicating, for each adjacent stage i with i <= k, the CST value
-		that minimized theta_out(.) for the optimal value of SI.
-		* If i serves k, then best_CST_adjacent[i] = the value of S_i that
-		minimizes theta_out(i, S_i).
-		* If i is served by k, then best_CST_adjacent[i] = the value of SI_i
-		that minimizes theta_in(i, SI_i).
-		* If i = k, then best_CST_adjacent[i] = the best value of SI chosen in
-		minimization of theta_out(.).
+		Dict indicating, for each adjacent stage :math:`i` with :math:`i \\le k`, the CST value
+		that minimized :math:`\\theta^o_i(\\cdot)` for the optimal value of :math:`SI`.
+		* If :math:`i` serves :math:`k`, then ``best_CST_adjacent[i]`` = the value of :math:`S_i` that
+		minimizes :math:`\\theta^o_i(S_i)`.
+		* If :math:`i` is served by :math:`k`, then ``best_CST_adjacent[i]`` = the value of :math:`SI_i`
+		that minimizes :math:`\\theta^i_i(SI_i)`.
+		* If :math:`i = k`, then ``best_CST_adjacent[i]`` = the best value of :math:`SI` chosen in
+		minimization of :math:`\\theta^o_k(\\cdot)`.
 	"""
 
-	# Get node k, for convenience.
-	node_k = tree.nodes[k]
+	# Get node k_index, for convenience.
+	k = tree.get_node_from_index(k_index)
 
 	# Initialize min_c.
 	min_c = float('inf')
 
 	# Initialize output dict.
 	best_cst_adjacent = {}
 
 	# Initialize dict of c_k(S, SI) values (keys = SI values).
 	c_SI = {}
 
-	# Set local_S: If S > external_outbound_cst[k], must pretend
-	# S = external_outbound_cst[k], otherwise stage thinks it can promise a
+	# Set local_S: If S > external_outbound_cst[k_index], must pretend
+	# S = external_outbound_cst[k_index], otherwise stage thinks it can promise a
 	# longer outbound CST than it really can.
 	# Note: external outbound CST defaults to BIG_INT if not provided.
-	local_S = min(S, node_k['external_outbound_cst'])
+	local_S = min(S, k.external_outbound_cst)
 
 	# Check whether S <= external outbound CST (otherwise this S is infeasible).
 	# Note that external outbound CST defaults to BIG_INT if not provided.
-	if S <= node_k['external_outbound_cst']:
+	if S <= k.external_outbound_cst:
 
-		# Loop through SI values between max(external inbound CST[k],
+		# Loop through SI values between max(external inbound CST[k_index],
 		# S - T_k) and M_k - T_k.
 		# Note that external inbound CST defaults to 0 if not provided.
-		lo_SI = max(node_k['external_inbound_cst'],
-					local_S - node_k['processing_time'])
-		hi_SI = node_k['max_replenishment_time'] - node_k['processing_time']
+		lo_SI = max(k.external_inbound_cst, local_S - k.processing_time)
+		hi_SI = k.max_replenishment_time - k.processing_time
 		for SI in range(lo_SI, hi_SI+1):
 
 			# Calculate c_k(S, SI).
 			c_SI[SI], stage_cost, best_upstream_S, best_downstream_SI = \
-				calculate_c(tree, k, local_S, SI, theta_in_partial, theta_out_partial)
+				_calculate_c(tree, k_index, local_S, SI, theta_in_partial, theta_out_partial)
 
 			# Compare to min.
 			if c_SI[SI] < min_c:
 				# Remember min cost and value of SI that attained it.
 				min_c = c_SI[SI]
-				best_cst_adjacent[k] = SI
+				best_cst_adjacent[k_index] = SI
 				# Remember values of other CSTs that attained min cost.
-				for i in range(np.min(tree.nodes), k):
-					if i in tree.predecessors(k):
+				for i in range(np.min(tree.node_indices), k_index):
+					if i in k.predecessor_indices():
 						best_cst_adjacent[i] = best_upstream_S[i]
-					elif i in tree.successors(k):
+					elif i in k.successor_indices():
 						best_cst_adjacent[i] = best_downstream_SI[i]
 
 	# Capture theta_out_k_S.
 	theta_out_k_S = min_c
 
 	return theta_out_k_S, best_cst_adjacent
 
 
-def calculate_theta_in(tree, k, SI, theta_in_partial, theta_out_partial):
-	"""Calculate the function theta_in(k, SI) as described in Section 6.3.6.2 of
-	Snyder and Shen (2019) [function g_i(SI) in Section 5 of Graves and Willems
+def _calculate_theta_in(tree, k_index, SI, theta_in_partial, theta_out_partial):
+	"""Calculate the function :math:`\\theta^i_k(SI)` as described in Section 6.3.6.2 of
+	|fosct| [function :math:`g_i(SI)` in Section 5 of Graves and Willems
 	(2003)].
 
 	Original function is modified in the following ways:
-	1. If SI is less than the external inbound CST for stage k,
-	theta_in(k, SI) is calculated as though SI = external inbound CST. (If k is a
-	source stage, theta_in(k,.) will never be calculated [theta_out(k,.) will be], but
-	k might have non-zero external inbound CST even if it is not a source stage.)
-	2. The demand bound demand bound over tau periods is assumed to be of the form
-	z_alpha * sigma * sqrt(tau).
-	3. When calculating c_k(S, SI), upstream nodes are allowed to use outbound
-	CSTs greater than SI, and downstream nodes are allowed to use inbound
-	CSTs greater than S. In effect, this allows multiple inbound/outbound
-	CSTs for a single nodes.
+	1. If :math:`SI` is less than the external inbound CST for stage :math:`k`,
+	:math:`\\theta^i_k(SI)` is calculated as though :math:`SI` = external inbound CST. (If :math:`k` is a
+	source stage, :math:`\\theta^i_k(\\cdot)` will never be calculated [:math:`\\theta^o_k(\\cdot)` will be], but
+	:math:`k` might have non-zero external inbound CST even if it is not a source stage.)
+	2. The demand bound demand bound over :math:`\\tau` periods is assumed to be of the form
+	:math:`z_\\alpha\\sigma\\sqrt{\\tau}`.
+	3. When calculating :math:`c_k(S, SI)`, upstream nodes are allowed to use outbound
+	CSTs greater than :math:`SI`, and downstream nodes are allowed to use inbound
+	CSTs greater than :math:`S`. In effect, this allows multiple inbound/outbound
+	CSTs for a single node.
 
 	Parameters
 	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
-		Tree must be pre-processed already.
-	k : int
+	tree : |class_network|
+		The multi-echelon tree network. Tree must be pre-processed already.
+	k_index : int
 		Index of node.
 	SI : int
 		Inbound committed service time.
 	theta_in_partial : dict
 		Dict of values of theta_in function that have been calculated so far
-		(i.e., for i < k).
+		(i.e., for :math:`i < k`).
 	theta_out_partial : dict
 		Dict of values of theta_out function that have been calculated so far
-		(i.e., for i < k).
+		(i.e., for :math:`i < k`).
 
 	Returns
 	-------
 	theta_in_k_SI : float
-		The value of theta_in(k, SI).
+		The value of :math:`\\theta^i_k(SI)`.
 	best_cst_adjacent : dict
-		Dict indicating, for each adjacent stage i with i <= k, the CST value
-		that minimized theta_in(.) for the optimal value of S.
-		* If i serves k, then best_CST_adjacent[i] = the value of S_i that
-		minimizes theta_out(i, S_i).
-		* If i is served by k, then best_CST_adjacent[i] = the value of SI_i
-		that minimizes theta_in(i, SI_i).
-		* If i = k, then best_CST_adjacent[i] = the best value of S chosen in
-		minimization of theta_in(.).
+		Dict indicating, for each adjacent stage :math:`i` with :math:`i \\le k`, the CST value
+		that minimized :math:`\\theta^i_i(\\cdot)` for the optimal value of S.
+		* If :math:`i` serves :math:`k`, then ``best_CST_adjacent[i]`` = the value of :math:`S_i` that
+		minimizes :math:`\\theta^o_i(S_i)`.
+		* If :math:`i` is served by :math:`k`, then ``best_CST_adjacent[i]`` = the value of :math:`SI_i`
+		that minimizes :math:`\\theta^i_i(SI_i)`.
+		* If :math:`i = k`, then ``best_CST_adjacent[i]`` = the best value of :math:`S` chosen in
+		minimization of :math:`theta^i(\\cdot)`.
 	"""
 
-	# Get node k, for convenience.
-	node_k = tree.nodes[k]
+	# Get node k_index, for convenience.
+	k = tree.get_node_from_index(k_index)
 
 	# Initialize min_c.
 	min_c = float('inf')
 
 	# Initialize output dict.
 	best_cst_adjacent = {}
 
 	# Initialize dict of c_k(S, SI) values (keys = S values).
 	c_S = {}
 
-	# Set local_SI: If SI < external_inbound_cst[k], must pretend
-	# SI = external_inbound_cst[k], otherwise stage thinks it can get a
+	# Set local_SI: If SI < external_inbound_cst[k_index], must pretend
+	# SI = external_inbound_cst[k_index], otherwise stage thinks it can get a
 	# shorter inbound CST than it really can.
 	# Note: external inbound CST defaults to 0 if not provided.
-	local_SI = max(SI, node_k['external_inbound_cst'])
+	local_SI = max(SI, k.external_inbound_cst)
 
-	# Loop through S values between 0 and min(SI + T_k, external outbound CST[k]).
+	# Loop through S values between 0 and min(SI + T_k, external outbound CST[k_index]).
 	# Note that external outbound CST defaults to BIG_INT if not provided.
 	lo_S = 0
-	hi_S = min(local_SI + node_k['processing_time'], node_k['external_outbound_cst'])
+	hi_S = min(local_SI + k.processing_time, k.external_outbound_cst)
 	for S in range(lo_S, hi_S+1):
 
 		# Calculate c_k(S, SI).
 		c_S[S], stage_cost, best_upstream_S, best_downstream_SI = \
-			calculate_c(tree, k, S, local_SI, theta_in_partial, theta_out_partial)
+			_calculate_c(tree, k_index, S, local_SI, theta_in_partial, theta_out_partial)
 
 		# Compare to min.
 		if c_S[S] < min_c:
 			# Remember min cost and value of S that attained it.
 			min_c = c_S[S]
-			best_cst_adjacent[k] = S
+			best_cst_adjacent[k_index] = S
 			# Remember values of other CSTs that attained min cost.
-			for i in range(np.min(list(tree.nodes)), k):
-				if i in tree.predecessors(k):
+			for i in range(np.min(tree.node_indices), k_index):
+				if i in k.predecessor_indices():
 					best_cst_adjacent[i] = best_upstream_S[i]
-				elif i in tree.successors(k):
+				elif i in k.successor_indices():
 					best_cst_adjacent[i] = best_downstream_SI[i]
 
 	# Capture theta_in_k_SI.
 	theta_in_k_SI = min_c
 
 	return theta_in_k_SI, best_cst_adjacent
 
 
-def calculate_c(tree, k, S, SI, theta_in_partial, theta_out_partial):
-	"""Calculate c_k(S,SI), the expected holding cost for N_k as function of
-	inbound and outbound CSTs at node_k k.
+def _calculate_c(tree, k_index, S, SI, theta_in_partial, theta_out_partial):
+	"""Calculate :math:`c_k(S,SI)`, the expected holding cost for :math:`N_k` as function of
+	inbound and outbound CSTs at node :math:`k`.
 
-	Assumes demand bound over tau periods is of the form
-	z_alpha * sigma * sqrt(tau).
-	# TODO: allow more general demand bound.
+	Assumes demand bound over :math:`\\tau` periods is of the form
+	:math:`z_\\alpha\\sigma\\sqrt{\\tau}`.
 
-	Upstream nodes are allowed to use outbound CSTs greater than SI and
-	downstream nodes are allowed to use inbound CSTs greater than S.
-	In effect, this allows multiple inbound/outbound CSTs for a single
-	node_k.
+	Upstream nodes are allowed to use outbound CSTs greater than :math:`SI` and
+	downstream nodes are allowed to use inbound CSTs greater than :math:`S`.
+	In effect, this allows multiple inbound/outbound CSTs for a single :math:`k`.
 
 	Parameters
 	----------
-	tree : graph
-		NetworkX directed graph representing the multi-echelon tree network.
-		Tree must be pre-processed already.
-	k : int
-		Index of node_k.
+	tree : |class_network|
+		The multi-echelon tree network. Tree must be pre-processed already.
+	k_index : int
+		Index of node.
 	S : int
 		Outbound committed service time.
 	SI : int
 		Inbound committed service time.
 	theta_in_partial : dict
-		Dict of values of theta_in function that have been calculated so far
-		(i.e., for i < k).
+		Dict of values of :math:`\\theta^i` function that have been calculated so far
+		(i.e., for :math:`i < k`).
 	theta_out_partial : dict
-		Dict of values of theta_out function that have been calculated so far
-		(i.e., for i < k).
+		Dict of values of :math:`\\theta^o` function that have been calculated so far
+		(i.e., for :math:`i < k`).
 
 	Returns
 	-------
 	cost : float
-		Value of c_k(S,SI).
+		Value of :math:`c_k(S,SI)`.
 	stage_cost : float
-		Cost to hold inventory at stage k (only) given CSTs of SI and S.
+		Cost to hold inventory at stage :math:`k` (only) given CSTs of :math:`SI` and :math:`S`.
 	best_upstream_S : dict
-		Dict indicating, for each i that is immediately upstream from k,
-		the best outbound CST for node_k i given k's CSTs of SI and S.
+		Dict indicating, for each :math:`i` that is immediately upstream from :math:`k`,
+		the best outbound CST for :math:`i` given :math:`k`'s CSTs of :math:`SI` and :math:`S`.
 	best_downstream_SI : dict
-		Dict indicating, for each i that is immediately downstream from k,
-		the best inbound CST for node_k i given k's CSTs of SI and S.
+		Dict indicating, for each :math:`i` that is immediately downstream from :math:`k`,
+		the best inbound CST for :math:`i` given :math:`k`'s CSTs of :math:`SI` and :math:`S`.
 	"""
 
 	# Get node k, for convenience.
-	node_k = tree.nodes[k]
+	k = tree.get_node_from_index(k_index)
 
 	# Initialize output dicts.
 	best_upstream_S = {}
 	best_downstream_SI = {}
 
 	# Calculate safety stock.
-	safety_stock = node_k['demand_bound_constant'] * \
-					node_k['net_demand_standard_deviation'] * \
-					np.sqrt(SI + node_k['processing_time'] - S)
+	safety_stock = k.demand_bound_constant * \
+					k.net_demand_standard_deviation * \
+					math.sqrt(SI + k.processing_time - S)
 
-	# Set stage_cost equal to holding cost at node_k k.
-	stage_cost = node_k['holding_cost'] * safety_stock
+	# Set stage_cost equal to holding cost at node k.
+	stage_cost = k.holding_cost * safety_stock
 
-	# Initialize cost to holding cost at node_k k.
+	# Initialize cost to holding cost at node k.
 	cost = stage_cost
 
-	# Add theta_out_partial(i) for nodes i that are immediately upstream from k
+	# Add theta_out_partial(i) for nodes i that are immediately upstream from k_index
 	# and have smaller index. (At this point, theta_out_partial(i) has already been
-	# calculated for i < k.)
-	for i in tree.predecessors(k):
-		if i < k:
+	# calculated for i < k_index.)
+	for i in k.predecessor_indices():
+		if i < k_index:
 			# Build dict of theta_out_partial(i, S2) values for S2 <= SI.
 			theta_out_values = {S2: theta_out_partial[i][S2] for S2 in range(SI + 1)}
 			# Find min value and argmin of theta_out_partial(i, S2) where S2 <= SI.
 			min_theta_out, best_upstream_S[i] = min_of_dict(theta_out_values)
 			# Add min value of theta_out_partial to cost.
 			cost += min_theta_out
 
-	# Add theta_in_partial(j) for nodes j that are immediately downstream from k
+	# Add theta_in_partial(j) for nodes j that are immediately downstream from k_index
 	# and have smaller index. (At this point, theta_in_partial(j) has already been
-	# calculated for j < k.)
-	for j in tree.successors(k):
-		if j < k:
+	# calculated for j < k_index.)
+	for j in k.successor_indices():
+		if j < k_index:
 			# Build dict of theta_in_partial(j, SI2) values for SI2 >= S.
 			theta_in_values = {SI2: theta_in_partial[j][SI2] for SI2 in
-							   range(S, tree.graph['max_max_replenishment_time'] + 1)}
+							   range(S, tree.max_max_replenishment_time + 1)}
 			# Find min value and argmin of theta_in_partial(i, SI2) for SI2 >= S.
 			min_theta_in, best_downstream_SI[j] = min_of_dict(theta_in_values)
 			# Add min value of theta_in_partial to cost.
 			cost += min_theta_in
 
 	return cost, stage_cost, best_upstream_S, best_downstream_SI
+
+
+### GRAPH MANIPULATION ###
+
+def preprocess_tree(tree):
+	"""Preprocess the GSM tree. Returns an independent copy.
+
+	If tree is already correctly labeled, does not relabel it.
+
+	Fill node-level attributes: ``net_demand_mean``,
+	``net_demand_standard_deviation``, ``larger_adjacent_node``,
+	``max_replenishment_time``.
+
+	Fill missing data for ``demand_bound_constant``, ``external_inbound_cst``, and
+	``external_outbound_cst attributes``.
+
+	Fill ``max_max_replenishment_time`` network-level attribute.
+
+	Parameters
+	----------
+	tree : |class_network|
+		The multi-echelon tree network. Current node labels are ignored and may be anything.
+	start_index : int, optional
+		Integer to use as starting (smallest) node label.
+
+	Returns
+	-------
+	new_tree : |class_network|
+		Pre-processed multi-echelon tree network.
+
+	"""
+
+	new_tree = copy.deepcopy(tree)
+
+	# Fill external inbound and outbound CST parameters, if not provided.
+	# Default value of external outbound CST = BIG_INT.
+	# Default value of external inbound CST = 0. (Not strictly necessary,
+	# but cleaner.)
+	for k in new_tree.nodes:
+		if k.external_inbound_cst is None:
+			k.external_inbound_cst = 0
+		if k.external_outbound_cst is None:
+			k.external_outbound_cst = BIG_INT
+
+	# Fill demand bound constant parameters, if not provided.
+	# Set equal to demand bound constant of sink node. If more than one sink node,
+	# one is chosen arbitrarily. If no sink nodes have demand bound constant,
+	# constant is set to 1.
+	sinks_with_dbc = [k for k in new_tree.sink_nodes if k.demand_bound_constant is not None]
+	for k in new_tree.nodes:
+		if k.demand_bound_constant is None:
+			if sinks_with_dbc == []:
+				k.demand_bound_constant = 1
+			else:
+				k.demand_bound_constant = \
+					sinks_with_dbc[0].demand_bound_constant
+
+	# Calculate net demand parameters.
+	net_demand_means, net_demand_standard_deviations = _net_demand(new_tree)
+	for k in new_tree.nodes:
+		k.net_demand_mean = net_demand_means[k.index]
+		k.net_demand_standard_deviation = net_demand_standard_deviations[k.index]
+
+	# Calculate max replenishment times.
+	max_replenishment_times = _longest_paths(new_tree)
+	for k in new_tree.nodes:
+		k.max_replenishment_time = max_replenishment_times[k.index]
+
+	# Calculate maximum value of max_replenishment_time.
+	new_tree.max_max_replenishment_time = \
+		np.max([k.max_replenishment_time for k in new_tree.nodes])
+
+	return new_tree
+
+
+def relabel_nodes(tree, start_index=0, force_relabel=False):
+	"""Perform the node-labeling algorithm described in Section 5 of Graves and
+	Willems (2000).
+
+	If tree is already correctly labeled, returns the original tree,
+	unless ``force_relabel`` is ``True``, in which case performs the relabeling.
+
+	Does not modify the input tree. Fills ``original_label``,
+	``larger_adjacent_node``, and ``larger_adjacent_node_is_downstream`` attributes
+	of nodes in new tree, whether or not original tree was already
+	correctly labeled.
+
+	Parameters
+	----------
+	tree : |class_network|
+		The multi-echelon tree network.
+		Current node labels are ignored (unless the tree is already correctly
+		labeled) and may be anything.
+	start_index : int, optional
+		Integer to use as starting (smallest) node label.
+	force_relabel : bool, optional
+		If ``True``, function will relabel nodes even if original tree is correctly
+		labeled.
+
+	Returns
+	-------
+	relabeled_tree : |class_network|
+		The relabeled tree network.
+
+	"""
+
+	# Check whether tree is already correctly labeled.
+	is_correct = is_correctly_labeled(tree)
+
+	# Do relabel?
+	if is_correct and not force_relabel:
+		relabeled_tree = copy.deepcopy(tree)
+		new_labels = {k.index: k.index for k in tree.nodes}
+	else:
+
+		# Initialize all nodes to "unlabeled", and initialize list of new labels.
+		labeled = {i.index: False for i in tree.nodes}
+		new_labels = {}
+
+		# Find nodes that are adjacent to at most 1 unlabeled node and label them.
+		for k_index in range(start_index, start_index+len(tree.nodes)):
+
+			# Find a node for labeling.
+			for i in tree.nodes:
+
+				# Make sure i is unlabeled.
+				if not labeled[i.index]:
+					# Count unlabeled nodes that are adjacent to node i.
+					num_adj = len([j for j in i.neighbor_indices if not labeled[j]])
+
+					# If i is adjacent to at most 1 unlabeled node, label it.
+					if num_adj <= 1:
+						# Change i's label to k_index.
+						new_labels[i.index] = k_index
+						# Mark i as labeled.
+						labeled[i.index] = True
+						# Break out of 'for i' loop
+						break
+
+		# Relabel the nodes
+		relabeled_tree = copy.deepcopy(tree)
+		relabeled_tree.reindex_nodes(new_labels)
+
+	# Fill attributes of relabeled tree.
+	larger_adjacent, downstream = _find_larger_adjacent_nodes(relabeled_tree)
+	for k in tree.nodes:
+		relabeled_node = relabeled_tree.get_node_from_index(new_labels[k.index])
+		relabeled_node.original_label = k.index
+		if new_labels[k.index] < np.max(list(new_labels.values())):
+			relabeled_node.larger_adjacent_node = larger_adjacent[relabeled_node.index]
+			relabeled_node.larger_adjacent_node_is_downstream = downstream[relabeled_node.index]
+		else:
+			# Largest-indexed node has no larger adjacent node.
+			relabeled_node.larger_adjacent_node = None
+			relabeled_node.larger_adjacent_node_is_downstream = None
+
+	return relabeled_tree
+
+
+def is_correctly_labeled(tree):
+	"""Determine whether tree is already correctly labeled.
+
+	Tree is correctly labeled if all labels are consecutive integers and
+	every stage (other than the highest-indexed one) has
+	exactly one adjacent stage with a greater index.
+
+	Parameters
+	----------
+	tree : |class_network|
+		The multi-echelon tree network.
+
+	Returns
+	-------
+	``True`` if tree is already correctly labeled.
+	"""
+
+	# Get indices.
+	ind = tree.node_indices
+
+	# Check whether labels are consecutive integers starting at min_index.
+	min_index = np.min(ind)
+	try:
+		if set(ind) != set(range(min_index, min_index + len(ind))):
+			is_correct = False
+		else:
+			# Check whether every node has exactly one adjacent node with
+			# greater index.
+			is_correct = True
+			for k in tree.nodes:
+				if k.index < np.max(ind):
+					greater_indexed_neighbors = \
+						{i_ind for i_ind in k.predecessor_indices() if i_ind > k.index}.union(
+							{i_ind for i_ind in k.successor_indices() if i_ind > k.index}
+						)
+					if len(greater_indexed_neighbors) != 1:
+						is_correct = False
+	except:
+		is_correct = False
+
+	return is_correct
+
+
+def _find_larger_adjacent_nodes(tree):
+	"""Find larger-indexed adjacent node, for each node in tree.
+
+	After the nodes are relabeled by :func:`relabel_nodes`, each node (except the
+	node with the largest index) is adjacent to exactly one node with a
+	larger index. Node :math:`k`'s neighbor with larger index is denoted :math:`p(k)` in
+	Graves and Willems (2000). This function finds :math:`p(k)` for all :math:`k` and also
+	indicates whether :math:`p(k)` is upstream or downstream from :math:`k`.
+
+	Parameters
+	----------
+	tree : |class_network|
+		The multi-echelon tree network.
+		Nodes are assumed to have been relabeled using :func:`relabel_nodes`.
+
+	Returns
+	-------
+	larger_adjacent: dict
+		Dict containing index of each node's larger-indexed adjacent node,
+		for all nodes except the largest-indexed node. Keys are node indices.
+	downstream: dict
+		Dict containing, for each node, ``True`` if the larger-indexed adjacent
+		node is downstream from the node, ``False`` if it is upstream, for all
+		nodes except the largest-indexed node. Keys are node indices.
+	"""
+
+	# Initialize dicts.
+	larger_adjacent = {}
+	downstream = {}
+
+	# Loop through nodes.
+	for k in tree.nodes:
+		if k.index < np.max(tree.node_indices):
+			# Get list of nodes that are adjacent to k and have a larger index,
+			# but the list will only contain a single item; set larger_adjacent[k_index] to it.
+			larger_adjacent_list = [i.index for i in k.neighbors if i.index > k.index]
+			larger_adjacent[k.index] = larger_adjacent_list[0]
+
+			# Set downstream flag.
+			if larger_adjacent[k.index] in k.successor_indices():
+				downstream[k.index] = True
+			else:
+				downstream[k.index] = False
+
+	return larger_adjacent, downstream
+
+
+def _longest_paths(tree):
+	"""Determine the length of the longest path from any source node to to each
+	node :math:`k`.
+
+	Arc lengths are determined by processing times. External inbound CSTs are
+	considered source nodes, so having an external inbound CST at node :math:`i` of 5 is
+	like having another node that serves node :math:`i` with a processing time of 5.
+
+	Parameters
+	----------
+	tree : |class_network|
+		The multi-echelon tree network.
+		Nodes are assumed to have been relabeled using :func:`relabel_nodes`.
+
+	Returns
+	-------
+	longest_lengths : dict
+		Dict of longest paths to each node, with keys equal to node indices. [:math:`M_k`].
+
+	"""
+
+	# Build the tree as networkx DiGraph. Set the weight of each edge into a given node k to the processing
+	# time of node k. If node k is a source node and/or it has an external inbound CST,
+	# add a dummy node before node k and set weight of edge from dummy node to node k
+	# equal to processing time of node k + external inbound CST for node k.
+	temp_tree = tree.networkx_digraph()
+	for k in tree.nodes:
+		for p in k.predecessors():
+			temp_tree[p.index][k.index]['weight'] = k.processing_time
+		if temp_tree.in_degree(k.index) == 0 or (k.external_inbound_cst or 0) > 0:
+			temp_tree.add_edge('dummy_' + str(k.index), k.index,
+				weight=k.processing_time + (k.external_inbound_cst or 0))
+
+	# Determine shortest path between every pair of nodes.
+	# (Really there's only one path, but shortest path is the
+	# most straightforward algorithm to use here.)
+	path_lengths = dict(nx.shortest_path_length(temp_tree, weight='weight'))
+
+	# Determine longest shortest path to each node k, among all
+	# source nodes that are ancestors to k.
+	longest_lengths = {}
+	for k in tree.nodes:
+		longest_lengths[k.index] = max([path_lengths[i][k.index] for i in
+								  nx.ancestors(temp_tree, k.index)], default=0)
+
+	return longest_lengths
+
+
+def _net_demand(tree):
+	"""Calculate net demand mean and standard deviation for all nodes in tree.
+
+	Net demand is the demand stream consisting of the external demand for the
+	node plus all downstream demand.
+
+	Parameters
+	----------
+	tree : |class_network|
+		The multi-echelon tree network.
+
+	Returns
+	-------
+	net_means : dict
+		Dict of net mean for each node.
+
+	net_standard_deviations : dict
+		Dict of net standard deviation for each node.
+
+	"""
+
+	# Initialize net_mean and net_variances using each node's external demand.
+	net_means = {k.index: k.demand_source.mean or 0 for k in tree.nodes}
+	net_variances = {k.index: (k.demand_source.standard_deviation or 0)**2 for k in tree.nodes}
+
+	# Make temp copy of tree.
+	temp_tree = copy.deepcopy(tree)
+
+	# Loop through temp_tree. At each iteration, handle leaf nodes (nodes with
+	# no _successors), adding their net_means and net_variances to those of their
+	# _predecessors. Then remove the leaf nodes and iterate.
+	while len(temp_tree.nodes) > 0:
+		leaf_nodes = temp_tree.sink_nodes
+		for k in leaf_nodes:
+			for i in k.predecessor_indices():
+				net_means[i] += net_means[k.index]
+				net_variances[i] += net_variances[k.index]
+			temp_tree.remove_node(k) 
+
+	net_standard_deviations = {k.index: math.sqrt(net_variances[k.index]) for k in tree.nodes}
+	return net_means, net_standard_deviations
+
+
+def _connected_subgraph_nodes(tree):
+	"""Determine nodes connected to :math:`k` in subgraph on :math:`\\{\\min_k,\\ldots,k\\}`, 
+	for each :math:`k`, where :math:`\\min_k` is smallest index in graph. [:math:`N_k`]
+
+	"Connected" does not necessarily mean "adjacent."
+
+	Parameters
+	----------
+	tree : |class_network|
+		The multi-echelon tree network.
+
+	Returns
+	-------
+	connected_nodes : dict
+		Dict of set of connected subgraph nodes for each node.
+
+	"""
+
+	# Intiailize output dict.
+	connected_nodes = {}
+
+	# Convert to networkx DiGraph so we can use subgraph().
+	networkx_tree = tree.networkx_digraph()
+
+	# Loop through nodes.
+	for k in networkx_tree:
+		# Build subgraph on {min_k,...,k}.
+		subgraph = networkx_tree.to_undirected().subgraph(range(np.min(networkx_tree.nodes), k+1))
+		# Build set of connected nodes.
+		connected_nodes[k] = set(i for i in subgraph.nodes if
+							  nx.has_path(subgraph, i, k))
+
+	return connected_nodes
+
+
+def gsm_to_ssm(tree, p=None):
+	"""Convert GSM tree to SSM tree:
+	
+		- Convert local to echelon holding costs.
+		- Convert processing times to lead times.
+		- Include stockout cost at demand nodes (if provided).
+
+	Tree must be pre-processed before calling.
+
+	Parameters
+	----------
+	tree : |class_network|
+		The multi-echelon tree network.
+	p : float or dict, optional
+		Stockout cost to use at demand nodes, or dict indicating stockout cost
+		for each demand node. If ``None``, copies ``stockout_cost``
+		field from tree for nodes that have it, and does not fill ``stockout_cost``
+		for nodes that do not.
+
+	Returns
+	-------
+	SSM_tree : |class_network|
+		SSM representation of tree.
+	"""
+
+	# Build new graph.
+	SSM_tree = SupplyChainNetwork()
+
+	# Add nodes.
+	for n in tree.nodes:
+		upstream_h = np.sum([k.local_holding_cost for k in n.predecessors()])
+		SSM_tree.add_node(SupplyChainNode(n.index, name=n.name, network=SSM_tree,
+			shipment_lead_time=n.processing_time+n.external_inbound_cst,
+			echelon_holding_cost=n.local_holding_cost-upstream_h))
+		SSM_node = SSM_tree.get_node_from_index(n.index)
+		SSM_node.demand_source = copy.deepcopy(n.demand_source)
+		if p is not None:
+			if n.demand_source is not None:
+				if isinstance(p, dict):
+					SSM_node.stockout_cost = p[SSM_node.index]
+				else:
+					SSM_node.stockout_cost = p
+		else:
+			if n.stockout_cost is not None:
+				SSM_node.stockout_cost = n.stockout_cost
+
+	# Add edges.
+	edge_list = tree.edges
+	SSM_tree.add_edges_from_list(edge_list)
+
+	return SSM_tree
+
+
```

### Comparing `stockpyl-0.1.0a0/stockpyl/ssm_serial.py` & `stockpyl-1.0.0/src/stockpyl/ssm_serial.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,115 +1,160 @@
 # ===============================================================================
 # stockpyl - ssm_serial Module
 # -------------------------------------------------------------------------------
-# Version: 0.0.0
-# Updated: 01-30-2022
 # Author: Larry Snyder
 # License: GPLv3
 # ===============================================================================
 
-"""The :mod:`ssm_serial` module contains code to implement Chen-Zheng (1994) algorithm 
-for stochastic serial systems under the stochastic service model (SSM), based on 
-Clark and Scarf (1960), as described in Snyder and Shen (2019).
-
-'node' and 'stage' are used interchangeably in the documentation.
-
-The notation and references (equations, sections, examples, etc.) used below
-refer to Snyder and Shen, *Fundamentals of Supply Chain Theory*, 2nd edition
-(2019).
+"""
+.. include:: ../../globals.inc
+
+Overview 
+--------
+
+The |mod_ssm_serial| module contains code to solve serial systems under the stochastic service
+model (SSM), either exactly, using the :func:`~stockpyl.ssm_serial.optimize_base_stock_levels` function
+(which implements the algorithm by Chen and Zheng (1994), which in turn is
+based on the algorithm by Clark and Scarf (1960)), or approximately, using the :func:`~stockpyl.ssm_serial.newsvendor_heuristic` 
+function (which implements the newsvendor heuristic by Shang and Song (2003)).
+
+.. note:: |node_stage|
+
+.. note:: |fosct_notation|
+
+
+.. seealso::
+
+	For an overview of multi-echelon inventory optimization in |sp|,
+	see the :ref:`tutorial page for multi-echelon inventory optimization<tutorial_meio_page>`.
+
 
 References
 ----------
 F. Chen and Y. S. Zheng. Lower bounds for multiechelon stochastic inventory systems. *Management Science*, 40(11):1426–1443, 1994.
 
 A. J. Clark and H. Scarf. Optimal policies for a multiechelon inventory problem. *Management Science*, 6(4):475–490, 1960.
+
+K. H. Shang and J.-S. Song. Newsvendor bounds and heuristic for optimal policies in serial supply chains. *Management Science*, 49(5):618-638, 2003.
+
+
+API Reference
+-------------
+
 """
 
-from multiprocessing.sharedctypes import Value
 import numpy as np
 from scipy import stats
 #import math
 import matplotlib.pyplot as plt
 import copy
 
 from stockpyl.demand_source import DemandSource
-from stockpyl.helpers import *
-#from stockpyl.supply_chain_network import *
+from stockpyl.helpers import round_dict_values
 from stockpyl.newsvendor import *
+from stockpyl.supply_chain_network import serial_system
 
 
 ### OPTIMIZATION ###
 
-def optimize_base_stock_levels(num_nodes=None, echelon_holding_cost=None, lead_time=None,
-								stockout_cost=None, demand_mean=None, demand_standard_deviation=None,
+def optimize_base_stock_levels(num_nodes=None, node_order_in_system=None, node_order_in_lists=None,
+								echelon_holding_cost=None, lead_time=None, stockout_cost=None, 
+								demand_mean=None, demand_standard_deviation=None,
 								demand_source=None, network=None,
 								S=None, plots=False, x=None,
 								x_num=1000, d_num=100,
 								ltd_lower_tail_prob=1-stats.norm.cdf(4),
 								ltd_upper_tail_prob=1-stats.norm.cdf(4),
 								sum_ltd_lower_tail_prob=1-stats.norm.cdf(4),
-								sum_ltd_upper_tail_prob=1-stats.norm.cdf(8)):
-	"""Chen-Zheng (1994) algorithm for stochastic serial systems under
-	stochastic service model (SSM), as described in Snyder and Shen (2019).
+								sum_ltd_upper_tail_prob=1-stats.norm.cdf(4)):
+	"""Chen-Zheng (1994) algorithm for stochastic serial systems under the stochastic service model (SSM), which in 
+	turn is based on Clark and Scarf (1960). 
 
 	Problem instance may either be provided in the individual parameters ``num_nodes``, ..., ``demand_source``,
-	or in the ``network`` parameter.
+	or as a |class_network| in the ``network`` parameter.
+
+	By default, the nodes in the system are assumed to be indexed
+	``num_nodes``, ..., 1, with node 1 at the downstream end, but this can be changed by
+	providing either the ``node_order_in_system`` or ``network`` parameter.
 
-	The nodes must be indexed :math:`N, \\ldots, 1`. The node-specific
-	parameters (``echelon_holding_cost`` and ``lead_time``) must be either 
-	a dict, a list, or a singleton, with the following requirements:
+	The node-specific parameters (``echelon_holding_cost``, ``lead_time``)
+	must be either a dict, a list, or a singleton, with the following requirements:
 	
-	* If the parameter is a dict, its keys must equal 1,..., ``num_nodes``,
-	  each corresponding to a node index.
-	* If the parameter is a list, it must have length ``num_nodes`` + 1;
-	  the 0th entry will be ignored and the other entries will correspond to the node indices.
-	* If the parameter is a singleton, all nodes will have that parameter set to the
-	  singleton value.
+	* If the parameter is a dict, then the keys must contain the node indices and the values
+	  must contain the corresponding attribute values. If a given node index is contained in
+	  ``node_order_in_system`` (or in 1, ..., ``num_nodes``, if ``node_order_in_system`` is not
+	  provided) but is not a key in the dict, the attribute value is set to ``None`` for that node.
+	* If the parameter is a singleton, then the attribute is set to that value for all nodes.
+	* If the parameter is a list and ``node_order_in_lists`` is provided, ``node_order_in_lists`` 
+	  must contain the same indices as ``node_order_in_system`` (if it is provided) or 1, ..., ``num_nodes``
+	  (if it is not), otherwise a ``ValueError`` is raised. The values in the list are assumed
+	  to correpond to the node indices in the order they are specified in ``node_order_in_lists``.
+	  That is, the value in slot ``k`` in the parameter list is assigned to the node with index
+	  ``node_order_in_lists[k]``. 
+	* If the parameter is a list and ``node_order_in_lists`` is not provided, the values
+	  in the list are assumed to correspond to nodes in the same order as ``node_order_in_system``
+	  (or in ``num_nodes``, ..., 1, if ``node_order_in_system`` is not provided).
+	
+	(These are the same requirements as in :func:`stockpyl.supply_chain_network.serial_system`, except
+	that the default node numbering is ``num_nodes``, ..., 1 here.)
 
 	Either ``demand_mean`` and ``demand_standard_deviation`` must be
-	provided (in which case the demand will be assumed to be normally distributed)
-	or a ``demand_source`` must be provided.
+	provided (in which case the demand will be assumed to be normally distributed),
+	or ``demand_source`` must be provided, or ``network`` must be provided.
 
+	If ``demand_source`` is provided and has all-integer support, this is accounted for
+	in the discretization, and the solutions returned will also be integer.
 
 	Parameters
 	----------
 	num_nodes : int, optional
 		Number of nodes in serial system. [:math:`N`]
+	node_order_in_system : list, optional
+		List of node indices in the order that they appear in the serial system,
+		with upstream-most node listed first. If omitted, the system will be indexed
+		``num_nodes``, ..., 1. Ignored if ``network`` is provided.
+	node_order_in_lists : list, optional
+		List of node indices in the order in which the nodes are listed in any
+		attributes that are lists. (``node_order_in_lists[k]`` is the index of the ``k`` th node.)
+		Ignored if ``network`` is provided.
 	echelon_holding_cost : float, list, or dict, optional
 		Echelon holding cost at each node. [:math:`h`]
 	lead_time : float, list, or dict, optional
 		(Shipment) lead time at each node. [:math:`L`]
 	stockout_cost : float, optional
 		Stockout cost per item per unit time at node 1. [:math:`p`]
 	demand_mean : float, optional
 		Mean demand per unit time at node 1. Ignored if ``demand_source`` is not ``None``. [:math:`\\mu`]
 	demand_standard_deviation : float, optional
-		Standard deviation of demand per unit time at node 1. Ignored if ``demand_source`` is not ``None``. [:math:`\\mu`]
-	demand_source : DemandSource, optional
-		A DemandSource object describing the demand distribution. Required if
+		Standard deviation of demand per unit time at node 1. Ignored if ``demand_source`` is not ``None``. [:math:`\\sigma`]
+	demand_source : |class_demand_source|, optional
+		A |class_demand_source| object describing the demand distribution. Required if
 		``demand_mean`` and ``demand_standard_deviation`` are ``None``.
-	network : SupplyChainNetwork, optional
-		A SupplyChainNetwork object that provides all of the necessary data. If provided,
+	network : |class_network|, optional
+		A |class_network| object that provides all of the necessary data. If provided,
 		``num_nodes``, ..., ``demand_source`` are ignored.
 	S : dict, optional
 		Dict of echelon base-stock levels to evaluate. If present, no
 		optimization is performed and the function just returns the cost
 		under base-stock levels ``S``; to optimize instead, set ``S`` = ``None``
 		(the default). [:math:`S`]
 	plots : bool, optional
 		``True`` for the function to generate plots of :math:`C(\\cdot)` functions,
 		``False`` otherwise.
 	x : ndarray, optional
 		x-array to use for truncation and discretization, or ``None`` (the default)
 		to determine automatically.
 	x_num : int, optional
 		Number of discretization intervals to use for ``x`` range. Ignored if
-		``x`` is provided.
+		``x`` is provided. Ignored if a discrete distribution is provided in
+		``demand_source`` (since in that case ``x`` range is discretized to integers).
 	d_num : int, optional
-		Number of discretization intervals to use for ``d`` range.
+		Number of discretization intervals to use for ``d`` range. 
+		Ignored if a discrete distribution is provided in
+		``demand_source`` (since in that case ``d`` range is discretized to integers).
 	ltd_lower_tail_prob : float, optional
 		Lower tail probability to use when truncating lead-time demand
 		distribution.
 	ltd_upper_tail_prob : float, optional
 		Upper tail probability to use when truncating lead-time demand
 		distribution.
 	sum_ltd_lower_tail_prob : float, optional
@@ -127,14 +172,16 @@
 		Optimal expected cost. [:math:`C^*`]
 
 	Raises
 	------
 	ValueError
 		If ``network`` is ``None`` and ``num_nodes``, ..., ``stockout_cost`` are ``None``.
 	ValueError
+		If ``network``, ``node_order_in_system``, and ``num_nodes`` are all ``None``.
+	ValueError
 		If ``stockout_cost`` is ``None`` or if ``echelon_holding_cost`` or
 		``lead_time`` is ``None`` for any node.
 	ValueError
 		If ``demand_mean`` or ``demand_standard_deviation`` is ``None`` and 
 		``demand_source`` is ``None``.
 	ValueError
 		If ``stockout_cost`` < 0 or if ``lead_time`` < 0 for any node.
@@ -168,86 +215,59 @@
 		\\begin{gather*}
 		\\lim_{x \\rightarrow -\\infty} \\hat{g}_j(x) = \\sum_{i=1}^j h_i\\left(x - \\sum_{k=i}^{j-1} E[D_k]\\right) - (p+h'_1)\\left(x - \\sum_{k=1}^{j-1} E[D_k]\\right) \\\\
 		\\lim_{x \\rightarrow +\\infty} \\hat{g}_j(x) = \\begin{cases} h_jx + g_{j-1}(S^*_{j-1}), & \\text{if $j>1$} \\\\
 															h_jx, & \\text{if $j=1$} \\end{cases}
 		\\end{gather*}
 
 
+	References
+	----------
+	F. Chen and Y. S. Zheng. Lower bounds for multiechelon stochastic inventory systems. *Management Science*, 40(11):1426–1443, 1994.
+
+	A. J. Clark and H. Scarf. Optimal policies for a multiechelon inventory problem. *Management Science*, 6(4):475–490, 1960.
+
+
 	**Example** (Example 6.1):
 
 	.. testsetup:: *
 
 		from stockpyl.ssm_serial import *
 
 	.. doctest::
+		:skipif: True	# set to False to run the test
 
 		>>> S_star, C_star = optimize_base_stock_levels(
 		... 	num_nodes=3, 
-		... 	echelon_holding_cost=[3, 2, 2], 
-		... 	lead_time=[1, 1, 2], 
+		... 	echelon_holding_cost=[2, 2, 3], 
+		... 	lead_time=[2, 1, 1], 
 		... 	stockout_cost=37.12, 
 		... 	demand_mean=5, 
 		... 	demand_standard_deviation=1
 		...	)
 		>>> S_star
-		{1: 6.5144388073261155, 2: 12.012332294949644, 3: 22.700237234889784}
+		{3: 22.700237234889784, 2: 12.012332294949644, 1: 6.5144388073261155}
 		>>> C_star
 		47.668653127136345
 	"""
 
-	# TODO: handle other indexing (other than N ... 1)
-
-	# Check for presence of data.
-	if network is None and (num_nodes is None or echelon_holding_cost is None or \
-		lead_time is None or stockout_cost is None):
-		raise ValueError("You must provide either network or num_nodes, ..., stockout_cost")
-
-	# Convert network to parameters, if network provided.
-	if network:
-		num_nodes = len(network.nodes)
-		echelon_holding_cost = {node.index: node.echelon_holding_cost for node in network.nodes}
-		lead_time = {node.index: node.lead_time for node in network.nodes}
-		stockout_cost = network.get_node_from_index(1).stockout_cost
-		demand_source = network.get_node_from_index(1).demand_source
-
-	# Build dicts of parameters.
-	indices = list(range(1, num_nodes+1))
-	echelon_holding_cost_dict = ensure_dict_for_nodes(echelon_holding_cost, indices)
-	lead_time_dict = ensure_dict_for_nodes(lead_time, indices, 0)
-	stockout_cost_dict = {n: stockout_cost if n == 1 else 0 for n in indices}
-	
-	# Validate parameters.
-	if not all(echelon_holding_cost_dict.values()): raise ValueError("echelon_holding_cost cannot be None for any node")
-	if not all(lead_time_dict.values()): raise ValueError("lead_time cannot be None for any node")
-	if any(l < 0 for l in lead_time_dict.values()): raise ValueError("lead_time must be non-negative for every node")
-	if stockout_cost is None: raise ValueError("stockout_cost cannot be None")
-	elif stockout_cost < 0: raise ValueError("stockout_cost must be non-negative")
-	if (demand_mean is None or demand_standard_deviation is None) and demand_source is None:
-		raise ValueError("You must provide either demand_mean and demand_standard_deviation, or demand_source")
+	# Validate data and re-index to N, ..., 1.
+	old_to_new_dict, num_nodes, echelon_holding_cost_dict, lead_time_dict, stockout_cost, demand_source \
+		= _preprocess_parameters(num_nodes, node_order_in_system, node_order_in_lists, echelon_holding_cost,
+		lead_time, stockout_cost, demand_mean, demand_standard_deviation, demand_source, network)
 
 	# Get shortcuts to some parameters (for convenience).
 	N = num_nodes
-	if demand_source is None:
-		mu = demand_mean
-	else:
-		mu = demand_source.demand_distribution.mean()
+	mu = demand_source.demand_distribution.mean()
 	L = [0] + [lead_time_dict[j] for j in range(1, N+1)]
 	h = [0] + [echelon_holding_cost_dict[j] for j in range(1, N+1)]
 	p = stockout_cost
 
 	# Build "sum of lead-time demand" distribution (LTD distribution in
 	# which L = sum of all lead times)
-	if demand_source is None:
-		demand_source = DemandSource()
-		demand_source.type = 'N'
-		demand_source.mean = demand_mean
-		demand_source.standard_deviation = demand_standard_deviation
-	sum_ltd_dist = demand_source.lead_time_demand_distribution(float(np.sum(L)))
-
-	# TODO: would it be better to calculate mean, a, b directly if we know them?
+	sum_ltd_dist = demand_source.lead_time_demand_distribution(sum(L))
 
 	# Get truncation bounds for sum-of-lead-time demand distribution.
 	# If support is finite, use support; otherwise, use F^{-1}(.).
 	if sum_ltd_dist.a == float("-inf"):
 		sum_ltd_lo = sum_ltd_dist.ppf(sum_ltd_lower_tail_prob)
 	else:
 		# interval(1) gives lo and hi end of interval that contains 100% of
@@ -255,49 +275,69 @@
 		# distribution is the entire support.
 		sum_ltd_lo = sum_ltd_dist.interval(1)[0]
 	if sum_ltd_dist.b == float("inf"):
 		sum_ltd_hi = sum_ltd_dist.ppf(1 - sum_ltd_upper_tail_prob)
 	else:
 		sum_ltd_hi = sum_ltd_dist.interval(1)[1]
 
+	# Is demand distribution discrete (integer)?
+	if demand_source.type in ('P', 'UD'):
+		discrete_distribution = True
+	elif demand_source.type == 'CD' and np.all([is_integer(d) for d in demand_source.demand_list]):
+		discrete_distribution = True
+	else:
+		discrete_distribution = False
+
 	# Determine x (inventory level) array (truncated and discretized).
+	# If demand distribution is discrete, discretize to integers; otherwise,
+	# use x_num to determine granularity.
 	if x is None:
-		# TODO: is this the best x-range to use?
 		# x-range = [sum_ltd_lo-sum_ltd_mean, sum_ltd_hi].
-		x_lo = sum_ltd_lo - sum_ltd_dist.mean()
+		x_lo = sum_ltd_lo - sum_ltd_hi # originally used sum_ltd_dist.mean() here but I think sum_ltd_hi is more accurate
 		x_hi = sum_ltd_hi
-		x_delta = (x_hi - x_lo) / x_num
-		# x_lo = -4 * sigma * np.sqrt(sum(L))
-		# x_hi = mu * sum(L) + 8 * sigma * np.sqrt(sum(L))
-		# x_delta = (x_hi - x_lo) / x_num
 		# Ensure x >= largest echelon BS level, if provided.
 		if S is not None:
-			x_hi = max(x_hi, max(S, key=S.get))
-		# Build x range.
-		x = np.arange(x_lo, x_hi + x_delta, x_delta)
+			x_hi = max(x_hi, max(S.values()))
+		# Build x range. Is demand distribution discrete?
+		if discrete_distribution:
+			# x_lo and h_hi should already be integers, but cast them anyway.
+			x_lo    = round(x_lo)
+			x_delta = int(1)
+			x_num   = round(x_hi-x_lo)
+		elif x_num and x_hi > x_lo:
+			x_lo    = float(x_lo)
+			x_delta = float((x_hi-x_lo)/x_num)
+		else:
+			x_lo    = float((x_lo+x_hi)*0.5)
+			x_delta = float(1)
+			x_num   = int()
+		x_hi = x_num*x_delta+x_lo
+		x = np.array([x_ind*x_delta+x_lo for x_ind in range(x_num+1)])
+	elif x.size > 1:
+		x_lo    = np.min(x)
+		x_hi    = np.max(x)
+		x_delta = abs(x[1]-x[0])
+		x_num   = int((x_hi-x_lo)/x_delta)
 	else:
-		x_delta = x[1] - x[0]
-
-	# Standard normal demand array (truncated and discretized).
-	# (Use mu + d * sigma to get distribution-specific demand_list).
-	# d_lo = -4
-	# d_hi = 4
-	# d_delta = (d_hi - d_lo) / d_num
-	# d = np.arange(d_lo, d_hi + d_delta, d_delta)
-	# # Probability array.
-	# fd = stats.norm.cdf(d+d_delta/2) - stats.norm.cdf(d-d_delta/2)
+		x_lo    = x[0]
+		x_hi    = x_lo
+		x_delta = int(1)
+		x_num   = int()
 
 	# Extended x array (used for approximate C-hat function).
-	x_ext_lo = np.min(x) - sum_ltd_hi
-	x_ext_hi = np.max(x) + sum_ltd_hi
+	x_ext_num = math.ceil(sum_ltd_hi/x_delta)
 	# x_ext_lo = np.min(x) - (mu * sum(L) +
 	# 						d.max() * sigma * np.sqrt(sum(L)))
 	# x_ext_hi = np.max(x) + (mu * sum(L) +
 	# 						d.max() * sigma * np.sqrt(sum(L)))
-	x_ext = np.arange(x_ext_lo, x_ext_hi, x_delta)
+	x_ext = np.array([x_ext_ind*x_delta+x_lo for x_ext_ind in range(-x_ext_num, x_num+x_ext_num+1)])
+
+	# Index dictionaries to find nearest entry for matching value faster
+	index_x     = {x    [ind]: ind for ind in range(x    .size)}
+	index_x_ext = {x_ext[ind]: ind for ind in range(x_ext.size)}
 
 	# Initialize arrays. (0th element is ignored since we are assuming stages
 	# are numbered starting at 1. C_bar is an exception since C_bar[0] is
 	# meaningful.)
 	C_hat = np.zeros((N+1, len(x)))
 	C = np.zeros((N+1, len(x)))
 	S_star = {}
@@ -320,162 +360,201 @@
 		# Calculate approximate C-hat function.
 		C_hat_lim1[j, :] = -(p + sum(h)) * (x_ext - mu * sum(L[1:j]))
 		for i in range(1, j+1):
 			C_hat_lim1[j, :] += h[i] * (x_ext - mu * sum(L[i:j]))
 		# C_hat_lim2 is never used since y-d is never greater than the y range;
 		# however, it is here so it can be plotted.
 		if j > 1:
-			C_hat_lim2[j, :] = h[j] * x_ext + C[j-1, find_nearest(x, S_star[j-1], True)]
+			C_hat_lim2[j, :] = h[j] * x_ext + C[j-1, find_nearest(x, S_star[j-1], True, index_x)]
 		else:
 			C_hat_lim2[j, :] = h[j] * x_ext
 
 		# Get lead-time demand distribution.
-		# TODO: what happens if demand_source does not provide these functions?
 		ltd_dist = demand_source.lead_time_demand_distribution(L[j])
 
 		# Get truncation bounds for lead-time demand distribution.
 		# If support is finite, use support; otherwise, use F^{-1}(.).
 		if ltd_dist.a == float("-inf"):
-			ltd_lo = ltd_dist.ppf(ltd_lower_tail_prob)
+			d_lo = max(ltd_dist.ppf(ltd_lower_tail_prob), float())
 		else:
-			ltd_lo = ltd_dist.interval(1)[0]
+			d_lo = max(ltd_dist.interval(1)[0], float())
 		if ltd_dist.b == float("inf"):
-			ltd_hi = ltd_dist.ppf(1 - ltd_upper_tail_prob)
+			d_hi = max(ltd_dist.ppf(float(1)-ltd_upper_tail_prob), d_lo)
 		else:
-			ltd_hi = ltd_dist.interval(1)[1]
+			d_hi = max(ltd_dist.interval(1)[1], d_lo)
 
 		# Determine d (lead-time demand) array (truncated and discretized).
-		d_lo = ltd_lo
-		d_hi = ltd_hi
-		d_delta = (d_hi - d_lo) / d_num
-		d = np.arange(d_lo, d_hi + d_delta, d_delta)
+		if discrete_distribution:
+			d_lo    = round(d_lo)
+			d_delta = int(1)
+			num     = round(d_hi-d_lo)
+		elif d_num and d_hi > d_lo:
+			d_lo    = float(d_lo)
+			d_delta = float((d_hi-d_lo)/d_num)
+			num     = d_num
+		else:
+			d_lo    = float((d_lo+d_hi)*0.5)
+			d_delta = float(1)
+			num     = int()
+		d_hi = num*d_delta+d_lo
+		d = np.array([d_ind*d_delta+d_lo for d_ind in range(num+1) if (ltd_dist.cdf((d_ind+0.5)*d_delta+d_lo) if d_ind != num else float(1)) > (ltd_dist.cdf((d_ind-0.5)*d_delta+d_lo) if d_ind else float())])
 
 		# Calculate discretized cdf array.
-		# TODO: handle situation where demand_distrib does not provide _cdf
-		fd = np.array([ltd_dist.cdf(d_val+d_delta/2) - ltd_dist.cdf(d_val-d_delta/2) for d_val in d])
-#		fd = ltd_dist.cdf(d+d_delta/2) - ltd_dist.cdf(d-d_delta/2)
+		fd = np.array([(ltd_dist.cdf(d[ind]+d_delta*float(0.5)) if ind+1 != d.size else float(1))-(ltd_dist.cdf(d[ind]-d_delta*float(0.5)) if ind else float()) for ind in range(d.size)])
+		#fd = ltd_dist.cdf(d+d_delta/2) - ltd_dist.cdf(d-d_delta/2)
 
 		# Calculate C.
 		for y in x:
 
 			# Get index of closest element of x to y.
-			the_x = find_nearest(x, y, True)
+			the_x = index_x[y]
 
-			# Loop through demand_list and calculate expected cost.
+			# Loop through demands and calculate expected cost.
 			# This method uses the following result (see Problem 6.13):
 			# lim_{y -> -infty} C_j(y) = -(p + h'_{j+1})(y - sum_{i=1}^j E[D_i])
 			# lim_{y -> +infty} C_j(y) = h_j(y - E[D_j]) + C_{j-1}(S*_{j-1})
-			# TODO: this can probably be vectorized and be much faster
 
 			the_cost = np.zeros(d.size)
 
 			for d_ind in range(d.size):
 				# Calculate y - d.
 				y_minus_d = y - d[d_ind]
-#				y_minus_d = y - (mu * L[j] + d[d_ind] * sigma * np.sqrt(L[j]))
 
 				# Calculate cost -- use approximate value of C-hat if y-d is
 				# outside of x-range.
-				if y_minus_d < np.min(x):
+				if y_minus_d < x_lo:
 					the_cost[d_ind] = \
-						C_hat_lim1[j, find_nearest(x_ext, y_minus_d, True)]
-				elif y_minus_d > np.max(x): # THIS SHOULD NEVER HAPPEN
+						C_hat_lim1[j, find_nearest(x_ext, y_minus_d, True, index_x_ext)]
+				elif y_minus_d > x_hi: # THIS SHOULD NEVER HAPPEN
+					print('WARNING: y > x + d', flush=True)
 					the_cost[d_ind] = \
-						C_hat_lim2[j, find_nearest(x_ext, y_minus_d, True)]
+						C_hat_lim2[j, find_nearest(x_ext, y_minus_d, True, index_x_ext)]
 				else:
 					the_cost[d_ind] = \
-						C_hat[j, find_nearest(x, y_minus_d, True)]
+						C_hat[j, find_nearest(x, y_minus_d, True, index_x)]
 
 			# Calculate expected cost.
 			C[j, the_x] = np.dot(fd, the_cost)
 
 		# Did user specify S?
 		if S is None:
 			# No -- determine S*.
 			opt_S_index = np.argmin(C[j, :])
 			S_star[j] = x[opt_S_index]
 		else:
 			# Yes -- use specified S.
 			S_star[j] = S[j]
-		C_star[j] = C[j, find_nearest(x, S_star[j], True)]
+		C_star[j] = C[j, find_nearest(x, S_star[j], True, index_x)]
 
 		# Calculate C_bar
-		C_bar[j, :] = C[j, find_nearest(x, np.minimum(S_star[j], x), True)]
+		C_bar[j, :] = C[j, find_nearest(x, np.minimum(S_star[j], x), True, index_x)]
 
 	# Plot functions.
 	if plots:
 		fig, axes = plt.subplots(2, 2)
 		# C_hat.
 		axes[0, 0].plot(x, np.transpose(C_hat[1:N+1, :]))
 		axes[0, 0].set_title('C-hat')
 		axes[0, 0].legend(list(map(str, range(1, N+1))))
 		k = N
-		axes[0, 0].plot(x, C_hat_lim1[k, find_nearest(x_ext, x)], ':')
-		axes[0, 0].plot(x, C_hat_lim2[k, find_nearest(x_ext, x)], ':')
+		axes[0, 0].plot(x, C_hat_lim1[k, find_nearest(x_ext, x, True, index_x_ext)], ':')
+		axes[0, 0].plot(x, C_hat_lim2[k, find_nearest(x_ext, x, True, index_x_ext)], ':')
 		# C_bar.
 		axes[0, 1].plot(x, np.transpose(C_bar))
 		axes[0, 1].set_title('C-bar')
 		axes[0, 1].legend(list(map(str, range(N+1))))
 		# C.
 		axes[1, 0].plot(x, np.transpose(C[1:N+1, :]))
 		axes[1, 0].set_title('C')
 		axes[1, 0].legend(list(map(str, range(1, N+1))))
 
 		plt.show()
 
+	# Revert to original node indexing.
+	temp_S_star = {n_ind: S_star[old_to_new_dict[n_ind]] for n_ind in old_to_new_dict.keys()}
+	S_star = temp_S_star
+
 	return S_star, C_star[N]	
 
 
-def newsvendor_heuristic(num_nodes=None, echelon_holding_cost=None, lead_time=None,
+def newsvendor_heuristic(num_nodes=None, node_order_in_system=None, node_order_in_lists=None,
+								echelon_holding_cost=None, lead_time=None,
 								stockout_cost=None, demand_mean=None, demand_standard_deviation=None,
-								demand_source=None, network=None, weight=0.5):
+								demand_source=None, network=None, weight=0.5, round_type=None):
 	"""Shang-Song (2003) heuristic for stochastic serial systems under
-	stochastic service model (SSM), as described in Snyder and Shen (2019).
+	stochastic service model (SSM), as described in |fosct|.
 
 	Problem instance may either be provided in the individual parameters ``num_nodes``, ..., ``demand_source``,
-	or in the ``network`` parameter.
+	or as a |class_network| in the ``network`` parameter.
+
+	By default, the nodes in the system are assumed to be indexed
+	``num_nodes``, ..., 1, with node 1 at the downstream end, but this can be changed by
+	providing either the ``node_order_in_system`` or ``network`` parameter.
 
-	The nodes must be indexed :math:`N, \\ldots, 1`. The node-specific
-	parameters (``echelon_holding_cost`` and ``lead_time``) must be either 
-	a dict, a list, or a singleton, with the following requirements:
+	The node-specific parameters (``echelon_holding_cost``, ``lead_time``)
+	must be either a dict, a list, or a singleton, with the following requirements:
 	
-	* If the parameter is a dict, its keys must equal 1,..., ``num_nodes``,
-	  each corresponding to a node index.
-	* If the parameter is a list, it must have length ``num_nodes`` + 1;
-	  the 0th entry will be ignored and the other entries will correspond to the node indices.
-	* If the parameter is a singleton, all nodes will have that parameter set to the
-	  singleton value.
+	* If the parameter is a dict, then the keys must contain the node indices and the values
+	  must contain the corresponding attribute values. If a given node index is contained in
+	  ``node_order_in_system`` (or in 1, ..., ``num_nodes``, if ``node_order_in_system`` is not
+	  provided) but is not a key in the dict, the attribute value is set to ``None`` for that node.
+	* If the parameter is a singleton, then the attribute is set to that value for all nodes.
+	* If the parameter is a list and ``node_order_in_lists`` is provided, ``node_order_in_lists`` 
+	  must contain the same indices as ``node_order_in_system`` (if it is provided) or 1, ..., ``num_nodes``
+	  (if it is not), otherwise a ``ValueError`` is raised. The values in the list are assumed
+	  to correpond to the node indices in the order they are specified in ``node_order_in_lists``.
+	  That is, the value in slot ``k`` in the parameter list is assigned to the node with index
+	  ``node_order_in_lists[k]``. 
+	* If the parameter is a list and ``node_order_in_lists`` is not provided, the values
+	  in the list are assumed to correspond to nodes in the same order as ``node_order_in_system``
+	  (or in  ``num_nodes``, ..., 1, if ``node_order_in_system`` is not provided).
+	
+	(These are the same requirements as in :func:`stockpyl.supply_chain_network.serial_system`, except
+	that the default node numbering is  ``num_nodes``, ..., 1 here.)
 
 	Either ``demand_mean`` and ``demand_standard_deviation`` must be
-	provided (in which case the demand will be assumed to be normally distributed)
-	or a ``demand_source`` must be provided.
+	provided (in which case the demand will be assumed to be normally distributed),
+	or ``demand_source`` must be provided, or ``network`` must be provided.
+
+	Rounding is discussed in Shang and Song (2003), p. 625.
 
 
 	Parameters
 	----------
 	num_nodes : int, optional
 		Number of nodes in serial system. [:math:`N`]
+	node_order_in_system : list, optional
+		List of node indices in the order that they appear in the serial system,
+		with upstream-most node listed first. If omitted, the system will be indexed
+		``num_nodes``, ..., 1. Ignored if ``network`` is provided.
+	node_order_in_lists : list, optional
+		List of node indices in the order in which the nodes are listed in any
+		attributes that are lists. (``node_order_in_lists[k]`` is the index of the ``k`` th node.)
+		Ignored if ``network`` is provided.
 	echelon_holding_cost : float, list, or dict, optional
 		Echelon holding cost at each node. [:math:`h`]
 	lead_time : float, list, or dict, optional
 		(Shipment) lead time at each node. [:math:`L`]
 	stockout_cost : float, optional
 		Stockout cost per item per unit time at node 1. [:math:`p`]
 	demand_mean : float, optional
 		Mean demand per unit time at node 1. Ignored if ``demand_source`` is not ``None``. [:math:`\\mu`]
 	demand_standard_deviation : float, optional
 		Standard deviation of demand per unit time at node 1. Ignored if ``demand_source`` is not ``None``. [:math:`\\mu`]
-	demand_source : DemandSource, optional
-		A DemandSource object describing the demand distribution. Required if
+	demand_source : |class_demand_source|, optional
+		A |class_demand_source| object describing the demand distribution. Required if
 		``demand_mean`` and ``demand_standard_deviation`` are ``None``.
-	network : SupplyChainNetwork, optional
-		A SupplyChainNetwork object that provides all of the necessary data. If provided,
+	network : |class_network|, optional
+		A |class_network| object that provides all of the necessary data. If provided,
 		``num_nodes``, ..., ``demand_source`` are ignored.
 	weight : float, optional
 		Weight to use in weighted sum of lower- and upper-bound base-stock levels. 
+	round_type : string, optional
+		Set to 'up' to always round base-stock levels up to next larger integer, 'down' to 
+		always round down, 'nearest' to round to nearest integer, or ``None`` to not round at all.
 
 	Returns
 	-------
 	S_heur : dict
 		Dict of heuristic echelon base-stock levels. [:math:`\\tilde{S}`]
 
 	Raises
@@ -488,14 +567,19 @@
 	ValueError
 		If ``demand_mean`` or ``demand_standard_deviation`` is ``None`` and 
 		``demand_source`` is ``None``.
 	ValueError
 		If ``stockout_cost`` < 0 or if ``lead_time`` < 0 for any node.
 		
 
+	References
+	----------
+	K. H. Shang and J.-S. Song. Newsvendor bounds and heuristic for optimal policies in serial supply chains. *Management Science*, 49(5):618-638, 2003.
+	
+
 	**Equation Used** (equation (6.32)): 
 
 	.. math::
 
 		\\tilde{S}_j = \\texttt{weight}\\tilde{F}_j^{-1}\\left(\\frac{p+\\sum_{i=j+1}^N h_i}{p+\\sum_{i=j}^N h_i}\\right) + (1-\\texttt{weight})\\tilde{F}_j^{-1}\\left(\\frac{p+\\sum_{i=j+1}^N h_i}{p+\\sum_{i=1}^N h_i}\\right)
 	
 	for :math:`j=1,\\ldots,N`.
@@ -507,106 +591,80 @@
 
 		from stockpyl.ssm_serial import *
 
 	.. doctest::
 
 		>>> S_heur = newsvendor_heuristic(
 		...		num_nodes=3, 
-		...		echelon_holding_cost=[3, 2, 2], 
-		...		lead_time=[1, 1, 2], 
+		...		echelon_holding_cost=[2, 2, 3], 
+		...		lead_time=[2, 1, 1], 
 		...		stockout_cost=37.12, 
 		...		demand_mean=5, 
 		...		demand_standard_deviation=1
 		...		)
-		>>> S_heur # (optimal is {1: 6.5144388073261155, 2: 12.012332294949644, 3: 22.700237234889784})
-		{1: 6.490880975286938, 2: 12.027434723327854, 3: 22.634032391786285}
+		>>> S_heur # (optimal is {3: 22.700237234889784, 2: 12.012332294949644, 1: 6.5144388073261155})
+		{3: 22.634032391786285, 2: 12.027434723327854, 1: 6.490880975286938}
 		>>> # Calculate expected cost of heuristic solution. (optimal is 47.668653127136345)
 		>>> expected_cost(
 		...		echelon_S=S_heur,
 		...		num_nodes=3, 
-		...		echelon_holding_cost=[3, 2, 2], 
-		...		lead_time=[1, 1, 2], 
+		...		echelon_holding_cost=[2, 2, 3], 
+		...		lead_time=[2, 1, 1], 
 		...		stockout_cost=37.12, 
 		...		demand_mean=5, 
 		...		demand_standard_deviation=1
 		...		)
-		47.68009914084217
+		47.65465421619295
 	"""
 
-	# Check for presence of data.
-	if network is None and (num_nodes is None or echelon_holding_cost is None or \
-		lead_time is None or stockout_cost is None):
-		raise ValueError("You must provide either network or num_nodes, ..., stockout_cost")
-
-	# Convert network to parameters, if network provided.
-	if network:
-		num_nodes = len(network.nodes)
-		echelon_holding_cost = {node.index: node.echelon_holding_cost for node in network.nodes}
-		lead_time = {node.index: node.lead_time for node in network.nodes}
-		stockout_cost = network.get_node_from_index(1).stockout_cost
-		demand_source = network.get_node_from_index(1).demand_source
-
-	# Build dicts of parameters.
-	indices = list(range(1, num_nodes+1))
-	echelon_holding_cost_dict = ensure_dict_for_nodes(echelon_holding_cost, indices)
-	lead_time_dict = ensure_dict_for_nodes(lead_time, indices, 0)
-	stockout_cost_dict = {n: stockout_cost if n == 1 else 0 for n in indices}
-	
-	# Validate parameters.
-	if not all(echelon_holding_cost_dict.values()): raise ValueError("echelon_holding_cost cannot be None for any node")
-	if not all(lead_time_dict.values()): raise ValueError("lead_time cannot be None for any node")
-	if any(l < 0 for l in lead_time_dict.values()): raise ValueError("lead_time must be non-negative for every node")
-	if stockout_cost is None: raise ValueError("stockout_cost cannot be None")
-	elif stockout_cost < 0: raise ValueError("stockout_cost must be non-negative")
-	if (demand_mean is None or demand_standard_deviation is None) and demand_source is None:
-		raise ValueError("You must provide either demand_mean and demand_standard_deviation, or demand_source")
+	# Validate data and re-index to N, ..., 1.
+	old_to_new_dict, num_nodes, echelon_holding_cost_dict, lead_time_dict, stockout_cost, demand_source \
+		= _preprocess_parameters(num_nodes, node_order_in_system, node_order_in_lists, echelon_holding_cost,
+		lead_time, stockout_cost, demand_mean, demand_standard_deviation, demand_source, network)
 
 	# Get shortcuts to some parameters (for convenience).
 	N = num_nodes
-	if demand_source is None:
-		mu = demand_mean
-		sigma = demand_standard_deviation
-	else:
-		mu = demand_source.demand_distribution.mean()
-		sigma = demand_source.demand_distribution.std()
+	indices = list(range(1, num_nodes+1))
+	# demand_source is filled by _preprocess_parameters() if not specified as parameters.
+	mu = demand_source.demand_distribution.mean()
+	sigma = demand_source.demand_distribution.std()
 	L = [0] + [lead_time_dict[j] for j in range(1, N+1)]
 	h = [0] + [echelon_holding_cost_dict[j] for j in range(1, N+1)]
 	p = stockout_cost
 
 	# Build "sum of lead-time demand" distributions (LTD distribution in
 	# which L = sum of lead times of stages 1, ..., j) for j = 1, ..., N.
 	sum_ltd_dist = {}
-	if demand_source is None:
-		demand_source = DemandSource()
-		demand_source.type = 'N'
-		demand_source.mean = demand_mean
-		demand_source.standard_deviation = demand_standard_deviation
 	for j in indices:
 		sum_ltd_dist[j] = demand_source.lead_time_demand_distribution(float(np.sum(L[1:(j+1)])))
-
-	# TODO: unit tests for non-normal demand distributions
 	
 	# Solve newsvendor problems.
 	S_heur = {}
 	for j in indices:
 		# Calculate effective holding and stockout costs.
 		p_eff = p + np.sum(h[j+1:])
 		h_eff_u = h[j]
 		h_eff_l = np.sum(h[1:j+1])
 		if demand_source.type == 'N':
 			# Normal.
 			# Calculate parameters of LTD distribution.
 			mu_ltd = mu * np.sum(L[1:j+1])
-			sigma_ltd = sigma * np.sqrt(np.sum(L[1:j+1]))
+			sigma_ltd = sigma * math.sqrt(np.sum(L[1:j+1]))
 			# Calculate newsvendor quantities.
 			S_u, _ = newsvendor_normal(h_eff_u, p_eff, mu_ltd, sigma_ltd)
 			S_l, _ = newsvendor_normal(h_eff_l, p_eff, mu_ltd, sigma_ltd)
+		elif demand_source.type == 'P':
+			# Poisson.
+			# Calculate parameters of LTD distribution.
+			mu_ltd = mu * np.sum(L[1:j+1])
+			# Calculate newsvendor quantities.
+			S_u, _ = newsvendor_poisson(h_eff_u, p_eff, mu_ltd)
+			S_l, _ = newsvendor_poisson(h_eff_l, p_eff, mu_ltd)
 		elif demand_source.type == 'UC':
 			# Uniform continuous.
-			# TODO: handle other continuous distributions (in DemandSource() too)
 			# Build LTD distribution.
 			ltd_distrib = demand_source.lead_time_demand_distribution(float(np.sum(L[1:(j+1)])))
 			# Calculate newsvendor quantities.
 			S_u, _ = newsvendor_continuous(h_eff_u, stockout_cost, ltd_distrib)
 			S_l, _ = newsvendor_continuous(h_eff_l, stockout_cost, ltd_distrib)
 		elif demand_source.type in ('UD', 'CD'):
 			# Discrete.
@@ -617,15 +675,19 @@
 			S_l, _ = newsvendor_discrete(h_eff_l, stockout_cost, ltd_distrib)
 		else:
 			raise ValueError(f"demand_source.type '{demand_source.type}' is not supported")
 		
 		# Take weighted average.
 		S_heur[j] = weight * S_l + (1 - weight) * S_u
 
-	return S_heur
+	# Revert to original node indexing.
+	temp_S_heur = {n_ind: S_heur[old_to_new_dict[n_ind]] for n_ind in old_to_new_dict.keys()}
+	S_heur = temp_S_heur
+
+	return round_dict_values(S_heur, round_type)
 
 
 ### COST-RELATED FUNCTIONS ###
 
 def expected_cost(echelon_S, 
 					num_nodes=None, echelon_holding_cost=None, lead_time=None,
 					stockout_cost=None, demand_mean=None, demand_standard_deviation=None,
@@ -633,73 +695,25 @@
 					x_num=1000, d_num=100,
 					ltd_lower_tail_prob=1-stats.norm.cdf(4),
 					ltd_upper_tail_prob=1-stats.norm.cdf(4),
 					sum_ltd_lower_tail_prob=1-stats.norm.cdf(4),
 					sum_ltd_upper_tail_prob=1-stats.norm.cdf(8)):
 	"""Calculate expected cost of given solution.
 
-	This is a wrapper function that calls ``optimize_base_stock_levels()``
+	This is a wrapper function that calls :func:`~stockpyl.ssm_serial.optimize_base_stock_levels`
 	without doing any optimization.
 
-	Problem instance may either be provided in the individual parameters ``num_nodes``, ..., ``demand_source``,
-	or in the ``network`` parameter.
-
-	The nodes must be indexed :math:`N, \\ldots, 1`. The node-specific
-	parameters (``echelon_holding_cost`` and ``lead_time``) must be either 
-	a dict, a list, or a singleton, with the following requirements:
-	
-	* If the parameter is a dict, its keys must equal 1,..., ``num_nodes``,
-	  each corresponding to a node index.
-	* If the parameter is a list, it must have length ``num_nodes`` + 1;
-	  the 0th entry will be ignored and the other entries will correspond to the node indices.
-	* If the parameter is a singleton, all nodes will have that parameter set to the
-	  singleton value.
-
-	Either ``demand_mean`` and ``demand_standard_deviation`` must be
-	provided (in which case the demand will be assumed to be normally distributed)
-	or a ``demand_source`` must be provided.
+	For parameter descriptions, see docstring for :func:`~stockpyl.ssm_serial.optimize_base_stock_levels`.
 
 	Parameters
 	----------
 	echelon_S : dict
 		Dict of echelon base-stock levels to be evaluated.
-	num_nodes : int, optional
-		Number of nodes in serial system. [:math:`N`]
-	echelon_holding_cost : float, list, or dict, optional
-		Echelon holding cost at each node. [:math:`h`]
-	lead_time : float, list, or dict, optional
-		(Shipment) lead time at each node. [:math:`L`]
-	stockout_cost : float, optional
-		Stockout cost per item per unit time at node 1. [:math:`p`]
-	demand_mean : float, optional
-		Mean demand per unit time at node 1. Ignored if ``demand_source`` is not ``None``. [:math:`\\mu`]
-	demand_standard_deviation : float, optional
-		Standard deviation of demand per unit time at node 1. Ignored if ``demand_source`` is not ``None``. [:math:`\\mu`]
-	demand_source : DemandSource, optional
-		A DemandSource object describing the demand distribution. Required if
-		``demand_mean`` and ``demand_standard_deviation`` are ``None``.
-	network : SupplyChainNetwork, optional
-		A SupplyChainNetwork object that provides all of the necessary data. If provided,
-		``num_nodes``, ..., ``demand_source`` are ignored.
-	x_num : int, optional
-		Number of discretization intervals to use for ``x`` range.
-	d_num : int, optional
-		Number of discretization intervals to use for ``d`` range.
-	ltd_lower_tail_prob : float, optional
-		Lower tail probability to use when truncating lead-time demand
-		distribution.
-	ltd_upper_tail_prob : float, optional
-		Upper tail probability to use when truncating lead-time demand
-		distribution.
-	sum_ltd_lower_tail_prob : float, optional
-		Lower tail probability to use when truncating "sum-of-lead-times"
-		demand distribution.
-	sum_ltd_upper_tail_prob : float, optional
-		Upper tail probability to use when truncating "sum-of-lead-times"
-		demand distribution.
+	other parameters :
+		See :func:`~stockpyl.ssm_serial.optimize_base_stock_levels`.
 
 	Returns
 	-------
 	cost : float
 		Expected cost of system.
 
 
@@ -725,21 +739,21 @@
 		from stockpyl.ssm_serial import *
 
 	.. doctest::
 
 		>>> expected_cost(
 		...		echelon_S={1: 6.5144388073261155, 2: 12.012332294949644, 3: 22.700237234889784},
 		... 	num_nodes=3, 
-		... 	echelon_holding_cost=[3, 2, 2], 
-		... 	lead_time=[1, 1, 2], 
+		... 	echelon_holding_cost=[2, 2, 3], 
+		... 	lead_time=[2, 1, 1], 
 		... 	stockout_cost=37.12, 
 		... 	demand_mean=5, 
 		... 	demand_standard_deviation=1
 		...	)
-		47.668653127136345
+		47.641099926743415
 	"""
 
 	# Validate echelon_S. (Other parameters will be validated in optimize_base_stock_levels().)
 	if not all(echelon_S.values()): raise ValueError("echelon_S cannot be None for any node")
 
 	_, cost = optimize_base_stock_levels(num_nodes=num_nodes, echelon_holding_cost=echelon_holding_cost,
 										lead_time=lead_time, stockout_cost=stockout_cost,
@@ -765,70 +779,22 @@
 							sum_ltd_lower_tail_prob=1-stats.norm.cdf(4),
 							sum_ltd_upper_tail_prob=1-stats.norm.cdf(8)):
 	"""Calculate expected holding cost of given solution.
 
 	The basic idea is to set the stockout cost to 0 and call 
 	:func:`optimize_base_stock_levels` without doing any optimization.
 
-	Problem instance may either be provided in the individual parameters ``num_nodes``, ..., ``demand_source``,
-	or in the ``network`` parameter.
-
-	The nodes must be indexed :math:`N, \\ldots, 1`. The node-specific
-	parameters (``echelon_holding_cost`` and ``lead_time``) must be either 
-	a dict, a list, or a singleton, with the following requirements:
-	
-	* If the parameter is a dict, its keys must equal 1,..., ``num_nodes``,
-	  each corresponding to a node index.
-	* If the parameter is a list, it must have length ``num_nodes`` + 1;
-	  the 0th entry will be ignored and the other entries will correspond to the node indices.
-	* If the parameter is a singleton, all nodes will have that parameter set to the
-	  singleton value.
-
-	Either ``demand_mean`` and ``demand_standard_deviation`` must be
-	provided (in which case the demand will be assumed to be normally distributed)
-	or a ``demand_source`` must be provided.
+	For parameter descriptions, see docstring for :func:`~stockpyl.ssm_serial.optimize_base_stock_levels`.
 
 	Parameters
 	----------
 	echelon_S : dict
 		Dict of echelon base-stock levels to be evaluated.
-	num_nodes : int, optional
-		Number of nodes in serial system. [:math:`N`]
-	echelon_holding_cost : float, list, or dict, optional
-		Echelon holding cost at each node. [:math:`h`]
-	lead_time : float, list, or dict, optional
-		(Shipment) lead time at each node. [:math:`L`]
-	stockout_cost : float, optional
-		Stockout cost per item per unit time at node 1. [:math:`p`]
-	demand_mean : float, optional
-		Mean demand per unit time at node 1. Ignored if ``demand_source`` is not ``None``. [:math:`\\mu`]
-	demand_standard_deviation : float, optional
-		Standard deviation of demand per unit time at node 1. Ignored if ``demand_source`` is not ``None``. [:math:`\\mu`]
-	demand_source : DemandSource, optional
-		A DemandSource object describing the demand distribution. Required if
-		``demand_mean`` and ``demand_standard_deviation`` are ``None``.
-	network : SupplyChainNetwork, optional
-		A SupplyChainNetwork object that provides all of the necessary data. If provided,
-		``num_nodes``, ..., ``demand_source`` are ignored.
-	x_num : int, optional
-		Number of discretization intervals to use for ``x`` range.
-	d_num : int, optional
-		Number of discretization intervals to use for ``d`` range.
-	ltd_lower_tail_prob : float, optional
-		Lower tail probability to use when truncating lead-time demand
-		distribution.
-	ltd_upper_tail_prob : float, optional
-		Upper tail probability to use when truncating lead-time demand
-		distribution.
-	sum_ltd_lower_tail_prob : float, optional
-		Lower tail probability to use when truncating "sum-of-lead-times"
-		demand distribution.
-	sum_ltd_upper_tail_prob : float, optional
-		Upper tail probability to use when truncating "sum-of-lead-times"
-		demand distribution.
+	other parameters :
+		See :func:`~stockpyl.ssm_serial.optimize_base_stock_levels`.
 
 	Returns
 	-------
 	holding_cost : float
 		Expected holding cost of system.
 
 
@@ -854,21 +820,21 @@
 		from stockpyl.ssm_serial import *
 
 	.. doctest::
 
 		>>> expected_holding_cost(
 		...		echelon_S={1: 6.5144388073261155, 2: 12.012332294949644, 3: 22.700237234889784},
 		... 	num_nodes=3, 
-		... 	echelon_holding_cost=[3, 2, 2], 
-		... 	lead_time=[1, 1, 2], 
+		... 	echelon_holding_cost=[2, 2, 3], 
+		... 	lead_time=[2, 1, 1], 
 		... 	stockout_cost=37.12, 
 		... 	demand_mean=5, 
 		... 	demand_standard_deviation=1
 		...	)
-		43.15945901616041
+		43.10006605241919
 	"""
 
 	# Validate echelon_S. (Other parameters will be validated in optimize_base_stock_levels().)
 	if not all(echelon_S.values()): raise ValueError("echelon_S cannot be None for any node")
 
 	# Make copy of network and set stockout cost to 0.
 	if network:
@@ -888,12 +854,96 @@
 										ltd_upper_tail_prob=ltd_upper_tail_prob,
 										sum_ltd_lower_tail_prob=sum_ltd_lower_tail_prob,
 										sum_ltd_upper_tail_prob=sum_ltd_upper_tail_prob)
 
 	return holding_cost
 
 
+### HELPER FUNCTIONS ###
 
+def _preprocess_parameters(num_nodes=None, node_order_in_system=None, node_order_in_lists=None,
+								echelon_holding_cost=None, lead_time=None, stockout_cost=None, 
+								demand_mean=None, demand_standard_deviation=None,
+								demand_source=None, network=None):
+	"""Check that appropriate parameters are provided, validate their values, convert to N, ..., 1
+	indexing, and return dict-ified parameters.
 
-#S_star, C_star = optimize_base_stock_levels(instance_2_stage, plots=False)
-#print('S_star = {}, C_star = {}'.format(S_star, C_star))
+	Parameters
+	----------
+	see optimize_base_stock_levels()
+
+	Returns
+	-------
+	old_to_new_dict
+		dict in which keys are old indices of nodes and values are new indices
+	num_nodes
+		Number of nodes in system
+	echelon_holding_cost_dict
+		Dict of echelon holding costs, under new indexing
+	lead_time_dict
+		Dict of lead times, under new indexing
+	stockout_cost
+		Stockout cost
+	demand_source
+		Demand source
+	"""
+
+	# Check for presence of data.
+	if network is None:
+		if (num_nodes is None or echelon_holding_cost is None or \
+			lead_time is None or stockout_cost is None):
+			raise ValueError("You must provide either network or num_nodes, ..., stockout_cost")
+	if network is None and (demand_mean is None or demand_standard_deviation is None) and demand_source is None:
+		raise ValueError("You must provide either demand_mean and demand_standard_deviation, or demand_source")
 
+	# Standardize parameters: Convert node indexing to N, ..., 1 and put all attributes in
+	# separate parameter dicts (if they are not already).
+	if network:
+		# Make local copy.
+		num_nodes = len(network.nodes)
+		local_network = copy.deepcopy(network)
+	else:
+		# Build a network with the specified node order.
+		if node_order_in_system is None:
+			# Make sure num_nodes is provided.
+			if num_nodes is None:
+				raise ValueError("Either num_nodes, node_order_in_system, or network must be provided")
+			node_order_in_system = list(range(num_nodes, 0, -1))
+		else:
+			num_nodes = len(node_order_in_system)
+		if node_order_in_lists is None:
+			# Build node_order_in_lists.
+			node_order_in_lists = node_order_in_system 
+		# Build demand_source, if not provided.
+		if demand_source is None:
+			demand_source = DemandSource(type='N', mean=demand_mean, standard_deviation=demand_standard_deviation)
+		# Build serial system.
+		local_network = serial_system(num_nodes=num_nodes, 
+			node_order_in_system=node_order_in_system,
+			node_order_in_lists=node_order_in_lists,
+			echelon_holding_cost=echelon_holding_cost,
+			shipment_lead_time=lead_time,
+			stockout_cost=stockout_cost,
+			demand_source=demand_source
+		)
+	# Reindex nodes to N, ..., 1.
+	old_to_new_dict = {}
+	k = num_nodes
+	n = local_network.source_nodes[0]
+	for _ in range(num_nodes):
+		old_to_new_dict[n.index] = k
+		k -= 1
+		n = n.get_one_successor()
+	local_network.reindex_nodes(old_to_new_dict)
+	# Build dicts and singletons of parameters.
+	echelon_holding_cost_dict = {node.index: node.echelon_holding_cost for node in local_network.nodes}
+	lead_time_dict = {node.index: node.lead_time for node in local_network.nodes}
+	stockout_cost = local_network.get_node_from_index(1).stockout_cost
+	demand_source = local_network.get_node_from_index(1).demand_source
+	
+	# Validate more parameters.
+	if any(c is None for c in echelon_holding_cost_dict.values()): raise ValueError("echelon_holding_cost cannot be None for any node")
+	if stockout_cost < 0: raise ValueError("stockout_cost must be non-negative")
+	if not all(lead_time_dict.values()): raise ValueError("lead_time cannot be None for any node")
+	if any(l < 0 for l in lead_time_dict.values()): raise ValueError("lead_time must be non-negative for every node")
+	
+	return old_to_new_dict, num_nodes, echelon_holding_cost_dict, lead_time_dict, stockout_cost, demand_source
```

