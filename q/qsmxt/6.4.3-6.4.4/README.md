# Comparing `tmp/qsmxt-6.4.3.tar.gz` & `tmp/qsmxt-6.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsmxt-6.4.3.tar", last modified: Wed Mar 27 07:01:41 2024, max compression
+gzip compressed data, was "qsmxt-6.4.4.tar", last modified: Tue May 14 03:33:32 2024, max compression
```

## Comparing `qsmxt-6.4.3.tar` & `qsmxt-6.4.4.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:41.385942 qsmxt-6.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-27 07:01:36.000000 qsmxt-6.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-27 07:01:36.000000 qsmxt-6.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-27 07:01:41.385942 qsmxt-6.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-27 07:01:36.000000 qsmxt-6.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:41.373942 qsmxt-6.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-03-27 07:01:36.000000 qsmxt-6.4.3/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:41.373942 qsmxt-6.4.3/qsmxt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34803 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/aseg_labels.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:41.377941 qsmxt-6.4.3/qsmxt/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    41949 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/cli/dicom_convert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9738 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/cli/dicom_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    74606 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/cli/main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14260 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/cli/nifti_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:41.381941 qsmxt-6.4.3/qsmxt/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1944 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_addtojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_analyse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_axialsampling.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_bet2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_clearswi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_combinemagnitude.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1625 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_erode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_fastsurfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_hdbet.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_laplacian_unwrapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_makehomogeneous.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10740 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_masking.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1553 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_mgz2nii.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_nextqsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_nii2dcm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2588 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_nonzeroaverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_phaseweights.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6379 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_processphase.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2599 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_qsm_referencing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8286 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_qsmjl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2719 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_resample_like.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4630 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_romeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_t2star_r2star.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_tgv_qsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_tgv_qsm_jl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2240 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_twopass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/interfaces/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/qsm_pipelines.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:41.385942 qsmxt-6.4.3/qsmxt/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/antsBuildTemplate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      699 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/hagberg_pb_masking.jl
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/makehomogeneous.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1736 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/mrt_clearswi.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/mrt_laplacian_unwrapping.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)      807 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/mrt_phase_weights.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1367 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/mrt_t2star_r2star.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)     5257 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/nii_fix_ge.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2187 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/qsmjl_full.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1109 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/qsmjl_laplacian_unwrapping.jl
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/qsmjl_medi.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/qsmjl_pdf.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1138 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/qsmjl_phase_to_frequency.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1186 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/qsmjl_rts.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1342 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/qsmjl_tv.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1387 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/qsmjl_vsharp.jl
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/qsmxt_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      632 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/qsmxt_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1473 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/resample_like.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/romeo_unwrapping.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)     2698 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/romeo_voxelquality.jl
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/sys_cmd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2522 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/tgv_qsm.jl
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/scripts/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:41.385942 qsmxt-6.4.3/qsmxt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12011 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/tests/setup_qsmxt.sh
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/tests/testInstanceSetup.sh
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/tests/test_hashes_qsm.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    15913 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/tests/test_qsm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4933 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/tests/test_segmentation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3877 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/tests/test_template.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      837 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/tests/test_transparent_singularity.sh
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:41.385942 qsmxt-6.4.3/qsmxt/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/workflows/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    54852 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/workflows/qsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-03-27 07:01:36.000000 qsmxt-6.4.3/qsmxt/workflows/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 07:01:41.385942 qsmxt-6.4.3/qsmxt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-27 07:01:41.000000 qsmxt-6.4.3/qsmxt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-03-27 07:01:41.000000 qsmxt-6.4.3/qsmxt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 07:01:41.000000 qsmxt-6.4.3/qsmxt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-27 07:01:41.000000 qsmxt-6.4.3/qsmxt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-27 07:01:41.000000 qsmxt-6.4.3/qsmxt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 07:01:41.000000 qsmxt-6.4.3/qsmxt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 07:01:41.385942 qsmxt-6.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-27 07:01:36.000000 qsmxt-6.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:32.719054 qsmxt-6.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 03:33:23.000000 qsmxt-6.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 03:33:23.000000 qsmxt-6.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-14 03:33:32.719054 qsmxt-6.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 03:33:23.000000 qsmxt-6.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:32.703054 qsmxt-6.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-14 03:33:23.000000 qsmxt-6.4.4/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:32.707054 qsmxt-6.4.4/qsmxt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34803 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/aseg_labels.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:32.707054 qsmxt-6.4.4/qsmxt/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41949 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/cli/dicom_convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9738 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/cli/dicom_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77738 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/cli/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14260 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/cli/nifti_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:32.711054 qsmxt-6.4.4/qsmxt/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1944 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_addtojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_axialsampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_bet2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_clearswi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_combinemagnitude.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1625 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_erode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_fastsurfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_hdbet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_laplacian_unwrapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_makehomogeneous.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10740 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_masking.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1553 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_mgz2nii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_nextqsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_nii2dcm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2588 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_nonzeroaverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_phaseweights.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6379 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_processphase.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2599 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_qsm_referencing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8286 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_qsmjl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2719 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_resample_like.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6269 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_romeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_t2star_r2star.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_tgv_qsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_tgv_qsm_jl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2240 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_twopass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/interfaces/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/qsm_pipelines.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:32.715054 qsmxt-6.4.4/qsmxt/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/antsBuildTemplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      699 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/hagberg_pb_masking.jl
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/makehomogeneous.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1736 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/mrt_clearswi.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/mrt_laplacian_unwrapping.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      807 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/mrt_phase_weights.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1367 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/mrt_t2star_r2star.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5257 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/nii_fix_ge.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2187 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/qsmjl_full.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1109 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/qsmjl_laplacian_unwrapping.jl
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/qsmjl_medi.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/qsmjl_pdf.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1138 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/qsmjl_phase_to_frequency.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1186 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/qsmjl_rts.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1342 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/qsmjl_tv.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1387 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/qsmjl_vsharp.jl
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/qsmxt_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      632 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/qsmxt_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1473 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/resample_like.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/romeo_unwrapping.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2698 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/romeo_voxelquality.jl
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/sys_cmd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2522 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/tgv_qsm.jl
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/scripts/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:32.719054 qsmxt-6.4.4/qsmxt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12014 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/tests/setup_qsmxt.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/tests/testInstanceSetup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/tests/test_hashes_qsm.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15913 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/tests/test_qsm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4933 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/tests/test_segmentation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3877 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/tests/test_template.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      837 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/tests/test_transparent_singularity.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:32.719054 qsmxt-6.4.4/qsmxt/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/workflows/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56833 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/workflows/qsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-05-14 03:33:23.000000 qsmxt-6.4.4/qsmxt/workflows/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:33:32.719054 qsmxt-6.4.4/qsmxt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-14 03:33:32.000000 qsmxt-6.4.4/qsmxt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-14 03:33:32.000000 qsmxt-6.4.4/qsmxt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 03:33:32.000000 qsmxt-6.4.4/qsmxt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-14 03:33:32.000000 qsmxt-6.4.4/qsmxt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 03:33:32.000000 qsmxt-6.4.4/qsmxt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 03:33:32.000000 qsmxt-6.4.4/qsmxt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 03:33:32.719054 qsmxt-6.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-14 03:33:23.000000 qsmxt-6.4.4/setup.py
```

### Comparing `qsmxt-6.4.3/LICENSE` & `qsmxt-6.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/PKG-INFO` & `qsmxt-6.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsmxt
-Version: 6.4.3
+Version: 6.4.4
 License-File: LICENSE
 Requires-Dist: psutil
 Requires-Dist: datetime
 Requires-Dist: networkx==2.8.8
 Requires-Dist: numpy
 Requires-Dist: h5py
 Requires-Dist: nibabel
