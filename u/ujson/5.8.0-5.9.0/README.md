# Comparing `tmp/ujson-5.8.0.tar.gz` & `tmp/ujson-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ujson-5.8.0.tar", last modified: Sun Jun 11 08:49:44 2023, max compression
+gzip compressed data, was "ujson-5.9.0.tar", last modified: Sun Dec 10 22:48:40 2023, max compression
```

## Comparing `ujson-5.8.0.tar` & `ujson-5.9.0.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.420806 ujson-5.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.392807 ujson-5.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/renovate.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.392807 ujson-5.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/fuzz.yml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/labels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-11 08:49:24.000000 ujson-5.8.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-11 08:49:24.000000 ujson-5.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-11 08:49:24.000000 ujson-5.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-06-11 08:49:24.000000 ujson-5.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-11 08:49:24.000000 ujson-5.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-06-11 08:49:44.420806 ujson-5.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-06-11 08:49:24.000000 ujson-5.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-11 08:49:24.000000 ujson-5.8.0/RELEASING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.384807 ujson-5.8.0/deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.392807 ujson-5.8.0/deps/double-conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/Changelog
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/SConstruct
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/WORKSPACE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.392807 ujson-5.8.0/deps/double-conversion/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/cmake/Config.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.396807 ujson-5.8.0/deps/double-conversion/double-conversion/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/SConscript
--rw-r--r--   0 runner    (1001) docker     (123)    27617 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/bignum-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/bignum-dtoa.h
--rw-r--r--   0 runner    (1001) docker     (123)    24726 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/bignum.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/bignum.h
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/cached-powers.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/cached-powers.h
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/diy-fp.h
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/double-conversion.h
--rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/double-to-string.cc
--rw-r--r--   0 runner    (1001) docker     (123)    22349 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/double-to-string.h
--rw-r--r--   0 runner    (1001) docker     (123)    31645 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/fast-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/fast-dtoa.h
--rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/fixed-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/fixed-dtoa.h
--rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/ieee.h
--rw-r--r--   0 runner    (1001) docker     (123)    27899 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/string-to-double.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/string-to-double.h
--rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/strtod.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/strtod.h
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/double-conversion/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.396807 ujson-5.8.0/deps/double-conversion/msvc/
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/msvc/double-conversion.sln
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/msvc/double-conversion.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/msvc/double-conversion.vcxproj.filters
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.396807 ujson-5.8.0/deps/double-conversion/msvc/run_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/msvc/testrunner.cmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.396807 ujson-5.8.0/deps/double-conversion/test/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.416806 ujson-5.8.0/deps/double-conversion/test/cctest/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/SConscript
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/cctest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/cctest.h
--rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/checks.h
--rw-r--r--   0 runner    (1001) docker     (123)  5791276 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-fixed.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-fixed.h
--rw-r--r--   0 runner    (1001) docker     (123)  6130717 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-precision.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-precision.h
--rw-r--r--   0 runner    (1001) docker     (123)   491279 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest-single.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest-single.h
--rw-r--r--   0 runner    (1001) docker     (123)  6323023 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest.h
--rw-r--r--   0 runner    (1001) docker     (123)    13486 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-bignum-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    53607 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-bignum.cc
--rw-r--r--   0 runner    (1001) docker     (123)   194514 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-conversions.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-diy-fp.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-fast-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16941 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-fixed-dtoa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18826 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-ieee.cc
--rw-r--r--   0 runner    (1001) docker     (123)    57667 2023-06-11 08:49:24.000000 ujson-5.8.0/deps/double-conversion/test/cctest/test-strtod.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.416806 ujson-5.8.0/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-11 08:49:24.000000 ujson-5.8.0/lib/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-11 08:49:24.000000 ujson-5.8.0/lib/dconv_wrapper.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-06-11 08:49:24.000000 ujson-5.8.0/lib/ultrajson.h
--rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-06-11 08:49:24.000000 ujson-5.8.0/lib/ultrajsondec.c
--rw-r--r--   0 runner    (1001) docker     (123)    25412 2023-06-11 08:49:24.000000 ujson-5.8.0/lib/ultrajsonenc.c
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-11 08:49:24.000000 ujson-5.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.416806 ujson-5.8.0/python/
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-06-11 08:49:24.000000 ujson-5.8.0/python/JSONtoObj.c
--rw-r--r--   0 runner    (1001) docker     (123)    25830 2023-06-11 08:49:24.000000 ujson-5.8.0/python/objToJSON.c
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-11 08:49:24.000000 ujson-5.8.0/python/ujson.c
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 08:49:24.000000 ujson-5.8.0/python/ujson.h
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-11 08:49:44.000000 ujson-5.8.0/python/version.h
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-11 08:49:24.000000 ujson-5.8.0/python/version_template.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.416806 ujson-5.8.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-06-11 08:49:24.000000 ujson-5.8.0/scripts/coverage.sh
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-11 08:49:44.420806 ujson-5.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-11 08:49:24.000000 ujson-5.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.420806 ujson-5.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    29345 2023-06-11 08:49:24.000000 ujson-5.8.0/tests/334-reproducer.json
--rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-06-11 08:49:24.000000 ujson-5.8.0/tests/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-11 08:49:24.000000 ujson-5.8.0/tests/fuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-11 08:49:24.000000 ujson-5.8.0/tests/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)   687492 2023-06-11 08:49:24.000000 ujson-5.8.0/tests/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)    35409 2023-06-11 08:49:24.000000 ujson-5.8.0/tests/test_ujson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:49:44.420806 ujson-5.8.0/ujson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-06-11 08:49:44.000000 ujson-5.8.0/ujson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-11 08:49:44.000000 ujson-5.8.0/ujson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 08:49:44.000000 ujson-5.8.0/ujson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 08:49:44.000000 ujson-5.8.0/ujson.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.197125 ujson-5.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.153125 ujson-5.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/renovate.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.153125 ujson-5.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/workflows/fuzz.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/workflows/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2023-12-10 22:48:08.000000 ujson-5.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-12-10 22:48:08.000000 ujson-5.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-10 22:48:08.000000 ujson-5.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2023-12-10 22:48:08.000000 ujson-5.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-10 22:48:08.000000 ujson-5.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2023-12-10 22:48:40.197125 ujson-5.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2023-12-10 22:48:08.000000 ujson-5.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2023-12-10 22:48:08.000000 ujson-5.9.0/RELEASING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.145125 ujson-5.9.0/deps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.157125 ujson-5.9.0/deps/double-conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/Changelog
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/SConstruct
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/WORKSPACE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.157125 ujson-5.9.0/deps/double-conversion/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/cmake/Config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.161125 ujson-5.9.0/deps/double-conversion/double-conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/SConscript
+-rw-r--r--   0 runner    (1001) docker     (127)    27617 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/bignum-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/bignum-dtoa.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24726 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/bignum.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/cached-powers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/cached-powers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/diy-fp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/double-conversion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15893 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/double-to-string.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    22348 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/double-to-string.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31645 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/fast-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/fast-dtoa.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15352 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/fixed-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/fixed-dtoa.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15223 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/ieee.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27899 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/string-to-double.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10848 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/string-to-double.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23469 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/strtod.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/strtod.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15556 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/double-conversion/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.161125 ujson-5.9.0/deps/double-conversion/msvc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/msvc/double-conversion.sln
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/msvc/double-conversion.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/msvc/double-conversion.vcxproj.filters
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.161125 ujson-5.9.0/deps/double-conversion/msvc/run_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9751 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/msvc/testrunner.cmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.161125 ujson-5.9.0/deps/double-conversion/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.189125 ujson-5.9.0/deps/double-conversion/test/cctest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/SConscript
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/cctest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/cctest.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13134 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/checks.h
+-rw-r--r--   0 runner    (1001) docker     (127)  5791276 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/gay-fixed.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/gay-fixed.h
+-rw-r--r--   0 runner    (1001) docker     (127)  6130717 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/gay-precision.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/gay-precision.h
+-rw-r--r--   0 runner    (1001) docker     (127)   491279 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/gay-shortest-single.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/gay-shortest-single.h
+-rw-r--r--   0 runner    (1001) docker     (127)  6323023 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/gay-shortest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/gay-shortest.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13486 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/test-bignum-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    53607 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/test-bignum.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   194514 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/test-conversions.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/test-diy-fp.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    16468 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/test-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13298 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/test-fast-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    16941 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/test-fixed-dtoa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    18826 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/test-ieee.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    57667 2023-12-10 22:48:08.000000 ujson-5.9.0/deps/double-conversion/test/cctest/test-strtod.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.189125 ujson-5.9.0/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2023-12-10 22:48:08.000000 ujson-5.9.0/lib/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2023-12-10 22:48:08.000000 ujson-5.9.0/lib/dconv_wrapper.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12404 2023-12-10 22:48:08.000000 ujson-5.9.0/lib/ultrajson.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21310 2023-12-10 22:48:08.000000 ujson-5.9.0/lib/ultrajsondec.c
+-rw-r--r--   0 runner    (1001) docker     (127)    25526 2023-12-10 22:48:08.000000 ujson-5.9.0/lib/ultrajsonenc.c
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-10 22:48:08.000000 ujson-5.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.193125 ujson-5.9.0/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2023-12-10 22:48:08.000000 ujson-5.9.0/python/JSONtoObj.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22732 2023-12-10 22:48:08.000000 ujson-5.9.0/python/objToJSON.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2023-12-10 22:48:08.000000 ujson-5.9.0/python/ujson.c
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-10 22:48:08.000000 ujson-5.9.0/python/ujson.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-12-10 22:48:40.000000 ujson-5.9.0/python/version.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2023-12-10 22:48:08.000000 ujson-5.9.0/python/version_template.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.193125 ujson-5.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      851 2023-12-10 22:48:08.000000 ujson-5.9.0/scripts/coverage.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-10 22:48:40.197125 ujson-5.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-12-10 22:48:08.000000 ujson-5.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.193125 ujson-5.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29345 2023-12-10 22:48:08.000000 ujson-5.9.0/tests/334-reproducer.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13419 2023-12-10 22:48:08.000000 ujson-5.9.0/tests/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2023-12-10 22:48:08.000000 ujson-5.9.0/tests/fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-12-10 22:48:08.000000 ujson-5.9.0/tests/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)   687492 2023-12-10 22:48:08.000000 ujson-5.9.0/tests/sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36685 2023-12-10 22:48:08.000000 ujson-5.9.0/tests/test_ujson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 22:48:40.193125 ujson-5.9.0/ujson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2023-12-10 22:48:40.000000 ujson-5.9.0/ujson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2023-12-10 22:48:40.000000 ujson-5.9.0/ujson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 22:48:40.000000 ujson-5.9.0/ujson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-10 22:48:40.000000 ujson-5.9.0/ujson.egg-info/top_level.txt
```

### Comparing `ujson-5.8.0/.github/labels.yml` & `ujson-5.9.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/.github/release-drafter.yml` & `ujson-5.9.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/.github/workflows/benchmark.yml` & `ujson-5.9.0/.github/workflows/benchmark.yml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.11"]
         os: [ubuntu-22.04]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - run: git fetch --prune --unshallow
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: pip
```

### Comparing `ujson-5.8.0/.github/workflows/deploy.yml` & `ujson-5.9.0/.github/workflows/deploy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -21,27 +21,27 @@
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [windows-latest, macOS-latest, ubuntu-latest]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - run: git fetch --prune --unshallow
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
           cache: pip
           cache-dependency-path: ".github/workflows/deploy.yml"
 
       # https://github.com/pypa/cibuildwheel
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.13.1
+        uses: pypa/cibuildwheel@v2.16.2
         with:
           output-dir: dist
         # Options are supplied via environment variables:
         env:
           # Build separate wheels for macOS's different architectures.
           CIBW_ARCHS_MACOS: "x86_64 arm64"
           # Build only on Linux architectures that don't need qemu emulation.
