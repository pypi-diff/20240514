# Comparing `tmp/debyetools-2.0.6.tar.gz` & `tmp/debyetools-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debyetools-2.0.6.tar", last modified: Fri May 10 16:22:04 2024, max compression
+gzip compressed data, was "debyetools-2.1.tar", last modified: Tue May 14 19:17:43 2024, max compression
```

## Comparing `debyetools-2.0.6.tar` & `debyetools-2.1.tar`

### file list

```diff
@@ -1,182 +1,185 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.591814 debyetools-2.0.6/
--rw-rw-r--   0 travis    (2000) travis    (2000)    34521 2024-05-10 16:20:12.000000 debyetools-2.0.6/LICENSE.md
--rw-r--r--   0 travis    (2000) travis    (2000)     4174 2024-05-10 16:22:04.591814 debyetools-2.0.6/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3294 2024-05-10 16:20:12.000000 debyetools-2.0.6/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.479803 debyetools-2.0.6/debyetools/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12478 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/anharmonicity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7994 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/aux_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3054 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/debfunct.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9511 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/defects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8553 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/electronic.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.479803 debyetools-2.0.6/debyetools/examples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.495805 debyetools-2.0.6/debyetools/examples/Ag_fcc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      732 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/CONTCAR.5
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.00
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)  1577236 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/OUTCAR.eps
--rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/SUMMARY.fcc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.515807 debyetools-2.0.6/debyetools/examples/Al3Li_D022/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1144 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/CONTCAR.5
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.00
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)  4597169 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/OUTCAR.eps
--rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/SUMMARY.fcc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.551810 debyetools-2.0.6/debyetools/examples/Al3Li_D023/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2063 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/CONTCAR.5
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.00
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)  5101281 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/OUTCAR.eps
--rw-rw-r--   0 travis    (2000) travis    (2000)     1576 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/SUMMARY.fcc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.567812 debyetools-2.0.6/debyetools/examples/Al3Li_L12/
--rw-rw-r--   0 travis    (2000) travis    (2000)      743 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/CONTCAR.5
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.00
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)  6488719 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/OUTCAR.eps
--rw-rw-r--   0 travis    (2000) travis    (2000)     1586 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/SUMMARY.fcc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.583814 debyetools-2.0.6/debyetools/examples/Al_fcc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      744 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/CONTCAR.5
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.00
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.1
--rw-rw-r--   0 travis    (2000) travis    (2000)  1485651 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/OUTCAR.eps
--rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/SUMMARY.fcc
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1532 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/fs_compound_db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13605 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/ndeb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4340 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/pairanalysis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3651 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/poisson.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   176909 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/potentials.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.587814 debyetools-2.0.6/debyetools/tpropsgui/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13556 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/atomtools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      688 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/dialog_doscar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1480 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/dialog_outcar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2079 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/dialog_summary.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      268 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/dialog_warning.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3019 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/elements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34358 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/events.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13883 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/functions0.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2272 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/get_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    43045 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/gui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      822 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/keygen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10086 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/layout.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      876 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/lock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10587 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/mainwindow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/plot_EV.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11627 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/plotter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4359 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/plotter_class.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      883 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/toolbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3416 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_dialogSUMMARY.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2460 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_dialog_doscar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2221 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_dialog_outcar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16226 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_heatcapacitywindow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18970 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_interatomic_params.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22872 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_mainwindow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_missingkey.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_warning.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8050 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/window_cp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6637 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/window_interatomicparams.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26101 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/vibrational.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.591814 debyetools-2.0.6/debyetools.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     4174 2024-05-10 16:22:04.000000 debyetools-2.0.6/debyetools.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     6985 2024-05-10 16:22:04.000000 debyetools-2.0.6/debyetools.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-10 16:22:04.000000 debyetools-2.0.6/debyetools.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       35 2024-05-10 16:22:04.000000 debyetools-2.0.6/debyetools.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2024-05-10 16:22:04.000000 debyetools-2.0.6/debyetools.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-05-10 16:22:04.591814 debyetools-2.0.6/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1531 2024-05-10 16:20:13.000000 debyetools-2.0.6/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-14 19:17:43.094963 debyetools-2.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34521 2024-05-14 19:15:56.000000 debyetools-2.1/LICENSE.md
+-rw-r--r--   0 travis    (2000) travis    (2000)     4172 2024-05-14 19:17:43.090963 debyetools-2.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3294 2024-05-14 19:15:56.000000 debyetools-2.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-14 19:17:42.986956 debyetools-2.1/debyetools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12478 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/anharmonicity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7994 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/aux_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3054 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/debfunct.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9511 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/defects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8553 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/electronic.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-14 19:17:42.990956 debyetools-2.1/debyetools/examples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-14 19:17:43.002957 debyetools-2.1/debyetools/examples/Ag_fcc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      732 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/CONTCAR.5
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.00
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1577236 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/OUTCAR.eps
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Ag_fcc/SUMMARY.fcc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-14 19:17:43.022958 debyetools-2.1/debyetools/examples/Al3Li_D022/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1144 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/CONTCAR.5
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.00
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)  4597169 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/OUTCAR.eps
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D022/SUMMARY.fcc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-14 19:17:43.054961 debyetools-2.1/debyetools/examples/Al3Li_D023/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2063 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/CONTCAR.5
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.00
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-14 19:15:56.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)  5101281 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/OUTCAR.eps
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1576 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_D023/SUMMARY.fcc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-14 19:17:43.070962 debyetools-2.1/debyetools/examples/Al3Li_L12/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      743 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/CONTCAR.5
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.00
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)  6488719 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/OUTCAR.eps
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1586 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al3Li_L12/SUMMARY.fcc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-14 19:17:43.082963 debyetools-2.1/debyetools/examples/Al_fcc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      744 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/CONTCAR.5
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.00
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.1
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1485651 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/OUTCAR.eps
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/Al_fcc/SUMMARY.fcc
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/examples/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1532 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/fs_compound_db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13605 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/ndeb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4340 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/pairanalysis.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3651 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/poisson.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   176909 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/potentials.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-14 19:17:43.090963 debyetools-2.1/debyetools/tpropsgui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13788 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/atomtools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4487 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/custom_widgets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      689 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/dialog_doscar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1032 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/dialog_outcar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2387 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/dialog_periodictable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/dialog_summary.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      268 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/dialog_warning.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3019 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/elements.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34358 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/events.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13883 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/functions0.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2272 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/get_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    43045 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/gui.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      822 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/keygen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10086 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/layout.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      876 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/lock.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13265 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/mainwindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/plot_EV.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11627 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/plotter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4359 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/plotter_class.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      883 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/toolbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3416 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/ui_dialogSUMMARY.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2460 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/ui_dialog_doscar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2221 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/ui_dialog_outcar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58505 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/ui_dialog_periodictable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19763 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/ui_heatcapacitywindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19010 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/ui_interatomic_params.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36599 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/ui_mainwindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/ui_missingkey.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/ui_warning.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8894 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/window_cp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6637 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/tpropsgui/window_interatomicparams.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26101 2024-05-14 19:15:57.000000 debyetools-2.1/debyetools/vibrational.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-14 19:17:43.090963 debyetools-2.1/debyetools.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     4172 2024-05-14 19:17:42.000000 debyetools-2.1/debyetools.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7117 2024-05-14 19:17:42.000000 debyetools-2.1/debyetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-14 19:17:42.000000 debyetools-2.1/debyetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       35 2024-05-14 19:17:42.000000 debyetools-2.1/debyetools.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2024-05-14 19:17:42.000000 debyetools-2.1/debyetools.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-05-14 19:17:43.094963 debyetools-2.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1529 2024-05-14 19:15:57.000000 debyetools-2.1/setup.py
```

### Comparing `debyetools-2.0.6/LICENSE.md` & `debyetools-2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/PKG-INFO` & `debyetools-2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debyetools
-Version: 2.0.6
+Version: 2.1
 Summary: Debye approximation implementation for the calculation of thermodynamic properties from ground-state atomistic simulations.
 Home-page: https://debyetools.readthedocs.io/
 Author: Javier Jofre
 Author-email: javier.jofre@polymtl.ca
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `debyetools-2.0.6/README.md` & `debyetools-2.1/README.md`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/anharmonicity.py` & `debyetools-2.1/debyetools/anharmonicity.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/aux_functions.py` & `debyetools-2.1/debyetools/aux_functions.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/debfunct.py` & `debyetools-2.1/debyetools/debfunct.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/defects.py` & `debyetools-2.1/debyetools/defects.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/electronic.py` & `debyetools-2.1/debyetools/electronic.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/CONTCAR.5` & `debyetools-2.1/debyetools/examples/Ag_fcc/CONTCAR.5`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.00` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.00`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.01` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.02` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.03` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.04` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.05` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.06` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.07` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.08` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.09` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.10` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.01` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.02` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.03` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.04` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.05` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.06` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.07` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.08` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.09` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.10` & `debyetools-2.1/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/OUTCAR.eps` & `debyetools-2.1/debyetools/examples/Ag_fcc/OUTCAR.eps`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Ag_fcc/SUMMARY.fcc` & `debyetools-2.1/debyetools/examples/Ag_fcc/SUMMARY.fcc`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/CONTCAR.5` & `debyetools-2.1/debyetools/examples/Al3Li_D022/CONTCAR.5`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.00` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.00`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.01` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.02` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.03` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.04` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.05` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.06` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.07` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.08` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.09` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.10` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.01` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.02` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.03` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.04` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.05` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.06` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.07` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.08` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.09` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.10` & `debyetools-2.1/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/OUTCAR.eps` & `debyetools-2.1/debyetools/examples/Al3Li_D022/OUTCAR.eps`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D022/SUMMARY.fcc` & `debyetools-2.1/debyetools/examples/Al3Li_D022/SUMMARY.fcc`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/CONTCAR.5` & `debyetools-2.1/debyetools/examples/Al3Li_D023/CONTCAR.5`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.00` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.00`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.01` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.02` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.03` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.04` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.05` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.06` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.07` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.08` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.09` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.10` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.01` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.02` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.03` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.04` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.05` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.06` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.07` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.08` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.09` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.10` & `debyetools-2.1/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/OUTCAR.eps` & `debyetools-2.1/debyetools/examples/Al3Li_D023/OUTCAR.eps`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_D023/SUMMARY.fcc` & `debyetools-2.1/debyetools/examples/Al3Li_D023/SUMMARY.fcc`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/CONTCAR.5` & `debyetools-2.1/debyetools/examples/Al3Li_L12/CONTCAR.5`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.00` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.00`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.01` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.02` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.03` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.04` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.05` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.06` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.07` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.08` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.09` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.10` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.01` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.02` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.03` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.04` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.05` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.06` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.07` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.08` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.09` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.10` & `debyetools-2.1/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/OUTCAR.eps` & `debyetools-2.1/debyetools/examples/Al3Li_L12/OUTCAR.eps`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al3Li_L12/SUMMARY.fcc` & `debyetools-2.1/debyetools/examples/Al3Li_L12/SUMMARY.fcc`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/CONTCAR.5` & `debyetools-2.1/debyetools/examples/Al_fcc/CONTCAR.5`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.00` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.00`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.01` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.02` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.03` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.04` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.05` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.06` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.07` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.08` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.09` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.10` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.01` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.02` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.03` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.04` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.05` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.06` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.07` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.08` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.09` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.1` & `debyetools-2.1/debyetools/examples/Al_fcc/DOSCAR.EvV.0.1`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/OUTCAR.eps` & `debyetools-2.1/debyetools/examples/Al_fcc/OUTCAR.eps`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/examples/Al_fcc/SUMMARY.fcc` & `debyetools-2.1/debyetools/examples/Al_fcc/SUMMARY.fcc`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/fs_compound_db.py` & `debyetools-2.1/debyetools/fs_compound_db.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/ndeb.py` & `debyetools-2.1/debyetools/ndeb.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/pairanalysis.py` & `debyetools-2.1/debyetools/pairanalysis.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/poisson.py` & `debyetools-2.1/debyetools/poisson.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/potentials.py` & `debyetools-2.1/debyetools/potentials.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/dialog_doscar.py` & `debyetools-2.1/debyetools/tpropsgui/dialog_doscar.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,7 +15,8 @@
     def getfiles(self):
             filepath = QFileDialog.getExistingDirectory(self, caption='Select a folder')
             self.ui.filepath.setText(filepath)
 
     def on_pushButton_OK(self):
         self.filepath = self.ui.filepath.text()
         self.close()
+
```

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/dialog_outcar.py` & `debyetools-2.1/debyetools/tpropsgui/dialog_summary.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 from PySide6.QtWidgets import  QDialog, QFileDialog
-from debyetools.tpropsgui.ui_dialog_outcar import Ui_Dialog as Ui_OUTCAR
-from debyetools.aux_functions import load_EM as dt_load_EM
-
-class dialogOUTCAR(QDialog):
+from debyetools.tpropsgui.ui_dialogSUMMARY import Ui_Dialog as Ui_SUMMARY
+from debyetools.tpropsgui.atomtools import atomic_mass
+from debyetools.aux_functions import load_V_E as dt_load_V_E
+
+def log_mean(lst):
+    import numpy as np
+    l = len(lst)
+    # lm = np.sum([np.log(li)/l for li in lst])
+
+    # m = np.exp(lm)
+    return np.sum([li for li in lst])/l
+class dialogSUMMARY(QDialog):
     def __init__(self, parent=None):
         super().__init__(parent)