```

### Comparing `qsmxt-6.4.3/docs/_config.yml` & `qsmxt-6.4.4/docs/_config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # PIP VERSION NUMBER FOR TESTING
-TEST_PACKAGE_VERSION: 6.4.3
+TEST_PACKAGE_VERSION: 6.4.4
 
 # PIP VERSION NUMBER FOR RELEASE
-DEPLOY_PACKAGE_VERSION: 6.4.3
+DEPLOY_PACKAGE_VERSION: 6.4.4
 
 # CONTAINER VERSION FOR TESTING ONCE BUILT
-TEST_CONTAINER_VERSION: 6.4.2
-TEST_CONTAINER_DATE: 20240315
+TEST_CONTAINER_VERSION: 6.4.3
+TEST_CONTAINER_DATE: 20240327
 
 # CONTAINER VERSION FOR PRODUCTION ONCE TESTED
-PROD_PACKAGE_VERSION: 6.4.2
-PROD_CONTAINER_VERSION: 6.4.2
-PROD_CONTAINER_DATE: 20240315
+PROD_PACKAGE_VERSION: 6.4.3
+PROD_CONTAINER_VERSION: 6.4.3
+PROD_CONTAINER_DATE: 20240327
 PROD_MINICONDA_PATH: ~/miniconda3
 
 remote_theme: just-the-docs/just-the-docs
 baseurl: "/QSMxT" # the subpath of your site, e.g. /blog
 repository: QSMxT/QSMxT
 
 permalink: pretty