@@ -60,44 +60,44 @@
 
   build-QEMU-emulated-wheels:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version:
-          - pp38
           - pp39
+          - pp310
           - cp38
           - cp39
           - cp310
           - cp311
           - cp312
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - run: git fetch --prune --unshallow
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
           cache: pip
           cache-dependency-path: ".github/workflows/deploy.yml"
 
       # https://github.com/docker/setup-qemu-action
       - name: Set up QEMU
-        uses: docker/setup-qemu-action@v2
+        uses: docker/setup-qemu-action@v3
 
       # https://github.com/docker/setup-buildx-action
       - name: Set up Docker Buildx
-        uses: docker/setup-buildx-action@v2
+        uses: docker/setup-buildx-action@v3
 
       # https://github.com/pypa/cibuildwheel
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.13.1
+        uses: pypa/cibuildwheel@v2.16.2
         with:
           output-dir: dist
         # Options are supplied via environment variables:
         env:
           # Build only the currently selected Linux architecture (so we can
           # parallelise for speed).
           CIBW_ARCHS_LINUX: "aarch64"
@@ -114,17 +114,20 @@
         with:
           name: wheels
           path: dist/*.whl
 
   build-sdist-and-upload:
     runs-on: ubuntu-latest
     needs: ['build-native-wheels', 'build-QEMU-emulated-wheels']
+    permissions:
+      # IMPORTANT: this permission is mandatory for trusted publishing
+      id-token: write
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - run: |
             git fetch --prune --unshallow
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
@@ -141,47 +144,37 @@
         with:
           name: wheels
           path: dist-wheels/
 
       - name: Build package
         run: |
           git tag
-          python setup.py --version
           python -m build --sdist
           twine check --strict dist/*
           twine check --strict dist-wheels/*
 
       - name: Publish wheels to PyPI
         if: github.event.action == 'published'
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          user: __token__
-          password: ${{ secrets.pypi_password }}
           packages-dir: dist-wheels/
 
       - name: Publish sdist to PyPI
         if: github.event.action == 'published'
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          user: __token__
-          password: ${{ secrets.pypi_password }}
 
       - name: Publish wheels to TestPyPI
         if: |
           github.repository == 'ultrajson/ultrajson' &&
           github.ref == 'refs/heads/main'
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          user: __token__
-          password: ${{ secrets.test_pypi_password }}
           repository-url: https://test.pypi.org/legacy/
           packages-dir: dist-wheels/
 
       - name: Publish sdist to TestPyPI
         if: |
           github.repository == 'ultrajson/ultrajson' &&
           github.ref == 'refs/heads/main'
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          user: __token__
-          password: ${{ secrets.test_pypi_password }}
           repository-url: https://test.pypi.org/legacy/
```

### Comparing `ujson-5.8.0/.github/workflows/test.yml` & `ujson-5.9.0/.github/workflows/test.yml`

 * *Files 18% similar despite different names*

```diff
@@ -7,31 +7,32 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy-3.8", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
+        python-version: ["pypy-3.10", "3.8", "3.9", "3.10", "3.11", "3.12"]
         os: [ubuntu-latest]
         include:
-          - { python-version: "pypy-3.8", os: windows-latest }
-          - { python-version: "pypy-3.8", os: macos-latest }
+          - { python-version: "pypy-3.10", os: windows-latest }
+          - { python-version: "pypy-3.10", os: macos-latest }
           - { python-version: "3.10", os: windows-latest }
           - { python-version: "3.10", os: macos-latest }
           - { python-version: "3.11", os: windows-latest }
           - { python-version: "3.11", os: macos-latest }
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+          allow-prereleases: true
           cache: pip
           cache-dependency-path: "setup.py"
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U pytest
@@ -64,24 +65,24 @@
   cross-arch:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         architecture: [ppc64le, s390x, aarch64, arm/v6, 386]
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - run: git fetch --prune --unshallow
 
       # https://github.com/docker/setup-qemu-action
       - name: Set up QEMU
-        uses: docker/setup-qemu-action@v2
+        uses: docker/setup-qemu-action@v3
 
       # https://github.com/docker/setup-buildx-action
       - name: Set up Docker Buildx
-        uses: docker/setup-buildx-action@v2
+        uses: docker/setup-buildx-action@v3
 
       - name: Test
         run: |
           docker run -v "$PWD:/io" --platform=linux/${{ matrix.architecture }} python:alpine ash -e -c '
             apk add gcc g++ musl-dev git
             cd /io
             git config --global --add safe.directory /io
```

### Comparing `ujson-5.8.0/.gitignore` & `ujson-5.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/.pre-commit-config.yaml` & `ujson-5.9.0/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.4.0
+    rev: v3.13.0
     hooks:
       - id: pyupgrade
         args: [--py38-plus]
 
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.9.1
     hooks:
       - id: black
         args: [--target-version=py38]
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
+    rev: 6.1.0
     hooks:
       - id: flake8
         additional_dependencies: [flake8-2020, flake8-implicit-str-concat]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
@@ -36,13 +36,13 @@
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
         exclude: "^.github/.*_TEMPLATE.md"
 
   - repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.3.0
+    rev: v2.4.0
     hooks:
       - id: setup-cfg-fmt
         args: [--include-version-classifiers, --max-py-version=3.12]
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `ujson-5.8.0/LICENSE.txt` & `ujson-5.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/PKG-INFO` & `ujson-5.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ujson
-Version: 5.8.0
+Version: 5.9.0
 Summary: Ultra fast JSON encoder and decoder for Python
 Home-page: https://github.com/ultrajson/ultrajson
 Download-URL: https://github.com/ultrajson/ultrajson
 Author: Jonas Tarnstrom
 Project-URL: Source, https://github.com/ultrajson/ultrajson
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -79,18 +79,18 @@
 ```
 
 #### escape_forward_slashes
 
 Controls whether forward slashes (`/`) are escaped. Default is `True`:
 
 ```pycon
->>> ujson.dumps("http://esn.me")
-'"http:\\/\\/esn.me"'
->>> ujson.dumps("http://esn.me", escape_forward_slashes=False)
-'"http://esn.me"'
+>>> ujson.dumps("https://example.com")
+'"https:\\/\\/example.com"'
+>>> ujson.dumps("https://example.com", escape_forward_slashes=False)
+'"https://example.com"'
 ```
 
 #### indent
 
 Controls whether indentation ("pretty output") is enabled. Default is `0` (disabled):
 
 ```pycon
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_ebbwtwue_/tmpokopfiuw_TarContainer/0/20", line 188, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ujson Version: 5.8.0 Summary: Ultra fast JSON
+Metadata-Version: 2.1 Name: ujson Version: 5.9.0 Summary: Ultra fast JSON
 encoder and decoder for Python Home-page: https://github.com/ultrajson/
 ultrajson Download-URL: https://github.com/ultrajson/ultrajson Author: Jonas
 Tarnstrom Project-URL: Source, https://github.com/ultrajson/ultrajson Platform:
 any Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Programming Language :: C Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `ujson-5.8.0/README.md` & `ujson-5.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -55,18 +55,18 @@
 ```
 
 #### escape_forward_slashes
 
 Controls whether forward slashes (`/`) are escaped. Default is `True`:
 
 ```pycon
->>> ujson.dumps("http://esn.me")
-'"http:\\/\\/esn.me"'
->>> ujson.dumps("http://esn.me", escape_forward_slashes=False)
-'"http://esn.me"'
+>>> ujson.dumps("https://example.com")
+'"https:\\/\\/example.com"'
+>>> ujson.dumps("https://example.com", escape_forward_slashes=False)
+'"https://example.com"'
 ```
 
 #### indent
 
 Controls whether indentation ("pretty output") is enabled. Default is `0` (disabled):
 
 ```pycon
```

### Comparing `ujson-5.8.0/RELEASING.md` & `ujson-5.9.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/BUILD` & `ujson-5.9.0/deps/double-conversion/BUILD`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/CMakeLists.txt` & `ujson-5.9.0/deps/double-conversion/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/COPYING` & `ujson-5.9.0/deps/double-conversion/COPYING`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/Changelog` & `ujson-5.9.0/deps/double-conversion/Changelog`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/LICENSE` & `ujson-5.9.0/deps/double-conversion/LICENSE`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/README.md` & `ujson-5.9.0/deps/double-conversion/README.md`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/SConstruct` & `ujson-5.9.0/deps/double-conversion/SConstruct`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/bignum-dtoa.cc` & `ujson-5.9.0/deps/double-conversion/double-conversion/bignum-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/bignum-dtoa.h` & `ujson-5.9.0/deps/double-conversion/double-conversion/bignum-dtoa.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/bignum.cc` & `ujson-5.9.0/deps/double-conversion/double-conversion/bignum.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/bignum.h` & `ujson-5.9.0/deps/double-conversion/double-conversion/bignum.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/cached-powers.cc` & `ujson-5.9.0/deps/double-conversion/double-conversion/cached-powers.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/cached-powers.h` & `ujson-5.9.0/deps/double-conversion/double-conversion/cached-powers.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/diy-fp.h` & `ujson-5.9.0/deps/double-conversion/double-conversion/diy-fp.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/double-conversion.h` & `ujson-5.9.0/deps/double-conversion/double-conversion/double-conversion.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/double-to-string.cc` & `ujson-5.9.0/deps/double-conversion/double-conversion/double-to-string.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/double-to-string.h` & `ujson-5.9.0/deps/double-conversion/double-conversion/double-to-string.h`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
   //   ToPrecision(123450.0, 3) -> "123000"
   //   ToPrecision(123450.0, 2) -> "1.2e5"
   //
   // Returns true if the conversion succeeds. The conversion always succeeds
   // except for the following cases:
   //   - the input value is special and no infinity_symbol or nan_symbol has
   //     been provided to the constructor,
-  //   - precision < kMinPericisionDigits
+  //   - precision < kMinPrecisionDigits
   //   - precision > kMaxPrecisionDigits
   //
   // The last condition implies that the result never contains more than
   // kMaxPrecisionDigits + 7 characters (the sign, the decimal point, the
   // exponent character, the exponent's sign, and at most 3 exponent digits).
   // In addition, the buffer must be able to hold the trailing '\0' character.
   bool ToPrecision(double value,
```

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/fast-dtoa.cc` & `ujson-5.9.0/deps/double-conversion/double-conversion/fast-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/fast-dtoa.h` & `ujson-5.9.0/deps/double-conversion/double-conversion/fast-dtoa.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/fixed-dtoa.cc` & `ujson-5.9.0/deps/double-conversion/double-conversion/fixed-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/fixed-dtoa.h` & `ujson-5.9.0/deps/double-conversion/double-conversion/fixed-dtoa.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/ieee.h` & `ujson-5.9.0/deps/double-conversion/double-conversion/ieee.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/string-to-double.cc` & `ujson-5.9.0/deps/double-conversion/double-conversion/string-to-double.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/string-to-double.h` & `ujson-5.9.0/deps/double-conversion/double-conversion/string-to-double.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/strtod.cc` & `ujson-5.9.0/deps/double-conversion/double-conversion/strtod.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/strtod.h` & `ujson-5.9.0/deps/double-conversion/double-conversion/strtod.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/double-conversion/utils.h` & `ujson-5.9.0/deps/double-conversion/double-conversion/utils.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/msvc/double-conversion.sln` & `ujson-5.9.0/deps/double-conversion/msvc/double-conversion.sln`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/msvc/double-conversion.vcxproj` & `ujson-5.9.0/deps/double-conversion/msvc/double-conversion.vcxproj`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/msvc/double-conversion.vcxproj.filters` & `ujson-5.9.0/deps/double-conversion/msvc/double-conversion.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj` & `ujson-5.9.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj.filters` & `ujson-5.9.0/deps/double-conversion/msvc/run_tests/run_tests.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/CMakeLists.txt` & `ujson-5.9.0/deps/double-conversion/test/cctest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/cctest.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/cctest.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/cctest.h` & `ujson-5.9.0/deps/double-conversion/test/cctest/cctest.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/checks.h` & `ujson-5.9.0/deps/double-conversion/test/cctest/checks.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/gay-fixed.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/gay-fixed.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/gay-fixed.h` & `ujson-5.9.0/deps/double-conversion/test/cctest/gay-fixed.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/gay-precision.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/gay-precision.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/gay-precision.h` & `ujson-5.9.0/deps/double-conversion/test/cctest/gay-precision.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest-single.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/gay-shortest-single.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest-single.h` & `ujson-5.9.0/deps/double-conversion/test/cctest/gay-shortest-single.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/gay-shortest.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/gay-shortest.h` & `ujson-5.9.0/deps/double-conversion/test/cctest/gay-shortest.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/test-bignum-dtoa.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/test-bignum-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/test-bignum.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/test-bignum.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/test-conversions.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/test-conversions.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/test-diy-fp.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/test-diy-fp.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/test-dtoa.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/test-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/test-fast-dtoa.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/test-fast-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/test-fixed-dtoa.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/test-fixed-dtoa.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/test-ieee.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/test-ieee.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/deps/double-conversion/test/cctest/test-strtod.cc` & `ujson-5.9.0/deps/double-conversion/test/cctest/test-strtod.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/lib/dconv_wrapper.cc` & `ujson-5.9.0/lib/dconv_wrapper.cc`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/lib/ultrajson.h` & `ujson-5.9.0/lib/ultrajson.h`

 * *Files 1% similar despite different names*

```diff
@@ -197,20 +197,20 @@
   const char *(*getStringValue)(JSOBJ obj, JSONTypeContext *tc, size_t *_outLen);
   JSINT64 (*getLongValue)(JSOBJ obj, JSONTypeContext *tc);
   JSUINT64 (*getUnsignedLongValue)(JSOBJ obj, JSONTypeContext *tc);
   double (*getDoubleValue)(JSOBJ obj, JSONTypeContext *tc);
 
   /*
   Retrieve next object in an iteration. Should return 0 to indicate iteration has reached end or 1 if there are more items.
-  Implementor is responsible for keeping state of the iteration. Use ti->prv fields for this
+  Implementer is responsible for keeping state of the iteration. Use ti->prv fields for this
   */
   JSPFN_ITERNEXT iterNext;
 
   /*
-  Ends the iteration of an iteratable object.
+  Ends the iteration of an iterable object.
   Any iteration state stored in ti->prv can be freed here
   */
   JSPFN_ITEREND iterEnd;
 
   /*
   Returns a reference to the value object of an iterator
   The is responsible for the life-cycle of the returned string. Use iterNext/iterEnd and ti->prv to keep track of current object
@@ -280,15 +280,15 @@
   void *prv;
 
   /*
   Pointer to the DoubleToStringConverter instance */
   void *d2s;
 
   /*
-  Set to an error message if error occured */
+  Set to an error message if error occurred */
   const char *errorMsg;
   JSOBJ errorObj;
 
   /* Buffer stuff */
   char *start;
   char *offset;
   char *end;