-        self.ui = Ui_OUTCAR()
+        self.ui = Ui_SUMMARY()
         self.ui.setupUi(self)
 
-        self.ui.browseoutcar.clicked.connect(self.getfilesoutcar)
-#        self.ui.browseposcar.clicked.connect(self.getfilesposcar)
+        self.ui.browsesummary.clicked.connect(self.getfilessummary)
+        self.ui.browseposcar.clicked.connect(self.getfilesposcar)
         self.ui.ok.clicked.connect(self.on_pushButton_OK)
         self.filepath='.'
 
-    def getfilesoutcar(self):
-        outcarpath, _ = QFileDialog.getOpenFileName(self, caption='Select an OUTCAR file')
-        self.ui.outcarpath.setText(outcarpath)
-
-#    def getfilesposcar(self):
-#        poscarpath, _ = QFileDialog.getOpenFileName(self, caption='Select a POSCAR or CONTCAR file')
-#        self.ui.poscarpath.setText(poscarpath)
+    def getfilessummary(self):
+        summarypath, _ = QFileDialog.getOpenFileName(self, caption='Select a SUMMARY file')
+        self.ui.summarypath.setText(summarypath)
+        self.summarypath = summarypath
+
+    def getfilesposcar(self):
+        poscarpath, _ = QFileDialog.getOpenFileName(self, caption='Select a POSCAR or CONTCAR file')
+        self.ui.poscarpath.setText(poscarpath)
+        self.poscarpath = poscarpath
 
     def on_pushButton_OK(self):
-        self.outcarpath = self.ui.outcarpath.text()
-#        self.poscarpath = self.ui.poscarpath.text()
+        self.summarypath = self.ui.summarypath.text()
+        self.poscarpath = self.ui.poscarpath.text()
         self.close()
-    def closeEvent(self, event):
-        EM = dt_load_EM(self.outcarpath)
-#        print(EM)
 
-        txt2paste = ''
-        for rowi in EM:
-            txt2paste=txt2paste+' '.join(['%.2f'%(float(coli)/10) for coli in rowi])+'\n'
+    def closeEvent(self, event):
+        V, E = dt_load_V_E(self.summarypath, self.poscarpath)
+        with open(self.poscarpath) as f:
+            poscar_lines = f.readlines()
+        elmnts = poscar_lines[5].split()
+        mult = poscar_lines[6].split()
+        elmntsall = []
+        for e, m in zip(elmnts, mult):
+            elmntsall = elmntsall + [e]*int(m)
+        masses = [float(atomic_mass[e])/1000. for e in elmntsall]
+        txt2paste = '#V\tE\n'
+        for v, e in zip(V, E):
+            txt2paste = txt2paste + '%.6e\t%.6e'%(v, e)+'\n'
+        self.EvVtext.setPlainText(txt2paste)
+        self.mass.setText(str(log_mean(masses)))
 #        print('event', event)
-        self.elastic_constants.setText(txt2paste)
-
-# This Python file uses the following encoding: utf-8
 
