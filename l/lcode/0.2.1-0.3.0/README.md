# Comparing `tmp/lcode-0.2.1.tar.gz` & `tmp/lcode-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcode-0.2.1.tar", last modified: Tue Mar 12 10:05:31 2024, max compression
+gzip compressed data, was "lcode-0.3.0.tar", last modified: Tue May 14 08:10:11 2024, max compression
```

## Comparing `lcode-0.2.1.tar` & `lcode-0.3.0.tar`

### file list

```diff
@@ -1,89 +1,97 @@
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.274033 lcode-0.2.1/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2200 2024-03-12 08:52:48.000000 lcode-0.2.1/LICENSE
--rw-r--r--   0 tuev      (1000) tuev      (1000)     2471 2024-03-12 10:05:31.274033 lcode-0.2.1/PKG-INFO
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1630 2024-03-12 08:52:48.000000 lcode-0.2.1/README.md
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.266033 lcode-0.2.1/lcode/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      142 2024-03-12 10:05:10.000000 lcode-0.2.1/lcode/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1273 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/__main__.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.270033 lcode-0.2.1/lcode/alt_beam_generator/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/alt_beam_generator/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     7164 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/alt_beam_generator/beam_generator.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2470 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/alt_beam_generator/beam_segment_shape.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1458 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/alt_beam_generator/beam_shape.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1756 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/alt_beam_generator/eshape.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2334 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/alt_beam_generator/rshape.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1496 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/alt_beam_generator/xishape.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.270033 lcode-0.2.1/lcode/beam/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      259 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    18329 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam/beam_calculate.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     5422 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam/beam_io.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     4408 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam/data.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam/profiles.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2232 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam/weights.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.270033 lcode-0.2.1/lcode/beam3d/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      382 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam3d/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     7036 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam3d/beam_calculator.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     3240 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam3d/beam_io.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     7220 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam3d/data.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    12898 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam3d/move.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     5119 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam3d/weights.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.270033 lcode-0.2.1/lcode/beam_generator/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)       31 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam_generator/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     4901 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam_generator/beam_generator.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     6595 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam_generator/beam_generator2.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     6379 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/beam_generator/beam_profiles.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.270033 lcode-0.2.1/lcode/config/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)       27 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/config/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     8288 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/config/config.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      157 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/config/default_config.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2854 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/config/default_config_values.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     3229 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/config/template.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.270033 lcode-0.2.1/lcode/diagnostics/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/diagnostics/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    33353 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/diagnostics/diagnostics_3d.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      464 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/diagnostics/diagnostics_class.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2320 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/diagnostics/diagnostics_list.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      120 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/diagnostics/process.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     7661 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/diagnostics/targets.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.270033 lcode-0.2.1/lcode/examples/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:10.000000 lcode-0.2.1/lcode/examples/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1603 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/examples/ssm.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.270033 lcode-0.2.1/lcode/mpi/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)       74 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/mpi/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     3747 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/mpi/beam_io.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1860 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/mpi/transport.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1646 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/mpi/util.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.270033 lcode-0.2.1/lcode/plasma/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      115 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1134 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma/data.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     8310 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma/fields.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     3310 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma/initialization.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     7977 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma/move.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2450 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma/ode.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     4718 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma/profiles.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     4648 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma/rhoj.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     3815 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma/solver.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.274033 lcode-0.2.1/lcode/plasma3d/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      115 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma3d/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     8842 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma3d/arraytools.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1134 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma3d/data.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    13029 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma3d/fields.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    21438 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma3d/initialization.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    13734 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma3d/move.py
--rwxrwxr-x   0 tuev      (1000) tuev      (1000)     9137 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma3d/noise_filter.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      748 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma3d/rhoj.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    14044 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma3d/savgol_filter_cp.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     3004 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma3d/solver.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    11217 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/plasma3d/weights.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.274033 lcode-0.2.1/lcode/push_solvers/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/push_solvers/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    10550 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/push_solvers/push_solver.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    11524 2024-03-12 08:52:48.000000 lcode-0.2.1/lcode/simulation.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-03-12 10:05:31.266033 lcode-0.2.1/lcode.egg-info/
--rw-r--r--   0 tuev      (1000) tuev      (1000)     2471 2024-03-12 10:05:31.000000 lcode-0.2.1/lcode.egg-info/PKG-INFO
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1984 2024-03-12 10:05:31.000000 lcode-0.2.1/lcode.egg-info/SOURCES.txt
--rw-rw-r--   0 tuev      (1000) tuev      (1000)        1 2024-03-12 10:05:31.000000 lcode-0.2.1/lcode.egg-info/dependency_links.txt
--rw-rw-r--   0 tuev      (1000) tuev      (1000)       36 2024-03-12 10:05:31.000000 lcode-0.2.1/lcode.egg-info/requires.txt
--rw-rw-r--   0 tuev      (1000) tuev      (1000)        6 2024-03-12 10:05:31.000000 lcode-0.2.1/lcode.egg-info/top_level.txt
--rw-rw-r--   0 tuev      (1000) tuev      (1000)       38 2024-03-12 10:05:31.274033 lcode-0.2.1/setup.cfg
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1350 2024-03-12 08:52:48.000000 lcode-0.2.1/setup.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.843410 lcode-0.3.0/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2200 2024-03-12 08:52:48.000000 lcode-0.3.0/LICENSE
+-rw-r--r--   0 tuev      (1000) tuev      (1000)     2543 2024-05-14 08:10:11.839410 lcode-0.3.0/PKG-INFO
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1702 2024-05-14 06:32:26.000000 lcode-0.3.0/README.md
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.815409 lcode-0.3.0/lcode/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      142 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1288 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/__main__.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.819409 lcode-0.3.0/lcode/alt_beam_generator/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     7164 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/beam_generator.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2470 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/beam_segment_shape.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1458 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/beam_shape.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1756 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/eshape.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2334 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/rshape.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1496 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/xishape.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.823409 lcode-0.3.0/lcode/beam/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      259 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    18315 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam/beam_calculate.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     5729 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam/beam_io.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     5580 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam/data.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam/profiles.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2232 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam/weights.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.827410 lcode-0.3.0/lcode/beam3d/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      382 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam3d/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     7022 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam3d/beam_calculator.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     3329 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam3d/beam_io.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     7220 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam3d/data.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    12891 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam3d/move.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     5112 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam3d/weights.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.827410 lcode-0.3.0/lcode/beam_generator/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)       31 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam_generator/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     4901 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam_generator/beam_generator.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     6595 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam_generator/beam_generator2.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     6379 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam_generator/beam_profiles.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.831410 lcode-0.3.0/lcode/config/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)       27 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/config/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    10536 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/config/config.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      157 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/config/default_config.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     3296 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/config/default_config_values.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     3222 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/config/template.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.835409 lcode-0.3.0/lcode/diagnostics/
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.835409 lcode-0.3.0/lcode/diagnostics/FXi/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     5332 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/FXi/FXi.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      466 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/FXi/Strategy.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     3928 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/FXi/Strategy3D.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2148 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/FXi/StrategyCircular.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)       35 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/FXi/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      154 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    33325 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/diagnostics_3d.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      464 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/diagnostics/diagnostics_class.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2320 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/diagnostics/diagnostics_list.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     4115 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/particles.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      120 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/diagnostics/process.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    19254 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/slice.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     7654 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/targets.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1790 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/utils.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.835409 lcode-0.3.0/lcode/examples/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     9778 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/examples/high-R.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1196 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/examples/original-ssm.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.835409 lcode-0.3.0/lcode/mpi/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)       74 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/mpi/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     4077 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/mpi/beam_io.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1860 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/mpi/transport.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1646 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/mpi/util.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.839410 lcode-0.3.0/lcode/plasma/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      115 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/plasma/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1287 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/data.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     8303 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/fields.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     4499 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/initialization.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     7970 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/move.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2450 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/plasma/ode.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     4711 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/profiles.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     4641 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/rhoj.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     3822 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/solver.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.839410 lcode-0.3.0/lcode/plasma3d/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      115 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/plasma3d/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1292 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/data.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    13022 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/fields.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    20487 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/initialization.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    14630 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/move.py
+-rwxrwxr-x   0 tuev      (1000) tuev      (1000)    11495 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/noise_filter.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     5942 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/profile.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      748 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/plasma3d/rhoj.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     3002 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/solver.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    11309 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/weights.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.839410 lcode-0.3.0/lcode/push_solvers/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/push_solvers/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    11080 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/push_solvers/push_solver.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    11311 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/simulation.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.815409 lcode-0.3.0/lcode.egg-info/
+-rw-r--r--   0 tuev      (1000) tuev      (1000)     2543 2024-05-14 08:10:11.000000 lcode-0.3.0/lcode.egg-info/PKG-INFO
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2213 2024-05-14 08:10:11.000000 lcode-0.3.0/lcode.egg-info/SOURCES.txt
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)        1 2024-05-14 08:10:11.000000 lcode-0.3.0/lcode.egg-info/dependency_links.txt
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)       36 2024-05-14 08:10:11.000000 lcode-0.3.0/lcode.egg-info/requires.txt
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)        6 2024-05-14 08:10:11.000000 lcode-0.3.0/lcode.egg-info/top_level.txt
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)       38 2024-05-14 08:10:11.843410 lcode-0.3.0/setup.cfg
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1534 2024-05-14 06:32:26.000000 lcode-0.3.0/setup.py
```

### Comparing `lcode-0.2.1/LICENSE` & `lcode-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/PKG-INFO` & `lcode-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcode
-Version: 0.2.1
+Version: 0.3.0
 Summary: LCODE is a free software for simulationplasma wakefield acceleration based on QSA.
 Home-page: https://lcode.info
 Download-URL: https://github.com/lcodePy-team/lcodePy
 Author: lcodePy-team
 Author-email: team@lcode.info
 License: BSD-3-Clause-extended
 Keywords: plasma wakefield acceleration,quasistatic approximation,numerical simulation
@@ -27,19 +27,19 @@
 ## Overview 
 
 LCODE is a free software for numerical simulation of
 particle beam-driven plasma wakefield acceleration.
 LCODE is based on the quasistatic approximation, capable
 of simulation in 2D and 3D geometry, and can use GPUs and CPUs.
 
-For now, this is new and experimental software. This is
+For now, this under active development. This is
 a complete overhaul of the old C version in Python.
 
