# Comparing `tmp/ewoksxrpd-0.7.0.tar.gz` & `tmp/ewoksxrpd-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewoksxrpd-0.7.0.tar", last modified: Thu Feb 22 16:46:09 2024, max compression
+gzip compressed data, was "ewoksxrpd-0.8.0.tar", last modified: Tue May 14 11:53:59 2024, max compression
```

## Comparing `ewoksxrpd-0.7.0.tar` & `ewoksxrpd-0.8.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:46:09.887119 ewoksxrpd-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2024-02-22 16:29:40.000000 ewoksxrpd-0.7.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2235 2024-02-22 16:46:09.887119 ewoksxrpd-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-02-22 16:29:40.000000 ewoksxrpd-0.7.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1654 2024-02-22 16:46:09.891119 ewoksxrpd-0.7.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:46:09.871119 ewoksxrpd-0.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:46:09.871119 ewoksxrpd-0.7.0/src/ewoksxrpd/
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-02-22 16:42:36.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:46:09.875119 ewoksxrpd-0.7.0/src/ewoksxrpd/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 16:46:03.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20451 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     2667 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/gui/plots.py
--rw-rw-rw-   0 root         (0) root         (0)      960 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/gui/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     5302 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/gui/trigger_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     1582 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/init_matplotlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:46:09.879119 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 16:46:03.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/ascii.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/background.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/bliss.py
--rw-rw-rw-   0 root         (0) root         (0)    15791 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/calibrate.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/convolution.py
--rw-rw-rw-   0 root         (0) root         (0)     2036 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/data_access.py
--rw-rw-rw-   0 root         (0) root         (0)     8955 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/diagnostics.py
--rw-rw-rw-   0 root         (0) root         (0)    22365 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/integrate.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/log.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/mask.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/morphology.py
--rw-rw-rw-   0 root         (0) root         (0)     4813 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     4782 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/pyfaiconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     1283 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/save_images.py
--rw-rw-rw-   0 root         (0) root         (0)    10861 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/sum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:46:09.879119 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 16:46:03.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3943 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/utils/data_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1799 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/utils/integrate_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    15287 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1556 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/utils/sum_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6036 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:46:09.883119 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 16:46:03.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6294 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1629 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_ascii.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_background.py
--rw-rw-rw-   0 root         (0) root         (0)     2521 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_batch_integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1838 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py
--rw-rw-rw-   0 root         (0) root         (0)    10430 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_calibrate.py
--rw-rw-rw-   0 root         (0) root         (0)    20665 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_calint_workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     2351 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_darkflat.py
--rw-rw-rw-   0 root         (0) root         (0)     4711 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_mask.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_nexus_integrated.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_pyfai_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_save_images.py
--rw-rw-rw-   0 root         (0) root         (0)     5010 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_sum.py
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     1850 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/ewoksxrpd/tests/xrpd_theory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:46:09.887119 ewoksxrpd-0.7.0/src/ewoksxrpd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2235 2024-02-22 16:46:09.000000 ewoksxrpd-0.7.0/src/ewoksxrpd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2940 2024-02-22 16:46:09.000000 ewoksxrpd-0.7.0/src/ewoksxrpd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 16:46:09.000000 ewoksxrpd-0.7.0/src/ewoksxrpd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      228 2024-02-22 16:46:09.000000 ewoksxrpd-0.7.0/src/ewoksxrpd.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-02-22 16:46:09.000000 ewoksxrpd-0.7.0/src/ewoksxrpd.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      319 2024-02-22 16:46:09.000000 ewoksxrpd-0.7.0/src/ewoksxrpd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-02-22 16:46:09.000000 ewoksxrpd-0.7.0/src/ewoksxrpd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:46:09.883119 ewoksxrpd-0.7.0/src/orangecontrib/
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:46:09.883119 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1448 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/ascii.py
--rw-rw-rw-   0 root         (0) root         (0)     2635 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/background.py
--rw-rw-rw-   0 root         (0) root         (0)     1361 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/batchintegrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/calculategeometry.py
--rw-rw-rw-   0 root         (0) root         (0)    11146 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/calibratemulti.py
--rw-rw-rw-   0 root         (0) root         (0)     7837 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/calibratesingle.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py
--rw-rw-rw-   0 root         (0) root         (0)     1443 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:46:09.887119 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 16:46:03.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   188527 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/icons/category.png
--rw-rw-rw-   0 root         (0) root         (0)   188527 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/icons/widget.png
--rw-rw-rw-   0 root         (0) root         (0)     2178 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/integrate1d.py
--rw-rw-rw-   0 root         (0) root         (0)     3252 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/mask.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py
--rw-rw-rw-   0 root         (0) root         (0)     1409 2024-02-22 16:29:41.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:46:09.887119 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 16:46:03.000000 ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/tutorials/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:53:59.799720 ewoksxrpd-0.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2243 2024-05-14 11:53:59.799720 ewoksxrpd-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      293 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1635 2024-05-14 11:53:59.799720 ewoksxrpd-0.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:53:59.787720 ewoksxrpd-0.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:53:59.787720 ewoksxrpd-0.8.0/src/ewoksxrpd/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:53:59.791720 ewoksxrpd-0.8.0/src/ewoksxrpd/gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 11:53:53.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20669 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/gui/image_viewer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/gui/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      960 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/gui/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     5302 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/gui/trigger_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1582 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/init_matplotlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:53:59.791720 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 11:53:53.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/background.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)    19380 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/calibrate.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/convolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/data_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     9594 2024-05-14 11:34:22.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/diagnostics.py
+-rw-rw-rw-   0 root         (0) root         (0)    23247 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/morphology.py
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     4782 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/pyfaiconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/save_images.py
+-rw-rw-rw-   0 root         (0) root         (0)    10895 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/sum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:53:59.791720 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 11:53:53.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3943 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/utils/data_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1819 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/utils/integrate_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    15038 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1556 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/utils/sum_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6036 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:53:59.795720 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 11:53:53.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6644 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_background.py
+-rw-rw-rw-   0 root         (0) root         (0)     2521 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_batch_integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1838 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py
+-rw-rw-rw-   0 root         (0) root         (0)    10805 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_calibrate.py
+-rw-rw-rw-   0 root         (0) root         (0)    20665 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_calint_workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2351 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_darkflat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4711 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1324 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_log.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_nexus_integrated.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_pyfai_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_save_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     5010 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_sum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1850 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/ewoksxrpd/tests/xrpd_theory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:53:59.795720 ewoksxrpd-0.8.0/src/ewoksxrpd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2243 2024-05-14 11:53:59.000000 ewoksxrpd-0.8.0/src/ewoksxrpd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2930 2024-05-14 11:53:59.000000 ewoksxrpd-0.8.0/src/ewoksxrpd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 11:53:59.000000 ewoksxrpd-0.8.0/src/ewoksxrpd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      228 2024-05-14 11:53:59.000000 ewoksxrpd-0.8.0/src/ewoksxrpd.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-14 11:53:59.000000 ewoksxrpd-0.8.0/src/ewoksxrpd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-14 11:53:59.000000 ewoksxrpd-0.8.0/src/ewoksxrpd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:53:59.787720 ewoksxrpd-0.8.0/src/orangecontrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:53:59.795720 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/background.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/batchintegrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/calculategeometry.py
+-rw-rw-rw-   0 root         (0) root         (0)    11146 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/calibratemulti.py
+-rw-rw-rw-   0 root         (0) root         (0)     7837 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/calibratesingle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:53:59.795720 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 11:53:53.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   188527 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/icons/category.png
+-rw-rw-rw-   0 root         (0) root         (0)   188527 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/icons/widget.png
+-rw-rw-rw-   0 root         (0) root         (0)     2178 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/integrate1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     3252 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     2181 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2024-05-14 11:34:23.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:53:59.795720 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 11:53:53.000000 ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/tutorials/__init__.py
```

### Comparing `ewoksxrpd-0.7.0/LICENSE.md` & `ewoksxrpd-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/PKG-INFO` & `ewoksxrpd-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksxrpd
-Version: 0.7.0
+Version: 0.8.0
 Summary: Data processing workflows for SAXS/WAXS
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksxrpd/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksxrpd/
 Project-URL: Documentation, https://ewoksxrpd.readthedocs.io/
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: silx>=1.1.0
+Requires-Dist: silx!=2.1.0,>=1.1.0
 Requires-Dist: pyopencl
 Requires-Dist: pyfai>=2023.3
 Requires-Dist: numexpr!=2.8.6
 Requires-Dist: ewoksdata>0.2.6
 Requires-Dist: ewoks[orange]>=0.1.2
 Requires-Dist: fabio
 Requires-Dist: h5py