-# if __name__ == "__main__":
-#     pass
```

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/elements.py` & `debyetools-2.1/debyetools/tpropsgui/elements.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/events.py` & `debyetools-2.1/debyetools/tpropsgui/events.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/functions0.py` & `debyetools-2.1/debyetools/tpropsgui/functions0.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/get_functions.py` & `debyetools-2.1/debyetools/tpropsgui/get_functions.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/gui.py` & `debyetools-2.1/debyetools/tpropsgui/gui.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/keygen.py` & `debyetools-2.1/debyetools/tpropsgui/keygen.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/layout.py` & `debyetools-2.1/debyetools/tpropsgui/layout.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/lock.py` & `debyetools-2.1/debyetools/tpropsgui/lock.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/mainwindow.py` & `debyetools-2.1/debyetools/tpropsgui/mainwindow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from PySide6.QtWidgets import QMainWindow
 from PySide6.QtGui import QIcon
 
 from debyetools.tpropsgui.dialog_doscar import dialogDOSCAR
 from debyetools.tpropsgui.dialog_summary import dialogSUMMARY
 from debyetools.tpropsgui.dialog_outcar import dialogOUTCAR
 from debyetools.tpropsgui.dialog_warning import dialogWarning
+from debyetools.tpropsgui.dialog_periodictable import dialogPeriodicTable
+
+
 from debyetools.tpropsgui.window_cp import windowCp
 from debyetools.tpropsgui.window_interatomicparams import windowInteratormic
 from debyetools.tpropsgui.plot_EV import windowPlot
 
 from debyetools.tpropsgui.ui_mainwindow import Ui_MainWindow as Ui_MW
 from debyetools.tpropsgui.ui_missingkey import Ui_Form as Ui_KEY
 
@@ -18,14 +21,31 @@
 
 from debyetools.poisson import poisson_ratio as dt_poisson_ratio
 from debyetools.aux_functions import load_doscar as dt_load_doscar
 from debyetools.electronic import fit_electronic as dt_fit_electronic
 
 from debyetools.tpropsgui.lock import keygen as kg
 
+import traceback
+import re
+
+def separate_atoms(formula):
+    # This pattern matches element symbols (one or two letters, starting with an uppercase letter)
+    # followed by optional counts (numbers)
+    pattern = r"([A-Z][a-z]*)(\d*)"
+    elements = re.findall(pattern, formula)
+    separated = []
+
+    for element, count in elements:
+        # If count is empty, it means there is one atom of this element
+        count = int(count) if count else 1
+        separated.extend([element] * count)
+
+    return separated
+
 class MainWindow(QMainWindow):
     def __init__(self, parent=None, app=None):
 
         super().__init__(parent)
 
         key1 = kg()
         try:
@@ -55,27 +75,30 @@
         self.cp_window = windowCp(self)
         self.cp_window.app = app
         self.doscardialog = dialogDOSCAR(self)
         self.summarydialog = dialogSUMMARY(self)
         self.outcardialog = dialogOUTCAR(self)
         self.warningdialog = dialogWarning(self)
 
+        self.dialogperiodictable = dialogPeriodicTable(self)
+        self.dialogperiodictable.external_lineEdit = self.ui.lineEdit_11
+        self.dialogperiodictable.external_lineEdit2 = self.ui.lineEdit
+
         self.ui.pushButton.clicked.connect(self.on_pushButton_fitEOS)
         self.ui.pushButton_5.clicked.connect(self.on_pushButton_Cp)
         self.ui.pushButton_2.clicked.connect(self.on_pushButton_calc_nu)
 
         self.ui.pushButton_3.clicked.connect(self.on_pushButton_calculate_el)
 
         self.eos_str = 'BM'
 
         self.molecule = Molecule()
 
         self.ui.comboBox.currentIndexChanged.connect(self.selectionchange)
 
-
         self.check_el, self.check_def, self.check_anh, self.check_xs = self.ui.checkBox, self.ui.checkBox_2, self.ui.checkBox_3, self.ui.checkBox_4
 
         self.state_el = False
         self.state_def = False
         self.state_anh = False
         self.state_xs = False
 
@@ -94,34 +117,43 @@
         self.plotwindow = windowPlot(self)
         self.ui.actionEV.triggered.connect(self.plotEV)
 
         self.ui.actionDOSCAR.triggered.connect(self.on_pushButton_loaddata)
         self.ui.actionSUMMARY.triggered.connect(self.on_pushButton_loadSUMMARY)
         self.ui.actionOUTCAR.triggered.connect(self.on_pushButton_loadOUTCAR)
 
+        self.ui.lineEdit_11.clicked.connect(self.showDialog)
+
+    def showDialog(self):
+        self.dialogperiodictable.ui.lineEdit.setText(self.ui.lineEdit_11.text())
+        self.dialogperiodictable.show()  # Assuming dialogxx is initialized and ready to be displayed
+
     def plotEV(self):
-        Xdata = self.Vdata/1e-5
-        Ydata = self.Edata/1e3
+        Xdata = self.Vdata / 1e-5
+        Ydata = self.Edata / 1e3
         self.plotwindow.ax.cla()
-        self.plotwindow.ax.plot(Xdata, Ydata, ls = '', marker='.', label = 'data', mfc='None', mec='black', markersize=10,mew=1)
-        self.plotwindow.ax.plot(Xdata, [self.eos.E0(Vi)/1e3 for Vi in Xdata*1e-5], ls = '', marker='+', label = 'model', mfc='purple', mec='purple', markersize=10,mew=1)
-
-        spanX = (max(Xdata) - min(Xdata))/20
-        spanY = (max(Ydata) - min(Ydata))/20
-        self.plotwindow.ax.set_xlim((min(Xdata)-spanX, max(Xdata)+spanX))
-        self.plotwindow.ax.set_ylim((min(Ydata)-spanY, max(Ydata)+spanY))
+        self.plotwindow.ax.plot(Xdata, Ydata, ls='', marker='.', label='data', mfc='None', mec='black', markersize=10,
+                                mew=1)
+        self.plotwindow.ax.plot(Xdata, [self.eos.E0(Vi) / 1e3 for Vi in Xdata * 1e-5], ls='', marker='+', label='model',
+                                mfc='purple', mec='purple', markersize=10, mew=1)
+
+        spanX = (max(Xdata) - min(Xdata)) / 20
+        spanY = (max(Ydata) - min(Ydata)) / 20
+        self.plotwindow.ax.set_xlim((min(Xdata) - spanX, max(Xdata) + spanX))
+        self.plotwindow.ax.set_ylim((min(Ydata) - spanY, max(Ydata) + spanY))
         self.plotwindow.ax.legend(loc=9)
         self.plotwindow.ax.set_xlabel(r'$10^{-5}m^3/mol$-$at$')
         self.plotwindow.ax.set_ylabel(r'$kJ/mol$-$at$')
         self.plotwindow.show()
 
     def selectionchange(self, i):
         self.ui.progress_2.setValue(0)
-        dict_eos = {'Birch-Murnaghan':'BM', 'Rose-Vinet':'RV', 'Mie-Gruneisen':'MG', 'TB-SMA':'TB',
-                    'Murnaghan':'MU', 'Poirier-Tarantola':'PT', 'Morse int. potential':'MP', 'EAM int. potential':'EAM'}
+        dict_eos = {'Birch-Murnaghan': 'BM', 'Rose-Vinet': 'RV', 'Mie-Gruneisen': 'MG', 'TB-SMA': 'TB',
+                    'Murnaghan': 'MU', 'Poirier-Tarantola': 'PT', 'Morse int. potential': 'MP',
+                    'EAM int. potential': 'EAM'}
         self.eos_str = dict_eos[self.ui.comboBox.itemText(i)]
 
         self.ipotparamsdialog.args = (None,)
         self.ui.lineEdit_2.setText('-3e5, 1e-5, 7e10, 4')
         if self.eos_str in ['MP', 'EAM']:
             self.ipotparamsdialog.ui.plainTextEdit.setPlainText('')
             for axi in self.ipotparamsdialog.ax:
@@ -134,45 +166,46 @@
             self.ipotparamsdialog.ui.OKbutton.setEnabled(False)
             self.ipotparamsdialog.show()
 
     def get_EvV(self):
         if self.ui.radioButton.isChecked():
             conv = [(1e-30 * 6.02e23), (0.160218e-18 * 6.02214e23)]
         elif self.ui.radioButton_3.isChecked():
-            conv =[1, 1]
+            conv = [1, 1]
 
         txt = self.ui.EvVText.toPlainText().split('\n')
         data_lst = []
         for ti in txt:
-            if len(ti)==0:continue
-            if ti[0]=='#': continue
+            if len(ti) == 0: continue
+            if ti[0] == '#': continue
             data_lst.append([float(tii) for tii in ti.split()])
         data = np.array(data_lst)
         ncols = len(data.T)
-        return (data[:,i]*conv[i] for i in range(ncols))
+        return (data[:, i] * conv[i] for i in range(ncols))
 
     def get_EOS_params(self):
         txt = self.ui.lineEdit_2.text()
-        if txt=='':
-            return -3e5,9e-6,7e10,4
-        return  [float(ti) for ti in txt.replace(' ','').split(',')]
+        if txt == '':
+            return -3e5, 9e-6, 7e10, 4
+        return [float(ti) for ti in txt.replace(' ', '').split(',')]
 
     def get_el_params(self):
         txt = self.ui.lineEdit_el.text()
-        if txt=='':
+        if txt == '':
             return 3e-01, -1e+04, 5e-04, 1e-06
-        return  [float(ti) for ti in txt.replace(' ','').split(',')]
+        return [float(ti) for ti in txt.replace(' ', '').split(',')]
 
     def get_C(self):
-        txt = self.ui.elastic_constants.toPlainText().replace('XX',' ').replace('YY',' ').replace('ZZ',' ').replace('XY',' ').replace('YZ',' ').replace('ZX',' ').split('\n')
+        txt = self.ui.elastic_constants.toPlainText().replace('XX', ' ').replace('YY', ' ').replace('ZZ', ' ').replace(
+            'XY', ' ').replace('YZ', ' ').replace('ZX', ' ').split('\n')
         data_lst = []
         for ti in txt:
-            if len(ti)==0:continue
-            if ti[0]=='#': continue
-            data_lst.append([float(tii) for tii in ti.replace('\t',' ').split()])
+            if len(ti) == 0: continue
+            if ti[0] == '#': continue
+            data_lst.append([float(tii) for tii in ti.replace('\t', ' ').split()])
         data = np.array(data_lst)
 
         return data
 
     def on_check_el(self):
         self.state_el = self.check_el.isChecked()
         self.ui.lineEdit_el.setEnabled(self.state_el)
@@ -194,51 +227,74 @@
         self.eos = getattr(dt_potentials, self.eos_str)(*self.ipotparamsdialog.args)
 
         Vdata, Edata = self.get_EvV()
         self.Vdata = Vdata
         self.Edata = Edata
 
         initial_guess = self.get_EOS_params()
-        self.eos.fitEOS(Vdata, Edata, initial_parameters = initial_guess, fit=True)
+        self.eos.fitEOS(Vdata, Edata, initial_parameters=initial_guess, fit=True)
 
         self.ui.lineEdit_2.setText(', '.join(['%.9e' % (p) for p in self.eos.pEOS]))
         self.ui.progress_2.setValue(100)
 
     def on_pushButton_calc_nu(self):
         C = self.get_C()
         BR, BV, B, GR, GV, S, AU, nu = dt_poisson_ratio(C, quiet=True)
-        self.ui.lineEdit_3.setText('%.3f'%(nu))
-        self.ui.lineEdit_4.setText('%.1f'%(BR*10))
-        self.ui.lineEdit_5.setText('%.1f'%(BV*10))
-        self.ui.lineEdit_6.setText('%.1f'%(B*10))
-        self.ui.lineEdit_9.setText('%.1f'%(GR*10))
-        self.ui.lineEdit_8.setText('%.1f'%(GV*10))
-        self.ui.lineEdit_7.setText('%.1f'%(S*10))
-        self.ui.lineEdit_10.setText('%.2f'%(AU))
+        self.ui.lineEdit_3.setText('%.3f' % (nu))
+        self.ui.lineEdit_4.setText('%.1f' % (BR * 10))
+        self.ui.lineEdit_5.setText('%.1f' % (BV * 10))
+        self.ui.lineEdit_6.setText('%.1f' % (B * 10))
+        self.ui.lineEdit_9.setText('%.1f' % (GR * 10))
+        self.ui.lineEdit_8.setText('%.1f' % (GV * 10))
+        self.ui.lineEdit_7.setText('%.1f' % (S * 10))
+        self.ui.lineEdit_10.setText('%.2f' % (AU))
 
     def on_pushButton_Cp(self):
-        self.molecule.nu = float(self.ui.lineEdit_3.text())
-        self.molecule.mass = float(self.ui.lineEdit.text())
-
-        self.molecule.p_anh = [float(si) for si in self.ui.lineEdit_anh.text().replace(',',' ').split()] if self.state_anh else [0,1]
-        self.molecule.p_el = [float(si) for si in self.ui.lineEdit_el.text().replace(',',' ').split()] if self.state_el else [0,0,0,0]
-        self.molecule.p_def = [float(si) for si in self.ui.lineEdit_def.text().replace(',',' ').split()] if self.state_def else [100, 1, 1000, 0.1]
-        self.molecule.p_xs = [float(si) for si in self.ui.lineEdit_xs.text().replace(',',' ').split()] if self.state_xs else [0,0,0]
-
-        self.molecule.initial_params = [float(si) for si in self.ui.lineEdit_2.text().replace(',',' ').split()]
-
-        if self.eos_str in ['MP','EAM']:
-            args = [self.molecule.formula, self.molecule.cell, self.molecule.basis, self.molecule.cutoff, self.molecule.number_of_NNs]
-        else:
-            args = [None]
-        self.molecule.set_eos(self.eos_str, args)
+        try:
+            self.molecule.nu = float(self.ui.lineEdit_3.text())
+            self.molecule.mass = float(self.ui.lineEdit.text())
 
+            self.molecule.p_anh = [float(si) for si in
+                                   self.ui.lineEdit_anh.text().replace(',', ' ').split()] if self.state_anh else [0, 1]
+            self.molecule.p_el = [float(si) for si in
+                                  self.ui.lineEdit_el.text().replace(',', ' ').split()] if self.state_el else [0, 0, 0,
+                                                                                                               0]
+            self.molecule.p_def = [float(si) for si in
+                                   self.ui.lineEdit_def.text().replace(',', ' ').split()] if self.state_def else [100,
+                                                                                                                  1,
+                                                                                                                  1000,
+                                                                                                                  0.1]
+            self.molecule.p_xs = [float(si) for si in
+                                  self.ui.lineEdit_xs.text().replace(',', ' ').split()] if self.state_xs else [0, 0, 0]
+
+            self.molecule.initial_params = [float(si) for si in self.ui.lineEdit_2.text().replace(',', ' ').split()]
+
+            if self.eos_str in ['MP', 'EAM']:
+                args = [self.molecule.formula, self.molecule.cell, self.molecule.basis, self.molecule.cutoff,
+                        self.molecule.number_of_NNs]
+            else:
+                args = [None]
+            self.molecule.set_eos(self.eos_str, args)
+
+            self.cp_window.ui.lineEdit.setText(self.ui.lineEdit_T.text())
+            self.cp_window.ui.lineEdit_2.setText(self.ui.lineEdit_P.text())
+
+            types = separate_atoms(self.ui.lineEdit_11.text())
+            self.molecule.update_fomula(types)
+            self.cp_window.debye_run(self.molecule, self.ui.progress, self.ui.lineEdit_11.text())
+            self.cp_window.show()
+        except Exception as e:
+            print(e)
+            error_message = f"An error occurred: {e}\n"
+            error_traceback = traceback.format_exc()
 
-        self.cp_window.debye_run(self.molecule, self.ui.progress)
-        self.cp_window.show()
+            # Combine the error message with the traceback
+            full_error_text = error_message + error_traceback
+            self.warningdialog.ui.label.setText(full_error_text)
+            self.warningdialog.show()
 
     def on_pushButton_loaddata(self):
         self.doscardialog.show()
 
     def on_pushButton_loadSUMMARY(self):
         self.summarydialog.mass = self.ui.lineEdit
         self.summarydialog.EvVtext = self.ui.EvVText
@@ -248,15 +304,18 @@
         self.outcardialog.elastic_constants = self.ui.elastic_constants
         self.outcardialog.show()
 
     def on_pushButton_calculate_el(self):
         Vdata, Edata = self.get_EvV()
         self.Vdata = Vdata
         try:
-            E, N, Ef = dt_load_doscar(self.doscardialog.filepath+'/DOSCAR.', list_filetags = [i+1 for i in range(len(Vdata))])
+            E, N, Ef = dt_load_doscar(self.doscardialog.filepath + '/DOSCAR.',
+                                      list_filetags=[i + 1 for i in range(len(Vdata))])
             p_el_initial = self.get_el_params()
-            p_electronic = dt_fit_electronic(self.Vdata, p_el_initial,E,N,Ef)
+            p_electronic = dt_fit_electronic(self.Vdata, p_el_initial, E, N, Ef)
             self.ui.lineEdit_el.setText(', '.join(['%.9e' % (p) for p in p_electronic]))
         except Exception as e:
             print(e)
-            self.warningdialog.ui.label.setText(str(e)+"\n\nProbably you haven't set a filepath to the eDOS data yet.")
-            self.warningdialog.show()
+            self.warningdialog.ui.label.setText(
+                str(e) + "\n\nProbably you haven't set a filepath to the eDOS data yet.")
+            self.warningdialog.show()
+
```

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/plot_EV.py` & `debyetools-2.1/debyetools/tpropsgui/plot_EV.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/plotter.py` & `debyetools-2.1/debyetools/tpropsgui/plotter.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/plotter_class.py` & `debyetools-2.1/debyetools/tpropsgui/plotter_class.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/toolbox.py` & `debyetools-2.1/debyetools/tpropsgui/toolbox.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/ui_dialogSUMMARY.py` & `debyetools-2.1/debyetools/tpropsgui/ui_dialogSUMMARY.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'dialogSUMMARY.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.2
+## Created by: Qt User Interface Compiler version 6.6.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/ui_dialog_doscar.py` & `debyetools-2.1/debyetools/tpropsgui/ui_dialog_doscar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'dialog_DOSCAR.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.2
+## Created by: Qt User Interface Compiler version 6.6.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/ui_dialog_outcar.py` & `debyetools-2.1/debyetools/tpropsgui/ui_dialog_outcar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'dialogOUTCAR.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.2
+## Created by: Qt User Interface Compiler version 6.6.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/ui_heatcapacitywindow.py` & `debyetools-2.1/debyetools/tpropsgui/ui_heatcapacitywindow.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,223 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'heatcapacitywindow.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.2
+## Created by: Qt User Interface Compiler version 6.6.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
 from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
     QFont, QFontDatabase, QGradient, QIcon,
     QImage, QKeySequence, QLinearGradient, QPainter,
     QPalette, QPixmap, QRadialGradient, QTransform)
 from PySide6.QtWidgets import (QApplication, QComboBox, QHBoxLayout, QHeaderView,
     QLabel, QLineEdit, QMainWindow, QMenuBar,
     QProgressBar, QPushButton, QRadioButton, QSizePolicy,
-    QStatusBar, QTableWidget, QTableWidgetItem, QWidget)
+    QSpacerItem, QStatusBar, QTableWidget, QTableWidgetItem,
+    QVBoxLayout, QWidget)
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         if not MainWindow.objectName():
             MainWindow.setObjectName(u"MainWindow")
