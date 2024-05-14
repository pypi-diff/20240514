# Comparing `tmp/modelcraft-4.0.0.tar.gz` & `tmp/modelcraft-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelcraft-4.0.0.tar", last modified: Mon Mar 18 09:36:46 2024, max compression
+gzip compressed data, was "modelcraft-4.0.1.tar", last modified: Tue May 14 11:57:48 2024, max compression
```

## Comparing `modelcraft-4.0.0.tar` & `modelcraft-4.0.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.282873 modelcraft-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-03-18 09:36:33.000000 modelcraft-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-18 09:36:33.000000 modelcraft-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-18 09:36:46.282873 modelcraft-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-18 09:36:33.000000 modelcraft-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.266873 modelcraft-4.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.266873 modelcraft-4.0.0/docs/css/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-18 09:36:33.000000 modelcraft-4.0.0/docs/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-03-18 09:36:33.000000 modelcraft-4.0.0/docs/css/milligram.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-18 09:36:33.000000 modelcraft-4.0.0/docs/css/normalize.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.266873 modelcraft-4.0.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (127)    39305 2024-03-18 09:36:33.000000 modelcraft-4.0.0/docs/img/modelcraft.png
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-03-18 09:36:33.000000 modelcraft-4.0.0/docs/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.270873 modelcraft-4.0.0/modelcraft/
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14606 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/combine.py
--rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/contents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.270873 modelcraft-4.0.0/modelcraft/coot/
--rw-r--r--   0 runner    (1001) docker     (127)    35851 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/coot/prune.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1847 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/coot/sidechains.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/environ.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.274873 modelcraft-4.0.0/modelcraft/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/acedrg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/acorn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/buccaneer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/comit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/coot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/ctruncate.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/emda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/findwaters.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/freerflag.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/libg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/molrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/nautilus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/parrot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/phasematch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/refmac.py
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/servalcat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/jobs/sheetbend.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/maps.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5133 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/modelcraftem.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12791 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/modelcraftxray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/monlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/reflections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.274873 modelcraft-4.0.0/modelcraft/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/scripts/contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/scripts/copies.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/scripts/modelcraft.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/solvent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4122 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.274873 modelcraft-4.0.0/modelcraft/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.282873 modelcraft-4.0.0/modelcraft/tests/ccp4/
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_acedrg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_buccaneer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_comit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_coot.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_copies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_ctruncate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_findwaters.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_freerflag.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_libg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_molrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_monlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_nautilus.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_parrot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_phasematch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_reflections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_refmac.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_sheetbend.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_solvent.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccp4/test_xray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.282873 modelcraft-4.0.0/modelcraft/tests/ccpem/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccpem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccpem/test_em.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccpem/test_emda.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccpem/test_refmac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/ccpem/test_servalcat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.282873 modelcraft-4.0.0/modelcraft/tests/unittests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/unittests/test_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/tests/unittests/test_reflections.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-18 09:36:33.000000 modelcraft-4.0.0/modelcraft/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:36:46.282873 modelcraft-4.0.0/modelcraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-18 09:36:46.000000 modelcraft-4.0.0/modelcraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-03-18 09:36:46.000000 modelcraft-4.0.0/modelcraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 09:36:46.000000 modelcraft-4.0.0/modelcraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-18 09:36:46.000000 modelcraft-4.0.0/modelcraft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-18 09:36:46.000000 modelcraft-4.0.0/modelcraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-18 09:36:46.000000 modelcraft-4.0.0/modelcraft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-18 09:36:46.282873 modelcraft-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-18 09:36:33.000000 modelcraft-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.159637 modelcraft-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-14 11:57:40.000000 modelcraft-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 11:57:40.000000 modelcraft-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-14 11:57:48.159637 modelcraft-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-14 11:57:40.000000 modelcraft-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.143637 modelcraft-4.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.147637 modelcraft-4.0.1/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-14 11:57:40.000000 modelcraft-4.0.1/docs/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-14 11:57:40.000000 modelcraft-4.0.1/docs/css/milligram.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-14 11:57:40.000000 modelcraft-4.0.1/docs/css/normalize.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.147637 modelcraft-4.0.1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    39305 2024-05-14 11:57:40.000000 modelcraft-4.0.1/docs/img/modelcraft.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-05-14 11:57:40.000000 modelcraft-4.0.1/docs/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.147637 modelcraft-4.0.1/modelcraft/
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14606 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/contents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.151637 modelcraft-4.0.1/modelcraft/coot/
+-rw-r--r--   0 runner    (1001) docker     (127)    35851 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/coot/prune.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1847 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/coot/sidechains.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.151637 modelcraft-4.0.1/modelcraft/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/acedrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/acorn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/buccaneer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/comit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/coot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/ctruncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/emda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/findwaters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/freerflag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/libg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/molrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/nautilus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/parrot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/phasematch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/refmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/servalcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/jobs/sheetbend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5133 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/modelcraftem.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12791 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/modelcraftxray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/monlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/reflections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.155637 modelcraft-4.0.1/modelcraft/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/scripts/contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/scripts/copies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/scripts/modelcraft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/solvent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4122 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.155637 modelcraft-4.0.1/modelcraft/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.159637 modelcraft-4.0.1/modelcraft/tests/ccp4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_acedrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_buccaneer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_comit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_coot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_copies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_ctruncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_findwaters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_freerflag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_libg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_molrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_monlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_nautilus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_parrot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_phasematch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_reflections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_refmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_sheetbend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_solvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccp4/test_xray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.159637 modelcraft-4.0.1/modelcraft/tests/ccpem/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccpem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccpem/test_em.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccpem/test_emda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccpem/test_refmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/ccpem/test_servalcat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.159637 modelcraft-4.0.1/modelcraft/tests/unittests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/unittests/test_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/tests/unittests/test_reflections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-14 11:57:40.000000 modelcraft-4.0.1/modelcraft/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:57:48.159637 modelcraft-4.0.1/modelcraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-14 11:57:48.000000 modelcraft-4.0.1/modelcraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-14 11:57:48.000000 modelcraft-4.0.1/modelcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:57:48.000000 modelcraft-4.0.1/modelcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-14 11:57:48.000000 modelcraft-4.0.1/modelcraft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 11:57:48.000000 modelcraft-4.0.1/modelcraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 11:57:48.000000 modelcraft-4.0.1/modelcraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 11:57:48.159637 modelcraft-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-14 11:57:40.000000 modelcraft-4.0.1/setup.py
```

### Comparing `modelcraft-4.0.0/LICENSE` & `modelcraft-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/PKG-INFO` & `modelcraft-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelcraft
-Version: 4.0.0
+Version: 4.0.1
 Summary: Automated model building pipeline for X-ray crystallography
 Home-page: https://github.com/paulsbond/modelcraft
 Author: Paul Bond
 Author-email: paul.bond@york.ac.uk
 License: LGPL-2.1
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
```

### Comparing `modelcraft-4.0.0/README.md` & `modelcraft-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/docs/css/milligram.min.css` & `modelcraft-4.0.1/docs/css/milligram.min.css`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/docs/css/normalize.min.css` & `modelcraft-4.0.1/docs/css/normalize.min.css`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/docs/img/modelcraft.png` & `modelcraft-4.0.1/docs/img/modelcraft.png`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/docs/index.html` & `modelcraft-4.0.1/docs/index.html`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/__init__.py` & `modelcraft-4.0.1/modelcraft/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "4.0.0"
+__version__ = "4.0.1"
 
 from .cell import max_distortion as max_cell_distortion
 from .cell import remove_scale
 from .cell import update_cell
 from .contents import AsuContents
 from .contents import PolymerType
 from .geometry import rmsz