```

### Comparing `ewoksxrpd-0.7.0/README.md` & `ewoksxrpd-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/setup.cfg` & `ewoksxrpd-0.8.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -18,29 +18,27 @@
 	Programming Language :: Python :: 3
 keywords = 
 	orange3 add-on,ewoks
 
 [options]
 package_dir = 
 	=src
-packages = find:
+packages = find_namespace:
 python_requires = >=3.7
 install_requires = 
 	numpy
 	scipy
-	silx >=1.1.0
+	silx >=1.1.0,!=2.1.0
 	pyopencl
 	pyfai >=2023.3
 	numexpr !=2.8.6
 	ewoksdata >0.2.6
 	ewoks[orange] >=0.1.2
 	fabio
 	h5py
-namespace_packages = 
-	orangecontrib
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 online = 
 	ewoksdata[online]
```

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/gui/forms.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/gui/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,19 @@
 
 
 def input_parameters_calibratesingle(values: Mapping) -> dict:
     parameters = dict()
     _add_data_singlecalib(parameters)
     _add_energy_geometry(parameters, values, calib=True)
     _add_detector_input(parameters)
+    parameters["ring_detector"] = {
+        "label": "Detector for the ring extraction. Leave this empty to use the same detector.",
+        "value_for_type": list(ALL_DETECTORS),
+        "serialize": str.lower,
+    }
     _add_calibrant_input(parameters)
     _apply_values(parameters, values)
     return parameters
 
 
 def output_parameters_calibratesingle() -> dict:
     parameters = dict()
```

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/gui/plots.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/gui/plots.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/gui/serialize.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/gui/serialize.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/gui/trigger_widget.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/gui/trigger_widget.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/init_matplotlib.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/init_matplotlib.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/ascii.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/ascii.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,20 +15,23 @@
     output_names=["saved"],
 ):
     """Save single diffractogram in ASCII format"""
 
     def run(self):
         if is_data(self.inputs.yerror):
             data = [self.inputs.x, self.inputs.y, self.inputs.yerror]
+            columns = ["x", "intensity", "intensity_error"]
         else:
             data = [self.inputs.x, self.inputs.y]
+            columns = ["x", "intensity"]
         data = numpy.stack(data, axis=1)
 
         header = self.get_input_value("header", dict())
         metadata = self.get_input_value("metadata", dict())
         lines = integration_info_as_text(header, xunits=self.inputs.xunits, **metadata)
+        lines.append(" ".join(columns))
 
         dirname = os.path.dirname(self.inputs.filename)
         if dirname:
             os.makedirs(dirname, exist_ok=True)
         numpy.savetxt(self.inputs.filename, data, header="\n".join(lines))
         self.outputs.saved = True