-        MainWindow.resize(818, 578)
+        MainWindow.resize(808, 525)
         self.centralwidget = QWidget(MainWindow)
         self.centralwidget.setObjectName(u"centralwidget")
-        self.label_3 = QLabel(self.centralwidget)
-        self.label_3.setObjectName(u"label_3")
-        self.label_3.setGeometry(QRect(720, 50, 51, 20))
-        self.lineEdit_2 = QLineEdit(self.centralwidget)
-        self.lineEdit_2.setObjectName(u"lineEdit_2")
-        self.lineEdit_2.setGeometry(QRect(600, 50, 113, 24))
+        self.horizontalLayout_9 = QHBoxLayout(self.centralwidget)
+        self.horizontalLayout_9.setObjectName(u"horizontalLayout_9")
+        self.verticalLayout_2 = QVBoxLayout()
+        self.verticalLayout_2.setObjectName(u"verticalLayout_2")
+        self.horizontalLayout = QHBoxLayout()
+        self.horizontalLayout.setObjectName(u"horizontalLayout")
+
+        self.verticalLayout_2.addLayout(self.horizontalLayout)
+
+        self.horizontalLayout_8 = QHBoxLayout()
+        self.horizontalLayout_8.setObjectName(u"horizontalLayout_8")
+        self.horizontalSpacer_5 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+
+        self.horizontalLayout_8.addItem(self.horizontalSpacer_5)
+
+        self.label_12 = QLabel(self.centralwidget)
+        self.label_12.setObjectName(u"label_12")
+
+        self.horizontalLayout_8.addWidget(self.label_12)
+
+        self.comboBox_2 = QComboBox(self.centralwidget)
+        self.comboBox_2.addItem("")
+        self.comboBox_2.addItem("")
+        self.comboBox_2.addItem("")
+        self.comboBox_2.addItem("")
+        self.comboBox_2.addItem("")
+        self.comboBox_2.addItem("")
+        self.comboBox_2.addItem("")
+        self.comboBox_2.addItem("")
+        self.comboBox_2.addItem("")
+        self.comboBox_2.addItem("")
+        self.comboBox_2.addItem("")
+        self.comboBox_2.setObjectName(u"comboBox_2")
+
+        self.horizontalLayout_8.addWidget(self.comboBox_2)
+
+
+        self.verticalLayout_2.addLayout(self.horizontalLayout_8)
+
+        self.verticalLayout_2.setStretch(0, 9)
+
+        self.horizontalLayout_9.addLayout(self.verticalLayout_2)
+
+        self.verticalLayout_3 = QVBoxLayout()
+        self.verticalLayout_3.setObjectName(u"verticalLayout_3")
+        self.verticalLayout_3.setContentsMargins(-1, -1, -1, 0)
+        self.horizontalLayout_2 = QHBoxLayout()
+        self.horizontalLayout_2.setObjectName(u"horizontalLayout_2")
+        self.horizontalSpacer = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+
+        self.horizontalLayout_2.addItem(self.horizontalSpacer)
+
         self.label = QLabel(self.centralwidget)
         self.label.setObjectName(u"label")