```

### Comparing `qsmxt-6.4.3/qsmxt/aseg_labels.csv` & `qsmxt-6.4.4/qsmxt/aseg_labels.csv`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/cli/dicom_convert.py` & `qsmxt-6.4.4/qsmxt/cli/dicom_convert.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/cli/dicom_sort.py` & `qsmxt-6.4.4/qsmxt/cli/dicom_sort.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/cli/main.py` & `qsmxt-6.4.4/qsmxt/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -642,25 +642,31 @@
         with open(args.pipeline_file, "r") as json_file:
             user_premades = json.load(json_file)
         premades.update(user_premades)
 
     # update implicit arguments based on the explicitly selected premade
     if 'premade' in explicit_args.keys():
         if explicit_args['premade'] in premades:
-            for key, value in premades[explicit_args['premade']].items():
-                if key not in explicit_args:# or explicit_args[key] == value:
+            for key in list(premades[explicit_args['premade']].keys()):
+                value = premades[explicit_args['premade']][key]
+                if key not in explicit_args:
                     implicit_args[key] = value
+                    if value is None:
+                        del implicit_args[key]
         else:
             logger.log(LogLevel.ERROR.value, f"Chosen premade pipeline '{explicit_args['premade']}' not found!")
             if args.auto_yes: script_exit(1, logger=logger)
             del explicit_args['premade']
     elif 'premade' in implicit_args.keys():
         if implicit_args['premade'] in premades:
-            for key, value in premades[implicit_args['premade']].items():
+            for key in list(premades[implicit_args['premade']].keys()):
+                value = premades[implicit_args['premade']][key]
                 implicit_args[key] = value
+                if value is None:
+                    del implicit_args[key]
         else:
             logger.log(LogLevel.ERROR.value, f"Chosen premade pipeline '{implicit_args['premade']}' not found!")
             del implicit_args['premade']
     
     # remove any unnecessary explicit args
     for key, value in implicit_args.items():
         if key in explicit_args and explicit_args[key] == value:
@@ -1281,71 +1287,101 @@
                     print("Invalid input")
             args.qsm_reference = user_in
         
     return args.copy(), implicit_args
 
 def process_args(args):
     run_args = {}
+    logger = make_logger('main')
 
     if not any([args.do_qsm, args.do_segmentation, args.do_swi, args.do_t2starmap, args.do_r2starmap]):
         args.do_qsm = True
 
+    if args.do_analysis:
+        if not args.do_segmentation:
+            logger.log(LogLevel.WARNING.value, f"--do_analysis requires --do_segmentation. Enabling --do_segmentation.")
+            args.do_segmentation = True
+    if args.do_segmentation:
+        if not args.do_qsm:
+            logger.log(LogLevel.WARNING.value, f"--do_segmentation requires --do_qsm. Enabling --do_qsm.")
+            args.do_qsm = True
+
     # default QSM algorithms
     if not args.qsm_algorithm:
+        logger.log(LogLevel.WARNING.value, 'No QSM algorithm selected! Defaulting to RTS.')
         args.qsm_algorithm = 'rts'
 
     # default masking settings for QSM algorithms
     if not args.masking_algorithm:
         if args.qsm_algorithm == 'nextqsm':
             args.masking_algorithm = 'bet'
         else:
             args.masking_algorithm = 'threshold'
+        logger.log(LogLevel.WARNING.value, f"No --masking_algorithm set! Defaulting to {args.masking_algorithm}.")
     
     # force masking input to magnitude if bet is the masking method
-    args.masking_input = 'magnitude' if 'bet' in args.masking_algorithm else args.masking_input
+    if 'bet' in args.masking_algorithm and args.masking_input != 'magnitude':
+        logger.log(LogLevel.WARNING.value, f"Switching --masking_input to 'magnitude' which is required for --masking_algorithm 'bet'.")
+        args.masking_input = 'magnitude'
 
     # default threshold settings
     if args.masking_algorithm == 'threshold':
         if not (args.threshold_value or args.threshold_algorithm):
+            logger.log(LogLevel.WARNING.value, f"--masking_algorithm set to 'threshold' but no --threshold_value or --threshold_algorithm set! Defaulting --threshold_algorithm to otsu.")
             args.threshold_algorithm = 'otsu'
         if not args.filling_algorithm:
+            logger.log(LogLevel.WARNING.value, f"--masking_algorithm set to 'threshold' but no --filling_algorithm set! Defaulting to 'both'.")
             args.filling_algorithm = 'both'
 
     # default unwrapping settings for QSM algorithms
-    if not args.unwrapping_algorithm:
-        if args.qsm_algorithm in ['nextqsm', 'rts', 'tv']:
-            args.unwrapping_algorithm = 'romeo'
+    if not args.unwrapping_algorithm and args.qsm_algorithm in ['nextqsm', 'rts', 'tv']:
+        args.unwrapping_algorithm = 'romeo'
+        logger.log(LogLevel.WARNING.value, f"Unwrapping is required for --qsm_algorithm {args.qsm_algorithm} but none is selected! Defaulting to --unwrapping_algorithm {args.unwrapping_algorithm}.")
     if args.combine_phase and args.unwrapping_algorithm != 'romeo':
+        logger.log(LogLevel.WARNING.value, f"--combine_phase option requires --unwrapping_algorithm 'romeo'. Switching to --unwrapping_algorithm 'romeo'.")
         args.unwrapping_algorithm = 'romeo'
 
-    if args.qsm_algorithm in ['tgv']:
+    if args.unwrapping_algorithm and args.qsm_algorithm in ['tgv']:
+        logger.log(LogLevel.WARNING.value, f"--unwrapping_algorithm {args.unwrapping_algorithm} selected, but unwrapping is already handled by --qsm_algorithm 'tgv'. Disabling unwrapping.")
         args.unwrapping_algorithm = None
 
     # add_bet option only works with non-bet masking and filling methods
-    args.add_bet &= 'bet' not in args.masking_algorithm
-    args.add_bet &= 'bet' != args.filling_algorithm
+    if 'bet' in args.masking_algorithm and args.add_bet:
+        logger.log(LogLevel.WARNING.value, f"--add_bet option does not work with --masking_algorithm bet. Disabling --add_bet.")
+        args.add_bet = False
+    if args.filling_algorithm == 'bet' and args.add_bet:
+        logger.log(LogLevel.WARNING.value, f"--add_bet option does not work with --filling_algorithm bet. Disabling --add_bet.")
+        args.add_bet = False
 
     # default two-pass settings for QSM algorithms
     if args.two_pass is None:
         if args.qsm_algorithm in ['rts', 'tgv', 'tv']:
             args.two_pass = True
+            logger.log(LogLevel.WARNING.value, f"--two_pass setting not selected. Defaulting to 'on' for --qsm_algorithm {args.qsm_algorithm}.")
         else:
             args.two_pass = False
+            logger.log(LogLevel.WARNING.value, f"--two_pass setting not selected. Defaulting to 'off' for --qsm_algorithm {args.qsm_algorithm}.")
     
     # two-pass does not work with bet masking, nextqsm, or vsharp
-    args.two_pass &= 'bet' not in args.masking_algorithm
-    args.two_pass &= args.qsm_algorithm != 'nextqsm'
-    args.two_pass &= not (args.bf_algorithm == 'vsharp' and args.qsm_algorithm in ['tv', 'rts', 'nextqsm'])
-
-    # 'bet' hole-filling not applicable for single-pass
-    if not args.two_pass and args.filling_algorithm == 'bet':
-        args.filling_algorithm == 'both'
+    if args.two_pass and 'bet' in args.masking_algorithm:
+        logger.log(LogLevel.WARNING.value, f"--two_pass setting incompatible with --masking_algorithm bet. Disabling --two_pass.")
+        args.two_pass = False
+    
+    if args.two_pass and args.qsm_algorithm == 'nextqsm':
+        logger.log(LogLevel.WARNING.value, f"--two_pass setting incompatible with --qsm_algorithm nextqsm. Disabling --two_pass.")
+        args.two_pass = False
+    
+    if args.two_pass and (args.bf_algorithm == 'vsharp' and args.qsm_algorithm in ['tv', 'rts', 'nextqsm']):
+        logger.log(LogLevel.WARNING.value, f"--two_pass setting incompatible with --bf_algorithm vsharp. Disabling --two_pass.")
+        args.two_pass = False
 
     # decide on inhomogeneity correction
-    args.inhomogeneity_correction &= (args.add_bet or args.masking_input == 'magnitude' or args.filling_algorithm == 'bet')
+    if args.inhomogeneity_correction and not (args.add_bet or args.masking_input == 'magnitude' or args.filling_algorithm == 'bet'):
+        logger.log(LogLevel.WARNING.value, f"--inhomogeneity_correction requries either --add_bet, --masking_input 'magnitude', or --filling_algorithm 'bet'.")
+        args.inhomogeneity_correction = False
 
     # decide on supplementary imaging
     if args.do_r2starmap is None: args.do_r2starmap = False
     if args.do_t2starmap is None: args.do_t2starmap = False
     if args.do_swi is None: args.do_swi = False
     
     # set number of concurrent processes to run depending on available resources
```

