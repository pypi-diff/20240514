# Comparing `tmp/rms-textkernel-1.0.1.tar.gz` & `tmp/rms_textkernel-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-textkernel-1.0.1.tar", last modified: Wed Jan 24 23:36:12 2024, max compression
+gzip compressed data, was "rms_textkernel-1.0.2.tar", last modified: Tue May 14 19:18:56 2024, max compression
```

## Comparing `rms-textkernel-1.0.1.tar` & `rms_textkernel-1.0.2.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:36:12.251469 rms-textkernel-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:36:12.239469 rms-textkernel-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:36:12.243469 rms-textkernel-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-01-24 23:36:12.251469 rms-textkernel-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:36:12.251469 rms-textkernel-1.0.1/rms_textkernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-01-24 23:36:12.000000 rms-textkernel-1.0.1/rms_textkernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-01-24 23:36:12.000000 rms-textkernel-1.0.1/rms_textkernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 23:36:12.000000 rms-textkernel-1.0.1/rms_textkernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-24 23:36:12.000000 rms-textkernel-1.0.1/rms_textkernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-24 23:36:12.000000 rms-textkernel-1.0.1/rms_textkernel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-24 23:36:12.251469 rms-textkernel-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:36:12.247469 rms-textkernel-1.0.1/test_files/
--rwxr-xr-x   0 runner    (1001) docker     (127)    18952 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/cas00149.tsc
--rwxr-xr-x   0 runner    (1001) docker     (127)    31060 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/cas_iss_v10.ti
--rwxr-xr-x   0 runner    (1001) docker     (127)    22880 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/cas_rocks_v18.tf
--rwxr-xr-x   0 runner    (1001) docker     (127)    10004 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/cas_status_v04.tf
--rwxr-xr-x   0 runner    (1001) docker     (127)   181119 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/cas_v40.tf
--rwxr-xr-x   0 runner    (1001) docker     (127)   205215 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/cpck14Oct2011.tpc
--rwxr-xr-x   0 runner    (1001) docker     (127)    71993 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/cpck_rock_21Jan2011_merged.tpc
--rwxr-xr-x   0 runner    (1001) docker     (127)    35081 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/earth_topo_050714.tf
--rwxr-xr-x   0 runner    (1001) docker     (127)    14198 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/juno_jiram_v00.ti
--rwxr-xr-x   0 runner    (1001) docker     (127)   106198 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/juno_v02.tf
--rwxr-xr-x   0 runner    (1001) docker     (127)    18035 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/mars_iau2000_v0.tpc
--rwxr-xr-x   0 runner    (1001) docker     (127)    10127 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/mk00062a.tsc
--rwxr-xr-x   0 runner    (1001) docker     (127)     4733 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/naif0009.tls
--rwxr-xr-x   0 runner    (1001) docker     (127)    31235 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/new_horizons_295.tsc
--rwxr-xr-x   0 runner    (1001) docker     (127)    24695 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/nh_lorri_v100.ti
--rwxr-xr-x   0 runner    (1001) docker     (127)   103294 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/nh_v110.tf
--rwxr-xr-x   0 runner    (1001) docker     (127)   126143 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/pck00010.tpc
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/spkmeta-171106.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    93376 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/vg200011.tsc
--rwxr-xr-x   0 runner    (1001) docker     (127)     1107 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/vg2_isswa_v01.ti
--rwxr-xr-x   0 runner    (1001) docker     (127)    12008 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/test_files/vg2_v02.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:36:12.247469 rms-textkernel-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/tests/test_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/tests/test_from_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/tests/test_name_grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/tests/test_value_grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:36:12.251469 rms-textkernel-1.0.1/textkernel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:36:12.251469 rms-textkernel-1.0.1/textkernel/SPICE_N0067/
--rw-r--r--   0 runner    (1001) docker     (127)    42433 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/textkernel/SPICE_N0067/zzfdat.f
--rw-r--r--   0 runner    (1001) docker     (127)    60816 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/textkernel/SPICE_N0067/zzidmap.f
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/textkernel/_DATA_GRAMMAR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/textkernel/_NAME_GRAMMAR.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/textkernel/_PREDEFINED_BODY_INFO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/textkernel/_PREDEFINED_FRAME_INFO.py
--rw-r--r--   0 runner    (1001) docker     (127)    22265 2024-01-24 23:35:53.000000 rms-textkernel-1.0.1/textkernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-24 23:36:12.000000 rms-textkernel-1.0.1/textkernel/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:56.146314 rms_textkernel-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:56.134314 rms_textkernel-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:56.138314 rms_textkernel-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-14 19:18:56.146314 rms_textkernel-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:56.146314 rms_textkernel-1.0.2/rms_textkernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-14 19:18:56.000000 rms_textkernel-1.0.2/rms_textkernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-14 19:18:56.000000 rms_textkernel-1.0.2/rms_textkernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:18:56.000000 rms_textkernel-1.0.2/rms_textkernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 19:18:56.000000 rms_textkernel-1.0.2/rms_textkernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 19:18:56.000000 rms_textkernel-1.0.2/rms_textkernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 19:18:56.146314 rms_textkernel-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:56.142315 rms_textkernel-1.0.2/test_files/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18952 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/cas00149.tsc
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31060 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/cas_iss_v10.ti
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22880 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/cas_rocks_v18.tf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10004 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/cas_status_v04.tf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   181119 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/cas_v40.tf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   205215 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/cpck14Oct2011.tpc
+-rwxr-xr-x   0 runner    (1001) docker     (127)    71993 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/cpck_rock_21Jan2011_merged.tpc
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35081 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/earth_topo_050714.tf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14198 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/juno_jiram_v00.ti
+-rwxr-xr-x   0 runner    (1001) docker     (127)   106198 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/juno_v02.tf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18035 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/mars_iau2000_v0.tpc
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10127 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/mk00062a.tsc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4733 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/naif0009.tls
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31235 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/new_horizons_295.tsc
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24695 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/nh_lorri_v100.ti
+-rwxr-xr-x   0 runner    (1001) docker     (127)   103294 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/nh_v110.tf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   126143 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/pck00010.tpc
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/spkmeta-171106.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    93376 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/vg200011.tsc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1107 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/vg2_isswa_v01.ti
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12008 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/test_files/vg2_v02.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:56.146314 rms_textkernel-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/tests/test_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/tests/test_from_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/tests/test_name_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/tests/test_value_grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:56.146314 rms_textkernel-1.0.2/textkernel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:56.146314 rms_textkernel-1.0.2/textkernel/SPICE_N0067/
+-rw-r--r--   0 runner    (1001) docker     (127)    42433 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/textkernel/SPICE_N0067/zzfdat.f
+-rw-r--r--   0 runner    (1001) docker     (127)    60816 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/textkernel/SPICE_N0067/zzidmap.f
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/textkernel/_DATA_GRAMMAR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/textkernel/_NAME_GRAMMAR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/textkernel/_PREDEFINED_BODY_INFO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/textkernel/_PREDEFINED_FRAME_INFO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22377 2024-05-14 19:18:41.000000 rms_textkernel-1.0.2/textkernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:18:56.000000 rms_textkernel-1.0.2/textkernel/_version.py
```

### Comparing `rms-textkernel-1.0.1/.github/workflows/publish_to_pypi.yml` & `rms_textkernel-1.0.2/.github/workflows/publish_to_pypi.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Publish to PyPI
-run-name: Publish to PyPI triggered by ${{ github.ref_type }} ${{ github.ref_name }}
+run-name: "Publish to PyPI: ${{ github.ref_type }} ${{ github.ref_name }}"
 
 on:
   release:
     types: [published]
 
 jobs:
   upload_pypi:
@@ -11,15 +11,15 @@
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
```

### Comparing `rms-textkernel-1.0.1/.github/workflows/publish_to_test_pypi.yml` & `rms_textkernel-1.0.2/.github/workflows/publish_to_test_pypi.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 name: Publish to Test PyPI
-run-name: Publish to Test PyPI triggered by ${{ github.ref_type }} ${{ github.ref_name }}
+run-name: "Publish to Test PyPI: ${{ github.ref_type }} ${{ github.ref_name }}"
 
 on:
   workflow_dispatch:
 
 jobs:
   upload_pypi:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
```

### Comparing `rms-textkernel-1.0.1/.github/workflows/run-tests.yml` & `rms_textkernel-1.0.2/.github/workflows/run-tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Run Tests
-run-name: Run Tests triggered by ${{ github.ref_type }} ${{ github.ref_name }} or ${{ github.triggering_actor }}
+run-name: "Run Tests: ${{ github.ref_type }} ${{ github.ref_name }} by ${{ github.triggering_actor }}"
 
 on:
   workflow_dispatch:
   pull_request:
     branches: [ main ]
   push:
     branches: [ main ]
@@ -22,25 +22,29 @@
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           ref: ${{ github.event.pull_request.head.sha }}
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
 
       - name: Test with coverage
         run: |
           coverage run -m pytest
+
+      - name: Print coverage report
+        run: |
           coverage report -m
 
       - name: Upload coverage report to codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
+        if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `rms-textkernel-1.0.1/.gitignore` & `rms_textkernel-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/LICENSE` & `rms_textkernel-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/pyproject.toml` & `rms_textkernel-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/rms_textkernel.egg-info/SOURCES.txt` & `rms_textkernel-1.0.2/rms_textkernel.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 .coveragerc
 .flake8
 .gitignore
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/workflows/publish_to_pypi.yml
 .github/workflows/publish_to_test_pypi.yml
```