-        self.label.setGeometry(QRect(490, 20, 101, 21))
+        self.label.setMinimumSize(QSize(110, 0))
+        self.label.setMaximumSize(QSize(120, 16777215))
+
+        self.horizontalLayout_2.addWidget(self.label)
+
+        self.lineEdit = QLineEdit(self.centralwidget)
+        self.lineEdit.setObjectName(u"lineEdit")
+
+        self.horizontalLayout_2.addWidget(self.lineEdit)
+
+        self.label_4 = QLabel(self.centralwidget)
+        self.label_4.setObjectName(u"label_4")
+        self.label_4.setMinimumSize(QSize(20, 0))
+
+        self.horizontalLayout_2.addWidget(self.label_4)
+
+
+        self.verticalLayout_3.addLayout(self.horizontalLayout_2)
+
+        self.horizontalLayout_3 = QHBoxLayout()
+        self.horizontalLayout_3.setObjectName(u"horizontalLayout_3")
+        self.horizontalSpacer_2 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+
+        self.horizontalLayout_3.addItem(self.horizontalSpacer_2)
+
         self.label_2 = QLabel(self.centralwidget)
         self.label_2.setObjectName(u"label_2")
-        self.label_2.setGeometry(QRect(490, 50, 101, 21))
+        self.label_2.setMinimumSize(QSize(110, 0))
+        self.label_2.setMaximumSize(QSize(120, 16777215))
+
+        self.horizontalLayout_3.addWidget(self.label_2)
+
+        self.lineEdit_2 = QLineEdit(self.centralwidget)
+        self.lineEdit_2.setObjectName(u"lineEdit_2")
+
+        self.horizontalLayout_3.addWidget(self.lineEdit_2)
+
+        self.label_3 = QLabel(self.centralwidget)
+        self.label_3.setObjectName(u"label_3")
+        self.label_3.setMinimumSize(QSize(20, 0))
+
+        self.horizontalLayout_3.addWidget(self.label_3)
+
+
+        self.verticalLayout_3.addLayout(self.horizontalLayout_3)
+
+        self.horizontalLayout_4 = QHBoxLayout()
+        self.horizontalLayout_4.setObjectName(u"horizontalLayout_4")
+        self.radioButton = QRadioButton(self.centralwidget)
+        self.radioButton.setObjectName(u"radioButton")
+        self.radioButton.setChecked(True)
+
+        self.horizontalLayout_4.addWidget(self.radioButton)
+
+        self.radioButton_2 = QRadioButton(self.centralwidget)
+        self.radioButton_2.setObjectName(u"radioButton_2")
+
+        self.horizontalLayout_4.addWidget(self.radioButton_2)
+
+        self.radioButton_3 = QRadioButton(self.centralwidget)
+        self.radioButton_3.setObjectName(u"radioButton_3")
+
+        self.horizontalLayout_4.addWidget(self.radioButton_3)
+
+
+        self.verticalLayout_3.addLayout(self.horizontalLayout_4)
+
+        self.horizontalLayout_5 = QHBoxLayout()
+        self.horizontalLayout_5.setObjectName(u"horizontalLayout_5")
+        self.label_7 = QLabel(self.centralwidget)
+        self.label_7.setObjectName(u"label_7")
+
+        self.horizontalLayout_5.addWidget(self.label_7)
+
+        self.horizontalSpacer_3 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+
+        self.horizontalLayout_5.addItem(self.horizontalSpacer_3)
+
+
+        self.verticalLayout_3.addLayout(self.horizontalLayout_5)
+
+        self.horizontalLayout_6 = QHBoxLayout()
+        self.horizontalLayout_6.setSpacing(2)
+        self.horizontalLayout_6.setObjectName(u"horizontalLayout_6")
+        self.label_5 = QLabel(self.centralwidget)
+        self.label_5.setObjectName(u"label_5")
+
+        self.horizontalLayout_6.addWidget(self.label_5)
+
+        self.lineEdit_3 = QLineEdit(self.centralwidget)
+        self.lineEdit_3.setObjectName(u"lineEdit_3")
+
+        self.horizontalLayout_6.addWidget(self.lineEdit_3)
+
+        self.label_6 = QLabel(self.centralwidget)
+        self.label_6.setObjectName(u"label_6")
+
+        self.horizontalLayout_6.addWidget(self.label_6)
+
         self.label_9 = QLabel(self.centralwidget)
         self.label_9.setObjectName(u"label_9")