```

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/background.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/background.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/calibrate.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/calibrate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from __future__ import annotations
 import logging
+import warnings
 from numbers import Number
-from typing import Dict, List, Optional, Set, Tuple
+from typing import Dict, List, Optional, Set, Tuple, Sequence, Union, Generator
 
 import pyFAI.detectors
 import pyFAI.calibrant
+import pyFAI.geometry
 import pyFAI.goniometer
+import pyFAI.geometryRefinement
 
 from .utils import xrpd_utils
 from .utils import data_utils
 from .data_access import TaskWithDataAccess
 
 
 __all__ = ["CalibrateSingle", "CalibrateMulti", "CalculateGeometry"]
@@ -32,111 +36,165 @@
         out |= set(parametrization.get(param, {param}))
     return out
 
 
 class CalibrateSingle(
     TaskWithDataAccess,
     input_names=["image", "detector", "calibrant", "geometry", "energy"],
-    optional_input_names=["detector_config", "fixed", "max_rings", "robust"],
+    optional_input_names=[
+        "detector_config",
+        "fixed",
+        "max_rings",
+        "robust",
+        "ring_detector",
+    ],
     output_names=["geometry", "energy", "detector", "detector_config", "rings", "chi2"],
 ):
     """Single distance and energy calibration."""
 
+    @property
+    def _max_rings(self):
+        max_rings = self.inputs.max_rings
+        if not max_rings:
+            return None
+        if max_rings < 0:
+            return None
+        return max_rings
+
     def run(self):
         detector = data_utils.data_from_storage(self.inputs.detector)
         detector_config = data_utils.data_from_storage(
             self.get_input_value("detector_config", None)
         )
         detector_object = pyFAI.detectors.detector_factory(
             detector, config=detector_config
         )
         calibrant = data_utils.data_from_storage(self.inputs.calibrant)
         calibrant_object = pyFAI.calibrant.get_calibrant(calibrant)
         geometry0 = data_utils.data_from_storage(self.inputs.geometry)
         xrpd_utils.validate_geometry(geometry0)
         wavelength0 = xrpd_utils.energy_wavelength(self.inputs.energy)
 
-        # Define setup
-        setup = pyFAI.goniometer.SingleGeometry(
-            "single",
-            image=self.get_image(self.inputs.image),
-            detector=detector_object,
-            geometry=dict(geometry0),
-            calibrant=calibrant_object,
-        )
-
-        setup.set_wavelength(wavelength0)
-
         # Find diffraction rings and fit
-        self._refine(setup)
+        geometry_refinement = self._refine(
+            dict(geometry0), wavelength0, calibrant_object, detector_object
+        )
 
         # Parse results
-        results = setup.geometry_refinement.get_config()
+        results = geometry_refinement.get_config()
         geometry = {
             k: v for k, v in results.items() if k in xrpd_utils.GEOMETRY_PARAMETERS
         }
         energy = xrpd_utils.energy_wavelength(results["wavelength"])
-        rings = xrpd_utils.points_to_rings(
-            setup.geometry_refinement.data, calibrant_object
-        )
+        rings = xrpd_utils.points_to_rings(geometry_refinement.data, calibrant_object)
 
         self.outputs.geometry = geometry
         self.outputs.energy = energy
         self.outputs.detector = detector
         self.outputs.detector_config = detector_config
         self.outputs.rings = rings
-        if setup.geometry_refinement.data.ndim != 2:
+        if geometry_refinement.data.ndim != 2:
             self.outputs.chi2 = float("nan")
         else:
-            self.outputs.chi2 = setup.geometry_refinement.chi2()
+            self.outputs.chi2 = geometry_refinement.chi2()
 
-    def _refine(self, setup: pyFAI.goniometer.GoniometerRefinement) -> None:
+    def _refine(
+        self,
+        geometry0: dict,
+        wavelength0: float,
+        calibrant: pyFAI.calibrant.Calibrant,
+        detector: pyFAI.detectors.Detector,
+    ) -> pyFAI.GeometryRefinement.GeometryRefinement:
         """Find diffraction rings and fit"""
         parametrization = {"energy": ["wavelength"]}
         force_fixed = parse_fixed(self.inputs.fixed, parametrization)
-        fixed = fixed_prev = set(xrpd_utils.GEOMETRY_PARAMETERS) | {
-            "wavelength"
-        }  # all fixed
+        all_parameters = xrpd_utils.GEOMETRY_PARAMETERS | {"wavelength"}
 
-        max_rings = self.inputs.max_rings
-        if max_rings:
-            if max_rings < 0:
-                max_rings = None
+        if self.inputs.robust:
+            parameter_release_groups = [
+                {"dist"},
+                {"poni1", "poni2"},
+                {"rot1", "rot2", "rot3"},
+                {"wavelength"},
+            ]
         else:
-            max_rings = None
+            parameter_release_groups = [set(all_parameters)]
+
+        # Initial fit parameters
+        geometry = geometry0
+        wavelength = wavelength0
+
+        n = len(parameter_release_groups)
+        it_fixed_parameters = _iter_fixed_parameters(
+            all_parameters, force_fixed, parameter_release_groups
+        )
+        for i, fixed_parameters in enumerate(it_fixed_parameters, 1):
+            # Detect experimental rings
+            cps = self._extract_control_points(
+                geometry, calibrant, wavelength, detector
+            )
+
+            # Fit parameters to detected rings
+            setup = pyFAI.goniometer.SingleGeometry(
+                "single_user_detector",
+                detector=detector,
+                geometry=geometry,
+                calibrant=calibrant,
+                control_points=cps,
+            )
+            setup.set_wavelength(wavelength)
 
-        def fit(*release):
-            nonlocal fixed, fixed_prev
-            set_free = set(release) - force_fixed
-            if not set_free:
-                return
-            fixed -= set_free
-            setup.extract_cp(max_rings=max_rings)
-            if setup.geometry_refinement.data.ndim != 2:
+            if cps is None:
                 logger.warning("No rings detected for calibration")
-                return
-            setup.geometry_refinement.refine3(fix=fixed)  # method="slsqp"
-            fixed_prev = fixed
+                return setup.geometry_refinement
+
+            _refine_geometry(
+                setup.geometry_refinement, fixed_parameters=fixed_parameters
+            )
+
+            # Update parameters with fit result
+            results = setup.geometry_refinement.get_config()
+            geometry = {
+                k: v for k, v in results.items() if k in xrpd_utils.GEOMETRY_PARAMETERS
+            }
+            wavelength = results["wavelength"]
 
-        if self.inputs.robust:
-            releases = [
-                ["dist"],
-                ["poni1", "poni2"],
-                ["rot1", "rot2", "rot3"],
-                ["wavelength"],
-            ]
-        else:
-            releases = [
-                ["dist", "poni1", "poni2", "rot1", "rot2", "rot3", "wavelength"]
-            ]
-        n = len(releases)
-        for i, release in enumerate(releases, 1):
-            fit(*release)
             self.progress = i / n * 100
 
+        return setup.geometry_refinement
+
+    def _extract_control_points(
+        self,
+        geometry: dict,
+        calibrant: pyFAI.calibrant.Calibrant,
+        wavelength: float,
+        detector: pyFAI.detectors.Detector,
+    ) -> pyFAI.goniometer.ControlPoints | None:
+        ring_detector_name = self.get_input_value("ring_detector", None)
+        if ring_detector_name is None:
+            ring_detector = detector
+        else:
+            ring_detector = pyFAI.detectors.detector_factory(ring_detector_name)
+
+        setup = pyFAI.goniometer.SingleGeometry(
+            "single_ring_detector",
+            image=self.get_image(self.inputs.image),
+            detector=ring_detector,
+            geometry=geometry,
+            calibrant=calibrant,
+        )
+        setup.set_wavelength(wavelength)
+
+        setup.extract_cp(max_rings=self._max_rings)
+        if setup.geometry_refinement.data.ndim != 2:
+            logger.warning("No rings detected for calibration")
+            return
+
+        return setup.control_points
+
 
 class CalibrateMulti(
     TaskWithDataAccess,
     input_names=[
         "images",
         "positions",
         "detector",
@@ -291,71 +349,62 @@
             geometry0["rot1"] * aunits_per_rad,
             geometry0["rot2"] * aunits_per_rad,
             geometry0["rot3"] * aunits_per_rad,
             energy0,
         ]
         return trans_function, initial_guess
 
+    @property
+    def _max_rings(self):
+        max_rings = self.inputs.max_rings
+        if not max_rings:
+            return None
+        if max_rings < 0:
+            return None
+        return max_rings
+
     def _refine(self, setup: pyFAI.goniometer.GoniometerRefinement) -> None:
         """Find diffraction rings and fit"""
         parametrization = {
             "dist": ["dist_offset", "dist_scale"],
             "poni1": ["poni1_offset", "poni1_scale"],
             "poni2": ["poni2_offset", "poni2_scale"],
             "rot1": ["arot1"],
             "rot2": ["arot2"],
             "rot3": ["arot3"],
         }
         force_fixed = parse_fixed(self.inputs.fixed, parametrization)
-        fixed = fixed_prev = set(setup.trans_function.param_names)  # all fixed
+        all_parameters = set(setup.trans_function.param_names)
 
-        max_rings = self.inputs.max_rings
-        if max_rings:
-            if max_rings < 0:
-                max_rings = None
+        if self.inputs.robust:
+            parameter_release_groups = [
+                {"dist_offset", "dist_scale"},
+                {"poni1_offset", "poni2_offset"},
+                {"arot1", "arot2", "arot3"},
+                {"poni1_scale", "poni2_scale"},
+                {"energy"},
+            ]
         else:
-            max_rings = None
+            parameter_release_groups = [set(all_parameters)]
 
-        def fit(*release):
-            nonlocal fixed, fixed_prev
-            set_free = set(release) - force_fixed
-            if not set_free:
-                return
-            fixed -= set_free
+        n = len(parameter_release_groups)
+        it_fixed_parameters = _iter_fixed_parameters(
+            all_parameters, force_fixed, parameter_release_groups
+        )
+        for i, fixed_parameters in enumerate(it_fixed_parameters, 1):
+            # Detect experimental rings
             for setup_single_dist in setup.single_geometries.values():
-                setup_single_dist.extract_cp(max_rings=max_rings)
-            setup.refine3(fix=fixed)  # method="slsqp"
-            fixed_prev = fixed
+                setup_single_dist.extract_cp(max_rings=self._max_rings)
+                if setup_single_dist.geometry_refinement.data.ndim != 2:
+                    logger.warning("No rings detected for calibration")
+                    return
+
+            # Fit parameters to detected rings
+            _refine_geometry(setup, fixed_parameters=fixed_parameters)
 
-        if self.inputs.robust:
-            releases = [
-                ["dist_offset", "dist_scale"],
-                ["poni1_offset", "poni2_offset"],
-                ["arot1", "arot2", "arot3"],
-                ["poni1_scale", "poni2_scale"],
-                ["energy"],
-            ]
-        else:
-            releases = [
-                [
-                    "dist_offset",
-                    "dist_scale",
-                    "poni1_offset",
-                    "poni2_offset",
-                    "arot1",
-                    "arot2",
-                    "arot3",
-                    "poni1_scale",
-                    "poni2_scale",
-                    "energy",
-                ]
-            ]
-        n = len(releases)
-        for i, release in enumerate(releases, 1):
-            fit(*release)
             self.progress = i / n * 100
 
     def _get_rings(
         self,
         setup: pyFAI.goniometer.GoniometerRefinement,
         calibrant: pyFAI.calibrant.Calibrant,
     ) -> Dict[str, dict]:
@@ -434,7 +483,56 @@
         geometry, energy = calculate_geometry(
             parametrization,
             self.inputs.parameters,
             self.get_data(self.inputs.position),
         )
         self.outputs.geometry = geometry
         self.outputs.energy = energy
+
+
+def _iter_fixed_parameters(
+    all_parameters: Set[str],
+    force_fixed: Set[str],
+    parameter_release_groups: Sequence[Set[str]],
+) -> Generator[Optional[Set[str]], None, None]:
+    """Start with all parameters fixed. Release parameters in groups and yield the fixed parameters after each iteration.
+
+    :param all_parameters: all parameters
+    :param force_fixed: parameters that are always fixed
+    :param parameter_release_groups: groups of parameters to release in each iteration
+    :yield: fixed parameters for each iteration
+    """
+    fixed_parameters = all_parameters
+    for release_group in parameter_release_groups:
+        release = release_group - force_fixed
+        if release:
+            fixed_parameters -= release
+            yield fixed_parameters
+        else:
+            yield None
+
+
+def _refine_geometry(
+    geometry_refinement: Union[
+        pyFAI.goniometer.GoniometerRefinement,
+        pyFAI.geometryRefinement.GeometryRefinement,
+    ],
+    fixed_parameters: Optional[Sequence] = None,
+) -> bool:
+    """
+    Refines the given geometry within the default parameter bounds.
+
+    :param geometry_refinement: A pyFAI object that parameterizes a single or multi-distances geometry.
+    :param fixed_parameters: Parameters that are not allowed to change during refinement.
+    :return: True if refinement is successful within the default parameter bounds, False otherwise.
+    """
+    with warnings.catch_warnings(record=True) as caught_warnings:
+        warnings.filterwarnings(
+            "always",
+            message="Values in x were outside bounds during a minimize step, clipping to bounds",
+            category=RuntimeWarning,
+        )
+        geometry_refinement.refine3(fix=fixed_parameters)  # method="slsqp"
+        if not caught_warnings:
+            return True
+
+    return False
```

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/data_access.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/data_access.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/diagnostics.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/diagnostics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import os
+import warnings
 from numbers import Number
