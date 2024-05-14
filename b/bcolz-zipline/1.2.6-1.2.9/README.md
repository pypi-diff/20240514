# Comparing `tmp/bcolz-zipline-1.2.6.tar.gz` & `tmp/bcolz_zipline-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcolz-zipline-1.2.6.tar", last modified: Thu Nov 17 20:23:40 2022, max compression
+gzip compressed data, was "bcolz_zipline-1.2.9.tar", last modified: Tue May 14 05:43:55 2024, max compression
```

## Comparing `bcolz-zipline-1.2.6.tar` & `bcolz_zipline-1.2.9.tar`

### file list

```diff
@@ -1,422 +1,414 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.133004 bcolz-zipline-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)    53248 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/.coverage
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.097004 bcolz-zipline-1.2.6/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.097004 bcolz-zipline-1.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3039 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/.github/workflows/build_conda.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/.github/workflows/build_wheels.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/.github/workflows/unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/.mailmap
--rw-r--r--   0 runner    (1001) docker     (121)     3459 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/ANNOUNCE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     4836 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/DISK_FORMAT_v1.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.101004 bcolz-zipline-1.2.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)     6555 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/LICENSES/APPVEYOR-DEMO.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/LICENSES/BCOLZ.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/LICENSES/BLOSC.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/LICENSES/FASTLZ.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/LICENSES/LZ4.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/LICENSES/NUMPY.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/LICENSES/SNAPPY.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/LICENSES/STDINT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/LICENSES/ZLIB.txt
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11672 2022-11-17 20:23:40.133004 bcolz-zipline-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8485 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    28440 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/RELEASE_NOTES.rst
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/THANKS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/appveyor.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.101004 bcolz-zipline-1.2.6/bcolz/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/PythonHelper.h
--rw-r--r--   0 runner    (1001) docker     (121)     4103 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-11-17 20:23:39.000000 bcolz-zipline-1.2.6/bcolz/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    26656 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/arrayprint.py
--rw-r--r--   0 runner    (1001) docker     (121)     3706 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/attrs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/carray_ext.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    97840 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/carray_ext.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/check_blosc_version.h
--rw-r--r--   0 runner    (1001) docker     (121)    11217 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/chunked_eval.py
--rw-r--r--   0 runner    (1001) docker     (121)    51578 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/ctable.py
--rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/definitions.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/py2help.py
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/py2help_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.101004 bcolz-zipline-1.2.6/bcolz/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/tests/all.py
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     5312 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (121)    92292 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/tests/test_carray.py
--rw-r--r--   0 runner    (1001) docker     (121)     5637 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/tests/test_carray_objects.py
--rw-r--r--   0 runner    (1001) docker     (121)    94148 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/tests/test_ctable.py
--rw-r--r--   0 runner    (1001) docker     (121)    31941 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/tests/test_ndcarray.py
--rw-r--r--   0 runner    (1001) docker     (121)    13627 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (121)    22635 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/toplevel.py
--rw-r--r--   0 runner    (1001) docker     (121)     6533 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bcolz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.101004 bcolz-zipline-1.2.6/bcolz_zipline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11672 2022-11-17 20:23:39.000000 bcolz-zipline-1.2.6/bcolz_zipline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13774 2022-11-17 20:23:40.000000 bcolz-zipline-1.2.6/bcolz_zipline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 20:23:39.000000 bcolz-zipline-1.2.6/bcolz_zipline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 20:23:39.000000 bcolz-zipline-1.2.6/bcolz_zipline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-17 20:23:39.000000 bcolz-zipline-1.2.6/bcolz_zipline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-17 20:23:39.000000 bcolz-zipline-1.2.6/bcolz_zipline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.105004 bcolz-zipline-1.2.6/bench/
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/arange.py
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/column-iter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2004 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/concat.py
--rw-r--r--   0 runner    (1001) docker     (121)     6212 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/ctable-query.py
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/eval-profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/eval.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/eval_and_replace.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/fill.py
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/fromiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/getitem.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/iter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/iterblocks.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/large_carray.py
--rw-r--r--   0 runner    (1001) docker     (121)  1242137 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/multithreaded_copy.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/objpickles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/pandas-fromdataframe-strings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/pandas-fromdataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/pandas-todataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/pytables-fromhdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/pytables-tohdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/query.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      136 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/run.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/serialization.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/sum.py
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/whereblocks.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/zeros.py
--rw-r--r--   0 runner    (1001) docker     (121)    10381 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench/zlib-vs-cblosc-zlib.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.105004 bcolz-zipline-1.2.6/bench_asv/
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench_asv/README_asv.md
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench_asv/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.105004 bcolz-zipline-1.2.6/bench_asv/bench/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench_asv/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench_asv/bench/arange.py
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench_asv/bench/bench_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench_asv/bench/column_iter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3006 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/bench_asv/bench/concat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.109004 bcolz-zipline-1.2.6/c-blosc/
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.093004 bcolz-zipline-1.2.6/c-blosc/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.109004 bcolz-zipline-1.2.6/c-blosc/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     4560 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/.github/workflows/cmake.yml
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/.github/workflows/fuzz.yml
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/.mailmap
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/ANNOUNCE.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14563 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8097 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/COMPILING_WITH_WHEELS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.109004 bcolz-zipline-1.2.6/c-blosc/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/LICENSES/BITSHUFFLE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/LICENSES/BLOSC.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/LICENSES/FASTLZ.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/LICENSES/LZ4.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/LICENSES/SNAPPY.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/LICENSES/STDINT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/LICENSES/ZLIB.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6958 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3398 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/README_CHUNK_FORMAT.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/README_THREADED.rst
--rw-r--r--   0 runner    (1001) docker     (121)    40487 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/RELEASE_NOTES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2822 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/RELEASING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/THANKS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      766 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/THOUGHTS_FOR_2.0.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.109004 bcolz-zipline-1.2.6/c-blosc/bench/
--rw-r--r--   0 runner    (1001) docker     (121)     4779 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/bench/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/bench/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/bench/Makefile.mingw
--rw-r--r--   0 runner    (1001) docker     (121)    18390 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/bench/bench.c
--rw-r--r--   0 runner    (1001) docker     (121)     7222 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/bench/plot-speeds.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.113004 bcolz-zipline-1.2.6/c-blosc/blosc/
--rw-r--r--   0 runner    (1001) docker     (121)     8299 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8295 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/bitshuffle-avx2.c
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/bitshuffle-avx2.h
--rw-r--r--   0 runner    (1001) docker     (121)     6812 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/bitshuffle-generic.c
--rw-r--r--   0 runner    (1001) docker     (121)     6491 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/bitshuffle-generic.h
--rw-r--r--   0 runner    (1001) docker     (121)    16683 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/bitshuffle-sse2.c
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/bitshuffle-sse2.h
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/blosc-common.h
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/blosc-comp-features.h
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/blosc-export.h
--rw-r--r--   0 runner    (1001) docker     (121)    69874 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/blosc.c
--rw-r--r--   0 runner    (1001) docker     (121)    19570 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/blosc.h
--rw-r--r--   0 runner    (1001) docker     (121)    26921 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/blosclz.c
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/blosclz.h
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/config.h.in
--rw-r--r--   0 runner    (1001) docker     (121)    16580 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/fastcopy.c
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/fastcopy.h
--rw-r--r--   0 runner    (1001) docker     (121)    30871 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/shuffle-avx2.c
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/shuffle-avx2.h
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/shuffle-generic.c
--rw-r--r--   0 runner    (1001) docker     (121)     3611 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/shuffle-generic.h
--rw-r--r--   0 runner    (1001) docker     (121)    25521 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/shuffle-sse2.c
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/shuffle-sse2.h
--rw-r--r--   0 runner    (1001) docker     (121)    17007 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/shuffle.c
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/shuffle.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.113004 bcolz-zipline-1.2.6/c-blosc/blosc/win32/
--rw-r--r--   0 runner    (1001) docker     (121)     6505 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/win32/pthread.c
--rw-r--r--   0 runner    (1001) docker     (121)     3976 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/win32/pthread.h
--rw-r--r--   0 runner    (1001) docker     (121)     8101 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc/win32/stdint-windows.h
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/blosc.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.113004 bcolz-zipline-1.2.6/c-blosc/cmake/
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/cmake/FindLZ4.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/cmake/FindSnappy.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/cmake/FindZstd.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/code_of_conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.117004 bcolz-zipline-1.2.6/c-blosc/compat/
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    26736 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.11.1-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    33610 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.11.1-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    32485 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.11.1-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (121)   199683 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.11.1-snappy.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    16176 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.11.1-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (121)     3569 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.11.1-zstd.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    36256 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.14.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    36267 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.14.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    36263 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.14.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (121)   199855 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.14.0-snappy.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    20530 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.14.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (121)     3569 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.14.0-zstd.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    75152 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-blosclz-bitshuffle.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    36256 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (121)   184228 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-lz4-bitshuffle.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    36267 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    36263 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    20530 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-zstd.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    36349 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.3.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    36267 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.3.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    31963 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.3.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (121)   199935 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.3.0-snappy.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    14956 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.3.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    36394 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.7.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    36267 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.7.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    31963 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.7.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (121)   199935 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.7.0-snappy.cdata
--rw-r--r--   0 runner    (1001) docker     (121)    14956 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.7.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/compat/filegen.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.117004 bcolz-zipline-1.2.6/c-blosc/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3182 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/examples/many_compressors.c
--rw-r--r--   0 runner    (1001) docker     (121)     2626 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/examples/multithread.c
--rw-r--r--   0 runner    (1001) docker     (121)     2273 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/examples/noinit.c
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/examples/simple.c
--rw-r--r--   0 runner    (1001) docker     (121)     3924 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/examples/win-dynamic-linking.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.093004 bcolz-zipline-1.2.6/c-blosc/internal-complibs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.117004 bcolz-zipline-1.2.6/c-blosc/internal-complibs/lz4-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)   105087 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/lz4-1.9.3/lz4.c
--rw-r--r--   0 runner    (1001) docker     (121)    40861 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/lz4-1.9.3/lz4.h
--rw-r--r--   0 runner    (1001) docker     (121)    69010 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/lz4-1.9.3/lz4hc.c
--rw-r--r--   0 runner    (1001) docker     (121)    20165 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/lz4-1.9.3/lz4hc.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.121004 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     4968 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/adler32.c
--rw-r--r--   0 runner    (1001) docker     (121)     2529 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/compress.c
--rw-r--r--   0 runner    (1001) docker     (121)    13174 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/crc32.c
--rw-r--r--   0 runner    (1001) docker     (121)    30562 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/crc32.h
--rw-r--r--   0 runner    (1001) docker     (121)    71476 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/deflate.c
--rw-r--r--   0 runner    (1001) docker     (121)    12774 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/deflate.h
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/gzclose.c
--rw-r--r--   0 runner    (1001) docker     (121)     6597 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/gzguts.h
--rw-r--r--   0 runner    (1001) docker     (121)    16415 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/gzlib.c
--rw-r--r--   0 runner    (1001) docker     (121)    18694 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/gzread.c
--rw-r--r--   0 runner    (1001) docker     (121)    16199 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/gzwrite.c
--rw-r--r--   0 runner    (1001) docker     (121)    22709 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/infback.c
--rw-r--r--   0 runner    (1001) docker     (121)    13455 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inffast.c
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inffast.h
--rw-r--r--   0 runner    (1001) docker     (121)     6332 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inffixed.h
--rw-r--r--   0 runner    (1001) docker     (121)    53512 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inflate.c
--rw-r--r--   0 runner    (1001) docker     (121)     6399 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inflate.h
--rw-r--r--   0 runner    (1001) docker     (121)    13028 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inftrees.c
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inftrees.h
--rw-r--r--   0 runner    (1001) docker     (121)    44255 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/trees.c
--rw-r--r--   0 runner    (1001) docker     (121)     8472 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/trees.h
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/uncompr.c
--rw-r--r--   0 runner    (1001) docker     (121)    15508 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/zconf.h
--rw-r--r--   0 runner    (1001) docker     (121)    87883 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/zlib.h
--rw-r--r--   0 runner    (1001) docker     (121)     7414 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/zutil.c
--rw-r--r--   0 runner    (1001) docker     (121)     6766 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/zutil.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.121004 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     4556 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/BUCK
--rw-r--r--   0 runner    (1001) docker     (121)    13871 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    10106 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.121004 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/
--rw-r--r--   0 runner    (1001) docker     (121)    18198 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/bitstream.h
--rw-r--r--   0 runner    (1001) docker     (121)    10157 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/compiler.h
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/cpu.h
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/debug.c
--rw-r--r--   0 runner    (1001) docker     (121)     3763 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/debug.h
--rw-r--r--   0 runner    (1001) docker     (121)    13790 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/entropy_common.c
--rw-r--r--   0 runner    (1001) docker     (121)     3009 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/error_private.c
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/error_private.h
--rw-r--r--   0 runner    (1001) docker     (121)    34578 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/fse.h
--rw-r--r--   0 runner    (1001) docker     (121)    14748 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/fse_decompress.c
--rw-r--r--   0 runner    (1001) docker     (121)    20216 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/huf.h
--rw-r--r--   0 runner    (1001) docker     (121)    13930 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/mem.h
--rw-r--r--   0 runner    (1001) docker     (121)    11305 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/pool.c
--rw-r--r--   0 runner    (1001) docker     (121)     2532 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/pool.h
--rw-r--r--   0 runner    (1001) docker     (121)     2941 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/threading.c
--rw-r--r--   0 runner    (1001) docker     (121)     5355 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/threading.h
--rw-r--r--   0 runner    (1001) docker     (121)    26976 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (121)    11706 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_common.c
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_deps.h
--rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_errors.h
--rw-r--r--   0 runner    (1001) docker     (121)    15880 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.125004 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/
--rw-r--r--   0 runner    (1001) docker     (121)    26953 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/fse_compress.c
--rw-r--r--   0 runner    (1001) docker     (121)     7450 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/hist.c
--rw-r--r--   0 runner    (1001) docker     (121)     3450 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/hist.h
--rw-r--r--   0 runner    (1001) docker     (121)    38336 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/huf_compress.c
--rw-r--r--   0 runner    (1001) docker     (121)   223634 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress.c
--rw-r--r--   0 runner    (1001) docker     (121)    49821 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_internal.h
--rw-r--r--   0 runner    (1001) docker     (121)     6272 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_literals.c
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_literals.h
--rw-r--r--   0 runner    (1001) docker     (121)    19691 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_sequences.c
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_sequences.h
--rw-r--r--   0 runner    (1001) docker     (121)    43413 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_superblock.c
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_superblock.h
--rw-r--r--   0 runner    (1001) docker     (121)    20165 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_cwksp.h
--rw-r--r--   0 runner    (1001) docker     (121)    25304 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_double_fast.c
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_double_fast.h
--rw-r--r--   0 runner    (1001) docker     (121)    22335 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_fast.c
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_fast.h
--rw-r--r--   0 runner    (1001) docker     (121)    63392 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_lazy.c
--rw-r--r--   0 runner    (1001) docker     (121)     3593 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_lazy.h
--rw-r--r--   0 runner    (1001) docker     (121)    26840 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_ldm.c
--rw-r--r--   0 runner    (1001) docker     (121)     4400 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_ldm.h
--rw-r--r--   0 runner    (1001) docker     (121)    62552 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_opt.c
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_opt.h
--rw-r--r--   0 runner    (1001) docker     (121)    78240 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstdmt_compress.c
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstdmt_compress.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.125004 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/
--rw-r--r--   0 runner    (1001) docker     (121)    54982 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/huf_decompress.c
--rw-r--r--   0 runner    (1001) docker     (121)     9164 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_ddict.c
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_ddict.h
--rw-r--r--   0 runner    (1001) docker     (121)    80283 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress.c
--rw-r--r--   0 runner    (1001) docker     (121)    66784 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress_block.c
--rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress_block.h
--rw-r--r--   0 runner    (1001) docker     (121)     7906 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.125004 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/deprecated/
--rw-r--r--   0 runner    (1001) docker     (121)    11503 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff.h
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff_common.c
--rw-r--r--   0 runner    (1001) docker     (121)     5331 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff_compress.c
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff_decompress.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.125004 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/
--rw-r--r--   0 runner    (1001) docker     (121)    42503 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/cover.c
--rw-r--r--   0 runner    (1001) docker     (121)     5009 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/cover.h
--rw-r--r--   0 runner    (1001) docker     (121)    54649 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/divsufsort.c
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/divsufsort.h
--rw-r--r--   0 runner    (1001) docker     (121)    28256 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/fastcover.c
--rw-r--r--   0 runner    (1001) docker     (121)    44652 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/zdict.c
--rw-r--r--   0 runner    (1001) docker     (121)    18451 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/zdict.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.097004 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dll/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.125004 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dll/example/
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dll/example/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2953 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dll/example/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dll/example/build_package.bat
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dll/example/fullbench-dll.sln
--rw-r--r--   0 runner    (1001) docker     (121)    10105 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dll/example/fullbench-dll.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.129004 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)    13909 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_legacy.h
--rw-r--r--   0 runner    (1001) docker     (121)    71519 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v01.c
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v01.h
--rw-r--r--   0 runner    (1001) docker     (121)   128192 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v02.c
--rw-r--r--   0 runner    (1001) docker     (121)     3713 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v02.h
--rw-r--r--   0 runner    (1001) docker     (121)   114312 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v03.c
--rw-r--r--   0 runner    (1001) docker     (121)     3725 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v03.h
--rw-r--r--   0 runner    (1001) docker     (121)   135425 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v04.c
--rw-r--r--   0 runner    (1001) docker     (121)     6443 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v04.h
--rw-r--r--   0 runner    (1001) docker     (121)   156589 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v05.c
--rw-r--r--   0 runner    (1001) docker     (121)     7541 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v05.h
--rw-r--r--   0 runner    (1001) docker     (121)   166216 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v06.c
--rw-r--r--   0 runner    (1001) docker     (121)     8079 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v06.h
--rw-r--r--   0 runner    (1001) docker     (121)   185264 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v07.c
--rw-r--r--   0 runner    (1001) docker     (121)     8722 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v07.h
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/libzstd.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)   138334 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/zstd.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.129004 bcolz-zipline-1.2.6/c-blosc/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     4869 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/check_symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.129004 bcolz-zipline-1.2.6/c-blosc/tests/fuzz/
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/fuzz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/fuzz/fuzz_compress.c
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/fuzz/fuzz_decompress.c
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/fuzz/standalone.c
--rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/gcc-segfault-issue.c
--rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/print_versions.c
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_all.sh
--rw-r--r--   0 runner    (1001) docker     (121)     4771 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_api.c
--rw-r--r--   0 runner    (1001) docker     (121)     3974 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_bitshuffle_leftovers.c
--rw-r--r--   0 runner    (1001) docker     (121)     4213 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_common.h
--rw-r--r--   0 runner    (1001) docker     (121)     3972 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_compress_roundtrip.c
--rw-r--r--   0 runner    (1001) docker     (121)     4528 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_compress_roundtrip.csv
--rw-r--r--   0 runner    (1001) docker     (121)    10680 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_compressor.c
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_forksafe.c
--rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_getitem.c
--rw-r--r--   0 runner    (1001) docker     (121)     6701 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_getitem.csv
--rw-r--r--   0 runner    (1001) docker     (121)     5554 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_maxout.c
--rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_noinit.c
--rw-r--r--   0 runner    (1001) docker     (121)     2697 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_nolock.c
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_nthreads.c
--rw-r--r--   0 runner    (1001) docker     (121)     4027 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_shuffle_roundtrip_avx2.c
--rw-r--r--   0 runner    (1001) docker     (121)     5057 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_shuffle_roundtrip_avx2.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_shuffle_roundtrip_generic.c
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_shuffle_roundtrip_generic.csv
--rw-r--r--   0 runner    (1001) docker     (121)     4202 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_shuffle_roundtrip_sse2.c
--rw-r--r--   0 runner    (1001) docker     (121)     5057 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/c-blosc/tests/test_shuffle_roundtrip_sse2.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.129004 bcolz-zipline-1.2.6/conda.recipe/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/conda.recipe/conda_build_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/conda.recipe/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.097004 bcolz-zipline-1.2.6/continuous-integration/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.129004 bcolz-zipline-1.2.6/continuous-integration/appveyor/
--rw-r--r--   0 runner    (1001) docker     (121)     3114 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/continuous-integration/appveyor/install.ps1
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/continuous-integration/appveyor/run_with_env.cmd
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/coveralls_after_test_succes.sh
--rw-r--r--   0 runner    (1001) docker     (121)    66040 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/cpuinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.133004 bcolz-zipline-1.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     4586 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     3613 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/bcolz.png
--rw-r--r--   0 runner    (1001) docker     (121)     7595 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/defaults.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5790 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4509 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.133004 bcolz-zipline-1.2.6/docs/my_package/
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/my_package/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.133004 bcolz-zipline-1.2.6/docs/my_package/my_extension/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/my_package/my_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/my_package/my_extension/example_ext.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/my_package/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/my_package/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     4243 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/opt-tips.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2829 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4526 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (121)    67135 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/tutorial_carray.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    54488 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/tutorial_carray_memory_profile.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    29522 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/tutorial_ctable.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/docs/tutorials.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:23:40.133004 bcolz-zipline-1.2.6/examples/
--rw-r--r--   0 runner    (1001) docker     (121)    12033 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/examples/querying-ranges.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/makefile
--rw-r--r--   0 runner    (1001) docker     (121)     6688 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/persistence.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/requirements_rtfd.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-11-17 20:23:40.133004 bcolz-zipline-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5771 2022-11-17 20:23:25.000000 bcolz-zipline-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.362610 bcolz_zipline-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/.coverage
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.286610 bcolz_zipline-1.2.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.286610 bcolz_zipline-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/.github/workflows/build_conda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/.github/workflows/build_wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/.github/workflows/unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/ANNOUNCE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/DISK_FORMAT_v1.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.290610 bcolz_zipline-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/LICENSES/APPVEYOR-DEMO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/LICENSES/BCOLZ.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/LICENSES/BLOSC.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/LICENSES/FASTLZ.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/LICENSES/LZ4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/LICENSES/NUMPY.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/LICENSES/SNAPPY.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/LICENSES/STDINT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/LICENSES/ZLIB.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-14 05:43:55.362610 bcolz_zipline-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    41517 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/RELEASE_NOTES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/THANKS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/appveyor.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.294611 bcolz_zipline-1.2.9/bcolz/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/PythonHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 05:43:55.000000 bcolz_zipline-1.2.9/bcolz/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26656 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/arrayprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/carray_ext.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    97886 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/carray_ext.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/check_blosc_version.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/chunked_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51578 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/ctable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/definitions.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/py2help.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/py2help_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.294611 bcolz_zipline-1.2.9/bcolz/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/tests/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92292 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/tests/test_carray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/tests/test_carray_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94148 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/tests/test_ctable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31940 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/tests/test_ndcarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22635 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/toplevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bcolz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.362610 bcolz_zipline-1.2.9/bcolz_zipline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-14 05:43:55.000000 bcolz_zipline-1.2.9/bcolz_zipline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-05-14 05:43:55.000000 bcolz_zipline-1.2.9/bcolz_zipline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 05:43:55.000000 bcolz_zipline-1.2.9/bcolz_zipline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 05:43:54.000000 bcolz_zipline-1.2.9/bcolz_zipline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-14 05:43:55.000000 bcolz_zipline-1.2.9/bcolz_zipline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 05:43:55.000000 bcolz_zipline-1.2.9/bcolz_zipline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.302610 bcolz_zipline-1.2.9/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/arange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/column-iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/ctable-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/eval-profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/eval_and_replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/fromiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/iterblocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/large_carray.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1242137 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/multithreaded_copy.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/objpickles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/pandas-fromdataframe-strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/pandas-fromdataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/pandas-todataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/pytables-fromhdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/pytables-tohdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/whereblocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/zeros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench/zlib-vs-cblosc-zlib.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.302610 bcolz_zipline-1.2.9/bench_asv/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench_asv/README_asv.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench_asv/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.306610 bcolz_zipline-1.2.9/bench_asv/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench_asv/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench_asv/bench/arange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench_asv/bench/bench_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench_asv/bench/column_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/bench_asv/bench/concat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.306610 bcolz_zipline-1.2.9/c-blosc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/ANNOUNCE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/COMPILING_WITH_WHEELS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.310610 bcolz_zipline-1.2.9/c-blosc/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/LICENSES/BITSHUFFLE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/LICENSES/BLOSC.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/LICENSES/FASTLZ.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/LICENSES/LZ4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/LICENSES/SNAPPY.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/LICENSES/STDINT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/LICENSES/ZLIB.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6958 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/README_CHUNK_FORMAT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/README_THREADED.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    40487 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/RELEASE_NOTES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/THANKS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/THOUGHTS_FOR_2.0.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.310610 bcolz_zipline-1.2.9/c-blosc/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/bench/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/bench/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/bench/Makefile.mingw
+-rw-r--r--   0 runner    (1001) docker     (127)    18390 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/bench/bench.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/bench/plot-speeds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.314610 bcolz_zipline-1.2.9/c-blosc/blosc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/bitshuffle-avx2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/bitshuffle-avx2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/bitshuffle-generic.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/bitshuffle-generic.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16683 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/bitshuffle-sse2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/bitshuffle-sse2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/blosc-common.h
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/blosc-comp-features.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/blosc-export.h
+-rw-r--r--   0 runner    (1001) docker     (127)    69856 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/blosc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19570 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/blosc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26921 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/blosclz.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/blosclz.h
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/fastcopy.c
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/fastcopy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30871 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/shuffle-avx2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/shuffle-avx2.h
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/shuffle-generic.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/shuffle-generic.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25521 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/shuffle-sse2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/shuffle-sse2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17007 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/shuffle.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/shuffle.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.314610 bcolz_zipline-1.2.9/c-blosc/blosc/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/win32/pthread.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/win32/pthread.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc/win32/stdint-windows.h
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/blosc.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.314610 bcolz_zipline-1.2.9/c-blosc/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/cmake/FindLZ4.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/cmake/FindSnappy.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/cmake/FindZstd.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/code_of_conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.322610 bcolz_zipline-1.2.9/c-blosc/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26736 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.11.1-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    33610 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.11.1-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    32485 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.11.1-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)   199683 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.11.1-snappy.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    16176 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.11.1-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.11.1-zstd.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36256 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.14.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.14.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36263 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.14.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)   199855 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.14.0-snappy.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    20530 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.14.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.14.0-zstd.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    75152 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-blosclz-bitshuffle.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36256 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)   184228 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-lz4-bitshuffle.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36263 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    20530 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-zstd.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36349 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.3.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.3.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    31963 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.3.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)   199935 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.3.0-snappy.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    14956 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.3.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36394 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.7.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.7.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    31963 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.7.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)   199935 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.7.0-snappy.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    14956 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.7.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/compat/filegen.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.326610 bcolz_zipline-1.2.9/c-blosc/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/examples/many_compressors.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/examples/multithread.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/examples/noinit.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/examples/simple.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/examples/win-dynamic-linking.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.282611 bcolz_zipline-1.2.9/c-blosc/internal-complibs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.326610 bcolz_zipline-1.2.9/c-blosc/internal-complibs/lz4-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)   105087 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/lz4-1.9.3/lz4.c
+-rw-r--r--   0 runner    (1001) docker     (127)    40861 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/lz4-1.9.3/lz4.h
+-rw-r--r--   0 runner    (1001) docker     (127)    69010 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/lz4-1.9.3/lz4hc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20165 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/lz4-1.9.3/lz4hc.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.330610 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13174 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/crc32.c
+-rw-r--r--   0 runner    (1001) docker     (127)    30562 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/crc32.h
+-rw-r--r--   0 runner    (1001) docker     (127)    71476 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/deflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/deflate.h
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/gzclose.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/gzguts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16415 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/gzlib.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18694 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/gzread.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16199 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/gzwrite.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22709 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/infback.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inffast.c
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inffast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inffixed.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53512 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inflate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inftrees.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inftrees.h
+-rw-r--r--   0 runner    (1001) docker     (127)    44255 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/trees.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/trees.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/uncompr.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/zconf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    87883 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/zlib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/zutil.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/zutil.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.330610 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/BUCK
+-rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10106 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.338610 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    18198 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10157 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/cpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/debug.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/debug.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/entropy_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/error_private.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/error_private.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34578 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/fse.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/fse_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20216 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/huf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13930 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/mem.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/pool.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/pool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/threading.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/threading.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_deps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_errors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15880 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.342610 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/
+-rw-r--r--   0 runner    (1001) docker     (127)    26953 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/fse_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/hist.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/hist.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38336 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/huf_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)   223634 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    49821 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_literals.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_literals.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19691 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_sequences.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_sequences.h
+-rw-r--r--   0 runner    (1001) docker     (127)    43413 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_superblock.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_superblock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20165 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_cwksp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25304 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_double_fast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_double_fast.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22335 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_fast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_fast.h
+-rw-r--r--   0 runner    (1001) docker     (127)    63392 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_lazy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_lazy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26840 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_ldm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_ldm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    62552 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_opt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_opt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    78240 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstdmt_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstdmt_compress.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.342610 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/
+-rw-r--r--   0 runner    (1001) docker     (127)    54982 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/huf_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_ddict.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_ddict.h
+-rw-r--r--   0 runner    (1001) docker     (127)    80283 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    66784 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress_block.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress_block.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.342610 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff_decompress.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.346610 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/cover.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/cover.h
+-rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/divsufsort.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/divsufsort.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28256 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/fastcover.c
+-rw-r--r--   0 runner    (1001) docker     (127)    44652 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/zdict.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18451 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/zdict.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.282611 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dll/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.346610 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dll/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dll/example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dll/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dll/example/build_package.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dll/example/fullbench-dll.sln
+-rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dll/example/fullbench-dll.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.350610 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)    13909 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_legacy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    71519 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v01.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v01.h
+-rw-r--r--   0 runner    (1001) docker     (127)   128192 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v02.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v02.h
+-rw-r--r--   0 runner    (1001) docker     (127)   114312 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v03.h
+-rw-r--r--   0 runner    (1001) docker     (127)   135425 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v04.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v04.h
+-rw-r--r--   0 runner    (1001) docker     (127)   156589 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v05.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v05.h
+-rw-r--r--   0 runner    (1001) docker     (127)   166216 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v06.h
+-rw-r--r--   0 runner    (1001) docker     (127)   185264 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v07.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v07.h
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/libzstd.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)   138334 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/zstd.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.354610 bcolz_zipline-1.2.9/c-blosc/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/check_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.354610 bcolz_zipline-1.2.9/c-blosc/tests/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/fuzz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/fuzz/fuzz_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/fuzz/fuzz_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/fuzz/standalone.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/gcc-segfault-issue.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/print_versions.c
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_all.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_bitshuffle_leftovers.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_compress_roundtrip.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_compress_roundtrip.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_compressor.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_forksafe.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_getitem.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_getitem.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_maxout.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_noinit.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_nolock.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_nthreads.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_shuffle_roundtrip_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_shuffle_roundtrip_avx2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_shuffle_roundtrip_generic.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_shuffle_roundtrip_generic.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_shuffle_roundtrip_sse2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/c-blosc/tests/test_shuffle_roundtrip_sse2.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.354610 bcolz_zipline-1.2.9/conda.recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/conda.recipe/conda_build_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/conda.recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.282611 bcolz_zipline-1.2.9/continuous-integration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.354610 bcolz_zipline-1.2.9/continuous-integration/appveyor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/continuous-integration/appveyor/install.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/continuous-integration/appveyor/run_with_env.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/coveralls_after_test_succes.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    66040 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/cpuinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.358610 bcolz_zipline-1.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/bcolz.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/defaults.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.358610 bcolz_zipline-1.2.9/docs/my_package/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/my_package/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.358610 bcolz_zipline-1.2.9/docs/my_package/my_extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/my_package/my_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/my_package/my_extension/example_ext.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/my_package/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/my_package/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/opt-tips.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    67135 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/tutorial_carray.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    54488 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/tutorial_carray_memory_profile.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    29522 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/tutorial_ctable.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/docs/tutorials.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:43:55.358610 bcolz_zipline-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    12033 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/examples/querying-ranges.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/persistence.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/requirements_rtfd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 05:43:55.362610 bcolz_zipline-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-05-14 05:43:47.000000 bcolz_zipline-1.2.9/setup.py
```

### Comparing `bcolz-zipline-1.2.6/.coverage` & `bcolz_zipline-1.2.9/.coverage`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/.github/workflows/build_conda.yml` & `bcolz_zipline-1.2.9/.github/workflows/build_conda.yml`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,18 @@
         run: |
           xcode-select --print-path
           xcode-select --print-path | ls
           xcrun --show-sdk-path
           xcrun --show-sdk-path | ls
 
       - name: Checkout bcolz
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Setup miniconda3
-        uses: conda-incubator/setup-miniconda@v2
+        uses: conda-incubator/setup-miniconda@v3
         with:
           miniconda-version: "latest"
           auto-update-conda: true
           mamba-version: "*"
           python-version: ${{ matrix.python }}
           activate-environment: recipe
           channels: conda-forge, defaults, anaconda