### Comparing `qsmxt-6.4.3/qsmxt/cli/nifti_convert.py` & `qsmxt-6.4.4/qsmxt/cli/nifti_convert.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_addtojson.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_addtojson.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_analyse.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_analyse.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_axialsampling.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_axialsampling.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_bet2.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_bet2.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_clearswi.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_clearswi.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_combinemagnitude.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_combinemagnitude.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_erode.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_erode.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_fastsurfer.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_fastsurfer.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_hdbet.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_hdbet.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_json.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_json.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_laplacian_unwrapping.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_laplacian_unwrapping.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_makehomogeneous.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_makehomogeneous.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_masking.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_masking.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_mgz2nii.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_mgz2nii.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_nextqsm.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_nextqsm.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_nii2dcm.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_nii2dcm.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_nonzeroaverage.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_nonzeroaverage.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_phaseweights.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_phaseweights.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_processphase.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_processphase.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_qsm_referencing.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_qsm_referencing.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_qsmjl.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_qsmjl.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_resample_like.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_resample_like.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_t2star_r2star.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_t2star_r2star.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_tgv_qsm.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_tgv_qsm.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_tgv_qsm_jl.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_tgv_qsm_jl.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/nipype_interface_twopass.py` & `qsmxt-6.4.4/qsmxt/interfaces/nipype_interface_twopass.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/interfaces/utils.py` & `qsmxt-6.4.4/qsmxt/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/qsm_pipelines.json` & `qsmxt-6.4.4/qsmxt/qsm_pipelines.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9826530612244898%*

 * *Differences: {"'body'": "{'unwrapping_algorithm': None}", "'nextqsm'": "{'masking_input': 'magnitude'}"}*