-        self.label_9.setGeometry(QRect(600, 170, 21, 21))
+
+        self.horizontalLayout_6.addWidget(self.label_9)
+
+        self.lineEdit_4 = QLineEdit(self.centralwidget)
+        self.lineEdit_4.setObjectName(u"lineEdit_4")
+
+        self.horizontalLayout_6.addWidget(self.lineEdit_4)
+
+        self.label_8 = QLabel(self.centralwidget)
+        self.label_8.setObjectName(u"label_8")
+
+        self.horizontalLayout_6.addWidget(self.label_8)
+
+        self.label_10 = QLabel(self.centralwidget)
+        self.label_10.setObjectName(u"label_10")
+
+        self.horizontalLayout_6.addWidget(self.label_10)
+
+        self.comboBox = QComboBox(self.centralwidget)
+        self.comboBox.setObjectName(u"comboBox")
+
+        self.horizontalLayout_6.addWidget(self.comboBox)
+
+        self.label_11 = QLabel(self.centralwidget)
+        self.label_11.setObjectName(u"label_11")
+
+        self.horizontalLayout_6.addWidget(self.label_11)
+
+
+        self.verticalLayout_3.addLayout(self.horizontalLayout_6)
+
         self.tableWidget = QTableWidget(self.centralwidget)
         if (self.tableWidget.columnCount() < 2):
             self.tableWidget.setColumnCount(2)
         __qtablewidgetitem = QTableWidgetItem()
         self.tableWidget.setHorizontalHeaderItem(0, __qtablewidgetitem)
         __qtablewidgetitem1 = QTableWidgetItem()
         self.tableWidget.setHorizontalHeaderItem(1, __qtablewidgetitem1)
@@ -88,112 +260,104 @@
         __qtablewidgetitem16 = QTableWidgetItem()
         __qtablewidgetitem16.setFlags(Qt.ItemIsSelectable|Qt.ItemIsDragEnabled|Qt.ItemIsDropEnabled|Qt.ItemIsUserCheckable|Qt.ItemIsEnabled);
         self.tableWidget.setItem(6, 1, __qtablewidgetitem16)
         __qtablewidgetitem17 = QTableWidgetItem()
         __qtablewidgetitem17.setFlags(Qt.ItemIsSelectable|Qt.ItemIsDragEnabled|Qt.ItemIsDropEnabled|Qt.ItemIsUserCheckable|Qt.ItemIsEnabled);
         self.tableWidget.setItem(7, 1, __qtablewidgetitem17)
         self.tableWidget.setObjectName(u"tableWidget")
-        self.tableWidget.setGeometry(QRect(500, 200, 311, 271))
-        self.label_5 = QLabel(self.centralwidget)
-        self.label_5.setObjectName(u"label_5")
-        self.label_5.setGeometry(QRect(490, 170, 41, 21))
-        self.label_4 = QLabel(self.centralwidget)
-        self.label_4.setObjectName(u"label_4")
-        self.label_4.setGeometry(QRect(720, 20, 51, 20))
-        self.lineEdit_3 = QLineEdit(self.centralwidget)
-        self.lineEdit_3.setObjectName(u"lineEdit_3")
-        self.lineEdit_3.setGeometry(QRect(530, 170, 41, 24))
-        self.horizontalLayoutWidget = QWidget(self.centralwidget)
-        self.horizontalLayoutWidget.setObjectName(u"horizontalLayoutWidget")
-        self.horizontalLayoutWidget.setGeometry(QRect(10, 10, 471, 421))
-        self.horizontalLayout = QHBoxLayout(self.horizontalLayoutWidget)
-        self.horizontalLayout.setObjectName(u"horizontalLayout")
-        self.horizontalLayout.setContentsMargins(0, 0, 0, 0)
-        self.label_8 = QLabel(self.centralwidget)
-        self.label_8.setObjectName(u"label_8")
-        self.label_8.setGeometry(QRect(670, 170, 51, 21))
-        self.lineEdit = QLineEdit(self.centralwidget)
-        self.lineEdit.setObjectName(u"lineEdit")
-        self.lineEdit.setGeometry(QRect(600, 20, 113, 24))
-        self.label_6 = QLabel(self.centralwidget)
-        self.label_6.setObjectName(u"label_6")
-        self.label_6.setGeometry(QRect(580, 170, 16, 21))
+        self.tableWidget.setMinimumSize(QSize(0, 270))
+        self.tableWidget.setMaximumSize(QSize(320, 16777215))
+
+        self.verticalLayout_3.addWidget(self.tableWidget)
+
+        self.horizontalLayout_7 = QHBoxLayout()
+        self.horizontalLayout_7.setObjectName(u"horizontalLayout_7")
+        self.horizontalSpacer_4 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+
+        self.horizontalLayout_7.addItem(self.horizontalSpacer_4)
+
+        self.verticalLayout = QVBoxLayout()
+        self.verticalLayout.setSpacing(1)
+        self.verticalLayout.setObjectName(u"verticalLayout")
+        self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+
+        self.verticalLayout.addItem(self.verticalSpacer)
+
         self.pushButton = QPushButton(self.centralwidget)
         self.pushButton.setObjectName(u"pushButton")
         self.pushButton.setEnabled(True)
-        self.pushButton.setGeometry(QRect(700, 480, 80, 24))
-        self.lineEdit_4 = QLineEdit(self.centralwidget)
-        self.lineEdit_4.setObjectName(u"lineEdit_4")
-        self.lineEdit_4.setGeometry(QRect(620, 170, 41, 24))
-        self.label_7 = QLabel(self.centralwidget)
-        self.label_7.setObjectName(u"label_7")
-        self.label_7.setGeometry(QRect(490, 150, 121, 16))
-        self.comboBox = QComboBox(self.centralwidget)
-        self.comboBox.setObjectName(u"comboBox")
-        self.comboBox.setGeometry(QRect(720, 170, 61, 24))
-        self.label_10 = QLabel(self.centralwidget)
-        self.label_10.setObjectName(u"label_10")
-        self.label_10.setGeometry(QRect(700, 170, 21, 21))
-        self.label_11 = QLabel(self.centralwidget)
-        self.label_11.setObjectName(u"label_11")
-        self.label_11.setGeometry(QRect(790, 170, 21, 21))
-        self.comboBox_2 = QComboBox(self.centralwidget)
-        self.comboBox_2.addItem("")
-        self.comboBox_2.addItem("")
-        self.comboBox_2.addItem("")
-        self.comboBox_2.addItem("")
-        self.comboBox_2.addItem("")
-        self.comboBox_2.addItem("")
-        self.comboBox_2.addItem("")
-        self.comboBox_2.addItem("")
-        self.comboBox_2.addItem("")
-        self.comboBox_2.addItem("")
-        self.comboBox_2.addItem("")
-        self.comboBox_2.setObjectName(u"comboBox_2")
-        self.comboBox_2.setGeometry(QRect(350, 440, 131, 24))
-        self.label_12 = QLabel(self.centralwidget)
-        self.label_12.setObjectName(u"label_12")
-        self.label_12.setGeometry(QRect(258, 440, 91, 21))
+
+        self.verticalLayout.addWidget(self.pushButton)
+
         self.progress = QProgressBar(self.centralwidget)
         self.progress.setObjectName(u"progress")
-        self.progress.setGeometry(QRect(700, 500, 81, 16))
+        self.progress.setMaximumSize(QSize(16777215, 2))
         self.progress.setValue(0)
         self.progress.setTextVisible(False)
         self.progress.setInvertedAppearance(False)
-        self.radioButton = QRadioButton(self.centralwidget)
-        self.radioButton.setObjectName(u"radioButton")
-        self.radioButton.setGeometry(QRect(490, 90, 91, 22))
-        self.radioButton.setChecked(True)
-        self.radioButton_2 = QRadioButton(self.centralwidget)
-        self.radioButton_2.setObjectName(u"radioButton_2")
-        self.radioButton_2.setGeometry(QRect(550, 90, 141, 22))
-        self.radioButton_3 = QRadioButton(self.centralwidget)
-        self.radioButton_3.setObjectName(u"radioButton_3")
-        self.radioButton_3.setGeometry(QRect(690, 90, 121, 22))
+
+        self.verticalLayout.addWidget(self.progress)
+
+
+        self.horizontalLayout_7.addLayout(self.verticalLayout)
+
+
+        self.verticalLayout_3.addLayout(self.horizontalLayout_7)
+
+
+        self.horizontalLayout_9.addLayout(self.verticalLayout_3)
+
+        self.horizontalLayout_9.setStretch(0, 9)
         MainWindow.setCentralWidget(self.centralwidget)
         self.menubar = QMenuBar(MainWindow)
         self.menubar.setObjectName(u"menubar")