@@ -66,35 +66,35 @@
 
       - name: activate uploader
         # address broken client under py3.9
         if: ${{ (matrix.python == '3.9') || (matrix.python == '3.10') }}
         run: conda activate up
 
       - name: store windows result
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         if: ${{ matrix.os == 'windows-latest' }}
         with:
           path: win-64/*.tar.bz2
 
       - name: upload windows
         if: ${{ matrix.os == 'windows-latest' }}
         run: anaconda upload -l main -u ml4t win-64/*.tar.bz2
 
       - name: store linux result
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         if: ${{ matrix.os == 'ubuntu-latest' }}
         with:
           path: linux-64/*.tar.bz2
 
       - name: upload linux
         if: ${{ matrix.os  == 'ubuntu-latest' }}
         run: anaconda upload -l main -u ml4t linux-64/*.tar.bz2
 
       - name: store macos result
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         if: ${{ matrix.os == 'macos-latest' }}
         with:
           path: osx-64/*.tar.bz2
 
       - name: upload macos
         if: ${{ matrix.os == 'macos-latest' }}
-        run: anaconda upload -l main -u ml4t osx-64/*.tar.bz2
+        run: anaconda upload -l main -u ml4t osx-64/*.tar.bz2
```

### Comparing `bcolz-zipline-1.2.6/.github/workflows/build_wheels.yml` & `bcolz_zipline-1.2.9/.github/workflows/build_wheels.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,104 +1,109 @@
 name: Build Wheels
 
 on:
   workflow_dispatch:
     inputs:
       target:
+        type: choice
         description: 'Package Index'
         required: true
-        default: 'TESTPYPI'
+        default: 'PYPI'
+        options: [ 'TESTPYPI', 'PYPI' ]
   release:
     types: qq
       - published
 
 jobs:
   build_wheels:
-    name: Wheels for py${{ matrix.python }} on ${{ matrix.os }} using ${{ matrix.manylinux_image }}
+    name: Wheels for py${{ matrix.python }} on ${{ matrix.os }} - upload to ${{github.event.inputs.target}}
     runs-on: ${{ matrix.os }}
 
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest , windows-latest, macos-latest ]
-        python: [ 37, 38, 39, '310', '311' ]
-        arch: [ auto ]
+        python: [ 38, 39, '310', '311' , '312']
+        arch: [ auto64 ]
 
     steps:
       - name: Checkout bcolz
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           submodules: 'recursive'
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: '3.10'
 
-      - name: Wheels for macOS / Linux
+      - name: Wheels macOS / Linux
         if: runner.os != 'Windows'
-        uses: pypa/cibuildwheel@v2.11.2
+        uses: pypa/cibuildwheel@v2.18.0
         env:
           CIBW_BEFORE_ALL_MACOS: brew install hdf5 c-blosc
-          CIBW_SKIP: '*-manylinux*_i686'
           CIBW_ARCHS_LINUX: ${{ matrix.arch }}
+          CIBW_ARCHS_MACOS: x86_64 arm64
           CIBW_BUILD: "cp${{ matrix.python }}-*"
+          CIBW_SKIP: "*-musllinux_*"
           CIBW_ENVIRONMENT_LINUX: DISABLE_BCOLZ_AVX2=true
-          CIBW_ENVIRONMENT_MACOS: MACOSX_DEPLOYMENT_TARGET=10.15 DISABLE_BCOLZ_AVX2=true
+          CIBW_ENVIRONMENT_MACOS: MACOSX_DEPLOYMENT_TARGET=10.15 DISABLE_BCOLZ_AVX2=true DISABLE_BCOLZ_SSE2=true
 
       - name: Install MSVC amd64
         uses: ilammy/msvc-dev-cmd@v1
         with:
           arch: amd64
 
-      - name: Build wheels windows
+      - name: Wheels Windows
         if: runner.os == 'Windows'
-        uses: pypa/cibuildwheel@v2.11.2
+        uses: pypa/cibuildwheel@v2.18.0
         env:
-          CIBW_BUILD: 'cp38-win_amd64 cp39-win_amd64 cp310-win_amd64 cp311-win_amd64'
+          CIBW_BUILD: 'cp38-win_amd64 cp39-win_amd64 cp310-win_amd64 cp311-win_amd64 cp312-win_amd64'
           CIBW_ENVIRONMENT: DISABLE_BCOLZ_AVX2=true DISABLE_BCOLZ_SSE2=true
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           path: wheelhouse/*.whl
 
   build_sdist:
     name: Build source distribution
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
           python-version: '3.10'
 
       - name: Build sdist
         run: pipx run --spec build pyproject-build --sdist
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           path: dist/*.tar.gz
 
   upload_pypi:
+    name: Upload to ${{github.event.inputs.target}}
     needs: [ build_wheels, build_sdist ]
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
 
-      - name: publish to testpypi
+      - name: Publish to PyPI
+        if: ${{ github.event.inputs.target  == 'PYPI' && startsWith(github.ref, 'refs/tags' ) }}
         uses: pypa/gh-action-pypi-publish@release/v1
-        if: ${{ github.event.inputs.target }} == 'TESTPYPI'
         with:
           user: __token__
-          password: ${{ secrets.PYPITEST_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
-      - name: publish to pypi
+          password: ${{ secrets.PYPI_TOKEN }}
+
+      - name: Publish to PyPI - Test
+        if: ${{ github.event.inputs.target  == 'TESTPYPI' }}
         uses: pypa/gh-action-pypi-publish@release/v1
-        if: ${{ github.event.inputs.target }} == 'PYPI' || (github.event_name == 'release' && github.event.action == 'published')
         with:
           user: __token__
-          password: ${{ secrets.PYPI_TOKEN }}
+          password: ${{ secrets.PYPITEST_TOKEN }}
+          repository_url: https://test.pypi.org/legacy/
```

### Comparing `bcolz-zipline-1.2.6/.github/workflows/unit_tests.yml` & `bcolz_zipline-1.2.9/.github/workflows/unit_tests.yml`

 * *Files 26% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 jobs:
   build:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest, windows-latest, macos-latest ]
-        python-version: [ 3.7, 3.8, 3.9, '3.10', '3.11' ]
+        python-version: [ 3.8, 3.9, '3.10', '3.11' , '3.12' ]
 
     steps:
       - name: Checkout bcolz-zipline
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install bcolz
         run: |
           python -VV
           python -m pip install --upgrade pip wheel setuptools
@@ -39,8 +39,8 @@
 
       - name: Run tests
         run: pytest --cov
 
       - name: Upload coverage data to coveralls.io
         run: coveralls --service=github
         env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `bcolz-zipline-1.2.6/DISK_FORMAT_v1.rst` & `bcolz_zipline-1.2.9/DISK_FORMAT_v1.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/LICENSES/APPVEYOR-DEMO.txt` & `bcolz_zipline-1.2.9/LICENSES/APPVEYOR-DEMO.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/LICENSES/BCOLZ.txt` & `bcolz_zipline-1.2.9/LICENSES/BCOLZ.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/LICENSES/BLOSC.txt` & `bcolz_zipline-1.2.9/LICENSES/BLOSC.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/LICENSES/FASTLZ.txt` & `bcolz_zipline-1.2.9/LICENSES/FASTLZ.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/LICENSES/LZ4.txt` & `bcolz_zipline-1.2.9/LICENSES/LZ4.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/LICENSES/NUMPY.txt` & `bcolz_zipline-1.2.9/LICENSES/NUMPY.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/LICENSES/SNAPPY.txt` & `bcolz_zipline-1.2.9/LICENSES/SNAPPY.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/LICENSES/STDINT.txt` & `bcolz_zipline-1.2.9/LICENSES/STDINT.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/LICENSES/ZLIB.txt` & `bcolz_zipline-1.2.9/LICENSES/ZLIB.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/PKG-INFO` & `bcolz_zipline-1.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcolz-zipline
-Version: 1.2.6
+Version: 1.2.9
 Summary: Columnar and compressed data containers.
 Author: Francesc Alted
 Author-email: francesc@blosc.org
 Maintainer: Francesc Alted
 Maintainer-email: francesc@blosc.org
 License: Copyright Notice and Statement for bcolz Software Library and Utilities:
         
@@ -49,23 +49,31 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.16
 Provides-Extra: optional
+Requires-Dist: numexpr>=2.5.2; extra == "optional"
+Requires-Dist: dask>=0.9.0; extra == "optional"
+Requires-Dist: pandas; extra == "optional"
+Requires-Dist: tables; extra == "optional"
 Provides-Extra: test
+Requires-Dist: pytest>=6.2.3; extra == "test"
+Requires-Dist: pytest-cov>=2.11.1; extra == "test"
+Requires-Dist: coveralls==3.0.1; extra == "test"
 
 # bcolz: columnar and compressed data containers
 
 <p align="center">
     <a href="https://gitter.im/Blosc/bcolz?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge" target="_blank">
         <img alt="Gitter" src="https://badges.gitter.im/Blosc/bcolz.svg" />
     </a>
@@ -114,17 +122,17 @@
 Furthermore, columnar means that the tabular datasets are stored column-wise order, and this turns out to offer better opportunities to improve compression ratio. This is because data tends to expose more similarity in elements that sit in the same column rather than those in the same row, so compressors generally do a much better job when data is aligned in such column-wise order. In addition, when you have to deal with tables with a large number of columns and your operations only involve some
 of them, a columnar-wise storage tends to be much more effective because minimizes the amount of data that travels to CPU caches.
 
 So, the ultimate goal for bcolz is not only reducing the memory needs of large arrays/tables, but also making bcolz operations to go faster than using a traditional data container like those in NumPy or Pandas. That is actually already the case in some real-life scenarios (see the notebook above) but that will become pretty more noticeable in combination with forthcoming, faster CPUs integrating more cores and wider vector units.
 
 ## Requisites
 
-- Python >= 3.7
+- Python >= 3.8
 - NumPy >= 1.16.5, <1.23 (1.23 is not supported yet)
-- Cython >= 0.22 (just for compiling the beast)
+- Cython >= 0.22 (Python 3.12 > 3) (just for compiling the beast)
 - C-Blosc >= 1.8.0 (optional, as the internal Blosc will be used by default)
 
 Optional:
 
 - numexpr >= 2.5.2
 - dask >= 0.9.0
 - pandas
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bcolz-zipline Version: 1.2.6 Summary: Columnar and
+Metadata-Version: 2.1 Name: bcolz-zipline Version: 1.2.9 Summary: Columnar and
 compressed data containers. Author: Francesc Alted Author-email:
 francesc@blosc.org Maintainer: Francesc Alted Maintainer-email:
 francesc@blosc.org License: Copyright Notice and Statement for bcolz Software
 Library and Utilities: Copyright (c) 2010-2011 by Francesc Alted Copyright (c)
 2012 by Continuum Analytics Copyright (c) 2013 by Francesc Alted Copyright (c)
 2014-2018 by Francesc Alted and the bcolz contributors All rights reserved.
 Redistribution and use in source and binary forms, with or without
@@ -27,20 +27,25 @@
 github.com/stefan-jansen/bcolz-zipline Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Operating System :: Microsoft ::
 Windows Classifier: Operating System :: Unix Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown Provides-Extra: optional Provides-Extra: test #
-bcolz: columnar and compressed data containers
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Requires-Python: >=3.7 Description-
+Content-Type: text/markdown Requires-Dist: numpy>=1.16 Provides-Extra: optional
+Requires-Dist: numexpr>=2.5.2; extra == "optional" Requires-Dist: dask>=0.9.0;
+extra == "optional" Requires-Dist: pandas; extra == "optional" Requires-Dist:
+tables; extra == "optional" Provides-Extra: test Requires-Dist: pytest>=6.2.3;
+extra == "test" Requires-Dist: pytest-cov>=2.11.1; extra == "test" Requires-
+Dist: coveralls==3.0.1; extra == "test" # bcolz: columnar and compressed data
+containers
    _[_G_i_t_t_e_r_]_[_V_e_r_s_i_o_n_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_][GitHub Workflow Status]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]
 [GitHub Workflow Status]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:_ _B_S_D_]_[_T_w_i_t_t_e_r_:_ _@_m_l_4_t_]
                                     _[_B_l_o_s_c_]
                         _[_h_t_t_p_s_:_/_/_i_m_g_u_r_._c_o_m_/_g_8_e_m_k_E_Z_._p_n_g_]
 bcolz provides columnar, chunked data containers that can be compressed either
 in-memory and on-disk. Column storage allows for efficiently querying tables,
 as well as for cheap column addition and removal. It is based on [NumPy](http:/
@@ -78,27 +83,27 @@
 them, a columnar-wise storage tends to be much more effective because minimizes
 the amount of data that travels to CPU caches. So, the ultimate goal for bcolz
 is not only reducing the memory needs of large arrays/tables, but also making
 bcolz operations to go faster than using a traditional data container like
 those in NumPy or Pandas. That is actually already the case in some real-life
 scenarios (see the notebook above) but that will become pretty more noticeable
 in combination with forthcoming, faster CPUs integrating more cores and wider
-vector units. ## Requisites - Python >= 3.7 - NumPy >= 1.16.5, <1.23 (1.23 is
-not supported yet) - Cython >= 0.22 (just for compiling the beast) - C-Blosc >=
-1.8.0 (optional, as the internal Blosc will be used by default) Optional: -
-numexpr >= 2.5.2 - dask >= 0.9.0 - pandas - tables (pytables) ## Installing as
-wheel There are wheels for Linux and Mac OS X that you can install with
-```python pip install bcolz-zipline ``` Then also install NumPy with and test
-your installation with ```python python -c 'import bcolz;bcolz.test()' ``` ##
-Building There are different ways to compile bcolz, depending on whether you
-want to link with an already installed Blosc library or not. ### Compiling with
-an installed Blosc library (recommended) Python and Blosc-powered extensions
-have a difficult relationship when compiled using GCC, so this is why using an
-external C-Blosc library is recommended for maximum performance (for details,
-see
+vector units. ## Requisites - Python >= 3.8 - NumPy >= 1.16.5, <1.23 (1.23 is
+not supported yet) - Cython >= 0.22 (Python 3.12 > 3) (just for compiling the
+beast) - C-Blosc >= 1.8.0 (optional, as the internal Blosc will be used by
+default) Optional: - numexpr >= 2.5.2 - dask >= 0.9.0 - pandas - tables
+(pytables) ## Installing as wheel There are wheels for Linux and Mac OS X that
+you can install with ```python pip install bcolz-zipline ``` Then also install
+NumPy with and test your installation with ```python python -c 'import
+bcolz;bcolz.test()' ``` ## Building There are different ways to compile bcolz,
+depending on whether you want to link with an already installed Blosc library
+or not. ### Compiling with an installed Blosc library (recommended) Python and
+Blosc-powered extensions have a difficult relationship when compiled using GCC,
+so this is why using an external C-Blosc library is recommended for maximum
+performance (for details, see
 github.com/Blosc/python-blosc/issues/110>). Go to
 github.com/Blosc/c-blosc/releases> and download and install the C-Blosc
 library. Then, you can tell bcolz where is the C-Blosc library in a couple of
 ways: Using an environment variable: ``` {.sourceCode .console} $ BLOSC_DIR=/
 usr/local (or "set BLOSC_DIR=\blosc" on Win) $ export BLOSC_DIR (not needed on
 Win) $ python setup.py build_ext --inplace ``` Using a flag: ``` {.sourceCode
 .console} $ python setup.py build_ext --inplace --blosc=/usr/local ``` ###
```

### Comparing `bcolz-zipline-1.2.6/README.md` & `bcolz_zipline-1.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,17 @@
 Furthermore, columnar means that the tabular datasets are stored column-wise order, and this turns out to offer better opportunities to improve compression ratio. This is because data tends to expose more similarity in elements that sit in the same column rather than those in the same row, so compressors generally do a much better job when data is aligned in such column-wise order. In addition, when you have to deal with tables with a large number of columns and your operations only involve some
 of them, a columnar-wise storage tends to be much more effective because minimizes the amount of data that travels to CPU caches.
 
 So, the ultimate goal for bcolz is not only reducing the memory needs of large arrays/tables, but also making bcolz operations to go faster than using a traditional data container like those in NumPy or Pandas. That is actually already the case in some real-life scenarios (see the notebook above) but that will become pretty more noticeable in combination with forthcoming, faster CPUs integrating more cores and wider vector units.
 
 ## Requisites
 
-- Python >= 3.7
+- Python >= 3.8
 - NumPy >= 1.16.5, <1.23 (1.23 is not supported yet)
-- Cython >= 0.22 (just for compiling the beast)
+- Cython >= 0.22 (Python 3.12 > 3) (just for compiling the beast)
 - C-Blosc >= 1.8.0 (optional, as the internal Blosc will be used by default)
 
 Optional:
 
 - numexpr >= 2.5.2
 - dask >= 0.9.0
 - pandas
```

#### html2text {}

```diff
@@ -40,27 +40,27 @@
 them, a columnar-wise storage tends to be much more effective because minimizes
 the amount of data that travels to CPU caches. So, the ultimate goal for bcolz
 is not only reducing the memory needs of large arrays/tables, but also making
 bcolz operations to go faster than using a traditional data container like
 those in NumPy or Pandas. That is actually already the case in some real-life
 scenarios (see the notebook above) but that will become pretty more noticeable
 in combination with forthcoming, faster CPUs integrating more cores and wider
-vector units. ## Requisites - Python >= 3.7 - NumPy >= 1.16.5, <1.23 (1.23 is
-not supported yet) - Cython >= 0.22 (just for compiling the beast) - C-Blosc >=
-1.8.0 (optional, as the internal Blosc will be used by default) Optional: -
-numexpr >= 2.5.2 - dask >= 0.9.0 - pandas - tables (pytables) ## Installing as
-wheel There are wheels for Linux and Mac OS X that you can install with
-```python pip install bcolz-zipline ``` Then also install NumPy with and test
-your installation with ```python python -c 'import bcolz;bcolz.test()' ``` ##
-Building There are different ways to compile bcolz, depending on whether you
-want to link with an already installed Blosc library or not. ### Compiling with
-an installed Blosc library (recommended) Python and Blosc-powered extensions
-have a difficult relationship when compiled using GCC, so this is why using an
-external C-Blosc library is recommended for maximum performance (for details,
-see
+vector units. ## Requisites - Python >= 3.8 - NumPy >= 1.16.5, <1.23 (1.23 is
+not supported yet) - Cython >= 0.22 (Python 3.12 > 3) (just for compiling the
+beast) - C-Blosc >= 1.8.0 (optional, as the internal Blosc will be used by
+default) Optional: - numexpr >= 2.5.2 - dask >= 0.9.0 - pandas - tables
+(pytables) ## Installing as wheel There are wheels for Linux and Mac OS X that
+you can install with ```python pip install bcolz-zipline ``` Then also install
+NumPy with and test your installation with ```python python -c 'import
+bcolz;bcolz.test()' ``` ## Building There are different ways to compile bcolz,
+depending on whether you want to link with an already installed Blosc library
+or not. ### Compiling with an installed Blosc library (recommended) Python and
+Blosc-powered extensions have a difficult relationship when compiled using GCC,
+so this is why using an external C-Blosc library is recommended for maximum
+performance (for details, see
 github.com/Blosc/python-blosc/issues/110>). Go to
 github.com/Blosc/c-blosc/releases> and download and install the C-Blosc
 library. Then, you can tell bcolz where is the C-Blosc library in a couple of
 ways: Using an environment variable: ``` {.sourceCode .console} $ BLOSC_DIR=/
 usr/local (or "set BLOSC_DIR=\blosc" on Win) $ export BLOSC_DIR (not needed on
 Win) $ python setup.py build_ext --inplace ``` Using a flag: ``` {.sourceCode
 .console} $ python setup.py build_ext --inplace --blosc=/usr/local ``` ###
```

### Comparing `bcolz-zipline-1.2.6/appveyor.yml` & `bcolz_zipline-1.2.9/appveyor.yml`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/__init__.py` & `bcolz_zipline-1.2.9/bcolz/__init__.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/arrayprint.py` & `bcolz_zipline-1.2.9/bcolz/arrayprint.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/attrs.py` & `bcolz_zipline-1.2.9/bcolz/attrs.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/carray_ext.pxd` & `bcolz_zipline-1.2.9/bcolz/carray_ext.pxd`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/carray_ext.pyx` & `bcolz_zipline-1.2.9/bcolz/carray_ext.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -585,15 +585,15 @@
 
     def __str__(self):
         """Represent the chunk as an string."""
         return str(self[:])
 
     def __repr__(self):
         """Represent the chunk as an string, with additional info."""
-        cratio = self.nbytes / float(self.cbytes)
+        cratio = self.nbytes // float(self.cbytes)
         fullrepr = "chunk(%s)  nbytes: %d; cbytes: %d; ratio: %.2f\n%r" % \
                    (self.dtype, self.nbytes, self.cbytes, cratio, str(self))
         return fullrepr
 
 
 cdef create_bloscpack_header(nchunks=None, format_version=FORMAT_VERSION):
     """Create the bloscpack header string.
@@ -1169,15 +1169,15 @@
             # Try a guess
             try:
                 expectedlen = len(array_)
             except TypeError:
                 raise NotImplementedError(
                     "creating carrays from scalar objects is not supported")
         try:
-            self.expectedlen = expectedlen
+            self.expectedlen = <long> expectedlen
         except OverflowError:
             raise OverflowError(
                 "The size cannot be larger than 2**31 on 32-bit platforms")
         if chunklen is None:
             # Try a guess
             chunksize = utils.calc_chunksize(
                 (expectedlen * atomsize) / float(_MB))
@@ -1540,15 +1540,15 @@
         if nitems <= 0:
             self.resize(self.len - nitems)
             return
 
         atomsize = self.atomsize
         chunks = self.chunks
         leftover = self.leftover
-        bsize = nitems * atomsize
+        bsize = <int> nitems * atomsize
         cbytes = 0
 
         # Check if items belong to the last chunk
         if (leftover - bsize) > 0:
             # Just update leftover counter
             leftover -= bsize
         else:
@@ -1644,19 +1644,19 @@
         isize = np.prod(ishape)
 
         # Check for -1 in newshape
         if -1 in newshape:
             if newshape.count(-1) > 1:
                 raise ValueError("only one shape dimension can be -1")
             pos = newshape.index(-1)
-            osize = np.prod(newshape[:pos] + newshape[pos + 1:])
+            osize = <int> np.prod(newshape[:pos] + newshape[pos + 1:])
             if isize == 0:
                 newshape = newshape[:pos] + (0,) + newshape[pos + 1:]
             else:
-                newshape = newshape[:pos] + (isize / osize,) + newshape[
+                newshape = newshape[:pos] + (isize // osize,) + newshape[
                                                                pos + 1:]
             newsize = np.prod(newshape)
 
         # Check shape compatibility
         if isize != newsize:
             raise ValueError(
                 "`newshape` is not compatible with the current one")
@@ -1678,15 +1678,15 @@
             rootdir = None
 
         # Create the final container and fill it
         out = carray([], dtype=newdtype, cparams=self.cparams,
                        expectedlen=newlen,
                        rootdir=rootdir, mode='w')
         if newlen < ilen:
-            rsize = isize / newlen
+            rsize = isize // newlen
             for i from 0 <= i < newlen:
                 out.append(
                     self[i * rsize:(i + 1) * rsize].reshape(newdtype.shape))
         else:
             for i from 0 <= i < ilen:
                 out.append(self[i].reshape(-1))
         out.flush()
@@ -2030,16 +2030,16 @@
             return self._getitem_object(start, stop, step)
 
         # Fill it from data in chunks
         nwrow = 0
         nchunks = <npy_intp> cython.cdiv(self._nbytes, self._chunksize)
         if self.leftover > 0:
             nchunks += 1
-        first_chunk = <npy_intp> cython.cdiv(start, self.chunklen)
-        last_chunk = <npy_intp> cython.cdiv(stop, self.chunklen) + 1
+        first_chunk = <npy_intp> <int> cython.cdiv(start, self.chunklen)
+        last_chunk = <npy_intp> <int> cython.cdiv(stop, self.chunklen) + 1
         last_chunk = min(last_chunk, nchunks)
         for nchunk from first_chunk <= nchunk < last_chunk:
             # Compute start & stop for each block
             startb, stopb, blen = clip_chunk(nchunk, chunklen, start, stop,
                                              step)
             if blen == 0:
                 continue
@@ -2196,16 +2196,16 @@
 
         # Fill it from data in chunks
         nwrow = 0
         chunklen = self._chunklen
         nchunks = <npy_intp> cython.cdiv(self._nbytes, self._chunksize)
         if self.leftover > 0:
             nchunks += 1
-        first_chunk = <npy_intp> cython.cdiv(start, self.chunklen)
-        last_chunk = <npy_intp> cython.cdiv(stop, self.chunklen) + 1
+        first_chunk = <npy_intp> <int> cython.cdiv(start, self.chunklen)
+        last_chunk = <npy_intp> <int> cython.cdiv(stop, self.chunklen) + 1
         last_chunk = min(last_chunk, nchunks)
         for nchunk from first_chunk <= nchunk < last_chunk:
             # Compute start & stop for each block
             startb, stopb, blen = clip_chunk(nchunk, chunklen, start, stop,
                                              step)
             if blen == 0:
                 continue
```

### Comparing `bcolz-zipline-1.2.6/bcolz/chunked_eval.py` & `bcolz_zipline-1.2.9/bcolz/chunked_eval.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/ctable.py` & `bcolz_zipline-1.2.9/bcolz/ctable.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/defaults.py` & `bcolz_zipline-1.2.9/bcolz/defaults.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/definitions.pxd` & `bcolz_zipline-1.2.9/bcolz/definitions.pxd`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/py2help.py` & `bcolz_zipline-1.2.9/bcolz/py2help.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/tests/all.py` & `bcolz_zipline-1.2.9/bcolz/tests/all.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/tests/common.py` & `bcolz_zipline-1.2.9/bcolz/tests/common.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/tests/test_attrs.py` & `bcolz_zipline-1.2.9/bcolz/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/tests/test_carray.py` & `bcolz_zipline-1.2.9/bcolz/tests/test_carray.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/tests/test_carray_objects.py` & `bcolz_zipline-1.2.9/bcolz/tests/test_carray_objects.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/tests/test_ctable.py` & `bcolz_zipline-1.2.9/bcolz/tests/test_ctable.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/tests/test_ndcarray.py` & `bcolz_zipline-1.2.9/bcolz/tests/test_ndcarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -649,15 +649,15 @@
         # print "b->", `b`
         assert_array_equal(a, b, "Arrays are not equal")
 
     def test00c(self):
         """Testing `reshape()` (unidim -> ndim, -1 in newshape (II))"""
         a = np.ones((3, 4), dtype="i4")
         b = bcolz.ones(12, dtype="i4").reshape((3, -1))
-        # print "b->", `b`
+        # print("b->", b)
         assert_array_equal(a, b, "Arrays are not equal")
 
     def test01(self):
         """Testing `reshape()` (ndim -> unidim)"""
         a = np.ones(12, dtype="i4")
         c = bcolz.ones(12, dtype="i4").reshape((3, 4))
         b = c.reshape(12)
```

### Comparing `bcolz-zipline-1.2.6/bcolz/tests/test_queries.py` & `bcolz_zipline-1.2.9/bcolz/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/toplevel.py` & `bcolz_zipline-1.2.9/bcolz/toplevel.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz/utils.py` & `bcolz_zipline-1.2.9/bcolz/utils.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bcolz_zipline.egg-info/PKG-INFO` & `bcolz_zipline-1.2.9/bcolz_zipline.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcolz-zipline
-Version: 1.2.6
+Version: 1.2.9
 Summary: Columnar and compressed data containers.
 Author: Francesc Alted
 Author-email: francesc@blosc.org
 Maintainer: Francesc Alted
 Maintainer-email: francesc@blosc.org
 License: Copyright Notice and Statement for bcolz Software Library and Utilities:
         
@@ -49,23 +49,31 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.16
 Provides-Extra: optional
+Requires-Dist: numexpr>=2.5.2; extra == "optional"
+Requires-Dist: dask>=0.9.0; extra == "optional"
+Requires-Dist: pandas; extra == "optional"
+Requires-Dist: tables; extra == "optional"
 Provides-Extra: test
+Requires-Dist: pytest>=6.2.3; extra == "test"
+Requires-Dist: pytest-cov>=2.11.1; extra == "test"
+Requires-Dist: coveralls==3.0.1; extra == "test"
 
 # bcolz: columnar and compressed data containers
 
 <p align="center">
     <a href="https://gitter.im/Blosc/bcolz?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge" target="_blank">
         <img alt="Gitter" src="https://badges.gitter.im/Blosc/bcolz.svg" />
     </a>
@@ -114,17 +122,17 @@
 Furthermore, columnar means that the tabular datasets are stored column-wise order, and this turns out to offer better opportunities to improve compression ratio. This is because data tends to expose more similarity in elements that sit in the same column rather than those in the same row, so compressors generally do a much better job when data is aligned in such column-wise order. In addition, when you have to deal with tables with a large number of columns and your operations only involve some
 of them, a columnar-wise storage tends to be much more effective because minimizes the amount of data that travels to CPU caches.
 
 So, the ultimate goal for bcolz is not only reducing the memory needs of large arrays/tables, but also making bcolz operations to go faster than using a traditional data container like those in NumPy or Pandas. That is actually already the case in some real-life scenarios (see the notebook above) but that will become pretty more noticeable in combination with forthcoming, faster CPUs integrating more cores and wider vector units.
 
 ## Requisites
 
-- Python >= 3.7
+- Python >= 3.8
 - NumPy >= 1.16.5, <1.23 (1.23 is not supported yet)
-- Cython >= 0.22 (just for compiling the beast)
+- Cython >= 0.22 (Python 3.12 > 3) (just for compiling the beast)
 - C-Blosc >= 1.8.0 (optional, as the internal Blosc will be used by default)
 
 Optional:
 
 - numexpr >= 2.5.2
 - dask >= 0.9.0
 - pandas
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bcolz-zipline Version: 1.2.6 Summary: Columnar and
+Metadata-Version: 2.1 Name: bcolz-zipline Version: 1.2.9 Summary: Columnar and
 compressed data containers. Author: Francesc Alted Author-email:
 francesc@blosc.org Maintainer: Francesc Alted Maintainer-email:
 francesc@blosc.org License: Copyright Notice and Statement for bcolz Software
 Library and Utilities: Copyright (c) 2010-2011 by Francesc Alted Copyright (c)
 2012 by Continuum Analytics Copyright (c) 2013 by Francesc Alted Copyright (c)
 2014-2018 by Francesc Alted and the bcolz contributors All rights reserved.
 Redistribution and use in source and binary forms, with or without
@@ -27,20 +27,25 @@
 github.com/stefan-jansen/bcolz-zipline Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Operating System :: Microsoft ::
 Windows Classifier: Operating System :: Unix Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown Provides-Extra: optional Provides-Extra: test #
-bcolz: columnar and compressed data containers
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Requires-Python: >=3.7 Description-
+Content-Type: text/markdown Requires-Dist: numpy>=1.16 Provides-Extra: optional
+Requires-Dist: numexpr>=2.5.2; extra == "optional" Requires-Dist: dask>=0.9.0;
+extra == "optional" Requires-Dist: pandas; extra == "optional" Requires-Dist:
+tables; extra == "optional" Provides-Extra: test Requires-Dist: pytest>=6.2.3;
+extra == "test" Requires-Dist: pytest-cov>=2.11.1; extra == "test" Requires-
+Dist: coveralls==3.0.1; extra == "test" # bcolz: columnar and compressed data
+containers
    _[_G_i_t_t_e_r_]_[_V_e_r_s_i_o_n_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_][GitHub Workflow Status]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]
 [GitHub Workflow Status]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:_ _B_S_D_]_[_T_w_i_t_t_e_r_:_ _@_m_l_4_t_]
                                     _[_B_l_o_s_c_]
                         _[_h_t_t_p_s_:_/_/_i_m_g_u_r_._c_o_m_/_g_8_e_m_k_E_Z_._p_n_g_]
 bcolz provides columnar, chunked data containers that can be compressed either
 in-memory and on-disk. Column storage allows for efficiently querying tables,
 as well as for cheap column addition and removal. It is based on [NumPy](http:/
@@ -78,27 +83,27 @@
 them, a columnar-wise storage tends to be much more effective because minimizes
 the amount of data that travels to CPU caches. So, the ultimate goal for bcolz
 is not only reducing the memory needs of large arrays/tables, but also making
 bcolz operations to go faster than using a traditional data container like
 those in NumPy or Pandas. That is actually already the case in some real-life
 scenarios (see the notebook above) but that will become pretty more noticeable
 in combination with forthcoming, faster CPUs integrating more cores and wider
-vector units. ## Requisites - Python >= 3.7 - NumPy >= 1.16.5, <1.23 (1.23 is
-not supported yet) - Cython >= 0.22 (just for compiling the beast) - C-Blosc >=
-1.8.0 (optional, as the internal Blosc will be used by default) Optional: -
-numexpr >= 2.5.2 - dask >= 0.9.0 - pandas - tables (pytables) ## Installing as
-wheel There are wheels for Linux and Mac OS X that you can install with
-```python pip install bcolz-zipline ``` Then also install NumPy with and test
-your installation with ```python python -c 'import bcolz;bcolz.test()' ``` ##
-Building There are different ways to compile bcolz, depending on whether you
-want to link with an already installed Blosc library or not. ### Compiling with
-an installed Blosc library (recommended) Python and Blosc-powered extensions
-have a difficult relationship when compiled using GCC, so this is why using an
-external C-Blosc library is recommended for maximum performance (for details,
-see
+vector units. ## Requisites - Python >= 3.8 - NumPy >= 1.16.5, <1.23 (1.23 is
+not supported yet) - Cython >= 0.22 (Python 3.12 > 3) (just for compiling the
+beast) - C-Blosc >= 1.8.0 (optional, as the internal Blosc will be used by
+default) Optional: - numexpr >= 2.5.2 - dask >= 0.9.0 - pandas - tables
+(pytables) ## Installing as wheel There are wheels for Linux and Mac OS X that
+you can install with ```python pip install bcolz-zipline ``` Then also install
+NumPy with and test your installation with ```python python -c 'import
+bcolz;bcolz.test()' ``` ## Building There are different ways to compile bcolz,
+depending on whether you want to link with an already installed Blosc library
+or not. ### Compiling with an installed Blosc library (recommended) Python and
+Blosc-powered extensions have a difficult relationship when compiled using GCC,
+so this is why using an external C-Blosc library is recommended for maximum
+performance (for details, see
 github.com/Blosc/python-blosc/issues/110>). Go to
 github.com/Blosc/c-blosc/releases> and download and install the C-Blosc
 library. Then, you can tell bcolz where is the C-Blosc library in a couple of
 ways: Using an environment variable: ``` {.sourceCode .console} $ BLOSC_DIR=/
 usr/local (or "set BLOSC_DIR=\blosc" on Win) $ export BLOSC_DIR (not needed on
 Win) $ python setup.py build_ext --inplace ``` Using a flag: ``` {.sourceCode
 .console} $ python setup.py build_ext --inplace --blosc=/usr/local ``` ###
```

### Comparing `bcolz-zipline-1.2.6/bcolz_zipline.egg-info/SOURCES.txt` & `bcolz_zipline-1.2.9/bcolz_zipline.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 .coverage
 .coveragerc
 .gitignore
-.mailmap
 ANNOUNCE.rst
 CODE_OF_CONDUCT.md
 DISK_FORMAT_v1.rst
 MANIFEST.in
 README.md
 RELEASE_NOTES.rst
 THANKS.rst
@@ -96,17 +95,14 @@
 bench_asv/README_asv.md
 bench_asv/asv.conf.json
 bench_asv/bench/__init__.py
 bench_asv/bench/arange.py
 bench_asv/bench/bench_helper.py
 bench_asv/bench/column_iter.py
 bench_asv/bench/concat.py
-c-blosc/.editorconfig
-c-blosc/.gitignore
-c-blosc/.mailmap
 c-blosc/ANNOUNCE.rst
 c-blosc/CMakeLists.txt
 c-blosc/COMPILING_WITH_WHEELS.rst
 c-blosc/CONTRIBUTING.md
 c-blosc/FUNDING.yml
 c-blosc/README.md
 c-blosc/README_CHUNK_FORMAT.rst
@@ -114,16 +110,14 @@
 c-blosc/RELEASE_NOTES.rst
 c-blosc/RELEASING.rst
 c-blosc/THANKS.rst
 c-blosc/THOUGHTS_FOR_2.0.txt
 c-blosc/blosc.pc.in
 c-blosc/cmake_uninstall.cmake.in
 c-blosc/code_of_conduct.md
-c-blosc/.github/workflows/cmake.yml
-c-blosc/.github/workflows/fuzz.yml
 c-blosc/LICENSES/BITSHUFFLE.txt
 c-blosc/LICENSES/BLOSC.txt
 c-blosc/LICENSES/FASTLZ.txt
 c-blosc/LICENSES/LZ4.txt
 c-blosc/LICENSES/SNAPPY.txt
 c-blosc/LICENSES/STDINT.txt
 c-blosc/LICENSES/ZLIB.txt
```

### Comparing `bcolz-zipline-1.2.6/bench/column-iter.py` & `bcolz_zipline-1.2.9/bench/column-iter.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/concat.py` & `bcolz_zipline-1.2.9/bench/concat.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/ctable-query.py` & `bcolz_zipline-1.2.9/bench/ctable-query.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/eval-profile.py` & `bcolz_zipline-1.2.9/bench/eval-profile.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/eval.py` & `bcolz_zipline-1.2.9/bench/eval.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/expression.py` & `bcolz_zipline-1.2.9/bench/expression.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/fromiter.py` & `bcolz_zipline-1.2.9/bench/fromiter.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/getitem.py` & `bcolz_zipline-1.2.9/bench/getitem.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/iter.py` & `bcolz_zipline-1.2.9/bench/iter.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/iterator.py` & `bcolz_zipline-1.2.9/bench/iterator.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/iterblocks.py` & `bcolz_zipline-1.2.9/bench/iterblocks.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/large_carray.py` & `bcolz_zipline-1.2.9/bench/large_carray.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/multithreaded_copy.ipynb` & `bcolz_zipline-1.2.9/bench/multithreaded_copy.ipynb`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/objpickles.py` & `bcolz_zipline-1.2.9/bench/objpickles.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/pandas-fromdataframe-strings.py` & `bcolz_zipline-1.2.9/bench/pandas-fromdataframe-strings.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/pandas-fromdataframe.py` & `bcolz_zipline-1.2.9/bench/pandas-fromdataframe.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/pandas-todataframe.py` & `bcolz_zipline-1.2.9/bench/pandas-todataframe.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/pytables-fromhdf5.py` & `bcolz_zipline-1.2.9/bench/pytables-fromhdf5.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/pytables-tohdf5.py` & `bcolz_zipline-1.2.9/bench/pytables-tohdf5.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/query.py` & `bcolz_zipline-1.2.9/bench/query.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/serialization.py` & `bcolz_zipline-1.2.9/bench/serialization.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/sum.py` & `bcolz_zipline-1.2.9/bench/sum.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/whereblocks.py` & `bcolz_zipline-1.2.9/bench/whereblocks.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench/zlib-vs-cblosc-zlib.ipynb` & `bcolz_zipline-1.2.9/bench/zlib-vs-cblosc-zlib.ipynb`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench_asv/asv.conf.json` & `bcolz_zipline-1.2.9/bench_asv/asv.conf.json`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench_asv/bench/arange.py` & `bcolz_zipline-1.2.9/bench_asv/bench/arange.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench_asv/bench/column_iter.py` & `bcolz_zipline-1.2.9/bench_asv/bench/column_iter.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/bench_asv/bench/concat.py` & `bcolz_zipline-1.2.9/bench_asv/bench/concat.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/ANNOUNCE.rst` & `bcolz_zipline-1.2.9/c-blosc/ANNOUNCE.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/CMakeLists.txt` & `bcolz_zipline-1.2.9/c-blosc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/COMPILING_WITH_WHEELS.rst` & `bcolz_zipline-1.2.9/c-blosc/COMPILING_WITH_WHEELS.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/CONTRIBUTING.md` & `bcolz_zipline-1.2.9/c-blosc/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/LICENSES/BITSHUFFLE.txt` & `bcolz_zipline-1.2.9/c-blosc/LICENSES/BITSHUFFLE.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/LICENSES/BLOSC.txt` & `bcolz_zipline-1.2.9/c-blosc/LICENSES/BLOSC.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/LICENSES/FASTLZ.txt` & `bcolz_zipline-1.2.9/c-blosc/LICENSES/FASTLZ.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/LICENSES/LZ4.txt` & `bcolz_zipline-1.2.9/c-blosc/LICENSES/LZ4.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/LICENSES/SNAPPY.txt` & `bcolz_zipline-1.2.9/c-blosc/LICENSES/SNAPPY.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/LICENSES/STDINT.txt` & `bcolz_zipline-1.2.9/c-blosc/LICENSES/STDINT.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/LICENSES/ZLIB.txt` & `bcolz_zipline-1.2.9/c-blosc/LICENSES/ZLIB.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/README.md` & `bcolz_zipline-1.2.9/c-blosc/README.md`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/README_CHUNK_FORMAT.rst` & `bcolz_zipline-1.2.9/c-blosc/README_CHUNK_FORMAT.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/README_THREADED.rst` & `bcolz_zipline-1.2.9/c-blosc/README_THREADED.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/RELEASE_NOTES.rst` & `bcolz_zipline-1.2.9/c-blosc/RELEASE_NOTES.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/RELEASING.rst` & `bcolz_zipline-1.2.9/c-blosc/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/THANKS.rst` & `bcolz_zipline-1.2.9/c-blosc/THANKS.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/THOUGHTS_FOR_2.0.txt` & `bcolz_zipline-1.2.9/c-blosc/THOUGHTS_FOR_2.0.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/bench/CMakeLists.txt` & `bcolz_zipline-1.2.9/c-blosc/bench/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/bench/Makefile` & `bcolz_zipline-1.2.9/c-blosc/bench/Makefile`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/bench/Makefile.mingw` & `bcolz_zipline-1.2.9/c-blosc/bench/Makefile.mingw`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/bench/bench.c` & `bcolz_zipline-1.2.9/c-blosc/bench/bench.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/bench/plot-speeds.py` & `bcolz_zipline-1.2.9/c-blosc/bench/plot-speeds.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/CMakeLists.txt` & `bcolz_zipline-1.2.9/c-blosc/blosc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/bitshuffle-avx2.c` & `bcolz_zipline-1.2.9/c-blosc/blosc/bitshuffle-avx2.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/bitshuffle-avx2.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/bitshuffle-avx2.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/bitshuffle-generic.c` & `bcolz_zipline-1.2.9/c-blosc/blosc/bitshuffle-generic.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/bitshuffle-generic.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/bitshuffle-generic.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/bitshuffle-sse2.c` & `bcolz_zipline-1.2.9/c-blosc/blosc/bitshuffle-sse2.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/bitshuffle-sse2.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/bitshuffle-sse2.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/blosc-common.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/blosc-common.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/blosc-comp-features.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/blosc-comp-features.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/blosc-export.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/blosc-export.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/blosc.c` & `bcolz_zipline-1.2.9/c-blosc/blosc/blosc.c`

 * *Files 0% similar despite different names*

```diff
@@ -539,23 +539,23 @@
     if (compversion != BLOSC_LZ4_VERSION_FORMAT) {
       return -9;
     }
     context->decompress_func = &lz4_wrap_decompress;
     return 0;
   }
 #endif /*  HAVE_LZ4 */