```diff
@@ -22,15 +22,16 @@
         ],
         "masking_algorithm": "threshold",
         "masking_input": "phase",
         "qsm_algorithm": "tgv",
         "threshold_value": [
             0.25
         ],
-        "two_pass": true
+        "two_pass": true,
+        "unwrapping_algorithm": null
     },
     "default": {
         "add_bet": false,
         "auto_yes": false,
         "bet_fractional_intensity": 0.5,
         "bf_algorithm": "pdf",
         "combine_phase": true,
@@ -139,11 +140,12 @@
     "nextqsm": {
         "combine_phase": true,
         "description": "Applies suggested settings for running the NeXtQSM algorithm (assumes human brain)",
         "mask_erosions": [
             3
         ],
         "masking_algorithm": "bet",
+        "masking_input": "magnitude",
         "qsm_algorithm": "nextqsm",
         "two_pass": false
     }
 }
```

### Comparing `qsmxt-6.4.3/qsmxt/scripts/antsBuildTemplate.py` & `qsmxt-6.4.4/qsmxt/scripts/antsBuildTemplate.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/hagberg_pb_masking.jl` & `qsmxt-6.4.4/qsmxt/scripts/hagberg_pb_masking.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/logger.py` & `qsmxt-6.4.4/qsmxt/scripts/logger.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/mrt_clearswi.jl` & `qsmxt-6.4.4/qsmxt/scripts/mrt_clearswi.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/mrt_phase_weights.jl` & `qsmxt-6.4.4/qsmxt/scripts/mrt_phase_weights.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/mrt_t2star_r2star.jl` & `qsmxt-6.4.4/qsmxt/scripts/mrt_t2star_r2star.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/nii_fix_ge.py` & `qsmxt-6.4.4/qsmxt/scripts/nii_fix_ge.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/qsmjl_full.jl` & `qsmxt-6.4.4/qsmxt/scripts/qsmjl_full.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/qsmjl_laplacian_unwrapping.jl` & `qsmxt-6.4.4/qsmxt/scripts/qsmjl_laplacian_unwrapping.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/qsmjl_medi.jl` & `qsmxt-6.4.4/qsmxt/scripts/qsmjl_medi.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/qsmjl_pdf.jl` & `qsmxt-6.4.4/qsmxt/scripts/qsmjl_pdf.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/qsmjl_phase_to_frequency.jl` & `qsmxt-6.4.4/qsmxt/scripts/qsmjl_phase_to_frequency.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/qsmjl_rts.jl` & `qsmxt-6.4.4/qsmxt/scripts/qsmjl_rts.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/qsmjl_tv.jl` & `qsmxt-6.4.4/qsmxt/scripts/qsmjl_tv.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/qsmjl_vsharp.jl` & `qsmxt-6.4.4/qsmxt/scripts/qsmjl_vsharp.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/qsmxt_functions.py` & `qsmxt-6.4.4/qsmxt/scripts/qsmxt_functions.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/qsmxt_version.py` & `qsmxt-6.4.4/qsmxt/scripts/qsmxt_version.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/resample_like.py` & `qsmxt-6.4.4/qsmxt/scripts/resample_like.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/romeo_voxelquality.jl` & `qsmxt-6.4.4/qsmxt/scripts/romeo_voxelquality.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/sys_cmd.py` & `qsmxt-6.4.4/qsmxt/scripts/sys_cmd.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/tgv_qsm.jl` & `qsmxt-6.4.4/qsmxt/scripts/tgv_qsm.jl`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/scripts/user_input.py` & `qsmxt-6.4.4/qsmxt/scripts/user_input.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/tests/setup_qsmxt.sh` & `qsmxt-6.4.4/qsmxt/tests/setup_qsmxt.sh`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         if [ "${CONTAINER_IMAGE}" != "vnmd/qsmxt_${TEST_CONTAINER_VERSION}:${TEST_CONTAINER_DATE}" ]; then
             echo "[DEBUG] Existing container image ${CONTAINER_IMAGE} has a different version than required version vnmd/qsmxt_${TEST_CONTAINER_VERSION}:${TEST_CONTAINER_DATE}"
             echo "[DEBUG] Stopping container"
             sudo docker stop qsmxt-container
             echo "[DEBUG] Removing container"
             sudo docker rm qsmxt-container
             echo "[DEBUG] Removing image ${CONTAINER_IMAGE}"
