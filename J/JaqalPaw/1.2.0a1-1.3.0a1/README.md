# Comparing `tmp/JaqalPaw-1.2.0a1.tar.gz` & `tmp/jaqalpaw-1.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/build-jaqal/jaqalpaw/dist/.tmp-4zgtcu7n/JaqalPaw-1.2.0a1.tar", last modified: Fri May 19 23:36:05 2023, max compression
+gzip compressed data, was "jaqalpaw-1.3.0a1.tar", last modified: Tue May 14 11:02:16 2024, max compression
```

## Comparing `JaqalPaw-1.2.0a1.tar` & `jaqalpaw-1.3.0a1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       81 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      197 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1366 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      486 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/
--rw-rw-r--   0 root         (0) root         (0)       49 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex14.jaqal
--rw-rw-r--   0 root         (0) root         (0)     1341 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex14.py
--rw-rw-r--   0 root         (0) root         (0)     3072 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex14.wvf
--rw-rw-r--   0 root         (0) root         (0)       55 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex3.jaqal
--rw-rw-r--   0 root         (0) root         (0)      508 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex3.py
--rw-rw-r--   0 root         (0) root         (0)     2816 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex3.wvf
--rw-rw-r--   0 root         (0) root         (0)      109 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex4.jaqal
--rw-rw-r--   0 root         (0) root         (0)      602 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex4.py
--rw-rw-r--   0 root         (0) root         (0)     9440 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex4.wvf
--rw-rw-r--   0 root         (0) root         (0)       87 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_a.jaqal
--rw-rw-r--   0 root         (0) root         (0)     1335 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_a.py
--rw-rw-r--   0 root         (0) root         (0)     7552 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_a.wvf
--rw-rw-r--   0 root         (0) root         (0)       94 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_b.jaqal
--rw-rw-r--   0 root         (0) root         (0)     1296 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_b.py
--rw-rw-r--   0 root         (0) root         (0)     8832 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_b.wvf
--rw-rw-r--   0 root         (0) root         (0)       83 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iv.jaqal
--rw-rw-r--   0 root         (0) root         (0)      554 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iv.py
--rw-rw-r--   0 root         (0) root         (0)     2816 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iv.wvf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/examples/MSGateFrameRotations/
--rw-rw-r--   0 root         (0) root         (0)      270 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.jaqal
--rw-rw-r--   0 root         (0) root         (0)     5703 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.py
--rw-rw-r--   0 root         (0) root         (0)     9792 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.wvf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/examples/ModulatedMS/
--rw-rw-r--   0 root         (0) root         (0)      331 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.jaqal
--rw-rw-r--   0 root         (0) root         (0)    10232 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.py
--rw-rw-r--   0 root         (0) root         (0)     9824 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.wvf
--rw-rw-r--   0 root         (0) root         (0)      518 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS_Config.txt
--rw-rw-r--   0 root         (0) root         (0)      111 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/test_sk1.jaqal
--rw-rw-r--   0 root         (0) root         (0)     8000 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/test_sk1.wvf
--rw-rw-r--   0 root         (0) root         (0)      111 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/test_std.jaqal
--rw-rw-r--   0 root         (0) root         (0)     7680 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/test_std.wvf
--rw-rw-r--   0 root         (0) root         (0)      111 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     2863 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1366 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2876 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/
--rw-rw-r--   0 root         (0) root         (0)       24 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2346 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/_cli.py
--rw-rw-r--   0 root         (0) root         (0)      410 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2005 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/binary_conversion.py
--rw-rw-r--   0 root         (0) root         (0)     7209 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/encoding_parameters.py
--rw-rw-r--   0 root         (0) root         (0)     6839 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/lut_programming.py
--rw-rw-r--   0 root         (0) root         (0)    18094 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/pulse_binarization.py
--rw-rw-r--   0 root         (0) root         (0)     4475 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/spline_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/compiler/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/compiler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    33383 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/compiler/jaqal_compiler.py
--rw-rw-r--   0 root         (0) root         (0)     2888 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/compiler/time_ordering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9387 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/arbiters.py
--rw-rw-r--   0 root         (0) root         (0)     9795 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/byte_decoding.py
--rw-rw-r--   0 root         (0) root         (0)    19023 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/firmware_emulator.py
--rw-rw-r--   0 root         (0) root         (0)      554 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/pdq_spline.py
--rw-rw-r--   0 root         (0) root         (0)     1928 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/uram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3462 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/ast_utilities.py
--rw-rw-r--   0 root         (0) root         (0)     4730 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/circuit_constructor.py
--rw-rw-r--   0 root         (0) root         (0)     7647 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/circuit_constructor_visitor.py
--rw-rw-r--   0 root         (0) root         (0)     6914 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/gate_slice.py
--rw-rw-r--   0 root         (0) root         (0)     1175 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/padding.py
--rw-rw-r--   0 root         (0) root         (0)     8614 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/pulse_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1274 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/datatypes.py
--rw-rw-r--   0 root         (0) root         (0)      144 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     1541 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/helper_functions.py
--rw-rw-r--   0 root         (0) root         (0)      103 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/qscout/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/qscout/v1/
--rw-rw-r--   0 root         (0) root         (0)    18055 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/qscout/v1/QSCOUTBuiltins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/qscout/v1/sk1/
--rw-rw-r--   0 root         (0) root         (0)      440 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/qscout/v1/sk1/jaqal_pulses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/qscout/v1/std/
--rw-rw-r--   0 root         (0) root         (0)      404 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/qscout/v1/std/jaqal_pulses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/tests/
--rw-rw-r--   0 root         (0) root         (0)      119 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/backcompat.jaqal
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/tests/benchmark/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/benchmark/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1887 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/benchmark/benchmark.py
--rw-rw-r--   0 root         (0) root         (0)    12982 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/run_benchmarks.py
--rw-rw-r--   0 root         (0) root         (0)     1651 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/test_backcompat.py
--rw-rw-r--   0 root         (0) root         (0)      956 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/test_repro.py
--rw-rw-r--   0 root         (0) root         (0)     1159 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/test_smoke.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.497547 jaqalpaw-1.3.0a1/
+-rw-r--r--   0 root         (0) root         (0)    11358 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1528 2024-05-14 11:02:16.497547 jaqalpaw-1.3.0a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      486 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.485547 jaqalpaw-1.3.0a1/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.489547 jaqalpaw-1.3.0a1/examples/DocumentationSamples/
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex14.jaqal
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex14.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex14.wvf
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex3.jaqal
+-rw-r--r--   0 root         (0) root         (0)      508 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex3.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex3.wvf
+-rw-r--r--   0 root         (0) root         (0)      109 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex4.jaqal
+-rw-r--r--   0 root         (0) root         (0)      602 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex4.py
+-rw-r--r--   0 root         (0) root         (0)     9440 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex4.wvf
+-rw-r--r--   0 root         (0) root         (0)       87 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iii_a.jaqal
+-rw-r--r--   0 root         (0) root         (0)     1335 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iii_a.py
+-rw-r--r--   0 root         (0) root         (0)     7552 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iii_a.wvf
+-rw-r--r--   0 root         (0) root         (0)       94 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iii_b.jaqal
+-rw-r--r--   0 root         (0) root         (0)     1296 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iii_b.py
+-rw-r--r--   0 root         (0) root         (0)     8832 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iii_b.wvf
+-rw-r--r--   0 root         (0) root         (0)       83 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iv.jaqal
+-rw-r--r--   0 root         (0) root         (0)      554 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iv.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iv.wvf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.489547 jaqalpaw-1.3.0a1/examples/MSGateFrameRotations/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.jaqal
+-rw-r--r--   0 root         (0) root         (0)     5703 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.py
+-rw-r--r--   0 root         (0) root         (0)     9792 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.wvf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.489547 jaqalpaw-1.3.0a1/examples/ModulatedMS/
+-rw-r--r--   0 root         (0) root         (0)      331 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.jaqal
+-rw-r--r--   0 root         (0) root         (0)    10232 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.py
+-rw-r--r--   0 root         (0) root         (0)     9824 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.wvf
+-rw-r--r--   0 root         (0) root         (0)      518 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/ModulatedMS/Exemplar_ModulatedMS_Config.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/test_sk1.jaqal
+-rw-r--r--   0 root         (0) root         (0)     8000 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/test_sk1.wvf
+-rw-r--r--   0 root         (0) root         (0)      111 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/test_std.jaqal
+-rw-r--r--   0 root         (0) root         (0)     7680 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/examples/test_std.wvf
+-rw-r--r--   0 root         (0) root         (0)      111 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2863 2024-05-14 11:02:16.497547 jaqalpaw-1.3.0a1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.481547 jaqalpaw-1.3.0a1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.497547 jaqalpaw-1.3.0a1/src/JaqalPaw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1528 2024-05-14 11:02:16.000000 jaqalpaw-1.3.0a1/src/JaqalPaw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2876 2024-05-14 11:02:16.000000 jaqalpaw-1.3.0a1/src/JaqalPaw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 11:02:16.000000 jaqalpaw-1.3.0a1/src/JaqalPaw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-14 11:02:16.000000 jaqalpaw-1.3.0a1/src/JaqalPaw.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-14 11:02:16.000000 jaqalpaw-1.3.0a1/src/JaqalPaw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-14 11:02:16.000000 jaqalpaw-1.3.0a1/src/JaqalPaw.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.489547 jaqalpaw-1.3.0a1/src/jaqalpaw/
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/_cli.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.489547 jaqalpaw-1.3.0a1/src/jaqalpaw/bytecode/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/bytecode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/bytecode/binary_conversion.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/bytecode/encoding_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/bytecode/lut_programming.py
+-rw-r--r--   0 root         (0) root         (0)    18094 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/bytecode/pulse_binarization.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/bytecode/spline_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.493547 jaqalpaw-1.3.0a1/src/jaqalpaw/compiler/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/compiler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33383 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/compiler/jaqal_compiler.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/compiler/time_ordering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.493547 jaqalpaw-1.3.0a1/src/jaqalpaw/emulator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/emulator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9387 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/emulator/arbiters.py
+-rw-r--r--   0 root         (0) root         (0)     9795 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/emulator/byte_decoding.py
+-rw-r--r--   0 root         (0) root         (0)    19023 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/emulator/firmware_emulator.py
+-rw-r--r--   0 root         (0) root         (0)      554 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/emulator/pdq_spline.py
+-rw-r--r--   0 root         (0) root         (0)     1928 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/emulator/uram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.493547 jaqalpaw-1.3.0a1/src/jaqalpaw/ir/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/ir/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/ir/ast_utilities.py
+-rw-r--r--   0 root         (0) root         (0)     4730 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/ir/circuit_constructor.py
+-rw-r--r--   0 root         (0) root         (0)     7647 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/ir/circuit_constructor_visitor.py
+-rw-r--r--   0 root         (0) root         (0)     6914 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/ir/gate_slice.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/ir/padding.py
+-rw-r--r--   0 root         (0) root         (0)     8614 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/ir/pulse_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.493547 jaqalpaw-1.3.0a1/src/jaqalpaw/utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/utilities/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/utilities/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/utilities/helper_functions.py
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/jaqalpaw/utilities/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.481547 jaqalpaw-1.3.0a1/src/qscout/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.493547 jaqalpaw-1.3.0a1/src/qscout/v1/
+-rw-r--r--   0 root         (0) root         (0)    18055 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/qscout/v1/QSCOUTBuiltins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.493547 jaqalpaw-1.3.0a1/src/qscout/v1/sk1/
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/qscout/v1/sk1/jaqal_pulses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.493547 jaqalpaw-1.3.0a1/src/qscout/v1/std/
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/src/qscout/v1/std/jaqal_pulses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.497547 jaqalpaw-1.3.0a1/tests/
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/tests/backcompat.jaqal
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:16.497547 jaqalpaw-1.3.0a1/tests/benchmark/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/tests/benchmark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/tests/benchmark/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)    12982 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/tests/run_benchmarks.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/tests/test_backcompat.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/tests/test_repro.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2024-05-14 11:01:42.000000 jaqalpaw-1.3.0a1/tests/test_smoke.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `JaqalPaw-1.2.0a1/LICENSE` & `jaqalpaw-1.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/PKG-INFO` & `jaqalpaw-1.3.0a1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaqalPaw
-Version: 1.2.0a1
+Version: 1.3.0a1
 Summary: Just Another Quantum Assembly Language Pulses and Waveform Specification
 Home-page: https://qscout.sandia.gov
 Author: Daniel Lobser, Benjamin C. A. Morrison, Kenneth Rudinger, Antonio Russo, Jay Wesley Van Der Wall
 Author-email: qscout@sandia.gov
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,18 +12,23 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: emulator
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: jaqalpaq>=1.3.0a1
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Provides-Extra: emulator
+Requires-Dist: matplotlib; extra == "emulator"
 
 For information on JaqalPaw usage and parameter descriptions, see the official
 [JaqalPaw manual](https://www.sandia.gov/app/uploads/sites/174/2021/11/JaqalPaw__A_Guide_to_Defining_Pulses_and_Waveforms_for_Jaqal.pdf),
 which can be found at [qscout.sandia.gov](https://qscout.sandia.gov).
 
 # Running The Emulator
```