### Comparing `rms-textkernel-1.0.1/test_files/cas00149.tsc` & `rms_textkernel-1.0.2/test_files/cas00149.tsc`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/cas_iss_v10.ti` & `rms_textkernel-1.0.2/test_files/cas_iss_v10.ti`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/cas_rocks_v18.tf` & `rms_textkernel-1.0.2/test_files/cas_rocks_v18.tf`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/cas_status_v04.tf` & `rms_textkernel-1.0.2/test_files/cas_status_v04.tf`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/cas_v40.tf` & `rms_textkernel-1.0.2/test_files/cas_v40.tf`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/cpck14Oct2011.tpc` & `rms_textkernel-1.0.2/test_files/cpck14Oct2011.tpc`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/cpck_rock_21Jan2011_merged.tpc` & `rms_textkernel-1.0.2/test_files/cpck_rock_21Jan2011_merged.tpc`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/earth_topo_050714.tf` & `rms_textkernel-1.0.2/test_files/earth_topo_050714.tf`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/juno_jiram_v00.ti` & `rms_textkernel-1.0.2/test_files/juno_jiram_v00.ti`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/juno_v02.tf` & `rms_textkernel-1.0.2/test_files/juno_v02.tf`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/mars_iau2000_v0.tpc` & `rms_textkernel-1.0.2/test_files/mars_iau2000_v0.tpc`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/mk00062a.tsc` & `rms_textkernel-1.0.2/test_files/mk00062a.tsc`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/naif0009.tls` & `rms_textkernel-1.0.2/test_files/naif0009.tls`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/new_horizons_295.tsc` & `rms_textkernel-1.0.2/test_files/new_horizons_295.tsc`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/nh_lorri_v100.ti` & `rms_textkernel-1.0.2/test_files/nh_lorri_v100.ti`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/nh_v110.tf` & `rms_textkernel-1.0.2/test_files/nh_v110.tf`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/pck00010.tpc` & `rms_textkernel-1.0.2/test_files/pck00010.tpc`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/spkmeta-171106.txt` & `rms_textkernel-1.0.2/test_files/spkmeta-171106.txt`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/vg200011.tsc` & `rms_textkernel-1.0.2/test_files/vg200011.tsc`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/vg2_isswa_v01.ti` & `rms_textkernel-1.0.2/test_files/vg2_isswa_v01.ti`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/test_files/vg2_v02.tf` & `rms_textkernel-1.0.2/test_files/vg2_v02.tf`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/tests/__init__.py` & `rms_textkernel-1.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/tests/test_from_file.py` & `rms_textkernel-1.0.2/tests/test_from_file.py`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/tests/test_from_text.py` & `rms_textkernel-1.0.2/tests/test_from_text.py`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/tests/test_name_grammar.py` & `rms_textkernel-1.0.2/tests/test_name_grammar.py`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/tests/test_value_grammar.py` & `rms_textkernel-1.0.2/tests/test_value_grammar.py`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/textkernel/SPICE_N0067/zzfdat.f` & `rms_textkernel-1.0.2/textkernel/SPICE_N0067/zzfdat.f`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/textkernel/SPICE_N0067/zzidmap.f` & `rms_textkernel-1.0.2/textkernel/SPICE_N0067/zzidmap.f`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/textkernel/_DATA_GRAMMAR.py` & `rms_textkernel-1.0.2/textkernel/_DATA_GRAMMAR.py`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/textkernel/_NAME_GRAMMAR.py` & `rms_textkernel-1.0.2/textkernel/_NAME_GRAMMAR.py`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/textkernel/_PREDEFINED_BODY_INFO.py` & `rms_textkernel-1.0.2/textkernel/_PREDEFINED_BODY_INFO.py`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/textkernel/_PREDEFINED_FRAME_INFO.py` & `rms_textkernel-1.0.2/textkernel/_PREDEFINED_FRAME_INFO.py`

 * *Files identical despite different names*

### Comparing `rms-textkernel-1.0.1/textkernel/__init__.py` & `rms_textkernel-1.0.2/textkernel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,20 @@
 import re
 
 from textkernel._DATA_GRAMMAR          import _DATA_GRAMMAR
 from textkernel._NAME_GRAMMAR          import _NAME_GRAMMAR
 from textkernel._PREDEFINED_BODY_INFO  import _PREDEFINED_BODY_INFO
 from textkernel._PREDEFINED_FRAME_INFO import _PREDEFINED_FRAME_INFO
 
+try:
+    from ._version import __version__
+except ImportError as err:
+    __version__ = 'Version unspecified'
+
+
 # Regular expressions to match \\begindata and \\begintext sections. These must be alone
 # on a line. NOTE: There's really only one backslash in front of the "b", but two are
 # needed in the Python source code because a single backslash indicates an escape.
 _BEGINDATA = re.compile(r'\n[ \t]*\\begindata[ \t]*\r?\n', re.S)
 _BEGINTEXT = re.compile(r'\n[ \t]*\\begintext[ \t]*\r?\n', re.S)
```