```

### Comparing `modelcraft-4.0.0/modelcraft/arguments.py` & `modelcraft-4.0.1/modelcraft/arguments.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/cell.py` & `modelcraft-4.0.1/modelcraft/cell.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/combine.py` & `modelcraft-4.0.1/modelcraft/combine.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/contents.py` & `modelcraft-4.0.1/modelcraft/contents.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/coot/prune.py` & `modelcraft-4.0.1/modelcraft/coot/prune.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/coot/sidechains.py` & `modelcraft-4.0.1/modelcraft/coot/sidechains.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/environ.py` & `modelcraft-4.0.1/modelcraft/environ.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/geometry.py` & `modelcraft-4.0.1/modelcraft/geometry.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/job.py` & `modelcraft-4.0.1/modelcraft/job.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/acedrg.py` & `modelcraft-4.0.1/modelcraft/jobs/acedrg.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/acorn.py` & `modelcraft-4.0.1/modelcraft/jobs/acorn.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/buccaneer.py` & `modelcraft-4.0.1/modelcraft/jobs/buccaneer.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/comit.py` & `modelcraft-4.0.1/modelcraft/jobs/comit.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/coot.py` & `modelcraft-4.0.1/modelcraft/jobs/coot.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/ctruncate.py` & `modelcraft-4.0.1/modelcraft/jobs/ctruncate.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/emda.py` & `modelcraft-4.0.1/modelcraft/jobs/emda.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/findwaters.py` & `modelcraft-4.0.1/modelcraft/jobs/findwaters.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/freerflag.py` & `modelcraft-4.0.1/modelcraft/jobs/freerflag.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/libg.py` & `modelcraft-4.0.1/modelcraft/jobs/libg.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/molrep.py` & `modelcraft-4.0.1/modelcraft/jobs/molrep.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/nautilus.py` & `modelcraft-4.0.1/modelcraft/jobs/nautilus.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/parrot.py` & `modelcraft-4.0.1/modelcraft/jobs/parrot.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/phasematch.py` & `modelcraft-4.0.1/modelcraft/jobs/phasematch.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/refmac.py` & `modelcraft-4.0.1/modelcraft/jobs/refmac.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/servalcat.py` & `modelcraft-4.0.1/modelcraft/jobs/servalcat.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/jobs/sheetbend.py` & `modelcraft-4.0.1/modelcraft/jobs/sheetbend.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/modelcraftem.py` & `modelcraft-4.0.1/modelcraft/modelcraftem.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/modelcraftxray.py` & `modelcraft-4.0.1/modelcraft/modelcraftxray.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/monlib.py` & `modelcraft-4.0.1/modelcraft/monlib.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 @functools.lru_cache(maxsize=None)
 def in_library(code: str) -> bool:
     return os.path.exists(_path(code))
 
 
 @functools.lru_cache(maxsize=None)
 def group(code: str) -> gemmi.ChemComp.Group:
-    doc = gemmi.cif.read(_path(code))
-    monlib = gemmi.MonLib()
-    monlib.read_monomer_doc(doc)
-    return monlib.monomers[code].group
+    if in_library(code):
+        doc = gemmi.cif.read(_path(code))
+        monlib = gemmi.MonLib()
+        monlib.read_monomer_doc(doc)
+        return monlib.monomers[code].group
+    return None
 
 
 @functools.lru_cache(maxsize=None)
 def is_protein(code: str) -> bool:
     return group(code) in {
         gemmi.ChemComp.Group.Peptide,
         gemmi.ChemComp.Group.PPeptide,
```

### Comparing `modelcraft-4.0.0/modelcraft/pipeline.py` & `modelcraft-4.0.1/modelcraft/pipeline.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/reflections.py` & `modelcraft-4.0.1/modelcraft/reflections.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/scripts/contents.py` & `modelcraft-4.0.1/modelcraft/scripts/contents.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/scripts/copies.py` & `modelcraft-4.0.1/modelcraft/scripts/copies.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/solvent.py` & `modelcraft-4.0.1/modelcraft/solvent.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/structure.py` & `modelcraft-4.0.1/modelcraft/structure.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/__init__.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/__init__.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_acedrg.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_acedrg.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_arguments.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_arguments.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_buccaneer.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_buccaneer.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_cell.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_cell.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_comit.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_comit.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_contents.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_contents.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_coot.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_coot.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_ctruncate.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_ctruncate.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_findwaters.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_findwaters.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_geometry.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_geometry.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_molrep.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_molrep.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_monlib.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_monlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,36 +22,40 @@
 def test_in_library():
     for code in PROTEIN_CODES.values():
         assert in_library(code)
     for code in DNA_CODES.values():
         assert in_library(code)
     for code in RNA_CODES.values():
         assert in_library(code)
+    assert not in_library("NOT_IN_MONLIB")
 
 
 def test_group():
     assert group("GLY") == gemmi.ChemComp.Group.Peptide
     assert group("ALA") == gemmi.ChemComp.Group.Peptide
     assert group("MSE") == gemmi.ChemComp.Group.Peptide
     assert group("PRO") == gemmi.ChemComp.Group.PPeptide
     assert group("U") == gemmi.ChemComp.Group.Rna
     assert group("DT") == gemmi.ChemComp.Group.Dna
     assert group("HOH") == gemmi.ChemComp.Group.NonPolymer
+    assert group("NOT_IN_MONLIB") is None
 
 
 def test_protein():
     assert is_protein("GLY")
     assert is_protein("ALA")
     assert is_protein("MSE")
     assert is_protein("PRO")
     assert not is_protein("U")
     assert not is_protein("DT")
     assert not is_protein("HOH")
+    assert not is_protein("NOT_IN_MONLIB")
 
 
 def test_nucleic():
     assert not is_nucleic("GLY")
     assert not is_nucleic("ALA")
     assert not is_nucleic("PRO")
     assert is_nucleic("U")
     assert is_nucleic("DT")
     assert not is_nucleic("HOH")
+    assert not is_nucleic("NOT_IN_MONLIB")
```

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_nautilus.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_nautilus.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_parrot.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_parrot.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_phasematch.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_phasematch.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_reflections.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_reflections.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_refmac.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_refmac.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_sheetbend.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_sheetbend.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_solvent.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_solvent.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccp4/test_xray.py` & `modelcraft-4.0.1/modelcraft/tests/ccp4/test_xray.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccpem/__init__.py` & `modelcraft-4.0.1/modelcraft/tests/ccpem/__init__.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccpem/test_em.py` & `modelcraft-4.0.1/modelcraft/tests/ccpem/test_em.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/ccpem/test_servalcat.py` & `modelcraft-4.0.1/modelcraft/tests/ccpem/test_servalcat.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/unittests/test_contents.py` & `modelcraft-4.0.1/modelcraft/tests/unittests/test_contents.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft/tests/unittests/test_reflections.py` & `modelcraft-4.0.1/modelcraft/tests/unittests/test_reflections.py`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/modelcraft.egg-info/PKG-INFO` & `modelcraft-4.0.1/modelcraft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelcraft
-Version: 4.0.0
+Version: 4.0.1
 Summary: Automated model building pipeline for X-ray crystallography
 Home-page: https://github.com/paulsbond/modelcraft
 Author: Paul Bond
 Author-email: paul.bond@york.ac.uk
 License: LGPL-2.1
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
```

### Comparing `modelcraft-4.0.0/modelcraft.egg-info/SOURCES.txt` & `modelcraft-4.0.1/modelcraft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelcraft-4.0.0/setup.py` & `modelcraft-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 setuptools.setup(
     name="modelcraft",
-    version="4.0.0",
+    version="4.0.1",
     author="Paul Bond",
     author_email="paul.bond@york.ac.uk",
     description="Automated model building pipeline for X-ray crystallography",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/paulsbond/modelcraft",
     packages=setuptools.find_packages(),
```

