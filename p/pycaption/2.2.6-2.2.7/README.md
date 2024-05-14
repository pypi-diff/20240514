# Comparing `tmp/pycaption-2.2.6.tar.gz` & `tmp/pycaption-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycaption-2.2.6.tar", last modified: Tue Apr  9 09:48:24 2024, max compression
+gzip compressed data, was "pycaption-2.2.7.tar", last modified: Tue May 14 07:51:14 2024, max compression
```

## Comparing `pycaption-2.2.6.tar` & `pycaption-2.2.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.950192 pycaption-2.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-09 09:48:12.000000 pycaption-2.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 09:48:12.000000 pycaption-2.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-09 09:48:24.946191 pycaption-2.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-09 09:48:12.000000 pycaption-2.2.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.938192 pycaption-2.2.6/pycaption/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.942191 pycaption-2.2.6/pycaption/dfxp/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/dfxp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50759 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/dfxp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/dfxp/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)   433305 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/english.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30173 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/microdvd.py
--rw-r--r--   0 runner    (1001) docker     (127)    28247 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/sami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.942191 pycaption-2.2.6/pycaption/scc/
--rw-r--r--   0 runner    (1001) docker     (127)    24902 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/scc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27793 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/scc/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    27734 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/scc/specialized_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/scc/state_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    32255 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/scc/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/srt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/webvtt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.946191 pycaption-2.2.6/pycaption.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-09 09:48:24.000000 pycaption-2.2.6/pycaption.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-09 09:48:24.000000 pycaption-2.2.6/pycaption.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:48:24.000000 pycaption-2.2.6/pycaption.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 09:48:24.000000 pycaption-2.2.6/pycaption.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 09:48:24.000000 pycaption-2.2.6/pycaption.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:48:24.950192 pycaption-2.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-09 09:48:12.000000 pycaption-2.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.946191 pycaption-2.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.946191 pycaption-2.2.6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49641 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/dfxp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/microdvd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17112 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/sami.py
--rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/scc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/srt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/translated_scc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/webvtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_dfxp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_dfxp_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_dfxp_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_microdvd.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_microdvd_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_sami.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_sami_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    22989 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_scc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_scc_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_scc_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_srt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_srt_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_webvtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_webvtt_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.405020 pycaption-2.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-14 07:50:55.000000 pycaption-2.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 07:50:55.000000 pycaption-2.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-14 07:51:14.405020 pycaption-2.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-14 07:50:55.000000 pycaption-2.2.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.397020 pycaption-2.2.7/pycaption/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.397020 pycaption-2.2.7/pycaption/dfxp/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/dfxp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50759 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/dfxp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/dfxp/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)   433305 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/english.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30173 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/microdvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28247 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/sami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.397020 pycaption-2.2.7/pycaption/scc/
+-rw-r--r--   0 runner    (1001) docker     (127)    24902 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/scc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/scc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27936 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/scc/specialized_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/scc/state_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32255 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/scc/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/webvtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.405020 pycaption-2.2.7/pycaption.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-14 07:51:14.000000 pycaption-2.2.7/pycaption.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-14 07:51:14.000000 pycaption-2.2.7/pycaption.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:51:14.000000 pycaption-2.2.7/pycaption.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 07:51:14.000000 pycaption-2.2.7/pycaption.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 07:51:14.000000 pycaption-2.2.7/pycaption.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:51:14.405020 pycaption-2.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-14 07:50:55.000000 pycaption-2.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.401020 pycaption-2.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.405020 pycaption-2.2.7/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49641 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/dfxp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/microdvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17112 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/sami.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/translated_scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/webvtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_dfxp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_dfxp_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_dfxp_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_microdvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_microdvd_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_sami.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_sami_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_scc_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_scc_translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_srt_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_webvtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_webvtt_conversion.py
```

### Comparing `pycaption-2.2.6/LICENSE` & `pycaption-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/PKG-INFO` & `pycaption-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaption
-Version: 2.2.6
+Version: 2.2.7
 Summary: Closed caption converter
 Author: Joe Norton
 Author-email: joey@nortoncrew.com
 Project-URL: Source, https://github.com/pbs/pycaption
 Project-URL: Documentation, https://pycaption.readthedocs.io/
 Project-URL: Release notes, https://pycaption.readthedocs.io/en/stable/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycaption-2.2.6/README.rst` & `pycaption-2.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/__init__.py` & `pycaption-2.2.7/pycaption/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/base.py` & `pycaption-2.2.7/pycaption/base.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/dfxp/base.py` & `pycaption-2.2.7/pycaption/dfxp/base.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/dfxp/extras.py` & `pycaption-2.2.7/pycaption/dfxp/extras.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/english.pickle` & `pycaption-2.2.7/pycaption/english.pickle`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/exceptions.py` & `pycaption-2.2.7/pycaption/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/geometry.py` & `pycaption-2.2.7/pycaption/geometry.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/microdvd.py` & `pycaption-2.2.7/pycaption/microdvd.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/sami.py` & `pycaption-2.2.7/pycaption/sami.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/scc/__init__.py` & `pycaption-2.2.7/pycaption/scc/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/scc/constants.py` & `pycaption-2.2.7/pycaption/scc/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1042,7 +1042,13 @@
      '•': ["."],
      '℠': ["s"],
      '┌': ["+"],
      '┐': ["+"],
      '└': ["+"],
      '┘': ["+"]
 }