-            sudo docker rmi "${CONTAINER_IMAGE}"
+            sudo docker rmi -f "${CONTAINER_IMAGE}"
         fi
     fi
 
     echo "[DEBUG] Checking if qsmxt-container already exists"
     CONTAINER_EXISTS=$(sudo docker ps -a -q -f name=qsmxt-container)
     if [ ! -n "${CONTAINER_EXISTS}" ]; then
         echo "[DEBUG] Creating qsmxt-container using image vnmd/qsmxt_${TEST_CONTAINER_VERSION}:${TEST_CONTAINER_DATE}"
```

### Comparing `qsmxt-6.4.3/qsmxt/tests/testInstanceSetup.sh` & `qsmxt-6.4.4/qsmxt/tests/testInstanceSetup.sh`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/tests/test_qsm.py` & `qsmxt-6.4.4/qsmxt/tests/test_qsm.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/tests/test_segmentation.py` & `qsmxt-6.4.4/qsmxt/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/tests/test_template.py` & `qsmxt-6.4.4/qsmxt/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/tests/test_transparent_singularity.sh` & `qsmxt-6.4.4/qsmxt/tests/test_transparent_singularity.sh`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/tests/utils.py` & `qsmxt-6.4.4/qsmxt/tests/utils.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/workflows/masking.py` & `qsmxt-6.4.4/qsmxt/workflows/masking.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt/workflows/qsm.py` & `qsmxt-6.4.4/qsmxt/workflows/qsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,14 +233,41 @@
             run_args.do_r2starmap = False
             run_args.do_t2starmap = False
     if (run_args.do_qsm and run_args.use_existing_masks):
         if any(nib.load(mask_files[i]).header['dim'][0] > 3 for i in range(len(mask_files))):
             logger.log(LogLevel.ERROR.value, f"{run_id}: Cannot use existing masks - >3D masks detected! Each mask must be 3D only for BIDS-compliance.")
             run_args.use_existing_masks = False
 