-You can also find a more mature 2D version of LCODE at
-http://lcode.info/.
+- **Website:** https://lcode.info
+- **Documentation:** https://lcode.info/docs
 
 ## Instalation 
 
 We use [Anaconda](https://www.continuum.io/why-anaconda) and we recommend 
 installing lcode in a separate environment. 
 Any other python installation should work fine, but has not been tested. 
 
@@ -73,9 +73,12 @@
 ```
 pip install .
 ```
 
 
 ----------
 
+You can also find a more mature 2D version of LCODE at
+http://lcode.info/.
+
 Fill free to contact `team@lcode.info` for assistance with it.
```

### Comparing `lcode-0.2.1/README.md` & `lcode-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 ## Overview 
 
 LCODE is a free software for numerical simulation of
 particle beam-driven plasma wakefield acceleration.
 LCODE is based on the quasistatic approximation, capable
 of simulation in 2D and 3D geometry, and can use GPUs and CPUs.
 
-For now, this is new and experimental software. This is
+For now, this under active development. This is
 a complete overhaul of the old C version in Python.
 
-You can also find a more mature 2D version of LCODE at
-http://lcode.info/.
+- **Website:** https://lcode.info
+- **Documentation:** https://lcode.info/docs
 
 ## Instalation 
 
 We use [Anaconda](https://www.continuum.io/why-anaconda) and we recommend 
 installing lcode in a separate environment. 
 Any other python installation should work fine, but has not been tested. 
 
@@ -49,9 +49,12 @@
 ```
 pip install .
 ```
 
 
 ----------
 
+You can also find a more mature 2D version of LCODE at
+http://lcode.info/.
+
 Fill free to contact `team@lcode.info` for assistance with it.
```

### Comparing `lcode-0.2.1/lcode/__main__.py` & `lcode-0.3.0/lcode/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import argparse
 from lcode import __version__
 
 __EXAMPLE_DIR = os.path.join(os.path.dirname(__file__), 'examples')
 def get_available_configs():
     configs = os.listdir(__EXAMPLE_DIR)
-    configs = [config.replace('.py', '') for config in configs]
+    configs = [conf.replace('.py', '') for conf in configs if conf[0] != '_']
     return configs
 
 def main():
     parser = argparse.ArgumentParser(prog="LCODE", usage="%(prog)s [options]")
 
     parser.add_argument("--version", action="version", version=f"%(prog)s {__version__}")
     subparsers = parser.add_subparsers(help="sub-command help", dest="subparser_name")
@@ -18,15 +18,15 @@
     __available_configs = get_available_configs()
     generate_parser.add_argument('config_name', type=str, help="Name of the config: {}".format(", ".join(__available_configs)))
     args = parser.parse_args()
     
 
     if args.subparser_name == "get":
         if args.config_name not in __available_configs:
-            print(f'Choose from {" ,".join(__available_configs)}')
+            print(f'Choose from: {", ".join(__available_configs)}')
             return
         with open(os.path.join(__EXAMPLE_DIR,'{}.py'.format(args.config_name)), 'r') as input, \
              open('run.py', 'w') as output:
             output.write(input.read())
```

### Comparing `lcode-0.2.1/lcode/alt_beam_generator/beam_generator.py` & `lcode-0.3.0/lcode/alt_beam_generator/beam_generator.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/alt_beam_generator/beam_segment_shape.py` & `lcode-0.3.0/lcode/alt_beam_generator/beam_segment_shape.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/alt_beam_generator/beam_shape.py` & `lcode-0.3.0/lcode/alt_beam_generator/beam_shape.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/alt_beam_generator/eshape.py` & `lcode-0.3.0/lcode/alt_beam_generator/eshape.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/alt_beam_generator/rshape.py` & `lcode-0.3.0/lcode/alt_beam_generator/rshape.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/alt_beam_generator/xishape.py` & `lcode-0.3.0/lcode/alt_beam_generator/xishape.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/beam/beam_calculate.py` & `lcode-0.3.0/lcode/beam/beam_calculate.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         The set of base parameters to perform the simulation.
     
     Returns
     -------
     push_particles : function
         Function that calculates the motion of the beam particles.
     """
-    r_step = float(config.get('window-width-step-size'))
+    r_step = float(config.get('transverse-step'))
     xi_step_p = float(config.get('xi-step'))
     max_radius = float(config.get('window-width'))
     lost_boundary = max(0.9 * max_radius, max_radius - 1)
     magnetic_field = config.getfloat('magnetic-field')
     locals_spec = {'r_step': nb.float64,
                    'xi_step': nb.float64,
                    'lost_boundary': nb.float64,
@@ -363,15 +363,15 @@
         
         Paramters 
         ---------
         config : Config
             The set of base parameters to perform the simulation.
         """
         # Get main calculation parameters.
-        self.r_step = config.getfloat('window-width-step-size')
+        self.r_step = config.getfloat('transverse-step')
         self.grid_steps = int(config.getfloat('window-width') / self.r_step) + 1
         self.xi_step = config.getfloat('xi-step')
         self.move_beam_slice = get_beam_slice_mover(config)
 
     def start_time_step(self):
         """
         Initialization of array to collect the partial beam density.
```

### Comparing `lcode-0.2.1/lcode/beam/beam_io.py` & `lcode-0.3.0/lcode/beam/beam_io.py`

 * *Files 12% similar despite different names*

```diff
@@ -123,14 +123,18 @@
     def push_lost(self, time, beam_slice: BeamParticles):
         if beam_slice.size > 0:
             print(f'MemoryBeamDrain: lost {beam_slice.size} particles')
             self._beam_buffer_lost.append(beam_slice)
 
     def beam_slice(self):
         return np.concatenate([beam_slice.particles for beam_slice in self._beam_buffer]) if len(self._beam_buffer )> 0 else np.array([], dtype = particle_dtype)
+    
+    def save(self, *args, **kwargs):
+        slice = np.array(self.beam_slice(), dtype = particle_dtype)
+        np.savez_compressed(*args, **kwargs, xi = slice['xi'], r = slice['r'], pz = slice['p_z'], pr = slice['p_r'], M = slice['M'], q_m = slice['q_m'], q_norm = slice['q_norm'], id = slice['id'])
 
 
 class DebugSource(BeamSource):
     def __init__(self, source):
         self._source = source
         self._beam_buffer = []
```

### Comparing `lcode-0.2.1/lcode/beam/data.py` & `lcode-0.3.0/lcode/beam/data.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 
 particle_dtype = np.dtype([('xi', 'f8'), ('r', 'f8'), ('p_z', 'f8'),
                            ('p_r', 'f8'), ('M', 'f8'), ('q_m', 'f8'),
                            ('q_norm', 'f8'), ('id', 'i8')])
 
 class BeamParticles:
-    def __init__(self, size, particles=None):
+    def __init__(self, size=0, particles=None):
         self.size = size
         if particles is not None:
             self.particles = particles
         else:
             self.particles = np.zeros(size, dtype=particle_dtype)
         self.xi = self.particles['xi']
         self.r = self.particles['r']
@@ -102,7 +102,33 @@
         self.q_norm = self.particles['q_norm']
         self.id = self.particles['id']
 
         self.dt = self.dt[sorted_idxes]
         self.remaining_steps = self.remaining_steps[sorted_idxes]
         self.lost = self.lost[sorted_idxes]
 
+    def load(self, *args, **kwargs):
+        with np.load(*args, **kwargs) as loaded:
+            self.size = loaded['xi'].shape[0]
+            self.particles = np.zeros(self.size, dtype=particle_dtype)
+            self.particles['xi'] = loaded['xi']
+            self.particles['r'] = loaded['r']
+            self.particles['p_r'] = loaded['p_r']
+            self.particles['p_z'] = loaded['p_z']
+            self.particles['M'] = loaded['M']
+            self.particles['q_m'] = loaded['q_m']
+            self.particles['q_norm'] = loaded['q_norm']
+            self.particles['id'] = loaded['id']
+            self.xi = self.particles['xi']
+            self.r = self.particles['r']
+            self.p_r = self.particles['p_r']
+            self.p_z = self.particles['p_z']
+            self.M = self.particles['M']
+            self.q_m = self.particles['q_m']
+            self.q_norm = self.particles['q_norm']
+            self.id = self.particles['id']
+
+            self.dt = np.zeros(self.size, dtype=np.float64)
+            self.remaining_steps = np.ones(self.size, dtype=np.int64)
+
+            self.nlost = 0
+            self.lost = np.zeros(self.size, dtype=np.bool_)
```

### Comparing `lcode-0.2.1/lcode/beam/weights.py` & `lcode-0.3.0/lcode/beam/weights.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/beam3d/beam_calculator.py` & `lcode-0.3.0/lcode/beam3d/beam_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 # ----- A class for a beam consisting of macroparticles -----
 
 class BeamCalculator:
     def __init__(self, config: Config):
         # Get main calculation parameters.
         self.xp = config.xp
 
-        self.grid_step_size = config.getfloat('window-width-step-size')
+        self.grid_step_size = config.getfloat('transverse-step')
         self.grid_steps = config.getint('window-width-steps')
         self.time_step = config.getfloat('time-step')
         self.substep_energy = config.getfloat('beam-substepping-energy')
 
         self.deposit = get_deposit_beam(config)
         self.move_particles = get_move_beam_particles(config)
 
@@ -149,15 +149,15 @@
     def __init__(self, config: Config):
         # Get main calculation parameters.
         self.xp = config.xp
         self.xi_step_size = config.getfloat('xi-step')
         
         # Creates a transversal grid
         grid_steps     = config.getint('window-width-steps')
-        grid_step_size = config.getfloat('window-width-step-size')
+        grid_step_size = config.getfloat('transverse-step')
 
         grid = ((self.xp.arange(grid_steps) - grid_steps // 2)
                 * grid_step_size)
         self.x_grid, self.y_grid = self.xp.meshgrid(grid, grid)
     
     def start_time_step(self):
         """A dummy function for the rigid-beam mode."""
```

### Comparing `lcode-0.2.1/lcode/beam3d/beam_io.py` & `lcode-0.3.0/lcode/beam3d/beam_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,17 @@
         Add lost beam particles to the buffer of lost particles.
         """
         if lost_layer.id.size > 0:
             self.lost_buffer.append(lost_layer)
     
     def beam_slice(self):
         return self.beam_buffer
+    
+    def save(self, *args, **kwargs):
+        self.beam_buffer.save(*args, **kwargs)
 
 
 # ----- Classes for a rigid beam -----
 
 class RigidBeamSource:
     def __init__(self, config: Config, beam_charge_distribution_function):
         # From input parameters:
```

### Comparing `lcode-0.2.1/lcode/beam3d/data.py` & `lcode-0.3.0/lcode/beam3d/data.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/beam3d/move.py` & `lcode-0.3.0/lcode/beam3d/move.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
         name='move_beam_cupy', preamble=weight1_cupy+weight4_cupy,
         no_return=True
     )
 
 
 def get_move_beam_particles(config: Config):
     xi_step_size = config.getfloat('xi-step')
-    grid_step_size = config.getfloat('window-width-step-size')
+    grid_step_size = config.getfloat('transverse-step')
     grid_steps = config.getint('window-width-steps')
 
     # Calculate the radius that marks that a particle is lost.
     max_radius = grid_step_size * grid_steps / 2
     lost_radius = max(0.9 * max_radius, max_radius - 1) # or just max_radius?
 
     pu_type = config.get('processing-unit-type').lower()
```

### Comparing `lcode-0.2.1/lcode/beam3d/weights.py` & `lcode-0.3.0/lcode/beam3d/weights.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         name='deposit_beam_cupy', preamble=weight1_cupy+weight4_cupy,
         no_return=True
     )
 
 
 def get_deposit_beam(config: Config):
     xi_step_size = config.getfloat('xi-step')
-    grid_step_size = config.getfloat('window-width-step-size')
+    grid_step_size = config.getfloat('transverse-step')
     grid_steps = config.getint('window-width-steps')
 
     pu_type = config.get('processing-unit-type').lower()
     if pu_type == 'cpu':
         deposit_beam_kernel = deposit_beam_numba
     elif pu_type == 'gpu':
         deposit_beam_kernel = get_deposit_beam_cupy()
```

### Comparing `lcode-0.2.1/lcode/beam_generator/beam_generator.py` & `lcode-0.3.0/lcode/beam_generator/beam_generator.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/beam_generator/beam_generator2.py` & `lcode-0.3.0/lcode/beam_generator/beam_generator2.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/beam_generator/beam_profiles.py` & `lcode-0.3.0/lcode/beam_generator/beam_profiles.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/config/config.py` & `lcode-0.3.0/lcode/config/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from copy import copy
+from pathlib import Path
 import numpy as np
 import re
+import lcode
 
+from copy import copy
 from typing import Any
-from .template import lcode_template
 
+from .template import lcode_template
 from .default_config_values import default_config_values
 
 
 class Config:
     # We don't really need config_values, can work with _arr. TODO: discuss this.
     # config_values: dict[str, str] # And we don't really need to declare this.
 
@@ -27,22 +29,23 @@
             self.update(default_config_values)
 
         # If a user sets new config values when initializing a new config:
         if new_config_values is not None:
             self.update(new_config_values)
 
     def get(self, option_name: str, fallback: str = '') -> str:
-        # TODO: Should we move adjusting from get() to set()?
-        self.adjust_config_values_on_get(option_name)
-
         if option_name in self.config_values:
-            return self.config_values.get(option_name)
+            return str(self.config_values.get(option_name))
         else:
             return fallback
 
+    def getraw(self, option_name):
+        return self.config_values.get(option_name)
+
+
     def getbool(self, option_name: str, fallback: bool = 0) -> bool:
         str_value = self.get(option_name).lower()
         if str_value == 'true':
             return True
         elif str_value == 'false':
             return False
         else:
@@ -57,15 +60,15 @@
     def getfloat(self, option_name: str, fallback: float = 0.0) -> float:
         try:
             return float(self.get(option_name))
         except ValueError:
             return fallback
 
     def set(self, option_name: str, option_value: Any):
-        self.config_values[option_name] = str(option_value)
+        self.config_values[option_name] = option_value
 
         # We intercept the setting of a new configuration value
         # in order to adjust other values:
         self.adjust_config_values_on_set(option_name)
 
     def update(self, new_config_values: dict=None): #, **kconfig_values):
         """
@@ -76,14 +79,78 @@
             for key in new_config_values:
                 self.set(key, new_config_values[key])
 
         # We can add this part if we want to support **karg
         # for key in kconfig_values:
         #     self.set(key, kconfig_values[key])
 
+    def dump(self, runas_name):
+        str_keys = set(['processing-unit-type',
+                        'geometry',
+                        'ion-model',
+                        'plasma-shape',
+                        'plasma-zshape', 
+                        'plasma-rshape',
+                        ])
+        if 'extra' in runas_name:
+            n_lines = -1
+        else:
+            n_lines = 94
+        
+        path_to_default = Path(__file__).parent / 'default_config_values.py'
+        conf_file = open(path_to_default,'r').readlines()
+        conf_file = ''.join(conf_file[3:n_lines]) + '}'
+        conf_file = '"""\n' \
+            + 'Simulation preformed with following lcode settings.\n' \
+            + f'Generated by lcode version {lcode.__version__}.\n' \
+            + f'Fill free to contact team@lcode.info for assistance.\n' \
+            + '"""\n\n' \
+            + 'config = {\n' \
+            + conf_file
+        for key, value in self.config_values.items():
+            old_line = fr"'{key}': .*?(?=,)"
+            if key in str_keys:
+                if key == "plasma-zshape": 
+                    profile = [8 * " " + x.strip() for x in 
+                               value.lower().strip().split('\n')]
+                    profile = r"\n".join(profile) + r"\n" + 8 * r" " + r"'''"
+                    new_line = fr"'{key}': '''\n{profile}"
+                    old_line = fr"'{key}': '''\n        '''"
+                    
+                elif key == "plasma-rshape":
+                    if isinstance(value, int):
+                        new_line = fr"'{key}': {value}"
+                        continue
+                    elif len(value.split()) == 1:
+                        new_line = fr"'{key}': '{value.lower()}'"
+                        continue
+                    profile = [8 * " " + x.strip() for x in 
+                               value.lower().strip().split('\n')]
+                    profile = r"\n".join(profile) + r"\n" + 8 * r" " + r"'''"
+                    new_line = fr"'{key}': '''\n{profile}"
+                    
+                elif key == 'plasma-shape' and callable(value):
+                    new_line = fr"'{key}': 'external function {value}'"
+                    
+                else: 
+                    new_line = fr"'{key}': '{value.lower()}'"
+            else:
+                new_line = fr"'{key}': {value}"
+            conf_file = re.sub(old_line, new_line, conf_file)
+        if self.config_values['geometry'].lower() == '3d': 
+            key = 'window-width'
+            value = float(self.config_values['window-width']) / 2
+            old_line = fr"'{key}': .*?(?=,)"
+            new_line = fr"'{key}': {value}"
+            conf_file = re.sub(old_line, new_line, conf_file)
+        
+        with open(runas_name, 'w') as f_out:
+            f_out.write(conf_file)
+        
+
     def __copy__(self) -> 'Config':
         """
         Works similarly to the copy() method of a Python dictionary.
         """
         ret = Config()
         ret.config_values = copy(self.config_values)
         return ret
@@ -91,31 +158,14 @@
     def c_config(self, path:str = None) -> str:
         cfg = lcode_template.format(**self.config_values)
         if path:
             with open(path, 'w') as cfg_f:
                 cfg_f.write(cfg)
         return cfg
 
-    def adjust_config_values_on_get(self, option_name: str):
-        """
-        Adjusts config values in 3d when we use config.get(...).
-        Required for compatibility of 2d and 3d codes.
-        """
-        if (option_name == 'window-width-steps' and
-            self.get('geometry').lower() == '3d'):
-            # Goes here every time Config.get('window-width-steps') is
-            # called in 3d to adjust window-width and window-width-steps.
-            self.adjust_window_width_and_steps_3d()
-
-        if (option_name == 'plasma-fineness' and
-            self.get('geometry').lower() == '3d'):
-            # Goes here every time Config.get('plasma-fineness') is called
-            # in 3d to adjust it according to 'plasma-particles-per-cell'.
-            self.adjust_plasma_fineness()
-
     def adjust_config_values_on_set(self, option_name: str):
         """
         Adjusts config values when we use config.set(...).
         """
         if option_name == 'processing-unit-type':
             # Goes here every time Config['processing-unit-type'] = 'cpu'/'gpu'
             # or something similar is called to change the type of the main
@@ -128,45 +178,48 @@
                 self.xp = cp
 
         if (option_name == 'geometry' and \
             self.config_values['geometry'] == "circ"):
             # 2d and circ are now the same.
             self.config_values['geometry'] = '2d'
 
-    def _correct_3d_settings(self):
+    def _adjust_config_values_3d(self):
         """