-import matplotlib
+from contextlib import contextmanager
+
 import numpy
+import matplotlib
 from numpy.typing import ArrayLike
 
 try:
     import matplotlib.pyplot as plt
     from matplotlib.colors import SymLogNorm, LogNorm
 except ModuleNotFoundError:
     plt = SymLogNorm = LogNorm = None
@@ -143,18 +146,20 @@
         if plt is None:
             raise RuntimeError("'matplotlib' is not installed")
 
         self.prepare()
         rings = self.inputs.rings
         figsize = self.get_input_value("figsize", (16, 8))
         if rings:
-            _, (ax1, ax2) = plt.subplots(nrows=1, ncols=2, figsize=figsize)
+            with _ignore_mpl_thread_warning():
+                _, (ax1, ax2) = plt.subplots(nrows=1, ncols=2, figsize=figsize)
         else:
             rings = dict()
-            _, ax1 = plt.subplots(nrows=1, ncols=1, figsize=figsize)
+            with _ignore_mpl_thread_warning():
+                _, ax1 = plt.subplots(nrows=1, ncols=1, figsize=figsize)
             ax2 = None
 
         self.plot_calibration(
             ax1,
             ax2,
             self.get_image(self.inputs.image),
             data_utils.data_from_storage(rings),
@@ -185,18 +190,22 @@
             raise RuntimeError("'matplotlib' is not installed")
         nimages = len(self.inputs.images)
         rings = self.inputs.rings
         figsize = self.get_input_value("figsize", (16, 8))
         figsize = (figsize[0], figsize[1] * nimages)
         if rings:
             rings = {int(k): v for k, v in rings.items()}
-            _, axes = plt.subplots(nrows=nimages, ncols=2, figsize=figsize)
+            with _ignore_mpl_thread_warning():
+                _, axes = plt.subplots(nrows=nimages, ncols=2, figsize=figsize)
         else:
             rings = {i: dict() for i in range(nimages)}
-            _, axes = plt.subplots(nrows=nimages, ncols=1, figsize=(10, 10 * nimages))
+            with _ignore_mpl_thread_warning():
+                _, axes = plt.subplots(
+                    nrows=nimages, ncols=1, figsize=(10, 10 * nimages)
+                )
             axes = [(ax1, None) for ax1 in axes]
 
         for image, position, ringsi, (ax1, ax2) in zip(
             self.inputs.images, self.inputs.positions, sorted(rings), axes
         ):
             image = self.get_image(image)
             position = self.get_data(position)
@@ -226,15 +235,16 @@
     def run(self):
         if self.inputs.filename:
             if os.path.exists(self.inputs.filename):
                 self.outputs.saved = True
                 return
         if plt is None:
             raise RuntimeError("'matplotlib' is not installed")
-        plt.figure(figsize=(16, 8))
+        with _ignore_mpl_thread_warning():
+            plt.figure(figsize=(16, 8))
         plt.title("Diffractogram")
 
         scaling = self.get_input_value("scaling", "squareroot").lower()
         if self.missing_inputs.yerror:
             plt.plot(self.inputs.x, self.inputs.y)
         else:
             yerr = numpy.minimum(3 * self.inputs.y, self.inputs.yerror)
@@ -262,7 +272,18 @@
             yvalues = numpy.interp(xvalues, self.inputs.x, self.inputs.y)
             labels = xrpd_utils.calibrant_ring_labels(calibrant)
             labels = numpy.array(labels[: mask.size])[mask]
             ymin = min(self.inputs.y)
             for label, x, ymax in zip(labels, xvalues, yvalues):
                 plt.plot([x, x], [ymin, ymax])
                 # plt.text(x, ymax, label)
+
+
+@contextmanager
+def _ignore_mpl_thread_warning():
+    with warnings.catch_warnings():
+        warnings.filterwarnings(
+            "ignore",
+            message="Starting a Matplotlib GUI outside of the main thread will likely fail.",
+            category=UserWarning,
+        )
+        yield
```

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/integrate.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/integrate.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import logging
 from numbers import Number
 from contextlib import contextmanager, ExitStack
 from typing import Union, Tuple, List, Dict, Optional, Any
 
 import numpy
 import h5py
+from ewoksdata.data.nexus import select_default_plot
 from ewoksdata.data.hdf5.dataset_writer import DatasetWriter
 
 from .worker import persistent_worker
 from .worker import set_maximum_persistent_workers
-from .log import log_iterator_progress
+from .log import zip_with_progress
 from .utils import data_utils, xrpd_utils, pyfai_utils, integrate_utils
 from .data_access import TaskWithDataAccess
 
 
 __all__ = [
     "Integrate1D",
     "Integrate1DList",
@@ -184,45 +185,47 @@
         with self._worker() as (worker, config):
             result = worker.process(raw_data, normalization_factor=normalization_factor)
 
             self.outputs.x = result.radial
             self.outputs.y = result.intensity
             yerror = integrate_utils.get_yerror(result)
             self.outputs.yerror = numpy.abs(yerror)
+            self.outputs.yerror[result.intensity <= 0] = numpy.nan
             self.outputs.xunits = result.unit.name
 
             info = pyfai_utils.compile_integration_info(
                 config,
                 monitor_value=monitor_value,
                 reference_value=reference_value,
             )
             self.outputs.info = info
 
 
 class Integrate1DList(
     _BaseIntegrate,
     input_names=["images", "output_file"],
-    optional_input_names=["monitors", "references"],
+    optional_input_names=["monitors", "references", "entry_name"],
     output_names=["output_uri"],
 ):
     """1D integration of a list of diffraction patterns."""
 
     def run(self):
         images: List[str] = self.inputs.images
         output_file: str = self.inputs.output_file
         monitors = self.get_input_value("monitors", [None] * len(images))
         references = self.get_input_value("references", [None] * len(images))
+        entry_name = self.get_input_value("entry_name", "processing")
 
         with ExitStack() as stack:
             h5file = stack.enter_context(h5py.File(output_file, "a"))
-            entry = h5file.require_group("processing")
-            entry.attrs["NX_class"] = "NXentry"
-            entry.attrs["default"] = "integrate"
+            entry = h5file.require_group(entry_name)
+            entry.attrs.setdefault("NX_class", "NXentry")
             process = entry.require_group("integrate")
             process.attrs["NX_class"] = "NXprocess"
+            entry.attrs.setdefault("default", "integrate")
 
             worker, config = stack.enter_context(self._worker())
 
             info = pyfai_utils.compile_integration_info(
                 config, monitors=monitors, references=references
             )
             nxtree_dict = pyfai_utils.integration_info_as_nxdict(info)
@@ -233,19 +236,20 @@
                 update_mode="modify",
                 mode="a",
             )
 
             intensity_writer = None
             error_writer = None
 
-            log_iterator = log_iterator_progress(
-                message="Integrated %s images of %s", logger=logger
-            )
-            for image, monitor, reference, _ in zip(
-                images, monitors, references, log_iterator
+            for image, monitor, reference in zip_with_progress(
+                images,
+                monitors,
+                references,
+                message="Integrated %s images of %s",
+                logger=logger,
             ):
                 # Set mode to 'a' in case images are in `output_file`
                 raw_data = self.get_image(image, mode="a")
                 (monitor_value, reference_value) = self._pyfai_normalization_factor(
                     [monitor], [reference]
                 )
                 normalization_factor = monitor_value / reference_value
@@ -315,28 +319,30 @@
         input_filename = os.path.abspath(self.inputs.filename)
         output_filename = os.path.abspath(self.inputs.output_filename)
         external_output_filename = os.path.abspath(
             self.get_input_value("external_output_filename", output_filename)
         )
         scan = self.inputs.scan
         subscan = self.get_input_value("subscan", 1)
-        input_url = data_utils.hdf5_url(input_filename, f"/{scan}.{subscan}")
-        output_url = data_utils.hdf5_url(output_filename, f"/{scan}.{subscan}")
-        external_output_url = data_utils.hdf5_url(
+        bliss_scan_url = data_utils.hdf5_url(input_filename, f"/{scan}.{subscan}")
+        link_results_nxentry_url = data_utils.hdf5_url(
+            output_filename, f"/{scan}.{subscan}"
+        )
+        results_nxentry_url = data_utils.hdf5_url(
             external_output_filename, f"/{scan}.{subscan}"
         )
 
         flush_period = self.get_input_value("flush_period", None)
 
         with ExitStack() as stack:
             worker = None
-            data_parent = None
-            master_parent = None
-            nxprocess = None
-            measurement = None
+            results_nxentry = None
+            link_results_nxentry = None
+            results_nxprocess = None
+            results_nxmeasurement = None
 
             intensity_writer = None
             error_writer = None
             ctr_writers = dict()
 
             if self.inputs.scan_memory_url:
                 logger.info("PyFAI integrate data from %r", self.inputs.scan_memory_url)
@@ -355,42 +361,48 @@
                 data_iterator = self.iter_bliss_data(
                     self.inputs.filename,
                     self.inputs.scan,
                     lima_names=[detector_name],
                     counter_names=counter_names,
                     subscan=subscan,
                 )
-            log_iterator = log_iterator_progress(
-                message="Integrated %s images of %s", logger=logger
-            )
 
-            for ptdata, _ in zip(data_iterator, log_iterator):
+            for (ptdata,) in zip_with_progress(
+                data_iterator, message="Integrated %s images of %s", logger=logger
+            ):
                 if worker is None:
                     # Start the worker + open the output file only after
                     # the first image is read
                     worker, config = stack.enter_context(self._worker())
                     info = pyfai_utils.compile_integration_info(
                         config,
                         monitors=monitors,
                         references=references,
                     )
-                    data_parent = stack.enter_context(
-                        self.open_h5item(external_output_url, mode="a", create=True)
+                    results_nxentry = stack.enter_context(
+                        self.open_h5item(results_nxentry_url, mode="a", create=True)
                     )
-                    assert isinstance(data_parent, h5py.Group)
+                    assert isinstance(results_nxentry, h5py.Group)
 
                     with self.open_h5item(
-                        output_url, mode="a", create=True
-                    ) as master_parent:
-                        assert isinstance(master_parent, h5py.Group)
-                        nxprocess = pyfai_utils.create_nxprocess(
-                            master_parent, data_parent, self._nxprocess_name, info
+                        link_results_nxentry_url, mode="a", create=True
+                    ) as link_results_nxentry:
+                        assert isinstance(link_results_nxentry, h5py.Group)
+                        results_nxprocess = pyfai_utils.create_nxprocess(
+                            results_nxentry,
+                            link_results_nxentry,
+                            self._nxprocess_name,
+                            info,
+                        )
+                        results_nxmeasurement = results_nxentry.require_group(
+                            "measurement"
+                        )
+                        results_nxmeasurement.attrs.setdefault(
+                            "NX_class", "NXcollection"
                         )
-                        measurement = data_parent.require_group("measurement")
-                        measurement.attrs["NX_class"] = "NXcollection"
 
                 monitor_value, reference_value = self._pyfai_normalization_factor(
                     monitors, references, ptdata
                 )
                 normalization_factor = monitor_value / reference_value
 
                 image = ptdata[detector_name]
@@ -398,78 +410,89 @@
                     image, normalization_factor=normalization_factor
                 )
 
                 intensity_writer, error_writer, flush = integrate_utils.save_result(
                     result,
                     intensity_writer,
                     error_writer,
-                    nxprocess,
+                    results_nxprocess,
                     stack,
                     flush_period,
                 )
                 for name in counter_names:
                     if name not in ctr_writers:
+                        # This copies the raw counter names
                         ctr_writers[name] = stack.enter_context(
-                            DatasetWriter(measurement, name, flush_period=flush_period)
+                            DatasetWriter(
+                                results_nxmeasurement,
+                                name,
+                                flush_period=flush_period,
+                            )
                         )
                     flush |= ctr_writers[name].add_point(ptdata[name])
                 if flush:
-                    data_parent.file.flush()
+                    results_nxentry.file.flush()
 
             if intensity_writer is None:
                 raise RuntimeError(
-                    f"No scan data yielded within {self.get_input_value('retry_timeout')}s from {input_url}"
+                    f"No scan data yielded within {self.get_input_value('retry_timeout')}s from {bliss_scan_url}"
                 )
 
             # Finalized writing
             intensity_writer.flush_buffer()
             if error_writer is not None:
                 error_writer.flush_buffer()
             nxdata = intensity_writer._parent
             nxdata["points"] = numpy.arange(intensity_writer.dataset.shape[0])
             axes = nxdata.attrs["axes"]
             axes[0] = "points"
             nxdata.attrs["axes"] = axes
 
             # Create links
-            with self.open_h5item(output_url, mode="a", create=True) as master_parent:
-                if data_parent.file.filename != master_parent.file.filename:
+            with self.open_h5item(
+                link_results_nxentry_url, mode="a", create=True
+            ) as link_results_nxentry:
+                if not pyfai_utils.is_same_hdf5_group(
+                    results_nxentry, link_results_nxentry
+                ):
                     pyfai_utils.create_hdf5_link(
-                        intensity_writer.dataset, measurement, self._nxmeasurement_name
+                        intensity_writer.dataset,
+                        results_nxmeasurement,
+                        self._nxmeasurement_name,
                     )
-                self.link_bliss_scan(master_parent, input_url)
-                mark_as_default = self.get_input_value("nxprocess_as_default", True)
-                master_measurement = master_parent.require_group("measurement")
-                master_measurement.attrs["NX_class"] = "NXcollection"
-                pyfai_utils.create_nxprocess_links(
-                    nxprocess,
-                    master_measurement,
+                self.link_bliss_scan(link_results_nxentry, bliss_scan_url)
+                if self.get_input_value("nxprocess_as_default", True):
+                    select_default_plot(nxdata)
+                link_nxmeasurement = link_results_nxentry.require_group("measurement")
+                link_nxmeasurement.attrs.setdefault("NX_class", "NXcollection")
+                pyfai_utils.create_hdf5_link(
+                    intensity_writer.dataset,
+                    link_nxmeasurement,
                     self._nxmeasurement_name,
-                    mark_as_default=mark_as_default,
                 )
 
             self.outputs.nxdata_url = f"{nxdata.file.filename}::{nxdata.name}"
 
     @property
-    def _nxprocess_name(self):
+    def _nxprocess_name(self) -> str:
         if self.inputs.nxprocess_name:
             return self.inputs.nxprocess_name
-        default = "integrate"
+        group_name = "integrate"
         if self.inputs.detector_name:
-            return f"{self.inputs.detector_name}_{default}"
-        return default
+            return f"{self.inputs.detector_name}_{group_name}"
+        return group_name
 
     @property
-    def _nxmeasurement_name(self):
+    def _nxmeasurement_name(self) -> str:
         if self.inputs.nxmeasurement_name:
             return self.inputs.nxmeasurement_name
-        default = "integrated"
+        link_name = "integrated"
         if self.inputs.detector_name:
-            return f"{self.inputs.detector_name}_{default}"
-        return default
+            return f"{self.inputs.detector_name}_{link_name}"
+        return link_name
 
 
 class IntegrateBlissScanWithoutSaving(
     _BaseIntegrate,
     input_names=["filename", "scan", "detector_name"],
     optional_input_names=[
         "counter_names",
@@ -546,20 +569,19 @@
                 data_iterator = self.iter_bliss_data(
                     self.inputs.filename,
                     self.inputs.scan,
                     lima_names=[detector_name],
                     counter_names=counter_names,
                     subscan=subscan,
                 )
-            log_iterator = log_iterator_progress(
-                message="Integrated %s images of %s", logger=logger
-            )
 
             normalization_factor = 0
-            for ptdata, _ in zip(data_iterator, log_iterator):
+            for (ptdata,) in zip_with_progress(
+                data_iterator, message="Integrated %s images of %s", logger=logger
+            ):
                 monitor_value, reference_value = self._pyfai_normalization_factor(
                     monitors, references, ptdata
                 )
                 normalization_factor = monitor_value / reference_value
                 image = ptdata[detector_name]
                 result = worker.process(
                     image, normalization_factor=normalization_factor
```

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/mask.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/mask.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/morphology.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/morphology.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/pyfaiconfig.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/pyfaiconfig.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/save_images.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/save_images.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/sum.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/sum.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
     def run(self):
         filename: str = self.inputs.filename
         scan: int = self.inputs.scan
         subscan = self.get_input_value("subscan", 1)
         detector_name: str = self.inputs.detector_name
         output_filename: str = self.inputs.output_filename
-        output_url = hdf5_url(output_filename, f"/{scan}.{subscan}")
+        output_nxentry_url = hdf5_url(output_filename, f"/{scan}.{subscan}")
         monitor_name: Optional[str] = self.get_input_value("monitor_name", None)
-        output_process: str = self.get_input_value("output_process", "sum")
+        output_nxprocess_name: str = self.get_input_value("output_process", "sum")
         background_step: bool = self.get_input_value("background_step", 1)
 
         if self.inputs.scan_memory_url:
             raise NotImplementedError("data from memory not supported yet")
         else:
             lima_iterator = self.iter_bliss_data(
                 filename,
@@ -62,19 +62,19 @@
                     subscan=subscan,
                 )
             else:
                 counter_iterator = (
                     {monitor_name: None} for _ in range(nb_points_in_scan)
                 )
 
-        with self.open_h5item(output_url, mode="a", create=True) as output:
-            sum_process = output.create_group(output_process)
-            sum_process.attrs["NX_class"] = "NXprocess"
-            sum_process.attrs["default"] = "results"
-            nxdata = sum_process.create_group("results")
+        with self.open_h5item(output_nxentry_url, mode="a", create=True) as nxentry:
+            nxprocess = nxentry.create_group(output_nxprocess_name)
+            nxprocess.attrs["NX_class"] = "NXprocess"
+            nxprocess.attrs["default"] = "results"
+            nxdata = nxprocess.create_group("results")
             nxdata.attrs["NX_class"] = "NXdata"
 
             scan_sum = None
             summed_indices = []
 
             for scan_index, ctrdata in iterate_scan_with_skip(
                 counter_iterator, background_step
@@ -187,15 +187,15 @@
             image_range = list(generate_range(start_image, end_image, nimages))
 
             scan_sum = ImageSum(detector_shape)
             full_sum = ImageSum(detector_shape)
 
             with h5py.File(output_filename, "a") as output:
                 entry = output.require_group(output_entry)
-                entry.attrs["NX_class"] = "NXentry"
+                entry.attrs.setdefault("NX_class", "NXentry")
                 entry.attrs["default"] = output_process
                 sum_process = entry.create_group(output_process)
                 sum_process.attrs["NX_class"] = "NXprocess"
                 sum_process.attrs["default"] = "results"
                 results = sum_process.create_group("results")
                 results.attrs["NX_class"] = "NXdata"
```

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/utils/data_utils.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/utils/integrate_utils.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/utils/integrate_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     error_writer: Optional[DatasetWriter],
     nxprocess: h5py.Group,
     stack: ExitStack,
     flush_period: Optional[float] = None,
 ) -> Tuple[Optional[DatasetWriter], Optional[DatasetWriter], bool]:
     if intensity_writer is None:
         radial_axis, azimuthal_axis = pyfai_utils.parse_pyfai_units(result.unit)
-        nxdata = pyfai_utils.create_nxdata(
+        nxdata = pyfai_utils.create_integration_results_nxdata(
             nxprocess,
             result.intensity.ndim + 1,  # +1 for the scan dimension
             result.radial,
             radial_axis.to_str(),
             result.azimuthal if isinstance(result, Integrate2dResult) else None,
             azimuthal_axis.to_str() if isinstance(result, Integrate2dResult) else None,
         )
```

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 import h5py
 from pyFAI import version as pyfai_version
 from ewoks import __version__ as ewoks_version
 from pyFAI.io.ponifile import PoniFile
 from pyFAI.units import Unit
 from silx.io.dictdump import dicttonx
 from ewokscore.task import TaskInputError
-from ewoksdata.data import nexus
 from ewokscore.missing_data import is_missing_data
 
 from .xrpd_utils import energy_wavelength
 from .data_utils import data_from_storage
 
+
 _REPLACE_PATTERNS = {
     "/gpfs/[^/]+/": "/",
     "/mnt/multipath-shares/": "/",
     "/lbsram/": "/",
 }
 
 
@@ -338,38 +338,46 @@
 
 def _add_extra(adict: Mapping, extra: Mapping):
     for k, v in extra.items():
         if v is not None:
             adict[k] = v
 
 
+def is_same_hdf5_group(group1: h5py.Group, group2: h5py.Group) -> bool:
+    """Does not take links into account"""
+    return (
+        os.path.abspath(group1.file.filename) == os.path.abspath(group2.file.filename)
+        and group1.name == group2.name
+    )
+
+
 def create_nxprocess(
-    master_parent: h5py.Group, data_parent: h5py.Group, nxprocess_name: str, info
+    parent: h5py.Group, link_parent: h5py.Group, nxprocess_name: str, info
 ) -> h5py.Group:
+    """Create NXprocess group in the external parent with link in the parent when these are different groups."""
     nxtree_dict = integration_info_as_nxdict(info)
-    nxprocess_path = f"{data_parent.name}/{nxprocess_name}"
-    dicttonx(nxtree_dict, data_parent.file, h5path=nxprocess_path, update_mode="modify")
-    nxprocess = data_parent[nxprocess_name]
-    if data_parent.file.filename != master_parent.file.filename:
-        create_hdf5_link(nxprocess, master_parent, nxprocess_name)
+    nxprocess_path = f"{parent.name}/{nxprocess_name}"
+    dicttonx(nxtree_dict, parent.file, h5path=nxprocess_path, update_mode="modify")
+    nxprocess = parent[nxprocess_name]
+    if not is_same_hdf5_group(parent, link_parent):
+        create_hdf5_link(nxprocess, link_parent, nxprocess_name)
     return nxprocess
 
 
-def create_nxdata(
+def create_integration_results_nxdata(
     nxprocess: h5py.Group,
     intensity_dim: int,
     radial,
     radial_units: str,
     azimuthal,
     azimuthal_units: str,
-    nxdata_name: str = "integrated",
 ) -> h5py.Group:
-    nxdata = nxprocess.create_group(nxdata_name)
+    nxdata = nxprocess.create_group("integrated")
     nxdata.attrs["NX_class"] = "NXdata"
-    nxprocess.attrs["default"] = nxdata_name
+    nxprocess.attrs["default"] = "integrated"
 
     # Axes interpretation
     add_axes_to_nxdata(
         nxdata, intensity_dim, radial, radial_units, azimuthal, azimuthal_units
     )
 
     return nxdata
@@ -405,39 +413,20 @@
     elif not has_azimuth and intensity_dim == 1:
         nxdata.attrs["axes"] = [radial_axis.name]
         nxdata.attrs["interpretation"] = "spectrum"
     else:
         raise ValueError("Unrecognized data")
 
     dset = nxdata.create_dataset(radial_axis.name, data=radial)
-    dset.attrs["units"] = radial_units
+    dset.attrs["units"] = radial_axis.units
     if has_azimuth:
         dset = nxdata.create_dataset(azimuthal_axis.name, data=azimuthal)
         dset.attrs["units"] = azimuthal_axis.units
 
 
-def create_nxprocess_links(
-    nxprocess: h5py.Group,
-    target: h5py.Group,
-    link_name: str,
-    mark_as_default: bool = True,
-) -> None:
-    nxdata = nxprocess["integrated"]
-    try:
-        intensity = nxdata["intensity"]
-    except KeyError:
-        return
-    create_hdf5_link(intensity, target, link_name)
-    if mark_as_default:
-        nexus.select_default_plot(intensity)
-        if intensity.file.filename != nxprocess.file.filename:
-            target.attrs["default"] = link_name
-            nexus.select_default_plot(target)
-
-
 def create_hdf5_link(
     source: Union[h5py.Dataset, h5py.Group], target: h5py.Group, link_name: str
 ) -> None:
     if link_name in target:
         return
     source_filename = source.file.filename
     target_filename = target.file.filename
```

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/utils/sum_utils.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/utils/sum_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tasks/worker.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tasks/worker.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/conftest.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -210,7 +210,20 @@
         "energy": setup1.energy,
         "geometry": setup1.geometry,
         "detector_name": "p3",
         "monitor_name": "monitor",
         "reference": 1.0,
         "retry_timeout": 2,
     }
+
+
+@pytest.fixture(autouse=True)
+def matplotlib_cleanup():
+    """Use this in tests that use matplotlib without ewoksorange.tests.conftest.qtapp"""
+    yield
+    try:
+        from matplotlib.backends import backend_qt
+
+        backend_qt.qApp = None
+        backend_qt._create_qApp.cache_clear()
+    except (ImportError, AttributeError):
+        pass
```

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_ascii.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_ascii.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_background.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_batch_integrate.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_batch_integrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_calibrate.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_calibrate.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,42 +14,54 @@
     OWDiagnoseCalibrateSingleResults,
 )
 from orangecontrib.ewoksxrpd.diagnose_multicalib import (
     OWDiagnoseCalibrateMultiResults,
 )
 
 
-@pytest.mark.parametrize("fixed", [[], ["energy"], ["rot2", "dist"]])
+@pytest.mark.parametrize(
+    "fixed",
+    [[], ["energy"], ["rot2", "dist"]],
+    ids=["fixed=none", "fixed=energy", "fixed=rot2,dist"],
+)
 def test_calibrate_single_distance_task(
     fixed: List[str],
     imageSetup1Calibrant1: Calibration,
     setup1: Setup,
     aiSetup1: pyFAI.azimuthalIntegrator.AzimuthalIntegrator,
     tmpdir: PathLike,
 ):
     assert_calibrate_single_distance(
         fixed, imageSetup1Calibrant1, setup1, aiSetup1, tmpdir, None
     )
 
 
-@pytest.mark.parametrize("fixed", [[], ["energy"], ["rot2", "dist"]])
+@pytest.mark.parametrize(
+    "fixed",
+    [[], ["energy"], ["rot2", "dist"]],
+    ids=["fixed=none", "fixed=energy", "fixed=rot2,dist"],
+)
 def test_calibrate_single_distance_widget(
     fixed: List[str],
     imageSetup1Calibrant1: Calibration,
     setup1: Setup,
     aiSetup1: pyFAI.azimuthalIntegrator.AzimuthalIntegrator,
     tmpdir: PathLike,
     qtapp,
 ):
     assert_calibrate_single_distance(
         fixed, imageSetup1Calibrant1, setup1, aiSetup1, tmpdir, qtapp
     )
 
 
-@pytest.mark.parametrize("fixed", [[], ["energy"], ["rot2", "dist"]])
+@pytest.mark.parametrize(
+    "fixed",
+    [[], ["energy"], ["rot2", "dist"]],
+    ids=["fixed=none", "fixed=energy", "fixed=rot2,dist"],
+)
 def test_calibrate_multi_distance_task(
     fixed: List[str],
     imageSetup1Calibrant1: Calibration,
     setup1: Setup,
     imageSetup2Calibrant1: Calibration,
     setup2: Setup,
     aiSetup1: pyFAI.azimuthalIntegrator.AzimuthalIntegrator,
@@ -65,15 +77,19 @@
         aiSetup1,
         aiSetup2,
         tmpdir,
         None,
     )
 
 
-@pytest.mark.parametrize("fixed", [[], ["energy"], ["rot2", "dist"]])
+@pytest.mark.parametrize(
+    "fixed",
+    [[], ["energy"], ["rot2", "dist"]],
+    ids=["fixed=none", "fixed=energy", "fixed=rot2,dist"],
+)
 def test_calibrate_multi_distance_widget(
     fixed: List[str],
     imageSetup1Calibrant1: Calibration,
     setup1: Setup,
     imageSetup2Calibrant1: Calibration,
     setup2: Setup,
     aiSetup1: pyFAI.azimuthalIntegrator.AzimuthalIntegrator,
@@ -98,15 +114,14 @@
     fixed: List[str],
     imageSetup1Calibrant1: Calibration,
     setup1: Setup,
     aiSetup1: pyFAI.azimuthalIntegrator.AzimuthalIntegrator,
     tmpdir: PathLike,
     qtapp: None,
 ):
-    fixed = []
     geometry0, energy0 = guess_fit_parameters(
         setup1.geometry, setup1.energy, aiSetup1, fixed=fixed
     )
     inputs = {
         "image": imageSetup1Calibrant1.image,
         "geometry": geometry0,
         "detector": setup1.detector,
@@ -365,8 +380,10 @@
             # wrong by +/- 0.5 pixels
             margin = 0.5 * ai.detector.pixel1
         elif pname == "poni2":
             # wrong by +/- 0.5 pixels
             margin = 0.5 * ai.detector.pixel2
         else:
             raise ValueError(pname)
-        assert pytest.approx(expected, abs=margin) == parameters[pname], pname
+        refined_value = parameters[pname]
+        err_msg = f"{pname}: {refined_value} too far from {expected}"
+        assert pytest.approx(expected, abs=margin) == refined_value, err_msg
```

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_calint_workflow.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_calint_workflow.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_darkflat.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_darkflat.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_integrate.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_integrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_mask.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_nexus.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_nexus_integrated.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_nexus_integrated.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_pyfai_utils.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_pyfai_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_save_images.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_save_images.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_sum.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_sum.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/test_worker.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd/tests/xrpd_theory.py` & `ewoksxrpd-0.8.0/src/ewoksxrpd/tests/xrpd_theory.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd.egg-info/PKG-INFO` & `ewoksxrpd-0.8.0/src/ewoksxrpd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksxrpd
-Version: 0.7.0
+Version: 0.8.0
 Summary: Data processing workflows for SAXS/WAXS
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksxrpd/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksxrpd/
 Project-URL: Documentation, https://ewoksxrpd.readthedocs.io/
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: silx>=1.1.0
+Requires-Dist: silx!=2.1.0,>=1.1.0
 Requires-Dist: pyopencl
 Requires-Dist: pyfai>=2023.3
 Requires-Dist: numexpr!=2.8.6
 Requires-Dist: ewoksdata>0.2.6
 Requires-Dist: ewoks[orange]>=0.1.2
 Requires-Dist: fabio
 Requires-Dist: h5py
```

### Comparing `ewoksxrpd-0.7.0/src/ewoksxrpd.egg-info/SOURCES.txt` & `ewoksxrpd-0.8.0/src/ewoksxrpd.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 setup.py
 src/ewoksxrpd/__init__.py
 src/ewoksxrpd/init_matplotlib.py
 src/ewoksxrpd.egg-info/PKG-INFO
 src/ewoksxrpd.egg-info/SOURCES.txt
 src/ewoksxrpd.egg-info/dependency_links.txt
 src/ewoksxrpd.egg-info/entry_points.txt
-src/ewoksxrpd.egg-info/namespace_packages.txt
 src/ewoksxrpd.egg-info/requires.txt
 src/ewoksxrpd.egg-info/top_level.txt
 src/ewoksxrpd/gui/__init__.py
 src/ewoksxrpd/gui/forms.py
+src/ewoksxrpd/gui/image_viewer.py
 src/ewoksxrpd/gui/plots.py
 src/ewoksxrpd/gui/serialize.py
 src/ewoksxrpd/gui/trigger_widget.py
 src/ewoksxrpd/tasks/__init__.py
 src/ewoksxrpd/tasks/ascii.py
 src/ewoksxrpd/tasks/background.py
 src/ewoksxrpd/tasks/bliss.py
@@ -46,23 +46,23 @@
 src/ewoksxrpd/tests/test_background.py
 src/ewoksxrpd/tests/test_batch_integrate.py
 src/ewoksxrpd/tests/test_bliss_integrate_no_save.py
 src/ewoksxrpd/tests/test_calibrate.py
 src/ewoksxrpd/tests/test_calint_workflow.py
 src/ewoksxrpd/tests/test_darkflat.py
 src/ewoksxrpd/tests/test_integrate.py
+src/ewoksxrpd/tests/test_log.py
 src/ewoksxrpd/tests/test_mask.py
 src/ewoksxrpd/tests/test_nexus.py
 src/ewoksxrpd/tests/test_nexus_integrated.py
 src/ewoksxrpd/tests/test_pyfai_utils.py
 src/ewoksxrpd/tests/test_save_images.py
 src/ewoksxrpd/tests/test_sum.py
 src/ewoksxrpd/tests/test_worker.py
 src/ewoksxrpd/tests/xrpd_theory.py
-src/orangecontrib/__init__.py
 src/orangecontrib/ewoksxrpd/__init__.py
 src/orangecontrib/ewoksxrpd/ascii.py
 src/orangecontrib/ewoksxrpd/background.py
 src/orangecontrib/ewoksxrpd/batchintegrate.py
 src/orangecontrib/ewoksxrpd/blissintegratenosave.py
 src/orangecontrib/ewoksxrpd/calculategeometry.py
 src/orangecontrib/ewoksxrpd/calibratemulti.py
```

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/__init__.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/ascii.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/ascii.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/background.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/background.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/batchintegrate.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/batchintegrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/calculategeometry.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/calculategeometry.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/calibratemulti.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/calibratemulti.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/calibratesingle.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/calibratesingle.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import os
-from AnyQt import QtWidgets
-from AnyQt import QtGui
-
 from ewoksxrpd.tasks.diagnostics import DiagnoseIntegrate1D
+from ewoksxrpd.gui.image_viewer import ImageViewer
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_diagnose_integrate1d
 
 
 __all__ = ["OWDiagnoseIntegrate1D"]
 
 
@@ -20,25 +17,19 @@
         parameter_info = input_parameters_diagnose_integrate1d(
             self.get_default_input_values()
         )
         self._create_input_form(parameter_info)
 
     def _init_main_area(self):
         layout = self._get_main_layout()
-        self._label = QtWidgets.QLabel()
-        layout.addWidget(self._label)
+        self._image_viewer = ImageViewer()
+        layout.addWidget(self._image_viewer)
         super()._init_main_area()
 
     def _refresh_non_form_output_widgets(self):
         with self._capture_errors():
             super()._refresh_non_form_output_widgets()
             self._update_output_file()
 
     def _update_output_file(self):
-        inputs = self.get_task_input_values()
-        filename = inputs.get("filename")
-        if not filename or not os.path.isfile(filename):
-            self._label.clear()
-            return
-
-        pixmap = QtGui.QPixmap(filename)
-        self._label.setPixmap(pixmap)
+        filename = self.get_task_input_value("filename")
+        self._image_viewer.load_image(filename)
```

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import os
-from AnyQt import QtWidgets
-from AnyQt import QtGui
-
 from ewoksxrpd.tasks.diagnostics import DiagnoseCalibrateMultiResults
+from ewoksxrpd.gui.image_viewer import ImageViewer
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_diagnose_multicalib
 
 
 __all__ = ["OWDiagnoseCalibrateMultiResults"]
 
 
@@ -22,25 +19,19 @@
         parameter_info = input_parameters_diagnose_multicalib(
             self.get_default_input_values()
         )
         self._create_input_form(parameter_info)
 
     def _init_main_area(self):
         layout = self._get_main_layout()
-        self._label = QtWidgets.QLabel()
-        layout.addWidget(self._label)
+        self._image_viewer = ImageViewer()
+        layout.addWidget(self._image_viewer)
         super()._init_main_area()
 
     def _refresh_non_form_output_widgets(self):
         with self._capture_errors():
             super()._refresh_non_form_output_widgets()
             self._update_output_file()
 
     def _update_output_file(self):
-        inputs = self.get_task_input_values()
-        filename = inputs.get("filename")
-        if not filename or not os.path.isfile(filename):
-            self._label.clear()
-            return
-
-        pixmap = QtGui.QPixmap(filename)
-        self._label.setPixmap(pixmap)
+        filename = self.get_task_input_value("filename")
+        self._image_viewer.load_image(filename)
```

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-import os
-from AnyQt import QtWidgets
-from AnyQt import QtGui
-
-# from AnyQt.QtCore import Qt
 from ewoksxrpd.tasks.diagnostics import DiagnoseCalibrateSingleResults
+from ewoksxrpd.gui.image_viewer import ImageViewer
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_diagnose_singlecalib
 
 
 __all__ = ["OWDiagnoseCalibrateSingleResults"]
 
 
@@ -23,26 +19,19 @@
         parameter_info = input_parameters_diagnose_singlecalib(
             self.get_default_input_values()
         )
         self._create_input_form(parameter_info)
 
     def _init_main_area(self):
         layout = self._get_main_layout()
-        self._label = QtWidgets.QLabel()
-        layout.addWidget(self._label)
+        self._image_viewer = ImageViewer()
+        layout.addWidget(self._image_viewer)
         super()._init_main_area()
 
     def _refresh_non_form_output_widgets(self):
         with self._capture_errors():
             super()._refresh_non_form_output_widgets()
             self._update_output_file()
 
     def _update_output_file(self):
-        inputs = self.get_task_input_values()
-        filename = inputs.get("filename")
-        if not filename or not os.path.isfile(filename):
-            self._label.clear()
-            return
-
-        pixmap = QtGui.QPixmap(filename)
-        # pixmap = pixmap.scaled(10,5,Qt.KeepAspectRatio)
-        self._label.setPixmap(pixmap)
+        filename = self.get_task_input_value("filename")
+        self._image_viewer.load_image(filename)
```

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/icons/category.png` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/icons/category.png`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/icons/widget.png` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/icons/widget.png`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/integrate1d.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/integrate1d.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/mask.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/mask.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/nexus.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/nexus.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,33 +31,38 @@
             super()._refresh_non_form_output_widgets()
             self._update_plot()
 
     def _update_plot(self):
         self._plot.remove(kind="curve")
 
         url = self.get_task_input_value("url")
+        url = self.get_task_input_value("external_url", url)
         if not url:
             return
         url = DataUrl(url)
         if not os.path.exists(url.file_path()):
             return
 
-        with h5py.File(url.file_path(), "r") as parent:
-            data_path = url.data_path()
-            if not data_path:
-                data_path = "/"
-            parent = parent[data_path]
-            while "default" in parent.attrs:
-                parent = parent[parent.attrs["default"]]
-            attrs = dict(parent.attrs)
+        nxprocess_name = self.get_task_input_value("nxprocess_name")
+
+        with h5py.File(url.file_path(), "r") as nxroot:
+            data_path = url.data_path() or "results"
+            nxprocess = nxroot[data_path].get(nxprocess_name)
+            if nxprocess is None:
+                return
+            nxdata = nxprocess.get("integrated")
+            if nxdata is None:
+                return
+            attrs = dict(nxdata.attrs)
             if {"axes", "signal"} - attrs.keys():
                 return
 
             xname = attrs["axes"][0]
             yname = attrs["signal"]
-            x = parent[xname]
+            x = nxdata[xname]
             xunits = x.attrs["units"]
-            y = parent[yname]
+            y = nxdata[yname]
 
-            self._plot.addCurve(
+            curve = self._plot.addCurve(
                 x[()], y[()], xlabel=f"{xname} ({xunits})", ylabel=yname
             )
+            self._plot.setActiveCurve(curve)
```

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.7.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py` & `ewoksxrpd-0.8.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py`

 * *Files identical despite different names*