-//#if defined(HAVE_SNAPPY)
-//  if (compformat == BLOSC_SNAPPY_FORMAT) {
-//    if (compversion != BLOSC_SNAPPY_VERSION_FORMAT) {
-//      return -9;
-//    }
-//    context->decompress_func = &snappy_wrap_decompress;
-//    return 0;
-//  }
-//#endif /*  HAVE_SNAPPY */
+#if defined(HAVE_SNAPPY)
+  if (compformat == BLOSC_SNAPPY_FORMAT) {
+    if (compversion != BLOSC_SNAPPY_VERSION_FORMAT) {
+      return -9;
+    }
+    context->decompress_func = &snappy_wrap_decompress;
+    return 0;
+  }
+#endif /*  HAVE_SNAPPY */
 #if defined(HAVE_ZLIB)
   if (compformat == BLOSC_ZLIB_FORMAT) {
     if (compversion != BLOSC_ZLIB_VERSION_FORMAT) {
       return -9;
     }
     context->decompress_func = &zlib_wrap_decompress;
     return 0;
```

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/blosc.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/blosc.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/blosclz.c` & `bcolz_zipline-1.2.9/c-blosc/blosc/blosclz.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/blosclz.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/blosclz.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/fastcopy.c` & `bcolz_zipline-1.2.9/c-blosc/blosc/fastcopy.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/fastcopy.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/fastcopy.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/shuffle-avx2.c` & `bcolz_zipline-1.2.9/c-blosc/blosc/shuffle-avx2.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/shuffle-avx2.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/shuffle-avx2.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/shuffle-generic.c` & `bcolz_zipline-1.2.9/c-blosc/blosc/shuffle-generic.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/shuffle-generic.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/shuffle-generic.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/shuffle-sse2.c` & `bcolz_zipline-1.2.9/c-blosc/blosc/shuffle-sse2.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/shuffle-sse2.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/shuffle-sse2.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/shuffle.c` & `bcolz_zipline-1.2.9/c-blosc/blosc/shuffle.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/shuffle.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/shuffle.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/win32/pthread.c` & `bcolz_zipline-1.2.9/c-blosc/blosc/win32/pthread.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/win32/pthread.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/win32/pthread.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/blosc/win32/stdint-windows.h` & `bcolz_zipline-1.2.9/c-blosc/blosc/win32/stdint-windows.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/cmake_uninstall.cmake.in` & `bcolz_zipline-1.2.9/c-blosc/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/CMakeLists.txt` & `bcolz_zipline-1.2.9/c-blosc/compat/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.11.1-blosclz.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.11.1-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.11.1-lz4.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.11.1-lz4.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.11.1-lz4hc.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.11.1-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.11.1-snappy.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.11.1-snappy.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.11.1-zlib.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.11.1-zlib.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.11.1-zstd.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.11.1-zstd.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.14.0-blosclz.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.14.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.14.0-lz4.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.14.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.14.0-lz4hc.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.14.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.14.0-snappy.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.14.0-snappy.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.14.0-zlib.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.14.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.14.0-zstd.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.14.0-zstd.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-blosclz-bitshuffle.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-blosclz-bitshuffle.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-blosclz.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-lz4-bitshuffle.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-lz4-bitshuffle.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-lz4.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-lz4hc.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-zlib.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.18.0-zstd.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.18.0-zstd.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.3.0-blosclz.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.3.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.3.0-lz4.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.3.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.3.0-lz4hc.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.3.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.3.0-snappy.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.3.0-snappy.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.3.0-zlib.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.3.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.7.0-blosclz.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.7.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.7.0-lz4.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.7.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.7.0-lz4hc.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.7.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.7.0-snappy.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.7.0-snappy.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/blosc-1.7.0-zlib.cdata` & `bcolz_zipline-1.2.9/c-blosc/compat/blosc-1.7.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/compat/filegen.c` & `bcolz_zipline-1.2.9/c-blosc/compat/filegen.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/examples/README.rst` & `bcolz_zipline-1.2.9/c-blosc/examples/README.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/examples/many_compressors.c` & `bcolz_zipline-1.2.9/c-blosc/examples/many_compressors.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/examples/multithread.c` & `bcolz_zipline-1.2.9/c-blosc/examples/multithread.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/examples/noinit.c` & `bcolz_zipline-1.2.9/c-blosc/examples/noinit.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/examples/simple.c` & `bcolz_zipline-1.2.9/c-blosc/examples/simple.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/examples/win-dynamic-linking.c` & `bcolz_zipline-1.2.9/c-blosc/examples/win-dynamic-linking.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/lz4-1.9.3/lz4.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/lz4-1.9.3/lz4.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/lz4-1.9.3/lz4.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/lz4-1.9.3/lz4.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/lz4-1.9.3/lz4hc.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/lz4-1.9.3/lz4hc.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/lz4-1.9.3/lz4hc.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/lz4-1.9.3/lz4hc.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/adler32.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/adler32.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/compress.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/compress.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/crc32.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/crc32.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/crc32.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/crc32.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/deflate.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/deflate.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/deflate.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/deflate.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/gzclose.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/gzclose.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/gzguts.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/gzguts.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/gzlib.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/gzlib.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/gzread.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/gzread.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/gzwrite.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/gzwrite.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/infback.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/infback.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inffast.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inffast.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inffixed.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inffixed.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inflate.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inflate.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inflate.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inflate.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inftrees.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inftrees.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/inftrees.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/inftrees.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/trees.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/trees.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/trees.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/trees.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/uncompr.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/uncompr.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/zconf.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/zconf.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/zlib.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/zlib.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/zutil.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/zutil.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zlib-1.2.8/zutil.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zlib-1.2.8/zutil.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/BUCK` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/BUCK`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/Makefile` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/Makefile`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/README.md` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/bitstream.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/compiler.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/compiler.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/cpu.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/cpu.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/debug.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/debug.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/debug.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/debug.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/entropy_common.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/error_private.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/error_private.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/error_private.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/error_private.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/fse.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/fse.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/fse_decompress.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/huf.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/huf.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/mem.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/mem.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/pool.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/pool.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/pool.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/pool.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/threading.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/threading.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/threading.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/threading.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/xxhash.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/xxhash.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_common.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_deps.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_errors.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_internal.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/fse_compress.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/fse_compress.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/hist.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/hist.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/hist.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/hist.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/huf_compress.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/huf_compress.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_internal.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_internal.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_literals.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_literals.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_literals.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_literals.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_sequences.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_sequences.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_sequences.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_sequences.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_superblock.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_superblock.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_superblock.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_compress_superblock.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_cwksp.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_cwksp.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_double_fast.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_double_fast.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_double_fast.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_double_fast.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_fast.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_fast.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_fast.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_fast.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_lazy.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_lazy.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_lazy.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_lazy.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_ldm.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_ldm.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_ldm.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_ldm.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_opt.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_opt.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_opt.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstd_opt.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstdmt_compress.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstdmt_compress.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/compress/zstdmt_compress.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/compress/zstdmt_compress.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/huf_decompress.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_ddict.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_ddict.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress_block.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress_block.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress_internal.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff_common.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff_common.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff_compress.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff_compress.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff_decompress.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/deprecated/zbuff_decompress.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/cover.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/cover.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/cover.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/cover.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/divsufsort.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/divsufsort.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/divsufsort.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/divsufsort.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/fastcover.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/fastcover.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/zdict.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/zdict.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/zdict.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dictBuilder/zdict.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dll/example/Makefile` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dll/example/Makefile`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dll/example/README.md` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dll/example/README.md`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dll/example/build_package.bat` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dll/example/build_package.bat`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dll/example/fullbench-dll.sln` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dll/example/fullbench-dll.sln`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/dll/example/fullbench-dll.vcxproj` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/dll/example/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_legacy.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_legacy.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v01.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v01.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v01.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v01.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v02.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v02.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v02.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v02.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v03.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v03.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v03.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v03.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v04.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v04.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v04.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v04.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v05.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v05.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v05.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v05.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v06.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v06.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v06.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v06.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v07.c` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v07.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v07.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/legacy/zstd_v07.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/internal-complibs/zstd-1.4.8/zstd.h` & `bcolz_zipline-1.2.9/c-blosc/internal-complibs/zstd-1.4.8/zstd.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/CMakeLists.txt` & `bcolz_zipline-1.2.9/c-blosc/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/Makefile` & `bcolz_zipline-1.2.9/c-blosc/tests/Makefile`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/check_symbols.py` & `bcolz_zipline-1.2.9/c-blosc/tests/check_symbols.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/fuzz/CMakeLists.txt` & `bcolz_zipline-1.2.9/c-blosc/tests/fuzz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/fuzz/fuzz_compress.c` & `bcolz_zipline-1.2.9/c-blosc/tests/fuzz/fuzz_compress.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/fuzz/fuzz_decompress.c` & `bcolz_zipline-1.2.9/c-blosc/tests/fuzz/fuzz_decompress.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/fuzz/standalone.c` & `bcolz_zipline-1.2.9/c-blosc/tests/fuzz/standalone.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/gcc-segfault-issue.c` & `bcolz_zipline-1.2.9/c-blosc/tests/gcc-segfault-issue.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/print_versions.c` & `bcolz_zipline-1.2.9/c-blosc/tests/print_versions.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_api.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_api.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_bitshuffle_leftovers.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_bitshuffle_leftovers.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_common.h` & `bcolz_zipline-1.2.9/c-blosc/tests/test_common.h`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_compress_roundtrip.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_compress_roundtrip.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_compress_roundtrip.csv` & `bcolz_zipline-1.2.9/c-blosc/tests/test_compress_roundtrip.csv`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_compressor.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_compressor.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_forksafe.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_forksafe.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_getitem.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_getitem.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_getitem.csv` & `bcolz_zipline-1.2.9/c-blosc/tests/test_getitem.csv`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_maxout.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_maxout.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_noinit.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_noinit.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_nolock.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_nolock.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_nthreads.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_nthreads.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_shuffle_roundtrip_avx2.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_shuffle_roundtrip_avx2.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_shuffle_roundtrip_avx2.csv` & `bcolz_zipline-1.2.9/c-blosc/tests/test_shuffle_roundtrip_avx2.csv`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_shuffle_roundtrip_generic.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_shuffle_roundtrip_generic.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_shuffle_roundtrip_generic.csv` & `bcolz_zipline-1.2.9/c-blosc/tests/test_shuffle_roundtrip_generic.csv`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_shuffle_roundtrip_sse2.c` & `bcolz_zipline-1.2.9/c-blosc/tests/test_shuffle_roundtrip_sse2.c`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/c-blosc/tests/test_shuffle_roundtrip_sse2.csv` & `bcolz_zipline-1.2.9/c-blosc/tests/test_shuffle_roundtrip_sse2.csv`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/conda.recipe/meta.yaml` & `bcolz_zipline-1.2.9/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/continuous-integration/appveyor/install.ps1` & `bcolz_zipline-1.2.9/continuous-integration/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/continuous-integration/appveyor/run_with_env.cmd` & `bcolz_zipline-1.2.9/continuous-integration/appveyor/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/cpuinfo.py` & `bcolz_zipline-1.2.9/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/Makefile` & `bcolz_zipline-1.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/bcolz.png` & `bcolz_zipline-1.2.9/docs/bcolz.png`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/conf.py` & `bcolz_zipline-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/defaults.rst` & `bcolz_zipline-1.2.9/docs/defaults.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/favicon.ico` & `bcolz_zipline-1.2.9/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/install.rst` & `bcolz_zipline-1.2.9/docs/install.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/intro.rst` & `bcolz_zipline-1.2.9/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/make.bat` & `bcolz_zipline-1.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/my_package/my_extension/example_ext.pyx` & `bcolz_zipline-1.2.9/docs/my_package/my_extension/example_ext.pyx`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/opt-tips.rst` & `bcolz_zipline-1.2.9/docs/opt-tips.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/reference.rst` & `bcolz_zipline-1.2.9/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/tutorial.rst` & `bcolz_zipline-1.2.9/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/tutorial_carray.ipynb` & `bcolz_zipline-1.2.9/docs/tutorial_carray.ipynb`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/tutorial_carray_memory_profile.ipynb` & `bcolz_zipline-1.2.9/docs/tutorial_carray_memory_profile.ipynb`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/tutorial_ctable.ipynb` & `bcolz_zipline-1.2.9/docs/tutorial_ctable.ipynb`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/docs/tutorials.ipynb` & `bcolz_zipline-1.2.9/docs/tutorials.ipynb`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/examples/querying-ranges.ipynb` & `bcolz_zipline-1.2.9/examples/querying-ranges.ipynb`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/persistence.rst` & `bcolz_zipline-1.2.9/persistence.rst`

 * *Files identical despite different names*

### Comparing `bcolz-zipline-1.2.6/pyproject.toml` & `bcolz_zipline-1.2.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bcolz-zipline"
-version = "1.2.6"
+dynamic = ["version"]
 requires-python = ">=3.7"
 dependencies = [
     "numpy >=1.16"
 ]
 
 description = "Columnar and compressed data containers."
 readme = "README.md"
@@ -24,19 +24,19 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: Unix",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12"
 ]
 license = { file = "LICENSES/BCOLZ.txt" }
 
 [project.urls]
 repository = "https://github.com/stefan-jansen/bcolz-zipline"
 
 [build-system]