+
+MID_ROW_CODES = [
+    "9120", "91a1", "91a2", "9123", "91a4", "9125", "9126",
+    "91a7", "91a8", "9129", "912a", "91ab", "912c", "91ad",
+    "97ae", "972f", "91ae", "912f", "94a8"
+]
```

### Comparing `pycaption-2.2.6/pycaption/scc/specialized_collections.py` & `pycaption-2.2.7/pycaption/scc/specialized_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from ..base import CaptionList, Caption, CaptionNode
 from ..geometry import (
     UnitEnum, Size, Layout, Point, Alignment,
     VerticalAlignmentEnum, HorizontalAlignmentEnum
 )
 from .constants import (
     PAC_BYTES_TO_POSITIONING_MAP, COMMANDS, PAC_TAB_OFFSET_COMMANDS,
-    MICROSECONDS_PER_CODEWORD, INCONVERTIBLE_TO_ASCII_EXTENDED_CHARS_ASSOCIATION
+    MICROSECONDS_PER_CODEWORD, INCONVERTIBLE_TO_ASCII_EXTENDED_CHARS_ASSOCIATION,
+    MID_ROW_CODES
 )
 
 PopOnCue = collections.namedtuple("PopOnCue", "buffer, start, end")
 
 
 class PreCaption:
     """
@@ -250,15 +251,15 @@
                     ))
 
             # handle text
             elif instruction.is_text_node():
                 layout_info = _get_layout_from_tuple(instruction.position)
                 caption.nodes.append(
                     CaptionNode.create_text(
-                        instruction.get_text(), layout_info=layout_info),
+                        instruction.text, layout_info=layout_info),
                 )
                 caption.layout_info = layout_info
 
         self._collection.extend(self._still_editing)
 
     def get_all(self):
         """Returns the Caption collection as a CaptionList