-        self.menubar.setGeometry(QRect(0, 0, 818, 21))
+        self.menubar.setGeometry(QRect(0, 0, 808, 21))
         MainWindow.setMenuBar(self.menubar)
         self.statusbar = QStatusBar(MainWindow)
         self.statusbar.setObjectName(u"statusbar")
         MainWindow.setStatusBar(self.statusbar)
 
         self.retranslateUi(MainWindow)
 
         QMetaObject.connectSlotsByName(MainWindow)
     # setupUi
 
     def retranslateUi(self, MainWindow):
         MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"debyetools GUI (lite) - Heat Capacity", None))
-        self.label_3.setText(QCoreApplication.translate("MainWindow", u"GPa", None))
-        self.lineEdit_2.setText(QCoreApplication.translate("MainWindow", u"0 30 10", None))
+        self.label_12.setText(QCoreApplication.translate("MainWindow", u"                                                                                           property to plot:", None))
+        self.comboBox_2.setItemText(0, QCoreApplication.translate("MainWindow", u"New Item", None))
+        self.comboBox_2.setItemText(1, QCoreApplication.translate("MainWindow", u"New Item", None))
+        self.comboBox_2.setItemText(2, QCoreApplication.translate("MainWindow", u"New Item", None))
+        self.comboBox_2.setItemText(3, QCoreApplication.translate("MainWindow", u"New Item", None))
+        self.comboBox_2.setItemText(4, QCoreApplication.translate("MainWindow", u"New Item", None))
+        self.comboBox_2.setItemText(5, QCoreApplication.translate("MainWindow", u"New Item", None))
+        self.comboBox_2.setItemText(6, QCoreApplication.translate("MainWindow", u"New Item", None))
+        self.comboBox_2.setItemText(7, QCoreApplication.translate("MainWindow", u"New Item", None))
+        self.comboBox_2.setItemText(8, QCoreApplication.translate("MainWindow", u"New Item", None))
+        self.comboBox_2.setItemText(9, QCoreApplication.translate("MainWindow", u"New Item", None))
+        self.comboBox_2.setItemText(10, QCoreApplication.translate("MainWindow", u"New Item", None))
+
         self.label.setText(QCoreApplication.translate("MainWindow", u"Temperature range:", None))
+        self.lineEdit.setText(QCoreApplication.translate("MainWindow", u"0.1 1000.1 100", None))
+        self.label_4.setText(QCoreApplication.translate("MainWindow", u"K", None))
         self.label_2.setText(QCoreApplication.translate("MainWindow", u"Pressure:", None))
-        self.label_9.setText(QCoreApplication.translate("MainWindow", u"to:", None))
+        self.lineEdit_2.setText(QCoreApplication.translate("MainWindow", u"0 30 10", None))
+        self.label_3.setText(QCoreApplication.translate("MainWindow", u"GPa", None))
+        self.radioButton.setText(QCoreApplication.translate("MainWindow", u"Slater", None))
+        self.radioButton_2.setText(QCoreApplication.translate("MainWindow", u"Dugdale-MacDonald", None))
+        self.radioButton_3.setText(QCoreApplication.translate("MainWindow", u"mean-free-volume", None))
+        self.label_7.setText(QCoreApplication.translate("MainWindow", u"FactSage parameters:", None))
+        self.label_5.setText(QCoreApplication.translate("MainWindow", u"From:", None))
+        self.lineEdit_3.setText(QCoreApplication.translate("MainWindow", u"298.15", None))
+        self.label_6.setText(QCoreApplication.translate("MainWindow", u"K", None))
+        self.label_9.setText(QCoreApplication.translate("MainWindow", u"   to:", None))
+        self.lineEdit_4.setText(QCoreApplication.translate("MainWindow", u"1000.1", None))
+        self.label_8.setText(QCoreApplication.translate("MainWindow", u"K", None))
+        self.label_10.setText(QCoreApplication.translate("MainWindow", u"    P:", None))
+        self.label_11.setText(QCoreApplication.translate("MainWindow", u"GPa", None))
         ___qtablewidgetitem = self.tableWidget.horizontalHeaderItem(0)
         ___qtablewidgetitem.setText(QCoreApplication.translate("MainWindow", u"Values", None));
         ___qtablewidgetitem1 = self.tableWidget.verticalHeaderItem(0)
         ___qtablewidgetitem1.setText(QCoreApplication.translate("MainWindow", u"G+TS (T=298.15)", None));
         ___qtablewidgetitem2 = self.tableWidget.verticalHeaderItem(1)
         ___qtablewidgetitem2.setText(QCoreApplication.translate("MainWindow", u"S (T=298.15)", None));
         ___qtablewidgetitem3 = self.tableWidget.verticalHeaderItem(2)
@@ -225,36 +389,10 @@
         ___qtablewidgetitem14.setText(QCoreApplication.translate("MainWindow", u"T^(2)", None));
         ___qtablewidgetitem15 = self.tableWidget.item(6, 1)
         ___qtablewidgetitem15.setText(QCoreApplication.translate("MainWindow", u"T^(-0.5)", None));
         ___qtablewidgetitem16 = self.tableWidget.item(7, 1)
         ___qtablewidgetitem16.setText(QCoreApplication.translate("MainWindow", u"T^(-3)", None));
         self.tableWidget.setSortingEnabled(__sortingEnabled)
 
-        self.label_5.setText(QCoreApplication.translate("MainWindow", u"From:", None))
-        self.label_4.setText(QCoreApplication.translate("MainWindow", u"K", None))
-        self.lineEdit_3.setText(QCoreApplication.translate("MainWindow", u"298.15", None))
-        self.label_8.setText(QCoreApplication.translate("MainWindow", u"K", None))
-        self.lineEdit.setText(QCoreApplication.translate("MainWindow", u"0.1 1000.1 100", None))
-        self.label_6.setText(QCoreApplication.translate("MainWindow", u"K", None))
         self.pushButton.setText(QCoreApplication.translate("MainWindow", u"re-calculate", None))
-        self.lineEdit_4.setText(QCoreApplication.translate("MainWindow", u"1000.1", None))
-        self.label_7.setText(QCoreApplication.translate("MainWindow", u"FactSage parameters:", None))
-        self.label_10.setText(QCoreApplication.translate("MainWindow", u"P:", None))
-        self.label_11.setText(QCoreApplication.translate("MainWindow", u"GPa", None))
-        self.comboBox_2.setItemText(0, QCoreApplication.translate("MainWindow", u"New Item", None))
-        self.comboBox_2.setItemText(1, QCoreApplication.translate("MainWindow", u"New Item", None))
-        self.comboBox_2.setItemText(2, QCoreApplication.translate("MainWindow", u"New Item", None))
-        self.comboBox_2.setItemText(3, QCoreApplication.translate("MainWindow", u"New Item", None))
-        self.comboBox_2.setItemText(4, QCoreApplication.translate("MainWindow", u"New Item", None))
-        self.comboBox_2.setItemText(5, QCoreApplication.translate("MainWindow", u"New Item", None))
-        self.comboBox_2.setItemText(6, QCoreApplication.translate("MainWindow", u"New Item", None))
-        self.comboBox_2.setItemText(7, QCoreApplication.translate("MainWindow", u"New Item", None))
-        self.comboBox_2.setItemText(8, QCoreApplication.translate("MainWindow", u"New Item", None))
-        self.comboBox_2.setItemText(9, QCoreApplication.translate("MainWindow", u"New Item", None))
-        self.comboBox_2.setItemText(10, QCoreApplication.translate("MainWindow", u"New Item", None))
-
-        self.label_12.setText(QCoreApplication.translate("MainWindow", u"property to plot:", None))
-        self.radioButton.setText(QCoreApplication.translate("MainWindow", u"Slater", None))
-        self.radioButton_2.setText(QCoreApplication.translate("MainWindow", u"Dugdale-MacDonald", None))
-        self.radioButton_3.setText(QCoreApplication.translate("MainWindow", u"mean-free-volume", None))
     # retranslateUi