### Comparing `JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex14.py` & `jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex14.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex14.wvf` & `jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex14.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex3.wvf` & `jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex3.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex4.py` & `jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex4.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex4.wvf` & `jaqalpaw-1.3.0a1/examples/DocumentationSamples/ex4.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_a.py` & `jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iii_a.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_a.wvf` & `jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iii_a.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_b.py` & `jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iii_b.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_b.wvf` & `jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iii_b.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iv.py` & `jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iv.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iv.wvf` & `jaqalpaw-1.3.0a1/examples/DocumentationSamples/examples_iv.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.py` & `jaqalpaw-1.3.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.wvf` & `jaqalpaw-1.3.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.py` & `jaqalpaw-1.3.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.wvf` & `jaqalpaw-1.3.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS_Config.txt` & `jaqalpaw-1.3.0a1/examples/ModulatedMS/Exemplar_ModulatedMS_Config.txt`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/test_sk1.wvf` & `jaqalpaw-1.3.0a1/examples/test_sk1.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/examples/test_std.wvf` & `jaqalpaw-1.3.0a1/examples/test_std.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/setup.cfg` & `jaqalpaw-1.3.0a1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = JaqalPaw
 author = Daniel Lobser, Benjamin C. A. Morrison, Kenneth Rudinger, Antonio Russo, Jay Wesley Van Der Wall
 author_email = qscout@sandia.gov
 description = Just Another Quantum Assembly Language Pulses and Waveform Specification
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache
-version = 1.2.0a1
+version = 1.3.0a1
 home_page = https://qscout.sandia.gov
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Physics
@@ -18,15 +18,15 @@
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Unix
 
 [options]
 packages = find_namespace:
 package_dir = 
 	=src