@@ -342,14 +343,20 @@
 
         :type command: str
         """
         self._update_positioning(command)
 
         text = COMMANDS.get(command, '')
 
+        if command in MID_ROW_CODES:
+            for node in self._collection[::-1]:
+                if node.is_text_node():
+                    node.text += ' '
+                    break
+
         if 'italic' in text:
             if 'end' not in text:
                 self._collection.append(
                     _InstructionNode.create_italics_style(
                         self._position_tracer.get_current_position())
                 )
             else:
```

### Comparing `pycaption-2.2.6/pycaption/scc/state_machines.py` & `pycaption-2.2.7/pycaption/scc/state_machines.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/scc/translator.py` & `pycaption-2.2.7/pycaption/scc/translator.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/srt.py` & `pycaption-2.2.7/pycaption/srt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/transcript.py` & `pycaption-2.2.7/pycaption/transcript.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption/webvtt.py` & `pycaption-2.2.7/pycaption/webvtt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/pycaption.egg-info/PKG-INFO` & `pycaption-2.2.7/pycaption.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaption
-Version: 2.2.6
+Version: 2.2.7
 Summary: Closed caption converter
 Author: Joe Norton
 Author-email: joey@nortoncrew.com
 Project-URL: Source, https://github.com/pbs/pycaption
 Project-URL: Documentation, https://pycaption.readthedocs.io/
 Project-URL: Release notes, https://pycaption.readthedocs.io/en/stable/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycaption-2.2.6/pycaption.egg-info/SOURCES.txt` & `pycaption-2.2.7/pycaption.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/setup.py` & `pycaption-2.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 transcript_dependencies = [
     'nltk'
 ]
 
 setup(
     name='pycaption',
-    version='2.2.6',
+    version='2.2.7',
     description='Closed caption converter',
     long_description=open(README_PATH).read(),
     author='Joe Norton',
     author_email='joey@nortoncrew.com',
     project_urls={
         'Source': 'https://github.com/pbs/pycaption',
         'Documentation': 'https://pycaption.readthedocs.io/',
```

### Comparing `pycaption-2.2.6/tests/conftest.py` & `pycaption-2.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/fixtures/dfxp.py` & `pycaption-2.2.7/tests/fixtures/dfxp.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/fixtures/microdvd.py` & `pycaption-2.2.7/tests/fixtures/microdvd.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/fixtures/sami.py` & `pycaption-2.2.7/tests/fixtures/sami.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/fixtures/scc.py` & `pycaption-2.2.7/tests/fixtures/scc.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/fixtures/srt.py` & `pycaption-2.2.7/tests/fixtures/srt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/fixtures/translated_scc.py` & `pycaption-2.2.7/tests/fixtures/translated_scc.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/fixtures/webvtt.py` & `pycaption-2.2.7/tests/fixtures/webvtt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/mixins.py` & `pycaption-2.2.7/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_base.py` & `pycaption-2.2.7/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_dfxp.py` & `pycaption-2.2.7/tests/test_dfxp.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_dfxp_conversion.py` & `pycaption-2.2.7/tests/test_dfxp_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_dfxp_extras.py` & `pycaption-2.2.7/tests/test_dfxp_extras.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_functions.py` & `pycaption-2.2.7/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_geometry.py` & `pycaption-2.2.7/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_microdvd.py` & `pycaption-2.2.7/tests/test_microdvd.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_microdvd_conversion.py` & `pycaption-2.2.7/tests/test_microdvd_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_sami.py` & `pycaption-2.2.7/tests/test_sami.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_sami_conversion.py` & `pycaption-2.2.7/tests/test_sami_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_scc.py` & `pycaption-2.2.7/tests/test_scc.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,18 +202,18 @@
         assert captions[0].nodes[0].content == 'MÄRTHA:'
         expected_result = ['JUNIOR: ¡Yum!', None, 'Ya me siento mucho mejor.']
         content = [node.content for node in captions[1].nodes]
         assert all(result in expected_result for result in content)
 
     def test_skip_duplicate_tab_offset(self, sample_scc_duplicate_tab_offset):
         expected_lines = [
-            '[Radio reporter]',
-            'The I-10 Santa Monica Freeway',
+            '[Radio reporter] ',
+            'The I-10 Santa Monica Freeway ',
             'westbound is jammed,',
-            'due to a three-car accident',
+            'due to a three-car accident ',
             'blocking lanes 1 and 2',
         ]
 
         caption_set = SCCReader().read(sample_scc_duplicate_tab_offset)
         actual_lines = [
             node.content
             for cap_ in caption_set.get_captions('en-US')
```

### Comparing `pycaption-2.2.6/tests/test_scc_conversion.py` & `pycaption-2.2.7/tests/test_scc_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_scc_translator.py` & `pycaption-2.2.7/tests/test_scc_translator.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_srt.py` & `pycaption-2.2.7/tests/test_srt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_srt_conversion.py` & `pycaption-2.2.7/tests/test_srt_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_webvtt.py` & `pycaption-2.2.7/tests/test_webvtt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.6/tests/test_webvtt_conversion.py` & `pycaption-2.2.7/tests/test_webvtt_conversion.py`

 * *Files identical despite different names*