```

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/ui_interatomic_params.py` & `debyetools-2.1/debyetools/tpropsgui/ui_interatomic_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'interatomic_params.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.4.2
+## Created by: Qt User Interface Compiler version 6.6.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
@@ -55,14 +55,15 @@
         self.plainTextEdit.setFrameShape(QFrame.Box)
         self.plainTextEdit.setTabChangesFocus(False)
         self.plainTextEdit.setReadOnly(True)
         self.plainTextEdit.setBackgroundVisible(False)
         self.plainTextEdit.setCenterOnScroll(False)
         self.OKbutton = QPushButton(Form)
         self.OKbutton.setObjectName(u"OKbutton")
+        self.OKbutton.setEnabled(False)
         self.OKbutton.setGeometry(QRect(680, 340, 80, 24))
         self.pushButton = QPushButton(Form)
         self.pushButton.setObjectName(u"pushButton")
         self.pushButton.setGeometry(QRect(590, 340, 71, 24))
         self.label = QLabel(Form)
         self.label.setObjectName(u"label")
         self.label.setGeometry(QRect(10, 10, 31, 16))
```

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/ui_missingkey.py` & `debyetools-2.1/debyetools/tpropsgui/ui_missingkey.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/ui_warning.py` & `debyetools-2.1/debyetools/tpropsgui/ui_warning.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/window_cp.py` & `debyetools-2.1/debyetools/tpropsgui/window_cp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from PySide6.QtWidgets import QMainWindow, QTableWidgetItem, QMenu
 from PySide6.QtCore import Qt
 
 from debyetools.tpropsgui.ui_heatcapacitywindow import Ui_MainWindow as Ui_Cp
 
 from debyetools.fs_compound_db import fit_FS as dt_fit_FS
+from debyetools.tpropsgui.atomtools import atom_energy
 #from debyetools.fs_compound_db import Cp2fit as dt_Cp2fit
 
 # from  debyetools.tpropsgui.backend_qt_patched.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 # from matplotlib.backends.backend_qt5agg import FigureCanvasAgg as FigureCanvas
 # from matplotlib.backends.backend_mixed import FigureCanvas
 # print(hola)
@@ -20,15 +21,15 @@
 import numpy as np
 
 class windowCp(QMainWindow):
     def __init__(self, parent=None):
         super().__init__(parent)
         self.ui = Ui_Cp()
         self.ui.setupUi(self)
-        # self.app = app
+#        self.app = app
 
         self.fig = Figure(figsize=(3, 3))
         self.canvas = FigureCanvas(self.fig)
         self.set_canvas_configuration()
 
         llayout = self.ui.horizontalLayout#QHBoxLayout()
         llayout.addWidget(self.canvas, 88)
@@ -110,15 +111,17 @@
 
         self._ax.set_xlabel(str_x)
         self._ax.set_ylabel(str_y)
 
         self.canvas.draw()
 
 
-    def debye_run(self, molecule, ui_progress):
+    def debye_run(self, molecule, ui_progress, formula):
+        self.formula=formula
+        txt4output = f'{formula}$'
         if self.ui.radioButton.isChecked():
             mode ='jjsl'
         elif self.ui.radioButton_2.isChecked():
             mode = 'jjdm'
         elif self.ui.radioButton_3.isChecked():
             mode = 'jjfv'
         self.ui.comboBox.clear()
@@ -160,20 +163,36 @@
 
             ix_T0 = np.where(np.round(molecule.tprops_dict['T'],2) == np.round(298.15,2))[0][0]
 
             self.dict_H298['%.1f'%(P/1e9)] = molecule.tprops_dict['G'][ix_T0]+molecule.tprops_dict['T'][ix_T0]*molecule.tprops_dict['S'][ix_T0]
             self.dict_S298['%.1f'%(P/1e9)] = molecule.tprops_dict['S'][ix_T0]
 
 #            self.plot_Cp(self.dict_tp['%.1f'%(P/1e9)], self.dict_FS['%.1f'%(P/1e9)])
+            nats = len(molecule.types)
+            if P==0:
+                # print(molecule.__dict__.keys())
+                Ef = molecule.eos.E0(molecule.eos.V0)-sum([atom_energy[ti] for ti in molecule.types])*(0.160218e-18 * 6.02214e23)/len(molecule.types)
+                txt4output += f'{Ef*nats:.7e}'
+
+        txt4output += f'${self.dict_S298['%.1f'%(0/1e9)]*nats:.7e}$'
 
         self.ui.tableWidget.setItem(0,0,QTableWidgetItem('%.5e' % (self.dict_H298['%.1f'%(0/1e9)])))
         self.ui.tableWidget.setItem(1,0,QTableWidgetItem('%.5e' % (self.dict_S298['%.1f'%(0/1e9)])))
+
+        lst4output = []
         for ix, p in enumerate(self.dict_FS['%.1f'%(0/1e9)]['Cp']):
+            lst4output.append(f'{p*nats:.7e}')
             self.ui.tableWidget.setItem(ix+2,0,QTableWidgetItem('%.5e' % (p)))
+        txt4output += '&'.join(lst4output)
+        txt4output += '$'
+        t4out = [f'{p:.2e}' for p in [self.FS_Tfrom, self.FS_Tto]]
+        txt4output += '&'.join(t4out)
 
+        with open('dtoutput4cmpnd', 'w') as f:
+            f.write(txt4output)
 #            self._ax.text(Y[-1],X[-1],'P=')
 
 
 #        print('xxxx', list(self.dict_tp[list(self.dict_tp.keys())[0]].keys()))
         self.proplist = list(self.dict_tp[list(self.dict_tp.keys())[0]].keys())
         current_plot = self.current_plot
         self.ui.comboBox_2.clear()
@@ -225,15 +244,16 @@
         clipboard=self.app.clipboard()
         clipboard.setText(txt2copy)
 
 
 
     def on_click_recalc(self):
         self._ax.cla()
-        self.debye_run(self.molecule, self.ui.progress)
+        self.debye_run(self.molecule, self.ui.progress, self.formula)
 
     def update_FS_Tto(self):
         try:
             Tf =self.get_T()[-1]
             self.ui.lineEdit_4.setText(str(Tf))
         except:
             pass
+
```

### Comparing `debyetools-2.0.6/debyetools/tpropsgui/window_interatomicparams.py` & `debyetools-2.1/debyetools/tpropsgui/window_interatomicparams.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools/vibrational.py` & `debyetools-2.1/debyetools/vibrational.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.6/debyetools.egg-info/PKG-INFO` & `debyetools-2.1/debyetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debyetools
-Version: 2.0.6
+Version: 2.1
 Summary: Debye approximation implementation for the calculation of thermodynamic properties from ground-state atomistic simulations.
 Home-page: https://debyetools.readthedocs.io/
 Author: Javier Jofre
 Author-email: javier.jofre@polymtl.ca
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `debyetools-2.0.6/debyetools.egg-info/SOURCES.txt` & `debyetools-2.1/debyetools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -137,16 +137,18 @@
 debyetools/examples/Al_fcc/DOSCAR.EvV.0.08
 debyetools/examples/Al_fcc/DOSCAR.EvV.0.09
 debyetools/examples/Al_fcc/DOSCAR.EvV.0.1
 debyetools/examples/Al_fcc/OUTCAR.eps
 debyetools/examples/Al_fcc/SUMMARY.fcc
 debyetools/tpropsgui/__init__.py
 debyetools/tpropsgui/atomtools.py
+debyetools/tpropsgui/custom_widgets.py
 debyetools/tpropsgui/dialog_doscar.py
 debyetools/tpropsgui/dialog_outcar.py
+debyetools/tpropsgui/dialog_periodictable.py
 debyetools/tpropsgui/dialog_summary.py
 debyetools/tpropsgui/dialog_warning.py
 debyetools/tpropsgui/elements.py
 debyetools/tpropsgui/events.py
 debyetools/tpropsgui/functions0.py
 debyetools/tpropsgui/get_functions.py
 debyetools/tpropsgui/gui.py
@@ -157,14 +159,15 @@
 debyetools/tpropsgui/plot_EV.py
 debyetools/tpropsgui/plotter.py
 debyetools/tpropsgui/plotter_class.py
 debyetools/tpropsgui/toolbox.py
 debyetools/tpropsgui/ui_dialogSUMMARY.py
 debyetools/tpropsgui/ui_dialog_doscar.py
 debyetools/tpropsgui/ui_dialog_outcar.py
+debyetools/tpropsgui/ui_dialog_periodictable.py
 debyetools/tpropsgui/ui_heatcapacitywindow.py
 debyetools/tpropsgui/ui_interatomic_params.py
 debyetools/tpropsgui/ui_mainwindow.py
 debyetools/tpropsgui/ui_missingkey.py
 debyetools/tpropsgui/ui_warning.py
 debyetools/tpropsgui/window_cp.py
 debyetools/tpropsgui/window_interatomicparams.py
```

### Comparing `debyetools-2.0.6/setup.py` & `debyetools-2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="debyetools",
-    version="2.0.6",
+    version="2.1",
     description="Debye approximation implementation for the calculation of thermodynamic properties from ground-state atomistic simulations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://debyetools.readthedocs.io/",
     author="Javier Jofre",
     author_email="javier.jofre@polymtl.ca",
     license="GPLv3",
```