@@ -81,8 +81,8 @@
 # Optional: support Universal2 for Apple Silicon with these two lines:
 [tool.cibuildwheel.macos]
 archs = ["x86_64", "arm64", "universal2"]
 test-skip = ["*universal2:arm64"]
 
 [tools.pytest]
 testpaths = "bcolz/tests"
-addopts = "-v"
+addopts = "-v"
```

### Comparing `bcolz-zipline-1.2.6/setup.py` & `bcolz_zipline-1.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from sys import version_info as v
 
 import setuptools_scm  # noqa: F401
 import toml  # noqa: F401
 
 # Check this Python version is supported
-if any([(3,) < v < (3, 7)]):
-    raise Exception("Unsupported Python version %d.%d. Requires Python > 3.6." % v[:2])
+if any([(3,) < v < (3, 8)]):
+    raise Exception("Unsupported Python version %d.%d. Requires Python > 3.7." % v[:2])
 
 import os
 from glob import glob
 import sys
 
 from setuptools import setup, Extension
 from pkg_resources import resource_filename
@@ -88,15 +88,15 @@
 # Allow setting the Blosc dir if installed in the system
 BLOSC_DIR = os.environ.get('BLOSC_DIR', '')
 
 # Sources & libraries
 inc_dirs = ['bcolz']
 lib_dirs = []
 libs = []
-def_macros = []
+def_macros = [("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION")]
 sources = ['bcolz/carray_ext.pyx']
 
 # Handle --blosc=[PATH] --lflags=[FLAGS] --cflags=[FLAGS]
 args = sys.argv[:]
 for arg in args:
     if arg.find('--blosc=') == 0:
         BLOSC_DIR = os.path.expanduser(arg.split('=')[1])
```