```

### Comparing `ujson-5.8.0/lib/ultrajsondec.c` & `ujson-5.9.0/lib/ultrajsondec.c`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/lib/ultrajsonenc.c` & `ujson-5.9.0/lib/ultrajsonenc.c`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 #include "ultrajson.h"
 #include <stdio.h>
 #include <assert.h>
 #include <string.h>
 #include <stdlib.h>
 #include <stddef.h>
+#include <stdint.h>
 #include <math.h>
 
 #include <float.h>
 
 #ifndef TRUE
 #define TRUE 1
 #endif
@@ -580,15 +581,21 @@
       for (i = 0; i < enc->indent; i++)
         Buffer_AppendCharUnchecked(enc, ' ');
 }
 
 static void Buffer_AppendLongUnchecked(JSONObjectEncoder *enc, JSINT64 value)
 {
   char* wstr;
-  JSUINT64 uvalue = (value < 0) ? -value : value;
+  JSUINT64 uvalue;
+
+  if (value == INT64_MIN) {
+    uvalue = INT64_MAX + UINT64_C(1);
+  } else {
+    uvalue = (value < 0) ? -value : value;
+  }
 
   wstr = enc->offset;
 #ifdef DEBUG
   // 20 is the maximum length of a JSINT64 (minus sign plus 19 digits)
   if (enc->end - enc->offset < 20) {
     fprintf(stderr, "Ran out of buffer space during Buffer_AppendLongUnchecked()\n");
     abort();
```

### Comparing `ujson-5.8.0/python/JSONtoObj.c` & `ujson-5.9.0/python/JSONtoObj.c`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/python/objToJSON.c` & `ujson-5.9.0/python/objToJSON.c`

 * *Files 15% similar despite different names*

```diff
@@ -55,16 +55,14 @@
   PFN_PyTypeToJSON PyTypeToJSON;
   PyObject *newObj;
   PyObject *dictObj;
   Py_ssize_t index;
   Py_ssize_t size;
   PyObject *itemValue;
   PyObject *itemName;
-  PyObject *attrList;
-  PyObject *iterator;
 
   union
   {
     PyObject *rawJSONValue;
     JSINT64 longValue;
     JSUINT64 unsignedLongValue;
   };
@@ -74,21 +72,14 @@
 
 // If newObj is set, we should use it rather than JSOBJ
 #define GET_OBJ(__jsobj, __ptrtc) (GET_TC(__ptrtc)->newObj ? GET_TC(__ptrtc)->newObj : __jsobj)
 
 // Avoid infinite loop caused by the default function
 #define DEFAULT_FN_MAX_DEPTH 3
 
-struct PyDictIterState
-{
-  PyObject *keys;
-  size_t i;
-  size_t sz;
-};
-
 //#define PRINTMARK() fprintf(stderr, "%s: MARK(%d)\n", __FILE__, __LINE__)
 #define PRINTMARK()
 
 static void *PyLongToINT64(JSOBJ _obj, JSONTypeContext *tc, void *outValue, size_t *_outLen)
 {
   *((JSINT64 *) outValue) = GET_TC(tc)->longValue;
   return NULL;
@@ -98,35 +89,31 @@
 {
   *((JSUINT64 *) outValue) = GET_TC(tc)->unsignedLongValue;
   return NULL;
 }
 
 static void *PyLongToINTSTR(JSOBJ _obj, JSONTypeContext *tc, void *outValue, size_t *_outLen)
 {
-  PyObject *obj = PyNumber_ToBase(_obj, 10);
-  if (!obj)
-  {
-    return NULL;
-  }
+  PyObject *obj = GET_TC(tc)->rawJSONValue;
   *_outLen = PyUnicode_GET_LENGTH(obj);
   return PyUnicode_1BYTE_DATA(obj);
 }
 
 static void *PyFloatToDOUBLE(JSOBJ _obj, JSONTypeContext *tc, void *outValue, size_t *_outLen)
 {
   PyObject *obj = (PyObject *) _obj;
   *((double *) outValue) = PyFloat_AsDouble (obj);
   return NULL;
 }
 
 static void *PyStringToUTF8(JSOBJ _obj, JSONTypeContext *tc, void *outValue, size_t *_outLen)
 {
   PyObject *obj = (PyObject *) _obj;
-  *_outLen = PyBytes_Size(obj);
-  return PyBytes_AsString(obj);
+  *_outLen = PyBytes_GET_SIZE(obj);
+  return PyBytes_AS_STRING(obj);
 }
 
 static char *PyUnicodeToUTF8Raw(JSOBJ _obj, size_t *_outLen, PyObject **pBytesObj)
 {
   /*
   Converts the PyUnicode object to char* whose size is stored in _outLen.
   This conversion may require the creation of an intermediate PyBytes object.
@@ -147,16 +134,16 @@
 
   PyObject *bytesObj = *pBytesObj = PyUnicode_AsEncodedString (obj, NULL, "surrogatepass");
   if (!bytesObj)
   {
     return NULL;
   }
 
-  *_outLen = PyBytes_Size(bytesObj);
-  return PyBytes_AsString(bytesObj);
+  *_outLen = PyBytes_GET_SIZE(bytesObj);
+  return PyBytes_AS_STRING(bytesObj);
 }
 
 static void *PyUnicodeToUTF8(JSOBJ _obj, JSONTypeContext *tc, void *outValue, size_t *_outLen)
 {
   return PyUnicodeToUTF8Raw(_obj, _outLen, &(GET_TC(tc)->newObj));
 }
 
@@ -171,290 +158,192 @@
   {
     return PyStringToUTF8(obj, tc, outValue, _outLen);
   }
 }
 
 static int Tuple_iterNext(JSOBJ obj, JSONTypeContext *tc)
 {
-  PyObject *item;
-
   if (GET_TC(tc)->index >= GET_TC(tc)->size)
   {
     return 0;
   }
 
-  item = PyTuple_GetItem (obj, GET_TC(tc)->index);
-
-  GET_TC(tc)->itemValue = item;
+  GET_TC(tc)->itemValue = PyTuple_GET_ITEM(obj, GET_TC(tc)->index);
   GET_TC(tc)->index ++;
   return 1;
 }
 
 static void Tuple_iterEnd(JSOBJ obj, JSONTypeContext *tc)
 {
 }
 
 static JSOBJ Tuple_iterGetValue(JSOBJ obj, JSONTypeContext *tc)
 {
   return GET_TC(tc)->itemValue;
 }
 
-static char *Tuple_iterGetName(JSOBJ obj, JSONTypeContext *tc, size_t *outLen)
-{
-  return NULL;
-}
-
 static int List_iterNext(JSOBJ obj, JSONTypeContext *tc)
 {
   if (GET_TC(tc)->index >= GET_TC(tc)->size)
   {
     PRINTMARK();
     return 0;
   }
 
-  GET_TC(tc)->itemValue = PyList_GetItem (obj, GET_TC(tc)->index);
+  GET_TC(tc)->itemValue = PyList_GET_ITEM(obj, GET_TC(tc)->index);
   GET_TC(tc)->index ++;
   return 1;
 }
 
 static void List_iterEnd(JSOBJ obj, JSONTypeContext *tc)
 {
 }
 
 static JSOBJ List_iterGetValue(JSOBJ obj, JSONTypeContext *tc)
 {
   return GET_TC(tc)->itemValue;
 }
 
-static char *List_iterGetName(JSOBJ obj, JSONTypeContext *tc, size_t *outLen)
-{
-  return NULL;
-}
-
 //=============================================================================
 // Dict iteration functions
-// itemName might converted to string (Python_Str). Do refCounting
+// itemName might converted to string (PyObject_Str). Do refCounting
 // itemValue is borrowed from object (which is dict). No refCounting
 //=============================================================================
 
-static int Dict_iterNext(JSOBJ obj, JSONTypeContext *tc)
+static PyObject* Dict_convertKey(PyObject* key)
 {
-  PyObject* itemNameTmp;
-
-  if (GET_TC(tc)->itemName)
+  if (PyUnicode_Check(key))
   {
-    Py_DECREF(GET_TC(tc)->itemName);
-    GET_TC(tc)->itemName = NULL;
+    return PyUnicode_AsEncodedString(key, NULL, "surrogatepass");
   }
-
-  if (!(GET_TC(tc)->itemName = PyIter_Next(GET_TC(tc)->iterator)))
+  if (PyBytes_Check(key))
   {
-    PRINTMARK();
-    return 0;
+    Py_INCREF(key);
+    return key;
   }
-
-  if (!(GET_TC(tc)->itemValue = PyDict_GetItem(GET_TC(tc)->dictObj, GET_TC(tc)->itemName)))
+  if (UNLIKELY(PyBool_Check(key)))
+  {
+    return PyBytes_FromString(key == Py_True ? "true" : "false");
+  }
+  if (UNLIKELY(key == Py_None))
+  {
+    return PyBytes_FromString("null");
+  }
+  PyObject* keystr = PyObject_Str(key);
+  if (!keystr)
   {
     PRINTMARK();
-    return 0;
+    return NULL;
   }
+  key = PyUnicode_AsEncodedString(keystr, NULL, "surrogatepass");
+  Py_DECREF(keystr);
+  return key;
+}
 
-  if (PyUnicode_Check(GET_TC(tc)->itemName))
+static int Dict_iterNext(JSOBJ obj, JSONTypeContext *tc)
+{
+  PyObject* key;
+  if (!PyDict_Next(GET_TC(tc)->dictObj, &GET_TC(tc)->index, &key, &GET_TC(tc)->itemValue))
   {
-    itemNameTmp = GET_TC(tc)->itemName;
-    GET_TC(tc)->itemName = PyUnicode_AsEncodedString (GET_TC(tc)->itemName, NULL, "surrogatepass");
-    Py_DECREF(itemNameTmp);
+    PRINTMARK();
+    return 0;
   }
-  else
-  if (!PyBytes_Check(GET_TC(tc)->itemName))
+  Py_XDECREF(GET_TC(tc)->itemName);
+  GET_TC(tc)->itemName = Dict_convertKey(key);
+  if (!GET_TC(tc)->itemName)
   {
-    if (UNLIKELY(GET_TC(tc)->itemName == Py_None))
-    {
-      itemNameTmp = PyUnicode_FromString("null");
-      GET_TC(tc)->itemName = PyUnicode_AsUTF8String(itemNameTmp);
-      Py_DECREF(Py_None);
-      return 1;
-    }
-
-    itemNameTmp = GET_TC(tc)->itemName;
-    GET_TC(tc)->itemName = PyObject_Str(GET_TC(tc)->itemName);
-    Py_DECREF(itemNameTmp);
-    if (PyErr_Occurred())
-    {
-      PRINTMARK();
-      return -1;
-    }
-    itemNameTmp = GET_TC(tc)->itemName;
-    GET_TC(tc)->itemName = PyUnicode_AsEncodedString (GET_TC(tc)->itemName, NULL, "surrogatepass");
-    Py_DECREF(itemNameTmp);
+    return -1;
   }
   PRINTMARK();
   return 1;
 }
 
 static void Dict_iterEnd(JSOBJ obj, JSONTypeContext *tc)
 {
-  if (GET_TC(tc)->itemName)
-  {
-    Py_DECREF(GET_TC(tc)->itemName);
-    GET_TC(tc)->itemName = NULL;
-  }
-  Py_CLEAR(GET_TC(tc)->iterator);
+  Py_CLEAR(GET_TC(tc)->itemName);
   Py_DECREF(GET_TC(tc)->dictObj);
   PRINTMARK();
 }
 
 static JSOBJ Dict_iterGetValue(JSOBJ obj, JSONTypeContext *tc)
 {
   return GET_TC(tc)->itemValue;
 }
 
 static char *Dict_iterGetName(JSOBJ obj, JSONTypeContext *tc, size_t *outLen)
 {
-  *outLen = PyBytes_Size(GET_TC(tc)->itemName);
-  return PyBytes_AsString(GET_TC(tc)->itemName);
+  *outLen = PyBytes_GET_SIZE(GET_TC(tc)->itemName);
+  return PyBytes_AS_STRING(GET_TC(tc)->itemName);
 }
 
 static int SortedDict_iterNext(JSOBJ obj, JSONTypeContext *tc)
 {
-  PyObject *items = NULL, *item = NULL, *key = NULL, *value = NULL;
-  Py_ssize_t i, nitems;
-  PyObject* keyTmp;
-
   // Upon first call, obtain a list of the keys and sort them. This follows the same logic as the
   // standard library's _json.c sort_keys handler.
   if (GET_TC(tc)->newObj == NULL)
   {
     // Obtain the list of keys from the dictionary.
-    items = PyMapping_Keys(GET_TC(tc)->dictObj);
-    if (items == NULL)
-    {
-      goto error;
-    }
-    else if (!PyList_Check(items))
+    PyObject *keys = PyDict_Keys(GET_TC(tc)->dictObj);
+    if (keys == NULL)
     {
-      PyErr_SetString(PyExc_ValueError, "keys must return list");
-      goto error;
+      return -1;
     }
-
     // Sort the list.
-    if (PyList_Sort(items) < 0)
+    if (PyList_Sort(keys) < 0)
     {
-      PyErr_SetString(PyExc_ValueError, "unorderable keys");
-      goto error;
+      Py_DECREF(keys);
+      return -1;
     }
-
-    // Obtain the value for each key, and pack a list of (key, value) 2-tuples.
-    nitems = PyList_Size(items);
-    for (i = 0; i < nitems; i++)
-    {
-      key = PyList_GetItem(items, i);
-      value = PyDict_GetItem(GET_TC(tc)->dictObj, key);
-
-      // Subject the key to the same type restrictions and conversions as in Dict_iterGetValue.
-      if (PyUnicode_Check(key))
-      {
-        key = PyUnicode_AsEncodedString(key, NULL, "surrogatepass");
-      }
-      else if (!PyBytes_Check(key))
-      {
-        key = PyObject_Str(key);
-        if (PyErr_Occurred())
-        {
-          goto error;
-        }
-        keyTmp = key;
-        key = PyUnicode_AsEncodedString(key, NULL, "surrogatepass");
-        Py_DECREF(keyTmp);
-      }
-      else
-      {
-        Py_INCREF(key);
-      }
-
-      item = PyTuple_Pack(2, key, value);
-      if (item == NULL)
-      {
-        goto error;
-      }
-      if (PyList_SetItem(items, i, item))
-      {
-        goto error;
-      }
-      Py_DECREF(key);
-    }
-
-    // Store the sorted list of tuples in the newObj slot.
-    GET_TC(tc)->newObj = items;
-    GET_TC(tc)->size = nitems;
+    // Store the sorted list of keys in the newObj slot.
+    GET_TC(tc)->newObj = keys;
+    GET_TC(tc)->size = PyList_GET_SIZE(keys);
   }
 
   if (GET_TC(tc)->index >= GET_TC(tc)->size)
   {
     PRINTMARK();
     return 0;
   }
 
-  item = PyList_GetItem(GET_TC(tc)->newObj, GET_TC(tc)->index);
-  GET_TC(tc)->itemName = PyTuple_GetItem(item, 0);
-  GET_TC(tc)->itemValue = PyTuple_GetItem(item, 1);
+  PyObject* key = PyList_GET_ITEM(GET_TC(tc)->newObj, GET_TC(tc)->index);
+  Py_XDECREF(GET_TC(tc)->itemName);
+  GET_TC(tc)->itemName = Dict_convertKey(key);
+  if (!GET_TC(tc)->itemName)
+  {
+    return -1;
+  }
+  GET_TC(tc)->itemValue = PyDict_GetItem(GET_TC(tc)->dictObj, key);
+  if (!GET_TC(tc)->itemValue)
+  {
+    return -1;
+  }
   GET_TC(tc)->index++;
   return 1;
-
-error:
-  Py_XDECREF(item);
-  Py_XDECREF(key);
-  Py_XDECREF(value);
-  Py_XDECREF(items);
-  return -1;
-}
-
-static void SortedDict_iterEnd(JSOBJ obj, JSONTypeContext *tc)
-{
-  GET_TC(tc)->itemName = NULL;
-  GET_TC(tc)->itemValue = NULL;
-  Py_DECREF(GET_TC(tc)->dictObj);
-  PRINTMARK();
-}
-
-static JSOBJ SortedDict_iterGetValue(JSOBJ obj, JSONTypeContext *tc)
-{
-  return GET_TC(tc)->itemValue;
-}
-
-static char *SortedDict_iterGetName(JSOBJ obj, JSONTypeContext *tc, size_t *outLen)
-{
-  *outLen = PyBytes_Size(GET_TC(tc)->itemName);
-  return PyBytes_AsString(GET_TC(tc)->itemName);
 }
 
 static void SetupDictIter(PyObject *dictObj, TypeContext *pc, JSONObjectEncoder *enc)
 {
   pc->dictObj = dictObj;
   if (enc->sortKeys)
   {
-    pc->iterEnd = SortedDict_iterEnd;
     pc->iterNext = SortedDict_iterNext;
-    pc->iterGetValue = SortedDict_iterGetValue;
-    pc->iterGetName = SortedDict_iterGetName;
-    pc->index = 0;
   }
   else
   {
-    pc->iterEnd = Dict_iterEnd;
     pc->iterNext = Dict_iterNext;
-    pc->iterGetValue = Dict_iterGetValue;
-    pc->iterGetName = Dict_iterGetName;
-    pc->iterator = PyObject_GetIter(dictObj);
   }
+  pc->iterEnd = Dict_iterEnd;
+  pc->iterGetValue = Dict_iterGetValue;
+  pc->iterGetName = Dict_iterGetName;
+  pc->index = 0;
 }
 
 static void Object_beginTypeContext (JSOBJ _obj, JSONTypeContext *tc, JSONObjectEncoder *enc)
 {
-  PyObject *obj, *objRepr, *exc, *defaultFn, *newObj;
+  PyObject *obj, *objRepr, *defaultFn, *newObj;
   int level = 0;
   TypeContext *pc;
   PRINTMARK();
   if (!_obj)
   {
     tc->type = JT_INVALID;
     return;
@@ -471,16 +360,14 @@
     PyErr_NoMemory();
     return;
   }
   pc->newObj = NULL;
   pc->dictObj = NULL;
   pc->itemValue = NULL;
   pc->itemName = NULL;
-  pc->iterator = NULL;
-  pc->attrList = NULL;
   pc->index = 0;
   pc->size = 0;
   pc->longValue = 0;
   pc->rawJSONValue = NULL;
 
 BEGIN:
   if (PyIter_Check(obj))
@@ -498,56 +385,51 @@
   else
   if (PyLong_Check(obj))
   {
     PRINTMARK();
     pc->PyTypeToJSON = PyLongToINT64;
     tc->type = JT_LONG;
     GET_TC(tc)->longValue = PyLong_AsLongLong(obj);
-
-    exc = PyErr_Occurred();
-    if (!exc)
+    if (!(GET_TC(tc)->longValue == -1 && PyErr_Occurred()))
     {
-        return;
+      return;
     }
-
-    if (exc && PyErr_ExceptionMatches(PyExc_OverflowError))
+    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
     {
-      PyErr_Clear();
-      pc->PyTypeToJSON = PyLongToUINT64;
-      tc->type = JT_ULONG;
-      GET_TC(tc)->unsignedLongValue = PyLong_AsUnsignedLongLong(obj);
-
-      exc = PyErr_Occurred();
+      goto INVALID;
     }
-
-    if (exc && PyErr_ExceptionMatches(PyExc_OverflowError))
+    PyErr_Clear();
+    pc->PyTypeToJSON = PyLongToUINT64;
+    tc->type = JT_ULONG;
+    GET_TC(tc)->unsignedLongValue = PyLong_AsUnsignedLongLong(obj);
+    if (!(GET_TC(tc)->unsignedLongValue == (unsigned long long)-1 && PyErr_Occurred()))
     {
-      PyErr_Clear();
-      pc->PyTypeToJSON = PyLongToINTSTR;
-      tc->type = JT_RAW;
-      // Overwritten by PyLong_* due to the union, which would lead to a DECREF in endTypeContext.
-      GET_TC(tc)->rawJSONValue = NULL;
       return;
     }
-
-    if (exc)
+    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
     {
-      PRINTMARK();
       goto INVALID;
     }
-
+    PyErr_Clear();
+    GET_TC(tc)->rawJSONValue = PyNumber_ToBase(obj, 10);
+    if (!GET_TC(tc)->rawJSONValue)
+    {
+      goto INVALID;
+    }
+    pc->PyTypeToJSON = PyLongToINTSTR;
+    tc->type = JT_RAW;
     return;
   }
   else
   if (UNLIKELY(PyBytes_Check(obj)))
   {
     PRINTMARK();
     if (enc->rejectBytes)
     {
-      PyErr_Format (PyExc_TypeError, "reject_bytes is on and '%s' is bytes", PyBytes_AsString(obj));
+      PyErr_Format (PyExc_TypeError, "reject_bytes is on and '%s' is bytes", PyBytes_AS_STRING(obj));
       goto INVALID;
     }
     else
     {
       pc->PyTypeToJSON = PyStringToUTF8; tc->type = JT_UTF8;
       return;
     }
@@ -587,95 +469,78 @@
   if (PyList_Check(obj))
   {
     PRINTMARK();
     tc->type = JT_ARRAY;
     pc->iterEnd = List_iterEnd;
     pc->iterNext = List_iterNext;
     pc->iterGetValue = List_iterGetValue;
-    pc->iterGetName = List_iterGetName;
     GET_TC(tc)->index =  0;
-    GET_TC(tc)->size = PyList_Size( (PyObject *) obj);
+    GET_TC(tc)->size = PyList_GET_SIZE( (PyObject *) obj);
     return;
   }
   else
   if (PyTuple_Check(obj))
   {
     PRINTMARK();
     tc->type = JT_ARRAY;
     pc->iterEnd = Tuple_iterEnd;
     pc->iterNext = Tuple_iterNext;
     pc->iterGetValue = Tuple_iterGetValue;
-    pc->iterGetName = Tuple_iterGetName;
     GET_TC(tc)->index = 0;
-    GET_TC(tc)->size = PyTuple_Size( (PyObject *) obj);
+    GET_TC(tc)->size = PyTuple_GET_SIZE( (PyObject *) obj);
     GET_TC(tc)->itemValue = NULL;
 
     return;
   }
 
   if (UNLIKELY(PyObject_HasAttrString(obj, "toDict")))
   {
-    PyObject* toDictFunc = PyObject_GetAttrString(obj, "toDict");
-    PyObject* tuple = PyTuple_New(0);
-    PyObject* toDictResult = PyObject_Call(toDictFunc, tuple, NULL);
-    Py_DECREF(tuple);
-    Py_DECREF(toDictFunc);
-
+    PyObject* toDictResult = PyObject_CallMethod(obj, "toDict", NULL);
     if (toDictResult == NULL)
     {
       goto INVALID;
     }
 
     if (!PyDict_Check(toDictResult))
     {
+      PyErr_Format(PyExc_TypeError, "toDict() should return a dict, got %s",
+                   Py_TYPE(toDictResult)->tp_name);
       Py_DECREF(toDictResult);
-      tc->type = JT_NULL;
-      return;
+      goto INVALID;
     }
 
     PRINTMARK();
     tc->type = JT_OBJECT;
     SetupDictIter(toDictResult, pc, enc);
     return;
   }
   else
   if (UNLIKELY(PyObject_HasAttrString(obj, "__json__")))
   {
-    PyObject* toJSONFunc = PyObject_GetAttrString(obj, "__json__");
-    PyObject* tuple = PyTuple_New(0);
-    PyObject* toJSONResult = PyObject_Call(toJSONFunc, tuple, NULL);
-    Py_DECREF(tuple);
-    Py_DECREF(toJSONFunc);
-
+    PyObject* toJSONResult = PyObject_CallMethod(obj, "__json__", NULL);
     if (toJSONResult == NULL)
     {
       goto INVALID;
     }
 
-    if (PyErr_Occurred())
-    {
-      Py_DECREF(toJSONResult);
-      goto INVALID;
-    }
-
     if (!PyBytes_Check(toJSONResult) && !PyUnicode_Check(toJSONResult))
     {
+      PyErr_Format(PyExc_TypeError, "__json__() should return str or bytes, got %s",
+                   Py_TYPE(toJSONResult)->tp_name);
       Py_DECREF(toJSONResult);
-      PyErr_Format (PyExc_TypeError, "expected string");
       goto INVALID;
     }
 
     PRINTMARK();
     pc->PyTypeToJSON = PyRawJSONToUTF8;
     tc->type = JT_RAW;
     GET_TC(tc)->rawJSONValue = toJSONResult;
     return;
   }
 
-DEFAULT:
   if (defaultFn)
   {
     // Break infinite loop
     if (level >= DEFAULT_FN_MAX_DEPTH)
     {
       PRINTMARK();
       PyErr_Format(PyExc_TypeError, "maximum recursion depth exceeded");
@@ -704,15 +569,15 @@
   if (!objRepr)
   {
     goto INVALID;
   }
   PyObject* str = PyUnicode_AsEncodedString(objRepr, NULL, "strict");
   if (str)
   {
-    PyErr_Format (PyExc_TypeError, "%s is not JSON serializable", PyBytes_AsString(str));
+    PyErr_Format (PyExc_TypeError, "%s is not JSON serializable", PyBytes_AS_STRING(str));
   }
   Py_XDECREF(str);
   Py_DECREF(objRepr);
 
 INVALID:
   PRINTMARK();
   tc->type = JT_INVALID;
@@ -899,34 +764,26 @@
   if (oseparators != NULL && oseparators != Py_None)
   {
     if (!PyTuple_Check(oseparators))
     {
       PyErr_SetString(PyExc_TypeError, "expected tuple or None as separator");
       return NULL;
     }
-    if (PyTuple_Size (oseparators) != 2)
+    if (PyTuple_GET_SIZE(oseparators) != 2)
     {
       PyErr_SetString(PyExc_ValueError, "expected tuple of size 2 as separator");
       return NULL;
     }
-    oseparatorsItem = PyTuple_GetItem(oseparators, 0);
-    if (PyErr_Occurred())
-    {
-      return NULL;
-    }
+    oseparatorsItem = PyTuple_GET_ITEM(oseparators, 0);
     if (!PyUnicode_Check(oseparatorsItem))
     {
       PyErr_SetString(PyExc_TypeError, "expected str as item separator");
       return NULL;
     }
-    oseparatorsKey = PyTuple_GetItem(oseparators, 1);
-    if (PyErr_Occurred())
-    {
-      return NULL;
-    }
+    oseparatorsKey = PyTuple_GET_ITEM(oseparators, 1);
     if (!PyUnicode_Check(oseparatorsKey))
     {
       PyErr_SetString(PyExc_TypeError, "expected str as key separator");
       return NULL;
     }
     encoder.itemSeparatorChars = PyUnicodeToUTF8Raw(oseparatorsItem, &encoder.itemSeparatorLength, &separatorsItemBytes);
     if (encoder.itemSeparatorChars == NULL)
@@ -967,18 +824,20 @@
   ret = JSON_EncodeObject (oinput, &encoder, buffer, sizeof (buffer), &retLen);
   PRINTMARK();
 
   dconv_d2s_free(&encoder.d2s);
   Py_XDECREF(separatorsItemBytes);
   Py_XDECREF(separatorsKeyBytes);
 
-  if (encoder.errorMsg && !PyErr_Occurred())
+  if (encoder.errorMsg)
   {
     // If there is an error message and we don't already have a Python exception, set one.
-    PyErr_Format (PyExc_OverflowError, "%s", encoder.errorMsg);
+    if (!PyErr_Occurred())
+      PyErr_Format(PyExc_OverflowError, "%s", encoder.errorMsg);
+    return NULL;
   }
 
   if (PyErr_Occurred())
   {
     if (ret != buffer)
     {
       encoder.free (ret);
```

### Comparing `ujson-5.8.0/python/ujson.c` & `ujson-5.9.0/python/ujson.c`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/python/version.h` & `ujson-5.9.0/python/version.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 
 Numeric decoder derived from from TCL library
 http://www.opensource.apple.com/source/tcl/tcl-14/tcl/license.terms
  * Copyright (c) 1988-1993 The Regents of the University of California.
  * Copyright (c) 1994 Sun Microsystems, Inc.
 */
 
-#define UJSON_VERSION "5.8.0"
+#define UJSON_VERSION "5.9.0"
```

### Comparing `ujson-5.8.0/python/version_template.h` & `ujson-5.9.0/python/version_template.h`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/scripts/coverage.sh` & `ujson-5.9.0/scripts/coverage.sh`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/setup.cfg` & `ujson-5.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/setup.py` & `ujson-5.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/tests/334-reproducer.json` & `ujson-5.9.0/tests/334-reproducer.json`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/tests/benchmark.py` & `ujson-5.9.0/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/tests/fuzz.py` & `ujson-5.9.0/tests/fuzz.py`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/tests/memory.py` & `ujson-5.9.0/tests/memory.py`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/tests/sample.json` & `ujson-5.9.0/tests/sample.json`

 * *Files identical despite different names*

### Comparing `ujson-5.8.0/tests/test_ujson.py` & `ujson-5.9.0/tests/test_ujson.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,16 +194,16 @@
     encoded_json = json.dumps(s, ensure_ascii=False)
     assert len(encoded) == len(s) + 2  # original length + quotes
     assert encoded == encoded_json
     decoded = ujson.loads(encoded)
     assert s == decoded
 
 
-def test_encode_long_neg_conversion():
-    test_input = -9223372036854775808
+@pytest.mark.parametrize("test_input", [-1, -9223372036854775808, 18446744073709551615])
+def test_encode_special_longs(test_input):
     output = ujson.encode(test_input)
 
     json.loads(output)
     ujson.decode(output)
 
     assert test_input == json.loads(output)
     assert output == json.dumps(test_input)
@@ -238,15 +238,15 @@
     ujson.dumps(data)
     assert ref_count == sys.getrefcount(value)
 
 
 @pytest.mark.skipif(
     hasattr(sys, "pypy_version_info"), reason="PyPy uses incompatible GC"
 )
-@pytest.mark.parametrize("key", ["key", b"key", 1, True, None])
+@pytest.mark.parametrize("key", ["key", b"key", 1, True, False, None])
 @pytest.mark.parametrize("sort_keys", [False, True])
 def test_encode_dict_key_ref_counting(key, sort_keys):
     import gc
 
     gc.collect()
     data = {key: "abc"}
     ref_count = sys.getrefcount(key)
@@ -491,14 +491,38 @@
             raise AttributeError
 
     d = {"key": JSONTest()}
     with pytest.raises(AttributeError):
         ujson.encode(d)
 
 
+def test_object_with_to_dict_type_error():
+    # toDict must return a dict, otherwise it should raise an error.
+    for return_value in (None, 1234, 12.34, True, "json"):
+
+        class JSONTest:
+            def toDict(self):
+                return return_value
+
+        d = {"key": JSONTest()}
+        with pytest.raises(TypeError):
+            ujson.encode(d)
+
+
+def test_object_with_to_dict_attribute_error():
+    # If toDict raises an error, make sure python actually raises it.
+    class JSONTest:
+        def toDict(self):
+            raise AttributeError
+
+    d = {"key": JSONTest()}
+    with pytest.raises(AttributeError):
+        ujson.encode(d)
+
+
 def test_decode_array_empty():
     test_input = "[]"
     obj = ujson.decode(test_input)
     assert [] == obj
 
 
 def test_encode_surrogate_characters():
@@ -548,14 +572,21 @@
 
 def test_sort_keys():
     data = {"a": 1, "c": 1, "b": 1, "e": 1, "f": 1, "d": 1}
     sorted_keys = ujson.dumps(data, sort_keys=True)
     assert sorted_keys == '{"a":1,"b":1,"c":1,"d":1,"e":1,"f":1}'
 
 
+def test_sort_keys_unordered():
+    data = {"a": 1, 1: 2, None: 3}
+    assert ujson.dumps(data) == '{"a":1,"1":2,"null":3}'
+    with pytest.raises(TypeError):
+        ujson.dumps(data, sort_keys=True)
+
+
 @pytest.mark.parametrize(
     "test_input",
     [
         "[31337]",  # array one item
         "18446744073709551615",  # long unsigned value
         "9223372036854775807",  # big value
         "-9223372036854775808",  # small value
@@ -971,17 +1002,21 @@
 
 
 def test_reject_bytes_false():
     data = {"a": b"b"}
     assert ujson.dumps(data, reject_bytes=False) == '{"a":"b"}'
 
 
-def test_encode_none_key():
-    data = {None: None}
-    assert ujson.dumps(data) == '{"null":null}'
+def test_encode_special_keys():
+    data = {None: 0, True: 1, False: 2}
+    assert ujson.dumps(data) == '{"null":0,"true":1,"false":2}'
+    data = {None: 0}
+    assert ujson.dumps(data, sort_keys=True) == '{"null":0}'
+    data = {True: 1, False: 2}
+    assert ujson.dumps(data, sort_keys=True) == '{"false":2,"true":1}'
 
 
 def test_default_function():
     iso8601_time_format = "%Y-%m-%dT%H:%M:%S.%f"
 
     class CustomObject:
         pass
@@ -1065,16 +1100,20 @@
 
 @pytest.mark.parametrize("sort_keys", [False, True])
 def test_obj_str_exception(sort_keys):
     class Obj:
         def __str__(self):
             raise NotImplementedError
 
+    key = Obj()
+    getrefcount = getattr(sys, "getrefcount", lambda x: 0)
+    old = getrefcount(key)
     with pytest.raises(NotImplementedError):
-        ujson.dumps({Obj(): 1}, sort_keys=sort_keys)
+        ujson.dumps({key: 1}, sort_keys=sort_keys)
+    assert getrefcount(key) == old
 
 
 def no_memory_leak(func_code, n=None):
     code = f"import functools, ujson; func = {func_code}"
     path = os.path.join(os.path.dirname(__file__), "memory.py")
     n = [str(n)] if n is not None else []
     p = subprocess.run([sys.executable, path, code] + n)
```

### Comparing `ujson-5.8.0/ujson.egg-info/PKG-INFO` & `ujson-5.9.0/ujson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ujson
-Version: 5.8.0
+Version: 5.9.0
 Summary: Ultra fast JSON encoder and decoder for Python
 Home-page: https://github.com/ultrajson/ultrajson
 Download-URL: https://github.com/ultrajson/ultrajson
 Author: Jonas Tarnstrom
 Project-URL: Source, https://github.com/ultrajson/ultrajson
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -79,18 +79,18 @@
 ```
 
 #### escape_forward_slashes
 
 Controls whether forward slashes (`/`) are escaped. Default is `True`:
 
 ```pycon
->>> ujson.dumps("http://esn.me")
-'"http:\\/\\/esn.me"'
->>> ujson.dumps("http://esn.me", escape_forward_slashes=False)
-'"http://esn.me"'
+>>> ujson.dumps("https://example.com")
+'"https:\\/\\/example.com"'
+>>> ujson.dumps("https://example.com", escape_forward_slashes=False)
+'"https://example.com"'
 ```
 
 #### indent
 
 Controls whether indentation ("pretty output") is enabled. Default is `0` (disabled):
 
 ```pycon
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_ebbwtwue_/tmpokopfiuw_TarContainer/0/120", line 188, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ujson Version: 5.8.0 Summary: Ultra fast JSON
+Metadata-Version: 2.1 Name: ujson Version: 5.9.0 Summary: Ultra fast JSON
 encoder and decoder for Python Home-page: https://github.com/ultrajson/
 ultrajson Download-URL: https://github.com/ultrajson/ultrajson Author: Jonas
 Tarnstrom Project-URL: Source, https://github.com/ultrajson/ultrajson Platform:
 any Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Programming Language :: C Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `ujson-5.8.0/ujson.egg-info/SOURCES.txt` & `ujson-5.9.0/ujson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