-        Adjust the width of the window to fit the 2d case.
+        Adjust some parameters for 3d simulation to fit 2D case.
+        Tweak some parameters to improve stability and performance 
         """
         if self.get('geometry')  == '3d':
             self.set('window-width', 2 * self.getfloat('window-width'))
-        if self.get('geometry')  == '3d':
-            self.set('field-solver-subtraction-coefficient', 
-                     1 + self.getfloat('xi-step'))
+            self.adjust_window_width_and_steps_3d()
+            self.adjust_plasma_fineness()
+            if self.get('field-solver-subtraction-coefficient') == '1':
+                self.set('field-solver-subtraction-coefficient', 
+                         1 + self.getfloat('xi-step'))
 
     def adjust_window_width_and_steps_3d(self):
         """
         Calculates the optimal number for window-width-steps and uses
         it to adjust window-width and window-width-steps in case of 3d.
         """
         # 0. Calculates an estimation of 'window-width-steps' value.
         estim = int(self.getfloat('window-width') /
-                    self.getfloat('window-width-step-size'))
+                    self.getfloat('transverse-step'))
 
         # 1. Calculates good numbers around the estimation.
         #    Hopefully, the difference is less than 100.
         # TODO: Rewrite so that there are no exceptions.
         lower_bound = (estim - 100) if (estim - 100) > 0 else 0
         good_numbers = np.array([a for a in range(lower_bound, estim + 100)
                                  if good_size(a)])
 
         # 2. Finds the closest good number to the estimation and
         #    uses it to adjust window-width and window-width-steps.
         optimal_steps = good_numbers[np.abs(good_numbers - estim).argmin()]
         self.set('window-width', (optimal_steps *
-                                  self.getfloat('window-width-step-size')))
+                                  self.getfloat('transverse-step')))
         self.set('window-width-steps', optimal_steps)
         # TODO: Add a message for the user.
 
     def adjust_plasma_fineness(self):
         """
         Calculates and adjusts 'plasma-fineness' using
         'plasma-particles-per-cell'.
```

### Comparing `lcode-0.2.1/lcode/config/default_config_values.py` & `lcode-0.3.0/lcode/config/default_config_values.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-"""Default values for a lcodePy config."""
+"""Default values for a lcodePy config"""
 
 default_config_values = {
-    'geometry': 'circ', # circ or 3d now available.
+    'geometry': 'circ', # 'circ' or '3d' 
 
-    # Here we set the type of processing unit: CPU or GPU.
+    # Here we set the type of processing unit: 'cpu' or 'gpu'.
     # For now, GPU can be used only for 3d simulations.
     'processing-unit-type': 'cpu',
 
     # Parameters of simulation window:
 
-    ## Window-width from the main axis to a boundary.
+    ## Transverse size of the window from axis to boundary and 
+    ## transverse grid step (dr in 2d or dx(=dy) in 3d). 
+    ## The window width is adjusted to the closest "good" value
+    ## to ensure fft performance. 
     'window-width': 5.0,
-    'window-width-step-size': 0.05,
+    'transverse-step': 0.05,
 
-    ## Here we set a window length along xi axis.
+    ## Window length along xi-axis and grid step in dxi.
     'window-length': 15.0,
     'xi-step': 0.05,
 
-    ## Set time-limit a bit bigger than the last time moment you want to calculate.
+    ## Time limit for beam evolution and time step.
     'time-limit': 200.5,
     'time-step': 25,
 
     # Parameters of plasma model:
 
-    ## The number of plasma particles per one cell must be the square of a number
-    ## in 3d. This parameter will be adjusted if 3d geometry is chosen by finding
-    ## the closest square number to plasma-particles-per-cell parameter.
+    ## The number of plasma particles per one cell must be the square of 
+    ## an integer in 3d. This parameter will be adjusted in 3d geometry
+    ## to the nearest integer squared (to 9 by default).
     'plasma-particles-per-cell': 10,
-    'ion-model': 'mobile',
-    'ion-mass': 1836,
+    'ion-model': 'mobile', # 'mobile' or 'background'
 
-    ## Numerical noise reduction.
-    'noise-reductor-enabled': False,
-    ### The following parameters are used for 3d noise reduction, 
-    ### for 2d they are ignored. 
-    'filter-window-length': 3,
-    'filter-coefficient': 0.3,
-    'damping-coefficient': 0.1,
-    'dx-max': 1e-3,
+    ## Mass of plasma ions in unita of electron mass
+    'ion-mass': 1836,
     
+    ## Plasma shaping mode: lagacy or function(t, x, y) -> density weights.
+    ## t is the current time, x(y) is the position of the plasma particles.   
+    ## The density of weights must have the same shape as x.  
+    ## x = r, y = 0 in cylindrical geometry.  
+    'plasma-shape': 'legacy', 
     
-    ## Longitudinal profile for plasma density. For 3d only. 
-    'plasma-zshape': '',
+    ## Transverse profile of plasma density settings.
+    ## Example https://lcode.info/site-files/manual.pdf p. 16 
+    'plasma-rshape': 'uniform',
+    'plasma-width': 1,
+    'plasma-width-2': 0,
+    'plasma-density-2': 0.5,
 
+    ## Longitudinal profile of the plasma density. For 3d only. 
+    ## Example https://lcode.info/site-files/manual.pdf p. 17
+    ## Only linear increase/decrease are available. 
+    'plasma-zshape': '''
+        ''',
+
+    ## Declustering of plasma electrons
+    'declustering-enabled': False,
+    ### The following parameters are used for 3d declustering, 
+    ### In 2d they are ignored. 
+    'declustering-averaging': 3,
+    'declustering-force': 0.3,
+    'declustering-damping': 0.1,
+    'declustering-limit': 1e-3,
 
     # Parameters of beam model:
     'beam-substepping-energy': 2,
 
 #This part of the configuration contains experimental and unfinished options. 
 #There is no guarantee that it will work or develop in the future. 
 
     # Partially supported options: 
 
     # Plasma:
-    ## Bz amplitude, supported for 2D only.
+    ## External Bz amplitude, 2D only.
     'magnetic-field': 0,
     
-    ## Plasma transverse profile settings, 2d only.
-    'plasma-profile': 1,
-    'plasma-width': 2,
-    'plasma-width-2': 1,
-    'plasma-density-2': 0.5,
-    
-    ## Longitudinal substepping, 2d only
+    ## Plasma substepping for xi, 2d only
     'substepping-depth': 3,
     'substepping-sensitivity': 0.2,
 
     ## Parameters of the area available for motion of plasma particles, 3d only.
-    'reflect-padding-steps': 10,
+    'bound-padding-steps': 10,
     'plasma-padding-steps': 15,
 
     ## Dual plasma approache for 3d, only GPU  
     'dual-plasma-approach': False,
     'plasma-coarseness': 5,
+    
     # Beam:
-
-    ## It works for 3d with an unusual beam configuration.
+    ## Works for 3d with an unusual beam configuration.
     'rigid-beam': False, 
     ####
-    
-    # Options not currently supported:
 
+# Developer settings
+    
+    ## Only 3d, default value is 1+dxi
+    'field-solver-subtraction-coefficient': 1, 
+    
+    ## Only 2d
     ## Plasma:
-    'plasma-temperature': 0,
     'trapped-path-limit': 0,
-
-    ## Beam:
-    'focusing': 'n',
-    'foc-period': 100,
-    'foc-strength': 0.1,
-    ####
-
-# Developer settings
-    'field-solver-subtraction-coefficient': 1,
-    'field-solver-variant-A': True,
-    'corrector-steps': 2, # Can we even change this???
-
-
-# Useless legacy parameters.
-    'filter-polyorder': 3,
-    'plasma-model': 'P',
-    'continuation': 'n', 
+    'correctotransverse-steps': 2, # Can we even change this???
 }