+    # ensure that all input files dimensions match and are 3d
+    if phase_files and any([run_args.do_qsm, run_args.do_swi]):
+        dims = nib.load(phase_files[0]).header.get_data_shape()
+        if len(dims) != 3 or any(dim == 1 for dim in dims[:3]):
+            logger.log(LogLevel.ERROR.value, f"{run_id}: Input dimensions must be 3D! Got {phase_files[0]}={dims}.")
+        for i in range(1, len(phase_files)):
+            dims_i = nib.load(phase_files[i]).header.get_data_shape()
+            if dims != dims_i:
+                logger.log(LogLevel.ERROR.value, f"{run_id}: Incompatible dimensions detected! {phase_files[0]}={dims}; {phase_files[i]}={dims}.")
+        
+        if any([run_args.do_t2starmap, run_args.do_r2starmap, run_args.do_segmentation, run_args.masking_input == 'magnitude', run_args.inhomogeneity_correction, run_args.add_bet]):
+            if not run_args.do_qsm:
+                dims = nib.load(magnitude_files[0]).header.get_data_shape()
+            if len(dims) != 3 or any(dim == 1 for dim in dims[:3]):
+                logger.log(LogLevel.ERROR.value, f"{run_id}: Input dimensions must be 3D! Got {magnitude_files[0]}={dims}.")
+            for i in range(len(magnitude_files)):
+                dims_i = nib.load(magnitude_files[i]).header.get_data_shape()
+                if dims != dims_i:
+                    logger.log(LogLevel.ERROR.value, f"{run_id}: Incompatible dimensions detected! {phase_files[0] if run_args.do_qsm else magnitude_files[0]}={dims}; {magnitude_files[i]}={dims}.")
+        
+        if run_args.do_qsm and run_args.use_existing_masks and mask_files:
+            dims = nib.load(phase_files[0]).header.get_data_shape()
+            for i in range(len(mask_files)):
+                dims_i = nib.load(mask_files[i]).header.get_data_shape()
+                if dims != dims_i:
+                    logger.log(LogLevel.ERROR.value, f"{run_id}: Incompatible dimensions detected! {phase_files[0]}={dims}; {mask_files[i]}={dims}.")
+    
     if not any([run_args.do_qsm, run_args.do_swi, run_args.do_t2starmap, run_args.do_r2starmap, run_args.do_segmentation]):
         return
     
     # create nipype workflow for this run
     wf = Workflow(f"qsmxt" + (f"_acq-{acq}" if acq else "") + (f"_run-{run}" if run else ""), base_dir=os.path.join(run_args.output_dir, "workflow", os.path.join(subject, session) if session else subject, acq or "", run or ""))
 
     # inputs and outputs
```

### Comparing `qsmxt-6.4.3/qsmxt/workflows/template.py` & `qsmxt-6.4.4/qsmxt/workflows/template.py`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/qsmxt.egg-info/PKG-INFO` & `qsmxt-6.4.4/qsmxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsmxt
-Version: 6.4.3
+Version: 6.4.4
 License-File: LICENSE
 Requires-Dist: psutil
 Requires-Dist: datetime
 Requires-Dist: networkx==2.8.8
 Requires-Dist: numpy
 Requires-Dist: h5py
 Requires-Dist: nibabel
```

### Comparing `qsmxt-6.4.3/qsmxt.egg-info/SOURCES.txt` & `qsmxt-6.4.4/qsmxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qsmxt-6.4.3/setup.py` & `qsmxt-6.4.4/setup.py`

 * *Files identical despite different names*