-install_requires = numpy; scipy; jaqalpaq>=1.2.0a1
+install_requires = numpy; scipy; jaqalpaq>=1.3.0a1
 python_requires = >=3.6.5
 platforms = any
 
 [options.packages.find]
 include = 
 	jaqalpaw
 	jaqalpaw.*
```

### Comparing `JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/PKG-INFO` & `jaqalpaw-1.3.0a1/src/JaqalPaw.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaqalPaw
-Version: 1.2.0a1
+Version: 1.3.0a1
 Summary: Just Another Quantum Assembly Language Pulses and Waveform Specification
 Home-page: https://qscout.sandia.gov
 Author: Daniel Lobser, Benjamin C. A. Morrison, Kenneth Rudinger, Antonio Russo, Jay Wesley Van Der Wall
 Author-email: qscout@sandia.gov
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,18 +12,23 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: emulator
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: jaqalpaq>=1.3.0a1
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Provides-Extra: emulator
+Requires-Dist: matplotlib; extra == "emulator"
 
 For information on JaqalPaw usage and parameter descriptions, see the official
 [JaqalPaw manual](https://www.sandia.gov/app/uploads/sites/174/2021/11/JaqalPaw__A_Guide_to_Defining_Pulses_and_Waveforms_for_Jaqal.pdf),
 which can be found at [qscout.sandia.gov](https://qscout.sandia.gov).
 
 # Running The Emulator
```

### Comparing `JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/SOURCES.txt` & `jaqalpaw-1.3.0a1/src/JaqalPaw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/_cli.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/_cli.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/binary_conversion.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/bytecode/binary_conversion.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/encoding_parameters.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/bytecode/encoding_parameters.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/lut_programming.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/bytecode/lut_programming.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/pulse_binarization.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/bytecode/pulse_binarization.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/spline_mapping.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/bytecode/spline_mapping.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/compiler/jaqal_compiler.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/compiler/jaqal_compiler.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/compiler/time_ordering.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/compiler/time_ordering.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/arbiters.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/emulator/arbiters.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/byte_decoding.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/emulator/byte_decoding.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/firmware_emulator.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/emulator/firmware_emulator.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/pdq_spline.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/emulator/pdq_spline.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/uram.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/emulator/uram.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/ir/ast_utilities.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/ir/ast_utilities.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/ir/circuit_constructor.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/ir/circuit_constructor.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/ir/circuit_constructor_visitor.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/ir/circuit_constructor_visitor.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/ir/gate_slice.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/ir/gate_slice.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/ir/padding.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/ir/padding.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/ir/pulse_data.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/ir/pulse_data.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/datatypes.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/utilities/datatypes.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/helper_functions.py` & `jaqalpaw-1.3.0a1/src/jaqalpaw/utilities/helper_functions.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/src/qscout/v1/QSCOUTBuiltins.py` & `jaqalpaw-1.3.0a1/src/qscout/v1/QSCOUTBuiltins.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/tests/benchmark/benchmark.py` & `jaqalpaw-1.3.0a1/tests/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/tests/run_benchmarks.py` & `jaqalpaw-1.3.0a1/tests/run_benchmarks.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/tests/test_backcompat.py` & `jaqalpaw-1.3.0a1/tests/test_backcompat.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/tests/test_repro.py` & `jaqalpaw-1.3.0a1/tests/test_repro.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.2.0a1/tests/test_smoke.py` & `jaqalpaw-1.3.0a1/tests/test_smoke.py`

 * *Files identical despite different names*