```

### Comparing `lcode-0.2.1/lcode/config/template.py` & `lcode-0.3.0/lcode/config/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 lcode_template = '''
 # Simulation area:
 geometry = c
-window-width = {window-width};          r-step = {window-width-step-size}
+window-width = {window-width};          transverse-step = {r-step}
 window-length = {window-length};        xi-step = {xi-step}
 time-limit = {time-limit};         time-step = {time-step}
 continuation = n # Plasma continuation (no/beam/longplasma, n/y/Y)
 
 # Particle beams: ????
 beam-current = 0.00281
 rigid-beam = n
```

### Comparing `lcode-0.2.1/lcode/diagnostics/diagnostics_3d.py` & `lcode-0.3.0/lcode/diagnostics/diagnostics_3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,28 +153,28 @@
             f"x_probe_lines={self.__x_probe}, " +
             f"y_probe_lines={self.__y_probe}, " +
             f"unique_directory_name={self.__unique_directory_name})")
 
     def pull_config(self, config: Config):
         """Pulls a config to get all required parameters."""
         steps = config.getint('window-width-steps')
-        grid_step_size = config.getfloat('window-width-step-size')
+        grid_step_size = config.getfloat('transverse-step')
 
         # We change how we store the positions of the 'probe' lines:
         self.__ax_x = (steps // 2 +
                        np.round(self.__x_probe / grid_step_size)).astype(int)
         self.__ax_y = (steps // 2 +
                        np.round(self.__y_probe / grid_step_size)).astype(int)
 
         # Here we check if the output period is less than the time step size.
         # In that case each time step is diagnosed. The first time step is
         # always diagnosed.
         self.__time_step_size = config.getfloat('time-step')
         self.__xi_step_size   = config.getfloat('xi-step')
-        self.__grid_step_size = config.getfloat('window-width-step-size')
+        self.__grid_step_size = config.getfloat('transverse-step')
 
         if self.__output_period < self.__time_step_size:
             self.__output_period = self.__time_step_size
 
         if self.__saving_xi_period < self.__xi_step_size:
             self.__saving_xi_period = self.__xi_step_size
 
@@ -319,15 +319,15 @@
             f"output_merging_r={self.__merging_r}, " +
             f"output_merging_xi={self.__merging_xi}, " +
             f"unique_directory_name={self.__unique_directory_name})")
 
     def pull_config(self, config: Config):
         """Pulls a config to get all required parameters."""
         self.__grid_steps = config.getint('window-width-steps')
-        grid_step_size = config.getfloat('window-width-step-size')
+        grid_step_size = config.getfloat('transverse-step')
 
         self.__grid = ((np.arange(self.__grid_steps) - self.__grid_steps // 2) *
                         grid_step_size)
 
         # Here we define subwindow borders in terms of number of steps:
         self.__r_f = self.__grid_steps // 2 + self.__r_from / grid_step_size
         self.__r_t = self.__grid_steps // 2 + self.__r_to   / grid_step_size
@@ -513,15 +513,15 @@
         # Here we check if the output period is less than the time step size.
         # In that case each time step is diagnosed. The first time step is
         # always diagnosed.
         self.__time_step_size = config.getfloat('time-step')
         self.__xi_step_size   = config.getfloat('xi-step')
 
         grid_steps     = config.getint('window-width-steps')
-        grid_step_size = config.getfloat('window-width-step-size')
+        grid_step_size = config.getfloat('transverse-step')
         self.__grid = (np.arange(grid_steps) - grid_steps // 2) * grid_step_size
 
         if self.__output_period < self.__time_step_size:
             self.__output_period = self.__time_step_size
 
         if self.__saving_xi_period < self.__xi_step_size:
             self.__saving_xi_period = self.__xi_step_size
```

### Comparing `lcode-0.2.1/lcode/diagnostics/diagnostics_list.py` & `lcode-0.3.0/lcode/diagnostics/diagnostics_list.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/diagnostics/targets.py` & `lcode-0.3.0/lcode/diagnostics/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def pull_config(self, config):
         self.dt = config.getfloat('time-step')
         self.tlim = config.getfloat('time-limit')
         if self.t_start is None:
             self.t_start = 0
         if self.t_end is None:
             self.t_end = self.tlim
-        r_step = config.getfloat('window-width-step-size')
+        r_step = config.getfloat('transverse-step')
         xi_step = config.getfloat('xi-step')
         self.w = int(config.getfloat('window-length')/xi_step)+1
         self.h = int(config.getfloat('window-width')/r_step)+1
         
         self.last_idx = self.w - 1
```

### Comparing `lcode-0.2.1/lcode/mpi/beam_io.py` & `lcode-0.3.0/lcode/mpi/beam_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,25 +19,26 @@
     def push(self, beam_slice) -> None:
         if self.final_step or self._rank == self._size - 1:
             self.final_drain.push_beam_slice(beam_slice)
             return
         if self.skip_first:
             self.skip_first = False
             return
+        self.final_drain.push_beam_slice(beam_slice)
         self.send(beam_slice.particles)
     
     def push3d(self, beam_layer):
         if self.final_step or self._rank == self._size - 1:
             self.final_drain.push_beam_layer(beam_layer)
             return
         
         if self.skip_first:
             self.skip_first = False
             return
-
+        self.final_drain.push_beam_layer(beam_layer)
         self.send(beam_layer.particles)
 
     def pull(self, xi_max, xi_min) -> BeamParticles:
         if self.first_step or self._rank == 0:
             return self.initial_source.get_beam_slice(xi_max, xi_min)
         
         beam = self.recv()
@@ -59,14 +60,17 @@
         def push_beam_slice(self, beam_slice):
             self.beam_transport.push(beam_slice)
         def beam_slice(self):
             return self.beam_transport.final_drain.beam_slice()
         
         def push_beam_layer(self, beam_layer):
             self.beam_transport.push3d(beam_layer)
+
+        def save(self, *args, **kwargs):
+            self.beam_transport.final_drain.save(*args, **kwargs)
         
     
     class MPIBeamSource:
         def __init__(self, beam_transport):
             self.beam_transport = beam_transport
         def get_beam_slice(self, xi_max, xi_min) -> BeamParticles:
             return self.beam_transport.pull(xi_max, xi_min)
@@ -100,13 +104,16 @@
             particles = self.final_drain.beam_slice()
             if type(particles) == np.ndarray:
                 self.send(particles)
             else:
                 self.send(particles.particles)
             self.final_drain = self.BeamDrain(self.cfg)
             return
+        
+        self.final_drain = self.BeamDrain(self.cfg)
         self.send(np.array([]))
 
         if self._rank == 0 and not is_last:
             particles = self.recv()
             self.initial_source = self.BeamSource(self.cfg, particles)
+            self.final_drain = self.BeamDrain(self.cfg)
             return
```

### Comparing `lcode-0.2.1/lcode/mpi/transport.py` & `lcode-0.3.0/lcode/mpi/transport.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/mpi/util.py` & `lcode-0.3.0/lcode/mpi/util.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/plasma/data.py` & `lcode-0.3.0/lcode/plasma/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Module for setting classes for Fields, Currents and Partciles data types."""
 import numpy as np
 
-
 # Grouping CPU/GPU arrays, with optional transparent RAM<->GPU copying #
 
 class Arrays:
     """
     A convenient way to group several CPU/GPU arrays and access them with a dot.
     `x = Arrays(xp=cupy, something=numpy_array, something_else=another_array)`
     will create `x` with `x.something` and `x.something_else` being CPU/GPU arrays.
@@ -24,7 +23,12 @@
             setattr(self, name, xp.array(array)) # or asarray?
 
     def copy(self):
         """
         Create an indentical copy of the group of `cupy` arrays.
         """
         return Arrays(**self.__dict__)
+
+    def save(self, *args, **kwargs):
+        data = self.__dict__.copy()
+        data.pop('xp')
+        self.xp.savez_compressed(*args, **kwargs, **data)
```

### Comparing `lcode-0.2.1/lcode/plasma/fields.py` & `lcode-0.3.0/lcode/plasma/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         prev_factor[j] = _prev_factor_multiplier * (1 / np.sqrt(invgamma_sq) - 1) - _prev_factor_threshold
     prev_factor[prev_factor < 0] = 0
     prev_factor += 1
     return prev_factor
 
 
 def get_field_computer(config: Config):
-    grid_step_size = config.getfloat('window-width-step-size')
+    grid_step_size = config.getfloat('transverse-step')
 
     def compute_fields(fields, fields_prev, rho_beam,
                        currents_previous, currents, xi_step_p):
         """
         Compute fields on the next xi step.
 
         Parameters
```

### Comparing `lcode-0.2.1/lcode/plasma/move.py` & `lcode-0.3.0/lcode/plasma/move.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         p_r_array[j] = p_r
         p_f_array[j] = p_f
         p_z_array[j] = p_z
         q_array[j] = q
 
 
 def get_plasma_particles_mover(config: Config):
-    grid_step_size = config.getfloat('window-width-step-size')
+    grid_step_size = config.getfloat('transverse-step')
     max_radius     = config.getfloat('window-width')
     magnetic_field = config.getfloat('magnetic-field')
 
     # Move particles one D_XIP step forward
     def move_particles(fields, particles_prev, noise_amplitude, 
                        xi_step_size, const_arrays):
         new_particles = {}
```

### Comparing `lcode-0.2.1/lcode/plasma/ode.py` & `lcode-0.3.0/lcode/plasma/ode.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/plasma/profiles.py` & `lcode-0.3.0/lcode/plasma/profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         """
         pass
 
 
 class CylindricalProfile(BaseProfile, ABC):
     def __init__(self, config):
         self.max_radius = config.getfloat('window-width')
-        self.r_step = config.getfloat('window-width-step-size')
+        self.r_step = config.getfloat('transverse-step')
 
     def cylindrical_weights(self, particle_positions):
         r_step_p = particle_positions[1] - particle_positions[0]
         return 2 * np.pi * r_step_p * particle_positions
 
 
 class UniformPlacedCylindricalProfile(CylindricalProfile, ABC):
```

### Comparing `lcode-0.2.1/lcode/plasma/rhoj.py` & `lcode-0.3.0/lcode/plasma/rhoj.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     cell_volume[0] *= (13 + 2 * cells_per_particle ** 2) / 32
     cell_volume[1] *= (193 + 2 * cells_per_particle ** 2) / 192
     cell_volume[-1] = np.pi * r_step ** 2 * (n_cells - 45/32)
     return cell_volume
 
 
 def get_rhoj_computer(config: Config):
-    grid_step_size = config.getfloat('window-width-step-size')
+    grid_step_size = config.getfloat('transverse-step')
     max_radius = config.getfloat('window-width')
     n_cells = int(max_radius / grid_step_size) + 1
     particles_per_cell = config.getint('plasma-particles-per-cell')
     cell_volume = _cell_volume(grid_step_size, particles_per_cell, n_cells)
     ion_model = config.get("ion-model")
 
     def compute_rhoj(all_particles: Arrays, const_arrays: Arrays):
```

### Comparing `lcode-0.2.1/lcode/plasma/solver.py` & `lcode-0.3.0/lcode/plasma/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
         self.rho_beam_arr = []
 
         self.xi_step_size = config.getfloat('xi-step')
         self.substepping_sensitivity = config.getfloat('substepping-sensitivity')
         self.substepping_max_depth = config.getint('substepping-depth')
         self.path_lim = config.getfloat('trapped-path-limit')
-        self.noisereductor_enabled = config.getbool('noise-reductor-enabled')
-        self.corrector_steps = config.getint('corrector-steps')
+        self.noisereductor_enabled = config.getbool('declustering-enabled')
+        self.corrector_steps = config.getint('correctotransverse-steps')
 
     # Performs one full step along xi
     def step_dxi(self, particles, fields, currents, const_arrays, 
                  rho_beam, rho_beam_prev):
         substeps = 0
         substepping_depth = 0
         step_begin = True
```

### Comparing `lcode-0.2.1/lcode/plasma3d/data.py` & `lcode-0.3.0/lcode/plasma3d/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Module for setting classes for Fields, Currents and Partciles data types."""
 import numpy as np
 
-
 # Grouping CPU/GPU arrays, with optional transparent RAM<->GPU copying #
 
 class Arrays:
     """
     A convenient way to group several CPU/GPU arrays and access them with a dot.
     `x = Arrays(xp=cupy, something=numpy_array, something_else=another_array)`
     will create `x` with `x.something` and `x.something_else` being CPU/GPU arrays.
@@ -24,7 +23,12 @@
             setattr(self, name, xp.array(array)) # or asarray?
 
     def copy(self):
         """
         Create an indentical copy of the group of `cupy` arrays.
         """
         return Arrays(**self.__dict__)
+    
+    def save(self, *args, **kwargs):
+        data = self.__dict__.copy()
+        data.pop('xp')
+        self.xp.savez_compressed(*args, **kwargs, **data)
```

### Comparing `lcode-0.2.1/lcode/plasma3d/fields.py` & `lcode-0.3.0/lcode/plasma3d/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 
     Bz -= Bz.mean()  # Integral over Bz must be 0.
 
     return Bz
 
 
 def get_field_computer(config: Config):
-    grid_step_size    = config.getfloat('window-width-step-size')
+    grid_step_size    = config.getfloat('transverse-step')
     xi_step_size      = config.getfloat('xi-step')
     subtraction_coeff = config.getfloat('field-solver-subtraction-coefficient')
 
     dst2d, mix2d, dct2d = get_functions(config)
 
     def compute_fields(
         fields, fields_prev, const, rho_beam_full, rho_beam_prev,
```

### Comparing `lcode-0.2.1/lcode/plasma3d/initialization.py` & `lcode-0.3.0/lcode/plasma3d/initialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module for plasma (3d solver) initialization routines."""
 import numpy as np
 
 from ..config.config import Config
 from .weights import get_deposit_plasma
 from .data import Arrays
+from .profile import profile_initial_plasma
 
 ELECTRON_CHARGE = -1
 ELECTRON_MASS = 1
 
 
 # Solving Laplace equation with Dirichlet boundary conditions (Ez) #
 
@@ -99,32 +100,41 @@
         right_half = (.5 + xp.arange(steps // 2 * fineness)) * plasma_step
         left_half = -right_half[::-1]  # invert, reverse
     plasma_grid = xp.concatenate([left_half, right_half])
     assert xp.array_equal(plasma_grid, -plasma_grid[::-1])
     return plasma_grid
 
 
-def make_plasma_single(xp: np, steps, cell_size, fineness=2):
+def make_plasma_single(config, current_time, steps, cell_size, fineness=2):
     """
     Initialize default plasma state, fineness**2 particles per cell.
     """
+    xp = config.xp
     pl_grid = make_plasma_grid(xp, steps, cell_size, fineness)
 
     Np = len(pl_grid)
 
     y_init = xp.broadcast_to(pl_grid, (Np, Np))
-    x_init = y_init.T
+    x_init = y_init.T.copy()
+    q = xp.ones_like(x_init) * ELECTRON_CHARGE / fineness**2 * cell_size**2
+    m = xp.ones_like(x_init) * ELECTRON_MASS / fineness**2 * cell_size**2
+    
+    # Here we change q and m arrays of plasma particles according to
+    # set plasma_zhape:
+    q, m  = profile_initial_plasma(config, current_time, 
+                                   x_init, y_init, q, m)
 
-    x_offt = xp.zeros((Np, Np))
-    y_offt = xp.zeros((Np, Np))
-    px = xp.zeros((Np, Np))
-    py = xp.zeros((Np, Np))
-    pz = xp.zeros((Np, Np))
-    q = xp.ones((Np, Np)) * ELECTRON_CHARGE / fineness**2 * cell_size**2
-    m = xp.ones((Np, Np)) * ELECTRON_MASS / fineness**2 * cell_size**2
+    x_offt = xp.zeros_like(x_init)
+    y_offt = xp.zeros_like(x_init)
+   # mask = q == 0
+   # x_offt[mask] = config.getfloat('window-width') * 100
+   # y_offt[mask] = config.getfloat('window-width') * 100
+    px = xp.zeros_like(x_init)
+    py = xp.zeros_like(x_init)
+    pz = xp.zeros_like(x_init)
 
     return x_init, y_init, x_offt, y_offt, px, py, pz, q, m
 
 
 # Coarse and fine plasma particles initialization #
 
 def make_coarse_plasma_grid(xp: np, steps, step_size, coarseness):
@@ -258,91 +268,50 @@
 
     return (
         coarse_x_init, coarse_y_init, coarse_x_offt, coarse_y_offt,
         coarse_px, coarse_py, coarse_pz, coarse_q, coarse_m, virt_params
     )
 
 
-# TODO: when more zshapes are created, move this fun to a separate file.
-def change_by_plasma_zshape(config: Config, current_time, q, m):
-    # Get required parameters:
-    time_step_size = config.getfloat('time-step')
-    plasma_zshape  = config.get('plasma-zshape')
-    time_middle = current_time - time_step_size / 2 # Just like in lcode2d
-
-    # Check if plasma_zshape is empty and nothing should be done with q and m
-    if plasma_zshape.isspace():
-        return q, m
-
-    # List comprehension to create an array that is easy to handle
-    lines = [line.split() for line in plasma_zshape.splitlines()
-             if len(line) != 0] # without empty lines
-
-    # TODO: Do we need to check ValueError?
-    for line in lines:
-        # Check if time_middle lies in one of the regions:
-        if time_middle < float(line[0]):
-            if line[2] == 'L': # Only linear rise/decrease is implemented now
-                coef = (float(line[1]) * (float(line[0]) - time_middle) +
-                        float(line[3]) * time_middle) / float(line[0])
-                if coef >= 0:
-                    return q * coef, m * coef
-                else:
-                    print('A density that is < 0 is not available, ' +
-                          'a density of 1 is assumed.')
-                    break
-            else:
-                print(line[2], 'segment shape is not available, a density ' +
-                      'of 1 is assumed.')
-                break
-        else:
-            time_middle -= float(line[0])
 
-    # If the total length is too small, hence we finished the loop above,
-    # or we broke from the loop, a density of 1 is assumed:
-    return q, m
 
 
 def init_plasma(config: Config, current_time=0):
     """
     Initialize all the arrays needed (for what?).
     """
-    pu_type = config.get('processing-unit-type').lower()
-    if pu_type == 'cpu':
-        xp = np
-    elif pu_type == 'gpu':
-        import cupy as xp
+    xp = config.xp
 
     grid_steps            = config.getint('window-width-steps')
-    grid_step_size        = config.getfloat('window-width-step-size')
-    reflect_padding_steps = config.getint('reflect-padding-steps')
+    grid_step_size        = config.getfloat('transverse-step')
+    bound_padding_steps   = config.getint('bound-padding-steps')
     plasma_padding_steps  = config.getint('plasma-padding-steps')
     plasma_fineness       = config.getfloat('plasma-fineness')
     dual_plasma_approach  = config.getbool('dual-plasma-approach')
     subtraction_coeff = config.getfloat('field-solver-subtraction-coefficient')
     xi_step_size = config.getfloat('xi-step')
     ion_model = config.get("ion-model")
 
     if plasma_fineness > 1:
         plasma_fineness = int(plasma_fineness)
 
     # for convenient diagnostics, a cell should be in the center of the grid
     assert grid_steps % 2 == 1
 
     # particles should not reach the window pre-boundary cells
-    if reflect_padding_steps <= 2:
-        raise Exception("'reflect_padding_steps' parameter is too low.\n" +
-                        "Details: 'reflect_padding_steps' must be bigger than" +
-                        " 2. By default it is 5.")
+    if bound_padding_steps <= 2:
+        raise Exception("'bound_padding_steps' parameter is too low.\n" +
+                        "Details: 'bound_padding_steps' must be bigger than" +
+                        " 2. By default it is 10.")
 
     if dual_plasma_approach and pu_type == 'gpu':
         plasma_coarseness = config.getint('plasma-coarseness')
 
         # virtual particles should not reach the window pre-boundary cells
-        assert reflect_padding_steps > plasma_coarseness + 1
+        assert bound_padding_steps > plasma_coarseness + 1
         # TODO: The (costly) alternative is to reflect after plasma virtualization,
         #       but it's better for stabitily, or is it?
 
         x_init, y_init, x_offt, y_offt, px, py, pz, q, m, virt_params = \
             make_plasma_dual(
                 xp, steps=grid_steps - 2*plasma_padding_steps,
                 cell_size=grid_step_size, coarseness=plasma_coarseness,
@@ -352,28 +321,26 @@
         Exception("We cannot use this type of processing unit." +
                   "Please choose GPU if you want to use dual plasma approach.")
     else:
         plasma_coarseness, virt_params = None, Arrays(xp)
 
         x_init, y_init, x_offt, y_offt, px, py, pz, q, m = \
             make_plasma_single(
-                xp, steps=grid_steps - plasma_padding_steps * 2,
+                config, current_time, 
+                steps=grid_steps - plasma_padding_steps * 2,
                 cell_size=grid_step_size, fineness=plasma_fineness)
 
-    # Here we change q and m arrays of plasma particles according to
-    # set plasma_zhape:
-    q, m = change_by_plasma_zshape(config, current_time, q, m)
 
     # We create arrays dx_chaotic, dy_chaotic, dx_chaotic_perp, dy_chaotic_perp
     # that are used in noise filter, with right sizes:
     size = x_offt.shape[0]
-    dx_chaotic = xp.zeros((size, size), dtype=xp.float64)
-    dy_chaotic = xp.zeros((size, size), dtype=xp.float64)
-    dx_chaotic_perp = xp.zeros((size, size), dtype=xp.float64)
-    dy_chaotic_perp = xp.zeros((size, size), dtype=xp.float64)
+    dx_chaotic = xp.zeros_like(x_init)
+    dy_chaotic = xp.zeros_like(x_init)
+    dx_chaotic_perp = xp.zeros_like(x_init)
+    dy_chaotic_perp = xp.zeros_like(x_init)
 
     particles = {'electrons' : Arrays(xp, x_init=x_init, y_init=y_init,
                                       x_offt=x_offt, y_offt=y_offt, 
                                       px=px, py=py, pz=pz,
                                       q=q, m=m,
                                       dx_chaotic=dx_chaotic,
                                       dy_chaotic=dy_chaotic,
@@ -446,37 +413,48 @@
 
     return fields, particles, currents, const_arrays, xi_plasma_layer
 
 
 def load_plasma(config: Config, path_to_plasmastate: str):
     fields, particles, currents, const_arrays, xi_plasma_layer =\
         init_plasma(config)
-
-    with fields.xp.load(file=path_to_plasmastate) as state:
-        fields = Arrays(fields.xp,
-                        Ex=state['Ex'], Ey=state['Ey'], Ez=state['Ez'],
-                        Bx=state['Bx'], By=state['By'], Bz=state['Bz'],
-                        Phi=state['Phi'])
-
-        particles = Arrays(fields.xp,
-                           x_init=state['x_init'], y_init=state['y_init'],
-                           q=state['q'], m=state['m'],
-                           x_offt=state['x_offt'], y_offt=state['y_offt'],
-                           px=state['px'], py=state['py'], pz=state['pz'], 
-        
-                           dx_chaotic=state['dx_chaotic'],
-                           dy_chaotic=state['dy_chaotic'],
-                           dx_chaotic_perp=state['dx_chaotic_perp'],
-                           dy_chaotic_perp=state['dy_chaotic_perp'])
-
-        currents = Arrays(fields.xp,
-                          ro=state['ro'], jx=state['jx'],
-                          jy=state['jy'], jz=state['jz'])
+    xp = fields.xp
+    # Load by numpy in RAM after that convert to cupy array if necessary.
+    # It is done because the particle type for cupy.load is too complex.
+    with np.load(file=path_to_plasmastate) as state:
+        fields = Arrays(xp=xp,
+                        Ex=xp.array(state['Ex']), Ey=xp.array(state['Ey']), 
+                        Ez=xp.array(state['Ez']),
+                        Bx=xp.array(state['Bx']), By=xp.array(state['By']), 
+                        Bz=xp.array(state['Bz']),
+                        Phi=xp.array(state['Phi']))
+        for sort in const_arrays.sorts:
+            particles[sort] = Arrays(
+                xp=xp,
+                x_init=xp.array(state[sort]['x_init']), 
+                y_init=xp.array(state[sort]['y_init']),
+                q=xp.array(state[sort]['q']), m=xp.array(state[sort]['m']),
+                x_offt=xp.array(state[sort]['x_offt']), 
+                y_offt=xp.array(state[sort]['y_offt']),
+                px=xp.array(state[sort]['px']), py=xp.array(state[sort]['py']), 
+                pz=xp.array(state[sort]['pz']), 
+            
+                dx_chaotic=xp.array(state[sort]['dx_chaotic']),
+                dy_chaotic=xp.array(state[sort]['dy_chaotic']),
+                dx_chaotic_perp=xp.array(state[sort]['dx_chaotic_perp']),
+                dy_chaotic_perp=xp.array(state[sort]['dy_chaotic_perp'])
+            )
+
+        currents = Arrays(xp=xp,
+                          ro=xp.array(state['ro']), jx=xp.array(state['jx']),
+                          jy=xp.array(state['jy']), jz=xp.array(state['jz']))
 
         try:
-            const_arrays.ro_initial = state['ro_initial']
+            const_arrays.ro_initial = xp.array(state['rho_initial'])
+        except:
+            pass
+        try: 
+            xi_plasma_layer = float(state['xi_plasma_layer'])
         except:
             pass
-        
-        xi_plasma_layer = float(state['xi_plasma_layer'][0])
 
     return fields, particles, currents, const_arrays, xi_plasma_layer
```

### Comparing `lcode-0.2.1/lcode/plasma3d/move.py` & `lcode-0.3.0/lcode/plasma3d/move.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,46 +5,91 @@
 from math import sqrt, floor
 
 from ..config.config import Config
 from .weights import weight4, weight4_cupy
 from .data import Arrays
 
 # Field interpolation and particle movement (fused), for CPU #
+        #    move_smart_kernel(
+        #        xi_step_size, boundary, grid_step_size, grid_steps,
+        #        
+        #        fields.Ex, fields.Ey, fields.Ez,
+        #        fields.Bx, fields.By, fields.Bz,
+
+        #        particles_prev[sort].x_init, particles_prev[sort].y_init,
+
+        #        particles_prev[sort].x_offt, particles_prev[sort].y_offt,
+        #        particles_prev[sort].px, particles_prev[sort].py, 
+        #        particles_prev[sort].pz,
+
+        #        
+        #        particles_full[sort].m, particles_full[sort].q, 
+        #        particles_full[sort].x_offt, particles_full[sort].y_offt,
+
+@nb.njit(inline='always')
+def _correct_boundary_particles(x_init, y_init, x_offt, y_offt, 
+                                px, py, pz, boundary): 
+    x = x_init + x_offt
+    y = y_init + y_offt
+    if x > +boundary:
+        x = +2 * boundary - x
+        x_offt = x - x_init
+        px = py = pz = 0
+    if x < -boundary:
+        x = -2 * boundary - x
+        x_offt = x - x_init
+        px = py = pz = 0
+    if y > +boundary:
+        y = +2 * boundary - y
+        y_offt = y - y_init
+        px = py = pz = 0
+    if y < -boundary:
+        y = -2 * boundary - y
+        y_offt = y - y_init
+        px = py = pz = 0
+    return x, y, x_offt, y_offt, px, py, pz
 
-@nb.njit(parallel=True)
+
+@nb.njit(parallel=True, cache=True)
 def move_smart_kernel_numba(
-    xi_step_size, reflect_boundary, grid_step_size, grid_steps,
-    ms, qs, x_init, y_init,
-    x_offt_prev, y_offt_prev, px_prev, py_prev, pz_prev,
+    xi_step_size, boundary, grid_step_size, grid_steps,
     Ex_avg, Ey_avg, Ez_avg, Bx_avg, By_avg, Bz_avg,
+    x_init, y_init, 
+    x_offt_prev, y_offt_prev, px_prev, py_prev, pz_prev,
+    ms, qs,
     x_offt_full, y_offt_full, px_full, py_full, pz_full,
     size):
     """
     Update plasma particle coordinates and momenta according to the field
     values interpolated halfway between the previous plasma particle location
     and the the best estimation of its next location currently available to us.
-    Also reflect the particles from `+-reflect_boundary`.
+    Also absorb the particles at `+-boundary`.
     """
     ms, qs = ms.ravel(), qs.ravel()
     x_init, y_init = x_init.ravel(), y_init.ravel()
     x_offt_prev, y_offt_prev = x_offt_prev.ravel(), y_offt_prev.ravel()
     x_offt_full, y_offt_full = x_offt_full.ravel(), y_offt_full.ravel()
     px_prev, py_prev, pz_prev = px_prev.ravel(), py_prev.ravel(), pz_prev.ravel()
     px_full, py_full, pz_full = px_full.ravel(), py_full.ravel(), pz_full.ravel()
 
     for k in nb.prange(size):
+        if qs[k] == 0:
+            continue
         m, q = ms[k], qs[k]
 
         opx, opy, opz = px_prev[k], py_prev[k], pz_prev[k]
         px, py, pz = opx, opy, opz
         x_offt, y_offt = x_offt_prev[k], y_offt_prev[k]
-
         # Calculate midstep positions and fields in them.
-        x_halfstep = x_init[k] + (x_offt_prev[k] + x_offt_full[k]) / 2
-        y_halfstep = y_init[k] + (y_offt_prev[k] + y_offt_full[k]) / 2
+        x_offt_aver = (x_offt_prev[k] + x_offt_full[k]) / 2
+        y_offt_aver = (y_offt_prev[k] + y_offt_full[k]) / 2
+        x_halfstep, y_halfstep, _, _, px, py, pz = \
+            _correct_boundary_particles(x_init[k], y_init[k], 
+                                        x_offt_aver, y_offt_aver, 
+                                        px, py, pz, boundary)
 
         x_h = x_halfstep / grid_step_size + .5
         y_h = y_halfstep / grid_step_size + .5
         x_loc = x_h - floor(x_h) - .5
         y_loc = y_h - floor(y_h) - .5
         ix = int(floor(x_h) + grid_steps // 2)
         iy = int(floor(y_h) + grid_steps // 2)
@@ -75,96 +120,97 @@
         vx, vy, vz = px / gamma_m, py / gamma_m, pz / gamma_m
         factor_1 = q * xi_step_size / (1 - pz / gamma_m)
         dpx = factor_1 * (Ex + vy * Bz - vz * By)
         dpy = factor_1 * (Ey - vx * Bz + vz * Bx)
         dpz = factor_1 * (Ez + vx * By - vy * Bx)
         px, py, pz = opx + dpx / 2, opy + dpy / 2, opz + dpz / 2
 
-        # Apply the coordinate and momenta increments
+        # Apply the coordinate and momenta increments.
         gamma_m = sqrt(m**2 + pz**2 + px**2 + py**2)
 
         x_offt += px / (gamma_m - pz) * xi_step_size  # no mixing with x_init
         y_offt += py / (gamma_m - pz) * xi_step_size  # no mixing with y_init
 
         px, py, pz = opx + dpx, opy + dpy, opz + dpz
+        
+        _, _, x_offt, y_offt, px, py, pz = \
+            _correct_boundary_particles(x_init[k], y_init[k], x_offt, y_offt, 
+                                        px, py, pz, boundary)
 
-        # Reflect the particles from `+-reflect_boundary`.
-        # TODO: avoid branching?
+        # Protection from non-physical particles.
         x = x_init[k] + x_offt
         y = y_init[k] + y_offt
-        if x > +reflect_boundary:
-            x = +2 * reflect_boundary - x
-            x_offt = x - x_init[k]
-            px = -px
-        if x < -reflect_boundary:
-            x = -2 * reflect_boundary - x
-            x_offt = x - x_init[k]
-            px = -px
-        if y > +reflect_boundary:
-            y = +2 * reflect_boundary - y
-            y_offt = y - y_init[k]
-            py = -py
-        if y < -reflect_boundary:
-            y = -2 * reflect_boundary - y
-            y_offt = y - y_init[k]
-            py = -py
+        if x >= +boundary or x <= -boundary or y >= +boundary or y <= -boundary:
+            x_offt = y_offt = px = py = pz = 0
+            qs[k] = 0
 
         # Save the results into the output arrays  # TODO: get rid of that
         x_offt_full[k], y_offt_full[k] = x_offt, y_offt
         px_full[k], py_full[k], pz_full[k] = px, py, pz
 
 
-def move_estimate_wo_fields_numba(xi_step, reflect_boundary, m, x_init, y_init,
-                                  x_offt, y_offt, px, py, pz, size):
+@nb.njit(parallel=True)
+def move_estimate_wo_fields_numba(xi_step, m, x_offt, y_offt, px, py, pz, size):
     """
     Move coarse plasma particles as if there were no fields.
-    Also reflect the particles from `+-reflect_boundary`.
     """
-    gamma_m = np.sqrt(m**2 + pz**2 + px**2 + py**2)
-
-    x_offt += px / (gamma_m - pz) * xi_step
-    y_offt += py / (gamma_m - pz) * xi_step
-
-    # TODO: Do we want to perform this checking for all particles? Doesn't we
-    #       lose accuracy then?
-    reflect = reflect_boundary
-    x, y = x_init + x_offt, y_init + y_offt
-
-    x[x >= +reflect] = +2 * reflect - x[x >= +reflect]
-    x[x <= -reflect] = -2 * reflect - x[x <= -reflect]
-    y[y >= +reflect] = +2 * reflect - y[y >= +reflect]
-    y[y <= -reflect] = -2 * reflect - y[y <= -reflect]
-    # TODO: Do we want to update momentum or is it not that important?
-
-    x_offt, y_offt = x - x_init, y - y_init
-
+    m = m.ravel()
+    px, py, pz = px.ravel(), py.ravel(), pz.ravel()
+    x_offt, y_offt = x_offt.ravel(), y_offt.ravel()
+    for k in nb.prange(size):
+        if m[k] == 0:
+            continue
+        gamma_m = np.sqrt(m[k]**2 + pz[k]**2 + px[k]**2 + py[k]**2)
 
-# Field interpolation and particle movement (fused), for GPU #
+        x_offt[k] += px[k] / (gamma_m - pz[k]) * xi_step
+        y_offt[k] += py[k] / (gamma_m - pz[k]) * xi_step
 
+    
 # TODO: Not very smart to get a kernel this way.
 def get_move_smart_kernel_cupy():
     import cupy as cp
 
     return cp.ElementwiseKernel(
         in_params="""
-        float64 xi_step_size, float64 reflect_boundary,
+        float64 xi_step_size, float64 boundary,
         float64 grid_step_size, float64 grid_steps,
-        raw T m, raw T q, raw T x_init, raw T y_init,
+        raw T Ex_avg, raw T Ey_avg, raw T Ez_avg,
+        raw T Bx_avg, raw T By_avg, raw T Bz_avg,
+        raw T x_init, raw T y_init,
         raw T x_offt_prev, raw T y_offt_prev,
         raw T px_prev, raw T py_prev, raw T pz_prev,
-        raw T Ex_avg, raw T Ey_avg, raw T Ez_avg,
-        raw T Bx_avg, raw T By_avg, raw T Bz_avg
+        raw T m
         """,
         out_params="""
-        raw T x_offt_full, raw T y_offt_full,
+        raw T q, raw T x_offt_full, raw T y_offt_full,
         raw T px_full, raw T py_full, raw T pz_full
         """,
         operation="""
-        const T x_halfstep = x_init[i] + (x_offt_prev[i] + x_offt_full[i]) / 2;
-        const T y_halfstep = y_init[i] + (y_offt_prev[i] + y_offt_full[i]) / 2;
+        if (q[i] == 0){
+            continue;
+        }
+        T px = px_prev[i], py = py_prev[i], pz = pz_prev[i];
+        T x_halfstep = x_init[i] + (x_offt_prev[i] + x_offt_full[i]) / 2;
+        T y_halfstep = y_init[i] + (y_offt_prev[i] + y_offt_full[i]) / 2;
+        if (x_halfstep > boundary) {
+            x_halfstep =  2 * boundary  - x_halfstep;
+            px = py = pz = 0;
+        }
+        if (x_halfstep < -boundary) {
+            x_halfstep = -2 * boundary - x_halfstep;
+            px = py = pz = 0;
+        }
+        if (y_halfstep > boundary) {
+            y_halfstep = 2 * boundary  - y_halfstep;
+            px = py = pz = 0;
+        }
+        if (y_halfstep < -boundary) {
+            y_halfstep = -2 * boundary - y_halfstep;
+            px = py = pz = 0;
+        }
         
         const T x_h = x_halfstep / (T) grid_step_size + 0.5;
         const T y_h = y_halfstep / (T) grid_step_size + 0.5;
         const T x_loc = x_h - floor(x_h) - 0.5;
         const T y_loc = y_h - floor(y_h) - 0.5;
         const int ix = floor(x_h) + floor(grid_steps / 2);
         const int iy = floor(y_h) + floor(grid_steps / 2);
@@ -178,15 +224,14 @@
 
                 Ex += Ex_avg[idx] * w; Bx += Bx_avg[idx] * w;
                 Ey += Ey_avg[idx] * w; By += By_avg[idx] * w;
                 Ez += Ez_avg[idx] * w; Bz += Bz_avg[idx] * w;
             }
         }
 
-        T px = px_prev[i], py = py_prev[i], pz = pz_prev[i];
         const T opx = px_prev[i], opy = py_prev[i], opz = pz_prev[i];
         T x_offt = x_offt_prev[i], y_offt = y_offt_prev[i];
 
         T gamma_m = sqrt(m[i]*m[i] + px*px + py*py + pz*pz);
         T vx = px / gamma_m, vy = py / gamma_m, vz = pz / gamma_m;
         T factor = q[i] * (T) xi_step_size / (1 - pz / gamma_m);
         T dpx = factor * (Ex + vy * Bz - vz * By);
@@ -204,33 +249,40 @@
 
         gamma_m = sqrt(m[i]*m[i] + px*px + py*py + pz*pz);
         x_offt += px / (gamma_m - pz) * xi_step_size;
         y_offt += py / (gamma_m - pz) * xi_step_size;
         px = opx + dpx; py = opy + dpy; pz = opz + dpz;
 
         T x = x_init[i] + x_offt, y = y_init[i] + y_offt;
-        if (x > reflect_boundary) {
-            x =  2 * reflect_boundary  - x;
+        if (x > boundary) {
+            x =  2 * boundary  - x;
             x_offt = x - x_init[i];
-            px = -px;
+            px = py = pz = 0;
         }
-        if (x < -reflect_boundary) {
-            x = -2 * reflect_boundary - x;
+        if (x < -boundary) {
+            x = -2 * boundary - x;
             x_offt = x - x_init[i];
-            px = -px;
+            px = py = pz = 0;
         }
-        if (y > reflect_boundary) {
-            y = 2 * reflect_boundary  - y;
+        if (y > boundary) {
+            y = 2 * boundary  - y;
             y_offt = y - y_init[i];
-            py = -py;
+            px = py = pz = 0;
         }
-        if (y < -reflect_boundary) {
-            y = -2 * reflect_boundary - y;
+        if (y < -boundary) {
+            y = -2 * boundary - y;
             y_offt = y - y_init[i];
-            py = -py;
+            px = py = pz = 0;
+        }
+        
+        if (x >= +boundary || x <= -boundary 
+            || y >= +boundary || y <= -boundary) {
+            x_offt = y_offt = 0;
+            px = py = pz = 0;
+            q[i] = 0; 
         }
 
         x_offt_full[i] = x_offt; y_offt_full[i] = y_offt;
         px_full[i] = px; py_full[i] = py; pz_full[i] = pz;
 
         """,
         name='move_smart_cupy', preamble=weight4_cupy, no_return=True
@@ -238,110 +290,92 @@
 
 
 def get_move_wo_fields_kernel_cupy():
     import cupy as cp
 
     return cp.ElementwiseKernel(
         in_params="""
-        float64 xi_step_size, float64 reflect_boundary,
-        raw T m, raw T x_init, raw T y_init
+        float64 xi_step_size, raw T m
         """,
         out_params="""
         raw T x_offt, raw T y_offt, raw T px, raw T py, raw T pz
         """,
         operation="""
+        if (m[i] == 0){
+            continue;
+        }
         const T gamma_m = sqrt(
             m[i]*m[i] + px[i]*px[i] + py[i]*py[i] + pz[i]*pz[i]);
 
         x_offt[i] += px[i] / (gamma_m - pz[i]) * xi_step_size;
         y_offt[i] += py[i] / (gamma_m - pz[i]) * xi_step_size;
-
-        T x = x_init[i] + x_offt[i], y = y_init[i] + y_offt[i];
-        if (x > reflect_boundary) {
-            x =  2 * reflect_boundary  - x;
-            px[i] = -px[i];
-        }
-        if (x < -reflect_boundary) {
-            x = -2 * reflect_boundary - x;
-            px[i] = -px[i];
-        }
-        if (y > reflect_boundary) {
-            y = 2 * reflect_boundary  - y;
-            py[i] = -py[i];
-        }
-        if (y < -reflect_boundary) {
-            y = -2 * reflect_boundary - y;
-            py[i] = -py[i];
-        }
-
-        x_offt[i] = x - x_init[i]; y_offt[i] = y - y_init[i];
         """,
         name='move_wo_fields_cupy', no_return=True
     )
 
 
 def get_plasma_particles_mover(config: Config):
     xi_step_size     = config.getfloat('xi-step')
-    grid_step_size   = config.getfloat('window-width-step-size')
+    grid_step_size   = config.getfloat('transverse-step')
     grid_steps       = config.getint('window-width-steps')
-    reflect_padding_steps = config.getint('reflect-padding-steps')
-    reflect_boundary = grid_step_size * (grid_steps / 2 - reflect_padding_steps)
+    bound_padding_steps = config.getint('bound-padding-steps')
+    boundary = grid_step_size * (grid_steps / 2 - bound_padding_steps)
 
     pu_type = config.get('processing-unit-type').lower()
     if pu_type == 'cpu':
         move_wo_fields_kernel = move_estimate_wo_fields_numba
         move_smart_kernel = move_smart_kernel_numba
     elif pu_type == 'gpu':
         move_wo_fields_kernel = get_move_wo_fields_kernel_cupy()
         move_smart_kernel = get_move_smart_kernel_cupy()
 
     def move_particles_wo_fields(particles: dict, const_arrays: Arrays):
         """
         Move coarse plasma particles as if there were no fields.
-        Also reflect the particles from `+-reflect_boundary`.
         """
         # NOTE: We need to copy particles to discriminate
         #       particles_full and particles_prev.
         particles_full = {}
         for sort in const_arrays.sorts:
             particles_full[sort] = particles[sort].copy()
 
         for sort in const_arrays.sorts:
             move_wo_fields_kernel(
-                xi_step_size, reflect_boundary, particles_full[sort].m,
-                particles_full[sort].x_init, particles_full[sort].y_init,
+                xi_step_size, particles_full[sort].m,
                 particles_full[sort].x_offt, particles_full[sort].y_offt,
                 particles_full[sort].px, particles_full[sort].py, 
-                particles_full[sort].pz, size=particles_full[sort].m.size)
+                particles_full[sort].pz, 
+                size = particles_full[sort].m.size)
 
         return particles_full
 
     def move_particles_smart(
         fields: Arrays, particles_prev: dict, particles_full: dict,
         const_arrays: Arrays):
         """
         Update plasma particle coordinates and momenta according to the
         field values interpolated halfway between the previous plasma
         particle location and the the best estimation of its next location
         currently available to us.
         """
         for sort in const_arrays.sorts:
             move_smart_kernel(
-                xi_step_size, reflect_boundary, grid_step_size, grid_steps,
+                xi_step_size, boundary, grid_step_size, grid_steps,
+                
+                fields.Ex, fields.Ey, fields.Ez,
+                fields.Bx, fields.By, fields.Bz,
 
-                particles_prev[sort].m, particles_prev[sort].q,
                 particles_prev[sort].x_init, particles_prev[sort].y_init,
 
                 particles_prev[sort].x_offt, particles_prev[sort].y_offt,
                 particles_prev[sort].px, particles_prev[sort].py, 
                 particles_prev[sort].pz,
 
-                fields.Ex, fields.Ey, fields.Ez,
-                fields.Bx, fields.By, fields.Bz,
-
+                
+                particles_full[sort].m, particles_full[sort].q, 
                 particles_full[sort].x_offt, particles_full[sort].y_offt,
                 particles_full[sort].px, particles_full[sort].py, 
                 particles_full[sort].pz,
 
                 size=particles_prev[sort].m.size)
 
         return particles_full
```

### Comparing `lcode-0.2.1/lcode/plasma3d/noise_filter.py` & `lcode-0.3.0/lcode/plasma3d/noise_filter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,109 @@
 """The module for experimental noise filters that we are trying to use to successfully pass the so-called test 1."""
 import numpy as np
+import numba as nb
 from ..config.config import Config
 from .data import Arrays
 
 
+def get_inhomogeneity_calculator_cupy(config):
+    cp = config.xp
+    calculate_inhomoginity_kernel = cp.RawKernel(r'''
+        extern "C" __global__
+        void calculate_inhomoginity_kernel(const float* d_offt, float* d_inhom
+                                           int size){
+            int i = blockDim.x * blockIdx.x + threadIdx.x;
+            int j = blockDim.y * blockIdx.y + threadIdx.y;
+
+            if (j !=0 && j != size-1){
+                d_offt_01 = d_offt[i, j+1];
+                d_offt_00 = d_offt[i, j];
+                d_offt_02 = d_offt[i, j+2];
+                if (d_offt_00 && d_offt_01 && d_offt_02){
+                    d_inhom[i, j+1] = d_offt_01 - (d_offt_00 + d_offt_02) / 2;
+                }
+            }
+        }
+        ''', 
+        'calculate_inhomoginity_kernel'
+    )
+
+    def calculate_inhomoginity_cupy(d_offt, axis):
+        if axis: d_offt = d_offt.T
+        d_inhom = cp.zeros_like(d_offt)
+        size = d_inhom.shape[0]
+        calculate_inhomoginity_kernel(d_offt, d_inhom, size)
+        mask = (d_offt[:, 0] != 0) * (d_offt[:, 1] != 0) * (d_offt[:, 2] != 0)
+        d_inhom[mask, 0] = d_offt[mask, 0] - 2*d_offt[mask, 1] + d_offt[mask, 2]
+        
+        mask = (d_offt[:, -1] != 0) * (d_offt[:, -2] != 0) * (d_offt[:, -3] != 0)
+        d_inhom[mask, -1] = d_offt[mask, -1] - 2*d_offt[mask, -2] + d_offt[mask, -3]
+            
+
+        if axis: d_inhom = d_inhom.T
+        return d_inhom
+
+    return calculate_inhomoginity_cupy
+
+
+@nb.njit(parallel=True)
+def calculate_inhomogeneity_numba(d_offt, axis):
+    if axis: d_offt = d_offt.T
+    d_inhom = np.zeros_like(d_offt)
+    size = d_inhom.shape[0]
+    for i in nb.prange(size):
+        for j in range(size-2):
+            d_offt_01 = d_offt[i, j+1]
+            if not d_offt_01:
+                continue
+            d_offt_00 = d_offt[i, j]
+            d_offt_02 = d_offt[i, j+2]
+            if d_offt_00 and d_offt_02:
+                d_inhom[i, j+1] = d_offt_01 - (d_offt_00 + d_offt_02) / 2
+                continue
+            d_offt_03 = d_offt[i, j+3]
+            if d_offt_03:
+                d_inhom[i, j+1] = d_offt_01 - 2*d_offt_02 + d_offt_03
+                continue
+            d_offt_00_1 = d_offt[i, j-1]
+            if d_offt_00_1:
+                d_inhom[i, j+1] = d_offt_01 - 2*d_offt_00 + d_offt_00_1
+                continue
+    
+    mask = (d_offt[:, 0] != 0) * (d_offt[:, 1] != 0) * (d_offt[:, 2] != 0)
+    d_inhom[mask, 0] = d_offt[mask, 0] - 2*d_offt[mask, 1] + d_offt[mask, 2]
+    
+    mask = (d_offt[:, -1] != 0) * (d_offt[:, -2] != 0) * (d_offt[:, -3] != 0)
+    d_inhom[mask, -1] = d_offt[mask, -1] - 2*d_offt[mask, -2] + d_offt[mask, -3]
+        
+
+    if axis: d_inhom = d_inhom.T
+    return d_inhom
+
+
 # This function generates a noise filtering function which
 # we then use in the predictor-corrector loop (solver.py).
 def get_noise_filter(config: Config):
     # Here it is much more convenient to take the config parameters only once,
     # and not just give them to the noise_filter along with the particles arrays.
     xi_step_size = config.getfloat('xi-step')
 
-    filter_window_length = config.getint('filter-window-length')
-    filter_polyorder = config.getint('filter-polyorder')
-    filter_coefficient = config.getfloat('filter-coefficient')
-    damping_coefficient = config.getfloat('damping-coefficient')
-    dx_max = config.getfloat('dx-max')
+    filter_window_length = config.getint('declustering-averaging')
+    filter_coefficient = config.getfloat('declustering-force')
+    damping_coefficient = config.getfloat('damping-declustering')
+    dx_max = config.getfloat('declustering-limit')
 
     pu_type = config.get('processing-unit-type').lower()
     if pu_type == 'cpu':
-        # from scipy.signal import savgol_filter
         from scipy.ndimage import fourier_gaussian
+        calculate_inhomogeneity = calculate_inhomogeneity_numba
     elif pu_type == 'gpu':
         from cupyx.scipy.ndimage import fourier_gaussian
-        # from .savgol_filter_cp import savgol_filter
+        calculate_inhomogeneity = get_inhomogeneity_calculator_cupy(config)
 
-    def calculate_inhomogeneity(d_offt, xp: np, axis):
-        if axis: d_offt = d_offt.T
-        d_inhom = xp.vstack((
-            d_offt[0, :] - 2 * d_offt[1, :] + d_offt[2, :],
-            d_offt[1:-1, :] - (d_offt[2:, :] + d_offt[:-2, :]) / 2,
-            d_offt[-1, :] - 2 * d_offt[-2, :] + d_offt[-3, :]))
-        if axis: d_inhom = d_inhom.T
-        return d_inhom
 
     # A new noise mitigation method.
     def noise_filter(particles: Arrays, particles_prev: Arrays):
         # Zero step. We determine if we will use numpy or cupy as xp:
         xp = particles.xp
 
         # First, we take out all the required arrays:
@@ -52,16 +119,16 @@
 #         # Longitudinal displacement inhomogeneity:
 #         dx_inhom = x_offt[1:-1, :] - (x_offt[2:, :] + x_offt[:-2, :]) / 2
 #         dy_inhom = y_offt[:, 1:-1] - (y_offt[:, 2:] + y_offt[:, :-2]) / 2
 #         # and transverse (perpendicular):
 #         dx_inhom_perp = y_offt[1:-1, :] - (y_offt[2:, :] + y_offt[:-2, :]) / 2
 #         dy_inhom_perp = x_offt[:, 1:-1] - (x_offt[:, 2:] + x_offt[:, :-2]) / 2
         
-        dx_inhom = (calculate_inhomogeneity(x_offt, xp, 0) + calculate_inhomogeneity(x_offt, xp, 1)) / 2
-        dy_inhom = (calculate_inhomogeneity(y_offt, xp, 1) + calculate_inhomogeneity(y_offt, xp, 0)) / 2
+        dx_inhom = (calculate_inhomogeneity(x_offt, 0) + calculate_inhomogeneity(x_offt, 1)) / 2
+        dy_inhom = (calculate_inhomogeneity(y_offt, 1) + calculate_inhomogeneity(y_offt, 0)) / 2
         # Зануление смещений на границе, пока только ухудшало все
         # dx_inhom[0,:] *= 0
         # dx_inhom[-1,:] *= 0
         # dx_inhom[:,0] *= 0
         # dx_inhom[:,-1] *= 0
         # dy_inhom[0,:] *= 0
         # dy_inhom[-1,:] *= 0
```

### Comparing `lcode-0.2.1/lcode/plasma3d/rhoj.py` & `lcode-0.3.0/lcode/plasma3d/rhoj.py`

 * *Files identical despite different names*

### Comparing `lcode-0.2.1/lcode/plasma3d/solver.py` & `lcode-0.3.0/lcode/plasma3d/solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self, config: Config):
         self.compute_rhoj = get_rhoj_computer(config)
         self.compute_fields = get_field_computer(config)
         self.move_particles_wo_fields, self.move_particles = \
             get_plasma_particles_mover(config)
 
         self.noise_filter = get_noise_filter(config)
-        self.noise_filter_enabled = config.getbool('noise-reductor-enabled')
+        self.declustering_enabled = config.getbool('declustering-enabled')
 
     # Perfoms one full step along xi.
     # To understand the numerical scheme, read values as following:
     # *_prev = * on the previous xi step, an index number = k
     # *_half = * on the halfstep, an index number = k + 1/2
     # *_full = * on the next xi step (fullstep), an index number = k + 1
     # *_prevprev = * on the xi step with an index number k - 1
@@ -61,15 +61,15 @@
             currents_prev, currents_full
         )
 
         particles_full = self.move_particles(
             fields_half, particles_prev, particles_full, const_arrays
         )
 
-        if self.noise_filter_enabled:
+        if self.declustering_enabled:
             # Here we perform noise filtering after the end of the movement:
             particles_full["electrons"] = \
                             self.noise_filter(particles_full["electrons"], 
                                               particles_prev["electrons"])
 
         currents_full = self.compute_rhoj(
             particles_full, const_arrays
```

### Comparing `lcode-0.2.1/lcode/plasma3d/weights.py` & `lcode-0.3.0/lcode/plasma3d/weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
                          out_ro, out_jx, out_jy, out_jz, size):
     """
     Deposit plasma particles onto the charge density and current grids.
     """
     x_h, y_h, m, q = x_h.ravel(), y_h.ravel(), m.ravel(), q.ravel()
     px, py, pz = px.ravel(), py.ravel(), pz.ravel()
     for k in range(size):
+        if q[k] == 0:
+            continue
         # Deposit the resulting fine particle on ro/j grids.
         gamma_m = sqrt(m[k]**2 + px[k]**2 + py[k]**2 + pz[k]**2)
         dro = q[k] / (1 - pz[k] / gamma_m)
         djx = px[k] * (dro / gamma_m)
         djy = py[k] * (dro / gamma_m)
         djz = pz[k] * (dro / gamma_m)
 
@@ -152,14 +154,17 @@
     return cp.ElementwiseKernel(
         in_params="""
         float64 grid_steps, float64 grid_step_size, raw T x_h, raw T y_h,
         raw T px, raw T py, raw T pz, raw T q, raw T m
         """,
         out_params='raw T out_ro, raw T out_jx, raw T out_jy, raw T out_jz',
         operation="""
+        if (q[i] == 0){
+            continue;
+        }
         const T gamma_m = sqrt(
             m[i]*m[i] + px[i]*px[i] + py[i]*py[i] + pz[i]*pz[i]);
         const T dro = q[i] / (1 - pz[i] / gamma_m);
         const T djx = px[i] * (dro / gamma_m);
         const T djy = py[i] * (dro / gamma_m);
         const T djz = pz[i] * (dro / gamma_m);
 
@@ -186,15 +191,15 @@
 
 
 def get_deposit_plasma(config: Config):
     """
     Check if a user set dual-plasma-approach to True or False and return
     the deposition function for the set approach.
     """
-    grid_step_size = config.getfloat('window-width-step-size')
+    grid_step_size = config.getfloat('transverse-step')
     grid_steps = config.getint('window-width-steps')
     plasma_fineness = config.getint('plasma-fineness')
     dual_plasma_approach = config.getbool('dual-plasma-approach')
 
     pu_type = config.get('processing-unit-type').lower()
     if pu_type == 'cpu':
         deposit_plasma_kernel = deposit_plasma_numba
```

### Comparing `lcode-0.2.1/lcode/push_solvers/push_solver.py` & `lcode-0.3.0/lcode/push_solvers/push_solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import pickle
 
 from ..config.config import Config
 
 #import for 2D simulation
 from ..beam import BeamParticles2D, BeamCalculator2D
 from ..plasma.solver import CylindricalPlasmaSolver
 
@@ -29,15 +30,15 @@
         self.config = config
         
         #remeber some config value
         self.dxi = config.getfloat('xi-step')
         self.grid_steps = config.getint('window-width-steps') 
         if not self.grid_steps:
             max_radius = config.getfloat('window-width')
-            r_step = config.getfloat('window-width-step-size')
+            r_step = config.getfloat('transverse-step')
             self.grid_steps = int(max_radius / r_step) + 1
         window_length = config.getfloat('window-length')
         self.xi_steps = int(window_length / self.dxi)
         
         #Final plasma state for tests
         self._plasmastate = None
     
@@ -48,15 +49,15 @@
         pass
     def _get_beam_layer(self, beam_source, xi_i):
         pass
     def _simple_diag(self, current_time, xi_i, pl_fields):
         pass
 
     def step_dt(self, pl_fields, pl_particles,
-                pl_currents, pl_const_arrays,
+                pl_currents, pl_const_arrays, xi_plasma_layer_start, 
                 beam_source, beam_drain,
                 current_time, diagnostics_list=[]):
         """
         Perform one time step of beam-plasma calculations.
         
         NOTE: The data structure is different for 2D and 3D so far. 
             The parameter type is written as `2D-data (3D-data)`.
@@ -89,16 +90,16 @@
         beam_layer_to_move = self._set_beam_particles(xp)
         fell_size = 0
 
         # TODO: Not sure this is right if we start from a saved plasma state and
         #       with a saved beamfile.
         #       Do we need array here?
         rho_beam_prev = self._set_rho_beam_array(xp, self.grid_steps)
-
-        for xi_i in np.arange(self.xi_steps + 1):
+        xi_i_plasma_layer_start = round(-xi_plasma_layer_start / self.dxi) + 1
+        for xi_i in range(xi_i_plasma_layer_start, self.xi_steps + 1, 1):
             # Get beam particles with xi in [dxi*{xi_i + 1}, dxi*{xi_i})
             # This use to finish rho_beam[xi_i]
             beam_layer_to_layout = self._get_beam_layer(beam_source, xi_i)
 
             rho_beam = self.beam_calc.layout_beam_layer(beam_layer_to_layout,
                                                         xi_i)
 
@@ -120,26 +121,33 @@
             rho_beam_prev = rho_beam.copy()
 
             # Add pircticles with xi in [dxi*{xi_i + 1}, dxi*{xi_i}) 
             # for move it in next xi step
             beam_layer_to_move = \
                 beam_layer_to_layout.append(fell_to_next_layer)
             fell_size = fell_to_next_layer.id.size
-
             # Send moved beam particles to next time step 
             beam_drain.push_beam_slice(moved)
             # beam_drain.finish_layer(xi_i * -self.dxi)
             
+            xi_plasma_layer = - xi_i * self.dxi
             # Every xi step diagnostics
             for diagnostic in diagnostics_list:
-                diagnostic.process(
-                    self.config, current_time, xi_i, 
-                    pl_particles, pl_fields, rho_beam, moved)
+                # diagnostic.process(
+                #     self.config, current_time, xi_i, 
+                #     pl_particles, pl_fields, rho_beam, moved)
+                diagnostic.after_step_dxi(
+                    current_time, xi_plasma_layer, pl_particles,
+                    pl_fields, pl_currents, rho_beam)
             if xi_i % 10 == 0:
                 self._simple_diag(current_time, xi_i, pl_fields)
+
+        for diagnostic in diagnostics_list:
+            diagnostic.dump(current_time, xi_plasma_layer, pl_particles,
+                            pl_fields, pl_currents, beam_drain)
         self._plasmastate = (pl_particles, pl_fields, pl_currents)
 
 
 class PusherAndSolver2D(PusherAndSolver):
     """
     Class for calculation xi-cycle in 2D axisymmetric geometry. 
     """
```

### Comparing `lcode-0.2.1/lcode/simulation.py` & `lcode-0.3.0/lcode/simulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class Simulation:
     """
     Top-level lcodePy simulation class that controls computational.
 
     This class contains configuration of simulation and controls diagnostics.
     """
     def __init__(self, config=default_config_values, beam_parameters={},
-                 diagnostics=[]):
+                 diagnostics=[], runas_filename="runas.py"):
         """
             Initializes a simulation.
 
             Parametrs
             ---------
             config : Dict, optional
                     The set of base parameters to perform the simulation.
@@ -51,22 +51,25 @@
                     Collection of diagnostics that should be run.
                     By default, diagnostics are desibled.      
         """
 
         self.config = copy.copy(config)
         self.beam_parameters = copy.copy(beam_parameters)
         self.diagnostics_list = copy.copy(diagnostics)
+        self.runas_filename = runas_filename
 
         # We use this time as a general time value:
         self.current_time = 0.
         # The user can change this value for diagnostic convenience.
 
         # We initialize a beam source and a beam drain:
         self.beam_source = None
         self.beam_drain = None
+        # To save particles from a load for MPIBeamTransport
+        self.__beam_particles = None
 
         # We set that initially the code doesn't use an external plasma state:
         self.external_plasmastate = False
         self.path_to_plasmastate = 'plasmastate.npz'
 
         #set geometry is None before reading config
         self.__geometry = None
@@ -90,15 +93,15 @@
         if self.__geometry is None:
             self.__geometry = self.__config.get('geometry').lower()
         elif self.__geometry != self.__config.get('geometry').lower():
             raise Exception("Sorry, update geometry does not support now.")
             
         if self.__geometry == '3d':
             self.particle_dtype = particle_dtype3d
-            self.__config._correct_3d_settings()
+            self.__config._adjust_config_values_3d()
             self.__push_solver = PusherAndSolver3D(config=self.__config)
             self.init_plasma, self.__load_plasma = \
                 init_plasma_3d, load_plasma_3d
             if self.__rigid_beam:
                 self.BeamParticles, self.BeamSource, self.BeamDrain = \
                     None, RigidBeamSource3D, RigidBeamDrain3D
             else:
@@ -129,20 +132,23 @@
 
 
     # TODO: Should we make load_beamfile just
     #       another method of beam genetration?
     def load_beamfile(self, path_to_beamfile='beamfile.npz'):
         if self.__rigid_beam:
             raise Exception("We cannot load a beam in the case of a rigid beam.")
-
-        beam_particles = self.BeamParticles(self.__config.xp)
+        if self.__geometry == '3d':
+            beam_particles = self.BeamParticles(self.__config.xp)
+        else:
+            beam_particles = self.BeamParticles()
         beam_particles.load(path_to_beamfile)
+        self.__beam_particles = beam_particles
 
-        self.beam_source = self.BeamSource(self.__config, beam_particles)
-        self.beam_drain  = self.BeamDrain(self.__config)
+       # self.beam_source = self.BeamSource(self.__config, beam_particles)
+       # self.beam_drain  = self.BeamDrain(self.__config)
 
     # def add_beamfile(self, path_to_beamfile='new_beamfile.npz'):
     #     """Add a new beam that is loaded from 'path_to_beamfile' to the beam source.
     #     """
     #     pass
 
     def __load_plasmastate(self):
@@ -174,14 +180,16 @@
         N_steps : int, optional
                 Number of time steps that will be done. 
                 Default : N_steps = time_limit / time_step.
         """
         # 0. It analyzes config values:
         #TODO: explicit config update. If we change xi-step we must change beam.
         self.__pull_config()
+        if self.runas_filename:
+            self.__config.dump(self.runas_filename)
 
         # 1. If we use an external plasma state, we load it:
         if self.external_plasmastate:
             self.__load_plasmastate()
 
         # t step function, makes N_steps time steps.
         if self.__rigid_beam:
@@ -196,76 +204,66 @@
         else:
             self.__time_limit = \
                 N_steps * self.__time_step_size + self.current_time
             print("Since the number of time steps has been set explicitly,",
                   f"the code will simulate till time limit = {self.__time_limit},",
                   f"with a time step size = {self.__time_step_size}.")
 
-        # 2. Checks for plasma continuation mode:
-        if self.__cont_mode == 'n' or self.__cont_mode == 'no':
-            # 3. If a beam source is empty (None), we generate
-            #    a new beam according to set parameters:
-
-            # Check for a beam being rigid:
-            if self.__rigid_beam:
-                # For now, beam_parameters is just a function representing
-                # the charge distribution of a rigid beam. In the future,
-                # we want to use the same beam_parameters as for a non-rigid
-                # beam in both cases.
-                beam_particles = self.beam_parameters
-
-                self.beam_source = self.BeamSource(self.__config,
-                                                   beam_particles)
-                self.beam_drain  = self.BeamDrain(self.__config)
-
-                self.MPITransport = MPIBeamTransport(self.__config, N_steps,
-                                                     beam_particles, self.particle_dtype,
-                                                     self.BeamSource, self.BeamDrain)
-
-            if self.beam_source is None:
-                # Generate all parameters for a beam:
+        # Check for a beam being rigid:
+        if self.__rigid_beam:
+            # For now, beam_parameters is just a function representing
+            # the charge distribution of a rigid beam. In the future,
+            # we want to use the same beam_parameters as for a non-rigid
+            # beam in both cases.
+            beam_particles = self.beam_parameters
+
+            self.beam_source = self.BeamSource(self.__config,
+                                               beam_particles)
+            self.beam_drain  = self.BeamDrain(self.__config)
+
+            self.MPITransport = MPIBeamTransport(self.__config, N_steps,
+                                                 beam_particles, self.particle_dtype,
+                                                 self.BeamSource, self.BeamDrain)
+
+        if self.beam_source is None:
+            # Generate all parameters for a beam:
+            if self.__beam_particles is None:
                 beam_particles = generate_beam(self.__config,
                                                self.beam_parameters)
+            else: 
+                beam_particles = self.__beam_particles
 
-                # Here we create a beam source and a beam drain:
-                self.beam_source = self.BeamSource(self.__config,
-                                                   beam_particles)
-                self.beam_drain  = self.BeamDrain(self.__config)
-
-                self.MPITransport = MPIBeamTransport(self.__config, N_steps,
-                                                beam_particles, self.particle_dtype,
-                                                self.BeamSource, self.BeamDrain)
-            
-            self.current_time = self.__time_step_size * (self.MPITransport._rank + 1)
-
-            # 4. A loop that calculates N time steps:
-            for t_i in range(self.MPITransport.steps_per_node):
-
-                self.beam_source, self.beam_drain = self.MPITransport.get_transports()
-
-
-                plasmastate = self.__init_plasmastate(self.current_time)
-
-                # Calculates one time step:
-                self.__push_solver.step_dt(
-                    *plasmastate, self.beam_source, self.beam_drain,
-                    self.current_time, self.diagnostics_list
-                )
-
-                # Here we transfer beam particles from beam_buffer to
-                # beam_source for the next time step. And create a new beam
-                # drain that is empty.
-                self.MPITransport.next_step()
-
-                self.current_time = self.current_time + self.__time_step_size * self.MPITransport._size
-            # 4. As in lcode2d, we save the beam state on reaching the time limit:
-            # self.beam_source.beam.save('beamfile') # Do we need it?
-            # TODO: Make checkpoints where all simulation information,
-            #       including beam and current time, is saved.
-            print('The work is done!')
-
-        # Other plasma continuation mode has not been implemented yet.
-        # If you are writing these modes, just change where you put
-        # init_plasma(...) and generate_beam(...)
-        else:
-            raise Exception("Sorry, for now, only 'no' mode of plasma" +
-                            "continuation is supported.")
+            # Here we create a beam source and a beam drain:
+            self.beam_source = self.BeamSource(self.__config,
+                                               beam_particles)
+            self.beam_drain  = self.BeamDrain(self.__config)
+
+            self.MPITransport = MPIBeamTransport(self.__config, N_steps,
+                                            beam_particles, self.particle_dtype,
+                                            self.BeamSource, self.BeamDrain)
+        
+        self.current_time = self.__time_step_size * (self.MPITransport._rank + 1)
+
+        # 4. A loop that calculates N time steps:
+        for t_i in range(self.MPITransport.steps_per_node):
+            self.beam_source, self.beam_drain = self.MPITransport.get_transports()
+
+
+            plasmastate = self.__init_plasmastate(self.current_time)
+
+            # Calculates one time step:
+            self.__push_solver.step_dt(
+                *plasmastate, self.beam_source, self.beam_drain,
+                self.current_time, self.diagnostics_list
+            )
+
+            # Here we transfer beam particles from beam_buffer to
+            # beam_source for the next time step. And create a new beam
+            # drain that is empty.
+            self.MPITransport.next_step()
+
+            self.current_time = self.current_time + self.__time_step_size * self.MPITransport._size
+        # 4. As in lcode2d, we save the beam state on reaching the time limit:
+        # self.beam_source.beam.save('beamfile') # Do we need it?
+        # TODO: Make checkpoints where all simulation information,
+        #       including beam and current time, is saved.
+        print('The work is done!')
```

### Comparing `lcode-0.2.1/lcode.egg-info/PKG-INFO` & `lcode-0.3.0/lcode.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcode
-Version: 0.2.1
+Version: 0.3.0
 Summary: LCODE is a free software for simulationplasma wakefield acceleration based on QSA.
 Home-page: https://lcode.info
 Download-URL: https://github.com/lcodePy-team/lcodePy
 Author: lcodePy-team
 Author-email: team@lcode.info
 License: BSD-3-Clause-extended
 Keywords: plasma wakefield acceleration,quasistatic approximation,numerical simulation
@@ -27,19 +27,19 @@
 ## Overview 
 
 LCODE is a free software for numerical simulation of
 particle beam-driven plasma wakefield acceleration.
 LCODE is based on the quasistatic approximation, capable
 of simulation in 2D and 3D geometry, and can use GPUs and CPUs.
 
-For now, this is new and experimental software. This is
+For now, this under active development. This is
 a complete overhaul of the old C version in Python.
 
-You can also find a more mature 2D version of LCODE at
-http://lcode.info/.
+- **Website:** https://lcode.info
+- **Documentation:** https://lcode.info/docs
 
 ## Instalation 
 
 We use [Anaconda](https://www.continuum.io/why-anaconda) and we recommend 
 installing lcode in a separate environment. 
 Any other python installation should work fine, but has not been tested. 
 
@@ -73,9 +73,12 @@
 ```
 pip install .
 ```
 
 
 ----------
 
+You can also find a more mature 2D version of LCODE at
+http://lcode.info/.
+
 Fill free to contact `team@lcode.info` for assistance with it.
```

### Comparing `lcode-0.2.1/lcode.egg-info/SOURCES.txt` & `lcode-0.3.0/lcode.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -37,37 +37,44 @@
 lcode/config/default_config.py
 lcode/config/default_config_values.py
 lcode/config/template.py
 lcode/diagnostics/__init__.py
 lcode/diagnostics/diagnostics_3d.py
 lcode/diagnostics/diagnostics_class.py
 lcode/diagnostics/diagnostics_list.py
+lcode/diagnostics/particles.py
 lcode/diagnostics/process.py
+lcode/diagnostics/slice.py
 lcode/diagnostics/targets.py
-lcode/examples/__init__.py
-lcode/examples/ssm.py
+lcode/diagnostics/utils.py
+lcode/diagnostics/FXi/FXi.py
+lcode/diagnostics/FXi/Strategy.py
+lcode/diagnostics/FXi/Strategy3D.py
+lcode/diagnostics/FXi/StrategyCircular.py
+lcode/diagnostics/FXi/__init__.py
+lcode/examples/high-R.py
+lcode/examples/original-ssm.py
 lcode/mpi/__init__.py
 lcode/mpi/beam_io.py
 lcode/mpi/transport.py
 lcode/mpi/util.py
 lcode/plasma/__init__.py
 lcode/plasma/data.py
 lcode/plasma/fields.py
 lcode/plasma/initialization.py
 lcode/plasma/move.py
 lcode/plasma/ode.py
 lcode/plasma/profiles.py
 lcode/plasma/rhoj.py
 lcode/plasma/solver.py
 lcode/plasma3d/__init__.py
-lcode/plasma3d/arraytools.py
 lcode/plasma3d/data.py
 lcode/plasma3d/fields.py
 lcode/plasma3d/initialization.py
 lcode/plasma3d/move.py
 lcode/plasma3d/noise_filter.py
+lcode/plasma3d/profile.py
 lcode/plasma3d/rhoj.py
-lcode/plasma3d/savgol_filter_cp.py
 lcode/plasma3d/solver.py
 lcode/plasma3d/weights.py
 lcode/push_solvers/__init__.py
 lcode/push_solvers/push_solver.py
```

### Comparing `lcode-0.2.1/setup.py` & `lcode-0.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from setuptools import setup, find_packages
+from distutils.command.install import INSTALL_SCHEMES
 from lcode import __version__
     
 with open('README.md', 'r') as f:
     long_description = f.read()
 
+for scheme in INSTALL_SCHEMES.values():
+    scheme['data'] = scheme['purelib']
 
 with open('requirements.txt', 'r') as f:
     requirements = f.read().split('\n')
 
 if __name__ == '__main__':
     setup(
         name='lcode',
@@ -18,14 +21,15 @@
                 'plasma wakefield acceleration based on QSA.',
         long_description=long_description,
         long_description_content_type='text/markdown',
         url='https://lcode.info',
         download_url='https://github.com/lcodePy-team/lcodePy',
         packages=find_packages(),
         install_requires=requirements,
+        package_data={'lcode': ['examples/*.py']},
         include_package_data=True,
         classifiers=[
           'Programming Language :: Python',
           'Development Status :: 4 - Beta',
           'Intended Audience :: Science/Research',
           'Topic :: Scientific/Engineering :: Physics',
           'Environment :: Console',
```

